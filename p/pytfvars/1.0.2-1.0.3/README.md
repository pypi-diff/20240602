# Comparing `tmp/pytfvars-1.0.2.tar.gz` & `tmp/pytfvars-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pytfvars/pytfvars/dist/.tmp-4r12xrp4/pytfvars-1.0.2.tar", last modified: Mon Jan 15 08:24:50 2024, max compression
+gzip compressed data, was "/home/runner/work/pytfvars/pytfvars/dist/.tmp-83j2mnju/pytfvars-1.0.3.tar", last modified: Sun Jun  2 09:38:09 2024, max compression
```

## Comparing `pytfvars-1.0.2.tar` & `pytfvars-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:24:50.000000 pytfvars-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-15 08:24:40.000000 pytfvars-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-01-15 08:24:50.000000 pytfvars-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-01-15 08:24:40.000000 pytfvars-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-15 08:24:40.000000 pytfvars-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 08:24:50.000000 pytfvars-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-15 08:24:40.000000 pytfvars-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:24:50.000000 pytfvars-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:24:50.000000 pytfvars-1.0.2/src/pytfvars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 08:24:40.000000 pytfvars-1.0.2/src/pytfvars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-01-15 08:24:40.000000 pytfvars-1.0.2/src/pytfvars/tfvars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:24:50.000000 pytfvars-1.0.2/src/pytfvars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-01-15 08:24:50.000000 pytfvars-1.0.2/src/pytfvars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-15 08:24:50.000000 pytfvars-1.0.2/src/pytfvars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 08:24:50.000000 pytfvars-1.0.2/src/pytfvars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-15 08:24:50.000000 pytfvars-1.0.2/src/pytfvars.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 08:24:50.000000 pytfvars-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-01-15 08:24:40.000000 pytfvars-1.0.2/tests/test_tfvars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:38:09.000000 pytfvars-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-02 09:38:02.000000 pytfvars-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-06-02 09:38:09.000000 pytfvars-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-06-02 09:38:02.000000 pytfvars-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-06-02 09:38:02.000000 pytfvars-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 09:38:09.000000 pytfvars-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-06-02 09:38:02.000000 pytfvars-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:38:09.000000 pytfvars-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:38:09.000000 pytfvars-1.0.3/src/pytfvars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 09:38:02.000000 pytfvars-1.0.3/src/pytfvars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-06-02 09:38:02.000000 pytfvars-1.0.3/src/pytfvars/tfvars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:38:09.000000 pytfvars-1.0.3/src/pytfvars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-06-02 09:38:09.000000 pytfvars-1.0.3/src/pytfvars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-06-02 09:38:09.000000 pytfvars-1.0.3/src/pytfvars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 09:38:09.000000 pytfvars-1.0.3/src/pytfvars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 09:38:09.000000 pytfvars-1.0.3/src/pytfvars.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:38:09.000000 pytfvars-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-06-02 09:38:02.000000 pytfvars-1.0.3/tests/test_tfvars.py
```

### Comparing `pytfvars-1.0.2/LICENSE.txt` & `pytfvars-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytfvars-1.0.2/PKG-INFO` & `pytfvars-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytfvars
-Version: 1.0.2
+Version: 1.0.3
 Summary: convert python dictionary to tfvars(hcl lang) formatted string
 Home-page: https://github.com/hohoonsong/pytfvars
 Author: hohoonsong
 Author-email: hohoonsong@gmail.com
 Project-URL: Bug Tracker, https://github.com/hohoonsong/pytfvars/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytfvars-1.0.2/README.md` & `pytfvars-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pytfvars-1.0.2/setup.py` & `pytfvars-1.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytfvars",
-    version="1.0.2",
+    version="1.0.3",
     author="hohoonsong",
     author_email="hohoonsong@gmail.com",
     description="convert python dictionary to tfvars(hcl lang) formatted string",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hohoonsong/pytfvars",
     project_urls={
```

### Comparing `pytfvars-1.0.2/src/pytfvars/tfvars.py` & `pytfvars-1.0.3/src/pytfvars/tfvars.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,9 +102,8 @@
             contents = '{}{}{}\n'.format(contents, indent_str, ']')
         elif type(v) is bool:
             contents = __convert_bool(contents, k, v, indent_no)
         elif type(v) is str:
             contents = __convert_str_kv(contents, k, v, indent_no)
 
     contents = __remove_empty_lines(contents)
-    print(contents)
     return contents
```

### Comparing `pytfvars-1.0.2/src/pytfvars.egg-info/PKG-INFO` & `pytfvars-1.0.3/src/pytfvars.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytfvars
-Version: 1.0.2
+Version: 1.0.3
 Summary: convert python dictionary to tfvars(hcl lang) formatted string
 Home-page: https://github.com/hohoonsong/pytfvars
 Author: hohoonsong
 Author-email: hohoonsong@gmail.com
 Project-URL: Bug Tracker, https://github.com/hohoonsong/pytfvars/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytfvars-1.0.2/tests/test_tfvars.py` & `pytfvars-1.0.3/tests/test_tfvars.py`

 * *Files identical despite different names*

