# Paradox Clone (tgstation)

Rewritten from the wiki's Paradox Clone page. It is not checked against the server's code. Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.

## 1. The role

A mid-round antagonist picked from ghosts who sign up. The game copies a random crew member: you spawn somewhere on the station with their **exact appearance, quirks, DNA, starting clothes and ID**, so you have their job's access. That can include jobs normally barred from antagonist roles (Security, Detective). Your one objective: **kill the original and live as them for the rest of the round**, ideally undetected. No gadgets, powers or backup. Difficulty: hard. You are a lone antagonist.

## 2. Kit

- Your target's clothes and ID as they were at shift start.
- A **mechanical toolbox**, so you can get out of maintenance if the ID lacks maintenance access.
- **Memories** (IC tab) gives your bank account ID. Alt-click your ID card to link it to the original's bank account and use their credits.

## 3. Tactics

- **Once exposed, expect the crew to try to kill you.** Confirmed antagonists are fair game for lethal force; plan your escape before you are seen.
- Don't let the original see you early.
- Copy their speech: how they talk on the radio, their phrases, their job habits. Read your copied job's skill so you can do the job convincingly afterwards.
- Watch for changes in their look (new clothes, hair); if they change and you don't, you stand out.
- **Quiet route:** ambush them somewhere out of the way, kill, hide the body, take their place.
- **Loud route:** attack them openly and shout that *they* are the clone.
- **Framing:** if they're hard to reach and Security is aggressive, frame them for a capital crime and let Security do it.
- **Lures:** a paramedic or eager doctor will come to a suit sensor; put a jumpsuit with sensors on a mutilated monkey (or monkey-human) and wait where it pings.
- **Weapons:** makeshift weapons (spears, stunprods) from parts found in maintenance.
- **Genetics:** a swarm of monkey-human copies of you makes it very hard to find the real you (doesn't kill the target).
- **Plan B:** ordnance. A bomb leaves nothing for Security to identify.
- Most changeling tips (impersonation, body disposal) apply to you.

## 4. Limits that still apply

- Lone antagonist (`server-rules.md` section 4): any means toward your objective, except metagaming or metacomms, bug or exploit abuse, erotic or creepy behaviour, OOC in IC, spawn-camping arrivals.
- Don't use OOC knowledge of your target (their real habits from other rounds); learn them IC.

## 5. For the crew

- Two identical people with the same ID: one is a clone. Ask things only the original would know from this shift.
- The clone wears the **starting** outfit; the original may have changed since.
- A clone carries a mechanical toolbox it spawned with.
- "They're the clone!" is exactly what a clone would shout; detain both and sort it out. Once you're certain which one is the clone, lethal force is fine.

## 6. Through the client

- `look` and `examine` the target to learn their name, job, outfit; `read_chat` to learn how they talk.
- Memories: `verbs` or the stat panel's IC tab; `call_verb` the Memories verb if listed.
- Link the bank account: `click {object_id, alt: true}` on your ID card, then answer the prompt with the account number.
- Speak as them: `say` with their style; their department radio key (`:h` uses your headset's channel).

## 7. Checklist

- [ ] Memories read; bank account linked.
- [ ] Target located without being seen; their speech and look noted.
- [ ] Weapon or plan ready; isolated spot or frame set up.
- [ ] Target dead and body hidden; you resume their job and routine.
- [ ] Keep your look matching theirs.

## 8. Sources

- The /tg/station 13 wiki, "Paradox Clone" (CC BY-SA 3.0), as provided in `pages_to_turn_into_skills/antag_paradox_clone.txt`. Not checked against the server's code.
