---
title: "Day 4 - Vector Calc, part 3"
permalink: /slides/day04
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">

### PH410 - Electromagnetism

Jan 27
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->

</section>


<section data-markdown>
While we wait for class to start: A rod (radius $R$) with a hole (radius $r$) drilled down its entire length $L$ has a mass density of $\frac{\rho_0\phi}{\phi_0}$ (where $\phi$ is the normal polar coordinate).

To find the total mass of this rod, which coordinate system should be used (take note that the mass density varies as a function of angle):

1. Cartesian ($x,y,z$)
2. Spherical ($r,\phi,\theta$)
3. Cylindrical ($s, \phi, z$)
4. It doesn't matter, just pick one.

Prove it by doing the integral.

Note:
* CORRECT ANSWER: C
* It makes the most sense from the geometry of the problem and writing the limits.
* Fall 2016: 0 0 [94] 6 0

</section>


<section data-markdown="">

### For Friday
- Homework 1 due
	
</section>


<section data-markdown>

A certain fluid has a velocity field given by $\mathbf{v} = x\hat{x} + z \hat{y}$. Which component(s) of the field contributed to "fluid flux" integral ($\int_S \mathbf{v}\cdot d\mathbf{A}$) through the x-z plane?

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

A certain fluid has a velocity field given by $\mathbf{v} = x\hat{x} + z \hat{y}$. If we intend to calculate the "fluid flux" integral ($\int_S \mathbf{v}\cdot d\mathbf{A}$) through the x-z plane, what is $d\mathbf{A}$ in this case? Be specific!

1. $dxdy\hat{y}$
2. $dxdz\hat{y}$
3. $dxdz\hat{z}$
4. $dydz\hat{z}$
4. It's none of these

</section>

<section data-markdown>

For the same fluid with velocity field given by $\mathbf{v} = x\hat{x} + z \hat{y}$. What is the value of the "fluid flux" integral ($\int_S \mathbf{v}\cdot d\mathbf{A}$) through the entire x-y plane?

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
_**Skipped in class, but good practice. Think about the starting and ending points.**_

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

![alt text](../images/d3-divredbox.png "Logo Title Text 1")

This picture represents the field lines of a single positive point charge. What is the divergence in the boxed region? What is the divergence of the whole field?


1. Boxed region is zero; whole field is zero
2. Boxed region is non-zero; whole field is zero
3. Boxed region is zero; whole field is non-zero
4. Boxed region is non-zero; whole field is non-zero
5. ???

Note:
* CORRECT ANSWER: C

</section>

<section data-markdown>

**Activity:** For a the electric field of a point charge, $\mathbf{E}(\mathbf{r}) = \dfrac{1}{4\pi\varepsilon_0}\dfrac{q}{r^2}\hat{r}$, compute $\nabla \cdot \mathbf{E}$.

*Hint: The front fly leaf of Griffiths suggests that the we take:*
$$\dfrac{1}{r^2}\dfrac{\partial}{\partial r}\left(r^2 E_r\right)$$

Note:
* You get zero! Motivates delta function

</section>

<section data-markdown>

Remember this?

![alt text](../images/d3-divredbox.png "Logo Title Text 1")

</section>


<section data-markdown>

What is the value of:

$$\int_{-\infty}^{\infty} x^2 \delta(x-2)dx$$

1. 0
2. 2
3. 4
4. $\infty$
5. Something else

Note:
* CORRECT ANSWER: C

</section>

<section data-markdown>

**Activity**: Compute the following integrals for 2-3 minutes. Note anything special you had to do.

* Left: $\int_{-\infty}^{\infty} xe^x \delta(x-1)dx$
* Middle-Left: $\int_{\infty}^{-\infty} \log(x) \delta(x-2)dx$
* Middle-Right: $\int_{-\infty}^{0} xe^x \delta(x-1)dx$
* Right: $\int_{-\infty}^{\infty} (x+1)^2 \delta(4x)dx$

Note:
* Give them 2-3 minutes to work on it and ask for what they did.

</section>

<section data-markdown>
_**Skipped in class, but good practice.**_
	
Compute:

$$\int_{-\infty}^{\infty} x^2\delta(3x+5)dx$$

1. $25/3$
2. $-5/3$
3. $25/27$
4. $25/9$
5. Something else


Note:
* CORRECT ANSWER: C
* Use a u substitution.

</section>
