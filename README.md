# RedPitaya Crosscompiler

This repository contains a sysroot for cross-compiling C/C++ applications targeting the RedPitaya board (ARM Cortex-A9).

## Features

- Includes necessary headers and shared libraries.
- Packaged as a `.deb` for easy installation under `/opt/redpitaya-sysroot`.
- Compatible with ARM toolchains like `arm-linux-gnueabihf-g++`.

## Download

You can download the latest `.deb` package from the [Releases page](https://github.com/aymanehajjaoui/redpitaya-crosscompiler/releases/latest).
Using wget command:
```bash
wget https://github.com/aymanehajjaoui/redpitaya-crosscompiler/releases/download/v1.0/redpitaya-sysroot.deb
```

## Installation

```bash
sudo dpkg -i redpitaya-sysroot.deb
```

## Usage

```bash
arm-linux-gnueabihf-gcc -o main main.c --sysroot=/opt/redpitaya-sysroot
```
