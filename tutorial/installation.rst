.. _tutorial-installation:

===========
Get started
===========

Download the documentation
==========================

Clone it from its Git repository::

    git clone git@github.com:evildmp/daniele-procida-starter-docs.git

If you have Git installed, but haven't yet set up your public key on your
GitHub account, use the HTTPS URL instead::

    git clone https://github.com/evildmp/daniele-procida-starter-docs.git

If you don't have Git installed at all, you can `download the files instead
<https://github.com/evildmp/daniele-procida-starter-docs/archive/master.zip>`_.

However, since using Git (or some other kind of version control) will be very
useful in maintaining your own documentation, it's recommended to take the
trouble to get started with Git if you can.


Run the install script
======================

The install script is handled by the documentation's `Makefile
<https://github.com/evildmp/daniele-procida-starter-docs/blob/master/Makefile>`_
. It creates a Python virtual environment (so that it won't affect anything
else on your system) and installs the necessary components into the new virtual
environment.

``cd`` into the the newly-created ``daniele-procida-starter-docs`` directory,
and run ``make install``::

    ➜  cd daniele-procida-starter-docs
    ➜  daniele-procida-starter-docs make install
    ... setting up virtualenv
    virtualenv env
    [...]
     ---------------------------------------------------------------
     * watch, build and serve the documentation: make run
     * check spelling: make spelling

     enchant must be installed in order for pyenchant (and therefore
     spelling checks) to work.
     ---------------------------------------------------------------


Build the documentation
=======================

``make html`` will build the HTML version of the documentation::

    ➜  daniele-procida-starter-docs make html
    . env/bin/activate; sphinx-build -M html "." "_build"
    Running Sphinx v1.6.3
    [...]
    Build finished. The HTML pages are in _build/html.


Open the documentation site
===========================

``make open`` will open the newly-created site, which can be found at
``_build/html/index.html``, in your browser.


Run the documentation site
==========================

An even more elegant way of building it is with the ``make run`` command,
which not only builds it but will automatically rebuild it each time you
make any changes, and even refresh the site if it's open in your browser::

    ➜  daniele-procida-starter-docs make run
    . env/bin/activate; sphinx-autobuild  . -a _build/html --host 0.0.0.0 --port 8001
    [...]
    [I 170912 15:28:34 server:283] Serving on http://0.0.0.0:8001
    [I 170912 15:28:34 handlers:60] Start watching changes
    [I 170912 15:28:34 handlers:62] Start detecting changes

As you can see, the site is available at http://0.0.0.0:8001.

Now's a good time to take a look around the site. Perhaps begin by reading
:ref:`about-the-structure`, which explains why this documentation is structured
like it is - and why yours should be too.

Then when you're ready, you can continue with the tutorial. The next step is to start making the
documentation your own. Alternatively, you can explore some of the other things you can do.
