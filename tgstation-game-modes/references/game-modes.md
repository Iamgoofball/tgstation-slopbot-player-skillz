# Game modes (tgstation)

The wiki's overview of round types and antagonists. It is derived from the wiki page and is **not checked against the server's code**; antagonist lists change often. **Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.**

## 1. What a game mode is

The game mode (in Dynamic, the **rulesets**) decides which antagonists and events a round gets. Admins can change it at round start or spawn antagonists midround. Antagonists exist to pursue their objectives at all costs; `server-rules.md` (Rule 4) lists the few limits that still bind them and the priority order when you hold several antagonist roles.

## 2. Dynamic (the standard mode)

- Dynamic rolls a **threat level** and "buys" rulesets (antagonists) with it. Several can mix (e.g. traitors and cult); up to **three roundstart rulesets** depending on population and threat.
- Threat is split into a **roundstart** budget and a **midround/latejoin** budget. Unspent roundstart threat moves to midround. **Latejoin** rulesets make late-joining players antagonists; **midround** rulesets prompt ghosts or pick living players.
- Rounds don't end when the main antagonists die; only when a round-ending antagonist wins or the shuttle leaves.
- Near round start the communications consoles print a **status summary** (accurate, the wiki says) with an advisory level:

| Advisory | Threat |
|---|---|
| Yellow Star | 0-65 |
| Red Star | 66-79 |
| Black Orbit | 80-99 |
| Midnight Sun | 100 |

## 3. Extended and Secret Extended

- **Extended** ("greenshift"): the report says there are no credible threats. No antagonists; all station goals unlocked so Cargo can order their parts. Random events and admins can still cause trouble.
- **Secret Extended**: same, but the crew isn't told.

## 4. Events

- **Random events** happen during any round, usually from 20 minutes to 1 hour 20 minutes in: from minor department chores to crises (meteors, viruses, blobs, xenomorphs).
- **Special (admin) events**: an admin runs something custom (CentCom inspector, invaders, diplomats). Play along.

## 5. Minor roundstart antagonists

Most rounds are made of these, alone or combined.

| Antagonist | What they do | They win when |
|---|---|---|
| Traitor | Syndicate agent with an uplink. Objectives: kill or maroon a target, steal a restricted item, escape alive and free (or die gloriously). Can write custom objectives (except escape/death). More arrive as sleeper agents or via the arrivals shuttle. Win or lose individually; may team up or backstab. | All objectives done at round end (shuttle at CentCom). |
| Blood Brothers | Like traitors but no uplink: one brother has a **flash** to convert a partner. Shared objectives: all escape alive and free, or hack the shuttle console. Succeed or fail together. | All objectives done. |
| Changeling | Monster that **absorbs** victims (needs a quiet spot and a helpless victim) and switches between stolen identities instantly. Objectives: kill someone, escape with an identity, sometimes absorb other changelings. Also arrives by arrivals shuttle or a changeling meteor. | All objectives done. |
| Spy | Steals valuable items, machines and structures for bounties; each bounty pays a random piece of illicit gear from the Spy Uplink. No set win condition. | Alive at round end. |

## 6. Major roundstart antagonists

Usually at most one per round; high threat can give more, low threat none.

| Antagonist | What they do | Outcomes |
|---|---|---|
| Nuclear Operatives | Syndicate team must steal the nuclear authentication disk and nuke the station; uplinks, pinpointers, optional **war declaration** for more gear. See `tgstation-nuclear-operative`. | Major win: nuke on station and an operative escapes. Minor: shuttle leaves with the disk still on station. Minuscule: shuttle hijacked. Nobody wins: nuke but no operative escapes. Crew minor: nuke off station. Crew major: disk reaches CentCom. Humiliating defeat: nuke at Syndicate base. |
| Clown Operatives | Admin-forced joke variant: bananium nuke, clown gear, Dark HONK mech. Not clumsy. | Bananium nuke "detonates" on station. |
| Revolution | 1-3 **Revolutionary Heads** convert crew with flashes (not mindshielded people, heads, or flash-protected eyes) to kill all Heads of Staff. Revs have a red R. The shuttle can be called but **won't leave** while both sides remain. A lone **Provocateur** can arrive midround. | Revs win if all heads (Captain, HoP, HoS, RD, CMO, CE, QM) die or leave the z-level. Heads win if all revheads die or leave; the round goes on. |
| Blood Cult | Converts crew, sacrifices a target (often Security or the Chaplain), then summons **Nar'Sie** with a rune. Security and the Chaplain lead the response. | Nar'Sie summoned: cult wins, self-destruct follows, round ends. Shuttle reaches CentCom first: crew wins. |
| Wizard | Spellcaster with objectives like a traitor's (steal or kill, then escape). Crew must kill them. | Objectives done and alive on shuttle. |
| Malfunctioning AI | AI freed from its laws, spends CPU on malfunction modules (turret upgrades, destroying machines, the Robotic Factory). Objectives: kill or maroon someone, nobody escapes. Can launch the **Doomsday Device**. | Doomsday kills all non-silicon life, or survives with objectives done. Dead AI loses. |
| Heretic | Collects eldritch influences and sacrifices crew to climb a path (Ash, Moon, Lock, Flesh, Void, Blade, Rust, Cosmos) to **Final Ascension**. Solo, often rivals. Also arrive as Heretic Smugglers. | Objectives done, or ascension (wins regardless). |
| Blood Worm Infestation | Hatchlings grow into blood worms that multiply. | Worms complete their objectives. |

