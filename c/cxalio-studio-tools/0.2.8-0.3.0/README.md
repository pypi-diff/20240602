# Comparing `tmp/cxalio_studio_tools-0.2.8.tar.gz` & `tmp/cxalio_studio_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxalio_studio_tools-0.2.8.tar", max compression
+gzip compressed data, was "cxalio_studio_tools-0.3.0.tar", max compression
```

## Comparing `cxalio_studio_tools-0.2.8.tar` & `cxalio_studio_tools-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,61 @@
--rw-r--r--   0        0        0    35821 2023-12-06 11:01:10.654584 cxalio_studio_tools-0.2.8/LICENSE
--rw-r--r--   0        0        0     1084 2024-05-22 12:52:36.684666 cxalio_studio_tools-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2193 2024-05-22 12:53:13.675715 cxalio_studio_tools-0.2.8/README.md
--rw-r--r--   0        0        0       21 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.8/src/cx_core/__init__.py
--rw-r--r--   0        0        0      108 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.8/src/cx_core/app/__init__.py
--rw-r--r--   0        0        0      139 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.8/src/cx_core/app/abstract_app.py
--rw-r--r--   0        0        0      839 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.8/src/cx_core/app/abstract_env.py
--rw-r--r--   0        0        0     1286 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.8/src/cx_core/app/app_logger.py
--rw-r--r--   0        0        0      489 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.8/src/cx_core/app/osinfo.py
--rw-r--r--   0        0        0       57 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.8/src/cx_core/filesystem/__init__.py
--rw-r--r--   0        0        0     7200 2024-05-22 12:52:36.690771 cxalio_studio_tools-0.2.8/src/cx_core/filesystem/path_expander.py
--rw-r--r--   0        0        0     1011 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.8/src/cx_core/filesystem/path_utils.py
--rw-r--r--   0        0        0      106 2024-05-17 10:52:51.742230 cxalio_studio_tools-0.2.8/src/cx_core/misc/__init__.py
--rw-r--r--   0        0        0     2252 2024-05-17 10:52:54.540884 cxalio_studio_tools-0.2.8/src/cx_core/misc/datapackage.py
--rw-r--r--   0        0        0      185 2024-05-17 10:52:51.742230 cxalio_studio_tools-0.2.8/src/cx_core/misc/misc_utils.py
--rw-r--r--   0        0        0     2991 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.8/src/cx_core/misc/timecode.py
--rw-r--r--   0        0        0     1640 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.8/src/cx_core/misc/timepoint.py
--rw-r--r--   0        0        0      111 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.8/src/cx_core/text/__init__.py
--rw-r--r--   0        0        0      490 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.8/src/cx_core/text/code_detecting.py
--rw-r--r--   0        0        0     1425 2024-05-17 10:52:54.540884 cxalio_studio_tools-0.2.8/src/cx_core/text/tag_replacer.py
--rw-r--r--   0        0        0     1641 2024-05-17 10:52:51.744230 cxalio_studio_tools-0.2.8/src/cx_core/text/text_utils.py
--rw-r--r--   0        0        0       29 2024-05-17 10:52:51.744230 cxalio_studio_tools-0.2.8/src/cx_core/tui/__init__.py
--rw-r--r--   0        0        0      465 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.8/src/cx_core/tui/tui_elements.py
--rw-r--r--   0        0        0      102 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.8/src/cx_subtitle/__init__.py
--rw-r--r--   0        0        0     4872 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.8/src/cx_subtitle/loader.py
--rw-r--r--   0        0        0     5739 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.8/src/cx_subtitle/saver.py
--rw-r--r--   0        0        0      736 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.8/src/cx_subtitle/subtitle.py
--rw-r--r--   0        0        0     2854 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.8/src/cx_subtitle/subtitle_formatter.py
--rw-r--r--   0        0        0       35 2024-01-27 12:52:22.618965 cxalio_studio_tools-0.2.8/src/media_killer/__init__.py
--rw-r--r--   0        0        0     1554 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.8/src/media_killer/env.py
--rw-r--r--   0        0        0     3244 2024-05-17 10:52:54.540884 cxalio_studio_tools-0.2.8/src/media_killer/example_project.toml
--rw-r--r--   0        0        0      783 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.8/src/media_killer/exceptions.py
--rw-r--r--   0        0        0     5453 2024-05-17 10:52:51.747736 cxalio_studio_tools-0.2.8/src/media_killer/help.md
--rw-r--r--   0        0        0     7390 2024-05-17 10:52:54.542516 cxalio_studio_tools-0.2.8/src/media_killer/media_killer_app.py
--rw-r--r--   0        0        0     7205 2024-05-17 10:52:54.542516 cxalio_studio_tools-0.2.8/src/media_killer/mission.py
--rw-r--r--   0        0        0     1324 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.8/src/media_killer/option_package.py
--rw-r--r--   0        0        0     3489 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.8/src/media_killer/profile_loader.py
--rw-r--r--   0        0        0     1772 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.8/src/media_killer/script_writer.py
--rw-r--r--   0        0        0     3075 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.8/src/media_killer/source_adapter.py
--rw-r--r--   0        0        0     4591 2024-05-17 10:52:54.542516 cxalio_studio_tools-0.2.8/src/media_killer/task_inspector.py
--rw-r--r--   0        0        0     4246 2024-05-17 10:52:51.749742 cxalio_studio_tools-0.2.8/src/media_killer/transcoder.py
--rw-r--r--   0        0        0       30 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.2.8/src/sub_conv/__init__.py
--rw-r--r--   0        0        0     1286 2024-05-17 10:52:51.749742 cxalio_studio_tools-0.2.8/src/sub_conv/env.py
--rw-r--r--   0        0        0      360 2024-05-17 10:52:51.749742 cxalio_studio_tools-0.2.8/src/sub_conv/exceptions.py
--rw-r--r--   0        0        0     3548 2024-05-17 10:52:51.750742 cxalio_studio_tools-0.2.8/src/sub_conv/help.md
--rw-r--r--   0        0        0     5503 2024-05-17 10:52:51.750742 cxalio_studio_tools-0.2.8/src/sub_conv/subconv_app.py
--rw-r--r--   0        0        0     1857 2024-05-17 10:52:51.750742 cxalio_studio_tools-0.2.8/src/sub_conv/subtitle_translator.py
--rw-r--r--   0        0        0     6762 2024-05-17 10:52:51.751742 cxalio_studio_tools-0.2.8/src/sub_conv/worker.py
--rw-r--r--   0        0        0        0 2024-05-17 10:52:51.751742 cxalio_studio_tools-0.2.8/src/systools/__init__.py
--rw-r--r--   0        0        0      282 2024-05-17 10:52:51.753851 cxalio_studio_tools-0.2.8/src/systools/env.py
--rw-r--r--   0        0        0     3750 2024-05-17 10:52:51.753851 cxalio_studio_tools-0.2.8/src/systools/update_githubhosts.py
--rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35821 2023-12-06 11:01:10.654584 cxalio_studio_tools-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1217 2024-06-02 15:42:19.839597 cxalio_studio_tools-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2426 2024-06-02 15:42:19.838598 cxalio_studio_tools-0.3.0/README.md
+-rw-r--r--   0        0        0       21 2024-05-22 12:54:36.342481 cxalio_studio_tools-0.3.0/src/cx_core/__init__.py
+-rw-r--r--   0        0        0      108 2024-05-22 12:54:36.342994 cxalio_studio_tools-0.3.0/src/cx_core/app/__init__.py
+-rw-r--r--   0        0        0      139 2024-05-22 12:54:36.342994 cxalio_studio_tools-0.3.0/src/cx_core/app/abstract_app.py
+-rw-r--r--   0        0        0      892 2024-06-02 15:42:19.841347 cxalio_studio_tools-0.3.0/src/cx_core/app/abstract_env.py
+-rw-r--r--   0        0        0     1286 2024-05-22 12:54:36.343592 cxalio_studio_tools-0.3.0/src/cx_core/app/app_logger.py
+-rw-r--r--   0        0        0      489 2024-05-22 12:54:36.344100 cxalio_studio_tools-0.3.0/src/cx_core/app/osinfo.py
+-rw-r--r--   0        0        0       57 2024-05-22 12:54:36.344215 cxalio_studio_tools-0.3.0/src/cx_core/filesystem/__init__.py
+-rw-r--r--   0        0        0     7431 2024-06-02 15:42:19.841347 cxalio_studio_tools-0.3.0/src/cx_core/filesystem/path_expander.py
+-rw-r--r--   0        0        0     1011 2024-05-22 12:54:36.344812 cxalio_studio_tools-0.3.0/src/cx_core/filesystem/path_utils.py
+-rw-r--r--   0        0        0      106 2024-05-22 12:54:36.345323 cxalio_studio_tools-0.3.0/src/cx_core/misc/__init__.py
+-rw-r--r--   0        0        0     2252 2024-05-22 12:54:36.345323 cxalio_studio_tools-0.3.0/src/cx_core/misc/datapackage.py
+-rw-r--r--   0        0        0      185 2024-05-22 12:54:36.345323 cxalio_studio_tools-0.3.0/src/cx_core/misc/misc_utils.py
+-rw-r--r--   0        0        0     2991 2024-05-22 12:54:36.345950 cxalio_studio_tools-0.3.0/src/cx_core/misc/timecode.py
+-rw-r--r--   0        0        0     1640 2024-05-22 12:54:36.345950 cxalio_studio_tools-0.3.0/src/cx_core/misc/timepoint.py
+-rw-r--r--   0        0        0      111 2024-05-22 12:54:36.346458 cxalio_studio_tools-0.3.0/src/cx_core/text/__init__.py
+-rw-r--r--   0        0        0      490 2024-05-22 12:54:36.346458 cxalio_studio_tools-0.3.0/src/cx_core/text/code_detecting.py
+-rw-r--r--   0        0        0     1425 2024-05-22 12:54:36.347014 cxalio_studio_tools-0.3.0/src/cx_core/text/tag_replacer.py
+-rw-r--r--   0        0        0     2033 2024-06-02 15:42:19.842277 cxalio_studio_tools-0.3.0/src/cx_core/text/text_utils.py
+-rw-r--r--   0        0        0       29 2024-05-22 12:54:36.347092 cxalio_studio_tools-0.3.0/src/cx_core/tui/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-22 12:54:36.347599 cxalio_studio_tools-0.3.0/src/cx_core/tui/tui_elements.py
+-rw-r--r--   0        0        0       97 2024-06-02 15:42:19.842277 cxalio_studio_tools-0.3.0/src/cx_image/__init__.py
+-rw-r--r--   0        0        0     1222 2024-06-02 15:42:19.842277 cxalio_studio_tools-0.3.0/src/cx_image/color_processors.py
+-rw-r--r--   0        0        0     2084 2024-06-02 15:42:19.843277 cxalio_studio_tools-0.3.0/src/cx_image/image_converter.py
+-rw-r--r--   0        0        0     5316 2024-06-02 15:42:19.843277 cxalio_studio_tools-0.3.0/src/cx_image/size_processors.py
+-rw-r--r--   0        0        0      102 2024-05-22 12:54:36.348147 cxalio_studio_tools-0.3.0/src/cx_subtitle/__init__.py
+-rw-r--r--   0        0        0     4872 2024-05-22 12:54:36.348235 cxalio_studio_tools-0.3.0/src/cx_subtitle/loader.py
+-rw-r--r--   0        0        0     5739 2024-05-22 12:54:36.348830 cxalio_studio_tools-0.3.0/src/cx_subtitle/saver.py
+-rw-r--r--   0        0        0      736 2024-05-22 12:54:36.348830 cxalio_studio_tools-0.3.0/src/cx_subtitle/subtitle.py
+-rw-r--r--   0        0        0     2854 2024-05-22 12:54:36.349430 cxalio_studio_tools-0.3.0/src/cx_subtitle/subtitle_formatter.py
+-rw-r--r--   0        0        0       28 2024-06-02 15:42:19.843277 cxalio_studio_tools-0.3.0/src/jpegger/__init__.py
+-rw-r--r--   0        0        0     4934 2024-06-02 15:42:19.843277 cxalio_studio_tools-0.3.0/src/jpegger/convert_agent.py
+-rw-r--r--   0        0        0     1286 2024-06-02 15:42:19.844276 cxalio_studio_tools-0.3.0/src/jpegger/env.py
+-rw-r--r--   0        0        0     7062 2024-06-02 15:42:19.844276 cxalio_studio_tools-0.3.0/src/jpegger/help.md
+-rw-r--r--   0        0        0     6256 2024-06-02 15:42:19.844276 cxalio_studio_tools-0.3.0/src/jpegger/jpegger_app.py
+-rw-r--r--   0        0        0       35 2024-01-27 12:52:22.618965 cxalio_studio_tools-0.3.0/src/media_killer/__init__.py
+-rw-r--r--   0        0        0     1554 2024-05-22 12:54:36.349938 cxalio_studio_tools-0.3.0/src/media_killer/env.py
+-rw-r--r--   0        0        0     3244 2024-05-22 12:54:36.349938 cxalio_studio_tools-0.3.0/src/media_killer/example_project.toml
+-rw-r--r--   0        0        0      783 2024-05-22 12:54:36.350485 cxalio_studio_tools-0.3.0/src/media_killer/exceptions.py
+-rw-r--r--   0        0        0     5453 2024-05-17 10:52:51.747736 cxalio_studio_tools-0.3.0/src/media_killer/help.md
+-rw-r--r--   0        0        0     7390 2024-05-22 12:54:36.350568 cxalio_studio_tools-0.3.0/src/media_killer/media_killer_app.py
+-rw-r--r--   0        0        0     7205 2024-05-22 12:54:36.351077 cxalio_studio_tools-0.3.0/src/media_killer/mission.py
+-rw-r--r--   0        0        0     1324 2024-05-22 12:54:36.351077 cxalio_studio_tools-0.3.0/src/media_killer/option_package.py
+-rw-r--r--   0        0        0     3489 2024-05-22 12:54:36.351703 cxalio_studio_tools-0.3.0/src/media_killer/profile_loader.py
+-rw-r--r--   0        0        0     1772 2024-05-22 12:54:36.351703 cxalio_studio_tools-0.3.0/src/media_killer/script_writer.py
+-rw-r--r--   0        0        0     3075 2024-05-22 12:54:36.352211 cxalio_studio_tools-0.3.0/src/media_killer/source_adapter.py
+-rw-r--r--   0        0        0     4591 2024-05-22 12:54:36.352211 cxalio_studio_tools-0.3.0/src/media_killer/task_inspector.py
+-rw-r--r--   0        0        0     4246 2024-05-22 12:54:36.352747 cxalio_studio_tools-0.3.0/src/media_killer/transcoder.py
+-rw-r--r--   0        0        0       30 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.3.0/src/sub_conv/__init__.py
+-rw-r--r--   0        0        0     1286 2024-05-22 12:54:36.352747 cxalio_studio_tools-0.3.0/src/sub_conv/env.py
+-rw-r--r--   0        0        0      360 2024-05-22 12:54:36.352747 cxalio_studio_tools-0.3.0/src/sub_conv/exceptions.py
+-rw-r--r--   0        0        0     3548 2024-06-02 15:42:19.845276 cxalio_studio_tools-0.3.0/src/sub_conv/help.md
+-rw-r--r--   0        0        0     5503 2024-05-22 12:54:36.353762 cxalio_studio_tools-0.3.0/src/sub_conv/subconv_app.py
+-rw-r--r--   0        0        0     1857 2024-05-22 12:54:36.353762 cxalio_studio_tools-0.3.0/src/sub_conv/subtitle_translator.py
+-rw-r--r--   0        0        0     6762 2024-05-22 12:54:36.353762 cxalio_studio_tools-0.3.0/src/sub_conv/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 10:52:51.751742 cxalio_studio_tools-0.3.0/src/systools/__init__.py
+-rw-r--r--   0        0        0      282 2024-05-22 12:54:36.354758 cxalio_studio_tools-0.3.0/src/systools/env.py
+-rw-r--r--   0        0        0     3750 2024-05-22 12:54:36.354758 cxalio_studio_tools-0.3.0/src/systools/update_githubhosts.py
+-rw-r--r--   0        0        0     3364 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.3.0/PKG-INFO
```

### Comparing `cxalio_studio_tools-0.2.8/LICENSE` & `cxalio_studio_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/pyproject.toml` & `cxalio_studio_tools-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "cxalio-studio-tools"
-version = "0.2.8"
+version = "0.3.0"
 description = "Scripts for po studio made by cxalio"
 authors = ["xiii_1991 <xiii_1991@163.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
     { include = "cx_core", from = "src" },
     { include = "media_killer", from = "src" },
     { include = "cx_subtitle", from = "src" },
     { include = "sub_conv", from = "src" },
     { include = "systools", from = "src" },
+    { include = "cx_image", from = "src" },
+    { include = "jpegger", from = "src" }
 ]
 
 repository = "https://gitee.com/xiii_1991/cxalio-studio-tools.git"
 homepage = "https://gitee.com/xiii_1991/cxalio-studio-tools"
 keywords = ["ffmpeg", "tool"]
 
 [tool.poetry.dependencies]
