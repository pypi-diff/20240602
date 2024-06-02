# Comparing `tmp/pip-setting-1.0.1.tar.gz` & `tmp/pip_setting-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-setting-1.0.1.tar", last modified: Thu Aug  3 08:23:45 2023, max compression
+gzip compressed data, was "pip_setting-1.0.2.tar", last modified: Sun Jun  2 13:21:46 2024, max compression
```

## Comparing `pip-setting-1.0.1.tar` & `pip_setting-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 08:23:45.765025 pip-setting-1.0.1/
--rw-rw-rw-   0        0        0     1082 2023-08-03 07:57:28.000000 pip-setting-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      832 2023-08-03 08:23:45.764022 pip-setting-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-08-03 07:57:28.000000 pip-setting-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 08:23:45.739522 pip-setting-1.0.1/pip_setting/
--rw-rw-rw-   0        0        0     1526 2023-08-03 08:00:22.000000 pip-setting-1.0.1/pip_setting/__init__.py
--rw-rw-rw-   0        0        0      955 2023-08-03 08:20:18.000000 pip-setting-1.0.1/pip_setting/mirrors.json
-drwxrwxrwx   0        0        0        0 2023-08-03 08:23:45.760004 pip-setting-1.0.1/pip_setting.egg-info/
--rw-rw-rw-   0        0        0      832 2023-08-03 08:23:45.000000 pip-setting-1.0.1/pip_setting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-08-03 08:23:45.000000 pip-setting-1.0.1/pip_setting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 08:23:45.000000 pip-setting-1.0.1/pip_setting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-08-03 08:23:45.000000 pip-setting-1.0.1/pip_setting.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2023-08-03 08:23:45.000000 pip-setting-1.0.1/pip_setting.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 08:23:45.765025 pip-setting-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      896 2023-08-03 08:00:25.000000 pip-setting-1.0.1/setup.py
+drwxr-xr-x   0 qiujiajin   (501) staff       (20)        0 2024-06-02 13:21:46.869632 pip_setting-1.0.2/
+-rw-r--r--   0 qiujiajin   (501) staff       (20)     1061 2024-06-02 10:58:10.000000 pip_setting-1.0.2/LICENSE
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      795 2024-06-02 13:21:46.869073 pip_setting-1.0.2/PKG-INFO
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      397 2024-06-02 10:58:10.000000 pip_setting-1.0.2/README.md
+drwxr-xr-x   0 qiujiajin   (501) staff       (20)        0 2024-06-02 13:21:46.866718 pip_setting-1.0.2/pip_setting/
+-rw-r--r--   0 qiujiajin   (501) staff       (20)     1621 2024-06-02 13:16:45.000000 pip_setting-1.0.2/pip_setting/__init__.py
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      374 2024-06-02 12:57:37.000000 pip_setting-1.0.2/pip_setting/mirrors.json
+drwxr-xr-x   0 qiujiajin   (501) staff       (20)        0 2024-06-02 13:21:46.868531 pip_setting-1.0.2/pip_setting.egg-info/
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      795 2024-06-02 13:21:46.000000 pip_setting-1.0.2/pip_setting.egg-info/PKG-INFO
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      253 2024-06-02 13:21:46.000000 pip_setting-1.0.2/pip_setting.egg-info/SOURCES.txt
+-rw-r--r--   0 qiujiajin   (501) staff       (20)        1 2024-06-02 13:21:46.000000 pip_setting-1.0.2/pip_setting.egg-info/dependency_links.txt
+-rw-r--r--   0 qiujiajin   (501) staff       (20)       78 2024-06-02 13:21:46.000000 pip_setting-1.0.2/pip_setting.egg-info/entry_points.txt
+-rw-r--r--   0 qiujiajin   (501) staff       (20)       12 2024-06-02 13:21:46.000000 pip_setting-1.0.2/pip_setting.egg-info/top_level.txt
+-rw-r--r--   0 qiujiajin   (501) staff       (20)       38 2024-06-02 13:21:46.869785 pip_setting-1.0.2/setup.cfg
+-rw-r--r--   0 qiujiajin   (501) staff       (20)      896 2024-06-02 13:19:40.000000 pip_setting-1.0.2/setup.py
```

### Comparing `pip-setting-1.0.1/PKG-INFO` & `pip_setting-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1
-Name: pip-setting
-Version: 1.0.1
-Summary: 快速设置pip镜像源的工具
-Home-page: https://github.com/qq1u/pip_setting
-Author: Hugh
-Author-email: 609799548@qq.com
-License: MIT Licence
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# 设置 pip 镜像源
-
-这是设置国内镜像源的工具，可以使用它快速切换镜像源地址。
-目前支持
-- 官方源
-- 阿里云源
-- 清华源
-- 豆瓣源
-- 腾讯云源
-- 上海交大
-
-#### 方式 1
-```
-命令行直接输入: pip-setting , 根据提示继续操作
-```
-
-#### 方式 2
-命令行输入
-- pip-setting -s 阿里云
-- pip-setting --source 阿里云
+Metadata-Version: 2.1
+Name: pip-setting
+Version: 1.0.2
+Summary: 快速设置pip镜像源的工具
+Home-page: https://github.com/qq1u/pip_setting
+Author: Hugh
+Author-email: 609799548@qq.com
+License: MIT Licence
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# 设置 pip 镜像源
+
+这是设置国内镜像源的工具，可以使用它快速切换镜像源地址。
+目前支持
+- 官方
+- 阿里云
+- 清华
+- 豆瓣
+- 腾讯云
+- 上海交大
+- 华为云
+
+#### 方式 1
+```
+命令行直接输入: pip-setting , 根据提示继续操作
+```
+
+#### 方式 2
+命令行输入
+- pip-setting -s 阿里云
+- pip-setting --source 阿里云
```

### Comparing `pip-setting-1.0.1/pip_setting/__init__.py` & `pip_setting-1.0.2/pip_setting/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import sys
 import json
 import shutil
 import argparse
 from pathlib import Path
