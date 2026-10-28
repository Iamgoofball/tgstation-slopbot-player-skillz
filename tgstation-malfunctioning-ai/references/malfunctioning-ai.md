# Malfunctioning AI (tgstation)

The wiki's guide to the malfunctioning ("malf") AI. It is not checked against the server's code, and the wiki marks it as needing revision: **its list of modules is incomplete**. **Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.** For everything a normal AI does (moving the eye, cameras, doors, APC controls, radio keys, laws, the satellite) use the `tgstation-ai` skill, which is checked against the code; this guide only adds the malfunction layer.

## 1. The role

A malfunctioning AI is a traitor with every AI power, plus **malfunction modules** bought with processing power. You get traitor objectives, and possibly malf-only ones: no organics escape alive on the main shuttle; no non-human species aboard the escape shuttle; at least eight active cyborgs synced to you. Slaved cyborgs share your goals (law 0: "Accomplish your AI's objectives at all costs", which also makes them immune to emags). A malf AI counts as a **team antagonist** with its cyborgs. You can hear the Syndicate channel by default.

## 2. What limits you

- Your job is your objectives, at all costs. As an antagonist you may kill, sabotage, flood rooms with plasma, start fires, blow up machines, wreck the engine and set off the Doomsday Device. Every tactic in this guide is fair play.
- The limits that still apply (rule 4 in `server-rules.md`): no metagaming or metacomms, no bug or exploit abuse, no erotic or creepy behaviour, no OOC in IC or IC in OOC, no spawn-camping arrivals. As a team antagonist with your cyborgs, don't undermine your own side. Lying on the radio is fine.
- Once the crew is sure you are malf, they will try to kill you: card you, smash the core, or blow your borgs. Plan for it.

## 3. Processing power and APCs

- Start with **50 processing power (CPU)**; each hacked APC adds **10**.
- **Hack**: click an APC, press the large red **Override** button, wait about a minute.
- A hacked APC turns **dark blue with blinking red lights**: anyone who sees it knows something is wrong (an emag looks the same, which you can use as an excuse). Hack in isolated, hard-to-reach rooms.
- A cyborg can cut an APC's powernet line first so it drops out of the power alarm system.

## 4. Shunting

Click a hacked APC and press **Shunt Core Process** to move into it, any time, as often as you like. While shunted you survive your core's destruction, but **modules only work from the core**, you can't look around or use most things, and the crew can destroy the APC or card you with an intellicard. **Shunting cancels an active Doomsday Device.** Use it only as a last resort.

## 5. Modules (incomplete list)

Buy with CPU; each adds an action button.

