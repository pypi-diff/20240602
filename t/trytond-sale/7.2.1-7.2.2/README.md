# Comparing `tmp/trytond_sale-7.2.1.tar.gz` & `tmp/trytond_sale-7.2.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale-7.2.1.tar", last modified: Wed May  1 11:28:15 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

