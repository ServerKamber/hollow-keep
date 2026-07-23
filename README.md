# THE HOLLOW KEEP — Update VIII: Steel and Crowns

A single-file, first-person liminal-horror shooter set in an abandoned blocky castle.
No build step, no assets — everything (audio included) is generated in code.

## Run it

Open `index.html` in any modern desktop browser and click to enter.
Internet is needed once, to fetch Three.js from cdnjs.

## Controls

| Input | Action |
|---|---|
| WASD / Mouse | Move / look, hold left button to fire |
| Space | Jump, double jump, wall jump (against walls) |
| Shift | Dash |
| 1 / 2 / 3 | Sidearm / Scattergun / Requiem (once unlocked) |
| F or Right click | Blade slash (also deflects projectiles) |
| E | Spectral Lance — piercing skill shot, 8s cooldown |
| Q | JUDGEMENT — ultimate blast, 45s cooldown |
| R | Reload (auto-reload triggers on empty) |

## New in Update I

- **Enemy roster** — Hollow One (baseline), Wraith (fast, frail, from Night II), Spitter (ranged orbs, keeps its distance), Brute (armored, hits hard, from Night III)
- **Scattergun** — 8-pellet blast with pump animation and recoil kick; aim at the floor mid-air for a shotgun boost
- **Left-hand blade** — short-range arc slash with knockback; can cut incoming projectiles out of the air
- **E — Spectral Lance** — piercing energy bolt that damages everything in a line
- **R — JUDGEMENT** — screen-whiting shockwave: slow-motion, expanding ring, massive area damage
- **Boss: Gabriel, Judge of the Hollow Keep** — descends at 35 souls; the courtyard empties for a 1v1. Golden-armored winged judge with a burning halo. Four telegraphed attacks: guided sword throws, a dash slash, a rain of blades on marked ground, and an expanding blade ring. At half health he enters a red-halo rage phase — faster, angrier, triple throws. Boss health bar at the top; defeating him resumes the nights, and he returns stronger 50 souls later.

## New in Update II — Dusk, Stone, and Steel

- **Lighting** — the keep now sits at dusk instead of near-black night: a deep blue sky, warm low sun, and dimmer torches that read as accents rather than the only light source.
- **Textures** — the ground is a generated grass field with a faint glassy sheen, and every castle block is wrapped in a generated running-bond brick texture instead of flat stone color.
- **A bigger, fuller courtyard** — the curtain wall was pushed outward and the extra space filled in: a ruined chapel with a freestanding arch, a well, a graveyard, scattered rubble, dead trees, banners on the keep, and a climbable rampart stair up to the wall walk. All of it is destructible, same as the rest of the keep.
- **Distinct enemies** — Hollow One, Wraith, Brute, and Spitter now have four completely different silhouettes (not just recolored humanoids), each with its own movement animation and death collapse.
- **Reworked blade** — a proper falchion with a fuller, glowing edge, and cross-guard, replacing the old thin box. The swing is now a three-phase windup / slash / recover motion with a trailing arc effect, and the hit lands when the blade actually connects instead of on keypress.

## New in Update III — Gabriel Ascendant

- **A fully jointed boss rig** — Gabriel now has elbows, knees, a turning neck, and a five-segment flowing cape, all layered on top of his existing attack timings without changing a single one of them.
- **A 2× greatsword** — the blade is now nearly as tall as he is. A live shoulder/elbow compensation keeps its tip clear of the floor through every attack, including the overhead slam.
- **Bigger, brighter wings** — more feathers, a longer wingspan, and an additive glow layer that pulses with each flap and flares on attack frames.

## New in Update IV — What Waits Outside

- **Beyond the gate** — taking the crown (or killing his true form) no longer opens the gate onto nothing. A causeway leads out over the fog to a sunken final arena, and reaching the doorframe at its centre ends the run with a real END screen — kills, night reached, judges felled, and a line that differs depending on whether you took the crown or refused it.
- **The Warden** — a fifth enemy, first met in a three-strong gauntlet on the causeway and occasionally thereafter in the courtyard from Night IV on. Its raised shield makes its front immune to everything; flank it, or catch it mid-lunge with the blade to shatter its guard for good.
- **Options menu** — mouse sensitivity, master volume, and field of view, reachable from the title screen and the pause menu. Settings persist between sessions.

