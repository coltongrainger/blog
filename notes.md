---
title: notes 
author: Colton Grainger
order: 2
---

### service-work 
<dl>
{% for post in site.tags["service-work"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</dl>

### computing 
<dl>
{% for post in site.tags["computing"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</dl>

### math
<dl>
{% for post in site.tags["math"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</dl>

### writing
<dl>
{% for post in site.tags["writing"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</dl>

### data-management 
<dl>
{% for post in site.tags["data-management"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</dl>

### personal
<dl>
{% for post in site.tags["personal"] %}
      <dt>
	<a href="{{ post.url }}">{{ post.title }}</a> 
      </dt>
{% endfor %}
</dl>

## by date created 
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

## meta

From the OED
> *note, n.* 13. A brief record or abstract of facts written down for the purpose of assisting the memory, or to serve as a basis for a more complete or full statement; also transf., a recollection or mental impression of something. 

In use
> 1693 Humours Town 19 'Tis as necessary as Notes to the Parson in the Pulpit.

