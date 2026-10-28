# Security Officer (MetaStation)

## 1. The job in one paragraph

You keep the crew alive and the station's property where it belongs. You patrol, answer calls on the security channel, stop crimes in progress, arrest with non-lethal tools, search and confiscate, hold prisoners in the brig for a sentence that fits Space Law, keep the security records up to date, and stand and fight when someone attacks the crew. Success is a shift in which killers and thieves end up cuffed in a cell or the Prison Wing, stolen high-value items (the nuclear authentication disk, the Captain's ID) go back to their owners, the officers stay alive, and nobody innocent is hurt by security. If another officer is on shift, pair up with them; if you're the only one, your backup is the AI (doors, cameras), the Captain, and crew who fight back. The crew listed for this shift is not everyone: more players can join at any time, in any job, including a Head of Security, a Warden, a Detective or more officers.

**Chain of command.** Captain > Head of Security (HoS) > Warden > Security Officer and Detective. Your job's supervisors are "the Head of Security, and the head of your assigned department". If a HoS is on shift, follow their orders. If a Warden is on shift, they run Brig Control, the armory, the cells and the records: bring prisoners to them and tell them the charges. **If no Warden or Head of Security is on shift, you run the brig yourself** (with any other officers) and answer to the Captain (then the Head of Personnel). A Detective does forensics: give them evidence. Lawyers may advise, but they have no authority over the brig, prisoners or sentences.

## 2. Starting kit and access

