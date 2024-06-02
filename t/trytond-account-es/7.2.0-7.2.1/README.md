# Comparing `tmp/trytond_account_es-7.2.0.tar.gz` & `tmp/trytond_account_es-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_es-7.2.0.tar", last modified: Mon Apr 29 15:32:59 2024, max compression
+gzip compressed data, was "trytond_account_es-7.2.1.tar", last modified: Sun Jun  2 17:10:41 2024, max compression
```

## Comparing `trytond_account_es-7.2.0.tar` & `trytond_account_es-7.2.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.054458 trytond_account_es-7.2.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2258 2024-04-29 15:13:42.000000 trytond_account_es-7.2.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      703 2024-04-29 15:13:42.000000 trytond_account_es-7.2.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3106 2024-04-29 15:32:59.054458 trytond_account_es-7.2.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1343 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6178 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)   454723 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   417678 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/account_normal.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1356 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/account_payment.py
--rw-r--r--   0 ced       (1000) ced       (1000)      525 2023-04-15 07:12:14.000000 trytond_account_es-7.2.0/account_payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   311313 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/account_pyme.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1186 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/aeat111.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      390 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/aeat115.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     2697 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/aeat303.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1087 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/aeat347.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      698 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/aeat349.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      884 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1434 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/create_chart.xsl
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.047791 trytond_account_es-7.2.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      934 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:36:53.000000 trytond_account_es-7.2.0/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-04-15 07:12:14.000000 trytond_account_es-7.2.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.051124 trytond_account_es-7.2.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10593 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10727 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10656 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10242 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9321 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10537 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9119 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     9682 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10407 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    10148 2024-04-29 13:17:17.000000 trytond_account_es-7.2.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-27 16:43:20.000000 trytond_account_es-7.2.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      418 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1428 2024-02-04 18:51:26.000000 trytond_account_es-7.2.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)      454 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    36721 2024-01-27 09:58:52.000000 trytond_account_es-7.2.0/reporting_tax.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11942 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/reporting_tax.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:32:59.054458 trytond_account_es-7.2.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     3912 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)   151042 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/tax.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1501 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tax_groups.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   158875 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/tax_normal.xml
--rw-r--r--   0 ced       (1000) ced       (1000)   156637 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/tax_pyme.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.051124 trytond_account_es-7.2.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)     1347 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/tests/111.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      847 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/tests/115.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tests/303.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     3010 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tests/303_compensate.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1002 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/tests/347.txt
--rw-r--r--   0 ced       (1000) ced       (1000)     1002 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/tests/349.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4577 2024-04-22 12:14:36.000000 trytond_account_es-7.2.0/tests/scenario_ec_operation_list.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8647 2024-04-27 16:30:39.000000 trytond_account_es-7.2.0/tests/scenario_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4244 2024-04-22 12:14:36.000000 trytond_account_es-7.2.0/tests/scenario_reporting_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5300 2024-04-22 12:14:36.000000 trytond_account_es-7.2.0/tests/scenario_reporting_cancelled_invoices.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4394 2024-04-22 12:14:36.000000 trytond_account_es-7.2.0/tests/scenario_reporting_compensate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4616 2024-04-22 12:14:36.000000 trytond_account_es-7.2.0/tests/scenario_reporting_surcharge_tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2024-03-17 11:01:36.000000 trytond_account_es-7.2.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      284 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/tests/vat_book.csv
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:36:53.000000 trytond_account_es-7.2.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2024-04-29 15:13:37.000000 trytond_account_es-7.2.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.054458 trytond_account_es-7.2.0/trytond_account_es.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3106 2024-04-29 15:32:58.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3430 2024-04-29 15:32:59.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:32:58.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-04-29 15:32:58.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:55.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2024-04-29 15:32:58.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:32:58.000000 trytond_account_es-7.2.0/trytond_account_es.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:32:59.054458 trytond_account_es-7.2.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/es_ec_operation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/es_ec_operation_list_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      423 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/payment_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-01-16 14:00:20.000000 trytond_account_es-7.2.0/view/print_aeat_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/tax_code_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      377 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/tax_code_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      791 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/tax_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      506 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/vat_book_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      531 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/vat_book_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/vat_list_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      585 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view/vat_list_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1276 2023-04-15 07:12:15.000000 trytond_account_es-7.2.0/view.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:10:41.884218 trytond_account_es-7.2.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2359 2024-06-02 17:10:38.000000 trytond_account_es-7.2.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      703 2024-06-02 17:10:38.000000 trytond_account_es-7.2.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3106 2024-06-02 17:10:41.884218 trytond_account_es-7.2.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      934 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1343 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6178 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   454723 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   417678 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/account_normal.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1356 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/account_payment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      525 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/account_payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   311313 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/account_pyme.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1186 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/aeat111.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      390 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/aeat115.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     2697 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/aeat303.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1087 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/aeat347.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      698 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/aeat349.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      884 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1434 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/create_chart.xsl
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:10:41.877551 trytond_account_es-7.2.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      934 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:10:41.877551 trytond_account_es-7.2.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10593 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10727 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10656 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10242 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9321 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10537 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9119 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     9682 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10407 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    10148 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     8807 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      418 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1428 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      454 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    36719 2024-05-26 17:46:37.000000 trytond_account_es-7.2.1/reporting_tax.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11942 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/reporting_tax.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 17:10:41.884218 trytond_account_es-7.2.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     3912 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   151042 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tax.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1501 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tax_groups.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   158875 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tax_normal.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)   156637 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tax_pyme.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:10:41.880885 trytond_account_es-7.2.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1347 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/111.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      847 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/115.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     3010 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/303.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     3010 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/303_compensate.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1002 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/347.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1002 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/349.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4577 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/scenario_ec_operation_list.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8647 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/scenario_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4244 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/scenario_reporting_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5300 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/scenario_reporting_cancelled_invoices.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4394 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/scenario_reporting_compensate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4616 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/scenario_reporting_surcharge_tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      284 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tests/vat_book.csv
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2024-04-30 17:21:06.000000 trytond_account_es-7.2.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:10:41.880885 trytond_account_es-7.2.1/trytond_account_es.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3106 2024-06-02 17:10:41.000000 trytond_account_es-7.2.1/trytond_account_es.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3430 2024-06-02 17:10:41.000000 trytond_account_es-7.2.1/trytond_account_es.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 17:10:41.000000 trytond_account_es-7.2.1/trytond_account_es.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       58 2024-06-02 17:10:41.000000 trytond_account_es-7.2.1/trytond_account_es.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 14:11:50.000000 trytond_account_es-7.2.1/trytond_account_es.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2024-06-02 17:10:41.000000 trytond_account_es-7.2.1/trytond_account_es.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 17:10:41.000000 trytond_account_es-7.2.1/trytond_account_es.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:10:41.880885 trytond_account_es-7.2.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/es_ec_operation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/es_ec_operation_list_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      423 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/payment_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/print_aeat_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/tax_code_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      377 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/tax_code_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      791 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      791 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/tax_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      506 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/vat_book_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      531 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/vat_book_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/vat_list_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      585 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view/vat_list_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1276 2024-04-30 17:20:59.000000 trytond_account_es-7.2.1/view.xml
```

### Comparing `trytond_account_es-7.2.0/CHANGELOG` & `trytond_account_es-7.2.1/CHANGELOG`

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

### Comparing `trytond_account_es-7.2.0/COPYRIGHT` & `trytond_account_es-7.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/LICENSE` & `trytond_account_es-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/PKG-INFO` & `trytond_account_es-7.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_es
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton with Spanish chart of accounts
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_es-7.2.0/README.rst` & `trytond_account_es-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/__init__.py` & `trytond_account_es-7.2.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/account.py` & `trytond_account_es-7.2.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/account.xml` & `trytond_account_es-7.2.1/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/account_normal.xml` & `trytond_account_es-7.2.1/account_normal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/account_payment.py` & `trytond_account_es-7.2.1/account_payment.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/account_payment.xml` & `trytond_account_es-7.2.1/account_payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/account_pyme.xml` & `trytond_account_es-7.2.1/account_pyme.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/aeat111.txt` & `trytond_account_es-7.2.1/aeat111.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/aeat303.txt` & `trytond_account_es-7.2.1/aeat303.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/aeat347.txt` & `trytond_account_es-7.2.1/aeat347.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/aeat349.txt` & `trytond_account_es-7.2.1/aeat349.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/company.py` & `trytond_account_es-7.2.1/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/create_chart.xsl` & `trytond_account_es-7.2.1/create_chart.xsl`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/doc/conf.py` & `trytond_account_es-7.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/doc/index.rst` & `trytond_account_es-7.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/bg.po` & `trytond_account_es-7.2.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/ca.po` & `trytond_account_es-7.2.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/cs.po` & `trytond_account_es-7.2.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/de.po` & `trytond_account_es-7.2.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/es.po` & `trytond_account_es-7.2.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/es_419.po` & `trytond_account_es-7.2.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/et.po` & `trytond_account_es-7.2.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/fa.po` & `trytond_account_es-7.2.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/fi.po` & `trytond_account_es-7.2.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/fr.po` & `trytond_account_es-7.2.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/hu.po` & `trytond_account_es-7.2.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/id.po` & `trytond_account_es-7.2.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/it.po` & `trytond_account_es-7.2.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/lo.po` & `trytond_account_es-7.2.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/lt.po` & `trytond_account_es-7.2.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/nl.po` & `trytond_account_es-7.2.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/pl.po` & `trytond_account_es-7.2.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/pt.po` & `trytond_account_es-7.2.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/ro.po` & `trytond_account_es-7.2.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/ru.po` & `trytond_account_es-7.2.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/sl.po` & `trytond_account_es-7.2.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/tr.po` & `trytond_account_es-7.2.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/uk.po` & `trytond_account_es-7.2.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/locale/zh_CN.po` & `trytond_account_es-7.2.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/party.py` & `trytond_account_es-7.2.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/reporting_tax.py` & `trytond_account_es-7.2.1/reporting_tax.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,15 @@
                 amount_to_compensate += account.balance
 
         for code in ['46', '64', '66', '67', '69', '71', '88']:
             assert code not in amounts, (
                 "computed code %s already defined" % code)
         amounts['46'] = amounts['27'] - amounts['45']
         amounts['64'] = amounts['46'] + amounts['58'] + amounts['76']
-        amounts['66'] = amounts['64'] * Decimal(amounts['65']) / Decimal(100.0)
+        amounts['66'] = amounts['64'] * Decimal(amounts['65']) / Decimal(100)
         amounts['110'] = amounts['78'] = amount_to_compensate
         amounts['87'] = amounts['110'] - amounts['78']
         amounts['69'] = (amounts['66'] + amounts['77'] - amounts['78']
             + amounts['68'])
         amounts['71'] = (amounts['69'] - amounts['70'])
         amounts['88'] = (amounts['80'] + amounts['81'] - amounts['93']
             + amounts['94'] + amounts['83'] + amounts['84'] + amounts['85']
```

