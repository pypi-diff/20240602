# Comparing `tmp/trytond_web_shop_product_data_feed-7.2.1.tar.gz` & `tmp/trytond_web_shop_product_data_feed-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop_product_data_feed-7.2.1.tar", last modified: Wed May  1 09:50:58 2024, max compression
+gzip compressed data, was "trytond_web_shop_product_data_feed-7.2.2.tar", last modified: Sun Jun  2 15:58:37 2024, max compression
```

## Comparing `trytond_web_shop_product_data_feed-7.2.1.tar` & `trytond_web_shop_product_data_feed-7.2.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.296672 trytond_web_shop_product_data_feed-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)      172 2024-05-01 09:50:55.000000 trytond_web_shop_product_data_feed-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      670 2024-05-01 09:50:55.000000 trytond_web_shop_product_data_feed-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2955 2024-05-01 09:50:58.296672 trytond_web_shop_product_data_feed-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      933 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.293338 trytond_web_shop_product_data_feed-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1778 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      555 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      557 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/doc/usage.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.293338 trytond_web_shop_product_data_feed-7.2.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/icons/LICENSE
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.293338 trytond_web_shop_product_data_feed-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2682 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2602 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2671 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2686 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     2638 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1516 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6208 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      801 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:50:58.296672 trytond_web_shop_product_data_feed-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4864 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.293338 trytond_web_shop_product_data_feed-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/tests/google-products.csv
--rw-r--r--   0 ced       (1000) ced       (1000)     5485 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      176 2024-04-30 17:21:06.000000 trytond_web_shop_product_data_feed-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.296672 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2955 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2035 2024-05-01 09:50:58.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      185 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:50:58.296672 trytond_web_shop_product_data_feed-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/product_category_facebook_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/product_category_facebook_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/product_category_google_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/product_category_google_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/view/web_shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    14227 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)      469 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.1/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:58:37.483986 trytond_web_shop_product_data_feed-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)      273 2024-06-02 15:58:34.000000 trytond_web_shop_product_data_feed-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      670 2024-06-02 15:58:34.000000 trytond_web_shop_product_data_feed-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3030 2024-06-02 15:58:37.483986 trytond_web_shop_product_data_feed-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1091 2024-05-26 17:41:55.000000 trytond_web_shop_product_data_feed-7.2.2/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:58:37.480653 trytond_web_shop_product_data_feed-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3089 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1778 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      395 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      555 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      557 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/doc/usage.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:58:37.480653 trytond_web_shop_product_data_feed-7.2.2/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/icons/LICENSE
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:58:37.483986 trytond_web_shop_product_data_feed-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2682 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2602 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2671 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2686 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     2638 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1969 2024-04-30 17:21:59.000000 trytond_web_shop_product_data_feed-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1516 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6208 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      801 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 15:58:37.483986 trytond_web_shop_product_data_feed-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4925 2024-05-26 17:41:55.000000 trytond_web_shop_product_data_feed-7.2.2/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:58:37.483986 trytond_web_shop_product_data_feed-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/tests/google-products.csv
+-rw-r--r--   0 ced       (1000) ced       (1000)     5530 2024-05-26 17:41:55.000000 trytond_web_shop_product_data_feed-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      205 2024-05-26 17:41:55.000000 trytond_web_shop_product_data_feed-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:58:37.483986 trytond_web_shop_product_data_feed-7.2.2/trytond_web_shop_product_data_feed.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3030 2024-06-02 15:58:37.000000 trytond_web_shop_product_data_feed-7.2.2/trytond_web_shop_product_data_feed.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2035 2024-06-02 15:58:37.000000 trytond_web_shop_product_data_feed-7.2.2/trytond_web_shop_product_data_feed.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 15:58:37.000000 trytond_web_shop_product_data_feed-7.2.2/trytond_web_shop_product_data_feed.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-06-02 15:58:37.000000 trytond_web_shop_product_data_feed-7.2.2/trytond_web_shop_product_data_feed.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:50:57.000000 trytond_web_shop_product_data_feed-7.2.2/trytond_web_shop_product_data_feed.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      228 2024-06-02 15:58:37.000000 trytond_web_shop_product_data_feed-7.2.2/trytond_web_shop_product_data_feed.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 15:58:37.000000 trytond_web_shop_product_data_feed-7.2.2/trytond_web_shop_product_data_feed.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:58:37.483986 trytond_web_shop_product_data_feed-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/view/product_category_facebook_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/view/product_category_facebook_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/view/product_category_google_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      247 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/view/product_category_google_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/view/web_shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    14930 2024-05-26 17:41:55.000000 trytond_web_shop_product_data_feed-7.2.2/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      469 2024-04-30 17:21:00.000000 trytond_web_shop_product_data_feed-7.2.2/web.xml
```

### Comparing `trytond_web_shop_product_data_feed-7.2.1/COPYRIGHT` & `trytond_web_shop_product_data_feed-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/LICENSE` & `trytond_web_shop_product_data_feed-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/PKG-INFO` & `trytond_web_shop_product_data_feed-7.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_product_data_feed
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module to expose product data feed
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
@@ -51,14 +51,15 @@
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: trytond_product<7.3,>=7.2
 Requires-Dist: trytond_web_shop<7.3,>=7.2
 Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
