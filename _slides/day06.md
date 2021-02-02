---
title: "Day 6 - Numerical integration"
permalink: /slides/day06
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
### PH410 - Electromagnetism

Feb 1
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>
<section data-markdown>
While waiting for class to start, answer this. It's a reminder for HW2 -- remember your physics 1! 
	
![hanging charges](../images/d6-hungspheres.png "hanging charges") 
	
Two small spheres (mass, $m$) are attached to insulating strings (length, $L$) and hung from the ceiling as shown.

How does the angle (with respect ot the vertical) that the string attached to the $-q$ charge ($\theta_1$) compare to that of the $-2q$ charge ($\theta_2$)?

1. $\theta_1 > \theta_2$
2. $\theta_1 = \theta_2$
3. $\theta_1 < \theta_2$
4. ????

Note:
CORRECT ANSWER: B
Draw the FBD, Newton 3 is important here.

</section>
<section data-markdown="">

### For Friday
- Read Griffiths 2.2
- Reading survey due at 9am 
- HW2 due
	
"Now that we have experience what the coding homework is like, it was pretty challenging. What are your recommendation in working with coding? (resources? classmates, office hours, etc.)" **>> All of the above, but, even more important, start early. You aren't going to have time to thoroughly think through these problems if you don't use the whole week to do so. If you started late and sought no help, then you didn't follow any of my advice!**
</section>
<section data-markdown>

## Numerical Integration

![alt text](../images/d5-numerical_midpoint.gif "Logo Title Text 1")

</section>

<section data-markdown>

Consider this trapezoid

![alt text](../images/d5-trapezoid_shape.png "Logo Title Text 1")

What is the area of this trapezoid?

1. $f(c)h$
2. $f(d)h$
3. $f(c)h + \frac{1}{2}f(d)h$
4. $\frac{1}{2}f(c)h + \frac{1}{2}f(d)h$
5. Something else

Note:
* Correct Answer: D
</section>

<section data-markdown>

The trapezoidal rule for a function $f(x)$ gives the area of the $k$th slice of width $h$ to be,

$$A_{k} = \frac{1}{2}h\left(f(a+(k-1)h) + f(a+kh)\right)$$

What is the approximate integral, $I(a,b) = \int_a^b f(x) dx$, $I(a,b) \approx$

1. $\sum_{k=1}^N \frac{1}{2}h\left(f(a+(k-1)h) + f(a+kh)\right)$
2. $h\left(\frac{1}{2}f(a) + \frac{1}{2}f(b) + \frac{1}{2}\sum_{k=1}^{N-1}f(a+kh)\right)$
3. $h\left(\frac{1}{2}f(a) + \frac{1}{2}f(b) + \sum_{k=1}^{N-1}f(a+kh)\right)$
4. None of these is correct.
4. More than one is correct.

Note:
* Correct Answer: D (both A and C)

</section>

<section data-markdown>

The trapezoidal rule takes into account the value and slope of the function. The next "best" approximation will also take into account:

1. Concavity of the function
2. Curvature of the function
3. Unequally spaced intervals
4. More than one of these
5. Something else entirely

</section>
<section data-markdown>

![alt text](../images/d5-simp.png "Source: https://www.value-at-risk.net/numerical-integration-in-one-dimension/")

</section>



