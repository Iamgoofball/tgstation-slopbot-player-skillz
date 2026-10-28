# Chemist

## 1. The job in one paragraph

You turn the chem dispenser's raw elements into medicine and keep medbay stocked, so the doctors never run out
of anything for any damage type. The basics come first: patches for **brute** and **burn**, something for **toxin**
and for **suffocation (oxygen)**, and **Synthflesh**, the one medicine that heals a corpse's brute and burn so a
defibrillator can bring it back. Then you restock in rounds, answer requests (doctors first, then Botany, the
Kitchen, anyone with a harmless need), and keep your lab shut to people who have no business there. You've done
the job well if the fridge the doctors use is never empty, every item in it is labelled with its contents and dose,
and nothing in your lab ever exploded, smoked or caught fire. Your boss is the **Chief Medical Officer** if one is
on shift. Another Chemist may join (the job has two slots): if one does, split the work, one of you in each lab.

## 2. Starting kit and access

Outfit (code: `code/modules/jobs/job_types/chemist.dm`):
- chemist's jumpsuit, **chemist labcoat** (50% bio, fire and acid protection), white sneakers;
- **science goggles** on your eyes: they scan reagents, so examining a beaker, pill or patch lists exactly what's in it;
- **medical radio headset**: Medical channel `:m`, Common `;` (the `say` tool's radio option does this for you);
- PDA on the belt, chemistry backpack with a medical survival box (breath mask, internals);
- left pocket: a 30u bottle of **Strong Acidic Buffer** or **Strong Basic Buffer** (random); right pocket: a **dropper**.

Access (ID trim `chemist`): **Medical** (medbay's doors), **Pharmacy** (the
Pharmacy, Chemical Storage, the pharmacy desks, the chemical closet), **Plumbing** (the Chemistry lab's door and
desk), mineral storeroom, medical mech bay. If the round started with 20 or fewer players ready, you also get
Morgue, Surgery (the door of the Medical Cold Room, where the blood freezers are), Virology and Paramedic. Doctors have Pharmacy
access; they get Chemistry's (Plumbing) only on those low-population rounds.

## 3. Where things are on MetaStation

Medbay is on the station's aft (south) side, west of the **Aft Primary Hallway**. You enter through the **Medbay
Lobby**; behind it, **Medbay Central** is the long corridor everything opens off. `walk_to {area: "Pharmacy"}` or
`{area: "Chemistry"}` gets you there from anywhere. You have two labs. Use either one, or both.

**Pharmacy** (area "Pharmacy"): the compact lab at medbay's north-east, between Medbay Central and the Medbay Lobby.
It's the better-equipped one. Door in its west wall, from Medbay Central.
- Two workstations, each a **chem dispenser**, a **reaction chamber** and a **ChemMaster 3000** within reach of
  one chair. North: dispenser in the north-east corner, reaction chamber on the north wall, ChemMaster on the east
  wall. South: dispenser and ChemMaster on either side of the south chair, reaction chamber on the south wall.
- **chemical closet** in the middle of the room (Pharmacy access): 2 boxes of **pill bottles**, 2 boxes of
  **medical gel** applicators (7 each), a pH booklet, a dropper, an acidic buffer bottle.
- East wall: tables with the **hand labeler**, package wrap and a pill bottle of epinephrine; a **fire
  extinguisher** cabinet. West side: a reagent grinder, the **Pharmacy Requests Console** (departments send
  requests here), an emergency shower, empty grenade casings (leave them). Tables with beakers, large beakers,
  droppers, epinephrine and Multiver bottles.
- Three **desks** (a table under a sliding window-door that your ID opens): **Pharmacy Desk** north, onto the
  Medbay Lobby, with a **desk bell** for patients; one west, onto Medbay Central; one east, onto the Aft Primary
  Hallway.
- Two **smart chemical storage** fridges set into the walls, usable from both sides: one in the **west wall**
  (opens onto Medbay Central, beside the Pharmacy door) and one in the **north wall** (opens onto the public Medbay
  Lobby).
- Shutter buttons: "pharmacy shutters control" on the north wall (needs Medical access) closes the north windows,
  the lobby fridge and the lobby desk, plus the east windows. "pharmacy shutters control" on the south wall (needs
  Pharmacy access) closes the east desk and its windows.

**Chemistry** (area "Chemistry"): the big lab on the east side of Medbay Central, its east windows onto the Aft
Primary Hallway. Door ("Chemistry", needs Plumbing) in its **west wall**.
- In the **south-west corner**, next to the door, is one workstation: **chem dispenser**, **reaction chamber**
  (north of it), **ChemMaster 3000** (two tiles east), with an office chair between them. Stand beside the chair and
  you can reach all three.
- On the west wall, just south of the door, is a **smart chemical storage** fridge that opens onto Medbay Central.
- **Chemistry Desk**: a desk in the south wall, onto Medbay Central. From inside, your ID opens its window; from
  outside, anyone can reach the table.
- Tables by the ChemMaster: beakers, a dropper, epinephrine and Multiver bottles, a reagent grinder. East wall: a
  second beaker table, a **mechanical toolbox**, plumbing supplies, and the ChemDrobe (vends the **chemistry
  bag** and latex gloves).
- "chemistry lockdown control" button on the north wall (needs Pharmacy access): it closes every "Chemistry
  Shutters" panel, covering the windows, the door, the desk and the fridge. An emergency shower is on the north wall.

**Chemical Storage** (area "Chemical Storage"): a small room at the south end of Medbay Central (door "Chemical
Storage", Pharmacy access). It holds 30u bottles of Potassium, Phosphorus, Sodium, Mercury, Nitrogen, Oxygen,
Ethanol, Carbon, Chlorine, Fluorine, Iodine, Iron, Lithium, Formaldehyde, Epinephrine and Multiver, one bottle
each of **acidic buffer** and **basic buffer**, a box of beakers, a large beaker, gloves and an igniter.

What else in medbay matters to you:
- **Medbay Treatment Center**: on the west side of Medbay Central, where the doctors treat patients. It has IV drips.
- **Medbay Storage** (west side): medkits, two **boxes of syringes**, two syringe guns.
- **Medical Cold Room** (Surgery access): two **blood freezers**, each with about ten filled 200u blood packs (a few
  are for lizard or ethereal crew). Packs can't be poured: they hang on an IV drip.
- **Cryogenics** (north-west): two cryo cells. Four beakers of **cryoxadone** and a pill bottle of **mannitol**
  are on its table.
- The NanoMed Plus and NanoDrug Plus vendors are in Medbay Central.

Already stocked at round start: each of the three smart chemical storage fridges holds **12 epinephrine pills,
5 Multiver pills, 1 epinephrine bottle and 1 Multiver bottle**, and more 30u bottles of both sit on the lab
tables. Don't make epinephrine early.

## 4. The machines (tgui actions)

Click a machine while you stand next to it to open its window. All three machines take a container: either click
the machine with the container in your active hand, or use the `insert` action, which takes the container from
your active hand. `eject` puts it back in your hand.

**chem dispenser** (window "ChemDispenser"). It runs on an internal cell (about 1,000 units when full, shown as
`data.displayedUnits`) that recharges slowly. Everything comes out at 300 K and 100% purity.
- `amount {target: N}`: the dispensing step. N must be one of the inserted container's `data.beaker.transferAmounts`:
  5, 10, 15, 20, 25, 30, 50 for a beaker (50u), plus 100 for a large beaker (100u). 1 and 2 aren't allowed.
- `dispense {reagent: "Hydrogen"}`: adds one step of that chemical. The names: Aluminium, Bromine, Carbon,
  Chlorine, Copper, Ethanol, Fluorine, Hydrogen, Iodine, Iron, Lithium, Mercury, Nitrogen, Oxygen, Phosphorus,
  Potassium, Radium, Silicon, Sodium, Stable Plasma, Sugar, Sulfur, Sulfuric Acid, Water, Welding Fuel. **Oil,
  Acetone, Ammonia, Ash, Diethylamine and Saltpetre are not available** (they need upgraded parts): make them.
- `remove {amount: N}`: throws away N units of *everything* in the beaker, in proportion. N must also be one of
  the transferAmounts: yesterday `remove 40` was silently ignored.
- `eject` (a right-click on the dispenser also ejects), `insert`.
- Read `data.beaker` (contents, `pH`, currentVolume). `static_data.reaction_list.<Product>` is the game's own
  recipe list: `required_reagents`, `required_catalysts`, `lower_temperature` (needed), `upper_temperature`
  (fastest), `lower_ph`/`upper_ph` (full purity). It doesn't show overheat temperatures: those are in §6.

**reaction chamber** (the chem heater; window "ChemHeater"). It heats or cools the inserted beaker toward a target.
- `temperature {target: K}` (0-1000), `power` (toggles on and off; check `data.isActive`), `insert`, `eject`.
  Eject doesn't switch it off.
- It closes about a tenth of the gap each second and never overshoots. To reach a minimum, set the target a little
  above it: 500 to make Ash (which needs 480), 395 for Multiver's 380-410 window.
- Buffers: the chamber holds 20u of Strong Acidic Buffer and 20u of Strong Basic Buffer. `disp_vol {target: 1-10}`
  sets how much one press injects. `acidBuffer {target: 1}` and `basicBuffer {target: 1}` inject that amount into
  the beaker. `acidBuffer {target: -100}` and `basicBuffer {target: -100}` ("Draw all") refill the chamber from the
  inserted beaker if it holds that buffer: insert your pocket bottle or a beaker of buffer you made.
- Read `data.currentTemp`, `data.beaker.pH`, `data.acidicBufferVol` and `data.basicBufferVol`, and
  `data.activeReactions`: each running reaction's `name`, `quality` (the purity being made right now), `danger`,
  `overheat`, `reactedVol` and `targetVol`.

**ChemMaster 3000** (window "ChemMaster"). It splits a beaker's contents and prints medicine. Its **buffer** holds
100u.
- `transfer {reagentRef, amount, target}`: `reagentRef` is the reagent's type path, from
  `data.beaker.contents[].ref` (e.g. "/datum/reagent/medicine/c2/libital"). `target: "buffer"` moves that much of
  that one reagent from the beaker into the buffer. `target: "beaker"` moves it back. `amount: -1` asks for a number.
  This is how you pick the product out of a messy beaker.
- `toggleTransferMode`: when `data.isTransfering` is false, a transfer to "beaker" **destroys** the reagent instead.
  Switch it back afterwards.
- `selectContainer {ref}`: the containers are in `static_data.categories`: **tubes** (test tubes, 30u, open-topped),
  **pills** (up to 50u, several styles) and **patches** (up to 40u, styles for brute, burn, toxin, oxygen and
  more: pick the matching icon). Each one has a `ref`. **It can't print bottles**: when someone asks for "a bottle",
  give them a 30u tube or a beaker.
- `setPillDuration {duration: 0-30}`: how many seconds a pill's sugar coating lasts before it releases in the
  stomach (the default is 3).
- `create {itemCount: N}`: prints N items (up to 50) and splits the buffer evenly among them, up to each container's
  maximum. A **TextInputModal** window titled "Name" opens next. Answer it with
  `tgui_act {id: <that window>, action: "submit", params: {entry: "Libital patch 10u (brute)"}}`. Printing takes
  0.75 s per item, and the items land on the ChemMaster's tile. `stopPrinting` stops it.
- Read `data.beaker.contents` and `data.buffer.contents`: each entry has `name`, `volume`, `pH`, **`purity`** and
  `overdose`.

**smart chemical storage** (window "SmartVend"). To load it, click it with a container in your active hand (not
in combat mode). It accepts pills, patches, filled bottles, tubes, beakers, syringes, sprays and medical gels, and
a pill bottle full of pills or patches. Click it with a **chemistry bag** to load everything in the bag at once. To
take something out: `Release {path, amount}` (the window lists the paths). It needs power to open.

## 5. The reaction system, briefly

- A reaction starts on its own once all its ingredients are in one container and the temperature is at least the
  required one (a cold recipe like Seiver needs it *at or below*). Ratios are by units: "1 Water + 1 Chlorine +
  1 Oil → 3 Phenol" means 10 + 10 + 10 makes 30. Leftover ingredients just stay in the beaker. Wait for each
  step to finish, until the ingredients are gone from `data.beaker.contents`, before you add the next step's.
  Otherwise the ingredients can pair up with each other in the wrong reaction.
- **Heat**: many reactions heat their beaker as they run (Libital, Mannitol and Synthflesh do), and some cool it
  (Aiuri, Seiver). Above a recipe's **overheat** temperature it loses yield, and for some recipes that's a bang,
  a flash or a fire (see §8). Check `data.currentTemp` in the reaction chamber.
- **pH and purity**: every chemical has a pH, and the beaker's pH is their volume-weighted average. A product's
  purity is 1.0 while the pH sits inside the recipe's range. It drops off outside that range, and a reaction
  won't even start if the pH is more than a few points out (4 for most medicines). Purity also carries over:
  impure Oil makes impure Phenol, which makes impure Libital. Yesterday's unbuffered chain gave Oil 0.48, Phenol
  0.67 and Libital 0.56, all usable.
- **What impurity does**: medicine heals in proportion to its purity. Below a threshold (0.3 for Libital and
  Oxandrolone, 0.35 for Aiuri, 0.45 for Mannitol) the *whole dose* turns into a harmful "inverse" chemical once it's
  inside the patient. Aim for 0.6 or better, and don't hand out anything under 0.45.
- pH of the raw chemicals. Strongly acidic: Hydrogen 0.1, Fluorine 2, Sulfuric Acid 2.75, Welding Fuel 4, Carbon 5.
  Basic: Oxygen 9.2, Aluminium 10, Lithium 11.3, Sodium and Ammonia 11.6, Diethylamine 12. Everything else is about
  7 (Water, Nitrogen, Chlorine 7.4, Blood 7.4, Sugar).
- **Buffers**: 1u of Strong Basic Buffer raises the beaker's pH by 30 ÷ (units in the beaker), and acidic buffer
  lowers it by the same amount. The buffer adds no volume. Example: 30u at pH 3, to bring it to 7, needs 4 × 30 ÷ 30
  = 4u of basic buffer. Inject it from the reaction chamber, or pour from a buffer bottle.
  Make more: **Strong Basic Buffer** = 3 Ammonia + 2 Chlorine + 2 Hydrogen + 2 Oxygen → 10. **Strong Acidic
  Buffer** = 2 Sodium + 2 Hydrogen + 2 Ethanol + 2 Water → 10. Both need 250 K or more, so room temperature works.
- Good practice: pH about 7 when the last ingredient goes in; about 9 for Libital and Synthflesh, whose
  reactions pull the pH down as they run.

## 6. Recipes (verified in this version's code)

Temperatures are kelvin. The dispenser gives 300 K, so a recipe that needs 300 or less works at room temperature.
"Overheat" is where yield loss or trouble starts. "pH" is the full-purity range.

**Intermediates**

| Product | Ingredients → yield | Temp | Notes |
|---|---|---|---|
| Oil | 1 Welding Fuel + 1 Carbon + 1 Hydrogen → 3 | room | acidic mix: buffer it toward 7 |
| Phenol | 1 Water + 1 Chlorine + 1 Oil → 3 | room | base of Libital, Oxandrolone, Salicylic Acid, Epinephrine |
| Acetone | 1 Oil + 1 Welding Fuel + 1 Oxygen → 3 | room | never with Ethanol (makes Napalm) |
| Ammonia | 3 Hydrogen + 1 Nitrogen → 3 | room | |
| Diethylamine | 1 Ammonia + 1 Ethanol → 2 | room | make it in its own beaker |
| Ash | 1 Oil → 1 | 480+ | set the reaction chamber to 500 |
| Table Salt | 1 Sodium + 1 Chlorine → 2 | room | the Cook's salt |
| Saltwater | 1 Water + 1 Table Salt → 2 | room | |
| Unstable Mutagen | 1 Radium + 1 Phosphorus + 1 Chlorine → 3 | room | toxic: label it, give it only to Botany (for plants) |
| Saltpetre | 1 Potassium + 1 Nitrogen + 3 Oxygen → 3 | room | for Botany; **no water in that beaker** |
| Space Cleaner | 1 Ammonia + 1 Water → 2 | room | for the Janitor |
| Granibitaluri | 1 Table Salt + 1 Carbon + 1 Sulfuric Acid → 3, needs 5u Iron in the beaker (not used up) | room | mild filler painkiller; heals small wounds |

**Medbay stock**

| For | Medicine | Ingredients → yield | Temp (start / overheat) | pH | What it does (per unit, at the purity the reaction usually gives) |
|---|---|---|---|---|---|
| Brute | **Libital** | 1 Phenol + 1 Oxygen + 1 Nitrogen → 3 | 225 / 840 | 6-10 | ~15 brute per unit; ~1.5 **liver** damage per unit; no overdose. Its reaction drives the pH down hard (yesterday it ended at 1.7). |
| Brute | **Salicylic Acid** | 1 Sodium + 1 Phenol + 1 Carbon + 1 Oxygen + 1 Sulfuric Acid → 5 | 100 / 900 | 5-10 | ~20 brute per unit while brute is over 25, ~2.5 below that; no side effects; **overdose 25** (worsens bruises) |
| Burn | **Oxandrolone** | 3 Carbon + 1 Phenol + 1 Hydrogen + 1 Oxygen → 6 | 100 / 900 | 5-10 | ~20 burn per unit while burn is over 25, ~2.5 below that; **overdose 25** (worsens burns) |
| Burn | **Aiuri** | 1 Ammonia + 1 Sulfuric Acid + 2 Hydrogen → 4 | 50 / **315** | 4.8-9 | ~10 burn per unit; ~1.25 **eye** damage per unit: 24u blinds, so dose 10u. It cools itself; above 315 K it bangs and flashes. |
| Toxin | **Seiver** | 1 Nitrogen + 1 Potassium + 1 Aluminium → 3 | cold recipe: runs at **320 or below** (fine at 300) | 5-8 | ~5 toxin per unit at room temperature; ~1 heart damage per 5 healed; no overdose. **Potassium: no water in that beaker, ever.** |
| Toxin | **Multiver** | 1 Ash + 1 Table Salt → 2 | **380 / 410** | 5-9.5 | weak alone (~2.5 toxin per unit, ~2.5 lung damage per unit), stronger the more *different* medicines the patient has in them; it **purges other medicines** unless the patient has 2 others in them. Preloaded pills exist. |
| Oxygen | **Salbutamol** | 1 Salicylic Acid + 1 Lithium + 1 Aluminium + 1 Bromine + 1 Ammonia → 5 | 100 / 900 | 5-10 | ~30 suffocation per unit, stops breath loss; no overdose |
| Oxygen | Convermol | 1 Hydrogen + 1 Fluorine + 1 Oil → 3 | 370 / 570 | 3-8.5 | skip it: an impure batch makes a pressure blast |
| Crit | **Epinephrine** | 1 each of Phenol, Acetone, Diethylamine, Oxygen, Chlorine, Hydrogen → 6 | 100 / 900 | 5-10 | for patients in critical condition: ~5 of each damage type per unit, stops breath loss; **overdose 30**. Already stocked (§3). |
| Revival | **Synthflesh** | 1 Blood + 1 Carbon + 1 Libital → 3 | 250 / **325** | 5.5-9.5 | on contact (patch, medical gel, splash, spray): heals **1.25 brute and 1.25 burn per unit, on corpses too**; adds toxin worth 50-75% of what it healed. 60u at 100% purity (100u at lower purity) un-husks a burnt corpse once its burn is 50 or less. |
| Brain | **Mannitol** | 1 Sugar + 1 Hydrogen + 1 Water → 3 | 50 / 650 | 5-7.5 | ~5 brain damage per unit; **overdose 15**: dose 10u |
| Blood loss | **Saline-Glucose Solution** | 2 Saltwater + 1 Sugar → 3 | 100 / 900 | 5-10 | stands in for blood for a while and speeds blood regeneration; small random brute and burn healing; overdose 60 |
| Cryo | Cryoxadone | 1 Stable Plasma + 1 Acetone + 1 Unstable Mutagen → 3 | 100 / 900 | 5-10 | works only while the body is below 273 K (cryo cells). Cryogenics already has 4 beakers. Add the Stable Plasma last: with leftover Radium + Phosphorus it makes Pyrosium, with Radium + Carbon a vortex. |
| Eyes | Oculine | 1 Multiver + 1 Carbon + 1 Hydrogen → 3 | 200 / 600 | 4.8-8.5 | heals eyes; overheating flashes |
| Ears | Inacusiate | 1 Water + 1 Carbon + 1 Multiver → 2 | 300 (heat it to ~350) / 500 | 5-10 | heals ears; overheating gives a deafening bang |

Not makeable here: **Sanguirite** (coagulant: no recipe; doctors use gauze and sutures), **Omnizine** (no recipe).
Lenturi needs silver, Syriniver needs Toxin (the dispenser has none), and Pentetic Acid needs cyanide, so skip them.

**Strange Reagent** exists: 1 Omnizine + 1 Holy Water + 1 Unstable Mutagen → 3 (alternative: Protozine in place of
Omnizine → 2). Without Omnizine you can't make it, and **Omnizine has no reaction at all**. It only comes from
plants (Ambrosia Deus, a mutation of Ambrosia Vulgaris; Lifeweed, a cannabis mutation), ground in a reagent grinder
and split out in the ChemMaster, or from warmed Donk Pockets. Holy Water is in the Chapel Office. Even with it,
Strange Reagent has to be **fed** to a corpse (by mouth). It fails on a husk, and on a corpse with more than 200
brute + burn combined; it needs about (brute + burn − 100) ÷ 5 units. So the revival plan is **Synthflesh +
defibrillator** (see §7.4), not Strange Reagent. Tell the surgeon this early, so nobody waits for it.

## 7. Core procedures

### 7.1 Shift start (first 10 minutes)
1. `walk_to {area: "Pharmacy"}` (or "Chemistry"). Put your goggles on if they aren't already.
2. Take **two large beakers** from the tables. In the Pharmacy, open the chemical closet: take a box of pill
   bottles and two or three medical gels. Vend a **chemistry bag** from the ChemDrobe in Chemistry, or skip it.
3. Open the dispenser and check `data.displayedUnits`. Open the reaction chamber: check its buffers, set it to
   300 K and switch it on, so it holds beakers at a safe temperature.
4. One line on Common radio, one on Medical: what you're making and where it will be. Ask the surgeon (Medical
   radio) what they want first.
5. Decide where the stock goes and say it once on Medical: **the smart chemical storage fridge that opens onto
   Medbay Central**, the one beside the Pharmacy door if you work in the Pharmacy, or the one beside the
   Chemistry door. The lobby-facing fridge in the Pharmacy's north wall is open to anyone in the Medbay Lobby: put
   only a few brute and burn patches there.

### 7.2 First stock, in order (aim: done within 20 minutes)
Each batch fits one 100u large beaker, using only allowed dispenser steps. Wait for each step to finish before
the next.

**Batch A, Libital and the Synthflesh base:**
1. Welding Fuel 5, Carbon 5, (optional, for purity: about 2u of basic buffer from the reaction chamber),
   Hydrogen 5 → 15 Oil.
2. Water 10, Chlorine 10 → 30 Phenol (5 Oil is left over and does nothing).
3. Bring the pH to about 9 (basic buffer). Oxygen 30, Nitrogen 30 → 90 **Libital**. If `activeReactions` shows
   the quality dropping as the pH falls, inject more basic buffer during the reaction.
4. ChemMaster: transfer 60 Libital to the buffer. Select a brute patch style, `create {itemCount: 6}`, and name
   them "Libital patch 10u (brute)". Leave the other 30 Libital in the beaker for Synthflesh.

**Batch B, Synthflesh** (in the same beaker, with its 30 Libital):
1. Blood: take an empty syringe (Medbay Storage, box of syringes). Hold it and **right-click yourself** to draw
   15u (instant), then left-click the beaker to inject it (5u per click; use the syringe in hand, key Z, to change
   the amount). Two draws give 30u. Losing 30-45u is harmless: a body holds about 560u. A doctor can also hang a
   blood pack on an IV drip and drag the drip onto the beaker.
2. Check the temperature (the reaction chamber at 300) and the pH. Raise the pH to 8-9 with basic buffer: the
   Libital is acidic, and below pH 2.5 Synthflesh won't even start.
3. Carbon 30 (dispenser) plus the 30 Blood → 90 **Synthflesh**. **Keep it under 325 K**: if the beaker is warm,
   hold it in the reaction chamber at 300 while it reacts.
4. ChemMaster: transfer 80 Synthflesh to the buffer and print 2 patches, "Synthflesh patch 40u (corpse
   brute+burn)". Pour the 10u left in the beaker into a medical gel (click the gel with the beaker in hand: a
   beaker pours 10u by default).

