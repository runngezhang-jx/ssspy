.. ssspy documentation master file, created by
   sphinx-quickstart on Fri Apr 29 20:59:12 2022.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to ssspy's documentation!
=================================

.. image:: https://readthedocs.org/projects/sound-source-separation-python/badge/?version=latest
   :target: https://sound-source-separation-python.readthedocs.io/en/latest/?badge=latest

.. image:: https://github.com/tky823/ssspy/actions/workflows/lint.yaml/badge.svg
   :target: https://github.com/tky823/ssspy/actions/workflows/lint.yaml

.. image:: https://codecov.io/gh/tky823/ssspy/branch/main/graph/badge.svg?token=IZ89MTV64G
   :target: https://codecov.io/gh/tky823/ssspy

``ssspy`` is a Python toolkit for sound source separation.

Build status
------------

+--------+--------------------------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------+
| Python | Ubuntu                                                                                                                         | MacOS (x86_64)                                                                                                            | MacOS (arm64)                                                                                                                 | Windows                                                                                                                         |
+--------+--------------------------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------------+
| 3.9    | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_ubuntu-latest_python-3.9.yaml/badge.svg?branch=main  | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-13_python-3.9.yaml/badge.svg?branch=main  | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-latest_python-3.9.yaml/badge.svg?branch=main  | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_windows-latest_python-3.9.yaml/badge.svg?branch=main  |
|        |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_ubuntu-latest_python-3.9.yaml                       |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-13_python-3.9.yaml                       |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-latest_python-3.9.yaml                       |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_windows-latest_python-3.9.yaml                       |
+--------+--------------------------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+---------------------------------+
| 3.10   | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_ubuntu-latest_python-3.10.yaml/badge.svg?branch=main | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-13_python-3.10.yaml/badge.svg?branch=main | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-latest_python-3.10.yaml/badge.svg?branch=main | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_windows-latest_python-3.10.yaml/badge.svg?branch=main |
|        |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_ubuntu-latest_python-3.10.yaml                      |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-13_python-3.10.yaml                      |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-latest_python-3.10.yaml                      |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_windows-latest_python-3.10.yaml                      |
+--------+--------------------------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+---------------------------------+
| 3.11   | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_ubuntu-latest_python-3.11.yaml/badge.svg?branch=main | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-13_python-3.11.yaml/badge.svg?branch=main | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-latest_python-3.11.yaml/badge.svg?branch=main | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_windows-latest_python-3.11.yaml/badge.svg?branch=main |
|        |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_ubuntu-latest_python-3.11.yaml                      |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-13_python-3.11.yaml                      |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-latest_python-3.11.yaml                      |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_windows-latest_python-3.11.yaml                      |
+--------+--------------------------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+---------------------------------+
| 3.12   | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_ubuntu-latest_python-3.12.yaml/badge.svg?branch=main | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-13_python-3.12.yaml/badge.svg?branch=main | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-latest_python-3.12.yaml/badge.svg?branch=main | .. image:: https://github.com/tky823/ssspy/actions/workflows/test_package_windows-latest_python-3.12.yaml/badge.svg?branch=main |
|        |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_ubuntu-latest_python-3.12.yaml                      |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-13_python-3.12.yaml                      |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_macos-latest_python-3.12.yaml                      |    :target: https://github.com/tky823/ssspy/actions/workflows/test_package_windows-latest_python-3.12.yaml                      |
+--------+--------------------------------------------------------------------------------------------------------------------------------+---------------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+---------------------------------+

Installation
------------

You can install ``ssspy`` by pip.

.. code-block:: shell

   pip install ssspy

To install latest version,

.. code-block:: shell

   pip install git+https://github.com/tky823/ssspy.git

Instead, you can build package from source.

.. code-block:: shell

   git clone https://github.com/tky823/ssspy.git
   cd ssspy
   pip install -e .

.. note::

   If you fail to install ``ssspy``, please update ``setuptools`` by

   .. code-block:: shell

      python -m pip install --upgrade setuptools

.. note::

   If you cannot install `ssspy` due to failure in building wheel for numpy, please install numpy in advance.
   
Build Documentation Locally (optional)
--------------------------------------
To build the documentation locally, you have to include ``docs`` and ``notebooks`` when installing ``ssspy``.

.. code-block:: shell

   pip install -e ".[docs,notebooks]"

You need to convert some notebooks by the following command:

.. code-block:: shell

   . ./docs/pre_build.sh

When you build the documentation, run the following command.

.. code-block:: shell

   cd docs/
   make html

Or, you can build the documentation automatically using ``sphinx-autobuild``.

.. code-block:: shell

   # in ssspy/
   sphinx-autobuild docs docs/_build/html

.. toctree::
   :maxdepth: 1
   :caption: Contents:

   _notebooks/Getting-Started.rst
   changelog
   api


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
