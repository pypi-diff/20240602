# Comparing `tmp/mds_account_de_skr04-7.0.8.tar.gz` & `tmp/mds_account_de_skr04-7.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_account_de_skr04-7.0.8.tar", last modified: Tue Mar 26 10:38:33 2024, max compression
+gzip compressed data, was "mds_account_de_skr04-7.0.9.tar", last modified: Sun Jun  2 18:23:55 2024, max compression
```

## Comparing `mds_account_de_skr04-7.0.8.tar` & `mds_account_de_skr04-7.0.9.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-03-26 10:38:32.998659 mds_account_de_skr04-7.0.8/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    35147 2023-12-01 14:36:50.000000 mds_account_de_skr04-7.0.8/LICENSE
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1639 2024-03-26 10:38:32.998659 mds_account_de_skr04-7.0.8/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      410 2024-03-26 10:33:20.000000 mds_account_de_skr04-7.0.8/README.rst
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      214 2023-12-01 14:36:50.000000 mds_account_de_skr04-7.0.8/__init__.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)   420212 2024-03-26 09:37:59.000000 mds_account_de_skr04-7.0.8/account_template.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    44541 2024-03-26 09:37:49.000000 mds_account_de_skr04-7.0.8/account_type_template.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-03-26 10:38:32.998659 mds_account_de_skr04-7.0.8/mds_account_de_skr04.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1639 2024-03-26 10:38:32.000000 mds_account_de_skr04-7.0.8/mds_account_de_skr04.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      570 2024-03-26 10:38:32.000000 mds_account_de_skr04-7.0.8/mds_account_de_skr04.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2024-03-26 10:38:32.000000 mds_account_de_skr04-7.0.8/mds_account_de_skr04.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       83 2024-03-26 10:38:32.000000 mds_account_de_skr04-7.0.8/mds_account_de_skr04.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2024-03-26 10:38:32.000000 mds_account_de_skr04-7.0.8/mds_account_de_skr04.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2024-03-26 10:38:32.000000 mds_account_de_skr04-7.0.8/mds_account_de_skr04.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2024-03-26 10:38:32.000000 mds_account_de_skr04-7.0.8/mds_account_de_skr04.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2024-03-26 10:38:32.998659 mds_account_de_skr04-7.0.8/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3613 2023-12-01 14:47:16.000000 mds_account_de_skr04-7.0.8/setup.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    19914 2024-03-26 10:29:59.000000 mds_account_de_skr04-7.0.8/tax_code_line_template.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    26405 2024-03-26 09:37:07.000000 mds_account_de_skr04-7.0.8/tax_code_template.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      902 2024-03-26 09:37:17.000000 mds_account_de_skr04-7.0.8/tax_group.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2272 2024-03-26 09:37:25.000000 mds_account_de_skr04-7.0.8/tax_rule_line_template.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1772 2024-03-26 09:37:33.000000 mds_account_de_skr04-7.0.8/tax_rule_template.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    11947 2024-03-26 09:37:41.000000 mds_account_de_skr04-7.0.8/tax_template.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      257 2024-03-26 10:36:36.000000 mds_account_de_skr04-7.0.8/tryton.cfg
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-06-02 18:23:55.516754 mds_account_de_skr04-7.0.9/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    35147 2024-06-02 18:10:46.000000 mds_account_de_skr04-7.0.9/LICENSE
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)       76 2024-06-02 18:15:12.000000 mds_account_de_skr04-7.0.9/MANIFEST.in
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1718 2024-06-02 18:23:55.516754 mds_account_de_skr04-7.0.9/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      457 2024-06-02 18:22:50.000000 mds_account_de_skr04-7.0.9/README.rst
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      214 2024-06-02 18:10:46.000000 mds_account_de_skr04-7.0.9/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)   420257 2024-06-02 18:21:40.000000 mds_account_de_skr04-7.0.9/account_template.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    44586 2024-06-02 18:21:40.000000 mds_account_de_skr04-7.0.9/account_type_template.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2024-06-02 18:23:55.516754 mds_account_de_skr04-7.0.9/mds_account_de_skr04.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1718 2024-06-02 18:23:55.000000 mds_account_de_skr04-7.0.9/mds_account_de_skr04.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      605 2024-06-02 18:23:55.000000 mds_account_de_skr04-7.0.9/mds_account_de_skr04.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2024-06-02 18:23:55.000000 mds_account_de_skr04-7.0.9/mds_account_de_skr04.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       83 2024-06-02 18:23:55.000000 mds_account_de_skr04-7.0.9/mds_account_de_skr04.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2024-06-02 18:23:55.000000 mds_account_de_skr04-7.0.9/mds_account_de_skr04.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2024-06-02 18:23:55.000000 mds_account_de_skr04-7.0.9/mds_account_de_skr04.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2024-06-02 18:23:55.000000 mds_account_de_skr04-7.0.9/mds_account_de_skr04.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2024-06-02 18:23:55.516754 mds_account_de_skr04-7.0.9/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3770 2024-06-02 18:21:40.000000 mds_account_de_skr04-7.0.9/setup.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    19959 2024-06-02 18:21:40.000000 mds_account_de_skr04-7.0.9/tax_code_line_template.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    26450 2024-06-02 18:21:40.000000 mds_account_de_skr04-7.0.9/tax_code_template.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      947 2024-06-02 18:21:40.000000 mds_account_de_skr04-7.0.9/tax_group.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2317 2024-06-02 18:21:40.000000 mds_account_de_skr04-7.0.9/tax_rule_line_template.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1817 2024-06-02 18:21:40.000000 mds_account_de_skr04-7.0.9/tax_rule_template.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    11992 2024-06-02 18:21:40.000000 mds_account_de_skr04-7.0.9/tax_template.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      257 2024-06-02 18:22:58.000000 mds_account_de_skr04-7.0.9/tryton.cfg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        2 2024-06-02 18:10:46.000000 mds_account_de_skr04-7.0.9/versiondep.txt
```

### Comparing `mds_account_de_skr04-7.0.8/LICENSE` & `mds_account_de_skr04-7.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-7.0.8/PKG-INFO` & `mds_account_de_skr04-7.0.9/mds_account_de_skr04.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds_account_de_skr04
-Version: 7.0.8
+Name: mds-account-de-skr04
+Version: 7.0.9
 Summary: Tryton module with German chart of accounts SKR04
 Home-page: https://www.m-ds.de/
 Author: m-ds GmbH
 Author-email: service@m-ds.de
 License: GPL-3
 Description: Chart of accounts 'SKR04'
         =========================
