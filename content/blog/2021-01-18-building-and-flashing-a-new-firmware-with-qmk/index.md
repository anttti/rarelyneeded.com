---
title: "Building And Flashing A New Firmware With QMK"
date: "2021-01-18"
tags:
  - "keyboards"
---

After just setting up a QMK environment and creating and flashing a firmware for my Hotdox keyboard, I decided to write the steps down because I will inevitably forget something the next time I need to change something.

## Installing the tools on macOS

[The official docs](https://docs.qmk.fm/#/newbs_getting_started) are good, but the current Brew version of `avr-gcc` is broken and needs to be manually built from source after setting up QMK:

```
brew uninstall --ignore-dependencies avr-gcc@8
brew install --build-from-source avr-gcc@8
```

## Creating a new layout

```
qmk new-keymap -kb hotdox
```

## Building the firmware

```
qmk compile -kb hotdox -km anttti
```

## Flashing the firmware

Once the keyboard is built, the `.hex` file is found in `~/qmk_firmware/.build` and it can be flashed with QMK Toolbox.
