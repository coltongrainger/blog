---
title: Computer Science Transitional Syllabus
author: Colton Grainger
date: 2020-07-14
revised: 2020-09-17
math: true
---

This is my adaptation of John Regehr's "wish-list for self-study" (<https://blog.regehr.org/archives/1578>) to help me pivot into software engineering. I've marked with TODO those tools that I'm not yet comfortable using professionally. The goal is to flesh out my knowledge during COVID-19 and for the next few years.

> In the software engineering course I’m teaching this spring, I often find myself saying things like “you need to know a scripting language” or “everyone should be able to run a code coverage tool.” Finally, the other day, a student stopped me and asked for the whole list. In other words, what — in my opinion — is the collection of tools that someone graduating with a CS degree should know how to use. Of course I couldn’t answer this on the spot but I’ve been thinking about it since then. The basic idea is that for most any common situation, you should have a decent tool at hand and be able to start solving problems with it without too much fumbling around. (John Regehr, 2018)


## The Basic Toolbox

### a version control system

"a Github-centric workflow including pull requests, remotes, merge conflicts, etc."

- git 
    - <https://gitolite.com/gcs.html>
- GitHub 
    - <https://docs.github.com>

### a text editor

"a solid default choice that does a good job with most editing tasks[; it] should highlight and indent any common programming language, integrate with a spellchecker, easily load gigantic files, have nice regex-based search and replace, etc."

- vim 
    - <http://vimcasts.org>
- vim plugins
    - <https://github.com/junegunn/vim-plug>
    - <http://vimcasts.org/categories/plugins>

### a shell language

"for scripting a smallish number of commands, doing a bit of error checking, and perhaps looping or interacting with the user slightly"

- bash 
    - <https://wiki.bash-hackers.org>
    - <https://www.seas.upenn.edu/~cis191>

- fish 
    - <https://jvns.ca/blog/2017/04/23/the-fish-shell-is-awesome/>

### a generic build system

- Make  (TODO)
    - <https://makefiletutorial.com>
    - <https://www.seas.upenn.edu/~cis191>

### a scripting language

"for low-grade automation, quick and dirty data analysis tasks, etc."

- Python3 (TODO: go deeper)
    - <https://cis192.github.io>

### a workhorse language

"for most tasks, [which] should have a huge collection of high-quality libraries, be pretty fast, run on all common platforms, etc.; know how to use its interactive debugger, static and dynamic bug-finding tools, a profiler, a code coverage tool, a package manager, and perhaps a random test-case generator."

- Java (TODO)
    - <https://introcs.cs.princeton.edu/java/home/>
- OCaml/Java (TODO)
    - <https://www.seas.upenn.edu/~cis120/>
- Scala (TODO)

### a pocket calculator

"go-to REPL for basic arithmetic and conversions between number representations, it should be near-instantaneous to get answers."

- again, Python3

### a data analysis language

- once more, Python3
    - <https://greenteapress.com/thinkstats2>
- pandas 
    - <https://github.com/guipsamora/pandas_exercises>
- numpy 
    - <https://scipy-lectures.org/intro/numpy/>
- SQLAlchemy

### a database

- MySQL
- AWS RDS (TODO)
    - <https://aws.amazon.com/rds/?nc2=h_ql_prod_db_rds>

### a graphing program

- numpy/pandas/matplotlib 
    - <https://scipy-lectures.org/intro/matplotlib>
    - <https://pandas.pydata.org/pandas-docs/stable/user_guide/visualization.html>
    - <https://jakevdp.github.io/PythonDataScienceHandbook>
- Graphviz (directed graphs)
    - <https://graphviz.readthedocs.io>
- $\LaTeX$'s TikZ, Xy-pic (commutative diagrams)
    - <http://presheaf.com>
    - <https://en.wikibooks.org/wiki/LaTeX/Xy-pic>

### a presentation tool

- Jupyter notebooks with RISE extension 
    - <https://rise.readthedocs.io>
- $\LaTeX\ $ beamer package
- Pandoc
    - <https://pandoc.org/demo/SLIDES>


## Secondary Tools

### a programmer's keyboard

```
not only our dream but also many thinkpad users' dream
    to be able to use the 7-row keyboard once again

reborn as thinkpad anniversary edition 25
    but it is just that, the one and only

like the shooting star soared through the darkest night
    so bright but so short

after using the 7-row keyboard
    you will see thinkpad's unique insights on keyboards

you will see how the full-size keyboard can be concentrated
    it has been 1991 days since the beginning
```
(paraphrased from <https://tex.com.tw/pages/back-to-the-future>)

![](https://upload.wikimedia.org/wikipedia/commons/0/05/TORU_docking_system.jpg)

![](https://upload.wikimedia.org/wikipedia/commons/b/b9/Wikimania_hackathon_1.JPG)

### a windowing system

- xmonad
- paperWM

### a browser language 

- JavaScript (TODO) 
    - <https://www.seas.upenn.edu/~cis197/>

### a CI/CD pipeline

- GitLab (TODO) 
    - <https://docs.gitlab.com>

### a systems language

 "for creating servers, daemons, and other code that wants to go fast, use little memory, have few dependencies, and interact tightly with the OS"

- C++ (TODO)
    - <https://www.seas.upenn.edu/~cis190/>
- Go (TODO)
    - <https://www.seas.upenn.edu/~cis193/>

### an interactive debugger for native executables

- GDB: The GNU Project Debugger (TODO)
    - <https://www.gnu.org/software/gdb/documentation>

