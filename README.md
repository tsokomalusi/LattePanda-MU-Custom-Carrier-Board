# High Speed PCB Design in KiCad

## Top Side
![PCB Overview](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/PCB_3D_MODEL_TOP.png)

## Bottom Side
![PCB Overview](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/PCB_3D_MODEL_BOTTOM.png)
## Overview

This repository contains a high-speed PCB design practice project created in KiCad
as part of the High Speed Design with KiCad course by D. Peter Dalmaris.

The goal of this project was to gain practical experience with modern high-speed
PCB layout techniques and signal integrity concepts.

## Technologies & Concepts

- USB 3.0 differential pair routing
- HDMI routing and skew tuning
- Gigabit Ethernet routing
- Differential pair length matching
- Controlled impedance awareness
- Return path considerations
- DFM analysis using NextPCB tools

## Design Goals

The project focused on learning and applying:

- High-speed routing practices
- Differential pair management
- Signal integrity fundamentals
- PCB stackup awareness
- Manufacturability considerations

## PCB Layout


### Full PCB Overview

![PCB Layout](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/PCB_Layout.png)

### USB 3.0 Routing

![USB3 Routing](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/USB3.0_Routing.png))

### HDMI Routing

![HDMI Routing](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/HDMI_Routing.png))

### Gigabit Ethernet Routing

![Ethernet Routing](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/Ethernet_Routing.png))

### Differential Pair Tuning

![Differential Pair Routing](docs/screenshots/differential-pairs.png)

### Length Matching

![Length Matching](docs/screenshots/length-matching.png)

## Design Notes

### USB 3.0
- Differential impedance target considered during routing
- Pair spacing maintained consistently
- Length matching applied to SuperSpeed pairs
- Minimal via transitions used

### HDMI
- Differential pair skew minimized
- Length tuning performed using KiCad tools
- Routing symmetry prioritized

### Gigabit Ethernet
- Pair matching applied
- Clean return paths considered
- Routing isolated from noisy regions where possible

## DFM Review

The design was analyzed using the NextPCB DFM tool to identify:

- trace width violations
- spacing violations
- drill clearance concerns
- manufacturability issues

This exercise helped reinforce practical PCB manufacturing constraints and layout discipline.

## Lessons Learned

- High-speed routing requires planning before placement
- Return paths strongly affect signal integrity
- Differential pair tuning introduces routing tradeoffs
- Layer stackup decisions affect impedance behavior
- DFM analysis helps bridge design and manufacturing

## TOOLCHAIN

- Git/Github: VCS and profile
- KICAD: Schematic Capture
- HQDFM - DFM Analysis
  
## Disclaimer

This project was created for educational and portfolio purposes.

The board has not been fabricated or electrically validated.

The DFM analysis is still work in progress.
