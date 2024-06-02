# Comparing `tmp/sparecores_crawler-0.1.3.tar.gz` & `tmp/sparecores_crawler-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparecores_crawler-0.1.3.tar", last modified: Thu May  9 22:02:51 2024, max compression
+gzip compressed data, was "sparecores_crawler-0.1.4.tar", last modified: Sun Jun  2 20:18:26 2024, max compression
```

## Comparing `sparecores_crawler-0.1.3.tar` & `sparecores_crawler-0.1.4.tar`

### file list

```diff
@@ -1,46 +1,51 @@
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.774617 sparecores_crawler-0.1.3/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    16726 2023-12-08 22:12:52.000000 sparecores_crawler-0.1.3/LICENSE
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       53 2024-04-12 16:09:18.000000 sparecores_crawler-0.1.3/MANIFEST.in
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7725 2024-05-09 22:02:51.774617 sparecores_crawler-0.1.3/PKG-INFO
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5326 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/README.md
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3737 2024-05-07 11:57:49.000000 sparecores_crawler-0.1.3/pyproject.toml
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       38 2024-05-09 22:02:51.774617 sparecores_crawler-0.1.3/setup.cfg
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.761283 sparecores_crawler-0.1.3/src/
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.764617 sparecores_crawler-0.1.3/src/sc_crawler/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)        0 2024-02-14 13:12:38.000000 sparecores_crawler-0.1.3/src/sc_crawler/__init__.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.764617 sparecores_crawler-0.1.3/src/sc_crawler/alembic/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2977 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic/env.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.764617 sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5929 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    68592 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     9694 2024-05-07 21:26:31.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/f6bf6152039a_v0_1_3_step2.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    13080 2024-05-09 21:10:36.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/f6edf4a96a78_v0_1_3_step1.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3618 2024-04-12 15:45:00.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic.ini
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1185 2024-04-12 16:10:05.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic_helpers.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    22486 2024-04-12 16:49:26.000000 sparecores_crawler-0.1.3/src/sc_crawler/cli.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6780 2024-04-10 22:14:16.000000 sparecores_crawler-0.1.3/src/sc_crawler/insert.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     8517 2024-04-04 14:01:05.000000 sparecores_crawler-0.1.3/src/sc_crawler/logger.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3624 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.3/src/sc_crawler/lookup.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2201 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/src/sc_crawler/str_utils.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    20637 2024-05-07 11:04:13.000000 sparecores_crawler-0.1.3/src/sc_crawler/table_bases.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     4705 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/src/sc_crawler/table_fields.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    17017 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.3/src/sc_crawler/tables.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2730 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/src/sc_crawler/tables_scd.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5156 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.3/src/sc_crawler/utils.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.767950 sparecores_crawler-0.1.3/src/sc_crawler/vendors/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      116 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.3/src/sc_crawler/vendors/__init__.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    42164 2024-05-09 20:10:59.000000 sparecores_crawler-0.1.3/src/sc_crawler/vendors/aws.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    35732 2024-05-09 19:59:03.000000 sparecores_crawler-0.1.3/src/sc_crawler/vendors/gcp.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    11349 2024-05-09 20:06:56.000000 sparecores_crawler-0.1.3/src/sc_crawler/vendors/hcloud.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1520 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.3/src/sc_crawler/vendors/vendors.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.771283 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7725 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/PKG-INFO
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1164 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)        1 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       50 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/entry_points.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      581 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/requires.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       11 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/top_level.txt
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.767950 sparecores_crawler-0.1.3/tests/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1391 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/tests/test_schemas.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1316 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/tests/test_str_utils.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1216 2024-03-25 14:01:48.000000 sparecores_crawler-0.1.3/tests/test_utils.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-06-02 20:18:26.798451 sparecores_crawler-0.1.4/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    16726 2023-12-08 22:12:52.000000 sparecores_crawler-0.1.4/LICENSE
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       53 2024-04-12 16:09:18.000000 sparecores_crawler-0.1.4/MANIFEST.in
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7749 2024-06-02 20:18:26.798451 sparecores_crawler-0.1.4/PKG-INFO
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5326 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.4/README.md
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3751 2024-06-02 13:32:13.000000 sparecores_crawler-0.1.4/pyproject.toml
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       38 2024-06-02 20:18:26.798451 sparecores_crawler-0.1.4/setup.cfg
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-06-02 20:18:26.781784 sparecores_crawler-0.1.4/src/
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-06-02 20:18:26.788451 sparecores_crawler-0.1.4/src/sc_crawler/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)        0 2024-02-14 13:12:38.000000 sparecores_crawler-0.1.4/src/sc_crawler/__init__.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-06-02 20:18:26.788451 sparecores_crawler-0.1.4/src/sc_crawler/alembic/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2977 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.4/src/sc_crawler/alembic/env.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-06-02 20:18:26.791784 sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      993 2024-06-01 23:00:26.000000 sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/19b010d3acdf_v1_1_4_memory_rename.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5929 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6637 2024-06-01 23:00:26.000000 sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/85c7256cc390_v1_1_4_add_cpu_ram_gpu_columns.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    68592 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    10617 2024-05-30 23:07:06.000000 sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/c8d2054e68eb_v1_1_4_benchmarks.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    75922 2024-06-02 15:14:20.000000 sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/e382f30fad09_v1_2_0_name_constraints.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     9694 2024-05-29 09:18:32.000000 sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/f6bf6152039a_v0_1_3_step2.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    12453 2024-05-29 09:18:32.000000 sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/f6edf4a96a78_v0_1_3_step1.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3618 2024-04-12 15:45:00.000000 sparecores_crawler-0.1.4/src/sc_crawler/alembic.ini
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1185 2024-04-12 16:10:05.000000 sparecores_crawler-0.1.4/src/sc_crawler/alembic_helpers.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    22647 2024-06-02 13:32:13.000000 sparecores_crawler-0.1.4/src/sc_crawler/cli.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6780 2024-04-10 22:14:16.000000 sparecores_crawler-0.1.4/src/sc_crawler/insert.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    14784 2024-06-01 23:07:44.000000 sparecores_crawler-0.1.4/src/sc_crawler/inspector.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     8517 2024-04-04 14:01:05.000000 sparecores_crawler-0.1.4/src/sc_crawler/logger.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    12589 2024-06-01 13:51:56.000000 sparecores_crawler-0.1.4/src/sc_crawler/lookup.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2201 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.4/src/sc_crawler/str_utils.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    24180 2024-06-02 13:33:15.000000 sparecores_crawler-0.1.4/src/sc_crawler/table_bases.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5409 2024-06-01 22:56:36.000000 sparecores_crawler-0.1.4/src/sc_crawler/table_fields.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    19144 2024-06-02 13:32:13.000000 sparecores_crawler-0.1.4/src/sc_crawler/tables.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2730 2024-06-02 13:32:13.000000 sparecores_crawler-0.1.4/src/sc_crawler/tables_scd.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5156 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.4/src/sc_crawler/utils.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-06-02 20:18:26.791784 sparecores_crawler-0.1.4/src/sc_crawler/vendors/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      116 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.4/src/sc_crawler/vendors/__init__.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    42171 2024-06-02 13:32:13.000000 sparecores_crawler-0.1.4/src/sc_crawler/vendors/aws.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    35746 2024-06-02 20:09:56.000000 sparecores_crawler-0.1.4/src/sc_crawler/vendors/gcp.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    11356 2024-06-02 13:32:13.000000 sparecores_crawler-0.1.4/src/sc_crawler/vendors/hcloud.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1520 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.4/src/sc_crawler/vendors/vendors.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-06-02 20:18:26.795118 sparecores_crawler-0.1.4/src/sparecores_crawler.egg-info/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7749 2024-06-02 20:18:26.000000 sparecores_crawler-0.1.4/src/sparecores_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1478 2024-06-02 20:18:26.000000 sparecores_crawler-0.1.4/src/sparecores_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)        1 2024-06-02 20:18:26.000000 sparecores_crawler-0.1.4/src/sparecores_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       50 2024-06-02 20:18:26.000000 sparecores_crawler-0.1.4/src/sparecores_crawler.egg-info/entry_points.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      590 2024-06-02 20:18:26.000000 sparecores_crawler-0.1.4/src/sparecores_crawler.egg-info/requires.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       11 2024-06-02 20:18:26.000000 sparecores_crawler-0.1.4/src/sparecores_crawler.egg-info/top_level.txt
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-06-02 20:18:26.795118 sparecores_crawler-0.1.4/tests/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1391 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.4/tests/test_schemas.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1316 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.4/tests/test_str_utils.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1216 2024-03-25 14:01:48.000000 sparecores_crawler-0.1.4/tests/test_utils.py
```

### Comparing `sparecores_crawler-0.1.3/LICENSE` & `sparecores_crawler-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/PKG-INFO` & `sparecores_crawler-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparecores-crawler
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pull and standardize data on cloud compute resources.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-crawler
 Project-URL: issues, https://github.com/SpareCores/sc-crawler/issues
 Project-URL: documentation, https://sparecores.github.io/sc-crawler/
 Project-URL: homepage, https://sparecores.com
