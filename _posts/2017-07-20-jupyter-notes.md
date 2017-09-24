---
title: Jupyter notebook webinar
author: Colton Grainger
created: 2017-07-20
revised: 2017-09-23
belief: likely
status: notes
---

I recently participated in a webinar (July 2017) hosted by Science Gateways Community Institute (which exists to facilitate community sharing of experiences, technologies, and practices at little or no cost!) These are my notes and reactions.

# Background

Dave Rosoff introduced me to SageMathCloud in 2014 for solving systems of differential equations, which was my first exposure to IPython notebooks. As I didn't know TeX then, I struggled tremendously to format my output. I didn't pry deep into python's libraries; I mostly stayed in the sage docs. 

I was tasked to analyze resonance given different forcing functions for 2nd order linear DEs. At finish, I had a mish-mashed assemblage of sage commands and non-compiling markdown. I couldn't even plot a collection of functions without manually typing in new the parameters (as opposed to now, where I'd use plot a just plot a list of functions indexed by parameter values).

`plot([exp(-3*x)*(x^2 + C) for C in [-1..2]], (-0.5, 0.5))`

# Webinar Notes

Carol Willing presented a whirlwind tour of Jupyter's development out of IPython:
- For information about IPython prior to 2011, see [Perez's historical ruminations](http://blog.fperez.org/2012/01/ipython-notebook-historical.html)])
- In 2013, the IPython project started engaging users of [Music21](http://web.mit.edu/music21/doc/about/what.html) with interactive musicology notebooks. 
- In 2014, to break down barriers to entry, the IPython project rebranded itself as Project Jupyter (where IPython continued to provide the kernel), 
	- Andrea Zonca's [blog](zonca.github.io) was instrumental in promoting the project. (He continues to write about high performance computing and to offer Python tips.) 
- In 2016, the original author of IPython, Fernando Perez, and contributor to the notebook interface, Brian Granger, won substantial funding for [development](http://vcresearch.berkeley.edu/news/project-jupyter-gets-6m-expand-collaborative-data-science-software): "to serve users and foster collaboration". 
	- Perez cites Richard Hamming's 1962 observation that "the purpose of computing is insight, not numbers" as historic impetus for IPython notebook and motivation for the current form of the Jupyter notebook ([video](https://youtu.be/4pnj-eNEaqk)).

Following, Carol mentioned that Project Jupyter is determined to reach wider audience (not just mathematicians and computer scientics). This bears similarity to SageMathCloud's [rebranding](https://cocalc.com/). To increase cross-disciplinary collaboration, Carol emphasized the notebook interface's strengths in *data exploration, visualization, and analysis*. 

# What's new with Jupyter?

- One could look at [trending notebooks](github.com/trending/juptyer-notebook)
- [Binder](https://beta.mybinder.org/) 
	- to build github repos into live notebooks with the python kernel
	- won't work for notebooks running on a sagemath kernel
- [JupyterHub](https://jupyterhub.readthedocs.io/en/latest/)
	- info sharing, passing off notebooks, browser based
	- also implemented [here](https://github.com/harvard/cloudJHub) on Amazon Cloud for teaching
	- to get started [Zero to JupyterHub](http://zero-to-jupyterhub.readthedocs.io/en/latest/)
- [Jupyter Lab](https://github.com/jupyterlab/jupyterlab)
- diffing and merging Jupyter notebooks with [nbdime](https://github.com/jupyter/nbdime)
- assigning and grading notebooks with [nbgrader](https://github.com/jupyter/nbgrader)
- Demba Ba's [Labs in the Wild](https://www.youtube.com/watch?v=h7WThtzuq_8) 
	- He's taught a few vertically integrated signal processing courses with wearable (physiological monitors)(https://www.empatica.com/e4-wristband)) and Jupyter notebooks.
	- Example project: using wrist accelerator to predict the success of a freethrow? Can we set up an algorithm to provide feedback during the freethrow? Assigning a signature to a basket
 	- Demba emphasizes that *data manipulation is part of literacy.*
> [In a notebook] we expect to see data collection, experiemental protocol, analysis, use of sophisiticated algorithms, etc.


