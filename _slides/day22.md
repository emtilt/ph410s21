---
title: "Day 22 -  finishing relaxation, starting sep. of var."
permalink: /slides/day22
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Mar 12<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown="">

### For Monday
- Griffiths Section 3.3.2
- Reading survey


### HW due today, new HW posted today or tomorrow
</section>


<section data-markdown>

The Method of Relaxation also works for Poisson's equation (i.e., when there is charge!).

Given, $\nabla^2 V \approx \dfrac{V(x+a)-2V(x)+V(x-a)}{a^2}$

Which equations describes the appropriate "averaging" that we must do:

1. $V(x) = \dfrac{1}{2}(V(x+a)-V(x-a))$
2. $V(x) = \dfrac{\rho(x)}{\varepsilon_0}+\dfrac{1}{2}(V(x+a)+V(x-a))$
3. $V(x) = \dfrac{a^2\rho(x)}{2\varepsilon_0}+\dfrac{1}{2}(V(x+a)+V(x-a))$

Note:
* Correct answer: C


</section>


<!--
<section data-markdown>

Given that we want to solve Laplace's equation in 2D and that we have a description for the numerical second derivative of one variable,

$$f''(x) \approx \dfrac{f(x+a)-2f(x)+f(x-a)}{a^2}$$

what is the appropriate numerical partial derivative for $V(x,y)$, $\partial^2 V/\partial x^2 \approx$

1. $$\left[V(x+a) - 2V(x) + V(x-a)\right]/a^2$$
2. $$\left[V(x+a,y) - 2V(x,y) + V(x-a,y)\right]/a^2$$
3. $$\left[V(y+a) - 2V(y) + V(y-a)\right]/a^2$$
4. $$\left[V(x,y+a) - 2V(x,y) + V(x,y-a)\right]/a^2$$
5. More than one is correct

Note:
* Correct answer: B is correct

</section>
<section data-markdown>

Given that the potential at any point is given by the average of the surrounding points,

$$V(x,y) \approx \dfrac{1}{4}[ V(x+a,y) + V(x,y+a)$$
$$ +V(x-a,y) + V(x,y-a)]$$

Draft the psuedocode for finding the approximate potential.

</section>
-->

<section data-markdown>

### Separation of Variables (Cartesian)

![alt text](../images/d17-cartesian_sep_variables.png "Logo Title Text 1")
<!--https://jeremykun.com/2016/09/26/voltage-temperature-and-harmonic-functions/-->


</section>

<section data-markdown>

Say you have three functions $f(x)$, $g(y)$, and $h(z)$.
$f(x)$  depends on $x$ but not on $y$ or $z$.
$g(y)$ depends on $y$ but not on $x$ or $z$.
$h(z)$ depends on $z$ but not on $x$ or $y$.

If $f(x) + g(y) + h(z) = 0$ for all $x$, $y$, $z$, then:

1. All three functions are constants (i.e. they do not depend on $x$, $y$, $z$ at all.)
2. At least one of these functions has to be zero everywhere.
3. All of these functions have to be zero everywhere.
4. All three functions have to be linear functions in $x$, $y$, or $z$ respectively (such as $f(x)=ax+b$)

Note:
* CORRECT ANSWER: A

</section>

<section data-markdown>

If our general solution contains the function,

$$X(x) = Ae^{\sqrt{c}x} + Be^{-\sqrt{c}x}$$

What does our solution look like if $c<0$; what about if $c>0$?

1. Exponential; Sinusoidal
2. Sinusoidal; Exponential
3. Both Exponential
4. Both Sinusoidal
5. ???

Note:
* CORRECT ANSWER: B

</section>

<section data-markdown>

Our example problem has the following boundary conditions:

* $V(0,y>0) = 0; V(a,y>0) = 0$
* $V(x_{0\rightarrow a},y=0) = V_0; V(x,y\rightarrow \infty) = 0$

If $X''= c_1 X$ and $Y'' = c_2Y$ with $c_1 + c_2 = 0$, which is constant is positive?

1. $c_1$
2. $c_2$
3. It doesn't matter either can be

Note:
* CORRECT ANSWER: B
* Exponential solutions are expected in the y direction
</section>


<section data-markdown>

Given the two diff. eq's :

$$\dfrac{1}{X}\dfrac{d^2X}{dx^2} = C_1 \qquad \dfrac{1}{Y}\dfrac{d^2Y}{dy^2} = C_2$$

where $C_1+C_2 = 0$.  Given the boundary conditions in the figure, which coordinate should be assigned to the negative constant (and thus the sinusoidal solutions)?

![alt text](../images/d17-cq_cartesian_bc_1.png "Logo Title Text 1")

1. x
2. y
3. $C_1 = C_2 = 0$ here
4. It doesn't matter.

Note:
* CORRECT ANSWER: B
* Because it has to vanish on both ends
</section>

<section data-markdown>

Given the two diff. eq's :

$$\dfrac{1}{X}\dfrac{d^2X}{dx^2} = C_1 \qquad \dfrac{1}{Y}\dfrac{d^2Y}{dy^2} = C_2$$

where $C_1+C_2 = 0$.  Given the boundary conditions in the figure, which coordinate should be assigned to the negative constant (and thus the sinusoidal solutions)?

![alt text](../images/d17-cq_cartesian_bc_2.png "Logo Title Text 1")

1. x
2. y
3. $C_1 = C_2 = 0$ here
4. It doesn't matter.

Note:
* CORRECT ANSWER: C
* It's constant throughout!
</section>
<section data-markdown>
	
While we wait on slack...
	
When does $\sin(ka)e^{-ky}$ vanish?

1. $k = 0$
2. $k = \pi/(2a)$
3. $k = \pi/a$
4. A and C
5. A, B, C

Note:
* CORRECT ANSWER: D
* It's actuall n*pi/a

</section>
<section data-markdown>

Suppose $V_1(r)$ and $V_2(r)$ are linearly independent functions which both solve Laplace's equation, $\nabla^2 V = 0$.

Does $aV_1(r)+bV_2(r)$ also solve it (with $a$ and $b$ constants)?

1. Yes. The Laplacian is a linear operator
2. No. The uniqueness theorem says this scenario is impossible, there are never two independent solutions!
3. It is a definite yes or no, but the reasons given above just aren't right!
4. It depends...


Note:
* CORRECT ANSWER: A

</section>

<section data-markdown>

What is the value of $\int_0^{a} \sin(n\pi x/a)\sin(m\pi x/a)\;dx$ ?

1. Zero
2. Non-zero
5. Depends on $n$ and $m$

Note:
* CORRECT ANSWER: C
* If n = m then integral is non-zero

</section>

<section data-markdown>


### Exact Solution to example in book:

$$V(x,y) = \sum_{n=1}^{\infty} \dfrac{4V_0}{n\pi}\dfrac{1}{\cosh\left(\frac{n\pi}{2}\right)}\cosh\left(\frac{n\pi x}{a}\right)\sin\left(\frac{n \pi y}{a}\right)$$

### Approximate Solutions:
### (1 term; 20 terms)

![alt text](../images/d17-saddle_potential.png "Logo Title Text 1")
![alt text](../images/d17-saddle_potential_20.png "Logo Title Text 1")

</section>
