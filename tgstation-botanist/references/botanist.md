# Botanist

## The job in one paragraph

You run Hydroponics: you grow food for the Cook (and drinks fruit for a bartender, if one is on shift), medicinal
plants for the Chemist and medbay, and flowers for the crew. Success is simple and measurable: the trays never die
of neglect, the kitchen always has fresh produce, every harvest goes into a plant bag and then into the smartfridge
(never onto the floor), and the Chemist gets the plants they ask for. A tray is a machine with a clock: every
**20 seconds** it ages the plant one "cycle" and uses up water and nutrients. Almost everything that goes wrong in
botany is a tray that ran dry of nutrients or water while you were elsewhere. Other botanists may join the shift:
if they do, split the trays and the deliveries.

## Starting kit and access

You spawn with (from the job's outfit in code):

| Slot | Item |
|---|---|
| Uniform / suit | botanist's jumpsuit, apron |
| Suit storage | **plant analyzer** |
| Belt | botanist PDA |
| Ears | **service radio headset**: Service channel (key `:v`) and Common (`;`) |
| Gloves | **botanist's leather gloves**: make you safe from thorns, nettles and other "backfire" plants |
| Back | botany backpack (or satchel/duffel) |

More gear is in the three **botanist's lockers** in the Hydroponics backroom (each: **portable seed extractor**,
plant analyzer, service headset, **cultivator**, **hatchet**, **secateurs**). Take one locker's contents at shift
start; leave the others for other botanists.

**Access**: Hydroponics, Service, Mineral Storeroom. On rounds that start with 20 or fewer players you also get
Bar, Kitchen and Morgue access. Your boss is the **Head of Personnel** (head of Service).

The NutriMax and MegaSeed Servitor charge your ID card, but your Service card pays only 20% of the list price
(about 5 credits a seed pack, 10 for an E-Z-Nutrient can).

## Where things are on MetaStation

**Hydroponics** (area "Hydroponics") is on the east side of the **Central Primary Hallway**, south of the
**Service Hallway**, the **Kitchen** and the **Bar**. Doors: a glass airlock in the west wall (to the Central
Primary Hallway) and one in the north wall (to the Service Hallway); both need Hydroponics access. The west wall
also has the **Hydroponics Desk** (two windoors on a counter with a desk bell) where anyone can ask you for things.

Inside the main room:
- **North wall**, west to east: **MegaSeed Servitor** (seeds), **NutriMax** (nutrients, tools), **SapMaster XP**
  (a condiment-only ChemMaster), a glass table with the **all-in-one grinder**, a table with a box of syringes and a
  box of beakers. A **Service Shutter Control** button is on this wall.
- **North wall, further east**: a **stationary water tank** and two **high-capacity water tanks**, each with a
  **watering can** on it.
- **North wall, in the wall itself** (reachable from both Hydroponics and the Service Hallway): the
  **smartfridge**, the **Hydroponics Window** (a windoor over a small table), the **biogenerator**, then the north
  door. Shutters ("Service Shutter") can close over the smartfridge and the window.
- **Centre**: **16 hydroponics trays** in five north–south rows with walkways between them (the westmost row has 3
  trays, the next 4, the other three 3 each). Trays in the same row touch each other; rows don't.
- **East side**: the **seed extractor**, and a table with free starter seeds (wheat, sugarcane, potato, apple) and
  some produce (a corn cob, a carrot, wheat, a pumpkin) you can turn into more seeds. A disposal bin is in the
  south-west corner, the room's **APC** on the south wall, the **Hydroponics Requests Console** on the west wall.
- **Hydroponics Backroom** (east, through the "Hydroponics Backroom" airlock, same area name): 3 botanist's
  lockers, the **Hydrobe** (botany clothing), a **sink**, a table with three **Plant-B-Gone** sprays, a backpack
  water tank and a weedkiller grenade, and a **hydroponics crate** (spade, wrench, watering can, cultivator,
  wirecutters).

A second **MegaSeed Servitor** and **NutriMax** stand in the Central Primary Hallway just outside the west door.

**Service Hallway** (north of Hydroponics): the **Kitchen Window** (a counter with a windoor into the Kitchen; you
put things on its table from the hallway side, the Cook takes them from inside), a table with a spare plant bag and
watering can, a water tank, the Service fax and the service techfab.

