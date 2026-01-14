# DermoDefense: Cutaneous Receptor Simulation

![Version](https://img.shields.io/badge/version-Final%20Master%20Edition-blue)
![Tech](https://img.shields.io/badge/tech-HTML5%20%7C%20CSS3%20%7C%20JS-yellow)
![Audio](https://img.shields.io/badge/audio-Procedural%20Web%20Audio%20API-success)

**DermoDefense** is an interactive educational simulation designed to gamify the learning process of human skin anatomy and neurophysiology. By combining "lane-defense" arcade mechanics with accurate biological data, players learn to associate specific somatosensory receptors with their corresponding external stimuli.

> **Project Constraint:** The entire application is self-contained within a **single HTML file** (logic, styling, assets, and audio engine), requiring zero external dependencies or installation.

---

## 🔬 Scientific Overview

The simulation models the integumentary system, specifically focusing on the dermis and its mechanoreceptors, thermoreceptors, and nociceptors. The gameplay requires the user to maintain homeostasis by activating the correct receptor to intercept incoming threats before they damage the skin layers (Epidermis, Dermis, Hypodermis).

### Receptor Mapping
The simulation accurately maps stimuli to their biological counterparts:

| Key | Receptor | Stimulus Type | Physiology |
| :---: | :--- | :--- | :--- |
| **Q** | **Corpusculii Ruffini** | Heat / Stretch | Tonic adaptation, detects continuous states. |
| **W** | **Corpusculii Krause** | Cold | Thermoreceptors active between 10-35°C. |
| **E** | **Corpusculii Pacini** | Deep Pressure | Phasic adaptation, detects vibration/acceleration. |
| **R** | **Corpusculii Meissner** | Light Touch | Located in dermal papillae, high sensitivity. |
| **SPC** | **Nociceptors** | Pain | Free nerve endings, non-adaptive (tonic). |

---

## ⚙️ Technical Features

### 1. Procedural Audio Engine v2.4
This project utilizes **no external audio files** (MP3/WAV). All sound is synthesized in real-time using the **Web Audio API**.
*   **Binaural Ambience:** Generates a low-frequency drone using detuned oscillators.
*   **Dynamic Synthesis:** Sound effects (shooting, damage, UI interaction) are generated mathematically on the fly.
*   **Interactive Oscilloscope:** The "Lab" view visualizes the generated waveforms in real-time on an HTML5 Canvas.

### 2. Architecture & Performance
*   **Zero-Dependency:** Runs entirely in the browser memory.
*   **Mobile-First Design:** Optimized for touch input, with specific CSS handling for iOS Safari notches (`safe-area-inset`) and touch-action handling.
*   **Local Storage:** Persists high scores and tutorial completion status.

### 3. Visuals
*   **CSS-Only Art:** Receptor diagrams and particle effects are drawn using CSS shapes and gradients.
*   **Post-Processing:** Simulates a CRT monitor aesthetic with scanlines, chromatic aberration, and screen curvature.

---

## 🎮 How to Play

### Controls

| Action | Keyboard | Mobile / UI |
| :--- | :--- | :--- |
| **Heat Defense** | `Q` or `1` | Red Button |
| **Cold Defense** | `W` or `2` | Blue Button |
| **Pressure Defense** | `E` or `3` | Green Button |
| **Touch Defense** | `R` or `4` | Purple Button |
| **Pain Defense** | `Space` or `5` | Yellow Bar |
| **Pause** | `Esc` | Pause Icon |

### Mechanics
1.  **Threats:** Different stimuli (e.g., UV rays, Ice, Needles) fall toward the skin layers.
2.  **Defense:** Press the button corresponding to the receptor that detects that specific threat.
3.  **Combo System:** Successful intercepts build a score multiplier (up to 5x).
4.  **Regeneration:** A 10-hit combo triggers cell regeneration, restoring system integrity.
5.  **Synaptic Fatigue:** pressing the wrong key causes a "lockout," simulating neural fatigue.

---

## 🛠️ Installation & Usage

1.  **Download:** Save the `index.html` file to your computer or mobile device.
2.  **Run:** Double-click the file to open it in any modern web browser (Chrome, Safari, Firefox, Edge).
3.  **Audio:** Click anywhere on the screen once loaded to initialize the Audio Context (browser security requirement).

---

## 🕵️ Secrets & Debugging

The simulation includes several "Easter Eggs" and debug modes triggered via keyboard sequences:

*   **Matrix Mode:** Types `matrix` to toggle a green-phosphor terminal aesthetic.
*   **Exam Mode:** Types `bac` (Baccalaureate) to trigger high-speed difficulty (Speed 3.0x).
*   **God Mode:** Click the watermark text 7 times to toggle invincibility.

---

## 📜 Credits

**Author:** Ruben Oltean  
**Date:** 2026  
**License:** Educational Use / Portfolio Edition

*Fonts provided by Google Fonts (Exo 2, Share Tech Mono).*
