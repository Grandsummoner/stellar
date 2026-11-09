# Grandsummoner Stellar

> **14 HP Dual-Voice Multi-Model Synthesizer Companion**

<p align="left">
  <img src="res/Stellar.svg" alt="Grandsummoner Stellar Front Panel" width="440" />
</p>

---

## Overview

**Stellar** is a 14 HP dual-voice analog/digital hybrid synthesizer module for [VCV Rack v2](https://vcvrack.com/). Engineered as the melodic core of the Grandsummoner family, Stellar combines two fully independent voice engines, each equipped with four combinable oscillator models, a warm 4-pole Moog-style resonant ladder filter with automatic bass compensation, an ultra-fast ADSR envelope generator, and dedicated sub-oscillator outputs.

In addition to its two primary synthesizer voices, Stellar houses a standalone white noise generator and an external audio input that mixes external modular sources directly with Voice 1 and Voice 2 before the master stereo stage.

---

## The Grandsummoner Module Family

Stellar delivers the harmonic foundation of the **Grandsummoner Eurorack Family**, designed to operate either as a dedicated voice or as part of a larger patch:

| Module | Width | Primary Function | Role in Ecosystem |
| :--- | :--- | :--- | :--- |
| **Spaces Command** | 38 HP | Dual-Scene Probabilistic CV/Gate Sequencer & Arpeggiator | Master Composition & Clock Brain |
| **Beams** | 18 HP | Quad Algorithmic Euclidean Drum Engine & Sampler | Rhythm, Percussion & Clock Sync |
| **Stellar** | 14 HP | Dual-Voice Multi-Model Synthesizer Companion | Primary Melodic & Harmonic Voice |
| **Intel** | 14 HP | Modulation Matrix, Dual FX Engine & Metering Ladder | Utility, Inter-Module Modulation & Modulation Router |
| **Explorer** | 12 HP | Tape-Cloud Delay, Diffusion Reverb & Octave Shimmer | Master Spatialization, Diffusion & Ambient Textures |

### Shared Design Language
Every Grandsummoner module adheres to an authentic laboratory aesthetic:
- **Warm Sand Cards** (`#F5F1E9` top gradient down to `#EDE7DC`) framed by precision `0.4–0.5pt` bronze borders (`#8A7F6A`).
- **Deep Obsidian Knobs** with ivory indicator lines (`#E8E0D0`).
- **Color-Coded Voice Accents**: Voice 1 performance elements accent in Brass (`#8A6423`), while Voice 2 accents in Maroon (`#8A2A2A`).
- **Clean Label Hierarchy**: Bold uppercase signal headers with high-contrast legibility.

### Standalone vs. Family Operation

- **100% Standalone**: Stellar is fully self-contained. Both voices take standard 1V/Oct pitch, gate, and VCA modulation inputs from any keyboard, sequencer, or MIDI interface.
- **Universal Adjacency Link**: Side connector LEDs (`LINK L` and `LINK R`) automatically illuminate when Stellar sits adjacent to any Grandsummoner family module (**Spaces Command**, **Intel**, **Beams**, or **Explorer**).

### Cross-Module Synergies
- **With Spaces Command**: Connect Spaces Command's `VOICE 1 PITCH` & `GATE` to Stellar's `VOCT 1` & `GATE 1`, and `VOICE 2 PITCH` & `GATE` to Stellar's `VOCT 2` & `GATE 2`. This creates an instant dual-timbre performance synthesizer where Scene A drives a lead and Scene B drives an arpeggiated bassline.
- **With Explorer**: Patch Stellar's `MASTER L/R` outputs directly into Explorer. Explorer's tape delay, diffusion reverb, and octave shimmer bloom elevate Stellar's Moog ladder filter into lush cinematic soundscapes.
- **With Intel**: Connect Intel's `TRIG 1–4` rhythmic pulses into Stellar's `MOD 1` or `MOD 2` jacks for synchronized tremolo and rhythmic gating.
- **With Beams**: Route Beams' external percussion hits into Stellar's `EXT IN` jack to process drum hits through Stellar's master stereo bus.

---

## User Guide & Controls

```
┌───────────────────────────────────────────────────┐
│                   STELLAR  14 HP                  │
│                                                   │
│  I/O 1: (VOCT 1)  (GATE 1)  (MOD 1)   [SUB 1]     │
│  I/O 2: (VOCT 2)  (GATE 2)  (MOD 2)   [SUB 2]     │
│  AUX:   (EXT IN)  [NOISE]   [OUT L]   [OUT R]     │
│                                                   │
│  VOICE 1                                          │
│  [AN]      [FM]       [SS]      [PL]              │
│  analog    freq mod   supersaw  pulse             │
│  [ATTACK]  [DECAY]    [SUSTAIN] [RELEASE] [CUTOFF]│
│                                                   │
│  VOICE 2                                          │
│  [AN]      [FM]       [SS]      [PL]              │
│  analog    freq mod   supersaw  pulse             │
│  [ATTACK]  [DECAY]    [SUSTAIN] [RELEASE] [CUTOFF]│
└───────────────────────────────────────────────────┘
```

### 1. Audio & CV I/O Section (Top Card)
- **VOCT 1 / VOCT 2 Inputs**: Standard 1V/Octave calibrated pitch inputs. Features fast legato-safe retriggering: pitch shifts occurring while gate remains high re-articulate the voice seamlessly.
- **GATE 1 / GATE 2 Inputs**: Active-high gate inputs (+1V threshold) that trigger the internal ADSR envelope and oscillator voice.
- **MOD 1 / MOD 2 Inputs (0–10V)**: External VCA modulation inputs. Multiplies with the internal envelope (`Output = Envelope × MOD`). When unpatched, normalled to +10V (fully open).
- **SUB 1 Output**: Dedicated square-wave sub-oscillator output tuned **-1 octave** below Voice 1, shaped by Voice 1's envelope.
- **SUB 2 Output**: Dedicated square-wave sub-oscillator output tuned **-2 octaves** below Voice 2, shaped by Voice 2's envelope.
- **EXT IN**: Mono audio input normalled across both stereo master channels for blending external drum or synth modules.
- **NOISE Output**: Standalone unshaped analog-style white noise source (±5V), always active.
- **MASTER L / MASTER R**: Stereo master mix outputs combining Voice 1, Voice 2, and EXT IN.

### 2. Voice 1 & Voice 2 Synthesizer Engines
Each voice offers four combinable oscillator models and an analog-modeled ladder filter:

- **Waveform Selector Buttons**:
  - **AN (Analog)**: Rich, warm sawtooth with subtle even-harmonic warmth.
  - **FM (Frequency Modulation)**: Dual-operator FM with dynamic harmonic sidebands, ideal for metallic bells and crystalline tones.
  - **SS (Supersaw)**: Multi-oscillator detuned saw stack with wide stereo phase dispersion.
  - **PL (Pulse)**: Symmetrical square wave with bold odd harmonics.
  - *Stacking*: You can engage multiple waveform buttons simultaneously to create layered hybrid sounds.
- **ATTACK (1 ms – 4 s)**: Initial envelope rise time from zero to peak.
- **DECAY (1 ms – 4 s)**: Envelope drop time from peak to sustain level.
- **SUSTAIN (0% – 100%)**: Continuous level held while gate remains high.
- **RELEASE (1 ms – 4 s)**: Envelope tail duration after gate drops low.
- **CUTOFF (0% – 100%)**: Controls the cutoff frequency of the **4-pole (-24 dB/oct) Moog-style resonant ladder filter**. Features internal bass compensation to maintain low-end punch even as resonance climbs.

---

## Technical Specifications

- **Width**: 14 HP (71.12 mm)
- **Height**: 3U (128.5 mm physical standard / bit-for-bit 380px VCV grid height)
- **Depth**: 28 mm
- **Polyphony**: 2 independent monophonic voice engines + 2 sub-oscillators
- **Pitch Tracking**: 1V/Octave over 8 octaves (-2V to +6V)
- **Envelope Time**: 1 ms to 4.0 seconds per stage
- **Filter**: 4-pole low-pass ladder (-24 dB/oct) with active low-end compensation
- **Signal Levels**: Audio outputs ±5V (10Vpp), Gate inputs +1V to +10V

---

## Building and Installation

### Prebuilt Plugin Package
Download `Stellar-2.0.0-<platform>.vcvplugin` from the [Releases](https://github.com/Grandsummoner/stellar/releases) section and copy it to your VCV Rack `plugins` directory:
- **Windows**: `Documents/Rack2/plugins/`
- **macOS**: `Documents/Rack2/plugins/`
- **Linux**: `~/.Rack2/plugins/`

### Building from Source
Ensure you have the [VCV Rack SDK v2](https://vcvrack.com/downloads/) installed.

```bash
# Clone the repository
git clone https://github.com/Grandsummoner/stellar.git
cd stellar

# Set your Rack SDK directory
export RACK_DIR=/path/to/Rack-SDK

# Build the distributable package
make -j2 dist
```

The compiled package will be located in `dist/Stellar-2.0.0-<platform>.vcvplugin`.

---

## License

This software is released under the **GNU General Public License v3.0 or later** (GPL-3.0-or-later).  
Copyright © 2026 Grandsummoner. All rights reserved.
