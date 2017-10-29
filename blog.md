---
title: blog
author: Colton Grainger
order: 3
---

# Recent Posts
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>, <i>{{ post.date | date: "%Y-%m-%d" }}</i>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

