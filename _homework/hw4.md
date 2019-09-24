---
layout: archive
collection: homework
title: "Homework 4 - Due Friday, September 27 at 4:30pm"
permalink: /homework/hw4/
author_profile: true
---
[Link to Slack team -- a great place to ask questions](https://ph410f19.slack.com)

Homework 4 emphasizes another alternative method to direct integration for solving the electric field problem by reducing the vector problem to a scalar one by using electric potential. In addition, it introduces the electric potential energy concept. This homework emphasizes 2.3 and 2.4, but Sec. 2.2 (Gauss’ Law) continues to be very important.


### 1. Overlapping clouds of charge

When solving some E&M problems, you will need to develop your solution using an arbitrary location. In this problem, consider how choosing an arbitrary point in the overlapping region of the charge clouds will help you derive the result.

![Overlapping Clouds](../../images/hw4-overlapping_clouds.png "Overlapping Clouds")
1. Consider two oppositely charged clouds (radii, $R$), both with known uniform charge densities. They overlap as in the figure, with their centers separated by $d$. Find the electric field in the overlapping region. (*Hint: Consider how Gauss' Law and superposition can help here. You should already know how to find the field inside each sphere separately -- is there a way to use that knowledge?*)
2. In this overlapping region, sketch the electric field lines.
3. In the limit that $d$ becomes very small compared to $R$, discuss in words and make a sketch of what the resulting (total, physical) charge distribution in space really looks like. Is this similar in any way to the physical situation in some other system that you have studied before? (So that later in the course when we encounter such a charge distribution, we will know where it came from and what the electric field looks like inside!)

### 2. Allowed Fields
1. If $c$ is a constant, which one of the following two static E-fields is physically impossible. Why?
  -  $\mathbf{E}=c\left(x\hat{x}+z\hat{y}+y\hat{z} \right)$
  -  $\mathbf{E}=c\left(x\hat{x}+2z\hat{y}+y\hat{z} \right)$
2. For the field that **is** possible, find the potential $V(\vec{r})$, using the origin as your reference point (i.e., setting $V(0)=0$). (Hint: You must select a specific path to integrate along. It doesn't matter which path you choose, since the answer is path-independent, but you can't compute a line integral without having a particular path in mind, so be explicit about that in your solution.)
3. Check your answer two ways: by explicitly computing the gradient of V and by checking that it gives the correct result at a particular point for which you already know the potential. 


### 3. Finding voltage from a charge distribution
1. Find the electrostatic potential $V(0,0,z)$ everywhere along the symmetry-axis of a charged ring (radius $a$, in the $x-y$ plane centered on the $z$-axis, with uniform linear charge density $\lambda$ around the ring).  Use the method of direct integration (Griffiths Equation 2.30, on p. 85) to do this, and set your reference point to be $V(\infty)=0$.   
2. Use this V(0,0,z) to find the z-component of the E field anywhere along the $z$-axis. We have already derived this result directly from Coulomb's law, so you should be able to confirm your answer.
3. Sketch $V(z)$ and $E_z(z)$ for points on the $z$-axis (both $z<0$ and $z>0$, being careful of the sign). Briefly comment on your results for $V$ and $E_z$ right at the origin – do they make physical sense to you, and are they consistent with each other?   
4. How does $V(z)$ behave as $z\rightarrow\infty$ ? Don't just say it goes to 0. **How** does it go to zero? Does your answer make physical sense to you? Briefly explain. 

### 4. Calculating voltage from $\vec{E}$
1. Show, via Gauss's Law, that the electric field a distance $s$ from an infinitely long straight wire that carries a uniform line charge $\lambda$ is $\mathbf{E}=2\lambda\vec{s}/4\pi\epsilon_0s^2$.
2. Find the potential $V(s)$ for points a distance $s$ away from the $z$-axis. (Hint: You will have to be careful to compute a difference of potentials between two points, perhaps introducing some arbitrary $s_0$ to your solution, to avoid integrals which are infinite.)
3. Check your answer by explicitly taking the gradient of $V$ to make sure it gives you $E$. 
4. Briefly discuss the question of "reference point": where did you set $V=0$? Can you use $s=\infty$, or $s=0$, as the reference point, $V(s)=0$, here? Why is there trouble with setting $V(\infty)=0$? (our usual choice), or $V(0)=0$ (often our second choice)?
5. How would your answer change if I told you that I wanted you to set $V=0$ at a distance $s=3 \rm m$ away from the $z$-axis?  


### 5. Estimation
I've made y'all due a bunch of programming because it is a crucial skill for a physical scientist. This week, we're taking a break from programming, but this problem is about another important skill. The ability to obtain rough estimations that are correct to about an order of magnitude is one of the most important skills a physicist can have. Ideally, a physicist should be able to come up with a correct order-of-magnitude estimate to any question at all with no calculator or uncommon numerical facts. Your goal in this problem is the make a *very rough* estimate of the voltage difference a across a distance the size of your heart when you hear thunder from a storm.

**Here's the actual problem:** A typical Colorado lightning bolt might transfer a few Coulombs of charge in a stroke. Although lightning is clearly not remotely "electrostatic", let's pretend it is - consider a brief period during the stroke, and assume all the charges are fairly uniformly distributed in a long thin line. If you see the lightning stroke, and then a few seconds later hear the thunder, make a very rough estimate of the resulting voltage difference across a distance the size of your heart. 

**Hints:** What simplified model should you use? I'm imagining a lightning strike as looking rather like a long uniform line of charge. You've done the "physics" of this in the previous problem.  But you still need an estimate of $\lambda$. How long might that lightning bolt be? For estimation problems, don't worry about any small details; you just want to be within about an order of magnitude of the correct answer. An error of a factor of 3 is fine, but an error of a factor of 3000 makes your answer useless. Make crude, but reasonable, approximations! One number that will be helpful to consider is the speed of sound; many people have this memorized as about $v_{sound}\sim 300 m/s$ (though you *could* make a rough estimate even of this number based on everyday stuff). It's also helpful in life to have a very small number of very common Taylor series memorized, like $\ln (1+x)\sim x$ for small $x$, as well as the rough order of magnitude of constants like Coulomb's $k\sim10^{10}$ in SI units (although, you could estimate even this!). You shouldn't really need anything else for this problem, though your thinking may range across many topics. My solution will mention airplanes and skyscrapers when I deduce $\lambda$.

**Encouragement:** I, of course, can't check *how* you went about solving this problem (e.g., I can't check if you used a calculator or looked up properties of storms). But I encourage you to engage in the *spirit* of this problem; look up nothing, use no computer or calculator, and [approximate aggressively](https://www.xkcd.com/2205/) but cleverly. (If you go to just the right sort of parties, estimation is a great party trick. It's relatively easy to immediately deduce the correct diameter of the earth, nmumber of piano tuners in LA, and speed of the continental drift off the top of your head.)


### 6. Energy of a point charge distribution

When studying crystal structures (e.g., in condensed matter physics), it is sometimes convenient to model those structures as rectangular grids of charged ions, this problem offers a starting point for such a model.

Imagine a small square (side $a$) with four point charges $+q$, one on each corner.

1. Calculate the total stored energy of this system (i.e. the amount of work required to assemble it).
2. Calculate how much work it takes to "neutralize" these charges by bringing in one more point charge ($-4q$) from far away and placing it right at the center of this square.


### 7. Screened Coulomb Potential

We've seen the electric field and charge distribution for a point charge using the electric potential.  In this problem, you will gain some additional practice doing this for the [screened Coulomb potential](https://en.wikipedia.org/wiki/Electric-field_screening).

Consider the "screened Coulomb potential" of a point charge $q$ that arises, for example, in plasma physics:

$$V(r) = \dfrac{q}{4\pi\varepsilon_0} \dfrac{e^{-r/\lambda}}{r}$$

where $\lambda$ is a constant (called [the screening length or Debye length](https://en.wikipedia.org/wiki/Debye_length)).

1. Determine the electric field $\mathbf{E}(\mathbf{r})$ associated with this potential.
2. Find the charge distribution $\rho(\mathbf{r})$ that produces this potential. (Hint: Think carefully about what happens at the origin. Will your answer therefore necessarily contain a certain special distribution function that we've talked about at length?)
3. Sketch this function $\rho(\mathbf{r})$ in a manner that clearly describes its characteristics. Label how the function is bhaving in different region (e.g., at $r=0$, near $r=0$, in the far-field).
4. Show, by explicit calculation over $\rho(\mathbf{r})$ that the net charge represented by this distribution is zero. (*If you don't get zero, think again about what happens at $r = 0$.*).
5. Verify this result using the integral form of Gauss' Law (i.e., integrate your electric flux over a *very large* spherical surface.)

### 8. Surface charge and boundary conditions

It might seem to you that the results that the electric field is discontinuous by an amount $\sigma/\varepsilon_0$ isn't really a big deal. There's probably a question about how useful this result is. We will come back to this particularly when we get to fields in matter, and suffice it to say, it will help us a lot there. To get a flavor of what is coming, this problem will discuss this discontinuity in a familiar context.

1. Consider a cylindrical metal rod (radius $r$, length $L$) with a constant charge density $\sigma$ distributed across its outer surface (as a conductor, that is the only place the charge can be). Using Gauss' Law (far from the ends of the rod; assume it's long and skinny), determine the electric field inside and outside the rod.
2. Take the difference between the electric fields you determined in Part 1 (technically, the perpendicular component) across the outer surface of the metal rod to show you recover the the result that the all the charge lives on the surface.
3. Consider a similarly cylindrical plastic rod with a constant charge density $\rho$ distributed over its entire volume. Again, using Gauss' Law (far from the ends of the rod; assume it's long and skinny), determine the electric field inside and outside the rod.
4. Again, take the difference between the electric fields you determined in Part 3 across the outer surface of the plastic rod. What do you find? Does your result make physical sense?
