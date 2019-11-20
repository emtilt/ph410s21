---
layout: archive
collection: homework
title: "Homework 7 - Due Friday, November 1 at 4:30pm"
permalink: /homework/hw7/
author_profile: true
---
[Link to Slack team -- a great place to ask questions](https://ph410f19.slack.com)

After wrapping up the method of relaxation, Homework 7 then helps you further investigates the multipole expansion and develop models for polarization that we will use to understand electric fields in matter. Notice that for polarization problems, we can often find the bound charges and solve the problems much like we have done before with free charges.


## 1. Method of Relaxation for Cartesian Problems

One of the major properties of a solution to Laplace's equation is that the value of the potential at a point is equal the average of all the points surrounding it (i.e., a sphere in 3D or a circle in 2D). We can exploit this property to solve Laplace's equation numerically by successively computing the average value of the potential at a point on a mesh (a grid of 2D points in this case) based on the 4 other points that surround it (see the figure below).

![Mesh](../../images/hw7-mesh.png)

To be explicit, in the simplest relaxation codes, we replace the value of the potential $V_{i,j}$ with the arithmetic average of its closest neighbors on the mesh:

$$V_{i,j} = \dfrac{1}{4}\left(V_{i-1,j} + V_{i,j-1} + V_{i,j+1} + V_{i+1,j}  \right)$$

The procedure for solving Laplace's equation numerically involves the following steps:

* **Step 1:** Slice up the space where $\nabla^2 V = 0$ (and the boundary) into a grid of points (called a "mesh") that are spaced an equal distance apart. That mesh may have different spacing between points based on what the details of the problem being solved might be. For example, if the potential is expected to be change over short distances in some points and not others, it can make sense to change the spacing to optimize computational time (or memory). In this problem, we will use a mesh of equally spaced points.
* **Step 2:** Set the value of the boundary points given the specific problem you intend to solve. This will typically be done in the initial parts of the program and can be changed easily to solve other kinds of problems. In this problem, we will start with a non-zero constant value (10 V) on one edge and zero at the other 3 edges.
* **Step 3:** Starting at some location off the boundary, systematically loop through each point applying the averaging function given above. It would be typical to start at one corner of the mesh and move systematically across (or down) and then down (or across) calculating the value at each new point as you go.
* **Step 4:** Compute the difference between the starting values of the potential and the values after a full iteration. Compare this difference to the accepted error that you decided on before starting the calculation, $Error_{i,j} = Vnew_{i,j}-Vold_{i,j}$. Here, you could use the average error, the maximum error, or something else. In this problem, you can choose what error to use.
* **Step 5:** Repeat steps 3 and 4 until the computed error is below the accepted error. Note that you should build in a maximum number of steps to take in case the code doesn't coverge on an answer quickly. You'd like to avoid infinite (or nearly infinite) loops
* **Step 6:** Plot the results to ensure that the solution is behaving in an understandable way.

1. Using the code you wrote for homework 6, expand/modify it to solve the 2D problem where one boundary is set at 10V and the others are set to zero. You will have to pick a reasonable step size for the mesh (make sure it can be adjusted!). 
2. Produce a 3D Plot of the potential.
3. [Review how to make a contour plot using matplotlib](http://matplotlib.org/examples/pylab_examples/contour_demo.html) and produce a contour plot of your results.
4. Determine how many iterations on the mesh are needed to obtain an error tolerances of: 1e-2, 1e-3, 1e-4, 1e-5, 1e-6, and 1e-7. You might have to adjust the maximum number of allowed iterations as the error tolerance is decreased.
5. Set the value of one of the boundaries to be a stepwise value (e.g., half the points to be 10V and the other half to -10V) with the other 3 boundaries to 0V. Repeat parts 2 and 3. Make note of the shape of the potenital plot. Are there any local max or min? Do they go away with tighter error tolerance?
6. Optional bonus of one point: Put a hole of some sort in the mesh. Set the exterior boundary of the hole to anything you like; that is, fix the potential around the hole as an additional boundary condition. This scenario is like having a 2D cavity with an interior boundary. This problem cannot be solved analytically, but is very easy to imagine and solve numerically. Plot the results.

## 2. The Beauty of the Multipole expansion

The [multipole expansion](https://en.wikipedia.org/wiki/Multipole_expansion) is a very powerful approximation that arises in a number of different kinds of field theories. The beauty of it is that it can provide a simple approximate form for the field in question far from the sources that produce the field. Often, this is helpful when solving problems where you only care about the dominant contributions because the others only provide small corrections to the behavior.

In this problem, you will explore the the multipole expansion for the charge configuration shown below.

![3 Charges](../../images/hw7-multipole.png)

1. For the three charges shown above, determine the approximate potential at a distance far from the origin of coordinates. Keep only the two lowest non-vanishing orders of the expansion. *Notice that each is a distance $r_0$ from the origin.*
2. Explain how you know the two terms you find are the lowest non-vanishing terms for the potential.
3. Using your answer to part 1, find the approximate electric field produced by this system of charges far from the origin. Express your answer in spherical coordinates.

*Hint: This should not be a very difficult problem. We have already derived most of the ideas that you need to solve it.*

## 3. Multipole Expansion of a Single Point Charge

For this problem, consider a single point charge $+q$. 

1. Place the charge at the origin, write down the electric potential at a location $\mathbf{r} = \langle x,y,z \rangle$ from the origin.
2. Move the charge to a short distance away from the origin on the $z$-axis, $\mathbf{r}' = \langle 0,0,d\rangle$. Write down the electric potential at a location $\mathbf{r} = \langle x,y,z \rangle$ from the origin.
3. Assume the location of interest in Part 2 is far from the charge ($r>>d$). Expand your result in Part 2 keeping only the two leading order terms. Interpret these terms in light of the multipole expansion. *Hint: It might help to rewrite your result in spherical coordinates.*
4. How do you resolve that your answer to Part 1 only contains a monopole term where your answer to Part 3 contains additional terms? Explain your reasoning.

*Hint: If you are struggling to explain your answers, or don't see the point to this problem, it may help to review Section 3.4.3 in Griffiths.*

<!--
## 4. A Curious Sphere of Charge

In this problem, we ask you to plot a few functions. You have plotted quite a bit using Jupyter, so we expect that you will use a Jupyter notebook of your own design to do your plotting now.

Consider a sphere of radius $R$ that has a volume charge density inside the sphere given by:

$$\rho(r,\theta) = \mu r \sin\left(\dfrac{3\theta}{2}\right)$$

where $\mu$ is known constant and $\theta$ is the usual polar angle in spherical coordinates.

1. Plot $\rho(r,\theta)/r$ in units of $\mu$ as a function of $\theta$. Where does this charge live in space? Note that $\rho \propto r$.
2. Calculate the total charge, $Q$, on the sphere.
3. Calculate the dipole moment, $\mathbf{p}$, of the sphere.
4. Use your results from Parts 2 and 3 to find $V(r,\theta)$ when you are far from the sphere ($r>>R$). Discuss how your results make sense with the plot in Part 1.
5. The function $\sin\left(\frac{3\theta}{2}\right) \approx \frac{1}{\sqrt{2}} + \frac{3}{2\sqrt{2}}\cos\theta$, which would suggest that the volume charge density can be written as $\rho(r,\theta) \approx \frac{\mu r}{\sqrt{2}} + \frac{3\mu r}{2\sqrt{2}} \cos \theta$. So this will look like a superposition of a spherically symmetric density and a density proportional to $\cos \theta$. Plot $\rho(r,\theta)/r$ in units of $\mu$ as a function of $\theta$ in this approximation.
6. How does your plot in Part 1 compare to your plot in Part 5? Is this a good approximation to the original charge density? What does this imply about our approximation of $V$ compared to the exact $V$?
-->

## 4. A spherical shell charge distribution
Griffiths derives (end of section 3.3.2) the exact potential $V(r,\theta)$ everywhere outside a spherical shell of radius $R$ which has a surface charge distribution $\sigma(R,\theta)=\sigma_0\cos\theta$.

1. Calculate the total charge of this object. What is the monopole moment of this object? Why does your answer make sense, given the charge distribution that you started from?
2. What is the dipole moment of this object?
3. Use the method of the multipole expansion (Griffiths sections 3.4.1 and 3.4.2) to find an approximate form for the potential far from the sphere. Stop with the first leading nonzero term.
4. Compare your result toh Griffith's exact formula (from the example, end of section 3.3.2). What does this tell you about the quadrupole moment (and higher moments) of this surface charge distribution? (I think this result is interesting.)

## 5. Atomic hydrogen and the polarization model

(Note: This problem is based off of Griffiths Problem 4.1, which was assigned in a reading survey. No one seemed to have a deep understanding of the problem, so this is a revisiting of it. You have an answer to much of this problem already. I'm asking you to reconsider it and clearly delineate the logic of it. As is always a good practice, use words to explain yourself clearly.)

Griffiths Table 4.1 gives an experimental value for $\alpha/4\pi\varepsilon_0$ for atomic hydrogen. (Read his caption carefully for units.)

1. The "atomic polarizibility", $\alpha$ is defined by $\mathbf{p}=\alpha\mathbf{E}$. Study Griffiths' Example 4.1, which tells you how to estimate the atomic polarizability, summarize the example in your own words.
2. Following the example and using it with this experimental value for $\alpha/4\pi\varepsilon_0$ for atomic hydrogen, estimate the atomic radius of hydrogen. How well did you do, compared, say, with the Bohr radius?
3. After summarizing the example, discuss what physical assumption (i.e., simplification) Griffiths is making about the physical distribution of negative charge inside an atom? Is that realistic?
4. Now suppose you have a single hydrogen atom inside a charged parallel-plate capacitor, with plate spacing 1 mm, and voltage 100 V. Determine the "separation distance" $d$ (as defined in that same Example 4.1 problem) of the electron cloud and the proton nucleus. What fraction of the atomic radius of part 2 is this? (You should conclude that 100 V across a 1mm gap capacitor is unlikely to ionize a hydrogen atom. Do you agree? Why?)
5. Use your calculations to *roughly* estimate what voltage (and thus, what E-field) would ionize this single hydrogen atom. (We might say that if you can pull the electron cloud one full atomic radius away, it's breaking down.)


## 6. Polarized sphere of charge

Consider a dielectric sphere of radius $a$ that has a polarization that is directed radially outward from the center of the sphere, $\mathbf{P} = P_0\mathbf{r}$.

1. Determine the bound charges at the surface, $\sigma_B$, and in the volume of the sphere, $\rho_B$.
2. Find the electric field everywhere.
4. Sketch the electric field lines inside and outside the sphere. What does your sketch say about the electric field at the boundary of the sphere? Does this make sense to you? Why or why not?

## 7. Charge conservation

When a neutral dielectric is polarized, no new charges are created or destroyed, so the total charge must still be zero. The charge density on the surface is given by:

$$\sigma_B = \mathbf{P}\cdot\hat{n}$$

The charge density in the bulk is given by:

$$\rho_B = -\nabla \cdot \mathbf{P}$$

Using these definitions, show that the total charge for any neutral dielectric with a polarization $\mathbf{P}$ is zero.
