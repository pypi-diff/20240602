# Comparing `tmp/termgraphics-1.0.1.tar.gz` & `tmp/termgraphics-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/termgraphics-1.0.1.tar", last modified: Thu Mar 28 08:15:32 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

