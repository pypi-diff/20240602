# Comparing `tmp/trytond_web_shop-7.2.1.tar.gz` & `tmp/trytond_web_shop-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop-7.2.1.tar", last modified: Wed May  1 09:51:23 2024, max compression
+gzip compressed data, was "trytond_web_shop-7.2.2.tar", last modified: Sun Jun  2 15:59:47 2024, max compression
```

## Comparing `trytond_web_shop-7.2.1.tar` & `trytond_web_shop-7.2.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.069357 trytond_web_shop-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1030 2024-05-01 09:51:20.000000 trytond_web_shop-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-05-01 09:51:19.000000 trytond_web_shop-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2863 2024-05-01 09:51:23.069357 trytond_web_shop-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      961 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.062691 trytond_web_shop-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.066024 trytond_web_shop-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6476 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6639 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6501 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6741 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5575 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5287 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5265 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6631 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6457 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     7294 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      754 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2419 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2222 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2208 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 09:51:23.069357 trytond_web_shop-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4517 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.066024 trytond_web_shop-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      459 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-30 17:21:06.000000 trytond_web_shop-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.066024 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2863 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2019 2024-05-01 09:51:23.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.1/trytond_web_shop.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 09:51:23.066024 trytond_web_shop-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_attribute_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_image_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_image_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/shop_attribute_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/shop_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/shop_price_list_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    12739 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3595 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.1/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:59:47.428823 trytond_web_shop-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1131 2024-06-02 15:59:44.000000 trytond_web_shop-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-06-02 15:59:44.000000 trytond_web_shop-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2938 2024-06-02 15:59:47.428823 trytond_web_shop-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1093 2024-05-26 17:41:55.000000 trytond_web_shop-7.2.2/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:59:47.425490 trytond_web_shop-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:59:47.425490 trytond_web_shop-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6476 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6639 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6501 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6741 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5575 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5287 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5265 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6631 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6457 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     7294 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:21:59.000000 trytond_web_shop-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      754 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2419 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2222 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2208 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 15:59:47.428823 trytond_web_shop-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4578 2024-05-26 17:41:55.000000 trytond_web_shop-7.2.2/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:59:47.428823 trytond_web_shop-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2024-05-26 17:41:55.000000 trytond_web_shop-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2024-05-26 17:41:55.000000 trytond_web_shop-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:59:47.428823 trytond_web_shop-7.2.2/trytond_web_shop.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2938 2024-06-02 15:59:46.000000 trytond_web_shop-7.2.2/trytond_web_shop.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2019 2024-06-02 15:59:47.000000 trytond_web_shop-7.2.2/trytond_web_shop.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 15:59:46.000000 trytond_web_shop-7.2.2/trytond_web_shop.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-06-02 15:59:46.000000 trytond_web_shop-7.2.2/trytond_web_shop.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 09:51:22.000000 trytond_web_shop-7.2.2/trytond_web_shop.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      376 2024-06-02 15:59:46.000000 trytond_web_shop-7.2.2/trytond_web_shop.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 15:59:46.000000 trytond_web_shop-7.2.2/trytond_web_shop.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 15:59:47.428823 trytond_web_shop-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/product_attribute_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/product_category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/product_image_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/product_image_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/product_product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/shop_attribute_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/shop_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/shop_price_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13298 2024-05-26 17:41:55.000000 trytond_web_shop-7.2.2/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3595 2024-04-30 17:21:00.000000 trytond_web_shop-7.2.2/web.xml
```

### Comparing `trytond_web_shop-7.2.1/CHANGELOG` & `trytond_web_shop-7.2.2/CHANGELOG`

 * *Files 15% similar despite different names*

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

### Comparing `trytond_web_shop-7.2.1/COPYRIGHT` & `trytond_web_shop-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/LICENSE` & `trytond_web_shop-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/PKG-INFO` & `trytond_web_shop-7.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module that provides a common base for webshops
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
@@ -55,14 +55,15 @@
 Requires-Dist: trytond_currency<7.3,>=7.2
 Requires-Dist: trytond_product<7.3,>=7.2
 Requires-Dist: trytond_sale<7.3,>=7.2
 Requires-Dist: trytond_stock<7.3,>=7.2
 Requires-Dist: trytond_web_user<7.3,>=7.2
 Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
+Requires-Dist: trytond_account_tax_rule_country<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_product_attribute<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_product_image<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_sale_price_list<7.3,>=7.2; extra == "test"
 
 Web Shop Module
 ###############
