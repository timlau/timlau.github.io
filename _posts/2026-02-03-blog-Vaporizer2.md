---
title: New plugin - Vaporizer2
date: 2026-02-03 08:00:00 +0100
categories: [Blog, Audio Production]
tags: [Fedora, Audio Production, Music Production]
image: assets/img/Vaporizer2.png
---

I have added a new plugin - Vaporizer2 to my [timlau/audio](https://copr.fedorainfracloud.org/coprs/timlau/audio/) COPR repository.

[Check here for install instructions](/posts/fedora-audio-timlau-audio/#vaporizer2)

It is a power house of a wavetable synthesizer sampler plug-in.

Here is what the creator of Vaporizer2 has to say about it:

 **PROBABLY THE MOST VERSATILE WAVETABLE SYNTHESIZER**

We're excited to announce that VAST Dynamics' hybrid wavetable synthesizer sampler plug-in, Vaporizer2, is now freely available as Open Source software under GPL3. This milestone comes after five years of dedicated development and we are thrilled to share it with the public. The project is readily available on GitHub for anyone interested in participating.

Vaporizer2 is a hybrid wavetable additive / subtractive VST / AU / AAX / LV2 synthesizer / sampler workstation.

The heart of this plugin is the alias-free versatile high-performance wavetable sound engine with low system CPU resource usage and a unique architecture allowing to freely change and even exchange / load wavetables while playing without aliasing.

Vaporizer 2 comes with a groundbreaking wavetable editor with a vast number of editing possibilities including frequency shift, smooth, clean, bend and bloat for single-cycles, parts of single-cycles or even whole wavetables.

Featuring an easy-to use wavetable draw mode with smooth Bezier curves and snap to grid function.

Includes 780+ wavetables and single cycles and 450+ factory presets.

Vaporizer 2 features a comprehensive preset management system with tags, free text search, file system folder management and ratings.

Low system CPU resource usage - even with more than 1.000 oscillators playing.

All parameter knobs / sliders automatable and support manual editing for exact parameter values.

State of the art preset management system with tags, free text search, file system folder management and ratings.

Comes with a rapidly growing number of presets – freely available on the website and GitHub.

Plus: the sound is stunning.

**Oscillators, polyphony, MPE and aftertouch:**

- Mono legato mode or polyphonic 4 / 16 / 32(!) voice modes.
- Support for MIDI Polyphonic Expression (MPE): receive MPE MIDI dimensions (X/Y/Z) pitchbend, aftertouch (freely assignable), release velocity / lift (controlled via MSEG) and brightness / timbre (freely assignable) from supported controllers for highly expressive control options.
- Intelligent polyphonic portamento / glissando (you need to hear it!).
- Support for polyphonic aftertouch.
- Oscillator pitch modulation and phase modulation with very fast modulations (up to ~ 2kHz).
- Microtuning support (AnaMark Tuning files .TUN support).

**Wavetable engine:**

- Unique architecture allowing to freely change and even exchange / load wavetables while playing without aliasing.
- Engine vectorized with CPU-specific intrinsics for highest performance (SSE2/3, AVX, Neon).
- 30 real-time wavetable effects per oscillator including innovative algorithms for hard sync, sincify, brew and bend / bloat.
- FM synthesis up to a chain of 4 oscillators.
- General setting of wavetable frequency characteristics: sharp (ideal filtering), soft (butterworth filtering), dull (linear).

**Wavetable editor:**

- Groundbreaking wavetable editor with a vast number of editing possibilities including frequency shift, smooth, clean, bend and bloat for single-cycles, parts of single-cycles or even whole wavetables.
- Easy-to use wavetable draw mode with smooth Bezier curves and snap to grid function.
- Mix-in, amplitude modulate, interpolate, convolute, time>frequency, frequency>time or normalize wavetable cycles.
- Generate FM, PWM, harmonic morphed / reduced, low pass / high pass / band pass / comb / formant filtering and even hard sync wavetables out of an arbitrary single cycle waveform.
- Morphing and phase shifting of wavetable cycles.
- Import and change standard (Serum, Icarus) format wavetables - also simply via drag and drop.
- Record single cycle changes into a new wavetable.
- Additive synthesis section that allows to freely edit all harmonics and phases in real-time.

**Sampler:**

- Sampler section (wav / aiff / ogg / mp3) with loop points, loop start modulation, zero crossing detection and key tracking.
- Granular synthesis mode in the sampler section for stunning ambient effects.
- Resample samples to wavetables with pitch detection.

**Effects:**

- Three effects busses including 4 x oversampling and mono cutoff to preserve a clean low end.
- 11+ highly parameterizable effects including reverb, delay, chorus, flanger, bitcrush, eq, compressor, limiter, flanger, phaser, comb filter, waveshaper and more.
- All effect times and durations can be synced to DAW.

**Filters:**

- State of the art filter section (30+ different types) with 4 x oversampled LPF (biquad, state variable and diode ladder implementations) plus high pass, all pass, band pass, notch, shelf, comb and scream filters - all with resonance.
- Very steep filter curves for punchy basses.
- Real-time filter response display.

**Modulation matrix:**

- Comprehensive modulation system with powerful modulation matrix including graphical display of modulation curves.
- 25 modulation sources including key track, random drift and four custom macro knobs.
- 220(!) modulation destinations (modulatable parameters) for almost unlimited modulation combinations.
- Innovative audio routing system for all sound generators, filters and effect busses.

**LFOs and MSEGs:**

- Five freely editable MSEG envelopes with loop function and DAW timecode sync.
- Five LFOs (per voice - means up to 80 LFOs in total) with smooth generation optimized for lowest frequencies with ramp and phase that can be set per voice or global - can be synced to the DAW.

**Arpeggiator and Step Sequencers:**

- Built-in arpeggiator that is freely editable and supports polyphonic modes, hold and MIDI file drag and drop and can be synced to the DAW.
- Three step sequencers that can be synced to the DAW.

**Plug-in editor user interface:**

- Easy to use and intuitive user interface that is freely scalable and resizable even up to 4k and more with many drag and drop features and many graphical components, e.g. audio-out oscilloscope, filter response, MSEG / LFO / ARP.
- Polyphonic real-time visualization of parameter modulations.
- Four different UI themes to choose from allowing for different contrasts and look-and-feel.
- Hotkeys for most important editor functions.


Here is a teaser video of the plugin in action:
{% include embed/youtube.html id='pPK5q8V6PZs' %}
