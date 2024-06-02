# Comparing `tmp/trytond_account_invoice-7.2.1.tar.gz` & `tmp/trytond_account_invoice-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice-7.2.1.tar", last modified: Wed May  1 12:21:41 2024, max compression
+gzip compressed data, was "trytond_account_invoice-7.2.2.tar", last modified: Sun Jun  2 17:02:33 2024, max compression
```

## Comparing `trytond_account_invoice-7.2.1.tar` & `trytond_account_invoice-7.2.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.912370 trytond_account_invoice-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     8236 2024-05-01 12:21:38.000000 trytond_account_invoice-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 12:21:38.000000 trytond_account_invoice-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-05-01 12:21:41.912370 trytond_account_invoice-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1977 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14844 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4877 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/company.py
--rw-r--r--   0 ced       (1000) ced       (1000)      466 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/company.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.902370 trytond_account_invoice-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      796 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7303 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.902370 trytond_account_invoice-7.2.1/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)     1920 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/usage/amend.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      210 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3446 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/usage/prepare.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3773 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/doc/usage/process.inc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      920 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.902370 trytond_account_invoice-7.2.1/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      356 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/icons/tryton-invoice.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    94000 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/invoice.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)   139705 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/invoice.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23815 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/invoice.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.905703 trytond_account_invoice-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    38545 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40107 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33376 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40811 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39814 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34299 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37631 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    41802 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33337 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40567 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35994 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35962 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36623 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39197 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37373 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39770 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    34002 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36946 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39091 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39208 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38359 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33319 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31901 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38369 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6873 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3324 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2389 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13402 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/payment_term.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5888 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/payment_term.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:21:41.912370 trytond_account_invoice-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.909037 trytond_account_invoice-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      229 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3122 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_cancelling_invoice_move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4010 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_credit_note.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    13167 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6057 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2881 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_exchange.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_lower_rate.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3488 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_rate_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_alternative_payee.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2666 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_customer_sequential.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_group_line.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1820 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_in_future.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2581 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_manual_tax.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3501 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_overpayment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2479 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_report_revision.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2989 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_reschedule_lines.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7240 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_supplier.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3373 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_supplier_post_paid.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3986 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_tax_deductible.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3349 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_invoice_with_credit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3632 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/scenario_renew_fiscalyear.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    11545 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1227 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-04-30 17:21:06.000000 trytond_account_invoice-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.912370 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     6312 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:21:41.912370 trytond_account_invoice-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/address_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      504 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/company_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      374 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/credit_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      511 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/fiscalyear_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4830 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      694 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_line_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      318 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_report_revision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_report_revision_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      842 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      442 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_sequence_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      462 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_sequence_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      744 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_tax_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_tax_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_tax_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/invoice_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/move_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/move_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/move_line_list_payment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/move_line_list_to_pay.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      738 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/pay_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/pay_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_method_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_method_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      629 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      871 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      370 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      776 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_relativedelta_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_relativedelta_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_line_relativedelta_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      491 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_test_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_test_result_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.1/view/payment_term_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:02:33.000337 trytond_account_invoice-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8337 2024-06-02 17:02:29.000000 trytond_account_invoice-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-06-02 17:02:29.000000 trytond_account_invoice-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-06-02 17:02:32.997004 trytond_account_invoice-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1977 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14844 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4877 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      720 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/company.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      466 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/company.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:02:32.987004 trytond_account_invoice-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3078 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      796 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7303 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:02:32.990338 trytond_account_invoice-7.2.2/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1920 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/doc/usage/amend.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      210 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3446 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/doc/usage/prepare.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3773 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/doc/usage/process.inc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      920 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:02:32.990338 trytond_account_invoice-7.2.2/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      356 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/icons/tryton-invoice.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    94000 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/invoice.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)   139692 2024-05-26 17:46:37.000000 trytond_account_invoice-7.2.2/invoice.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23815 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/invoice.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:02:32.993671 trytond_account_invoice-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    38545 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40107 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33376 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40811 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39814 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34299 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37631 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    41802 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33337 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40567 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35994 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35962 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36623 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39197 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37373 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39770 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    34002 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36946 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39091 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39208 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38359 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33319 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31901 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38369 2024-04-30 17:21:59.000000 trytond_account_invoice-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6873 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3324 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2389 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13374 2024-05-26 17:46:37.000000 trytond_account_invoice-7.2.2/payment_term.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5888 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/payment_term.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 17:02:33.000337 trytond_account_invoice-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:02:32.993671 trytond_account_invoice-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      229 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3122 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_cancelling_invoice_move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4010 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_credit_note.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    13167 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6057 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_alternate_currency.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2881 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_alternate_currency_exchange.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2853 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_alternate_currency_lower_rate.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3488 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_alternate_currency_rate_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3763 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_alternative_payee.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2666 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_customer_sequential.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_group_line.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1820 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_in_future.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2581 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_manual_tax.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3501 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_overpayment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2479 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_report_revision.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2989 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_reschedule_lines.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7240 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_supplier.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3373 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_supplier_post_paid.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3986 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_tax_deductible.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3349 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_invoice_with_credit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3632 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/scenario_renew_fiscalyear.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    11545 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1227 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      230 2024-05-01 12:21:51.000000 trytond_account_invoice-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:02:32.997004 trytond_account_invoice-7.2.2/trytond_account_invoice.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3036 2024-06-02 17:02:32.000000 trytond_account_invoice-7.2.2/trytond_account_invoice.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     6312 2024-06-02 17:02:32.000000 trytond_account_invoice-7.2.2/trytond_account_invoice.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 17:02:32.000000 trytond_account_invoice-7.2.2/trytond_account_invoice.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       68 2024-06-02 17:02:32.000000 trytond_account_invoice-7.2.2/trytond_account_invoice.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:21:41.000000 trytond_account_invoice-7.2.2/trytond_account_invoice.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2024-06-02 17:02:32.000000 trytond_account_invoice-7.2.2/trytond_account_invoice.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 17:02:32.000000 trytond_account_invoice-7.2.2/trytond_account_invoice.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:02:32.997004 trytond_account_invoice-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      321 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/address_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      504 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/company_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      374 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      619 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/credit_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      511 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/fiscalyear_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4830 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      694 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_line_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      318 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_report_revision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_report_revision_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      842 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      442 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_sequence_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      462 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_sequence_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      744 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_tax_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_tax_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      537 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_tax_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      886 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/invoice_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/move_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/move_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/move_line_list_payment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      382 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/move_line_list_to_pay.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      738 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/pay_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/pay_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      559 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_method_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_method_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      629 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_term_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      871 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_term_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      370 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_term_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_term_line_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      776 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_term_line_relativedelta_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_term_line_relativedelta_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_term_line_relativedelta_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      491 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_term_test_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_term_test_result_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2024-04-30 17:20:59.000000 trytond_account_invoice-7.2.2/view/payment_term_tree.xml
```

### Comparing `trytond_account_invoice-7.2.1/CHANGELOG` & `trytond_account_invoice-7.2.2/CHANGELOG`

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

### Comparing `trytond_account_invoice-7.2.1/COPYRIGHT` & `trytond_account_invoice-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/LICENSE` & `trytond_account_invoice-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/PKG-INFO` & `trytond_account_invoice-7.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice-7.2.1/__init__.py` & `trytond_account_invoice-7.2.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/account.py` & `trytond_account_invoice-7.2.2/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/account.xml` & `trytond_account_invoice-7.2.2/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/company.py` & `trytond_account_invoice-7.2.2/company.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/doc/conf.py` & `trytond_account_invoice-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/doc/configuration.rst` & `trytond_account_invoice-7.2.2/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/doc/design.rst` & `trytond_account_invoice-7.2.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/doc/usage/amend.inc.rst` & `trytond_account_invoice-7.2.2/doc/usage/amend.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/doc/usage/prepare.inc.rst` & `trytond_account_invoice-7.2.2/doc/usage/prepare.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/doc/usage/process.inc.rst` & `trytond_account_invoice-7.2.2/doc/usage/process.inc.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/exceptions.py` & `trytond_account_invoice-7.2.2/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/icons/LICENSE` & `trytond_account_invoice-7.2.2/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/invoice.fodt` & `trytond_account_invoice-7.2.2/invoice.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/invoice.py` & `trytond_account_invoice-7.2.2/invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # this repository contains the full copyright notices and license terms.
 import datetime as dt
 from collections import defaultdict, namedtuple
 from decimal import Decimal
 from itertools import chain, combinations, groupby
 
 from genshi.template.text import TextTemplate
