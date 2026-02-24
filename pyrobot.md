---
layout: default
---

# PyroBot Fire Suppression

Developed for local and autonomous firefighting in remote areas, PyroBot is an autonomous fire suppression system engineered for operation in hazardous or remote environments. It consists of a 2.5-DoF robotic turret, capable of detecting flames and autonomous delivery of fire retardant (water in our case).

**I owned all mechatronic systems on the robot, and worked closely with the electronics lead to create the low-level computer vision required for the autonomous operation.**

<video style="width: 100%; max-width: 640px;" controls>
    <source src="https://raw.githubusercontent.com/eyandocumet/eyandocumet.github.io/refs/heads/main/assets/pyrobot/pyro_demo.mp4" type="video/mp4">
</video>
<br>

## Outcomes
- Completion of a fully integrated, semi-autonomous fire suppression prototype with both manual and autonomous control modes.
- Successful thermal detection and event-driven suppression response tested under controlled conditions.
- Published a comprehensive [final report (PDF)](assets/pyrobot/PyroBot_Final_Report.pdf).

## Skills Demonstrated
- **Computer Aided Design (CAD).** Created stylish and functional 3D design using Autodesk Fusion. Integrated top-down and bottom-up assembly.
- **Mechanical Design for Manufacturing and Assembly (DFMA).** Integrated over 50 custom and COTS components with standard ASME hardware. Optimized design for manufacturing on an FDM 3D printer. Minimized part count. Use of standardized ASME fasteners.
- **Embedded Systems & Finite-State Machines.** Implemented event-driven architecture on an ESP32 microcontroller. Integrated sensor input and actuator control for autonomous operation.
- **Reverse Engineering.** Disassembled and integrated an off-the-shelf device and created a "virtual twin" in CAD. Designed new subsystems around existing components saving time and cost.

## Highlights

# General Strategy

Our robot obeyed the following high-level strategy:

1. Turret on passive patrol regimen, sweeping back and forth w/ IR camera
2. IR camera (attached to ESP32) detects large thermal signature and determines trajectory
3. Turrect actuates fire retardant measures until heat signature is below threshold.
4. Fire is extinguished, return to Step #1.

This was implemented in the following finite-state design:
![Finite State Machine](assets/pyrobot/state_transition_diagram.png)

# Autonomous Heat Tracking & Suppression

Running the entire system locally was important; our group did not want to do any processing outside of the microcontroller on-board since our system is intended to work in inaccessible enviornments. To achieve reliable targeting without high-level processing overhead, I co-developed a low-level Thermal CV pipeline. Using raw data from the thermal array, the system implements a "weighted center of mass" algorithm to localize heat signatures in real-time.

- **Centroid Localization:** The turret calculates the spatial average of all pixels exceeding a calibrated threshold (T>Tthreshold​), allowing it to naturally center the nozzle on the hottest point of a flame.

- **Suppression Logic:** To prevent false positives from ambient heat, the system requires a minimum temperature across the entire vision array

![Computer Vision](assets/pyrobot/thermal.gif)

## CAD & Layout Drawings

All components were engineered in Autodesk Fusion using a hybrid top-down assembly approach to ensure fit between the 3D-printed chassis and the reverse-engineered internal hardware. In this prototyping stage, manufacturing considerations were given to FDM 3D printing (e.g. no support material, mindfulness of print orientation)

![Platform Design](assets/pyrobot/platform_drawing.png)

![Base Design](assets/pyrobot/base_drawing.png)

![Arm Design](assets/pyrobot/arm_drawing.png)


