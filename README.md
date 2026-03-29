# Active 2-Way Crossover DSP (AT-2XDSP)

![DSP](https://img.shields.io/badge/DSP-RealTime-blue)
![Platform](https://img.shields.io/badge/Platform-JamesDSP-green)
![Status](https://img.shields.io/badge/Status-Active-success)
![CPU](https://img.shields.io/badge/CPU-Mobile%20Optimized-orange)

AT-2XDSP is a real-time 2-way crossover DSP project for JamesDSP LiveProg, designed for clean subwoofer control, tight low-end behavior, controlled ultra-low response, and stable playback in mobile or embedded audio workflows.

This repository contains multiple AT-2XDSP versions for testing, comparison, and tuning.

## Documentation

- [Dokumentasi Bahasa Indonesia](./README_ID.md)
- [English Documentation](./README_EN.md)

## Related JamesDSP Projects

- JamesDSP Linux / PipeWire-PulseAudio port: https://github.com/ppw0/jamesdsp
- Rootless JamesDSP for non-rooted Android devices: https://github.com/timschneeb/RootlessJamesDSP
- JamesDSP Android framework variant: https://github.com/james34602/JamesDSPManager

## What this project focuses on

- LR4 crossover design
- Subsonic protection and ultra-low control
- Phase alignment and all-pass compensation
- Transient control for kick, clap, and snare bleed
- Lightweight mobile-friendly DSP variants
- Stable tuning for everyday playback and live-style use

## Sound signature

- Tight subwoofer response
- Controlled ultra-low “glerr”
- Clean mid/sub separation
- High SPL with discipline
- Avoids boomy, blurred, or uncontrolled bass behavior

## Version guide

| Version | Character | Best for |
|--------|-----------|----------|
| V1–V16 | Development / earlier tuning stages | Testing and comparison |
| V17 | Stable / Clean | Daily use and reliable playback |
| V18 | Ultra Low Enhanced | Deeper bass feel with controlled pressure |
| V19 | Experimental / Heavy | Advanced processing and higher CPU demand |
| V20 | Mobile Optimized | Lighter build for smoother real-time performance |

## Recommended starting points

- Use the stable version if you want the safest default behavior.
- Use enhanced versions only if your device and audio engine can handle the extra processing load.
- Keep headroom safe because the project does not include a limiter or clipper.

## Quick start

1. Install JamesDSP on your device.
2. Open LiveProg or the matching processing engine.
3. Paste the DSP script from the version you want to test.
4. Tune the parameters gradually.
5. Compare versions and keep the one that matches your playback system.

## Compatibility notes

This project is intended for:
- JamesDSP LiveProg scripting workflows
- Android audio processing setups
- Real-time experimentation on supported devices
- Mobile-friendly DSP tuning and testing

## License / usage

This project is intended for learning, experimentation, and personal tuning workflows. Use responsibly in any live or high-power playback system.
