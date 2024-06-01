# Comparing `tmp/pygetcomics-1.4.5.tar.gz` & `tmp/pygetcomics-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygetcomics-1.4.5.tar", max compression
+gzip compressed data, was "pygetcomics-1.4.6.tar", max compression
```

## Comparing `pygetcomics-1.4.5.tar` & `pygetcomics-1.4.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1323 2017-01-14 11:37:10.942799 pygetcomics-1.4.5/LICENSE
--rw-r--r--   0        0        0       73 2018-09-02 10:16:15.940076 pygetcomics-1.4.5/README.rst
--rw-r--r--   0        0        0      638 2023-06-10 19:44:37.513034 pygetcomics-1.4.5/berhoel/__init__.py
--rw-r--r--   0        0        0     1362 2023-03-18 17:04:23.687285 pygetcomics-1.4.5/berhoel/get_comics/__init__.py
--rw-r--r--   0        0        0     1732 2023-03-19 18:35:26.907425 pygetcomics-1.4.5/berhoel/get_comics/garfield/__init__.py
--rw-r--r--   0        0        0     2430 2023-03-19 18:37:25.695432 pygetcomics-1.4.5/berhoel/get_comics/gen_pdf/__init__.py
--rw-r--r--   0        0        0     1363 2017-01-22 21:50:10.690581 pygetcomics-1.4.5/berhoel/get_comics/gen_pdf/template/book.tex
--rw-r--r--   0        0        0     8635 2024-05-01 18:53:09.835701 pygetcomics-1.4.5/berhoel/get_comics/gocomics/__init__.py
--rw-r--r--   0        0        0     3591 2022-08-09 15:38:07.250228 pygetcomics-1.4.5/berhoel/get_comics/peanuts/__init__.py
--rw-r--r--   0        0        0     1186 2022-08-09 15:01:30.240906 pygetcomics-1.4.5/berhoel/get_comics/peanuts/clean_up.py
--rw-r--r--   0        0        0     5507 2023-03-19 18:38:06.927435 pygetcomics-1.4.5/berhoel/get_comics/peanuts/gen_book.py
--rw-r--r--   0        0        0     1160 2022-08-09 15:51:27.853290 pygetcomics-1.4.5/berhoel/get_comics/tests/test_get_comics.py
--rw-r--r--   0        0        0     2474 2024-05-01 18:40:18.105734 pygetcomics-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pygetcomics-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1323 2017-01-14 11:37:10.942799 pygetcomics-1.4.6/LICENSE
+-rw-r--r--   0        0        0       73 2018-09-02 10:16:15.940076 pygetcomics-1.4.6/README.rst
+-rw-r--r--   0        0        0      638 2023-06-10 19:44:37.513034 pygetcomics-1.4.6/berhoel/__init__.py
+-rw-r--r--   0        0        0     1279 2024-06-01 23:09:06.313748 pygetcomics-1.4.6/berhoel/get_comics/__init__.py
+-rw-r--r--   0        0        0     1732 2023-03-19 18:35:26.907425 pygetcomics-1.4.6/berhoel/get_comics/garfield/__init__.py
+-rw-r--r--   0        0        0     2430 2023-03-19 18:37:25.695432 pygetcomics-1.4.6/berhoel/get_comics/gen_pdf/__init__.py
+-rw-r--r--   0        0        0     1363 2017-01-22 21:50:10.690581 pygetcomics-1.4.6/berhoel/get_comics/gen_pdf/template/book.tex
+-rw-r--r--   0        0        0     8672 2024-06-01 22:58:30.586495 pygetcomics-1.4.6/berhoel/get_comics/gocomics/__init__.py
+-rw-r--r--   0        0        0     3591 2022-08-09 15:38:07.250228 pygetcomics-1.4.6/berhoel/get_comics/peanuts/__init__.py
+-rw-r--r--   0        0        0     1186 2022-08-09 15:01:30.240906 pygetcomics-1.4.6/berhoel/get_comics/peanuts/clean_up.py
+-rw-r--r--   0        0        0     5507 2023-03-19 18:38:06.927435 pygetcomics-1.4.6/berhoel/get_comics/peanuts/gen_book.py
+-rw-r--r--   0        0        0     1160 2022-08-09 15:51:27.853290 pygetcomics-1.4.6/berhoel/get_comics/tests/test_get_comics.py
+-rw-r--r--   0        0        0     2498 2024-06-01 23:11:42.277224 pygetcomics-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pygetcomics-1.4.6/PKG-INFO
```

### Comparing `pygetcomics-1.4.5/LICENSE` & `pygetcomics-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.5/berhoel/__init__.py` & `pygetcomics-1.4.6/berhoel/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.5/berhoel/get_comics/__init__.py` & `pygetcomics-1.4.6/berhoel/get_comics/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """Download various daily comics.
 """
 
