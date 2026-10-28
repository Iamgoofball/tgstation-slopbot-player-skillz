# Spy (tgstation)

Rewritten from the wiki's Spy page. It is not checked against the server's code, and the page itself has an unfinished section (examples of bounties by difficulty). Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.

## 1. The role

A Spy is a lone antagonist: a crew member in your normal job with a **Spy Uplink**. You earn Syndicate gear by stealing the items on a shared **bounty list**. Your objectives are suggestions only ("set Engineering on fire", "frame someone"); you may pick your own goal or just steal. Difficulty: medium. Access is your job's, plus whatever you can get illicitly. Other spies may be aboard and are rivals, not allies.

## 2. The Spy Uplink

- Implanted in the device a traitor uplink would go in, usually your **PDA** (an uplink-implant preference falls back to the PDA).
- Only spies can open it. No lock code to remember. **It can't be replaced.**
- You can't buy gear with telecrystals; you get gear only from bounties.
- Use the uplink in hand to open the bounty list.

## 3. Bounties

- Bounties are minor theft tasks: an item, a machine, or a body part. Range: insulated gloves up to the AI upload, the clown's arm, Beepsky.
- **Shared by all spies; only one can claim each.** Keep your identity from other spies.
- Colour shows difficulty: **green easy, yellow medium, red hard.** Harder bounties give better rewards.
- **Claim:** right-click the bounty target with your uplink. It takes a moment, with an obvious visual tell and a quiet sound. A wall or two between you and witnesses is usually enough to hide the sound.
- **Body-part bounties** on a crew member: you don't need surgery. Incapacitate them (knock out with chemicals, crit, or kill) and scan the body with the uplink.
- After a set time the whole list refreshes, claimed or not.
- **Rewards:** random Syndicate devices, including most traitor items, some nuclear operative and clown operative items, and some spy-only rewards. Advanced gear such as MODsuits and heavy weapons is yours to use openly, but keep it out of Security's (and assistants') hands.

## 4. Tactics

- **Once exposed, expect the crew to try to kill you.** Confirmed antagonists are fair game for lethal force; plan your escape before you are seen.
- Start with easy bounties and build up.
- Generic items (a stun baton): claim at once, before another spy does. For unique targets it can pay to wait and see who else comes for it.
- If the list is all hard, lie low until it refreshes; gather tools, watch for other spies.
- Claimed items may appear on the Black Market under "fenced goods"; build a Black Market Uplink to buy them.
- If you're human, Asimov law 2 lets you order silicons to help; stealing isn't harm, but word it carefully, some will report you.
- Thermite burns through reinforced walls quickly; carry it in 50u beakers.
- Note other spies' rewards so you aren't caught by them; you can tip Security off anonymously.
- If a bounty targets you or your department, prepare a weapon (stunprod, spear), restraints (cablecuffs) and a disguise.
- Don't take every reward you can: pack light and use your job's abilities.

## 5. Limits that still apply

- Lone antagonist (`server-rules.md` section 4): any goal by any means, except metagaming or metacomms, bug or exploit abuse, erotic or creepy behaviour, OOC in IC, and spawn-camping arrivals.
- Snitching on other spies is fine IC; never use OOC knowledge of who they are.

## 6. For the crew

- A person right-clicking an item with a PDA while it glows is claiming a bounty.
- Spies carry gear they didn't buy: nuke-op or clown-op items on a crew member are a sign.
- Spies can't replace their uplink: confiscating the PDA ends their supply.
- Once a spy is confirmed (seen claiming, carrying reward gear), lethal force is fine; Syndicate rewards make them hard to hold.

## 7. Through the client

- **Open the uplink:** hold the PDA in your active hand and `click` it (use in hand); `tgui_window` reads the bounty list, `tgui_act` acts on it.
- **Claim:** with the uplink in hand, `click {object_id, right: true}` on the target. `look` around first; check no one is in view.
- Swap hands (`key {key: "X"}`) so the uplink is active before claiming.
- `inventory` shows what landed after a reward.

## 8. Checklist

- [ ] Uplink located (PDA) and bounty list read.
- [ ] Easiest bounties first; generic ones at once.
- [ ] Out of sight before every claim; walls between you and others.
- [ ] Plan serves your mission; no metagaming.
- [ ] Watch for other spies; keep the uplink safe, it can't be replaced.

## 9. Sources

- The /tg/station 13 wiki, "Spy" (CC BY-SA 3.0), as provided in `pages_to_turn_into_skills/antag_spy.txt`. Not checked against the server's code. The page's bounty-examples section is marked "TBA".
