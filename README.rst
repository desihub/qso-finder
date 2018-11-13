============
qso_priority
============

Introduction
============

This repository contains software to change the priority of re-observation for QSO
Ly-alpha targets according to their cosmological value predicted using the Fisher-matrix
formalism.

Installation
============

This package is `pip` installable:

    `pip install git+https://github.com/desihub/qso-finder.git@0.1.0`

At NERSC_, DESI_ products should be installed with desiInstall.  The main purpose
of desiInstall is to ensure that different versions of a package are kept
separate and to install `Module files`_.  desiInstall is not part of this package,
but part of desiutil_.

The package can also be installed using:

    `python setup.py install --prefix=$PREFIX`

Unit tests are provided. To run these tests run `python setup.py test`.


Product Contents
================

Directory Structure
-------------------

bin/
    This directory contains the executable scripts (for now this is a dummy).
doc/
    Contains high-level documentation of the software.
etc/
    This directory contains the data file with the Fisher-predicted cosmological
    value of the QSOs as a function of their redshift and r-band magnitude.
py/
    Contains Python code.  Top-level Python package directories should be
    placed *within* the ``py/`` directory.  This simplifies the specification
    of the ``$PYTHONPATH`` variable.

LICENSE
~~~~~~~

This product includes a 3-clause BSD-style license, the
standard adopted by DESI.


.. image:: https://coveralls.io/repos/github/desihub/qso-finder/badge.svg?branch=master
:target: https://coveralls.io/github/desihub/qso-finder?branch=master

.. image:: https://travis-ci.org/desihub/qso-finder.svg?branch=master
    :target: https://travis-ci.org/desihub/qso-finder
