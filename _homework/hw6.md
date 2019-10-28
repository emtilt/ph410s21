---
layout: archive
collection: homework
title: "Homework 6 - Due Friday, October 25 at 4:30pm"
permalink: /homework/hw6/
author_profile: true
---
[Link to Slack team -- a great place to ask questions](https://ph410f19.slack.com)

Homework 6 focuses on Laplace’s equations and solving it using infinite series solutions. You should become comfortable with setting boundary conditions for PDE problems like this and develop a sense of the process for solving these problems analytically. Additionaly, you will plot these solutions in 2D and develop the method of relaxation in 1D to investigate issues with the method.


## 1. Potential and electric field with Laplace's equation

In class we derived the solution for the 2D version of Laplace's equation with the boundary conditions shown below.

![Channel](../../images/hw6-channel.png "Channel")

That solution was analytic, but it contained an infinite series:

$$V(x,y) = \sum_{n=1,3,5,\dots}^{\infty} \dfrac{4 V_0}{\pi n} \sin \left(\dfrac{n\pi x}{a}\right)e^{-\dfrac{n\pi y}{a}}$$


While perfectly analytic, this solution is hard to visualize. What does that solution look like? Take $V_0 = 10V$ and $a = 1m$.

1. Plot the approximate solution in 3D space using Python's ```mplot3D``` for just the first term in the sum (i.e., only for $n = 1$). Download this [Jupyter notebook](../../jupyter/HW6-3dPotentialPlot.ipynb) (you can [view it here](https://github.com/emtilt/ph410f19/blob/master/jupyter/HW6-3dPotentialPlot.ipynb)), which walks you through how to plot in 3D.
2. Plot the approximate solution in 3D space for the first 5 terms. What do you notice about the boundary where $V=V_0$?
3. Plot the approximate solution such that the boundary where $V=V_0$ looks very close to constant. How many terms did you need? If you didn't do it for Part 2, you will have to figure out how to automatically compute each term to construct your plot instead of copying-and-pasting 50, or 100, or 1000 times!
4. Given this plot of the potential, sketch (by hand) what the electric field looks like. Recall that $\mathbf{E} = -\nabla V$.


## 2. Potential in a cubical box

You have a cubical box (sides all of length $a$) made of 6 metal plates that are insulated from each other. The left wall is located at $y=-a/2$ and the right wall is at $y=+a/2$. Both left and right walls are held at constant potential $V=V_0$. All four other walls are grounded ($V=0$ for these walls).

(Note that I've set up the geometry so the cube runs from $x=0$ to $x=a$, and from $z=0$ to $z=a$,  but from $y=-a/2$ to $y=+a/2$  This should actually make the math work out a little easier!)

1. Find the potential $V(x,y,z)$ everywhere inside the box.
2. Is V=0 at the center of this cube?
3. Is E=0 at the center of the cube? Why, or why not?

## 3. Separation of variables - Cartesian 2D with new Boundary Conditions

A square rectangular pipe (sides of length $a$) runs parallel to the z-axis (from $-\infty$ to $\infty$)  The 4 sides are maintained with boundary conditions given in the figure. (Each of the 4 sides is insulated from the others at the corners).

![Tube](../../images/hw6-tube_2.png "Tube")


1. Find the potential $V(x,y,z)$ at all points in this pipe.
2. Sketch the E-field lines and equipotential contours inside the pipe. 
3. State in words what the boundary condition on the bottom wall means - what does it tell you? Is the bottom wall a conductor? (Bonus of one half-point: What physical situation would produce such a boundary condition? That is, how would an experimentalist arrange things so as to guarantee that $\partial V/\partial y=0$  on the 4th side?)    
3. Find the charge density $\sigma(x=0,y,z)$ everywhere on the left conducting wall ($x=0$).


## 4. Method of relaxation in 1D

In this problem, you will write a 1D method of relaxation solver for Laplace's equation. Your solver should start with boundary conditions (e.g., $V(0) = 0$ and $V(1) = 1$) and then use the method of relaxation to develop a linear solution (in 1D, we *know* that the solution should turn out linear, so this let's you check that your code works). Though this solver might seems trivial because the solution is obvious in 1D, this will allow you to get a feel for implementing the method before I ask you to expand it to 2D next week. Secondly, you will investigate what happens when you make bad initial guesses. Your solution to this problem should take the form of a Python notebook.

Let me briefly remind you of the pseudocode that we developed in class:

* Cut up the space into equal size bins (called the mesh) of size $a$
* Set the boundary conditions at V(left side) and V(right side)
* Make some reasonable guess for all the values in between
* Set a maximum number of iterations (just in case -- we don't want infinite loops)
* For each value **not** at the boundary set it equal to average of the surrounding two points
  - Compute the error (e.g., the difference between all the points before and after the previous step)
  - Compare the error to your acceptable value
  - Repeat the averaging until you reach the acceptable value or hit the maximum iterations
* Plot your results

Your solution to this problem should address the following:
1. For at least one set of boundary conditions, plot all the estimates of the potential until your answer converges (to demonstrate how the algorithm works)
2. Plot how many iterations it takes to achieve different levels of acceptable error (0.1, 0.01, etc.). Do not go too small because your code may run for a very long time.
3. Attempt to increase/reduce the number of iterations with poorer/better initial guesses. What kinds of initial guesses coverge the quickest, which ones are the slowest to coverge?
4. Find guesses that throw off the algorithm (i.e., give nonsensiscal answers). Griffith's mentions this in the book: the method of relaxation works for "reasonable initial guesses." As a hint, try sinsoudial, expoential, or logarithmic guesses.

## 5. Sphere with a known potential

We have a sphere (radius, $R$) where we have glued charges to the outside such that the electric potential at the surface of the sphere is given by:

$$V(r=R,\theta) = V_0 \cos 2\theta$$

where $k$ is some constant.

You are going to find the potential inside and outside the sphere (there are no charges other than those at the surface of the sphere) as well as the charge density $\sigma(\theta)$ on the surface of the sphere. Each part of this problem is meant to walk you through the process for solving these kinds of boundary-value problems.

1. Rewrite the potential at the surface using Legendre polynomials. *You will need to dust off some trig identities to do this.* You can find a [listing of Legendre polynomials online](http://mathworld.wolfram.com/LegendrePolynomial.html).
2. Using this boundary condition and the knowledge that $V$ should be finite inside the sphere, find the electric potential, $V(r,\theta)$, inside this sphere. You do not have to re-derive the general solution to Laplace's equation, just use the result:
$$V(r,\theta) = \sum_l \left(A_lr^l+\dfrac{B_l}{r^{l+1}}\right)P_l(\cos \theta)$$
3. Using the same boundary condition and the knowledge that $V$ should vanish far from the sphere, find the electric potential, $V(r,\theta)$, outside this sphere.
4. Show explicitly that your solutions to parts 2 and 3 match at the surface of the sphere.
5. Take the "normal" derivative of each of your solutions ($\partial V/\partial r$) and use their difference at the surface to find the charge on the surface via our usual boundary condition on electric field discontinuities: $$\left(\dfrac{\partial V_{out}}{\partial r}-\dfrac{\partial V_{in}}{\partial r}\right) = -\dfrac{\sigma}{\varepsilon_0}$$
6. Sketch the charge distrbution on the surface of the sphere.


## 6. Solving Laplace's Equation in Cylindrical Coordinates

We have gone through how to solve Laplace's equation in Cartesian and spherical coordinates. In both cases, finding a separable and general solution was possible. In fact, there are a [number of possible coordinate systems](http://mathworld.wolfram.com/LaplacesEquation.html) where we can do this, but the most relevant to this class (besides Cartesian and spherical) is cylindrical coordinates.

In this problem, you will develop the general solution to Laplace's equation in cylindrical coordinates where there is no dependence on the $z$ coordinate (i.e., where we have cylindrical symmetry).

1. Starting from Laplace's equation in Cylindrical coordinates, use the ansatz $V(s,\phi) = S(s)\Phi(\phi)$ to convert the problem from one partial differential equation to two 2nd order ordinary differential equations -- one for $S(s)$ and one for $\Phi(\phi)$.
2. As we have argued twice, each of those differential equations is equal to a constant. Which constant is positive and which is negative? Explain your choice. *Think about what happens when you rotate your problem by 2$\pi$ in the $\phi$ direction, should the physics care that you've done that?* Going forward, choose the positive constant to be $+k^2$ and the negative one to be $-k^2$.
3. Solve the differential equation for $\Phi(\phi)$ to obtain the general solution for $\Phi(\phi)$. Hint: $\Phi(\phi) = \Phi(\phi + 2\pi)$ so this puts an additional condition on $k$ that it must be an integer with $k \geq 0$.
4. Armed with this information about $k$, solve the differential equation for $S(s)$ to obtain the general solution for $S(s)$. *Be careful to treat $k=0$ separately as that generates an additional and completely physical solution!*
5. Combine your solutions to Parts 3 and 4 to generate the complete general solution $V(s,\phi) = S(s)\Phi(\phi)$.
6. The potential at a distance $s$ away from an infinite line charge (which should be captured by this solution) is: $V(s) = \dfrac{2\lambda}{4 \pi\varepsilon_0}\ln(s)$ + constant, which terms in general solution vanish to capture this solution?

*This problem is tough. But here's a little help. The general solution for the electric potential in cylindrical coordinates (with cylindrical symmetry) is:*

$$V(s,\phi) = a_0 + b_0 \ln s + \sum_{k=1}^\infty \left[s^k(a_k \cos k\phi + b_k \sin k \phi)+s^{-k}(c_k \cos k\phi + d_k \sin k \phi)\right]$$

You will not get credit for this problem unless your work clearly shows how this solution is developed. I can't imagine giving full credit for this solutions if your solution doesn't include some English words explaining your reasoning and logical flow at various steps. Ask your self: Could another student *fully* understand your logic just by looking at your solution? If not, then you have not completed this problem.

## 7. Conceptual Multipole Expansion

Developing intuition about the dominant contribution to the field that you are looking at will serve you very well in the future. In this problem, you will look at a few charge distributions (blue - positive charge; orange - negative charge) and discuss what the dominant contribution (monopole, dipole, quadrapole) to the field would be far from the distribution (as $r \rightarrow \infty$).

For each distribution below, discuss which contribution to the multipole expansion dominates at large $r$. Explain how you can tell this is the dominant contribution (use equations, pictures, and words as you see fit).

1. Distribution 1: ![Distribution 1](../../images/hw6-distribution1.png)
2. Distribution 2: ![Distribution 2](../../images/hw6-distribution2.png)
3. Distribution 3: ![Distribution 3](../../images/hw6-distribution3.png)
