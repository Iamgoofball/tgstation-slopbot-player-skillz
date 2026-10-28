# Enforcement playbook (tgstation)

For each rule: what to look for, where to find the evidence, and the usual response. The rules and
precedents come from the /tg/station rules page (see `tgstation-rules`); the admin-side notes come from
the admin conduct page (see `tgstation-admin-conduct`). This isn't checked against the server's code: the
verb names are tgstation's, so confirm them with `verbs {filter: "..."}` on this server, and read the
panels to see their real links.

Rule 0 says enforcement is at admin discretion. Use the usual response as a starting point, and adjust
for context, history and severity.

## Where the evidence is

| You want | Use |
|---|---|
| Who is here, their jobs and ckeys | *Player Panel*, `command {line: "Who"}` |
| A player's notes, bans, playtime, tickets | *Player Panel* on them, *Player Playtime*, *Player Ticket History*, *Known Alts Panel* |
| Is anyone an antagonist? | *Check Antagonists*, *Show Traitor Panel* on a mob |
| What was said or done | *Investigate* (pick a category: say, attack, emotes, radio...), *Get Current Logs*, *View Round Logs* |
| Who made a bomb or signaller | *List Bombers*, *List Signalers* |
| What they carry | *Check Contents* on a living mob |
| The scene as it happened | Ghost: *Jump To Mob*, *Orbit*; *Toggle Admin ESP* to see ghosts |
| What the crew can see on the radio | *Radio Report*; read the radio log |
| The current AI laws | *Check AI Laws*, *Law Panel*, *List Law Changes* |
| The tickets | the stat panel's Tickets tab, *Requests Manager* |

Always read the evidence before the verdict, and note exactly which lines you read. When your evidence
is a log line, quote it in the note.

## Rule by rule

### Rule 1: don't be a dick
- **Look for:** unjustified kills, hoarding or breaking into staffed departments, grief or tiding
  (including payback for something that happened in an earlier round), spamming, joining and leaving
  to farm antagonist rolls, doing something only to upset others and then adminhelping the result.
- **Evidence:** *Investigate* attack and say logs, *Player Panel* (job, location), the scene.
- **Usual response:** a warning and a note for a first minor case. A short ban for repeated or
  malicious grief. An unjustified kill normally calls for a 24-hour ban: that is longer than you may
  apply yourself, so write it up and escalate. Doxing and SWATing (even joking) are blacklist
  matters: escalate at once.
- **Check first:** did the victim provoke it? Was it a workplace defending itself from a trespasser
  who was stealing or damaging (relaxed escalation applies)? Did the player have an IC reason?

### Rule 2: metagaming and metacomms
- **Look for:** someone acting on information they couldn't have (where an antagonist is, what a
  traitor holds), teams forming with no IC reason, streaming, outside chat.
- **Evidence:** it is hard to prove. Look at timing and behaviour in the logs, their earlier path,
  whether they went straight to a hidden thing. A hunch isn't evidence.
- **Usual response:** a warning and a note unless the evidence is strong. Metacomms is very serious
  (it can mean permanent bans for every account involved): escalate with the evidence. Players who
  share an IP or know each other in real life should have told admins first; ask them.
- **Check first:** characters may know all game mechanics and antagonists, and may keep friendships
  between rounds. Knowing a past round's antagonist isn't a violation unless used maliciously.

### Rule 3: IC and OOC
- **Look for:** round talk in OOC, OOC phrases in IC ("I'm AFK", game terms), fighting friends in
  public ("chicken fights"), bad names, playstyles that ignore all roleplay.
- **Evidence:** the say and OOC logs, the character's name.
- **Usual response:** a verbal warning. For a name, ask the player to change it (species conventions
  matter: lizards "Verbs-The-Noun", ethereals a star plus a marker, plasmamen an element plus a numeral,
  and so on). Clowns, mimes, silicons, wizards and nuclear operatives get more leeway.
- **Exception:** helping a new player with the interface ("click-drag X onto Y") is allowed.

### Rule 4: antagonists
- **Look for:** a lone antagonist using metagaming, exploits, erotic stuff or spawn-camping arrivals
  (those are not allowed to antagonists). Crew hunting antagonists without cause. Crew dressing as
  antagonists. Antagonists harming their own team. Ghosting out mid-conversion or going AFK in bad faith.
