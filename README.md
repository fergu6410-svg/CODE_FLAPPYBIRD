<div align="center">

# Flappy — Celestial Edition

**A premium, high-performance Flappy Bird clone with dynamic environments and polished physics.**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES2020-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

</div>

---

## Overview

Flappy — Celestial Edition is a lightweight, single-file web game built with vanilla JavaScript and HTML5 Canvas. It features a sophisticated day/night cycle, orbital celestial bodies, and pixel-perfect hitboxes designed for a fair yet challenging gameplay experience.

---

## Features

| Feature | Description |
|---|---|
| **Day/Night Cycle** | Seamless 24-second transition between Noon, Sunset, Midnight, and Sunrise. |
| **Celestial Orbit** | Dynamic Sun and Moon rotation with adaptive lighting and fading stars. |
| **Polished Physics** | Optimized gravity and flap impulse for a "floaty," responsive feel. |
| **Fair Hitboxes** | Tightened collision detection (14.5px radius) focused on the bird's core body. |
| **Visual Feedback** | Glow flashes on input, 3D pipe gradients, and animated wing flaps. |
| **Debug Mode** | Toggle visible collision boundaries in real-time by pressing the **'H'** key. |
| **Persistence** | Automatically saves your high score using `localStorage`. |
| **Responsive** | Mobile-ready with support for touch, mouse clicks, and Spacebar input. |

---

## Technical Details

- **Language:** JavaScript ES2020+ (No frameworks, pure logic).
- **Rendering:** Zero-dependency HTML5 Canvas API.
- **Physics:** Frame-independent time-based velocity updates.
- **Optimization:** Single-pass rendering at 60FPS with efficient pipe pooling.
- **Assets:** Procedural SVG-based graphics (no external image requests).

---

## How to Play

### Controls
- **Spacebar / Click / Tap:** Flap wings and gain altitude.
- **H Key:** Toggle Hitbox Debug Layer.

### Objective
Navigate through the gaps in the pipes. The game speeds up and the gaps shrink as your score increases, testing your reflexes under pressure.

---

## Setup & Running

Simply clone the repository and open `index.html` in any modern web browser.

```bash
# Clone the repository
git clone https://github.com/your-username/flappy-celestial.git

# Open the game
open flappy-bird/index.html
```

---

## Development & Customization

The game is contained entirely within `index.html`. You can easily adjust the difficulty by modifying the constants at the top of the `<script>` tag:

```javascript
/* ── Constants ── */
const GRAVITY      = 0.26;   // Adjust fall speed
const FLAP         = -6.4;   // Adjust jump height
const PIPE_SPD_BASE= 2.2;    // Initial scroll speed
const DAY_DURATION = 24000;  // Length of a full day cycle (ms)
```

---

## Browser Compatibility

| Browser | Support |
|---|---|
| Google Chrome | ✅ Full |
| Mozilla Firefox | ✅ Full |
| Apple Safari | ✅ Full |
| Microsoft Edge | ✅ Full |

> Supports all modern browsers with Canvas 2D and ES6+ support.
