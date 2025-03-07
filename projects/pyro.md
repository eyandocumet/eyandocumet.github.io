---
layout: project
type: project
image: img/pyro/pyro_square.png
title: "πRo-Bot Autonomous Fire Suppression"
date: 2025-03-07
published: true
labels:
  - Robotics
  - Automation
  - Fire Suppression
  - Embedded Systems
summary: "An autonomous 3DoF robot designed for fire suppression in hazardous environments, featuring both manual and automatic control."
---

<img class="img-fluid" src="../img/pyro/pyro_concept.jpg">

πRo-Bot is an autonomous fire suppression and prevention system, which functions via a 3DoF robotic turret designed to prevent and extinguish fires in hazardous or remote environments. The robot operates in both manual and automatic modes, using a robotic arm to accurately aim and deploy fire retardant at sources of fire. In addition, πRo has the capability to autonomously pre-apply retardant to an area, preventing fires before they spread. The chassis of the robot is modeled in Fusion360, with NEMA17 motors controlling the movement of the arm for precise targeting. The system is powered by an ESP32 board, which uses event-driven programming to control scanning motions, assisted by an IR camera mounted on the barrel for fire detection.

The project's goals include successfully suppressing small fires at a distance of up to 6 meters, implementing fully functional scanning, suppression, and manual control modes, and designing a sleek, robust, and modular robot that can be adapted for various settings, such as vehicles or buildings. The project is still ongoing, with further developments expected to enhance its capabilities.

After a first round of design iteration, my team has developed the following assembly:
<div class="row">
  <div class="col-md-6">
    <img class="img-fluid" src="../img/pyro/pyro1_iso.png" alt="Pyro ISO View">
  </div>
  <div class="col-md-6">
    <img class="img-fluid" src="../img/pyro/pyro1_top.png" alt="Pyro Top View">
  </div>
</div>

<div class="row">
  <div class="col-md-6">
    <img class="img-fluid" src="../img/pyro/pyro1_bottom.png" alt="Pyro Bottom View">
  </div>
  <div class="col-md-6">
    <img class="img-fluid" src="../img/pyro/pyro_firing_assembly.png" alt="Pyro Firing Assembly">
  </div>
</div>

Next steps involve 3D printing and initial assembly. We're intended un using 3D printed PLA plastic for our structual components.
