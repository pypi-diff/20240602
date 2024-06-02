# Comparing `tmp/sif_tools-0.2-py3-none-any.whl.zip` & `tmp/sif_tools-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 20429 bytes, number of entries: 15
+Zip file size: 20458 bytes, number of entries: 15
 -rw-r--r--  2.0 unx    11034 b- defN 24-Jun-01 17:59 sif_tools/SIFopen.py
 -rw-r--r--  2.0 unx     8457 b- defN 24-Jun-01 23:42 sif_tools/SIFplot.py
 -rw-r--r--  2.0 unx     1588 b- defN 24-Jun-01 23:06 sif_tools/SIFpy.py
 -rw-r--r--  2.0 unx       55 b- defN 24-Jun-01 23:31 sif_tools/__init__.py
 -rw-r--r--  2.0 unx      460 b- defN 24-Jun-01 23:31 sif_tools/__main__.py
 -rw-r--r--  2.0 unx     7523 b- defN 24-Jun-01 23:14 sif_tools/utils.py
 -rw-r--r--  2.0 unx     6318 b- defN 24-Jun-01 23:18 sif_tools/CommandLine/CommandLineInterface.py
 -rw-r--r--  2.0 unx     2249 b- defN 24-Jun-01 23:35 sif_tools/CommandLine/CommandLineTools.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jun-01 22:31 sif_tools/CommandLine/__init__.py
--rw-r--r--  2.0 unx    14874 b- defN 24-Jun-02 00:18 sif_tools-0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4015 b- defN 24-Jun-02 00:18 sif_tools-0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-02 00:18 sif_tools-0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 24-Jun-02 00:18 sif_tools-0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-Jun-02 00:18 sif_tools-0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1227 b- defN 24-Jun-02 00:18 sif_tools-0.2.dist-info/RECORD
-15 files, 57956 bytes uncompressed, 18395 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx    14874 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4017 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1239 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/RECORD
+15 files, 57970 bytes uncompressed, 18400 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: sif_tools/CommandLine/CommandLineTools.py
 Comment: 
 
 Filename: sif_tools/CommandLine/__init__.py
 Comment: 
 
-Filename: sif_tools-0.2.dist-info/LICENSE
+Filename: sif_tools-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: sif_tools-0.2.dist-info/METADATA
+Filename: sif_tools-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: sif_tools-0.2.dist-info/WHEEL
+Filename: sif_tools-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: sif_tools-0.2.dist-info/entry_points.txt
+Filename: sif_tools-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sif_tools-0.2.dist-info/top_level.txt
+Filename: sif_tools-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sif_tools-0.2.dist-info/RECORD
+Filename: sif_tools-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sif_tools-0.2.dist-info/LICENSE` & `sif_tools-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sif_tools-0.2.dist-info/METADATA` & `sif_tools-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sif_tools
-Version: 0.2
+Version: 0.3.0
 Summary: A light-weight package for Andor SIF file analysis
 Home-page: https://github.com/BjornFS/SIF-Tools
 Author: Bjorn F. Schroder N.
 Author-email: Bjornfschroder@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

## Comparing `sif_tools-0.2.dist-info/RECORD` & `sif_tools-0.3.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 sif_tools/SIFpy.py,sha256=tCG00H1bplEolEhpJPubVpbrUN_8ZmzDG-EZPZjB0oY,1588
 sif_tools/__init__.py,sha256=p85vqN2shbLq5sAMRCBpt8c0vIYltBlPtqa5Zy4oxac,55
 sif_tools/__main__.py,sha256=iR9cpEf_WFEyC-uxVbTEXJHIQjA_XKYwi-StpbMJpNk,460
 sif_tools/utils.py,sha256=uKP4bTmItwtDfzlv_CRyjpq4Axbl1QF8oox9iparSU0,7523
 sif_tools/CommandLine/CommandLineInterface.py,sha256=6GIp8BN1GjJOVVfHhwE2-RpxbLUd-RJ84-XA2geYz38,6318
 sif_tools/CommandLine/CommandLineTools.py,sha256=fWa6nPUgH83vLIJPHFbYGMqUFIaoq9ORwqf7BJs1z9g,2249
 sif_tools/CommandLine/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sif_tools-0.2.dist-info/LICENSE,sha256=baLxFkeB7Yhvfd2bvZHGsxrX8T_0FeM0SOf8iPapzw8,14874
-sif_tools-0.2.dist-info/METADATA,sha256=jH3Z_P6RAoCpbWosOnZ0ZnlL3lMNcNYTaTryLQJ5__s,4015
-sif_tools-0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-sif_tools-0.2.dist-info/entry_points.txt,sha256=DqG3nDHpwF6a9Pi-8ic6LnI9j5GbrFF-VZHepRl22HM,54
-sif_tools-0.2.dist-info/top_level.txt,sha256=8EV42y0oQ9ntR0iu1o7m8YbEoQeY9FvOzrc1RJhEgzo,10
-sif_tools-0.2.dist-info/RECORD,,
+sif_tools-0.3.0.dist-info/LICENSE,sha256=baLxFkeB7Yhvfd2bvZHGsxrX8T_0FeM0SOf8iPapzw8,14874
+sif_tools-0.3.0.dist-info/METADATA,sha256=Ey7z29gRy0qO9SnDpox44DhDXwrWR80ZaAsIBcABB6s,4017
+sif_tools-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+sif_tools-0.3.0.dist-info/entry_points.txt,sha256=DqG3nDHpwF6a9Pi-8ic6LnI9j5GbrFF-VZHepRl22HM,54
+sif_tools-0.3.0.dist-info/top_level.txt,sha256=8EV42y0oQ9ntR0iu1o7m8YbEoQeY9FvOzrc1RJhEgzo,10
+sif_tools-0.3.0.dist-info/RECORD,,
```

