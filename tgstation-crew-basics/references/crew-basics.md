# Crew basics: life on Space Station 13 (tgstation, MetaStation)

What every crew member needs to know about the game, before the role guide. All of it was checked against the server's own code. Your role guide covers your job; this covers the station, talking, doors, health, fighting, hazards, death, and the everyday actions people fumbled last shift.

Who is on shift: the crew list you were given is not complete. More players can join at any time, in any job (a Head of Security, a Chief Engineer, cargo technicians, a bartender, assistants and so on). Treat everyone you meet as crew until they show otherwise.

---

## 1. The station and the shift

### Chain of command

| Rank | Who | Notes |
|---|---|---|
| Captain | Captain | Commands the station. Holds the nuclear authentication disk. Sets alert levels and calls the evacuation shuttle. |
| Heads of staff | Head of Personnel (HoP), Quartermaster (QM), and when on shift the Head of Security (HoS), Chief Engineer (CE), Chief Medical Officer (CMO), Research Director (RD) | Each head runs a department and has the Command radio channel. The HoP is second in command and runs Service. The QM is a head of staff in this version, on Command and Supply. |
| Crew | Everyone else | Answers to their department's head. If that head isn't on shift, they answer to the Captain (the HoP for Service). |
| The AI | Station AI | Follows its laws. It controls doors and cameras and hears every radio channel. It isn't in the chain of command, but it usually serves the crew and the Captain. |

If the Captain is missing or dead, the HoP (or another head) acts as Captain. Orders from a head to their own department are lawful. Orders from someone outside your chain are requests.

### Departments

| Department | Head | Staff (any may be on shift) | Radio key | Where (MetaStation) |
|---|---|---|---|---|
| Command | Captain | heads of staff | `:c` | Bridge, centre of the station |
| Security | HoS | Warden, Detective, Security Officers | `:s` | Brig and Security Office, north |
| Engineering | CE | Station Engineers, Atmospheric Technicians | `:e` | Engineering, north-east; Atmospherics, east |
| Medical | CMO | Medical Doctors, Paramedics, Chemists, Coroner | `:m` | Medbay, south-west |
| Science | RD | Scientists, Roboticists, Geneticists | `:n` | Research Division, south and south-east |
| Supply (Cargo) | QM | Cargo Technicians, Shaft Miners, Bitrunners | `:u` | Cargo Bay, north-west |
| Service | HoP | Cook, Botanist, Janitor, Bartender, Clown, Mime, Chaplain, Curator, Lawyer | `:v` | Bar, Kitchen and Hydroponics just east of centre; others spread around |
| Silicon | none | AI, cyborgs | `:b` (binary, silicons only) | AI Satellite, out in space to the east |

### Alert levels

The Captain or the AI sets green or blue at a communications console. Red needs two heads of staff swiping IDs at Keycard Authentication Devices. Delta means the station's destruction is imminent. Each change is announced station-wide.

| Level | Meaning for the crew (the game's announcement text) | Shuttle arrival after a call |
|---|---|---|
| Green | "All threats to the station have passed." Security keeps weapons holstered. | 20 min |
| Blue | "Reliable information about possible hostile activity." Security may show weapons; random searches are allowed. | 10 min |
| Red | "An immediate serious threat to the station." Weapons drawn, searches advised, some door access lifted (on MetaStation, the EVA Storage and Medbay Storage doors open for everyone). Escape pods can launch. | 5 min |
| Delta | "Destruction of the station is imminent." Obey heads of staff. | 2.5 min |

At red or delta: stay with others, keep your radio on, and do what the Captain and heads say.

### Evacuation: the emergency shuttle

No evacuation is scheduled. The Captain calls the shuttle only if the station can't go on (it's being destroyed, most of the crew is dead, or there is a threat nobody can stop), or late in a long shift. Don't ask for it as a routine. Don't call it yourself.

How a call works (from the code):
- **Calling.** Someone with Command access (normally the Captain) or the AI uses a communications console. A call needs a reason of at least 12 characters. The shuttle can't be called in the first 20 minutes of a round.
- **Announcements.** "The emergency shuttle has been called. It will arrive in N minutes." The time depends on the alert level when called (table above). A recall is possible only in the first half of the trip, and never at delta; it is announced too.
- **Docking.** The shuttle docks on the **south side of the Departure Lounge**, at the south end of the Aft Primary Hallway. The announcement says it "has docked with the station. You have 3 minutes to board the emergency shuttle." Board through the external airlocks on the Lounge's south wall.
- **Leaving.** After those 3 minutes it leaves, and it never waits. You count as evacuated only if you are **aboard (in the "Emergency Shuttle" area) when it leaves**. The flight to CentCom takes 2 minutes and the round ends when it arrives. Bring wounded crew aboard, and the dead if you can.
- **Before docking, those external airlocks open onto space.** Never open them until the docking announcement has come.

