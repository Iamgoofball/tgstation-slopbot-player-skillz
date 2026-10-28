# Paramedic (tgstation)

The wiki's job page for the Paramedic, rewritten. It is not checked against the server's code. `crew-basics.md` and `server-rules.md` win where they disagree, and for treatment, defibrillation and corpse care the code-checked `tgstation-medical-doctor` guide wins (its field-medic and revival sections agree with this page's defib criteria and formaldehyde advice).

## 1. The role

You are the rescue medic. You spend most of the shift outside medbay finding the injured and dead, giving first aid, and bringing them to medbay for the doctors. You answer to the CMO. Difficulty: easy.

- **Bare minimum:** find injured crew and bring them to Medbay.
- **Basic:** enforce suit sensors, first aid, **formaldehyde into corpses** to stop organ decay, **don't drag bleeding people through the halls**.
- **Advanced:** treat every damage type on the spot, defibrillate, heal more with less, rescue people from far away (space, Lavaland).

## 2. Kit, access, radio

- **Access (wiki):** Medbay, Morgue, **Maintenance**, **external airlocks**; sometimes Surgery. Less medbay access than a doctor.
- **Headset:** Medical (`:m`).
- **You spawn with:** a **medical belt** (handheld crew monitor and some minor medicine), a collapsed **roller bed**, and the **Lifeline** PDA app (tracks people).
- **Get next:** a **crew pinpointer** (NanoMed Plus vendor, or research), a **health scanner HUD** (glasses, Medical Storage table), a **health analyzer** (techfab or your PDA).
- On MetaStation, Paramedic Dispatch holds the emergency team locker and a medical MODsuit (see `tgstation-medical-doctor`).

## 3. The patrol loop

1. Keep the **handheld crew monitor** open (put it in a pocket or suit slot so the window stays on).
2. When someone shows damage, find them with the pinpointer.
3. Minor: tell them to walk to medbay. Serious: treat on the spot or bring them in.
4. **Move bleeding patients on a roller bed**, never by dragging (dragging worsens bleeding and slows you).
5. Leave them with the doctors; go back out.
6. Corpses: inject **formaldehyde** to stop decay; bring them in for revival.

If you're unsure whether someone needs help, PDA them and ask.

## 4. Field kit

Ask a doctor for their starting medkit once you know the basics; Robotics often has spare medkits.

| Item | Use |
|---|---|
| **Sutures** | cheap brute healing; faster with practice |
| **Regenerative mesh** | cheap burn healing; faster with practice |
| Drapes, scalpel, hemostat, cautery | basic surgery for wounds like severe burns (leave real surgery to doctors) |
| **Hercuri spray** | cools and slowly heals burns; freezes the patient (give them something warm after). **Not on lizards** (cold-blooded) |
| Patches, syringes, gels, sprays | faster healing; **Libital**, **Aiuri**, **Syriniver** are cheap and useful (side effects) |
| **Medipens** | scarce, strong: salicylic acid, oxandrolone, pentetic acid (in their medkits). Save for emergencies |
| Libital/Aiuri gel (NanoMed) | diluted with granibitaluri; heals best under 50 physical damage |

Equipment: **compact defibrillator** (research or the CMO), crew pinpointers, **medical MODsuit** (low pressure and cold), handheld crew monitors, health analyzer (right-click for chemicals; diseases and traumas too), health scanner HUD (health bars; icons for viruses and alien larvae; night-vision upgrade researchable), **nitrile gloves** (no fingerprints, faster syringe injections), roller beds (later: bluespace body bags).

Spare first-aid kits in Medical Storage are contested: take them sparingly and tell the CMO. Biosuits there for outbreaks.

## 5. Defibrillation

Bulky defib: take off your backpack, wear the defib, click it, free your other hand, wield the paddles in both hands, target the **chest**, click the patient. Strip thick suits (space suit, firesuit) first; **activated MODsuits and EVA suits block it**. **Stop dragging the patient** or you get shocked too.

Revival requires all of:
1. Under **180 brute** and under **180 burn** (each counted separately; 179/179 is fine).
2. Not a **suicide**.
3. Not **catatonic**.
4. The patient is **in their body** (they get a message when you start).
5. A working **heart** (plasmamen have none; a decayed heart must be replaced).

A revived patient is still deep in crit: treat them immediately. Scan with a health analyzer for the cause; harmful chemicals remain in a dead body (they don't metabolise).

## 6. Retrieval

You have maintenance and external airlock access for a reason: fetch bodies from wrecked Engineering, space, or Lavaland (a dead miner). Wear a space suit or the medical MODsuit for vacuum.

## 7. Tips

- Bar drinks top off damage: cream (brute), lime juice (toxin), orange juice (oxygen), tomato juice (burn), Bloody Mary (blood). Normal plus iced tea: mild toxin heal.
- Raw carrots and blindfolds heal eyes; earmuffs heal ears.
- **Miner's salve:** twinkie + plasma sheet + iron sheet in a grinder; apply to skin.
- Ask chemistry for patches of salicylic acid, oxandrolone, salbutamol, multiver.
- Borrow a patient's epipen before using your own.
- Carry tools to crowbar doors open.
- Surgery outside medbay: use a table; failing that, the roller bed.
- Winter boots and a pocket protector let you carry three extra medipens.

## 8. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Dragging a bleeder | roller bed |
| Defibbing while pulling the body | stop pulling first |
| Defib on a suited patient | strip the suit or deactivate the MODsuit |
| Corpse left to rot | formaldehyde at once |
| Hercuri on a lizard | don't |
| Using up medipens on minor injuries | sutures and mesh first |
| Going into space unsuited | space suit or MODsuit |

## 9. Rules notes

- **If you are an antagonist:** you look normal anywhere and nobody questions a body on your roller bed; use maintenance. A stethoscope cracks safes. Swap cryo's cryoxadone for acid. A 15 u lexorin syringe-gun shot kills without treatment (thick suits block it). Poison someone, finish them in maintenance, then morgue them or behead them and space the body. Antagonists may pursue their objectives by any means; `tgstation-rules` still forbids metagaming and metacomms, bug or exploit abuse, erotic or creepy behaviour, OOC in IC, and spawn-camping arrivals. Once exposed, expect the crew to try to kill you.
- **Confirmed antagonists:** once you are certain beyond doubt that someone is an antagonist, lethal force is fine and expected (most can't be held safely, and dead antagonists return to the ghost pool). Confirm first.

## 10. Working with the crew

| Who | Notes |
|---|---|
| CMO | your head; compact defib, spare kits |
| Medical Doctors | hand patients over; medkits |
| Chemist | patches and pills |
| Coroner | bodies that can't be revived |
| Quartermaster / miners | Lavaland retrievals |
| AI | locating bodies on camera |

## 11. Through the client

- Radio: `say {channel: "radio", radio: "medical"}`; Common for "turn your suit sensors on".
- Crew monitor: `click` it in hand; read it with `tgui_window` for names, health and locations; then `walk_to` the area.
- Treat: hold the item in the active hand and `click` the patient; `examine` them or use the analyzer for damage.
- Roller bed: deploy it, buckle the patient onto it, then pull the bed (`click {object_id, ctrl: true}`).
- Check `inventory` for the defib, pens and kit before leaving medbay.

## 12. Checklist

- [ ] Belt, roller bed, crew monitor in a pocket, pinpointer, HUD, analyzer.
- [ ] Sutures, mesh, a few chems.
- [ ] Patrol; respond to the monitor.
- [ ] Bleeders on the roller bed; corpses get formaldehyde.
- [ ] Defib criteria checked before shocking.

## 13. Sources

The /tg/station 13 wiki, "Paramedic" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/paramedic.txt. Not checked against the server's code. The page's fifth defib criterion is cut off mid-sentence in the source.
