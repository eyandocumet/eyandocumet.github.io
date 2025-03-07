---
layout: project
type: project
image: img/pyro/pyro_square.png
title: "πRo-Bot Autonomous Fire Suppression"
date: 2025
published: true
labels:
  - Robotics
  - Mechatronics
  - Automation
  - Event-Driven Programming
  - Embedded Systems
summary: "An autonomous 3DoF robot designed for fire suppression in hazardous environments, featuring both manual and automatic control."
---

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/pyro_concept.jpg" alt="πRo-Bot Concept">
</div>

πRo-Bot is an autonomous fire suppression system featuring a 3DoF robotic turret designed to prevent and extinguish fires in hazardous or remote environments. It operates in both manual and automatic modes, with its arm precisely aiming and deploying fire retardant at fire sources. Additionally, πRo-Bot can autonomously pre-apply retardant to areas, preventing fire spread.

The chassis is modeled in Fusion360, while NEMA17 motors handle the arm’s movement for accurate targeting. The system is powered by an ESP32, running event-driven code to control scanning motions, with an IR camera mounted on the turret for fire detection.

Key goals include successful suppression of small fires at distances of up to 6 meters, full functionality in scanning, suppression, and manual modes, and a sleek, modular design adaptable for vehicles or buildings. The project is ongoing, with further enhancements planned.

After the first design iteration, my team has developed the following assembly:
<div class="text-center">
  <div class="row">
    <div class="col-md-6">
      <img class="img-fluid" src="../img/pyro/pyro1_iso.png" alt="Pyro ISO View" style="width: 50%;">
    </div>
    <div class="col-md-6">
      <img class="img-fluid" src="../img/pyro/pyro1_top.png" alt="Pyro Top View" style="width: 50%;">
    </div>
  </div>
  
  <div class="row">
    <div class="col-md-6">
      <img class="img-fluid" src="../img/pyro/pyro1_bottom.png" alt="Pyro Bottom View" style="width: 50%;">
    </div>
    <div class="col-md-6">
      <img class="img-fluid" src="../img/pyro/pyro_firing_assembly.png" alt="Pyro Firing Assembly" style="width: 50%;">
    </div>
  </div>
</div>
Next steps involve 3D printing and initial assembly. We plan to use 3D-printed PLA plastic for structural components.
