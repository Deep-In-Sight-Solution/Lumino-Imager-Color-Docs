*********************************
VOMASYS-meerecompany User Manual
*********************************

.. contents:: Table of Contents

---------

개발 환경
========

`OS` : ``Windows 11``

`IDE` : ``Qt 5.15.2``

`Compiler` : ``MSVC2019 ( Visual Studio 2019 )``
    
:doc:`Changelog </dev_env/changelog>`
    개발 환경 변경 사항.

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: development
    
    /dev_env/development
    /dev_env/changelog


실행 환경
========

`OS` : `Windows 11``
    
:doc:`Changelog </exec_env/changelog>`
    실행 환경 변경 사항.

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: execution
   
   /exec_env/excution
   /exec_env/changelog


실행 방법
========

#. ToF camera 드라이버 설치
#. PC 에 연결 후 ( I/F: USB ) 장치 인식 상태 확인 :menuselection:`제어판 --> 장치 관리자`
#. `Git for Windows <https://git-scm.com/download/win>`__ 설치.

    - if ``64-bit OS`` : Download :guilabel:`64-bit Git for Windows Setup`.
    - if ``32-bit OS`` : Download :guilabel:`32-bit Git for Windows Setup`.

#. 실행 파일 다운로드

   .. code-block:: window

    PS c:\work> git clone ssh://meerecompany@220.78.49.161:2222/repo/meerecompany/vomasys-release

#. :guilabel:`파일 탐색기` 실행 후 작업 디렉토리 ``c:\work\vomasys-release\build-src-Desktop_Qt_5_15_2_MSVC2019_64bit-Release`` 에 있는 ``BoxDimensionDetectionPrototype.exe`` 를 실행한다. 


검증 환경
========

.. list-table:: 

    * - .. figure:: static/1.jpeg

      - .. figure:: static/2.jpeg

      - .. figure:: static/3.jpeg


운영 환경
========

:doc:`DeepInsight Issue Management System </op_env/operation>`
    딥인사이트 이슈 관리 시스템 (협력 업체 대응 이슈)
    
:doc:`Changelog </op_env/changelog>`
    운영 환경 변경 사항.

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: operation
   
   /op_env/operation
   /op_env/changelog
