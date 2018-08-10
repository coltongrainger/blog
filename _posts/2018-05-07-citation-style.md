---
title: Citation Style
author: Colton Grainger
date: 2018-05-07
status: notes
mathjax: true
---

To collect my thoughts on citation styles in different contexts. I'll list the places where I want to cite effectively (and quickly dagnabit!).

- pandoc markdown
  - notes
  - blog posts
  - informal letters
  - problem sets
- mediawiki
  - articles
- jupyter notebooks
  - data wrangling!
  - collaborative computation
- twitter
  - *[guck mal!](https://german.stackexchange.com/questions/36810/sieh-mal-vs-guck-mal)* moments
  - social bookmarks (this site supplants the need to post technical bookmarks on twitter)
- $\mathrm{\LaTeX}$
  - curriculum vitae
  - letters
  - syllabi

## makefile strategy 

If I'm citing the same source (e.g. Simon Jones) repeatedly, I'd like just to `[@sjones]`, in the [pandoc-citeproc](https://github.com/jgm/pandoc-citeproc) style. I'll need a `.bib` bibliography included and also a thorough understanding of the compilation process from whatever plain text source to the desired `.pdf` or `.html`. I suspect `pandoc-citeproc` and [CSL citation styles](https://citationstyles.org/)  will become my tools of choice.[^complex]

[^complex]: I imagine I'm going to run into trouble implementing these in gitit.

Kieran Healy models one workflow [here](https://kieranhealy.org/resources/). And I've taken the [Makefile](https://raw.githubusercontent.com/kjhealy/pandoc-templates/master/makefile/Makefile) (see also [discussion here](http://plain-text.co/pull-it-together.html)) from his [pandoc-templates repo](https://github.com/kjhealy/pandoc-templates).

Joseph Reagle gives a stellar example for marking up a curriculum vitae ([markdown](http://reagle.org/joseph/2003/cv/cv.md) and corresponding [html](http://reagle.org/joseph/2003/cv/cv.html)). Reagle opened two relevant issues (which are interesting forums to read for anyone trying to incorporate `.csl` files with a `pandoc-citeproc` workflow):

1. [Including styles with inline-references (instead of bibliography) for publication lists](https://github.com/citation-style-language/styles/issues/1619)
1. [apa-cv.csl not working with pandoc-citeproc](https://github.com/citation-style-language/styles/issues/1619)

## citation style languages

In undergrad, I was comfortable using [Biber](https://en.wikipedia.org/wiki/Biber_(LaTeX)) and $\rm\LaTeX$ for papers in the [Chicago footnote style](https://tex.stackexchange.com/questions/30287/get-biblatex-chicago-working) and in the [elsarticle.cls](https://tex.stackexchange.com/questions/110515/elsarticle-cls-and-biblatex-incompatibility) document class. I never really moved beyond `\footnote{https://math.dartmouth.edu}` for references in my mathematics problem sets. 

And yes, it seems Chicago (as footnotes or inline author-date) for informal writing and "numeric (or mnemonic), with titles, sorted alphabetically"  for mathematical writing remain the best choices for my intended audience.

There're also the [IEEE](https://github.com/citation-style-language/styles/blob/master/ieee.csl) and ACM proceedings styles, but these are further out of my scope. (Although I
see the advantage to IEEE in handling mixed media and link rot.)

Now to give examples of different `.csl` styles in (approximate) use.

### computer science

[acm-sig-proceedings.csl](https://github.com/citation-style-language/styles/blob/master/acm-sig-proceedings.csl)
: N. Polikarpova and J Yang et al., [Enforcing Information Flow Policies with Type-Targeted Program Synthesis](https://arxiv.org/pdf/1607.03445.pdf) (2018).

Note that Polikarpova expanded the reference keys to be more legible, which I like quite a bit.

[acm-sigchi-proceedings.csl](https://github.com/citation-style-language/styles/blob/master/acm-sigchi-proceedings.csl)
: P. J. Guo, [Non-Native English Speakers Learning Computer Programming: Barriers, Desires, and Design Opportunities](http://pgbovine.net/publications/non-native-english-speakers-learning-programming_CHI-2018.pdf) (2018).

### mathematics

[elsevier-with-tiles-alphabetical.csl](https://github.com/citation-style-language/styles/blob/master/elsevier-with-titles-alphabetical.csl) (i.e., numeric)
: T. Tao, [What is good mathematics?](https://arxiv.org/pdf/math/0702396.pdf) (2007).

Mnemonic
: M. Mirzakhani and A. Wright, [Full Rank Affine Invariant Submanifolds](https://web.stanford.edu/~amwright/FullRank.pdf) (2018).

I fear, in general, mnemonic bibliographies are formatted by hand. For example,
from the front matter of [“[1801.07530] A Guide for Computing Stable Homotopy Groups”](https://arxiv.org/abs/1801.07530), we find

```
% \MRhref is called by the amsart/book/proc definition of \MR.
\begin{thebibliography}{EKMM97}

\bibitem[Ada58]{adams_cohomology}
J.~F. Adams, \emph{On the structure and applications of the {S}teenrod
  algebra}, Comment. Math. Helv. \textbf{32} (1958), 180--214. \MR{0096219}

\bibitem[Ada60]{adams_hopf_inv_one}
\bysame, \emph{On the non-existence of elements of {H}opf invariant one}, Ann.
  of Math. (2) \textbf{72} (1960), 20--104. \MR{0141119}

% and so on
```

which, unfortunately, matches the colloquial instructions given in math departments and recapitulated here:

- [LaTeX Tips: Bibliographies](https://faculty.math.illinois.edu/~hildebr/tex/bibliographies.html). Retrieved May 8, 2018.

Some Definitive Style Guides

- [AMS Style Guide](https://www.ams.org/publications/authors/AMS-StyleGuide-print.pdf). Retrieved May 7, 2018.
- [MAA Reference Guide](https://www.maa.org/sites/default/files/pdf/pubs/Ref_Guide.pdf). Retrieved May 7, 2018.
- [SIAM Style Manual: For Journals and Books](https://www.siam.org/journals/pdf/stylemanual.pdf). Retrieved May 8, 2018.

## trivia

*But how do I manage my citation collection?* [CiteULike](http://www.citeulike.org/) subsumes MathSciNet for bibtex records, which is helpful for citing papers across traditional discipline boundaries. (See also [“What are good sites to find citations in BibTex format?”](https://tex.stackexchange.com/questions/143/what-are-good-sites-to-find-citations-in-bibtex-format/153). TeX - LaTeX Stack Exchange. Retrieved May 9, 2018.)

*Don't confound file extensions!*

- `.cls` for [LaTeX document class](https://tex.stackexchange.com/questions/7770/file-extensions-related-to-latex-etc)
  - [elsarticle.cls](https://www.elsevier.com/__data/assets/pdf_file/0008/56843/elsdoc-1.pdf)
- `.csl` for [citation style language](https://github.com/citation-style-language/styles) 
  - [chicago-note-bibliography.csl](https://github.com/jgm/pandoc-citeproc/blob/master/tests/chicago-note-bibliography.csl)

## meta

Isn't the goal to have internalized key references such that I can just prattle off at the appropriate times? 

Not necessarily to have memorized a series of author-dates but rather to *be familiar* with "the field" or "the canon" such that citations are more akin to introductions? And as with introductions to be mindful of who is getting to know who and the relationship that's therein forged?

(And also, isn't it curious that mathematicians are using `\bibitem` as opposed to curating a bibliography database? Maybe it's just one of those inherited quirks, but it also evinces that the mathematical canon, for many professionals, develops much slower than the spit-fire developments in, say, programming language research. I suspect, also, to lower the signal to noise ratio, professional mathematicians might regard parts of the canon as immutable.)

(Aside: Rosoff pointed me to Spivak's *Differential Geometry* at a point in my life where the text didn't make much sense. Still doesn't, but I now get the reference.)

![spivak-parade](https://images-na.ssl-images-amazon.com/images/I/91L0KVJjGlL.jpg){:width="100%"}
