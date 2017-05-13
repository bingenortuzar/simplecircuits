---
layout: page
title: "Theory Behind"
subheadline: "Trying to understand 'why'"
teaser: ""
permalink: /theory/
---

I have to start this section wir a big DISCLAIMER. You can expect a lot of simplifications and therefore misinformation. My electrical knowledge is limited (at most). 


{% assign items = site.posts | sort: 'date' %}
<ul>
{% for post in items  %}
  {% if post.categories contains 'theory' %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>
  {% endif %}
{% endfor %}
</ul>
