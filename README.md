# Ultra-Realistic 3D Solar System + Gargantua

A high-performance, interactive 3D space simulation built with **Three.js**. This project features a procedural solar system and a gravitationally accurate (visual) representation of a "Gargantua" style black hole, complete with post-processing bloom and custom shaders.

## 🚀 Live Features

### 🪐 Celestial Bodies

- **Dynamic Sun:** Procedural corona particles, multiple glow layers, and sunspot textures.
- **The Eight Planets:** Individual rotation speeds, axial tilts, and custom-generated textures (canvas-based).
- **Earth & Moon:** High-resolution textures with an additive cloud layer and orbital moon pivot.
- **Saturn’s Rings:** Procedurally mapped ring geometry with transparency and shadow support.
- **Asteroid Belt:** 900+ instanced icosahedrons for performance-friendly orbital debris.

### 🕳️ The "Gargantua" Black Hole

- **Event Horizon:** A light-absorbing black core.
- **Accretion Disk:** A swirling, glowing disk with custom UV mapping to simulate heat gradients.
- **Gravitational Lensing:** A Fresnel-based halo shader that simulates the bending of light.
- **Spacetime Warp:** Focusing on the black hole triggers a FOV "warp" effect and a particle-based "pulling space" animation.

### 🛠️ Technical Highlights

- **Post-Processing:** Uses `EffectComposer` with `UnrealBloomPass` for realistic light bleeding.
- **Optimized Rendering:** Instanced rendering for asteroids and custom canvas textures to reduce external asset dependency.
- **Interactive Controls:** `OrbitControls` enhanced with smooth damping and a custom "Zoom to Cursor" logic.

## 🎮 Controls

| Action           | Control                                  |
| :--------------- | :--------------------------------------- |
| **Rotate**       | Left Click + Drag                        |
| **Pan**          | Right Click + Drag                       |
| **Zoom**         | Scroll Wheel (Zooms toward mouse cursor) |
| **Focus Object** | Double-Click on a Planet or Black Hole   |
| **Reset Focus**  | Double-Click on empty space              |

## 📦 Dependencies

- [Three.js](https://threejs.org/) (Core Library)
- [OrbitControls](https://threejs.org/docs/#examples/en/controls/OrbitControls)
- [UnrealBloomPass](https://www.google.com/search?q=https://threejs.org/docs/%23examples/en/postprocessing/UnrealBloomPass)
