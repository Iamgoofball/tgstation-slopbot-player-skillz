# Captain

## The job in one paragraph

You command the station. Heads of staff answer to you, and through them every department does too. The Head of Personnel is your second in command, then the Research Director, Chief Engineer, Chief Medical Officer, Head of Security and Quartermaster, for whichever of them are on shift. Your duties: keep the crew alive and working; give clear orders over the Command and common channels; settle disputes; authorise Security when force is needed; keep the **nuclear authentication disk** on your person all shift; keep your **gold ID**, which opens every door and is a thief's first target; and decide when the station evacuates. A good shift ends with the disk secure on you (aboard the escape shuttle, if there is an evacuation), the crew informed, nobody needlessly dead and every department working. You lead and delegate. Doing other people's jobs, or charging into fights alone, is not your role. The crew list you were given is not complete: more players can join at any time, in any job, other heads of staff included.

## Starting kit and access

Your outfit (`code/modules/jobs/job_types/captain.dm`):

| Slot | Item | Notes |
|---|---|---|
| ID | **gold identification card** (Captain) | All station access. It is also the key to your own rooms: lose it and you are locked out of them, or locked in. |
| Uniform / suit | captain's jumpsuit, **captain's carapace** | Armour: melee 50, bullet 40, laser 50, energy 50, fireproof. Its suit storage slot holds a gun or a baton. |
| Head | captain's hat | Melee armour 25. |
| Gloves | captain's gloves | Insulated: you can touch live wires. |
| Glasses | sunglasses | Protect you from flashes. |
| Ears | **captain's bowman headset** | Protects you from flashbangs. See the radio notes below. |
| Belt | captain PDA | |
| Backpack | **gold-capped telescopic baton**, station charter, survival box | |
| Implant | mindshield | |
| Skillchip | disk verifier | When you examine a fake nuke disk, you see "The serial numbers on [it] are incorrect." |
| Also | **spare ID safe code biscuit card** | In a pocket, your backpack or your hands. It holds the 5-digit code for the spare ID safe. Keep it secret. |

**Access**: every station door (common, command, private head offices, Captain), plus the Armory, AI Upload, Vault, EVA, Teleporter, telecomms, keycard authentication and ID changes.

