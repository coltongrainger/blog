---
title: web blog
author: Colton Grainger
---

<dl>
  {% for post in site.posts %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a>, {{ post.date | date: "%Y-%m-%d" }}
      </dt>
      <dd>
	{{ post.excerpt }}
      </dd>
  {% endfor %}
</dl>