## New in Update V — The Second Judge

- **Duel mode** — a DUEL button on the title screen drops you straight into a 1v1 against either boss, no wave rush required. Pick your judge and go.
- **Boss: Moss, the Second Judge** — a player-scale purple angel, faster and more relentless than Gabriel. A chase-and-smash mace, a leap slam with a telegraphed landing ring, and a sweeping purple laser you have to run out of the arc of. Two phases (a 50% gate that speeds everything up), no wide chained openings — his recoveries are short. In a normal run he only descends once Gabriel has fallen and 70 souls have been freed; he opens the way out rather than dropping a crown.

## New in Update VI — A Score for the Keep

- **A real score** — a generative music engine (no samples, all synthesized) replaces the old single ambient drone. A slow, sparse exploration theme plays through the keep, and each boss has his own track — Gabriel a heavy ceremonial march, Moss a fast, driving pursuit — both audibly intensifying once the fight crosses its phase-2 gate.
- **Music volume** — a separate MUSIC slider in the options menu, alongside the existing master volume, sensitivity, and FOV. Persists between sessions.
- **Victory / defeat stings and a low-HP heartbeat** — a rising sting on a boss kill, a descending one on death, and a muffled heartbeat cue that kicks in when your health runs low.
- **Duel mode fixed and reworked** — finishing a boss in a duel no longer dumps you into the normal wave rush. It now ends on a real choice screen: rematch the same judge, switch to the other, or return to the title.
- **Cleaner screen transitions** — dying or clearing a run now returns you to the title screen instead of auto-restarting, and a couple of leftover-overlay bugs (a phantom duel screen on first load, a stuck pause overlay after a duel) are fixed.

## New in Update VII — The Descent

- **Roguelite relics** — every 2nd night, and after every judge felled, choose one of three stacking
  relics (faster dash, harder hits, a bigger scattergun spread, quicker Lance/JUDGEMENT cooldowns,
  more max vitality, lifesteal, a triple jump, and more). An acquired-relics HUD tracks your build;
  everything resets clean at the start of a new run.
- **The Gloom** — a new aerial enemy that hovers well above the courtyard, forcing you to look and
  shoot up, then telegraphs and dive-bombs before climbing back to altitude. Appears from Night III on.
- **Three built zones, not one courtyard** — a run now descends through three distinct hand-built
  levels: the Hollow Keep, a low-roofed and pillar-choked Crypt, and the Void Below — a shattered
  cathedral on floating stone over a real abyss (fall off and you're returned to solid ground, the
  hard way). Each has its own palette, hazards, and enemy mix. Felling a level's judge opens a
  glowing descent portal down to the next, instead of the old crown/gate ending.
- **Boss: Sable, the Third Judge** — a hulking, ground-bound void-armored judge closing out the Void
  Below. Slow and deliberate: a stomp shockwave, a ground eruption, and a pull-then-slam. Also
  playable in Duel mode alongside Gabriel and Moss.
- **Requiem** — the long-missing third weapon. A heavy breach cannon: slow, small blast radius,
  devastating up close. Unlocked permanently through the Shrine.
- **Meta-progression — the Shrine** — souls earned from a run are now banked, not just spent. Return
  to the title screen and visit the Shrine to spend them on permanent upgrades: unlock Requiem,
  extra starting vitality (stacks), or begin every run with a relic already in hand.

## Update VIII — Legible relics, and three guns that aren't the same gun

### Relic cards you can read at a glance

An offering used to be three paragraphs of prose. Now it is three cards:

- **An icon per relic** — 25 hand-drawn 24×24 stroke glyphs, generated in code like everything else
  in this game. No image files, no CDN, crisp at any size, and they recolour themselves.
- **A category chip** — OFFENSE, MOBILITY, SURVIVAL, SKILL or WEAPON, each with its own colour. The
  border, icon, chip and number on a card all share it, so you sort the offering by colour before
  you read a word.
