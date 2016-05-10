.. image:: http://mybinder.org/badge.svg
    :target: http://mybinder.org/repo/qinfer/qinfer-examples

# QInfer Examples #

This repository hosts several Jupyter notebooks detailing how to use **QInfer**.
These examples can be viewed online using
[nbviewer](http://nbviewer.jupyter.org/github/qinfer/qinfer-examples/tree/master/),
and can be used interactively online with [binder](http://mybinder.org/repo/qinfer/qinfer-examples).
Instructions for running these examples on your own computer are provided below.

# Running Examples #

## Anaconda Environment ##

To run the example notebooks provided in this repository, we suggest
using Python 3 with the [Anaconda distribution](https://www.continuum.io/downloads) for
Linux and OS X, or Python 2 with Anaconda for Windows. To get started, [download the
latest notebooks from GitHub](https://github.com/QInfer/qinfer-examples/archive/master.zip),
or clone the repository using Git:

.. code-block:: bash

    $ git clone https://github.com/QInfer/qinfer-examples.git

We have provided an Anaconda environment for use with these notebooks. This
environment currently does not work on Windows, so please follow the manual
installation instructions below to use these notebooks on Windows. To install
the environment and all required software (NumPy/SciPy, QuTiP, Pandas and
Mpltools), use the ``conda`` tool provided with Anaconda.

.. code-block:: bash

    $ cd qinfer-examples
    $ conda env create -f environment.yml

Next, activate the environment and run Jupyter Notebook.

    $ source activate qinfer-examples
    $ jupyter notebook

When you are done, you can deactivate the new environment, leaving
your Anaconda configuration unchanged.

    $ source deactivate

## Manual Installation ##

The examples provided in this repository demonstrate using **QInfer** with
other libraries, such as [QuTiP](http://qutip.org), such that these libraries
must be installed first to use the example notebooks. The instructions below
detail how to do so with Anaconda for Python 2.7 or 3.5 on Linux or OS X, and
with Anaconda for Python 2.7 on Windows. Note that these instructions assume
that you have Git installed; on Windows, Git can be installed from the
`official downloads <https://git-scm.com/downloads>`_.

.. code-block:: bash

    $ conda install numpy scipy pandas configobj jupyter
    $ conda install -c conda-forge qutip
    $ pip install mpltools
    $ pip install git+https://github.com/QInfer/python-qinfer.git

Once everything has been installed, the examples can be run by using Jupyer
Notebook:

.. code-block:: bash

    $ cd qinfer-examples
    $ jupyter notebook

