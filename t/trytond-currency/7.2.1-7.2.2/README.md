# Comparing `tmp/trytond_currency-7.2.1.tar.gz` & `tmp/trytond_currency-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_currency-7.2.1.tar", last modified: Wed May  1 11:59:21 2024, max compression
+gzip compressed data, was "trytond_currency-7.2.2.tar", last modified: Sun Jun  2 18:15:01 2024, max compression
```

## Comparing `trytond_currency-7.2.1.tar` & `trytond_currency-7.2.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     4085 2024-05-01 11:59:18.000000 trytond_currency-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-05-01 11:59:18.000000 trytond_currency-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2969 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15628 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/currency.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6457 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/currency.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.760269 trytond_currency-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      668 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1797 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      431 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2217 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3150 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/ecb.py
--rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1364 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/fields.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.760269 trytond_currency-7.2.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/icons/tryton-currency.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     1127 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.760269 trytond_currency-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5012 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5977 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4810 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5914 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6014 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4597 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5185 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5949 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4797 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5901 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5480 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4825 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5615 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5532 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5369 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5853 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5791 2024-04-30 17:21:59.000000 trytond_currency-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5654 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5806 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5186 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5594 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4797 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6453 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5508 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      722 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/message.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.760269 trytond_currency-7.2.1/scripts/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/scripts/__init__.py
--rwxr-xr-x   0 ced       (1000) ced       (1000)     3222 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/scripts/import_currencies.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4801 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      584 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/scenario_currency_compute.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/scenario_currency_import.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1296 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/scenario_currency_rate_update.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14824 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)       85 2024-04-30 17:21:06.000000 trytond_currency-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/trytond_currency.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2969 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2309 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      163 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      148 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:59:21.000000 trytond_currency-7.2.1/trytond_currency.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:59:21.763603 trytond_currency-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/cron_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      854 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/currency_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/currency_rate_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      311 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/currency_rate_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/currency_rate_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-30 17:20:59.000000 trytond_currency-7.2.1/view/currency_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 18:15:01.849930 trytond_currency-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4186 2024-06-02 18:14:58.000000 trytond_currency-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      728 2024-06-02 18:14:58.000000 trytond_currency-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2969 2024-06-02 18:15:01.849930 trytond_currency-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      470 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15624 2024-05-26 17:46:37.000000 trytond_currency-7.2.2/currency.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6457 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/currency.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 18:15:01.843263 trytond_currency-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      668 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1797 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      431 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      474 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/doc/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2217 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3150 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/ecb.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      225 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1364 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/fields.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 18:15:01.846596 trytond_currency-7.2.2/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      495 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/icons/tryton-currency.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1127 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 18:15:01.846596 trytond_currency-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5012 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5977 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4810 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5914 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6014 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4597 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5185 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5949 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4797 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5901 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5480 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4825 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5615 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5532 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5369 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5853 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5791 2024-04-30 17:21:59.000000 trytond_currency-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5654 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5806 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5186 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5594 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4797 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6453 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5508 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      722 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/message.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 18:15:01.846596 trytond_currency-7.2.2/scripts/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/scripts/__init__.py
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3222 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/scripts/import_currencies.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 18:15:01.849930 trytond_currency-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4801 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 18:15:01.849930 trytond_currency-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      257 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      584 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/tests/scenario_currency_compute.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/tests/scenario_currency_import.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1296 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/tests/scenario_currency_rate_update.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14824 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)       85 2024-05-01 11:59:28.000000 trytond_currency-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 18:15:01.849930 trytond_currency-7.2.2/trytond_currency.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2969 2024-06-02 18:15:01.000000 trytond_currency-7.2.2/trytond_currency.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2309 2024-06-02 18:15:01.000000 trytond_currency-7.2.2/trytond_currency.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 18:15:01.000000 trytond_currency-7.2.2/trytond_currency.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      163 2024-06-02 18:15:01.000000 trytond_currency-7.2.2/trytond_currency.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:59:21.000000 trytond_currency-7.2.2/trytond_currency.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      148 2024-06-02 18:15:01.000000 trytond_currency-7.2.2/trytond_currency.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 18:15:01.000000 trytond_currency-7.2.2/trytond_currency.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 18:15:01.849930 trytond_currency-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      724 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/view/cron_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      854 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/view/currency_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/view/currency_rate_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      311 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/view/currency_rate_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      287 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/view/currency_rate_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-30 17:20:59.000000 trytond_currency-7.2.2/view/currency_tree.xml
```

### Comparing `trytond_currency-7.2.1/CHANGELOG` & `trytond_currency-7.2.2/CHANGELOG`

 * *Files 1% similar despite different names*

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

### Comparing `trytond_currency-7.2.1/COPYRIGHT` & `trytond_currency-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/LICENSE` & `trytond_currency-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/PKG-INFO` & `trytond_currency-7.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_currency
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module with currencies
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_currency-7.2.1/currency.py` & `trytond_currency-7.2.2/currency.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             return [(field,) + tuple(clause[1:])]
         return [(cls._rec_name,) + tuple(clause[1:])]
 
     @fields.depends('rates')
     def on_change_with_rate(self):
         now = datetime.date.today()
         closer = datetime.date.min
