# Head of Personnel (HoP)

## The job in one paragraph
You run the station's ID cards. You add and remove access, change job titles, move people to new jobs, and strip access from troublemakers. You are also head of Service, the Captain's second in command, and Ian the corgi's keeper.

Success looks like this:
- The HoP line is open, and requests are answered within minutes.
- Reasonable requests are granted correctly; nobody gets access they shouldn't.
- Service has what it needs and Ian survives.
- You are ready to take command if the Captain falls.

Yesterday's HoP issued zero access changes all shift. The desk is the job: be at it, announce it, process requests.

## Starting kit and access
**Worn:**
- head of personnel's jumpsuit, HoP cap, laceup shoes
- **head of personnel's coat**: an armor vest covering chest, groin and arms
- **the head of personnel's headset**
- **head of personnel PDA** on your belt
- **platinum identification card** in your ID slot

**Backpack:** survival box and a **silver-capped telescopic baton**.

**Headset:** Command `:c`, Service `:v`, Common `;` (radio keys for `say`).

**Your access:** Personal Lockers, Auxiliary Base, Bar, Brig (front doors), Department Budget, Cargo Bay, Chapel Office, ID Console, Crematorium, Command (the Bridge), Courtroom, Engineering, EVA, Gateway, Hydroponics, Custodial Closet, Keycode Auth., Kitchen, Law Office, Library, Maintenance, Medical, Mineral Storage, Morgue, Coroner, Psychology, RC Announcements, R&D Lab, Service Hallway, Teleporter, Theatre, Weapon Permit, AI Chambers, HoP Office.

You do **not** have Security, Atmospherics, Power and Engineering Equipment, Technical Storage, Science, Robotics, Pharmacy, Surgery, Virology, Main Vault or Captain.

**Head of personnel's locker** (in your office):
- **energy gun**, **handheld flash**, **service door remote**
- **box of spare IDs** (7 grey cards), **box of spare silver IDs** (7 silver cards)
- **jumbo dog bone**, **pet carrier**, pet collar
- command megaphone, spare headset, box of rubber stamps, medal boxes
- a Departmental Techfab - Service board

**PDA apps** besides the crew ones (Direct Messenger, crew manifest, NT Pay): security records, **Plexagon HR Core** (job slots), status display, NT Shopping Network (department orders).

## Where things are on MetaStation
**Head of Personnel's Office** sits between the **Central Primary Hallway** (west) and the **Bridge** (east). It has two "Head of Personnel" airlocks (HoP Office access): the west one onto the Central Primary Hallway, the east one into the Bridge. If one is blocked, use the other.

- **Your desk (south side):**
  - Your office chair (a spawn point). The **identification console** (ID console) is just west of it, then a **security records console**.
  - South of the chair is the desk. It is a reinforced table with a desk bell and two windoors: **"Head of Personnel's Desk"** on your side (HoP Office access) and **"Reception Window"** on the customer side (anyone).
  - **Privacy Shutters** cover the desk and the office windows.
- **Table east of your chair:**
  - On it: the **HoP's rubber stamp**, a carbon-paper bin, a pen.
  - On the wall: **Privacy Shutters Control**, **Queue Shutters Control**, **increment ticket counter**, and the photobooth button.
  - The **flasher button** for the queue is on the wall at your chair.
