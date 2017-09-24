---
title: blog
author: Colton Grainger
order: 3
---

This page is pretty scarce until I salvage some notes & journal entries. I've taken equal parts of time (i) to develop a relationship with an implied reader[^who] and (ii) to set up the medium to do so. 
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>, <i>{{ post.created | date_to_string }}</i>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

<hr>

[^who]: For [Wolfgang Iser](https://en.wikipedia.org/wiki/Wolfgang_Iser), the *implied reader* is "a textual structure anticipating the presence of a recipient without necessarily defining [them]…the concept of the implied reader designates a network of response-inviting structures, which impel the reader to grasp the text."
