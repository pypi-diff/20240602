# Comparing `tmp/flake8-typing-collections-2.0.tar.gz` & `tmp/flake8_typing_collections-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-typing-collections-2.0.tar", last modified: Fri Jul 14 23:32:32 2023, max compression
+gzip compressed data, was "flake8_typing_collections-2.1.tar", last modified: Sun Jun  2 09:09:21 2024, max compression
```

## Comparing `flake8-typing-collections-2.0.tar` & `flake8_typing_collections-2.1.tar`

### file list

```diff
@@ -1,17 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:32.633916 flake8-typing-collections-2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-14 23:32:32.633916 flake8-typing-collections-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:32.633916 flake8-typing-collections-2.0/flake8_typing_collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/flake8_typing_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/flake8_typing_collections/ast_import_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/flake8_typing_collections/checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:32.633916 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-14 23:32:32.633916 flake8-typing-collections-2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:09:21.047426 flake8_typing_collections-2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-06-02 09:09:21.047426 flake8_typing_collections-2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:09:21.039426 flake8_typing_collections-2.1/flake8_typing_collections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/flake8_typing_collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/flake8_typing_collections/ast_import_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/flake8_typing_collections/checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:09:21.047426 flake8_typing_collections-2.1/flake8_typing_collections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-06-02 09:09:21.000000 flake8_typing_collections-2.1/flake8_typing_collections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-06-02 09:09:21.000000 flake8_typing_collections-2.1/flake8_typing_collections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 09:09:21.000000 flake8_typing_collections-2.1/flake8_typing_collections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-02 09:09:21.000000 flake8_typing_collections-2.1/flake8_typing_collections.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 09:09:21.000000 flake8_typing_collections-2.1/flake8_typing_collections.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-06-02 09:09:21.000000 flake8_typing_collections-2.1/flake8_typing_collections.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-06-02 09:09:21.047426 flake8_typing_collections-2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:09:21.047426 flake8_typing_collections-2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_ast_import_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_nested_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco102.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco103.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco104.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco105.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco106.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco107.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco108.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco109.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco110.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco111.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco112.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco113.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco114.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco115.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco116.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco117.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco118.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco119.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco120.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco121.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco122.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco123.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco124.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco125.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco126.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco127.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco129.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco130.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco131.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco132.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco201.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-06-02 09:09:06.000000 flake8_typing_collections-2.1/tests/test_tyco202.py
```

### Comparing `flake8-typing-collections-2.0/LICENSE` & `flake8_typing_collections-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-typing-collections-2.0/PKG-INFO` & `flake8_typing_collections-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-typing-collections
-Version: 2.0
+Version: 2.1
 Summary: A flake8 plugin that checks the use of type alternatives from the typing module over actual run time types, especially from the collections module.
 Home-page: https://github.com/atollk/flake8-typing-collections
 Author: Andreas Tollkötter
 License: MIT
 Keywords: flake8,typing,type-annotations
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flake8-typing-collections
 A flake8 plugin that checks the use of type alternatives from
 the `typing` module over actual run time types, especially from
```

### Comparing `flake8-typing-collections-2.0/README.md` & `flake8_typing_collections-2.1/README.md`

 * *Files identical despite different names*

### Comparing `flake8-typing-collections-2.0/flake8_typing_collections/ast_import_decode.py` & `flake8_typing_collections-2.1/flake8_typing_collections/ast_import_decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,17 @@
     :return: The name that is represented by the node, as a string.
     """
     if isinstance(node, ast.Name):
         return node.id
     elif isinstance(node, ast.Attribute):
         return _build_node_identifier(node.value) + "." + node.attr
     else:
-        raise TypeError("Can only decode nodes of type ast.Name and ast.Attribute.")
+        raise TypeError(
+            "Can only decode nodes of type ast.Name and ast.Attribute."
+        )
 
 
 def _ast_ancestors(tree: ast.AST, node: ast.AST) -> List[ast.AST]:
     """
     Finds a list of ancestors from a given node to its root.
 
     :param tree: The root of the given ast.
@@ -146,15 +148,23 @@
             assignments.append(statement)
         elif isinstance(statement, ast.Import):
             for alias in statement.names:
                 if alias.asname is not None:
                     potential_aliases[alias.asname].append(alias.name)
         elif isinstance(statement, ast.ImportFrom):
             for alias in statement.names:
-                fullname = ("." * statement.level) + statement.module + "." + alias.name
+                if statement.module is not None:
+                    fullname = (
+                        ("." * statement.level)
+                        + statement.module
+                        + "."
+                        + alias.name
+                    )
+                else:
+                    fullname = ("." * statement.level) + alias.name
                 if alias.asname is None:
                     potential_aliases[alias.name].append(fullname)
                 else:
                     potential_aliases[alias.asname].append(fullname)
         else:
             raise KeyError(f"{statement} cannot be analyzed.")
```

### Comparing `flake8-typing-collections-2.0/flake8_typing_collections/checker.py` & `flake8_typing_collections-2.1/flake8_typing_collections/checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,21 +188,26 @@
     def _use_better_alternative(
         self, type_hint: ast.AST, error_code: int
     ) -> Iterable[Tuple[int, int, str, type]]:
         if error_code in ERROR_CODES_GENERIC_ALT and not self.flags.generic_alt:
             return []
         if error_code in ERROR_CODES_ALIAS_ALT and not self.flags.alias_alt:
             return []
-        if error_code in ERROR_CODES_GENERAL_ARGS and not self.flags.general_args:
+        if (
+            error_code in ERROR_CODES_GENERAL_ARGS
+            and not self.flags.general_args
+        ):
             return []
 
         while isinstance(type_hint, ast.Subscript):
             type_hint = type_hint.value
 
-        if isinstance(type_hint, ast.Name) or isinstance(type_hint, ast.Attribute):
+        if isinstance(type_hint, ast.Name) or isinstance(
+            type_hint, ast.Attribute
+        ):
             if (
                 ast_import_decode.decode(self.tree, type_hint)
                 in BETTER_ALTERNATIVES[error_code]
             ):
                 yield (
                     type_hint.lineno,
                     type_hint.col_offset,
```

### Comparing `flake8-typing-collections-2.0/flake8_typing_collections.egg-info/PKG-INFO` & `flake8_typing_collections-2.1/flake8_typing_collections.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-typing-collections
-Version: 2.0
+Version: 2.1
 Summary: A flake8 plugin that checks the use of type alternatives from the typing module over actual run time types, especially from the collections module.
 Home-page: https://github.com/atollk/flake8-typing-collections
 Author: Andreas Tollkötter
 License: MIT
 Keywords: flake8,typing,type-annotations
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flake8-typing-collections
 A flake8 plugin that checks the use of type alternatives from
 the `typing` module over actual run time types, especially from
```

### Comparing `flake8-typing-collections-2.0/setup.cfg` & `flake8_typing_collections-2.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flake8-typing-collections
-version = 2.0
+version = 2.1
 description = A flake8 plugin that checks the use of type alternatives from the typing module over actual run time types, especially from the collections module.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Andreas Tollkötter
 url = https://github.com/atollk/flake8-typing-collections
 license = MIT
 license_file = LICENSE
@@ -16,14 +16,15 @@
 	Natural Language :: English
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
 packages = 
 	flake8_typing_collections
 include_package_data = True
 python_requires = >=3.8
 zip_safe = False
```