@@ -17,14 +17,18 @@
         =======
         
           pip install mds-account-de-skr04
         
         Changes
         =======
         
+        *7.0.9 - 02.06.2024*
+        
+        - fix: setup + fileinfo
+        
         *7.0.8 - 26.03.2024*
         
         - fix: invert tax-code-lines for vorsteuer
         
         *7.0.7 - 01.12.2023*
         
         - compatiblity to Tryton 7.0
```

### Comparing `mds_account_de_skr04-7.0.8/account_template.xml` & `mds_account_de_skr04-7.0.9/account_template.xml`

 * *Files 0% similar despite different names*

#### Comparing `mds_account_de_skr04-7.0.8/account_template.xml` & `mds_account_de_skr04-7.0.9/account_template.xml`

```diff
@@ -1,10 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
-this repository contains the full copyright notices and license terms. -->
+<!-- This file is part of the account-de-skr04-module for Tryton from m-ds.de.
+ The COPYRIGHT file at the top level of
+ this repository contains the full copyright notices and license terms.-->
 <tryton>
   <data>
     <record id="root_de" model="account.account.template">
       <field name="name">Kontenplan SKR04 (Germany)</field>
       <field name="type" ref="type_balance"/>
       <field name="closed" eval="True"/>
     </record>
```

### Comparing `mds_account_de_skr04-7.0.8/account_type_template.xml` & `mds_account_de_skr04-7.0.9/account_type_template.xml`

 * *Files 0% similar despite different names*

#### Comparing `mds_account_de_skr04-7.0.8/account_type_template.xml` & `mds_account_de_skr04-7.0.9/account_type_template.xml`

```diff
@@ -1,10 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
-this repository contains the full copyright notices and license terms. -->
+<!-- This file is part of the account-de-skr04-module for Tryton from m-ds.de.
+ The COPYRIGHT file at the top level of
+ this repository contains the full copyright notices and license terms.-->
 <tryton>
   <data>
     <record id="type_balance" model="account.account.type.template">
       <field name="name">Kontentypenplan SKR04 (Germany)</field>
       <field eval="10" name="sequence"/>
     </record>
     <record id="type_960" model="account.account.type.template">
