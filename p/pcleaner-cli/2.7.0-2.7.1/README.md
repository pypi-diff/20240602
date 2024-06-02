# Comparing `tmp/pcleaner_cli-2.7.0.tar.gz` & `tmp/pcleaner_cli-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner_cli-2.7.0.tar", last modified: Sun Jun  2 13:47:56 2024, max compression
+gzip compressed data, was "pcleaner_cli-2.7.1.tar", last modified: Sun Jun  2 15:48:06 2024, max compression
```

## Comparing `pcleaner_cli-2.7.0.tar` & `pcleaner_cli-2.7.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 13:47:56.977232 pcleaner_cli-2.7.0/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner_cli-2.7.0/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    18385 2024-06-02 13:47:56.977232 pcleaner_cli-2.7.0/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16700 2024-05-28 23:39:26.000000 pcleaner_cli-2.7.0/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 13:47:56.970565 pcleaner_cli-2.7.0/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2024-05-28 20:38:35.000000 pcleaner_cli-2.7.0/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23733 2024-04-14 22:05:44.000000 pcleaner_cli-2.7.0/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6988 2024-05-10 12:24:58.000000 pcleaner_cli-2.7.0/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 13:47:56.970565 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 13:47:56.970565 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 13:47:56.970565 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 13:47:56.973898 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    62869 2024-05-28 18:53:55.000000 pcleaner_cli-2.7.0/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10896 2024-05-10 12:24:58.000000 pcleaner_cli-2.7.0/pcleaner/ctd_interface.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 13:47:56.973898 pcleaner_cli-2.7.0/pcleaner/data/
--rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner_cli-2.7.0/pcleaner/data/LiberationSans-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner_cli-2.7.0/pcleaner/data/NotoMono-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner_cli-2.7.0/pcleaner/data/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4258 2024-05-10 13:16:37.000000 pcleaner_cli-2.7.0/pcleaner/data/windows_explorer_integration_regedit.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6796 2024-04-14 22:05:44.000000 pcleaner_cli-2.7.0/pcleaner/denoiser.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8909 2024-05-29 15:22:27.000000 pcleaner_cli-2.7.0/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35578 2024-05-10 12:24:58.000000 pcleaner_cli-2.7.0/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11506 2024-04-14 22:05:44.000000 pcleaner_cli-2.7.0/pcleaner/inpainting.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    31711 2024-06-02 13:45:15.000000 pcleaner_cli-2.7.0/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     9496 2024-04-14 22:05:44.000000 pcleaner_cli-2.7.0/pcleaner/masker.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7541 2024-04-14 22:05:44.000000 pcleaner_cli-2.7.0/pcleaner/model_downloader.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 13:47:56.973898 pcleaner_cli-2.7.0/pcleaner/ocr/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2024-05-10 12:24:58.000000 pcleaner_cli-2.7.0/pcleaner/ocr/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2457 2024-05-10 13:16:26.000000 pcleaner_cli-2.7.0/pcleaner/ocr/ocr.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1156 2024-05-10 12:24:58.000000 pcleaner_cli-2.7.0/pcleaner/ocr/ocr_mangaocr.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2738 2024-05-10 12:24:58.000000 pcleaner_cli-2.7.0/pcleaner/ocr/ocr_tesseract.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13032 2024-05-28 18:53:55.000000 pcleaner_cli-2.7.0/pcleaner/preprocessor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8311 2024-04-14 22:05:44.000000 pcleaner_cli-2.7.0/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    22204 2024-05-28 18:53:55.000000 pcleaner_cli-2.7.0/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 13:47:56.977232 pcleaner_cli-2.7.0/pcleaner_cli.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    18385 2024-06-02 13:47:56.000000 pcleaner_cli-2.7.0/pcleaner_cli.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1742 2024-06-02 13:47:56.000000 pcleaner_cli-2.7.0/pcleaner_cli.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2024-06-02 13:47:56.000000 pcleaner_cli-2.7.0/pcleaner_cli.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       52 2024-06-02 13:47:56.000000 pcleaner_cli-2.7.0/pcleaner_cli.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      431 2024-06-02 13:47:56.000000 pcleaner_cli-2.7.0/pcleaner_cli.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2024-06-02 13:47:56.000000 pcleaner_cli-2.7.0/pcleaner_cli.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2024-01-09 17:47:58.000000 pcleaner_cli-2.7.0/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1470 2024-06-02 13:47:56.977232 pcleaner_cli-2.7.0/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner_cli-2.7.0/setup.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 13:47:56.973898 pcleaner_cli-2.7.0/tests/
--rw-r--r--   0 corbin    (1000) corbin    (1001)      635 2024-02-11 23:18:20.000000 pcleaner_cli-2.7.0/tests/test_log_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:06.623762 pcleaner_cli-2.7.1/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner_cli-2.7.1/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    18746 2024-06-02 15:48:06.623762 pcleaner_cli-2.7.1/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    17013 2024-06-02 14:38:38.000000 pcleaner_cli-2.7.1/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:06.620428 pcleaner_cli-2.7.1/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2024-06-02 15:46:38.000000 pcleaner_cli-2.7.1/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23733 2024-04-14 22:05:44.000000 pcleaner_cli-2.7.1/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6988 2024-05-10 12:24:58.000000 pcleaner_cli-2.7.1/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:06.620428 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:06.620428 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:06.620428 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:06.620428 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    63083 2024-06-02 15:41:06.000000 pcleaner_cli-2.7.1/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10896 2024-05-10 12:24:58.000000 pcleaner_cli-2.7.1/pcleaner/ctd_interface.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:06.620428 pcleaner_cli-2.7.1/pcleaner/data/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner_cli-2.7.1/pcleaner/data/LiberationSans-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner_cli-2.7.1/pcleaner/data/NotoMono-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner_cli-2.7.1/pcleaner/data/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4258 2024-05-10 13:16:37.000000 pcleaner_cli-2.7.1/pcleaner/data/windows_explorer_integration_regedit.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6796 2024-04-14 22:05:44.000000 pcleaner_cli-2.7.1/pcleaner/denoiser.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8909 2024-06-02 14:39:00.000000 pcleaner_cli-2.7.1/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35578 2024-05-10 12:24:58.000000 pcleaner_cli-2.7.1/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11506 2024-04-14 22:05:44.000000 pcleaner_cli-2.7.1/pcleaner/inpainting.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    31711 2024-06-02 14:38:38.000000 pcleaner_cli-2.7.1/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     9496 2024-04-14 22:05:44.000000 pcleaner_cli-2.7.1/pcleaner/masker.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7541 2024-06-02 15:34:18.000000 pcleaner_cli-2.7.1/pcleaner/model_downloader.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:06.623762 pcleaner_cli-2.7.1/pcleaner/ocr/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2024-05-10 12:24:58.000000 pcleaner_cli-2.7.1/pcleaner/ocr/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2457 2024-05-10 13:16:26.000000 pcleaner_cli-2.7.1/pcleaner/ocr/ocr.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1156 2024-05-10 12:24:58.000000 pcleaner_cli-2.7.1/pcleaner/ocr/ocr_mangaocr.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2738 2024-06-02 15:34:18.000000 pcleaner_cli-2.7.1/pcleaner/ocr/ocr_tesseract.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13032 2024-06-02 15:34:18.000000 pcleaner_cli-2.7.1/pcleaner/preprocessor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8311 2024-04-14 22:05:44.000000 pcleaner_cli-2.7.1/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    22204 2024-06-02 15:34:18.000000 pcleaner_cli-2.7.1/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:06.623762 pcleaner_cli-2.7.1/pcleaner_cli.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    18746 2024-06-02 15:48:06.000000 pcleaner_cli-2.7.1/pcleaner_cli.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1742 2024-06-02 15:48:06.000000 pcleaner_cli-2.7.1/pcleaner_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2024-06-02 15:48:06.000000 pcleaner_cli-2.7.1/pcleaner_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       52 2024-06-02 15:48:06.000000 pcleaner_cli-2.7.1/pcleaner_cli.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      467 2024-06-02 15:48:06.000000 pcleaner_cli-2.7.1/pcleaner_cli.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2024-06-02 15:48:06.000000 pcleaner_cli-2.7.1/pcleaner_cli.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2024-01-09 17:47:58.000000 pcleaner_cli-2.7.1/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1504 2024-06-02 15:48:06.623762 pcleaner_cli-2.7.1/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner_cli-2.7.1/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:06.623762 pcleaner_cli-2.7.1/tests/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      635 2024-02-11 23:18:20.000000 pcleaner_cli-2.7.1/tests/test_log_parser.py
```

### Comparing `pcleaner_cli-2.7.0/LICENSE` & `pcleaner_cli-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/PKG-INFO` & `pcleaner_cli-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner-cli
-Version: 2.7.0
+Version: 2.7.1
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -36,14 +36,15 @@
 Requires-Dist: PySide6>=6.7.0
 Requires-Dist: attrs
 Requires-Dist: psutil
 Requires-Dist: dictdiffer
 Requires-Dist: humanfriendly
 Requires-Dist: simple_lama_inpainting
 Requires-Dist: pytesseract
