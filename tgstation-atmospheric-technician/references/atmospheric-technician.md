# Atmospheric Technician (MetaStation)

## 1. The job in one paragraph

You keep the station's air breathable. Atmospherics mixes nitrogen and oxygen into air, pushes it through the distribution loop ("distro") to every vent on the station, and pulls used air back through the scrubbers ("waste loop") to be filtered. You make sure that chain runs. You watch the alarm consoles, answer air alarms, seal and refill breached rooms, put out fires and clean up gas leaks (plasma, N2O, CO2). You also bring the engineers coolant (nitrogen) for the Supermatter engine when they ask. A good shift: distro never stops, every alarm you see gets a report and a fix, no one suffocates or burns, and you never make things worse by venting a room, mixing gases or opening a door onto vacuum. You're Engineering staff. If a Chief Engineer is on shift, they're your boss; the Station Engineers are your peers.

## 2. Starting kit and access

**Worn** (`code/modules/jobs/job_types/atmospheric_technician.dm`):
- atmospheric technician's jumpsuit (fire resistant).
- **atmospherics overalls** (suit slot): fireproof, fire armor 100. Its suit storage holds an analyzer, RPD, extinguisher, emergency oxygen tank, T-ray scanner or RCD.
- **atmospheric technician's toolbelt**: screwdriver, wrench, welding tool, crowbar, wirecutters, T-ray scanner, **pocket fire extinguisher** (30 units, force 3).
- **engineering radio headset**: Engineering channel (`say` with `radio: "engineering"`) plus Common (`radio: "common"`).
- **atmospherics PDA** (left pocket). Its apps:
  - **Canary**: the station's Atmosphere/Fire/Power alarms, readable anywhere.
  - **AtmoZphere**: reads the air where you stand.
  - **NT CIMS**: Supermatter status.
- **analyzer** (right pocket).
- Industrial backpack with an **extended-capacity survival box**: breath mask, extended-capacity emergency oxygen tank, epinephrine medipen.

**Access.** Atmospherics, Engineering, maintenance tunnels, external airlocks, Construction, Aux Base, Mineral Storeroom and mech engine. On rounds that start with fewer than 20 players you also get Engine Equipment, Tech Storage, Telecomms and the AI Satellite (Minisat).
- Air alarms need Engineering access: you have it.
- Your atmos access also opens: the atmospheric technician's lockers, the Atmospherics doors, the "Inner Pipe Access" windoors to the chamber pumps, and the "Atmospherics Lockdown" button.

## 3. Where things are on MetaStation

Atmospherics is on the starboard (east) side of the station, south of Engineering. From anywhere, `walk_to {area: "Atmospherics Gas Storage"}` (front office) or `{area: "Atmospherics"}` (main hall).

**Atmospherics Gas Storage** is the front office. You enter it from the **Engineering Foyer** (north) through the "Atmospherics" airlock. Its "Atmospherics Desk" windoor, with a desk bell, serves the **Starboard Primary Hallway**. What's inside:
- **Station alert console** (west wall): Atmosphere, Fire and Power alarms.
- **station atmospherics monitoring** console (west wall): the gas mix in the Distribution Loop and Waste Loop.
- **Atmospheric alert console** (south wall).
- **Tank dispenser**. A plain click gives a **plasma** tank; a **right click gives an oxygen tank**.
- Table at the north-east: **4 smart metal foam grenades**, T-ray scanners, welding helmets. Next to it: 2×50 iron sheets and two space heaters.
- **Canisters** in the south-west: 3 Air, 3 Oxygen, 3 Nitrogen, 3 Nitrous Oxide.
- **"Atmospherics Lockdown"** button (north wall): closes the "Atmospherics Blast Door" shutters over the desk and the main door.
- The "Atmospherics Monitoring" glass door (south-east) leads into Atmospherics.

**Atmospherics** is the main hall.

*West part, the equipment area:*
- **Two atmospheric technician's lockers** with the **atmos suit storage unit** between them.
- The **fire axe cabinet** on the wall beside them.
- The AtmosDrobe, emergency showers, a water tank, a large fuel tank; racks and tables with gas masks, multitools, high-capacity cells, air/fire alarm electronics, 2×50 glass and 2×50 rods.
- On the west wall: two **portable air pumps** and a **portable air scrubber** on connector ports, three empty canisters, and two air alarms.

*South part, the gas chambers:* seven sealed chambers behind windows, west to east:
- Nitrogen
- Oxygen
- Mixed Air
- Carbon Dioxide
- Plasma
- Nitrous Oxide
- Mix

