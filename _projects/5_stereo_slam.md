---
layout: page
title: Stereo SLAM System Development
description: "Robust 1D and 2D SLAM pipeline utilizing C++, OpenCV, and Pose-Graph Optimization."
img: assets/img/thumb_slam.png
importance: 2
category: computer-vision
tags: [SLAM, C++, OpenCV, Robotics, 3D-Reconstruction]
keywords: SLAM, Simultaneous Localization and Mapping, OpenCV, Pose-Graph Optimization, Bundle Adjustment, Perspective-n-Point, C++, Computer Vision
---

Building a reliable Simultaneous Localization and Mapping (SLAM) system is one of the foundational challenges in modern robotics. For this project, I engineered a robust 1D and 2D SLAM pipeline from scratch, leveraging the power of **C++** and **OpenCV**.

### Core Technical Implementation

The system architecture focuses on high-accuracy trajectory estimation and environmental reconstruction:

- **Mathematical Foundations**: Implemented Stereo Reconstruction and Perspective-n-Point (PnP) algebraic solvers to translate 2D camera feeds into mathematically rigorous 3D spatial points. 
- **Bundle Adjustment**: Integrated local and global Bundle Adjustment techniques to jointly refine the 3D coordinates describing the scene geometry and the parameters of the relative motion, significantly reducing reprojection errors.
- **Pose-Graph Optimization**: A major hurdle in SLAM is accumulated drift over long operational distances. I applied advanced Pose-Graph Optimization algorithms to detect loop closures and correct trajectory drift. This drastically enhanced the global localization accuracy of the mapping process.

By bridging theoretical mathematical models with highly optimized C++ code, this project successfully demonstrates a low-latency, highly accurate tracking and mapping solution suitable for real-time robotic navigation.
