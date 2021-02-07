---
title: "Day 8 - Coulomb, Taylor Series"
permalink: /slides/day08
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Feb 5
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown="">

### For Monday
- HW2 due on Monday
- Read Section 1.5 in Griffiths, and then revisit the mentions of the delta function in Section 2.2 to make sense of them
	
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
