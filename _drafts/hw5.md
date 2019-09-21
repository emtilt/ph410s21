---
layout: archive
collection: homework
title: "Homework 5 - Due Friday, September ?? at 4:30pm"
permalink: /homework/hw5/
author_profile: true
---
[Link to Slack team -- a great place to ask questions](https://ph410f19.slack.com)


#### 1.  Ring of charge - Motion of a test charge

While we spend a large amount of time working with source charges and the electric fields that they produce, we are ultimately concerned about their effect on the motion of other charges (so-called "test charges"). In this problem, you will work with the electric field due to a ring of charge to develop an approximate solution for the motion of a test charge by "linearizing" the differential equation that describes the motion. In working this problem, you will have to dust off some of your classical mechanics knowledge regarding differential equations.

Consider a thin ring (positive charge, $Q$; radius, $a$) that has its central axis directed along the $x$-direction as shown.

![Ring of charge](../../images/hw4-ring_w_charge.png "Ring of Charge")

A charged ring with these parameters will produce an electric field along its central axis given by,

$$E_x = \dfrac{1}{4\pi\varepsilon_0}\dfrac{Qx}{\left(x^2+a^2\right)^{3/2}}$$

1. Write down the differential equation that describes the motion of a particle with negative charge $-q$ and mass $m$ that is carefully positioned on the $x$-axis. *Note: this particle has a charge that is opposite the sign of the ring, so $q$ is the magnitude of the charge of this particle.*
2. What kind of motion do you expect to see for this charge? Why? Does the differential equation describe that kind of motion? *Hint: Consider if this differential equation is analytically tractable (i.e., can it be solved in closed form).*
3. Consider the situation where the particle is very close to a large ring (i.e., where $x/a$<<$1$). Determine the approximate form of the differential equation for this case -- keep only terms that depend linearly on $x$. This is called "linearizing" the differential equation and makes the solution analytically tractable.
4. Solve the differential equation for the case where the particle starts from rest at a distance of $x_0$ from the ring. Sketch the resulting motion of the test charge as a function of time. Does your graph agree with your intuition about the motion?
5. What would happen to the test charge if it was not placed precisely on the central axis? Why?
6. (Turn in using DropBox) We have created a Jupyter notebook that begins to model the motion of the test charge using both the exact and the approximate differential equation. You can [download it here](../jupyter/HW4-MotionOfTestCharge.ipynb) (or [view it here](https://github.com/dannycab/phy481msu_f2019/blob/master/jupyter/HW4-MotionOfTestCharge.ipynb)). By working through this notebook, we expect you to complete the model and be able to explain the output of each model and its assumptions. We also ask that you determine under what conditions the approximate model is a good one and explain how you know.
7. (Turn in using DropBox) **BONUS:** Break up the ring into small chunks, so that you can determine the electric field at any point. Model the motion of the charged particle **in general** in the presence of this charged ring. Can you get any interesting or cool trajectories? How would you plot this in 3D? *This BONUS is worth 15 points (about one full problem).*
