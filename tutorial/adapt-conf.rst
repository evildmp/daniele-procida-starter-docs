.. _tutorial-adapt-conf:

==========================
Adapt the ``conf.py`` file
==========================

As well as your own content, you're going to need to add your own configuration
data to the project, in its :ref:`conf <conf.py>` file.

In the examples below, we'll assume your name is *Muriel Spark* and your
project is called *The driving seat*. The examples are mainly for illustration,
as it's easy enough to discern from the existing examples how to arrive at the
correct form.

You will need to change the following sections appropriately.

Name/authorship changes
-----------------------

These sections will be used to display name/authorship information throughout
the documentation, when it's built in different forms. Depending on what you do
with your documentation, the Latex and other output forms may never be used but
you may as well have them set up correctly.


General information
~~~~~~~~~~~~~~~~~~~

::

    project = u"Daniele Procida's documentation starter kit"
    copyright = u"2017, Daniele Procida"
    author = u"Daniele Procida"

becomes::

    project = u"The driving seat"
    copyright = u"2017, Muriel Spark"
    author = u"Muriel Spark"


htmlhelp_basename
~~~~~~~~~~~~~~~~~

::
    htmlhelp_basename = 'DanieleProcidasdocumentationstarterkitdoc'

becomes::

    htmlhelp_basename = 'Thedrivingseatdoc'


Latex information
~~~~~~~~~~~~~~~~~

::

    latex_documents = [(
        master_doc,
        "DanieleProcidasdocumentationstarterkit.tex",
        u"Daniele Procida's documentation starter kit Documentation",
        u"Daniele Procida", "manual"
    ),]

becomes::

    latex_documents = [(
        master_doc,
        "Thedrivingseat.tex",
        u"The driving seat Documentation",
        u"Muriel Spark", "manual"
    ),]


Manual pages information
~~~~~~~~~~~~~~~~~~~~~~~~

::

    man_pages = [(
        master_doc,
        "danieleprocidasdocumentationstarterkit",
        u"Daniele Procida's documentation starter kit",
        [author], 1
    )]

becomes::

    man_pages = [(
        master_doc,
        "thedrivingseat",
        u"The driving seat",
        [author], 1
    )]


Texinfo information
~~~~~~~~~~~~~~~~~~~

::

    texinfo_documents = [(
        master_doc,
        "DanieleProcidasDocumentationStarterKit",
        u"Daniele Procida's documentation starter kit",
        author,
        "Daniele Procida",
        "One line description of project.",
        "Miscellaneous"
    ),]

becomes::

    texinfo_documents = [(
        master_doc,
        "Thedrivingseat",
        u"The driving seat",
        author,
        "Muriel Spark",
        "One line description of project.",
        "Miscellaneous"
    ),]


Version information
-------------------

If your documentation is part of a software release (i.e. part of the source
code for the project), or is tied to a software release, its version/release
numbers should follow those of the software *exactly* - ideally, by
:ref:`reading this from the software itself <automatic_version_number>`.

Otherwise, just keep them updated in a sensible way.

The ``version`` is a short ``x.y`` number. The ``release`` is a full ``x.y.z``,
and can include ``alpha``/``beta``/``rc`` tags. (If you're not using ``x.y.z``
numbering just make the ``release`` the same as the ``version``.)

Example::

    version = u'2.1'
    release = u'2.1.3rc1'
