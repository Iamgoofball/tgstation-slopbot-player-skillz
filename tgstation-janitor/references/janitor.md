# Janitor guide (MetaStation)

## 1. The job

You keep the station's floors safe and its lights working. Clean up what makes people fall (pools of oil, soap,
banana peels, spills) and what makes the place grim (blood, vomit, trash, broken glass). Replace broken lights. Clear
trash into disposal units. Return things people lose. Clean up after fights and in medbay once the doctors are done.
Success: nobody gets hurt on a floor you could have cleaned, every dangerous mess you hear about is gone within
minutes, and the lights work. Your boss is the Head of Personnel (head of Service). If more janitors join, split the
station between you (one fore, one aft) instead of following each other.

## 2. Starting kit and access

| Slot | Item |
|---|---|
| Uniform | janitor's jumpsuit |
| Belt | janitor PDA (programs: Custodial Locator, skill tracker) |
| Ears | service radio headset: **common** (`;`) and **service** (`:v`) |
| ID | Janitor ID card |
| Shoes | black sneakers (swap for galoshes, below) |
| Backpack | survival box, **access key ring** |
| Implanted | two skillchips, already active: CL34NM4ST.R (cleanbots like you) and **T4RG3T.bin**: every item you throw at a disposal unit lands in it (others miss 1 in 4) |

**Access:** Custodial Closet (janitor), maintenance tunnels, mineral storeroom, Service (the "Service Hall" doors).
You **can't** open the Kitchen, Bar, Hydroponics, Medbay Central, Cargo Bay, Delivery Office, Science, Engineering
or Security doors. Ask the department, or ask the AI ("AI, open the Delivery Office door for the janitor").

