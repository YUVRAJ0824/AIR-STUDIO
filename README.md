# AIR//STUDIO

Webcam motion instrument studio in the browser. Translates real-time hand tracking into live procedural drum, piano, and percussion hits with zero external hardware or build tools.

*Personal experimental project for learning, creative demo testing, and motion-audio research.*

---

## TECH STACK

- **MediaPipe Hands**: 21 3D hand landmarks tracking at 24-30 fps for fingertip strike velocity and dual-hand interaction.
- **Web Audio API**: Real-time procedural synthesis (sine/triangle/square oscillators, white noise buffers, biquad filters, 28-voice management).
- **HTML5 Canvas 2D**: 60fps hardware-accelerated AR overlays (10-piece drum kit, bronze lathe cymbals, chromatic keys, hit ripples).
- **Vanilla JS & CSS**: Zero build dependencies, ~12ms response latency, light purple neon (#C084FC) cyber aesthetic.

---

## FEATURES & INSTRUMENTS

- **10-Piece Drum Kit**: Cymbals (Crash, Splash, Ride, Hats) and Drums (Snare, Toms, Kick) with velocity sensing.
- **Chromatic Piano**: Standard 13-key and extended 20-key layout anchored at bottom 50% stage with multi-finger polyphony.
- **Xylophone**: 7 to 10-bar melodic percussion with wood/metal resonance.
- **Controls & Privacy**: 3-step sensitivity buttons (Light, Normal, Firm), face-blur privacy toggle, and live oscilloscope.

---

## WORKFLOW & ROADMAP

- **Pacing**: Heavy testing is built in `air-studio-exp.html` (git-ignored); stable code lands in `air-studio.html` via daily 3-5% commits. See `TASK.txt` for live status.
- **Future Plans**:
  - Native Java DSP backend engine and virtual MIDI output for DAWs (Ableton, FL Studio).
  - 808 Synth Bass, 4-bar looper, custom WAV sound pack loader, and 4-tier gesture sensitivity.

---

## QUICK START

Open `air-studio.html` in any browser, click **Launch System**, allow webcam access, and play.
