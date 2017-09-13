.. _how-to-publish-rtfd:

===========================================
Publish your documentation on Read the Docs
===========================================

..  warning::

    This section is incomplete.


We'll assume you've already:

* :ref:`customised your documentation <how-to-adapt>`
* created content
* checked that it build and passes tests.

..  admonition:: If you're not using Git/GitHub

    In this how-guide it's assumed that you'll be using Git and GitHub. You don't have to use
    either. Read the Docs will work with several other version control systems, but you'll need
    to adapt these steps appropriately.

#.  Create a repository for your project on GitHub. You don't need to add a README, as your
    documentation will already have one.
#.  Add the repository as a remote. Let's suppose that your name is Jean, ::

        git remote add jean <github URL>
        git commit -a
        git push origin master
#.  Create the documentation project on Read the Docs
