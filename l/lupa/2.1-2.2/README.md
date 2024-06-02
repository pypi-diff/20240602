# Comparing `tmp/lupa-2.1.tar.gz` & `tmp/lupa-2.2-cp310-cp310-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupa-2.1.tar", last modified: Sun Mar 24 18:24:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

