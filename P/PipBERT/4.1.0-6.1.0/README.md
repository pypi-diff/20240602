# Comparing `tmp/PipBERT-4.1.0.tar.gz` & `tmp/pipbert-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PipBERT-4.1.0.tar", last modified: Mon Apr  3 13:51:31 2023, max compression
+gzip compressed data, was "pipbert-6.1.0.tar", last modified: Sat Jun  1 21:50:05 2024, max compression
```

## Comparing `PipBERT-4.1.0.tar` & `pipbert-6.1.0.tar`

### file list

```diff
@@ -1,66 +1,96 @@
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.048024 PipBERT-4.1.0/
--rw-r--r--   0 dbanas     (501) staff       (20)     1310 2022-12-22 13:18:52.000000 PipBERT-4.1.0/LICENSE
--rw-r--r--   0 dbanas     (501) staff       (20)      205 2022-12-22 13:18:52.000000 PipBERT-4.1.0/MANIFEST.in
--rw-r--r--   0 dbanas     (501) staff       (20)     5421 2023-04-03 13:51:31.047904 PipBERT-4.1.0/PKG-INFO
--rw-r--r--   0 dbanas     (501) staff       (20)     4003 2022-12-22 13:18:52.000000 PipBERT-4.1.0/README.md
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.038973 PipBERT-4.1.0/docs/
--rw-r--r--   0 dbanas     (501) staff       (20)      608 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/Makefile
--rw-r--r--   0 dbanas     (501) staff       (20)      814 2023-02-08 21:45:20.000000 PipBERT-4.1.0/docs/make.bat
--rw-r--r--   0 dbanas     (501) staff       (20)   179893 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/screen_shot.png
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.041665 PipBERT-4.1.0/docs/source/
--rw-r--r--   0 dbanas     (501) staff       (20)      209 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/bert.rst
--rw-r--r--   0 dbanas     (501) staff       (20)       78 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/cdr.rst
--rw-r--r--   0 dbanas     (501) staff       (20)     4930 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/conf.py
--rw-r--r--   0 dbanas     (501) staff       (20)       78 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/dfe.rst
--rw-r--r--   0 dbanas     (501) staff       (20)      100 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/help.rst
--rw-r--r--   0 dbanas     (501) staff       (20)     1314 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/index.rst
--rw-r--r--   0 dbanas     (501) staff       (20)      114 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/intro.rst
--rw-r--r--   0 dbanas     (501) staff       (20)     1019 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/modules.rst
--rw-r--r--   0 dbanas     (501) staff       (20)      115 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/plot.rst
--rw-r--r--   0 dbanas     (501) staff       (20)      733 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/pybert.rst
--rw-r--r--   0 dbanas     (501) staff       (20)   179893 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/screen_shot.png
--rw-r--r--   0 dbanas     (501) staff       (20)    75433 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/src_docs_scrn_sht.png
--rw-r--r--   0 dbanas     (501) staff       (20)      127 2022-12-22 13:18:52.000000 PipBERT-4.1.0/docs/source/view.rst
--rw-r--r--   0 dbanas     (501) staff       (20)     2327 2023-03-16 20:50:07.000000 PipBERT-4.1.0/pyproject.toml
--rw-r--r--   0 dbanas     (501) staff       (20)       38 2023-04-03 13:51:31.048052 PipBERT-4.1.0/setup.cfg
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.037316 PipBERT-4.1.0/src/
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.042296 PipBERT-4.1.0/src/PipBERT.egg-info/
--rw-r--r--   0 dbanas     (501) staff       (20)     5421 2023-04-03 13:51:31.000000 PipBERT-4.1.0/src/PipBERT.egg-info/PKG-INFO
--rw-r--r--   0 dbanas     (501) staff       (20)     1249 2023-04-03 13:51:31.000000 PipBERT-4.1.0/src/PipBERT.egg-info/SOURCES.txt
--rw-r--r--   0 dbanas     (501) staff       (20)        1 2023-04-03 13:51:31.000000 PipBERT-4.1.0/src/PipBERT.egg-info/dependency_links.txt
--rw-r--r--   0 dbanas     (501) staff       (20)       42 2023-04-03 13:51:31.000000 PipBERT-4.1.0/src/PipBERT.egg-info/entry_points.txt
--rw-r--r--   0 dbanas     (501) staff       (20)       50 2023-04-03 13:51:31.000000 PipBERT-4.1.0/src/PipBERT.egg-info/requires.txt
--rw-r--r--   0 dbanas     (501) staff       (20)        7 2023-04-03 13:51:31.000000 PipBERT-4.1.0/src/PipBERT.egg-info/top_level.txt
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.044645 PipBERT-4.1.0/src/pybert/
--rw-r--r--   0 dbanas     (501) staff       (20)     1194 2023-03-16 20:50:07.000000 PipBERT-4.1.0/src/pybert/__init__.py
--rw-r--r--   0 dbanas     (501) staff       (20)      396 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/__main__.py
--rw-r--r--   0 dbanas     (501) staff       (20)     1861 2023-02-08 21:45:20.000000 PipBERT-4.1.0/src/pybert/cli.py
--rw-r--r--   0 dbanas     (501) staff       (20)     8426 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/configuration.py
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.045594 PipBERT-4.1.0/src/pybert/gui/
--rw-r--r--   0 dbanas     (501) staff       (20)        0 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/gui/__init__.py
--rw-r--r--   0 dbanas     (501) staff       (20)     2531 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/gui/help.py
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.045787 PipBERT-4.1.0/src/pybert/gui/images/
--rw-r--r--   0 dbanas     (501) staff       (20)   182675 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/gui/images/icon.png
--rw-r--r--   0 dbanas     (501) staff       (20)    26899 2023-03-09 14:32:04.000000 PipBERT-4.1.0/src/pybert/gui/plot.py
--rw-r--r--   0 dbanas     (501) staff       (20)    41040 2023-03-09 14:32:04.000000 PipBERT-4.1.0/src/pybert/gui/view.py
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.046669 PipBERT-4.1.0/src/pybert/models/
--rw-r--r--   0 dbanas     (501) staff       (20)        0 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/models/__init__.py
--rw-r--r--   0 dbanas     (501) staff       (20)    40614 2023-03-09 14:32:04.000000 PipBERT-4.1.0/src/pybert/models/bert.py
--rwxr-xr-x   0 dbanas     (501) staff       (20)     4978 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/models/cdr.py
--rwxr-xr-x   0 dbanas     (501) staff       (20)    12518 2023-03-09 14:32:04.000000 PipBERT-4.1.0/src/pybert/models/dfe.py
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.046887 PipBERT-4.1.0/src/pybert/parsers/
--rw-r--r--   0 dbanas     (501) staff       (20)        0 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/parsers/__init__.py
--rw-r--r--   0 dbanas     (501) staff       (20)     2013 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/parsers/hspice.py
--rwxr-xr-x   0 dbanas     (501) staff       (20)    65901 2023-03-09 14:32:04.000000 PipBERT-4.1.0/src/pybert/pybert.py
--rw-r--r--   0 dbanas     (501) staff       (20)     5778 2023-03-09 14:32:04.000000 PipBERT-4.1.0/src/pybert/results.py
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.047143 PipBERT-4.1.0/src/pybert/solvers/
--rw-r--r--   0 dbanas     (501) staff       (20)      707 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/solvers/__init__.py
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.047258 PipBERT-4.1.0/src/pybert/solvers/simbeor/
--rw-r--r--   0 dbanas     (501) staff       (20)     8718 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/solvers/simbeor/__init__.py
--rw-r--r--   0 dbanas     (501) staff       (20)     2072 2022-12-22 13:18:52.000000 PipBERT-4.1.0/src/pybert/solvers/solver.py
--rw-r--r--   0 dbanas     (501) staff       (20)    45343 2023-03-09 14:32:04.000000 PipBERT-4.1.0/src/pybert/utility.py
-drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2023-04-03 13:51:31.047752 PipBERT-4.1.0/tests/
--rw-r--r--   0 dbanas     (501) staff       (20)      277 2022-12-22 13:18:52.000000 PipBERT-4.1.0/tests/conftest.py
--rw-r--r--   0 dbanas     (501) staff       (20)     2092 2022-12-22 13:18:52.000000 PipBERT-4.1.0/tests/test_basic.py
--rw-r--r--   0 dbanas     (501) staff       (20)     1532 2022-12-22 13:18:52.000000 PipBERT-4.1.0/tests/test_command_line.py
--rw-r--r--   0 dbanas     (501) staff       (20)     5409 2023-03-09 14:32:04.000000 PipBERT-4.1.0/tests/test_loading_and_saving.py
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.780438 pipbert-6.1.0/
+-rw-r--r--   0 dbanas     (501) staff       (20)     1466 2023-12-12 10:48:40.000000 pipbert-6.1.0/LICENSE
+-rw-r--r--   0 dbanas     (501) staff       (20)      334 2024-06-01 20:26:42.000000 pipbert-6.1.0/MANIFEST.in
+-rw-r--r--   0 dbanas     (501) staff       (20)     3596 2024-06-01 21:44:30.000000 pipbert-6.1.0/Makefile
+-rw-r--r--   0 dbanas     (501) staff       (20)     5837 2024-06-01 21:50:05.780270 pipbert-6.1.0/PKG-INFO
+-rw-r--r--   0 dbanas     (501) staff       (20)     4003 2022-12-22 13:18:52.000000 pipbert-6.1.0/README.md
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.772696 pipbert-6.1.0/docs/
+-rw-r--r--   0 dbanas     (501) staff       (20)      608 2022-12-22 13:18:52.000000 pipbert-6.1.0/docs/Makefile
+-rw-r--r--   0 dbanas     (501) staff       (20)      814 2023-02-08 21:45:20.000000 pipbert-6.1.0/docs/make.bat
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.774006 pipbert-6.1.0/docs/source/
+-rw-r--r--   0 dbanas     (501) staff       (20)      209 2022-12-22 13:18:52.000000 pipbert-6.1.0/docs/source/bert.rst
+-rw-r--r--   0 dbanas     (501) staff       (20)       78 2022-12-22 13:18:52.000000 pipbert-6.1.0/docs/source/cdr.rst
+-rw-r--r--   0 dbanas     (501) staff       (20)     5543 2024-05-30 20:18:43.000000 pipbert-6.1.0/docs/source/conf.py
+-rw-r--r--   0 dbanas     (501) staff       (20)       78 2022-12-22 13:18:52.000000 pipbert-6.1.0/docs/source/dfe.rst
+-rw-r--r--   0 dbanas     (501) staff       (20)      100 2022-12-22 13:18:52.000000 pipbert-6.1.0/docs/source/help.rst
+-rw-r--r--   0 dbanas     (501) staff       (20)     1333 2024-05-30 20:20:34.000000 pipbert-6.1.0/docs/source/index.rst
+-rw-r--r--   0 dbanas     (501) staff       (20)      114 2022-12-22 13:18:52.000000 pipbert-6.1.0/docs/source/intro.rst
+-rw-r--r--   0 dbanas     (501) staff       (20)      927 2024-05-30 21:29:06.000000 pipbert-6.1.0/docs/source/modules.rst
+-rw-r--r--   0 dbanas     (501) staff       (20)      115 2022-12-22 13:18:52.000000 pipbert-6.1.0/docs/source/plot.rst
+-rw-r--r--   0 dbanas     (501) staff       (20)      646 2024-05-30 21:17:34.000000 pipbert-6.1.0/docs/source/pybert.rst
+-rw-r--r--   0 dbanas     (501) staff       (20)       37 2024-05-30 21:00:30.000000 pipbert-6.1.0/docs/source/todo.rst
+-rw-r--r--   0 dbanas     (501) staff       (20)      127 2022-12-22 13:18:52.000000 pipbert-6.1.0/docs/source/view.rst
+-rw-r--r--   0 dbanas     (501) staff       (20)     2715 2024-05-31 10:29:13.000000 pipbert-6.1.0/pyproject.toml
+-rw-r--r--   0 dbanas     (501) staff       (20)       38 2024-06-01 21:50:05.780470 pipbert-6.1.0/setup.cfg
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.770870 pipbert-6.1.0/src/
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.780081 pipbert-6.1.0/src/PipBERT.egg-info/
+-rw-r--r--   0 dbanas     (501) staff       (20)     5837 2024-06-01 21:50:05.000000 pipbert-6.1.0/src/PipBERT.egg-info/PKG-INFO
+-rw-r--r--   0 dbanas     (501) staff       (20)     1982 2024-06-01 21:50:05.000000 pipbert-6.1.0/src/PipBERT.egg-info/SOURCES.txt
+-rw-r--r--   0 dbanas     (501) staff       (20)        1 2024-06-01 21:50:05.000000 pipbert-6.1.0/src/PipBERT.egg-info/dependency_links.txt
+-rw-r--r--   0 dbanas     (501) staff       (20)       42 2024-06-01 21:50:05.000000 pipbert-6.1.0/src/PipBERT.egg-info/entry_points.txt
+-rw-r--r--   0 dbanas     (501) staff       (20)       67 2024-06-01 21:50:05.000000 pipbert-6.1.0/src/PipBERT.egg-info/requires.txt
+-rw-r--r--   0 dbanas     (501) staff       (20)        7 2024-06-01 21:50:05.000000 pipbert-6.1.0/src/PipBERT.egg-info/top_level.txt
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.775554 pipbert-6.1.0/src/pybert/
+-rw-r--r--   0 dbanas     (501) staff       (20)     1967 2024-05-31 10:29:03.000000 pipbert-6.1.0/src/pybert/__init__.py
+-rw-r--r--   0 dbanas     (501) staff       (20)      422 2024-05-26 11:23:40.000000 pipbert-6.1.0/src/pybert/__main__.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     1875 2024-05-26 11:23:40.000000 pipbert-6.1.0/src/pybert/cli.py
+-rw-r--r--   0 dbanas     (501) staff       (20)      647 2024-05-26 11:23:40.000000 pipbert-6.1.0/src/pybert/common.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     9579 2024-05-28 23:51:30.000000 pipbert-6.1.0/src/pybert/configuration.py
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.776147 pipbert-6.1.0/src/pybert/gui/
+-rw-r--r--   0 dbanas     (501) staff       (20)        0 2022-12-22 13:18:52.000000 pipbert-6.1.0/src/pybert/gui/__init__.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     7487 2024-05-28 21:26:24.000000 pipbert-6.1.0/src/pybert/gui/handler.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     2575 2024-05-26 11:23:40.000000 pipbert-6.1.0/src/pybert/gui/help.py
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.776286 pipbert-6.1.0/src/pybert/gui/images/
+-rw-r--r--   0 dbanas     (501) staff       (20)   182675 2022-12-22 13:18:52.000000 pipbert-6.1.0/src/pybert/gui/images/icon.png
+-rw-r--r--   0 dbanas     (501) staff       (20)    29912 2024-05-30 10:13:42.000000 pipbert-6.1.0/src/pybert/gui/plot.py
+-rw-r--r--   0 dbanas     (501) staff       (20)    37855 2024-05-30 09:59:46.000000 pipbert-6.1.0/src/pybert/gui/view.py
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.776958 pipbert-6.1.0/src/pybert/models/
+-rw-r--r--   0 dbanas     (501) staff       (20)        0 2022-12-22 13:18:52.000000 pipbert-6.1.0/src/pybert/models/__init__.py
+-rw-r--r--   0 dbanas     (501) staff       (20)    37234 2024-06-01 21:48:46.000000 pipbert-6.1.0/src/pybert/models/bert.py
+-rwxr-xr-x   0 dbanas     (501) staff       (20)     5115 2024-05-26 11:23:40.000000 pipbert-6.1.0/src/pybert/models/cdr.py
+-rwxr-xr-x   0 dbanas     (501) staff       (20)    13201 2024-05-27 18:48:07.000000 pipbert-6.1.0/src/pybert/models/dfe.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     1175 2024-05-28 21:20:18.000000 pipbert-6.1.0/src/pybert/models/tx_tap.py
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.777161 pipbert-6.1.0/src/pybert/parsers/
+-rw-r--r--   0 dbanas     (501) staff       (20)        0 2022-12-22 13:18:52.000000 pipbert-6.1.0/src/pybert/parsers/__init__.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     2137 2024-05-26 11:23:40.000000 pipbert-6.1.0/src/pybert/parsers/hspice.py
+-rw-r--r--   0 dbanas     (501) staff       (20)        0 2022-12-22 13:18:52.000000 pipbert-6.1.0/src/pybert/py.typed
+-rwxr-xr-x   0 dbanas     (501) staff       (20)    54166 2024-06-01 21:48:06.000000 pipbert-6.1.0/src/pybert/pybert.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     5819 2024-05-26 11:23:40.000000 pipbert-6.1.0/src/pybert/results.py
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.777367 pipbert-6.1.0/src/pybert/solvers/
+-rw-r--r--   0 dbanas     (501) staff       (20)      881 2024-05-26 11:23:40.000000 pipbert-6.1.0/src/pybert/solvers/__init__.py
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.777474 pipbert-6.1.0/src/pybert/solvers/simbeor/
+-rw-r--r--   0 dbanas     (501) staff       (20)     8895 2024-05-26 11:23:40.000000 pipbert-6.1.0/src/pybert/solvers/simbeor/__init__.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     2193 2024-05-26 11:23:40.000000 pipbert-6.1.0/src/pybert/solvers/solver.py
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.777862 pipbert-6.1.0/src/pybert/threads/
+-rw-r--r--   0 dbanas     (501) staff       (20)        0 2023-12-10 23:09:02.000000 pipbert-6.1.0/src/pybert/threads/__init__.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     7328 2024-05-28 21:37:06.000000 pipbert-6.1.0/src/pybert/threads/optimization.py
+-rw-r--r--   0 dbanas     (501) staff       (20)      639 2024-05-27 18:51:14.000000 pipbert-6.1.0/src/pybert/threads/sim.py
+-rw-r--r--   0 dbanas     (501) staff       (20)      796 2024-05-26 11:23:40.000000 pipbert-6.1.0/src/pybert/threads/stoppable.py
+-rw-r--r--   0 dbanas     (501) staff       (20)    61088 2024-05-28 21:31:20.000000 pipbert-6.1.0/src/pybert/utility.py
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.778386 pipbert-6.1.0/tests/
+-rw-r--r--   0 dbanas     (501) staff       (20)      277 2022-12-22 13:18:52.000000 pipbert-6.1.0/tests/conftest.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     2129 2024-05-26 11:23:40.000000 pipbert-6.1.0/tests/test_basic.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     1532 2022-12-22 13:18:52.000000 pipbert-6.1.0/tests/test_command_line.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     5427 2024-05-28 22:02:56.000000 pipbert-6.1.0/tests/test_loading_and_saving.py
+-rw-r--r--   0 dbanas     (501) staff       (20)      688 2023-12-20 22:31:49.000000 pipbert-6.1.0/tests/test_sim_thread.py
+-rw-r--r--   0 dbanas     (501) staff       (20)     2808 2024-06-01 20:12:26.000000 pipbert-6.1.0/tox.ini
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.778486 pipbert-6.1.0/type_stubs/
+-rw-r--r--   0 dbanas     (501) staff       (20)      351 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/ReadMe.txt
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.778800 pipbert-6.1.0/type_stubs/pyibisami/
+-rw-r--r--   0 dbanas     (501) staff       (20)       45 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/__init__.pyi
+-rw-r--r--   0 dbanas     (501) staff       (20)        0 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/__main__.pyi
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.779331 pipbert-6.1.0/type_stubs/pyibisami/ami/
+-rw-r--r--   0 dbanas     (501) staff       (20)        0 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/ami/__init__.pyi
+-rw-r--r--   0 dbanas     (501) staff       (20)      431 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/ami/config.pyi
+-rw-r--r--   0 dbanas     (501) staff       (20)     1216 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/ami/model.pyi
+-rw-r--r--   0 dbanas     (501) staff       (20)      432 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/ami/parameter.pyi
+-rw-r--r--   0 dbanas     (501) staff       (20)     1386 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/ami/parser.pyi
+-rw-r--r--   0 dbanas     (501) staff       (20)      303 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/common.pyi
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.779741 pipbert-6.1.0/type_stubs/pyibisami/ibis/
+-rw-r--r--   0 dbanas     (501) staff       (20)        0 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/ibis/__init__.pyi
+-rw-r--r--   0 dbanas     (501) staff       (20)      854 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/ibis/file.pyi
+-rw-r--r--   0 dbanas     (501) staff       (20)      645 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/ibis/model.pyi
+-rw-r--r--   0 dbanas     (501) staff       (20)     1796 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/ibis/parser.pyi
+drwxr-xr-x   0 dbanas     (501) staff       (20)        0 2024-06-01 21:50:05.779935 pipbert-6.1.0/type_stubs/pyibisami/tools/
+-rw-r--r--   0 dbanas     (501) staff       (20)        0 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/tools/__init__.pyi
+-rw-r--r--   0 dbanas     (501) staff       (20)      495 2024-05-26 11:23:40.000000 pipbert-6.1.0/type_stubs/pyibisami/tools/run_tests.pyi
```

### Comparing `PipBERT-4.1.0/LICENSE` & `pipbert-6.1.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-License
-=======
-
-Copyright (c) 2014, David Banas
-All rights reserved World wide.
+Copyright 2014 David Banas
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
-Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
-Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+    2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+    3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `PipBERT-4.1.0/PKG-INFO` & `pipbert-6.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 Metadata-Version: 2.1
 Name: PipBERT
-Version: 4.1.0
+Version: 6.1.0
 Summary: Serial communication link bit error rate tester simulator, written in Python.
 Author: David Patterson
 Author-email: David Banas <capn.freako@gmail.com>
 License: BSD
-Project-URL: documentation, https://github.com/capn-freako/PyBERT/wiki
+Project-URL: Wiki, https://github.com/capn-freako/PyBERT/wiki
+Project-URL: Installation, https://github.com/capn-freako/PyBERT/wiki/instant_gratification
+Project-URL: FAQ, https://github.com/capn-freako/PyBERT/wiki/pybert_faq
+Project-URL: GitHub, https://github.com/capn-freako/PyBERT
+Project-URL: PyPi, https://pypi.org/project/PipBERT/
 Keywords: bert,communication,simulator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Adaptive Technologies
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: System :: Emulators
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: kiwisolver
+Requires-Dist: PyIBIS-AMI>=5.1.4
+Requires-Dist: pyside6<6.7
+Requires-Dist: pyyaml>=6
+Requires-Dist: scikit-rf>=0.29
 
 PyBERT
 ======
 
 PyBERT is a serial communication link bit error rate tester simulator with a graphical user interface (GUI).
 
 It uses the Traits/UI package of the Enthought Python Distribution (EPD) <http://www.enthought.com/products/epd.php>,
```

### Comparing `PipBERT-4.1.0/README.md` & `pipbert-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `PipBERT-4.1.0/docs/Makefile` & `pipbert-6.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PipBERT-4.1.0/docs/make.bat` & `pipbert-6.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PipBERT-4.1.0/docs/source/conf.py` & `pipbert-6.1.0/docs/source/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,34 +12,63 @@
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
-# import os
-# import sys
-# sys.path.insert(0, os.path.abspath('.'))
+import os
+import sys
+# sys.path.insert(0, os.path.abspath('../../PyAMI/src'))
+sys.path.insert(0, os.path.abspath('../../src'))
 
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
-    "sphinx.ext.viewcode",
-    "sphinx.ext.napoleon",
+    "sphinx.ext.coverage",
     "sphinx.ext.githubpages",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.todo",
+    "sphinx.ext.viewcode",
+    "m2r2",
+]
+autodoc_default_options = {
+    "undoc-members": True,
+    "inherited-members": False,
+    "show-inheritance": True,
+    "members": True,
+    "exclude-members": "default_traits_view",
+}
+autodoc_mock_imports = [
+    "chaco",
+    "click",
+    "em",
+    "enable",
+    "matplotlib",
+    "numpy",
+    "parsec",
+    "pyface",
+    "pyibisami",
+    "scipy",
+    "skrf",
+    "traits",
+    "traitsui",
+    "yaml",
 ]
+autoclass_content = "both"
+autodata_content = "both"
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
@@ -54,17 +83,17 @@
 author = "David Banas & David Patterson"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "4.0"
+version = "6.1"
 # The full version, including alpha/beta/rc tags.
-release = "4.0.0"
+release = "6.1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
@@ -74,23 +103,24 @@
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["../build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
+todo_include_todos = True
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "alabaster"
+# html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # This didn't work:
 # html_theme_options = {
```

### Comparing `PipBERT-4.1.0/docs/source/index.rst` & `pipbert-6.1.0/docs/source/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 The documentation for the *PyBERT* project has 2 parts:
 
 * help for stand-alone GUI application *users*, and
 * help for PyBERT *developers* and *importers*
 
 This is the help for developers and importers.
 
-If you're looking for usage instructions, you're in the wrong place.
+If you're looking for help with the GUI application, you're in the wrong place.
 Instead, try:
 
 * Looking at the *Help* tab of the PyBERT GUI.
 * Looking at the `PyBERT FAQ <https://github.com/capn-freako/PyBERT/wiki/pybert_faq>`_.
 * Sending me e-mail at: <capn.freako@gmail.com>.
 
 Note to PyBERT *importers*
@@ -36,14 +36,15 @@
 --------
 
 .. toctree::
    :maxdepth: 2
 
    intro
    modules
+   todo
 
 Indices and tables
 ------------------
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `PipBERT-4.1.0/docs/source/modules.rst` & `pipbert-6.1.0/docs/source/modules.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 =================
 Top Level Modules
 =================
 
-Main Module (`pybert.pybert`)
-*****************************
-
-.. automodule:: pybert.pybert
-
 .. toctree::
    :maxdepth: 1
 
    pybert
 
 Models (`pybert.models`)
 ************************
```

### Comparing `PipBERT-4.1.0/pyproject.toml` & `pipbert-6.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,75 @@
 [build-system]
-requires = ["setuptools>=45"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PipBERT"
 description = "Serial communication link bit error rate tester simulator, written in Python."
-version = "4.1.0"
+version = "6.1.0"
+# dynamic = ["version"]
 authors = [ {name = "David Banas",     email = "capn.freako@gmail.com"}
           , {name = "David Patterson"}
           ]
-urls = { documentation = "https://github.com/capn-freako/PyBERT/wiki"}
+
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9,<3.12"
 license = {text = "BSD"}
 dependencies = [
-        "PyIBIS-AMI>=4.1",
-        "pyside2",
-        "pyyaml>=6",
-        "scikit-rf>=0.24",
+    "kiwisolver",
+    # "PyIBIS-AMI>=6.1.0",
+    "PyIBIS-AMI>=5.1.4",
+    "pyside6<6.7",
+    "pyyaml>=6",
+    "scikit-rf>=0.29",
 ]
 keywords=["bert", "communication", "simulator"]
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Telecommunications Industry",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Adaptive Technologies",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: System :: Emulators",
     "Topic :: System :: Networking",
     "Topic :: Utilities"
 ]
 
+[project.urls]
+Wiki = "https://github.com/capn-freako/PyBERT/wiki"
+Installation = "https://github.com/capn-freako/PyBERT/wiki/instant_gratification"
+FAQ = "https://github.com/capn-freako/PyBERT/wiki/pybert_faq"
+GitHub = "https://github.com/capn-freako/PyBERT"
+PyPi = "https://pypi.org/project/PipBERT/"
+
 [project.scripts]
 pybert = "pybert.cli:cli"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.black]
 line-length = 119
 
 [tool.isort]
-profile = "black"
+# profile = "black"
+known_first_party = ["pybert", "pyibisami"]
+known_third_party = ["enable", "chaco"]
 
 [tool.docformatter]
 wrap-summaries = 0
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-vv --durations=3"
```

### Comparing `PipBERT-4.1.0/src/PipBERT.egg-info/PKG-INFO` & `pipbert-6.1.0/src/PipBERT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 Metadata-Version: 2.1
 Name: PipBERT
-Version: 4.1.0
+Version: 6.1.0
 Summary: Serial communication link bit error rate tester simulator, written in Python.
 Author: David Patterson
 Author-email: David Banas <capn.freako@gmail.com>
 License: BSD
-Project-URL: documentation, https://github.com/capn-freako/PyBERT/wiki
+Project-URL: Wiki, https://github.com/capn-freako/PyBERT/wiki
+Project-URL: Installation, https://github.com/capn-freako/PyBERT/wiki/instant_gratification
+Project-URL: FAQ, https://github.com/capn-freako/PyBERT/wiki/pybert_faq
+Project-URL: GitHub, https://github.com/capn-freako/PyBERT
+Project-URL: PyPi, https://pypi.org/project/PipBERT/
 Keywords: bert,communication,simulator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Adaptive Technologies
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: System :: Emulators
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: kiwisolver
+Requires-Dist: PyIBIS-AMI>=5.1.4
+Requires-Dist: pyside6<6.7
+Requires-Dist: pyyaml>=6
+Requires-Dist: scikit-rf>=0.29
 
 PyBERT
 ======
 
 PyBERT is a serial communication link bit error rate tester simulator with a graphical user interface (GUI).
 
 It uses the Traits/UI package of the Enthought Python Distribution (EPD) <http://www.enthought.com/products/epd.php>,
```

### Comparing `PipBERT-4.1.0/src/pybert/cli.py` & `pipbert-6.1.0/src/pybert/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Main Entry Point for the PyBERT GUI when using the CLI."""
 from pathlib import Path
 
-import click
+import click  # type: ignore
 
 from pybert import __version__
 from pybert.gui.view import traits_view
 from pybert.pybert import PyBERT
 
 
-@click.group(invoke_without_command=True, context_settings=dict(help_option_names=["-h", "--help"]))
+@click.group(invoke_without_command=True, context_settings={"help_option_names": ['-h', '--help']})
 @click.pass_context
 @click.version_option(version=__version__)
 @click.option("--config-file", "-c", type=click.Path(exists=True), help="Load an existing configuration file.")
 @click.option("--results", "-r", type=click.Path(exists=True), help="Load results from a prior run.")
 def cli(ctx, config_file, results):
     """Serial communication link bit error rate tester."""
 
@@ -25,15 +25,15 @@
         if results:
             pybert.load_results(results)
 
         # Show the GUI.
         pybert.configure_traits(view=traits_view)
 
 
-@cli.command(context_settings=dict(help_option_names=["-h", "--help"]))
+@cli.command(context_settings={"help_option_names": ['-h', '--help']})
 @click.argument("config-file", type=click.Path(exists=True))
 @click.option("--results", "-r", type=click.Path(), help="Override the results filename.")
 def sim(config_file, results):
     """Run a simulation without opening the GUI.
 
     Will load the CONFIG_FILE from the given filepath, run the
     simulation and then save the results into a file with the same name
```

### Comparing `PipBERT-4.1.0/src/pybert/configuration.py` & `pipbert-6.1.0/src/pybert/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,71 +40,70 @@
         "Yaml Config (*.yaml;*.yml)|*.yaml;*.yml",
         "All files (*)|*",
     ]
 )
 """This sets the supported file types in the GUI's save-as dialog."""
 
 
-class PyBertCfg:
+class PyBertCfg:  # pylint: disable=too-many-instance-attributes
     """PyBERT simulation configuration data encapsulation class.
 
     This class is used to encapsulate that subset of the configuration
     data for a PyBERT instance, which is to be saved when the user
     clicks the "Save Config." button.
     """
 
-    def __init__(self, the_PyBERT, date_created: str, version: str):
+    def __init__(self, the_PyBERT, date_created: str, version: str):  # pylint: disable=too-many-statements
         """Copy just that subset of the supplied PyBERT instance's __dict__,
         which should be saved."""
 
         # Generic Information
         self.date_created = date_created
         self.version = version
 
         # Simulation Control
         self.bit_rate = the_PyBERT.bit_rate
         self.nbits = the_PyBERT.nbits
         self.pattern = the_PyBERT.pattern
         self.seed = the_PyBERT.seed
-        self.nspb = the_PyBERT.nspb
+        self.nspui = the_PyBERT.nspui
         self.eye_bits = the_PyBERT.eye_bits
         self.mod_type = list(the_PyBERT.mod_type)  # See Issue #95 and PR #98 (jdpatt)
-        self.num_sweeps = the_PyBERT.num_sweeps
-        self.sweep_num = the_PyBERT.sweep_num
-        self.sweep_aves = the_PyBERT.sweep_aves
-        self.do_sweep = the_PyBERT.do_sweep
         self.debug = the_PyBERT.debug
+        self.f_max = the_PyBERT.f_max
+        self.f_step = the_PyBERT.f_step
 
         # Channel Control
         self.use_ch_file = the_PyBERT.use_ch_file
         self.ch_file = the_PyBERT.ch_file
         self.impulse_length = the_PyBERT.impulse_length
-        self.f_step = the_PyBERT.f_step
         self.Rdc = the_PyBERT.Rdc
         self.w0 = the_PyBERT.w0
         self.R0 = the_PyBERT.R0
         self.Theta0 = the_PyBERT.Theta0
         self.Z0 = the_PyBERT.Z0
         self.v0 = the_PyBERT.v0
         self.l_ch = the_PyBERT.l_ch
+        self.renumber = the_PyBERT.renumber
+        self.use_window = the_PyBERT.use_window
 
         # Tx
         self.vod = the_PyBERT.vod
         self.rs = the_PyBERT.rs
         self.cout = the_PyBERT.cout
         self.pn_mag = the_PyBERT.pn_mag
         self.pn_freq = the_PyBERT.pn_freq
         self.rn = the_PyBERT.rn
         tx_taps = []
         for tap in the_PyBERT.tx_taps:
-            tx_taps.append((tap.enabled, tap.value))
+            tx_taps.append((tap.enabled, tap.value, tap.min_val, tap.max_val))
         self.tx_taps = tx_taps
         self.tx_tap_tuners = []
         for tap in the_PyBERT.tx_tap_tuners:
-            self.tx_tap_tuners.append((tap.enabled, tap.value))
+            self.tx_tap_tuners.append((tap.enabled, tap.pos, tap.min_val, tap.max_val, tap.step))
         self.tx_use_ami = the_PyBERT.tx_use_ami
         self.tx_use_ts4 = the_PyBERT.tx_use_ts4
         self.tx_use_getwave = the_PyBERT.tx_use_getwave
         self.tx_ami_file = the_PyBERT.tx_ami_file
         self.tx_dll_file = the_PyBERT.tx_dll_file
         self.tx_ibis_file = the_PyBERT.tx_ibis_file
         self.tx_use_ibis = the_PyBERT.tx_use_ibis
@@ -114,48 +113,54 @@
         self.cin = the_PyBERT.cin
         self.cac = the_PyBERT.cac
         self.use_ctle_file = the_PyBERT.use_ctle_file
         self.ctle_file = the_PyBERT.ctle_file
         self.rx_bw = the_PyBERT.rx_bw
         self.peak_freq = the_PyBERT.peak_freq
         self.peak_mag = the_PyBERT.peak_mag
-        self.ctle_offset = the_PyBERT.ctle_offset
-        self.ctle_mode = the_PyBERT.ctle_mode
-        self.ctle_mode_tune = the_PyBERT.ctle_mode_tune
-        self.ctle_offset_tune = the_PyBERT.ctle_offset_tune
+        self.ctle_enable = the_PyBERT.ctle_enable
         self.rx_use_ami = the_PyBERT.rx_use_ami
         self.rx_use_ts4 = the_PyBERT.rx_use_ts4
         self.rx_use_getwave = the_PyBERT.rx_use_getwave
         self.rx_ami_file = the_PyBERT.rx_ami_file
         self.rx_dll_file = the_PyBERT.rx_dll_file
         self.rx_ibis_file = the_PyBERT.rx_ibis_file
         self.rx_use_ibis = the_PyBERT.rx_use_ibis
 
         # DFE
-        self.use_dfe = the_PyBERT.use_dfe
-        self.use_dfe_tune = the_PyBERT.use_dfe_tune
         self.sum_ideal = the_PyBERT.sum_ideal
         self.decision_scaler = the_PyBERT.decision_scaler
         self.gain = the_PyBERT.gain
         self.n_ave = the_PyBERT.n_ave
-        self.n_taps = the_PyBERT.n_taps
         self.sum_bw = the_PyBERT.sum_bw
 
         # CDR
         self.delta_t = the_PyBERT.delta_t
         self.alpha = the_PyBERT.alpha
         self.n_lock_ave = the_PyBERT.n_lock_ave
         self.rel_lock_tol = the_PyBERT.rel_lock_tol
         self.lock_sustain = the_PyBERT.lock_sustain
 
         # Analysis
         self.thresh = the_PyBERT.thresh
 
+        # Optimization
+        self.rx_bw_tune = the_PyBERT.rx_bw_tune
+        self.peak_freq_tune = the_PyBERT.peak_freq_tune
+        self.peak_mag_tune = the_PyBERT.peak_mag_tune
+        self.min_mag_tune = the_PyBERT.min_mag_tune
+        self.max_mag_tune = the_PyBERT.max_mag_tune
+        self.step_mag_tune = the_PyBERT.step_mag_tune
+        self.ctle_enable_tune = the_PyBERT.ctle_enable_tune
+        self.dfe_tap_tuners = []
+        for tap in the_PyBERT.dfe_tap_tuners:
+            self.dfe_tap_tuners.append((tap.enabled, tap.min_val, tap.max_val))
+
     @staticmethod
