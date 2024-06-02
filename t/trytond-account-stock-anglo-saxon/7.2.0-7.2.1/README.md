# Comparing `tmp/trytond_account_stock_anglo_saxon-7.2.0.tar.gz` & `tmp/trytond_account_stock_anglo_saxon-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_anglo_saxon-7.2.0.tar", last modified: Mon Apr 29 15:36:25 2024, max compression
+gzip compressed data, was "trytond_account_stock_anglo_saxon-7.2.1.tar", last modified: Sun Jun  2 16:52:51 2024, max compression
```

## Comparing `trytond_account_stock_anglo_saxon-7.2.0.tar` & `trytond_account_stock_anglo_saxon-7.2.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2653 2024-04-29 15:16:26.000000 trytond_account_stock_anglo_saxon-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:16:26.000000 trytond_account_stock_anglo_saxon-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3812 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/account.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.172400 trytond_account_stock_anglo_saxon-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-27 16:30:39.000000 trytond_account_stock_anglo_saxon-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      905 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:00.000000 trytond_account_stock_anglo_saxon-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      231 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4253 2024-01-27 09:58:52.000000 trytond_account_stock_anglo_saxon-7.2.0/invoice.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.172400 trytond_account_stock_anglo_saxon-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1337 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1275 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)      985 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1176 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1338 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1319 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1301 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-27 16:43:21.000000 trytond_account_stock_anglo_saxon-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      669 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1124 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      691 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      706 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      692 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2236 2024-01-27 09:58:52.000000 trytond_account_stock_anglo_saxon-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      472 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4685 2024-03-17 11:01:36.000000 trytond_account_stock_anglo_saxon-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6725 2024-02-04 18:51:26.000000 trytond_account_stock_anglo_saxon-7.2.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12305 2024-04-27 16:30:39.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/scenario_account_stock_anglo_saxon.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7997 2024-04-27 16:30:39.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1829 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-01-27 09:58:52.000000 trytond_account_stock_anglo_saxon-7.2.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:00.000000 trytond_account_stock_anglo_saxon-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2024-04-29 15:16:21.000000 trytond_account_stock_anglo_saxon-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3812 2024-04-29 15:36:24.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2318 2024-04-29 15:36:25.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:24.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:36:24.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-04-29 15:36:24.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:24.000000 trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:25.175733 trytond_account_stock_anglo_saxon-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-01-16 14:00:20.000000 trytond_account_stock_anglo_saxon-7.2.0/view/category_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:52:51.918868 trytond_account_stock_anglo_saxon-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2754 2024-06-02 16:52:48.000000 trytond_account_stock_anglo_saxon-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-06-02 16:52:48.000000 trytond_account_stock_anglo_saxon-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3812 2024-06-02 16:52:51.918868 trytond_account_stock_anglo_saxon-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/account.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:52:51.915535 trytond_account_stock_anglo_saxon-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      905 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      231 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4245 2024-05-26 17:46:37.000000 trytond_account_stock_anglo_saxon-7.2.1/invoice.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:52:51.918868 trytond_account_stock_anglo_saxon-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1337 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1275 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      985 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1176 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1398 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1338 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1260 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1319 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1301 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1106 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      669 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1124 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      691 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      706 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      692 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2236 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      472 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 16:52:51.918868 trytond_account_stock_anglo_saxon-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4685 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6721 2024-05-26 17:46:37.000000 trytond_account_stock_anglo_saxon-7.2.1/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:52:51.918868 trytond_account_stock_anglo_saxon-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12305 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/tests/scenario_account_stock_anglo_saxon.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7997 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1829 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2024-04-30 17:21:06.000000 trytond_account_stock_anglo_saxon-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:52:51.918868 trytond_account_stock_anglo_saxon-7.2.1/trytond_account_stock_anglo_saxon.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3812 2024-06-02 16:52:51.000000 trytond_account_stock_anglo_saxon-7.2.1/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2318 2024-06-02 16:52:51.000000 trytond_account_stock_anglo_saxon-7.2.1/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 16:52:51.000000 trytond_account_stock_anglo_saxon-7.2.1/trytond_account_stock_anglo_saxon.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-06-02 16:52:51.000000 trytond_account_stock_anglo_saxon-7.2.1/trytond_account_stock_anglo_saxon.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 14:11:51.000000 trytond_account_stock_anglo_saxon-7.2.1/trytond_account_stock_anglo_saxon.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2024-06-02 16:52:51.000000 trytond_account_stock_anglo_saxon-7.2.1/trytond_account_stock_anglo_saxon.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 16:52:51.000000 trytond_account_stock_anglo_saxon-7.2.1/trytond_account_stock_anglo_saxon.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:52:51.918868 trytond_account_stock_anglo_saxon-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2024-04-30 17:20:59.000000 trytond_account_stock_anglo_saxon-7.2.1/view/category_form.xml
```

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/CHANGELOG` & `trytond_account_stock_anglo_saxon-7.2.1/CHANGELOG`

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

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/COPYRIGHT` & `trytond_account_stock_anglo_saxon-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/LICENSE` & `trytond_account_stock_anglo_saxon-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/PKG-INFO` & `trytond_account_stock_anglo_saxon-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_anglo_saxon
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for anglo-saxon real-time stock valuation
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/README.rst` & `trytond_account_stock_anglo_saxon-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/doc/conf.py` & `trytond_account_stock_anglo_saxon-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/doc/index.rst` & `trytond_account_stock_anglo_saxon-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/invoice.py` & `trytond_account_stock_anglo_saxon-7.2.1/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,18 @@
         move_line = MoveLine()
         move_line.description = self.description
         move_line.amount_second_currency = None
         move_line.second_currency = None
 
         if type_.startswith('in_'):
             move_line.debit = amount
