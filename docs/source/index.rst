Welcome to DTK4412 Documentation
================================

DTK4412 is Android / Linux Training Kit based on Exynos4412_.
DTK4412 Training Kit is a full featured Android development platform that provides an ideal starting point for creating high-performance embedded devices. Based upon Samsung Exynos4412_ quad core processor, the DTK4412 includes all of the software tools and accessories required to immediately begin development work.

.. _Exynos4412: https://en.wikipedia.org/wiki/Exynos

Bootloader ( U-boot )
---------------------

:doc:`configure </linux/bootloader/u-boot/configure>`
    How to configure bootloader

:doc:`compile </linux/bootloader/u-boot/compile>`
    How to build bootloader

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Bootloader

   /linux/bootloader/u-boot/configure
   /linux/bootloader/u-boot/compile
   /linux/bootloader/u-boot/devlopment
   /linux/bootloader/u-boot/changelog

Kernel ( Linux )
----------------

:doc:`configure </linux/kernel/configure>`
    How to configure kernel

:doc:`compile </linux/kernel/compile>`
    How to configure kernel

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Kernel
   
   /linux/kernel/configure
   /linux/kernel/compile
   /linux/kernel/development
   /linux/kernel/changelog

RootFS
----------------

:doc:`create </linux/rootfs/index>`
    How to create a rootfs image

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: RootFS
   
   /linux/rootfs/image
   /linux/rootfs/development
   /linux/rootfs/changelog
   
Buildroot
----------------

:doc:`build </platform/build/buildroot/index>`
    How to build DTK4412 linux-based development system

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Buildroot
   
   /platform/build/buildroot/configure
   /platform/build/buildroot/build
   /platform/build/buildroot/development
   /platform/build/buildroot/changelog
   
Yocto
----------------

:doc:`build </platform/build/yocto/index>`
    How to build DTK4412 linux-based development system

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Yocto
   
   /platform/build/yocto/configure
   /platform/build/yocto/build
   /platform/build/yocto/development
   /platform/build/yocto/changelog
   
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
    
:ref:`supported-dependencies`
    Supported project dependencies, like Python and Sphinx.

.. _Read the Docs contributor guide: https://docs.readthedocs.io/en/stable/contribute.html
