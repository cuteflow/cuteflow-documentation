Documentation Format
====================

The CuteFlow documentation uses `reStructuredText`_ as its markup language and
`Sphinx`_ for building the output (HTML, PDF, ...).

reStructuredText
----------------

reStructuredText "is an easy-to-read, what-you-see-is-what-you-get plaintext
markup syntax and parser system".

You can learn more about its syntax by reading existing CuteFlow `documents`_
or by reading the `reStructuredText Primer`_ on the Sphinx website.

If you are familiar with Markdown, be careful as things as sometimes very
similar but different:

* Lists starts at the beginning of a line (no indentation is allowed);

* Inline code blocks use double-ticks (````like this````).

Sphinx
------

Sphinx is a build system that adds some nice tools to create documentation
from reStructuredText documents. As such, it adds new directives and
interpreted text roles to standard reST `markup`_.

Syntax Highlighting
~~~~~~~~~~~~~~~~~~~

All code examples uses PHP as the default highlighted language. You can change
it with the ``code-block`` directive:

.. code-block:: rst

    .. code-block:: yaml

        { foo: bar, bar: { foo: bar, bar: baz } }

If your PHP code begins with ``<?php``, then you need to use ``html+php`` as
the highlighted pseudo-language:

.. code-block:: rst

    .. code-block:: html+php

        <?php echo $this->foobar(); ?>

.. note::

    A list of supported languages is available on the `Pygments website`_.

Testing Documentation
~~~~~~~~~~~~~~~~~~~~~

To test documentation before a commit:

 * Install `Sphinx`_;

 * Run ``make html`` and view the generated HTML in the ``build`` directory.

.. _reStructuredText:           http://docutils.sf.net/rst.html
.. _Sphinx:                     http://sphinx.pocoo.org/
.. _documents:                  http://github.com/cuteflow/cuteflow-documentation
.. _reStructuredText Primer:    http://sphinx.pocoo.org/rest.html
.. _markup:                     http://sphinx.pocoo.org/markup/
.. _Pygments website:           http://pygments.org/languages/
.. _Sphinx quick setup:         http://sphinx.pocoo.org/tutorial.html#setting-up-the-documentation-sources