```

### Comparing `trytond_web_shop-7.2.1/__init__.py` & `trytond_web_shop-7.2.2/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,7 +28,10 @@
         module='web_shop', type_='model', depends=['product_attribute'])
     Pool.register(
         product.Image,
         module='web_shop', type_='model', depends=['product_image'])
     Pool.register(
         web.Shop_PriceList,
         module='web_shop', type_='model', depends=['sale_price_list'])
+    Pool.register(
+        web.Shop_TaxRuleCountry,
+        module='web_shop', type_='model', depends=['account_tax_rule_country'])
```

### Comparing `trytond_web_shop-7.2.1/doc/conf.py` & `trytond_web_shop-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/bg.po` & `trytond_web_shop-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/ca.po` & `trytond_web_shop-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/cs.po` & `trytond_web_shop-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/de.po` & `trytond_web_shop-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/es.po` & `trytond_web_shop-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/es_419.po` & `trytond_web_shop-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/et.po` & `trytond_web_shop-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/fa.po` & `trytond_web_shop-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/fi.po` & `trytond_web_shop-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/fr.po` & `trytond_web_shop-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/hu.po` & `trytond_web_shop-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/id.po` & `trytond_web_shop-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/it.po` & `trytond_web_shop-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/lo.po` & `trytond_web_shop-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/lt.po` & `trytond_web_shop-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/nl.po` & `trytond_web_shop-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/pl.po` & `trytond_web_shop-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/pt.po` & `trytond_web_shop-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/ro.po` & `trytond_web_shop-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/ru.po` & `trytond_web_shop-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/sl.po` & `trytond_web_shop-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/tr.po` & `trytond_web_shop-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/uk.po` & `trytond_web_shop-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/locale/zh_CN.po` & `trytond_web_shop-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/message.xml` & `trytond_web_shop-7.2.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/product.py` & `trytond_web_shop-7.2.2/product.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/product.xml` & `trytond_web_shop-7.2.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/sale.py` & `trytond_web_shop-7.2.2/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/setup.py` & `trytond_web_shop-7.2.2/setup.py`

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
     get_require_version('trytond_product_attribute'),
     get_require_version('trytond_product_image'),
     get_require_version('trytond_sale_price_list'),
     ]
 
 setup(name=name,
     version=version,
```

### Comparing `trytond_web_shop-7.2.1/tox.ini` & `trytond_web_shop-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/trytond_web_shop.egg-info/PKG-INFO` & `trytond_web_shop-7.2.2/trytond_web_shop.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module that provides a common base for webshops
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
@@ -55,14 +55,15 @@
 Requires-Dist: trytond_currency<7.3,>=7.2
 Requires-Dist: trytond_product<7.3,>=7.2
 Requires-Dist: trytond_sale<7.3,>=7.2
 Requires-Dist: trytond_stock<7.3,>=7.2
 Requires-Dist: trytond_web_user<7.3,>=7.2
 Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
+Requires-Dist: trytond_account_tax_rule_country<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_product_attribute<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_product_image<7.3,>=7.2; extra == "test"
 Requires-Dist: trytond_sale_price_list<7.3,>=7.2; extra == "test"
 
 Web Shop Module
 ###############
```

### Comparing `trytond_web_shop-7.2.1/trytond_web_shop.egg-info/SOURCES.txt` & `trytond_web_shop-7.2.2/trytond_web_shop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/view/shop_form.xml` & `trytond_web_shop-7.2.2/view/shop_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.2.1/web.py` & `trytond_web_shop-7.2.2/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,14 +293,30 @@
     def get_sale(self, party=None):
         sale = super().get_sale(party=party)
         if self.sale_price_list:
             sale.price_list = self.sale_price_list
         return sale
 
 
+class Shop_TaxRuleCountry(metaclass=PoolMeta):
+    __name__ = 'web.shop'
+
+    def get_products(self, pattern=None):
+        pattern = pattern.copy() if pattern is not None else {}
+        if (self.warehouse
+                and self.warehouse.address
+                and self.warehouse.address.country):
+            pattern.setdefault(
+                'from_country', self.warehouse.address.country.id)
+        else:
+            pattern.setdefault('from_country')
+        pattern.setdefault('to_country')
+        return super().get_products(pattern=pattern)
+
+
 class Shop_Warehouse(ModelSQL):
     "Web Shop - Warehouse"
     __name__ = 'web.shop-stock.location'
 
     shop = fields.Many2One(
         'web.shop', "Shop", ondelete='CASCADE', required=True)
     warehouse = fields.Many2One(
```

### Comparing `trytond_web_shop-7.2.1/web.xml` & `trytond_web_shop-7.2.2/web.xml`

 * *Files identical despite different names*

