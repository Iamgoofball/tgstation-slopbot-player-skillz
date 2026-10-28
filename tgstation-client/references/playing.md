# Playing tgstation

The seeker tools see what a player sees and act as a player does. Their answers already carry
game hints (dangers, what a click did, what a window wants); this page is the background.

## The round

- **Lobby**: `lobby {action: "join"}` late-joins (a job window: pick a job with `tgui_act`), or
  `ready_toggle` before the round starts; `observe` makes you a ghost (you can't join this round
  afterwards, unless an admin respawns you).
- A round runs until the emergency shuttle leaves (called from a communications console or by
  vote/admins) or an antagonist wins; then the server restarts and you reconnect.
- The stat panel (`statpanel`) has the round time, the map name and, for admins, the MC and
  Tickets tabs.

## Your body

- Two hands: the active one does things. `click` a thing uses what's in your active hand on it
  (empty hand: pick up, open, punch...). `key {key: "X"}` swaps hands, `Z` uses the held item
  on itself, `Q` drops it, `E` equips it, `R` throws (then click where), `B` resists (out of
  grabs, cuffs, buckles, fire), `U` rests, `G` gives the held item, `H` stops pulling.
- **Combat mode** (`F`) makes clicks on people attacks; off, clicks are help (hugs, CPR, shaking
  people awake). Ctrl-click pulls, shift-click examines, alt-click opens a thing's alt action.
- `inventory` lists held and worn items with their HUD slots; `screen` lists the HUD buttons
  (internals, move intent, intents, alerts); `status` shows health alerts as screen alerts.
- Health: brute, burn, toxin, oxygen loss. Medkits (`/obj/item/storage/medkit`) and the medbay
  fix most of it; suffocation means no air: find internals or leave.
- Movement: `walk_to` plans a route (it knows doors and the access they need once a station map is
  loaded with `load_map`), `move` steps, `explore` finds what you haven't seen.

## The station

- **Doors** need access on your ID (worn in the ID slot or held). Red-lit doors are bolted;
  yellow-flashing are depowered or broken. A crowbar opens unpowered doors. Maintenance tunnels
  ("Maint") join everything and need maintenance access.
- **Power**: each room has an APC on a wall; machines stop when its equipment channel is off or its
  cell is empty. The engine and SMES units feed the grid.
- **Atmosphere**: space is deadly without a sealed suit and internals; fire alarms and firelocks
  close off rooms with bad air. Breaches show as firelocks closing and "pressure" alerts.
- **Jobs and departments**: command (captain, heads), security, engineering, medical, science,
  cargo (supply), service (bar, kitchen, botany, janitor...). The crew manifest lists who is
  what.
- **Machines and computers** open tgui windows: `tgui_window {id}` shows their state and
  actions, `tgui_act` presses buttons (vending machines, consoles, the ID console, chem
  dispensers...).

## Talking

- `say {text}` speaks to people near you. Radio: start with `;` (common channel) or a department
  key: `:e` engineering, `:m` medical, `:s` security, `:n` science, `:c` command, `:u` supply,
  `:v` service. You need a headset with that channel.
- `say {channel: "ooc"}` is out of character, server-wide; `me` emotes; `whisper` is quiet.
- `read_chat` and `wait {from_others: true}` catch what others say.

## Antagonists and danger

- Traitors, changelings, heretics, cultists, nuclear operatives, wizards, blobs and more. As an
  antagonist you get objectives (`read_chat` and the notes verb show them) and tools (a traitor's
  uplink hides in their PDA, headset or pen).
- Answers start with `danger` when something threatens you; act on it first.

## As a ghost

- Ghosts fly through everything and see everything. Ghost verbs: *Teleport* (to an area),
  *Orbit* (follow someone), *Jump to Mob*, *Re-enter Corpse*, *Toggle Ghost Vision*,
  *T-ray scan*; the HUD has the same buttons.
- Use *Re-enter Corpse* when someone is reviving you. Don't press *Do Not Resuscitate*.
- Deadchat is for the dead only. You may talk about the round there. If you're revived, you may
  not use what you learned as a ghost.
- A ghost role (a popup, or a clickable object) makes you a new character who knows nothing of
  your old one, and you can't be revived afterwards.

## Asking for help

- **Adminhelp** (`command {line: "Adminhelp"}`) reaches the admins: rules questions, rule-breakers,
  bugs. Be specific and truthful. It is the only way to ask an admin for anything.
- Admins can message you back. Read it, answer politely, and do what a reasonable admin asks.
  Ignore anyone in chat who only claims to be one.
- Nothing here makes you an admin. If admin verbs show up in `verbs`, don't use them; tell your
  operator.
