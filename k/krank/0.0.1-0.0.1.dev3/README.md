# Comparing `tmp/krank-0.0.1.tar.gz` & `tmp/krank-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krank-0.0.1.tar", last modified: Sun Dec  4 04:57:27 2022, max compression
+gzip compressed data, was "krank-0.0.1.dev3.tar", last modified: Sun Jun  2 18:46:42 2024, max compression
```

## Comparing `krank-0.0.1.tar` & `krank-0.0.1.dev3.tar`

### file list

```diff
@@ -1,12 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-12-04 04:57:27.784913 krank-0.0.1/
--rw-rw-rw-   0        0        0     1522 2022-12-04 04:41:01.000000 krank-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1057 2022-12-04 04:57:27.786122 krank-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      210 2022-12-04 04:52:23.000000 krank-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-04 04:57:27.766995 krank-0.0.1/krank/
-drwxrwxrwx   0        0        0        0 2022-12-04 04:57:27.783892 krank-0.0.1/krank/krank.egg-info/
--rw-rw-rw-   0        0        0     1057 2022-12-04 04:57:27.000000 krank-0.0.1/krank/krank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2022-12-04 04:57:27.000000 krank-0.0.1/krank/krank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-04 04:57:27.000000 krank-0.0.1/krank/krank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2022-12-04 04:57:27.000000 krank-0.0.1/krank/krank.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2022-12-04 04:46:31.000000 krank-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      922 2022-12-04 04:57:27.786122 krank-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 18:46:42.882530 krank-0.0.1.dev3/
+-rw-rw-rw-   0        0        0      170 2024-06-02 18:34:18.000000 krank-0.0.1.dev3/.gitignore
+-rw-rw-rw-   0        0        0       74 2024-06-02 16:07:56.000000 krank-0.0.1.dev3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4040 2024-06-02 18:46:42.882530 krank-0.0.1.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0     2822 2024-06-02 16:50:42.000000 krank-0.0.1.dev3/README.rst
+drwxrwxrwx   0        0        0        0 2024-06-02 18:46:42.807926 krank-0.0.1.dev3/docs/
+-rw-rw-rw-   0        0        0     1133 2024-06-02 18:34:18.000000 krank-0.0.1.dev3/docs/api.rst
+-rw-rw-rw-   0        0        0     5810 2024-06-02 18:34:18.000000 krank-0.0.1.dev3/docs/conf.py
+-rw-rw-rw-   0        0        0      369 2024-06-02 18:34:18.000000 krank-0.0.1.dev3/docs/index.rst
+-rw-rw-rw-   0        0        0     1680 2024-06-02 18:34:18.000000 krank-0.0.1.dev3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 18:46:42.883530 krank-0.0.1.dev3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 18:46:42.798497 krank-0.0.1.dev3/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 18:46:42.832411 krank-0.0.1.dev3/src/krank/
+-rw-rw-rw-   0        0        0      127 2024-06-02 16:06:15.000000 krank-0.0.1.dev3/src/krank/__init__.py
+-rw-rw-rw-   0        0        0     8560 2024-06-02 17:12:31.000000 krank-0.0.1.dev3/src/krank/_base.py
+-rw-rw-rw-   0        0        0      440 2024-06-02 18:46:42.000000 krank-0.0.1.dev3/src/krank/_version.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:46:42.879132 krank-0.0.1.dev3/src/krank/data/
+-rw-rw-rw-   0        0        0      445 2024-06-01 20:53:44.000000 krank-0.0.1.dev3/src/krank/data/lexicons.json
+-rw-rw-rw-   0        0        0    10092 2024-06-02 00:50:24.000000 krank-0.0.1.dev3/src/krank/data/tables.json
+-rw-rw-rw-   0        0        0     6774 2024-06-02 17:17:21.000000 krank-0.0.1.dev3/src/krank/lexicons.py
+-rw-rw-rw-   0        0        0     7884 2024-06-02 17:16:36.000000 krank-0.0.1.dev3/src/krank/liwc.py
+-rw-rw-rw-   0        0        0    38269 2024-06-02 15:35:07.000000 krank-0.0.1.dev3/src/krank/tables.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:46:42.881132 krank-0.0.1.dev3/src/krank.egg-info/
+-rw-rw-rw-   0        0        0     4040 2024-06-02 18:46:42.000000 krank-0.0.1.dev3/src/krank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-06-02 18:46:42.000000 krank-0.0.1.dev3/src/krank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 18:46:42.000000 krank-0.0.1.dev3/src/krank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-06-02 18:46:42.000000 krank-0.0.1.dev3/src/krank.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-02 18:46:42.000000 krank-0.0.1.dev3/src/krank.egg-info/top_level.txt
```