@@ -16,14 +16,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: alembic
 Requires-Dist: cachier
 Requires-Dist: pydantic
 Requires-Dist: pydantic_extra_types
+Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: sqlmodel
 Requires-Dist: typer
 Provides-Extra: mkdocs
 Requires-Dist: markdown==3.5.2; extra == "mkdocs"
 Requires-Dist: mkdocs; extra == "mkdocs"
 Requires-Dist: mkdocs-material[imaging]==9.5.13; extra == "mkdocs"
```

### Comparing `sparecores_crawler-0.1.3/README.md` & `sparecores_crawler-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/pyproject.toml` & `sparecores_crawler-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sparecores-crawler"
-version = "0.1.3"
+version = "0.1.4"
 requires-python = ">= 3.7"
 dependencies = [
   "alembic",
   "cachier",
   "pydantic",
   "pydantic_extra_types",
+  "requests",
   "rich",
   "sqlmodel",
   "typer",
 ]
 authors = [
   { name="Attila Nagy" },
   { name="Gergely Daroczi" },
```

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/alembic/env.py` & `sparecores_crawler-0.1.4/src/sc_crawler/alembic/env.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py` & `sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py` & `sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/f6bf6152039a_v0_1_3_step2.py` & `sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/f6bf6152039a_v0_1_3_step2.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/f6edf4a96a78_v0_1_3_step1.py` & `sparecores_crawler-0.1.4/src/sc_crawler/alembic/versions/f6edf4a96a78_v0_1_3_step1.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,83 +40,48 @@
         ),
         insert_after="api_reference",
     )
 
 
 # need to provide the table schema for offline mode support
 meta = sa.MetaData()
-enum_status = sa.Enum("ACTIVE", "INACTIVE", name="status").with_variant(
-    sa.dialects.postgresql.ENUM("ACTIVE", "INACTIVE", name="status", create_type=False),
-    "postgresql",
-)
-enum_cpuallocation = sa.Enum(
-    "SHARED", "BURSTABLE", "DEDICATED", name="cpuallocation"
-).with_variant(
-    sa.dialects.postgresql.ENUM(
-        "SHARED", "BURSTABLE", "DEDICATED", name="cpuallocation", create_type=False
-    ),
-    "postgresql",
-)
-enum_cpuarchitecture = sa.Enum(
-    "ARM64", "ARM64_MAC", "I386", "X86_64", "X86_64_MAC", name="cpuarchitecture"
-).with_variant(
-    sa.dialects.postgresql.ENUM(
-        "ARM64",
-        "ARM64_MAC",
-        "I386",
-        "X86_64",
-        "X86_64_MAC",
-        name="cpuarchitecture",
-        create_type=False,
-    ),
-    "postgresql",
-)
-enum_storage_type = enum_storage_type = sa.Enum(
-    "HDD", "SSD", "NVME_SSD", "NETWORK", name="storagetype"
-).with_variant(
-    sa.dialects.postgresql.ENUM(
-        "HDD",
-        "SSD",
-        "NVME_SSD",
-        "NETWORK",
-        name="storagetype",
-        create_type=False,
-    ),
-    "postgresql",
-)
 datacenter_table = sa.Table(
     "datacenter_scd" if op.get_context().config.attributes.get("scd") else "datacenter",
     meta,
     sa.Column("vendor_id", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
     sa.Column("datacenter_id", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
     sa.Column("name", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
     sa.Column("aliases", sa.JSON(), nullable=False),
     sa.Column("country_id", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
     sa.Column("state", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
     sa.Column("city", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
     sa.Column("address_line", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
     sa.Column("zip_code", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
     sa.Column("founding_year", sa.Integer(), nullable=True),
     sa.Column("green_energy", sa.Boolean(), nullable=True),
-    sa.Column("status", enum_status, nullable=False),
+    sa.Column("status", sa.Enum("ACTIVE", "INACTIVE", name="status"), nullable=False),
     sa.Column("observed_at", sa.DateTime(), nullable=False),
     sa.ForeignKeyConstraint(["country_id"], ["country.country_id"]),
     sa.ForeignKeyConstraint(["vendor_id"], ["vendor.vendor_id"]),
     sa.PrimaryKeyConstraint("vendor_id", "datacenter_id", "observed_at")
     if op.get_context().config.attributes.get("scd")
     else sa.PrimaryKeyConstraint("vendor_id", "datacenter_id"),
 )
 zone_table = sa.Table(
     "zone_scd" if op.get_context().config.attributes.get("scd") else "zone",
     meta,
     sa.Column("vendor_id", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
     sa.Column("datacenter_id", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
     sa.Column("zone_id", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
     sa.Column("name", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
-    sa.Column("status", enum_status, nullable=False),
+    sa.Column(
+        "status",
+        sa.Enum("ACTIVE", "INACTIVE", name="status"),
+        nullable=False,
+    ),
     sa.Column("observed_at", sa.DateTime(), nullable=False),
     sa.ForeignKeyConstraint(
         ["vendor_id"],
         ["vendor.vendor_id"],
     ),
     sa.PrimaryKeyConstraint("vendor_id", "datacenter_id", "zone_id", "observed_at")
     if op.get_context().config.attributes.get("scd")
@@ -127,37 +92,55 @@
     meta,
     sa.Column("vendor_id", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
     sa.Column("server_id", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
     sa.Column("name", sqlmodel.sql.sqltypes.AutoString(), nullable=False),
     sa.Column("description", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
     sa.Column("vcpus", sa.Integer(), nullable=False),
     sa.Column("hypervisor", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
-    sa.Column("cpu_allocation", enum_cpuallocation, nullable=False),
+    sa.Column(
+        "cpu_allocation",
+        sa.Enum("SHARED", "BURSTABLE", "DEDICATED", name="cpuallocation"),
+        nullable=False,
+    ),
     sa.Column("cpu_cores", sa.Integer(), nullable=True),
     sa.Column("cpu_speed", sa.Float(), nullable=True),
-    sa.Column("cpu_architecture", enum_cpuarchitecture, nullable=False),
+    sa.Column(
+        "cpu_architecture",
+        sa.Enum(
+            "ARM64",
+            "ARM64_MAC",
+            "I386",
+            "X86_64",
+            "X86_64_MAC",
+            name="cpuarchitecture",
+        ),
+        nullable=False,
+    ),
     sa.Column("cpu_manufacturer", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
     sa.Column("cpu_family", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
     sa.Column("cpu_model", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
     sa.Column("cpus", sa.JSON(), nullable=False),
     sa.Column("memory", sa.Integer(), nullable=False),
     sa.Column("gpu_count", sa.Integer(), nullable=False),
     sa.Column("gpu_memory_min", sa.Integer(), nullable=True),
     sa.Column("gpu_memory_total", sa.Integer(), nullable=True),
     sa.Column("gpu_manufacturer", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
     sa.Column("gpu_model", sqlmodel.sql.sqltypes.AutoString(), nullable=True),
     sa.Column("gpus", sa.JSON(), nullable=False),
     sa.Column("storage_size", sa.Integer(), nullable=False),
-    sa.Column("storage_type", enum_storage_type),
+    sa.Column(
+        "storage_type",
+        sa.Enum("HDD", "SSD", "NVME_SSD", "NETWORK", name="storagetype"),
+    ),
     sa.Column("storages", sa.JSON(), nullable=False),
     sa.Column("network_speed", sa.Float(), nullable=True),
     sa.Column("inbound_traffic", sa.Float(), nullable=False),
     sa.Column("outbound_traffic", sa.Float(), nullable=False),
     sa.Column("ipv4", sa.Integer(), nullable=False),
-    sa.Column("status", enum_status, nullable=False),
+    sa.Column("status", sa.Enum("ACTIVE", "INACTIVE", name="status"), nullable=False),
     sa.Column("observed_at", sa.DateTime(), nullable=False),
     sa.ForeignKeyConstraint(
         ["vendor_id"],
         ["vendor.vendor_id"],
     ),
     sa.PrimaryKeyConstraint("vendor_id", "server_id", "observed_at")
     if op.get_context().config.attributes.get("scd")
```

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/alembic.ini` & `sparecores_crawler-0.1.4/src/sc_crawler/alembic.ini`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/alembic_helpers.py` & `sparecores_crawler-0.1.4/src/sc_crawler/alembic_helpers.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/cli.py` & `sparecores_crawler-0.1.4/src/sc_crawler/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from sqlmodel import Session, create_engine, select
 from typing_extensions import Annotated
 
 from . import vendors as vendors_module
 from .alembic_helpers import alembic_cfg, get_revision
 from .insert import insert_items
 from .logger import ProgressPanel, ScRichHandler, VendorProgressTracker, logger
-from .lookup import compliance_frameworks, countries
+from .lookup import benchmarks, compliance_frameworks, countries
 from .table_fields import Status
 from .tables import Vendor, tables
 from .tables_scd import tables_scd
 from .utils import HashLevels, get_row_by_pk, hash_database, table_name_to_model
 
 supported_vendors = [
     vendor[1]
@@ -577,14 +577,17 @@
             # add/merge static objects to database
             for compliance_framework in compliance_frameworks.values():
                 session.merge(compliance_framework)
             logger.info("%d Compliance Frameworks synced." % len(compliance_frameworks))
             for country in countries.values():
                 session.merge(country)
             logger.info("%d Countries synced." % len(countries))
+            for benchmark in benchmarks:
+                session.merge(benchmark)
+            logger.info("%d Benchmarks synced." % len(benchmarks))
             # get data for each vendor and then add/merge to database
             # TODO each vendor should open its own session and run in parallel
             for vendor in vendors:
                 logger.info("Starting to collect data from vendor: " + vendor.vendor_id)
                 vendor = session.merge(vendor)
                 # register session to the Vendor so that dependen objects can auto-merge
                 vendor.session = session
```

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/insert.py` & `sparecores_crawler-0.1.4/src/sc_crawler/insert.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/logger.py` & `sparecores_crawler-0.1.4/src/sc_crawler/logger.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/str_utils.py` & `sparecores_crawler-0.1.4/src/sc_crawler/str_utils.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/table_bases.py` & `sparecores_crawler-0.1.4/src/sc_crawler/table_bases.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from .str_utils import snake_case
 from .table_fields import (
     Allocation,
     Cpu,
     CpuAllocation,
     CpuArchitecture,
+    DdrGeneration,
     Disk,
     Gpu,
     PriceTier,
     PriceUnit,
     Status,
     StorageType,
     TrafficDirection,
@@ -49,14 +50,24 @@
     def __init__(subclass, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # early return for non-tables
         if subclass.model_config.get("table") is None:
             return
         satable = subclass.metadata.tables[subclass.__tablename__]
 
+        # enforce auto-naming constrains as per
+        # https://alembic.sqlalchemy.org/en/latest/naming.html
+        subclass.metadata.naming_convention = {
+            "ix": "ix_%(column_0_label)s",
+            "uq": "uq_%(table_name)s_%(column_0_name)s",
+            "ck": "ck_%(table_name)s_%(constraint_name)s",
+            "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
+            "pk": "pk_%(table_name)s",
+        }
+
         # table comment
         if subclass.__doc__ and satable.comment is None:
             satable.comment = subclass.__doc__.splitlines()[0]
 
         # column comments
         for k, v in subclass.model_fields.items():
             comment = satable.columns[k].comment
@@ -226,14 +237,20 @@
 
 class HasServerIdPK(ScModel):
     server_id: str = Field(
         primary_key=True, description="Unique identifier, as called at the Vendor."
     )
 
 
+class HasBenchmarkIdPK(ScModel):
+    benchmark_id: str = Field(
+        primary_key=True, description="Unique identifier of a specific Benchmark."
+    )
+
+
 class HasName(ScModel):
     name: str = Field(description="Human-friendly name.")
 
 
 class HasDescription(ScModel):
     description: Optional[str] = Field(description="Short description.")
 
@@ -276,21 +293,37 @@
 class HasServerPK(ScModel):
     server_id: str = Field(
         primary_key=True,
         description="Reference to the Server.",
     )
 
 
+class HasServerPKFK(ScModel):
+    server_id: str = Field(
+        foreign_key="server.server_id",
+        primary_key=True,
+        description="Reference to the Server.",
+    )
+
+
 class HasStoragePK(ScModel):
     storage_id: str = Field(
         primary_key=True,
         description="Reference to the Storage.",
     )
 
 
+class HasBenchmarkPKFK(ScModel):
+    benchmark_id: str = Field(
+        foreign_key="benchmark.benchmark_id",
+        primary_key=True,
+        description="Reference to the Benchmark.",
+    )
+
+
 class HasPriceFieldsBase(ScModel):
     unit: PriceUnit = Field(description="Billing unit of the pricing model.")
     # set to max price if tiered
     price: float = Field(description="Actual price of a billing unit.")
     # e.g. setup fee for dedicated servers,
     # or upfront costs of a reserved instance type
     price_upfront: float = Field(
@@ -530,26 +563,48 @@
         default=None,
         description="The product line/family of the primary processor, e.g. Xeon, Core i7, Ryzen 9.",
     )
     cpu_model: Optional[str] = Field(
         default=None,
         description="The model number of the primary processor, e.g. 9750H.",
     )
+    cpu_l1_cache: Optional[int] = Field(
+        default=None, description="L1 cache size (MiB)."
+    )
+    cpu_l2_cache: Optional[int] = Field(
+        default=None, description="L2 cache size (MiB)."
+    )
+    cpu_l3_cache: Optional[int] = Field(
+        default=None, description="L3 cache size (MiB)."
+    )
+    cpu_flags: List[str] = Field(
+        sa_type=JSON, default=[], description="CPU features/flags."
+    )
     cpus: List[Cpu] = Field(
         default=[],
         sa_type=JSON,
         description=(
             "JSON array of known CPU details, e.g. the manufacturer, family, model; "
             "L1/L2/L3 cache size; microcode version; feature flags; bugs etc."
         ),
     )
-    memory: int = Field(
+    memory_amount: int = Field(
         default=None,
         description="RAM amount (MiB).",
     )
+    memory_generation: Optional[DdrGeneration] = Field(
+        default=None, description="Generation of the DDR SDRAM, e.g. DDR4 or DDR5."
+    )
+    memory_speed: Optional[int] = Field(
+        default=None, description="DDR SDRAM clock rate (Mhz)."
+    )
+    memory_ecc: Optional[bool] = Field(
+        default=None,
+        description="If the DDR SDRAM uses error correction code to detect and correct n-bit data corruption.",
+    )
     gpu_count: int = Field(
         default=0,
         description="Number of GPU accelerator(s).",
     )
     gpu_memory_min: Optional[int] = Field(
         default=None,
         description="Memory (MiB) allocated to the lowest-end GPU accelerator.",
@@ -558,17 +613,21 @@
         default=None,
         description="Overall memory (MiB) allocated to all the GPU accelerator(s).",
     )
     gpu_manufacturer: Optional[str] = Field(
         default=None,
         description="The manufacturer of the primary GPU accelerator, e.g. Nvidia or AMD.",
     )
+    gpu_family: Optional[str] = Field(
+        default=None,
+        description="The product family of the primary GPU accelerator, e.g. Turing.",
+    )
     gpu_model: Optional[str] = Field(
         default=None,
-        description="The model number of the primary GPU accelerator.",
+        description="The model number of the primary GPU accelerator, e.g. Tesla T4.",
     )
     gpus: List[Gpu] = Field(
         default=[],
         sa_type=JSON,
         description=(
             "JSON array of GPU accelerator details, including "
             "the manufacturer, name, and memory (MiB) of each GPU."
@@ -644,7 +703,54 @@
 
 class TrafficPriceBase(HasPriceFields, TrafficPriceFields):
     pass
 
 
 class Ipv4PriceBase(HasPriceFields, HasDatacenterPK, HasVendorPKFK):
     pass
+
+
+class BenchmarkFields(HasDescription, HasName, HasBenchmarkIdPK):
+    framework: str = Field(
+        description="The name of the benchmark framework/software/tool used.",
+    )
+    config_fields: dict = Field(
+        default={},
+        sa_type=JSON,
+        description='A dictionary of descriptions on the framework-specific config options, e.g. {"bandwidth": "Memory amount to use for compression in MB."}.',
+    )
+    measurement: Optional[str] = Field(
+        default=None,
+        description="The name of measurement recoreded in the benchmark.",
+    )
+    unit: Optional[str] = Field(
+        default=None,
+        description="Optional unit of measurement for the benchmark score.",
+    )
+    higher_is_better: bool = Field(
+        default=True,
+        description="If higher benchmark score means better performance, or vica versa.",
+    )
+
+
+class BenchmarkBase(MetaColumns, BenchmarkFields):
+    pass
+
+
+class BenchmarkScoreFields(HasBenchmarkPKFK, HasServerPKFK, HasVendorPKFK):
+    config: dict = Field(
+        default={},
+        sa_type=JSON,
+        primary_key=True,
+        description='Dictionary of config parameters of the specific benchmark, e.g. {"bandwidth": 4096}',
+    )
+    score: float = Field(
+        description="The resulting score of the benchmark.",
+    )
+    note: Optional[str] = Field(
+        default=None,
+        description="Optional note, comment or context on the benchmark score.",
+    )
+
+
+class BenchmarkScoreBase(MetaColumns, BenchmarkScoreFields):
+    pass
```

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/table_fields.py` & `sparecores_crawler-0.1.4/src/sc_crawler/table_fields.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,21 +52,33 @@
     """BogoMips value."""
 
 
 class Gpu(Json):
     """GPU accelerator details."""
 
     manufacturer: str
-    """The manufacturer of the GPU accelerator, e.g. Nvidia or AMD."""
-    model: str
+    """The manufacturer/brand of the GPU accelerator, e.g. Nvidia or AMD."""
+    family: Optional[str] = None
+    """The model family/architecture of the GPU accelerator."""
+    model: Optional[str] = None
     """The model number of the GPU accelerator."""
     memory: int
     """Memory (MiB) allocated to the GPU accelerator."""
-    firmware: Optional[str] = None
+    firmware_version: Optional[str] = None
     """Firmware version."""
+    bios_version: Optional[str] = None
+    """Video BIOS version."""
+    graphics_clock: Optional[int] = None
+    """GPU core clock speed (Mhz)."""
+    sm_clock: Optional[int] = None
+    """Streaming Multiprocessor clock speed (Mhz)."""
+    mem_clock: Optional[int] = None
+    """Memory clock speed (Mhz)."""
+    video_clock: Optional[int] = None
+    """Video clock speed (Mhz)."""
 
 
 class StorageType(str, Enum):
     """Type of a storage, e.g. HDD or SSD."""
 
     HDD = "hdd"
     """Magnetic hard disk drive."""
@@ -118,14 +130,25 @@
     """32-bit x86 architecture."""
     X86_64 = "x86_64"
     """64-bit x86 architecture."""
     X86_64_MAC = "x86_64_mac"
     """Apple 64-bit x86 architecture."""
 
 
+class DdrGeneration(str, Enum):
+    """Generation of the DDR SDRAM."""
+
+    DDR3 = "DDR3"
+    """DDR3 SDRAM."""
+    DDR4 = "DDR4"
+    """DDR4 SDRAM."""
+    DDR5 = "DDR5"
+    """DDR5 SDRAM."""
+
+
 class Allocation(str, Enum):
     """Server allocation options."""
 
     ONDEMAND = "ondemand"
     """On-demand server."""
     RESERVED = "reserved"
     """Reserved server."""
```

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/tables.py` & `sparecores_crawler-0.1.4/src/sc_crawler/tables.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 from typing import Callable, List, Optional
 
 from pydantic import ImportString, PrivateAttr
 from sqlalchemy import ForeignKeyConstraint, update
 from sqlmodel import Relationship, Session, SQLModel
 
 from .insert import insert_items
+from .inspector import inspect_server_benchmarks, inspect_update_server_dict
 from .logger import VendorProgressTracker, log_start_end, logger
 from .table_bases import (
+    BenchmarkBase,
+    BenchmarkScoreBase,
     ComplianceFrameworkBase,
     CountryBase,
     DatacenterBase,
     Ipv4PriceBase,
     ScModel,
     ServerBase,
     ServerPriceBase,
@@ -90,14 +93,17 @@
     )
     ipv4_prices: List["Ipv4Price"] = Relationship(
         back_populates="vendor", sa_relationship_kwargs={"viewonly": True}
     )
     storage_prices: List["StoragePrice"] = Relationship(
         back_populates="vendor", sa_relationship_kwargs={"viewonly": True}
     )
+    benchmark_scores: List["BenchmarkScore"] = Relationship(
+        back_populates="vendor", sa_relationship_kwargs={"viewonly": True}
+    )
 
     # private attributes
     _methods: Optional[ImportString[ModuleType]] = PrivateAttr(default=None)
     _session: Optional[Session] = PrivateAttr()
     _progress_tracker: Optional[VendorProgressTracker] = PrivateAttr()
 
     def __init__(self, **kwargs):
@@ -224,15 +230,31 @@
     def inventory_zones(self):
         """Get all the zones in the vendor's datacenters."""
         self._inventory(Zone, self._get_methods().inventory_zones)
 
     @log_start_end
     def inventory_servers(self):
         """Get the vendor's all server types."""
-        self._inventory(Server, self._get_methods().inventory_servers)
+        self.set_table_rows_inactive(Server)
+        servers = self._get_methods().inventory_servers(self)
+        for server in servers:
+            server = inspect_update_server_dict(server)
+        insert_items(Server, servers, self)
+        benchmarks = []
+        self.progress_tracker.start_task(
+            name="Searching for benchmark(s)", total=len(self.servers)
+        )
+        for server in self.servers:
+            benchmarks += inspect_server_benchmarks(server)
+            self.progress_tracker.advance_task()
+        self.progress_tracker.hide_task()
+        self.set_table_rows_inactive(
+            BenchmarkScore, BenchmarkScore.vendor_id == self.vendor_id
+        )
+        insert_items(BenchmarkScore, benchmarks, self)
 
     @log_start_end
     def inventory_server_prices(self):
         """Get the current standard/ondemand/reserved prices of all server types."""
         self.set_table_rows_inactive(
             ServerPrice, ServerPrice.allocation != Allocation.SPOT
         )
@@ -344,14 +366,17 @@
 class Server(ServerBase, table=True):
     """Server types."""
 
     vendor: Vendor = Relationship(back_populates="servers")
     prices: List["ServerPrice"] = Relationship(
         back_populates="server", sa_relationship_kwargs={"viewonly": True}
     )
+    benchmark_scores: List["BenchmarkScore"] = Relationship(
+        back_populates="server", sa_relationship_kwargs={"viewonly": True}
+    )
 
 
 class ServerPrice(ServerPriceBase, table=True):
     """Server type prices per Datacenter and Allocation method."""
 
     __table_args__ = (
         ForeignKeyConstraint(
@@ -470,14 +495,47 @@
                 "and_(Datacenter.datacenter_id == foreign(Ipv4Price.datacenter_id),"
                 "Vendor.vendor_id == foreign(Ipv4Price.vendor_id))"
             )
         },
     )
 
 
+class Benchmark(BenchmarkBase, table=True):
+    """Benchmark scenario definitions."""
+
+    benchmark_scores: List["BenchmarkScore"] = Relationship(
+        back_populates="benchmark", sa_relationship_kwargs={"viewonly": True}
+    )
+
+
+class BenchmarkScore(BenchmarkScoreBase, table=True):
+    """Results of running Benchmark scenarios on Servers."""
+
+    __table_args__ = (
+        ForeignKeyConstraint(
+            ["vendor_id", "server_id"],
+            [
+                "benchmark_score.vendor_id",
+                "benchmark_score.server_id",
+            ],
+        ),
+    )
+    vendor: Vendor = Relationship(back_populates="benchmark_scores")
+    server: Server = Relationship(
+        back_populates="benchmark_scores",
+        sa_relationship_kwargs={
+            "primaryjoin": (
+                "and_(Server.server_id == foreign(BenchmarkScore.server_id), "
+                "Vendor.vendor_id == foreign(BenchmarkScore.vendor_id))"
+            )
+        },
+    )
+    benchmark: Benchmark = Relationship(back_populates="benchmark_scores")
+
+
 Country.model_rebuild()
 ComplianceFramework.model_rebuild()
 Vendor.model_rebuild()
 VendorComplianceLink.model_rebuild()
 Datacenter.model_rebuild()
 Zone.model_rebuild()
 Storage.model_rebuild()
```

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/tables_scd.py` & `sparecores_crawler-0.1.4/src/sc_crawler/tables_scd.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/utils.py` & `sparecores_crawler-0.1.4/src/sc_crawler/utils.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/vendors/aws.py` & `sparecores_crawler-0.1.4/src/sc_crawler/vendors/aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         "family": it.split(".")[0],
         "vcpus": vcpu_info["DefaultVCpus"],
         "cpu_allocation": allocation,
         "cpu_cores": vcpu_info["DefaultCores"],
         "cpu_speed": cpu_info.get("SustainedClockSpeedInGhz", None),
         "cpu_architecture": cpu_info["SupportedArchitectures"][0],
         "cpu_manufacturer": cpu_info.get("Manufacturer", None),
-        "memory": instance_type["MemoryInfo"]["SizeInMiB"],
+        "memory_amount": instance_type["MemoryInfo"]["SizeInMiB"],
         "gpu_count": gpu_info[0],
         "gpu_memory_min": gpu_info[1],
         "gpu_memory_total": gpu_info[2],
         "gpu_manufacturer": gpu_info[3],
         "gpu_model": gpu_info[4],
         "gpus": _get_gpus_of_instance_type(instance_type),
         "storage_size": storage_info[0],
```

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/vendors/gcp.py` & `sparecores_crawler-0.1.4/src/sc_crawler/vendors/gcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
             # add ram and cpu prices
             elif skus["cpu"][family]:
                 try:
                     price = (
                         skus["cpu"][family][region][allocation.value.lower()][0]
                         * server.vcpus
                         + skus["ram"][family][region][allocation.value.lower()][0]
-                        * server.memory
+                        * server.memory_amount
                         / 1024
                     )
                     currency = skus["cpu"][family][region][allocation.value.lower()][1]
                 except (ValueError, TypeError):
                     vendor.log(
                         f"{allocation.value} price not found for '{server.name}' in '{region}'",
                         DEBUG,
@@ -810,15 +810,15 @@
                         if server.name.startswith("t2a")
                         else CpuArchitecture.X86_64
                     ),
                     "cpu_manufacturer": None,
                     "cpu_family": None,
                     "cpu_model": None,
                     "cpus": [],
-                    "memory": server.memory_mb,
+                    "memory_amount": server.memory_mb,
                     "gpu_count": (
                         server.accelerators[0].guest_accelerator_count
                         if server.accelerators
                         else 0
                     ),
                     "gpu_memory_min": None,
                     "gpu_memory_total": None,
```

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/vendors/hcloud.py` & `sparecores_crawler-0.1.4/src/sc_crawler/vendors/hcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                     if server.architecture == "arm"
                     else CpuArchitecture.X86_64
                 ),
                 "cpu_manufacturer": cpu[0],
                 "cpu_family": cpu[1],
                 "cpu_model": cpu[2],
                 "cpus": [],
-                "memory": server.memory * 1024,
+                "memory_amount": server.memory * 1024,
                 "gpu_count": 0,
                 "gpu_memory_min": None,
                 "gpu_memory_total": None,
                 "gpu_manufacturer": None,
                 "gpu_model": None,
                 "gpus": [],
                 "storage_size": server.disk,
```

### Comparing `sparecores_crawler-0.1.3/src/sc_crawler/vendors/vendors.py` & `sparecores_crawler-0.1.4/src/sc_crawler/vendors/vendors.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/PKG-INFO` & `sparecores_crawler-0.1.4/src/sparecores_crawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparecores-crawler
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pull and standardize data on cloud compute resources.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-crawler
 Project-URL: issues, https://github.com/SpareCores/sc-crawler/issues
 Project-URL: documentation, https://sparecores.github.io/sc-crawler/
 Project-URL: homepage, https://sparecores.com
@@ -16,14 +16,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: alembic
 Requires-Dist: cachier
 Requires-Dist: pydantic
 Requires-Dist: pydantic_extra_types
+Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: sqlmodel
 Requires-Dist: typer
 Provides-Extra: mkdocs
 Requires-Dist: markdown==3.5.2; extra == "mkdocs"
 Requires-Dist: mkdocs; extra == "mkdocs"
 Requires-Dist: mkdocs-material[imaging]==9.5.13; extra == "mkdocs"
```

### Comparing `sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/requires.txt` & `sparecores_crawler-0.1.4/src/sparecores_crawler.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 alembic
 cachier
 pydantic
 pydantic_extra_types
+requests
 rich
 sqlmodel
 typer
 
 [all]
 sparecores-crawler[testing]
 sparecores-crawler[vendors]
```

### Comparing `sparecores_crawler-0.1.3/tests/test_schemas.py` & `sparecores_crawler-0.1.4/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/tests/test_str_utils.py` & `sparecores_crawler-0.1.4/tests/test_str_utils.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.3/tests/test_utils.py` & `sparecores_crawler-0.1.4/tests/test_utils.py`

 * *Files identical despite different names*