@@ -23,16 +25,18 @@
 chardet = "^5.2.0"
 rich-argparse = '^1.4.0'
 python-ffmpeg = "^2.0.10"
 python-docx = "^1.1.0"
 openpyxl = "^3.1.2"
 translators = "^5.9.2"
 xpinyin = "^0.7.6"
+pillow = "^10.3.0"
 
 [tool.poetry.scripts]
 mediakiller = 'media_killer:run'
 subconv = 'sub_conv:run'
 update_githubhosts = 'systools.update_githubhosts:run'
+jpegger = 'jpegger:run'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cxalio_studio_tools-0.2.8/README.md` & `cxalio_studio_tools-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,24 +24,34 @@
 请查看[具体说明](src/media_killer/help.md)
 
 ### SubConv
 
 subconv 是一个批量从字幕文件提取台词本的工具。
 请查看[具体说明](src/sub_conv/help.md)
 
+### Jpegger
+
+Jpegger 是一个批量转换图片格式的工具。请查看[具体说明](src/jpegger/help.md)
+
 ### update_githubhosts
 
 一个自动更新hosts的小工具
 
 ## To-do
 
 - media-inspector 解析媒体信息
 
 ## Change-log
 
+### 0.3.0
+
+- 新工具 jpegger
+- 修改了 subconv 帮助文件中的错误内容
+- 增加了 cx_image 模块
+
 ### 0.2.8
 
 - 强制扩展名按小写判断，不再区分大小写
 
 ### 0.2.7
 
 - 为 mediakiller 增加忽略默认白名单的功能
