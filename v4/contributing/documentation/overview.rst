Contributing to the Documentation
=================================

Documentation is a very import part of a software. It follows some important principles:
DRY, tests, ease of maintenance, extensibility, optimization, and refactoring
just to name a few. And of course, documentation has bugs, typos, hard to read
tutorials, and more.

Contributing
------------

Before contributing, you need to become familiar with the :doc:`markup
language <format>` used by the documentation.

The CuteFlow documentation is hosted on GitHub:

.. code-block:: text

    https://github.com/cuteflow/cuteflow-documentation

If you want to submit a patch, `fork`_ the official repository on GitHub and
then clone your fork:

.. code-block:: bash

    $ git clone git://github.com/YOURUSERNAME/cuteflow-documentation.git

Next, create a dedicated branch for your changes (for organization):

.. code-block:: bash

    $ git checkout -b improving_foo_and_bar

You can now make your changes directly to this branch and commit them. When
you're done, push this branch to *your* GitHub fork and initiate a pull request.
The pull request will be between your ``improving_foo_and_bar`` branch and
the ``cuteflow-documentation`` ``master`` branch.

.. image:: /images/docs-pull-request.png
   :align: center

GitHub covers the topic of `pull requests`_ in detail.

.. note::

    The CuteFlow documentation is licensed under a Creative Commons
    Attribution-Share Alike 3.0 Unported :doc:`License <license>`.

Reporting an Issue
------------------

The most easy contribution you can make is reporting issues: a typo, a grammar
mistake, a bug in code example, a missing explanation, and so on.

Steps:

* Submit a bug in the bug tracker;

* *(optional)* Submit a patch.

.. _`fork`: http://help.github.com/fork-a-repo/
.. _`pull requests`: http://help.github.com/pull-requests/
