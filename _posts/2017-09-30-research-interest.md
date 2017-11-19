---
title: Research Interest
author: Colton Grainger
date: 2017-09-30
belief: likely 
status: notes
---

I aim to study under one of the following disciplines: 
- topological data analysis, which seeks to take advantage of persistent homology in a computational setting
- computational topology


What's the goal? We need to perform persistent homology. We have a data set to represent as a simplicial complex. How to build? What're the parameters? What's the good radius? As we vary the radius (and some other parameters) how does the homology change?

Software: 
- JavaPlex
	- great tutorial, works with MatLab
- Persius 
	- [Vidit Nanda's introduction](https://www.youtube.com/watch?v=JqajfI4-WnM)
	- acts as a package for Python to call?
	- [discrete morse theory](https://en.wikipedia.org/wiki/Discrete_Morse_theory)
	- simplifies complex while preserving homology (fast!)

Here's my reflection. Nanda is "building filtered complexes around data points." Only imposes a nearest neighbor model on data points, which are vertices in Euclidean n-space. The filtered complexes provide computable topological invariants that "reveal underlying structure". Matrices record how boundaries in the graph are touched, from vertices to edges to triangles to tetrahedrons (etc). From these matrices (corresponding to different dimensions of the homology?) one may compute ranks, which are finite invariants. Nanda describes the process as a "very imperfect Fourier transform" (and emphasizes that it's not an invertible process). 

Nanda introduces Homology as that which "eats spaces and spits out sequences of vector spaces", where the dimension of the zeroth term is the number of connected components, of the first term is the number of independent closed loops, of the second term is the number of enclosed cavities (and so on).

Persistent homology refers to the persistence of a certain feature (say a cavity) through increasing radius for nearest neighbor pairings. 

Nanda cites applications, including sensor network coverage, granular force chains, and protein compressibility.
- PHAT
	- works well with R?

Then some more resources:
- [Kathryn Hess Bellwald](https://hessbellwald-lab.epfl.ch/HessBellwald)
	- [publications](https://hessbellwald-lab.epfl.ch/publications)
	- some application to neuro-science, which loops around with potential treatments of MS
	- blue brain project

