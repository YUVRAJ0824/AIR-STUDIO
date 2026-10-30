# AIR//STUDIO

**Real-Time Hand Gesture Musical Workstation Using Computer Vision and Web Audio Technology**  
*Author: Yuvraj V*

---

A browser-based motion musical workstation featuring a 10-piece drum kit, chromatic piano, and xylophone. Play instruments in mid-air using webcam hand tracking and procedural sound synthesis with zero external hardware or build tools.

*Personal experimental project for learning, creative demo testing, and motion-audio research.*

---

## TECH STACK

- **MediaPipe Hands**: 21 3D hand landmarks tracking at 24-30 fps for fingertip strike velocity and dual-hand interaction.
- **Web Audio API**: Real-time procedural synthesis (sine/triangle/square oscillators, white noise buffers, biquad filters, 28-voice management).
- **HTML5 Canvas 2D**: 60fps hardware-accelerated AR overlays (10-piece drum kit, bronze lathe cymbals, chromatic keys, hit ripples).
- **Vanilla JS & CSS**: Zero build dependencies, ~12ms response latency, light purple neon (#C084FC) cyber aesthetic.

---

## FEATURES & INSTRUMENTS

- **10-Piece Drum Kit**: Full acoustic/cyber layout with 5 cymbals (Crash, Splash, Ride, Closed Hat, Open Hat) and 5 drums (Snare, High Tom, Mid Tom, Floor Tom, Bass/Kick) with velocity sensing.
- **Chromatic Piano**: Standard 13-key and extended 20-key layout anchored at bottom 50% stage with multi-finger polyphonic strike detection.
- **Xylophone**: 7 to 10-bar melodic percussion with wood/metal resonance.
- **Controls & Privacy**: 4-level sensitivity presets (Very Low, Low, Mid, High), face-blur privacy toggle, and live oscilloscope.

---

## REPOSITORY STRUCTURE

- **`ORG/air-studio.html`**: Production-ready, stable browser application. Zero build tools or npm dependencies required—runs directly in any modern browser.

---

## FUTURE ROADMAP & JAVA EXPANSION

- Native Java DSP backend engine and virtual MIDI output for DAWs (Ableton, FL Studio).
- 808 Synth Bass, 4-bar looper, custom WAV sound pack loader, and 1-finger chord mode.

---

## QUICK START

Open `ORG/air-studio.html` in any browser, click **Launch System**, allow webcam access, and play.
