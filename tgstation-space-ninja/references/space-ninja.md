# Space Ninja (tgstation)

The wiki's guide to the Space Ninja. It is not checked against the server's code. Where it disagrees with `crew-basics.md` or `server-rules.md` (the `tgstation-rules` skill), **those win**, except for the few limits in section 7.

## 1. The role in one paragraph

A midround antagonist given to a random ghost: a Spider Clan agent who spawns in space near the station. You are a **saboteur, not a killer**: stealth, doorjacking, hacking and power theft. You get six standard objectives plus "survive"; you're not forced to follow them, but try.

## 2. Kit

- **Ninja MODsuit**: space suit, minor armour, all your powers. It runs on **electricity**. You **can't use guns** while wearing it.
  - Boots: no-slip. Mask: enhanced (night) vision. Hood: the AI can't track you.
  - Gloves: work like an emag; right-click with an empty hand to use them on airlocks, APCs and objective consoles.
- **Energy katana** on your belt. **Spider bomb** and an emergency oxygen tank in your pocket.
- A built-in self-destruct (microbomb) that fires if you die. Never press it yourself.
- Old features gone: the suit no longer holds a pAI; the energy net no longer sends people to the Dojo.

## 3. Abilities

| Ability | How | Notes |
|---|---|---|
| Dash | katana in hand, right-click an empty visible tile | Teleports there, through doors and windows. 3 charges, refill over time. Loud and obvious. Use it to reach the station from space. |
| Recall Katana | hotbar | Warps it back; costs more energy the further it is; hurts people between you and it. The katana is good thrown too. |
| Katana attack | click | Doesn't stun on the first hit. |
| Glove: siphon | touch APC, SMES, wire, cell, cyborg | Recharges you. Stand still; noisy, sparks. Hacks APCs visibly (people blame the AI). Highly charged SMES give the most. |
| Glove: doorjack | touch a door | Hacks it open permanently. Low cooldown, unlimited. A **bolted** door stays bolted and becomes nearly unopenable. |
| Glove: shock | touch a person | 3 s stun. |
| Glove: convert cyborg | touch and hold 6 s | Once per round (objective). |
| Phase Cloak | hotbar toggle | Near-invisible; drains energy slowly. **Taking damage disables all suit powers for 5 s**, cloak included. |
| EM Burst | hotbar | Large EMP around you: cameras off, borgs stunned, energy weapons drained. Very expensive on the base cell. |
| Throwing stars | hotbar, in hand | Cheap; embed and deal steady stamina damage. |
| Energy Net | hotbar | Traps one target; they can break it slowly. Good one-on-one. |
| Adrenaline Burst | hotbar | Removes stuns and slows instantly; 5u stimulants (90% shorter stuns, faster) for ~50 s; also 5u radium (~15 toxin). One use; refill by using a container of **20u radium** on the suit. |
| Status | hotbar | Your health and state. |

## 4. Objectives

1. **Convert a cyborg**: gloves, hold 6 s. EMP it first, with no crew around. It becomes a random Syndicate borg (assault, medical, saboteur) with matching laws, an antagonist of its own. Once per round; deactivated borgs and AI shells also count.
2. **Steal X research nodes**: touch the R&D server (Bridge or Science) with your gloves. Only researched nodes count: do this last, or spend points yourself at a console.
3. **Doorjack X doors**: maintenance doors are the safe way to meet the quota; vital doors cause more trouble and make your presence obvious.
4. **Detonate the spider bomb in the named room**: only works there. Use it in hand to set the timer, plant it on a wall or floor of that room, run. Big, loud blast: a great distraction.
5. **Set everyone to arrest**: gloves on any security records console, 20 s, the AI is alerted when you start. Then everyone is Wanted. Departmental security posts have consoles; use a quiet one.
6. **Call in another threat**: gloves on a communications console, 20 s, AI alerted. Summons another side antagonist (pirates, swarmers, a space dragon...). If command guards the console, build one from Secure Tech Storage (the AI may bolt it; your converted borg can help).
7. **Survive** to the end.

## 5. Upgrades

- **Bigger power cell**: screwdriver opens the suit cover; the suit must power down and up again (slow).
- **Full oxygen tank** in place of the emergency one.
- **Radium (beaker) and toxin-healing patches**: more Adrenaline uses; the toxin builds up. Only patches work in the suit.
- **MOD modules**: DNA lock and status readout are useless; springlock speeds start-up (avoid water); a jetpack is useful.

## 6. Tactics

- Stay in the dark; use night vision. Cloak when moving, but avoid getting hit while cloaked.
- Not everyone has to die: a witness may keep quiet if you spare them.
- To capture: make cable restraints, shock with the gloves, cuff; EMP their radio.
- Escape into space. Don't kill all the engineers: you need their power.
- EMP Beepsky.
- **Hunger**: each step costs hunger and you move fast. Eating means taking the suit off (slow, vulnerable). Stock good food from the Cook; healthy food slows hunger and eases the radium. Eat off-station.
- Watch power, health, hunger and objectives together; check status often.

## 7. The few limits that still apply

- You are a lone antagonist (rule 4): bomb the target room, open the external airlocks, drain the SMES, call in the next threat. Do whatever gets the objectives done.
- Rule 4 still limits you: no metagaming or metacomms, no bug or exploit abuse, no erotic or creepy behaviour, no OOC in IC (or IC in OOC), no spawn-camping arrivals. Everything else that serves your objectives is fair game.
- **Expect to be killed once exposed.** Crew may kill an antagonist as soon as they're sure what it is; most antagonists can't be held safely, and a dead one goes back to the ghost pool. Stay hidden until you're ready to go loud, then fight to win.

## 8. Common mistakes

| Mistake | Fix |
|---|---|
| Spending all dash charges | Keep one for escape. |
| Running dry on power | Siphon whenever safe; upgrade the cell. |
| Doorjacking a bolted door | It becomes unopenable; check first. |
| Hacking consoles in public | 20 s and the AI is told: pick a quiet console. |
| Stealing research before any exists | Do it late. |
| Taking hits while cloaked | Powers drop for 5 s; break line of sight first. |
| Starving | Carry food; eat in a safe place. |
| Losing the spider bomb | Keep it pocketed even if you never use it. |

## 9. Fighting a ninja (crew)

Once you're certain it's an antagonist, lethal force is normal and expected: don't try to arrest or brig it. Confirm first.

Loud dash noises, sparking APCs, doors hacked open everywhere and a sudden "everyone is wanted" are signs. The AI can't track a ninja's hood. EMPs and water (springlock) hurt them; damage drops their cloak for 5 s. A dead ninja explodes: step back.

## 10. Through the client

- `screen` lists the suit's hotbar abilities; `click` one to use or toggle it.
- Dash: katana in the active hand, `click` the target tile with `right: true`. Glove use: empty active hand, `click` the target with `right: true` (the page says right-click).
- Bomb timer: hold it, `key {key: "Z"}`.
- Talk in plain `say`; the AI hears its own alerts, not you.
- Objectives: `read_chat` and the notes verb (`verbs` / `call_verb`).

## 11. Checklist

- [ ] Read the objectives; note the bomb room and quotas.
- [ ] Dash in from space; siphon power on arrival.
- [ ] Doors quota (maintenance first).
- [ ] Records console and comms console, each in a quiet spot.
- [ ] Convert one cyborg (EMP first). Research theft late.
- [ ] Keep power, food and health up; survive.

## 12. Sources

The /tg/station 13 wiki, "Space Ninja" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_space_ninja.txt. Not checked against the server's code.
