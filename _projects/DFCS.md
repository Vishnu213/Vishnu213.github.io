---
title: "Drag free orbital control system "
excerpt: "<p>Part of Attitude dynamics and control system coursework @Polimi<br/>
<strong>Dec 2019 to Feb 2020</strong><br/>
(PHOTO: @ESA)<br/>
<img src='/images/In-Orbit_Servicing_Target_inspection.png' width='200' height='150' alt='In-Orbit Servicing Target Inspection'>
</p>
"
collection: projects
category: "SDC"
tags:
  - Gauss planetary equations
  - Orbital mechanics
  - Numerical integration
  - Numerical stability
  - Taylor series
  - Sensitivity analysis
  - Spacecraft modeling and simulation
  - Control system
# permalink: /projects/current/
---

This project is part of Modeling and Simulation coursework at Polimi.
Project aims to model and simulate single uni-directional drag control of the GOCE spacecraft. Essentially the spacecraft was tasked to measure the gravity at very high accurate scales, this requires negation of drag forces experienced by the spacecraft in its orbit. 

You will see below the different dynamics systems modeled. The physical controller is the valve diameter, we control this to control the flow of fuel to the electric thruster. By doing so, we are able to compensate for aerodynamic drag.


One of the interesting things about this project is the fact, we were able to understand the characteristics of different simulation integrators on Matlab, ode45, ode113, ode23s, ode115. For the dynamics that you saw above,  the gravimetry system has higher frequency dynamics while the orbital mechanics has lower frequency, this makes the system highly stiff, with this in mind, ode115 was chosen to simulate the system. 

Various tuning parameters for the classical controller present in the circuit were tuned according to the simulation results. You can read more in this short and concise report. 






