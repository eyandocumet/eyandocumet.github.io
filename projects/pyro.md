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
  <img class="img-fluid" src="../img/pyro/final_design.png" alt="Our Final design plan, ready to print!" style="width: 30%;">
</div>

# Overview

πRo-Bot is a prototype, semi-autonomous fire suppression system engineered for operation in hazardous or remote environments. It consists of a 2.5DoF robotic turret, capable of detecting flames and delivering retardant (water in our case). The system supports both autonomous and manual operation modes and is also capable of preemptively applying retardant to mitigate fire spread.

# Skills Demonstrated
- **Computer Aided Design** – Parametric mechanical design using *Fusion 360*, including assemblies, joints, and toleranced components.  
- **Mechanical Design for Manufacturing (DFM)** – Use of standardized ASME fasteners, fits, and allowances tailored for 3D-printed components.  
- **Hardware Selection & Integration** – Specification of motors, transmission, and mechanical-electrical interfaces.  
- **Prototyping & Fabrication Planning** – Shop consultation, iterative design validation, and PLA-based 3D printing workflow execution.
- **Embedded Systems** - Implemented control architecture on an ESP32 microcontroller, integrating sensor input and actuator control for autonomous operation.
- **Event Driven Programming** – Developed non-blocking firmware to coordinate scanning, targeting, and suppression behaviors based on real-time IR sensor data.

# Mechanical Design

Fire response in hazardous or remote environments often places human lives at risk. My team sought to prototype an affordable, semi-autonomous robotic system capable of detecting and suppressing small fires in constrained or inaccessible locations. We aimed to combine embedded intelligence, precise mechanical control, and modular design into a compact solution suitable for further development in vehicular or building-based applications.

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/pyro_concept.jpg" alt="πRo-Bot Concept">
</div>

<div class="text-center">
  <div class="row">
    <div class="col-md-6">
      <img class="img-fluid" src="../img/pyro/fea.png" alt="Our armature passing FEA testing." style="width: 80%;">
    </div>
    <div class="col-md-6">
      <img class="img-fluid" src="../img/pyro/thermal.gif" alt="Thermal Camera initial testing." style="width: 80%;">
    </div>
  </div>
</div>

To reduce development time and simplify fabrication, I disassembled and cannibalized a toy electric water gun as our delivery mechanism. This allowed us to focus on system integration and targeting, rather than pump design. We presented our finalized design to a machinist review panel and received approval to proceed with fabrication. Following that, we secured a Maker Grant from the ASME UC Berkeley Chapter to fund manufacturing and testing.

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/water_gun.jpeg" alt="The FunWee water gun. Fun to play with!" style="width: 40%">
</div>

As Mechanical Lead, I was responsible for the structural architecture, manufacturability, and subsystem integration of πRo-Bot’s physical platform. I designed the custom chassis and turret assembly using *Fusion 360*, implementing a 2.5-degree-of-freedom motion system. Finite Element Analysis (FEA) was used to validate mechanical strength, confirm deflection limits, and ensure safe operation under expected loading conditions. I specified all hardware and transmission components, including NEMA 17 stepper motors and ASME-standard M3 fasteners (B18.3.4M bolts, B18.2.4.1M nuts, B18.22M washers). Design choices were guided by availability, ease of assembly, and tolerance control for 3D-printed PLA parts. The three main components I designed were the base, the armature, and the firing assembly.

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/platform_drawing.png" alt="Gun platform drawing" style="width: 40%">
</div>

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/arm_drawing.png" alt="Armature (wrist, waist) drawing" style="width: 40%">
</div>

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/base_drawing.png" alt="Base" style="width: 40%">
</div>

All critical mates in our design are metal-to-metal, utilizing off-the-shelf coupling flanges along with standardized washers, nuts, and bolts. We used ASME-standard fasteners, as they are readily available in bulk at our local hardware supplier, simplifying procurement. Specifically, we selected M3 ASME B18.22M washers, ASME B18.2.4.1M nuts, and ASME B18.3.4M bolts. Standardization reduced the need for custom tolerancing and mating analysis.

# Outcomes

At present, we are in the final manufacturing phase, fabricating and assembling components for full system integration. Our design has passed structural validation and subsystem testing, and we are on track to demonstrate the fully functional prototype at our capstone showcase later this month. Current outcomes include:
- Completion of a fully integrated, semi-autonomous fire suppression prototype with both manual and autonomous control modes.
- Verified mechanical performance under expected operational loads via FEA, with acceptable deflection and safety margins.
- Successful thermal detection and event-driven suppression response tested under controlled conditions.
- Streamlined mechanical-electrical integration, enabling efficient maintenance, modular upgrades, and clear subsystem interfacing.
