# 🔥 VR Fire Evacuation Training Simulator — Meta Quest 3S

An immersive, standalone **Virtual Reality Fire Evacuation Training Simulator** built with **A-Frame** and **WebXR**, specifically optimized for the **Meta Quest 3S** (with full desktop preview fallback).

The purpose of this simulator is to train students, employees, and residents to make critical life-safety decisions during a realistic structural fire emergency.

---

## 🎯 Key Training Objectives

1. **Observe & Decide**: Don't blindly run. Read environmental cues, evaluate smoke density, and follow emergency illuminated signs.
2. **Recognize Hazards**: Understand that smoke inhalation and blocked routes require dynamic re-routing.
3. **Use Safety Hardware Correctly**:
   - Pull manual fire alarm pull stations to alert facility occupants.
   - Use fire extinguishers only on small, controllable fires. Large structural fires cannot be fought—evacuate immediately!
4. **Locate Assembly Points**: Follow illuminated emergency exits to the designated outside ISO 7010 assembly point.

---

## 🚀 How to Run

### Option 1: On Meta Quest 3S / Quest 3 / Quest 2 Headset
1. Host this project on a local network (e.g., `python -m http.server 8080`) or deploy to GitHub Pages / Netlify / Vercel.
2. Open the URL inside the **Meta Quest Browser**.
3. Click the **VR** button in the bottom right corner of the screen.

### Option 2: Desktop Preview (Browser)
Open `index.html` directly in any modern WebGL-supported browser (Chrome, Edge, Firefox, Brave):
- **Move**: `W`, `A`, `S`, `D`
- **Look**: Click and drag mouse
- **Interact**: Click on doors, alarm station, extinguisher, or buttons

---

## 🎮 Meta Quest 3S Controls

- **Left Controller**:
  - **Thumbstick**: Smooth locomotion in the direction you are facing
  - **Laser Ray**: Pointer and secondary interaction
- **Right Controller**:
  - **Thumbstick Horizontal Flick**: 45° snap turn (prevents VR motion sickness)
  - **Trigger**: Click / interact with buttons, doors, pull stations, and extinguisher

---

## 🏢 Training Scenarios

- **Scenario 1: BASIC (Clear Exit)**
  - Small localized trash fire, low smoke spread.
  - Main lobby entrance remains clear and safe.
  - Ideal for learning controls and basic evacuation procedure.

- **Scenario 2: INTERMEDIATE (Exit Blocked)**
  - Utility fire in lobby. Moderate smoke spreading down the corridor.
  - Main entrance is blocked by structural fire and collapsed ceiling beam.
  - Occupants must identify the hazard, backtrack, and locate **Emergency Exit B (Stairwell)**.

- **Scenario 3: ADVANCED (Heavy Hazards)**
  - Rapid structural fire with heavy toxic smoke and emergency lighting.
  - Multiple hazard zones testing rapid adaptation, route assessment, and minimum smoke inhalation.

---

## 📊 Analytics & Post-Evacuation Report

Upon reaching the outside safe assembly point, a 3D VR board presents:
- Total evacuation time
- Initial reaction time
- Cumulative smoke exposure rating
- Hazards avoided vs wrong route decisions
- Fire alarm pulled (Yes/Delayed)
- Safety score (out of 100) and letter grade
- Actionable training insights and recommendations
- Restart button to practice again

---

## 🛠️ Technology Stack

- **A-Frame 1.7.0** (WebXR Framework)
- **Web Audio API** (100% procedural synthesized audio: Temporal Code 3 siren, fire crackle, extinguisher hiss, latch squeaks, fanfare)
- **Zero External Media Dependencies**: Entirely self-contained in a single, lightweight `index.html` file.
