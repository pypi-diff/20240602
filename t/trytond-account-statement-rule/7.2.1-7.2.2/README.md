# Comparing `tmp/trytond_account_statement_rule-7.2.1.tar.gz` & `tmp/trytond_account_statement_rule-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_statement_rule-7.2.1.tar", last modified: Wed May  1 12:15:41 2024, max compression
+gzip compressed data, was "trytond_account_statement_rule-7.2.2.tar", last modified: Sun Jun  2 16:57:14 2024, max compression
```

## Comparing `trytond_account_statement_rule-7.2.1.tar` & `trytond_account_statement_rule-7.2.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.935118 trytond_account_statement_rule-7.2.1/
--rw-r--r--   0 ced       (1000) ced       (1000)     1226 2024-05-01 12:15:38.000000 trytond_account_statement_rule-7.2.1/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-05-01 12:15:38.000000 trytond_account_statement_rule-7.2.1/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     4478 2024-05-01 12:15:41.935118 trytond_account_statement_rule-7.2.1/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1821 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15926 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5381 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.931785 trytond_account_statement_rule-7.2.1/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1821 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.931785 trytond_account_statement_rule-7.2.1/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5079 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5290 2024-04-30 17:21:59.000000 trytond_account_statement_rule-7.2.1/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4198 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4268 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5253 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4673 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4088 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-01 12:15:41.935118 trytond_account_statement_rule-7.2.1/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4534 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.931785 trytond_account_statement_rule-7.2.1/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2641 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3950 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule_keyword_bank_account.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3484 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule_keywords.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      429 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-04-30 17:21:06.000000 trytond_account_statement_rule-7.2.1/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.935118 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     4478 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     2139 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-01 12:15:41.935118 trytond_account_statement_rule-7.2.1/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1017 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1031 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_information_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      277 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_information_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/statement_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.1/view/statement_tree.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:57:14.761994 trytond_account_statement_rule-7.2.2/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1327 2024-06-02 16:57:11.000000 trytond_account_statement_rule-7.2.2/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      651 2024-06-02 16:57:11.000000 trytond_account_statement_rule-7.2.2/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     4478 2024-06-02 16:57:14.761994 trytond_account_statement_rule-7.2.2/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1821 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15922 2024-05-26 17:46:37.000000 trytond_account_statement_rule-7.2.2/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5381 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:57:14.755328 trytond_account_statement_rule-7.2.2/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3085 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1821 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:57:14.758661 trytond_account_statement_rule-7.2.2/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5079 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5290 2024-04-30 17:21:59.000000 trytond_account_statement_rule-7.2.2/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5081 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4498 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5176 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4198 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4268 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4170 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5253 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4673 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4142 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4088 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4108 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-06-02 16:57:14.761994 trytond_account_statement_rule-7.2.2/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4534 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:57:14.758661 trytond_account_statement_rule-7.2.2/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2641 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/tests/scenario_account_statement_rule.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3950 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/tests/scenario_account_statement_rule_keyword_bank_account.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3484 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/tests/scenario_account_statement_rule_keywords.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      429 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      160 2024-05-01 12:15:48.000000 trytond_account_statement_rule-7.2.2/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:57:14.758661 trytond_account_statement_rule-7.2.2/trytond_account_statement_rule.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4478 2024-06-02 16:57:14.000000 trytond_account_statement_rule-7.2.2/trytond_account_statement_rule.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2139 2024-06-02 16:57:14.000000 trytond_account_statement_rule-7.2.2/trytond_account_statement_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-06-02 16:57:14.000000 trytond_account_statement_rule-7.2.2/trytond_account_statement_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       82 2024-06-02 16:57:14.000000 trytond_account_statement_rule-7.2.2/trytond_account_statement_rule.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-01 12:15:41.000000 trytond_account_statement_rule-7.2.2/trytond_account_statement_rule.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2024-06-02 16:57:14.000000 trytond_account_statement_rule-7.2.2/trytond_account_statement_rule.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-06-02 16:57:14.000000 trytond_account_statement_rule-7.2.2/trytond_account_statement_rule.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-06-02 16:57:14.758661 trytond_account_statement_rule-7.2.2/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1017 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1031 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/view/rule_information_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      277 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/view/rule_information_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/view/rule_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      345 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/view/rule_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/view/rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/view/statement_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2024-04-30 17:20:59.000000 trytond_account_statement_rule-7.2.2/view/statement_tree.xml
```

### Comparing `trytond_account_statement_rule-7.2.1/CHANGELOG` & `trytond_account_statement_rule-7.2.2/CHANGELOG`

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

### Comparing `trytond_account_statement_rule-7.2.1/COPYRIGHT` & `trytond_account_statement_rule-7.2.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/LICENSE` & `trytond_account_statement_rule-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/PKG-INFO` & `trytond_account_statement_rule-7.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_rule
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module to automate statement import with rules
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_statement_rule-7.2.1/README.rst` & `trytond_account_statement_rule-7.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/__init__.py` & `trytond_account_statement_rule-7.2.2/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/account.py` & `trytond_account_statement_rule-7.2.2/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
         account = self.account
         if not account:
             related_to_account = self._get_account_from(related_to)
             if related_to_account:
                 account = related_to_account
             elif party:
                 with Transaction().set_context(date=origin.date):
