*********************************
시스템 사양
*********************************

.. contents:: Table of Contents

---------

구성 요소
========

- Imaging & Processing
    - Dual Image Sensor: NIR ( Dual )
        - Output Mode: RGB + NIR
        - Output Format: RGB Raw Bayer
    - Board: FPGA
        - Role: UVC Webcam
        - Input Format: RGB Raw Bayer
        - Image Processing: Image composition ( RGB + NIR mode )
        - Output Format: RGB, YUV
        - Display Interface: HDMI ( RGB )
        - HS Communication Interface: USB2.0 or USB3.0 ( YUV )

- Recording & Storage
    - Board: Raspberry Pi 4 CM4 Lite + I/O Board
        - Storage: SD Card
            - Type: SD, SDHC, SDXC
            - Capacity: 2GB ~ 2TB
            - Speed Grade: UHS-I ( 104MB/s )
        - Recording
            - Video Codec: H.264
            - File Format: AVI

Image Sensor
-------------

+------------------+----------------------------------------+
| Image Sensor     | Description                            |
+==================+========================================+
| Manufacturer     | ``Sony IMX462``                        |
+------------------+----------------------------------------+
| Resolution       | ``1920x1080 @ 30fps``                  |
+------------------+----------------------------------------+
| Supported Format | ``RGB Raw Bayer``                      |
+------------------+----------------------------------------+

FPGA
-----

+------------------+----------------------------------------+
| FPGA            | Description                             |
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
| Video Processing | ``1080p@30fps, RGB/YUV Format``        |
+------------------+----------------------------------------+

Raspberry Pi 4 CM4 Lite + I/O Board
------------------------------------

+------------------+----------------------------------------+
| CM4 Lite        | Description                             |
+==================+========================================+
| Processor       | ``BCM2711 Quad-core Cortex-A72 64-bit`` |
+------------------+----------------------------------------+
| Memory          | ``Up to 8GB LPDDR4-2400 SDRAM``         |
+------------------+----------------------------------------+
| Video Codec     | ``H.265 ( 4Kp60 decode )``              |
|                 | ``H.264 ( 1080p60 decode, 1080p30 )``   |
+------------------+----------------------------------------+
| I/O             | ``USB 2.0 / 3.0``                       |
+------------------+----------------------------------------+


동작 환경
========

하위 항목
---------