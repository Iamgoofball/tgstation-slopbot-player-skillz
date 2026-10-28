# Bartender (tgstation)

The wiki's guide to the Bartender. It is derived from the wiki page and is **not checked against the server's code**. **Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.**

## 1. The role

Service job under the **Head of Personnel**; you and the Cook run the station's front of house. Bare minimum: stay at the bar and give people drinks in glasses. Difficulty: easy.

## 2. Kit, access, radio

- **Access:** Bar, Theatre, ORM, weapon permit. The wiki lists Hydroponics, Kitchen and Morgue as additional (may vary).
- **Radio:** Service `:v`, Common `;`.
- **Equipment:** armour vest, double-barrelled shotgun (beanbags loaded, spares in your bag), shaker, Barman Recipes book, beer goggles, drink display smartfridge (some maps), Bardrobe vendor (formal wear, shoes, top hats; a spare top hat on the bar).
- **Booze-O-Mat:** ID-locked vendor with every spirit.
- **Back room:** beer keg, beer locker, vendors and a blender/mixer.
- **Pun Pun:** your monkey. Pushes people, rings the bell, gets abused and harvested by the Cook.
- **Beer goggles:** show reagents in drinks; let you throw glasses without breaking or spilling them.

## 3. The shotgun

Two shells, fires both in quick succession. Use it in hand to break it open (shells drop on the floor). Starts with two beanbags. More shells from Cargo's autolathe.

| Shell | Effect |
|---|---|
| Beanbag | 1 projectile, 10 brute, 55 stamina. |
| Rubbershot | 6 pellets, 3 brute + 11 stamina each. |
| Dart | 5 brute, injects up to 30u of a loaded reagent. |
| Incendiary slug | 20 brute, sets target on fire. |
| Lethal slug | Removed from autolathes (Dec 2020). |

- A circular saw (autolathe) saws it off to fit in a bag. **Unload first**: sawing a loaded gun fires it into your face.
- Science's technological shells unlock crafted ammo (meteorslug, pulse slug, dragonsbreath and more).
- The shotgun is for defending the bar and yourself under the escalation rules, not for settling arguments.

## 4. Running the bar

- Mix drinks from the Booze-O-Mat with the shaker; recipes in the book and the wiki's drink guide.
- **Diluting:** water reduces a drink's (and a bloodstream's) alcohol strength in proportion: 25u water + 75u booze is 25% weaker, 50/50 halves it.
- The Chemist will usually supply extra chemicals; many reagents have their own taste and can be added for new flavours.
- Keep finished specials in the drink display, not scattered on the counter.
- Bar fights get deadly when Security is drunk; people also like to attack the bar. Beepsky Smash attracts trouble.

### Drinks with effects

| Drink | Effect |
|---|---|
| Vodka | Cures some radiation. |
| Screwdriver | Purges radiation well: serve Engineering. |
| Beepsky Smash | Illusory Beepskies chase the drinker (stamina damage); heals Security's stamina; drinker can't hold items. Needs iron (techfab). |
| Milk cream / orange / lime / tomato juice | Small heal: brute / oxygen / toxin / burn. |
| Nothing, banana juice | Heal clowns and mimes of all damage. |
| Carrot juice | Heals eye damage. |
| Cream, milk, soy milk, café latte, soy latte, chocolate milk | 20% chance per roll to heal 1 brute. Get a cow. |
| Dr. Gibb | Prevents drowsiness. |
| Lemon-lime, iced tea, iced beer, Thirteen Loko, Space-Up | Cool you down. |
| Antifreeze, sbiten, soy latte, coffee, chocolate, Toxins Special | Warm you up. |

### Bottles

Bottles can be drunk, thrown (splash) or smashed over heads (knockdown if the target lacks sturdy headgear). A tray on your belt carries many bottles; the quick-equip-belt hotkey draws them fast. Useful fills: synthflesh (heals on splash, leaves toxin; tea helps), condensed capsaicin from a Security pepper spray refiller (knocks down and blinds exposed skin; good to hand to Security or the Clown). Ask the Janitor for cleaner grenade beakers; foam (fluorosurfactant) makes a healing keg stand.

## 5. Pun Pun as a player

- Genetics: scan Pun Pun's UI+UE and SE. Inject a **willing** player with the SE (they become a monkey), then the UI+UE.
- Or put a Mind Magnification helmet (Cargo) on a monkey to give it a ghost.
- Talk to it with a pAI. Handcuffing it to a chair is restraint: only with the player's consent.

## 6. Traitor bartender

When the game makes you a traitor, go after your objectives with everything below. Rule 4 limits still apply (no metagaming, exploits, OOC in IC, spawn-camping); see `server-rules.md`.

- You only have Bar access; being absent from the bar draws attention. Stay there as cover.
- Lethal shells need Cargo's help; they can use your shotgun to open locked crates, a basis for a deal. An emag helps.
- Stuns: Beepsky Smash, neurotoxin (stronger than chloral hydrate). Poisoned drinks.
- Bottle over the head drenches the target: flammable fill plus a lighter, or acid.
- The damp rag soaked in a chemical carries 5u; use it on someone in combat mode to smother (not through mouth cover).
- A pill dropped in a not-full glass gives a visible message.
- Toxins kit plus shotgun darts: one-shot kills (20u polonium is lethal).
- Emag on the bar screen makes a Syndicate Café sign (cosmetic).

As a non-antagonist, the wiki's harmful bottle "pranks" (acids, ants, itching powder on crewmates) are griefing: save them for when you are a traitor.

## 7. Common mistakes

| Mistake | Fix |
|---|---|
| Sawing a loaded shotgun | Break it open first. |
| Shooting troublemakers | Ask them to leave, call Security on `;`; shotgun only for self-defence. |
| Overserving Security | Dilute with water. |
| Leaving the bar unattended | Tell Service on `:v` if you step out. |
| Splashing harmful bottles on crew | Not allowed unless you are an antagonist. |

## 8. Working with others

Cook (food partner), Botanist (juices), Chemist (reagents), Cargo (shells), Janitor (glass and spills), HoP (your head).

## 9. Through the client

- Booze-O-Mat, Bardrobe and the drink display open tgui windows: `tgui_window`, then `tgui_act` (read the button names first).
- Pouring: hold a glass or bottle, `click` the target container. Shaker in hand, `click` to fill; examine to check contents.
- Serving: put the drink on the counter (click the table with it in hand) and `say` what it is.
- `inventory` before every `click`: a shotgun in hand on a patron shoots them in combat mode.
- Radio: Service `:v`, Common `;`.

## 10. Checklist

- [ ] Shotgun checked and kept behind the bar; vest on.
- [ ] Booze-O-Mat and back room stocked; shaker and glasses ready.
- [ ] Bar announced open on Common.
- [ ] Engineering offered Screwdrivers; Security drinks diluted.
- [ ] Counter clean, specials in the display.

## Sources

The /tg/station 13 wiki, "Bartender" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/bartender.txt. Not checked against the server's code. The page notes lethal shells were removed from autolathes (Dec 2020).
