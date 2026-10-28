# Holoparasite (tgstation)

The wiki's guide to holoparasites (the tech version), guardian spirits (the magic version) and power miners. It is not checked against the server's code. **Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.** The page is short: it gives no numbers for damage, ranges or cooldowns.

## 1. The role

A holoparasite is a ghost-like being bound to one person, its summoner, and living inside them. You follow your summoner, do what they say, and keep both of you alive. Your summoner's role decides what you are for. If they are a traitor or a wizard, you serve their objectives at all costs, and everything below is fair play. If they are a shaft miner with a dusty shard and not an antagonist, they are crew, and you act as crew under `server-rules.md`.

## 2. How one is made

| Source | Who gets it | Type |
|---|---|---|
| Holoparasite injector (nanomachines) | Traitors (uplink) | Summoner chooses |
| Guardian deck (tarot cards) | Wizards | Summoner chooses |
| Dusty shard | Shaft miners (power miner) | Random |

Magic and tech versions differ only in how they are summoned and how they look; the abilities are the same. Once summoned, you pick your own name and colour.

## 3. Bound to the summoner

- **Telepathy:** you talk to your summoner through a HUD icon; they answer with a button in the **Guardian tab**. Nobody else hears it.
- **Manifest and recall:** come out of and go back into your summoner at will.
- **Leash:** go too far and you are pulled back to them.
- **Shared damage:** you can't be killed on your own, but damage you take passes to your summoner, at a reduced amount.
- **Shared death:** if the summoner dies, you die, and their body is dusted at once (no revival).

Protect your summoner first. Recall when you are being shot; manifest to fight.

## 4. Types

| Type | Strengths | Weaknesses and notes |
|---|---|---|
| Standard | Rapid, devastating melee; high damage resist; smashes weak walls | Close range only. Pick a battle cry (up to 6 letters) shouted over and over while attacking. |
| Assassin | Stealth: the next attack from stealth does massive damage and ignores armour | Medium damage, takes full damage; briefly can't recall after a stealth attack. |
| Gaseous | Releases a chosen gas: O2, N2, CO2, BZ (hallucinations), H2O (slippery floor), N2O (knocks people out), plasma (toxic, flammable). Punches spark. Keeps the summoner's temperature stable and puts them out if burning. | Sparks ignite plasma; keep your summoner out of the fire. |
| Charger | Very fast; charges at a target, damaging the first one hit and making them drop held items | Medium damage. |
| Explosive | High damage resist, medium attacks. **Alt-click any object** (even ones too big to lift) to trap it: the next person to touch it takes explosive damage. | The trap fades after a delay or once triggered. Examining it shows "It glows with a strange light!" |
| Gravitokinetic | Hits put heavy gravity on the target (slowed, drops items); **alt-click the ground** to place gravity fields | Fields vanish when you recall or go over 10 tiles from them. Average stats. |
| Lightning | Attacks chain lightning to targets; you also have a chain to your summoner. Chains shock everything near them for constant damage. | The chain to your summoner shocks whoever stands near it. |
| Protector | Your summoner teleports to you when out of range. Combat mode: medium damage dealt and taken. Protection mode: almost no damage dealt or taken, slightly slower. | Use protection mode as a shield. |
| Ranged | Two modes; one fires a constant stream of weak, armour-ignoring projectiles. Lays surveillance snares that alert you when crossed. | Low damage per shot. |
| Dexterous | Holds items in its hands and stores one item inside itself | Low damage. Drops held items on recall; keeps the stored one. |
| Support | Two modes; **Healer** mode heals instead of damaging. Deploy a **bluespace beacon** (verb in the Guardian tab), then **alt-click** someone to warp them to it (not instant), your summoner included. | Low damage resist and slow in healer mode. |

## 5. Tactics (antagonist summoner)

- Stay recalled while your summoner blends in; manifest only to strike. A visible guardian outs your summoner.
- **Standard, Charger, Assassin:** ambush targets in maintenance. Charger disarms first, then you both finish them. Assassin opens from stealth for the kill.
- **Gaseous:** N2O to knock out a room before your summoner walks in; plasma plus your sparking punches to burn Security or a target's department. Get your summoner a gas mask and internals first.
- **Explosive:** trap doors, consoles, a target's locker, or armoury gear.
- **Support:** put the beacon in a hidden base and warp stunned targets there (stun first so they can't walk off during the delay), or warp your summoner out when cornered. Heal them mid-fight.
- **Dexterous:** carry the stolen objective or your summoner's weapon inside you, out of reach of searches.
- Once your summoner is exposed, the crew will try to kill them, and you die with them. Keep them out of crit: recall, use Protector's protection mode, heal with Support, flee early.

## 6. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Tanking hits while manifested | The damage goes to your summoner. Recall when focused. |
| Wandering off | The leash pulls you back, and your summoner is unguarded meanwhile. Stay close. |
| Plasma and sparks near your summoner | You burn them too. Masks and distance first, then ignite. |
| Lightning chain near allies | It shocks everyone near it, your summoner's friends included. |
| Ignoring your summoner | You serve them. Ask by telepathy what they want, and report what you see. |
| Letting the summoner die | Their body dusts and you die with them. Their survival comes first. |

## 7. Fighting one (crew)

- Kill the summoner: the guardian dies with them and can't be killed on its own. Once someone is confirmed beyond doubt to have a hostile guardian, lethal force is normal and expected.
- Damage on the guardian bleeds through to the summoner, so shooting it still helps.
- Examine suspicious objects for "It glows with a strange light!" before touching them (Explosive traps).

## 8. Through the client

- Guardian-tab actions (telepathy, beacon) and the telepathy HUD icon: list HUD buttons with `screen` and `click` them by id; tab verbs show in `verbs` and run with `call_verb`. Read the exact names there; don't guess them.
- Telepathy text comes as a prompt or input window: `answer_prompt`, or `tgui_act` on a tgui input.
- Alt-click abilities (Explosive traps, gravity fields, Support warps): `click` the target with `alt: true`.
- `look` before manifesting to see who is watching; `read_chat` and `wait {from_others: true}` for your summoner's messages.

## 9. Checklist

- [ ] Name and colour set; type known; summoner's role and objectives known.
- [ ] Telepathy working both ways.
- [ ] Recalled until needed; manifest to strike.
- [ ] Summoner kept out of crit; recall or flee when the fight turns.

## Sources

The /tg/station 13 wiki, "Guardian Spirit" (Holoparasite) (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_holoparasite.txt. Not checked against the server's code.
