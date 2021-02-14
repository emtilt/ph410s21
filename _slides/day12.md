---
title: "Day 12 - Finishing Gauss's Law"
permalink: /slides/day12
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Feb 15
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown="">

### For Wednesday
- no reading

HW3 due Wednesday
	
</section>

<!--<section data-markdown>

Consider a cube of constant charge density centered at the origin.

**True or False**: I can use Gauss' Law to find the electric field directly above the center of the cube.

1. True and I can argue how we'd do it.
2. True. I'm sure we can, but I don't see how to just yet.
3. False. I'm pretty sure we can't, but I can't say exactly why.
4. False and I can argue why we can't do it.

</section>
<section data-markdown>
Consider a spherical Gaussian surface. What is the $d\mathbf{A}$ in $\int\int\mathbf{E}\cdot d\mathbf{A}$?

1. $r d\theta d\phi \hat{r}$
2. $r^2 d\theta d\phi \hat{r}$
3. $r \sin \theta d\theta d\phi \hat{r}$
4. $r^2 \sin \theta d\theta d\phi \hat{r}$
5. Something else

Note:
* Correct Answer: D
</section>-->


<section data-markdown>

Consider an infinite sheet of charge with uniform surface charge density $+\sigma$ lying in the $x-y$ plane. From symmetry arguments, we can argue that $\mathbf{E}(x,y,z)$ can be simplified to:

1. $\mathbf{E}(x,y)$; direction undetermined
2. $E_z(x,y)$
3. $\mathbf{E}(z)$; direction undetermined
4. $E_z(z)$
5. Something else

</section>

<section data-markdown>

We derived that the electric field due to an infinite sheet with charge density $\sigma$ was as follows:

$$\mathbf{E}(z) = \begin{cases} \dfrac{\sigma}{2\varepsilon_0}\hat{k} & \mbox{if} & \mbox{ z > 0} \cr \dfrac{-\sigma}{2\varepsilon_0}\hat{k} & \mbox{if} & \mbox{ z < 0}\end{cases}$$

What does that tell you about the difference in the field when we cross the sheet, $\mathbf{E}(+z)-\mathbf{E}(-z)$?

1. it's zero
2. it's ${\sigma}/{\varepsilon_0}$
3. it's -${\sigma}/{\varepsilon_0}$
4. it's +${\sigma}/{\varepsilon_0} \hat{k}$
5. it's -${\sigma}/{\varepsilon_0} \hat{k}$

Note:
* CORRECT ANSWER: D
* Makes for a good discussion about cross one direction versus the other

</section>
<section data-markdown>

SLAC (Stanford Linear Accelerator Center) is where quarks (including the charm
quark), and the tauon (like a heavier electron) were discovered.

![alt text](../images/d8-slac_overhead.jpg "Logo Title Text 1")

Note: Charged particles are accelerated inside a long metal cylindrical pipe, which is 2 miles long and has a radius R = 6 cm. All the air is pumped out of this pipe, known as the "beam line."
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
<section data-markdown>

## Gauss's law in integral form...

$\oint_S \mathbf{E}\cdot d\mathbf{a}=\frac{Q_{\rm enc}}{\epsilon_0}$

## ...plus divergence theorem...

$\oint_S \mathbf{E}\cdot d\mathbf{a}=\int_V\left( \nabla\cdot \mathbf{E}\right) d\tau$

## ...Gauss's law in differential form

$\nabla\cdot\mathbf{E}=\rho/\epsilon_0$


</section>
<section data-markdown>

#### Div of $\mathbf{E}$ contains Guass's Law. What about curl?
Know $\mathbf{E}(\vec{r})=k\int_V \frac{\rho(\vec{r^\prime})d\tau^\prime}{|\mathfrak{r}|^2}\hat{\mathfrak{r}}$.

Also, from HW1:
- $\nabla\times\nabla f=0$
- $\nabla\frac{1}{|\mathfrak{r}|}=-\frac{\hat{\mathfrak{r}}}{|\mathfrak{r}|^2}$

</section>
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
