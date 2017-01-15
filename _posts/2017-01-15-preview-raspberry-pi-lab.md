---
layout: post
title: Preview - Raspberry Pi Lab
tags:
  - raspberrypi
  - aarch64
  - arm
  - bare-metal
---

To preview what to expect at this site - 

I'm preparing a guide for setting up a convenient "lab" for bare-metal
/ systems programming on a [Raspberry Pi
3](https://www.raspberrypi.org/products/raspberry-pi-3-model-b/). The
lab fits in a shoe-box with only one cord to it (for power) and can be
used from anywhere in the world. It cost about $170.00 USD new.

The setup has two Raspberry Pis, a "bare-metal" Pi that runs your
development code, and another that is a full Linux system accessible
over wifi. The two Pis are connected by both an ethernet cable (for
PXE booting the bare-metal Pi) and a serial cable (providing IO using
the simplest available device to program, UART).

The Raspberry Pi does not have a convenient remote reboot option. I
have the Linux Pi reboot the bare-metal Pi (and consequently load new
code by PXE) using a [WeMo
Switch](http://www.belkin.com/us/p/P-F7C027/).

The Linux Pi can be used to compile your bare-metal code, but doesn't
have to. The guide will provide instructions for setting up compiler
tool-chains for both aarch32 and aarch64 on the Linux Pi (Raspberry Pi
3 supports both architectures).
