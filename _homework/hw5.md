---
layout: archive
collection: homework
title: "Homework 5 - Due Friday, October 4 at 4:30pm"
permalink: /homework/hw5/
author_profile: true
---
[Link to Slack team -- a great place to ask questions](https://ph410f19.slack.com)

**Note: This is the last homework and week of classes prior to our first exam. Your homework this week thus should also include some reflection on and practice with the ideas and goals we've had so far in this course. Begin thinking about the sorts of problems we've been solving, what the big picture of these few weeks has been, and where you personally are at with your mastery of these ideas.**

Homework 5 emphasizes the conductor problem, which requires new methods to approach finding $V$ or $E$ as we are often unable to find $\rho$ a priori. In the presense of an external electric field, charges will shift in a conductor, thus complicating matters of finding $\rho$. This homework will also begin to introduce practice thinking about the Laplace equation.

### 1. Estimation

Estimate the maximum charge you can put onto a child’s balloon.  Given that, what is the associated maximum voltage of the balloon (with respect to infinity)?  Like last week, estimation problems give you a lot of freedom. How big is a balloon? Why should there be a maximum at all? That's key: if the balloon **sparks** (i.e., if a current flows away from it), it can bear no more charge.  Though you *could* make this estimate purely from basic physics, I'll suggest that, to make this easier, you should [google one fact about air](https://www.google.com/search?q=breakdown+electric+field+air). Your answer can be *very* rough, I only want an order of magnitude -- but it should be right to an order of magnitude.  

### 2. A Spherical Capacitor?
Griffiths (at the end of Chapter 2, Example 2.12) finds the capacitance of two concentric spherical metal shells.

1. By letting the radius of the outer shell go to infinity, you get a finite result, called "the capacitance of the sphere." It tells you the charge needed on a sphere to get the surface up to voltage $V$ with respect to infinity. Use Griffiths's result to obtain an expression for the "capacitance of a sphere." 
2. Estimate the capacitance of an isolated human body and give your answers in Farads. We're approximating here, and I'm an astronomer, so we approximate more aggressively than most. Humans are pretty much spheres when I squint. These estimates should give you a sense of how big a one Farad capacitance is.
3. By shuffling over a carpet on a dry winter day, you can easily charge yourself up to a high voltage.  Estimate this voltage by thinking about the length of the spark when your hand comes close to a grounded conductor (like a doorknob). Use your capacitance (part b) to estimate the energy dissipated when you touch a doorknob (or a family member that you dislike) and spark. Is it a lot, or a little?  (Hints: The basic definition of voltage (Equation 2.21 in Griffiths) suggests that over short distances, $\Delta V\sim E\Delta x$, right? And you learned something about air in Problem 1, right?)
4. Try to estimate the radius of Earth based on common knowledge, without looking up anything at all or using a computer or calculator. I did this verbally with one member of our class the other day (a basketball player), so one approach already exists out in the wild. You can actually get this number *incredibly* accurately from common knowlege (doing it verbally the other day, I didn't just get to within an order of magnitude -- I got to within 1% of the true value). See if you can come up with a cool way to estimate it.
5. Estimate the capacitance of planet Earth.
6. Planet earth has a static E field at sea level of $\sim 100~\rm V/m$. Use this to estimate the net charge on the earth, and then the total stored energy our "planetary capacitor" holds. If we could tap this, could it solve all our energy problems (you can google something here, if you want)? (An aside: It turns out that the role of lightning in this story may surprise you, lightning is not *discharging* the giant earth capacitor...[it's actually the *charging* mechanism.](https://en.wikipedia.org/wiki/Atmospheric_electricity)) 


### 3. An Energy Conundrum

There's a bit of a conundrum that occurs when we begin to compare our two different descriptions of energy associated with electrostatic systems. In this problem, you will compare these descriptions and develop an argument that resolves the conundrum.

Consider two point charges ($q_1$ and $q_2$) that are brought to be a distance $r$ apart. You can locate them anywhere to develop this argument, but for the sake clarity, let's put them on the $x$-axis straddling the origin (i.e., one at $r/2$ and the other at $-r/2$).

1. First, compute the work done to bring the charge configuration together. Recall that it costs nothing (i.e., there's no work done) to bring the first charge to it's location. Does this expression look familiar?
2. Now, construct the integral expression for the total energy associated with the charge configuration using the integral formalism: $\frac{\varepsilon_0}{2} \int E^2 d\tau$. Remember that the electric field in this integral expression is due to the field from both charges: $\mathbf{E} = \mathbf{E}_1 + \mathbf{E}_2$. *Do not actually try to integrate it -- that is not required.*
3. Your integral expression can be expanded out to three terms: in principle, you can integrate one of the terms, but not the other two. Which two can't you integrate and why not?
4. What is the physical significance of the two un-integrable terms? What must the integrable term be?


### 4. Gauss's Law and Conductors

A **metal** sphere of radius $R$, carrying a charge $+q$, is surrounded by a thick concentric **metal** shell (inner radius $a$, outer radius $b$). The shell carries no net charge. Where requested, please explain your reasoning.

![Concentric Spheres](../../images/hw5-concentric_spheres.png "Concentric Spheres")

1. Sketch the charge distribution everywhere. If the charge is zero anywhere, indicate that explicitly.
2. From part 1, you probably noticed the charge distributes in some way on the metals. Determine the surface charge density $\sigma$ at $R$, at $a$, and at $b$.
3. Sketch the electric field everywhere; explain how you know the field you have drawn is correct. If the field is zero anywhere, indicate that explicitly.
4. Find the potential everywhere, use $r \rightarrow \infty$ as your reference point for $V=0$.
5. Now the outer surface is touched by a grounding wire, which lowers its potential to zero. How do your answers change to parts 2 and 4? Explain your reasoning.

### 5. Coaxial Capacitors

Consider a coaxial cable with an inner conducting cylinder has radius $a$ and the outer conducting cylindrical shell has inner radius $b$. It is physically easy to set up any fixed potential difference $\Delta V$ between the inner and outer conductors. In practice, the cable is always electrically neutral.

1. Assuming charge per length $+\lambda$ and $-\lambda$ on the inner and outer cylinders, derive a formula for the voltage difference $\Delta V$ between the cylinders.
2. Assuming infinitely long cylinders, find the **energy stored per length (W/L)** inside this capacitor. Notice I am asking for the energy per unit length, the answer is *not* infinity.  Let's do it two ways so we can check:
* Find the capacitance per length ($C/L$) of this system, and then use stored energy $W = \frac{1}{2} C (\Delta V)^2$.
* Integrate the energy density stored in the E field.
3. Based on your answers to part 2, where in space would you say this energy is physically stored?
4. Estimate the capacitance per meter of the coaxial cable that the cable company uses to send TV signals into homes. Justify any assumptions.
5. This model is also excellent for "axons", which are long cylindrical cells (basically coax cables) carrying nerve impulses in your body and brain.  Estimate the capacitance (in SI metric units, Farads) of your sciatic nerve. *Suggested assumptions: The sciatic nerve is the longest in your body, it has a diameter of roughly 1 micron, and a length of perhaps 1 m. Note that axons generally have a value of $b$ which is very close to $a$ (i.e. the gap is extremely tiny, $b-a$ is about 1 nanometer). An approximation of a logarithm of the form $ln(1+\epsilon)$ where $\epsilon$ is some very small number should be helpful.*


### 6. Superposition in Conductors ("shielding")

Suppose we carve out two spherical cavities from a metal sphere of radius $R$ (as shown below). The first cavity (radius, $a$) has a charge $+q_a$ placed at the center of the cavity. Similarly, the second cavity (radius, $b$) has a charge $+q_b$ placed at the center of that cavity.

![Shielded Charges](../../images/hw5-shielded_charges.png "Shielded Charges")


1. Sketch the surface charge everywhere. Explain how you know the surface charge looks this way.
2. Determine the surface charges ($\sigma_a$, $\sigma_b$, and $\sigma_R$).
3. Sketch the electric field everywhere. If the field is zero anywhere, indicate this explicitly. Explain how you know the electric field looks this way.
4. Determine the magnitude of electric field outside the conductor and inside each cavity.
5. If we brought an external charge $q_c$ near the conducting sphere how do your answers to parts 1-4 change? You may answer in words, pictures or both.


### 7. Proving Uniqueness

For this homework problem, you will prove the "second uniqueness theorem" yourself, using a slightly different method than what Griffiths does (though you may find some common ideas are involved). It will really help to review/read the section on the second uniqueness theorem as you work through this problem. On the first two homeworks, I was quite forgiving of imprecision and lack of clarity in vector proofs; I will now expect completely clear and rigorous logic.

**Do it like this:**

1. Use the divergence theorem and Product Rule 5 to prove Green's Identity: 
   
   $$\int_V \left(T \nabla^2 U + \nabla T \cdot \nabla U\right) d\tau = \oint_S \left(T \nabla U\right)\cdot d\mathbf{A}.$$ 

   (Hint: Let $\mathbf{v}=T\nabla U$ in the divergence theorem. This is Griffiths Problem 1.61 part c.)

2.  Now prove the second uniqueness theorem. Green's Identity is true for **any** choice of $T$ and $U$, so let the functions $T$ and $U$ in that identity both be the **same** function. Specifically, you should set them both equal to $V_3=V_1-V_2$ where $V_1$ and $V_2$ represent *different* solutions to the same boundary value problem ($\nabla^2 V = 0$ with boundary conditions). Then, using Green's Identity (along with some arguments about what happens at the boundaries, rather like Griffiths uses in his proof) should let you  show that $E_3$, which is defined to be the negative gradient of $V_3$ (as usual), must vanish everywhere throughout the volume.  That will complete the proof

Work to understand the game, here: the goal, the strategy, and the result. We are checking if there are two different potential functions, $V_1$ and $V_2$, each of which satisfies Laplace's equation throughout the region we're considering. You construct (define) $V_3$ to be the difference of these, and you prove that $V_3$ (or in this case, $\mathbf{E}_3$) must vanish everywhere in the region. This means there really is only one unique E-field throughout the region after all.  This is a rather *formal manipulation* type of problem, giving you a chance to practice with the divergence theorem and think about what boundary conditions really mean.

### 8. The Method of Images -- The corner problem 

In this problem, it may or may not help you to work on the two parts simultaneously or out of order. The second part is just a tool for visualizing the first part.

![images Charges](../../images/hw5-images.png "image Charges")

1. Obtain a formula for the voltage $V(x,y,z)$ arising from a single point charge $+q$ located symmetrically a distance a from the inside corner formed by bending an infinite, grounded metal sheet through a right angle. (Hint: You'll need more than one "image" charge.) 

2. The hardest thing about coming up with these "image" solutions is having a good intuition for what fields and potentials look like in different scenarios. Use the [PhET simulation *Charges and Fields*](http://phet.colorado.edu/en/simulation/charges-and-fields) to visualize your resulting E-field and some relevant equipotential contours (these can be added as green curves by using a tool on the right side of the simulation). Clearly illustrate how your images solve this problem. Take a screen shot and include it, with a few comments, to explain what you learned in this problem. 