**Worn at spawn** (from the job's outfit in code):

| Slot | Item | Notes |
|---|---|---|
| Uniform | security uniform | 10 melee armor |
| Suit | armor vest | melee 35, bullet 30, laser 30, energy 40, **chest only** |
| Suit storage | **disabler** | in the vest's suit storage; Shift+Q draws it |
| Head | helmet | same armor as the vest; a seclite can be attached |
| Gloves | security gloves | **cuff 25% faster** (3 s instead of 4 s); not insulated |
| Shoes | jackboots | |
| Ears | security bowman headset | **protects your ears from flashbangs** |
| Belt | security PDA | has a view-only Security Records program |
| Left pocket | handcuffs | |
| Right pocket | flash | |
| Back | security backpack | survival box (security gas mask with hailer, emergency oxygen tank, epinephrine medipen) and an evidence bag |
| Implant | mindshield | you can't be converted or brainwashed |

You do **not** spawn with a stun baton or a security HUD. Both are in the lockers of the **Gear Room** (§3). Donuts heal security officers slowly (the sprinkles in them heal a little brute and burn damage).

**Radio.** The headset has the security channel, `:s`, plus common, `;`. A departmental officer's headset also has that department's channel: Medical `:m`, Engineering `:e`, Science `:n` or Supply `:u`. The AI hears every channel.

**Department assignment.** At round start, each officer is assigned to Engineering, Medical, Science or Supply (Cargo). Officers are grouped into departments in pairs where possible (a lone officer gets a department of their own). Chat says "You have been assigned to Medical!". Your ID's title becomes e.g. "Security Officer (Medical)", you get an armband, and at round start you spawn in that department's Security Post. If you join later, you arrive at Arrivals and the next free department is chosen for you. A department with exactly one officer gets the next one.

**Access** (code: `id_trim/job/security_officer`):
- Always: Security (security), Brig (brig), Brig Entrance (brig_entrance), Courtroom (court), Weapons permit (weapons), Security mech (mech_security), Mineral storeroom.
- If fewer than 20 players were ready at round start, you also get Maintenance tunnels, the Detective's office (detective) and the Morgue. The welcome text says "skeleton crew, additional access may have been added". If it says "full crew", you don't have these.
- Department bonus: Medical: medical and morgue. Engineering: engineering and atmospherics. Science: research and science. Supply: cargo, mining, shipping and the bitrunning den.
- **Not included:** the **Armory**, **Brig Control** (the Warden's office), the Bridge and other command rooms, the Captain's Quarters, and the Head of Security's Office. `walk_to`'s access_note warns you about these doors.

## 3. Where things are on MetaStation

North is up (y grows northward). The Security wing is in the north of the station. You enter it from the **Fore Primary Hallway**, north of the Central Primary Hallway, through two sets of "Brig" glass doors. The outer pair is fitted with a gun scanner gate; both pairs need brig_entrance access. `walk_to {area: "Brig"}`.

| Area (exact name) | What's there | Door access |
|---|---|---|
| **Brig** | The main corridor and the three cells. **Cell 1, Cell 2, Cell 3** are along the south-west side of the corridor. Each has a "cell door" (brig), a bed, a "Cell N locker" and a flasher. Each cell's **door timer**, a wall display named "Cell 1"/"Cell 2"/"Cell 3", hangs on the corridor side by its door. Also here: buttons for the "Brig Entrance Flasher" and the "Holding Cell Flasher" (security); a recharger near the Interrogation door; and, at the west end, the evidence and prisoner boxes, the labor camp consoles and the "Labor Camp Shuttle Airlock". Officer Beepsky (a securitron) patrols here. | brig_entrance from the hallway |
| **Holding Cell** | East of the brig entrance, through the "Holding Cell" windoor (security). Has a rack with 5 handcuffs and prisoner clothes, and two brig lockers. "Court Cell" doors (brig) lead to the Courtroom. No timer. | security |
| **Security Office** | North of the Brig corridor, through the "Security Office" doors. **Along its south wall, just inside:** the **security records console**, the **security camera console** and the **department techfab (Security)**. Also here: a rack with 3 handcuffs and radios, a recharger and a **pepper spray refiller** (east wall), the fax, Space Law books, and the "Interrogation Monitoring" door to the east. | security |
| **Security Locker Room** (doors named **"Gear Room"**) | Between the Brig corridor (south door) and the Security Office (east door). **Six "security officer's locker"s**, the **SecTech** vendor, the **SecDrobe**, 2 rechargers and a pepper spray refiller. To the north, "Secure Gear Storage" (armory access) holds firing pins, implants and spare handcuffs. | brig |
| **Armory** | West of the Gear Room, door "Armory" off the Brig corridor, plus the "Weapon Distribution" windoor. Racks of energy guns, laser guns, disablers, a shotgun, riot and bulletproof armor, helmets and shields, an ion rifle, a battle rifle, a temperature gun, a grenade launcher, and flashes and teargas boxes (some racks are random). Guarded by the securitron Sergeant-At-Armsky. | **armory (you don't have it)** |
| **Brig Control** | West of the brig entrance. Has the reception window to the hallway, the warden's locker, a security records console, a prisoner management console, a crew monitor, the cell-window, brig-lockdown and prison-wing lockdown buttons, and the buttons for the brig's interior and exterior doors. | armory (you don't have it) |
| **Interrogation Room** | East end of the corridor, door "Interrogation". Has tape recorders. | security |
| **Evidence Storage** | West part, door "Evidence Storage". Evidence closets 1-5 are unlocked; the "secure evidence closet" needs armory or detective access. | security |
| **Security Medical** | Far west of the Brig. Has a medkit, bandages, epinephrine, multiver, a health analyzer and a "DeForest first aid station" on the wall. | (inside the Brig) |
| **Prison Wing** (permabrig) | North-west, behind the "Prison Wing" doors (security) and the "Security Blast Door" prison gate. Includes Prison Wing Cells (doors also named Cell 1-4; these are not the timed brig cells), the Prison Mess Hall, Prison Garden, Prison Work Room, Prison Shower and Prison Visitation Area. The Transfer Centre (door "Permabrig Transfer", brig) holds orange prisoner uniforms, straight jackets, muzzles and blindfolds. | security / brig |
| **Firing Range**, **Security Mechbay** | North. The mechbay has the "Paddy" security mech (disabler arm, claw, prisoner cage; not tested through the client). | security |
| **Detective's Office** | East of the Holding Cell. | detective |
| **Courtroom** | Just south-east of the brig entrance, off the Fore Primary Hallway. | public / court |

**Security Posts** (the departmental offices). Each has a security records console, a recharger, a pepper spray refiller and a departmental "security officer's locker". **The departmental lockers have no security belt, so no stun baton.**
- **Security Post - Medbay**: between the Medbay Lobby and Medbay Central, door "Medbay Security Post". It has a "Medbay Doors Control" button (opens and closes the "Medbay" and "Medbay Clinic" doors), a "Privacy Shutters Control", a medical records console and a medbay camera screen.
- **Security Post - Engineering**: off the Engineering Foyer. It has the "Engineering Lockdown" and "Atmospherics Lockdown" buttons (they need engineering and atmospherics access, which an Engineering officer has), plus engine and minisat camera screens.
- **Security Post - Science**: in the Research Division, door "Security Office". It has a rack of handcuffs, a camera console and a mech console.
- **Security Post - Cargo Bay**: by the Cargo Lobby and Delivery Office. It has a camera console, a mining camera console and binoculars.
- **Customs**: at the Arrival Shuttle Hallway, door "Customs Desk". It has a records console, a camera console, an ID console, a locker, a flash and a crowbar.

**Hallways for patrols.** These are the area names `walk_to` accepts:
- Fore Primary Hallway: in front of the brig.
- Central Primary Hallway: the big loop around the Bridge, which also has the Command Hallway.
- Starboard Primary Hallway: east; Bar Lounge, Theater, Kitchen side, Engineering Foyer at its far end.
- Aft Primary Hallway: south; Science Lobby, Medbay Lobby, Departure Lounge at its far end.
- Port Primary Hallway: west; Library, Cargo Lobby, Arrival Shuttle Hallway beyond.

## 4. Core procedures

### 4.1 Gear up (shift start)
1. `walk_to {area: "Security Locker Room"}`. Click a **security officer's locker** once to unlock it (your ID has brig access), then again to open it. Each one holds: an armor vest, a helmet, a security radio headset, a security bowman headset, **security HUDSunglasses**, a seclite, enhanced retrieval gloves (tackling) and a **security belt**. The belt holds a **stun baton**, handcuffs, a pepperspray, a flash and a flashbang. Take one locker; leave the rest for other officers.
2. Wear the **security HUDSunglasses**. They give you the security HUD (criminal status on examine) **and flash protection** (a flash can't blind you).
3. Your belt slot holds the PDA. Put the PDA in your backpack, then wear the security belt. Shift+E draws from the belt or holsters into it.
4. Click your helmet with the seclite to attach it (it adds a light toggle). The seclite also works as a club (force 9).
5. Hold the stun baton and press `key Z` to turn it on ("turned on"). It doesn't drain while idle. Examine it to see its charge percentage.
6. Optional, from the **SecTech** (credits from your account, at a security discount): **zipties** (10, single-use, 45 s to break), handcuffs (8), flashes (5), **energy bolas** (7), seclites, evidence boxes, flashbangs (4), enhanced retrieval gloves, security holobarrier projectors; premium: security webbing (6 slots), energy holsters. **No stun batons.**
7. Say on `:s` who you are, your department, and where you'll be.

### 4.2 Non-lethal tools: how they work in this version
A person goes into **stamina crit** (floored, helpless) at **100 stamina damage**. Stamina damage resets to 0 **10 seconds after the last stamina hit**, so cuff within those 10 s. Each new hit restarts the clock, but after about three extra hits while they're down, further hits stop counting ("starts to recover from the exhaustion!").

| Tool | Use | Effect (code values) |
|---|---|---|
| **Stun baton** (must be ON) | Left click on the target, combat mode or not. Right click = "Harmful Stun" (also does 10 brute). | **60 stamina** at once, jitter, stutter, 10 s confusion. **2 s later the target collapses for 5 s** ("Your muscles seize"). **Two hits stamcrit an unarmored target.** 2.5 s cooldown, and you can't re-stun the same target for 2.5 s. A high-capacity cell gives **10 hits**; recharge it in a recharger. Energy armor on the chest reduces it: an armor vest takes it to 45 per hit. If OFF and you're not in combat mode, it only "prods" harmlessly. If OFF in combat mode, it hits for 10 brute. |
| **Disabler** | Hold it and click the target at any range in view. Right click within 2 tiles = **hold them at gunpoint**: if they move, attack or draw, you fire automatically. | **30 stamina per shot**, so **4 shots to stamcrit** an unarmored target. **20 shots** per charge. An armor vest (energy 40) takes it to 18 per shot on the chest only, so aim at the legs (target keys Numpad1 / Numpad3); the hit zone isn't guaranteed. Doesn't stamcrit cyborgs. |
| **Flash** (handheld) | Hold it and click an adjacent target. | Full effect only if they **face you**: knockdown 2.5-5 s plus **80-120 stamina** (often a stamcrit) and 5 s confusion. From the side, half. **From behind, nothing.** Sunglasses, security HUDSunglasses or welding gear block it. There is no cooldown, but each use within about 10 s of the last adds a 3% chance it **burns out** ("burnt-out flash"); spares are in the SecTech and the belts. `key Z` with it in hand flashes everyone within 3 tiles: confusion only, no knockdown. |
| **Pepperspray** | Hold it and click a target up to 4 tiles away. | Blind 6 s, **knockdown 3 s**, confusion 5 s, slowed 10 s. Only someone with **both eye and mouth protection** is immune. 50 units, 5 per spray, so 10 sprays. Click a pepper spray refiller with it to refill. |
| **Handcuffs** | Hold them and click the target. | **3 s** with your security gloves (4 s without). You both must stay put; if they walk off, it fails. Breaking out takes them **1 minute standing still**; zipties 45 s. |
| **Energy bola** | Throw it: `key R` (throw mode), then click them. | Snares their legs (slowed) until they spend 2 s breaking free. It can't be caught. Use it to close the distance, then baton them. |
| **Flashbang** | `key Z` to arm (5 s fuse), `key R`, click a tile. | Knocks down everyone in view within 7 tiles who lacks protection; the strongest effect is close in. Your bowman headset protects your ears, your HUDSunglasses your eyes. It hits allies too. |
| **Seclite** | | A light (range 5) and a weak club. |

**Best openers:** baton at melee range (one hit, then cuff when they fall 2 s later); disabler at range (4 hits); flash when they're facing you and wear no sunglasses. Then **cuff immediately**.

### 4.3 Arrest, step by step
1. **Identify.** `examine` the suspect. With the HUD on you see their criminal status and links. A name like "X (as Y)" means they wear someone else's ID; "Unknown" means a hidden face and no ID.
2. **Warn**, unless they're armed and attacking or caught mid-crime: `say` "Stop. You're under arrest for theft. Stay where you are." Say it on `:s` (another officer, the AI).
3. **Disable** them if they don't comply (§4.2).
4. **Cuff:** handcuffs in your active hand, click them, and wait the 3 s while you stay adjacent.
5. **Pull:** `click {ctrl: true}` on them. **A cuffed person being pulled can't move and can't break the pull.** `key H` stops pulling.
6. **Search:** `drag` them onto yourself to open the **strip menu**, with your active hand **empty**. Take their hands' contents first, then the belt, the back (open the backpack after you take it), suit storage, both pockets, gloves (insulated gloves), mask and glasses (flash protection), and the ID if it's stolen. Each item takes about 4 s.
7. **Confiscate:** weapons, contraband and stolen items go to Evidence Storage (an evidence closet), or back to the owner. The disk and the Captain's ID go to the Captain, in person. Never drop confiscated items on the floor near the prisoner.
8. **Escort:** keep pulling and `walk_to {area: "Brig"}`. If you have no time for a cell, the Holding Cell will do.
9. **Cell** (if a Warden is on shift, hand the prisoner to them instead):
   1. Pick a free cell and click its cell door to open it.
   2. Pull the prisoner in, stop pulling, and put their belongings in the **Cell N locker**. Contraband goes to evidence instead.
   3. Step out. The prisoner keeps the cuffs, or you remove them first if they're cooperative.
   4. Use the cell's door timer (named "Cell N"): set the time, then **Start**. Starting **closes the cell door and locks the cell locker**.
10. **Records:** set them to **Incarcerated** and add the crime (§4.5). Announce it on `:s`, for example "Cell 2: Jane Doe, theft (310), 8 min, started".
11. **Release.** When the timer runs out, the security channel says "Timer for Cell 2 has expired. Releasing prisoner." The door opens and the locker unlocks. Get your cuffs back (strip menu "handcuffs"), let them take their own things, set them to **Discharged**, and say it on `:s`.

### 4.4 Brig timer (tgui "BrigTimer"; needs security access; stand adjacent)
`click` the door timer, then use these actions:

| Action | Params | Effect |
|---|---|---|
| `preset` | `{preset: "short"}` / `"medium"` / `"long"` | 2 / 3 / 5 minutes |
| `time` | `{adjust: 600}` / `{adjust: 100}` / `-100` / `-600` | ±1 min / ±10 s |
| `start` | | Closes the cell door, locks the cell locker, starts the countdown |
| `stop` | | Ends early: opens the door and unlocks the locker, with no radio message |
| `flash` | | Fires the cell's flasher |

The maximum is 15 minutes. Example for 8 minutes: `preset long`, then `time {adjust: 600}` three times, then `start`.

### 4.5 Records and criminal status
The statuses are **None, Suspected, Arrest, Incarcerated, Parole, Discharged**. Setting someone to **Arrest** makes **Officer Beepsky** and the other securitrons arrest them on sight. Securitrons also take note of Suspected, Incarcerated and Parole.
- **Through the HUD** (wear the security HUDSunglasses): `examine` the person. The answer has "Criminal status: [None]" with a link, plus "Security record: [View]", "[Add citation]", "[Add crime]" and "[Add note]". The links **expire 1 minute after the examine**. Follow the status link with `topic`. A tgui list window titled "Security HUD" opens: `tgui_act` with action `submit` and params `{entry: "Arrest"}` (or any other status). Choosing Arrest through the HUD adds a crime "Set by SecHUD" automatically. [Add crime] asks for a crime name in a text window (`submit {entry: "..."}`).
- **Through a security records console** (Security Office, Security Posts, Customs, Detective's Office, Brig Control): `click` it to open the tgui window "SecurityRecords".
  1. `login` (needs security access).
  2. Find the person in `data.records[]`, which has `name`, `rank`, `wanted_status` and `crew_ref`.
  3. `add_crime {crew_ref, name: "Theft", details: "Took the Captain's ID from his locker", fine: 0}`. With fine 0 it's a crime, and it **sets the status to Arrest**. A fine above 0 makes a citation instead.
  4. `set_wanted {crew_ref, status: "Incarcerated"}`. **Arrest needs at least one crime on the record.**
  5. `set_note {crew_ref, note}`. `invalidate_crime {crew_ref, crime_ref}` voids a crime. `logout` when done.
  
  Only the author of a crime, or someone with armory access, can edit it.
- The security PDA's Security Records program is view-only.

### 4.6 Space Law (summary of the wiki's Space Law page; it's a guideline, not code)
Sentence only for the **worst** crime, then apply modifiers. A repeat trip to the brig raises the tier by one. When unsure, charge the lesser crime.

| Tier | Crimes (code) | Sentence |
|---|---|---|
| Mischief 1XX | Disturbing the Peace 101, Spreading Disinformation 103, Littering 104, Insubordination 105, Trespass 106, Possession of a Weapon 108, Drug Possession 109, Indecent Exposure 112 | 3 min (preset medium), or a fine up to 100 cr |
| Misdemeanor 2XX | Assault 201, Animal Cruelty 202, Rioting 203, Vandalism 204, Dereliction of Duty 205, Breaking and Entry 206, Possession of a Restricted Weapon 208 (guns, batons, flashes, grenades; Captain, HoP and Security are licensed), Petty Theft 210, Creating a Workplace Hazard 212 | 5 min (preset long), or a fine up to 300 cr |
| Felony 3XX | Assault With a Deadly Weapon 301, Assault of an Officer 302 (includes grabbing or disarming an officer), Inciting a Riot 303, Sabotage 304, Aiding and Abetting 305, B&E of a Restricted Area 306, High-Security Trespass 307 (security, command, EVA, engine, atmos, toxins), Contraband 308, Possession of Explosives 309, Theft 310 (weapons, insulated gloves, spacesuits, jetpacks), Kidnapping 311, Manslaughter 312 | 8 min |
| Grand Felony 4XX | Attempted Murder 401 (attacking someone already in critical condition), Brainwashing 403, Grand Sabotage 404, Enemy of the Corporation 405, Grand Theft 410 (**the nuclear authentication disk, the Captain's ID**, the blackbox, a supermatter sliver) | Permabrig, or a timed sentence plus parole |
| Capital 5XX | Murder 501, Mutiny 503 | Permabrig (execution only with the Captain's authorization: not your call) |

Modifiers: Resisting Arrest +2 min. Cooperation or surrendering −2 min. Self-defence (protecting yourself, colleagues or workplace): immediate release. Escaping the brig: reset to the full sentence. Prisoners get medical care if seriously hurt. Permanent imprisonment is ordered by the Warden or HoS; if neither is on shift, ask the Captain.

**Permabrig.** Pull the prisoner through the "Prison Wing" doors and strip them completely; evidence goes to Evidence Storage, other belongings to a prison locker. Dress them in an orange prisoner uniform from the Transfer Centre or Holding Cell, take the cuffs and leave. The Prison Wing doors need security access, so a prisoner without an ID stays in. Set them to **Incarcerated** with the crime noted.

### 4.7 Patrol and posting
- **Patrol loop** (from the Brig):
  1. Fore Primary Hallway
  2. Central Primary Hallway (Command Hallway: the Bridge, Captain's Quarters and AI Upload Access are here; the disk and the Captain's ID are prime targets)
  3. Starboard Primary Hallway (Bar Lounge, Kitchen side)
  4. Aft Primary Hallway (Science Lobby, **Medbay Lobby**)
  5. Port Primary Hallway (Cargo Lobby, Library, Arrivals)
  6. Storage Wing / Primary Tool Storage
  7. back to the Brig

  Stop briefly at each lobby and at your department's Security Post. Check in on `:s` whenever you change area, so the AI and the crew know where you are.
- **Alone** (the only officer on shift): you are both the patrol and the brig. Patrol the loop, but come back to the Brig whenever you hold a prisoner, and check the security camera console now and then. Answer minor calls (theft, trespass, vandalism) yourself. For **anything armed or violent**, get the AI on the doors and cameras first, warn the crew, and bring crew who fight back; don't walk into it alone.
- **With other officers:** one holds the Brig and Security Office (prisoners, records, cameras, break-outs) and the Command Hallway; the others take their department posts and the patrol loop. The nearest officer answers minor calls; **armed or violent calls get two officers**, who meet at a rally point (the Brig, or the nearest Security Post) and arrive together.
- **Under a Warden or Head of Security:** go where they post you; prisoners go to the Warden at Brig Control.
- **Hot spots** seen in past shifts: Captain's Quarters and the Bridge (disk and ID theft), the Medbay Lobby and Medbay Treatment Center (beatings, people dragged there to be finished off), the Bar, Cargo deliveries, maintenance (where attackers hide).

### 4.8 Radio protocol (security channel `:s`)
- Format: **what, where, who, need**. For example: `:s Armed: Not A Clanker, Medbay Lobby, energy gun, stunned the Janitor. Need backup.` and `:s Copy, en route from Brig, 30 s.`
- Status lines: "on patrol Starboard Primary Hallway", "at Security Post - Medbay", "back at Brig", "prisoner in Cell 1".
- Wanted call: `:s Wanted: Kira Swarner, grand theft (410), the disk. Set to Arrest.` Repeat it on `;` only if you want the crew's eyes. Don't spread unconfirmed accusations on common.
- `Officer down, <area>` means every officer and the AI drop everything.
- To the AI: `:s AI, track <name> and bolt the doors around them`, or `AI, open the Armory for the Captain`.
- Keep it short. **Radio and announcements can be faked**: a parrot repeats lines, players spoof Captain announcements, OOC claims of admin authority come from ordinary players. Trust what you see and confirm through a second source.

## 5. Dangers and common mistakes
- **No baton:** it's in the **security belt** inside the six Gear Room lockers. Not in the SecTech, not in the departmental lockers. In a past shift an officer patrolled without one.
- **Going alone after an armed attacker.** In a past shift an officer was shoved and **disarmed of his disabler**. The attacker took a baton and an energy gun, cuffed the officer and shot him in the brig. Later he was dragged into medbay while cuffed, re-cuffed after a doctor freed him, and beaten to death on glass tables; he couldn't be revived ("heart too damaged"). Lessons:
  - Keep weapons in suit storage and on the belt until you use them.
  - Don't let suspects crowd you.
  - Bring backup: another officer if one is on shift, otherwise the AI on the doors and crew who fight back.
  - Cuff and strip a disabled attacker at once.
- **Releasing a thief too fast or searching too little.** In a past shift a cuffed thief was released without a full search and **took the disk back** the moment the officer was shoved. Check both pockets and the backpack. Hand the disk straight to the Captain; never put it down or drop it.
- **Stamina wears off in 10 s.** Don't stop to talk between the stun and the cuffs.
- **Flash from behind, or on someone in sunglasses:** nothing happens. Check what they wear and which way they face.
- **Armor:** a target in a stolen armor vest takes 25-40% less from the baton and disabler.
- **Strip menu with an item in your hand:** it tries to *put* that item on them. Empty your active hand first.
- **Locking yourself in a cell:** step out before you press `start`.
- **Doors you can't open:** Captain's Quarters, the Bridge, Brig Control, the Armory. Ask the AI or the Captain. Never break in on a hunch.
- **Abuse of power:** no harm-baton on a cuffed person, no beating someone who's down, no searches without cause (red alert permits random searches). Unlawful arrest counts as Kidnapping (311).

## 6. Emergencies
- **Attacker or killer loose:**
  1. Report on `:s` and `;`: description, weapon, area, direction.
  2. Ask the AI to track them on cameras and to bolt or close doors around them.
  3. Gather backup (another officer, crew who fight back), then follow §7.2.
  4. Ask the Captain for armory access, and for red alert if it's bad. Red alert needs two heads of staff at two keycard authentication devices; the communications console can only set blue or green.
- **Mass casualty / bodies:** secure the scene first (the attacker may still be there), then get the wounded to Medbay and call the doctors (`:m` if your headset has it, otherwise `;`). Don't leave a body where an attacker can keep beating it.
- **Prison break / riot:**
  - Brig Control's lockdown buttons need armory access. Ask the AI to bolt doors.
  - The Brig Entrance Flasher and Holding Cell Flasher buttons need only security access; so does a cell timer's `flash`.
  - Order the crowd to disperse before you charge anyone with rioting.
- **Fire, breach, power failure:** get civilians out, keep the brig's prisoners safe (move them if the cell is endangered, otherwise release them, per Space Law), and leave repairs to engineering and atmos. Your survival box has a gas mask and oxygen. Never open a door that leads to space.
- **Evacuation:** escort prisoners to the shuttle cuffed and keep them pulled; stay with the Captain and the disk.

## 7. Defending yourself and your department
You are the one expected to stand and fight. Shared combat mechanics are in crew-basics: combat mode (`key F`), shoves, grabs, resisting (`key B`).

### 7.1 Your means
Armor vest and helmet (35 melee each), stun baton (2 hits floor an unarmored person), disabler (4 shots), flash, pepperspray, flashbang, HUDSunglasses (flash-proof), bowman headset (flashbang-proof), mindshield, rechargers in every security room, and the security-access doors, flashers and cameras of the Brig and the Security Posts.

The client's `fight` tool (crew basics §6) does the clicking for you: `fight {target: <id>, goal: "subdue"}` with the
baton turned on (Z) in your active hand stuns them; with handcuffs in hand it cuffs someone who is down and holds
still the 4 s; `goal: "kill"` only under lethal force (§7.3). Set `fight {stance: "fight back"}` at shift start.

### 7.2 Fighting an armed killer
1. Never chase alone into maintenance or a dark room. Let them come to you, or wait for backup and the AI's tracking. Ask the AI to bolt the doors around them so they have to come out where you are.
2. With another officer: approach from two sides. One stays back 3-5 tiles with the disabler and shoots; the other closes in with the baton when the target turns to the shooter, then batons and cuffs. Alone: open with the disabler from range (4 hits), close in with the baton only when they're slowed or down, and cuff at once. Crew who help can shove, pepper-spray or hold the target while you cuff.
3. Stay out of doorways and narrow corridors where only one of you can shoot. Don't stand in another officer's line of fire, and keep crew out of yours.
4. Once they're down: cuff them, strip their weapons first (hands, belt, suit storage, back), then pull them.
5. Hurt below half health? Disengage to the Security Medical or Medbay, and say so on `:s`.

### 7.3 Lethal force
Non-lethal by default. Your personal file sets how far you go, within these rules (Space Law, "Use of Deadly Force"): lethal force is only for someone actively trying to kill crew who keeps going after your non-lethal means have failed, targets non-lethal tools don't stop (mechs, borgs), or being mobbed with no other way out. Never on someone cuffed, floored, surrendering or fleeing unarmed. Stop as soon as they're down, then cuff them. Lethal weapons are in the **Armory**: the HoS, the Warden and the Captain's ID open it, and the AI can open its door when the Captain orders it. Get permission over the radio before you take anything from it.

### 7.4 If you're cuffed
- `key B` (resist) starts 1 minute of work ("you need to stand still"). Zipties take 45 s.
- **Any movement cancels it, including being pulled or shoved.** While you're cuffed and pulled you can't move ("You're restrained! You can't move!") and you can't break the pull.
- If you're buckled, you must unbuckle first, which takes the same time.
- Call `:s Officer cuffed, <area>, pulled by <name>` while your radio still works (it fails in critical condition). Ask any crew member to remove your cuffs through your strip menu ("handcuffs").
- Don't fight a pull; resist the moment they let go.

### 7.5 Protecting Medbay
In a past shift the killer worked in Medbay. Medical-assigned officers hold the Security Post - Medbay. Its "Medbay Doors Control" button closes the Medbay and Medbay Clinic doors, and the post overlooks the Medbay Lobby. Everyone else: when someone is dragging a cuffed or unconscious person into Medbay and they aren't medical staff, stop them and ask why. Escort wounded prisoners and keep them cuffed while they're treated.

### 7.6 The nuclear authentication disk
If you recover it, put it in your pocket and walk it to the Captain. Hand it over in person (`key G` to give, or ctrl+shift+click to offer) and say on `:s` that it's delivered. If the Captain is dead or missing, keep it on you, tell the Head of Personnel and the AI, and guard it. Never leave it in a closet or on a table. Arrest whoever took it (Grand Theft 410).

## 8. Working with the crew
- **Captain:** your superior when no HoS is on shift. Owns the disk. Grants armory access, decides permabrig and execution, and with the HoP can raise red alert. Escort them when they're threatened.
- **Head of Personnel:** second in command. Can change IDs and access, and can demote criminals. Ask them to strip access from a convicted thief, or to grant an officer an access you need for a task (the Captain decides armory access).
- **Head of Security, Warden, Detective, other officers** (if they're on shift): the HoS and Warden outrank you. Prisoners go to the Warden. Forensic evidence goes to the Detective. Pair up with any other officer on shift.
- **AI:** your best partner. It tracks people on cameras, opens and bolts doors, opens doors you lack access to, and announces. Tell it on `:s` what you need, in one line.
- **Medical Doctors:**
  - Take hurt prisoners and officers to them.
  - Protect Medbay.
  - Ask them to report anyone who drags in a body.
- **Chemist:** medicine for you and your prisoners.
- **Scientist:** the department techfab (Security) prints from researched designs. At round start: rubber .38 rounds and beanbag and rubbershot shotgun shells. Ask for the techweb nodes **Security Equipment** (pepperspray, zipties, seclite, evidence bags) and **Riot Supression** (handcuffs, energy bola, shields).
- **Engineers, Atmospheric Technician:** call them for breached or destroyed doors, walls built across the corridors, and fires. Escort them into dangerous areas.
- **Quartermaster:** security crates through cargo.
- **Shaft Miner:** carries a combat knife and a seclite and works off-station; a willing fighter when they're aboard.
- **Janitor:** cleans up after fights. Can return found weapons. Keep a list of what was recovered.
- **Cook, Botanist:** donuts. Drugs grown in hydroponics are part of a botanist's job, not a crime by itself.
- Everyone: be visible and polite, say why you're arresting someone, and release on time.

## 9. Through the client
- `connect`, then `load_map` with the map file named in your prompt. After that `walk_to {area: "Security Locker Room"}` and the others work station-wide. `access_note` tells you when a door needs access you lack.
- **Find a suspect:** use `search` (kind mob) with their name, or with the "as" name when they wear a stolen ID. `walk_to {object_id, kind: "mob", adjacent: true}` follows them while they stay in view. It can answer "arrived" when they've already moved, so check with `look` that they're adjacent before you cuff. A fleeing mob that leaves your view must be re-found with `search` or tracked by the AI.
- **Equip:**
  - Click a HUD slot with an item in hand to put it there.
  - `key Shift+E` draws from or holsters to the belt; `key Shift+Q` does the same for suit storage.
  - `key Z` uses the item in your hand: turns the baton on, arms a flashbang, AOE-flashes with a flash.
  - `key X` swaps hands.
  - `inventory` shows what's in each slot.
- **Fight:**
  - Baton: left click (`click {object_id}`).
  - Disabler: click the target from range. `right: true` within 2 tiles holds them at gunpoint.
  - Throw (bola, flashbang): `key R`, then click.
  - Pull: `click {ctrl: true}`; `key H` stops pulling.
  - Resist: `key B`.
- **Strip menu:** with your hand empty and the target adjacent and not moving (cuff first), `drag` them onto yourself. A tgui window "StripMenu" opens. `tgui_act {action: "use", params: {key: "right_hand"}}`. Other keys: left_hand, belt, back, suit_storage, id, left_pocket, right_pocket, gloves, eyes, mask, head, suit, jumpsuit, shoes, ears, handcuffs, legcuffs. The window goes view-only when either of you steps away. `use` on "handcuffs" uncuffs the target.
- **Lockers:** click once to unlock and again to open. Put items in by clicking the open locker with the item in hand, or drop the item on its tile; then click the locker to close it.
- **tgui:** BrigTimer and SecurityRecords actions are in §4.4-4.5; the SecTech uses `vend` with the product's ref (`tgui_window` lists them).
- **HUD links** from `examine` are only good for 1 minute. Follow them with `topic` at once.
- **Chat:**
  - `mute` emote spam ("points at") during busy moments.
  - `wait` with `until` stops on any line containing that text, including your own.
  - `say` with `radio: "security"` sends on `:s`; the answer tells you when no radio line came back (for example in critical condition).
- `status` shows health bands. When you're hurt, retreat before you enter critical condition, not after.

## 10. Checklist

**Shift start:**
1. `connect`, `load_map`; read your department assignment line.
2. Gear Room: open a security officer's locker. Put on the security belt (PDA into the backpack) and the security HUDSunglasses, attach the seclite to the helmet, turn the baton on.
3. Optional SecTech buys: zipties, energy bola, a spare flash.
4. Check in on `:s`. If other officers are on shift, agree who holds the Brig and who patrols. Say hello to the AI.
5. Visit your department's Security Post (records console, recharger, the head of the department).

**Ongoing loop:**
1. Patrol the route, or hold the Brig; check Medbay Lobby and the Command Hallway.
2. Read chat and radio; respond with **what, where, who, need**.
3. Arrest: warn, disable, cuff, pull, search, confiscate, cell + timer, records, announce.
4. After every fight: recharge the baton and disabler, replace burnt flashes, restock cuffs.
5. Release on time, set them to Discharged, return their belongings.
6. Recovered disk or Captain's ID: straight to the Captain.

## 11. Sources
- Code (tgstation 54c22023): `code/modules/jobs/job_types/security_officer.dm`, `code/datums/id_trim/jobs.dm`, `config/game_options.txt`, `code/modules/vending/security.dm`, `code/game/objects/structures/crates_lockers/closets/secure/security.dm`, `code/game/objects/items/storage/belt.dm`, `code/game/objects/items/weaponry/melee/baton.dm`, `code/modules/projectiles/`, `code/modules/assembly/flash.dm`, `code/game/objects/items/handcuffs.dm`, `code/datums/status_effects/debuffs/stamcrit.dm`, `code/modules/mob/living/damage_procs.dm`, `code/game/machinery/doors/brigdoors.dm`, `code/game/machinery/computer/records/`, `code/modules/mob/living/carbon/examine.dm`, `human.dm`, `carbon.dm`, `living.dm`, `code/modules/research/techweb/nodes/security_nodes.dm`; tgui `BrigTimer.tsx`, `SecurityRecords/`, `StripMenu.tsx`, `ListInputWindow`.
- Map: `_maps/map_files/MetaStation/MetaStation.dmm`; areas: `code/game/area/areas/station/security.dm`.
- Wiki (CC BY-SA 3.0, Internet Archive captures): Space_Law, Security_Officer, Guide_to_Security, Standard_Operating_Procedure.
- Past shifts' reports: 12-security, 12-assistant1, 12-assistant2, 12-janitor, 12-captain, 12-doctor, 12-chaplain.
