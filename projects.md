---
layout: default
title: Projects
permalink: /projects.html
---

<!-- Navigation -->
<div style="margin-bottom: 30px;">
  <a href="{{ '/' | relative_url }}"> Home</a> |
  <a href="{{ '/resume.html' | relative_url }}"> Resume</a> |
  <a href="{{ '/projects.html' | relative_url }}"> Projects</a> |
</div>

# Projects
---

## Flexible Lubricator Handling Platform
**Dec 2024 – Jun 2025**  
**Industry Collaboration: WellMaster Corporation, SJTU**  
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Computer Vision</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">PID Control</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Mechanical Design</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">ANSYS</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Parameter Optimization</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">SolidWorks</span>  
**Role:** Lead Mechanical Designer    
**Summary:** Developed a production-ready 5-DOF gantry system that automates the extraction, reorientation and visual inspection of industrial lubricators, increasing throughput and saving operation time.  
**Impact:** Eliminates manual handling of 200 lb lubricators in hazardous factory environments, reducing workplace injury risk while enabling 24/7 automated quality control at industrial scale.

<details markdown="1">
  <summary><strong>View Project Details</strong></summary>
<div style="margin-bottom: 8px;"></div>

1\. Designed a modular 5-DOF cantilever gantry and a torque-matched flipping platform using aluminum profiles and custom brackets. Conducted **ANSYS static** and **modal simulations** to validate structural integrity, successfully limiting maximum deflection to **<0.7 mm** and ensuring a modal frequency **>25 Hz** to eliminate operational resonance.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 1.8; margin: 0; text-align: center;">
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

2\. Implemented multi-actuator coordination utilizing **Fuzzy PID** for Z-axis soft-landing and coupled PID for synchronized 5-axis gantry motion. Integrated real-time safety interlocks via torque sensing and IMU-based alignment, achieving flipping stability with **<3°** overshoot and a settling time of **<2.5 s**.

<figure style="margin: 1.5rem auto; text-align: center; max-width: 85%;">
  <img src="{{ '/assets/img/1-4.png' | relative_url }}" 
       alt="Full CAD assembly" 
       style="width: 100%; height: auto; border-radius: 12px; border: 1px solid #eee;">
  <figcaption style="margin-top: 0.8rem; font-size: 0.85rem; color: #555;">
    <strong>Control System Architecture & Simulation via Simulink</strong>
  </figcaption>
</figure>

3\. Engineered a real-time perception system by deploying a **YOLOv11 model**, utilizing a **Sim-to-Real data strategy** (3D CAD models and real-world photography). Achieved **92% mAP** for multi-class part detection, enabling fully automated inspection logic.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 1.2; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/1-6.png' | relative_url }}" 
         alt="YOLOv11 Training Metrics" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>YOLOv11 Training mAP Curve</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/1-7.png' | relative_url }}" 
         alt="Real-time Inference and Localization" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Real-time Localization</strong>
    </figcaption>
  </figure>

</div>

</details>

<div style="margin-bottom: 8px;"></div>
---

## Neuro-Mechatronics Lab, CMU
**Sep 2025 - Present**   
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Exoskeleton</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Biosignal Processing</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Wearable Devices</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Embedded Systems</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">3D Printing</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Deep Learning</span>  
**Role:** Graduate Research Assistant  
**Summary:** Designed a wearable actuation module for hand exoskeletons featuring an integrated sEMG decoder. The system assists SCI patients in daily tasks via finger actuation while utilizing the wrist module for high-fidelity signal processing and intention decoding to close the loop for rehabilitation.  
**Impact:** Provides spinal cord injury (SCI) patients with an intent-driven assistive device that restores functional hand movement, supporting independence in daily tasks and accelerating motor rehabilitation.  

<details markdown="1">
  <summary><strong>View Project Details</strong></summary>
<div style="margin-bottom: 8px;"></div>
  
1\. Developed a light wearable finger linkage featuring iterative CAD packaging for cable routing and palm-mounted motor housing. The system achieves **33%** improvement in wrist range of motion in patient trials. The Arduino-driven actuation delivers a peak torque of **0.18 Nm** while integrating spring-guided soft returns and mechanical stops to ensure user safety and ergonomic comfort.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 1.8; margin: 0; text-align: center;">
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
      <strong>Functional Prototype</strong>
    </figcaption>
  </figure>

</div>

2\. Designed a high-fidelity rehabilitation rig utilizing an electric damper and a closed-loop control architecture for smooth torque tracking. The system integrates a load cell and IMU for **multi-modal** sensor fusion, enabling responsive feedback and programmable resistance. This device ensures the acquisition of **high-quality dEMG** data within the framework of scientific experimental design, achieving a repetitive tracking error of less than **0.5°**.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/2-3.png' | relative_url }}" 
         alt="Finger Linkage CAD Design" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>3D CAD of Wrist Rig</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/GUI.png' | relative_url }}" 
         alt="Wearable Prototype on Hand" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Experiment GUI</strong>
    </figcaption>
  </figure>

