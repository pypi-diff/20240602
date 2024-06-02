# Comparing `tmp/trytond_purchase_blanket_agreement-7.2.1.tar.gz` & `tmp/trytond_purchase_blanket_agreement-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase_blanket_agreement-7.2.1.tar", last modified: Wed May  1 11:36:50 2024, max compression
+gzip compressed data, was "trytond_purchase_blanket_agreement-7.2.2.tar", last modified: Sun Jun  2 16:17:29 2024, max compression
```

## Comparing `trytond_purchase_blanket_agreement-7.2.1.tar` & `trytond_purchase_blanket_agreement-7.2.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.108954 trytond_purchase_blanket_agreement-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      565 2024-05-01 11:36:46.000000 trytond_purchase_blanket_agreement-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-05-01 11:36:46.000000 trytond_purchase_blanket_agreement-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2755 2024-05-01 11:36:50.108954 trytond_purchase_blanket_agreement-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)       13 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      699 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.105621 trytond_purchase_blanket_agreement-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1686 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.105621 trytond_purchase_blanket_agreement-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7777 2024-04-30 17:21:59.000000 trytond_purchase_blanket_agreement-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7827 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7838 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7784 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6718 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7900 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      933 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      519 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    32617 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11915 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:36:50.108954 trytond_purchase_blanket_agreement-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4824 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.105621 trytond_purchase_blanket_agreement-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5537 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/tests/scenario_purchase_blanket_agreement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      153 2024-04-30 17:21:06.000000 trytond_purchase_blanket_agreement-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.108954 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2755 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2405 2024-05-01 11:36:50.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:36:50.108954 trytond_purchase_blanket_agreement-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/product_list_agreement_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_create_purchase_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1608 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1290 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      480 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.1/view/purchase_line_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:17:29.017725 trytond_purchase_blanket_agreement-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)      666 2024-06-02 16:17:25.000000 trytond_purchase_blanket_agreement-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      804 2024-06-02 16:17:25.000000 trytond_purchase_blanket_agreement-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2755 2024-06-02 16:17:29.017725 trytond_purchase_blanket_agreement-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)       13 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      699 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:17:29.011058 trytond_purchase_blanket_agreement-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1686 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:17:29.014392 trytond_purchase_blanket_agreement-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7777 2024-04-30 17:21:59.000000 trytond_purchase_blanket_agreement-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7827 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7838 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7784 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6718 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7900 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6615 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      933 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      519 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    32609 2024-05-26 17:46:37.000000 trytond_purchase_blanket_agreement-7.2.2/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11915 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 16:17:29.017725 trytond_purchase_blanket_agreement-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4824 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:17:29.014392 trytond_purchase_blanket_agreement-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5537 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/tests/scenario_purchase_blanket_agreement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      153 2024-05-01 11:36:56.000000 trytond_purchase_blanket_agreement-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:17:29.017725 trytond_purchase_blanket_agreement-7.2.2/trytond_purchase_blanket_agreement.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2755 2024-06-02 16:17:28.000000 trytond_purchase_blanket_agreement-7.2.2/trytond_purchase_blanket_agreement.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2405 2024-06-02 16:17:28.000000 trytond_purchase_blanket_agreement-7.2.2/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 16:17:28.000000 trytond_purchase_blanket_agreement-7.2.2/trytond_purchase_blanket_agreement.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-06-02 16:17:28.000000 trytond_purchase_blanket_agreement-7.2.2/trytond_purchase_blanket_agreement.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:36:49.000000 trytond_purchase_blanket_agreement-7.2.2/trytond_purchase_blanket_agreement.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-06-02 16:17:28.000000 trytond_purchase_blanket_agreement-7.2.2/trytond_purchase_blanket_agreement.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 16:17:28.000000 trytond_purchase_blanket_agreement-7.2.2/trytond_purchase_blanket_agreement.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:17:29.017725 trytond_purchase_blanket_agreement-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/view/product_list_agreement_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/view/purchase_blanket_agreement_create_purchase_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1608 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/view/purchase_blanket_agreement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1290 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/view/purchase_blanket_agreement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/view/purchase_blanket_agreement_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      480 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/view/purchase_blanket_agreement_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/view/purchase_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      340 2024-04-30 17:21:00.000000 trytond_purchase_blanket_agreement-7.2.2/view/purchase_line_list.xml
```

### Comparing `trytond_purchase_blanket_agreement-7.2.1/CHANGELOG` & `trytond_purchase_blanket_agreement-7.2.2/CHANGELOG`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 7.2.2 - 2024-06-02
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 7.2.1 - 2024-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 7.2.0 - 2024-04-29
 --------------------------
```

