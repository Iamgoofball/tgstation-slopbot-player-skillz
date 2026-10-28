# Fugitive (tgstation)

The wiki's guide to the Fugitive. It is derived from the wiki page and is **not checked against the server's code**. **Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.**

## 1. The role

Fugitives come from a random event ("Fugitives / Hunters") that can only fire with **more than 20 active crew** and at least **30 minutes** into the shift. Ghosts get a prompt; the winners become a solo fugitive or a team. You spawn in **maintenance** with a single **toolbox** and **no access**. **10 minutes later** a team of Hunters arrives. From then on your goal is to avoid capture, or kill the hunters.

## 2. Rules for you

You are **not a Rule 4 antagonist**. The wiki's admin note:

- Don't kill crew unprovoked. If Security is helping you, attacking them earns an admin PM.
- You may do anything to **avoid capture**.
- If crew (e.g. Security) cooperate with the hunters, you may retaliate with force.
- Prisoners get "a bit more leeway" on escalation as enemies of Nanotrasen; that is still not a licence to attack bystanders.

Anyone hunting you, or helping the hunters, is fair game: use whatever force keeps you free. The general antagonist limits in `server-rules.md` (no metagaming, exploits, OOC in IC) also apply.

## 3. Getting around

No ID access: **hack** maintenance doors with the toolbox (screwdriver to open the panel, then pulse or cut wires). Stay in maintenance and low-traffic areas. Prepare before the hunters arrive at the 10-minute mark: hiding places, escape routes, weapons, allies.

## 4. Fugitive types

| Type | Count | Kit and notes |
|---|---|---|
| Prisoners | team | Escaped a Nanotrasen superjail. Shivs, and a determined moodlet (always in a good mood). Extra escalation leeway. |
| Synths | team | Freed synths, hunted. Luminous eyes; the leader has an implanter and random cybernetic implants. Flavour says you sense other silicons and could free them. |
| The Invisible Man | solo | Toggleable cloaking implant (slightly stronger than a ninja's) and several stabilized Saturn X injectors: fully invisible for 10 minutes each, **only while wearing nothing**. |
| Waldo | solo | Unremovable striped outfit (you are conspicuous) and the **knock** spell to open doors. |

## 5. Outcomes

| Result | When |
|---|---|
| Major Fugitive Victory | All fugitives survived uncaptured. |
| Fugitive Victory | A fugitive survived, no bodies recovered by the hunters. |
| Minor Fugitive Victory | All fugitives died, none recovered. |
| Stalemate | Everyone died, no fugitives recovered. |
| Minor Security Victory | All hunters died, but they captured a fugitive (dead or alive). |
| Security Victory | Hunters captured a fugitive. |
| Major Security Victory | Hunters captured every fugitive. |
| Badass Security Victory | Every fugitive captured alive. |
| Postmortem Security Victory | Every fugitive captured, all dead. |

Dying is better than being recovered: keep your body out of hunter hands.

## 6. Tactics

- Stay together as a team; split only with a plan.
- Make friends with the crew: the station may side with either party. Being polite and harmless makes Security less likely to help the hunters.
- Hunters have a **Bounty Locator** on their shuttle that reveals one fugitive's location; keep moving.
- Watch for bounty-hunter traps: they only trigger on fugitives and broadcast your position.
- Invisible Man: strip before injecting Saturn X; track the 10-minute timer.

## 7. Common mistakes

| Mistake | Fix |
|---|---|
| Attacking crew who are helping or ignoring you | Only fight those who hunt you or side with the hunters. |
| Wasting the first 10 minutes | Hack routes and find a hideout before the hunters land. |
| Dying where hunters can drag your body off | Die (if you must) somewhere unreachable; a recovered body counts as a capture. |
| Saturn X while clothed | It only hides you naked. |

## 8. Recognising fugitives (crew)

Strangers in maintenance with no ID and a toolbox, a man in an unremovable striped outfit, synths with glowing eyes, shiv-carrying prisoners. They are not automatically hostile: Rule 4 says crew need cause to hinder antagonists. You may help either side with IC reason.

## 9. Through the client

- `look` / `search` to find doors and hiding spots; hacking opens a wire panel window (`tgui_window`, `tgui_act`), read it first.
- `inventory` before every `click`; a screwdriver in hand on a door opens its panel.
- Spells and implants show as actions or verbs: `verbs`, `call_verb`.
- Talk to your team with `say` (no special radio is given); `whisper` to stay quiet.

## 10. Checklist

- [ ] Rules read: no unprovoked crew kills.
- [ ] Type and kit checked.
- [ ] Routes hacked, hideout chosen before the 10-minute mark.
- [ ] Team together; crew friendly where possible.
- [ ] Alive and uncaptured at round end.

## Sources

The /tg/station 13 wiki, "Fugitive" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_fugitive.txt. Not checked against the server's code. Original PR: tgstation #42554. The hacking steps in section 3 are general game knowledge, not from the page.