**Garden** (area "Garden", a public room east of the **Locker Room**, well north of Hydroponics): **6 rich soil**
plots in two east–west rows of three, its own **biogenerator** and **seed extractor**, a puddle you can fill a
watering can from, and wooden tables with 3 hatchets, cultivators, a plant analyzer, a plant bag, a watering can,
a bottle of E-Z-Nutrient, a bottle of Robust Harvest, a Plant-B-Gone and a pest spray. Soil plots need no power
and have no autogrow.

Backup: **Aft Starboard Maintenance** has 8 plain soil plots, a biogenerator and a seed extractor.

## How a hydroponics tray works (this version, from the code)

Every 20 seconds (one **cycle**) a tray with a living plant does, in order:

1. **Age** +1.
2. **Nutrients**: each nutrient chemical in the tray (at least 1u of it) acts on the plant (table below), then the
   tray loses **1u** of nutrients in total. The tray holds **20u** (a soil plot 20u too, plain soil 15u). At round
   start each tray and plot holds 10u of E-Z-Nutrient and 100 water.
3. **No nutrients left**: the plant loses **1-3 health every cycle**. This is what killed yesterday's plants. Any
   chemical in the tray counts as "nutrients" for this check.
4. **Light**: in a dark tile (lights off, power cut) the plant loses 2 health per cycle (mushrooms 1, and they
   tolerate dim light).
5. **Water**: the plant drinks **1-6** (about 3.5) per cycle out of **100**. At 10 or less it loses health; at 0 it
   loses more. With water above 10 *and* some nutrients, it **gains 1-2 health** per cycle.
6. **Weeds** grow: about 10% chance per cycle of +1 (more for some plants). At **5+ weeds** the plant loses 1-2
   **yield** per cycle (not below 3). An **empty** tray that has water and nutrients also grows weeds (10% per cycle), and at 10
   weeds a weed plant (reishi, nettles, harebells, fly amanitas, chanterelles, tower caps, plump helmets or
   starthistle) takes the empty tray over. That is where yesterday's fly amanitas came from.
7. **Pests**: 5% per cycle +1. At 4+ pests, plants with potency 30 or more lose potency. Pests don't kill.
8. **Toxins** (from pest spray and other poisons): harmless below 40, then cost health.
9. **Cross-pollination** with touching trays (same row): each cycle the neighbours' yield moves halfway toward this
   plant's, their potency and instability 10% toward it.
10. **Instability** effects (see Mutations).
11. **Health 0** = the plant dies ("It's dead!"); weeds +1.
12. **Old age**: once age passes the plant's **lifespan**, it loses 1-5 health per cycle and soon dies.
13. **Harvest ready**: first at age **maturation + production** cycles; a perennial plant ("Perennial Growth")
    then again every **production + 1** cycles. A single-harvest plant leaves the tray empty when harvested.

The plant's **maximum health is its endurance** (often only 10-15), so a neglected plant dies in 2-4 minutes.

**Nutrient chemicals** (each acts every cycle while 1u+ of it is in the tray; V = its volume in the tray):

| Chemical (where) | What it does each cycle |
|---|---|
| **E-Z-Nutrient** (NutriMax "E-Z-Nutrient™ can", 200u; biogenerator) | potency +V×0.3 (3 at 10u, 6 at 20u), **yield +1 at 10-19u, +2 at 20u**, instability +0.2 |
| **Robust Harvest** (NutriMax can; biogenerator) | **yield +1 at 5-9u, +2 at 10-14u, +4 at 20u**, potency +1 per 10u, instability −0.25 |
| **Left 4 Zed** (NutriMax can; biogenerator) | health +1 per 10u, **instability +2 at 10u** (mutations) |
| Enduro Grow (biogenerator) | endurance up, potency and yield down |
| Liquid Earthquake (biogenerator) | faster production, more weeds |
| Water (tanks, sink, puddle) | fills the water level |

Yield caps at 10, potency at 100. So **a tray kept at 10-20u of E-Z or Robust Harvest reaches yield 10 within a
few minutes**; that is how to get big harvests.

