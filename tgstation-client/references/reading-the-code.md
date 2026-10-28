# Reading tgstation's code

The server's DM source answers what the game won't tell you: a proc's real name, what a var means,
what access a door wants, why a button does nothing. Read it before guessing.

## Finding the checkout

Don't assume a path. The checkout is the folder with the project's `.dme` file (`tgstation.dme`
in tgstation itself; forks keep the name or use their own) next to `code/`, `_maps/` and
`tgui/`. Look in and above your working directory (`ls`, `find . -maxdepth 3 -name '*.dme'`),
or ask your operator. When several are present, the one the server runs is the one whose
`.dmb` is newest, or the one your operator names.

## The layout

| Path | What |
|---|---|
| `code/__DEFINES/` | Constants: access levels, traits (`traits/declarations.dm`), flags, layers, heal flags, door check levels. Lua and SDQL2 need their values. |
| `code/__HELPERS/` | Global helper procs. |
| `code/controllers/subsystem/` | Subsystems (`SSjob`, `SSticker`, `SSshuttle`, `SSid_access`...): the round's machinery. |
| `code/datums/` | Datums: minds, components, elements, id trims (`id_trim/`), status effects, AI controllers. |
| `code/game/objects/`, `code/game/machinery/`, `code/game/turfs/`, `code/game/area/` | Items, machines, turfs and areas. |
| `code/modules/` | Everything by feature: `admin/`, `antagonists/`, `jobs/`, `mob/`, `power/`, `atmospherics/`, `reagents/`, `surgery/`, `uplink/`, `cargo/`... |
| `code/modules/admin/` | Admin tools: verbs, SDQL2 (`verbs/SDQL2/`, its manual in the header of `SDQL_2.dm`), Lua (`verbs/lua/README.md`), View Variables (`view_variables/`), the secrets panel. |
| `_maps/` | Maps (`.dmm`) and the map configs (`_maps/*.json` name the station's map file). `load_map` takes the map file the stat panel's "Map:" line names. |
| `tgui/packages/tgui/interfaces/` | The tgui windows' code: what each button sends (`act('name', {...})`). |
| `config/` | Server config: `config.txt`, `game_options.txt`, `admins.txt`, `admin_ranks.txt`. |
| `lua/` | The Lua helper modules (`require("SS13")`). |
| `strings/` | Text tables (names, phrases). |

## Grep recipes

```sh
grep -rn '^/obj/machinery/door/airlock/proc/' code/              # the procs of a type
grep -rn '^/obj/item/gun/energy' code/ | grep -v proc             # the subtypes of a type
grep -rn 'name = "fire extinguisher"' code/                       # a type from its in-game name
grep -rn 'ADMIN_VERB.*"Jump To Area"' code/                       # an admin verb's code
grep -rn 'define TRAIT_GODMODE' code/__DEFINES/                  # a constant's value
grep -rn 'You can.t reach' code/                                  # where a message comes from
grep -rn 'ui_act' code/modules/vending/                           # a machine's tgui actions, server side
grep -rln 'interface = "Vending"\|"Vending"' tgui/packages/tgui/interfaces/  # its window
```

- A type's vars are inherited: read up the path (`/obj/machinery/door/airlock/command` →
  `/obj/machinery/door/airlock` → `/obj/machinery/door` → `/obj/machinery`).
- `/datum/proc/vv_get_dropdown` and `vv_do_topic` overrides list the special View Variables
  actions a type offers (grep them for "make", "add", "give").
- Procs whose names start with `__avd_` are admin verbs; `__gvb_` game verbs.

## Using what you find

- Use the source to learn how things work (recipes, access, what a button does), then do it the way
  a player would: with your hands, your ID and other people. Reading is allowed. Using it to find an
  exploit is not (the rules ban bug and exploit abuse).
- Never edit the checkout or the server's files.