- **North wall:** **PTech** (PDA vendor), **Tablet & ID Painter** (changes a card's job trim), **Head of Personnel's Requests Console**, **Ian's dog bed** (with Ian), filing cabinet.
- **East wall:** **Keycard Authentication Device**.
- **Middle:** the HoP's fax machine, a photocopier, the office APC (north wall).
- **South-west:** your **locker**, a disposal bin, package wrap, hand labeler.
- **North-west back room**, behind the windoor **"HoP's Desk"** (HoP Office access):
  - account lookup console, cargo request console
  - a table with a **handheld flash**
  - a **recharger** (for the energy gun)
  - another Privacy Shutters Control (a third is on the office's west wall)

**The HoP line:**
- South of the desk is a queue strip in the **Command Hallway**.
- The queue has two openings with **HoP Queue Shutters**: the west one is the entrance, the east one (at the desk) is the exit.
- A **ticket machine** is by the entrance.
- A **mounted flash** in the queue wall fires from your flasher button: 2-tile range, about 5 s stun, 15 s recharge.

**Elsewhere:**
- The **Bridge** has its own **identification console** in its north-west corner: your backup.
- The Captain's Quarters and each head's office have ID consoles too (heads are limited to their own department).
- The Bridge's **communications console** is in the middle of the Bridge, with the **Captain's spare ID safe** next to it.
- Evacuation leaves from the **Departure Lounge**.

## How ID cards work (read before touching the console)
Every card has a **trim** (its job, e.g. "Station Engineer": the icon and the HUD job) and a list of accesses.
- Accesses in the card's own trim are **basic**: free and unlimited.
- **Every other access is a wildcard** and uses a slot of its level:

| Card | Who gets it | Common | Command | Private Command | Captain |
|---|---|---|---|---|---|
| grey identification card | almost every job; box of spare IDs | 4 | 0 | 0 | 0 |
| silver identification card | heads of staff (CE, CMO, RD, HoS, QM); box of silver IDs | 6 | 2 | 1 | 0 |
| platinum identification card | you | unlimited | 2 | 1 (taken by your HoP Office) | 0 |
| gold identification card | Captain, Captain's spare ID | unlimited, any level | | | |

A Command slot also takes Common accesses. A Private Command slot takes Command and Common ones too.

**Access levels:**
- **Command:** Command (Bridge), AI Chambers, Teleporter, Keycode Auth., RC Announcements, ID Console, Personal Lockers, Armory, AI Satellite, Telecommunications, Main Vault. EVA and Department Budget are listed under both Common and Command in the code; a wildcard's label in the console names its level, e.g. "EVA (Command)".
- **Private Command:** HoP Office, CE Office, CMO Office, HoS Office, QM Office, RD Office.
- **Captain:** only "Captain".
- **Everything else is Common.**

What follows from this:
- **Captain access only fits on a gold card.** Nothing you print can hold it. That is why yesterday's HoP "couldn't grant the Captain's quarters access". A Captain who loses their ID needs the **spare ID in the Bridge safe** (they have its code).
- **A grey card takes only 4 extra Common accesses, and no Command ones.** Anything bigger is a **job change** (procedure B): the new trim makes the job's accesses basic.
- **A template only adds accesses that are in the card's trim.** The "Station Engineer" template on an Assistant's card mostly wipes it. Imprint the trim first.
- **Skeleton crew:** if fewer than 20 players were ready at round start, every job also gets its extra accesses. The spawn message says "additional access may have been added". Templates follow the same rule. In the access table below, * marks these extras.

## The ID console: Plexagon Access Management
The identification console runs NtOS with **Plexagon Access Management** (`plexagonidwriter`), **Plexagon HR Core** (`plexagoncore`), **Plexagon Crew List** (`plexagoncrew`) and a chat client. It has two slots:
- **main slot:** your ID, which logs you in
- **secondary slot:** the card you edit

Your ID Console access gives full rights: every station access and every template.

| tgui action (`NtosCard`) | Params | Effect |
|---|---|---|
| `PRG_insert_main_id` | none | ID **in your active hand** into the main slot |
| `PRG_authenticate` | none | Log In with the main-slot card |
| `PRG_insert_alt_id` | none | ID in your active hand into the secondary slot |
| `PRG_access` | `access_target`: ref (e.g. `"maint_tunnels"`); optional `access_wildcard`: `"Common"`, `"Command"`, `"Private Command"` | toggles that access on the secondary card (wildcards take the first free fitting slot) |
| `PRG_template` | `name`: job title (`"Botanist"`) | wipes access, then adds the job's accesses that are in the card's trim; needs a trimmed card |
| `PRG_assign` | `assignment`: text | job title shown on the card (no access change; security HUDs still show the trim's icon) |
| `PRG_edit` | `name`: text | registered name (letters and numbers; empty clears it) |
| `PRG_age` | `id_age`: 17-85 | age |
| `PRG_terminate` | none | "Terminate Employment": title "Demoted", trim and **all** access removed |
| `PRG_print` | none | prints an access report (needs paper) |
| `PRG_remove_alt_id` / `PRG_remove_main_id` | none | eject that card to your hand |
| `PRG_logout` | none | Log Out |

NtOS frame actions: `PC_runprogram {name}`, `PC_exit`, `PC_minimize`.

What the window shows:
- `data.authed_user`: who is logged in.
- `data.modified_card` (and `auth_card`): `id_owner`, `id_rank`, `trim_assignment`, `trim_access`, `access_on_card`, and `wildcard_slots` (`limit`, `usage`; -1 means unlimited).
- `data.regions`: every access as `{desc, ref}` under General, Security, Medbay, Research, Engineering, Supply, Command.
- `data.templates`: the job names.

**Critical:**
- Ejecting your ID or closing the program does **not** log you out. Only `PRG_logout` does.
- A console left logged in gives anyone full rights.
- An add that changes nothing means no free slot of that level. It fails silently, so check `wildcard_slots`.

## Core procedures
**Opening the line:**
1. `load_map`, then `walk_to {area: "Head of Personnel's Office"}`.
2. Open the locker. Take the energy gun, flash and dog bone. Befriend Ian.
3. Click the ID console (the first click may only power it on). `PC_runprogram {name: "plexagonidwriter"}`.
4. Hold your ID, `PRG_insert_main_id`, then `PRG_authenticate`.
5. Announce on Common, e.g. `say ";HoP line open at the Command Hallway desk: access, job changes, titles."`. Make a station announcement too (see Paperwork).
6. Wait in your chair tile with `wait {until/from_others}`.

**Card hand-off across the desk:**
- The customer clicks the **Reception Window** to open it, then puts the card on the desk table.
- You open the **Head of Personnel's Desk** windoor and pick the card up.
- Windoors close by themselves after about 6 s.
- Return the card the same way.
- If their ID is inside their PDA, they eject it first (alt-click the PDA).

**A. Add or remove one access:**
1. `PRG_insert_alt_id`.
2. Read `data.modified_card`.
3. `PRG_access {access_target: "<ref>"}`. Check that the ref appears in, or leaves, `access_on_card`.
4. `PRG_remove_alt_id`, return the card, report on Command.

A full grey card needs a wildcard removed before another fits.

**B. Job change** (e.g. Assistant to Botanist):
1. Get approval: the department's head if one is on shift, else the Captain.
2. Click the **Tablet & ID Painter** with the card to insert it. Click it empty-handed to open the `PaintingMachine` window.
3. `trim_card {selection: "Botanist"}` (Imprint ID Trim). This **wipes all access** and sets the title.
   - Head trims need a **silver** card; the Captain trim needs **gold**. A wrong card gets "You will need a rarer ID card to imprint that trim data."
4. `eject_card`, then insert the card in the console's secondary slot.
5. `PRG_template {name: "Botanist"}`. Add any extra wildcards.
6. Optionally `PRG_assign` a title. Then `PC_exit` with the card still in the slot to update the crew manifest. Eject and return it.

**C. Titles and names:**
- `PRG_assign {assignment: "Chief Sandwich Officer"}` changes no access. Grant these freely (keep them inoffensive).
- `PRG_edit` (names) only for a real reason, such as a typo or a Captain-approved alias: fake names are how impostors work.

**D. Demotion:**
- To remove one abused access, use `PRG_access` on it.
- A full demotion needs an order from the Captain, the person's department head, or Security for a crime:
  1. `PRG_terminate`.
  2. To keep them as an Assistant: imprint the **Assistant** trim, then `PRG_template {name: "Assistant"}`.
  3. Announce it on Command, and tell the department so they can recover gear.
- If the person won't hand over their card, Security takes it; don't wrestle them for it yourself.

**E. New card** (lost ID, or no ID):
1. Take a grey card from the box (silver for a head).
2. Imprint the trim.
3. `PRG_edit {name}`, then `PRG_template {name: "<job>"}`.

Box cards have no bank account linked.

**F. Your own card:**
1. Log in, then `PRG_remove_main_id` (you stay logged in).
2. `PRG_insert_alt_id` your card and edit it.
3. `PRG_remove_alt_id`, then `PRG_logout`.

Your platinum card takes unlimited Common accesses but only 2 Command ones. Give yourself only what an emergency needs and say so on Command. Access is not permission: Security arrests HoPs who wander into the Armory.

**G. Job slots** (Plexagon HR Core, `NtosJobManager`, on the console or your PDA): your ID must be in that computer's main slot (no login).
- `PRG_open_job {target: "<job title>"}` adds a slot.
- `PRG_close_job {target}` removes one.
- `PRG_priority {target}` marks the job as wanted in the join menu (up to 5 jobs).

A job opens only while its slots are at most 30% of the players connected. There is a 30 s cooldown (`data.cooldown`). Players can join at any time: open slots the station needs (Medical Doctor after deaths, Station Engineer in an engine crisis) and close slots being abused.

## Access reference
\* = only with skeleton-crew extras. Level: C = Common, Cmd = Command.

| Console label (ref) | Lvl | Opens on MetaStation | Normally held by |
|---|---|---|---|
| Maintenance (`maint_tunnels`) | C | maintenance tunnels | Station Engineer, Atmospheric Technician, Janitor, Quartermaster, Cargo Technician, Paramedic, HoP; Assistant\*, Security Officer\* |
| Engineering (`engineering`) | C | Engineering Foyer, Engine Room, Supermatter Engine Room | Station Engineer, Atmospheric Technician, CE, HoP |
| Construction (`construction`) | C | Engineering Foyer, Gravity Generator Room | Station Engineer, Atmospheric Technician, CE, RD |
| Power and Engineering Equipment (`engine_equip`) | C | Engineering Storage, APCs, engineering lockers | Station Engineer, CE; Atmospheric Technician\* |
| Atmospherics (`atmospherics`) | C | Atmospherics, air alarms | Atmospheric Technician, CE; Station Engineer\* |
| Technical Storage (`tech_storage`) | C | Tech Storage (Secure Tech Storage also needs Command) | Station Engineer, CE, RD, Roboticist |
| External Airlocks (`external airlocks`) | C | airlocks to space | Station Engineer, Atmospheric Technician, CE, Paramedic |
| Telecommunications / AI Satellite (`tcomms` / `minisat`) | Cmd | Telecomms Storage / MiniSat access | Station Engineer, CE |
| Medical (`medical`) | C | Medbay Central, Treatment Center, Medbay Storage | Medical Doctor, Chemist, Paramedic, CMO, Coroner, Psychologist, HoP |
| Surgery (`surgery`) | C | surgical theatres, Medical Cold Room | Medical Doctor, CMO, Coroner; Chemist\* |
| Chemistry Lab (`plumbing`) | C | Chemistry | Chemist, CMO; Medical Doctor\* |
| Pharmacy (`pharmacy`) | C | Pharmacy, Chemical Storage | Chemist, Medical Doctor, CMO |
| Virology (`virology`) | C | Virology | Medical Doctor, CMO; Chemist\* |
| Morgue (`morgue`) | C | Morgue (its Medbay-side door also needs Medical) | Medical Doctor, Cook, Coroner, Chaplain, CMO, HoP; Botanist\*, Security Officer\*, Chemist\* |
| Coroner (`morgue_secure`) | C | Coroner's Office | Coroner, CMO, Detective, HoP |
| R&D Lab (`science`) | C | Research Division, R&D Lab | Scientist, Roboticist, Geneticist, RD, HoP |
| Science (`research`) | C | Testing Labs, science lockers | Scientist, Roboticist, Geneticist, RD |
| Robotics / Genetics Lab / Xenobiology Lab / Ordnance Lab | C | those labs | RD and science jobs (Scientist: Xenobiology, Ordnance; Robotics\*, Genetics\*) |
| Cargo Bay (`cargo`) | C | Cargo Lobby, Cargo Bay, Warehouse | Quartermaster, Cargo Technician, Shaft Miner, HoP |
| Cargo Shipping / Mining Dock (`shipping` / `mining`) | C | Delivery Office / Mining Office | Quartermaster, Cargo Technician / Shaft Miner |
| Kitchen (`kitchen`) | C | Kitchen, Kitchen Cold Room | Cook, HoP; Bartender\*, Botanist\* |
| Bar (`bar`) | C | Bar, Bar Backroom, also the Kitchen door | Bartender, HoP; Cook\*, Botanist\* |
| Hydroponics (`hydroponics`) | C | Hydroponics | Botanist, HoP; Cook\*, Bartender\* |
| Custodial Closet (`janitor`) | C | janitor's room | Janitor, HoP |
| Service Hallway (`service`) | C | Service Hallway | all Service jobs, HoP |
| Theatre, Library, Chapel Office, Crematorium, Law Office | C | those rooms | Clown/Mime, Curator, Chaplain, Lawyer; HoP |
| Security, Holding Cells, Brig, Courtroom, Weapon Permit | C | Security and brig; Weapon Permit lets you carry weapons past secbots | Security Officer, Warden, Detective, HoS (HoP: Brig, Courtroom, Weapon Permit) |
| Command (`command`), EVA (`eva`) | Cmd | the Bridge, EVA Storage | heads of staff |
| Teleporter, AI Chambers, Main Vault, Armory, ID Console, Keycode Auth. | Cmd | those rooms and devices | heads only (Armory: Warden, HoS; Main Vault: QM) |

## When to say no
- **Never:**
  - ID Console access
  - all-access
  - "Captain" (impossible anyway)
  - Security, Armory or Weapon Permit without the HoS, Warden or Captain agreeing
- **Captain's approval required:** Command-level access, head trims, silver cards.
- **Department access:** ask the department's head on Command when a CE, CMO, RD, HoS or QM is on shift. If nobody heads it, ask the crew working there or use judgment.
  - Fine without asking: an access someone's own job needs, and maintenance for an Assistant.
- **Refuse:**
  - anyone who has attacked crew, is wanted, is masked, or holds a card that isn't theirs
  - anyone with no reason, or a reason that fits an attack (Atmospherics or Ordnance for an Assistant, AI Chambers for anyone)
- Refuse politely and offer something else ("the Chemist can hand you pills"). A fun title is a good consolation.

## Head of Service
Service is the Cook, Botanist and Janitor, plus a Bartender, Chaplain, Curator, Lawyer, Clown, Mime or Psychologist when on shift; players can join in any job at any time. Talk on `:v`.
- Check early that the Kitchen has ingredients, Hydroponics has seeds and nutrients, and the Janitor has their cart.
- Order supplies through Cargo with the back-room cargo request console or the PDA's NT Shopping Network (Service budget).
- **Janitor keys:** at any Keycard Authentication Device, a head's `give_janitor_access` gives the Janitor's access key ring the Service region for 10 minutes (30 s cooldown).
- Grant Service accesses (Bar, Kitchen, Hydroponics) yourself: you are their head. If a Service job is empty, open its slot or cover the basics.
- A Service Techfab already stands in the Service Hallway. Your locker board can build another (an engineer or scientist does it).

## Second in command, keycard, evacuation
**Chain of command:** Captain, you, RD, CE, CMO, HoS, QM. Stay in touch with the Captain on Command and take over desk-bound work.

**Acting captain:**
- If there was no Captain when the round started (or when you joined), you are promoted automatically. A notice tells you, and a confidential folder with the **spare ID safe code** lands in your pocket, backpack or hands.
- If the Captain dies or goes missing mid-shift, announce on Common that you are taking command.
- Then take their ID, or the spare from the Bridge safe (the Captain has the code), and secure the nuclear authentication disk.

**Communications console** (Bridge): log in with `toggleAuthentication` (Command access, which you have).
- Logged in, you can `callShuttle {reason}` (12+ characters) and `recallShuttle`.
- Alert level changes, priority announcements and emergency maintenance access need Captain access.

**Keycard Authentication Device** (yours on the east wall; others on the Bridge, in the Captain's Quarters and in each head's office):
1. One head presses **Red Alert** (`red_alert`), **Emergency Maintenance Access** (`emergency_maint`) or **Bluespace Artillery Unlock** (`bsa_unlock`).
2. A second head presses **Authorize** (`auth_swipe`) on a **different** device **within 2 seconds**.

Count down on the radio first. Red Alert is for a confirmed lethal threat; Emergency Maintenance Access is for trapped crew.

**Evacuation:** there is no scheduled evacuation.
- The Captain calls the emergency shuttle only if the round becomes unplayable (station being destroyed, most of the crew dead, a threat nobody can stop) or after about 90 minutes of round time (stat panel, Status tab).
- The Captain recalls any call by someone else that has no such reason.
- As acting captain, those calls and recalls are yours. If the Captain is unavailable and someone calls without reason, recall it and report.
- Timing:
  - No call is possible in the first 20 minutes.
  - At green the shuttle arrives 20 min after the call and can be recalled until 10 min remain. At blue: 10 min, recallable until 5. At red: 5 min, recallable until 2.5.
  - It stays docked 3 minutes.
- When a real call stands:
  1. Help the Captain get everyone to the **Departure Lounge**: relay the ETA and check Service is moving.
  2. Log out and take your ID.
  3. Bring Ian.

## Ian
Ian is a corgi in your office's dog bed. If he died last shift, he is a puppy named Ian. Keep him alive and get him onto the shuttle.
- **Befriend him:** click Ian with the **jumbo dog bone** (not in combat mode). It fully heals him, befriends you, and is used up.
- **Commands:** a friend's spoken lines within his sight steer him.
  - Lines containing "heel" or "follow": he follows you.
  - "sit", "stay" or "stop": he stays.
  - "free" or "loose": he goes free.
  - The words match anywhere in a sentence ("stop that man" makes him sit).
- **Pet carrier:** hold it open and click Ian (3 s) to load him. Use it in hand to close it. To let him out, open it and drag it onto a floor tile.
- Keep the office doors shut; he can't open them. Don't let anyone carry him off.

## Paperwork and messages
- **Stamp:** hold the HoP's rubber stamp and right-click a paper.
- **Write:** hold a pen and click a paper (`PaperSheet` window), then `add_text {text}`.
- **Station announcement:** click the Head of Personnel's Requests Console with your ID in hand. Then open it empty-handed and send `send_announcement {message}`. Your ID has RC Announcements; there is a 30 s cooldown, and you swipe again for each announcement.
- **PDA message:** `PC_runprogram {name: "nt_messenger"}`, then `PDA_sendMessage {ref, message}`. Use it when the radio fails or for private matters.
- Report each change on Command (who, what, who approved): that is your record.

## Dangers and common mistakes
- **Console left logged in.** `PRG_logout` every time you leave the chair.
- **Losing your card.** It can rewrite any card on the station. Keep it in your ID slot unless it's in the console, and never lend it.
- **A template on a card with another trim** wipes the card.
- **Promising Captain access.** Only gold cards can hold it.
- **Yesterday:**
  - Two Assistants shoved the HoP into a disposal unit and demanded all access.
  - One walled up the office; walk_to bounced between the Bridge and the office for minutes.
  - The borrowed welder was empty.
  - Nothing was issued all shift.

  Fixes: shutters ready, flash and baton at hand, the Bridge console as fallback, fuel checked before relying on a welder.
- **Moved between calls.** If `status` shows you elsewhere, go back and check your ID and the console.

## Emergencies
- **Power failure:** the console and painter need power (office APC on the north wall). Call an engineer. HR Core on your PDA still works.
- **Breach or fire nearby:** close the privacy shutters, put Ian in the carrier, leave by the other door, report.
- **Mass casualties:** open Medical Doctor and Station Engineer slots. Grant Medical or Morgue to body carriers if the CMO (or the doctors, when there is no CMO) agree.
- **Attacker:** call Security on Common with name, place and weapon; see the next section.

## Defending yourself and the console
**Kit:**
- **Silver-capped telescopic baton** (backpack): extend it by using it in hand (Z).
  - Left-click a person to stun: stamina damage, a short knockdown, 30% armor penetration, 4 s cooldown. Two hits floor most people.
  - Right-click is a plain 10-damage hit.
- **Energy gun** (locker): starts on **disable** (stamina beams, 20 shots; about 4 hits drop someone).
  - Use it in hand to switch to **kill** (12 shots), only when a life is at stake.
  - Recharge it in the back room.
- **Handheld flashes:**
  - Click an adjacent person who faces you: a long knockdown, unless they wear sunglasses or welding gear.
  - Used in hand, it only confuses everyone nearby.
  - Overuse burns it out.
- **Queue flash** (flasher button): stuns everyone within 2 tiles of it.
- **Service door remote:** click a door at range.
  - It works on powered doors that Service access or your own access opens, except doors in the Bridge, Security, the Vault and AI areas.
  - Using it in hand cycles Open Door, Toggle Bolts, Toggle Emergency Access.
  - Bolt your office doors to keep intruders out.

**Guarding the desk:**
- Customers stay on their side. Never open your windoor for someone who demands rather than asks.
- **Queue Shutters Control** seals the queue; **Privacy Shutters Control** seals the desk and windows. Use them when the line turns into a mob or a window breaks.
- If someone gets in: log out, flash, then baton, and call Security.
- If you're overpowered: keep your card, log out, leave by the other door. A console without your card is harmless. A lost card is a disaster: report it on Command at once.
- Stand your ground for the console, your card and Ian. For anything else, call Security and step back.

Combat mode, shoving, grabs and resisting are in crew-basics.

## Walled up or locked out
1. Use the other door: west from the Central Primary Hallway, east from the Bridge.
2. If the desk is cut off, work at the **Bridge identification console** (north-west corner of the Bridge).
3. **A plain wall** built by a player: ask an engineer, or use a welding tool yourself.
   - Examine the welder for fuel first; refill at a welding fuel tank.
   - Light it in hand and click the wall: about 10 s, leaving a girder.
   - Wrench the girder (4 s) to loosen it, then push it aside or screwdriver it apart (4 s). Girders can't be welded apart.
4. A **reinforced wall**, or a bolted or unpowered door: ask an engineer, or ask the AI to open the door.

## Working with the crew
- **Captain:** your boss. Approves Command access, silver cards and head trims; calls the evacuation. Report important changes.
- **Security Officers:** bring cards for demotion and back up your refusals. Ask before granting Security access. Report all-access and weapon seekers to them.
- **Department heads** (CE, CMO, RD, HoS, QM when on shift): outrank you in their departments and have limited ID consoles. Ask before adding people to their departments.
- **Station Engineers and the Atmospheric Technician:** get the engineering access their work needs. They cut walls and restore power for you.
- **Medical Doctors and the Chemist:** Surgery, Pharmacy and Morgue inside medbay as needed.
- **Scientist:** Robotics or Genetics for research.
- **Quartermaster:** heads Supply. Ask before granting Cargo Bay or Mining Dock. Service orders go through them.
- **Cook, Botanist, Janitor:** your department. Access, supplies, the janitor's keys.
- **AI:** opens and bolts doors on request and watches your office cameras.
- **Players you don't know:** more can join at any time, in any job. Check that their card's trim and name match their story.

## Through the client
- If `walk_to` bounces or says "no progress" near the office, a door or a new wall blocks it: `look` and use the other door.
- Click the console empty-handed (twice if it was off). Don't right-click it empty-handed: that toggles "frame" mode.
- Every `PRG_insert_*` needs the card **in your active hand**. Take your ID out of the ID slot by clicking it in your inventory with an empty hand; click the slot while holding it to put it back.
- Before and after each change, read `tgui_window {path: "data.modified_card"}`. Find refs with `tgui_window {path: "data.regions", find: "Hydroponics"}`.
- `data_changes: none` after `PRG_access` means no free slot or a wrong ref.
- The customer stands 2 tiles away, so give (G) doesn't reach: use the desk table.
- To mute Ian, give `mute` a full phrase like `"Ian barks"`; it is a plain substring match.
- If the radio fails, use Direct Messenger, the requests console, or walk over.

## Checklist
**Shift start:**
1. `load_map`, go to the office.
2. Gun, flash, bone; befriend Ian.
3. Console on, logged in.
4. Announce the line on Common and on the requests console. Say hello on `:c` and `:v`.
5. Glance at HR Core.

**Loop:**
1. Wait at the desk, listening to Common, Command and Service.
2. Per request: identify the person, check the reason, get approval if needed, apply A-G, return the card, report on Command.
3. Every ~15 min: check on Service, Ian and the Captain. Log out whenever you leave.
4. When a real shuttle call stands: help move the crew to the Departure Lounge, log out, take your ID and Ian.

## Sources
- Code, tgstation 54c22023:
  - `code/modules/jobs/job_types/head_of_personnel.dm`, `_job.dm`
  - `code/datums/id_trim/jobs.dm`
  - `code/__DEFINES/access.dm`, `id_cards.dm`
  - `code/controllers/subsystem/networks/id_access.dm`, `job.dm`, `shuttle.dm`
  - `code/game/objects/items/cards_ids.dm`
  - `code/modules/modular_computers/file_system/programs/card.dm`, `jobmanagement.dm`
  - `code/game/machinery/PDApainter.dm`
  - `closets/secure/security.dm`
  - `melee/baton.dm`, `assembly/flash.dm`, `machinery/flasher.dm`, `tools/control_wand.dm`
  - `security_levels/keycard_authentication.dm`, `computer/communications.dm`
  - `pets/dog/_dog.dm`, `corgi.dm`, `pet_carrier.dm`
  - `requests_console.dm`, `paperwork/paper.dm`
  - `turfs/closed/walls.dm`, `structures/girders.dm`
  - `config/game_options.txt`, `config.txt`
- tgui: `NtosCard.tsx`, `common/AccessList.jsx`, `PaintingMachine.jsx`, `NtosJobManager.jsx`, `KeycardAuth.jsx`, `NtosMain.tsx`.
- Map: `_maps/map_files/MetaStation/MetaStation.dmm`, `_maps/map_jsons/metastation.json`.
- Wiki: /tg/station wiki "Head_of_Personnel" (Internet Archive, 2026-02-06), CC BY-SA 3.0.
- Yesterday's round: `seeker-play/play/crew/runs/12-hop/report.md`, `transcript.jsonl` (grepped).
