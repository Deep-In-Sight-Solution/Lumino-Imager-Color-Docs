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
   :caption: Specification

   /spec_env/product
   /spec_env/system
   /spec_env/development
   /spec_env/support

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: 개발 환경

   /dev_env/impl
   /dev_env/test
   /dev_env/verify
   /dev_env/cicd
   /dev_env/quality
   /dev_env/repo

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: 관리 환경

   /mgmt_env/issues
   /mgmt_env/changes
   /mgmt_env/status
   /mgmt_env/risk

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: 운영 환경

   /op_env/deploy
   /op_env/release

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: Reference

   /ref_env/changelog
   /ref_env/icg


.. contents:: Table of Contents

----------

Welcome to ICG-Color Documentation
==================================

- 형광 영상 장비를 이용한 첨단 종양 수술에 사용되는 영상 장비를 개발중이며, 실시간 형광 이미징 기술을 활용하여 종양과 정상 조직을 명확하게 구분하고, 보다 정밀한 수술이 가능하도록 지원하는 것을 목표로 한다.
- ( 형광 영상 장비를 이용한 첨단 종양 수술 관련 자세한 정보는 여기에_ )

.. _여기에: https://deep-in-sight-lumino-imager-color-private.readthedocs.io/ko/latest/ref_env/icg.html

.. raw:: html

    <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe src="https://www.youtube.com/embed/FKaYvVP2f4o" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
    </div>

----------

.. tabs::
    
    .. tab:: White Light Mode
        
        .. figure:: static/icg-color-white-light-mode.png
            
            출처: https://www.mdpi.com/1648-9144/59/9/1530

    .. tab:: NIR/ICG Overay Mode
        
        .. figure:: static/icg-color-overlay.png

            출처: https://www.mdpi.com/1648-9144/59/9/1530

    .. tab:: NIR/ICG Intensity Map Mode
        
        .. figure:: static/icg-color-overlay-intensity-map.png

            출처: https://www.mdpi.com/1648-9144/59/9/1530

.. list-table:: 

    * - .. figure:: static/icg-color-white-light-mode.png
            :width: 100%
            :alt: NIR/ICG White Light Mode

      - .. figure:: static/icg-color-overlay.png
            :width: 100%
            :alt: NIR/ICG Overay Mode

      - .. figure:: static/icg-color-overlay-intensity-map.png
            :width: 100%
            :alt: NIR/ICG Intensity Map Mode

----------

지원 사양
---------

:doc:`USB <spec_env/usb>`
    USB 포트를 통해 데이터 전송 및 주변기기 연결이 가능합니다.
    USB 2.0/3.0을 지원하며, ...

:doc:`SD Card <spec_env/sdcard>`
    SD/SDHC/SDXC 카드를 지원하여 데이터 저장 및 백업이 가능합니다.
    최대 2TB까지의 저장 용량을 지원합니다. ...

:doc:`Network <spec_env/network>`
    유선 이더넷(RJ45) 및 무선 Wi-Fi 연결을 지원합니다.
    TCP/IP 프로토콜을 통한 네트워크 통신이 가능하며, 원격 접속 및 데이터 전송을 지원합니다. ...


동작 환경
---------

:doc:`시스템 구동 <exec_env/exec_hw_method>`
    시스템의 하드웨어 구성요소를 초기화하고 부팅하는 과정을 설명합니다.
    전원 공급, 카메라 모듈 초기화, 디스플레이 설정, 네트워크 연결 등 하드웨어 관련 구동 절차를 포함합니다.

:doc:`프로그램 실행 <exec_env/exec_sw_method>`
    ICG-Color 소프트웨어의 실행 방법과 작동 절차를 설명합니다.
    사용자 인터페이스 조작, 영상 촬영 및 처리, 데이터 저장, 시스템 종료 등 소프트웨어 운영에 관한 상세 절차를 포함합니다.


개발 환경
---------

:doc:`구현 <dev_env/impl>`
    시스템의 주요 기능과 모듈별 구현 방법을 설명합니다.
    프로그래밍 언어, 프레임워크, 라이브러리 등 개발 도구와 코드 구조, 주요 알고리즘, API 명세를 포함합니다.

:doc:`배포 <dev_env/deploy>`
    소프트웨어 빌드, 패키징 및 배포 프로세스를 설명합니다.
    컴파일 방법, 의존성 관리, 설치 패키지 생성,
    버전 관리 및 릴리스 절차를 포함합니다.

:doc:`테스트 <dev_env/test>`
    소프트웨어 품질 보증을 위한 테스트 방법론과 절차를 설명합니다.
    단위 테스트, 통합 테스트, 시스템 테스트, 성능 테스트 등
    각종 테스트 케이스와 자동화 도구 활용 방법을 포함합니다.

:doc:`검증 <dev_env/test>`
    개발된 시스템의 요구사항 충족 여부를 검증하는 방법을 설명합니다.
    기능 검증, 성능 검증, 안정성 검증 등
    품질 기준 충족 여부를 확인하는 절차를 포함합니다.

:doc:`형상 관리 <dev_env/repo>`
    소스 코드와 문서의 버전 관리 방법을 설명합니다.
    Git 저장소 구조, 브랜치 전략, 커밋 규칙,
    코드 리뷰 프로세스 등을 포함합니다.


실행 환경
---------

:doc:`소프트웨어 스택 <exec_env/sw_stack>`
    시스템 운영에 필요한 소프트웨어 계층 구조를 설명합니다.
    운영체제, 미들웨어, 응용 프로그램 등 각 계층별 구성요소와
    버전 정보, 의존성 관계를 포함합니다.
    또한 드라이버, 라이브러리, 프레임워크 등
    시스템 구동에 필요한 모든 소프트웨어 요소들의 구성을 설명합니다.

관리 환경
---------

:doc:`이슈 관리 <mgmt_env/issues>`
    시스템 개발 및 운영 과정에서 발생하는 문제점, 개선사항 등을 추적하고 관리하는 프로세스

:doc:`변경 관리 <mgmt_env/changes>`
    요구사항(사용자, 시스템, 품질 등)과 그에 따른 시스템의 하드웨어 및 소프트웨어 구성요소의 변경사항을 관리하는 프로세스

:doc:`현황 관리 <mgmt_env/status>`
    프로젝트에서 소프트웨어 개발 전체 진행 상황을 한눈에 파악할 수 있는 대시보드를 제공

:doc:`위험 관리 <mgmt_env/risk>`
    프로젝트 진행 중 발생할 수 있는 위험 요소 식별 및 대응 전략을 설명

운영 환경
---------

:doc:`배포 <op_env/deploy>`
    배포 단계에서는 애플리케이션의 설치, 구성, 업데이트 및 유지보수와 관련된 절차와 환경 구성이 상세히 설명됩니다.
    개발 완료된 시스템을 운영 환경에 적용하기 위한 배포 방법과 절차를 설명합니다.


Reference
-----------

:doc:`Changelog <ref_env/changelog>`
    각 버전별 변경사항과 업데이트 내용을 기록합니다.

:doc:`ICG <ref_env/icg>`
    형광 영상 장비와 관련된 추가 정보와 참고 자료를 제공합니다.
