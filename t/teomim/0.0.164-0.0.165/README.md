# Comparing `tmp/teomim-0.0.164.tar.gz` & `tmp/teomim-0.0.165.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teomim-0.0.164.tar", last modified: Thu Jan 25 22:34:03 2024, max compression
+gzip compressed data, was "teomim-0.0.165.tar", last modified: Thu Jan 25 23:03:30 2024, max compression
```

## Comparing `teomim-0.0.164.tar` & `teomim-0.0.165.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2024-01-25 22:34:03.371193 teomim-0.0.164/
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1065 2024-01-10 19:57:02.000000 teomim-0.0.164/LICENSE
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)      198 2024-01-13 02:40:05.000000 teomim-0.0.164/MANIFEST.in
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1596 2024-01-25 22:34:03.371193 teomim-0.0.164/PKG-INFO
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)      730 2024-01-13 02:40:05.000000 teomim-0.0.164/README.rst
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)       38 2024-01-25 22:34:03.371193 teomim-0.0.164/setup.cfg
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1796 2024-01-25 22:33:49.000000 teomim-0.0.164/setup.py
-drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2024-01-25 22:34:03.367193 teomim-0.0.164/teomim/
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1869 2024-01-13 02:40:05.000000 teomim-0.0.164/teomim/__init__.py
-drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2024-01-25 22:34:03.367193 teomim-0.0.164/teomim/assets/
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)  4006357 2024-01-13 02:40:05.000000 teomim-0.0.164/teomim/assets/adrd_5K_01.pkl.gz
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     6971 2024-01-25 22:31:21.000000 teomim-0.0.164/teomim/teomim.py
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)      247 2024-01-10 21:02:35.000000 teomim-0.0.164/teomim/viz.py
-drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2024-01-25 22:34:03.367193 teomim-0.0.164/teomim.egg-info/
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1596 2024-01-25 22:34:02.000000 teomim-0.0.164/teomim.egg-info/PKG-INFO
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)      281 2024-01-25 22:34:03.000000 teomim-0.0.164/teomim.egg-info/SOURCES.txt
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)        1 2024-01-25 22:34:02.000000 teomim-0.0.164/teomim.egg-info/dependency_links.txt
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)       55 2024-01-25 22:34:02.000000 teomim-0.0.164/teomim.egg-info/requires.txt
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)        7 2024-01-25 22:34:02.000000 teomim-0.0.164/teomim.egg-info/top_level.txt
--rw-r--r--   0 ishanu    (1000) ishanu    (1000)       24 2024-01-25 22:31:46.000000 teomim-0.0.164/version.py
+drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2024-01-25 23:03:30.340333 teomim-0.0.165/
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1065 2024-01-10 19:57:02.000000 teomim-0.0.165/LICENSE
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)      198 2024-01-13 02:40:05.000000 teomim-0.0.165/MANIFEST.in
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1596 2024-01-25 23:03:30.339333 teomim-0.0.165/PKG-INFO
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)      730 2024-01-13 02:40:05.000000 teomim-0.0.165/README.rst
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)       38 2024-01-25 23:03:30.340333 teomim-0.0.165/setup.cfg
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1796 2024-01-25 23:02:53.000000 teomim-0.0.165/setup.py
+drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2024-01-25 23:03:30.336333 teomim-0.0.165/teomim/
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1869 2024-01-13 02:40:05.000000 teomim-0.0.165/teomim/__init__.py
+drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2024-01-25 23:03:30.336333 teomim-0.0.165/teomim/assets/
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)  4006357 2024-01-13 02:40:05.000000 teomim-0.0.165/teomim/assets/adrd_5K_01.pkl.gz
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)     6971 2024-01-25 22:31:21.000000 teomim-0.0.165/teomim/teomim.py
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)      247 2024-01-10 21:02:35.000000 teomim-0.0.165/teomim/viz.py
+drwxr-xr-x   0 ishanu    (1000) ishanu    (1000)        0 2024-01-25 23:03:30.336333 teomim-0.0.165/teomim.egg-info/
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)     1596 2024-01-25 23:03:29.000000 teomim-0.0.165/teomim.egg-info/PKG-INFO
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)      281 2024-01-25 23:03:30.000000 teomim-0.0.165/teomim.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)        1 2024-01-25 23:03:29.000000 teomim-0.0.165/teomim.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)       55 2024-01-25 23:03:29.000000 teomim-0.0.165/teomim.egg-info/requires.txt
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)        7 2024-01-25 23:03:29.000000 teomim-0.0.165/teomim.egg-info/top_level.txt
+-rw-r--r--   0 ishanu    (1000) ishanu    (1000)       24 2024-01-25 22:34:16.000000 teomim-0.0.165/version.py
```

### Comparing `teomim-0.0.164/LICENSE` & `teomim-0.0.165/LICENSE`

 * *Files identical despite different names*

### Comparing `teomim-0.0.164/PKG-INFO` & `teomim-0.0.165/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: teomim
-Version: 0.0.164
+Version: 0.0.165
 Summary: Digital twin for generating and analyzing medical histories with deep comorbidity structures
 Home-page: https://github.com/zeroknowledgediscovery/teomim
-Download-URL: https://github.com/zeroknowledgediscovery/teomim/archive/0.0.164.tar.gz
+Download-URL: https://github.com/zeroknowledgediscovery/teomim/archive/0.0.165.tar.gz
 Author: paraknowledge corp
 Author-email: research@paraknowledge.ai
 License: LICENSE
 Keywords: machine learning,statistics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `teomim-0.0.164/README.rst` & `teomim-0.0.165/README.rst`

 * *Files identical despite different names*

### Comparing `teomim-0.0.164/setup.py` & `teomim-0.0.165/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     long_description=long_description,
     long_description_content_type='text/x-rst',
     install_requires=[
         "scikit-learn", 
         "scipy", 
         "numpy",  
         "pandas",
-        "quasinet>=0.1.62",
+        "quasinet>=0.1.63",
         "scipy"],
     python_requires='>=3.7',
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Information Analysis",
```

### Comparing `teomim-0.0.164/teomim/__init__.py` & `teomim-0.0.165/teomim/__init__.py`

 * *Files identical despite different names*

### Comparing `teomim-0.0.164/teomim/assets/adrd_5K_01.pkl.gz` & `teomim-0.0.165/teomim/assets/adrd_5K_01.pkl.gz`

 * *Files identical despite different names*

### Comparing `teomim-0.0.164/teomim/teomim.py` & `teomim-0.0.165/teomim/teomim.py`

 * *Files identical despite different names*

### Comparing `teomim-0.0.164/teomim.egg-info/PKG-INFO` & `teomim-0.0.165/teomim.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: teomim
-Version: 0.0.164
+Version: 0.0.165
 Summary: Digital twin for generating and analyzing medical histories with deep comorbidity structures
 Home-page: https://github.com/zeroknowledgediscovery/teomim
-Download-URL: https://github.com/zeroknowledgediscovery/teomim/archive/0.0.164.tar.gz
+Download-URL: https://github.com/zeroknowledgediscovery/teomim/archive/0.0.165.tar.gz
 Author: paraknowledge corp
 Author-email: research@paraknowledge.ai
 License: LICENSE
 Keywords: machine learning,statistics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

