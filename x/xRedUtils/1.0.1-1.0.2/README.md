# Comparing `tmp/xredutils-1.0.1.tar.gz` & `tmp/xredutils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xredutils-1.0.1.tar", last modified: Sat May 25 19:27:51 2024, max compression
+gzip compressed data, was "xredutils-1.0.2.tar", last modified: Sun Jun  2 14:46:24 2024, max compression
```

## Comparing `xredutils-1.0.1.tar` & `xredutils-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 19:27:51.832071 xredutils-1.0.1/
--rw-rw-rw-   0        0        0     1090 2024-04-21 12:02:44.000000 xredutils-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1289 2024-05-25 19:27:51.831070 xredutils-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      607 2024-05-25 19:02:11.000000 xredutils-1.0.1/README.rst
--rw-rw-rw-   0        0        0      862 2024-05-25 19:27:01.000000 xredutils-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-25 19:27:51.832071 xredutils-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-25 19:27:51.818518 xredutils-1.0.1/xRedUtils/
--rw-rw-rw-   0        0        0     1239 2024-05-25 17:40:50.000000 xredutils-1.0.1/xRedUtils/__init__.py
--rw-rw-rw-   0        0        0     1189 2024-05-25 18:28:34.000000 xredutils-1.0.1/xRedUtils/dates.py
--rw-rw-rw-   0        0        0     5220 2024-05-25 18:27:52.000000 xredutils-1.0.1/xRedUtils/dicts.py
--rw-rw-rw-   0        0        0     3158 2024-05-25 18:27:19.000000 xredutils-1.0.1/xRedUtils/errors.py
--rw-rw-rw-   0        0        0     1754 2024-05-25 18:26:36.000000 xredutils-1.0.1/xRedUtils/funcs.py
--rw-rw-rw-   0        0        0     1324 2024-05-25 16:23:21.000000 xredutils-1.0.1/xRedUtils/general.py
--rw-rw-rw-   0        0        0     3275 2024-05-25 18:26:26.000000 xredutils-1.0.1/xRedUtils/iterables.py
--rw-rw-rw-   0        0        0     2354 2024-05-25 18:25:53.000000 xredutils-1.0.1/xRedUtils/maths.py
--rw-rw-rw-   0        0        0      705 2024-05-25 16:19:38.000000 xredutils-1.0.1/xRedUtils/regexes.py
--rw-rw-rw-   0        0        0     2803 2024-05-25 18:24:58.000000 xredutils-1.0.1/xRedUtils/strings.py
-drwxrwxrwx   0        0        0        0 2024-05-25 19:27:51.829072 xredutils-1.0.1/xRedUtils/test/
--rw-rw-rw-   0        0        0     5253 2024-05-25 16:26:31.000000 xredutils-1.0.1/xRedUtils/test/test.py
--rw-rw-rw-   0        0        0     3096 2024-05-25 18:24:25.000000 xredutils-1.0.1/xRedUtils/times.py
--rw-rw-rw-   0        0        0     6629 2024-05-25 18:23:56.000000 xredutils-1.0.1/xRedUtils/type_hints.py
-drwxrwxrwx   0        0        0        0 2024-05-25 19:27:51.830069 xredutils-1.0.1/xRedUtils.egg-info/
--rw-rw-rw-   0        0        0     1289 2024-05-25 19:27:51.000000 xredutils-1.0.1/xRedUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2024-05-25 19:27:51.000000 xredutils-1.0.1/xRedUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 19:27:51.000000 xredutils-1.0.1/xRedUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-25 19:27:51.000000 xredutils-1.0.1/xRedUtils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 14:46:24.366903 xredutils-1.0.2/
+-rw-rw-rw-   0        0        0     1090 2024-04-21 12:02:44.000000 xredutils-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1289 2024-06-02 14:46:24.365902 xredutils-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2024-05-25 19:02:11.000000 xredutils-1.0.2/README.rst
+-rw-rw-rw-   0        0        0      862 2024-06-02 14:46:18.000000 xredutils-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 14:46:24.366903 xredutils-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 14:46:24.348886 xredutils-1.0.2/xRedUtils/
+-rw-rw-rw-   0        0        0     1239 2024-05-25 20:11:43.000000 xredutils-1.0.2/xRedUtils/__init__.py
+-rw-rw-rw-   0        0        0     1189 2024-05-25 18:28:34.000000 xredutils-1.0.2/xRedUtils/dates.py
+-rw-rw-rw-   0        0        0     5220 2024-05-25 18:27:52.000000 xredutils-1.0.2/xRedUtils/dicts.py
+-rw-rw-rw-   0        0        0     3158 2024-05-25 18:27:19.000000 xredutils-1.0.2/xRedUtils/errors.py
+-rw-rw-rw-   0        0        0     1754 2024-05-25 18:26:36.000000 xredutils-1.0.2/xRedUtils/funcs.py
+-rw-rw-rw-   0        0        0     1351 2024-06-02 14:43:37.000000 xredutils-1.0.2/xRedUtils/general.py
+-rw-rw-rw-   0        0        0     3275 2024-05-25 18:26:26.000000 xredutils-1.0.2/xRedUtils/iterables.py
+-rw-rw-rw-   0        0        0     2354 2024-05-25 18:25:53.000000 xredutils-1.0.2/xRedUtils/maths.py
+-rw-rw-rw-   0        0        0      705 2024-05-25 16:19:38.000000 xredutils-1.0.2/xRedUtils/regexes.py
+-rw-rw-rw-   0        0        0     2803 2024-05-25 18:24:58.000000 xredutils-1.0.2/xRedUtils/strings.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:46:24.363901 xredutils-1.0.2/xRedUtils/test/
+-rw-rw-rw-   0        0        0     5253 2024-05-25 20:12:04.000000 xredutils-1.0.2/xRedUtils/test/test.py
+-rw-rw-rw-   0        0        0     3096 2024-05-25 18:24:25.000000 xredutils-1.0.2/xRedUtils/times.py
+-rw-rw-rw-   0        0        0     6629 2024-05-25 18:23:56.000000 xredutils-1.0.2/xRedUtils/type_hints.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:46:24.364901 xredutils-1.0.2/xRedUtils.egg-info/
+-rw-rw-rw-   0        0        0     1289 2024-06-02 14:46:24.000000 xredutils-1.0.2/xRedUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2024-06-02 14:46:24.000000 xredutils-1.0.2/xRedUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 14:46:24.000000 xredutils-1.0.2/xRedUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 14:46:24.000000 xredutils-1.0.2/xRedUtils.egg-info/top_level.txt
```

### Comparing `xredutils-1.0.1/LICENSE` & `xredutils-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/PKG-INFO` & `xredutils-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xRedUtils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple, general purpose functions in one place!
 Author: xRedCrystalx
 Project-URL: Homepage, https://github.com/xRedCrystalx/RedUtils
 Project-URL: Issues, https://github.com/xRedCrystalx/RedUtils/issues
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `xredutils-1.0.1/README.rst` & `xredutils-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/pyproject.toml` & `xredutils-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xRedUtils"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{ name="xRedCrystalx" }]
 description = "Simple, general purpose functions in one place!"
 requires-python = ">=3.12"
 readme = "README.rst"
 
 classifiers = [
     "Natural Language :: English",
```

