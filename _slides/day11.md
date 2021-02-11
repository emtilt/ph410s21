---
title: "Day 11 - Gauss's Law practice examples"
permalink: /slides/day11
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Feb 12
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown="">

### For Monday
- no reading

HW3 due Wednesday
	
</section>
<section data-markdown>
Summarizing the implications of last class...From the divergence theorem,

$\int_V \left(\nabla\cdot{\bf E}\right)d\tau=\oint_S{\bf E}\cdot d{\bf a}$

Working on the right side of the equation by considering a small sphere of radius $r$ around an enclosed charge $q$...

$\oint_S{\bf E}\cdot d{\bf a}=\oint_S\frac{q}{4\pi\epsilon_0 r^2}\hat{\bf r}\cdot d{\bf a}=\frac{q}{4\pi\epsilon_0 r^2}\int  da=\frac{q}{\epsilon_0}$

So $\int_V \left(\nabla\cdot{\bf E}\right)d\tau=\frac{q}{\epsilon_0}$ always, and $\nabla\cdot{\bf E}=\frac{q\delta^3\left({\bf r}\right)}{\epsilon_0}$

</section>
<section data-markdown>

A Gaussian surface which is *not* a sphere has a single charge (q) inside it, *not* at the center. There are more charges outside. What can we say about total electric flux through this surface $\oint_S \mathbf{E} \cdot d\mathbf{A}$?

1. It is $q/\varepsilon_0$.
2. We know what it is, but it is NOT $q/\varepsilon_0$.
3. Need more info/details to figure it out.

Note:
* CORRECT ANSWER: A

</section>
<section data-markdown>

A Gaussian surface which is *not* a sphere has a single charge (q) inside it, *not* at the center. There are more charges outside. Can we use Gauss's Law ($\oint_S \mathbf{E} \cdot d\mathbf{A}$) to find $|\mathbf{E}|$?

1. Yes
2. No
3. Maybe?

Note:
* CORRECT ANSWER: B

</section>
<section data-markdown>


![alt text](../images/d8-dipole_gauss.png "Logo Title Text 1")


An electric dipole ($+q$ and $–q$, small distance $d$ apart) sits centered in a Gaussian sphere.

What can you say about the flux of $\mathbf{E}$ through the sphere, and $|\mathbf{E}|$ on the sphere?

1. Flux = 0, E = 0 everywhere on sphere surface
2. Flux = 0, E need not be zero *everywhere* on sphere
3. Flux is not zero, E = 0 everywhere on sphere
4. Flux is not zero, E need not be zero...

Note:
* CORRECT ANSWER: B
* Think about Q enclosed; what can we say about E though? 
USED IN:  Spring 2013 (Pollock) 
LECTURE NUMBER:  5 (Gauss’ Law)
STUDENT RESPONSES:  12, [[84]], 2,2, 0  Sp ’13 (preclass question) 
INSTRUCTOR NOTES This was the “review’ question to start class. Most remembered Gauss law (which was on the board) to vote for A or B, but the debate was about whether the fact that the integral vanishes, does that mean E vanishes EVERYWHERE. It’s so important to understand that knowing the integral doesn’t by itself tell you about the integrand. (There was a lot of discussion, even though the end vote was solid)  -SJP
WRITTEN BY:  Steven Pollock (CU-Boulder) NEW in 2013, combining two older questions. 


</section>
<section data-markdown>

SLAC (Stanford Linear Accelerator Center) is where quarks (including the charm
quark), and the tauon (like a heavier electron) were discovered.

![alt text](../images/d8-slac_overhead.jpg "Logo Title Text 1")

Note: Charged particles are accelerated inside a long metal cylindrical pipe, which is 2 miles long and has a radius R = 6 cm. All the air is pumped out of this pipe, known as the "beam line."
</section>

<!--<section data-markdown>

Consider a cube of constant charge density centered at the origin.

**True or False**: I can use Gauss' Law to find the electric field directly above the center of the cube.

1. True and I can argue how we'd do it.
2. True. I'm sure we can, but I don't see how to just yet.
3. False. I'm pretty sure we can't, but I can't say exactly why.
4. False and I can argue why we can't do it.

</section>-->
<section data-markdown>
Consider a spherical Gaussian surface. What is the $d\mathbf{A}$ in $\int\int\mathbf{E}\cdot d\mathbf{A}$?

1. $r d\theta d\phi \hat{r}$
2. $r^2 d\theta d\phi \hat{r}$
3. $r \sin \theta d\theta d\phi \hat{r}$
4. $r^2 \sin \theta d\theta d\phi \hat{r}$
5. Something else

Note:
* Correct Answer: D
</section>


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
