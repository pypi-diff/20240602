# Comparing `tmp/fretbursts-0.8.1.tar.gz` & `tmp/fretbursts-0.8.2-cp37-cp37m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fretbursts-0.8.1.tar", last modified: Sun Jun  2 04:02:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

