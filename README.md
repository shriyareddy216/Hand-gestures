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