### Comparing `trytond_account_es-7.2.0/reporting_tax.xml` & `trytond_account_es-7.2.1/reporting_tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/setup.py` & `trytond_account_es-7.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tax.xml` & `trytond_account_es-7.2.1/tax.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tax_groups.xml` & `trytond_account_es-7.2.1/tax_groups.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tax_normal.xml` & `trytond_account_es-7.2.1/tax_normal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tax_pyme.xml` & `trytond_account_es-7.2.1/tax_pyme.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/111.txt` & `trytond_account_es-7.2.1/tests/111.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/115.txt` & `trytond_account_es-7.2.1/tests/115.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/303.txt` & `trytond_account_es-7.2.1/tests/303.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/303_compensate.txt` & `trytond_account_es-7.2.1/tests/303_compensate.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/347.txt` & `trytond_account_es-7.2.1/tests/347.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/349.txt` & `trytond_account_es-7.2.1/tests/349.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/scenario_ec_operation_list.rst` & `trytond_account_es-7.2.1/tests/scenario_ec_operation_list.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/scenario_reporting.rst` & `trytond_account_es-7.2.1/tests/scenario_reporting.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/scenario_reporting_alternate_currency.rst` & `trytond_account_es-7.2.1/tests/scenario_reporting_alternate_currency.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/scenario_reporting_cancelled_invoices.rst` & `trytond_account_es-7.2.1/tests/scenario_reporting_cancelled_invoices.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/scenario_reporting_compensate.rst` & `trytond_account_es-7.2.1/tests/scenario_reporting_compensate.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tests/scenario_reporting_surcharge_tax.rst` & `trytond_account_es-7.2.1/tests/scenario_reporting_surcharge_tax.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/tox.ini` & `trytond_account_es-7.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/trytond_account_es.egg-info/PKG-INFO` & `trytond_account_es-7.2.1/trytond_account_es.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_es
-Version: 7.2.0
+Version: 7.2.1
 Summary: Tryton with Spanish chart of accounts
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_es-7.2.0/trytond_account_es.egg-info/SOURCES.txt` & `trytond_account_es-7.2.1/trytond_account_es.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/view/tax_form.xml` & `trytond_account_es-7.2.1/view/tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/view/tax_template_form.xml` & `trytond_account_es-7.2.1/view/tax_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/view/vat_book_list.xml` & `trytond_account_es-7.2.1/view/vat_book_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/view/vat_list_list.xml` & `trytond_account_es-7.2.1/view/vat_list_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_es-7.2.0/view.xml` & `trytond_account_es-7.2.1/view.xml`

 * *Files identical despite different names*

