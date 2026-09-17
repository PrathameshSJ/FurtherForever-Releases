# Further Forever (tpp-3) — Official Game & Strategy Guide

Welcome to **Further Forever**, an epic third-person action RPG set across spherical planetoids with 360-degree curvature physics, real-time celestial transitions, dynamic cinematic cutscenes, and colossi boss battles.

---

## Table of Contents
1. [The Story](#the-story)
2. [Game Overview & Core Mechanics](#game-overview--core-mechanics)
3. [Complete Controls & Keybindings](#complete-controls--keybindings)
4. [Equipment, Inventory & Altar Transmutation](#equipment-inventory--altar-transmutation)
5. [Combat Skills & Mechanics](#combat-skills--mechanics)
6. [Boss Strategy Guide: Tips & Secret Tricks](#boss-strategy-guide-tips--secret-tricks)
7. [Realm Progression & Dual Portals](#realm-progression--dual-portals)
8. [Credits & Third-Party Attribution](#credits--third-party-attribution)

---

## The Story

In the tranquil, secluded medieval settlement nestled at the North Pole of Level 0, a young boy uncovers an ancient chest inside his master's cottage. Upon opening it, the blade within springs to life—singing eccentric tunes, shouting in alarm, and conversing with sentient wisdom. It is the **Cylinder Blade**, a legendary burning sword tied to primordial forces.

The village Master reveals the prophecy: four celestial realms hang suspended in the cosmos, each guarded by a primordial Colossus. By braving the celestial Bifrost portals, felling each guardian, and offering their monster cores to the ancient Angel Altars, the boy can forge divine armor, uncover the secrets of the shattered cosmos, and ascend to the celestial plane at the North Pole Altar.

---

## Game Overview & Core Mechanics

- **Spherical Planetoid Gravity**: You walk on true 3D spherical planets (60m–90m radius). Gravity pulls directly toward the planet center, allowing full 360° locomotion across poles and horizons without falling off.
- **Dynamic Navigation System**:
  - **Rotating Mini-Globe**: Bottom-right HUD sphere displays player orientation and real-time landmark pins.
  - **Ribbon Compass**: Top of screen shows headings and quest objective icons.
  - **Perimeter-Clamped Objective Markers**: Golden diamonds highlight active targets with pulsating proximity alarms.
- **Dynamic Camera Modes**: Seamless switching between instantaneous 1:1 mouse tracking, dampened cinematic follow, and heading-aligned action chase camera.
- **Cinematic Cutscenes**: Integrated scripted sequences with dynamic letterboxing, camera sweeping, subtitles, and dialogue.

---

## Complete Controls & Keybindings

| Input | Action | In-Depth Description |
| :--- | :--- | :--- |
| **W, A, S, D** | **Locomotion** | Move forward, backward, strafe left, and strafe right. Movement is calculated tangent to the planetoid sphere relative to camera heading. |
| **Space** | **Jump** | Leap off the spherical terrain. Features authentic multi-phase jump physics (`jump_start`, in-air hang, and smooth momentum landing). |
| **Shift** (Hold) | **Sprint** | Dash across the terrain at high speed (9 m/s). Essential for dodging large area attacks and boss gap closing. |
| **LMB** (Left Click) | **Attack / Confirm** | Perform a sword strike. Chains into an alternating 2-hit combo (Slash 1 &rarr; Slash 2). While moving, your hero turns toward the camera forward for the swing and returns seamlessly to movement. Recaptures mouse cursor when clicked in-game. |
| **3** | **Crescent Moon Slash (Skill)** | Activates the Crescent Moon skill for 5 seconds. Shifts the camera to an over-the-shoulder third-person aiming view and ignites the blade with flipbook flames. Pressing **LMB** fires high-speed radiant crescent energy projectiles that pierce through the air along planet curvature. (3.0s cooldown). |
| **1** | **Health Potion** | Consumes 1 Health Potion from your hotbar to instantly restore your HP back to 100% full health. Stackable up to 5 per chest. |
| **E** / **Tab** / **I** | **Inventory & Paperdoll** | Opens the sleek RPG inventory menu, showing your 3-slot backpack, interactive Angel Altar slot, and a real-time 3D Paperdoll displaying your currently equipped gear. |
| **F** | **Primary Interact** | Interact with chests, NPCs, altars, and Bifrost portals. |
| **Q, 2, R, X** | **Secondary Interact** | Dynamic contextual interaction keys. When multiple interactables are in close proximity (e.g., dual return/forward portals), secondary keys are automatically assigned to prevent input overlap. |
| **C** | **Cycle Camera Mode** | Toggles between **Free Orbit** (1:1 mouse control), **Smooth Follow** (cinematic inertia), and **Action Chase** (auto-aligning heading). |
| **Mouse Motion** | **Look / Aim** | 360-degree free orbit around the character. During idle, looking around does not force the character's body to turn. |
| **ESC** | **Menu / Pause / Skip** | Opens the settings and pause overlay. During skippable cutscenes, instantly skips to gameplay. |
| **Space / RMB** | **Skip Cutscene** | Secondary shortcuts to skip active dialogue or cutscenes. |

---

## Equipment, Inventory & Altar Transmutation

Your backpack has a 3-slot capacity, alongside dedicated equipment slots that visually equip armor pieces directly onto your character model in real time:

- **Cylinder Blade (Burning Sword)**:
  - *Base Weapon*: 65.0 base damage per strike.
  - Ignites with flipbook flame geometry when Crescent Skill is engaged.
- **Iron Helm (Head Armor)**:
  - *Base Defense*: 10% damage reduction.
  - *Special Effect*: Critical defense against aerial crushing blows (reduces Boss 2's Sky Slam damage from 35.0 down to 5.0).
- **Iron Vest (Torso Armor)**:
  - *Base Defense*: 25% damage reduction against all incoming melee and elemental attacks.
  - *Special Effect*: Vital protection against lingering magma damage in Realm 3.
- **Kite Shield (Off-Hand Armor)**:
  - *Base Defense*: 15% defense rating.
  - *Special Effect*: Complete damage immunity / projectile deflection while held.
- **Monster Cores**:
  - Primordial essences dropped on the ground when defeating Realm bosses:
    - Realm 1: **Heart of Verdure** (`monster_core_verdant`)
    - Realm 2: **Abyssal Heart** (`monster_core_abyssal`)
    - Realm 3: **Pyroclast Heart** (`monster_core_pyroclast`)
    - Realm 4: **Astral Core** (`monster_core_azure`)
- **Angel Altar Transmutation**:
  - Monster cores remain dormant in their native realm. Transport them through the portal to the next realm's Angel Altar:
    - Realm 2 Altar + Heart of Verdure &rarr; **Iron Helm**
    - Realm 3 Altar + Abyssal Heart &rarr; **Iron Vest**
    - Realm 4 Altar + Pyroclast Heart &rarr; **Kite Shield**
    - Realm 1 / Level 0 Altar + Astral Core &rarr; **Seraph Feather** (Endgame Relic)

---

## Combat Skills & Mechanics

### Crescent Moon Slash (Key '3')
1. Press **3** when facing tough enemies or distant bosses.
2. The camera smoothly zooms into a right-shoulder over-the-shoulder aim perspective.
3. Your blade ignites with animated fire meshes.
4. Left-click (**LMB**) to unleash searing crescent arc projectiles that travel along the spherical horizon, hitting targets far beyond melee range.
5. Lasts for **5.0 seconds** followed by a brief **3.0-second cooldown**.

### Decoupled Combat Movement
- While idle, moving your mouse orbits your camera freely without turning your character.
- Pressing movement keys directs your character along the camera's tangent vector.
- Striking (**LMB**) locks your swing forward toward the camera aim. If you attack while strafing sideways, your character swings toward the crosshair, then immediately resumes sideways locomotion once the slash completes.

---

## Boss Strategy Guide: Tips & Secret Tricks

### Boss 1: Sylvan Goliath (Realm 1 — Verdant Planetoid)
- **Health**: 1,200 HP | **Cooldown**: 3.2s
- **Spawns**: Bursts from the soil 3 seconds after you reach the realm.
- **Attacks**:
  - *Root Quake*: Sends shockwaves through the earth within 6m (15 dmg + launch).
  - *Boulder Slam*: Smashes the earth with colossal stone fists within 7m (20 dmg + heavy launch).
- **Pro Tips & Tricks**:
  - Sylvan Goliath attacks in combos of 3 to 4 abilities, followed by an exhaustive cooldown of 3.0–4.0 seconds. Bait his two ground slams by sprint-strafing in a circle, then rush in and unleash your full attack combo during his recovery pause.
  - *Crucial*: After defeating him, open the reward chest for 5 Health Potions, and **pick up the Heart of Verdure (`monster_core_verdant`) resting on the ground** before entering the portal!

---

### Boss 2: Abyssal Colossus (Realm 2 — Misty Planetoid)
- **Health**: 1,000 HP | **Cooldown**: 3.5s
- **Spawns**: Descends from the high atmosphere with orbiting crystal wards.
- **Attacks**:
  - *Abyssal Shockwave*: Pulses crystal energy in a wide arc (18 dmg).
  - *Sky Slam*: Leaps 22 meters into the upper sky, tracks your exact coordinates, and plummets straight down onto your head!
- **SECRET TRICK (The Helmet Rule)**:
  - **Do NOT fight Boss 2 without crafting your helmet!**
  - Boss 2's *Sky Slam* lands directly on top of your character's skull. Without a helmet, it inflicts a crushing **35.0 damage** and blasts you far into orbit.
  - *What to do*: Before engaging, visit the Angel Altar and transmute the **Heart of Verdure** you brought from Realm 1. This crafts the **Iron Helm**.
  - When the Iron Helm is equipped on your head, it absorbs the impact of the falling colossus: damage drops from **35.0 down to a mere 5.0**, and knockback is neutralized!

---

### Boss 3: Pyroclast Behemoth (Realm 3 — Crimson Planet with Moons)
- **Health**: 1,500 HP | **Cooldown**: 3.6s
- **Spawns**: Bursts out from the volcanic crust with fiery shockwaves.
- **Attacks**:
  - *Magma Burst*: Erupts lava jets from shoulder spires.
  - *Phase 2 Rage (Triggered at &le; 50% HP)*:
    - The Behemoth collapses to the earth, then revives in a berserk fury.
    - Fiery fissures tear open across the planet surface.
    - His carapace cracks leak blazing magma, dealing **5.0 fire damage per second to anyone within 9.5m**.
    - Rains **8 falling meteorites** from the cosmos that impact the sphere with red warning decals.
- **SECRET TRICK (Ranged Kite & Armor)**:
  - *Craft the Vest First*: Transmute the **Abyssal Heart** from Realm 2 at the altar into the **Iron Vest** (25% damage reduction).
  - *Do NOT Melee in Phase 2*: The moment Phase 2 begins, sprint away from the 9.5m fire leakage zone. Engaging in close melee will burn your health bar rapidly.
  - Instead, press **3** to trigger **Crescent Moon Slash**. Kite the Behemoth around the planet curve and bombard him with crescent projectiles from a safe distance while dodging the red meteor impact craters.

---

### Boss 4: Azure Seraph (Realm 4 — Celestial Blue Realm)
- **Health**: 1,800 HP &times; 2 Phases | **Cooldown**: 3.2s
- **Spawns**: Rests dormant with folded wings at the center of the azure sphere until approached.
- **Attacks**:
  - *Starfall Barrage*: Summons radiant blue star shards from orbit.
  - *Warden Beam*: Rings spin at 4.5&times; speed while charging for 3.0s, then fires a colossal **350-meter radiant death ray** that curves along the spherical horizon!
  - *Phase 2 Full Revival*: Upon reaching 0 HP, releases a massive 20m shockwave, shatters the entire planet with radiant cyan fissures, and **fully heals back to 100% HP (1800 HP)**!
- **SECRET TRICK (Tangential Sprint & Kite Shield)**:
  - *Craft the Kite Shield*: Transmute the **Pyroclast Heart** at the altar into the **Kite Shield**.
  - The *Warden Beam* cannot be outrun backward due to its 350m range and spherical curvature. When you see the dual gyroscopic halos spinning rapidly and particles charging, sprint **perpendicularly (tangentially) around the planet curve** to rotate out of the beam's aiming cone, or hold your ground behind your shield.
  - Preserve your **Health Potions** (press **1**) and keep your skill ready for Phase 2—the battle effectively has 3,600 total boss HP.

---

## Realm Progression & Dual Portals

1. **Bifrost Scorch Marks**: When a boss dies, a Thor-style Bifrost runic scorch mark burns into the surface, and a rising crystal `RealmPillar` appears.
2. **Dual Portals System**:
   - As you defeat guardians, both **Forward Portals** (leading to the next realm) and **Return Portals** (leading back to earlier realms) will coexist.
   - If the next boss is alive, the objective marker points you directly to the forward portal.
   - If the next boss is dead, objective markers guide you to both portals, allowing complete backtracking to collect missed cores or craft items.
3. **The Celestial Altar Victory**:
   - Defeat Boss 4 &rarr; collect the **Astral Core** &rarr; transmute it into the **Seraph Feather** at the Angel Altar.
   - Journey back through the portals to **Realm 1 / Realm 0**.
   - Place the Seraph Feather onto the **Celestial Altar** at the North Pole to trigger the final ascension cutscene and complete the game!

---

## Credits & Third-Party Attribution

This project is made possible through open-source software and creative community assets under permissive licenses:

- **Character Model**: "Boy" by **jetsu** ([Sketchfab](https://sketchfab.com/3d-models/boy-528bcfc73ba94870ac8e7164a36b5c41)), licensed under [CC-BY-4.0](http://creativecommons.org/licenses/by/4.0/).
- **Weapon Model & Texture**: "Burning Sword" by **atomtwist** ([Sketchfab](https://skfb.ly/67vyX)), licensed under [CC BY-NC-SA 4.0](http://creativecommons.org/licenses/by-nc-sa/4.0/).
- **Equipment Models**:
  - "Armor Metal" by **Quaternius** ([Poly Pizza](https://poly.pizza/m/TMUoxILh9w)) — CC0.
  - "Shield" by **Quaternius** ([quaternius.com](https://quaternius.com)) — CC0.
  - "Helmet" by **samflorencio** — Creative Commons Attribution (CC-BY).
- **Environment & Textures**:
  - "Prototype Textures 1.0" by **Kenney** ([kenney.nl](https://kenney.nl)) — [CC0 1.0 Universal](http://creativecommons.org/publicdomain/zero/1.0/).
  - "Low Poly Trees Collection" — CC0 / Public Domain.
- **Engine & Plugins**:
  - **Godot Engine 4** ([godotengine.org](https://godotengine.org)) — MIT License.
  - "Script Dock" Editor Plugin by **GBInFlames** — MIT License.

For detailed legal notices, see [`license.txt`](file:///D:/DOLD/Godot_Engine/Godot_Games/videogame3-PRIVATE%20-%20Copy/license.txt).
