---
layout: page
title: Eye-in-Hand Visual Servoing for Dynamic Tracking
description: "Active visual servoing control loop using an XArm manipulator and an RGB-D camera."
img: assets/img/thumb_visual_servoing.png
importance: 2
category: robotics
tags: [Robotics, Visual-Servoing, ROS, RGB-D, Control-Theory]
keywords: Eye-in-Hand, Visual Servoing, Dynamic Tracking, OpenCV, ROS TF, ArUco markers, XArm manipulator, Control Loop, C++, Python
---

Dynamic target tracking requires an intricate balance between perception and mechanical control. In this project, I developed an **Eye-in-Hand visual servoing system**, utilizing an XArm robotic manipulator equipped with a wrist-mounted RGB-D camera to actively track and follow moving targets.

### Control and Perception Integration

This system closes the loop between what the robot "sees" and how its joints move in a highly dynamic environment:

- **Real-Time Pose Estimation**: Engineered a high-frequency perception pipeline utilizing **OpenCV** to detect ArUco markers within the camera's field of view. By computing the Perspective-n-Point (PnP) problem, the system rapidly estimates the 6D pose (translation and rotation) of the target.
- **Velocity Kinematics**: Leveraging the **ROS TF (Transform Library)**, the target's relative pose is transformed into the robot's base frame. I formulated an active control loop that computes the spatial velocity commands necessary to minimize the error between the current end-effector pose and the target marker.
- **Dynamic Responsiveness**: Programmed in a hybrid environment of **C++ and Python**, the control system calculates real-time joint velocity matrices. This allows the robotic arm to smoothly and dynamically adjust its trajectory on the fly, demonstrating robust tracking even when the target introduces unpredictable rapid movements.

This project sits at the intersection of modern Computer Vision and classical Control Theory, showcasing a highly responsive and autonomous robotic tracking node.
