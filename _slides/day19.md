---
title: "Day 19 -  Starting laplace's equation"
permalink: /slides/day19
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Mar 3<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown="">

### No reading for Monday

### HW6 due friday	
</section>

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