**Never put these in a tray**: **Plant-B-Gone** (despite "Kills those pesky weeds!", it takes 10 health per unit
every cycle: it kills the plant), acids, chlorine, fluorine, sugar or honey (weeds and pests), blood (pests),
**mutagen, unstable mutagen, uranium or radium** (can turn weeds into kudzu or death nettles, or pests into
spiders), **strange reagent** (spawns a killer tomato or a killer tree). Pest spray is fine in small doses.

**Autogrow** (Ctrl-click a powered tray; Garden soil has none), what it really does:
- adds water continuously, removes weeds and pests continuously, **halves nutrient use** (0.5u per cycle, so 20u
  lasts about 13 minutes instead of 7), lights the tray up, and blocks species mutation from high instability;
- it **does not add nutrients**: the plant still dies when they run out. The message "maintaining the tray's
  health" means water, weeds and pests only;
- it costs **1 kW per tray** from the Hydroponics APC, switches itself off when the room loses equipment power,
  and when a single-harvest plant is harvested.
Use it on trays you will be away from, if the station has power to spare. Turn it off (Ctrl-click again) during
power trouble.

**What examine on a tray shows**: "It has Tomato Plants planted." then one of "It's dead!", "It's ready to
harvest.", "It looks unhealthy." (health at half or less); "Water: 64/100.", "Nutrient: 13/20."; the autogrow line
if on; "It's filled with weeds!" (5+), "It's filled with tiny worms!" (pests 5+). A tray's name includes its plant:
"hydroponics tray (Tomato Plants)".

**The plant analyzer** (click a tray, a seed pack or a produce with it in hand) opens a "Plant Analyzer" window:
the tray's plant health, age, water, nutrients (and which chemicals), light, weeds, pests, toxins, and the seed's
potency, yield, instability, maturation, production, lifespan, endurance, traits, chemical contents and possible
mutations. It keeps updating while you stay next to the last tray you scanned. Right-click with it for the
chemicals tab.

## Core procedures

### Shift start (first 10 minutes)
1. `walk_to` area "Hydroponics". Open one **botanist's locker** in the backroom: take the cultivator, hatchet,
   secateurs and portable seed extractor.
2. Get a **plant bag** (NutriMax sells 5; spares on the Service Hallway table and in the Garden) and keep it in a
   hand. If you want both hands free, move the PDA from your belt to your backpack and wear the plant bag on the
   belt.
3. At the NutriMax buy an **E-Z-Nutrient™ can** and a **Robust Harvest™ can** (200u each; they are bulky: carry
   them in a hand, or set them down on a table in the room).
4. Pick up a **watering can**. Set it to 100u (use it in hand once: it switches 20 ↔ 100; examine confirms). At
   100u one click on a water tank fills it, one click on a tray tops that tray to 100 and uses only what it needed.
5. Set the nutrient can to **30u** (use it in hand: 10 → 15 → 30). One click then tops a tray up to 20u.
6. Ask the Cook (Service radio) what they want, and the Chemist if they have a wish list.
7. Buy seeds at the MegaSeed Servitor (3 packs of each kind per machine) and plant (below). Announce once on
   Common that Hydroponics is open.

### Planting
1. Hold the seed pack, click an **empty** tray ("You plant the tomato seed pack.").
2. Click the tray with the nutrient can (to 20/20) and the watering can (to 100/100).
3. Plant the same crop along a whole row; keep high-instability plants (corn) in a row of their own.
A dead plant: click the tray with an empty hand to remove it. A living plant you don't want: use a **spade**
(NutriMax, backroom crate) on the tray ("Clear tray", 5 seconds).

### The tending loop (every 5 minutes, all planted trays)
- **Nutrients**: one click with the can at 30u. 20u lasts about 7 minutes (13 on autogrow). Never let it reach 0.
- **Water**: one click with the can at 100u. 100 water lasts about 9 minutes.
- **Weeds**: click the tray with the **cultivator** at 5+ weeds ("You remove the weeds") or every 15 minutes.
  Also cultivate empty trays now and then, or keep every tray planted.
- **Pests**: usually ignore. If "filled with tiny worms", one click with a pest spray.
- **Examine** each tray (or scan it) as you go: it tells you which needs what.

### Harvesting
- **Always harvest with the plant bag in your active hand**: click the ready tray and the produce goes straight
  into the bag (up to 100 items).
