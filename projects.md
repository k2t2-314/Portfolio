---
layout: default
title: Projects
permalink: /projects.html
---

<div style="margin-bottom: 30px;">
  <a href="{{ '/' | relative_url }}">🏠 Home</a> |
  <a href="{{ '/projects.html' | relative_url }}">🛠 Projects</a> |
  <a href="{{ '/contact.html' | relative_url }}">📬 Contact</a>
</div>

# Projects
---

## Flexible Lubricator Handling & Inspection Platform
**Industry Collaboration: Well Master Corporation & SJTU**  
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Computer Vision</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Robotics Control</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Mechanical Design</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">CAE/FEA</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">SolidWorks</span>
**Role:** Lead Mechanical Designer    
**Summary:** Developed a production-ready, 5-DOF gantry system that automates the extraction, reorientation, and visual inspection of 200-lb industrial lubricators, increasing throughput by 40%.

<details markdown="1">
  <summary><strong>View Project Details</strong></summary>
  
1\. Designed a modular 5-DOF cantilever gantry and a torque-matched flipping platform using aluminum profiles and custom brackets. Conducted **ANSYS static** and **modal simulations** to validate structural integrity, successfully limiting maximum deflection to <0.7 mm and ensuring a modal frequency >25 Hz to eliminate operational resonance.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 2; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/1-1.png' | relative_url }}" 
         alt="Full CAD assembly" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Full CAD assembly of 5‑DOF gantry</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/1-2.png' | relative_url }}" 
         alt="parameter optimization in ANSYS" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>ANSYS Optimization</strong>
    </figcaption>
  </figure>

</div>

2\. Implemented multi-actuator coordination utilizing **Fuzzy PID** for Z-axis soft-landing and coupled PID for synchronized 5-axis gantry motion. Integrated real-time safety interlocks via torque sensing and IMU-based alignment, achieving flipping stability with <3° overshoot and a settling time of <2.5 s.

<figure style="margin: 1.5rem auto; text-align: center; max-width: 85%;">
  <img src="{{ '/assets/img/1-4.png' | relative_url }}" 
       alt="Full CAD assembly" 
       style="width: 100%; height: auto; border-radius: 12px; border: 1px solid #eee; box-shadow: 0 4px 6px -1px rgba(0,0,0,0.1);">
  <figcaption style="margin-top: 0.8rem; font-size: 0.85rem; color: #555;">
    <strong>Control System Architecture & Simulation via Simulink</strong>
  </figcaption>
</figure>

3\. Engineered a real-time perception system by deploying a **YOLOv11 model**, utilizing a **Sim-to-Real data strategy** (3D synthetic models + real-world photography). Achieved **92% mAP** for multi-class industrial part detection and 25 FPS inference speed, enabling fully automated pass/fail inspection logic.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 1.2; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/1-6.png' | relative_url }}" 
         alt="YOLOv11 Training Metrics" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>YOLOv11 Training Metrics & mAP Curve</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/1-7.png' | relative_url }}" 
         alt="Real-time Inference and Localization" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Real-time Detection & Localization</strong>
    </figcaption>
  </figure>

</div>

</details>


---

## Actuation Module for Hand Exoskeleton   
**Research Project: Carnegie Mellon University (CMU) | NeuroMechatronics Lab**  
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Biosignal Processing</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Machine Learning</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Soft Robotics</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Embedded Systems</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">3D Printing</span>  
**Role:** Graduate Research Assistant  
**Summary:** Designed a wearable actuation module for hand exoskeletons featuring an integrated sEMG decoder. The system assists SCI patients in daily tasks via finger actuation while utilizing the wrist module for high-fidelity signal processing and intention decoding to close the loop for rehabilitation.

<details markdown="1">
  <summary><strong>View Project Details</strong></summary>

