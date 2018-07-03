---
title: latest
order: 1
---

{% for post in site.posts limit:3 %}
# [{{ post.title }}]({{ post.url }})

  <dl id="yaml_header_data">
    {% if post.author != nil %}
      <dt>author: {{ post.author }}</dt>
    {% endif %}

    {% if post.date != nil %}
      <dt>date: {{ post.date | date: "%Y-%m-%d" }}</dt>
    {% endif %}

    {% if post.revised != nil %}
      <dt>revised: {{ post.revised }}</dt>
    {% endif %}

    {% if post.belief != nil %}
      <dt>belief: <a href = "https://www.gwern.net/About#confidence-tags">{{ post.belief }}</a></dt>
    {% endif %}

    {% if post.status != nil %}
      <dt>status: {{ post.status }}</dt>
    {% endif %}
  </dl>

{{ post.content }}
<br><br>

{% endfor %}
[older posts](/archive)
