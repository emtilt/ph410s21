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
<img src="profile-b&w-lowquality.png" align="left" width="200" />
<pre><code data-trim data-noescape>
(def lazy-fib
  (concat
   [0 1]
   <mark>((fn rfib [a b]</mark>
        (lazy-cons (+ a b) (rfib b (+ a b)))) 0 1)))
</code></pre>
