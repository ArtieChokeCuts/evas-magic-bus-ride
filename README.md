# Eva’s Magic Bus Ride

A lightweight 3D educational game built with **HTML5, CSS3, JavaScript, and Three.js**.

Eva’s Magic Bus Ride is designed as a high-level learning journey where a child explores floating bubbles in a sky world and practices two core tracks:

- **Arithmetic (Math)**
- **Literacy (Alphabet/Spelling)**

---

## Core Experience

The game presents a clean 3D environment with clouds and interactive floating spheres (“bubbles”).
Each bubble is rendered as a 3D sphere and labeled with a number or letter using canvas-texture mapping.

When Eva taps a bubble:

1. The bubble triggers a **pop animation** (scales down to zero).
2. A rewarding **`pop.mp3`** sound effect plays.

This interaction model acts as Eva’s “magic wand” mechanic—simple, tactile, and focused on educational feedback.

---

## Learning Paths

### 1) Arithmetic Path (Math)

The math journey emphasizes number recognition and arithmetic growth.

- Learners identify and pop target number bubbles (e.g., `11`, `9`).
- Progress is tracked independently with a math progression value (e.g., `mathLevel`).

### 2) Literacy Path (Spelling)

The literacy journey focuses on alphabet familiarity, phonics readiness, and spelling progression.

- Learners interact with letter bubbles (e.g., `E`, `B`).
- Progress is tracked independently with a spelling progression value (e.g., `spellingLevel`).

### Independent Growth Model

Math and spelling are tracked separately so learners can advance at different speeds in each domain.

---

## Audio Identity

The game uses personalized audio cues to reinforce momentum and milestones:

- **Theme:** `eva_theme.mp3` (soulful background identity)
- **Milestone cue:** `magic.mp3` (level transition / special event reward)
- **Interaction cue:** `pop.mp3` (bubble pop feedback)

---

## Technical Profile

- **Rendering:** Three.js (`three.min.js`)
- **App shell:** `index.html`
- **Assets:** static local media files (`.mp3`, `.png`)
- **Philosophy:** lean educational repository with no combat/action systems
  - No enemies
  - No lasers
  - No health packs

---

## Repository Structure

```text
.
├── index.html        # Main game scene and logic
├── three.min.js      # Three.js runtime
├── eva_theme.mp3     # Theme music
├── magic.mp3         # Milestone sound
├── pop.mp3           # Bubble pop sound
├── eva.png           # Eva-related art asset
└── splash.png        # Splash / branding art asset
```

---

## Run Locally

Because this is a static web app, you can run it with any local web server.

### Option A: Python

```bash
python3 -m http.server 8080
```

Then open:

- <http://localhost:8080>

### Option B: VS Code Live Server

Open the folder and run **“Open with Live Server”**.

---

## Educational Design Goals

- Encourage repeatable, low-friction interaction.
- Reward correct actions with immediate visual and audio feedback.
- Build confidence through separate progression in math and literacy.
- Maintain a calm, wonder-driven atmosphere suitable for young learners.
