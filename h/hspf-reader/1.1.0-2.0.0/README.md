# Comparing `tmp/hspf_reader-1.1.0.tar.gz` & `tmp/hspf_reader-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspf_reader-1.1.0.tar", last modified: Wed May 29 02:22:09 2024, max compression
+gzip compressed data, was "hspf_reader-2.0.0.tar", last modified: Sat Jun  1 22:50:45 2024, max compression
```

## Comparing `hspf_reader-1.1.0.tar` & `hspf_reader-2.0.0.tar`

### file list

```diff
@@ -1,60 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.978034 hspf_reader-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.966035 hspf_reader-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.966035 hspf_reader-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.github/workflows/clean-workflow-runs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.github/workflows/pypi-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/BADGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-29 02:22:09.978034 hspf_reader-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.966035 hspf_reader-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/function_summary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 02:22:09.978034 hspf_reader-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.962035 hspf_reader-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.970034 hspf_reader-1.1.0/src/hspf_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/src/hspf_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/src/hspf_reader/hspf_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.974034 hspf_reader-1.1.0/src/hspf_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 02:22:09.000000 hspf_reader-1.1.0/src/hspf_reader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:09.974034 hspf_reader-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    81920 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data.wdm
--rw-r--r--   0 runner    (1001) docker     (127)   822321 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data_6b_np1.hbn
--rw-r--r--   0 runner    (1001) docker     (127)    62131 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data_plotgen.plt
--rw-r--r--   0 runner    (1001) docker     (127)   172779 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data_wdm_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)   264240 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data_wdm_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)   822321 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/data_yearly.hbn
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/debug_hspf_reader
--rw-r--r--   0 runner    (1001) docker     (127)    30250 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/sunspot_area.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15138 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/sunspot_area_with_missing.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/test_hbn.py
--rw-r--r--   0 runner    (1001) docker     (127)    35532 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/test_plotgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-29 02:22:02.000000 hspf_reader-1.1.0/tests/test_wdm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.633499 hspf_reader-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.621499 hspf_reader-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.621499 hspf_reader-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/.github/workflows/clean-workflow-runs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/BADGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-06-01 22:50:45.633499 hspf_reader-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.621499 hspf_reader-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/docs/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/docs/function_summary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:50:45.633499 hspf_reader-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.617498 hspf_reader-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.621499 hspf_reader-2.0.0/src/hspf_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/src/hspf_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/src/hspf_reader/hspf_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.617498 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.621499 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.617498 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.621499 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.625499 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/readers/hbn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/readers/plotgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/readers/wdm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.625499 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/tssplit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-06-01 22:50:37.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/tssplit/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.625499 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/tssplit/tssplit/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-01 22:50:37.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/tssplit/tssplit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-06-01 22:50:37.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/tssplit/tssplit/tssplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89991 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/src/toolbox_utils/tsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.625499 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_asbestfreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_common_kwds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_date_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_dateparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_hbn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_make_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_period_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34649 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_plotgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_range_to_numlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_tssplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-06-01 22:50:36.000000 hspf_reader-2.0.0/src/hspf_reader/toolbox_utils/tests/test_wdm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.633499 hspf_reader-2.0.0/src/hspf_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-06-01 22:50:45.000000 hspf_reader-2.0.0/src/hspf_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-06-01 22:50:45.000000 hspf_reader-2.0.0/src/hspf_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:50:45.000000 hspf_reader-2.0.0/src/hspf_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 22:50:45.000000 hspf_reader-2.0.0/src/hspf_reader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-06-01 22:50:45.000000 hspf_reader-2.0.0/src/hspf_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-01 22:50:45.000000 hspf_reader-2.0.0/src/hspf_reader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:45.633499 hspf_reader-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81920 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/data.wdm
+-rw-r--r--   0 runner    (1001) docker     (127)   822321 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/data_6b_np1.hbn
+-rw-r--r--   0 runner    (1001) docker     (127)    62131 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/data_plotgen.plt
+-rw-r--r--   0 runner    (1001) docker     (127)   172779 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/data_wdm_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   264240 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/data_wdm_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   822321 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/data_yearly.hbn
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/debug_hspf_reader
+-rw-r--r--   0 runner    (1001) docker     (127)    30250 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/sunspot_area.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15138 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/sunspot_area_with_missing.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/test_hbn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35532 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/test_plotgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-06-01 22:50:35.000000 hspf_reader-2.0.0/tests/test_wdm.py
```

### Comparing `hspf_reader-1.1.0/.github/workflows/pypi-package.yml` & `hspf_reader-2.0.0/.github/workflows/pypi-package.yml`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         permissions:
             # IMPORTANT: this permission is mandatory for trusted publishing
             id-token: write
 
         steps:
             - name: Checkout source
               uses: actions/checkout@v4
+              with:
+                  submodules: recursive
 
             - name: Build sdist and wheel
               run: |
                   python -m pip install build
                   python -m build
 
             - name: Download artifact
```

