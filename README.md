# Interactive Receipt UI with Three.js + WebGL

## Project Description

This project is an interactive 3D receipt UI built with **Three.js** and **WebGL**, designed to simulate the behavior of a real thermal paper receipt rather than a simple flat animation.

![ScreenRecording2026-04-03at4 39 19AM-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/96fe4fdb-5970-4ca0-be51-65a29cddc5cb)


The receipt is modeled as a particle-based paper surface using **Verlet integration** and a **constraint system**, allowing it to behave like soft paper under user interaction. Users can grab the receipt with the **left mouse button**, drag it around, bend it, fold it, and observe natural motion such as swaying, creasing, and spring-back.

A key requirement of this project is that the **entire top edge remains fully constrained and perfectly straight**, preventing the common “clothesline” sagging effect that often appears in cloth simulations. At the same time, the lower portion of the receipt remains flexible, preserving the lightweight and responsive feel of paper.

The receipt surface is styled to resemble **thermal paper**, and it includes a humorous shopping list filled with 3D graphics terminology to reinforce the visual identity of the demo.

---

## Features

- Real-time interactive 3D receipt simulation
- Paper-like deformation using Verlet integration
- Constraint-based particle system
- Full-width top edge constraint to keep the top perfectly straight
- Mouse-based grabbing and dragging
- Natural bending, folding, swaying, and spring-back behavior
- Thermal paper-inspired material and texture
- White background with subtle shadows and highlights
- Optimized for smooth performance on desktop browsers

---

## How to Run

### Option 1: Open directly in the browser
Save the project as an `index.html` file and open it in a modern browser.

### Option 2: Run with a local server
Some browsers handle ES modules more reliably through a local server.

Using Python:

```bash
python -m http.server 8000