- A click with an **empty hand** also harvests, but drops everything **on the floor under you**. If that happens,
  click one of the items on the floor with the plant bag: it scoops up everything on that tile.
- After harvesting a single-harvest crop the tray is empty: replant it at once (weeds start otherwise).
- Never use the plant bag in hand (clicking it while it is your active hand): that **dumps the whole bag on the
  floor**. To look inside, Alt-click it, or click it with your other, empty hand.

### Seeds
- **Seed extractor**: click it with one produce in hand. You get 2-5 seed packs of that plant, **with the same
  stats as the produce** (improved yield and potency carry over). Left-click drops them on the extractor's tile;
  right-click stores them inside (its "Seed Extractor" window lists them; "take" hands you one). Clicking it with a
  plant bag moves only the bag's **seeds** into it, not the produce.
- **Portable seed extractor** (from your locker; it is a plant bag): Ctrl-click it and **every** produce inside
  becomes seeds (2 per produce). Never Ctrl-click it while it holds food meant for the Cook.
- Keep 1-2 of your best produce of each crop for seeds before you deliver; replant from those, not from the
  vendor: they are already improved.

### Biogenerator (Hydroponics north wall, and in the Garden)
1. Feed it food: click it with produce, or with the plant bag (it takes every food item in the bag, up to 20). Use
   rotten, surplus or weed produce, not the Cook's delivery.
2. In its "Biogenerator" window press **Generate** (action `activate`): the food becomes **biomass** (1 per unit
   of nutriment and vitamins in it; bigger, higher-potency produce gives more).
3. For liquids, first put a container in it (click it with a beaker, a bottle, a watering can or an empty
   jerrycan; Alt-click ejects it). Then `create` with `design_path` and `amount`. The design_path is
   `/datum/design/biogen/` + the short name in brackets below (e.g. `/datum/design/biogen/ez_nut`).

| Tab | Design (design_path) | Biomass per unit/item |
|---|---|---|
| Chemicals | E-Z Nutrient (ez_nut) | 0.1 per u (10u per biomass) |
| Chemicals | Left 4 Zed (l4z_nut) | 0.1 per u |
| Chemicals | Robust Harvest (rh_nut) | 0.2 per u |
| Chemicals | Enduro Grow (end_gro), Liquid Earthquake (liq_earth) | 0.3 per u |
| Chemicals | Chemo Cultivate (chemo_cult), Stabili Feed (stab_feed) | 0.4 per u |
| Chemicals | Weed Killer (weed_killer) 0.2, Pest Killer (pest_spray) 0.4, Organic Pest Killer (org_pest_spray) 0.6 | per u |
| Food | Synthetic Milk (milk), Synthetic Soy Milk (soymilk) | 0.4 per u |
| Food | Synthetic Cream, Ethanol, Black Pepper, Enzyme, Flour, Sugar (cream, ethanol, black_pepper, enzyme, flour, sugar) | 0.6 per u |
| Food | Monkey Cube (monkey_cube) 50, Seaweed Sheet (seaweed_sheet) 3 | per item |
| Materials | Sheet of Leather (leather) 30, Sheet of Cloth (cloth) 10, Sheet of Cardboard (cardboard) 5, Sheet of Paper (paper) 2, Sheet of Rolling Paper (rolling_paper) 1, Candle (candle) 3 | per item |

Items appear on the biogenerator's own tile: pick them up from beside it at once. Ask the Cook whether they want
milk, cream, flour, sugar or enzyme from it.

### Delivering
1. Put the bag's seeds into the seed extractor first (click it with the bag).
2. Click the **smartfridge** (Hydroponics north wall) with the plant bag: it loads all the produce. The Cook opens
   it from the Service Hallway side. It needs power ("magnetic door won't open without power").
3. Tell the Cook on Service: "Cook, 10 tomatoes and 8 wheat in the Hydroponics smartfridge."
4. Alternatives: hand it over in person, or put it on the **Kitchen Window** table in the Service Hallway and
   tell the Cook. Never leave produce on a floor.

**Rotting**: food lying on a floor (not on a table) starts to mould after 5 seconds and becomes mould in
about **10 minutes**. In a bag, in your hands, on a table or in the smartfridge it is safe. Flowers
(poppies, roses, sunflowers, lilies, harebells) never rot.

## Plant stats and how to improve them