In front of each chamber (north side) are its control computer and, except for Mixed Air and Mix, its filter: "Nitrogen supply control", "Oxygen supply control", "mixed air supply control", "Carbon Dioxide supply control", "Plasma supply control", "Nitrous Oxide supply control", "mix chamber control". The "X to Pure" pumps stand on the same row; "N2 to Airmix" and "O2 to Airmix" sit in the pipe corridor behind the "Inner Pipe Access" windoors (atmos access). The **air mixer** stands just north of the N2/O2 chambers.

*East part:*
- The port-mix pumps and three connector ports with empty canisters ("canister charging").
- Heaters, a freezer, the crystallizer.
- The "Hypertorus Fusion Reactor" doors to the **Atmospherics Engine** room (the empty HFR room; a third atmos locker is there).
- "Atmospherics External Access" airlocks to space (east end). **Never use them.**

**Atmospherics Pumping Room**: north of Atmospherics, through the "Distribution Loop" glass door. Distro and waste meet the station here:
- **"Air to Distro"** pump (north wall).
- "Distro to Waste", "Distro Staging to Distro", "Waste to Filter", "Distro Staging to Filter".
- Freezers and a heater.
- The distribution and waste loop gas flow meters.
- An air alarm.

**Incinerator**: reached from **Greater Starboard Maintenance** through the "Incinerator Access" door. It holds the burn chamber and gas turbine, a plasma tank, an ignition button and the fourth atmos locker. Leave the burn chamber alone unless an engineer asks.

**Outside Atmospherics**:
- **Starboard Primary Hallway**, just outside the desk: two portable air pumps on the "External Air Ports" and two portable scrubbers on the "External Waste Ports".
- The **Locker Room** has two more portable air pumps and two portable scrubbers.
- Fire-safety closets (red) are all over the station. Each holds a firefighter suit, gas mask, oxygen tank, fire extinguisher, red hardhat and emergency crowbar.
- Extinguisher cabinets on walls hold full-size fire extinguishers.

**Atmos lockers** (2 in Atmospherics, 1 in Atmospherics Engine, 1 in Incinerator), each:
- **rapid pipe dispenser (RPD)**
- **ATMOS holofan projector**
- **backpack firefighter tank**
- **atmospheric firesuit** (fire immune)
- **atmospheric firefighter helmet** (pressure-proof, works as a mask for internals, welding visor)
- atmospheric extrication gloves
- atmospheric gas mask
- meson/T-ray goggles
- **advanced fire extinguisher** (foam)
- extended-capacity emergency oxygen tank, mechanical toolbox, spare headset

