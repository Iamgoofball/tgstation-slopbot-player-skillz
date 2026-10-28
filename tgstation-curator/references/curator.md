# Curator (tgstation)

Derived from the wiki's Curator page; not checked against the server's code. Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.

## 1. The role in one paragraph

You run the Library, in Service under the Head of Personnel. You stock the empty shelves from the station's persistent book archive, lend books, bind and upload new ones, replace the Chaplain's bible when it's lost, report station news on the newscaster and the broadcast camera, and, if you want, go adventuring with the kit from your heroic beacon. The book and painting databases persist between rounds and servers: you are the first and last defence against low-effort junk entering them. Difficulty: easy. Minimum: know how to write and publish books and how to use the library computer.

## 2. Kit, access and radio

- **Access:** Library private study, Construction, Mining Station. Construction access covers the Auxiliary Base Construction Area (meson scanners, a full toolbelt, a cargo headset) and the Vacant Office.
- **Radio:** Service, plus an **Entertainment** channel on your headset, off by default; it plays on every entertainment monitor.
- **Kit:** barcode scanner, bookbag (carries many books, like a mining satchel), pen and paper, tape recorder, camera with spare film, the **broadcast camera** (in your backpack; only one on the station), the **heroic beacon**.
- **Languages:** you understand and can speak cultspeak, robotic beeping, drone chatter and xenomorph.

## 3. Where things are

The Library has the check-in/out computers, the book binder (east back of the Library), shelves labelled Religious, Fiction, Adult, Reference and Forbidden Knowledge (back room), a newscaster behind the desk, a photocopier, and some canvases. Your private study has its own bookshelf.

## 4. Core procedures

### Stocking the shelves

The shelves start empty. On a check-in/out computer, choose **"4. Connect to External Archive"**, browse (unsorted, many duplicates; pick the good ones), and **ORDER** to print a bound copy. Shelve by category. Don't print dozens of one book: a big pile lags players who right-click it.

### The barcode scanner

Use it in hand to cycle modes, and use it **on the computer** after scanning a book.

| Mode | Effect |
|---|---|
| 0 | Scan book to local buffer |
| 1 | Scan, and set the computer's buffer to match |
| 2 | Scan, and try to check the book in |
| 3 | Scan, and try to add the book to the inventory |

Add printed books to inventory (mode 3), then lend them through the computer for a set time, like a real library.

### Publishing a book

