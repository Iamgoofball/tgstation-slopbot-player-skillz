# Blood cultist (tgstation)

The wiki's guide to the Cult of Nar'Sie. It is not checked against the server's code. **Where it disagrees with `crew-basics.md` or `server-rules.md`, those win**. Section 11 lists the few limits that still bind you.

## 1. The role

Several cultists start the round on the station; more join by conversion. You work as a team toward two objectives: **sacrifice the target** (shown to all cultists in the top right of the screen; usually a head of staff or a Security officer) on an Offer rune, then **summon Nar'Sie** in one of three set locations with 9 cultists and/or constructs standing on the finished summoning rune. If Nar'Sie is summoned, the cult wins. Cult is a **team antagonist**: you must not harm the cult's work, by acting or by doing nothing, and the Cult Master's orders and your converter's goals come first.

## 2. Kit and communication

- **In your bag at start:** a ritual dagger and 10 runed metal. Converts get a dagger from the Offer rune.
- **Commune** (action button): sends a message to every cultist. **Anyone near you sees and hears you whispering it**, so commune only where you are alone. Stunned or restrained cultists cannot commune.
- **Blood Magic** (action button): prepares spells (section 4).
- **Assert Leadership** (next to Commune): apply to be Cult Master (section 7).
- Your access is whatever your job gives you. Jobs with isolated workplaces make good meeting points; so does space.

## 3. The ritual dagger

- Draws runes ("Scribe Rune"; costs minor damage from cutting your wrist).
- Hit a cultist with it: removes holy water from them.
- Hit a non-cultist: 15 armour-piercing brute. Thrown: 25. Can be sharpened (Eldritch Whetstone). 25% chance to block melee.
- Hit a rune: erases it. Hit a cult structure: anchors or unanchors it. Hit a runed girder: dismantles it.
- Lost it? The Summon Ritual Dagger spell makes a new one.

## 4. Blood spells

Prepare with the Blood Magic button. **Off an Empowering rune you get only one spell, it takes longer and costs a lot of blood. On one you can hold four**, faster and cheaply; the Empowering rune also removes spells to make room. Preparing leaves blood on the floor: do it unseen. To use a spell, click its action button to put it in your hand, then use it in hand or on a target. To put it away unused, press `Q` or click the button again.

Keep one Stun and one Teleport whenever you can.

| Spell | Effect | Cost / charges |
|---|---|---|
| Stun | Paralyses and mutes, slurs speech into cult-speak. Before red eyes: 16 s paralysis, 12 s mute, 30 s slur. With red eyes: 9.6 / 7.2 / 18 s. With halos: 1.6 / 1.2 / 3 s. On a cyborg: heavy EMP effect at any cult size. No effect on anyone with magic protection, heretics, or a chaplain holding a null rod. | 1 charge, 10 HP |
| Teleport | Touch a cultist (or yourself) to send them to a chosen teleport rune. | 1 charge, 7 HP |
| Electromagnetic Pulse | EMP, range 5. | 1 charge, 10 HP |
| Shadow Shackles | Cuffs a victim and silences them 10 s. Vanish when the victim converts. | 4 charges |
| Twisted Construction | Plasteel to runed metal; 50 metal sheets to a construct shell; cyborg to construct; cyborg shell to construct shell; airlock to brittle cult airlock (in combat mode). | 1 charge, 12 HP |
| Summon Ritual Dagger | Activate, then click yourself. | 1 charge |
| Summon Combat Equipment | Black jumpsuit, armoured robes, hood, boots, trophy rack, Nar'Sien bola, spare dagger. Activate, click yourself. Occupied slots get only the dagger and bola. | 1 charge |
| Hallucinations | Ranged, stealthy hallucinations. The wiki calls it near useless. | 4 charges |
| Conceal Presence | Toggles hiding/revealing runes and cult structures within 5 tiles. Concealed teleport runes still work as destinations, concealed empowering runes still work. Runed airlocks look like maintenance airlocks (cultists only). | 10 charges |
| Blood Rites | Absorb blood from the floor, or 50 per drain from a living victim; spend it to heal yourself or others, or on: **Blood Spear (150)**, a two-handed halberd, 24 brute, recalls to hand within 10 tiles with a clear path, thrown it shatters for 40 brute and a stun; **Blood Bolt Barrage (300)**, 25 shots of 20 brute (keep both hands free, it switches hands each shot; good on mechs); **Blood Beam (500)**, a channelled cone that pierces structures, converts walls, floors, airlocks and windows to cult versions, damages non-cultists and heals cultists with unholy water. Blessed tiles block it. | 5 charges |

## 5. Runes

