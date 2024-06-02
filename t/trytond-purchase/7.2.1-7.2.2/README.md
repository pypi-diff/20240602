# Comparing `tmp/trytond_purchase-7.2.1.tar.gz` & `tmp/trytond_purchase-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_purchase-7.2.1.tar", last modified: Wed May  1 11:38:28 2024, max compression
+gzip compressed data, was "trytond_purchase-7.2.2.tar", last modified: Sun Jun  2 16:22:00 2024, max compression
```

## Comparing `trytond_purchase-7.2.1.tar` & `trytond_purchase-7.2.2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.529713 trytond_purchase-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     7241 2024-05-01 11:38:25.000000 trytond_purchase-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 11:38:25.000000 trytond_purchase-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-05-01 11:38:28.529713 trytond_purchase-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1909 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3581 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2508 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.519714 trytond_purchase-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7482 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.519714 trytond_purchase-7.2.1/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2000 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/usage/prepurchase.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5036 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/usage/process.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2027 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/doc/usage/returns.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.523047 trytond_purchase-7.2.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      471 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/icons/tryton-purchase.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5999 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1715 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.523047 trytond_purchase-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    37931 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38111 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33102 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38601 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38303 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32642 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34815 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40065 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33089 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38471 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37153 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33743 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36400 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37935 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35906 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38479 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34444 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36141 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38529 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38486 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37835 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33080 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31383 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36567 2024-04-30 17:21:59.000000 trytond_purchase-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4336 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3698 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1146 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    20794 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    77247 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/purchase.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    87914 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/purchase.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31720 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/purchase.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    11639 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/purchase_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23812 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/purchase_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:38:28.529713 trytond_purchase-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4577 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8934 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4754 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.526380 trytond_purchase-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19177 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1678 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_copy_product_suppliers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1581 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_default_taxes.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1285 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2794 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_line_cancelled.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2509 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_line_cancelled_on_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2448 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_manual_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3040 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5169 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3003 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/scenario_purchase_return_wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5595 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-04-30 17:21:06.000000 trytond_purchase-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.529713 trytond_purchase-7.2.1/trytond_purchase.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     5171 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:38:28.000000 trytond_purchase-7.2.1/trytond_purchase.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:38:28.529713 trytond_purchase-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      482 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/move_list_shipment_in.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      444 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_list_purchase_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_price_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_price_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_price_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/product_supplier_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3651 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1860 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      918 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      589 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      544 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_time_series_graph_expense.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_reporting_supplier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      656 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/purchase_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/return_purchase_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2024-04-30 17:21:00.000000 trytond_purchase-7.2.1/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:22:00.523957 trytond_purchase-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     7342 2024-06-02 16:21:57.000000 trytond_purchase-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-06-02 16:21:56.000000 trytond_purchase-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-06-02 16:22:00.523957 trytond_purchase-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1909 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3581 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2508 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:22:00.517290 trytond_purchase-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7482 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:22:00.517290 trytond_purchase-7.2.2/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      232 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2000 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/doc/usage/prepurchase.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5036 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2027 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/doc/usage/returns.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:22:00.517290 trytond_purchase-7.2.2/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      471 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/icons/tryton-purchase.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5999 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1715 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:22:00.520624 trytond_purchase-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    37931 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38111 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33102 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38601 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38303 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32642 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34815 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40065 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33089 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38471 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37153 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33743 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36400 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37935 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35906 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38479 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34444 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36141 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38529 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38486 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37835 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33080 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31383 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36567 2024-04-30 17:21:59.000000 trytond_purchase-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4336 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3698 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1146 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    20794 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    77247 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/purchase.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    87894 2024-05-26 17:46:37.000000 trytond_purchase-7.2.2/purchase.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31720 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/purchase.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    11639 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/purchase_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23812 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/purchase_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 16:22:00.523957 trytond_purchase-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4577 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8934 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4754 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:22:00.520624 trytond_purchase-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19177 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/scenario_purchase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1678 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/scenario_purchase_copy_product_suppliers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1581 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/scenario_purchase_default_taxes.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1285 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/scenario_purchase_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2794 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/scenario_purchase_line_cancelled.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2509 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/scenario_purchase_line_cancelled_on_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2448 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/scenario_purchase_manual_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3040 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/scenario_purchase_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5169 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/scenario_purchase_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3003 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/scenario_purchase_return_wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5595 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      329 2024-05-01 11:38:38.000000 trytond_purchase-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:22:00.523957 trytond_purchase-7.2.2/trytond_purchase.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-06-02 16:22:00.000000 trytond_purchase-7.2.2/trytond_purchase.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     5171 2024-06-02 16:22:00.000000 trytond_purchase-7.2.2/trytond_purchase.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 16:22:00.000000 trytond_purchase-7.2.2/trytond_purchase.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-06-02 16:22:00.000000 trytond_purchase-7.2.2/trytond_purchase.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:38:28.000000 trytond_purchase-7.2.2/trytond_purchase.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-06-02 16:22:00.000000 trytond_purchase-7.2.2/trytond_purchase.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 16:22:00.000000 trytond_purchase-7.2.2/trytond_purchase.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:22:00.523957 trytond_purchase-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      435 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      369 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      482 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/move_list_shipment_in.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      879 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      444 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/product_list_purchase_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1049 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/product_supplier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      453 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/product_supplier_price_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/product_supplier_price_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/product_supplier_price_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/product_supplier_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/product_supplier_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3651 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1860 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      918 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      589 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      544 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_reporting_main_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_reporting_main_time_series_graph_expense.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_reporting_supplier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      656 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/purchase_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/return_purchase_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1032 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2024-04-30 17:21:00.000000 trytond_purchase-7.2.2/view/template_tree.xml
```

### Comparing `trytond_purchase-7.2.1/CHANGELOG` & `trytond_purchase-7.2.2/CHANGELOG`

 * *Files 0% similar despite different names*

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

### Comparing `trytond_purchase-7.2.1/COPYRIGHT` & `trytond_purchase-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/LICENSE` & `trytond_purchase-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/PKG-INFO` & `trytond_purchase-7.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase-7.2.1/__init__.py` & `trytond_purchase-7.2.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/configuration.py` & `trytond_purchase-7.2.2/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/configuration.xml` & `trytond_purchase-7.2.2/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/doc/conf.py` & `trytond_purchase-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/doc/design.rst` & `trytond_purchase-7.2.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/doc/usage/prepurchase.inc.rst` & `trytond_purchase-7.2.2/doc/usage/prepurchase.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/doc/usage/process.inc.rst` & `trytond_purchase-7.2.2/doc/usage/process.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/doc/usage/returns.inc.rst` & `trytond_purchase-7.2.2/doc/usage/returns.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/icons/LICENSE` & `trytond_purchase-7.2.2/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/invoice.py` & `trytond_purchase-7.2.2/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/invoice.xml` & `trytond_purchase-7.2.2/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/bg.po` & `trytond_purchase-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/ca.po` & `trytond_purchase-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/cs.po` & `trytond_purchase-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/de.po` & `trytond_purchase-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/es.po` & `trytond_purchase-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/es_419.po` & `trytond_purchase-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/et.po` & `trytond_purchase-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/fa.po` & `trytond_purchase-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/fi.po` & `trytond_purchase-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/fr.po` & `trytond_purchase-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/hu.po` & `trytond_purchase-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/id.po` & `trytond_purchase-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/it.po` & `trytond_purchase-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/lo.po` & `trytond_purchase-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/lt.po` & `trytond_purchase-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/nl.po` & `trytond_purchase-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/pl.po` & `trytond_purchase-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/pt.po` & `trytond_purchase-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/ro.po` & `trytond_purchase-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/ru.po` & `trytond_purchase-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/sl.po` & `trytond_purchase-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/tr.po` & `trytond_purchase-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/uk.po` & `trytond_purchase-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/locale/zh_CN.po` & `trytond_purchase-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/message.xml` & `trytond_purchase-7.2.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/party.py` & `trytond_purchase-7.2.2/party.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/party.xml` & `trytond_purchase-7.2.2/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/product.py` & `trytond_purchase-7.2.2/product.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/product.xml` & `trytond_purchase-7.2.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/purchase.fodt` & `trytond_purchase-7.2.2/purchase.fodt`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/purchase.py` & `trytond_purchase-7.2.2/purchase.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,17 +476,17 @@
             context['language'] = self.party.lang.code
         if self.company:
             context['company'] = self.company.id
         return context
 
     @fields.depends('lines', 'currency', methods=['get_tax_amount'])
     def on_change_lines(self):
-        self.untaxed_amount = Decimal('0.0')
-        self.tax_amount = Decimal('0.0')
-        self.total_amount = Decimal('0.0')
+        self.untaxed_amount = Decimal(0)
+        self.tax_amount = Decimal(0)
+        self.total_amount = Decimal(0)
         if self.lines:
             for line in self.lines:
                 self.untaxed_amount += getattr(line, 'amount', None) or 0
             self.tax_amount = self.get_tax_amount()
         if self.currency:
             self.untaxed_amount = self.currency.round(self.untaxed_amount)
             self.tax_amount = self.currency.round(self.tax_amount)
@@ -1620,23 +1620,23 @@
                 return currency.round(amount)
             return amount
 
     def get_amount(self, name):
         if self.type == 'line':
             return self.on_change_with_amount()
         elif self.type == 'subtotal':
-            amount = Decimal('0.0')
+            amount = Decimal(0)
             for line2 in self.purchase.lines:
                 if line2.type == 'line':
                     amount += line2.purchase.currency.round(
                         Decimal(str(line2.quantity)) * line2.unit_price)
                 elif line2.type == 'subtotal':
                     if self == line2:
                         break
-                    amount = Decimal('0.0')
+                    amount = Decimal(0)
             return amount
 
     @fields.depends('purchase', '_parent_purchase.warehouse')
     def on_change_with_warehouse(self, name=None):
         return self.purchase.warehouse if self.purchase else None
 
     def get_from_location(self, name):
```

