# Station Engineer (MetaStation)

## 1. The job

The station runs on the **Supermatter crystal**: emitters fire lasers into it, it throws electrical arcs into tesla coils, and the coils charge the **SMES** units that power every APC on the station. Until the crystal runs, the station lives on the charge the SMES start with, and nothing refills it. In yesterday's shift the engine was never confirmed stable, the station's power ran out, the radio died for about 12 minutes because telecomms lost power, and the engineer died when they were pulled into the near-vacuum chamber. Success looks like this: the engine runs within about 10 minutes of the shift starting, holds 100% integrity for the rest of the shift, the SMES charge, every department has power, and you're both alive at the end.

There are two of you.
- **Engineer A** runs the Supermatter engine and the power grid (SMES).
- **Engineer B** handles repairs, APCs, telecomms, solars and hull breaches, and is A's buddy at the engine.

If a Chief Engineer is on shift, they are your boss and their orders come first. If not, you answer to the Captain, then the Head of Personnel. More players can join in any job at any time, including more engineers. Bring new engineers into this plan and give them tasks from it.

**Buddy rule at the engine:**
- Nobody does the chamber-door step or the emitter step alone. The other engineer stands in the Supermatter Engine Room, in view, out of the doorway, and keeps NT CIMS open.
- Say each step on the engineering radio before you do it ("A: in the chamber doorway, setting the chamber pumps") and say when you're out.
- If your partner goes silent for 2 minutes near the engine, go and look, but don't follow anyone into the chamber.
- If B isn't available yet, A still starts the engine on time, avoids the doorway step whenever the AI can do it instead, and reports every step on the radio.

## 2. Starting kit and access

**Outfit** (code: `station_engineer.dm`):
- Engineer's jumpsuit, work boots.
- **Insulated gloves**: yellow gloves that fully protect you from electric shocks.
- **Welding hard hat**: its visor starts up, so flip it down before you weld.
- **Engineering radio headset**.
- **Engineering PDA** in your left pocket.
- **T-ray scanner** in your right pocket: it shows cables and pipes under the floor.
- **Industrial backpack**, holding an **RCD with 160 matter** and an extended-capacity survival box (extended emergency oxygen tank and breath mask).
- **Toolbelt**: screwdriver, wrench, industrial welding tool (40 fuel), crowbar, wirecutters, multitool, cable coil.

**Engineering skillchip:** it shows you what each **airlock and APC wire** does, so the wire window names the wires for you.

**PDA programs:**
- **NT CIMS** (`ntcims`): the crystal monitor.
- **Canary** (`alarmmonitor`): station alarms.
- **AtmoZphere** (`atmosscan`): reads the gas on your tile.

PDA programs need NTNet, which runs through the **NTNet Quantum Relay** in the Telecomms Server Room. Wall consoles work without it.

**Access:** Engineering, Engine Equipment, Construction, Technical Storage, Telecomms, MiniSat (AI satellite), Maintenance, External Airlocks, Mineral Storeroom, Aux Base, Mech Engine. If 20 or fewer players were ready at round start, you also get **Atmospherics**. You **cannot** open:
- the Chief Engineer's Office,
- Secure Tech Storage (it also needs command access),
- the AI Chamber.

**Radio keys:**
- `;` = common
- `:e` = engineering
- `:i` = speak into a wall intercom next to you. This still works when telecomms is down; see §7.

## 3. Where things are on MetaStation

Engineering is on the starboard (east) side. Use `walk_to {area: "Engineering"}` from anywhere. Lockers open with your ID (Engine Equipment access).

**Engineering Foyer:**
- You enter it from the **Starboard Primary Hallway** through the **"Engineering Foyer"** door.
- North: two cycling **"Engine Room"** airlocks lead into Engineering. In and just past that corridor stand:
  - the **radiation suit closet** (radiation suit, radiation hood, Geiger counter),
  - a fire-safety closet and two tool closets,
  - the **welding supplies locker** (3 welding helmets, 3 welding tools),
  - the **electrical supplies locker** (2 inducers, 3 electrical toolboxes, 3 APC electronics, 3 multitools, 2 insulated gloves).
- East: **Shared Engineering Storage** (YouTool vendor, protolathe), the Circuit Workshop and the **"MiniSat Access"** hatch to the **Transit Tube** room (the way to telecomms).
- South: Atmospherics.
- **Technical Storage** opens off the hallway north-west of the Foyer. It holds 2 handheld flashes, insulated gloves, multitools, electrical toolboxes, cells and a cell charger, airlock and APC electronics.
- **Telecomms Storage** (spare telecomms parts) opens off the hallway south-west of the Foyer.

