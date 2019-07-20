---
title: blog
order: 1
---

`2018-12-27` I have begun a [journal](https://journal.coltongrainger.com) for short, naive, and otherwise inchoate updates.

{% for post in site.posts %}
`{{ post.date | date: "%Y-%m-%d" }}` [{{ post.title }}]({{ post.url }})
{% endfor %}