-            move_line.credit = Decimal('0.0')
+            move_line.credit = Decimal(0)
             move_line.account = self.product.account_stock_in_used
         else:
-            move_line.debit = Decimal('0.0')
+            move_line.debit = Decimal(0)
             move_line.credit = amount
             move_line.account = self.product.account_stock_out_used
 
         result.append(move_line)
         debit, credit = move_line.debit, move_line.credit
         move_line = MoveLine()
         move_line.description = self.description
```

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/bg.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/ca.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/cs.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/de.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/es.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/es_419.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/et.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/fa.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/fi.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/fr.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/hu.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/id.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/it.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/lo.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/lt.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/nl.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/pl.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/pt.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/ro.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/ru.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/sl.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/tr.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/uk.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/locale/zh_CN.po` & `trytond_account_stock_anglo_saxon-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/message.xml` & `trytond_account_stock_anglo_saxon-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart.xml` & `trytond_account_stock_anglo_saxon-7.2.1/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_bg.xml` & `trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_ca.xml` & `trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_de.xml` & `trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_en.xml` & `trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_es.xml` & `trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_fr.xml` & `trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_nl.xml` & `trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_pt.xml` & `trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_ru.xml` & `trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/minimal_chart_sl.xml` & `trytond_account_stock_anglo_saxon-7.2.1/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/product.py` & `trytond_account_stock_anglo_saxon-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/setup.py` & `trytond_account_stock_anglo_saxon-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/stock.py` & `trytond_account_stock_anglo_saxon-7.2.1/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         assert type_.startswith('in_') or type_.startswith('out_'), \
             'wrong type'
 
         total_qty = Uom.compute_qty(
             unit, quantity, product.default_uom, round=False)
 
         as_qty_field = _get_field(type_)
-        cost = Decimal('0.0')
+        cost = Decimal(0)
         consumed_qty = 0.0
         for move, move_qty, move_cost_price in cls._get_anglo_saxon_move(
                 moves, total_qty, type_):
             consumed_qty += move_qty
 
             cost += move_cost_price * Decimal(str(move_qty))
```

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/tests/scenario_account_stock_anglo_saxon.rst` & `trytond_account_stock_anglo_saxon-7.2.1/tests/scenario_account_stock_anglo_saxon.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst` & `trytond_account_stock_anglo_saxon-7.2.1/tests/scenario_account_stock_anglo_saxon_with_drop_shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/tests/test_module.py` & `trytond_account_stock_anglo_saxon-7.2.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/tests/tools.py` & `trytond_account_stock_anglo_saxon-7.2.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/tox.ini` & `trytond_account_stock_anglo_saxon-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO` & `trytond_account_stock_anglo_saxon-7.2.1/trytond_account_stock_anglo_saxon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_anglo_saxon
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for anglo-saxon real-time stock valuation
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_stock_anglo_saxon-7.2.0/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt` & `trytond_account_stock_anglo_saxon-7.2.1/trytond_account_stock_anglo_saxon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