- **The number, in big type** — `DASH REFILL −40%`, `+35% VS BOSSES`, `+3 HP PER KILL`. The prose
  moved to a small line underneath, where it belongs.
- **The same treatment in the Shrine**, where the big slot holds the price and the level (`◆ 245 — LV 3`).
- **The build HUD** carries the matching mini-icons, so you can see your run's shape at a glance.

### Three weapons, three jobs

The sidearm used to be the correct answer to almost every situation: same DPS as the scattergun, at
any range, with pinpoint accuracy and the best headshot. That's fixed — each gun now owns a band,
and its role is printed in the ammo HUD.

| | contact (3 m) | mid (10 m) | long (26 m) | notes |
|---|---|---|---|---|
| **SIDEARM** · precision | 129 | 129 | 129 | body shots; **514 on the head, at any range** |
| **SCATTERGUN** · close | **263** | 236 | 74 | range falloff from 8 m, floors at 28% past 22 m |
| **REQUIEM** · crowd | 100 | 100 | 100 | **280 against four**, and 2.2× guard damage |

- **Sidearm** — the lowest sustained body damage in the game and by far the highest headshot. It
  never falls off and it barely spreads, so range and aim are its whole identity. 14-round magazine.
- **Scattergun** — hits nearly twice as hard as anything else in your face and is close to useless
  across a courtyard. The self-knockback still makes it a movement tool.
- **Requiem** — worst single-target gun on the board and the best against a group, with a wider
  6-unit blast at 60% splash. Against a judge it deals **2.2× poise damage**: it opens a stagger for
  420 damage where the other two need ~700. It's the guard-breaker, not the DPS gun.

### Rounds you can see, and keys where you expect them

- **A magazine, not a number** — the ammo panel now draws one brass-tipped casing per round, sized
  to the weapon (slim for the sidearm, fat shells for the Requiem), sitting to the left of the
  count. Spent rounds hollow out; the last few burn red and pulse — four on the sidearm, two on the
  scattergun, the final shell on the Requiem. Reloading dims the whole strip.
- **Q casts JUDGEMENT, R reloads.** E is still the Spectral Lance.
### The Wraith and the Gloom, rebuilt

The animation fixes below were real but they were polish on top of two bodies that didn't read as
creatures at all. Rendered in isolation the Wraith was a **black plank** — a 0.4-wide slab with two
0.09-thick sticks for arms and a cloak hinged at its feet — and the Gloom was a **flat purple
board**: two 0.06-thick plates that vanished edge-on. Both are rebuilt:

- **The Wraith is hollow.** A wraith with a torso is just another cultist, and the roster already
  has three solid humanoids. There is no body in the robe: an open cowl shell with nothing inside
  it but two coals, rags hanging where a chest should be, small claws on the ends of empty sleeves,
  and no legs. It is also **the only thing in the game you can see the courtyard through** — it
  rests at 62% opacity, which reads as a ghost from across the yard before you can make out a
  single shape. Every fade (the blink, the death dissolve) multiplies against that resting
  transparency instead of resetting it to solid.
- **The Gloom** is built to read from underneath, which is where you actually see it. Each wing is a
  hinged Group — inner spar, swept outer spar on its own elbow, membrane, tip claw — over a compact
  body with a long trailing tail and a pair of hanging talons. The outer wing trails the inner by a
  beat, so it strokes rather than waggles.
- **The blink is a vanishing act**, not a pop: the robe fades as the shape collapses to nothing on an
  eased curve, it spins up as it unravels, the eyes stay lit to the last frame, and it **arrives
  facing you**.
- **The dive is a stoop**: it rears back on the telegraph, pitches nose-down through the pass with
  the wings swept and the talons out, then levels off as it climbs.

### Dash audit — the mechanic is fine, one relic was broken

Checked the dash system end to end. The **core mechanic needs nothing**: three charges refilling
over 0.9s each (2.7s for a full reload, 0.54s with BLOODLUST), momentum-preserving so a dash never
slows a faster approach, 0.16s of i-frames baked in, dash speed 2× your run. That's a modern dash
and it plays right.

