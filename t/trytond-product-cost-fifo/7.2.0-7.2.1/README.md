# Comparing `tmp/trytond_product_cost_fifo-7.2.0.tar.gz` & `tmp/trytond_product_cost_fifo-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_product_cost_fifo-7.2.0.tar", last modified: Mon Apr 29 15:42:48 2024, max compression
+gzip compressed data, was "trytond_product_cost_fifo-7.2.1.tar", last modified: Sun Jun  2 16:32:20 2024, max compression
```

## Comparing `trytond_product_cost_fifo-7.2.0.tar` & `trytond_product_cost_fifo-7.2.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:48.752368 trytond_product_cost_fifo-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2759 2024-04-29 15:21:34.000000 trytond_product_cost_fifo-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-04-29 15:21:33.000000 trytond_product_cost_fifo-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-04-29 15:42:48.752368 trytond_product_cost_fifo-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:48.749035 trytond_product_cost_fifo-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-27 16:30:39.000000 trytond_product_cost_fifo-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2023-01-16 14:00:20.000000 trytond_product_cost_fifo-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:15.000000 trytond_product_cost_fifo-7.2.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:48.749035 trytond_product_cost_fifo-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1125 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1427 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1480 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1434 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1306 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1538 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1492 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1214 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1513 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1478 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1465 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1208 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1417 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1175 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-27 16:43:24.000000 trytond_product_cost_fifo-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      827 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6559 2024-02-04 18:51:26.000000 trytond_product_cost_fifo-7.2.0/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9974 2024-02-04 18:51:26.000000 trytond_product_cost_fifo-7.2.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:42:48.752368 trytond_product_cost_fifo-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4473 2024-03-17 11:01:36.000000 trytond_product_cost_fifo-7.2.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:48.752368 trytond_product_cost_fifo-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4836 2024-04-22 12:14:36.000000 trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3233 2024-04-22 12:14:36.000000 trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_no_in.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4837 2024-04-22 12:14:36.000000 trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_recompute_cost_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3406 2024-04-22 12:14:36.000000 trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4610 2024-04-22 12:14:36.000000 trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_uom.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      335 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_product_cost_fifo-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:15.000000 trytond_product_cost_fifo-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-29 15:21:29.000000 trytond_product_cost_fifo-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:42:48.752368 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1902 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:01.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      105 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:42:48.000000 trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:32:20.261082 trytond_product_cost_fifo-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2860 2024-06-02 16:32:16.000000 trytond_product_cost_fifo-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-06-02 16:32:16.000000 trytond_product_cost_fifo-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-06-02 16:32:20.261082 trytond_product_cost_fifo-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:32:20.254415 trytond_product_cost_fifo-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:32:20.257748 trytond_product_cost_fifo-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1125 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1427 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1480 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1434 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1306 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1538 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1492 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1214 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1513 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1478 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1465 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1208 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1417 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1175 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      827 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6555 2024-05-26 17:46:37.000000 trytond_product_cost_fifo-7.2.1/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9974 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 16:32:20.261082 trytond_product_cost_fifo-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4473 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:32:20.257748 trytond_product_cost_fifo-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4836 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/tests/scenario_product_cost_fifo.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3233 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/tests/scenario_product_cost_fifo_no_in.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4837 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/tests/scenario_product_cost_fifo_recompute_cost_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3406 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4610 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/tests/scenario_product_cost_fifo_uom.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      335 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_product_cost_fifo-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-04-30 17:21:06.000000 trytond_product_cost_fifo-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:32:20.257748 trytond_product_cost_fifo-7.2.1/trytond_product_cost_fifo.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-06-02 16:32:19.000000 trytond_product_cost_fifo-7.2.1/trytond_product_cost_fifo.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1902 2024-06-02 16:32:20.000000 trytond_product_cost_fifo-7.2.1/trytond_product_cost_fifo.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 16:32:19.000000 trytond_product_cost_fifo-7.2.1/trytond_product_cost_fifo.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-06-02 16:32:19.000000 trytond_product_cost_fifo-7.2.1/trytond_product_cost_fifo.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 14:11:52.000000 trytond_product_cost_fifo-7.2.1/trytond_product_cost_fifo.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      105 2024-06-02 16:32:19.000000 trytond_product_cost_fifo-7.2.1/trytond_product_cost_fifo.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 16:32:19.000000 trytond_product_cost_fifo-7.2.1/trytond_product_cost_fifo.egg-info/top_level.txt
```

### Comparing `trytond_product_cost_fifo-7.2.0/CHANGELOG` & `trytond_product_cost_fifo-7.2.1/CHANGELOG`

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

### Comparing `trytond_product_cost_fifo-7.2.0/COPYRIGHT` & `trytond_product_cost_fifo-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/LICENSE` & `trytond_product_cost_fifo-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/PKG-INFO` & `trytond_product_cost_fifo-7.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product_cost_fifo
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add FIFO cost method
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product_cost_fifo-7.2.0/doc/conf.py` & `trytond_product_cost_fifo-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/bg.po` & `trytond_product_cost_fifo-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/ca.po` & `trytond_product_cost_fifo-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/cs.po` & `trytond_product_cost_fifo-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/de.po` & `trytond_product_cost_fifo-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/es.po` & `trytond_product_cost_fifo-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/es_419.po` & `trytond_product_cost_fifo-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/et.po` & `trytond_product_cost_fifo-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/fa.po` & `trytond_product_cost_fifo-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/fi.po` & `trytond_product_cost_fifo-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/fr.po` & `trytond_product_cost_fifo-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/hu.po` & `trytond_product_cost_fifo-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/id.po` & `trytond_product_cost_fifo-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/it.po` & `trytond_product_cost_fifo-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/lo.po` & `trytond_product_cost_fifo-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/lt.po` & `trytond_product_cost_fifo-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/nl.po` & `trytond_product_cost_fifo-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/pl.po` & `trytond_product_cost_fifo-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/pt.po` & `trytond_product_cost_fifo-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/ro.po` & `trytond_product_cost_fifo-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/ru.po` & `trytond_product_cost_fifo-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/sl.po` & `trytond_product_cost_fifo-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/tr.po` & `trytond_product_cost_fifo-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/uk.po` & `trytond_product_cost_fifo-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/locale/zh_CN.po` & `trytond_product_cost_fifo-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/message.xml` & `trytond_product_cost_fifo-7.2.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/move.py` & `trytond_product_cost_fifo-7.2.1/move.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
         total_qty = Uom.compute_qty(
             self.unit, self.quantity, self.product.default_uom, round=False)
 
         with Transaction().set_context(company=self.company.id):
             fifo_moves = self.product.get_fifo_move(total_qty)
 