```

### Comparing `mds_account_de_skr04-7.0.8/mds_account_de_skr04.egg-info/PKG-INFO` & `mds_account_de_skr04-7.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds-account-de-skr04
-Version: 7.0.8
+Name: mds_account_de_skr04
+Version: 7.0.9
 Summary: Tryton module with German chart of accounts SKR04
 Home-page: https://www.m-ds.de/
 Author: m-ds GmbH
 Author-email: service@m-ds.de
 License: GPL-3
 Description: Chart of accounts 'SKR04'
         =========================
@@ -17,14 +17,18 @@
         =======
         
           pip install mds-account-de-skr04
         
         Changes
         =======
         
+        *7.0.9 - 02.06.2024*
+        
+        - fix: setup + fileinfo
+        
         *7.0.8 - 26.03.2024*
         
         - fix: invert tax-code-lines for vorsteuer
         
         *7.0.7 - 01.12.2023*
         
         - compatiblity to Tryton 7.0
```

### Comparing `mds_account_de_skr04-7.0.8/mds_account_de_skr04.egg-info/SOURCES.txt` & `mds_account_de_skr04-7.0.9/mds_account_de_skr04.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+LICENSE
+MANIFEST.in
 README.rst
 setup.py
+versiondep.txt
 ./LICENSE
 ./README.rst
 ./__init__.py
 ./account_template.xml
 ./account_type_template.xml
 ./tax_code_line_template.xml
 ./tax_code_template.xml
```

### Comparing `mds_account_de_skr04-7.0.8/setup.py` & `mds_account_de_skr04-7.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-""" Tryton module with German chart of accounts SKR04
-"""
+# -*- coding: utf-8 -*-
+# This file is part of the account-de-skr04-module for Tryton from m-ds.de.
+# The COPYRIGHT file at the top level of
+# this repository contains the full copyright notices and license terms.
+
 
 # Always prefer setuptools over distutils
 from setuptools import setup
 # To use a consistent encoding
 from codecs import open
 from os import path
 import re
```

### Comparing `mds_account_de_skr04-7.0.8/tax_code_line_template.xml` & `mds_account_de_skr04-7.0.9/tax_code_line_template.xml`

 * *Files 1% similar despite different names*

#### Comparing `mds_account_de_skr04-7.0.8/tax_code_line_template.xml` & `mds_account_de_skr04-7.0.9/tax_code_line_template.xml`

```diff
@@ -1,10 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
-this repository contains the full copyright notices and license terms. -->
+<!-- This file is part of the account-de-skr04-module for Tryton from m-ds.de.
+ The COPYRIGHT file at the top level of
+ this repository contains the full copyright notices and license terms.-->
 <tryton>
   <data>
     <!--21 -->
     <record model="account.tax.code.line.template" id="tax_code_21-tax_not_taxable_eu">
       <field name="code" ref="tax_code_21"/>
       <field name="tax" ref="tax_not_taxable_eu"/>
       <field name="operator">+</field>
```

### Comparing `mds_account_de_skr04-7.0.8/tax_code_template.xml` & `mds_account_de_skr04-7.0.9/tax_code_template.xml`

 * *Files 0% similar despite different names*

#### Comparing `mds_account_de_skr04-7.0.8/tax_code_template.xml` & `mds_account_de_skr04-7.0.9/tax_code_template.xml`

```diff
@@ -1,10 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
-this repository contains the full copyright notices and license terms. -->
+<!-- This file is part of the account-de-skr04-module for Tryton from m-ds.de.
+ The COPYRIGHT file at the top level of
+ this repository contains the full copyright notices and license terms.-->
 <tryton>
   <data>
     <record id="tax_code_USTVA" model="account.tax.code.template">
       <field name="name">Kennzifferntabelle SKR04 (Germany)</field>
       <field name="code">USTVA</field>
       <field name="account" ref="root_de"/>
     </record>
