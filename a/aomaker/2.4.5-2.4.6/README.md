# Comparing `tmp/aomaker-2.4.5.tar.gz` & `tmp/aomaker-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aomaker-2.4.5.tar", last modified: Mon Dec 25 09:03:23 2023, max compression
+gzip compressed data, was "aomaker-2.4.6.tar", last modified: Sun Jun  2 13:44:26 2024, max compression
```

## Comparing `aomaker-2.4.5.tar` & `aomaker-2.4.6.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.949289 aomaker-2.4.5/
--rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.4.5/LICENSE
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       43 2023-05-20 11:36:28.000000 aomaker-2.4.5/MANIFEST.in
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     6799 2023-12-25 09:03:23.949149 aomaker-2.4.5/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     6368 2023-10-12 09:40:29.000000 aomaker-2.4.5/README.md
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.943508 aomaker-2.4.5/aomaker/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2023-12-25 09:03:22.000000 aomaker-2.4.5/aomaker/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    11527 2023-10-08 05:59:36.000000 aomaker-2.4.5/aomaker/_aomaker.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      688 2023-08-01 15:01:49.000000 aomaker-2.4.5/aomaker/_constants.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/_log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1245 2023-09-05 08:05:08.000000 aomaker-2.4.5/aomaker/_printer.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      358 2023-12-04 02:28:21.000000 aomaker-2.4.5/aomaker/aomaker.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.944901 aomaker-2.4.5/aomaker/base/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/base/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7346 2023-09-15 09:23:55.000000 aomaker-2.4.5/aomaker/base/base_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/base/base_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     6139 2023-05-29 14:52:36.000000 aomaker-2.4.5/aomaker/cache.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    11247 2023-12-20 05:59:24.000000 aomaker-2.4.5/aomaker/cli.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.945551 aomaker-2.4.5/aomaker/database/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/database/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      997 2023-08-01 14:59:09.000000 aomaker-2.4.5/aomaker/database/mysql.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3749 2023-08-01 14:49:32.000000 aomaker-2.4.5/aomaker/database/sqlite.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1685 2023-05-29 14:39:13.000000 aomaker-2.4.5/aomaker/exceptions.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.945775 aomaker-2.4.5/aomaker/extension/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/extension/__init__.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.946096 aomaker-2.4.5/aomaker/extension/har_parse/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.4.5/aomaker/extension/har_parse/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/extension/har_parse/har_parse.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.946663 aomaker-2.4.5/aomaker/extension/recording/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.4.5/aomaker/extension/recording/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      134 2023-10-19 14:51:30.000000 aomaker-2.4.5/aomaker/extension/recording/addons.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2023-10-20 08:45:37.000000 aomaker-2.4.5/aomaker/extension/recording/recording.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.947107 aomaker-2.4.5/aomaker/extension/retry/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2023-09-13 07:48:44.000000 aomaker-2.4.5/aomaker/extension/retry/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1755 2023-09-15 06:40:13.000000 aomaker-2.4.5/aomaker/extension/retry/retry.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/field.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2624 2023-09-05 07:01:36.000000 aomaker-2.4.5/aomaker/fixture.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-12-04 02:28:10.000000 aomaker-2.4.5/aomaker/hook_manager.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.947760 aomaker-2.4.5/aomaker/html/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.4.5/aomaker/html/heading.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.4.5/aomaker/html/report.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2023-05-20 11:43:25.000000 aomaker-2.4.5/aomaker/html/template.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4639 2023-12-25 09:01:09.000000 aomaker-2.4.5/aomaker/log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/make.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/make_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/make_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2112 2023-09-05 08:04:36.000000 aomaker-2.4.5/aomaker/models.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      503 2023-06-13 10:28:50.000000 aomaker-2.4.5/aomaker/param_types.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      803 2023-09-15 04:26:34.000000 aomaker-2.4.5/aomaker/path.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2890 2023-05-20 14:38:18.000000 aomaker-2.4.5/aomaker/report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8513 2023-06-28 06:57:49.000000 aomaker-2.4.5/aomaker/runner.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8630 2023-10-19 14:42:23.000000 aomaker-2.4.5/aomaker/scaffold.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.948194 aomaker-2.4.5/aomaker/send_msg/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/send_msg/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4795 2023-10-10 06:49:17.000000 aomaker-2.4.5/aomaker/send_msg/wechat.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7587 2023-08-01 15:23:26.000000 aomaker-2.4.5/aomaker/swagger2yaml.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/template.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.948847 aomaker-2.4.5/aomaker/utils/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.4.5/aomaker/utils/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9529 2023-05-22 08:33:10.000000 aomaker-2.4.5/aomaker/utils/gen_allure_report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.4.5/aomaker/utils/utils.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    16507 2023-10-20 14:55:37.000000 aomaker-2.4.5/aomaker/yaml2case.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-12-25 09:03:23.944372 aomaker-2.4.5/aomaker.egg-info/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     6799 2023-12-25 09:03:23.000000 aomaker-2.4.5/aomaker.egg-info/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1390 2023-12-25 09:03:23.000000 aomaker-2.4.5/aomaker.egg-info/SOURCES.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2023-12-25 09:03:23.000000 aomaker-2.4.5/aomaker.egg-info/dependency_links.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2023-12-25 09:03:23.000000 aomaker-2.4.5/aomaker.egg-info/entry_points.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      302 2023-12-25 09:03:23.000000 aomaker-2.4.5/aomaker.egg-info/requires.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2023-12-25 09:03:23.000000 aomaker-2.4.5/aomaker.egg-info/top_level.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2023-12-25 09:03:23.949330 aomaker-2.4.5/setup.cfg
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1462 2023-12-25 09:03:22.000000 aomaker-2.4.5/setup.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.816707 aomaker-2.4.6/
+-rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.4.6/LICENSE
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       49 2024-04-25 14:22:21.000000 aomaker-2.4.6/MANIFEST.in
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     6799 2024-06-02 13:44:26.816544 aomaker-2.4.6/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     6368 2023-10-12 09:40:29.000000 aomaker-2.4.6/README.md
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.808606 aomaker-2.4.6/aomaker/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2024-06-02 13:43:55.000000 aomaker-2.4.6/aomaker/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    11651 2024-06-02 13:43:55.000000 aomaker-2.4.6/aomaker/_aomaker.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      688 2024-06-02 13:27:45.000000 aomaker-2.4.6/aomaker/_constants.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/_log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1245 2023-09-05 08:05:08.000000 aomaker-2.4.6/aomaker/_printer.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      358 2023-12-04 02:28:21.000000 aomaker-2.4.6/aomaker/aomaker.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.810352 aomaker-2.4.6/aomaker/base/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/base/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7475 2024-06-02 13:37:19.000000 aomaker-2.4.6/aomaker/base/base_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/base/base_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     6139 2024-06-02 13:27:45.000000 aomaker-2.4.6/aomaker/cache.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    11247 2024-06-02 13:27:45.000000 aomaker-2.4.6/aomaker/cli.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.811186 aomaker-2.4.6/aomaker/database/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/database/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      997 2023-08-01 14:59:09.000000 aomaker-2.4.6/aomaker/database/mysql.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3749 2024-06-02 13:27:45.000000 aomaker-2.4.6/aomaker/database/sqlite.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1685 2023-05-29 14:39:13.000000 aomaker-2.4.6/aomaker/exceptions.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.811369 aomaker-2.4.6/aomaker/extension/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/extension/__init__.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.811756 aomaker-2.4.6/aomaker/extension/har_parse/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.4.6/aomaker/extension/har_parse/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/extension/har_parse/har_parse.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.812759 aomaker-2.4.6/aomaker/extension/recording/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.4.6/aomaker/extension/recording/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      134 2023-10-19 14:51:30.000000 aomaker-2.4.6/aomaker/extension/recording/addons.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2023-10-20 08:45:37.000000 aomaker-2.4.6/aomaker/extension/recording/recording.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.813427 aomaker-2.4.6/aomaker/extension/retry/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2023-09-13 07:48:44.000000 aomaker-2.4.6/aomaker/extension/retry/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1755 2023-09-15 06:40:13.000000 aomaker-2.4.6/aomaker/extension/retry/retry.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/field.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2624 2023-09-05 07:01:36.000000 aomaker-2.4.6/aomaker/fixture.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-12-04 02:28:10.000000 aomaker-2.4.6/aomaker/hook_manager.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.814458 aomaker-2.4.6/aomaker/html/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      131 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/html/AOReporter_logo.png
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.4.6/aomaker/html/heading.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.4.6/aomaker/html/report.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2023-05-20 11:43:25.000000 aomaker-2.4.6/aomaker/html/template.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4639 2024-06-02 13:27:45.000000 aomaker-2.4.6/aomaker/log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/make.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/make_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/make_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2112 2023-09-05 08:04:36.000000 aomaker-2.4.6/aomaker/models.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      503 2023-06-13 10:28:50.000000 aomaker-2.4.6/aomaker/param_types.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      803 2024-06-02 13:27:45.000000 aomaker-2.4.6/aomaker/path.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2890 2023-05-20 14:38:18.000000 aomaker-2.4.6/aomaker/report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8513 2024-06-02 13:27:45.000000 aomaker-2.4.6/aomaker/runner.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8630 2023-10-19 14:42:23.000000 aomaker-2.4.6/aomaker/scaffold.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.814993 aomaker-2.4.6/aomaker/send_msg/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/send_msg/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4795 2023-10-10 06:49:17.000000 aomaker-2.4.6/aomaker/send_msg/wechat.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7587 2023-08-01 15:23:26.000000 aomaker-2.4.6/aomaker/swagger2yaml.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/template.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.816100 aomaker-2.4.6/aomaker/utils/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.4.6/aomaker/utils/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9529 2024-06-02 13:27:45.000000 aomaker-2.4.6/aomaker/utils/gen_allure_report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.4.6/aomaker/utils/utils.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    16507 2023-10-20 14:55:37.000000 aomaker-2.4.6/aomaker/yaml2case.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2024-06-02 13:44:26.809725 aomaker-2.4.6/aomaker.egg-info/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     6799 2024-06-02 13:44:26.000000 aomaker-2.4.6/aomaker.egg-info/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1423 2024-06-02 13:44:26.000000 aomaker-2.4.6/aomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2024-06-02 13:44:26.000000 aomaker-2.4.6/aomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2024-06-02 13:44:26.000000 aomaker-2.4.6/aomaker.egg-info/entry_points.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      318 2024-06-02 13:44:26.000000 aomaker-2.4.6/aomaker.egg-info/requires.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2024-06-02 13:44:26.000000 aomaker-2.4.6/aomaker.egg-info/top_level.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2024-06-02 13:44:26.816752 aomaker-2.4.6/setup.cfg
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1548 2024-06-02 13:44:21.000000 aomaker-2.4.6/setup.py
```

### Comparing `aomaker-2.4.5/LICENSE` & `aomaker-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/PKG-INFO` & `aomaker-2.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.4.5
+Version: 2.4.6
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.4.5/README.md` & `aomaker-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/__init__.py` & `aomaker-2.4.6/aomaker/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from emoji import emojize
 