-        cost_price = Decimal("0.0")
+        cost_price = Decimal(0)
         consumed_qty = 0.0
         to_save = []
         for move, move_qty in fifo_moves:
             consumed_qty += move_qty
             cost_price += move.get_cost_price() * Decimal(str(move_qty))
 
             move_qty = Uom.compute_qty(
```

### Comparing `trytond_product_cost_fifo-7.2.0/product.py` & `trytond_product_cost_fifo-7.2.1/product.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/setup.py` & `trytond_product_cost_fifo-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo.rst` & `trytond_product_cost_fifo-7.2.1/tests/scenario_product_cost_fifo.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_no_in.rst` & `trytond_product_cost_fifo-7.2.1/tests/scenario_product_cost_fifo_no_in.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_recompute_cost_price.rst` & `trytond_product_cost_fifo-7.2.1/tests/scenario_product_cost_fifo_recompute_cost_price.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst` & `trytond_product_cost_fifo-7.2.1/tests/scenario_product_cost_fifo_recompute_cost_price_production.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/tests/scenario_product_cost_fifo_uom.rst` & `trytond_product_cost_fifo-7.2.1/tests/scenario_product_cost_fifo_uom.rst`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/tox.ini` & `trytond_product_cost_fifo-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/PKG-INFO` & `trytond_product_cost_fifo-7.2.1/trytond_product_cost_fifo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_product_cost_fifo
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton module to add FIFO cost method
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_product_cost_fifo-7.2.0/trytond_product_cost_fifo.egg-info/SOURCES.txt` & `trytond_product_cost_fifo-7.2.1/trytond_product_cost_fifo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

