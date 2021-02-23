---
title: "Day 15 -  Boundary conditions, energy"
permalink: /slides/day15
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Feb 22
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown="">

### For Wednesday
- Read Section 2.5 in Griffiths if you missed it because I was unclear

HW5 due Friday.
	
</section>

<section data-markdown>
Review from last time:
	
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

<section data-markdown>

### Last time, we kinda started thinking about boundary conditions

- $\mathbf{E}$ can be discontinuous, but $V$ cannot.
- Can we be more specific?
<!--- $E^\perp_{\rm above}-E^\perp_{\rm below}=\frac{\sigma}{\epsilon_0}$
- What about $E^\parallel$?-->

</section>
<section data-markdown>

### Electrostatic Potential Energy

</section>

<section data-markdown>

Consider slowly moving a positive charge from a location of low electric potential to one of high electric potential. What is the sign of the work done by you ($W_u$)? What is the sign of the work done by electric field ($W_f$)?

1. $W_u < 0$; $W_f > 0$
2. $W_u < 0$; $W_f < 0$
3. $W_u > 0$; $W_f > 0$
4. $W_u > 0$; $W_f < 0$

Note: Correct Answer is D; Draw field

</section>

<section data-markdown>

![alt text](../images/d11-three_charges.png "Logo Title Text 1")

Three identical charges $+q$ sit on an equilateral triangle. What would be the final $KE$ of the top charge if you released it (keeping the other two fixed)?

1. $\frac{1}{4\pi\varepsilon_0}\frac{q^2}{a}$
2. $\frac{1}{4\pi\varepsilon_0}\frac{2q^2}{3a}$
3. $\frac{1}{4\pi\varepsilon_0}\frac{2q^2}{a}$
4. $\frac{1}{4\pi\varepsilon_0}\frac{3q^2}{a}$
5. Other

Note:
CORRECT ANSWER: C

</section>

<section data-markdown>

![alt text](../images/d11-three_charges.png "Logo Title Text 1")

Three identical charges $+q$ sit on an equilateral triangle. What would be the final $KE$ of the top charge if you released *all three*?

1. $\frac{1}{4\pi\varepsilon_0}\frac{q^2}{a}$
2. $\frac{1}{4\pi\varepsilon_0}\frac{2q^2}{3a}$
3. $\frac{1}{4\pi\varepsilon_0}\frac{2q^2}{a}$
4. $\frac{1}{4\pi\varepsilon_0}\frac{3q^2}{a}$
5. Other

Note:
CORRECT ANSWER: A

</section>

<!--<section data-markdown>

Does system energy "superpose"?

That is, if you have one system of charges with total stored energy $W_1$, and a second charge distribution with $W_2$...if you superpose these charge distributions, is the total energy of the new system simply $W_1 + W_2$?

1. Yes
2. No

Note:
* CORRECT ANSWER: B
* Draw 4 charges and show that it is not the sum of the 2 charges and the other 2.

</section>-->
