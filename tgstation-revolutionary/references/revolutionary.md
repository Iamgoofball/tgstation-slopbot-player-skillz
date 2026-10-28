# Revolutionary (tgstation)

Rewritten from the wiki's Revolutionary page. It is not checked against the server's code. Where it disagrees with `crew-basics.md` or `server-rules.md`, those win; section 7 lists the limits that still apply.

## 1. The round in one paragraph

Revolution is a Dynamic ruleset. A few crew start as **Head Revolutionaries**; they convert others with **flashes**. The revs win when every head of staff (Captain, Head of Security, Head of Personnel, Chief Engineer, Chief Medical Officer, Research Director, Quartermaster, latejoined heads included) is dead, turned into an MMI or cyborg, or exiled. The station wins when every Head Revolutionary is dead or exiled. **The shuttle can be called but won't leave; the round doesn't end until one side wins.** Leaving the station's Z-level, or hiding in a locker or crate, counts as exiled ("abandoned the station"), which lets either side remove a target without killing.

Revs are a **team antagonist** (`server-rules.md` section 4): don't harm the team's work, and conversion goals rank above traitor or nuclear ones.

## 2. Head Revolutionary

- **Flash people to convert them.** As a rev head you can flash from behind. Sunglasses or welding masks block it: remove them first. You **cannot convert** Security, anyone mindshielded, heads of staff, or the permanently blind.
- **Once exposed, expect the crew to try to kill you.** Confirmed antagonists are fair game for lethal force; plan your escape before you are seen.
- **Stay low.** Your death loses the round for the revs. Let converts do the fighting, keep your identity hidden, and only mix with non-revs to flash them. If spotted, run and change your look.
- **Don't hide forever.** Making yourself an impossible target (sealed away, off station) is poor form; admins frown on it, and leaving the Z-level exiles you.
- **Priority converts:**
  - Roboticists: Robotics makes replacement flashes and mechs.
  - Geneticists: superpowers; they can save a killed head's UI/UE and make you look like them (minus the mindshield).
  - Scientists: research and weapons.
  - Cargo Technicians: a base, and orders for flashes and weapons with the right access.
  - A rev Botanist with a syringe of your blood can grow you back in a replica pod.
- Converted Lawyers can screwdriver the encryption key out of their headset and give it to you for the Security channel.

## 3. Converted revolutionary

- You were flashed: you are now a rev. Kill or exile heads without getting caught, and **keep the Head Revolutionaries alive**. Killing one head is a full contribution.
- Use your job: mechs as a roboticist, hulk from genetics, guns ordered through cargo. Makeshift weapons are fine.
- Once you're confirmed as a rev, expect lethal force; some officers will deconvert instead (mindshield implant, a hard knock to the head).

## 4. Heads of staff and Security

- **On the first credible evidence** (not the clown shouting), get somewhere safe, likely the Brig.
- **Open the mindshield implant cases.** One in the Armory, one in the Head of Security's locker, four implants each. Ask the Quartermaster on Command radio to order more at once.
- **Implant order:** Cargo (protects the implant supply), Medical (keeps officers alive), Lawyers (keeps the brig clean of revs), Science (stops mechs, maxcaps, golems, slimes, hulks). After that, the most suspicious and aggressive people.
- **A deconversion** shows "X looks as if they've remembered their true allegiance!" Ask them at once who flashed them: that's a rev head. Repeat.
- **A hard knock to the head** (a toolbox) can deconvert. Don't club everyone on suspicion: brig suspects until you can implant. **Once someone is confirmed beyond doubt as a rev (seen flashing, attacking heads, showing the rev icon to a deconvert's account), lethal force is fine**; a confirmed Head Revolutionary should be killed, since their death is how the station wins. If someone was knocked out several times and didn't turn, get them healed, apologise and note it in security records.
- **Don't hide** in a closet or leave it to the AI. Hiding as a head is poor form, just like for rev heads.

## 5. Ordinary crew

- Treat it like any traitor round: if someone is beating a head to death, stop them or call Security.
- Heads and Security are on edge. If you aren't mindshielded, keep your distance, don't startle them, and **accept any mindshield request**.

## 6. When it ends

**If the Head Revolutionaries lose:**
- Converts lose antagonist status at once and **must stop acting as antagonists**. The red rev HUD icon disappears and CentCom announces the defeat. Harm after that point gets you banned: watch for it.
- Exiled rev heads become **Enemies of the State**, with a choice: survive in exile, or try to hijack the shuttle.
- The shuttle becomes available again (it showed "UNAVAILABLE", "ERR --:--").

**If the heads lose:** the round ends.

## 7. Limits that still apply

- Revs are a team antagonist (`server-rules.md` section 4): use any means toward the goal, but don't harm the team's work, directly or by idling. Converted players must not ghost, suicide or log off in bad faith.
- Lone-antagonist limits apply too: no metagaming, exploits, OOC in IC.
- After CentCom announces the revs' defeat, converts are no longer antagonists: stop.
- Heads and Security are **not** antagonists. They may kill confirmed revs, but suspicion alone still falls under escalation (`server-rules.md` section 5). The page's struck-through surrender advice and its joke about causing a supermatter delamination as a head are not allowed for crew.

## 8. Through the client

- **Flashing:** hold the flash in your active hand and `click` the target (from behind works for rev heads). Check `examine` or `look` for sunglasses first.
- **Who is a rev:** the HUD icons (`screen` or `look` on people) show rev and rev head marks to fellow revs.
- **Mindshields (Security):** an implanter case is a container; take an implanter and `click` the person with it in hand while they're restrained.
- **Radio:** Command `:c` for heads; Security `:s`; Common `;`. Revs coordinate face to face or on a channel the heads can't hear, never in OOC.
- Watch `read_chat` for the CentCom announcement that the revolution failed, and stop at once if it appears.

## 9. Checklist

**Rev head**
- [ ] Flash in hand; target has no eye protection; nobody watching.
- [ ] Convert Robotics, Genetics, Science, Cargo first.
- [ ] Stay low; keep converts between you and Security.
- [ ] Don't leave the station's Z-level or seal yourself away.

**Head of staff**
- [ ] Safe place; mindshield cases opened; more ordered.
- [ ] Implant Cargo, Medical, Lawyers, Science, then suspects.
- [ ] Every deconvert: ask who flashed them.

**Everyone**
- [ ] After a rev defeat announcement, stop all antagonist behaviour.

## 10. Sources

- The /tg/station 13 wiki, "Revolution" (CC BY-SA 3.0), as provided in `pages_to_turn_into_skills/antag_revolutionary.txt`. Not checked against the server's code.
