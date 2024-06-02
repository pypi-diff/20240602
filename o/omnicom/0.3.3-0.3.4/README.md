# Comparing `tmp/omnicom-0.3.3-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/omnicom-0.3.4-pp39-pypy39_pp73-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 97318 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   208384 b- defN 24-May-31 20:56 omnicom.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat      188 b- defN 24-May-31 20:56 omnicom-0.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 24-May-31 20:56 omnicom-0.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-31 20:56 omnicom-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      389 b- defN 24-May-31 20:56 omnicom-0.3.3.dist-info/RECORD
-5 files, 209076 bytes uncompressed, 96594 bytes compressed:  53.8%
+Zip file size: 100526 bytes, number of entries: 6
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jun-02 06:56 omnicom-0.3.4.dist-info/
+-rwxr-xr-x  2.0 unx   308512 b- defN 24-Jun-02 06:56 omnicom.pypy39-pp73-darwin.so
+-rw-rw-r--  2.0 unx      390 b- defN 24-Jun-02 06:56 omnicom-0.3.4.dist-info/RECORD
+-rw-r--r--  2.0 unx      115 b- defN 24-Jun-02 06:56 omnicom-0.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Jun-02 06:56 omnicom-0.3.4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      181 b- defN 24-Jun-02 06:56 omnicom-0.3.4.dist-info/METADATA
+6 files, 309206 bytes uncompressed, 99686 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
-Filename: omnicom.pypy39-pp73-win_amd64.pyd
+Filename: omnicom-0.3.4.dist-info/
 Comment: 
 
-Filename: omnicom-0.3.3.dist-info/METADATA
+Filename: omnicom.pypy39-pp73-darwin.so
 Comment: 
 
-Filename: omnicom-0.3.3.dist-info/WHEEL
+Filename: omnicom-0.3.4.dist-info/RECORD
 Comment: 
 
-Filename: omnicom-0.3.3.dist-info/top_level.txt
+Filename: omnicom-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: omnicom-0.3.3.dist-info/RECORD
+Filename: omnicom-0.3.4.dist-info/top_level.txt
+Comment: 
+
+Filename: omnicom-0.3.4.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

