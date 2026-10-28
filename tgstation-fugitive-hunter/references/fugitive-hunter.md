# Fugitive Hunter (tgstation)

The wiki's guide to the Hunters. It is derived from the wiki page and is **not checked against the server's code**. **Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.**

## 1. The role

The Fugitives/Hunters event fires with **more than 20 active crew** and at least **30 minutes** into the shift. Fugitives spawn in maintenance with a toolbox and no access. **10 minutes later** your hunter team spawns on its own shuttle. Your job: capture the fugitives, dead or alive, and bring them back to your shuttle, while convincing the crew not to shoot you. If the fugitives have been causing trouble, the crew may help.

Access: basic, varying by team; anything else you must get by other means.

## 2. Rules for you

You are **not a Rule 4 antagonist**. The wiki's admin note:

- Don't kill crew unprovoked. If Security is helping you, shooting them earns an admin PM.
- You may do anything to **capture the fugitives**.
- If Security cooperates with the fugitives, you may use force against them.
- Fugitives and anyone shielding them are fair game: use whatever force gets the capture. The general antagonist limits in `server-rules.md` (no metagaming, exploits, OOC in IC) also apply.

## 3. Shuttle and tools

- The shuttle can dock directly at the **arrivals auxiliary dock**.
- **Bounty Locator** (on the shuttle): reveals the location of one fugitive on board the station.
- **Shuttle Pinpointer**: points back to your shuttle once you have a fugitive.
- A capture counts dead or alive, but **alive** is the best result (Badass Security Victory).

## 4. Hunter teams

| Team | Kit and notes |
|---|---|
| SpacePol | Space police, HUD implants that recognise the fugitives. Moderately armed; start with a pistol. Security may or may not cooperate. |
| Russians | Space-Russian smugglers, many of them, poor gear, each with a Mosin-Nagant surplus rifle: lethal, bulky, manually reloaded. Aim at legs if you want them alive. |
| Bounty Hunters | Small team with exotic weapons (flamethrowers, double-barrelled shotguns); one may be a synth. **Traps** that only trigger on fugitives (harmless to crew) and broadcast their location to all bounty hunters. |
| Psyker Shikari | Three psykers who navigate by echolocation plus their Seer, who must guide them. Very heavily armed; use your abilities, and don't overdose on "gore". |
| MI13 | Covert agents: suppressed Makarov pistols, lightly armoured tuxedos, a random spy gadget each. Shuttle can spy on station comms and cameras. Microbombs implanted in case of capture. Security unlikely to welcome you. |

## 5. Outcomes

| Result | When |
|---|---|
| Badass Security Victory | Every fugitive captured alive. |
| Major Security Victory | Every fugitive captured. |
| Postmortem Security Victory | Every fugitive captured, all dead. |
| Security Victory | A fugitive captured. |
| Minor Security Victory | All hunters died but a fugitive was captured. |
| Stalemate | Everyone died, no fugitive recovered. |
| Minor Fugitive Victory | All fugitives died, none recovered. |
| Fugitive Victory | A fugitive survived, no bodies recovered. |
| Major Fugitive Victory | All fugitives survived uncaptured. |

## 6. Tactics

- Use the Bounty Locator early, then search maintenance; fugitives start there with no access.
- Talk to Security and Command first. Explain who you are; a cooperative station is a huge advantage, a hostile one a second front.
- Prefer non-lethal takedowns and bring them back alive.
- Bounty Hunters: lay traps in maintenance chokepoints.
- MI13: use the shuttle's comms and camera spying to find targets.

## 7. Common mistakes

| Mistake | Fix |
|---|---|
| Shooting crew in the way | Only fugitives and those actively protecting them. |
| Kill without recovering the body | A capture means getting them to your shuttle. |
| Barging in armed with no explanation | Announce yourself and ask for cooperation. |
| Getting lost with a prisoner | Use the Shuttle Pinpointer. |

## 8. Recognising hunters (crew)

An unknown shuttle at arrivals' auxiliary dock, armed strangers (police, Russians with rifles, bounty hunters with flamethrowers, tuxedoed agents) asking after fugitives. They are not automatically enemies; you may help either side with IC reason.

## 9. Through the client

- Locator, pinpointer and shuttle consoles: `tgui_window` then `tgui_act`; read the window first.
- `inventory` before `click`; combat mode with `key {key: "F"}` only for an actual fight.
- Negotiating: `say` in person, or `;` on Common if you have a headset.
- Dragging a captive: grab/pull, then `walk_to` back to the shuttle.

## 10. Checklist

- [ ] Rules read: no unprovoked crew kills.
- [ ] Team kit checked; locator used.
- [ ] Security contacted.
- [ ] Every fugitive captured, ideally alive, on the shuttle.

## Sources

The /tg/station 13 wiki, "Hunter" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_fugitive_hunter.txt. Not checked against the server's code. Original PRs: tgstation #42554, #44802.
