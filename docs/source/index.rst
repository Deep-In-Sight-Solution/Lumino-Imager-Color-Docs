Welcome to DTK4412 Documentation
================================

DTK4412 is Android / Linux Training Kit based on Exynos4412_.
DTK4412 Training Kit is a full featured Android development platform that provides an ideal starting point for creating high-performance embedded devices. Based upon Samsung Exynos4412_ quad core processor, the DTK4412 includes all of the software tools and accessories required to immediately begin development work.

.. _Exynos4412: https://en.wikipedia.org/wiki/Exynos

Bootloader ( U-boot )
---------------------

:doc:`configure </linux/bootloader/u-boot/configure>`
    How to configure bootloader

:doc:`build </linux/bootloader/u-boot/build>`
    How to build bootloader

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Bootloader

   /linux/bootloader/u-boot/index

Kernel ( Linux )
----------------

:doc:`configure </linux/kernel/configure>`
    How to configure kernel

:doc:`build </linux/kernel/build>`
    How to configure kernel.

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Kernel
   
   /linux/kernel/index

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
