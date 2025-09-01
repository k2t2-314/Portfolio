---
title: Iris Tang – Mechanical Engineering Portfolio
layout: default
---

# 👋 Hi, I'm Iris Tang

I’m a Mechanical Engineering master’s student at Carnegie Mellon University with a strong foundation in robotics, intelligent systems, and mechatronic design. I specialize in building full-stack engineering solutions — from CAD design and structural simulation to embedded control and AI integration.

This portfolio showcases selected projects that highlight my technical capabilities, research experience, and passion for solving real-world problems through innovative mechanical systems. Projects range from collaborative robotic arms and self-leveling tripods to wave-dampening devices and vision-driven manipulators, many of which have been prototyped, published, or patented.

> Feel free to explore the projects below
> 
> For more, check out my [GitHub](https://github.com/k2t2-314) or [LinkedIn](https://www.linkedin.com/in/xinxuantang)).

# Thesis & Research Projects

This section highlights my academic research and thesis-related work, focusing on interdisciplinary mechanical systems that integrate structural design, control algorithms, and intelligent sensing. Many of these projects were conducted under faculty supervision or as part of research labs, and involve hands-on prototyping, simulations, and early-stage AI applications. The work reflects both deep technical investigation and practical engineering execution.

## Hand Exoskeleton

**Institution:** Carnegie Mellon University  
**Role:** Research Assistant (Sep 2024 – Present)  
**Tools:** SolidWorks · EMG Sensors · OpenCV · Arduino · Python (Supervised Learning Models)

#### Overview
This research project aims to develop an intelligent hand exoskeleton system for spinal cord injury (SCI) patients, enabling motion assistance and rehabilitation through sensor-driven control. The device is designed to actuate not only individual fingers but also the wrist, supporting full-hand movement. Surface EMG sensors placed on the forearm detect muscle activity, while a vision-based system tracks real hand motion to provide training data.

![Model Image](/assets/img/Exo.png)

#### My Contributions
As a core member of the team, I was responsible for:
- Designing and prototyping the finger actuation system using compact motors and custom joint geometry, optimized for natural range of motion (–30° to +80°)
- Implementing a computer vision pipeline to track fingertip trajectories using 2D video data
- Developing supervised learning models (classification and regression) to predict intended motion from EMG and visual inputs
- Preparing the pipeline for eventual real-time control integration
Other team members supported motor smoothing algorithms, mechanical integration for the wrist module, and hardware testing on volunteers.

#### Outcome
The prototype demonstrated ergonomic compliance and mechanical reliability during user testing on both healthy individuals and one SCI patient. Initial model training showed promising performance in motion intention prediction, establishing a foundation for adaptive, sensor-driven control in future iterations.

![Prototype Image](/assets/img/outcomeExo.png)

## Offshore Curtain Array for Wave Dissipation

**Institution:** Shanghai Jiao Tong University  
**Role:** Student (Feb 2023 – Feb 2024)  
**Tools & Methods:** SolidWorks · FEA · Raspberry Pi · Python (Tkinter GUI) · Water Tank Testing

#### Overview

 - Designed and prototyped a 5 m modular inflatable curtain segment with foldable, interlocking structure, capable of deploying over 2.5 m below deckline for wave interception, offering roll-up storage and superior portability over traditional water bags.
 - Developed an integrated control system combining Raspberry Pi–based logic, embedded actuation, and IR remote interface, supporting real-time adaptive wave response and autonomous deployment.
 - Validated system via prototype fabrication and controlled wave tank testing, achieving ~70% wave height reduction and ~85% energy attenuation.

#### Outcome
The system achieved ~70% wave height reduction and ~85% energy attenuation in field tests. The modular design enables rapid deployment, convenient transport, and easy depth customization — making it suitable for offshore platforms, environmental buoys, or underwater operations requiring a calm local water surface.

# Industry Collaboration Project

## Automated Lubricator Lifting & Handling Device
**Institution:** Shanghai Jiao Tong University × Well Master Corporation  
**Role:** Capstone Lead Engineer (Dec 2024 – Jun 2025)  
**Tools & Methods:** SolidWorks · ANSYS FEA · YOLOv11 · Arduino · OpenCM · Multi-DOF Actuation · Parametric Optimization (MOGA)

#### Overview
This industry-sponsored capstone project aimed to develop an intelligent, semi-autonomous system to handle large lubricators used in industrial pipelines. The system was designed to automate the process of lifting, flipping, inspecting, and repositioning multi-model lubricators safely and efficiently using computer vision and coordinated multi-axis actuation.

 - Architected a lightweight, 5-DOF gantry system to support high-load (200 lb) lubricator handling with ±1.5 mm precision; enabled multi-DOF flipping and placement through a modular, extensible actuation framework.
 - Built and validated a 1:2 functional prototype integrating adaptive gripping, flipping, and inspection, automating full operation cycles within 90 seconds—over 3× faster than manual workflows.
 - Implemented a YOLOv11-driven perception module for model identification and vision-guided manipulation, enabling accurate autonomous recognition and handling of 8+ distinct lubricator types.
 - Led simulation-driven structural optimization using MOGA and response surface methods, reducing mass by 6.71% while increasing first-order natural frequency by 15.61%, significantly improving stiffness-to-weight ratio and dynamic safety.
   
#### Outcome
The system achieved stable and efficient handling of multiple lubricator types, with precise motion control and consistent flipping accuracy. It was presented at SJTU’s online exhibition, earning recognition for best project demonstration. This work laid the foundation for potential industrial deployment and IP filing.

# Course Projects

## Simulated Jumping Bionic Frog
**Tools & Methods:** SolidWorks · Incomplete Gear Design · Arduino · MATLAB Simscape  
**Position:** Mechanical Design & Simulation  
**Description:**  
Developed a bionic robot that mimics frog-like jumping using spring-based elastic energy storage and an incomplete gear mechanism. Designed a one-DOF leg linkage and performed dynamic simulation to optimize jumping stability. The system was compact, energy-efficient, and featured rollover-preventing geometry. The prototype, powered by MG996R servos, consistently achieved 20 cm horizontal jumps on flat ground.

## Automatic Pot-Forming & Seed-Planting System  
**Tools & Methods:** SolidWorks · QFD · Manual Prototyping · Animation  
**Position:** Problem Definition, Structural Design, Visualization  
**Description:**  
Created an integrated device for pot formation and seed dispensing aimed at efficient small-scale farming. Designed a rotating seed wheel with volume-controlled grooves and a spring-based pedal system to extrude nutrient pots. Employed QFD for functional analysis and contributed to physical prototyping and visual animation. The system reduced manual effort and improved planting precision.

## Light-Tracking Turret Using Photoresistors  
**Tools & Methods:** Arduino · LDR Sensors · Servo Control · Analog Circuit (TDA2882)  
**Position:** System Architecture & Control Logic  
**Description:**  
Designed a servo-controlled turret that continuously tracks a moving light source using differential voltage from four LDR sensors. Implemented a simple analog-to-digital system that translated light intensity differences into horizontal and vertical servo adjustments. Inspired by robotic docking systems, the turret performed accurate spherical tracking and showed strong potential for low-cost solar alignment systems.

## Collaborative Robotic Arm Design  
**Tools & Methods:** SolidWorks · MATLAB · Simscape · Kinematics & Dynamics Modeling  
**Position:** Modeling & Simulation Engineer  
**Description:**  
Designed a lightweight, collaborative robotic arm inspired by the JAKA Zu5 structure. Focused on internal wiring, joint design, and reducer/motor selection based on static torque estimates. Modeled kinematics and dynamics using Simscape and performed multi-pose trajectory planning. Simulated advanced tasks such as ball juggling to verify dexterity and precision.

## Self-Leveling Tripod (Patent Pending)  
**Tools & Methods:** SolidWorks · ANSYS · Arduino · IMU · 3D Printing · CNC  
**Position:** Mechanical Designer & Control System Developer  
**Description:**  
Engineered a self-leveling tripod to assist users with wrist pain, using an IMU to detect tilt and servos to auto-correct orientation. Designed a compact structural form and verified strength through FEA. Built the prototype using PLA 3D printing and CNC-machined aluminum plates. The tripod auto-leveled successfully on startup and met ergonomic expectations, with a patent application submitted.

## Model-Based Control System for Magnetic Whiteboard Cleaning Robot  
**Tools & Methods:** Python · TVLQR · Model Predictive Control · EKF · IMU · AprilTag · Simulation  
**Position:** Mechatronics Engineer  
**Description:**  
Designed and implemented a hybrid control framework integrating Time-Varying LQR (TVLQR) and Model Predictive Control (MPC) to enable responsive and stable trajectory tracking for an indoor magnetic robot. Simulated full-system dynamics with sensor fusion via Extended Kalman Filter (EKF), combining IMU and vision input for real-time state estimation. Integrated control logic with AprilTag-based localization and custom user-defined path interfaces to enable autonomous shape-following and area coverage. Optimized controller robustness under ~2 Hz Bluetooth constraints, demonstrating stability in low-bandwidth, noisy environments.

# Self Interests

### 2D Python Shooting Game  
**Tools & Methods:** Python · UI/UX Design · Multi-File Architecture  
**Position:** Full-Stack Developer & Designer  
**Description:**  
Built a 2D underground-themed shooting game with custom character selection, level design, and power-up mechanics using CMU_Graphics. Designed modular animation and game logic through multi-file architecture. Implemented a real-time user interface with dynamic map switching and gravity effects. The final demo included a promotional video and gameplay preview.
