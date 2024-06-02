# Comparing `tmp/pkg_vers-0.0.2.tar.gz` & `tmp/pkg_vers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_vers-0.0.2.tar", last modified: Sun Jun  2 15:33:29 2024, max compression
+gzip compressed data, was "pkg_vers-0.0.3.tar", last modified: Sun Jun  2 15:42:35 2024, max compression
```

## Comparing `pkg_vers-0.0.2.tar` & `pkg_vers-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:33:29.826215 pkg_vers-0.0.2/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 pkg_vers-0.0.2/LICENSE.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     2021 2024-06-02 15:33:29.825345 pkg_vers-0.0.2/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1529 2024-06-02 07:32:14.000000 pkg_vers-0.0.2/README.md
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:33:29.819530 pkg_vers-0.0.2/pkg_vers/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      263 2024-06-02 07:14:12.000000 pkg_vers-0.0.2/pkg_vers/__init__.py
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     2928 2024-06-02 15:31:43.000000 pkg_vers-0.0.2/pkg_vers/package_manager.py
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      851 2024-06-01 16:26:36.000000 pkg_vers-0.0.2/pkg_vers/utils.py
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:33:29.824463 pkg_vers-0.0.2/pkg_vers.egg-info/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     2021 2024-06-02 15:33:29.000000 pkg_vers-0.0.2/pkg_vers.egg-info/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      290 2024-06-02 15:33:29.000000 pkg_vers-0.0.2/pkg_vers.egg-info/SOURCES.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-06-02 15:33:29.000000 pkg_vers-0.0.2/pkg_vers.egg-info/dependency_links.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)        9 2024-06-02 15:33:29.000000 pkg_vers-0.0.2/pkg_vers.egg-info/top_level.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 pkg_vers-0.0.2/pyproject.toml
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-06-02 15:33:29.826470 pkg_vers-0.0.2/setup.cfg
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      684 2024-06-02 15:13:19.000000 pkg_vers-0.0.2/setup.py
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:33:29.822899 pkg_vers-0.0.2/tests/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      657 2024-06-02 07:04:23.000000 pkg_vers-0.0.2/tests/test_package_manager.py
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      469 2024-06-02 07:15:06.000000 pkg_vers-0.0.2/tests/test_utils.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:42:35.110057 pkg_vers-0.0.3/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 pkg_vers-0.0.3/LICENSE.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     2021 2024-06-02 15:42:35.109419 pkg_vers-0.0.3/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1529 2024-06-02 07:32:14.000000 pkg_vers-0.0.3/README.md
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:42:35.104184 pkg_vers-0.0.3/pkg_vers/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      305 2024-06-02 15:41:53.000000 pkg_vers-0.0.3/pkg_vers/__init__.py
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     2928 2024-06-02 15:31:43.000000 pkg_vers-0.0.3/pkg_vers/package_manager.py
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1135 2024-06-02 15:41:08.000000 pkg_vers-0.0.3/pkg_vers/utils.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:42:35.108607 pkg_vers-0.0.3/pkg_vers.egg-info/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     2021 2024-06-02 15:42:35.000000 pkg_vers-0.0.3/pkg_vers.egg-info/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      290 2024-06-02 15:42:35.000000 pkg_vers-0.0.3/pkg_vers.egg-info/SOURCES.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-06-02 15:42:35.000000 pkg_vers-0.0.3/pkg_vers.egg-info/dependency_links.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)        9 2024-06-02 15:42:35.000000 pkg_vers-0.0.3/pkg_vers.egg-info/top_level.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 pkg_vers-0.0.3/pyproject.toml
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-06-02 15:42:35.110207 pkg_vers-0.0.3/setup.cfg
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      684 2024-06-02 15:36:48.000000 pkg_vers-0.0.3/setup.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-06-02 15:42:35.107392 pkg_vers-0.0.3/tests/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      657 2024-06-02 07:04:23.000000 pkg_vers-0.0.3/tests/test_package_manager.py
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      469 2024-06-02 07:15:06.000000 pkg_vers-0.0.3/tests/test_utils.py
```

### Comparing `pkg_vers-0.0.2/LICENSE.txt` & `pkg_vers-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkg_vers-0.0.2/PKG-INFO` & `pkg_vers-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pkg_vers
-Version: 0.0.2
+Name: pkg-vers
+Version: 0.0.3
 Summary: pkg_vers is a utility to determine versions of top-level packages used in your project
 Home-page: https://github.com/chuckfinca/pkg_vers
 Author: Charles Feinn
 Author-email: chuckfinca@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pkg_vers-0.0.2/README.md` & `pkg_vers-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pkg_vers-0.0.2/pkg_vers/package_manager.py` & `pkg_vers-0.0.3/pkg_vers/package_manager.py`

 * *Files identical despite different names*

### Comparing `pkg_vers-0.0.2/pkg_vers/utils.py` & `pkg_vers-0.0.3/pkg_vers/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import os
 import subprocess
-import re
-import sys
 import logging
+from IPython.display import Javascript, display
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
+def retrieve_notebook_name():
+    display(Javascript('''
+    (function() {
+        var kernel = Jupyter.notebook.kernel;
+        var command = "notebook_name = '" + Jupyter.notebook.notebook_name + "'";
+        kernel.execute(command);
+    })();
+    '''))
+
 def find_all_py_files(directory):
     py_files = []
     for root, _, files in os.walk(directory):
         for file in files:
             if file.endswith('.py'):
                 py_files.append(os.path.join(root, file))
     return py_files
```

### Comparing `pkg_vers-0.0.2/pkg_vers.egg-info/PKG-INFO` & `pkg_vers-0.0.3/pkg_vers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pkg_vers
-Version: 0.0.2
+Name: pkg-vers
+Version: 0.0.3
 Summary: pkg_vers is a utility to determine versions of top-level packages used in your project
 Home-page: https://github.com/chuckfinca/pkg_vers
 Author: Charles Feinn
 Author-email: chuckfinca@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pkg_vers-0.0.2/setup.py` & `pkg_vers-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="pkg_vers",
-    version="0.0.2",
+    name="pkg-vers",
+    version="0.0.3",
     packages=find_packages(),
     author='Charles Feinn',
     author_email='chuckfinca@gmail.com',
     description="pkg_vers is a utility to determine versions of top-level packages used in your project",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chuckfinca/pkg_vers',
```

### Comparing `pkg_vers-0.0.2/tests/test_package_manager.py` & `pkg_vers-0.0.3/tests/test_package_manager.py`

 * *Files identical despite different names*

