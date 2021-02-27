---
title: "Day 18 -  Finishing conductors, starting laplace"
permalink: /slides/day18
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Mar 1<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown="">

### For Wednesday
- Read Griffiths Section 3.1. (We won't spend much class time on this section, but you will have a homework question that uses it in the future.)

HW6 due friday	
</section>
<section data-markdown>

![alt text](../images/d12-coax_offcenter.png "Logo Title Text 1")

 Consider how the charge distribution would change if the inner conductor is shifted off-center, but still has $+Q$ on it, and the outer conductor remains electrically neutral. Draw the new charge distribution (little + and – signs) and be precise about how you know.

Note:
* Ask them for answers, put up on board and turn into clicker question
* Answer should be plusses on outside of inner and minuses inside of outer and plusses on outside of outer (equal numbers); shift only on outside of inner and inside of outer (no net field from them)

</section>
<!--
<section data-markdown>

![alt text](../images/d12-cylinder_charge_outside.png "Logo Title Text 1")

A long coax has total charge $+Q$ on the OUTER conductor. The INNER conductor is neutral.

What is the sign of the potential difference, $\Delta V = V(c)-V(0)$, between the center of the inner conductor ($s = 0$)
and the outside of the outer conductor?

1. Positive
2. Negative
3. Zero

Note:
* CORRECT ANSWER: C; there's no field inside at all

</section>
-->
<section data-markdown>

![alt text](../images/d12-conducting_cap_plates_simple.png "Logo Title Text 1")


Given a pair of very large, flat, conducting capacitor plates with total charges $+Q$ and $-Q$. Ignoring edges, what is the equilibrium distribution of the charge?

1. Throughout each plate
2. Uniformly on both side of each plate
3. Uniformly on top of $+Q$ plate and bottom of $–Q$ plate
4. Uniformly on bottom of $+Q$ plate and top of $–Q$ plate
5. Something else

Note:
* CORRECT ANSWER: D

</section>

<section data-markdown>

![alt text](../images/d12-conducting_cap_plates.png "Logo Title Text 1")


Given a pair of very large, flat, conducting capacitor plates with surface charge densities $+/-\sigma$, what is the E field in the region between the plates?

1. $\sigma/2\varepsilon_0$
2. $\sigma/\varepsilon_0$
3. $2\sigma/\varepsilon_0$
4. $4\sigma/\varepsilon_0$
5. Something else

Note:
* CORRECT ANSWER: B

</section>
<!--
<section data-markdown>

The eletric field between the shells is just that of a point charge. What is the electric potential difference between the outer shell ($r=b$) and the inner shell ($r=a$)?

1. $\dfrac{Q}{4\pi\varepsilon_0}\left(\dfrac{1}{b}-\dfrac{1}{a}\right)$
2. $\dfrac{Q}{4\pi\varepsilon_0}\left(\dfrac{1}{a}-\dfrac{1}{b}\right)$
3. $\dfrac{Q}{4\pi\varepsilon_0}\left(\dfrac{1}{b^2}-\dfrac{1}{a^2}\right)$
4. $\dfrac{Q}{4\pi\varepsilon_0}\left(\dfrac{1}{a^2}-\dfrac{1}{b^2}\right)$
5. Something else?

Note: Correct Answer is B
</section>

<section data-markdown>

What is the sign of the potential difference between the outer shell ($r=b$) and the inner shell ($r=a$)?

$\Delta V = V(b) - V(a)$

1. $\Delta V > 0$
2. $\Delta V < 0$
2. ???

Note: Correct Answer is A

</section>
<section data-markdown>

![alt text](../images/d12-capacitor_gap_bigger.png "Logo Title Text 1")



You have two very large parallel plate capacitors, both with the same area and the same charge $Q$.
Capacitor \#1 has twice the gap of Capacitor \#2. Which has more stored potential energy?

1. \#1 has twice the stored energy
2. \#1 has more than twice
3. They both have the same
4. \#2 has twice the stored energy
5. \#2 has more than twice.

Note:
* CORRECT ANSWER: A
* E same; twice volume

</section>


<section data-markdown>

![alt text](../images/d12-capacitor_gap_connected.png "Logo Title Text 1")


A parallel plate capacitor is attached to a battery which maintains a constant voltage difference V between the capacitor plates.  While the battery is attached, the plates are pulled apart. The electrostatic energy stored in the capacitor

1. increases.
2. decreases.
3. stays constant.

Note:
* CORRECT ANSWER: B
* Potential same; field is reduced; but shows up squared while d is increased, overall goes down
</section>
-->



<section data-markdown>

### Laplace's Equation

![alt text](../images/d14-laplace.png "Logo Title Text 1")


</section>

<section data-markdown>
	
This shows up in, like, every field. It's in thermodynamics, plasma physics, fluid dynamics, and even videogame development:
![alt text](../images/d16-gdc.png "Logo Title Text 1")

</section>

<section data-markdown>

![alt text](../images/d14-region_w_no_charge.png "Logo Title Text 1")


A region of space contains no charges. What can I say about $V$ in the interior?

1. Not much, there are lots of possibilities for $V(r)$ in there
2. $V(r)=0$ everywhere in the interior.
3. $V(r)=$constant everywhere in the interior

Note:
* CORRECT ANSWER: A

</section>
<section data-markdown>

### Summary of properties w/o proof

- $V$ has no local min/max except on boundaries
- $V$ is smooth and continuous everywhere
- $V$ at a location is equal to the average over any surrounding sphere: $V(\vec{r})=\iint_{sphere} Vda$
- $V$ is unique if you know boundary conditions
</section>

<section data-markdown>
![alt text](../images/d14-region_with_no_charge_Vset.png "Logo Title Text 1")


A region of space contains no charges. The boundary has V=0 everywhere.
What can I say about $V$ in the interior?

1. Not much, there are lots of possibilities for $V(r)$ in there
2. $V(r)=0$ everywhere in the interior.
3. $V(r)=$constant everywhere in the interior

Note:
* CORRECT ANSWER: B

</section>
<!--
<section data-markdown>

For the 1D Laplace problem ($\nabla^2 V = \partial^2 V/\partial x^2 = 0$), we can choose the following ansatz:

1. $k_0\,x$
2. $k_0\,x+k_1$
3. $k_0\,x^2+k_1\,x+k_2$
4. Can't tell

</section>
-->

<section data-markdown>

![alt text](../images/d14-cubical_lattice.png "Logo Title Text 1")



If you put a positive test charge at the center of this cube of charges, could it be in stable equilibrium?

1. Yes
2. No
3. ???

Note:
* CORRECT ANSWER: B

</section>

<section data-markdown>
Griffiths, in a minor parenthetical aside: "This, incidentally, suggests the method of relaxation, on which computer solutions to Laplace's equation are based..."

You know what this means, right?
</section>



<!--
<section data-markdown>

### Method of Relaxation

![alt text](../images/d14-convergence_relax.png "Logo Title Text 1")

</section>

<section data-markdown>

Consider a function $f(x)$ that is both continuous and continuously differentiable over some domain. Given a step size of $a$, which could be an approximate derivative of this function somewhere in that domain? $df/dx \approx$

1. $f(x_i+a) - f(x_i)$
2. $f(x_i) - f(x_i-a)$
3. $\frac{f(x_i+a) - f(x_i)}{a}$
4. $\frac{f(x_i) - f(x_i-a)}{a}$
5. More than one of these


Note:
* Correct Answer: E (C and D)
</section>

<section data-markdown>
If we choose to use:

$$\dfrac{df}{dx} \approx \dfrac{f(x_i+a) - f(x_i)}{a}$$

Where are we computing the approximate derivative?

1. $a$
2. $x_i$
3. $x_i + a$
4. Somewhere else

Note:
* Correct Answer: D (it's halfway between)

</section>

<section data-markdown>

Taking the second derivative of $f(x)$ discretely is as simple as applying the discrete definition of the derivative,

$$f''(x_i) \approx \dfrac{f'(x_i + a/2) - f'(x_i - a/2)}{a}$$

Derive the second derivative in terms of $f$.

</section>

<section data-markdown>

With the approximate form of Laplace's equation:

$\dfrac{V(x_i+a) - 2V(x_i) + V(x_i-a)}{a} \approx 0$

What is a the appropriate estimate of $V(x_i)$?

1. ${1}/{2}(V(x_i+a)-V(x_i-a))$
2. ${1}/{2}(V(x_i+a)+V(x_i-a))$
3. ${a}/{2}(V(x_i+a)-V(x_i-a))$
4. ${a}/{2}(V(x_i+a)+V(x_i-a))$
5. Something else

Note:
* Correct answer: B

</section>


<section data-markdown>

To investigate the convergence, we must compare the estimate of $V$ before and after each calculation. For our 1D relaxation code, $V$ will be a 1D array. For the kth estimate, we can compare $V_k$ against its previous value by simply taking the difference.

Store this in a variable called ``err``. What is the type for ``err``?

1. A single number
2. A 1D array
3. A 2D array
4. ???

Note:
* Correct Answer: B

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
-->
