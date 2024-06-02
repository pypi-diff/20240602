# Comparing `tmp/gspread_delimited_export-0.2.1.tar.gz` & `tmp/gspread_delimited_export-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspread_delimited_export-0.2.1.tar", max compression
+gzip compressed data, was "gspread_delimited_export-0.2.2.tar", max compression
```

## Comparing `gspread_delimited_export-0.2.1.tar` & `gspread_delimited_export-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      245 2024-06-01 20:43:49.269681 gspread_delimited_export-0.2.1/README.md
--rw-r--r--   0        0        0      664 2024-06-01 20:51:56.993147 gspread_delimited_export-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 19:25:40.774331 gspread_delimited_export-0.2.1/src/gspread_delimited_export/__init__.py
--rwxr-xr-x   0        0        0     1543 2024-06-01 15:00:07.399216 gspread_delimited_export-0.2.1/src/gspread_delimited_export/cli.py
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 gspread_delimited_export-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      245 2024-06-01 20:43:49.269681 gspread_delimited_export-0.2.2/README.md
+-rw-r--r--   0        0        0      664 2024-06-02 19:07:47.192098 gspread_delimited_export-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 19:25:40.774331 gspread_delimited_export-0.2.2/src/gspread_delimited_export/__init__.py
+-rwxr-xr-x   0        0        0     1542 2024-06-02 19:07:27.106302 gspread_delimited_export-0.2.2/src/gspread_delimited_export/cli.py
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 gspread_delimited_export-0.2.2/PKG-INFO
```

### Comparing `gspread_delimited_export-0.2.1/pyproject.toml` & `gspread_delimited_export-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gspread-delimited-export"
-version = "0.2.1"
+version = "0.2.2"
 description = "This package provides a script to export sheet from a Google Spreadsheet to a delimited file"
 authors = ["Scott Burns <scott@lentigo.net>"]
 readme = "README.md"
 packages = [{ include = "gspread_delimited_export", from = "src" }]
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `gspread_delimited_export-0.2.1/src/gspread_delimited_export/cli.py` & `gspread_delimited_export-0.2.2/src/gspread_delimited_export/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         )
     )
     sh = gc.open_by_key(key)
     ws = sh.worksheet(worksheet)
 
     df = get_as_dataframe(ws, evaluate_formulas=True, dtype=str, dialect="excel")
     df.dropna(axis="index", how="all", inplace=True)
-    df.dropna(axis="columns", how="all", inplace=False)
+    df.dropna(axis="columns", how="all", inplace=True)
 
     # normalize column names
     df.columns = ["_".join(header.split()).lower() for header in list(df.columns)]
 
     if type == "tsv":
         df.to_csv(output, index=False, sep="\t")
     else:
```

### Comparing `gspread_delimited_export-0.2.1/PKG-INFO` & `gspread_delimited_export-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspread-delimited-export
-Version: 0.2.1
+Version: 0.2.2
 Summary: This package provides a script to export sheet from a Google Spreadsheet to a delimited file
 License: MIT
 Author: Scott Burns
 Author-email: scott@lentigo.net
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

