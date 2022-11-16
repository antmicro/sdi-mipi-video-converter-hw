# Antmicro's open source CrossLink-NX Video Accessory

Copyright (c) 2022 [Antmicro](https://www.antmicro.com)

![Crosslink NX Video Accessory](/img/crosslink-nx-video-accessory.png)

## Overview

This repository contains open hardware design files for a video accessory using [Lattice Crosslink NX](https://www.latticesemi.com/Products/FPGAandCPLD/CrossLink-NX) FPGA.

This boards allows to connect multiple video streams from SDI or CSI inputs, process it on-board and export with CSI output.

## Repository structure

The main repository directory contains KiCad PCB project files, a [LICENSE](LICENSE), and a README.
The remaining files are stored in the following directories:

* `lib` - contains the KiCad 6 component libraries,
* `img` - contains graphics for this README,

## Key Features

* Crosslink NX FPGA
* SDI input with loopback output
* 3x4 CSI interfaces on two Antmicro's 50-pin FFC connectors 
* DDR3 memory module with x16 interface

The board can be powered from:

* USB connector
* Antmicro's 50-pin FFC connector

The Antmicro's 50-pin FFC connector is electrically compatible with several boards created by Antmicro, such as:
 
* [Jetson Nano Baseboard](https://github.com/antmicro/jetson-nano-baseboard)
* [OV9281 Dual Camera Board](https://github.com/antmicro/ov9281-camera-board)
* [HDMI-MIPI bridge](https://github.com/antmicro/hdmi-mipi-bridge)

## License

[Apache-2.0](LICENSE)