+from urllib.parse import urlparse
 
+UTF8 = "UTF8"
 WIN = sys.platform.startswith("win")
-with (Path(__file__).parent / "mirrors.json").open(encoding="utf8") as f:
+with (Path(__file__).parent / "mirrors.json").open(encoding=UTF8) as f:
     mirrors = json.load(f)
-
 pip = Path(f"~/{'pip/pip.ini' if WIN else '.pip/pip.conf'}").expanduser()
 pip_dir = pip.parent
+pip_dir.mkdir(exist_ok=True)
 
 
 def new_file(mirror):
-    if not pip_dir.exists():
-        pip_dir.mkdir()
-    with pip.open("w") as file:
-        file.write("\n".join([f"[{k}]\n{v}" for k, v in mirrors[mirror].items()]))
+    url = mirrors[mirror]
+    host = urlparse(url).hostname
+    with pip.open("w", encoding=UTF8) as fw:
+        fw.writelines([line + "\n" for line in ["[global]", f"index-url={url}", "[install]", f"trusted-host={host}"]])
     print("设置成功")
 
 
 def remove_pip():
     if pip_dir.exists():
         shutil.rmtree(pip_dir)
     print("设置成功")
@@ -32,18 +34,15 @@
     arg = parser.parse_args().source
     if arg in mirrors:
         new_file(arg)
     elif arg == "pypi":
         remove_pip()
     else:
         options = ["官方", *mirrors, "退出"]
-        print(
-            "使用此工具可切换pip镜像源\n"
-            + "\n".join([f"{index}、{item}" for index, item in enumerate(options)])
-        )
+        print("使用此工具可切换pip镜像源\n" + "\n".join([f"{index}、{item}" for index, item in enumerate(options)]))
         while True:
             opt = input("请输入序号: ")
             if opt in tuple(map(str, range(len(options)))):
                 if opt == "0":
                     remove_pip()
                 elif opt != str(len(options) - 1):
                     new_file(options[int(opt)])
```

### Comparing `pip-setting-1.0.1/pip_setting.egg-info/PKG-INFO` & `pip_setting-1.0.2/pip_setting.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1
-Name: pip-setting
-Version: 1.0.1
-Summary: 快速设置pip镜像源的工具
-Home-page: https://github.com/qq1u/pip_setting
-Author: Hugh
-Author-email: 609799548@qq.com
-License: MIT Licence
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# 设置 pip 镜像源
-
-这是设置国内镜像源的工具，可以使用它快速切换镜像源地址。
-目前支持
-- 官方源
-- 阿里云源
-- 清华源
-- 豆瓣源
-- 腾讯云源
-- 上海交大
-
-#### 方式 1
-```
-命令行直接输入: pip-setting , 根据提示继续操作
-```
-
-#### 方式 2
-命令行输入
-- pip-setting -s 阿里云
-- pip-setting --source 阿里云
+Metadata-Version: 2.1
+Name: pip-setting
+Version: 1.0.2
+Summary: 快速设置pip镜像源的工具
+Home-page: https://github.com/qq1u/pip_setting
+Author: Hugh
+Author-email: 609799548@qq.com
+License: MIT Licence
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# 设置 pip 镜像源
+
+这是设置国内镜像源的工具，可以使用它快速切换镜像源地址。
+目前支持
+- 官方
+- 阿里云
+- 清华
+- 豆瓣
+- 腾讯云
+- 上海交大
+- 华为云
+
+#### 方式 1
+```
+命令行直接输入: pip-setting , 根据提示继续操作
+```
+
+#### 方式 2
+命令行输入
+- pip-setting -s 阿里云
+- pip-setting --source 阿里云
```

### Comparing `pip-setting-1.0.1/setup.py` & `pip_setting-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.core import setup
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name="pip-setting",
-    version="1.0.1",
+    version="1.0.2",
     author="Hugh",
     author_email="609799548@qq.com",
     description="快速设置pip镜像源的工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT Licence",
     url="https://github.com/qq1u/pip_setting",
```

