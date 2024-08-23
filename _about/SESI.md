---
title: "System Identification and State estimation of an UAV"
excerpt: "<p>This project is part of Estimation in Aerospace coursework taught by prof. Marco Lovera  at Polimi.<br/>
<strong>Dec 2019 to Feb 2020</strong><br/>
(PHOTO: @ESA)<br/>
<img src='/images/In-Orbit_Servicing_Target_inspection.png' width='200' height='150' alt='In-Orbit Servicing Target Inspection'>
</p>
"
collection: projects
category: "SDC"
tags:
  - System Identification
  - State estimation
  - Grey box model
  - Cramer Rao bound
  - Output error method
# permalink: /projects/current/
---

## System Identification:

Models that we use in our application sometimes are assumed to be available to us, but in reality, every dynamic model parameter, if not for the simple cases, has to be estimated via empirical methods. For example, the exact inertia of the satellite or helicopter has to be estimated empirically. Given the importance of finding the parameters of the dynamic model, in this project a well known method called output error method is applied. The dynamic model considered was the lateral dynamic model (greybox model) of the drone that is inherently unstable, due to this reason, frequency based output error method is utilized. I know, I right-away using the term “output error method” as if everyone in this world knows about it. Actually, it simply fits a model that minimizes the error between the actual output and model’s output. In matlab, you can use the “greyest“ function to use the OE method for grey box models. 

After estimating the model using the greyest function, we validated the model with experiment data. With Monte Carlo simulation, we were able to see that within the fixed variance of the estimated parameters, we were able to observe that the system was stable. 

## State estimation

With the estimated model. We wanted to estimate the lateral velocity using the measurements coming from an inertial sensor. With the Kalman filter both custom implemented and matlab versions are applied to the problem and validated with real data.

For more information please consult this presentation.
