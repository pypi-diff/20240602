# Comparing `tmp/pkscreener-0.45.20240601.425.tar.gz` & `tmp/pkscreener-0.45.20240602.426-cp310-cp310-macosx_12_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240601.425.tar", last modified: Sat Jun  1 22:57:25 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

