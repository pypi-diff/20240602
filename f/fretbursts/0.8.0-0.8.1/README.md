# Comparing `tmp/fretbursts-0.8.0.tar.gz` & `tmp/fretbursts-0.8.1-cp312-cp312-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fretbursts-0.8.0.tar", last modified: Fri May 31 19:46:03 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

