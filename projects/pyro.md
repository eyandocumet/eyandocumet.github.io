---
layout: project
type: project
image: img/pyro/pyro_moves.gif
title: "\"πRo-Bot\" Autonomous Fire Suppression"
date: 2025
published: true
summary: "An autonomous 2DoF robot designed for fire suppression in hazardous environments, featuring both manual and automatic control."
---

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/Pyro_Final.png" alt="Gun platform drawing" style="height: 400px;">
</div>

# Overview

πRo-Bot is a prototype fire suppression system engineered for operation in hazardous or remote environments. It consists of a 2.5DoF robotic turret, capable of detecting flames and delivering retardant (water in our case). The system supports both autonomous and manual operation modes and is also capable of preemptively applying retardant to mitigate fire spread.

# Skills Demonstrated
- **Computer Aided Design** – Created maintainable parametric design using Fusion 360. Integrated top-down and bottom-up assembly.
- **Mechanical Design for Manufacturing (DFM)** – Optimized design for manufacturing on an FDM 3D printer. Minimized part count. Use of standardized ASME fasteners.
- **Embedded Systems** - Implemented even-driven architecture on an ESP32 microcontroller. Integrated sensor input and actuator control for autonomous operation.
- **Reverse Engineering** - Dissasembled an off-the-shelf device and created a "virtual twin" in CAD. Designed new subsystems around existing components.

# Mechanical Design
Fire response in hazardous or remote environments often places human lives at risk. My team sought to prototype an affordable, semi-autonomous robotic system capable of detecting and suppressing small fires in constrained or inaccessible locations. We aimed to combine embedded intelligence, precise mechanical control, and modular design into a compact solution suitable for further development in vehicular or building-based applications. 

As Mechanical Lead, I was responsible for the structural architecture, manufacturability, and subsystem integration of πRo-Bot’s physical platform. I designed the custom chassis and turret assembly using Fusion 360. Hand-calculations were used to confirm deflection limits, and ensure safe operation under expected loading conditions.

<div class="d-grid" style="grid-template-columns: 1fr 1fr; gap: 10px;">
  <div class="d-flex justify-content-center align-items-start">
    <img class="img-fluid" src="../img/pyro/final_design.png" alt="Final design plan" style="height: 200px; object-fit: contain;">
  </div>
  <div class="text-center">
    <img class="img-fluid" src="../img/pyro/platform_drawing.png" alt="Gun platform drawing" style="height: 200px;">
  </div>
  <div class="text-center">
    <img class="img-fluid" src="../img/pyro/arm_drawing.png" alt="Armature (wrist, waist) drawing" style="height: 200px;">
  </div>
  <div class="text-center">
    <img class="img-fluid" src="../img/pyro/base_drawing.png" alt="Base" style="height: 200px;">
  </div>
</div>



Several components required redesigns—namely, the gear linking the Pololu motor to the firing assembly, which underwent multiple iterations before settling on a shaft-collar mount and interference fit with the motor shaft.

# Outcomes

At present, we are in the final integration phase, finishing up our event-driven code and implementing our software goals. Our design has passed structural validation and subsystem testing, and we are on track to demonstrate the fully functional prototype at our capstone showcase later this month. Current outcomes include:

- Completion of a fully integrated, semi-autonomous fire suppression prototype with both manual and autonomous control modes.
- Verified mechanical performance under expected operational loads via hand-calculations, with acceptable deflection and safety margins.
- Successful thermal detection and event-driven suppression response tested under controlled conditions.
- Streamlined mechanical-electrical integration, enabling efficient maintenance, modular upgrades, and clear subsystem interfacing.
