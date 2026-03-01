---
layout: page
title: Pose Graph Optimization and Trajectory Evaluation
description: "Mathematical backend optimization to correct trajectory drift for mobile navigating robots."
img: assets/img/thumb_mobile_robot.png
importance: 3
category: mobile-robotics
tags: [Mobile-Robotics, SLAM, Optimization, Trajectory, Mathematics]
keywords: Pose Graph Optimization, Trajectory Evaluation, Mobile Robotics, SLAM, Loop Closure, State Estimation, Robotics Course Project
---

A fundamental limitation in mobile robotic navigation (specifically odometry and SLAM systems) is the accumulation of measurement errors over time, leading to severe trajectory drift. To counteract this, my *Mobile Robotics* course project centered around the rigorous application of **Pose Graph Optimization**.

### Drift Correction Algorithms

The objective was to mathematically refine state estimates based on relative sensor measurements:

- **Graph Formulation**: Modeled the robot's state over time as a graph—where nodes represent the robot's 6D poses at different timestamps, and edges represent the constrained relative spatial transformations (odometry) between them.
- **Loop Closure Constraints**: Integrated loop closure detection. When the robot recognized a previously visited location, non-linear constraints were added to the graph, effectively "pinning" the map to a known environmental topology.
- **Non-Linear Least Squares**: Implemented optimization techniques (such as Gauss-Newton or Levenberg-Marquardt algorithms) to systematically distribute the accumulated error across all edges in the graph. This global relaxation process significantly smoothed and corrected the final trajectory evaluation, resulting in high-fidelity mapping.