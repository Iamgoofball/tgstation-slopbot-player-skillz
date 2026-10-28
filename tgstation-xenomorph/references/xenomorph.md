# Xenomorph (tgstation)

The wiki's guide to playing the xenomorph hive and fighting it. It is not checked against the server's code. Where it disagrees with `crew-basics.md` or `server-rules.md` (the `tgstation-rules` skill), **those win**, except for the few limits in section 7.

## 1. The role in one paragraph

Xenomorphs are a midround threat (usually a random event: one larva spawns on the station; also wizards or, rarely, xenobiology). There are no written objectives: build a nest, grow the hive, take the station. Xenos have night vision, see humans through walls, rip open airlocks, are space-proof, and talk on the **hivemind**. The Queen leads; the rules count her as a **team antagonist**, and other xenos should follow her where they can.

## 2. The life cycle and castes

| Form | Role | Notes |
|---|---|---|
| Facehugger | NPC | Hatches from Queen eggs; leaps at humans and monkeys, tears off most face protection, implants a larva, dies. Adult xenos can pick them up and throw them. |
| Larva | you, at first | Bursts from a host's chest. No real attack. Hides under tables, ventcrawls. Grows by staying on weeds, then evolves into Hunter, Sentinel or Drone. |
| Hunter | offence | Very fast, pounce stun, neurotoxin, small plasma pool. Ventcrawls. Best at catching hosts and spreading weeds. |
| Sentinel | nest guard | Slower, tougher, big plasma pool and fast recharge (more spit and acid). Partial invisibility while still. |
| Drone | builder | Resin walls, membranes (windows), nests (beds). The only adult that can evolve further, into a Praetorian. |
| Praetorian | heavy | Queen-like abilities without eggs. Becomes Queen if there is none. Can't ventcrawl. |
| Queen | leader | One per hive. Lays eggs. Tough in melee, tail swing knockback (long cooldown), very slow, can't ventcrawl. |

## 3. Shared mechanics

