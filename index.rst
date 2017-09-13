.. raw:: html

    <style>
        .row {clear: both}

        .column img {border: 1px solid black;}

        @media only screen and (min-width: 1000px),
               only screen and (min-width: 600px) and (max-width: 768px){
            .column {
                padding-left: 5px;
                padding-right: 5px;
                float: left;
                width: 25%;
            }
        }
        h2 {border-top: 1px solid black; padding-top: 1em}
    </style>


===================================
Daniele's documentation starter kit
===================================

.. image:: /images/overview.png
   :alt: 'Overview of the structure'


..  warning::

    You're looking at a work in progress! Parts of this are incomplete, stop
    dead, are broken or might not even make complete sense...


Contents
========

.. rst-class:: clearfix row

.. rst-class:: column


:ref:`Tutorial <tutorial>`
--------------------------

Learn how to build, modify and deploy the documentation.


.. rst-class:: column

:ref:`How-to guides <how-to>`
-----------------------------

Step-by-step guides covering key particular tasks


.. rst-class:: column

:ref:`Reference <reference>`
----------------------------

Technical reference - tools, components and commands


.. rst-class:: column

:ref:`Explanation <explanation>`
--------------------------------

Explanation and discussion of key topics


.. rst-class:: clearfix row

About the Documentation Starter Kit
===================================

The `Documentation Starter Kit <https://divio.com>`_ aims to solve several of
the key problems software project maintainers who need to manage the project's
documentation. It's a set of files to help software documentation authors make
a quick start, with a clean, well-structured project.

The project includes tooling to set itself up, and build the documentation,
publishing it as a self-contained HTML website.

It's easy to use as the basis for your own, real documentation, and is ready to
be published on `Read the Docs <https://readthedocs.org>`_.

The kit uses:

* ReStructured Text (RST)
* Sphinx
* Git and GitHub
* Read the Docs
* A prescribed documentation structure

All you need to do is make a copy of the Kit, and start editing and adding your
own material to it. When you're ready, send it to Read the Docs, and you'll
have good looking, easy-to-maintain and feature-rich public documentation for
your project.

Even with minimal quantity of actual documentation content, you'll have
a structure and tools that will help you add to it in rational, obvious ways,
and will ancourage others to contribute to it too.

Go straight to the :ref:`tutorial` for a complete step-by-step guide through the
entire process.

The kit was developed at `Divio <https://divio.com>`_ by Daniele Procida.

See :ref:`users` for examples of documentation that use the principles and
tools used in the kit.

..
    The Table of Contents below is hidden, using :hidden:. We need it to exist,
    in order to generate the table of contents in the sidebar, but we don't
    want it to appear in the middle of this page.

.. toctree::
    :maxdepth: 2
    :hidden:

    tutorial/index
    how-to/index
    reference/index
    explanation/index