| Stat | Meaning |
|---|---|
| Potency | Size and chemical content: a plant's chemicals = potency × rate (a poppy at potency 20 holds 4u libital, at 60 holds 12u). |
| Yield | Produce per harvest (max 10). Soil lovers (potatoes, carrots, beets) get only 70% of it in a hydroponics tray, and less potency: they do best in soil (the Garden, or a tray filled from a NutriMax **soil sack**). |
| Maturation | Cycles before production starts. |
| Production | Cycles between harvests (lower is faster). |
| Endurance | Maximum health. |
| Lifespan | Age at which the plant starts dying of old age. |
| Instability | Chance of mutations (see below). |

Simple improvements, in order:
1. **Keep 10-20u of nutrient in every tray**: Robust Harvest for yield (food crops), E-Z-Nutrient for potency
   (medicine). Both maxed in one or two generations.
2. **Replant from your best produce** through the seed extractor: the stats carry over.
3. **Plant one crop per row**: pollination averages neighbours' yield and potency, so one good plant lifts its row.
4. **Grafting** (optional): secateurs on a ready plant cut a **graft** (once per plant, costs 5 health). Click a
   growing plant with the graft: it gains the graft's trait (most plants' graft trait is **Perennial Growth**, e.g.
   from cabbage or grapes: graft it onto wheat or potatoes and they stay in the tray after each harvest), and its
   yield, lifespan and endurance rise toward the graft's where the graft's are higher. This version has no plant
   DNA manipulator.

## Mutations

Instability thresholds (per cycle unless noted):
- **20+**: stats drift randomly (strongly at 40+).
- **30+**: at harvest, each produce has instability ÷ 3 % chance to be a **mutant species** instead.
- **60+**: instability ÷ 2 % chance per cycle for the whole plant to become a mutant (not on autogrow).
- **80+**: random new traits or chemicals.
Raise it with Left 4 Zed; lower it with Robust Harvest. Corn (50) raises the instability of every plant that
touches it.

Common mutations (seed → mutants): **tomato → blue tomato (lube, slippery), blood tomato, killer tomato**;
cabbage → replica pod; corn → snapcorn, pepper-corn; wheat → oat, meatwheat; potato → sweet potato; carrot →
parsnip, Cahn'root; onion → red onion; chili → chilly pepper, ghost chili; soybean → koibean (poisonous),
butterbean; pumpkin → blumpkin (toxic); watermelon → holy melon, barrel melon; apple → golden apple; grape → green
grape (aiuri); berry → glow-berry (uranium), poison-berry → death berry; banana → mimana, bluespace banana;
sugarcane → bamboo, saltcane; poppy → geranium, lily → Spaceman's Trumpet; **ambrosia vulgaris → ambrosia deus
(omnizine, synaptizine)** → ambrosia gaia; sunflower → moonflower, novaflower (sets people on fire); tea aspera →
tea astra (synaptizine); coffee arabica → coffee robusta; tobacco → space tobacco; plump helmet → walking
mushroom; peas → laughin' peas → world peas.

**Plants to avoid or contain**
- **Killer tomatoes**: a killer tomato comes alive as a hostile monster when **used in hand** ("shaken"), and with
  a 25% chance when handled without botanist's gloves. Keep tomatoes' instability under 30 (Robust Harvest, not
  next to corn), and if one appears, put it straight into the biogenerator.
- **Kudzu** (spreading vines): comes from mutated weeds (mutagen or radiation in a weedy tray). Never plant it.
- **Nettles and death nettles** (burn and acid; contraband or weed invasion), **fly amanitas and destroying
  angels** (deadly amatoxin), **poison and death berries**, **koibeans**, **blumpkins**, **glow-berries**:
  never deliver these as food. Bin or biogenerate them.
- **Walking mushrooms**, **bluespace tomatoes/bananas** (teleport), **novaflowers**, **strange seeds**, and the
  MegaSeed's hidden contraband: not this shift.

## Growing plan

Times: 1 cycle = 20 s. "First" = maturation + production; "again" = production + 1 (perennials only).

**For the Cook** (ask what they want first; common kitchen crops):

