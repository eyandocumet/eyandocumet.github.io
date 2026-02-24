---
layout: default
---

# PyroBot Fire Suppression

Designed to minimize human risk in hazardous environments, PyroBot is a 2.5-DoF robotic turret that utilizes low-level computer vision to detect and extinguish thermal signatures.

**I owned the mechatronic design and co-developed the embedded vision pipeline for autonomous operation.**

<video style="width: 100%; max-width: 640px;" controls>
    <source src="https://raw.githubusercontent.com/eyandocumet/eyandocumet.github.io/refs/heads/main/assets/pyrobot/pyro_demo.mp4" type="video/mp4">
</video>
<br>

## Outcomes
- Delivered a fully functional system featuring Autonomous, Manual (RC), and Preventative spray modes.
- Integrated 50+ custom and COTS components using standardized ASME hardware and FDM-optimized geometries.
- Released a 15-page [Technical Report and Operations Manual (PDF)](assets/pyrobot/PyroBot_Final_Report.pdf) designed to allow re-production of our work.

## Skills Demonstrated
- **Computer Aided Design (CAD).** Created stylish and functional 3D design using Autodesk Fusion. Integrated top-down and bottom-up assembly.
- **Mechanical Design for Manufacturing and Assembly (DFMA).** Integrated over 50 custom and COTS components with standard ASME hardware. Optimized design for manufacturing on an FDM 3D printer. Minimized part count. Use of standardized ASME fasteners.
- **Embedded Systems & Finite-State Machines.** Implemented event-driven architecture on an ESP32 microcontroller. Integrated sensor input and actuator control for autonomous operation.
- **Reverse Engineering.** Disassembled and integrated an off-the-shelf device and created a "virtual twin" in CAD. Designed new subsystems around existing components saving time and cost.

## Control Logic and Strategy

The system architecture follows a prioritized control logic managed by an ESP32-based Finite State Machine (FSM). This allowed the robot to transition seamlessly between passive patrolling and active suppression. The three modes were: "automatic" (autonomous detection and extinguishing), "manual" (user controlled via a remote), and "preventative" (spraying in a prescribed pattern).

![Finite State Machine](assets/pyrobot/state_transition_diagram.png)

## Autonomous Heat Tracking & Suppression

To ensure reliability in remote areas, all processing is performed locally on the microcontroller. I co-developed a Low-Level Thermal CV pipeline to localize heat signatures without high-level external processing.

![Computer Vision](assets/pyrobot/thermal.gif)

## CAD & Layout Drawings

All components were engineered in Autodesk Fusion using a hybrid top-down assembly approach. Designs were specifically optimized for FDM 3D printing, minimizing support material and prioritizing print orientation for structural integrity.

![Platform Design](assets/pyrobot/platform_drawing.png)

![Base Design](assets/pyrobot/base_drawing.png)

![Arm Design](assets/pyrobot/arm_drawing.png)


