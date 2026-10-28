# Pirate (tgstation)

The wiki's guide to space pirates. It is not checked against the server's code. Where it disagrees with `crew-basics.md` or `server-rules.md` (the `tgstation-rules` skill), **those win** on the few limits in section 7.

## 1. The role in one paragraph

Pirates come from a rare random event. The station gets a ransom demand (80% of cargo's points at that moment, per the page; the crews' own messages name other sums). If command pays at a communications console (usually on the Bridge), nothing happens. If they refuse or ignore it, a pirate ship spawns in space with your crew (sleepers let late ghosts join if too few took it). Fly next to the station, board, and loot. **Target: at least 50,000 credits**, scaling with how rich the crew is. Your superior is the Pirate Captain (slightly better gear); your access is "Pirate".

## 2. What to loot, in order

1. The **vault**: siphon the station's credits; take the mined materials.
2. **People**: kill them and take the money on their IDs.
3. Anything valuable not bolted down: haul it back to the ship.

## 3. The crews

| Crew | Type | Strengths and notes |
|---|---|---|
| Human Rogues | normal | Captain + 2. Modest ship with a small armoury: energy scimitars, laser guns, some explosives. First move: C4 into the station armoury for more guns. |
| Silverscale Elite Royalty | normal | Lizards: pressure-proof, no breathing, tougher, but **not cold-proof** (they freeze in space over time). Can harden into a silver statue (must be speared, not batoned); use it to ambush. E-swords and rifles. |
| The Grey Tide | normal | Little armour, weapons or ship, but **double** the crew. Plays like fugitives with license to kill. |
| Lustrous Geode Dwellers | normal | Ethereals in a bluespace asteroid. Same space resistances as Silverscales, weak to brute, innate Bluespace Prophecy trauma. No turrets; mining kit: bluespace crystals, PKA pressure kits (**two stack** for very high damage), jump boots, a bluespace launchpad. Play hit-and-run. |
| Skeletons (Flying Dutchman) | dangerous | Immune to temperature, pressure, radiation, disease and embedding; no eating, breathing or blood. Can't process chemicals: **heal with milk** (ship fridge, kitchen, the garden's cow, or cargo); not soy milk. Ship cannons (below). |
| Ex-Pharmacists | dangerous | Fungal tuberculosis grenade (vaccines included: use them), biohazard chem sprayer (knockdown + toxins), traitor poison kit, Interdyne medical modsuits. Ship has chemistry, virology and a cryotube. Rivals a small nuke team; experiment. |
| Space IRS | dangerous | Best on the station, weak in space. Autorifles, pistols, breaching shotguns, telescopic batons, a grenade launcher with flashbangs and smoke. Tactical vests; ship has ballistic turrets (don't lean on them). |

### Dutchman cannons
Load a cannonball, add **15u gunpowder**, light it with anything that lights a cigarette (lighter to plasma cutter).

| Ball | Effect |
|---|---|
| Standard | Unarmoured chest/head hit: full health to crit; limb hits delimb; shrapnel. Mostly for breaching. |
| Explosive | Big blast: fire it at Security and loot the armoury. |
| Malfunction | Large EMP: stops mechs and borgs, kills APCs and lights, drains energy weapons. |
| The Biggest One | Rare; a toxins maxcap. Use it when you're done looting an area (not on the armoury you want). |

## 4. The data siphon

Optional. Once on, it can't be turned off. It drains credits from cargo and tech from R&D, creates a "hostile environment" that stops the cargo and emergency shuttles moving, and locks R&D and supply consoles. But it broadcasts a GPS signal ("Nautical Signal") and alerts the whole crew, who will come for it and your ship. Turn it on only when ready to defend it.

## 5. Tactics

- Board where your crew's resistances help: skeletons and lizards can enter from space anywhere.
- Go for the armoury early (C4 or cannon), then the vault.
- Strip IDs of the dead; haul loot back often so a lost fight doesn't lose everything.
- Keep someone on the ship if it has turrets or the siphon runs.
- Crew-side: confirmed pirates may be killed outright; paying the ransom avoids all this; welding vents won't help, but locking down the vault and armoury will. Pirates can't loot what they can't reach.

## 6. Common mistakes

| Mistake | Fix |
|---|---|
| Lingering in space as Silverscale/Geode | You freeze; get inside. |
| Skeleton taking medicine | It doesn't work; drink milk. |
| Pharmacists skipping their own vaccines | Vaccinate before the TB grenade. |
| Siphon on with nobody to guard | Everyone homes in on the GPS; defend it or don't start it. |
| Maxcap on the armoury | Nothing left to loot. |

## 7. The few limits that still apply

- You're a team antagonist: don't hurt your crew's raid, by action or by idling. Otherwise blast, breach, kill and loot as needed to hit the target.
- Rule 4 still limits you: no metagaming or metacomms, no bug or exploit abuse, no erotic or creepy behaviour, no OOC in IC (or IC in OOC), no spawn-camping arrivals.
- **Expect to be killed once exposed.** Crew may kill an antagonist as soon as they're sure what it is; most antagonists can't be held safely, and a dead one goes back to the ghost pool. Stay hidden until you're ready to go loud, then fight to win.

## 8. Through the client

- Ship consoles and the siphon open tgui windows: `tgui_window` to read, `tgui_act` with the actions the window lists. Don't guess action names.
- Cannons: ball in hand, `click` the cannon; then the gunpowder container; then a lit lighter.
- Talk to your crew on the radio channel your headset shows (`say` with the prefix from `inventory`/examine), or in person.
- Loot: `click` items to pick up; pull bodies and crates with `click` `ctrl: true`.

## 9. Checklist

- [ ] Read your crew type and gear on the ship.
- [ ] Fly beside the station; plan the boarding point.
- [ ] Armoury, then vault credits and materials.
- [ ] IDs off the dead; haul loot home regularly.
- [ ] Decide on the siphon; reach 50,000+ credits.

## 10. Sources

The /tg/station 13 wiki, "Pirate" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_pirate.txt. Not checked against the server's code.
