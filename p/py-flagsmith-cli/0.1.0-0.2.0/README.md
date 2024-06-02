# Comparing `tmp/py_flagsmith_cli-0.1.0.tar.gz` & `tmp/py_flagsmith_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_flagsmith_cli-0.1.0.tar", last modified: Sun Jun  2 14:09:25 2024, max compression
+gzip compressed data, was "py_flagsmith_cli-0.2.0.tar", last modified: Sun Jun  2 14:22:31 2024, max compression
```

## Comparing `py_flagsmith_cli-0.1.0.tar` & `py_flagsmith_cli-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      158 2024-06-02 13:53:42.473299 py_flagsmith_cli-0.1.0/README.md
--rw-r--r--   0        0        0       53 2024-06-02 13:49:46.581061 py_flagsmith_cli-0.1.0/py_flagsmith_cli/__init__.py
--rw-r--r--   0        0        0       59 2024-06-01 11:42:10.260550 py_flagsmith_cli-0.1.0/py_flagsmith_cli/__main__.py
--rw-r--r--   0        0        0      355 2024-06-02 12:54:28.594925 py_flagsmith_cli-0.1.0/py_flagsmith_cli/cli.py
--rw-r--r--   0        0        0     6142 2024-06-02 13:18:10.560202 py_flagsmith_cli-0.1.0/py_flagsmith_cli/clis/get.py
--rw-r--r--   0        0        0     1313 2024-06-02 13:44:01.399153 py_flagsmith_cli-0.1.0/py_flagsmith_cli/clis/showenv.py
--rw-r--r--   0        0        0      159 2024-06-02 12:42:46.510348 py_flagsmith_cli-0.1.0/py_flagsmith_cli/constant.py
--rw-r--r--   0        0        0      883 2024-06-02 13:18:14.121680 py_flagsmith_cli-0.1.0/py_flagsmith_cli/utils.py
--rw-r--r--   0        0        0     1323 2024-06-02 14:09:25.186965 py_flagsmith_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1891 2024-06-01 11:43:03.803849 py_flagsmith_cli-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 13:32:57.627945 py_flagsmith_cli-0.1.0/tests/clis/__init__.py
--rw-r--r--   0        0        0     7660 2024-06-02 13:26:03.552719 py_flagsmith_cli-0.1.0/tests/clis/test_get.py
--rw-r--r--   0        0        0     1740 2024-06-02 13:47:26.108567 py_flagsmith_cli-0.1.0/tests/clis/test_showenv.py
--rw-r--r--   0        0        0       42 2024-06-01 13:29:14.438520 py_flagsmith_cli-0.1.0/tests/mockdata/__init__.py
--rw-r--r--   0        0        0     1011 2024-06-01 13:28:13.395307 py_flagsmith_cli-0.1.0/tests/mockdata/clis/get.py
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 py_flagsmith_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      213 2024-06-02 14:20:29.346214 py_flagsmith_cli-0.2.0/README.md
+-rw-r--r--   0        0        0       53 2024-06-02 14:22:06.045023 py_flagsmith_cli-0.2.0/py_flagsmith_cli/__init__.py
+-rw-r--r--   0        0        0       59 2024-06-01 11:42:10.260550 py_flagsmith_cli-0.2.0/py_flagsmith_cli/__main__.py
+-rw-r--r--   0        0        0      355 2024-06-02 12:54:28.594925 py_flagsmith_cli-0.2.0/py_flagsmith_cli/cli.py
+-rw-r--r--   0        0        0     6142 2024-06-02 13:18:10.560202 py_flagsmith_cli-0.2.0/py_flagsmith_cli/clis/get.py
+-rw-r--r--   0        0        0     1313 2024-06-02 13:44:01.399153 py_flagsmith_cli-0.2.0/py_flagsmith_cli/clis/showenv.py
+-rw-r--r--   0        0        0      159 2024-06-02 12:42:46.510348 py_flagsmith_cli-0.2.0/py_flagsmith_cli/constant.py
+-rw-r--r--   0        0        0      883 2024-06-02 13:18:14.121680 py_flagsmith_cli-0.2.0/py_flagsmith_cli/utils.py
+-rw-r--r--   0        0        0     1323 2024-06-02 14:22:31.029557 py_flagsmith_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1891 2024-06-01 11:43:03.803849 py_flagsmith_cli-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 13:32:57.627945 py_flagsmith_cli-0.2.0/tests/clis/__init__.py
+-rw-r--r--   0        0        0     7660 2024-06-02 13:26:03.552719 py_flagsmith_cli-0.2.0/tests/clis/test_get.py
+-rw-r--r--   0        0        0     1740 2024-06-02 13:47:26.108567 py_flagsmith_cli-0.2.0/tests/clis/test_showenv.py
+-rw-r--r--   0        0        0       42 2024-06-01 13:29:14.438520 py_flagsmith_cli-0.2.0/tests/mockdata/__init__.py
+-rw-r--r--   0        0        0     1011 2024-06-01 13:28:13.395307 py_flagsmith_cli-0.2.0/tests/mockdata/clis/get.py
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 py_flagsmith_cli-0.2.0/PKG-INFO
```

### Comparing `py_flagsmith_cli-0.1.0/py_flagsmith_cli/clis/get.py` & `py_flagsmith_cli-0.2.0/py_flagsmith_cli/clis/get.py`

 * *Files identical despite different names*

### Comparing `py_flagsmith_cli-0.1.0/py_flagsmith_cli/clis/showenv.py` & `py_flagsmith_cli-0.2.0/py_flagsmith_cli/clis/showenv.py`

 * *Files identical despite different names*

### Comparing `py_flagsmith_cli-0.1.0/py_flagsmith_cli/utils.py` & `py_flagsmith_cli-0.2.0/py_flagsmith_cli/utils.py`

 * *Files identical despite different names*

### Comparing `py_flagsmith_cli-0.1.0/pyproject.toml` & `py_flagsmith_cli-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "0.1.0"
+version = "0.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 pysmith = "py_flagsmith_cli.cli:app"
```

### Comparing `py_flagsmith_cli-0.1.0/tests/__init__.py` & `py_flagsmith_cli-0.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `py_flagsmith_cli-0.1.0/tests/clis/test_get.py` & `py_flagsmith_cli-0.2.0/tests/clis/test_get.py`

 * *Files identical despite different names*

### Comparing `py_flagsmith_cli-0.1.0/tests/clis/test_showenv.py` & `py_flagsmith_cli-0.2.0/tests/clis/test_showenv.py`

 * *Files identical despite different names*

### Comparing `py_flagsmith_cli-0.1.0/tests/mockdata/clis/get.py` & `py_flagsmith_cli-0.2.0/tests/mockdata/clis/get.py`

 * *Files identical despite different names*

### Comparing `py_flagsmith_cli-0.1.0/PKG-INFO` & `py_flagsmith_cli-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-flagsmith-cli
-Version: 0.1.0
+Version: 0.2.0
 Summary: flagsmith-cli Python Implementation.
 Author-Email: belingud <im.victor@qq.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,14 +14,15 @@
 Requires-Dist: typer>=0.12.3
 Requires-Dist: requests>=2.32.3
 Requires-Dist: python-dotenv>=1.0.1
 Description-Content-Type: text/markdown
 
 # py-flagsmith-cli
 
-
 flagsmith-cli Python Implementation.
 
+Homepage: https://github.com/belingud/py-flagsmith-cli
+
 Refer to:
 
 1. https://docs.flagsmith.com/clients/CLI
 2. https://github.com/Flagsmith/flagsmith-cli
```