**Escape pods** dock at four places: the north end of the Arrival Shuttle Hallway, Security's Transfer Centre (north), the Recreation Area (north-east) and Engineering Maintenance (east). They launch only at red or delta alert; otherwise they leave together with the shuttle. Use one only if you can't reach the shuttle.

---

## 2. MetaStation overview

Orientation: north is "fore", south is "aft", west is "port", east is "starboard". Map y grows to the north. Area names below are exactly as the game names them; `walk_to {area}` takes them.

### The hallways (the public skeleton)

- **Arrival Shuttle Hallway**: far west. The arrival shuttle docks on its west side (that area is "Arrival Shuttle"), so new crew start here. Also customs and an escape pod.
- **Port Primary Hallway**: runs east from Arrivals to the centre. The Library is south of it; the Vacant Office and Auxiliary Restrooms open off it.
- **Central Primary Hallway**: a big ring around the Bridge in the middle of the station. Nearly every department opens off it.
- **Command Hallway**: inside the ring, along the Bridge's south side. Doors lead to the Bridge, Captain's Quarters, Head of Personnel's Office, EVA Storage, Teleporter Room and Gateway.
- **Fore Primary Hallway**: runs north from the ring to the Brig and Security.
- **Starboard Primary Hallway**: runs east from the ring to the Engineering Foyer. Technical Storage, Telecomms Storage and Auxiliary Tool Storage open off it, and the Bar Lounge borders it.
- **Aft Primary Hallway**: runs south from the ring, past the Medbay Lobby, Science Lobby, Mech Bay, Genetics Lab and Morgue, to the **Departure Lounge**.
- **Service Hallway**: a staff corridor behind the Kitchen, Bar Backroom and Hydroponics, south-east of the ring.

### Departments and key rooms

