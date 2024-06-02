# Comparing `tmp/advanced_automapper-0.1.4.tar.gz` & `tmp/advanced_automapper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advanced_automapper-0.1.4.tar", max compression
+gzip compressed data, was "advanced_automapper-0.1.5.tar", max compression
```

## Comparing `advanced_automapper-0.1.4.tar` & `advanced_automapper-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-06-01 20:46:39.880221 advanced_automapper-0.1.4/LICENSE
--rw-r--r--   0        0        0     3581 2024-06-01 20:46:39.880221 advanced_automapper-0.1.4/README.md
--rw-r--r--   0        0        0     1311 2024-06-01 20:47:06.816308 advanced_automapper-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       56 2024-06-01 20:46:39.908221 advanced_automapper-0.1.4/src/automapper/__init__.py
--rw-r--r--   0        0        0     2187 2024-06-01 20:46:39.908221 advanced_automapper-0.1.4/src/automapper/functions.py
--rw-r--r--   0        0        0     7708 2024-06-01 20:46:39.908221 advanced_automapper-0.1.4/src/automapper/mapper.py
--rw-r--r--   0        0        0      275 2024-06-01 20:46:39.908221 advanced_automapper-0.1.4/src/automapper/types.py
--rw-r--r--   0        0        0     4618 1970-01-01 00:00:00.000000 advanced_automapper-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-06-02 10:37:49.212842 advanced_automapper-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3581 2024-06-02 10:37:49.212842 advanced_automapper-0.1.5/README.md
+-rw-r--r--   0        0        0     1311 2024-06-02 10:38:18.620664 advanced_automapper-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-06-02 10:37:49.232842 advanced_automapper-0.1.5/src/automapper/__init__.py
+-rw-r--r--   0        0        0     2187 2024-06-02 10:37:49.232842 advanced_automapper-0.1.5/src/automapper/functions.py
+-rw-r--r--   0        0        0     7708 2024-06-02 10:37:49.232842 advanced_automapper-0.1.5/src/automapper/mapper.py
+-rw-r--r--   0        0        0      275 2024-06-02 10:37:49.232842 advanced_automapper-0.1.5/src/automapper/types.py
+-rw-r--r--   0        0        0     4618 1970-01-01 00:00:00.000000 advanced_automapper-0.1.5/PKG-INFO
```

### Comparing `advanced_automapper-0.1.4/LICENSE` & `advanced_automapper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `advanced_automapper-0.1.4/README.md` & `advanced_automapper-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `advanced_automapper-0.1.4/pyproject.toml` & `advanced_automapper-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "advanced-automapper"
-version = "0.1.4"
+version = "0.1.5"
 description = "Object mapper based on type hints"
 authors = ["impalah <impalah@gmail.com>"]
 readme = "README.md"
 packages = [{include = "automapper", from = "src"}]
 license = "MIT"
 homepage = "https://impalah.github.io/advanced-automapper/"
 repository = "https://github.com/impalah/advanced-automapper"
```

### Comparing `advanced_automapper-0.1.4/src/automapper/functions.py` & `advanced_automapper-0.1.5/src/automapper/functions.py`

 * *Files identical despite different names*

### Comparing `advanced_automapper-0.1.4/src/automapper/mapper.py` & `advanced_automapper-0.1.5/src/automapper/mapper.py`

 * *Files identical despite different names*

### Comparing `advanced_automapper-0.1.4/PKG-INFO` & `advanced_automapper-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advanced-automapper
-Version: 0.1.4
+Version: 0.1.5
 Summary: Object mapper based on type hints
 Home-page: https://impalah.github.io/advanced-automapper/
 License: MIT
 Keywords: mapper,typehints,python
 Author: impalah
 Author-email: impalah@gmail.com
 Requires-Python: >=3.10
```