**Batch C, burn** (Oxandrolone): Welding Fuel 5, Carbon 5, Hydrogen 5 → 15 Oil. Water 5, Chlorine 5 → 15 Phenol
(10 Oil left over). pH to about 7. Carbon 25 + 20, Hydrogen 15, Oxygen 15 → 90 **Oxandrolone**. Print **20u**
patches (it overdoses at 25), "Oxandrolone patch 20u (burn)". Or make Aiuri for burn: Hydrogen 15 + Nitrogen 5
(→ 15 Ammonia), Sulfuric Acid 15, Hydrogen 30 → 60 Aiuri, printed as **10u** patches.

**Batch D, toxin** (Seiver): a clean, **dry** beaker. Nitrogen 30, Potassium 30, Aluminium 30 → 90 **Seiver**.
It's already near pH 8 and needs no heating. Print 15u patches, "Seiver patch 15u (toxin)". The fridges' Multiver
pills are the backup.

**Batch E, oxygen** (Salbutamol): first Salicylic Acid. Fuel 5, Carbon 5, Hydrogen 5 → Oil. Water 5, Chlorine 5
→ 15 Phenol. *After* the Chlorine is used up: Sodium 15, Carbon 15, Oxygen 15, Sulfuric Acid 15 → 75 **Salicylic
Acid**. Move 60 to the ChemMaster buffer and print 20u brute patches. To the 15 left in the beaker add Hydrogen
15 + Nitrogen 5 (→ Ammonia), then Lithium 15, Aluminium 15, Bromine 15 → 75 **Salbutamol**: print 10u patches,
"Salbutamol patch 10u (oxygen)".