The four dash relics (BLOODLUST, GHOSTSTEP, PHANTOM DASH, HOLLOW RESURGENCE) aren't redundant with
each other either — they're a coherent dash-melee lane (uptime + damage + refresh-on-kill +
survivability), so removing them would delete a build, not trim fat. But the audit found the lane's
offensive node was **broken**:

- **PHANTOM DASH almost never connected.** Its hit check measured full 3D distance from
  `player.pos` (head height, ~1.8) to a monster's feet (y 0), so the 2-unit threshold collapsed to
  **0.87 units of real horizontal reach** — you had to dash through the enemy's centre, in a window
  you cross in two frames. In a live 15-second test it landed **zero** hits. Fixed to measure
  horizontal distance only (2.2u reach), exactly how the blade already does it. Base bumped 40 → 60,
  and it scales with damage relics (78 with EXECUTIONER, 90 with GLASS CANNON) — so the dash-melee
  build is finally real: one-shots the Wraith, chips the Brute.

### RICOCHET, and offers that lean toward your build

The Spectral Lance's base is deliberately left where it is — a 42-damage utility poke on a 5s
cooldown. What was weak wasn't the ceiling of an E build (a full one already measured 128–167 DPS);
it was that the build almost never came together, because the three lance relics arrived at random.
Two changes fix that:

- **RICOCHET** *(new lance relic)* — the Spectral Lance rebounds off walls twice, resetting its
  hit-set on each bounce so it carves the same bodies again on the way back. In the open it's a
  small bonus; in the pillar-choked Crypt it's a room-clear. It raises the E build's ceiling without
  touching the base.
- **VOLATILE LANCE reworked** — it used to blow up on the *first* body, which killed the pierce that
  is the lance's whole identity, so it was a weak pick. Now the lance pierces the full line as
  always **and** detonates for a blast among the bodies it carved (and against the wall a RICOCHET
  bounce leaves it on). Measured: pierces all 5 in a line, +40 AoE on the cluster.
- **Synergy-weighted offers, for every build** — each relic belongs to a lane (lance, ult, blade,
  low-HP, gun, dash, guard; EXECUTIONER and GIANT SLAYER stay laneless universal picks). Each relic
  you own in a lane adds **0.45** to a same-lane card's draw weight, so a build leans together over a
  run. Kept deliberately light so you can still pivot: with two lance relics, lance cards show in
  ~64% of offers (up from ~51%) — a nudge, not a rail. Applies to dash, gun, every lane alike; crowns
  are drawn flat.

### Keystones — the pool now has build doors

An audit of all 24 relics turned up the real structural problem: **not one of them read your
build.** Every relic was a flat, standalone knob, so three mobility relics gave you three unrelated
small effects rather than a *Dasher*. Three dead nodes are gone, replaced by the pool's first three
**keystones** — relics whose power comes from a system you're already running:

