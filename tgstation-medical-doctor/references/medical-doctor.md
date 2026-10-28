# Medical Doctor

Shared by two Medical Doctors: **Doctor A** (treatment, surgery and revival lead, works in medbay) and **Doctor B**
(field medic: crew monitor, retrieval, triage). Both should know all of it. Facts here are checked against this
server's game code and the MetaStation map. Where the /tg/station wiki says otherwise, the code wins.

## 1. The job in one paragraph

Keep the crew alive and bring the dead back. In practice: get medbay ready at shift start (defibrillators mounted,
tools laid out, the Chemist's stock in reach), treat walk-ins in the clinic, find and fetch the badly hurt and the
dead (crew monitor, radio), and revive every body that reaches you in time. Revival is a race against the
**heart, which rots to "Non-Functional" about 6 minutes after death** unless you stop the rot (stasis bed,
formaldehyde from an epinephrine medipen, cold). Yesterday all three deaths ended with "heart too damaged": nobody
stopped the rot and nobody repaired the heart. Success: every death on the station gets a doctor and a fixed,
shocked heart before it is too late. If a Chief Medical Officer is on shift, they are your boss; paramedics, a
coroner or more doctors may join too. The crew list you were given is not exhaustive: more players can join at any
time, in any job.

## 2. Starting kit and access

Worn: medical doctor's jumpsuit, **labcoat** (penlight in its suit storage), white sneakers, **medical radio
headset**, medical PDA on the belt (medical records app), medical backpack (or satchel/duffel) with a survival
box (medical breath mask). **In your left hand: the surgical medkit.** It holds: a **health analyzer**, medical
gauze (12), 2 sutures, 2 regenerative mesh, 1 epinephrine **medipen**, **surgical drapes**, **scalpel**,
**hemostat**, **cautery**. Missing for most surgery: retractor, circular saw, bonesetter, bone gel (they are on
the surgery trays, section 3).

Radio: your headset has **common** (`;`) and **medical** (`:m`) only. **There is no security channel on your
headset**: call Security on common.

Access: Medical (medbay doors, Medbay Storage, Treatment Center, Cryogenics), Surgery (both operating rooms, the
anesthetic closet), Morgue, Pharmacy, Virology, Paramedic (Paramedic Dispatch and its locker), Mineral
Storeroom, medical exosuit bay. Not the CMO's office. Chemistry's own door needs plumbing access, which doctors
get only on some server settings: if it refuses you, use the Pharmacy Desk or ask the Chemist.

## 3. Where things are on MetaStation

North is "fore" (up), south is "aft". Medbay is in the south-west quarter. From the Central Primary Hallway go
south along the **Aft Primary Hallway**; the **Medbay Lobby** opens off its west side at the north end ("Aft
Primary Hallway" glass doors). Science is across that hallway to the east. Area names below are exact
(`walk_to {area: "..."}`).

| Area | What's there |
|---|---|
| **Medbay Lobby** (NE corner, public) | Tables with mesh, sutures, gauze (two sets) and a box of body bags; 3 emergency medical beds (roller beds) on the south wall; "Cargo Deliveries" chute. South: "Medbay Clinic" doors (public) into the clinic. |
| **Medbay Central** | The clinic just south of the lobby (medical kiosk, DeForest first aid station on the wall, a medkit on a table); the staff corridor running north-south through medbay (north end: "Medbay Staff Entrance"); the east-west corridor south of Medbay Storage with the two vendors: **NanoMed Plus** and **NanoDrug Plus** (side by side on its south side, next to the Medical Break Room). "Medbay" doors (medical access) separate the clinic from the staff side. |
| **Medbay Treatment Center** (door name: "Primary Treatment Centre", 2 doors in its east wall) | Your main room. North wall: 2 **lifeform stasis units** (stasis beds), each under a **defibrillator mount**, each with an IV drip and vitals reader. South wall: 2 **medical beds**, each under a defibrillator mount, each with an IV drip. **All 4 mounts start empty.** Centre: **crew monitoring console**. Tables west of it: 4 **health HUD glasses**, gauze, a chem pack, body bags, gloves, masks. Tables east of it: 4 empty medical belts, mesh, epinephrine and multiver bottles, a syringe. West wall: **smart organ storage** (empty) between the two "Primary Surgical Theatre" doors. North wall middle: "Cryogenics Bay" door. |
| **Grand Surgery Theatre** (west of the Treatment Center, surgery access) | 2 **operating tables** on the west wall, each with an **operating computer** and vitals reader; a **full surgery tray** at each end (scalpel, hemostat, retractor, cautery, circular saw, surgical drill, bonesetter, bone gel, surgical tape, drapes, blood filter, surgical razor, mask); behind the "Surgical Supplies" windoor (east side): 3 **anesthetic tanks**, 3 breath muzzles, bone gel, surgical tape; a crate of surplus prosthetic limbs. |
| **Medbay Storage** (south of the Treatment Center) | Behind the "First Aid Supplies" windoors (east side): **4 loaded defibrillators**, 2 **medical syringe guns**, boxes of syringes, medkits (4 regular, 3 brute, 3 fire, 3 toxin, 3 oxygen). West side: **department techfab (Medical)** (a lathe), MediDrobe, cell charger, nitrile gloves, recharge station, medical records console. |
| **Cryogenics** (north of the Treatment Center) | 2 **cryo cells** (north wall), the **freezer** (thermomachine, SW corner, starts **off**), table with 4 **cryoxadone beakers** and a **mannitol pill bottle**, 2 anesthetic canisters, 2 stethoscopes. |
| **Paramedic Dispatch** (NE of Cryogenics, paramedic access) | Crew monitoring console, medical records, **emergency medical team locker** (emergency medkit, box of bandages, **crew pinpointer**, paramedic medical belt, 2 medical headsets, **2 roller beds**), medical suit storage unit (medical MODsuit, oxygen tank), **jaws of recovery cabinet** with a surgical drill on the table beside it. |
| **Aft Operating Room** (south-west, door "Auxilliary Surgery", surgery access) | Operating table, operating computer, full surgery tray, **anesthetic closet** (3 anesthetic tanks, 3 muzzles), smart organ storage, IV drip, "corpse disposal" bin. |
| **Medical Cold Room** (west end of the south corridor) | 2 **blood freezers** (each: blood packs A-, B-, B+, O-, O+, lizard, ethereal, 3 random types, 2 empty packs, a blood types paper), 2 anesthetic canisters. |
| **Morgue** (south-east; doors from Medbay Central and from the Aft Primary Hallway) | 13 morgue trays, smart organ storage, operating table + computer, autopsy tray, body bags, IV drip, emergency bed. |
| **Chemistry** (east of the central corridor) and **Pharmacy** (east of the clinic) | The Chemist's rooms. The Pharmacy Desk windoors face the lobby and the clinic: that's where medicine is handed over. |
| Others | Chief Medical Officer's Office (east of the Treatment Center), Medical Break Room, Psychology Office, Virology (far west), Security Post - Medbay (north of the clinic), Abandoned Medbay (maintenance, south). |

No wall-mounted NanoMeds exist on this map.

**Vendors** (medical staff get 80% off normal items; Premium items cost full price):
- **NanoMed Plus**: gauze ×8, syringes ×12, droppers, **health analyzers ×4** (and simple ones ×4), surgical tape
  ×3, ointment ×2, **sutures ×2**, **bone gel ×4**, crutches, triage cards, bandage boxes, **crew pinpointers ×2**.
  Premium: medipens ×3, medical belts ×3, handheld crew monitor (sensor device) ×2, advanced medkits ×2, shears,
  tourniquets ×6, organ box.
- **NanoDrug Plus**: **libital patches ×5** (brute), **aiuri patches ×5** (burn), convermol syringes ×2, insulin
  pills, bottles of multiver ×2, syriniver ×2, calomel ×2, epinephrine ×3, morphine ×4, potassium iodide,
  saline-glucose ×3, toxin ×3; antiviral syringes; medigels of libital, aiuri, sterilizine. Premium: **synthflesh
  medigel ×2** (60u, best corpse repair), psicodine, sansufentanyl, albuterol inhalers.

## 4. The health analyzer

Hold it, click the patient: health scan (left click). **Right click: chemical scan** (what's in their blood and
stomach). Use it in hand (key Z): switches between health and **wound** mode (wound mode explains each wound and
its treatment). Alt-click it: toggles the per-limb damage table. Ctrl-shift-click: prints the last scan.

Readout, top to bottom:
- **Overall status**: "N% healthy" or **Deceased**. Health = 100 minus (brute + burn + toxin + suffocation).
- Husked (needs synthflesh), Fatigue (stamina) level.
- Damage table: Brute (red), Burn (orange), Toxin (green), Suffocation (cyan), per limb, with **"Physical trauma:
  <wound name> (<severity>)"** lines under each wounded limb.
- **Organ status**: each organ "OK", **Mildly Damaged** (>10), **Severely Damaged** (>45), **Non-Functional**
  (failing, 100). The heart line can also read **Myocardial Infarction** (heart attack: defibrillate now) or
  **Cardiac Arrest**. A **Non-Functional heart = the defibrillator will refuse.**
- Body temperature, **blood level** (% and volume; normal 560; red below 85%) and **blood type**.
- Diseases with their cures.
- For the dead: **Time of Death** and **"Subject died X ago."** This is your revival clock.

The **operating computer** beside each operating table shows the patient on that table: status, health, the four
damage numbers, blood type and level, and the **surgery state of the zone you target** ("Ready for surgery",
"Skin is cut", "Bone is sawed", "Bodypart is obstructed by clothing"...).

## 5. Damage types and treatments

| Damage | Living patient | Corpse / quick | Where from |
|---|---|---|---|
| **Brute** (bruises, cuts) | Libital patch (heals 3/s, slight liver damage), suture (10 brute + stops bleeding, per use), bruise pack / first aid bandage, probital pills | **Synthflesh** (1.25 × volume on touch, works on the dead), tend wounds surgery | NanoDrug Plus, brute medkits, Chemist |
| **Burn** | Aiuri patch (2/s, slight eye damage), regenerative mesh (10 burn per use, treats burn wounds), ointment | Synthflesh, tend wounds | NanoDrug Plus, fire medkits, Chemist |
| **Toxin** | Multiver (purges other chems too), syriniver (inject only; overdose at 6u), calomel (purge), potassium iodide (radiation), seiver | Not needed for revival (defib ignores toxin) | NanoDrug Plus, toxin medkits |
| **Suffocation** (oxy) | **Convermol** syringe, salbutamol medipen, **epinephrine** in crit, **CPR**; fix the cause (air, lungs, blood) | The defib adds oxy to put the revived at -50 health; CPR and epinephrine after | NanoDrug Plus, oxygen medkits |
| **Blood loss** | Stop bleeding first (section 6), then **blood pack on an IV drip** (matching type), saline-glucose, iron pills | Blood doesn't regenerate without a working heart | Medical Cold Room, NanoDrug Plus |
| **Brain** | **Mannitol** (in the cryo room) | Brain surgery (section 9); a brain fails after ~30 min dead | Cryogenics table, Chemist |
| **Organ damage** (heart, lungs, liver, stomach, eyes, ears) | Rest heals mild damage; repair surgeries; replace the organ | **Coronary bypass** or a new heart (section 8) | Medical techfab (cybernetic organs) |
| **Stamina** (exhaustion, "Fatigue") | Rest; epinephrine reduces it | none | |
| **Critical / dying** | **Epinephrine** (stops crit suffocation, heals 1/s of each in crit; overdose 30u) | Medipen first | Every medkit, NanoDrug Plus |

Notes:
- **Corpses don't metabolize** most chemicals: pills, syringes and patches of libital or aiuri do nothing to a
  dead body. Touch chemicals still act: **synthflesh** (patch, splash, medigel spray) heals the dead, and
  **formaldehyde stays in a corpse and stops organ rot**.
- **Synthflesh** heals brute and burn equally and adds toxin (50-75% of what it healed). The NanoDrug Plus
  synthflesh medigel sprays all 60u at once (3 s): 75 brute + 75 burn. A patch delivers 0.75u/s, and
  **patches pause on a running stasis bed**. A splash from a beaker (combat mode on, right-click the patient with
  the beaker) delivers everything at once. Chemist's recipe: blood 1 + carbon 1 + libital 1, heated to 250 K or
  more (best at 310 K), gives 3. 60u of pure synthflesh also un-husks a body husked by burns (once its burn damage
  is low enough).
- Medical stacks (sutures, mesh, gauze, ointment) heal the limb you target (body zone), work through most
  clothing, **don't work on corpses** (gauze does), and need **combat mode off**. Sutures and mesh repeat over
  every hurt limb until the stack runs out.

## 6. Wounds

A wound is a per-limb injury on top of damage. The scanner names it under the limb. Treat with the limb targeted
(Numpad zone keys, section 15) and combat mode off.

| Type (names, mild to worst) | Effect | Field treatment | Surgery |
|---|---|---|---|
| **Slash**: Rough Abrasion, Open Laceration, Weeping Avulsion (also "Numerous Small Slashes", "Burning Avulsion") | Bleeding. The worst one gets worse on its own. | **Sutures** (stop 0.5 flow per use), **gauze** (soaks and slows), **cautery** on the limb (burns it shut, small burn), sanguirite (coagulant; 2u in every medipen) | Not needed |
| **Pierce**: Pinprick Pierce, Minor Skin Breakage / Penetration, Open Stab / Bullet Puncture, Ruptured Cavity | Bleeding, internal bleeding | Same as slash | **realign blood vessels** (hemostat) then **seal blood vessels** (cautery), with skin open and organs incised |
| **Blunt**: **Joint Dislocation** | Limp or clumsy hand | **Bonesetter** on the limb; or an aggressive grab, then click the limb with an empty hand, combat mode off (65% per try, 20 brute) | **reset dislocation** (bonesetter) |
| **Hairline Fracture** | Pain, limp, internal bleeding | **Bone gel then surgical tape** on the limb (gel: 25 brute + 100 stamina; heals in ~4 min); gauze as a splint meanwhile | Cut skin (scalpel), then **repair hairline fracture** (bone gel, bonesetter or surgical tape) |
| **Compound Fracture** | Limb disabled, bleeding | Gauze/splint; gel + tape (heals in ~8 min) | Retract skin, **clamp bleeders**, **reset compound fracture** (bonesetter), **repair compound fracture** (bone gel), mend |
| **Cranial Fissure** (head) | Brain exposed | none | **discard skull debris** (hemostat), **repair cranium** (bone gel) |
| **Burn**: Second Degree Burns, Third Degree Burns, Catastrophic Burns | Infection grows (sepsis in ~9 or ~4 min for the worse two) | **Regenerative mesh** or ointment (sanitize and regrow flesh), synthflesh, **cryo**, clean gauze | **debride infected flesh** (hemostat), loops |

Direct bone gel/tape **won't apply on a limb prepared for surgery** (drapes, operating table, stasis bed): the
surgery version is used there instead. Bleeding patients lose blood; check "blood level" and refill (section 10).

## 7. Crit and death

- Health 100 = unhurt. **0 or below: critical** ("soft crit", weak, can't talk on the radio). **-30: hard crit**,
  unconscious. **-100: dead.** In crit a patient can't breathe properly and suffocation damage climbs: give
  **epinephrine** (medipen: 10u epinephrine + 3u formaldehyde + 2u sanguirite) to stop it, then heal.
- **CPR**: empty hand, combat mode off, click a patient lying in crit (not dead). 3 s, then -7 suffocation,
  repeating quickly while they stay in crit. Both of you need uncovered mouths (remove masks).
- Death is not the end: section 8.

## 8. Revival (exactly as this server implements it)

### What the defibrillator checks

When you shock a corpse (paddles on the chest), it fails with one of these, in this order:

| Message ("Resuscitation failed - ...") | Cause | Fix |
|---|---|---|
| "Recovery of patient impossible. Further attempts futile." | Suicide | None |
| "Patient's body is a mere husk, repair and try again." | Husked | Synthflesh (60u) after lowering burn damage; a husk from desiccation can't be fixed |
| "Tissue damage too severe, repair and try again." | **Brute ≥ 180 or burn ≥ 180** (each counted separately) | Synthflesh, tend wounds |
| "Patient's heart is missing." | No heart | Insert one (section 9) |
| **"Patient's heart too damaged, replace or repair and try again."** | **Heart failing (damage 100, "Non-Functional")** | **Coronary bypass** or a **new heart** |
| "Patient's brain is too damaged, repair and try again." | Brain failing | Brain surgery |
| "No intelligence pattern can be detected..." / "...brain is missing..." | No mind / no brain | None (see "Other ways back") |

**There is no time limit in the defibrillator itself.** The limit is organ rot:
- A dead body's **heart rots to failure in about 6 minutes** (room temperature); the lungs ~16 min, stomach ~13,
  **brain ~30 min**. Rot slows in a body below 20 °C and stops below 0 °C.
- **Rot stops completely while**: the body is **buckled to a running stasis bed**; the body contains **at least 1u
  of formaldehyde** (an epinephrine medipen injected into a corpse gives 3u, and the dead don't metabolize it, so it
  lasts); or cryostylane. Organs in **smart organ storage** don't rot; **cybernetic organs** never rot.
- So: **the first thing to do with a fresh corpse is inject an epinephrine medipen** (every doctor starts with one;
  every regular, fire and oxygen medkit has one; NanoMed Plus sells them), then get it onto a stasis bed.

A successful shock revives the patient at **-50 health** (deep crit), with suffocation damage added. Heal them
immediately: epinephrine, CPR, then brute/burn. A revived patient with a failing heart has cardiac arrest again
and dies: fix the heart before the shock.

### Using a defibrillator

Defibrillators: 4 loaded ones in **Medbay Storage** (First Aid Supplies table), 2 more in a cargo "Defibrillator
Crate", and the medical techfab prints them and wall mounts. Each charge (10 per cell) is used by every attempt,
failed or not; 5 s recharge between shocks ("Unit ready" beep). Mounts don't recharge.

1. **Mount it** (best): click an empty **defibrillator mount** in the Treatment Center with the defibrillator. The
   mounts are directly over the 2 stasis beds and the 2 medical beds. Or **wear it on your back**: take off your
   backpack first (the defib only fits the back slot), equip the defib, then click it on your back with an empty
   hand to take the paddles.
2. **Take the paddles**: click the mount with an empty hand. **Paddles must stay within 1 tile of the unit**: if you
   step 2 tiles from the mount they "overextend and come out of your hands" and snap back. Stand next to the mount
   with the patient next to you; a patient on the bed under the mount is right.
3. **Wield** them: both hands empty except the paddles, key **Z** ("You need to wield the paddles in both hands").
4. **Target the chest** (Numpad5). **Combat mode off.**
5. **Clear**: **stop pulling the patient** and make sure nobody else is pulling them (key H, "stop pulling"). The shock
   **electrocutes whoever is pulling the body** (yesterday's doctor shocked himself this way). Remove thick chest
   wear (space suits, MODsuits, bio suits, some heavy armor and coats): "Patient's chest is obscured. Operation
   aborted."
6. Click the patient with the paddles and **stand still 5 s** (3 s placing, 2 s charging). Then read the message.
7. After a success: drop the paddles (they snap back into the unit), CPR or epinephrine, then treat.

### Fixing a heart that is "too damaged"

- **Coronary bypass** (section 9): sets the heart to 60 damage (no longer failing). **Once per heart.** In a
  corpse at room temperature it rots from 60 back to failing in about **2.4 minutes**, so do it on a running
  stasis bed (or with formaldehyde in the body) and shock right after.
- **Replace the heart** (organ manipulation, section 9). Sources:
  - **Basic cybernetic heart** from the **department techfab (Medical)** in Medbay Storage (the "Augmentation" design
    is available from round start; costs a little iron and glass, from the station's material silo or sheets put
    in). Never rots. The Scientist's protolathe and the Roboticist's exosuit fabricator can print it too; better
    cybernetic hearts need research.
  - A healthy heart from a body that can't be revived (no mind, suicided).
  - Cargo's "Organ Growing Kit" (a vat grower, microscope, biopsy tool): slow, not a quick source.
- Keep spare organs in **smart organ storage** (Treatment Center west wall, Aft Operating Room, Morgue).

### Revival procedure (Doctor A, with Doctor B fetching)

1. At the body: **inject the epinephrine medipen** (formaldehyde stops the rot). Scan: note "died X ago" and the
   heart line. Report on medical radio: who, where, how long dead.
2. Bring the body to the **Medbay Treatment Center**: drag it, or better, buckle it to a roller bed and pull that
   (section 10). Stop pulling before any shock.
3. **Buckle it to a stasis bed** (drag the body onto the bed; 2 s). A running stasis bed stops rot and counts as
   prepared for surgery on every limb. Mount a defib over it if not done.
4. Strip what covers the chest (drag the body onto yourself for the strip menu: suit, jumpsuit).
5. Scan. If **brute or burn ≥ 180**: synthflesh (medigel spray, splash, or several patches with the stasis bed
   switched off), or **tend wounds** (slow on a corpse: 20% effect).
6. If the heart is **Non-Functional** (or missing): coronary bypass, or replace it.
7. If the brain is Non-Functional: brain surgery.
8. Close all incisions (cautery: "mend skin incision").
9. Shock (steps above). Then **alt-click the stasis bed to switch it off** so the patient breathes and
   medicines work; epinephrine, CPR, heal, refill blood.

### Other ways back

- **"shock brain"** surgery (Brain Defibrillation): head skin open and skull sawed, then wielded paddles. It doesn't
  check the heart or brute/burn thresholds, but the body needs health above -100 after it (-50 suffocation
  removed), and a failing heart still kills again. A fallback, not the plan.
- **Strange Reagent**: revives a corpse with total brute + burn ≤ 200, using 1u per 5 points above 100. For a
  normal body it must be **swallowed**: feed it from a beaker (3 s, mouth uncovered). Recipe: omnizine + holy
  water + unstable mutagen (1:1:1). **Chemistry can't make omnizine**: it comes from Ambrosia Deus (the
  Botanist), so this is rare.
- A body that can't come back: put it in a **body bag**, take it to the **Morgue**, load it in a morgue tray
  (label it), tell the Captain and the Head of Personnel. A brain can go into an MMI (a Roboticist's job, if one is
  on shift).

## 9. Surgery

### Starting a surgery (the rule yesterday's doctor missed)

A surgical tool used on a patient whose targeted limb is **not prepared** just **attacks** them ("You rip ... in
the chest with the scalpel!"). Prepare first:
- **Buckle the patient to an operating table or a stasis bed** (drag them onto it; they lie down): every limb
  counts as prepared, no drapes needed. Or
- Target the zone and click the patient with **surgical drapes** (a bedsheet, cape or cloak also works): "[zone]
  surgery prepared". Click again to clear. Drapes fall off if the patient walks 4 tiles.

Then the patient must be **lying down** and the **targeted zone uncovered**: any worn item covering it blocks the
surgery ("operation site is obstructed!"); a jumpsuit covers chest, arms and legs, a labcoat chest and arms. Strip
them (strip menu). Click the patient with the tool: a **radial menu** lists the operations that tool can do there
(a single option starts by itself). Stay adjacent and still until it finishes.

Speed and failure: operating table ×1.0, stasis bed ×1.15, table ×1.25, bed ×1.5, **floor ×2.0**; tool factors (a
kitchen knife instead of a scalpel ×1.5, etc.); a patient on painkillers (morphine) or analyzed ×0.8; a drunk
surgeon is slower. Up to ×2.5 nothing fails; beyond that each extra second adds 10% failure chance. With the
proper tool nothing fails even on the floor (×2.0, just slow); improvised tools on the floor can fail.

**Anaesthesia** is not required: an awake patient feels pain and may scream, nothing more. For a calmer patient:
an **anesthetic tank** (N2O mix) with a **breath muzzle/mask** on their internals (Grand Surgery Theatre supplies,
anesthetic closet), or morphine. An operating table can hold a tank and a mask (attach a tank under it, a mask to
its side; then drag the table onto the patient to connect their internals).

### Surgical states, tools and radial names (body zone targeted)

| Step (radial name) | Tool | Notes |
|---|---|---|
| **make skin incision** | scalpel (knife, shard...) | Skin cut, vessels unclamped (bleeds) |
| **retract skin** | retractor (screwdriver, wirecutters) | Skin open |
| **clamp bleeders** / unclamp bleeders | hemostat (wirecutters) | Heals 20 if the bone is sawed |
| **saw limb bone** | circular saw | **50 brute** to the limb |
| drill limb bone | surgical drill | For implants |
| **incise organs** | scalpel | 10 brute |
| **mend skin incision** | cautery (or a suture, welder, laser gun) | Closes everything; **heals 40 if the bone was sawed** |
| fix limb bone | bone gel / surgical tape | Unsaws the bone, heals 40 (not needed if you mend) |

### Tend wounds (brute/burn surgery)

Chest, any skin state: **scalpel "make skin incision"**, then **hemostat "tend bruises"** or **"tend burns"**. It
repeats by itself (2.5 s each) while that damage remains: heals 5 + 7% of the current damage each time; **×0.55
if the chest is clothed** and **×0.2 on a corpse**. Hold the health analyzer in your other hand to see the
numbers. Close with the cautery when done. Failure deals damage, so use a table or stasis bed.

### Coronary bypass ("graft coronary bypass")

Chest. Only when the heart has ≥60 damage and was never bypassed before. Steps: scalpel **make skin incision** →
retractor **retract skin** → circular saw **saw limb bone** → hemostat **clamp bleeders** → scalpel **incise
organs** → hemostat **graft coronary bypass** (9 s) → cautery **mend skin incision**. Net damage roughly zero
(saw +50, incise +10, clamp −20, mend −40). Failure tears the heart (+20 damage, heavy bleeding). In the
hemostat's radial, don't pick **"remove heart"** by mistake.

### Replacing an organ (internal organ manipulation)

Chest organs (heart, lungs, liver, stomach) need skin open, **organs incised and the bone sawed**; head organs
(brain, eyes, ears) need skin open and organs incised (the brain also needs the skull sawed). Then: hemostat →
**"remove heart"** (the organ drops on the floor), then click the patient with the new organ in your hand →
**"insert basic cybernetic heart"** (or "insert heart"). Close with the cautery.

### Brain surgery

Head: incision, retract, saw, clamp (blocked while vessels are unclamped), then hemostat **"brain surgery"**
(10 s, repeats, heals 25% of the brain per pass). Close.

## 10. Equipment

- **Lifeform stasis unit** (stasis bed): drag the patient onto it (buckles them). While running it stops the
  body's processes: **no organ rot, no bleeding loss, no metabolism (patches and pills pause)**, wounds still
  process. Alt-click the bed toggles it on/off (5 s cooldown). Counts as prepared for surgery. Needs power.
- **Cryo cell** (living patients only; the dead are ejected): heals all damage types and wounds over time with
  cryoxadone, which **only works below 273 K body temperature**. Setup: in Cryogenics, open the **freezer**'s
  window, turn it on (action `power`) and set its target to the minimum (action `target`, ~73 K; alt-click
  instead cycles 20 °C → maximum heat → minimum, so from 20 °C alt-click twice); click a cryo cell with a
  **cryoxadone beaker**. Load: drag the patient onto the cell
  (instant if they're incapacitated, else 2.5 s), then close the door (cell window action `door`, or alt-click)
  and turn it on (`power`, or ctrl-click). It ejects automatically when they're healed (`autoeject`). If it says
  "Insufficient cryogenic gas", ask an Atmospheric Technician.
- **IV drip**: click it with a blood pack or a beaker, then **drag the IV drip onto the patient** (1 s). Default
  5u/s injecting; stays attached within 1 tile. Its window: `changeMode` (inject/take blood), `changeRate`
  {rate 0-5}, `detach`, `eject`. Alt-click toggles 0/5 u/s.
- **Blood types**: O- can go to anyone; O+ to O+, A+, B+, AB+; A- to A-, A+, AB-, AB+; B- to B-, B+, AB-, AB+; A+
  to A+ and AB+; B+ to B+ and AB+; AB+ takes any of these. Wrong blood causes toxin damage. Lizards and ethereals
  have their own types (packs in the blood freezers). Saline-glucose substitutes briefly and speeds regrowth; iron
  pills too. Blood only regrows with a working heart.
- **Body bags** (boxes in the Lobby, Treatment Center, Morgue and Medbay Central): use in hand to unfold, put the
  body in, close, pull. A bag doesn't stop rot. Stasis body bags need research (Cryostasis).
- **Moving patients**: ctrl-click to pull (key H stops). Better: a **roller bed** (emergency medical bed: 3 in the
  Lobby, 2 folded ones in the emergency medical team locker, 2 in the Abandoned Medbay). Unfold one by using it in
  hand, drag the patient onto it to buckle them, then pull the bed. Alt-click toggles its brakes; right-click
  folds it (empty). Medical beds in the Treatment Center have wheels too.
- **Jaws of recovery** (Paramedic Dispatch cabinet: unlock it with the surgical drill on the table there, click to
  open, click to take): pries open most airlocks for rescues (not command, security or other high-security
  doors) and **announces it on the security and medical channels**; its other mode is a bonesetter.
- **Medical MODsuit** (Paramedic Dispatch suit storage unit) for fetching bodies from vacuum. Take it off a
  patient before defibrillating.

## 11. Suit sensors, the crew monitor and finding people

- Every jumpsuit has sensors: **Off, Living, Vitals, Tracking**. The crew monitor shows a person only if their
  sensors are on; damage numbers only at **Vitals** or higher; **location only at Tracking**. Players set their own
  with the "Adjust Suit Sensors" verb. Yours: set to Tracking at shift start. Ask the crew on common to do the
  same. On a patient: strip menu, jumpsuit, alternate action "adjust_sensor".
- **Crew monitoring console** (Treatment Center centre, Paramedic Dispatch, CMO's office). Its tgui data
  `sensors` lists, for each person: `name`, `assignment`, `life_status` (**0 conscious, 1 soft crit, 2
  unconscious, 3 hard crit, 4 dead**), `oxydam`, `toxdam`, `burndam`, `brutedam`, `health`, `area`. Read it with
  `tgui_window` (path/fields) instead of looking at it. Watch for life_status ≥ 1 and falling health.
- **Crew pinpointer** (NanoMed Plus ×2, emergency medical team locker): use in hand, pick a name ("Person to
  track"); it points to people whose sensors are on Tracking. The premium handheld crew monitor (sensor device) is
  a portable crew monitor.
- **Health HUD glasses** (4 on the Treatment Center table): health bars and status over people's heads.

## 12. Triage (several hurt at once)

1. Shout on medical: how many, where, who takes whom. Doctor A holds the Treatment Center, Doctor B goes out.
2. Order: **bleeding out or in crit** (epinephrine medipen, gauze/sutures on the bleeding limb, then move) →
   **fresh dead** (medipen for formaldehyde, stasis bed: they wait without rotting) → serious but stable (patches,
   mesh, sutures, splints) → walking wounded (hand them patches or send them to the clinic's first aid station).
3. A corpse that's been dead long without formaldehyde or stasis has a failing heart: put it on stasis anyway and
   plan a bypass or a new heart; don't let it block a living patient in crit.
4. Two stasis beds: if both are full, inject formaldehyde (medipens) and lay others on the medical beds or in the
   morgue trays. Formaldehyde in a corpse works anywhere.
5. Keep a short log: name, injury, treatment, outcome. Report deaths and revivals on common.

## 13. Dangers and common mistakes (several from yesterday)

- **Heart rot**: every defib failed with "heart too damaged" because bodies sat for minutes with nothing done.
  Medipen at the body, stasis bed, bypass or new heart, then shock.
- **Scalpel on an unprepared patient = an attack.** Operating table, stasis bed or drapes first, clothes off,
  patient lying down, combat mode off.
- **Paddles have 1 tile of reach from the unit.** Stand next to the mount, patient next to you. Don't drop the unit
  on the floor and walk off.
- **Pulling the body during a shock electrocutes you.** Stop pulling first (key H); warn helpers to let go.
- **Disposal units eat what you click into them** (yesterday a medkit was lost). Don't click a disposal bin with
  something you want to keep.
- **Oil and water on floors**: walking over them can slip you; a slip near disposals can flush you into the pipes.
  Walk (not run) over wet floors.
- Clicking with a full active hand uses the item on the target. Keep one hand empty for consoles, doors, beds,
  paddles (key X swaps hands).
- Tend wounds on a corpse is slow (20%); synthflesh is the fast way.
- Stasis pauses patches and metabolism: switch the bed off when the patient is alive and needs medicine to work.
- Overdoses: epinephrine 30u, syriniver 6u, convermol 35u, morphine 30u. Multiver purges other medicines.
- Cryo doesn't work on the dead or when the freezer is off.
- The crew monitor can be missing people with sensors off. Ask on common.
- Radio in crit fails (you only whisper): get help before you go down.

## 14. Emergencies

- **Power failure**: stasis beds, cryo, the freezer and the techfab stop. Inject formaldehyde into corpses on
  stasis (rot resumes otherwise). Defibs run on their own cells. Report the medbay APC on common for the
  engineers.
- **Breach or fire in medbay**: move patients out on roller beds; leave the area to Atmospherics. Don't open doors
  to space. Burn victims: mesh, synthflesh, cryo later.
- **Mass casualty**: section 12. Ask the Chemist for brute and burn patches and synthflesh in bulk, the
  Quartermaster for a Medical Supplies or Blood Pack Variety crate.
- **Attacker in medbay**: section 15.
- **Evacuation**: bring stable patients to the shuttle on roller beds. Bodies you can't revive go in body bags
  onto the shuttle or into the morgue. Take medkits and a defibrillator on your back for the ride.

## 15. Defending yourself and your patients

Yesterday a killer worked inside medbay: the Treatment Center saw a patient beaten to death. Shared combat
mechanics (combat mode, shoving, grabs, resisting) are in crew-basics; here is what your role has.

- **Call for help on common** (`;`), with the attacker's description and the exact area: you have **no security
  channel**. The AI can bolt and close medbay doors on request and watch the cameras.
- **Keep the inner doors shut**: the Treatment Center ("Primary Treatment Centre"), "Medbay" and Storage doors need
  medical access, but anyone can follow you through. Treat strangers in the public clinic and lobby; bring only
  patients and medical staff inside. In an emergency, ask the AI to bolt the Treatment Center doors.
- **Weapons in reach** (combat mode on): the **circular saw** and **surgical drill** (15 damage each, cutting/
  piercing) and the **scalpel** (10) from the surgery trays; a fire extinguisher from the wall cabinets. The
  defibrillator can't be used as a weapon while its safety is on (always, unless sabotaged).
- **Sedation is slow**: morphine (NanoDrug Plus bottles) makes someone sleep only after about 1.5 minutes and 10u+;
  a **medical syringe gun** (2 in Medbay Storage, holds 1 syringe) can deliver it from range. Use it on a violent
  patient, not as a fight opener. N2O from an anesthetic tank needs a mask on the target.
- **Shove, don't brawl**: a shove into a wall or table knocks people down; then walk away and call security.
- **Protect the vulnerable**: patients on stasis beds and operating tables can't defend themselves. If an
  attacker is in the room, stand between, call it in, and if they're armed and you're not, leave and come back
  with security. A dead doctor revives no one.
- **Surgery and medicine only with consent or need.** Never use surgery, toxins or the syringe gun to punish;
  treat everyone, arrested people and attackers included, once they're no longer a threat.

## 16. Working with the crew

- **Chief Medical Officer** (if on shift): your boss; follow their triage and assignments. **Paramedics**: like
  Doctor B; share the crew monitor and roller beds. **Coroner**: the morgue and autopsies; hand them the dead you
  can't revive. **Other doctors**: split rooms (one per stasis bed / operating table).
- **Chemist**: ask early for brute (libital) and burn (aiuri) patches, **synthflesh** (patches and a beaker; the
  most important item for revival), epinephrine, convermol, mannitol. Pick it up at the Pharmacy Desk. If nobody is
  doing chemistry, the NanoDrug Plus covers the basics and you can't make more synthflesh.
- **Botanist**: medicinal plants for the Chemist; Ambrosia Deus for omnizine (strange reagent).
- **Scientist**: research for medbay (Improved Wound-Tending, cybernetic organs, Cryostasis for stasis bags and more
  stasis beds), protolathe prints (cybernetic hearts).
- **Quartermaster**: crates (Medical Supplies, Defibrillator Crate, Blood Pack Variety, Surgical Supplies with a
  roller bed, IV Drip, Organ Growing Kit). They arrive at the Lobby's Cargo Deliveries chute or by hand.
- **Security Officers**: bring in wounded prisoners and fighters; call them for violent patients. Treat everyone.
- **AI**: doors, cameras, finding people and bodies with sensors off. Ask it to open doors you lack access to for a
  rescue.
- **Station Engineers / Atmospheric Technician**: power for the stasis beds and cryo, breaches, the cryo gas loop.
- **Captain / Head of Personnel**: report deaths and revivals; the Head of Personnel can add access.
- **Janitor**: blood, broken glass and bodies left in halls; tell them where.
- **Cook**: food fixes hunger (well-fed patients heal organs faster).

## 17. Through the client

- `walk_to {area: "Medbay Treatment Center"}` (or "Medbay Storage", "Grand Surgery Theatre", "Cryogenics",
  "Paramedic Dispatch", "Morgue", "Medical Cold Room", "Medbay Lobby"). Doors you lack access to stop the walk with
  an access note: ask the AI or another doctor.
- **Body zones**: keys Numpad5 chest, Numpad8 head (again: eyes, mouth), Numpad4/6 right/left arm, Numpad1/3
  right/left leg, Numpad2 groin. The click answer shows `zone_selected`. Defib = chest; tend wounds and bypass =
  chest; brain = head.
- **Key Z** uses the held item in hand (wield paddles, switch the analyzer's mode, use the crew pinpointer, unfold a
  roller bed or body bag). **Key X** swaps hands. **Ctrl-click** pulls, **key H** stops pulling.
- **Defib**: `click` the mount with an empty hand (paddles in hand) → key Z (wield) → Numpad5 → `click` the patient
  → `wait` ~6 s and read the defibrillator's line in chat ("pings: Resuscitation successful" or "buzzes:
  Resuscitation failed - ...").
- **Surgery**: `click` the patient with the tool → the answer shows `menu_opened` with the radial choices → `click`
  the choice's id. One choice starts by itself. Long steps show progress; wait and stay put.
- **Buckling**: `drag` the patient onto the stasis bed, operating table, roller bed or cryo cell. **Strip menu**:
  `drag` the patient onto yourself, then `tgui_act` action `use` with `{key: "jumpsuit"}` (or "suit", "mask",
  "back"...). Suit sensors on someone else: action `alt` with `{key: "jumpsuit", alternate_action:
  "adjust_sensor"}`, then answer the list.
- **Crew monitor**: click the console, then `tgui_window` with `path: "data.sensors"` and fields like `name,
  life_status, health, area`. Re-read it every few minutes.
- **Vendors**: `tgui_act` action `vend` with the product's ref (from `tgui_window`). Synthflesh medigel is under
  Premium.
- **Analyzer**: the scan comes back as a chat box; `read_chat` if it scrolled away. Right click (`click {right:
  true}`) for chemicals.
- **IV drip, cryo, freezer, techfab**: tgui windows (IVDrip: `changeRate {rate}`, `changeMode`, `detach`; Cryo:
  `power`, `door`, `autoeject`, `eject`; freezer: `power`, `target {target: <K>}`; techfab: `build` with the
  design's `design_path` and `amount`).
- Splash a beaker of synthflesh: combat mode on, `click {object_id: patient, right: true}` with the beaker, combat
  mode off again.
- Medical radio: `say {text, radio: "medical"}`; everyone: `radio: "common"`.

## 18. Checklists

**Shift start (both)**
1. `load_map`, walk to the Medbay Treatment Center. Suit sensors to Tracking. Health analyzer and medipen are in
   your surgical medkit; buy a second medipen and sutures/mesh if needed.
2. Medbay Storage: take the 4 loaded defibrillators; **mount 2 over the stasis beds** (Doctor A), keep one for the
   field (Doctor B, worn on the back when needed).
3. Grand Surgery Theatre: check both surgery trays; put a retractor, circular saw and bonesetter with your kit.
4. Cryogenics: freezer on, at minimum; a cryoxadone beaker in each cell.
5. Medical techfab: print a basic cybernetic heart for the organ storage, if materials allow.
6. Ask the Chemist for synthflesh, brute and burn patches. Announce on common: "Medbay open; set your suit sensors
   to Tracking; call medical if someone's down."
7. Doctor B: crew pinpointer (NanoMed Plus or the emergency medical team locker), roller bed, a regular medkit,
   jaws of recovery if you'll go through locked doors.

**Ongoing loop**
- Every few minutes: crew monitor (life_status ≥ 1, health dropping, anyone dead), radio, chat.
- Someone down: Doctor B goes, medipen first, stop bleeding, roller bed, back to medbay. Doctor A readies a stasis
  bed and defib.
- Every death: medipen (formaldehyde) within minutes, stasis bed, heart and tissue checks, fix, shock, heal.
- Restock: patches, synthflesh, medipens, sutures, mesh, gauze, defib charge.
- Report treatments and revivals briefly on medical; deaths and threats on common.

## 19. Sources

- Code (tgstation 54c22023): `code/modules/jobs/job_types/medical_doctor.dm`, `code/datums/id_trim/jobs.dm`,
  `code/game/objects/items/storage/medkit.dm`, `code/game/objects/items/tools/medical/defib.dm`,
  `code/game/machinery/defibrillator_mount.dm`, `code/modules/mob/living/carbon/carbon.dm` (can_defib),
  `code/modules/mob/living/carbon/life.dm` (organ decay, formaldehyde, stasis),
  `code/modules/surgery/organs/` (decay rates), `code/modules/surgery/operations/*.dm` (all operations),
  `code/datums/elements/surgery_aid.dm`, `code/datums/components/free_operation.dm`,
  `code/game/objects/structures/tables_racks.dm` (operating table), `code/game/machinery/stasis.dm`,
  `code/modules/atmospherics/machinery/components/unary_devices/cryo.dm`, `.../thermomachine.dm`,
  `code/game/machinery/iv_drip.dm`, `code/datums/wounds/*.dm`, `code/game/objects/items/stacks/medical.dm`,
  `code/modules/reagents/chemistry/reagents/{medicine,cat2_medicine,toxin}_reagents.dm`,
  `code/modules/reagents/chemistry/recipes/{medicine,cat2_medicines}.dm`, `code/modules/vending/medical.dm`,
  `code/game/objects/items/devices/scanners/health_analyzer.dm`, `code/game/machinery/computer/crew.dm`,
  `tgui/packages/tgui/interfaces/CrewConsole.tsx`, `code/modules/cargo/packs/medical.dm`,
  `code/modules/research/techweb/nodes/{cyborg,medbay}_nodes.dm`, `code/game/area/areas/station/medical.dm`.
- Map: `_maps/map_files/MetaStation/MetaStation.dmm`.
- Yesterday's round: `runs/12-doctor`, `12-chemist`, `12-cargo`, `12-security` reports.
- /tg/station wiki (CC BY-SA 3.0), Internet Archive captures Feb 2026: Medical_Doctor, Surgery, Guide_to_wounds.
