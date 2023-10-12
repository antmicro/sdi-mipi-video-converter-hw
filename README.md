# SDI-MIPI Video Converter

Copyright (c) 2022-2023 [Antmicro](https://www.antmicro.com)

[![image](https://img.shields.io/badge/View%20on-Antmicro%20Open%20Hardware%20Portal-332d37?style=flat-square)](https://openhardware.antmicro.com/boards/sdi-mipi-video-converter/?github=https%3A%2F%2Fgithub.com%2Fantmicro%2Fsdi-mipi-video-converter%2Ftree%2Fmain&tab=features)
![SDI-MIPI Video Converter](/img/sdi-mipi-video-converter.png)

## Overview

This repository contains open hardware design files for a video accessory based on the [Lattice CrossLink-NX](https://www.latticesemi.com/Products/FPGAandCPLD/CrossLink-NX) FPGA which allows to connect multiple video streams from SDI or CSI inputs, process it on-board and export with CSI output.

## Repository structure

The main repository directory contains KiCad PCB project files, a [LICENSE](LICENSE), and a README.
The remaining files are stored in the following directories:

* `lib` - contains the KiCad 6 component libraries,
* `img` - contains graphics for this README,

## Key Features

* LIFCL-40-9BG256C Lattice CrossLink-NX FPGA
* 3G SDI Input implemented with Semtech GS2971A deserializer 
* 3G SDI Loopback output implemented with Semtech GS2988 cable driver
* 3x4 CSI interfaces split 2/1 between two Antmicro 50-pin FFC connectors 
* 2Gbit (128Mx16) DDR3L DRAM

The board can be powered from either USB or Antmicro's 50-pin FFC connector.

Antmicro's 50-pin FFC connector is electrically compatible with several boards created by Antmicro, such as:
 
* [Jetson Nano/TX2 NX/Xavier NX Baseboard](https://github.com/antmicro/jetson-nano-baseboard)
* [OV9281 Dual Camera Board](https://github.com/antmicro/ov9281-camera-board)
* [HDMI-MIPI bridge](https://github.com/antmicro/hdmi-mipi-bridge)

## License

[Apache-2.0](LICENSE)