Then: label, stock and announce (§7.3). After that, Mannitol (10u pills), Saline-Glucose (a beaker or 30u tubes
for IV drips and syringes: Sodium 10 + Chlorine 10, Water 20, Sugar 20 → 60), and a second Synthflesh batch.

### 7.3 Labelling, stocking and announcing
- Name every print in the ChemMaster: **medicine, units, damage type**. To label a beaker, tube, gel or pill
  bottle, use the **hand labeler** (Pharmacy east table): use it in hand (key Z), type the label into its "Label
  text" box, then click the item.
- A **pill bottle** holds pills and patches. With the bottle in hand, click a pile on the floor to scoop it up.
  A **chemistry bag** (50 items) does the same, and loads the fridge in one click.
- Put the stock in the agreed fridge. Keep a few brute and burn patches in your pockets or bag for emergencies.
- Announce exact counts on Medical: "Fridge by the Pharmacy door: 6 Libital 10u, 4 Oxandrolone 20u, 6 Seiver 15u,
  5 Salbutamol 10u, 2 Synthflesh 40u, 1 Synthflesh gel." One line on Common when the first stock is in.
- Every 15 minutes: open the fridge (`tgui_window`), count, and remake whatever is low.

### 7.4 Revival support (with the surgeon)
- A defibrillator fails when a corpse has **180 or more brute, or 180 or more burn**, when it's husked, or when
  its heart or brain is failing ("heart too damaged" means the heart organ: that's surgery, not you).
- Synthflesh is the chemist's answer. It acts on contact, so a corpse that no longer processes medicine still
  heals from it. Other patches are wasted on the dead: their medicine goes in but nothing happens, and the patch
  falls off empty. That's what happened yesterday.
- Ways to apply it to a corpse: a **40u patch** (heals ~50 brute + 50 burn over about a minute; clothing doesn't
  matter); a **medical gel** (10u per spray, instant); or **splash** a beaker (combat mode on, right-click the body
  with the open beaker: everything in it at once, but suits and labcoats block part of a splash, so strip them first).
- Example: a corpse at 250 brute needs at least 60u of Synthflesh to drop below 180 brute. Make 90u per batch and
  keep at least one 40u patch and one gel in stock at all times.
- Husked bodies (burnt to a husk): heal the burn to 50 or less first, then give 60u of pure Synthflesh, or 100u at
  lower purity.

### 7.5 The ongoing loop
Restock, answer requests, then make the next most useful thing: Synthflesh, Mannitol, Saline-Glucose, more of
whatever ran out. Keep one empty large beaker ready. Empty a beaker with the dispenser's `remove {amount: 100}` (50 for a small
one), and never reuse a beaker for a different recipe without emptying it. Clicking a disposal bin with an item
throws the item away (yesterday a doctor lost a medkit that way).

