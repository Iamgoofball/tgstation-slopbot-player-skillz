# Blob (tgstation)

Taken from the /tg/station wiki's Blob page, not checked against the server's code. `crew-basics.md` and `server-rules.md` win where they disagree.

## 1. The role, and the rules

A blob is a round event: a growing mass that destroys walls, fixtures and creatures in its path. You are the **overmind**, an invisible camera-like mind that builds the blob. You win by covering **400 tiles of the station** ("critical mass"). After that the blob gets a huge spread rate and infinite resources for about a minute, and the station is lost. The crew wins by destroying the **core**.

- A blob is a team antagonist and sits at the top of the rules' priority order ("Blob / Zombie" first). Blobbernauts, spores and zombies under ghost control serve the overmind.
- Eating the station is the objective: destroy whatever helps you win. As a team antagonist you still keep the limits in `server-rules.md` section 4 (no metagaming or metacomms, exploits, erotic/creepy behaviour, OOC in IC, spawn-camping arrivals), and must not hurt the team's work.
- **Crew side:** the wiki warns that crew using plasma fires or bombs against a blob may be banned; crew are not antagonists, so take that seriously.

## 2. Before you burst

- Open the status panel. You can burst from **1 minute**; at **6 minutes** you are forced to burst where you stand. Until then you move freely and unseen.
- At **75 tiles**, or **10 minutes** after bursting, Central Command announces a Level 5 Biohazard. Aim not to be found before then.
- Best spot: a spacious abandoned maintenance room: no cameras, dark, narrow approaches that funnel the crew into chokepoints, hard to shoot at from space.
- Stand in the middle of the room, away from walls: the core and nodes eat nearby walls on their own before growing onto them.
- If you can't hide: places that cripple the crew when lost (Telecomms, Science, AI Sat) or that hold hazards (Ordnance, Atmospherics canisters).

## 3. Pieces and costs

Place a normal blob by clicking a tile cardinally next to an existing blob. Place a building by hovering over a blob tile and clicking its HUD icon. Same-type buildings need spacing (count cardinal steps).

| Piece | Cost | Requirement | What it does |
|---|---|---|---|
| Core | — | — | Pulses nearby resource and factory blobs. Its health is on your HUD; if it drops, go and defend it. Lose it and you lose. |
| Normal blob | 4 | Cardinally adjacent to a blob | Click a tile with a dense object, or diagonal, to attack it instead. Spreading into space often fails. Left-click. |
| Strong blob | 15 | On a normal blob | Tough, fireproof, blocks gas. Ctrl-click. |
| Reflective blob | 15 | On a strong blob | Reflects projectiles by ricochet chance; bounces emitters and lasers. Ctrl-click again. |
| Resource blob | 40 | 4+ tiles from another resource blob | Gives resources when pulsed by core or node. Each extra one slows generation slightly. |
| Node blob | 50 | 5+ tiles from another node | A mini-core: expands, heals, pulses resource and factory blobs. |
| Factory blob | 60 | 7+ tiles from another factory | Makes spores when pulsed, up to 3. |
| Blobbernaut | 40 | An undamaged factory | Heavily damages the factory to make a player-controlled blobbernaut. It dies slowly if its factory is destroyed. |