### Comparing `hspf_reader-1.1.0/.github/workflows/tests.yml` & `hspf_reader-2.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/.pre-commit-config.yaml` & `hspf_reader-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/.sourcery.yaml` & `hspf_reader-2.0.0/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/BADGES.rst` & `hspf_reader-2.0.0/BADGES.rst`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/CHANGELOG.md` & `hspf_reader-2.0.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+## v2.0.0 (2024-06-01)
+
 ## v1.1.0 (2024-05-28)
 
 ### Feat
 
 - include local copy of toolbox_utils using git submodules
 - reworked the about functions
```

### Comparing `hspf_reader-1.1.0/CONTRIBUTING.rst` & `hspf_reader-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/LICENSE.txt` & `hspf_reader-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/PKG-INFO` & `hspf_reader-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspf_reader
-Version: 1.1.0
+Version: 2.0.0
 Summary: Command line script and Python library to read HSPF WDM, binary, and plotgen time series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hspf_reader/docs/index.html#hspf_reader-documentation
 Project-URL: github, https://github.com/timcera/hspf_reader
 Project-URL: bitbucket, https://bitbucket.org/timcera/hspf_reader/src/main/
 Keywords: time-series,hspf,simulation,hydrology,hydrologic,python,cli,command line,script,cli-application
```

### Comparing `hspf_reader-1.1.0/README.rst` & `hspf_reader-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/docs/Makefile` & `hspf_reader-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/docs/conf.py` & `hspf_reader-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/docs/make.bat` & `hspf_reader-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/pyproject.toml` & `hspf_reader-2.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     ".ipynb_checkpoints/*"
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "1.1.0"
+version = "2.0.0"
 version_files = ["VERSION"]
 
 [tool.isort]
 profile = "black"
 
 [tool.jupytext]
 formats = "ipynb,py:percent"
```

### Comparing `hspf_reader-1.1.0/src/hspf_reader/hspf_reader.py` & `hspf_reader-2.0.0/src/hspf_reader/hspf_reader.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/src/hspf_reader.egg-info/PKG-INFO` & `hspf_reader-2.0.0/src/hspf_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspf_reader
-Version: 1.1.0
+Version: 2.0.0
 Summary: Command line script and Python library to read HSPF WDM, binary, and plotgen time series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hspf_reader/docs/index.html#hspf_reader-documentation
 Project-URL: github, https://github.com/timcera/hspf_reader
 Project-URL: bitbucket, https://bitbucket.org/timcera/hspf_reader/src/main/
 Keywords: time-series,hspf,simulation,hydrology,hydrologic,python,cli,command line,script,cli-application
```

### Comparing `hspf_reader-1.1.0/tests/data.wdm` & `hspf_reader-2.0.0/tests/data.wdm`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/tests/data_6b_np1.hbn` & `hspf_reader-2.0.0/tests/data_6b_np1.hbn`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/tests/data_plotgen.plt` & `hspf_reader-2.0.0/tests/data_plotgen.plt`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/tests/data_wdm_1.csv` & `hspf_reader-2.0.0/tests/data_wdm_1.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/tests/data_wdm_2.csv` & `hspf_reader-2.0.0/tests/data_wdm_2.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/tests/data_yearly.hbn` & `hspf_reader-2.0.0/tests/data_yearly.hbn`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/tests/sunspot_area.csv` & `hspf_reader-2.0.0/tests/sunspot_area.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/tests/sunspot_area_with_missing.csv` & `hspf_reader-2.0.0/tests/sunspot_area_with_missing.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/tests/test_hbn.py` & `hspf_reader-2.0.0/tests/test_hbn.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/tests/test_plotgen.py` & `hspf_reader-2.0.0/tests/test_plotgen.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.1.0/tests/test_wdm.py` & `hspf_reader-2.0.0/tests/test_wdm.py`

 * *Files identical despite different names*

