---
title: INTERSECT - A nondestructive, time-stretching, and intersecting sample slicer 
date: 2026-02-27 07:00:00 +0100
categories: [Blog, Audio Production]
tags: [Fedora, Audio Production, Music Production, Linux, Plugin, VST3, LV2, Clap, Sampler]
image: assets/img/INTERSECT.png
---

I have just added a new plugin called INTERSECT. To my [timlau/audio](https://copr.fedorainfracloud.org/coprs/timlau/audio/) COPR repository.

[INTERSECT](https://github.com/tucktuckg00se/INTERSECT) is a nondestructive, time-stretching, and intersecting sample slicer plugin with independent per-slice parameter control, per-slice locking, multiple time/pitch algorithms, and MIDI-triggered slice playback.

[Check here for install instructions](/posts/fedora-audio-timlau-audio/#intersect)

## Workflow Basics 

1. **One sample at a time:** INTERSECT loads one audio file per instance (`.wav`, `.ogg`, `.aiff`, `.flac`, `.mp3`).
2. **Slice creation:** Draw slices manually, chop live with **LAZY**, or split via **AUTO**.
3. **Inheritance model:** Header controls are sample defaults. Slice controls can lock overrides per field.
4. **Playback model:** MIDI triggers slices by note mapping; mute groups can choke voices in the same group.
5. **Load behavior:** File decoding/loading is asynchronous (off the audio thread).
6. **Algorithms:**
   - `Repitch`: pitch and speed are linked.
   - `Stretch`: independent time/pitch via Signalsmith Stretch (`TONAL`, `FMNT`, `FMNT C`).
   - `Bungee`: granular stretch mode with `GRAIN` choices (`Fast`, `Normal`, `Smooth`).
7. **Repitch + Stretch interaction:** when `ALGO=Repitch` and `STRETCH=ON`, `PITCH`/`TUNE` become BPM-driven read-only displays.
8. **SET BPM:** compute BPM from selected slice length (or full sample context) against a musical duration.
9. **MIDI host stop handling:** responds to `All Notes Off (CC 123)` and `All Sound Off (CC 120)`.
10. **Undo/redo:** snapshot-based history for slice and parameter edits.
