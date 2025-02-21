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
   /spec_env/srs
   /spec_env/feature
   /spec_env/tech
   /spec_env/design
   /spec_env/manual

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

제품 구성
---------

.. raw:: html

   <p style="color: #0066cc;">제품의 물리적/소프트웨어적 구성 요소를 나열해서 전체 시스템의 구조를 설명합니다.</p>

:doc:`하드웨어 <spec_env/product>`
    제품의 하드웨어 구성요소와 사양을 설명합니다. 
    카메라, 광학계, 조명 등 사용자가 실제로 조작하고 
    다루게 될 물리적 장비들의 특징과 사용법을 포함합니다.

:doc:`소프트웨어 <spec_env/product>`
    사용자 인터페이스, 영상 처리 기능, 데이터 저장 및 관리 등 
    시스템을 실제로 사용하는데 필요한 소프트웨어 기능과 
    조작 방법을 설명합니다.

시스템 사양
-----------

.. raw:: html

   <p style="color: #0066cc;">시스템 전체의 성능, 용량, 환경 조건 등 기술적 요구사항에 따라 시스템이 동작해야 하는 기준을 정의합니다.</p>

:doc:`구성 요소 <spec_env/system>`
    시스템을 구성하는 주요 하드웨어 및 소프트웨어 컴포넌트들의 구조와 상호작용을 설명합니다.
    각 컴포넌트의 역할, 인터페이스, 의존성 관계를 포함하며,
    개발자가 시스템 아키텍처를 이해하고 유지보수하는데 필요한 상세 정보를 제공합니다.

:doc:`성능 목표 <spec_env/system>`
    시스템의 성능 목표와 측정 방법을 설명합니다.
    예를 들어, 영상 처리 속도, 데이터 전송 속도, 사용자 인터페이스 반응 시간 등을 포함합니다.

:doc:`구동 환경 <spec_env/system>`
    시스템의 하드웨어 구성요소를 초기화하고 부팅하는 과정을 설명합니다.

:doc:`동작 환경 <spec_env/system>`
    시스템이 실행되는 환경의 하드웨어 / 소프트웨어 요구사항과 설정을 설명합니다.
    운영체제 등의 최소 / 권장 사양과 필수 라이브러리, 드라이버, 런타임 환경 등을 포함합니다.
    또한 보안 설정 등 시스템 운영에 필요한 환경 설정 방법을 상세히 기술합니다.

요구 사항 명세서
---------------

.. raw:: html

   <p style="color: #0066cc;">사용자와 시스템이 충족해야 하는 기능적 / 비기능적 요구사항에 따른 개발 목표와 기준을 제시합니다.</p>

:doc:`요구 사항 <spec_env/srs>`
    시스템 개발에 필요한 기능적 / 비기능적 요구사항을 정의합니다.
    사용자 요구사항, 시스템 요구사항, 성능 요구사항 등을
    명확하게 문서화하여 개발 범위와 목표를 설정합니다.
    또한 보안, 신뢰성, 확장성 등 품질 요구사항과
    법적/규제 요구사항도 포함하여 준수해야 할 기준을 제시합니다.

:doc:`개발 범위 <spec_env/srs>`
    시스템 개발의 범위와 제약사항을 정의합니다.
    구현해야 할 핵심 기능과 선택적 기능을 구분하고,
    개발 일정, 리소스, 기술적 제약 등을 고려하여
    현실적인 개발 범위를 설정합니다.
    또한 개발 단계별 마일스톤과 산출물을 정의하여
    프로젝트 진행 상황을 효과적으로 관리할 수 있도록 합니다.

기능 명세서
-----------

.. raw:: html

   <p style="color: #0066cc;">소프트웨어가 제공해야 하는 구체적인 기능 설명하며 요구사항을 기능 단위로 세분화합니다.</p>

:doc:`기능 정의 <spec_env/feature>`
    시스템의 주요 기능들을 상세히 정의하고 문서화합니다.
    각 기능의 입출력 인터페이스, 처리 로직, 예외 처리 등
    개발에 필요한 상세 스펙을 제공합니다.
    또한 기능간 의존성과 호출 관계를 명확히 하여
    모듈화된 개발이 가능하도록 합니다.
    API 문서화를 통해 각 기능의 사용법과 제약사항을
    명확하게 전달하여 개발 생산성을 높입니다.

기술 명세서
-----------

.. raw:: html

   <p style="color: #0066cc;">시스템 구현을 위한 기술적 세부사항과 설계 지침을 제공합니다.</p>  

:doc:`소프트웨어 스택 <spec_env/tech>`
    시스템 운영에 필요한 소프트웨어 계층 구조를 설명합니다.
    운영체제, 미들웨어, 응용 프로그램 등 각 계층별 구성요소와
    버전 정보, 의존성 관계를 포함합니다.
    또한 드라이버, 라이브러리, 프레임워크 등
    시스템 구동에 필요한 모든 소프트웨어 요소들의 구성을 설명합니다.

