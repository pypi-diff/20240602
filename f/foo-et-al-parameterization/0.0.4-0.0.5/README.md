# Comparing `tmp/foo_et_al_parameterization-0.0.4.tar.gz` & `tmp/foo_et_al_parameterization-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foo_et_al_parameterization-0.0.4.tar", last modified: Sun Jun  2 19:47:56 2024, max compression
+gzip compressed data, was "foo_et_al_parameterization-0.0.5.tar", last modified: Sun Jun  2 19:52:32 2024, max compression
```

## Comparing `foo_et_al_parameterization-0.0.4.tar` & `foo_et_al_parameterization-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 19:47:56.294730 foo_et_al_parameterization-0.0.4/
--rw-rw-rw-   0        0        0     1091 2024-06-02 18:35:49.000000 foo_et_al_parameterization-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1223 2024-06-02 19:47:56.292731 foo_et_al_parameterization-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-06-02 19:43:40.000000 foo_et_al_parameterization-0.0.4/README.md
--rw-rw-rw-   0        0        0      526 2024-06-02 19:47:24.000000 foo_et_al_parameterization-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-02 19:47:56.294730 foo_et_al_parameterization-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-02 19:47:56.259554 foo_et_al_parameterization-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-06-02 19:47:56.266554 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization/
--rw-rw-rw-   0        0        0        2 2024-06-02 19:37:46.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization/__init__.py
--rw-rw-rw-   0        0        0      409 2024-06-02 19:01:29.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization/foo-et-al-parameterization.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:47:56.291734 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/
--rw-rw-rw-   0        0        0     1223 2024-06-02 19:47:56.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-06-02 19:47:56.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 19:47:56.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-06-02 19:47:56.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 19:52:32.627647 foo_et_al_parameterization-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2024-06-02 18:35:49.000000 foo_et_al_parameterization-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1223 2024-06-02 19:52:32.625695 foo_et_al_parameterization-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-06-02 19:43:40.000000 foo_et_al_parameterization-0.0.5/README.md
+-rw-rw-rw-   0        0        0      526 2024-06-02 19:52:25.000000 foo_et_al_parameterization-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 19:52:32.627647 foo_et_al_parameterization-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 19:52:32.594150 foo_et_al_parameterization-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 19:52:32.601150 foo_et_al_parameterization-0.0.5/src/foo_et_al_parameterization/
+-rw-rw-rw-   0        0        0       54 2024-06-02 19:52:25.000000 foo_et_al_parameterization-0.0.5/src/foo_et_al_parameterization/__init__.py
+-rw-rw-rw-   0        0        0      409 2024-06-02 19:01:29.000000 foo_et_al_parameterization-0.0.5/src/foo_et_al_parameterization/foo-et-al-parameterization.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:52:32.624648 foo_et_al_parameterization-0.0.5/src/foo_et_al_parameterization.egg-info/
+-rw-rw-rw-   0        0        0     1223 2024-06-02 19:52:32.000000 foo_et_al_parameterization-0.0.5/src/foo_et_al_parameterization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-06-02 19:52:32.000000 foo_et_al_parameterization-0.0.5/src/foo_et_al_parameterization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 19:52:32.000000 foo_et_al_parameterization-0.0.5/src/foo_et_al_parameterization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-06-02 19:52:32.000000 foo_et_al_parameterization-0.0.5/src/foo_et_al_parameterization.egg-info/top_level.txt
```

### Comparing `foo_et_al_parameterization-0.0.4/LICENSE` & `foo_et_al_parameterization-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `foo_et_al_parameterization-0.0.4/PKG-INFO` & `foo_et_al_parameterization-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foo-et-al-parameterization
-Version: 0.0.4
+Version: 0.0.5
 Summary: A basic python library to gain the volume of a sphere given its radius
 Author-email: Aidan Goldstein <goldstai@oregonstate.edu>
 Project-URL: Homepage, https://github.com/aidangold/foo-et-al-parameterization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `foo_et_al_parameterization-0.0.4/README.md` & `foo_et_al_parameterization-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `foo_et_al_parameterization-0.0.4/pyproject.toml` & `foo_et_al_parameterization-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "foo-et-al-parameterization"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name ="Aidan Goldstein", email="goldstai@oregonstate.edu" },
 ]
 description = "A basic python library to gain the volume of a sphere given its radius"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/PKG-INFO` & `foo_et_al_parameterization-0.0.5/src/foo_et_al_parameterization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foo-et-al-parameterization
-Version: 0.0.4
+Version: 0.0.5
 Summary: A basic python library to gain the volume of a sphere given its radius
 Author-email: Aidan Goldstein <goldstai@oregonstate.edu>
 Project-URL: Homepage, https://github.com/aidangold/foo-et-al-parameterization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

