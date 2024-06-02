# Comparing `tmp/x12306-0.3.0.tar.gz` & `tmp/x12306-0.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x12306-0.3.0.tar", last modified: Thu Apr 25 13:45:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

