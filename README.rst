Abydos
======

.. image:: https://travis-ci.org/chrislit/abydos.svg
    :target: https://travis-ci.org/chrislit/abydos
    :alt: Build Status

.. image:: https://coveralls.io/repos/chrislit/abydos/badge.svg
    :target: https://coveralls.io/r/chrislit/abydos
    :alt: Coverage Status

.. image:: https://codeclimate.com/github/chrislit/abydos/badges/gpa.svg
   :target: https://codeclimate.com/github/chrislit/abydos
   :alt: Code Climate

.. image:: https://landscape.io/github/chrislit/abydos/master/landscape.svg?style=flat
   :target: https://landscape.io/github/chrislit/abydos/master
   :alt: Code Health

.. image:: https://img.shields.io/badge/Pylint-9.99/10-green.svg
    :alt: Pylint Score

.. image:: https://img.shields.io/badge/PEP8-0-brightgreen.svg
    :alt: PEP8 Errors

.. image:: https://img.shields.io/pypi/v/abydos.svg
    :target: https://pypi.python.org/pypi/abydos
    :alt: PyPI

.. image:: https://readthedocs.org/projects/abydos/badge/?version=latest
    :target: https://abydos.readthedocs.org/en/latest/
    :alt: Documentation Status

.. image:: https://www.openhub.net/p/abydosnlp/widgets/project_thin_badge.gif
    :target: https://www.openhub.net/p/abydosnlp
    :alt: OpenHUB

.. image:: https://badges.gitter.im/Join%20Chat.svg
   :alt: Join the chat at https://gitter.im/chrislit/abydos
   :target: https://gitter.im/chrislit/abydos?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
   
|

.. image:: https://raw.githubusercontent.com/chrislit/abydos/master/abydos-small.png
    :alt: abydos
    :align: right

|
| Abydos NLP/IR library
| Copyright 2014-2015 by Chris Little

This library contains code I'm using for research, in particular dissertation research & experimentation.

Required:

- Numpy

Recommended:

- PylibLZMA   (Python 2 only--for LZMA compression string distance metric)

Suggested for development, testing, & QA:

- Nose        (for unit testing)
- coverage.py (for code coverage checking)
- Pylint      (for code quality checking)
- PEP8        (for code quality checking)

-----

Installation
============

To install Abydos from PyPI using pip::

   pip install abydos

It should run on Python 2.7 and Python 3.3+


To build/install/unittest from source in Python 2::

    sudo python setup.py install
    nosetests -v --with-coverage --cover-erase --cover-html --cover-branches --cover-package=abydos .

To build/install/unittest from source in Python 3::

    sudo python3 setup.py install
    nosetests3 -v --with-coverage --cover-erase --cover-html --cover-branches --cover-package=abydos .

For pylint testing, run::

    pylint --rcfile=pylint.rc abydos > pylint.log

A simple shell script is also included, which will build,
install, test, and code-quality check (with Pylint & PEP8)
the package and build the documentations. To run it, execute::

    ./btest.sh
