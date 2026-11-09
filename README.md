# Grandsummoner Stellar

**Stellar** is a 14 HP dual-voice Eurorack synthesizer companion module for [VCV Rack v2](https://vcvrack.com/).

It features 4 switchable oscillator models per voice (Analog, FM, Supersaw, Pulse) routed into a shared 4-pole Moog-style ladder filter, integrated ADSR envelope generator, external MOD input (VCA / tremolo), dedicated per-voice sub-oscillator outputs, standalone noise generator, and an external audio input mixed with Voice 1 & 2 before the stereo outputs.

## Family Adjacency (Connector LED)
Stellar functions completely standalone with standard 1V/OCT, GATE, and MOD inputs. When placed directly adjacent to any other Grandsummoner family module (**Spaces Command**, **Intel**, **Beams**, or **Explorer**), the side connector LEDs automatically light up to confirm physical alignment.

## Building from Source

### Prerequisites
- [VCV Rack SDK v2](https://vcvrack.com/downloads/)
- C++17 compatible compiler toolchain (`make`, `g++`, `mingw-w64`)

### Build Commands
```bash
# Set path to your Rack-SDK directory
export RACK_DIR=/path/to/Rack-SDK

# Build the distributable plugin package
make -j2 dist
```

The resulting package will be placed in `dist/Stellar-2.0.0-<platform>.vcvplugin`.

## License
GPL-3.0-or-later. Created by Grandsummoner.