:doc:`소프트웨어 아키텍처 <spec_env/tech>`
    시스템의 전체적인 소프트웨어 구조와 설계 원칙을 설명합니다.
    계층화된 아키텍처 구조, 주요 컴포넌트와 모듈의 구성,
    데이터 흐름과 제어 흐름을 상세히 기술합니다.
    또한 확장성, 유지보수성, 재사용성을 고려한
    디자인 패턴과 아키텍처 패턴의 적용 방안을 포함합니다.
    시스템의 주요 인터페이스 정의와 통신 프로토콜,
    외부 시스템과의 연동 방식도 명확히 문서화합니다.

설계 사양
---------

.. raw:: html

   <p style="color: #0066cc;">소프트웨어 아키텍처, 모듈 간 인터페이스, 데이터 흐름 등 설계 세부사항과 시스템 설계의 청사진을 보여줍니다.</p>  

:doc:`설계 <spec_env/design>`
    시스템의 설계 내용을 설명합니다.
    클래스 다이어그램, 시퀀스 다이어그램 등 UML을 활용하여
    객체 구조와 상호작용을 명확히 표현합니다.
    실제 구현의 기초가 되는 상세 설계 정보를 제공합니다.
    또한 성능, 보안, 확장성을 고려한 설계 의사결정 내용도
    함께 문서화하여 개발 과정에서 참고할 수 있도록 합니다.

:doc:`구현 <spec_env/design>`
    시스템의 주요 기능과 모듈별 구현 방법을 설명합니다.
    프로그래밍 언어, 프레임워크, 라이브러리 등 개발 도구와 코드 구조, 주요 알고리즘, API 명세를 포함합니다.

:doc:`실행 환경 <spec_env/design>`
    시스템 실행에 필요한 하드웨어 및 소프트웨어 환경을 설명합니다.
    서버 사양, 운영체제, 미들웨어, 데이터베이스 등
    필수 구성요소의 설치 및 설정 방법을 포함합니다.
    또한 시스템 모니터링, 로깅, 백업/복구 등
    운영 관리를 위한 도구와 절차도 문서화합니다.
    개발자가 로컬 환경에서 시스템을 구동하고 테스트할 수 있도록
    개발 환경 구성 가이드도 제공합니다.

개발 환경
---------

.. raw:: html

   <p style="color: #0066cc;">소프트웨어를 개발하고 테스트하는 데 필요한 도구, 플랫폼, 설정을 정의. 개발 프로세스의 기반을 설명합니다.</p>  

:doc:`시험 <dev_env/test>`
    소프트웨어 품질 보증을 위한 테스트 방법론과 절차를 설명합니다.
    단위 테스트, 통합 테스트, 시스템 테스트, 성능 테스트 등 각종 테스트 케이스와 자동화 도구 활용 방법을 포함합니다.

:doc:`검증 <dev_env/verify>`
    개발된 시스템의 요구사항 충족 여부를 검증하는 방법을 설명합니다.
    기능 검증, 성능 검증, 안정성 검증 등 품질 기준 충족 여부를 확인하는 절차를 포함합니다.

:doc:`CI/CD <dev_env/cicd>`
    소프트웨어 빌드, 패키징 및 배포 프로세스를 설명합니다.

:doc:`코드 품질 <dev_env/quality>`
    소프트웨어의 코드 품질을 보장하기 위한 도구와 프로세스를 설명합니다.
    정적 코드 분석, 코드 스타일 검사, 코드 복잡도 측정, 코드 중복 검사 등 품질 지표 측정 방법과 기준을 포함합니다.

:doc:`형상 관리 <dev_env/repo>`
    소스 코드 버전 관리 방법을 설명합니다.
    Git 저장소 구조, 브랜치 전략, 커밋 규칙, 코드 리뷰 프로세스 등을 포함합니다.

관리 환경
---------

.. raw:: html

   <p style="color: #0066cc;">소프트웨어 개발, 배포, 유지보수를 관리하는 데 필요한 환경과 프로세스를 정의합니다.</p>

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

.. raw:: html

   <p style="color: #0066cc;">소프트웨어가 실제 배포되고 운영되는 환경을 정의합니다.</p>

:doc:`배포 <op_env/deploy>`
    소프트웨어 개발 과정에서 생성된 코드와 리소스를 실제 운영 환경에 적용하는 과정입니다.
    개발 완료된 시스템을 운영 환경에 적용하기 위한 배포 방법과 절차를 보여줍니다.
    주요 기능으로는 기록 조회, 상태 모니터링, 세부 정보 확인 등 배포 이력을 관리하고 추적합니다.
    배포 내역을 실시간으로 추적하고 분석할 수 있어, 개발팀과 운영팀이 배포 주기, 성능, 문제 발생 원인 등을 파악하고 개선할 수 있도록 지원합니다.

:doc:`프로젝트 버전 관리 <op_env/release>`
    프로젝트 버전 관련 정보를 종합적으로 관리하고 추적합니다.
    주요 기능으로는 목록 조회, 계획 및 관리, 진행 사항 추적 및 보고, 이슈 연계 관리를 포함합니다.
    프로젝트 버전을 체계적으로 관리하고, 특정 버전에 포함된 작업을 명확히 파악하도록 돕습니다.

Reference
-----------

:doc:`Changelog <ref_env/changelog>`
    각 버전별 변경사항과 업데이트 내용을 기록합니다.

:doc:`ICG <ref_env/icg>`
    형광 영상 장비와 관련된 추가 정보와 참고 자료를 제공합니다.