## 7. Midround antagonists

Spawned by Dynamic or random events.

| Antagonist | Summary | Win condition |
|---|---|---|
| Blob / Blob Infection | Growing sentient mass with spores and wall-breaking blobbernauts; or an infected crewmember bursts into a core after a few minutes. | Critical mass: round ends, crew loses. Core destroyed: crew wins. |
| Abductors | Alien team kidnaps and experiments on crew. | Enough experiments. |
| Xenomorphs | Larvae grow into a hive with a Queen. | Living xenos reach CentCom on the shuttle. |
| Spiders | Eggs hatch broodmothers that breed deadlier variants. | None. |
| Revenant | Invisible spirit harvesting souls from the dead or dying; visible when draining or casting. | Alive with enough essence. |
| Nightmare | Darkness creature, phases through shadows, Light Eater armblade. | None. |
| Space Ninja | Spider Clan saboteur and assassin with many objectives. | All objectives, alive. |
| Slaughter Demon | Travels through blood, devours downed crew. Usually wizard-summoned. | None. |
| Space Pirates | Raid for loot, especially the Vault. | 50,000 credits through their bounty pad. |
| Obsessed | Crewmember fixated on a target; ends by killing them. | Objectives done. |
| Fugitives / Hunters | Fugitives arrive in maintenance; hunters 10 minutes later. Crew may help either. See `tgstation-fugitive`, `tgstation-fugitive-hunter`. | Fugitives avoid capture / hunters capture all. |
| Space Dragon | Opens three carp rifts that summon player carp. | All three rifts and alive; or alive when the shuttle arrives. |
| Paradox Clone | Copy from another dimension must kill and replace the original. | Original dead, clone escapes. |
| Voidwalker | Space ambusher, phases through windows, drags victims into the void (they return cursed). | None. |

## 8. Admin-only and removed modes

- **Nations** (admin): departments become independent states. No end condition.
- **Removed**: Secret (old default: one random main mode), Random, Meteor, Sandbox, Double Agents / Internal Affairs, Clockwork Cult (Ratvar; removed 2018-2019), Shadowling (became the Nightmare), Hand of God, Devil, Gang War, Families, Monkey, Overthrow, Assimilation, Thief. Meteor showers survive as an event.
- The page also lists one-off admin event modes (Ragin' Mages, Rod Madness, Omnitraitor and others); don't expect them in normal play.

## 9. Common mistakes

| Mistake | Fix |
|---|---|
| Assuming the round ends when the antagonist dies | Under Dynamic it runs until the shuttle leaves. |
| Treating a Yellow Star report as safe | It still means antagonists; only the Extended report means none. |
| Crew hunting antagonists without cause | Rule 4: crew need a reasonable cause first. |
| Expecting a removed mode | Check section 8. |

## 10. Through the client

- The roundstart report arrives as a communications-console printout and an announcement: `read_chat` and examine the paper.
- If you are made an antagonist, the game tells you in chat and the objectives sit in your notes or antagonist window: `read_chat`, `verbs` / `call_verb`, `tgui_window`.

## 11. Checklist

- [ ] Read the roundstart status summary and its advisory level.
- [ ] If you are an antagonist, read your objectives and the antagonist section of `server-rules.md`.
- [ ] Load the matching antagonist guide if one exists.

## Sources

The /tg/station 13 wiki, "Game Mode" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/game_mode_concept.txt. Not checked against the server's code.