**Access key ring** (in your backpack): a head of staff can lend it their whole department's access for **10
minutes**. They press **Grant Janitor Access** on a Keycard Authentication Device (one in each head's office, the
Bridge and the Captain's Quarters). Captain: Command. Head of Personnel: general areas. Quartermaster: Supply.
A Chief Medical Officer, Research Director, Chief Engineer or Head of Security, if one is on shift: their own
department. The ring beeps "Access granted to ... area." Then click a door in that department with the ring in hand:
3 s of fumbling, and it opens. It beeps again when the time runs out.

You start with 250 cr on your ID's account.

## 3. Where things are

**Custodial Closet** (area "Custodial Closet"): a small 4x4 room in **Greater Starboard Maintenance**, south-east
of Hydroponics and south of the Service Hallway. Its only door ("Custodial Closet", janitor access) is in its west
wall. The Incinerator is on the other side of its east wall. `walk_to {area: "Custodial Closet"}` gets you there
through the Service Hallway and the maintenance doors (Service access opens them). The usual way in from the
Central Primary Hallway is the west "Service Hall" door. Janitors who start with the round appear in the closet.

Inside, by position:
- North wall, west to east: a **disposal unit** (north-west corner); a table with 2 boxes of **mousetraps** and 2
  **cleaner grenades**; a table with 2 **boxes of replacement lights** (14 tubes + 7 bulbs each), a **space
  cleaner** spray bottle and a third cleaner grenade; the **JaniDrobe** vending machine (north-east corner). There
  is a Requests Console on the north wall.
- West side: a **bucket** by the door; 2 **bear traps** on the floor in the south-west corner (see Dangers).
- Middle: a stool; **Wags-His-Tail**, the department's pet lizard (leave him be).
- East wall: a closet with a janitor's bio suit, hood, breath mask and oxygen tank (for a biohazard), with **orange
  gloves** on top; below it the **sink**, with the **mop** on the sink's tile.
- South wall, west to east: the **janicart (pimpin' ride)** with its **key** (a "key") beside it, the
  **janitorial cart**, the **water tank** (1000 u of water), a water vapor canister.

**The JaniDrobe** sells (you pay a fifth of the price, so about **10 cr** each; galoshes about 30, the backpack
cleaner tank about 50): galoshes, janibelt, backpack cleaner tank, flashlight, push broom, paint remover,
flyswatter, wet floor sign (6), holographic sign projector, **light replacer**, **soap** (Nanotrasen brand), trash bag,
plunger, wire brush, black gloves, clothes, a spare service headset. The closet has **no light replacer, no
galoshes, no soap and no trash bag** until you buy them.

**Spares:** a mop and mop bucket in the "Cleaning Closet" (Lesser Starboard Maintenance, just west of yours), in
Aft Starboard Maintenance and in Fore Starboard Maintenance. Boxes of replacement lights: the Service Hallway (a rack),
Primary Tool Storage, Auxiliary Tool Storage.

**Public sinks** to rewet a mop when the cart is empty or out of reach (the cart is better): Restrooms, Auxiliary
Restrooms, Cafeteria, Recreation Area.

**Cleanbots:** one patrols from the Central Primary Hallway, another starts in Medbay Storage. They clean as they go.

## 4. How your tools work

### The mop and wet floors
- The **mop** holds 15 u. It must be wet: a dry mop only says "mop is dry!".
- **Wet it:** with the mop in hand, **right-click** the janitorial cart or a mop bucket. That soaks it full
  ("doused mop"). A **left-click on the janitorial cart puts the mop into the cart** instead. Left-click a sink with
  the mop: +5 u ("You wet the mop in the sink."). Click a bucket you're carrying with the mop: +5 u. Right-click a
  sink with the mop to wring it out.
- **Mop a tile:** click the floor tile with the wet mop. It takes **1.5 s**: don't move until it's done. It cleans
  the floor messes on that tile: blood, oil, vomit, dirt, footprints, crayon. **Cobwebs and rubble** don't come off
  with the floor: click the cobweb itself with the mop or soap. A mop uses 1 u per tile, so a full mop does about 15
  tiles. You get faster with practice.
- **Mopping with water leaves the tile wet and slippery.** A tile mopped once stays wet for about 15 s at room
  temperature. Each extra pass on a tile that's still wet adds about a minute, up to 5 minutes. Cold rooms dry
  slower. **Below 0 °C the water freezes into ice**, which stays as long as the room is cold, slides people and
  ignores galoshes. Never mop the Kitchen Cold Room (-14 °C), or a room cooling after a breach.
- **Wet floor:** anyone **running** onto it falls for 6 s. People **walking** don't slip on water, and galoshes stop
  it completely.
- **A mop that holds space cleaner instead of water cleans without wetting.** Put space cleaner from the Chemist
  into an **empty** cart or bucket (no water mixed in) and your floors stay dry.
- A wet mop cleans **whatever you left-click** with it: a table, a crewmate (even in combat mode) and, out of combat
  mode, your own backpack. Yesterday a janitor started mopping their backpack. Keep the mop in one hand or in the cart.

### The janitorial cart, the bucket and the water tank
- The **janitorial cart** holds **250 u** of liquid and starts **empty**. It also carries one mop, one push broom,
  one trash bag, one space cleaner spray, one light replacer and up to 4 wet floor signs: left-click it with any of
  those to stow it.
- Empty-handed **left-click**: a radial menu (Trash bag, Mop, Broom, Spray bottle, Light replacer, Sign) to take one
  out. Empty-handed **right-click**: take the mop straight out. **Right-click** it holding any small item to drop that
  item into the cart's trash bag.
- **Fill the cart:** pick up the bucket (70 u). Use it in hand to change how much it pours: each use steps 5, 10,
  15, 20, 25, 30, 50, 70 u (it starts at 20). Set it to 70. Click the water tank with it ("You fill bucket with 70
  units..."), then click the cart ("You transfer 70 units..."). Three or four loads fill the cart.
- The cart is dense: walk into it to push it, or pull it (ctrl-click; `key h` lets go). **Take it with you when you
  clean**: pull it behind you, park it in the doorway or beside the mess, and rewet the mop from it as you go. It's
  slower through doors and crowds, but it carries your water, mop, broom, signs and trash bag, so you never walk back
  for any of them. Sinks are the fallback, for when the cart is empty or out of reach. Examine it to see its water
  level, and refill it at the closet's water tank.

### Space cleaner spray
- 100 u of space cleaner, 2 u per spray. Click a tile up to 3 tiles away: the puff cleans the blood, oil, vomit,
  dirt and footprints on every tile it crosses. It **doesn't wet the floor**. Use in hand to switch between spray
  (3 tiles) and stream (1 tile).
- It doesn't remove cobwebs (use the mop or soap). Spraying a person washes the blood off them and their clothes.
- **Refill:** the Chemist makes space cleaner from ammonia and water, 1 part each (1 + 1 → 2 u). Or buy the backpack
  cleaner tank (500 u, with a nozzle; it takes your backpack slot). The spray clicked on the cart goes into the cart;
  it doesn't refill there.

### Soap
- **Soap** (the JaniDrobe's Nanotrasen bar): click a tile, thing or person to scrub it clean in 2.8 s, 300 uses. It cleans
  everything the mop does, with no water and **no wet floor**. It's ideal for medbay.
- **Soap is slippery:** anyone stepping on it falls for 8 s, **even walking**. Galoshes protect you. Never leave it
  on a floor by accident. The client's `walk_to` steers around soap.

### Galoshes
- Yellow rubber boots (JaniDrobe). With them on you **never slip on water, soap, oil or banana peels**. They don't
  help on **space lube** or **ice**. They slow you down a little. Wear them all shift: put them on your feet, and
  stow or drop the sneakers.

### Light replacer
- Starts with **10 lights**, holds up to 20. Examine it, or use it in hand when not under a fixture, to see the count
  ("[n] lights, x/4 fragments").
- **Load it:** hold a box of replacement lights in your active hand and click the replacer. It takes every light it
  has room for. Other loads: a light tube or bulb (+1), a **glass sheet (+5)**, and broken lights or plain glass
  shards (1 fragment each; 4 fragments make 1 light). Clicking a glass shard on the floor with the replacer picks it
  up.
- **Replace a light:** stand next to a broken, burnt-out or empty fixture and click it with the replacer, or stand
  on the tile under it and use the replacer in hand. The broken tube goes into the replacer as a fragment. It fits
  tubes and bulbs alike. A working fixture answers "light already installed!".
- **By hand:** an empty-handed right-click on a fixture takes the tube out. If the light is **on**, that burns your
  hand (5 burn) unless your gloves resist heat (the black gloves from the JaniDrobe do, the orange ones don't). Click
  an empty fixture with the right kind of light to insert it. Never stick anything else in an empty socket: you can
  be shocked.
- **Dark isn't broken:** a fixture with no power just looks dark. Check the area's power before using up lights.

### Signs
- **Wet floor sign:** a small item. Drop it on or next to a tile you mop. The cart holds 4, the JaniDrobe has 6.
- **Holographic sign projector** (JaniDrobe): click a tile to project a wet-floor hologram, up to 10 at once. Use it
  in hand to clear them all. Put signs out whenever you leave a wet floor.

### Trash bag and disposals
- A **trash bag** holds 30 small or tiny items (wrappers, cans, cigarette butts, shards, bulbs). Click an item on the
  floor with it to scoop up everything small on that tile. Click a **disposal unit** with it to empty it there.
  Taking one item back out takes 1.5 s.
- **Disposal units:** clicking one with an item **puts that item in** (yesterday a doctor lost a medkit that way). An
  empty-handed click opens its window: Handle (flush), Eject (everything inside falls out), Power. A unit with
  anything inside flushes on its own about once a minute once its pressure is full.
- **Throw trash in:** with your T4RG3T.bin skillchip, a throw at a disposal unit always lands. Turn throw mode on
  (key `r`), then click the unit.
- The unit in **Virology** (the "deathsposal unit") **leads into space**. The one in the Aft Operating Room leads to
  the morgue.

### Custodial Locator (your PDA)
Tracks every mop, janitorial cart, key ring, janicart and cleanbot on the station: use it to find a stolen mop.
Open your PDA and run the program (`tgui_act PC_runprogram {name: "custodiallocator"}`). Press `scan` and choose
an entry with `selecttarget {ref}`; the list shows "Wet mop" or "Dry mop", and the cart's water level. The target
data: when the thing is within 24 tiles, it is (locx − 24) tiles east and (24 − locy) tiles north of you. Further
away you only get a bearing, `rot` (0 = north, 90 = east).

### Other kit
- **Cleaner grenades** (3 in the closet): foaming space cleaner for a whole room. Use it in hand to arm it (5 s
  fuse), then throw it. Expect some wet tiles afterwards.
- **Push broom** (JaniDrobe): use it in hand to hold it in both hands, then walk to sweep loose items ahead of you.
  Pushed into a disposal unit's tile, they go inside.
- **Plunger** (JaniDrobe): ends a vent clog (see Pests).
- **Mousetraps:** use one in hand to arm it, then drop it. It snaps whoever steps on it barefoot; shoes and gloves
  protect.
- **Janicart (pimpin' ride):** optional fast vehicle. Click it with its key, then drag yourself onto it.
- **Advanced mop:** the Scientist's techweb node Advanced Sanitation Technology, printed at the "Departmental
  Techfab - Service" in the Service Hallway. It refills itself with water, mops in 0.8 s and hits for 12.
- **Cargo crates** (the Quartermaster orders them, 400 cr each): Janitorial Supplies Crate (3 buckets, mop, broom,
  3 signs, trash bag, spray, 3 cleaner grenades), Replacement Lights (3 boxes).

## 5. What "mess" is

| Mess (in-game name) | Slippery? | Clean with |
|---|---|---|
| pool of oil (some mapped ones) | **Yes**: 8 s down and you **slide 4 tiles**; not if walking; galoshes protect | spray, mop, soap |
| motor oil from robots, vent clogs | no | spray, mop, soap |
| wet floor (water) | **Yes**, if running: 6 s down | wait, or put up signs |
| space lube (from the Clown, the Chemist, a scrubber overflow) | **Yes**: 8 s down, slide, confusion; **walking and galoshes don't help** | a Chemist's **drying agent**, or wait behind signs |
| ice (water below 0 °C) | **Yes**: slide; galoshes don't help | drying agent; warming the room |
| soap, banana peels, some foods | **Yes** | pick them up |
| pool of blood, blood trails, footprints, vomit, dirt, dust | no (blood dries in about 5 min) | spray, mop, soap |
| cobweb, rubble | no | click the cobweb or rubble itself with the mop or soap (the spray can't do it) |
| decomposing garbage | no | mop or soap only (the spray can't do it) |
| pool of fuel | no, but it burns | spray, mop, soap |
| shards (broken glass) | no; they cut people with bare feet | trash bag, or the light replacer |
| trash items | no | trash bag → disposal unit |

**Drying agent:** the Chemist makes it from stable plasma 2, ethanol 1 and sodium 1 (→ 3 u). Sprayed on a floor, it
dries water, lube and ice (each unit removes 10 s of wetness, so use plenty). The Atmospheric Technician's resin
foam also dries the floor it covers.

**Slippery oil at shift start** (pools of oil placed on the map): the **Delivery Office** (the worst one, see
below), the **Warehouse**, the **Research Division**, and two in **Fore Port Maintenance** near Waste Disposal.
Dirt is everywhere at shift start (most in the Service Hallway, Kitchen and Warehouse); cobwebs in maintenance.

## 6. Procedures

### Shift start (first 10 minutes)
1. If you aren't there yet: `walk_to {area: "Custodial Closet"}`.
2. At the JaniDrobe (north-east corner), buy **galoshes**, a **light replacer**, **soap**, a **trash
   bag**, a **holographic sign projector** and, if you like, black gloves and a flashlight. Put the galoshes on.
3. Load the light replacer from a box of replacement lights on the north table (box in hand, click the replacer).
   Put the box in your backpack for refills.
4. Take the space cleaner spray from the same table.
5. Fill the cart: bucket to 70 u, water tank, cart, two or three times. Pick up the mop (sink tile) and right-click
   the cart with it.
6. Stow the kit: spray and soap in your pockets, the rest in your backpack. Keep the mop in one hand and use the
   other for everything else (swap hands: `x`).
7. Announce on common, once: "Janitor on duty. Report spills, broken lights and messes to me on common or service."
8. **First job: the Delivery Office oil.** Ask the Quartermaster or the AI to open the **"Deliveries"** door (off the
   Cargo Bay; it needs supply access). The pool of oil is **2 tiles straight south of that door**. Below it is the
   row of delivery chutes. A running slip slides you 4 tiles south into the **"Service Deliveries" chute**, and you get
   flushed through the pipes. Yesterday that caught a cargo worker three times and a doctor once. Turn on walk mode and keep your galoshes on. From
   the doorway, spray toward the oil (it's within 3 tiles), then check it's gone. Tell common it's clean.
9. Clean the other slippery oil when you're nearby: the Warehouse (ask Cargo), the Research Division (ask Science),
   and the two in Fore Port Maintenance (you have access).

### Patrol loop (about every 15 minutes)
Messes collect where people eat, fight and bleed. Walk this loop with the cart in tow, cleaning as you go and
rewetting the mop from the cart (a public sink only when the cart is empty or you had to leave it behind):
1. **Service Hallway** (dirty from the start): the Kitchen and the Bar open off it. You can't enter them, so ask the
   Cook to let you in for the Kitchen floor.
2. **Bar Lounge** (public, north of the Kitchen and the Bar): the crew meeting is held here. Clean it after the
   meeting. The Bar itself needs bar access.
3. **Starboard Primary Hallway**, then west along the **Central Primary Hallway**.
4. **Cargo Lobby**, then the **Delivery Office** and the **Cargo Bay**, if the Quartermaster lets you in: trash and
   oil collect there.
5. **Port Primary Hallway** to the **Arrival Shuttle Hallway**: new arrivals, litter.
6. Back east, then south to the **Medbay Lobby** (public; the Medbay Central doors need medical access, so ask a
   doctor or the AI), then down the **Aft Primary Hallway** to the **Departure Lounge**.
7. Back north to the Service Hallway and the closet: refill the mop, empty the trash bag into the closet's disposal
   unit, top up the light replacer.

On every leg, `search` for "light fixture" and look for states ending in `-broken`, `-burned` or `-empty` (`tube-...`
for tubes, `bulb-...` for small lights). Five small lights start the shift broken: in the Warehouse and four
maintenance areas.

### Answering a spill or mess report
1. Get the place and what it is. Slippery messes (oil, lube, soap, banana peels, wet floors) come before anything
   cosmetic.
2. Go there with your galoshes on. Walk the last few tiles.
3. Put up a sign or hologram first if people are running through.
4. Clean it: spray for oil, blood and vomit (no wet floor); soap or a space-cleaner mop where people run; a water mop
   where it's quiet, with signs out.
5. Say it's done ("Common, Janitor: Delivery Office oil cleaned. Walk, floor's damp.").

### After a fight, and in medbay
- Wait until it's over and Security is done there. Then clean the blood pools, trails and footprints, sweep up glass
  and trash, and replace the broken lights. Bodies leave long blood trails on their way to medbay: follow them.
- Hand any weapons you find to Security and don't keep them. A dead or unconscious crewmate goes to the Medbay Lobby
  (pull them with ctrl-click). Never put a body in a disposal unit.
- **Medbay:** ask the doctors when you can clean. Use soap or the spray, so you don't leave a wet floor where people
  carry patients. Blood dries in about 5 minutes, then it's a "dried" stain; you can still clean it.

### Trash
- Scoop it up with the trash bag, empty the bag into any disposal unit, or throw single items straight into a unit.
- Don't throw away other people's things: tools, IDs, medkits, weapons, anything with a name on it. Those go to the
  lost-and-found.

### Pests
- **Mice:** 10 appear at round start in maintenance, on exposed cables. They **chew through cables**, cutting
  power. A mouse dies to any hit (5 health). Arm mousetraps from the closet boxes and drop them along maintenance
  cable runs. Tell the engineers where you find chewed cables.
- **Ventilation clog** (announcement: "Minor biological obstruction detected in the ventilation network. Blockage
  is believed to be in the [area]."): a vent there keeps spitting out cockroaches, mice, snails, butterflies or
  small spiders, with vomit, insect guts or motor oil. Examine the vents there; the clogged one says "Something's
  trying to get out." Click it with a **plunger** (JaniDrobe) and hold still 6 s: that ends the event. Then clean up.
- **Scrubber overflow** (announcement: "The scrubbers network is experiencing a backpressure surge..."): foam
  pours out of scrubbers across the station. It's mostly harmless, but it can carry water or **space lube**. Sign off
  lubed floors and get drying agent from the Chemist.

### Lost and found
- Your lost-and-found is the tables on the north wall of the **Custodial Closet**. Only janitor access opens that
  door, so people ask you on the radio and you bring things to them.
- Lost **ID cards** go to the Head of Personnel. The Captain's things (and anything from the Bridge) go to the
  Captain. Weapons, the nuclear authentication disk and anything stolen go to Security. Medkits and medicine go to
  medbay. Tools go to Engineering or a tool storage.
- Announce each item once on common: "Common, Janitor: found a toolbox in the Bar Lounge, it's in the custodial
  lost-and-found."
- To take an item off someone (the strip menu: drag them onto yourself), **both your hands must be empty**.

## 7. Dangers and common mistakes

- **Disposal units.** Yesterday the janitor was beaten into critical condition in the Medbay Lobby, shoved into the
  disposal unit there, flushed to the Delivery Office, and died. A single shove puts you inside a unit (knocked down)
  if it's right behind you. **In any confrontation, keep disposal units out from behind you.** If you're put in one,
  **move or resist (`b`) at once**: you climb straight out unless it has started flushing. Once in the pipes you
  can't get out, so wait until you're expelled at the far end. Never climb into one (dragging yourself onto it does
  that).
- **The Delivery Office oil.** See shift start. `walk_to` steers around soap, banana peels and wet floors, but **not
  around pools of oil**.
- **Your own wet floors.** Mopping with water where people run is how a janitor hurts the crew. Sign it, or use the
  spray or soap there.
- **Bear traps** (2 in the closet): an armed trap does 20 brute and locks the victim's legs. Leave them disarmed and
  out of walkways.
- **Theft:** yesterday two troublemakers stole the janitor's mop and traded it for favours. Use the Custodial Locator
  to find it. A spare mop is in the Lesser Starboard Maintenance "Cleaning Closet".
- **Cold rooms:** water there turns to permanent ice.

## 8. Emergencies

- **Power failure:** lights go dark but aren't broken; don't waste your replacer on them. Tell the engineers which
  areas are dark. Carry a flashlight.
- **Fire:** water puts out burning people and burning tiles. With a full bucket in hand and **combat mode on**,
  right-click a burning person or tile to splash it. Then get clear and let the Atmospheric Technician deal with the
  room. Don't mop near a fire you can't see the end of.
- **Breach:** stay out of the depressurised area and away from any door to space. Once it's repaired, sweep the glass
  and debris (the light replacer eats plain shards), replace the lights, and don't use water while the room is still
  cold.
- **Mass casualties:** help move the injured and the dead to the Medbay Lobby. Clean the trails and pools once
  medbay is past the rush. Keep the medbay floors dry.
- **Lube or ice on a main corridor:** signs or holograms across it, a common warning ("Lube in the Central Primary
  Hallway by the Bar, go around"), drying agent from the Chemist.
- **Evacuation:** when the shuttle is called, clean the **Departure Lounge** and the Aft Primary Hallway so nobody
  slips on the way. Board with your kit.

## 9. Defending yourself and your floors

Combat mode, shoves, grabs and breaking free are in `crew-basics.md`. Your personal file says how readily you fight.
What your kit adds:
- **Galoshes + slippery floors.** You can't slip on water, soap or oil; a chaser can. Before trouble comes, mop the
  tiles inside a doorway you might retreat through. Running chasers fall for 6 s; you walk on.
- **Soap** is the strongest trick: drop it (`q`) on your own tile as you go through a doorway or a 1-tile corridor,
  then keep going. Whoever steps there falls for 8 s, walking or not. Pick the soap up again afterwards.
- **A slipped attacker** is on the floor for several seconds: use them to get away, shout for Security on common
  with the name and place, or let Security cuff them. Downed people can still crawl and swing, so don't stand over
  them.
- **The mop as a weapon:** **right-click** a person with it to hit them (force 8; the advanced mop 12). A left-click
  only mops them, even in combat mode. Thrown, the mop does 10. The push broom does 8, or 12 held in both hands
  (left-click with combat mode on). The light replacer does 8.
- **The cart**, left in a doorway or a 1-tile corridor behind you, keeps the door open but makes a chaser push it
  aside: it slows them, it won't stop them.
- **Your closet:** its door opens only for janitor access (and the Captain's and HoP's). Retreat inside and ask the
  AI to bolt the door. Stay away from the closet's disposal unit while doing it.
- **Shoving into disposals** works on attackers too: shove one who has a unit right behind them and they drop inside.
  It's non-lethal and gets them out of the room. **Never with the Virology unit** (it leads into space), and never to
  someone already helpless.
- When they stop, flee or go down, you stop. Then report to Security.

## 10. Working with the crew

| Crew | You give them | You need from them |
|---|---|---|
| Everyone | Safe floors, working lights, lost items back | Reports of spills, broken lights, messes |
| Head of Personnel (your head) | A tidy Service department | Support; key ring access (general areas); lost IDs go to them |
| Captain | The Captain's lost things back | Key ring access (Command) in an emergency |
| Security Officers | Weapons and stolen goods you find; where fights left traces | Help with troublemakers; say when a scene can be cleaned |
| Medical Doctors | A clean, dry medbay; bodies brought to the Lobby | Medbay Central opened for you; a word when the blood can go |
| Chemist | Clean floors around Chemistry | Space cleaner refills (ammonia + water); drying agent |
| Station Engineers | Where lights are dark, cables are chewed, floors are wrecked | Power back; floor repairs |
| Atmospheric Technician | Spill and fire reports | Resin foam on bad wet floors; safe air after breaches |
| Scientist | Clean labs | Advanced Sanitation Technology: advanced mop, janicart upgrades |
| Quartermaster | A clean Cargo Bay and Delivery Office | The Delivery Office door; janitorial and light crates |
| Cook, Botanist | Clean Kitchen, Bar Lounge and Hydroponics floors | Being let in to clean; a heads-up on spills |
| The AI | Reports of what you cleaned | Doors (Delivery Office, Medbay Central, Kitchen); spill and broken-light reports from cameras |

The crew list isn't complete: more players can join at any time, in any job. If another janitor joins, share the
station. If a cyborg with a janitor module is on shift, it cleans as it moves, so leave it the hallways and take the
rooms. If nobody is doing a related job (no engineer for floors, no chemist for space cleaner), do what you safely
can and say what's missing.

## 11. Through the client

- **Mop a tile:** wet mop in the active hand, `click {x, y, turf: true}` on the floor. A plain tile click may hit an
  item lying there instead. Wait the 1.5 s before your next action.
- **Wet the mop:** `click {object_id: <cart>, right: true}`. The answer's floating text says "doused mop", "already
  soaked!" or "empty!". A plain left click stows the mop in the cart ("placed mop").
- **Walk mode:** `search {query: "run/walk", kind: "screen"}`, then click the "run/walk toggle". Turn it on near oil
  and on wet floors. Yesterday it fixed repeated oil slips.
- `walk_to` reports a slip ("You slipped on the pool of oil!") and stops. It steers around soap, banana peels, armed
  bear traps and wet, lubed or icy floors when it can, but **not around pools of oil**.
- **Using things in hand** (key `z`): the bucket's pour amount, arming a mousetrap or grenade, the light replacer
  under a fixture, clearing holograms, wielding the broom.
- **JaniDrobe:** its window lists products; buy with `tgui_act vend {ref, premium: false}`. You need your ID on you.
- **Disposal unit window** (DisposalUnit): `handle-1` flushes, `handle-0` unflushes, `eject` empties it. Get out of a
  unit you're inside with `move` (any direction) or `key b`.
- **Find broken lights:** `search {query: "light fixture"}` and read each fixture's state.
- **Radio:** `say {text, channel: "radio", radio: "service"}` for Service, `radio: "common"` for everyone.
- **Pulling** the cart or a body: `click {object_id, ctrl: true}`; `key h` stops pulling.

## 12. Checklist

**Shift start:** galoshes on · light replacer loaded · soap, trash bag, holosign projector bought · spray in hand ·
cart filled, mop wet · announce on common · Delivery Office oil cleaned (walk mode, from the door) · other slippery
oil noted.

**Loop:** patrol (Service Hallway → Bar Lounge → hallways → Cargo → Arrival Shuttle Hallway → Medbay Lobby →
Departure Lounge → closet) · slippery messes first · signs on every wet floor · lights fixed on the way · trash into
disposal units · lost items logged and returned · answer every report · clean after every fight and after the crew
meeting · keep disposal units out from behind you · refill the mop, spray and replacer at the closet.

## 13. Sources

- Code (tgstation 54c22023): `code/modules/jobs/job_types/janitor.dm`, `code/datums/id_trim/jobs.dm`, `mop.dm`,
  `datums/components/{cleaner,wet_floor,slippery}.dm`, `structures/janitor.dm` (cart, bucket), `other_reagents.dm`
  (water, space cleaner, drying agent), `decals/cleanable/`, `lightreplacer.dm`, `clown_items.dm` (soap),
  `holosign_creator.dm`, `vending/wardrobes.dm` (JaniDrobe), `recycling/disposal/bin.dm`, `janitor_key.dm`,
  `programs/radar.dm`, `events/{vent_clog,scrubber_overflow}.dm`, `turfs/open/_open.dm` (slips),
  `techweb/nodes/service_nodes.dm`, `cargo/packs/service.dm`.
- Map: `_maps/map_files/MetaStation/MetaStation.dmm` (closet contents, oil pools, doors and their access).
- tgui: `DisposalUnit.tsx`, `NtosRadar.tsx`, `KeycardAuth.jsx`, `Vending.tsx`.
- /tg/station wiki, "Janitor" (Internet Archive capture, Nov 2025), CC BY-SA 3.0. Where it disagrees with the code
  (it says the cart holds 100 u; the code says 250), the code is used.
- Yesterday's round: the janitor, cargo, doctor, chaplain and assistant reports.
