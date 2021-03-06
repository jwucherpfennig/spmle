spmle
================
Philipp Hunziker
November 25, 2018

System Requirements
===================

Python 2.7 (tested) or Python 3.6 (not tested). Also, [conda](https://conda.io/docs/user-guide/install/windows.html) if on Windows.

Installation
============

Install `spmle` directly from this repository:

``` r
devtools::install_github("hunzikp/spmle")
```

In case you don't have scipy and numpy installed (or don't know what these are), run the following in an R console:

``` r
spmle::install_pydep()
```

The command installs the Python dependencies in the `r-reticulate` virtual environment.

Usage
=====

To use the package you need to specify a python binary or virtual environment where scipy and numpy are installed. If use used the `install_pydep()` command from above:

``` r
library(reticulate)
library(spmle)
reticulate::use_virtualenv("r-reticulate")  # In Unix
reticulate::use_condaenv("r-reticulate")  # In Windows
```

Examples
========

See [here](scripts/mbdm_testing.md).
