# Comparing `tmp/lupin_grognard-2.1.0.dev0.tar.gz` & `tmp/lupin_grognard-2.1.0.dev1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin_grognard-2.1.0.dev0.tar", last modified: Wed May 15 08:09:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

