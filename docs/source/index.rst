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

`OS` : ``Windows 11``

실행 방법
--------

#. ToF camera 드라이버 설치
#. PC 에 연결 후 ( I/F: USB ) 장치 인식 상태 확인 :menuselection:`제어판 --> 장치 관리자`
#. `Git for Windows <https://git-scm.com/download/win>`__ 설치.

    - if ``64-bit OS`` : Download :guilabel:`64-bit Git for Windows Setup`.
    - if ``32-bit OS`` : Download :guilabel:`32-bit Git for Windows Setup`.

#. 실행 파일 다운로드

   .. code-block:: window

    PS c:\work> git clone ssh://meerecompany@220.78.49.161:2222/repo/meerecompany/vomasys-release

#. :guilabel:`파일 탐색기` 실행 후 작업 디렉토리 ``c:\work\vomasys-release\build-src-Desktop_Qt_5_15_2_MSVC2019_64bit-Release`` 에 있는 ``BoxDimensionDetectionPrototype.exe`` 를 실행한다. 

측정 방법
--------

.. tabs::

    :menuselection:`Calibration --> Range Setting --> 측정` 순서로 진행하세요.

    .. tab:: Calibration

        1 ~ 2. Depth Image에서 ROI로 지정할 :menuselection:`좌상단 --> 우하단` 좌표를 선택하여 사각형 ROI 지정한다.
        3. 지정 후 지정된 영역을 제외한 다른 영역을 선택하여 셋팅을 완료한다.

        .. figure:: static/4.jpeg

        .. figure:: static/5.jpeg


    .. tab:: Range Setting

        박스를 올려 둘 공간을 지정하는 작업
        1) Calibration과 동일한 방법으로 영역을 지정한다.
        2) 지정 후 지정된 영역을 제외한 다른 영역을 선택하여 셋팅을 완료한다.

        .. figure:: static/6.jpeg


:doc:`Changelog </exec_env/changelog>`
    실행 환경 변경 사항.

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: execution
   
   /exec_env/excution
   /exec_env/changelog


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
