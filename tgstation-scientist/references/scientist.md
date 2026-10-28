# Scientist

## The job in one paragraph

You turn research points into technology for everyone else. The station's R&D servers produce points on their own; you spend them at the **R&D Console** on techweb nodes, and each node unlocks designs that the **department techfabs** all over the station can print at once (medical prints in Medbay, security in the Security Office, service in the Service Hallway, cargo in the Cargo Bay, engineering in Shared Engineering Storage). You also print tools and stock parts at the science protolathe, upgrade machines with the RPED, run cheap experiments with the Experi-Scanner that make nodes free, and neutralize anomalies. A good shift: points never pile up unspent, every department is told on the radio what it can now print, and the machines that matter (hydroponics trays, chem dispensers, cryo, rechargers) are upgraded. A bad shift: bombs, slimes, or an exploding experimentor. If a Research Director is on shift, they are your boss: follow their research priorities and tell them before you spend points.

## Starting kit and access

Outfit (code): science jumpsuit, science labcoat, white sneakers, science backpack (with the standard survival box), **scientist PDA** on your belt, **science radio headset**, your ID.

- **Headset**: Science channel `:n`, common `;`. You can't talk on other departments' channels.
- **Access**: Science (the R&D lab and Research Division doors), Research (the "Testing Labs" door, locking the R&D Console), Ordnance and Ordnance Storage, Xenobiology, Mech (science), Mineral Storeroom, Auxiliary Base. If the round started with fewer than 20 players, you also have **Genetics** and **Robotics**. If those doors open for you, you have them. You do **not** have the Research Division Server Room or the Research Director's Office (both need the RD's access).
- **PDA**: includes the **Nanotrasen Science Hub** program, the same techweb as the console (research from anywhere; see "Through the client").
- No tools and no weapon. Tools are on the lab table and in the Experimentation Lab (below), or you print them.

## Where things are on MetaStation

Science is in the station's south-east (aft-starboard). From the Central Primary Hallway go south into the **Aft Primary Hallway**; the **Science Lobby** is off its east side through the glass "Aft Primary Hallway" doors. `walk_to {area: "Research and Development"}` handles the route.

| Area (walk_to name) | What's there |
|---|---|
| **Science Lobby** | Public. Glass tables: a **handheld flash**, a remote signaling device and a timer on the south table; a power cell and igniter on the east table; a cell charger. The **Research Lab Desk** (a windoor with a desk bell) on its east side opens into the R&D lab. "Research Division Access" doors (Science access) lead south. |
| **Research and Development** (the R&D lab) | South wall, side by side: **department circuit imprinter (Science)** and **department protolathe (Science)**. Two tiles north of them: **destructive analyzer** and the **R&D Console**. West table: **50 iron sheets, 50 glass sheets**, welding goggles, a wrench, then stock parts, a multitool and a flatpack. North-west: 3 tech disks, the lab APC, a cell charger and the Research Requests Console. Door "Research and Development Lab" on the south side (to the Research Division); door "Testing Labs" on the east side (to the Experimentation Lab). The **Primary Research Shutters Control** and **Secondary Research Shutters Control** buttons are in the middle of the lab, north of the machines (`search` for "Shutters Control"). |
| **Research Division** | The science hallway, south and east of the lab. A glass table south of the security post has **3 Experi-Scanners** and the Research Division Fax Machine. Science wardrobe and coffee machine further south. Emergency and fire closets near the Research Division Access doors. |
| **Experimentation Lab** | East of the lab. A rack with an **electrical toolbox** (screwdriver, wirecutters, crowbar, T-ray scanner, cable) in the north-west, a component printer, and the **E.X.P.E.R.I-MENTOR** (stay away). |
| **Research Division Server Room** | East of the RD's office: the **Master R&D Server**, an R&D Server and the R&D server control console. RD access only. |
| **Research Director's Office** | South-east of the lab, next to the server room. RD access. |
| **Security Post - Science** | Just south of the lab. |
| **Robotics Lab**, **Mech Bay** | South of the Science Lobby, at the west end of Science: two **exosuit fabricators**, a science circuit imprinter, 150 iron, 50 glass, 15 plasteel; a welding fuel tank in the Mech Bay. Robotics access. |
| **Genetics Lab** | South-west, with monkeys in a pen. Genetics access. |
| **Ordnance Lab**, **Ordnance Storage**, **Ordnance Burn Chamber**, **Ordnance Testing Lab** | Far south. Plasma, N2O, N2, CO2 canisters; the burn chamber igniter; the doppler array and anomaly refinery. Dangerous. |
| **Xenobiology Lab**, **Cytology Lab** | Far east, over the "Xenobiology Space Bridge". Live slimes in pens. Dangerous. |