-    def load_from_file(filepath: Union[str, Path], pybert):
+    def load_from_file(filepath: Union[str, Path], pybert):  # pylint: disable=too-many-branches
         """Apply all of the configuration settings to the pybert instance.
 
         Confirms that the file actually exists, is the correct extension and
         attempts to set the values back in pybert.
 
         Args:
             filepath: The full filepath including the extension to save too.
@@ -184,21 +189,31 @@
         # Right now the loads deserialize back into a `PyBertCfg` class.
         if not isinstance(user_config, PyBertCfg):
             raise ValueError("The data structure read in is NOT of type: PyBertCfg!")
 
         # Actually load values back into pybert using `setattr`.
         for prop, value in vars(user_config).items():
             if prop == "tx_taps":
-                for count, (enabled, val) in enumerate(value):
+                for count, (enabled, val, min_val, max_val) in enumerate(value):
                     setattr(pybert.tx_taps[count], "enabled", enabled)
                     setattr(pybert.tx_taps[count], "value", val)
+                    setattr(pybert.tx_taps[count], "min_val", min_val)
+                    setattr(pybert.tx_taps[count], "max_val", max_val)
             elif prop == "tx_tap_tuners":
-                for count, (enabled, val) in enumerate(value):
+                for count, (enabled, pos, min_val, max_val, step) in enumerate(value):
                     setattr(pybert.tx_tap_tuners[count], "enabled", enabled)
-                    setattr(pybert.tx_tap_tuners[count], "value", val)
+                    setattr(pybert.tx_tap_tuners[count], "pos", pos)
+                    setattr(pybert.tx_tap_tuners[count], "min_val", min_val)
+                    setattr(pybert.tx_tap_tuners[count], "max_val", max_val)
+                    setattr(pybert.tx_tap_tuners[count], "step", step)
+            elif prop == "dfe_tap_tuners":
+                for count, (enabled, min_val, max_val) in enumerate(value):
+                    setattr(pybert.dfe_tap_tuners[count], "enabled", enabled)
+                    setattr(pybert.dfe_tap_tuners[count], "min_val", min_val)
+                    setattr(pybert.dfe_tap_tuners[count], "max_val", max_val)
             elif prop in ("version", "date_created"):
                 pass  # Just including it for some good housekeeping.  Not currently used.
             else:
                 setattr(pybert, prop, value)
 
     def save(self, filepath: Union[str, Path]):
         """Save out pybert's current configuration to a file.
```

### Comparing `PipBERT-4.1.0/src/pybert/gui/help.py` & `pipbert-6.1.0/src/pybert/gui/help.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,23 @@
       <LI>Hover over any user-settable value in the <em>Config.</em> tab, for help message.</LI>\n
       <LI>Peruse the <em>General Tips</em> & <em>Help by Tab</em> sections, below.</LI>\n
       <LI>Visit the PyBERT FAQ at: https://github.com/capn-freako/PyBERT/wiki/pybert_faq.</LI>\n
       <LI>Send e-mail to David Banas at capn.freako@gmail.com.</LI>\n
     </UL>\n
   <H3>General Tips</H3>\n
     <H4>Main Window Status Bar</H4>\n
-      The status bar, just above the <em>Run</em> button, gives the following information, from left to right:.<p>\n
+      The status bar, at the bottom of the window, gives the following information, from left to right:.<p>\n
       (Note: the individual pieces of information are separated by vertical bar, or 'pipe', characters.)\n
         <UL>\n
           <LI>Current state of, and/or activity engaged in by, the program.</LI>\n
           <LI>Simulator performance, in mega-samples per minute. A 'sample' corresponds to a single value in the signal vector being processed.</LI>\n
           <LI>The observed delay in the channel; can be used as a sanity check, if you know your channel.</LI>\n
           <LI>The number of bit errors detected in the last successful simulation run.</LI>\n
           <LI>The average power dissipated by the transmitter, assuming perfect matching to the channel ,no reflections, and a 50-Ohm system impedance.</LI>\n
-          <LI>The jitter breakdown for the last run. (Taken at DFE output.)</LI>\n
+          <LI>The jitter breakdown for the last run, taken at DFE output. (Parenthesized numbers are Dual-Dirac equivalents.))</LI>\n
         </UL>\n
   <H3>Help by Tab</H3>\n
     <H4>Config.</H4>\n
       This tab allows you to configure the simulation.\n
       Hover over any user configurable element for a help message.\n
 """
 # +           "    <H4>DFE</H4>\n" \
```

### Comparing `PipBERT-4.1.0/src/pybert/gui/images/icon.png` & `pipbert-6.1.0/src/pybert/gui/images/icon.png`

 * *Files identical despite different names*

### Comparing `PipBERT-4.1.0/src/pybert/gui/plot.py` & `pipbert-6.1.0/src/pybert/gui/plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,118 +8,137 @@
 """
 
 from chaco.api import ColorMapper, GridPlotContainer, Plot
 from chaco.tools.api import PanTool, ZoomTool
 
 from pybert.models.bert import update_eyes
 
-PLOT_SPACING = 20
+PLOT_SPACING = 1
+PLOT_PADDING = 75
+PLOT_PADDING_BOT = 50
 
 
+# pylint: disable=too-many-locals,too-many-statements
 def make_plots(self, n_dfe_taps):
     """Create the plots used by the PyBERT GUI."""
 
     post_chnl_str = "Channel"
     post_tx_str = "Channel + Tx Preemphasis"
     post_ctle_str = "Channel + Tx Preemphasis + CTLE (+ AMI DFE)"
     post_dfe_str = "Channel + Tx Preemphasis + CTLE (+ AMI DFE) + PyBERT DFE"
 
     plotdata = self.plotdata
 
     # - DFE tab
-    plot2 = Plot(plotdata, padding_left=75)
+    plot2 = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING_BOT)
     plot2.plot(("t_ns", "ui_ests"), type="line", color="blue")
     plot2.title = "CDR Adaptation"
     plot2.index_axis.title = "Time (ns)"
     plot2.value_axis.title = "UI (ps)"
 
     plot9 = Plot(
         plotdata,
-        auto_colors=["red", "orange", "yellow", "green", "blue", "purple"],
-        padding_left=75,
+        auto_colors=["magenta", "red", "orange", "yellow", "green", "cyan", "blue", "purple", "brown", "black"],
+        padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING_BOT,
     )
+    line_styles = ["line", "dash"]
+    plot9.legend.labels = []
     for i in range(n_dfe_taps):
+        name = f"tap{int(i + 1)}"
         plot9.plot(
-            ("tap_weight_index", f"tap{int(i + 1)}_weights"),
+            ("tap_weight_index", name + "_weights"),
             type="line",
             color="auto",
-            name=f"tap{int(i + 1)}",
+            style=line_styles[i // 10],
+            name=name,
         )
+        plot9.legend.labels.append(name)
     plot9.title = "DFE Adaptation"
+    plot9.index_axis.title = "Sample Number"
     plot9.tools.append(PanTool(plot9, constrain=True, constrain_key=None, constrain_direction="x"))
     zoom9 = ZoomTool(plot9, tool_mode="range", axis="index", always_on=False)
     plot9.overlays.append(zoom9)
     plot9.legend.visible = True
     plot9.legend.align = "ul"
 
-    plot_clk_per_hist = Plot(plotdata, padding_left=75)
+    plot_clk_per_hist = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING_BOT)
     plot_clk_per_hist.plot(("clk_per_hist_bins", "clk_per_hist_vals"), type="line", color="blue")
     plot_clk_per_hist.title = "CDR Clock Period Histogram"
     plot_clk_per_hist.index_axis.title = "Clock Period (ps)"
     plot_clk_per_hist.value_axis.title = "Bin Count"
 
-    plot_clk_per_spec = Plot(plotdata, padding_left=75)
+    plot_clk_per_spec = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING_BOT)
     plot_clk_per_spec.plot(("clk_freqs", "clk_spec"), type="line", color="blue")
     plot_clk_per_spec.title = "CDR Clock Period Spectrum"
     plot_clk_per_spec.index_axis.title = "Frequency (bit rate)"
     plot_clk_per_spec.value_axis.title = "|H(f)| (dB mean)"
     plot_clk_per_spec.value_range.low_setting = -10
     zoom_clk_per_spec = ZoomTool(plot_clk_per_spec, tool_mode="range", axis="index", always_on=False)
     plot_clk_per_spec.overlays.append(zoom_clk_per_spec)
 
     container_dfe = GridPlotContainer(shape=(2, 2), spacing=(PLOT_SPACING, PLOT_SPACING))
     container_dfe.add(plot2)
     container_dfe.add(plot9)
     container_dfe.add(plot_clk_per_hist)
     container_dfe.add(plot_clk_per_spec)
     self.plots_dfe = container_dfe
-    self._dfe_plot = plot9
+    self._dfe_plot = plot9  # pylint: disable=protected-access
 
     # - EQ Tune tab
-    # plot_h_tune = Plot(plotdata, padding_left=75)
-    plot_h_tune = Plot(plotdata, padding_bottom=75)
-    plot_h_tune.plot(("t_ns_chnl", "ctle_out_h_tune"), type="line", color="blue")
-    plot_h_tune.plot(("t_ns_chnl", "clocks_tune"), type="line", color="gray")
+    plot_h_tune = Plot(plotdata, padding_bottom=PLOT_PADDING)
+    plot_h_tune.plot(("t_ns_opt", "clocks_tune"), name="Clocks", type="line", color="gray")
+    plot_h_tune.plot(("t_ns_opt", "ctle_out_h_tune"), name="Equalized Pulse Response", type="line", color="blue")
+    plot_h_tune.plot(("t_ns_opt", "p_chnl"), name="Channel Pulse Response", type="line", color="magenta")
+    plot_h_tune.plot(("curs_ix", "curs_amp"), name="Main Cursor", type="segment", color="red")
     plot_h_tune.title = "Channel + Tx Preemphasis + CTLE (+ AMI DFE) + Ideal DFE"
+    plot_h_tune.legend.labels = ["Channel Pulse Response",
+                                 "Equalized Pulse Response",
+                                 "Clocks",
+                                 "Main Cursor"]
+    plot_h_tune.legend.visible = True
+    plot_h_tune.legend_alignment = "ur"
     plot_h_tune.index_axis.title = "Time (ns)"
     plot_h_tune.y_axis.title = "Pulse Response (V)"
     zoom_tune = ZoomTool(plot_h_tune, tool_mode="range", axis="index", always_on=False)
     plot_h_tune.overlays.append(zoom_tune)
-    self.plot_h_tune = plot_h_tune
+
+    container_tune = GridPlotContainer(shape=(1, 1))
+    container_tune.add(plot_h_tune)
+    self.plot_h_tune = container_tune
 
     # - Impulse Responses tab
-    plot_h_chnl = Plot(plotdata, padding_left=75)
+    plot_h_chnl = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_h_chnl.plot(("t_ns_chnl", "chnl_h"), type="line", color="blue", name="Incremental")
     plot_h_chnl.title = post_chnl_str
     plot_h_chnl.index_axis.title = "Time (ns)"
     plot_h_chnl.y_axis.title = "Impulse Response (V/ns)"
     plot_h_chnl.legend.visible = True
     plot_h_chnl.legend.align = "ur"
     zoom_h = ZoomTool(plot_h_chnl, tool_mode="range", axis="index", always_on=False)
     plot_h_chnl.overlays.append(zoom_h)
 
-    plot_h_tx = Plot(plotdata, padding_left=75)
+    plot_h_tx = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_h_tx.plot(("t_ns_chnl", "tx_out_h"), type="line", color="red", name="Cumulative")
     plot_h_tx.title = post_tx_str
     plot_h_tx.index_axis.title = "Time (ns)"
     plot_h_tx.y_axis.title = "Impulse Response (V/ns)"
     plot_h_tx.legend.visible = True
     plot_h_tx.legend.align = "ur"
     plot_h_tx.index_range = plot_h_chnl.index_range  # Zoom x-axes in tandem.
 
-    plot_h_ctle = Plot(plotdata, padding_left=75)
+    plot_h_ctle = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_h_ctle.plot(("t_ns_chnl", "ctle_out_h"), type="line", color="red", name="Cumulative")
     plot_h_ctle.title = post_ctle_str
     plot_h_ctle.index_axis.title = "Time (ns)"
     plot_h_ctle.y_axis.title = "Impulse Response (V/ns)"
     plot_h_ctle.legend.visible = True
     plot_h_ctle.legend.align = "ur"
     plot_h_ctle.index_range = plot_h_chnl.index_range  # Zoom x-axes in tandem.
 
-    plot_h_dfe = Plot(plotdata, padding_left=75)
+    plot_h_dfe = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_h_dfe.plot(("t_ns_chnl", "dfe_out_h"), type="line", color="red", name="Cumulative")
     plot_h_dfe.title = post_dfe_str
     plot_h_dfe.index_axis.title = "Time (ns)"
     plot_h_dfe.y_axis.title = "Impulse Response (V/ns)"
     plot_h_dfe.legend.visible = True
     plot_h_dfe.legend.align = "ur"
     plot_h_dfe.index_range = plot_h_chnl.index_range  # Zoom x-axes in tandem.
@@ -128,91 +147,94 @@
     container_h.add(plot_h_chnl)
     container_h.add(plot_h_tx)
     container_h.add(plot_h_ctle)
     container_h.add(plot_h_dfe)
     self.plots_h = container_h
 
     # - Step Responses tab
-    plot_s_chnl = Plot(plotdata, padding_left=75)
+    plot_s_chnl = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_s_chnl.plot(("t_ns_chnl", "chnl_s"), type="line", color="blue", name="Incremental")
     plot_s_chnl.title = post_chnl_str
     plot_s_chnl.index_axis.title = "Time (ns)"
     plot_s_chnl.y_axis.title = "Step Response (V)"
     plot_s_chnl.legend.visible = True
     plot_s_chnl.legend.align = "lr"
     zoom_s = ZoomTool(plot_s_chnl, tool_mode="range", axis="index", always_on=False)
     plot_s_chnl.overlays.append(zoom_s)
 
-    plot_s_tx = Plot(plotdata, padding_left=75)
+    plot_s_tx = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_s_tx.plot(("t_ns_chnl", "tx_s"), type="line", color="blue", name="Incremental")
     plot_s_tx.plot(("t_ns_chnl", "tx_out_s"), type="line", color="red", name="Cumulative")
     plot_s_tx.title = post_tx_str
     plot_s_tx.index_axis.title = "Time (ns)"
     plot_s_tx.y_axis.title = "Step Response (V)"
     plot_s_tx.legend.visible = True
     plot_s_tx.legend.align = "lr"
+    plot_s_tx.legend.labels = ["Incremental", "Cumulative"]
     plot_s_tx.index_range = plot_s_chnl.index_range  # Zoom x-axes in tandem.
 
-    plot_s_ctle = Plot(plotdata, padding_left=75)
+    plot_s_ctle = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_s_ctle.plot(("t_ns_chnl", "ctle_s"), type="line", color="blue", name="Incremental")
     plot_s_ctle.plot(("t_ns_chnl", "ctle_out_s"), type="line", color="red", name="Cumulative")
     plot_s_ctle.title = post_ctle_str
     plot_s_ctle.index_axis.title = "Time (ns)"
     plot_s_ctle.y_axis.title = "Step Response (V)"
     plot_s_ctle.legend.visible = True
     plot_s_ctle.legend.align = "lr"
+    plot_s_ctle.legend.labels = ["Incremental", "Cumulative"]
     plot_s_ctle.index_range = plot_s_chnl.index_range  # Zoom x-axes in tandem.
 
-    plot_s_dfe = Plot(plotdata, padding_left=75)
+    plot_s_dfe = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_s_dfe.plot(("t_ns_chnl", "dfe_s"), type="line", color="blue", name="Incremental")
     plot_s_dfe.plot(("t_ns_chnl", "dfe_out_s"), type="line", color="red", name="Cumulative")
     plot_s_dfe.title = post_dfe_str
     plot_s_dfe.index_axis.title = "Time (ns)"
     plot_s_dfe.y_axis.title = "Step Response (V)"
     plot_s_dfe.legend.visible = True
     plot_s_dfe.legend.align = "lr"
+    plot_s_dfe.legend.labels = ["Incremental", "Cumulative"]
     plot_s_dfe.index_range = plot_s_chnl.index_range  # Zoom x-axes in tandem.
 
     container_s = GridPlotContainer(shape=(2, 2), spacing=(PLOT_SPACING, PLOT_SPACING))
     container_s.add(plot_s_chnl)
     container_s.add(plot_s_tx)
     container_s.add(plot_s_ctle)
     container_s.add(plot_s_dfe)
     self.plots_s = container_s
 
     # - Pulse Responses tab
-    plot_p_chnl = Plot(plotdata, padding_left=75)
+    plot_p_chnl = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_p_chnl.plot(("t_ns_chnl", "chnl_p"), type="line", color="blue", name="Incremental")
     plot_p_chnl.title = post_chnl_str
     plot_p_chnl.index_axis.title = "Time (ns)"
     plot_p_chnl.y_axis.title = "Pulse Response (V)"
     plot_p_chnl.legend.visible = True
     plot_p_chnl.legend.align = "ur"
     zoom_p = ZoomTool(plot_p_chnl, tool_mode="range", axis="index", always_on=False)
     plot_p_chnl.overlays.append(zoom_p)
 
-    plot_p_tx = Plot(plotdata, padding_left=75)
+    plot_p_tx = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_p_tx.plot(("t_ns_chnl", "tx_out_p"), type="line", color="red", name="Cumulative")
     plot_p_tx.title = post_tx_str
     plot_p_tx.index_axis.title = "Time (ns)"
     plot_p_tx.y_axis.title = "Pulse Response (V)"
     plot_p_tx.legend.visible = True
     plot_p_tx.legend.align = "ur"
     plot_p_tx.index_range = plot_p_chnl.index_range  # Zoom x-axes in tandem.
 
-    plot_p_ctle = Plot(plotdata, padding_left=75)
+    plot_p_ctle = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_p_ctle.plot(("t_ns_chnl", "ctle_out_p"), type="line", color="red", name="Cumulative")
     plot_p_ctle.title = post_ctle_str
     plot_p_ctle.index_axis.title = "Time (ns)"
     plot_p_ctle.y_axis.title = "Pulse Response (V)"
     plot_p_ctle.legend.visible = True
     plot_p_ctle.legend.align = "ur"
     plot_p_ctle.index_range = plot_p_chnl.index_range  # Zoom x-axes in tandem.
 
-    plot_p_dfe = Plot(plotdata, padding_left=75)
+    plot_p_dfe = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_p_dfe.plot(("t_ns_chnl", "dfe_out_p"), type="line", color="red", name="Cumulative")
     plot_p_dfe.title = post_dfe_str
     plot_p_dfe.index_axis.title = "Time (ns)"
     plot_p_dfe.y_axis.title = "Pulse Response (V)"
     plot_p_dfe.legend.visible = True
     plot_p_dfe.legend.align = "ur"
     plot_p_dfe.index_range = plot_p_chnl.index_range  # Zoom x-axes in tandem.
@@ -221,188 +243,187 @@
     container_p.add(plot_p_chnl)
     container_p.add(plot_p_tx)
     container_p.add(plot_p_ctle)
     container_p.add(plot_p_dfe)
     self.plots_p = container_p
 
     # - Frequency Responses tab
-    plot_H_chnl = Plot(plotdata, padding_left=75)
-    plot_H_chnl.plot(("f_GHz", "chnl_H"), type="line", color="blue", name="Original Impulse", index_scale="log")
+    plot_H_chnl = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
+    plot_H_chnl.plot(("f_GHz", "chnl_H_raw"), type="line", color="black", name="Perfect Term.", index_scale="log")
+    plot_H_chnl.plot(("f_GHz", "chnl_H"), type="line", color="blue", name="Actual Term.", index_scale="log")
     plot_H_chnl.plot(("f_GHz", "chnl_trimmed_H"), type="line", color="red", name="Trimmed Impulse", index_scale="log")
     plot_H_chnl.title = post_chnl_str
     plot_H_chnl.index_axis.title = "Frequency (GHz)"
     plot_H_chnl.y_axis.title = "Frequency Response (dB)"
     plot_H_chnl.index_range.low_setting = 0.01
-    plot_H_chnl.index_range.high_setting = 40.0
+    plot_H_chnl.value_range.low_setting = -40.0
     plot_H_chnl.legend.visible = True
     plot_H_chnl.legend.align = "ll"
 
-    plot_H_tx = Plot(plotdata, padding_left=75)
+    plot_H_tx = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_H_tx.plot(("f_GHz", "tx_H"), type="line", color="blue", name="Incremental", index_scale="log")
     plot_H_tx.plot(("f_GHz", "tx_out_H"), type="line", color="red", name="Cumulative", index_scale="log")
     plot_H_tx.title = post_tx_str
     plot_H_tx.index_axis.title = "Frequency (GHz)"
     plot_H_tx.y_axis.title = "Frequency Response (dB)"
     plot_H_tx.index_range.low_setting = 0.01
-    plot_H_tx.index_range.high_setting = 40.0
+    plot_H_tx.value_range.low_setting = -40.0
     plot_H_tx.legend.visible = True
+    plot_H_tx.legend.labels = ["Incremental", "Cumulative"]
     plot_H_tx.legend.align = "ll"
 
-    plot_H_ctle = Plot(plotdata, padding_left=75)
+    plot_H_ctle = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_H_ctle.plot(("f_GHz", "ctle_H"), type="line", color="blue", name="Incremental", index_scale="log")
     plot_H_ctle.plot(("f_GHz", "ctle_out_H"), type="line", color="red", name="Cumulative", index_scale="log")
     plot_H_ctle.title = post_ctle_str
     plot_H_ctle.index_axis.title = "Frequency (GHz)"
     plot_H_ctle.y_axis.title = "Frequency Response (dB)"
     plot_H_ctle.index_range.low_setting = 0.01
-    plot_H_ctle.index_range.high_setting = 40.0
     plot_H_ctle.value_range.low_setting = -40.0
     plot_H_ctle.legend.visible = True
     plot_H_ctle.legend.align = "ll"
+    plot_H_ctle.legend.labels = ["Incremental", "Cumulative"]
 
-    plot_H_chnl.value_range = plot_H_ctle.value_range
-    plot_H_tx.value_range = plot_H_ctle.value_range
-
-    plot_H_dfe = Plot(plotdata, padding_left=75)
+    plot_H_dfe = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_H_dfe.plot(("f_GHz", "dfe_H"), type="line", color="blue", name="Incremental", index_scale="log")
     plot_H_dfe.plot(("f_GHz", "dfe_out_H"), type="line", color="red", name="Cumulative", index_scale="log")
     plot_H_dfe.title = post_dfe_str
     plot_H_dfe.index_axis.title = "Frequency (GHz)"
     plot_H_dfe.y_axis.title = "Frequency Response (dB)"
     plot_H_dfe.index_range.low_setting = 0.01
-    plot_H_dfe.index_range.high_setting = 40.0
-    plot_H_dfe.value_range = plot_H_ctle.value_range
+    plot_H_dfe.value_range.low_setting = -40.0
     plot_H_dfe.legend.visible = True
     plot_H_dfe.legend.align = "ll"
+    plot_H_dfe.legend.labels = ["Incremental", "Cumulative"]
 
     container_H = GridPlotContainer(shape=(2, 2), spacing=(PLOT_SPACING, PLOT_SPACING))
     container_H.add(plot_H_chnl)
     container_H.add(plot_H_tx)
     container_H.add(plot_H_ctle)
     container_H.add(plot_H_dfe)
     self.plots_H = container_H
 
     # - Outputs tab
-    plot_out_chnl = Plot(plotdata, padding_left=75)
-    # plot_out_chnl.plot(("t_ns", "ideal_signal"), type="line", color="lightgrey")
+    plot_out_chnl = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
+    plot_out_chnl.plot(("t_ns", "ideal_signal"), type="line", color="lightgrey")
     plot_out_chnl.plot(("t_ns", "chnl_out"), type="line", color="blue")
     plot_out_chnl.title = post_chnl_str
     plot_out_chnl.index_axis.title = "Time (ns)"
     plot_out_chnl.y_axis.title = "Output (V)"
     plot_out_chnl.tools.append(PanTool(plot_out_chnl, constrain=True, constrain_key=None, constrain_direction="x"))
     zoom_out_chnl = ZoomTool(plot_out_chnl, tool_mode="range", axis="index", always_on=False)
     plot_out_chnl.overlays.append(zoom_out_chnl)
 
-    plot_out_tx = Plot(plotdata, padding_left=75)
-    plot_out_tx.plot(("t_ns", "tx_out"), type="line", color="blue")
+    plot_out_tx = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
+    plot_out_tx.plot(("t_ns", "rx_in"), type="line", color="blue")
     plot_out_tx.title = post_tx_str
     plot_out_tx.index_axis.title = "Time (ns)"
     plot_out_tx.y_axis.title = "Output (V)"
     plot_out_tx.index_range = plot_out_chnl.index_range  # Zoom x-axes in tandem.
 
-    plot_out_ctle = Plot(plotdata, padding_left=75)
+    plot_out_ctle = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_out_ctle.plot(("t_ns", "ctle_out"), type="line", color="blue")
     plot_out_ctle.title = post_ctle_str
     plot_out_ctle.index_axis.title = "Time (ns)"
     plot_out_ctle.y_axis.title = "Output (V)"
     plot_out_ctle.index_range = plot_out_chnl.index_range  # Zoom x-axes in tandem.
 
-    plot_out_dfe = Plot(plotdata, padding_left=75)
+    plot_out_dfe = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_out_dfe.plot(("t_ns", "dfe_out"), type="line", color="blue")
     plot_out_dfe.title = post_dfe_str
     plot_out_dfe.index_axis.title = "Time (ns)"
     plot_out_dfe.y_axis.title = "Output (V)"
     plot_out_dfe.index_range = plot_out_chnl.index_range  # Zoom x-axes in tandem.
 
     container_out = GridPlotContainer(shape=(2, 2), spacing=(PLOT_SPACING, PLOT_SPACING))
     container_out.add(plot_out_chnl)
     container_out.add(plot_out_tx)
     container_out.add(plot_out_ctle)
     container_out.add(plot_out_dfe)
     self.plots_out = container_out
 
     # - Eye Diagrams tab