### Comparing `trytond_purchase-7.2.1/purchase.xml` & `trytond_purchase-7.2.2/purchase.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/purchase_reporting.py` & `trytond_purchase-7.2.2/purchase_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/purchase_reporting.xml` & `trytond_purchase-7.2.2/purchase_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/setup.py` & `trytond_purchase-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/stock.py` & `trytond_purchase-7.2.2/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/stock.xml` & `trytond_purchase-7.2.2/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tests/scenario_purchase.rst` & `trytond_purchase-7.2.2/tests/scenario_purchase.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tests/scenario_purchase_copy_product_suppliers.rst` & `trytond_purchase-7.2.2/tests/scenario_purchase_copy_product_suppliers.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tests/scenario_purchase_default_taxes.rst` & `trytond_purchase-7.2.2/tests/scenario_purchase_default_taxes.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tests/scenario_purchase_empty.rst` & `trytond_purchase-7.2.2/tests/scenario_purchase_empty.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tests/scenario_purchase_line_cancelled.rst` & `trytond_purchase-7.2.2/tests/scenario_purchase_line_cancelled.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tests/scenario_purchase_line_cancelled_on_shipment.rst` & `trytond_purchase-7.2.2/tests/scenario_purchase_line_cancelled_on_shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tests/scenario_purchase_manual_invoice.rst` & `trytond_purchase-7.2.2/tests/scenario_purchase_manual_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tests/scenario_purchase_modify_header.rst` & `trytond_purchase-7.2.2/tests/scenario_purchase_modify_header.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tests/scenario_purchase_reporting.rst` & `trytond_purchase-7.2.2/tests/scenario_purchase_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tests/scenario_purchase_return_wizard.rst` & `trytond_purchase-7.2.2/tests/scenario_purchase_return_wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tests/test_module.py` & `trytond_purchase-7.2.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/tox.ini` & `trytond_purchase-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/trytond_purchase.egg-info/PKG-INFO` & `trytond_purchase-7.2.2/trytond_purchase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_purchase
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for purchase
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_purchase-7.2.1/trytond_purchase.egg-info/SOURCES.txt` & `trytond_purchase-7.2.2/trytond_purchase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/view/party_form.xml` & `trytond_purchase-7.2.2/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/view/product_supplier_form.xml` & `trytond_purchase-7.2.2/view/product_supplier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/view/purchase_form.xml` & `trytond_purchase-7.2.2/view/purchase_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/view/purchase_line_form.xml` & `trytond_purchase-7.2.2/view/purchase_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/view/purchase_line_tree.xml` & `trytond_purchase-7.2.2/view/purchase_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/view/purchase_line_tree_sequence.xml` & `trytond_purchase-7.2.2/view/purchase_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/view/purchase_reporting_context_form.xml` & `trytond_purchase-7.2.2/view/purchase_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/view/purchase_tree.xml` & `trytond_purchase-7.2.2/view/purchase_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_purchase-7.2.1/view/template_form.xml` & `trytond_purchase-7.2.2/view/template_form.xml`

 * *Files identical despite different names*