-from __future__ import annotations, generator_stop
-
 # Standard library imports.
 import argparse
 
 # Local library imports.
 from . import peanuts, garfield
 
-__date__ = "2023/03/18 18:04:22 hoel"
+__date__ = "2024/06/02 01:09:05 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2017, 2022 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
 __maintainer__ = "Berthold Höllmann"
 __email__ = "berhoel@gmail.com"
-
-try:
-    # Local library imports.
-    from ._version import __version__
-except ImportError:
-    __version__ = "0.0.0.invalid0"
+__version__ = __import__("importlib.metadata", fromlist=["version"]).version(
+    "get_comics"
+)
 
 
 def get_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         prog="get_comics", description="Download various periodic comics."
     )
     parser.add_argument(
```

### Comparing `pygetcomics-1.4.5/berhoel/get_comics/garfield/__init__.py` & `pygetcomics-1.4.6/berhoel/get_comics/garfield/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.5/berhoel/get_comics/gen_pdf/__init__.py` & `pygetcomics-1.4.6/berhoel/get_comics/gen_pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.5/berhoel/get_comics/gen_pdf/template/book.tex` & `pygetcomics-1.4.6/berhoel/get_comics/gen_pdf/template/book.tex`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.5/berhoel/get_comics/gocomics/__init__.py` & `pygetcomics-1.4.6/berhoel/get_comics/gocomics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,17 @@
 
                     mk_dir_tree(png_path.parent)
 
                     res = request.urlretrieve(data, gif_path)
                     if res[1].get_content_type() == "text/html" and data != data_norm:
                         request.urlretrieve(data_norm, gif_path)
 
-                process = subprocess.Popen(f"convert {gif_path} -strip {png_path}", shell=True)
+                process = subprocess.Popen(
+                    f"magick {gif_path} -strip {png_path}", shell=True
+                )
                 os.waitpid(process.pid, 0)
 
                 gif_path.unlink()
                 png_path.chmod(FILE_MODE)
 
                 sys.stdout.write(f"\r                    \r{png_path}\n")
```

### Comparing `pygetcomics-1.4.5/berhoel/get_comics/peanuts/__init__.py` & `pygetcomics-1.4.6/berhoel/get_comics/peanuts/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.5/berhoel/get_comics/peanuts/clean_up.py` & `pygetcomics-1.4.6/berhoel/get_comics/peanuts/clean_up.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.5/berhoel/get_comics/peanuts/gen_book.py` & `pygetcomics-1.4.6/berhoel/get_comics/peanuts/gen_book.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.5/berhoel/get_comics/tests/test_get_comics.py` & `pygetcomics-1.4.6/berhoel/get_comics/tests/test_get_comics.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.5/pyproject.toml` & `pygetcomics-1.4.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "pyGetComics"
-version = "1.4.5"
+version = "1.4.6"
 
 description = "Download various daily comics."
 
 packages = [{ include = "berhoel" }]
+exclude = ["**/.#*.py", "**/#*.py#"]
 
 authors = ["Berthold Höllmann <berhoel@gmail.com>"]
 license = "BSD-2-Clause"
 
 repository = "https://gitlab.com/berhoel/python/pyGetComics.git"
 
 readme = "README.rst"
@@ -46,15 +47,14 @@
 pytest-runner = "*"
 pytest-sugar = "*"
 isort = "*"
 rope = "*"
 pylint = "*"
 pylint-common = "*"
 pylint-plugin-utils = "*"
-bhoelhelper = ">=1.3.0"
 berhoel-sphinx-settings = { git = "https://gitlab.com/berhoel/python/berhoel-sphinx-settings.git", rev = "main" }
 tomli = "*"
 sphinx-argparse-cli = "*"
 
 [tool.berhoel.helper.set_version]
 version_files = ["berhoel/get_comics/_version.py"]
 
@@ -90,9 +90,9 @@
 addopts = "--doctest-modules --ff --pdb -s --cov=berhoel --cov-report=term --cov-report=html --cov-branch --isort --black --flake8"
 testpaths = ["berhoel"]
 
 [flake8]
 max-line-length = 88
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pygetcomics-1.4.5/PKG-INFO` & `pygetcomics-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGetComics
-Version: 1.4.5
+Version: 1.4.6
 Summary: Download various daily comics.
 Home-page: https://gitlab.com/berhoel/python/pyGetComics.git
 License: BSD-2-Clause
 Author: Berthold Höllmann
 Author-email: berhoel@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