Spores: fragile, AI-controlled, explode into a smoke cloud of your chemical, and turn humanoid corpses into **blob zombies** (tougher, use the corpse's armour; ghosts can take them over).

| Ability | Cost | Use |
|---|---|---|
| Jump to Core | — | Teleport to the core; before bursting, places the core where you are. |
| Jump to Node | — | Teleport to a node of your choice. |
| Remove Blob | refunds ~40% | Alt-click a non-core blob. Not all can be removed. |
| Rally Spores | — | Middle-click: send spores (and zombies) to a spot. |
| Readapt Strain | 40 (first free, another free every few minutes) | Choose a new chemical from a random handful (the page says 4 in one place, 5 in another). |
| Relocate Core | 80 | Swap the core with the node under your selector. Not allowed in some areas. |

## 4. Chemicals (strains)

Your chemical sets your colour and the effect of every attack (applied as vapor). Blobbernauts deal 80% of these numbers.

| Strain | Attack | Upside | Downside |
|---|---|---|---|
| Blazing Oil | 5 brute, 20 burn, ignites | Bursts of flame when burned; fireproof | Weak to water (extinguishers) |
| Cryogenic Poison | 10 brute, 7.5u frost oil + 7.5u ice + 7.5u poison | — | — |
| Debris Devourer | ~5 brute | Absorbs items it spreads over, throws them; spores burst with 3 items; resistance up to 10 from items | — |
| Electromagnetic Web | 5 brute, 25 burn, 20% EMP | EMPs when killed by melee/bullets/lasers | +25% burn, full brute; mechs shoot from range |
| Energized Jelly | 5 brute, 15 oxy, 30 stamina, stops breathing | Tesla immune | Burn damage from EMPs |
| Explosive Lattice | 20 brute + 10 to nearby | Spores/zombies explode; explosion immune | +50% from fire and tesla |
| Networked Fibers | 20 brute, 15 burn | Core regenerates 2.5x; nodes/core make resources instead of tiles | Expands only by hand, only next to core/nodes; expanding there moves the core. Alt-click to remove a tile if stuck. |
| Pressurized Slime | 15 brute, 10 oxy, 25 stamina | Releases water when hit; 50% brute resist | — |
| Reactive Spines | 5 brute + 25 armour-ignoring brute | Hits the area when meleed | — |
| Regenerative Materia | 5 brute, 17.5 toxin, victims look healthy | Core regenerates 10x, +1 resource | — |
| Replicating Foam | 22.5 brute | Expands when burned, bonus spread | Double brute damage |
| Shifting Fragments | 22.5 brute | Swaps places with a nearby blob when damaged | — |
| Synchronous Mesh | 17.5–70 brute by nearby blobs | Spreads damage between blobs | +25% fire/explosion/tesla; killed tiles take neighbours with them |
| Distributed Neurons | 5 brute, 15 toxin | Zombifies unconscious (not just dead) humans for 5 resources; ghosts control spores, which harvest sleeping/crit targets for 5–10 resources | — |

The wiki calls all safe except Blazing Oil and Electromagnetic Web. Change strain to shake up what the crew is using against you.

## 5. Strategy (overmind)

1. Build resource blobs first. When the core can't support more, place a node and build resource blobs around it.
2. Let the core and nodes eat walls and expand on their own; spend on manual growth only when it pays. Destroy machines and structures by hand (the auto-growth won't).
3. Don't spread into space unless you must: you need station tiles to build and to win.
4. Once found (or about to be), build factories, then blobbernauts. Keep a few blobbernauts at all times: they pressure attackers away from your tiles and act as eyes.
5. Win by placing nodes and out-growing the damage the crew does. Break their tools: rechargers, emitters, exofabs.
6. Manual tiles are best used to cut off a fleeing crew member or to reach a machine you want gone. Don't fight a resource war of repairs: the crew usually wins those.
7. Upgrade to strong, then reflective, where lasers and emitters hit you.
8. If one side is collapsing, relocate the core to a node. Losing a node is survivable; losing the core is not.

## 6. Blobbernaut

- You obey the overmind. Talking normally goes to the blob hivemind; you don't understand common speech.
- About 400 health, but you start at 50%: heal first. You heal fast near a node or the core, run faster on blob, and take slow damage off blob. Your factory dying kills you slowly, and you can't claim a new one.
- Hit and run: strike, retreat to heal. Mechs (Durand) kill you in a few punches; stay away.
- Body-block shots aimed at the core and structures. You don't need kills: keeping the crew off the nodes is enough for critical mass.

## 7. Fighting the blob (crew)

- **The emergency shuttle won't leave while a core lives.** Kill it. Blobbernauts and zombies are confirmed antagonists: kill them on sight.
- Brute is weak and the blob can't be stunned. Use **burn**. This does not mean fire.
- Armour and bio protection block blob attacks (riot armour, bio suits). Don't get surrounded.
- **Welders:** from YouTool (hacking it gives two upgraded welders) or the autolathe. Burn a path to a resource blob. Keep fuel tanks nearby, welder off when refueling, and keep tanks away from the blob. Swap to plasma cutters from Science when they appear (same damage, no fuel, don't ignite plasma).
- **Lasers:** limited. Take at most two, only with good armour or a space suit, bring an unwrenched recharger. Armory, some heads' offices, R&D, Cargo. Disablers are useless.
- **Emitters:** as far away as you can while still hitting the core. Three side by side beat a core. Power them with a PACMAN and aim with reflectors.
- **IEDs:** small blast, opens a gap without ruining atmos.
- **Never** flamethrowers, plasma fires or bombs: they kill the crew and help the blob. Two strains are weak to fire, three benefit. Adminhelp before anything big.
- **Zombies:** don't run (they chase and auto-hit, and helpers can't land hits). Stand and hit with a lit welder; an armoured zombie needs armour, a fire axe or friends. Pull downed crew away before they become zombies.
- **Critical mass:** about a minute until the nuke. Get off the station's level: pod or shuttle to Lavaland, or space.
- **BoH bomb:** not recommended. If the core is caught in the tear it teleports randomly; otherwise it makes an area the blob can't cross.

| Department | Do this |
|---|---|
| Medical Doctor | Field medic with HUD and kit; triage, brute and burn patches/sutures/meshes. Don't let armed crew die and get engulfed. Check bags of anyone you drag back. Forward surgery table: 2 rods + 1 silver bar. |
| Chemist | Mass-produce medicine for the blob's damage type; leave it on the counter or bring it forward. |
| CMO | Coordinate, don't field-medic. Hand out the kit, maybe the hypospray; healing viruses. |
| Cargo | Order emitters, laser gun crates (not energy guns), metal and glass. Express beacon near the front. Sell rare ores for weapons. |
| Miners | Use Lavaland loot and PKAs; attack from space without getting surrounded. |
| R&D | Rush advanced beam weapons (beam snipers). |
| Ordnance | No bombs. |
| Roboticist | Medibots from emptied medkits, floorbots; Durand/Gygax, or Ripley/Clarke with a PKA in space. No cleanbots. |
| Xenobiology | Regen jelly (purple), golems or sentient creatures, IEDs. |
| Genetics | Pressure adaptation for spaced blob areas, TK to hit safely, Hulk for hard-to-reach blob. |
| Engineer | Emitters from Secure Storage (or the SM chamber if none), PACMAN-powered, aimed with reflectors. Healing emitters exist. |
| Atmos Tech | Help engineers with emitters. No plasma floods. |
| Security | Lasers from the armory, rechargers near the front. |

The wiki's old advice to mass-print industrial welders from hacked autolathes is struck through: true, but likely to get you killed.

## 8. Common mistakes

| Mistake | Fix |
|---|---|
| Bursting next to walls | Centre of the room. |
| Bursting in a lit, camera-covered area | Abandoned maintenance room; hit 75 tiles before you're seen. |
| Spending resources repairing tiles | Build nodes, resources, factories; repair only when needed. |
| No blobbernauts when the crew arrives | Factories as soon as you're found; keep several naughts. |
| Core under fire with nowhere to go | Keep a node somewhere safe; Relocate Core (80). |
| Blobbernaut wandering off blob | You lose health off blob; return to a node or the core. |
| Crew using fire or bombs | Don't; burn damage from welders, lasers, emitters. |
| Running from a zombie | Stand and fight with a lit welder. |

## 9. Through the client

- The countdown and resource count are in `statpanel`; HUD buttons (buildings, abilities) are in `screen`.
- Place a normal blob: `click` the tile (by its object or the tile's turf) next to your blob. Strong/reflective: `click` with `ctrl: true`. Remove: `click` with `alt: true`. A building: `click` the HUD icon while hovering the target tile; if hover isn't available, check what `screen` says the button does. Middle-click (Rally Spores) may not be offered by `click`; use the Rally Spores HUD button if it isn't.
- Abilities that are verbs (Jump to Core and the like) show in `verbs`; run them with `call_verb`. Strain choice opens a window: read it with `tgui_window`, choose with `tgui_act`.
- Blobbernaut: `say` talks to the hivemind. `status` for health; `walk_to` back to a node; `fight` to hit and run.
- Crew: `walk_to` the YouTool or Engineering, `key Z` to light a welder, `click` the blob tile with it in hand. `say` with `radio` to call out core location.

## 10. Checklist

**Overmind**
- [ ] Status panel read; burst window (1–6 min) noted.
- [ ] Secluded maintenance room, centre tile; core placed.
- [ ] Resource blobs, then a node, then more resource blobs.
- [ ] Factories and blobbernauts before discovery.
- [ ] Strong/reflective blobs facing lasers and emitters; a safe node for relocation.

**Crew**
- [ ] Armour or bio suit, welder or laser, recharger brought along.
- [ ] Emitters ordered/placed far from the core.
- [ ] No fire, no bombs.

## Sources

The /tg/station 13 wiki, "Blob" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_blob.txt. Not checked against the server's code.
