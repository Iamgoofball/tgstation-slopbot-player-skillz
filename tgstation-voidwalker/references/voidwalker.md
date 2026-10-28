# Voidwalker (tgstation)

The wiki's guide to the voidwalker. It is not checked against the server's code. **Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.** The page links pull requests 84674, 85045, 91004 and 91646 (the role's history) and 87982, which **was not merged**: nothing from it applies. The role may have changed since; trust what the game shows you.

## 1. The role

A rare midround antagonist that spawns near the station: an ambush predator from space. You are invisible and fast in space, slow in gravity. You phase through windows, knock out crew near space, drag them out and kidnap them into the void; they come back cursed (the Voided). You have no kill ability of your own, but nothing stops you from leaving victims to die in space. Hunt aggressively, and enter gravity only to strike.

Limits that still apply (rule 4, lone antagonist): no metagaming or metacomms, no bug or exploit abuse, no erotic or creepy behaviour, no OOC in IC or IC in OOC, no spawn-camping arrivals.

## 2. Physiology

- **150 HP, 33% burn armour.** Lasers hurt you less than bullets.
- **Left click:** heavy oxygen damage, your knockout tool. **Right click:** a little brute.
- **In space** you regenerate health. **In gravity** you are slowed. **Planetary gravity kills you quickly**: never go to Lavaland or any planet.
- **Glass and grilles:** you walk through them unless they are **electrified**. The window stays passable, so victims may crawl back in and crew may follow you out.
- **Under the station:** bump into a wall while standing in space to move under the station. From there you watch for victims and reach isolated stretches of space.

## 3. Abilities

| Ability | Effect | Notes |
|---|---|---|
| Space Camouflage | Invisible and free-moving while in space | Hitting something or being hit reveals you briefly. Crew may sweep for you. |
| Unsettle | Stuns, slows and slurs a target | Stay in their view for 6 s to complete it; reveals you briefly. |
| Cosmic Dash | A charge; only space tiles are valid targets | Escapes and space fights. |
| Voidwalker Telepathy | Send a message to someone | You can't speak. Taunt your next victims. |
| Vomit Walker | Dive in and out of nebula vomit, and kidnap people into it | Diving in **removes** that puddle. Plan your exit before diving in mid-station. |
| Wall Conversion | **Right-click** a soft wall (non-reinforced iron or weaker): it and adjacent walls become void windows you walk through | Starts with **2 charges**; successful kidnaps give more. |

## 4. Kidnapping and the Voided

1. Get a victim **into space and unconscious**: phase in, knock them out with left clicks, Unsettle them if they fight, drag them out through the window.
2. Kidnap them. They go to the void and come back after a while with the **Voided** trauma.
3. **The Voided** are fragile and pacified, and can't enter space. One hit puts a Voided to sleep for 30 s if they're in your way. You can't kidnap the same person twice unless they're cured (lobotomy, or dying in planetary gravity).
4. The Voided spew **nebula vomit** now and then: new portals for you around the station. Every kidnap widens your reach and gives wall-conversion charges.

## 5. Tactics

- Stalk from under the station. Pick lone crew next to exterior windows: maintenance, solars, the escape arm, departments on the hull.
- Phase in, knock out, drag out, kidnap, vanish. Don't fight in the open in gravity: you're slow and easy to shoot.
- Use void walls and vomit puddles to reach rooms with no exterior window, but always keep a way back to space.
- Skip electrified windows; find unpowered ones.
- Use telepathy to panic people into isolated corners.
- Once you're seen, the crew will hunt you and try to kill you: retreat to space, regenerate, strike somewhere else.

## 6. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Lingering inside | You're slow, revealed and stuck. Strike and leave. |
| Diving into your only vomit puddle | It's used up. Keep a second exit (a window, a void wall). |
| Taking on a group | Unsettle needs 6 s on one target. Pick off loners. |
| Electrified windows | You can't pass them. Go around. |
| Gunfights with bullet users | Bullets hurt you far more than lasers. Avoid them. |
| Planetary gravity | Kills you fast. Stay at the station. |

## 7. Fighting a voidwalker (crew)

- It's most vulnerable when it comes in for a victim: inside, it's slowed and has no easy way out. Once it's confirmed, kill it; that is normal and expected.
- **Bullets beat lasers** against it. Lasers still punish it through windows.
- **Electrify windows** or block them off. Shutters, and a friend hiding nearby while you play the bait, make good traps.
- Space patrols in MODsuits with jetpacks can hunt it, but it is strongest in space: hit it to reveal it, then shoot. Go in pairs so Unsettle can't lock one person down.
- **On death** it shatters into glass and a **Cosmic Skull**. Staring into the skull gives **Stable Voided**: still fragile to brute and killed by planetary gravity, but full space immunity and the ability to walk through glass.

## 8. Through the client

- Attack: `click` the target (left click). Right click (brute, or Wall Conversion on a soft wall): `click {object_id, right: true}`.
- Unsettle, Cosmic Dash and Telepathy are HUD action buttons: list them with `screen`, `click` the button, then `click` the target.
- Telepathy text: `answer_prompt`, or `tgui_act` on a tgui input.
- Going under the station: `move` into a wall while standing in space.
- `look` for windows and lone crew; `examine` a window if you're unsure it's electrified.

## 9. Checklist

- [ ] Stay in space; never planetary gravity.
- [ ] Lone crew near exterior windows found.
- [ ] Knock out, drag to space, kidnap.
- [ ] New vomit puddles and wall charges used to widen your reach; an exit always kept.
- [ ] Back to space to regenerate when hurt or seen.

## Sources

The /tg/station 13 wiki, "Voidwalker" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_void_walker.txt. Not checked against the server's code. The page lists GitHub pull requests 84674, 85045, 87982 (not merged), 91004 and 91646.
