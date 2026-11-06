# 🧊 PartiCube

> **Interactive 3D Glass Cube Particle Automata with GPU Instanced WebGL**

[![Live Demo](https://img.shields.io/badge/Live-Demo-38bdf8?style=for-the-badge&logo=github)](https://ozlphrt.github.io/PartiCube/)
[![WebGL](https://img.shields.io/badge/WebGL-1.0-blue?style=for-the-badge)](https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API)
[![FPS](https://img.shields.io/badge/Target-60_FPS-10b981?style=for-the-badge)](#performance)

**PartiCube** is a real-time, interactive 3D WebGL simulation featuring multi-species particle cellular automata inhabiting the outer surfaces of a transparent, colorless glass wireframe cube.

---

## 🌟 Key Features

- **🚀 60 FPS GPU Instancing**: Render up to thousands of beveled 3D chiclets smoothly using `ANGLE_instanced_arrays` with zero per-frame vertex regeneration bottlenecks.
- **🧬 4-Species Multi-Agent Dynamics**:
  - 🔴 **Red (Sprinters)**: Rapid reflexes & aggressive pursuits.
  - 🟢 **Green (Cruisers)**: Steady cadence & territorial clustering.
  - 🟡 **Yellow (Darters)**: Lightning velocity & twitchy flocking.
  - 🔵 **Blue (Gliders)**: Heavy momentum, deliberate pathing, and bottom-dwelling buoyancy.
- **🎛️ Asymmetric Attraction / Repulsion Matrix**:
  - Interactive 4×4 force editor (attract, repel, neutral).
  - Built-in presets: **Chase**, **Tribes**, **Predator**, **Chaos**, **Random**, and **Neutral**.
  - Dynamic active preset highlighting and custom configuration detection.
- **🌐 3D Face Transitions & Corner Swiping**: Tiles seamlessly traverse cube faces, gliding across 90-degree edges on the cube's exterior surface without clipping.
- **🛡️ Anti-Oscillation ($n-1$ Lockout $\ge 5$s)**: Strict temporal lockout prevents tiles from ping-ponging back and forth to their previous cell.
- **🎚️ Dynamic Cube Subdivision Slider**: Glassmorphic capsule slider adjusts grid resolution from `9×9` up to `99×99` (default `31×31`), automatically maintaining 25% cube capacity.
- **🌓 Dual Theme Modes**: Elegant frosted dark glass default theme with instant toggle to high-contrast white mode.

---

## 🕹️ Controls

- **Left Mouse Click + Drag / Touch**: Orbit camera around the cube.
- **Right Mouse Click + Drag**: Pan camera.
- **Scroll Wheel / Pinch**: Zoom in and out.
- **Matrix Panel**:
  - Click any cell swatch in the matrix table to toggle force (+0.85 attract, -0.85 repel, 0.00 neutral).
  - Click any preset button to instantly load multi-species behaviors.
  - Click **Balance** to toggle population kinetic damping.
  - Click **Vertical Zones** to assign vertical strata affinities.
  - Drag the **Cube Size** slider to dynamically resize the simulation domain.

---

## 🚀 Live Deployment

The project is hosted and executable via GitHub Pages:
**[https://ozlphrt.github.io/PartiCube/](https://ozlphrt.github.io/PartiCube/)**

---

## 📄 License

MIT License.

