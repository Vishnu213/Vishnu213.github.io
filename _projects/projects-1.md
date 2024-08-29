---
title: "Autonomous spacecraft Inspection mission"
excerpt: "<p>Master thesis at Politecnico di Milano<br/>
<strong>June 2020 to April 2021</strong><br/>
(PHOTO: @ESA)<br/>
<img src='/images/In-Orbit_Servicing_Target_inspection.png' width='200' height='150' alt='In-Orbit Servicing Target Inspection'>
</p>
"
collection: projects
category: "GNC"
tags:
  - Inspection mission
  - Proximity operation
  - On-orbit servicing mission
  - Autonomous guidance
  - Relative motion
  - Motion planning algorithm
# permalink: /projects/past/
---
<br/>
## Spacecraft Inspection mission

Spacecraft inspection is a critical phase in various on-orbit servicing (OOS) missions, which are increasingly important as the commercial space sector continues to grow. These missions are essential for maintaining, repairing, and extending the life of satellites and other spacecraft, particularly those in geostationary orbit, where the space available is limited and highly valuable. By performing inspections, spacecraft can gather crucial data about the physical state of a target object, including its position, orientation, and operational status. This information is vital for subsequent operations like refueling, repair, or repositioning, making the inspection problem a foundational element of successful OOS missions.

<div style="text-align: center;">
    <img src="/images/PROXIMITY.png" alt="Proximity Operation Scenarios" style="width:50%; height:auto;">
    <img src="/images/OSS_DEMO.png" alt="On-Orbit Servicing Missions" style="width:50%; height:auto;">
</div>


## Objective and Approach of the Thesis

The thesis addresses the spacecraft inspection problem by developing a novel framework for autonomous guidance for cubesat sized spacecraft equipped with low thrust propulsion system. The primary goal was to create a methodology that can efficiently generate both translation and rotational trajectories to ensure maximum coverage of the target object during the inspection phase.

To tackle the problem, the thesis adopts Sample Based Motion Planning (SBMP) algorithms due to their flexibility and ability to handle complex, constrained environments with reduced computational costs. The methodology is built around the Fast Marching Tree* (FMT*) algorithm, with significant adaptations to address the specific challenges of spacecraft inspection missions. This includes coupling the translation and attitude control to produce a holistic guidance solution.


## Methodology

The methodology developed in the thesis is known as the Autonomous Motion Planning Spacecraft Guidance for Inspection Mission (AMPSGIM) framework. This framework integrates SBMP algorithms to generate feasible paths that ensure good coverage of the target object while minimizing fuel consumption and control torque.

1. **System Dynamics:** The thesis begins by modeling the relative dynamics of spacecraft, both in terms of translation and rotational motion. The framework considers these dynamics when generating the guidance law.

2. **Algorithm Adaptations:** The Fast Marching Tree* (FMT*) algorithm was adapted for the inspection mission. These adaptations involved incorporating constraints specific to spacecraft operations, such as collision avoidance and control feasibility.

3. **Simulation Scenarios:** The framework was tested through various numerical simulations involving single and multiple spacecraft inspecting targets of different sizes. These simulations demonstrated the framework's ability to efficiently solve the inspection problem while adhering to mission constraints.

## Application and Further Developments

The AMPSGIM framework was applied to different simulation scenarios with various target sizes, it succeeded in producing the coupled guidance for both single and multiple spacecraft systems. Following figures shows the trajectory around the target body. In both the figures, the dark line indicates thrusting trajectory and the light line shows the coasting/non-thrusting trajectory.

<div style="text-align: center;">
    <img src="/images/one_sat_case.png" alt="Single Spacecraft inspection trajectory" style="width:50%; height:auto;">
</div>

In the two spacecraft situation (as shown below), the constraints such as collision avoidance, pointing avoidance were considered along with typical constraints on the thrust magnitude, attitude actuator magnitude.

<div style="text-align: center;">
    <img src="/images/two_sate_case.png" alt="Two Spacecraft inspection trajectories" style="width:50%; height:auto;">
</div>

## Limitation and Future work

The framework has certain limitations, such as the assumption of readily available spacecraft's state and the exclusion of disturbances in the dynamics along with assumption of coasting and non-coasting arcs simplified the approach to obtain translation and rotational motion explicit coupling via Guidance frame instead of considering them implicitly coupled rotational and translation dynamics.

Future work could focus on improving the robustness of the framework by incorporating disturbance modeling and state estimation techniques. Further analysis has to be carried out to make the framework feasible in terms of computational time, making it applicable to practical settings.

For more detailed information, please check out [my thesis](https://www.politesi.polimi.it/retrieve/1d539c29-5b5c-4911-ab7c-8f07ce1b2f58/2021_07_Shakthibala.pdf){:target="_blank"}.