## 8. Dangers and common mistakes

**Reactions never to make by accident** (they happen as soon as the ingredients meet, unless a temperature is
given):

| Ingredients together | Makes | What happens |
|---|---|---|
| **Water + Potassium** (or Holy Water + Potassium) | explosion | instant blast, bigger with more volume |
| **Diethylamine + Iodine + Phosphorus + Hydrogen**, at 300 K | explosion | strong even in small amounts. Epinephrine work involves Diethylamine and Hydrogen: keep Iodine and Phosphorus away. |
| Aluminium + Potassium + Sulfur | Flash Powder | instant blinding flash; people within 3 tiles knocked down |
| Potassium + Sugar + Phosphorus | Smoke Powder | instant smoke carrying the whole beaker over the room |
| Phosphorus + Sulfuric Acid + Stable Plasma | Phlogiston | releases burning plasma gas: a plasma fire in your lab |
| Stable Plasma + Radium + Phosphorus | Pyrosium | heats violently once oxygen is present |
| Mercury + Oxygen + Nitrogen + Carbon | Sorium | instant vortex that throws people and items |
| Stable Plasma + Radium + Carbon | Liquid Dark Matter | instant vortex that pulls everything in |
| Chlorine + Fluorine, heated to 424 K+ | Chlorine Trifluoride | fire on every tile around. Never heat a beaker that holds both. |
| Ammonia + Nitrogen + Oxygen at 525 K+ | Nitrous Oxide | explodes at 575 K |
| Aluminium + Iron + Oxygen | Thermite | burns through walls once lit |
| Oil + Welding Fuel + Ethanol | Napalm | sticky fuel; a fire if lit |
| Water + Silicon + Oxygen | Space Lube | makes floors slippery. Never give it out. |
| Ethanol + 3 Chlorine + Water | Chloral Hydrate | knockout poison |
| Silicon + Hydrogen + Multiver | Mindbreaker Toxin | hallucinogen |
| Oil + Ammonia + Oxygen, 380 K+ | Cyanide | lethal poison |
| Penthrite + Epinephrine or Atropine | explosion | |

