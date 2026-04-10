---
layout: page
title: Boston Dynamics Spot — Autonomous Navigation in Tunnels & Power Substations
description: LiDAR-inertial SLAM, ROS2 navigation stack, and custom controller for Spot in GPS-denied industrial environments
img: assets/img/thumb_mobile_robot.png
importance: 1
category: robotics
---

## Overview

Deployed a full autonomy stack on Boston Dynamics Spot for inspection in GPS-denied industrial environments — specifically underground tunnels and high-voltage power substations. These environments present two hard SLAM problems: geometric degeneracy in long featureless corridors, and IMU degradation from electromagnetic interference near high-voltage equipment.

## Demo

<div class="embed-responsive embed-responsive-16by9 mb-4" style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 8px;">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/XNpkjHjB2C4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
</div>

## Stack

- **SLAM:** FAST-LIO (LiDAR-inertial odometry) tuned for tunnel geometry and EMI-heavy environments
- **Navigation:** ROS2 navigation stack configured for legged locomotion on uneven industrial terrain
- **Control:** Designed and implemented an improved locomotion controller for Spot to handle substation and tunnel floor conditions
- **Platform:** Boston Dynamics Spot
- **Framework:** ROS2

## Key challenges solved

- Mitigated LiDAR degeneracy in long tunnel corridors through FAST-LIO parameter tuning and scan pre-processing
- Addressed IMU noise from high-voltage EMI at power substations for reliable state estimation
- Developed a custom controller improving Spot's traversability and stability on industrial terrain
- Integrated ROS2 navigation stack for autonomous waypoint following in GPS-denied environments

## Environments

Underground tunnels · High-voltage power substations
