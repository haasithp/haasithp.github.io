---
layout: page
title: Mathematical Modelling of Throwing a Rigid Body
description: "Independent Study formulating the rigid body dynamics and initial conditions for dynamic robotic throwing."
img: assets/img/thumb_throwing.png
importance: 4
category: robotics-dynamics
tags: [Dynamics, Simulation, Robotic-Manipulation, Mathematics, Physics]
keywords: Mathematical Modelling, Simulation, Rigid Body, Throwing Manipulation, Kinematics, Dynamics, Optimization, Independent Study
---

Traditional robotic manipulation heavily focuses on slow, "pick-and-place" grasping. Through an Independent Study, I explored the far more complex domain of **dynamic throwing manipulation**, requiring advanced mathematical modeling of rigid body dynamics in flight.

### Trajectory Optimization

Successfully directing an object through ballistic flight requires perfect initial release conditions:

- **Dynamic Formulation**: Modeled the complex equations of motion for an asymmetrical rigid body subjected to gravity and aerodynamic drag. This required calculating spatial inertia matrices and Coriolis forces to predict tumbling behaviors post-release.
- **Optimal Initial Conditions**: Implemented trajectory optimization algorithms to compute the precise release velocity, angle, and angular momentum required to hit a specific 3D coordinate target.
- **Simulation Validation**: The mathematical framework was heavily simulated to visualize the trajectory arcs, proving that the computed control parameters could effectively execute targeted throws—a foundational step toward advanced robotic end-effectors capable of dynamic object propulsion.

### Physical Experiments & Implementation

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/robot_throwing.png" title="Robotic Arm Throwing" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/drone_throwing.png" title="Drone Throwing" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/throwing_arm_gif.jpg" title="Robotic Arm Throwing Motion" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/throwing_drone_gif.jpg" title="Drone Throwing Motion" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Targeted throwing manipulation: into a 20cm x 20cm bin using an industrial robotic arm (left) and from an aerial drone hexacopter outdoors (right).
</div>