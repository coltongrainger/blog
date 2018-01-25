---
title: all pages 
author: Colton Grainger
order: 2
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

## meta

Right now I'm not using a tag cloud (doing so would be [premature optimization](http://wiki.c2.com/?PrematureOptimization)). That is, until I have momentum in a career/field of research, I see tags as a noncritical part of my writing. Analogously, from Knuth,
> Programmers waste enormous amounts of time thinking about, or worrying about, the speed of noncritical parts of their programs, and these attempts at efficiency actually have a strong negative impact when debugging and maintenance are considered.

For me, the "debugging and maintenance" is as revising and moving around old information. So no tag cloud.

But, just to sketch an idea of what themes I *would like* to write on, here some exemplar tag clouds (all of which, I think, were carefully designed well after the initial seed to write for a general audience had germinated).

[Matt Might](matt.might.net/articles/)'s tag cloud
> Functional Programming; Graduate School; Productivity; iPhone, iPad, iPod; HOWTOs; Undergraduate Computer Science; Parsing; Compilation; Mathematics; Writing; Giving Presentations; Lambda Calculus; C; C++; Scheme; Racket; JavaScript; Swift; Python; Perl; Java; Scala; LaTeX; ML; SQL; Haskell; Scripting; Lambda; Apple; Unix; Web servers; Security; Hacks; Travel; Academia; Teaching; Science; Health; Gadgets; Gaming; Home Improvement; Rants

[Jean Yang](http://jxyzabc.blogspot.com/)'s tag cloud
> gender (48), life (47), women in science (37), academic advice (31), programming languages (29), programming (19), food (16), research (15), academic culture (14), travel (13), advice (9)

a subset of the "math" prefixed [arXiv categories](https://arxiv.org/archive/math)[^order]
> AG Algebraic Geometry, AT Algebraic Topology, CT Category Theory, CA Classical Analysis and ODEs, CV Complex Variables, DG Differential Geometry, DS Dynamical Systems, FA Functional Analysis, GN General Topology, GT Geometric Topology, HO History and Overview, KT K-Theory and Homology, LO Logic, MP Mathematical Physics, NT number theory, NA numerical Analysis, OC Optimization and Control, PR Probability, ST Statistics Theory, SG Symplectic Geometry

[^order]: It might be fun to order these by asking: In which categories am I likely to find a related job after grad school? Mathematical Physics? Numerical Analysis? Statistics Theory? Optimization and Control?
