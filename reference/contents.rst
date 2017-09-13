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
            }
            .column2 {width: 50%;}
            .column3 {width: 33%;}
            .column4 {width: 25%;}
        }
    </style>


.. _toc-ref:

==================
Tables of contents
==================

A table of contents is the basis for building the navigation around your documentation.

It's created by the ``toctree`` directive, followed by a list of the things you want to appear in
that particular table of contents. If a page has headings, those headings will also be listed,
creating a tree structure. Unless otherwise specified (using ``:maxdepth:``), the table of contents
will list items to indefinite depth in the tree.

In this project you'll find a ``toctree`` on the ``index.rst`` page of each section, so the overall
project structure looks like this::

    index.rst/
        explanation/
            index.rst
            about-the-structure.rst
        how-to/
            index.rst
        reference/
            index.rst
            conf.rst
            contents.rst
            headings.rst
            makefile.rst
            miscellaneous.rst
            notes-warnings.rst
        tutorial/
            index.rst
            installation.rst


Examples
========

A simple table of contents
--------------------------

Limited to a depth of 1, listing the items we require, similar to the one used in the :ref:`main
page of this section <reference>`.


.. rst-class:: clearfix row column column2

Markup
^^^^^^

::

    ..  toctree::
        :maxdepth: 1

        headings
        notes-warnings
        miscellaneous
        makefile


.. rst-class:: column column2

Output
^^^^^^

..  toctree::
    :maxdepth: 1

    headings
    notes-warnings
    miscellaneous
    makefile

..  Why doesn't the example above contain the contents page (i.e. this page)?

    This is Sphinx would run into a circular reference and raise a warning.

.. rst-class:: clearfix row

Numbered tables of contents
---------------------------

See the :ref:`tutorial's table of contents <tutorial-contents>` for an example.

.. rst-class:: clearfix row column column2

Markup
^^^^^^

::

    ..  toctree::
        :maxdepth: 1
        :numbered:

        installation


.. rst-class:: column column2

Output
^^^^^^

..  toctree::
    :maxdepth: 1

    ../tutorial/installation

..  Why doesn't the actual code above use the :numbered: option?

    This is because the tutorial already has section numbers assigned and this would raise a
    warning.


Other ways of listing items
---------------------------

Markup
^^^^^^

::

    ..  toctree::
        :maxdepth: 1

        Notes and warnings <notes-warnings>  # a custom title
        ../explanation/about-the-structure   # traversing the directory structure
        https://apple.com                    # a URL
        Github <https://github.com>          # a URL with a custom title

Output
^^^^^^

..  toctree::
    :maxdepth: 1

    Notes and warnings <notes-warnings>
    ../explanation/about-the-structure
    https://apple.com
    Github <https://github.com>

..  warning::

    Traversing the directory structure or adding external URLs to your tables of content are
    good ways to confuse both your reader and yourself. There's no good reason to do either of
    them.

..  admonition:: Sphinx documentation

    `The TOC tree <http://www.sphinx-doc.org/en/stable/markup/toctree.html>`_
