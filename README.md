# 3D Rubik's Cube Simulator (3x3x3)

A high-performance, fully 3D Rubik's Cube simulator and group-theoretic analysis tool built with Three.js.

**Live Deployment:** [https://rubiks-cube-3d-gamma.vercel.app](https://rubiks-cube-3d-gamma.vercel.app)

---

## Features

- **Realistic 3D Graphics**:
  - 26 beveled cubies with an internal black core rendered via Three.js.
  - Official WCA color scheme: White (Top / U), Yellow (Bottom / D), Green (Front / F), Blue (Back / B), Red (Right / R), Orange (Left / L).
  - 60fps slice turns with smooth cubic easing and clean mathematical matrix updates.

- **Direct Touch & Mouse Interaction**:
  - Click/touch and drag any sticker directly to rotate that specific layer.
  - Interactive drag projection with release snap to the nearest $90^\circ$ turn.
  - Right-click / two-finger drag camera orbit controls with damping.

- **Full Cube Naming Schemes**:
  - **GAP54**: Standard computational group theory enumeration (1–54 across U, L, F, R, B, D).
  - **Singmaster**: Full canonical clockwise cyclic Singmaster notation with sub-indices for all 54 facelets (e.g. $U_{RF}, R_{FU}, F_{UR}$).
  - **Both**: Simultaneous dual-badge mode rendering Singmaster above GAP54 on high-contrast markers.
  - **Current-State Stamping**: Dynamically calculates upright relative rotation based on the current cubie orientation.

- **Facelet & Tracking Drawer**:
  - Place custom tracking dots on any facelet to track piece movement during algorithms.
  - Customizable dot colors via real-time color picker and custom text labels.
  - Save and load dot configurations to `localStorage`.
  - 2D Unfolded Net View synchronized in real-time with the 3D cube.

- **Algorithms & Themes**:
  - Valid 20-move WCA scrambler and state reset.
  - Preset algorithms (Sexy Move, Sune, T-Perm).
  - Visual themes: Classic WCA, Cyberpunk Neon, Frosted Glass, Carbon Fiber.
  - PWA support with offline caching via Service Worker.

---

## Local Development

Open `index.html` in any modern web browser or serve locally:

```bash
# Python simple HTTP server
python -m http.server 8000
```
