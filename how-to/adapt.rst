.. _how-to-adapt:

============================
How to adapt the starter kit
============================

..  warning::

    This section is incomplete.


Set the version number
======================

..  _automatic_version_number:

Set the version number automatically
------------------------------------

If you're documenting a project in Python, it would be sensible to use Python
to read the version number directly from your software, so that you don't need
to update it manually.

If your documentation is in a directory at the root of your Python package, and
the application containing the version number you want to extract is called
``my_application`` and has a ``__version__`` attribute, you could do::

    path = os.path.split(os.path.dirname(__file__))[0]
    path = os.path.split(path)[0]
    sys.path.insert(0, path)
    import my_application

    version = my_application.__version__
    release = my_application.__version__
