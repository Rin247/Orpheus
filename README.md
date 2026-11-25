# Orpheus — Standalone Groovebox & Music Workstation

Orpheus is a powerful standalone Android groovebox and digital audio workstation inspired by the hardware workflows of the Roland MC-101 and MC-707. Built with Kotlin, Jetpack Compose, and a low-latency C++ audio synthesis engine (`AAudio`/`Oboe`), Orpheus delivers a complete portable music production environment.

---

## 🎹 Key Features & Module Breakdown

### 🥁 Step Sequencer & Pattern Matrix (`sequencer`)
- **Current**: 16-step grid sequencer, multi-track pattern chaining, velocity control, probability triggers, and micro-timing adjustments.
- **Planned / Roadmap**: Polyphonic step sequencing, scene chaining, song mode arranger, and parameter automation recording.

### 🎹 Synthesizer & Tone Engine (`synth`)
- **Current**: Multi-oscillator subtractive synthesis engine, resonant low-pass/high-pass filters, ADSR envelopes, and LFO modulation.
- **Planned / Roadmap**: FM synthesis engine, wavetable oscillator engine, sample slicing / drum kit engine, and SoundFont (.sf2) support.

### 🎚️ Mixer & Effects Processor (`fx`)
- **Current**: Per-track volume/pan mixer, delay, reverb, and overdrive effects.
- **Planned / Roadmap**: Multi-band compressor, master limiter, sidechain compression, and 3-band parametric track EQ.

### 💾 MIDI & File I/O (`midi`)
- **Current**: USB MIDI controller support, WAV audio export, and project file saving.
- **Planned / Roadmap**: Bluetooth LE MIDI support, MIDI clock sync (Ableton Link / DIN sync), and Stem WAV exporter.

---

## 🏗️ Architecture & Technology Stack

- **Platform**: Android 13+ (minSdk 33, targetSdk 37).
- **UI & Controls**: Kotlin, Jetpack Compose, Custom hardware-inspired dials & step pads.
- **Audio Engine**: Native C++ Audio Pipeline (`Oboe` / `AAudio` 32-bit float engine).
- **Licensing**: AGPL-3.0.

---

## 🛠️ Building & Running

```bash
./gradlew assembleDebug
./gradlew installDebug
```

---

## 📜 License

Orpheus is released under the **GNU Affero General Public License v3.0** (AGPL-3.0). See [`LICENSE`](LICENSE) for details.
