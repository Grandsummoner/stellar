---

# 3. Stellar (`stellar/README.md`)

```markdown
# Grandsummoner Stellar

> **14 HP Dual-Voice Multi-Model Synthesizer Companion**

<p align="center">
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
