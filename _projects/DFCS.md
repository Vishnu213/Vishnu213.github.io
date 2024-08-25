---
title: "Drag free orbital control system "
excerpt: "<p>Part of Attitude dynamics and control system coursework @Polimi<br/>
<strong>Dec 2019 to Feb 2020</strong><br/>
(PHOTO: @ESA)<br/>
<img src='/images/GOCE_pillars.jpg' width='200' height='150' alt='In-Orbit Servicing Target Inspection'>
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

Following are the important modeling steps involved.
- Orbitam dynamics via Gauss planetaryu equations with J2 + aerodynamics forces
- Gravity gradiometer, which is basically an accelerometer as shown in the figure below:

  <div style="text-align: center; margin-top: 10px;">
    <img src="/images/GOCE_accelorometer.png" alt="Gravity Gradiometer" style="max-width: 100%; height: auto;">
    <p><strong>Figure 1: Gravity Gradiometer (Accelerometer)</strong></p>
  </div>

- Next, we have the solenoid valve system that controls the fuel valve:

  <div style="text-align: center; margin-top: 10px;">
    <img src="/images/GOCE_solenoid_valve.png" alt="Solenoid Valve System" style="max-width: 100%; height: auto;">
    <p><strong>Figure 2: Solenoid Valve System</strong></p>
  </div>

With different dynamics systems combined together, we end up with 13 first order differential equation system. A block diagram representation is shown below. 
  <div style="text-align: center; margin-top: 10px;">
    <img src="/images/GOCE_BLOCK.png" alt="Goce block diagram" style="max-width: 100%; height: auto;">
    <p><strong>Figure 3: Goce dynamics system block diagram</strong></p>
  </div>
With the modeling part done, we next look at how we can simulate it.

One of the interesting things about this project is the fact that we were able to understand the characteristics of different simulation integrators on Matlab, ode45, ode113, ode23s, ode115. For the dynamics that you saw above,  the gravimetry system has higher frequency dynamics while the orbital mechanics has lower frequency, this makes the system highly stiff, with this in mind, ode115 was chosen to simulate the system. 

Various tuning parameters for the classical controller present in the circuit were tuned according to the simulation results. You can read more in this short and [concise report](https://drive.google.com/file/d/1IEg0pgLE8COlaYaMVE8NSF560V4Mlp_t/view?usp=sharing){:target="_blank"}. 