```

### Comparing `cxalio_studio_tools-0.2.8/src/cx_core/app/abstract_env.py` & `cxalio_studio_tools-0.3.0/src/cx_core/app/abstract_env.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+from rich import traceback
+
 from .app_logger import AppLogger, LogLevel
 
+traceback.install()
+
 
 class AbstractEnv:
     def __init__(self):
         self._logger = AppLogger()
 
     def print(self, *objs):
         self._logger.print(*objs, level=LogLevel.NORMAL)
```

### Comparing `cxalio_studio_tools-0.2.8/src/cx_core/app/app_logger.py` & `cxalio_studio_tools-0.3.0/src/cx_core/app/app_logger.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/cx_core/filesystem/path_expander.py` & `cxalio_studio_tools-0.3.0/src/cx_core/filesystem/path_expander.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from cx_core.filesystem.path_utils import normalize_path
 
 
 class PathExpander:
     @dataclass
     class Settings:
         anchor_dir: Path = Path('..')
+        search_subdir:bool=True
         resolve_symlinks: bool = True
         existed_only: bool = True
         accept_file: bool = True
         accept_dir: bool = True
         accept_other: bool = False
         global_validator: Callable[[Path], bool] = None
         file_validator: Callable[[Path], bool] = None
@@ -26,14 +27,15 @@
         if not isinstance(source, Iterable):
             return [Path(str(source))]
         return sorted([Path(str(x)) for x in source], key=lambda a: a.absolute())
 
     def __init__(self, sources: Any,
                  settings: Settings = None,
                  anchor_dir: Path = None,
+                 search_subdir:bool = None,
                  resolve_symlinks: bool = None,
                  existed_only: bool = None,
                  accept_file: bool = None,
                  accept_dir: bool = None,
                  accept_other: bool = None,
                  global_validator: Callable[[Path], bool] = None,
                  file_validator: Callable[[Path], bool] = None,
@@ -41,14 +43,16 @@
                  skip_duplicated: bool = None,
                  **kwargs):
         self._sources = PathExpander._prepare_path_list(sources)
 
         self.settings = settings or PathExpander.Settings()
         if anchor_dir is not None:
             self.settings.anchor_dir = Path(anchor_dir)
