.. _headings:

========================
Page titles and headings
========================

Headings and titles (titles are really just headings, as far as RST is concerned) are declared by
underlining/overlining. It doesn't matter too much exactly what style you use, but it should be
consistent.

Page titles
===========

Each page in this documentation contains a page title::

    ==========
    Page title
    ==========


Headings
========

The heading above is a first level heading. Headings in this documentation are as follows:

::

    First level heading
    ===================

    Second level heading
    --------------------

    Third level heading
    ~~~~~~~~~~~~~~~~~~~

    Fourth level heading
    ^^^^^^^^^^^^^^^^^^^^

    Fifth level heading
    ...................


First level heading
===================

Second level heading
--------------------

Third level heading
~~~~~~~~~~~~~~~~~~~

Fourth level heading
^^^^^^^^^^^^^^^^^^^^

Fifth level heading
...................


..  note::

    These five levels, plus the title, add up to six levels of heading, and thus exhaust HTML's
    heading specification. You could add another level in your document, with for example::

        Sixth level heading
        '''''''''''''''''''

    but since there is no ``<h7>`` in HTML, it won't be a meaningful construct in the output.
