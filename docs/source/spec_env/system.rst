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
        - Input Format: RGB Raw Bayer
        - Image Processing: Image composition ( RGB + NIR mode )
        - Output Format: YUV 4:2:0 ( YU12, YV12 )
        - Output Interface: HDMI (for display), USB2.0 (for recording)

- Recording & Storage
    - Board: Raspberry Pi 4 CM4 Lite + I/O Board
    - SD Card
        - Storage: 512GB
        - Speed Grade: UHS-I (104MB/s)
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
| Supported Format | ``RGB Raw Bayer / NIR``                |
+------------------+----------------------------------------+

FPGA
-----

+------------------+----------------------------------------+
| Image Sensor     | Description                            |
+==================+========================================+
| Manufacturer     | ``Sony IMX462``                        |
+------------------+----------------------------------------+
| Resolution       | ``1920x1080 @ 30fps``                  |
+------------------+----------------------------------------+
| Supported Format | ``RGB Raw Bayer / NIR``                |
+------------------+----------------------------------------+

Raspberry Pi 4 CM4 Lite + I/O Board
------------------------------------

+------------------+----------------------------------------+
| Image Sensor     | Description                            |
+==================+========================================+
| Manufacturer     | ``Sony IMX462``                        |
+------------------+----------------------------------------+
| Resolution       | ``1920x1080 @ 30fps``                  |
+------------------+----------------------------------------+
| Supported Format | ``RGB Raw Bayer / NIR``                |
+------------------+----------------------------------------+


동작 환경
========

하위 항목
---------