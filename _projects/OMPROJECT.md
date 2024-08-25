---
title: "Preliminary Interplanetary trajectory optimization"
excerpt: "<p>This project is part of Estimation in Aerospace coursework taught by prof. Marco Lovera  at Polimi.<br/>
<strong>Dec 2019 to Feb 2020</strong><br/>
(PHOTO: @ESA)<br/>
<img src='/images/In-Orbit_Servicing_Target_inspection.png' width='200' height='150' alt='In-Orbit Servicing Target Inspection'>
</p>
"
collection: projects
category: "SDC"
tags:
  - Orbital mechanics
  - Delta V optimization
  - Interplanetary trajectory optimization
  - Impulse manuever
  - Gauss planetary equations
# permalink: /projects/current/
---

This project had two tasks. First task involves finding a **optimal trajectory** using impulsive manuever to go from Mars to Mercury via gravity assist around Earth for scientific mission. Second task is a orbital analysis of a MEO orbit in the presence of Earth oblateness and Moon gravitational effects.  

## Trajectory optimizatiion:

A patched conic approach was used to model the interplanetary trajectory optimization problem. There are three Delta_V that are present, first manauver is at the departure point (Mars), another one is corrective manauver to support gravity assist at Earth and last one is at Mercury. Porkshop plots were used as the main tool to find the optimal Delta_V manuver for the given timeslot. An example porkchop plot is shown in the figure below, it is a 3-D plot with DEPARTURE, FLYBY, ARRIVAL times on its axis.
<img src="/images/pork_chop_1.png" alt="Pork Chop plot" />
*Figure 1: Scattered PorkChop plot*

To find the best possible Delta_V combination, a simple **triple for loop** is used to find the minimal overal Delta_V. Before going for the triple for loop, 12 year period was pruned via trail and error to find out the timeslot that at the first-go gives the indication of possible optimal trajectory. After selecting the time slot, triple for loop is run with smaller time discretization points along with the genetic algorithm to obtain the refined trajectory. 

The final interplanetary trajectory is shown in the figure below:

<img src="/images/Interplanetary_trajectory.png" alt="Interplanetary_trajectory.png" />
*Figure 2: Best Delta_V Interplanetary trajectory*



## Perturbation analysis:
Prelimary Orbital analysis was conducted with Earth oblateness and Moon third body perturbations. The orbit considered was a MEO orbit that experiences perturbation from both Earth oblateness and Moon gravitation force. Guass plantary equation and carterian equation of motion is used to simulate the orbit. 