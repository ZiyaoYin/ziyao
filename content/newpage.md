---
title: "UR5e Robot Arm Arcade"
date: 2024-10-09
author: "Ziyao Yin"
description: "Intro to Robotics project using the UR5e robotic arm."
---

# Duke University *2023-2024*

> I am a Master of Engineering student in Mechanical Engineering at Duke University focusing on Robotics.

---

## UR5e Robot Arm Arcade

**ME 555: Intro to Robotics**

Important tasks involved in this project include:

- Design End Effector Rim and housing in SolidWorks
- Programming Arduino system with LCD screen and sensor
- Motion planning of the UR5e Arm in Python ROS, MoveIt, and Gazebo

Thanks to Duke MEMS department, we have the Universal UR5e with a gripper/end effector Robotiq 2F-140 to use.

To illustrate our knowledge of robot control and hardware design learned this semester, our team engineered an arcade game featuring a UR5e robotic arm. With the UR5e robotic arm as its centerpiece, we integrated a 3D-designed rim and an Arduino system with an LCD screen and sensor. The robot arm dynamically moves and presents a challenge for players aiming to shoot ping-pong balls into a designated rim. Scores are displayed on an LCD screen, which is managed through an Arduino board connected to a sensor system.

---

## **Design Specifics**

### CAD Design

We designed a model that attaches to the gripper of the UR5e robotic arm and provides housing for our Arduino system. The rim and housing were created in SolidWorks and 3D printed using an Ultimaker S3 printer. The CAD design of the UR5e robotic arm end effector allowed for precise dimensions when designing the rim. For the housing, we had to measure the electronics to ensure a proper fit. Multiple versions were designed and refined through testing.

During the design process, we encountered issues fitting the electronic components into the housing. Adjustments had to be made to allow the wires to move freely. The final design allows for the breadboard to be taped to the surface, and the electronics to fit snugly inside the housing. To prevent components from falling off while the arm is in motion, screws can be inserted through the ends after attaching the rim to the end effector.

For future upgrades, we could consider adding a cover to protect the electronics from accidental contact with any balls during gameplay.

---

## **Arduino Logistics**

My work primarily involved implementing an Arduino system with our robotic arm alongside [Athre Hollakal](https://sites.google.com/view/athre-hollakal/about-me). We successfully designed and implemented a system where the sensor’s difficulty changes every 20 seconds. Additionally, the counter increments when motion is detected, indicating that the player has scored.

Before connecting everything, we first tested and implemented our entire code in simulation using TinkerCAD, simplifying testing and deployment.

Components used in the Arduino system:

- *1602 Serial LCD Module*: Responsible for showing the score and time countdown when the game starts.
- *HC-SR501 PIR Human Body Motion Sensor*: Detects and sends a signal to the controller when a score is made.
- *ELEGOO Arduino UNO R3 Board ATmega328P*: Updates the score and responds to the sensor.

---

## **Motion Planning and Testing**

Motion planning for moving the robotic arm was initially done in simulation using Gazebo and Planit, then tested on the physical system. **Robot Operating System (ROS 1)** was used for communication through subscriber and publisher nodes.

A Python script specified waypoints for the end effector to reach in Cartesian space. The path was calculated using MoveIt, with a specified resolution. The Python script sent movement commands to the arm in Gazebo. To run the physical system, a similar script was executed, sending commands directly to the arm through Linux.

---

## **Our Team**

- [Athre Hollakal](https://sites.google.com/view/athre-hollakal/about-me)
- Rory Pfister
- [Boyu Cao](https://1424681467.wixsite.com/website)
- [Ziyao Yin](https://ziyaoyin.github.io/ziyao/)
- Yujie Huang