---
title: Audio applications in timlau/audio repository
date: 2026-02-02 07:21:00 +0100
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

OB-Xf is a Synth based on the legendary Oberheim OB-X.
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
Lost N' Found Piano, a virtual instrument plug-in that combines updated versions of the classic mda Piano and mda EPiano VSTs and gives them a new coat of paint.

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

JUCE exist in multiple mayor versions both 8.0 and 7.0 and multiple minor versions. (8.0.11, 8.0.6, 7.0.12)
different plugins need different versions of JUCE to compile.

```terminal
sudo dnf install JUCE8.0-devel-8.0.11
sudo dnf install JUCE8.0-devel-8.0.6
sudo dnf install JUCE7.0-devel
```