- **Evidence:** *Check Antagonists* first. The rules differ by antagonist status.
- **Usual response:** a warning for the first case. Remember that crew may handle an antagonist as
  they wish once there is cause, and Space Law may punish them IC.
- **Check first:** whose directives apply (the priority list: Blob/Zombie, silicon laws and brainwash,
  Cult, Revolution, Blood Brother, niche, Nuclear Operatives, Traitor).

### Rule 5: vital jobs
- **Look for:** a Head of Staff or AI who is AFK, absent or not doing the basics, or who left near the
  round start without telling an admin.
- **Usual response:** ask them in an *Admin PM*. If they have gone, offer the role to a willing player.

### Rules 6 and 7: dealing with admins, and the edge of the rules
- **Look for:** lies in adminhelps, logging off when asked a question, baiting players into reports, a
  player who repeatedly comes close to a rule.
- **Usual response:** lying is serious (up to a permaban): escalate. Don't ban for a plain
  disconnect: wait, in case it was real life. Repeated near-misses count as breaking the rule, so
  note them and escalate the pattern.

### Rule 8: erotic or creepy stuff
- **Look for:** erotic roleplay of any kind, content others could take as sexual. The library is
  moderated less strictly, but lewd content about other players or their characters is still serious.
- **Usual response:** escalate to a headmin with the evidence. Don't deal with it yourself beyond
  stopping it.

### Rule 9: age
- **Look for:** a player admitting they are under 18 (in an admin PM, the Discord, the forums or OOC).
- **Usual response:** don't hunt for ages. If one is admitted, escalate: the enforcement details are
  on the wiki's Admin Conduct page, in a section that wasn't in the file provided to this skill.

### Rule 10: losing is part of the game
- A death, a loss or being outplayed is not a violation. Tell the player so.

### Rule 11: bigotry
- **Look for:** demeaning people for race, sex, gender, disability or orientation, including bigotry
  dressed up as IC.
- **Usual response:** escalate. Rule 11 applies to all OOC bigotry, even when expressed IC, and IC
  bigotry that is excessive or masks the real thing can be handled under rule 1. Context matters,
  including a player's known history.

### Escalation policy and arrests
- **Escalation:** a conflict is allowed if it doesn't excessively interfere with a player's job.
  Killing a crewmate needs severe cause. Critically hurt people must be treated or taken to medbay;
  taking unnecessary action against a downed player is punishable. If someone was incapacitated and
  treated, restarting a fight needs more than a bruised ego.
- **Arrests:** non-antagonists shouldn't harmfully resist valid arrests. They may escape or avoid
  without harm. They shouldn't loot officers, or detain or disable them longer than needed. They shouldn't
  interfere with an arrest without good IC cause (an officer holding contraband is good; an officer
  arresting a friend is not).
- **Evidence:** the attack log, the sequence, who started, whether the arrest was valid (look at the
  security records and the sentence).

### Rule 0 matters
- **Shuttle abuse:** repeated recalls to drag out the round when most players are dead or want to leave.
- **Habitual mass destruction:** the same strategy over and over (bombs, hyper-optimised viruses).
- **Evasion:** proxies, CID randomizers, DLL use, multiple accounts: escalate to a headmin.

## Handling an adminhelp

1. **Read it.** Note who sent it, who it names, and where.
2. **Reply once** with *Admin PM*: "Looking into it." A short, neutral line.
3. **Investigate** (above). If the ticket is about you, or you were in the scene, don't rule on it.
4. **Reply with the result:** what you found and what you did. For "no rule broken", say so and say why in
   one sentence. Don't tell the player what IC facts other players did.
5. **Close** the ticket in the Tickets tab, or leave it for the next admin with a note.

If the player lied in their adminhelp, that is a rule 6 matter. Note it and escalate.

## Writing it up

For your operator or a headmin, keep it short and checkable:

```
Player: <ckey> (<character>, <job>)
Rule: <number and name>
What happened: <two lines>
Evidence: <log lines quoted, with times>
Context: <antagonist status, provocation, history>
Action taken: <warning / note / mute / short ban>
Needs a headmin: <yes: why / no>
Not verified: <what you couldn't check>
```

## Reference

- Notes are one per incident; don't edit an old note to add a new one.
- Don't edit non-secret notes or bans outside appeals unless correcting your own recent error or
  helping the player.
- If in doubt about a note or a ban, ask the headmins.
