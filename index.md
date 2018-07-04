---
title: latest
order: 1
---

{% for post in site.posts limit:3 %}

`{{ post.date | date: "%Y-%m-%d" }}` [{{ post.title }}]({{ post.url }})

{{ post.excerpt }}

{% endfor %}

*[older posts](/archive)*
