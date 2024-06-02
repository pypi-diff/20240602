# Comparing `tmp/changy-0.4.1.tar.gz` & `tmp/changy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changy-0.4.1.tar", max compression
+gzip compressed data, was "changy-0.4.2.tar", max compression
```

## Comparing `changy-0.4.1.tar` & `changy-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1504 2024-06-01 08:49:47.291402 changy-0.4.1/LICENSE
--rw-r--r--   0        0        0     2740 2024-06-01 08:49:47.291402 changy-0.4.1/README.md
--rw-r--r--   0        0        0        0 2024-06-01 08:49:47.291402 changy-0.4.1/changy/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 08:49:47.291402 changy-0.4.1/changy/cli/__init__.py
--rw-r--r--   0        0        0      381 2024-06-01 08:49:47.291402 changy-0.4.1/changy/cli/__main__.py
--rw-r--r--   0        0        0       34 2024-06-01 08:49:47.291402 changy-0.4.1/changy/cli/application.py
--rw-r--r--   0        0        0      175 2024-06-01 08:49:47.291402 changy-0.4.1/changy/cli/changelog.py
--rw-r--r--   0        0        0      287 2024-06-01 08:49:47.291402 changy-0.4.1/changy/cli/unreleased.py
--rw-r--r--   0        0        0      426 2024-06-01 08:49:47.291402 changy-0.4.1/changy/cli/version.py
--rw-r--r--   0        0        0      409 2024-06-01 08:49:47.291402 changy-0.4.1/changy/constants.py
--rw-r--r--   0        0        0     1592 2024-06-01 08:49:47.291402 changy-0.4.1/changy/errors.py
--rw-r--r--   0        0        0     3881 2024-06-01 08:49:47.291402 changy-0.4.1/changy/logic.py
--rw-r--r--   0        0        0      768 2024-06-01 08:49:47.291402 changy-0.4.1/changy/settings.py
--rw-r--r--   0        0        0        0 2024-06-01 08:49:47.291402 changy-0.4.1/changy/tests/__init__.py
--rw-r--r--   0        0        0       29 2024-06-01 08:49:47.295402 changy-0.4.1/changy/tests/test_logic.py
--rw-r--r--   0        0        0      231 2024-06-01 08:49:47.295402 changy-0.4.1/changy/utils.py
--rw-r--r--   0        0        0     1953 2024-06-01 08:49:55.103363 changy-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3830 1970-01-01 00:00:00.000000 changy-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-06-02 10:01:47.023345 changy-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2740 2024-06-02 10:01:47.023345 changy-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-06-02 10:01:47.023345 changy-0.4.2/changy/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:01:47.023345 changy-0.4.2/changy/cli/__init__.py
+-rw-r--r--   0        0        0      381 2024-06-02 10:01:47.023345 changy-0.4.2/changy/cli/__main__.py
+-rw-r--r--   0        0        0       34 2024-06-02 10:01:47.023345 changy-0.4.2/changy/cli/application.py
+-rw-r--r--   0        0        0      175 2024-06-02 10:01:47.023345 changy-0.4.2/changy/cli/changelog.py
+-rw-r--r--   0        0        0      287 2024-06-02 10:01:47.023345 changy-0.4.2/changy/cli/unreleased.py
+-rw-r--r--   0        0        0      426 2024-06-02 10:01:47.023345 changy-0.4.2/changy/cli/version.py
+-rw-r--r--   0        0        0      409 2024-06-02 10:01:47.023345 changy-0.4.2/changy/constants.py
+-rw-r--r--   0        0        0     1620 2024-06-02 10:01:47.023345 changy-0.4.2/changy/errors.py
+-rw-r--r--   0        0        0     4007 2024-06-02 10:01:47.027345 changy-0.4.2/changy/logic.py
+-rw-r--r--   0        0        0      768 2024-06-02 10:01:47.027345 changy-0.4.2/changy/settings.py
+-rw-r--r--   0        0        0        0 2024-06-02 10:01:47.027345 changy-0.4.2/changy/tests/__init__.py
+-rw-r--r--   0        0        0       29 2024-06-02 10:01:47.027345 changy-0.4.2/changy/tests/test_logic.py
+-rw-r--r--   0        0        0      231 2024-06-02 10:01:47.027345 changy-0.4.2/changy/utils.py
+-rw-r--r--   0        0        0     1953 2024-06-02 10:01:55.859359 changy-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3830 1970-01-01 00:00:00.000000 changy-0.4.2/PKG-INFO
```

### Comparing `changy-0.4.1/LICENSE` & `changy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `changy-0.4.1/README.md` & `changy-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `changy-0.4.1/changy/errors.py` & `changy-0.4.2/changy/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class ChangesDirDoesNotExist(ChangyError):
     message = "Changes directory ({directory}) does not exist"
 
 
 class AlreadyInitialized(ChangyError):
-    message = "Already initialized"
+    message = "Already initialized, file {file} already exists"
 
 
 class NoApprovedChanges(ChangyError):
     message = "No approved changes found ({file}). Ensure you edited unreleased changes file and called `changy unrelease approve`."  # noqa: E501
 
 
 class NoUnreleasedChanges(ChangyError):
```

### Comparing `changy-0.4.1/changy/logic.py` & `changy-0.4.2/changy/logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,19 +58,21 @@
 
     changes_list.sort(key=lambda x: x.time, reverse=True)
 
     return changes_list
 
 
 def init() -> None:
+    if not configs_dir.exists():
+        configs_dir.mkdir()
 
-    if configs_dir.exists():
-        raise errors.AlreadyInitialized()
+    for file in (header_file, changes_template_file, unreleased_changes_file):
+        if file.exists():
+            raise errors.AlreadyInitialized(file=file)
 
-    configs_dir.mkdir()
     header_file.write_text(c.default_changelog_header)
     changes_template_file.write_text(c.default_change_file_template)
 
     create_unreleased()
 
 
 def create_unreleased() -> None:
```

### Comparing `changy-0.4.1/changy/settings.py` & `changy-0.4.2/changy/settings.py`

 * *Files identical despite different names*

### Comparing `changy-0.4.1/pyproject.toml` & `changy-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "changy"
-version = "0.4.1"
+version = "0.4.2"
 description = "Simplest changelog manager, oriented to human editing, not to special message formatting in commits and tags.."
 readme = "README.md"
 repository = "https://github.com/Tiendil/changy"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = "BSD-3-Clause"
 keywords = ["changelog", "release-notes", "release-automation", "release-management", "changelog-generator", "changelog-formatter"]
 classifiers = [
```

### Comparing `changy-0.4.1/PKG-INFO` & `changy-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Simplest changelog manager, oriented to human editing, not to special message formatting in commits and tags..
 Home-page: https://github.com/Tiendil/changy
 License: BSD-3-Clause
 Keywords: changelog,release-notes,release-automation,release-management,changelog-generator,changelog-formatter
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
 Requires-Python: >=3.12,<4.0
```

