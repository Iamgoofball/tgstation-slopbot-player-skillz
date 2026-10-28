# Roboticist (tgstation)

The wiki's job page for the Roboticist, rewritten. It is not checked against the server's code. `crew-basics.md` and `server-rules.md` win where they disagree.

## 1. The role

You build and maintain the station's cyborgs, bots and exosuits (mechs), in Robotics and the Mech Bay. You answer to the Research Director. Difficulty: easy.

- **Bare minimum:** build and maintain cyborgs.

## 2. Access, radio, lab

- **Access (wiki):** Robotics, Tech Storage, Morgue, Research Division, mineral storage. On some rounds also the research labs, Ordnance, Xenobiology, Genetics.
- **Headset:** Science (`:n`).
- **Robotics contains:** exosuit fabricators, cyborg recharging stations, exosuit recharging stations, a chest with metal sheets, power cells and wire, tables with a multitool, toolboxes, flashes, a crowbar, a proximity sensor, more power cells and a cell charger.
- **Tech Storage** has two flashes, two power cells and insulated gloves. Secure tech storage holds the robotics/exosuit control boards (ask the CE, RD or AI).

## 3. Building a cyborg

1. Load the exosuit fabricators with metal; print the cyborg parts.
2. Head: two **flashes**. Torso: **cables** and a **power cell**. Attach all parts to the endoskeleton.
3. Volunteers wait at your door or service window; let them in.
4. Remove the brain by **surgery**; put it in an **MMI**. Put the body in the **Morgue** (not disposals).
5. **Examine the MMI first** to check the brain isn't braindead (a live one can speak). Then insert the MMI into the shell.

Keep at least **one finished cyborg body ready** for the bodies that will arrive.

Maintenance: cyborgs come with minimal power cells; swap in better ones when they visit.

## 4. Bots

- **Medibots** (from any first-aid kit; keep its colour): can stabilise several people in crit; infinite basic chems. Unlock with your ID/PDA and lower the **heal threshold to 5** so they top up anyone at 95 % health or less; lock it again. Sync them with research for better efficiency. Turn one off or set it stationary to stop it chasing patients while you move it. Several medibots use the same chemical, so doses don't stack but linger; useful to pre-heal before a fight. **Slimepeople take toxin damage from green (toxin) medibots**: set those stationary or off near slimepeople.
- **Cleanbots:** need a bucket (Hydroponics, or the Cargo autolathe).
- Rename a bot by writing on the assembly with a pen anywhere between the robotic arm and the sensor module.
- Small assemblies fit in a backpack; carry one missing its last part and finish it on site.
- **Drone shells** let ghosts rejoin the round.

## 5. Exosuits

- You need **circuit boards** from R&D research and enough materials before starting. A pile of limbs with no boards or silver is useless. Plan first.
- Sync the fabricators with research for extra parts and cyborg upgrades.
- Fit a **tracking beacon** and **DNA lock** to every mech. Build a **Cyborg and Exosuit Control Console**.
- Ripley boards eat Cargo's money; don't drain it if you want the QM to buy you metal.

| Mech | Notes |
|---|---|
| **Ripley** | cheap utility mech, a forklift; good armour for a non-combat suit (MK1's open cabin lets pilots be shot from front and sides). **Drill** cuts walls, items, blast doors (diamond drill: reinforced walls). **Hydraulic clamp** moves crates. Weak punch. |
| **Odysseus** | medical mech; scans any chemical; its generator makes unlimited chemicals; the syringe gun's syringes can be recovered; up to 5 chemicals per 15 u syringe. Click a box of syringes to load them all. |
| **Gygax** | knockdown punch |
| **Durand** | combat; needs a lot of silver |
| **Phazon** | toggleable elemental punches |

General: a sealed, air-filled cabin is spaceworthy; a destroyed mech ejects you unharmed; drills open lockers.

## 6. When the AI is rogue

- **Cut LawSync** and reset cyborg laws.
- Against a **malfunctioning** AI don't blow all cyborgs: dismantle the Robotics Control console and rebuild it somewhere **off camera**, then lock and reset the cyborgs so they fight for you.
- Don't blow every cyborg because one was emagged.

## 7. Do and don't

**Do:** build cyborg shells and fill them; borg dead antagonists when Security hands them over (killing a confirmed antagonist is also fine); make useful bots; make drone shells; beacon and DNA-lock mechs; get R&D to unlock mech tech.

**Don't:** insert a braindead MMI; build a mech you lack materials for; give a mech to anyone who asks (or who refuses a beacon); go on mech rampages; wear no eye protection while welding (you go blind).

## 8. Rules notes

- Borging someone needs their consent or proper authority (e.g. an executed or dead prisoner with Security's say). Borging a living crew member against their will is a rule 1 matter.
- **If you are an antagonist:** you spawn with flashes and are expected to build dangerous machines; Tech Storage gives you insulated gloves early. Emag bots (a medibot loaded with the traitor toxins kit makes a deadly helper) and cyborgs (Syndicate laws, new tools, immune to control consoles; cyborgs slaved to a malf AI can't be emagged). Debrain your victims for cyborgs; few question a body already on the table. Inside a mech people see only its name: rename it and walk about unrecognised (not in the open-cabin Ripley MK1). Medibots take any chemical. Get augmented so you can self-install implants; a reviver implant gets you back up after a mutual takedown; an emagged toolset arm adds a combat knife. Changelings: regenerating ejects cybernetics. Antagonists may pursue their objectives by any means; `tgstation-rules` still forbids metagaming and metacomms, bug or exploit abuse, erotic or creepy behaviour, OOC in IC, and spawn-camping arrivals. Once exposed, expect the crew to try to kill you.
- **Confirmed antagonists:** once you are certain beyond doubt that someone is an antagonist, lethal force is fine and expected (most can't be held safely, and dead antagonists return to the ghost pool). Confirm first.
- Changelings: regenerating ejects cybernetic parts.

## 9. Working with the crew

| Who | Notes |
|---|---|
| Research Director | your head; approves combat mechs |
| Scientists | mech boards, upgrades via research |
| Shaft Miners, QM | metal, glass, silver |
| Medical | brains and bodies for borging; medibots |
| AI | cyborg status, law changes |

## 10. Through the client

- Radio: `say {channel: "radio", radio: "science"}`.
- Exosuit fabricator: `click` it, read the window with `tgui_window` (`find` a part by name), build with `tgui_act` using the actions the window lists.
- Assembly: hold the part in the active hand and `click` the endoskeleton or assembly; `examine` it to see what's missing; `examine` an MMI before inserting it.
- Bots and cyborgs: `click` with your ID in hand to unlock; their settings window via `tgui_window`.

## 11. Checklist

- [ ] Fabricators loaded with metal; cyborg parts printed.
- [ ] One finished shell on standby.
- [ ] MMIs checked before insertion.
- [ ] Medibots set to threshold 5 and locked.
- [ ] Every mech beaconed and DNA-locked.
- [ ] Welding with eye protection.

## 12. Sources

The /tg/station 13 wiki, "Roboticist" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/roboticist.txt. Not checked against the server's code.
