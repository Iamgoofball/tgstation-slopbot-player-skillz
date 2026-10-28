# Detective (tgstation)

Derived from the wiki's Detective page; not checked against the server's code. Where it disagrees with `crew-basics.md` or `server-rules.md`, those win. Arrests, records screens and Space Law are in `tgstation-security-officer`.

## 1. The role in one paragraph

You investigate crimes: examine scenes, collect and scan evidence, identify the culprit, and ask Security to arrest them. You are an evidence collector and monster hunter, not a beat cop or warden, which is why your Security access is limited. **Your revolver is for self-defence only.** Difficulty: medium; you answer to the Head of Security. Minimum: scan evidence at crime scenes, look up the prints and DNA, and pass the names to Security. By default the Detective can't be an antagonist.

**Confirmed antagonists.** Once you have determined beyond doubt that someone is an antagonist (and that is often your job), Security, you included, may kill them. Most antagonists can't be safely contained, and dead ones return to the ghost poll for midround antagonists and events, so killing a confirmed antagonist is normal and expected. Until it's certain, the revolver stays for self-defence and suspects go to Security for arrest. Say plainly on `:s` when an identification is confirmed and when it is only a suspicion.

## 2. Kit, access and radio

- **Access:** Brig, Detective's Office, Coroner Office, Morgue, Maintenance, weapon permit; Security as an extra. Getting past a department's outer doors gives you its security outpost.
- **Radio:** Security (`:s`). Report on it, not on Common, or the suspect hears and runs.
- **On you / in the office:**
  - Forensic scanner (backpack; spare in the office closet). Lists fingerprints, materials and fibers as a timeline, oldest first. Works at range; scanning a person gives their prints.
  - Black gloves: **never take them off** while investigating, or your prints spoil the evidence.
  - PDA with Security Records (download Medical Records too) to identify prints on the go.
  - .38 revolver in a holster in your locker, plus speed loaders (keep them in your internals box). Reskin, rename, special ammo.
  - Worn suit, coat and hat (armor; hat holds candy corn), armored vest, security headset, seclite (pocket it lit), classic police baton, handcuffs.
  - Universal recorder (doubles as a translator for slimes, monkeys, xenos), hand labeller, camera, white crayon (corpse outlines).
  - Crew pinpointer (finds people whose suit sensors are on), Security holotape projector (cordon scenes), binoculars, spyglass kit (hidden camera pocket protector and linked sunglasses).
  - Cigarettes and Zippo; a clothing vendor with outfits.
- Ask the Warden for more standard Security gear.

### .38 ammo

| Type | Damage | Effect | Source |
|---|---|---|---|
| Normal | 25 brute | standard | Cargo, autolathe, Security techfab, starting holster |
| TRAC | 10 | weak short-lived tracker | Cargo, Security techfab |
| Match | 25 | better ricochet | Cargo |
| Rubber | 10 | disabler-level stamina damage (still some brute) | Cargo |
| DumDum | 15 | sharp, likely to embed, weak vs armor | Cargo |
| Hotshot | 20 | sets target on fire | Cargo, Security techfab |
| Iceblox | 20 | chills to 100 K: slowdown and burns | Cargo, Security techfab |
| Flareshot | - | marks a limb 2 min so every hit lands there; washes off | Security techfab |

Recycle empty speed loaders in the autolathe for a refund (one tip says full, another partial). A wrench converts the revolver to .357, far more lethal but liable to backfire; eject the rounds first.

## 3. Where things are

Your office has Security Records and Medical Records consoles, a camera terminal (an old TV), a filing cabinet, two folders, the closet with the spare scanner, and the clothing vendor. Evidence Storage (Brig) has several lockers. The Interrogation room is in the Brig. The Morgue and Coroner are your other haunts.

## 4. Working a scene

1. Cordon it with holotape. Photograph relevant things.
2. Scan everything around it: doors, walls, consoles, out-of-place items, and any body (prints and fibers). Scanning containers works at range.
3. Bag the evidence. To avoid contamination, bag an item without touching it; to put it down, hold the bag in the active hand with the other hand full and press `Z` to drop the item out.
4. Body already moved? Go to the Morgue or genetics and scan it there. Find out who brought it in and who touched it (medbay should wear nitrile gloves).
5. Back at your office or a security outpost, match prints on the Security Records console and blood/DNA on the Medical Records console. Blood but no body identifies the victim.
6. Read fibers carefully: insulated gloves and an engineer's jumpsuit on the body suggest an engineer; only your own fibers or black gloves mean a cold case.
7. A weapon with someone's prints (not the confiscating officer's) is strong. One clear hit: set them to arrest in records and tell Security on `:s` with what helps: likely contraband, other identities, jumpsuit color, hairstyle.
8. If there is a trial, **you attend as prosecution** with scan results, photos and witness statements. The HoS may want to prosecute; brief them fully.

