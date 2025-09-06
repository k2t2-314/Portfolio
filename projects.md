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
  <figcaption><strong>
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
       alt="Full CAD assembly of gantry"
       style="max-width: 100%; border-radius: 12px;">
  <figcaption><strong>
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
       alt="Full CAD assembly of gantry"
       style="max-width: 100%; border-radius: 12px;">
  <figcaption><strong>
</figure>

</details>

---

### Bionic Mandibular Robot (Undergraduate)
_Anthropomorphic robotic jaw with actuation & control experiments_

**Overview.** Biomimetic mechanism studying jaw motion and actuation strategies.

**Design & Controls.** Mechanism synthesis; embedded control and initial feedback strategies; safety and repeatability checks.

**Status & Impact.** Early validation of kinematics & actuation; basis for future bio‑robotic studies.

**Department.** Mechanical Engineering (SJTU)

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** Anthropomorphic linkage; compliance tuning; measurement fixtures.

</details>

---
### Self‑Deployable Offshore Wave‑Damping Curtain System
_Modular inflatable structure with embedded control; wave‑tank validated_

**Overview.** Research assistant project developing a deployable curtain to damp waves for offshore use.

**Design & Controls.** Curtain deployment mechanism; embedded control (Raspberry Pi); test procedures for hydrodynamic performance.

**Status & Impact.** Wave‑tank experiments validate concept feasibility and deployment reliability.

**Department.** Mechanical Engineering (SJTU)

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** Deployment dynamics; seal/inflation integrity; control routines for safe actuation.

</details>

---

## 📚 Coursework

### Design of Collaborative Robotic Arms
_High payload‑to‑weight ratio; internal wiring; reducer selection & simulation_

**Overview.** Concept‑to‑simulation study for a collaborative arm focusing on internal wiring and reducer/motor selection.

**Design & Controls.** Reference JAKA Zu5 form factor; reducer selection (RV‑N / Harmonic CSD) via static torque; Simscape model for kinematics/dynamics.

**Status & Impact.** Validated trajectories in simulation; groundwork for advanced tasks (e.g., ball‑juggling path planning).

**Department.** Mechanical Engineering (SJTU)

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** Hollow links for wire routing & weight reduction; torque/mass trade‑offs; modular joint stack.

</details>

---
### Self‑Leveling Tripod (Patent Applied)
_Arduino + IMU + 3 servos; FEA‑validated structure_

**Overview.** Accessibility‑oriented tripod that auto‑levels to reduce user strain.

**Design & Controls.** IMU senses tilt → Arduino computes corrections → 3 servos actuate legs; structure optimized with FEA.

**Status & Impact.** Prototype achieves reliable self‑leveling on startup; roadmap includes closed‑loop tuning & robustness tests.

**Department.** Mechanical Engineering (SJTU)

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** Open‑loop with IMU feedback; smooth boot sequence; lightweight chassis.

</details>

---
### Magnetic Whiteboard Cleaning Robot (WIPER) — Model-Based Control & Trajectory Optimization
_Differential-drive platform with TVLQR/MPC tracking, AprilTag localization, EKF sensor fusion; includes a coursework module and a multi-agent trajectory-optimization extension_

**Overview.** Unified research & coursework project built around WIPER for model-based control benchmarking and planning. Compares TVLQR vs MPC under real-world localization, and extends to multi-agent planar quadrotor trajectory optimization to prototype planner–controller ideas.

**Design & Controls.** RK4 integration; EKF (IMU/encoders) + AprilTag localization; velocity-reference adaptation and heading-drift mitigation; controller ablation (TVLQR vs MPC). Trajectory-optimization extension uses iLQR for warm starts and DIRCOL for constraint satisfaction (reorientation + separation).

**Status & Impact.** Demonstrated robust tracking on varied paths with reusable logging/evaluation tools. Coursework produced reproducible controller baselines. The multi-agent trajopt module generates dynamically feasible, collision-free paths that inform planner–controller stack design.

**Department.** Mechanical Engineering (CMU) · Coursework

