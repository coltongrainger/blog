---
title: Personal Statement
author: Colton Grainger
date: 2017-11-23
status: draft
mathjax: true
---

The robustness of a mathematical method determines its utility. Just imagine designing a communication network that fails to account for dynamical perturbations, or modeling an epidemic with strictly deterministic differential equations. My goal, then, is to research robust topological methods for data analysis and physical applied mathematics. My interests, from abstract to concrete, include algebraic topology, dynamical systems, and scientific computation.

Consider training an AI to distinguish the tone signature of different musical instruments. Applying persistent homology, we associate holes in an audio recording's time-delay phase-space with a sample statistic: the persistent rank function. Corresponding with Nikki Sanderson, I learned a computer trained on such PRFs will more accurately classify tone signatures than one trained on FFTs. Here, a topological invariant answers "which instrument?" with higher fidelity than frequency analysis, demonstrating topology's robustness in application.

My research interest stems from (i) my exposure to topology and its applications as a college senior, and (ii) insight from two years of service work since graduating.

Advised by Dr. Jonny Comes, my senior independent study[^study] examined how Galois theory constrains the solution space $V$ of Fuchsian-type DiffEqs. Following Michio Kuga, I developed a correspondence between the fundamental group on $D = \mathbf{C}\setminus\\{x_1,\ldots,x_n\\}$ and this region's universal covering space $\tilde{D}$. Exploiting the representation of the group of covering transformations $\Gamma(\tilde{D} \to \tilde{D})$ as a group of linear automorphisms of $V$, I parameterized solutions to the hypergeometric DiffEq. For interesting cases, I found the monodromy representation at singular points, and generated plots. I presented my method, its history, and an application to fluid flow at The College of Idaho's 2016 student research conference.

[^study]: C. Grainger, [Applications of Galois Theory: Monodromy Groups and Fuchsian Differential Equation](http://coltongrainger.com/documents/cgrainger_coursework_galois_poster.pdf), The College of Idaho Student Research Conference, 2016.

At the same time, I studied point-set topology under Dr. Dave Rosoff. He led a small class in a modified Moore method: no lecture, only assigned theorems and student presentations. I built foundations from counter examples, often finding erratum in our notes by discovering non-intuitive spaces, e.g., consider a space $X$ whose open sets are exactly those sets with countable complements. Let $A \subset X$. For a every topological space, it is known "if $x_i \in A$ for each $i \in \mathrm{N}$ and $x_i \to x$, then $x$ is in the closure of $A$", but in our case, the converse fails to hold, as $X$ is not a second countable topology. We sampled category theory and progressed upto connectivity and compactness. I am enthusiastic to build from these *Grundlagen* upto higher applications, one of which I reached in my senior study, another of which Nikki Sanderson demonstrated ahead of me.

I have gained insight on the necessity of *applications* (esp. ones with positive societal impact) by completing two years of voluntary service: in Houston, TX at a refugee resettlement agency and in Olympia, WA at a homeless shelter for families.
 
In Houston, under Shaoli Bhadra, I developed novel, scalable [resources](https://github.com/coltongrainger/ymca-resources) for refugee case management. I learned to query Google Maps API and created a [map of clinics and languages spoken](https://drive.google.com/open?id=1kk9yn6-4nifHLIf2tGYbW_7PiYo&usp=sharing). I wrote bug reports for the implementation of a SQL case-notes database, and, when Texas cut funding for Refugee Medical Assistance, I contributed to a data management plan for the transition from state to federal indigent medical care.

In Olympia I am coordinating a volunteer program for a 24-hour homeless shelter. I cleave to a distributed workflow. I built [volunteer.fscss.org](https://volunteer.fscss.org) to manage a schedule of community events and to "reply all" to FAQs. As we rely on academic internships and work-studies, I am also collaborating with Dr. Catalino Ocampo at the Evergreen State College to write service-learning syllabi. In the coming year, I intend to apply for \\$90,000 in grant funding for shelter operation.

I am serious, however, to continue my studies in pursuit of my vocation. While I am grateful for learning to manage multiple projects and work with collaborators, I find myself constrained in social service agencies as an end-user of inefficient systems, and bound to idiosyncratic best practices. To sharpen the saw, I have enrolled part-time in continuing education through the University of Idaho's Engineering Outreach program. I will complete courses in Probabilty, Differential Equations, and Numerical Methods by May 2018. Independently, I am learning to chew on data with UNIX tools and to write interactive expositions with Juptyer notebooks.

Though I am open to a wide variety of research in applied mathematics, my experience with messy data sets and my appetite for topology leads naturally into topological data analysis. I would be enthusiastic to work with Professors Meiss (APPM), Bradley (CS) and  Agnes (MTH). From reading papers and surveying project websites, I see fruitful application of TDA in signal processing and network analysis, but I believe TDA could weigh in optimization problems material science and studies of contaminant dispersion. Upon obtaining a PhD, I imagine myself working in a research laboratory in the Western US.

Thank you for your consideration.

## Pedagogy

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

Meta-understanding of maths. Metaphorically a journey through an unfamilar domain. From [Eliezer Yudkowsky](http://lesswrong.com/lw/31/what_do_we_mean_by_rationality/)
> believing, and updating on evidence, so as to systematically improve the correspondence between your map and the territory
As an occasional rock climber, I really enjoy the play between "math improves one's map of territory" and "programming is climbing a mountain". Rosoff once commented that a meta-theorem of math was to prove useful theorems alone, and once for all, so that higher level math can be done. Which amounts to having explored (either in detail or with breadth) common features and routes in the foundational territory of mathematical knowledge. I think of theorems and installations, then, as signposts in a domain. When performing mathematical research, or a long computation, theorems are like carabiners.

From [Philip Guo](https://www.oreilly.com/ideas/code-carabiners-essential-protection-tools-for-safe-programming)
> Somewhere around a few hundred lines of code, your code base becomes too large to fit inside your head; you start to forget why you wrote certain code in a quirky way; and you don’t quite remember what you were trying to do last week, or what assumptions about your internal data structures still hold true. Is that snippet of documentation from last month still valid? What about this TODO note? And how come this function used to work so well but doesn’t anymore? What made it suddenly break? Wait, how did this other module ever work? ARGH!!!

From [How People Learn](https://www.colorado.edu/MCDB/LearningBiology/readings/How-people-learn.pdf) 
> The new science of learning does not deny that facts are important for thinking and problem solving. Research on expertise in areas such as chess, history, science, and mathematics demonstrate that experts’ abilities to think and solve problems depend strongly on a *rich body of knowledge about subject matter* (e.g., Chase and Simon, 1973; Chi et al., 1981; deGroot, 1965).  However, the research also shows clearly that “usable knowledge” is not the same as a mere list of disconnected facts. Experts’ knowledge is connected and organized around important concepts (e.g., Newton’s second law of motion); it is “conditionalized” to specify the contexts in which it is applicable; it supports understanding and transfer (to other contexts) rather than only the ability to remember.