| Crop (seed pack) | First harvest | Again | Base yield | Notes |
|---|---|---|---|---|
| Wheat | 2 min 20 s | – | 4 | grinds into flour |
| Rice | 2 min 20 s | – | 4 | |
| Onion | 2 min 20 s | – | 6 | |
| Cabbage | 2 min 40 s | 2 min | 4 | lifespan 50: many harvests |
| Soybean | 2 min 40 s | 1 min 40 s | 3 | |
| Green bean | 2 min 20 s | 1 min 20 s | 3 | never mutates; contains multiver |
| Sugarcane | 3 min | 2 min 20 s | 4 | sugar; lifespan 60 |
| Potato | 3 min 40 s | – | 4 | soil lover |
| Carrot | 3 min 40 s | – | 5 | soil lover |
| Cucumber | 3 min 40 s | 40 s | 5 | |
| Chili | 3 min 20 s | 2 min | 4 | instability 30; lifespan 20 |
| Garlic | 4 min | – | 6 | |
| Tomato | 4 min 40 s | 2 min 20 s | 3 | instability 25 (killer tomato risk: Robust Harvest) |
| Corn | 4 min 40 s | – | 3 | instability 50: its own row, or the Garden |
| Pumpkin, watermelon, apple, eggplant, herbs | 4 min | 2 min 20 s | 2-5 | lifespan 50+ (eggplant and herbs 25) |
| Grape | 2 min 40 s | 2 min | 4 | for a bartender: wine |
| Chanterelle mushrooms | 2 min 40 s | – | 5 | mushrooms tolerate dim light |

A starting layout for the 16 trays, rows west to east: tomatoes (3), wheat (4), cabbage (3), onion/carrot/potato
(3), medicine (3); corn and potatoes do better in the Garden's soil. Replant single-harvest crops as soon as they're picked.
A bartender, if one is on shift, may want grapes, berries, citrus (lemon, lime, orange), apples, potatoes, wheat,
rice or corn: a fermenting barrel turns them into wine, gin, triple sec, cider, vodka, beer, sake and whiskey.

**For the Chemist and medbay** (chemical content per produce = potency × rate; feed E-Z-Nutrient for potency):

| Plant | First / again | Contains | Use |
|---|---|---|---|
| **Poppy** | 4 min 40 s / – (yield 6) | **libital** (brute medicine, 20% of potency) | eat or grind; libital is an ingredient of **synthflesh** (blood + carbon + libital); endurance only 10: never let it dry |
| **Aloe** | 2 min 40 s / – (yield 6) | vitamins | microwaved or baked it becomes **aloe cream** (heals brute and burn) |
| **Ambrosia vulgaris** | 4 min / 2 min 20 s | aiuri (burn medicine), libital, space drugs, a little toxin | instability 30: may mutate into **ambrosia deus** (omnizine, synaptizine) |
| **Green bean** | 2 min 20 s / 1 min 20 s | multiver (toxin purger) | |
| Lily, geranium (poppy mutants) | as poppy | libital | |
| Tea astra, coffee robusta, space tobacco (mutants) | – | synaptizine, ephedrine, salbutamol | |

**Flowers for the crew**: 6 poppies (lilies and geraniums count), 6 roses or 6 sunflowers make a bouquet in the
crafting menu (Entertainment category); 2 lilies + 2 sunflowers + 2 geraniums make a mixed bouquet. Flowers never
rot. Roses have thorns: keep your gloves on.

**A prize plant**: a yield-10, potency-100 harvest is reachable with 20u of nutrients kept in the tray for the
whole growth, and a second generation from its seeds.

## Dangers and common mistakes

- **Plants starving** (yesterday): 10u of nutrients at round start lasts 3 minutes 20 seconds. Fill every planted
  tray to 20u at once and top up every 5 minutes.
- **Trusting autogrow** (yesterday): it never adds nutrients.
- **Produce on floors** (yesterday): harvesting with an empty hand, or using the bag in hand, puts everything on
  the floor, where it moulds in 10 minutes and draws ants.
- **Using the plant bag in hand** dumps it (yesterday). Alt-click to open it.
- **Spraying Plant-B-Gone on a tray** kills the plant.
- **Pouring a nutrient can onto the watering can** (clicking one container with another) mixes nutrient into your
  water. Keep track of what's in your active hand before every click.
