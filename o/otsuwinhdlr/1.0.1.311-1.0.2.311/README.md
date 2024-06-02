# Comparing `tmp/otsuwinhdlr-1.0.1.311.tar.gz` & `tmp/otsuwinhdlr-1.0.2.311-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otsuwinhdlr-1.0.1.311.tar", last modified: Fri Apr 28 12:40:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

