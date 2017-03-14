---
layout: page
title: "Getting Started"
subheadline: "Your first visit? Welcome!"
teaser: ""
permalink: /gettingStarted/
---






{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}
{% assign items = posts | sort: 'date' %}
<ul>
{% for post in items  %}
  {% if post.tags contains t %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>
  {% endif %}
{% endfor %}
</ul>
{% endfor %}