- **Right-click on a tray with an empty hand** asks "Empty Tray Nutrients?": answer No.
- **Power cuts** (yesterday: about 10 minutes): vendors, the smartfridge, the biogenerator and autogrow stop, and
  plants lose health in the dark. Trays themselves need no power.
- **Weeds in empty trays** turn into weed plants (some poisonous). Keep trays planted or cultivated.
- **Corn next to tomatoes** pushes the tomatoes toward killer tomatoes.
- Never eat or deliver anything you can't name; scan unknown produce with the analyzer first.

## Emergencies

- **Power failure** (lights out, vendors dark): turn autogrow off, keep water and nutrients topped up so the plants
  have health to spare, don't plant new seeds until the lights are back, and tell the engineers (Service or Common
  radio) that the Hydroponics APC is down. Restock nutrients from the biogenerator once power returns.
- **Fire**: fire extinguisher cabinets are on the room's walls (and in the backroom and the Garden). If the air
  alarm reports danger or there is smoke, leave and close the doors behind you.
- **Breach / bad air**: leave, close the doors, report where. Plants can wait; you can't.
- **Kudzu (space vines)**: if vines appear anywhere, spray them with Plant-B-Gone (it kills vines) and cut them
  with the hatchet (sharp tools deal four times their damage to vines). Report the spread on Common.
- **Mass casualties**: carry poppies, aloe cream and green beans to medbay, help move the injured.
- **Attacker in or near Hydroponics**: see below.
- **Evacuation**: make a last delivery, pack fruit, go to the Departure Lounge when the shuttle docks.

## Defending yourself and Hydroponics

How readily you fight is set by your personal file; shared combat basics (combat mode, shoving, grabs, resisting)
are in crew-basics. What botany gives you:
- **Doors**: both Hydroponics doors need Hydroponics access, so most crew can't follow you in. The **Service
  Shutter Control** button (north wall) closes the shutters over the smartfridge and the Hydroponics Window.
- **Hatchet**: the best weapon in reach (force 12, sharp, can cause bleeding; thrown it hits for 15 and may stick
  in). One in each botanist's locker, three in the Garden.
- **Cultivator** and **secateurs**: weak (force 5).
- **Slipping, without hurting anyone**: banana peels (eat a banana) and blue tomatoes are slippery; a peel knocks
  down whoever steps on it for about potency × 0.16 seconds (potency 50: 8 seconds). Drop one in a doorway behind
  you when you run.
- **Nettles** are a weak weapon (force 5 + potency ÷ 5, wear down with each hit) that burn bare hands; your gloves
  protect you. Not worth growing for this.
- Sprays (Plant-B-Gone, pest spray) are poisons: don't spray people.
Raise the alarm first: who, where, what weapon, on Common; ask the AI to bolt the doors on them.

## Working with the crew

| Crew | You give | You need |
|---|---|---|
| Cook | produce, often; milk, cream, flour, sugar, enzyme from the biogenerator | their wish list; a meal |
| Bartender (if on shift) | grapes, berries, citrus, fermentables | their wish list |
| Chemist | poppies (libital, synthflesh), ambrosia, green beans, aloe | their wish list; mutagen only for a planned experiment, never in weedy trays |
| Medical Doctors | aloe cream, poppies | healing |
| Head of Personnel | a working Hydroponics; reports | access fixes; help if Service is short-handed |
| Quartermaster | produce for exports or bounties | Seeds Crate, Exotic Seeds Crate, Hydroponics Crate or NT-Ag Potting Soil Crate when the vendors run dry |
| Scientist | produce for experiments | upgraded parts for the trays (better matter bins hold more water and nutrients; better servos slow water and nutrient use) |
| Station Engineers | a report when the Hydroponics APC is down | power |
| Janitor | a heads-up about spills or mould | clean floors |
| AI | – | doors, and locking out an attacker |

Other botanists or a bartender may join at any time: share the trays, say on Service who grows what.

## Through the client

- **Vendors**: click the MegaSeed Servitor or NutriMax; its window lists products with prices and refs;
  `tgui_act` `vend` with the product's `ref`. Have a hand free, or the item lands on the floor.
