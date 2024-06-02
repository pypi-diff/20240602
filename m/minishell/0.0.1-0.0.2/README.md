# Comparing `tmp/minishell-0.0.1.tar.gz` & `tmp/minishell-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minishell-0.0.1.tar", max compression
+gzip compressed data, was "minishell-0.0.2.tar", max compression
```

## Comparing `minishell-0.0.1.tar` & `minishell-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       82 2024-06-02 08:20:27.767835 minishell-0.0.1/README.md
--rw-r--r--   0        0        0      550 2024-06-02 08:18:41.000000 minishell-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      799 2024-06-02 08:18:41.000000 minishell-0.0.1/src/minishell/__init__.py
--rw-r--r--   0        0        0     4832 2024-06-02 08:20:27.768835 minishell-0.0.1/src/minishell/cmd.py
--rw-r--r--   0        0        0     1400 2024-06-02 08:20:27.768835 minishell-0.0.1/src/minishell/config.py
--rw-r--r--   0        0        0     1518 2024-06-02 08:20:27.768835 minishell-0.0.1/src/minishell/error.py
--rw-r--r--   0        0        0     1994 2024-06-02 08:20:27.768835 minishell-0.0.1/src/minishell/logger.py
--rw-r--r--   0        0        0     1308 2024-06-02 08:20:27.768835 minishell-0.0.1/src/minishell/manual_test_run.py
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 minishell-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       82 2024-06-02 08:51:21.894575 minishell-0.0.2/README.md
+-rw-r--r--   0        0        0      550 2024-06-02 08:54:37.000000 minishell-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      799 2024-06-02 08:54:37.000000 minishell-0.0.2/src/minishell/__init__.py
+-rw-r--r--   0        0        0     4832 2024-06-02 08:51:21.895575 minishell-0.0.2/src/minishell/cmd.py
+-rw-r--r--   0        0        0     1400 2024-06-02 08:51:21.895575 minishell-0.0.2/src/minishell/config.py
+-rw-r--r--   0        0        0     1518 2024-06-02 08:51:21.895575 minishell-0.0.2/src/minishell/error.py
+-rw-r--r--   0        0        0     1994 2024-06-02 08:51:21.895575 minishell-0.0.2/src/minishell/logger.py
+-rw-r--r--   0        0        0     1308 2024-06-02 08:51:21.895575 minishell-0.0.2/src/minishell/manual_test_run.py
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 minishell-0.0.2/PKG-INFO
```

### Comparing `minishell-0.0.1/pyproject.toml` & `minishell-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "minishell"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["RomanLabs <rromanotero@romanlabs.com>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 packages = [{include = "minishell", from = "src"}]
 
 [tool.poetry.scripts]
```

### Comparing `minishell-0.0.1/src/minishell/__init__.py` & `minishell-0.0.2/src/minishell/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with API Pipe. If not, see <http://www.gnu.org/licenses/>.
 
 '''
     Module Name
 '''
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 __author__ = 'RomanLabs'
```

### Comparing `minishell-0.0.1/src/minishell/cmd.py` & `minishell-0.0.2/src/minishell/cmd.py`

 * *Files identical despite different names*

### Comparing `minishell-0.0.1/src/minishell/config.py` & `minishell-0.0.2/src/minishell/config.py`

 * *Files identical despite different names*

### Comparing `minishell-0.0.1/src/minishell/error.py` & `minishell-0.0.2/src/minishell/error.py`

 * *Files identical despite different names*

### Comparing `minishell-0.0.1/src/minishell/logger.py` & `minishell-0.0.2/src/minishell/logger.py`

 * *Files identical despite different names*

### Comparing `minishell-0.0.1/src/minishell/manual_test_run.py` & `minishell-0.0.2/src/minishell/manual_test_run.py`

 * *Files identical despite different names*

### Comparing `minishell-0.0.1/PKG-INFO` & `minishell-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minishell
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 License: LGPL-3.0-or-later
 Author: RomanLabs
 Author-email: rromanotero@romanlabs.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

