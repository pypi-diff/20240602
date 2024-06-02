# Comparing `tmp/typer_shell-0.1.8.tar.gz` & `tmp/typer_shell-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_shell-0.1.8.tar", max compression
+gzip compressed data, was "typer_shell-0.1.9.tar", max compression
```

## Comparing `typer_shell-0.1.8.tar` & `typer_shell-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35150 2024-01-24 15:07:17.650220 typer_shell-0.1.8/LICENSE
--rw-r--r--   0        0        0     1653 2023-05-23 10:10:15.036154 typer_shell-0.1.8/README.md
--rw-r--r--   0        0        0      536 2024-02-14 09:37:26.242072 typer_shell-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      404 2023-09-24 13:23:43.066522 typer_shell-0.1.8/typer_shell/__init__.py
--rw-r--r--   0        0        0     7673 2024-02-14 09:37:23.225624 typer_shell-0.1.8/typer_shell/typer_shell.py
--rw-r--r--   0        0        0     1136 2023-05-27 12:03:50.620414 typer_shell-0.1.8/typer_shell/utils.py
--rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 typer_shell-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35150 2024-01-24 15:07:17.650220 typer_shell-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1653 2023-05-23 10:10:15.036154 typer_shell-0.1.9/README.md
+-rw-r--r--   0        0        0      536 2024-06-02 11:11:48.442749 typer_shell-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-09-24 13:23:43.066522 typer_shell-0.1.9/typer_shell/__init__.py
+-rw-r--r--   0        0        0     7673 2024-02-14 09:37:23.225624 typer_shell-0.1.9/typer_shell/typer_shell.py
+-rw-r--r--   0        0        0     1136 2023-05-27 12:03:50.620414 typer_shell-0.1.9/typer_shell/utils.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 typer_shell-0.1.9/PKG-INFO
```

### Comparing `typer_shell-0.1.8/LICENSE` & `typer_shell-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_shell-0.1.8/README.md` & `typer_shell-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `typer_shell-0.1.8/pyproject.toml` & `typer_shell-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "typer-shell"
-version = "0.1.8"
+version = "0.1.9"
 description = "A shell for typer apps with autocompletion and history"
 authors = ["fergus <fergusfettes@gmail.com>"]
 readme = "README.md"
 packages = [{include = "typer_shell"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.12"
+python = ">=3.8.1,<3.13"
 typer = "^0.9.0"
 click = "^8.1.3"
 rich = "^13.3.5"
 click-shell = "^2.1"
 iterfzf = "^0.5.0.20.0"
 pyyaml = "^6.0"
```

### Comparing `typer_shell-0.1.8/typer_shell/typer_shell.py` & `typer_shell-0.1.9/typer_shell/typer_shell.py`

 * *Files identical despite different names*

### Comparing `typer_shell-0.1.8/typer_shell/utils.py` & `typer_shell-0.1.9/typer_shell/utils.py`

 * *Files identical despite different names*

### Comparing `typer_shell-0.1.8/PKG-INFO` & `typer_shell-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: typer-shell
-Version: 0.1.8
+Version: 0.1.9
 Summary: A shell for typer apps with autocompletion and history
 Author: fergus
 Author-email: fergusfettes@gmail.com
-Requires-Python: >=3.8.1,<3.12
+Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-shell (>=2.1,<3.0)
 Requires-Dist: iterfzf (>=0.5.0.20.0,<0.6.0.0.0)
```