- **BLOOD PACT** *(the low-health door — replaces BLOODRUSH)* — below half vitality you deal +45%
  damage, and every kill claws back 10 vitality. It turns the two relics that push you low
  (GLASS CANNON, BERSERKER'S PACT) from a death sentence into a loop. Stacks with berserker to
  ×2.15 at 20% health.
- **WAR RHYTHM** *(the blade door — replaces SOUL LEECH)* — every landed blade hit sharpens the
  next, up to +72%, lost the instant the chain drops. A Duelist who lives in melee ramps the
  finisher from 90 to 144. A whiff dulls the edge back to nothing.
- **OVERCHARGE** *(the caster door — replaces SCAVENGER)* — every shot that hits flesh takes 0.2s
  off both the Lance and JUDGEMENT. It snowballs with the six skill relics you were already
  clustering, and one trigger pull of the scattergun is one refund, not eight.

Why these three replacements specifically: **SOUL LEECH** and **SANGUINE RITE** were two
"heal-on-X" relics that both measured **+0 hp/min** now the blade finisher heals — one was
redundant. **BLOODRUSH** was pure feel, measured ×1.00, and fought HOLLOW RESURGENCE for the
on-kill slot. **SCAVENGER** was near-dead against a 14-round sidearm. All three were the pool's
weakest nodes; each is now the anchor of a build.

### Crowns — a judge should not pay out like night two

Felling a judge drew from exactly the same relic pool as clearing twelve hollows. It doesn't any
more. A judge now offers three **Crowns**: a separate tier that never appears in the nightly pool,
never repeats, and changes how one of your systems behaves rather than nudging a number. The
screen changes with it — gold, and it says *A JUDGE HAS FALLEN*.

| Crown | What it does |
|---|---|
| **EXECUTIONER'S CROWN** | Any hit that leaves a foe under 25% health kills it outright. Judges are immune. |
| **THE HOLLOW CROWN** | Two charges of JUDGEMENT, recharging one after the other. |
| **CROWN OF EMBERS** | The blade finisher leaves a burning ring — 26 a tick for four seconds, and it never burns you. |
| **CROWN OF THORNS** | A quarter less damage taken, and 60% of what does land goes back into whatever landed it. |
| **THE TURNING CROWN** | Every blade you turn out of the air takes 10s off JUDGEMENT and 4s off the Lance. |
| **CROWN OF THE STARVED** | Every kill takes 0.6s off every cooldown you're holding. |

Once all six are on your head a judge falls back to the ordinary pool.

### What the relic audit turned up

Measured all 24 relics against a fixed rotation (sidearm + blade + E + Q) on a live scene:

- **The spread was extreme for one rarity.** GLASS CANNON ×1.50 and EXECUTIONER ×1.30 sat in the
  same pool, at the same odds, as a dozen relics that measured ×1.00.
- **FEATHERFALL was a dead pick the second time it appeared** — it assigned `maxJumps = 3` rather
  than incrementing, and it wasn't marked unique, so a second copy did literally nothing. It stacks
  now, to a ceiling of five.
- **HAIR TRIGGER measured ×1.08** against EXECUTIONER's ×1.30 for the same slot. Raised to −38%
  between shots (×1.61 fire rate).
- **The healing relics are quieter than they look** now the blade finisher returns vitality — at
  50% health carving a pack, the baseline already caps out before SANGUINE RITE or SOUL LEECH adds
  anything. They still matter for a gun-only build, so they stay as they are.
- A first pass measured HAIR TRIGGER at ×0.76 — *worse* than nothing. That was the harness, not the
  relic: it fired without ever letting recoil recover, so a faster gun just climbed off target
  sooner.

### The blade is worth drawing now

It was one 45-damage swing on a 0.5s timer — **90 DPS at knife range against a sidearm that does
129 from anywhere**. There was no reason to ever close. It owns close quarters now, through a
chain rather than a bigger number:

- **Three-hit chain** — 45 → 58 → 90, each step reaching further and cutting a wider arc. The
  third is a **finisher**: a full sweep all the way around you, heavy knockback, gold trail.
- **Kills buy back the recovery.** A killing blow cuts 70% off the remaining cooldown, so a good
  player carves through a pack instead of waiting out a timer between each body — 47 swings a
  minute becomes 75.
- **The finisher heals you** — 4 vitality per enemy caught, up to 12. It is the only thing in the
  kit that pays you for standing in the middle of a pack, and it caps at 8 HP/sec against three or
  more, which is roughly what the horde takes off you. Risk breaks even; it isn't a fountain.
- **A parry hands the swing straight back** — deflecting anything (a judge's sword *or* a Spitter
  orb) refunds the cooldown entirely and advances the chain. Turn his steel, then finish him.
- **A whiff drops the chain**, and it goes cold on its own after 1.4 seconds.

| | DPS |
|---|---|
| 1 target | **154** (was 90) |
| 3 targets in the arc | 463 |
| a real 4-strong pack, kill refunds firing | 600 |

Which slots it correctly: above the sidearm's body shots (129), below the scattergun at contact
(263), far below a headshot chain (514) — and the best crowd damage in the game, at the range
where the crowd can hit back. Against a judge the chain is 60 / 78 / 118.

### The Spitter owns a mechanic now

It was the only archetype without one — a walking turret that backed away and lobbed a single
leading orb. It's the area-denial enemy now: the one that takes ground off you instead of coming
at you.

- **Mortar, from Night IV** — every third shot is lobbed instead of thrown: a ring on the ground
  where you're heading, a full second of warning, a visible arc, then an impact that only bites
  inside 3 units and **leaves a patch of acid for 3 seconds** (6 a tick, twice a second).
- **It replaces the direct shot, never adds to it**, and costs a longer reload. This is a change of
  texture, not a new damage source.
- **A telegraph you can read across the courtyard** — the charge now runs over a full 0.7s: the gut
  swells and burns brighter, the maw cranks open, and for a mortar the arms go overhead instead of
  forward, so you can tell which shot is coming before it leaves.
- **Rebuilt to carry that on its silhouette** — a bloated body with an exposed glowing sac between
  stacked gut plates, a wide forward maw, long thin arms, and splayed frog legs. It no longer reads
  as a third hunched humanoid with a bead on its chest.

Measured against one mortar every 3.5 seconds for a minute:

| what the player does | damage per mortar |
|---|---|
| never moves | 49 |
| wanders, ignores the ring | 14 |
| **steps off the ring** | **0** |

That's the shape it should have: fully avoidable if you read it, steeply punishing if you camp.

**The Wraith is smaller too** — scale 1.00 → 0.84. At 1.73 × 0.49 it's the slightest thing in the
roster by a wide margin (the Hollow is 2.70 × 1.18, the Brute 3.53 × 3.11), which suits something
you're meant to lose track of.

### The animation faults underneath



Both hovering types shared a melee windup written for something with arms, and only ever wrote
their altitude from the walk cycle — so the moment they did anything else, they broke:

- **The Gloom's wings were rolled about their own length.** The shared attack swing drove
  `rotation.x` on limbs that hinge on `rotation.z`, and nothing ever cleared it — one attack and
  the wings stayed twisted for the rest of that monster's life. It has its own windup now: it
  folds the wings and **stoops onto you from altitude**, then rides back up.
- **Hover was only maintained while walking.** Attacking froze the bob mid-cycle, and the Wraith's
  blink telegraph slammed it from its hover to the floor on the tell's first frame. One
  `restHoverY()` now owns rest altitude in every state.
- **The blink read as a bug, not a teleport.** It shrank to a visible quarter-size doll and popped.
  It now collapses to nothing on an eased curve, spins up as it goes, keeps its eyes lit to the
  last frame, and **arrives facing you**.
- **Dying mid-blink left a 3%-scale corpse.** Death normalises scale and altitude once, whatever
  state it was interrupted in.
- **The Gloom spawned on the floor** and snapped 4.2 units into the air on its first animated
  frame; it arrives at altitude. Its dive now launches from its real height and its climb converges
  onto the live bob instead of a bare constant, so the hand-off back to flight doesn't pop.
- **It was blocked by rubble it was flying four units above** — anything above 2.4 units ignores
  the waist-high collision band, and collides again the moment a dive brings it down.

Measured over 30-second traces: the worst single-frame altitude change is now 0.60 for the Gloom
(inside its 22 u/s dive, where it belongs) and 1.40 for the Wraith (the teleport itself). Nothing
pops on a state transition, and death from any state leaves a full-size body.

### Other

- **The offering won't eat your trigger finger.** The relic screen interrupts a firefight, so the
  cards arrive faded and **refuse input for half a second**, with a sweep under the subtitle
  showing when they go live. A pick also spends the offer, so a double-click can't take two.
- **Waves arrive from nearby doors.** The spawner used to sort its points *farthest-first*, so every
  wave came from the two 90-unit corners while 25-unit doorways sat unused and each night opened
  with a long walk. It now picks from a near band (15–38 units), shuffled so the same entrance
  doesn't feed every wave. Average spawn distance drops **90 → 25 units**; nothing spawns inside
  geometry or within 10 units of you.
