# Comparing `tmp/foo_et_al_parameterization-0.0.2.tar.gz` & `tmp/foo_et_al_parameterization-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foo_et_al_parameterization-0.0.2.tar", last modified: Sun Jun  2 19:27:28 2024, max compression
+gzip compressed data, was "foo_et_al_parameterization-0.0.4.tar", last modified: Sun Jun  2 19:47:56 2024, max compression
```

## Comparing `foo_et_al_parameterization-0.0.2.tar` & `foo_et_al_parameterization-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 19:27:28.082056 foo_et_al_parameterization-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-06-02 18:35:49.000000 foo_et_al_parameterization-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1223 2024-06-02 19:27:28.081056 foo_et_al_parameterization-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-06-02 19:11:11.000000 foo_et_al_parameterization-0.0.2/README.md
--rw-rw-rw-   0        0        0      526 2024-06-02 19:14:46.000000 foo_et_al_parameterization-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-02 19:27:28.083063 foo_et_al_parameterization-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-02 19:27:28.057062 foo_et_al_parameterization-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-06-02 19:27:28.066055 foo_et_al_parameterization-0.0.2/src/foo-et-al-parameterization/
--rw-rw-rw-   0        0        0        0 2024-06-02 18:10:47.000000 foo_et_al_parameterization-0.0.2/src/foo-et-al-parameterization/__init__.py
--rw-rw-rw-   0        0        0      409 2024-06-02 19:01:29.000000 foo_et_al_parameterization-0.0.2/src/foo-et-al-parameterization/foo-et-al-parameterization.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:27:28.079055 foo_et_al_parameterization-0.0.2/src/foo_et_al_parameterization.egg-info/
--rw-rw-rw-   0        0        0     1223 2024-06-02 19:27:28.000000 foo_et_al_parameterization-0.0.2/src/foo_et_al_parameterization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-06-02 19:27:28.000000 foo_et_al_parameterization-0.0.2/src/foo_et_al_parameterization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 19:27:28.000000 foo_et_al_parameterization-0.0.2/src/foo_et_al_parameterization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-06-02 19:27:28.000000 foo_et_al_parameterization-0.0.2/src/foo_et_al_parameterization.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 19:47:56.294730 foo_et_al_parameterization-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-06-02 18:35:49.000000 foo_et_al_parameterization-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1223 2024-06-02 19:47:56.292731 foo_et_al_parameterization-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-06-02 19:43:40.000000 foo_et_al_parameterization-0.0.4/README.md
+-rw-rw-rw-   0        0        0      526 2024-06-02 19:47:24.000000 foo_et_al_parameterization-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 19:47:56.294730 foo_et_al_parameterization-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 19:47:56.259554 foo_et_al_parameterization-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 19:47:56.266554 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization/
+-rw-rw-rw-   0        0        0        2 2024-06-02 19:37:46.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization/__init__.py
+-rw-rw-rw-   0        0        0      409 2024-06-02 19:01:29.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization/foo-et-al-parameterization.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:47:56.291734 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/
+-rw-rw-rw-   0        0        0     1223 2024-06-02 19:47:56.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-06-02 19:47:56.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 19:47:56.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-06-02 19:47:56.000000 foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/top_level.txt
```

### Comparing `foo_et_al_parameterization-0.0.2/LICENSE` & `foo_et_al_parameterization-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `foo_et_al_parameterization-0.0.2/PKG-INFO` & `foo_et_al_parameterization-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foo-et-al-parameterization
-Version: 0.0.2
+Version: 0.0.4
 Summary: A basic python library to gain the volume of a sphere given its radius
 Author-email: Aidan Goldstein <goldstai@oregonstate.edu>
 Project-URL: Homepage, https://github.com/aidangold/foo-et-al-parameterization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -23,14 +23,14 @@
 This is a community focused project that is open source and values all contributions to improvements.
 
 ## Installation
 
 You can install the package via pip:
 
 ```bash
-pip install foo-et-al-parameterization
+pip install foo_et_al_parameterization
 ```
 Don't forget to import before using in a file!
 
 ```bash
-from foo-et-al-parameterization import sphere_volume
+from foo_et_al_parameterization import sphere_volume
 ```
```

### Comparing `foo_et_al_parameterization-0.0.2/README.md` & `foo_et_al_parameterization-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 This is a community focused project that is open source and values all contributions to improvements.
 
 ## Installation
 
 You can install the package via pip:
 
 ```bash
-pip install foo-et-al-parameterization
+pip install foo_et_al_parameterization
 ```
 Don't forget to import before using in a file!
 
 ```bash
-from foo-et-al-parameterization import sphere_volume
+from foo_et_al_parameterization import sphere_volume
 ```
```

### Comparing `foo_et_al_parameterization-0.0.2/pyproject.toml` & `foo_et_al_parameterization-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "foo-et-al-parameterization"
-version = "0.0.2"
+version = "0.0.4"
 authors = [
   { name ="Aidan Goldstein", email="goldstai@oregonstate.edu" },
 ]
 description = "A basic python library to gain the volume of a sphere given its radius"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `foo_et_al_parameterization-0.0.2/src/foo_et_al_parameterization.egg-info/PKG-INFO` & `foo_et_al_parameterization-0.0.4/src/foo_et_al_parameterization.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foo-et-al-parameterization
-Version: 0.0.2
+Version: 0.0.4
 Summary: A basic python library to gain the volume of a sphere given its radius
 Author-email: Aidan Goldstein <goldstai@oregonstate.edu>
 Project-URL: Homepage, https://github.com/aidangold/foo-et-al-parameterization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -23,14 +23,14 @@
 This is a community focused project that is open source and values all contributions to improvements.
 
 ## Installation
 
 You can install the package via pip:
 
 ```bash
-pip install foo-et-al-parameterization
+pip install foo_et_al_parameterization
 ```
 Don't forget to import before using in a file!
 
 ```bash
-from foo-et-al-parameterization import sphere_volume
+from foo_et_al_parameterization import sphere_volume
 ```
```

