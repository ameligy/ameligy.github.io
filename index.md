---
layout: default
---

<h2>Posts</h2>

<ul>
  {% for post in site.posts %}
    <li style="margin-bottom: 2em;">
      {% if post.cover_image %}
        <img src="{{ post.cover_image | relative_url }}" alt="Cover image" style="width:100%; max-width:400px;">
      {% endif %}
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <small>{{ post.date | date: "%b %-d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
