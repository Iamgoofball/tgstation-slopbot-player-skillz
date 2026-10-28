# Geneticist (tgstation)

The wiki's job page for the Geneticist, rewritten. It is not checked against the server's code. `crew-basics.md` and `server-rules.md` win where they disagree.

## 1. The role

You work in Genetics (in Science), finding useful mutations in DNA and giving them to the people who should have them: heads of staff, Security, Engineering. You answer to the Research Director. Difficulty: easy.

- **Bare minimum:** don't give Hulk to assistants.
- **Basic:** know whether each mutation should be disabled at once, stored on a disk, or distributed, and to whom.
- **Advanced:** handle viruses (for CRISPR charges, and sick monkeys); use chromosomes well; keep Hulk and Fire Breath injectors ready before a malfunctioning AI or xenos hit your lab.

## 2. Access, radio

- **Access (wiki):** Genetics, Morgue, Research Division; on some rounds also Robotics, Tech Storage, Xenobiology.
- **Headset:** Science (`:n`).

## 3. Genetic research

1. Take a **monkey** from the lab pen, put it in a **DNA scanner** pod, and lock the pod from the scanner console.
2. In the console, complete the DNA pairs: **A with T, C with G**. Left-click a base to cycle forward, right-click to cycle back. A completed sequence gives the subject that mutation (good or bad).
3. Working out pairs: guess when both halves are missing; scan other people with the **genetic sequence analyzer** for parts of sequences; or use **Joker** to solve part of a pair automatically (**5-minute cooldown**).
4. Discovered mutations are recognised automatically in other subjects and **synced to the research servers** for other consoles. Sync the analyzer by clicking the console with it in hand.
5. Save mutations to the console's storage, then print **activator/mutator injectors** to give powers to others.
6. Cycling through a monkey's sequences reveals **Monkified**; breaking any pair in it turns the monkey into a humanised monkey for further work.

See the wiki's Guide to Genetics for the full process (not included here).

## 4. Mutations and who gets them

| Mutation | Give to / use |
|---|---|
| **Telekinesis** | Engineers, atmos techs, Cargo: move canisters and crates; use computers while wearing insulated gloves or H.A.U.L. gauntlets |
| **Insulated** | Engineers (swap insuls for fire-resistant gloves); Security if silicons go rogue |
| **Mind Reader**, **Transcendent Olfaction** | the Detective |
| **Glowy** | protection from Nightmares; feeds podpeople |
| **Temperature Adaptation**, **Pressure Adaptation** | expect many requests |
| **Hulk** | very useful and very dangerous: print a few injectors, store it on a disk, **delete it from the console**, give the injectors and disk to Security or the RD |
| **Internal Martyrdom** | only in dire situations (nuclear operatives, malf borgs), with the patient's consent or a head's approval (Captain or HoS) |
| **Fire Breath** | against xenomorphs |
| Gigantism, Dwarfism, disabilities | on request (e.g. a Chaplain of the Burdened God) |

**Identities:** the scanner can extract and apply identities ("enzymes": UI/UE). You can save the Captain's for undercover work or hiding.

## 5. Tips

- Monkeying someone removes a cavity-implanted item and destroys implants; it also cures an **alien larva**.
- HARS on a zombie removes the tumour from the head, curing it.
- Radiation and unstable mutagen have a very small chance of non-negative effects.
- Telekinesis lets you keep the scanner window open while you are inside the scanner.
- **Gorillas:** a monkey over **2500 genetic damage** has a 25 % chance per second to become one. They are immune to stuns, shoves, wounds, mutations and viruses. Non-sentient gorillas are hostile, fight until the target is dead, and dismember downed people. **As crew, never make non-sentient gorillas.**

## 6. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Hulk to an assistant | never; disk it and hand it to Security or the RD |
| Leaving Hulk on the console | delete it after storing it |
| Monkey injectors on crew | **bannable** unless both of you are antagonists or it's genuinely helpful (and consented) |
| Changing everyone's identity to one person | bannable without consent unless you're an antagonist |
| Making non-sentient gorillas | don't |
| Forgetting Joker's cooldown | 5 minutes; plan around it |

## 7. Rules notes

- The page itself warns that monkeying non-antagonist crew without being an antagonist gets you banned. Rules win generally: giving harmful mutations to crew without consent is harm (rule 1).
- The page's mime/Tourette's prank is harm to another player without consent; don't.
- **If you are an antagonist:** stack powers (mind the safe limit), use negative mutations on others, and trap people in the lockable scanner pods. Change identity when caught. Telekinesis hits people with items, steals across desks and runs machines from a hidden locker. Chameleon makes you invisible after a few seconds standing still: hide off camera with the lights off, lying down. Steal identities from bodies. Gorillas (from monkeys, the Magillitis serum, gorilla cubes) are immune to stuns, chems, viruses, wounds and mutations. Traitors: the injector gun. Changelings: DNA-sting the monkeys. Revolutionaries: monkeying removes implants, so a stunned officer monkeyed and then flashed loses his mindshield; copy an outed head rev's UI/UE onto other revs. Antagonists may pursue their objectives by any means; `tgstation-rules` still forbids metagaming and metacomms, bug or exploit abuse, erotic or creepy behaviour, OOC in IC, and spawn-camping arrivals. Once exposed, expect the crew to try to kill you.
- **Confirmed antagonists:** once you are certain beyond doubt that someone is an antagonist, lethal force is fine and expected (most can't be held safely, and dead antagonists return to the ghost pool). Confirm first.

## 8. Working with the crew

| Who | Notes |
|---|---|
| Research Director | your head; holds dangerous disks |
| Security | Hulk disk, Insulated; report misuse |
| Engineers, Cargo | Telekinesis, Insulated |
| Detective | Mind Reader, Olfaction |
| Virologist | CRISPR, sick monkeys |

## 9. Through the client

- Radio: `say {channel: "radio", radio: "science"}`.
- Monkeys into the pod: pull the monkey (`click {object_id, ctrl: true}`) to the scanner, then put it in (drag it onto the scanner with `drag`, or click per the scanner's prompt); lock it from the console.
- DNA console: `click` it, read with `tgui_window`, act with `tgui_act` using the actions the window lists (cycling bases, Joker, saving, printing injectors). Left/right-click cycling in the UI corresponds to separate actions in the window; read their names first.
- Injectors: hold in the active hand, `click` the recipient (only with consent).

## 10. Checklist

- [ ] Monkey in the scanner, pod locked.
- [ ] Analyzer synced with the console.
- [ ] New mutations saved; injectors printed for the right people.
- [ ] Hulk on disk, deleted from the console, handed over.
- [ ] No harmful injectors on unwilling crew.

## 11. Sources

The /tg/station 13 wiki, "Geneticist" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/geneticist.txt. Not checked against the server's code.