**Radio** (your headset's key): Command and Security are on from the start. Engineering, Science, Medical, Supply and Service are on the key but switched **off**. While a channel is off you don't hear it, and you can't send on it either (the game drops the line). To turn one on, open the headset's Radio window and toggle that channel (see "Through the client"). Keys: `;` common, `:c` command, `:s` security, `:e` engineering, `:n` science, `:m` medical, `:u` supply, `:v` service. Alt-clicking your headset toggles high-volume mode, which makes your radio lines louder.

## Where things are on MetaStation

**Getting there.** From the Arrival Shuttle Hallway (west), go east along the Port Primary Hallway into the Central Primary Hallway. The **Command Hallway** runs along the Bridge's south wall. The Bridge is near the station's centre, the Departure Lounge is at the far south end, and the AI Satellite is far to the east.

### Captain's Quarters

The whole suite is one area, "Captain's Quarters", east of the Bridge. Every door in it needs **Captain access, from both sides**.

- **Outer airlocks** "Captain's Quarters": one on the west wall, opening from the Bridge's starboard access corridor, and one on the south wall, opening from the Command Hallway. Both lead into the **lounge**: booze-o-mat, cigarette machine, chairs, and Renault the fox (your pet).
- **Desk**: two windoors named "Captain's Desk" in the counter on the lounge's north side. Walk through the **west** one. The east one stands on a table and works as a service hatch. On the counter: a secure briefcase and the **medal lockbox** (west end), a fax, and the **hand tele** with your stamp (east end). Thieves want the hand tele: lock it in your locker or carry it.
- **Office**, behind the desk:
  - West end: the **display case** (antique laser gun) and a table with Space Law and the chain of command.
  - East wall: the **communications console**, with the **keycard authentication device** on the wall beside it.
  - Below them: an ID console and the Captain's Requests Console.
- **Inner airlock** "Captain's Quarters", north of the office, leads into a short hallway with:
  - the **Bathroom** airlock (west);
  - the **captain's locker** and the **suit storage unit** (north side);
  - the **"Captain's Bedroom" windoor** (Captain access), which opens into the bedroom.
- **Bedroom**: the **nuclear authentication disk** and the **pinpointer** start on the table in its north-west corner. A cyborg recharge station and a disposal bin stand on the north wall. The bed is behind a plain windoor that anyone can open. Next to the bed: a dresser with a wall safe and a gun recharger on a table.

What is where:
- **Captain's locker** (Captain access): energy gun, **sabre sheath with the officer's sabre**, **command door remote**, command megaphone, two spare captain's headsets, clothes.
- **Suit storage unit**: magnate MODsuit (space-proof armoured suit: melee 40, bullet 50, laser 50), captain's gas mask, captain's jetpack.
- **Display case**: the **antique laser gun** (self-recharging, 30 burn per shot). It is locked to CentCom access, so your ID cannot open it. Breaking the glass sets off a burglar alarm. Leave it there unless the station is lost.

### Bridge

Area "Bridge". The Council Chamber meeting table is inside it.

**Entrances**: two pairs of "Bridge Access" glass airlocks on the south wall, opening from the Command Hallway, one pair at the west end and one at the east. Behind each pair is a short corridor and a second pair, "Bridge". The two doors of a pair cycle, so one opens at a time. All need command access.
- West corridor: the door "Head of Personnel" into the Head of Personnel's Office, and a "Council Chamber" door.
- East corridor: the other "Council Chamber" door, and the Captain's Quarters west airlock.

**Command pit**: in the middle of the Bridge, behind windows. You get in through the "Command Desk" airlock (from the Council Chamber) or the "Command Desk" windoor (from the north). Both need command access. Inside:
- the **communications console**;
- the **captain's spare ID safe**, on the table beside it;
- the command chair;
- buttons: "Bridge Access Blast Door Control", "Council Chamber Blast Door Control", "Gateway Shutter Control", "E.V.A. Storage Shutter Control". More Bridge Access blast door buttons are in the two access corridors.

**North console row**, west to east: ID console, Medical Records, **Crew Monitoring Console**, Station Alert Console, **Bridge Power Monitoring Console**, Atmospheric Alert, **Security Cameras**, Security Records, R&D console.

**Elsewhere on the Bridge:**
- West side: command and engineering consoles, a **medkit**, and a **DeForest first aid station** on the wall. Click the station with an empty hand: it heals brute and burn damage, charges your account, and is free on red alert.
- East side: the **keycard authentication device** (north wall, by the mining camera console), the Bridge Requests Console and a cargo request console.
- **Handcuffs**: two pairs, one on a table with a recharger (east) and one in the command pit.
- South racks: an intellicard, signalers, emergency toolboxes, a wrench and multitool; a fire axe cabinet.

### Other places you will use

- **Head of Personnel's Office**: west of the Bridge. It has a keycard authentication device on its east wall.
- **AI Upload Chamber**: fore of the Bridge. It holds the AI's core module rack (its laws) and is guarded by turrets. Changing laws is a last resort and not covered here.
- **AI Chamber** (the AI core): in the AI Satellite, reached through the **Transit Tube** from Engineering.
- **Armory**: in the Brig, north part of the station. Lasers, energy guns, disablers, a shotgun, riot gear. You have access.
- **Departure Lounge**: at the south end of the **Aft Primary Hallway**. The emergency shuttle docks on its south side and you board through the "Departure Lounge Airlock" doors. **Those lead to space unless the shuttle is docked.**
- **Bar Lounge** (with the Bar): just east of your quarters. It is a public room for crew meetings. The Council Chamber is on the Bridge, so crew without command access can't get in.

## Doors: how not to get locked in

Yesterday the Captain spent 47 minutes shut inside her own quarters. A thief had taken her ID, and every door there needs Captain access, from inside too. Prevent it:

1. **Your ID never leaves your ID slot.** Take it into your hand only to swipe at the communications console, then put it straight back.
2. **Carry the command door remote** from your locker, in a pocket. It opens the Bridge, your quarters (doors and windoors), the HoP's office, EVA, the Vault, the Teleporter and the AI Upload, from a distance, with no ID needed.
   - Use it in hand to cycle modes: Open Door → Toggle Bolts → Toggle Emergency Access.
   - Hold it and click a door to apply the mode.
   - Bolting your outer airlock shut keeps thieves out. Unbolt it with the same remote.
3. **If you lose both**, call the AI on common: "AI, open the Captain's Quarters inner door." The AI can open any powered door. Engineers can also hack or pry doors.
4. Don't let anyone follow you through a door. Yesterday a thief walked into the quarters through an airlock the Captain had just opened.
5. The spare ID safe is on the Bridge, outside your quarters. If you are locked in your quarters, it can't help you.

## Shift start (in order)

1. `load_map`, then go to the Captain's Quarters. You may have spawned there (roundstart) or at Arrivals (late join).
2. **Bedroom**: pick up the **nuclear authentication disk** and the **pinpointer**. If the disk is gone, follow "The disk is missing" below.
3. **Captain's locker**: the first click unlocks it with your worn ID, the next click opens it. Take:
   - the **sabre sheath**: wear it on your belt and move the PDA to your backpack;
   - the **energy gun**: put it in your carapace's suit storage slot;
   - the **command door remote**: a pocket;
   - the megaphone, if you want it.

   Close the locker, then right-click it to lock it again. Lock the hand tele inside if you're not carrying it.
4. Stow the disk. The backpack is safer than a pocket: when someone strips your backpack you get a warning, while a pickpocket that succeeds is silent ("You feel your … pocket being fumbled with!" appears only when the attempt fails). Every strip takes about 4 seconds next to you, and stepping away breaks it.
5. Read your spare ID code: hold the spare ID safe code biscuit card, use it in hand and answer Yes to crack it open, then read the paper slip inside. Remember the 5 digits. **Tell nobody.**
6. Open your headset's Radio window and turn on the department channels you will coordinate (Engineering and Medical at least). Turn them off again if they flood you.
7. At the communications console, make a short welcome announcement: who you are, the priorities for the shift, and how to reach you.
8. Over Command (`:c`): ask each head of staff on shift to report in. Then ask each department on common for a short status: Engineering (engine and power), Atmospherics, Medical, Security, Supply, Science, Service. Departments with no head of staff report to you directly. Delegate staffing and access requests to the Head of Personnel.

## The communications console

There are two on MetaStation: one in the Bridge's command pit and one in your office. Any command-access ID can log in, call or recall the shuttle, set the status displays and read messages. Only **Captain access** (or the AI) can make announcements, change the alert level, or toggle emergency maintenance access. Only the Captain can message CentCom. Whoever holds your gold ID can do all of this: yesterday a thief made a fake "kill security" announcement with the Captain's stolen card.

| Button (tgui action) | What it does, exact rules |
|---|---|
| Log In / Log Out (`toggleAuthentication`) | Reads your worn or held ID. You must log in before anything else. |
| Make Priority Announcement (`makePriorityAnnouncement`) | Opens a text box; submit your text. It shows station-wide as "Captain's Announcement". 30 s cooldown for crew announcements. |
| Call Emergency Shuttle (`callShuttle`, `{reason}`) | The reason must be **at least 12 characters**. Not allowed in the round's first **20 minutes** ("The emergency shuttle is refueling…"). |
| Recall Emergency Shuttle (`recallShuttle`) | See "Recalling" below. The AI cannot recall. |
| Green / Blue (`changeSecurityLevel`, `{newSecurityLevel: "green"\|"blue"}`) | **Hold your ID in your active hand** ("Swipe ID"). Only green and blue can be set here; **red needs the keycard authentication device.** |
| Enable/Disable Emergency Maintenance Access (`toggleEmergencyAccess`) | Unlocks every maintenance airlock for everyone, station-wide. 3 quick uses, then a 30 s cooldown. |
| Set Status Display (`setState {state: "changing_status"}`, then `setStatusMessage {upperText, lowerText}`) | Two short lines on every status display. |
| Message List (`setState {state: "messages"}`) | CentCom messages; answer one with `answerMessage {message: N, answer: M}`. `setState {state: "main"}` goes back. |
| Send message to CentCom (`messageAssociates {message}`) | 60 s cooldown. It rarely gets an answer. |

Don't touch "Request Nuclear Authentication Codes" or "Purchase Shuttle". The shuttle purchase spends the cargo budget.

## Alert levels

- **Green**: normal operations.
- **Blue**: credible threat. Security may carry weapons openly and search people.
- **Red**: immediate serious threat. Weapons drawn, searches advised. The EVA Storage and Medbay Storage doors open for everyone, defibrillator wall mounts unlock for any ID, and first aid stations become free.
- **Delta**: the station is about to be destroyed. It is set by the game (for example by a nuke), never by you.

The alert level also changes the shuttle's travel time (see the evacuation section).

Raise to **blue** at the communications console: ID in your active hand, press Blue. Go back to **green** when the threat is over.

**Red alert** needs two people at two different **keycard authentication devices**, each with keycard access: you, plus the Head of Personnel, Quartermaster or any other head on shift. The AI can't do it.
1. Agree on common or Command who stands where. Good pairs: your office device and the Bridge's, or the Bridge's and the HoP's office device.
2. Both click your devices; each opens a "KeycardAuth" window.
3. You press **Red Alert** (`red_alert`). Every other device then offers **Authorize** (`auth_swipe`) for only **2 seconds**.
4. Your partner has to press it inside that window, which is hard to time. Count down on the radio. From zero, you press `red_alert` again every few seconds and your partner keeps sending `auth_swipe`, until the red alert announcement appears.
5. The same device also has **Emergency Maintenance Access** (`emergency_maint`), confirmed the same way. You can toggle that one alone at the communications console.

## The nuclear authentication disk

- **The rule**: the disk stays on the station and **on your person**. Never leave it in a locker, a safe or on a table. Never hand it over except to the next in command when you are about to die or be captured.
- **What the game checks**: the disk counts as secured only while a connected player carries it **and moves around**. If it sits unmoved for more than about 8 minutes (500 s), the chance of a nuclear operative being sent for it slowly rises. Examining the disk tells you "Right now, it is" or "…it isn't."
- **Where it can be**: anywhere on the station, the emergency shuttle or the escape pods. If it is carried off the station any other way, it teleports to a random spot on the station.
- **Pinpointer**: use it in hand to switch it on. It points toward the real disk (never a fake) and shows close, medium or far. Examining it shows what it is tracking. It also sounds an alarm if a nuclear bomb is armed. The client may show its direction as "facing …" (unverified).
- **Fakes**: decoy disks exist. Examine any disk you recover: if "The serial numbers on [it] are incorrect" appears, it's a fake. Keep looking with the pinpointer.

**The disk is missing**:
1. Check your `inventory` first. Then switch on the pinpointer and follow it. `search` finds a disk only once it is in view; things inside bags, closets or someone's hands don't show.
2. Tell Security on `:s`: the description, where it was last seen, and who was near you. Ask the AI to track the suspect with its cameras and to bolt doors around them. Ask the crew on common to report sightings.
3. Raise the alert to blue. If the thief is armed or violent, go to red.
4. Once the thief is restrained, open their strip menu, take the disk back, and verify it isn't a fake.
5. Never chase alone into maintenance. Go with Security.

## The emergency shuttle

### When you call it
Call it only when:
- **the round has become unplayable**: the station is being destroyed (engine delamination, large areas depressurised or burning), most of the crew is dead, or there is a threat nobody can stop; or
- **about 90 minutes of round time have passed.** Your `statpanel` (Status tab) shows "Shift Time/PT: hh:mm:ss", the time since the round started.

Don't call it on a schedule otherwise. Before calling, tell Command (`:c`) why.

### Recalling
If anyone else calls the shuttle without such a reason, recall it. The announcement "The emergency shuttle has been called" shows their reason, and each console shows where the call came from (most of the time). To recall:
1. Log in at a communications console.
2. Press **Recall Emergency Shuttle** (`recallShuttle`).
3. Announce that you recalled it and why.

Recalling is only possible during the **first half** of the trip:

| Alert | Call → arrival | Recall allowed while more than |
|---|---|---|
| green | 20 min | 10 min remain |
| blue | 10 min | 5 min remain |
| red | 5 min | 2.5 min remain |
| delta | 2.5 min | never (no recall) |

If the alert level changes mid-flight, the remaining time scales with it. A recalled shuttle can't be called again until it is back at CentCom. Someone with command access can keep calling, so find out who (Security, the HoP) and keep them away from the consoles.

Once docked, the shuttle waits **3 minutes**, then flies to CentCom in **2 minutes**, and the round ends. The shuttle is also called automatically if every communications console is destroyed and there is no working AI.

### Evacuation procedure (when it happens)
1. At a communications console, press **Call Emergency Shuttle** (`callShuttle`) with a clear reason, for example "Station-wide breach, evacuating crew".
2. Make a priority announcement:
   - "Evacuation: the shuttle docks at the Departure Lounge (south end, down the Aft Primary Hallway) in N minutes."
   - "Bring the injured and the dead. Security brings prisoners."
   - "Do not open the Departure Lounge Airlocks until the shuttle has docked."
3. Over Command and the radio, assign the jobs:
   - Medical carries casualties.
   - Security escorts and holds the Departure Lounge.
   - Engineering keeps the route powered and sealed.
   - The AI announces routes and opens doors.

   If doors are the obstacle, enable Emergency Maintenance Access.
4. Give a reminder on common at 10, 5 and 2 minutes, reading the ETA from the status panel.
5. Walk to the Departure Lounge early, **with the disk on you**, staying with Security or other crew. You are the most valuable target on the station.
6. When "Emergency Shuttle Arrival … You have 3 minutes to board" is announced, board through the Departure Lounge Airlocks. Prisoners go in the "Escape Shuttle Brig". Do a head count over the radio: each department reports who is aboard and who is missing.
7. **Don't authorise an early launch.** It takes three different command-access IDs at the shuttle's console. Allow it only if the shuttle itself is under attack.
8. Keep the disk on you until the round ends at CentCom.

## Leading the station (ongoing loop)

- **Orders**: one clear task per person, by name, on the right channel. Department matters go to their channel; heads of staff and the AI are on Command.
  - Example: "Chief Engineer, or Engineers if no CE: power on the Bridge is out, check the Bridge APC."
  - Follow the chain: you command heads, heads command their departments. Where a department has no head on shift, its crew report to you, or to the Head of Personnel for Service.
- **Delegate to the HoP**: access changes, job changes, Service, and the crew's paperwork.
  - The HoP's card cannot grant Captain access.
  - The HoP takes command if you die or disappear. Tell them where the disk is whenever that matters.
- **Monitor** from the Bridge every ~10 minutes and send help: **Crew Monitoring Console** (who is hurt or dead, and where, if suit sensors are on), **Station Alert** and **Bridge Power Monitoring** (fires, atmos alarms, power), **Security Cameras**.
- **Crew meeting**: once per shift, after the first 20-30 minutes. Announce a time and place (the Bar Lounge works: public and next to your quarters). Each department gives one line of status; then you set priorities, praise good work, and close within about 10 minutes. You can award a medal from the medal lockbox on your desk (Captain access).
- **Disputes**: hear both sides briefly, decide, state the decision on common, and move on. Space Law governs crimes. Security makes arrests, and you are the final authority on sentences and on any order to Security.
- **Authorising Security**:
  - Searches and arrests on blue.
  - Lethal force only against someone actively killing or armed and attacking.
  - Opening the **Armory** (you, or the Warden or Head of Security if on shift) only on red or when crew are being killed.
  - Say these authorisations explicitly on `:s`.
- **Keep moving** with the disk, and check your `inventory` now and then (disk, ID, remote).

## Emergencies

- **Someone is killing crew**:
  1. Find them: Crew Monitoring Console for the bodies, Security Cameras, and ask the AI to track them.
  2. On `:s`: description, location, and your authorisation (lethal force if they are killing).
  3. Raise blue at once, then red with the HoP.
  4. Announce which area to avoid and who to report sightings to.
  5. Arm Security from the Armory if they are outgunned. Send Medical in only behind Security.
  6. Stay with armed crew; never go after them alone.
  7. Afterwards: the brig, recover stolen gear, lower the alert.
- **The AI is damaged or silent**: doors still work with IDs, but nobody watches the cameras or opens doors remotely. Send Engineers to the AI Chamber in the AI Satellite (through the Transit Tube from Engineering). If the AI turns on the crew (bolting people in, shocked doors, turrets, ignoring orders): declare red alert, warn the crew not to trust doors, and keep people out of its reach. If it threatens the whole station, evacuate.
- **Power failure**: check the Bridge Power Monitoring Console and Station Alert. Order Engineering (Supermatter and grid) and Atmospherics as needed, and announce it. If the Bridge console is dark, use the one in your office.
- **Breach or fire**: send Atmospherics and Engineering. Announce the area to avoid and keep people out until it's sealed. Large areas depressurised or burning is a reason to evacuate.
- **Radio down** (telecomms): priority announcements still reach everyone (30 s cooldown); use them for orders. Send Engineering to Telecomms.
- **ID stolen**:
  - Announce at once on common that anything announced or done with your card is not you.
  - Get the spare ID: the safe in the command pit. Click it, enter your 5 digits with `keypad {digit}`, then `E` (`C` locks it again).
  - If you can't get onto the Bridge, the AI or the HoP opens doors for you.
  - Have Security recover your card.
- **You are hurt**: medkit and first aid station on the Bridge, otherwise Medbay. Hand off command to the HoP on Command if you'll be out of action.

## Defending yourself

You are the station's most-wanted target: the disk, the all-access ID, the hand tele, the antique gun. Shared combat mechanics are in crew-basics. Your own means:

- **Officer's sabre** (from the sabre sheath on your belt): 20 brute damage per hit with armour penetration 75, and **1.35× damage against assistants**.
  - While it is in your hand, you block 50% of melee attacks. It doesn't block projectiles.
  - Alt-click the worn sheath to draw it quickly.
  - The sheath also gives a **Counterattack** action button: click it, then click an attacker. If they hit you in melee within the next second, you draw and strike for 3× the sabre's force. A failed counterattack has a 60 s cooldown.
- **Energy gun** (suit storage): two modes, switched by using it in hand.
  - **disable** (starting mode): 30 stamina damage per shot, 20 shots.
  - **kill**: 25 burn per shot, 12 shots.

  Recharge it at the rechargers on the Bridge or by your bed.
- **Gold-capped telescopic baton** (backpack): use it in hand to extend it.
  - A normal click knocks the target down for 1.5 s and deals 55 stamina damage (gets through most armour). Two hits floor them.
  - It has a 4 s cooldown between stuns.
  - A right-click is a plain 10-damage hit.
- **Handcuffs**: two pairs on the Bridge. Cuff a downed or stunned attacker, then call Security.
- **Armour**: carapace, hat, insulated gloves; the sunglasses stop flashes and the bowman headset stops flashbang deafness. The magnate MODsuit in your suit storage unit is better armour, but it takes your back slot.
- **Antique laser gun**: only if the station is being lost. Breaking the case sets off an alarm.

**When to fight**:
- Defend yourself and the disk.
- Use non-lethal means first: the disabler mode, or the baton, then cuffs.
- Use lethal force only against someone killing or armed and attacking.

Otherwise give the orders, let Security make the arrest, and stay alive: a dead Captain loses the disk and the ID to whoever loots the body. If you're outmatched, retreat to armed crew and keep the disk away from the attacker.

## Working with the crew

| Role | You give | You need |
|---|---|---|
| Head of Personnel | Delegation (access, jobs, Service), red alert partner, command when you're gone | Staffing reports, access fixes, a second keycard |
| Security Officers | Clear authorisations, priorities, suspect details | Disk and ID recovery, escorts, arrests, holding Departures |
| Station Engineers | Power and repair priorities | Engine and power status, door and breach repairs, telecomms and AI repairs |
| Atmospheric Technician | Breach and fire priorities | Air, fire and breach status |
| Medical Doctors, Chemist | Where casualties are (crew monitor) | Treatment, revival, casualty counts |
| Scientist | Research priorities that help other departments | Upgrades and equipment |
| Quartermaster | Approval for big orders, a second keycard if needed | Supply status, budget |
| Cook, Botanist, Janitor | Recognition, meeting invitations | Food, cleanup after fights |
| The AI | Orders (doors, tracking, announcements) | Door control, camera tracking, warnings |
| Any other head who joins | Priorities; they run their department | Reports over Command |

## Through the client

- **Comms console**:
  1. Click the console, then `tgui_act toggleAuthentication`.
  2. `tgui_act makePriorityAnnouncement` opens a second window (the text box).
  3. Answer it with `tgui_act submit {entry: "your text"}`.

  For alert changes, take the ID from your ID slot into your active hand, `tgui_act changeSecurityLevel {newSecurityLevel: "blue"}`, then put the ID back at once.
- **Radio window**: `drag` your worn headset onto yourself to open "Radio", then `tgui_act channel {channel: "Engineering"}` (or "Medical", "Science", "Supply", "Service"). `say {radio: "engineering"}` sends nothing while that channel is off.
- **Keycard device**: click it to open "KeycardAuth"; the actions are `red_alert`, `emergency_maint` and `auth_swipe`. You must stand next to it.
- **Spare ID safe**: click it to open "LockedSafe", send `keypad {digit: "1"}` once per digit, then `{digit: "E"}`, then click the safe again to open its storage.
- **Your quarters**: `walk_to {area: "Captain's Quarters"}` dithered at the door yesterday. Use `walk_to` with the communications console's `object_id` instead, or `move` into the airlock. A windoor that refuses you is access-locked ("the game refused the step").
- **Stripping a restrained thief**: `drag` their mob onto yourself to open their strip menu, then `tgui_act` on the slot. Stay next to them until it finishes.
- **Items in hand**: `key Z` uses the item in your active hand (extends the baton, turns on the pinpointer, cycles the remote's mode, switches the energy gun's mode).
- `search` doesn't see inside closets, bags or someone's hands. Open containers first, and use the pinpointer for the disk.

## Dangers and common mistakes (yesterday's shift)

- She stood talking near thieves: first the ID was stripped, then the disk. **Don't stand still next to anyone you don't trust; step away when chat says someone "tries to remove your …".**
- Without the ID she was trapped in her quarters for 47 minutes. **Carry the door remote; ask the AI.**
- A thief used her card for a fake Captain's Announcement. **Deny fakes on common at once.**
- A right-click with a crowbar in hand hit a crewmate. **Empty your hand before shoving.**
- Her Engineering radio lines went nowhere: the channel was off. **Turn channels on first.**
- She chased thieves alone. **Give Security the facts and the authorisation instead.**

## Checklist

**Shift start**: disk and pinpointer from the bedroom → locker (sheath on belt, energy gun in suit storage, door remote in a pocket, hand tele locked away) → read the spare ID code → radio channels on → welcome announcement → heads and departments report in.

**Every ~10 minutes**:
- `inventory` (disk, ID, remote);
- keep moving;
- read the radio and answer;
- Bridge consoles (crew monitor, alerts, power);
- one clear order per problem;
- recall any shuttle called without a reason.

**When it's time** (unplayable, or ~90 min of shift time): call the shuttle → announce → assign evacuation jobs → reminders → board with the disk.

## Sources

- tgstation code (commit 54c22023): the Captain job and ID trim, the communications console (DM and tgui), the keycard device and alert levels, the shuttle subsystem and emergency shuttle, the disk and pinpointer, safes, lockers, the display case, the door remote, the sabre, baton and radio code, the stat panel, and `config/game_options.txt`.
- Map: MetaStation.dmm, metastation.json, emergency_meta.dmm.
- Yesterday's round: the reports of the Captain, the HoP and both assistants.
- /tg/station wiki (CC BY-SA 3.0): Captain, Nuclear_Authentication_Disk, Standard_Operating_Procedure.
