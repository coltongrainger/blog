---
title: Jupyter Notebook Configuration
author: Colton Grainger
date: 2018-03-04
---

I treat Jupyter notebooks as if they were [journal entries](journal-keeping), and therefore have adopted a configuration with multiple kernels and jq-filters for version control.

## Sage Kernel Installation

In 2016, I compiled Sage from binary. I generally opened the Jupyter notebook interface with `sage -n jupyter`.

By 2018, I realized I wanted `nbextensions` (namely, the
[jupyter-vim-binding](https://github.com/lambdalisue/jupyter-vim-binding)) for
all my Jupyter notebooks. (See [“Unofficial Jupyter Notebook Extensions — jupyter_contrib_nbextensions 0.4.0 documentation”](http://jupyter-contrib-nbextensions.readthedocs.io/en/latest/).)

I discovered that Sage uses its own version of the Jupyter notebook, whence I
needed to [install sagemath as a kernel in Jupyter](https://stackoverflow.com/questions/39296020/how-to-install-sagemath-kernel-in-jupyter). I followed [Samuel Lelièvre](https://stackoverflow.com/users/3827575/samuel-leli%c3%a8vre)'s advice
```shell
sudo jupyter kernelspec install ./SageMath/local/share/jupyter/kernels/sagemath
```
> Where SageMath is your root sagemath directory.

In my case `/Applications/SageMath/`. Further, they advised

> ...edit the `kernel.json` file to make the SageMath Jupyter kernel aware of SageMath's location, by adding `"env":{"SAGE_ROOT":"/path/to/sage"}` at the end of the dictionary in `kernel.json`. 
>
> You will find the location of `kernel.json` by executing `jupyter kernelspec list`.

My `kernel.json` now reads

```json
{
 "display_name": "SageMath 8.0", 
 "argv": [
  "/Applications/SageMath/local/bin/sage", 
  "--python", 
  "-m", 
  "sage.repl.ipython_kernel", 
  "-f", 
  "{connection_file}"], 
 "env":{"SAGE_ROOT":"/Applications/SageMath/"}
}
```

whence SageMath is loaded as a kernel in the (standard) Jupyter Notebook.

## Version Control paradigm

How should I curate individual notebooks? By subject? By date? By most
recently updated?

On one hand, I could follow [Jonathan
Whitmore](https://svds.com/jupyter-notebook-best-practices-for-data-science/)'s
suggestion - be verbose!

> Let a traditional paper lab notebook be your guide here:
> 
> - Each notebook keeps a historical (and dated) record of the analysis as it’s being explored.
> - The notebook is not meant to be anything other than a place for experimentation and development.
> - Each notebook is controlled by a single author: a data scientist on the team (marked with initials).
> - Notebooks can be split when they get too long.
> - Notebooks can be split by topic, if it makes sense.

Yet, I have no one in mind as an imagined reader. I might as well get notebooks configured in a way that would be useful for a data-analytic "reading". As in, which did I return to edit most frequently? which were referenced for code most often? least often?

Thinking about [“Philip Guo - PG Podcast - Episode 35 - Audrey Boguchwal + Nadia Eghbal on sustainable online communities”](http://pgbovine.net/PG-Podcast-35-Audrey-Boguchwal-and-Nadia-Eghbal.htm), right now, I want neither to add noise to an online community nor hear it. It seems more beneficial to use notebooks to (i) build rote mechanical skill, and (ii) develop intuition, than to write for an audience.

Consequently, I'm following [Tim Saley](http://timstaley.co.uk/posts/making-git-and-jupyter-notebooks-play-nice/)'s advice: strip notebooks of outputs and metadata for version control.

Because I occasionally run `sagemath` and `mit-scheme` as kernels for REPL style computations, I'll only remove metadata from the individual cells.

I've set a [filter](https://git-scm.com/docs/gitattributes#__code_filter_code) to clean `*.ipynb` files in any of my git repos with [jq](https://stedolan.github.io/jq/).

In my `~/.gitconfig`

```shell
[core]
attributesfile = ~/.gitattributes_global

[filter "nbstrip_full"]
clean = "jq --indent 1 \
        '(.cells[] | select(has(\"outputs\")) | .outputs) = []  \
        | (.cells[] | select(has(\"execution_count\")) | .execution_count) = null  \
        | .cells[].metadata = {} \
        '"
smudge = cat
required = true
```

and then in my `~/.gitattributes_global`

```config
*.ipynb filter=nbstrip_full
```

## meta

Similar to my activities feeds, I've flattened the directory tree for notebooks. I have no doubt an organization beyond chronology will fall out.

In a sociological analog, from [Why Workers Can Suffer in Bossless Companies
Like GitHub](https://www.wired.com/2014/03/tyranny-flatness/), we have
> Critics say flat organizations can conceal power structures and shield
> individuals from accountability. This idea dates to the 1972 essay *[The
> Tyranny of Structurelessness](http://www.jofreeman.com/joreen/tyranny.htm)*
> by Jo Freeman, who describes her experiences in "leaderless" feminist
> organizations in the 1960s. "There is no such thing as a structureless
> group," Freeman wrote. "Any group of people of whatever nature that comes
> together for any length of time for any purpose will inevitably structure
> itself in some fashion."

## see also

- [file save hooks](http://jupyter-notebook.readthedocs.io/en/latest/extending/savehooks.html) to pretty print "deliverable" notebooks.
- [Installing the SageMath Jupyter Kernel and Extensions](http://doc.sagemath.org/html/en/reference/repl/sage/repl/ipython_kernel/install.html)
- [Making Kernels for
  Jupyter](http://jupyter-client.readthedocs.io/en/stable/kernels.html)
- Ch. 2, [“Sage Installation Guide - installation.pdf”](http://doc.sagemath.org/pdf/en/installation/installation.pdf)
