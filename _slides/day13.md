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
	
</section

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
