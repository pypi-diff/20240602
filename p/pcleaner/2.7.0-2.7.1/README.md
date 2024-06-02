# Comparing `tmp/pcleaner-2.7.0.tar.gz` & `tmp/pcleaner-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-2.7.0.tar", last modified: Tue May 28 20:47:41 2024, max compression
+gzip compressed data, was "pcleaner-2.7.1.tar", last modified: Sun Jun  2 15:48:02 2024, max compression
```

## Comparing `pcleaner-2.7.0.tar` & `pcleaner-2.7.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.718572 pcleaner-2.7.0/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-2.7.0/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    18341 2024-05-28 20:47:41.718572 pcleaner-2.7.0/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16660 2024-05-28 20:41:47.000000 pcleaner-2.7.0/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.701906 pcleaner-2.7.0/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2024-05-28 20:38:35.000000 pcleaner-2.7.0/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23733 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6988 2024-05-10 12:24:58.000000 pcleaner-2.7.0/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.701906 pcleaner-2.7.0/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.701906 pcleaner-2.7.0/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.701906 pcleaner-2.7.0/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.705239 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-2.7.0/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    62869 2024-05-28 18:53:55.000000 pcleaner-2.7.0/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10896 2024-05-10 12:24:58.000000 pcleaner-2.7.0/pcleaner/ctd_interface.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.705239 pcleaner-2.7.0/pcleaner/data/
--rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-2.7.0/pcleaner/data/LiberationSans-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-2.7.0/pcleaner/data/NotoMono-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-2.7.0/pcleaner/data/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4258 2024-05-10 13:16:37.000000 pcleaner-2.7.0/pcleaner/data/windows_explorer_integration_regedit.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6796 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/denoiser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.711906 pcleaner-2.7.0/pcleaner/gui/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.711906 pcleaner-2.7.0/pcleaner/gui/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5671 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/gui/CustomQ/CBadgeButton.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2642 2024-01-25 04:44:05.000000 pcleaner-2.7.0/pcleaner/gui/CustomQ/CColorButton.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4791 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/gui/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      682 2023-10-07 13:58:30.000000 pcleaner-2.7.0/pcleaner/gui/CustomQ/CDropFrame.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2092 2023-10-07 13:58:30.000000 pcleaner-2.7.0/pcleaner/gui/CustomQ/CElidedLabel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3345 2024-05-10 13:25:48.000000 pcleaner-2.7.0/pcleaner/gui/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1150 2024-02-15 00:39:49.000000 pcleaner-2.7.0/pcleaner/gui/CustomQ/CTextEdit.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1628 2023-10-07 13:58:30.000000 pcleaner-2.7.0/pcleaner/gui/CustomQ/CTooltipLabel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-2.7.0/pcleaner/gui/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-2.7.0/pcleaner/gui/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1381 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/gui/about_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5972 2024-05-10 13:21:07.000000 pcleaner-2.7.0/pcleaner/gui/ctd_interface_gui.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2293 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/gui/error_dialog_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11024 2024-05-10 12:24:58.000000 pcleaner-2.7.0/pcleaner/gui/file_manager_extension_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27405 2024-05-10 12:24:58.000000 pcleaner-2.7.0/pcleaner/gui/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14573 2024-05-28 19:37:33.000000 pcleaner-2.7.0/pcleaner/gui/gui_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    34445 2024-05-28 18:53:55.000000 pcleaner-2.7.0/pcleaner/gui/image_details_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    22000 2024-05-10 12:24:58.000000 pcleaner-2.7.0/pcleaner/gui/image_file.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4351 2024-05-10 12:24:58.000000 pcleaner-2.7.0/pcleaner/gui/image_tab.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7561 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/gui/image_viewer.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3591 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/gui/issue_reporter_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6633 2024-05-10 12:24:58.000000 pcleaner-2.7.0/pcleaner/gui/launcher.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      519 2023-10-07 13:58:30.000000 pcleaner-2.7.0/pcleaner/gui/license_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3563 2024-02-12 16:50:11.000000 pcleaner-2.7.0/pcleaner/gui/log_parser.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4873 2024-02-12 23:21:16.000000 pcleaner-2.7.0/pcleaner/gui/log_viewer.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    66431 2024-05-28 19:37:47.000000 pcleaner-2.7.0/pcleaner/gui/mainwindow_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    19431 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/gui/model_downloader_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4648 2023-10-07 13:58:30.000000 pcleaner-2.7.0/pcleaner/gui/new_profile_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    42480 2024-05-28 18:53:55.000000 pcleaner-2.7.0/pcleaner/gui/processing.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    22466 2024-05-28 18:53:55.000000 pcleaner-2.7.0/pcleaner/gui/profile_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.715239 pcleaner-2.7.0/pcleaner/gui/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-2.7.0/pcleaner/gui/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   152834 2024-05-28 20:47:39.000000 pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_icons.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   166313 2024-05-28 20:47:39.000000 pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_theme_icons.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4452 2024-05-28 20:47:39.000000 pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_themes.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   450977 2024-05-28 18:53:55.000000 pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_translations.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   159185 2024-05-28 20:38:35.000000 pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_windows_icons.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)   171403 2024-05-28 20:38:35.000000 pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_windows_theme_icons.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4675 2024-05-28 20:38:35.000000 pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_windows_themes.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)  1131372 2024-05-28 20:38:35.000000 pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_windows_translations.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      956 2024-03-02 00:01:57.000000 pcleaner-2.7.0/pcleaner/gui/setup_greeter_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      557 2024-05-10 13:28:08.000000 pcleaner-2.7.0/pcleaner/gui/structures.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      758 2024-05-28 18:53:55.000000 pcleaner-2.7.0/pcleaner/gui/supported_languages.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.718572 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2024-02-12 21:19:18.000000 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6619 2024-05-28 20:47:39.000000 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_About.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5576 2024-05-28 20:47:39.000000 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4481 2024-05-28 20:47:39.000000 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13725 2024-05-28 20:47:39.000000 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6367 2024-05-28 20:47:39.000000 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_IssueReporter.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    41024 2024-05-28 20:47:39.000000 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_License.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    49222 2024-05-28 20:47:39.000000 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6958 2024-05-28 20:47:39.000000 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7411 2024-05-28 20:47:40.000000 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_NewProfile.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    12580 2024-05-28 20:47:40.000000 pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5545 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/gui/worker_thread.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8826 2024-05-01 21:35:49.000000 pcleaner-2.7.0/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35578 2024-05-10 12:24:58.000000 pcleaner-2.7.0/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11506 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/inpainting.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    31089 2024-05-10 13:13:32.000000 pcleaner-2.7.0/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     9496 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/masker.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7541 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/model_downloader.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.718572 pcleaner-2.7.0/pcleaner/ocr/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2024-05-10 12:24:58.000000 pcleaner-2.7.0/pcleaner/ocr/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2457 2024-05-10 13:16:26.000000 pcleaner-2.7.0/pcleaner/ocr/ocr.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1156 2024-05-10 12:24:58.000000 pcleaner-2.7.0/pcleaner/ocr/ocr_mangaocr.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2738 2024-05-10 12:24:58.000000 pcleaner-2.7.0/pcleaner/ocr/ocr_tesseract.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13032 2024-05-28 18:53:55.000000 pcleaner-2.7.0/pcleaner/preprocessor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8311 2024-04-14 22:05:44.000000 pcleaner-2.7.0/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    22204 2024-05-28 18:53:55.000000 pcleaner-2.7.0/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.718572 pcleaner-2.7.0/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    18341 2024-05-28 20:47:41.000000 pcleaner-2.7.0/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3834 2024-05-28 20:47:41.000000 pcleaner-2.7.0/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2024-05-28 20:47:41.000000 pcleaner-2.7.0/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       90 2024-05-28 20:47:41.000000 pcleaner-2.7.0/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      431 2024-05-28 20:47:41.000000 pcleaner-2.7.0/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2024-05-28 20:47:41.000000 pcleaner-2.7.0/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2024-01-09 17:47:58.000000 pcleaner-2.7.0/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1532 2024-05-28 20:47:41.718572 pcleaner-2.7.0/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-2.7.0/setup.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-05-28 20:47:41.718572 pcleaner-2.7.0/tests/
--rw-r--r--   0 corbin    (1000) corbin    (1001)      635 2024-02-11 23:18:20.000000 pcleaner-2.7.0/tests/test_log_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.247095 pcleaner-2.7.1/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-2.7.1/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    18742 2024-06-02 15:48:02.247095 pcleaner-2.7.1/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    17013 2024-06-02 14:38:38.000000 pcleaner-2.7.1/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.237095 pcleaner-2.7.1/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2024-06-02 15:46:38.000000 pcleaner-2.7.1/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23733 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6988 2024-05-10 12:24:58.000000 pcleaner-2.7.1/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.240428 pcleaner-2.7.1/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.240428 pcleaner-2.7.1/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.240428 pcleaner-2.7.1/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.240428 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-2.7.1/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    63083 2024-06-02 15:41:06.000000 pcleaner-2.7.1/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10896 2024-05-10 12:24:58.000000 pcleaner-2.7.1/pcleaner/ctd_interface.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.240428 pcleaner-2.7.1/pcleaner/data/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-2.7.1/pcleaner/data/LiberationSans-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-2.7.1/pcleaner/data/NotoMono-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-2.7.1/pcleaner/data/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4258 2024-05-10 13:16:37.000000 pcleaner-2.7.1/pcleaner/data/windows_explorer_integration_regedit.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6796 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/denoiser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.243762 pcleaner-2.7.1/pcleaner/gui/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.243762 pcleaner-2.7.1/pcleaner/gui/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5671 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/gui/CustomQ/CBadgeButton.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2642 2024-01-25 04:44:05.000000 pcleaner-2.7.1/pcleaner/gui/CustomQ/CColorButton.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4791 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/gui/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      682 2023-10-07 13:58:30.000000 pcleaner-2.7.1/pcleaner/gui/CustomQ/CDropFrame.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2092 2023-10-07 13:58:30.000000 pcleaner-2.7.1/pcleaner/gui/CustomQ/CElidedLabel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3345 2024-05-10 13:25:48.000000 pcleaner-2.7.1/pcleaner/gui/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1150 2024-02-15 00:39:49.000000 pcleaner-2.7.1/pcleaner/gui/CustomQ/CTextEdit.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1628 2023-10-07 13:58:30.000000 pcleaner-2.7.1/pcleaner/gui/CustomQ/CTooltipLabel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-2.7.1/pcleaner/gui/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-2.7.1/pcleaner/gui/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1381 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/gui/about_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5972 2024-05-10 13:21:07.000000 pcleaner-2.7.1/pcleaner/gui/ctd_interface_gui.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2293 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/gui/error_dialog_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11024 2024-05-10 12:24:58.000000 pcleaner-2.7.1/pcleaner/gui/file_manager_extension_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27405 2024-05-10 12:24:58.000000 pcleaner-2.7.1/pcleaner/gui/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14573 2024-06-02 14:15:17.000000 pcleaner-2.7.1/pcleaner/gui/gui_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    34445 2024-06-02 14:15:17.000000 pcleaner-2.7.1/pcleaner/gui/image_details_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    22000 2024-05-10 12:24:58.000000 pcleaner-2.7.1/pcleaner/gui/image_file.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4351 2024-05-10 12:24:58.000000 pcleaner-2.7.1/pcleaner/gui/image_tab.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7561 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/gui/image_viewer.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3591 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/gui/issue_reporter_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6633 2024-05-10 12:24:58.000000 pcleaner-2.7.1/pcleaner/gui/launcher.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      519 2023-10-07 13:58:30.000000 pcleaner-2.7.1/pcleaner/gui/license_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3563 2024-02-12 16:50:11.000000 pcleaner-2.7.1/pcleaner/gui/log_parser.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4873 2024-02-12 23:21:16.000000 pcleaner-2.7.1/pcleaner/gui/log_viewer.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    66431 2024-05-28 19:37:47.000000 pcleaner-2.7.1/pcleaner/gui/mainwindow_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    19431 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/gui/model_downloader_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4648 2023-10-07 13:58:30.000000 pcleaner-2.7.1/pcleaner/gui/new_profile_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    42480 2024-06-02 14:15:17.000000 pcleaner-2.7.1/pcleaner/gui/processing.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    22466 2024-06-02 15:34:18.000000 pcleaner-2.7.1/pcleaner/gui/profile_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.247095 pcleaner-2.7.1/pcleaner/gui/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-2.7.1/pcleaner/gui/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   152834 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   166270 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_theme_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4443 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_themes.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   450977 2024-06-02 14:15:17.000000 pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_translations.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   159185 2024-06-02 14:15:17.000000 pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_windows_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   171403 2024-06-02 14:15:17.000000 pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_windows_theme_icons.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4675 2024-05-28 20:38:35.000000 pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_windows_themes.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)  1131372 2024-06-02 14:15:17.000000 pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_windows_translations.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      956 2024-03-02 00:01:57.000000 pcleaner-2.7.1/pcleaner/gui/setup_greeter_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      557 2024-05-10 13:28:08.000000 pcleaner-2.7.1/pcleaner/gui/structures.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      758 2024-06-02 14:15:17.000000 pcleaner-2.7.1/pcleaner/gui/supported_languages.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.247095 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2024-02-12 21:19:18.000000 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6619 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_About.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5576 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4481 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13725 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6367 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_IssueReporter.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    41024 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_License.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    49222 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6958 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7411 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_NewProfile.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12580 2024-06-02 15:48:00.000000 pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5545 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/gui/worker_thread.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8909 2024-06-02 14:39:00.000000 pcleaner-2.7.1/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35578 2024-05-10 12:24:58.000000 pcleaner-2.7.1/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11506 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/inpainting.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    31711 2024-06-02 14:38:38.000000 pcleaner-2.7.1/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     9496 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/masker.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7541 2024-06-02 15:34:18.000000 pcleaner-2.7.1/pcleaner/model_downloader.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.247095 pcleaner-2.7.1/pcleaner/ocr/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2024-05-10 12:24:58.000000 pcleaner-2.7.1/pcleaner/ocr/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2457 2024-05-10 13:16:26.000000 pcleaner-2.7.1/pcleaner/ocr/ocr.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1156 2024-05-10 12:24:58.000000 pcleaner-2.7.1/pcleaner/ocr/ocr_mangaocr.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2738 2024-06-02 15:34:18.000000 pcleaner-2.7.1/pcleaner/ocr/ocr_tesseract.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13032 2024-06-02 15:34:18.000000 pcleaner-2.7.1/pcleaner/preprocessor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8311 2024-04-14 22:05:44.000000 pcleaner-2.7.1/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    22204 2024-06-02 15:34:18.000000 pcleaner-2.7.1/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.247095 pcleaner-2.7.1/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    18742 2024-06-02 15:48:02.000000 pcleaner-2.7.1/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3834 2024-06-02 15:48:02.000000 pcleaner-2.7.1/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2024-06-02 15:48:02.000000 pcleaner-2.7.1/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       90 2024-06-02 15:48:02.000000 pcleaner-2.7.1/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      467 2024-06-02 15:48:02.000000 pcleaner-2.7.1/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2024-06-02 15:48:02.000000 pcleaner-2.7.1/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2024-01-09 17:47:58.000000 pcleaner-2.7.1/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1566 2024-06-02 15:48:02.247095 pcleaner-2.7.1/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-2.7.1/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2024-06-02 15:48:02.247095 pcleaner-2.7.1/tests/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      635 2024-02-11 23:18:20.000000 pcleaner-2.7.1/tests/test_log_parser.py
```

### Comparing `pcleaner-2.7.0/LICENSE` & `pcleaner-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/PKG-INFO` & `pcleaner-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
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
 
@@ -94,15 +95,15 @@
 
 ## Features
 
 - Cleans text bubbles without leaving artifacts.
 
 - Avoids painting over parts of the image that aren't text.
 
-- Inpaints bubbles that can't simply be masked out.
+- Inpaints bubbles (with LaMa machine learning) that can't simply be masked out.
 
 - Ignores bubbles containing only symbols or numbers, as those don't need translation.
 
 - Offers a GUI for easy use, dark, light, and system themes are supported.
 
 - No internet connection required after installing the model data.
 
@@ -117,15 +118,15 @@
 
 - Can handle bubbles on any solid grayscale background color.
 
 - Can also cut out the text from the rest of the image, e.g. to paste it over a colored rendition.
 
 - Can also run OCR on the pages and output the text to a file.
 
