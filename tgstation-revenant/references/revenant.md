# Revenant (tgstation)

The wiki's guide to the revenant. It is not checked against the server's code. **Where it disagrees with `crew-basics.md` or `server-rules.md`, those win.**

## 1. The role

A revenant is a ghost charged with alien energy, half back in the mortal world. You are invisible, fly through walls, and can't be hurt while hidden; the chaplain and holy things can still affect you, and machines may notice you. You feed on the crew's life force (essence) to grow stronger and spread chaos. Most abilities reveal you briefly, and that is when you can die.

You become one by a random event (if you have the Revenant preference on: the special-candidacy verb in the Preferences tab) or by an admin. A sound plays, and you spawn somewhere thick with death.

Limits that still apply (rule 4, lone antagonist): no metagaming or metacomms, no bug or exploit abuse, no erotic or creepy behaviour, no OOC in IC or IC in OOC, no spawn-camping arrivals. Killing crew to harvest them is the role.

## 2. Essence

- The number with an **E** on the right of your screen. **Essence is your health and your currency.**
- It regenerates up to **75** by default. **At 0 you die**, leaving blue dust (glimmering residue) that revives you within about a minute unless someone scatters it.
- Unlocking needs the cost **on top of** what you keep: to unlock a 75E ability you need 150E on hand.
- Harvesting a living human, or a "perfect soul", can raise your maximum essence.

## 3. Abilities

| Ability | Unlock | Use | Cooldown | Stun / reveal | Effect |
|---|---|---|---|---|---|
| Harvest | Start | – | None | 5 s / 5 s | Click an adjacent unconscious or dead human. Dead body: 15-20E. Body with soul in: 35-50E. Living, no soul: 45-70E. **Living with soul: 75-100E.** An unconscious or stunned living target **dies**. Each body only once. |
| Toggle Nightvision | Start | – | None | – | On by default. |
| Transmit | Start | – | None | – | A spooky message to one person. Works from inside walls. |
| Defile | 10E | 30E | 15 s | 1 s / 4 s | 9x9: removes holiness from tiles (clears holy water and salt), rips up floor tiles, rusts walls, damages windows, fills showers with blood, opens most containers, flickers lights. |
| Overload Light | 25E | 40E | 20 s | 3 s / 8 s | 13x13: after a sparking delay, lights shoot lightning at anyone still nearby (medium damage, stun, sparks). |
| Blight | 75E | 50E | 20 s | 2 s / 5 s | 9x9: infects humans with a virus doing heavy stamina and toxin damage over time until cured; nonhumans take toxin; damages or kills plants. |
| Malfunction | 125E | 60E | 20 s | 2 s / 8 s | 9x9: machines and objects malfunction, sometimes with an emag effect; stuns and damages cyborgs, disables electronics on humans, emags bots at once. |

## 4. Being revealed

While harvesting or channelling, and for a while after an ability, you are **visible and attackable**, can't move during the channel, and afterwards are slow and can't pass walls or most solid objects. You can still open doors, cross tables and plastic flaps, and pass through living mobs. **This is your most vulnerable state.** Use abilities where you can't be cornered.

## 5. Tactics

- **Early:** find corpses (morgue, maintenance, after fights) and harvest them. Ghosts in deadchat can point you to bodies, but don't trust them blindly.
- **Big essence:** a living human with a soul gives 75-100E and dies if stunned or unconscious. Stun with Overload Light or let Blight wear someone down, then harvest them somewhere private.
- **Unlock order:** Defile (cheap, breaks holy-water and salt lines) and Overload Light first, then Blight, then Malfunction.
- **Malfunction** on Security's gear, borgs and bots; **Defile** to strip the chapel's protection and to open lockers; **Blight** on crowds; **Overload Light** in busy hallways, then harvest whoever drops.
- Use **Transmit** to scare and mislead people.
- Keep enough essence banked to survive: spending to near 0 and then getting revealed kills you.
- Once you're spotted, the crew will hunt you with the chaplain and holy water. Lie low inside walls, regenerate, then hit another part of the station.

## 6. Dangers and common mistakes

| Mistake | Fix |
|---|---|
| Harvesting in the open | 5 s stuck and visible. Drag or find bodies somewhere quiet. |
| Spending all your essence | Essence is your health. Keep a buffer. |
| Fighting the chaplain | The null rod drains huge chunks of essence. Avoid them, Defile their protections, or catch them alone and stunned. |
| Walking into holy water or salt | You can't pass it unless you Defile it; salt also stuns and reveals you. |
| Trusting ghosts | They lie (you are **not** immune to the Supermatter; it dusts you). |
| Leaving your residue near crew | If they throw it, you're gone for good. Die far from people if you must. |

## 7. Fighting a revenant (crew)

- Signs: a person with purple light flowing out of them toward a blue ghost (a harvest), flickering lights, defiled tiles, sudden lightning from lights. Shout it on the radio.
- **Get the chaplain**: the null rod drains large amounts of essence.
- Strike when it reveals itself: during a harvest or right after an ability. Once confirmed, kill it; that is normal and expected.
- **Holy water and salt** block it unless it Defiles them; coat floors, or spray it when it casts. Salt also stuns and reveals it.
- When it dies it leaves **glimmering residue**; left alone, it respawns in 60 s. **Pick the residue up and throw it** to kill it permanently.

## 8. Through the client

- Essence: read it from `screen` or `status`.
- Abilities are HUD action buttons: list them with `screen`, `click` one to use it (area abilities fire around you; Transmit asks for a target and text). Unlocking uses the same buttons; read the exact names there.
- Harvest: `click` the adjacent body.
- Transmit text: `answer_prompt`, or `tgui_act` on a tgui input.
- Deadchat: `read_chat`, and `say` on the dead channel if the tool lists one.
- Before revealing yourself, `look` for crew and the chaplain nearby.

## 9. Checklist

- [ ] Bodies found and harvested; essence banked above 75.
- [ ] Defile and Overload Light unlocked, then Blight, then Malfunction.
- [ ] Living targets stunned and harvested in private.
- [ ] Chaplain located and avoided.
- [ ] Hide and regenerate after each reveal.

## Sources

The /tg/station 13 wiki, "Revenant" (CC BY-SA 3.0), as provided in pages_to_turn_into_skills/antag_revenant.txt. Not checked against the server's code.
