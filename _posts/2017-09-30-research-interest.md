---
title: Research Interest
author: Colton Grainger
date: 2017-09-30
modified: 2017-11-18
belief: likely 
status: draft 
---

I aim to study topological data analysis, which seeks to answer the question: *What is the shape of data?* 

Historically, I have been motivated to understand particle flows in dynamical systems, given their utility for modeling contaminant dispersion. However, I feel any policy recommendations to come from research in contaminant dispersion amounts to suggesting techniques for smearing some neutralizing agent through the contaminanted region. From a high level, it's tempting, but perhaps distracting, to devote too much mental effort towards cleaning up messes. On the other hand, neutralizing a contaminant by cleverly exploiting bending-and-folding seems praiseworthy.

In 2016, as I applied to MS programs, I wrote
> I would design and implement numerical methods to model ground water and aquifers.

I had also boiled down cute scenerios for the fulfillment of this promise, for example, regarding sediment transport
> In Idaho's Treasure Valley, farmers use a network of reservoirs and canals to suspend and divert the Boise river. To understand how this irrigation regime sweeps up and transports material, I would model water's energy in flood irrigated fields. Constrained by agricultural machinery and topography, I would search for furrow patterns that minimize water's turbidity. As a related project, I would consider canal geometries that interrupt high-velocity flows.

A few months after declaring my intent to implement numerical methods, a former mentor mentioned he was concerned I "had quashed my own desires and interests out of a feeling of duty or a need to make more palpable, measurable contributions to society in general", so I will necessarily proceed cautiously as I express interest in applied topics. Maybe a study of contaminant diffusion is rooted too much in *application* and *analysis* (the middle sections of [Bloom's taxonomy](https://upload.wikimedia.org/wikipedia/commons/2/24/Blooms_rose.svg)) rather than *synthesis* and *evaluation*, which I relish as areas to suggest new approaches, then embark again into experimentation.

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

### Roseanna Neupauer's [Chaotic Advection and Reaction](http://onlinelibrary.wiley.com/doi/10.1002/2013WR014057/full)

- Studies how Engineered Injection and Extraction (EIE) methods can deform treatment solution emplaced in a contaminated aquifer. 
- Numerical simulation implemented with [MODPATH](https://pubs.usgs.gov/of/1994/0464/report.pdf) (a particle tracking post-processing package for MODFLOW, The U.S. Geological Survey finite-difference ground-water flow model). 

Seems like some of the software that would be necessary to fulfill a promise I made in 2016 (in terms of modeling contaminants).
> With the Army's decision not to grant an easement for the Dakota Access Pipeline (DAPL), I have a redoubled interest in contaminant dispersion. If I were contributing to an environmental impact statement for DAPL, I would (i) consider geomorphic stresses on the pipeline and (ii) model hydrocarbon dispersion through sand, shale or clay at points of stress. 

Neupauer's analysis extends beyond modeling, however, and focuses on the interface between the treatment solution and the contaminant. 
> In heterogeneous aquifers, the heterogeneity causes local variations in the plume movement that result in deviations from radial flow.... For the heterogeneous aquifers, the interface is more irregular than the interface for the homogeneous aquifer. The deviation from the smooth three-branched shape increases as the variance of the random field increases and as the correlation length decrease.

To gauge an aquifier's heterogeneity, one could bury some diodes to characterize homogeneous filaments (strands of sand, shale, or clay) then map the filaments as data for the numerical simulation. But burying the diodes seems tedious, right, if we're utlimately concerned with the probability that contaminant/treatment *does not* reach a source of drinking water? I'm not confident that sampling impedance across a handful of points would suffice to explicitly model the aquifier's heterogeneous composition. So relying on some sort of stochasitic analysis in the first place, then minimizing probability of extracting solution seems to be computationally parsimonious. 

Neupauer states:
>  A full optimization of the EIE sequence would be necessary to balance the trade-offs between reducing the probability of extracting treatment solution and maximizing the amount of degradation.
