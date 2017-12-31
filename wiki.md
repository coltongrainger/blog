---
title: wiki 
author: Colton Grainger
order: 2
---

<dl>
  {% for post in site.posts %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a>, <i>{{ post.date | date: "%Y-%m-%d" }}</i>
      </dt>
      <dd>
	{{ post.excerpt }}
      </dd>
  {% endfor %}
</dl>
