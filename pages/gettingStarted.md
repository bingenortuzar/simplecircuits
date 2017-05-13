---
layout: page
title: "Getting Started"
subheadline: "Your first visit? Welcome!"
teaser: ""
permalink: /gettingStarted/
---






{% assign items = site.posts | sort: 'date' %}
<ul>
{% for post in items  %}
  {% if post.categories contains 'intro' %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>
  {% endif %}
{% endfor %}
</ul>