+        if search_subdir is not None:
+            self.settings.search_subdir = search_subdir
         if resolve_symlinks is not None:
             self.settings.resolve_symlinks = resolve_symlinks
         if existed_only is not None:
             self.settings.existed_only = existed_only
         if accept_file is not None:
             self.settings.accept_file = accept_file
         if accept_dir is not None:
@@ -126,16 +130,17 @@
             if self._is_acceptable_file(entry):
                 self._cache_entry(entry)
                 yield entry
             elif self._is_acceptable_dir(entry):
                 if self.settings.accept_dir:
                     # 如果接受目录的话，将会迭代出目录的路径
                     yield entry
-                for sub_entry in entry.iterdir():
-                    yield from self._expand(entry / sub_entry)
+                if self.settings.search_subdir:
+                    for sub_entry in entry.iterdir():
+                        yield from self._expand(entry / sub_entry)
             elif self.settings.accept_other:
                 self._cache_entry(entry)
                 yield entry
 
     def __iter__(self):
         return self._expand(*self._sources)
```

### Comparing `cxalio_studio_tools-0.2.8/src/cx_core/filesystem/path_utils.py` & `cxalio_studio_tools-0.3.0/src/cx_core/filesystem/path_utils.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/cx_core/misc/datapackage.py` & `cxalio_studio_tools-0.3.0/src/cx_core/misc/datapackage.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/cx_core/misc/timecode.py` & `cxalio_studio_tools-0.3.0/src/cx_core/misc/timecode.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/cx_core/misc/timepoint.py` & `cxalio_studio_tools-0.3.0/src/cx_core/misc/timepoint.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/cx_core/text/tag_replacer.py` & `cxalio_studio_tools-0.3.0/src/cx_core/text/tag_replacer.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/cx_core/text/text_utils.py` & `cxalio_studio_tools-0.3.0/src/cx_core/text/text_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,7 +47,17 @@
 
 
 def quote_text(s: str, quote='"'):
     """阔起字符串，默认使用引号。如果给定的quote包含多个字符，则会使用前两个分别阔起，例如使用括号"""
     left = quote[0]
     right = quote[1] if len(quote) > 1 else left
     return left + str(s) + right
