---
title: Audio applications in Fedora repositories
date: 2025-02-27 06:44:00 +0100
categories: [Fedora, Audio Production]
tags: [fedora, audio production, music production]
image: assets/img/pexels-pixabay-257904.jpg    
---


### Ardour
[Ardour](https://ardour.org/) is a multi-channel digital audio workstation (DAW), allowing users to record,
edit, mix and master audio and MIDI projects. It is targeted at audio engineers, musicians, soundtrack editors and composers.


![ardour](https://ardour.org/images/retina_no_plugs2.png){: .shadow }

```bash
sudo dnf ardour8
```
{: .nolineno }

### Audacity
[Audacity](https://www.audacityteam.org/) is the world’s most popular free software for recording and editing audio. 
It does destructive editing, not like most DAW's there is doing non-destructive editing.

![audacity](https://flathub.org/_next/image?url=https%3A%2F%2Fdl.flathub.org%2Fmedia%2Forg%2Faudacityteam%2FAudacity%2Fe3b7bcec1d992bcec6dfea86b70a5833%2Fscreenshots%2Fimage-1_orig.webp&w=3840&q=75)

`audacity` exist in the Fedora repositories, in a version with support for some file formats removed for patent reasons.\
`audacity-freeworld` exist in the rpmfusion repository, it contains support for mp3 & ffmpeg imports/exports missing in the fedora package.

I use the [flathub](https://flathub.org/apps/org.audacityteam.Audacity) version 

```bash
flatpak install org.audacityteam.Audacity --user
```
{: .nolineno }

### Calf
[Calf Studio Gear](https://calf-studio-gear.org/) is a number of instruments and effects there can be use standalone or with a DAW that support LV2 plugins. Very high quality with a great looking user interfaces.

![calf](https://calf-studio-gear.org/images/plugins/Calf%20-%20Monosynth%20-%20Audio%20Path.jpg){: .shadow }

```bash
sudo dnf install calf lv2-calf-plugins*
```
{: .nolineno }

### Linux Studio Plugins (LSP)
[Linux Studio Plugins](https://lsp-plug.in/) is a collection of audio effect plugins for linux, they are available as standalone and in a lot of different plugin formats like (lc2,vst3,clap etc)

![lsp](https://lsp-plug.in/img/plugins/filter_stereo.png){: .shadow }


**Standalone**
```bash
sudo dnf install lsp-plugins-jack
```
{: .nolineno }

**LV2**
```bash
sudo dnf install lsp-plugins-lv2
```
{: .nolineno }

**VST3**
```bash
sudo dnf install lsp-plugins-vst3
```
{: .nolineno }

**clap**
```bash
sudo dnf install lsp-plugins-clap
```
{: .nolineno }
