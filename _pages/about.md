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
Test this image 
<img src="./images/profile.png" align="left" style="width: 100px"; />
<pre><code data-trim data-noescape>
(def lazy-fib
  (concat
   [0 1]
   <mark>((fn rfib [a b]</mark>
        (lazy-cons (+ a b) (rfib b (+ a b)))) 0 1)))
</code></pre>
