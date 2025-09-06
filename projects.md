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

*Grouped into three buckets: **Industry Collaboration | Research | Coursework***

---

## 🤝 Industry Collaboration / 企业合作 {#industry}

### Flexible Lubricator Handling & Inspection Platform
_A modular 5‑DOF gantry with a vision‑assisted flexible gripper for ≈200‑lb lubricators_

**Overview.** Production‑oriented handling & inspection cell that lifts lubricators from crates, reorients them horizontal→vertical, and supports vision‑guided inspection.

**Design & Controls.** Modular 5‑DOF gantry + flipping platform + flexible gripper. Structure sized/verified via CAD/FEA (SolidWorks/ANSYS). Controls use coupled/fuzzy PID for multi‑actuator coordination with safety interlocks.

**Status & Impact.** 2:1 prototype validated mechanism & control strategy. Real‑time object detection integrated for inspection automation; reduces manual handling risk.

**Department.** Mechanical Engineering (CMU) · Industry collaboration with Well Master Corporation

<details>
  <summary><strong>Expand for details</strong></summary>

**Architecture (Condensed).** Mechanics: modular rails, reinforced carriage, compliant fingers. Actuation: synchronized multi‑axis; flip/settle profiles. Controls: coupled/fuzzy PID; interlocks; calibration. Perception: real‑time object detection; inspection checklist hooks.

**Notes / Metrics (examples).** FEA‑checked stiffness/deflection on critical members; repeatable flipping with drift suppression & tuned settle time; pass/fail logging pipeline.

</details>

---

## 🔬 Research / 科研 {#research}

### Magnetic Whiteboard Cleaning Robot (WIPER)
_Differential‑drive robot with TVLQR vs MPC trajectory tracking, AprilTag localization, and EKF fusion_

**Overview.** Research platform for comparing TVLQR vs MPC tracking with real‑world localization and sensor fusion.

**Design & Controls.** RK4 integration; EKF (IMU/encoders) + AprilTag; velocity‑reference adaptation and heading‑drift mitigation.

**Status & Impact.** Demonstrated robust tracking on varying paths; ablation between controllers informs controller selection and tuning.

**Department.** Mechanical Engineering (CMU)

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** Controller comparison framework; log‑based evaluation; reusable tooling for future platforms.

</details>

### Hand Exoskeleton – Finger Actuation Module
_Wearable finger actuators with compact design and user testing_

**Overview.** Design of compact, wearable finger actuation with comfort‑driven iterations and human‑in‑the‑loop feedback.

**Design & Controls.** CAD/mechanism packaging; embedded control; explored EMG‑driven concepts and safe force transmission.

**Status & Impact.** Functional prototype validated fit & repeatability; informed future multi‑finger integration.

**Department.** Mechanical Engineering (CMU)

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** Low‑profile routing; quick‑release features; safety stops.

</details>

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

## 📚 Coursework / 课设 {#coursework}

### Model‑Based Control System for Magnetic Whiteboard Cleaning Robot
_Course project focusing on TVLQR & MPC control with sensor fusion_

**Overview.** Course adaptation of the WIPER platform for model‑based control benchmarking.

**Design & Controls.** TVLQR/MPC comparison; AprilTag‑based localization; EKF fusion of IMU/encoders.

**Status & Impact.** Produced reproducible controller baselines and evaluation scripts.

**Department.** Mechanical Engineering (CMU) · Coursework

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** Data‑driven tuning; failure‑case analysis; standardized plots & metrics.

</details>

### Trajectory Optimization of Three Planar Quadrotors
_Optimizing collision‑free trajectories with iLQR and DIRCOL methods_

**Overview.** Coursework exploring multi‑agent trajectory optimization with separation constraints.

**Design & Controls.** iLQR for warm starts; DIRCOL for constraint satisfaction; reorientation and minimum‑separation enforcement.

**Status & Impact.** Generated dynamically feasible, collision‑free paths under task constraints.

**Department.** Mechanical Engineering (CMU) · Coursework

<details>
  <summary><strong>Expand for details</strong></summary>

**Highlights.** RK4 vs Hermite‑Simpson integration; cost shaping vs direct collision constraints; parameter sweeps.

</details>

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


