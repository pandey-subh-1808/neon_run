# ⚡ NEON DRIFT

A fast-paced, single-file 3D perspective arcade game built with vanilla HTML5 Canvas, CSS, and the Web Audio API. Dodge rhythm-synced barriers, collect energy orbs, race your personal ghost, and challenge friends using shareable run codes—with zero dependencies and no backend required.

---

## 🎮 Gameplay & Features

- **One-Tap & Keyboard Controls:** Tap the left/right sides of the screen (or center to cycle) on mobile, or use `Space`, `A`/`D`, or `Arrow Keys` on desktop.
- **Procedural Synthwave Audio:** Real-time basslines, kick drums, and sound effects generated natively via the **Web Audio API**—no external `.mp3` or `.wav` files required.
- **Rhythm-Synced Obstacles:** Barriers and orbs spawn on the beat, escalating in velocity the longer you survive.
- **Ghost Racing:** Your personal best run is recorded locally and replayed as a translucent ghost ball so you can race against your past self.
- **Daily Seed Challenge:** Uses a deterministic date-seeded PRNG (`Mulberry32`) so every player gets the exact same obstacle layout each day.
- **Zero-Backend Friend Challenges:** Encodes your run seed, score, and movement replay into a compact `ND-...` share code that friends can paste to race your ghost directly.
- **Near-Miss & Combo System:** Grazing past obstacles in adjacent lanes boosts your score multiplier up to **10x**.
- **Power-Ups:**
  - **Shield:** Absorbs a single barrier collision.
  - **Time Warp (Slow-Mo):** Temporarily slows track velocity for tight maneuvers.
  - **Magnet:** Pulls nearby orbs into your lane automatically.
- **Unlockable Visual Themes:** Unlock **Sunset** (500 pts), **Matrix** (1,500 pts), and **Retro GB** (3,000 pts) palettes saved via `localStorage`.

---

## 🚀 Quick Start (GitHub Pages)

Because the entire game lives inside a single `index.html` file, deploying it takes less than a minute:

1. Create a new repository on GitHub and upload `index.html` to the root directory.
2. Go to **Settings → Pages** in your repository.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`, select `main` (or `master`) and `/ (root)`, then click **Save**.
4. Your live arcade link will be ready at `https://<your-username>.github.io/<repo-name>/`.

### Run Locally
Simply double-click `index.html` to open it in any modern browser, or serve it locally:
```bash
npx serve .
