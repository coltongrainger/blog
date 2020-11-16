---
title: Jupyter Notebook Configuration
author: Colton Grainger
revised: 2018-07-16
---

*Update: while notebooks usefully package code, kernel, and exposition, putting content into the `ipynb` qua `json` format is (or should be) the last step in my workflow.*

Why? Rather than tooling around in a browser, I prefer to open a Jupyter Qt-console^[Always a nightmare to setup. Presently, I have qtconsole installed at `$HOME/.local/lib/python3.7/site-packages/qtconsole`. For whatever reason, I usually forget this, then install qtconsole for python 2.7 or python 3.6, then get stuck with cryptic error messages.], load a data set (which, thanks to the IPython kernel, will stay "hot in RAM"[^hot]), draft functions in vim, then `%run -i` to bring the defined functions into the kernel. I only create a `*ipynb` file (i) when I am certain I can generalize my sequence of transformations of the data, and (ii) when I am satisfied that the data set is exemplar to lead into exposition. Finally, thanks to [ipynb_notedown](https://github.com/goerz/ipynb_notedown.vim), I can polish my argument in markdown.

[^hot]: [“Philip Guo - PG Vlog #145 - Python + R Data Analysis Setup”](http://pgbovine.net/PG-Vlog-145-python-r-data-analysis-setup.htm). Retrieved July 16, 2018.

Old: I treat Jupyter notebooks as [journal entries](journal-keeping). This post outlines my exposure and initial workflow in the IPython kernel as a user of [SageMath](https://en.wikipedia.org/wiki/SageMath).

## Sage Kernel

In 2016, I compiled Sage from binary. I generally opened the Jupyter notebook interface with `sage -n jupyter`.

By 2018, I realized I wanted `nbextensions` (namely, the [jupyter-vim-binding](https://github.com/lambdalisue/jupyter-vim-binding)) for all my Jupyter notebooks. (See [“Unofficial Jupyter Notebook Extensions — jupyter_contrib_nbextensions 0.4.0 documentation”](http://jupyter-contrib-nbextensions.readthedocs.io/en/latest/).)

I discovered that Sage uses its own version of the Jupyter notebook, whence I needed to [install sagemath as a kernel in Jupyter](https://stackoverflow.com/questions/39296020/how-to-install-sagemath-kernel-in-jupyter). I followed [Samuel Lelièvre](https://stackoverflow.com/users/3827575/samuel-leli%c3%a8vre)'s advice 

```shell
sudo jupyter kernelspec install ./SageMath/local/share/jupyter/kernels/sagemath
```

> Where SageMath is your root sagemath directory.

On MacOS `/Applications/SageMath/`. Further, they advised

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

## Version Control

How should I curate individual notebooks? By subject? By date? By most recently updated?

On one hand, I could follow [Jonathan Whitmore](https://svds.com/jupyter-notebook-best-practices-for-data-science/)'s suggestion - be verbose!

> Let a traditional paper lab notebook be your guide here:
> 
> - Each notebook keeps a historical (and dated) record of the analysis as it’s being explored.
> - The notebook is not meant to be anything other than a place for experimentation and development.
> - Each notebook is controlled by a single author: a data scientist on the team (marked with initials).
> - Notebooks can be split when they get too long.
> - Notebooks can be split by topic, if it makes sense.

Yet, I have no one in mind as an imagined reader. I might as well get notebooks
configured in a way that would be useful for a data-analytic "reading". As in,
which did I return to edit most frequently? which were referenced for code most
often? least often?

Thinking about [“Philip Guo - PG Podcast - Episode 35 - Audrey Boguchwal + Nadia Eghbal on sustainable online communities”](http://pgbovine.net/PG-Podcast-35-Audrey-Boguchwal-and-Nadia-Eghbal.htm), right now, I want neither to add noise to an online community nor hear it. It seems more beneficial to use notebooks to (i) build mechanical skill, and (ii) develop intuition, than to write for an audience.

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

In a sociological analog, from [Why Workers Can Suffer in Bossless Companies Like GitHub](https://www.wired.com/2014/03/tyranny-flatness/), we have

> Critics say flat organizations can conceal power structures and shield individuals from accountability. This idea dates to the 1972 essay *[The Tyranny of Structurelessness](http://www.jofreeman.com/joreen/tyranny.htm)* by Jo Freeman, who describes her experiences in "leaderless" feminist organizations in the 1960s. "There is no such thing as a structureless group," Freeman wrote. "Any group of people of whatever nature that comes together for any length of time for any purpose will inevitably structure itself in some fashion."

## see also

- [file save hooks](http://jupyter-notebook.readthedocs.io/en/latest/extending/savehooks.html) to pretty print "deliverable" notebooks.
- [Installing the SageMath Jupyter Kernel and Extensions](http://doc.sagemath.org/html/en/reference/repl/sage/repl/ipython_kernel/install.html)
- [Making Kernels for Jupyter](http://jupyter-client.readthedocs.io/en/stable/kernels.html)
- Ch. 2, [“Sage Installation Guide”](http://doc.sagemath.org/pdf/en/installation/installation.pdf)