-        res = Decimal('0.0')
+        res = Decimal(0)
         for rate in self.rates or []:
             date = getattr(rate, 'date', None) or now
             if date <= now and date > closer:
                 res = rate.rate
                 closer = date
         return res
```

### Comparing `trytond_currency-7.2.1/currency.xml` & `trytond_currency-7.2.2/currency.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/doc/conf.py` & `trytond_currency-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/doc/configuration.rst` & `trytond_currency-7.2.2/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/doc/design.rst` & `trytond_currency-7.2.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/doc/usage.rst` & `trytond_currency-7.2.2/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/ecb.py` & `trytond_currency-7.2.2/ecb.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/fields.py` & `trytond_currency-7.2.2/fields.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/icons/LICENSE` & `trytond_currency-7.2.2/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/ir.py` & `trytond_currency-7.2.2/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/bg.po` & `trytond_currency-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/ca.po` & `trytond_currency-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/cs.po` & `trytond_currency-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/de.po` & `trytond_currency-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/es.po` & `trytond_currency-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/es_419.po` & `trytond_currency-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/et.po` & `trytond_currency-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/fa.po` & `trytond_currency-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/fi.po` & `trytond_currency-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/fr.po` & `trytond_currency-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/hu.po` & `trytond_currency-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/id.po` & `trytond_currency-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/it.po` & `trytond_currency-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/lo.po` & `trytond_currency-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/lt.po` & `trytond_currency-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/nl.po` & `trytond_currency-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/pl.po` & `trytond_currency-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/pt.po` & `trytond_currency-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/ro.po` & `trytond_currency-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/ru.po` & `trytond_currency-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/sl.po` & `trytond_currency-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/tr.po` & `trytond_currency-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/uk.po` & `trytond_currency-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/locale/zh_CN.po` & `trytond_currency-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/message.xml` & `trytond_currency-7.2.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/scripts/import_currencies.py` & `trytond_currency-7.2.2/scripts/import_currencies.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/setup.py` & `trytond_currency-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/tests/scenario_currency_compute.rst` & `trytond_currency-7.2.2/tests/scenario_currency_compute.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/tests/scenario_currency_rate_update.rst` & `trytond_currency-7.2.2/tests/scenario_currency_rate_update.rst`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/tests/test_module.py` & `trytond_currency-7.2.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/tests/tools.py` & `trytond_currency-7.2.2/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/tox.ini` & `trytond_currency-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/trytond_currency.egg-info/PKG-INFO` & `trytond_currency-7.2.2/trytond_currency.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_currency
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module with currencies
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_currency-7.2.1/trytond_currency.egg-info/SOURCES.txt` & `trytond_currency-7.2.2/trytond_currency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/view/cron_form.xml` & `trytond_currency-7.2.2/view/cron_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_currency-7.2.1/view/currency_form.xml` & `trytond_currency-7.2.2/view/currency_form.xml`

 * *Files identical despite different names*