1\. Developed a low-profile, wearable finger linkage featuring iterative CAD packaging for cable routing and palm-mounted motor housing. By employing Bowden-cable routing for tendon mimicry, the system achieves a 60° ROM with <5 mm lateral shift. The Arduino-driven actuation delivers a peak torque of 0.18 Nm with ~180 ms latency, while integrating spring-guided soft returns and mechanical stops to ensure user safety and ergonomic comfort.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 2; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/2-1.png' | relative_url }}" 
         alt="Finger Linkage CAD Design" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Iterative CAD Packaging of Finger Linkage</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/2-2.png' | relative_url }}" 
         alt="Wearable Prototype on Hand" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Functional Prototype & Wearable Interface</strong>
    </figcaption>
  </figure>

</div>

2\. Designed a high-fidelity rehabilitation rig utilizing an electric damper and a closed-loop control architecture for smooth torque tracking. The system integrates a load cell and IMU for multi-modal sensor fusion, enabling responsive feedback and programmable resistance. By deploying an embedded sEMG decoder, the platform achieves real-time, intent-based control with a system-level latency of <500 ms, validated through rigorous actuator-response trials.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 2; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/2-3.png' | relative_url }}" 
         alt="Finger Linkage CAD Design" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>3D CAD of Wrist Rig</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/2-4.png' | relative_url }}" 
         alt="Wearable Prototype on Hand" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Wrist Rig Prototype</strong>
    </figcaption>
  </figure>

</div>

3\. Engineered a high-dimensional time-series classification pipeline utilizing a 1D-CNN architecture to decode multi-channel sEMG signals into 7 predictive categories. By integrating a real-time data acquisition and inference framework, the system achieves sub-second latency for seamless intention forecasting. The model was iteratively optimized via a data-driven feedback loop from user research trials, ensuring robust classification across diverse movement patterns and validating the rig's functionality through qualitative performance metrics.


</details>

---

## Model-Based Control System for Magnetic Whiteboard Cleaning Robot 
**Course Project: Carnegie Mellon University (CMU)**  
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Model Predictive Control (MPC)</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Trajectory Optimization (iLQR)</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">State Estimation (EKF)</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Mobile Robotics</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Arduino/Embedded Control</span>  
**Role:** Robotics and Control Systems Designer
**Summary:** Developed a differential-drive robot (WIPER) benchmarking platform to validate hybrid TVLQR/MPC tracking frameworks. Engineered a robust state estimation stack and explored multi-agent trajectory optimization using iLQR and Direct Collocation.

<details markdown="1">
  <summary><strong>View Project Details</strong></summary>

1\. Designed a hybrid TVLQR/MPC tracking framework optimized for the WIPER platform. To overcome the high latency and low bandwidth of the Bluetooth-Arduino communication link, I leveraged iLQR (Iterative LQR) for rapid trajectory generation and warm-starting. This ensured the PC-based terminal could compute optimal control inputs at high frequency, mitigating potential path instability caused by wireless transmission delays and the limited computational power of the embedded microcontroller.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/3-1.png' | relative_url }}" 
         alt="2D Trajectory Simulation" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>2D Simulation: iLQR Trajectory Optimization</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/3-2.png' | relative_url }}" 
         alt="Real-world Robot Trajectory" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Experimental Validation: Real-world Tracking</strong>
    </figcaption>
  </figure>

</div>

2\. Engineered an autonomous software stack integrating AprilTag vision localization with EKF-based sensor fusion (IMU and Encoders). The system effectively mitigates real-world sensing noise and non-systematic errors, maintaining a localization drift of <2.5 cm. This high-fidelity state estimation provides the necessary feedback for the model-based controller to execute adaptive tracking and collision avoidance in dynamic indoor environments.

</details>


---

## Self-Deployable Offshore Wave-Damping Curtain System
**Research Project: SJTU PRP Offshore Structures Group**  
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Marine Engineering</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Fluid-Structure Interaction (FSI)</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Material Science</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">CFD Simulation</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Wave-Tank Testing</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Embedded Systems</span>  
**Role:** Mechatronics Researcher and Tester
**Summary:** eveloped an autonomous, modular inflatable curtain system for offshore wave attenuation. Engineered a composite material structure and a remote deployment framework to ensure operational safety and structural integrity in harsh marine environments.

