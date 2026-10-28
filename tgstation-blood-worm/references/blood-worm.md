# Blood Worm (tgstation)

The wiki's guide to the blood worm. It is not checked against the server's code. Where it disagrees with `crew-basics.md` or `server-rules.md` (the `tgstation-rules` skill), **those win** on the few limits in section 7. **The page is marked "under construction"**: it is mostly copied from the PR that added the worms (tgstation PR #93787) and its facts are unverified, so expect differences in game.

## 1. The role in one paragraph

Blood worms are a failed Syndicate bioweapon: space leeches that drink blood, grow through three stages, take over **corpses** as hosts, and reproduce. Duties: kill, consume, multiply, conquer. They are sentient and social; they recognise each other at a glance and share a language, **Wormspeak** (`.w`), but they are not a hivemind: each acts on its own. Access is wherever you can crawl, or whatever your host's ID opens.

## 2. Growth stages

| Stage | Health | Bite | Movement | Abilities (worm / in host) |
|---|---|---|---|---|
| Hatchling | 80 | 12–14 brute | ventcrawls; slides under doors (3 s) | Leech Blood, Invade Corpse, Mature / Inject Blood, Leave Host, Revive Host |
| Juvenile | 120 | 18–22 brute, often puncture bleeds | no vents; slides under doors (5 s) | adds Spit Blood (worm and host) |
| Adult | 180 | 25–30 brute | slower; can't slide under doors but **smashes airlocks** | Spit Blood with burst, Leech, Invade, **Reproduce** |

Everyone starts as a hatchling. **Mature** cocoons you for 30 s and needs more consumed blood each stage. **Reproduce** (adult, after a short cooldown) cocoons you for 30 s and makes **four hatchlings**, you among them.

## 3. Abilities

| Ability | Effect |
|---|---|
| Leech Blood | Drain blood from a living target or a reagent container. Aggressive grab holds them (about 1 s to start), causes oxygen damage. NPC monkeys can't escape and are floored. |
| Invade Corpse | Turn to blood and enter a corpse; you take all its blood and become it. Host blood loss damages you; you keep your fire weakness (but burn no longer does extra damage). |
| Spit Blood | Ranged corrosive spit. Right-click: melt your host's restraints; as an adult outside a host, a shotgun-like burst (long cooldown). All spit costs blood. |
| Inject Blood | Heal your host (organs, wounds and so on). Stronger as you grow; costs more blood and has a longer cooldown. |
| Leave Host | Leave after a delay (about 3 s), even if the host is dead, stunned or moving. |
| Revive Host | Revives a revivable host after an animation. |

Passives: no breathing (hosts too); insert organs into a host by right-clicking it with the organ; hosts live without heart, lungs or liver (lungs let you speak, a liver processes reagents); regeneration 0.3 / 0.4 / 0.5 HP/s by stage; night vision (not in a host); a blood HUD showing targets' blood and an antag HUD showing other worm hosts; examine a living target for more.

## 4. Tactics

- **Hatchling**: use vents to move unseen. Monkeys and medbay's blood freezers (synthetic blood; freezers are loud through walls) are easy blood. Mature as soon as you can.
- **Fast food**: invading a corpse takes all its blood at once. Blood gained while already in a host doesn't count toward growth; duplicated blood does but is synthetic and weaker.
- **Hosts are meat shields** with access. Heal them with Inject Blood when low, or in medbay to keep blood for spit (and avoid the tell-tale deathly pale skin).
- **Surprise**: block escape routes, then leave your host to attack, best as an adult.
- **Door stalking**: hatchlings and juveniles slide under doors after victims; watch for someone opening it.
- **Jail break**: Spit Blood right-click melts cuffs and breaks out of lockers; or leave the host and crawl or smash out.
- **Life insurance**: you're thrown out of the host at 10% health, a last chance to flee.
- **Jumpstart**: as an adult, gather corpses and blood for your hatchlings to grow fast after you reproduce.
- **Team up** with other worms in Wormspeak; spot their hosts on your HUD.

## 5. Weaknesses (and how the crew uses them)

Crew who are certain someone is a worm host may kill it outright; that is normal.

| Weakness | Detail |
|---|---|
| Heat and fire | You die fast; your blood burns if the host's core temperature is too high. Pick hosts with fire-resistant gear. |
| Bleeding | Host bleeding damages you directly; hosts bleed 50% faster and keep bleeding while dead ("just keep hitting them"). |
| Stuns | A stunned host can only be escaped by leaving it. |
| Space | Extreme cold and low pressure still hurt the worm itself; a space suit on the host protects you. |
| Testing | Security can order a blood worm testing crate (20 min cooldown from the security cargo console, or 10,000 credits at supply): 4 single-use, instant, 100% accurate testers. |

## 6. Common mistakes

| Mistake | Fix |
|---|---|
| Maturing out of hatchling in the open | Cocoon is 30 s helpless: hide first. Juveniles lose vents. |
| Letting the host bleed out | Inject Blood or medbay before it's critical. |
| Spending all blood on spit | Spit costs blood you need to heal and grow. |
| Hosting near fire, cremators or gibbers | Fire kills you; leave or move. |
| Reproducing with no food nearby | Stockpile corpses first. |

## 7. The few limits that still apply

- You are an antagonist: kill, consume and spread as fast as you can; nowhere on the station is off limits.
- Rule 4 still limits you: no metagaming or metacomms, no bug or exploit abuse, no erotic or creepy behaviour, no OOC in IC (or IC in OOC), no spawn-camping arrivals.
- **Expect to be killed once exposed.** Crew may kill an antagonist as soon as they're sure what it is; most antagonists can't be held safely, and a dead one goes back to the ghost pool. Stay hidden until you're ready to go loud, then fight to win.

## 8. Through the client

- `screen` lists your ability buttons; `click` one, then `click` the target. Right-click functions: `click` with `right: true`.
- Ventcrawl: `click` the vent with `alt: true` (assumed to work as for other ventcrawlers; the page doesn't say).
- Wormspeak: `say {text: ".w <message>"}`.
- In a host, `inventory` shows its gear and ID; `walk_to` uses its access.
- `examine` living targets for blood info; `status` for your health.

## 9. Checklist

- [ ] Hatchling: vents, find monkeys or blood bags, drink, mature somewhere hidden.
- [ ] Find a corpse; invade it for a host and its blood.
- [ ] Keep host healed and away from fire; break restraints with spit.
- [ ] Adult: stockpile corpses, reproduce, feed the hatchlings.
- [ ] Coordinate with kin in Wormspeak.

## 10. Sources

The /tg/station 13 wiki, "Blood Worm" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_blood_worm.txt. Not checked against the server's code.
