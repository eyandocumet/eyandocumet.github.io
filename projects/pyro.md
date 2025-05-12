---
layout: project
type: project
image: img/pyro/pyro_moves.gif
title: "\"πRo-Bot\" Autonomous Fire Suppression"
date: 2025
published: true
summary: "An autonomous 2DoF robot designed for fire suppression in hazardous environments, featuring both manual and automatic control."
---

<div align="center">
  <img src="../img/pyro/hero_shot.jpg" width="400" alt="Hero Shot">
</div>

## Overview

πRo-Bot is a prototype fire suppression system engineered for operation in hazardous or remote environments. It consists of a 2.5DoF robotic turret, capable of detecting flames and delivering retardant (water in our case). The system supports both autonomous and manual operation modes and is also capable of preemptively applying retardant to mitigate fire spread.

<div align="center">
  <video src="../img/pyro/pyro_demo.mp4" width="640" height="360" controls></video>
</div>

## Skills Demonstrated
- **Computer Aided Design** – Created maintainable parametric design using Fusion 360. Integrated top-down and bottom-up assembly.
- **Mechanical Design for Manufacturing (DFM)** – Optimized design for manufacturing on an FDM 3D printer. Minimized part count. Use of standardized ASME fasteners.
- **Embedded Systems** - Implemented event-driven architecture on an ESP32 microcontroller. Integrated sensor input and actuator control for autonomous operation.
- **Reverse Engineering** - Dissasembled an off-the-shelf device and created a "virtual twin" in CAD. Designed new subsystems around existing components.

## Mechanical Design
Fire response in hazardous or remote environments often places human lives at risk. My team sought to prototype an affordable, semi-autonomous robotic system capable of detecting and suppressing small fires in constrained or inaccessible locations.

As Mechanical Lead, I was responsible for the structural architecture, manufacturability, and subsystem integration of πRo-Bot’s physical platform. I designed the custom chassis and turret assembly using Fusion 360. Hand-calculations were used to confirm deflection limits, and ensure safe operation under expected loading conditions.

<div class="d-grid" style="grid-template-columns: 1fr 1fr; gap: 10px;">
  <div class="d-flex justify-content-center align-items-start">
    <img class="img-fluid" src="../img/pyro/final_design.png" alt="Final design plan" style="max-height: 300px; width: auto;">
  </div>
  <div class="text-center">
    <img class="img-fluid" src="../img/pyro/platform_drawing.png" alt="Gun platform drawing" style="max-height: 300px; width: auto;">
  </div>
  <div class="text-center">
    <img class="img-fluid" src="../img/pyro/arm_drawing.png" alt="Armature (wrist, waist) drawing" style="max-height: 300px; width: auto;">
  </div>
  <div class="text-center">
    <img class="img-fluid" src="../img/pyro/base_drawing.png" alt="Base" style="max-height: 300px; width: auto;">
  </div>
</div>

Several components required iterative redesign—most notably, the gear coupling our Pololu motor to the rack gear on the firing assembly, which was optimized through successive prototypes before converging on a shaft-collar mounting scheme and interference fit for secure power transmission.

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/gear_evolution.jpeg" alt="Gun platform drawing" style="height: 400px;">
</div>

## Outcomes
- Completion of a fully integrated, semi-autonomous fire suppression prototype with both manual and autonomous control modes.
- Successful thermal detection and event-driven suppression response tested under controlled conditions.
- Streamlined mechanical-electrical integration, enabling efficient maintenance, modular upgrades, and clear subsystem interfacing.
- Successful demo at semi-annual Jacobs Hall design showcase.
- Comprehensive reporting. [Available online](https://eyandocumet.xyz/img/pyro/ME102B_Final_Report_Group8.pdf).

\* *Special thanks to teammate Menooa Avrand for the creation of the demonstration video.*
