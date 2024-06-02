# Comparing `tmp/foo_et_al_parameterization-0.0.6.tar.gz` & `tmp/foo_et_al_parameterization-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foo_et_al_parameterization-0.0.6.tar", last modified: Sun Jun  2 19:58:08 2024, max compression
+gzip compressed data, was "foo_et_al_parameterization-0.0.7.tar", last modified: Sun Jun  2 20:07:52 2024, max compression
```

## Comparing `foo_et_al_parameterization-0.0.6.tar` & `foo_et_al_parameterization-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 19:58:08.069228 foo_et_al_parameterization-0.0.6/
--rw-rw-rw-   0        0        0     1091 2024-06-02 18:35:49.000000 foo_et_al_parameterization-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1223 2024-06-02 19:58:08.067228 foo_et_al_parameterization-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-06-02 19:43:40.000000 foo_et_al_parameterization-0.0.6/README.md
--rw-rw-rw-   0        0        0      526 2024-06-02 19:58:00.000000 foo_et_al_parameterization-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-02 19:58:08.069228 foo_et_al_parameterization-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-02 19:58:08.040234 foo_et_al_parameterization-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-06-02 19:58:08.048227 foo_et_al_parameterization-0.0.6/src/foo_et_al_parameterization/
--rw-rw-rw-   0        0        0       54 2024-06-02 19:52:25.000000 foo_et_al_parameterization-0.0.6/src/foo_et_al_parameterization/__init__.py
--rw-rw-rw-   0        0        0      409 2024-06-02 19:01:29.000000 foo_et_al_parameterization-0.0.6/src/foo_et_al_parameterization/sphere_volume.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:58:08.066227 foo_et_al_parameterization-0.0.6/src/foo_et_al_parameterization.egg-info/
--rw-rw-rw-   0        0        0     1223 2024-06-02 19:58:08.000000 foo_et_al_parameterization-0.0.6/src/foo_et_al_parameterization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2024-06-02 19:58:08.000000 foo_et_al_parameterization-0.0.6/src/foo_et_al_parameterization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 19:58:08.000000 foo_et_al_parameterization-0.0.6/src/foo_et_al_parameterization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-06-02 19:58:08.000000 foo_et_al_parameterization-0.0.6/src/foo_et_al_parameterization.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 20:07:52.731979 foo_et_al_parameterization-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2024-06-02 18:35:49.000000 foo_et_al_parameterization-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1222 2024-06-02 20:07:52.729980 foo_et_al_parameterization-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      691 2024-06-02 20:07:37.000000 foo_et_al_parameterization-0.0.7/README.md
+-rw-rw-rw-   0        0        0      526 2024-06-02 20:07:41.000000 foo_et_al_parameterization-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 20:07:52.731979 foo_et_al_parameterization-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 20:07:52.704242 foo_et_al_parameterization-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 20:07:52.712242 foo_et_al_parameterization-0.0.7/src/foo_et_al_parameterization/
+-rw-rw-rw-   0        0        0      409 2024-06-02 19:01:29.000000 foo_et_al_parameterization-0.0.7/src/foo_et_al_parameterization/SphereVolume.py
+-rw-rw-rw-   0        0        0       54 2024-06-02 19:52:25.000000 foo_et_al_parameterization-0.0.7/src/foo_et_al_parameterization/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:07:52.728978 foo_et_al_parameterization-0.0.7/src/foo_et_al_parameterization.egg-info/
+-rw-rw-rw-   0        0        0     1222 2024-06-02 20:07:52.000000 foo_et_al_parameterization-0.0.7/src/foo_et_al_parameterization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-06-02 20:07:52.000000 foo_et_al_parameterization-0.0.7/src/foo_et_al_parameterization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 20:07:52.000000 foo_et_al_parameterization-0.0.7/src/foo_et_al_parameterization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-06-02 20:07:52.000000 foo_et_al_parameterization-0.0.7/src/foo_et_al_parameterization.egg-info/top_level.txt
```

### Comparing `foo_et_al_parameterization-0.0.6/LICENSE` & `foo_et_al_parameterization-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `foo_et_al_parameterization-0.0.6/PKG-INFO` & `foo_et_al_parameterization-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foo-et-al-parameterization
-Version: 0.0.6
+Version: 0.0.7
 Summary: A basic python library to gain the volume of a sphere given its radius
 Author-email: Aidan Goldstein <goldstai@oregonstate.edu>
 Project-URL: Homepage, https://github.com/aidangold/foo-et-al-parameterization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -28,9 +28,9 @@
 
 ```bash
 pip install foo_et_al_parameterization
 ```
 Don't forget to import before using in a file!
 
 ```bash
-from foo_et_al_parameterization import sphere_volume
+from foo_et_al_parameterization import SphereVolume
 ```
```

### Comparing `foo_et_al_parameterization-0.0.6/README.md` & `foo_et_al_parameterization-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 
 ```bash
 pip install foo_et_al_parameterization
 ```
 Don't forget to import before using in a file!
 
 ```bash
-from foo_et_al_parameterization import sphere_volume
+from foo_et_al_parameterization import SphereVolume
 ```
```

### Comparing `foo_et_al_parameterization-0.0.6/pyproject.toml` & `foo_et_al_parameterization-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "foo-et-al-parameterization"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name ="Aidan Goldstein", email="goldstai@oregonstate.edu" },
 ]
 description = "A basic python library to gain the volume of a sphere given its radius"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `foo_et_al_parameterization-0.0.6/src/foo_et_al_parameterization.egg-info/PKG-INFO` & `foo_et_al_parameterization-0.0.7/src/foo_et_al_parameterization.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foo-et-al-parameterization
-Version: 0.0.6
+Version: 0.0.7
 Summary: A basic python library to gain the volume of a sphere given its radius
 Author-email: Aidan Goldstein <goldstai@oregonstate.edu>
 Project-URL: Homepage, https://github.com/aidangold/foo-et-al-parameterization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -28,9 +28,9 @@
 
 ```bash
 pip install foo_et_al_parameterization
 ```
 Don't forget to import before using in a file!
 
 ```bash
-from foo_et_al_parameterization import sphere_volume
+from foo_et_al_parameterization import SphereVolume
 ```
```

