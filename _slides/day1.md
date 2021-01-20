---
title: "Day 1 - Course Introduction"
permalink: /slides/day1
layout: slide
theme: white
transition: slide
spotifyplaylist: embed/playlist/0Q3VleFxIlnKZMoeC75aNn
---

<section data-markdown="">
	
### PH410 - Electromagnetism

January 20
<!--this doesn't work... {% include spotifyplaylist.html id=page.spotifyplaylist %}-->
</section>


<section data-markdown="">

### I'm Evan (he/him/his)

- Office: Carroll 108C
    - Probably not in pandemic...
- Email: &lt;etilton@regis.edu&gt;
    - Try not to use email except for personal matters...

Who are y'all?

</section>

<section data-markdown="">

### Committment to an Inclusive Classroom

I'm committed to creating an inclusive classroom.  If I can do anything to make the classroom a better learning environment for you, please let me know.

If you observe or experience behaviors that violate our committment to inclusivity, please let me know.

If I violate this principle, please let me know or please tell the physics chair. I want to learn from my mistakes!

</section>

<section data-markdown="">

### Confidentiality and Mandatory Reporting

One of my responsibilities is to help create a safe learning environment. It is my goal that you feel able to share information related to your life experiences. I will seek to keep information you share private.

However, I'm required to share information regarding sexual misconduct, relationship violence, or information about criminal activity with the university.

Students may speak to someone confidentially by contacting the Office of Counseling and Personal Development. OCPD is located in the Coors Life Direction Center, Room 114 and can be contacted by phone 24/7 at 303-458-3507. See www.regis.edu/ocpd.

</section>

<section data-markdown="">
	
### Important Sites

* Course Webpage: [evantilton.com/ph410s21](http://evantilton.com/ph410s21)
* Slack Team: [physicsatregis.slack.com](http://physicsatregis.slack.com)
  * *You should already be a part of this.*

</section>

<section data-markdown="">

### Books

| Required | Highly Optional |
| :---: | :---: |
| ![griffiths book](../images/griffiths.png "griffiths book") | ![Div Grad Curl book](../images/divgradcurl.jpg "Div Grad Curl book") |

</section>



<section data-markdown="">

### Course Activities
* Midterm Exams (2 of them, format TBD, likely some combo of in-person, oral, and/or remote depending on pandemic) - 15% each
* Final Exam  - 20%
* Homework (Lots of it; mostly due on Fridays) - 40%
* Participation (Reading quizzes, polls, etc) - 10%

[Much more detail on website](http://evantilton.com/ph410s21)

</section>


<section data-markdown="">
	
### Exam corrections

Exams can be very stressful. However, I'll try to come up with the least stressful formats I can.

If we have written exams, then there will be an opportunity to correct and reflect upon your mistakes for credit.
</section>

<section data-markdown="">

## This Week!!!

* Homework 1 is already up (due a week from Friday at 4:30 pm)
* Read (seriously do this!) Griffiths Advertisement (pp. xiv-xviii) and Sections 1.1 & 1.2 (pp. 1-24)
* Reading survey on WorldClass due by 9am before each class for which we have one
* Get Python, Slack, and Github working

**Stay up-to-date by checking website, calendar, and Slack regularly.**

*Chapter 1 of Griffiths should be mostly review.*

</section>

<section data-markdown="">

### Homework problems

* We will be using Python on homework problems this semester. You are welcome to use any distribution, but I recommend [Google Colab](https://colab.research.google.com) or [Anaconda](https://www.continuum.io/downloads)
* Computational homework questions will take the form of a Jupyter notebook, which you can turn in by adding them to the Github repository.
* If you get stuck somewhere, post on Slack, so your classmates benefit from your question. Use the channels and giphy responsibly.
* Regular homework should be handwritten. Alternately, you are welcome to typeset it in LaTeX or Markdown, but I won't accept it unless you typeset using standard mathematical notation and convention.

</section>

<section data-markdown="">
	
### Personal Integrity

Let's talk about what that means for class, exams, and homework.

</section>

<section data-markdown="">
	
### Advice 

What advice do you have for each other?

</section>



<section data-markdown="">

## What do you think PH410 is about?

</section>


<section data-markdown="">

### Electromagnetism is the foundational field theory of physics

Think about everything you already know about electromagnetism (it's a lot already!).

Work with a partner to map out the electromagnetism concepts that you know and how they are related to each other. 

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