<details markdown="1">
  <summary><strong>View Project Details</strong></summary>

1\. Engineered modular curtain cells using high-strength silicone rubber encapsulated by an interconnected PVC armor-plate interface. This hybrid design provides structural rigidity, protects the internal bladders from sharp marine debris, and mitigates thermal expansion under high-temperature exposure. Achieved a rapid, tangle-free deployment sequence (<8 s) through a motorized retraction system and layered folding patterns, validated to withstand cyclic hydrodynamic loads without leakage.

2\. Developed a Raspberry Pi-based control system featuring an Infrared (IR) remote interface to enable stand-off operations from a catamaran platform, mitigating high-risk close-range manual tasks. Implemented a closed-loop pressure monitoring logic that maintains internal stability within ±3%, incorporating safety interlocks for auto-deflation and over-inflation prevention. Wave tank results demonstrated a 25–30% peak wave height reduction, confirming the system's energy dissipation efficiency.


</details>

---

## 📚 Coursework

### IV. Design of Collaborative Robotic Arms  
**Department:** Mechanical Engineering (SJTU) · Coursework  
**Role:** Designer & Simulation Engineer  
_Concept‑to‑simulation study for a collaborative arm, focusing on high payload‑to‑weight ratio, reducer selection, and internal wiring layout._

<details markdown="1">
  <summary><strong>Expand for details</strong></summary>

**Goal.**  
Design a 6-DOF collaborative arm balancing weight, torque, and manufacturability; benchmark reducers and simulate motion feasibility.

**Design & Methods.**  
- Referenced JAKA Zu5 architecture; designed hollow links for weight saving and signal/power routing.  
- Compared RV-N vs Harmonic CSD reducers under static torque demand.  
- Simscape model for verifying workspace, joint speeds, and trajectory feasibility.

<figure style="margin: 1.2rem 0;">
  <img src="{{ '/assets/img/arm.png' | relative_url }}"
       alt="Functional test outcome photo"
       style="max-width: 100%; border-radius: 12px;">
  <figcaption><strong>Collaborative Robotic Arms CAD layout</strong></figcaption>
</figure>

**Results.**  
- Achieved simulated tasks (e.g. pick‑place, ball toss) within joint torque limits.  
- Demonstrated >4:1 payload‑to‑weight ratio; enabled joint modularization for future prototypes.

</details>

---
### V. Self‑Leveling Tripod (Patent Applied)  
**Department:** Mechanical Engineering (SJTU) · Coursework  
**Role:** Designer & Embedded Developer  
_Accessibility‑oriented tripod that auto‑levels using IMU‑based sensing and servo correction; structure validated with FEA._

<details markdown="1">
  <summary><strong>Expand for details</strong></summary>

**Goal.**  
Develop a self-leveling tripod that minimizes manual adjustment for users with limited mobility or field use cases.

**Design & Methods.**  
- IMU measures tilt; Arduino computes correction offsets; 3 servos adjust individual legs.  
- Boot sequence ensures smooth startup leveling without instability.  
- FEA simulations confirm leg/frame stiffness and load capacity under typical camera payloads.

<figure style="margin: 1.2rem 0;">
  <img src="{{ '/assets/img/tripod.png' | relative_url }}"
       alt="Functional test outcome photo"
       style="max-width: 100%; border-radius: 12px;">
  <figcaption><strong>Self‑Leveling Tripod CAD layout</strong></figcaption>
</figure>

**Results.**  
- Reliable auto-leveling on uneven surfaces at boot.  
- Structural deflection < 0.3 mm under expected loading.  
- Patent filing submitted based on novelty in mechanical design and control workflow.

</details>
---
### VI. Magnetic Whiteboard Cleaning Robot (WIPER) — Model-Based Control & Trajectory Optimization  
**Department:** Mechanical Engineering (CMU) · Coursework  
**Role:** Mechatronics Engineer  
_Differential-drive platform for controller benchmarking and trajectory optimization, integrating AprilTag localization and EKF sensor fusion. Also serves as basis for multi-agent planner–controller stack._

