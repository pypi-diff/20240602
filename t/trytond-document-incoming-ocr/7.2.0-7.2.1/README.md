# Comparing `tmp/trytond_document_incoming_ocr-7.2.0.tar.gz` & `tmp/trytond_document_incoming_ocr-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_document_incoming_ocr-7.2.0.tar", last modified: Mon Apr 29 15:40:29 2024, max compression
+gzip compressed data, was "trytond_document_incoming_ocr-7.2.1.tar", last modified: Sun Jun  2 16:39:23 2024, max compression
```

## Comparing `trytond_document_incoming_ocr-7.2.0.tar` & `trytond_document_incoming_ocr-7.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.479344 trytond_document_incoming_ocr-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-04-29 15:19:46.000000 trytond_document_incoming_ocr-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:19:46.000000 trytond_document_incoming_ocr-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2623 2024-04-29 15:40:29.479344 trytond_document_incoming_ocr-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      920 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.476010 trytond_document_incoming_ocr-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-27 16:30:39.000000 trytond_document_incoming_ocr-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      701 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      235 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:09.000000 trytond_document_incoming_ocr-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    18186 2024-04-13 17:12:23.000000 trytond_document_incoming_ocr-7.2.0/document.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4523 2024-04-27 16:30:39.000000 trytond_document_incoming_ocr-7.2.0/document.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.476010 trytond_document_incoming_ocr-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1954 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2018 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1957 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2011 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1931 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1755 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-27 16:43:24.000000 trytond_document_incoming_ocr-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:40:29.479344 trytond_document_incoming_ocr-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4614 2024-04-27 16:30:39.000000 trytond_document_incoming_ocr-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.476010 trytond_document_incoming_ocr-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1443 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:09.000000 trytond_document_incoming_ocr-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      205 2024-04-29 15:19:42.000000 trytond_document_incoming_ocr-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.479344 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2623 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1786 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:29:56.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:40:29.000000 trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:40:29.479344 trytond_document_incoming_ocr-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      485 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/view/document_incoming_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      535 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/view/document_incoming_ocr_service_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/view/document_incoming_ocr_service_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-02-04 18:51:26.000000 trytond_document_incoming_ocr-7.2.0/view/document_incoming_ocr_service_list_sequence.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:39:23.096689 trytond_document_incoming_ocr-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)      273 2024-06-02 16:39:19.000000 trytond_document_incoming_ocr-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-06-02 16:39:19.000000 trytond_document_incoming_ocr-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2623 2024-06-02 16:39:23.096689 trytond_document_incoming_ocr-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      235 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      920 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:39:23.093356 trytond_document_incoming_ocr-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3084 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      701 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      235 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    18207 2024-05-29 09:17:30.000000 trytond_document_incoming_ocr-7.2.1/document.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4523 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/document.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:39:23.093356 trytond_document_incoming_ocr-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1954 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2018 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1957 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2011 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1931 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1755 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1532 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 16:39:23.096689 trytond_document_incoming_ocr-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4614 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:39:23.096689 trytond_document_incoming_ocr-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1443 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      205 2024-04-30 17:21:06.000000 trytond_document_incoming_ocr-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:39:23.096689 trytond_document_incoming_ocr-7.2.1/trytond_document_incoming_ocr.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2623 2024-06-02 16:39:22.000000 trytond_document_incoming_ocr-7.2.1/trytond_document_incoming_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1786 2024-06-02 16:39:23.000000 trytond_document_incoming_ocr-7.2.1/trytond_document_incoming_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 16:39:22.000000 trytond_document_incoming_ocr-7.2.1/trytond_document_incoming_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2024-06-02 16:39:22.000000 trytond_document_incoming_ocr-7.2.1/trytond_document_incoming_ocr.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 14:11:51.000000 trytond_document_incoming_ocr-7.2.1/trytond_document_incoming_ocr.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-06-02 16:39:22.000000 trytond_document_incoming_ocr-7.2.1/trytond_document_incoming_ocr.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 16:39:22.000000 trytond_document_incoming_ocr-7.2.1/trytond_document_incoming_ocr.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:39:23.096689 trytond_document_incoming_ocr-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      485 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/view/document_incoming_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      535 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/view/document_incoming_ocr_service_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/view/document_incoming_ocr_service_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-04-30 17:20:59.000000 trytond_document_incoming_ocr-7.2.1/view/document_incoming_ocr_service_list_sequence.xml
```

### Comparing `trytond_document_incoming_ocr-7.2.0/COPYRIGHT` & `trytond_document_incoming_ocr-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/LICENSE` & `trytond_document_incoming_ocr-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/PKG-INFO` & `trytond_document_incoming_ocr-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_document_incoming_ocr
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to process incoming document with OCR
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_document_incoming_ocr-7.2.0/__init__.py` & `trytond_document_incoming_ocr-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/account.py` & `trytond_document_incoming_ocr-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/doc/conf.py` & `trytond_document_incoming_ocr-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/doc/design.rst` & `trytond_document_incoming_ocr-7.2.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/document.py` & `trytond_document_incoming_ocr-7.2.1/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,17 @@
         Currency = pool.get('currency.currency')
 
         invoice = super()._process_supplier_invoice()
         if self.ocr_service:
             invoice_data = self.ocr_service.get_supplier_invoice(self)
 
             tax_identifier = invoice_data.get('tax_identifier')