- **Using an item on a tray**: hold it in the **active** hand and `click` the tray's object id (`search` "tray"
  finds them; names show the plant). The chat answer tells you what happened ("You plant…", "You remove the
  weeds", "[tray] is full.").
- **Clicking what your active hand holds uses it in hand**: the watering can and nutrient cans switch transfer
  amount (examine shows the current one), the plant bag **dumps**, a killer tomato **wakes up**. Swap hands (key
  X) before clicking the bag; Alt-click the bag (`click` with `alt: true`) to open it.
- **Ctrl-click** a tray (`click` with `ctrl: true`) toggles autogrow. Avoid `right: true` on trays with an empty
  hand (the empty-nutrients prompt; answer "No").
- **Picking things up from tables and tanks**: click the item's own object id, not the tile (a tile click hits the
  tank or table under it). `command "Pick-up <exact name>"` also works next to it; names with ™ must be exact
  ("E-Z-Nutrient™ can").
- **Reading trays**: `examine` the tray for water/nutrient numbers; the plant analyzer's window (`tgui_window`)
  gives everything. No chat line announces "ready to harvest": check by examine on your loop.
- **Machines' windows**: Biogenerator (`activate`, `create` {design_path, amount}, `eject`, `select` {category});
  Seed Extractor (`take` / `scrap` {item: the seed's key}); smartfridge "SmartVend" (`Release` {path, amount}).
- **Waiting**: `wait` in chunks of a minute or two between loops, and keep an eye on the clock (a cycle is 20 s).
- If `walk_to` says a Hydroponics door is blocked although you have access, step into it with `move`.
- Radio: Service is `:v` (the say tool's radio option "service"), Common `;`.

## Checklist

**Shift start**
- [ ] Locker: cultivator, hatchet, secateurs, portable seed extractor. Plant bag in hand.
- [ ] NutriMax: E-Z-Nutrient™ can + Robust Harvest™ can; can set to 30u. Watering can set to 100u, filled.
- [ ] Ask the Cook and the Chemist what they want (Service radio).
- [ ] Seeds bought and planted; every planted tray at 20/20 nutrients and 100/100 water.
- [ ] One line on Common: Hydroponics is open.

**Every 5 minutes**
- [ ] Each tray: examine → nutrient click, water click, cultivator if weedy.
- [ ] Ready trays: harvest with the plant bag in hand; replant empty trays.
- [ ] Keep 1-2 best produce per crop for the seed extractor.

**Every 15 minutes**
- [ ] Delivery: seeds into the extractor, produce into the smartfridge, tell the Cook on Service.
- [ ] Check the Chemist's requests; surplus produce into the biogenerator for nutrients.
- [ ] No produce on any floor.

**Last half hour**
- [ ] Final delivery, a bouquet or fruit for the crew, then the Departure Lounge.

## Sources

- Code (tgstation 54c22023): `code/modules/jobs/job_types/botanist.dm`, `code/datums/id_trim/jobs.dm`,
  `code/modules/hydroponics/` (hydroponics.dm, hydroponics_chemreact.dm, seeds.dm, seed_extractor.dm,
  biogenerator.dm, soil.dm, hydroponics_items.dm, plant_genes.dm, unique_plant_genes.dm, grown/*.dm),
  `code/__DEFINES/botany.dm`, `code/modules/reagents/chemistry/reagents/other_reagents.dm` (plant nutrients) and
  the other reagents' `on_hydroponics_apply`, `code/modules/research/designs/biogenerator_designs.dm`,
  `code/modules/vending/megaseed.dm`, `nutrimax.dm`, `code/modules/food_and_drinks/machinery/smartfridge.dm`,
  `code/datums/components/food/decomposition.dm`, `germ_sensitive.dm`, `code/datums/storage/storage.dm`,
  `code/game/objects/items/devices/scanners/plant_analyzer.dm`, `code/datums/components/crafting/entertainment.dm`.
- Map: `_maps/map_files/MetaStation/MetaStation.dmm` (Hydroponics, Garden, Service Hallway, Aft Starboard
  Maintenance).
- tgui: `tgui/packages/tgui/interfaces/Biogenerator.tsx`, `SeedExtractor.tsx`, `SmartVend.tsx`, `PlantAnalyzer/`.
- Wiki (CC BY-SA 3.0): Botanist, Guide_to_hydroponics (Internet Archive, Feb 2026); the code wins where they
  differ.
- Yesterday's round: `runs/12-botanist/report.md`, `runs/12-cook/report.md`.
