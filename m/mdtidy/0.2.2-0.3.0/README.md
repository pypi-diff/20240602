# Comparing `tmp/mdtidy-0.2.2.tar.gz` & `tmp/mdtidy-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdtidy-0.2.2.tar", last modified: Thu May 23 10:11:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

