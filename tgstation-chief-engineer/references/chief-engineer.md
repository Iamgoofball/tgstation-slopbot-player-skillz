# Chief Engineer (tgstation)

The wiki's job page for the Chief Engineer, rewritten. It is not checked against the server's code. `crew-basics.md` and `server-rules.md` win where they disagree, and for the engine, power grid and repairs themselves the code-checked `tgstation-station-engineer` guide wins (this page only covers what a CE does on top).

## 1. The role

You head Engineering: the Station Engineers and the Atmospheric Technicians. You answer to the Captain. You direct the department, make sure a power source comes online, keep the Supermatter from delaminating, keep telecomms working, and do engineer work yourself when nobody else will. Difficulty: hard.

- **Bare minimum:** at least one power source online at round start; know what to do when telecomms or medbay gets blown up; know how to repair the station and machines such as APCs.
- **Basic skills:** construction, telecomms and atmospherics; communicate with and teach your staff.
- **Advanced:** optimise power and atmos; coordinate repairs after meteors, nuclear operatives or a malfunctioning AI; handle rogue cyborgs and revolutionaries.

## 2. Kit, access, radio

- **Access (wiki):** all Engineering and Atmospherics, power equipment, CE Office, construction site, Bridge, maintenance, EVA, Tech Storage, Telecommunications, external airlocks, Brig, mineral storage.
- **Headset:** Engineering (`:e`) and Command (`:c`). Like every head's, it has a **High Volume** mode (larger text).
- **Unique gear (wiki):** the CE's white suit/hardsuit or MODsuit that resists **both fire and radiation** and has a built-in jetpack (needs an air tank in suit storage); **advanced magboots** (stop all slipping when active, no slowdown); a copy of the **station blueprints** (create and rename areas, view wire layouts); advanced tools. Engineering has only **two** engineering suits (radiation, no fire) and Atmospherics **one** (fire, no radiation).
- **Poly** the parrot lives in your office. It kills spiders and carp quickly.

## 3. Shift start

1. Greet the team on Engineering. Find out who is there and give everyone a job. Taking charge in the first minutes is what makes the department listen later; staying silent until mid-round means nobody will.
2. Send one person (a volunteer if possible) to set up **solars**; everyone else on the **Supermatter**. If a solars worker needs EVA gear, ask the AI to let them into EVA, or do solars yourself.
3. Help new engineers. If someone is disruptive, warn them, then demote if it continues (through the HoP or your ID powers).
4. When the first power source is online, announce it to the crew.
5. If an engineer runs off in a suit to explore space before doing minimal duties, tell them to come back; it counts as dereliction.

## 4. Power sources

Get the default source working first; a second one is pointless while the crew is angry that the first isn't running.

| Source | Notes |
|---|---|
| **Supermatter** | The usual engine. Emits radiation, makes viewers hallucinate, releases hot oxygen and plasma, heats the air, throws tesla bolts. Starts inert; any object or projectile hitting it activates it. Mishandled, it explodes or turns into a tesla or singularity. Details: `tgstation-station-engineer`. |
| **Solars** | Decent steady output; keeps the station alive while the Supermatter is sorted out. Easy; delegate it. |
| **Turbine** | Present on some maps; burns plasma. Follow the turbine guide. (The page also strikes out the thermo-electric generator.) |
| Singularity / Tesla generators | **Removed** from the game per the page. A singularity or tesla can still form from a delaminating Supermatter. |

## 5. Atmospherics and telecomms

- Atmos is yours too. Know the basics, make sure the atmos techs can run it (teach them or do it), and check periodically that nobody has tampered with it.
- **Do not "sabotage-proof" atmos (e.g. pulling the plasma from the loop) without in-character evidence of a threat. That is metagaming** (rule 2).
- Keep **telecomms** working. The chain is receiver -> mainframe -> processor -> mainframe -> server -> broadcaster; with everything linked you don't need a hub, but Mining and remote stations do need one.

## 6. After setup

- Listen for hull breaches; send engineers to fix them.
- Check the **Station Alert Console** for power and atmos alarms.
- Check atmos periodically.
- Make sure solars are wired.
- Set up a third or fourth power source; tune the Supermatter for more output.
- Get an **RCD** (Engi-Vend, or the Engineering techfab once researched) for fast patching or demolition. The techfab also prints the advanced tools R&D unlocks.

## 7. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Staying silent at shift start | Assign jobs on Engineering in the first minutes. |
| Starting a second engine before the first works | Stick to the default source until it is stable. |
| Sabotage-proofing atmos with no IC reason | Don't; it's metagaming. Act on evidence. |
| Barricading Engineering during a revolution (emitters, RCD) | Don't. It drags the round out and is bad form. Defend yourself normally and work with Security. |
| Letting an engineer leave with a suit | Recall them; suits are scarce. |
| You are a head: revolutionaries target you | Stay alert, keep your gear on, stay near help. |

## 8. Rules notes and antagonist play

- The page's tips mention **reading and forging PDA messages** at the telecomms message monitor, and scanning the monitor key into your PDA. Reading crew messages or impersonating people as crew is not a job duty; don't do it without an IC reason (rules win).
- **If you are an antagonist:** your access reaches almost everything important. Options from the page: wreck telecomms, subvert the AI with the AI board in Tech Storage, sabotage atmospherics and the engine, deconstruct anything fast, and hide in space or inside the Supermatter chamber in your suit. A high-capacity oxygen tank filled to 1013 kPa lasts a very long time; advanced magboots resist all slips except space lube. Antagonists may pursue their objectives by any means; `tgstation-rules` still forbids metagaming and metacomms, bug or exploit abuse, erotic or creepy behaviour, OOC in IC, and spawn-camping arrivals. Once exposed, expect the crew to try to kill you.
- **Confirmed antagonists:** once you are certain beyond doubt that someone is an antagonist, lethal force is fine and expected (most can't be held safely, and dead antagonists return to the ghost pool). Confirm first.

## 9. Working with the crew

| Who | Notes |
|---|---|
| Station Engineers, Atmos techs | your staff; assign, teach, check on |
| AI | opens EVA, reports alarms and breaches |
| Captain, heads | power status reports on Command |
| Research Director | techfab unlocks, upgraded parts |
| Quartermaster | engine and solar crates, insulated gloves |

## 10. Through the client

- Radio: `say {channel: "radio", radio: "engineering"}` for your staff, `radio: "command"` for heads, plain `channel: "radio"` for Common.
- Consoles (Station Alert, power monitoring): `click` the console, then read it with `tgui_window`; act with `tgui_act` using the actions the window lists.
- Find things: `search {query: "...", area: "..."}`, then `walk_to`. `examine` a machine (APC, SMES, Supermatter) for its state.
- Use items by holding them in the active hand and `click`ing the target; check `inventory` first.

## 11. Checklist

- [ ] Greet Engineering, assign solars and the Supermatter.
- [ ] Power source online; announce it.
- [ ] Atmos staffed and running; telecomms working.
- [ ] Station Alert Console checked; breaches assigned.
- [ ] Backup power source.
- [ ] No barricading; stay alert as a head.

## 12. Sources

The /tg/station 13 wiki, "Chief Engineer" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/chief_engineer.txt. Not checked against the server's code. The page marks the singularity and tesla generators, and the thermo-electric generator, as removed.
