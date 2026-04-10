---
layout: page
title: Application of PID Control on a Bionic-Hand
description: "Multi-DOF hardware and Mujoco simulation applying PID loops to actuate a bionic hand."
img: assets/img/thumb_bionic_hand.png
importance: 3
category: robotics
tags: [Control-Systems, PID, Hardware, Mujoco, Simulation]
keywords: PID Control, Bionic Hand, Robotics, Mujoco Simulation, Kinematics, Control Theory, Actuation, Advances in Robotics and Control
---

Achieving smooth, lifelike motion in robotic prostheses demands precise regulation of motor torques and positions. For the *Advances in Robotics and Control* curriculum, I tackled the intricate control problem of actuating a multi-degree-of-freedom **Bionic Hand**.

### System Simulation and Tuning

The project required a deep understanding of classical control theory applied to non-linear physical systems:

- **Mujoco Physics Simulation**: Before touching hardware, I modeled the complex kinematics and contact dynamics of the hand joints within the **Mujoco** physics engine to ensure safe algorithmic development.
- **PID Loop Formulation**: Designed robust Proportional-Integral-Derivative (PID) controllers for individual finger actuators. The primary challenge was tuning the $K_p$, $K_i$, and $K_d$ gains to eliminate steady-state error while heavily dampening potential oscillations—crucial for delicate grasping maneuvers.
- **Hardware Deployment**: The tuned control algorithms were transitioned from simulated environments to a physical bionic prototype, demonstrating stable, responsive actuation that closely mirrored biological articulation under variable loads.

### System Visualization

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/bionic_hand_hardware.png" title="Bionic Hand Prototype" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/bionic_hand_mujoco.png" title="Mujoco Simulation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    PID control applied to a 3D-printed bionic hand prototype (left) and the underlying kinematic model simulated in Mujoco (right).
</div>