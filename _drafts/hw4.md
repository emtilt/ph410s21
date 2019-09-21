---
layout: archive
collection: homework
title: "Homework 4 - Due Friday, September 27 at 4:30pm"
permalink: /homework/hw4/
author_profile: true
---
[Link to Slack team -- a great place to ask questions](https://ph410f19.slack.com)

Homework 4 emphasizes another alternative method to direct integration for solving the electric field problem by reducing the vector problem to a scalar one by using electric potential. In addition, it introduces the electric potential energy concept. This homework emphasizes 2.3 and 2.4, but Sec. 2.2 (Gauss’ Law) continues to be very important.


### 1. Overlapping clouds of charge

When solving some E&M problems, you will need to develop your solution using an arbitrary location. In this problem, consider how choosing an arbitrary point in the overlapping region of the charge clouds will help you derive the result.

![Overlapping Clouds](../../images/hw4-overlapping_clouds.png "Overlapping Clouds")
1. Consider two oppositely charged clouds (radii, $R$), both with known uniform charge densities. They overlap as in the figure, with their centers separated by $d$. Find the electric field in the overlapping region. (*Hint: Consider how Gauss' Law and superposition can help here. You should already know how to find the field inside each sphere separately -- is there a way to use that knowledge?*)
2. In this overlapping region, sketch the electric field lines.
3. In the limit that $d$ becomes very small compared to $R$, discuss in words and make a sketch of what the resulting (total, physical) charge distribution in space really looks like. Is this similar in any way to the physical situation in some other system that you have studied before? (So that later in the course when we encounter such a charge distribution, we will know where it came from and what the electric field looks like inside!)

### 2. Allowed Fields
1. If $c$ is a constant, which one of the following two static E-fields is physically impossible. Why?
  -  $\mathbf{E}=c\left(x\hat{x}+z\hat{z}+y\hat{z} \right)$
  -  $\mathbf{E}=c\left(x\hat{x}+2z\hat{z}+y\hat{z} \right)$
2. For the field that **is** possible, find the potential $V(\vec{r})$, using the origin as your reference point (i.e., setting $V(0)=0$). (Hint: You must select a specific path to integrate along. It doesn't matter which path you choose, since the answer is path-independent, but you can't compute a line integral without having a particular path in mind, so be explicit about that in your solution.)
3. Check your answer two ways: by explicitly computing the gradient of V and by checking that it gives the correct result at a particular point for which you already know the potential. 


### 3. Connecting potential, electric field, and charge

It is common in theoretical physics to describe the interactions of a system in terms of a scalar field (i.e., its potential). It is a compact description and you can (if you are careful) derive other important aspects of the system (e.g., how its sources are configured) from that scalar field if there is a rule for doing so. In this problem, you will do this work for a negative point charge. The understanding you draw from this problem will be used in future problems where the electric field and charge density might not be obvious.

Consider the potential of a point charge at the origin:

$$V(r) = -\dfrac{1}{4\pi\varepsilon_0}\dfrac{q}{r}$$

1. Determine the electric field of this charge by calculating the gradient ($\mathbf{E} = -\nabla V$). Show your work.
2. Calculate the charge density from the electric field by using Gauss' Law directly ($\nabla \cdot \mathbf{E} = \frac{\rho}{\varepsilon_0}$). Do this 2 ways: (1) Use the definition of the divergence from the front fly leaf of Griffiths in spherical coordinates (what do you get?) and (2) by performing a coordinate-free calculation (is your answer the same?).
3. How do your two answers from part 2 compare? Which one is correct? How do you know? What does this tell you about computing charge densities from electric potentials?

For part 2, the following vector identities might be helpful:

$$\nabla \cdot \left(f(\mathbf{r}) \mathbf{A}\right) = \nabla f(\mathbf{r}) \cdot \mathbf{A} + f(\mathbf{r}) \nabla \cdot \mathbf{A}$$

$$\nabla \cdot \dfrac{\hat{r}}{r^2} = 4\pi\delta^3(\mathbf{r})$$

$$\nabla \cdot \dfrac{\hat{r}}{r} = \dfrac{1}{r^2}$$



### 5. Finding voltage from a charge distribution

We have found a number of ways of relating $\rho$, $\mathbf{E}$, and $V$. In this problem, you will use $\rho$ to find $V$ through the method of direct integration (i.e., using the integral expression for $V$).

1. Find a formula for the electrostatic potential $V(z)$ everywhere along the symmetry-axis of a charged disk (radius $a$, centered on the $z$-axis, with uniform surface charge density $+\sigma$ around the ring).  Please use the method of direct integration to do this, and set your reference point to be $V(\infty)=0$.
2. Sketch $V(z)$, how does $V(z)$ behave as $z \rightarrow \infty$? (Don't just say it goes to zero. How does it go to zero?) Does your answer make physical sense to you? Explain briefly.
3. Use your result from part 1 for $V(0,0,z)$ to find $z$-component of the electric field anywhere along the $z$-axis?
4. What is the voltage at the origin? What is the electric field at the origin? Do these results from $V$ and $\mathbf{E}$ at the origin make physical sense to you, and are they consistent with each other? Briefly explain.

### 6. Energy of a point charge distribution

When studying crystal structures (e.g., in condensed matter physics), it is sometimes convenient to model those structures as rectangular grids of charged ions, this problem offers a starting point for such a model.

Imagine a small square (side $a$) with four point charges $+q$, one on each corner.

1. Calculate the total stored energy of this system (i.e. the amount of work required to assemble it).
2. Calculate how much work it takes to "neutralize" these charges by bringing in one more point charge ($-4q$) from far away and placing it right at the center of this square.


### 1. Screened Coulomb Potential

In a [previous problem](./homework3.html#connecting-potential-electric-field-and-charge), you worked out the electric field and charge distribution for a point charge using the electric potential.  In this problem, you will gain some additional practice doing this for the [screened Coulomb potential](https://en.wikipedia.org/wiki/Electric-field_screening).

Consider the "screened Coulomb potential" of a point charge $q$ that arises, for example, in plasma physics:

$$V(r) = \dfrac{q}{4\pi\varepsilon_0} \dfrac{e^{-r/\lambda}}{r}$$

where $\lambda$ is a constant (called [the screening length](https://en.wikipedia.org/wiki/Debye_length)).

1. Determine the electric field $\mathbf{E}(\mathbf{r})$ associated with this potential.
2. Find the charge distribution $\rho(\mathbf{r})$ that produces this potential. (Think carefully about what happens at the origin!)
3. Sketch this function $\rho(\mathbf{r})$ in a manner that clearly describes its characteristics (i.e., what's the best way of representing this three-dimensional charge distribution? Use it, and explain what you are plotting.)
4. Show, by explicit calculation over $\rho(\mathbf{r})$ that the net charge represented by this distribution is zero. (*If you don't get zero, think again about what happens at $r = 0$.*).
5. Verify this result using the integral form of Gauss' Law (i.e., integrate your electric flux over a *very large* spherical surface.)

### 2. Surface charge and boundary conditions

It might seem to you that the results that the electric field is discontinuous by an amount $\sigma/\varepsilon_0$ isn't really a big deal. There's probably a question about how useful this result is. We will come back to this particularly when we get to fields in matter, and suffice it to say, it will help us a lot there. To get a flavor of what is coming, this problem will discuss this discontinuity in a familiar context.

1. Consider a cylindrical metal rod (radius $r$, length $L$) with a constant charge density $\sigma$ distributed across its outer surface (as we will learn that is the only place the charge can be). Using Gauss' Law (far from the ends of the rod; assume it's long and skinny), determine the electric field inside and outside the rod.
2. Take the difference between the electric fields you determined in Part 1 (technically, the perpendicular component) across the outer surface of the metal rod to show you recover the the result that the all the charge lives on the surface.
3. Consider a similarly cylindrical plastic rod with a constant charge density $\rho$ distributed over its entire volume. Again, using Gauss' Law (far from the ends of the rod; assume it's long and skinny), determine the electric field inside and outside the rod.
4. Again, take the difference between the electric fields you determined in Part 3 across the outer surface of the plastic rod. What do you find? Does your result make physical sense?

### 3. An energy conundrum

There's a bit of a conundrum that occurs when we begin to compare our two different descriptions of energy associated with electrostatic systems. In this problem, you will compare these descriptions and develop an argument that resolves the conundrum.

Consider two point charges ($q_1$ and $q_2$) that are brought to be a distance $r$ apart. You can locate them anywhere to develop this argument, but for the sake clarity, let's put them on the $x$-axis straddling the origin (i.e., one at $r/2$ and the other at $-r/2$).

1. First, compute the work done to bring the charge configuration together. Recall that it costs nothing (i.e., there's no work done) to bring the first charge to it's location. Does this expression look familiar?
2. Now, construct the integral expression for the total energy associated with the charge configuration using the integral formalism: $\frac{\varepsilon_0}{2} \int E^2 d\tau$. Remember that the electric field in this integral expression is due to the field from both charges: $\mathbf{E} = \mathbf{E}_1 + \mathbf{E}_2$. *Do not try to integrate it.*
3. Your integral expression can be expanded out to three terms: in principle, you can integrate one of the terms, but not the other two. Which two can't you integrate and why not?
4. What is the physical significance of the two un-integrable terms? What must the integrable term be?
