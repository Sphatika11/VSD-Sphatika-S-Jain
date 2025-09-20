# VSD-Sphatika-S-Jain
# 🚀 RTL2GDS_Sphatika S Jain

Welcome to my journey through the SoC Tapeout Program VSD! This repository documents my week-by-week progress with tasks inside each week.

## VLSI System Design Program - Week 0 Tool Setup

![VLSI](https://img.shields.io/badge/-VLSI-blue) ![Tool Setup](https://img.shields.io/badge/-Tool_Setup-blue) ![RTL2GDS](https://img.shields.io/badge/-RTL2GDS-blue)

## Week 0: VLSI System Design Foundation & Tool Setup

Welcome to my VLSI System Design (VSD) Program repository! This week focused on setting up the development environment and installing the essential open-source tools that will be used throughout the program. The goal was to create a reliable and efficient workspace for synthesis, simulation, and design tasks. This guide provides step-by-step instructions to install Docker and OpenLane on an Ubuntu-based system running under WSL (Windows Subsystem for Linux).

## System and Virtual Machine Configuration

To ensure optimal performance, I configured a Virtual Machine (VM) with the following specifications:

| Specification         | Details          |
|-----------------------|------------------|
| Operating System 🐧   | Ubuntu 20.04+    |
| RAM 💾                | 6GB              |
| Storage 💿            | 50GB HDD         |
| vCPUs ⚡              | 4                |

> 💡 **Pro Tip:** This setup guarantees sufficient resources for handling toolchain demands and running simulations smoothly.

## Tool Installation & Verification

The following tools were installed for RTL synthesis, simulation, circuit analysis, and layout design.

### Yosys

**Purpose:** RTL Synthesis Tool - Converts RTL code into gate-level representations.

```bash
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make
sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
make
sudo make install
```

**Status:** ✅ Successfully Installed

### Iverilog

**Purpose:** Verilog Simulator - Compiles and simulates Verilog designs.

```bash
sudo apt-get install iverilog
```

**Status:** ✅ Successfully Installed

### GTKWave

**Purpose:** Waveform Viewer - Analyzes and visualizes simulation waveforms.

```bash
sudo apt update
sudo apt install gtkwave
```

**Status:** ✅ Successfully Installed

### Ngspice

**Purpose:** Circuit Simulator - Performs analog and mixed-signal simulation.

```bash
sudo apt update
sudo apt install ngspice
```

**Status:** ✅ Successfully Installed

### Magic VLSI

**Purpose:** Layout Tool - Creates, edits, and analyzes VLSI layouts.

```bash
sudo apt-get install m4 tcsh csh
sudo apt-get install libx11-dev tcl-dev tk-dev
sudo apt-get install libcairo2-dev
sudo apt-get install mesa-common-dev libglu1-mesa-dev
sudo apt-get install libncurses-dev
git clone https://github.com/RTimothyEdwards/magic
cd magic
./configure
make
sudo make install
```

**Status:** ✅ Successfully Installed

## Installation Summary

| Tool | Status | Primary Use |
|------|---------|-------------|
| 🧠 Yosys | ✅ Complete | RTL Synthesis |
| 📟 Iverilog | ✅ Complete | Verilog Simulation |
| 📊 GTKWave | ✅ Complete | Waveform Analysis |
| ⚡ Ngspice | ✅ Complete | Circuit Simulation |
| 🎨 Magic VLSI | ✅ Complete | Layout Design |

## Environment Ready for VLSI Design Journey!

All tools have been successfully installed and verified. The development environment is now ready for RTL to GDSII flow implementation.

## Author

**Sphatika S Jain**  
VLSI System Design Enthusiast

## Acknowledgements

I would like to express my sincere gratitude to **Kunal Ghosh** (Founder of VSD) for this incredible opportunity to learn and grow in the field of VLSI design. This program has provided me with the foundation and tools necessary to embark on my VLSI journey.

---

*This repository will be continuously updated with weekly progress and assignments throughout the VSD SoC Tapeout Program.*
