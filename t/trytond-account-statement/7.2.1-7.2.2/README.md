# Comparing `tmp/trytond_account_statement-7.2.1.tar.gz` & `tmp/trytond_account_statement-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement-7.2.1.tar", last modified: Wed May  1 12:16:15 2024, max compression
+gzip compressed data, was "trytond_account_statement-7.2.2.tar", last modified: Sun Jun  2 17:00:21 2024, max compression
```

## Comparing `trytond_account_statement-7.2.1.tar` & `trytond_account_statement-7.2.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     5500 2024-05-01 12:16:12.000000 trytond_account_statement-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-05-01 12:16:11.000000 trytond_account_statement-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      897 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1403 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/account.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1552 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/bank.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.434242 trytond_account_statement-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      748 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3278 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/doc/requirements-doc.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3680 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/journal.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3104 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/journal.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.434242 trytond_account_statement-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    16002 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16795 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14452 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17297 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16837 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14608 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15240 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17386 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14426 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17016 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15409 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14586 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15204 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16521 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14726 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    17151 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14408 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15437 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15067 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15872 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15199 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14638 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13739 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14654 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3474 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)    51356 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/statement.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    47460 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/statement.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18593 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/statement.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14862 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/scenario_account_statement.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2553 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/scenario_account_statement_bank_account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3240 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/scenario_account_statement_second_currency_invoice.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2992 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/scenario_statement_origin.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3525 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/scenario_statement_origin_invoices.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      179 2024-04-30 17:21:06.000000 trytond_account_statement-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2872 2024-05-01 12:16:15.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.1/trytond_account_statement.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:16:15.437575 trytond_account_statement-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      670 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/line_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/line_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1732 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_import_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      663 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_journal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_journal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1003 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      564 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_line_tree_editable.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      961 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_origin_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_origin_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.1/view/statement_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:00:21.233784 trytond_account_statement-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5601 2024-06-02 17:00:17.000000 trytond_account_statement-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      763 2024-06-02 17:00:17.000000 trytond_account_statement-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-06-02 17:00:21.233784 trytond_account_statement-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      897 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1403 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/account.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1552 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/bank.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:00:21.230450 trytond_account_statement-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3080 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      748 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/doc/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3278 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/doc/requirements-doc.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3680 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/journal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3104 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/journal.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:00:21.230450 trytond_account_statement-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16002 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16795 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14452 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17297 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16837 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14608 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15240 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17386 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14426 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17016 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15409 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14586 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15204 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16521 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14726 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    17151 2024-04-30 17:21:59.000000 trytond_account_statement-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14408 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15437 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15067 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15872 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15199 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14638 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13739 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14654 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3474 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 17:00:21.233784 trytond_account_statement-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4635 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51356 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/statement.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    47452 2024-05-26 17:46:37.000000 trytond_account_statement-7.2.2/statement.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18593 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/statement.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:00:21.233784 trytond_account_statement-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14862 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/tests/scenario_account_statement.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2553 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/tests/scenario_account_statement_bank_account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3240 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/tests/scenario_account_statement_second_currency_invoice.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2992 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/tests/scenario_statement_origin.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3525 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/tests/scenario_statement_origin_invoices.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      179 2024-05-01 12:16:22.000000 trytond_account_statement-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:00:21.233784 trytond_account_statement-7.2.2/trytond_account_statement.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2937 2024-06-02 17:00:20.000000 trytond_account_statement-7.2.2/trytond_account_statement.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2872 2024-06-02 17:00:21.000000 trytond_account_statement-7.2.2/trytond_account_statement.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 17:00:20.000000 trytond_account_statement-7.2.2/trytond_account_statement.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2024-06-02 17:00:20.000000 trytond_account_statement-7.2.2/trytond_account_statement.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:16:14.000000 trytond_account_statement-7.2.2/trytond_account_statement.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      220 2024-06-02 17:00:20.000000 trytond_account_statement-7.2.2/trytond_account_statement.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 17:00:20.000000 trytond_account_statement-7.2.2/trytond_account_statement.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 17:00:21.233784 trytond_account_statement-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      670 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/line_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      430 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/line_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1732 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/statement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/statement_import_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      663 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/statement_journal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/statement_journal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1003 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/statement_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/statement_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      564 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/statement_line_tree_editable.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      961 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/statement_origin_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      524 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/statement_origin_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2024-04-30 17:20:59.000000 trytond_account_statement-7.2.2/view/statement_tree.xml
```

### Comparing `trytond_account_statement-7.2.1/CHANGELOG` & `trytond_account_statement-7.2.2/CHANGELOG`

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

### Comparing `trytond_account_statement-7.2.1/COPYRIGHT` & `trytond_account_statement-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/LICENSE` & `trytond_account_statement-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/PKG-INFO` & `trytond_account_statement-7.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module with account statements
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_statement-7.2.1/__init__.py` & `trytond_account_statement-7.2.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/account.py` & `trytond_account_statement-7.2.2/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/bank.py` & `trytond_account_statement-7.2.2/bank.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/doc/conf.py` & `trytond_account_statement-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/doc/configuration.rst` & `trytond_account_statement-7.2.2/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/doc/design.rst` & `trytond_account_statement-7.2.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/journal.py` & `trytond_account_statement-7.2.2/journal.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/journal.xml` & `trytond_account_statement-7.2.2/journal.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/bg.po` & `trytond_account_statement-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/ca.po` & `trytond_account_statement-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/cs.po` & `trytond_account_statement-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/de.po` & `trytond_account_statement-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/es.po` & `trytond_account_statement-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/es_419.po` & `trytond_account_statement-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/et.po` & `trytond_account_statement-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/fa.po` & `trytond_account_statement-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/fi.po` & `trytond_account_statement-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/fr.po` & `trytond_account_statement-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/hu.po` & `trytond_account_statement-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/id.po` & `trytond_account_statement-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/it.po` & `trytond_account_statement-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/lo.po` & `trytond_account_statement-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/lt.po` & `trytond_account_statement-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/nl.po` & `trytond_account_statement-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/pl.po` & `trytond_account_statement-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/pt.po` & `trytond_account_statement-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/ro.po` & `trytond_account_statement-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/ru.po` & `trytond_account_statement-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/sl.po` & `trytond_account_statement-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/tr.po` & `trytond_account_statement-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/uk.po` & `trytond_account_statement-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/locale/zh_CN.po` & `trytond_account_statement-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/message.xml` & `trytond_account_statement-7.2.2/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/setup.py` & `trytond_account_statement-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/statement.fodt` & `trytond_account_statement-7.2.2/statement.fodt`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/statement.py` & `trytond_account_statement-7.2.2/statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -865,15 +865,15 @@
         return [(None, '')] + [(m, get_name(m)) for m in models]
 
     @fields.depends('amount', 'party', 'date', methods=['invoice'])
     def on_change_party(self):
         if self.party:
             if self.amount:
                 with Transaction().set_context(date=self.date):
-                    if self.amount > Decimal("0.0"):
+                    if self.amount > Decimal(0):
                         self.account = self.party.account_receivable_used
                     else:
                         self.account = self.party.account_payable_used
 
         if self.invoice:
             if self.party:
                 if (self.invoice.party != self.party
@@ -891,15 +891,15 @@
             with Transaction().set_context(date=self.date):
                 if self.account and self.account not in (
                         self.party.account_receivable_used,
                         self.party.account_payable_used):
                     # The user has entered a non-default value, we keep it.
                     pass
                 elif self.amount:
-                    if self.amount > Decimal("0.0"):
+                    if self.amount > Decimal(0):
                         self.account = self.party.account_receivable_used
                     else:
                         self.account = self.party.account_payable_used
 
     @fields.depends('account', methods=['invoice'])
     def on_change_account(self):
         if self.invoice:
```

