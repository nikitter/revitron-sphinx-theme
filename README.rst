**************************
Revitron Sphinx Theme
**************************

This Sphinx_ theme is a fork of the original `Read the Docs`_ theme
that was designed to provide a great reader experience for
documentation users on both desktop and mobile devices. You can find
a working demo of the theme in the `Revitron documentation`_.

.. _Sphinx: http://www.sphinx-doc.org
.. _Read the Docs: https://github.com/readthedocs/sphinx_rtd_theme
.. _Revitron documentation: https://revitron.readthedocs.io/en/latest/

.. image:: https://raw.githubusercontent.com/marcantondahmen/media-files/master/themes/revitron/default.png

Installation
============

This theme can be installed with ``pip``:

.. code:: console

   $ pip install https://github.com/revitron/revitron-sphinx-theme/archive/master.zip

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

.. code:: python

    html_theme_options = {
        'canonical_url': '',
        'analytics_id': 'UA-XXXXXXX-1', 
        'style_external_links': False,
        'collapse_navigation': True,
        'sticky_navigation': True,
        'navigation_depth': 4,
        'includehidden': True,
        'titles_only': False,
        'github_url': '',
		'logo_mobile': 'demo/static/logo-mobile.svg
    }

    html_logo = 'demo/static/logo.svg'

Adding a Landing Page
=====================

It is possible to render the ``master_doc`` page with a landing page template. 
That template provides some special classes to style content and add buttons. 
It can be enabled and configured in the ``conf.py`` as follows.

.. code:: python

    html_context = {
        'landing_page': {
            'menu': [
                {'title': 'Get Started', 'url': 'installing.html'},
                {'title': 'GitHub', 'url': 'https://github.com/user/repo'}
            ]
        } 
    }

.. image:: https://raw.githubusercontent.com/marcantondahmen/media-files/master/themes/revitron/landing.png

Container Classes
=================

This theme provides three ``container`` classes to style paragraphs, wrap images and create buttons directly in a ``.rst`` file.

.. code:: 

    .. container:: .large
	
       A large text block ...

    .. container:: .buttons

       `Docs <installing.html>`_
       `GitHub <installing.html>`_

    .. container:: .image

       .. image:: image.png

.. image:: https://raw.githubusercontent.com/marcantondahmen/media-files/master/themes/revitron/mobile.png

Contributing
============

If you would like to help modify or translate the theme, you'll find more
information on contributing in the `contributing guide`_ of the original theme.

.. _contributing guide: https://sphinx-rtd-theme.readthedocs.io/en/latest/contributing.html
