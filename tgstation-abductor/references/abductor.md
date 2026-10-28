# Abductor (tgstation)

Taken from the /tg/station wiki's Abductor page, not checked against the server's code. `crew-basics.md` and `server-rules.md` win where they disagree.

## 1. The role, and the rules

Two aliens on a UFO, an **agent** and a **scientist**, kidnap station crew, replace their heart with an experimental gland, and send them back. Each finished experiment gives a point; your objective is a set number.

- **Abductors are not full antagonists.** Don't murderbone, don't set the release point on the supermatter, don't affect the station in big ways unrelated to experiments, and don't brainwash others into killing for you. Adminhelp first if unsure.
- Rules priority: abductor teams are a team antagonist, under Blob/Brainwash/Cult/Revs/Blood Brother. Never work against your partner.
- Best play: warp in, take one person, experiment, put them back quickly as if nothing happened.
- You can't use ordinary guns. You can't talk normally: anything you say is telepathy to your teammate. Talk constantly.

## 2. The ship

| Thing | Use |
|---|---|
| Human Observation Console | Scientist's base. View the station through cameras. Scan disguises, mark the agent, Send To (telepad → station), Send Self, Retrieve, set the Experiment Release Point, switch the vest's disguise or mode. |
| Abductor Console | Set the teleport destination, Retrieve Mark, Select Agent Vest Disguise, toggle vest stealth/combat, unlock the vest, link the vest, buy gear with points. |
| Alien Telepad | Stand on it to be sent down. Retrieved people arrive here. |
| Replacement Organ Storage | Glands. Limited stock of each; use a different one per subject. |
| Alien Operating Table | Surgery. Drag a cuffed subject onto it to buckle them. |
| Experimentation Machine | Put in a glanded subject, press an option: it gives a point and sends them to the release point. |

## 3. Agent kit

| Item | Use |
|---|---|
| Agent vest | Grafted on. **Stealth:** wear a scanned disguise (any damage breaks it). **Combat:** big armour boost, and "Activate" removes all stuns (long cooldown); no disguise. Modes are set from the ship's consoles. |
| Advanced baton | Use in hand to cycle: **stun → sleep → cuff → probe** (probe says if a subject is suitable). Left-click applies the mode harmlessly; right-click only does damage. Humans can't use it. |
| Abductor silencer | Turns off radios and headsets around the target. |
| Alien pistol | 10 shots of radiation (clone damage); recharge at station rechargers. Last resort: you need subjects alive. |
| Agent belt and tools | Very fast tools; the welder never runs out or blinds, the multitool shows every wire. |

## 4. Scientist kit

| Item | Use |
|---|---|
| Science tool | Use in hand to switch **SCAN / MARK**. SCAN (through cameras) saves a person's look as a disguise; rescanning updates it; scanning a cuffed person shows the cuffs. MARK: the agent instantly, even through the console; anyone else only adjacent, with a slow progress bar. |
| Teleporter implant | Blue crystal HUD icon: back to the ship. Cooldown. |
| Surgery | The scientist knows every surgery, including Alien Tend Wounds (fast brute and burn healing for the agent or subjects). Only the scientist can examine a gland's true name. |

**The scientist is the only way home.** If they die on the station, the mission fails. Teleport out at the first sign of danger.

## 5. The abduction loop

1. Plan together. Do a test run to a quiet spot to practise marking and teleporting out. Consider grabbing medkits from medbay storage first.
2. Scientist: take the science tool out of the backpack, MARK the agent.
3. Scientist at the observation console: SCAN suitable disguises through cameras; pick a target and tell the agent where they're going and who to watch out for.
4. Select the disguise (either console); confirm the vest is in stealth mode (Abductor Console). Agent clicks the vest's **Activate** HUD icon.
5. Agent stands on the telepad; scientist clicks **Send To**. MARK the agent now if you forgot.
6. Agent: baton on stun. **Stun, sleep, cuff**, switching modes between hits. Probe to check the subject isn't catatonic (catatonic subjects don't count).
7. Agent drags the subject somewhere secluded that **has a camera**.
8. Scientist: **Send Self** to the subject, MARK them (slow; instant on a cow), teleport back with the implant, **Retrieve** the subject, then MARK and Retrieve the agent.
9. Agent in danger at any point: scientist Retrieves them at once.
10. Surgery (section 6), set the Experiment Release Point, put the subject in the experimentation machine, press an option.
11. Repeat until you have enough points. Buying replacement gear spends points that count toward the objective.

## 6. Experimental organ surgery

Works through clothing.

1. Aggressive grab, put the subject on the operating table (buckle if cuffed).
2. Drapes, choose **Experimental Organ Manipulation**.
3. Combat mode **off**. Target the **chest**.
4. Scalpel (incision) → retractor → hemostat → scalpel again.
5. Use your hand to pull out organs until you have the heart (removed organs are trash). Heartless species can't be experimented on.
6. Insert the chosen gland.

## 7. Glands

