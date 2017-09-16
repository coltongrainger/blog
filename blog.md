---
title: posts
author: Colton Grainger
order: 3
---

This page is pretty scarce until I salvage some handwritten journal entries. I've taken equal parts of time (i) to find a general audience and (ii) to communicate with one.
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>, <i>{{ post.created | date_to_string }}</i>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
