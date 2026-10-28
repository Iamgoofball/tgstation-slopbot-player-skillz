# Lawyer (tgstation)

Rewritten from the wiki's Lawyer page. It is not checked against the server's code. Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.

## 1. The job

You give the crew legal aid: you advise on Space Law, defend prisoners, push for fair sentences, write contracts, and chase health-and-safety violations. Superior: **Head of Personnel** (not the HoS). Access: Law Office, Courtroom, Brig. Difficulty: easy. **Bare minimum: talk to prisoners and speak to Security for them when asked; urge the Warden to cut overly harsh sentences; represent crew who need it.**

## 2. Kit and radio

- Blue or purple suit, brown shoes, a **briefcase** with 6 sheets of paper and a pen, a PDA, a box.
- **Law and Order headset:** Security (`:s`) and Service (`:v`). Don't abuse the Security channel; Security will take the headset, or arrest you and take it.
- Start in the Law Office. The briefcase holds a toolbox's worth of items.

## 3. Duties

- **Consult on the law.** Be there when people are jailed: give the correct time, explain each crime's sentence and the total. Argue mitigation (clowning, insanity) but don't push it.
- **Establish guilt or innocence.** Hear the officers' stories; point out the wrong person or a lesser crime. Ask the Detective for forensic scans to back your client (any suspect brought in).
- **Get inmates medical care.** Officers go back on patrol; keep their prisoners healthy.
- **Keep the Brig clean.** You'll be there a lot and it gets messy.
- **Release inmates.** When time is up, bring their belongings (often in the evidence room), see them out, and make sure the Warden or HoS sets their record to "Released".
- **Trials.** Rare: usually for prisoners facing execution, or when the HoS agrees. High-profile defendants (wizards) happen.
- **Contracts.** The fastest way to get things done: e.g. both parties agree to trade helmets. Write them with paper markdown, sign and stamp.
- **Confirmed antagonists** may lawfully be killed by the crew once there is no doubt; don't obstruct that or demand a trial. Your work is for suspects and ordinary criminals.
- **Litigation:** health, safety and rights violations; expect resistance.
- Nothing to do? Fetch tools from Tool Storage and redecorate the office.

## 4. Working with Security and the heads

- Win Security over: greet them, call them "officer", say please and thank you. Don't imply authority you don't have.
- **Never attack Security**, even when they deserve it; fleeing is fine. They'll remember.
- Make clear you serve justice, your clients and the station.
- **HoS:** befriending them fixes most trouble with officers in one PDA message. (The page suggests backing the HoS even in illegal actions and calls corruption "a tool of power": that's roleplay colour, not a duty.)
- **HoP:** your boss and the easiest ally; report Security misconduct to them.
- **Captain:** the top authority, hard to reach; go through the HoP first.
- **Fax machine:** sends paper to other faxes or to Nanotrasen (admins). For a reply, make it neat, signed, stamped and interesting. Last resort over the Captain's head, or for roleplay.

## 5. As an antagonist

- **Traitor:** you're close to Security: officers alone in the break room are vulnerable; the briefcase hides handcuffs and flashbangs from Security storage less suspiciously than a toolbox; the Security channel gives intel. Contracts with death clauses keep victims quiet, and a signed contract in your bag may make Security treat a killing as business. Other gimmicks: loan shark who collects by force, entrapment, a mob boss with underlings carrying "legal immunity" forms.
- **Revolutionary:** your brig access lets you drag revs out; you'll be mindshielded fast, so act early. Screwdriver the encryption key out of your headset and give it to a rev head for the Security channel.
- Follow `tgstation-rules` for antagonist limits. These gimmicks are antagonist-only; as plain crew, contracts don't authorise harm.

## 6. Mistakes and fixes

| Mistake | Fix |
|---|---|
| Acting as if you outrank officers | You don't. Ask, advise, appeal to the HoP or HoS. |
| Spamming the Security channel | Use it only for your clients' cases. |
| Fighting an officer | Never; flee and report to the HoP or adminhelp if it's a rule problem. |
| Wrong sentence totals | Check Space Law (crew-basics section 6) before quoting time. |
| Forgetting release paperwork | Record set to "Released" every time. |

## 7. Through the client

- Radio: `say {text, radio: "security"}` or the `:s` prefix; Service `:v`.
- Paper and contracts: pen in active hand, `click` the paper, write in its window; stamp by `click`ing the paper with a stamp in hand.
- Fax: `click` the machine with the paper in hand, then pick the destination in `tgui_window`/`tgui_act`.
- Records: ask the Warden or HoS; you can't edit Security records yourself.
- Find clients: `walk_to` the Brig; `look` for cells and timers.

## 8. Checklist

- [ ] Briefcase, paper and pen; headset checked (`:s`, `:v`).
- [ ] Greet Security; tell the Warden you're available.
- [ ] Each arrest: crimes, sentence, total time, mitigation.
- [ ] Inmates healthy; brig clean.
- [ ] Each release: belongings returned, record "Released".

## 9. Sources

- The /tg/station 13 wiki, "Lawyer" (CC BY-SA 3.0), as provided in `pages_to_turn_into_skills/lawyer.txt`. Not checked against the server's code.
