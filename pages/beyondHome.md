---
layout: page
title: "Beyond the paper"
subheadline: "This wasn't supossed to be here"
teaser: ""
permalink: /beyond/
---
In this section you can find those experiments that do not fit the original idea of this project, but also make sense as fun and learning.
For now it is empty, but surely end up doing something with arduino or possibly, some simple wearables.
in the meantime, you can take a look to [make] [1] or [hackster.io][2]



 [1]: http://makezine.com/category/technology/arduino/
 [2]: https://www.hackster.io/wearables


 
{% assign items = site.posts | sort: 'date' %}
<ul>
{% for post in items  %}
  {% if post.tags contains 'beyond' %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>
  {% endif %}
{% endfor %}
</ul>