-from sql import Literal, Null
+from sql import Null
 from sql.aggregate import Sum
 from sql.conditionals import Coalesce
 from sql.functions import CharLength, Round
 from sql.operators import Exists
 
 from trytond import backend
 from trytond.config import config
@@ -635,48 +635,48 @@
 
     @fields.depends(
         'lines', 'taxes', 'currency', methods=['_get_taxes', 'tax_date'])
     def _on_change_lines_taxes(self):
         pool = Pool()
         InvoiceTax = pool.get('account.invoice.tax')
 
-        self.untaxed_amount = Decimal('0.0')
-        self.tax_amount = Decimal('0.0')
-        self.total_amount = Decimal('0.0')
+        self.untaxed_amount = Decimal(0)
+        self.tax_amount = Decimal(0)
+        self.total_amount = Decimal(0)
         computed_taxes = {}
 
         if self.lines:
             for line in self.lines:
                 self.untaxed_amount += getattr(line, 'amount', None) or 0
             computed_taxes = self._get_taxes()
 
         def is_zero(amount):
             if self.currency:
                 return self.currency.is_zero(amount)
             else:
-                return amount == Decimal('0.0')
+                return amount == Decimal(0)
 
         tax_keys = []
         taxes = list(self.taxes or [])
         for tax in (self.taxes or []):
             if tax.manual:
