---
title: "Day 17 -  Conductors"
permalink: /slides/day17
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Feb 26
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown="">

### For Monday
- No reading due. Some people skipped today's reading survey today, though, so make sure you're caught up through Section 3.1....

HW5 due today. HW6 posted tonight or tomorrow.
	
</section>


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
<!--

<section data-markdown>

A positive charge ($q$) is outside a metal conductor with a hole cut out of it at a distance $a$ from the center of the hole. What is the *net* electric field at center of the hole?

1. $\dfrac{1}{4 \pi \varepsilon_0}\dfrac{q}{a^2}$
2. $\dfrac{-1}{4 \pi \varepsilon_0}\dfrac{q}{a^2}$
3. $\dfrac{1}{4 \pi \varepsilon_0}\dfrac{2q}{a^2}$
4. $\dfrac{-1}{4 \pi \varepsilon_0}\dfrac{2q}{a^2}$
5. Zero

Note: Correct Answer E
</section>

<section data-markdown>

With $\nabla \times \mathbf{E} = 0$, we know that,

$$\oint \mathbf{E} \cdot d\mathbf{l} = 0$$

If we choose a loop that includes a metal and interior vacuum (i.e., both in and **inside the hole**), we know that the contribution to this integral in the metal vanishes. What can we say about the contribution in the hole?

1. It vanishes also
2. $\mathbf{E}$ must be zero in there
3. $\mathbf{E}$ must be perpendicular to d$\mathbf{l}$ everywhere
4. $\mathbf{E}$ is perpendicular to the metal surface
5. More than one of these

Note:
* Correct answer: E (A and B)

</section>

<section data-markdown>

With $\nabla \times \mathbf{E} = 0$, we know that,

$$\oint \mathbf{E} \cdot d\mathbf{l} = 0$$

If we choose a loop that includes a metal and vacuum (i.e., both in and **just outside of the metal**), we know that the contribution to this integral in the metal vanishes. What can we say about the contribution just outside the metal?

1. It vanishes also
2. $\mathbf{E}$ must be zero out there
3. $\mathbf{E}$ must be perpendicular to d$\mathbf{l}$ everywhere
4. $\mathbf{E}$ is perpendicular to the metal surface
5. More than one of these

Note:
* Correct answer: E (both A and D)

</section>
-->
<section data-markdown>

A neutral copper sphere has a spherical hollow in the center.  A charge $+q$ is placed in the center of the hollow.  What is the total charge on the outside surface of the copper sphere? (Assume Electrostatic equilibrium.)

![alt text](../images/d12-coppersphere_hole_and_charge.png "Logo Title Text 1")


1. Zero
2. $-q$
3. $+q$
4. $0 < q_{outer} < +q$
5. $-q < q_{outer} < 0$

Note:
* Correct answer: C


</section>
