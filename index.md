---
title: home
author: Colton Grainger
order: 1
# date: 2017-09-15
# created: 2017-07-15
---
<img src="images/ccg-dogs.jpg" style="float: right; margin: 0px 0px 23px 23px" height="150" width="150">
   
# Colton Grainger

This is the personal website of Colton Grainger.
<hr>

I am coordinating the [volunteer program](http://coltongrainger.com/fscss-volunteers) for a family homeless shelter in Olympia, WA. 

Additionally, I am reviewing [Probabilty](http://webpages.uidaho.edu/cremien/math451EO/) and [Ordinary Differential Equations](http://www.webpages.uidaho.edu/~barannyk/Teaching/Math310.html).

## Recent Posts

{% for post in site.posts %}
  <a href="{{ post.url }}">{{ post.title }}</a><br> {{ post.date | date: "%Y-%m-%d"}}<br>
{% endfor %}

## Contact

- Email: [colton.grainger@gmail.com](mailto:colton.grainger@gmail.com)
- Twitter: [@coltongrainger](https://twitter.com/coltongrainger)
- Here's my <a href="images/ccg-profile.png">photo</a>.
