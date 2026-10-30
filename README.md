# AIR//STUDIO

A lightweight, webcam-based air instrument studio built directly in the browser. Using computer vision and procedural audio synthesis, it turns hand motions into live drum, piano, and melodic percussion hits with zero external hardware.

Note: Personal project built for experimentation, learning, and creative demo testing.

---

## TECH STACK & ARCHITECTURE

The application runs entirely client-side with no build step or node bundling required:

- **MediaPipe Hands**:
  - Detects up to 2 hands in real time, tracking 21 3D skeletal landmarks per hand.
  - Used for fingertip strike velocity calculation, key/pad hover targeting, and dual-hand interaction.
- **Web Audio API**:
  - Generates procedural instrument audio on the fly with zero external sound packs.
  - Uses custom oscillators (sine, triangle, square), procedural white noise buffers, highpass/bandpass biquad filters, and dynamic compression.
  - Supports 28-voice polyphonic voice management with automatic oldest-voice reclamation.
- **HTML5 Canvas 2D**:
  - Renders AR overlays on top of the webcam feed at 60 fps.
  - Draws realistic 10-piece drum skins, lathe-grooved bronze cymbals, chromatic piano keybeds, skeletal hand laser tracking, and velocity ripple rings.
- **Vanilla JavaScript & CSS3**:
  - Zero framework overhead for minimal input-to-sound latency (~12ms).
  - Styled with a dark cyber aesthetic using light purple neon accents (#C084FC).

---

## CURRENT FEATURES & INSTRUMENTS

### Instruments
- **10-Piece Acoustic & Cyber Drum Kit**:
  - Cymbals: Crash, Splash, Ride, Closed Hi-Hat, Open Hi-Hat.
  - Drums: Snare, High Tom, Mid Tom, Floor Tom, Bass / Kick.
  - Dual-hand multi-finger strikes with dynamic velocity sensing.
- **Chromatic Piano**:
  - Standard 13-key (C4 to C5) and extended 20-key (C4 to G5) chromatic layouts.
  - Bottom 50% stage anchor for comfortable hand reach.
  - Multi-finger polyphonic strike detection with hover target guides.
- **Xylophone**:
  - Diatonic 7-bar and extended 10-bar chromatic bars with bright marimba/wood resonance.

### Interface & Controls
- **Discrete Sensitivity Options**: Quick toggles (LIGHT: 0.040, NORMAL: 0.052, FIRM: 0.072) to prevent jitter and false triggers.
- **Privacy Mode**: Real-time webcam face-blur filter while maintaining full hand skeletal tracking.
- **Live Diagnostics**: Audio oscilloscope waveform visualizer, hit counter, system state, and latency monitor.
- **Dual Layouts**: Standard and compact mini view.

---

## WORKFLOW & REPOSITORY STRUCTURE

- **`air-studio.html`**: Production-ready, stable codebase updated in measured daily increments (~3% to 5% per session).
- **`air-studio-exp.html`**: Experimental sandbox for testing heavy features, complex audio DSP, or layout experiments before rolling into the main branch.
- **`TASK.txt`**: Active daily progress log and roadmap tracker.

---

## FUTURE ROADMAP & JAVA EXPANSION

### Java-Based Desktop Engine & Backend
- **Native Java DSP Audio Engine**: Heavy audio processing backend for ultra-low latency ASIO/CoreAudio buffer playback.
- **Virtual MIDI Out**: Bridge hand tracking events into local DAWs (Ableton Live, FL Studio, Logic Pro, Reaper) via virtual MIDI ports.
- **Java Native Desktop Client**: Standalone lightweight wrapper using JavaFX / lightweight WebView with background thread audio processing.

### Planned Instrument & Sound Extensions
- **Synth Bass & 808 Machine**: Sub-bass oscillators and 808-style trap kicks.
- **Chords & Pad Mode**: 1-finger auto-chord progressions for ambient textures.
- **4-Bar Beat Looper**: Layer percussion loops live with hand gesture punch-in recording.
- **Custom Sound Pack Loader**: Drag-and-drop WAV/MP3 sample pack loader for custom user kits.
- **Advanced Sensitivity Controls**: 4-level trigger selector (Very Low, Mid-Low, Mid-High, Auto) and finger mode options (index finger isolation vs all 5 fingers).

---

## RUNNING LOCALLY

1. Clone the repository:
   ```bash
   git clone https://github.com/YUVRAJ0824/AIR-STUDIO.git
   ```
2. Open `air-studio.html` directly in any modern browser (Chrome, Edge, Firefox, Brave).
3. Click **Launch System**, grant webcam permission, and play.
