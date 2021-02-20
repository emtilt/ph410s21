---
title: "Day 14 -  Potential"
permalink: /slides/day14
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Feb 19
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown="">

### For Monday
- ~~Read Section 3.1~~ *This was an error. The correct assignment is to read Section 2.5 in Griffiths*
- Do survey
- I might be a few minutes late to class. Please be patient.
HW4 due today
HW5 posted tonight or tomorrow, due Friday.
	
</section>

<section data-markdown>

### So far, we have Gauss plus...

- Find $V$ from $E$: $V(\vec{r})=-\int_A^B\vec{E}\cdot d\vec{l}$
- Find $V$ from $\rho$: $V(\vec{r})=k\int_V\frac{\rho (\mathbf{r}^\prime)d\tau^\prime}{|\mathfrak{r}|}$
- Find E from V: $\vec{E}(\vec{r})=-\nabla V(\vec{r})$
- Find E from $\rho$: Coulomb integral...
	
</section>
<section data-markdown>
 The potential is zero at some point in space.

You can conclude that:
1. The E-field is zero at that point
2. The E-field is non-zero at that point
3. You can conclude nothing at all about the E-field at that point

Note:
* Correct Answer: C

</section>





<section data-markdown>

The potential is constant everywhere in some region of space.

You can conclude that:
1. The E-field has a constant magnitude in that space.
2. The E-field is zero in that space.
3. You can conclude nothing at all about the magnitude of $\mathbf{E}$ along that line.

Note:
* Correct Answer: B

</section>

<section data-markdown>

We are trying to compute the the electric potential $V(\mathbf{r})$ for a line of charge at the location $\langle x,0,z \rangle$. What is $|\mathfrak{R}|$ in this case?

1. $x$
2. $z$
3. $\sqrt{x^2+z^2}$
4. Something else

Note: Correct Answer D (needs to have z')

</section>

<section data-markdown>

We derived the potential for this short rod to be

$V(x,z) = \dfrac{\lambda}{4\pi\varepsilon_0}\log\left[\dfrac{L+z+\sqrt{x^2+(L+z)^2}}{L-z+\sqrt{x^2+(L-z)^2}}\right]$

The associated electric field at $\langle x,0,z\rangle$ location can have the following components:

1. only x
2. only y
3. only z
4. x, y, and z
5. Something else

</section>

<section data-markdown>

![alt text](../images/d10-charged_shell.png "Logo Title Text 1")

A spherical *shell* has a uniform positive charge density on its surface. (There are no other charges around.)

What is the electric field *inside* the sphere?
1. $\mathbf{E}=0$ everywhere inside
2. $\mathbf{E}$ is non-zero everywhere in the sphere
3. $\mathbf{E}=0$ only that the very center, but non-zero elsewhere inside the sphere.
4. Not enough information given

Note:
* Correct Answer: A
Used as lead in to “continuity/boundary conditions”. 91% correct, but still worth making sure they know WHY E=0 everywhere, that is, can they articulate the symmetry argument (that E must be radial) from which Gauss’ law gives the answer. (Many seem to think if flux is zero, then E is zero, so they can get the right answer for inadequate reasoning!) -SJP
WRITTEN BY:  Steven Pollock (CU-Boulder), from a freshman question by M. Dubson

</section>

<section data-markdown>

We derived the electric potential outside ($r>R$) the charged shell to be

$$V(r) = \dfrac{1}{4\pi\varepsilon_0}\dfrac{q}{r}$$

What is it for $r<R$?

1. Zero
2. Constant
3. It changes but I don't know how yet
4. Something else

Note:
* Correct Answer: B

</section>

