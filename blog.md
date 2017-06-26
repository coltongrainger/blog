---
layout: default
title: blog
order: 3
---

## Blog

<ul>
  {% for post in site.posts %}
    <li>
      <b>{{ post.date | date_to_string }}</b> <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
