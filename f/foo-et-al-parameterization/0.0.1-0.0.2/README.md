# Comparing `tmp/foo_et_al_parameterization-0.0.1.tar.gz` & `tmp/foo_et_al_parameterization-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foo_et_al_parameterization-0.0.1.tar", last modified: Sun Jun  2 18:38:52 2024, max compression
+gzip compressed data, was "foo_et_al_parameterization-0.0.2.tar", last modified: Sun Jun  2 19:27:28 2024, max compression
```

## Comparing `foo_et_al_parameterization-0.0.1.tar` & `foo_et_al_parameterization-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 18:38:52.641797 foo_et_al_parameterization-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-06-02 18:35:49.000000 foo_et_al_parameterization-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      707 2024-06-02 18:38:52.639797 foo_et_al_parameterization-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-06-02 18:29:23.000000 foo_et_al_parameterization-0.0.1/README.md
--rw-rw-rw-   0        0        0      526 2024-06-02 18:38:46.000000 foo_et_al_parameterization-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-02 18:38:52.641797 foo_et_al_parameterization-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-02 18:38:52.611798 foo_et_al_parameterization-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-06-02 18:38:52.619798 foo_et_al_parameterization-0.0.1/src/foo-et-al-parameterization/
--rw-rw-rw-   0        0        0        0 2024-06-02 18:10:47.000000 foo_et_al_parameterization-0.0.1/src/foo-et-al-parameterization/__init__.py
--rw-rw-rw-   0        0        0      264 2024-06-02 18:35:10.000000 foo_et_al_parameterization-0.0.1/src/foo-et-al-parameterization/foo-et-al-parameterization.py
-drwxrwxrwx   0        0        0        0 2024-06-02 18:38:52.638797 foo_et_al_parameterization-0.0.1/src/foo_et_al_parameterization.egg-info/
--rw-rw-rw-   0        0        0      707 2024-06-02 18:38:52.000000 foo_et_al_parameterization-0.0.1/src/foo_et_al_parameterization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-06-02 18:38:52.000000 foo_et_al_parameterization-0.0.1/src/foo_et_al_parameterization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 18:38:52.000000 foo_et_al_parameterization-0.0.1/src/foo_et_al_parameterization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-06-02 18:38:52.000000 foo_et_al_parameterization-0.0.1/src/foo_et_al_parameterization.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 19:27:28.082056 foo_et_al_parameterization-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-06-02 18:35:49.000000 foo_et_al_parameterization-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1223 2024-06-02 19:27:28.081056 foo_et_al_parameterization-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-06-02 19:11:11.000000 foo_et_al_parameterization-0.0.2/README.md
+-rw-rw-rw-   0        0        0      526 2024-06-02 19:14:46.000000 foo_et_al_parameterization-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 19:27:28.083063 foo_et_al_parameterization-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 19:27:28.057062 foo_et_al_parameterization-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 19:27:28.066055 foo_et_al_parameterization-0.0.2/src/foo-et-al-parameterization/
+-rw-rw-rw-   0        0        0        0 2024-06-02 18:10:47.000000 foo_et_al_parameterization-0.0.2/src/foo-et-al-parameterization/__init__.py
+-rw-rw-rw-   0        0        0      409 2024-06-02 19:01:29.000000 foo_et_al_parameterization-0.0.2/src/foo-et-al-parameterization/foo-et-al-parameterization.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:27:28.079055 foo_et_al_parameterization-0.0.2/src/foo_et_al_parameterization.egg-info/
+-rw-rw-rw-   0        0        0     1223 2024-06-02 19:27:28.000000 foo_et_al_parameterization-0.0.2/src/foo_et_al_parameterization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-06-02 19:27:28.000000 foo_et_al_parameterization-0.0.2/src/foo_et_al_parameterization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 19:27:28.000000 foo_et_al_parameterization-0.0.2/src/foo_et_al_parameterization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-06-02 19:27:28.000000 foo_et_al_parameterization-0.0.2/src/foo_et_al_parameterization.egg-info/top_level.txt
```

### Comparing `foo_et_al_parameterization-0.0.1/LICENSE` & `foo_et_al_parameterization-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `foo_et_al_parameterization-0.0.1/pyproject.toml` & `foo_et_al_parameterization-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "foo-et-al-parameterization"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name ="Aidan Goldstein", email="goldstai@oregonstate.edu" },
 ]
 description = "A basic python library to gain the volume of a sphere given its radius"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