### Case files

- Label everything in one case with one name ("Clown Case"); one Evidence Storage locker per case.
- One folder per case; closed cases go in the filing cabinet; copy key documents for yourself or Security.
- Stay in touch with the Coroner for unusual deaths and autopsies.

## 5. Advanced work

- **Multiple suspects** usually mean inconclusive forensics: interview. Carry the universal recorder. Go in with a hunch and ask relevant questions; a non-pointed question can trip a bluffer; someone who warms up after a subject changes may be lying.
- **Groups** (changelings, some traitors) are easy to spot and one confession can bring down all of them, but they take a lot of officers to arrest. Be careful at their scenes.
- **Time of death:** a health analyzer from Medbay gives damage types, diseases and time of death; right-click a body with it for bloodstream chemicals (good for fresh poisonings). The Coroner's autopsies give more.
- **Husks:** draw blood with a syringe or scan with an analyzer; changelings drain all the blood when they husk. Scan an unidentified husk for its prints.
- **Hidden walls:** meson scanners show hidden doors as open space when not in direct sight.
- **Labelled gloves:** label your black gloves with your name at round start so your fibers are distinguishable from other black gloves.

## 6. Spare time

You'll rarely be called, so investigate on your own initiative:
- Snoop maintenance (off-camera).
- Help Security generally, or bodyguard a weak head (the RD).
- Watch the camera terminal and report crimes on `:s` (not Common).
- Update security records.
- Check disposals for bodies, contraband and weapons.

The Horrific Necktie from the clothing vendor has an action button that offers ghosts a voice-only "imaginary friend" role only you can hear.

## 7. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Taking off the black gloves | Keep them on; your prints ruin evidence. |
| Contaminating evidence by handling it | Bag without touching; drop from the bag with `Z`. |
| Announcing a suspect on Common | Use the Security channel. |
| Acting as a beat cop or shooting a suspect | Investigate; the revolver is self-defence until an antagonist is confirmed. |
| .357 conversion blows up in your hand | Eject rounds first; expect backfires anyway. |
| Body moved before you scanned it | Scan at the Morgue; trace who moved it. |
| Missing your own trial | Attend with all evidence. |

**If you are an antagonist.** By default the Detective can't be one. If the game makes you one anyway, the page's "Smooth Criminal" advice applies: your gun, Security access and position as lead investigator cover you. Falsify evidence, stage scenes, cover up your kills, or buy a Syndicate revolver. The limits in `server-rules.md` rule 4 still apply (no metagaming, metacomms, exploits, erotic or creepy behaviour, OOC in IC, or spawn-camping arrivals). As crew, never falsify evidence.

## 8. Working with others

- **Security:** you find, they arrest. Give them names and descriptions.
- **HoS:** your superior; brief them for trials.
- **Warden:** issues extra gear; puts dangerous evidence in the Armory.
- **Coroner and Medbay:** autopsies, time of death, unusual deaths.

## 9. Through the client

- `walk_to {area: "Detective's Office"}`; `inventory` to confirm scanner, gloves and gun; open the locker (click to unlock, click to open) for the revolver.
- Scan by holding the scanner in the active hand and `click`ing the object or person; the result comes back as chat or a window. `examine` items for printed details.
- Records consoles are tgui windows: `click` the console, `tgui_window` for its contents and actions, `tgui_act` to search or set arrest status.
- Report with `say {text, radio: "security"}`. Use `search` (kind mob) with a name to find a suspect, as in `tgstation-security-officer` §9.
- `key Z` uses the held item (drop from an evidence bag, toggle the seclite). Swap hands with `key X`.

## 10. Checklist

- [ ] Gloves on; label them; take scanner, revolver and speed loaders.
- [ ] Scene: cordon, photograph, scan, bag.
- [ ] Look up prints and blood; set arrest; tell Security on `:s`.
- [ ] One label, locker and folder per case.
- [ ] Attend trials as prosecution.
- [ ] Quiet time: cameras, maintenance, disposals, records.

## 11. Sources

The /tg/station 13 wiki, "Detective" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/detective.txt. Not checked against the server's code.