The icon is randomised every time; only the scientist's examine shows the true name.

| Gland (true name) | Effect | Control uses | Control time |
|---|---|---|---|
| Healing (organic replicator) | Rejects and regrows damaged or robotic organs/limbs; purges toxic blood; rejects implants including mindshields | 3 | 300 s |
| Spider (araneae cloister accelerator) | Spawns spiderlings | 2 | 240 s |
| Slime (gastric animation galvanizer) | Vomits slimes, which won't attack them | 1 | 240 s |
| Trauma (white matter randomiser) | Random brain traumas, up to 5 | 3 | 180 s |
| Species (anthropmorphic transmorphosizer) | Changes appearance and species | 7 | 30 s |
| Egg (roe/enzymatic synthesizer) | Lays eggs of random reagents | 2 | 180 s |
| Stretch (pliant cartilage enabler) | Ventcrawls freely | 4 | 180 s |
| Mindshock (neural crosstalk uninhibitor) | Psychic pulses: stun, hallucination or brain damage nearby; control hits everyone near | 1 | 600 s |
| Viral (contamination incubator) | Carries a random advanced disease, unaffected | 1 | 180 s |
| Electric (electron accumulator/discharger) | Shock immune, random bolts | 2 | 90 s |
| Chemical (intrinsic pharma-provider) | Random chemicals in blood, fast toxin healing | 3 | 120 s |
| Plasma (effluvium sanguine-synonym emitter) | Random plasma clouds | 1 | 80 s |
| Blood (pseudonuclear hemo-destabilizer) | Blood becomes a random reagent | 3 | 150 s |
| Quantum (quantic de-observation matrix) | Links to someone in view, later swaps places; control copies to them | 2 | 120 s |
| Access (anagraphic electro-scrambler) | Intrinsic all-access | 3 | 90 s |

Choose glands to fit: avoid healing or stretch glands on Security or other threats.

## 8. Shop (points)

| Item | Cost | Use |
|---|---|---|
| Mind Interface Device | 2 | **Transmit:** anonymous psychic message to anyone. **Control:** give a glanded subject a directive that becomes their main objective for the gland's time, limited uses per gland. Don't direct them to murder (section 1). |
| Reagent Synthetizer | 2 | Beacon that spawns an alien chem dispenser: everything an emagged dispenser makes, minus carpotoxin, plus plasma and uranium. |
| Shrink Ray | 2 | 5 shots, recharges ~1 per 12 s. Shrinks anything but floors for 9 s; small things don't block sight and can be walked over (walls too); small people drop their gear, move slowly, take double damage. |

## 9. Crew, and being caught

An alien in an abductor vest is a confirmed antagonist; the crew will try to kill you on sight. That's why the scientist retrieves the agent at the first sign of trouble. Crew: once certain, lethal force is fine.

## 10. Abductee

If you were abducted, you have new objectives and an odd body. Play the crazed alien-obsessed lunatic for the round's fun; it's a roleplay prompt, not a licence to break rules.

## 11. Common mistakes

| Mistake | Fix |
|---|---|
| Agent not marked before going down | MARK the agent first, so you can pull them out. |
| Vest in combat mode when disguising | Check stealth mode on the Abductor Console. |
| Subject dragged where there's no camera | The scientist can't Send Self there; pick a camera-covered spot. |
| Scanning a cuffed person | The disguise shows cuffs; scan before cuffing. |
| Catatonic subject | Probe first; it won't count. |
| Scientist lingering on station | Implant out as soon as the mark lands. |
| Killing subjects with the pistol | Baton only; they must live. |
| Same gland every time | Stock is limited; vary. |
| Blaming each other | Talk, plan, don't argue. |
| Teleporting into the AI chamber | Not possible. |

## 12. Through the client

- Consoles and machines open windows: `tgui_window` to read the actions, `tgui_act` to use them (Send To, Retrieve, disguise selection, vest mode, release point, buying). Check action names in the window, don't guess.
- HUD icons on the observation console and your vest/implant are in `screen`; press them with `click`.
- Cycle the baton or science tool: `key Z` with it in hand. Then `click` the target (left) for the mode's effect.
- Telepathy: `say` normally.
- Agent: `walk_to` and `fight` for the take-down; `status` for health; ask for Retrieve early.
- Surgery: grab with `click {ctrl: true}`, `drag` the subject onto the table, then `click` with each tool in hand, chest targeted (see `tgstation-medical-doctor`).

## 13. Checklist

- [ ] Plan agreed; test run done.
- [ ] Agent marked; disguises scanned; vest in stealth; disguise on.
- [ ] Target chosen near a camera-covered quiet spot.
- [ ] Stun, sleep, cuff, probe.
- [ ] Scientist marks, implants home, retrieves subject and agent.
- [ ] Heart out, gland in; release point set somewhere harmless; machine run.
- [ ] Points counted against the objective; nothing murderous or station-wrecking.

## Sources

The /tg/station 13 wiki, "Abductor" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_abductor.txt. Not checked against the server's code.
