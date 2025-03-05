*********************************
시스템 사양
*********************************

.. contents:: Table of Contents

---------

목표 사양
==========

.. list-table:: 
   :header-rows: 1
   :widths: 20 50 30

   * - 항목
     - 사양
     - 비고
   * - Model Name
     - Lumino-Imager-Color
     - 
   * - Display
     - 7 inch LCD
     - 
   * - 화면구성
     - 컬러영상 / 흑백영상 / 컬러영상 + 흑백영상
     - 각 화면 볼 선택 가능
   * - NIR-LED 조도
     - 15 mW/cm², 강도 조절 ( 1 ~ 8 Step )
     - Over ( 복사 조도 )
   * - Wavelength
     - 740nm
     - ( 광원 )
   * - 포작 정확도
     - 0.5IOU
     - ( 개요 참조 )
   * - NIR Camera
     - Resolution : 1920 x 1080, Auto-Focus
     - 
   * - Recording Camera
     - Resolution : 1920 x 1080, Auto-Focus
     - 
   * - Image Processing Time
     - 25fps ( @ 1920 x 1080 )
     - 
   * - Image Storage
     - Image Capture ( 1920 x 1080 ), 동영상 Recording
     - SD Card
   * - Data Interface
     - USB C-Type
     - 내부 메모리 외장하드로 인식 ( Cyber Security 등급화 )
   * - Control Interface
     - Tact Switch ( 4EA )
     - 
   * - Battery
     - Continuous Operation Time: 1.5H, Charging Time: < 4H
     - 
   * - Power consumption
     - < 5W ( @ DC +5V )
     - 
   * - Conformity
     - IEC-60601-1,-2, 의료기기 적합성 시험 ( 전기적 위험, 전기/기계적 등의 안전적 요인 보증 )
     - 
   * - Weight
     -  900g
     - 
   * - Dimensions
     - 107 x 220 x 80
     -


구성 요소
=========

- Image Processing
    - Dual Image Sensor: :guilabel:`NIR ( Dual )`
        - **Resolution**: 1920x1080@30fps
        - **Output Mode**: RGB + NIR
        - **Output Format**: RGB Raw Bayer
    - Camera Module: :guilabel:`FPGA`
        - **Input Format**: RGB Raw Bayer
        - **Image Processing**: Image composition ( RGB + NIR mode )
        - **Output Format**: RGB, YUV ( 4:2:0, etc )
        - **Display Interface**: HDMI ( RGB )
        - **HS Communication Interface**: USB2.0 or USB3.0 ( YUV )

.. important::
    :guilabel:`Camera module` 은 UVC 규격를 준수해야 합니다.

.. warning::
    :guilabel:`Camera module` 이 UVC 규격을 준수하지 않을 경우, 카메라 모듈의 동작이 보장되지 않아 드라이버 수정이 필요할 수 있습니다.

.. note::
    기본 기능 외에 추가 기능을 구현할 경우, Cypress FX3 펌웨어 수정이 필요할 수 있습니다.

- Video Processing
    - Video Recorder: :guilabel:`System on Module`
        - **Board**: SoM ( Raspberry Pi 4 CM4 Lite ) + Self-designed I/O Board
    - Storage: SD Card
        - **Capacity**: 2GB ~ 2TB
        - **Video Speed Class**: V30 ( 30MB/s, 4K )
    - Recording
        - **Resolution**: 1280x720@25fps
        - **Video Codec**: MPEG-4
        - **File Format**: MP4
    - Snapshot
        - **Resolution**: 1280x720
        - **Compression Format**: JPEG

Image Sensor
--------------

+------------------+----------------------------------------+
| Image Sensor     | Description                            |
+==================+========================================+
| Manufacturer     | ``Sony IMX462``                        |
+------------------+----------------------------------------+
| Resolution       | ``1920x1080p@120fps``                  |
+------------------+----------------------------------------+
| Supported Format | - ``MIPI D-PHY: 2-lane``               |
|                  | - ``MIPI CSI-2: RAW10 / RAW12``        |
+------------------+----------------------------------------+

FPGA
------

+------------------+----------------------------------------+
| FPGA             | Description                            |
+==================+========================================+
| Manufacturer     | ``Xilinx Zynq-7000 XC7020-CLG400``     |
+------------------+----------------------------------------+
| Architecture     | ``Dual-core ARM Cortex-A9 + FPGA``     |
+------------------+----------------------------------------+
| Logic Cells      | ``85K``                                |
+------------------+----------------------------------------+
| Memory           | ``4.9Mb Block RAM``                    |
+------------------+----------------------------------------+
| I/O Pins         | ``400-pin CLG Package``                |
+------------------+----------------------------------------+
| Video Processing | ``1080p@30fps, RGB / YUV Format``      |
+------------------+----------------------------------------+

System On Module
------------------

+------------------+----------------------------------------------------------------------------+
| System On MOdule | Description                                                                |
+==================+============================================================================+
| SOM              | ``Raspberry Pi 4 CM4 Lite``                                                |
+------------------+----------------------------------------------------------------------------+
| Processor        | ``BCM2711 Quad-core Cortex-A72 64-bit``                                    |
+------------------+----------------------------------------------------------------------------+
| Memory           | ``Up to 8GB LPDDR4-2400 SDRAM``                                            |
+------------------+----------------------------------------------------------------------------+
| SD Card          | - ``Type: SD, SDHC, SDXC``                                                 |
|                  | - ``Capacity: 2GB ~ 2TB``                                                  |
|                  | - ``Speed Class ( Max Data Transfer Rate ): UHS-I ( SDR104, 104MB/s )``    |
|                  | - ``Video Speed Class ( Min Sustained Write Speed ): V30 ( 30MB/s, 4K )``  | 
+------------------+----------------------------------------------------------------------------+
| Video Codec      | - ``H.265 ( 4Kp60 decode )``                                               |
|                  | - ``H.264 ( 1080p60 decode, 1080p30 )``                                    |
+------------------+----------------------------------------------------------------------------+
| I/O              | ``USB 2.0 / 3.0``                                                          |
+------------------+----------------------------------------------------------------------------+

I/O Board
-----------

+------------------+----------------------------------------------------------------------------+
| I/O Board        | Description                                                                |
+==================+============================================================================+
| Manufacturer     | ``Self-designed``                                                          |
+------------------+----------------------------------------------------------------------------+
| JTAG for DBG     |                                                                            |
+------------------+----------------------------------------------------------------------------+
| UART for DBG     |                                                                            |
+------------------+----------------------------------------------------------------------------+
| SD Card          | ``Form factor: micro SD``                                                  |
+------------------+----------------------------------------------------------------------------+
| USB              | ``USB 2.0 x 1 ( Type-A )``                                                 |
+------------------+----------------------------------------------------------------------------+
| RESET            | ``1-pin``                                                                  |
+------------------+----------------------------------------------------------------------------+
| Power            | ``5V 8A``                                                                  |
+------------------+----------------------------------------------------------------------------+

---------


동작 환경
=========

Hardware
----------

Power
~~~~~~~

Temperature
~~~~~~~~~~~~~

Software
----------

Software Stack
~~~~~~~~~~~~~~~~