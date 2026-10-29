---
name: tgstation-crew-basics
description: Life on a tgstation (MetaStation) crew: chain of command, departments and where they are, alert levels, the emergency shuttle, radio keys, doors and access, health and crit, combat and self-defence, hazards, death and revival, and everyday interactions through the seeker tools. Use it at the start of any shift, and whenever you are unsure how to talk, open a door, treat an injury, fight or flee, or what a hazard does.
---

# tgstation crew basics

What every crew member needs to know about the game before their role guide: the station, talking, access, health, fighting, hazards, death and the everyday actions people get wrong.

Read [references/crew-basics.md](references/crew-basics.md) before you act on anything it covers. It is the full guide, and it lists the common mistakes and their fixes, so come back to it when something goes wrong.

## STAY ALIVE: check chat, status and surroundings CONSTANTLY

Between actions — after every script, before every new area, at the first hint
of anything odd — look at three cheap things: recent chat, your status line, and
what's around you. Through the seeker tools this is one envelope:
`run_script {script: ".../common/check.py"}` → {chat_tail, you, around,
danger_words}. Danger you will only catch by looking: supermatter delamination
warnings and countdowns, gas floods and fires, people attacking you, an admin or
crew member telling you to stop, your own health collapsing. A character died to
an engine delamination purely because scripts were run back-to-back while blind.
Rules:
1. Never fire a world-affecting action while blind.
2. Multi-step scripts must embed a chat+status `watch()` between steps (scriptz
   README section 1) and the AGENT must read the returned chat/status and the
   surroundings after every script before planning the next one.
3. If anything is wrong — hurt, warned, something burning, a countdown — stop,
   fix or flee, and only then resume.

Related skills: `tgstation-client` (how the seeker tools work), `tgstation-crew-basics` (the game itself), `tgstation-rules` (what is allowed).