+Requires-Dist: strenum; python_version < "3.11"
 Requires-Dist: python-magic; platform_system != "Windows"
 Requires-Dist: python-magic-bin; platform_system == "Windows"
 Requires-Dist: dbus-python; platform_system == "Linux"
 Requires-Dist: pywin32; platform_system == "Windows"
 Requires-Dist: win10toast; platform_system == "Windows"
 Requires-Dist: pyuac; platform_system == "Windows"
 
@@ -149,30 +150,36 @@
 
 As you can see, with a bit of extra cleanup applied to the AI output, some leftover text and jpeg compression artifacts are removed, and the bubble is fully cleaned. \
 When fully cleaning it isn't possible, Panel Cleaner will instead skip the bubble so as not to waste your time with a poorly cleaned bit of text. The exact cleaning behavior is highly configurable, see [Profiles](#profiles) for more details.
 
 
 ## Installation
 
-You have the choice between installing a pre-built binary from the [releases section](https://github.com/VoxelCubes/PanelCleaner/releases/latest) 
+You have the choice between installing a pre-built binary (exe or elf) from the [releases section](https://github.com/VoxelCubes/PanelCleaner/releases/latest) (**recommended for most users**),
 or installing it to your local python interpreter using pip.
 
 Note: All versions will need to download model data on first launch (approx. 500MB). This model data will not need to be downloaded again if Panel Cleaner updates.
 
 Important: The pre-built binaries do not support CUDA acceleration. To use CUDA, you must install the program with pip and ensure you install the appropriate [pytorch](https://pytorch.org/get-started/locally/) version for your system.
 
 ### Install with Pip
 
-The program requires **Python 3.10** or newer.
+The program requires **Python 3.10 or newer**.
 
-Install the program with pip from [PyPI](https://pypi.org/project/pcleaner/):
+Install the program with both the command line interface and graphical interface using pip from [PyPI](https://pypi.org/project/pcleaner/):
 ```bash
 pip install pcleaner
 ```
 
+Or if you only wish to use the command line interface:
+```bash
+pip install pcleaner-cli
+```
+Note: `pcleaner` and `pcleaner-cli` can be installed side by side, but the CLI-only package would be redundant.
+
 Note: The program has been tested to work on Linux, MacOS, and Windows, with varying levels of setup required. See the [FAQ](https://github.com/VoxelCubes/PanelCleaner/blob/master/docs/faq.md) for help.
 
 ### Installation from the Arch User Repository
 
 This installs the program in a `pipx` environment, which allows pytorch to download the appropriate CUDA version for your system, making this the best method of installation.
 
 You can find the package here: [panelcleaner](https://aur.archlinux.org/packages/panelcleaner)
```

### Comparing `pcleaner_cli-2.7.0/README.md` & `pcleaner_cli-2.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,30 +100,36 @@
 
 As you can see, with a bit of extra cleanup applied to the AI output, some leftover text and jpeg compression artifacts are removed, and the bubble is fully cleaned. \
 When fully cleaning it isn't possible, Panel Cleaner will instead skip the bubble so as not to waste your time with a poorly cleaned bit of text. The exact cleaning behavior is highly configurable, see [Profiles](#profiles) for more details.
 
 
 ## Installation
 
-You have the choice between installing a pre-built binary from the [releases section](https://github.com/VoxelCubes/PanelCleaner/releases/latest) 
+You have the choice between installing a pre-built binary (exe or elf) from the [releases section](https://github.com/VoxelCubes/PanelCleaner/releases/latest) (**recommended for most users**),
 or installing it to your local python interpreter using pip.
 
 Note: All versions will need to download model data on first launch (approx. 500MB). This model data will not need to be downloaded again if Panel Cleaner updates.
 
 Important: The pre-built binaries do not support CUDA acceleration. To use CUDA, you must install the program with pip and ensure you install the appropriate [pytorch](https://pytorch.org/get-started/locally/) version for your system.
 
 ### Install with Pip
 
-The program requires **Python 3.10** or newer.
+The program requires **Python 3.10 or newer**.
 
-Install the program with pip from [PyPI](https://pypi.org/project/pcleaner/):
+Install the program with both the command line interface and graphical interface using pip from [PyPI](https://pypi.org/project/pcleaner/):
 ```bash
 pip install pcleaner
 ```
 
+Or if you only wish to use the command line interface:
+```bash
+pip install pcleaner-cli
+```
+Note: `pcleaner` and `pcleaner-cli` can be installed side by side, but the CLI-only package would be redundant.
+
 Note: The program has been tested to work on Linux, MacOS, and Windows, with varying levels of setup required. See the [FAQ](https://github.com/VoxelCubes/PanelCleaner/blob/master/docs/faq.md) for help.
 
 ### Installation from the Arch User Repository
 
 This installs the program in a `pipx` environment, which allows pytorch to download the appropriate CUDA version for your system, making this the best method of installation.
 
 You can find the package here: [panelcleaner](https://aur.archlinux.org/packages/panelcleaner)
```

### Comparing `pcleaner_cli-2.7.0/pcleaner/analytics.py` & `pcleaner_cli-2.7.1/pcleaner/analytics.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/cli_utils.py` & `pcleaner_cli-2.7.1/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/basemodel.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/inference.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/export.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/general.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner_cli-2.7.1/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/config.py` & `pcleaner_cli-2.7.1/pcleaner/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import re
 import sys
 import shutil
 from collections import defaultdict
-from enum import StrEnum
 from pathlib import Path
 from typing import Any, NewType
 
 import configupdater as cu
 from attrs import define, field
 from loguru import logger
 
 from pcleaner.helpers import tr
 from pcleaner import cli_utils as cli
 from pcleaner import helpers as hp
 from pcleaner import model_downloader as md
 
+# If using Python 3.10 or older, use the 3rd party StrEnum.
+if sys.version_info < (3, 11):
+    from strenum import StrEnum
+else:
+    from enum import StrEnum
+
 # Logging session markers.
 STARTUP_MESSAGE = "---- Starting up ----"
 SHUTDOWN_MESSAGE = "---- Shutting down ----"
 
 # Supported image suffixes.
 SUPPORTED_IMG_TYPES = [
     ".jpeg",
@@ -962,23 +967,27 @@
             self.profile_editor if self.profile_editor is not None else "System default",
         )
         print(
             "Cache Directory:", self.cache_dir if self.cache_dir is not None else "System default"
         )
         print(
             "Default Torch Model Path:",
-            self.default_torch_model_path
-            if self.default_torch_model_path is not None
-            else "Not downloaded",
+            (
+                self.default_torch_model_path
+                if self.default_torch_model_path is not None
+                else "Not downloaded"
+            ),
         )
         print(
             "Default CV2 Model Path:",
-            self.default_cv2_model_path
-            if self.default_cv2_model_path is not None
-            else "Not downloaded",
+            (
+                self.default_cv2_model_path
+                if self.default_cv2_model_path is not None
+                else "Not downloaded"
+            ),
         )
         print(
             "GUI Theme:",
             self.gui_theme if self.gui_theme is not None else "System default",
         )
 
         print("\n" + "-" * 20 + "\n")
```

### Comparing `pcleaner_cli-2.7.0/pcleaner/ctd_interface.py` & `pcleaner_cli-2.7.1/pcleaner/ctd_interface.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/data/LiberationSans-Regular.ttf` & `pcleaner_cli-2.7.1/pcleaner/data/LiberationSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/data/NotoMono-Regular.ttf` & `pcleaner_cli-2.7.1/pcleaner/data/NotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/data/windows_explorer_integration_regedit.py` & `pcleaner_cli-2.7.1/pcleaner/data/windows_explorer_integration_regedit.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/denoiser.py` & `pcleaner_cli-2.7.1/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/helpers.py` & `pcleaner_cli-2.7.1/pcleaner/helpers.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/image_ops.py` & `pcleaner_cli-2.7.1/pcleaner/image_ops.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/inpainting.py` & `pcleaner_cli-2.7.1/pcleaner/inpainting.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/main.py` & `pcleaner_cli-2.7.1/pcleaner/main.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/masker.py` & `pcleaner_cli-2.7.1/pcleaner/masker.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/model_downloader.py` & `pcleaner_cli-2.7.1/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/ocr/ocr.py` & `pcleaner_cli-2.7.1/pcleaner/ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/ocr/ocr_mangaocr.py` & `pcleaner_cli-2.7.1/pcleaner/ocr/ocr_mangaocr.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/ocr/ocr_tesseract.py` & `pcleaner_cli-2.7.1/pcleaner/ocr/ocr_tesseract.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/preprocessor.py` & `pcleaner_cli-2.7.1/pcleaner/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/profile_cli.py` & `pcleaner_cli-2.7.1/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner/structures.py` & `pcleaner_cli-2.7.1/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/pcleaner_cli.egg-info/PKG-INFO` & `pcleaner_cli-2.7.1/pcleaner_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner-cli
-Version: 2.7.0
+Version: 2.7.1
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -36,14 +36,15 @@
 Requires-Dist: PySide6>=6.7.0
 Requires-Dist: attrs
 Requires-Dist: psutil
 Requires-Dist: dictdiffer
 Requires-Dist: humanfriendly
 Requires-Dist: simple_lama_inpainting
 Requires-Dist: pytesseract
+Requires-Dist: strenum; python_version < "3.11"
 Requires-Dist: python-magic; platform_system != "Windows"
 Requires-Dist: python-magic-bin; platform_system == "Windows"
 Requires-Dist: dbus-python; platform_system == "Linux"
 Requires-Dist: pywin32; platform_system == "Windows"
 Requires-Dist: win10toast; platform_system == "Windows"
 Requires-Dist: pyuac; platform_system == "Windows"
 
@@ -149,30 +150,36 @@
 
 As you can see, with a bit of extra cleanup applied to the AI output, some leftover text and jpeg compression artifacts are removed, and the bubble is fully cleaned. \
 When fully cleaning it isn't possible, Panel Cleaner will instead skip the bubble so as not to waste your time with a poorly cleaned bit of text. The exact cleaning behavior is highly configurable, see [Profiles](#profiles) for more details.
 
 
 ## Installation
 
-You have the choice between installing a pre-built binary from the [releases section](https://github.com/VoxelCubes/PanelCleaner/releases/latest) 
+You have the choice between installing a pre-built binary (exe or elf) from the [releases section](https://github.com/VoxelCubes/PanelCleaner/releases/latest) (**recommended for most users**),
 or installing it to your local python interpreter using pip.
 
 Note: All versions will need to download model data on first launch (approx. 500MB). This model data will not need to be downloaded again if Panel Cleaner updates.
 
 Important: The pre-built binaries do not support CUDA acceleration. To use CUDA, you must install the program with pip and ensure you install the appropriate [pytorch](https://pytorch.org/get-started/locally/) version for your system.
 
 ### Install with Pip
 
-The program requires **Python 3.10** or newer.
+The program requires **Python 3.10 or newer**.
 
-Install the program with pip from [PyPI](https://pypi.org/project/pcleaner/):
+Install the program with both the command line interface and graphical interface using pip from [PyPI](https://pypi.org/project/pcleaner/):
 ```bash
 pip install pcleaner
 ```
 
+Or if you only wish to use the command line interface:
+```bash
+pip install pcleaner-cli
+```
+Note: `pcleaner` and `pcleaner-cli` can be installed side by side, but the CLI-only package would be redundant.
+
 Note: The program has been tested to work on Linux, MacOS, and Windows, with varying levels of setup required. See the [FAQ](https://github.com/VoxelCubes/PanelCleaner/blob/master/docs/faq.md) for help.
 
 ### Installation from the Arch User Repository
 
 This installs the program in a `pipx` environment, which allows pytorch to download the appropriate CUDA version for your system, making this the best method of installation.
 
 You can find the package here: [panelcleaner](https://aur.archlinux.org/packages/panelcleaner)
```

### Comparing `pcleaner_cli-2.7.0/pcleaner_cli.egg-info/SOURCES.txt` & `pcleaner_cli-2.7.1/pcleaner_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcleaner_cli-2.7.0/setup.cfg` & `pcleaner_cli-2.7.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 	PySide6 >= 6.7.0
 	attrs
 	psutil
 	dictdiffer
 	humanfriendly
 	simple_lama_inpainting
 	pytesseract
+	strenum; python_version < "3.11"
 	python-magic; platform_system != "Windows"
 	python-magic-bin; platform_system == "Windows"
 	dbus-python; platform_system == "Linux"
 	pywin32; platform_system == "Windows"
 	win10toast; platform_system == "Windows"
 	pyuac; platform_system == "Windows"
 python_requires = >=3.10
```

### Comparing `pcleaner_cli-2.7.0/tests/test_log_parser.py` & `pcleaner_cli-2.7.1/tests/test_log_parser.py`

 * *Files identical despite different names*