-__version__ = "2.4.5"
+__version__ = "2.4.6"
 __description__ = "Quickly Arrange,Quickly Test!"
 __image__ = emojize(fr"""
               :----.                                                             ::::
              .------            .:::::::::::::::::::::::::::::::::::::::::::::. :---:  ::::::::::::::::::::::::::
             .---::--:                                                           ----
             ----  :--:          ..::::.      :.:..::::  .::::     ..:::. .:::  :---: ...:.    .::::.     .:.:..::
            :---    :::        .---------:   :-----------------   :----------:  ----.:---:   :---::---:   -------:
```

### Comparing `aomaker-2.4.5/aomaker/_aomaker.py` & `aomaker-2.4.6/aomaker/_aomaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,18 @@
                 if job_id is None:
                     if condition is None:
                         raise JsonPathExtractFailed(res=resp, jsonpath_expr=jsonpath_expr)
                     return resp
 
                 logger.info(
                     f"==========后置异步接口断言开始<{func.__name__}>: 轮询函数<{cycle_func.__name__}>==========")
-                cycle_func(job_id, *out_args, **out_kwargs)
+                async_res = cycle_func(job_id, *out_args, **out_kwargs)
+                if async_res:
+                    resp["async_res"] = async_res
+                    return resp
                 logger.info(f"==========后置异步接口断言结束<{func.__name__}>==========")
             else:
                 logger.info(f"==========后置异步接口不满足执行条件，不执行<{func.__name__}>==========")
             return resp
 
         return wrapper
```

### Comparing `aomaker-2.4.5/aomaker/_constants.py` & `aomaker-2.4.6/aomaker/_constants.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/_log.py` & `aomaker-2.4.6/aomaker/_log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/_printer.py` & `aomaker-2.4.6/aomaker/_printer.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/base/base_api.py` & `aomaker-2.4.6/aomaker/base/base_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 def response_callback(payload: dict):
     def inner(response: requests.models.Response, *args, **kwargs):
         api_caller = _get_api_frame()
         caller_class_obj = api_caller.f_locals['self']
         caller_of_class = caller_class_obj.__class__.__name__
         caller_of_method = api_caller.f_code.co_name
         caller_name = f"{caller_of_class}.{caller_of_method}"
-        doc = caller_class_obj.__class__.__dict__[caller_of_method].__doc__
+        method_ref = getattr(caller_class_obj, caller_of_method, None)
+        doc = method_ref.__doc__ if method_ref and method_ref.__doc__ else ""
         doc = doc.split("\n")[0].strip() if doc else ""
         caller_name = f"{caller_name} {doc}"
 
         print_info, allure_info, std_logger = _handle_print_info(payload, response, caller_name)
 
         if response.status_code >= 400:
             logger.error(_render_template(template, print_info))
@@ -98,18 +99,19 @@
 
     return inner
 
 
 def _get_api_frame():
     current_frame = inspect.currentframe()
     outer_frames = inspect.getouterframes(current_frame)
-    for frame_info in outer_frames[8:]:
+    for frame_info in outer_frames:
         frame = frame_info.frame
+        code = frame.f_code
         filename = frame_info.filename
-        if API_DIR in filename:
+        if API_DIR in filename and code.co_name != 'send_http':
             return frame
 
 
 def _handle_print_info(request_payload, response, caller_name):
     url = request_payload.get('url')
     params = request_payload.get('params')
     req_data = request_payload.get("data")
```

### Comparing `aomaker-2.4.5/aomaker/base/base_testcase.py` & `aomaker-2.4.6/aomaker/base/base_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/cache.py` & `aomaker-2.4.6/aomaker/cache.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/cli.py` & `aomaker-2.4.6/aomaker/cli.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/database/mysql.py` & `aomaker-2.4.6/aomaker/database/mysql.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/database/sqlite.py` & `aomaker-2.4.6/aomaker/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/exceptions.py` & `aomaker-2.4.6/aomaker/exceptions.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/extension/har_parse/__init__.py` & `aomaker-2.4.6/aomaker/extension/har_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/extension/har_parse/har_parse.py` & `aomaker-2.4.6/aomaker/extension/har_parse/har_parse.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/extension/recording/__init__.py` & `aomaker-2.4.6/aomaker/extension/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/extension/recording/recording.py` & `aomaker-2.4.6/aomaker/extension/recording/recording.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/extension/retry/retry.py` & `aomaker-2.4.6/aomaker/extension/retry/retry.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/field.py` & `aomaker-2.4.6/aomaker/field.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/fixture.py` & `aomaker-2.4.6/aomaker/fixture.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/hook_manager.py` & `aomaker-2.4.6/aomaker/hook_manager.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/html/heading.html` & `aomaker-2.4.6/aomaker/html/heading.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/html/report.html` & `aomaker-2.4.6/aomaker/html/report.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/html/template.html` & `aomaker-2.4.6/aomaker/html/template.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/log.py` & `aomaker-2.4.6/aomaker/log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/make.py` & `aomaker-2.4.6/aomaker/make.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/make_api.py` & `aomaker-2.4.6/aomaker/make_api.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/make_testcase.py` & `aomaker-2.4.6/aomaker/make_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/models.py` & `aomaker-2.4.6/aomaker/models.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/path.py` & `aomaker-2.4.6/aomaker/path.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/report.py` & `aomaker-2.4.6/aomaker/report.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/runner.py` & `aomaker-2.4.6/aomaker/runner.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/scaffold.py` & `aomaker-2.4.6/aomaker/scaffold.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/send_msg/wechat.py` & `aomaker-2.4.6/aomaker/send_msg/wechat.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/swagger2yaml.py` & `aomaker-2.4.6/aomaker/swagger2yaml.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/template.py` & `aomaker-2.4.6/aomaker/template.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/utils/gen_allure_report.py` & `aomaker-2.4.6/aomaker/utils/gen_allure_report.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/utils/utils.py` & `aomaker-2.4.6/aomaker/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker/yaml2case.py` & `aomaker-2.4.6/aomaker/yaml2case.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.4.5/aomaker.egg-info/PKG-INFO` & `aomaker-2.4.6/aomaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.4.5
+Version: 2.4.6
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.4.5/aomaker.egg-info/SOURCES.txt` & `aomaker-2.4.6/aomaker.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 aomaker/extension/har_parse/__init__.py
 aomaker/extension/har_parse/har_parse.py
 aomaker/extension/recording/__init__.py
 aomaker/extension/recording/addons.py
 aomaker/extension/recording/recording.py
 aomaker/extension/retry/__init__.py
 aomaker/extension/retry/retry.py
+aomaker/html/AOReporter_logo.png
 aomaker/html/heading.html
 aomaker/html/report.html
 aomaker/html/template.html
 aomaker/send_msg/__init__.py
 aomaker/send_msg/wechat.py
 aomaker/utils/__init__.py
 aomaker/utils/gen_allure_report.py
```

### Comparing `aomaker-2.4.5/setup.py` & `aomaker-2.4.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # --coding:utf-8--
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="aomaker",
-    version="2.4.5",
+    version="2.4.6",
     author="ancientone",
     author_email="listeningsss@163.com",
     description="An api testing framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ae86sen/aomaker",
     packages=setuptools.find_packages(),
@@ -34,15 +34,18 @@
         'colorlog==6.7.0',
         'jsonschema==4.17.3',
         'genson==1.2.2',
         'click==8.1.3',
         'emoji==2.2.0',
         'click-help-colors==0.9.1',
         'tenacity==8.2.3',
-        'ruamel.yaml==0.17.21'
+        'ruamel.yaml==0.17.21',
+        'tabulate==0.9.0',
+        # 'fastapi==0.110.0',
+        # 'uvicorn==0.28.0'
 
     ],
     entry_points={
         'console_scripts': [
             'amake=aomaker.cli:main_make_alias',
             'arun=aomaker.cli:main_arun_alias',
             'arec=aomaker.cli:main_record_alias',
```