1. Write on paper with a pen (the wiki's Paper Markdown page covers formatting).
2. Put the paper in the **book binder**; a book comes out.
3. With the pen, title it, sign it, add more.
4. Scan it with the barcode scanner, then on the computer choose **"5. Upload New Title to Archive"**, set category and author, review, and **UPLOAD**.

### Saving a painting

1. Get a canvas (some in the Library, or craft from cloth) and crayons or a spraycan (full RGB).
2. Holding the tool, click the canvas to paint. **Finish**, then title and optionally sign it.
3. Choose a collection: Public (most frames), Secure (behind glass), Private (your office or somewhere discreet). Not every station has all three.
4. Hang it in a **roundstart frame** (remove an existing painting with wirecutters if all are full). A frame you crafted yourself won't save it.
5. If it is still framed at round end, it is saved and may appear in future rounds.

**Persistent content.** Uploaded books and saved paintings go into a database every future round and player can see. Keep them within `server-rules.md` (no slurs, bigotry or OOC), don't upload junk, and when you're playing through the client for someone, check with them before uploading anything permanent.

### News

- Newscaster: post stories (interviews, events, the clown's latest), attach camera photos, print up to 15 newspapers (refill with paper) and deliver them to busy places (Medbay, Brig).
- Broadcast camera: use in hand to broadcast live to every entertainment monitor; right-click to rename the broadcast; Alt-click to toggle its microphone (on by default).
- Podcast: talk on the Entertainment channel.

## 5. Heroic beacon kits

Pick one:

| Kit | Contents |
|---|---|
| First Man on the Moon | NASA voidsuit (two pieces), GPS, oxygen tank |
| Braveheart | Kilt and sandals, claymore (blocks sometimes), spray paint |
| Courageous Tomb Raider | Treasure hunter's hat, armored coat, suit, boots; **whip** (high disarm chance; one tip says it always disarms) |
| Carp Hunter | Carp space suit (spaceworthy, no protection), carp mask, hunting knife (butchering bonus), sack of meat |
| Mothic Flight Pioneer | Softcap, flightsuit, wrench, screwdriver, crowbar, full stacks of iron and glass, lantern |
| Ethereal Trailwarden | Tunic, oilcoat, saddlepack (duffel capacity, no slowdown) |
| Assassinated by CIA (journalist) | Shirt, slacks, press fedora, suspenders, Entertainment microphone, press badge, clipboard, tape recorder, paper bundle, camera, entertainment monitor and radio |

With Construction access you can build a base, go to Lavaland, or renovate the Vacant Office.

## 6. Tips

- Cut a hidden slot in a book with wirecutters.
- Make the Library worth visiting: a hand-picked shelf, decorations, events, advertising on the radio.
- Fix rotting wood tiles (pry up with a screwdriver; deconstruct tables with a wrench) and clear cobwebs.
- The databases can also be browsed outside the game on the wiki's linked site (needs a /tg/ forum account).
- Your study can be welded shut against a mob, but Security or the AI will get in; it buys seconds, not safety.

## 7. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Empty shelves all round | Order from the external archive at shift start. |
| Printing 100 copies | Print a few. |
| Scanner does nothing | Use it on the computer, in the right mode. |
| Painting not saved | Hang it in a roundstart frame and keep it there to round end. |
| Uploading offensive or junk books | Don't; it's permanent and still covered by the rules. |
| Readings or broadcasts that provoke the crew | Read the room; don't break rules for a joke. |

**If you are an antagonist (the page's "Book'em Danno").** You have armor and the whip: disarm Security's guns, silence loud targets. Your access is poor and your outfit is recognizable, so ditch it, do the steal or kill fast, and hole up in the study. An emagged library computer prints a cult tome (readable only by cultists) to confuse Security; expect to be searched and brigged. Exposed antagonists should expect the crew to try to kill them. The limits in `server-rules.md` rule 4 still apply (no metagaming, metacomms, exploits, erotic or creepy behaviour, OOC in IC, or spawn-camping arrivals).

## 8. Working with the crew

Bring the Chaplain a new bible when theirs is lost. Lend books to anyone who asks. Interview heads and crew for the news, and deliver newspapers. Your languages make you useful to Security for understanding cultists or xenos; tell them what you hear.

## 9. Through the client

- `walk_to {area: "Library"}`; `look` for the computers, binder, shelves and newscaster.
- Library computer and newscaster: `click`, then `tgui_window` to read the menu and `tgui_act` to choose; if it is an old HTML window, follow its links with `topic`. Use the options it shows (e.g. "Connect to External Archive", "ORDER", "UPLOAD") rather than guessing names.
- Barcode scanner: `key Z` with it in hand to cycle modes; `click` a book with it, then `click` the computer.
- Writing: hold the pen and `click` the paper; text input arrives as a prompt (`answer_prompt`).
- Broadcast camera: `key Z` in hand to start; `click {right: true}` to rename; `click {alt: true}` for the mic.
- Entertainment channel: check with `say`'s radio options; it must be switched on in the headset first.

## 10. Checklist

- [ ] Stock the shelves from the archive.
- [ ] Choose a beacon kit.
- [ ] Put printed books in the inventory; lend on request.
- [ ] Bind and upload worthwhile books; save good paintings in roundstart frames.
- [ ] Post news; print and deliver papers.
- [ ] Replace the Chaplain's bible if needed.

## 11. Sources

The /tg/station 13 wiki, "Curator" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/curator.txt. Not checked against the server's code.