**Engineering (the main hall):**
- **"Power Monitoring" room, west side near the south end:** the **three SMES** ("power storage unit") and the **engineering console** (AmpCheck power monitor, Canary, NT CIMS). The console works without NTNet.
- **West wall:**
  - the Engi-Vend (engineering scanner goggles, multitools, smart metal foam grenades, high-capacity cells and batteries, electronics),
  - the EngiDrobe,
  - a cell charger,
  - the "Secure Storage" shutters (4 spare emitters inside; only the Chief Engineer's Office can open them).
- **Middle:**
  - a **P.A.C.M.A.N.-type portable generator**,
  - an engineering crate with 30 **plasma sheets**, iron, glass and rods, plus 150 iron and 150 glass on the tables,
  - 2 smart metal foam grenades,
  - mesons, toolbelts, engineering scanner goggles and 3 RPDs,
  - a fuel tank and a water tank.
- **North end:**
  - the "Engineering Storage" room: 2 suit storage units with **engineering MODsuits** (space-proof, radiation-proof, magboots), a tank dispenser, 3 insulated gloves, plasteel and reinforced glass,
  - 2 **engineer's lockers** (mechanical toolbox, gas mask, extended oxygen tank, engineering scanner goggles, holosign projector).
- **East wall:** three **"Supermatter Engine Room"** doors.
- **South-west:** the **Chief Engineer's Office** (CE access only). **Poly**, the Chief Engineer's parrot, lives there and repeats old radio lines, including fake engine alarms.
- **North:** the Gravity Generator Foyer, then the **Gravity Generator Room** (2 more radiation suit closets). **Starboard Bow Solar Access** is through maintenance to the north-east.

**Supermatter Engine Room:** a large room east of Engineering.
- In its middle is the **Supermatter Engine** area (its own area name). That area is the 3×3 crystal chamber, plus a small airlock with two doors both named **"Supermatter Chamber"** on its west side: the outer door, a one-tile antechamber, then the inner door. The tesla coils and grounding rods sit in alcoves north and south of the crystal, behind plasma glass.
- The east end of the room, behind two **"Laser Room"** doors, holds the emitters and reflectors. The north alcove (the freezers) has a fire-safety closet and a table with two spare oxygen tanks and a breath mask.
- The room's APC is in the Laser Room. **If that APC dies, every pump, filter and freezer in the room stops.** Only the two chamber pumps (Gas to Chamber, Gas to Filter) keep running.

**Telecomms** is on the AI satellite (MiniSat), east of the station; see §7.

## 4. The Supermatter engine

### 4.1 How it works (numbers from the code)

- **Integrity** is 100% minus damage.
  - Below **95%** the crystal says on the engineering radio: "Danger! Crystal hyperstructure integrity faltering! Integrity: X%".
  - Below **25%** it says on **common**: "CRYSTAL DELAMINATION IMMINENT!".
  - At **0%** a **15-second countdown** starts. Healing above 0% in time stops it.
  - The crystal repeats its warnings every 60 s (every 30 s below 25%). The real speaker is the "supermatter crystal". Lines from Poly are fake.
- **Heat damage:** when the gas the crystal absorbs is hotter than its **temperature limit**, it loses up to 0.3% integrity per second (about 18% a minute). Below the limit it heals up to 0.2%/s.
  - The limit is 313 K, doubled to **≈626 K** while the absorbed gas is under 100 mol (NT CIMS shows the limit as `temp_limit`).
  - From 100% to 0% at maximum heat damage takes about 5–6 minutes. More damage comes from energy above **5,000 MeV** (5 GeV) and from over **1,800 absorbed moles**.
- **Internal energy** comes from emitter hits (+60 MeV per hit) and from hot gas (oxygen and plasma add power; nitrogen adds none). It also decays on its own.
  - Three emitters on a nitrogen engine settle at about **1.3–1.6 GeV**. That yields about **1.4–1.7 MW** of arcs into the coils (`zap_transmission`).
  - The crystal turns energy into heat, plus plasma and oxygen waste. Pure **nitrogen** gives the lowest waste multiplier (0.5). **Plasma** in the chamber multiplies heat by up to 14×, so keep plasma and oxygen out.
- **A healthy MetaStation engine reads roughly** (from a stable run on this server): integrity **100**, energy **1.3–1.6 GeV**, gas temperature **70–85 K**, absorbed moles **≈14**, gas **≈97% N2**.
  - NT CIMS shows the gas the crystal **absorbs**, which is 15% of its tile. So 14 mol in CIMS means about 95 mol in the chamber, around 20 kPa: **far below room pressure**.
- **Hazards around an active crystal:**
  - **Touching it** (walking or being pushed into it, or touching it with an item) turns you to dust instantly.
  - It **pulls** loose things and people toward itself: up to 3 tiles away once energy passes 2.5 GeV, 1–2 tiles below that. Magboots (switched on) stop the pull.
  - It sends out **radiation** within 8 tiles. Only a radiation suit **and** radiation hood worn together (or a MODsuit with its radiation module) protect you. A suit without a hood doesn't count. Radiation means toxin damage over time.
  - It causes **hallucinations** for anyone who can see it within about 6–7 tiles. **Mesons do not prevent this in this version**; only breaking line of sight does. Hallucinations can show you fake people, fake attacks and fake messages. Trust NT CIMS readings and the radio, and step out of view.
- **Bullets damage the crystal; lasers don't.** Never fire a gun at it. A random "space dust" event can hit the crystal and switch it on early, so set up the cooling first.

### 4.2 The gas loop on this map

The coolant is **nitrogen**. Gas circulates like this:

1. **Two Nitrogen canisters** feed the cold line through **"External Gas to Loop"** (×2).
2. The cold line runs down past the **"Engine Coolant Bypass"** (it leaks cold gas straight to the hot line; **turn it off**).
3. **"Gas to Chamber"** pushes it through 3 chamber vents into the chamber.
4. 3 chamber scrubbers pull the chamber gas out through **"Gas to Filter"**.
5. The gas passes the **unnamed "gas filter"** south-west of the chamber (it can divert one gas into two empty canisters; leave it on with nothing selected).
6. The hot line runs east along the south side. **"Gas to Cold Loop"** sends it through heat-exchange pipes in space. **"Cold Loop to Gas"** brings it back. ("Cooling Loop Bypass" skips space cooling; **leave it off**. "Atmos to Loop" lets in gas from Atmospherics.)
7. The gas rises through **four "gas filter"s in a column east of the chamber**. The southernmost one is preset to **N2**: it sends the nitrogen back into the cold line and passes everything else north. The other three are set to nothing and pass waste north to a vent into space. **Every filter must be ON.** A filter that's off blocks the line.
8. The cold line runs north and then west across the north side, through **"Gas to Mix"**, the two freezers ("Temperature control unit") and **"Mix to Gas"**, with **"Mix Bypass"** alongside. Then it comes back down to step 2.

| Machine (in-game name) | Where | Start state | Set to |
|---|---|---|---|
| Nitrogen canister ×2 | NW of the chamber, on connector ports | **not connected** | wrench to the port; **valve stays closed** |
| External Gas to Loop ×2 | just west of the canisters | off, 101 kPa | ON, 4500 kPa |
| Engine Coolant Bypass | on the tile in front of the outer "Supermatter Chamber" door | **ON** | **OFF** |
| Gas to Chamber | Supermatter Engine area, alcove north of the antechamber | off | ON, 4500 kPa |
| Gas to Filter | Supermatter Engine area, alcove south of the antechamber | off | ON, 4500 kPa |
| gas filter (blue, SW) | south-west of the chamber, next to two empty canisters | off, nothing, 200 L/s | ON, nothing selected |
| Gas to Cold Loop | south side | ON, 101 kPa | 4500 kPa |
| Cold Loop to Gas | south side, east of it | ON, 101 kPa | 4500 kPa |
| Cooling Loop Bypass | south side, between those two | off | leave OFF |
| Atmos to Loop | south side, west | off | OFF unless Atmospherics is sending N2 |
| gas filter ×4 (white column) | east of the chamber, west of the Laser Room | off; southern one N2, others nothing; 200 L/s | all ON; keep N2 only on the southern one |
| Gas to Mix / Mix to Gas / Mix Bypass | north side of the room | off | all ON, 4500 kPa |
| Temperature control unit ×2 (freezers) | north alcove, behind two "Supermatter Engine Room" doors | off, 293.15 K | ON, **73.15 K** (minimum) |
| engine air alarm | chamber's west wall, just south of the outer chamber door | unlocked; controls the chamber's 3 vents and 3 scrubbers | vents: external limit off; scrubbers: siphon + expanded range (in that order, see below) |
| Radiation Shutters Control (button) | chamber's west wall, just north of the outer chamber door | shutters open | press after the engine is stable (closed shutters block radiation) |
| emitter ×3 | Laser Room: one at the north end facing south, two at the south end facing north | off, welded to the floor, on the station power grid | ON after cooling works |
| reflector box ×2, double sided reflector, reflector ×2 | Laser Room | pre-aimed (box reflectors 270°, double 45°, the southern single 225°) | don't touch; lock their rotation with a screwdriver |
| tesla coil ×4, grounding rod ×2 | alcoves north and south of the crystal | anchored | nothing to do |

The beams travel west along the crystal's row: out of the Laser Room, through a window, across the open tiles of the engine room east of the chamber, then through the chamber window into the crystal. **Anyone standing in that row, or in front of an emitter, gets shot** (30 burn per hit).

### 4.3 Setup, step by step (A does it, B is the buddy; aim to finish within 10 minutes of shift start)

Keep your **hands empty** for every click except the wrench step. A plain click with a tool in your active hand uses the tool on the machine; with a wrench, that **unfastens the pump** and dumps its gas. Ctrl-click and alt-click are safe.

1. **Gear (2 min).**
   - Put on the radiation suit **and** radiation hood (radiation suit closet in the Engine Room corridor, or the two in the Gravity Generator Room). The suit slows you down, so A keeps it on and B can take it off for errands.
   - Keep your insulated gloves on.
   - Open NT CIMS: open your PDA's window and send `PC_runprogram {name: "ntcims"}`, then `PRG_refresh`. Read `sm_data`: `integrity`, `internal_energy`, `gas_temperature`, `temp_limit`, `gas_total_moles`, `gas_composition`, `zap_transmission`, `waste_multiplier`. Expect integrity 100 and energy 0 at the start.
   - Say on `:e`: "A at the engine, starting setup".
2. **Canisters.**
   - With the **wrench** in your active hand, click each **Nitrogen canister** once ("You fasten Nitrogen canister to the port").
   - Open each canister's window and check `portConnected: 1`.
   - **Do not open the valve.** A connected canister shares its gas with the port's pipe on its own. With no tank inserted, the "release valve" dumps gas **into the room on its tile**. If a valve is open (`valveOpen: 1`), close it with `valve`.
   - Put the wrench away.
3. **Engine Coolant Bypass:** ctrl-click it → "turned off".
4. **External Gas to Loop ×2:** ctrl-click (on), then alt-click ("pressure output set to 4500 kPa").
5. **Chamber pumps.** This is the only step done from the chamber airlock. Do it now, while the crystal is inactive and the chamber still holds normal air, or ask the AI to set these two pumps remotely instead.
   - Stand on the Engine Coolant Bypass tile, west of the outer "Supermatter Chamber" door.
   - `move` east into the door until it opens, and step **into the outer doorway**. `walk_to` refuses to go there; `move` is the deliberate way in.
   - From the doorway, both pumps are diagonally next to you. **Gas to Chamber** (north-east): ctrl-click, alt-click. **Gas to Filter** (south-east): ctrl-click, alt-click.
   - **Step west out of the doorway.** Never go further east than the outer doorway.
   - B watches from the room and confirms on `:e`.
6. **Blue gas filter** (south-west of the chamber): ctrl-click → on. Leave its gas list empty; its rate is already 200 L/s.
7. **North side:** Gas to Mix, Mix to Gas, Mix Bypass: ctrl-click and alt-click each.
8. **Freezers:** open each **Temperature control unit** window. Send `power`, then `target {target: 73.15}`. Check `on: 1`, `target: 73.15`. **Don't alt-click a freezer:** the first alt-click sets it to **573 K, heating**.
9. **White filter column:** ctrl-click all four filters on. Open the southern one and check that nitrogen (`n2`) is the only enabled gas. Check the other three have none.
10. **South side:** alt-click **Gas to Cold Loop** and **Cold Loop to Gas** to 4500 kPa (both are already on). Leave Cooling Loop Bypass and Atmos to Loop off.
11. **engine air alarm, vents:**
    - Open the alarm's window. It lists 3 "Supermatter Engine air vent"s and 3 "air scrubber"s.
    - For each vent, send `excheck {ref: <vent refID>, val: <that vent's current checks value>}`. The action flips the external-limit bit: with `checks: 1`, send `val: 1`, which gives `checks: 0`. Sending `val: 0` does nothing.
    - Leave the vents **on** and on "Pressurizing" (`direction: 1`). **Never set the vents to siphon.**
12. **Wait 1–2 minutes and read NT CIMS.** Moles should rise, nitrogen should take over the composition and the temperature should fall. **Only when `gas_total_moles` is above about 8 and N2 is above about 90%:** set each scrubber to siphon, `scrubbing {ref, val: 0}`, then `widenet {ref, val: 1}`.
    - Siphoning before the nitrogen arrives empties the chamber to vacuum. That happened in two earlier attempts.
13. **Read CIMS again over 1–2 minutes.** Go on only when the gas temperature is **below about 100 K**, moles are steady around **10–20**, and N2 is 95% or more. If not, check every machine in the table again (§4.6).
14. **SMES** (B can do this in parallel, see §5.1): all three set to input 200 kW and output 190 kW.
15. **Emitters.**
    - Announce on `:e` ("A: emitters going on, stay out of the Laser Room beam lines").
    - Enter the Laser Room. Click each **emitter** with an empty hand **from beside or behind it, never from in front**. You should see "You turn on emitter".
    - Examine each one. "Its status display reads: Emitting one beam between…" means it is firing. "glowing faintly" means it has no power (§4.6). "currently turned off" means it is off.
    - Within a minute, NT CIMS `internal_energy` should climb by about 60 MeV per hit, toward 1–2 GeV, and `zap_transmission` should show hundreds of kW to MW.
    - Don't kiss the crystal, throw things at it, or fire guns at it to "kick-start" it. The emitters are enough, and an inner door left open kills you.
16. **Radiation Shutters Control:** click the button (it needs engineering access). The "Radiation Chamber Shutters" close.
17. **Lock it down:**
    - Click each running emitter with your ID or PDA in hand to lock its controls ("You lock the controls"). This only works while it's on. Locked emitters can't be switched by someone without Engine Equipment access.
    - With a screwdriver, click each reflector once ("You lock reflector's rotation"). An empty-hand click opens its "Reflector" window, which shows `rotation_angle`. Read it there, but never send `rotate`.
18. **Watch for 5 minutes.** Read CIMS every minute: integrity 100, energy steady, temperature steady and well under `temp_limit`. Then report on `:e` and `;`, for example "Engine stable: integrity 100, 1.4 GeV, 75 K, SMES charging." From then on, check it every 5–10 minutes.

### 4.4 What not to do (each of these has killed engineers or engines)

- **Never step past the outer "Supermatter Chamber" doorway, and never open the inner door.** After step 12 the chamber is far below room pressure. Opening the inner door pulls you into the chamber, and you choke, freeze and then touch the crystal. That is exactly how the engineer died yesterday: standing in the inner doorway. The doors cycle (opening one closes the other), so keep it that way.
- Don't siphon the chamber before nitrogen is flowing into it, and never set the chamber **vents** to siphon.
- Don't start the emitters before the loop reads cold, nitrogen-rich and above 8 mol.
- Don't open the Nitrogen canisters' valves, and don't connect plasma or oxygen canisters to any port in the room. The three empty connector ports north of the freezers feed the freezer loop: **leave them empty**.
- Don't turn on Cooling Loop Bypass or Engine Coolant Bypass, don't change which gas the southern white filter takes, and don't turn any filter off.
- Don't stand in the beam row east of the chamber, in front of an emitter, or within 3 tiles of the crystal (its pull).
- Don't click machines with a tool in your hand, and don't alt-click freezers.
- Don't trust engine alarms from **Poly** or from anyone on the radio you can't confirm. Confirm on NT CIMS before you react.

### 4.5 Ongoing loop (A)

Every 5–10 minutes, read NT CIMS (or the engineering console's NT CIMS if PDA programs are down). Check:
- integrity is 100,
- `gas_temperature` is under about 150 K and far below `temp_limit`,
- moles are steady,
- N2 is at 90% or more.

Check the SMES as well (§5.1). Report changes on `:e`. If integrity drops below 100, act right away (§4.6). Don't wait for the radio warning.

### 4.6 Troubleshooting

| Symptom (NT CIMS / radio) | Likely cause | Do this |
|---|---|---|
| Integrity falling and `gas_temperature` above `temp_limit` | cooling failure | 1) **Emitters OFF** (unlock with your ID first if you locked them). 2) Walk the loop: both chamber pumps, External Gas to Loop, Gas to Cold Loop, Cold Loop to Gas, Gas to Mix, Mix to Gas on and at 4500 kPa; all 5 filters on; freezers on at 73 K; scrubbers siphoning; vents on. 3) Check the Supermatter Engine Room APC has power. 4) Turn the emitters back on only once the temperature is back under 100 K. |
| Moles very low (under ~5), chamber near vacuum | scrubbers siphon but nothing feeds the chamber | Set the scrubbers back to `scrubbing {val: 1}`. Check Gas to Chamber is on, the canisters are connected and not empty, and External Gas to Loop is on. Siphon again once moles climb. |
| Nitrogen running out (canisters near 0 kPa, moles falling) | coolant lost (the waste vent, a leak) | Ask the Atmospheric Technician for more Nitrogen canisters; wrench them onto the same ports, valves closed. Or have them send nitrogen through **"Mix to Engine"** in Atmospherics (it feeds the engine line, off at round start) while you turn **Atmos to Loop** on (also off at start). |
| O2 or plasma high in `gas_composition`, waste multiplier above 1 | filters wrong or off | Southern white filter ON with N2 only; the other three ON with nothing; blue filter ON; scrubbers siphoning. Emitters off until it clears. |
| Energy 0 with emitters "on" | beams don't reach, or emitters unpowered | Examine the emitters. "Glowing faintly" means the station grid has no power: SMES output, §5.3. If they're firing, check nothing stands in the beam path and the reflectors read 270° (both boxes), 45° (double) and 225° (southern single). |
| Energy above 5 GeV and rising | too much energy, or hot oxygen/plasma | Emitters off. Power damage and a "tesla" delamination start above 5 GeV. |
| Engine fine but station power low | SMES settings, coil side | §5.1: `inputting: 1` and `inputAvailable` above 0 on each SMES. If input stays 0, the coils, terminals or cable under the SMES are damaged: B traces them with the T-ray scanner. |
| "Danger! … integrity faltering" on the radio | real damage (if the speaker is the crystal) | Confirm on CIMS, then work through the first row. Say on `:e` what you're doing. |
| "CRYSTAL DELAMINATION IMMINENT", integrity under 25% and still falling | cooling can't keep up | Emitters off and fix the first row for at most a minute. If integrity keeps falling: **evacuate** (§10). |

