# Comparing `tmp/foo_et_al_parameterization-0.0.8.tar.gz` & `tmp/foo_et_al_parameterization-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foo_et_al_parameterization-0.0.8.tar", last modified: Sun Jun  2 20:10:58 2024, max compression
+gzip compressed data, was "foo_et_al_parameterization-0.0.9.tar", last modified: Sun Jun  2 20:18:36 2024, max compression
```

## Comparing `foo_et_al_parameterization-0.0.8.tar` & `foo_et_al_parameterization-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 20:10:58.421529 foo_et_al_parameterization-0.0.8/
--rw-rw-rw-   0        0        0     1091 2024-06-02 18:35:49.000000 foo_et_al_parameterization-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1222 2024-06-02 20:10:58.419545 foo_et_al_parameterization-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      691 2024-06-02 20:08:41.000000 foo_et_al_parameterization-0.0.8/README.md
--rw-rw-rw-   0        0        0      526 2024-06-02 20:09:06.000000 foo_et_al_parameterization-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-02 20:10:58.421529 foo_et_al_parameterization-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-02 20:10:58.376850 foo_et_al_parameterization-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-06-02 20:10:58.385828 foo_et_al_parameterization-0.0.8/src/foo_et_al_parameterization/
--rw-rw-rw-   0        0        0      409 2024-06-02 19:01:29.000000 foo_et_al_parameterization-0.0.8/src/foo_et_al_parameterization/SphereVolume.py
--rw-rw-rw-   0        0        0       53 2024-06-02 20:10:46.000000 foo_et_al_parameterization-0.0.8/src/foo_et_al_parameterization/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 20:10:58.416545 foo_et_al_parameterization-0.0.8/src/foo_et_al_parameterization.egg-info/
--rw-rw-rw-   0        0        0     1222 2024-06-02 20:10:58.000000 foo_et_al_parameterization-0.0.8/src/foo_et_al_parameterization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-06-02 20:10:58.000000 foo_et_al_parameterization-0.0.8/src/foo_et_al_parameterization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 20:10:58.000000 foo_et_al_parameterization-0.0.8/src/foo_et_al_parameterization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-06-02 20:10:58.000000 foo_et_al_parameterization-0.0.8/src/foo_et_al_parameterization.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 20:18:36.758247 foo_et_al_parameterization-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2024-06-02 18:35:49.000000 foo_et_al_parameterization-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1204 2024-06-02 20:18:36.757246 foo_et_al_parameterization-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2024-06-02 20:18:27.000000 foo_et_al_parameterization-0.0.9/README.md
+-rw-rw-rw-   0        0        0      526 2024-06-02 20:18:27.000000 foo_et_al_parameterization-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 20:18:36.758247 foo_et_al_parameterization-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 20:18:36.731247 foo_et_al_parameterization-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 20:18:36.739247 foo_et_al_parameterization-0.0.9/src/foo_et_al_parameterization/
+-rw-rw-rw-   0        0        0      409 2024-06-02 19:01:29.000000 foo_et_al_parameterization-0.0.9/src/foo_et_al_parameterization/SphereVolume.py
+-rw-rw-rw-   0        0        0       41 2024-06-02 20:15:41.000000 foo_et_al_parameterization-0.0.9/src/foo_et_al_parameterization/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:18:36.755246 foo_et_al_parameterization-0.0.9/src/foo_et_al_parameterization.egg-info/
+-rw-rw-rw-   0        0        0     1204 2024-06-02 20:18:36.000000 foo_et_al_parameterization-0.0.9/src/foo_et_al_parameterization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-06-02 20:18:36.000000 foo_et_al_parameterization-0.0.9/src/foo_et_al_parameterization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 20:18:36.000000 foo_et_al_parameterization-0.0.9/src/foo_et_al_parameterization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-06-02 20:18:36.000000 foo_et_al_parameterization-0.0.9/src/foo_et_al_parameterization.egg-info/top_level.txt
```

### Comparing `foo_et_al_parameterization-0.0.8/LICENSE` & `foo_et_al_parameterization-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `foo_et_al_parameterization-0.0.8/PKG-INFO` & `foo_et_al_parameterization-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foo-et-al-parameterization
-Version: 0.0.8
+Version: 0.0.9
 Summary: A basic python library to gain the volume of a sphere given its radius
 Author-email: Aidan Goldstein <goldstai@oregonstate.edu>
 Project-URL: Homepage, https://github.com/aidangold/foo-et-al-parameterization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -28,9 +28,9 @@
 
 ```bash
 pip install foo-et-al-parameterization
 ```
 Don't forget to import before using in a file!
 
 ```bash
-from foo_et_al_parameterization import SphereVolume
+import foo_et_al_parameterization
 ```
```

### Comparing `foo_et_al_parameterization-0.0.8/README.md` & `foo_et_al_parameterization-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 
 ```bash
 pip install foo-et-al-parameterization
 ```
 Don't forget to import before using in a file!
 
 ```bash
-from foo_et_al_parameterization import SphereVolume
+import foo_et_al_parameterization
 ```
```

### Comparing `foo_et_al_parameterization-0.0.8/pyproject.toml` & `foo_et_al_parameterization-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "foo-et-al-parameterization"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name ="Aidan Goldstein", email="goldstai@oregonstate.edu" },
 ]
 description = "A basic python library to gain the volume of a sphere given its radius"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `foo_et_al_parameterization-0.0.8/src/foo_et_al_parameterization.egg-info/PKG-INFO` & `foo_et_al_parameterization-0.0.9/src/foo_et_al_parameterization.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foo-et-al-parameterization
-Version: 0.0.8
+Version: 0.0.9
 Summary: A basic python library to gain the volume of a sphere given its radius
 Author-email: Aidan Goldstein <goldstai@oregonstate.edu>
 Project-URL: Homepage, https://github.com/aidangold/foo-et-al-parameterization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -28,9 +28,9 @@
 
 ```bash
 pip install foo-et-al-parameterization
 ```
 Don't forget to import before using in a file!
 
 ```bash
-from foo_et_al_parameterization import SphereVolume
+import foo_et_al_parameterization
 ```
```

