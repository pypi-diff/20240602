# Comparing `tmp/pyiso20022-0.2.0.tar.gz` & `tmp/pyiso20022-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiso20022-0.2.0.tar", last modified: Wed May 29 19:49:22 2024, max compression
+gzip compressed data, was "pyiso20022-0.3.1.tar", last modified: Sun Jun  2 20:01:14 2024, max compression
```

## Comparing `pyiso20022-0.2.0.tar` & `pyiso20022-0.3.1.tar`

### file list

```diff
@@ -1,165 +1,279 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.432451 pyiso20022-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-29 19:48:55.000000 pyiso20022-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-05-29 19:49:22.432451 pyiso20022-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-05-29 19:48:55.000000 pyiso20022-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.408451 pyiso20022-0.2.0/pyiso20022/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 19:49:00.000000 pyiso20022-0.2.0/pyiso20022/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.412451 pyiso20022-0.2.0/pyiso20022/camt/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 19:49:20.000000 pyiso20022-0.2.0/pyiso20022/camt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.412451 pyiso20022-0.2.0/pyiso20022/camt/camt_025_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-29 19:49:20.000000 pyiso20022-0.2.0/pyiso20022/camt/camt_025_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42176 2024-05-29 19:49:20.000000 pyiso20022-0.2.0/pyiso20022/camt/camt_025_001_08/camt_025_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.412451 pyiso20022-0.2.0/pyiso20022/camt/camt_029_001_13/
--rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-05-29 19:49:21.000000 pyiso20022-0.2.0/pyiso20022/camt/camt_029_001_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   141116 2024-05-29 19:49:21.000000 pyiso20022-0.2.0/pyiso20022/camt/camt_029_001_13/camt_029_001_13.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.412451 pyiso20022-0.2.0/pyiso20022/camt/camt_050_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-29 19:49:21.000000 pyiso20022-0.2.0/pyiso20022/camt/camt_050_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25364 2024-05-29 19:49:21.000000 pyiso20022-0.2.0/pyiso20022/camt/camt_050_001_07/camt_050_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.412451 pyiso20022-0.2.0/pyiso20022/camt/camt_054_001_12/
--rw-r--r--   0 runner    (1001) docker     (127)    11021 2024-05-29 19:49:20.000000 pyiso20022-0.2.0/pyiso20022/camt/camt_054_001_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   183576 2024-05-29 19:49:20.000000 pyiso20022-0.2.0/pyiso20022/camt/camt_054_001_12/camt_054_001_12.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.412451 pyiso20022-0.2.0/pyiso20022/camt/camt_056_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-29 19:49:21.000000 pyiso20022-0.2.0/pyiso20022/camt/camt_056_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   103658 2024-05-29 19:49:22.000000 pyiso20022-0.2.0/pyiso20022/camt/camt_056_001_11/camt_056_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.412451 pyiso20022-0.2.0/pyiso20022/head/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 19:49:11.000000 pyiso20022-0.2.0/pyiso20022/head/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.412451 pyiso20022-0.2.0/pyiso20022/head/head_001_001_02/
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-29 19:49:12.000000 pyiso20022-0.2.0/pyiso20022/head/head_001_001_02/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32949 2024-05-29 19:49:12.000000 pyiso20022-0.2.0/pyiso20022/head/head_001_001_02/head_001_001_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.412451 pyiso20022-0.2.0/pyiso20022/head/head_001_001_04/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-29 19:49:11.000000 pyiso20022-0.2.0/pyiso20022/head/head_001_001_04/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-05-29 19:49:11.000000 pyiso20022-0.2.0/pyiso20022/head/head_001_001_04/head_001_001_04.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.412451 pyiso20022-0.2.0/pyiso20022/pacs/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 19:49:00.000000 pyiso20022-0.2.0/pyiso20022/pacs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.416451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-29 19:49:07.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91247 2024-05-29 19:49:07.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_08/pacs_002_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.416451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-29 19:49:08.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    92601 2024-05-29 19:49:08.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_09/pacs_002_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.416451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-05-29 19:49:06.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   105538 2024-05-29 19:49:06.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_11/pacs_002_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.416451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_12/
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-29 19:49:08.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   106664 2024-05-29 19:49:08.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_12/pacs_002_001_12.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.416451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_13/
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-29 19:49:07.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   108350 2024-05-29 19:49:07.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_13/pacs_002_001_13.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.416451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_14/
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-29 19:49:06.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_14/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   106172 2024-05-29 19:49:06.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_14/pacs_002_001_14.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.416451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_003_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-29 19:49:09.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_003_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   101568 2024-05-29 19:49:09.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_003_001_11/pacs_003_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.416451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-29 19:49:09.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    93875 2024-05-29 19:49:10.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_07/pacs_004_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.416451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-29 19:49:09.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   108639 2024-05-29 19:49:09.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_09/pacs_004_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.420451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-29 19:49:10.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   130882 2024-05-29 19:49:10.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_11/pacs_004_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.420451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_13/
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-29 19:49:10.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   127463 2024-05-29 19:49:11.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_13/pacs_004_001_13.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.420451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_007_001_13/
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-05-29 19:49:05.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_007_001_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   108036 2024-05-29 19:49:05.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_007_001_13/pacs_007_001_13.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.420451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_06/
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-29 19:49:00.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_06/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91471 2024-05-29 19:49:00.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_06/pacs_008_001_06.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.420451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-29 19:49:01.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    92665 2024-05-29 19:49:01.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_07/pacs_008_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.420451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-29 19:49:01.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100613 2024-05-29 19:49:01.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_08/pacs_008_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.420451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-29 19:49:02.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   107712 2024-05-29 19:49:03.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_09/pacs_008_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.420451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_10/
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-29 19:49:02.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   107685 2024-05-29 19:49:02.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_10/pacs_008_001_10.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.420451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_12/
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-29 19:49:02.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   104266 2024-05-29 19:49:02.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_12/pacs_008_001_12.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.424451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-29 19:49:03.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    92079 2024-05-29 19:49:03.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_07/pacs_009_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.424451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-29 19:49:04.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100868 2024-05-29 19:49:04.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_08/pacs_009_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.424451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-29 19:49:04.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100166 2024-05-29 19:49:04.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_09/pacs_009_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.424451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-29 19:49:05.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100319 2024-05-29 19:49:05.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_11/pacs_009_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.424451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_010_001_06/
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-29 19:49:00.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_010_001_06/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41010 2024-05-29 19:49:00.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_010_001_06/pacs_010_001_06.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.424451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_028_001_06/
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-05-29 19:49:11.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_028_001_06/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    98096 2024-05-29 19:49:11.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_028_001_06/pacs_028_001_06.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.424451 pyiso20022-0.2.0/pyiso20022/pacs/pacs_029_001_02/
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-29 19:49:03.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_029_001_02/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35965 2024-05-29 19:49:03.000000 pyiso20022-0.2.0/pyiso20022/pacs/pacs_029_001_02/pacs_029_001_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.424451 pyiso20022-0.2.0/pyiso20022/pain/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 19:49:12.000000 pyiso20022-0.2.0/pyiso20022/pain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.424451 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-29 19:49:14.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    90820 2024-05-29 19:49:14.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_07/pain_001_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.424451 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-29 19:49:14.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91335 2024-05-29 19:49:15.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_08/pain_001_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.428451 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-29 19:49:15.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    99320 2024-05-29 19:49:15.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_09/pain_001_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.428451 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-29 19:49:15.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   109547 2024-05-29 19:49:15.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_11/pain_001_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.428451 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-29 19:49:17.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91765 2024-05-29 19:49:17.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_08/pain_002_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.428451 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-29 19:49:16.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    93119 2024-05-29 19:49:16.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_09/pain_002_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.428451 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-29 19:49:16.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   109842 2024-05-29 19:49:16.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_11/pain_002_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.428451 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_12/
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-29 19:49:17.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   109813 2024-05-29 19:49:17.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_12/pain_002_001_12.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.428451 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-29 19:49:13.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    90494 2024-05-29 19:49:13.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_07/pain_007_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.428451 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-29 19:49:13.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91844 2024-05-29 19:49:13.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_08/pain_007_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.428451 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_10/
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-29 19:49:14.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   104507 2024-05-29 19:49:14.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_10/pain_007_001_10.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.432451 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-29 19:49:12.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   104478 2024-05-29 19:49:12.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_11/pain_007_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.432451 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_06/
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-29 19:49:19.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_06/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89884 2024-05-29 19:49:19.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_06/pain_008_001_06.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.432451 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-29 19:49:18.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91285 2024-05-29 19:49:18.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_07/pain_008_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.432451 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-29 19:49:19.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100667 2024-05-29 19:49:19.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_09/pain_008_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.432451 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_10/
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-29 19:49:18.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100638 2024-05-29 19:49:18.000000 pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_10/pain_008_001_10.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:49:22.412451 pyiso20022-0.2.0/pyiso20022.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-05-29 19:49:22.000000 pyiso20022-0.2.0/pyiso20022.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-29 19:49:22.000000 pyiso20022-0.2.0/pyiso20022.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:49:22.000000 pyiso20022-0.2.0/pyiso20022.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 19:49:22.000000 pyiso20022-0.2.0/pyiso20022.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:49:22.432451 pyiso20022-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-29 19:48:55.000000 pyiso20022-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.957332 pyiso20022-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-02 20:00:27.000000 pyiso20022-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-06-02 20:01:14.953333 pyiso20022-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-06-02 20:00:27.000000 pyiso20022-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.917333 pyiso20022-0.3.1/pyiso20022/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 20:00:31.000000 pyiso20022-0.3.1/pyiso20022/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.917333 pyiso20022-0.3.1/pyiso20022/camt/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 20:00:51.000000 pyiso20022-0.3.1/pyiso20022/camt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.917333 pyiso20022-0.3.1/pyiso20022/camt/camt_025_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-06-02 20:00:51.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_025_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42176 2024-06-02 20:00:51.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_025_001_08/camt_025_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.917333 pyiso20022-0.3.1/pyiso20022/camt/camt_029_001_13/
+-rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-06-02 20:01:12.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_029_001_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   141116 2024-06-02 20:01:13.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_029_001_13/camt_029_001_13.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.917333 pyiso20022-0.3.1/pyiso20022/camt/camt_050_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-06-02 20:00:51.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_050_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25364 2024-06-02 20:00:51.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_050_001_07/camt_050_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.917333 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_01/
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-06-02 20:00:57.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_01/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104310 2024-06-02 20:00:57.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_01/camt_052_001_01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.917333 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_02/
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-06-02 20:00:56.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118981 2024-06-02 20:00:56.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_02/camt_052_001_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.917333 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_03/
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-06-02 20:00:54.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_03/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   158576 2024-06-02 20:00:54.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_03/camt_052_001_03.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.921332 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_04/
+-rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-06-02 20:00:52.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_04/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   159128 2024-06-02 20:00:52.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_04/camt_052_001_04.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.921332 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_05/
+-rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-06-02 20:00:54.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_05/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171607 2024-06-02 20:00:54.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_05/camt_052_001_05.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.921332 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-06-02 20:00:53.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   176334 2024-06-02 20:00:53.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_06/camt_052_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.921332 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-06-02 20:00:56.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182722 2024-06-02 20:00:56.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_07/camt_052_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.921332 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-06-02 20:00:53.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190009 2024-06-02 20:00:53.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_08/camt_052_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.921332 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-06-02 20:00:58.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   189941 2024-06-02 20:00:59.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_09/camt_052_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.921332 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-06-02 20:00:58.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193248 2024-06-02 20:00:58.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_10/camt_052_001_10.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.925333 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-06-02 20:00:55.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193607 2024-06-02 20:00:55.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_11/camt_052_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.925333 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_12/
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-06-02 20:00:57.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   188756 2024-06-02 20:00:57.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_052_001_12/camt_052_001_12.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.925333 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_01/
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-06-02 20:01:08.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_01/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104232 2024-06-02 20:01:08.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_01/camt_053_001_01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.925333 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_02/
+-rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-06-02 20:01:11.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119003 2024-06-02 20:01:11.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_02/camt_053_001_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.925333 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_03/
+-rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-06-02 20:01:06.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_03/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   158369 2024-06-02 20:01:06.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_03/camt_053_001_03.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.925333 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_04/
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-06-02 20:01:11.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_04/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   158921 2024-06-02 20:01:11.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_04/camt_053_001_04.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.925333 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_05/
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-06-02 20:01:07.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_05/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   171631 2024-06-02 20:01:07.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_05/camt_053_001_05.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.925333 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-06-02 20:01:10.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   176358 2024-06-02 20:01:10.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_06/camt_053_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.929333 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-06-02 20:01:12.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182746 2024-06-02 20:01:12.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_07/camt_053_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.929333 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-06-02 20:01:07.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190033 2024-06-02 20:01:07.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_08/camt_053_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.929333 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-06-02 20:01:09.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   189967 2024-06-02 20:01:09.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_09/camt_053_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.929333 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11511 2024-06-02 20:01:08.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193274 2024-06-02 20:01:08.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_10/camt_053_001_10.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.929333 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-06-02 20:01:10.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193633 2024-06-02 20:01:10.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_053_001_11/camt_053_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.929333 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_01/
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-06-02 20:01:04.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_01/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99537 2024-06-02 20:01:04.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_01/camt_054_001_01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.929333 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_02/
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-06-02 20:01:02.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114710 2024-06-02 20:01:02.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_02/camt_054_001_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.933333 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_03/
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-06-02 20:01:02.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_03/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154080 2024-06-02 20:01:02.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_03/camt_054_001_03.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.933333 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_04/
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-06-02 20:01:03.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_04/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154632 2024-06-02 20:01:03.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_04/camt_054_001_04.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.933333 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_05/
+-rw-r--r--   0 runner    (1001) docker     (127)    10189 2024-06-02 20:01:05.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_05/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167344 2024-06-02 20:01:06.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_05/camt_054_001_05.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.933333 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-06-02 20:01:03.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   172078 2024-06-02 20:01:03.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_06/camt_054_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.933333 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-06-02 20:01:00.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   177542 2024-06-02 20:01:00.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_07/camt_054_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.933333 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)    10963 2024-06-02 20:00:59.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   184829 2024-06-02 20:00:59.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_08/camt_054_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.933333 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-06-02 20:01:05.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   184761 2024-06-02 20:01:05.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_09/camt_054_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.937332 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-06-02 20:01:00.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   188068 2024-06-02 20:01:00.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_10/camt_054_001_10.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.937332 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-06-02 20:01:04.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   188427 2024-06-02 20:01:04.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_11/camt_054_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.937332 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_12/
+-rw-r--r--   0 runner    (1001) docker     (127)    11021 2024-06-02 20:01:01.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   183576 2024-06-02 20:01:01.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_12/camt_054_001_12.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.937332 pyiso20022-0.3.1/pyiso20022/camt/camt_056_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-06-02 20:00:51.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_056_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103658 2024-06-02 20:00:52.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_056_001_11/camt_056_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.937332 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_03/
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-06-02 20:01:13.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_03/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33886 2024-06-02 20:01:13.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_03/camt_060_001_03.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.937332 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_04/
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-06-02 20:01:14.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_04/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36578 2024-06-02 20:01:14.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_04/camt_060_001_04.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.937332 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_05/
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-06-02 20:01:13.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_05/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44233 2024-06-02 20:01:13.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_05/camt_060_001_05.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.937332 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-06-02 20:01:14.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44189 2024-06-02 20:01:14.000000 pyiso20022-0.3.1/pyiso20022/camt/camt_060_001_06/camt_060_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.937332 pyiso20022-0.3.1/pyiso20022/head/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 20:00:43.000000 pyiso20022-0.3.1/pyiso20022/head/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.937332 pyiso20022-0.3.1/pyiso20022/head/head_001_001_02/
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-06-02 20:00:43.000000 pyiso20022-0.3.1/pyiso20022/head/head_001_001_02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32949 2024-06-02 20:00:43.000000 pyiso20022-0.3.1/pyiso20022/head/head_001_001_02/head_001_001_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/head/head_001_001_04/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-06-02 20:00:43.000000 pyiso20022-0.3.1/pyiso20022/head/head_001_001_04/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-06-02 20:00:43.000000 pyiso20022-0.3.1/pyiso20022/head/head_001_001_04/head_001_001_04.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/pacs/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 20:00:31.000000 pyiso20022-0.3.1/pyiso20022/pacs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-06-02 20:00:38.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91247 2024-06-02 20:00:38.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_08/pacs_002_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-06-02 20:00:39.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92601 2024-06-02 20:00:39.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_09/pacs_002_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-06-02 20:00:37.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105538 2024-06-02 20:00:37.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_11/pacs_002_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_12/
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-06-02 20:00:39.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106664 2024-06-02 20:00:39.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_12/pacs_002_001_12.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_13/
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-06-02 20:00:38.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108350 2024-06-02 20:00:38.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_13/pacs_002_001_13.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_14/
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-06-02 20:00:37.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_14/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106172 2024-06-02 20:00:37.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_14/pacs_002_001_14.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_003_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-06-02 20:00:40.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_003_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101568 2024-06-02 20:00:40.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_003_001_11/pacs_003_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-06-02 20:00:41.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93875 2024-06-02 20:00:41.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_07/pacs_004_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-06-02 20:00:40.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108639 2024-06-02 20:00:40.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_09/pacs_004_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.941333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-06-02 20:00:41.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130882 2024-06-02 20:00:41.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_11/pacs_004_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.945333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_13/
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-06-02 20:00:42.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127463 2024-06-02 20:00:42.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_13/pacs_004_001_13.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.945333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_007_001_13/
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-06-02 20:00:36.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_007_001_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108036 2024-06-02 20:00:37.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_007_001_13/pacs_007_001_13.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.945333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-06-02 20:00:31.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91471 2024-06-02 20:00:31.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_06/pacs_008_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.945333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-06-02 20:00:32.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92665 2024-06-02 20:00:32.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_07/pacs_008_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.945333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-06-02 20:00:32.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100613 2024-06-02 20:00:32.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_08/pacs_008_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.945333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-06-02 20:00:34.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107712 2024-06-02 20:00:34.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_09/pacs_008_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.945333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_10/
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-06-02 20:00:33.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107685 2024-06-02 20:00:33.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_10/pacs_008_001_10.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.945333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_12/
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-06-02 20:00:33.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104266 2024-06-02 20:00:33.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_12/pacs_008_001_12.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.945333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-06-02 20:00:35.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92079 2024-06-02 20:00:35.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_07/pacs_009_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.945333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-06-02 20:00:35.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100868 2024-06-02 20:00:35.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_08/pacs_009_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-06-02 20:00:35.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100166 2024-06-02 20:00:36.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_09/pacs_009_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-06-02 20:00:36.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100319 2024-06-02 20:00:36.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_11/pacs_009_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_010_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-06-02 20:00:31.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_010_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41010 2024-06-02 20:00:31.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_010_001_06/pacs_010_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_028_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-06-02 20:00:42.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_028_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98096 2024-06-02 20:00:42.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_028_001_06/pacs_028_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pacs/pacs_029_001_02/
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-06-02 20:00:34.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_029_001_02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35965 2024-06-02 20:00:34.000000 pyiso20022-0.3.1/pyiso20022/pacs/pacs_029_001_02/pacs_029_001_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pain/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 20:00:43.000000 pyiso20022-0.3.1/pyiso20022/pain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-06-02 20:00:45.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90820 2024-06-02 20:00:45.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_07/pain_001_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-06-02 20:00:46.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91335 2024-06-02 20:00:46.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_08/pain_001_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-06-02 20:00:47.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99320 2024-06-02 20:00:47.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_09/pain_001_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-06-02 20:00:46.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109547 2024-06-02 20:00:46.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_11/pain_001_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-06-02 20:00:48.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91765 2024-06-02 20:00:48.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_08/pain_002_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.949333 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-06-02 20:00:47.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93119 2024-06-02 20:00:47.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_09/pain_002_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.953333 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-06-02 20:00:47.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109842 2024-06-02 20:00:48.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_11/pain_002_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.953333 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_12/
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-06-02 20:00:48.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109813 2024-06-02 20:00:48.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_12/pain_002_001_12.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.953333 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-06-02 20:00:44.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90494 2024-06-02 20:00:44.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_07/pain_007_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.953333 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-06-02 20:00:44.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91844 2024-06-02 20:00:44.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_08/pain_007_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.953333 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_10/
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-06-02 20:00:45.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104507 2024-06-02 20:00:45.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_10/pain_007_001_10.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.953333 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-06-02 20:00:43.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104478 2024-06-02 20:00:43.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_11/pain_007_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.953333 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-06-02 20:00:50.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89884 2024-06-02 20:00:50.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_06/pain_008_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.953333 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-06-02 20:00:49.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91285 2024-06-02 20:00:49.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_07/pain_008_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.953333 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-06-02 20:00:50.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100667 2024-06-02 20:00:50.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_09/pain_008_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.953333 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_10/
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-06-02 20:00:49.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100638 2024-06-02 20:00:49.000000 pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_10/pain_008_001_10.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:14.917333 pyiso20022-0.3.1/pyiso20022.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-06-02 20:01:14.000000 pyiso20022-0.3.1/pyiso20022.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-06-02 20:01:14.000000 pyiso20022-0.3.1/pyiso20022.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 20:01:14.000000 pyiso20022-0.3.1/pyiso20022.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 20:01:14.000000 pyiso20022-0.3.1/pyiso20022.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 20:01:14.957332 pyiso20022-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-06-02 20:00:27.000000 pyiso20022-0.3.1/setup.py
```

### Comparing `pyiso20022-0.2.0/LICENSE` & `pyiso20022-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/PKG-INFO` & `pyiso20022-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiso20022
-Version: 0.2.0
+Version: 0.3.1
 Summary: pyiso20022 is a library for generating ISO20022 messages in Python.
 Home-page: https://github.com/phoughton/pyiso20022
 Author: Peter Houghton
 Author-email: pete@investigatingsoftware.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyiso20022-0.2.0/README.md` & `pyiso20022-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/camt/camt_025_001_08/__init__.py` & `pyiso20022-0.3.1/pyiso20022/camt/camt_025_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/camt/camt_025_001_08/camt_025_001_08.py` & `pyiso20022-0.3.1/pyiso20022/camt/camt_025_001_08/camt_025_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/camt/camt_029_001_13/__init__.py` & `pyiso20022-0.3.1/pyiso20022/camt/camt_029_001_13/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/camt/camt_029_001_13/camt_029_001_13.py` & `pyiso20022-0.3.1/pyiso20022/camt/camt_029_001_13/camt_029_001_13.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/camt/camt_050_001_07/__init__.py` & `pyiso20022-0.3.1/pyiso20022/camt/camt_050_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/camt/camt_050_001_07/camt_050_001_07.py` & `pyiso20022-0.3.1/pyiso20022/camt/camt_050_001_07/camt_050_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/camt/camt_054_001_12/__init__.py` & `pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_12/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/camt/camt_054_001_12/camt_054_001_12.py` & `pyiso20022-0.3.1/pyiso20022/camt/camt_054_001_12/camt_054_001_12.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/camt/camt_056_001_11/__init__.py` & `pyiso20022-0.3.1/pyiso20022/camt/camt_056_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/camt/camt_056_001_11/camt_056_001_11.py` & `pyiso20022-0.3.1/pyiso20022/camt/camt_056_001_11/camt_056_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/head/head_001_001_02/__init__.py` & `pyiso20022-0.3.1/pyiso20022/head/head_001_001_02/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/head/head_001_001_02/head_001_001_02.py` & `pyiso20022-0.3.1/pyiso20022/head/head_001_001_02/head_001_001_02.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/head/head_001_001_04/__init__.py` & `pyiso20022-0.3.1/pyiso20022/head/head_001_001_04/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/head/head_001_001_04/head_001_001_04.py` & `pyiso20022-0.3.1/pyiso20022/head/head_001_001_04/head_001_001_04.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_08/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_08/pacs_002_001_08.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_08/pacs_002_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_09/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_09/pacs_002_001_09.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_09/pacs_002_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_11/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_11/pacs_002_001_11.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_11/pacs_002_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_12/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_12/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_12/pacs_002_001_12.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_12/pacs_002_001_12.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_13/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_13/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_13/pacs_002_001_13.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_13/pacs_002_001_13.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_14/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_14/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_002_001_14/pacs_002_001_14.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_002_001_14/pacs_002_001_14.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_003_001_11/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_003_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_003_001_11/pacs_003_001_11.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_003_001_11/pacs_003_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_07/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_07/pacs_004_001_07.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_07/pacs_004_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_09/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_09/pacs_004_001_09.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_09/pacs_004_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_11/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_11/pacs_004_001_11.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_11/pacs_004_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_13/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_13/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_004_001_13/pacs_004_001_13.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_004_001_13/pacs_004_001_13.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_007_001_13/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_007_001_13/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_007_001_13/pacs_007_001_13.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_007_001_13/pacs_007_001_13.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_06/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_06/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_06/pacs_008_001_06.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_06/pacs_008_001_06.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_07/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_07/pacs_008_001_07.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_07/pacs_008_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_08/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_08/pacs_008_001_08.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_08/pacs_008_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_09/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_09/pacs_008_001_09.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_09/pacs_008_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_10/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_10/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_10/pacs_008_001_10.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_10/pacs_008_001_10.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_12/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_12/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_008_001_12/pacs_008_001_12.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_008_001_12/pacs_008_001_12.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_07/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_07/pacs_009_001_07.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_07/pacs_009_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_08/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_08/pacs_009_001_08.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_08/pacs_009_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_09/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_09/pacs_009_001_09.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_09/pacs_009_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_11/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_009_001_11/pacs_009_001_11.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_009_001_11/pacs_009_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_010_001_06/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_010_001_06/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_010_001_06/pacs_010_001_06.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_010_001_06/pacs_010_001_06.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_028_001_06/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_028_001_06/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_028_001_06/pacs_028_001_06.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_028_001_06/pacs_028_001_06.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_029_001_02/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_029_001_02/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pacs/pacs_029_001_02/pacs_029_001_02.py` & `pyiso20022-0.3.1/pyiso20022/pacs/pacs_029_001_02/pacs_029_001_02.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_07/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_07/pain_001_001_07.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_07/pain_001_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_08/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_08/pain_001_001_08.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_08/pain_001_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_09/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_09/pain_001_001_09.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_09/pain_001_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_11/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_001_001_11/pain_001_001_11.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_001_001_11/pain_001_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_08/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_08/pain_002_001_08.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_08/pain_002_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_09/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_09/pain_002_001_09.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_09/pain_002_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_11/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_11/pain_002_001_11.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_11/pain_002_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_12/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_12/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_002_001_12/pain_002_001_12.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_002_001_12/pain_002_001_12.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_07/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_07/pain_007_001_07.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_07/pain_007_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_08/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_08/pain_007_001_08.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_08/pain_007_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_10/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_10/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_10/pain_007_001_10.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_10/pain_007_001_10.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_11/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_007_001_11/pain_007_001_11.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_007_001_11/pain_007_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_06/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_06/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_06/pain_008_001_06.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_06/pain_008_001_06.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_07/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_07/pain_008_001_07.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_07/pain_008_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_09/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_09/pain_008_001_09.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_09/pain_008_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_10/__init__.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_10/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022/pain/pain_008_001_10/pain_008_001_10.py` & `pyiso20022-0.3.1/pyiso20022/pain/pain_008_001_10/pain_008_001_10.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.2.0/pyiso20022.egg-info/PKG-INFO` & `pyiso20022-0.3.1/pyiso20022.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiso20022
-Version: 0.2.0
+Version: 0.3.1
 Summary: pyiso20022 is a library for generating ISO20022 messages in Python.
 Home-page: https://github.com/phoughton/pyiso20022
 Author: Peter Houghton
 Author-email: pete@investigatingsoftware.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyiso20022-0.2.0/setup.py` & `pyiso20022-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyiso20022",
-    version="0.2.0",
+    version="0.3.1",
     author="Peter Houghton",
     author_email="pete@investigatingsoftware.co.uk",
     description="pyiso20022 is a library for generating ISO20022 messages in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phoughton/pyiso20022",
     packages=setuptools.find_packages(),
```

