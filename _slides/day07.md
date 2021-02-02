---
title: "Day 7 - Coulomb"
permalink: /slides/day07
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Feb 3
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>

<section data-markdown="">

### For Friday
- Read Griffiths 2.2
- Reading survey due at 9am 
- HW2 due
	
</section>

<section data-markdown>
## Classical Electromagnetism
|  |  |
| :---: | :---: |
| ![jupiter](../images/d6-jupiter.jpg "jupiter") | ![helium](../images/d6-helium.png "helium") |


$\sim 10^8\mathrm{m} \longrightarrow \longrightarrow \longrightarrow\longrightarrow\longrightarrow\longrightarrow \sim 10^{-16}\mathrm{m}$

**24 orders of magnitude**

Note: As far we know, the theory of Classical E&M works for 24 orders of magnitude. It breaks down on the subatomic scale (QM), but we really don't know how far it extends one the upper-end as it is consistent with relativity. Tests of Jupiter's magnetic field are consistent with predictions from Classical E&M.

</section>

<section data-markdown>
## Electrostatics

![efield](../images/d6-efieldwiki.png "efield")</section>

<!--<section data-markdown>

Ten charges are arranged as shown. What is the E field at point P?

![](../images/d6-superpositioncharges.png "") 

1. Zero
2. Non-zero
3. Really need trig and a calculator to decide

Note:
CORRECT ANSWER: A
</section> -->

<section data-markdown>

5 charges, q, are arranged in a regular pentagon, as shown.
What is the E field at the center?

![](../images/5charges.png "") 

1. Zero
2. Non-zero
3. Really need trig and a calculator to decide

Note:
CORRECT ANSWER: A
</section>

<section data-markdown>

1 of the 5 charges has been removed, as shown. What’s the E field at the center?

![](../images/4charges.png "") 

1. $+(kq/a^2)\hat{y}$
2. $-(kq/a^2)\hat{y}$
3. 0
4. Something entirely different!
5. This is a nasty problem which I need more time to solve

Note:
CORRECT ANSWER:  B
Superposition!

</section>

<section data-markdown>

If all the charges live on a line (1-D), use:

$$ \lambda \equiv \dfrac{\mathrm{charge}}{\mathrm{length}}$$

<!--Draw your own picture. What's $\mathbf{E}(\mathbf{r})$?-->

</section>

<section data-markdown>

To find the E-field at P from a thin line (uniform charge density $\lambda$):

![line charge](../images/d6-linecharge.png "line charge")
$$ \mathbf{E}(\mathbf{r}) = \dfrac{1}{4\pi\varepsilon_0}\int \dfrac{\lambda dl'}{\mathfrak{R}^2}\hat{\mathfrak{R}}$$
What is $\mathfrak{R}$?

1. $x$
2. $y'$
3. $\sqrt{dl'^2 + x^2}$
4. $\sqrt{x^2+y'^2}$
5. Something else

Note:
CORRECT ANSWER: D

</section>

<section data-markdown>

$\mathbf{E}(\mathbf{r}) = \int \dfrac{\lambda dl'}{4\pi\varepsilon_0\mathfrak{R}^3}\vec{\mathfrak{R}}$, so: $E_x(x,0,0) = \dfrac{\lambda}{4\pi\varepsilon_0}\int \dots$

![line charge](../images/d6-linecharge_coords.png "line charge")

1. $\int \dfrac{dy'x}{x^3}$
2. $\int \dfrac{dy' x}{(x^2 + y'^2)^{3/2}}$
3. $\int \dfrac{dy' y'}{x^3}$
4. $\int \dfrac{dy' y'}{(x^2+y'^2)^{3/2}}$
5. Something else

Note:
CORRECT ANSWER: B

</section>

<section data-markdown>

What do you expect to happen to the field as you get really far from the rod?

$$E_x = \dfrac{\lambda}{4\pi\varepsilon_0\}\dfrac{L}{x\sqrt{x^2+L^2}}$$

1. $E_x$ goes to 0.
2. $E_x$ begins to look like a point charge.
3. $E_x$ goes to $\infty$.
4. More than one of these is true.
5. I can't tell what should happen to $E_x$.

Note:
CORRECT ANSWER: D (A and B)

</section>
<section data-markdown>

### Taylor Series are crucial tools
https://en.wikipedia.org/wiki/Taylor_series

The Taylor series of a  function$f(x)$ that is differentiable at a  number $a$ is the power series
$$f(a)+\frac {f'(a)}{1!} (x-a)+ \frac{f''(a)}{2!} (x-a)^2+\frac{f'''(a)}{3!}(x-a)^3+ \cdots = \sum_{n=0} ^ {\infty} \frac {f^{(n)}(a)}{n!} (x-a)^{n},$$
where $f^{(n)}(a)$ denotes the $n$th derivative of $f$ evaluated at the point $a$. 

Some are so common that you'll memorize them through frequent use if you stay in physics.
</section>

<section data-markdown>

What do you expect to happen to the field as you get really far from the rod?

$$E_x = \dfrac{\lambda}{4\pi\varepsilon_0\}\dfrac{L}{x\sqrt{x^2+L^2}}$$

1. $E_x$ goes to 0.
2. $E_x$ begins to look like a point charge.
3. $E_x$ goes to $\infty$.
4. More than one of these is true.
5. I can't tell what should happen to $E_x$.

Note:
CORRECT ANSWER: D (A and B)

</section>

<section data-markdown>

$$E_x = \dfrac{\lambda}{4\pi\varepsilon_0\}\dfrac{L}{x\sqrt{x^2+L^2}}$$


If we are *far from the rod*, what is the small parameter in our Taylor expansion?

1. $x$
2. $L$
3. $x/L$
4. $L/x$
5. More than one of these

Note: Correct answer is D, but this is about a discussion about dimensionless parameters - small compared to what!
</section>


<section data-markdown>

$$E_x = \dfrac{\lambda}{4\pi\varepsilon_0\}\dfrac{L}{x\sqrt{x^2+L^2}}$$


If we are *very close* to the rod, what is the small parameter in our Taylor expansion?

1. $x$
2. $L$
3. $x/L$
4. $L/x$
5. More than one of these

Note: Correct answer is C, but this is about a discussion about dimensionless parameters - small compared to what!
</section>

<!--<section data-markdown>

The model we developed for the motion of the charged particle near the charged disk (on the center axis) is represented by this *nonlinear* differential equation:

$$\ddot{x} = C \left[1- \dfrac{1}{(x^2+R^2)^{1/2}}\right]$$

You decide to expand this expression for small parameter is $x/R$, under what conditions is any solution appropriate?

1. When the disk is very large
2. When the disk is very small
3. When the particle is far from the disk
4. When the particle is near the disk
5. More than one of these

Note: Correct answer is E; it's that you are both close compared to the size of the disk (A and D)
</section>-->

<section data-markdown>

Given the location of the little bit of charge ($dq$), what is $|\vec{\mathfrak{R}}|$?

![charged sphere with position vectors](../images/d7-sphereintegrate.png "charged sphere with position vectors")

1. $\sqrt{z^2+r'^2}$
2. $\sqrt{z^2+r'^2-2zr'\cos\theta}$
3. $\sqrt{z^2+r'^2+2zr'\cos\theta}$
4. Something else

Note:
CORRECT ANSWER: B


</section>