-    seg_map = dict(
-        red=[
+    seg_map = {
+        "red": [
             (0.00, 0.00, 0.00),  # black
             (0.00001, 0.00, 0.00),  # blue
             (0.15, 0.00, 0.00),  # cyan
             (0.30, 0.00, 0.00),  # green
             (0.45, 1.00, 1.00),  # yellow
             (0.60, 1.00, 1.00),  # orange
             (0.75, 1.00, 1.00),  # red
             (0.90, 1.00, 1.00),  # pink
             (1.00, 1.00, 1.00),  # white
         ],
-        green=[
+        "green": [
             (0.00, 0.00, 0.00),  # black
             (0.00001, 0.00, 0.00),  # blue
             (0.15, 0.50, 0.50),  # cyan
             (0.30, 0.50, 0.50),  # green
             (0.45, 1.00, 1.00),  # yellow
             (0.60, 0.50, 0.50),  # orange
             (0.75, 0.00, 0.00),  # red
             (0.90, 0.50, 0.50),  # pink
             (1.00, 1.00, 1.00),  # white
         ],
-        blue=[
+        "blue": [
             (0.00, 0.00, 0.00),  # black
             (1e-18, 0.50, 0.50),  # blue
             (0.15, 0.50, 0.50),  # cyan
             (0.30, 0.00, 0.00),  # green
             (0.45, 0.00, 0.00),  # yellow
             (0.60, 0.00, 0.00),  # orange
             (0.75, 0.00, 0.00),  # red
             (0.90, 0.50, 0.50),  # pink
             (1.00, 1.00, 1.00),  # white
-        ],
-    )
+        ]
+    }
     clr_map = ColorMapper.from_segment_map(seg_map)
     self.clr_map = clr_map
 
-    plot_eye_chnl = Plot(plotdata, padding_left=75)
+    plot_eye_chnl = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_eye_chnl.img_plot("eye_chnl", colormap=clr_map)
     plot_eye_chnl.y_direction = "normal"
     plot_eye_chnl.components[0].y_direction = "normal"
     plot_eye_chnl.title = post_chnl_str
     plot_eye_chnl.x_axis.title = "Time (ps)"
     plot_eye_chnl.x_axis.orientation = "bottom"
     plot_eye_chnl.y_axis.title = "Signal Level (V)"
     plot_eye_chnl.x_grid.visible = True
     plot_eye_chnl.y_grid.visible = True
     plot_eye_chnl.x_grid.line_color = "gray"
     plot_eye_chnl.y_grid.line_color = "gray"
 
-    plot_eye_tx = Plot(plotdata, padding_left=75)
+    plot_eye_tx = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_eye_tx.img_plot("eye_tx", colormap=clr_map)
     plot_eye_tx.y_direction = "normal"
     plot_eye_tx.components[0].y_direction = "normal"
     plot_eye_tx.title = post_tx_str
     plot_eye_tx.x_axis.title = "Time (ps)"
     plot_eye_tx.x_axis.orientation = "bottom"
     plot_eye_tx.y_axis.title = "Signal Level (V)"
     plot_eye_tx.x_grid.visible = True
     plot_eye_tx.y_grid.visible = True
     plot_eye_tx.x_grid.line_color = "gray"
     plot_eye_tx.y_grid.line_color = "gray"
 
-    plot_eye_ctle = Plot(plotdata, padding_left=75)
+    plot_eye_ctle = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_eye_ctle.img_plot("eye_ctle", colormap=clr_map)
     plot_eye_ctle.y_direction = "normal"
     plot_eye_ctle.components[0].y_direction = "normal"
     plot_eye_ctle.title = post_ctle_str
     plot_eye_ctle.x_axis.title = "Time (ps)"
     plot_eye_ctle.x_axis.orientation = "bottom"
     plot_eye_ctle.y_axis.title = "Signal Level (V)"
     plot_eye_ctle.x_grid.visible = True
     plot_eye_ctle.y_grid.visible = True
     plot_eye_ctle.x_grid.line_color = "gray"
     plot_eye_ctle.y_grid.line_color = "gray"
 
-    plot_eye_dfe = Plot(plotdata, padding_left=75)
+    plot_eye_dfe = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_eye_dfe.img_plot("eye_dfe", colormap=clr_map)
     plot_eye_dfe.y_direction = "normal"
     plot_eye_dfe.components[0].y_direction = "normal"
     plot_eye_dfe.title = post_dfe_str
     plot_eye_dfe.x_axis.title = "Time (ps)"
     plot_eye_dfe.x_axis.orientation = "bottom"
     plot_eye_dfe.y_axis.title = "Signal Level (V)"
@@ -415,109 +436,103 @@
     container_eye.add(plot_eye_chnl)
     container_eye.add(plot_eye_tx)
     container_eye.add(plot_eye_ctle)
     container_eye.add(plot_eye_dfe)
     self.plots_eye = container_eye
 
     # - Jitter Distributions tab
-    plot_jitter_dist_chnl = Plot(plotdata, padding_left=75)
-    plot_jitter_dist_chnl.plot(("jitter_bins", "jitter_chnl"), type="line", color="blue", name="Measured")
-    plot_jitter_dist_chnl.plot(("jitter_bins", "jitter_ext_chnl"), type="line", color="red", name="Extrapolated")
+    plot_jitter_dist_chnl = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
+    plot_jitter_dist_chnl.plot(("jitter_bins", "jitter_chnl"), type="line", color="blue", name="Total")
+    plot_jitter_dist_chnl.plot(("jitter_bins", "jitter_ext_chnl"), type="line", color="red", name="Data-Ind.")
     plot_jitter_dist_chnl.title = post_chnl_str
     plot_jitter_dist_chnl.index_axis.title = "Time (ps)"
-    plot_jitter_dist_chnl.value_axis.title = "Count"
+    plot_jitter_dist_chnl.value_axis.title = "PDF"
     plot_jitter_dist_chnl.legend.visible = True
     plot_jitter_dist_chnl.legend.align = "ur"
 
-    plot_jitter_dist_tx = Plot(plotdata, padding_left=75)
-    plot_jitter_dist_tx.plot(("jitter_bins", "jitter_tx"), type="line", color="blue", name="Measured")
-    plot_jitter_dist_tx.plot(("jitter_bins", "jitter_ext_tx"), type="line", color="red", name="Extrapolated")
+    plot_jitter_dist_tx = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
+    plot_jitter_dist_tx.plot(("jitter_bins", "jitter_tx"), type="line", color="blue", name="Total")
+    plot_jitter_dist_tx.plot(("jitter_bins", "jitter_ext_tx"), type="line", color="red", name="Data-Ind.")
     plot_jitter_dist_tx.title = post_tx_str
     plot_jitter_dist_tx.index_axis.title = "Time (ps)"
-    plot_jitter_dist_tx.value_axis.title = "Count"
+    plot_jitter_dist_tx.value_axis.title = "PDF"
     plot_jitter_dist_tx.legend.visible = True
     plot_jitter_dist_tx.legend.align = "ur"
 
-    plot_jitter_dist_ctle = Plot(plotdata, padding_left=75)
-    plot_jitter_dist_ctle.plot(("jitter_bins", "jitter_ctle"), type="line", color="blue", name="Measured")
-    plot_jitter_dist_ctle.plot(("jitter_bins", "jitter_ext_ctle"), type="line", color="red", name="Extrapolated")
+    plot_jitter_dist_ctle = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
+    plot_jitter_dist_ctle.plot(("jitter_bins", "jitter_ctle"), type="line", color="blue", name="Total")
+    plot_jitter_dist_ctle.plot(("jitter_bins", "jitter_ext_ctle"), type="line", color="red", name="Data-Ind.")
     plot_jitter_dist_ctle.title = post_ctle_str
     plot_jitter_dist_ctle.index_axis.title = "Time (ps)"
-    plot_jitter_dist_ctle.value_axis.title = "Count"
+    plot_jitter_dist_ctle.value_axis.title = "PDF"
     plot_jitter_dist_ctle.legend.visible = True
     plot_jitter_dist_ctle.legend.align = "ur"
 
-    plot_jitter_dist_dfe = Plot(plotdata, padding_left=75)
-    plot_jitter_dist_dfe.plot(("jitter_bins", "jitter_dfe"), type="line", color="blue", name="Measured")
-    plot_jitter_dist_dfe.plot(("jitter_bins", "jitter_ext_dfe"), type="line", color="red", name="Extrapolated")
+    plot_jitter_dist_dfe = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
+    plot_jitter_dist_dfe.plot(("jitter_bins", "jitter_dfe"), type="line", color="blue", name="Total")
+    plot_jitter_dist_dfe.plot(("jitter_bins", "jitter_ext_dfe"), type="line", color="red", name="Data-Ind.")
     plot_jitter_dist_dfe.title = post_dfe_str
     plot_jitter_dist_dfe.index_axis.title = "Time (ps)"
-    plot_jitter_dist_dfe.value_axis.title = "Count"
+    plot_jitter_dist_dfe.value_axis.title = "PDF"
     plot_jitter_dist_dfe.legend.visible = True
     plot_jitter_dist_dfe.legend.align = "ur"
 
     container_jitter_dist = GridPlotContainer(shape=(2, 2), spacing=(PLOT_SPACING, PLOT_SPACING))
     container_jitter_dist.add(plot_jitter_dist_chnl)
     container_jitter_dist.add(plot_jitter_dist_tx)
     container_jitter_dist.add(plot_jitter_dist_ctle)
     container_jitter_dist.add(plot_jitter_dist_dfe)
     self.plots_jitter_dist = container_jitter_dist
 
     # - Jitter Spectrums tab
-    plot_jitter_spec_chnl = Plot(plotdata)
-    plot_jitter_spec_chnl.plot(("f_MHz", "jitter_spectrum_chnl"), type="line", color="blue", name="Total")
-    plot_jitter_spec_chnl.plot(
-        ("f_MHz", "jitter_ind_spectrum_chnl"), type="line", color="red", name="Data Independent"
-    )
-    plot_jitter_spec_chnl.plot(("f_MHz", "thresh_chnl"), type="line", color="magenta", name="Pj Threshold")
+    plot_jitter_spec_chnl = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
+    plot_jitter_spec_chnl.plot(("f_MHz", "jitter_spectrum_chnl"),     type="line", color="blue",    name="Total")
+    plot_jitter_spec_chnl.plot(("f_MHz", "jitter_ind_spectrum_chnl"), type="line", color="red",     name="Data Independent")
+    plot_jitter_spec_chnl.plot(("f_MHz", "thresh_chnl"),              type="line", color="magenta", name="Pj Threshold")
     plot_jitter_spec_chnl.title = post_chnl_str
     plot_jitter_spec_chnl.index_axis.title = "Frequency (MHz)"
     plot_jitter_spec_chnl.value_axis.title = "|FFT(TIE)| (dBui)"
     plot_jitter_spec_chnl.tools.append(
         PanTool(plot_jitter_spec_chnl, constrain=True, constrain_key=None, constrain_direction="x")
     )
     zoom_jitter_spec_chnl = ZoomTool(plot_jitter_spec_chnl, tool_mode="range", axis="index", always_on=False)
     plot_jitter_spec_chnl.overlays.append(zoom_jitter_spec_chnl)
     plot_jitter_spec_chnl.legend.visible = True
     plot_jitter_spec_chnl.legend.align = "lr"
 
-    plot_jitter_spec_tx = Plot(plotdata)
-    plot_jitter_spec_tx.plot(("f_MHz", "jitter_spectrum_tx"), type="line", color="blue", name="Total")
-    plot_jitter_spec_tx.plot(("f_MHz", "jitter_ind_spectrum_tx"), type="line", color="red", name="Data Independent")
-    plot_jitter_spec_tx.plot(("f_MHz", "thresh_tx"), type="line", color="magenta", name="Pj Threshold")
+    plot_jitter_spec_tx = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
+    plot_jitter_spec_tx.plot(("f_MHz", "jitter_spectrum_tx"),     type="line", color="blue",    name="Total")
+    plot_jitter_spec_tx.plot(("f_MHz", "jitter_ind_spectrum_tx"), type="line", color="red",     name="Data Independent")
+    plot_jitter_spec_tx.plot(("f_MHz", "thresh_tx"),              type="line", color="magenta", name="Pj Threshold")
     plot_jitter_spec_tx.title = post_tx_str
     plot_jitter_spec_tx.index_axis.title = "Frequency (MHz)"
     plot_jitter_spec_tx.value_axis.title = "|FFT(TIE)| (dBui)"
     plot_jitter_spec_tx.value_range.low_setting = -40.0
     plot_jitter_spec_tx.index_range = plot_jitter_spec_chnl.index_range  # Zoom x-axes in tandem.
     plot_jitter_spec_tx.legend.visible = True
     plot_jitter_spec_tx.legend.align = "lr"
 
     plot_jitter_spec_chnl.value_range = plot_jitter_spec_tx.value_range
 
-    plot_jitter_spec_ctle = Plot(plotdata)
-    plot_jitter_spec_ctle.plot(("f_MHz", "jitter_spectrum_ctle"), type="line", color="blue", name="Total")
-    plot_jitter_spec_ctle.plot(
-        ("f_MHz", "jitter_ind_spectrum_ctle"), type="line", color="red", name="Data Independent"
-    )
-    plot_jitter_spec_ctle.plot(("f_MHz", "thresh_ctle"), type="line", color="magenta", name="Pj Threshold")
+    plot_jitter_spec_ctle = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
+    plot_jitter_spec_ctle.plot(("f_MHz", "jitter_spectrum_ctle"),     type="line", color="blue",    name="Total")
+    plot_jitter_spec_ctle.plot(("f_MHz", "jitter_ind_spectrum_ctle"), type="line", color="red",     name="Data Independent")
+    plot_jitter_spec_ctle.plot(("f_MHz", "thresh_ctle"),              type="line", color="magenta", name="Pj Threshold")
     plot_jitter_spec_ctle.title = post_ctle_str
     plot_jitter_spec_ctle.index_axis.title = "Frequency (MHz)"
     plot_jitter_spec_ctle.value_axis.title = "|FFT(TIE)| (dBui)"
     plot_jitter_spec_ctle.index_range = plot_jitter_spec_chnl.index_range  # Zoom x-axes in tandem.
     plot_jitter_spec_ctle.legend.visible = True
     plot_jitter_spec_ctle.legend.align = "lr"
     plot_jitter_spec_ctle.value_range = plot_jitter_spec_tx.value_range
 
-    plot_jitter_spec_dfe = Plot(plotdata)
-    plot_jitter_spec_dfe.plot(("f_MHz_dfe", "jitter_spectrum_dfe"), type="line", color="blue", name="Total")
-    plot_jitter_spec_dfe.plot(
-        ("f_MHz_dfe", "jitter_ind_spectrum_dfe"), type="line", color="red", name="Data Independent"
-    )
-    plot_jitter_spec_dfe.plot(("f_MHz_dfe", "thresh_dfe"), type="line", color="magenta", name="Pj Threshold")
+    plot_jitter_spec_dfe = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
+    plot_jitter_spec_dfe.plot(("f_MHz_dfe", "jitter_spectrum_dfe"),     type="line", color="blue",    name="Total")
+    plot_jitter_spec_dfe.plot(("f_MHz_dfe", "jitter_ind_spectrum_dfe"), type="line", color="red",     name="Data Independent")
+    plot_jitter_spec_dfe.plot(("f_MHz_dfe", "thresh_dfe"),              type="line", color="magenta", name="Pj Threshold")
     plot_jitter_spec_dfe.title = post_dfe_str
     plot_jitter_spec_dfe.index_axis.title = "Frequency (MHz)"
     plot_jitter_spec_dfe.value_axis.title = "|FFT(TIE)| (dBui)"
     plot_jitter_spec_dfe.index_range = plot_jitter_spec_chnl.index_range  # Zoom x-axes in tandem.
     plot_jitter_spec_dfe.legend.visible = True
     plot_jitter_spec_dfe.legend.align = "lr"
     plot_jitter_spec_dfe.value_range = plot_jitter_spec_tx.value_range
@@ -526,42 +541,43 @@
     container_jitter_spec.add(plot_jitter_spec_chnl)
     container_jitter_spec.add(plot_jitter_spec_tx)
     container_jitter_spec.add(plot_jitter_spec_ctle)
     container_jitter_spec.add(plot_jitter_spec_dfe)
     self.plots_jitter_spec = container_jitter_spec
 
     # - Bathtub Curves tab
-    plot_bathtub_chnl = Plot(plotdata)
+    # ToDo: Make extrapolated portion of curve dashed.
+    plot_bathtub_chnl = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_bathtub_chnl.plot(("jitter_bins", "bathtub_chnl"), type="line", color="blue")
     plot_bathtub_chnl.value_range.high_setting = 0
     plot_bathtub_chnl.value_range.low_setting = -18
     plot_bathtub_chnl.value_axis.tick_interval = 3
     plot_bathtub_chnl.title = post_chnl_str
     plot_bathtub_chnl.index_axis.title = "Time (ps)"
     plot_bathtub_chnl.value_axis.title = "Log10(P(Transition occurs inside.))"
 
-    plot_bathtub_tx = Plot(plotdata)
+    plot_bathtub_tx = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_bathtub_tx.plot(("jitter_bins", "bathtub_tx"), type="line", color="blue")
     plot_bathtub_tx.value_range.high_setting = 0
     plot_bathtub_tx.value_range.low_setting = -18
     plot_bathtub_tx.value_axis.tick_interval = 3
     plot_bathtub_tx.title = post_tx_str
     plot_bathtub_tx.index_axis.title = "Time (ps)"
     plot_bathtub_tx.value_axis.title = "Log10(P(Transition occurs inside.))"
 
-    plot_bathtub_ctle = Plot(plotdata)
+    plot_bathtub_ctle = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_bathtub_ctle.plot(("jitter_bins", "bathtub_ctle"), type="line", color="blue")
     plot_bathtub_ctle.value_range.high_setting = 0
     plot_bathtub_ctle.value_range.low_setting = -18
     plot_bathtub_ctle.value_axis.tick_interval = 3
     plot_bathtub_ctle.title = post_ctle_str
     plot_bathtub_ctle.index_axis.title = "Time (ps)"
     plot_bathtub_ctle.value_axis.title = "Log10(P(Transition occurs inside.))"
 
-    plot_bathtub_dfe = Plot(plotdata)
+    plot_bathtub_dfe = Plot(plotdata, padding_left=PLOT_PADDING, padding_bottom=PLOT_PADDING)
     plot_bathtub_dfe.plot(("jitter_bins", "bathtub_dfe"), type="line", color="blue")
     plot_bathtub_dfe.value_range.high_setting = 0
     plot_bathtub_dfe.value_range.low_setting = -18
     plot_bathtub_dfe.value_axis.tick_interval = 3
     plot_bathtub_dfe.title = post_dfe_str
     plot_bathtub_dfe.index_axis.title = "Time (ps)"
     plot_bathtub_dfe.value_axis.title = "Log10(P(Transition occurs inside.))"
```

### Comparing `PipBERT-4.1.0/src/pybert/gui/view.py` & `pipbert-6.1.0/src/pybert/gui/view.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,902 +2,817 @@
 
 Original author: David Banas <capn.freako@gmail.com>
 
 Original date:   August 24, 2014 (Copied from pybert.py, as part of a major code cleanup.)
 
 Copyright (c) 2014 David Banas; all rights reserved World wide.
 """
-import sys
-import webbrowser
-from pathlib import Path
-from threading import Thread
 
 from enable.component_editor import ComponentEditor
-from pyface.api import OK, FileDialog, MessageDialog
 from pyface.image_resource import ImageResource
-from traits.api import Instance
 from traitsui.api import (  # CloseAction,
     Action,
     CheckListEditor,
     FileEditor,
     Group,
-    Handler,
     HGroup,
     Item,
     Menu,
     MenuBar,
     NoButtons,
     ObjectColumn,
     Separator,
     TableEditor,
     TextEditor,
     VGroup,
     View,
     spring,
 )
 
-from pybert import __authors__, __copy__, __date__, __version__
-from pybert.configuration import CONFIG_LOAD_WILDCARD, CONFIG_SAVE_WILDCARD
-from pybert.models.bert import my_run_sweeps
-from pybert.results import RESULTS_FILEDIALOG_WILDCARD
-
-
-class RunSimThread(Thread):
-    """Used to run the simulation in its own thread, in order to preserve GUI
-    responsiveness."""
-
-    def run(self):
-        """Run the simulation(s)."""
-        my_run_sweeps(self.the_pybert)
-
-
-class MyHandler(Handler):
-    """This handler is instantiated by the View and handles user button
-    clicks."""
-
-    run_sim_thread = Instance(RunSimThread)
-
-    def do_run_simulation(self, info):
-        """Spawn a simulation thread and run with the current settings."""
-        the_pybert = info.object
-        if self.run_sim_thread and self.run_sim_thread.is_alive():
-            pass
-        else:
-            self.run_sim_thread = RunSimThread()
-            self.run_sim_thread.the_pybert = the_pybert
-            self.run_sim_thread.start()
-
-    def do_stop_simulation(self):
-        """Kill the simulation thread."""
-        if self.run_sim_thread and self.run_sim_thread.is_alive():
-            self.run_sim_thread.stop()
-
-    def do_save_cfg(self, info):
-        """Save the configuration.
-
-        If no config file is set, use the `self.do_save_cfg_as()` method to prompt the user.
-
-        Args:
-            info: When an action is clicked, it passes the whole trait instance to this function.
-        """
-        # pylint: disable=no-self-use
-        pybert = info.object
-        configuration_file = Path(pybert.cfg_file)
-        if pybert.cfg_file and configuration_file.exists():
-            pybert.save_configuration(configuration_file)
-        else:  # A configuration file hasn't been set yet so use the save-as method
-            self.do_save_cfg_as(info)
-
-    def do_save_cfg_as(self, info):
-        """Prompt the user to choose where to save the config and save it.
-
-        Args:
-            info: When an action is clicked, it passes the whole trait instance to this function.
-        """
-        # pylint: disable=no-self-use
-        pybert = info.object
-        dialog = FileDialog(
-            action="save as",
-            wildcard=CONFIG_SAVE_WILDCARD,
-            default_path=pybert.cfg_file,
-        )
-        if dialog.open() == OK:
-            pybert.save_configuration(Path(dialog.path))
-
-    def do_load_cfg(self, info):
-        """Prompt the user to choose where to load the config from and load it.
-
-        Args:
-            info: When an action is clicked, it passes the whole trait instance to this function.
-        """
-        # pylint: disable=no-self-use
-        pybert = info.object
-        dialog = FileDialog(
-            action="open",
-            wildcard=CONFIG_LOAD_WILDCARD,
-            default_path=pybert.cfg_file,
-        )
-        if dialog.open() == OK:
-            pybert.load_configuration(Path(dialog.path))
-
-    def do_save_data(self, info):
-        """Prompt the user to choose where to save the results and save it.
-
-        Args:
-            info: When an action is clicked, it passes the whole trait instance to this function.
-        """
-        # pylint: disable=no-self-use
-        pybert = info.object
-        dialog = FileDialog(action="save as", wildcard=RESULTS_FILEDIALOG_WILDCARD, default_path=pybert.data_file)
-        if dialog.open() == OK:
-            pybert.save_results(Path(dialog.path))
-
-    def do_load_data(self, info):
-        """Prompt the user to choose where to load the results from and load it.
-
-        Pybert will load these as "reference" plots for the responses.
-
-        Args:
-            info: When an action is clicked, it passes the whole trait instance to this function.
-        """
-        # pylint: disable=no-self-use
-        pybert = info.object
-        dialog = FileDialog(action="open", wildcard=RESULTS_FILEDIALOG_WILDCARD, default_path=pybert.data_file)
-        if dialog.open() == OK:
-            pybert.load_results(Path(dialog.path))
-
-    def do_clear_data(self, info):
-        """If any reference or prior results has been loaded, clear it.
-
-        Args:
-            info: When an action is clicked, it passes the whole trait instance to this function.
-        """
-        # pylint: disable=no-self-use
-        pybert = info.object
-        pybert.clear_reference_from_plots()
-
-    def toggle_debug_clicked(self, info):
-        """Toggle whether debug mode is enabled or not."""
-        # pylint: disable=no-self-use
-        info.object.debug = not info.object.debug
-
-    def getting_started_clicked(self, info):
-        """Open up Pybert's wiki."""
-        # pylint: disable=no-self-use,unused-argument
-        webbrowser.open("https://github.com/capn-freako/PyBERT/wiki")
-
-    def show_about_clicked(self, info):
-        """Open a dialog and show the user the about info."""
-        # pylint: disable=no-self-use,unused-argument
-        dialog = MessageDialog(
-            title="About Pybert",
-            message=f"PyBERT v{__version__} - a serial communication link design tool, written in Python.",
-            informative=(
-                f"{__authors__}<BR>\n" f"{__date__}<BR><BR>\n\n" f"{__copy__};<BR>\n" "All rights reserved World wide."
-            ),
-            severity="information",
-        )
-        dialog.open()
-
-    def close_app(self, info):
-        """Close the app.
-
-        Can't use CloseAction until https://github.com/enthought/traitsui/issues/1442 is resolved.
-        """
-        # pylint: disable=no-self-use,unused-argument
-        sys.exit(0)
+from pybert.gui.handler import MyHandler
 
+HIGH_RES = True
 
 # Main window layout definition.
 traits_view = View(
     Group(
         VGroup(
             HGroup(
-                VGroup(
-                    HGroup(  # Simulation Control
+                VGroup(  # Simulation Control
+                    HGroup(
                         VGroup(
-                            Item(
-                                name="bit_rate",
-                                label="Bit Rate (Gbps)",
-                                tooltip="bit rate",
-                                show_label=True,
-                                enabled_when="True",
-                                editor=TextEditor(auto_set=False, enter_set=True, evaluate=float),
-                            ),
-                            Item(
-                                name="nbits",
-                                label="Nbits",
-                                tooltip="# of bits to run",
-                                editor=TextEditor(auto_set=False, enter_set=True, evaluate=int),
+                            HGroup(
+                                Item(
+                                    name="bit_rate",
+                                    label="Bit Rate",
+                                    tooltip="bit rate",
+                                    show_label=True,
+                                    enabled_when="True",
+                                    editor=TextEditor(auto_set=False, enter_set=True, evaluate=float),
+                                ),
+                                Item(label="Gbps"),
                             ),
                             Item(
-                                name="nspb",
-                                label="Nspb",
-                                tooltip="# of samples per bit",
+                                name="nspui",
+                                label="Samps. per UI",
+                                tooltip="# of samples per unit interval",
                                 editor=TextEditor(auto_set=False, enter_set=True, evaluate=int),
                             ),
                             Item(
                                 name="mod_type",
                                 label="Modulation",
                                 tooltip="line signalling/modulation scheme",
                                 editor=CheckListEditor(values=[(0, "NRZ"), (1, "Duo-binary"), (2, "PAM-4")]),
                             ),
+                            label="Rate && Modulation",
+                            show_border=True,
                         ),
                         VGroup(
-                            Item(name="do_sweep", label="Do Sweep", tooltip="Run parameter sweeps."),
-                            Item(
-                                name="sweep_aves",
-                                label="SweepAves",
-                                tooltip="# of trials, per sweep, for averaging.",
-                                enabled_when="do_sweep == True",
-                            ),
                             HGroup(
                                 Item(
                                     name="pattern",
                                     label="Pattern",
                                     tooltip="pattern to use to construct bit stream",
-                                    # editor=TextEditor(auto_set=False, enter_set=True, evaluate=int),
                                 ),
+                                spring,
                                 Item(
                                     name="seed",
                                     label="Seed",
                                     tooltip="LFSR seed. 0 means new random seed for each run.",
                                 ),
                             ),
                             Item(
+                                name="nbits",
+                                label="Nbits",
+                                tooltip="# of bits to run",
+                                editor=TextEditor(auto_set=False, enter_set=True, evaluate=int),
+                            ),
+                            Item(
                                 name="eye_bits",
                                 label="EyeBits",
                                 tooltip="# of bits to use to form eye diagrams",
                                 editor=TextEditor(auto_set=False, enter_set=True, evaluate=int),
                             ),
+                            label="Test Pattern",
+                            show_border=True,
                         ),
                         VGroup(
-                            Item(name="vod", label="Vod (V)", tooltip="Tx output voltage into matched load"),
-                            Item(name="rn", label="Rn (V)", tooltip="standard deviation of random noise"),
-                            Item(name="pn_mag", label="Pn (V)", tooltip="peak magnitude of periodic noise"),
-                            Item(name="pn_freq", label="f(Pn) (MHz)", tooltip="frequency of periodic noise"),
+                            HGroup(
+                                Item(name="vod", label="Vod", tooltip="Tx output voltage into matched load"),
+                                Item(label="V"),
+                            ),
+                            HGroup(
+                                Item(name="rn", label="Rn", tooltip="standard deviation of random noise"),
+                                Item(label="V"),
+                            ),
+                            HGroup(
+                                Item(name="pn_mag", label="Pn", tooltip="peak magnitude of periodic noise"),
+                                Item(label="V"),
+                            ),
+                            HGroup(
+                                Item(name="pn_freq", label="f(Pn)", tooltip="frequency of periodic noise"),
+                                Item(label="MHz"),
+                            ),
+                            label="Tx Level && Noise",
+                            show_border=True,
                         ),
                     ),
+                    HGroup(
+                        Item(name="debug", label="Debug", tooltip="Enable to log extra information to console."),
+                        label="Miscellaneous Options",
+                        show_border=True,
+                    ),
                     label="Simulation Control",
                     show_border=True,
                 ),
                 VGroup(
-                    Item(
-                        name="thresh",
-                        label="Pj Threshold (sigma)",
-                        tooltip="Threshold for identifying periodic jitter spectral elements. (sigma)",
+                    HGroup(
+                        Item(
+                            name="impulse_length",
+                            label="Impulse Response Length",
+                            tooltip="Manual impulse response length override",
+                        ),
+                        Item(label="ns"),
+                        spring,
                     ),
-                    Item(
-                        name="impulse_length",
-                        label="Impulse Response Length (ns)",
-                        tooltip="Manual impulse response length override",
+                    HGroup(
+                        Item(
+                            name="thresh",
+                            label="Pj Threshold",
+                            tooltip="Threshold for identifying periodic jitter spectral elements. (sigma)",
+                        ),
+                        Item(label="sigma"),
+                        spring,
+                    ),
+                    HGroup(
+                        Item(
+                            name="f_max",
+                            label="fMax",
+                            tooltip="Maximum frequency used for plotting, modeling, and signal processing. (GHz)",
+                        ),
+                        Item(label="GHz"),
+                        spring,
+                    ),
+                    HGroup(
+                        Item(
+                            name="f_step",
+                            label="fStep",
+                            tooltip="Frequency step used for plotting, modeling, and signal processing. (MHz)",
+                        ),
+                        Item(label="MHz"),
+                        spring,
                     ),
-                    Item(name="debug", label="Debug", tooltip="Enable to log extra information to console."),
                     label="Analysis Parameters",
                     show_border=True,
                 ),
             ),
-            HGroup(
-                VGroup(
+            HGroup(  # "Channel"
+                VGroup(  # "Tx"
                     VGroup(
                         HGroup(
                             Item(
                                 name="tx_ibis_file",
                                 label="File",
                                 springy=True,
                                 editor=FileEditor(dialog_style="open", filter=["*.ibs"]),
                             ),
                             Item(name="tx_ibis_valid", label="Valid", style="simple", enabled_when="False"),
                         ),
                         HGroup(
                             Item(name="tx_use_ibis", label="Use IBIS"),
                             Item(name="btn_sel_tx", show_label=False),
                             Item(name="btn_view_tx", show_label=False),
-                            Item(
-                                name="tx_use_ts4",
-                                label="Use on-die S-parameters.",
-                                enabled_when="tx_use_ibis and tx_has_ts4",
-                            ),
-                            enabled_when="tx_ibis_valid == True",
+                            enabled_when="tx_ibis_valid",
                         ),
+                        Item(name="tx_use_ts4", label="Use on-die S-parameters.",
+                             enabled_when="tx_use_ibis and tx_ibis_valid and tx_has_ts4",),
                         label="IBIS",
                         show_border=True,
                     ),
                     VGroup(
-                        Item(
-                            name="rs",
-                            label="Tx_Rs (Ohms)",
-                            tooltip="Tx differential source impedance",
+                        HGroup(
+                            Item(
+                                name="rs",
+                                label="Tx_Rs",
+                                tooltip="Tx differential source impedance",
+                            ),
+                            Item(label="Ohms"),
+                            spring,
                         ),
-                        Item(
-                            name="cout",
-                            label="Tx_Cout (pF)",
-                            tooltip="Tx parasitic output capacitance (each pin)",
-                            editor=TextEditor(auto_set=False, enter_set=True, evaluate=float),
+                        HGroup(
+                            Item(
+                                name="cout",
+                                label="Tx_Cout",
+                                tooltip="Tx parasitic output capacitance (each pin)",
+                                editor=TextEditor(auto_set=False, enter_set=True, evaluate=float),
+                            ),
+                            Item(label="pF"),
+                            spring,
                         ),
                         label="Native",
                         show_border=True,
                         enabled_when="tx_use_ibis == False",
                     ),
                     label="Tx",
                     show_border=True,
                 ),
                 VGroup(  # Interconnect
                     VGroup(  # From File
                         VGroup(
-                            HGroup(
-                                Item(
-                                    name="ch_file",
-                                    label="File",
-                                    springy=True,
-                                    editor=FileEditor(dialog_style="open"),
-                                ),
+                            Item(
+                                name="ch_file",
+                                label="File",
+                                editor=FileEditor(dialog_style="open"),
                             ),
                             HGroup(
                                 Item(
                                     name="use_ch_file",
                                     label="Use file",
                                 ),
+                                Item(
+                                    name="renumber",
+                                    label="Fix port numbering",
+                                ),
                                 spring,
-                                # Item(name="padded",   label="Zero-padded", enabled_when="use_ch_file == True"),
-                                # Item(name="windowed", label="Windowed",    enabled_when="use_ch_file == True"),
-                            ),
-                        ),
-                        HGroup(
-                            Item(
-                                name="f_step",
-                                label="f_step",
-                                tooltip="Frequency step to use in generating H(f).",
                             ),
-                            Item(label="MHz"),
-                            enabled_when="use_ch_file == True",
                         ),
                         label="From File",
                         show_border=True,
                     ),
                     HGroup(  # Native (i.e. - Howard Johnson's) interconnect model.
                         VGroup(
-                            Item(
-                                name="l_ch",
-                                label="Length (m)",
-                                tooltip="interconnect length",
+                            HGroup(
+                                Item(
+                                    name="l_ch",
+                                    label="Length",
+                                    tooltip="interconnect length",
+                                ),
+                                Item(label="m"),
+                                spring,
                             ),
-                            Item(
-                                name="Theta0",
-                                label="Loss Tan.",
-                                tooltip="dielectric loss tangent",
+                            HGroup(
+                                Item(
+                                    name="Theta0",
+                                    label="Loss Tan.",
+                                    tooltip="dielectric loss tangent",
+                                ),
+                                spring,
                             ),
-                            Item(
-                                name="Z0",
-                                label="Z0 (Ohms)",
-                                tooltip="characteristic differential impedance",
+                            HGroup(
+                                Item(
+                                    name="Z0",
+                                    label="Z0",
+                                    tooltip="characteristic differential impedance",
+                                ),
+                                Item(label="Ohms"),
+                                spring,
                             ),
-                            Item(
-                                name="v0",
-                                label="v_rel (c)",
-                                tooltip="normalized propagation velocity",
+                            HGroup(
+                                Item(
+                                    name="v0",
+                                    label="v_rel",
+                                    tooltip="normalized propagation velocity",
+                                ),
+                                Item(label="c"),
+                                spring,
                             ),
                         ),
+                        spring,
                         VGroup(
-                            Item(
-                                name="Rdc",
-                                label="Rdc (Ohms)",
-                                tooltip="d.c. resistance",
+                            HGroup(
+                                spring,
+                                Item(
+                                    name="Rdc",
+                                    label="Rdc",
+                                    tooltip="d.c. resistance",
+                                ),
+                                Item(label="Ohms"),
                             ),
-                            Item(
-                                name="w0",
-                                label="w0 (rads./s)",
-                                tooltip="transition frequency",
+                            HGroup(
+                                spring,
+                                Item(
+                                    name="w0",
+                                    label="w0",
+                                    tooltip="transition frequency",
+                                ),
+                                Item(label="rads./s"),
                             ),
-                            Item(
-                                name="R0",
-                                label="R0 (Ohms)",
-                                tooltip="skin effect resistance",
+                            HGroup(
+                                spring,
+                                Item(
+                                    name="R0",
+                                    label="R0",
+                                    tooltip="skin effect resistance",
+                                ),
+                                Item(label="Ohms"),
                             ),
                         ),
                         label="Native",
                         show_border=True,
                         enabled_when="use_ch_file == False",
                     ),
+                    HGroup(  # Misc.
+                        Item(
+                            name="use_window",
+                            label="Apply window",
+                            tooltip="Apply raised cosine window to frequency response before FFT()'ing.",
+                        ),
+                        label="Misc.",
+                        show_border=True,
+                    ),
                     label="Interconnect",
                     show_border=True,
                 ),
-                VGroup(
+                VGroup(  # Rx
                     VGroup(
                         HGroup(
                             Item(
                                 name="rx_ibis_file",
                                 label="File",
                                 springy=True,
                                 editor=FileEditor(dialog_style="open", filter=["*.ibs"]),
                             ),
                             Item(name="rx_ibis_valid", label="Valid", style="simple", enabled_when="False"),
                         ),
                         HGroup(
                             Item(name="rx_use_ibis", label="Use IBIS"),
                             Item(name="btn_sel_rx", show_label=False),
                             Item(name="btn_view_rx", show_label=False),
-                            Item(
-                                name="rx_use_ts4",
-                                label="Use on-die S-parameters.",
-                                enabled_when="rx_use_ibis and rx_has_ts4",
-                            ),
-                            enabled_when="rx_ibis_valid == True",
+                            enabled_when="rx_ibis_valid",
                         ),
+                        Item(name="rx_use_ts4", label="Use on-die S-parameters.",
+                             enabled_when="rx_use_ibis and rx_ibis_valid and rx_has_ts4",),
                         label="IBIS",
                         show_border=True,
                     ),
                     VGroup(
-                        Item(
-                            name="rin",
-                            label="Rx_Rin (Ohms)",
-                            tooltip="Rx differential input impedance",
+                        HGroup(
+                            Item(
+                                name="rin",
+                                label="Rx_Rin",
+                                tooltip="Rx differential input impedance",
+                            ),
+                            Item(label="Ohms"),
+                            spring,
                         ),
-                        Item(
-                            name="cin",
-                            label="Rx_Cin (pF)",
-                            tooltip="Rx parasitic input capacitance (each pin)",
-                            editor=TextEditor(auto_set=False, enter_set=True, evaluate=float),
+                        HGroup(
+                            Item(
+                                name="cin",
+                                label="Rx_Cin",
+                                tooltip="Rx parasitic input capacitance (each pin)",
+                                editor=TextEditor(auto_set=False, enter_set=True, evaluate=float),
+                            ),
+                            Item(label="pF"),
+                            spring,
                         ),
-                        Item(
-                            name="cac",
-                            label="Rx_Cac (uF)",
-                            tooltip="Rx a.c. coupling capacitance (each pin)",
+                        HGroup(
+                            Item(
+                                name="cac",
+                                label="Rx_Cac",
+                                tooltip="Rx a.c. coupling capacitance (each pin)",
+                            ),
+                            Item(label="uF"),
+                            spring,
                         ),
                         label="Native",
                         show_border=True,
                         enabled_when="rx_use_ibis == False",
                     ),
                     label="Rx",
                     show_border=True,
                 ),
                 label="Channel",
                 show_border=True,
             ),
-            # spring,
             label="Config.",
             id="config",
         ),
         # "Equalization" tab.
-        VGroup(  # Channel Parameters
-            HGroup(
+        HGroup(  # Channel Parameters
+            VGroup(
                 VGroup(
-                    VGroup(
-                        HGroup(
-                            VGroup(
-                                HGroup(
-                                    Item(name="tx_ami_file", label="AMI File:", style="readonly", springy=True),
-                                    Item(name="tx_ami_valid", label="Valid", style="simple", enabled_when="False"),
-                                ),
-                                HGroup(
-                                    Item(name="tx_dll_file", label="DLL File:", style="readonly", springy=True),
-                                    Item(name="tx_dll_valid", label="Valid", style="simple", enabled_when="False"),
-                                ),
+                    HGroup(
+                        VGroup(
+                            HGroup(
+                                Item(name="tx_ami_file", label="AMI File:", style="readonly", springy=True),
+                                Item(name="tx_ami_valid", label="Valid", style="simple", enabled_when="False"),
                             ),
-                            VGroup(
-                                Item(
-                                    name="tx_use_ami",
-                                    label="Use AMI",
-                                    tooltip="You must select both files, first.",
-                                    enabled_when="tx_ami_valid == True and tx_dll_valid == True",
-                                ),
-                                Item(
-                                    name="tx_use_getwave",
-                                    label="Use GetWave",
-                                    tooltip="Use the model's GetWave() function.",
-                                    enabled_when="tx_use_ami and tx_has_getwave",
-                                ),
-                                Item(
-                                    "btn_cfg_tx",
-                                    show_label=False,
-                                    tooltip="Configure Tx AMI parameters.",
-                                    enabled_when="tx_ami_valid == True",
-                                ),
+                            HGroup(
+                                Item(name="tx_dll_file", label="DLL File:", style="readonly", springy=True),
+                                Item(name="tx_dll_valid", label="Valid", style="simple", enabled_when="False"),
+                            ),
+                        ),
+                        VGroup(
+                            Item(
+                                name="tx_use_ami",
+                                label="Use AMI",
+                                tooltip="You must select both files, first.",
+                                enabled_when="tx_ami_valid == True and tx_dll_valid == True",
+                            ),
+                            Item(
+                                name="tx_use_getwave",
+                                label="Use GetWave",
+                                tooltip="Use the model's GetWave() function.",
+                                enabled_when="tx_use_ami and tx_has_getwave",
+                            ),
+                            Item(
+                                "btn_cfg_tx",
+                                show_label=False,
+                                tooltip="Configure Tx AMI parameters.",
+                                enabled_when="tx_ami_valid == True",
                             ),
                         ),
-                        label="IBIS-AMI",
-                        show_border=True,
                     ),
-                    VGroup(
-                        Item(
-                            name="tx_taps",
-                            editor=TableEditor(
-                                columns=[
-                                    ObjectColumn(name="name", editable=False),
-                                    ObjectColumn(name="enabled", style="simple"),
-                                    ObjectColumn(name="min_val", horizontal_alignment="center"),
-                                    ObjectColumn(name="max_val", horizontal_alignment="center"),
-                                    ObjectColumn(name="value", format="%+05.3f", horizontal_alignment="center"),
-                                    ObjectColumn(name="steps", horizontal_alignment="center"),
-                                ],
-                                configurable=False,
-                                reorderable=False,
-                                sortable=False,
-                                selection_mode="cell",
-                                # auto_size=True,
-                                rows=4,
+                    label="IBIS-AMI",
+                    show_border=True,
+                ),
+                VGroup(
+                    Item(
+                        name="tx_taps",
+                        editor=TableEditor(
+                            columns=[
+                                ObjectColumn(name="name", editable=False),
+                                ObjectColumn(name="enabled", style="simple"),
+                                ObjectColumn(name="value", format="%+05.3f", horizontal_alignment="center"),
+                            ],
+                            configurable=False,
+                            reorderable=False,
+                            sortable=False,
+                            selection_mode="cell",
+                            rows=4,
+                        ),
+                        show_label=False,
+                    ),
+                    label="Native",
+                    show_border=True,
+                    enabled_when="tx_use_ami == False",
+                ),
+                label="Tx Equalization",
+                show_border=True,
+            ),
+            VGroup(
+                VGroup(
+                    HGroup(
+                        VGroup(
+                            HGroup(
+                                Item(name="rx_ami_file", label="AMI File:", style="readonly", springy=True),
+                                Item(name="rx_ami_valid", label="Valid", style="simple", enabled_when="False"),
+                            ),
+                            HGroup(
+                                Item(name="rx_dll_file", label="DLL File:", style="readonly", springy=True),
+                                Item(name="rx_dll_valid", label="Valid", style="simple", enabled_when="False"),
+                            ),
+                        ),
+                        VGroup(
+                            Item(
+                                name="rx_use_ami",
+                                label="Use AMI",
+                                tooltip="You must select both files, first.",
+                                enabled_when="rx_ami_valid == True and rx_dll_valid == True",
+                            ),
+                            Item(
+                                name="rx_use_getwave",
+                                label="Use GetWave",
+                                tooltip="Use the model's GetWave() function.",
+                                enabled_when="rx_use_ami and rx_has_getwave",
+                            ),
+                            Item(
+                                "btn_cfg_rx",
+                                show_label=False,
+                                tooltip="Configure Rx AMI parameters.",
+                                enabled_when="rx_ami_valid == True",
                             ),
-                            show_label=False,
                         ),
-                        label="Native",
-                        show_border=True,
-                        enabled_when="tx_use_ami == False",
                     ),
-                    label="Tx Equalization",
+                    label="IBIS-AMI",
                     show_border=True,
                 ),
                 VGroup(
-                    VGroup(
-                        HGroup(
-                            VGroup(
-                                HGroup(
-                                    Item(name="rx_ami_file", label="AMI File:", style="readonly", springy=True),
-                                    Item(name="rx_ami_valid", label="Valid", style="simple", enabled_when="False"),
-                                ),
-                                HGroup(
-                                    Item(name="rx_dll_file", label="DLL File:", style="readonly", springy=True),
-                                    Item(name="rx_dll_valid", label="Valid", style="simple", enabled_when="False"),
-                                ),
+                    VGroup(  # CTLE
+                        Item(name="ctle_enable", label="Enable", tooltip="CTLE enable",),
+                        HGroup(  # File
+                            Item(
+                                name="use_ctle_file",
+                                label="Use",
+                                tooltip="Select CTLE impulse/step response from file.",
+                                enabled_when="ctle_file",
                             ),
-                            VGroup(
+                            Item(
+                                name="ctle_file",
+                                label="Filename",
+                                enabled_when="use_ctle_file == True",
+                                editor=FileEditor(dialog_style="open"),
+                            ),
+                            label="File",
+                            show_border=True,
+                        ),
+                        VGroup(  # Model
+                            HGroup(
                                 Item(
-                                    name="rx_use_ami",
-                                    label="Use AMI",
-                                    tooltip="You must select both files, first.",
-                                    enabled_when="rx_ami_valid == True and rx_dll_valid == True",
+                                    name="peak_freq",
+                                    label="CTLE fp",
+                                    tooltip="CTLE peaking frequency (GHz)",
+                                    enabled_when="use_ctle_file == False",
                                 ),
+                                Item(label="GHz"),
+                                spring,
                                 Item(
-                                    name="rx_use_getwave",
-                                    label="Use GetWave",
-                                    tooltip="Use the model's GetWave() function.",
-                                    enabled_when="rx_use_ami and rx_has_getwave",
+                                    name="rx_bw",
+                                    label="Bandwidth",
+                                    tooltip="unequalized signal path bandwidth (GHz).",
+                                    enabled_when="use_ctle_file == False",
                                 ),
+                                Item(label="GHz"),
+                            ),
+                            HGroup(
                                 Item(
-                                    "btn_cfg_rx",
-                                    show_label=False,
-                                    tooltip="Configure Rx AMI parameters.",
-                                    enabled_when="rx_ami_valid == True",
+                                    name="peak_mag",
+                                    label="CTLE boost",
+                                    tooltip="CTLE peaking magnitude (dB)",
+                                    format_str="%4.1f",
+                                    enabled_when="use_ctle_file == False",
                                 ),
+                                Item(label="dB"),
+                                spring,
                             ),
+                            label="Model",
+                            show_border=True,
+                            enabled_when="use_ctle_file == False",
                         ),
-                        label="IBIS-AMI",
+                        label="CTLE",
                         show_border=True,
+                        enabled_when="rx_use_ami == False",
                     ),
-                    VGroup(
+                    HGroup(
                         VGroup(
-                            VGroup(
-                                HGroup(
-                                    Item(
-                                        name="use_ctle_file",
-                                        label="fromFile",
-                                        tooltip="Select CTLE impulse/step response from file.",
-                                    ),
-                                    Item(
-                                        name="ctle_file",
-                                        label="Filename",
-                                        enabled_when="use_ctle_file == True",
-                                        editor=FileEditor(dialog_style="open"),
-                                    ),
-                                ),
-                                HGroup(
-                                    Item(
-                                        name="peak_freq",
-                                        label="CTLE fp (GHz)",
-                                        tooltip="CTLE peaking frequency (GHz)",
-                                        enabled_when="use_ctle_file == False",
-                                    ),
-                                    Item(
-                                        name="rx_bw",
-                                        label="Bandwidth (GHz)",
-                                        tooltip="unequalized signal path bandwidth (GHz).",
-                                        enabled_when="use_ctle_file == False",
-                                    ),
-                                ),
-                                HGroup(
-                                    Item(
-                                        name="peak_mag",
-                                        label="CTLE boost (dB)",
-                                        tooltip="CTLE peaking magnitude (dB)",
-                                        format_str="%4.1f",
-                                        enabled_when="use_ctle_file == False",
-                                    ),
-                                    Item(
-                                        name="ctle_mode",
-                                        label="CTLE mode",
-                                        tooltip="CTLE Operating Mode",
-                                        enabled_when="use_ctle_file == False",
-                                    ),
-                                    Item(
-                                        name="ctle_offset",
-                                        tooltip="CTLE d.c. offset (dB)",
-                                        show_label=False,
-                                        enabled_when='ctle_mode == "Manual"',
-                                    ),
-                                ),
-                                label="CTLE",
-                                show_border=True,
-                                enabled_when="rx_use_ami == False",
-                            ),
-                        ),
-                        HGroup(
-                            VGroup(
+                            HGroup(
                                 Item(
                                     name="delta_t",
-                                    label="Delta-t (ps)",
+                                    label="Delta-t",
                                     tooltip="magnitude of CDR proportional branch",
                                 ),
-                                Item(name="alpha", label="Alpha", tooltip="relative magnitude of CDR integral branch"),
-                                Item(
-                                    name="n_lock_ave",
-                                    label="Lock Nave.",
-                                    tooltip="# of UI estimates to average, when determining lock",
-                                ),
-                                Item(
-                                    name="rel_lock_tol",
-                                    label="Lock Tol.",
-                                    tooltip="relative tolerance for determining lock",
-                                ),
-                                Item(
-                                    name="lock_sustain",
-                                    label="Lock Sus.",
-                                    tooltip="length of lock determining hysteresis vector",
-                                ),
-                                label="CDR",
-                                show_border=True,
+                                Item(label="ps"),
+                            ),
+                            Item(name="alpha", label="Alpha", tooltip="relative magnitude of CDR integral branch"),
+                            Item(
+                                name="n_lock_ave",
+                                label="Lock Nave.",
+                                tooltip="# of UI estimates to average, when determining lock",
+                            ),
+                            Item(
+                                name="rel_lock_tol",
+                                label="Lock Tol.",
+                                tooltip="relative tolerance for determining lock",
                             ),
+                            Item(
+                                name="lock_sustain",
+                                label="Lock Sus.",
+                                tooltip="length of lock determining hysteresis vector",
+                            ),
+                            label="CDR",
+                            show_border=True,
+                        ),
+                        VGroup(
+                            Item(label="Use Optimizer tab to configure."),
                             VGroup(
+                                Item(name="gain", label="Gain", tooltip="error feedback gain"),
+                                Item(name="n_ave", label="Nave.", tooltip="# of CDR adaptations per DFE adaptation"),
+                                HGroup(
+                                    Item(name="decision_scaler", label="Level", tooltip="target output magnitude"),
+                                    Item(label="V"),
+                                ),
                                 HGroup(
                                     Item(
-                                        name="use_dfe",
-                                        label="Use DFE",
-                                        tooltip="Include DFE in simulation.",
+                                        name="sum_bw",
+                                        label="Bandwidth",
+                                        tooltip="summing node bandwidth",
+                                        enabled_when="sum_ideal == False",
                                     ),
+                                    Item(label="GHz"),
                                     Item(
                                         name="sum_ideal",
                                         label="Ideal",
                                         tooltip="Use ideal DFE. (performance boost)",
-                                        enabled_when="use_dfe == True",
                                     ),
                                 ),
-                                VGroup(
-                                    Item(name="n_taps", label="Taps", tooltip="# of taps"),
-                                    Item(name="gain", label="Gain", tooltip="error feedback gain"),
-                                    Item(name="decision_scaler", label="Level", tooltip="target output magnitude"),
-                                    Item(
-                                        name="n_ave", label="Nave.", tooltip="# of CDR adaptations per DFE adaptation"
-                                    ),
-                                    Item(
-                                        name="sum_bw",
-                                        label="BW (GHz)",
-                                        tooltip="summing node bandwidth",
-                                        enabled_when="sum_ideal == False",
-                                    ),
-                                    enabled_when="use_dfe == True",
-                                ),
-                                label="DFE",
-                                show_border=True,
                             ),
+                            label="DFE",
+                            show_border=True,
                         ),
-                        label="Native",
-                        show_border=True,
-                        enabled_when="rx_use_ami == False",
                     ),
-                    label="Rx Equalization",
+                    label="Native",
                     show_border=True,
+                    enabled_when="rx_use_ami == False",
                 ),
-                springy=True,
+                label="Rx Equalization",
+                show_border=True,
             ),
-            HGroup(),
             label="Equalization",
-            id="channel",
+            id="equalization",
         ),
         # "Optimizer" tab.
         VGroup(
-            HGroup(
-                Group(
+            HGroup(  # EQ Config.
+                Group(  # Tx FFE Config.
                     Item(
                         name="tx_tap_tuners",
                         editor=TableEditor(
                             columns=[
                                 ObjectColumn(name="name", editable=False),
                                 ObjectColumn(name="enabled"),
                                 ObjectColumn(name="min_val"),
                                 ObjectColumn(name="max_val"),
+                                ObjectColumn(name="step"),
                                 ObjectColumn(name="value", format="%+05.3f"),
                             ],
                             configurable=False,
                             reorderable=False,
                             sortable=False,
                             selection_mode="cell",
                             auto_size=False,
-                            rows=4,
+                            rows=6,
                             orientation="horizontal",
                             is_grid_cell=True,
                         ),
                         show_label=False,
                     ),
-                    label="Tx Equalization",
+                    label="Tx FFE",
                     show_border=True,
-                    springy=True,
                 ),
-                # HGroup(
-                VGroup(
-                    HGroup(
-                        Item(
-                            name="peak_mag_tune",
-                            label="CTLE: boost (dB)",
-                            tooltip="CTLE peaking magnitude (dB)",
-                            format_str="%4.1f",
+                VGroup(  # Rx CTLE
+                    Item(name="ctle_enable_tune", label="Enable", tooltip="CTLE enable",),
+                    VGroup(
+                        HGroup(
+                            Item(name="peak_freq_tune", label="fp", tooltip="CTLE peaking frequency (GHz)",
+                                 enabled_when="ctle_enable_tune",),
+                            Item(label="GHz"),
                         ),
-                        Item(
-                            name="max_mag_tune",
-                            label="Max boost (dB)",
-                            tooltip="CTLE maximum peaking magnitude (dB)",
-                            format_str="%4.1f",
+                        HGroup(
+                            Item(name="rx_bw_tune", label="BW", tooltip="unequalized signal path bandwidth (GHz).",
+                                 enabled_when="ctle_enable_tune",),
+                            Item(label="GHz"),
                         ),
-                    ),
-                    HGroup(
-                        Item(name="peak_freq_tune", label="fp (GHz)", tooltip="CTLE peaking frequency (GHz)"),
-                        Item(
-                            name="rx_bw_tune",
-                            label="BW (GHz)",
-                            tooltip="unequalized signal path bandwidth (GHz).",
+                        HGroup(
+                            Item(name="min_mag_tune", label="Min.", tooltip="CTLE peaking magnitude minimum (dB)",
+                                 format_str="%4.1f", enabled_when="ctle_enable_tune",),
+                            Item(label="dB"),
                         ),
-                    ),
-                    HGroup(
-                        Item(name="ctle_mode_tune", label="mode", tooltip="CTLE Operating Mode"),
-                        Item(
-                            name="ctle_offset_tune",
-                            tooltip="CTLE d.c. offset (dB)",
-                            show_label=False,
-                            enabled_when='ctle_mode_tune == "Manual"',
+                        HGroup(
+                            Item(name="max_mag_tune", label="Max.", tooltip="CTLE peaking magnitude maximum (dB)",
+                                 format_str="%4.1f", enabled_when="ctle_enable_tune",),
+                            Item(label="dB"),
+                        ),
+                        HGroup(
+                            Item(name="step_mag_tune", label="Step", tooltip="CTLE peaking magnitude step (dB)",
+                                 format_str="%4.1f", enabled_when="ctle_enable_tune",),
+                            Item(label="dB"),
                         ),
+                        label="Configuration",
+                        show_border=True,
+                        enabled_when="ctle_enable_tune",
                     ),
                     HGroup(
-                        Item(name="use_dfe_tune", label="DFE: Enable", tooltip="Include ideal DFE in optimization."),
-                        Item(name="n_taps_tune", label="Taps", tooltip="Number of DFE taps."),
+                        Item(name="peak_mag_tune", label="Boost", tooltip="CTLE peaking magnitude result (dB)",
+                             format_str="%4.1f", style="readonly"),
+                        Item(label="dB"),
+                        label="Result",
+                        show_border=True,
+                        enabled_when="ctle_enable_tune",
                     ),
-                    label="Rx Equalization",
+                    label="Rx CTLE",
                     show_border=True,
                 ),
-                # ),
                 VGroup(
-                    Item(
-                        name="max_iter",
-                        label="Max. Iterations",
-                        tooltip="Maximum number of iterations to allow, during optimization.",
-                    ),
-                    Item(
-                        name="rel_opt",
-                        label="Rel. Opt.:",
-                        format_str="%7.4f",
-                        tooltip="Relative optimization metric.",
-                        style="readonly",
+                    HGroup(
+                        Item(name="btn_disable", show_label=False, tooltip="Disable all DFE taps."),
+                        Item(name="btn_enable",  show_label=False, tooltip="Enable all DFE taps."),
                     ),
                     Item(
-                        name="przf_err",
-                        label="PRZF Err.:",
-                        format_str="%5.3f",
-                        tooltip="Pulse Response Zero Forcing approximation error.",
-                        style="readonly",
+                        name="dfe_tap_tuners",
+                        editor=TableEditor(
+                            columns=[
+                                ObjectColumn(name="name", editable=False),
+                                ObjectColumn(name="enabled"),
+                                ObjectColumn(name="min_val"),
+                                ObjectColumn(name="max_val"),
+                                ObjectColumn(name="value", format="%+05.3f", style="readonly"),
+                            ],
+                            configurable=False,
+                            reorderable=False,
+                            sortable=False,
+                            selection_mode="cell",
+                            auto_size=True,
+                            rows=6,
+                            orientation="horizontal",
+                            is_grid_cell=True,
+                        ),
+                        show_label=False,
                     ),
-                    label="Tuning Options",
+                    label="Rx DFE",
                     show_border=True,
                 ),
-                springy=False,
             ),
             Item(
-                label="Note: Only CTLE boost will be optimized; please, set peak frequency, bandwidth, and mode appropriately.",
-            ),
-            Item("plot_h_tune", editor=ComponentEditor(high_resolution=False), show_label=False, springy=True),
-            HGroup(
-                Item("btn_rst_eq", show_label=False, tooltip="Reset all values to those on the 'Config.' tab."),
-                Item("btn_save_eq", show_label=False, tooltip="Store all values to 'Config.' tab."),
-                Item("btn_opt_tx", show_label=False, tooltip="Run Tx tap weight optimization."),
-                Item("btn_opt_rx", show_label=False, tooltip="Run Rx CTLE optimization."),
-                Item("btn_coopt", show_label=False, tooltip="Run co-optimization."),
-                Item("btn_abort", show_label=False, tooltip="Abort all optimizations."),
+                label="To zoom: Click in the plot, hit `z` (Cursor will change to crosshair.), and click/drag to select horizontal region of interest.",
             ),
+            Item("plot_h_tune", editor=ComponentEditor(high_resolution=HIGH_RES), show_label=False, springy=True),
             label="Optimizer",
             id="eq_tune",
         ),
         Group(  # Responses
             Group(
-                Item("plots_h", editor=ComponentEditor(high_resolution=False), show_label=False),
+                Item("plots_h", editor=ComponentEditor(high_resolution=HIGH_RES), show_label=False),
                 label="Impulses",
                 id="plots_h",
             ),
             Group(
-                Item("plots_s", editor=ComponentEditor(high_resolution=False), show_label=False),
+                Item("plots_s", editor=ComponentEditor(high_resolution=HIGH_RES), show_label=False),
                 label="Steps",
                 id="plots_s",
             ),
             Group(
-                Item("plots_p", editor=ComponentEditor(high_resolution=False), show_label=False),
+                Item("plots_p", editor=ComponentEditor(high_resolution=HIGH_RES), show_label=False),
                 label="Pulses",
                 id="plots_p",
             ),
             Group(
-                Item("plots_H", editor=ComponentEditor(high_resolution=False), show_label=False),
+                Item("plots_H", editor=ComponentEditor(high_resolution=HIGH_RES), show_label=False),
                 label="Freq. Resp.",
                 id="plots_H",
             ),
             layout="tabbed",
             label="Responses",
             id="responses",
         ),
         Group(  # Results
             Group(
-                Item("plots_dfe", editor=ComponentEditor(high_resolution=False), show_label=False),
+                Item("plots_dfe", editor=ComponentEditor(high_resolution=HIGH_RES), show_label=False),
                 label="DFE",
                 id="plots_dfe",
             ),
             Group(
-                Item("plots_out", editor=ComponentEditor(high_resolution=False), show_label=False),
+                Item("plots_out", editor=ComponentEditor(high_resolution=HIGH_RES), show_label=False),
                 label="Outputs",
                 id="plots_out",
             ),
             Group(
-                Item("plots_eye", editor=ComponentEditor(high_resolution=False), show_label=False),
+                Item("plots_eye", editor=ComponentEditor(high_resolution=HIGH_RES), show_label=False),
                 label="Eyes",
                 id="plots_eye",
             ),
             Group(
-                Item("plots_bathtub", editor=ComponentEditor(high_resolution=False), show_label=False),
+                Item("plots_bathtub", editor=ComponentEditor(high_resolution=HIGH_RES), show_label=False),
                 label="Bathtubs",
                 id="plots_bathtub",
             ),
-            Group(Item("sweep_info", style="readonly", show_label=False), label="Sweep Info"),
             layout="tabbed",
             label="Results",
             id="results",
         ),
         Group(  # Jitter
             Group(
-                Item("plots_jitter_dist", editor=ComponentEditor(high_resolution=False), show_label=False),
+                Item("plots_jitter_dist", editor=ComponentEditor(high_resolution=HIGH_RES), show_label=False),
                 label="Jitter Dist.",
                 id="plots_jitter_dist",
             ),
             Group(
-                Item("plots_jitter_spec", editor=ComponentEditor(high_resolution=False), show_label=False),
+                Item("plots_jitter_spec", editor=ComponentEditor(high_resolution=HIGH_RES), show_label=False),
                 label="Jitter Spec.",
                 id="plots_jitter_spec",
             ),
             Group(Item("jitter_info", style="readonly", show_label=False), label="Jitter Info"),
             layout="tabbed",
             label="Jitter",
             id="jitter",
         ),
         Group(  # Info
             Group(
                 Item("perf_info", style="readonly", show_label=False),
                 label="Performance",
             ),
             Group(Item("instructions", style="readonly", show_label=False), label="User's Guide"),
-            Group(Item("console_log", style="readonly", show_label=False), label="Console", id="console"),
+            Group(Item("console_log", style="custom", show_label=False), label="Console", id="console"),
             layout="tabbed",
             label="Info",
             id="info",
         ),
         layout="tabbed",
         springy=True,
         id="tabs",
     ),
-    resizable=True,
-    handler=MyHandler(),
     menubar=MenuBar(
         Menu(
-            Action(name="Load Config.", action="do_load_cfg", accelerator="Ctrl+O"),
+            Action(name="&Quit", action="close_app", accelerator="Ctrl+Q"),  # CloseAction()
+            Separator(),
             Action(name="Load Results", action="do_load_data"),
+            Action(name="Save Results", action="do_save_data"),
             Separator(),
+            Action(name="Load Config.", action="do_load_cfg", accelerator="Ctrl+O"),
             Action(name="Save Config.", action="do_save_cfg", accelerator="Ctrl+S"),
             Action(name="Save Config. As...", action="do_save_cfg_as", accelerator="Ctrl+Shift+S"),
-            Action(name="Save Results", action="do_save_data"),
-            Separator(),
-            Action(name="&Quit", action="close_app", accelerator="Ctrl+Q"),  # CloseAction()
             id="file",
             name="&File",
         ),
         Menu(
             Action(
                 name="Debug Mode",
                 action="toggle_debug_clicked",
@@ -908,22 +823,36 @@
             Action(
                 name="Clear Loaded Waveforms",
                 action="do_clear_data",
             ),
             id="view",
             name="&View",
         ),
-        Menu(Action(name="Run", action="do_run_simulation", accelerator="Ctrl+R"), id="simulation", name="Simulation"),
+        Menu(
+            Action(name="Run", action="do_run_simulation", accelerator="Ctrl+R"),
+            Action(name="Abort", action="do_stop_simulation"),
+            id="simulation",
+            name="Simulation",
+        ),
+        Menu(
+            Action(name="Use EQ", action="do_use_eq", accelerator="Ctrl+U"),
+            Action(name="Reset EQ", action="do_reset_eq"),
+            Separator(),
+            Action(name="Tune EQ", action="do_tune_eq", accelerator="Ctrl+T"),
+            Action(name="Abort", action="do_stop_tune", accelerator="Ctrl+Esc"),
+            id="optimization",
+            name="Optimization",
+        ),
         Menu(
             Action(name="Getting Started", action="getting_started_clicked"),
             Action(name="&About", action="show_about_clicked"),
             id="help",
             name="&Help",
         ),
     ),
     buttons=NoButtons,
+    handler=MyHandler(),
+    icon=ImageResource("icon.png"),
+    resizable=True,
     statusbar="status_str",
     title="PyBERT",
-    # width=0.95,
-    # height=0.9,
-    icon=ImageResource("icon.png"),
 )
```

### Comparing `PipBERT-4.1.0/src/pybert/models/bert.py` & `pipbert-6.1.0/src/pybert/models/bert.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,532 +3,424 @@
 Original author: David Banas <capn.freako@gmail.com>
 
 Original date:   August 24, 2014 (Copied from pybert.py, as part of a major code cleanup.)
 
 Copyright (c) 2014 David Banas; all rights reserved World wide.
 """
 from time import perf_counter
-
-clock = perf_counter
+from typing import Callable, Optional
 
 import scipy.signal as sig
-from chaco.api import Plot
-from chaco.tools.api import PanTool, ZoomTool
-from numpy import (
+from numpy import (  # type: ignore
     arange,
     argmax,
     array,
     convolve,
     correlate,
-    cumsum,
     diff,
     histogram,
     linspace,
     mean,
-    ones,
-    pad,
     repeat,
     resize,
-    std,
     transpose,
     where,
     zeros,
 )
-from numpy.fft import fft, irfft
-from numpy.random import normal
-from pyibisami.ami.model import AMIModel, AMIModelInitializer
+from numpy.fft import rfft, irfft  # type: ignore
+from numpy.random import normal  # type: ignore
 from scipy.signal import iirfilter, lfilter
+from scipy.interpolate import interp1d
 
 from pybert.models.dfe import DFE
 from pybert.utility import (
     calc_eye,
     calc_jitter,
+    calc_resps,
     find_crossings,
-    getwave_step_resp,
     import_channel,
+    make_bathtub,
     make_ctle,
+    run_ami_model,
     safe_log10,
     trim_impulse,
 )
 
-DEBUG = False
-MIN_BATHTUB_VAL = 1.0e-18
-
-gFc = 1.0e6  # Corner frequency of high-pass filter used to model capacitive coupling of periodic noise.
+clock = perf_counter
 
+DEBUG           = False
+MIN_BATHTUB_VAL = 1.0e-18
+gFc             = 1.0e6  # Corner frequency of high-pass filter used to model capacitive coupling of periodic noise.
 
-def my_run_sweeps(self):
-    """Runs the simulation sweeps.
 
-    Args:
-        self(PyBERT): Reference to an instance of the *PyBERT* class.
+# pylint: disable=too-many-locals,protected-access,too-many-branches,too-many-statements
+def my_run_simulation(self, initial_run: bool = False, update_plots: bool = True,
+                      aborted_sim: Optional[Callable[[], bool]] = None):
     """
-
-    sweep_aves = self.sweep_aves
-    do_sweep = self.do_sweep
-    tx_taps = self.tx_taps
-
-    if do_sweep:
-        # Assemble the list of desired values for each sweepable parameter.
-        sweep_vals = []
-        for tap in tx_taps:
-            if tap.enabled:
-                if tap.steps:
-                    sweep_vals.append(list(arange(tap.min_val, tap.max_val, (tap.max_val - tap.min_val) / tap.steps)))
-                else:
-                    sweep_vals.append([tap.value])
-            else:
-                sweep_vals.append([0.0])
-        # Run the sweep, using the lists assembled, above.
-        sweeps = [
-            [w, x, y, z] for w in sweep_vals[0] for x in sweep_vals[1] for y in sweep_vals[2] for z in sweep_vals[3]
-        ]
-        num_sweeps = sweep_aves * len(sweeps)
-        self.num_sweeps = num_sweeps
-        sweep_results = []
-        sweep_num = 1
-        for sweep in sweeps:
-            for i in range(4):
-                self.tx_taps[i].value = sweep[i]
-            bit_errs = []
-            for i in range(sweep_aves):
-                self.sweep_num = sweep_num
-                my_run_simulation(self, update_plots=False)
-                bit_errs.append(self.bit_errs)
-                sweep_num += 1
-            sweep_results.append((sweep, mean(bit_errs), std(bit_errs)))
-        self.sweep_results = sweep_results
-    else:
-        my_run_simulation(self)
-
-
-def my_run_simulation(self, initial_run=False, update_plots=True):
-    """Runs the simulation.
+    Runs the simulation.
 
     Args:
-        self(PyBERT): Reference to an instance of the *PyBERT* class.
-        initial_run(Bool): If True, don't update the eye diagrams, since
+        self: Reference to an instance of the *PyBERT* class.
+
+    Keyword Args:
+        initial_run: If True, don't update the eye diagrams, since
             they haven't been created, yet.
-            (Optional; default = False.)
-        update_plots(Bool): If True, update the plots, after simulation
+            Default: False
+        update_plots: If True, update the plots, after simulation
             completes. This option can be used by larger scripts, which
             import *pybert*, in order to avoid graphical back-end
             conflicts and speed up this function's execution time.
-            (Optional; default = True.)
+            Default: True
+        aborted_sim: a function that is used to tell the simulation that the user
+            has requested to stop/abort the simulation.
+
+    Raises:
+        RuntimeError: If the simulation is aborted by the user or cannot continue.
+
+    Notes:
+        1. When using IBIS-AMI models, we often need to scale the impulse response
+            by the sample interval, or its inverse, because while IBIS-AMI models
+            take the impulse response to have units: (V/s), PyBERT uses: (V/sample).
     """
-    num_sweeps = self.num_sweeps
-    sweep_num = self.sweep_num
+
+    def _check_sim_status():
+        """Checks the status of the simulation thread and if this simulation needs to stop."""
+        if aborted_sim and aborted_sim():
+            self.status = "Aborted Simulation"
+            raise RuntimeError("Simulation aborted by User.")
 
     start_time = clock()
-    self.status = "Running channel...(sweep %d of %d)" % (sweep_num, num_sweeps)
+    self.status = "Running channel..."
 
     if not self.seed:  # The user sets `seed` to zero to indicate that she wants new bits generated for each run.
         self.run_count += 1  # Force regeneration of bit stream.
 
     # Pull class variables into local storage, performing unit conversion where necessary.
     t = self.t
+    t_irfft = self.t_irfft
+    f = self.f
     w = self.w
     bits = self.bits
     symbols = self.symbols
     ffe = self.ffe
     nbits = self.nbits
     nui = self.nui
-    bit_rate = self.bit_rate * 1.0e9
     eye_bits = self.eye_bits
     eye_uis = self.eye_uis
-    nspb = self.nspb
     nspui = self.nspui
     rn = self.rn
     pn_mag = self.pn_mag
     pn_freq = self.pn_freq * 1.0e6
     pattern = self.pattern_
     rx_bw = self.rx_bw * 1.0e9
     peak_freq = self.peak_freq * 1.0e9
     peak_mag = self.peak_mag
-    ctle_offset = self.ctle_offset
-    ctle_mode = self.ctle_mode
+    ctle_enable = self.ctle_enable
     delta_t = self.delta_t * 1.0e-12
     alpha = self.alpha
     ui = self.ui
-    n_taps = self.n_taps
     gain = self.gain
     n_ave = self.n_ave
     decision_scaler = self.decision_scaler
     n_lock_ave = self.n_lock_ave
+    dfe_tap_tuners = self.dfe_tap_tuners
     rel_lock_tol = self.rel_lock_tol
     lock_sustain = self.lock_sustain
     bandwidth = self.sum_bw * 1.0e9
     rel_thresh = self.thresh
     mod_type = self.mod_type[0]
+    impulse_length = self.impulse_length
 
-    try:
-        # Calculate misc. values.
-        fs = bit_rate * nspb
-        Ts = t[1]
-        ts = Ts
-
-        # Generate the ideal over-sampled signal.
-        #
-        # Duo-binary is problematic, in that it requires convolution with the ideal duobinary
-        # impulse response, in order to produce the proper ideal signal.
-        x = repeat(symbols, nspui)
-        self.x = x
-        if mod_type == 1:  # Handle duo-binary case.
-            duob_h = array(([0.5] + [0.0] * (nspui - 1)) * 2)
-            x = convolve(x, duob_h)[: len(t)]
-        self.ideal_signal = x
-
-        # Find the ideal crossing times, for subsequent jitter analysis of transmitted signal.
-        ideal_xings = find_crossings(t, x, decision_scaler, mod_type=mod_type)
-        self.ideal_xings = ideal_xings
+    # Calculate misc. values.
+    Ts = t[1]
+    ts = Ts
+    fs = 1 / ts
+    min_len =  30 * nspui
+    max_len = 100 * nspui
+    if impulse_length:
+        min_len = max_len = impulse_length / ts
+    if mod_type == 2:  # PAM-4
+        nspb = nspui // 2
+    else:
+        nspb = nspui
+    # Generate the ideal over-sampled signal.
+    #
+    # Duo-binary is problematic, in that it requires convolution with the ideal duobinary
+    # impulse response, in order to produce the proper ideal signal.
+    x = repeat(symbols, nspui)
+    ideal_signal = x
+    if mod_type == 1:  # Handle duo-binary case.
+        duob_h = array(([0.5] + [0.0] * (nspui - 1)) * 2)
+        ideal_signal = convolve(x, duob_h)[: len(t)]
 
-        # Calculate the channel output.
-        #
-        # Note: We're not using 'self.ideal_signal', because we rely on the system response to
-        #       create the duobinary waveform. We only create it explicitly, above,
-        #       so that we'll have an ideal reference for comparison.
+    # Calculate the channel response, as well as its (hypothetical)
+    # solitary effect on the data, for plotting purposes only.
+    try:
         split_time = clock()
         chnl_h = self.calc_chnl_h()
         _calc_chnl_time = clock() - split_time
+        # Note: We're not using 'self.ideal_signal', because we rely on the system response to
+        #       create the duobinary waveform. We only create it explicitly, above,
+        #       so that we'll have an ideal reference for comparison.
         split_time = clock()
-        chnl_out = convolve(self.x, chnl_h)[: len(t)]
+        chnl_out = convolve(x, chnl_h)[: len(t)]
         _conv_chnl_time = clock() - split_time
         if self.debug:
             self.log(f"Channel calculation time: {_calc_chnl_time}")
             self.log(f"Channel convolution time: {_conv_chnl_time}")
-
         self.channel_perf = nbits * nspb / (clock() - start_time)
-        split_time = clock()
-        self.status = "Running Tx...(sweep %d of %d)" % (sweep_num, num_sweeps)
-    except Exception:
-        self.status = "Exception: channel"
+    except Exception as err:
+        self.status = f"Exception: channel: {err}"
         raise
-
     self.chnl_out = chnl_out
-    self.chnl_out_H = fft(chnl_out)
 
-    # Generate the output from, and the incremental/cumulative impulse/step/frequency responses of, the Tx.
-    try:
-        if self.tx_use_ami:
-            # Note: Within the PyBERT computational environment, we use normalized impulse responses,
-            #       which have units of (V/ts), where 'ts' is the sample interval. However, IBIS-AMI models expect
-            #       units of (V/s). So, we have to scale accordingly, as we transit the boundary between these two worlds.
-            tx_cfg = self._tx_cfg  # Grab the 'AMIParamConfigurator' instance for this model.
-            # Get the model invoked and initialized, except for 'channel_response', which
-            # we need to do several different ways, in order to gather all the data we need.
-            tx_param_dict = tx_cfg.input_ami_params
-            tx_model_init = AMIModelInitializer(tx_param_dict)
-            tx_model_init.sample_interval = ts  # Must be set, before 'channel_response'!
-            # Start with a delta function, to capture the model's impulse response.
-            tx_model_init.channel_response = [1.0 / ts] + [0.0] * (len(chnl_h) - 1)
-            tx_model_init.bit_time = ui
-            tx_model = AMIModel(self.tx_dll_file)
-            tx_model.initialize(tx_model_init)
-            self.log(
-                "Tx IBIS-AMI model initialization results:\nInput parameters: {}\nOutput parameters: {}\nMessage: {}".format(
-                    tx_model.ami_params_in.decode("utf-8"),
-                    tx_model.ami_params_out.decode("utf-8"),
-                    tx_model.msg.decode("utf-8"),
-                )
-            )
-            if tx_cfg.fetch_param_val(["Reserved_Parameters", "Init_Returns_Impulse"]):
-                tx_h = array(tx_model.initOut) * ts
-            elif not tx_cfg.fetch_param_val(["Reserved_Parameters", "GetWave_Exists"]):
-                self.status = "Simulation Error."
-                self.log(
-                    "ERROR: Both 'Init_Returns_Impulse' and 'GetWave_Exists' are False!\n \
-I cannot continue.\nYou will have to select a different model.",
-                    alert=True,
-                )
-                return
-            elif not self.tx_use_getwave:
-                self.status = "Simulation Error."
-                self.log(
-                    "ERROR: You have elected not to use GetWave for a model, which does not return an impulse response!\n \
-I cannot continue.\nPlease, select 'Use GetWave' and try again.",
-                    alert=True,
-                )
-                return
-            if self.tx_use_getwave:
-                try:
-                    tx_s = getwave_step_resp(tx_model)
-                except RuntimeError as err:
-                    self.status = "Tx GetWave() Error."
-                    self.log("ERROR: Never saw a rising step come out of Tx GetWave()!", alert=True)
-                    return
-                tx_h, _ = trim_impulse(diff(tx_s))
-                tx_out, _ = tx_model.getWave(self.x)
-            else:  # Init()-only.
-                tx_out = convolve(tx_h, self.x)
-                tx_s = tx_h.cumsum()
-            self.tx_model = tx_model
+    _check_sim_status()
+    split_time = clock()
+    self.status = "Running Tx..."
+
+    # Calculate Tx output power dissipation.
+    ffe_out = convolve(symbols, ffe)[: len(symbols)]
+    if self.use_ch_file:
+        self.rel_power = mean(ffe_out**2) / self.rs
+    else:
+        self.rel_power = mean(ffe_out**2) / self.Z0
+
+    # Generate the uncorrelated periodic noise. (Assume capacitive coupling.)
+    # Generate the ideal rectangular aggressor waveform.
+    pn_period = 1.0 / pn_freq
+    pn_samps = int(pn_period / Ts + 0.5)
+    pn = zeros(pn_samps)
+    pn[pn_samps // 2:] = pn_mag
+    self.pn_period = pn_period
+    self.pn_samps = pn_samps
+    pn = resize(pn, len(x))
+    # High pass filter it. (Simulating capacitive coupling.)
+    (b, a) = iirfilter(2, gFc / (fs / 2), btype="highpass")
+    pn = lfilter(b, a, pn)[: len(pn)]
+    self.pn = pn
+
+    noise = pn + normal(scale=rn, size=(len(x),))
+    self.noise = noise
+
+    # Tx and Rx modeling are not separable in all cases.
+    # So, we model each of the 4 possible combinations explicitly.
+    # For the purposes of tallying possible combinations,
+    # AMI Init() and PyBERT native are equivalent,
+    # as both rely on convolving w/ impulse responses.
+
+    def get_ctle_h():
+        "Return the impulse response of the PyBERT native CTLE model."
+        if self.use_ctle_file:
+            # FIXME: The new import_channel() implementation breaks this:  # pylint: disable=fixme
+            ctle_h = import_channel(self.ctle_file, ts, f)
+            if max(abs(ctle_h)) < 100.0:  # step response?
+                ctle_h = diff(ctle_h)  # impulse response is derivative of step response.
+            else:
+                ctle_h *= ts  # Normalize to (V/sample)
+            ctle_h.resize(len(t))
+            ctle_H = rfft(ctle_h)  # ToDo: This needs interpolation first.  # pylint: disable=fixme
+            # ctle_H *= sum(ctle_h) / ctle_H[0]
         else:
-            # - Generate the ideal, post-preemphasis signal.
-            # To consider: use 'scipy.interp()'. This is what Mark does, in order to induce jitter in the Tx output.
-            ffe_out = convolve(symbols, ffe)[: len(symbols)]
-            if self.use_ch_file:
-                self.rel_power = mean(ffe_out**2) / self.rs
+            if ctle_enable:
+                _, ctle_H = make_ctle(rx_bw, peak_freq, peak_mag, w)
+                _ctle_h = irfft(ctle_H)
+                krnl = interp1d(t_irfft, _ctle_h, bounds_error=False, fill_value=0)
+                ctle_h = krnl(t)
+                # ctle_h *= t[1] / t_irfft[1]
+                ctle_h *= sum(_ctle_h) / sum(ctle_h)
+                ctle_h, _ = trim_impulse(ctle_h, front_porch=False, min_len=min_len, max_len=max_len)
             else:
-                self.rel_power = mean(ffe_out**2) / self.Z0
-            tx_out = repeat(ffe_out, nspui)  # oversampled output
+                ctle_h = array([1.] + [0. for _ in range(min_len - 1)])
+        return ctle_h
 
-            # - Calculate the responses.
-            # - (The Tx is unique in that the calculated responses aren't used to form the output.
-            #    This is partly due to the out of order nature in which we combine the Tx and channel,
-            #    and partly due to the fact that we're adding noise to the Tx output.)
-            tx_h = array(sum([[x] + list(zeros(nspui - 1)) for x in ffe], []))  # Using sum to concatenate.
-            tx_h.resize(len(chnl_h), refcheck=False)  # "refcheck=False", to get around Tox failure.
-            tx_s = tx_h.cumsum()
-        tx_out.resize(len(t))
-        temp = tx_h.copy()
-        temp.resize(len(t), refcheck=False)
-        tx_H = fft(temp)
-        tx_H *= tx_s[-1] / abs(tx_H[0])
-
-        # - Generate the uncorrelated periodic noise. (Assume capacitive coupling.)
-        #   - Generate the ideal rectangular aggressor waveform.
-        pn_period = 1.0 / pn_freq
-        pn_samps = int(pn_period / Ts + 0.5)
-        pn = zeros(pn_samps)
-        pn[pn_samps // 2 :] = pn_mag
-        pn = resize(pn, len(tx_out))
-        #   - High pass filter it. (Simulating capacitive coupling.)
-        (b, a) = iirfilter(2, gFc / (fs / 2), btype="highpass")
-        pn = lfilter(b, a, pn)[: len(pn)]
-
-        # - Add the uncorrelated periodic and random noise to the Tx output.
-        tx_out += pn
-        tx_out += normal(scale=rn, size=(len(tx_out),))
-
-        # - Convolve w/ channel.
-        tx_out_h = convolve(tx_h, chnl_h)[: len(chnl_h)]
-        temp = tx_out_h.copy()
-        temp.resize(len(t), refcheck=False)
-        tx_out_H = fft(temp)
-        rx_in = convolve(tx_out, chnl_h)[: len(tx_out)]
-
-        self.tx_s = tx_s
-        self.tx_out = tx_out
-        self.rx_in = rx_in
-        self.tx_out_s = tx_out_h.cumsum()
-        self.tx_out_p = self.tx_out_s[nspui:] - self.tx_out_s[:-nspui]
-        self.tx_H = tx_H
-        self.tx_h = tx_h
-        self.tx_out_H = tx_out_H
-        self.tx_out_h = tx_out_h
-
-        self.tx_perf = nbits * nspb / (clock() - split_time)
-        split_time = clock()
-        self.status = "Running CTLE...(sweep %d of %d)" % (sweep_num, num_sweeps)
-    except Exception:
-        self.status = "Exception: Tx"
+    try:
+        if self.tx_use_ami and self.tx_use_getwave:
+            tx_out, _, tx_h, tx_out_h, msg = run_ami_model(
+                self.tx_dll_file, self._tx_cfg, True, ui, ts, chnl_h, x)
+            self.log(f"Tx IBIS-AMI model initialization results:\n{msg}")
+            rx_in = convolve(tx_out + noise, chnl_h)[:len(tx_out)]
+            # Calculate the remaining responses from the impulse responses.
+            tx_s, tx_p, tx_H = calc_resps(t, tx_h, ui, f)
+            tx_out_s, tx_out_p, tx_out_H = calc_resps(t, tx_out_h, ui, f)
+            self.tx_perf = nbits * nspb / (clock() - split_time)
+            split_time = clock()
+            self.status = "Running CTLE..."
+            if self.rx_use_ami and self.rx_use_getwave:
+                ctle_out, _, ctle_h, ctle_out_h, msg = run_ami_model(
+                    self.rx_dll_file, self._rx_cfg, True, ui, ts, tx_out_h, convolve(tx_out, chnl_h))
+                self.log(f"Rx IBIS-AMI model initialization results:\n{msg}")
+            else:  # Rx is either AMI_Init() or PyBERT native.
+                if self.rx_use_ami:  # Rx Init()
+                    _, _, ctle_h, ctle_out_h, msg = run_ami_model(
+                        self.rx_dll_file, self._rx_cfg, False, ui, ts, chnl_h, tx_out)
+                    self.log(f"Rx IBIS-AMI model initialization results:\n{msg}")
+                    ctle_out = convolve(tx_out, ctle_out_h)[:len(tx_out)]
+                else:                # PyBERT native Rx
+                    ctle_h = get_ctle_h()
+                    ctle_out_h = convolve(ctle_h, tx_out_h)[:len(ctle_h)]
+                    ctle_out = convolve(tx_out, convolve(ctle_h, chnl_h))[:len(tx_out)]
+        else:  # Tx is either AMI_Init() or PyBERT native.
+            if self.tx_use_ami:  # Tx is AMI_Init().
+                rx_in, _, tx_h, tx_out_h, msg = run_ami_model(
+                    self.tx_dll_file, self._tx_cfg, False, ui, ts, chnl_h, x)
+                self.log(f"Tx IBIS-AMI model initialization results:\n{msg}")
+                rx_in += noise
+            else:                # Tx is PyBERT native.
+                # Using `sum` to concatenate:
+                tx_h = array(sum([[x] + list(zeros(nspui - 1)) for x in ffe], []))
+                tx_h.resize(len(chnl_h), refcheck=False)  # "refcheck=False", to get around Tox failure.
+                tx_out_h = convolve(tx_h, chnl_h)[: len(chnl_h)]
+                rx_in = convolve(x, tx_out_h)[:len(x)] + noise
+            # Calculate the remaining responses from the impulse responses.
+            tx_s, tx_p, tx_H = calc_resps(t, tx_h, ui, f)
+            tx_out_s, tx_out_p, tx_out_H = calc_resps(t, tx_out_h, ui, f)
+            self.tx_perf = nbits * nspb / (clock() - split_time)
+            split_time = clock()
+            self.status = "Running CTLE..."
+            if self.rx_use_ami and self.rx_use_getwave:
+                ctle_out, _, ctle_h, ctle_out_h, msg = run_ami_model(
+                    self.rx_dll_file, self._rx_cfg, True, ui, ts, tx_out_h, rx_in)
+                self.log(f"Rx IBIS-AMI model initialization results:\n{msg}")
+            else:  # Rx is either AMI_Init() or PyBERT native.
+                if self.rx_use_ami:  # Rx Init()
+                    ctle_out, _, ctle_h, ctle_out_h, msg = run_ami_model(
+                        self.rx_dll_file, self._rx_cfg, False, ui, ts, tx_out_h, x)
+                    self.log(f"Rx IBIS-AMI model initialization results:\n{msg}")
+                    ctle_out += noise
+                else:                # PyBERT native Rx
+                    if ctle_enable:
+                        ctle_h = get_ctle_h()
+                        ctle_out_h = convolve(tx_out_h, ctle_h)[:len(tx_out_h)]
+                        ctle_out = convolve(x + noise, ctle_out_h)[:len(x)]
+                    else:
+                        ctle_h = array([1.] + [0.] * (min_len - 1))
+                        ctle_out_h = tx_out_h
+                        ctle_out = rx_in
+    except Exception as err:
+        self.status = f"Exception: {err}"
         raise
 
-    # Generate the output from, and the incremental/cumulative impulse/step/frequency responses of, the CTLE.
-    try:
-        if self.rx_use_ami:
-            rx_cfg = self._rx_cfg  # Grab the 'AMIParamConfigurator' instance for this model.
-            # Get the model invoked and initialized, except for 'channel_response', which
-            # we need to do several different ways, in order to gather all the data we need.
-            rx_param_dict = rx_cfg.input_ami_params
-            rx_model_init = AMIModelInitializer(rx_param_dict)
-            rx_model_init.sample_interval = ts  # Must be set, before 'channel_response'!
-            rx_model_init.channel_response = tx_out_h / ts
-            rx_model_init.bit_time = ui
-            rx_model = AMIModel(self.rx_dll_file)
-            rx_model.initialize(rx_model_init)
-            self.log(
-                "Rx IBIS-AMI model initialization results:\nInput parameters: {}\nMessage: {}\nOutput parameters: {}".format(
-                    rx_model.ami_params_in.decode("utf-8"),
-                    rx_model.msg.decode("utf-8"),
-                    rx_model.ami_params_out.decode("utf-8"),
-                )
-            )
-            if rx_cfg.fetch_param_val(["Reserved_Parameters", "Init_Returns_Impulse"]):
-                ctle_out_h = array(rx_model.initOut) * ts
-            elif not rx_cfg.fetch_param_val(["Reserved_Parameters", "GetWave_Exists"]):
-                self.status = "Simulation Error."
-                self.log(
-                    "ERROR: Both 'Init_Returns_Impulse' and 'GetWave_Exists' are False!\n \
-I cannot continue.\nYou will have to select a different model.",
-                    alert=True,
-                )
-                return
-            elif not self.rx_use_getwave:
-                self.status = "Simulation Error."
-                self.log(
-                    "ERROR: You have elected not to use GetWave for a model, which does not return an impulse response!\n \
-I cannot continue.\nPlease, select 'Use GetWave' and try again.",
-                    alert=True,
-                )
-                return
-            if self.rx_use_getwave:
-                try:
-                    ctle_s = getwave_step_resp(rx_model)
-                except RuntimeError as err:
-                    self.status = "Rx GetWave() Error."
-                    self.log("ERROR: Never saw a rising step come out of Rx GetWave()!", alert=True)
-                    return
-                ctle_h = diff(ctle_s)
-                temp = ctle_h.copy()
-                temp.resize(len(t))
-                ctle_H = fft(temp)
-                ctle_h.resize(len(chnl_h))
-                ctle_out_h = convolve(ctle_h, tx_out_h)[: len(chnl_h)]
-            else:  # Init() only.
-                ctle_out_h_padded = pad(
-                    ctle_out_h,
-                    (nspb, len(rx_in) - nspb - len(ctle_out_h)),
-                    "linear_ramp",
-                    end_values=(0.0, 0.0),
-                )
-                tx_out_h_padded = pad(
-                    tx_out_h,
-                    (nspb, len(rx_in) - nspb - len(tx_out_h)),
-                    "linear_ramp",
-                    end_values=(0.0, 0.0),
-                )
-                ctle_H = fft(ctle_out_h_padded) / fft(tx_out_h_padded)  # ToDo: I think this is wrong.
-                ctle_h = irfft(ctle_H)  # I shouldn't be sending the output of `fft()` into `irfft()`, should I?
-                ctle_h.resize(len(chnl_h))
-            ctle_s = ctle_h.cumsum()
-            ctle_out = convolve(rx_in, ctle_h)
-        else:
-            if self.use_ctle_file:
-                # FIXME: The new import_channel() implementation breaks this:
-                ctle_h = import_channel(self.ctle_file, ts, self.f)
-                if max(abs(ctle_h)) < 100.0:  # step response?
-                    ctle_h = diff(ctle_h)  # impulse response is derivative of step response.
-                else:
-                    ctle_h *= ts  # Normalize to (V/sample)
-                ctle_h.resize(len(t))
-                ctle_H = fft(ctle_h)
-                ctle_H *= sum(ctle_h) / ctle_H[0]
-            else:
-                _, ctle_H = make_ctle(rx_bw, peak_freq, peak_mag, w, ctle_mode, ctle_offset)
-                ctle_h = irfft(ctle_H)
-            ctle_h.resize(len(chnl_h), refcheck=False)
-            ctle_out = convolve(rx_in, ctle_h)
-            ctle_out -= mean(ctle_out)  # Force zero mean.
-            if self.ctle_mode == "AGC":  # Automatic gain control engaged?
-                ctle_out *= 2.0 * decision_scaler / ctle_out.ptp()
-            ctle_s = ctle_h.cumsum()
-            ctle_out_h = convolve(tx_out_h, ctle_h)[: len(tx_out_h)]
-        ctle_out.resize(len(t), refcheck=False)
-        ctle_out_h_main_lobe = where(ctle_out_h >= max(ctle_out_h) / 2.0)[0]
-        if ctle_out_h_main_lobe.size:
-            conv_dly_ix = ctle_out_h_main_lobe[0]
-        else:
-            conv_dly_ix = int(self.chnl_dly // Ts)
-        conv_dly = t[conv_dly_ix]  # Keep this line only.
-        ctle_out_s = ctle_out_h.cumsum()
-        temp = ctle_out_h.copy()
-        temp.resize(len(t), refcheck=False)
-        ctle_out_H = fft(temp)
-        # - Store local variables to class instance.
-        # Consider changing this; it could be sensitive to insufficient "front porch" in the CTLE output step response.
-        self.ctle_out_p = ctle_out_s[nspui:] - ctle_out_s[:-nspui]
-        self.ctle_H = ctle_H
-        self.ctle_h = ctle_h
-        self.ctle_s = ctle_s
-        self.ctle_out_H = ctle_out_H
-        self.ctle_out_h = ctle_out_h
-        self.ctle_out_s = ctle_out_s
-        self.ctle_out = ctle_out
-        self.conv_dly = conv_dly
-        self.conv_dly_ix = conv_dly_ix
+    # Calculate the remaining responses from the impulse responses.
+    ctle_s, ctle_p, ctle_H = calc_resps(t, ctle_h, ui, f)
+    ctle_out_s, ctle_out_p, ctle_out_H = calc_resps(t, ctle_out_h, ui, f)
+
+    # Calculate convolutional delay.
+    ctle_out.resize(len(t), refcheck=False)
+    ctle_out_h_main_lobe = where(ctle_out_h >= max(ctle_out_h) / 2.0)[0]
+    if ctle_out_h_main_lobe.size:
+        conv_dly_ix = ctle_out_h_main_lobe[0]
+    else:
+        conv_dly_ix = int(self.chnl_dly // Ts)
+    conv_dly = t[conv_dly_ix]
 
-        self.ctle_perf = nbits * nspb / (clock() - split_time)
-        split_time = clock()
-        self.status = "Running DFE/CDR...(sweep %d of %d)" % (sweep_num, num_sweeps)
-    except Exception:
-        self.status = "Exception: Rx"
-        raise
+    # Stash needed intermediate results, as instance variables.
+    self.tx_h = tx_h
+    self.tx_s = tx_s
+    self.tx_p = tx_p
+    self.tx_H = tx_H
+    self.tx_out_h = tx_out_h
+    self.tx_out_s = tx_out_s
+    self.tx_out_p = tx_out_p
+    self.tx_out_H = tx_out_H
+    self.ideal_signal = ideal_signal
+    self.rx_in = rx_in
+    self.ctle_h = ctle_h
+    self.ctle_s = ctle_s
+    self.ctle_p = ctle_p
+    self.ctle_H = ctle_H
+    self.ctle_out_h = ctle_out_h
+    self.ctle_out_s = ctle_out_s
+    self.ctle_out_p = ctle_out_p
+    self.ctle_out_H = ctle_out_H
+    self.ctle_out = ctle_out
+    self.conv_dly = conv_dly
+    self.conv_dly_ix = conv_dly_ix
+
+    self.ctle_perf = nbits * nspb / (clock() - split_time)
+    split_time = clock()
+    self.status = "Running DFE/CDR..."
 
-    # Generate the output from, and the incremental/cumulative impulse/step/frequency responses of, the DFE.
+    _check_sim_status()
+
+    # DFE output and incremental/cumulative responses.
     try:
-        if self.use_dfe:
-            dfe = DFE(
-                n_taps,
-                gain,
-                delta_t,
-                alpha,
-                ui,
-                nspui,
-                decision_scaler,
-                mod_type,
-                n_ave=n_ave,
-                n_lock_ave=n_lock_ave,
-                rel_lock_tol=rel_lock_tol,
-                lock_sustain=lock_sustain,
-                bandwidth=bandwidth,
-                ideal=self.sum_ideal,
-            )
+        if any(tap.enabled for tap in dfe_tap_tuners):
+            _gain = gain
+            _ideal = self.sum_ideal
+            _n_taps = len(dfe_tap_tuners)
         else:
-            dfe = DFE(
-                n_taps,
-                0.0,
-                delta_t,
-                alpha,
-                ui,
-                nspui,
-                decision_scaler,
-                mod_type,
-                n_ave=n_ave,
-                n_lock_ave=n_lock_ave,
-                rel_lock_tol=rel_lock_tol,
-                lock_sustain=lock_sustain,
-                bandwidth=bandwidth,
-                ideal=True,
-            )
-        (dfe_out, tap_weights, ui_ests, clocks, lockeds, clock_times, bits_out) = dfe.run(t, ctle_out)
+            _gain = 0.0
+            _ideal = True
+            _n_taps = 0
+        limits = []
+        for tuner in self.dfe_tap_tuners:
+            if tuner.enabled:
+                limits.append((tuner.min_val, tuner.max_val))
+            else:
+                limits.append((0., 0.))
+        dfe = DFE(_n_taps, _gain, delta_t, alpha, ui, nspui, decision_scaler, mod_type,
+                  n_ave=n_ave, n_lock_ave=n_lock_ave, rel_lock_tol=rel_lock_tol,
+                  lock_sustain=lock_sustain, bandwidth=bandwidth, ideal=_ideal,
+                  limits=limits)
+        (dfe_out, tap_weights, ui_ests, clocks,
+            lockeds, clock_times, bits_out) = dfe.run(t, ctle_out)
         dfe_out = array(dfe_out)
         dfe_out.resize(len(t))
         bits_out = array(bits_out)
+        start_ix = len(bits_out) - eye_bits
+        assert start_ix >= 0, "`start_ix` is negative!"
+        end_ix = len(bits_out)
         auto_corr = (
-            1.0
-            * correlate(bits_out[(nbits - eye_bits) :], bits[(nbits - eye_bits) :], mode="same")
-            / sum(bits[(nbits - eye_bits) :])
+            1.0 * correlate(bits_out[start_ix: end_ix], bits[start_ix: end_ix], mode="same") /  # noqa: W504
+            sum(bits[start_ix: end_ix])
         )
-        auto_corr = auto_corr[len(auto_corr) // 2 :]
+        auto_corr = auto_corr[len(auto_corr) // 2:]
         self.auto_corr = auto_corr
         bit_dly = where(auto_corr == max(auto_corr))[0][0]
-        bits_ref = bits[(nbits - eye_bits) :]
-        bits_tst = bits_out[(nbits + bit_dly - eye_bits) :]
+        bits_ref = bits[(nbits - eye_bits):]
+        bits_tst = bits_out[(nbits + bit_dly - eye_bits):]
         if len(bits_ref) > len(bits_tst):
             bits_ref = bits_ref[: len(bits_tst)]
         elif len(bits_tst) > len(bits_ref):
             bits_tst = bits_tst[: len(bits_ref)]
         bit_errs = where(bits_tst ^ bits_ref)[0]
         self.bit_errs = len(bit_errs)
 
-        dfe_h = array([1.0] + list(zeros(nspb - 1)) + sum([[-x] + list(zeros(nspb - 1)) for x in tap_weights[-1]], []))
+        dfe_h = array(
+            [1.0] + list(zeros(nspui - 1)) +  # noqa: W504
+            sum([[-x] + list(zeros(nspui - 1)) for x in tap_weights[-1]], []))  # sum as concat
         dfe_h.resize(len(ctle_out_h), refcheck=False)
-        temp = dfe_h.copy()
-        temp.resize(len(t), refcheck=False)
-        dfe_H = fft(temp)
-        self.dfe_s = dfe_h.cumsum()
-        dfe_out_H = ctle_out_H * dfe_H
         dfe_out_h = convolve(ctle_out_h, dfe_h)[: len(ctle_out_h)]
-        dfe_out_s = dfe_out_h.cumsum()
-        self.dfe_out_p = dfe_out_s - pad(dfe_out_s[:-nspui], (nspui, 0), "constant", constant_values=(0, 0))
-        self.dfe_H = dfe_H
+
+        # Calculate the remaining responses from the impulse responses.
+        dfe_s, dfe_p, dfe_H = calc_resps(t, dfe_h, ui, f)
+        dfe_out_s, dfe_out_p, dfe_out_H = calc_resps(t, dfe_out_h, ui, f)
+
         self.dfe_h = dfe_h
-        self.dfe_out_H = dfe_out_H
+        self.dfe_s = dfe_s
+        self.dfe_p = dfe_p
+        self.dfe_H = dfe_H
         self.dfe_out_h = dfe_out_h
         self.dfe_out_s = dfe_out_s
+        self.dfe_out_p = dfe_out_p
+        self.dfe_out_H = dfe_out_H
         self.dfe_out = dfe_out
+        self.lockeds = lockeds
 
         self.dfe_perf = nbits * nspb / (clock() - split_time)
         split_time = clock()
-        self.status = "Analyzing jitter...(sweep %d of %d)" % (sweep_num, num_sweeps)
+        self.status = "Analyzing jitter..."
     except Exception:
         self.status = "Exception: DFE"
+        print(f"len(bits_out): {len(bits_out)}\nnbits: {nbits}\neye_bits: {eye_bits}")
+        print(f"len(t): {len(t)}, len(ctle_out): {len(ctle_out)}")
         raise
 
+    _check_sim_status()
+
     # Save local variables to class instance for state preservation, performing unit conversion where necessary.
     self.adaptation = tap_weights
     self.ui_ests = array(ui_ests) * 1.0e12  # (ps)
     self.clocks = clocks
     self.lockeds = lockeds
     self.clock_times = clock_times
 
@@ -551,157 +443,203 @@
     self.f_MHz_dfe = array([])
     self.jitter_rejection_ratio = array([])
 
     # The pattern length must be doubled in the duo-binary and PAM-4 cases anyway, because:
     #  - in the duo-binary case, the XOR pre-coding can invert every other pattern rep., and
     #  - in the PAM-4 case, the bits are taken in pairs to form the symbols and we start w/ an odd # of bits.
     # So, while it isn't strictly necessary, doubling it in the NRZ case as well provides a certain consistency.
+    pattern_len = (pow(2, max(pattern)) - 1) * 2
+    len_x_m1 = len(x) - 1
+    xing_min_t = (nui - eye_uis) * ui
+
+    def eye_xings(xings, ofst=0):
+        """
+        Return crossings from that portion of the signal used to generate the eye.
+
+        Args:
+            xings([float]): List of crossings.
+
+        KeywordArgs:
+            ofst(float): Time offset to be subtracted from all crossings.
+
+        Returns:
+            [float]: Selected crossings, offset and eye-start corrected.
+        """
+        _xings = array(xings) - ofst
+        return _xings[where(_xings > xing_min_t)] - xing_min_t
+
     try:
-        pattern_len = (pow(2, max(pattern)) - 1) * 2
+        # - ideal
+        ideal_xings = find_crossings(t, ideal_signal, decision_scaler, mod_type=mod_type)
+        self.ideal_xings = ideal_xings
+        ideal_xings_jit = eye_xings(ideal_xings)
 
         # - channel output
-        len_x_m1 = len(x) - 1
-        actual_xings = find_crossings(t, chnl_out, decision_scaler, mod_type=mod_type)
         ofst = (argmax(sig.correlate(chnl_out, x)) - len_x_m1) * Ts
-        actual_xings -= ofst
+        actual_xings = find_crossings(t, chnl_out, decision_scaler, mod_type=mod_type)
+        actual_xings_jit = eye_xings(actual_xings, ofst)
         (
-            _,
+            tie,
             t_jitter,
             isi,
             dcd,
             pj,
             rj,
-            _,
+            pjDD,
+            rjDD,
+            tie_ind,
             thresh,
             jitter_spectrum,
             jitter_ind_spectrum,
             spectrum_freqs,
             hist,
             hist_synth,
             bin_centers,
-        ) = calc_jitter(ui, nui, pattern_len, ideal_xings, actual_xings, rel_thresh)
-        self.t_jitter = t_jitter
-        self.isi_chnl = isi
-        self.dcd_chnl = dcd
-        self.pj_chnl = pj
-        self.rj_chnl = rj
+        ) = calc_jitter(ui, eye_uis, pattern_len, ideal_xings_jit, actual_xings_jit, rel_thresh)
+        self.t_jitter  = t_jitter
+        self.isi_chnl  = isi
+        self.dcd_chnl  = dcd
+        self.pj_chnl   = pj
+        self.rj_chnl   = rj
+        self.pjDD_chnl = pjDD
+        self.rjDD_chnl = rjDD
         self.thresh_chnl = thresh
         self.jitter_chnl = hist
         self.jitter_ext_chnl = hist_synth
         self.jitter_bins = bin_centers
         self.jitter_spectrum_chnl = jitter_spectrum
         self.jitter_ind_spectrum_chnl = jitter_ind_spectrum
         self.f_MHz = array(spectrum_freqs) * 1.0e-6
+        self.ofst_chnl = ofst
+        self.tie_chnl = tie
+        self.tie_ind_chnl = tie_ind
 
         # - Tx output
-        actual_xings = find_crossings(t, rx_in, decision_scaler, mod_type=mod_type)
         ofst = (argmax(sig.correlate(rx_in, x)) - len_x_m1) * Ts
-        actual_xings -= ofst
+        actual_xings = find_crossings(t, rx_in, decision_scaler, mod_type=mod_type)
+        actual_xings_jit = eye_xings(actual_xings, ofst)
         (
-            _,
+            tie,
             t_jitter,
             isi,
             dcd,
             pj,
             rj,
-            _,
+            pjDD,
+            rjDD,
+            tie_ind,
             thresh,
             jitter_spectrum,
             jitter_ind_spectrum,
             spectrum_freqs,
             hist,
             hist_synth,
             bin_centers,
-        ) = calc_jitter(ui, nui, pattern_len, ideal_xings, actual_xings, rel_thresh)
-        self.isi_tx = isi
-        self.dcd_tx = dcd
-        self.pj_tx = pj
-        self.rj_tx = rj
+        ) = calc_jitter(ui, eye_uis, pattern_len, ideal_xings_jit, actual_xings_jit, rel_thresh, dbg_obj=self)
+        self.isi_tx  = isi
+        self.dcd_tx  = dcd
+        self.pj_tx   = pj
+        self.rj_tx   = rj
+        self.pjDD_tx = pjDD
+        self.rjDD_tx = rjDD
         self.thresh_tx = thresh
         self.jitter_tx = hist
         self.jitter_ext_tx = hist_synth
+        self.jitter_centers_tx = bin_centers
         self.jitter_spectrum_tx = jitter_spectrum
         self.jitter_ind_spectrum_tx = jitter_ind_spectrum
+        self.jitter_freqs_tx = spectrum_freqs
+        self.t_jitter_tx = t_jitter
+        self.tie_tx = tie
+        self.tie_ind_tx = tie_ind
 
         # - CTLE output
-        actual_xings = find_crossings(t, ctle_out, decision_scaler, mod_type=mod_type)
         ofst = (argmax(sig.correlate(ctle_out, x)) - len_x_m1) * Ts
-        actual_xings -= ofst
+        actual_xings = find_crossings(t, ctle_out, decision_scaler, mod_type=mod_type)
+        actual_xings_jit = eye_xings(actual_xings, ofst)
         (
-            jitter,
+            tie,
             t_jitter,
             isi,
             dcd,
             pj,
             rj,
-            jitter_ext,
+            pjDD,
+            rjDD,
+            tie_ind,
             thresh,
             jitter_spectrum,
             jitter_ind_spectrum,
             spectrum_freqs,
             hist,
             hist_synth,
             bin_centers,
-        ) = calc_jitter(ui, nui, pattern_len, ideal_xings, actual_xings, rel_thresh)
-        self.isi_ctle = isi
-        self.dcd_ctle = dcd
-        self.pj_ctle = pj
-        self.rj_ctle = rj
+        ) = calc_jitter(ui, eye_uis, pattern_len, ideal_xings_jit, actual_xings_jit, rel_thresh)
+        self.isi_ctle  = isi
+        self.dcd_ctle  = dcd
+        self.pj_ctle   = pj
+        self.rj_ctle   = rj
+        self.pjDD_ctle = pjDD
+        self.rjDD_ctle = rjDD
         self.thresh_ctle = thresh
         self.jitter_ctle = hist
         self.jitter_ext_ctle = hist_synth
         self.jitter_spectrum_ctle = jitter_spectrum
         self.jitter_ind_spectrum_ctle = jitter_ind_spectrum
+        self.tie_ctle = tie
+        self.tie_ind_ctle = tie_ind
 
         # - DFE output
-        ignore_until = (nui - eye_uis) * ui
-        ideal_xings = array(list(filter(lambda x: x >= ignore_until, ideal_xings)))
-        ideal_xings -= ignore_until
-        actual_xings = find_crossings(t, dfe_out, decision_scaler, mod_type=mod_type)
         ofst = (argmax(sig.correlate(dfe_out, x)) - len_x_m1) * Ts
-        actual_xings -= ofst
-        actual_xings = array(list(filter(lambda x: x >= ignore_until, actual_xings)))
-        actual_xings -= ignore_until
+        actual_xings = find_crossings(t, dfe_out, decision_scaler, mod_type=mod_type)
+        actual_xings_jit = eye_xings(actual_xings, ofst)
         (
-            jitter,
+            tie,
             t_jitter,
             isi,
             dcd,
             pj,
             rj,
-            jitter_ext,
+            pjDD,
+            rjDD,
+            tie_ind,
             thresh,
             jitter_spectrum,
             jitter_ind_spectrum,
             spectrum_freqs,
             hist,
             hist_synth,
             bin_centers,
-        ) = calc_jitter(ui, eye_uis, pattern_len, ideal_xings, actual_xings, rel_thresh)
-        self.isi_dfe = isi
-        self.dcd_dfe = dcd
-        self.pj_dfe = pj
-        self.rj_dfe = rj
+        ) = calc_jitter(ui, eye_uis, pattern_len, ideal_xings_jit, actual_xings_jit, rel_thresh)
+        self.isi_dfe  = isi
+        self.dcd_dfe  = dcd
+        self.pj_dfe   = pj
+        self.rj_dfe   = rj
+        self.pjDD_dfe = pjDD
+        self.rjDD_dfe = rjDD
         self.thresh_dfe = thresh
         self.jitter_dfe = hist
         self.jitter_ext_dfe = hist_synth
         self.jitter_spectrum_dfe = jitter_spectrum
         self.jitter_ind_spectrum_dfe = jitter_ind_spectrum
+        self.tie_dfe = tie
+        self.tie_ind_dfe = tie_ind
         self.f_MHz_dfe = array(spectrum_freqs) * 1.0e-6
         dfe_spec = self.jitter_spectrum_dfe
         self.jitter_rejection_ratio = zeros(len(dfe_spec))
 
         self.jitter_perf = nbits * nspb / (clock() - split_time)
         self.total_perf = nbits * nspb / (clock() - start_time)
         split_time = clock()
-        self.status = "Updating plots...(sweep %d of %d)" % (sweep_num, num_sweeps)
+        self.status = "Updating plots..."
     except Exception:
         self.status = "Exception: jitter"
         raise
 
+    _check_sim_status()
     # Update plots.
     try:
         if update_plots:
             update_results(self)
             if not initial_run:
                 update_eyes(self)
 
@@ -709,14 +647,15 @@
         self.status = "Ready."
     except Exception:
         self.status = "Exception: plotting"
         raise
 
 
 # Plot updating
+# pylint: disable=too-many-locals,protected-access,too-many-statements
 def update_results(self):
     """Updates all plot data used by GUI.
 
     Args:
         self(PyBERT): Reference to an instance of the *PyBERT* class.
     """
 
@@ -726,80 +665,65 @@
     eye_uis = self.eye_uis
     num_ui = self.nui
     clock_times = self.clock_times
     f = self.f
     t = self.t
     t_ns = self.t_ns
     t_ns_chnl = self.t_ns_chnl
-    n_taps = self.n_taps
+    t_irfft = self.t_irfft
 
     Ts = t[1]
     ignore_until = (num_ui - eye_uis) * ui
     ignore_samps = (num_ui - eye_uis) * samps_per_ui
 
     # Misc.
-    f_GHz = f[: len(f) // 2] / 1.0e9
+    f_GHz = f / 1.0e9
     len_f_GHz = len(f_GHz)
     len_t = len(t_ns)
     self.plotdata.set_data("f_GHz", f_GHz[1:])
-    self.plotdata.set_data("t_ns", t_ns)
     self.plotdata.set_data("t_ns_chnl", t_ns_chnl)
+    self.plotdata.set_data("t_ns_irfft", t_irfft * 1e9)
+    if len_t > 1000:  # to prevent Chaco plotting error with too much data
+        t_ns_plot = linspace(0, t_ns[-1], 1000)
+    else:
+        t_ns_plot = t_ns
+    self.plotdata.set_data("t_ns", t_ns_plot)
 
     # DFE.
     tap_weights = transpose(array(self.adaptation))
-    i = 1
-    for tap_weight in tap_weights:
-        self.plotdata.set_data("tap%d_weights" % i, tap_weight)
-        i += 1
-    self.plotdata.set_data("tap_weight_index", list(range(len(tap_weight))))
-    if self._old_n_taps != n_taps:
-        new_plot = Plot(
-            self.plotdata,
-            auto_colors=["red", "orange", "yellow", "green", "blue", "purple"],
-            padding_left=75,
-        )
-        for i in range(self.n_taps):
-            new_plot.plot(
-                ("tap_weight_index", "tap%d_weights" % (i + 1)),
-                type="line",
-                color="auto",
-                name="tap%d" % (i + 1),
-            )
-        new_plot.title = "DFE Adaptation"
-        new_plot.tools.append(PanTool(new_plot, constrain=True, constrain_key=None, constrain_direction="x"))
-        zoom9 = ZoomTool(new_plot, tool_mode="range", axis="index", always_on=False)
-        new_plot.overlays.append(zoom9)
-        new_plot.legend.visible = True
-        new_plot.legend.align = "ul"
-        self.plots_dfe.remove(self._dfe_plot)
-        self.plots_dfe.insert(1, new_plot)
-        self._dfe_plot = new_plot
-        self._old_n_taps = n_taps
+    for k, tap_weight in enumerate(tap_weights):  # pylint: disable=undefined-loop-variable
+        self.plotdata.set_data(f"tap{k + 1}_weights", tap_weight)
+    self.plotdata.set_data("tap_weight_index", list(range(len(tap_weight))))  # pylint: disable=undefined-loop-variable
 
     clock_pers = diff(clock_times)
     lockedsTrue = where(self.lockeds)[0]
     if lockedsTrue.any():
         start_t = t[lockedsTrue[0]]
     else:
         start_t = 0
     start_ix = where(array(clock_times) > start_t)[0][0]
     (bin_counts, bin_edges) = histogram(clock_pers[start_ix:], bins=100)
     bin_centers = (bin_edges[:-1] + bin_edges[1:]) / 2.0
-    clock_spec = fft(clock_pers[start_ix:])
+    clock_spec = rfft(clock_pers[start_ix:])
     clock_spec = abs(clock_spec[: len(clock_spec) // 2])
     spec_freqs = arange(len(clock_spec)) / (2.0 * len(clock_spec))  # In this case, fNyquist = half the bit rate.
     clock_spec /= clock_spec[1:].mean()  # Normalize the mean non-d.c. value to 0 dB.
     self.plotdata.set_data("clk_per_hist_bins", bin_centers * 1.0e12)  # (ps)
     self.plotdata.set_data("clk_per_hist_vals", bin_counts)
     self.plotdata.set_data("clk_spec", 10.0 * safe_log10(clock_spec[1:]))  # Omit the d.c. value.
     self.plotdata.set_data("clk_freqs", spec_freqs[1:])
     self.plotdata.set_data("dfe_out", self.dfe_out)
-    self.plotdata.set_data("ui_ests", self.ui_ests)
     self.plotdata.set_data("clocks", self.clocks)
     self.plotdata.set_data("lockeds", self.lockeds)
+    if len_t > 1000:  # to prevent Chaco plotting error with too much data
+        krnl = interp1d(t_ns, self.ui_ests)
+        ui_ests_plot = krnl(t_ns_plot)
+    else:
+        ui_ests_plot = self.ui_ests
+    self.plotdata.set_data("ui_ests", ui_ests_plot)
 
     # Impulse responses
     self.plotdata.set_data("chnl_h", self.chnl_h * 1.0e-9 / Ts)  # Re-normalize to (V/ns), for plotting.
     self.plotdata.set_data("tx_h", self.tx_h * 1.0e-9 / Ts)
     self.plotdata.set_data("tx_out_h", self.tx_out_h * 1.0e-9 / Ts)
     self.plotdata.set_data("ctle_h", self.ctle_h * 1.0e-9 / Ts)
     self.plotdata.set_data("ctle_out_h", self.ctle_out_h * 1.0e-9 / Ts)
@@ -817,123 +741,128 @@
 
     # Pulse responses
     self.plotdata.set_data("chnl_p", self.chnl_p)
     self.plotdata.set_data("tx_out_p", self.tx_out_p)
     self.plotdata.set_data("ctle_out_p", self.ctle_out_p)
     self.plotdata.set_data("dfe_out_p", self.dfe_out_p)
 
-    # Outputs
-    self.plotdata.set_data("ideal_signal", self.ideal_signal[:len_t])
-    self.plotdata.set_data("chnl_out", self.chnl_out[:len_t])
-    self.plotdata.set_data("tx_out", self.rx_in[:len_t])
-    self.plotdata.set_data("ctle_out", self.ctle_out[:len_t])
-    self.plotdata.set_data("dfe_out", self.dfe_out[:len_t])
-
     # Frequency responses
+    self.plotdata.set_data("chnl_H_raw", 20.0 * safe_log10(abs(self.chnl_H_raw[1:len_f_GHz])))
     self.plotdata.set_data("chnl_H", 20.0 * safe_log10(abs(self.chnl_H[1:len_f_GHz])))
     self.plotdata.set_data("chnl_trimmed_H", 20.0 * safe_log10(abs(self.chnl_trimmed_H[1:len_f_GHz])))
-    self.plotdata.set_data("tx_H", 20.0 * safe_log10(abs(self.tx_H[1:len_f_GHz])))
+    self.plotdata.set_data("tx_H", 20.0 * safe_log10(abs(self.tx_H[1:])))
     self.plotdata.set_data("tx_out_H", 20.0 * safe_log10(abs(self.tx_out_H[1:len_f_GHz])))
     self.plotdata.set_data("ctle_H", 20.0 * safe_log10(abs(self.ctle_H[1:len_f_GHz])))
     self.plotdata.set_data("ctle_out_H", 20.0 * safe_log10(abs(self.ctle_out_H[1:len_f_GHz])))
     self.plotdata.set_data("dfe_H", 20.0 * safe_log10(abs(self.dfe_H[1:len_f_GHz])))
     self.plotdata.set_data("dfe_out_H", 20.0 * safe_log10(abs(self.dfe_out_H[1:len_f_GHz])))
 
+    # Outputs
+    ideal_signal = self.ideal_signal[:len_t]
+    chnl_out = self.chnl_out[:len_t]
+    rx_in = self.rx_in[:len_t]
+    ctle_out = self.ctle_out[:len_t]
+    dfe_out = self.dfe_out[:len_t]
+    lockeds = self.lockeds[:len_t]
+    if len_t > 1000:  # to prevent Chaco plotting error with too much data
+        krnl = interp1d(t_ns, ideal_signal)
+        ideal_signal_plot = krnl(t_ns_plot)
+        krnl = interp1d(t_ns, chnl_out)
+        chnl_out_plot = krnl(t_ns_plot)
+        krnl = interp1d(t_ns, rx_in)
+        rx_in_plot = krnl(t_ns_plot)
+        krnl = interp1d(t_ns, ctle_out)
+        ctle_out_plot = krnl(t_ns_plot)
+        krnl = interp1d(t_ns, dfe_out)
+        dfe_out_plot = krnl(t_ns_plot)
+        krnl = interp1d(t_ns, lockeds)
+        lockeds_plot = krnl(t_ns_plot)
+    else:
+        ideal_signal_plot = ideal_signal
+        chnl_out_plot = chnl_out
+        rx_in_plot = rx_in
+        ctle_out_plot = ctle_out
+        dfe_out_plot = dfe_out
+        lockeds_plot = lockeds
+    self.plotdata.set_data("ideal_signal", ideal_signal_plot)
+    self.plotdata.set_data("chnl_out", chnl_out_plot)
+    self.plotdata.set_data("rx_in", rx_in_plot)
+    self.plotdata.set_data("ctle_out", ctle_out_plot)
+    self.plotdata.set_data("dfe_out", dfe_out_plot)
+    self.plotdata.set_data("dbg_out", lockeds_plot)
+
     # Jitter distributions
-    jitter_ext_chnl = self.jitter_ext_chnl  # These are used, again, in bathtub curve generation, below.
-    jitter_ext_tx = self.jitter_ext_tx
-    jitter_ext_ctle = self.jitter_ext_ctle
-    jitter_ext_dfe = self.jitter_ext_dfe
-    self.plotdata.set_data("jitter_bins", array(self.jitter_bins) * 1.0e12)
-    self.plotdata.set_data("jitter_chnl", self.jitter_chnl)
-    self.plotdata.set_data("jitter_ext_chnl", jitter_ext_chnl)
-    self.plotdata.set_data("jitter_tx", self.jitter_tx)
-    self.plotdata.set_data("jitter_ext_tx", jitter_ext_tx)
-    self.plotdata.set_data("jitter_ctle", self.jitter_ctle)
-    self.plotdata.set_data("jitter_ext_ctle", jitter_ext_ctle)
-    self.plotdata.set_data("jitter_dfe", self.jitter_dfe)
-    self.plotdata.set_data("jitter_ext_dfe", jitter_ext_dfe)
+    jitter_chnl = self.jitter_chnl  # These are used again in bathtub curve generation, below.
+    jitter_tx   = self.jitter_tx
+    jitter_ctle = self.jitter_ctle
+    jitter_dfe  = self.jitter_dfe
+    jitter_bins = self.jitter_bins
+    self.plotdata.set_data("jitter_bins", array(self.jitter_bins)  * 1e12)
+    self.plotdata.set_data("jitter_chnl",     jitter_chnl          * 1e-12)  # PDF (/ps)
+    self.plotdata.set_data("jitter_ext_chnl", self.jitter_ext_chnl * 1e-12)
+    self.plotdata.set_data("jitter_tx",       jitter_tx            * 1e-12)
+    self.plotdata.set_data("jitter_ext_tx",   self.jitter_ext_tx   * 1e-12)
+    self.plotdata.set_data("jitter_ctle",     jitter_ctle          * 1e-12)
+    self.plotdata.set_data("jitter_ext_ctle", self.jitter_ext_ctle * 1e-12)
+    self.plotdata.set_data("jitter_dfe",      jitter_dfe           * 1e-12)
+    self.plotdata.set_data("jitter_ext_dfe",  self.jitter_ext_dfe  * 1e-12)
 
     # Jitter spectrums
     log10_ui = safe_log10(ui)
     self.plotdata.set_data("f_MHz", self.f_MHz[1:])
     self.plotdata.set_data("f_MHz_dfe", self.f_MHz_dfe[1:])
     self.plotdata.set_data("jitter_spectrum_chnl", 10.0 * (safe_log10(self.jitter_spectrum_chnl[1:]) - log10_ui))
-    self.plotdata.set_data(
-        "jitter_ind_spectrum_chnl", 10.0 * (safe_log10(self.jitter_ind_spectrum_chnl[1:]) - log10_ui)
-    )
+    self.plotdata.set_data("jitter_ind_spectrum_chnl", 10.0 * (safe_log10(self.jitter_ind_spectrum_chnl[1:]) - log10_ui))
     self.plotdata.set_data("thresh_chnl", 10.0 * (safe_log10(self.thresh_chnl[1:]) - log10_ui))
     self.plotdata.set_data("jitter_spectrum_tx", 10.0 * (safe_log10(self.jitter_spectrum_tx[1:]) - log10_ui))
     self.plotdata.set_data("jitter_ind_spectrum_tx", 10.0 * (safe_log10(self.jitter_ind_spectrum_tx[1:]) - log10_ui))
     self.plotdata.set_data("thresh_tx", 10.0 * (safe_log10(self.thresh_tx[1:]) - log10_ui))
     self.plotdata.set_data("jitter_spectrum_ctle", 10.0 * (safe_log10(self.jitter_spectrum_ctle[1:]) - log10_ui))
-    self.plotdata.set_data(
-        "jitter_ind_spectrum_ctle", 10.0 * (safe_log10(self.jitter_ind_spectrum_ctle[1:]) - log10_ui)
-    )
+    self.plotdata.set_data("jitter_ind_spectrum_ctle", 10.0 * (safe_log10(self.jitter_ind_spectrum_ctle[1:]) - log10_ui))
     self.plotdata.set_data("thresh_ctle", 10.0 * (safe_log10(self.thresh_ctle[1:]) - log10_ui))
     self.plotdata.set_data("jitter_spectrum_dfe", 10.0 * (safe_log10(self.jitter_spectrum_dfe[1:]) - log10_ui))
     self.plotdata.set_data("jitter_ind_spectrum_dfe", 10.0 * (safe_log10(self.jitter_ind_spectrum_dfe[1:]) - log10_ui))
     self.plotdata.set_data("thresh_dfe", 10.0 * (safe_log10(self.thresh_dfe[1:]) - log10_ui))
     self.plotdata.set_data("jitter_rejection_ratio", self.jitter_rejection_ratio[1:])
 
     # Bathtubs
-    half_len = len(jitter_ext_chnl) // 2
-    #  - Channel
-    bathtub_chnl = list(cumsum(jitter_ext_chnl[-1 : -(half_len + 1) : -1]))
-    bathtub_chnl.reverse()
-    bathtub_chnl = array(bathtub_chnl + list(cumsum(jitter_ext_chnl[: half_len + 1])))
-    bathtub_chnl = where(
-        bathtub_chnl < MIN_BATHTUB_VAL,
-        0.1 * MIN_BATHTUB_VAL * ones(len(bathtub_chnl)),
-        bathtub_chnl,
-    )  # To avoid Chaco log scale plot wierdness.
+    bathtub_chnl, (_, _) = make_bathtub(
+        jitter_bins, jitter_chnl, min_val=0.1 * MIN_BATHTUB_VAL,
+        rj=self.rj_chnl, extrap=True)
+    bathtub_tx,   (_,  _) = make_bathtub(
+        jitter_bins, jitter_tx,   min_val=0.1 * MIN_BATHTUB_VAL,
+        rj=self.rj_tx,   extrap=True)
+    bathtub_ctle, (_, _) = make_bathtub(
+        jitter_bins, jitter_ctle, min_val=0.1 * MIN_BATHTUB_VAL,
+        rj=self.rj_ctle, extrap=True)
+    bathtub_dfe,  (_,  _) = make_bathtub(
+        jitter_bins, jitter_dfe,  min_val=0.1 * MIN_BATHTUB_VAL,
+        rj=self.rj_dfe,  extrap=True)
     self.plotdata.set_data("bathtub_chnl", safe_log10(bathtub_chnl))
-    #  - Tx
-    bathtub_tx = list(cumsum(jitter_ext_tx[-1 : -(half_len + 1) : -1]))
-    bathtub_tx.reverse()
-    bathtub_tx = array(bathtub_tx + list(cumsum(jitter_ext_tx[: half_len + 1])))
-    bathtub_tx = where(
-        bathtub_tx < MIN_BATHTUB_VAL, 0.1 * MIN_BATHTUB_VAL * ones(len(bathtub_tx)), bathtub_tx
-    )  # To avoid Chaco log scale plot wierdness.
-    self.plotdata.set_data("bathtub_tx", safe_log10(bathtub_tx))
-    #  - CTLE
-    bathtub_ctle = list(cumsum(jitter_ext_ctle[-1 : -(half_len + 1) : -1]))
-    bathtub_ctle.reverse()
-    bathtub_ctle = array(bathtub_ctle + list(cumsum(jitter_ext_ctle[: half_len + 1])))
-    bathtub_ctle = where(
-        bathtub_ctle < MIN_BATHTUB_VAL,
-        0.1 * MIN_BATHTUB_VAL * ones(len(bathtub_ctle)),
-        bathtub_ctle,
-    )  # To avoid Chaco log scale plot wierdness.
+    self.plotdata.set_data("bathtub_tx",   safe_log10(bathtub_tx))
     self.plotdata.set_data("bathtub_ctle", safe_log10(bathtub_ctle))
-    #  - DFE
-    bathtub_dfe = list(cumsum(jitter_ext_dfe[-1 : -(half_len + 1) : -1]))
-    bathtub_dfe.reverse()
-    bathtub_dfe = array(bathtub_dfe + list(cumsum(jitter_ext_dfe[: half_len + 1])))
-    bathtub_dfe = where(
-        bathtub_dfe < MIN_BATHTUB_VAL, 0.1 * MIN_BATHTUB_VAL * ones(len(bathtub_dfe)), bathtub_dfe
-    )  # To avoid Chaco log scale plot wierdness.
-    self.plotdata.set_data("bathtub_dfe", safe_log10(bathtub_dfe))
+    self.plotdata.set_data("bathtub_dfe",  safe_log10(bathtub_dfe))
 
     # Eyes
     width = 2 * samps_per_ui
     xs = linspace(-ui * 1.0e12, ui * 1.0e12, width)
-    height = 100
+    height = 1000
+    tiny_noise = normal(scale=1e-3, size=len(chnl_out[ignore_samps:]))  # to make channel eye easier to view.
     y_max = 1.1 * max(abs(array(self.chnl_out)))
-    eye_chnl = calc_eye(ui, samps_per_ui, height, self.chnl_out[ignore_samps:], y_max)
+    eye_chnl = calc_eye(ui, samps_per_ui, height, self.chnl_out[ignore_samps:] + tiny_noise, y_max)
     y_max = 1.1 * max(abs(array(self.rx_in)))
     eye_tx = calc_eye(ui, samps_per_ui, height, self.rx_in[ignore_samps:], y_max)
     y_max = 1.1 * max(abs(array(self.ctle_out)))
     eye_ctle = calc_eye(ui, samps_per_ui, height, self.ctle_out[ignore_samps:], y_max)
     i = 0
     while clock_times[i] <= ignore_until:
         i += 1
         assert i < len(clock_times), "ERROR: Insufficient coverage in 'clock_times' vector."
     y_max = 1.1 * max(abs(array(self.dfe_out)))
-    eye_dfe = calc_eye(ui, samps_per_ui, height, self.dfe_out, y_max, clock_times[i:])
+    eye_dfe = calc_eye(ui, samps_per_ui, height, self.dfe_out[ignore_samps:], y_max, clock_times[i:])
     self.plotdata.set_data("eye_index", xs)
     self.plotdata.set_data("eye_chnl", eye_chnl)
     self.plotdata.set_data("eye_tx", eye_tx)
     self.plotdata.set_data("eye_ctle", eye_ctle)
     self.plotdata.set_data("eye_dfe", eye_dfe)
```

### Comparing `PipBERT-4.1.0/src/pybert/models/cdr.py` & `pipbert-6.1.0/src/pybert/models/cdr.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 data recovery (CDR) unit. The class defined, here, is intended for
 integration into the larger *PyBERT* framework.
 
 Copyright (c) 2019 by David Banas; All rights reserved World wide.
 """
 from typing import List, Sequence, Tuple
 
-from numpy import array, mean, sign, where
+from numpy import array, mean, sign, where  # type: ignore
 
 
-class CDR:
+class CDR:  # pylint: disable=too-many-instance-attributes
     """A class providing behavioral modeling of a 'bang- bang' clock data
     recovery (CDR) unit."""
 
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         delta_t: float,
         alpha: float,
         ui: float,
         n_lock_ave: int = 500,
         rel_lock_tol: float = 0.01,
         lock_sustain: int = 500,
@@ -66,15 +66,15 @@
 
     @property
     def locked(self) -> bool:
         """The current locked state."""
 
         return self._locked
 
-    def adapt(self, samples: Sequence[float]) -> Tuple[float, bool]:
+    def adapt(self, samples: Sequence[float]) -> Tuple[float, bool]:  # pylint: disable=too-many-locals
         """Adapt period/phase, according to 3 samples.
 
         Should be called, when the clock has just struck.
 
         Synopsis:
             (ui, locked) = adapt(samples)
```

### Comparing `PipBERT-4.1.0/src/pybert/models/dfe.py` & `pipbert-6.1.0/src/pybert/models/dfe.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 This Python script provides a behavioral model of a decision feedback
 equalizer (DFE). The class defined, here, is intended for integration
 into the larger *PyBERT* framework.
 
 Copyright (c) 2014 by David Banas; All rights reserved World wide.
 """
-from numpy import array, sign, zeros
+from numpy import array, sign, zeros  # type: ignore
 from scipy.signal import iirfilter
 
 from pybert.models.cdr import CDR
 
 gNch_taps = 3  # Number of taps used in summing node filter.
 
 
-class LfilterSS:
+class LfilterSS:  # pylint: disable=too-few-public-methods
     """A single steppable version of scipy.signal.lfilter()."""
 
     def __init__(self, b, a):
         """
         Args:
             b([float]): Coefficients of the numerator of the rational transfer function.
             a([float]): Coefficients of the denominator of the rational transfer function.
@@ -58,18 +58,18 @@
 
         self.xs = xs
         self.ys = ys
 
         return y
 
 
-class DFE:
+class DFE:  # pylint: disable=too-many-instance-attributes
     """Behavioral model of a decision feedback equalizer (DFE)."""
 
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments,too-many-locals
         self,
         n_taps,
         gain,
         delta_t,
         alpha,
         ui,
         n_spb,
@@ -77,14 +77,15 @@
         mod_type=0,
         bandwidth=100.0e9,
         n_ave=10,
         n_lock_ave=500,
         rel_lock_tol=0.01,
         lock_sustain=500,
         ideal=True,
+        limits=None,
     ):
         """
         Inputs:
 
           Required:
 
           - n_taps           # of taps in adaptive filter
@@ -141,14 +142,15 @@
         self.ui = ui
         self.decision_scaler = decision_scaler
         self.mod_type = mod_type
         self.cdr = CDR(delta_t, alpha, ui, n_lock_ave, rel_lock_tol, lock_sustain)
         self.n_ave = n_ave
         self.corrections = zeros(n_taps)
         self.ideal = ideal
+        self.limits = limits
 
         thresholds = []
         if mod_type == 0:  # NRZ
             pass
         elif mod_type == 1:  # Duo-binary
             thresholds.append(-decision_scaler / 2.0)
             thresholds.append(decision_scaler / 2.0)
@@ -179,15 +181,22 @@
         n_ave = self.n_ave
 
         # Calculate this step's corrections and add to running total.
         corrections = [old + new for (old, new) in zip(self.corrections, [val * error * gain for val in tap_values])]
 
         # Update the tap weights with the average corrections, if appropriate.
         if update:
-            tap_weights = [weight + correction / n_ave for (weight, correction) in zip(tap_weights, corrections)]
+            if self.limits:
+                limits = self.limits
+                tap_weights = [max(limits[k][0],
+                                   min(limits[k][1],
+                                       weight + correction / n_ave))
+                               for (k, (weight, correction)) in enumerate(zip(tap_weights, corrections))]
+            else:
+                tap_weights = [weight + correction / n_ave for (weight, correction) in zip(tap_weights, corrections)]
             corrections = zeros(len(corrections))  # Start the averaging process over, again.
 
         # Step the filter delay chain and generate the new output.
         tap_values = [decision] + tap_values[:-1]
         filter_out = sum(array(tap_weights) * array(tap_values))
 
         # Copy local values back to their respective class object variables.
@@ -251,14 +260,15 @@
                 decision = -1
                 bits = [0, 0]
         else:
             raise RuntimeError("ERROR: DFE.decide(): Unrecognized modulation type requested!")
 
         return decision, bits
 
+    # pylint: disable=too-many-locals,too-many-branches,too-many-statements
     def run(self, sample_times, signal):
         """Run the DFE on the input signal.
 
         Args:
             sample_times([float]): Vector of time values at wich
                 corresponding signal values were sampled.
             signal([float]): Vector of sampled signal values.
@@ -311,14 +321,15 @@
         res = []
         tap_weights = [self.tap_weights]
         ui_ests = []
         lockeds = []
         clocks = zeros(len(sample_times))
         clock_times = [next_clock_time]
         bits = []
+        boundary_sample = 0
         for t, x in zip(sample_times, signal):
             if not ideal:
                 sum_out = summing_filter.step(x - filter_out)
             else:
                 sum_out = x - filter_out
             res.append(sum_out)
             if t >= next_boundary_time:
@@ -348,15 +359,15 @@
                 bits.extend(new_bits)
                 slicer_output = decision * decision_scaler
                 error = sum_out - slicer_output
                 update = locked and (clk_cntr % n_ave) == 0
                 if locked:  # We only want error accumulation to happen, when we're locked.
                     nxt_filter_out = self.step(slicer_output, error, update)
                 else:
-                    nxt_filter_out = self.step(decision, 0.0, update)
+                    nxt_filter_out = self.step(slicer_output, 0.0, update)
                 tap_weights.append(self.tap_weights)
                 last_clock_sample = sum_out
                 next_boundary_time = next_clock_time + ui / 2.0
                 next_clock_time += ui
                 clock_times.append(next_clock_time)
             ui_ests.append(ui)
             lockeds.append(locked)
```

### Comparing `PipBERT-4.1.0/src/pybert/parsers/hspice.py` & `pipbert-6.1.0/src/pybert/parsers/hspice.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 Original author: David Banas <capn.freako@gmail.com>
 
 Original date:   January 7, 2022
 
 Copyright (c) 2022 David Banas; all rights reserved World wide.
 """
 import re
+from functools import reduce
+from parsec import count, generate, many, many1, none_of, regex, sepBy1, string  # type: ignore
 
-from parsec import count, generate, many, many1, none_of, regex, sepBy1, string
 
-
-class CSDF:
+class CSDF:  # pylint: disable=too-few-public-methods
     """Common Simulation Data Format (CSDF)"""
 
     def __init__(self, hdr, nms, wvs):
         assert len(nms) == int(hdr["NODES"])
         self.header = {}
         self.header.update(hdr)
         self.names = nms
@@ -72,10 +72,11 @@
 def csdf_data():
     "Parse CSDF file contents."
     hdr = yield header
     nms = yield sig_names
     wvs = yield many1(wave_samps)
     return CSDF(
         dict(map(lambda pr: (pr[0], "".join(pr[1])), hdr)),
-        list(map(lambda cs: "".join(cs), nms)),
+        # list(map(lambda cs: "".join(cs), nms)),
+        list(reduce("".join, nms)),
         list(map(lambda pr: (float(pr[0]), pr[1]), wvs)),
     )
```

### Comparing `PipBERT-4.1.0/src/pybert/pybert.py` & `pipbert-6.1.0/src/pybert/pybert.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,443 +1,198 @@
 #! /usr/bin/env python
 
-"""Bit error rate tester (BERT) simulator, written in Python.
+# pylint: disable=too-many-lines
+
+"""
+Bit error rate tester (BERT) simulator, written in Python.
 
 Original Author: David Banas <capn.freako@gmail.com>
 
 Original Date:   17 June 2014
 
 Testing by: Mark Marlett <mark.marlett@gmail.com>
 
 This Python script provides a GUI interface to a BERT simulator, which
 can be used to explore the concepts of serial communication link design.
 
 Copyright (c) 2014 by David Banas; All rights reserved World wide.
+
+ToDo:
+    1. Add optional AFE (4th-order Bessel-Thomson).
+    2. Add eye contour plots.
 """
+
 import platform
 import time
 from datetime import datetime
 from os.path import dirname, join
 from pathlib import Path
-from threading import Event, Thread
-from time import sleep
 
-import numpy as np
+import numpy as np  # type: ignore
 import skrf as rf
 from chaco.api import ArrayPlotData, GridPlotContainer
-from numpy import array, convolve, cos, exp, ones, pad, pi, sinc, where, zeros
-from numpy.fft import fft, irfft
-from numpy.random import randint
-from pyibisami import __version__ as PyAMI_VERSION
-from pyibisami.ami.model import AMIModel
-from pyibisami.ami.parser import AMIParamConfigurator
-from pyibisami.ibis.file import IBISModel
-from scipy.optimize import minimize, minimize_scalar
+from numpy import arange, array, cos, exp, pad, pi, sinc, where, zeros
+from numpy.fft import irfft, rfft  # type: ignore
+from numpy.random import randint  # type: ignore
 from traits.api import (
     Array,
     Bool,
     Button,
-    Enum,
     File,
     Float,
     HasTraits,
     Instance,
     Int,
     List,
     Map,
     Property,
     Range,
     String,
     cached_property,
 )
-from traitsui.message import message
+from traits.etsconfig.api import ETSConfig
+from traitsui.message import message, error
+from scipy.interpolate import interp1d
+
+from pyibisami import __version__ as PyAMI_VERSION  # type: ignore
+from pyibisami.ami.model import AMIModel
+from pyibisami.ami.parser import AMIParamConfigurator
+from pyibisami.ibis.file import IBISModel
 
-from pybert import __authors__ as AUTHORS
-from pybert import __copy__ as COPY
-from pybert import __date__ as DATE
 from pybert import __version__ as VERSION
 from pybert.configuration import InvalidFileType, PyBertCfg
 from pybert.gui.help import help_str
 from pybert.gui.plot import make_plots
 from pybert.models.bert import my_run_simulation
+from pybert.models.tx_tap import TxTapTuner
 from pybert.results import PyBertData
+from pybert.threads.optimization import OptThread
 from pybert.utility import (
     calc_gamma,
     import_channel,
-    interp_s2p,
     lfsr_bits,
-    make_ctle,
-    pulse_center,
+    raised_cosine,
     safe_log10,
     sdd_21,
     trim_impulse,
 )
 
 gDebugStatus = False
-gDebugOptimize = False
-gMaxCTLEPeak = 20.0  # max. allowed CTLE peaking (dB) (when optimizing, only)
-gMaxCTLEFreq = 20.0  # max. allowed CTLE peak frequency (GHz) (when optimizing, only)
-
-# Default model parameters - Modify these to customize the default simulation.
-# - Simulation Control
-gBitRate = 10  # (Gbps)
-gNbits = 8000  # number of bits to run
-gPatLen = 127  # repeating bit pattern length
-gNspb = 32  # samples per bit
-gNumAve = 1  # Number of bit error samples to average, when sweeping.
-# - Channel Control
-#     - parameters for Howard Johnson's "Metallic Transmission Model"
-#     - (See "High Speed Signal Propagation", Sec. 3.1.)
-#     - ToDo: These are the values for 24 guage twisted copper pair; need to add other options.
-gRdc = 0.1876  # Ohms/m
-gw0 = 10.0e6  # 10 MHz is recommended in Ch. 8 of his second book, in which UTP is described in detail.
-gR0 = 1.452  # skin-effect resistance (Ohms/m)log
-gTheta0 = 0.02  # loss tangent
-gZ0 = 100.0  # characteristic impedance in LC region (Ohms)
-gv0 = 0.67  # relative propagation velocity (c)
-gl_ch = 1.0  # cable length (m)
-gRn = (
-    0.001  # standard deviation of Gaussian random noise (V) (Applied at end of channel, so as to appear white to Rx.)
-)
-# - Tx
-gVod = 1.0  # output drive strength (Vp)
-gRs = 100  # differential source impedance (Ohms)
-gCout = 0.50  # parasitic output capacitance (pF) (Assumed to exist at both 'P' and 'N' nodes.)
-gPnMag = 0.001  # magnitude of periodic noise (V)
-gPnFreq = 0.437  # frequency of periodic noise (MHz)
-# - Rx
-gRin = 100  # differential input resistance
-gCin = 0.50  # parasitic input capacitance (pF) (Assumed to exist at both 'P' and 'N' nodes.)
-gCac = 1.0  # a.c. coupling capacitance (uF) (Assumed to exist at both 'P' and 'N' nodes.)
-gBW = 12.0  # Rx signal path bandwidth, assuming no CTLE action. (GHz)
-gUseDfe = True  # Include DFE when running simulation.
-gDfeIdeal = True  # DFE ideal summing node selector
-gPeakFreq = 5.0  # CTLE peaking frequency (GHz)
-gPeakMag = 1.7  # CTLE peaking magnitude (dB)
-gCTLEOffset = 0.0  # CTLE d.c. offset (dB)
-# - DFE
-gDecisionScaler = 0.5
-gNtaps = 5
-gGain = 0.5
-gNave = 100
-gDfeBW = 12.0  # DFE summing node bandwidth (GHz)
-# - CDR
-gDeltaT = 0.1  # (ps)
-gAlpha = 0.01
-gNLockAve = 500  # number of UI used to average CDR locked status.
-gRelLockTol = 0.1  # relative lock tolerance of CDR.
-gLockSustain = 500
-# - Analysis
-gThresh = 6  # threshold for identifying periodic jitter spectral elements (sigma)
-
-
-class StoppableThread(Thread):
-    """Thread class with a stop() method.
-
-    The thread itself has to check regularly for the stopped() condition.
-
-    All PyBERT thread classes are subclasses of this class.
-    """
-
-    def __init__(self):
-        super(StoppableThread, self).__init__()
-        self._stop_event = Event()
-
-    def stop(self):
-        """Called by thread invoker, when thread should be stopped
-        prematurely."""
-        self._stop_event.set()
-
-    def stopped(self):
-        """Should be called by thread (i.e. - subclass) periodically and, if this function
-        returns True, thread should clean itself up and quit ASAP.
-        """
-        return self._stop_event.is_set()
-
-
-class TxOptThread(StoppableThread):
-    """Used to run Tx tap weight optimization in its own thread, in order to
-    preserve GUI responsiveness."""
-
-    def run(self):
-        """Run the Tx equalization optimization thread."""
-
-        pybert = self.pybert
-
-        if self.update_status:
-            pybert.status = "Optimizing Tx..."
-
-        max_iter = pybert.max_iter
-
-        old_taps = []
-        min_vals = []
-        max_vals = []
-        for tuner in pybert.tx_tap_tuners:
-            if tuner.enabled:
-                old_taps.append(tuner.value)
-                min_vals.append(tuner.min_val)
-                max_vals.append(tuner.max_val)
-
-        cons = {"type": "ineq", "fun": lambda x: 0.7 - sum(abs(x))}
-
-        bounds = list(zip(min_vals, max_vals))
-
-        try:
-            if gDebugOptimize:
-                res = minimize(
-                    self.do_opt_tx,
-                    old_taps,
-                    bounds=bounds,
-                    constraints=cons,
-                    options={"disp": True, "maxiter": max_iter},
-                )
-            else:
-                res = minimize(
-                    self.do_opt_tx,
-                    old_taps,
-                    bounds=bounds,
-                    constraints=cons,
-                    options={"disp": False, "maxiter": max_iter},
-                )
-
-            if self.update_status:
-                if res["success"]:
-                    pybert.status = "Optimization succeeded."
-                else:
-                    pybert.status = f"Optimization failed: {res['message']}"
-
-        except Exception as err:
-            pybert.status = err
-
-    def do_opt_tx(self, taps):
-        """Run the Tx Optimization."""
-        sleep(0.001)  # Give the GUI a chance to acknowledge user clicking the Abort button.
-
-        if self.stopped():
-            raise RuntimeError("Optimization aborted.")
-
-        pybert = self.pybert
-        tuners = pybert.tx_tap_tuners
-        taps = list(taps)
-        for tuner in tuners:
-            if tuner.enabled:
-                tuner.value = taps.pop(0)
-        return pybert.cost
-
-
-class RxOptThread(StoppableThread):
-    """Used to run Rx tap weight optimization in its own thread, in order to
-    preserve GUI responsiveness."""
-
-    def run(self):
-        """Run the Rx equalization optimization thread."""
-
-        pybert = self.pybert
-
-        pybert.status = "Optimizing Rx..."
-        max_iter = pybert.max_iter
-        max_mag_tune = pybert.max_mag_tune
-
-        try:
-            if gDebugOptimize:
-                res = minimize_scalar(
-                    self.do_opt_rx,
-                    bounds=(0, max_mag_tune),
-                    method="Bounded",
-                    options={"disp": True, "maxiter": max_iter},
-                )
-            else:
-                res = minimize_scalar(
-                    self.do_opt_rx,
-                    bounds=(0, max_mag_tune),
-                    method="Bounded",
-                    options={"disp": False, "maxiter": max_iter},
-                )
-
-            if res["success"]:
-                pybert.status = "Optimization succeeded."
-            else:
-                pybert.status = f"Optimization failed: {res['message']}"
-
-        except Exception as err:
-            pybert.status = err
+gUseDfe      = True     # Include DFE when running simulation.
+gMaxCTLEPeak =    20.0  # max. allowed CTLE peaking (dB) (when optimizing, only)
+gPeakFreq    =     5.0  # CTLE peaking frequency (GHz)
+gPeakMag     =     1.7  # CTLE peaking magnitude (dB)
+gCTLEOffset  =     0.0  # CTLE d.c. offset (dB)
+gNtaps       =     5
 
-    def do_opt_rx(self, peak_mag):
-        """Run the Rx Optimization."""
-        sleep(0.001)  # Give the GUI a chance to acknowledge user clicking the Abort button.
 
-        if self.stopped():
-            raise RuntimeError("Optimization aborted.")
-
-        pybert = self.pybert
-        pybert.peak_mag_tune = peak_mag
-        return pybert.cost
-
-
-class CoOptThread(StoppableThread):
-    """Used to run co-optimization in its own thread, in order to preserve GUI
-    responsiveness."""
-
-    def run(self):
-        """Run the Tx/Rx equalization co-optimization thread."""
-
-        pybert = self.pybert
-
-        pybert.status = "Co-optimizing..."
-        max_iter = pybert.max_iter
-        max_mag_tune = pybert.max_mag_tune
-
-        try:
-            if gDebugOptimize:
-                res = minimize_scalar(
-                    self.do_coopt,
-                    bounds=(0, max_mag_tune),
-                    method="Bounded",
-                    options={"disp": True, "maxiter": max_iter},
-                )
-            else:
-                res = minimize_scalar(
-                    self.do_coopt,
-                    bounds=(0, max_mag_tune),
-                    method="Bounded",
-                    options={"disp": False, "maxiter": max_iter},
-                )
-
-            if res["success"]:
-                pybert.status = "Optimization succeeded."
-            else:
-                pybert.status = f"Optimization failed: {res['message']}"
-
-        except Exception as err:
-            pybert.status = err
-
-    def do_coopt(self, peak_mag):
-        """Run the Tx and Rx Co-Optimization."""
-        sleep(0.001)  # Give the GUI a chance to acknowledge user clicking the Abort button.
-
-        if self.stopped():
-            raise RuntimeError("Optimization aborted.")
-
-        pybert = self.pybert
-        pybert.peak_mag_tune = peak_mag
-        if any([pybert.tx_tap_tuners[i].enabled for i in range(len(pybert.tx_tap_tuners))]):
-            while pybert.tx_opt_thread and pybert.tx_opt_thread.is_alive():
-                sleep(0.001)
-            pybert._do_opt_tx(update_status=False)
-            while pybert.tx_opt_thread and pybert.tx_opt_thread.is_alive():
-                sleep(0.001)
-        return pybert.cost
-
-
-class TxTapTuner(HasTraits):
-    """Object used to populate the rows of the Tx FFE tap tuning table."""
-
-    name = String("(noname)")
-    enabled = Bool(False)
-    min_val = Float(0.0)
-    max_val = Float(0.0)
-    value = Float(0.0)
-    steps = Int(0)  # Non-zero means we want to sweep it.
-
-    def __init__(self, name="(noname)", enabled=False, min_val=0.0, max_val=0.0, value=0.0, steps=0):
-        """Allows user to define properties, at instantiation."""
-
-        # Super-class initialization is ABSOLUTELY NECESSARY, in order
-        # to get all the Traits/UI machinery setup correctly.
-        super().__init__()
-
-        self.name = name
-        self.enabled = enabled
-        self.min_val = min_val
-        self.max_val = max_val
-        self.value = value
-        self.steps = steps
-
-
-class PyBERT(HasTraits):
+class PyBERT(HasTraits):  # pylint: disable=too-many-instance-attributes
     """A serial communication link bit error rate tester (BERT) simulator with
     a GUI interface.
 
     Useful for exploring the concepts of serial communication link
     design.
     """
 
     # Independent variables
 
     # - Simulation Control
-    bit_rate = Range(low=0.1, high=120.0, value=gBitRate)  #: (Gbps)
-    nbits = Range(low=1000, high=10000000, value=gNbits)  #: Number of bits to simulate.
+    bit_rate = Range(low=0.1, high=120.0, value=10.0)    #: (Gbps)
+    nbits = Range(low=1000, high=10000000, value=15000)  #: Number of bits to simulate.
+    eye_bits = Int(10160)                                #: Number of bits used to form eye.
     pattern = Map(
         {
             "PRBS-7": [7, 6],
             "PRBS-15": [15, 14],
             "PRBS-23": [23, 18],
         },
         default_value="PRBS-7",
     )
     seed = Int(1)  # LFSR seed. 0 means regenerate bits, using a new random seed, each run.
-    nspb = Range(low=2, high=256, value=gNspb)  #: Signal vector samples per bit.
-    eye_bits = Int(gNbits // 5)  #: # of bits used to form eye. (Default = last 20%)
-    mod_type = List([0])  #: 0 = NRZ; 1 = Duo-binary; 2 = PAM-4
-    num_sweeps = Int(1)  #: Number of sweeps to run.
-    sweep_num = Int(1)
-    sweep_aves = Int(gNumAve)
-    do_sweep = Bool(False)  #: Run sweeps? (Default = False)
-    debug = Bool(False)  #: Send log messages to terminal, as well as console, when True. (Default = False)
+    nspui = Range(low=2, high=256, value=32)  #: Signal vector samples per unit interval.
+    mod_type   = List([0])                   #: 0 = NRZ; 1 = Duo-binary; 2 = PAM-4
+    do_sweep   = Bool(False)  #: Run sweeps? (Default = False)
+    debug      = Bool(False)  #: Send log messages to terminal, as well as console, when True. (Default = False)
+    thresh     = Float(3.0)   #: Spectral threshold for identifying periodic components (sigma). (Default = 3.0)
 
     # - Channel Control
     ch_file = File(
         "", entries=5, filter=["*.s4p", "*.S4P", "*.csv", "*.CSV", "*.txt", "*.TXT", "*.*"]
     )  #: Channel file name.
     use_ch_file = Bool(False)  #: Import channel description from file? (Default = False)
-    f_step = Float(10)  #: Frequency step to use when constructing H(f). (Default = 10 MHz)
+    renumber = Bool(False)  #: Automically fix "1=>3/2=>4" port numbering? (Default = False)
+    f_step = Float(10)  #: Frequency step to use when constructing H(f) (MHz). (Default = 10 MHz)
+    f_max = Float(40)  #: Frequency maximum to use when constructing H(f) (GHz). (Default = 40 GHz)
     impulse_length = Float(0.0)  #: Impulse response length. (Determined automatically, when 0.)
-    Rdc = Float(gRdc)  #: Channel d.c. resistance (Ohms/m).
-    w0 = Float(gw0)  #: Channel transition frequency (rads./s).
-    R0 = Float(gR0)  #: Channel skin effect resistance (Ohms/m).
-    Theta0 = Float(gTheta0)  #: Channel loss tangent (unitless).
-    Z0 = Float(gZ0)  #: Channel characteristic impedance, in LC region (Ohms).
-    v0 = Float(gv0)  #: Channel relative propagation velocity (c).
-    l_ch = Float(gl_ch)  #: Channel length (m).
+    Rdc = Float(0.1876)  #: Channel d.c. resistance (Ohms/m).
+    w0 = Float(10e6)  #: Channel transition frequency (rads./s).
+    R0 = Float(1.452)  #: Channel skin effect resistance (Ohms/m).
+    Theta0 = Float(0.02)  #: Channel loss tangent (unitless).
+    Z0 = Float(100)  #: Channel characteristic impedance, in LC region (Ohms).
+    v0 = Float(0.67)  #: Channel relative propagation velocity (c).
+    l_ch = Float(0.5)  #: Channel length (m).
+    use_window = Bool(False)  #: Apply raised cosine to frequency response before FFT()-ing? (Default = False)
 
     # - EQ Tune
     tx_tap_tuners = List(
         [
-            TxTapTuner(name="Pre-tap", enabled=True, min_val=-0.2, max_val=0.2, value=0.0),
-            TxTapTuner(name="Post-tap1", enabled=False, min_val=-0.4, max_val=0.4, value=0.0),
-            TxTapTuner(name="Post-tap2", enabled=False, min_val=-0.3, max_val=0.3, value=0.0),
-            TxTapTuner(name="Post-tap3", enabled=False, min_val=-0.2, max_val=0.2, value=0.0),
+            TxTapTuner(name="Pre-tap3",  pos=-3, enabled=True, min_val=-0.05, max_val=0.05, step=0.01),
+            TxTapTuner(name="Pre-tap2",  pos=-2, enabled=True, min_val=-0.1,  max_val=0.1,  step=0.02),
+            TxTapTuner(name="Pre-tap1",  pos=-1, enabled=True, min_val=-0.2,  max_val=0.2,  step=0.04),
+            TxTapTuner(name="Post-tap1", pos=1,  enabled=True, min_val=-0.2,  max_val=0.2,  step=0.04),
+            TxTapTuner(name="Post-tap2", pos=2,  enabled=True, min_val=-0.1,  max_val=0.1,  step=0.02),
+            TxTapTuner(name="Post-tap3", pos=3,  enabled=True, min_val=-0.05, max_val=0.05, step=0.01),
         ]
     )  #: EQ optimizer list of TxTapTuner objects.
-    rx_bw_tune = Float(gBW)  #: EQ optimizer CTLE bandwidth (GHz).
+    rx_bw_tune = Float(12.0)  #: EQ optimizer CTLE bandwidth (GHz).
     peak_freq_tune = Float(gPeakFreq)  #: EQ optimizer CTLE peaking freq. (GHz).
     peak_mag_tune = Float(gPeakMag)  #: EQ optimizer CTLE peaking mag. (dB).
-    max_mag_tune = Float(20)  #: EQ optimizer CTLE peaking mag. (dB).
-    ctle_offset_tune = Float(gCTLEOffset)  #: EQ optimizer CTLE d.c. offset (dB).
-    ctle_mode_tune = Enum("Off", "Passive", "AGC", "Manual")  #: EQ optimizer CTLE mode
-    use_dfe_tune = Bool(gUseDfe)  #: EQ optimizer DFE select (Bool).
-    n_taps_tune = Int(gNtaps)  #: EQ optimizer # DFE taps.
-    max_iter = Int(50)  #: EQ optimizer max. # of optimization iterations.
-    tx_opt_thread = Instance(TxOptThread)  #: Tx EQ optimization thread.
-    rx_opt_thread = Instance(RxOptThread)  #: Rx EQ optimization thread.
-    coopt_thread = Instance(CoOptThread)  #: EQ co-optimization thread.
+    min_mag_tune = Float(2)   #: EQ optimizer CTLE peaking mag. min. (dB).
+    max_mag_tune = Float(12)  #: EQ optimizer CTLE peaking mag. max. (dB).
+    step_mag_tune = Float(1)  #: EQ optimizer CTLE peaking mag. step (dB).
+    ctle_enable_tune = Bool(True)  #: EQ optimizer CTLE enable
+    dfe_tap_tuners = List(
+        [TxTapTuner(name="Tap1",  enabled=True,  min_val=0.1,   max_val=0.4,  value=0.1),
+         TxTapTuner(name="Tap2",  enabled=True,  min_val=-0.15, max_val=0.15, value=0.0),
+         TxTapTuner(name="Tap3",  enabled=True,  min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap4",  enabled=True,  min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap5",  enabled=True,  min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap6",  enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap7",  enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap8",  enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap9",  enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap10", enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap11", enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap12", enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap13", enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap14", enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap15", enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap16", enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap17", enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap18", enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap19", enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),
+         TxTapTuner(name="Tap20", enabled=False, min_val=-0.05, max_val=0.1,  value=0.0),]
+    )  #: EQ optimizer list of DFE tap tuner objects.
+    opt_thread = Instance(OptThread)  #: EQ optimization thread.
 
     # - Tx
-    vod = Float(gVod)  #: Tx differential output voltage (V)
-    rs = Float(gRs)  #: Tx source impedance (Ohms)
-    cout = Range(low=0.001, high=1000, value=gCout)  #: Tx parasitic output capacitance (pF)
-    pn_mag = Float(gPnMag)  #: Periodic noise magnitude (V).
-    pn_freq = Float(gPnFreq)  #: Periodic noise frequency (MHz).
-    rn = Float(gRn)  #: Standard deviation of Gaussian random noise (V).
+    vod = Float(1.0)  #: Tx differential output voltage (V)
+    rs = Float(100)  #: Tx source impedance (Ohms)
+    cout = Range(low=0.001, high=1000, value=0.5)  #: Tx parasitic output capacitance (pF)
+    pn_mag = Float(0.1)  #: Periodic noise magnitude (V).
+    pn_freq = Float(11)  #: Periodic noise frequency (MHz).
+    rn = Float(0.1)  #: Standard deviation of Gaussian random noise (V).
     tx_taps = List(
         [
-            TxTapTuner(name="Pre-tap", enabled=True, min_val=-0.2, max_val=0.2, value=-0.066),
-            TxTapTuner(name="Post-tap1", enabled=False, min_val=-0.4, max_val=0.4, value=0.0),
-            TxTapTuner(name="Post-tap2", enabled=False, min_val=-0.3, max_val=0.3, value=0.0),
-            TxTapTuner(name="Post-tap3", enabled=False, min_val=-0.2, max_val=0.2, value=0.0),
+            TxTapTuner(name="Pre-tap3",  pos=-3, enabled=True, min_val=-0.05, max_val=0.05),
+            TxTapTuner(name="Pre-tap2",  pos=-2, enabled=True, min_val=-0.1,  max_val=0.1),
+            TxTapTuner(name="Pre-tap1",  pos=-1, enabled=True, min_val=-0.2,  max_val=0.2),
+            TxTapTuner(name="Post-tap1", pos=1,  enabled=True, min_val=-0.2,  max_val=0.2),
+            TxTapTuner(name="Post-tap2", pos=2,  enabled=True, min_val=-0.1,  max_val=0.1),
+            TxTapTuner(name="Post-tap3", pos=3,  enabled=True, min_val=-0.05, max_val=0.05),
         ]
     )  #: List of TxTapTuner objects.
     rel_power = Float(1.0)  #: Tx power dissipation (W).
     tx_use_ami = Bool(False)  #: (Bool)
     tx_has_ts4 = Bool(False)  #: (Bool)
     tx_use_ts4 = Bool(False)  #: (Bool)
     tx_use_getwave = Bool(False)  #: (Bool)
@@ -453,57 +208,49 @@
             "IBIS Models (*.ibs)|*.ibs",
         ],
     )  #: (File)
     tx_ibis_valid = Bool(False)  #: (Bool)
     tx_use_ibis = Bool(False)  #: (Bool)
 
     # - Rx
-    rin = Float(gRin)  #: Rx input impedance (Ohm)
-    cin = Float(gCin)  #: Rx parasitic input capacitance (pF)
-    cac = Float(gCac)  #: Rx a.c. coupling capacitance (uF)
+    rin = Float(100)  #: Rx input impedance (Ohm)
+    cin = Float(0.5)  #: Rx parasitic input capacitance (pF)
+    cac = Float(1.0)  #: Rx a.c. coupling capacitance (uF)
     use_ctle_file = Bool(False)  #: For importing CTLE impulse/step response directly.
     ctle_file = File("", entries=5, filter=["*.csv"])  #: CTLE response file (when use_ctle_file = True).
-    rx_bw = Float(gBW)  #: CTLE bandwidth (GHz).
+    rx_bw = Float(12.0)  #: CTLE bandwidth (GHz).
     peak_freq = Float(gPeakFreq)  #: CTLE peaking frequency (GHz)
     peak_mag = Float(gPeakMag)  #: CTLE peaking magnitude (dB)
-    ctle_offset = Float(gCTLEOffset)  #: CTLE d.c. offset (dB)
-    ctle_mode = Enum("Off", "Passive", "AGC", "Manual")  #: CTLE mode ('Off', 'Passive', 'AGC', 'Manual').
-    ctle_mode = "Passive"
+    ctle_enable = Bool(True)  #: CTLE enable.
     rx_use_ami = Bool(False)  #: (Bool)
     rx_has_ts4 = Bool(False)  #: (Bool)
     rx_use_ts4 = Bool(False)  #: (Bool)
     rx_use_getwave = Bool(False)  #: (Bool)
     rx_has_getwave = Bool(False)  #: (Bool)
     rx_ami_file = File("", entries=5, filter=["*.ami"])  #: (File)
     rx_ami_valid = Bool(False)  #: (Bool)
     rx_dll_file = File("", entries=5, filter=["*.dll", "*.so"])  #: (File)
     rx_dll_valid = Bool(False)  #: (Bool)
     rx_ibis_file = File("", entries=5, filter=["*.ibs"])  #: (File)
     rx_ibis_valid = Bool(False)  #: (Bool)
     rx_use_ibis = Bool(False)  #: (Bool)
 
     # - DFE
-    use_dfe = Bool(gUseDfe)  #: True = use a DFE (Bool).
-    sum_ideal = Bool(gDfeIdeal)  #: True = use an ideal (i.e. - infinite bandwidth) summing node (Bool).
-    decision_scaler = Float(gDecisionScaler)  #: DFE slicer output voltage (V).
-    gain = Float(gGain)  #: DFE error gain (unitless).
-    n_ave = Float(gNave)  #: DFE # of averages to take, before making tap corrections.
-    n_taps = Int(gNtaps)  #: DFE # of taps.
-    _old_n_taps = n_taps
-    sum_bw = Float(gDfeBW)  #: DFE summing node bandwidth (Used when sum_ideal=False.) (GHz).
+    sum_ideal = Bool(True)  #: True = use an ideal (i.e. - infinite bandwidth) summing node (Bool).
+    decision_scaler = Float(0.5)  #: DFE slicer output voltage (V).
+    gain = Float(0.2)  #: DFE error gain (unitless).
+    n_ave = Float(100)  #: DFE # of averages to take, before making tap corrections.
+    sum_bw = Float(12.0)  #: DFE summing node bandwidth (Used when sum_ideal=False.) (GHz).
 
     # - CDR
-    delta_t = Float(gDeltaT)  #: CDR proportional branch magnitude (ps).
-    alpha = Float(gAlpha)  #: CDR integral branch magnitude (unitless).
-    n_lock_ave = Int(gNLockAve)  #: CDR # of averages to take in determining lock.
-    rel_lock_tol = Float(gRelLockTol)  #: CDR relative tolerance to use in determining lock.
-    lock_sustain = Int(gLockSustain)  #: CDR hysteresis to use in determining lock.
-
-    # - Analysis
-    thresh = Int(gThresh)  #: Threshold for identifying periodic jitter components (sigma).
+    delta_t = Float(0.1)  #: CDR proportional branch magnitude (ps).
+    alpha = Float(0.01)  #: CDR integral branch magnitude (unitless).
+    n_lock_ave = Int(500)  #: CDR # of averages to take in determining lock.
+    rel_lock_tol = Float(0.1)  #: CDR relative tolerance to use in determining lock.
+    lock_sustain = Int(500)  #: CDR hysteresis to use in determining lock.
 
     # Misc.
     cfg_file = File("", entries=5, filter=["*.pybert_cfg"])  #: PyBERT configuration data storage file (File).
     data_file = File("", entries=5, filter=["*.pybert_data"])  #: PyBERT results data storage file (File).
 
     # Plots (plot containers, actually)
     plotdata = ArrayPlotData()
@@ -540,76 +287,61 @@
     # - Handled by the Traits/UI machinery. (Should only contain "low overhead" variables, which don't freeze the GUI noticeably.)
     #
     # - Note: Don't make properties, which have a high calculation overhead, dependencies of other properties!
     #         This will slow the GUI down noticeably.
     jitter_info = Property(String, depends_on=["jitter_perf"])
     status_str = Property(String, depends_on=["status"])
     sweep_info = Property(String, depends_on=["sweep_results"])
-    tx_h_tune = Property(Array, depends_on=["tx_tap_tuners.value", "nspui"])
-    ctle_h_tune = Property(
-        Array,
-        depends_on=[
-            "peak_freq_tune",
-            "peak_mag_tune",
-            "rx_bw_tune",
-            "w",
-            "len_h",
-            "ctle_mode_tune",
-            "ctle_offset_tune",
-            "use_dfe_tune",
-            "n_taps_tune",
-        ],
-    )
-    ctle_out_h_tune = Property(Array, depends_on=["tx_h_tune", "ctle_h_tune", "chnl_h"])
-    cost = Property(Float, depends_on=["ctle_out_h_tune", "nspui"])
-    rel_opt = Property(Float, depends_on=["cost"])
-    t = Property(Array, depends_on=["ui", "nspb", "nbits"])
+    t = Property(Array, depends_on=["ui", "nspui", "nbits"])
     t_ns = Property(Array, depends_on=["t"])
-    f = Property(Array, depends_on=["t"])
+    f = Property(Array, depends_on=["f_step", "f_max"])
     w = Property(Array, depends_on=["f"])
+    t_irfft = Property(Array, depends_on=["f"])
     bits = Property(Array, depends_on=["pattern", "nbits", "mod_type", "run_count"])
     symbols = Property(Array, depends_on=["bits", "mod_type", "vod"])
     ffe = Property(Array, depends_on=["tx_taps.value", "tx_taps.enabled"])
     ui = Property(Float, depends_on=["bit_rate", "mod_type"])
     nui = Property(Int, depends_on=["nbits", "mod_type"])
-    nspui = Property(Int, depends_on=["nspb", "mod_type"])
     eye_uis = Property(Int, depends_on=["eye_bits", "mod_type"])
     dfe_out_p = Array()
-    przf_err = Property(Float, depends_on=["dfe_out_p"])
 
     # Custom buttons, which we'll use in particular tabs.
     # (Globally applicable buttons, such as "Run" and "Ok", are handled more simply, in the View.)
-    btn_rst_eq = Button(label="ResetEq")
-    btn_save_eq = Button(label="SaveEq")
-    btn_opt_tx = Button(label="OptTx")
-    btn_opt_rx = Button(label="OptRx")
-    btn_coopt = Button(label="CoOpt")
-    btn_abort = Button(label="Abort")
+    btn_disable = Button(label="Disable All")  # Disable all DFE taps in optimizer.
+    btn_enable = Button(label="Enable All")  # Enable all DFE taps in optimizer.
     btn_cfg_tx = Button(label="Configure")  # Configure AMI parameters.
     btn_cfg_rx = Button(label="Configure")
     btn_sel_tx = Button(label="Select")  # Select IBIS model.
     btn_sel_rx = Button(label="Select")
     btn_view_tx = Button(label="View")  # View IBIS model.
     btn_view_rx = Button(label="View")
 
     # Logger & Pop-up
     def log(self, msg, alert=False, exception=None):
         """Log a message to the console and, optionally, to terminal and/or
         pop-up dialog."""
         _msg = msg.strip()
         txt = f"[{datetime.now()}]: PyBERT: {_msg}"
         if self.debug:
-            ## In case PyBERT crashes, before we can read this in its `Console` tab:
+            # In case PyBERT crashes, before we can read this in its `Console` tab:
             print(txt, flush=True)
         self.console_log += txt + "\n"
         if exception:
             raise exception
         if alert and self.GUI:
             message(_msg, "PyBERT Alert")
 
+    # User "yes"/"no" alert box.
+    def alert(self, msg):
+        "Prompt for a yes/no response, using simple alert dialog."
+        _msg = msg.strip()
+        if self.GUI:
+            return error(_msg, "PyBERT Alert")
+        raise RuntimeError("Alert box requested, but no GUI!")
+
     # Default initialization
     def __init__(self, run_simulation=True, gui=True):
         """Initial plot setup occurs here.
 
         In order to populate the data structure we need to
         construct the plots, we must run the simulation.
 
@@ -629,88 +361,45 @@
 
         self.GUI = gui
         self.log("Started.")
         self.log_information()
         if self.debug:
             self.log("Debug Mode Enabled.")
 
+        INIT_LEN = 640
+        self.plotdata.set_data("t_ns_opt", self.t_ns[:INIT_LEN])
+        self.plotdata.set_data("clocks_tune", zeros(INIT_LEN))
+        self.plotdata.set_data("ctle_out_h_tune", zeros(INIT_LEN))
+        self.plotdata.set_data("s_ctle", zeros(INIT_LEN))
+        self.plotdata.set_data("s_ctle_out", zeros(INIT_LEN))
+        self.plotdata.set_data("s_tx", zeros(INIT_LEN))
+        self.plotdata.set_data("p_chnl", zeros(INIT_LEN))
+        self.plotdata.set_data("p_ctle", zeros(INIT_LEN))
+        self.plotdata.set_data("p_ctle_out", zeros(INIT_LEN))
+        self.plotdata.set_data("p_tx", zeros(INIT_LEN))
+        self.plotdata.set_data("p_tx_out", zeros(INIT_LEN))
+        self.plotdata.set_data("curs_ix", [0, 0])
+        self.plotdata.set_data("curs_amp", [0, 0])
+
         if run_simulation:
             self.simulate(initial_run=True)
-        else:
-            self.calc_chnl_h()  # Prevents missing attribute error in _get_ctle_out_h_tune().
-
-    # Custom button handlers
-    def _btn_rst_eq_fired(self):
-        """Reset the equalization."""
-        for i in range(4):
-            self.tx_tap_tuners[i].value = self.tx_taps[i].value
-            self.tx_tap_tuners[i].enabled = self.tx_taps[i].enabled
-        self.peak_freq_tune = self.peak_freq
-        self.peak_mag_tune = self.peak_mag
-        self.rx_bw_tune = self.rx_bw
-        self.ctle_mode_tune = self.ctle_mode
-        self.ctle_offset_tune = self.ctle_offset
-        self.use_dfe_tune = self.use_dfe
-        self.n_taps_tune = self.n_taps
-
-    def _btn_save_eq_fired(self):
-        """Save the equalization."""
-        for i in range(4):
-            self.tx_taps[i].value = self.tx_tap_tuners[i].value
-            self.tx_taps[i].enabled = self.tx_tap_tuners[i].enabled
-        self.peak_freq = self.peak_freq_tune
-        self.peak_mag = self.peak_mag_tune
-        self.rx_bw = self.rx_bw_tune
-        self.ctle_mode = self.ctle_mode_tune
-        self.ctle_offset = self.ctle_offset_tune
-        self.use_dfe = self.use_dfe_tune
-        self.n_taps = self.n_taps_tune
-
-    def _btn_opt_tx_fired(self):
-        if (
-            self.tx_opt_thread
-            and self.tx_opt_thread.is_alive()
-            or not any([self.tx_tap_tuners[i].enabled for i in range(len(self.tx_tap_tuners))])
-        ):
-            pass
-        else:
-            self._do_opt_tx()
-
-    def _do_opt_tx(self, update_status=True):
-        self.tx_opt_thread = TxOptThread()
-        self.tx_opt_thread.pybert = self
-        self.tx_opt_thread.update_status = update_status
-        self.tx_opt_thread.start()
 
-    def _btn_opt_rx_fired(self):
-        if self.rx_opt_thread and self.rx_opt_thread.is_alive() or self.ctle_mode_tune == "Off":
+    def _btn_disable_fired(self):
+        if self.opt_thread and self.opt_thread.is_alive():
             pass
         else:
-            self.rx_opt_thread = RxOptThread()
-            self.rx_opt_thread.pybert = self
-            self.rx_opt_thread.start()
+            for tap in self.dfe_tap_tuners:
+                tap.enabled = False
 
-    def _btn_coopt_fired(self):
-        if self.coopt_thread and self.coopt_thread.is_alive():
+    def _btn_enable_fired(self):
+        if self.opt_thread and self.opt_thread.is_alive():
             pass
         else:
-            self.coopt_thread = CoOptThread()
-            self.coopt_thread.pybert = self
-            self.coopt_thread.start()
-
-    def _btn_abort_fired(self):
-        if self.coopt_thread and self.coopt_thread.is_alive():
-            self.coopt_thread.stop()
-            self.coopt_thread.join(10)
-        if self.tx_opt_thread and self.tx_opt_thread.is_alive():
-            self.tx_opt_thread.stop()
-            self.tx_opt_thread.join(10)
-        if self.rx_opt_thread and self.rx_opt_thread.is_alive():
-            self.rx_opt_thread.stop()
-            self.rx_opt_thread.join(10)
+            for tap in self.dfe_tap_tuners:
+                tap.enabled = True
 
     def _btn_cfg_tx_fired(self):
         self._tx_cfg()
 
     def _btn_cfg_rx_fired(self):
         self._rx_cfg()
 
@@ -763,33 +452,39 @@
     def _get_t_ns(self):
         """Calculate the system time vector, in ns."""
 
         return self.t * 1.0e9
 
     @cached_property
     def _get_f(self):
-        """Calculate the frequency vector appropriate for indexing non-shifted
-        FFT output, in Hz.
-
-        # (i.e. - [0, f0, 2 * f0, ... , fN] + [-(fN - f0), -(fN - 2 * f0), ... , -f0]
-
-        Note: Changed to positive freqs. only, in conjunction w/ irfft() usage.
         """
-        t = self.t
-        npts = len(t)
-        f0 = 1.0 / (t[1] * npts)
-        half_npts = npts // 2
-        return array([i * f0 for i in range(half_npts)])
+        Calculate the frequency vector for channel model construction.
+        """
+        fstep = self.f_step * 1e6
+        fmax  = self.f_max  * 1e9
+        return arange(0, fmax + fstep, fstep)  # "+fstep", so fmax gets included
 
     @cached_property
     def _get_w(self):
-        """System frequency vector, in rads./sec."""
+        """
+        Channel modeling frequency vector, in rads./sec.
+        """
         return 2 * pi * self.f
 
     @cached_property
+    def _get_t_irfft(self):
+        """
+        Calculate the time vector appropriate for indexing `irfft()` output.
+        """
+        f = self.f
+        tmax = 1 / f[1]
+        tstep = 0.5 / f[-1]
+        return arange(0, tmax, tstep)
+
+    @cached_property
     def _get_bits(self):
         "Generate the bit stream."
         pattern = self.pattern_
         seed = self.seed
         nbits = self.nbits
 
         if not seed:  # The user sets `seed` to zero when she wants a new random seed generated for each run.
@@ -825,27 +520,14 @@
         nui = nbits
         if mod_type == 2:  # PAM-4
             nui //= 2
 
         return nui
 
     @cached_property
-    def _get_nspui(self):
-        """Returns the number of samples per unit interval."""
-
-        mod_type = self.mod_type[0]
-        nspb = self.nspb
-
-        nspui = nspb
-        if mod_type == 2:  # PAM-4
-            nspui *= 2
-
-        return nspui
-
-    @cached_property
     def _get_eye_uis(self):
         """Returns the number of unit intervals to use for eye construction."""
 
         mod_type = self.mod_type[0]
         eye_bits = self.eye_bits
 
         eye_uis = eye_bits
@@ -854,15 +536,15 @@
 
         return eye_uis
 
     @cached_property
     def _get_ideal_h(self):
         """Returns the ideal link impulse response."""
 
-        ui = self.ui
+        ui = self.ui.value
         nspui = self.nspui
         t = self.t
         mod_type = self.mod_type[0]
         ideal_type = self.ideal_type[0]
 
         t = array(t) - t[-1] / 2.0
 
@@ -870,20 +552,20 @@
             ideal_h = zeros(len(t))
             ideal_h[len(t) / 2] = 1.0
         elif ideal_type == 1:  # sinc
             ideal_h = sinc(t / (ui / 2.0))
         elif ideal_type == 2:  # raised cosine
             ideal_h = (cos(pi * t / (ui / 2.0)) + 1.0) / 2.0
             ideal_h = where(t < -ui / 2.0, zeros(len(t)), ideal_h)
-            ideal_h = where(t > ui / 2.0, zeros(len(t)), ideal_h)
+            ideal_h = where(t >  ui / 2.0, zeros(len(t)), ideal_h)
         else:
-            raise Exception("PyBERT._get_ideal_h(): ERROR: Unrecognized ideal impulse response type.")
+            raise ValueError("PyBERT._get_ideal_h(): ERROR: Unrecognized ideal impulse response type.")
 
         if mod_type == 1:  # Duo-binary relies upon the total link impulse response to perform the required addition.
-            ideal_h = 0.5 * (ideal_h + pad(ideal_h[:-nspui], (nspui, 0), "constant", constant_values=(0, 0)))
+            ideal_h = 0.5 * (ideal_h + pad(ideal_h[:-1 * nspui], (nspui, 0), "constant", constant_values=(0, 0)))
 
         return ideal_h
 
     @cached_property
     def _get_symbols(self):
         """Generate the symbol stream."""
 
@@ -906,15 +588,15 @@
                 elif bits == (0, 1):
                     symbols.append(-1.0 / 3.0)
                 elif bits == (1, 0):
                     symbols.append(1.0 / 3.0)
                 else:
                     symbols.append(1.0)
         else:
-            raise Exception("ERROR: _get_symbols(): Unknown modulation type requested!")
+            raise ValueError("ERROR: _get_symbols(): Unknown modulation type requested!")
 
         return array(symbols) * vod
 
     @cached_property
     def _get_ffe(self):
         """Generate the Tx pre-emphasis FIR numerator."""
 
@@ -922,239 +604,233 @@
 
         taps = []
         for tuner in tap_tuners:
             if tuner.enabled:
                 taps.append(tuner.value)
             else:
                 taps.append(0.0)
-        taps.insert(1, 1.0 - sum(map(abs, taps)))  # Assume one pre-tap.
+        curs_pos = -tap_tuners[0].pos
+        curs_val = 1.0 - sum(abs(array(taps)))
+        if curs_pos < 0:
+            taps.insert(0, curs_val)
+        else:
+            taps.insert(curs_pos, curs_val)
 
         return taps
 
-    @cached_property
+    # pylint: disable=too-many-locals,consider-using-f-string,too-many-branches,too-many-statements
+    # @cached_property
     def _get_jitter_info(self):
-        try:
-            isi_chnl = self.isi_chnl * 1.0e12
-            dcd_chnl = self.dcd_chnl * 1.0e12
-            pj_chnl = self.pj_chnl * 1.0e12
-            rj_chnl = self.rj_chnl * 1.0e12
-            isi_tx = self.isi_tx * 1.0e12
-            dcd_tx = self.dcd_tx * 1.0e12
-            pj_tx = self.pj_tx * 1.0e12
-            rj_tx = self.rj_tx * 1.0e12
-            isi_ctle = self.isi_ctle * 1.0e12
-            dcd_ctle = self.dcd_ctle * 1.0e12
-            pj_ctle = self.pj_ctle * 1.0e12
-            rj_ctle = self.rj_ctle * 1.0e12
-            isi_dfe = self.isi_dfe * 1.0e12
-            dcd_dfe = self.dcd_dfe * 1.0e12
-            pj_dfe = self.pj_dfe * 1.0e12
-            rj_dfe = self.rj_dfe * 1.0e12
-
-            isi_rej_tx = 1.0e20
-            dcd_rej_tx = 1.0e20
-            isi_rej_ctle = 1.0e20
-            dcd_rej_ctle = 1.0e20
-            pj_rej_ctle = 1.0e20
-            rj_rej_ctle = 1.0e20
-            isi_rej_dfe = 1.0e20
-            dcd_rej_dfe = 1.0e20
-            pj_rej_dfe = 1.0e20
-            rj_rej_dfe = 1.0e20
-            isi_rej_total = 1.0e20
-            dcd_rej_total = 1.0e20
-            pj_rej_total = 1.0e20
-            rj_rej_total = 1.0e20
-
-            if isi_tx:
-                isi_rej_tx = isi_chnl / isi_tx
-            if dcd_tx:
-                dcd_rej_tx = dcd_chnl / dcd_tx
-            if isi_ctle:
-                isi_rej_ctle = isi_tx / isi_ctle
-            if dcd_ctle:
-                dcd_rej_ctle = dcd_tx / dcd_ctle
-            if pj_ctle:
-                pj_rej_ctle = pj_tx / pj_ctle
-            if rj_ctle:
-                rj_rej_ctle = rj_tx / rj_ctle
-            if isi_dfe:
-                isi_rej_dfe = isi_ctle / isi_dfe
-            if dcd_dfe:
-                dcd_rej_dfe = dcd_ctle / dcd_dfe
-            if pj_dfe:
-                pj_rej_dfe = pj_ctle / pj_dfe
-            if rj_dfe:
-                rj_rej_dfe = rj_ctle / rj_dfe
-            if isi_dfe:
-                isi_rej_total = isi_chnl / isi_dfe
-            if dcd_dfe:
-                dcd_rej_total = dcd_chnl / dcd_dfe
-            if pj_dfe:
-                pj_rej_total = pj_tx / pj_dfe
-            if rj_dfe:
-                rj_rej_total = rj_tx / rj_dfe
-
-            # Temporary, until I figure out DPI independence.
-            info_str = "<style>\n"
-            # info_str += ' table td {font-size: 36px;}\n'
-            # info_str += ' table th {font-size: 38px;}\n'
-            info_str += " table td {font-size: 12em;}\n"
-            info_str += " table th {font-size: 14em;}\n"
-            info_str += "</style>\n"
-            # info_str += '<font size="+3">\n'
-            # End Temp.
-
-            info_str = "<H1>Jitter Rejection by Equalization Component</H1>\n"
-
-            info_str += "<H2>Tx Preemphasis</H2>\n"
-            info_str += '<TABLE border="1">\n'
-            info_str += '<TR align="center">\n'
-            info_str += "<TH>Jitter Component</TH><TH>Input (ps)</TH><TH>Output (ps)</TH><TH>Rejection (dB)</TH>\n"
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">ISI</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                isi_chnl,
-                isi_tx,
-                10.0 * safe_log10(isi_rej_tx),
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">DCD</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                dcd_chnl,
-                dcd_tx,
-                10.0 * safe_log10(dcd_rej_tx),
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">Pj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>n/a</TD>\n' % (
-                pj_chnl,
-                pj_tx,
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">Rj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>n/a</TD>\n' % (
-                rj_chnl,
-                rj_tx,
-            )
-            info_str += "</TR>\n"
-            info_str += "</TABLE>\n"
+        isi_chnl = self.isi_chnl * 1.0e12
+        dcd_chnl = self.dcd_chnl * 1.0e12
+        pj_chnl = self.pj_chnl * 1.0e12
+        rj_chnl = self.rj_chnl * 1.0e12
+        isi_tx = self.isi_tx * 1.0e12
+        dcd_tx = self.dcd_tx * 1.0e12
+        pj_tx = self.pj_tx * 1.0e12
+        rj_tx = self.rj_tx * 1.0e12
+        isi_ctle = self.isi_ctle * 1.0e12
+        dcd_ctle = self.dcd_ctle * 1.0e12
+        pj_ctle = self.pj_ctle * 1.0e12
+        rj_ctle = self.rj_ctle * 1.0e12
+        isi_dfe = self.isi_dfe * 1.0e12
+        dcd_dfe = self.dcd_dfe * 1.0e12
+        pj_dfe = self.pj_dfe * 1.0e12
+        rj_dfe = self.rj_dfe * 1.0e12
+
+        isi_rej_tx = 1.0e20
+        dcd_rej_tx = 1.0e20
+        isi_rej_ctle = 1.0e20
+        dcd_rej_ctle = 1.0e20
+        pj_rej_ctle = 1.0e20
+        rj_rej_ctle = 1.0e20
+        isi_rej_dfe = 1.0e20
+        dcd_rej_dfe = 1.0e20
+        pj_rej_dfe = 1.0e20
+        rj_rej_dfe = 1.0e20
+        isi_rej_total = 1.0e20
+        dcd_rej_total = 1.0e20
+        pj_rej_total = 1.0e20
+        rj_rej_total = 1.0e20
+
+        if isi_tx:
+            isi_rej_tx = isi_chnl / isi_tx
+        if dcd_tx:
+            dcd_rej_tx = dcd_chnl / dcd_tx
+        if isi_ctle:
+            isi_rej_ctle = isi_tx / isi_ctle
+        if dcd_ctle:
+            dcd_rej_ctle = dcd_tx / dcd_ctle
+        if pj_ctle:
+            pj_rej_ctle = pj_tx / pj_ctle
+        if rj_ctle:
+            rj_rej_ctle = rj_tx / rj_ctle
+        if isi_dfe:
+            isi_rej_dfe = isi_ctle / isi_dfe
+        if dcd_dfe:
+            dcd_rej_dfe = dcd_ctle / dcd_dfe
+        if pj_dfe:
+            pj_rej_dfe = pj_ctle / pj_dfe
+        if rj_dfe:
+            rj_rej_dfe = rj_ctle / rj_dfe
+        if isi_dfe:
+            isi_rej_total = isi_chnl / isi_dfe
+        if dcd_dfe:
+            dcd_rej_total = dcd_chnl / dcd_dfe
+        if pj_dfe:
+            pj_rej_total = pj_tx / pj_dfe
+        if rj_dfe:
+            rj_rej_total = rj_tx / rj_dfe
+
+        # Temporary, until I figure out DPI independence.
+        info_str = "<style>\n"
+        info_str += " table td {font-size: 12em;}\n"
+        info_str += " table th {font-size: 14em;}\n"
+        info_str += "</style>\n"
+        # End Temp.
+
+        info_str = "<H1>Jitter Rejection by Equalization Component</H1>\n"
+
+        info_str += "<H2>Tx Preemphasis</H2>\n"
+        info_str += '<TABLE border="1">\n'
+        info_str += '<TR align="center">\n'
+        info_str += "<TH>Jitter Component</TH><TH>Input (ps)</TH><TH>Output (ps)</TH><TH>Rejection (dB)</TH>\n"
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">ISI</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            isi_chnl,
+            isi_tx,
+            10.0 * safe_log10(isi_rej_tx),
+        )
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += f'<TD align="center">DCD</TD><TD>{dcd_chnl:6.3f}</TD><TD>{dcd_tx:6.3f}</TD><TD>{10.0 * safe_log10(dcd_rej_tx):4.1f}</TD>\n'
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">Pj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>n/a</TD>\n' % (
+            pj_chnl,
+            pj_tx,
+        )
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">Rj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>n/a</TD>\n' % (
+            rj_chnl,
+            rj_tx,
+        )
+        info_str += "</TR>\n"
+        info_str += "</TABLE>\n"
 
-            info_str += "<H2>CTLE (+ AMI DFE)</H2>\n"
-            info_str += '<TABLE border="1">\n'
-            info_str += '<TR align="center">\n'
-            info_str += "<TH>Jitter Component</TH><TH>Input (ps)</TH><TH>Output (ps)</TH><TH>Rejection (dB)</TH>\n"
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">ISI</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                isi_tx,
-                isi_ctle,
-                10.0 * safe_log10(isi_rej_ctle),
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">DCD</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                dcd_tx,
-                dcd_ctle,
-                10.0 * safe_log10(dcd_rej_ctle),
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">Pj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                pj_tx,
-                pj_ctle,
-                10.0 * safe_log10(pj_rej_ctle),
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">Rj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                rj_tx,
-                rj_ctle,
-                10.0 * safe_log10(rj_rej_ctle),
-            )
-            info_str += "</TR>\n"
-            info_str += "</TABLE>\n"
+        info_str += "<H2>CTLE (+ AMI DFE)</H2>\n"
+        info_str += '<TABLE border="1">\n'
+        info_str += '<TR align="center">\n'
+        info_str += "<TH>Jitter Component</TH><TH>Input (ps)</TH><TH>Output (ps)</TH><TH>Rejection (dB)</TH>\n"
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">ISI</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            isi_tx,
+            isi_ctle,
+            10.0 * safe_log10(isi_rej_ctle),
+        )
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">DCD</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            dcd_tx,
+            dcd_ctle,
+            10.0 * safe_log10(dcd_rej_ctle),
+        )
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">Pj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            pj_tx,
+            pj_ctle,
+            10.0 * safe_log10(pj_rej_ctle),
+        )
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">Rj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            rj_tx,
+            rj_ctle,
+            10.0 * safe_log10(rj_rej_ctle),
+        )
+        info_str += "</TR>\n"
+        info_str += "</TABLE>\n"
 
-            info_str += "<H2>DFE</H2>\n"
-            info_str += '<TABLE border="1">\n'
-            info_str += '<TR align="center">\n'
-            info_str += "<TH>Jitter Component</TH><TH>Input (ps)</TH><TH>Output (ps)</TH><TH>Rejection (dB)</TH>\n"
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">ISI</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                isi_ctle,
-                isi_dfe,
-                10.0 * safe_log10(isi_rej_dfe),
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">DCD</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                dcd_ctle,
-                dcd_dfe,
-                10.0 * safe_log10(dcd_rej_dfe),
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">Pj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                pj_ctle,
-                pj_dfe,
-                10.0 * safe_log10(pj_rej_dfe),
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">Rj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                rj_ctle,
-                rj_dfe,
-                10.0 * safe_log10(rj_rej_dfe),
-            )
-            info_str += "</TR>\n"
-            info_str += "</TABLE>\n"
+        info_str += "<H2>DFE</H2>\n"
+        info_str += '<TABLE border="1">\n'
+        info_str += '<TR align="center">\n'
+        info_str += "<TH>Jitter Component</TH><TH>Input (ps)</TH><TH>Output (ps)</TH><TH>Rejection (dB)</TH>\n"
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">ISI</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            isi_ctle,
+            isi_dfe,
+            10.0 * safe_log10(isi_rej_dfe),
+        )
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">DCD</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            dcd_ctle,
+            dcd_dfe,
+            10.0 * safe_log10(dcd_rej_dfe),
+        )
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">Pj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            pj_ctle,
+            pj_dfe,
+            10.0 * safe_log10(pj_rej_dfe),
+        )
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">Rj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            rj_ctle,
+            rj_dfe,
+            10.0 * safe_log10(rj_rej_dfe),
+        )
+        info_str += "</TR>\n"
+        info_str += "</TABLE>\n"
 
-            info_str += "<H2>TOTAL</H2>\n"
-            info_str += '<TABLE border="1">\n'
-            info_str += '<TR align="center">\n'
-            info_str += "<TH>Jitter Component</TH><TH>Input (ps)</TH><TH>Output (ps)</TH><TH>Rejection (dB)</TH>\n"
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">ISI</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                isi_chnl,
-                isi_dfe,
-                10.0 * safe_log10(isi_rej_total),
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">DCD</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                dcd_chnl,
-                dcd_dfe,
-                10.0 * safe_log10(dcd_rej_total),
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">Pj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                pj_tx,
-                pj_dfe,
-                10.0 * safe_log10(pj_rej_total),
-            )
-            info_str += "</TR>\n"
-            info_str += '<TR align="right">\n'
-            info_str += '<TD align="center">Rj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
-                rj_tx,
-                rj_dfe,
-                10.0 * safe_log10(rj_rej_total),
-            )
-            info_str += "</TR>\n"
-            info_str += "</TABLE>\n"
-        except Exception as err:
-            info_str = "<H1>Jitter Rejection by Equalization Component</H1>\n"
-            info_str += "Sorry, the following error occurred:\n"
-            info_str += str(err)
+        info_str += "<H2>TOTAL</H2>\n"
+        info_str += '<TABLE border="1">\n'
+        info_str += '<TR align="center">\n'
+        info_str += "<TH>Jitter Component</TH><TH>Input (ps)</TH><TH>Output (ps)</TH><TH>Rejection (dB)</TH>\n"
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">ISI</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            isi_chnl,
+            isi_dfe,
+            10.0 * safe_log10(isi_rej_total),
+        )
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">DCD</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            dcd_chnl,
+            dcd_dfe,
+            10.0 * safe_log10(dcd_rej_total),
+        )
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">Pj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            pj_tx,
+            pj_dfe,
+            10.0 * safe_log10(pj_rej_total),
+        )
+        info_str += "</TR>\n"
+        info_str += '<TR align="right">\n'
+        info_str += '<TD align="center">Rj</TD><TD>%6.3f</TD><TD>%6.3f</TD><TD>%4.1f</TD>\n' % (
+            rj_tx,
+            rj_dfe,
+            10.0 * safe_log10(rj_rej_total),
+        )
+        info_str += "</TR>\n"
+        info_str += "</TABLE>\n"
 
         return info_str
 
-    @cached_property
+    # @cached_property
     def _get_perf_info(self):
         info_str = "<H2>Performance by Component</H2>\n"
         info_str += '  <TABLE border="1">\n'
         info_str += '    <TR align="center">\n'
         info_str += "      <TH>Component</TH><TH>Performance (Msmpls./min.)</TH>\n"
         info_str += "    </TR>\n"
         info_str += '    <TR align="right">\n'
@@ -1169,203 +845,80 @@
         info_str += '    <TR align="right">\n'
         info_str += f'      <TD align="center">DFE</TD><TD>{self.dfe_perf * 6e-05:6.3f}</TD>\n'
         info_str += "    </TR>\n"
         info_str += '    <TR align="right">\n'
         info_str += f'      <TD align="center">Jitter Analysis</TD><TD>{self.jitter_perf * 6e-05:6.3f}</TD>\n'
         info_str += "    </TR>\n"
         info_str += '    <TR align="right">\n'
-        info_str += '      <TD align="center"><strong>TOTAL</strong></TD><TD><strong>%6.3f</strong></TD>\n' % (
-            self.total_perf * 60.0e-6
-        )
+        info_str += f'      <TD align="center"><strong>TOTAL</strong></TD><TD><strong>{self.total_perf * 60.0e-6:6.3f}</strong></TD>\n'
         info_str += "    </TR>\n"
         info_str += '    <TR align="right">\n'
         info_str += f'      <TD align="center">Plotting</TD><TD>{self.plotting_perf * 6e-05:6.3f}</TD>\n'
         info_str += "    </TR>\n"
         info_str += "  </TABLE>\n"
 
         return info_str
 
-    @cached_property
+    # @cached_property
     def _get_sweep_info(self):
         sweep_results = self.sweep_results
 
         info_str = "<H2>Sweep Results</H2>\n"
         info_str += '  <TABLE border="1">\n'
         info_str += '    <TR align="center">\n'
         info_str += "      <TH>Pretap</TH><TH>Posttap</TH><TH>Mean(bit errors)</TH><TH>StdDev(bit errors)</TH>\n"
         info_str += "    </TR>\n"
 
         for item in sweep_results:
             info_str += '    <TR align="center">\n'
             info_str += str(item)
-            # info_str += "      <TD>%+06.3f</TD><TD>%+06.3f</TD><TD>%d</TD><TD>%d</TD>\n" % (
-            #     item[0],
-            #     item[1],
-            #     item[2],
-            #     item[3],
-            # )
             info_str += "    </TR>\n"
 
         info_str += "  </TABLE>\n"
 
         return info_str
 
-    @cached_property
+    # @cached_property
     def _get_status_str(self):
-        status_str = "%-20s | Perf. (Msmpls./min.):  %4.1f" % (
-            self.status,
-            self.total_perf * 60.0e-6,
-        )
-        dly_str = f"         | ChnlDly (ns):    {self.chnl_dly * 1000000000.0:5.3f}"
-        err_str = f"         | BitErrs: {int(self.bit_errs)}"
-        pwr_str = f"         | TxPwr (W): {self.rel_power:4.2f}"
+        status_str = f"{self.status:20s} | Perf. (Msmpls./min.): {self.total_perf * 60.0e-6:4.1f}"
+        dly_str = f"    | ChnlDly (ns): {self.chnl_dly * 1000000000.0:5.3f}"
+        err_str = f"    | BitErrs: {int(self.bit_errs)}"
+        pwr_str = f"    | TxPwr (mW): {self.rel_power * 1e3:3.0f}"
         status_str += dly_str + err_str + pwr_str
-
-        try:
-            jit_str = "         | Jitter (ps):    ISI=%6.3f    DCD=%6.3f    Pj=%6.3f    Rj=%6.3f" % (
-                self.isi_dfe * 1.0e12,
-                self.dcd_dfe * 1.0e12,
-                self.pj_dfe * 1.0e12,
-                self.rj_dfe * 1.0e12,
-            )
-        except:
-            jit_str = "         | (Jitter not available.)"
-
+        jit_str = "    | Jitter (ps):  ISI=%6.1f  DCD=%6.1f  Pj=%6.1f (%6.1f)  Rj=%6.1f (%6.1f)" % (
+            self.isi_dfe * 1.0e12,
+            self.dcd_dfe * 1.0e12,
+            self.pj_dfe * 1.0e12,
+            self.pjDD_dfe * 1.0e12,
+            self.rj_dfe * 1.0e12,
+            self.rjDD_dfe * 1.0e12,
+        )
         status_str += jit_str
 
         return status_str
 
-    @cached_property
-    def _get_tx_h_tune(self):
-        nspui = self.nspui
-        tap_tuners = self.tx_tap_tuners
-
-        taps = []
-        for tuner in tap_tuners:
-            if tuner.enabled:
-                taps.append(tuner.value)
-            else:
-                taps.append(0.0)
-        taps.insert(1, 1.0 - sum(map(abs, taps)))  # Assume one pre-tap.
-
-        h = sum([[x] + list(zeros(nspui - 1)) for x in taps], [])
-
-        return h
-
-    @cached_property
-    def _get_ctle_h_tune(self):
-        w = self.w
-        len_h = self.len_h
-        rx_bw = self.rx_bw_tune * 1.0e9
-        peak_freq = self.peak_freq_tune * 1.0e9
-        peak_mag = self.peak_mag_tune
-        offset = self.ctle_offset_tune
-        mode = self.ctle_mode_tune
-
-        _, H = make_ctle(rx_bw, peak_freq, peak_mag, w, mode, offset)
-        h = irfft(H)
-
-        return h
-
-    @cached_property
-    def _get_ctle_out_h_tune(self):
-        chnl_h = self.chnl_h
-        tx_h = self.tx_h_tune
-        ctle_h = self.ctle_h_tune
-
-        tx_out_h = convolve(tx_h, chnl_h)
-        return convolve(ctle_h, tx_out_h)
-
-    @cached_property
-    def _get_cost(self):
-        nspui = self.nspui
-        h = self.ctle_out_h_tune
-        mod_type = self.mod_type[0]
-
-        s = h.cumsum()
-        p = s - pad(s[:-nspui], (nspui, 0), "constant", constant_values=(0, 0))
-
-        (clock_pos, thresh) = pulse_center(p, nspui)
-        if clock_pos == -1:
-            return 1.0  # Returning a large cost lets it know it took a wrong turn.
-        clocks = thresh * ones(len(p))
-        if mod_type == 1:  # Handle duo-binary.
-            clock_pos -= nspui // 2
-        clocks[clock_pos] = 0.0
-        if mod_type == 1:  # Handle duo-binary.
-            clocks[clock_pos + nspui] = 0.0
-
-        # Cost is simply ISI minus main lobe amplitude.
-        # Note: post-cursor ISI is NOT included in cost, when we're using the DFE.
-        isi = 0.0
-        ix = clock_pos - nspui
-        while ix >= 0:
-            clocks[ix] = 0.0
-            isi += abs(p[ix])
-            ix -= nspui
-        ix = clock_pos + nspui
-        if mod_type == 1:  # Handle duo-binary.
-            ix += nspui
-        while ix < len(p):
-            clocks[ix] = 0.0
-            if not self.use_dfe_tune:
-                isi += abs(p[ix])
-            ix += nspui
-        if self.use_dfe_tune:
-            for i in range(self.n_taps_tune):
-                if clock_pos + nspui * (1 + i) < len(p):
-                    p[int(clock_pos + nspui * (0.5 + i)) :] -= p[clock_pos + nspui * (1 + i)]
-        plot_len = len(self.chnl_h)
-        self.plotdata.set_data("ctle_out_h_tune", p[:plot_len])
-        self.plotdata.set_data("clocks_tune", clocks[:plot_len])
-
-        if mod_type == 1:  # Handle duo-binary.
-            return isi - p[clock_pos] - p[clock_pos + nspui] + 2.0 * abs(p[clock_pos + nspui] - p[clock_pos])
-        return isi - p[clock_pos]
-
-    @cached_property
-    def _get_rel_opt(self):
-        return -self.cost
-
-    @cached_property
-    def _get_przf_err(self):
-        p = self.dfe_out_p
-        nspui = self.nspui
-        n_taps = self.n_taps
-
-        (clock_pos, _) = pulse_center(p, nspui)
-        err = 0
-        len_p = len(p)
-        for i in range(n_taps):
-            ix = clock_pos + (i + 1) * nspui
-            if ix < len_p:
-                err += p[ix] ** 2
-
-        return err / p[clock_pos] ** 2
-
     # Changed property handlers.
     def _status_str_changed(self):
         if gDebugStatus:
             print(self.status_str, flush=True)
 
     def _use_dfe_changed(self, new_value):
         if not new_value:
             for i in range(1, 4):
                 self.tx_taps[i].enabled = True
         else:
             for i in range(1, 4):
                 self.tx_taps[i].enabled = False
 
-    def _use_dfe_tune_changed(self, new_value):
-        if not new_value:
-            for i in range(1, 4):
-                self.tx_tap_tuners[i].enabled = True
-        else:
-            for i in range(1, 4):
-                self.tx_tap_tuners[i].enabled = False
+    def _dfe_tap_tuners_changed(self, new_value):
+        limits = []
+        for tuner in new_value:
+            limits.append((tuner.min_val, tuner.max_val))
+        self.dfe.limits = limits
+        print(f"limits: {limits}", flush=True)
 
     def _tx_ibis_file_changed(self, new_value):
         self.status = f"Parsing IBIS file: {new_value}"
         dName = ""
         try:
             self.tx_ibis_valid = False
             self.tx_use_ami = False
@@ -1377,15 +930,15 @@
             dName = dirname(new_value)
             if self._tx_ibis.dll_file and self._tx_ibis.ami_file:
                 self.tx_dll_file = join(dName, self._tx_ibis.dll_file)
                 self.tx_ami_file = join(dName, self._tx_ibis.ami_file)
             else:
                 self.tx_dll_file = ""
                 self.tx_ami_file = ""
-        except Exception as err:
+        except Exception as err:  # pylint: disable=broad-exception-caught
             self.status = "IBIS file parsing error!"
             error_message = f"Failed to open and/or parse IBIS file!\n{err}"
             self.log(error_message, alert=True, exception=err)
         self._tx_ibis_dir = dName
         self.status = "Done."
 
     def _tx_ami_file_changed(self, new_value):
@@ -1405,27 +958,27 @@
                     self.tx_use_getwave = True
                 if pcfg.fetch_param_val(["Reserved_Parameters", "Ts4file"]):
                     self.tx_has_ts4 = True
                 else:
                     self.tx_has_ts4 = False
                 self._tx_cfg = pcfg
                 self.tx_ami_valid = True
-        except Exception as err:
-            raise
+        except Exception as err:  # pylint: disable=broad-exception-caught
             error_message = f"Failed to open and/or parse AMI file!\n{err}"
             self.log(error_message, alert=True)
+            raise
 
     def _tx_dll_file_changed(self, new_value):
         try:
             self.tx_dll_valid = False
             if new_value:
                 model = AMIModel(str(new_value))
                 self._tx_model = model
                 self.tx_dll_valid = True
-        except Exception as err:
+        except Exception as err:  # pylint: disable=broad-exception-caught
             error_message = f"Failed to open DLL/SO file!\n{err}"
             self.log(error_message, alert=True)
 
     def _rx_ibis_file_changed(self, new_value):
         self.status = f"Parsing IBIS file: {new_value}"
         dName = ""
         try:
@@ -1439,15 +992,15 @@
             dName = dirname(new_value)
             if self._rx_ibis.dll_file and self._rx_ibis.ami_file:
                 self.rx_dll_file = join(dName, self._rx_ibis.dll_file)
                 self.rx_ami_file = join(dName, self._rx_ibis.ami_file)
             else:
                 self.rx_dll_file = ""
                 self.rx_ami_file = ""
-        except Exception as err:
+        except Exception as err:  # pylint: disable=broad-exception-caught
             self.status = "IBIS file parsing error!"
             error_message = f"Failed to open and/or parse IBIS file!\n{err}"
             self.log(error_message, alert=True)
             raise
         self._rx_ibis_dir = dName
         self.status = "Done."
 
@@ -1464,52 +1017,54 @@
                     self.rx_use_getwave = True
                 if pcfg.fetch_param_val(["Reserved_Parameters", "Ts4file"]):
                     self.rx_has_ts4 = True
                 else:
                     self.rx_has_ts4 = False
                 self._rx_cfg = pcfg
                 self.rx_ami_valid = True
-        except Exception as err:
+        except Exception as err:  # pylint: disable=broad-exception-caught
             error_message = f"Failed to open and/or parse AMI file!\n{err}"
             self.log(error_message, alert=True)
 
     def _rx_dll_file_changed(self, new_value):
         try:
             self.rx_dll_valid = False
             if new_value:
                 model = AMIModel(str(new_value))
                 self._rx_model = model
                 self.rx_dll_valid = True
-        except Exception as err:
+        except Exception as err:  # pylint: disable=broad-exception-caught
             error_message = f"Failed to open DLL/SO file!\n{err}"
             self.log(error_message, alert=True)
 
     def _rx_use_ami_changed(self, new_value):
         if new_value:
-            self.use_dfe = False
+            self._btn_disable_fired()
 
     def check_pat_len(self):
+        "Validate chosen pattern length against number of bits being run."
         taps = self.pattern_
         pat_len = 2 * pow(2, max(taps))
         if pat_len > 5 * self.nbits:
             self.log(
                 "Accurate jitter decomposition may not be possible with the current configuration!\n \
 Try to keep Nbits & EyeBits > 10 * 2^n, where `n` comes from `PRBS-n`.",
                 alert=True,
             )
 
-    def _pattern_changed(self, new_value):
+    def _pattern_changed(self):
         self.check_pat_len()
 
-    def _nbits_changed(self, new_value):
+    def _nbits_changed(self):
         self.check_pat_len()
 
     # This function has been pulled outside of the standard Traits/UI "depends_on / @cached_property" mechanism,
     # in order to more tightly control when it executes. I wasn't able to get truly lazy evaluation, and
     # this was causing noticeable GUI slowdown.
+    # pylint: disable=attribute-defined-outside-init
     def calc_chnl_h(self):
         """Calculates the channel impulse response.
 
         Also sets, in 'self':
          - chnl_dly:
              group delay of channel
          - start_ix:
@@ -1520,53 +1075,59 @@
              channel frequency response
          - chnl_s:
              channel step response
          - chnl_p:
              channel pulse response
         """
 
-        t = self.t
+        t = self.t  # This time vector has NO relationship to `f`/`w`!
+        t_irfft = self.t_irfft  # This time vector IS related to `f`/`w`.
         f = self.f
         w = self.w
         nspui = self.nspui
         impulse_length = self.impulse_length * 1.0e-9
         Rs = self.rs
         Cs = self.cout * 1.0e-12
         RL = self.rin
         Cp = self.cin * 1.0e-12
-        CL = self.cac * 1.0e-6
+        # CL = self.cac * 1.0e-6  # pylint: disable=unused-variable
 
         ts = t[1]
-        len_t = len(t)
         len_f = len(f)
 
         # Form the pre-on-die S-parameter 2-port network for the channel.
         if self.use_ch_file:
-            ch_s2p_pre = import_channel(self.ch_file, ts, self.f)
+            ch_s2p_pre = import_channel(self.ch_file, ts, f, renumber=self.renumber)
+            self.log(str(ch_s2p_pre))
+            H = ch_s2p_pre.s21.s.flatten()
         else:
             # Construct PyBERT default channel model (i.e. - Howard Johnson's UTP model).
             # - Grab model parameters from PyBERT instance.
             l_ch = self.l_ch
             v0 = self.v0 * 3.0e8
             R0 = self.R0
             w0 = self.w0
             Rdc = self.Rdc
             Z0 = self.Z0
             Theta0 = self.Theta0
             # - Calculate propagation constant, characteristic impedance, and transfer function.
             gamma, Zc = calc_gamma(R0, w0, Rdc, Z0, v0, Theta0, w)
             self.Zc = Zc
-            H = exp(-l_ch * gamma)
+            H = exp(-l_ch * gamma)  # pylint: disable=invalid-unary-operand-type
             self.H = H
             # - Use the transfer function and characteristic impedance to form "perfectly matched" network.
             tmp = np.array(list(zip(zip(zeros(len_f), H), zip(H, zeros(len_f)))))
             ch_s2p_pre = rf.Network(s=tmp, f=f / 1e9, z0=Zc)
             # - And, finally, renormalize to driver impedance.
             ch_s2p_pre.renormalize(Rs)
-        ch_s2p_pre.name = "ch_s2p_pre"
+        try:
+            ch_s2p_pre.name = "ch_s2p_pre"
+        except Exception:  # pylint: disable=broad-exception-caught
+            print(f"ch_s2p_pre: {ch_s2p_pre}")
+            raise
         self.ch_s2p_pre = ch_s2p_pre
         ch_s2p = ch_s2p_pre  # In case neither set of on-die S-parameters is being invoked, below.
 
         # Augment w/ IBIS-AMI on-die S-parameters, if appropriate.
         def add_ondie_s(s2p, ts4f, isRx=False):
             """Add the effect of on-die S-parameters to channel network.
 
@@ -1578,15 +1139,17 @@
                 isRx(bool): True when Rx on-die S-params. are being added. (Default = False).
 
             Returns:
                 skrf.Network: Resultant 2-port network.
             """
             ts4N = rf.Network(ts4f)  # Grab the 4-port single-ended on-die network.
             ntwk = sdd_21(ts4N)  # Convert it to a differential, 2-port network.
-            ntwk2 = interp_s2p(ntwk, s2p.f)  # Interpolate to system freqs.
+            # Interpolate to system freqs.
+            ntwk2 = ntwk.extrapolate_to_dc().windowed(normalize=False).interpolate(
+                s2p.f, coords='polar', bounds_error=False, fill_value='extrapolate')
             if isRx:
                 res = s2p**ntwk2
             else:  # Tx
                 res = ntwk2**s2p
             return (res, ts4N, ntwk2)
 
         if self.tx_use_ibis:
@@ -1613,117 +1176,126 @@
                 ch_s2p, ts4N, ntwk = add_ondie_s(ch_s2p, fname, isRx=True)
                 self.ts4N = ts4N
                 self.ntwk = ntwk
         ch_s2p.name = "ch_s2p"
         self.ch_s2p = ch_s2p
 
         # Calculate channel impulse response.
+        # ToDo: Incorporate Tx output impedance.  # pylint: disable=fixme
         Zt = RL / (1 + 1j * w * RL * Cp)  # Rx termination impedance
         ch_s2p_term = ch_s2p.copy()
         ch_s2p_term_z0 = ch_s2p.z0.copy()
         ch_s2p_term_z0[:, 1] = Zt
         ch_s2p_term.renormalize(ch_s2p_term_z0)
         ch_s2p_term.name = "ch_s2p_term"
         self.ch_s2p_term = ch_s2p_term
         # We take the transfer function, H, to be a ratio of voltages.
         # So, we must normalize our (now generalized) S-parameters.
         chnl_H = ch_s2p_term.s21.s.flatten() * np.sqrt(ch_s2p_term.z0[:, 1] / ch_s2p_term.z0[:, 0])
-        chnl_h = irfft(chnl_H)
+        if self.use_window:
+            chnl_h = irfft(raised_cosine(chnl_H))
+        else:
+            chnl_h = irfft(chnl_H)
+        krnl = interp1d(t_irfft, chnl_h, kind="cubic",
+                        bounds_error=False, fill_value=0, assume_sorted=True)
+        temp = krnl(t)
+        chnl_h = temp * t[1] / t_irfft[1]
         chnl_dly = where(chnl_h == max(chnl_h))[0][0] * ts
 
         min_len = 20 * nspui
         max_len = 100 * nspui
         if impulse_length:
             min_len = max_len = impulse_length / ts
-        chnl_h, start_ix = trim_impulse(chnl_h, min_len=min_len, max_len=max_len)
-        temp = chnl_h.copy()
-        temp.resize(len(t), refcheck=False)
-        chnl_trimmed_H = fft(temp)
+        chnl_h, start_ix = trim_impulse(chnl_h, min_len=min_len, max_len=max_len,
+                                        front_porch=True, kept_energy=0.999)
+        krnl = interp1d(t[:len(chnl_h)], chnl_h, kind="cubic",
+                        bounds_error=False, fill_value=0, assume_sorted=True)
+        chnl_trimmed_H = rfft(krnl(t_irfft)) * t_irfft[1] / t[1]
 
         chnl_s = chnl_h.cumsum()
-        chnl_p = chnl_s - pad(chnl_s[:-nspui], (nspui, 0), "constant", constant_values=(0, 0))
+        chnl_p = chnl_s - pad(chnl_s[:-nspui], (nspui, 0), "constant", constant_values=(0, 0))  # pylint: disable=invalid-unary-operand-type
 
         self.chnl_h = chnl_h
         self.len_h = len(chnl_h)
         self.chnl_dly = chnl_dly
         self.chnl_H = chnl_H
+        self.chnl_H_raw = H
         self.chnl_trimmed_H = chnl_trimmed_H
         self.start_ix = start_ix
-        self.t_ns_chnl = array(t[start_ix : start_ix + len(chnl_h)]) * 1.0e9
+        self.t_ns_chnl = array(t[start_ix: start_ix + len(chnl_h)]) * 1.0e9
         self.chnl_s = chnl_s
         self.chnl_p = chnl_p
 
         return chnl_h
 
     def simulate(self, initial_run=False, update_plots=True):
         """Run all queued simulations."""
         # Running the simulation will fill in the required data structure.
         my_run_simulation(self, initial_run=initial_run, update_plots=update_plots)
         # Once the required data structure is filled in, we can create the plots.
-        make_plots(self, n_dfe_taps=gNtaps)
+        make_plots(self, n_dfe_taps=len(self.dfe_tap_tuners))
 
     def load_configuration(self, filepath: Path):
         """Load in a configuration into pybert.
 
         Args:
             filepath: A full filepath include the suffix.
         """
         try:
             PyBertCfg.load_from_file(filepath, self)
             self.cfg_file = filepath
             self.status = "Loaded configuration."
         except InvalidFileType:
             self.log("This filetype is not currently supported.")
-        except Exception as exp:
+        except Exception as err:  # pylint: disable=broad-exception-caught
             self.log("Failed to load configuration. See the console for more detail.")
-            self.log(str(exp))
+            self.log(str(err))
 
     def save_configuration(self, filepath: Path):
         """Save out a configuration from pybert.
 
         Args:
             filepath: A full filepath include the suffix.
         """
         try:
             PyBertCfg(self, time.asctime(), VERSION).save(filepath)
             self.cfg_file = filepath
             self.status = "Configuration saved."
         except InvalidFileType:
             self.log("This filetype is not currently supported. Please try again as a yaml file.")
-        except Exception as exp:
-            self.log("Failed to save current user configuration. See the console for more detail.")
-            self.log(str(exp))
+        except Exception as err:  # pylint: disable=broad-exception-caught
+            self.log(f"Failed to save configuration:\n\t{err}", alert=True)
 
     def load_results(self, filepath: Path):
         """Load results from a file into pybert.
 
         Args:
             filepath: A full filepath include the suffix.
         """
         try:
             PyBertData.load_from_file(filepath, self)
             self.data_file = filepath
             self.status = "Loaded results."
-        except Exception as exp:
+        except Exception as err:  # pylint: disable=broad-exception-caught
             self.log("Failed to load results from file. See the console for more detail.")
-            self.log(str(exp))
+            self.log(str(err))
 
     def save_results(self, filepath: Path):
         """Save the existing results to a pickle file.
 
         Args:
             filepath: A full filepath include the suffix.
         """
         try:
             PyBertData(self, time.asctime(), VERSION).save(filepath)
             self.data_file = filepath
             self.status = "Saved results."
-        except Exception as exp:
+        except Exception as err:  # pylint: disable=broad-exception-caught
             self.log("Failed to save results to file. See the console for more detail.")
-            self.log(str(exp))
+            self.log(str(err))
 
     def clear_reference_from_plots(self):
         """If any plots have ref in the name, delete them and then regenerate the plots.
 
         If we don't actually delete any data, skip regenerating the plots.
         """
         atleast_one_reference_removed = False
@@ -1733,19 +1305,51 @@
                 try:
                     atleast_one_reference_removed = True
                     self.plotdata.del_data(reference_plot)
                 except KeyError:
                     pass
 
         if atleast_one_reference_removed:
-            make_plots(self, n_dfe_taps=gNtaps)
+            make_plots(self, n_dfe_taps=len(self.dfe_tap_tuners))
 
     def log_information(self):
         """Log the system information."""
-        from traits.etsconfig.api import ETSConfig
         self.log(f"System: {platform.system()} {platform.release()}")
         self.log(f"Python Version: {platform.python_version()}")
         self.log(f"PyBERT Version: {VERSION}")
         self.log(f"PyAMI Version: {PyAMI_VERSION}")
         self.log(f"GUI Toolkit: {ETSConfig.toolkit}")
         self.log(f"Kiva Backend: {ETSConfig.kiva_backend}")
-        # self.log(f"Pixel Scale: {self.trait_view().window.base_pixel_scale}")
+
+    _tx_ibis = Instance(IBISModel)
+    _tx_ibis_dir = ""
+    _tx_cfg = Instance(AMIParamConfigurator)
+    _tx_model = Instance(AMIModel)
+    _rx_ibis = Instance(IBISModel)
+    _rx_ibis_dir = ""
+    _rx_cfg = Instance(AMIParamConfigurator)
+    _rx_model = Instance(AMIModel)
+
+    isi_chnl = 0
+    dcd_chnl = 0
+    pj_chnl = 0
+    rj_chnl = 0
+    pjDD_chnl = 0
+    rjDD_chnl = 0
+    isi_tx = 0
+    dcd_tx = 0
+    pj_tx = 0
+    rj_tx = 0
+    pjDD_tx = 0
+    rjDD_tx = 0
+    isi_ctle = 0
+    dcd_ctle = 0
+    pj_ctle = 0
+    rj_ctle = 0
+    pjDD_ctle = 0
+    rjDD_ctle = 0
+    isi_dfe = 0
+    dcd_dfe = 0
+    pj_dfe = 0
+    rj_dfe = 0
+    pjDD_dfe = 0
+    rjDD_dfe = 0
```

### Comparing `PipBERT-4.1.0/src/pybert/results.py` & `pipbert-6.1.0/src/pybert/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
         Args:
             filepath: The full filepath including the extension to save too.
         """
         with open(filepath, "wb") as the_file:
             pickle.dump(self, the_file)
 
+    # pylint: disable=too-many-branches
     @staticmethod
     def load_from_file(filepath: Union[str, Path], pybert):
         """Recall all the results from a file and load them as reference plots.
 
         Confirms that the file actually exists and attempts to load back the
         graphs as reference plots in pybert.
 
@@ -97,15 +98,15 @@
         if not filepath.exists():
             raise FileNotFoundError(f"{filepath} does not exist.")
 
         # Right now the loads deserialize back into a `PyBertData` class.
         with open(filepath, "rb") as the_file:
             user_results = pickle.load(the_file)
         if not isinstance(user_results, PyBertData):
-            raise Exception("The data structure read in is NOT of type: ArrayPlotData!")
+            raise ValueError("The data structure read in is NOT of type: ArrayPlotData!")
 
         # Load the reference plots.
         for prop, value in user_results.the_data.arrays.items():
             pybert.plotdata.set_data(prop + "_ref", value)
 
         # Add reference plots, if necessary.
         # - time domain
```

### Comparing `PipBERT-4.1.0/src/pybert/solvers/__init__.py` & `pipbert-6.1.0/src/pybert/solvers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,11 @@
 so as to support solvers, which may need extra data/support files.
 
 Copyright (c) 2019 by David Banas; all rights reserved World wide.
 """
 __all__ = [
     "simbeor",
 ]  # Should contain the name of each submodule.
-from . import *  # Makes each solver package available as: solvers.simbeor, etc.
+# from . import *  # Makes each solver package available as: solvers.simbeor, etc.
+# Actually, the above line causes a self-import.
+# The `__all__` definition, above, should be all we need, such that
+# `from pybert.solvers import *` does the right thing.
```

### Comparing `PipBERT-4.1.0/src/pybert/solvers/simbeor/__init__.py` & `pipbert-6.1.0/src/pybert/solvers/simbeor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # pylint: disable=undefined-variable
 # type: ignore
+# flake8: noqa
+
 """Initialization file for Simbeor solver.
 
 .. moduleauthor:: David Banas <capn.freako@gmail.com>
 
 Original Author: David Banas <capn.freako@gmail.com>
 
 Original Date:   20 September 2019
@@ -22,23 +24,24 @@
 
 import numpy as np
 
 from pybert.solvers import solver as slvr
 
 sdkdir = os.environ.get("SIMBEOR_SDK")
 __path__ = [osp.join(sdkdir, "python")]
-__all__ = [
-    "simbeor",
-]  # Should contain the name of each submodule.
-from . import *  # Makes each submodule available as: pybert.solvers.simbeor.simbeor, etc.
+# __all__ = [
+#     "simbeor",
+# ]  # Should contain the name of each submodule.
+# from . import *  # Makes each submodule available as: pybert.solvers.simbeor.simbeor, etc.
 
 
-class Solver(slvr.Solver):
+class Solver(slvr.Solver):  # pylint: disable=too-few-public-methods
     """Simbeor-specific override of `pybert.solver.Solver` class."""
 
+    # pylint: disable=too-many-arguments,too-many-locals,too-many-branches,too-many-statements,unused-argument
     def solve(
         self,
         ch_type: slvr.ChType = "microstrip_se",  #: Channel cross-sectional configuration.
         diel_const: float = 4.0,  #: Dielectric constant of substrate (rel.).
         loss_tan: float = 0.02,  #: Loss tangent at ``des_freq``.
         des_freq: float = 1.0e9,  #: Frequency at which ``diel_const`` and ``loss_tan`` are quoted (Hz).
         thickness: float = 0.036,  #: Trace thickness (mm).
```

### Comparing `PipBERT-4.1.0/src/pybert/solvers/solver.py` & `pipbert-6.1.0/src/pybert/solvers/solver.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import List, Tuple
 
 ChType = Enum("ChType", "microstrip_se microstrip_diff stripline_se stripline_diff")
 
 
-class Solver(ABC):
+class Solver(ABC):  # pylint: disable=too-few-public-methods
     """Abstract base class providing a consistent interface to channel
     solver."""
 
     @abstractmethod
-    def solve(
+    def solve(  # pylint: disable=too-many-arguments
         self,
         ch_type: str = "microstrip_se",  #: Channel cross-sectional configuration.
         diel_const: float = 4.3,  #: Dielectric constant of substrate at ``des_freq`` (rel.).
         loss_tan: float = 0.02,  #: Loss tangent at ``des_freq``.
         des_freq: float = 1.0e9,  #: Frequency at which ``diel_const`` and ``loss_tan`` are quoted (Hz).
         thickness: float = 0.036,  #: Trace thickness (mm).
         width: float = 0.254,  #: Trace width (mm).
         height: float = 0.127,  #: Trace height above/below ground plane (mm).
         separation: float = 0.508,  #: Trace separation (mm).
         roughness: float = 0.004,  #: Trace surface roughness (mm-rms).
-        fs: List[float] = None,  #: Angular frequency sample points (Hz).
+        fs: List[float] = [],  #: Angular frequency sample points (Hz).  # pylint: disable=dangerous-default-value
         lic_path: str = "",  #: Path to license file.
         lic_name: str = "",  #: Name of license type (if needed by solver).
         prj_name: str = "",  #: Name of project (if needed by solver).
     ) -> Tuple[List[complex], List[complex], List[float]]:
         """Solves a particular channel cross-section.
 
         Returns:
```

### Comparing `PipBERT-4.1.0/tests/test_basic.py` & `pipbert-6.1.0/tests/test_basic.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,9 +48,9 @@
     def test_adapt(self, dut):
         """Test DFE lock, by ensuring that last 20% of all coefficient vectors
         are stable to within +/-20% of their mean."""
         _weights = dut.adaptation  # rows = step; cols = tap
         _ws = np.array(list(zip(*_weights[4 * len(_weights) // 5 :])))  # zip(*x) = unzip(x)
         _means = list(map(lambda xs: sum(xs) / len(xs), _ws))
         assert all(
-            map(lambda pr: all(abs(pr[0] - pr[1]) / pr[1] < 0.2), zip(_ws, _means))
-        ), "DFE adaptation is unstable!"
+            list(map(lambda pr: all(abs(pr[0] - pr[1]) / pr[1] < 0.2), zip(_ws, _means)))
+        ), f"DFE adaptation is unstable! {max(_ws[-1])} {min(_ws[-1])}"
```

### Comparing `PipBERT-4.1.0/tests/test_command_line.py` & `pipbert-6.1.0/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `PipBERT-4.1.0/tests/test_loading_and_saving.py` & `pipbert-6.1.0/tests/test_loading_and_saving.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     dut.load_configuration(filepath_converter(save_file))
 
     # For everything saved in configuration, make sure they match.
     # All items should exist in both, so fail if one isn't found.
     for name in user_config.__dict__.keys():
         # These are handled differently so skip them.
-        if name not in ["tx_taps", "tx_tap_tuners", "version", "date_created"]:
+        if name not in ["tx_taps", "tx_tap_tuners", "dfe_tap_tuners", "version", "date_created"]:
             # Test the values
             assert getattr(user_config, name) == getattr(dut, name)
 
 
 @pytest.mark.usefixtures("dut")
 def test_load_config_from_pickle(dut, tmp_path: Path):
     """Make sure that pybert can correctly load a pickle file."""
```