<details markdown="1">
  <summary><strong>Expand for details</strong></summary>

**Goal.**  
Build a model-based controller benchmarking platform (TVLQR vs MPC) with real-world sensing and control. Extend to trajectory optimization for multi-agent platforms with planner-to-controller compatibility.

**Design & Methods.**  
- **WIPER baseline module:** TVLQR and MPC tracking implemented over RK4 dynamics. EKF fuses encoder and IMU data with AprilTag localization for robust state estimation. Log-based ablation supports repeatability.  
- **Model-based control coursework module:** Setup reused to produce reproducible plots, tuning routines, and failure-case evaluations.  
- **Trajectory optimization module (planar quadrotors):** iLQR for warm-starting; DIRCOL for constraint enforcement including reorientation and inter-agent separation. Explored Hermite–Simpson integration and cost shaping.

**Results.**  
- Consistent controller performance on varying test paths.  
- TVLQR showed superior stability; MPC allowed greater responsiveness under tight constraints.  
- EKF localization errors <2.5 cm drift on average.  
- TrajOpt experiments yielded 3-agent collision-free paths under dynamic feasibility, validated by cost/time metrics.  
- Framework informs future planner–controller integration stack for multi-agent systems.

</details>
---
### VII. Simulated Jumping Bionic Frog  
**Department:** Mechanical Engineering (SJTU) · Coursework / Competition  
**Role:** Mechanical Designer  
_Contest‑oriented robotic frog using spring-powered legs and compact actuation to achieve horizontal jumping motion._

<details markdown="1">
  <summary><strong>Expand for details</strong></summary>

**Goal.**  
Design a lightweight jumping mechanism for horizontal distance optimization under actuator and size constraints.

**Design & Methods.**  
- **Drive system:** Incomplete-gear mechanism winds and releases a leg-mounted spring for explosive jump power.  
- **Structure:** Parallel 1-DoF linkage design stabilizes center of gravity; MG996R 360° servo drives the energy cycle.  
- **Controls:** Arduino Uno handles trigger timing and energy release; leg-body integration cushions landing and limits rebound.  
- **Simulations:** Kinematic and dynamic simulations inform optimal stroke length and angle.

**Results.**  
- Reached ~20 cm horizontal jump distance with minimal post-jump oscillation.  
- Reliable takeoff/landing on flat indoor surfaces.  
- Structure and gearing reused for later bionic-jump prototypes.

</details>


---
### VIII. A 2D Shooting Game (CMU_graphics)  
**Department:** Mechanical Engineering (CMU) · Coursework  
**Role:** Developer  
_2D Python shooting game with multiple levels, animations, and structured codebase using CMU_graphics._

<details markdown="1">
  <summary><strong>Expand for details</strong></summary>

**Goal.**  
Design a complete action game in Python using CMU_graphics with polished gameplay, modular code, and UI/UX refinement.

**Design & Methods.**  
- **Architecture:** Multi-file Python project with modules for main loop, UI, assets, and character/enemy logic.  
- **Gameplay:** Includes health, buffs, cooldowns, map switching, and enemy types; optimized timing and input feedback.  
- **Assets:** Lazy loading for weapons/maps/characters to improve runtime performance and expandability.

**Results.**  
- Fully playable game demo with stable mechanics and transitions.  
- Modular and well-documented code structure supports future features (e.g., multiplayer, online scores).  
- Positive peer feedback and smooth demo showcase during course final.

<figure style="margin: 1.2rem 0;">
  <img src="{{ '/assets/img/game1.png' | relative_url }}"
       alt="Functional test outcome photo"
       style="max-width: 100%; border-radius: 12px;">
</figure>
<figure style="margin: 1.2rem 0;">
  <img src="{{ '/assets/img/game2.png' | relative_url }}"
       alt="Functional test outcome photo"
       style="max-width: 100%; border-radius: 12px;">
  <figcaption><strong>Real game desktop screen shoot</strong></figcaption>
</figure>

</details>


