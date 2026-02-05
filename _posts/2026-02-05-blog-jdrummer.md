---
title: New plugin - jdrummer
date: 2026-02-05 13:00:00 +0100
categories: [Blog, Audio Production]
tags: [Fedora, Audio Production, Music Production]
image: assets/img/jdrummer.png
---

## Introduction

I have added a new plugin - jdrummer to my [timlau/audio](https://copr.fedorainfracloud.org/coprs/timlau/audio/) COPR repository.

[jdrummer](https://github.com/jmantra/jdrummer) is a Soundfont-based drum kit plugin, a comprehensive groove library with tempo-synced playback,
a composition tool, and an intelligent Groove Matcher that analyzes audio to find matching drum patterns.

[Check here for install instructions](/posts/fedora-audio-timlau-audio/#jdrummer)

**Here is an overview of the plugin's features:**

### Drum Pads
- **16-pad drum grid** with velocity-sensitive playback
- **Multiple Soundfont kits** - Ships with 28 drum kits including:
  - Standard acoustic kits (Standard, Room Drums, Power Drums, Jazz Drums)
  - Electronic kits (808, Electronic Drums, Dance Drums, House Kit)
  - Specialty kits (Orchestral Percussion, Brush Drums, NIN Drumkit)
- **Per-pad controls**:
  - Individual volume adjustment (0-100%)
- Pan control (left/right) (Panning is currently backwards, see issue 10: https://github.com/jmantra/jdrummer/issues/10 )
- Solo and mute options
- **Dynamic kit loading** - Add your own .sf2 SoundFont files to expand your library
- **Multi Out Support** - Fan each drum pience to an individual track for mixing


### 🎵 Grooves Browser
- **Extensive groove library** organized by category:
  - Basic Beats
  - Break Beats
  - Buildups
  - Double Bass Beats
  - Fills
  - Half Time Beats
  - OffBeats
  - Swing Beats
  - Tom Beats
- **Tempo-synced playback** - Grooves automatically sync to your DAW's tempo
- **Preview functionality** - Audition grooves before adding them to your project
- **Drag and drop** - Drag any groove directly into your DAW as a MIDI clip
- **Bar selection** - Choose how many bars of a groove to use (1-16 bars)
- **Dynamic Groove Loading** add your own drum grooves

### 🎼 Composer
- **Build complete drum parts** by combining multiple grooves
- **Visual timeline** showing your arrangement
- **Reorder and remove** items from your composition
- **Export as MIDI** - Drag your entire composition to the DAW
- **Loop playback** for previewing your arrangement

### 🎯 Groove Matcher
An intelligent feature inspired by professional drum software that helps you find the perfect groove for your music:

- **Audio analysis** - Drop any audio file (WAV, MP3, FLAC, OGG, AIFF) to analyze its rhythm
- **BPM detection** - Automatically detects tempo using the minibpm library
- **Smart filename parsing** - Extracts BPM from filenames (e.g., "beat_120bpm.wav")
- **Pattern matching** - Analyzes rhythm patterns and finds matching grooves from your library
- **Similarity scoring** - Shows match percentage for each suggested groove
- **Preview with audio** - Play back the matched groove alongside your original audio
- **Automatic composition** - Best match is automatically added to the composer
- **Seamless workflow** - Found the perfect match? Drag it straight to your DAW

**Here is a teaser video of the plugin in action:**
{% include embed/youtube.html id='mbGQnUJ8rxg' %}
