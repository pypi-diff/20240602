# Comparing `tmp/masthay_helpers-0.2.96-py3-none-macosx_11_0_arm64.whl.zip` & `tmp/masthay_helpers-0.2.97-py3-none-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 20045 bytes, number of entries: 12
--rw-r--r--  2.0 unx      308 b- defN 24-May-22 05:02 mh/__init__.py
--rw-r--r--  2.0 unx    23311 b- defN 24-May-22 05:02 mh/core.py
--rw-r--r--  2.0 unx     4133 b- defN 24-May-22 05:02 mh/core_legacy.py
--rw-r--r--  2.0 unx       51 b- defN 24-May-22 05:02 mh/errors.py
--rw-r--r--  2.0 unx     4232 b- defN 24-May-22 05:02 mh/import_env.py
--rw-r--r--  2.0 unx     7394 b- defN 24-May-22 05:02 mh/jupyter.py
--rw-r--r--  2.0 unx    14178 b- defN 24-May-22 05:02 mh/typlotlib.py
--rw-r--r--  2.0 unx     4450 b- defN 24-May-22 05:02 mh/typlotlib_legacy.py
--rw-r--r--  2.0 unx     1361 b- defN 24-May-22 05:02 masthay_helpers-0.2.96.dist-info/METADATA
--rw-r--r--  2.0 unx      106 b- defN 24-May-22 05:02 masthay_helpers-0.2.96.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 24-May-22 05:02 masthay_helpers-0.2.96.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      908 b- defN 24-May-22 05:02 masthay_helpers-0.2.96.dist-info/RECORD
-12 files, 60435 bytes uncompressed, 18545 bytes compressed:  69.3%
+Zip file size: 20104 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      308 b- defN 24-Jun-02 19:23 mh/__init__.py
+-rw-r--r--  2.0 unx    23311 b- defN 24-Jun-02 19:23 mh/core.py
+-rw-r--r--  2.0 unx     4294 b- defN 24-Jun-02 19:23 mh/core_legacy.py
+-rw-r--r--  2.0 unx       51 b- defN 24-Jun-02 19:23 mh/errors.py
+-rw-r--r--  2.0 unx     4232 b- defN 24-Jun-02 19:23 mh/import_env.py
+-rw-r--r--  2.0 unx     7394 b- defN 24-Jun-02 19:23 mh/jupyter.py
+-rw-r--r--  2.0 unx    14178 b- defN 24-Jun-02 19:23 mh/typlotlib.py
+-rw-r--r--  2.0 unx     4450 b- defN 24-Jun-02 19:23 mh/typlotlib_legacy.py
+-rw-r--r--  2.0 unx     1361 b- defN 24-Jun-02 19:23 masthay_helpers-0.2.97.dist-info/METADATA
+-rw-r--r--  2.0 unx      106 b- defN 24-Jun-02 19:23 masthay_helpers-0.2.97.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 24-Jun-02 19:23 masthay_helpers-0.2.97.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      908 b- defN 24-Jun-02 19:23 masthay_helpers-0.2.97.dist-info/RECORD
+12 files, 60596 bytes uncompressed, 18604 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: mh/typlotlib.py
 Comment: 
 
 Filename: mh/typlotlib_legacy.py
 Comment: 
 
-Filename: masthay_helpers-0.2.96.dist-info/METADATA
+Filename: masthay_helpers-0.2.97.dist-info/METADATA
 Comment: 
 
-Filename: masthay_helpers-0.2.96.dist-info/WHEEL
+Filename: masthay_helpers-0.2.97.dist-info/WHEEL
 Comment: 
 
-Filename: masthay_helpers-0.2.96.dist-info/top_level.txt
+Filename: masthay_helpers-0.2.97.dist-info/top_level.txt
 Comment: 
 
-Filename: masthay_helpers-0.2.96.dist-info/RECORD
+Filename: masthay_helpers-0.2.97.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mh/core_legacy.py

```diff
@@ -135,8 +135,14 @@
     exc = [] if exc is None else exc
     full_inc = set(inc).difference(exc)
     return {k: d[k] for k in full_inc}
 
 
 def vco(s):
     """vanilla check output"""
-    return co(s, shell=True).decode('utf-8').strip()
+    try:
+        return co(s, shell=True).decode('utf-8').strip()
+    except CalledProcessError as e:
+        if "returned non-zero exit status 1" in str(e):
+            return ""
+        else:
+            raise e
```

## Comparing `masthay_helpers-0.2.96.dist-info/METADATA` & `masthay_helpers-0.2.97.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masthay-helpers
-Version: 0.2.96
+Version: 0.2.97
 Summary: Helper functions for repetitive and useful tasks
 Author: Tyler Masthay
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

## Comparing `masthay_helpers-0.2.96.dist-info/RECORD` & `masthay_helpers-0.2.97.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mh/__init__.py,sha256=8aCfNWpIjiYHXdBDiQ1csfwvTLV4M6AzsGX4Zyls8Fc,308
 mh/core.py,sha256=7lM9qjLb5qLfzOti28QvUkQdXekp4SROUMoK8hkbcMI,23311
-mh/core_legacy.py,sha256=M6HI-k50OIZ5-je6PtSgxK5ax2psD0TPDJfq7_25MXY,4133
+mh/core_legacy.py,sha256=YdsXYmBdkzbgneljleHcaiWiLeyvc-F6ZLhRlfJ0ijU,4294
 mh/errors.py,sha256=jDpCLCSGEcRCNJCxCdMZx_hr3__V8m8g5vGg88zamh4,51
 mh/import_env.py,sha256=ycv0sIvYrJReJgSRm6qF28EsQ06PNj3BBAhiErWcN4U,4232
 mh/jupyter.py,sha256=tWsOPBQUaVNjvJn0HIfnsTyY4NrG4qhvLL7XH3SBPQ4,7394
 mh/typlotlib.py,sha256=KaANXD9xLuEnkUEuCqp2odb10JEKNfDmKvwL1LMoR6U,14178
 mh/typlotlib_legacy.py,sha256=4tCla5R4ryQB81YqzUfGzryOwKP898hkK0reQCgNDmE,4450
-masthay_helpers-0.2.96.dist-info/METADATA,sha256=ADn95I-zbWQu2nQIiPQ1JFanaKu28rbbEcD2OkEy6eY,1361
-masthay_helpers-0.2.96.dist-info/WHEEL,sha256=S7b8YYk-yJ5La3yIsS368T2_Hd_9s929Seaql3JcY7Q,106
-masthay_helpers-0.2.96.dist-info/top_level.txt,sha256=8Pn8eTSlPGDH3Lgl_pW5A8ch7lAIInNkhVBsc7ro8pM,3
-masthay_helpers-0.2.96.dist-info/RECORD,,
+masthay_helpers-0.2.97.dist-info/METADATA,sha256=7abqEA5QJ1XsOvCiGIwyOz4PJXbg84pb04nMZRiDsc0,1361
+masthay_helpers-0.2.97.dist-info/WHEEL,sha256=S7b8YYk-yJ5La3yIsS368T2_Hd_9s929Seaql3JcY7Q,106
+masthay_helpers-0.2.97.dist-info/top_level.txt,sha256=8Pn8eTSlPGDH3Lgl_pW5A8ch7lAIInNkhVBsc7ro8pM,3
+masthay_helpers-0.2.97.dist-info/RECORD,,
```

