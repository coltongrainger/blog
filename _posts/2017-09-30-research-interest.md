---
title: Research Interest
author: Colton Grainger
date: 2017-09-30
modified: 2017-11-18
belief: likely 
status: draft 
---

I aim to study topological data analysis, which seeks to answer the question: *What is the shape of data?*


## Software
- JavaPlex
	- great tutorial, works with MatLab
- Persius 
	- acts as a package for Python to call?
	- [discrete morse theory](https://en.wikipedia.org/wiki/Discrete_Morse_theory)
	- simplifies complex while preserving homology (fast!)
- PHAT
	- works well with R?

## Reflections

### Vidit Nanda's [Introduction to Persius](https://www.youtube.com/watch?v=JqajfI4-WnM)

Nanda is "building filtered complexes around data points." Only imposes a nearest neighbor model on data points, which are vertices in Euclidean n-space. The filtered complexes provide computable topological invariants that "reveal underlying structure". Matrices record how boundaries in the graph are touched, from vertices to edges to triangles to tetrahedrons (etc). From these matrices (corresponding to different dimensions of the homology?) one may compute ranks, which are finite invariants. Nanda describes the process as a "very imperfect Fourier transform" (and emphasizes that it's not an invertible process). 

Nanda introduces Homology as that which "eats spaces and spits out sequences of vector spaces", where the dimension of the zeroth term is the number of connected components, of the first term is the number of independent closed loops, of the second term is the number of enclosed cavities (and so on).

Persistent homology refers to the persistence of a certain feature (say a cavity) through increasing radius for nearest neighbor pairings. 

Nanda cites applications including sensor network coverage, granular force chains, and protein compressibility.

### Nicole Sanderson's [Time Series in Dynamical Systems](https://arxiv.org/abs/1708.09359)

What's the goal? We need to perform persistent homology. We have a data set to represent as a simplicial complex. How to build? What're the parameters? What's the good radius? As we vary the radius (and some other parameters) how does the homology change?

