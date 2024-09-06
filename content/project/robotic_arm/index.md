---
title: Robotic Arm Arcade
date: 2023-11-26
external_link: 'ziyao/project/robotic_arm/'
reading_time: false  # Show estimated reading time?
share: false  # Show social sharing links?
profile: false  # Show author profile?
comments: true  # Show comments?
tags:
  - Duke
  - Robotics
  - Mechanical Engineering
---


To illustrate our knowledge of robot control and hardware design we learned this semester, our team has  engineered an  arcade game featuring an UR5e robotic arm.

![UR5e Robot arm and Me](//assets/media/icon.png "some img")
![alt txt](//assets/media/icon.png "some img")
UR5e Robot arm and Me

Important tasks involved in this project include:

- Design End Effector Rim and housing in SolidWorks
- Programming arduino system with LCD screen and sensor
- Motion planning of the UR5e Arm in Python ROS, MoveIt and Gazebo

All thanks to Duke MEMS department, We have the Universal UR5e with gripper/end effector Robotiq 2F-140 to play with.

To illustrate our knowledge of robot control and hardware design we learned this semester, our team has engineered an arcade game featuring an UR5e robotic arm. With UR5e robotic arm as its centerpiece, we integrate a designed 3D rim and an arduino system with an LCD screen and a sensor. The robot arm would dynamically move and present a challenge for players who aim to shoot ping-pong balls into a designated rim. Scores are displayed on an LCD screen, which is managed through an Arduino board connected to a sensor system.

![Robot arm with rim and arduino parts](https://prod-files-secure.s3.us-west-2.amazonaws.com/f182da4c-40b7-4bec-a266-0eff4ff79e72/a9e5f86b-02df-4718-83e1-37a0b1923b60/WhatsApp_Image_2023-11-20_at_11.10.02.jpeg)

## Design Specifics

**CAD Design**

![UR5e Robotic arm with gripper](https://prod-files-secure.s3.us-west-2.amazonaws.com/f182da4c-40b7-4bec-a266-0eff4ff79e72/86cd38db-8233-4341-b42b-50e70b90a0f9/IMG_4376_2.heic)

UR5e Robotic arm with gripper

![CAD model for rim and housing](https://prod-files-secure.s3.us-west-2.amazonaws.com/f182da4c-40b7-4bec-a266-0eff4ff79e72/0860bf4d-f893-4b73-8bac-e9e5d80eed6d/Screenshot_2023-12-05_at_14.05.44.png)

CAD model for rim and housing

We designed a model that attaches to the gripper of the UR5e robotic arm and provides housing for our Arduino system...

![Final System](https://prod-files-secure.s3.us-west-2.amazonaws.com/f182da4c-40b7-4bec-a266-0eff4ff79e72/9f8622f7-c496-4cfd-924e-bc49b02f2f14/IMG_4413.heic)

Final System

![Final Design](https://prod-files-secure.s3.us-west-2.amazonaws.com/f182da4c-40b7-4bec-a266-0eff4ff79e72/02ef53dc-1e5c-4bf5-b837-2453845f2dcb/IMG_4384.heic)

Final Design

**Arduino Logistics**

My work primarily involves implementing an Arduino system with our robotic arm alongside [Athre Hollakal](https://sites.google.com/view/athre-hollakal/about-me). We have successfully designed and implemented a system where the difficulty of the sensor changes every 20 seconds...

**Motion Planning and Testing**

Motion planning for moving the robotic arm was initially done in simulation using **Gazebo** and **Planit**...

## Our Team

![Team Photo](https://prod-files-secure.s3.us-west-2.amazonaws.com/f182da4c-40b7-4bec-a266-0eff4ff79e72/55d0465d-1500-4706-96c2-90f18f790bd5/1A9DB565-1B8E-4A39-96AB-C594A541E745_1_201_a.jpeg)