**Delamination:** at 0% (after the 15 s countdown), the crystal explodes and irradiates and hallucinates the area. With a nitrogen chamber the blast is small (heavy damage about 9 tiles out, light damage about 11). With an oxygen- or plasma-rich chamber it reaches up to about 37 tiles of heavy damage. When you evacuate:
- Announce on `;` "Supermatter delaminating, everyone out of Engineering and Atmospherics".
- Leave Engineering and get at least 20 tiles away, more if the gas is oxygen or plasma.
- Ask the AI to keep people out.
- Afterwards, B fixes breaches and both of you restore power from the SMES, solars and P.A.C.M.A.N.s.

## 5. The power grid

### 5.1 SMES (A, or B in parallel at shift start)

- **Where:** three "power storage unit"s in the **Power Monitoring** room (west side of Engineering, near the south end).
- **Wiring:** they take input from the tesla coils through their terminals (the tiles north of them) and output to the whole station grid.
- **Start state:** each holds **50 MJ** and outputs **90 kW**, input 50 kW. Together they supply 270 kW. Nothing recharges them until the engine runs. At full load they last **about 9 minutes**, then APC cells take over until they run dry. That's why the engine comes first.
- **Set each one:** click it to open the "Smes" window. Send `input {target: 200000}` (watts; 200 kW is the maximum, `target: "max"` also works) and `output {target: 190000}`. Check `inputAttempt: 1` and `outputAttempt: 1`; if either is 0, send `tryinput` or `tryoutput` to toggle it.
- **Healthy:** `inputting: 1` with `inputAvailable` above 0, `outputting: 1` with `outputUsed` near 190 kW, and `charge` rising.
- **Other SMES on the map:**
  - **Gravity Generator Room** (its own small grid, with a P.A.C.M.A.N.).
  - **MiniSat Maintenance** on the AI satellite (it powers the satellite **and telecomms**).
  - The AI chamber.
  - One in each of the four solar maintenance rooms (empty, since the solars aren't wired).
  - The Incinerator.

### 5.2 Checking the station gets power

- **Engineering console** (Power Monitoring room): open **AmpCheck** for `supply` vs `demand` and a table of every APC on the main grid with its charge % and channel states. Supply should be above demand once the engine runs, and APC charges should rise.
- There's also the **Bridge Power Monitoring Console** on the Bridge.
- The satellite and telecomms are on a separate grid: use the power monitoring console in **MiniSat Maintenance**.

### 5.3 Backup power: the P.A.C.M.A.N.

The "P.A.C.M.A.N.-type portable generator" in Engineering sits on a station cable. Use it when the grid is dead and the emitters "glow faintly":
1. Wrench it to anchor it.
2. Click it with **plasma sheets** (30 in the engineering crate) to load fuel.
3. Open its window and send `toggle_power`. It makes 10 kW per output level (`higher_power` / `lower_power`, 1–4). That's plenty for the emitters, which draw about 0.3 kW each and get first claim on grid power. Keep it at level 1–2: an **overheating P.A.C.M.A.N. explodes**.

More P.A.C.M.A.N.s, already fuelled, stand in maintenance rooms around the station.

### 5.4 APCs (B)

Every room has an APC on its wall (the "area name APC").

- **Unlock:** click it with your ID or PDA in hand ("unlocked"; needs Engine Equipment access). The "Apc" window then accepts actions.
- **Read:**
  - `externalPower`: 0 none, 1 low, 2 good.
  - `powerCellStatus`: cell %.
  - `chargingStatus`: 0 not charging, 1 charging, 2 full.
  - Equipment / Lighting / Environment status: 0 off, 1 auto (now off), 2 on, 3 auto (now on).
- **Auto shut-off** as the cell drains: below **30%** equipment turns off (consoles, telecomms machines, vendors). Below **15%** lighting turns off too. At **0%** everything goes, including environment (air alarms, vents, doors).
- **Actions:**
  - `channel {eqp|lgt|env: 1 off, 2 on, 3 auto}`.
  - `breaker`: the whole APC on/off.
  - `charge`: charging on/off.
  - `cover`: cover lock.
  - Setting a channel to 2 (on) keeps it running below the auto threshold until the cell is empty. Use it for critical rooms (telecomms, medbay), and turn lighting off (1) to save their charge.
- **Recharge a cell in place:** click the APC with an **inducer** (2 in the electrical supplies locker). Stand still while it charges in 1-second pulses. An inducer's 10 MJ battery refills about four APC cells (2.5 MJ each).
- **Swap a cell:** unlock, send `cover` to unlock the cover, crowbar the cover open, take the cell out with an empty hand, put a charged one in, crowbar the cover shut. Cell chargers are in Engineering, Technical Storage and the CE's Office; spare cells come from the Engi-Vend.
- **An APC that won't respond:** check its wires (§8.3). Spare "APC electronics" are in the electrical supplies locker, Technical Storage and the Engi-Vend.

## 6. Engineer B's other jobs

### 6.1 Solars (optional, EVA)

MetaStation's four arrays are Port Bow, Port Quarter, Starboard Bow and Starboard Quarter Solar Array. Their control rooms are the "… Solar Maintenance" areas: "Port Bow Solar Control", "Starboard Bow Solar Control" and so on. **The arrays are not connected at round start.**
- The main cable to each array has deliberate gaps on the space-side catwalks, and the panel rows aren't joined to it.
- The Port Quarter array is half unbuilt panel assemblies; the Starboard Quarter array has floor but no panels.
- The control computer's window shows `connected_panels: 0` until the array is wired.

Wiring them is space work:
- **Gear:** an engineering MODsuit (Engineering Storage), internals, a buddy, insulated gloves, cable coil and rods.
- Lay cable onto catwalk tiles over the gaps (a cable only goes on a catwalk over space, or on plating).
- Then open the solar control and send `refresh`, then `tracking {mode: 2}` (automatic; it needs the tracker connected) or `{mode: 1}` (timed).
- Each array feeds its room's SMES, which outputs to the station. Check that SMES's output is on.

Do solars only once the engine is stable and nothing is broken. Never do them alone.

### 6.2 Gravity generator

The "gravitational generator" in the **Gravity Generator Room** starts **on** and charged. It has its own SMES and P.A.C.M.A.N. backup.
- Within **2 tiles of it gravity is crushing** ("Crushing Gravity" damage), and its control part is the bottom-middle of the 3×3 machine, inside that zone. **Leave it alone unless gravity is actually off station-wide.**
- If gravity is off: check the room's APC and SMES first. Then step next to the bottom-middle part, open "GravityGenerator" (`breaker` and `charge_count` fields; `gentoggle` flips the breaker), let it charge to 100 and leave immediately. Yesterday's engineer lost half their health doing this for no reason.

### 6.3 Hull breaches (with the Atmospheric Technician)

Signs:
- an air alarm or the Canary program flags a room,
- a "Choking (No O2)" or low-pressure alert,
- `walk_to` reports space or "danger".

How to fix one:
- **Don't walk in without internals and a space suit or MODsuit.** Wind blows toward the hole. Mark it from outside and tell the Atmospheric Technician on `:e`.
- **Fastest fix: your RCD.** Use it in hand to open its window, pick the floor/wall design ("Construction" → "Structures", the first entry), and click each space tile to place plating instantly (3 matter per tile, 1 if there's a lattice). Click a floor with the same design to build a wall (16 matter, 2 s). Right-click deconstructs (careful). Refill the RCD by clicking it with iron sheets (4 matter each) or glass.
- **By hand:** click space with **rods** to make a lattice (1 rod), click it with a **floor tile** to make plating, then add a floor tile on top for a normal floor.
- **Broken window:** grille first (2 rods on the floor), then a window (glass sheets: 2 for a full-tile window), then fasten it with a screwdriver.
- **Smart metal foam grenades** (Engineering and the Engi-Vend) seal holes fast but can wall you in; you'll need a crowbar or welder to get out.
- Then the Atmospheric Technician refills the room. Don't open doors into a vacuum room. Doors between rooms with different pressures are dangerous.

### 6.4 Repairs and construction

- **Walls:** iron sheets right-clicked on an empty floor tile make a girder (2 sheets, 4 s). Clicking the girder with 2 more iron sheets makes a wall (4 s). A lit welder **cuts down a normal wall** in 10 s (unless it only has dents, which it smooths first; reinforced walls take more steps). Never weld outer walls by accident.
- **Floors:** pry a floor tile up with a crowbar to reach plating; put a tile back by clicking with floor tiles. Iron sheets make floor tiles from the sheet's recipe window.
- **Windows:** a welder on a damaged window repairs it (non-combat click).
- **Airlocks:** a welder on a damaged, closed airlock repairs it (left-click, 4 s). Right-click with a lit welder **welds it shut or unwelds it**. Spare "airlock electronics" are in Engineering and Technical Storage.
- **Cable:** with the floor tile removed, click plating with a cable coil. Wirecutters cut cable; keep insulated gloves on, because live cable shocks you. The T-ray scanner (right pocket) or the engineering scanner goggles' t-ray mode (use the goggles in hand to cycle none → meson → t-ray) show what's under the floor.
- **Welding:** flip your welding hard hat's visor down first. Welding without eye protection hurts your eyes. Refill the welder at the fuel tank in Engineering.

## 7. Telecomms: "the radio is dead"

**Where:** on the **AI satellite**, east of the station.
1. Go through the Engineering Foyer → "MiniSat Access" hatch → **Transit Tube** room.
2. Walk into the **"station tube pod dispenser"**: a pod forms around you and carries you to the satellite. `walk_to` doesn't know about the tube; use `move` into the dispenser.
3. Arrive in the satellite's entry room → "MiniSat Foyer" hatch. The **"Antechamber Turret Control"** is on the foyer's wall.
4. Go through the "MiniSat Antechamber" hatch into the satellite interior. **Its AI turrets stun everyone who walks through.** Before you go in, either ask the AI to turn them off, or click the turret control with your ID in hand to unlock it and send `power` (turn them back on when you leave).
5. In the interior, take the "Telecomms Control Room" hatch south. Telecomms servers and monitor consoles are there.
6. Two "Telecomms Server Room" hatches lead on to the server room: receivers, buses, processors, servers, broadcasters, the hub, the message server, the **NTNet Quantum Relay** and the blackbox.
7. **"MiniSat Maintenance"** (east side of the interior) holds the satellite's SMES and power monitor.

**Why it dies:**
- Telecomms has its own grid: the MiniSat SMES charges from the station. When station power fails, that SMES drains, then the two telecomms APCs drain. Below 30%, their equipment channel switches off and **every headset goes silent**. The NTNet relay also dies, and with it NT CIMS on PDAs.
- An EMP switches telecomms machines off for up to 5 minutes.
- Sabotage: a machine toggled off or smashed.

**Diagnosis, in order:**
1. **Check it's not just you.** If `say` on `:e` reports "no radio line of yours came back", the network is down.
2. **Talk anyway.** Stand next to a wall intercom (its room needs power) and `say ":i <message>"`. Intercoms and handheld "station bounced radios" (one on the Foyer rack) fall back to a direct broadcast on the station's z-level when telecomms is down, and headsets still hear it on common.
3. **Station power:** check the engineering console's AmpCheck. If the main grid is starving, fix the engine and SMES first.
4. **At the satellite:**
   - **MiniSat Maintenance SMES:** charge above 0, `outputting: 1`; raise input to 200 kW.
   - **Telecomms Server Room and Telecomms Control Room APCs:** unlock with your ID. Set Equipment to on (`channel {eqp: 2}`) and lighting off (`{lgt: 1}`). Recharge them with an inducer.
5. **Machines:** hold a **multitool** and click each telecomms machine to open its "Telecomms" window. The `toggle` action turns it on or off (it needs the multitool in your active hand). Examine each one: broken ones need parts from Telecomms Storage.

## 8. Doors

### 8.1 Opening a door for someone

You can't remote-open doors yourself. Ask the AI ("AI, open the Medbay door for the Chemist"), or meet the person and walk through ahead of them. Don't hack department doors without reason; it's treated as breaking in.

### 8.2 Stuck doors

- **Unpowered airlock:** a **crowbar** pries it open or shut instantly. This doesn't work on a bolted or welded door.
- **Powered airlock:** a crowbar won't move it ("The airlock's motors resist"). Hack it (§8.3).
- **Bolted:** examine says the bolts are down. Raise them by pulsing the "Bolts" wire (only while the door has power) or ask the AI.
- **Welded:** right-click with a lit welder to unweld (4 s).
- **Firelocks** close automatically on fire or pressure alarms. Let the Atmospheric Technician clear the alarm first: there's usually a reason behind them.

### 8.3 Hacking an airlock (and APCs)

1. Screwdriver the airlock to open its maintenance panel.
2. Click it with wirecutters or a multitool to open the **"Wires"** window. Thanks to your skillchip, each wire shows its function next to its colour. Colours are the same for all airlocks in a round and change every round.
3. Actions:
   - `pulse {wire: "<colour>"}` needs a **multitool** in hand.
   - `cut {wire: "<colour>"}` needs **wirecutters** in hand; cutting a cut wire mends it.

| Airlock wire | Pulse | Cut |
|---|---|---|
| ID Scan | flashes the lights, ends emergency access | the ID scanner is dead: the door no longer opens for anyone walking into it, but pulsing "Open" now works |
| Open | opens or closes the door, **only if ID Scan is cut** or the door needs no access | — |
| Bolts | raises the bolts (with power) or drops them | drops the bolts |
| Main Power 1/2 | cuts main power briefly | no main power until mended (shocks you without gloves) |
| Auxiliary Power 1/2 | cuts backup power briefly | no backup power |
| AI Connection | AI loses control for 1 s | AI can't control the door |
| High Voltage Ground | electrifies the door briefly | **electrifies it permanently**; mend to stop |
| Safety | toggles the crush safety | the door closes on people |
| Timing | toggles closing speed | no auto-close |
| Feedback | toggles lights and sounds | — |
| High Voltage Circuit 1/2 | — | shocks you |

**Open a powered door you have no access to:** cut **ID Scan**, then pulse **Open**; pulse Open again to close it. To make a door unpowered (crowbar-able), cut one Main Power wire and one Auxiliary Power wire. Close the panel with the screwdriver and mend what you cut when you're done.

APC wires work the same way: Equipment, Lights, Environment, Main Power 1/2, Interface and AI Connection; the skillchip names them. Pulsing **Interface** unlocks the APC's controls briefly; cutting it locks them until you mend it.

## 9. Electrical hazards

- Your **insulated gloves** fully protect you from shocks: electrified doors and grilles, live cable, the wire panel. Keep them on. Budget insulated gloves (from other sources) are unreliable.
- An electrified door shocks whoever touches it without gloves. You can still hack it with gloves on.
- A **grille with a powered cable under it** shocks anyone who touches or attacks it.

## 10. Emergencies

- **Power failure:** A checks the engine and SMES (input, output, charge). B checks AmpCheck, then the medbay and telecomms APCs (inducer, Equipment channel on). If the engine can't run, start P.A.C.M.A.N.s. Tell the crew on `;` what's down and roughly when it'll be back.
- **Radio dead:** §7. Meanwhile, talk with `:i` at an intercom.
- **Hull breach:** §6.3, with the Atmospheric Technician.
- **Fire:** the Atmospheric Technician leads, with fire extinguishers from the wall cabinets. Cut a burning room's power only if the wiring is the cause.
- **Delamination:** §4.6. Get everyone else out of Engineering first, then yourselves.
- **Mass casualties:** clear wreckage with the RCD and a welder, and pull the injured to medbay.
- **Attacker in Engineering:** §11.
- **Evacuation:** leave the engine stable. If the cooling isn't working, switch the emitters off before you go. Board the shuttle together.

## 11. Defending yourself and engineering

Shared combat basics (combat mode, shoving, grabs, resisting) are in crew-basics.

**What you carry and what's nearby** (damage per hit):
- **mechanical or electrical toolbox:** 13 (mechanical in the engineer's lockers, electrical on the Foyer table and in the electrical locker),
- **fire extinguisher:** 13 (wall cabinets),
- **lit welding tool:** 15 burn,
- **wirecutters:** 6; **wrench, crowbar or screwdriver:** 5.

**Handheld flashes:** two are in Technical Storage (you have access). A flash blinds and stuns someone in front of you, and it's the best non-lethal tool you can get. Pick one up at shift start if your stance allows it.

**The engine is a sabotage target.** A saboteur might switch off pumps, filters or freezers, disconnect canisters, change the white filter, connect plasma to the freezer ports, switch off emitters, turn reflectors, open the chamber, cut the engine room's APC or cables, or break the heat-exchange pipes outside.

Countermeasures:
- Lock the emitters with your ID and lock the reflectors with a screwdriver.
- Keep the Engine Room and Supermatter Engine Room doors shut behind you, and never leave tools or canisters lying in the engine room.
- Check NT CIMS often.
- If someone without engineering business is in the engine room, ask them on the radio and in person to leave, and call Security and the AI. The AI can bolt doors and watch cameras.
- A Chief Engineer, Security or the AI can drop the **Engineering Security Doors**. Their "Engineering Lockdown" buttons are in the Chief Engineer's Office and the Engineering Security Post.

**Never fight in the Supermatter Engine Room:** a shove near the chamber or the beam line kills. Back out into Engineering, keep the fight away from the engine, and don't drag anyone into danger.

You're expected to stand your ground for the engine only by calling for help, locking things down and blocking doors. Leave the fighting to Security unless your personal stance says otherwise.

## 12. Working with the crew

- **Atmospheric Technician:** your closest partner. They supply nitrogen (canisters, or "Mix to Engine" → "Atmos to Loop"), refill breached rooms and handle fires. You fix the hull and power for them. Agree before either of you touches the other's engine machines.
- **AI:** sets the chamber pumps so nobody stands in the doorway, opens and bolts doors, switches off the MiniSat turrets, and watches the engine room on camera.
- **Captain / Head of Personnel:** they get an engine status when they ask and before the evacuation call. The HoP can add access you need.
- **Security Officers:** call them for intruders in Engineering. They may need doors hacked or rooms sealed.
- **Medical Doctors:** they treat radiation (toxin damage) and burns. Keep medbay's APC powered.
- **Scientist:** better parts for the emitters, SMES or freezers. Install upgrades only with the emitters off.
- **Quartermaster:** spare parts and canisters. **Janitor:** replaces lights, which only work if you keep the power on.
- **Everyone:** you report power and radio status on `;` when it changes. Ask people to report broken doors, windows and APCs with the room name.

## 13. Through the client

- `walk_to {area: "Supermatter Engine Room"}` gets you to the engine. Walks never enter the "Supermatter Engine" area (chamber and airlock) and never stop next to the crystal: step into the outer chamber doorway with one `move`, then `move` back out.
- `search` with `area: "Supermatter Engine Room"` (or `"Supermatter Engine"`) lists the loop's machines with their state. The two chamber pumps may only show up from close by, or through `tile`.
- **Ctrl-click** = on/off and **alt-click** = maximum on pumps and filters. Everything else goes through `tgui_window` and `tgui_act` (action names are in the steps above).
  - `data_changes` shows whether an action took effect.
  - Entries with value 0 may be left out of the answer, so check the exact field you set.
  - **MODsuit:** `deploy {ref}` each part, `activate`, then `select {ref}` the magboots module.
- **NT CIMS** can be read while the PDA stays in your pocket.
- **Equipping:** quick-equip (key E) puts on a held radiation suit or hood.
- **Held items:** the answer's `active_hand` says what a click will use. Empty your hand before you click a machine.
- **Radio:** `say` with the engineering radio, or text starting `:e`. If the answer says no radio line came back, telecomms is down (§7).
- A line from Poly, or a "danger" that NT CIMS doesn't show, is not proof. Near the crystal, hallucinations can add lines and attackers that don't exist: step out of view and re-read.

## 14. Checklists

**Engineer A, shift start (finish within ~10 min):**
1. Radiation suit and hood, gloves on, NT CIMS open.
2. Wrench both canisters (valves closed).
3. Engine Coolant Bypass off.
4. External Gas to Loop ×2 on and max.
5. Gas to Chamber and Gas to Filter on and max, from the outer doorway or by the AI. Step out.
6. Blue filter on.
7. Gas to Mix, Mix to Gas, Mix Bypass on and max; freezers on at 73.15 K.
8. 4 white filters on (southern = N2).
9. Gas to Cold Loop and Cold Loop to Gas max.
10. Vents: external limit off.
11. CIMS above 8 mol and N2 above 90% → scrubbers siphon + widenet.
12. CIMS below 100 K and stable → SMES 200 in / 190 out.
13. Emitters on, from behind.
14. Shutters closed.
15. Lock the emitters (ID) and reflectors (screwdriver).
16. Watch 5 min → report on `:e` and `;`.

**Engineer B, shift start:**
1. Gloves on, T-ray scanner in pocket, inducer from the electrical supplies locker, optionally a flash from Technical Storage.
2. Set the three SMES (200/190) and check AmpCheck.
3. Be A's buddy for the doorway and emitter steps.
4. Check the MiniSat SMES and the telecomms APCs once the engine is stable.
5. Then repair round: breaches, broken APCs and doors reported on the radio.

**Ongoing (both):**
- Every 5–10 min: NT CIMS (integrity 100, temperature under 150 K, N2 above 90%) and SMES charging.
- Watch AmpCheck for any APC under 30%.
- Answer repair calls with the room name and an estimate.
- Keep the Engineering doors shut.
- Re-check the engine after any fight, event or power alarm.
- Before evacuation: report the engine state, and leave the emitters on only if the cooling is fine.

## 15. Sources

- tgstation source at commit 54c22023: the job and outfit; the supermatter, emitter and reflector code; SMES, APC, P.A.C.M.A.N., solar, gravity generator and cable code; atmospherics machinery; telecomms, NTNet and radio; wires and doors; turfs and the RCD; PDA programs; radiation; tgui interfaces.
- `_maps/map_files/MetaStation/MetaStation.dmm`: machine presets, the cable networks, door access.
- /tg/station wiki (CC BY-SA 3.0, Internet Archive captures): Guide_to_the_Supermatter, Station_Engineer, Guide_to_power, Solars, Guide_to_Telecommunications, Gravity_Generator, Guide_to_construction. Where the wiki and the code disagree, this guide follows the code (for example, mesons don't stop the crystal's hallucinations in this version).
- Earlier rounds on this server: the engineering reports and the readings from a stable engine run.
