Here is a professional, high-impact `README.md` designed to accompany your single-file project. It bridges the gap between a biology assignment and a technical showcase.

***

# 🛡️ DERMO DEFENSE: Laboratory Edition

> **A Gamified Exploration of Cutaneous Receptors & Somatosensory Physiology.**
> *Built entirely in a single HTML file.*

![Version](https://img.shields.io/badge/Version-Final_Master-blue)
![Tech](https://img.shields.io/badge/Tech-HTML5_|_JS_|_Web_Audio_API-yellow)
![Status](https://img.shields.io/badge/Status-Biology_Approved-green)

**DermoDefense** is an interactive tower defense game designed to teach the anatomy and physiology of the human skin's sensory system. Players take on the role of the central nervous system, processing signals from various mechanoreceptors and thermoreceptors to maintain homeostasis against environmental threats.

---

## 🔬 Features

### 🎮 The Simulation (Game Mode)
Defend the three layers of the skin (**Epidermis, Dermis, Hypodermis**) from incoming threats. You must identify the type of stimulus and trigger the correct receptor to neutralize it before it compromises tissue integrity.

### 🎛️ The Neural Oscilloscope (Lab Mode)
Explore a fully interactive **virtual laboratory**. Select any receptor from the database to view its:
*   **Anatomical Properties:** Location, field size, and fiber type.
*   **Signal Visualization:** A real-time canvas oscilloscope simulating action potentials.
*   **Interactive Stimulus:** Click to apply pressure/heat and watch/hear how Phasic vs. Tonic receptors adapt differently.

### 🔊 Procedural Audio Engine (No Assets)
This project uses **zero external audio files** (no `.mp3` or `.wav`).
*   **Real-time Synthesis:** All sounds—from the lab drone to the "synapse fire"—are generated mathematically in real-time using the **JavaScript Web Audio API**.
*   **Dynamic Soundscape:** The audio reacts to game states (Matrix mode, damage, menu interactions).

---

## 🕹️ Controls & Mechanics

Reflexes are key. Match the incoming threat icon to the correct biological receptor.

| Key | Receptor | Stimulus Type | Icon Example |
| :---: | :--- | :--- | :--- |
| **Q** | **Corpusculii Ruffini** | 🔥 Heat / Stretch | Sun, Fire |
| **W** | **Corpusculii Krause** | ❄️ Cold | Snow, Ice |
| **E** | **Corpusculii Pacini** | 🔨 Deep Pressure / Vibration | Hammer, Crush |
| **R** | **Corpusculii Meissner** | 🪶 Fine Touch | Feather, Insect |
| **SPACE** | **Nociceptors** | ⚡ Pain / Sharp | Needle, Knife |
| **ESC** | **Pause Menu** | - | - |

> **Pro Tip:** Missing a target causes "Synaptic Fatigue" (input jam) and score penalty. Accuracy is more important than spamming keys.

---

## 🧬 Scientific Concepts Covered

This project visualizes the following biological concepts:

1.  **Receptor Adaptation:**
    *   **Phasic (Rapid):** Pacini & Meissner (detect changes/vibrations).
    *   **Tonic (Slow):** Ruffini & Krause (detect constant states).
2.  **Skin Stratification:** Threats target specific layers (Epidermis vs. Hypodermis) based on real-world penetration depth.
3.  **Signal Transduction:** Visualized via the oscilloscope and audio pitch shifting.

---

## 🛠️ Technical Implementation

### The "Single-File" Constraint
The entire project (HTML structure, CSS styling, Game Logic, Databases, and Audio Engine) is contained within `main.html`.
*   **No external CSS/JS links.**
*   **No image assets** (everything is CSS art or Emojis).
*   **No audio files** (Procedural generation).

### The Audio System (`AudioSys`)
The game implements a custom sound synthesizer class containing:
*   **Oscillators:** Sine, Square, Sawtooth, and Triangle waves.
*   **Gain Nodes:** For envelope shaping (ADSR - Attack, Decay, Sustain, Release).
*   **Biquad Filters:** Low-pass and High-pass filters to create "muffled" or "sharp" sounds.

---

## 🥚 Secrets & Easter Eggs

Can you find them all?

*   **Matrix Mode:** Type `matrix` on your keyboard during the game to hack the visual mainframe.
*   **God Mode:** Click the "Watermark" in the bottom right corner **7 times**.
*   **Exam Mode:** Type `bac` to trigger "Bacalaureat Mode" (Hyper-speed).

---

## 🚀 How to Run

1.  Download `main.html`.
2.  Open the file in any modern web browser (Chrome, Firefox, Edge, Safari).
3.  **Click anywhere** on the screen once to initialize the Audio Context (browsers block auto-playing audio by default).
4.  Protect the skin!

---

## 👤 Author

**Ruben Oltean**
*Project developed for Biology & Computer Science Class.*
*Date: 2026*

> *"Homeostasis is not a choice, it's a requirement."*
