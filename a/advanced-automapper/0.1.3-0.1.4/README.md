# Comparing `tmp/advanced_automapper-0.1.3.tar.gz` & `tmp/advanced_automapper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advanced_automapper-0.1.3.tar", max compression
+gzip compressed data, was "advanced_automapper-0.1.4.tar", max compression
```

## Comparing `advanced_automapper-0.1.3.tar` & `advanced_automapper-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-06-01 20:35:25.709552 advanced_automapper-0.1.3/LICENSE
--rw-r--r--   0        0        0     3567 2024-06-01 20:35:25.709552 advanced_automapper-0.1.3/README.md
--rw-r--r--   0        0        0     1311 2024-06-01 20:35:53.005589 advanced_automapper-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       56 2024-06-01 20:35:25.729552 advanced_automapper-0.1.3/src/automapper/__init__.py
--rw-r--r--   0        0        0     2187 2024-06-01 20:35:25.729552 advanced_automapper-0.1.3/src/automapper/functions.py
--rw-r--r--   0        0        0     7708 2024-06-01 20:35:25.729552 advanced_automapper-0.1.3/src/automapper/mapper.py
--rw-r--r--   0        0        0      275 2024-06-01 20:35:25.729552 advanced_automapper-0.1.3/src/automapper/types.py
--rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 advanced_automapper-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-06-01 20:46:39.880221 advanced_automapper-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3581 2024-06-01 20:46:39.880221 advanced_automapper-0.1.4/README.md
+-rw-r--r--   0        0        0     1311 2024-06-01 20:47:06.816308 advanced_automapper-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-06-01 20:46:39.908221 advanced_automapper-0.1.4/src/automapper/__init__.py
+-rw-r--r--   0        0        0     2187 2024-06-01 20:46:39.908221 advanced_automapper-0.1.4/src/automapper/functions.py
+-rw-r--r--   0        0        0     7708 2024-06-01 20:46:39.908221 advanced_automapper-0.1.4/src/automapper/mapper.py
+-rw-r--r--   0        0        0      275 2024-06-01 20:46:39.908221 advanced_automapper-0.1.4/src/automapper/types.py
+-rw-r--r--   0        0        0     4618 1970-01-01 00:00:00.000000 advanced_automapper-0.1.4/PKG-INFO
```

### Comparing `advanced_automapper-0.1.3/LICENSE` & `advanced_automapper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `advanced_automapper-0.1.3/README.md` & `advanced_automapper-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 
 ## Installation
 
 Using pip:
 
 ```bash
-pip install pyautomapper
+pip install advanced-automapper
 ```
 
 Using poetry
 
 ```bash
-poetry pyautomapper
+poetry advanced-automapper
 ```
 
 
 ## Get started
 
 It is important to note that PyAutomapper requieres that both origin and destination classes have have type hints to define the type for every field.
```

### Comparing `advanced_automapper-0.1.3/pyproject.toml` & `advanced_automapper-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "advanced-automapper"
-version = "0.1.3"
+version = "0.1.4"
 description = "Object mapper based on type hints"
 authors = ["impalah <impalah@gmail.com>"]
 readme = "README.md"
 packages = [{include = "automapper", from = "src"}]
 license = "MIT"
 homepage = "https://impalah.github.io/advanced-automapper/"
 repository = "https://github.com/impalah/advanced-automapper"
```

### Comparing `advanced_automapper-0.1.3/src/automapper/functions.py` & `advanced_automapper-0.1.4/src/automapper/functions.py`

 * *Files identical despite different names*

### Comparing `advanced_automapper-0.1.3/src/automapper/mapper.py` & `advanced_automapper-0.1.4/src/automapper/mapper.py`

 * *Files identical despite different names*

### Comparing `advanced_automapper-0.1.3/PKG-INFO` & `advanced_automapper-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advanced-automapper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Object mapper based on type hints
 Home-page: https://impalah.github.io/advanced-automapper/
 License: MIT
 Keywords: mapper,typehints,python
 Author: impalah
 Author-email: impalah@gmail.com
 Requires-Python: >=3.10
@@ -29,21 +29,21 @@
 
 
 ## Installation
 
 Using pip:
 
 ```bash
-pip install pyautomapper
+pip install advanced-automapper
 ```
 
 Using poetry
 
 ```bash
-poetry pyautomapper
+poetry advanced-automapper
 ```
 
 
 ## Get started
 
 It is important to note that PyAutomapper requieres that both origin and destination classes have have type hints to define the type for every field.
```