<details>
  <summary><strong>Expand for module details</strong></summary>

#### Capstone module (WIPER baseline)
- **Goal.** Empirically compare TVLQR vs MPC with real-world sensing.
- **Methods.** RK4 dynamics; EKF (IMU/encoders) + AprilTag; log-based evaluation.
- **Highlights.** Controller comparison framework; reusable tooling for future platforms.

#### Coursework module (Model-Based Control System)
- **Goal.** Turn the research setup into reproducible classroom baselines.
- **Methods.** Standardized datasets/plots; failure-case analysis; data-driven tuning.
- **Highlights.** Clean scripts for repeatable benchmarks and reports.

#### Trajectory optimization module (Three planar quadrotors)
- **Goal.** Prototype planner ideas for multi-agent coordination.
- **Methods.** iLQR warm starts; DIRCOL with reorientation & min-separation constraints.
- **Highlights.** RK4 vs Hermite-Simpson integration; cost shaping vs direct constraints; parameter sweeps.

</details>
---

### Recipe Recommender System
_Python‑based recommender with logistic‑preference modeling & multi‑objective scoring_

**Overview.** Builds like/protein/cost/time objectives into a unified ranking; ingredient‑aware filtering.

**Design & Controls.** Logistic regression preference model; ipywidgets UI for selections; robust ingredient management; egg keyword matching; meat tag column for filtering.

**Status & Impact.** Interactive notebook with confirm/feedback loop; extensible dataset processing.

**Department.** Mechanical Engineering (CMU) · AI for Engineers · Coursework

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** Cold‑start defaults; deterministic UI state; fast filtering pipeline.

</details>
---

### Light‑Tracking Turret (Photoresistor‑based)
_Four photoresistors + dual‑axis servos; Arduino Uno signal chain_

**Overview.** Light‑tracking turret for pointing/aiming tasks; inspired by return‑to‑dock behaviors.

**Design & Controls.** Two photoresistor pairs compute intensity deltas → servo angles; Arduino control loop.

**Status & Impact.** Low‑cost, compact, wide rotation; applicable to solar tracking / directional lighting.

**Department.** Mechanical Engineering (SJTU) · Coursework

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** Sensor‑to‑actuator mapping; noise handling; calibration routine.

</details>
---

### Automatic Seed Planting & Pot‑Forming Device
_Integrated pot forming + single‑seed metering with spring‑aided wheel_

**Overview.** One‑pass pot forming and seeding for low‑carbon agriculture.

**Design & Controls.** Rotating disk for seed distribution; coil‑spring‑assisted grooves ensure single‑seed metering; frame + pedal structure extrudes soil pots.

**Status & Impact.** Raises operation efficiency; adaptable to small‑scale cotton planting and other single‑piece feed processes.

**Department.** Mechanical Engineering (SJTU) · Coursework / Competition

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** Single‑wheel rope drive; spring rebound timing; keeper geometry.

</details>
---

### Simulated Jumping Bionic Frog
_Incomplete‑gear spring drive; ~20 cm horizontal jump_

**Overview.** Contest‑oriented jumping robot; performance measured by horizontal distance.

**Design & Controls.** Incomplete gear stretches leg spring; consolidated front‑limb/body for impact cushioning; MG996R 360° servo + Arduino R3.

**Status & Impact.** Lightweight, low‑energy design achieving ~20 cm horizontal jumps on flat ground.

**Department.** Mechanical Engineering (SJTU) · Coursework / Competition

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** 1‑DoF parallel linkage prevents CoG‑forward rollover; kinematics/dynamics sims guide stroke.

</details>

---
### A 2D Shooting Game (CMU_graphics)
_Multi‑file Python app; gameplay & UI/UX polish_

**Overview.** Term project building a complete 2D action game with levels & buffs.

**Design & Controls.** Multi‑module architecture (main loop, lazy loading, effects, class defs); galleries for maps/weapons/characters.

**Status & Impact.** Playable build with demo; codebase structured for future expansion.

**Department.** CMU · Coursework

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** Gameplay loop tuning; animation timing; input handling.

</details>


