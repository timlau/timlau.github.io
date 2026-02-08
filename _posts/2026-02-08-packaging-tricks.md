---
title: Packaging Tricks
date: 2026-02-06 11:00:00 +0100
categories: [Fedora, Packageing]
tags: [Fedora, Packaging, rpmbuild, CMake]     
image: assets/img/code01.jpg
---

## Introduction
This post is a collection of packaging tricks and tips that I have learned over the years of packaging software for Fedora, it is not a comprehensive guide to packaging, but rather a collection of tips and tricks that I have found useful in my packaging journey.

## rpmbuild
### Limmit the number of cores when building packages
When building a package, it is often useful to limit the number of cores used by the build process, on a system with limited resources, as it will leave some cores free for other processes.

This can be done by setting the `RPM_BUILD_NCPUS` environment variable before calling rpmbuild, for example:

```bash
RPM_BUILD_NCPUS=$(nproc --ignore=2) rpmbuild ...
```
{: .nolineno }

the `nproc --ignore=2` command will return the number of available cores minus 2,

What is happening is that rpmbuild wiil add the `-j` flag to the build command, which will limit the number of cores used by the build process to the value of `RPM_BUILD_NCPUS`.

### Control the build directory used by rpmbuild
By default, rpmbuild will use the `~/rpmbuild/BUILD` directory to build packages, but it is possible to change this by setting the `_topdir`  variable when calling rpmbuild, for example:

```bash
rpmbuild --define '_topdir $(pwd)/BUILD'
```
{: .nolineno }
This will make rpmbuild use the `BUILD` directory in the current working directory as the build directory instead of the default `~/rpmbuild/BUILD` directory.


## Cmake

### Using CMake presets to control the build process
CMake presets are a powerful way to control the build process of a CMake project, they allow you to define a set of build options and configurations that can be easily reused across different build environments. 

With CMake presets,your can control the generator used, the build type, the compiler flags, the binary directory and more.

The presets are defined in a `CMakePresets.json` or `CMakeUserPresets.json` file in the root of the project, and can be used to configure and build the project with a single command.

```bash
cmake --preset=debug
cmake --build --preset=debug
```
{: .nolineno }

For example, you can define a preset for building a package for debug or release.
```json
{
  "$schema": "https://cmake.org/cmake/help/latest/_downloads/3e2d73bff478d88a7de0de736ba5e361/schema.json",
  "version": 10,
  "cmakeMinimumRequired": {
    "major": 3,
    "minor": 31
  },
  "configurePresets": [
    {
      "name": "debug",
      "displayName": "Debug",
      "description": "Debug build using Ninja generator",
      "generator": "Ninja",
      "binaryDir": "build/debug",
      "cacheVariables": {
        "CMAKE_BUILD_TYPE": "Debug",
        "CPM_USE_LOCAL_PACKAGES": "ON",
        "CMAKE_CXX_FLAGS": "-flto=auto",
        "CMAKE_EXPORT_COMPILE_COMMANDS": "ON"
      }
    },
    {
      "name": "release",
      "displayName": "Release",
      "description": "Release build using Ninja generator",
      "generator": "Ninja",
      "binaryDir": "build/release",
      "cacheVariables": {
        "CMAKE_BUILD_TYPE": "Release",
        "CPM_USE_LOCAL_PACKAGES": "ON",
        "CMAKE_CXX_FLAGS": "-flto=auto",
        "CMAKE_EXPORT_COMPILE_COMMANDS": "ON"
      },
      "warnings": {
        "dev": false
      },
      "errors": {
        "dev": false
      }
    }
  ],
  "buildPresets": [
    {
      "name": "debug",
      "displayName": "App Debug Build",
      "configurePreset": "debug",
      "configuration": "Debug",
      "targets": ["LostAndFoundPiano_Standalone"]
    },

    {
      "name": "release",
      "displayName": "Release Build",
      "configurePreset": "release",
      "configuration": "Release",
      "targets": []
    }
  ]
}
```
{: .nolineno }

[Learn more about CMake presets](https://cmake.org/cmake/help/latest/manual/cmake-presets.7.html)
