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

# 🛠 Projects

## 🤝 Industry Collaboration

### I. Flexible Lubricator Handling & Inspection Platform  
**Department:** Mechanical Engineering (SJTU) · Industry collaboration with Well Master Corporation  
**Role:** Lead Mechanical Designer  
_A modular 5‑DOF gantry lifts ~200‑lb lubricators, reorients them horizontally to vertically, and enables inspection via real-time object detection; validated by a 2:1 prototype using CAD/FEA and multi-actuator fuzzy PID._

<details markdown="1">
  <summary><strong>Expand for details</strong></summary>

**Goal.**  
Develop a production-ready system to automate the extraction, flipping, and inspection of lubricators stored in bulk shipping crates. The solution must be mechanically robust, operator-safe, and capable of integrating with an intelligent vision system to replace manual handling.

**Design & Methods.**  
- **Mechanical system:**  
  Designed a modular 5‑DOF cantilever gantry using aluminum profiles and custom brackets; verified critical joints and beams with ANSYS static analysis and modal simulation to ensure <1 mm deflection under load.  
  The flipping mechanism uses a torque-matched motorized platform with lateral stabilizers to maintain balance during rotation.  
  The flexible gripper combines compliant silicone pads with passive alignment geometry to accommodate shape variance in lubricators.

- **Control architecture:**  
  Implemented multi-actuator coordination using fuzzy PID (for Z-axis deceleration and gripper soft-landing) and coupled PID (for synchronized gantry motion). Safety interlocks prevent flipping when out-of-alignment or over-torque is detected.

- **Perception system:**  
  Integrated YOLOv11-based object detection to locate visual inspection regions (e.g. ports, labels, connector points) and to automatically trigger pass/fail decisions. Data is logged for traceability.

**Results / Metrics.**  
- Built and tested a 2:1 prototype demonstrating successful lifting and flipping with high repeatability.  
- **Structure:** FEA confirmed maximum deflection < 0.7 mm under 100 N equivalent load; modal frequency > 25 Hz avoids vibration.  
- **Control:** Flipping stability achieved with <3° overshoot and <2.5 s settle time.  
- **Perception:** Real-time inference (25 FPS) with >92% detection accuracy on known components; integrated inspection pass/fail logic.  
- **Throughput:** Task cycle time reduced by ~40% compared to manual workflow.  
- Delivered CAD package, electrical/control schematic, and final report to Well Master Corp.

<figure style="margin: 1.2rem 0;">
  <img src="{{ '/assets/img/assembly.png' | relative_url }}"
       alt="Full CAD assembly of gantry"
       style="max-width: 100%; border-radius: 12px;">
  <figcaption><strong>Full CAD assembly of 5‑DOF gantry system</strong></figcaption>
</figure>


</details>

---

## 🔬 Research

### II. Hand Exoskeleton – Finger Actuation Module  
**Department:** Mechanical Engineering (CMU)  
**Role:** Researcher – Exoskeleton Lab, Neuroscience Institute  
_A low-profile, user-conforming actuator system for finger flexion/extension, integrating ergonomic routing and embedded control; validated through user testing and mechanical refinement._

<details markdown="1">
  <summary><strong>Expand for details</strong></summary>

**Goal.**  
Develop a wearable, comfortable, and testable actuation module for single-finger motion assistance. The design must minimize bulk, ensure safe force transmission, and enable future EMG-based control.

**Design & Methods.**  
- **Mechanical design:** Iterative CAD packaging for finger linkage, actuation cable routing, and palm-mounted motor housing. Focused on low-profile layout and mechanical safety (e.g. finger stops, soft returns).  
- **Actuation system:** Embedded control using Arduino-compatible microcontroller, motor driver, and feedback loop. Used mini DC gearmotor with Bowden-cable routing for tendon mimicry.  
- **EMG integration (exploratory):** Bench-tested surface EMG preprocessing and activation thresholds using MyoWare sensors to explore user-intent-based triggering logic.  
- **Ergonomics:** Conducted comfort trials with 4 participants; quick-release Velcro glove mount for easy donning/doffing; adjustable tension and actuation limits.
- 
<figure style="margin: 1.2rem 0;">
  <img src="{{ '/assets/img/Exo.png' | relative_url }}"
       alt="Wearable finger actuator module"
       style="max-width: 100%; border-radius: 12px;">
  <figcaption><strong>Wearable finger actuator CAD layout</strong></figcaption>
</figure>


**Results / Metrics.**  
- Functional finger flex/extend motion over ~60° ROM with <5 mm lateral shift from neutral position.  
- Actuation latency ~180 ms from command trigger; peak torque transmission up to 0.18 Nm.  
- Passive return achieved via spring-guided neutral restoration; user safety enhanced with mechanical stops.  
- Feedback from user tests guided improvements to comfort, strap interface, and routing constraints.  
- Final design informs upcoming multi-finger exoskeleton framework.  
- **A machine-learning-based decoder for EMG intent detection is currently under development** to support multi-modal, user-adaptive control strategies.

<figure style="margin: 1.2rem 0;">
  <img src="{{ '/assets/img/outcomeExo.png' | relative_url }}"
       alt="Functional test outcome photo"
       style="max-width: 100%; border-radius: 12px;">
  <figcaption><strong>Functional prototype validation & outcome test</strong></figcaption>
</figure>


</details>

---
### III. Self‑Deployable Offshore Wave‑Damping Curtain System  
**Department:** Mechanical Engineering (SJTU)  
**Role:** Researcher – PRP Offshore Structures Group  
_A modular, inflatable curtain system designed to autonomously deploy at sea and attenuate wave energy; validated through wave-tank testing and embedded control._

<details markdown="1">
  <summary><strong>Expand for details</strong></summary>

**Goal.**  
Develop a robust, self-deploying inflatable curtain for offshore wave damping. The system must function autonomously, withstand hydrodynamic loads, and demonstrate reliable sealing and actuation.

**Design & Methods.**  
- **Mechanical structure:** Modular curtain cells fabricated from flexible, waterproof fabric with internal air channels. Designed custom inflation ports with redundant sealing rings to withstand repeated cycles and pressure spikes.  
- **Deployment system:** Motorized retraction + inflation sequence using pressurized air canisters; unrolls curtain with timed actuation. Compact stowage size and layered folding pattern ensured rapid and tangle-free deployment.  
- **Embedded control:** Raspberry Pi 3B+ used for real-time control of valve opening, pump activation, and pressure monitoring. Safety interlocks prevent over-inflation; auto-deflation included for retrieval.  
- **Testing setup:** Built scaled prototype for wave tank testing; tracked curtain dynamics under regular and irregular wave conditions using overhead camera system and pressure sensors.

**Results / Metrics.**  
- Achieved successful deployment in <8 s in all trials with full curtain inflation and locking in place.  
- Maintained seal integrity for >20 minutes with no leakage under cyclic wave loading.  
- Peak wave height reduction of ~25–30% in downstream measurement zones, validating energy dissipation.  
- Embedded controller maintained internal pressure within ±3% of target range using closed-loop sensing.  
- Control sequence and mechanical layout delivered as a reproducible reference system for offshore damping studies.

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


