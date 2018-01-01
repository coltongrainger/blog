---
title: wiki 
author: Colton Grainger
order: 2
---

### Service Work 
<ul>
{% for post in site.tags["service-work"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</ul>

### Computing 
<ul>
{% for post in site.tags["computing"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</ul>

### Math 
<ul>
{% for post in site.tags["math"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</ul>

### Writing
<ul>
{% for post in site.tags["writing"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</ul>

### Data Management
<ul>
{% for post in site.tags["data-management"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</ul>

### Personal
<ul>
{% for post in site.tags["personal"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</ul>

### Chronological
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