</div>


3\. Engineered a high-dimensional time-series classification pipeline comparing 1D-CNN, RNN, and Random Forest algorithms to decode multi-channel sEMG signals into 7 predictive categories, achieving **85% accuracy in cross-day testing**. By integrating a real-time data acquisition and inference framework, the system achieves sub-second latency for seamless intention forecasting. The model was iteratively optimized via a data-driven feedback loop from user research trials, ensuring robust classification across diverse movement patterns.

</details>
<div style="margin-bottom: 8px;"></div>
---

## Generative Diffusion on Dexterous Hands
**Jan 2026 - May 2026**  
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Diffusion Policy</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Reinforcement Learning</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">PPO</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">IsaacLab</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Dexterous Manipulation</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Robot Simulation</span>  
**Role:** Algorithm Researcher   
**Summary:** Reproduced and extended a generative diffusion on-policy learning pipeline in IsaacLab to enhance the expressiveness of on-policy RL algorithms for dexterous manipulation tasks. Conducted ablation experiments to evaluate alternative stochastic estimation methods within the diffusion process.  
**Impact:** Demonstrated that Hutchinson stochastic estimation can offer a more efficient path toward real-time dexterous manipulation.  

<details markdown="1">
  <summary><strong>View Project Details</strong></summary>

<div style="margin-bottom: 8px;"></div>

1\. Established and reproduced a full diffusion policy learning pipeline in **IsaacLab**, integrating on-policy training with **a generative diffusion model** to improve action distribution expressiveness for complex manipulation tasks including object reorientation. This algorithm can slightly outperform **PPO** under the same training environment, and far surpasses PPO under better **GPU** environments.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/environment.png' | relative_url }}" 
         alt="Finger Linkage CAD Design" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Simulation Environment</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/reward_all_method.png' | relative_url }}" 
         alt="Wearable Prototype on Hand" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Comparison of Rewards</strong>
    </figcaption>
  </figure>

</div>

2\. Designed and conducted ablation experiments comparing **Jacobian-based** and **Hutchinson stochastic trace estimation** within the diffusion process. The Hutchinson method achieved **90%** of the original reward value while reducing per-step computation time, validating its viability as a lightweight alternative for real-time deployment scenarios.


</details>
<div style="margin-bottom: 8px;"></div>
---

## Auto-Meshing App for FEA Optimization
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Scientific Computing</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Finite Element Analysis (FEA)</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Machine Learning (MLP)</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Feature Engineering</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Full-Stack Deployment</span>  
**Role:** Backend & Feature Science Developer  
**Summary:** Developed a fully automated pipeline for FEA simulation and mesh optimization. Integrated geometric feature extraction with deep learning to predict optimal mesh parameters, significantly accelerating the pre-processing workflow for mechanical components.  
**Impact:** Reduces manual FEA pre-processing time for mechanical engineers, lowering the barrier to simulation-driven design and enabling faster, more reliable product development cycles.


<details markdown="1">
  <summary><strong>View Project Details</strong></summary>

<div style="margin-bottom: 8px;"></div>

1\. Developed an end-to-end FEA automation framework using PyAnsys to generate scalable datasets from STEP CAD models. I engineered a Python-based feature extraction module that translates complex geometric entities (holes, fillets, faces) into numerical descriptors. This allows the system to "understand" the mechanical significance of different part regions, forming the basis for intelligent mesh refinement.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/6-2.png' | relative_url }}" 
         alt="FEA Training Dataset" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Training Dataset: Labeled FEA Samples</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1.2; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/6-1.png' | relative_url }}" 
         alt="Auto-Meshing Inference Results" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Inference Results: ML-Predicted Mesh Refinement</strong>
    </figcaption>
  </figure>

</div>


2\. Trained a Multilayer Perceptron (MLP) model to predict optimal mesh parameters by combining rule-based heuristics with learned geometric patterns. The model achieved 75% accuracy and 90% recall despite limited data. The entire backend was containerized via Docker and deployed as an open-source application on Hugging Face, providing a user-friendly interface for real-time mesh refinement suggestions.

<div style="margin: 1.5rem 0; text-align: center;">
  <figure style="max-width: 90%; margin: 0 auto;">
    <img src="{{ '/assets/img/6-3.png' | relative_url }}" 
         alt="App User Interface" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee; box-shadow: 0 4px 12px rgba(0,0,0,0.08);">
    <figcaption style="margin-top: 0.8rem; font-size: 0.85rem;">
      <strong>Cloud Deployment: Interactive Mesh-Refinement Interface</strong>
    </figcaption>
  </figure>
</div>

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
**Impact:** Demonstrates a low-cost autonomous cleaning platform applicable to shared workspaces and classrooms, validating model-based control frameworks that generalize to mobile service robotics.

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
**Summary:** Developed an autonomous, modular inflatable curtain system for offshore wave attenuation. Engineered a composite material structure and a remote deployment framework to ensure operational safety and structural integrity in harsh marine environments.   
**Impact:** Protects offshore infrastructure and marine workers from wave damage in harsh sea conditions, offering a rapidly deployable, reusable alternative to permanent coastal protection structures.
 