- **Hivemind**: the page gives both `.a` and `:a`; start your line with one of them (try `:a` first, the page's main text).
- **Plasma**: all adults build it over time and spend it. **Plant weeds** first; weeds spread resin, and standing on resin speeds plasma regen.
- **Corrosive acid**: melts a structure or object slowly (any wall eventually).
- **Neurotoxin spit**: ranged stun. Click the ability to ready it, then click the target.
- **Right-click** in melee stuns/knocks down; then attack.
- **Ventcrawl**: Alt-click a vent (larvae, hunters, sentinels, drones).

## 4. Procedures by caste

### First xeno alone (larva)
1. Get safe: vents, under tables; solars in space are a good hide (you're space-proof).
2. **Become a Drone.** You must reach Queen to start the hive. Choosing Hunter as the only larva wastes the round.
3. Pick a safe, out-of-the-way, defensible nest site with room for eggs **before** evolving to Praetorian/Queen (you lose ventcrawling).
4. Lay weeds and resin, stay on them until you have enough plasma, evolve.

### Queen
1. Nest out of sight; smash cameras the AI could watch.
2. Weeds down, then spend all plasma on eggs. Click a grown egg to open it, click again to clear it after the hugger leaves, lay more.
3. First hosts: monkeys (Virology, Genetics) don't fight back. Carry a facehugger in each hand, throw, drag hosts back to the nest. Humans hit by a thrown hugger usually go down.
4. Medbay can remove a larva surgically: get hosts to the nest fast.
5. **Survive above all**: if you die with no successor the hive ends. Ranged attackers are your weakness; tail swing and right-click stuns for melee.
6. Once a Hunter is up, let it do the hunting; you keep laying.

### Hunter
- Leave the nest with a facehugger in each hand.
- Ready pounce, click a target: you leap and stun them. Shields stun **you** instead.
- Hugger them, drag them to the nest, right-click to keep them down. Drop them if you must retreat.
- Strip prey of items, **radios first**. Plant weeds around the station as pit stops. Spend your small plasma pool carefully.

### Sentinel
- Guard the entrance, invisible, on resin. Keep captured hosts buckled until the larva bursts. Spit at intruders; melt walls for the drones.

### Drone (with a Queen)
- Resin walls for mazes and barricades, membranes where seeing out helps, **resin nests** to buckle hosts on.
- Smash lights and cameras in the nest. Fight only if no one else can; protect the Queen.
- If the Queen dies, a Drone must become the new one (after a long wait): get safe, weed, evolve, lay.

## 5. Common mistakes

| Mistake | Fix |
|---|---|
| Only larva picks Hunter | Drone, then Queen. |
| Evolving to Queen somewhere unsafe | Pick the site first: no ventcrawling afterwards. |
| No weeds | Plasma first, always. |
| Hunting humans before the hive exists | Eggs first; monkeys are easy hosts. |
| Pouncing a riot shield | You're the one stunned. |
| Leaving radios on prey | Strip them. |
| Queen fighting at range | Retreat; she can't trade shots. |

## 6. Fighting xenos (crew)

Once you're certain it's an antagonist, lethal force is normal and expected: don't try to arrest or brig it. Confirm first.

- **Weld the vents and scrubbers** in your area (eye protection). Losing air flow is a small price.
- Facehugger-proof headgear: bio hoods, riot helmets, hardsuit and space helmets, flipped-down welding masks. Pull a hugger off a friend fast.
- Xenos are **weak to fire**; energy weapons next, then ballistics. Melee is a bad idea. Beat up lone larvae.
- An infected person can be saved by surgery; weld the surgery room's vents and be ready to kill the larva. Spacing an infected body only delays it.
- Space suits and jetpacks let you attack from space, where they like to hide.
- Cargo can order guns; genetics can give pressure/temperature adaptation and hulk; robotics can build combat mechs.
- Dead xenos: their organs sell well and can be implanted for xeno abilities.
- In a class A emergency, plasma-flooding and torching the nest, engineering borgs dragging welder-fuel tanks in, or toxins bombs can be worth the collateral: warn your allies first. (The "Queen must duel a Ripley" line is a joke.)

## 7. The few limits that still apply

- Queens (and Praetorians leading) are team antagonists: don't harm the hive's work, by action or by doing nothing. Other xenos follow the Queen's direction where they can.
- Otherwise take the station by any means: break windows and vent the nest's air so humans need suits, break cameras, kill or infect anyone.
- Rule 4 still limits you: no metagaming or metacomms, no bug or exploit abuse, no erotic or creepy behaviour, no OOC in IC (or IC in OOC), no spawn-camping arrivals. Everything else that serves your objectives is fair game.
- **Expect to be killed once exposed.** Crew may kill an antagonist as soon as they're sure what it is; most antagonists can't be held safely, and a dead one goes back to the ghost pool. Stay hidden until you're ready to go loud, then fight to win.

## 8. Through the client

- Hivemind: `say {text: ":a <message>"}` (or `.a`).
- `screen` lists your abilities (weeds, evolve, acid, spit, pounce, invisibility, eggs, resin); `click` the button, then `click` the target where one is needed.
- Ventcrawl: `click` the vent with `alt: true`. Right-click stuns: `click` with `right: true` in combat mode (`key {key: "F"}`).
- Throw a held facehugger: `key {key: "R"}`, then `click` the target. Pull prey: `click` with `ctrl: true`.
- `status` shows plasma and health.

## 9. Checklist

- [ ] Larva: hide, talk on the hivemind, see if a Queen exists.
- [ ] No Queen: Drone, pick a nest site, weeds, evolve Queen.
- [ ] Queen: weeds, eggs non-stop, cameras broken.
- [ ] Hunters: two huggers, monkeys first, drag hosts home, strip radios.
- [ ] Hosts buckled on resin nests and guarded.

## 10. Sources

The /tg/station 13 wiki, "Xenomorph" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_xenomorph.txt. Not checked against the server's code.
