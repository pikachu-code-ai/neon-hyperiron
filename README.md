# 🚀 NEON HYPERION — Cyberpunk Bullet-Hell Arcade SHMUP

A high-intensity, single-file 60 FPS cyberpunk bullet-hell shoot-'em-up built with HTML5 Canvas, Vanilla JavaScript, Tailwind CSS, and procedural Web Audio synthesis. Thread dense neon bullet curtains with a pinpoint **4px Quantum Core**, chain up to a **16X Bullet Graze Combo**, evolve your cannons across **6 weapon tiers**, unleash **Rainbow Hyper Overdrive**, and conquer **3-Phase Transforming Dreadnought Bosses**!

---

## ✨ Key Features

* **Precision `4px` Quantum Core & Focus Mode:** Hold `Shift` (or `Right-Click` / mobile **Hold Focus**) to cut thruster velocity in half for micro-dodging, tightening Option Drone formations forward and illuminating your exact **`4px` Quantum Core** hitbox and **`28px` Graze Field**.
* **Bullet Graze System (Up to `16X` Combo):** Skimming within `28px` of enemy projectiles without taking a core hit arcs cyan-magenta lightning, triggers rising harmonic synth ticks, awards `+100` base points per bullet grazed, builds up to a **16X Score Multiplier** (`3.5s` decay window), and charges **+4% HYPER OVERDRIVE**.
* **7-Second Rainbow Hyper Overdrive:** At `100%` charge, detonate a screen-wide **Quantum Nova Shockwave** that converts every active enemy bullet into magnetic score crystals (`+250` each) and activates **7.0 seconds** of Rainbow Overdrive (`2.15x` fire rate, `2x` score multiplier, `4` Option Drones, and full hull invulnerability).
* **Hull Shields & Emergency EMP Pulse:** Start with **4 Hull Shields** (expandable up to **5**). Taking damage triggers `1.4s` of invulnerability and fires a `240px` Emergency EMP Pulse that vaporizes surrounding bullets and blasts enemies back so you never get cornered.
* **Locked 60 FPS Zero-GC Engine:** Built with an offscreen pre-rendered glow sprite cache, fixed-size swap-and-pop object pools (`260` player bolts, `450` enemy bullets, `300` particles, `140` crystals, `32` popups), AABB early-out collision checks, a `1.5` DPR cap, and dirty-flagged HUD updates for smooth performance even during intense Phase III Boss curtains.

---

## ⚡ Stackable Weapon Tiers & 7 Power-Up Capsules

### Main Cannon Evolution (`WPN+`)
Collecting **`WPN+`** capsules permanently upgrades your primary armament from **LV 1** to **LV 6 HYPER-VOLLEY**:
* **LV 1–2:** Twin Cyber-Pulse Cannons & Center Heavy Piercing Rail-Lance
* **LV 3–4:** 4-Way Spread Fan + High-Velocity Piercing Center Rail
* **LV 5:** Twin Heavy Piercing Rails + 4-Way Wide Plasma Fan
* **LV 6 HYPER-VOLLEY:** **7-Way Storm + Twin Heavy Piercing Rails** *(Collecting `WPN+` at MAX awards `+5,000` Overcharge points and `+25%` Hyper charge)*

### Tactical Power-Up Capsules
| Capsule | Code | Duration | Combat Effect |
| :--- | :--- | :--- | :--- |
| **Option Drones** | `DRONE` | `11.0s` | Deploys up to **4 autonomous flanking pods** firing synchronized lime-plasma lasers (tightens forward in Focus Mode). |
| **Omega Rail-Beam** | `BEAM` | `8.0s` | Projects a continuous screen-piercing hyper-laser that melts enemy waves and Boss armor. |
| **Swarm Seekers** | `SEEK` | `9.0s` | Launches continuous salvos of homing micro-missiles with glowing magenta trails. |
| **Aegis Phase Shield** | `SHLD` | `+1` & `8.0s` | Restores **+1 Hull Shield** (up to 5 max) and projects a `34px` green barrier that converts touching bullets into crystals and blocks one hit. |
| **Chrono Stasis** | `SLOW` | `7.0s` | Dilates combat time, slowing all enemy ships, patterns, and incoming projectiles by **55%**. |
| **Quantum Nova** | `NOVA` | Instant | Unleashes a `480px` shockwave converting bullets to crystals, damaging nearby foes, and granting **+35% Hyper charge**. |

---

## 👾 Hostile Archetypes & 3-Phase Dreadnought Bosses

### Enemy Squadron
* **Crimson Dart (`#ff1e56`):** Sine-weaving fast interceptors firing aimed plasma orbs.
* **Amber Turret (`#ffaa00`):** Rotating octagonal gunships unleashing expanding spiral bullet rings.
* **Violet Splitter (`#a855f7`):** Diamond cruisers that fracture into **two high-speed Strikers** when destroyed.
* **Cyan Sniper (`#00f3ff`):** Locks a `0.85s` telegraphed dashed laser sightline before firing high-velocity needle darts.
* **Emerald Carrier (`#00ff66`):** Armored hexagonal supply escorts that drop guaranteed Power-Up Capsules upon destruction.

### 3-Phase Transforming Dreadnought Bosses
At the end of every Sector, face rotating **Dreadnought Bosses** (*Hyperion Dreadnought*, *Omega Seraph*, *Void Leviathan*, *Apex Singularity*, *Chronos Valkyrie*) featuring health-bar phase markers and mid-battle transformations:
1. **Phase I (`100% – 65%` HP) — Armored Winged Core:** Counter-rotating outer reactor ring, multi-arm spiral flower curtains, and geometric ring bursts.
2. **Phase II (`65% – 30%` HP) — Twin-Ring Accelerator:** Converts active bullets into crystals, deploys an inner counter-rotating ring, and fires **telegraphed twin sweeping laser cannons**.
3. **Phase III (`30% – 0%` HP) — Unbound Omega Core:** Maximum reactor rotation speed, 6-arm spiral curtains, rapid ring bursts, and accelerated twin sweep lasers.

---

## 🎮 Controls

### Desktop
| Action | Keys / Input |
| :--- | :--- |
| **Pilot Interceptor** | `W` `A` `S` `D` or `Arrow Keys` (Auto-Fire is always active) |
| **Focus Mode (`4px` Core)** | Hold `Shift` or `Right-Click` (or click `FOCUS [SHIFT]` on HUD to toggle) |
| **Hyper Overdrive (`100%`)** | `Space`, `E`, `X`, or `Enter` (or click the HUD `HYPER` gauge) |
| **Pause / Resume** | `P` or `Esc` |
| **Mute / Unmute SFX** | `M` (or click `SFX` on HUD) |

### Mobile & Touch Devices
* **Touch-Drag Piloting:** Touch and drag anywhere on the screen to fly smoothly (your ship automatically offsets above your fingertip for clear visibility).
* **Tactile Bottom Pads:** Hold the bottom-left **`HOLD FOCUS (4PX CORE)`** button for precision micro-dodging, and tap the bottom-right **`HYPER`** button when charged to `100%`.

---

## 🚀 Getting Started

**NEON HYPERION** is completely self-contained in a single HTML file with zero build steps or external audio/image assets:

1. Save or download the game file as `neon_hyperion.html`.
2. Open `neon_hyperion.html` in any modern desktop or mobile web browser.
3. Click **▶ INITIATE LAUNCH** (or press `Space` / `Enter`) to launch into Sector 1.