```

### Comparing `mds_account_de_skr04-7.0.8/tax_group.xml` & `mds_account_de_skr04-7.0.9/tax_group.xml`

 * *Files 25% similar despite different names*

#### Comparing `mds_account_de_skr04-7.0.8/tax_group.xml` & `mds_account_de_skr04-7.0.9/tax_group.xml`

```diff
@@ -1,10 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
-this repository contains the full copyright notices and license terms. -->
+<!-- This file is part of the account-de-skr04-module for Tryton from m-ds.de.
+ The COPYRIGHT file at the top level of
+ this repository contains the full copyright notices and license terms.-->
 <tryton>
   <data>
     <record id="tax_group_vst_reduced" model="account.tax.group">
       <field name="name">Vorsteuer ermäßigt</field>
       <field name="code">vst_reduced</field>
       <field name="kind">purchase</field>
     </record>
```

### Comparing `mds_account_de_skr04-7.0.8/tax_rule_line_template.xml` & `mds_account_de_skr04-7.0.9/tax_rule_line_template.xml`

 * *Files 14% similar despite different names*

#### Comparing `mds_account_de_skr04-7.0.8/tax_rule_line_template.xml` & `mds_account_de_skr04-7.0.9/tax_rule_line_template.xml`

```diff
@@ -1,10 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
-this repository contains the full copyright notices and license terms. -->
+<!-- This file is part of the account-de-skr04-module for Tryton from m-ds.de.
+ The COPYRIGHT file at the top level of
+ this repository contains the full copyright notices and license terms.-->
 <tryton>
   <data>
     <record id="tax_rule_line_11" model="account.tax.rule.line.template">
       <field name="rule" ref="tax_rule_non_eu_purchase"/>
       <field name="group" ref="tax_group_vst"/>
       <field name="tax" ref="tax_import_19"/>
     </record>
```

### Comparing `mds_account_de_skr04-7.0.8/tax_rule_template.xml` & `mds_account_de_skr04-7.0.9/tax_rule_template.xml`

 * *Files 2% similar despite different names*

#### Comparing `mds_account_de_skr04-7.0.8/tax_rule_template.xml` & `mds_account_de_skr04-7.0.9/tax_rule_template.xml`

```diff
@@ -1,10 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
-this repository contains the full copyright notices and license terms. -->
+<!-- This file is part of the account-de-skr04-module for Tryton from m-ds.de.
+ The COPYRIGHT file at the top level of
+ this repository contains the full copyright notices and license terms.-->
 <tryton>
   <data>
     <record id="tax_rule_eu_no_id_purchase" model="account.tax.rule.template">
       <field name="name">Lieferant EU (ohne Ust-ID)</field>
       <field name="account" ref="root_de"/>
       <field name="kind">purchase</field>
     </record>
```

### Comparing `mds_account_de_skr04-7.0.8/tax_template.xml` & `mds_account_de_skr04-7.0.9/tax_template.xml`

 * *Files 2% similar despite different names*

#### Comparing `mds_account_de_skr04-7.0.8/tax_template.xml` & `mds_account_de_skr04-7.0.9/tax_template.xml`

```diff
@@ -1,10 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
-this repository contains the full copyright notices and license terms. -->
+<!-- This file is part of the account-de-skr04-module for Tryton from m-ds.de.
+ The COPYRIGHT file at the top level of
+ this repository contains the full copyright notices and license terms.-->
 <tryton>
   <data>
     <!-- Nicht steuerbar für Drittland-EU -->
     <record id="tax_not_taxable_eu" model="account.tax.template">
       <field name="name">nicht steuerbar für Drittland-EU</field>
       <field name="account" ref="root_de"/>
       <field name="description">nicht steuerbar</field>
```

