---
layout: page
title: "MPP Reflections"
permalink: /mpp-reflections/
---
A reverse chronological list of reflection posts from my one-year University of Calgary MPP program.

---

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a><br>
    <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
  </li>
{% endfor %}
</ul>
