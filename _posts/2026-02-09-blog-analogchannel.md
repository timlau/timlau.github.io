---
title: New plugin - AnalogChannel
date: 2026-02-09 14:00:00 +0100
categories: [Blog, Audio Production]
tags: [Fedora, Audio Production, Music Production, Linux, Plugin, VST3, LV2, Clap, Effect]
image: assets/img/AnalogChannel.png
---

## Introduction

I have added a new plugin **AnalogChannel** to my [timlau/audio](https://copr.fedorainfracloud.org/coprs/timlau/audio/) COPR repository.

[AnalogChannel](https://github.com/FilTer87/VST-AnalogChannel) is a channel strip plugin designed for mixing engineers who demand fast and characterful results in their workflow.

Each section provides carefully limited controls: fixed attack/release times, discrete frequency selections, and pre-configured parameters (both fixed and dynamic) working under the hood to deliver professional results with most source material. This is your go-to channel strip for fast, colored, musical mixing decisions.

It is not intended for surgical precision!

Built with faithful ports of legendary algorithms from Airwindows and classic JSFX processors.

**Key Features**

 - Dual-Mono Architecture: Left and right channels process independently, enabling analog channel modeling through the Channel Variation system
 - Channel Variation System: Emulates natural component tolerances in analog consoles with 48 unique channel presets (see UserManual.md for details)
 - Independent Bypass: All sections feature smooth 10ms crossfade CPU-efficient bypass, for A/B comparison without clicks and resource optimization.
 - Flexible Signal Routing: Style Comp. can be placed pre or post-EQ, filters can be routed post-OutStage for creative effects
 - Comprehensive Metering: Input/output peak meters plus dedicated GR meters for dynamics sections
 - Full DAW Automation: All parameters support VST3 automation and MIDI control
 - Zero Latency: Real-time processing suitable for tracking and mixing

**Processing sections**

- Input stage saturation: 4 modes to choose between Clean (digital gain), Pure (transparent saturation), Tape (vintage reel saturation with flutter and head bump), and Tube (3-stages asymmetric harmonics); DSP ported from AirWindows
- HPF/LPF filters with "Bump" option (higher Q factor) and switchable slopes
- "Clean" Compressor: Transparent peak control for taming dynamics before EQ
- Low Dynamic custom design section: Dual-mode dynamics processor for signals below the threshold; a custom 1-knob approach that works as either a downward expander/gate or an upward compressor
- 4 bands EQ with custom design: Musical baxandall shelving + parametric EQ, using custom curves with dynamic Q (similar to an API-style EQ); Mid-Cut control for precise mid-range shaping added to the original baxandall shelves.
- Style Compressor with Two character compression modes: "Warm" (optical CL1B-style) that with the coloration and adaptive attack/release time adds warmth, glue and vibes, and "Punch" mode to enhance the initial parts of the transients on percussive elements
- Console Emulation: Choose one of the magic console tones between Essex (Neve), Oxford (SSL style), and USA (API); DSP ported from AirWindows Output Stage - Final stage with saturation and clipping options (Hard/Soft); DSP ported from

[Check here for install instructions](/posts/fedora-audio-timlau-audio/#analog-channel)
