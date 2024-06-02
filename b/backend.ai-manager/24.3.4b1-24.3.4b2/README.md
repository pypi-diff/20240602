# Comparing `tmp/backend.ai-manager-24.3.4b1.tar.gz` & `tmp/backend.ai_manager-24.3.4b2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-manager-24.3.4b1.tar", last modified: Fri May 31 19:10:21 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

