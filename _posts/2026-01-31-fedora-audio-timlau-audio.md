---
title: Audio applications in timlau/audio repository
date: 2026-02-06 11:40:00 +0100
categories: [Fedora, Audio Production]
tags: [Fedora, Audio Production, Music Production]
image: assets/img/pexels-tima-miroshnichenko-4988137.jpg  
pin: true
---

I have created a [timlau/audio](https://copr.fedorainfracloud.org/coprs/timlau/audio/) COPR repository to make it easier to install some audio plugins in Fedora 42+, spec files and Makefiles to build the packages is available on [github](https://github.com/timlau/audio_spec_files)

### You can enable the repository using
```terminal
sudo dnf enable timlau/audio
```

## Instruments

### Loopino
![Loopino](assets/img/loopino.png){: .shadow }
[Loopino](https://github.com/brummer10/Loopino) is a lightweight audio sampler. It allows you to load, trim, and loop audio files with precision, making it ideal for crafting seamless sample loops. With a clean, minimal interface, Loopino fits perfectly into any audio workflow — whether for sound design, live performance, or creative sampling experiments.

```terminal
sudo dnf install Loopino-clap
sudo dnf install Loopino
```

### Wavetable
![Wavetable](assets/img/Wavetable.png){: .shadow }
[Wavetable](https://socalabs.com/synths/wavetable/) is A 2 oscillator wavetable synthesizer with flexible modulation options.

```terminal
sudo dnf install Wavetable-vst3
sudo dnf install Wavetable-lv2
sudo dnf install Wavetable-clap
sudo dnf install Wavetable
```

### jdrummer
![jdrummer](assets/img/jdrummer.png){: .shadow }
 [jdrummer](https://github.com/jmantra/jdrummer) is a Soundfont-based drum kits, a comprehensive groove library with tempo-synced playback,
a composition tool, and an intelligent Groove Matcher that analyzes audio to find matching drum patterns.

```terminal
sudo dnf install jdrummer-vst3
sudo dnf install jdrummer-lv2
sudo dnf install jdrummer-clap
sudo dnf install jdrummer
```


### Vaporizer2
![Vaporizer2](assets/img/Vaporizer2.png){: .shadow }

[Vaporizer2](https://github.com/VASTDynamics/Vaporizer2) is a hybrid wavetable additive / subtractive synthesizer / sampler workstation
created by [VAST Dynamics](https://www.vast-dynamics.com/).
Vaporizer2 comes with a groundbreaking wavetable editor with a vast number of editing possibilities including
frequency shift, smooth, clean, bend and bloat for single-cycles, parts of single-cycles or even whole wavetables.
Featuring an easy-to use wavetable draw mode with smooth Bezier curves and snap to grid function.

```terminal
sudo dnf install Vaporizer2-vst3
sudo dnf install Vaporizer2-lv2
sudo dnf install Vaporizer2-clap
sudo dnf install Vaporizer2
```
Extra patches can be downloaded from [here](https://www.vast-dynamics.com/?q=presets)


### Dexed
![Dexed](assets/img/dexed.png){: .shadow }

[Dexed](https://asb2m10.github.io/dexed/) is a synth that is closely modeled on the Yamaha DX7

```terminal
sudo dnf install dexed-clap
sudo dnf install dexed-vst3
sudo dnf install dexed
```

### Odin 2
![odin2](https://cdn.shopify.com/s/files/1/0641/1304/9835/files/odin.2.4_fading.png?v=1748421452){: .shadow }

[Odin 2](https://thewavewarden.com/pages/odin-2) is a 24-voice polyphonic powerhouse that will transport you from your studio straight to Valhalla.
Whether you're after earth-shattering basses, soaring leads, or otherworldly FX, Odin 2 delivers it all.
Harness the classic warmth of analog waveforms — or draw custom ones. 
High-quality emulations of legendary analog filters, like the Moog Ladder, the Korg 35 and many more let you shape your sound. 
Finish it off with five onboard FX or dive into endless modulation possibilities. 
There’s a whole world to explore in Odin 2.

```terminal
sudo dnf install odin2-vst3
sudo dnf install odin2-lv2
sudo dnf install odin2
```

### Crypt2
![crypt2](https://camo.githubusercontent.com/6a946eeb9d6a1b116ead1f865a2813692f6f50b7120e5185dbf21354821be0c4/68747470733a2f2f7777772e7669746c696e672e78797a2f63727970742f7265736f75726365732f63727970742d73637265656e73686f742e6a7067){: .shadow }

[Crypt](https://www.vitling.xyz/crypt/) is a software synthesiser plugin designed for creating spacious cold hyper-unisoned
synth sounds

```terminal
sudo dnf install Crypt2-vst3
sudo dnf install Crypt2-clap
sudo dnf install Crypt2-lv2
sudo dnf install Crypt2
```

### OB-Xf
![OB-Xf](assets/img/OBXf.png)

[OB-Xf](https://github.com/surge-synthesizer/OB-Xf) is a Synth based on the legendary Oberheim OB-X.
OB-Xf is a continuation of the last open source version of OB-Xd by 2DaT and later discoDSP,
bringing together several efforts going on in the audio space and combining them inside the Surge Synth Team infrastructure.
The synth is currently in a beta phase, with a few features still under development, but the plugin is feature stable and working rather well,we believe.

```terminal
sudo dnf install OB-Xf-vst3
sudo dnf install OB-Xf-clap
sudo dnf install OB-Xf-lv2
sudo dnf install OB-Xf
```

### Lost N' Found Piano
![lostandfoundpiano](https://github.com/timlau/lost-and-found-piano/raw/main/images/Screenshot.png){: .shadow }
[Lost N' Found Piano](https://github.com/surge-synthesizer/OB-Xf), a virtual instrument plug-in that combines updated versions of the classic mda Piano and mda EPiano VSTs and gives them a new coat of paint.

```terminal
sudo dnf install LostAndFoundPiano-vst3
sudo dnf install LostAndFoundPiano-clap
sudo dnf install LostAndFoundPiano-lv2
sudo dnf install LostAndFoundPiano
```

### Sfizz
[Sfizz](https://sfztools.github.io/sfizz/) is a sample-based musical synthesizer.
It features the well-established SFZ instrument format at its core, which permits to use existing instrument libraries, or create personal instruments with ease. Not only is sfizz ready-to-use as an instrument plugin of its own, the library allows developers to create instruments of their own, taking advantage of the abilities of SFZ.

```terminal
sudo dnf install sfizz-vst3
sudo dnf install sfizz-lv2
```

### Geonkick
Geonkick is a synthesizer that can synthesize elements of percussion. The most basic examples are: kicks, snares, hit-hats, shakers, claps.

```terminal
sudo dnf install geonkick
sudo dnf install geonkick-lv2
```

## Effects

### ZL Compressor
![ZLCompressor](assets/img/ZLCompressor.png)

[ZL Compressor](https://zl-audio.github.io/plugins/zlcompressor/) is 
ZL Equalizer is an equalizer plugin with the following key features:

- **Multiple Filter Settings:** Supports 6 filter structures, 16 frequency bands, 8 filter types, 5 stereo modes, 7 variable slopes.
- **High-Quality Sound:** With 64-bit floating-point processing and de-cramping technique, outstanding performance is ensured in both low-end and high-end.
- **Adjustable Dynamics:** Adjustable threshold, attack, release, and side-chain frequency, etc.
- **Carefully Designed Interface:** Interactive spectrum graph, smart collision detection, and smooth animations.

```terminal
sudo dnf install ZLCompressor-vst3
sudo dnf install ZLCompressor-lv2
```


### Setekh
![setekh](assets/img/setekh.png)

[Setekh](https://fullfxmedia.com/plugins/setekh) is a minimalistic yet sonically powerful distortion plugin

Setekh is a god of deserts, storms, disorder, violence, and foreigners in ancient Egyptian religion.

```terminal
sudo dnf install setekh-vst3
sudo dnf install setekh-clap
sudo dnf install setekh-lv2
sudo dnf install setekh
```


### Analog Channel
![AnalogChannel](assets/img/AnalogChannel.png)
[Analog Channel](https://github.com/FilTer87/VST-AnalogChannel) is a channel strip plugin designed for mixing engineers who demand fast and characterful results in their workflow.
Each section provides carefully limited controls: fixed attack/release times, discrete frequency selections, and pre-configured parameters (both fixed and dynamic) working under the hood to deliver professional results with most source material. This is your go-to channel strip for fast, colored, musical mixing decisions.

```terminal
sudo dnf install AnalogChannel-vst3
sudo dnf install AnalogChannel-clap
sudo dnf install AnalogChannel-lv2
sudo dnf install AnalogChannel
```


### Build Your Own Distortion (BYOD)
![BYOD](assets/img/BYOD.png)
[BYOD](https://github.com/Chowdhury-DSP/BYOD) is a guitar effects plugin with a customisable signal chain that allows users to create their own guitar distortion effects. The plugin contains a wide variety of distortion effects from analog modelled circuits to purely digital creations, along with some musical tone-shaping filters, and a handful of other useful signal processors.

```terminal
sudo dnf install BYOD
sudo dnf install BYOD-lv2
sudo dnf install BYOD-clap
sudo dnf install BYOD-vst3
```
The manual is available [here](https://github.com/Chowdhury-DSP/BYOD/blob/main/manual/Manual.md#byod-user-manual)

### Neural Amp Modeler 
Neural Amp Modeler is a plugin that allows you to model the sound of an physiGuitar amplifier and cabinet.

```terminal
sudo dnf install neural-amp-modeler-lv2
```

### AIDA-X
AIDA-X is an Amp Model Player, allowing it to load models of AI trained music gear, which you can then play through guitar

```terminal
sudo dnf install AIDA-X-clap
sudo dnf install AIDA-X-vst3
sudo dnf install AIDA-X-lv2
sudo dnf install AIDA-X
```
### Dragonfly Reverb
Dragonfly Reverb is a bundle of free audio effects for Linux, MacOS, and Windows. The reverb algorithms are based on the original Freeverb. The DR-1 algorithm is based on the Schroeder/Moorer reverb. The DR-2 algorithm is based on the original Freeverb algorithm. The DR-3 algorithm is a unique reverb algorithm developed by Michael Willis.

```terminal
sudo dnf install dragonfly-reverb-clap
sudo dnf install dragonfly-reverb-vst3
sudo dnf install dragonfly-reverb-lv2
sudo dnf install dragonfly-reverb
```

### YK Chorus
A chorus effect inspired by the one found in certain well-known Japanese vintage analog synthesizers (Juno 60)

```terminal
sudo dnf install ykchorus-clap
sudo dnf install ykchorus-vst3
sudo dnf install ykchorus-lv2
sudo dnf install ykchorus
```

## Applications

### Polyphone
Polyphone is a multiplatform and open-source soundfont editor for creating musical instruments.

* editing of sf2, sf3, sfz and sfArk file formats
* compatible with Jack and ASIO audio servers
* built-in synthesizer, controlled by a virtual keyboard or MIDI signals
* automatic recognition of root keys
* automatic loop of samples
* simultaneous editing of parameters
* specific tools for musical instrument creation
* recorder to keep a trace of what is played in a .wav file
* soundfont browser connected to the online repository

```terminal
sudo dnf install polyphone
```

## Development

### JUCE
[JUCE](https://juce.com/) is an open-source cross-platform C++ application framework for creating desktop and mobile applications, including VST, VST3, AU, AUv3, AAX and LV2 audio plug-ins and plug-in hosts.
This package is used to build application there is using the JUCE framework, so the package don't need to have the whole JUCE source and build it every time.
a very basic dummy plugin made with JUCE is located [Here](https://github.com/timlau/juce-test)

JUCE exist in multiple mayor versions both 8.0 and 7.0 and multiple minor versions. (8.0.12, 8.0.11, 8.0.6, 7.0.12)
different plugins need different versions of JUCE to compile.

```terminal
sudo dnf install JUCE8.0-devel-8.0.12
sudo dnf install JUCE8.0-devel-8.0.11
sudo dnf install JUCE8.0-devel-8.0.6
sudo dnf install JUCE7.0-devel
```
