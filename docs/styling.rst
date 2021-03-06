.. _hieroglyph-themes:

================
 Styling Slides
================

Styling
-------

- Slides are contained in ``<article>`` elements
- Each slide has an HTML ``id`` that corresponds to the permalink ID
  generated by Sphinx (for example, you're currentling reading
  ``styling``).
- The heading level is added as a class; ie, ``level-2``
- Slides may be styled using a theme, or custom CSS.

Included Themes
---------------

Hieroglyph includes two :ref:`themes <custom-themes>`.

``slides``

  Two slides levels: the first level of headers become "section"
  headers, and the second become the real content.

``single-level``

  Only one style of slide, every slide has a title at the top.


Setting the Theme
-----------------

You can set your theme using the ``slide_theme`` configuration
setting.

::

  slide_theme = 'single-level'

If you're using a custom theme, you can also set the directory to look
in for themes::

  slide_theme_path = '...'

.. _custom-css:

Custom CSS
----------

The standard Hieroglyph themes support adding a custom stylesheet with
the ``slide_theme_options`` dict in ``conf.py``::

  slide_theme_options = {'custom_css':'custom.css'}

The custom CSS file should be located in the ``html_static_path``
(``_static`` by default).