-            if tax_identifier:
+            if tax_identifier and invoice.party:
                 tax_identifier_types = Party.tax_identifier_types()
-                for identifier in self.party.identifiers:
+                for identifier in invoice.party.identifiers:
                     if (identifier.type in tax_identifier_types
                             and identifier.code == tax_identifier):
                         invoice.party_tax_identifier = identifier
 
             currency = invoice_data.get('currency')
             if currency:
                 try:
```

### Comparing `trytond_document_incoming_ocr-7.2.0/document.xml` & `trytond_document_incoming_ocr-7.2.1/document.xml`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/bg.po` & `trytond_document_incoming_ocr-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/ca.po` & `trytond_document_incoming_ocr-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/cs.po` & `trytond_document_incoming_ocr-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/de.po` & `trytond_document_incoming_ocr-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/es.po` & `trytond_document_incoming_ocr-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/es_419.po` & `trytond_document_incoming_ocr-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/et.po` & `trytond_document_incoming_ocr-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/fa.po` & `trytond_document_incoming_ocr-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/fi.po` & `trytond_document_incoming_ocr-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/fr.po` & `trytond_document_incoming_ocr-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/hu.po` & `trytond_document_incoming_ocr-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/id.po` & `trytond_document_incoming_ocr-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/it.po` & `trytond_document_incoming_ocr-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/lo.po` & `trytond_document_incoming_ocr-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/lt.po` & `trytond_document_incoming_ocr-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/nl.po` & `trytond_document_incoming_ocr-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/pl.po` & `trytond_document_incoming_ocr-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/pt.po` & `trytond_document_incoming_ocr-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/ro.po` & `trytond_document_incoming_ocr-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/ru.po` & `trytond_document_incoming_ocr-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/sl.po` & `trytond_document_incoming_ocr-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/tr.po` & `trytond_document_incoming_ocr-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/uk.po` & `trytond_document_incoming_ocr-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/locale/zh_CN.po` & `trytond_document_incoming_ocr-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/setup.py` & `trytond_document_incoming_ocr-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/tests/test_module.py` & `trytond_document_incoming_ocr-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/tox.ini` & `trytond_document_incoming_ocr-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/PKG-INFO` & `trytond_document_incoming_ocr-7.2.1/trytond_document_incoming_ocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_document_incoming_ocr
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to process incoming document with OCR
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_document_incoming_ocr-7.2.0/trytond_document_incoming_ocr.egg-info/SOURCES.txt` & `trytond_document_incoming_ocr-7.2.1/trytond_document_incoming_ocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_document_incoming_ocr-7.2.0/view/document_incoming_ocr_service_form.xml` & `trytond_document_incoming_ocr-7.2.1/view/document_incoming_ocr_service_form.xml`

 * *Files identical despite different names*

