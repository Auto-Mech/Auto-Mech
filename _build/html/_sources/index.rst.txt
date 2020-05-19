.. AutoMech documentation master file, created by
   sphinx-quickstart on Sat Jan  4 14:21:30 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Auto Mech
=========

What is Auto Mech?
~~~~~~~~~~~~~~~~~~

.. Some filler text to fill in later (also, this is how to put comments here).

A high-level description of the code goes here.

.. figure:: figs/paper-graphic.png
    :width: 80%


The Code Structure of Auto Mech
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. The syntax for linking to other documentation is :doc:`text <path/to>`

The overall workflow of Auto Mech is driven by
:doc:`moldriver <./repos/moldriver/docs/index>`,
whose overarching task is to invoke electronic structure calculations through
the
:doc:`elstruct <./repos/elstruct/docs/index>`
interface and feed the results into
:doc:`MESS <./repos/MESS/docs/index>`
for calculating partition functions and kinetic rates.

Data generated during the workflow is written to a file system database using
the
:doc:`autofile <./repos/autofile/docs/index>`
module, which also provides functions for retrieving previously stored data.

The aforementioned codes are supported by several helper libraries:

    * :doc:`automol <./repos/automol/docs/index>` provides routines for
      manipulating and interconverting between molecular descriptors (Cartesian
      geometry, z-matrix, molecular graph, InChI, SMILES, molecular formula)
    * :doc:`interfaces <./repos/interfaces/docs/index>` contains a hodge-podge
      of interaces to various programs
    * :doc:`autoparse <./repos/autoparse/docs/index>` is a low-level parsing
      library employed by the various I/O modules

The following schematic summarizes this general overview.

.. figure:: figs/code-structure.png
    :width: 80%

.. toctree::
    :maxdepth: 1
    :caption: Contents:

    repos/moldriver/docs/index

    repos/autofile/docs/index
    repos/MESS/docs/index
    repos/elstruct/docs/index

    repos/automol/docs/index
    repos/autoparse/docs/index
    repos/interfaces/docs/index



Indices and tables
~~~~~~~~~~~~~~~~~~

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