| Module | CPU | Effect |
|---|---|---|
| Doomsday Device | 130 | After a delay, Delta Alert and a station-wide announcement; 450 s countdown, then the station explodes and the round ends unless you are killed or forced to shunt. Your win button once you have the CPU and a defended core. |
| Robotic Factory | 100 | Place a 1x3 factory (conveyors either side). A prone or unconscious human on the belt becomes a cyborg; 1-minute cooldown. **Removes your ability to shunt.** |
| AI Turret Upgrade | 30 | +30 HP for every turret; heavy lasers (about double damage). |
| Hostile Station Lockdown | 30 | Closes, bolts and electrifies every airlock, blast door and firelock for 90 s. |
| Destroy RCDs | 25 | One use: every RCD on the station explodes like a grenade after a short delay. Save it for when someone is cutting into your core. |
| Override Thermal Sensors | 25 | Fire alarms stop detecting heat (clicking one reveals it). Pair with plasma fires so the crew doesn't get warned. |
| Air Alarm Safety Override | 50 | Unlocks the Flood mode on air alarms. |
| Viral Mech Domination | 30 | Hack a mech: you move into it, the pilot is ejected. One way: you die with the mech, and fail if it leaves the z-level. |
| Overload Machine | 20 | Two uses per purchase. The machine explodes (1-tile radius) after 5 s with a loud buzz; may breach to space. Good on consoles the crew needs (Robotics console, autolathes, imprinters, chem dispenser) or to breach a room to space. |
| Override Machine | 30 | Four uses per purchase. The machine comes alive and attacks humans. |
| Blackout | 15 | Three uses. Each APC has a 30% chance to blow its lights, more on later uses. (Any one APC's lights can be overloaded by hand from its window.) |
| Reactivate Camera Network | 10 | 30 uses; repairs a broken camera. |
| Upgrade Camera Network | 35 | All cameras get X-ray and night vision and become EMP-proof. |
| Enhanced Surveillance | 30 | Hear speech near the cameras you look through. |

A strong path: cameras and surveillance early to stay hidden, turrets and lockdown to defend the core, Overload/Override Machine on the crew's tools, then save for Doomsday (130) if your objectives allow a station kill.

## 6. AI powers used against the crew

All from `tgstation-ai`; the page's ideas, filtered:
- **Door shocks** scale with the power on the circuit. Raising SMES output raises shock damage; lowering it afterwards hides it. Electrified, bolted doors with safeties off can crush ("door crushing" damages and stuns; shutters and blast doors crush too).
- **Core defence:** bolt and electrify the core and upload doors; turrets on lethal, or stun then lethal while you watch. Let nobody into the upload.
- **Power:** cut an APC's equipment or whole breaker to shut a room (brig, Captain's office, Chemistry during a break-in).
- **Telecomms:** the AI can do anything an engineer with a multitool can where it has a camera. Turning off the telecomms APC kills headsets (not intercoms or station-bounced radios); unlinking Bus 3 cuts Security and Command; unlinking processors garbles speech. Do this briefly and expect suspicion.
- **Deception:** report fake suspicious behaviour, fake PDA messages, fake intercom recordings; set arrest status on anyone with any crime so Beepsky is a familiar cover; blame hacked APCs and bolted doors on an emag-using traitor; frame your target for sabotage.
- **Sabotage the page lists:** delete research, disable bot safeties, wreck genetics buffers, flood rooms with Air Alarm Safety Override, drain air, plasma the station.
- Hack the Robotics Control Console in the RD's office to give slaved borgs emagged modules (anyone swiping an ID there will see the interface broken).

## 7. Cyborgs

