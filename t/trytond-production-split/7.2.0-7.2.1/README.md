# Comparing `tmp/trytond_production_split-7.2.0.tar.gz` & `tmp/trytond_production_split-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_production_split-7.2.0.tar", last modified: Mon Apr 29 15:44:21 2024, max compression
+gzip compressed data, was "trytond_production_split-7.2.1.tar", last modified: Sun Jun  2 16:26:32 2024, max compression
```

## Comparing `trytond_production_split-7.2.0.tar` & `trytond_production_split-7.2.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     1468 2024-04-29 15:22:45.000000 trytond_production_split-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      708 2024-04-29 15:22:45.000000 trytond_production_split-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_production_split-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2611 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-01-16 14:00:21.000000 trytond_production_split-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.876599 trytond_production_split-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-27 16:30:39.000000 trytond_production_split-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-01-16 14:00:21.000000 trytond_production_split-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:18.000000 trytond_production_split-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.876599 trytond_production_split-7.2.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      242 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/icons/tryton-production-split.svg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1145 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1162 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1183 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1157 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1022 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1120 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1181 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1157 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1113 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      993 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1113 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1207 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1165 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1165 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1115 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1063 2024-04-27 16:43:25.000000 trytond_production_split-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3634 2024-02-04 18:51:26.000000 trytond_production_split-7.2.0/production.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1438 2024-04-27 16:30:39.000000 trytond_production_split-7.2.0/production.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4333 2024-03-17 11:01:36.000000 trytond_production_split-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1551 2024-02-04 18:51:26.000000 trytond_production_split-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:18.000000 trytond_production_split-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-29 15:22:41.000000 trytond_production_split-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/trytond_production_split.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2611 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1525 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:07.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       55 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:44:21.000000 trytond_production_split-7.2.0/trytond_production_split.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:44:21.879932 trytond_production_split-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      349 2023-04-15 07:12:15.000000 trytond_production_split-7.2.0/view/production_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-02-04 18:51:26.000000 trytond_production_split-7.2.0/view/split_start_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:26:32.443512 trytond_production_split-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1569 2024-06-02 16:26:29.000000 trytond_production_split-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      708 2024-06-02 16:26:29.000000 trytond_production_split-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2611 2024-06-02 16:26:32.443512 trytond_production_split-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:26:32.440178 trytond_production_split-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3079 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:26:32.440178 trytond_production_split-7.2.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      242 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/icons/tryton-production-split.svg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:26:32.443512 trytond_production_split-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1145 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1162 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1183 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1157 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1022 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1120 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1181 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1157 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1113 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      993 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1113 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1207 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1048 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1165 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1165 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1115 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      988 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1063 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3635 2024-05-29 10:23:59.000000 trytond_production_split-7.2.1/production.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1438 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/production.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 16:26:32.443512 trytond_production_split-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4333 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:26:32.443512 trytond_production_split-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1551 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       78 2024-04-30 17:21:06.000000 trytond_production_split-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:26:32.443512 trytond_production_split-7.2.1/trytond_production_split.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2611 2024-06-02 16:26:32.000000 trytond_production_split-7.2.1/trytond_production_split.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1525 2024-06-02 16:26:32.000000 trytond_production_split-7.2.1/trytond_production_split.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 16:26:32.000000 trytond_production_split-7.2.1/trytond_production_split.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       70 2024-06-02 16:26:32.000000 trytond_production_split-7.2.1/trytond_production_split.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 14:11:52.000000 trytond_production_split-7.2.1/trytond_production_split.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       55 2024-06-02 16:26:32.000000 trytond_production_split-7.2.1/trytond_production_split.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 16:26:32.000000 trytond_production_split-7.2.1/trytond_production_split.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:26:32.443512 trytond_production_split-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      349 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/view/production_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:21:00.000000 trytond_production_split-7.2.1/view/split_start_form.xml
```

### Comparing `trytond_production_split-7.2.0/CHANGELOG` & `trytond_production_split-7.2.1/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.2.1 - 2024-06-02
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.2.0 - 2024-04-29
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.0.0 - 2023-10-30
 --------------------------
```

### Comparing `trytond_production_split-7.2.0/COPYRIGHT` & `trytond_production_split-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/LICENSE` & `trytond_production_split-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/PKG-INFO` & `trytond_production_split-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_production_split
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to split production
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_production_split-7.2.0/doc/conf.py` & `trytond_production_split-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/icons/LICENSE` & `trytond_production_split-7.2.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/bg.po` & `trytond_production_split-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/ca.po` & `trytond_production_split-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/cs.po` & `trytond_production_split-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/de.po` & `trytond_production_split-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/es.po` & `trytond_production_split-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/es_419.po` & `trytond_production_split-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/et.po` & `trytond_production_split-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/fa.po` & `trytond_production_split-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/fi.po` & `trytond_production_split-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/fr.po` & `trytond_production_split-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/hu.po` & `trytond_production_split-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/id.po` & `trytond_production_split-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/it.po` & `trytond_production_split-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/lo.po` & `trytond_production_split-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/lt.po` & `trytond_production_split-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/nl.po` & `trytond_production_split-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/pl.po` & `trytond_production_split-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/pt.po` & `trytond_production_split-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/ro.po` & `trytond_production_split-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/ru.po` & `trytond_production_split-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/sl.po` & `trytond_production_split-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/tr.po` & `trytond_production_split-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/uk.po` & `trytond_production_split-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/locale/zh_CN.po` & `trytond_production_split-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/production.py` & `trytond_production_split-7.2.1/production.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             Button('Split', 'split', 'tryton-ok', default=True),
             ])
     split = StateTransition()
 
     def default_start(self, fields):
         return {
             'unit': self.record.unit.id,
-            'uom_category': self.record.uom.category.id,
+            'uom_category': self.record.unit.category.id,
             }
 
     def transition_split(self):
         self.record.split(
             self.start.quantity, self.start.unit, count=self.start.count)
         return 'end'
```

### Comparing `trytond_production_split-7.2.0/production.xml` & `trytond_production_split-7.2.1/production.xml`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/setup.py` & `trytond_production_split-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/tests/test_module.py` & `trytond_production_split-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/tox.ini` & `trytond_production_split-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_production_split-7.2.0/trytond_production_split.egg-info/PKG-INFO` & `trytond_production_split-7.2.1/trytond_production_split.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_production_split
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to split production
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_production_split-7.2.0/trytond_production_split.egg-info/SOURCES.txt` & `trytond_production_split-7.2.1/trytond_production_split.egg-info/SOURCES.txt`

 * *Files identical despite different names*

