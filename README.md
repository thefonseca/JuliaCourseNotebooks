# JuliaCourseNotebooks

## Setup environment using Conda
These steps were tested on macOS 10.15.4.

1. Install Anaconda or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
2. Create and activate the `julia` environment:
```
conda create -n julia
conda activate julia
```
3. Install Jupyter and Julia (from conda-forge):
```
conda install jupyter
conda install -c conda-forge julia==1.1.1
```
3. Enter the [Julia REPL](https://docs.julialang.org/en/v1/stdlib/REPL/):
```
julia
```
4. Install the [Julia kernel for Jupyter](https://github.com/JuliaLang/IJulia.jl):
```
using Pkg
Pkg.add("IJulia")
# exit Julia REPL
exit()
```
5. Run Jupyter
```
jupyter notebook
```
A new browser window/tab will be opened and you should see an option to create a new "Julia" notebook.

---

Jupyter notebooks and Juno .jl files for the Julia Scientific Programming course on Coursera

The recently released version 1.0 of Julia marked a milestone in the development of the language.  Julia has been a rapidly evolving language.  This creates challenges when teaching Julia.  Over the next few weeks and month the course code will be adapted to comply with the changes introduced in Julia 1.0 (0.7).

**Juno** is the integrated development environment (IDE) choice for Julia.  It is built on the Atom IDE.  As of the time of writing of this README file, Julia Computing still releases version 0.6.4 of Julia.  To use Julia 1.0, dowload it from https://julialang.org.  Also dowload Atom from https://atom.io  In Atom hit the CONTROL key (or COMMAND key on a Mac) and the comma key.  This brings up the settings.  Under the Install tab search for *uber-juno* which will install the Julia interface for Atom.  When this is done, also add the address to the julia 1.0 executable on your computer.  Restart ATOM.

When creating a new file, save it first, explicitely using the .jl extension.  This will tell Atom to use the Julia interface.  Have a look at some of the new .jl files added to this repository.

Julia Computing ( https://www.juliacomputing.com ) releases of Julia contains the Juno interface.  We will let you know when the 1.0 release goes live.