+Requires-Dist: trytond_account_tax_rule_country<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_product_kit<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_product_measurements<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
 
 #################################
 Web Shop Product Data Feed Module
 #################################
```

### Comparing `trytond_web_shop_product_data_feed-7.2.1/__init__.py` & `trytond_web_shop_product_data_feed-7.2.2/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,7 +25,11 @@
         web.Shop_Measurement,
         module='web_shop_product_data_feed', type_='model',
         depends=['product_measurements'])
     Pool.register(
         web.Shop_ShipmentCost,
         module='web_shop_product_data_feed', type_='model',
         depends=['sale_shipment_cost'])
+    Pool.register(
+        web.Shop_TaxRuleCountry,
+        module='web_shop_product_data_feed', type_='model',
+        depends=['account_tax_rule_country'])
```

### Comparing `trytond_web_shop_product_data_feed-7.2.1/doc/conf.py` & `trytond_web_shop_product_data_feed-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/doc/design.rst` & `trytond_web_shop_product_data_feed-7.2.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/doc/reference.rst` & `trytond_web_shop_product_data_feed-7.2.2/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/doc/usage.rst` & `trytond_web_shop_product_data_feed-7.2.2/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/icons/LICENSE` & `trytond_web_shop_product_data_feed-7.2.2/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/bg.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/ca.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/cs.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/de.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/es.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/es_419.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/et.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/fa.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/fi.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/fr.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/hu.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/id.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/it.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/lo.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/lt.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/nl.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/pl.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/pt.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/ro.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/ru.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/sl.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/tr.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/uk.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/locale/zh_CN.po` & `trytond_web_shop_product_data_feed-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/product.py` & `trytond_web_shop_product_data_feed-7.2.2/product.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/product.xml` & `trytond_web_shop_product_data_feed-7.2.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/routes.py` & `trytond_web_shop_product_data_feed-7.2.2/routes.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/setup.py` & `trytond_web_shop_product_data_feed-7.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
+    get_require_version('trytond_account_tax_rule_country'),
     get_require_version('trytond_product_kit'),
     get_require_version('trytond_product_measurements'),
     get_require_version('trytond_sale_shipment_cost'),
     ]
 
 setup(name=name,
     version=version,
```

### Comparing `trytond_web_shop_product_data_feed-7.2.1/tests/test_module.py` & `trytond_web_shop_product_data_feed-7.2.2/tests/test_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from trytond.tests.test_tryton import (
     ModuleTestCase, RouteTestCase, with_transaction)
 
 
 class WebShopProductDataFeedTestCase(ModuleTestCase):
     "Test Web Shop Product Data Feed module"
     module = 'web_shop_product_data_feed'
-    extras = ['product_kit', 'product_measurements', 'sale_shipment_cost']
+    extras = [
+        'account_tax_rule_country', 'product_kit', 'product_measurements',
+        'sale_shipment_cost']
 
     @with_transaction()
     def test_data_feed(self):
         "Test data feed"
         pool = Pool()
         Account = pool.get('account.account')
         Carrier = pool.get('carrier')
```

### Comparing `trytond_web_shop_product_data_feed-7.2.1/tox.ini` & `trytond_web_shop_product_data_feed-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/PKG-INFO` & `trytond_web_shop_product_data_feed-7.2.2/trytond_web_shop_product_data_feed.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop_product_data_feed
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module to expose product data feed
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
@@ -51,14 +51,15 @@
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: trytond_product<7.3,>=7.2
 Requires-Dist: trytond_web_shop<7.3,>=7.2
 Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
+Requires-Dist: trytond_account_tax_rule_country<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_product_kit<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_product_measurements<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_sale_shipment_cost<7.3,>=7.2; extra == "test"
 
 #################################
 Web Shop Product Data Feed Module
 #################################
```

### Comparing `trytond_web_shop_product_data_feed-7.2.1/trytond_web_shop_product_data_feed.egg-info/SOURCES.txt` & `trytond_web_shop_product_data_feed-7.2.2/trytond_web_shop_product_data_feed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_web_shop_product_data_feed-7.2.1/web.py` & `trytond_web_shop_product_data_feed-7.2.2/web.py`

 * *Files 9% similar despite different names*

```diff
@@ -392,7 +392,25 @@
                     product, country, carrier, price)
                 if cost is not None:
                     shipping.append(
                         f'{country.code}::{carrier.carrier_product.name}:'
                         f'{cost} {self.currency.code}')
         row['shipping'] = ','.join(shipping)
         return row
+
+
+class Shop_TaxRuleCountry(metaclass=PoolMeta):
+    __name__ = 'web.shop'
+
+    def _product_data_feed_carrier_cost(
+            self, product, country, carrier, price, pattern=None):
+        pattern = pattern.copy() if pattern is not None else {}
+        if (self.warehouse
+                and self.warehouse.address
+                and self.warehouse.address.country):
+            pattern.setdefault(
+                'from_country', self.warehouse.address.country.id)
+        else:
+            pattern.setdefault('from_country')
+        pattern.setdefault('to_country', country.id)
+        return super()._product_data_feed_carrier_cost(
+            product, country, carrier, price, pattern=pattern)
```

