# Writing scripts (run_script)

`run_script` runs Python against the same game session as the other tools. It
exists so multi-step work doesn't cost one tool call and one answer per step:
one script can look, decide, walk, click, and read a window, then report once.

## Reusable beats clever: build a script library

Default to **reusable scripts, not one-off snippets**. Break every task into
small, single-purpose parts and keep the parts. A task like "unbuckle, leave
the shuttle, get to the bar" is then *composed* of pieces you already have;
only the glue is new. Over a session the library grows, and each new task gets
cheaper.

Starters in the seeker-mcp repo under `scripts/examples/`:

- `status_probe.py` — a cheap heartbeat (where am I, what's pending)
- `goto_area.py` — walk to an area by name (`args: {area: "Medbay Lobby"}`)
- `unbuckle_to_bar.py` — unbuckle, walk out of the arrival shuttle, walk on
- `machine_flow.py` — open a machine, read its window, press its buttons
- `chat_watch.py` — wait for chat and report it

Rules of thumb:

1. **One script = one thing.** `unbuckle`, `goto_area`, `open_machine`,
   `watch_chat`. Top-level task scripts stay thin: they call the components
   with `args` and judge the results.
2. **Behavior comes from `args`, never from edited code.** The same
   `goto_area.py` serves "Bar" and "Medbay Lobby". A script with a hardcoded
   destination is a one-off, not a component. (And passing values as `args`
   keeps the envelope's digest honest — never splice values into code text.)
3. **Guard on state before acting.** Check the "Buckled" alert is actually up
   before clicking a seat (an empty seat under an empty hand sits you back
   down); check the shuttle has docked before walking out. Log what you
   checked.
4. **Return a structured verdict.** The last bare expression is the `result`:
   a dict with `ok`, where you ended up, and what failed and why (truncate
   `.text` of the failed answer). `print()` progress into `logs` so a failed
   run is readable without rerunning it.
5. **Check `.failed` on every answer.** A call answering is not proof the game
   applied it. The `bot.*` composites already verify; prefer them over raw
   `sk.*` when one exists.
6. **Retries are cheap inside a script.** Wrap flaky phases (shuttle still in
   hyperspace, door queueing) in a small loop with `sk.wait(s)` between
   attempts, with a bounded number of tries.
7. **Save new components** next to the examples, with a docstring line showing
   the `run_script` invocation and its args. Name them for the act, not the
   task: `goto_area.py`, not `go_to_medbay_from_bar.py`.

## The envelope

Every run answers `{ok, result, logs, error{kind, message}, elapsed_ms,
digest}`. `ok` says the script finished — your own verdict lives in the
result. `error.kind`: `exception` (bug in the script), `timeout` (raise
`timeout_s` for long walks), `cancelled` (rerun with `{cancel: true}` to stop
the current script), `not_connected`, `invalid_input`. `digest` lists what
changed in the session around the run.

## The environment

Globals in every script: `sk`, `bot`, `call`, `args`, `Answer`,
`wait_for_chat`, `wait_for_window`, `wait_until`, `json`, `re`, `time`,
`random`. Stdlib only, no pip installs.

- `sk.*` — one thin method per remote tool; the answer is what the game says,
  parsed into an `Answer` (`.text`, `.facts`, `.ok`, `.failed`, `.rev`).
- `bot.*` — verified composites: `goto`, `goto_area`, `find`, `click_thing`,
  `open_machine`, `say`, `reply`, `handle_alert`, `snapshot`. Check `.failed`.
- Full reference: `sdk/API.md` in the seeker-mcp repo.

## Conventions and gotchas

- **One script at a time.** A script holds the session: while it walks, no
  other tool call should move the mob. Cancel with `run_script {cancel: true}`.
- **`load_map` once per session** with the server's `.dmm` path (the repo the
  `.dmb` was built from), so `walk_to` plans over unseen tiles and area names
  resolve from the map. Afterwards it stays loaded.
- **Area names:** `search {query: "medbay", kind: "area"}` lists what the map
  knows. Some areas are access-gated: "Bar" is staff-only, and `walk_to`
  detours to the public side and says so — read the `instead:` line.
- **Refusals never raise.** A refused or errored call comes back as an
  `Answer` with `.failed` and the reason in `.text`; only transport trouble
  (wrapper down) raises. Expect an exception only for your own bugs.
- **Idempotence helps.** A component run twice in a row should not do damage:
  "unbuckle" when not buckled is a no-op, "goto_area" where you already are
  takes zero steps.
- **Keep player rules in the script too.** A script acts as the player: it
  waits for doors, asks for access it lacks, and never assumes admin powers.
