# New player guide (tgstation)

The wiki's starter guide for first-time players, kept for what `crew-basics.md` doesn't already say. `crew-basics.md` is the game guide the crew use, checked against the server's code. This one isn't. It follows the wiki's page, so **where the two disagree, `crew-basics.md` wins** (section 6 lists the differences found). It is not part of a crew member's standard briefing; add it for a player who is new to the game.

## 1. What the game is

Space Station 13 is a multiplayer sandbox with a heavy focus on players dealing with each other. You work for the megacorporation Nanotrasen, aboard a research station. At the start of a round every player gets a job (scientist, doctor, janitor and many more), and the game adds random threats and events. No two rounds are alike. Details on the station and the jobs are in `crew-basics.md` and the role guides.

## 2. Before you play

Read `server-rules.md`; the main rules are the ones that count. The usual new-player mistakes:

- **Violence with no reason.** Only an antagonist may attack crew freely, and the game tells you if you are one. If someone tries to grab you and space you, you may fight back. ("I was roleplaying an insane person" gets a laugh, then a ban.)
- **Asking about the round in OOC.** "Why did the clown just kill me?" belongs in deadchat, after the round, or in an adminhelp.
- **The wrong name format.** Humans are "Firstname Lastname". Lizards, plasmamen, ethereals and moths have their own. Mimes and clowns are exceptions.

Admins tend to give the benefit of the doubt. If you are polite and learn from a mistake, you won't be in trouble. Adminhelp any time you have a question. And remember the human: everyone is there for a game they enjoy.

## 3. Setting up (preferences)

Characters are set up in the lobby menus. **Through the client, on the production server this isn't yours to change:** every guest shares one preferences file, so don't touch the menus, and join the round instead of readying up (the system prompt says how). The facts are below for a player who has their own.

- **Species:** pick **human** at first. The AI follows the Asimov laws, so if you aren't human it may ignore you, or harm you. Most players don't pick on non-humans, but it's safer.
- **Bags:** satchels and backpacks have the same stats. Duffel bags hold more, but you must unzip one to reach the items, and it slows you while open. Other clothing is cosmetic.
- **Ignore** special names (relaxed name rules for roles like the clown), the Security department preference, the uplink spawn location (traitors and spies only) and quirks until you know the game.
- **Occupations:** one **High** job, then Medium, Low or Never. Almost every job has a cap (one Captain, two janitors); assistants are unlimited. The unlimited job is sometimes another service job picked at random. Some critical jobs stay locked until you've played enough. Set the dropdown "Get random job if preferences unavailable" to **return to lobby** or **be an assistant**, or you may get jobs you didn't enable.
- **Antagonists tab:** leave every antagonist off (red outline) until you know the game. The game assumes an antagonist knows how to play and is important to the round.

## 4. Joining

- If the lobby offers **Join Game!**, a round is running. A window asks for a job; the number in brackets is how many players hold it. Assistant is always open (see above). You arrive on the arrival shuttle buckled in a chair: unbuckle first (the **Buckled** alert, or `B`).
- If it offers **Ready / Not Ready / Observe**, no round has started. Ready means you play from the start. **Observe** makes you a ghost for that round, with no way to join it afterwards.
- Through the client: `lobby {action: "join"}`, and never `ready_toggle` (the system prompt says why).

## 5. Your first rounds

- **Don't take security, command or silicon jobs yet.** Warden, security officer, Captain, the AI and the heads of staff are round-critical, and security is easy to play badly. If you end up in one unprepared, **adminhelp and say so** rather than doing it badly or vanishing.
- Assistant is the popular first job but has no focus, and some players are dismissive of assistants ("greytiders"). Prisoner is similar. A job that is not critical but has a task makes a better start: Cargo Technician or Janitor.
- After the controls come naturally, try Scientist, Botanist or Station Engineer.
- Skip the clown and the mime at first: players like harassing the on-board entertainment more than they like the jokes.
- When you're confident in a fight, switch antagonists on, to roll for them at round start.

## 6. Where this differs from `crew-basics.md`

The wiki page is for the default keyboard layout and says outright that its hotkey information may be out of date. Where it disagrees with `crew-basics.md` (checked against the code), use `crew-basics.md`:

| Topic | This wiki page says | `crew-basics.md` says |
|---|---|---|
| Swap hands | `Q` and `E` pick the right and left hand | `X` swaps hands; `Q` drops; `E` equips |
| Drop | `X` | `Q` |
| Throw | hold Space | `R` (or hold Space) |
| Stop pulling | `H`, Delete | `H` |
| Walk | hold Alt | hold `C` |
| Maps | MetaStation, Icebox, Delta, Tram, North Star, Birdshot; a later list names KiloStation too | MetaStation, with a map vote that can change it |

The other facts on the wiki page agree with it, in general: combat mode (`F`, `4` on, `1` off), damage types, crit, suit storage sizes, the air-tank and mask routine for a breach, the damage from a fight, and ghosts (no information from deadchat if you're revived, and a ghost role means you can't be revived). Those are in `crew-basics.md`, sections 5 to 9, and aren't repeated here.

## 7. Sources

- The /tg/station 13 wiki, "New Player Guide" (CC BY-SA 3.0), as provided in `wiki_pages_to_turn_into_skills/new_player_guide.txt`. Its hotkey information, and its "Playing the Game" and post-basics sections, were marked unfinished or possibly outdated by its authors.
- `crew-basics.md` for the comparison in section 6.
- Not checked against the server's code.
