---
title: Personal Statement
author: Colton Grainger
date: 2017-11-23
status: draft
mathjax: true
---

I aim to pursue a PhD in mathematics, and my career aspiration is to become a quantitative scientist. 

The robustness of a mathematical discipline determines its utility. Just imagine designing a communication network that fails to account for dynamical perturbations, or modeling an epidemic with strictly deterministic differential equations. My goal, then, is to research robust topological methods for data analysis and physical applied mathematics. My interests, from abstract to concrete, include algebraic topology, dynamical systems, and scientific computation.

Consider training an AI to distinguish the tone signature of different musical instruments. Applying persistent homology, we associate holes in an audio recording's time-delay phase-space with a sample statistic: the persistent rank function. In correspondence with Nikki Sanderson, I learned a computer trained on such PRFs will more accurately classify tone signatures than one trained on FFTs. Here, a topological invariant answers "which instrument?" with higher fidelity than frequency analysis, demonstrating topology's robustness in application.

My research interest stems from (i) my exposure to topology and its applications as a college senior, and (ii) insight from two years of service work since graduating.

Advised by Dr. Jonny Comes, my senior independent study[^study] examined how Galois theory constrains the solution space $V$ of Fuchian-type DiffEq's. Following Michio Kuga, I developed a the correspondence between the fundamental group on $D = \mathbf{C}\setminus\\{x_1,\ldots,x_n\\}$ and this region's universal covering space $\tilde{D}$. Exploiting the monodromy representation of the group of covering transformations $\Gamma(\tilde{D} \to \tilde{D})$ as the group of linear automorphisms of $V$, I parameterized solutions to the hypergeometric DiffEq. For interesting cases, I found the monodromy representation at singular points, and generated plots. I presented my method, its history, and an application to fluid flow at The College of Idaho's 2016 student research conference.

[^study]: C. Grainger, [Applications of Galois Theory: Monodromy Groups and Fuchsian Differential Equation](http://coltongrainger.com/cgrainger_coursework_galois_poster.pdf), The College of Idaho SRC, 2016.

At the same time, I studied point-set topology under Dr. Dave Rosoff. He led a small, discussion-based class in a modified Moore method: no textbook, no lecture, only student presentations. Three classmates and I discovered there exists a topological space $X$, a set $A\subset X$, and an $X$-limit point $x \in A$ for which there is no sequence $x_i \in A$, $i \in \mathrm{N}$ such that $x_i \to x$. One such space is the space whose open sets are exactly those sets with countable complements. We had found a counter example to show the converse[^converse] of the following theorem is false: "Let $A \subseteq X$ be a subset of the topological space $X$. If $x_i \in A$ for each $i \in \mathrm{N}$ and $x_i \to x$, then $x$ is in the closure of $A$." 

By Fall 2018, I will have completed a two years of service: in Houston,TX at a refugee resettlement agency, and in Olympia, WA at a family homeless shelter. 
In Houston, I developed novel, scalable [resources](https://github.com/coltongrainger/ymca-resources) for persistent issues in refugee case management. I created and distributed a [map of clinics](https://drive.google.com/open?id=1kk9yn6-4nifHLIf2tGYbW_7PiYo&usp=sharing). I participated in a refugee health needs assessment with medical students at Baylor. I even was fortunate to be invited to contribute to the design of a data management plan for the next refugee social service database.
I began to build an [GitHub repository](https://github.com/coltongrainger/ymca-resources) of forms and instructions for low income healthcare applications and rental assistance. I established contact with and solicited feedback from staff in the Harris Health System, at the Islamic Society of Greater Houston, and at Gulf Coast Community Services Association. I incorporated my experience in direct service with the higher-level feedback from each organization. I found the best way for case managers to submit applications and detailed exactly what is expected of the client during the application process. Because our clients have limited English proficiency, I emphasized that case managers need to be aggressive and “get the job done” when faced with unnecessarily complicated release of information constraints. I also learned more about Shaoli’s Refugee Health Working Group. I created and distributed a [map of clinics](https://drive.google.com/open?id=1kk9yn6-4nifHLIf2tGYbW_7PiYo&usp=sharing). I participated in a refugee health needs assessment with medical students at Baylor. I even was fortunate to be invited to contribute to the design of a data management plan for the next refugee social service database. The above examples are united by a common thread: each represents a small contribution to a larger dialogue surrounding the resettlement of displaced persons.
	- 2017 
		- year of service in refugee case management
			- data management
			- vetted data during the implementation of 3 refugee databases
		- novel, scalable resources for social workers
			- case notes as narratives
			- google maps API
			- attemping to crowd source cultural knowledge
				- native language speakers
				- clinics 
				- bus routes
			- refugee health needs assessment with medical students at Baylor
		- git, web design
			- coordinating volunteer program for family homeless shelter
		- supplemental coursework
			- probability 
			- differential equations
			- numerical methods
		- personal transparency
		- coltongrainger.com
## Outline

- chronology
	- 2014
		- coupled oscillating pendula
		- putnam
	- 2015
		- Putnam
		- fourier series for heat equation
		- COMAP: SIRS model for Ebola in Africa
		- academic withdrawal (?)
	- 2016
		- rigourous coursework in Analysis and Topology
		- modelling HIV in Houston
		- logistic equation
		- tutoring and grading 
		- putnam
		- Galois Theory & Fuchsian Equations 
		- Igneous Dikes in Scotland
	- 2017 
		- year of service in refugee case management
			- data management
			- vetted data during the implementation of 3 refugee databases
		- novel, scalable resources for social workers
			- case notes as narratives
			- google maps API
			- attemping to crowd source cultural knowledge
				- native language speakers
				- clinics 
				- bus routes
			- refugee health needs assessment with medical students at Baylor
		- git, web design
			- coordinating volunteer program for family homeless shelter
		- supplemental coursework
			- probability 
			- differential equations
			- numerical methods
		- personal transparency
		- coltongrainger.com
- pedagogy
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

- U.S. Committee for Refugees and Immigrants to ensure that clients were effectively rolled out of the Texas Medicaid \& Healthcare Partnership database into the RMA portal

[^converse]: However, the converse holds if $X$ is a second countable topology.