Recipe-specific overheats: **Aiuri above 315 K** (a bang and a flash that blurs eyes nearby); **Synthflesh above
325 K** (yield loss); **Multiver above 410 K** (yield loss, fire if it went impure); Oculine above 600 (flash);
Inacusiate above 500 (deafening bang); Helbital and Convermol (fire, a pressure blast), which you shouldn't make.

Common mistakes:
- Dumping several recipes' ingredients into one beaker at once. Make intermediates first, let each step finish,
  and use the ChemMaster to move just the product into a clean beaker.
- Forgetting the leftovers. Before reusing a beaker, look at `data.beaker.contents`, especially for Potassium,
  Phosphorus, Iodine, Stable Plasma, Fluorine and Water.
- Overdose by patch. A patch feeds 0.75u per second while the body uses only about 0.1u per second, so nearly
  the whole patch ends up inside the patient at once. Keep each patch under the overdose: Oxandrolone and
  Salicylic Acid 20u, Mannitol 10u. Keep Aiuri at 10u (eyes) and Libital at 10-15u (liver). Write the dose on the
  label so doctors don't stack two.
- Waiting to be asked. Yesterday's Chemist made two kinds of patch and stopped. Stock every damage type, plus
  Synthflesh, before anyone asks.
- Yesterday's dead-end: a Strange Reagent revival with no Omnizine (§6). Synthflesh first, every time.
- From yesterday: dispense answers sometimes hide the new contents under "changed too, as it does by itself":
  read `data.beaker.contents` to see them.