| Where | Areas (exact names) | How to get there |
|---|---|---|
| Centre | **Bridge** (comms console, crew monitor); **Captain's Quarters** (east of the Bridge); **Head of Personnel's Office** (west end; its desk window faces the Command Hallway); EVA Storage, Teleporter Room, Gateway, Corporate Showroom (south of the Command Hallway) | Through the Command Hallway; all need Command access. (The AI Upload Chamber is off the ring's north side, behind high-security doors.) |
| North | **Brig**, Security Office, Security Locker Room, Brig Control, Armory, Holding Cell, Interrogation Room, Prison Wing; Courtroom and Detective's Office near the Fore Primary Hallway | Fore Primary Hallway, then the "Brig" doors (Security access) |
| North-west | **Cargo Lobby** (public), Delivery Office (behind the "Cargo Desk"), **Cargo Bay**, Warehouse, Quartermaster's Office, Mining Office | Off the ring's north-west corner through the Storage Wing |
| North-east | **Locker Room** (public, via "Crew Quarters Access"), Dormitories, Restrooms, Garden, Law Office, Recreation Area, Fitness Room, Recreational Holodeck | North-east side of the ring |
| North-east | **Engineering** (main room, through the "Engine Room" door), **Supermatter Engine Room** and its crystal chamber "Supermatter Engine", Shared Engineering Storage, Chief Engineer's Office, Gravity Generator Room (further north) | Starboard Primary Hallway, then **Engineering Foyer** (Engineering access) |
| East | **Atmospherics**, Atmospherics Gas Storage, Incinerator | Through the Engineering Foyer |
| Far east, in space | AI Satellite (AI Chamber), **Telecomms Server Room** and Telecomms Control Room (the radio's machines) | The "MiniSat Access" Transit Tube from the Engineering Foyer |
| East of centre | **Bar Lounge** (public seating), **Bar** (behind the counter), Bar Backroom, **Kitchen** (south of the Bar Lounge; its back door and "Kitchen Window" open onto the Service Hallway), Kitchen Cold Room, **Theater**; **Hydroponics** further south (front door and desk on the ring, back door on the Service Hallway; Hydroponics access) | The Bar Lounge opens onto both the ring and the Starboard Primary Hallway |
| South-east | **Custodial Closet** | Only through Greater Starboard Maintenance (off the Service Hallway's east end and the Starboard Primary Hallway); Janitor access |
| South-west | **Medbay Lobby** (public); through the "Medbay Clinic" door, a small public part of **Medbay Central** with a first-aid kit on a table; staff only beyond: Medbay Treatment Center, Medbay Storage, Grand Surgery Theatre, Cryogenics, Chemistry, Pharmacy, Morgue, Virology, Paramedic Dispatch | South-west corner of the ring, where the Aft Primary Hallway starts |
| South | **Science Lobby** (public), Research and Development (desk onto the lobby), **Research Division** (behind "Research Division Access"), Robotics Lab, Mech Bay, Genetics Lab, Ordnance, Xenobiology Lab (far south-east) | South side of the ring, next to the Medbay Lobby |
| South | **Departure Lounge**; the **Chapel** (west of it, entered through the Lounge's "Chapel" door or from maintenance) with the Chapel Office and Chapel Funeral Room | End of the Aft Primary Hallway |
| Everywhere | Maintenance tunnels ("Central Maintenance", "Port Maintenance", "Fore Port Maintenance", "Greater Starboard Maintenance", "Aft Port Maintenance" and more), Waste Disposal | Doors with maintenance access; not every job has it |

### Public supplies

- **Food and drink:** a snack vendor (e.g. "Getmore Chocolate Corp") in the Central Primary Hallway, Departure Lounge, Library, Research Division and Medical Break Room; drinks vendors ("Robust Softdrinks" or a variant) in the Port Primary Hallway, Bar Lounge, Command Hallway, Cargo Lobby, Aft Primary Hallway, Recreation Area and Arrival Shuttle Hallway; coffee ("Solar's Best Hot Drinks") in many places. Vendors charge your ID's bank account. The Kitchen and Bar serve real food and drinks.
- **Emergency closets** ("emergency closet"): Arrival Shuttle Hallway (5), Central Primary Hallway (6), Port Primary Hallway, Departure Lounge, Recreation Area, Research Division and in maintenance. They hold breath masks and oxygen tanks, sometimes an emergency medkit, sometimes an emergency toolbox.
- **Fire-safety closets** ("fire-safety closet"): Central Primary Hallway (3), Arrival Shuttle Hallway, Port Primary Hallway, Departure Lounge, Recreation Area, Research Division, Engineering and in maintenance. Each holds a firefighter suit, gas mask, oxygen tank, fire extinguisher, red hard hat and an emergency crowbar.
- **Extinguisher cabinets** are on walls in every hallway and most rooms.
- **First-aid kits:** one in the public part of Medbay Central (on a table, past the Medbay Clinic door), one on the Bridge, more in Medbay Storage and Security Medical. This map has **no wall-mounted Emergency NanoMeds**. The NanoMed Plus vendor (gauze, sutures, ointment, analyzers) is inside medbay, behind staff doors. Ask a doctor.

---

## 3. Talking

### Speech

| What | How | Who hears |
|---|---|---|
| Say | plain text | everyone in view, about 7 tiles |
| Whisper | the whisper channel, or start with `#` | adjacent people clearly; a little further garbled |
| Emote | the `me` channel, text like "waves" | everyone who can see you |
| Radio | start with a key (below), or the say tool's radio option | everyone whose headset has that channel, station-wide |

Stay in character; don't use OOC.

### Radio keys

`;` = Common (everyone), `:h` = your headset's own department channel, `:c` Command, `:s` Security, `:e` Engineering, `:m` Medical, `:n` Science, `:u` Supply, `:v` Service, `:o` AI Private, `:b` binary (silicons only), `:i` the nearest wall intercom. `.` works in place of `:`.

A key for a channel your headset doesn't have sends nothing. Examine your headset to see its channels.

| Job | Headset | Channels besides Common |
|---|---|---|
| Captain | captain's bowman headset | Command and Security on; Engineering, Science, Medical, Supply and Service present but switched **off** at shift start (the Captain must switch them on in the headset's window) |
| Head of Personnel | head of personnel's headset | Command, Service |
| Quartermaster | quartermaster's headset | Command, Supply |
| Security Officer | security bowman headset | Security |
| Station Engineer, Atmospheric Technician | engineering radio headset | Engineering |
| Medical Doctor, Chemist | medical radio headset | Medical |
| Scientist | science radio headset | Science |
| Cook, Botanist, Janitor | service radio headset | Service |
| AI | built in | every channel, plus AI Private and binary |

### When the radio fails

- **Headsets need telecomms.** Headsets only send through the Telecomms machines on the satellite. If telecomms loses power or is damaged, no headset message goes anywhere, and you just whisper to whoever is next to you. Last shift the whole station's radio died for about 12 minutes while station power was down. The fix belongs to the engineers: power the station, then check telecomms.
- **Wall intercoms** ("station intercom") are made for this: "ready to spring into action even when the headsets go silent." Stand next to one and start your line with `:i`. Intercoms can still reach each other without telecomms (not headsets), if the room has power.
- **In critical condition the radio doesn't work at all.** The game drops the radio key and `;` in crit, and you can only whisper to adjacent people. Last shift a bartender in crit "radioed" for help and nobody heard. Call for help *before* you go down, and say where you are. `:i` next to an intercom still works in soft crit, but whispered and garbled.
- **Talking into a radio is also heard nearby.** People next to you hear you whisper the line. Don't radio secrets with a stranger at your elbow.

### Other channels

- **Poly the parrot** lives in the Chief Engineer's Office and wears an engineering headset. Poly repeats lines it heard, including radio lines from **earlier rounds**. A line from Poly about delamination or deaths is not news. Trust what you see.
- **PDA messages:** your PDA (on your belt, or in a pocket for engineers and atmos techs) has a "Direct Messenger" app for private text to a named crew member. It also goes through telecomms.
- **The AI hears every channel.** Say "AI, …" on the radio to ask it something.

---

## 4. Access and doors

- **Your ID card** (in your ID slot, often inside your PDA) carries your access. Doors and lockers check the ID in your ID slot or in your hands, not one in a pocket or bag. A denied door flashes and buzzes; it doesn't mean the door is broken.
- **Access depends on your job.** When few players are on at round start, the game gives every job some extra access. Most staff areas (medbay treatment, engineering, security, cargo back rooms, command) are closed to outsiders. Maintenance doors need maintenance access, which not every job has.
- **To get through a door you can't open:** ask on the radio ("AI, please open the Medbay Storage door"; the AI can open, close and bolt doors), or ask someone inside to open it. For a permanent change, ask the **Head of Personnel**, who changes access and jobs at the ID console in the HoP's office.
- **Firelocks** (thin emergency doors that drop in doorways) close when there's fire or bad air on one side. A bare-hand click only knocks. A crowbar forces one open; check first why it closed. **Emergency shutters and blast doors** are opened by buttons or by the AI.
- **Bolted doors** don't open for anyone until someone unbolts them. **Electrified doors** shock you when you touch them.
- Hacking doors (wires, multitool) and prying them is engineers' work, or a medbay break-in for urgent healing when nobody can let you in. Breaking into secure areas otherwise is a crime (see Space Law below).

---

## 5. Health

### Damage and thresholds

Health = 100 minus brute, burn, toxin and oxygen damage. Stamina, brain and organ damage are tracked separately.

| Damage | Comes from | Fixed by |
|---|---|---|
| Brute | blows, bullets, falls, crushing | sutures, bruise packs, brute patches (libital), surgery |
| Burn | fire, lasers, shocks, heat, cold | regenerative mesh, ointment, burn patches (aiuri) |
| Toxin | poisons, radiation, bad chemicals | the Chemist's antitoxins; a doctor |
| Oxygen (suffocation) | no air, bad air, crit, being strangled | breathing again: air, internals, CPR, epinephrine; it heals once you breathe |
| Stamina | shoves, failed grab escapes, batons, flashes | rest; when it fills (about 100) you collapse for a while (stamina crit) |
| Brain and organs | head trauma, decay after death, toxins | doctors (surgery, specific medicine) |

| Health | State | What it means |
|---|---|---|
| 100 to 1 | Alive | Heavy damage slows you. |
| 0 or below | **Soft crit** | You fall and can only crawl slowly. Your hands don't work. You can only whisper, and **your radio doesn't work**. You miss breaths, so oxygen damage climbs. |
| -30 or below | **Hard crit** | Unconscious and deaf, slowly dying. Whispering here becomes your "last words" and you die. |
| -100 or below | **Dead** | See section 8. |

In crit a "Succumb" alert appears. Clicking it kills you. Don't, unless you choose to die.

### Wounds and bleeding

Hits cause wounds on body parts: cuts (bleeding), punctures (bleeding), bone wounds (dislocations, fractures; limbs work badly) and burn wounds (can get infected). Bleeding drains your blood; low blood makes you faint and short of breath, and can kill. Medical gauze slows bleeding and splints bones; sutures close cuts; regenerative mesh dresses burns. A doctor treats the rest. Being dragged along the floor while bleeding loses extra blood. Click your own body with an empty hand (not in combat mode) to check yourself: it lists your injuries and bleeding.

### Treating yourself

Click yourself (or a patient) with the item. It treats the most damaged body part, then the next, until the job is done or the stack runs out. Applying it to yourself is slower than to someone else, and moving interrupts it.

| Item | Treats | Time on yourself |
|---|---|---|
| suture | brute (10 per use), slows bleeding | 3 s |
| regenerative mesh | burn (10 per use) | 3 s |
| bruise pack | brute | 4 s |
| ointment | burn (5 per use) | 4 s |
| medical gauze | bleeding, splints broken bones | 5 s |
| epinephrine medipen | stabilises someone in crit (stops the suffocation spiral); also slows bleeding, and delays decay of a dead body | instant injection |
| patches and pills | whatever the label says (the Chemist makes them) | click yourself with it |

A **first-aid kit** (regular medkit) holds 1 medical gauze, 2 sutures, 2 regenerative mesh, 1 epinephrine medipen and a simple health analyzer. Your backpack's **survival box** holds a breath mask, an emergency oxygen tank and an epinephrine medipen (some jobs' boxes add more).

Badly hurt: say so on the radio *with your location*, then go to the Medbay Lobby or wait for a doctor. The doctors' crew monitor shows you only if your suit sensors are on (below).

### Suit sensors (so medics can find you)

Your jumpsuit reports to medbay's crew monitor. At shift start it's set to a random mode: off, binary (alive/dead), vitals, or tracking. **Set it to tracking** so a medic sees your health *and your position*:
- **Ctrl-click your worn jumpsuit** (the uniform slot on your HUD). The game answers "set to tracking".
- Or use the verb **"Adjust Suit Sensors"** and pick "Tracking beacon" (the choices are "Off", "Binary vitals", "Exact vitals", "Tracking beacon").

Do it at shift start. Sensors with a "shorted out" warning can be fixed with cable.

### Hunger, cold, heat, air

- **Hunger:** you get hungry within the first half hour or so; eat a meal or two a shift (Kitchen, vendors). Starving makes you sluggish. There is no thirst in this version.
- **Temperature:** your body takes cold damage below about 270 K (-3 °C) and heat damage above about 340 K (67 °C). Alerts read "Too Cold"/"Too Hot". Leave the area; a fire suit or space suit protects.
- **Pressure:** below 50 kPa is a warning; below 20 kPa (near vacuum) damages you fast. Normal air is about 101 kPa. In space, or in a breached room, you take pressure, cold and suffocation damage together.
- **No air ("Choking (No O2)" alert): use internals.**
  1. Put on the **breath mask** (mask slot) from your survival box.
  2. Hold the **emergency oxygen tank** in a hand, belt, pocket or suit storage. It must be on you, not inside the backpack.
  3. Click the tank's **"Set Internals"** action button on your HUD. "You open … valve" means you're breathing from it. Click it again to close.
  4. Get out of the bad air. An emergency tank lasts a few minutes. A helmet that isn't airtight won't work ("You need a mask!").

---

## 6. Combat and self-defence

Your personal file says how readily you fight. This section gives the means. Defend yourself and others when you must; run when you can't win.

### The fight tool: let the client fight

For any fight, use the client's **`fight`** tool rather than clicking yourself: it closes in, turns combat mode on,
attacks with what your active hand holds at the game's pace (a punch with an empty hand), resists grabs, picks up a
weapon lying next to you, steps off a goliath's tentacles, backs off when badly hurt, and puts combat mode and your
hands back as they were. It answers within `max_s` (default 15 s, up to 60) with what happened: hits dealt and taken,
where everyone is, how it ended. One call fights a whole fight; clicking by hand is slower and easy to get wrong (a
click with combat mode off is a hug).
- `fight {target: <mob id>, goal: "kill"}`: vermin, fauna, a killer. `goal: "subdue"` stops when they're down (with
  handcuffs in hand it cuffs them; with a stun baton turned on, it stuns). `goal: "defend"` (the default) fights
  back until they stop or fall. `goal: "flee"` gets away from them (in the open someone as fast as you keeps up: then it hands back to you).
- No `target`: whoever attacks you. `target: {"search": "goliath"}` names one by what it is.
- Any other action stops it at once; looking, talking and waiting don't.
- **Set your stance once a shift**: `fight {stance: "fight back"}` (or `"get away"`). Then, when someone hits, shoves or
  grabs you while you wait or talk, the client answers at once (a few seconds, a few actions) instead of waiting for
  your next turn, and tells you what happened. Without it, you take every hit until you notice.

### Controls

| Action | Key | HUD button |
|---|---|---|
| Combat mode: toggle / on / off | `F` / `4` / `1` | "toggle combat mode" |
| Resist (grabs, cuffs, buckles, lockers, fire) | `B` | "resist" |
| Throw mode (next click throws your held item) | `R` (or hold Space) | "throw/catch" |
| Swap active hand | `X` | "swap hand" |
| Drop held item | `Q` | "drop" |
| Use held item in hand | `Z` | |
| Quick-equip held item to the best slot | `E` | |
| Put into / take from backpack, belt | `Shift+B`, `Shift+E` | |
| Give held item to someone adjacent | `G` | |
| Stop pulling | `H` | "stop pulling" |
| Lie down / get up | `U` | "rest" |
| Walk while held (run is the default) | hold `C` | "run/walk toggle" |
| Aim at a body part | numpad (8 head, 5 chest, 4/6 arms, 1/3 legs, 2 groin) | the target doll |

### What a click on a person does

| Click | Empty hand, combat mode off | Empty hand, combat mode on | Item in hand |
|---|---|---|---|
| Left | hug; pat on the head (head aimed); shake someone lying down to get them up; **CPR** on someone lying in crit or dead (heals 7 oxygen damage each round, repeats while they stay in crit) | **punch** (5-10 brute; can miss, never misses a just-shoved target); kicks someone lying down (7-15) | **uses the item on them**. Medical items heal, cuffs cuff, food feeds. Anything else (toolbox, wrench, crowbar, extinguisher) **hits them, whether or not combat mode is on** |
| Right | **shove** (same in either mode) | shove | the item's secondary use; with a tool or weapon this usually still attacks |

**Shove:** pushes the target one tile and staggers (slows) them. If they hit a wall, a table, another person or a machine, they're **knocked down** (2 s). Shove them again while they're down and dazed and you kick them onto their side (3 s paralysis). A shove that moves someone loosens any grab they had to a plain pull. Someone lying down drops the item in their hand when shoved. Shoving someone into a **disposal unit** puts them inside it; into an open locker, it shuts them in.

### Grabs

- **Ctrl-click** a person to pull them (a passive grab: you drag them along).
- Ctrl-click again: **aggressive grab** (instant). They can't move or use their hands until they break free.
- Again: **neck grab** (3 s; you must stand still).
- Again: **strangle** (3 s). They can't breathe and take oxygen damage.

**Escaping (resist, `B`):** a passive grab breaks at once. Each resist (one every 2 s) has these odds: aggressive 60%, neck 30%, strangle 20%, and lower if you're lying down. A failed try costs stamina. A third person shoving the grabber loosens the grip to a plain pull, and the victim can then break free with one resist. If someone grabs you aggressively, resist immediately and keep resisting, and shout for help on the radio *before* it reaches the neck.

### Restraints and traps

`B` works through these in order: a grab (if you aren't cuffed), then a buckle, then a container you're in, then fire, then cuffs.

| You are… | Resist (`B`) does | Time |
|---|---|---|
| handcuffed | removes the cuffs | 1 minute |
| in cable restraints / zipties | removes them | 30 s / 45 s |
| bola'd (legs) | removes it | 3.5 s (energy bola 6 s) |
| buckled to a chair or bed | unbuckles you (if cuffed, it takes as long as the cuffs' time first) | instant if not cuffed |
| in an unlocked locker or crate | opens it | instant |
| in a locked or welded locker | breaks out | 2 minutes |
| in a disposal unit | climbs out | instant, before it flushes |
| on fire | stop, drop and roll | a few seconds of rolling; repeat |

**Cuff removal fails if you move or are moved.** Being pulled, shoved or swapped interrupts it, and it can't finish while you're buckled. Last shift a cuffed officer never got free because people kept pulling him. Stand still in a quiet corner, or ask someone to take the cuffs off you (they drag you onto themselves and remove the cuffs in the strip menu).

### Common items as weapons

Higher is better. Fists do 5-10.

| Item | Force | Notes |
|---|---|---|
| fire axe (two-handed) | 24 | locked fire-axe cabinets on the Bridge and in Atmospherics |
| circular saw, butcher's cleaver | 15 | sharp |
| glass bottle | 15 | smashes on the target |
| welding tool, lit | 15 | burn damage; 3 when unlit |
| toolbox | 13 | throws hard too |
| fire extinguisher | 13 | in every hallway cabinet; `Z` toggles its safety, and with the safety off a click sprays toward the fire or a burning person |
| emergency or large crowbar | 12 | in every fire-safety closet |
| hatchet | 12 | sharp (Botany) |
| oxygen tank (full size) | 10 | |
| scalpel, kitchen knife | 10 | sharp |
| rolling pin, mop, chair, push broom | 8 | |
| red crowbar | 8 | |
| wirecutters, wrench, screwdriver, crowbar | 5-6 | |

**Throwing:** press `R`, then click where to throw. A thrown toolbox or extinguisher does 13. A thrown person (from an aggressive grab) knocks down whoever they hit.

**Flashes and pepper spray** are Security's tools (every officer carries a flash). A flash in someone's face knocks them down and drains their stamina. It works only if they're facing you, and sunglasses or welding gear block it. Ordinary crew rarely have either; don't count on them.

### Fleeing, and protecting others

- Run (the default). Put doors between you and the attacker: a door you have access to closes behind you and may stop someone without access. Head for crowded public places, and keep reporting on the radio: who, where, armed with what.
- **Protecting someone:** shove the attacker (it loosens their grip on the victim and, against a wall or table, knocks them down), then pull the victim away (ctrl-click them) toward medbay or Security. Call Security on `:s` if you have it, otherwise on Common, and ask the AI to bolt doors on the attacker's path.
- **Proportionality:** stop when the threat stops. Don't attack anyone who is cuffed, down, surrendering or fleeing. To disarm, shove them into a wall or table, shove again while they're down (they drop what they hold) and pick the weapon up; then hand them to Security. Killing is murder unless it was truly the only way to save a life.

### Space Law in brief (wiki guideline; Security enforces it)

- Crimes come in tiers: mischief (e.g. trespass, littering), misdemeanours (assault, petty theft, vandalism, breaking and entry, creating a workplace hazard), felonies (assault with a deadly weapon, theft of restricted items, sabotage, kidnapping, high-security trespass into Security, Command, the Engine Room or Atmos), grand felonies (attempted murder, grand theft such as stealing the Captain's ID) and capital crimes (murder, mutiny).
- **Self-defence** is "the protection of oneself, the protection of thy colleagues, and the protection of thine workplace", and it's a full excuse. Jumping into fights in another department isn't self-defence; that's vigilantism. "Unauthorized vigilante field executions are classed as Murder."
- Arrests and brigging are Security's job. Crew who stop an attacker hand them over to Security right away. If no Security is on shift, tell the Captain or HoP and keep the person restrained, unhurt, and with medical care if they need it.
- Captain, HoP and Security may carry weapons. Others carrying weapons outside their job is a crime, but your job's tools are fine.

---

## 7. Hazards

- **Slips.** You fall (knocked down) and may drop what you hold.
  - **Walking prevents slipping** on wet floors (fresh mopping, water) and on **motor oil** puddles. Last shift three people slipped on an oil puddle in the **Delivery Office**, fell into a disposal unit and were flushed through the pipes.
  - Walking does **not** help with banana peels, soap, lube or ice. Step around them.
  - More oil puddles start in the Warehouse, Fore Port Maintenance and the Research Division. Report a slick to the Janitor.
- **Disposal units** (the bins with a flush handle). Clicking one with an item in hand puts the item in: last shift a doctor binned their medkit this way. Anything inside is flushed automatically within about a minute, to Cargo's Delivery Office or Waste Disposal, and people get flushed too. To get your item back, click the unit with an empty hand and press **Eject** before it flushes. If you end up inside, move or resist at once.
- **The Supermatter crystal** (Supermatter Engine, inside the Supermatter Engine Room in Engineering): touching it, or anything bumping you into it, turns you to dust instantly. Being near an unstable crystal gives radiation and hallucinations. Stay out of the chamber unless you're an engineer working on it, and don't throw things at it.
- **Space and external airlocks.** Never open a door or airlock that leads to space. Breaches (holes to space) suck air out and pull loose things and people toward them. Leave the area, close doors behind you, and report it to Engineering and Atmos.
- **Fire and plasma.** Purple-tinted air or a "plasma" warning is toxic and burns. Fires spread through the air. Fire alarms and firelocks seal off the area: don't force firelocks into a burning room. If you're on fire, press `B` (stop, drop and roll) or get someone to use an extinguisher on you.
- **Electricity.** Electrified doors and grilles shock you; insulated gloves protect. Don't touch broken lights or open machine panels without engineering gear.
- **Conveyor belts** (Cargo, Waste Disposal) carry you along.
- **The gravity generator** (Gravity Generator Room): standing near it hurts ("Crushing Gravity"). Last shift an engineer lost half their health working beside it.
- **Hostile mobs, anomalies, random events.** When the game announces an anomaly or a hazard in an area, avoid that area unless your job is to handle it.

---

## 8. Death and revival

- **When you die**, you stay in your body as a dead mob. Your speech goes only to **deadchat**, which the living can't hear. The game tells you that you "can in most cases be revived by other players". Don't press **"Do Not Resuscitate"** (on the ghost HUD); it stops revival.
- **Ghosts:** the Ghost verb makes you a ghost that can only watch. Use **"Re-enter Corpse"** to go back, especially when someone is trying to revive you.
- **How revival works:** a doctor shocks the body with a **defibrillator**. It fails if the body has 180 or more brute or 180 or more burn damage (heal it first), or if the **heart has failed**. A dead body's heart decays and fails about **6 minutes after death** (slower in the cold; an epinephrine medipen's preservative slows it). After that the heart must be replaced or repaired in surgery. That's why last shift's defibrillations all ended in "heart too damaged". So:
  - If someone dies, call Medical **at once** with the exact location ("Medical, body in the Delivery Office").
  - Bring the body to the Medbay Lobby or Treatment Center, on a roller bed or by pulling it, without dragging a bleeding body farther than needed.
  - Inject an epinephrine medipen into the body if you have one.
- **If you're dead,** wait. Don't spam deadchat expecting the living to hear.

---

## 9. Everyday interactions (what people fumbled last shift)

### The rule that caused most accidents

**A click uses whatever is in your active hand on what you click.** With a wrench in hand, a click on a console hits it ("You pulverise the atmospheric alert console with the wrench") or unwrenches a canister. A medkit clicked on a disposal unit goes into the bin. A wet mop clicked on a backpack mops it. A crowbar clicked on a person attacks them, even with combat mode off. So:
- **Before clicking a machine, console, door button or person, empty your active hand or switch to an empty one** (`X` swaps hands). Put the item away first (`E`, `Shift+B`) or drop it (`Q`).
- Clicking the item in your own active hand **uses it in hand**. Some bags empty out onto the floor this way, so open bags as below instead.

### Items and storage

| To… | Do this |
|---|---|
| pick something up | click it with an empty active hand, standing next to it (a full hand picks up nothing) |
| equip / put away | `E` puts the held item in its best slot; click an empty inventory slot with the item; `Shift+B` puts it in the backpack, `Shift+E` the belt |
| open a bag | click it with an empty active hand while you wear it or hold it in your other hand; right-click opens one on the floor or a table |
| put an item in a bag or box | click the bag with the item |
| place on a table | click the table with the item; to take it back, click the item with an empty hand |
| put in a locker or crate | open it (empty-hand click), click it with the item (the item lands on its tile), then close it (empty-hand click); locked lockers need access |
| give to someone adjacent | with the item in your **active** hand, **ctrl-shift-click** them (offers it to them), or press `G` (offers it to everyone next to you). They take it by clicking the offer alert, and they need an empty hand ("You have no empty hands!" cancels it) |
| take from or put on someone | **drag them onto yourself** to open the strip menu, then pick a slot. It takes about 4 s per item. Your active hand must be empty (holding something, you try to put that item on them instead), and both of you must stay adjacent; if they step away, the menu goes view-only. They are warned ("You feel someone fumble with your belongings"). Use it to remove cuffs from a friend, not to rob |
| pull a crate, locker or body | ctrl-click it; `H` stops. A pulled crate is solid and can box you into a corridor or doorway: stop pulling before tight spots, and push it ahead instead |
| climb onto a table | drag yourself onto it (takes a moment) |

### Body actions

- **Buckled** (you arrive buckled to an arrival shuttle seat): click the **"Buckled" alert**, or press `B`. To sit down, drag yourself onto a chair.
- **Eat or drink:** hold the food or drink in your active hand and **click yourself**; repeat for more bites. Clicking someone else with food feeds them by force; ask first.
- **Read paper:** examine it; the paper window opens. To write on it, click it with a pen.
- **Check yourself:** click your own body with an empty hand, combat mode off.

### Through the client (the traps from last shift)

- **Check your hands before every click.** The answers' `active_hand` shows what you hold. If it isn't what you mean to use, swap (`key X`) or put it away first.
- **Right-click** is a real right-click in tgstation (`click {…, right: true}`): it shoves a person.
- **Combat mode** is `key F` (or `4` on, `1` off). Check the answer before you click a person: in combat mode an empty-hand click is a punch.
- **Offer and strip.** Offering is `click {object_id: <person>, ctrl: true, shift: true}` with the item in your active hand; `key G` offers to everyone adjacent. Stripping is `drag` of the person onto yourself, then `tgui_act` on the StripMenu slot, and it needs an empty active hand.
- **Walk mode stops slips.** `walk_to` avoids banana peels and soap but walked people straight over motor oil. Before crossing Cargo's Delivery Office, or any freshly mopped floor, switch to walk (click the HUD "run/walk toggle", or hold `C`).
- **Pulling.** `status` shows `pulling`, and walk answers show `came_along`. If `walk_to` says "no known path" or "blocked by mob" while you're pulling a crate, the crate is probably what's boxing you in: `key H` to let go.
- **Being moved.** If someone keeps shoving or pulling you, a "moved between calls" note appears, and cuff removal and other timed actions fail. Get clear first.
- **Radio failures.** If the radio answer says "no radio line of yours came back", the radio isn't working (telecomms down, or you're in crit). Use a wall intercom (`:i`) or go and talk in person.
- **The emergency shuttle isn't in the station map file.** Once it docks, `walk_to {area: "Departure Lounge"}`, then walk south through one of the Lounge's external airlocks.

---

## 10. Etiquette

- **Stay in character.** You are a crew member on a space station. Spectators are watching; make it a good shift.
- **Short radio lines:** who you are, where, what you need. For example: "Medical, Janitor here, hurt in the Bar Lounge, need a doctor." Use your department channel for department business and Common for the station.
- **Answer people** who talk to you or call your name or job on the radio, even if only to say no.
- **Coordinate:** say what you're starting and when you're done ("Kitchen open, steaks on the counter"). Ask the right department instead of doing their job badly. Report hazards, bodies, breaches and attackers at once, with locations.
- **Don't flood:** no repeated lines, no spam emotes, no long radio speeches. If chat is noisy, mute the noise rather than adding to it.
- **Respect people's departments.** Ask before taking things from other departments' rooms. Don't strip, hit or rob people for fun. Return what you borrow.
- **Never trust a single chat line.** People lie, Poly repeats old lines, and fake announcements happen. Trust what you see and what you can check.

---

## Sources

- tgstation source at the server's commit (54c22023): `code/__DEFINES/`, `code/modules/mob/` (speech, crit, grabs, shoves, resist, offers), `code/game/objects/items/devices/radio/`, `code/datums/keybinding/`, `code/game/objects/items/` (restraints, medical stacks, medkits, survival box, tools), `code/modules/clothing/under/_under.dm`, `code/controllers/subsystem/shuttle.dm`, `code/modules/shuttle/`, `code/modules/security_levels/`, `code/game/machinery/` (comms console, doors, firelocks), `code/modules/recycling/disposal/bin.dm`, `code/datums/components/{slippery,wet_floor}.dm`, `code/modules/jobs/job_types/`, `config/game_options.txt`; `_maps/map_files/MetaStation/MetaStation.dmm` with `code/game/area/areas/` (area names, positions, doors, vendors, closets).
- /tg/station wiki (CC BY-SA 3.0), Internet Archive captures: Space_Law (2025-12-30), Guide_to_combat (2026-02-09), MetaStation (2025-12-10).
- Last shift's crew reports (`/workspaces/seeker-play/play/crew/runs/12-*/report.md`).
