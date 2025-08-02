---
layout: default
title: "Ahmed Elmeligy's Blog"
---

<h1>{{ page.title }}</h1>

<p>Engineer. Policy Leader. Storyteller. This blog explores the intersection of technical problem solving and public impact.</p>

<hr>

{% for post in site.posts %}
<div style="border-bottom: 1px solid #ccc; padding: 1em 0;">
  <h2 style="margin-bottom: 0.2em;">
    <a href="{{ post.url | relative_url }}" style="text-decoration: none; color: #2a7ae2;">{{ post.title }}</a>
  </h2>
  <small style="color: #666;">{{ post.date | date: "%B %d, %Y" }}</small>
</div>
{% endfor %}
