# Regal Rat (tgstation)

The wiki's guide to the Regal Rat. It is not checked against the server's code. Where it disagrees with `crew-basics.md` or `server-rules.md` (the `tgstation-rules` skill), **those win**.

## 1. The role in one paragraph

A giant rat king who rules maintenance: hoard trash and cheese, raise an army of vermin, chew the power grid, and fight off anyone who intrudes. **You are not a full antagonist.** The wiki quotes an admin ruling: Regal Rats are a roleplay role like the space hermit; play your flavour text in good faith (hoard, claim a kingdom, gather minions), with **relaxed escalation** against anyone who interferes, but you are not free to do anything like an antagonist is.

## 2. How you spawn

- The Mice Migration event spreads about ten mice through maintenance; each has a 2% chance to be a Regal Rat (about 20% per event). Not tied to Dynamic threat.
- Feeding a mouse **Royal Cheese** (kitchen recipe) makes a non-sentient Regal Rat.
- Normal mice that eat cheese make more mice.

## 3. Stats

Health 70, melee 15, structure damage 10, slow (waddles). You can **speak and understand** the crew's language. Each rat gets a unique filthy royal name.

Healing: **eat cheese** (any kind; bigger heals more), or stand in rooms with enough **miasma**.

## 4. Abilities

| Ability | Cooldown | Effect |
|---|---|---|
| Raise Army | 4 s | Converts nearby mice, cockroaches and frogs into loyal rats, sewer roaches and trash frogs: tougher and hostile to all organics but you. With none nearby, spawns a mouse under you if your ratio of loyal rats to wild mice is high enough; otherwise it tells you to convert local mice first. |
| Regal Rat's Domain | 6 s | Puts out a little miasma, dirt and sometimes filth (rarely a slippery oil puddle). Repeat in a sealed room to heal passively. |
| Rummage | — | Use a disposal bin: 66% trash, 28% cheese wedge, 5% coins. Bins are mostly outside maintenance. |
| Rat Spit | 2 s | Lick food (not cheese) or a drink container: adds 1–3u Rat Spit. Causes nausea and vomiting; **20u+ (overdose)** makes the drinker rat-faction, so your rats won't attack them: a way to recruit humanoid subjects. |
| Ventcrawl | — | Alt-click a vent or scrubber. Scrubber (waste) pipes may be burning hot or freezing cold. |
| Pry airlocks | — | Click a powered airlock in combat mode. |
| Chew cables | — | Costs health; enough chewing blacks out areas. |

## 5. Royal Command

Say the word aloud; your loyal rats and roaches obey (trash frogs ignore you). Alt-click one creature for a radial menu of orders.

| Order | Words |
|---|---|
| Follow | "heel", "follow" |
| Stay | "sit", "stay", "stop" |
| Attack | "attack", "sic", "kill", "cheese em" — then **point** at the target (they shake their heads at invalid ones) |
| Release | "free", "loose" — they return to attacking any organic in sight |

## 6. Building the kingdom

- Early on you're weak: hide in maintenance and keep pressing Raise Army and Domain.
- Massed rats are deadly, even to cyborgs. Order "follow" to move the army; order attacks on structures and machines to tear them down.
- Oil puddles from Domain in tight corridors or at your entrance send pursuers sliding into your swarm.
- Ventcrawl everywhere until the crew welds vents.
- Hurt? Rummage bins for cheese or raid the kitchen, and lick the kitchen's and bar's food and drinks while there.
- A fun play: take over a little-used room of a department; trash it, break lights and machines, spread filth, guard it with rats, pry the airlock to nearby maintenance and cut the department's wires. Hold it until Security or someone dangerous shows up, then vent away and repeat.
- Talk to the crew: allies (a traitor, say) might help you depose the station's "king".
- **Don't fight directly**: a few laser shots kill you.

## 7. Rules: what limits you

- **Not a full antagonist.** Stick to your flavour: maintenance, hoarding, minions, your territory. Relaxed escalation applies to people who interfere with that; random murder outside it is not covered. If unsure, adminhelp.
- Rule 4's limits apply all the more: no metagaming, exploits, creepy behaviour, OOC in IC, or arrivals camping.
- **Expect to be killed once exposed.** Crew may kill an antagonist as soon as they're sure what it is; most antagonists can't be held safely, and a dead one goes back to the ghost pool. Stay hidden until you're ready to go loud, then fight to win.
- Fighting a rat (crew): once you're sure it's the Regal Rat, killing it is fine; weld vents, bring a laser, avoid narrow corridors full of rats and oil.

## 8. Common mistakes

| Mistake | Fix |
|---|---|
| Fighting in the open | Let the swarm fight; you hang back. |
| Raise Army with no mice converted | Convert wild mice first so it can spawn new ones. |
| Crawling the waste loop blind | It may be hot or frozen; use air vents. |
| Chewing cables at low health | It hurts you; heal first. |
| Acting like a traitor | You're a roleplay role with relaxed escalation, not a free antagonist. |

## 9. Through the client

- `screen` lists Raise Army and Domain; `click` them (spam them early).
- Orders: `say {text: "heel"}` and so on; for attack, `say {text: "sic"}`, then point (find the Point verb with `verbs`, use `call_verb`, or `click` with the modifier the client documents). Single-rat orders: `click` it with `alt: true` and pick from the radial menu.
- Ventcrawl: `click` a vent with `alt: true`. Pry: combat mode (`key {key: "F"}`), `click` the airlock.
- Rummage: `click` a disposal bin. Lick: `click` the food or glass.

## 10. Checklist

- [ ] Hide in maintenance; Raise Army and Domain on cooldown.
- [ ] Convert local mice and roaches; build the swarm.
- [ ] Claim a room; seal it and fill with miasma to heal.
- [ ] Cheese: rummage bins, raid the kitchen.
- [ ] Defend your kingdom; flee by vent when outmatched.

## 11. Sources

The /tg/station 13 wiki, "Regal Rat" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_regal_rat.txt. Not checked against the server's code.
