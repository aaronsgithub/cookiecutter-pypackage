======================
cookiecutter-pypackage
======================

Simple cookiecutter template for a Python package.

Features
--------

* Free software: BSD license
* Pytest_ runner: Supports `unittest`, `pytest`, `nose` style tests and more
* Travis-CI_: Ready for Travis Continuous integration testing
* Tox_ testing: Setup to easily test for python 2.6, 2.7, 3.3, 3.4 and PyPy_
* Sphinx_ docs: Documentation ready for generation with, for example, ReadTheDocs_
* Wheel_ support: Use the newest python package distribution standard from the get go

Usage
-----

Generate a Python package project::

    cookiecutter https://github.com/aaronsgithub/cookiecutter-pypackage.git

Documentation
^^^^^^^^^^^^^

This cookiecutter template generates sensible defaults for a package author to begin writing documentation. The files are set to obey the "Don't Repeat Yourself" or "DRY" principle, and are integrated with the package distribution's setup.py file so that relevant information is added to the package distribution's metadata.

In terms of documentation, the root directory of the package distribution will contain:

* A README.rst - to provide a summary and any other key information to potential users of the package distribution.
* A HISTORY.rst file - to be updated with a summary of changes to the package distribution for each release.
* A LICENSE file - set up to produce a copy of the BSD license.
* A "docs" directory - set up to begin writing detailed documentation with Sphinx. More information on the default settings provided for Sphinx is given below.

Default Sphinx Configuration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This cookiecutter template will generate some sensible defaults for Sphinx documentation in the docs directory. These defaults can easily be adjusted by changing settings in the conf.py file within the docs directory.

The docs directory will contain:

* A conf.py file - containing the initial settings for Sphinx
* A Makefile - which provides a number of commands and shortcuts when used with the Make utitlity
* A make.bat file - which provides similar functionality to the Makefile for users on Windows.
* An index.rst file - the master document of Sphinx documentation. Includes the Sphinx directive "toctree" to generate the table of contents.
* A history.rst file - which pulls in the contents of HISTORY.rst from the root directory to keep things DRY.

Sphinx extensions enabled by default:

* Autodoc
* Coverage
* Viewcode

The documentation is set up to use the "Readthedocs" theme for its HTML output.

For more information on how to use Sphinx, including how to add to the documentation already generated, please consult the `Sphinx documentation <http://sphinx-doc.org/>`_.


Dependencies
------------

* wheel==0.24.0
* Sphinx==1.3.1
