Welcome to DTK4412 Documentation
================================

DTK4412 is Android / Linux Training Kit based on Exynos4412_.
DTK4412 Training Kit is a full featured Android development platform that provides an ideal starting point for creating high-performance embedded devices. Based upon Samsung Exynos4412_ quad core processor, the DTK4412 includes all of the software tools and accessories required to immediately begin development work.

.. _Exynos4412: https://en.wikipedia.org/wiki/Exynos

Bootloader ( U-boot )
----------------

:doc:`environment`
    How to setup bootloader source build environment

:doc:`configuring`
    How to configure bootloader

:doc:`building`
    HOw to build bootloader

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Bootloader

   /bootloader/environment
   /bootloader/configuring
   /bootloader/building

Kernel ( Linux )
----------------

:doc:`environment`
    How to setup bootloader source build environment

:doc:`configuring`
    How to configure kernel

:doc:`building`
    How to configure kernel.

Development
-----------

:doc:`contributing`
    How to contribute changes to the theme.

:doc:`Development guidelines <development>`
    Guidelines the theme developers use for developing and testing changes.

`Read the Docs contributor guide`_
    Our contribution guidelines extend to all projects maintained by Read the
    Docs core team.

:doc:`changelog`
    The theme development changelog.

:doc:`Demo documentation <demo/structure>`
    The theme's styleguide test environment, where new changes are tested.

:ref:`supported-browsers`
    Supported browser/operating system combinations.

:ref:`supported-dependencies`
    Supported project dependencies, like Python and Sphinx.

.. _Read the Docs contributor guide: https://docs.readthedocs.io/en/stable/contribute.html

.. Hidden TOCs

.. toctree::
   :maxdepth: 1
   :hidden:

   changelog

.. toctree::
    :maxdepth: 2
    :numbered:
    :caption: Demo Documentation
    :hidden:

    demo/structure
    demo/demo
    demo/lists_tables
    demo/api

.. toctree::
    :maxdepth: 3
    :numbered:
    :caption: This is an incredibly long caption for a long menu
    :hidden:

    demo/long