+
+
+def extract_numbers(input_string) -> [float]:
+    if not input_string:
+        return []
+    # 使用正则表达式匹配字符串中的所有数字，包括小数
+    numbers = re.findall(r'-?\d+\.?\d*', input_string)
+    # 将匹配到的数字从字符串转换为浮点数或整数
+    numbers = [float(num) if '.' in num else int(num) for num in numbers]
+    return numbers
```

### Comparing `cxalio_studio_tools-0.2.8/src/cx_subtitle/loader.py` & `cxalio_studio_tools-0.3.0/src/cx_subtitle/loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/cx_subtitle/saver.py` & `cxalio_studio_tools-0.3.0/src/cx_subtitle/saver.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/cx_subtitle/subtitle.py` & `cxalio_studio_tools-0.3.0/src/cx_subtitle/subtitle.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/cx_subtitle/subtitle_formatter.py` & `cxalio_studio_tools-0.3.0/src/cx_subtitle/subtitle_formatter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/env.py` & `cxalio_studio_tools-0.3.0/src/media_killer/env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/example_project.toml` & `cxalio_studio_tools-0.3.0/src/media_killer/example_project.toml`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/exceptions.py` & `cxalio_studio_tools-0.3.0/src/media_killer/exceptions.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/help.md` & `cxalio_studio_tools-0.3.0/src/media_killer/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/media_killer_app.py` & `cxalio_studio_tools-0.3.0/src/media_killer/media_killer_app.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/mission.py` & `cxalio_studio_tools-0.3.0/src/media_killer/mission.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/option_package.py` & `cxalio_studio_tools-0.3.0/src/media_killer/option_package.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/profile_loader.py` & `cxalio_studio_tools-0.3.0/src/media_killer/profile_loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/script_writer.py` & `cxalio_studio_tools-0.3.0/src/media_killer/script_writer.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/source_adapter.py` & `cxalio_studio_tools-0.3.0/src/media_killer/source_adapter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/task_inspector.py` & `cxalio_studio_tools-0.3.0/src/media_killer/task_inspector.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/media_killer/transcoder.py` & `cxalio_studio_tools-0.3.0/src/media_killer/transcoder.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/sub_conv/env.py` & `cxalio_studio_tools-0.3.0/src/jpegger/env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/sub_conv/help.md` & `cxalio_studio_tools-0.3.0/src/sub_conv/help.md`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 启用了 `--translate` 参数后，输出的字幕文本将自动转换为英文。
 
 英文翻译使用 bing 翻译服务完成，需要确保网络通畅。
 
 ## 测试运行
 
