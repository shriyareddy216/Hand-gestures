# 🖐 Dual Hand Particle System

An interactive 3D particle experience controlled entirely by your hands via webcam. No clicks, no keyboard — just gestures.

Built with **Three.js** and **MediaPipe Hand Landmarker**.

---

## ✨ Demo

Open `dual-hand-particles.html` in any modern browser and allow webcam access. That's it — no build step, no dependencies to install.

---

## 🎮 Controls

### ✋ Right Hand — Shape Control

| Gesture | Shape |
|--------|-------|
| ✊ Fist (0 fingers) | Sphere |
| ☝️ 1 finger | Heart |
| ✌️ 2 fingers | Saturn |
| 🤟 3 fingers | Helix |
| 🖖 4 fingers | Cube |
| 🖐 Open hand (5) | Galaxy |
| 👌 Pinch | **Cycle through all 18 shapes** |

> Pinch also **drags** the entire particle system around the screen while held.

---

### 🤚 Left Hand — Effects & FX

| Gesture | Effect |
|--------|--------|
| ✊ Fist (0 fingers) | Normal (no effect) |
| ☝️ 1 finger | Pulse — shape breathes in and out |
| ✌️ 2 fingers | Vortex — particles spin in rings |
| 🤟 3 fingers | Scatter — noisy turbulent jitter |
| 🖖 4 fingers | Wave — ripple distortion |
| 🖐 Open hand (5) | **BLAST** — full explosive expansion |
| 👌 Pinch | **Cycle color palette** (8 palettes) |

---

## 🔷 All 18 Shapes

| # | Shape | # | Shape |
|---|-------|----|-------|
| 0 | Sphere | 9 | Trefoil Knot |
| 1 | Heart | 10 | Rose (5-petal) |
| 2 | Saturn | 11 | Butterfly Curve |
| 3 | Helix | 12 | Icosahedron |
| 4 | Cube | 13 | Tornado |
| 5 | Galaxy | 14 | Star (8-point) |
| 6 | Torus | 15 | Portal (nested rings) |
| 7 | DNA Double Helix | 16 | Mushroom |
| 8 | Möbius Strip | 17 | Klein Bottle |

A dot strip at the bottom of the screen tracks your current shape index.

---

## 🎨 Color Palettes

Cycle through 8 palettes using **left hand pinch**:

`Electric` · `Fire` · `Emerald` · `Rose` · `Gold` · `Ice` · `Lavender` · `Sunset`

---

## 🚀 Getting Started

```bash
git clone https://github.com/yourusername/dual-hand-particles.git
cd dual-hand-particles
```

Then open `dual-hand-particles.html` directly in Chrome or Edge.

> **Note:** Webcam access requires a secure context. If opening locally doesn't work, serve it over HTTP:
> ```bash
> npx serve .
> # or
> python -m http.server 8080
> ```
> Then visit `http://localhost:8080`

---

## 🛠 Tech Stack

| Library | Version | Purpose |
|---------|---------|---------|
| [Three.js](https://threejs.org) | 0.160.0 | 3D rendering & particles |
| [MediaPipe Tasks Vision](https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker) | 0.10.0 | Real-time hand tracking |

No bundler. No framework. Single HTML file with ES module imports.

---

## 📁 File Structure

```
dual-hand-particles/
├── dual-hand-particles.html   # Entire app — open this
└── README.md
```

---

## ⚙️ Configuration

At the top of the `<script>` block you can tweak:

```js
const PARTICLE_COUNT = 22000;   // Lower for better performance
const PARTICLE_SIZE  = 0.075;   // Increase for larger dots
const LERP_BASE      = 0.07;    // Higher = snappier transitions
```

Mobile devices automatically use `8000` particles for performance.

---

## 🌐 Browser Support

| Browser | Status |
|---------|--------|
| Chrome 90+ | ✅ Recommended |
| Edge 90+ | ✅ Works |
| Firefox | ⚠️ MediaPipe GPU delegate may fall back to CPU |
| Safari | ⚠️ Limited — use Chrome on iOS |

---

## 📄 License

MIT — do whatever you want with it.

---

## 🙌 Credits

- Hand tracking powered by [Google MediaPipe](https://mediapipe.dev)
- 3D rendering by [Three.js](https://threejs.org)
- Shape math inspired by various parametric equation resources
