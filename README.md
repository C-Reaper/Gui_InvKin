# Project README

## Overview
This project is an interactive simulation of Inverse Kinematics (IK) using a window-based engine. It demonstrates the use of mouse input to control the movement of an IK system.

## Features
- Interactive inverse kinematics simulation.
- Real-time rendering of the IK system based on mouse position.
- Supports different build targets for Linux, Windows, Wine, and WebAssembly.

## Project Structure

### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools
- Libraries needed in specific projects:
  - X11 for Linux GUI
  - WINAPI for Windows GUI
  - ALSA for audio input/output on Linux

## Build & Run

### Linux
To build and run the project on Linux:
```bash
cd <Project>
make -f Makefile.linux all
make -f Makefile.linux exe
```

### Windows
To build and run the project on Windows:
```bash
cd <Project>
make -f Makefile.windows all
make -f Makefile.windows exe
```

### Wine
To cross-compile for Windows using Wine on Linux:
```bash
cd <Project>
make -f Makefile.wine all
make -f Makefile.wine exe
```

### WebAssembly
To build and run the project as a web application:
```bash
cd <Project>
make -f Makefile.web all
make -f Makefile.web exe
```
This will generate an `index.html` file in the `build/` directory. Open this file in your browser to view the simulation.

For clean builds and debugging, use the provided targets such as `clean`, `debug`, etc., as described in the build steps section.