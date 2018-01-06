---
title: Personal statement for grad apps
author: Colton Grainger
date: 2017-11-23
modified: 2018-01-04
status: draft
belief: likely
mathjax: true
tags: 
  - math
---

The robustness of a mathematical method determines its utility. Just
imagine designing a communication network that fails to account for
topological perturbations, or modeling an epidemic with strictly
deterministic differential equations. My goal, then, is to study robust
methods in algebraic topology and apply them in abstract and
computational settings.

For example, consider training an AI to distinguish the tone signature
of different musical instruments. Applying persistent homology, we
associate holes in an audio recording’s time-delay phase-space with a
sample statistic: the persistent rank function (PRF). Corresponding with
Nikki Sanderson, I learned a computer trained on PRFs more accurately
classifies tone signatures than one trained on Fast Fourier Transforms.
Here, a topological invariant answers the question “which instrument?”
with higher fidelity than the Fourier Transform.

My research interest stems from (i) my exposure to topology and its
applications as a college senior, and (ii) insight from two years of
service work since graduating.

Advised by Dr. Jonny Comes, my senior independent study[^1] examined how
Galois theory constrains the solution space of Fuchsian-type DiffEqs.
Following Michio Kuga, we developed a correspondence between the
fundamental group on $D = \mathbf{C}\setminus\{x_1,\ldots,x_n\}$ and
this region’s universal covering space $\tilde{D}$. Exploiting the
representation of the group of covering transformations
$\Gamma(\tilde{D} \to \tilde{D})$ as a group of linear automorphisms, I
parameterized solutions to the hypergeometric DiffEq. For interesting
cases, I found the monodromy representation at singular points, and
generated plots. I presented my method, its history, and an application
to fluid flow at The College of Idaho’s 2016 student research
conference. At the same time, I studied point-set topology under
Dr. Dave Rosoff. He led seminar in a modified Moore method. I reasoned
from topological counter examples, finding errata in our notes by
discovering non-intuitive spaces, e.g., the space whose open sets are
those sets with countable complements. Further, we drew out analogies
from topology to introduce category theory. I am enthusiastic to build
from this ground to higher results, one of which I reached in my senior
study, another of which Nikki Sanderson demonstrated ahead of me.

I gained insight to the necessity of *applications* (especially with
positive societal impact) by completing two years of service work. In
Houston, under Shaoli Bhadra, I developed scalable
[resources](https://github.com/coltongrainger/ymca-resources) for
refugee case management. I crowd-sourced a [map of clinics and languages
spoken](https://drive.google.com/open?id=1kk9yn6-4nifHLIf2tGYbW_7PiYo&usp=sharing)
with the Google Maps API. I wrote bug reports for the implementation of
a SQL case-notes database, and, when Texas cut funding for Refugee
Medical Assistance, I contributed to a data management plan for the
small refugee population transitioning from state to federal medical
care. In Olympia, I am coordinating the volunteer program for a 24/7
homeless shelter. I rely on a distributed workflow—with `git` for
version control and pandoc markdown for administrivia. I built
[volunteer.fscss.org](http://volunteer.fscss.org) to maintain a schedule
of events and to “reply all” to volunteers. As we rely on interns and
work-studies, I am also collaborating with the Evergreen State College
to write service-learning syllabi.

I am serious, however, to pursue math as my vocation. To prepare for
graduate study, I have enrolled in correspondence courses at the
University of Idaho. By May 2018, I will have reviewed Differential
Equations, Probability and Numerical Analysis. I am also reading from
Hatcher’s *Algebraic Topology*, surveying topics in Gower’s *Companion
to Mathematics*, and building a base of computing skills in the UNIX
philosophy.

While I am open to a breadth of mathematical inquiry at CU Boulder, I am
most motivated to develop a rigorous foundation in algebraic
topology. My career aspiration is to become an applied mathematician, working
in machine learning or environmental preservation. I would be glad to
collaborate with Profs Beaudry, Farsi, or Pflaum, potentially also with
Profs Meiss and Bradley across departments. Having surveyed their recent
publications and seminar webpages, I believe the doctoral program in
mathematics at CU Boulder would be a great fit for my interests.

Thank you for your consideration.

[^1]: C. Grainger, [Applications of Galois Theory: Monodromy Groups and Fuchsian DiffEqs](http://coltongrainger.com/documents/cgrainger_coursework_galois_poster.pdf), College of Idaho SRC, 2016.

## meta 

- computationally intensive
	- TeX, Markdown, MathJax, Mathbook
	- programming, algorithm design
	- Sage, SciPy, plotting
	- examples first!
- emphasis on literacy
	- G. Polya
	- R. L. Moore
	- exposition as a social activity
		- writing for an audience
		- presentations as karaoke
- learning math at scale
	- nbgrader
	- WebWork
	- to publish small deck of Calculus review anki card

What's my meta-understanding of math? It's a journey through an unfamilar domain. From [Eliezer Yudkowsky](http://lesswrong.com/lw/31/what_do_we_mean_by_rationality/)
> believing, and updating on evidence, so as to systematically improve the correspondence between your map and the territory

As an occasional rock climber, I really enjoy the play between "math improves one's map of territory" and "programming is climbing a mountain". Rosoff once commented that a meta-theorem of math was to prove useful theorems alone, and once for all, so that higher level math can be done. Which amounts to having explored (either in detail or with breadth) common features and routes in the foundational territory of mathematical knowledge. I think of theorems and installations, then, as signposts in a domain. When performing mathematical research, or a long computation, theorems are like carabiners.

From [Philip Guo](https://www.oreilly.com/ideas/code-carabiners-essential-protection-tools-for-safe-programming)
> Somewhere around a few hundred lines of code, your code base becomes too large to fit inside your head; you start to forget why you wrote certain code in a quirky way; and you don’t quite remember what you were trying to do last week, or what assumptions about your internal data structures still hold true. Is that snippet of documentation from last month still valid? What about this TODO note? And how come this function used to work so well but doesn’t anymore? What made it suddenly break? Wait, how did this other module ever work? ARGH!!!

From [How People Learn](https://www.colorado.edu/MCDB/LearningBiology/readings/How-people-learn.pdf) 
> The new science of learning does not deny that facts are important for thinking and problem solving. Research on expertise in areas such as chess, history, science, and mathematics demonstrate that experts’ abilities to think and solve problems depend strongly on a *rich body of knowledge about subject matter* (e.g., Chase and Simon, 1973; Chi et al., 1981; deGroot, 1965).  However, the research also shows clearly that “usable knowledge” is not the same as a mere list of disconnected facts. Experts’ knowledge is connected and organized around important concepts (e.g., Newton’s second law of motion); it is “conditionalized” to specify the contexts in which it is applicable; it supports understanding and transfer (to other contexts) rather than only the ability to remember.

