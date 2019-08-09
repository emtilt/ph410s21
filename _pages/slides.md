---
layout: archive
title: "slides"
permalink: /slides/
author_profile: true
---



{% include base_path %}
{% for post in site.slides %}
    * [{{ post.title }}]({{ site.url }}{{ site.baseurl }}{{ entry.url }})
{% endfor %}


