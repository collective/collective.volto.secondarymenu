
====================
Volto Secondary Menu
====================

Add-on for Volto to manage a secondary menu (right column) for `Dropdown Menu`_.

.. _Dropdown Menu: https://github.com/collective/volto-dropdownmenu

Features
--------

- Control panel for plone registry to manage secondary menu configuration.
- Restapi view that exposes these settings for Volto

Volto endpoint
--------------

Anonymous users can't access registry resources by default with plone.restapi (there is a special permission).

To avoid enabling registry access to everyone, this package exposes a dedicated restapi route with the infos to draw the menu: *@secondary-menu*::

    > curl -i http://localhost:8080/Plone/@secondary-menu -H 'Accept: application/json'


Control panel
-------------

You can edit settings directly from Volto because the control has been registered on Plone and available with plone.restapi.


Volto integration
-----------------

To use this product in Volto, your Volto project needs to include a new plugin: https://github.com/collective/volto-secondarymenu


Translations
------------

This product has been translated into

- Italian

- Spanish


Installation
------------

Install collective.volto.secondarymenu by adding it to your buildout::

    [buildout]

    ...

    eggs =
        collective.volto.secondarymenu


and then running ``bin/buildout``


Contribute
----------

- Issue Tracker: https://github.com/collective/collective.volto.secondarymenu/issues
- Source Code: https://github.com/collective/collective.volto.secondarymenu


License
-------

The project is licensed under the GPLv2.

Authors
-------

This product was developed by **RedTurtle Technology** team.

.. image:: https://avatars1.githubusercontent.com/u/1087171?s=100&v=4
   :alt: RedTurtle Technology Site
   :target: http://www.redturtle.it/
