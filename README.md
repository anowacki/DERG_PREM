# DERG_PREM: Interrogating PREM

This repo contains Jupyter notebooks to interrogate PREM as part of
the University of Leeds's
[Deep Earth Research Group](https://environment.leeds.ac.uk/institute-geophysics-tectonics/doc/deep-earth)
meetings.  It uses [Julia](https://julialang.org) code to do this.

## Installation instructions

### Note about Python
The TauPy package uses Obspy's `taup` module, and by default installs
this for you in a separate Julia-specific Miniconda installation.
If you have a working install of Python with Obspy and geographiclib
that you'd rather re-use, then you can do that.
In that case, set the environment variable `$PYTHON` to the path to your
Python executable.  In step 4, the Python in `$PYTHON` will then be used
instead of the default Miniconda install.

If the above makes no sense, ignore it and move on.

### Installation steps
0. [Install the latest version of Julia](https://julialang.org/downloads) if
   you haven't already.  v1.3 is strongly recommended for this project.
1. Clone this repo:

    $ git clone https://github.com/anowacki/DERG_PREM

2. `cd` to the repo directory.
3. Launch julia and activate the project:

    ```$ julia --project```
4. Install all dependencies:

    ```julia> import Pkg; Pkg.instantiate()```
5. Open the Jupyter interface:

    ```julia> import IJulia; IJulia.notebook(dir=".")```

(Note that the very first time you do most things in Julia, precompilation
and caching happen, so things will take a little while.  Be patient, and
feel assured that the second time you do things, it will be faster!)

## Running instructions

Repeat steps 1, 2 and 4 above each time you want to launch a Jupyter
notebook within this environment.