-                    if amount > Decimal('0.0'):
+                    if amount > Decimal(0):
                         account = party.account_receivable_used
                     else:
                         account = party.account_payable_used
 
         if not account:
             return
         if not party:
```

### Comparing `trytond_account_statement_rule-7.2.1/account.xml` & `trytond_account_statement_rule-7.2.2/account.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/doc/conf.py` & `trytond_account_statement_rule-7.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/doc/index.rst` & `trytond_account_statement_rule-7.2.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/bg.po` & `trytond_account_statement_rule-7.2.2/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/ca.po` & `trytond_account_statement_rule-7.2.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/cs.po` & `trytond_account_statement_rule-7.2.2/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/de.po` & `trytond_account_statement_rule-7.2.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/es.po` & `trytond_account_statement_rule-7.2.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/es_419.po` & `trytond_account_statement_rule-7.2.2/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/et.po` & `trytond_account_statement_rule-7.2.2/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/fa.po` & `trytond_account_statement_rule-7.2.2/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/fi.po` & `trytond_account_statement_rule-7.2.2/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/fr.po` & `trytond_account_statement_rule-7.2.2/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/hu.po` & `trytond_account_statement_rule-7.2.2/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/id.po` & `trytond_account_statement_rule-7.2.2/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/it.po` & `trytond_account_statement_rule-7.2.2/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/lo.po` & `trytond_account_statement_rule-7.2.2/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/lt.po` & `trytond_account_statement_rule-7.2.2/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/nl.po` & `trytond_account_statement_rule-7.2.2/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/pl.po` & `trytond_account_statement_rule-7.2.2/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/pt.po` & `trytond_account_statement_rule-7.2.2/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/ro.po` & `trytond_account_statement_rule-7.2.2/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/ru.po` & `trytond_account_statement_rule-7.2.2/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/sl.po` & `trytond_account_statement_rule-7.2.2/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/tr.po` & `trytond_account_statement_rule-7.2.2/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/uk.po` & `trytond_account_statement_rule-7.2.2/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/locale/zh_CN.po` & `trytond_account_statement_rule-7.2.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/setup.py` & `trytond_account_statement_rule-7.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule.rst` & `trytond_account_statement_rule-7.2.2/tests/scenario_account_statement_rule.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule_keyword_bank_account.rst` & `trytond_account_statement_rule-7.2.2/tests/scenario_account_statement_rule_keyword_bank_account.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/tests/scenario_account_statement_rule_keywords.rst` & `trytond_account_statement_rule-7.2.2/tests/scenario_account_statement_rule_keywords.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/tox.ini` & `trytond_account_statement_rule-7.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/PKG-INFO` & `trytond_account_statement_rule-7.2.2/trytond_account_statement_rule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_statement_rule
-Version: 7.2.1
+Version: 7.2.2
 Summary: Tryton module to automate statement import with rules
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_statement_rule-7.2.1/trytond_account_statement_rule.egg-info/SOURCES.txt` & `trytond_account_statement_rule-7.2.2/trytond_account_statement_rule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/view/rule_form.xml` & `trytond_account_statement_rule-7.2.2/view/rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_account_statement_rule-7.2.1/view/rule_information_form.xml` & `trytond_account_statement_rule-7.2.2/view/rule_information_form.xml`

 * *Files identical despite different names*

