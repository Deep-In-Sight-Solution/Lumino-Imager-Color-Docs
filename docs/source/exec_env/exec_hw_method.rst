*********************************
시스템 구동
*********************************

.. contents:: Table of Contents

---------

실행 환경
=========

+------------+----------+-------------------------+
| SW         | Description                        |
+============+==========+=========================+
| OS         | ``Windows 11``                     |
+------------+----------+-------------------------+
| Framework  | T.B.D                              |
+------------+----------+-------------------------+
| Stack      | T.B.D                              |
+------------+----------+-------------------------+


실행 절차
=========

#. ToF camera 드라이버 설치
#. PC 에 연결 후 ( I/F: USB ) 장치 인식 상태 확인 :menuselection:`제어판 --> 장치 관리자`
#. `Git for Windows <https://git-scm.com/download/win>`__ 설치.

    - if ``64-bit OS`` : Download :guilabel:`64-bit Git for Windows Setup`.
    - if ``32-bit OS`` : Download :guilabel:`32-bit Git for Windows Setup`.

#. 실행 파일 다운로드

   .. code-block:: window

    PS c:\work> git clone ssh://meerecompany@220.78.49.161:2222/repo/meerecompany/vomasys-release

#. :guilabel:`파일 탐색기` 실행 후 작업 디렉토리 ``c:\work\vomasys-release\build-src-Desktop_Qt_5_15_2_MSVC2019_64bit-Release`` 에 있는 ``BoxDimensionDetectionPrototype.exe`` 를 실행한다. 


실행화면
========

.. tabs::

    .. tab:: 실행 화면
        
        .. figure:: ../static/app.jpeg

            택배물 안착 및 부피 측정 요청

    .. tab:: 측정
        
        .. figure:: ../static/capture.jpeg

            택배물 가로 세로 길이 계측 및 면적 산정, 높이 계측

    .. tab:: 결과
        
        .. figure:: ../static/result.jpeg

            택배물 부피 산정

    .. tab:: 실행 흐름
        
        .. figure:: ../static/flow.png


측정방법
========

.. important::

    :menuselection:`Calibration --> Range Setting --> Capture (부피 측정)` 순서로 진행하세요.

    .. list-table:: 

        * - .. figure:: ../static/capture_button.png

            Capture
    
          - .. figure:: ../static/cal_button.png

            Calibration
    
          - .. figure:: ../static/range_button.png

            Range Setting

.. warning::

    ROI 영역 지정 시 반드시 :menuselection:`좌상단 --> 우하단` 방향으로 좌표를 지정해야 하며, 이 지침을 지키지 않을 시 제대로 동작하지 않을 수 있습니다.

.. tabs::

    .. tab:: Calibration

        1. Depth Image에서 ROI로 지정할 :menuselection:`좌상단 --> 우하단` 좌표를 선택하여 사각형 ROI 지정한다.
        2. 지정 후 지정된 영역을 제외한 다른 영역을 선택하여 셋팅을 완료한다.

        .. figure:: ../static/4.jpeg

        .. figure:: ../static/5.jpeg


    .. tab:: Range Setting

        1. Calibration과 동일한 방법으로 박스를 올려 둘 영역을 지정한다.
        2. 지정 후 지정된 영역을 제외한 다른 영역을 선택하여 셋팅을 완료한다.

        .. figure:: ../static/6.jpeg
