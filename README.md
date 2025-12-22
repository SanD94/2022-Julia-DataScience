[![nbviewer](https://github.com/jupyter/design/blob/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/JuliaAcademy/DataScience/)

# Julia for Data Science
Prepared by [@nassarhuda](https://github.com/nassarhuda). 

Last updated: Dec 2025. Julia version used: 1.11.5

Accompanying videos are available at [JuliaAcademy](https://juliaacademy.com/p/julia-for-data-science).

There are three main components in this tutorial.
- Data (1 notebook) => Not necessary to watch the video for this part, self-explained
- Methods (10 notebooks)
- Visualization (1 notebook)

If one wants to integrate with `R`, they can use the `RCall` package but there is a catch.
The `$LD_LIBRARY_PATH` has to be set before running notebooks that use `RCall`. If, i.e., vscode is used, it should be set before opening it from the terminal.

Another catch is about Python. Normal packages would use miniconda or conda to isolate package use from the system. If one does not want this kind of separation, as it's not easy to manage what is where, set the system python as default by exporting and run `Pkg.build("PyCall")`.

```sh
export R_HOME=`R RHOME`
export LD_LIBRARY_PATH=$R_HOME/lib:$LD_LIBRARY_PATH
export PYTHON=`which python`
code .
```



----------------------------
# What is covered

Every data science task has one main ingredient, the **data**! Most likely, you want to use your data to learn something new. But before the **new** part, what about the data you already have? This is why our first section is on _Data_.  

### Data
In the first part we will make sure you can
- read and save your data via various File I/O options
- store, reformat, and process your data using different data structures.

---

Next, popular methods and tools used in Data Science are covered.

### Methods
In this section, the tools one needs to use Julia as a programming language for data science tasks
are provided. This includes
- understanding how Linear Algebra and Statistics tasks are performed in Julia
- going through some of the most popular data science methods such as classification, regression, clustering, and more.
- calling existing Python, R, or C code from Julia.
-----
And finally, a few tips and tricks to generate good looking and informative visualizations are given.
### Visualization
Note that the methods section show several kinds of plots too. But here, other plotting tools are introduced. This includes
- statistics plots
- managing the axes (double axes)
- showing error bars
- managing colors and color schemes
- plot annotations.

--------
### This is what one should expect in every notebook
<img src="data/format.png" width="400">

-----
#### And finally... Enjoy the tutorial!
