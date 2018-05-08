---
title: Citation Styles
author: Colton Grainger
date: 2018-05-07
status: notes
mathjax: true
---

To collect my thoughts on citation styles in different contexts. I'll list the contexts where I want to cite effectively (and quickly dagnabit!).

- pandoc markdown
  - notes
  - blog posts
  - informal letters
  - problem sets
- mediawiki
  - articles
- jupyter notebooks
- twitter
  - *[guck mal!](https://german.stackexchange.com/questions/36810/sieh-mal-vs-guck-mal)* moments
  - timorous outbursts
  - bookmarks
  - link dumps
- $\LaTeX$
  - curriculum vitae
  - formal letters

## strategy

If I'm citing the same source (e.g. Simon Jones) repeatedly, I'd like just to
`@sjones`, in the [`pandoc-citeproc`](https://github.com/jgm/pandoc-citeproc)
style. I'll need a `.bib` bibliography included and also a thorough
understanding of the compilation process from whatever plain text source to the desired `.pdf` or `.html`. I suspect `pandoc-citeproc` and [CSL citation styles](https://citationstyles.org/)  will become my tools of choice.

Joseph Reagle gives a stellar example for marking up a curriculum vitae ([markdown](http://reagle.org/joseph/2003/cv/cv.md) and corresponding [html](http://reagle.org/joseph/2003/cv/cv.html)). Reagle opened two relevant issues (which I think are good starting points for anyone trying to incorporate `.csl` files with a `pandoc-citeproc` workflow):

1. [Including styles with inline-references (instead of bibliography) for
   publication lists](https://github.com/citation-style-language/styles/issues/1619)
1. [apa-cv.csl not working with pandoc-citeproc](https://github.com/citation-style-language/styles/issues/1619)

In undergrad, I was comfortable using
[Biber](https://en.wikipedia.org/wiki/Biber_(LaTeX)) and $\LaTeX$ for papers in the [Chicago footnote style](https://tex.stackexchange.com/questions/30287/get-biblatex-chicago-working) and in the [elsarticle.cls](https://tex.stackexchange.com/questions/110515/elsarticle-cls-and-biblatex-incompatibility) document class. I never really moved beyond `\footnote{https://math.dartmouth.edu}` for references in my mathematics problem sets.

Now, however, I'd like to know what's standard for mathematical writing.
Perhaps one of the following?

- [AMS Style Guide](https://www.ams.org/publications/authors/AMS-StyleGuide-print.pdf). Retrieved May 7, 2018.
- [MAA Reference Guide](https://www.maa.org/sites/default/files/pdf/pubs/Ref_Guide.pdf).
Retrieved May 7, 2018.

Or just to look at exemplar formatting: T. Tao, [What is good mathematics?](https://arxiv.org/pdf/math/0702396.pdf) (2007).

## other tips

- don't confound file extensions.
  - `.cls` for [LaTeX document class](https://tex.stackexchange.com/questions/7770/file-extensions-related-to-latex-etc)
    - [elsarticle.cls](https://www.elsevier.com/__data/assets/pdf_file/0008/56843/elsdoc-1.pdf)
  - `.csl` for [citation style language](https://github.com/citation-style-language/styles) 
    - [chicago-note-bibliography.csl](https://github.com/jgm/pandoc-citeproc/blob/master/tests/chicago-note-bibliography.csl)

## meta

Isn't the goal to have internalized key references such that I can just
prattle off at the appropriate times? 

Not necessarily to have memorized a series of author-dates but rather to *be
familiar* with "the field" or "the canon" such that citations are more akin to
introductions? And as with introductions to be mindful of who is getting to
know who and the relationship that's therein forged?

I think Rosoff exposed me to Spivak's *Differential Geometry* at a point in my
life where the text didn't make much sense. I'm grateful for the introduction,
however, in that I felt I was being pointed towards a parade going by, which
was compelling enough for me to take Vol. 1 to rehabilitation, set some
goals there, and build the sort of grit necessary to become a more rigorous
interlocutor.

![spivak-parade](https://images-na.ssl-images-amazon.com/images/I/91L0KVJjGlL.jpg){:width="100%"}
