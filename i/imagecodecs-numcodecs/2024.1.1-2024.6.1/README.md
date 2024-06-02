# Comparing `tmp/imagecodecs_numcodecs-2024.1.1-py3-none-any.whl.zip` & `tmp/imagecodecs_numcodecs-2024.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2773 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     4317 b- defN 23-Dec-31 05:30 imagecodecs_numcodecs-2024.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Dec-31 05:30 imagecodecs_numcodecs-2024.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2801 b- defN 23-Dec-31 05:30 imagecodecs_numcodecs-2024.1.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Dec-31 05:30 imagecodecs_numcodecs-2024.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      479 b- defN 23-Dec-31 05:30 imagecodecs_numcodecs-2024.1.1.dist-info/RECORD
-5 files, 7690 bytes uncompressed, 1865 bytes compressed:  75.7%
+Zip file size: 2801 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     4432 b- defN 24-Jun-02 18:16 imagecodecs_numcodecs-2024.6.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-02 18:16 imagecodecs_numcodecs-2024.6.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2905 b- defN 24-Jun-02 18:16 imagecodecs_numcodecs-2024.6.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Jun-02 18:16 imagecodecs_numcodecs-2024.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      479 b- defN 24-Jun-02 18:16 imagecodecs_numcodecs-2024.6.1.dist-info/RECORD
+5 files, 7909 bytes uncompressed, 1893 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: imagecodecs_numcodecs-2024.1.1.dist-info/METADATA
+Filename: imagecodecs_numcodecs-2024.6.1.dist-info/METADATA
 Comment: 
 
-Filename: imagecodecs_numcodecs-2024.1.1.dist-info/WHEEL
+Filename: imagecodecs_numcodecs-2024.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: imagecodecs_numcodecs-2024.1.1.dist-info/entry_points.txt
+Filename: imagecodecs_numcodecs-2024.6.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: imagecodecs_numcodecs-2024.1.1.dist-info/top_level.txt
+Filename: imagecodecs_numcodecs-2024.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: imagecodecs_numcodecs-2024.1.1.dist-info/RECORD
+Filename: imagecodecs_numcodecs-2024.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `imagecodecs_numcodecs-2024.1.1.dist-info/METADATA` & `imagecodecs_numcodecs-2024.6.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagecodecs-numcodecs
-Version: 2024.1.1
+Version: 2024.6.1
 Summary: Numcodecs entry points for the imagecodecs package
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 Project-URL: Bug Tracker, https://github.com/cgohlke/imagecodecs/issues
 Project-URL: Source Code, https://github.com/cgohlke/imagecodecs
 Platform: any
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Requires-Dist: numcodecs
-Requires-Dist: imagecodecs >=2024.1.1
+Requires-Dist: imagecodecs >=2024.6.1
 
 
 Imagecodecs_numcodecs is a Python package that registers the following 
 `Numcodecs <https://github.com/zarr-developers/numcodecs>`_ entry points 
 for the `Imagecodecs <https://github.com/cgohlke/imagecodecs>`_ package::
 
     imagecodecs_aec = imagecodecs.numcodecs:Aec
@@ -64,14 +64,16 @@
     imagecodecs_lzf = imagecodecs.numcodecs:Lzf
     imagecodecs_lzfse = imagecodecs.numcodecs:Lzfse
     imagecodecs_lzham = imagecodecs.numcodecs:Lzham
     imagecodecs_lzma = imagecodecs.numcodecs:Lzma
     imagecodecs_lzo = imagecodecs.numcodecs:Lzo
     imagecodecs_lzw = imagecodecs.numcodecs:Lzw
     imagecodecs_packbits = imagecodecs.numcodecs:Packbits
+    imagecodecs_packints = imagecodecs.numcodecs:Packints
+    imagecodecs_pcodec = imagecodecs.numcodecs:Pcodec
     imagecodecs_pglz = imagecodecs.numcodecs:Pglz
     imagecodecs_png = imagecodecs.numcodecs:Png
     imagecodecs_qoi = imagecodecs.numcodecs:Qoi
     imagecodecs_quantize = imagecodecs.numcodecs:Quantize
     imagecodecs_rcomp = imagecodecs.numcodecs:Rcomp
     imagecodecs_rgbe = imagecodecs.numcodecs:Rgbe
     imagecodecs_snappy = imagecodecs.numcodecs:Snappy
@@ -81,9 +83,9 @@
     imagecodecs_tiff = imagecodecs.numcodecs:Tiff
     imagecodecs_webp = imagecodecs.numcodecs:Webp
     imagecodecs_xor = imagecodecs.numcodecs:Xor
     imagecodecs_zfp = imagecodecs.numcodecs:Zfp
     imagecodecs_zlib = imagecodecs.numcodecs:Zlib
     imagecodecs_zlibng = imagecodecs.numcodecs:Zlibng
     imagecodecs_zopfli = imagecodecs.numcodecs:Zopfli
-    imagecodecs_zstd = imagecodecs.numcodecs:Zstd
+    imagecodecs_zstd = imagecodecs.numcodecs:Zstd'
```

## Comparing `imagecodecs_numcodecs-2024.1.1.dist-info/entry_points.txt` & `imagecodecs_numcodecs-2024.6.1.dist-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 imagecodecs_lzf = imagecodecs.numcodecs:Lzf
 imagecodecs_lzfse = imagecodecs.numcodecs:Lzfse
 imagecodecs_lzham = imagecodecs.numcodecs:Lzham
 imagecodecs_lzma = imagecodecs.numcodecs:Lzma
 imagecodecs_lzo = imagecodecs.numcodecs:Lzo
 imagecodecs_lzw = imagecodecs.numcodecs:Lzw
 imagecodecs_packbits = imagecodecs.numcodecs:Packbits
+imagecodecs_packints = imagecodecs.numcodecs:Packints
+imagecodecs_pcodec = imagecodecs.numcodecs:Pcodec
 imagecodecs_pglz = imagecodecs.numcodecs:Pglz
 imagecodecs_png = imagecodecs.numcodecs:Png
 imagecodecs_qoi = imagecodecs.numcodecs:Qoi
 imagecodecs_quantize = imagecodecs.numcodecs:Quantize
 imagecodecs_rcomp = imagecodecs.numcodecs:Rcomp
 imagecodecs_rgbe = imagecodecs.numcodecs:Rgbe
 imagecodecs_snappy = imagecodecs.numcodecs:Snappy
```

