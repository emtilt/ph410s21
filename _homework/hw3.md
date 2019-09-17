---
layout: archive
collection: homework
title: "Homework 3 - Due Friday, September 20 at 4:30pm"
permalink: /homework/hw3/
author_profile: true
---
[Link to Slack team -- a great place to ask questions](https://ph410f19.slack.com)


Homework 3 emphasizes alternative methods to direct integration (Coulomb's Law) for solving the electric field problem including the use of Gauss' Law. In addition, it introduces the concept of the Dirac delta function as a tool for describing distributions of charge. This homework makes use of what you learned in Secs. 1.5 and 2.2, but what you know from 2.1 (i.e., superposition of $\mathbf{E}$) will also be important. Additionally, for the first time so far in this course, we are able to start to apply our skills to real physical systems (Problems 8 and 9 allow you to model an atom and a liquid crystal, respectively).

### 1. Numerical Superposition - Electric field of a line charge

As we discussed in class, you can break up a disutrubiton of charge into chunks - each a point charge - and add up the contirubtions to the electric field of each chunk. This process forms the basis of numerical superposition, which you began to explore in the [last homework (problem 3)](../hw2). In this problem, you will extend that work to a line of charge. You will solve this problem using a Jupyter notebook. You can [download the notebook](../../jupyter/HW3_Electric_Field_Line_Charge.ipynb) (or [view it here](https://github.com/emtilt/ph410f19/blob/master/jupyter/HW3_Electric_Field_Line_Charge.ipynb)). Using numerical superposition, adding up the contributions to the electric field due to each chunk, you will study the electric field that results from this charge distribution.

### 2. Comparing Coulomb's Law to Gauss' Law

Now that we have, in principle, fully described how to solve any electrostatics problem (i.e., by adding up the contribution of each chunk of charge), we turn to building our theoretical toolbox by learning alternative methods that make the solving of certain kinds of problems more tractable. The first of these alternatives is Gauss' Law. It is important to know when and how to apply Gauss' Law - in the problem below, you are asked to compare Gauss' Law with Coulomb's Law.

Consider the following questions in finding the electric field everywhere for a conducting sphere, a uniformly charged sphere, and a sphere with charge distribution varying as $r^n$, all with radius $r_0$ and total charge $Q$:

1. What are the advantages and disadvantages of using Gauss' Law to find the electric field instead of using Coulomb's Law (Griffiths Eq 2.8)?  What role does symmetry play?
2. Answer the same questions for three cubes with the same properties (i.e., charge distributions that vary radially as $r^n$).
3. What do your answers to parts 1 and 2 tell you about using Gauss' Law versus using Coulomb's Law (direct integration) to solve for the electric field?

### 3. Spherical charge distributions are special

As you might have picked up by now, spherically symmetric charge distributions are very special. We have a number of theoretical tools we can bring to bear on them and the results we produce are often quite simple in a mathematical sense. In this problem, you will explore these distributions a bit more and connect the mathematics (i.e., the integrals you must do) to the geometry of the problem (i.e., where the charge lives) to gain intuition about these spherically symmetric distributions of charge.

For parts 1 and 2, consider a sphere of radius $R$, centered one the origin, with a radially symmetric charge distribution $\rho(r)$.

1. What $\rho(r)$ is required for the electric field **in the sphere** to have the power law form $E(r) = cr^n$, where $c$ and $n$ are constants? The case of n=-2 is special. How so? Some values of $n$ are unphysical because these would lead to an infinite amount of charge in the sphere.. Which values of $n$ are allowed?
2. What kind of charge distribution is required for the radial E-field inside the sphere to be of constant magnitude; that is, what $\rho(r)$ produces $E(r) = $ constant (inside only)? Is this distribution physical realizable? Why or why not?
3. For each of these allowable charge distributions, what does the electric field look like outside the sphere ($r>R$)?
4. Two spherical, nonconducting, and very thin shells of uniformly distributed positive charge $Q$ and radius $d$ are located a distance $10d$ apart. A positive point charge $q$ is placed inside on of the shells at a distance $2d/3$ from the center, on the line connecting the centers of the two shells, as shown in the figure. What is the net force on the charge $q$?

![two spheres](../../images/hw3-gre_problem.png "two spheres")


### 4. Describing charge distributions with delta functions

The [Dirac delta function](https://en.wikipedia.org/wiki/Dirac_delta_function) is an important theoretical tool for describing distributions of a variety of physical quantities (e.g., mass, charge) where a point object (or system of point objects) is the model we intend to use. In addition, it can be used to describe distributions where these quantities exist in highly constrained spaces (e.g., on a plane or spherical shell). In this class, we will use the Dirac delta function to describe how a charges are distributed. In this problem, you will get familiar with the Dirac delta function for a set point charges on a line.

The linear charge density for a series of charges on the $x$-axis is given by:

$$\lambda(x) = \sum_{n=0}^{10} q_0 n^2\delta\left(x-\dfrac{n}{10~\rm m^{-1}}\right)$$

1. In words, describe the units of each part of this equation. (Don't forget the delta function!)
2. What is the total charge on $x$-axis?

### 5. Gauss's Law and Divergence
Gauss’ law and Divergence 
The electric field outside an infinite line that runs along the z-axis is  $\vec{E}=\frac{2\lambda}{4\pi\epsilon_0}\frac{\hat{s}}{s}$
in cylindrical coordinates. (This is derived in Griffiths Example 2.1.) 

1. Find the divergence of the E field for $s>0$. 
2. Calculate the electric flux out of an imaginary Gaussian cylinder of length $L$, and radius $a$, centered around the $z$ axis. Please do this 2 different ways to check yourself: by direct integration, and using Gauss' law. 
3.  Given your (superficially contradictory) results from parts 1 and 2, what is the divergence of this E field?  Express it as a single mathemtical equation valid over all space in cylindrical coordinates


### 6. A rod with a hole drilled in it

Gauss' Law can be useful in situations where you want to determine the electric field in conceptually different physical spaces. In this problem, you will explore this using the example of a uniformly charged rod with a hole drilled through it.

Consider a rod of length $L$ and radius $b$ that has a hole drilled down the center of it (along it's length-wise axis) with a radius of $a$. The rod is very long compared to it's radius, so that Gauss' Law can be used to find the approximate electric field near the middle of the rod (far from the ends). The rod has a uniform charge distribution $\rho$. 

1. Find the electric field inside the hole ($r<a$).
2. Find the electric field outside the rod ($r>b$).
3. Find the electric field between the hole and outer surface of the rod ($a<r<b$).
4. Why did you need to solve Gauss' Law 3 times in this case to find the electric field "everywhere"?
5. Compare the value of the electric field right at the material boundaries ($r=a$ and $r=b$), where two of your three solutions meet. Do the values match? As we will find, this matching has important implications for bound charge on material surfaces.

### 7. The E field in hydrogen atoms

1. Consider a hydrogen atom, consisting of an (approximately) point-like proton at its center and an electron around the proton. Quantum mechanics tells us that the electron is effectively "smeared out," so the electron's resulting contribution to the charge density is $\rho_e\left( r \right)=\rho_0 \exp \left( -2r/a_0 \right)$ where $a_0$ is the Bohr radius. **Find an expression for the electric field in this atom as a function of distance $r$ from its center.** Your final answer should depend only on $r$, $a_0$, and other fundamental constants, so you'll need to somehow figure out what $\rho_0$ equals. Also, don’t forget there is also that point-like proton in the middle of this atom!
2. Plot your result in a Python notebook (which you should submit). Your result will have a bunch of nasty constants with cumbersome units associated with them, which do not make for an easy plot to set up in Python. There's no reason to worry about them either; the purpose of making a plot is to see how the function behaves, not study the size of various SI units. You should therefore make a plot in terms of a *dimensionless* variable. In this case, your x-axis variable should be $r/a_0$, so you will need to rearrange your function such that you only have factors of $r/a_0$, not factors of $r$ alone. Continue rearranging your equation so that *both* sides of the equation are dimensionless. (Hint: once you've done this succesffully, you'll want to label your vertical axis with something like "$E$ (in units of $4\pi\epsilon_0 a_0^2/e$)" and your horizontal axis with $r/a_0$.)
3. Explain clearly in words how all of  the features of your plot makes physical sense, including the behavior near the center of the atom, far from the center, and the behavior in between (simply saying something like "it decreases" is **not** sufficient).


### 8. A liquid crystal
Smectic-C liquid crystals are made of long rodlike molecules with a positive head and a negative tail which pack together to form a long, thin sheet as shown.  The volume charge density is obviously complicated, but can be quite successfully modeled with the rather simple form  $\rho(x,y,z)=\rho_0 \sinh\left(z/z_0\right)$, i.e. uniform in $x$ and $y$, but varying in $z$, with $z = 0$ defined to be the middle of the sheet. (That's the [hyperbolic sine](https://en.wikipedia.org/wiki/Hyperbolic_function#Exponential_definitions) function, by the way, in case the notation is unfamiliar.) Find the electric field everywhere in space, in terms of the constants $\rho_0$, $z_0$ and the sheet thickness $T$. Sketch it as a function of $z$. Where is it biggest?

![smeticc](../../images/hw3-smeticc.png "smecticc")


