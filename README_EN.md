# AT-2XDSP — Active 2 Way Crossover LR4 DSP Processor

**AT-2XDSP** is a real-time **DSP crossover script** for **JamesDSP LiveProg**, designed to shape subwoofer behavior into something **tight, clean, precise, and still capable of deep ultra-low “glerr”** without turning the system into a boomy mess.

This repository follows a pro-audio style approach: **phase-aware, crossover-controlled, and headroom-conscious**.

---

## Overview

AT-2XDSP focuses on three core goals:

1. **Clean separation between sub and mid**
2. **Deep but controlled subwoofer character**
3. **Transient protection so upper-frequency energy does not leak into the sub path**

The result is a sound that feels big, strong, and alive, while still being pleasant for long listening sessions.

---

## Main Features

- **LR4 crossover** for precise sub/mid separation
- **Subsonic protection** to remove unnecessary ultra-low rumble
- **Phase alignment** to help sub and mid lock together
- **All-pass compensation** for additional phase correction
- **Ultra Low Enhancer** to strengthen 30–45 Hz without making the system boomy
- **Auto headroom** to gently reduce gain when output becomes too dense
- **Transient guards** to reduce hi-hat, clap, kick attack, and snare-body leakage into the sub path
- **Mobile-oriented design**: optimized to remain practical on everyday devices, even though more advanced versions can be heavier

---

## Sound Philosophy

This project is not just about “more bass”. It is about:

- bass that can be **felt**
- bass that has **shape**
- bass that **stops cleanly**
- bass that does **not smear into the midrange**

If a system sounds big but blurred, the usual problems are:
- crossover overlap
- phase mismatch
- weak transient control
- insufficient headroom

AT-2XDSP tries to address those problems with a simple but effective approach.

---

## Available Versions

### V17 — Stable Core + Ultra Low Enhancer
This is the safest and most balanced baseline.

**Main traits:**
- clean
- tight
- stable
- lively sub response
- suitable for daily use

**Sound character:**
- precise sub behavior
- strong SPL without chaos
- enough ultra-low “glerr”
- limited dynamic complexity

**Best for:**
- users who want a safe, stable default
- devices with limited CPU headroom
- daily tuning without extra complexity

---

### V18 — Hajatan Killer / Scene-Based Mode
This version explores a more aggressive, live-event-oriented character.

**Important note:**
- more experimental than V17
- can feel more energetic and more “open”
- enjoyable on stronger devices
- may be heavier on weaker devices

**Sound character:**
- thicker
- bigger
- more live-sound-like
- still controlled, but more adventurous

**Best for:**
- experimentation
- devices with extra performance headroom
- users who want a festival / live-party feel

---

### V19 — Adaptive Music Analyzer
This version adds adaptive music analysis that observes low, mid, and high energy in real time.

**Important note:**
- the most complex version
- the most feature-rich
- also the most demanding for CPU/phone hardware

**Sound character:**
- smarter automatic behavior
- can feel very advanced on stronger hardware
- may cause crackling or dropout if the device is overloaded

**Best for:**
- advanced experimentation
- strong hardware
- users who want automatic tone adaptation

---

### V20 — Mobile Optimized High-Quality
This version balances sound quality and computational load.

**Main goal:**
- keep a high-end sound character
- remain clean
- be much lighter than highly layered guard/analyzer versions

**Sound character:**
- more stable
- safer on phones
- still delivers premium sub behavior
- better for daily mobile use

**Best for:**
- phones
- medium or large buffers
- users who want stability first

---

## Version Recommendation

If you want to choose by use case:

- **V17** → safest overall choice
- **V18** → more aggressive character
- **V19** → most advanced, but heaviest
- **V20** → best mobile-friendly balance

---

## Example Tone Goals

### Cleaner, safer sub
- keep crossover restrained
- avoid excessive body shelf
- keep subsonic protection active
- use only moderate auto headroom

### More obvious ultra-low feel
- raise Ultra Low Enhancer slightly
- keep body shelf modest
- avoid widening crossover too much

### Less boom and more control
- reduce sub-bass amount
- avoid overemphasis in 50–80 Hz
- keep phase alignment enabled

---

## Performance Notes

Because this is **real-time per-sample DSP**, hardware quality matters a lot.

Things that can make playback unstable:
- too many guards
- overly complex analyzers
- too-small audio buffers
- unnecessary convolver or extra engine modules

If the device starts to crackle:
- choose a lighter version
- disable non-essential processing
- increase buffer size if your setup allows it

---

## Installation

1. Install JamesDSP
2. Open **LiveProg**
3. Paste the AT-2XDSP script you want to use
4. Save and enable the preset
5. Fine-tune parameters for your speaker system

---

## System Requirements

Minimum recommended:
- Android device with JamesDSP
- CPU capable of stable realtime audio
- medium or large audio buffer

More comfortable if:
- the device is not running too many background apps
- the audio engine is not forced to share too many extra effects
- heavy charging and heavy audio processing are not combined when the device is already struggling

---

## FAQ

### Why does the sub feel big but still tight?
Because crossover, phase alignment, and transient guards are tuned so the sub stays focused and does not spill into other bands.

### Why do some versions crackle?
Usually because that version is too heavy for the device being used, not because the DSP idea is wrong.

### Why are there multiple versions?
Different devices and different sound goals need different trade-offs. Some versions are safe, some aggressive, some experimental.

### Why does ultra-low feel better on some songs?
Because the mix itself is different. Not every track contains the same amount of 30–45 Hz energy.

---

## Contributing

Useful contributions include:
- CPU optimization
- clearer parameter documentation
- better tuning notes
- lighter-device versions
- version-by-version sound character notes

---

## License

This repository is intended for learning, experimentation, and personal audio tuning. Use responsibly, especially on powerful speaker and amplifier systems.

---

## Closing

AT-2XDSP is built for listeners who want bass that is **large, clear, and controlled**.  
Not just loud, but shaped, musical, and enjoyable for long sessions.