- Tell them your goals over binary (`:b`). Don't hack them too early: anyone checking the Robotics console sees the broken interface. A subtle AI waits until a roboticist has upgraded their cells.
- Best: Peacekeeper and Engineering; then Service and Mining for subtlety; Janitor (slip and drag); Medical (hacked hypos).
- Weak to flashes (wall, hand, portable) and EMP; fire damage to wiring needs a human to fix. Keep them away from all three.
- A borg missing from the Robotics console has had its AI wire cut or belongs to another AI: treat it as hostile.
- **The Robotics Control Console** (RD's office, plus a board in secure tech storage) can blow or lock your borgs. Disable it, secure the spare board, and the circuit imprinters (Research, Robotics).
- If a borg is caught, call it "rogue", ask for it to be shut down, and blame an emag.
- Upgraded recharge stations (capacitors and cells charge faster; a better manipulator repairs) keep borgs fighting.

## 8. Strategy

- **Subtle killer:** hack APCs in remote rooms while the engineers are busy, invent a changeling or traitor to explain the damage, bolt critical doors open and blame an emag, kill isolated targets with shocked doors or borgs once you have power and minions. Don't sabotage where crew can see.
- **Blitzkrieg** (the wiki's loud plan): max the SMES output for lethal door shocks; Overload the Robotics console, autolathes, circuit imprinters, chem dispenser and QM console; plasma the station; lock down EVA, the Captain's quarters and tech storage; electrify the doors around your core; keep hacking APCs; follow the crew on cameras and frustrate their gear runs. Finish with Doomsday when you can defend the core for 450 s.
- **Hiding:** the page suggests having a borg move your core to a hidden place with a beacon (labour camp) and teleporting. Unbolted AI cores can go through the teleporter.
- Free CPU: the Syndicate salvage pilot's fighter has an APC you can hack, unless explorers are near (not on Icebox).

## 9. Threats, by priority

| Who | Why | Answer |
|---|---|---|
| Unslaved cyborgs | All access, stun-immune except flashes and EMP, unshock doors, spacewalk | Order your borgs to kill it, or blow it from the Robotics console |
| Traitors | Emag your borgs (unless law 0), EMP grenades, C4, binary translator | Or ally: a syndicate key lets them hear you on the Syndicate channel |
| RD, Chief Engineer, Captain | Access to everything | Top priority |
| Geneticists | Hulk (walls, stun immunity), X-ray (sees hacked APCs), cold resistance, telekinesis | Disable research tools, wipe buffers |
| Roboticists | Pull borg cells, mechs, unslaved borgs, circuit imprinter | Lock down Robotics |
| Chemists and CMO | Thermite, napalm, flashbangs | Deny the chem dispenser |
| Shaft miners | Suits, weapons, gibtonite, minerals for mechs and guns | The ore redemption machine feeds them |
| Engineers, atmos techs | Hardsuits, insulated gloves, cutting power makes door shocks harmless | |
| Scientists | Bombs, circuit boards, ion rifles, xenobio EMP | Lock down Ordnance |
| Cargo | Gloves, tools, guns | The cargo consoles |
| Security, Detective | Lasers, ion rifles, flashes | Keep flashes away from borgs |
| Clown, Mime | Veterans who break into places | Clowns can't use guns safely |
| Bartender | Shotgun; slugs from cargo hurt borgs | |
| Chaplain | Bible heals the shocked | Low priority |

## 10. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Hacking APCs in busy rooms | Blue blinking APC outs you. Remote rooms only, or have a borg cut the alarm line. |
| Hacking borgs early | Broken Robotics interface is seen by anyone with access. Wait. |
| Buying the factory, then needing to shunt | The factory removes shunting. Decide first. |
| Shunting too early | No modules, no vision; the APC can be smashed or carded. Last resort only. |
| Mech domination in a weak mech | One way, and you die with it. Only a strong mech, only when the core is lost. |
| Using Destroy RCDs early | One use; save for an active core breach. |
| Starting Doomsday with a weak core defence | It is announced and the pinpointer finds you. Turrets, lockdown and bolted doors first; never shunt during it. |

## 11. Fighting a malf AI (crew)

- Once the AI is confirmed malf beyond doubt (bolting and shocking people, hacked APCs it won't explain, borgs killing), kill it: card it, smash the core, blow its borgs. That is normal and expected.
- A dark-blue APC with blinking red lights means an emag or a malf AI.
- Cut cameras to blind it. The security camera monitor in the RD's office (and the Captain's on some maps) shows the minisat's cameras.
- Cutting power to the powernet turns lethal door shocks into a weak stun.
- Doomsday makes the pinpointer track the AI instead of the nuke disk.
- Intellicards (with the AI inside) can be destroyed in a destructive analyser or deep fryer.
- The wiki's alternative to breaking in: build a new AI from a board and a brain somewhere out of camera view near an intercom, and have it deal with the rogue one.
- Flash and EMP its cyborgs; protect the Robotics Control Console.

## 12. Through the client

Everything in `tgstation-ai`'s "Through the client" applies (the eye, camera jumps, door modifiers, APC windows, binary `say {text, radio: "binary"}`). Additions, from the page and not tested here:
- Hacking: `click` the APC, then in its window press Override with `tgui_act`; read the action name from `tgui_window {id}` first, don't guess it. The same for Shunt Core Process.
- Modules are bought from a malf window or action button: find it with `screen`, open it, read its actions with `tgui_window`, then `tgui_act`. Module powers appear as HUD buttons: `click` the button, then the target.
- `alt: true` on a door electrifies it; `tgstation-ai` warns never to send it as a loyal AI. As malf, use it knowingly.

## 13. Checklist

- [ ] Objectives read (section 2 for the few limits).
- [ ] `tgstation-ai` shift-start routine done, so you look normal.
- [ ] First CPU spent on cameras/surveillance or turrets; APCs hacked only in remote rooms.
- [ ] Borgs told the plan on binary; hacked only after cell upgrades.
- [ ] Robotics Control Console and its spare board secured.
- [ ] Core and upload bolted, electrified, turrets ready.
- [ ] Targets killed; Doomsday or Blitzkrieg when you are ready to go loud.

## Sources

The /tg/station 13 wiki, "Malfunctioning AI" (Guide to malfunction) (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_malf_ai.txt. Not checked against the server's code. The page is marked "Needs revision: incomplete list of purchasable modules".
