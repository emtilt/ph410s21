---
layout: archive
collection: homework
title: "Homework 2 - Due Friday, September 13 at 4:30pm"
permalink: /homework/hw2/
author_profile: true
---

[Link to Slack team -- a great place to ask questions](https://ph410f19.slack.com)

Homework 2 emphasizes the electric field and the principle of superposition that will form the basis of much of your understanding of electrostatics. This homework makes use of what you learned from Secs. 1.1-1.4 in Griffiths and adds to it the concepts from Sec. 2.1, which make up the bulk of the assignment. In addition, we have begun to introduce the idea of finding approximate formulae using Taylor expansions, which is one of the most common practices of theoretical physics. In this assignment, you will use a Jupyter notebook to determine an electric field as we build up the architecture to solve electric field problems numerically.

### 1. Finding the angle between two suspended charges

When working through some physics, you will typically find yourself in a situation where a strict analytical solution to your problem evades you because the models that you have used have sophisticated algebraic forms that lead to transcendental equations, non-integrable forms, or other problematic situations. In these situations, it is often instructive to step back a moment and consider under what conditions you want to solve your problem. Those conditions might provide you with reasonable limitations and assumptions that lead to approximate forms that get you very close to what you need. In this problem, which has a familiar context from Physics 2, I will give you the assumption to make. But in future problems, you might have to decide for yourself: *What assumptions and approximations can I make here and why?*

Two charges of identical mass $m$, one with charge $q$ and the other with charge $4q$, hang from strings of length $l$ from a common point. Assume that $q$ is sufficiently small that the electric force on each mass is quite small compared to the gravitational force on each.

1. Find an approximate expression for the angle $\theta$ that each charge makes with respect to the vertical. (Hint: what variable is necessarily very small?)
2. Describe how this assumption of the relationship between the forces (i.e., that the electric force is small compared to the gravitational force) played out in your calculation. Which quantities were approximated and why?
3. Check (i.e., explcitly show) that the units of your solution work out.
4. Show that the limiting behavior for large masses ($m$), large length ($l$), and small charge ($q$) are physically reasonable and match your expectations.

### 2. A curious distribution of charge

In this problem, you will explore numerical integration in the context of an analytically intractable charge distribution. You can [download the notebook](../../jupyter/HW2-loopsandintegration.ipynb) (or [view it here](https://github.com/emtilt/ph410f19/blob/master/jupyter/HW2-loopsandintegration.ipynb)).

### 3. Numerically calculating the electric field

In this problem, we will lay the ground work for determining the electric field of a distribution of charge numerically. We won't actually attempt an integral this time, but instead we will lay the groundwork for how to think about them and how to set them up in Python.

You will do this work in a Jupyter notebook. You can [download the notebook](../../jupyter/hw2-electricfield.ipynb) (or [view it here](https://github.com/emtilt/ph410f19/blob/master/jupyter/hw2-electricfield.ipynb)). 

### 4. Disk of charge - Checking new results against your intuition

In this class, you will often produce new formulae that describe some situation for which you might not have developed intuition yet. One question you should always be asking yourself is: *Why do I believe the physics/math that I've just done?* In this problem, you will develop some techniques for checking your results against the intuition that you already hold.

Consider a thin disk of radius $R$ with a uniform charge density, $-\sigma$.

![Disk of Charge](../../images/hw2-diskofcharge.png "Disk of Charge")

This may seem like a very artificial problem, but the disk of charge is an idealization of many physical devices: a capacitor plate, a small patch of any surface, etc. Once you have solved this ideal problem, you will be able to apply it to realistic situations.

1. Find the electric field at point P, which is a distance $z$ above the center of the disk, by integrating across the surface of the disk. [Hint: One way of doing this is by realizing that a disk is just a bunch of concentric rings of charge $dq$.] (This electric field is well-known (you could easily Google the answer), but the practice of setting up and doing these kinds of integrals is important. The functional form of your solution will be bit complicated, and it might be tough to tell on first glance if it is correct. You can certainly look up the answer to check it, but you won't always be able to do that in this class (and in life). So instead, try calculating it without reference to external resources, and then check your result against your intuition with the steps below.)
2. If you were very far from this disk, what would you expect the field to look like? Use your intuition from Physics 2, and explain. Then explicitly check the limiting form of your solution at very large $z$ (i.e., when $z \gg R$). By "limiting form", I mean for you to determine how it behaves as a function of distance within this limit. Your answer should not simply be, "it goes to zero" (if that's what you expect). Instead, determine how, functionally, it behaves in that limit (like $1/z$? like $e^{-z}$? Something else?). (Hint: Maybe there is a useful Taylor series approximation?)
3. If you were very close to the disk, what would expect the field too look like? Again, use your intuition from Physics 2 to explain. Explicitly check the limiting form of your solution at very small $z$ (i.e., when $z \ll R$).
4. Sketch a qualitatively correct graph of the component of the electric field in the $z$-direction along the center line. Be sure to include both the positive and negative $z$-axis in your graph. Your answers to parts 2 and 3 might help you here.


### 5. Checking your answers

Suppose you've just spent an hour calculating the magnitude of the electric field of a charged ring of radius $R$ that holds a uniform linear charge density $\lambda$ at a distance $z$ from the center of the ring. You ended up with the result:

$E = \dfrac{1}{4\pi\varepsilon_0}\dfrac{\lambda 2\pi Rz}{(z^2+R^2)^{3/2}}$

1. Check the units of this expression to verify it is correct.
2. What are at least two other indepdent checks that you could do to see if you believe your result?
3. Perform those two independent checks. Comment on if you believe this result based on these checks. Why or why not?

### 6. Quick questions based on symmetrical reasoning
 Deduce answers to the following questions, explaining your reasoning clearly and rigorously. You should not need to do significant mathematical work to answer these if you carefully consider the symmetries of the scenario. (This is quite similar to Griffiths Problem 2.1. I strongly encourage you to reason this out alone, without recourse to solutions by others from the internet. It's not a long problem.)
 
- Consider eight positive charges of magntiude $q$ arranged symmetrically around the circumference of a circle of radius $r$. 
  1. What is the magnitude of the electric field at the center of the circle?
  2. What is the magnitude of the electric field at the center of the circle if one charge is removed? 
- Now consider nine positive charges of magntiude $q$ arranged symmetrically around the circumference of a circle of radius $r$.
  1. What is the magnitude of the electric field at the center of the circle?
  2. What is the magnitude of the electric field at the center of the circle if one charge is removed? 
