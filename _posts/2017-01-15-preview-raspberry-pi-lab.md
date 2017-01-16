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
3](https://www.raspberrypi.org/products/raspberry-pi-3-model-b/)
[(amazon)](https://www.amazon.com/gp/product/B01CD5VC92/ref=as_li_tl?ie=UTF8&tag=esstone-20&camp=1789&creative=9325&linkCode=as2&creativeASIN=B01CD5VC92&linkId=359fc9438a52c607ffd1dc16e3d02e58).
The lab fits in a shoe-box with only one cord to it (for power) and
can be used from anywhere in the world. It cost about $170.00 USD new.

The setup has two Raspberry Pis, a "bare-metal" Pi that runs your
development code, and another that is a full Linux system accessible
over wifi. The two Pis are connected by both an ethernet cable (for
PXE booting the bare-metal Pi) and a serial cable (providing IO using
the simplest available device to program, UART).

The Raspberry Pi does not have a convenient remote reboot option. I
have the Linux Pi reboot the bare-metal Pi (and consequently load new
code by PXE) using a [WeMo
Switch](http://www.belkin.com/us/p/P-F7C027/)
[(amazon)](https://www.amazon.com/gp/product/B00BB2MMNE/ref=as_li_tl?ie=UTF8&tag=esstone-20&camp=1789&creative=9325&linkCode=as2&creativeASIN=B00BB2MMNE&linkId=63c8c3b32ec08706128f4c88ff19a05f).

The Linux Pi can be used to compile your bare-metal code, but doesn't
have to. The guide will provide instructions for setting up compiler
tool-chains for both aarch32 and aarch64 on the Linux Pi (Raspberry Pi
3 supports both architectures).
