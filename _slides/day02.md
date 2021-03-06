---
title: "Day 2 - What is E&M, Vector Calc"
permalink: /slides/day02
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
		
### PH410 - Electromagnetism

Jan 22
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>


<section data-markdown="">

### For Monday
- Read Griffiths Sections 1.3 and 1.4
- Do reading survey by 9am on Monday (on WorldClass)
	
</section>

<section data-markdown="">
	
## Textbook stuff
### Errata
https://www.reed.edu/physics/faculty/griffiths/
### Remember to read actively!
Have a pen & paper, work things out and check things!
</section>

<section data-markdown="">

### Have you looked at the homework?
1. No, I haven't looked at it.
2. Yes, I looked at it but did none of it.
3. Yes, I did the computer setup, but nothing else.
4. Yes, I did some of the problems, but not the computer setup.
5. I've made progress on both the computer setup and the problems.

</section>




<section data-markdown="">

## What do you think PH410 is about?

</section>

<section data-markdown="">

### Electromagnetism is the foundational field theory of physics

Think about everything you already know about electromagnetism (it's a lot already!).

<!-- Work with a partner to map out the electromagnetism concepts that you know and how they are related to each other. -->

</section>
<section data-markdown>

## Mathematical Preliminaries

$\nabla \cdot \mathbf{E}=\frac{\rho}{\epsilon_{0}} \qquad \oint \mathbf{E} \cdot d \mathbf{a}=\frac{Q_{\mathrm{enc}}}{\epsilon_{0}}$


$\nabla \cdot \mathbf{B}=0 \qquad \oint \mathbf{B} \cdot d \mathbf{a}=0$


$\nabla \times \mathbf{E}=\color{gray}{-\frac{\partial \mathbf{B}}{\partial t}} \qquad \oint \mathbf{E} \cdot d \mathbf{l}=\color{gray}{-\int \frac{\partial \mathbf{B}}{\partial t} \cdot d \mathbf{a}}$


$\nabla \times \mathbf{B}=\mu_{0} \mathbf{J}\color{gray}{+\mu_{0} \epsilon_{0} \frac{\partial \mathbf{E}}{\partial t}} \qquad \oint \mathbf{B} \cdot d \mathbf{l}=\mu_{0} I_{\mathrm{enc}}\color{gray}{+\mu_{0} \epsilon_{0} \int \frac{\partial \mathbf{E}}{\partial t} \cdot d \mathbf{a}}$


Note:
There's a reason that we are starting with vectors and vector operations; it's inherent in the way electromagnetism is described!
</section>

<section data-markdown="">
	
Two charges $+Q$ and $-Q$ are fixed a distance $r$ apart. The direction of the force on a test charge $-q$ at point A is:

![alt text](../images/d2-twocharge.png "Logo Title Text 1") 

Note:
* CORRECT ANSWER:  A
* Use superposition
</section>

<section data-markdown>

In a typical Cartesian coordinate system, vector $\mathbf{A}$ lies along the $+\hat{x}$ direction and vector $\mathbf{B}$ lies along the $-\hat{y}$ direction. What is the direction of $\mathbf{A} \times \mathbf{B}$?

1. $-\hat{x}$
2. $+\hat{y}$
3. $+\hat{z}$
4. $-\hat{z}$
5. Can't tell

Note:
* Correct Answer: D
* Use the right-hand rule
* Fall 2016: 0 0 23 [77]

</section>

<section data-markdown>

<!--_**Skipped in class, good review.**_-->
In a typical Cartesian coordinate system, vector $\mathbf{A}$ lies along the $+\hat{x}$ direction and vector $\mathbf{B}$ lies along the $-\hat{y}$ direction. What is the direction of $\mathbf{B} \times \mathbf{A}$?

1. $-\hat{x}$
2. $+\hat{y}$
3. $+\hat{z}$
4. $-\hat{z}$
5. Can't tell

Note:
* Correct Answer: C
* Use right-hand rule; means $\mathbf{A} \times \mathbf{B} = - \mathbf{B} \times \mathbf{A}$
* Fall 2016: 0 0 [94] 6 0
</section>

<section data-markdown>
<!--_**Skipped in class, good review.**_-->
How is the vector $\mathfrak{R}_{12}$ related to $\mathbf{r}_1$ and  $\mathbf{r}_2$?

![alt text](../images/d2-rvec.png "Logo Title Text 1") 

1. $\mathfrak{R}_{12} = \mathbf{r}_1 +\mathbf{r}_2$
2. $\mathfrak{R}_{12} = \mathbf{r}_1 - \mathbf{r}_2$
3. $\mathfrak{R}_{12} = \mathbf{r}_2 - \mathbf{r}_1$
4. None of these

Note:
* CORRECT ANSWER:  C

</section>


<section data-markdown="">
	
In terms of primed and/or unprimed vector names using Griffiths-style notation, what is the magnitude of vector B if P is some point at which you need to find the electric field due to the point charge at C? Which names should A, B, and C have accoridng to Griffiths notation?

![alt text](../images/d2-scriptrpointcharge.png "Logo Title Text 1") 

Note:

</section>