**The atmos suit storage unit** holds the **atmospheric MODsuit**, an atmospheric gas mask and a backpack firefighter tank.
- The MODsuit is fireproof, heat immune and pressure-proof when sealed, so it's your space and vacuum suit.
- Its modules: storage, welding, radiation protection, flashlight, magboots, T-ray, quick carry, head protector, and a **MOD resin mister** (the same three modes as the firefighter tank's nozzle).
- It takes the back slot, so you can't wear it together with a firefighter tank.

## 4. How the air works (MetaStation's loop, as mapped)

**Supply.**
1. "N2 to Airmix" (on) and "O2 to Airmix" (on) feed the **air mixer**:
   - on, 4500 kPa;
   - Main Node = nitrogen from the west, **79%**;
   - Side Node = oxygen from the south, **21%**.
2. The mixer fills the Mixed Air chamber.
3. The air chamber's output feeds the **air supply line**, which feeds:
   - **"Air to Distro"**: on, **101 kPa** (the map leaves the default 101.325) → distro (blue pipes, layer 4): about 258 vents station-wide.
   - "Air to External Air Ports" (on).
   - The two portable-pump ports in Atmospherics.
   - "Air to Ports", "Air to Mix" and "Air to Pure" (all off).

**Waste.**
1. About 210 scrubbers (red pipes, layer 2) feed the waste loop.
2. **"Waste to Filter"** (on) feeds the filter line.
3. The filters, all on, run in a row: nitrogen → oxygen → carbon dioxide → plasma → nitrous oxide. Each pulls its gas into its own chamber.
4. What's left goes to the Mix chamber through "Unfiltered & Air to Mix" (on).

**Off by default** (leave them off unless you mean it):
- "Distro to Waste"
- "Distro Staging to Distro"
- "Mix to Distro Staging"
- "Mix Outlet Pump"
- every "X to Pure" pump (N2, O2, Air, CO2, Plasma, N2O)
- "Mix to Engine"
- "Fuel Pipe to Incinerator"
- the two digital valves named "Waste Release", which dump waste to space through passive vents

**The chamber computers** (AtmosControlConsole): `toggle_input`/`toggle_output {chamber}`, `adjust_input`/`adjust_output {chamber, rate}`. Their inlets and outlets start on, except the Mix chamber's output; leave them.

**Distro has connector ports in maintenance and the Locker Room** (layer 4). A canister wrenched onto one feeds the whole station: this is how plasma gets into distro.

**Pumps** (window "AtmosPump"):
- Actions: `power`; `pressure` with `{pressure: <kPa>}` or `{pressure: "max"}` (4500).
- Shortcuts: ctrl-click turns a pump on or off; alt-click sets it to max. Pumps, mixers and filters can't be unwrenched while on.
- Mixer ("AtmosMixer"): `power`, `pressure`, `node1`/`node2` with `{concentration: 0-100}`.
- Filter ("AtmosFilter"): `power`, `rate`, `toggle_filter`.

**Optional at shift start** (common practice; the wiki suggests ~800 kPa):
- Raise "Air to Distro" to a few hundred kPa (300-800). The vents still stop rooms at 101 kPa in normal modes, but refills get much faster and the air alarm's Refill mode can work.
- Don't max it: a contaminated distro at high pressure takes far longer to purge.
- Maxing "Waste to Filter" (alt-click) clears the waste loop faster.

## 5. Core procedures

### 5.1 Shift start

1. Load the map. `walk_to` Atmospherics Gas Storage. Read the **atmospheric alert console** and the **station atmospherics monitoring** console. Distro should read about 101 kPa of air, 21% O2.
2. In the Atmospherics Pumping Room, check that "Air to Distro" and "Waste to Filter" are on and "Distro to Waste" is off.
3. In Atmospherics, check:
   - the air mixer: on, Main 79 / Side 21;
   - "N2 to Airmix" and "O2 to Airmix": on;
   - the filters: on;
   - "Plasma to Pure", "N2O to Pure" and the Mix pumps: off.
4. Gear up from an atmos locker: RPD, holofan projector, backpack firefighter tank or advanced extinguisher, firesuit and firefighter helmet carried for later. Take 2 smart metal foam grenades from Gas Storage. Keep your analyzer handy.
5. Optionally wrench the two portable air pumps onto their ports in Atmospherics so they fill with air: mapped portables are **not** connected at round start. The engineers' two N2 canisters weren't either yesterday.
6. Announce on Engineering: "Atmos: distro and waste running, alarms clear."

### 5.2 Checking the air

- **Analyzer**:
  - Use it in hand (key Z) to analyze your own tile.
  - Click an adjacent canister, pipe, tank or tile with it in your active hand to analyze that.
  - Right-click in hand opens its gas analyzer window.
  - The chat report gives moles, each gas in mol and %, temperature, volume and pressure.
- **Normal air**: about 101 kPa, about 21% O2 / 79% N2, 20 °C (293 K).
- **Air alarm limits** (defaults):

| | Warning | Hazard |
|---|---|---|
| Pressure | ≤ 50 or ≥ 325 kPa | ≤ 20 or ≥ 550 kPa |
| Temperature | ≤ 280 K or ≥ 313 K | ≤ 270 K or ≥ 340 K |
| Oxygen (partial pressure) | ≤ 19 kPa | ≤ 16 kPa |
| CO2 | ≥ 5 kPa | ≥ 10 kPa |
| Plasma, N2O, tritium, BZ, other dangerous gases | ≥ 0.2 kPa | ≥ 0.5 kPa |

- **Atmospheric alert console** ("AtmosAlertConsole"): every station air alarm by area name, "priority" (hazard) or "minor" (warning). Its `clear` button is useless because it refills every tick; fix the room instead.
- **Station alert console** and the **PDA's Canary app**: Atmosphere, Fire and Power alarms by area.

### 5.3 Air alarms ("[area] Air Alarm", window "AirAlarm")

1. **Unlock** it with your ID card. Either right-click the alarm (`click {object_id, right: true}`) while wearing your ID, or click it with the ID in hand. While it's locked the window shows status only, and every action is ignored.
2. **Home screen buttons:**
   - "Area Atmosphere Alarm": action `alarm` / `reset`.
   - "Panic Siphon": toggles between Panic Siphon and Filtering.
   - "Vent Controls", "Scrubber Controls", "Operating Mode", "Alarm Thresholds".
   - These screens are display-only; send the actions directly.
3. **Modes**: action `mode` with `{mode: "/datum/air_alarm_mode/<name>"}`.

| Mode (path name) | What it does | Use |
|---|---|---|
| Filtering (`filtering`) | Vents release to 101 kPa; scrubbers take CO2 only, normal range. **Default.** | Normal; back to this after any fix. |
| Contaminated (`contaminated`) | Vents to 101 kPa; scrubbers take every gas except O2, N2 and pluoxium, expanded range. | Plasma/N2O/CO2 in a room with people. |
| Draught (`draught`) | Vents to 202 kPa; scrubbers siphon everything. | Slow air exchange. |
| Refill (`refill`) | Vents to 304 kPa; scrubbers CO2. | Fast refill. Needs distro above 101 kPa; switch back to Filtering near 100 kPa. |
| Cycle (`cycle`) | Vents off, scrubbers siphon until the room is below about 5 kPa, then Filtering. | Replace bad air in an empty room. |
| Siphon (`siphon`) | Vents off; scrubbers siphon, normal range. | Drain a room. |
| Panic Siphon (`panic_siphon`) | Vents off; scrubbers siphon, expanded range. | Drain a burning or flooded room fast. **Room must be empty.** |
| Off (`off`) | Vents and scrubbers off. | Stop feeding a breach until it's sealed. |

4. **Vents.** Actions take `ref` (the vent's refID from the window data):
   - `power {ref, val: 0/1}`
   - `direction {ref, val}`: 1 = Pressurizing, 0 = Siphoning
   - `excheck` / `incheck {ref, val}`: the Pressure Regulator, "External" / "Internal"
   - `set_external_pressure {ref, value}`, `reset_external_pressure`
   - `set_internal_pressure`, `reset_internal_pressure`
   - `overclock {ref}`: removes the pressure limit, but damages the fan
   
   A damaged vent ("Integrity" in the window) is repaired with a screwdriver, up to 10 s.
5. **Scrubbers:**
   - `power {ref, val}`
   - `scrubbing {ref, val}`: 1 Scrubbing, 0 Siphoning
   - `widenet {ref, val}`: Expanded range (also cleans the neighbouring tiles)
   - `toggle_filter {ref, val: "<gas id>"}`. Ids: `co2`, `plasma`, `n2o`, `water_vapor`, `tritium`, `bz`, `o2`, `n2`.
6. **Lock it again when done** (right-click it again).

### 5.4 Breaches (a room losing its air)

**Find it.**
- Signs: a "priority" alert on the atmos alert console; "Danger! Low pressure detected." on the room's air alarm; your own "Choking (No O2)", "Too Cold" or low-pressure alerts.
- Look for space tiles inside the room, broken windows, open external airlocks.

**Make yourself safe first.**
- **If you walk into a vacuum without a suit, back out immediately.** Yesterday's technician walked into one in Fore Port Maintenance.
- Suit up: atmospheric MODsuit sealed with internals on. Or, for a short job: firesuit plus atmospheric firefighter helmet (both pressure-proof, but cold-rated only to 60 K) with internals on.
- Warn the crew on Common: area, "no air, stay out".

**Stop the loss.**
1. Close doors around it; firelocks close by themselves on cold air.
2. Set the room's air alarm to **Off** so its vents stop pouring distro air into space.
3. Throw up **holofirelocks** as a stop-gap. The projector makes up to 6; click a tile with it in hand.
   - Each holds gas back but lets people and objects walk through.
   - It can be placed on doors, windows and grilles. Placed on a firelock's tile, it opens that firelock, so crew can pass while the gas stays put.
   - Using the projector in hand (Z) clears all its holograms.
   - Any hit destroys one.

**Seal it.**
- **Floor holes:**
  - A floor tile can go straight onto a space tile next to a floor.
  - Otherwise put rods first (lattice), then the tile.
  - Iron sheet in hand (Z) → crafting window "StackCrafting", action `make`: "floor tile", 4 per sheet.
- **Smart metal foam grenade:**
  - Prime it in hand (Z, 5 s), then throw it (key R, then click the spot).
  - It turns space tiles into foam plating and builds foamed-metal walls only where the room meets another area: doorways, holes to space.
  - **Throw it from well inside the room, not from a doorway.** Yesterday's technician stood on the edge and walled themselves in. Foamed metal breaks after a few hits with a crowbar or another tool.
- **Resin**, from the firefighter tank or the MOD mister:
  - Resin launcher mode: 100 water a shot, 10 s cooldown.
  - Resin foam mode: one adjacent tile at a time.
  - ATMOS Resin seals breaches, kills fire, deletes every gas except O2, N2, pluoxium and halon on its tiles, and sets them to 20 °C.
  - It is **dense** (blocks walking, breaks with one hit) and **welds shut every vent and scrubber on its tiles**. Unweld those afterwards with a lit welder.
- **Walls and windows**: ask a Station Engineer. If nobody is doing engineering repairs, plate the floor and keep the room holofanned and closed.

**Refill it.**
1. Check that the hole is closed (analyzer: pressure rising, not falling).
2. Set the air alarm to **Filtering**. Vents bring the room back to 101 kPa from distro, slowly if distro is at 101 kPa.
3. Faster:
   - **Refill** mode, after raising "Air to Distro"; back to Filtering near 100 kPa.
   - Or wheel in an **Air canister** from Gas Storage: release pressure about 101 kPa, open the valve, close it when the alarm clears. One full Air canister (about 4,560 kPa) holds roughly enough air for 35 tiles at normal pressure.
   - Or a filled portable air pump (window "PortablePump": `power`, `direction`, `pressure`) set to blow out at 101 kPa.
4. Report it fixed on Engineering and Common. Reset the fire alarm if it's still ringing (right-click it).

### 5.5 Fires

Fire needs fuel, oxygen and heat. Plasma burns in air above 100 °C (373 K). Fires spread at 150 °C and above. Firelocks close when the air next to them reaches 100 °C or drops to 270 K or below, and when anyone pulls the area's fire alarm. Fire alarms: click to trigger (closes all the area's firelocks); right-click to reset (firelocks reopen, and close again if it's still bad).

**Small fires** (a burning person, object or corner):
- Extinguisher in hand, Z to take the safety off, click toward the fire.
- Full-size extinguishers (100 water) are in wall cabinets: click the cabinet to take one. The advanced extinguisher (foam) is in your locker. Refill at a water tank by clicking it with the extinguisher.
- Spray burning people, or tell them to resist (stop, drop and roll).

**Room fires (usually plasma):**
1. Suit up: atmospheric firesuit plus firefighter helmet, or the atmos MODsuit, with internals on. Warn everyone away on Common.
2. Keep it closed. Firelocks will shut; don't crowbar them open toward the fire unless you're going in. Holofan the door you use.
3. **Get the fuel and oxygen out**:
   - At the room's air alarm, with the room empty of crew, set **Panic Siphon**. The burning gas goes into the waste loop, and the plasma ends up in the Plasma chamber.
   - Or go in with the firefighter tank in **resin launcher** mode and resin the burning area.
   - Extinguishers alone rarely stop a room of burning plasma.
4. Pull out anyone inside (drag them), give them to the Medical Doctors, and look for the cause (a leaking canister, a lit welder, an igniter). Close a leaking canister's valve; tell Security if it looks deliberate.
5. When it's out and cool: **Filtering** (or Cycle/Contaminated to clear the leftovers), then refill as in 5.4. Unweld any vents and scrubbers your resin sealed.

**Never "vent a fire to space"** by opening a door or airlock to space: you kill the room and anyone in it, and the hole is now yours to fix.

### 5.6 Gas leaks and contamination

- **Plasma, N2O or CO2 in a room**: set its air alarm to **Contaminated**. If the room is empty and the gas is heavy, use Cycle or Panic Siphon, then Filtering. Find the source: a canister with its valve open (close it: canister window, action `valve`), a broken pipe, someone with a tank.
- **Contaminated distro** (plasma or N2O coming out of vents everywhere):
  1. Turn **"Air to Distro" off** and **"Distro to Waste" on** to drain distro into the waste filters.
  2. Find the source. It's usually a canister wrenched onto a **distro connector port** (in maintenance and the Locker Room), or pumps switched on in Atmospherics: "Distro Staging to Distro", the Mix pumps, "X to Pure".
  3. Set affected rooms to Contaminated.
  4. When the monitoring console shows clean distro, "Distro to Waste" off, "Air to Distro" on.
  
  Report sabotage to Security.
- A **portable air scrubber** ("PortableScrubber": `power`, `toggle_filter`, `eject`) cleans a room with no working scrubbers. Empty it later through its connector port in Atmospherics; that port's volume pump feeds the waste filters.

### 5.7 Canisters

- **Move one**: pull it (ctrl-click), then walk.
- **Connect it to a port**: stand next to it, wrench in active hand, click the canister while it's on a connector port. "You fasten ... to the port"; window "Port: Connected". Click again with the wrench to unfasten. A connected canister is anchored. It shares gas with that pipe automatically; **its valve stays closed**.
- **Canister window** ("Canister"):
  - `valve`: "Open"/"Closed".
  - `pressure` with `{pressure: <kPa>}`, or `"reset"` (101), `"min"` (10), `"max"` (2533).
  - `eject`: the holding tank.
  - **An open valve with no tank inside releases the gas into the room** at the release pressure. That's how you refill a room with an Air canister, and how a plasma canister floods one.
- **Filling an internals tank**: click the canister with the tank to insert it, set release pressure, open the valve, close it, eject. Or take a full oxygen tank from the tank dispenser with a right click.
- Full canisters hold about 4,560 kPa. Cargo sells Nitrogen, Oxygen, CO2, N2O, BZ and Water Vapor canisters. Dangerous ones need atmos access to order.

### 5.8 Supporting the Supermatter engine

The engine is the Station Engineers' job (engineering's guide). What you supply is **nitrogen**, the coolant.
- In the **Supermatter Engine Room**, west side, two Nitrogen canisters sit on the ports of the two **"External Gas to Loop"** pumps. They start **unconnected**: wrench them to their ports.
- Spare nitrogen: the 3 Nitrogen canisters in Atmospherics Gas Storage. When an engineer asks:
  1. Pull one to the engine room.
  2. Wrench the empty one off its port and move it aside.
  3. Push the full one onto the port and wrench it on.
  4. Tell the engineer. They run the "External Gas to Loop" pumps.
  
  Never open a connected canister's valve: it dumps the nitrogen into the room.
- When the spares are gone, ask the Quartermaster to order "Nitrogen Canister" crates.
- There is also a pipe from Atmospherics' port-mix line into the loop: the **"Mix to Engine"** pump (east Atmospherics) to the **"Atmos to Loop"** pump (engine room), both off. That line carries Air or the Mix chamber's gas unless you set the pure-gas mixer up. Use it only if the engineer asks and you know what's in the line. Don't put air, plasma or anything but nitrogen into the engine loop on your own.
- Watch the engine from your PDA (**NT CIMS**). Report trouble on Engineering.

### 5.9 RPD basics

Use it in hand (Z) to open "RapidPipeDispenser".
- Actions:
  - `category`: 0 Atmospherics, 1 Disposals, 2 Transit Tubes.
  - `pipe_type {category: "Pipes", pipe_type: 1}`: a plain pipe (indexes start at 1).
  - `pipe_layers {pipe_layers: <bitmask>}`.
  - `color {paint_color: "blue"}`.
  - `mode {mode: n}`: toggles Build/Wrench/Destroy/Reprogram; all are on by default.
- Click a tile to lay the selected pipe already wrenched. Click a loose pipe to eat it.
- Match what you repair: **distro = blue, layer 4; waste = red ("scrubbers"), layer 2**. The RPD defaults to green, layer 3, which connects to neither.
- It sparks when you change settings: never use it near plasma.
- Don't unwrench pressurized pipes with a wrench: the gas escapes and can throw you.

## 6. Dangers and common mistakes

- **Vacuum**: below 20 kPa you take damage that grows the longer you stay. Space itself is about 2.7 K. **Never open a door or airlock that leads to space**, and don't open a door between a vacuum and an aired room: the air rushes out, and the alarms on the far side trip. Yesterday a door held open by a pulled canister did exactly that to the Storage Wing.
- **Plasma**: toxic to breathe above 0.05 kPa. It burns hot with any oxygen and a spark: welders (a lit welder is a spark), igniters, lighters, the RPD's sparks. Never open a plasma canister's valve into a room. The tank dispenser's **plain click hands you a plasma tank**: never put it on internals.
- **N2O**: above 1 kPa you start passing out; above 5 kPa you sleep. Only release it into a room on purpose; it hits everyone there, you included.
- **CO2**: above 10 kPa it suffocates (oxygen damage).
- **Mixing gases**: don't feed anything but N2+O2 air into distro or the engine loop. Keep the "X to Pure" pumps, the Mix outlets and "Distro Staging to Distro" off unless you know the whole path.
- **Foam**: smart foam walls form on area borders, so you can wall yourself in (yesterday). Resin walls block walking and weld vents and scrubbers shut.
- **Your active hand's item**: a click uses whatever you hold. Yesterday a click on the atmos alert console with a wrench in hand hit it ("You pulverise..."). A wrench on a pump tries to unwrench it, and a wrench on a connected canister disconnects it. Empty your active hand (key X to swap hands) before clicking consoles, alarms and machines.
- **Clearing alarm entries** on the alert console does nothing; leaving a sealed pocket airless keeps it a priority alert. Yesterday's sealed maintenance room stayed on the console all shift. Refill what you seal, or report why you left it.
- **Leftovers**: yesterday a borrowed welder and an air canister were left behind. Return canisters and tools.

## 7. Emergencies

- **Power failure**: pumps, mixers, filters, air alarms and vents need power. Without it distro stops and the station slowly goes stale. Tell the Station Engineers the Atmospherics, Atmospherics Pumping Room and Atmospherics Gas Storage APCs come first. Rooms keep their air for a long time; don't panic-refill.
- **Breach**: 5.4. If several rooms go at once (meteors, a bomb), protect the busiest first: Medbay, the Bridge, hallways, the Departure Lounge.
- **Fire**: 5.5.
- **Mass casualty**: keep air in Medbay and the hallways. Hand spare oxygen tanks (tank dispenser, right click) and breath masks to anyone without. Move the wounded out of bad air and send them to the doctors.
- **An attacker in or near Atmospherics**: see 8. Report it on Common with location and description.
- **Evacuation**:
  - Keep the route and the **Departure Lounge** breathable. Its air alarm is on the north wall by the emergency and fire-safety closets.
  - Check the lounge on the alert console. If it or the hallways to it are breached or hot, seal and refill them first, or holofan the doorway so the crew can walk through.
  - Bring an Air canister or a filled portable air pump if needed.
  - Hand out oxygen tanks to people in bad air.
  - Board with the crew when the shuttle comes.

## 8. Defending yourself and your department

Shared combat mechanics (combat mode, shoving, grabbing, resisting) are in crew-basics. Your own means:
- **Fire extinguisher** (full-size, from any wall cabinet; bulky): force 13, thrown 13.
  - In combat mode with the safety on, its right click on a person (`click {..., right: true}`) is a 2-second wind-up head bash for 39 brute with a severe wound. It only lands if they stay next to you for the whole 2 seconds.
  - The advanced extinguisher does force 10 and has no bash; the pocket one does 3.
- **Fire axe**:
  - Two are on the station: on the west wall in Atmospherics, and one on the Bridge.
  - Force 5 in one hand, **24 wielded** (use it in hand, Z, to wield).
  - Wielded, it pries open unpowered airlocks.
  - To open the cabinet, use a multitool on it (2 s) to unlock, then click to open, then click to take. Or break the glass.
  - Traitors may come to steal the Atmospherics fire axe; keep the cabinet locked.
- **Lit welding tool**: force 15 burn. **RPD**: force 10. Wrench and crowbar: force 5.
- **Armor**: the atmospheric firesuit and firefighter helmet make you fire immune. The atmos MODsuit adds light melee armor (10), bio 100 and fire 100. Fighting near fire is in your favour; never start one.
- **Blocking a pursuer**:
  - Holofirelocks **don't** stop people; they only hold gas.
  - ATMOS Resin and foamed metal are dense and block a doorway for a few seconds (one hit breaks resin; foamed metal takes a few).
  - Closed firelocks stop anyone without a crowbar or fire axe, and your toolbelt's crowbar gets you through. Pulling a fire alarm closes every firelock in that area. Do this only to get away from an attack, and reset the alarm after.
- **The department**: the "Atmospherics Lockdown" button in Gas Storage closes the shutters over the desk and the main door. Don't let strangers into Atmospherics. If someone is turning valves or pumps, step away, report on Common and Engineering, then undo it. Don't use gas as a weapon: plasma or N2O hits the crew and you as well.

## 9. Working with the crew

- **Chief Engineer** (if on shift): your boss. Follow their orders on engine and atmos changes.
- **Station Engineers**: they run the engine and power and do structural repairs (walls, windows). You bring them nitrogen, seal and refill rooms after their repairs, and fight fires. Tell them which APCs Atmospherics needs.
- **Captain / Head of Personnel**: report major breaches, fires or sabotage. The HoP can add access if you need into a room.
- **Security Officers**: report sabotage (opened canisters, a plasma canister on a distro port, tampered pumps) and arsonists. Give them a description and the area.
- **Medical Doctors**: keep Medbay's air clean. Pull burned and suffocated crew out to them. Don't hand out N2O canisters.
- **Chemist / Scientist**: their labs leak and burn; answer their alarms first. Ordnance storage holds plasma canisters.
- **Quartermaster**: orders gas canisters (Nitrogen etc.) and can sell spare gas. Dangerous gas crates need atmos access.
- **Cook / Botanist / Janitor**: the kitchen cold room and hydroponics trip temperature and CO2 alarms.
- **The AI**: can open doors, watch cameras and **control air alarms remotely**. Ask it to set a far room to Off, Panic Siphon or Contaminated while you run there, or to bolt doors around a fire.

The crew list is not exhaustive: more players can join at any time, in any job.

## 10. Through the client

- **Tgui windows**: `tgui_window` lists the actions and their params. Air alarm, pump, mixer, filter, canister and console actions are the names in sections 4-5. Vents and scrubbers need the `ref` from the window's `vents[]` / `scrubbers[]` data. Air alarm modes take the path string.
- **Unlock first**: right-click the air alarm with your ID worn. A locked alarm silently ignores every `tgui_act`. Check `locked` in the window data.
- **Empty hand**: before clicking any console, alarm or machine, check `active_hand` in `status`, and swap hands (key X) to an empty one.
- **Shortcuts**: `click {object_id, ctrl: true}` turns a pump, mixer or filter on/off; `alt: true` maxes its pressure. On a canister, ctrl-click pulls instead.
- **Suit storage unit**: clicking it opens a radial menu: "open", then "mod" (or "suit", "helmet", "mask", "storage"). Take off your backpack before putting the MODsuit on your back.
  - Then right-click the HUD button "Deploy MODsuit" (deploys all parts) and right-click "Activate MODsuit" (skips the prompt).
  - Wait about 10 s for "The atmospheric MOD helmet hisses closed".
  - Put a tank in your suit storage and click "Set Internals".
- **Grenades**: `key Z` primes the grenade in your hand; `key R` and a click throw it.
- **Finding things**: `search` by name ("Air to Distro", "air mixer", "Atmospherics Air Alarm", "Nitrogen canister"). The alert console gives area names that `walk_to {area}` accepts.

## 11. Checklist

**Shift start**
1. Gas Storage: atmos alert console, station atmospherics monitoring (distro about 101 kPa, 21% O2).
2. Pumping Room: "Air to Distro" on (optionally 300-800 kPa), "Waste to Filter" on, "Distro to Waste" off.
3. Atmospherics: air mixer on, Main 79 / Side 21; "N2 to Airmix", "O2 to Airmix" on; filters on; Pure, Mix and Staging pumps off.
4. Locker: RPD, holofan, firefighter tank or advanced extinguisher; 2 foam grenades. Firesuit and helmet ready.
5. Report on Engineering.

**Ongoing loop**
1. Every few minutes: atmos alert console or Canary. Answer priority alerts first.
2. For each alert: analyze, fix (alarm mode, seal, refill, clean), report it fixed, set the alarm back to Filtering and lock it.
3. Recheck the distro and air mixer settings now and then, and after any stranger visits Atmospherics.
4. Answer engineers' coolant requests: Nitrogen canisters from Gas Storage, wrenched onto the engine room ports.
5. Before the shuttle: Departure Lounge and the hallways to it breathable.

## 12. Sources

- Code (tgstation 54c22023): job and ID trim (`code/modules/jobs/job_types/atmospheric_technician.dm`, `code/datums/id_trim/jobs.dm`); atmos lockers (`closets/secure/engineering.dm`); `code/modules/atmospherics/` (air alarm, pumps, mixer, filter, canisters, vents, scrubbers); alert/monitoring consoles (`code/game/machinery/computer/`); holofan, firefighter tank, extinguisher, RPD, analyzer, foam, fire alarm, firelock, atmos MODsuit, lungs; tgui `AirAlarm/`, `common/AtmosControls.tsx`, `AtmosPump`, `AtmosMixer`, `Canister`, `RapidPipeDispenser`.
- Map: `_maps/map_files/MetaStation/MetaStation.dmm` (machine names and pipe networks traced from the file).
- Wiki (CC BY-SA 3.0, Internet Archive captures): Atmospheric_Technician, Guide_to_Atmospherics, Air_Alarm, Guide_to_the_Supermatter.
- Yesterday's round: `runs/12-atmos/report.md`, `runs/12-engineer/report.md`.