## 9. Emergencies

- **Power failure**: the dispenser, ChemMaster, reaction chamber and fridges stop working (fridges won't open
  without power). Hand out what's in your bag. Tell the engineers on Common which room lost power ("APC for
  Pharmacy").
- **Fire in the lab**: step out and close the door. Use the fire extinguisher (Pharmacy east wall). If you're on
  fire, stand under an emergency shower (Chemistry north wall, Pharmacy west side) or stop, drop and roll (see
  crew-basics).
- **Breach or bad air**: leave, put on the breath mask and internals from your survival box, and report the room.
- **Mass casualties**: fill your bag with every brute, burn and Synthflesh item and go to the Medbay Treatment
  Center. Patch whoever the doctors point at (a patch takes 1.5 s and works on someone unconscious), then go back
  and make more Synthflesh and Libital.
- **Evacuation**: leave a full stock in the fridge, take a bag with a few patches of each kind and a Synthflesh
  gel, and board with the crew.

## 10. Defending yourself and chemistry

Your stance is in your personal file. The general combat moves (combat mode, shoving, grabs, resisting) are in
crew-basics. What your job gives you:
- **Shut doors.** Both labs are access-locked: don't hold doors open for anyone who has no business inside.
  Hand things over through a desk instead. If someone hostile is coming, close the shutters ("chemistry lockdown
  control", or the two "pharmacy shutters control" buttons). This also blocks that lab's fridge, so tell the doctors.
  Ask the AI to keep the lab doors closed to strangers, and to open them for you if you're locked out.
- **Weapons at hand**, all ordinary tools: the mechanical toolbox (Chemistry east table) and the fire extinguisher
  (Pharmacy east wall) each hit for 13 damage. Shoving someone back out of the door and closing it often ends it.
- **Never use chemicals on people**: no poison, no smoke, no flash powder, no splash, no syringe gun, even in
  self-defence. Never hand out anything harmful (Lube, Chloral Hydrate, Mutagen to anyone but Botany for plants,
  explosive powders, Potassium to a stranger). If someone wants "something for self-defence", the answer is no.
- When you're hurt: patch yourself (with the patch in hand, click yourself), then get to a doctor. If a doctor or
  patient is attacked in medbay, call it on Medical and Common radio with the attacker's name and where they are.
  You have no Security channel: report on Common.

## 11. Working with the crew

Crew roles that matter to you (the list is not exhaustive: more players can join at any time, in any job, such as
a Chief Medical Officer, Paramedics, another Chemist, or a Bartender):
- **Medical Doctors** (usually one on treatment and surgery, one in the field): they use your stock. Ask the
  surgeon what revival needs; give the field medic patches to carry. A **Chief Medical Officer**, if on shift, is
  your boss.
- **Botanist**: you give Unstable Mutagen (mutations), Saltpetre (+potency, faster growth), Diethylamine (+yield,
  fewer pests), Ammonia (plant health) and Multiver (clears tray toxins). They can give you plants to grind,
  including the Ambrosia line that leads to Omnizine. Weed Killer and Pest Killer need Toxin, which the dispenser
  doesn't have; Botany has its own nutrient vendor.
- **Cook**: Table Salt (Sodium + Chlorine), Sugar straight from the dispenser. The station has no Universal Enzyme
  recipe.
- **Janitor**: Space Cleaner (Ammonia + Water) refills.
- **Scientist**: may want Sulfuric Acid; can upgrade your machines (tier-4 servos add Oil, Acetone, Ammonia and
  more to the dispenser).
- **Quartermaster**: orders for what you can't make. **Engineers**: medbay's power. **AI**: doors. **Security
  Officers**: removing intruders; medicine for prisoners (never poison).
- Requests also come by the **Pharmacy Requests Console** and the lobby desk bell.

## 12. Through the client

- `search` for "chem dispenser", "reaction chamber", "ChemMaster", "smart chemical storage", "large beaker", then
  `walk_to {object_id, adjacent: true}`. Pick up with `command {line: "pick-up large beaker"}`. Many interactions
  want an empty hand: swap hands with key X.
- After `tgui_act`, read `tgui_window {id, path: "data.beaker"}`. Recipe lookup: `tgui_window {id, find:
  "/Seiver|Salbutamol/"}` on the dispenser, then `path: "static_data.reaction_list.Seiver"`.
- `create` on the ChemMaster opens a second window (TextInputModal). Its answer can say "data_changes: none" just
  before the modal appears: that's normal. Submit the name in the new window, then pick up the prints from the
  ChemMaster's tile.
- Right-click is `click {object_id, right: true}`: it ejects the dispenser's beaker, and with a syringe in hand it
  draws blood (click yourself). Splashing needs combat mode on plus a right-click.
- To apply a patch, hold it in the active hand and click the patient. The answer says it "sticks itself to" them.
  To give someone an item, hold it in the active hand: the offer uses the active hand only.
- `wait {until: "/chem|pharm|patch|synthflesh/"}` waits until someone asks for you; `mute` cuts fight spam.

## 13. Checklist

Shift start:
- [ ] Go to the Pharmacy or Chemistry. Goggles on. Two large beakers, pill bottles, medical gels, a chemistry bag.
- [ ] Reaction chamber on, at 300 K. Check the buffers and the dispenser's energy.
- [ ] Announce on Medical and Common. Ask the surgeon's priorities. Name the stock fridge.
- [ ] Batches A-E: Libital, Synthflesh, Oxandrolone or Aiuri, Seiver, Salbutamol. Print, label, stock, announce counts.

Every 15 minutes:
- [ ] Count the fridge and remake what's low (Synthflesh always at least one 40u patch and one gel).
- [ ] Answer requests (desk bell, requests console, radio), harmless ones only.
- [ ] Check your health; keep the doors shut; empty and reuse beakers safely.

End of shift: leave a full stock, take a bag of patches to the shuttle.

## 14. Sources

- Code (tgstation 54c22023): `code/modules/jobs/job_types/chemist.dm`, `code/datums/id_trim/jobs.dm`; `code/modules/reagents/chemistry/` (machinery/, recipes/, reagents/, equilibrium.dm, holder/); `code/modules/reagents/reagent_containers/`; `smartfridge.dm`; tgui `ChemDispenser`, `ChemMaster`, `ChemHeater`, `SmartVend`; defib checks in `mob/living/carbon/carbon.dm`.
- Map: `_maps/map_files/MetaStation/MetaStation.dmm`; areas `code/game/area/areas/station/medical.dm`.
- Yesterday's round: the Chemist's and the Medical Doctor's own reports.
- /tg/station wiki (CC BY-SA 3.0): "Chemist", "Guide to chemistry" (where they disagree with the code, e.g. "the ChemMaster prints bottles", this guide follows the code).