-                self.tax_amount += tax.amount or Decimal('0.0')
+                self.tax_amount += tax.amount or Decimal(0)
                 continue
             key = tax._key
             if (key not in computed_taxes) or (key in tax_keys):
                 taxes.remove(tax)
                 continue
             tax_keys.append(key)
             if not is_zero(computed_taxes[key]['base']
-                    - (tax.base or Decimal('0.0'))):
+                    - (tax.base or Decimal(0))):
                 self.tax_amount += computed_taxes[key]['amount']
                 tax.amount = computed_taxes[key]['amount']
                 tax.base = computed_taxes[key]['base']
             else:
-                self.tax_amount += tax.amount or Decimal('0.0')
+                self.tax_amount += tax.amount or Decimal(0)
         for key in computed_taxes:
             if key not in tax_keys:
                 self.tax_amount += computed_taxes[key]['amount']
                 value = InvoiceTax.default_get(
                     list(InvoiceTax._fields.keys()), with_rec_name=False)
                 value.update(computed_taxes[key])
                 invoice_tax = InvoiceTax(**value)
@@ -892,15 +892,16 @@
                                 currency.digits)), 0).as_('total_amount'),
                 where=(line.invoice.in_(invoice_query)
                     & (invoice.total_amount_cache == Null)),
                 group_by=line.invoice)
             | tax.select(tax.invoice.as_('invoice'),
                 Coalesce(Sum(tax.amount), 0).as_('total_amount'),
                 where=(tax.invoice.in_(invoice_query)
-                    & ~Exists(invoice.select(Literal(1),
+                    & Exists(invoice.select(
+                            invoice.id,
                             where=(invoice.total_amount_cache == Null)
                             & (invoice.id == tax.invoice)))),
                 group_by=tax.invoice))
         union |= invoice.select(
             invoice.id.as_('invoice'),
             invoice.total_amount_cache.as_('total_amount'),
             where=(invoice.id.in_(invoice_query)
@@ -964,15 +965,16 @@
         Operator = fields.SQL_OPERATORS[operator]
         # SQLite uses float for sum
         if value is not None and backend.name == 'sqlite':
             value = float(value)
 
         query = tax.select(tax.invoice,
             where=(tax.invoice.in_(invoice_query)
-                & ~Exists(invoice.select(Literal(1),
+                & Exists(invoice.select(
+                        invoice.id,
                         where=(invoice.tax_amount_cache == Null)
                         & (invoice.id == tax.invoice)))),
             group_by=tax.invoice,
             having=Operator(Coalesce(Sum(tax.amount), 0).cast(type_name),
                 value))
         query |= invoice.select(invoice.id,
             where=invoice.id.in_(invoice_query)
@@ -2485,31 +2487,31 @@
         '_parent_invoice.currency', 'currency', 'taxes',
         '_parent_invoice.type', 'invoice_type',
         methods=['_get_taxes'])
     def on_change_with_amount(self):
         if self.type == 'line':
             currency = (self.invoice.currency if self.invoice
                 else self.currency)
-            amount = (Decimal(str(self.quantity or '0.0'))
-                * (self.unit_price or Decimal('0.0')))
+            amount = (Decimal(str(self.quantity or 0))
+                * (self.unit_price or Decimal(0)))
             invoice_type = (
                 self.invoice.type if self.invoice else self.invoice_type)
             if (invoice_type == 'in'
                     and self.taxes_deductible_rate is not None
                     and self.taxes_deductible_rate != 1):
                 with Transaction().set_context(_deductible_rate=1):
                     tax_amount = sum(
                         t['amount'] for t in self._get_taxes().values())
                 non_deductible_amount = (
                     tax_amount * (1 - self.taxes_deductible_rate))
                 amount += non_deductible_amount
             if currency:
                 return currency.round(amount)
             return amount
-        return Decimal('0.0')
+        return Decimal(0)
 
     def get_amount(self, name):
         if self.type == 'line':
             return self.on_change_with_amount()
         elif self.type == 'subtotal':
             subtotal = Decimal(0)
             for line2 in self.invoice.lines:
@@ -2990,19 +2992,19 @@
     @classmethod
     def __setup__(cls):
         super().__setup__()
         cls.__access__.add('invoice')
 
     @staticmethod
     def default_base():
-        return Decimal('0.0')
+        return Decimal(0)
 
     @staticmethod
     def default_amount():
-        return Decimal('0.0')
+        return Decimal(0)
 
     @staticmethod
     def default_manual():
         return True
 
     @classmethod
     def default_invoice_state(cls):
@@ -3451,15 +3453,15 @@
     @staticmethod
     def default_type():
         return 'partial'
 
     @fields.depends(
         'lines', 'amount', 'currency', 'invoice', 'payment_lines', 'company')
     def on_change_lines(self):
-        self.amount_writeoff = Decimal('0.0')
+        self.amount_writeoff = Decimal(0)
         if not self.invoice:
             return
 
         def balance(line):
             if self.currency == line.second_currency:
                 return line.amount_second_currency
             elif self.currency == self.company.currency:
@@ -3528,15 +3530,15 @@
 
     def transition_choice(self):
         invoice = self.record
         amount = self.start.amount
         currency = self.start.currency
         _, remainder = self.get_reconcile_lines_for_amount(
             invoice, amount, currency)
-        if remainder == Decimal('0.0') and amount <= invoice.amount_to_pay:
+        if remainder == Decimal(0) and amount <= invoice.amount_to_pay:
             return 'pay'
         return 'ask'
 
     def default_ask(self, fields):
         default = {}
         invoice = self.record
         amount = self.start.amount
```

### Comparing `trytond_account_invoice-7.2.1/invoice.xml` & `trytond_account_invoice-7.2.2/invoice.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/bg.po` & `trytond_account_invoice-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/ca.po` & `trytond_account_invoice-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/cs.po` & `trytond_account_invoice-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/de.po` & `trytond_account_invoice-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/es.po` & `trytond_account_invoice-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/es_419.po` & `trytond_account_invoice-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/et.po` & `trytond_account_invoice-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/fa.po` & `trytond_account_invoice-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/fi.po` & `trytond_account_invoice-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/fr.po` & `trytond_account_invoice-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/hu.po` & `trytond_account_invoice-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/id.po` & `trytond_account_invoice-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/it.po` & `trytond_account_invoice-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/lo.po` & `trytond_account_invoice-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/lt.po` & `trytond_account_invoice-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/nl.po` & `trytond_account_invoice-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/pl.po` & `trytond_account_invoice-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/pt.po` & `trytond_account_invoice-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/ro.po` & `trytond_account_invoice-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/ru.po` & `trytond_account_invoice-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/sl.po` & `trytond_account_invoice-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/tr.po` & `trytond_account_invoice-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/uk.po` & `trytond_account_invoice-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/locale/zh_CN.po` & `trytond_account_invoice-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/message.xml` & `trytond_account_invoice-7.2.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/party.py` & `trytond_account_invoice-7.2.2/party.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/party.xml` & `trytond_account_invoice-7.2.2/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/payment_term.py` & `trytond_account_invoice-7.2.2/payment_term.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,23 +50,23 @@
         """Calculate payment terms and return a list of tuples
         with (date, amount) for each payment term line.
 
         amount must be a Decimal used for the calculation.
         """
         # TODO implement business_days
         # http://pypi.python.org/pypi/BusinessHours/
-        sign = 1 if amount >= Decimal('0.0') else -1
+        sign = 1 if amount >= Decimal(0) else -1
         res = []
         remainder = amount
         for line in self.lines:
             value = line.get_value(remainder, amount, currency)
             value_date = line.get_date(date)
             if value is None or not value_date:
                 continue
-            if ((remainder - value) * sign) < Decimal('0.0'):
+            if ((remainder - value) * sign) < Decimal(0):
                 res.append((value_date, remainder))
                 break
             if value:
                 res.append((value_date, value))
             remainder -= value
         else:
             # Enforce to have at least one term
@@ -129,32 +129,32 @@
         if Transaction().user == 0:
             return []
         return [{}]
 
     @fields.depends('type')
     def on_change_type(self):
         if self.type != 'fixed':
-            self.amount = Decimal('0.0')
+            self.amount = Decimal(0)
             self.currency = None
         if self.type not in ('percent', 'percent_on_total'):
-            self.ratio = Decimal('0.0')
-            self.divisor = Decimal('0.0')
+            self.ratio = Decimal(0)
+            self.divisor = Decimal(0)
 
     @fields.depends('ratio')
     def on_change_ratio(self):
         if not self.ratio:
-            self.divisor = Decimal('0.0')
+            self.divisor = Decimal(0)
         else:
             self.divisor = self.round(1 / self.ratio,
                 self.__class__.divisor.digits[1])
 
     @fields.depends('divisor')
     def on_change_divisor(self):
         if not self.divisor:
-            self.ratio = Decimal('0.0')
+            self.ratio = Decimal(0)
         else:
             self.ratio = self.round(1 / self.divisor,
                 self.__class__.ratio.digits[1])
 
     def get_date(self, date):
         for relativedelta_ in self.relativedeltas:
             date += relativedelta_.get()
```

### Comparing `trytond_account_invoice-7.2.1/payment_term.xml` & `trytond_account_invoice-7.2.2/payment_term.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/setup.py` & `trytond_account_invoice-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_cancelling_invoice_move.rst` & `trytond_account_invoice-7.2.2/tests/scenario_cancelling_invoice_move.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_credit_note.rst` & `trytond_account_invoice-7.2.2/tests/scenario_credit_note.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_alternate_currency.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_exchange.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_alternate_currency_exchange.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_lower_rate.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_alternate_currency_lower_rate.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_alternate_currency_rate_change.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_alternate_currency_rate_change.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_alternative_payee.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_alternative_payee.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_customer_sequential.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_customer_sequential.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_group_line.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_group_line.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_in_future.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_in_future.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_manual_tax.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_manual_tax.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_overpayment.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_overpayment.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_report_revision.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_report_revision.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_reschedule_lines.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_reschedule_lines.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_supplier.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_supplier.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_supplier_post_paid.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_supplier_post_paid.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_tax_deductible.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_tax_deductible.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_invoice_with_credit.rst` & `trytond_account_invoice-7.2.2/tests/scenario_invoice_with_credit.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/scenario_renew_fiscalyear.rst` & `trytond_account_invoice-7.2.2/tests/scenario_renew_fiscalyear.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/test_module.py` & `trytond_account_invoice-7.2.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tests/tools.py` & `trytond_account_invoice-7.2.2/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/tox.ini` & `trytond_account_invoice-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/PKG-INFO` & `trytond_account_invoice-7.2.2/trytond_account_invoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module for invoicing
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice-7.2.1/trytond_account_invoice.egg-info/SOURCES.txt` & `trytond_account_invoice-7.2.2/trytond_account_invoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/credit_start_form.xml` & `trytond_account_invoice-7.2.2/view/credit_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/invoice_form.xml` & `trytond_account_invoice-7.2.2/view/invoice_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/invoice_line_form.xml` & `trytond_account_invoice-7.2.2/view/invoice_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/invoice_line_tree.xml` & `trytond_account_invoice-7.2.2/view/invoice_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/invoice_line_tree_sequence.xml` & `trytond_account_invoice-7.2.2/view/invoice_line_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/invoice_sequence_form.xml` & `trytond_account_invoice-7.2.2/view/invoice_sequence_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/invoice_tax_form.xml` & `trytond_account_invoice-7.2.2/view/invoice_tax_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/invoice_tax_tree_sequence.xml` & `trytond_account_invoice-7.2.2/view/invoice_tax_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/invoice_tree.xml` & `trytond_account_invoice-7.2.2/view/invoice_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/move_line_list_payment.xml` & `trytond_account_invoice-7.2.2/view/move_line_list_payment.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/party_form.xml` & `trytond_account_invoice-7.2.2/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/pay_ask_form.xml` & `trytond_account_invoice-7.2.2/view/pay_ask_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/pay_start_form.xml` & `trytond_account_invoice-7.2.2/view/pay_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/payment_method_form.xml` & `trytond_account_invoice-7.2.2/view/payment_method_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/payment_term_form.xml` & `trytond_account_invoice-7.2.2/view/payment_term_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/payment_term_line_form.xml` & `trytond_account_invoice-7.2.2/view/payment_term_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice-7.2.1/view/payment_term_line_relativedelta_form.xml` & `trytond_account_invoice-7.2.2/view/payment_term_line_relativedelta_form.xml`

 * *Files identical despite different names*

