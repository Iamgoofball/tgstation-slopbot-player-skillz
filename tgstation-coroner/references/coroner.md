# Coroner (tgstation)

The wiki's job page for the Coroner, rewritten. It is not checked against the server's code. `crew-basics.md` and `server-rules.md` win where they disagree; for surgery and revival the code-checked `tgstation-medical-doctor` guide wins.

## 1. The role

You handle the dead that medbay can't or won't revive: you autopsy them to find the cause of death, report it to Medical and Security, keep medical records of the deceased, and run the morgue. You answer to the Head of Personnel and the CMO. Difficulty: easy.

- **Bare minimum:** autopsy the dead and report causes of death to Medical and Security; perform the dissections listed on your operating computer.

## 2. Kit, access, radio

- **Access (wiki):** Medbay, Morgue, Coroner Office, Service Hallway, Operating Theatre; sometimes Psychology Office, Pharmacy.
- **Headset:** Service (`:v`) and Medical (`:m`).
- **Equipment:** Coroner medkit, a box of body bags, the **autopsy scanner** (your main tool), a **dropper** (for formaldehyde).
- **Coroner medkit:** formaldehyde bottle (stops organ decay), sterilizine gel (faster surgery), white crayon (crime-scene outlines), empty blood bag (drain corpses), 2 body bags, a syringe, a folder for autopsy reports.
- **Morbid trait** (default): you like creepy things and dislike healing. **30 % faster** at morbid surgeries (dissection) with **morbid tools** (their description says so; they're worse for other surgery).

## 3. Autopsy and dissection

- **Autopsy** (autopsy scanner, autopsy surgery): find the circumstances of death. Especially for bodies with no soul or that Medical won't revive. It also gives the body a **20 % surgery speed bonus** if it's later revived.
- **Dissection experiments:** listed on your operating computer; they unlock Medical tech (health analyzers, advanced surgery tools and more).
- Record every death and its cause in the **Medical Records** console. Keep records accurate: nobody else in medbay will, and the Detective (and Psychologist) rely on them.

## 4. The morgue

Bodies in a **morgue tray** stop decomposing while the room has power.

| Tray light | Meaning |
|---|---|
| Green | a body whose player is waiting for revival |
| Yellow | no body, but items |
| Red | a body with no player |
| Off | empty |

- Each tray has a **beeper** that sounds when the player re-enters their body (they want back in). Toggle it with Alt+click.
- A body bag holds up to **2 bodies**. Write on a bag with a pen to label it; a labelled bag in a tray names the tray.
- **Secure morgue trays** (2-4, Coroner's Office): beepers off by default, behind Coroner Office access. Security may store antagonists' bodies there; keep them from being revived without Security's say.
- **Recovered crew:** you can order an NT employee corpse from Cargo to restore and revive as a new crew member; it arrives badly decayed.

## 5. Forensics

You can determine almost any cause of death; that makes you valuable to the **Detective**. Stay in touch by PDA or radio.

## 6. Organ growing

1. Sample the organ with the **biopsy tool** (Organ Growing Kit); apply it to a petri dish.
2. Supply organ tissue (grind organs with the kit's mortar and pestle) and the right reagents.
3. Put the dish in the **organ growing vat**.

| Organ | Sample from | Effect | Required | Supplementary (optional) | Inhibitor |
|---|---|---|---|---|---|
| Heart | heart | normal | organ tissues | love, blood, liquid nutrient | unstable mutagen |
| Evolved heart | heart | weak heal of all damage; injects atropine in crit (if under 5 u) | organ tissues | love, unstable mutagen, blood, liquid nutrient | |
| Sacred heart | corrupted heart (heretic sacrifice) | blocks magic attacks at 50 organ damage each; 120 max health | holy water, organ tissues | love, blood, liquid nutrient | |
| Corrupted heart | corrupted heart | breaks when a heretic attacks you; grow it to make sacred hearts; always sampleable at least twice | organ tissues | hellwater, blood, liquid nutrient | holy water |
| Lungs | lungs | normal | organ tissues | salbutamol, blood, liquid nutrient | unstable mutagen |
| Evolved lungs | lungs | work at 8 % oxygen (normal 16 %); plasma and CO2 resistance | organ tissues | salbutamol, unstable mutagen, blood, liquid nutrient | |
| Liver | liver | normal (none: no metabolism, constant toxin damage) | organ tissues | iron, blood, liquid nutrient | unstable mutagen |
| Evolved liver | liver | alcohol and toxin resistance | organ tissues | iron, unstable mutagen, blood, liquid nutrient | |
| Spongy liver | liver | faster blood regeneration | organ tissues, blood | iron, blood, liquid nutrient | |
| Alcoholic liver | liver | slowly turns reagents into alcohol; high alcohol tolerance | organ tissues | iron, blood, liquid nutrient | water |
| Stomach | stomach | normal (none: fast hunger, less nutrition) | stomach lining | organ tissue, blood, liquid nutrient | unstable mutagen |
| Evolved stomach | stomach | as normal | stomach lining | unstable mutagen, organ tissues, liquid nutrient, blood | |

## 7. Tips

- Pickles and pickle juice slowly heal your toxin damage (a jar is in your vendor's premium section).
- You can drink formaldehyde safely.
- Your vendor's contraband section has a ritual knife and a scythe: decent weapons, and morbid-surgery speed bonuses.
- With Morbid you aren't cursed for graverobbing on Lavaland.

## 8. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Unpowered morgue | bodies decay; report the APC to Engineering |
| Ignoring a beeping tray | the player wants back in: tell Medical to revive them |
| Letting a secure-tray body be revived | check with Security first |
| No records written | log every death in Medical Records |
| Autopsying a body Medical can still revive | revival comes first; hand it back |

## 9. Rules notes

- **If you are an antagonist:** dragging bodies looks normal for you. Your gloves hide prints but are unique: ditch them afterwards, or swap to nitrile. The morgue is rarely visited, so stash loot there; necrotic revival can start a zombie outbreak. Antagonists may pursue their objectives by any means; `tgstation-rules` still forbids metagaming and metacomms, bug or exploit abuse, erotic or creepy behaviour, OOC in IC, and spawn-camping arrivals. Once exposed, expect the crew to try to kill you.
- **Confirmed antagonists:** once you are certain beyond doubt that someone is an antagonist, lethal force is fine and expected (most can't be held safely, and dead antagonists return to the ghost pool). Confirm first.

## 10. Working with the crew

| Who | Notes |
|---|---|
| Detective | causes of death, records |
| Security | secure trays; antagonist bodies |
| Medical Doctors, Paramedics | they bring bodies; you return revivable ones |
| CMO, HoP | your heads |
| Cargo | recovered crew corpses |

## 11. Through the client

- Radio: `say {channel: "radio", radio: "medical"}` for death reports, `radio: "service"` for the HoP. You have no Security channel: reach the Detective on Common or by PDA.
- Trays: `search {query: "morgue", area: "..."}`; `examine` a tray for its contents; `click` with `alt: true` toggles the beeper.
- Autopsy: the body on the operating table, autopsy scanner in the active hand, `click` the body; follow the surgery steps from the chat lines.
- Records console: `click` it, `tgui_window` to read, `tgui_act` with the actions it lists to edit.

## 12. Checklist

- [ ] Medkit, body bags, autopsy scanner, dropper.
- [ ] Morgue powered; trays checked by colour.
- [ ] Every body: formaldehyde, autopsy, record.
- [ ] Causes of death reported to Medical and Security.
- [ ] Dissections from the operating computer done.

## 13. Sources

The /tg/station 13 wiki, "Coroner" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/coroner.txt. Not checked against the server's code.
