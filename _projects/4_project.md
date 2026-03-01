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