---
layout: project
type: project
image: img/pyro/pyro_moves.gif
title: "\"πRo-Bot\" Autonomous Fire Suppression"
date: 2025
published: true
labels:
  - Robotics
  - Mechatronics
  - Automation
  - Event-Driven Programming
  - Embedded Systems
summary: "An autonomous 2DoF robot designed for fire suppression in hazardous environments, featuring both manual and automatic control."
---

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/final_design.png" alt="Our Final design plan, ready to print!" style="width: 60%;>
</div>

πRo-Bot is a prototype, semi-autonomous fire suppression system engineered for operation in hazardous or remote environments. It consists of a 2.5DoF robotic turret, capable of detecting flames and delivering retardant (water in our case). The system supports both autonomous and manual operation modes and is also capable of preemptively applying retardant to mitigate fire spread.

As the Mechanical Lead for the project, I was tasked with creating our custom-designed chassis and turret assembly, which I modeled in Fusion 360. I also selected much of hardware, including the transmission components and NEMA 17 stepper motors for precise directional control, while structural integrity has been rigorously validated using built-in finite element analysis (FEA). Our simulations confirmed that the design withstands operational loads with acceptable deflection and safety margins.

Motion control and fire detection are handled by an ESP32 microcontroller running an event-driven architecture. The turret integrates an IR camera module for thermal targeting, feeding data to the onboard system to autonomously track and suppress heat signatures. Below is our original concept sketch, which guided our mechanical layout and subsystem integration:

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/pyro_concept.jpg" alt="πRo-Bot Concept">
</div>

To simplify the overhead and reduce lead time, our team begun the design process by acquiring a commercial electric water gun and disassembling it. We cannibilized its parts to serve as our water delivery system.

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/water_gun.png" alt="The FunWee water gun. Fun to play with!">
</div>

Key goals include successful suppression of small fires at distances of up to 6 meters, full functionality in scanning, suppression, and manual modes, and a sleek, modular design adaptable for vehicles or buildings. After the first design iteration, my team has developed the following assembly:

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

After meeting with a panel of machinists, we were given some feedback and the green-light to manufacture our device. After some final design adjustments and structural validation (completed via Fusion 360’s FEA solver), we are currently proceeding to 3D printing of PLA components. At this point, we also recieved a Maker Grant from UC Berkeley's Chapter of the ASME. We've also begun implementing our code, which includes the IR Sensor mentioned previously.

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/fea.png" alt="Our armature passing FEA testing." style="width: 50%;">
</div>

<div class="text-center">
  <img class="img-fluid" src="../img/pyro/thermal.gif" alt="Thermal Camera initial testing." style="width: 50%;">
</div>
