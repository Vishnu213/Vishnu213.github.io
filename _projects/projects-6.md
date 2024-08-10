---
title: "Attitude control system design"
excerpt: "<p>Part of Attitude dynamics and control system coursework @Polimi<br/>
<strong>Dec 2019 to Feb 2020</strong><br/>
(PHOTO: @ESA)<br/>
<img src='/images/In-Orbit_Servicing_Target_inspection.png' width='200' height='150' alt='In-Orbit Servicing Target Inspection'>
</p>
"
collection: projects
category: "SDC"
# permalink: /projects/current/
---

# Cubesat Attitude Control System

This project is part of the **Attitude Dynamics and Control** coursework at Polimi. In this project, a cubesat attitude control system has been designed to meet specific mission requirements using the given sensors and actuators. Below, you will find information about the mission requirements and pre-defined parameters.

<img src="/images/AOCS_requirement.png" alt="AOCS Mission requirements" />
*Figure 1: Mission Requirements and Parameters*

## Modeling

For the modeling, rigid body attitude dynamics with simplified environment, sensors, and actuators models were used.

<img src="/images/AOCS_2.png" alt="Attitude dynamics and control system" />
*Figure 2: Overview of the Modeling Approach*

## Control Design

Lyapunov direct method was employed to derive the control law for both detumbling and tracking phases. The control law was demonstrated to be asymptotically stable even in the presence of disturbances. A simple complementary filter was used as an observer to estimate the state of the system.

![Control Design](path/to/dummy_image3.png)  
*Figure 3: Control Design using Lyapunov Direct Method*

The control parameters were tuned according to the mission requirements.

The entire simulation was carried out using Matlab and Simulink.

## Keywords

- Attitude Control System
- Rigid Body Dynamics
- Lyapunov Direct Method
- Control System Design
- Modeling and Simulation