### Comparing `trytond_account_statement-7.2.1/statement.xml` & `trytond_account_statement-7.2.2/statement.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/tests/scenario_account_statement.rst` & `trytond_account_statement-7.2.2/tests/scenario_account_statement.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/tests/scenario_account_statement_bank_account.rst` & `trytond_account_statement-7.2.2/tests/scenario_account_statement_bank_account.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/tests/scenario_account_statement_second_currency_invoice.rst` & `trytond_account_statement-7.2.2/tests/scenario_account_statement_second_currency_invoice.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/tests/scenario_statement_origin.rst` & `trytond_account_statement-7.2.2/tests/scenario_statement_origin.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/tests/scenario_statement_origin_invoices.rst` & `trytond_account_statement-7.2.2/tests/scenario_statement_origin_invoices.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/tox.ini` & `trytond_account_statement-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/trytond_account_statement.egg-info/PKG-INFO` & `trytond_account_statement-7.2.2/trytond_account_statement.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module with account statements
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_statement-7.2.1/trytond_account_statement.egg-info/SOURCES.txt` & `trytond_account_statement-7.2.2/trytond_account_statement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/view/line_group_form.xml` & `trytond_account_statement-7.2.2/view/line_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/view/statement_form.xml` & `trytond_account_statement-7.2.2/view/statement_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/view/statement_journal_form.xml` & `trytond_account_statement-7.2.2/view/statement_journal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/view/statement_line_form.xml` & `trytond_account_statement-7.2.2/view/statement_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/view/statement_line_tree.xml` & `trytond_account_statement-7.2.2/view/statement_line_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/view/statement_line_tree_editable.xml` & `trytond_account_statement-7.2.2/view/statement_line_tree_editable.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/view/statement_origin_form.xml` & `trytond_account_statement-7.2.2/view/statement_origin_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement-7.2.1/view/statement_origin_tree.xml` & `trytond_account_statement-7.2.2/view/statement_origin_tree.xml`

 * *Files identical despite different names*

