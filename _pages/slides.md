---
layout: archive
title: "slides"
permalink: /slides/
author_profile: true
---



{% include base_path %}
{% for post in site.slides %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ entry.url }}" title="{{ post.title | escape }}">{{ post.title }}</a></li>{% endfor %}
{% endfor %}



<!--
{% include loop-category category='slides' %}

{% for entry in site.categories[include.category] %}
<li><a href="{{ site.url }}{{ site.baseurl }}{{ entry.url }}" title="{{ entry.title | escape }}">{{ entry.title }}</a></li>{% endfor %}
-->
