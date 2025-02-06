**************************************
Lumino Imager Color User Manual
**************************************

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: 개요

   /intro_env/about

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: 사양

   /spec_env/usb
   /spec_env/sdcard
   /spec_env/network

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: 개발환경

   /dev_env/impl
   /dev_env/deploy
   /dev_env/test
   /dev_env/repo

.. toctree::    
   :maxdepth: 2
   :hidden:
   :caption: 실행환경

   /exec_env/exec_method
   /exec_env/exec_screen

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: 검증환경

   /verif_env/verify

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: 관리환경

   /mgmt_env/changes
   /mgmt_env/status

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: 운영환경

   /op_env/deploy
   /op_env/release

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Reference

   /ref_env/changelog


.. contents:: Table of Contents

Welcome to ICG-Color Documentation
==================================

- Indocyanine Green (ICG) and Colorectal Surgery_: A Literature Review on Qualitative and Quantitative Methods of Usage.
- Indocyanine Green Fluorescence in Gastrointestinal Surgery_: Appraisal of current evidence

.. _Indocyanine Green (ICG) and Colorectal Surgery: https://www.mdpi.com/1648-9144/59/9/1530
.. _Indocyanine Green Fluorescence in Gastrointestinal Surgery: https://www.wjgnet.com/1948-9366/full/v15/i12/2693.htm

.. image:: static/icg-color.jpeg
    :width: 100%


Specification
---------------------

:doc:`USB </spec_env/usb>`
    ... .

:doc:`SD Card </spec_env/sdcard>`
    ... .

:doc:`Network </spec_env/network>`
    ... .


개발환경
---------------------

:doc:`구현 </dev_env/impl>`
    ... .

:doc:`배포 </dev_env/deploy>`
    ... .

:doc:`테스트 </dev_env/test>`
    ... .

:doc:`형상관리 </dev_env/repo>`
    ... .


실행환경
---------------------

:doc:`실행방법 </exec_env/exec_method>`
    ... .


검증환경
---------------------

:doc:`검증방법 </verif_env/verify>`
    ... .


관리환경
---------------------

:doc:`변경관리 </mgmt_env/changes>`
    ... .

:doc:`현황관리 </mgmt_env/status>`
    ... .


운영환경
---------------------

:doc:`배포 </op_env/deploy>`
    ... .

:doc:`출시 </op_env/release>`
    ... .


.. contents:: Table of Contents


검증 환경
========

- 부피 측정 장비 1set
- 박스 3ea ( small, medium, big )

.. important::

    플레이트와 거리 측정 센서와의 거리는 현재 0.710mm (71Cm)이며 해당 높이에 대한 offset 값이 적용되어 있다.

.. list-table:: 

    * - .. figure:: static/1.jpeg

      - .. figure:: static/2.jpeg

      - .. figure:: static/3.jpeg


운영 환경
========

`DeepInsight Issue Management System <http://220.78.49.161:8084/>`__
    딥인사이트 이슈 관리 시스템 (협력 업체 대응 이슈)
    
:doc:`Changelog </op_env/changelog>`
    운영 환경 변경 사항.
