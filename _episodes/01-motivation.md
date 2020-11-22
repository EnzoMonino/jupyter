---
layout: episode
title: Motivation
teaching: 10
exercises: 0
questions:
  - What are Jupyter Notebooks?
  - What can Jupyter Notebooks be used for?
objectives:
  - Get an idea of the purpose of Jupyter.
  - See some inspirational Jupyter notebooks.
keypoints:
  - Jupyter is an open-source, interactive web tool allowing researchers
    to combine code, output, explanatory text and multimedia resources
    in a single document.
---

# Jupyter Notebooks

## Some history
- In 2014, Fernando Pérez announced a spin-off project from IPython called Project Jupyter, moving the notebook and other language-agnostic parts of IPython to Jupyter.
- The name "Jupyter" derives from Julia+Python+R, but today Jupyter kernels exist for [dozens of programming languages](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels).
- Galileo's publication in a pamphlet in 1610 in Sidereus Nuncius, one of the first notebooks!
<img src="http://media.gettyimages.com/photos/pages-from-sidereus-nuncius-magna-by-galileo-galilei-a-book-of-and-picture-id90732970" width="500">

---

## What are Jupyter notebooks?

- A [literate programming](https://en.wikipedia.org/wiki/Literate_programming) tool.
- Code, text, equations, figures, etc. are interleaved, creating a *computational narrative*.
- [*"an environment in which users execute code, see what happens, modify and repeat in a kind of iterative conversation between researcher and data"*](https://www.nature.com/articles/d41586-018-07196-1)

### Common use cases

- Experimenting with new ideas, testing new libraries/databases
- As an *interactive* development environment for code, data analysis and visualization
- Interactive work on HPC clusters
- Sharing and explaining code to colleagues
- Teaching (programming, experimental/theoretical science)
- Learning from other notebooks
- Keeping track of interactive sessions, like a digital lab notebook
- Supplementary information with published articles
- Slide presentations using [Reveal.js](https://github.com/damianavila/RISE)

### When not to use notebooks

- Less useful for large codebases
- More difficult to do automated testing on
- Tricky when it comes to non-linear execution of cells, discipline is needed
- We will discuss pitfalls later

---

## Two case examples

#### [Gravitational wave discovery](https://www.gw-openscience.org/about/)

<img src="{{ site.baseurl }}/img/MergingBlackHoles_V2.jpg" width="50%">

Let us have a look at the analysis published together with the
discovery of gravitational waves. [This
page](https://losc.ligo.org/tutorials/) lists the available analyses
and presents several options to browse them.

- A quick look at short segments of data can be found at
  [https://github.com/losc-tutorial/quickview](https://github.com/losc-tutorial/quickview)
- The notebook can be opened and interactively explored
  using Binder by clicking the "launch Binder" button.
- How does the Binder instance know which Python packages to load?


#### [Activity inequality](http://activityinequality.stanford.edu/)

<img src="{{ site.baseurl }}/img/activity_inequality.png" style="background-color:black;" width="80%">

Researchers in the Stanford Activity Inequality Study measured daily
activity from cell phone tracking data for over 700,000 users in
different countries across the world.
- All data and notebooks are available at
  [https://github.com/timalthoff/activityinequality](https://github.com/timalthoff/activityinequality)
- Even without a "launch binder" button, the notebooks can still be
  [launched on Binder](https://mybinder.org/v2/gh/timalthoff/activityinequality/master)
  (you may see an error "missing R kernel" because a file `runtime.txt` is missing - more about that later)
- Do you see any potential problems in recreating e.g.
  [fig3bc](https://github.com/timalthoff/activityinequality/blob/master/fig3/fig3bc.ipynb)?

---

For further inspiration, head over to the [Gallery of interesting Jupyter Notebooks](https://github.com/jupyter/jupyter/wiki/A-gallery-of-interesting-Jupyter-Notebooks).
