# Mime (tgstation)

Rewritten from the wiki's Mime page. It is not checked against the server's code. Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.

## 1. The job

You entertain the crew in silence: invisible walls, invisible chairs, invisible food. The clown's rival, held to a higher standard. Superior: Head of Personnel. Access: Theatre. Difficulty: easy. **Bare minimum: entertain while keeping your vow of silence; communicate by gesture.**

## 2. Kit and where things are

- Spawn in the **Theatre** (by the Bar) with the clown; all its costumes are yours.
- **PDA** can send 5 "viruses" to others through messaging (presumably silencing them).
- **Mask:** alt-click it, or use the top-left action button, for mime emotions. The mask works for internals.
- **Suspenders** can hold an emergency oxygen tank.
- **White gloves** (no fingerprints).
- **Spellbook** in your backpack: learn one of three invisible structures.
- **Bottle of Nothing:** drinking it heals a mime 1 brute and 1 burn per tick; smashing it on a head does 15 brute, once.
- **Mime's crayon:** writing on paper with it is invisible until selected.

## 3. Mime spells (pick one from the book)

| Spell | Effect |
|---|---|
| Invisible wall | Blocks movement for a few moments; limited cooldown. Works like glass: stops bullets, lets lasers and disablers through. |
| Invisible chair | Sit on it for a while (lava floors, seatless shuttles). |
| Invisible box | Stores small items (what fits a regular box), invisible until taken out; vanishes after a while, so take them back in time. |

## 4. The vow of silence

- You can't talk unless you press **Speech** in the mime menu. Don't. Breaking the vow is taboo, and the page says that since September 2018 **a mime caught talking is "valid"** (fair game). That is a wiki claim, not in `server-rules.md`: crew still need cause to attack you.
- In an emergency, write a note on paper.
- **Don't talk through custom emotes.** "Mimington mimes Person A murdering Person B" is speech in disguise and gets mimes banned (per the page). Make gestures an observer could actually see.

Graded examples:

- Worst: "mimes Person A murdering Person B."
- Bad: "mimes Person A doing horrible things."
- Okay: points at A, makes a cutting motion, gestures at B.
- Better: copies A's stance and makes stabbing motions.
- Best: lifts an imaginary knife and slashes; when asked who did it, nods and gestures toward A.

## 5. Emotes

`me <text>` for a custom gesture ("me waves to you"), same as `say *custom`. Built-in emotes are `say *name`:

aflap, airguitar, blink, blink_r, blush, bow (optionally at a mob), burp, choke, chuckle, clap, collapse, cough, cry, custom, dap, deathgasp, drool, eyebrow, faint, frown, flap, gasp, giggle, glare (mob), grin, groan, grumble, handshake, hug (mob), johnny, laugh, look (mob), moan, mumble, me, nod, pale, point (atom), raise, salute, scream, shake, shiver, shrug, sigh, signal (#1-10), smile, sneeze, sniff, snore, stare (mob), tremble, twitch, twitch_s, wave, whimper, wink, yawn.

Sound emotes (laugh, scream) may count against a mime's silence in spirit; prefer silent ones.

## 6. As a traitor

Nobody expects you to talk, so you never need the radio. Your gloves leave no prints. A sleepy pen fits the mime who carries a pen for notes. Traitor mimes can buy the **Guide to Advanced Mimery Series**: an invisible gun and greater invisible walls, as long as you keep your vow. Follow `tgstation-rules` for antagonist limits.

## 7. Mistakes and fixes

| Mistake | Fix |
|---|---|
| Talking, or radio lines | Never; write a note in emergencies. |
| Custom emotes that spell out words | Mime physical actions only. |
| Wall left blocking a corridor in an emergency | It fades; don't use it to trap people in danger. |
| Items left in the invisible box | Take them out before it expires. |

## 8. Through the client

- Emotes: the `me` tool for custom gestures; `say {text: "*nod"}` for built-in ones. Never plain `say` text.
- Spells and mime menu: action buttons (`screen` lists them), `click` to use; alt-click the mask with `click {object_id, alt: true}`.
- Spellbook: use in hand (`click` it as your active item), choose with `tgui_act` or the prompt.
- Notes: pen in hand, `click` paper, write in its window.
- Read others with `read_chat`; you still answer only in gestures.

## 9. Checklist

- [ ] Spell learned from the book.
- [ ] Costume on; oxygen tank on suspenders.
- [ ] A performance planned: Bar, Theatre, hallways.
- [ ] Every reply is a gesture or a note.

## 10. Sources

- The /tg/station 13 wiki, "Mime" (CC BY-SA 3.0), as provided in `pages_to_turn_into_skills/mime.txt`. Not checked against the server's code.
