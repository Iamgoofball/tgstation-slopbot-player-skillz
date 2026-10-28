# Chief Medical Officer (tgstation)

The wiki's job page for the Chief Medical Officer, rewritten. It is not checked against the server's code. `crew-basics.md` and `server-rules.md` win where they disagree; for treatment itself the code-checked `tgstation-medical-doctor` guide wins.

## 1. The role

You head Medical: doctors, paramedics, chemists, the coroner and virology. You answer to the Captain. Medbay is one of the busiest places on the station: keep it organised, protect and help your staff, remove loiterers, and make sure the dead are revived or borged. Difficulty: hard.

- **Bare minimum:** remind the crew about **suit sensors**; make sure **cryo** is set up.

## 2. Kit, access, radio

- **Access (wiki):** all Medical departments, Bridge, CMO's office, Brig. Full chemistry access.
- **Headset:** Medical (`:m`) and Command (`:c`), with the heads' High Volume mode.
- **Gear (wiki):**
  - **Hypospray**: instant injector, 5 u per injection, holds 30 u, starts with 30 u **omnizine** (heals brute, burn, oxygen and toxin). Empty it by injecting into a container or drawing with a syringe.
  - **Compact defibrillator**: works like the medbay defib but clips to your belt and fits a backpack; 10 kW cell = 10 charges. Recharge it, or ask R&D for a 30 kW cell. Don't leave it in your locker.
  - **Telescopic baton**: your self-defence and bouncer tool.
  - **Defibrillator wall mount** (locker): install it by the stasis beds; click it to take the paddles out without wearing the defib.
  - **Advanced health analyzer** (locker): exact organ damage; detects legion tumours, heretic and abductor organs. More from the medical techfab after Advanced Biotech.
  - **CMO MODsuit**: has a large autoinjector you can load with 30 u of any chemical (e.g. multiver and epinephrine).
  - **Biohazard suit** in your office.
- **Runtime**, your cat, lives in your office. She kills mice well; carry her into maintenance during a mouse infestation.

## 3. Shift start

1. Announce on Common for everyone to turn their **suit sensors** on (all three: vitals, health, tracking).
2. Check in with your staff on Medical.
3. Make sure cryo is set up.
4. Optionally make medicines in chemistry for later, or cover chemistry if understaffed.

## 4. Crew monitoring

- Consoles on the Bridge and in your office; **handheld crew monitors** come from the med-vendors for anyone with a medical ID (the Virology vendor is rarely raided; take spares from it). Give one to the Detective if asked.
- Sensor levels: binary (alive/dead), vitals (health), tracking (location).
- Check it periodically and send a doctor to anyone hurt. Keep a handheld monitor in a pocket: the window stays open while it's equipped.
- Dead but no location? Ask the AI to find the body on cameras.

## 5. Disease outbreak

1. Put on the **biohazard suit** from your office.
2. A doctor makes vaccines; chemists split them into pills.
3. Vaccinate medical staff first, **quarantine the infected**, treat, keep medbay sterile and free of blood.

**Virology oversight:** you are the one who unlocks the **Virus Crate**. Have a doctor prove themselves on a simple vaccine (flu) first. Tell them to clear any beneficial virus with you before release, and check their work. If they release one without asking: take a blood sample from someone infected and scan it in the PANDEMIC machine. Good symptoms only: praise, then tell them to ask next time. Bad symptoms (or superpowers: ask the Captain on Command): tell the other heads and hand out the cure widely; let Security deal with the doctor unless you can subdue them safely.

## 6. Medbay security

- Use the baton to keep trespassers away from chemists and staff; show loiterers out.
- **Revolution:** medbay is a bad place in a mutiny and heads are targets. If people act strangely, arm yourself and be ready to leave. Baton first; the hypospray with **20 u chloral hydrate** knocks someone out for a long time (fill it only for this, see below); fire axe, a space lube spray, or a syringe gun as alternatives.
- Traitors see you as an easy target for Bridge access. Stay alert.

## 7. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Forgetting you loaded chloral into the hypospray and injecting a patient in crit | It can kill them. Track what is loaded; refill with epinephrine or salbutamol for patients. |
| Injecting the wrong person with the hypospray | People will assume you are a changeling. Use it on the dying only. |
| Losing the compact defib | Keep it on your belt; recharge it. |
| Letting a virologist release untested viruses | Require sign-off; scan blood in the PANDEMIC. |
| Hiding silent | Announce yourself early, or people forget you're a head. |

## 8. Tips

- The starting 30 u of omnizine makes **strange reagent** (revives corpses).
- Spend your money on advanced first aid kits for the doctors.
- Scan the Cook's food with your PDA reagent scanner if poisoning is suspected.

## 9. Rules notes and antagonist play

- As crew, use the chloral hypospray on anyone not confirmed as an antagonist only in self-defence, under the escalation rules. **Confirmed antagonists:** once you are certain beyond doubt that someone is an antagonist, lethal force is fine and expected (most can't be held safely, and dead antagonists return to the ghost pool). Confirm first.
- **If you are an antagonist:** you need no emag or uplink weapon. Fill the hypospray with chloral hydrate (or worse), strike fast and stealthily, then get back to work in medbay, where nobody suspects you; a coat disguises you. As a changeling, capture people on the pretence of healing them, and ask the HoP for maintenance access. Convince the HoP you need more access and you can reach almost anywhere. Antagonists may pursue their objectives by any means; `tgstation-rules` still forbids metagaming and metacomms, bug or exploit abuse, erotic or creepy behaviour, OOC in IC, and spawn-camping arrivals. Once exposed, expect the crew to try to kill you.

## 10. Working with the crew

| Who | Notes |
|---|---|
| Doctors, paramedics | send them to patients from the monitor |
| Chemists | medicines, vaccine pills |
| Coroner | autopsies, morgue |
| Virologist | outbreak response; Virus Crate approval |
| Detective | crew monitor, death causes |
| AI | finding bodies on camera |
| Captain, heads | outbreak and casualty reports on Command |

## 11. Through the client

- Radio: `say {channel: "radio", radio: "medical"}`, `radio: "command"`, plain `channel: "radio"` for the sensors announcement.
- Crew monitor: `click` it (in hand or the console), read it with `tgui_window`.
- Hypospray, defib, baton: check with `inventory`, hold in the active hand, `click` the target. `examine` the hypospray to see what it holds.
- Find people and bodies: `search`, then `walk_to`.

## 12. Checklist

- [ ] Suit sensors announcement; staff check-in on Medical.
- [ ] Cryo set up; defib mount by the stasis beds.
- [ ] Compact defib on belt; hypospray contents known.
- [ ] Crew monitor checked regularly.
- [ ] Virology supervised; outbreak plan (biosuit, vaccine, quarantine).

## 13. Sources

The /tg/station 13 wiki, "Chief Medical Officer" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/chief_medical_officer.txt. Not checked against the server's code.
