# Comparing `tmp/trytond_sale-7.2.1.tar.gz` & `tmp/trytond_sale-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_sale-7.2.1.tar", last modified: Wed May  1 11:28:15 2024, max compression
+gzip compressed data, was "trytond_sale-7.2.2.tar", last modified: Sun Jun  2 16:05:29 2024, max compression
```

## Comparing `trytond_sale-7.2.1.tar` & `trytond_sale-7.2.2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.555745 trytond_sale-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     6785 2024-05-01 11:28:12.000000 trytond_sale-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 11:28:12.000000 trytond_sale-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-05-01 11:28:15.555745 trytond_sale-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2345 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3898 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2379 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/configuration.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.545745 trytond_sale-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3067 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9121 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      437 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.549079 trytond_sale-7.2.1/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      268 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1985 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/usage/presales.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4187 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/usage/process.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      726 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/usage/reporting.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1618 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/doc/usage/returns.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      503 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.549079 trytond_sale-7.2.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/icons/tryton-sale.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     5255 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1754 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.549079 trytond_sale-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    41783 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42532 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36808 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43272 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42730 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35108 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40072 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    44826 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36769 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    43139 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41105 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37993 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39376 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40834 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41176 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42618 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38275 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39584 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    42692 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41861 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39277 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36760 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34519 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37068 2024-04-30 17:21:59.000000 trytond_sale-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4617 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4595 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2980 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9027 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2740 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    76278 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/sale.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    89113 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25512 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    36794 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/sale_reporting.py
--rw-r--r--   0 ced       (1000) ced       (1000)    55353 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/sale_reporting.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 11:28:15.555745 trytond_sale-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4556 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7637 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2944 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.552412 trytond_sale-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20145 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      898 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_default_methods.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1517 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_default_taxes.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1197 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_empty.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2700 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_line_cancelled.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2414 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_line_cancelled_on_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2423 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_line_cancelled_on_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2344 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_manual_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1935 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_manual_shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_modify_header.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    12959 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/scenario_sale_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2524 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-30 17:21:06.000000 trytond_sale-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.555745 trytond_sale-7.2.1/trytond_sale.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     5488 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       46 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 11:28:15.000000 trytond_sale-7.2.1/trytond_sale.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 11:28:15.555745 trytond_sale-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/handle_invoice_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/handle_shipment_exception_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/modify_header_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      844 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/product_configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/product_list_sale_line.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      688 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/product_sale_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/return_sale_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3954 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1596 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      845 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      529 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_country_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_customer_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_customer_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_customer_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_customer_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_customer_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      281 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_time_series_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_time_series_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_product_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_product_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_product_graph_number.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_product_graph_revenue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_reporting_region_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      652 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/sale_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      935 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:21:00.000000 trytond_sale-7.2.1/view/template_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:05:29.259883 trytond_sale-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6886 2024-06-02 16:05:25.000000 trytond_sale-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-06-02 16:05:25.000000 trytond_sale-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-06-02 16:05:29.259883 trytond_sale-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2345 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3898 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2379 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/configuration.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:05:29.246550 trytond_sale-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3067 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9121 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      437 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:05:29.249883 trytond_sale-7.2.2/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      268 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1985 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/doc/usage/presales.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4187 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      726 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/doc/usage/reporting.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1618 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/doc/usage/returns.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      503 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:05:29.249883 trytond_sale-7.2.2/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      224 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/icons/tryton-sale.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     5255 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1754 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:05:29.253216 trytond_sale-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    41783 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42532 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36808 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43272 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42730 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35108 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40072 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    44826 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36769 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    43139 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41105 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37993 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39376 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40834 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41176 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42618 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38275 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39584 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    42692 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41861 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39277 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36760 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34519 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37068 2024-04-30 17:21:59.000000 trytond_sale-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4617 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4595 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2980 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9044 2024-05-26 17:39:36.000000 trytond_sale-7.2.2/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2740 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    76278 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/sale.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    89077 2024-05-26 17:46:37.000000 trytond_sale-7.2.2/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25512 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    36794 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/sale_reporting.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    55353 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/sale_reporting.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 16:05:29.259883 trytond_sale-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4556 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7637 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2944 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:05:29.253216 trytond_sale-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20145 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/scenario_sale.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      898 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/scenario_sale_default_methods.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1517 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/scenario_sale_default_taxes.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1197 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/scenario_sale_empty.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2700 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/scenario_sale_line_cancelled.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2414 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/scenario_sale_line_cancelled_on_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2423 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/scenario_sale_line_cancelled_on_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2344 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/scenario_sale_manual_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1935 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/scenario_sale_manual_shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3004 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/scenario_sale_modify_header.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    12959 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/scenario_sale_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2524 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-05-01 11:28:24.000000 trytond_sale-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:05:29.259883 trytond_sale-7.2.2/trytond_sale.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3332 2024-06-02 16:05:28.000000 trytond_sale-7.2.2/trytond_sale.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     5488 2024-06-02 16:05:29.000000 trytond_sale-7.2.2/trytond_sale.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 16:05:28.000000 trytond_sale-7.2.2/trytond_sale.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       46 2024-06-02 16:05:28.000000 trytond_sale-7.2.2/trytond_sale.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 11:28:15.000000 trytond_sale-7.2.2/trytond_sale.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2024-06-02 16:05:28.000000 trytond_sale-7.2.2/trytond_sale.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 16:05:28.000000 trytond_sale-7.2.2/trytond_sale.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:05:29.259883 trytond_sale-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/handle_invoice_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      428 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/handle_shipment_exception_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/modify_header_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      478 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      844 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      326 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/product_configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/product_list_sale_line.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      688 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/product_sale_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/return_sale_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3954 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1596 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      845 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      529 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      341 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_country_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_customer_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_customer_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_customer_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_customer_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_customer_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_main_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      281 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_main_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      319 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_main_time_series_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_main_time_series_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_product_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_product_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_product_graph_number.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_product_graph_revenue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      303 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_reporting_region_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      652 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/sale_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      935 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2024-04-30 17:21:00.000000 trytond_sale-7.2.2/view/template_tree.xml
```

### Comparing `trytond_sale-7.2.1/CHANGELOG` & `trytond_sale-7.2.2/CHANGELOG`

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

### Comparing `trytond_sale-7.2.1/COPYRIGHT` & `trytond_sale-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/LICENSE` & `trytond_sale-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/PKG-INFO` & `trytond_sale-7.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale-7.2.1/__init__.py` & `trytond_sale-7.2.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/configuration.py` & `trytond_sale-7.2.2/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/configuration.xml` & `trytond_sale-7.2.2/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/doc/conf.py` & `trytond_sale-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/doc/design.rst` & `trytond_sale-7.2.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/doc/usage/presales.inc.rst` & `trytond_sale-7.2.2/doc/usage/presales.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/doc/usage/process.inc.rst` & `trytond_sale-7.2.2/doc/usage/process.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/doc/usage/reporting.inc.rst` & `trytond_sale-7.2.2/doc/usage/reporting.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/doc/usage/returns.inc.rst` & `trytond_sale-7.2.2/doc/usage/returns.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/icons/LICENSE` & `trytond_sale-7.2.2/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/invoice.py` & `trytond_sale-7.2.2/invoice.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/invoice.xml` & `trytond_sale-7.2.2/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/bg.po` & `trytond_sale-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/ca.po` & `trytond_sale-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/cs.po` & `trytond_sale-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/de.po` & `trytond_sale-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/es.po` & `trytond_sale-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/es_419.po` & `trytond_sale-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/et.po` & `trytond_sale-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/fa.po` & `trytond_sale-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/fi.po` & `trytond_sale-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/fr.po` & `trytond_sale-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/hu.po` & `trytond_sale-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/id.po` & `trytond_sale-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/it.po` & `trytond_sale-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/lo.po` & `trytond_sale-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/lt.po` & `trytond_sale-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/nl.po` & `trytond_sale-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/pl.po` & `trytond_sale-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/pt.po` & `trytond_sale-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/ro.po` & `trytond_sale-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/ru.po` & `trytond_sale-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/sl.po` & `trytond_sale-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/tr.po` & `trytond_sale-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/uk.po` & `trytond_sale-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/locale/zh_CN.po` & `trytond_sale-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/message.xml` & `trytond_sale-7.2.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/party.py` & `trytond_sale-7.2.2/party.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/party.xml` & `trytond_sale-7.2.2/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/product.py` & `trytond_sale-7.2.2/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 
         for product in products:
             unit_price = product._get_sale_unit_price(quantity=quantity)
             if unit_price is not None:
                 if uom and product.default_uom.category == uom.category:
                     unit_price = Uom.compute_price(
                         product.default_uom, unit_price, uom)
