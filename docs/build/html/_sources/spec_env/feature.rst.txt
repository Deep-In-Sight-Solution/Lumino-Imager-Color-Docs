*********************************
기능 명세서
*********************************

.. |date| date:: %Y-%m-%d
.. contents:: Table of Contents

---------

기능 정의
=========

Recording
-----------
- Resolution: 1280x720
- Video Codec: MPEG-4
    - Part: MPEG-4 Part 10 ( H.264 )
    - Profile: BP, MP, HP etc.
    - Level: 4.x
    - Bitrate: 5 ~ 10Mbps
    - Frame Rate: 30 ~ 60fps

Snapshot
----------
- Resolution: 1280x720
- Compression Format: JPEG
    - Quality: 100

Storage
---------
- SD Card
    - Capacity: 2GB ~ 2TB
    - Video Speed Class: V30 ( 30MB/s, 4K )
    - 저장 데이터
        - 이미지 파일 ( JPEG, 1280x720 )
        - 영상 파일 ( MPEG-4, 1280x720 )
    - 데이터 암호화

File Transfer
---------------
- USB
    - USB OTG ( On-The-Go ) 지원
    - PC와 데이터 전송 가능
    - 전송 방식
        - 단말기가 USB Mass Storage로 인식
        - SD 카드가 이동식 디스크로 마운트
    - 전송 가능 데이터
        - 저장된 이미지 파일 ( JPEG, 1280x720 )
        - 녹화된 영상 파일 ( H.264, 1280x720 )
    - 전송 속도
        - USB C-Type 인터페이스 사용
        - USB 3.0 지원 ( 최대 5Gbps )
    - 사용 방법
        1. USB C-Type 케이블로 PC와 단말기 연결
        2. 단말기가 자동으로 Mass Storage 모드로 전환
        3. PC에서 이동식 디스크로 인식되어 파일 접근 가능
        4. 드래그 앤 드롭으로 파일 전송

Data Encryption Tool
-----------------------
- 오픈 소스 암호화 소프트웨어 및 모바일 앱 제공
    - USB Mass Storage 암호화 지원
    - 지원 OS
        - Windows ( X64 & ARM64 )
        - MacOS ( Monterey 12 and later )
        - Linux
        - Android ( EDS NG )
        - iOS ( Disk Decipher, Crypto Disks )
    - 주요 기능
        - 실시간 암/복호화
        - 볼륨 생성 및 마운트
        - 숨겨진 볼륨 지원
        - 다중 인증 지원