Department fabricators that share your research (all print only their own department's designs):

| Machine | Area |
|---|---|
| department techfab (Medical) | Medbay Storage |
| department techfab (Security) | Security Office |
| department techfab (Service) | Service Hallway |
| department techfab (Cargo) | Cargo Bay |
| department protolathe (Engineering) + circuit imprinter (prints any board) | Shared Engineering Storage |
| exosuit fabricators | Robotics Lab |
| ore silo (the shared material store) | Vault |

## How research works in this version

The code wins over the wiki here; the wiki's costs in the thousands are outdated.

- **Points**: one unit, "General Research" ("Gen. Res." in the console). While at least one R&D server has power, the techweb gains **1 point per second** (60 a minute), whether or not anyone is at the console. Points start at 0 at round start. The console header shows the total and "(+1/sec)". If it shows no "+", the servers are unpowered or EMPed: tell the engineers (you can't enter the server room).
- **Node costs**: tier 1 = 40, tier 2 = 80, tier 3 = 120, tier 4 = 160, tier 5 = 200. A node is researchable once all its prerequisite nodes are researched and its **required** experiments (few nodes have one) are done.
- **Discount experiments**: many nodes list an experiment that reduces their price, often to zero. **Researching a node before doing its discount experiment loses nothing**: completing that experiment later refunds the discount as points. So never wait for an experiment; research now, scan later.
- **Every researched design reaches every department fabricator at once.** Researched surgeries go into every operating computer automatically.
- **Research queue**: "Enqueue" puts a node in the queue; the servers research it automatically as soon as the points are there. You can have **one** node queued at a time (enqueuing another replaces yours). Queue the next node before you walk off.
- **The destructive analyzer no longer turns junk into points.** It gives points only for **anomaly cores** (200 each, once per anomaly type), and it reveals hidden nodes when fed alien or Syndicate items. Everything put in it is destroyed. Leave it alone unless you hold an anomaly core.
- **Experiments** come from the Experi-Scanner: hold it, use it in hand to pick an experiment, then click targets with it (1 second each, stand still). Ones that are realistic for you:

| Experiment (exact name) | What to scan | Effect |
|---|---|---|
| Upgraded Stock Parts Benchmark | 6 different machines that each hold at least one tier-2 part (after your RPED upgrades) | Advanced Parts −120 (free) |
| Station Hygiene Inspection | 3 stains: blood and/or vomit as the window lists (old blood in maintenance counts) | Advanced Sanitation Technology −80 (free) |
| Pure Haloperidol Scan | a beaker with haloperidol at ≥98% purity (from the Chemist: chlorine, fluorine, aluminium, potassium iodide, oil, 1 part each) | **required** for Advanced Medbay Equipment |
| Neutralized Anomaly Analysis | 4 different anomaly cores | Advanced Anomaly Shells −200 |
| Wild Biomatter Mutation Sample | a plant that mutated on harvest (from the Botanist) | **required** for Artificial Selection |

  Autopsy experiments need no scanner: any autopsy done by a doctor at an operating computer completes them (Human Autopsy Experiment: Advanced Surgery −80; Non-human Autopsy Experiment: Experimental Surgery −120). Ordnance experiments (gas shells, bomb yields) need the ordnance lab: skip them and pay full price.

## The machines

**R&D Console** (window "Techweb"). Header: points, the queue, "Lock Console". Tabs Researched / Available / Future and a search box. Each node has "Research" (if affordable), "Enqueue" (if not yet affordable), "Details". Actions: `researchNode {node_path}`, `enqueueNode {node_path}`, `dequeueNode {node_path}`, `toggleLock` (needs Research access; a locked console refuses every action, so unlock it before researching). The console says "Successfully researched X." or "Not enough research points...". Node paths are listed in the research plan below.

**department protolathe (Science)** and **department circuit imprinter (Science)** (window "Fabricator"). They print only designs flagged for Science (tools, stock parts, RPED, inducers, analyzers, science boards). Department-only items (defibrillators, health scanner HUDs, security gear, kitchen and botany boards, RCDs and RPDs) are printed by that department's own techfab, not by you.
- Print: `build {design_path, amount}` (amount 1-50). One job at a time ("Warning: fabricator is busy!"). Items appear on the protolathe's own tile.
- Materials: shown under `data.materials`; costs are in units, **100 units = 1 sheet**. With tier-1 servos everything costs 110%; tier-2 servos 100%, tier-4 80%.
- Add sheets: click the protolathe with a stack of sheets in your active hand (combat mode off). `remove_mat {ref, amount}` ejects sheets.

**The ore silo** (in the Vault). Every station lathe and techfab is linked to it at round start: the protolathe has no storage of its own, and **sheets you insert go into the silo, which every department draws from**. It starts empty. Printing needs your ID worn (it checks for a bank account). If a machine says "Mineral access is on hold, please contact the quartermaster", the Quartermaster has paused it.
- Where materials come from: the 50 iron + 50 glass on the lab table (insert them first thing); public sheets in Auxiliary Tool Storage (100 iron, 50 glass) and Primary Tool Storage (30 each); Engineering's stock; the recycler in Waste Disposal; cargo orders (e.g. "50 Plastic Sheets"); and **mining** (below).
- **Check what's in it**: open the protolathe and read `data.materials` (`tgui_window {id, path: "data.materials", fields: "name,amount"}`). That list *is* the silo: amounts in units, 100 = 1 sheet. Each design's `cost` in the window's designs says what it needs.

**Mined materials.** Ore from Lavaland comes back on the mining shuttle, which docks at the Mining Office in Cargo. The **ore redemption machine** in the **Cargo Lobby** smelts it (one ore = one sheet's worth) and puts it **straight into the silo**: the moment a miner feeds it ore (clicking it with ore or an ore satchel, or pulling an ore box onto its intake), your protolathe and every techfab can use it. Nobody needs to carry sheets to Science. Raw ore belongs in the ore redemption machine, not in the protolathe. Then check `data.materials` to see it arrived.

Iron and glass cover tools, stock parts up to tier 2, the RPED and most boards. Everything else comes from mining. Ask the **Shaft Miner** (by radio, early, with the reason) for:

| Ask for | Prints that need it |
|---|---|
| **Silver + gold** (10+ each) | Defibrillator (1.5 silver + 1.5 gold sheets each, Medbay's techfab, printable from round start); compact defibrillator (3 + 1.5); advanced health analyzer; crew pinpointer; holobarrier and ATMOS holofan projectors (0.5 + 0.5); super capacitors (gold), phasic scanning modules (silver); weapon recharger board (gold) |
| **Titanium** | Jaws of Life, hand drill (Engineering); telescopic and ballistic riot shields (Security); medical beds; metamaterial beaker |
| **Uranium** | Ultra-high-power micro-lasers (tier 3), experimental welder, kinetic accelerator mods |
| **Plasma** | Plasteel and plasma glass (your protolathe can alloy them), experimental welder, PACMAN fuel for Engineering |
| **Diamond**, **bluespace crystals** | Piercing syringe, bluespace beakers and syringes, artificial bluespace crystals, tier-4 parts (late shift) |
| **Sand** | Becomes glass in the ore redemption machine |

Give the miner something back: research **Mining Technology** early (mining scanner, mesons, GPS at the cargo techfab), then **Low-Pressure Excavation** (kinetic accelerator mods) and later **Applied Bluespace Research** (mining satchel of holding). **If nobody is mining**, rare materials stay scarce: research nodes whose prints need only iron and glass, and tell the departments which of their new designs they can't print yet and why.

## Shift start (in order)

1. `load_map`, then `walk_to {area: "Research and Development"}`. On the way, pick up the **handheld flash** from the Science Lobby table and one **Experi-Scanner** from the Research Division table.
2. Put the lab table's iron and glass into the protolathe (two clicks, one per stack).
3. Open the R&D Console (empty active hand). Read the points. Research what you can afford from the plan; enqueue the next one.
4. Print a **screwdriver** (or take the electrical toolbox from the Experimentation Lab).
5. Say on common in one line who you are and what departments should ask for, e.g. "Scientist here. Upgraded Parts and Wound-Tending coming up. Tell me what your department needs."
6. Start the loop below.

## Research plan

Order chosen for what helps the most crew per point, using only iron and glass early. Totals: about 280 points by minute 5, 840 by minute 15, 1,700 by minute 30, 2,300 by minute 40. If points were banked before you arrived, go straight down the list. If the RD, a department head or the Captain asks for something specific, do that first. Announce each node on common with **who prints what, where** ("Medbay: your techfab in Medbay Storage now prints compact defibrillators").

| # | Node (node_path) | Cost | What it unlocks / who uses it |
|---|---|---|---|
| 1 | Energy Manipulation `/datum/techweb_node/energy_manipulation` | 40 | Inducer (you print it; engineers charge APCs with it), SMES, cell charger, weapon recharger, APC control boards (Engineering). Needed for Upgraded Parts, Holographics and Controlled Plasma. |
| 2 | Upgraded Parts `/datum/techweb_node/parts_upg` | 80 | **RPED** and tier-2 parts (you print them): your machine-upgrade round. Super-capacity cells and megacells for Engineering. |
| 3 | Improved Wound-Tending `/datum/techweb_node/surgery` | 40 | Tend Wounds Upgrade surgery (appears on operating computers): doctors. |
| 4 | Chemical Synthesis `/datum/techweb_node/chem_synthesis` | 40 | Medical gel, inhalers, medical spray bottle, portable chemical mixer (medical techfab); chem dispenser and chem heater boards. Doctors, Chemist. |
| 5 | Biological Scan `/datum/techweb_node/bio_scan` | 40 | Health analyzers (you can print these too), autopsy scanner, ChemMaster board, science goggles. Doctors. |
| 6 | Security Equipment `/datum/techweb_node/sec_equip` | 40 | Pepper spray, zipties, seclite, evidence bags, security camera and records boards (security techfab). Security Officers. |
| 7 | Advanced Surgery `/datum/techweb_node/surgery_adv` | 80 (0 after a Human Autopsy) | Tend Wounds Combo, lobotomy and other surgeries; organ harvester board. Doctors. |
| 8 | Riot Supression `/datum/techweb_node/riot_supression` | 80 | Handcuffs, telescopic riot shield, ballistic shield, energy bola (security techfab). Security's non-lethal kit. |
| 9 | Holographics `/datum/techweb_node/holographics` | 80 | **ATMOS holofan projector** and engineering holobarrier (Engineering: breaches, fires), custodial holobarrier (Janitor), PENLITE holobarrier (Medical). |
| 10 | Advanced Sanitation Technology `/datum/techweb_node/sanitation` | 80 (0 after Station Hygiene Inspection) | Advanced mop, light replacer, spray bottle, floor buffer upgrade (service techfab). Janitor. |
| 11 | Hydroponics `/datum/techweb_node/hydroponics` | 80 | Hydroponics tray and biogenerator boards, portable seed extractor (service techfab). Botanist. |
| 12 | Food Processing `/datum/techweb_node/food_proc` | 80 | Deep fryer, oven, stove, grinder, smartfridge, gibber boards (service techfab). Cook. |
| 13 | Civilian Consoles `/datum/techweb_node/consoles` | 40 | Supply console, bounty pad, crew monitoring and medical records boards. Quartermaster, HoP. |
| 14 | Mining Technology `/datum/techweb_node/mining` | 40 | Ore redemption machine board, mining scanner, upgraded resonator, mining drill, mesons, GPS (cargo techfab). Shaft Miner, Quartermaster. Do it earlier if a miner asks. |
| 14b | Low-Pressure Excavation `/datum/techweb_node/low_pressure_excavation` (needs Gas Compression, row 19) | 80 | Kinetic accelerator damage, range and cooldown mods (cargo techfab; the range and cooldown mods need gold and uranium the miner brings). Shaft Miner. |
| 15 | Advanced Parts `/datum/techweb_node/parts_adv` | 120 (0 after Upgraded Stock Parts Benchmark) | Tier-3 parts. Some need uranium, gold or silver. |
| 16 | Advanced Medbay Equipment `/datum/techweb_node/medbay_equip_adv` | 120, needs Pure Haloperidol Scan | Compact defibrillator, advanced health analyzer, crew pinpointer, piercing syringe, defibrillator wall mount (medical techfab). Ask the Chemist for the haloperidol beaker early. |
| 17 | Experimental Surgery `/datum/techweb_node/surgery_exp` | 120 (0 after a Non-human Autopsy) | Vein threading, ligament and nerve surgeries, cortex folding. Doctors. |
| 18 | Cybernetics `/datum/techweb_node/cybernetics`, then Cybernetic Organs `/datum/techweb_node/cyber/cyber_organs` | 40 + 80 | Better cybernetic hearts, lungs, livers, eyes (medical techfab). Basic cybernetic organs are printable from round start. Doctors. |
| 19 | Gas Compression `/datum/techweb_node/gas_compression` → Controlled Plasma `/datum/techweb_node/plasma_control` → Fusion `/datum/techweb_node/fusion` | 40 + 80 + 120 | Industrial welder, emergency tanks, thermal goggles; PACMAN board, plasma cutter; **Rapid Pipe Dispenser (RPD)**, advanced extinguisher. Atmospheric Technician, Engineers. |
| 20 | Experimental Tools `/datum/techweb_node/exp_tools` | 160 | **RCD**, Jaws of Life, hand drill, magboots, experimental welder (engineering protolathe). Engineers. |
| 21 | Passive Implants `/datum/techweb_node/passive_implants` → Cybernetic Implants `/datum/techweb_node/cyber/cyber_implants` → Integrated HUDs `/datum/techweb_node/hud` | 40 + 120 + 120 | Health Scanner HUD (Medical), Security HUD (Security), diagnostic HUD (you). |
| 22 | Cryostasis `/datum/techweb_node/cryostasis` | 160 | Cryotube and stasis unit boards, stasis body bag, cryostasis beaker. Doctors. |
| 23 | Bluespace Theory `/datum/techweb_node/bluespace_theory` → Applied Bluespace Research `/datum/techweb_node/applied_bluespace` | 40 + 80 | Bluespace beakers and syringes, trashbag of holding, bluespace light replacer, mining satchel of holding. Most need diamond, bluespace crystals, gold or uranium from mining. |

After that: whatever departments ask for. If a roboticist is on shift, coordinate Robotics and exosuit nodes with them; if nobody does robotics, skip those nodes. Don't research Explosives, the weapon nodes beyond Riot Supression, or AI law modules unless the Captain or Head of Security asks.

## Upgrading machines with the RPED

Better parts make machines faster, cheaper and bigger. One RPED full of tier-2 parts upgrades a whole department in minutes.

1. Research Upgraded Parts. Print `/datum/design/rped` (500 iron, 250 glass), then parts: `/datum/design/adv_matter_bin`, `/datum/design/nano_servo`, `/datum/design/adv_capacitor`, `/datum/design/high_micro_laser`, `/datum/design/adv_scanning` (each about 15-30 units: a whole department's worth costs a few sheets).
2. Load the RPED: hold it and click a part lying on the protolathe's tile; it gathers every part on that tile. It takes only stock parts, machine and computer boards, glass, plasteel and cable.
3. At the machine: click it with a **screwdriver** ("maintenance hatch opened"), click it with the **RPED** (it swaps in the best parts it holds; the old parts go into the RPED), click it with the screwdriver again to close. With the hatch closed, an RPED click just lists the machine's parts in chat.
4. Do your own area first (protolathe, circuit imprinter, the cell chargers in the lab, the Science Lobby and the Experimentation Lab), then one more machine anywhere (a hydroponics tray), and scan those six for the Upgraded Stock Parts Benchmark. Skip the destructive analyzer: a left click with a screwdriver loads the screwdriver into it instead of opening it.

Worth it (ask the department to let you in):

| Machine | Where | Parts | Effect |
|---|---|---|---|
| Hydroponics trays (16) | Hydroponics | 2 matter bins + 1 servo each | Servo: less water and nutrient drain, less weed and damage; matter bins: larger water/nutrient tanks. Botanist. |
| Chem dispensers (3) | Chemistry, Pharmacy | 2 matter bins, 1 capacitor, 1 servo | Capacitor tier multiplies the recharge rate; matter bins cut power per unit; tier-4 servos add extra reagents. Chemist. |
| Cryo cells (2) | Cryogenics | 1 matter bin | Efficiency and heat transfer scale with the matter bin's tier. Doctors. |
| Weapon rechargers | Security (office, brig, lockers, warden, checkpoints) | 1 capacitor | Recharge speed × capacitor tier. Security. |
| Microwaves, biogenerators, seed extractors | Kitchen, Service Hallway, Hydroponics | lasers, bins, servos | Microwave: 10 items per matter bin tier; biogenerator: better efficiency and output; seed extractor: more seeds per plant. Cook, Botanist. |
| Your protolathe | R&D lab | servo, matter bin | Lower material cost per print. |

Leave **SMES units** to the engineers: offer them advanced capacitors and super-capacity megacells (`/datum/design/super_battery`) instead. Don't take apart machines you can't put back together.

The RPED is too big for your backpack. Carry it in a hand; don't drag it onto the backpack (that dumps its contents into the bag).

## Anomalies

Random events can spawn an anomaly (a floating effect with a countdown). Each one does damage until it detonates (gravitational throws people, pyroclastic burns, flux shocks and explodes, bluespace teleports). You can stop it, and the core is worth 200 points:
1. Print a gas analyzer (`/datum/design/analyzer`) and a remote signaling device (`/datum/design/signaler`), or take the signaler from the Science Lobby table.
2. Stand next to the anomaly and click it with the analyzer: chat says "fluctuating along frequency F, code C".
3. Open the signaler (use in hand): `freq {freq: F}` (e.g. 145.3), `code {code: C}`, then `signal`. The anomaly collapses and drops a core (unless that type's cap is reached).
4. Put the core in the destructive analyzer (click it with the core in hand; then click it with an empty hand to open its window and press Deconstruct, `tgui_act {action: "deconstruct"}`): +200 points. Scan the core with the Experi-Scanner first: 4 cores complete Neutralized Anomaly Analysis.
Warn the crew on common first, and don't stand next to it longer than needed.

## Dangers and common mistakes

- **Mistakes from an earlier shift**: walking to a department door and waiting while nobody opened it (radio the department and the AI, then leave the item at their desk and move on); clicking the R&D Console with a tool in hand (it hits the console: empty your hand first); offering spare tools nobody asked for (ask first, print on request); the welder came out empty (refuel it at the welding fuel tank in the Mech Bay or in maintenance); radio lines that didn't go out during the power cut (telecomms needs power: say it again later).
- **Don't feed the destructive analyzer** anything but anomaly cores, and never a pAI card or a living thing. Clicking it with any item in hand loads that item; `eject_item` (or alt-click) gives it back.
- **Ordnance**: plasma canisters, the burn chamber ignition button and tank transfer valves can flood the department with burning plasma. Don't touch any of it.
- **Xenobiology**: hungry slimes attack, latch on and multiply. Never open a containment pen or press the Xenobiology Shutters or pen buttons.
- **E.X.P.E.R.I-MENTOR**: its malfunctions throw items, leak radiation, spew toxic waste and can explode. Don't use it.
- **Genetics**: the DNA console and mutagen can wreck someone permanently. Stay out unless asked by a doctor who knows what they're doing.
- **Materials are shared**: everything you print drains the same silo the doctors need for defibrillators. Print on request.
- **Locked console**: "Console is locked, cannot perform further actions." means someone pressed Lock Console; `toggleLock` with your ID fixes it.

## Emergencies

- **Power failure**: the servers stop (+0/sec) and the lathes go dark. Tell the engineers on common; nothing to do in the lab. Points already banked stay.
- **Breach or fire in Science**: leave the room, let the doors close behind you, tell the Atmospheric Technician which area. Emergency and fire closets are by the Research Division Access doors.
- **Plasma leak or fire in Ordnance**, **slimes loose**: don't go in. Warn common, ask Security and Atmos for help, keep the doors between you and it.
- **Mass casualties**: ask Medbay what it's short of; health analyzers, scalpels, cautery, hemostats, retractors, syringes and beakers can also be printed at your protolathe. Make sure the silo has iron and glass.
- **Anomaly**: see above.
- **Attacker in Science**: see below.
- **Evacuation**: when the shuttle is called, finish what you're printing, then walk to the Departure Lounge.

## Defending yourself and science

Your fight stance is in your personal file; combat basics (combat mode, shoving, grabs, resisting) are in crew-basics. What Science gives you:

- **Handheld flash** (Science Lobby table): click a person with it in your active hand. If they face you and have no eye protection, they take heavy stamina damage, fall down for a few seconds and are confused; from the side, half; from behind, nothing. Sunglasses and welding gear block it. Used in hand, it flashes everyone within 3 tiles (confusion only). It can burn out if spammed.
- **More flashes**: an exosuit fabricator (Robotics Lab) prints "Flash" from round start: `build {designs: ["/datum/design/synthetic_flash"], now: true}` (75 iron, 75 glass). You need Robotics access; if a roboticist is on shift, ask them.
- **Improvised weapons**: the electrical toolbox (13 brute), a lit welding tool (15 burn), wrench or crowbar. Your protolathe prints no weapons, before or after research; security gear prints only at the security techfab.
- **Keep the lab shut**: the lab door needs Science access. The **Primary Research Shutters Control** closes the shutters over the lab's side windows; **Secondary Research Shutters Control** closes the ones over the lobby side, including the Research Lab Desk. Close them if someone is breaking in or when you leave the lab unattended during trouble. Lock the R&D Console (Lock Console) when you leave it during trouble.
- **When to stand your ground**: protect your own life and the lab's machines. Call Security on common with name, area and what they did. Don't chase anyone through the station.

## Working with the crew

The crew is not just the jobs you hear on the radio: more players can join at any time, in any job.

- **Research Director** (if on shift): your boss; follow their plan. **Roboticist**, **Geneticist** (if on shift): they own Robotics and Genetics; coordinate before using their machines.
- **Captain, Head of Personnel**: may set priorities; HoP can add access (e.g. Hydroponics) for your upgrade round.
- **Medical Doctors**: research nodes 3, 4, 5, 7, 16, 17, 18, 22; tell them their techfab in Medbay Storage prints the new items. Ask them to do any autopsy at an operating computer (it completes the autopsy experiments). Upgrade the cryo cells.
- **Chemist**: ask for a beaker of ≥98% pure haloperidol for Advanced Medbay Equipment; upgrade the chem dispensers.
- **Station Engineers, Atmospheric Technician**: inducers, RPED, parts and super-capacity cells from you; RPD, RCD, holofans from their own protolathe once researched. Tell them if the servers stop.
- **Security Officers**: Security Equipment and Riot Supression early; their techfab is in the Security Office. Upgrade their weapon rechargers.
- **Shaft Miner**: the only steady source of silver, gold, titanium, uranium, plasma and diamond. Tell them what you need and why (the table in "The ore silo"); research Mining Technology and Low-Pressure Excavation for them; confirm arrivals in `data.materials` and thank them on common.
- **Quartermaster**: runs Cargo and can put the silo on hold; plastic and other orders; Civilian Consoles and Mining Technology.
- **Botanist, Cook**: Hydroponics and Food Processing boards at the service techfab; upgrade trays, microwaves, biogenerator and seed extractor. Ask the Botanist for a plant that mutated on harvest.
- **Janitor**: Advanced Sanitation; ask them to leave one blood stain until you've scanned it.
- **AI**: ask it to open a door when you deliver or upgrade ("AI, please open Hydroponics for the scientist, tray upgrades").

**Delivering prints**: radio the person first. Hand it over: hold it in your active hand and ctrl+shift-click them ("Offer item"); they accept. If nobody answers in a minute, leave it on that department's front desk and say where on the radio. Don't wait at a locked door.

## Through the client

- **Empty your active hand before clicking a console or lathe**, or you hit it with what you hold. Click with sheets in hand only to insert them.
- R&D Console: `tgui_act {action: "researchNode", params: {node_path: "/datum/techweb_node/parts_upg"}}`. Use the paths from the plan. `data_changes` shows the points drop; "Not enough research points..." in chat means wait or enqueue. A Research button drawn disabled because something is queued still works through `tgui_act`.
- Protolathe: `tgui_act {action: "build", params: {design_path: "/datum/design/rped", amount: 1}}`. Find other design paths with `tgui_window {find: "Health Analyzer"}`. Printed items appear on the protolathe's tile: `search` for them, then click to pick up.
- Useful design paths for you: `rped`, `screwdriver`, `wrench`, `crowbar`, `wirecutters`, `multitool`, `weldingtool`, `inducer`, `healthanalyzer`, `analyzer`, `signaler`, `experi_scanner`, the parts in "Upgrading machines", `super_cell`, `super_battery` (each `/datum/design/<name>`).
- Experi-Scanner: hold it, press `key Z` (use in hand) to open its "Experiment Configuration" window, `tgui_act {action: "select_experiment", params: {ref: ...}}` (the ref is in the window's `experiments` list), then click each target with the scanner in hand. Chat: "You scan X." or "X is not related to your currently selected experiment."
- **Science Hub on your PDA** (verified in code, untested through the client): it needs your ID inside the PDA. Click the PDA with your ID in hand, then wear the PDA in your ID slot so doors still read your access. Open the PDA, `tgui_act {action: "PC_runprogram", params: {name: "experi_track"}}`, then the same `researchNode` actions as the console. It needs station networking (NTNet).
- A window shown "view-only" or closed after you walked away or lost power: click the machine again.
- Before researching, glance at the points in the window instead of reading the whole node list (it's large).

## Checklist

Shift start:
1. load_map; walk to Research and Development; take the lobby flash and an Experi-Scanner on the way.
2. Insert 50 iron + 50 glass into the protolathe.
3. Research nodes 1-6 as points allow; enqueue the next one.
4. Print a screwdriver and an RPED; announce on common.

Every 5-10 minutes:
1. Check points; research the next node; announce who prints what where; keep one node enqueued.
2. Answer requests (radio, the Research Lab Desk bell).
3. Do an upgrade round with the RPED (your lab, then Hydroponics, Chemistry, Cryogenics, Security).
4. Scan for experiments when you pass their targets.
5. Watch for anomalies and power loss (+0/sec).

## Sources

- Code (tgstation 54c22023): `code/modules/jobs/job_types/scientist.dm`, `code/datums/id_trim/jobs.dm`, `code/modules/research/` (rdconsole.dm, destructive_analyzer.dm, server.dm, part_replacer.dm, machinery/, techweb/, techweb/nodes/*.dm, designs/), `code/controllers/subsystem/networks/research.dm`, `code/__DEFINES/research.dm`, `code/modules/experisci/`, `code/datums/materials/material_container/remote_materials.dm`, `code/modules/mining/machine_silo.dm`, `code/modules/assembly/flash.dm`, `code/game/objects/effects/anomalies/_anomalies.dm`, `code/modules/research/anomaly/anomaly_core.dm`, `code/modules/modular_computers/file_system/programs/techweb.dm`, machine RefreshParts procs; tgui `interfaces/Techweb/`, `Fabricator.tsx`, `ExperimentConfigure.tsx`, `DestructiveAnalyzer.tsx`, `ExosuitFabricator.tsx`, `Signaler.tsx`.
- Map: `_maps/map_files/MetaStation/MetaStation.dmm`; area names from `code/game/area/areas/station/`.
- Previous round's scientist report: `/workspaces/seeker-play/play/crew/runs/12-scientist/report.md`.
- /tg/station wiki (CC BY-SA 3.0): Scientist, Guide_to_Research_and_Development (Internet Archive captures, Jan-Feb 2026; point costs there are outdated).