-                else:
+                elif product.sale_uom:
                     unit_price = Uom.compute_price(
                         product.default_uom, unit_price, product.sale_uom)
             if currency and company and unit_price is not None:
                 if company.currency != currency:
                     with Transaction().set_context(date=date):
                         unit_price = Currency.compute(
                             company.currency, unit_price,
```

### Comparing `trytond_sale-7.2.1/product.xml` & `trytond_sale-7.2.2/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/sale.fodt` & `trytond_sale-7.2.2/sale.fodt`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/sale.py` & `trytond_sale-7.2.2/sale.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,17 +539,17 @@
         Config = Pool().get('ir.configuration')
         if self.party and self.party.lang:
             return self.party.lang.code
         return Config.get_language()
 
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
@@ -1676,36 +1676,36 @@
 
     @fields.depends(
         'type', 'quantity', 'unit_price',
         'sale', '_parent_sale.currency')
     def on_change_with_amount(self):
         if self.type == 'line':
             currency = self.sale.currency if self.sale else None
-            amount = Decimal(str(self.quantity or '0.0')) * \
-                (self.unit_price or Decimal('0.0'))
+            amount = Decimal(str(self.quantity or 0)) * \
+                (self.unit_price or Decimal(0))
             if currency:
                 return currency.round(amount)
             return amount
-        return Decimal('0.0')
+        return Decimal(0)
 
     def get_amount(self, name):
         if self.type == 'line':
             return self.on_change_with_amount()
         elif self.type == 'subtotal':
-            amount = Decimal('0.0')
+            amount = Decimal(0)
             for line2 in self.sale.lines:
                 if line2.type == 'line':
                     amount += line2.sale.currency.round(
                         Decimal(str(line2.quantity)) * line2.unit_price)
                 elif line2.type == 'subtotal':
                     if self == line2:
                         break
-                    amount = Decimal('0.0')
+                    amount = Decimal(0)
             return amount
-        return Decimal('0.0')
+        return Decimal(0)
 
     @fields.depends('sale', '_parent_sale.warehouse')
     def on_change_with_warehouse(self, name=None):
         return self.sale.warehouse if self.sale else None
 
     def get_from_location(self, name):
         if (self.quantity or 0) >= 0:
```

### Comparing `trytond_sale-7.2.1/sale.xml` & `trytond_sale-7.2.2/sale.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/sale_reporting.py` & `trytond_sale-7.2.2/sale_reporting.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/sale_reporting.xml` & `trytond_sale-7.2.2/sale_reporting.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/setup.py` & `trytond_sale-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/stock.py` & `trytond_sale-7.2.2/stock.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/stock.xml` & `trytond_sale-7.2.2/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/scenario_sale.rst` & `trytond_sale-7.2.2/tests/scenario_sale.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/scenario_sale_default_methods.rst` & `trytond_sale-7.2.2/tests/scenario_sale_default_methods.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/scenario_sale_default_taxes.rst` & `trytond_sale-7.2.2/tests/scenario_sale_default_taxes.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/scenario_sale_empty.rst` & `trytond_sale-7.2.2/tests/scenario_sale_empty.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/scenario_sale_line_cancelled.rst` & `trytond_sale-7.2.2/tests/scenario_sale_line_cancelled.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/scenario_sale_line_cancelled_on_invoice.rst` & `trytond_sale-7.2.2/tests/scenario_sale_line_cancelled_on_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/scenario_sale_line_cancelled_on_shipment.rst` & `trytond_sale-7.2.2/tests/scenario_sale_line_cancelled_on_shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/scenario_sale_manual_invoice.rst` & `trytond_sale-7.2.2/tests/scenario_sale_manual_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/scenario_sale_manual_shipment.rst` & `trytond_sale-7.2.2/tests/scenario_sale_manual_shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/scenario_sale_modify_header.rst` & `trytond_sale-7.2.2/tests/scenario_sale_modify_header.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/scenario_sale_reporting.rst` & `trytond_sale-7.2.2/tests/scenario_sale_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tests/test_module.py` & `trytond_sale-7.2.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/tox.ini` & `trytond_sale-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/trytond_sale.egg-info/PKG-INFO` & `trytond_sale-7.2.2/trytond_sale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_sale
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for sale
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_sale-7.2.1/trytond_sale.egg-info/SOURCES.txt` & `trytond_sale-7.2.2/trytond_sale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/configuration_form.xml` & `trytond_sale-7.2.2/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/party_form.xml` & `trytond_sale-7.2.2/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/product_list_sale_line.xml` & `trytond_sale-7.2.2/view/product_list_sale_line.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/product_sale_context_form.xml` & `trytond_sale-7.2.2/view/product_sale_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/sale_form.xml` & `trytond_sale-7.2.2/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/sale_line_form.xml` & `trytond_sale-7.2.2/view/sale_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/sale_line_tree.xml` & `trytond_sale-7.2.2/view/sale_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/sale_line_tree_sequence.xml` & `trytond_sale-7.2.2/view/sale_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/sale_reporting_context_form.xml` & `trytond_sale-7.2.2/view/sale_reporting_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/sale_reporting_customer_category_list.xml` & `trytond_sale-7.2.2/view/sale_reporting_customer_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/sale_reporting_product_category_list.xml` & `trytond_sale-7.2.2/view/sale_reporting_product_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/sale_tree.xml` & `trytond_sale-7.2.2/view/sale_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_sale-7.2.1/view/template_form.xml` & `trytond_sale-7.2.2/view/template_form.xml`

 * *Files identical despite different names*

