# Comparing `tmp/bain-wizard-interpreter-1.0.3.tar.gz` & `tmp/bain_wizard_interpreter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bain-wizard-interpreter-1.0.3.tar", last modified: Thu Jun  2 07:45:05 2022, max compression
+gzip compressed data, was "bain_wizard_interpreter-1.0.4.tar", max compression
```

## Comparing `bain-wizard-interpreter-1.0.3.tar` & `bain_wizard_interpreter-1.0.4.tar`

### file list

```diff
@@ -1,41 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 07:45:05.010705 bain-wizard-interpreter-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6169 2022-06-02 07:45:05.010705 bain-wizard-interpreter-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5553 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 07:45:05.006705 bain-wizard-interpreter-1.0.3/bain_wizard_interpreter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6169 2022-06-02 07:45:04.000000 bain-wizard-interpreter-1.0.3/bain_wizard_interpreter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-06-02 07:45:04.000000 bain-wizard-interpreter-1.0.3/bain_wizard_interpreter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 07:45:04.000000 bain-wizard-interpreter-1.0.3/bain_wizard_interpreter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-02 07:45:04.000000 bain-wizard-interpreter-1.0.3/bain_wizard_interpreter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-02 07:45:04.000000 bain-wizard-interpreter-1.0.3/bain_wizard_interpreter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-06-02 07:45:05.010705 bain-wizard-interpreter-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 07:45:05.006705 bain-wizard-interpreter-1.0.3/wizard/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 07:45:05.010705 bain-wizard-interpreter-1.0.3/wizard/antlr4/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/antlr4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23501 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/antlr4/wizardLexer.py
--rw-r--r--   0 runner    (1001) docker     (121)    15487 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/antlr4/wizardListener.py
--rw-r--r--   0 runner    (1001) docker     (121)   125472 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/antlr4/wizardParser.py
--rw-r--r--   0 runner    (1001) docker     (121)     9447 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/antlr4/wizardVisitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 07:45:05.010705 bain-wizard-interpreter-1.0.3/wizard/contexts/
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28815 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/contexts/contexts.py
--rw-r--r--   0 runner    (1001) docker     (121)     6969 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/contexts/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     8995 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/contexts/keywords.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/contexts/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4895 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    13339 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/expr.py
--rw-r--r--   0 runner    (1001) docker     (121)     7492 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2383 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5539 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/keywords.py
--rw-r--r--   0 runner    (1001) docker     (121)     9099 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/mappings.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    10723 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     6093 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/scriptrunner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2418 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/severity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/state.py
--rw-r--r--   0 runner    (1001) docker     (121)     3199 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/tweaks.py
--rw-r--r--   0 runner    (1001) docker     (121)    10105 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12555 2022-06-02 07:44:54.000000 bain-wizard-interpreter-1.0.3/wizard/value.py
+-rw-r--r--   0        0        0     1046 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5937 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/README.md
+-rw-r--r--   0        0        0     1417 2024-06-02 09:32:34.452890 bain_wizard_interpreter-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/antlr4/__init__.py
+-rw-r--r--   0        0        0    11897 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizard.interp
+-rw-r--r--   0        0        0     1135 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizard.tokens
+-rw-r--r--   0        0        0    24710 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizardLexer.interp
+-rw-r--r--   0        0        0    77943 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizardLexer.py
+-rw-r--r--   0        0        0     1417 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizardLexer.pyi
+-rw-r--r--   0        0        0     1135 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizardLexer.tokens
+-rw-r--r--   0        0        0    15519 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizardListener.py
+-rw-r--r--   0        0        0   151969 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizardParser.py
+-rw-r--r--   0        0        0    15191 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizardParser.pyi
+-rw-r--r--   0        0        0     9424 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizardVisitor.py
+-rw-r--r--   0        0        0     2101 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/contexts/__init__.py
+-rw-r--r--   0        0        0    30804 2024-06-02 09:32:25.728892 bain_wizard_interpreter-1.0.4/src/wizard/contexts/contexts.py
+-rw-r--r--   0        0        0     8123 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/contexts/factory.py
+-rw-r--r--   0        0        0     9846 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/contexts/keywords.py
+-rw-r--r--   0        0        0     1079 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/contexts/utils.py
+-rw-r--r--   0        0        0     5360 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/errors.py
+-rw-r--r--   0        0        0    13778 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/expr.py
+-rw-r--r--   0        0        0     7766 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/functions.py
+-rw-r--r--   0        0        0     2438 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/interpreter.py
+-rw-r--r--   0        0        0     5865 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/keywords.py
+-rw-r--r--   0        0        0     9077 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/manager.py
+-rw-r--r--   0        0        0        0 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/py.typed
+-rw-r--r--   0        0        0    11193 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/runner.py
+-rw-r--r--   0        0        0     6342 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/scriptrunner.py
+-rw-r--r--   0        0        0     2397 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/severity.py
+-rw-r--r--   0        0        0     1322 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/state.py
+-rw-r--r--   0        0        0     3197 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/tweaks.py
+-rw-r--r--   0        0        0     6413 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/utils/__init__.py
+-rw-r--r--   0        0        0     4031 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/utils/error_strategy.py
+-rw-r--r--   0        0        0     2257 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/utils/mappings.py
+-rw-r--r--   0        0        0    13231 2024-06-02 09:32:25.732892 bain_wizard_interpreter-1.0.4/src/wizard/value.py
+-rw-r--r--   0        0        0     6451 1970-01-01 00:00:00.000000 bain_wizard_interpreter-1.0.4/PKG-INFO
```

### Comparing `bain-wizard-interpreter-1.0.3/LICENSE` & `bain_wizard_interpreter-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bain-wizard-interpreter-1.0.3/PKG-INFO` & `bain_wizard_interpreter-1.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,14 @@
-Metadata-Version: 2.1
-Name: bain-wizard-interpreter
-Version: 1.0.3
-Summary: A BAIN Wizard Interpreter based on wizparse.
-Home-page: https://github.com/Holt59/bain-wizard-interpreter
-Author: Holt59
-Author-email: capelle.mikael@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: tests
-License-File: LICENSE
-
 # BAIN Wizard Interpreter
 
