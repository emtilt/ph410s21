---
title: "Day 13 - Beginning Potential"
permalink: /slides/day13
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Feb 17
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown="">

### For Wednesday
- no reading

HW3 due today
	
</section>

<section data-markdown>

## Gauss's law in integral form...

$\oint_S \mathbf{E}\cdot d\mathbf{a}=\frac{Q_{\rm enc}}{\epsilon_0}$

## ...plus divergence theorem...

$\oint_S \mathbf{E}\cdot d\mathbf{a}=\int_V\left( \nabla\cdot \mathbf{E}\right) d\tau$

## ...Gauss's law in differential form

$\nabla\cdot\mathbf{E}=\rho/\epsilon_0$


</section>
<section data-markdown>

What is the curl of the vector field, $\mathbf{v}= c\hat{\phi}$, in the region shown below?

![alt text](../images/d10-c_phi_field.png "Logo Title Text 1")

1. non-zero everywhere
2. zero at some points, non-zero at others
3. zero curl everywhere

Note:
* CORRECT ANSWER: A

</section>


<!--<section data-markdown>

What is the curl of this vector field, in the red region shown below?

![alt text](../images/curl_red_box.png "Logo Title Text 1")

1. non-zero everywhere in the box
2. non-zero at a limited set of points
3. zero curl everywhere shown
4. we need a formula to decide

Note:
* CORRECT ANSWER: D
* I think it's D because it depends on how the field drops off, which we haven't indicated. If it's drops off like 1/r, then it has no curl.
</section>

<section data-markdown>

What is the curl of this vector field, $\mathbf{v} = \dfrac{c}{s}\hat{\phi}$, in the red region shown below?

![alt text](../images/curl_red_box.png "Logo Title Text 1")

1. non-zero everywhere in the box
2. non-zero at a limited set of points
3. zero curl everywhere shown

</section>-->


<section data-markdown>

#### Div of $\mathbf{E}$ contains Guass's Law. What about curl?
Know $\mathbf{E}(\vec{r})=k\int_V \frac{\rho(\vec{r^\prime})d\tau^\prime}{|\mathfrak{r}|^2}\hat{\mathfrak{r}}$.

Also, from HW1:
- $\nabla\times\nabla f=0$
- $\nabla\frac{1}{|\mathfrak{r}|}=-\frac{\hat{\mathfrak{r}}}{|\mathfrak{r}|^2}$

</section>
<!--<section data-markdown>

Consider a vector field $\mathbf{F}$. If the curl of that vector field is zero ($\nabla \times \mathbf{F} = 0$), which of the following are true?

I. $\int \nabla \times \mathbf{F} \cdot d\mathbf{A} = 0$<br>

II. $\oint \mathbf{F} \cdot d\mathbf{l} = 0$<br>

III. $\int_A^B \mathbf{F} \cdot d\mathbf{l}_1$ = $\int_A^B \mathbf{F} \cdot d\mathbf{l}_2$<br>

IV. $\vec{F}$ is the gradient of some scalar function $f$, $\vec{F} = \nabla f$.

1. Only I
2. I and II
3. II and III
4. I, II, and III
5. Some other combination


</section>

<section data-markdown>

Is the following mathematical operation ok?

$$\nabla \times \left(\dfrac{1}{4\pi\epsilon_0}\int\int\int_V \dfrac{\rho(\mathbf{r}')d\tau'}{\mathfrak{R}^2}\hat{\mathfrak{R}}\right) = $$
$$\dfrac{1}{4\pi\epsilon_0}\int\int\int_V \left(\nabla \times\dfrac{\rho(\mathbf{r}')d\tau'}{\mathfrak{R}^2}\hat{\mathfrak{R}}\right)
$$

1. Yup. It's just fine and I can say why
2. I think it's fine, but I'm not sure I know why
3. No, we can't exchange the curl and an integral!
4. I'm not sure.


</section>

<section data-markdown>

Is it mathematically ok to do this?

$$\mathbf{E} = \dfrac{1}{4\pi\varepsilon_0}\int_V\rho(\mathbf{r}')d\tau'\left(-\nabla\dfrac{1}{\mathfrak{R}}\right)$$

$$\longrightarrow \mathbf{E} =-\nabla\left( \dfrac{1}{4\pi\varepsilon_0}\int_V\rho(\mathbf{r}')d\tau'\dfrac{1}{\mathfrak{R}}\right)$$

1. Yes
2. No
3. ???

Note:
* Correct Answer: A
</section>-->

<section data-markdown>

## Electric Potential

![alt text](../images/d9-lightning.jpg "Logo Title Text 1")

</section>
<section data-markdown>

### Stokes

$\int_S\left(\nabla\times\mathbf{E}\right)\cdot d\mathbf{a}=\oint_C\mathbf{E}\cdot d\mathbf{l}$
</section>

<section data-markdown>

If $\nabla \times \mathbf{E} = 0$, then $\oint_C \mathbf{E} \cdot d\mathbf{l} =$

1. 0
2. something finite
3. $\infty$
4. Can't tell without knowing $C$

Note:
* Correct Answer: A

</section>
<section data-markdown>

### If...

$\int_S\left(\nabla\times\mathbf{E}\right)\cdot d\mathbf{a}=\oint_C\mathbf{E}\cdot d\mathbf{l}$

### Then...

$\oint_C\mathbf{E}\cdot d\mathbf{l}=0$

</section>
<section data-markdown>

Can superposition be applied to electric potential, $V$?

$$V_{tot} \stackrel{?}{=} \sum_i V_i = V_1 +V_2 + V_3 + \dots$$

1. Yes
2. No
3. Sometimes

Note:
* Correct answer: A (usually)
As long as the zero potential is the same for all measurements.

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

### So far, we have Gauss plus...

- Find $V$ from $E$: $V(\vec{r})=-\int_A^B\vec{E}\cdot d\vec{l}$
- Find $V$ from $\rho$: $V(\vec{r})=k\int_V\frac{\rho (\mathbf{r}^\prime)d\tau^\prime}{|\mathfrak{r}|}$
- Find E from V: $\vec{E}(\vec{r})=-\nabla V(\vec{r})$
- Find E from $\rho$: Coulomb integral...
	
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



<section data-markdown>

![alt text](../images/d10-graph_shell.png "Logo Title Text 1")

Could this be a plot of $\left|\mathbf{E}(r)\right|$? Or $V(r)$? (for SOME physical situation?)

1. Could be $E(r)$, or $V(r)$
2. Could be $E(r)$, but can't be $V(r)$
3. Can't be $E(r)$, could be $V(r)$
4. Can't be either

Note:
* Correct Answer: B

</section>
<!--
<section data-markdown>

We usually choose $V(r\rightarrow\infty) \equiv 0$ when calculating the potential of a point charge to be $V(r) = +kq/r$. How does the potential $V(r)$ change if we choose our reference point to be $V(R) = 0$ where $R$ is close to $+q$.

1. $V(r)$ higher than it was before
2. $V(r)$ is lower than it was before
4. $V(r)$ doesn’t change ($V$ is independent of  choice of reference)

Note:
* CORRECT ANSWER: B
* Show redefinition.


</section>
-->
