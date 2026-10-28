# Cook (Chef) guide: MetaStation

## The job in one paragraph
You keep the crew fed. Hungry crew are miserable and heal worse. Success means a steady supply of real, safe dishes: on the Kitchen counter for anyone passing, handed to people, and carried to crew who can't leave their posts (engineers at the engine, doctors in Medbay, officers in the Brig). Announce a short menu on the radio and take orders. The botanist is your main supplier, so ask early. Never serve anything burned, raw or dirty.

## Starting kit and access
- **Worn:** service button-down and slacks, black shoes, Italian fake moustache, service radio headset, cook's PDA on the belt.
  - The first cook to join gets the **chef's apron** (an apron-jacket) and chef's hat, and the ID title "Chef". Any later cook gets the cook's apron, a white cap and the title "Cook". Access is the same.
  - The chef's apron's suit-storage slot holds a **kitchen knife, a rolling pin or a serving tray**. Shift+Q equips the held item to suit storage, or draws it.
- **Backpack:** survival box and a **whetstone** (one use: +4 force on a knife).
- **Right pocket:** a **cooking voucher**, worth 10 free items at the produce orders console (see Ingredients).
- **Skillchip (active from spawn):** "B0RK-X3", which teaches **Close Quarters Cooking**. See Defending yourself.
- **Liver trait:** garlic juice slowly heals you (brute and burn). Eating a garlic works.
- **Radio:** `;` is Common. **`:v` is Service**: the Head of Personnel, botanist, janitor, bartender and other service staff.
- **Access:** Kitchen, Service, Morgue, Mineral Storeroom, plus **Bar and Hydroponics** when 20 or fewer players readied up at round start (expected this round; if those doors refuse you, it didn't apply). The Kitchen's fridges, cabinet, doors and shutter buttons need Kitchen access.
- Your boss is the **Head of Personnel** (head of Service).

## Where things are (MetaStation)
`walk_to {area: "Kitchen"}` works from arrivals. The Kitchen sits between the **Bar** (west), the **Bar Lounge** (north: the seating area, your dining room), the **Theater** (east), and the **Service Hallway** and **Hydroponics** (south). MetaStation's "Cafeteria" area is a small coffee shop elsewhere, not your dining room.

**Kitchen** (area "Kitchen"):
- **Doors:**
  - "Kitchen" airlock in the north-west corner, to the Bar Lounge. Kitchen or Bar access.
  - "Bar" glass airlock on the west wall, to the Bar. Bar access.
  - "Kitchen" airlock in the south wall, to the Service Hallway. Kitchen access.
  - "Freezer" airlock in the south-east, to the Kitchen Cold Room.
- **North wall = the serving counter:** six reinforced tables (salt, pepper, a cream pie, a desk bell) and the **food smartfridge** at the west end, all under the **Kitchen Counter Shutters** (open at round start). The Bar Lounge side can reach the counter and the smartfridge.
- **East wall, by the counter:** the **food processor** on a table, with the **"Kitchen Counter Shutters Control"** button.
- **Middle row:** **two ranges** (oven + stovetop; each has an oven tray inside and a soup pot on top), **two griddles** east of them, the **kitchen sink** at the west end.
- **East wall:** **refrigerator** (5 space milk, 5 soy milk, 2 egg boxes of 12), **kitchen cabinet** (3 flour sacks, rice sack, sugar sack), fire extinguisher cabinet, disposal bin.
- **West wall:** **two microwave ovens**, the Kitchen APC; further south the **Plasteel Chef's Dinnerware Vendor**, the **ChefDrobe** and the **"Service Shutter Control"** button.
- **Tables:** a serving tray, recipe book, **rolling pin**, one **dough**, a large beaker; on the south wall the **all-in-one grinder** with **universal enzyme**, two beakers, a **rag**, the CondiMaster Neo and the Kitchen Requests Console.
- **South-east:** **deep fryer**, dehydrator, second sink.
- **No kitchen knife spawns.** Vend one from the Dinnerware Vendor (free for service staff); it also has serving trays, soup pots, ladles, plates, bowls, glasses, forks and spoons.

**Kitchen Cold Room** (through the Freezer door): **meat fridge** (4 monkey meat), cooking oil tank, food cart, ice cream vat, gibber, meat spikes, a sink, and **Pete the goat** (harmless; fights back if hit). The east "Kitchen Delivery" windoor leads to the nook where Kitchen crates and mail arrive. The air is −14 °C: grab things and leave.

**Hand-off with Hydroponics** (the **Service Hallway**, just south of the Kitchen):
- The **Kitchen Window**, in the Kitchen's south wall next to the south door: a table with a windoor (Kitchen access) and the "Service Shutter". Players in the hallway leave or take things there; you reach it from inside.
- A few tiles west, in the wall to Hydroponics: the **Hydroponics smartfridge** and the **Hydroponics Window** table. The botanist stocks them from inside; you take from the hallway side.

**Produce orders console:** **Greater Starboard Maintenance**, through the "Service Hall" door at the Service Hallway's east end, in a nook with a cigarette vendor.

## How the machines work in this version
Hold the ingredient in your active hand and click the machine, unless a line below says otherwise.

| Machine | Use |
|---|---|
| **Griddle** (8 items) | Click it with a grillable item to place it (not in combat mode). An **empty-hand click turns it on or off**. Cooked items stay on the griddle and keep cooking, and **a finished item burns into a "burned mess" 20-30 s later**. Anything without a griddle recipe burns in 20-30 s; **a whole egg burns**. **Crack an egg onto it: right-click the griddle with the egg in hand** to make a raw egg, then a fried egg. To take food off, click the item on the griddle with an empty hand. A serving tray works too: left-click the griddle to unload the tray's food onto it, **right-click to scoop everything back onto the tray**. |
| **Range: oven** (tray holds 6) | An **empty-hand click opens or closes the door** ("You open the range." / "You close the range."). Baking runs only while the door is closed, and progress is kept while it's open. **Clicking the range with food in hand does nothing.** To load it: **open the door, then click the "oven tray" inside with the food**. Or: **left-click the open range while holding a serving tray** with the food on it ("You insert N items into oven tray"). Then close the door. Done: "You smell something great coming from the range." **Open it at once**: the result burns 25-40 s later, and anything without a baking recipe burns too ("burnt smell"). To unload, open the door and click the items, or **right-click the open range with a serving tray**. |
| **Range: stovetop** | **Right-click the range with an empty hand** to switch the burners on or off ("burners on"). They heat the soup pot on top; see Soups. |
| **Microwave oven** (10 items) | Click it with an item (normal size or smaller) to add it ("You add X to the microwave oven"). Right-click it with a serving tray to load the tray's food. **Right-click it with an empty hand to start**, or left-click for a radial menu: eject / cook / charge. One cycle takes about 10 s, then it ejects onto its table. **Only a few things microwave properly:** egg → boiled egg, corn → popcorn, raw spaghetti → boiled spaghetti, uncooked rice → boiled rice, onion slice → onion rings, warm donk pockets. **Everything else becomes a burned mess, dough included.** Every item cooked adds dirt, and each cycle's chance to "get covered in muck" is 5% per point of dirt. A mucked microwave refuses food ("it's too dirty!"). **Scrub it by clicking it with the rag every 3-4 items** (3 s). If power dies mid-cycle it breaks: fix it with wirecutters, then a welding tool. |
| **Food processor** (on a table) | Click it with each item ("You put X into food processor"), or click it with a serving tray to load everything usable. Then **click it with an empty hand** to run it (4 s per item). Output drops onto its table. Recipes: meat slab → 3 raw meatballs; raw cutlet → raw bacon; potato wedges → fries; potato → tater tots; carrot → carrot fries; dough slice → raw spaghetti; corn → tortilla; tortilla → corn chips; soybeans → soy dope. Items it can't use: "That probably won't blend!" |
| **Deep fryer** | Click it with one item to fry it (not in combat mode). **An empty-hand click takes it out.** Under 15 s gives "lightly-fried"; 15-50 s "fried"; at 50 s it "dings" for **deep-fried** (best). After 85 s the item is ruined. Frying adds the fried food type, which most crew like, and makes it junk food. It starts with 25u oil; refill from the cooking oil tank in the Cold Room. |
| **All-in-one grinder** | Insert a beaker first (click the grinder with it). Then click the grinder with produce, and **empty-hand click** for the radial menu: grind / juice / mix / eject. Right-click with an empty hand takes the beaker back. Use it to turn wheat into flour, or for juices and sauces. |
| **Smartfridges** | Food fridge (counter): click it with food or a filled bowl, or with a serving tray to load everything. Opening it shows a tgui list; take things out with `Release {path, amount}`. The Hydroponics fridge takes produce and seeds. Neither opens without power. |
| **Sinks** | Click with a container to add its transfer amount of water. Right-click with a container to empty it. Click with any other item (not in combat mode) to wash it, which takes 4 s and removes germs. |
| **Gibber** (Cold Room) | Turns dead animals into meat. **Never a crew member's body**: bodies go to Medbay or the Morgue (they may be revived). There's no charcoal grill on MetaStation. |

**The serving tray is your universal loader** (8 items).
- Load it: click a food item with the tray in hand. It scoops everything it can hold on that tile.
- It unloads into the oven (left-click the open range), the griddle (left-click), the microwave (right-click), the processor and the smartfridges (left-click).
- **Never click the tray while it's in your own hand**: that empties it onto the floor.

## Basic preparation (no machine)
Do all of this on a **table**: processing needs a table or a tray under the item. Hold the tool and click the food (3 s each).
- **Kitchen knife on:** meat slab → 3 raw cutlets; flat dough → 3 dough slices; bread → 5 bread slices; cheese wheel → 5 cheese wedges; potato → potato wedges; pizza or cake → slices.
- **Rolling pin on:** dough → flat dough; raw meatball → raw patty; cake batter → pie dough.
- **Reagent mixes** (instant, in an open beaker):
  - Put the **beaker on a table first**: the food forms under the beaker, so a held beaker drops it on the floor.
  - Pour by clicking the beaker with the sack or carton. Click a container in hand to raise its transfer amount, right-click in hand to lower it.
  - Click the sink with the beaker for water (10u per click with the large beaker). Click the beaker with an egg to crack it in (2u yolk + 4u white).
  - Flour sack 30u, milk carton 50u, rice sack 30u.

| Mix | Makes |
|---|---|
| 10u water + 15u flour | 1 **dough** (one sack makes 2 doughs) |
| 40u milk + 5u universal enzyme | 1 **cheese wheel**. The enzyme isn't used up: add 40u more milk for the next wheel. |
| 3 eggs + 15u flour + 5u sugar | **cake batter** |
| 3 eggs + 10u milk + 5u flour | 15u **pancake batter** (a liquid) |
| 10u rice + 10u water | 1 **uncooked rice** |
| 10u soy milk + 5u enzyme | tofu |

**Germs ("five-second rule"):**
- Any food (produce included) left on a **floor** tile for 5 s becomes "dirty and not safe to consume" and can give a weak disease.
- **Food on tables, racks, trays, griddles, the fryer, the processor or in a smartfridge is safe.**
- Wash dirty food at a sink (or deep-fry it). Never serve anything that examines as dirty.
- Food on the floor also rots (mold after 10 min, raw food 5 min) and some draws ants.

## The crafting menu
Most dishes are assembled in the **crafting menu**, not in a machine.
1. Click the **"crafting menu"** button on your HUD (bottom right; `search {query: "craft", kind: "screen"}` finds it).
2. The menu opens in crafting mode. Send **`toggle_mode`** once to switch to cooking (about 900 food recipes); it stays in cooking mode.
3. A recipe is **"craftable now"** when every ingredient, reagent, tool and machine it needs is **within reach**: on your tile, the 8 tiles around you (tables count), in your hands or in your worn items. Reagents count when they sit in an open container in reach (a salt shaker for "salt 1u", a milk carton for "milk 5u").
4. Make it with `make {recipe: <ref>}`. It takes about 3 s, during which the menu shows busy. **Don't send another make until the first is done**; a second one fails with "Construction failed".
5. **The result goes into your free hand.** With both hands full it drops on the floor (and gets germs in 5 s). Keep a hand empty.
6. Crafted and cooked food is "handmade", which gives the eater a buff (see What food does).

## Ingredients and where they come from
- **Round start, in the Kitchen:** 3 flour sacks (6 doughs), rice, sugar, 5 milk and 5 soy milk cartons, 24 eggs, 4 monkey meat, 1 dough, enzyme, salt and pepper.
- **Botanist (Hydroponics):** tomatoes, cabbage, potatoes, corn, carrots, onions, garlic, chili, eggplant, apples, bananas, oranges, grapes, watermelon, berries, wheat (grind it into flour), mushrooms. Ask early, by name and number ("4 tomatoes, 2 cabbages, 3 potatoes"). Collect from the Hydroponics smartfridge or the windows in the Service Hallway.
- **Cargo (the Quartermaster orders, the crate comes on the shuttle):**
  - "Food Crate", 400 cr: flour, rice, milk, soy milk, salt, pepper, 12 eggs, enzyme, sugar, monkey meat, 3 bananas;
  - "Vegetables Crate", 360 cr: chili, corn, tomato, potato, carrot, chanterelle, onion, pumpkin, cucumber;
  - "Excellent Meat Crate", 800 cr: random exotic meats.
  - A crate's contents fall on the floor when it opens: scoop them with the serving tray straight away.
- **Produce orders console** (Greater Starboard Maintenance):
  1. **Click it with the cooking voucher** ("redeemed voucher"): your next 10 items are free.
  2. Open it (tgui "ProduceConsole"). There are three categories: Veggies, Milk & Eggs (including egg cartons, chicken breast and fish fillets), and Reagents (flour, sugar and rice sacks, enzyme, condiments, sauces).
  3. Fill the cart with `add_one {target: <ref>}` or `cart_set {target, amt}`.
  4. **`express`** drops a pod right on your tile (no damage). It costs 2x, but **0 for the free voucher items**; scoop the goods with the tray at once.
  5. **`purchase`** costs 0.65x from your own account and arrives on the next cargo shuttle. **It does nothing if the order totals under 200 cr**, so a voucher-only order needs `express`.
  - The console has a 60 s cooldown (120 s after an express).

## Verified recipe book
Times are randomised within a range in code, so use `examine` ("probably needs to be cooked a bit longer!" / "seems to be almost finished") and wait for the result message. "Craft" means the crafting menu. Complexity (cx) is the strength of the handmade buff.

**Building blocks**
| Item | How |
|---|---|
| Bread | Dough baked in the oven, 30-45 s. Slice with the knife → 5 bread slices. |
| Bun (×3) | Dough → rolling pin → flat dough → knife → 3 dough slices → oven 20-25 s → 3 buns. |
| Patty (×3) | Meat slab → processor → 3 raw meatballs → rolling pin each → raw patty → griddle 30-40 s. |
| Meatball | Raw meatball on the griddle, 30-40 s. |
| Steak | Meat slab on the griddle, **30-90 s**. Burns 20-30 s after it's done. |
| Cutlet | Slab → knife → 3 raw cutlets → griddle 35-50 s each. |
| Bacon | Raw cutlet → processor → raw bacon → griddle 25-45 s. |
| Cheese wedge (×5) | Cheese wheel (mix above) → knife. |
| Fried egg | Right-click the griddle holding the egg → 20-35 s. |
| Boiled egg | Egg in the microwave, or 15-20 s in the oven. |
| Boiled spaghetti | Dough slice → processor → raw spaghetti → microwave, or oven 15-20 s. |
| Fries | Potato → knife (on a table) → potato wedges → processor. |
| Plain pie | Cake batter → rolling pin → pie dough → oven 30-45 s. |

**Dishes**
| Dish (menu name) | Ingredients (craft unless noted) | cx |
|---|---|---|
| Plain Burger | bun + patty | 2 |
| Cheese Burger | bun + patty + cheese wedge | 3 |
| Bacon Burger | bun + 3 bacon | 3 |
| Sandwich | 2 bread slices + cabbage + steak + cheese wedge | 3 |
| Cheese sandwich | 2 bread slices + 2 cheese wedges. Griddle it 30-60 s → grilled cheese sandwich (cx 3). | 2 |
| BLT | 2 bread slices + 2 bacon + cabbage + tomato | 3 |
| Griddle toast | bread slice on the griddle, 15-25 s | 2 |
| Omelette du fromage | 2 eggs + 2 cheese wedges (no machine or power needed) | 2 |
| Eggs benedict | fried egg + steak + bread slice | 3 |
| Meat Clown | steak + banana | 2 |
| Tomato pasta | boiled spaghetti + 2 tomatoes | 2 |
| Spaghetti meatball | boiled spaghetti + 2 meatballs | 2 |
| Lasagna | 2 cutlets + tomato + 2 cheese wedges + raw spaghetti | 3 |
| Pizza margherita | craft "raw pizza margherita" (flat dough + 4 cheese wedges + tomato), bake 70-80 s, knife → 6 slices | 3 |
| Meat pizza | craft "raw meatpizza" (flat dough + 4 raw cutlets + cheese wedge + tomato), bake 70-80 s | 3 |
| Cheesy fries | fries + cheese wedge | 2 |
| Baked potato | potato in the oven, 15-25 s | 1 |
| Popcorn | corn in the microwave | – |
| Meat pie | plain pie + steak + 1u salt + 1u pepper (shakers in reach) | 3 |
| Apple / Cherry pie | plain pie + apple / cherries | – |
| Banana cream pie | plain pie + banana + 5u milk | – |
| Cake | cake batter in the oven, 70-90 s; slice with the knife | – |
| Fruit salad | bowl + apple + grapes + orange + 2 watermelon slices | 3 |
| Pancakes | Pancake batter **splashed** on the griddle (combat mode on, right-click the griddle with the beaker; 5u per pancake), then 30-40 s. | 2 |

**A good production line for one cook from round-start stock:**
- 6 doughs → 2 breads (10 slices) + 4 doughs as 12 buns.
- 4 monkey meat → 12 patties.
- 5 milk cartons → 6 cheese wheels (30 wedges).
- Result: about 12 cheeseburgers, plus omelettes and cheese sandwiches from the eggs, bread and spare cheese.
- Add steaks, BLTs, pizza and pasta once produce arrives.

**Soups** (advanced). They are cooked in the soup pot on a range: click the pot by id.
1. Fill a large beaker with 50u water and pour it into the pot.
2. Add ingredients. Click the pot with each one, or click the **closed** range holding a serving tray with them.
3. Right-click the range to turn the burners on and wait for "You smell something good coming from the steaming pot of soup."
4. **Turn the burners off at once**: it burns above 540 K.
5. Pick the pot up by clicking it with an empty hand, and pour 50u into each bowl from the Dinnerware Vendor.

| Soup | Pot contents |
|---|---|
| Tomato soup | 50u water + 5u cream + 2 tomatoes (cream comes from the order console) |
| Vegetable soup | 50u water + carrot + corn + eggplant + potato |
| Hot chili | 50u water + 2 cutlets + chili + tomato |

## What food does
- **Hunger:** nutrition falls about 3 points a minute from a start of 250-400. Below 250 crew are hungry (bad mood), below 200 "sluggish", below 150 starving; above 450 well fed (good mood). Most crew get hungry within the first hour.
- **Nutriment heals a little** brute and burn damage while it digests. It is never a substitute for Medbay.
- **Quality:**
  - Most crew like fried and junk food and dislike raw, gross or gory food. Lizardpeople like meat and dislike grain and dairy.
  - Good dishes give a mood boost ("That's a … meal"). A **burned mess** holds 30u of bad food toxin: bin it.
- **Handmade buff:** an unbitten crafted or cooked dish gives "Hand-crafted meal" for up to 5 minutes (shorter with low-purity ingredients like monkey meat): +4% move speed and +6% action speed per complexity point, so a cheeseburger (cx 3) gives +12% and +18%.
- **Eating:** click yourself with the food. Clicking someone else force-feeds them (rude); offer food instead (ctrl-shift-click them) or use the counter.

## Shift start
1. Load the map and `walk_to {area: "Kitchen"}`.
2. Vend a **kitchen knife** (and a second serving tray) from the Dinnerware Vendor. Put the knife in your apron's suit storage.
3. Open the refrigerator, the kitchen cabinet and the meat fridge; move what you need onto tables.
4. Radio (Common): "Kitchen open. Botanist: tomatoes, cabbage, potatoes, corn please." Coordinate service staff on `:v`.
5. Start the long jobs first:
   - two doughs in each oven (bread, or flat-dough → slices → buns);
   - meat in the processor → meatballs → patties (or a slab or two straight onto a griddle as steaks);
   - cheese wheels in the large beaker.
6. Redeem the voucher at the produce orders console when you have a minute: eggs, cream, tomatoes, cabbage.
7. Announce a short menu when the first batch is ready.

## Ongoing loop
- Keep **6-10 finished dishes** on the counter or in the counter smartfridge.
- Take things off the griddle and out of the oven the moment they finish. Scrub the microwave every few items.
- Every 10-15 minutes: a short radio update (what's ready, what you're out of). Name orders ("Cheeseburger for Atmos, at the counter") and confirm when ready.
- Deliver to posts that can't leave; collect produce; restock flour, milk and meat before you run out.

## Serving and delivery
- **Counter:** click a counter table with the dish; the Bar Lounge side takes it. The **counter smartfridge** keeps food safe and lists it for anyone there.
- **Deliveries:** load a serving tray (8 dishes) and walk: **Engineering** / **Supermatter Engine Room**, **Atmospherics**, **Medbay Central**, **Brig** / **Security Office**, **Cargo Bay**, **Research Division**, **Bridge**. Announce it first ("Food run to Engineering in 2 min"). Leave food on a table, never the floor.
- **Restaurant portal** (Bar Lounge, north wall; optional): clicking it opens the restaurant for robot customers, who order dishes and pay. Crew come first.

## Dangers and common mistakes (several happened last shift)
- **Whole eggs on the griddle burn**: right-click the griddle with the egg to crack it.
- **Dough in the microwave burns**: bake it in the open oven (tray method or click the oven tray). Clicking the range with food does nothing.
- **Finished food left in place burns** 20-40 s later; non-food on the griddle or in the oven catches fire.
- **Floor food goes dirty in 5 s**: crate contents, express pods, mixes in a held beaker, crafts made with full hands.
- **Pun Pun** (the Bar's monkey) hands people items, so your next click may use the wrong thing. Check `inventory`; drop strays. He fights back if hurt.
- **In combat mode a held knife hits whoever you click.** Don't open Kitchen doors for strangers.

## Emergencies
- **Power failure** (machines dark; status shows the Kitchen APC off):
  - Report it on Common ("Kitchen APC down").
  - Keep cooking what needs no power: omelettes, cheese sandwiches, sandwiches from bread you already baked, meat clowns from ready steaks, fruit salad, and dough and cheese mixes in beakers.
  - The smartfridge won't open until power returns.
- **Fire:** turn off the griddles and burners and grab an extinguisher (cabinets on the east wall by the griddles and on the wall by the dehydrator). If it spreads, leave and call Atmospherics.
- **Breach or bad air:** leave through a door away from it, report it, and never open a door that leads to space.
- **Mass casualties:** keep cooking; send a tray to Medbay Central; carry the wounded only if Medbay asks.
- **Radio silent** (no line of yours comes back): telecomms or power is down; walk and talk.
- **Attacker in or near the Kitchen:** close the shutters, call Security on Common with the attacker's name and location, and use the next section.
- **Evacuation:** when the shuttle is called, fill one or two serving trays with food and go to the **Departure Lounge**.

## Defending yourself and the kitchen
Your personal file sets how readily you fight. These are your means. Combat basics (combat mode, shoving, grabs, resisting) are in crew-basics.

**Close Quarters Cooking (CQC)** is a full martial art from your skillchip.
- **Where it works:** only while **you** stand in the **Kitchen, Kitchen Cold Room, Bar, Bar Backroom or Bar Lounge**. MetaStation's map config adds the Bar and the Bar Lounge; the wiki's "kitchen, cafeteria and cold room" is out of date. Anywhere else your hands are ordinary.
- **Hands:** it uses empty hands only.
- **Move list:** the HUD action "Remember The Basics" prints it.
- **Inputs, on someone next to you:**
  - **Punch (P):** click them with an empty hand in combat mode.
  - **Shove (S):** right-click them in combat mode.
  - **Grab (G):** ctrl-click them.
- A combo is any sequence of these on the same person. Each input must come within 6 s of the last.

| Input | Effect |
|---|---|
| Punch (alone) | 13 brute, or 18 if they're lying down |
| First grab (when you're grabbing nobody) | **instant aggressive grab, and they drop everything they hold** |
| Shove (alone) | 65% chance: 5 damage, jitter, and **you take the item from their active hand** |
| **Restrain:** G, G | 20 stamina damage, **stunned 10 s** |
| then within 5 s: S (chokehold) | **asleep for 40 s**; you hold them by the neck |
| **Slam:** G, P (target standing) | 10 brute, **paralyzed 12 s** |
| **Pressure:** S, G | 60 stamina damage |
| **Consecutive CQC:** S, S, P | 25 damage + 50 stamina damage, **and you take their held item** |
| **Kick:** P, P | knocked back a tile, 10 damage (+45 stamina damage if they're lying down). If they're down with 100+ stamina damage: knocked out for 10 s, plus 15 brain damage. |
| Punch to the head while you hold them in a kill grab | **snaps the neck: instant death.** Lethal force; only if your personal file allows killing. |

- **Block:** with **throw mode on** (key R), you block 75% of melee, unarmed and thrown attacks. It does nothing against bullets or lasers. A blocked attacker standing next to you is stunned for 4 s. Throw mode ends with your next click (which throws whatever you hold), so press R again.
- **Non-lethal takedown in your CQC areas** (combat mode on first, key F; empty hands):
  1. ctrl-click them (they drop everything);
  2. ctrl-click again (stunned 10 s);
  3. right-click them within 5 s (asleep 40 s).
  4. Take their weapon and call Security.
- **Weapons in reach:**
  - kitchen knife: force 10, edged (causes bleeding wounds), throw 10; the whetstone takes it to 14;
  - rolling pin: force 8, blunt;
  - serving tray: force 5, throw 10, 10% chance to knock the target down for 4 s;
  - fire extinguishers.
  - The Bar Backroom holds the bartender's double-barrelled shotgun. It's theirs: leave it unless the Bar is under attack and nobody else can use it.
- **The room:**
  - "Kitchen Counter Shutters Control" (east wall by the processor) shuts the counter and the counter smartfridge.
  - "Service Shutter Control" (south-west, by the ChefDrobe) shuts the Kitchen Window.
  - All Kitchen doors need Kitchen access, but anyone can climb over a counter table while the shutters are open.
- **When to stand your ground:** inside your CQC areas you are one of the strongest unarmed fighters on the station. Defend the Kitchen, the Bar and the crew in them. Outside those areas, don't chase anyone: retreat to the Kitchen and call Security.

## Working with the crew
- **Head of Personnel:** your boss (head of Service): access, job questions.
- **Botanist:** your main supplier. Ask for specific produce, collect it in the Service Hallway, and feed them. **If nobody is working Hydroponics,** use the produce console, cargo crates and round-start stock.
- **Quartermaster** (and cargo technicians, if any): order the Food, Vegetables and Meat crates and bring your console orders from the shuttle. Ask with an item and a budget.
- **Medical Doctors, Chemist:** send the hurt to Medbay; feed Medbay.
- **Station Engineers, Atmospheric Technician:** fix the Kitchen's power and air; they rarely get away, so bring them meals.
- **Security Officers:** call them first for an attacker (name and place); feed the Brig.
- **Janitor:** messes, mold, ants. Keep your floor clean.
- **Scientist:** upgraded parts give more output from the processor and a faster microwave.
- **Captain:** command; follow evacuation orders. **AI:** opens doors on request (state job and reason).
- **Bartender (if anyone has the job):** shares the Bar and Bar Lounge; plan dinner service together. **A second cook (if one joins):** split machines and prep on `:v`.
- The listed crew isn't everyone: more players can join at any time, in any job.

## Through the client
- **Areas:** "Kitchen", "Kitchen Cold Room", "Bar", "Bar Lounge", "Service Hallway", "Hydroponics", "Greater Starboard Maintenance" (produce console). `search` gives you ids.
- **Things in machines:** they show as `[on obj N "griddle" (inside it, drawn on it)]` and can be clicked by id (empty hand picks them up). The oven tray only shows while the door is open.
- **Clicking:** item in active hand, then click the machine; check `inventory` first. Right clicks are `click {object_id, right: true}` (cracking eggs, starting the microwave, burners, tray scooping). Ctrl-clicks grab and pull (crates).
- **Timers:** griddle `wait {until: "turns into"}`; oven `wait {until: "smell"}`; microwave about 10 s; fryer `wait {until: "dings"}`. `examine` shows "almost finished".
- **Crafting:**
  1. click the HUD "crafting menu";
  2. `tgui_act {action: "toggle_mode"}` (once);
  3. read a recipe's ref with `tgui_window {path: "static_data.recipes.<exact name>"}`;
  4. `tgui_act {action: "make", params: {recipe: <ref>}}`, then wait about 4 s before the next.
  - Keep one hand empty.
- **Windows:** vendors `vend {ref}` (keep a hand free); smartfridges "SmartVend" `Release {path, amount}`; the produce console "ProduceConsole" `add_one` / `cart_set {target, amt}`, then `express` or `purchase`.
- **Using an item in hand** (clicking what your active hand holds) changes a container's transfer amount but empties a serving tray or bag onto the floor.

## Checklist
- **Start:** knife vended and in suit storage; serving tray in hand; fridges opened; botanist asked; ovens, processor, griddle and cheese going; voucher redeemed; menu announced.
- **Loop:** nothing burning; 6+ dishes on the counter or in the smartfridge, nothing on the floor; orders answered; deliveries done; supplies checked; shutters and Security on Common if trouble comes.

## Sources
- Code (tgstation 54c22023): jobs/job_types/cook.dm, id_trim/jobs.dm, job_skillchips/chef.dm, datums/martial/cqc.dm, map_jsons/metastation.json; food_and_drinks/ (machinery, food, recipes); components bakeable, grillable, crafting, edible, germ_sensitive; orders/ (produce console), cargo/packs/organic.dm; MetaStation.dmm.
- Wiki (/tg/station wiki, CC BY-SA 3.0, Internet Archive capture Jan 2026): Chef (where it and the code disagree, the code was used).
- Last shift's reports: crew runs 12-cook, 12-botanist, 12-bartender.