-![Python Versions](https://img.shields.io/pypi/pyversions/bain-wizard-interpreter)
-![PyPi](https://img.shields.io/pypi/v/bain-wizard-interpreter?style=flat-square)
-![Tests](https://img.shields.io/github/workflow/status/holt59/bain-wizard-interpreter/Tests?style=flat-square)
-![Linters](https://img.shields.io/github/workflow/status/holt59/bain-wizard-interpreter/Linters?style=flat-square)
-![MIT License](https://img.shields.io/github/license/holt59/bain-wizard-interpreter?style=flat-square)
+![Python Versions](https://img.shields.io/pypi/pyversions/bain-wizard-interpreter?style=flat-square)
+[![PyPi](https://img.shields.io/pypi/v/bain-wizard-interpreter?style=flat-square)](https://pypi.org/project/bain-wizard-interpreter/)
+[![Tests](https://img.shields.io/github/actions/workflow/status/holt59/bain-wizard-interpreter/python-tests.yml?branch=master&label=tests&style=flat-square)](https://github.com/Holt59/bain-wizard-interpreter/actions/workflows/python-tests.yml)
+[![Linters](https://img.shields.io/github/actions/workflow/status/holt59/bain-wizard-interpreter/python-linters.yml?branch=master&label=linters&style=flat-square)](https://github.com/Holt59/bain-wizard-interpreter/actions/workflows/python-linters.yml)
+[![MIT License](https://img.shields.io/github/license/holt59/bain-wizard-interpreter?style=flat-square)](https://opensource.org/licenses/MIT)
 
 A BAIN Wizard Interpreter based on [`wizparse`](https://github.com/wrye-bash/wizparse) that can
 be used in various settings to run BAIN Wizard installers.
 
 # Basic Usage
 
 There are various way to use the interpreter.
@@ -173,15 +154,15 @@
 
 The code under [`wizard/antlr4`](wizard/antlr4) is generated from [`wizard/antlr4/wizard.g4`](wizard/antlr4/wizard.g4)
 from the [`wizparse`](https://github.com/wrye-bash/wizparse) repository.
 To generate the file, you need `antlr4`, and you simply have to run:
 
 ```bash
 # IMPORTANT: use FORWARD SLASH (/) everywhere, otherwise it does not work
-java -jar antlr-4.10.1-complete.jar -visitor -Dlanguage=Python3 -o ./wizard/antlr4 ./vendor/wizparse/wizards/wizard.g4
+java -jar antlr-4.13.1-complete.jar -visitor -Dlanguage=Python3 -o ./src/wizard/antlr4 ./vendor/wizparse/wizards/wizard.g4
 ```
 
 ## Run tests
 
 To run the tests, you need the Python 3 ANTLR4 runtime and `pytest`:
 
 ```bash
@@ -199,9 +180,7 @@
 
 - The code in [`wizard/antlr4`](wizard/antlr4) is generated from
   the [`wizparse`](https://github.com/wrye-bash/wizparse) repository, so the `wizparse`
   LICENSE applies to it.
 - The code in [`vendor/wizparse`](vendor/wizparse) is under the `wizparse` LICENSE.
 - The files in [`vendor/wizparse/tests`](vendor/wizparse/tests) have their own accompanying license. See the
   [`wizparse`](https://github.com/wrye-bash/wizparse) repository for more details.
-
-
```

### Comparing `bain-wizard-interpreter-1.0.3/README.md` & `bain_wizard_interpreter-1.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,29 @@
+Metadata-Version: 2.1
+Name: bain-wizard-interpreter
+Version: 1.0.4
+Summary: BAIN Wizard Interpreter based on wizparse.
+License: MIT
+Author: Mikaël Capelle
+Author-email: capelle.mikael@gmail.com
+Requires-Python: >=3.11.1,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: antlr4-python3-runtime (>=4.13.1,<5.0.0)
+Requires-Dist: chardet (>=5.2.0,<6.0.0)
+Description-Content-Type: text/markdown
+
 # BAIN Wizard Interpreter
 
-![Python Versions](https://img.shields.io/pypi/pyversions/bain-wizard-interpreter)
-![PyPi](https://img.shields.io/pypi/v/bain-wizard-interpreter?style=flat-square)
-![Tests](https://img.shields.io/github/workflow/status/holt59/bain-wizard-interpreter/Tests?style=flat-square)
-![Linters](https://img.shields.io/github/workflow/status/holt59/bain-wizard-interpreter/Linters?style=flat-square)
-![MIT License](https://img.shields.io/github/license/holt59/bain-wizard-interpreter?style=flat-square)
+![Python Versions](https://img.shields.io/pypi/pyversions/bain-wizard-interpreter?style=flat-square)
+[![PyPi](https://img.shields.io/pypi/v/bain-wizard-interpreter?style=flat-square)](https://pypi.org/project/bain-wizard-interpreter/)
+[![Tests](https://img.shields.io/github/actions/workflow/status/holt59/bain-wizard-interpreter/python-tests.yml?branch=master&label=tests&style=flat-square)](https://github.com/Holt59/bain-wizard-interpreter/actions/workflows/python-tests.yml)
+[![Linters](https://img.shields.io/github/actions/workflow/status/holt59/bain-wizard-interpreter/python-linters.yml?branch=master&label=linters&style=flat-square)](https://github.com/Holt59/bain-wizard-interpreter/actions/workflows/python-linters.yml)
+[![MIT License](https://img.shields.io/github/license/holt59/bain-wizard-interpreter?style=flat-square)](https://opensource.org/licenses/MIT)
 
 A BAIN Wizard Interpreter based on [`wizparse`](https://github.com/wrye-bash/wizparse) that can
 be used in various settings to run BAIN Wizard installers.
 
 # Basic Usage
 
 There are various way to use the interpreter.
@@ -154,15 +169,15 @@
 
 The code under [`wizard/antlr4`](wizard/antlr4) is generated from [`wizard/antlr4/wizard.g4`](wizard/antlr4/wizard.g4)
 from the [`wizparse`](https://github.com/wrye-bash/wizparse) repository.
 To generate the file, you need `antlr4`, and you simply have to run:
 
 ```bash
 # IMPORTANT: use FORWARD SLASH (/) everywhere, otherwise it does not work
-java -jar antlr-4.10.1-complete.jar -visitor -Dlanguage=Python3 -o ./wizard/antlr4 ./vendor/wizparse/wizards/wizard.g4
+java -jar antlr-4.13.1-complete.jar -visitor -Dlanguage=Python3 -o ./src/wizard/antlr4 ./vendor/wizparse/wizards/wizard.g4
 ```
 
 ## Run tests
 
 To run the tests, you need the Python 3 ANTLR4 runtime and `pytest`:
 
 ```bash
@@ -180,7 +195,8 @@
 
 - The code in [`wizard/antlr4`](wizard/antlr4) is generated from
   the [`wizparse`](https://github.com/wrye-bash/wizparse) repository, so the `wizparse`
   LICENSE applies to it.
 - The code in [`vendor/wizparse`](vendor/wizparse) is under the `wizparse` LICENSE.
 - The files in [`vendor/wizparse/tests`](vendor/wizparse/tests) have their own accompanying license. See the
   [`wizparse`](https://github.com/wrye-bash/wizparse) repository for more details.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/antlr4/wizardListener.py` & `bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizardListener.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,507 +1,453 @@
-# Generated from ./vendor/wizparse/wizards/wizard.g4 by ANTLR 4.10.1
+# Generated from ./vendor/wizparse/wizards/wizard.g4 by ANTLR 4.13.1
 from antlr4 import *
-if __name__ is not None and "." in __name__:
+
+if "." in __name__:
     from .wizardParser import wizardParser
 else:
     from wizardParser import wizardParser
 
+
 # This class defines a complete listener for a parse tree produced by wizardParser.
 class wizardListener(ParseTreeListener):
-
     # Enter a parse tree produced by wizardParser#parseWizard.
-    def enterParseWizard(self, ctx:wizardParser.ParseWizardContext):
+    def enterParseWizard(self, ctx: wizardParser.ParseWizardContext):
         pass
 
     # Exit a parse tree produced by wizardParser#parseWizard.
-    def exitParseWizard(self, ctx:wizardParser.ParseWizardContext):
+    def exitParseWizard(self, ctx: wizardParser.ParseWizardContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#body.
-    def enterBody(self, ctx:wizardParser.BodyContext):
+    def enterBody(self, ctx: wizardParser.BodyContext):
         pass
 
     # Exit a parse tree produced by wizardParser#body.
-    def exitBody(self, ctx:wizardParser.BodyContext):
+    def exitBody(self, ctx: wizardParser.BodyContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#stmt.
-    def enterStmt(self, ctx:wizardParser.StmtContext):
+    def enterStmt(self, ctx: wizardParser.StmtContext):
         pass
 
     # Exit a parse tree produced by wizardParser#stmt.
-    def exitStmt(self, ctx:wizardParser.StmtContext):
+    def exitStmt(self, ctx: wizardParser.StmtContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#assignment.
-    def enterAssignment(self, ctx:wizardParser.AssignmentContext):
+    def enterAssignment(self, ctx: wizardParser.AssignmentContext):
         pass
 
     # Exit a parse tree produced by wizardParser#assignment.
-    def exitAssignment(self, ctx:wizardParser.AssignmentContext):
+    def exitAssignment(self, ctx: wizardParser.AssignmentContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#compoundAssignment.
-    def enterCompoundAssignment(self, ctx:wizardParser.CompoundAssignmentContext):
+    def enterCompoundAssignment(self, ctx: wizardParser.CompoundAssignmentContext):
         pass
 
     # Exit a parse tree produced by wizardParser#compoundAssignment.
-    def exitCompoundAssignment(self, ctx:wizardParser.CompoundAssignmentContext):
+    def exitCompoundAssignment(self, ctx: wizardParser.CompoundAssignmentContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Break.
-    def enterBreak(self, ctx:wizardParser.BreakContext):
+    def enterBreak(self, ctx: wizardParser.BreakContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Break.
-    def exitBreak(self, ctx:wizardParser.BreakContext):
+    def exitBreak(self, ctx: wizardParser.BreakContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Cancel.
-    def enterCancel(self, ctx:wizardParser.CancelContext):
+    def enterCancel(self, ctx: wizardParser.CancelContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Cancel.
-    def exitCancel(self, ctx:wizardParser.CancelContext):
+    def exitCancel(self, ctx: wizardParser.CancelContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Continue.
-    def enterContinue(self, ctx:wizardParser.ContinueContext):
+    def enterContinue(self, ctx: wizardParser.ContinueContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Continue.
-    def exitContinue(self, ctx:wizardParser.ContinueContext):
+    def exitContinue(self, ctx: wizardParser.ContinueContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#For.
-    def enterFor(self, ctx:wizardParser.ForContext):
+    def enterFor(self, ctx: wizardParser.ForContext):
         pass
 
     # Exit a parse tree produced by wizardParser#For.
-    def exitFor(self, ctx:wizardParser.ForContext):
+    def exitFor(self, ctx: wizardParser.ForContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#If.
-    def enterIf(self, ctx:wizardParser.IfContext):
+    def enterIf(self, ctx: wizardParser.IfContext):
         pass
 
     # Exit a parse tree produced by wizardParser#If.
-    def exitIf(self, ctx:wizardParser.IfContext):
+    def exitIf(self, ctx: wizardParser.IfContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Return.
-    def enterReturn(self, ctx:wizardParser.ReturnContext):
+    def enterReturn(self, ctx: wizardParser.ReturnContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Return.
-    def exitReturn(self, ctx:wizardParser.ReturnContext):
+    def exitReturn(self, ctx: wizardParser.ReturnContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Select.
-    def enterSelect(self, ctx:wizardParser.SelectContext):
+    def enterSelect(self, ctx: wizardParser.SelectContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Select.
-    def exitSelect(self, ctx:wizardParser.SelectContext):
+    def exitSelect(self, ctx: wizardParser.SelectContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#While.
-    def enterWhile(self, ctx:wizardParser.WhileContext):
+    def enterWhile(self, ctx: wizardParser.WhileContext):
         pass
 
     # Exit a parse tree produced by wizardParser#While.
-    def exitWhile(self, ctx:wizardParser.WhileContext):
+    def exitWhile(self, ctx: wizardParser.WhileContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#cancelStmt.
-    def enterCancelStmt(self, ctx:wizardParser.CancelStmtContext):
+    def enterCancelStmt(self, ctx: wizardParser.CancelStmtContext):
         pass
 
     # Exit a parse tree produced by wizardParser#cancelStmt.
-    def exitCancelStmt(self, ctx:wizardParser.CancelStmtContext):
+    def exitCancelStmt(self, ctx: wizardParser.CancelStmtContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#caseStmt.
-    def enterCaseStmt(self, ctx:wizardParser.CaseStmtContext):
+    def enterCaseStmt(self, ctx: wizardParser.CaseStmtContext):
         pass
 
     # Exit a parse tree produced by wizardParser#caseStmt.
-    def exitCaseStmt(self, ctx:wizardParser.CaseStmtContext):
+    def exitCaseStmt(self, ctx: wizardParser.CaseStmtContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#defaultStmt.
-    def enterDefaultStmt(self, ctx:wizardParser.DefaultStmtContext):
+    def enterDefaultStmt(self, ctx: wizardParser.DefaultStmtContext):
         pass
 
     # Exit a parse tree produced by wizardParser#defaultStmt.
-    def exitDefaultStmt(self, ctx:wizardParser.DefaultStmtContext):
+    def exitDefaultStmt(self, ctx: wizardParser.DefaultStmtContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#elifStmt.
-    def enterElifStmt(self, ctx:wizardParser.ElifStmtContext):
+    def enterElifStmt(self, ctx: wizardParser.ElifStmtContext):
         pass
 
     # Exit a parse tree produced by wizardParser#elifStmt.
-    def exitElifStmt(self, ctx:wizardParser.ElifStmtContext):
+    def exitElifStmt(self, ctx: wizardParser.ElifStmtContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#elseStmt.
-    def enterElseStmt(self, ctx:wizardParser.ElseStmtContext):
+    def enterElseStmt(self, ctx: wizardParser.ElseStmtContext):
         pass
 
     # Exit a parse tree produced by wizardParser#elseStmt.
-    def exitElseStmt(self, ctx:wizardParser.ElseStmtContext):
+    def exitElseStmt(self, ctx: wizardParser.ElseStmtContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#forStmt.
-    def enterForStmt(self, ctx:wizardParser.ForStmtContext):
+    def enterForStmt(self, ctx: wizardParser.ForStmtContext):
         pass
 
     # Exit a parse tree produced by wizardParser#forStmt.
-    def exitForStmt(self, ctx:wizardParser.ForStmtContext):
+    def exitForStmt(self, ctx: wizardParser.ForStmtContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#forRangeHeader.
-    def enterForRangeHeader(self, ctx:wizardParser.ForRangeHeaderContext):
+    def enterForRangeHeader(self, ctx: wizardParser.ForRangeHeaderContext):
         pass
 
     # Exit a parse tree produced by wizardParser#forRangeHeader.
-    def exitForRangeHeader(self, ctx:wizardParser.ForRangeHeaderContext):
+    def exitForRangeHeader(self, ctx: wizardParser.ForRangeHeaderContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#forInHeader.
-    def enterForInHeader(self, ctx:wizardParser.ForInHeaderContext):
+    def enterForInHeader(self, ctx: wizardParser.ForInHeaderContext):
         pass
 
     # Exit a parse tree produced by wizardParser#forInHeader.
-    def exitForInHeader(self, ctx:wizardParser.ForInHeaderContext):
+    def exitForInHeader(self, ctx: wizardParser.ForInHeaderContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#ifStmt.
-    def enterIfStmt(self, ctx:wizardParser.IfStmtContext):
+    def enterIfStmt(self, ctx: wizardParser.IfStmtContext):
         pass
 
     # Exit a parse tree produced by wizardParser#ifStmt.
-    def exitIfStmt(self, ctx:wizardParser.IfStmtContext):
+    def exitIfStmt(self, ctx: wizardParser.IfStmtContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#selectStmt.
-    def enterSelectStmt(self, ctx:wizardParser.SelectStmtContext):
+    def enterSelectStmt(self, ctx: wizardParser.SelectStmtContext):
         pass
 
     # Exit a parse tree produced by wizardParser#selectStmt.
-    def exitSelectStmt(self, ctx:wizardParser.SelectStmtContext):
+    def exitSelectStmt(self, ctx: wizardParser.SelectStmtContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#selectCaseList.
-    def enterSelectCaseList(self, ctx:wizardParser.SelectCaseListContext):
+    def enterSelectCaseList(self, ctx: wizardParser.SelectCaseListContext):
         pass
 
     # Exit a parse tree produced by wizardParser#selectCaseList.
-    def exitSelectCaseList(self, ctx:wizardParser.SelectCaseListContext):
+    def exitSelectCaseList(self, ctx: wizardParser.SelectCaseListContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#optionTuple.
-    def enterOptionTuple(self, ctx:wizardParser.OptionTupleContext):
+    def enterOptionTuple(self, ctx: wizardParser.OptionTupleContext):
         pass
 
     # Exit a parse tree produced by wizardParser#optionTuple.
-    def exitOptionTuple(self, ctx:wizardParser.OptionTupleContext):
+    def exitOptionTuple(self, ctx: wizardParser.OptionTupleContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#selectOne.
-    def enterSelectOne(self, ctx:wizardParser.SelectOneContext):
+    def enterSelectOne(self, ctx: wizardParser.SelectOneContext):
         pass
 
     # Exit a parse tree produced by wizardParser#selectOne.
-    def exitSelectOne(self, ctx:wizardParser.SelectOneContext):
+    def exitSelectOne(self, ctx: wizardParser.SelectOneContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#selectMany.
-    def enterSelectMany(self, ctx:wizardParser.SelectManyContext):
+    def enterSelectMany(self, ctx: wizardParser.SelectManyContext):
         pass
 
     # Exit a parse tree produced by wizardParser#selectMany.
-    def exitSelectMany(self, ctx:wizardParser.SelectManyContext):
+    def exitSelectMany(self, ctx: wizardParser.SelectManyContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#whileStmt.
-    def enterWhileStmt(self, ctx:wizardParser.WhileStmtContext):
+    def enterWhileStmt(self, ctx: wizardParser.WhileStmtContext):
         pass
 
     # Exit a parse tree produced by wizardParser#whileStmt.
-    def exitWhileStmt(self, ctx:wizardParser.WhileStmtContext):
+    def exitWhileStmt(self, ctx: wizardParser.WhileStmtContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#argList.
-    def enterArgList(self, ctx:wizardParser.ArgListContext):
+    def enterArgList(self, ctx: wizardParser.ArgListContext):
         pass
 
     # Exit a parse tree produced by wizardParser#argList.
-    def exitArgList(self, ctx:wizardParser.ArgListContext):
+    def exitArgList(self, ctx: wizardParser.ArgListContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#keywordStmt.
-    def enterKeywordStmt(self, ctx:wizardParser.KeywordStmtContext):
+    def enterKeywordStmt(self, ctx: wizardParser.KeywordStmtContext):
         pass
 
     # Exit a parse tree produced by wizardParser#keywordStmt.
-    def exitKeywordStmt(self, ctx:wizardParser.KeywordStmtContext):
+    def exitKeywordStmt(self, ctx: wizardParser.KeywordStmtContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#PreIncrement.
-    def enterPreIncrement(self, ctx:wizardParser.PreIncrementContext):
+    def enterPreIncrement(self, ctx: wizardParser.PreIncrementContext):
         pass
 
     # Exit a parse tree produced by wizardParser#PreIncrement.
-    def exitPreIncrement(self, ctx:wizardParser.PreIncrementContext):
+    def exitPreIncrement(self, ctx: wizardParser.PreIncrementContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#DotFunctionCall.
-    def enterDotFunctionCall(self, ctx:wizardParser.DotFunctionCallContext):
+    def enterDotFunctionCall(self, ctx: wizardParser.DotFunctionCallContext):
         pass
 
     # Exit a parse tree produced by wizardParser#DotFunctionCall.
-    def exitDotFunctionCall(self, ctx:wizardParser.DotFunctionCallContext):
+    def exitDotFunctionCall(self, ctx: wizardParser.DotFunctionCallContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Or.
-    def enterOr(self, ctx:wizardParser.OrContext):
+    def enterOr(self, ctx: wizardParser.OrContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Or.
-    def exitOr(self, ctx:wizardParser.OrContext):
+    def exitOr(self, ctx: wizardParser.OrContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#In.
-    def enterIn(self, ctx:wizardParser.InContext):
+    def enterIn(self, ctx: wizardParser.InContext):
         pass
 
     # Exit a parse tree produced by wizardParser#In.
-    def exitIn(self, ctx:wizardParser.InContext):
+    def exitIn(self, ctx: wizardParser.InContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#PostDecrement.
-    def enterPostDecrement(self, ctx:wizardParser.PostDecrementContext):
+    def enterPostDecrement(self, ctx: wizardParser.PostDecrementContext):
         pass
 
     # Exit a parse tree produced by wizardParser#PostDecrement.
-    def exitPostDecrement(self, ctx:wizardParser.PostDecrementContext):
+    def exitPostDecrement(self, ctx: wizardParser.PostDecrementContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#TimesDivideModulo.
-    def enterTimesDivideModulo(self, ctx:wizardParser.TimesDivideModuloContext):
+    def enterTimesDivideModulo(self, ctx: wizardParser.TimesDivideModuloContext):
         pass
 
     # Exit a parse tree produced by wizardParser#TimesDivideModulo.
-    def exitTimesDivideModulo(self, ctx:wizardParser.TimesDivideModuloContext):
+    def exitTimesDivideModulo(self, ctx: wizardParser.TimesDivideModuloContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Index.
-    def enterIndex(self, ctx:wizardParser.IndexContext):
+    def enterIndex(self, ctx: wizardParser.IndexContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Index.
-    def exitIndex(self, ctx:wizardParser.IndexContext):
+    def exitIndex(self, ctx: wizardParser.IndexContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Exponentiation.
-    def enterExponentiation(self, ctx:wizardParser.ExponentiationContext):
+    def enterExponentiation(self, ctx: wizardParser.ExponentiationContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Exponentiation.
-    def exitExponentiation(self, ctx:wizardParser.ExponentiationContext):
+    def exitExponentiation(self, ctx: wizardParser.ExponentiationContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#PlusMinus.
-    def enterPlusMinus(self, ctx:wizardParser.PlusMinusContext):
+    def enterPlusMinus(self, ctx: wizardParser.PlusMinusContext):
         pass
 
     # Exit a parse tree produced by wizardParser#PlusMinus.
-    def exitPlusMinus(self, ctx:wizardParser.PlusMinusContext):
+    def exitPlusMinus(self, ctx: wizardParser.PlusMinusContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Not.
-    def enterNot(self, ctx:wizardParser.NotContext):
+    def enterNot(self, ctx: wizardParser.NotContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Not.
-    def exitNot(self, ctx:wizardParser.NotContext):
+    def exitNot(self, ctx: wizardParser.NotContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Lesser.
-    def enterLesser(self, ctx:wizardParser.LesserContext):
+    def enterLesser(self, ctx: wizardParser.LesserContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Lesser.
-    def exitLesser(self, ctx:wizardParser.LesserContext):
+    def exitLesser(self, ctx: wizardParser.LesserContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Negative.
-    def enterNegative(self, ctx:wizardParser.NegativeContext):
+    def enterNegative(self, ctx: wizardParser.NegativeContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Negative.
-    def exitNegative(self, ctx:wizardParser.NegativeContext):
+    def exitNegative(self, ctx: wizardParser.NegativeContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Equal.
-    def enterEqual(self, ctx:wizardParser.EqualContext):
+    def enterEqual(self, ctx: wizardParser.EqualContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Equal.
-    def exitEqual(self, ctx:wizardParser.EqualContext):
+    def exitEqual(self, ctx: wizardParser.EqualContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#And.
-    def enterAnd(self, ctx:wizardParser.AndContext):
+    def enterAnd(self, ctx: wizardParser.AndContext):
         pass
 
     # Exit a parse tree produced by wizardParser#And.
-    def exitAnd(self, ctx:wizardParser.AndContext):
+    def exitAnd(self, ctx: wizardParser.AndContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Slice.
-    def enterSlice(self, ctx:wizardParser.SliceContext):
+    def enterSlice(self, ctx: wizardParser.SliceContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Slice.
-    def exitSlice(self, ctx:wizardParser.SliceContext):
+    def exitSlice(self, ctx: wizardParser.SliceContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Value.
-    def enterValue(self, ctx:wizardParser.ValueContext):
+    def enterValue(self, ctx: wizardParser.ValueContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Value.
-    def exitValue(self, ctx:wizardParser.ValueContext):
+    def exitValue(self, ctx: wizardParser.ValueContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#Greater.
-    def enterGreater(self, ctx:wizardParser.GreaterContext):
+    def enterGreater(self, ctx: wizardParser.GreaterContext):
         pass
 
     # Exit a parse tree produced by wizardParser#Greater.
-    def exitGreater(self, ctx:wizardParser.GreaterContext):
+    def exitGreater(self, ctx: wizardParser.GreaterContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#FunctionCall.
-    def enterFunctionCall(self, ctx:wizardParser.FunctionCallContext):
+    def enterFunctionCall(self, ctx: wizardParser.FunctionCallContext):
         pass
 
     # Exit a parse tree produced by wizardParser#FunctionCall.
-    def exitFunctionCall(self, ctx:wizardParser.FunctionCallContext):
+    def exitFunctionCall(self, ctx: wizardParser.FunctionCallContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#PostIncrement.
-    def enterPostIncrement(self, ctx:wizardParser.PostIncrementContext):
+    def enterPostIncrement(self, ctx: wizardParser.PostIncrementContext):
         pass
 
     # Exit a parse tree produced by wizardParser#PostIncrement.
-    def exitPostIncrement(self, ctx:wizardParser.PostIncrementContext):
+    def exitPostIncrement(self, ctx: wizardParser.PostIncrementContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#ParenExpr.
-    def enterParenExpr(self, ctx:wizardParser.ParenExprContext):
+    def enterParenExpr(self, ctx: wizardParser.ParenExprContext):
         pass
 
     # Exit a parse tree produced by wizardParser#ParenExpr.
-    def exitParenExpr(self, ctx:wizardParser.ParenExprContext):
+    def exitParenExpr(self, ctx: wizardParser.ParenExprContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#PreDecrement.
-    def enterPreDecrement(self, ctx:wizardParser.PreDecrementContext):
+    def enterPreDecrement(self, ctx: wizardParser.PreDecrementContext):
         pass
 
     # Exit a parse tree produced by wizardParser#PreDecrement.
-    def exitPreDecrement(self, ctx:wizardParser.PreDecrementContext):
+    def exitPreDecrement(self, ctx: wizardParser.PreDecrementContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#constant.
-    def enterConstant(self, ctx:wizardParser.ConstantContext):
+    def enterConstant(self, ctx: wizardParser.ConstantContext):
         pass
 
     # Exit a parse tree produced by wizardParser#constant.
-    def exitConstant(self, ctx:wizardParser.ConstantContext):
+    def exitConstant(self, ctx: wizardParser.ConstantContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#integer.
-    def enterInteger(self, ctx:wizardParser.IntegerContext):
+    def enterInteger(self, ctx: wizardParser.IntegerContext):
         pass
 
     # Exit a parse tree produced by wizardParser#integer.
-    def exitInteger(self, ctx:wizardParser.IntegerContext):
+    def exitInteger(self, ctx: wizardParser.IntegerContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#decimal.
-    def enterDecimal(self, ctx:wizardParser.DecimalContext):
+    def enterDecimal(self, ctx: wizardParser.DecimalContext):
         pass
 
     # Exit a parse tree produced by wizardParser#decimal.
-    def exitDecimal(self, ctx:wizardParser.DecimalContext):
+    def exitDecimal(self, ctx: wizardParser.DecimalContext):
         pass
 
-
     # Enter a parse tree produced by wizardParser#string.
-    def enterString(self, ctx:wizardParser.StringContext):
+    def enterString(self, ctx: wizardParser.StringContext):
         pass
 
     # Exit a parse tree produced by wizardParser#string.
-    def exitString(self, ctx:wizardParser.StringContext):
+    def exitString(self, ctx: wizardParser.StringContext):
         pass
 
 
-
-del wizardParser
+del wizardParser
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/antlr4/wizardVisitor.py` & `bain_wizard_interpreter-1.0.4/src/wizard/antlr4/wizardVisitor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,288 +1,234 @@
-# Generated from ./vendor/wizparse/wizards/wizard.g4 by ANTLR 4.10.1
+# Generated from ./vendor/wizparse/wizards/wizard.g4 by ANTLR 4.13.1
 from antlr4 import *
-if __name__ is not None and "." in __name__:
+
+if "." in __name__:
     from .wizardParser import wizardParser
 else:
     from wizardParser import wizardParser
 
 # This class defines a complete generic visitor for a parse tree produced by wizardParser.
 
-class wizardVisitor(ParseTreeVisitor):
 
+class wizardVisitor(ParseTreeVisitor):
     # Visit a parse tree produced by wizardParser#parseWizard.
-    def visitParseWizard(self, ctx:wizardParser.ParseWizardContext):
+    def visitParseWizard(self, ctx: wizardParser.ParseWizardContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#body.
-    def visitBody(self, ctx:wizardParser.BodyContext):
+    def visitBody(self, ctx: wizardParser.BodyContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#stmt.
-    def visitStmt(self, ctx:wizardParser.StmtContext):
+    def visitStmt(self, ctx: wizardParser.StmtContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#assignment.
-    def visitAssignment(self, ctx:wizardParser.AssignmentContext):
+    def visitAssignment(self, ctx: wizardParser.AssignmentContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#compoundAssignment.
-    def visitCompoundAssignment(self, ctx:wizardParser.CompoundAssignmentContext):
+    def visitCompoundAssignment(self, ctx: wizardParser.CompoundAssignmentContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Break.
-    def visitBreak(self, ctx:wizardParser.BreakContext):
+    def visitBreak(self, ctx: wizardParser.BreakContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Cancel.
-    def visitCancel(self, ctx:wizardParser.CancelContext):
+    def visitCancel(self, ctx: wizardParser.CancelContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Continue.
-    def visitContinue(self, ctx:wizardParser.ContinueContext):
+    def visitContinue(self, ctx: wizardParser.ContinueContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#For.
-    def visitFor(self, ctx:wizardParser.ForContext):
+    def visitFor(self, ctx: wizardParser.ForContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#If.
-    def visitIf(self, ctx:wizardParser.IfContext):
+    def visitIf(self, ctx: wizardParser.IfContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Return.
-    def visitReturn(self, ctx:wizardParser.ReturnContext):
+    def visitReturn(self, ctx: wizardParser.ReturnContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Select.
-    def visitSelect(self, ctx:wizardParser.SelectContext):
+    def visitSelect(self, ctx: wizardParser.SelectContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#While.
-    def visitWhile(self, ctx:wizardParser.WhileContext):
+    def visitWhile(self, ctx: wizardParser.WhileContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#cancelStmt.
-    def visitCancelStmt(self, ctx:wizardParser.CancelStmtContext):
+    def visitCancelStmt(self, ctx: wizardParser.CancelStmtContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#caseStmt.
-    def visitCaseStmt(self, ctx:wizardParser.CaseStmtContext):
+    def visitCaseStmt(self, ctx: wizardParser.CaseStmtContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#defaultStmt.
-    def visitDefaultStmt(self, ctx:wizardParser.DefaultStmtContext):
+    def visitDefaultStmt(self, ctx: wizardParser.DefaultStmtContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#elifStmt.
-    def visitElifStmt(self, ctx:wizardParser.ElifStmtContext):
+    def visitElifStmt(self, ctx: wizardParser.ElifStmtContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#elseStmt.
-    def visitElseStmt(self, ctx:wizardParser.ElseStmtContext):
+    def visitElseStmt(self, ctx: wizardParser.ElseStmtContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#forStmt.
-    def visitForStmt(self, ctx:wizardParser.ForStmtContext):
+    def visitForStmt(self, ctx: wizardParser.ForStmtContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#forRangeHeader.
-    def visitForRangeHeader(self, ctx:wizardParser.ForRangeHeaderContext):
+    def visitForRangeHeader(self, ctx: wizardParser.ForRangeHeaderContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#forInHeader.
-    def visitForInHeader(self, ctx:wizardParser.ForInHeaderContext):
+    def visitForInHeader(self, ctx: wizardParser.ForInHeaderContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#ifStmt.
-    def visitIfStmt(self, ctx:wizardParser.IfStmtContext):
+    def visitIfStmt(self, ctx: wizardParser.IfStmtContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#selectStmt.
-    def visitSelectStmt(self, ctx:wizardParser.SelectStmtContext):
+    def visitSelectStmt(self, ctx: wizardParser.SelectStmtContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#selectCaseList.
-    def visitSelectCaseList(self, ctx:wizardParser.SelectCaseListContext):
+    def visitSelectCaseList(self, ctx: wizardParser.SelectCaseListContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#optionTuple.
-    def visitOptionTuple(self, ctx:wizardParser.OptionTupleContext):
+    def visitOptionTuple(self, ctx: wizardParser.OptionTupleContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#selectOne.
-    def visitSelectOne(self, ctx:wizardParser.SelectOneContext):
+    def visitSelectOne(self, ctx: wizardParser.SelectOneContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#selectMany.
-    def visitSelectMany(self, ctx:wizardParser.SelectManyContext):
+    def visitSelectMany(self, ctx: wizardParser.SelectManyContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#whileStmt.
-    def visitWhileStmt(self, ctx:wizardParser.WhileStmtContext):
+    def visitWhileStmt(self, ctx: wizardParser.WhileStmtContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#argList.
-    def visitArgList(self, ctx:wizardParser.ArgListContext):
+    def visitArgList(self, ctx: wizardParser.ArgListContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#keywordStmt.
-    def visitKeywordStmt(self, ctx:wizardParser.KeywordStmtContext):
+    def visitKeywordStmt(self, ctx: wizardParser.KeywordStmtContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#PreIncrement.
-    def visitPreIncrement(self, ctx:wizardParser.PreIncrementContext):
+    def visitPreIncrement(self, ctx: wizardParser.PreIncrementContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#DotFunctionCall.
-    def visitDotFunctionCall(self, ctx:wizardParser.DotFunctionCallContext):
+    def visitDotFunctionCall(self, ctx: wizardParser.DotFunctionCallContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Or.
-    def visitOr(self, ctx:wizardParser.OrContext):
+    def visitOr(self, ctx: wizardParser.OrContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#In.
-    def visitIn(self, ctx:wizardParser.InContext):
+    def visitIn(self, ctx: wizardParser.InContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#PostDecrement.
-    def visitPostDecrement(self, ctx:wizardParser.PostDecrementContext):
+    def visitPostDecrement(self, ctx: wizardParser.PostDecrementContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#TimesDivideModulo.
-    def visitTimesDivideModulo(self, ctx:wizardParser.TimesDivideModuloContext):
+    def visitTimesDivideModulo(self, ctx: wizardParser.TimesDivideModuloContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Index.
-    def visitIndex(self, ctx:wizardParser.IndexContext):
+    def visitIndex(self, ctx: wizardParser.IndexContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Exponentiation.
-    def visitExponentiation(self, ctx:wizardParser.ExponentiationContext):
+    def visitExponentiation(self, ctx: wizardParser.ExponentiationContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#PlusMinus.
-    def visitPlusMinus(self, ctx:wizardParser.PlusMinusContext):
+    def visitPlusMinus(self, ctx: wizardParser.PlusMinusContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Not.
-    def visitNot(self, ctx:wizardParser.NotContext):
+    def visitNot(self, ctx: wizardParser.NotContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Lesser.
-    def visitLesser(self, ctx:wizardParser.LesserContext):
+    def visitLesser(self, ctx: wizardParser.LesserContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Negative.
-    def visitNegative(self, ctx:wizardParser.NegativeContext):
+    def visitNegative(self, ctx: wizardParser.NegativeContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Equal.
-    def visitEqual(self, ctx:wizardParser.EqualContext):
+    def visitEqual(self, ctx: wizardParser.EqualContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#And.
-    def visitAnd(self, ctx:wizardParser.AndContext):
+    def visitAnd(self, ctx: wizardParser.AndContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Slice.
-    def visitSlice(self, ctx:wizardParser.SliceContext):
+    def visitSlice(self, ctx: wizardParser.SliceContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Value.
-    def visitValue(self, ctx:wizardParser.ValueContext):
+    def visitValue(self, ctx: wizardParser.ValueContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#Greater.
-    def visitGreater(self, ctx:wizardParser.GreaterContext):
+    def visitGreater(self, ctx: wizardParser.GreaterContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#FunctionCall.
-    def visitFunctionCall(self, ctx:wizardParser.FunctionCallContext):
+    def visitFunctionCall(self, ctx: wizardParser.FunctionCallContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#PostIncrement.
-    def visitPostIncrement(self, ctx:wizardParser.PostIncrementContext):
+    def visitPostIncrement(self, ctx: wizardParser.PostIncrementContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#ParenExpr.
-    def visitParenExpr(self, ctx:wizardParser.ParenExprContext):
+    def visitParenExpr(self, ctx: wizardParser.ParenExprContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#PreDecrement.
-    def visitPreDecrement(self, ctx:wizardParser.PreDecrementContext):
+    def visitPreDecrement(self, ctx: wizardParser.PreDecrementContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#constant.
-    def visitConstant(self, ctx:wizardParser.ConstantContext):
+    def visitConstant(self, ctx: wizardParser.ConstantContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#integer.
-    def visitInteger(self, ctx:wizardParser.IntegerContext):
+    def visitInteger(self, ctx: wizardParser.IntegerContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#decimal.
-    def visitDecimal(self, ctx:wizardParser.DecimalContext):
+    def visitDecimal(self, ctx: wizardParser.DecimalContext):
         return self.visitChildren(ctx)
 
-
     # Visit a parse tree produced by wizardParser#string.
-    def visitString(self, ctx:wizardParser.StringContext):
+    def visitString(self, ctx: wizardParser.StringContext):
         return self.visitChildren(ctx)
 
 
-
-del wizardParser
+del wizardParser
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/contexts/contexts.py` & `bain_wizard_interpreter-1.0.4/src/wizard/contexts/contexts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,17 @@
-# -*- encoding: utf-8 -*-
-
 """
 This file contains "context" which are used to rewind the
 interpreter.
 """
 
+from __future__ import annotations
+
 from abc import abstractmethod
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Generic,
-    List,
-    Optional,
-    Sequence,
-    Tuple,
-    TypeVar,
-    Union,
-)
+from collections.abc import Sequence
+from typing import TYPE_CHECKING, Any, Callable, Generic, Self, TypeVar
 
 from antlr4 import ParserRuleContext
 
 from ..antlr4.wizardParser import wizardParser
 from ..errors import WizardError, WizardNameError, WizardParseError, WizardTypeError
 from ..manager import SelectOption
 from ..severity import Issue
@@ -33,39 +23,38 @@
     from .factory import WizardInterpreterContextFactory
 
 
 RuleContext = TypeVar("RuleContext", bound=ParserRuleContext)
 
 
 class WizardInterpreterContext(Generic[ContextState, RuleContext]):
-
     """
     The base context class. The context are represented by a tree, where each
     child has access to his parent. Unlike ANTLR4 context, not all rules or
     elements in the grammer creates a context.
     """
 
     # The interpreter:
-    _factory: "WizardInterpreterContextFactory"
+    _factory: WizardInterpreterContextFactory[ContextState]
 
     # The ANTLR4 context:
     _context: RuleContext
 
     # The parent context:
-    _parent: "WizardInterpreterContext"
+    _parent: WizardInterpreterContext[ContextState, Any]
 
     # The state of this context:
     _state: ContextState
 
     def __init__(
         self,
-        factory: "WizardInterpreterContextFactory",
+        factory: WizardInterpreterContextFactory[ContextState],
         context: RuleContext,
-        parent: "WizardInterpreterContext[ContextState, Any]",
-        state: Optional[ContextState] = None,
+        parent: WizardInterpreterContext[ContextState, Any],
+        state: ContextState | None = None,
     ):
         """
         Args:
             factory: The context factory.
             context: The ANTLR4 context.
             parent: The parent context.
             state: The state for this context. If None, a copy of the
@@ -76,24 +65,31 @@
         self._parent = parent
 
         if state is None:
             self._state = parent.state.copy()  # type: ignore
         else:
             self._state = state
 
+    def is_top_level(self) -> bool:
+        """
+        Returns:
+            True if this context is top-level (no parent), False otherwise.
+        """
+        return self is self.parent
+
     @property
-    def factory(self) -> "WizardInterpreterContextFactory":
+    def factory(self) -> WizardInterpreterContextFactory[ContextState]:
         """
         Returns:
             The factory associated with this context.
         """
         return self._factory
 
     @property
-    def parent(self) -> "WizardInterpreterContext":
+    def parent(self) -> WizardInterpreterContext[ContextState, Any]:
         """
         Returns:
             The parent context.
         """
         return self._parent
 
     @property
@@ -109,91 +105,88 @@
         """
         Returns:
             The state before the execution of this context.
         """
         return self._state
 
     @abstractmethod
-    def exec_(self) -> "WizardInterpreterContext":
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
         """
         Execute the next 'step' of this context and returns the next context
         to execute. When done, should return the parent context.
 
         This method should be implement by all sub-classes representing specific
         contexts.
         """
         pass
 
-    def exec(self) -> "WizardInterpreterContext":
+    def exec(self) -> WizardInterpreterContext[ContextState, Any]:
         """
         Execute the next 'step' of this context and returns the next context
         to execute. When done, should return the parent context.
         """
         if self.context.exception:
             raise WizardParseError(self.context, self.context.exception)
         return wrap_exceptions(self.exec_, self.context)
 
 
-class WizardBreakableContext:
-
+class WizardBreakableContext(Generic[ContextState]):
     """
     Context that can be broken by a 'Break' expression.
     """
 
     @abstractmethod
-    def break_(self) -> WizardInterpreterContext:
+    def break_(self) -> WizardInterpreterContext[ContextState, Any]:
         """
         Called when a 'Break' instruction is encountered, should usually return
         the parent.
 
         Returns:
             The next context to use after this break.
         """
         pass
 
 
-class WizardContinuableContext:
-
+class WizardContinuableContext(Generic[ContextState]):
     """
     Context that can be broken by a 'Continue' expression.
     """
 
     @abstractmethod
-    def continue_(self) -> WizardInterpreterContext:
+    def continue_(self) -> WizardInterpreterContext[ContextState, Any]:
         """
         Called when a 'Continue' instruction is encountered, should usually return
         the context itself.
 
         Returns:
             The next context to use after this continue.
         """
         pass
 
 
 class WizardTerminationContext(
     WizardInterpreterContext[ContextState, wizardParser.ParseWizardContext]
 ):
-
     """
     Special context returned at the end of the execution. You can check what caused
     the termination using the `is_cancel`, `is_return` and `is_complete` method. If you
     want to check for "normal" completion, you can check for `not is_return()`.
     """
 
-    def exec_(self) -> WizardInterpreterContext:
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
         raise NotImplementedError("exec() should not be called on termination context.")
 
     def is_cancel(self) -> bool:
         """
         Returns:
             True if this termination was caused by a 'Cancel' keyword.
         """
         return isinstance(self.parent, WizardCancelContext)
 
-    def message(self) -> Optional[str]:
+    def message(self) -> str | None:
         """
         Returns:
             The cancel message, if any. If `is_cancel()` is False, this returns None.
         """
         if not isinstance(self.parent, WizardCancelContext):
             return None
         return self.parent.message()
@@ -212,112 +205,120 @@
         """
         return not isinstance(self.parent, (WizardCancelContext, WizardReturnContext))
 
 
 class WizardTopLevelContext(
     WizardInterpreterContext[ContextState, wizardParser.ParseWizardContext]
 ):
-
     """
     Special context to be the entry context point.
     """
 
     def __init__(
         self,
-        factory: "WizardInterpreterContextFactory",
+        factory: WizardInterpreterContextFactory[ContextState],
         context: wizardParser.ParseWizardContext,
-        state: ContextState,
-        parent: Optional[WizardInterpreterContext] = None,
+        parent: WizardInterpreterContext[ContextState, Any] | None,
+        state: ContextState | None = None,
     ):
         """
         Args:
             factory: The factory used to create this context and future contexts.
             context: The ANTLR4 context.
             state: The starting state for this context.
             parent: If not None, it means that this context was created from an Exec()
                 expression and the parent should be the enclosing body.
         """
         super().__init__(factory, context, self if parent is None else parent, state)
 
-    def exec_(self) -> WizardInterpreterContext:
+    def exec_(self) -> WizardBodyContext[ContextState]:
         # We forward the parent, which is either self (no parent) or the parent body
         # for Exec().
         return self._factory.make_body_context(self.context.body(), self.parent)
 
 
 class WizardCancelContext(
-    WizardInterpreterContext[ContextState, wizardParser.CancelContext]
+    WizardInterpreterContext[ContextState, wizardParser.CancelStmtContext]
 ):
-
     """
     Special context that is returned when a 'Cancel' instruction is encountered.
     """
 
     # The cancel message:
-    _message: Optional[str]
+    _message: str | None
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(
+        self,
+        factory: WizardInterpreterContextFactory[ContextState],
+        context: wizardParser.CancelStmtContext,
+        parent: WizardInterpreterContext[ContextState, Any],
+        state: ContextState | None = None,
+    ):
+        super().__init__(factory, context, parent, state)
 
         self._message = None
         if self.context.expr():
             self._message = self._factory.evisitor.visitExpr(
                 self.context.expr(), self.state, str
             ).value
 
-    def message(self) -> Optional[str]:
+    def message(self) -> str | None:
         """
         Returns:
             The cancel message, if any.
         """
         return self._message
 
-    def exec_(self) -> WizardInterpreterContext:
+    def exec_(self) -> WizardTerminationContext[ContextState]:
         return self._factory.make_termination_context(self)
 
 
 class WizardReturnContext(
     WizardInterpreterContext[ContextState, wizardParser.ReturnContext]
 ):
-
     """
     Special context that is returned when a 'Return' instruction is encountered.
     """
 
-    def exec_(self) -> WizardInterpreterContext:
+    def exec_(self) -> WizardTerminationContext[ContextState]:
         return self._factory.make_termination_context(self)
 
 
 class WizardBodyContext(
     WizardInterpreterContext[ContextState, wizardParser.BodyContext]
 ):
-
     """
     Body context.
     """
 
     # Index of the next child to process.
     _ichild: int
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._ichild = 0
+    def __init__(
+        self,
+        factory: WizardInterpreterContextFactory[ContextState],
+        context: wizardParser.BodyContext,
+        parent: WizardInterpreterContext[ContextState, Any],
+        state: ContextState | None = None,
+    ):
+        super().__init__(factory, context, parent, state)
 
-    def exec_(self) -> WizardInterpreterContext:
+        self._ichild = 0
 
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
         # Empty block or no more children:
         if not self._context.children or self._ichild == len(self._context.children):
             if isinstance(self._parent, WizardTopLevelContext):
                 return self._factory.make_termination_context(self)
-            return self._factory._copy_parent(self)
+            return self._factory.copy_parent(self)
 
         child = self._context.children[self._ichild]
 
         # Copy the body and increment the child counter:
-        body = self._factory._copy_context(self)
+        body = self._factory.copy_context(self)
         body._ichild += 1
 
         # Expression - Standard context:
         if isinstance(child, wizardParser.ExprContext):
             # Specific handling of exec()
             if (
                 isinstance(child, wizardParser.FunctionCallContext)
@@ -339,17 +340,18 @@
                 return self._make_control_flow_context(child.controlFlowStmt(), body)
             elif child.keywordStmt():
                 return self._factory.make_keyword_context(child.keywordStmt(), body)
 
         raise WizardParseError(child, f"Unknown context in body: {child}.")
 
     def _make_control_flow_context(
-        self, ctx: wizardParser.ControlFlowStmtContext, parent: "WizardBodyContext"
-    ) -> WizardInterpreterContext:
-
+        self,
+        ctx: wizardParser.ControlFlowStmtContext,
+        parent: WizardBodyContext[ContextState],
+    ) -> WizardInterpreterContext[ContextState, Any]:
         if isinstance(ctx, wizardParser.ForContext):
             return self._factory.make_for_loop_context(ctx.forStmt(), parent)
         elif isinstance(ctx, wizardParser.WhileContext):
             return self._factory.make_while_loop_context(ctx.whileStmt(), parent)
         elif isinstance(ctx, wizardParser.IfContext):
             return self._factory.make_if_context(ctx.ifStmt(), parent)
         elif isinstance(ctx, wizardParser.SelectContext):
@@ -365,84 +367,83 @@
 
         raise WizardParseError(ctx, f"Unknown control flow statement: {ctx}.")
 
 
 class WizardBreakContext(
     WizardInterpreterContext[ContextState, wizardParser.BreakContext]
 ):
-    def exec_(self) -> WizardInterpreterContext:
-
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
         # Find the first loop or case:
-        loop_or_case: Optional[WizardInterpreterContext] = self
+        loop_or_case: WizardInterpreterContext[ContextState, Any] = self
 
-        while loop_or_case is not None and not isinstance(
+        while not loop_or_case.is_top_level() and not isinstance(
             loop_or_case, WizardBreakableContext
         ):
             loop_or_case = loop_or_case.parent
 
-        if loop_or_case is None:
+        if not isinstance(loop_or_case, WizardBreakableContext):
             raise WizardParseError(
                 self.context, "Invalid 'Break' statement encountered."
             )
 
-        return self._factory._copy_context(loop_or_case.break_(), self.state)
+        context: WizardInterpreterContext[ContextState, Any] = loop_or_case.break_()
+        return self._factory.copy_context(context, self.state)
 
 
 class WizardContinueContext(
     WizardInterpreterContext[ContextState, wizardParser.ContinueContext]
 ):
-    def exec_(self) -> WizardInterpreterContext:
-
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
         # Find the first parent loop:
-        loop: Optional[WizardInterpreterContext] = self
+        loop: WizardInterpreterContext[ContextState, Any] = self
 
-        while loop is not None and not isinstance(loop, WizardContinuableContext):
+        while loop.is_top_level() and not isinstance(loop, WizardContinuableContext):
             loop = loop.parent
 
-        if loop is None:
+        if not isinstance(loop, WizardContinuableContext):
             raise WizardParseError(
                 self.context, "Invalid 'Continue' statement encountered."
             )
 
-        return self._factory._copy_context(loop.continue_(), self.state)
+        context: WizardInterpreterContext[ContextState, Any] = loop.continue_()
+        return self._factory.copy_context(context, self.state)
 
 
 class WizardExecContext(
     WizardInterpreterContext[ContextState, wizardParser.FunctionCallContext]
 ):
-    def exec_(self) -> WizardInterpreterContext:
-        # Import here otherwise we have circular imports:
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
+        # import here otherwise we have circular imports
         from ..utils import make_parse_wizard_context
 
         state = self.state.copy()
 
         # Parse the expression:
-        args: List[wizardParser.ExprContext] = list(self.context.argList().expr())
+        args = list(self.context.argList().expr())
         if len(args) != 1:
             raise WizardTypeError(
                 self.context, f"Exec() expect exactly one argument, found {len(args)}."
             )
         script = self._factory.evisitor.visitExpr(args[0], state, str).value
 
         try:
             context = make_parse_wizard_context(script)
         except WizardError as we:
             # If an error occurs, the WizardError does not have a context, set it:
-            we._ctx = self.context
+            we._ctx = self.context  # type: ignore
             raise we
 
-        return WizardTopLevelContext(self._factory, context, state, self.parent)
+        return WizardTopLevelContext(self._factory, context, self.parent, state)
 
 
 class WizardIfContext(
     WizardInterpreterContext[ContextState, wizardParser.IfStmtContext]
 ):
-    def exec_(self) -> WizardInterpreterContext:
-
-        parent = self._factory._copy_parent(self)
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
+        parent = self._factory.copy_parent(self)
 
         if self._factory.evisitor.visitExpr(self.context.expr(), parent.state):
             return self._factory.make_body_context(self.context.body(), parent)
         else:
             for eifc in self.context.elifStmt():
                 if self._factory.evisitor.visitExpr(eifc.expr(), parent.state):
                     return self._factory.make_body_context(eifc.body(), parent)
@@ -454,161 +455,162 @@
                 )
 
         return parent
 
 
 class WizardForLoopContext(
     WizardInterpreterContext[ContextState, wizardParser.ForStmtContext],
-    WizardBreakableContext,
-    WizardContinuableContext,
+    WizardBreakableContext[ContextState],
+    WizardContinuableContext[ContextState],
 ):
-
     """
     For-loop context.
     """
 
     # Name of the loop variable, sequence of values and current index:
     _name: str
-    _values: Sequence[Value]
+    _values: Sequence[Value[Any]]
     _index: int
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(
+        self,
+        factory: WizardInterpreterContextFactory[ContextState],
+        context: wizardParser.ForStmtContext,
+        parent: WizardInterpreterContext[ContextState, Any],
+        state: ContextState | None = None,
+    ):
+        super().__init__(factory, context, parent, state)
 
         if self.context.forInHeader():
             self._values = self._for_in_header(self.context.forInHeader())
         else:
             self._values = self._for_range_header(self.context.forRangeHeader())
 
         self._name = self.context.Identifier().getText()
         self._index = 0
 
-    def break_(self) -> WizardInterpreterContext:
-        return self._factory._copy_parent(self)
+    def break_(self) -> WizardInterpreterContext[ContextState, Any]:
+        return self._factory.copy_parent(self)
 
-    def continue_(self) -> WizardInterpreterContext:
+    def continue_(self) -> WizardInterpreterContext[ContextState, Any]:
         return self
 
     def _for_range_header(
         self, ctx: wizardParser.ForRangeHeaderContext
-    ) -> Sequence[Value]:
-
+    ) -> Sequence[Value[Any]]:
         sta: Value[int] = self._factory.evisitor.visitExpr(ctx.expr(0), self.state, int)
         end: Value[int] = self._factory.evisitor.visitExpr(ctx.expr(1), self.state, int)
 
-        if ctx.expr(2):
-            by = self._factory.evisitor.visitExpr(ctx.expr(2), self.state, int)
+        if e2 := ctx.expr(2):
+            by = self._factory.evisitor.visitExpr(e2, self.state, int)
         else:
             by = Value(1)
 
         return [Value(i) for i in range(sta.value, end.value + 1, by.value)]
 
-    def _for_in_header(self, ctx: wizardParser.ForInHeaderContext) -> Sequence[Value]:
-
+    def _for_in_header(
+        self, ctx: wizardParser.ForInHeaderContext
+    ) -> Sequence[Value[Any]]:
         value = self._factory.evisitor.visitExpr(ctx.expr(), self.state)
 
         if isinstance(value.value, SubPackage):
             return [Value(f) for f in value.value.files]
         elif isinstance(value.value, SubPackages):
             return [Value(sp) for sp in value.value]
         elif isinstance(value.value, str):
             # TODO: Allow?
             return [Value(s) for s in value.value]
         else:
             raise WizardTypeError(
                 ctx, f"Cannot iterable over value of type {value.type}."
             )
 
-    def exec_(self) -> WizardInterpreterContext:
-
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
         # End of the loop:
         if self._index == len(self._values):
-            return self._factory._copy_parent(self)
+            return self._factory.copy_parent(self)
 
         # Retrieve the next value and set it:
         value = self._values[self._index]
 
         # Copy the context:
-        loop = self._factory._copy_context(self)
+        loop = self._factory.copy_context(self)
         loop._index += 1
 
-        loop.state._variables[self._name] = value
+        loop.state.set(self._name, value)
 
         # Return a body context:
         return self._factory.make_body_context(self.context.body(), loop)
 
 
 class WizardWhileLoopContext(
     WizardInterpreterContext[ContextState, wizardParser.WhileStmtContext],
-    WizardBreakableContext,
-    WizardContinuableContext,
+    WizardBreakableContext[ContextState],
+    WizardContinuableContext[ContextState],
 ):
-    def break_(self) -> WizardInterpreterContext:
-        return self._factory._copy_parent(self)
+    def break_(self) -> WizardInterpreterContext[ContextState, Any]:
+        return self._factory.copy_parent(self)
 
-    def continue_(self) -> WizardInterpreterContext:
+    def continue_(self) -> WizardInterpreterContext[ContextState, Any]:
         return self
 
-    def exec_(self) -> WizardInterpreterContext:
-
-        loop = self._factory._copy_context(self)
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
+        loop = self._factory.copy_context(self)
 
         # If the expression evaluates to True, we return a body context:
         if self._factory.evisitor.visitExpr(self.context.expr(), loop.state):
             return self._factory.make_body_context(self.context.body(), loop)
 
         # Otherwise we return the parent (after updating the variables):
-        return self._factory._copy_parent(loop)
+        return self._factory.copy_parent(loop)
 
 
 class WizardAssignmentContext(
     WizardInterpreterContext[
         ContextState,
         wizardParser.AssignmentContext,
     ]
 ):
-    def exec_(self) -> WizardInterpreterContext:
-
-        parent = self._factory._copy_parent(self)
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
+        parent = self._factory.copy_parent(self)
 
         # Retrieve the name:
         name: str = self.context.Identifier().getText()
 
         # Evaluate the expression:
-        value: Value = self._factory.evisitor.visitExpr(
+        value: Value[Any] = self._factory.evisitor.visitExpr(
             self.context.expr(), parent.state
         )
 
-        parent.state._variables[name] = value
+        parent.state.set(name, value)
 
         return parent
 
 
 class WizardCompoundAssignmentContext(
     WizardInterpreterContext[
         ContextState,
         wizardParser.CompoundAssignmentContext,
     ]
 ):
-    def exec_(self) -> WizardInterpreterContext:
-
-        parent = self._factory._copy_parent(self)
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
+        parent = self._factory.copy_parent(self)
 
         # Retrieve the name:
         name: str = self.context.Identifier().getText()
 
         # Evaluate the expression:
-        value: Value = self._factory.evisitor.visitExpr(
+        value: Value[Any] = self._factory.evisitor.visitExpr(
             self.context.expr(), parent.state
         )
 
-        if name not in parent.state._variables:
-            raise WizardNameError(self.context.Identifier(), name)
+        if name not in parent.state.variables:
+            raise WizardNameError(self.context, name)
 
-        op: Callable[[Value, Value], Value]
+        op: Callable[[Value[Any], Value[Any]], Value[Any]]
         if self.context.CompoundExp():
             op = Value.__pow__
         elif self.context.CompoundMul():
             op = Value.__mul__
         elif self.context.CompoundDiv():
             op = Value.__div__
         elif self.context.CompoundMod():
@@ -619,34 +621,33 @@
             op = Value.__sub__
         else:
             raise WizardParseError(
                 self.context, f"Unknown compound operation: {self.context}."
             )
 
         try:
-            value = op(parent.state._variables[name], value)
+            value = op(parent.state.variables[name], value)
         except TypeError as te:
-            raise WizardTypeError(self.context, str(te))
+            raise WizardTypeError(self.context, str(te)) from te
 
-        parent.state._variables[name] = value
+        parent.state.set(name, value)
 
         return parent
 
 
 def parse_select_options(
-    factory: "WizardInterpreterContextFactory",
-    context: Union[wizardParser.SelectOneContext, wizardParser.SelectManyContext],
+    factory: WizardInterpreterContextFactory[ContextState],
+    context: wizardParser.SelectOneContext | wizardParser.SelectManyContext,
     state: ContextState,
-) -> Tuple[str, List[SelectOption], List[SelectOption]]:
-
+) -> tuple[str, list[SelectOption], list[SelectOption]]:
     # Parse the description and option:
     description = factory.evisitor.visitExpr(context.expr(), state, str).value
 
-    options: List[SelectOption] = []
-    defaults: List[SelectOption] = []
+    options: list[SelectOption] = []
+    defaults: list[SelectOption] = []
     for opt in context.optionTuple():
         a, b, c = (
             factory.evisitor.visitExpr(opt.expr(0), state, str),
             factory.evisitor.visitExpr(opt.expr(1), state, str),
             factory.evisitor.visitExpr(opt.expr(2), state, str),
         )
 
@@ -667,33 +668,41 @@
     # Not default in SelectOne -> Select first one.
     if not isinstance(context, wizardParser.SelectManyContext) and not defaults:
         defaults.append(options[0])
 
     return description, options, defaults
 
 
-class WizardSelectContext(WizardInterpreterContext[ContextState, RuleContext]):
+_SelectOneOrManyRuleContext = TypeVar(
+    "_SelectOneOrManyRuleContext",
+    wizardParser.SelectOneContext,
+    wizardParser.SelectManyContext,
+)
+
 
+class WizardSelectContext(
+    WizardInterpreterContext[ContextState, _SelectOneOrManyRuleContext]
+):
     # The description:
     _description: str
 
     # The list of options:
-    _options: List[SelectOption]
+    _options: list[SelectOption]
 
     # The default option(s):
-    _default: List[SelectOption]
+    _default: list[SelectOption]
 
     # The selected option(s):
-    _selected: List[SelectOption]
+    _selected: list[SelectOption]
 
     def __init__(
         self,
-        factory: "WizardInterpreterContextFactory",
-        context: Union[wizardParser.SelectOneContext, wizardParser.SelectManyContext],
-        parent: WizardInterpreterContext,
+        factory: WizardInterpreterContextFactory[ContextState],
+        context: _SelectOneOrManyRuleContext,
+        parent: WizardInterpreterContext[ContextState, Any],
     ):
         super().__init__(factory, context, parent)
 
         self._description, self._options, self._defaults = parse_select_options(
             factory, context, self.state
         )
 
@@ -704,50 +713,52 @@
         """
         Returns:
             The description for this select context.
         """
         return self._description
 
     @property
-    def options(self) -> List[SelectOption]:
+    def options(self) -> Sequence[SelectOption]:
         """
         Returns:
             The available options for this select context.
         """
         return self._options
 
-    def _select(self, options: List[SelectOption]) -> "WizardSelectContext":
+    def _select(self, options: Sequence[SelectOption]) -> Self:
         """
         Select the given options and return the object.
 
         Args:
             options: The options to select.
 
         Returns:
             A copy of the current object with the given options selected.
         """
-        copy = self._factory._copy_context(self)
-        copy._selected = options
+        copy = self._factory.copy_context(self)
+        copy._selected = list(options)
         return copy
 
-    def exec_(self) -> "WizardSelectCasesContext":
+    def exec_(
+        self,
+    ) -> WizardSelectCasesContext[ContextState, _SelectOneOrManyRuleContext]:
         # This completely delegates to the other context:
         return self._factory.make_select_cases_context(
             self._selected, self.context, self.parent
         )
 
 
 class WizardSelectOneContext(
     WizardSelectContext[ContextState, wizardParser.SelectOneContext]
 ):
     def __init__(
         self,
-        factory: "WizardInterpreterContextFactory",
+        factory: WizardInterpreterContextFactory[ContextState],
         context: wizardParser.SelectOneContext,
-        parent: WizardInterpreterContext,
+        parent: WizardInterpreterContext[ContextState, Any],
     ):
         super().__init__(factory, context, parent)
 
         # More than one default in SelectOne:
         if len(self._defaults) != 1:
             self._factory.severity.raise_or_warn(
                 Issue.MULTIPLE_DEFAULTS_IN_SELECT_ON,
@@ -767,142 +778,140 @@
     def default(self) -> SelectOption:
         """
         Returns:
             The default option for this select context.
         """
         return self._defaults[0]
 
-    def select(self, option: SelectOption) -> "WizardSelectOneContext":
+    def select(self, option: SelectOption) -> WizardSelectOneContext[ContextState]:
         """
         Select the given option and return the object.
 
         Args:
             option: The option to select.
 
         Returns:
             A copy of the current object with the given option selected.
         """
-        return self._select([option])  # type: ignore
+        return self._select([option])
 
 
 class WizardSelectManyContext(
-    WizardSelectContext[ContextState, wizardParser.SelectOneContext]
+    WizardSelectContext[ContextState, wizardParser.SelectManyContext]
 ):
     def __init__(
         self,
-        factory: "WizardInterpreterContextFactory",
+        factory: WizardInterpreterContextFactory[ContextState],
         context: wizardParser.SelectManyContext,
-        parent: WizardInterpreterContext,
+        parent: WizardInterpreterContext[ContextState, Any],
     ):
         super().__init__(factory, context, parent)
 
         # We select the defaults:
         self._selected = self._defaults
 
     @property
-    def defaults(self) -> List[SelectOption]:
+    def defaults(self) -> Sequence[SelectOption]:
         """
         Returns:
             The default options for this select context.
         """
         return self._defaults
 
-    def select(self, options: List[SelectOption]) -> "WizardSelectManyContext":
+    def select(
+        self, options: Sequence[SelectOption]
+    ) -> WizardSelectManyContext[ContextState]:
         """
         Select the given list of options and return the object.
 
         Args:
             options: The options to select.
 
         Returns:
             A copy of the current object with the given options selected.
         """
-        return self._select(options)  # type: ignore
+        return self._select(options)
 
 
 class WizardSelectCasesContext(
-    WizardInterpreterContext[ContextState, wizardParser.SelectStmtContext],
-    WizardBreakableContext,
+    WizardInterpreterContext[ContextState, _SelectOneOrManyRuleContext],
+    WizardBreakableContext[ContextState],
 ):
-
     # The list of selected options:
-    _options: List[SelectOption]
+    _options: list[SelectOption]
 
     # The list of cases, the current index, a boolean indicating if
     # the value has been found, and a boolean for fallthrough:
     _ismany: bool
-    _cases: List[wizardParser.CaseStmtContext]
-    _default: Optional[wizardParser.DefaultStmtContext]
+    _cases: list[wizardParser.CaseStmtContext]
+    _default: wizardParser.DefaultStmtContext | None
     _index: int
     _found: bool
     _fallthrough: bool
 
     def __init__(
         self,
-        factory: "WizardInterpreterContextFactory",
-        options: List[SelectOption],
-        context: Union[wizardParser.SelectOneContext, wizardParser.SelectManyContext],
-        parent: WizardInterpreterContext,
+        factory: WizardInterpreterContextFactory[ContextState],
+        options: Sequence[SelectOption],
+        context: _SelectOneOrManyRuleContext,
+        parent: WizardInterpreterContext[ContextState, Any],
     ):
         """
         Args:
             factory: The context factory.
             options: List of selected options.
             context: The select context.
             parent: The parent context.
         """
         super().__init__(factory, context, parent)
 
-        self._options = options
+        self._options = list(options)
 
         if isinstance(self.context, wizardParser.SelectOneContext):
             self._ismany = False
         else:
             self._ismany = True
 
         self._cases = list(context.selectCaseList().caseStmt())
         self._default = context.selectCaseList().defaultStmt()
 
         self._index = 0
         self._found = False
         self._fallthrough = False
 
-    def break_(self) -> WizardInterpreterContext:
+    def break_(self) -> WizardInterpreterContext[ContextState, Any]:
         # Disable fallthrough:
-        copy = self._factory._copy_context(self)
+        copy = self._factory.copy_context(self)
         copy._fallthrough = False
 
         # We return the context itself to keep evaluating cases:
         return copy
 
-    def exec_(self) -> WizardInterpreterContext:
-
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
         # Element found in a selectOne, returns to the parent:
         if self._found and not self._ismany and not self._fallthrough:
-            return self._factory._copy_parent(self)
+            return self._factory.copy_parent(self)
 
         # Copy the current context:
-        snext = self._factory._copy_context(self)
+        snext = self._factory.copy_context(self)
 
         # Cases remaining:
         if self._index < len(self._cases):
-
             # Find the next case:
             case = self._cases[self._index]
             snext._index += 1
 
             target: Value[str] = self._factory.evisitor.visitExpr(
                 case.expr(), snext.state, str
             )
 
             # Check if the case match or if we have a fallthrough:
             if self._fallthrough or any(
                 sopt.name == target.value for sopt in self._options
             ):
-
                 # We found the value, remember it:
                 snext._found = True
 
                 # Assume fallthrough, the break_() will set this off if a 'Break'
                 # statement is found:
                 snext._fallthrough = True
 
@@ -914,19 +923,18 @@
         # No cases remaining, default, and not found:
         elif self._default and (self._fallthrough or not self._found):
             snext._found = True
             return self._factory.make_case_context(self._default, snext)
 
         # No need to copy from snext since if we reach this return statement, nothing
         # has been updated in snext.
-        return self._factory._copy_parent(self)
+        return self._factory.copy_parent(self)
 
 
 class WizardCaseContext(
     WizardInterpreterContext[
-        ContextState,
-        Union[wizardParser.CaseStmtContext, wizardParser.DefaultStmtContext],
+        ContextState, wizardParser.CaseStmtContext | wizardParser.DefaultStmtContext
     ]
 ):
-    def exec_(self) -> WizardInterpreterContext:
+    def exec_(self) -> WizardBodyContext[ContextState]:
         # It's the select context job to check if this should be executed:
         return self._factory.make_body_context(self.context.body(), self.parent)
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/contexts/keywords.py` & `bain_wizard_interpreter-1.0.4/src/wizard/contexts/keywords.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,263 +1,259 @@
-# -*- encoding: utf-8 -*-
+from __future__ import annotations
 
-from abc import abstractproperty
-from typing import TYPE_CHECKING, Callable, List, Optional, Tuple
+from abc import abstractmethod
+from collections.abc import Sequence
+from typing import TYPE_CHECKING, Any, Generic, TypeVarTuple, cast
 
 from ..antlr4.wizardParser import wizardParser
 from ..errors import WizardNameError, WizardTypeError
 from ..severity import Issue
-from ..value import Value, VariableType
+from ..value import AnyValueType, VariableType
 from .contexts import ContextState, WizardInterpreterContext
 
 if TYPE_CHECKING:
     from .factory import WizardInterpreterContextFactory
 
 
+_Args = TypeVarTuple("_Args")
+
+
 class WizardKeywordContext(
     WizardInterpreterContext[ContextState, wizardParser.KeywordStmtContext]
-):
+): ...
+
 
+class _WizardKeywordContext(
+    WizardKeywordContext[ContextState],
+    Generic[ContextState, *_Args],
+):
     """
     Top-level class for keyword contexts.
     """
 
     @property
-    def _argtypes(self) -> List[type]:
+    def _argtypes(self) -> list[type]:
         return []
 
-    @abstractproperty
-    def _visitor(self) -> Callable[..., None]:
-        ...
+    @abstractmethod
+    def _visit(self, state: ContextState, *args: *_Args) -> None: ...
 
-    def _get_args(self, types: List[type]) -> List[Value]:
+    def _get_args(self, types: Sequence[type]) -> tuple[*_Args]:
         keyword = self.context.Keyword().getText()
         arglist = [
             self._factory.evisitor.visitExpr(ex, self.state)
             for ex in self.context.argList().expr()
         ]
-        if len(arglist) > len(types):
-            raise WizardTypeError(f"Keyword {keyword}: too many arguments.")
+
+        n_arg_none = sum(int(isinstance(None, t)) for t in types)
+        min_args = len(types) - n_arg_none
+        max_args = len(types)
+
+        if len(arglist) < min_args:
+            raise WizardTypeError(
+                self._context,
+                f"Keyword {keyword}: not enough arguments, expected {len(types)}.",
+            )
+        elif len(arglist) > max_args:
+            raise WizardTypeError(
+                self._context,
+                f"Keyword {keyword}: too many arguments, expected {len(types)}.",
+            )
         elif len(arglist) < len(types):
             raise WizardTypeError(
-                f"Keyword {keyword}: not enough arguments, expected {len(types)}."
+                self._context,
+                f"Keyword {keyword}: not enough arguments, expected {len(types)}.",
             )
 
-        for i, (a, t) in enumerate(zip(arglist, types)):
-            if not isinstance(a.value, t):
-                raise WizardTypeError(
-                    f"Keyword {keyword}: Argument at position {i + 1} has incorrect"
-                    f" type, expected {VariableType.from_pytype(t)}, got {a.type}."
-                )
-
-        return arglist
+        # extract value from arguments and pad with None to reach the exact number of
+        # arguments
+        args = tuple(arg.value for arg in arglist)
+        args += (None,) * (len(types) - len(args))
+
+        return cast(
+            "tuple[*_Args]",
+            tuple(arg.value for arg in arglist),
+        )
 
-    def exec_(self) -> WizardInterpreterContext:
+    def exec_(self) -> WizardInterpreterContext[ContextState, Any]:
         state = self.state.copy()
-        self._visitor(
-            self, state, *(arg.value for arg in self._get_args(self._argtypes))
-        )
-        return self._factory._copy_parent(self, state)
+        self._visit(state, *self._get_args(self._argtypes))
+        return self._factory.copy_parent(self, state)
 
 
-class WizardDeSelectAllContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitDeSelectAll
+class WizardDeSelectAllContext(_WizardKeywordContext[ContextState]):
+    def _visit(self, state: ContextState) -> None:
+        return self._factory.kvisitor.visitDeSelectAll(self, state)
 
 
-class WizardDeSelectAllPluginsContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitDeSelectAllPlugins
+class WizardDeSelectAllPluginsContext(_WizardKeywordContext[ContextState]):
+    def _visit(self, state: ContextState) -> None:
+        return self._factory.kvisitor.visitDeSelectAllPlugins(self, state)
 
 
-class WizardDeSelectPluginContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitDeSelectPlugin
+class WizardDeSelectPluginContext(_WizardKeywordContext[ContextState, str]):
+    def _visit(self, state: ContextState, plugin: str) -> None:
+        return self._factory.kvisitor.visitDeSelectPlugin(self, state, plugin)
 
     @property
     def _argtypes(self):
         return [str]
 
 
-class WizardDeSelectSubPackageContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitDeSelectSubPackage
+class WizardDeSelectSubPackageContext(_WizardKeywordContext[ContextState, str]):
+    def _visit(self, state: ContextState, package: str) -> None:
+        return self._factory.kvisitor.visitDeSelectSubPackage(self, state, package)
 
     @property
     def _argtypes(self):
         return [str]
 
 
-class WizardRenamePluginContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitRenamePlugin
+class WizardRenamePluginContext(_WizardKeywordContext[ContextState, str, str]):
+    def _visit(self, state: ContextState, name1: str, name2: str) -> None:
+        return self._factory.kvisitor.visitRenamePlugin(self, state, name1, name2)
 
     @property
     def _argtypes(self):
         return [str, str]
 
 
-class WizardResetPluginNameContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitResetPluginName
+class WizardResetPluginNameContext(_WizardKeywordContext[ContextState, str]):
+    def _visit(self, state: ContextState, plugin: str) -> None:
+        return self._factory.kvisitor.visitResetPluginName(self, state, plugin)
 
     @property
     def _argtypes(self):
         return [str]
 
 
-class WizardResetAllPluginNamesContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitResetAllPluginNames
+class WizardResetAllPluginNamesContext(_WizardKeywordContext[ContextState]):
+    def _visit(self, state: ContextState) -> None:
+        return self._factory.kvisitor.visitResetAllPluginNames(self, state)
 
 
-class WizardSelectAllContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitSelectAll
+class WizardSelectAllContext(_WizardKeywordContext[ContextState]):
+    def _visit(self, state: ContextState) -> None:
+        return self._factory.kvisitor.visitSelectAll(self, state)
 
 
-class WizardSelectAllPluginsContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitSelectAllPlugins
+class WizardSelectAllPluginsContext(_WizardKeywordContext[ContextState]):
+    def _visit(self, state: ContextState) -> None:
+        return self._factory.kvisitor.visitSelectAllPlugins(self, state)
 
 
-class WizardSelectPluginContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitSelectPlugin
+class WizardSelectPluginContext(_WizardKeywordContext[ContextState, str]):
+    def _visit(self, state: ContextState, plugin: str) -> None:
+        return self._factory.kvisitor.visitSelectPlugin(self, state, plugin)
 
     @property
     def _argtypes(self):
         return [str]
 
 
-class WizardSelectSubPackageContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitSelectSubPackage
+class WizardSelectSubPackageContext(_WizardKeywordContext[ContextState, str]):
+    def _visit(self, state: ContextState, subpackage: str) -> None:
+        return self._factory.kvisitor.visitSelectSubPackage(self, state, subpackage)
 
     @property
     def _argtypes(self):
         return [str]
 
 
-class WizardRequireVersionsContext(WizardKeywordContext[ContextState]):
-
+class WizardRequireVersionsContext(
+    _WizardKeywordContext[ContextState, str, str | None, str | None, str | None]
+):
     """
     The require versions context is a bit special since it probably requires
     user interaction which is why we parse the arguments inside constructor.
     """
 
-    _args: Tuple[str, Optional[str], Optional[str], Optional[str]]
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(
+        self,
+        factory: WizardInterpreterContextFactory[ContextState],
+        context: wizardParser.KeywordStmtContext,
+        parent: WizardInterpreterContext[ContextState, Any],
+        state: ContextState | None = None,
+    ):
+        super().__init__(factory, context, parent, state)
 
-        self._args = tuple(
-            arg.value if arg.value else None for arg in self._get_args(self._argtypes)
-        )
+        self._args = self._get_args(self._argtypes)
 
-    # These property are useful to use the interpreter:
+    # these property are useful to use the interpreter
     @property
     def game_version(self) -> str:
         return self._args[0]
 
     @property
-    def script_extender_version(self) -> Optional[str]:
+    def script_extender_version(self) -> str | None:
         return self._args[1]
 
     @property
-    def graphics_extender_version(self) -> Optional[str]:
+    def graphics_extender_version(self) -> str | None:
         return self._args[2]
 
     @property
-    def wrye_bash_version(self) -> Optional[str]:
+    def wrye_bash_version(self) -> str | None:
         return self._args[3]
 
-    # These two are not used at all but required for mypy or other tools
-    # since otherwise the class is abstract.
-
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitRequireVersions
+    def _get_args(
+        self, types: Sequence[type]
+    ) -> tuple[str, str | None, str | None, str | None]:
+        # weird stuff to please type checkers
+        gv, sew, gew, wbv = super()._get_args(types)
+        return (gv, sew or None, gew or None, wbv or None)
+
+    def _visit(
+        self,
+        state: ContextState,
+        game_version: str,
+        script_extender_version: str | None,
+        graphics_extender_version: str | None,
+        wrye_bash_version: str | None,
+    ) -> None:
+        return self._factory.kvisitor.visitRequireVersions(
+            state,
+            game_version=game_version,
+            script_extender_version=script_extender_version,
+            graphics_extender_version=graphics_extender_version,
+            wrye_bash_version=wrye_bash_version,
+        )
 
     @property
     def _argtypes(self):
-        return [str, str, str, str]
-
-    def _get_args(self, types: List[type]) -> List[Value]:
-        keyword = self.context.Keyword().getText()
-        arglist = [
-            self._factory.evisitor.visitExpr(ex, self.state)
-            for ex in self.context.argList().expr()
-        ]
-
-        if len(arglist) < 1:
-            raise WizardTypeError(
-                f"Keyword {keyword}: not enough arguments, expected between 1 and 4."
-            )
-
-        if len(arglist) > 4:
-            raise WizardTypeError(f"Keyword {keyword}: too many arguments.")
+        return [str, str | None, str | None, str | None]
 
-        if len(arglist) < 4:
-            arglist = arglist + [Value("")] * (4 - len(arglist))
 
-        for i, a in enumerate(arglist):
-            if not isinstance(a.value, str):
-                raise WizardTypeError(
-                    f"Keyword {keyword}: Argument at position {i + 1} has incorrect"
-                    f" type, expected {VariableType.from_pytype(str)}, got {a.type}."
-                )
+class WizardNoteContext(_WizardKeywordContext[ContextState, str]):
+    # note context is a bit special as it accepts any type but warn if the type is
+    # not str
 
-        return arglist
-
-    def exec_(self) -> WizardInterpreterContext:
-        state = self.state.copy()
-        self._visitor(state, *self._args)
-        return self._factory._copy_parent(self, state)
-
-
-class WizardNoteContext(WizardKeywordContext[ContextState]):
-    @property
-    def _visitor(self):
-        return self._factory.kvisitor.visitNote
-
-    @property
-    def _argtypes(self):
-        return [object]
-
-    def _get_args(self, types: List[type]):
-        args = super()._get_args(types)
-        if not isinstance(args[0].value, str):
+    def _visit(self, state: ContextState, note: AnyValueType) -> None:
+        if not isinstance(note, str):
+            type_ = VariableType.from_pytype(type(note))  # type: ignore
             self._factory.severity.raise_or_warn(
                 Issue.USAGE_OF_ANYTHING_IN_NOTE,
                 WizardTypeError(
                     self.context,
-                    f"'Note' keyword expected string, found {args[0].type}.",
+                    f"'Note' keyword expected string, found {type_}.",
                 ),
-                f"'Note' keyword expected string, found {args[0].type}.",
+                f"'Note' keyword expected string, found {type_}.",
             )
-        return [Value(str(args[0].value))]
+        return self._factory.kvisitor.visitNote(self, state, str(note))
+
+    @property
+    def _argtypes(self):
+        return [object]
 
 
 def make_keyword_context(
-    factory: "WizardInterpreterContextFactory",
+    factory: WizardInterpreterContextFactory[ContextState],
     context: wizardParser.KeywordStmtContext,
-    parent: WizardInterpreterContext,
-) -> WizardKeywordContext:
+    parent: WizardInterpreterContext[ContextState, Any],
+) -> WizardInterpreterContext[ContextState, wizardParser.KeywordStmtContext]:
     name: str = context.Keyword().getText()
     if name == "RequireVersions":
         return WizardRequireVersionsContext(factory, context, parent)
     if name in ["ResetAllPluginNames", "ResetAllEspmNames"]:
         return WizardResetAllPluginNamesContext(factory, context, parent)
     if name == "DeSelectSubPackage":
         return WizardDeSelectSubPackageContext(factory, context, parent)
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/contexts/utils.py` & `bain_wizard_interpreter-1.0.4/src/wizard/contexts/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-# -*- encoding: utf-8 -*-
-
-from typing import Callable, Optional, TypeVar
+from typing import Callable, TypeVar
 
 from antlr4 import ParserRuleContext
 from antlr4.error.Errors import InputMismatchException, ParseCancellationException
 
 from ..errors import WizardError, WizardIndexError, WizardParseError, WizardTypeError
 
 T = TypeVar("T")
 
 
-def wrap_exceptions(
-    fn: Callable[[], T], context: Optional[ParserRuleContext] = None
-) -> T:
+def wrap_exceptions(fn: Callable[[], T], context: ParserRuleContext | None = None) -> T:
     """
     Wrap the given call to `fn` in a proper try/except block to convert as many
     exceptions as possible to WizardError.
     """
 
     try:
         return fn()
@@ -25,13 +21,14 @@
         raise ex
     # Wrap parser exceptions:
     except ParseCancellationException as ex:
         # Try to find a context:
         if context is None and isinstance(ex.args[0], InputMismatchException):
             context = ex.args[0].ctx
 
-        raise WizardParseError(context, ex)
+        raise WizardParseError(context, ex) from ex
+
     # Wrap "known" exceptions:
     except TypeError as te:
-        raise WizardTypeError(context, te)
+        raise WizardTypeError(context, te) from te
     except IndexError as ie:
-        raise WizardIndexError(context, *ie.args)
+        raise WizardIndexError(context, *ie.args) from ie
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/errors.py` & `bain_wizard_interpreter-1.0.4/src/wizard/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# -*- encoding: utf-8 -*-
+from typing import cast
 
-from typing import Optional
-
-from antlr4 import Parser, ParserRuleContext, Token
+from antlr4 import Parser, ParserRuleContext, Token, TokenStream
 from antlr4.error.Errors import (
     FailedPredicateException,
     InputMismatchException,
     NoViableAltException,
     RecognitionException,
 )
 
@@ -15,79 +13,88 @@
     """
     Base class for all Wizard errors.
 
     The only case where there is no context associated is if the parser fails
     at the beginning.
     """
 
-    _ctx: ParserRuleContext
+    _ctx: ParserRuleContext | None
 
-    def __init__(self, context: ParserRuleContext, *args):
+    def __init__(self, context: ParserRuleContext | None, *args: object):
         super().__init__(*args)
         self._ctx = context
 
     @property
-    def context(self) -> Optional[ParserRuleContext]:
+    def context(self) -> ParserRuleContext | None:
         return self._ctx
 
     @property
     def line(self) -> int:
+        if not self._ctx:
+            return -1
         return self._ctx.start.line  # type: ignore
 
     @property
     def column(self) -> int:
+        if not self._ctx:
+            return -1
         return self._ctx.start.column  # type: ignore
 
     # The messageXXX are taken from ANTLR4 error strategy (reportXXX):
 
     def escapeWSAndQuote(self, s: str) -> str:
         s = s.replace("\n", "\\n")
         s = s.replace("\r", "\\r")
         s = s.replace("\t", "\\t")
         return "'" + s + "'"
 
-    def getTokenErrorDisplay(self, t: Token):
+    def getTokenErrorDisplay(self, t: Token | None):
         if t is None:
             return "<no token>"
-        s = t.text
+        s = cast(str | None, t.text)  # pyright: ignore[reportUnknownMemberType]
         if s is None:
             if t.type == Token.EOF:
                 s = "<EOF>"
             else:
                 s = "<" + str(t.type) + ">"
         return self.escapeWSAndQuote(s)
 
     def messageNoViableAlternative(
         self, recognizer: Parser, e: NoViableAltException
     ) -> str:
-        tokens = recognizer.getTokenStream()
+        tokens = cast(TokenStream | None, recognizer.getTokenStream())  # pyright: ignore[reportUnknownMemberType]
         if tokens is not None:
             if e.startToken.type == Token.EOF:
                 input = "<EOF>"
             else:
-                input = tokens.getText(e.startToken, e.offendingToken)
+                input = cast(str, tokens.getText(e.startToken, e.offendingToken))  # type: ignore
         else:
             input = "<unknown input>"
         return "no viable alternative at input " + self.escapeWSAndQuote(input)
 
     def messageInputMismatch(
         self, recognizer: Parser, e: InputMismatchException
     ) -> str:
-        msg: str = (
+        return (
             "mismatched input "
             + self.getTokenErrorDisplay(e.offendingToken)
             + " expecting "
-            + e.getExpectedTokens().toString(
-                recognizer.literalNames, recognizer.symbolicNames
+            + cast(
+                str,
+                e.getExpectedTokens().toString(  # type: ignore
+                    recognizer.literalNames,  # type: ignore
+                    recognizer.symbolicNames,  # type: ignore
+                ),
             )
         )
-        return msg
 
-    def messageFailedPredicate(self, recognizer, e) -> str:
-        ruleName = recognizer.ruleNames[recognizer._ctx.getRuleIndex()]
+    def messageFailedPredicate(
+        self, recognizer: Parser, e: FailedPredicateException
+    ) -> str:
+        ruleName: str = recognizer.ruleNames[recognizer._ctx.getRuleIndex()]  # type: ignore
         return f"rule {ruleName} {e.message}"
 
     @property
     def message(self) -> str:
         if not self.args or not isinstance(self.args[0], RecognitionException):
             return super().__str__()
 
@@ -104,76 +111,71 @@
             return f"unknown recognition error type: {type(e).__name__}"
 
     def __str__(self) -> str:
         return f"Line {self.line}, Column {self.column}: {self.message}"
 
 
 class WizardParseError(WizardError):
-
     """
     Error raised when a parsing error occurs.
     """
 
     pass
 
 
 class WizardUnsupportedOperation(WizardError):
     """
     Error raised when an operation is not supported (not yet implemented).
     """
 
-    def __init__(self, context: ParserRuleContext, operation: str):
+    def __init__(self, context: ParserRuleContext | None, operation: str):
         super().__init__(context, f"'{operation}' operation is not implemented.")
 
 
 class WizardIndexError(WizardError):
-
     _index: int
 
-    def __init__(self, context: ParserRuleContext, index: int):
+    def __init__(self, context: ParserRuleContext | None, index: int):
         super().__init__(context, f"Index {index} out of range.")
         self._index = index
 
     @property
     def index(self) -> int:
         return self._index
 
 
 class WizardNameError(WizardError):
-
     _name: str
 
-    def __init__(self, context: ParserRuleContext, name):
+    def __init__(self, context: ParserRuleContext | None, name: str):
         super().__init__(context, f"The name '{name}' is not defined.")
         self._name = name
 
     @property
     def name(self) -> str:
         return self._name
 
 
 class WizardTypeError(WizardError):
     pass
 
 
 class WizardMissingPackageError(WizardError):
-
     _name: str
 
     def __init__(self, context: ParserRuleContext, name: str):
         super().__init__(context, f"Trying to activate missing '{name}' sub-package.")
         self._name = name
 
     @property
     def subpackage(self) -> str:
         return self._name
 
 
 class WizardMissingPluginError(WizardError):
-
     _name: str
 
     def __init__(self, context: ParserRuleContext, name: str):
         super().__init__(context, f"Trying to activate missing '{name}' plugin.")
         self._name = name
 
     @property
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/expr.py` & `bain_wizard_interpreter-1.0.4/src/wizard/expr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-# -*- encoding: utf-8 -*-
-
 import codecs
 import re
-from typing import Callable, List, Mapping, Optional, Type, overload
+from collections.abc import Mapping, Sequence
+from typing import Any, Callable, Type, overload
 
 from .antlr4.wizardParser import wizardParser
 from .errors import WizardIndexError, WizardNameError, WizardParseError, WizardTypeError
 from .severity import Issue, SeverityContext
 from .state import WizardInterpreterState
-from .value import (  # noqa: F401
+from .value import (
     SubPackage,
     SubPackages,
     Value,
     ValueType,
     VariableType,
-    Void,
 )
 
 
 class WizardExpressionVisitor:
-
     """
     Visitor for Wizard expression. This visitor can be used to interpret Wizard
     expression and return `Value` object. The main entry point is `visitExpr()`
     which takes an expression context and returns a `Value`.
     """
 
     BAD_ESCAPE_SEQUENCE = re.compile(r"(^|(?<=[^\\]))\\(?=[^abfnrtuUx0-7\\])")
 
     _subpackages: SubPackages
-    _functions: Mapping[str, Callable[[WizardInterpreterState, List[Value]], Value]]
+    _functions: Mapping[
+        str, Callable[[WizardInterpreterState, Sequence[Value[Any]]], Value[Any]]
+    ]
     _severity: SeverityContext
 
     def __init__(
         self,
         subpackages: SubPackages,
-        functions: Mapping[str, Callable[[WizardInterpreterState, List[Value]], Value]],
+        functions: Mapping[
+            str, Callable[[WizardInterpreterState, Sequence[Value[Any]]], Value[Any]]
+        ],
         severity: SeverityContext,
     ):
         """
         Args:
             subpackages: The subpackages for the visitor.
             functions: The list of usable functions.
             severity: The severity context.
@@ -48,234 +49,243 @@
         self._functions = functions
         self._severity = severity
 
     def visitTimesDivideModulo(
         self,
         ctx: wizardParser.TimesDivideModuloContext,
         state: WizardInterpreterState,
-    ) -> Value:
-        op: Callable[[Value, Value], Value] = Value.__mul__
+    ) -> Value[float] | Value[int]:
+        op: Callable[[Value[Any], Value[Any]], Value[int] | Value[float]] = (
+            Value.__mul__
+        )
         if ctx.Divide():
             op = Value.__div__
         elif ctx.Modulo():
             op = Value.__mod__
         return op(
             self.visitExpr(ctx.expr(0), state),
             self.visitExpr(ctx.expr(1), state),
         )
 
     def visitPlusMinus(
         self, ctx: wizardParser.PlusMinusContext, state: WizardInterpreterState
-    ) -> Value:
-        op: Callable[[Value, Value], Value] = Value.__add__
+    ) -> Value[float] | Value[int] | Value[str]:
+        op: Callable[
+            [Value[Any], Value[Any]], Value[int] | Value[float] | Value[str]
+        ] = Value.__add__
         if ctx.Minus():
             op = Value.__sub__
         return op(
             self.visitExpr(ctx.expr(0), state),
             self.visitExpr(ctx.expr(1), state),
         )
 
     def visitOr(
         self, ctx: wizardParser.OrContext, state: WizardInterpreterState
-    ) -> Value:
+    ) -> Value[bool]:
         return self.visitExpr(ctx.expr(0), state) | self.visitExpr(ctx.expr(1), state)
 
     def visitFunctionCall(
         self,
         ctx: wizardParser.FunctionCallContext,
         state: WizardInterpreterState,
-    ) -> Value:
-
+    ) -> Value[Any]:
         name = ctx.Identifier().getText()
 
         # Specific handle for Exec:
         if name == "Exec":
             raise WizardNameError(ctx, "Exec() cannot be used in a complex expression.")
         if name == "EndExec":
             raise WizardNameError(ctx, "EndExec() should not be used explicitly.")
 
-        function: Callable[[WizardInterpreterState, List[Value]], Value]
+        function: Callable[[WizardInterpreterState, Sequence[Value[Any]]], Value[Any]]
         if name in self._functions:
             function = self._functions[name]
             is_visit = False
         elif hasattr(self, "visit" + name):
             function = getattr(self, "visit" + name)
             is_visit = True
         else:
             raise WizardNameError(ctx, name)
 
-        values: List[Value] = []
+        values: list[Value[Any]] = []
         if ctx.argList():
             for ex in ctx.argList().expr():
                 values.append(self.visitExpr(ex, state))
 
         if is_visit:
             return Value(function(state, *(value.value for value in values)))
         return function(state, values)
 
     def visitDotFunctionCall(
         self,
         ctx: wizardParser.DotFunctionCallContext,
         state: WizardInterpreterState,
-    ) -> Value:
-        values: List[Value] = [self.visitExpr(ctx.expr(), state)]
+    ) -> Value[Any]:
+        values: list[Value[Any]] = [self.visitExpr(ctx.expr(), state)]
 
         mname = "{}.{}".format(values[0].type, ctx.Identifier().getText())
         if mname not in self._functions:
             raise WizardNameError(ctx, mname)
 
         if ctx.argList():
             for ex in ctx.argList().expr():
                 values.append(self.visitExpr(ex, state))
 
         return self._functions[mname](state, values)
 
     def visitIn(
         self, ctx: wizardParser.InContext, state: WizardInterpreterState
-    ) -> Value:
+    ) -> Value[bool]:
         return self.visitExpr(ctx.expr(1), state).contains(
             self.visitExpr(ctx.expr(0), state), bool(ctx.Colon())
         )
 
     def doCmp(
         self,
-        op: Callable[[Value, Value], Value],
-        lhs: Value,
-        rhs: Value,
+        ctx: wizardParser.ExprContext,
+        op: Callable[[Value[Any], Value[Any]], Value[bool]],
+        lhs: Value[Any],
+        rhs: Value[Any],
         case_insensitive: bool = True,
-    ) -> Value:
+    ) -> Value[bool]:
         if case_insensitive:
             if not isinstance(lhs.value, str) or not isinstance(rhs.value, str):
                 raise WizardTypeError(
+                    ctx,
                     "Cannot use case-insensitive comparison with values of type"
-                    f" {lhs.type}, {rhs.type}."
+                    f" {lhs.type}, {rhs.type}.",
                 )
             lhs = Value(lhs.value.lower())
             rhs = Value(rhs.value.lower())
         return op(lhs, rhs)
 
     def visitEqual(
         self, ctx: wizardParser.EqualContext, state: WizardInterpreterState
-    ) -> Value:
+    ) -> Value[bool]:
         op = Value.equals
         if ctx.NotEqual():
             op = Value.not_equals
         return self.doCmp(
+            ctx,
             op,
             self.visitExpr(ctx.expr(0), state),
             self.visitExpr(ctx.expr(1), state),
             bool(ctx.Colon()),
         )
 
     def visitLesser(
         self, ctx: wizardParser.LesserContext, state: WizardInterpreterState
-    ) -> Value:
+    ) -> Value[bool]:
         op = Value.__le__
         if ctx.Lesser():
             op = Value.__lt__
         return self.doCmp(
+            ctx,
             op,
             self.visitExpr(ctx.expr(0), state),
             self.visitExpr(ctx.expr(1), state),
             bool(ctx.Colon()),
         )
 
     def visitGreater(
         self, ctx: wizardParser.GreaterContext, state: WizardInterpreterState
-    ) -> Value:
+    ) -> Value[bool]:
         op = Value.__ge__
         if ctx.Greater():
             op = Value.__gt__
         return self.doCmp(
+            ctx,
             op,
             self.visitExpr(ctx.expr(0), state),
             self.visitExpr(ctx.expr(1), state),
             bool(ctx.Colon()),
         )
 
     def visitExponentiation(
         self,
         ctx: wizardParser.ExponentiationContext,
         state: WizardInterpreterState,
-    ) -> Value:
+    ) -> Value[float] | Value[int]:
         return self.visitExpr(ctx.expr(0), state) ** self.visitExpr(ctx.expr(1), state)
 
     def visitIndex(
         self, ctx: wizardParser.IndexContext, state: WizardInterpreterState
-    ) -> Value:
+    ) -> Value[str] | Value[SubPackage]:
         return self.visitExpr(ctx.expr(0), state)[self.visitExpr(ctx.expr(1), state)]
 
-    def visitPreDecrement(
+    def _visitIncDec(
         self,
-        ctx: wizardParser.PreDecrementContext,
+        ctx: wizardParser.PreDecrementContext
+        | wizardParser.PostDecrementContext
+        | wizardParser.PreIncrementContext
+        | wizardParser.PostIncrementContext,
+        offset: int,
         state: WizardInterpreterState,
-    ) -> Value:
+    ) -> Value[int] | Value[float]:
         name = ctx.Identifier().getText()
-        if name not in state._variables:
+        value = state.variables.get(name, None)
+        if value is None:
             raise WizardNameError(ctx, name)
-        state._variables[ctx.Identifier().getText()] -= Value(1)
-        return state._variables[ctx.Identifier().getText()]
+
+        state.set(name, value + Value(offset))
+        return state.variables[name]
+
+    def visitPreDecrement(
+        self,
+        ctx: wizardParser.PreDecrementContext,
+        state: WizardInterpreterState,
+    ) -> Value[int] | Value[float]:
+        return self._visitIncDec(ctx, -1, state)
+
+    def visitPostDecrement(
+        self,
+        ctx: wizardParser.PostDecrementContext,
+        state: WizardInterpreterState,
+    ) -> Value[int] | Value[float]:
+        return self._visitIncDec(ctx, -1, state)
 
     def visitPreIncrement(
         self,
         ctx: wizardParser.PreIncrementContext,
         state: WizardInterpreterState,
-    ) -> Value:
-        name = ctx.Identifier().getText()
-        if name not in state._variables:
-            raise WizardNameError(ctx, name)
-        state._variables[ctx.Identifier().getText()] += Value(1)
-        return state._variables[ctx.Identifier().getText()]
+    ) -> Value[int] | Value[float]:
+        return self._visitIncDec(ctx, +1, state)
 
     def visitPostIncrement(
         self,
         ctx: wizardParser.PostIncrementContext,
         state: WizardInterpreterState,
-    ) -> Value:
-        name = ctx.Identifier().getText()
-        if name not in state._variables:
-            raise WizardNameError(ctx, name)
-        state._variables[ctx.Identifier().getText()] += Value(1)
-        return state._variables[ctx.Identifier().getText()]
-
-    def visitPostDecrement(
-        self,
-        ctx: wizardParser.PostDecrementContext,
-        state: WizardInterpreterState,
-    ) -> Value:
-        name = ctx.Identifier().getText()
-        if name not in state._variables:
-            raise WizardNameError(ctx, name)
-        state._variables[ctx.Identifier().getText()] -= Value(1)
-        return state._variables[ctx.Identifier().getText()]
+    ) -> Value[int] | Value[float]:
+        return self._visitIncDec(ctx, +1, state)
 
     def visitNegative(
         self, ctx: wizardParser.NegativeContext, state: WizardInterpreterState
-    ) -> Value:
+    ) -> Value[int] | Value[float]:
         return -self.visitExpr(ctx.expr(), state)
 
     def visitNot(
         self, ctx: wizardParser.NotContext, state: WizardInterpreterState
-    ) -> Value:
+    ) -> Value[bool]:
         return self.visitExpr(ctx.expr(), state).logical_not()
 
     def visitParenExpr(
         self, ctx: wizardParser.ParenExprContext, state: WizardInterpreterState
-    ) -> Value:
+    ) -> Value[Any]:
         return self.visitExpr(ctx.expr(), state)
 
     def visitSlice(
         self, ctx: wizardParser.SliceContext, state: WizardInterpreterState
-    ) -> Value:
+    ) -> Value[str]:
         # expr LeftBracket expr? Colon expr? (Colon expr?)? RightBracket
         lhs = self.visitExpr(ctx.expr(0), state)
 
-        start: Optional[Value] = None
-        end: Optional[Value] = None
-        step: Optional[Value] = None
+        start: Value[Any] | None = None
+        end: Value[Any] | None = None
+        step: Value[Any] | None = None
 
         # Index of end expression in ctx.children (without start by
         # default):
         cidx: int = 3
 
         # Is there a start?
         if isinstance(ctx.children[2], wizardParser.ExprContext):
@@ -291,92 +301,93 @@
             step = self.visitExpr(ctx.children[-2], state)
 
         # We keep None and let python built-in slice() do the job for us.
         return lhs.slice(start, end, step)
 
     def visitAnd(
         self, ctx: wizardParser.AndContext, state: WizardInterpreterState
-    ) -> Value:
-        lhs, rhs = self.visitExpr(ctx.expr(0), state), self.visitExpr(
-            ctx.expr(1), state
+    ) -> Value[bool]:
+        lhs, rhs = (
+            self.visitExpr(ctx.expr(0), state),
+            self.visitExpr(ctx.expr(1), state),
         )
         return lhs & rhs
 
     def visitValue(
         self, ctx: wizardParser.ValueContext, state: WizardInterpreterState
-    ) -> Value:
+    ) -> Value[Any]:
         if ctx.constant():
             return self.visitConstant(ctx.constant())
         if ctx.integer():
             return self.visitInteger(ctx.integer())
         if ctx.decimal():
             return self.visitDecimal(ctx.decimal())
         if ctx.string():
             return self.visitString(ctx.string())
         if ctx.Identifier():
             name = ctx.Identifier().getText()
-            if name not in state._variables:
+            if name not in state.variables:
                 # Severity check:
                 self._severity.raise_or_warn(
                     Issue.USAGE_OF_NOTSET_VARIABLES,
                     WizardNameError(ctx, name),
                     f"Variable {name} used before being set, default to 0.",
                 )
                 return Value(0)
             else:
-                return state._variables[ctx.Identifier().getText()]
+                return state.variables[ctx.Identifier().getText()]
 
         raise WizardNameError(ctx, ctx.getText())
 
-    def visitConstant(self, ctx: wizardParser.ConstantContext) -> Value:
+    def visitConstant(
+        self, ctx: wizardParser.ConstantContext
+    ) -> Value[bool] | Value[SubPackages]:
         if ctx.getText() == "False":
             return Value(False)
         elif ctx.getText() == "True":
             return Value(True)
         else:
             return Value(self._subpackages)
 
-    def visitInteger(self, ctx: wizardParser.IntegerContext) -> Value:
+    def visitInteger(self, ctx: wizardParser.IntegerContext) -> Value[int]:
         return Value(int(ctx.getText()))
 
-    def visitDecimal(self, ctx: wizardParser.DecimalContext) -> Value:
+    def visitDecimal(self, ctx: wizardParser.DecimalContext) -> Value[float]:
         return Value(float(ctx.getText()))
 
-    def visitString(self, ctx: wizardParser.StringContext) -> Value:
+    def visitString(self, ctx: wizardParser.StringContext) -> Value[str]:
         # Remove the quotation marks:
         txt = ctx.getText()[1:-1]
 
         # Remove bad escape sequences:
         txt = self.BAD_ESCAPE_SEQUENCE.sub("", txt)
 
         # Replace escape sequences by Python escape sequences:
         txt = codecs.decode(txt, "unicode_escape")
 
         return Value(txt)
 
     @overload
     def visitExpr(
         self, ctx: wizardParser.ExprContext, state: WizardInterpreterState
-    ) -> Value:
-        ...
+    ) -> Value[Any]: ...
 
     @overload
     def visitExpr(
         self,
         ctx: wizardParser.ExprContext,
         state: WizardInterpreterState,
         typ: Type[ValueType],
-    ) -> Value[ValueType]:
-        ...
+    ) -> Value[ValueType]: ...
 
     def visitExpr(
         self,
         ctx: wizardParser.ExprContext,
         state: WizardInterpreterState,
-        typ: Optional[Type[ValueType]] = None,
+        typ: Type[ValueType] | None = None,
     ):
         """
         Evaluate the given expression.
 
         IMPORTANT: This method can modify the state.
 
         Args:
@@ -388,21 +399,23 @@
             The result of the given expression.
         """
 
         if ctx.exception:
             raise WizardParseError(ctx, ctx.exception)
 
         try:
-            value = getattr(self, "visit" + type(ctx).__name__[:-7])(ctx, state)
+            value: Value[Any] = getattr(self, "visit" + type(ctx).__name__[:-7])(
+                ctx, state
+            )
         except TypeError as te:
-            raise WizardTypeError(ctx, *te.args)
+            raise WizardTypeError(ctx, *te.args) from te
         except IndexError as ie:
-            raise WizardIndexError(ctx, *ie.args)
+            raise WizardIndexError(ctx, *ie.args) from ie
 
         if typ is not None and not isinstance(value.value, typ):
             raise WizardTypeError(
                 ctx,
                 f"Expected value of type {VariableType.from_pytype(typ)} but got value"
                 f" of type {value.type}.",
             )
 
-        return value  # type: ignore
+        return value
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/functions.py` & `bain_wizard_interpreter-1.0.4/src/wizard/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,82 @@
-# -*- encoding: utf-8 -*-
-
 """
 This file contains the implementation of the "basic" functions for BAIN Wizard,
 i.e. functions that do not require specific handling.
 """
 
 import inspect
-from typing import Callable, Dict, List, Mapping, Union
+from collections.abc import Sequence
+from typing import Any, Callable, TypeAlias, cast
 
-from .expr import SubPackage, SubPackages, Value, VariableType, Void
+from .expr import SubPackage, SubPackages, VariableType
 from .manager import ManagerModInterface
 from .severity import SeverityContext
 from .state import WizardInterpreterState
+from .value import Value, Void
 
+WizardFunction: TypeAlias = Callable[
+    [WizardInterpreterState, Sequence[Value[Any]]], Value[Any]
+]
 
-class WizardFunctions:
 
+class WizardFunctions:
     """
     This is simply a class containing all the basic functions.
     """
 
-    def str(self, value: Value) -> Value:
+    def str_(self, value: Value[Any]) -> Value[str]:
         return Value(str(value.value))
 
-    def int(self, value: Value) -> Value:
+    def int_(self, value: Value[Any]) -> Value[int]:
         if isinstance(value.value, (SubPackage, SubPackages, Void)):
             return Value(0)
         return Value(int(value.value))
 
-    def float(self, value: Value) -> Value:
+    def float_(self, value: Value[Any]) -> Value[float]:
         if isinstance(value.value, (SubPackage, SubPackages, Void)):
             return Value(0.0)
         return Value(float(value.value))
 
-    def len(self, value: Value) -> Value:
+    def len_(self, value: Value[Any]) -> Value[int]:
         if not isinstance(value.value, str):
             return Value(0)
         return Value(len(value.value))
 
-    def startswith(self, value: Value, *args: Value) -> Value:
+    def startswith(self, value: Value[Any], *args: Value[Any]) -> Value[bool]:
         if not isinstance(value.value, str):
             return Value(False)
         for prefix in args:
             if not isinstance(prefix.value, str):
                 continue
             if value.value.startswith(prefix.value):
                 return Value(True)
         return Value(False)
 
-    def endswith(self, value: Value, *args: Value) -> Value:
+    def endswith(self, value: Value[Any], *args: Value[Any]) -> Value[bool]:
         if not isinstance(value.value, str):
             return Value(False)
         for prefix in args:
             if not isinstance(prefix.value, str):
                 continue
             if value.value.endswith(prefix.value):
                 return Value(True)
         return Value(False)
 
-    def lower(self, value: Value) -> Value:
+    def lower(self, value: Value[Any]) -> Value[str]:
         if not isinstance(value.value, str):
             return value
         return Value(value.value.lower())
 
     def find(
         self,
-        string: Value,
-        substring: Value,
-        start: Value = Value(0),
-        end: Value = Value(-1),
-    ) -> Value:
+        string: Value[Any],
+        substring: Value[Any],
+        start: Value[Any] = Value(0),
+        end: Value[Any] = Value(-1),
+    ) -> Value[int]:
         if (
             not isinstance(string.value, str)
             or not isinstance(substring.value, str)
             or not isinstance(start.value, int)
             or not isinstance(end.value, int)
         ):
             return Value(-1)
@@ -82,19 +85,19 @@
             string.value.find(
                 substring.value, start.value, end.value if end.value != -1 else None
             )
         )
 
     def rfind(
         self,
-        string: Value,
-        substring: Value,
-        start: Value = Value(0),
-        end: Value = Value(-1),
-    ) -> Value:
+        string: Value[Any],
+        substring: Value[Any],
+        start: Value[Any] = Value(0),
+        end: Value[Any] = Value(-1),
+    ) -> Value[int]:
         if (
             not isinstance(string.value, str)
             or not isinstance(substring.value, str)
             or not isinstance(start.value, int)
             or not isinstance(end.value, int)
         ):
             return Value(-1)
@@ -111,47 +114,45 @@
 
     def __init__(self, t: type):
         self.t = t
 
 
 def wrap_function(
     name: str,
-    method,
-    *args: Union[optional, type],
+    method: Callable[..., Any],
+    *args: optional | type,
     varargs: bool = False,
     rawargs: bool = False,
-) -> Callable[[WizardInterpreterState, List[Value]], Value]:
-
+) -> WizardFunction:
     """
     Wrap the given function to be usable by the Wizard expression visitor.
 
     Args:
         name: The name of the function, for logging purpose (warning / errors).
         method: The function to wrap.
         *args: The type of arguments expected by the method.
         varargs: True if the method accept any number of arguments.
         rawargs: True if the method accept Value(), False to extract the underlying
             object.
     """
 
-    def fn(st: WizardInterpreterState, vs: List[Value]) -> Value:
-
+    def fn(st: WizardInterpreterState, vs: Sequence[Value[Any]]) -> Value[Any]:
         # List of Python arguments:
-        pargs: List = []
+        pargs: list[Any] = []
 
         if not varargs and len(vs) > len(args):
             raise TypeError(f"{name}: too many arguments.")
 
         for iarg, arg in enumerate(args):
             if iarg >= len(vs) and not isinstance(arg, optional):
                 raise TypeError(f"{name}: missing required positional argument(s).")
 
             tp: type
             if isinstance(arg, optional):
-                tp = arg.t
+                tp = cast(type, arg.t)  # type: ignore
             else:
                 tp = arg
 
             if not isinstance(vs[iarg].value, tp):
                 raise TypeError(
                     f"Argument at position {iarg} has incorrect type for"
                     f" {name}, expected {VariableType.from_pytype(tp)} got"
@@ -159,81 +160,80 @@
                 )
 
             if rawargs:
                 pargs.append(vs[iarg])
             else:
                 pargs.append(vs[iarg].value)
 
-        ret: Value = method(*pargs)
+        ret: Value[Any] | Void | None = method(*pargs)
         if ret is None:
             ret = Void()
 
         if not rawargs:
-            ret = Value(ret)  # type: ignore
+            ret = Value(ret)
 
-        return ret
+        return cast(Value[Any], ret)
 
     return fn
 
 
-def make_basic_functions() -> Dict[
-    str, Callable[[WizardInterpreterState, List[Value]], Value]
-]:
+def make_basic_functions() -> dict[str, WizardFunction]:
     """
     Create a list of basic functions.
 
     Args:
         wf: The WizardFunctions object to use for the basic functions.
 
     Returns:
         A mapping from function name to basic functions, including methods.
     """
 
     wf = WizardFunctions()
-    fns: Dict[str, Callable[[WizardInterpreterState, List[Value]], Value]] = {}
+    fns: dict[str, WizardFunction] = {}
 
     # Add all the free functions:
     for fname in dir(wf):
         if fname.startswith("__"):
             continue
         sig = inspect.signature(getattr(wf, fname))
         varargs = "args" in sig.parameters
         fns[fname] = wrap_function(
-            fname,
+            fname.rstrip("_"),
             getattr(wf, fname),
             *(object for _ in range(len(sig.parameters) - varargs)),
             varargs=varargs,
             rawargs=True,
         )
 
     # Add methods:
     for fname in dir(wf):
         if fname.startswith("__"):
             continue
         fns["string." + fname] = fns[fname]
 
     for t in ("integer", "float", "bool"):
-        fns[t + ".str"] = fns["str"]
+        fns[t + ".str"] = fns["str_"]
 
-    return fns
+    # strip the right _ from the name for special function (int_, float_, etc.)
+    return {name.rstrip("_"): fn for name, fn in fns.items()}
 
 
 def make_manager_functions(
     manager: ManagerModInterface, scontext: SeverityContext
-) -> Mapping[str, Callable[[WizardInterpreterState, List[Value]], Value]]:
+) -> dict[str, WizardFunction]:
     """
     Add manager functions to the _functions member variables. These functions
     calls method of the manager passed in.
 
     Args:
         manager: The manager to delete the call to.
         scontext: The severity context to use (for the Note keyword for instance).
     """
 
-    fns: Dict[str, Callable[[WizardInterpreterState, List[Value]], Value]] = {}
+    fns: dict[str, WizardFunction] = {}
 
     for t in [
         # Functions:
         ("CompareGameVersion", manager.compareGameVersion, str),
         ("CompareSEVersion", manager.compareSEVersion, str),
         ("CompareGEVersion", manager.compareGEVersion, str),
         ("CompareWBVersion", manager.compareWBVersion, str),
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/interpreter.py` & `bain_wizard_interpreter-1.0.4/src/wizard/interpreter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# -*- encoding: utf-8 -*-
+from __future__ import annotations
 
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Any, Optional, Sequence, TextIO, Type, Union, overload
+from typing import Any, Generic, TextIO, overload
 
 from antlr4 import InputStream
 
 from .contexts import (
     WizardInterpreterContext,
     WizardInterpreterContextFactory,
     WizardTerminationContext,
     WizardTopLevelContext,
 )
 from .state import ContextState, WizardInterpreterState
 from .utils import make_top_level_context
 
 
-class WizardInterpreter:
-
+class WizardInterpreter(Generic[ContextState]):
     """
     The WizardInterpreter is the main interpreter for Wizard scripts.
     """
 
     # The severity context:
-    _factory: WizardInterpreterContextFactory
+    _factory: WizardInterpreterContextFactory[ContextState]
 
     def __init__(
         self,
-        factory: WizardInterpreterContextFactory,
+        factory: WizardInterpreterContextFactory[ContextState],
     ):
         """
         Args:
             factory: The context factory.
         """
         self._factory = factory
 
     def exec_until(
         self,
         context: WizardInterpreterContext[ContextState, Any],
-        targets: Sequence[Type[WizardInterpreterContext]],
+        targets: Sequence[type[WizardInterpreterContext[ContextState, Any]]],
     ) -> WizardInterpreterContext[ContextState, Any]:
         """
         Execute the contexts until a context of the given type is found, or
         a termination context is found. If context is one of the given targets,
         the function returns immediately.
 
         Args:
@@ -57,26 +57,24 @@
         while not isinstance(context, stargets + (WizardTerminationContext,)):
             context = context.exec()
 
         return context
 
     @overload
     def make_top_level_context(
-        self, script: Union[InputStream, Path, TextIO, str], state: ContextState
-    ) -> WizardTopLevelContext[ContextState]:
-        ...
+        self, script: InputStream | Path | TextIO | str, state: ContextState
+    ) -> WizardTopLevelContext[ContextState]: ...
 
     @overload
     def make_top_level_context(
-        self, script: Union[InputStream, Path, TextIO, str]
-    ) -> WizardTopLevelContext[WizardInterpreterState]:
-        ...
+        self, script: InputStream | Path | TextIO | str
+    ) -> WizardTopLevelContext[WizardInterpreterState]: ...
 
     def make_top_level_context(
         self,
-        script: Union[InputStream, Path, TextIO, str],
-        state: Optional[ContextState] = None,
-    ) -> Union[
-        WizardTopLevelContext[ContextState],
-        WizardTopLevelContext[WizardInterpreterState],
-    ]:
+        script: InputStream | Path | TextIO | str,
+        state: ContextState | None = None,
+    ) -> (
+        WizardTopLevelContext[ContextState]
+        | WizardTopLevelContext[WizardInterpreterState]
+    ):
         return make_top_level_context(script, self._factory, state)  # type: ignore
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/keywords.py` & `bain_wizard_interpreter-1.0.4/src/wizard/keywords.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-# -*- encoding: utf-8 -*-
-
 from enum import Enum
-from typing import Generic, Optional
+from typing import Generic
 
 from .contexts.keywords import WizardKeywordContext
 from .severity import SeverityContext
 from .state import ContextState
 
 
 class WizardKeyword(Enum):
-
     """
     Enumeration representing possible keywords in a Wizard scripts.
     """
 
     DESELECT_ALL = "DeSelectAll"
     DESELECT_ALL_PLUGINS = "DeSelectAllPlugins"
     DESELECT_PLUGIN = "DeSelectPlugin"
@@ -26,77 +23,89 @@
     SELECT_ALL = "SelectAll"
     SELECT_ALL_PLUGINS = "SelectAllPlugins"
     SELECT_PLUGIN = "SelectPlugin"
     SELECT_SUBPACKAGE = "SelectSubPackage"
 
 
 class WizardKeywordVisitor(Generic[ContextState]):
-
     """
     Keyword visitor that can be extended to perform specific actions for
     each keywords. By default, none of the methods do anything.
     """
 
     _severity: SeverityContext
 
     def __init__(self, severity: SeverityContext):
         self._severity = severity
 
-    def visitDeSelectAll(self, context: WizardKeywordContext, state: ContextState):
+    def visitDeSelectAll(
+        self, context: WizardKeywordContext[ContextState], state: ContextState
+    ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
         """
         ...
 
     def visitDeSelectAllPlugins(
-        self, context: WizardKeywordContext, state: ContextState
+        self, context: WizardKeywordContext[ContextState], state: ContextState
     ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
         """
         ...
 
     def visitDeSelectPlugin(
-        self, context: WizardKeywordContext, state: ContextState, name: str
+        self,
+        context: WizardKeywordContext[ContextState],
+        state: ContextState,
+        name: str,
     ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
             name: The name of the plugin to de-select.
         """
         ...
 
     def visitDeSelectSubPackage(
-        self, context: WizardKeywordContext, state: ContextState, name: str
+        self,
+        context: WizardKeywordContext[ContextState],
+        state: ContextState,
+        name: str,
     ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
             name: The name of the subpackage to de-select.
         """
         ...
 
-    def visitNote(self, context: WizardKeywordContext, state: ContextState, text: str):
+    def visitNote(
+        self,
+        context: WizardKeywordContext[ContextState],
+        state: ContextState,
+        text: str,
+    ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
             text: The text for the note.
         """
         ...
 
     def visitRenamePlugin(
         self,
-        context: WizardKeywordContext,
+        context: WizardKeywordContext[ContextState],
         state: ContextState,
         original_name: str,
         new_name: str,
     ):
         """
         Args:
             context: The context corresponding to the keyword.
@@ -106,79 +115,92 @@
         """
         ...
 
     def visitRequireVersions(
         self,
         state: ContextState,
         game_version: str,
-        script_extender_version: Optional[str],
-        graphics_extender_version: Optional[str],
-        wrye_bash_version: Optional[str],
+        script_extender_version: str | None,
+        graphics_extender_version: str | None,
+        wrye_bash_version: str | None,
     ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
             game_version: The required game version.
             script_extender_version: The required script extender version.
             graphics_extender_version: The required graphics extender version.
             wrye_bash_version: The required wrye bash version.
         """
         ...
 
     def visitResetAllPluginNames(
-        self, context: WizardKeywordContext, state: ContextState
+        self, context: WizardKeywordContext[ContextState], state: ContextState
     ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
         """
         ...
 
     def visitResetPluginName(
-        self, context: WizardKeywordContext, state: ContextState, name: str
+        self,
+        context: WizardKeywordContext[ContextState],
+        state: ContextState,
+        name: str,
     ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
             name: The original name of the plugin.
         """
         ...
 
-    def visitSelectAll(self, context: WizardKeywordContext, state: ContextState):
+    def visitSelectAll(
+        self, context: WizardKeywordContext[ContextState], state: ContextState
+    ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
         """
         ...
 
-    def visitSelectAllPlugins(self, context: WizardKeywordContext, state: ContextState):
+    def visitSelectAllPlugins(
+        self, context: WizardKeywordContext[ContextState], state: ContextState
+    ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
         """
         ...
 
     def visitSelectPlugin(
-        self, context: WizardKeywordContext, state: ContextState, name: str
+        self,
+        context: WizardKeywordContext[ContextState],
+        state: ContextState,
+        name: str,
     ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
             name: The name of the plugin to select.
         """
         ...
 
     def visitSelectSubPackage(
-        self, context: WizardKeywordContext, state: ContextState, name: str
+        self,
+        context: WizardKeywordContext[ContextState],
+        state: ContextState,
+        name: str,
     ):
         """
         Args:
             context: The context corresponding to the keyword.
             state: The interpreter state to update.
             name: The name of the subpackage to select.
         """
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/manager.py` & `bain_wizard_interpreter-1.0.4/src/wizard/manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-# -*- encoding: utf-8 -*-
-
-
 from abc import abstractmethod
-from typing import List, Optional
+from collections.abc import Sequence
 
 
 class ManagerModInterface:
-
     """
     The ManagerModInterface represents the interface to implement to let the
     interpreter (or runner) interact with the game information and files.
     """
 
     # Function methods:
     @abstractmethod
@@ -99,15 +95,15 @@
         Returns:
             The load order of the plugin or fallback if the plugin has no load order
             index.
         """
         ...
 
     @abstractmethod
-    def getPluginStatus(self, filename) -> int:
+    def getPluginStatus(self, filename: str) -> int:
         """
         Returns the status of a plugin in the Data directory.
 
         Args:
             filename: Path relative to the Data direcotry to the plugin.
 
         Returns:
@@ -147,20 +143,19 @@
             an empty string, otherwise returns the name of the folder the path points
             to.
         """
         ...
 
 
 class SelectOption:
-
     """
     Option from SelectOne or SelectMany statement.
     """
 
-    def __init__(self, name: str, desc: str, image: Optional[str] = None):
+    def __init__(self, name: str, desc: str, image: str | None = None):
         self._name = name
         self._desc = desc
         self._image = image
 
     @property
     def name(self) -> str:
         """
@@ -174,15 +169,15 @@
         """
         Returns:
             The description of the option.
         """
         return self._desc
 
     @property
-    def image(self) -> Optional[str]:
+    def image(self) -> str | None:
         """
         Returns:
             The image for the option, or None if there are no image.
         """
         return self._image
 
     def __eq__(self, other: object) -> bool:
@@ -195,15 +190,14 @@
         )
 
     def __repr__(self) -> str:
         return f"SelectOption({self.name}, {self.description}, {self.image})"
 
 
 class ManagerUserInterface:
-
     """
     The ManagerUserInterface represents the interface to implement to let the
     interpreter (or runner) interact with the user.
     """
 
     # Development methods:
     def warning(self, text: str):
@@ -247,15 +241,15 @@
         Returns:
             True to stop executing the script, False to continue.
         """
         return True
 
     @abstractmethod
     def selectOne(
-        self, description: str, options: List[SelectOption], default: SelectOption
+        self, description: str, options: Sequence[SelectOption], default: SelectOption
     ) -> SelectOption:
         """
         Query user to select one of the proposed options.
 
         Args:
             description: Description to display to the user.
             options: List of available options.
@@ -266,17 +260,17 @@
         """
         ...
 
     @abstractmethod
     def selectMany(
         self,
         description: str,
-        options: List[SelectOption],
-        default: List[SelectOption] = [],
-    ) -> List[SelectOption]:
+        options: Sequence[SelectOption],
+        default: Sequence[SelectOption] = [],
+    ) -> Sequence[SelectOption]:
         """
         Query user to select many of the proposed options.
 
         Args:
             description: Description to display to the user.
             options: List of available options.
             default: Default selected options.
@@ -286,17 +280,17 @@
         """
         ...
 
     @abstractmethod
     def requiresVersions(
         self,
         game_version: str,
-        se_version: Optional[str],
-        ge_version: Optional[str],
-        wrye_bash_version: Optional[str],
+        se_version: str | None,
+        ge_version: str | None,
+        wrye_bash_version: str | None,
     ):
         """
         Tests the user system against version requirements you specify. If the
         requirements are not met, a warning dialog will be shown asking if you wish
         to continue anyway.
 
         Args:
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/mappings.py` & `bain_wizard_interpreter-1.0.4/src/wizard/utils/mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# -*- encoding: utf-8 -*-
+from __future__ import annotations
 
-from typing import Iterator, MutableMapping, Optional, Set, TypeVar
+from collections.abc import Iterator, MutableMapping
+from typing import TypeVar
 
 K = TypeVar("K")
 V = TypeVar("V")
 
 
 class StackMutableMapping(MutableMapping[K, V]):
-
     """
     Class representing a stacked mapping. It exposes the usual MutableMapping
     interface, but contains a "fallback" mapping and expose the union of both.
     """
 
-    _parent: Optional["StackMutableMapping[K, V]"]
-    _variables: MutableMapping[K, V]
-    _deleted: Set[K]
+    _parent: StackMutableMapping[K, V] | None
+    _variables: dict[K, V]
+    _deleted: set[K]
 
-    def __init__(self, parent: Optional["StackMutableMapping[K, V]"] = None):
+    def __init__(self, parent: StackMutableMapping[K, V] | None = None):
         self._parent = parent
         self._variables = {}
         self._deleted = set()
 
     def __delitem__(self, item: K):
         # Remove the item from the list of variables:
         if item in self._variables:
@@ -51,27 +51,27 @@
             raise KeyError(item)
 
         # Fallback to parent:
         return self._parent[item]
 
     def __iter__(self) -> Iterator[K]:
         # Retrieve the parent keys:
-        keys: Set[K] = set()
+        keys: set[K] = set()
 
         if self._parent is not None:
             keys.update(self._parent)
             keys.difference_update(self._deleted)
 
         keys.update(self._variables)
 
         return iter(keys)
 
     def __len__(self) -> int:
         # Retrieve the parent keys:
-        keys: Set[K] = set()
+        keys: set[K] = set()
 
         if self._parent is not None:
             keys.update(self._parent)
             keys.difference_update(self._deleted)
 
         keys.update(self._variables)
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/runner.py` & `bain_wizard_interpreter-1.0.4/src/wizard/runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-# -*- encoding: utf-8 -*-
+# pyright: reportPrivateUsage=false
 
-from typing import Any, List, Mapping, MutableMapping, Optional, Sequence, cast
+from __future__ import annotations
+
+from collections.abc import Mapping, MutableMapping, Sequence
+from typing import Any, cast
 
 from .contexts import WizardKeywordContext
 from .errors import WizardMissingPackageError, WizardMissingPluginError
 from .expr import WizardExpressionVisitor
 from .keywords import WizardKeywordVisitor
 from .severity import Issue, SeverityContext
 from .state import WizardInterpreterState
 from .tweaks import WizardINISetting, WizardINISettingEdit, WizardINITweaks
 from .value import Plugin, SubPackage, SubPackages
 
 
 class WizardRunnerState(WizardInterpreterState):
-
     """
     Wrapper around multiple containers that are updated during the execution
     of a Wizard script and need to be rewound.
     """
 
     # The list of selected subpackages and plugins:
-    _subpackages: List[SubPackage]
-    _plugins: List[Plugin]
+    _subpackages: list[SubPackage]
+    _plugins: list[Plugin]
 
     # Renaming of plugins (original name -> new name):
     _renames: MutableMapping[Plugin, str]
 
     # The INI tweaks (disabled and modified settings):
     _tweaks: WizardINITweaks
 
     # The list of notes:
-    _notes: List[str]
+    _notes: list[str]
 
     def __init__(self):
         super().__init__()
         self._subpackages = []
         self._plugins = []
         self._renames = {}
         self._tweaks = WizardINITweaks()
         self._notes = []
 
-    def copy(self) -> "WizardRunnerState":
+    def copy(self) -> WizardRunnerState:
         state: WizardRunnerState = super().copy()  # type: ignore
         state._subpackages.extend(self._subpackages)
         state._plugins.extend(self._plugins)
         state._renames.update(self._renames)
         state._notes.extend(self._notes)
         state._tweaks._disabled.extend(self.tweaks.disabled)
         state._tweaks._modified.extend(self.tweaks.modified)
@@ -89,15 +91,14 @@
         Returns:
             The list of notes.
         """
         return self._notes
 
 
 class WizardRunnerExpressionVisitor(WizardExpressionVisitor):
-
     """
     Simple extension of the expression visitor to update INI tweaks.
     """
 
     def visitDisableINILine(
         self, state: WizardInterpreterState, filename: str, section: str, setting: str
     ):
@@ -116,15 +117,15 @@
     def visitEditINI(
         self,
         state: WizardInterpreterState,
         filename: str,
         section: str,
         setting: str,
         value: Any,
-        comment: Optional[str] = "",
+        comment: str | None = "",
     ):
         """
         Create an INI tweak file with some tweaks in it. If file that to apply the
         tweak to is from the current installer or is the game's ini file, then the
         tweaks are also applied, otherwise, it will just be generated for the user
         to apply manually.
 
@@ -137,18 +138,17 @@
         """
         assert isinstance(state, WizardRunnerState)
         state.tweaks._modified.append(
             WizardINISettingEdit(filename, section, setting, value, comment)
         )
 
 
-class WizardRunnerKeywordVisitor(WizardKeywordVisitor):
-
+class WizardRunnerKeywordVisitor(WizardKeywordVisitor[WizardRunnerState]):
     _subpackages: SubPackages
-    _plugins: List[Plugin]
+    _plugins: list[Plugin]
 
     def __init__(self, subpackages: SubPackages, severity: SeverityContext):
         super().__init__(severity)
         self._subpackages = subpackages
 
         # use a dictionary to keep insertion order and remove duplicates
         plugins = {pg: True for sp in self._subpackages for pg in sp.plugins()}
@@ -159,76 +159,89 @@
         """
         Returns:
             The list of all available subpackages.
         """
         return self._subpackages
 
     @property
-    def plugins(self) -> List[Plugin]:
+    def plugins(self) -> Sequence[Plugin]:
         """
         Returns:
             The list of all available plugins.
         """
         return self._plugins
 
-    def plugins_for(self, subpackage: SubPackage) -> List[Plugin]:
+    def plugins_for(self, subpackage: SubPackage) -> Sequence[Plugin]:
         """
         Returns:
             The list of plugin names in the given subpackage.
         """
         return list(subpackage.plugins())
 
-    def visitDeSelectAll(self, context: WizardKeywordContext, state: WizardRunnerState):
+    def visitDeSelectAll(
+        self,
+        context: WizardKeywordContext[WizardRunnerState],
+        state: WizardRunnerState,
+    ):
         state._subpackages.clear()
         state._plugins.clear()
 
     def visitDeSelectAllPlugins(
-        self, context: WizardKeywordContext, state: WizardRunnerState
+        self, context: WizardKeywordContext[WizardRunnerState], state: WizardRunnerState
     ):
         """
         Args:
             state: The interpreter state to update.
         """
         state._plugins.clear()
 
     def visitDeSelectPlugin(
-        self, context: WizardKeywordContext, state: WizardRunnerState, name: str
+        self,
+        context: WizardKeywordContext[WizardRunnerState],
+        state: WizardRunnerState,
+        name: str,
     ):
         """
         Args:
             state: The interpreter state to update.
             name: The name of the plugin to de-select.
         """
-        if name in state._plugins:
-            state._plugins.remove(cast(Plugin, name))
+        if name in state.plugins:
+            state._plugins.remove(Plugin(name))
 
     def visitDeSelectSubPackage(
-        self, context: WizardKeywordContext, state: WizardRunnerState, name: str
+        self,
+        context: WizardKeywordContext[WizardRunnerState],
+        state: WizardRunnerState,
+        name: str,
     ):
         """
         Args:
             state: The interpreter state to update.
             name: The name of the subpackage to de-select.
         """
-        if name in state._subpackages:
-            state._subpackages.remove(cast(SubPackage, name))
+        if name in state.subpackages:
+            state._subpackages.remove(SubPackage(name))
 
     def visitNote(
-        self, context: WizardKeywordContext, state: WizardRunnerState, text: str
+        self,
+        context: WizardKeywordContext[WizardRunnerState],
+        state: WizardRunnerState,
+        text: str,
     ):
         """
         Args:
             state: The interpreter state to update.
             text: The text for the note.
         """
         state._notes.append(text)
 
     def visitRenamePlugin(
         self,
-        context: WizardKeywordContext,
+        context: WizardKeywordContext[WizardRunnerState],
         state: WizardRunnerState,
         original_name: str,
         new_name: str,
     ):
         """
         Args:
             state: The interpreter state to update.
@@ -237,68 +250,76 @@
         """
         state._renames[Plugin(original_name)] = new_name
 
     def visitRequireVersions(
         self,
         state: WizardRunnerState,
         game_version: str,
-        script_extender_version: Optional[str],
-        graphics_extender_version: Optional[str],
-        wrye_bash_version: Optional[str],
+        script_extender_version: str | None,
+        graphics_extender_version: str | None,
+        wrye_bash_version: str | None,
     ):
         """
         Args:
             state: The interpreter state to update.
             game_version: The required game version.
             script_extender_version: The required script extender version.
             graphics_extender_version: The required graphics extender version.
             wrye_bash_version: The required wrye bash version.
         """
         ...
 
     def visitResetAllPluginNames(
-        self, context: WizardKeywordContext, state: WizardRunnerState
+        self, context: WizardKeywordContext[WizardRunnerState], state: WizardRunnerState
     ):
         """
         Args:
             state: The interpreter state to update.
         """
         state._renames.clear()
 
     def visitResetPluginName(
-        self, context: WizardKeywordContext, state: WizardRunnerState, name: str
+        self,
+        context: WizardKeywordContext[WizardRunnerState],
+        state: WizardRunnerState,
+        name: str,
     ):
         """
         Args:
             state: The interpreter state to update.
             name: The original name of the plugin.
         """
         if name in state._renames:
-            del state._renames[cast(Plugin, name)]
+            del state._renames[Plugin(name)]
 
-    def visitSelectAll(self, context: WizardKeywordContext, state: WizardRunnerState):
+    def visitSelectAll(
+        self, context: WizardKeywordContext[WizardRunnerState], state: WizardRunnerState
+    ):
         """
         Args:
             state: The interpreter state to update.
         """
         state._subpackages = list(self._subpackages)
         self.visitSelectAllPlugins(context, state)
 
     def visitSelectAllPlugins(
-        self, context: WizardKeywordContext, state: WizardRunnerState
+        self, context: WizardKeywordContext[WizardRunnerState], state: WizardRunnerState
     ):
         """
         Args:
             state: The interpreter state to update.
         """
         # Guess we only select plugins from selected subpackages?
         state._plugins = [pg for sp in state._subpackages for pg in sp.plugins()]
 
     def visitSelectPlugin(
-        self, context: WizardKeywordContext, state: WizardRunnerState, name: str
+        self,
+        context: WizardKeywordContext[WizardRunnerState],
+        state: WizardRunnerState,
+        name: str,
     ):
         """
         Args:
             state: The interpreter state to update.
             name: The name of the plugin to select.
         """
         try:
@@ -310,15 +331,18 @@
                 f"Trying to select plugin '{name}' that does not exist.",
             )
             return
 
         state._plugins.append(self._plugins[ipg])
 
     def visitSelectSubPackage(
-        self, context: WizardKeywordContext, state: WizardRunnerState, name: str
+        self,
+        context: WizardKeywordContext[WizardRunnerState],
+        state: WizardRunnerState,
+        name: str,
     ):
         """
         Args:
             state: The interpreter state to update.
             name: The name of the subpackage to select.
         """
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/scriptrunner.py` & `bain_wizard_interpreter-1.0.4/src/wizard/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,200 +1,177 @@
-# -*- encoding: utf-8 -*-
-
-from enum import Enum, auto
 from pathlib import Path
-from typing import Optional, TextIO, Tuple, Union
+from typing import Any, BinaryIO, TextIO, Union, overload
+
+import chardet
+from antlr4 import CommonTokenStream, InputStream
+from antlr4.error.ErrorListener import ConsoleErrorListener
+
+from ..antlr4.wizardLexer import wizardLexer
+from ..antlr4.wizardParser import wizardParser
+from ..contexts import WizardInterpreterContextFactory, WizardTopLevelContext
+from ..contexts.utils import wrap_exceptions
+from ..expr import WizardExpressionVisitor
+from ..functions import make_basic_functions, make_manager_functions
+from ..keywords import WizardKeywordVisitor
+from ..manager import ManagerModInterface
+from ..runner import WizardRunnerExpressionVisitor, WizardRunnerKeywordVisitor
+from ..severity import SeverityContext
+from ..state import ContextState, WizardInterpreterState
+from ..value import SubPackages
+
+
+def make_basic_context_factory(
+    subpackages: SubPackages, severity: SeverityContext
+) -> WizardInterpreterContextFactory[Any]:
+    """
+    Make a basic context factory from the given subpackages and severity context.
+    The expression visitor includes the basic functions (see `make_basic_functions`).
+
+    Args:
+        subpackages: The subpackages used for the expression visitor.
+        severity: The severity context to use.
+
+    Returns:
+        A basic context factory, built using default expression and keyword visitors.
+    """
+    return WizardInterpreterContextFactory(
+        WizardExpressionVisitor(subpackages, make_basic_functions(), severity),
+        WizardKeywordVisitor(severity),
+        severity,
+    )
+
+
+def make_runner_context_factory(
+    subpackages: SubPackages, manager: ManagerModInterface, severity: SeverityContext
+) -> WizardInterpreterContextFactory[Any]:
+    """
+    Make a runner context factory from the given subpackages, severity context and
+    manager.
+
+    This method constructs a context factory using a `WizardRunnerExpressionVisitor`
+    and a `WizardRunnerKeywordVisitor` constructed from the given parameters. The
+    expression visitor also includes the basic functions (see `make_basic_functions`).
+
+    Args:
+        subpackages: The subpackages used for the expression visitor and keyword
+            visitors.
+        manager: The manager to use for the expression visitor (functions).
+        severity: The severity context to use.
+
+    Returns:
+        A context factory, built using runner expression and keyword visitors.
+    """
+    functions = make_basic_functions()
+    functions.update(make_manager_functions(manager, severity))
+    evisitor = WizardRunnerExpressionVisitor(subpackages, functions, severity)
+    kvisitor = WizardRunnerKeywordVisitor(subpackages, severity)
+    return WizardInterpreterContextFactory(evisitor, kvisitor, severity)
+
+
+def make_parse_wizard_context(
+    script: Union[InputStream, Path, BinaryIO, TextIO, str],
+    wrap_excs: bool = True,
+) -> wizardParser.ParseWizardContext:
+    """
+    Create a ParseWizardContext from the given script. Depending on the type of
+    the script, the following procedure is used to parse the script:
+    - If `script` is an `InputStream`, it is used as-is.
+    - If `script` is a `Path`, it should point to a file containing a Wizard script.
+    - If `script` is a `TextIO`, it is equivalent to the `str` version after reading
+        the whole file.
+    - If `script` is a `str`, an `InputStream` is constructed from it.
+
+    Args:
+        script: The script to create a context for.
+        wrap_excs: If True, exceptions will be converted to Wizard exceptions (when
+            possible).
+
+    Returns:
+        A ParseWizardContext extracted from the given script.
+    """
+    from .error_strategy import WizardErrorStrategy
+
+    # Make a stream:
+    stream: InputStream
+    if isinstance(script, InputStream):
+        stream = script
+    elif isinstance(script, str):
+        stream = InputStream(script)
+    else:
+        if isinstance(script, Path):
+            with open(script, "rb") as fp:
+                data = fp.read()
+        else:
+            data = script.read()  # type: ignore
+        if isinstance(data, bytes):
+            encoding = chardet.detect(data)["encoding"]
+            text = data.decode(encoding)
+        else:
+            text = data
+        stream = InputStream(text)
+
+    # Create the lexer and disable console logs:
+    lexer = wizardLexer(stream)
+    lexer.removeErrorListener(ConsoleErrorListener.INSTANCE)
+
+    token_stream = CommonTokenStream(lexer)
+
+    # Create the parser with a custom error strategy:
+    parser = wizardParser(token_stream)
+    parser.removeErrorListener(ConsoleErrorListener.INSTANCE)
+    parser._errHandler = WizardErrorStrategy()
+
+    # Run the interpret:
+    if wrap_excs:
+        return wrap_exceptions(parser.parseWizard)
+    return parser.parseWizard()
+
+
+@overload
+def make_top_level_context(
+    script: Union[InputStream, Path, TextIO, str],
+    factory: WizardInterpreterContextFactory[ContextState],
+    state: ContextState,
+    *,
+    wrap_excs: bool = True,
+) -> WizardTopLevelContext[ContextState]: ...
+
+
+@overload
+def make_top_level_context(
+    script: Union[InputStream, Path, TextIO, str],
+    factory: WizardInterpreterContextFactory[WizardInterpreterState],
+    *,
+    wrap_excs: bool = True,
+) -> WizardTopLevelContext[WizardInterpreterState]: ...
+
+
+def make_top_level_context(
+    script: Union[InputStream, Path, TextIO, str],
+    factory: WizardInterpreterContextFactory[ContextState],
+    state: ContextState | None = None,
+    *,
+    wrap_excs: bool = True,
+) -> WizardTopLevelContext[ContextState]:
+    """
+    Create a WizardTopLevelContext from the given script.
+
+    Args:
+        script: The script to create a context for. See make_parse_wizard_context for
+            details on the possible types.
+        factory: The factory for the top-level context.
+        state: The state for the top-level context. If None, a WizardInterpreterState()
+            will be used.
+        **kwargs: Extra named parameters that are passed to `make_parse_wizard_context`.
+
+    Returns:
+        A ParseWizardContext extracted from the given script.
+    """
 
-from antlr4 import InputStream
+    ctx = make_parse_wizard_context(script, wrap_excs=wrap_excs)
 
-from .contexts import (
-    WizardInterpreterContext,
-    WizardInterpreterContextFactory,
-    WizardSelectManyContext,
-    WizardSelectOneContext,
-    WizardTerminationContext,
-    WizardTopLevelContext,
-)
-from .functions import make_basic_functions, make_manager_functions
-from .interpreter import WizardInterpreter
-from .manager import ManagerModInterface, ManagerUserInterface
-from .runner import (
-    WizardRunnerExpressionVisitor,
-    WizardRunnerKeywordVisitor,
-    WizardRunnerState,
-)
-from .severity import SeverityContext
-from .value import SubPackages
-
-
-class WizardScriptRunnerKeywordFactory(WizardRunnerKeywordVisitor):
-
-    """
-    Small extension of the runner keyword visitor to call requireVersions()
-    on a manager.
-    """
-
-    _manager: ManagerUserInterface
-
-    def __init__(
-        self,
-        manager: ManagerUserInterface,
-        subpackages: SubPackages,
-        severity: SeverityContext,
-    ):
-        super().__init__(subpackages, severity)
-        self._manager = manager
-
-    def visitRequireVersions(
-        self,
-        state: WizardRunnerState,
-        game_version: str,
-        script_extender_version: Optional[str],
-        graphics_extender_version: Optional[str],
-        wrye_bash_version: Optional[str],
-    ):
-        self._manager.requiresVersions(
-            game_version,
-            script_extender_version,
-            graphics_extender_version,
-            wrye_bash_version,
-        )
-
-
-class WizardScriptRunnerStatus(Enum):
-
-    # A 'Cancel' instruction was encountered:
-    CANCEL = auto()
-
-    # A 'Return' instruction was encountered:
-    RETURN = auto()
-
-    # The script was completely executed:
-    COMPLETE = auto()
-
-    # An error was encountered:
-    ERROR = auto()
-
-
-class WizardScriptRunner(
-    WizardInterpreter, ManagerModInterface, ManagerUserInterface, SeverityContext
-):
-
-    """
-    The WizardRunner is a high-level interface for the interpreter that
-    uses callbacks to interact with the user.
-
-    Implementations should inherit the WizardRunner class and implements
-    missing methods from the manager interfaces.
-    """
-
-    # Internal exceptions used to rewind / cancel at any point:
-    class RewindFlow(Exception):
-
-        """
-        Exception used to rewind a script execution when calling rewind().
-        """
-
-        context: WizardInterpreterContext
-
-        def __init__(self, context: WizardInterpreterContext):
-            self.context = context
-
-    class CancelFlow(Exception):
-
-        """
-        Exception used to cancel a script execution when calling abort().
-        """
-
-        ...
-
-    # The current context:
-    _ctx: WizardInterpreterContext
-
-    def __init__(self, subpackages: SubPackages = SubPackages()):
-        functions = make_basic_functions()
-        functions.update(make_manager_functions(self, self))
-
-        factory = WizardInterpreterContextFactory(
-            WizardRunnerExpressionVisitor(subpackages, functions, self),
-            WizardScriptRunnerKeywordFactory(self, subpackages, self),
-            self,
-        )
-
-        SeverityContext.__init__(self)
-        WizardInterpreter.__init__(self, factory)
-
-    def context(self) -> WizardInterpreterContext:
-        return self._ctx
-
-    def abort(self):
-        raise WizardScriptRunner.CancelFlow()
-
-    def rewind(self, context: WizardInterpreterContext):
-        raise WizardScriptRunner.RewindFlow(context)
-
-    def make_top_level_context(  # type: ignore
-        self,
-        script: Union[InputStream, Path, TextIO, str],
-        state: Optional[WizardRunnerState] = None,
-    ) -> WizardTopLevelContext[WizardRunnerState]:
-        if state is None:
-            state = WizardRunnerState()
-        return super().make_top_level_context(script, state)
-
-    def run(
-        self, script: Union[InputStream, Path, TextIO, str]
-    ) -> Tuple[WizardScriptRunnerStatus, WizardRunnerState]:
-        """
-        Run the script from the given input stream.
-
-        Args:
-            script: The script to read the script from. Can be a antlr4 stream,
-                a path to a script file, a string containing the script or a TextIO
-                object.
-
-        Returns:
-            A tuple (result, state) from running the script where state is the last
-            state of the interpreter and result the result.
-        """
-
-        # Run the interpret:
-        ctx: WizardInterpreterContext = self.make_top_level_context(script)
-
-        while True:
-
-            self._ctx = ctx
-
-            try:
-                if isinstance(ctx, WizardSelectOneContext):
-                    ctx = ctx.select(
-                        self.selectOne(ctx.description, ctx.options, ctx.default)
-                    )
-                elif isinstance(ctx, WizardSelectManyContext):
-                    ctx = ctx.select(
-                        self.selectMany(ctx.description, ctx.options, ctx.defaults)
-                    )
-                elif isinstance(ctx, WizardTerminationContext):
-                    if ctx.is_cancel():
-                        if self.cancel():
-                            return (WizardScriptRunnerStatus.CANCEL, ctx.state)
-                    elif ctx.is_return():
-                        if self.complete():
-                            return (WizardScriptRunnerStatus.RETURN, ctx.state)
-                    else:
-                        if self.complete():
-                            return (WizardScriptRunnerStatus.COMPLETE, ctx.state)
-
-                ctx = ctx.exec()
-
-            except WizardScriptRunner.RewindFlow as rfex:
-                ctx = rfex.context
-
-            except WizardScriptRunner.CancelFlow:
-                if self.cancel():
-                    return (WizardScriptRunnerStatus.CANCEL, ctx.state)
-
-            except Exception as ex:
-                self.error(ex)
-                return (WizardScriptRunnerStatus.ERROR, ctx.state)
+    if state is None:
+        # if state is None, the second overload matches so we are using the basic
+        # interpreter state
+        state = WizardInterpreterState()  # type: ignore
 
-        return (WizardScriptRunnerStatus.COMPLETE, ctx.state)
+    return WizardTopLevelContext(factory, ctx, None, state)
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/severity.py` & `bain_wizard_interpreter-1.0.4/src/wizard/severity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-# -*- encoding: utf-8 -*-
-
 from abc import abstractmethod
+from collections.abc import MutableMapping
 from enum import Enum, auto
-from typing import MutableMapping
 
 
 class Severity(Enum):
-
     ALLOW = auto()
     WARNING = auto()
     ERROR = auto()
 
 
 class Issue(Enum):
-
     # Indicates if multiple default values are allowed in SelectOne statement.
     MULTIPLE_DEFAULTS_IN_SELECT_ON = auto()
 
     # Indicates if using a non-set variable is allowed or not.
     USAGE_OF_NOTSET_VARIABLES = auto()
 
     # Indicates if case labels can be non-string and Identifier instead.
@@ -28,15 +24,14 @@
 
     # Select a sub-package or a plugin that does not exist:
     SELECT_MISSING_SUBPACKAGE = auto()
     SELECT_MISSING_PLUGIN = auto()
 
 
 class SeverityContext:
-
     _default_severity: Severity
     _context: MutableMapping[Issue, Severity] = {}
 
     def __init__(self):
         self._default_severity = Severity.WARNING
 
     @abstractmethod
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/state.py` & `bain_wizard_interpreter-1.0.4/src/wizard/state.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-# -*- encoding: utf-8 -*-
-
-from typing import Mapping, MutableMapping, TypeVar
+from collections.abc import Mapping, MutableMapping
+from typing import Any, Self, TypeVar
 
 from .value import Value
 
 
 class WizardInterpreterState:
-
     """
     State of the interpreter, stored in the context. This class can be
     inherited to use custom states that should implement a proper copy().
     """
 
     # The variables - The underlying mapping is mutable but is never
     # modified, except right after constructing the state:
-    _variables: MutableMapping[str, Value]
+    _variables: MutableMapping[str, Value[Any]]
 
-    def __init__(self, variables: Mapping[str, Value] = {}):
+    def __init__(self, variables: Mapping[str, Value[Any]] = {}):
         self._variables = dict(variables)
 
     @property
-    def variables(self) -> Mapping[str, Value]:
+    def variables(self) -> Mapping[str, Value[Any]]:
         """
         Returns:
             The variables in this state.
         """
         return self._variables
 
-    def copy(self) -> "WizardInterpreterState":
+    def set(self, name: str, value: Value[Any]):
+        self._variables[name] = value
+
+    def copy(self) -> Self:
         """
         Copy this state. This can be a mix between a shallow or a deep copy, the
         restriction is that modifying the returned state should not impact the
         current state.
 
         Returns:
             A copy of this state.
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/tweaks.py` & `bain_wizard_interpreter-1.0.4/src/wizard/tweaks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# -*- encoding: utf-8 -*-
-
-from typing import Any, List, Optional
+from collections.abc import Sequence
+from typing import Any
 
 
 class WizardINISetting:
-
     _filename: str
     _section: str
     _setting: str
 
     def __init__(self, filename: str, section: str, setting: str):
         self._filename = filename
         self._section = section
@@ -36,94 +34,92 @@
         Returns:
             The name of the setting.
         """
         return self._setting
 
 
 class WizardINISettingEdit(WizardINISetting):
-
     _value: Any
-    _comment: Optional[str]
+    _comment: str | None
 
     def __init__(
         self,
         filename: str,
         section: str,
         setting: str,
         value: Any,
-        comment: Optional[str] = None,
+        comment: str | None = None,
     ):
         super().__init__(filename, section, setting)
         self._value = value
         self._comment = comment
 
     @property
     def value(self) -> Any:
         """
         Returns:
             The new value for the setting.
         """
         return self._value
 
     @property
-    def comment(self) -> Optional[str]:
+    def comment(self) -> str | None:
         """
         Returns:
             The comment for the setting.
         """
         return self._comment
 
 
 class WizardINITweaks:
-
-    _disabled: List[WizardINISetting]
-    _modified: List[WizardINISettingEdit]
+    _disabled: list[WizardINISetting]
+    _modified: list[WizardINISettingEdit]
 
     def __init__(self):
         self._disabled = []
         self._modified = []
 
     @property
-    def disabled(self) -> List[WizardINISetting]:
+    def disabled(self) -> Sequence[WizardINISetting]:
         """
         Returns:
             The list of INI settings that have been disabled by the script.
         """
         return self._disabled
 
     @property
-    def modified(self) -> List[WizardINISettingEdit]:
+    def modified(self) -> Sequence[WizardINISettingEdit]:
         """
         Returns:
             The list of settings that have been created or modified by the script. May
             contain multiple edits for the same setting.
         """
         return self._modified
 
-    def files(self) -> List[str]:
+    def files(self) -> Sequence[str]:
         """
         Returns:
             The list of all files containing INI tweaks (either modified or disabled).
         """
         return sorted(
             set(m.filename for m in self._modified).union(
                 m.filename for m in self._disabled
             )
         )
 
-    def tweaks(self, file: str) -> List[WizardINISetting]:
+    def tweaks(self, file: str) -> Sequence[WizardINISetting]:
         """
         Args:
             file: The file to retrieve the tweaks for.
 
         Returns:
             The union of modified and disabled tweaks for the given file.
         """
         file = file.lower()
-        tweaks: List[WizardINISetting] = [
+        tweaks: list[WizardINISetting] = [
             m for m in self.modified if m.filename.lower() == file
         ]
         tweaks.extend(m for m in self.disabled if m.filename.lower() == file)
         return tweaks
 
     def __bool__(self) -> bool:
         """
```

### Comparing `bain-wizard-interpreter-1.0.3/wizard/value.py` & `bain_wizard_interpreter-1.0.4/src/wizard/value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# -*- encoding: utf-8 -*-
+from __future__ import annotations
 
 import operator
-from abc import abstractproperty
+from abc import abstractmethod
+from collections.abc import Iterable
 from enum import Enum, auto
 from pathlib import Path
-from typing import Callable, Generic, Iterable, List, Optional, Type, TypeVar, Union
+from typing import Any, Callable, Generic, Type, TypeAlias, TypeVar, cast
 
 
 class CaseFoldNamedObject:
-
     _name: str
 
-    def __init__(self, name: str):
+    def __init__(self, name: str | CaseFoldNamedObject):
+        if isinstance(name, CaseFoldNamedObject):
+            name = name.name
         self._name = name
 
     @property
     def name(self) -> str:
         """
         Returns:
             The name of the object.
@@ -55,29 +57,28 @@
         return self._name
 
     def __repr__(self) -> str:
         return repr(self._name)
 
 
 class Void:
-
     """
     Simple class representing the result of a function call without a return
     value.
     """
 
     pass
 
 
-class Plugin(CaseFoldNamedObject):
-    ...
+class Plugin(CaseFoldNamedObject): ...
 
 
 class SubPackage(CaseFoldNamedObject):
-    @abstractproperty
+    @property
+    @abstractmethod
     def files(self) -> Iterable[str]:
         pass
 
     @staticmethod
     def is_plugin(name: str) -> bool:
         """
         Check if the given name corresponds to a plugin.
@@ -90,38 +91,40 @@
         """
         return name.endswith(".esp") or name.endswith(".esm") or name.endswith(".esl")
 
     def plugins(self) -> Iterable[Plugin]:
         return (Plugin(Path(file).name) for file in self.files if self.is_plugin(file))
 
 
-class SubPackages(List[SubPackage]):
-
+class SubPackages(list[SubPackage]):
     """
     Class to wrap the 'SubPackages' variable.
     """
 
     ...
 
 
-class VariableType(Enum):
+ValueType = TypeVar("ValueType", Void, SubPackage, SubPackages, bool, int, float, str)
+AnyValueType: TypeAlias = Void | SubPackage | SubPackages | bool | int | float | str
 
+
+class VariableType(Enum):
     BOOL = auto()
     INTEGER = auto()
     FLOAT = auto()
     STRING = auto()
 
     VOID = auto()
 
     # Note: This is used only for SubPackages and item in SubPackages.
     LIST_SUBPACKAGES = auto()
     SUBPACKAGE = auto()
 
     @staticmethod
-    def from_pytype(pytype: Type) -> "VariableType":
+    def from_pytype(pytype: Type[ValueType]) -> VariableType:
         if pytype is Void:
             return VariableType.VOID
         if issubclass(pytype, SubPackages):
             return VariableType.LIST_SUBPACKAGES
         if issubclass(pytype, SubPackage):
             return VariableType.SUBPACKAGE
         if pytype is bool:
@@ -140,36 +143,28 @@
 
         if self is VariableType.SUBPACKAGE:
             return "SubPackage"
 
         return super().__str__().lower().split(".")[-1]
 
 
-# Union of possible type for Wizard value:
-WizardValueType = Union[bool, int, float, str, SubPackage, SubPackages, Void]
-
-
-ValueType = TypeVar("ValueType", bound=WizardValueType)
-
-
 class Value(Generic[ValueType]):
-
     """
     Represent a value of a given type, that can be a constant or the result of
     a complex expression.
 
     Value expose operators from the BAIN Wizard specification with proper type
     checking so you can use them directly.
     """
 
     _value: ValueType
 
-    def __init__(self, value: ValueType):
+    def __init__(self, value: ValueType | None):
         if value is None:
-            value = Void()
+            value = cast(ValueType, Void())
         self._type = VariableType.from_pytype(type(value))
         self._value = value
 
     @property
     def type(self) -> VariableType:
         """
         Returns:
@@ -188,124 +183,126 @@
     def value(self) -> ValueType:
         """
         Returns:
             The value of this constant.
         """
         return self._value
 
-    def __pos__(self) -> "Value":
+    def __pos__(self) -> Value[ValueType]:
         if not isinstance(self._value, (int, float)):
             raise TypeError(
                 f"Cannot use plus operator on variable of type {self._type}."
             )
         return Value(self._value)
 
-    def __neg__(self) -> "Value":
-        if not isinstance(self._value, (int, float)):
+    def __neg__(self) -> Value[ValueType]:
+        if not isinstance(self._value, (int, float)) or isinstance(self._value, bool):
             raise TypeError(
                 f"Cannot use minus operator on variable of type {self._type}."
             )
         return Value(-self._value)
 
-    def __add__(self, other: "Value") -> "Value":
+    def __add__(
+        self: Value[Any], other: Value[Any]
+    ) -> Value[int] | Value[float] | Value[str]:
         if (
             not isinstance(self._value, (int, float, str))
             or not isinstance(other._value, (int, float, str))
             or isinstance(self._value, str) != isinstance(other._value, str)
         ):
             raise TypeError(f"Cannot add values of types {self._type}, {other._type}.")
         return Value(self._value + other._value)  # type: ignore
 
-    def __sub__(self, other: "Value") -> "Value":
+    def __sub__(self: Value[Any], other: Value[Any]) -> Value[int] | Value[float]:
         if not isinstance(self._value, (int, float)) or not isinstance(
             other._value, (int, float)
         ):
             raise TypeError("Cannot substract non-numeric values.")
         return Value(self._value - other._value)
 
-    def __mul__(self, other: "Value") -> "Value":
+    def __mul__(self: Value[Any], other: Value[Any]) -> Value[int] | Value[float]:
         if not isinstance(self._value, (int, float)) or not isinstance(
             other._value, (int, float)
         ):
             raise TypeError("Cannot multiply non-numeric values.")
         return Value(self._value * other._value)
 
-    def __div__(self, other: "Value") -> "Value":
+    def __div__(self: Value[Any], other: Value[Any]) -> Value[int] | Value[float]:
         if not isinstance(self._value, (int, float)) or not isinstance(
             other._value, (int, float)
         ):
             raise TypeError("Cannot divide non-numeric values.")
         return Value(self._value / other._value)
 
-    def __pow__(self, other: "Value") -> "Value":
+    def __pow__(self: Value[Any], other: Value[Any]) -> Value[int] | Value[float]:
         if not isinstance(self._value, (int, float)) or not isinstance(
             other._value, (int, float)
         ):
             raise TypeError("Cannot raise non-numeric values.")
         return Value(self._value**other._value)
 
-    def __mod__(self, other: "Value") -> "Value":
+    def __mod__(self: Value[Any], other: Value[Any]) -> Value[int] | Value[float]:
         if not isinstance(self._value, (int, float)) or not isinstance(
             other._value, (int, float)
         ):
             raise TypeError("Cannot modulo non-numeric values.")
         return Value(self._value % other._value)
 
-    def logical_not(self) -> "Value":
+    def logical_not(self) -> Value[bool]:
         return Value(not self._value)
 
-    def equals(self, other: "Value") -> "Value":
+    def equals(self: Value[Any], other: Value[Any]) -> Value[bool]:
         return Value(self._value == other._value)
 
-    def not_equals(self, other: "Value") -> "Value":
+    def not_equals(self: Value[Any], other: Value[Any]) -> Value[bool]:
         return Value(self._value != other._value)
 
-    def __or__(self, other: "Value") -> "Value":
-        return Value(self._value or other._value)
+    def __or__(self, other: Value[Any]) -> Value[bool]:
+        return Value(bool(self._value or other._value))
 
-    def __and__(self, other: "Value") -> "Value":
+    def __and__(self, other: Value[Any]) -> Value[bool]:
         return Value(self._value and other._value)
 
-    def __gt__(self, other: "Value") -> "Value":
+    def __gt__(self: Value[Any], other: Value[Any]) -> Value[bool]:
         if isinstance(self._value, (int, float)) and isinstance(
             other._value, (int, float)
         ):
             return Value(self._value > other._value)
         if isinstance(self._value, str) and isinstance(other._value, str):
             return Value(self._value > other._value)
         raise TypeError(f"Cannot compare values of types {self._type}, {other._type}.")
 
-    def __ge__(self, other: "Value") -> "Value":
+    def __ge__(self: Value[Any], other: Value[Any]) -> Value[bool]:
         if isinstance(self._value, (int, float)) and isinstance(
             other._value, (int, float)
         ):
             return Value(self._value >= other._value)
         if isinstance(self._value, str) and isinstance(other._value, str):
             return Value(self._value >= other._value)
         raise TypeError(f"Cannot compare values of types {self._type}, {other._type}.")
 
-    def __lt__(self, other: "Value") -> "Value":
+    def __lt__(self: Value[Any], other: Value[Any]) -> Value[bool]:
         if isinstance(self._value, (int, float)) and isinstance(
             other._value, (int, float)
         ):
             return Value(self._value < other._value)
         if isinstance(self._value, str) and isinstance(other._value, str):
             return Value(self._value < other._value)
         raise TypeError(f"Cannot compare values of types {self._type}, {other._type}.")
 
-    def __le__(self, other: "Value") -> "Value":
+    def __le__(self: Value[Any], other: Value[Any]) -> Value[bool]:
         if isinstance(self._value, (int, float)) and isinstance(
             other._value, (int, float)
         ):
             return Value(self._value <= other._value)
         if isinstance(self._value, str) and isinstance(other._value, str):
             return Value(self._value <= other._value)
         raise TypeError(f"Cannot compare values of types {self._type}, {other._type}.")
 
-    def contains(self, item: "Value", case_insensitive: bool = False) -> "Value":
+    def contains(self, item: Value[Any], case_insensitive: bool = False) -> Value[bool]:
         if not isinstance(self._value, (SubPackage, SubPackages)):
             raise TypeError(f"Cannot iterate variable of type {self._type}.")
 
         if not isinstance(item._value, (str, SubPackage)):
             raise TypeError(f"Cannot check presence of variable of type {self._type}.")
 
         if isinstance(item._value, SubPackage):
@@ -324,64 +321,63 @@
             if case_insensitive:
                 istr = istr.lower()
             if item._value == istr:
                 return Value(True)
 
         return Value(False)
 
-    def __getitem__(self, index: "Value") -> "Value":
+    def __getitem__(self, index: Value[Any]) -> Value[str] | Value[SubPackage]:
         if not isinstance(self._value, (str, SubPackage, SubPackages)):
             raise TypeError(f"Cannot index variable of type {self._type}.")
         if not isinstance(index._value, (int)):
             raise TypeError(f"Cannot index with variable of type {index._type}.")
 
-        value: Union[str, SubPackages]
+        value: str | SubPackages
         if isinstance(self._value, SubPackage):
             value = self._value.name
         else:
             value = self._value
 
         try:
-            return Value(value[index._value])
-        except IndexError:
-            raise IndexError(index._value)
+            return Value(value[index._value])  # type: ignore
+        except IndexError as err:
+            raise IndexError(index._value) from err
 
     def slice(
-        self, start: Optional["Value"], end: Optional["Value"], step: Optional["Value"]
-    ) -> "Value":
-
+        self, start: Value[Any] | None, end: Value[Any] | None, step: Value[Any] | None
+    ) -> Value[str]:
         if not isinstance(self._value, str):
             raise TypeError(f"Cannot access slice of variable of type {self._type}.")
 
         for v in (start, end, step):
             if v is not None and not isinstance(v.value, int):
                 raise TypeError(f"Cannot index with variable of type {v.type}.")
 
         return Value(
             self._value[
                 slice(*(None if v is None else v.value for v in (start, end, step)))
             ]
         )
 
-    def __iter__(self) -> Iterable["Value"]:
+    def __iter__(self) -> Iterable[Value[SubPackage]] | Iterable[Value[str]]:
         if not isinstance(self._value, (SubPackage, SubPackages)):
             raise TypeError(f"Cannot iterate variable of type {self._type}.")
 
         it: Iterable[str]
         if isinstance(self._value, SubPackages):
             it = (s.name for s in self._value)
         else:
             it = self._value.files
 
         return (Value(x) for x in it)
 
     # Those operations are not "Wizardly", i.e. they make sense in Python:
 
     def __eq__(self, other: object) -> bool:
-        value: Value
+        value: Value[Any]
         if not isinstance(other, Value):
             value = Value(other)  # type: ignore
         else:
             value = other
 
         if self.is_void() and value.is_void():
             return True
```

