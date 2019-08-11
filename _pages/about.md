---
permalink: /
title: "Syllabus"
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Course details are coming soon.
<!--[download this Jupyter notebook](jupyter/HW1-GradientProblem.ipynb) (you can [view it here](https://github.com/emtilt/ph410f19/blob/master/jupyter/HW1-GradientProblem.ipynb)-->
<img src="images/profile-b&w-lowquality.png" align="left" width="200" />

<pre><code data-trim data-noescape>
(def lazy-fib
  (concat
   [0 1]
   <mark>((fn rfib [a b]</mark>
        (lazy-cons (+ a b) (rfib b (+ a b)))) 0 1)))
</code></pre>