### Comparing `trytond_purchase_blanket_agreement-7.2.1/COPYRIGHT` & `trytond_purchase_blanket_agreement-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/LICENSE` & `trytond_purchase_blanket_agreement-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/PKG-INFO` & `trytond_purchase_blanket_agreement-7.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_blanket_agreement
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for purchase blanket agreement
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_blanket_agreement-7.2.1/__init__.py` & `trytond_purchase_blanket_agreement-7.2.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/doc/conf.py` & `trytond_purchase_blanket_agreement-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/doc/design.rst` & `trytond_purchase_blanket_agreement-7.2.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/bg.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/ca.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/cs.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/de.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/es.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/es_419.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/et.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/fa.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/fi.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/fr.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/hu.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/id.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/it.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/lo.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/lt.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/nl.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/pl.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/pt.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/ro.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/ru.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/sl.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/tr.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/uk.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/locale/zh_CN.po` & `trytond_purchase_blanket_agreement-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/message.xml` & `trytond_purchase_blanket_agreement-7.2.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/product.xml` & `trytond_purchase_blanket_agreement-7.2.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/purchase.py` & `trytond_purchase_blanket_agreement-7.2.2/purchase.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,16 +581,16 @@
         return self.product.default_uom_category if self.product else None
 
     @fields.depends(
         'quantity', 'unit_price', 'blanket_agreement',
         '_parent_blanket_agreement.currency')
     def on_change_with_amount(self, name=None):
         amount = (
-            Decimal(str(self.quantity or '0.0'))
-            * (self.unit_price or Decimal('0.0')))
+            Decimal(str(self.quantity or 0))
+            * (self.unit_price or Decimal(0)))
 
         if self.blanket_agreement and self.blanket_agreement.currency:
             return self.blanket_agreement.currency.round(amount)
         return amount
 
     @fields.depends('blanket_agreement', '_parent_blanket_agreement.currency')
     def on_change_with_currency(self, name=None):
```

### Comparing `trytond_purchase_blanket_agreement-7.2.1/purchase.xml` & `trytond_purchase_blanket_agreement-7.2.2/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/setup.py` & `trytond_purchase_blanket_agreement-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/tests/scenario_purchase_blanket_agreement.rst` & `trytond_purchase_blanket_agreement-7.2.2/tests/scenario_purchase_blanket_agreement.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/tox.ini` & `trytond_purchase_blanket_agreement-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/PKG-INFO` & `trytond_purchase_blanket_agreement-7.2.2/trytond_purchase_blanket_agreement.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase_blanket_agreement
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for purchase blanket agreement
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase_blanket_agreement-7.2.1/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt` & `trytond_purchase_blanket_agreement-7.2.2/trytond_purchase_blanket_agreement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_form.xml` & `trytond_purchase_blanket_agreement-7.2.2/view/purchase_blanket_agreement_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_line_form.xml` & `trytond_purchase_blanket_agreement-7.2.2/view/purchase_blanket_agreement_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase_blanket_agreement-7.2.1/view/purchase_blanket_agreement_line_list.xml` & `trytond_purchase_blanket_agreement-7.2.2/view/purchase_blanket_agreement_line_list.xml`

 * *Files identical despite different names*

