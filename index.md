---
title: blog
order: 1
---

`2019-01-01--Present` I have begun a [<i class="fas fa-images"></i> working journal](https://journal.coltongrainger.com) for naive/raw/inchoate and otherwise unsuitably written material.

{% for post in site.posts %}
`{{ post.date | date: "%Y-%m-%d" }}` [{{ post.title }}]({{ post.url }})
{% endfor %}
