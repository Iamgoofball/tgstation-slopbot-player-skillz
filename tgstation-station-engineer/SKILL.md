---
name: tgstation-station-engineer
description: Play the Station Engineer on tgstation (MetaStation): the Supermatter engine, emitters, tesla coils, SMES units, the power grid, telecomms, APCs, solars and repairs. Use it when your job is Station Engineer or a task involves power, the engine or fixing the station.
---

# Station Engineer

The job guide for the Station Engineer (two variants: power and repairs).

Read [references/station-engineer.md](references/station-engineer.md) before you act on anything it covers. It is the full guide, and it lists the common mistakes and their fixes, so come back to it when something goes wrong.

## ENGINE WORK = CONSTANT VIGILANCE

Engineering is the job that can kill the whole station, so the checking habit is
not optional. After EVERY action (script, click, valve, emitter): read chat, your
status, and your surroundings — `run_script {script: ".../common/check.py"}` is
one cheap envelope for all three; `engineering/cims_read.py` reads the crystal.
A real delamination killed our engineer: integrity warnings and the 15 s
countdown were in chat for minutes while scripts were fired back-to-back blind.
When the supermatter starts eating integrity: `engineering/delam_response.py`
(beams off → panic siphon → N2 flood), then RUN — the countdown is 15 s and the
blast is ~37 tiles with O2 in the chamber. Multi-step scripts embed the watchdog
(scriptz README section 1); you must read what they return before firing the
next one. The reference's **4.1b** has the wiki guide's mechanics: the four
delam types (explosive / tesla >5 GeV / singularity >1800 mol / resonance
cascade), the 373 K plasma+O2 combustion limit, diode disks and emitter
kickstarts.

Related skills: `tgstation-client` (how the seeker tools work), `tgstation-crew-basics` (the game itself), `tgstation-rules` (what is allowed).
