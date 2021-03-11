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
<!--
<section data-markdown>

Given that the potential at any point is given by the average of the surrounding points,

$$V(x,y) \approx \dfrac{1}{4}[ V(x+a,y) + V(x,y+a)$$
$$ +V(x-a,y) + V(x,y-a)]$$

Draft the psuedocode for finding the approximate potential.

</section>
-->
