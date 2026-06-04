# LattePanda MU Custom Carrier Board

## High Speed PCB Design in KiCad

This repository contains a high-speed PCB design practice project created in KiCad
as part of the High Speed Design with KiCad course by D. Peter Dalmaris.

The primary goal of this project was to gain practical experience with modern
high-speed PCB layout techniques, signal integrity awareness, PCB stackup planning,
and manufacturability considerations.

# Project Background

The project workflow was inspired by the DFRobot LattePanda MU Carrier Board.

As part of the learning process:

- Existing PCB design constraints were studied
- PCB stackup parameters were imported into KiCad
- Routing practices from the reference design were analyzed
- High-speed layout techniques were explored through practical implementation
- Differential pair routing and length tuning techniques were practiced
- Teardrops were implemented throughout the PCB design process

PCIe functionality was not implemented, as the primary focus of the project
was PCB layout practice, signal routing exposure, and understanding high-speed
design workflows.

# 3D PCB Views

## Top Side
![PCB Overview](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/PCB_3D_MODEL_TOP.png)

## Bottom Side
![PCB Overview](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/PCB_3D_MODEL_BOTTOM.png)
## Overview

# Technologies & Concepts

 USB 3.0 high-speed routing
- HDMI interface routing
- Gigabit Ethernet routing
- M.2 connector integration
- Differential pair routing and length tuning
- Controlled impedance awareness
- PCB stackup planning
- Return path considerations
- Teardrop implementation
- DFM analysis using NextPCB HQDFM tools

## Design Goals

The project focused on learning and applying:

- High-speed routing practices
- Differential pair management
- Signal integrity fundamentals
- PCB stackup awareness
- Manufacturability considerations


# PCB Stackup & Impedance Planning

The PCB stackup and impedance calculations were reviewed using the NextPCB
impedance calculator and stackup tools.

## Impedance Calculator

![IMPEDANCE_CAL](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/PCB_Impedance_Calculator.png)

## NextPCB Stackup : Huaqiu04161H03-7628

![PCB_STACKUP](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/PCB_STACKUP.png)

## KiCad Stackup Configuration

![PCB_STACKUP](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/PCB_STACKUP_KICAD.png)

## PCB Layout


### Full PCB Overview

![PCB Layout](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/PCB_Layout.png)

# High-Speed Routing Examples

### USB 3.0 Routing

![USB3 Routing](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/USB3.0_Routing.png))

### Notes

- Differential pair routing applied to SuperSpeed signals
- Length tuning performed using KiCad tuning tools
- Pair spacing kept as consistent as possible
- Via transitions minimized where practical
- Teardrops applied throughout the routing process
- ESD protection placed close to connectors

### HDMI Routing

![HDMI Routing](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/HDMI_Routing.png))
### Notes

- TMDS differential pair routing implemented
- Length tuning and routing symmetry considered
- High-speed signal paths prioritized
- Teardrops used to improve routing transitions

### Gigabit Ethernet Routing

![Ethernet Routing](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/Images/Ethernet_Routing.png))
### Notes

- Differential pair routing used for Ethernet signals
- Return path continuity considered
- Routing isolation considered where possible
- Length matching practices applied where practical

# Schematics
Detailed Schematic of this project can be found within this repository.
[Schematic](https://github.com/tsokomalusi/LattePanda-MU-Custom-Carrier-Board/blob/main/LattePandaMU_Carrier_Custom_Board.pdf)

## DFM Review

The design was analyzed using the NextPCB DFM tool to identify:

- trace width violations
- spacing violations
- drill clearance concerns
- manufacturability issues

This exercise helped reinforce practical PCB manufacturing constraints and layout discipline.

## Lessons Learned

- High-speed routing requires careful planning before layout begins
- PCB stackup directly affects routing constraints and impedance behavior
- Differential pair routing introduces spacing and tuning challenges
- Length tuning requires balancing routing quality and board space
- Reference designs are valuable learning tools for understanding real-world layouts
- DFM analysis helps identify manufacturing issues early in the design process
- Teardrops improve routing robustness and manufacturability
- High-speed PCB design involves both electrical and mechanical tradeoffs

## TOOLCHAIN

- KiCad — schematic capture and PCB layout
- Git & GitHub — version control and project hosting
- NextPCB HQDFM — DFM analysis and manufacturability review
  
## Disclaimer

This project was created for educational and portfolio purposes.

The board has not been fabricated or electrically validated.
PCIe - not implemented to reduce complexity at this stage, but can be future enhancement for V2.0 hopefully.

The DFM analysis is still work in progress.
