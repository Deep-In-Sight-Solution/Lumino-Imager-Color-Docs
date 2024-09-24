DeepInsight VOMASYS Documentation
=================================

...

개발 환경
#####################

:doc:`OS`
    Windows 11
    
:doc:`IDE`
    Qt 5.15.2
    
:doc:`Compiler`
    MSVC2019 ( Visual Studio 2019 )
    
:doc:`Changelog </dev_env/changelog>`
    Development environment changelog.
    

실행 환경
#####################

:doc:`OS`
    Windows 11

:doc:`Install </exec_env/excution>`
    How to configure kernel.
    
:doc:`development </linux/kernel/development>`
    Guidelines and release planning and check dependencies.
    
:doc:`Changelog </exec_env/changelog>`
    Execution environment changelog.

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Kernel
   
   /linux/kernel/configure
   /linux/kernel/compile
   /linux/kernel/development
   /linux/kernel/changelog

운영 환경
#####################

:doc:`create </linux/rootfs/index>`
    How to create a rootfs image
    
:doc:`development </linux/rootfs/development>`
    Guidelines and release planning and check dependencies.
    
:doc:`changelog </linux/rootfs/changelog>`
    The rootfs development changelog.

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: RootFS
   
   /linux/rootfs/image
   /linux/rootfs/development
   /linux/rootfs/changelog
