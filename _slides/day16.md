---
title: "Day 16 -  Finishing energy, starting conductors"
permalink: /slides/day16
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Feb 24
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown="">

### For Friday
- Read Section  in Griffiths

HW5 due Friday.
	
</section>

<section data-markdown="">

$W_{sys}=\frac{1}{2}\int V(\vec{r^\prime})\rho(\vec{r^\prime})d\tau^\prime$

where $V(\vec{r^\prime})$ is the potential at $\vec{r^\prime}$ due to all of $\rho$ except right at $\vec{r^\prime}$ (so...everything)


	
</section>


<section data-markdown>

![alt text](../images/d11-pt_charges_energy.png "Logo Title Text 1")

Two charges, $+q$ and $-q$, are a distance $r$ apart.  As the charges are slowly moved together, the total field energy

$$\dfrac{\varepsilon_0}{2}\int E^2 d\tau$$

1. increases
2. decreases
3. remains constant

Note:
* CORRECT ANSWER: B
* Consider when they overlap, field goes to zero, must be E gets smaller as they get closer. same volume
</section>

<!--
<section data-markdown>

![alt text](../images/d11-capacitor_pull_apart.png "Logo Title Text 1")


A parallel-plate capacitor has $+Q$ on one plate, $-Q$ on the other.  The plates are isolated so the charge $Q$ cannot change.  As the plates are pulled apart, the total electrostatic energy stored in the capacitor:

1. increases
2. decreases
3. remains constant.
</section>
-->
<section data-markdown>

### Conductors

![alt text](../images/d12-electron_sea.gif "Logo Title Text 1")


</section>

<section data-markdown>

### The conductor problem
![alt text](../images/d12-metal.png "Logo Title Text 1")



Note:
* CORRECT ANSWER: A
* Same E; constant; larger volume where it is non-zero
</section>
<!--
<section data-markdown>

A typical metal has one free election per atom. These electrons are free to move in response to external electric fields. There are $\sim 10^{22}$ free electrons in a cubic centimeter of copper. Roughly what size of electric field could a single 1cm sub of copper "respond" to by polarizing?

1. 1 N/C
2. 10 N/C
3. 100 N/C
4. 1000 N/C
5. Something more than these


Note: Correct answer is E. It's closer to 10e17 N/C

</section>
-->

<section data-markdown>

A point charge $+q$ sits outside a **solid neutral conducting copper sphere** of radius $A$. The charge q is a distance $r > A$ from the center, on the right side. What is the E-field at the center of the sphere? (Assume equilibrium situation).

![alt text](../images/d12-copper_1.png "Logo Title Text 1")


1. $|E| = kq/r^2$, to left
2. $kq/r^2 > |E| > 0$, to left
3. $|E| > 0$, to right
4. $E = 0$
5. None of these

Note:
* CORRECT ANSWER: D
* Net electric field inside of a metal in static equilibrium is zero
* Talk about the net field versus the field due to the charges on the metal.

</section>

<section data-markdown>

In the previous question, suppose **the copper sphere is charged**, total charge $+Q$. (We are still in static equilibrium.) What is now the magnitude of the E-field at the center of the sphere?

![alt text](../images/d12-copper_2.png "Logo Title Text 1")


1. $|E| = kq/r^2$
2. $|E| = kQ/A^2$
3. $|E| = k(q-Q)/r^2$
4. $|E| = 0$
5. None of these! / it’s hard to compute

Note:
* CORRECT ANSWER: D
* Talk about the net field versus the field due to the charges on the metal.
</section>
<section data-markdown>

We have a large copper plate with uniform surface charge density, $\sigma$.
Imagine the Gaussian surface drawn below.  Calculate the E-field a small distance $s$ above the conductor surface.

![alt text](../images/d12-copper_plate.png "Logo Title Text 1")

1. $|E| = \frac{\sigma}{\varepsilon_0}$
2. $|E| = \frac{\sigma}{2\varepsilon_0}$
3. $|E| = \frac{\sigma}{4\varepsilon_0}$
4. $|E| = \frac{1}{4\pi\varepsilon_0}\frac{\sigma}{s^2}$
5. $|E| = 0$

Note:
* CORRECT ANSWER: A
* Might have to do derivation and go through details of infinitely thin line charge. Must be +sigma on other side, btw.

</section>

<section data-markdown>

Consider a long coaxial with charge $+Q$ placed on the inside metal wire and $-Q$ outside metal sheath as shown.

![alt text](../images/d12-coax_abc.png "Logo Title Text 1")

Sketch the distribution of charge in this situtation using plus signs to represent positive chages and minus signs to represent negative charges.

Note:
* Ask them for answers, put up on board and turn into clicker question
* Answer should be plusses on outside of inner and minuses inside of outer (equal numbers)

</section>

<section data-markdown>

If you were calculating the potential difference, $\Delta V$, between the center of the inner conductor ($s=0$) and infinitely far away ($s \rightarrow \infty$), what regions of space would have a (non-zero) contribution to your calculation?

![alt text](../images/d12-coax_abc.png "Logo Title Text 1")

1. $s<a$
2. $a<s<b$
3. $b<s<c$
4. $s>c$
5. More than one of these

Note:
* Correct answer: E
* Should be where the metal is

</section>

<section data-markdown>
	
![alt text](../images/d12-coax_Qin.png "Logo Title Text 1")

Now, draw the charge distribution (little + and – signs) if the inner conductor has a total charge $+Q$ on it, and the outer conductor is electrically neutral.

Note:
* Ask them for answers, put up on board and turn into clicker question
* Answer should be plusses on outside of inner and minuses inside of outer and plusses on outside of outer (equal numbers)

</section>

<section data-markdown>

![alt text](../images/d12-coax_offcenter.png "Logo Title Text 1")

 Consider how the charge distribution would change if the inner conductor is shifted off-center, but still has $+Q$ on it, and the outer conductor remains electrically neutral. Draw the new charge distribution (little + and – signs) and be precise about how you know.

Note:
* Ask them for answers, put up on board and turn into clicker question
* Answer should be plusses on outside of inner and minuses inside of outer and plusses on outside of outer (equal numbers); shift only on outside of inner and inside of outer (no net field from them)

</section>

<section data-markdown>

![alt text](../images/d12-coax_Qout.png "Logo Title Text 1")


Return the inner conductor to the center.

Instead of the total charge $+Q$ being on the inner conductor, sketch the charge distribution (little + and – signs) if the outer conductor has a total charge $+Q$ on it, and the inner conductor is electrically neutral. Be precise about exactly where the charge will be on these conductors, and how you know.

Note:
* Ask them for answers, put up on board and turn into clicker question
* Answer should be plusses on outside of outer; nothing else.

</section>