<details markdown="1">
  <summary><strong>View Project Details</strong></summary>

1\. Engineered modular curtain cells using high-strength silicone rubber encapsulated by an interconnected PVC armor-plate interface. This hybrid design provides structural rigidity, protects the internal bladders from sharp marine debris, and mitigates thermal expansion under high-temperature exposure. Achieved a rapid, tangle-free deployment sequence (<8 s) through a motorized retraction system and layered folding patterns, validated to withstand cyclic hydrodynamic loads without leakage.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 1.2; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/4-1.png' | relative_url }}" 
         alt="Curtain System CAD Design" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>SolidWorks CAD: Modular Curtain & PVC Armor</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/4-2.png' | relative_url }}" 
         alt="Prototype Real-shot" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Experimental Prototype: Wave-Tank Validation</strong>
    </figcaption>
  </figure>

</div>


2\. Developed a Raspberry Pi-based control system featuring an Infrared (IR) remote interface to enable stand-off operations from a catamaran platform, mitigating high-risk close-range manual tasks. Implemented a closed-loop pressure monitoring logic that maintains internal stability within ±3%, incorporating safety interlocks for auto-deflation and over-inflation prevention. Wave tank results demonstrated a 25–30% peak wave height reduction, confirming the system's energy dissipation efficiency.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/4-3.png' | relative_url }}" 
         alt="Wave Height vs Distance Plot" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Wave Height vs. Distance: Regular Sea States</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/4-4.png' | relative_url }}" 
         alt="Wave Energy Dissipation Results" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Wave Energy Dissipation: Irregular Sea States</strong>
    </figcaption>
  </figure>

</div>


</details>

---

## Collaborative Robotic Arm Design and Simulation  
**Course Project: SJTU, Robotics**  
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Robotic Manipulators</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Mechanism Design (CAD/CAE)</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">MATLAB/Simulink</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Kinematics & Dynamics</span>
<span style="background: #f0f0f0; border: 1px solid #ccc; border-radius: 4px; padding: 2px 6px; font-family: monospace; font-size: 0.9em; white-space: nowrap;">Trajectory Planning</span>  
**Role:** Designer & Simulation Engineer  
**Summary:** Engineered a lightweight, 6-DOF collaborative robotic arm with an optimized payload-to-weight ratio. Conducted comprehensive market benchmarking and MATLAB-based dynamic simulations to validate high-precision trajectory tracking for collaborative manipulation tasks.  
**Impact:** Advances the design of lightweight collaborative robots for human-safe manufacturing environments, where payload efficiency directly translates to lower energy costs and broader deployment feasibility.

<details markdown="1">
  <summary><strong>View Project Details</strong></summary>

1\. Inspired by industrial standards like the JAKA Zu5, I designed a hollow-structure 6-DOF robotic arm that improves the payload-to-weight ratio by >25%. The design supports internal wiring and achieves a 1m reach within a total weight envelope of <2kg. Through rigorous CAD modeling and benchmarking against UR5e and Franka Emika, I optimized the joint configurations for peak torque, stiffness, and seamless integration of reducers and motors.


<div style="margin: 1.5rem 0; text-align: center;">
  
  <figure style="max-width: 80%; margin: 0 auto;">
    <img src="{{ '/assets/img/5-1.png' | relative_url }}" 
         alt="Collaborative Robotic Arm CAD Design" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee; box-shadow: 0 4px 10px rgba(0,0,0,0.05);">
    <figcaption style="margin-top: 0.8rem; font-size: 0.85rem;">
      <strong>6-DOF Collaborative Arm: Lightweight Hollow-Structure CAD Model</strong>
    </figcaption>
  </figure>

</div>


2\. Developed a MATLAB-based simulation framework to demonstrate advanced motion capabilities, including complex 3D trajectory tracking (e.g., dual-arm ball juggling). The system achieved an RMS path tracking error of <1.5mm, showcasing the feasibility of real-time collaborative manipulation. This data-driven approach ensured that the motor and reducer selections met the dynamic requirements of high-speed, high-precision industrial applications.

<div style="display: flex; justify-content: space-between; align-items: flex-end; gap: 15px; margin: 1.2rem 0;">
  
  <figure style="flex: 1; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/5-2.png' | relative_url }}" 
         alt="Robotic Arm Workspace Analysis" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Workspace Analysis: 1m Reach Visualization</strong>
    </figcaption>
  </figure>

  <figure style="flex: 1.2; margin: 0; text-align: center;">
    <img src="{{ '/assets/img/5-4.png' | relative_url }}" 
         alt="Ball Juggling Path Tracking Results" 
         style="width: 100%; border-radius: 12px; border: 1px solid #eee;">
    <figcaption style="margin-top: 0.5rem; font-size: 0.85rem;">
      <strong>Motion Simulation: Ball Juggling Path Tracking</strong>
    </figcaption>
  </figure>

</div>

</details>

---



