**************************
Revitron Sphinx Theme
**************************

This Sphinx_ theme is a fork of the original `Read the Docs`_ theme
that was designed to provide a great reader experience for
documentation users on both desktop and mobile devices. You can find
a working demo of the theme in the `Revitron documentation`_

.. _Sphinx: http://www.sphinx-doc.org
.. _Read the Docs: https://github.com/readthedocs/sphinx_rtd_theme
.. _Revitron documentation: https://revitron.readthedocs.io/en/latest/

Installation
============

This theme can be installed with ``pip``:

.. code:: console

   $ pip install https://github.com/revitron/revitron-sphinx-theme/tarball/master

To use the theme in your Sphinx project, you will need to add the following to
your ``conf.py`` file:

.. code:: python

    import revitron_sphinx_theme

    extensions = [
        ...
        "revitron_sphinx_theme",
    ]

    html_theme = "revitron_sphinx_theme"

Configuration
=============

This theme is highly customizable on both the page level and on a global level.
To see all the possible configuration options, read the documentation for the original theme on
`configuring the theme`_.

.. _configuring the theme: https://sphinx-rtd-theme.readthedocs.io/en/latest/configuring.html

Contributing
============

If you would like to help modify or translate the theme, you'll find more
information on contributing in `contributing guide`_ of the original theme.

.. _contributing guide: https://sphinx-rtd-theme.readthedocs.io/en/latest/contributing.html
