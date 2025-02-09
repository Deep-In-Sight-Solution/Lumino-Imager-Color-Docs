*********************************
시스템 사양
*********************************

.. contents:: Table of Contents

---------

구성 요소
========

- Image Processing
    - Dual Image Sensor: NIR ( Dual )
        - Resolution: 1920x1080@30fps
        - Output Mode: RGB + NIR
        - Output Format: RGB Raw Bayer
    - Camera Module Board: FPGA
        - Role: UVC Webcam
        - Input Format: RGB Raw Bayer
        - Image Processing: Image composition ( RGB + NIR mode )
        - Output Format: RGB, YUV
        - Display Interface: HDMI ( RGB )
        - HS Communication Interface: USB2.0 or USB3.0 ( YUV )
    - Video Recorder: SOM ( System on Module )
        - Board: Raspberry Pi 4 CM4 Lite Series + Self-designed I/O Board
        
- Video Processing
    - Board: Raspberry Pi 4 CM4 Lite + I/O Board
        - Storage: SD Card
            - Capacity: 2GB ~ 2TB
            - Video Speed Class: V30 ( 30MB/s, 4K )
        - Recording
            - Resolution: 1280x720@25fps
            - Video Codec: MPEG-4
            - File Format: MP4
        - Snapshot
            - Resolution: 1280x720
            - Compression Format: JPEG

Image Sensor
-------------

+------------------+----------------------------------------+
| Image Sensor     | Description                            |
+==================+========================================+
| Manufacturer     | ``Sony IMX462``                        |
+------------------+----------------------------------------+
| Resolution       | ``1920x1080p@120fps``                  |
+------------------+----------------------------------------+
| Supported Format | - ``MIPI D-PHY: 2-lane ``              |
|                  | - ``MIPI CSI-2: RAW10 / RAW12 ``       |
+------------------+----------------------------------------+

FPGA
-----

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

Raspberry Pi 4 CM4 Lite + I/O Board
------------------------------------

+------------------+----------------------------------------------------------------------------+
| CM4 Lite         | Description                                                                |
+==================+============================================================================+
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


동작 환경
========

하위 항목
---------