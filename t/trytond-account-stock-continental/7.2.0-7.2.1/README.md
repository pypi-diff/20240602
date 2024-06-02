# Comparing `tmp/trytond_account_stock_continental-7.2.0.tar.gz` & `tmp/trytond_account_stock_continental-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_stock_continental-7.2.0.tar", last modified: Mon Apr 29 15:36:31 2024, max compression
+gzip compressed data, was "trytond_account_stock_continental-7.2.1.tar", last modified: Sun Jun  2 16:46:29 2024, max compression
```

## Comparing `trytond_account_stock_continental-7.2.0.tar` & `trytond_account_stock_continental-7.2.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:31.388904 trytond_account_stock_continental-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2812 2024-04-29 15:16:33.000000 trytond_account_stock_continental-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-04-29 15:16:33.000000 trytond_account_stock_continental-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_stock_continental-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3953 2024-04-29 15:36:31.388904 trytond_account_stock_continental-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-01-27 09:58:52.000000 trytond_account_stock_continental-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      571 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1231 2024-04-27 16:30:39.000000 trytond_account_stock_continental-7.2.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:31.385571 trytond_account_stock_continental-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-27 16:30:39.000000 trytond_account_stock_continental-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-01-27 09:58:52.000000 trytond_account_stock_continental-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:01.000000 trytond_account_stock_continental-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:31.388904 trytond_account_stock_continental-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1321 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1654 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1626 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1653 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1637 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1462 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1659 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1571 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1550 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1323 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1572 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1328 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1351 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1556 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1308 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1601 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1335 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1525 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-27 16:43:21.000000 trytond_account_stock_continental-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4058 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/minimal_chart.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2188 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/minimal_chart_bg.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2142 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/minimal_chart_ca.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2132 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/minimal_chart_de.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2128 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/minimal_chart_en.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2144 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/minimal_chart_es.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2142 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/minimal_chart_fr.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2121 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/minimal_chart_nl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2141 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/minimal_chart_pt.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2192 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/minimal_chart_ru.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2126 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/minimal_chart_sl.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     8111 2024-01-27 09:58:52.000000 trytond_account_stock_continental-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:36:31.388904 trytond_account_stock_continental-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4696 2024-03-17 11:01:36.000000 trytond_account_stock_continental-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6426 2024-02-04 18:51:26.000000 trytond_account_stock_continental-7.2.0/stock.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:31.388904 trytond_account_stock_continental-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11909 2024-04-27 16:30:39.000000 trytond_account_stock_continental-7.2.0/tests/scenario_account_stock_continental.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      747 2024-01-27 09:58:52.000000 trytond_account_stock_continental-7.2.0/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:01.000000 trytond_account_stock_continental-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      376 2024-04-29 15:16:27.000000 trytond_account_stock_continental-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:31.388904 trytond_account_stock_continental-7.2.0/trytond_account_stock_continental.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3953 2024-04-29 15:36:30.000000 trytond_account_stock_continental-7.2.0/trytond_account_stock_continental.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2244 2024-04-29 15:36:31.000000 trytond_account_stock_continental-7.2.0/trytond_account_stock_continental.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:36:30.000000 trytond_account_stock_continental-7.2.0/trytond_account_stock_continental.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-04-29 15:36:30.000000 trytond_account_stock_continental-7.2.0/trytond_account_stock_continental.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:04.000000 trytond_account_stock_continental-7.2.0/trytond_account_stock_continental.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2024-04-29 15:36:30.000000 trytond_account_stock_continental-7.2.0/trytond_account_stock_continental.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:36:30.000000 trytond_account_stock_continental-7.2.0/trytond_account_stock_continental.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:36:31.388904 trytond_account_stock_continental-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      581 2023-04-15 07:12:15.000000 trytond_account_stock_continental-7.2.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      415 2024-02-04 18:51:26.000000 trytond_account_stock_continental-7.2.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-01-16 14:00:20.000000 trytond_account_stock_continental-7.2.0/view/fiscalyear_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:46:29.755530 trytond_account_stock_continental-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2913 2024-06-02 16:46:26.000000 trytond_account_stock_continental-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2024-06-02 16:46:26.000000 trytond_account_stock_continental-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3953 2024-06-02 16:46:29.752197 trytond_account_stock_continental-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      571 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1508 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1231 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:46:29.748864 trytond_account_stock_continental-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3088 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1104 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:46:29.752197 trytond_account_stock_continental-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1321 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1654 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1626 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1653 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1637 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1462 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1659 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1571 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1550 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1323 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1572 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1328 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1351 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1556 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1308 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1601 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1335 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1525 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1304 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4058 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/minimal_chart.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2188 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/minimal_chart_bg.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2142 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/minimal_chart_ca.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2132 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/minimal_chart_de.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2128 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/minimal_chart_en.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2144 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/minimal_chart_es.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2142 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/minimal_chart_fr.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2121 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/minimal_chart_nl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2141 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/minimal_chart_pt.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2192 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/minimal_chart_ru.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2126 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/minimal_chart_sl.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     8111 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 16:46:29.755530 trytond_account_stock_continental-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4696 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6402 2024-05-26 17:46:37.000000 trytond_account_stock_continental-7.2.1/stock.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:46:29.752197 trytond_account_stock_continental-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11909 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/tests/scenario_account_stock_continental.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      747 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2024-04-30 17:21:06.000000 trytond_account_stock_continental-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:46:29.752197 trytond_account_stock_continental-7.2.1/trytond_account_stock_continental.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3953 2024-06-02 16:46:29.000000 trytond_account_stock_continental-7.2.1/trytond_account_stock_continental.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2244 2024-06-02 16:46:29.000000 trytond_account_stock_continental-7.2.1/trytond_account_stock_continental.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 16:46:29.000000 trytond_account_stock_continental-7.2.1/trytond_account_stock_continental.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       88 2024-06-02 16:46:29.000000 trytond_account_stock_continental-7.2.1/trytond_account_stock_continental.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 14:11:51.000000 trytond_account_stock_continental-7.2.1/trytond_account_stock_continental.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2024-06-02 16:46:29.000000 trytond_account_stock_continental-7.2.1/trytond_account_stock_continental.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 16:46:29.000000 trytond_account_stock_continental-7.2.1/trytond_account_stock_continental.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:46:29.752197 trytond_account_stock_continental-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      581 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      415 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2024-04-30 17:20:59.000000 trytond_account_stock_continental-7.2.1/view/fiscalyear_form.xml
```

### Comparing `trytond_account_stock_continental-7.2.0/CHANGELOG` & `trytond_account_stock_continental-7.2.1/CHANGELOG`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_account_stock_continental-7.2.0/COPYRIGHT` & `trytond_account_stock_continental-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/LICENSE` & `trytond_account_stock_continental-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/PKG-INFO` & `trytond_account_stock_continental-7.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_continental
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for continental real-time stock valuation
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_stock_continental-7.2.0/README.rst` & `trytond_account_stock_continental-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/__init__.py` & `trytond_account_stock_continental-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/account.py` & `trytond_account_stock_continental-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/account.xml` & `trytond_account_stock_continental-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/doc/conf.py` & `trytond_account_stock_continental-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/doc/index.rst` & `trytond_account_stock_continental-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/bg.po` & `trytond_account_stock_continental-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/ca.po` & `trytond_account_stock_continental-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/cs.po` & `trytond_account_stock_continental-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/de.po` & `trytond_account_stock_continental-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/es.po` & `trytond_account_stock_continental-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/es_419.po` & `trytond_account_stock_continental-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/et.po` & `trytond_account_stock_continental-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/fa.po` & `trytond_account_stock_continental-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/fi.po` & `trytond_account_stock_continental-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/fr.po` & `trytond_account_stock_continental-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/hu.po` & `trytond_account_stock_continental-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/id.po` & `trytond_account_stock_continental-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/it.po` & `trytond_account_stock_continental-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/lo.po` & `trytond_account_stock_continental-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/lt.po` & `trytond_account_stock_continental-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/nl.po` & `trytond_account_stock_continental-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/pl.po` & `trytond_account_stock_continental-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/pt.po` & `trytond_account_stock_continental-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/ro.po` & `trytond_account_stock_continental-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/ru.po` & `trytond_account_stock_continental-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/sl.po` & `trytond_account_stock_continental-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/tr.po` & `trytond_account_stock_continental-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/uk.po` & `trytond_account_stock_continental-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/locale/zh_CN.po` & `trytond_account_stock_continental-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/minimal_chart.xml` & `trytond_account_stock_continental-7.2.1/minimal_chart.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/minimal_chart_bg.xml` & `trytond_account_stock_continental-7.2.1/minimal_chart_bg.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/minimal_chart_ca.xml` & `trytond_account_stock_continental-7.2.1/minimal_chart_ca.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/minimal_chart_de.xml` & `trytond_account_stock_continental-7.2.1/minimal_chart_de.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/minimal_chart_en.xml` & `trytond_account_stock_continental-7.2.1/minimal_chart_en.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/minimal_chart_es.xml` & `trytond_account_stock_continental-7.2.1/minimal_chart_es.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/minimal_chart_fr.xml` & `trytond_account_stock_continental-7.2.1/minimal_chart_fr.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/minimal_chart_nl.xml` & `trytond_account_stock_continental-7.2.1/minimal_chart_nl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/minimal_chart_pt.xml` & `trytond_account_stock_continental-7.2.1/minimal_chart_pt.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/minimal_chart_ru.xml` & `trytond_account_stock_continental-7.2.1/minimal_chart_ru.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/minimal_chart_sl.xml` & `trytond_account_stock_continental-7.2.1/minimal_chart_sl.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/product.py` & `trytond_account_stock_continental-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/setup.py` & `trytond_account_stock_continental-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/stock.py` & `trytond_account_stock_continental-7.2.1/stock.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,20 +33,20 @@
             unit_price = self.cost_price
         unit_price = Uom.compute_price(
             self.product.default_uom, unit_price, self.unit)
         amount = self.company.currency.round(
                 Decimal(str(self.quantity)) * unit_price)
 
         if type_.startswith('in_'):
-            move_line.debit = Decimal('0.0')
+            move_line.debit = Decimal(0)
             move_line.credit = amount
             move_line.account = self.product.account_stock_in_used
         else:
             move_line.debit = amount
-            move_line.credit = Decimal('0.0')
+            move_line.credit = Decimal(0)
             move_line.account = self.product.account_stock_out_used
 
         return [move_line]
 
     def _get_account_stock_move_line(self, amount):
         '''
         Return counterpart move line value for stock move
@@ -54,20 +54,20 @@
         pool = Pool()
         AccountMoveLine = pool.get('account.move.line')
         move_line = AccountMoveLine(
             account=self.product.account_stock_used,
             )
         if not amount:
             return
-        if amount >= Decimal('0.0'):
-            move_line.debit = Decimal('0.0')
+        if amount >= Decimal(0):
+            move_line.debit = Decimal(0)
             move_line.credit = amount
         else:
             move_line.debit = - amount
-            move_line.credit = Decimal('0.0')
+            move_line.credit = Decimal(0)
         return move_line
 
     def _get_account_stock_move_type(self):
         '''
         Get account move type
         '''
         type_ = (self.from_location.type, self.to_location.type)
@@ -137,15 +137,15 @@
                 account_move_lines = self._get_account_stock_move_lines(
                     'in_customer')
                 account_move_lines.extend(self._get_account_stock_move_lines(
                         'out_supplier'))
             else:
                 account_move_lines = self._get_account_stock_move_lines(type_)
 
-        amount = Decimal('0.0')
+        amount = Decimal(0)
         for line in account_move_lines:
             amount += line.debit - line.credit
 
         if not amount:
             return
         move_line = self._get_account_stock_move_line(amount)
         if move_line:
```

### Comparing `trytond_account_stock_continental-7.2.0/tests/scenario_account_stock_continental.rst` & `trytond_account_stock_continental-7.2.1/tests/scenario_account_stock_continental.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/tests/tools.py` & `trytond_account_stock_continental-7.2.1/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/tox.ini` & `trytond_account_stock_continental-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/trytond_account_stock_continental.egg-info/PKG-INFO` & `trytond_account_stock_continental-7.2.1/trytond_account_stock_continental.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_stock_continental
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module for continental real-time stock valuation
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_stock_continental-7.2.0/trytond_account_stock_continental.egg-info/SOURCES.txt` & `trytond_account_stock_continental-7.2.1/trytond_account_stock_continental.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_stock_continental-7.2.0/view/category_form.xml` & `trytond_account_stock_continental-7.2.1/view/category_form.xml`

 * *Files identical despite different names*

