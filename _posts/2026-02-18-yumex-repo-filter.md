---
title: Yum Extender - Repository filtering
date: 2026-02-18 15:30:00 +0100
categories: [Yum Extender, New Features]
tags: [Fedora, Feature, yumex, Codeing]
image: assets/img/yumex-repo-filter.png
---


## Description
I have added a new feature to Yum Extender that allows users to filter search results byrepository keywords. This feature is particularly useful for users who want to install packages from specific repositories.

**This video demonstrates how to use the repository filtering feature in Yum Extender.**
{%
  include embed/video.html
  src='assets/video/yumex_repo_filtering.webm'
  types='webm'
  poster='assets/img/yumex-repo-filter.png'
  title='Yum Extender Repository Filtering'
  autoplay=false
  loop=true
  muted=true
%}

## Installation
The feature is available in the latest development version of Yum Extender available in the [yumex-ng-dev ](https://copr.fedorainfracloud.org/coprs/timlau/yumex-ng-dev/) COPR Repository

To install it, run the following commands:

```terminal
sudo dnf copr enable timlau/yumex-ng-dev
sudo dnf install yumex
```
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/P5P81FOLMO)
