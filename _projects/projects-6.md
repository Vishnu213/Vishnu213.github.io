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
tags:
  - ADCS
  - Attitude representation
  - Quaternions
  - Direction cosine matrix
  - Lyaponav direct method
  - Attitude controller
  - Spacecraft attitude dynamics
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

<div style="display: flex; justify-content: space-around; align-items: center;">

  <div style="text-align: center; margin-right: 10px;">
    <img src="/images/detumbling.png.png" alt="Image 1" style="max-width: 100%; height: auto;">
    <p><strong>Figure 3: Detumbling </strong></p>
  </div>

  <div style="text-align: center; margin-left: 10px;">
    <img src="/images/pointing_error.png" alt="Image 2" style="max-width: 100%; height: auto;">
    <p><strong>Figure 4: Tracking pointing error</strong></p>
  </div>

</div>

The control parameters were tuned according to the mission requirements. Figure 3 and 4 shows the detumbling manauever and pointing error results obtained with the controller developed. Specifically in figure 4, the parameters were to such that the pointing error reaches the limit to 2 degree very fast and remain inside the threshold through out the mission. Likewise, for detumbling depending on the availability of time and actuation power, control parameters can be choosed to satisfy the mission requirements.

The entire simulation was carried out using Matlab and Simulink. You can find more details in this [report](https://drive.google.com/file/d/1eL6Sg0PQE51EKPc4YNhUSzYIgh_O2uU6/view?usp=sharing){:target="_blank"}