-- Interface available in: English, German (See [Translating](https://github.com/VoxelCubes/PanelCleaner/blob/master/translations/TRANSLATING.md) for more languages)
+- Interface available in: English, German, Bulgarian (See [Translating](https://github.com/VoxelCubes/PanelCleaner/blob/master/translations/TRANSLATING.md) for more languages)
 
 
 ## Limitations
 
 - It only supports Japanese and English text for cleaning (success may vary with other languages), Japanese only for OCR.
 
 - Supported file types: .jpeg, .jpg, .png, .bmp, .tiff, .tif, .jp2, .dib, .webp, .ppm
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

### Comparing `pcleaner-2.7.0/README.md` & `pcleaner-2.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 ## Features
 
 - Cleans text bubbles without leaving artifacts.
 
 - Avoids painting over parts of the image that aren't text.
 
-- Inpaints bubbles that can't simply be masked out.
+- Inpaints bubbles (with LaMa machine learning) that can't simply be masked out.
 
 - Ignores bubbles containing only symbols or numbers, as those don't need translation.
 
 - Offers a GUI for easy use, dark, light, and system themes are supported.
 
 - No internet connection required after installing the model data.
 
@@ -68,15 +68,15 @@
 
 - Can handle bubbles on any solid grayscale background color.
 
 - Can also cut out the text from the rest of the image, e.g. to paste it over a colored rendition.
 
 - Can also run OCR on the pages and output the text to a file.
 
-- Interface available in: English, German (See [Translating](https://github.com/VoxelCubes/PanelCleaner/blob/master/translations/TRANSLATING.md) for more languages)
+- Interface available in: English, German, Bulgarian (See [Translating](https://github.com/VoxelCubes/PanelCleaner/blob/master/translations/TRANSLATING.md) for more languages)
 
 
 ## Limitations
 
 - It only supports Japanese and English text for cleaning (success may vary with other languages), Japanese only for OCR.
 
 - Supported file types: .jpeg, .jpg, .png, .bmp, .tiff, .tif, .jp2, .dib, .webp, .ppm
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

### Comparing `pcleaner-2.7.0/pcleaner/analytics.py` & `pcleaner-2.7.1/pcleaner/analytics.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/cli_utils.py` & `pcleaner-2.7.1/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/inference.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-2.7.1/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/config.py` & `pcleaner-2.7.1/pcleaner/config.py`

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

### Comparing `pcleaner-2.7.0/pcleaner/ctd_interface.py` & `pcleaner-2.7.1/pcleaner/ctd_interface.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/data/LiberationSans-Regular.ttf` & `pcleaner-2.7.1/pcleaner/data/LiberationSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/data/NotoMono-Regular.ttf` & `pcleaner-2.7.1/pcleaner/data/NotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/data/windows_explorer_integration_regedit.py` & `pcleaner-2.7.1/pcleaner/data/windows_explorer_integration_regedit.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/denoiser.py` & `pcleaner-2.7.1/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/CustomQ/CBadgeButton.py` & `pcleaner-2.7.1/pcleaner/gui/CustomQ/CBadgeButton.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/CustomQ/CColorButton.py` & `pcleaner-2.7.1/pcleaner/gui/CustomQ/CColorButton.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/CustomQ/CComboBox.py` & `pcleaner-2.7.1/pcleaner/gui/CustomQ/CComboBox.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/CustomQ/CDropFrame.py` & `pcleaner-2.7.1/pcleaner/gui/CustomQ/CDropFrame.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/CustomQ/CElidedLabel.py` & `pcleaner-2.7.1/pcleaner/gui/CustomQ/CElidedLabel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/CustomQ/CTableWidget.py` & `pcleaner-2.7.1/pcleaner/gui/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/CustomQ/CTextEdit.py` & `pcleaner-2.7.1/pcleaner/gui/CustomQ/CTextEdit.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/CustomQ/CTooltipLabel.py` & `pcleaner-2.7.1/pcleaner/gui/CustomQ/CTooltipLabel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/about_driver.py` & `pcleaner-2.7.1/pcleaner/gui/about_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/ctd_interface_gui.py` & `pcleaner-2.7.1/pcleaner/gui/ctd_interface_gui.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/error_dialog_driver.py` & `pcleaner-2.7.1/pcleaner/gui/error_dialog_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/file_manager_extension_driver.py` & `pcleaner-2.7.1/pcleaner/gui/file_manager_extension_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/file_table.py` & `pcleaner-2.7.1/pcleaner/gui/file_table.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/gui_utils.py` & `pcleaner-2.7.1/pcleaner/gui/gui_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/image_details_driver.py` & `pcleaner-2.7.1/pcleaner/gui/image_details_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/image_file.py` & `pcleaner-2.7.1/pcleaner/gui/image_file.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/image_tab.py` & `pcleaner-2.7.1/pcleaner/gui/image_tab.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/image_viewer.py` & `pcleaner-2.7.1/pcleaner/gui/image_viewer.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/issue_reporter_driver.py` & `pcleaner-2.7.1/pcleaner/gui/issue_reporter_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/launcher.py` & `pcleaner-2.7.1/pcleaner/gui/launcher.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/license_driver.py` & `pcleaner-2.7.1/pcleaner/gui/license_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/log_parser.py` & `pcleaner-2.7.1/pcleaner/gui/log_parser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/log_viewer.py` & `pcleaner-2.7.1/pcleaner/gui/log_viewer.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/mainwindow_driver.py` & `pcleaner-2.7.1/pcleaner/gui/mainwindow_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/model_downloader_driver.py` & `pcleaner-2.7.1/pcleaner/gui/model_downloader_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/new_profile_driver.py` & `pcleaner-2.7.1/pcleaner/gui/new_profile_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/processing.py` & `pcleaner-2.7.1/pcleaner/gui/processing.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/profile_parser.py` & `pcleaner-2.7.1/pcleaner/gui/profile_parser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_icons.py` & `pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_icons.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_theme_icons.py` & `pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_theme_icons.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,243 +2,243 @@
 # Created by: object code
 # Created by: The Resource Compiler for Qt version 6.7.0
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
-\x00\x00\x0e$\
+\x00\x00\x0e%\
 (\
-\xb5/\xfd`\xb3K\xd5p\x00\xcan\xb0\x17I\xb0\x96\
+\xb5/\xfd`\xb3K\xddp\x00:o\xc4\x17I\xb0\x96\
 q\x0e\xa81\x8e\x1b\xdf\x82|\xc5\x98;\xe31\xca0\
 \x85\xc3\xc5\x99\xc4\x10\x19VF\x9a)a&\xce+#\
 \xd7\x12\xa9\x94-rm\x17k-\xdcJx!x\x19\
 \x19\xd8\x80}\xf2S\x11|Y\x96y\xbb\xfb_m\x7f\
-\xd0\x7f\xb0\xff\xa7\xc3\x01t\x01v\x01Z\x01y\xac\xbb\
-v\x8b\xd32\xb7W\x9c\xeb\xc5\xd5\x9b\xb5p\x15\x14\xf1\
-~\xc3\x8d\x12\xd1\x11\x8f\x05O\x95zUO}\x1d\xaf\
-Yc7\x9d}\x90po\xd4\x9a\xb9\x0d\xed~R \
-?\xe9O\xe57C\xbc\x22\x9e\x8d\xd2\x10\xef\x06\xefy\
-\xf0>(\x19\xed(\xdd(\x9d\xbd\x8e6\x9f=\xef\x90\
-\xfe\xc3\x09R\xa37\x84\x054\xaf^kr5\x97\xf6\
-\xb2\x1c\x01\xa5<\x80\xd2\x10A\xa9.(\xbd\x09JK\
-\x00\xa5\x9f\x22(\xb5\x09J\x87\x80\xd2\x1a@\xa9Y\x84\
-Tf\x9cq\xfc\xe4e\xc59P<\xe9\xec4\xc9A\
-\xe2\xe9v\x13\xbai\xfa\x81\xd3d\x83\xd3T-|\xad\
-\xa9\xe9\xfdv\xd3\x81D\xce\xf4[kVl[\xc8z\
-\xcf\x9e\xa3\x9f\xd4\xe7'\xfd\x1f?\xa9\xee'\xb5\x81\x91\
-\x0e\xfd\xa4!`\xa45~R\x9e\x1eO/E\xefy\
-z$z'z@\xbd\x9d\x9e\xcd\xe2j\x1b\xb7\xb6\x91\
-_\xab\xb6_Xk\x86\xac\xedY\xa9\xf9\xa6]Z>\
-\xf1=my\xf6\xae\xf7\xc9\xb5]\xd0B\x93\x1f\x04\x11\
-\xa3$\x1eIDI\x19\x88\x00I\xea\x91\xf4\x22\xa95\
-\x83-\xb6\xb7|Z\xb2\x92AH\xb8Z\xca\xf8\x1d\xb3\
-\xc5\x15\xa7\xa0\x8e\x5c\xd3\xbe\xf2[G#\x1e\x11\xef\x07\
-\xcf\x83\x92\x0b\xde\xd7fg\x0dN\x07R\xf9d\xfe\x81\
-\xd4\xff\x9b\xa9\xd9\xc0\x84\xc3$cIh\xe950y\
-`\xc2\xb1\xb4\x81\xa95\xb3k\x85\xdb\xae\xae\xb75\xd6\
-\xee\x05-[\xd6\x18\xd4\x8c-\xadM\xf6Y\x8f.\x15\
-\x02\xe7n\xf9\xd2F\x90]y\x95=\xb6\xbce\xf7\x1d\
-o\x9a\xe7\xae\xe5\xda\xe5\x96\xfc\x8a\xb1=\xf9\xc5=?\
-\x80\xab\x8f9\x07~\xeeO\xebZ/t\xbeu?\xeb\
-\xff\x0dP\xfa!(\xbd\x01\xa4#\xca\x01\xf2\x01J9\
-\x04\xa5=0\xb4\x8d\x91\x156F\x1eC\x90\xae\xc9k\
-q8\x5ck\xaf\xebq\xb2\xb3\xe2I\xd7\xe2\xe9u\x19\
-\x9etJ<\xf1x\xd1\xa4h\x07\x93/R\xf1\xa4\xb3\
-\xe2\x89\x87\xa7\xc9c\x18b\xa2\xfb\xf0\xa4u8Et\
-p\x8a\x8c\xc0)\xe2\x83S\x84@\x80\x00\xff\x1fn\x9a\
-rn\x9ah`hz\x1f\xa4M{\x9b\xc5\xfa\xf1o\
-k\xbe\xca\xc2R\xf5\xe2\x1d!\xbd\xfe\x13\xc5\xd0\x11\xe5\
-p\x80\x91\xf6\xe8zA\xbd?\xd1+\xb1\xe3\xa2\xa7\xd7\
-\xd3\x8b\xd1\xfb\x19=\x9d\xde\x8a\x95&\xbf\xfe u|\
-\xa0\xe6[\xb3\x7f\xfb:&\xb0\xb5\xf9_\xc5@l\x88\
-\xd8H\xfa\x9d5\xeei\xf5I\xfd\x1c[\x12[\xf3{\
-\xb5{\xfc\xef\xe6\xf3\x89!d\xbe\xb4\x13C\xf6\x89!\
-\xfdk\x84\x96<0\xe9\x10-\xcdX\xfa\xa0%\x1eK\
-95\x9640}\x8bK\xc2\xbf\x5c/om\xfds\
-\xb3\xef\xd9\x96\xa5fAM\x90\xdd\xe8\xe0dcG\x12\
-\x11/\x96\xec\x8e\x90\xc4\xb0\xd0\xd8jP\x14E\xb9\xed\
-\x04\xd0\x1d\x1fEd\x177D\xc4sq;s\xfa\xe5\
-o\xcf\x97\xbfz\x1c\x15\x15\xf10\xa8\xa8\xe5\x08\xa5\xbb\
-]\x8a\xa1g\x97~\x08\xa1\xb4h\x97\xda\x08\xa5C\xbb\
-\x14\xc8.\x9d\xb1\xeb7\xff\xd9m\x1bw\xb5<\xf5(\
-\x15\xa7\xcb\xb7\xbd\xbe\xfc\xaa\xb6\xb2\x7f\x00\x01\x85\x071\
-0\x00\x00\x00$\xc0Z\xf7\xdf\x96\xbf\x8a\xa7,\x99\xef\
-[~\xb2RPVK\xd6\xea\xa8\xed\x19Li\xa1f\
-*\xa0\xacYG~\xcb.\xbf5z\x19<\x81\x07S\
-P0\x85\xaf\x98\xa6\x18~(\xa8\x80EZ\x5c\xc7\x18\
-*<{\xed\xdc@\x18\x9a\xb9n\xcb[v\xad\x82\xc2\
-K\x8bg\xa5\xb5\xe3\xc5Y\xf2~`\xb7\xd8\x8e\x99f\
-\xb7\x19\x9af-o\xae\xa1\xc8\xfa\xc0\x14\x94>\xd6V\
-n\xbc\xdd\xce\xaa\xcd\xc4\xf5\xc9\x5c?\xb7u\xcd\x92v\
-kn\xef\xd6}\xb4\xfb\xba^\x00\x0aU\xc3\xf1U\x8b\
-g}y\xb6\x1d}\x11@\xd54\xae\xd7es\x95\xc1\
-\xb8\x96\xb1|+\x0c\x0a\x04w\x9da\xade(V\x01\
-\xf0S\x01S>\x91\xf5\xa9\x88\x1f\x18~ \xf8\xb1R\
-Z\xdc\xd6\xdc\x98\x8a\xd8\xea\xf8\xac4\xeb2u\xbfq\
-k\xcf\xdd[c\x8c\x85_\xd0\x18k\x06\x96\xc4\x9a\xd6\
-\xb2\xd8,+\xfaB\xa1\xb6\xc6z\xbc\xb6Y\x8b\xf7\xbb\
-\xad-\xbb\xa0P`\xd8\xb2u\xd3\xbar\x15\x9b\xfc\xba\
->\x03\x0a%F/\x9c<\xa0XbB\x87\xc4\xe8\x88\
-\x8e\x9cW\xb10\xb1\xc4E\x0a$>;\xa7\xa3\x9dS\
-\x07\x19N\x1bd8\xa5\xde\x06\x8f\x12\x10?\x9e\x98p\
-\xb1\xc4G\xd1\x11\x14\xd5<7\xbe\xdb\xf9\xb9\x92\xf9\x9c\
-\x05(\x06\xb0\x17\xb9Ze\xbd+>\xc7\xdbw5\xbf\
-\xeb\x98_\xe5\xea\x96\xa1\xd8\xd2%\x0cC\xfe0.,\
-\x03\xa1\x8d\xd7\xdd\x1f\xdf\x0a\xf3\x12\x9a\x15\xcb\xb0B1\
-,i0\x1f\xf6\x8ai(\xe3\xed\x9a_T\xe5%\x86\
-\xe4\xbbT.\x14\x18|\xe7\xa7\x85\xd4g]\xd6\x9c/\
-\xcbK\xb6\x02s\xbe\xe6x\xe5W]c;\xe6\xfa@\
-\x85\xae\xd0\x95\x98z\x1aM\xdf\xc6\xfb\x12ad\xe9\xb6\
-F\xde\x0b\x8f\xf2\xa3\xa5\xd1\xec\x93\x7f\x0bc\x15P9\
-\x9b\x83y\xb9\xe5\x8b\xcb\x1c\xffo\xd7\x91\xb4\xfc\xfc\x1c\
-\xce0\x15i\xc9\xd1\xee\xef:\xa7X\x06P\x96\x81\x8a\
-\xfe\x87\xfe\xf7\x9f\x8aL\xfd\x01N\xe3\xb5|{\xb7\xb1\
-/m\xe7\xb9X(#\xb3BCa\x01\xcd\xabe%\
-\x06\xc6\xe2B\xd3\x12\x03\x83\xc0\xfb\xa9g+(\xb8\xe6\
-[n+\xfblMX\xef\xe7\x8c\xcc\xa7\xde\xf5\xb6\xf5\
-\x84\x10\x0c\x07\xfc\x83\x95\x18\x98\x8bL\x06\xa6]\xb4\xf1\
-\xae\x88,\x91%\xb2P\x91\xa5\x22\xaa\x88*\x22\xaa\x22\
-\x86a\x18\x86h\x85\xc9\x17\x06\x15\x86!\x0a\x86\xa1(\
-\x8a/\xb2\x16\x11D\xc5\x10\x04\xc7\x0b\xa2 \x18\x86-\
-\x16\xab\xd4\xdb6\xea\xaca^\xb1\x07/\x9a\x17\x84W\
-\x83\x09\x14bVh^\xb1\x0842X\x0c\x0d\xccu\
-\xc1^\xdc[\xbb\xfb\xdfN\x07\xafZ\x8d\xdd\xfe\xd7G\
-kAo\xf3{\xb6{\x9fc\x83\xd1\xa8\x82\xa4R)\
-$\x22#\x22\x92$I:\xa2!\x04bi\x14J\x1d\
-\xb8\x1e\x12Q\x0cC2\x96\x81\x10C\x04\x1a!\x840\
-B\x04\x84\x08D$(9\x91\xa0 I\xdc\xd3\xa8\xd4\
-^p\x08\xac\x94\x9f q\xd3B\xb6\xce\xad\xdc\x90\x99\
-\xbeN\xe5\xe9y\xfc\xb0\x0fA\xc8\xd7C\x8c3\xe5L\
-\xcc\x0c\xad\x14t\x95\xba\x89\xdc|Y\x15R\xe9\xf9(\
-\xbc\xa8\xc1\xd3\xe3\xbf\x8e_}\x0b`j\xb1\x09'\xb1\
-\xa3\xcfy6\xd59\xf8\xe1a7\xd1\xb1Ft\x82F\
-\xac\x92N\x05\xf6\xa3o\x12\xd5\xca'\xe9\xaa=\x8c\xb2\
-\xe8\xea\xed\x00\xbc~\xc6\xce\x0a.\xa290h_\xf0\
-\x19\xc8d\x15\xf1\xaa\x02\x99\x895w\xd9}\x0aK\x0b\
-}u&\xdb~\x98\xea\xe9\xfdg\xd9u\xcd\xbe\x9bS\
-6\x12J\xe7\x1c'&\x85\x08\xbe\x12V\xc3\xed\x94\xe4\
-v\x0a\x942\xc0\xaa\xf1j\xfe\x17\x19\xe1:\xbf@4\
-\xf6\xbci\xbb\x0e_\xf1\x029Z\x8e\xab\x0f\xd8/\xb8\
-\xbes*\xe7\xb7\xc4%\x12y\x85i\x85\xb9\xd8+\x8b\
-\xe6h<\x90\xb2\xdc\xe8cbJY\x91\x0c\xd8f\xbe\
-\xafp\xf4\xd5\x07\xacs)\xf4\x11\x94\xc2m\x1b\x1fl\
-=\x09\xfb,\x00\xc8\xec\x86As\xca\xd2\x8f\x9c\xeb\x22\
-\x16\x8f/=\x181\xc5A/\x9f\x1b\x06\xff\xe0\x97\xa0\
-\x86\x02\x0c>\xd1\xce\xbe\x81\xc7\xdd'\x96gCm\xb6\
-\xbd\xb3\xee\xfdUL*\xe3\x15\xf7\xa8\x1a\xe7\x07\x19k\
-E,\xca\x00\x8f\x09nm\x04%\xf6~\xe8\xb9:\xed\
-\x10q\xa4\xd1S\x87mb1lD\xbb\xb04\xbf7\
-\x12\xad\xeb\xe8\x22\xd2\x9eY\x8aqWL\x17\xe6\xff!\
-\xd9?\x05\xedi\xef\xfeb\xef9\x89\x8a^2\xbc\xc7\
-l\xa1\x9a2,\x0e\x0a\xfc#\xa1\xa9\x93\x8b\xdaD\xe6\
-D!|RNHt\x8amn\x10p\xfa\x1d\x08t\
-\x9c &iIp1s\x12\xce\xd0mU\xff\xc6^\
-\x87'\xb3MOn\xafSoS\xd1\xc7\x7f\xa6d\x96\
-\xfbWU\x8f\x17#`g-%\xa9\x5cX.\xd4\xa1\
-[j\xc6\xf18\x1ay\xa3(\x8b5\x94<\xec\x90\x0a\
-\xe5\x1c\xb0\x06v5KWT\x89;4'\xb5\x8c\x94\
-\x84\xe3\x0b\xcf\xee/\xb5\xad!0\xd5d\x04\x91\x1d0\
-4\xa6\x95~\x91\xb3\xa1YM\x1fP\x1c'\xe07w\
-N&\x88\xa2\x10\x8bT7\xe0\xde\xd8\x00\xa4\x0f\xc5\x03\
-\xb4N\xc3\xf1\xee\xdb\xa3\x91\x90\xd1\xd1x\x91.\x977\
-\xe7\x09U\x09\xf5\x93i\x22\xee$\xe7\xb1ol\x8bW\
-{R1\x90\x90\x8c\xb2-l\x10:X*\xab\xe3\xcc\
-\xb5\xc0]\xed\xd9-f\x22\x8fM\xaf\xbb9\x00S\x1d\
-Y7!C\xa9\xac\x0b\x02^\x9e\x10\x93\xe9I\x91\xae\
-\xea-\xdd\x1b\x8e\x93\x05\xb5viTq\x8d\xf8\xde\xbd\
-N\x88\xf2(\x17\xddj\xbb\x84\xcfa\xc4\xd8]\x19\xe9\
-O\x92c\xa4\xe1\xf8\xca_%\x0d\xf24\xfc\x87\x10\x8a\
-O\xd1\x83\x9a\xaa[\x08\x1b\xe8\xeb\xd77[\xe2I\x8e\
-\xb6\xf4S?Lw\xdb\xb4~\xf3,\x10\x17\x1f\x80&\
-\xde\xcd\xfc\x16s\xa9\xa1yw\x93B\xf0\x99\x85\x93\x0e\
-\xb9\xadBO\xe0\x83u\x85M\x06\xb1\xb8\x98\xd1\xb6\xcb\
-\xfdA\x0d\xee\xc3n\xcc\xf3\xaaOM\xc4\xcb\x0aB3\
-!\x82\xed\x9b\xbb\x89\xab5\xc5\x13\x22\xef\x17\x1c1R\
-\x02\xb8\xc6\x95p\x8c\x81\xc1r\xc5@\x1c\x09;A7\
-\xe8\x8f\x8b\xb8\x18P\x97\x8a\xbc\xa9\x85\x91I\x80\x96e\
-f\xab\xa1\xc1\x16\x02\x87j\xc8\x1d\xd0\x07\x7f\xba\x14\xd3\
-K>\xcc\xdf\x043k\x1f\x93\x0fw \xbb0\xe5\xb9\
-Y\xab1\xe6\xf4\xa0b\xcd\x17u\xc7\xf5\x07\xd5\xb6\x08\
-\x93\xc3\x94\xd6a&)\xcb\xeaZF\x9f\x0d\x13W\xfd\
-\x9ctHpF=\x02\xfbr-\xf7c/\x8b\x15\x17\
-\x9d\xed\x14E/c\x87\x93\x93\x93\x22n\xd7\xbe\x96\xc1\
-\x07\xf3-7\xbe\x1e\x01%]'\x16\xca\x95wW\x1c\
-\xb1e\x94\x01\x01\xd3N\xd4|\xa3S\x17\x86\xa7G\x83\
-\x88\x11m5\xfbl\xf5\xb4\xed\x0e\xf7\x0a\x894pX\
-\xee\x18\x8f@1D\xd6V\xf8\xd4\xday\xf8BfG\
-\x5c\x22]\x89\x96\x99E\xc4\xef&\x88\x95\x9fMr\xd9\
-%\x969\xb9*\x8f1*\xfb\xf3\x89XF\xf8BC\
-a\xf9\xee\xc9rU\xccP\xf6\xe1\x09\xe4{!\xd1\xc9\
-\x9f\x82\xbe]%\xd2\xc8\xf8\xbc{\x99s!\x1fL\xb7\
-\xdc\xd8^\x16\x0c\xc8\x97\x0fD\xac\x85zH6\xd4\xee\
-\xc3\xc7\xa1\xfamL\xeb\x02Zo\x04\xd8\xf1\x05#8\
-\xa0\xb8\xa5m\xdcw\x87\xe9T\xe4uA\x04\xd7\xc6\x10\
-\xd4\x89a\xab\xd1\xba\xf7m\xa7\x1c\xf3\x9c5\x06\xb5\x06\
-\xb8\x88\x8b\xaa\x8f\x86w\x96\xf4\x19\xdc:c\xe6\xcd\xc5\
-f\x12\xc6\xc0\x0c\xed\xe0\xe6J\xcc\xa8d\x0a\x095u\
-\xbe\xc9\x84\xa3\xe9\x8c\x04\x00\x02\xb4\xed\x84{\x94\xe8L\
-\xc3\x85\x0d\x00}\xfc?\x0c\x85\x00\xa9\x83\x0a\xc3si\
-\x15\xc76 ,:C\xfe\xbb/\x10,\x18)\x19s\
-\xd2\xbe\xcap\xee\x81\x8e\xad\xcc\xd1\xa6\xd1vY\xc6\x92\
-4\xb1Z\xbe\xa7\xf0\xd2\x14;T\x03o\xa4\x10\x80\xc0\
-h\xf2\xb3\x14'\xea\xd9H1\xdcWpy\x0b\x10}\
-\xc67\x09\xf0\xcc\xc2SR*\x8d\xf9\xdf\xfcE\xe8[\
- \x0e2\xaa\xd2\x14\x80\x8b\x15\x88P\xcf\x846\x0b\x98\
-0 j\xc5*\x1d\xd82\x17\x1f\xd8*e\x17\x9f\xe4\
-\x5cq\xf0U\xd8\x8b\x9fV\xe6\xe9\xe6\x97$\x0a8\x82\
-\xe9 N\xb8N\x88\x85dV\xfe\x03\xe1\x99`A\xa1\
-a\xfb\xfc\xbc\xcaN\x18\x8bK\xf0=DD\xac\x0b\xf0\
-f6A\xec\xbf\x90e2\xba;\xeb\xdc\x09e\xbb\xee\
-\xb1\xb0%&\x94!\x0b!\xf8\xea\x16\xd0\x12rBX\
-'\x8a\xaf\x89\x0a\x89\x1e\xb35\xa4.I~\x00R\xbf\
-\xc7\xcd\xa9\x0a\x22m\x93,\xd0\x92D(tQ\xe7\xcc\
-AZ\x05B-\x07\xd5~\x15\x08\xec\xbe\x99\x19>x\
-l(bl\xd2rS@8[ \x0e\xce\xd9B$\
-\x849\xb8f\xf2\xdc\xf2g\xde\x5cH,\xfb.\x06\x86\
-D\x10\xb3\x8e\xeb\xc5\xff%\x11l\xdd\xc58\x1dN$\
->\xb2A\x01\xb3\x1f]Wa\x09\xa2\x98\x0c\xf9\x80:\
-\x0a\xc7\x0a5H\xaa?E\xb8D\x82\x16\xf6E\xd4\x96\
-\x9b\xb9\xdd\x0a\xcf/\xef\x1cP\xf3\xf0\xe4a\xb3ZJ\
-\x98\x00\xb9\x0e\xa6\xf2@\x91\xa0U\xf2\xb7\xe6|\x89\xbc\
-]<\x06\xe3\xec\xcb\x07D\x80Q,\xb1\xa3\xc4O\x0f\
-I\x07D6\xd9\x5c\xce\x02\xb5\xc1A\xcf\x0bV.\xac\
-\xfa\xa6\xc3`*P\xbcL;\x0chg\x96Hl\xe4\
-#pC\xc12@\xda\x16\x14t\xaf\xa1\xc0\xa8\xf1@\
-\x03t\xc3\x03|\x5c\xe4\x93\x8b`\xb0\xe4\x9b>\xb0y\
-5\x1aP\xef\xa3\x13\xff\x07\xa3\xcc\xee\xff\xa2H\xc0\x85\
-\xe1\xfb\x88\x95\xf9|\xbf\xbbA`\xf7\xf1XH\x08\xe6\
-\x0a\xa7\x02\x82\x97\xd8\xbcE\xb4/\xe6\xa5\xa7\xb2xk\
-\x92\xed\xd0\xfe4\xcd\x01\xa1\xedj\x96p\xc5\xaa\xedb\
-\xdf\xa5\xf3E`\xb3\x82\xe8\x00\x91\x08X\xf0\x88_\xc3\
-v\xd2e\xd9\xc0Q\x04\x1f\x97\x8e\xb7\xac\xb3I\x97\x5c\
-\x16\x8e\xce\xaa\xa5b3+\x0b\x172\x0a\xfc\x04&\xce\
-a\xd0\xab2\xe7\x0e\xb9\x0dO\xe6\xf4\xc6\xb4K\xc5\xa3\
-\x06\xdb\xcav\xf9_\x87n\xaa\xd6\xdd\xee\xca\x95\xdc\xa5\
-[c\xec\x89~\x18\x83\x9e3\xbd\xd5\x11wN2\x05\
-d\xe7\xd9\x18\xe3\xd8\xabdk\xd5\xc823:\xe2\xcc\
-2&.@\xb1\xee\xc5\x93C\x88q\x8e\xea\xc9\xb5\xad\
-Pf<'\x8d\xe6\xdc\xa7Y5\xfd\xaa`a\xdb\x08\
-\x85~\x00xn\x08\x10\xc6\xcf\xb6\xce\x88\xeeYg\xd4\
-\xc9\x9f\xbe\x9e\x95\xcc\xec\x80\x22z(pN\x1ah\xa6\
-\xb7\xe5\x17\x12\x98\x13\xd8l\x14\xbf!\xaa\xb3\xeb\xb2\x0f\
-\xafWX\x04\xd5#DX\xb1\x94\xcekz\xe4\x98J\
-\xa4\x16\xa6\x880K\xc6g\x9d\xe7\x00\x9f\xe1+\x14\x0b\
-N\xc7\x11\xeaf\xce\xf714\xd1Q\x1d\xad\x86\xc3w\
-e\x94\xf8\x0d-\x0e\x98\x22\x10\x10\x8a\x0bJ\x1d\x13\x87\
-\xbf\xac\xa830\xc8)4[\xf8\x85\x89\xb15\xc3\x17\
-\x18\x9c\x8d'\xa6\x88\x04\xd9\x13\xc5\x094\x09/u\xf1\
-\xa6|\xbc7{\xac\xe6Yx\xa4-\x85i*%\x89\
-\xb0\xa3\x08e\xde\xd8\xf2BqA\xb6;\xc7`\x22\x98\
-\xc0H\xe0\xbcT\x06\x11e+8^\xd4}\x0cH\xe4\
-\xe0\x8c\x88\xaf\xdf\xcev\x11\xe4\xe8\x10e4\xadF\x85\
-\xaf#vaJPn5\xd5Wa\x06\xdctFR\
-\x06\x975\xd7\xf5\xc0\x91M:y\x90\xae\x1f!S\xeb\
-\xad\xc7!\x00A\x9de\xd6fpeR\x9a\x9c3\x1c\
-\x9d\x0d\x87\
+\xd0\x7f\xb0\xff\xa7\xc3\x01u\x01x\x01[\x01\xfd\xe6\xb1\
+\xee\xda-N\xcb\xdc^q\xae\x17Wo\xd6\xc2UP\
+\xc4\xfb\x0d7JDG<\x16<U\xeaU=\xf5u\
+\xbcf\x8d\xddt\xf6A\xc2\xbdQk\xe66\xb4\xfbI\
+\x81\xfc\xa4?\x95\xdf\x0c\xf1\x8ax6JC\xbc\x1b\xbc\
+\xe7\xc1\xfb\xa0d\xb4\xa3t\xa3t\xf6:\xda|\xf6\xbc\
+C\xfa\x0f'H\x8d\xde\x10\x16\xd0\xbcz\xad\xc9\xd5\x5c\
+\xda\xcbr\x04\x94\xf2\x00JC\x04\xa5\xba\xa0\xf4&(\
+-\x01\x94~\x8a\xa0\xd4&(\x1d\x02Jk\x00\xa5f\
+\x11R\x99q\xc6\xf1\x93\x97\x15\xe7@\xf1\xa4\xb3\xd3$\
+\x07\x89\xa7\xdbM\xe8\xa6\xe9\x07N\x93\x0dNS\xb5\xf0\
+\xb5\xa6\xa6\xf7\xdbM\x07\x129\xd3o\xadY\xb1m!\
+\xeb={\x8e~R\x9f\x9f\xf4\x7f\xfc\xa4\xba\x9f\xd4\x06\
+F:\xf4\x93\x86\x80\x91\xd6\xf8Iyz<\xbd\x14\xbd\
+\xe7\xe9\x91\xe8\x9d\xe8\x01\xf5vz6\x8b\xabm\xdc\xda\
+F~\xad\xda~a\xad\x19\xb2\xb6g\xa5\xe6\x9bvi\
+\xf9\xc4\xf7\xb4\xe5\xd9\xbb\xde'\xd7vA\x0bM~\x10\
+D\x8c\x92x$\x11%e \x02$\xa9G\xd2\x8b\xa4\
+\xd6\x0c\xb6\xd8\xde\xf2i\xc9J\x06!\xe1j)\xe3w\
+\xcc\x16W\x9c\x82:rM\xfb\xcao\x1d\x8dxD\xbc\
+\x1f<\x0fJ.x_\x9b\x9d58\x1dH\xe5\x93\xf9\
+\x07R\xffo\xa6f\x03\x13\x0e\x93\x8c%\xa1\xa5\xd7\xc0\
+\xe4\x81\x09\xc7\xd2\x06\xa6\xd6\xcc\xae\x15n\xbb\xba\xde\xd6\
+X\xbb\x17\xb4lYcP3\xb6\xb46\xd9g=\xba\
+T\x08d>g\xe7n\xf9\xd2F\x90]y\x95=\xb6\
+\xbce\xf7\x1do\x9a\xe7\xae\xe5\xda\xe5\x96\xfc\x8a\xb1=\
+\xf9\xc5=?\x80\xab\x8f9\x07~\xeeO\xebZ/t\
+\xbeu?\xeb\xff\x0dP\xfa!(\xbd\x01\xa4#\xca\x01\
+\xf2\x01J9\x04\xa5=0\xb4\x8d\x91\x156F\x1eC\
+\x90\xae\xc9kq8\x5ck\xaf\xebq\xb2\xb3\xe2I\xd7\
+\xe2\xe9u\x19\x9etJ<\xf1x\xd1\xa4h\x07\x93/\
+R\xf1\xa4\xb3\xe2\x89\x87\xa7\xc9c\x18b\xa2\xfb\xf0\xa4\
+u8Etp\x8a\x8c\xc0)\xe2\x83S\x84@\x80\x00\
+\xff\x1fn\x9arn\x9ah`hz\x1f\xa4M{\x9b\
+\xc5\xfa\xf1ok\xbe\xca\xc2R\xf5\xe2\x1d!\xbd\xfe\x13\
+\xc5\xd0\x11\xe5p\x80\x91\xf6\xe8zA\xbd?\xd1+\xb1\
+\xe3\xa2\xa7\xd7\xd3\x8b\xd1\xfb\x19=\x9d\xde\x8a\x95&\xbf\
+\xfe u|\xa0\xe6[\xb3\x7f\xfb:&\xb0\xb5\xf9_\
+\xc5@l\x88\xd8H\xfa\x9d5\xeei\xf5I\xfd\x1c[\
+\x12[\xf3{\xb5{\xfc\xef\xe6\xf3\x89!d\xbe\xb4\x13\
+C\xf6\x89!\xfdk\x84\x96<0\xe9\x10-\xcdX\xfa\
+\xa0%\x1eK95\x9640}\x8bK\xc2\xbf\x5c/\
+om\xfds\xb3\xef\xd9\x96\xa5fAM\x90\xdd\xe8\xe0\
+dcG\x12\x11/\x96\xec\x8e\x90\xc4\xb0\xd0\xd8jP\
+\x14E\xb9\xed\x04\xd0\x1d\x1fEd\x177D\xc4sq\
+;s\xfa\xe5o\xcf\x97\xbfz\x1c\x15\x15\xf10\xa8\xa8\
+\xe5\x08\xa5\xbb]\x8a\xa1g\x97~\x08\xa1\xb4h\x97\xda\
+\x08\xa5C\xbb\x14\xc8.\x9d\xb1\x0b\xe7\xf8\x9f\xdd\xb6q\
+W\xcbS\x8fRq\xba|\xdb\xeb\xcb\xafj+\xfb\x07\
+\x10Px\x10\x03\x03\x00\x00@\x02\xacu\xffm\xf9\xab\
+x\xca\x92\xf9\xbe\xe5'+\x05e\xb5d\xad\x8e\xda\x9e\
+\xc1\x94\x16j\xa6\x02\xca\x9au\xe4\xb7\xec\xf2[\xa3\x97\
+\xc1\x13x0\x05\x05S\xf8\x8ai\x8a\xe1\x87\x82\x0aX\
+\xa4\xc5u\x8c\xa1\xce^;7\x10\x86f\xae\xdb\xf2\x96\
+]\xab\xa0\xf0\xd2\xe2Yi\xedxq\x96\xbc\x1f\xd8-\
+\xb6c\xa6\xd9m\x86\xa6Y\xcb\x9bk(\xb2>0\x05\
+\xa5\x8f\xb5\x85B\xe50\xae\xe3\xedvVm&\xaeO\
+\xe6\xfa\xb9\xadk\x96\xb4[s{\xb7\xee\xa3\xdd\xd7\xf5\
+\x02P\xa8\x1a\x8e\xafZ<\xeb\xcb\xb3\xed\xe8\x8b\x00\xaa\
+\xa6q\xbd.\x9b\xab\x0c\xc6\xb5\x8c\xe5[aP \xb8\
+\xeb\x0ck-C\xb1\x0a\x80\x9f\x0a\x98\xf2\x89\xacOE\
+\xfc\xc0\xf0\x03\xc1\x8f\x95\xd2\xe2\xb6\xe6\xc6T\xc4V\xc7\
+g\xa5Y\x97\xa9\xfb\x8d[{\xee\xde\x1ac,\xfc\x82\
+\xc6X3\xb0$\xd6\xb4\x96\xc5fY\xd1\x17\x0a\xb55\
+\xd6\xe3\xb5\xcdZ\xbc\xdfmm\xd9\x05\x85\x02\xc3\x96\xad\
+\x9b\xd6\x95\xab\xd8\xe4\xd7\xf5\x19P(1z\xe1\xe4\x01\
+\xc5\x12\x13:$FGt\xe4\xbc\x8a\x85\x89%.R\
+ \xf1\xd99\x1d\xed\x9c:\xc8p\xda \xc3)\xf56\
+x\x94\x80\xf8\xf1\xc4\x84\x8b%>\x8a\x8e\xa0\xa8\xe6\xb9\
+\xf1\xdd\xce\xcf5(\x06\xb0\x17\xb9Ze\xbd+>\xc7\
+\xdbw5\xbf\xeb\x98_\xe5\xea\x96\xa1\xd8\xd2\x05\x0c\xc3\
+\x90?\x8c\x0b\xcb@h\xe3u\xf7\xc7\xb7\xc2\xbc\x84f\
+\xc52\xacP\x0cK\x1a\xcc\x87\xbdb\x1a\xcax\xbb\xe6\
+\x17Uy\x89!\xf9.\x95\x0b\x05\x06\xdf\xf9i!\xf5\
+Y\x975\xe7\xcb\xf2\x92\xad\xc0\x9c\xaf9^\xf9U\xd7\
+\xd8\x8e\xb9>P\xa1+t%\xa6\x9eF\xd3\xb7\xf1\xbe\
+D\x18Y\xba\xad\x91\xf7\xc2\xa3\xfchi4\xfb\xe4\xdf\
+\xc2X\x05T\xce\xe6`^n\xf9\xe22\xc7\xff\xdbu\
+$-??\x873LEZr\xb4\xfb\xbb\xce)\x96\
+\x01\x94e\xa0\xa2\xff\xa1\xff\xfd\xa7\x22S\x7f\x80\xd3x\
+-\xdf\xdem\xecK\xdby.\x16\xca\xc8\xac\xd0PX\
+@\xf3jY\x89\x81\xb1\xb8\xd0\xb4\xc4\xc0 \xf0~\xea\
+\xd9\x0a\x0a\xae\xf9\x96\xdb\xca>[\x13\xd6\xfb9#\xf3\
+\xa9w\xbdm=!4M0\x1c\xf0\x0fVb`.\
+2\x19\x98v\xd1\xc6\xbb\x22\xb2D\x96\xc8BE\x96\x8a\
+\xa8\x22\xaa\x88\xa8\x8a\x18\x86a\x18\xa2\x15&_\x18T\
+\x18\x86(\x18\x86\xa2(\xbe\xc8ZD\x10\x15C\x10\x1c\
+/\x88\x82`\x18\xb6X\xacRo\xdb\xa8\xb3\x86y\xc5\
+\x1e\xbch^\x10^\x0d&P\x88Y\xa1y\xc5\x22\xd0\
+\xc8`140\xd7\x05{qo\xed\xee\x7f;\x1d\xbc\
+j5v\xfb_\x1f\xad\x05\xbd\xcd\xef\xd9\xee\x1d\x83\xcf\
+\xa8\x82\xa4R)$\x22#\x22\x92$I:\xa2!\x04\
+bi\x14J\x1d\xb8\x1e\x12Q\x0c\xe31\x96\x81\x10C\
+\x04\x9c!\x840B\x04\x84\x102\x12\x88\xa0H\x90 \
+I\xf4\xd3\xa8\xbeP\xfd`\x9c\x82\x9f\xa0tS\x81l\
+\xdd\xae\xdc\x10\x99\xbe\xe7\xf3\x94\x1e\x7f\xeeC\x0e\xf9J\
+\x88\xc1\x99r\xc6g\x86\x16\x0a\xbaB\xdd$o\xbe\xa2\
+\x09\xa9ld\x0e[\x94\xe2\xe9\xcf\xafC\xef\xdfB0\
+\xf5C\x85{\xb1\x03\xe6<\x9b\x8es\xf0\x83\xc3>\xa2\
+\x03\x8d(\x80F\xcc%=\x00\x92\xac\x16i\xe1s\xd6\
+\xaa4\x9bb\xccE\xe8\x02\xefc\x83\x0c\x04\x17k\x0d\
+t\xdb\x0b|F=^-x\xf5@eb\x83\xbb\xac\
+3\x85EJx\xd5&\xdb\xf10e\xf6\xf2\xb3,\xb9\
+f\xdf\xcd)\x1b\xc9\xa4p\x8e?\x91&\x82\x07\x09\xd7\
+p\x1b%j;\x85\xa0\x0cH5^\x9d\xf9\x22\x0a.\
+\xf5KGc\x9b\x916\xc7B\x1b\x1e%G\xfdx\xbb\
+\x01K\x01W\xe5^\xe5\x0c2b\x89\x95\xbcv\xb4\x98\
+\x5c\xf4\xca\xa2s42$\x137\xee\x98\x08\xa5\x06%\
+\x036\xb0\xef+\xbcr\xf5Av.\x85>\x06R\xb8\
+m\xe3C\xd63a\x9f\x0d\x00\xccn\x184\xa7\x1e\xfd\
+H\x90\xfeb1y)\xcd\x88\x11\x0ez\xf9\xdc0\xf8\
+\xc7\xbe\x04\x05\x0ad\xf0Y:\xfb\x03\x1el\xb4S\x0d\
+\x97j\xb7\x8d;\x0b\xb2X\x91\xa4J^\x02\x8fv\xe0\
+D!\x81\xd6\xea\x8b\x02\xf0 \xf1\xd6\x8eR\x22\xee\x87\
+\x06\xab\xd3\xae\x11Gb\x15\x14\xb2\xcd(\x07\x14Q\x12\
+\x16\xea\xf7.\xd1\xba\x8e.\x22\xed\x8dE\x18w\xf2t\
+\xa1\xfd\xefd\xffI\xd0\x9e\xf6\xee\x0f\xbb\x9fSW\xdc\
+\x92\xfb=\xd6\x0b\xd5\xcb0\xc8A\x91#R\xcc\xcds\
+Q\x81\x14\x0c(TOJ\x08\x89\xeeM\xca\x1aV8\
+\xc5\x06B\xf7\xbc $\xf1\x08\xeee\xae\x983\xb4@\
+\xd5\xa7\xb1\xd7\xee\xc9\xcc\xd3\x13\xc0\xeb\xd4\x88\x84\xf5\xf1\
+7(\x99\x99\xfd{\xd5\xd3\xc58\xb0/\x16!\xa96\
+\xcc.4\xa0[R\xc6\xf5qdy#Z\x8c5\x94\
+$\xa6H\xeds\x0ef\x05\xbb\xc7\xd2\x15UJ\x0f\xcd\
+I\xad\xc4\x80\x84\xcb\x8d\x87NZjYC4Z\x93\
+\x0e\x22W`\xa8L\xf3\xfc\x22AC\x86\x9a>T\x1c\
+\xc7\xe17oNJ\x89\xa2x\x8bT\xcf\xe0\xde(\x01\
+\x18\x1a\x8a\x01h\x05\x86\xe3]\xde\xa3.!\x03\xd0x\
+\xd1/\x97w\xe7\x89\xab\x12`'\x13D\x5c@\xce\xcb\
+nl\x8bW{R1t\x90\x8cR\xadlPu\xb0\
+\x94Q\x97\x9ck\xc1\xba\xfagw\x87\x8996\xbd\xee\
+\xe6\x08L\xb5\xb2\xaejV\xa9\x8c\x17\x04\xfc\x9c\x10\x13\
+\xe8I)]\xd7[\xb178g\x06\xb5vQTe\
+\x8d\xf8\xfe\xbdn\x88\xf4(\x17\xdd\xd5\x16\x09\xcfa$\
+\xd8]A\xd2\x9f'\xc7H\xc4\xf1\xb5\xbfJ\x1d\xe4\xe9\
+\xf7\x0f!\x1b\x9f\xa2\x075B\xb7x7P\xee\xd7k\
+[bJ\x8e\xa3\xf4\xd3\x02Lw\xdbt\x7fs,\x10\
+\x11\x07\x80F\xda\xcd\xcc\x8b\xb9T\xd7\xbc{\x92B0\
+\xcd\x8c\x93\x01\xb9\x15B\x0f\xe0\x15\xeb\x0e\x9b\xa8\x89\x05\
+bF\xd8\xae\xfb\x83\xea\xde\x87\x8d\xd8\xe7U\xdf\x9a\x8c\
+\x97\x15\x9efB\x90\xed\x9bA\x13wj\x8a'D\xde\
+/8b\xa4\x04p\x8d+\xe1\x18\x03\x8b\xe5\xca\xa0\x1c\
+\x89+A7\xf4\xc7\x8b8\x89P\x97\x8a\xbc\xd5\xc2\x98\
+I\xd4\x96el\xab\xc1\xc0\x96\x02\x87j\xc8\x1d\xa0\x06\
+\x7fv)\xaa\x97\x1c\xcc\xaf\x073e\x1f\x93\x84; \
+{`J\xda\x99\xd4\x18\xe2\xf4\xa2b+\x8b:\xc6U\
+\x06\xd5\xb7\xc8\x87\x1c\xa6\xd4\x820V\xd42\xf7\xd9\x18\
+}i\xcei\x0e\xc9\xf7\xdb#\xab\xc9\xab\x9c\xf4\xf7\xc2\
+2r\xf5l\x07&@\x84\x9d\x03\x8e\x04GqQS\
+\xac\x0cd\x98\xef\xa5qF\x04`t\xf5\xb0\x80\xa9\xbc\
+-\xc6\xd1CFI \xe0\xa4\x89*st\x0a\x01\xea\
+i:\x04c}[1>C:m\x83\xc3] \xc5\
+\x06\x0e\xcb\xbd\x91\x0e\xb0!\xb2h\x85J\xad=\x87o\
+3\xfb\xe0\x92\xef\x0a\xb6\xe6\xac%~7a\xb1\xda\xad\
+d,\xb8D3\x91\xab\xfc\x18\x8b\xb2\xff\x9f\xc8e\x84\
+/4\x140\x9f%Y_\x0fs\x94>\xdc\x81\xdc_\
+\x18t\xffSp\xb7\xeb\x8b$26\xef\x12\xe6\xfc\xcd\
+\x07\xd1\xed6\xb6\xcc\x82\xa1z\xfc\xa8\xc5Z\xa8\x87d\
+C\xe3>\xdc\x0e\xedoO[\x17\xd0z# \x8e\x09\
+\x18\xc1\x0f\xc5-m\xe3\xbe;L\xa7\x22\xaf\x0b\x22x\
+m\x80\xa0F\x0c[\x89\xd6Q\xdf\x06\xca1\xcfYc\
+Pk\x80\x0bw\x91\xf0Q\xf2\xceH\x9f\xd9\xad3d\
+\xde\xfci&a\x10\x18\xa0\x13\xdct\x89\x1b\x95` \
+\xa1\xb3\xce\xcf\x99\xb0\x84\xd6\x98\x07A\x96`;\xe5\x8e\
+\xeat\xb8Aa\x0b@<\xfe\x1f\xc6E\x00\xf9A\xb9\
+\xe1\xba\xd4\xc5\xb1\x1b\x1e\x96\x9d7\x7f\xb8\xae\x08|<\
+B\x1a\xe6\x0c\xfb+\xc2Y\x0f!\xd6\xca\x00m\xcam\
+\x15f\xacJs\xab\xca\x17\x14^\x1ab\x87j\xa0\x0d\
+T\x13\x08tdz\x12\xa2\x84<\x03i\x0e\x9d\x15\xcc\
+\xde\x02D\x9f\x11M\x7f\x12M\xd8:*\xe9T\xee7\
+\xbe(q\x8b\x8c\x86\x8c\xaah\x0f@\xc6\x0aF\xa8=\
+Q\x9b\x0f\x5c\x18\x10\x99b\x95\x0el\x85\x8b\x1bl\x91\
+2\x95\x9f\xe2Bq\xe2U\xb8\x177\xad\xc4\xd2\xdd\x17\
+%*\xd0\x04\xd9A\x9cp\x9d\x10\x0b\xc9Ry\x06\xc2\
+7\xc1\x92B\x93\x0d\xf3\xf3*;a,.\xc1\xfd!\
+\x0ab*\xc4[\xd7\x04`\xbc\x84\x84\xc9\xea.\xaes\
+\xc5B\xa1\xc6D!\xc9\x02?\xbe3O\x0a~N\x08\
+\xeb\x84\xf9\x9a\xa8\x98\xe86[\x13u\x95\xb4\x07\x0d\xf5\
+8VNW\x10\xd9\xf6\xc9\x0a\x96d\xad\xaa\x8b\x9c3\
+\x87k\x15\x1c\xb5\xdc\xa8\xf6\x93@`\xf5\xcd|\xf8\xe0\
+\x11\xa4\x881I\xcbo\x01\xfdl\x81?8G\x0b\x91\
+\x1e\xe6\x18\x9b\xc9\xa7\xe5\xf7\xbc\xa9\x90\xd8\xf7]\x0c\x8c\
+D\xb0\xb3.\xebe\xfd%#\xd8\xb4\x8b)\x1dU$\
+>\x92A\xa1\xb3\x1f\xbd\xab\xba\x04\xb9M\x860\xa0\xce\
+\x85c@\x0d\xa6\xebOy\x5c\xe2\xa1\x85\xf5\xa2`K\
+\xcf\x00n\x85A\x97\xb7\x1dS\x99\xf0d`3QJ\
+h\x00\xb9\xc2\xa6rW\x91\xe0Tro\xcd\x07\x12\x19\
+\xb9\x14\x06\xa3\xec\x8b\x07D\x80Ql\xb1\xa3\xc6O/\
+$\x1d\xb0l\xbe9:\x0b\xd4\x06\x07=/Xr\xe1\
+\xeb\x99\x0e\xe9T\xa0}\x93vx\xd0\x8e,\x91\xdb\xc8\
+N\xe0\x06\x86\x9d\x80\xb4!(P\xae\xa1\x8a\x91\xf0@\
+\x03\x8c\x86G\xf3\xb8\xc9'\x16\xc1b\xc97}`\xf3\
+\x0a5\xa0\xecG'\xffW\xa3\x9c\xdd\xbf\xa3\xc8\xc1\x85\
+\xf1}\xec\xca\xf9|\xb7\xb8A\x00\xfbx\x1cH8\xe3\
+B\xa7\x82\x82\x17\xd9\xbcI\xb4)\xe6\xe5\xa6_\xbc\x05\
+\xc8vb\x7f\x9b\xf6\x80\xda\xf65K6\xc4\xaa\x9db\
+\xdf\xa5\xf3En\xb3\x82\xe8\x00\x91\x08X\xf0\x88_\xc3\
+v\xd2e\xd9\xe2(\x1c\x1f_\xc7GW\xd8D%\xd7\
+\x8a\xa3\x8f\xea\xa8\xd8\xcc\xca2\x84\xec\x02?\x81\x89s\
+\xf8\xf4\xaa\xc8\xf9!\xb7\xeb\xc9\x99\xde\x9bv\xbexh\
+\xb0\xcd\xd9>\xbf\xea\x90B\xd5\xba\xdbA\xb9\x92\xbbt\
+0\xc6\x9b\xe8\x831\xe89\xd3+\x1cx\xe7$S!\
+[\xcf\x062\x8e]%;\xab\xe6\x96Y\xd2\x11m\x96\
+\x11q\x09\x14\xbb]<\x13\x84&\xceM\x1d\x5c\xd7\x0a\
+E\xc6S\xd6(\xd0}\x02U\xd3\x89\x0a\xd6\xb7\x8d\x10\
+\xea\x07\x90\xe7J\x80\xd0~\xb6}FD\x9eu\xa0\xd2\
+\xfet\xf9\xacdf\x07\x14\xd1S\x81}\xd2\x84fn\
+[^!\x019\x01\xcd\x06\xf1\x1bW\x9du\x97\xfd\xf1\
+\xfa\x87ED=\x04\xc2\x8a\xa5t^\xd3#\xc7T\x22\
+\xf53E\x83Y9>\xeb<\x07\xf8\x0c_\xa1X\xe0\
+t\x8fPg\xe6|\x1e\xc3\x13\x1d\xd2\xd1\xea8|W\
+F\x89\xdf\xd0\x1a\x80\x19\x02\x81\xa3\xb8p\xd71m\xf8\
+c\x15E\x01\x06-\x9f6\x17~`\xa2l\xcd\xfc\x05\
+\x04g\xeb\x89\xf1\x22\x09\xbb\xad8\xae&\xb1\xa5\xfe\xbd\
+)\x0c\xef\xcd\x1d\xab\x00\x16\xee\xd2\x96a\x15\x95\x12#\
+\xd7Q\x842ok\xfcB\x09A\xe6;g\xb0\x17\x8c\
+k$X^>\x83\x89\xb2\x05\x1c)\xea\x0e\x06D\xe4\
+\xee\x8c\x88\xa7\xdf\xce\xef\x22\xeeh:e\x1c\xadF\x8f\
+\xbbc\xec\xe2\x94`\x9cl\xaa\xb6\xc2t\xb9\xe9\x86\xe4\
+\x0f.;]7\x0276\xe9\xe4A\xba~\x84j\xad\
+\x9f\x1e\x17\x00\x9c\xba\x99\x99\xcd`\xc9\xa449\xffp\
+\x144\x1c\x02\
 \x00\x00\x02%\
 <\
 ?xml version=\x221.\
 0\x22 encoding=\x22UTF\
 -8\x22?>\x0a<svg viewB\
 ox=\x220 0 16 16\x22 v\
 ersion=\x221.1\x22 xml\
@@ -3611,223 +3611,223 @@
  color-interpola\
 tion=\x22sRGB\x22 text\
 -rendering=\x22auto\
 \x22 fill=\x22#8542c2\x22\
  shape-rendering\
 =\x22auto\x22/>\x0a</svg>\
 \x0a\
-\x00\x00\x0c\xec\
+\x00\x00\x0c\xea\
 (\
-\xb5/\xfd`XJ\x15g\x00Zd<\x15G\xb0\x98\
+\xb5/\xfd`XJ\x05g\x00\xdac$\x15G\xb0\x98\
 Q\x07\x90\xdd\x9b\xb9o\x0fl\x05'^\xe0DZ\xc0\
 $\x22\x87\xa5\xa0\x9a\xf0!C\xb5f\x13/\xba\x15d\
 K\xa5\xd9R\xae\xc4Rb\xd3v\x12\x96\xc6/\xa36\
 \x95pC_\xe2\x03a\xd3p\xc38\x06'\xfcS\xfa\
-\xd3\xa8\xfd\x18\x07M\x01X\x01,\x01\xd63\x15\xb3P\
-\xd2\xb6\x07\xe8\xad\xb4w\x1bj\xdc\x96\xc0\xc6\xa2\xa6\x96\
-\x08\x12\x0dI\x5cD\x92\x9d$:\x90\xd8\xcf\x17\xdf~\
-F\x1d\xc4\xda>h_\xf4M?\x7f\x8e\xe2Q\x82\xa4\
-\xa3\xe5\x5c\xa0#\xe0\xad3\xa0#\x19\xe8\xc8\xf6\x1cJ\
- \x96|\x96zz(\xd9Pr\x22% J\x1ep\
-(qX\xda\xb0\xe42-\x09\xeej\xd1\xf8\xd7\xb6\xe3\
-r\xf6\xfd0\xc41\xa7\x091\x122\xa2\x14!=q\
-\x9b\x18YM\x87$IR\xff&@\xd6\x9bm\xac\xfb\
-V\xed\x12\xa2;\xd2ehA\x1b\x91\xa3<**w\
-r\x94FE%\x91\xa2\xd2F\xd1\xfeh\xa6\xfbo\xf8\
-\xa6nj/\xad7j{\x0bU\x01\x87\x1d%F:\
-\x1e%=t;tH\xba\x17:\x96\x15\xa7_\x15)\
-\xcc\x86oP\x92\x04\x16\x8eM\xf7\x14\xd1\xc1\x19\xc2\x02\
-\xd9\x16q,\x88\xca\x1d\xa2\xd2h\xa8\xc41D\xc5k\
-\xefm[l\xa3\x16\xa8\x8e\x8e~\x90V!BeN\
-\xa8\xdc\x99Q\x1a\x09\x95#f\x948\x84\xca\x9f\x1d\x8a\
-\x1d\xd0nhWbW\xb34\xfa\xbb\xbeX8 -\
-\xd7\xd9\xb8_\xe3\x052\xb2k\xff)\xa8\xebw\xdf\xd2\
-\x9b\x02\xaa+\xfdh98:\x1b\x96@,\xf1P\xe2\
-\xb0\xc4\xc2\xc9\xb4\xc2\xeb\xfc\xe7\x05\xac\x0f\xa9\xcd\x09\xe7\
-\xc3\xaf\xc5\xfc\xe2o\xa6B\xfa\xc7\xbcY\x1f,Fc\
-\xc0\xd6b\x06\x0fZ<c\xbd\x15CJ\xbaN\xa7\x8c\
--\xfej\x8d\xa5w\xcd_\xbb3\xa7\x937Y\xb5-\
-~\x0bG\xad\xa8k\xcb5\xac\x802D\x06\x13\x88\x15\
-QT\xe4\x9e\x0cq\xe2\xc3\x83\xb3\xbcP\x11%\x06\x8b\
-'AELHEL\x1fj0q\xa8\xc1\xb4\xa2\xe3\
-\x07\x8a\x08!UT\xc4\x88\x12\xe4\xc8\x09I\xd6\xdb\xcf\
-\x11\xd2\x0e\x94_\x0a\xde1g\xcc2\x1e\xea(\x92\xa9\
-\xa61\xb7\xaf\xb3\x8f$\x99\xbc\x7f\xe8\x8ct.\x8ac\
-\xa6]Z\xd5\xd6\xfe\xa8\xeb\xcd\xf5\x81\x1b\xbdY\xad\xc7\
-\x8c\xc2\x98n\x8aa\xeb\x8c\xf7H\xddy\x86\xca\x10D\
-\xe5\x8e\xa1\x5c\x8f\xa1\xa1\xa0\xa1\xb2\x03Qyb\xc6\xbd\
-\x19\xef0q\xb1\xc3\xc43\x14\xd9\x18\xac\x7f\xbbYJ\
-\xa3\xe2\xb6\xb9\x13TJ\xb8h\xca\xc1h\xf2\x9c\x86&\
-\x9f\x14M@dL9\xfa!\xc5\x8fZ4\xf9\xb8h\
-\xfa\xf9\x99\xe2\x19\x8c\xa4\xe4B4\xe1\x5c\xcf\x12\x9f\x9e\
-%&z\x96\x04\xf5,\xf1\x10<M<\xf04\xb9\x91\
-\xa1IPR\x9e\xd5\xdeb\xb0Z\xcf/:\xcb\x0a\xad\
-\xb6\x84\x91=:\x92\x10\x8d\x5c\x0f\xa1\xd2=\x04\x09\x95\
-\x1df\x94'r;\xa2\x9d\x03\xedR\x94\x88\xb1\xfb9\
-\xb1\xa3\xb1s\x1b;\x9f\x9d\x8b\x9d\xa70\xe8?^\xa8\
-5\x91f\x9a_\x5c\xb7\xf8\x9fX\xc7\x0bDI\x02\x02\
-\xabU\x88s\xed\xc3\x17\xd7\xb8`\x0f\x5c2\x17\x04W\
-\x83\x09\x14l`d.X\x04Y\xece#{\xb50\
-|\xbd\xf9\x7f\xden\x1b\x1dx\xc6\xce\x92\xfa\xf6;j\
-\x7fo\x01g\xd1\xf7\xfd\x9c\xc7\xcf\xb5/\xd3\xd7+\xde\
-Bo8\xf4\xdf\x94\xc6S\xb4\xd4\xfb\x01\x04\x14\x1e\xd8\
-\xbc\x00\x00\x00\x90\xc0b\xbc=\xbfv\x16\xbd\xf2\xe0\xad\
-\xfez\x5c\xb9\x90+V\x8c\xb5\xc9\xdf\xd7sa\x9dp\
-*\x9c^\xa4\x9f\xb6\xdd\x19\xcf\x18|\xb22p\x02\xee\
-\xb9\x90\x9e\x8b\x86\x99\x9e'\x8a\xaa\x89\x22=\x05+\xf0\
--\xfd`\xa79n\xba\xb5\x819E\xdc\xfe\xb0\x86\x1b\
-\xbf\xb4\xe8\xf0mN\xf8\xff\xd5\xdb\x83\x15\xe5y\xfb\xed\
-\x7f\xf7\xf3\xcf>\x8bS\x14iX/\x9d\xaa\x15\xcas\
-i\xd9\x1fe\xe1\xac\xa5_\xdd\x9fCk\xa2\xa5\x0e^\
-\xea\xb8\x8ci\xbf\xe9\x07~~0c\xfd5\xe3\xfd}\
-\xae-\x0fp:\xd1n:\xc5\xd2\x17W}\x7f\x93.\
-\x02'o\xd2\xb0\xa5\xb5\xf5\x97\xdeXKC\xd8\xad\xb4\
-\xe6\xe4y\x99\xe6X\x8cc\xa7U\x01\x0f\xf5\xe2\xb9\xa0\
-T+\xd4\x8b\x0a\xe5M\x94\xe7\xa1V.,\xfd:\x15\
-\xf6\xa2bm;\xd2\xd9\xb7D\xbcm\x01'\x06/\x17\
-\x98J]\x9c\xa9\x1d\xbf\xba3\x15}c\x1bO\xe1h\
-\x8e\xb5|8\xe3\xcd9\xb5\xd7\xcc\xac\x0c\xcc\x9a\xa6y\
-\xbb\xad\xb4\x86f\x8a\xd4\xde\xac\xa6j\x86\xb3\x1a\x9f\xbf\
-\xf1\xa6v\xd6\xf2\xd5\x8d_W\xf2\xc5\xa5\x9as\x86c\
-\x05?\x9c\x13\xf4\x16\xcb\x0c\x05\x06\xbe\xf5ha\xc5/\
-\x0e\xe9\xbd5\xc6\x15\x83\xa9\x19\x1dk\x0b\xe3\xa9\x8d\xed\
-\x7f\x97>`!SdJ\xb5\xe2\xb3\x19\xb6}\x95&\
-B\x8c\xef\xa7\x81\x15\x83\xb7\xf8\xf7\xb3\xd9;\xe8\xb6\x09\
-\xabp\xc2=\xae\x86\xc6v\xab\x0dq\xdaQ\x99~\xe0\
-\xeb\xd1q\xf6\xbeX\xc0\x07\xbf\xcf\xbe\xf1]Y\x19 \
-W\x06(\xe9(\xd2Q\x8eb\x01W\xfc\x80\x9ei\xda\
-\xad{?\xcc\xc3\xdf\x1a\x07\x9b7702\x0a\x0bd\
-.\x19\x18\x9bW\xcc\x8cL\xc6\xe6\x05A\xef\x11\xe7\xc0\
-\xb4Xzk\x98?\xe6\xf7\xc5\xd7\xdec\x0exG\x9c\
-\xa9-\xe3\x09S\x14E\xd1\x9b\x03\xfc\x01\x8c\xcdk&\
-v\xf3\xaa\x89\x16\xb7f_\xb5\xa2\x08\xa3Z\xa9V\xaa\
-\x15\xa9Z\xbd\xa8^T/*\xf2E5\xe7\x9csU\
-\x80\xa45\xb7\xd6\x9c\xe6\x9c\xa47\xe7T\xa9hb2\
-*\x8fTM\xcf\xfb\xaaGz\xde\x9c\xac\x83\x96\xa8\x92\
-\xa4\x14!\x92\x91\x19I\x92\xa40\x8c\x01\xd2!\x04b\
-a\x18\x0a\x9d\x98\x1e\xe2@\x0c\xa68$C\x10\xc3 \
-\xe2\x08Q\x84 \x01!D '<\x91 A\x92\xe8\
-\x013\xb0\x0e\xb7\xb7\xde1\x82\x9a\xb8zEAl\x1e\
-\x0az\x1bg:\xc8\xcaC\xcdcG\x1f\xda\xd1b-\
-\xe2\x9e\x94%3n\xb4\xa0\x16\xec\xd5=\xce\x5c\xacP\
-H]\xbe\xa5v1\xca\xd3\xca]\x17\x0b\xdftc\xfa\
-\x9c\x14\xca\x83\x95\xafg\xf7\xdaS\xf3\xf72\xcc@4\
-\x10\xc7\xc0T\xa3n\x88\x04\xf9\x03\xe6\x14k\xe9\x03\xbb\
-j\xb7N\xa1\xbb\xfa\x05`\xf6\xc98\x98\xe0\x82bC\
-|\xf4\x02yo\x98-6^\xcbK\xca\xc4\xbe8\xad\
-\x9a\xc2\xa6l.\x99d\xa7\x0f\xbc\x9eJ^\xf4\x98h\
-\xed\xfb\xb5oFn\x1f~u1\xad\x93\xdei\x82\xd4\
-p7\xa5\xa9\x9d\x89\xcaf)/\x8c\xa7\x17\xf7\xd6{\
-~\x0a4\xbe\xfchr,$\xf1\x18r\x94x\xfc8\
-\x9b\x95B\x15\xea\xa9\xd7\x83b\x94\xb8\xd7\xbfC\xab\xdc\
-\xc5\xf1\x16%\xa0\xb1C\xca\xe9F\x83DL\x9a6\x86\
-l\xd9\xdeC\xb9\x0a\xd5W\xc9\xd9a\xf4\x8d\xaa\xc2\xed\
-\x1e\x1f\xbf^\xc7\x92\x16\x00\xb8\xfe\x1b6\xca5\xb2\xb2\
-\xcc\x85\x17\x8b\x07\xca\xb5G\xac\xc8\xc1\xc4si\xcb\xff\
-$o\xf2D}\x01<\xa22\xe3\x03w\xe7H\x8c\xde\
-\xcd\x07m\xe0\xb3\x8a\xff\x8a\x81ToK\xfe\xe8og\
-\x8a\xdckQ*\xc5\xcd\x1e\x9d\xdd\xda\xabB\xbd~\xee\
-\x96M\xdc5\x93L\x81[\xb4m\x8b'\x10D\x0d\xc2\
-\x98g\xef\xd5\xbc\xd0\xa9c\x9c\x07\x12\x17X\xba\xbc\xfd\
-\x05\xc8F\xa0\x19S\xfb\xfd,\xdf\xbf\xfe\x90\xdb\xa7\xfb\
-\xac,\x85\xea\xd0\xf0\xe1[I\x88<\xd0O\xef\x1e\x93\
-\xa1\x97\x22\xf7/VHt\x1f\xde7\xd0\x87\xd8\x05\x08\
-\x17\xd6cI\x9ej\x05\x0ds\xf8\x90\xa3\xd5\xaa\x16?\
-\x06\xb66\x8e\xfa*\x92\xc4Y\xf3\xe5=\xe8F\xa1\x86\
-\xb1:\x82*i\xefX\xe0\xe8t\xf2j\xb6\xb6Wl\
-\xcahS\xa6\xe6\xf3I\xc3\xf5\xdb[q\x8ez)\xad\
-\x13c\xcc\x1a\xcbl\xd7\xcb\xa9#b\xbf&:tj\
-\x1e\x9c?\xac.\xbb$\x89\x9c\x93\xf2\xc0\xde\xb1D\xa1\
-w\xe2CMR\xaf\x9d&\xa1+\xd1Q\xd0\x92\xfb\x1a\
-\xda\xd3\x1a\xf5A\x0c\x06\xe3k\x92\xdb\x17\xa8\x8c\x99\xd5\
-\xf4Y=\x1a\xe37\x9a9\x94.\x8a(\x1f\xa9\xd4\x80\
-{\x8b\x00f\x87\xd2\x09\xc4\x1e\xdd\xf1\x16\x0eG\xf8\x82\
-\xecw\xe0\xf5\xbf\x5c~sN\x81*A\x99<\xebw\
-\xd9+'\x9a\x8d\x89\x9d\xdf:L\xe9B\x86\x9a7!\
-rL\x97=\x93j\xb2\xa8\xa5\xe0\x22\x80\x05\x1e\x98\xc1\
-cOp7\xfaC\xbd`\xadf\xa9\xa4\xf2>\x15\x18\
-pi\xec\xb5'3i\xd5^\x7fo\xae\xf6$ak\
-\x7f\xa0R\xd2\x88\xa9|/\x09\x82~l\x11A5:\
-\xc2\xaa\xd5Y\xe8\xae\x88\xe93\xbf\xeeH\x81\xe3+f\
-U\x96\xbd\xa0\x86\xd2\x10\x22\xe2S\x5cP\xbcz\x9b7\
-\x03\xe3\xfd\xaa\xb8\xa5\xa7\xc8\xe3B\xa0\xae^\xba\xa5\xb7\
-\x8bo\x1f\x0b\xf40\x0e \x88\xe9\xe6\xc1\x0b\xc7tf\
-\xde\x9aY\x08\x22\x02\xe6\x1eL.\x85\xe8\x12L`\xb5\
-\xc0\x86\x9c\xb8V\xccBmOfH\x5c\x1f\x04\x1d\xed\
-^e6w\xe0[\xea\xf5L \x89\xc8\xd1\x05q\xbb\
-16\x0f\xb1\xc0\xc0e#=\x00\xb3\xb8\x1c\xc8b\x80\
-t\xb9N\x87;\xb22\xa3t\xf4\xdfEl\x11\xd4\xf5\
-\x85\xdc\xd4bb\x12\xfc)\xe3D\x0dc\x16:\xa0T\
-\xbd\x82\xc5\x0e\xe4\x13\x97\xaf\xf6\xb2\x83\x8c\xfa`\xba\xb0\
-\xc4\x94\xe3.e\x11L{\xbc\x9c\x1aiNs\x95r\
-pQ8Nw\x81:\xd08L\xadEe\xb32\x14\
-\xa9\xb3\xd1\xf629\xe7.$\xc7\xf1<\x82\xd5\x9b\xe6\
-\xb0\xdb\x0b\xe4\xe2\x1a\xba\x9d\xacH5v\x82\x1c?^\
-HnU\xa4\x0c\x10\xc7gA@Fwu\x22\xec\x8b\
-#\xa3\x18e\x04B\xd3\x12eI\xd3Tb\x90\xa8\xc6\
-\x19g\xdd\xaf\x02o6)\xb7\x0dG\x9ah\x8f@\xda\
-\xe5\xaa\x95\xb02 \xb2\xa9+\xe2\xdc\xe4HV\x0c\x97\
-\x0fW\x8a\xdb\xdf\x8d\xfc.\xbb%Z\xd2\xf5]\xd2s\
-\xfb\x07:\x18\xd21\xe8\x9dW\x95\xb8\x12Q<\x1d\xca\
-hYP\xf2C\xb95\xb7\xfc\xb0\x00q\x5c((\x8b\
-\xa7\xa8o\xcfFrN\x1ao,\xcd\xe1\xe5\x83\xfa\x9e\
-4\xbe\xc7\x0a\xf6J?x\xc4Z\xd0\x1f\xda\xd0\x96\xc9\
-\x8d\x83\xe0\xcbS\xd6\x05\xea^A\xe8@\x0f\x8f\xe0?\
-\xc2\x8d\x837u\x1b\xae\x12EF\xa7\x9b\x02\xc1J\x0e\
-\xee\x9f\xb0\x9b\x1d\xf2\x82,\xbf\xaf\xad\xe3t\xfcy]\
-\xae\xa5\x0b\x1d\xc7\x80wd\xde\x19_\x90\xaa\xa4\xa0\xd8\
-\x00\x1c\x98\xa1\xee\x00\xad\x92\xfc\x99\xe6\xdf`Hn\xce\
-s\xac\xf3:9\xe6\x90f\xb8\xcf\x5c\xf1\xb3\x0eu\x04\
-\xc4@\xd0\xff\xf5\x86\xdb\x02\xc84N\x84\x0b\xd8\x7f\xb3\
-)\xc0\xee\xce\x15\xaa\xe6\x13BX\x83\xef\xda\x88\x1e`\
-\xb0\x92\xbb\xbb.\xc4\x9f\xdfy|FZ\xedM\x1c\x15\
-\xa7/\xcf\xf9\xeb91\x89\xed\xe8\x12;5<\x87\x08\
-\x9d\xb7u#.\xdd\xdf'\x19I]#2<\x08\xff\
-?\x86N\xce8j\x10\xceX\x19\xc0\xd8\x07[Q\xfd\
-f\xe1\xc1V\xb4\xa6 \x06'\xae\x0a!\xa0\xf1md\
-\x10\xa5[@\x07\xae\xf5\x8d\x87\xb3\xb0\xde\xf9:!+\
-(\xbc\xc5\xb3\xedU\xd3\xbd\x08\xd6\xc2T#\xdf/\xf1\
-\xea\x05R)\x8d]\x15q]\xcaI\xb4S\xfc+\xbb\
-\x09y\xf0\xcc\xae\xcc[\xa2\x86i\x90\x06q\xdb\xc8K\
-TV\xe2Z\xa8|R\xb7\x19\x9f\xd7\x82\xfarh\xb7\
-\xe3\xc8tU*\xbd0\xedD\x22\xff\xf6g*g\xec\
-\xe2u<\x81J]}\x1d;\xff\xf7\xf0\xa5U7w\
-\x92l\xfc\xbf\x94\x04\x98uZ\x95\xeb\x9e0\xdc\xe26\
-(\xa8\xa10\x09\x8d\x01\xc8r]\x0e\xf0\x07?;\xf1\
-\xee\xd2b\xb8\xb4\x9f\xa7\xdd\xae\xb8\x89\xce\xae\xadtz\
-\xc2\xba\xb3\xc2?D#S9\x08\x87\x04\xb9ji\xe6\
-=\xd7U}\xbb\xc9\x0b'\xcf\x98\xfe\xe8\xb1\xba\xdb\xa7\
-dYo\x17\xc6\xc7\xd1\xd4h\xd6%s\xf5\xfb\xe1\xdc\
-2xn^*\x96\x7f\x7f[\xb9\xe1D\x1c\x0e\xbfn\
-\x81\xd4\xbd\xa4\x84\xd8/\x1fV\xe7<\xc4P\xec\xd9L\
-\xd92\x11\xb3\x93\x9dk\xf6\x0e\xaf5a\x8c\xc1\xea<\
-\xed<\xe1\xab\xb7\xbf-L\xd9\xb8\xcf\xdb\x90Q\xb1Y\
-\x90;\xb0ZC5\xaf6\x08\xc2\xe4-\xcd{)N\
-0\x842(Cd\x7fq)TX\xbaI&0,\
-]S \xfc&8\xe1\x22\xc7\x1b\xba>\xd1\xb8\xafV\
-\x9dpd\x14\x00\x99'^\x8ca\xa8\xe2=\x08c\x9f\
-xc\x0e3wD\xcb\xce\xb8\x98\xec\xa5\xfax\x92\xdb\
-\xcek%Y\xa1\x13\xc2\x80I\x04\x80\x13\x84\x86\x08\xaa\
-7\x98$\xabZs+]\x99Q!}\x87\x06\xf93\
-s\x19\x06\xd6x\x10\xfe\xa18\xaf\xb9J\xb4\xac\xf3\xc3\
-7\xee\xbdz\x1f\xc2w\x17,yE\xfe\x06$\x03\xd2\
-\xf8;\xc1:\xa5\x1e\xb5\x86\xef\xbaL\xd7(A\xd5-\
-\x1b\xed\xbe\xf5\xda\xaed\x95\x83d\x02k\x07P\xe9'\
-]\xed\x80N\x0b7\xb6\x9e\x05:G\x13\xa7B\x800\
-\x90\x80\xeb\x02\x9cL\x93\x01\xc3\x82\x80\xb5\x09\x22\xe8f\
-\x07d1\x1a\xa5wO\x5cw\xf2\x87z\x0b\x924\xce\
-\xb4Q\x07\x1e\x18\xd1\x1f\xd5\xbaHC3\xe9\xe7\x17F\
-\x0cPQr\xa2/\xd0pU,'\xa4<\xfe\xae\xdb\
-\xa2\xb1\xcc\xf1\xae\xf5\xa1G\xf2^E\xfcS\xb6sC\
-EJDP\x9c\x85\xc2\xe3 \x18\xf0\xfc\x5c\x9e\xfew\
-\x87\xddw:\xf8pk~L\x90\x13 \x0a_&\xf1\
-]\xbc\x97\xdb\x98\x92\x93^\x90\xca\xe6+-\x02\xc7\xa9\
-\xa1\x09cqi\xc9\x18AW\x0c\x11\x9c\xbc\xa6\xcb\xa8\
-\xc0\x86\xbe\x94l\xe1\xf8Zs\xb4ZjHXA\x9b\
-\xe1:E\x0b\xb5\x96R\xe1\x22\xc3!\
+\xd3\xa8\xfd\x18\x07L\x01V\x01+\x01\xd63\xcdBI\
+\xdb\x1e\xa0\xb7\xd2\xdem\xa8q[\x02\x1b\x8b\x9aZ\x22\
+H4$q\x11Iv\x92\xe8@b?_|\xfb\x19\
+\xa5 \x885h_\xf4M?\x7f\x8e\xe2Q\x82\xa4\xa3\
+\xe5\x5c\xa0#\xe0\xad3\xa0#\x19\xe8\xc8\xf6\x1cJ \
+\x96|\x96zz(\xd9Pr\x22% J\x1ep(\
+qX\xda\xb0\xe42-\x09\xeej\xd1\xf8\xd7\xb6\xe3r\
+\xf6\xfd0\xc41\xa7\x091\x122\xa2\x14!=q\x9b\
+\x18YM\x87$IR\xff&@\xd6\x9bm\xac\xfbV\
+\xed\x12\xa2;\xd2ehA\x1b\x91\xa3<**wr\
+\x94FE%\x91\xa2\xd2F\xd1\xfeh\xa6\xfbo\xf8\xa6\
+nj/\xad7j{\x0bU\x01\x87\x1d%F:\x1e\
+%=t;tH\xba\x17:\x96\x15\xa7_\x15)\xcc\
+\x86oP\x92\x04\x16\x8eM\xf7\x14\xd1\xc1\x19\xc2\x02\xd9\
+\x16q,\x88\xca\x1d\xa2\xd2h\xa8\xc41D\xc5k\xef\
+m[l\xa3\x16\xa8\x8e\x8e~\x90V!BeN\xa8\
+\xdc\x99Q\x1a\x09\x95#f\x948\x84\xca\x9f\x1d\x8a\x1d\
+\xd0nhWbW\xb34\xfa\xbb\xbeX8 -\xd7\
+\xd9\xb8_\xe3\x052\xb2k\xff)\xa8\xebw\xdf\xd2\x9b\
+\x02\xaa+\xfdh98:\x1b\x96@,\xf1P\xe2\xb0\
+\xc4\xc2\xc9\xb4\xc2\xeb\xfc\xe7\x05\xac\x0f\xa9\xcd\x09\xe7\xc3\
+\xaf\xc5\xfc\xe2o\xa6B\xb0\x18\x8d\x01[\x8b\x19<h\
+\xf1\x8c\xf5V\x0c)\xe9:\x9d2\xb6\xf8\xab5\x96\xde\
+5\x7f\xed\xce\x9cN\xded\xd5\xb6\xf8-\x1c\xb5\xa2\xae\
+-\xd7\xb0\x02\xca\x10\x19L VDQ\x91{2\xc4\
+\x89\x0f\x0f\xce\xf2BE\x94\x18,\x9e\x04\x151!\x15\
+1}\xa8\xc1\xc4\xa1\x06\xd3\x8a\x8e\x1f(\x22\x84TQ\
+\x11#J\x90#'$Yo?GH;P~)\
+x\xc7\x9c1\xcbx\xa8\xa3H\xa6\x9a\xc6\xdc\xbe\xce>\
+\x92d\xf2\xfe\xa13\xd2\xb9(\x8e\x99viU[\xfb\
+\xa3\xae7\xd7\x07n\xf4f\xb5\x1e3\x0ac\xba)\x86\
+\xad3\xde#u\xe7\x19*C\x10\x95;\x86r=\x86\
+\x86\x82\x86\xca\x0eD\xe5\x89\x19\xf7f\xbc\xc3\xc4\xc5\x0e\
+\x13\xcfPdc\xb0\xfe\xedf)\x8d\x8a\xdb\xe6NP\
+)\xe1\xa2)\x07\xa3\xc9s\x1a\x9a|R4\x01\x911\
+\xe5\xe8\x87\x14?j\xd1\xe4\xe3\xa2\xe9\xe7g\x8ag0\
+\x92\x92\x0b\xd1\x84s=K|z\x96\x98\xe8Y\x12\xd4\
+\xb3\x84\xda<\x04O\x13\x0f<Mndh\xe2AI\
+y\xa6ko1X\xad\xe7\x17\x9de\x85V[\xc2\xc8\
+\xa6\xeeHB4r=\x84J\xf7\x10$Tv\x98Q\
+\x9e\xc8\xed\x88v\x0e\xb4KQ\x22\xc6\xee\xe7\xc4\x8e\xc6\
+\xcem\xec|v.v\x9e\xc2\xa0\xffx\xa1\xd6D\x9a\
+i~q\xdd\xe2\x7fb\x1d/\x10%\x09\x08\xab\x10\xe7\
+\xda\x87/\xaeq\xc1\x1e\xb8d.\x08\xae\x06\x13(\xd8\
+\xc0\xc8\x5c\xb0\x08\xb2\xd8\xcbF\xf6ja\xf8z\xf3\xff\
+\xbc\xdd6:\xf0\x8c\x9d%\xf5\xedw\xd4\xfe\xde\x02\xce\
+\xa2\xef\xfb9\x8f\x9fk_\xa6\xafW\xbc\x85\xdep\xe8\
+\xbf)\x8d\xa7h\xa9\xf7\x03\x08(<\xb0y\x01\x00\x00\
+ \x81\xc5x{~\xed,z\xe5\xc1[\xfd\xf5\xb8r\
+!W\xac\x18k\x93\xbf\xaf\xe7\xc2:\xe1T8\xbdH\
+?m\xbb3\x9e1Y\x198\x01\xf7\x5cH\xcfE\xc3\
+LQTM\x14\xe9)X\x81o\xe9\x07;\xcdq\xd3\
+\xad\x0d\xcc)\xe2\xf6\x875\xdc\xf8\xa5E\x87os\xc2\
+\x9f\xff\xd5\xdb\x83\x15\xe5y\xfb\xed\x7fw\xf6Y\x9c\xa2\
+H\xc3z\xa97U+\x94\xe7\xd2\xb2?\xca\xc2YK\
+\xbf\xba?\x87\xd6DK\x1d\xbc\xd4q\x19\xd3~\xd3\x0f\
+\xfc\x8c\xf5\xd7\x8c\xf7\xf7\xb9\xb6<\xc0\xe9D\xbb\xe9\x14\
+K_\x5c\xf5\xfdM\xba\x08\x9c\xbcI\xc3\x96\xd6\xd6_\
+zc-\x0da\xb7\xd2\x9a\x93\xe7e\x9ac1\x8e\x9d\
+V\x05<\xd4\x8b\xe7\x82R\xadP/*\x947Q\x9e\
+\x87Z\xb9\xb0\xf4\xebT\xd8\x8b\x8a\xb5\xedHg\xdf\x12\
+\xf1\xb6\xe9\x1f\xf3f}\x01'\x06/\x17\x98J]\x9c\
+\xa9\x1d\xbf\xba3\x15}c\x1bO\xe1h\x8e\xb5|8\
+\xe3\xcd9\xb5\xd7\xcc\xac\x0c\xcc\x9a\xa6y\xbb\xad\xb4\x86\
+f\x8a\xd4\xde\xac\xa6j\x86\xb3\x1a\x9f\xbf\xa9\x9d\xb5|\
+u\xe3\xd7\x95|q\xa9\xe6\x9c\xe1X\xc1\x0f'\xe8-\
+\x96\x19\x0a\x0c|\xeb\xd1\xc2\x8a_\x1c\xd2{k\x8c+\
+\x06S3:\xd6\x16\xc6S\x1b\xdb\xff.}\xc0B\xa6\
+\xc8\x94j\xc5g3l\xfb*\x8d\x8e\x10\xe3\xfbi`\
+\xc5\xe0-\xfe\xfdl\xf6\x0e\xbam\xc2p\x8f\xab\xa1\xb1\
+\xddjC\x9cvT\xa6\x1f\xf8zt\x9c\xbd/\x16\xf0\
+\xc1\xef\xb3o|WV\x06\xc8\x95\x01J:\x8at\x94\
+\xa3X\xc0\x15?\xa0g\x9av\xeb\xde\x0f\xf3\xf0\xb7\xc6\
+\xc1\xe6\x9c7702\x0a\x0bd.\x19\x18\x9bW\xcc\
+\x8cL\xc6\xe6\x05A\xef\x11\xe7\xc0\xb4Xzk\x98?\
+\xe6\xf7\xc5\xd7\xdec\x0exG\x9c\xa9-\xe3\x09S\x14\
+E\xd1\x9b\x03\xfc\x01\x8c\xcdk&v\xf3\xaa\x89\x16\xb7\
+f_\xb5\xa2\x08\xa3Z\xa9V\xaa\x15\xa9Z\xbd\xa8^\
+T/*\xf2E5\xe7\x9c\x93\xa45\xb7\xd6\x9c\xe6\x9c\
+\xa47\xe7T\xa9hb2*\x8fT\xcd\xe9y_\xf5\
+H\xcf\x9b\x93\xb5\x0a\x83\x9e\xa8\xa2\xa4\x16!\x12\x91\x11\
+I\x92\xa40\x8c\x01\xf2\x19\x04\x82Y\x18\x0a\x9d\x97\x1e\
+\x229\x8c\x041\xa4A\x10\x06B\x04\x1a\x82\x08A\x84\
+\x10\x22\x10KB\x91`\x82\x8cD\x0f3\xb0(\x80\xaf\
+B\x22\xe5J\x0c\x9d[\x08\x9b\x17,ouL\xc7\x10\
+\xf3\xf4<\x86\xefC\x8f\x16;\x11O\xa7<\x8aq\xa3\
+\xc5i\xc1B\xf7ps\xb1\xc5\x8b\xd4\x09=u\x8b\x11\
+O\xf9q\x9dj\xbfI`\x0a^\x11\x0a\xbbM\x96a\
+\xf7\xfa\xa8\xf9;\x1ff#\xda\x97\x91\xdc\xa4QL\x22\
+y-\xe7C\x85\x0e\xf9\x10\xba\xea\x10\xa7p\x5c\x1do\
+\x98\xfd4\xae#\xb8\xbc\x8a\xa1z\xe9A\xde=\x02\x17\
+7\xafM\xd82\xbf,N\x1b\xa2\xb0\x0b\xdb\xa5Y\x92\
+\x8d<8<Ul\xd1\xcfr\xedshw\x8c\xc4H\
+\xfcU\x06*Nz\xeb\x09\x08\xc3\xbd\x94\xb4vh\x95\
+\x99#/*\xcc\x17\x93\xfa\xd0\x1f\x87F\x5c)\xad\xdf\
+B<\xaf?G\xc7\xf1\xa6l\xa6\xf8\xa9\xb9i\xbd.\
+\xdaX\x22+!Z\xeb\x92\x8bK%\xca=\x1a\xc9$\
+\xc1o\xe4M\x88!y\xc1\x90\xad\xb1{(W\x81\xfa\
+\xca\xb8\xf3\x01\xfa\x06\xaf\xe1v\x1f\x1fY\xaf}I\xeb\
+\x00\xa7\xff\x86\x8dr\x8dZY\xfa\x0b\xb1\xb8\xe4\xe1x\
+\xa2K\x0e\x96=\x97V\xfe@\xbf\xc9\x02%8x(\
+\xcf\x8c\x1f\x19\xf7\xa2\xc4XN\xd1\xda.\xcfZ\xfaU\
+n\xa9(\xab\xfe\xe8_\xa7\x14\xa9i\xb9E\x8a\xbe?\
+B\xd9\xda\xdcJ\xea\xfdh\xca\x9ah/$\x99\xd8\x90\
+\x97-*\xe5\x111\xc1\x11\xb9\xd0^\xbb\xf9\xbe\xe3\x81\
+s\xca\xd6\x13\xae0\xba\x04\xfe<\xceF\x90\x8c\xa9\x89\
+\xfd\x05)\xbf\xb2%\x9cv\xf1Y\x22\x06\x95m\xc8\xfd\
+\x96>\x22.\x09\xe0\xbbJy\x04)\x9c\x7fw\x81\x04\
+;\x9f\xc1\xc0\x0f1\x14A\xa8\xb3^\x5cbT\xadp\
+2\x0b\x049:T\xd5\xf9\xb1\xea\xb5y\xd1G\xd3%\
+\xce\xc7\x5c\xf7\xa0Y\x85\xfa\xb3\xea\xe8\xab\xa4\xdf1\x03\
+\x17\x96\x89\x0a\x06y\xbef\x96\xd1(\x99\xda\xcfE\x09\
+\x17\xb1bxNT\x89\xa8\x13\x9b\xb0FLv\xefr\
+\xe2H;\x9f\x13!\x9e\x1a15\xd6l\x89\x10%\xf5\
+8\xc7\x97\x81\xfd\xb7\xf0\xa17\xe5\x87hR\x17\xd2\x93\
+p\xa2\x81P\xa1R\xaf\x1aRUM\x05A\xac\x0d\x86\
+\xd6t\xca/F\x0c\xca\xd2\xf4\xad~\x80\x8a\xdf\x1cr\
+\x10\x98(\x16#R\xa3\xc6\xbd\xdf\x03\x84\x13\x8a'\xe8\
+.\xd4\xf1\xb6\x14\x0e\x8b\x05\x19\xec\xc0k\xa8w\x19w\
+^\xc2\x99\xe4\xc9\xe6~\xd7\x1a9gnl\xe3\xfd\xf6\
+\xf0@\x88\xc8 \xed\xb4\xcdJ]6\xccQGl-\
+m\x17\x06,\xbea\x86\xc5\x9e\xe8n\xf4\x0e\xf5\x82\xb5\
+\x9a\x9aJ%xy@M\xa7\xb1\xb7\x9e\x0c\xd2\x9az\
+o\xbd\x19H\x8c\x95\xad\xc5Um\x08\x8d\xec\x1c{h\
+P\xf2A%\xc2\xaaQ\x13ZPw\xbc\xbb8H\x1f\
+\xbeI\xba\xf4\xc1\xe8\xc4\x0f)5\xba\xbd\xa0|\xd2\x10\
+\x90 @\x1b\x82\x82\x83\x9b\xe0\x0e$\xfb%)[b\
+C~\xf0\x10x2L7Z\xab\xfd^\xc0\x02a9\
+\x02\xc8\x08\xde\x1c\xd3\xc21=\x9a\xb7t\x13\x826$\
+q\x98\xc9%\x81T\x03|g1`\xa3\x10\xd35f\
+\xab\xed.\xcc0\xb6\x0fo\xa1\xadW\xd7~\xf0\xfa\x16\
+\x19=\x13b%r\xeeYt\xd3\xc8stX \x0d\
+\xb2\xf1\x12\x00\x8fkP\xfc\x18l\x96\xcb\xd7K\x9d\x94\
+\xdc\x8a\xd6^\xc4\xe0\x8e\xba[d\x9f\xf6\xcb&}\xb2\
+\xca<\xa7&\x84\xf5\x0c\xe8pQxP\x92\xff{\x89\
+\xbf\x97h\x8c9\x13\xcc}\x89\xb1N\xb8c\xad1\xad\
+\x1c\xe4\xa0\xf6\x1b\xa7@U\xcf\x17e\x82\xabc\xa0\xda\
+\x09\x1c\xa6jE2\xabia\xc0\xd9\x10\xbcT\xe64\
+BR\xd8\xf1\x08\xca/*\x87\xba\x17\x10\xcd\xa5t;\
+9\x02D\xec\xb0q\x8a~m\xa3\x95\x9fd\x80)\xae\
+\x8a\x80\xa4\xdd-W\xd8:\x8e\xec2\xca(\x08\xadH\
+\x94\xc5\xa6\xa9\xde\xe8\x9bf\xdf\xd9\xd6{\xb5\xb9\x19\x97\
+\xdc6\x1c\x15\xd9\x14!\x07\xb9SH\x94,D\x9e^\
+\xc5\xed\x0b]\xccF%k\xe3r\xce\xa5p\xda\x8fx\
+~7\xc73X\xec\x95\x0b}\xb9\xc6\xc7\x0d\xda\x0b\xc6\
+f\xb0\xab\x92\x18\x1aA\xcf\x1fJ\xd0\x92\xe3=u\xb7\
+\xb2\xf5\xfb(\x02H\xf6\xd2\xa0\xc7\x9eB\xbbm\x10y\
+\x87\x16\xef\xaa\xcf\x19\x87\x7f\xe1\xadi\x94K\x11\xac\xe4\
+W\x95\xb0\x164}hCA&%\x0e\xd9\xf7}\xad\
+\x0b\xdb\xa3\x7f`x\xee\xc1\x08\xa1\x1d\x1f\x07oV6\
+\xbc\x04\x8a\x8aN7A\xcc\x02\x07\x9b\xee\xb0\xe1\x0e\x8d\
+\x8d\xec\x0b\xaaMs\xba\x17\xb5&\xfb\xe3\xd5\x89G\xa6\
+wcuvzHIT\x90\xc49\x1c\x9a\xf0\x0fi\
+\xf2Z\xe5P\xcfp\xf2\x86\x1crO\xcd\x81\xe2\xea\xab\
+B\xe0\xb1\x93\x22\x7f7\x19\xda\xb6\x0f\xa0\x01\xa4\xfe\xd7\
+\x0d\xe3\x0c\x90\xcc\xc7P\xb9\xb4\xfc\xaf\x1b\x1f\x08\xee_\
+!\x14\x9b\xe9\xa3\x0d\xe1W\x04\xba\xae\x1fS%\xf7\xb7\
+S\x11\x83\xaf\x09\x01;\xa0\xba3ao\xbf%\xd9\xe0\
+\xc4\xbf\x90\x93\x11\xa1\xadQ\x22\xed\xc2\x04\x17\xb1\xac\xc1\
+7I\xa1\xc8\x7fIC%\xb6 9\x02\x84\xe4/\xe5\
+\x13\x98\xe7\x0f\x9b\x10\xf8b\x03\xfbS\xd6\xc6j\xae\xd4\
+\x80b*\x1d\xce0\xe7\xda!\xd4\xba\x8a-\x03\x0d\xdf\
+F\x04\x03=:i{\xee\xf9Z:H.*|\x94\
+\x87\xb4R\xca\xc5\x91\x96?\xe8\xef9\x13\xf2,4\x91\
+\xac\xce3\x121\x92\x0cY\x01\x05\x94\xc1[\x05h\xd1\
+\xcf\xedM_>\x17\xf3\xa0~d'\xf2\x97<)\x16\
+\xbf\x16\xca\x22\xe5l\xf0\xce\xbb\xa0\x80>\xf4\xcd\x8f\xcc\
+\x10_>?]R\x18`\x22#w\x9b\x15\xdd3\x96\
+\xf1:X\x18\xb4\xad\xf0\xe6\xc5\x94;\x84o\xd9\xb3\xc2\
+\x22\xfdJ\xb7F\x10s\x11\xadj\xbb\x87xl\xd1\x04\
+\x14\xcc#\x98+\x8d\x01\xac\xb7\x06\x06\x08\x83\xff\xca\xbf\
+\x0b{G\x9c\xf6\xf3Z\xb7\x0f\xb2If\xa7^\xba.\
+!\x8c\xde`!\xc4\x18T\xf6\x80G\x82\x22-{\xf2\
+\xa6\xd5\x96t\xbb\x9f\x17JR\xd8\xe0\xa3\xed\xbcm?\
+%\xe1\x96\x8e!\xdc\x09M\xd1e]f\xd7\x8b<\x1c\
+|\xb4\x03\xf2bI\xb9\x90o\xd7\xc4\x08\x8bs\xfe\xd7\
+|\xe4o/\x1b!\x9a\xe3\x87%9G\x99\x1dc\x9b\
+\xc5\xec7\xe2~\x96\xba\x06\xed\xb0E\x13\xb61\xb8\xf9\
+\x81\x9b\x07\xe1k\xf9a\x86\x81\xc2\xb8H\x1a\xfd9\x9e\
+\x12M\x07\xd6\x9d\x04\xbf\xaby\x82v\xd6\x167\x02%\
+\x8e&#T\xda{\xc1\xa5va\xbd\xc9C\xc6'0\
+!|\x10\x9csqm\x19y'a\xbb\xf7Pow\
+\xe6\xf2\x0e2\x07\x22\x1b[T\xdf[\x95Y\xc4\x03\xc4\
+=\xdc\xa1\xd9\xc52\xc6\xdc\xe3\xae\xaa\xb8\xdc\x1c\xbc\xad\
+\xb9E>\x99\x0b\xe7D\xf59\x03f\x03\x08\x94\xc1\x88\
+e\xc33}t\x95D(d~\xa8$?;\x12\xf2\
+\xa2\xcb\x8d/\xb19\xd4,\x99\xa2\x10\x10_\xffB\x86\
+\xcb0\x84\xc7\xca;\xa1C\xfc\xc8\xa7\x01\xf5\x85\x8c\x7f\
+G\x9f\xa8\xf0{\xda\xbc\xa4[z\xc2:\x84\x92\xec\xa9\
+z\x1a\xaek\x8d\x1e\x929\x93\xc1\xee.\xa1K\xca\xda\
+\x01\x90\x16qv6St\x97&\x1c\x85\x90\x9bd\x02\
+\xb0\x1b\xfc!\x8dt\x0c\x00\x01\xe49\xe0\xa1\x9b2\xc8\
+-\xd3\xae\x90\x9b\xe6r(\xff\xfe[`N\xb1\x9f\xbc\
+@c\x03\x9b\xbb[\xa3+2Ty\x7fK\x18\xb2@\
+-\xc9\xa5\xbc\xa8\x89\xeb\xeeb\xca\xe0K\x1f\x18Ht\
+\x80\xbc\xb5Z`Zm\xda(\x94I\x81\x1f#\x8e\x05\
+5P\xb6\xc2\xc5#\xcf1$\xb9\xc2\x9d\xc5\xbbYM\
+!\xa3Tr\xc4*x\xbco\xb10a\x1b\x04\xc7\xd2\
+\x86\xccI\xf8\x98\x11\x82\xf9\xa7\x7f\xb7 \x8ag\x92\xd6\
+/q\xd9.\x91\x92F\xa4(\xb8\xab6\xbfP\xe2l\
+\xdf'7\xd6A\x22mXtO\x86x\x95\x8f\x0d\x15\
+W \x99Re\x85\x07\x0d\x87\
 \x00\x00\x02.\
 <\
 svg viewBox=\x220 0\
  16 16\x22 version=\
 \x221.1\x22 xmlns=\x22htt\
 p://www.w3.org/2\
 000/svg\x22>\x0a    <d\
@@ -7483,219 +7483,219 @@
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00f\x00\x02\x00\x00\x00\x01\x00\x00\x003\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00~\x00\x02\x00\x00\x00\x02\x00\x00\x00.\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x90\x00\x02\x00\x00\x00\x01\x00\x00\x00\x08\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00J\x00\x04\x00\x00\x00\x01\x00\x00\xdb\x17\
-\x00\x00\x01\x8f\xc0\x8dE\xe5\
+\x00\x00\x00J\x00\x04\x00\x00\x00\x01\x00\x00\xdb\x18\
+\x00\x00\x01\x8f\xd9M\xfc\x1e\
 \x00\x00\x00\xa4\x00\x02\x00\x00\x00%\x00\x00\x00\x09\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\xbe\x00\x00\x00\x00\x00\x01\x00\x00\xfe\xd2\
+\x00\x00\x01\xbe\x00\x00\x00\x00\x00\x01\x00\x00\xfe\xd1\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x01x\x00\x00\x00\x00\x00\x01\x00\x00\xf8{\
+\x00\x00\x01x\x00\x00\x00\x00\x00\x01\x00\x00\xf8z\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x00\xae\x00\x00\x00\x00\x00\x01\x00\x00\xe8\x07\
+\x00\x00\x00\xae\x00\x00\x00\x00\x00\x01\x00\x00\xe8\x06\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x04~\x00\x00\x00\x00\x00\x01\x00\x01~\xa0\
+\x00\x00\x04~\x00\x00\x00\x00\x00\x01\x00\x01~\x9f\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x04\x9e\x00\x00\x00\x00\x00\x01\x00\x01\x80\xba\
+\x00\x00\x04\x9e\x00\x00\x00\x00\x00\x01\x00\x01\x80\xb9\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x03\x02\x00\x00\x00\x00\x00\x01\x00\x01g\x9d\
-\x00\x00\x01\x8f\xc0\x8dE\xe5\
-\x00\x00\x01P\x00\x00\x00\x00\x00\x01\x00\x00\xf3\x97\
+\x00\x00\x03\x02\x00\x00\x00\x00\x00\x01\x00\x01g\x9c\
+\x00\x00\x01\x8f\xd9M\xfc\x1e\
+\x00\x00\x01P\x00\x00\x00\x00\x00\x01\x00\x00\xf3\x96\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x05\xb8\x00\x00\x00\x00\x00\x01\x00\x01\x8f\x05\
+\x00\x00\x05\xb8\x00\x00\x00\x00\x00\x01\x00\x01\x8f\x04\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x02\xda\x00\x00\x00\x00\x00\x01\x00\x01_\xd2\
+\x00\x00\x02\xda\x00\x00\x00\x00\x00\x01\x00\x01_\xd1\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x03\xa2\x00\x00\x00\x00\x00\x01\x00\x01q\x8b\
+\x00\x00\x03\xa2\x00\x00\x00\x00\x00\x01\x00\x01q\x8a\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x06\x06\x00\x00\x00\x00\x00\x01\x00\x01\x94-\
+\x00\x00\x06\x06\x00\x00\x00\x00\x00\x01\x00\x01\x94,\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x03\x1e\x00\x00\x00\x00\x00\x01\x00\x01j]\
+\x00\x00\x03\x1e\x00\x00\x00\x00\x00\x01\x00\x01j\x5c\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x062\x00\x00\x00\x00\x00\x01\x00\x01\x96)\
+\x00\x00\x062\x00\x00\x00\x00\x00\x01\x00\x01\x96(\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x06R\x00\x00\x00\x00\x00\x01\x00\x01\x98\x1c\
-\x00\x00\x01\x8f\xc0\x8dE\xe5\
-\x00\x00\x01\x00\x00\x00\x00\x00\x00\x01\x00\x00\xed\xae\
+\x00\x00\x06R\x00\x00\x00\x00\x00\x01\x00\x01\x98\x1b\
+\x00\x00\x01\x8f\xd9M\xfc\x1e\
+\x00\x00\x01\x00\x00\x00\x00\x00\x00\x01\x00\x00\xed\xad\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x01\xf0\x00\x00\x00\x00\x00\x01\x00\x01\x04\x0e\
-\x00\x00\x01\x8f\xc0\x8dE\xe5\
-\x00\x00\x05l\x00\x00\x00\x00\x00\x01\x00\x01\x8a\xdb\
+\x00\x00\x01\xf0\x00\x00\x00\x00\x00\x01\x00\x01\x04\x0d\
+\x00\x00\x01\x8f\xd9M\xfc\x1e\
+\x00\x00\x05l\x00\x00\x00\x00\x00\x01\x00\x01\x8a\xda\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x01\x9e\x00\x00\x00\x00\x00\x01\x00\x00\xfa\xf1\
+\x00\x00\x01\x9e\x00\x00\x00\x00\x00\x01\x00\x00\xfa\xf0\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x02F\x00\x00\x00\x00\x00\x01\x00\x01W0\
+\x00\x00\x02F\x00\x00\x00\x00\x00\x01\x00\x01W/\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x05\x8a\x00\x00\x00\x00\x00\x01\x00\x01\x8d<\
+\x00\x00\x05\x8a\x00\x00\x00\x00\x00\x01\x00\x01\x8d;\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\xea9\
+\x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\xea8\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x02\x8a\x00\x00\x00\x00\x00\x01\x00\x01[*\
-\x00\x00\x01\x8f\xc0\x8dE\xe5\
-\x00\x00\x05N\x00\x00\x00\x00\x00\x01\x00\x01\x88\xed\
+\x00\x00\x02\x8a\x00\x00\x00\x00\x00\x01\x00\x01[)\
+\x00\x00\x01\x8f\xd9M\xfc\x1e\
+\x00\x00\x05N\x00\x00\x00\x00\x00\x01\x00\x01\x88\xec\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x03N\x00\x00\x00\x00\x00\x01\x00\x01l\xa4\
+\x00\x00\x03N\x00\x00\x00\x00\x00\x01\x00\x01l\xa3\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x03\xd0\x00\x00\x00\x00\x00\x01\x00\x01sJ\
+\x00\x00\x03\xd0\x00\x00\x00\x00\x00\x01\x00\x01sI\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x02\x16\x00\x00\x00\x00\x00\x01\x00\x01\x06\x5c\
+\x00\x00\x02\x16\x00\x00\x00\x00\x00\x01\x00\x01\x06[\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x02f\x00\x00\x00\x00\x00\x01\x00\x01Y\x85\
+\x00\x00\x02f\x00\x00\x00\x00\x00\x01\x00\x01Y\x84\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x05\xe0\x00\x00\x00\x00\x00\x01\x00\x01\x92\x07\
+\x00\x00\x05\xe0\x00\x00\x00\x00\x00\x01\x00\x01\x92\x06\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x03\xfe\x00\x00\x00\x00\x00\x01\x00\x01v\xe3\
+\x00\x00\x03\xfe\x00\x00\x00\x00\x00\x01\x00\x01v\xe2\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x02\xb2\x00\x00\x00\x00\x00\x01\x00\x01]\xef\
+\x00\x00\x02\xb2\x00\x00\x00\x00\x00\x01\x00\x01]\xee\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x04\xc6\x00\x00\x00\x00\x00\x01\x00\x01\x82\xcc\
+\x00\x00\x04\xc6\x00\x00\x00\x00\x00\x01\x00\x01\x82\xcb\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x01.\x00\x00\x00\x00\x00\x01\x00\x00\xf1\xa4\
+\x00\x00\x01.\x00\x00\x00\x00\x00\x01\x00\x00\xf1\xa3\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x03z\x00\x00\x00\x00\x00\x01\x00\x01n\xa3\
-\x00\x00\x01\x8f\xc0\x8dE\xe5\
-\x00\x00\x04\xf8\x00\x00\x00\x00\x00\x01\x00\x01\x84\xde\
+\x00\x00\x03z\x00\x00\x00\x00\x00\x01\x00\x01n\xa2\
+\x00\x00\x01\x8f\xd9M\xfc\x1e\
+\x00\x00\x04\xf8\x00\x00\x00\x00\x00\x01\x00\x01\x84\xdd\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x05\x18\x00\x00\x00\x00\x00\x01\x00\x01\x87\xd6\
+\x00\x00\x05\x18\x00\x00\x00\x00\x00\x01\x00\x01\x87\xd5\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x04\x5c\x00\x00\x00\x00\x00\x01\x00\x01|#\
+\x00\x00\x04\x5c\x00\x00\x00\x00\x00\x01\x00\x01|\x22\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x044\x00\x00\x00\x00\x00\x01\x00\x01yB\
+\x00\x00\x044\x00\x00\x00\x00\x00\x01\x00\x01yA\
 \x00\x00\x01\x8dp\x13\x90\xf8\
 \x00\x00\x00\xa4\x00\x02\x00\x00\x00\x02\x00\x00\x001\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x06p\x00\x02\x00\x00\x00\x01\x00\x00\x000\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x06z\x00\x00\x00\x00\x00\x01\x00\x01\x9a\xc8\
+\x00\x00\x06z\x00\x00\x00\x00\x00\x01\x00\x01\x9a\xc7\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x06\xc6\x00\x00\x00\x00\x00\x01\x00\x01\xa8\xda\
+\x00\x00\x06\xc6\x00\x00\x00\x00\x00\x01\x00\x01\xa8\xd9\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x06\xa0\x00\x00\x00\x00\x00\x01\x00\x01\xa6{\
+\x00\x00\x06\xa0\x00\x00\x00\x00\x00\x01\x00\x01\xa6z\
 \x00\x00\x01\x8dp\x13\x90\xf8\
 \x00\x00\x00\xa4\x00\x02\x00\x00\x00\x05\x00\x00\x004\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x07V\x00\x00\x00\x00\x00\x01\x00\x01\xb1\xd5\
+\x00\x00\x07V\x00\x00\x00\x00\x00\x01\x00\x01\xb1\xd4\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x07x\x00\x00\x00\x00\x00\x01\x00\x01\xb4;\
+\x00\x00\x07x\x00\x00\x00\x00\x00\x01\x00\x01\xb4:\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x076\x00\x00\x00\x00\x00\x01\x00\x01\xafs\
+\x00\x00\x076\x00\x00\x00\x00\x00\x01\x00\x01\xafr\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x06\xe8\x00\x00\x00\x00\x00\x01\x00\x01\xaa\xaf\
+\x00\x00\x06\xe8\x00\x00\x00\x00\x00\x01\x00\x01\xaa\xae\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x07\x0a\x00\x00\x00\x00\x00\x01\x00\x01\xad\x11\
+\x00\x00\x07\x0a\x00\x00\x00\x00\x00\x01\x00\x01\xad\x10\
 \x00\x00\x01\x8dp\x13\x90\xf8\
 \x00\x00\x00f\x00\x02\x00\x00\x00\x01\x00\x00\x00h\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00~\x00\x02\x00\x00\x00\x02\x00\x00\x00c\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x90\x00\x02\x00\x00\x00\x01\x00\x00\x00=\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00J\x00\x04\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x8f\xc0\x8dE\xe5\
+\x00\x00\x01\x8f\xd9M\xfc\x1e\
 \x00\x00\x00\xa4\x00\x02\x00\x00\x00%\x00\x00\x00>\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\xbe\x00\x00\x00\x00\x00\x01\x00\x00$\x90\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x01x\x00\x00\x00\x00\x00\x01\x00\x00\x1eb\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x00\xae\x00\x00\x00\x00\x00\x01\x00\x00\x0e(\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x04~\x00\x00\x00\x00\x00\x01\x00\x00\xa3'\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x04\x9e\x00\x00\x00\x00\x00\x01\x00\x00\xa58\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x03\x02\x00\x00\x00\x00\x00\x01\x00\x00\x8c\x0c\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x01P\x00\x00\x00\x00\x00\x01\x00\x00\x19\x88\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x05\xb8\x00\x00\x00\x00\x00\x01\x00\x00\xb3k\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x02\xda\x00\x00\x00\x00\x00\x01\x00\x00\x85\x92\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x03\xa2\x00\x00\x00\x00\x00\x01\x00\x00\x96\x0d\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x06\x06\x00\x00\x00\x00\x00\x01\x00\x00\xb8\x89\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x03\x1e\x00\x00\x00\x00\x00\x01\x00\x00\x8e\xd5\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x062\x00\x00\x00\x00\x00\x01\x00\x00\xba\x81\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x06R\x00\x00\x00\x00\x00\x01\x00\x00\xbc{\
-\x00\x00\x01\x8f\xc0\x8dE\xe5\
-\x00\x00\x01\x00\x00\x00\x00\x00\x00\x01\x00\x00\x13\xa1\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x01\xf0\x00\x00\x00\x00\x00\x01\x00\x00)\xc8\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x05l\x00\x00\x00\x00\x00\x01\x00\x00\xafI\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x01\x9e\x00\x00\x00\x00\x00\x01\x00\x00 \xb5\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x02F\x00\x00\x00\x00\x00\x01\x00\x00|\xfa\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x05\x8a\x00\x00\x00\x00\x00\x01\x00\x00\xb1\xa6\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\x10Q\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x02\x8a\x00\x00\x00\x00\x00\x01\x00\x00\x80\xe6\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x05N\x00\x00\x00\x00\x00\x01\x00\x00\xad_\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x03N\x00\x00\x00\x00\x00\x01\x00\x00\x91\x16\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x03\xd0\x00\x00\x00\x00\x00\x01\x00\x00\x97\xc8\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x02\x16\x00\x00\x00\x00\x00\x01\x00\x00,=\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x02f\x00\x00\x00\x00\x00\x01\x00\x00\x7fK\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x05\xe0\x00\x00\x00\x00\x00\x01\x00\x00\xb6g\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x03\xfe\x00\x00\x00\x00\x00\x01\x00\x00\x9b]\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x02\xb2\x00\x00\x00\x00\x00\x01\x00\x00\x83\xb4\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x04\xc6\x00\x00\x00\x00\x00\x01\x00\x00\xa7F\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x01.\x00\x00\x00\x00\x00\x01\x00\x00\x17\x8e\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x03z\x00\x00\x00\x00\x00\x01\x00\x00\x93\x1c\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x04\xf8\x00\x00\x00\x00\x00\x01\x00\x00\xa9O\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x05\x18\x00\x00\x00\x00\x00\x01\x00\x00\xacA\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x04\x5c\x00\x00\x00\x00\x00\x01\x00\x00\xa0\x95\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
-\x00\x00\x044\x00\x00\x00\x00\x00\x01\x00\x00\x9d\xb8\
-\x00\x00\x01\x8f\xc0\x8dE\xe1\
+\x00\x00\x01\xbe\x00\x00\x00\x00\x00\x01\x00\x00$\x91\
+\x00\x00\x01\x8f\xd9M\xfc\x17\
+\x00\x00\x01x\x00\x00\x00\x00\x00\x01\x00\x00\x1ec\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x00\xae\x00\x00\x00\x00\x00\x01\x00\x00\x0e)\
+\x00\x00\x01\x8f\xd9M\xfc\x14\
+\x00\x00\x04~\x00\x00\x00\x00\x00\x01\x00\x00\xa3(\
+\x00\x00\x01\x8f\xd9M\xfc\x17\
+\x00\x00\x04\x9e\x00\x00\x00\x00\x00\x01\x00\x00\xa59\
+\x00\x00\x01\x8f\xd9M\xfc\x14\
+\x00\x00\x03\x02\x00\x00\x00\x00\x00\x01\x00\x00\x8c\x0d\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x01P\x00\x00\x00\x00\x00\x01\x00\x00\x19\x89\
+\x00\x00\x01\x8f\xd9M\xfc\x17\
+\x00\x00\x05\xb8\x00\x00\x00\x00\x00\x01\x00\x00\xb3l\
+\x00\x00\x01\x8f\xd9M\xfc\x14\
+\x00\x00\x02\xda\x00\x00\x00\x00\x00\x01\x00\x00\x85\x93\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x03\xa2\x00\x00\x00\x00\x00\x01\x00\x00\x96\x0e\
+\x00\x00\x01\x8f\xd9M\xfc\x14\
+\x00\x00\x06\x06\x00\x00\x00\x00\x00\x01\x00\x00\xb8\x8a\
+\x00\x00\x01\x8f\xd9M\xfc\x14\
+\x00\x00\x03\x1e\x00\x00\x00\x00\x00\x01\x00\x00\x8e\xd6\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x062\x00\x00\x00\x00\x00\x01\x00\x00\xba\x82\
+\x00\x00\x01\x8f\xd9M\xfc\x17\
+\x00\x00\x06R\x00\x00\x00\x00\x00\x01\x00\x00\xbc|\
+\x00\x00\x01\x8f\xd9M\xfc\x1e\
+\x00\x00\x01\x00\x00\x00\x00\x00\x00\x01\x00\x00\x13\xa2\
+\x00\x00\x01\x8f\xd9M\xfc\x14\
+\x00\x00\x01\xf0\x00\x00\x00\x00\x00\x01\x00\x00)\xc9\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x05l\x00\x00\x00\x00\x00\x01\x00\x00\xafJ\
+\x00\x00\x01\x8f\xd9M\xfc\x17\
+\x00\x00\x01\x9e\x00\x00\x00\x00\x00\x01\x00\x00 \xb6\
+\x00\x00\x01\x8f\xd9M\xfc\x14\
+\x00\x00\x02F\x00\x00\x00\x00\x00\x01\x00\x00|\xfb\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x05\x8a\x00\x00\x00\x00\x00\x01\x00\x00\xb1\xa7\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x00\xda\x00\x00\x00\x00\x00\x01\x00\x00\x10R\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x02\x8a\x00\x00\x00\x00\x00\x01\x00\x00\x80\xe7\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x05N\x00\x00\x00\x00\x00\x01\x00\x00\xad`\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x03N\x00\x00\x00\x00\x00\x01\x00\x00\x91\x17\
+\x00\x00\x01\x8f\xd9M\xfc\x14\
+\x00\x00\x03\xd0\x00\x00\x00\x00\x00\x01\x00\x00\x97\xc9\
+\x00\x00\x01\x8f\xd9M\xfc\x14\
+\x00\x00\x02\x16\x00\x00\x00\x00\x00\x01\x00\x00,>\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x02f\x00\x00\x00\x00\x00\x01\x00\x00\x7fL\
+\x00\x00\x01\x8f\xd9M\xfc\x17\
+\x00\x00\x05\xe0\x00\x00\x00\x00\x00\x01\x00\x00\xb6h\
+\x00\x00\x01\x8f\xd9M\xfc\x14\
+\x00\x00\x03\xfe\x00\x00\x00\x00\x00\x01\x00\x00\x9b^\
+\x00\x00\x01\x8f\xd9M\xfc\x14\
+\x00\x00\x02\xb2\x00\x00\x00\x00\x00\x01\x00\x00\x83\xb5\
+\x00\x00\x01\x8f\xd9M\xfc\x17\
+\x00\x00\x04\xc6\x00\x00\x00\x00\x00\x01\x00\x00\xa7G\
+\x00\x00\x01\x8f\xd9M\xfc\x17\
+\x00\x00\x01.\x00\x00\x00\x00\x00\x01\x00\x00\x17\x8f\
+\x00\x00\x01\x8f\xd9M\xfc\x17\
+\x00\x00\x03z\x00\x00\x00\x00\x00\x01\x00\x00\x93\x1d\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x04\xf8\x00\x00\x00\x00\x00\x01\x00\x00\xa9P\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x05\x18\x00\x00\x00\x00\x00\x01\x00\x00\xacB\
+\x00\x00\x01\x8f\xd9M\xfc\x1b\
+\x00\x00\x04\x5c\x00\x00\x00\x00\x00\x01\x00\x00\xa0\x96\
+\x00\x00\x01\x8f\xd9M\xfc\x17\
+\x00\x00\x044\x00\x00\x00\x00\x00\x01\x00\x00\x9d\xb9\
+\x00\x00\x01\x8f\xd9M\xfc\x17\
 \x00\x00\x00\xa4\x00\x02\x00\x00\x00\x02\x00\x00\x00f\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x06p\x00\x02\x00\x00\x00\x01\x00\x00\x00e\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x06z\x00\x00\x00\x00\x00\x01\x00\x00\xbf0\
+\x00\x00\x06z\x00\x00\x00\x00\x00\x01\x00\x00\xbf1\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x06\xc6\x00\x00\x00\x00\x00\x01\x00\x00\xcdI\
-\x00\x00\x01\x8f\xc0\x8dE\xe5\
-\x00\x00\x06\xa0\x00\x00\x00\x00\x00\x01\x00\x00\xca\xe3\
-\x00\x00\x01\x8f\xc0\x8dE\xe5\
+\x00\x00\x06\xc6\x00\x00\x00\x00\x00\x01\x00\x00\xcdJ\
+\x00\x00\x01\x8f\xd9M\xfc\x1e\
+\x00\x00\x06\xa0\x00\x00\x00\x00\x00\x01\x00\x00\xca\xe4\
+\x00\x00\x01\x8f\xd9M\xfc\x1e\
 \x00\x00\x00\xa4\x00\x02\x00\x00\x00\x05\x00\x00\x00i\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x07V\x00\x00\x00\x00\x00\x01\x00\x00\xd6K\
+\x00\x00\x07V\x00\x00\x00\x00\x00\x01\x00\x00\xd6L\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x07x\x00\x00\x00\x00\x00\x01\x00\x00\xd8\xb1\
+\x00\x00\x07x\x00\x00\x00\x00\x00\x01\x00\x00\xd8\xb2\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x076\x00\x00\x00\x00\x00\x01\x00\x00\xd3\xe9\
+\x00\x00\x076\x00\x00\x00\x00\x00\x01\x00\x00\xd3\xea\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x06\xe8\x00\x00\x00\x00\x00\x01\x00\x00\xcf%\
+\x00\x00\x06\xe8\x00\x00\x00\x00\x00\x01\x00\x00\xcf&\
 \x00\x00\x01\x8dp\x13\x90\xf8\
-\x00\x00\x07\x0a\x00\x00\x00\x00\x00\x01\x00\x00\xd1\x87\
+\x00\x00\x07\x0a\x00\x00\x00\x00\x00\x01\x00\x00\xd1\x88\
 \x00\x00\x01\x8dp\x13\x90\xf8\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
```

### Comparing `pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_themes.py` & `pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_themes.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 \x91~\xf1E=IOR\xbf9\xab\xba\x9a\xbar\xcf\
 5\x0f\x91^\xc3\xf8$\xa7N\x07%\x98\x9c\xfcu^\
 \xf5i\xbb<*\x92\xb4\xda\x05qhXZ\xc5\xb2|\
 \xad\xe4/\xdf`\x874\xce\xf5\x03\xe0C\xff\xb7 \x1f\
 \xfb\x8d%\xa1~\xbf\xbe\xe2c\xaf:+\x0fv\x04\x9b\
 zN\xea\x0av\xfc\xfc\xa4tf\xa6\xd6Nbd\xa0\
 \x91\x11E\x8e\x10\x11\x83\x82J\xa1\x030\x88\x04\xc6\xc6\
-N\x07B$\xec\xa8\xe1\x9c\xc4\xd8\xfa}8\xd5\xd1\x9d\
+N\x07B:\xec\xa2A\x9cD\xd3\x9a|d\xd51\x9b\
 \xda\x0bT\xceU[\xb3\x87\x9ao\x89Y\x97>\xd9\x0c\
 \xc9\xb02\xe0\x8d\x972'`\x06\xae\x02hz\xfd\xbf\
 1e1U\x99\xa8Z\xe4\xaa\x90\x11o\x99\xed\xda\xb5\
 |\x10\xd5.\xa2\xaa5\xb06D\xde\x0d\x8a-D\xe3\
 \xc7.M\xc6\x8d\x94Y\x9eiS\xadx\x85\xb3\x9a)\
 \x84\xd9\xcf\xe4\x896\x85\x09/fE\x22R\xd92\x10\
 \xeeF\xcc\x9970\x06\x08\x08\x88-\xb0\xb9dop\
```

### Comparing `pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_translations.py` & `pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_translations.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_windows_icons.py` & `pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_windows_icons.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_windows_theme_icons.py` & `pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_windows_theme_icons.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_windows_themes.py` & `pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_windows_themes.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/rc_generated_files/rc_windows_translations.py` & `pcleaner-2.7.1/pcleaner/gui/rc_generated_files/rc_windows_translations.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/setup_greeter_driver.py` & `pcleaner-2.7.1/pcleaner/gui/setup_greeter_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/structures.py` & `pcleaner-2.7.1/pcleaner/gui/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/supported_languages.py` & `pcleaner-2.7.1/pcleaner/gui/supported_languages.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_About.py` & `pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_About.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py` & `pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_ErrorDialog.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py` & `pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_FileManagerIntegration.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_ImageDetails.py` & `pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_ImageDetails.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_IssueReporter.py` & `pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_IssueReporter.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_License.py` & `pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_License.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_Mainwindow.py` & `pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_Mainwindow.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py` & `pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_ModelDownloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_NewProfile.py` & `pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_NewProfile.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py` & `pcleaner-2.7.1/pcleaner/gui/ui_generated_files/ui_SetupGreeter.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/gui/worker_thread.py` & `pcleaner-2.7.1/pcleaner/gui/worker_thread.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/helpers.py` & `pcleaner-2.7.1/pcleaner/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import difflib
 import platform
 from enum import Enum
 import subprocess
 from itertools import takewhile, groupby
 from pathlib import Path
-import PySide6.QtCore as Qc
 
 import tifffile
 from loguru import logger
 
+try:
+    import PySide6.QtCore as Qc
+except ImportError:
+    Qc = None
+
 
 def tr(
     text: str,
     disambiguation: str | None = None,
     context: str = "",
     count: int = -1,
 ) -> str:
     """
     Translate a string to the current locale.
     """
+    if Qc is None:
+        return text
     return Qc.QCoreApplication.translate(context, text, disambiguation, count)
 
 
 def f_plural(value, singular: str, plural: str) -> str:
     """
     Selects which form to use based on the value.
     """
```

### Comparing `pcleaner-2.7.0/pcleaner/image_ops.py` & `pcleaner-2.7.1/pcleaner/image_ops.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/inpainting.py` & `pcleaner-2.7.1/pcleaner/inpainting.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/main.py` & `pcleaner-2.7.1/pcleaner/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
                                     but still run the cleaning process using the settings from the profile
                                     called myprofile2. This can be useful when you tweaked settings only
                                     related to the cleaning process. You can save time skipping the first one
                                     or two steps, since the results are saved in the cache directory (unless
                                     you choose to delete them).
 
 """
+
 import sys
 import csv
 import itertools
 import multiprocessing
 import platform
 import time
 from multiprocessing import Pool
@@ -128,15 +129,14 @@
 from tqdm import tqdm
 
 import pcleaner.analytics as an
 import pcleaner.cli_utils as cli
 import pcleaner.config as cfg
 import pcleaner.denoiser as dn
 import pcleaner.inpainting as ip
-import pcleaner.gui.launcher as gui
 import pcleaner.helpers as hp
 import pcleaner.masker as ma
 import pcleaner.model_downloader as md
 import pcleaner.preprocessor as pp
 import pcleaner.profile_cli as pc
 import pcleaner.structures as st
 import pcleaner.ocr.ocr as ocr
@@ -272,15 +272,31 @@
             # Prevent this fom getting too long.
             hp.send_desktop_notification("Cleaning complete.", f"Cleaned: {img_paths}")
 
     else:
         # Launch the GUI. Either the user specified it, or no command was given.
         # This is done so that a bundled executable can be launched in gui mode without a command,
         # without hindering access to the cli.
-        gui.launch(args.image_path, args.debug)
+        try:
+            import pcleaner.gui.launcher as gui
+        except ImportError:
+            if not args.gui:
+                print(
+                    "This is the CLI version of Panel Cleaner. "
+                    "Calling pcleaner-cli without any arguments will attempt to launch the GUI. "
+                    "Please install the GUI version 'pcleaner' to use the GUI."
+                )
+            else:
+                print(
+                    "The GUI version of Panel Cleaner is not installed. "
+                    "Please install the GUI version 'pcleaner' to use the GUI."
+                )
+            sys.exit(1)
+        else:
+            gui.launch(args.image_path, args.debug)
 
 
 def run_cleaner(
     image_paths: list[Path],
     output_dir: Path,
     config: cfg.Config,
     skip_text_detection: bool,
```

### Comparing `pcleaner-2.7.0/pcleaner/masker.py` & `pcleaner-2.7.1/pcleaner/masker.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/model_downloader.py` & `pcleaner-2.7.1/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/ocr/ocr.py` & `pcleaner-2.7.1/pcleaner/ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/ocr/ocr_mangaocr.py` & `pcleaner-2.7.1/pcleaner/ocr/ocr_mangaocr.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/ocr/ocr_tesseract.py` & `pcleaner-2.7.1/pcleaner/ocr/ocr_tesseract.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/preprocessor.py` & `pcleaner-2.7.1/pcleaner/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/profile_cli.py` & `pcleaner-2.7.1/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner/structures.py` & `pcleaner-2.7.1/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/pcleaner.egg-info/PKG-INFO` & `pcleaner-2.7.1/pcleaner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
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
 
@@ -94,15 +95,15 @@
 
 ## Features
 
 - Cleans text bubbles without leaving artifacts.
 
 - Avoids painting over parts of the image that aren't text.
 
-- Inpaints bubbles that can't simply be masked out.
+- Inpaints bubbles (with LaMa machine learning) that can't simply be masked out.
 
 - Ignores bubbles containing only symbols or numbers, as those don't need translation.
 
 - Offers a GUI for easy use, dark, light, and system themes are supported.
 
 - No internet connection required after installing the model data.
 
@@ -117,15 +118,15 @@
 
 - Can handle bubbles on any solid grayscale background color.
 
 - Can also cut out the text from the rest of the image, e.g. to paste it over a colored rendition.
 
 - Can also run OCR on the pages and output the text to a file.
 
-- Interface available in: English, German (See [Translating](https://github.com/VoxelCubes/PanelCleaner/blob/master/translations/TRANSLATING.md) for more languages)
+- Interface available in: English, German, Bulgarian (See [Translating](https://github.com/VoxelCubes/PanelCleaner/blob/master/translations/TRANSLATING.md) for more languages)
 
 
 ## Limitations
 
 - It only supports Japanese and English text for cleaning (success may vary with other languages), Japanese only for OCR.
 
 - Supported file types: .jpeg, .jpg, .png, .bmp, .tiff, .tif, .jp2, .dib, .webp, .ppm
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

### Comparing `pcleaner-2.7.0/pcleaner.egg-info/SOURCES.txt` & `pcleaner-2.7.1/pcleaner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcleaner-2.7.0/setup.cfg` & `pcleaner-2.7.1/setup.cfg`

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

### Comparing `pcleaner-2.7.0/tests/test_log_parser.py` & `pcleaner-2.7.1/tests/test_log_parser.py`

 * *Files identical despite different names*