### Comparing `xredutils-1.0.1/xRedUtils/__init__.py` & `xredutils-1.0.2/xRedUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils/dates.py` & `xredutils-1.0.2/xRedUtils/dates.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils/dicts.py` & `xredutils-1.0.2/xRedUtils/dicts.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils/errors.py` & `xredutils-1.0.2/xRedUtils/errors.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils/funcs.py` & `xredutils-1.0.2/xRedUtils/funcs.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils/general.py` & `xredutils-1.0.2/xRedUtils/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,11 +34,11 @@
 DEVICE_ENCODING: str | None = os.device_encoding(1)
 
 WIN_EDITION: str = platform.win32_edition()
 WIN_IOT: bool = platform.win32_is_iot()
 
 CPU_COUNT: int | None = os.cpu_count()
 PROCESSOR_NAME: str = platform.processor()
-DRIVES: list[str] = os.listdrives()
+DRIVES: list[str] = os.listdrives() if OS == "Windows" else []
 
 CWD: str = os.getcwd()
 RECURSION_LIMIT: int = sys.getrecursionlimit()
```

### Comparing `xredutils-1.0.1/xRedUtils/iterables.py` & `xredutils-1.0.2/xRedUtils/iterables.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils/maths.py` & `xredutils-1.0.2/xRedUtils/maths.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils/regexes.py` & `xredutils-1.0.2/xRedUtils/regexes.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils/strings.py` & `xredutils-1.0.2/xRedUtils/strings.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils/test/test.py` & `xredutils-1.0.2/xRedUtils/test/test.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils/times.py` & `xredutils-1.0.2/xRedUtils/times.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils/type_hints.py` & `xredutils-1.0.2/xRedUtils/type_hints.py`

 * *Files identical despite different names*

### Comparing `xredutils-1.0.1/xRedUtils.egg-info/PKG-INFO` & `xredutils-1.0.2/xRedUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xRedUtils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple, general purpose functions in one place!
 Author: xRedCrystalx
 Project-URL: Homepage, https://github.com/xRedCrystalx/RedUtils
 Project-URL: Issues, https://github.com/xRedCrystalx/RedUtils/issues
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.12
```