-指定 `--dry-run` 参数可以启用干转模式，
+指定 `--pretend` 参数可以启用干转模式，
 subconv 将会处理所有的内容，但是不会真的输出文件。
 
 也可以使用 `--debug` 参数，将会输出所有工作过程的信息，方便查看。
 
 两个选项可以一起使用。
 
 -----
```

### Comparing `cxalio_studio_tools-0.2.8/src/sub_conv/subconv_app.py` & `cxalio_studio_tools-0.3.0/src/sub_conv/subconv_app.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/sub_conv/subtitle_translator.py` & `cxalio_studio_tools-0.3.0/src/sub_conv/subtitle_translator.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/sub_conv/worker.py` & `cxalio_studio_tools-0.3.0/src/sub_conv/worker.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/src/systools/update_githubhosts.py` & `cxalio_studio_tools-0.3.0/src/systools/update_githubhosts.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.8/PKG-INFO` & `cxalio_studio_tools-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: cxalio-studio-tools
-Version: 0.2.8
+Version: 0.3.0
 Summary: Scripts for po studio made by cxalio
 Home-page: https://gitee.com/xiii_1991/cxalio-studio-tools
 License: GPL-3.0-or-later
 Keywords: ffmpeg,tool
 Author: xiii_1991
 Author-email: xiii_1991@163.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
+Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: python-docx (>=1.1.0,<2.0.0)
 Requires-Dist: python-ffmpeg (>=2.0.10,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: rich-argparse (>=1.4.0,<2.0.0)
 Requires-Dist: translators (>=5.9.2,<6.0.0)
 Requires-Dist: xpinyin (>=0.7.6,<0.8.0)
 Project-URL: Repository, https://gitee.com/xiii_1991/cxalio-studio-tools.git
@@ -49,24 +50,34 @@
 请查看[具体说明](src/media_killer/help.md)
 
 ### SubConv
 
 subconv 是一个批量从字幕文件提取台词本的工具。
 请查看[具体说明](src/sub_conv/help.md)
 
+### Jpegger
+
+Jpegger 是一个批量转换图片格式的工具。请查看[具体说明](src/jpegger/help.md)
+
 ### update_githubhosts
 
 一个自动更新hosts的小工具
 
 ## To-do
 
 - media-inspector 解析媒体信息
 
 ## Change-log
 
+### 0.3.0
+
+- 新工具 jpegger
+- 修改了 subconv 帮助文件中的错误内容
+- 增加了 cx_image 模块
+
 ### 0.2.8
 
 - 强制扩展名按小写判断，不再区分大小写
 
 ### 0.2.7
 
 - 为 mediakiller 增加忽略默认白名单的功能
```

