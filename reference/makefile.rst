================
The ``Makefile``
================

..  important::

    The ``Makefile`` in the project works - but could certainly be improved.
    If you have some ``Makefile`` expertise, please help!


The project's ``Makefile`` encapsulates the commands you'll need to use most
often when working with the documentation tools. Each one can be invoked from
the documentation's root directory with ``make``, followed by the command - for
example::

    make html

Available commands are:

``install``
    Creates a new Python virtualenv called ``env``, and installs the
    packages listed in ``requirements.txt`` into it. They are::

        sphinx
        sphinxcontrib-spelling
        pyenchant
        sphinx-autobuild
        sphinx_rtd_theme

``html``
    Activates the virtualenvironment, then builds the HTML documentation, in
    ``_build/html``. The home page is ``_build/html/index.html``.

``open``
    Opens ``_build/html/index.html`` - with luck, in your browser.

``run``
    Activates the virtualenvironment, then builds the documentation, and serves
    it at http://localhost:8001.

.. _make-clean:

``clean``
    Deletes the ``_build/html`` directory.

``spelling``
    Activates the virtual environment, then checks spelling in the documentation.
