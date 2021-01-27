---
title: "Day 5 - Vector Calc, part 4, and numerical integration"
permalink: /slides/day05
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Jan 29
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>


<section data-markdown="">

### This afternoon
- Homework 1 due

### For Monday
- Read Griffiths 2.1
- Reading survey 

### For next Friday
- HW2 due
	
</section>


<section data-markdown>

You are trying to compute the work done by a force, $\mathbf{F} = a\hat{x} + x\hat{y}$, along the line $y=2x$ from $\langle 0,0 \rangle$ to $\langle 1,2 \rangle$. What is $d\mathbf{l}$?

1. $dl$
2. $dx\~\hat{x}$
3. $dy\~\hat{y}$
4. $2dx\~\hat{x}$
5. Something else

Note:
* CORRECT ANSWER: E
* It's $dx\~\hat{x}+dy\~\hat{y}$.
* Fall 2016 (given right at the end of class): 8 6 8 58 [20]; 5 0 3 38 [54]

</section>

<section data-markdown>

You are trying to compute the work done by a force, $\mathbf{F} = a\hat{x} + x\hat{y}$, along the line $y=2x$ from $\langle 0,0 \rangle$ to $\langle 1,2 \rangle$. Given that $d\mathbf{l} = dx\hat{x}+dy\hat{y}$, which of the following forms of the integral is correct?

1. $\int_0^1 adx + \int_0^2 xdy$
2. $\int_0^1 (adx + 2xdx)$
3. $\frac{1}{2} \int_0^2 (ady + ydy)$
4. More than one is correct

Note:
* CORRECT ANSWER: D
* All are correct forms, but B and C are ready to integrate.
* Fall 2016: 7 3 0 [90] 0

</section>


<section data-markdown>

A certain fluid has a velocity field given by $\mathbf{v} = x\hat{x} + b \hat{y}$. Which component(s) of the field contributed to "fluid flux" integral ($\int_S \mathbf{v}\cdot d\mathbf{A}$) through the x-z plane?

1. $v_x$
2. $v_y$
3. both
4. neither

Note:
* CORRECT ANSWER: B
* Only the vector perpendicular to the surface will contribute
* Fall 2016: 16 [78] 4 0 0
</section>

<section data-markdown>

A certain fluid has a velocity field given by $\mathbf{v} = x\hat{x} + b \hat{y}$. If we intend to calculate the "fluid flux" integral ($\int_S \mathbf{v}\cdot d\mathbf{A}$) through the x-z plane, what is $d\mathbf{A}$ in this case? Be specific!

1. $dxdy\hat{y}$
2. $dxdz\hat{y}$
3. $dxdz\hat{z}$
4. $dydz\hat{z}$
4. It's none of these

</section>

<section data-markdown>

For the same fluid with velocity field given by $\mathbf{v} = x\hat{x} + b \hat{y}$. What is the value of the "fluid flux" integral ($\int_S \mathbf{v}\cdot d\mathbf{A}$) through the entire x-y plane?

1. It is zero
2. It is something finite
3. It is infinite
4. I can't tell without doing the integral

Note:
* CORRECT ANSWER: A
* The velocity field is parallel to the x-y plane every where and hence contributes no flux through the surface.
* Fall 2016: [89] 9 3 0 0

</section>

<section data-markdown>

A rod (radius $R$) with a hole (radius $r$) drilled down its entire length $L$ has a mass density of $\frac{\rho_0\phi}{\phi_0}$ (where $\phi$ is the normal polar coordinate).

To find the total mass of this rod, which coordinate system should be used (take note that the mass density varies as a function of angle):

1. Cartesian ($x,y,z$)
2. Spherical ($r,\phi,\theta$)
3. Cylindrical ($s, \phi, z$)
4. It doesn't matter, just pick one.

Note:
* CORRECT ANSWER: C
* It makes the most sense from the geometry of the problem and writing the limits.
* Fall 2016: 0 0 [94] 6 0

</section>



<section data-markdown>

Proved in book:

#### Gradient Theorem

$$\int_\mathbf{a}^\mathbf{b} \left(\nabla T\right)\cdot d\mathbf{l}=T(\mathbf{b})-T(\mathbf{a})$$

#### Divergence Theorem

$$\int_V \left( \nabla\cdot\mathbf{v}\right) d\tau=\oint_S \mathbf{v}\cdot d\mathbf{a}$$

#### Stokes Theorem

$$\int_S \left( \nabla\times\mathbf{v}\right)\cdot d\mathbf{a}=\oint_P \mathbf{v}\cdot d\mathbf{l}$$

Note:
elev: sum of path along slope, diff of start end
water: faucets, flux out
flux of curl through S, circulation (flow along closed boundary)

</section>

<section data-markdown>

Consider a vector field defined as the gradient of some well-behaved scalar function:
$$\mathbf{v}(x,y,z) = \nabla T(x,y,z).$$

What is the value of $\oint_C \mathbf{v} \cdot d\mathbf{l}$?

1. Zero
2. Non-zero, but finite
3. Can't tell without a function for $T$

Note:
* CORRECT ANSWER: A
* Closed loop integral of a gradient is zero.
* Fall 2016: [92] 4 4 0 0

</section>

<section data-markdown>

## Numerical Integration

![alt text](../images/d5-numerical_midpoint.gif "Logo Title Text 1")

</section>

<section data-markdown>

Consider this trapezoid

![alt text](../images/d5-trapezoid_shape.png "Logo Title Text 1")

What is the area of this trapezoid?

1. $f(c)h$
2. $f(d)h$
3. $f(c)h + \frac{1}{2}f(d)h$
4. $\frac{1}{2}f(c)h + \frac{1}{2}f(d)h$
5. Something else

Note:
* Correct Answer: D
</section>

<section data-markdown>

The trapezoidal rule for a function $f(x)$ gives the area of the $k$th slice of width $h$ to be,

$$A_{k} = \frac{1}{2}h\left(f(a+(k-1)h) + f(a+kh)\right)$$

What is the approximate integral, $I(a,b) = \int_a^b f(x) dx$, $I(a,b) \approx$

1. $\sum_{k=1}^N \frac{1}{2}h\left(f(a+(k-1)h) + f(a+kh)\right)$
2. $h\left(\frac{1}{2}f(a) + \frac{1}{2}f(b) + \frac{1}{2}\sum_{k=1}^{N-1}f(a+kh)\right)$
3. $h\left(\frac{1}{2}f(a) + \frac{1}{2}f(b) + \sum_{k=1}^{N-1}f(a+kh)\right)$
4. None of these is correct.
4. More than one is correct.

Note:
* Correct Answer: D (both A and C)

</section>

<section data-markdown>

The trapezoidal rule takes into account the value and slope of the function. The next "best" approximation will also take into account:

1. Concavity of the function
2. Curvature of the function
3. Unequally spaced intervals
4. More than one of these
5. Something else entirely

</section>
<section data-markdown>

![alt text](../images/d5-simp.png "Source: https://www.value-at-risk.net/numerical-integration-in-one-dimension/")

</section>
