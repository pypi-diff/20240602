# Comparing `tmp/pycountries-1.0.2.tar.gz` & `tmp/pycountries-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycountries-1.0.2.tar", last modified: Sat May  4 20:50:44 2024, max compression
+gzip compressed data, was "pycountries-1.0.3.tar", last modified: Sun Jun  2 17:27:48 2024, max compression
```

## Comparing `pycountries-1.0.2.tar` & `pycountries-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:50:44.945775 pycountries-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-04 20:50:39.000000 pycountries-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-04 20:50:44.945775 pycountries-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-04 20:50:39.000000 pycountries-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-04 20:50:39.000000 pycountries-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 20:50:44.945775 pycountries-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-04 20:50:39.000000 pycountries-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:50:44.941775 pycountries-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:50:44.941775 pycountries-1.0.2/src/pycountries/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    47277 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/countries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30868 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    85082 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/languages.py
--rw-r--r--   0 runner    (1001) docker     (127)    43057 2024-05-04 20:50:39.000000 pycountries-1.0.2/src/pycountries/phones.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:50:44.945775 pycountries-1.0.2/src/pycountries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-04 20:50:44.000000 pycountries-1.0.2/src/pycountries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-04 20:50:44.000000 pycountries-1.0.2/src/pycountries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 20:50:44.000000 pycountries-1.0.2/src/pycountries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 20:50:44.000000 pycountries-1.0.2/src/pycountries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 20:50:44.000000 pycountries-1.0.2/src/pycountries.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:50:44.945775 pycountries-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-04 20:50:39.000000 pycountries-1.0.2/tests/test_currencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:27:48.039823 pycountries-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-02 17:27:43.000000 pycountries-1.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-06-02 17:27:48.039823 pycountries-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-06-02 17:27:43.000000 pycountries-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-06-02 17:27:43.000000 pycountries-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:27:48.039823 pycountries-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-06-02 17:27:43.000000 pycountries-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:27:48.035823 pycountries-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:27:48.035823 pycountries-1.0.3/src/pycountries/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-06-02 17:27:43.000000 pycountries-1.0.3/src/pycountries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-02 17:27:43.000000 pycountries-1.0.3/src/pycountries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47277 2024-06-02 17:27:43.000000 pycountries-1.0.3/src/pycountries/countries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30868 2024-06-02 17:27:43.000000 pycountries-1.0.3/src/pycountries/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85082 2024-06-02 17:27:43.000000 pycountries-1.0.3/src/pycountries/languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43057 2024-06-02 17:27:43.000000 pycountries-1.0.3/src/pycountries/phones.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:27:48.039823 pycountries-1.0.3/src/pycountries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-06-02 17:27:48.000000 pycountries-1.0.3/src/pycountries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-02 17:27:48.000000 pycountries-1.0.3/src/pycountries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:27:48.000000 pycountries-1.0.3/src/pycountries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 17:27:48.000000 pycountries-1.0.3/src/pycountries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-02 17:27:48.000000 pycountries-1.0.3/src/pycountries.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:27:48.039823 pycountries-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-06-02 17:27:43.000000 pycountries-1.0.3/tests/test_currencies.py
```

### Comparing `pycountries-1.0.2/LICENSE.md` & `pycountries-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.2/PKG-INFO` & `pycountries-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycountries
-Version: 1.0.2
+Version: 1.0.3
 Summary: List of existing countries and currencies
 Home-page: https://github.com/koldakov/pycountries
 Author: Ivan Koldakov
 Author-email: Ivan Koldakov <ivan@koldakov.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/koldakov/pycountries
 Project-URL: Issues, https://github.com/koldakov/pycountries/issues
```

### Comparing `pycountries-1.0.2/README.md` & `pycountries-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.2/pyproject.toml` & `pycountries-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pycountries"
-version = "1.0.2"
+version = "1.0.3"
 license = {text = "MIT License"}
 authors = [
   { name="Ivan Koldakov", email="ivan@koldakov.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pycountries-1.0.2/src/pycountries/__init__.py` & `pycountries-1.0.3/src/pycountries/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     WrongAmountDigitsNumberError,
     WrongAmountTypeError,
     ZeroAmountNotAllowedError,
 )
 from pycountries.languages import Language
 from pycountries.phones import Phone
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __author__ = "Ivan Koldakov"
 __all__ = [
     "AmountSpecialValuesNotAllowedError",
     "Country",
     "Currency",
     "Language",
     "NegativeAmountNotAllowedError",
```

### Comparing `pycountries-1.0.2/src/pycountries/_base.py` & `pycountries-1.0.3/src/pycountries/_base.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.2/src/pycountries/countries.py` & `pycountries-1.0.3/src/pycountries/countries.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.2/src/pycountries/currencies.py` & `pycountries-1.0.3/src/pycountries/currencies.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.2/src/pycountries/languages.py` & `pycountries-1.0.3/src/pycountries/languages.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.2/src/pycountries/phones.py` & `pycountries-1.0.3/src/pycountries/phones.py`

 * *Files identical despite different names*

### Comparing `pycountries-1.0.2/src/pycountries.egg-info/PKG-INFO` & `pycountries-1.0.3/src/pycountries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycountries
-Version: 1.0.2
+Version: 1.0.3
 Summary: List of existing countries and currencies
 Home-page: https://github.com/koldakov/pycountries
 Author: Ivan Koldakov
 Author-email: Ivan Koldakov <ivan@koldakov.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/koldakov/pycountries
 Project-URL: Issues, https://github.com/koldakov/pycountries/issues
```

### Comparing `pycountries-1.0.2/tests/test_currencies.py` & `pycountries-1.0.3/tests/test_currencies.py`

 * *Files identical despite different names*