Scribe with the dagger, then click the rune to invoke it. Examine a rune to see its name and effect. Rune drawing is 50% faster on engraved cult floor (not the Nar'Sie rune).

| Rune | Invokers | Effect |
|---|---|---|
| Offering | 1 to sacrifice the dead, 2 to convert, 3 to sacrifice the objective or a living ineligible target | Converts a crewmember on it (heals 75% of their brute and burn, spawns a dagger). Mindshielded crew, the dead, and the sacrifice target are **sacrificed** instead: gibbed, leaving a soulstone shard. Heads' pets can be converted into cult pets that attack non-cultists and drag dead cultists to revive runes. |
| Empowering | 1 | Hold up to 4 blood spells, prepared faster and with less blood loss. |
| Teleport | 1 | Sends everything on it to another teleport rune; you tag each one when you draw it. **Teleporting from Lavaland or space makes the destination glow and opens a rift that can reveal it and your base.** |
| Revive | 1 | Revives a cultist corpse on it for 3 charges (global; starts with 1, each sacrifice adds 1). Puts a new soul into a catatonic (disconnected or ghosted) cultist for free. |
| Barrier | 1 | Invisible wall for 5 minutes; invoke again to drop it. 2 brute to raise or drop; 100 health; the rune breaks if the wall does. |
| Summoning | 2 | Pulls any living cultist to the rune, then the rune is used up. Works only on the station. Fails on restrained cultists who are buckled or being pulled. |
| Blood Boil | 3 | Costs the invokers health; three pulses of 25/50/75 damage (half brute, half burn) to every non-cultist who can see it, then sets fire to what is on it. Bloodless species (golems) and magic-immune people are unaffected. |
| Spirit Realm | 1 | Either manifest ghosts as weak homunculus cultists (station only; you must stay on the rune and take brute over time for each; erase the rune with the dagger if stuck), or ascend as a dark spirit: see what ghosts see, commune loudly, and mark a target for the cult. |
| Apocalypse | 3 | Only in one of the three ritual areas, and that area can then **no longer be used for Nar'Sie**. Massive EMP and hallucinations; scales with crew strength. If the cult is under 15% of players, a d100 picks: 1-10 disease outbreak + mice; 11-20 radiation storm; 21-30 brand intelligence; 31-40 three immovable rods; 41-50 meteor wave; 51-60 spiders; 61-70 anomalies; 71-80 space vines + grey tide; 81-100 Nar'Sian portal storm. |
| Ritual of Dimensional Rending | 9 to invoke | The Nar'Sie rune. Needs a free 3x3 in one of the three areas, and the target already sacrificed. Drawing takes 45 seconds, shields the drawer in a weak forcefield and **announces the location to the whole station**. When drawn, 9 cultists, constructs or manifested ghosts stand on it (lie down with rest to fit) and one clicks it with an empty hand. |

## 6. Structures and constructs

Runed metal: start with 10; make more with Twisted Construction on plasteel (from mining, Robotics, Engineering, EVA, or deconstructed reinforced walls and tables; the AI satellite holds spare plasma and metal). Dagger-hit a structure to move it. Conceal Presence hides them.

| Structure | Cost | Makes (each use starts a 4-minute recharge) |
|---|---|---|
| Altar | 3 | Eldritch Whetstone; Construct Shell; Flask of Unholy Water (heals cultists and cuts stuns; thrown, poisons non-cultists) |
| Forge | 3 | True Nar'Sian Hardened Armor (hardsuit, no slowdown); Flagellant's Robe (faster, +45% damage taken); Eldritch Longsword (30 damage, 50% block, fits cult armour's suit storage) |
| Archives | 3 | Zealot's Blindfold (night vision, medical HUD, flashproof); Shuttle Curse (delays the escape shuttle 2 minutes; limited per round); Veil Walker Set (Veil Shifter: 4 forward teleports taking what you drag; Void Torch: teleports objects to other cultists) |
| Pylon | 4 | Slowly heals cultists; turns floor to engraved floor (faster runes, resists atmosphere changes) |
| Runed door | 1 | Cultist-only airlock; stuns and throws non-cultists; a dead giveaway |
| Runed girder | 1 | Girder the dagger dismantles instantly |

Each cultist's 10 metal builds 3 of altar/forge/archives. Build one of each early; pylons only heal. Don't make items you don't need: each one locks that structure for 4 minutes.

**Constructs**: a filled soulstone (from a sacrifice, or an artificer's stone used on a corpse) in an empty shell (Twisted Construction on 50 metal, an altar, or an artificer). Choose: **Artificer** (makes shells and soulstones; build this first), **Juggernaut** (tank), **Wraith** (jaunts; can reach and kill the AI). An empty soulstone used on a corpse captures its soul; clicking it in hand releases a weak **shade**, which can ventcrawl (alt-click a vent). A shade you release and recapture lets you invoke two-person runes alone, but it counts as an invoker only after one minute out of the stone. Constructs reveal the cult: keep them hidden early.

## 7. The Cult Master

Any cultist can press Assert Leadership; a cult-wide vote follows. Many cults wait to pick a Master until they are ready to summon. The Master's commune is large and bold. Master powers (top-left HUD):

| Power | Effect | Cooldown |
|---|---|---|
| Final Reckoning | Brings the entire cult to the Master. Not usable inside a summoning area. | **One use only** |
| Mark Target | Marks a person for the cult for 90 s, sending their name and location. | 120 s |
| Eldritch Pulse | Teleports a cultist or cult structure to a spot on your screen (into the armory, behind a raid, out of danger). | 15 s |

The Master's job: pick a hidden, defensible base; keep intruders out; stay near base (with healing nearby) to be the second invoker for conversions; keep altars and forges producing ahead of need; direct the cult from a Spirit Realm rune; use Final Reckoning only when ready to draw the Nar'Sie rune.

## 8. The plan, step by step

1. **Commune** alone: say where you work and what access you have, agree a plan.
2. **Base**: in a secluded place draw a **Teleport rune**, then commune its location so others can come. Add an **Empowering** rune and an **Offer** rune. Non-cultists must not find them.
3. **Convert**: on the Empowering rune prepare Stun, Shadow Shackles and two more (several Stuns are fine). Stun a crewmember, take them somewhere private, shackle, pull off their headset if base is far, bring them to the Offer rune, invoke with a second cultist (or a Spirit Realm ghost next to it, which lets you convert alone). Mindshielded crew (Security, heads) are sacrificed instead and leave a soulstone: finish Security victims quickly, before their radio or suit sensors give you away.
4. **Build**: altar, forge, archives; first construct an Artificer.
5. **Go loud** when found out, or when red eyes and halos make hiding impossible: spread backup Teleport runes and mini-bases, push conversions, deal with the AI.
6. **Sacrifice** the target (3 invokers if alive). Its icon changes to the three summoning locations.
7. **Summon**: fortify one location, Final Reckoning the cult there, draw the 3x3 rune (45 s), get 9 on it, invoke.

## 9. Being found out

- **20% of active players in the cult**: after a delay every cultist's eyes turn permanently red. Examine shows it unless you wear eyewear.
- **40%**: after a delay every cultist gets a blood-red halo. Nothing hides it.
- Stun gets far weaker at each stage (section 4).
- Other giveaways: whispering while communing, blood splatters from spell preparation, cut arms, runed doors, constructs, cult-slurred speech on the radio.

## 10. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Communing next to crew | They hear the whisper. Commune alone, in maintenance, space or a private workplace. |
| Preparing spells off an empower rune | One spell, slow, heavy blood loss. Use the rune. |
| Stunning the chaplain while he holds a null rod | It does nothing and outs you. Avoid him or fight him another way. |
| Teleporting from space or Lavaland to your main base | The rift reveals it. Use an outlying rune. |
| Wasting Final Reckoning | One use. Only when the summoning site is ready. |
| Drawing the Apocalypse rune in your planned summon area | That area can no longer summon Nar'Sie. |
| Building items "just in case" | 4-minute lockout. Build when needed, and enough for everyone at once. |
| Leaving an arrested cultist | Watch Common for arrests and report them in commune; a Summoning rune can pull them out unless buckled or pulled. Ask ghosts (Spirit Realm) where dead cultists are. |
| Converting golems | Adamantine golems are anti-magic; silver and cloth golems are holy: immune. |
| Mindshield thinking | A mindshield does not deconvert; it blocks conversion. Implanted crew can still be sacrificed. |
| Trusting the holy | Holy water in you is removed by a cultist's dagger hit; get it out before it deconverts you (section 12). |

## 11. What limits you

- Cult is a team antagonist (rule 4): don't undermine the cult, follow the Master and whoever converted you. In priority, cult sits below blob/zombie, brainwash, construct orders and silicon laws, and above revolutionaries, blood brothers, nuclear operatives and traitors.
- Your job is the objectives, at all costs. Kill, sacrifice, burn with Blood Boil, call the Apocalypse rune's meteors and rods, EMP Security and the borgs, and send a wraith to kill the AI: all fair play.
- The limits that still apply (rule 4): no metagaming or metacomms, no bug or exploit abuse, no erotic or creepy behaviour, no OOC in IC or IC in OOC, no spawn-camping arrivals.
- Once you are exposed, expect the crew to kill you rather than deconvert you. Don't get caught alone.

## 12. Fighting the cult (crew)

**Signs:** people loitering near strange runes, small cuts on one arm, blood spills at someone's workplace, whispering, cult-slurred radio, red eyes (ask suspects to remove eyewear, then examine: "eyes are glowing an unnatural red"), pentagram halos.

**Killing or deconverting:** once someone is confirmed a cultist beyond doubt (seen using cult magic, runes or gear, red eyes or halo), lethal force is normal and expected; dead antagonists go back to the ghost pool. Deconversion is the option when you have them safely cuffed and want them back.

**Deconversion (Security):**
1. Arrest and cuff. A cuffed cultist who is held or buckle-cuffed to a chair can't be teleported away.
2. Search everywhere for the dagger and cult gear (boots of jackboots and workboots hide a dagger); lock it away and strip cult clothing.
3. Feed at least **25u holy water** (30u to be safe; a sip is 5u). Deconversion takes 60 chemical ticks (about 2 minutes). After 25 ticks they may blurt cult phrases and pass out for 12 s. Re-stun or flash them now and then so they don't slip the cuffs. Holy water wipes their prepared spells and blood rites at once.
4. **Mindshield-implant** them so they can't be reconverted.
A purple message, "... looks like he/she just reverted to his/her old faith!", confirms it. Deconverted cultists remember nothing of their time in the cult. Arm confirmed, implanted ex-cultists: they are your allies. Don't implant people at random: it proves nothing.

**When halos appear:** there is no time to deconvert; team up and fight, then go back to deconverting when it's under control. Shotgun slugs (30+ damage) shatter mirror shields and stun the user. Zealot's Blindfolds stop flashes, not flashbangs. Constructs can't be stunned: use lethal force.

**By job:**
- **Chaplain:** immune to conversion, and to cult magic while holding the null rod; still sacrificeable and often the target. Bless water with the bible into holy water, take a water tank to the brig and stay with Security. Fill an emptied fire extinguisher with holy water to bless tiles (blocks Blood Beams and wraith jaunts); bless the AI chamber's tiles. The bible reveals hidden runes. Anyone can purify a soulstone with a bible; a purified soul in a shell makes a construct that helps the crew.
- **Medical:** examine patients for red eyes and cult gear before treating. A smoke machine (board from the medical techfab or tech storage) filled with holy water wipes cultists' spells and blesses tiles touched by 10u+. Chemists: chloral hydrate in a syringe gun (harmless if you hit an innocent), combat drugs for Security. Geneticists: powers for Security. Keep away from suspicious people in quiet corners.
- **Cargo:** order Religious Supplies crates (holy water) if there is no chaplain; order mindshield implants; weapons if you can open the crates.
- **Science:** Robotics exosuits can't be stunned by cult magic. Silver golems are magic-immune. Ordnance: the wiki suggests a bomb on an announced summoning site as a last resort.
- **Engineering:** keep power up, build backup telecomms (cultists don't need it), help the AI move its core somewhere hidden. Atmospherics: don't flood the station with gas; fix breaches.
- **Botany:** holymelons ground into holy water; one held in hand protects against conversion and some spells until its charges run out.
- **Traitors:** a hypnotic flash can make a cultist talk (brainwash outranks cult in the priority list); not on deconverted cultists.

## 13. Through the client

- **Action buttons** (Commune, Blood Magic, prepared spells, Master powers) are HUD objects: list them with `screen` and `click` them by id. A prepared spell goes to your hand; `click` the target with it.
- **Commune** asks for text in a prompt or input window: answer with `answer_prompt` or, for a tgui input, `tgui_act {id, action: "submit", params: {entry: "..."}}` (the pattern documented for input boxes in `tgstation-ai`). Check `look` for nearby people first.
- **Scribing a rune** with the dagger in your active hand: use it in hand (click the held item) and pick the rune from the choice window or prompt that appears. Don't guess option names: read them from the window.
- **Invoking**: `click` the rune with an empty hand while the other invokers stand on adjacent tiles.
- Watch Common (`read_chat`) for arrests of brothers; use `wait {from_others: true}` between steps.
- `examine` suspects (crew side) to see red eyes; `examine` a rune to read what it does.

## 14. Checklist

**Start**
- [ ] Dagger and 10 runed metal in bag; objectives read.
- [ ] Commune alone: job, access, plan.
- [ ] Secluded base: Teleport rune (commune its tag), Empowering rune, Offer rune.

**Growing**
- [ ] Stun + Teleport always prepared.
- [ ] Conversions with two invokers; Security victims finished fast.
- [ ] Altar, forge, archives built; first construct is an Artificer.
- [ ] Backup teleport runes; Conceal Presence on the base.
- [ ] Eyewear once eyes go red.

**Ending**
- [ ] Target sacrificed (3 invokers if alive).
- [ ] Summon site fortified; Final Reckoning; 3x3 rune drawn and defended 45 s; 9 on it; invoke.
- [ ] AI killed or subverted; anything that threatens the summoning destroyed.

## Sources

The /tg/station 13 wiki, "Blood Cult" (cultist page, "Follower of Nar'Sie") (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_cultist.txt. Not checked against the server's code.
