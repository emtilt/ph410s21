---
title: "Day 4 - Vector Calc, part 3"
permalink: /slides/day04
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">

### PH410 - Electromagnetism

Jan 27


### For Friday
- No reading
- Homework 1 due @ 4:30 on Github

<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->

</section>
<section data-markdown>
"How often will we use cylindrical coordinates?" **>>> We'll use all three systems quite a bit, though I'd say that cyllindrical gets used less than the other two by a small margin.**
</section>

<section data-markdown>

![alt text](../images/d3-cylindrical.png "Logo Title Text 1") 

In cylindrical (2D) coordinates, what would be the correct description of the position vector $\mathbf{r}$ of the point P shown at $(x,y) = (1, 1)$?

1. $\mathbf{r} = \sqrt{2} \hat{s}$
2. $\mathbf{r} = \sqrt{2} \hat{s} + \pi/4 \hat{\phi}$
3. $\mathbf{r} = \sqrt{2} \hat{s} - \pi/4 \hat{\phi}$
4. $\mathbf{r} = \pi/4 \hat{\phi}$
5. Something else entirely

Note:
* CORRECT ANSWER:  A
* The position vector is different from the coordinates! The point P has r=Sqrt[2], phi=pi/4, but it is certainly not the case that, e.g. B would be the position vector. The units aren’t even correct!
* Fall 2016: [6] 90 3 0 1; Second vote (discussion and hint about units): [54] 35 4 1 4

</section>
<section data-markdown>

![alt text](../images/d3-spherical.png "Logo Title Text 1") 

### You derive it

Consider the radial unit vector ($\hat{r}$) in the spherical coordinate system as shown in the figure.

Determine the $z$ component of this unit vector in the Cartesian $(x,y,z)$ system as a function of $r,\theta,\phi$.


Note:
This demonstrates that the r unit vector is a curious thing, in fact in contains all the information that is needed to define where you on the unit sphere. The other vectors can be though of as defined relative to that.
Altered for F2017 to be shorter, only work on z component
</section>



<section data-markdown>
![alt text](../images/d3-spherical2.png "Logo Title Text 1") 

In spherical coordinates, what would be the correct description of the position vector $\vec{r}$ of the point P shown at $(x,y,z) = (0,2~{\rm m},0)$?
1. $\vec{r}=(2~{\rm m})\hat{r}$
2. $\vec{r}=(2~{\rm m})\hat{r}+\pi\hat{\theta}$
3. $\vec{r}=(2~{\rm m})\hat{r}+\pi\hat{\theta}+\pi\hat{\phi}$
4. $\vec{r}=(2~{\rm m})\hat{r}+\pi\hat{\theta}+\frac{\pi}{2}\hat{\phi}$
5. something else

Note:
The position vector points in the “r” direction! There was a lot of discussion about this, it was clearly confusing to them. Answer D has nonsensical units. And it says that r vector has a “down” component over there. Demo: pick a coordinate system in the room and had everyone “point” in the rhat, and then phi-hat, directions, to show them that these are not constants, they are different for everyone in the room. “r_hat” has a “hidden notation”, it’s really “r_hat(r,theta,phi)”. 
Potential questions: COULD a vector have a thetahat or phihat component (how about VELOCITY of a point passing DOWN at P?) Could we could “fix it up” by putting meters in with the Pi/2’s… ?(Not in this case, A is correct). Answer A is ALSO the answer for OTHER points on that sphere, that’s right, R=2 m r_hat is by itself NOT sufficient. Writing r = (r, theta, phi) is fine, describing a point in spherical components, those three “bits” of information are what you need, but that notation is NOT the same as the cartesian, it is not saying “r r_hat + theta theta_hat + phi phi_hat”) 
  
WRITTEN BY:  Steven Pollock (CU-Boulder) This comes from research by Brant Hinrichs, it’s a known student difficulty. 

</section>
