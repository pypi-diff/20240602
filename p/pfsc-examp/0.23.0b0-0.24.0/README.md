# Comparing `tmp/pfsc-examp-0.23.0b0.tar.gz` & `tmp/pfsc_examp-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfsc-examp-0.23.0b0.tar", last modified: Thu Jan 19 20:31:46 2023, max compression
+gzip compressed data, was "pfsc_examp-0.24.0.tar", last modified: Sun Jun  2 18:47:09 2024, max compression
```

## Comparing `pfsc-examp-0.23.0b0.tar` & `pfsc_examp-0.24.0.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-01-19 20:31:46.129157 pfsc-examp-0.23.0b0/
--rw-r--r--   0 skieffer   (501) staff       (20)    11359 2023-01-19 18:19:45.000000 pfsc-examp-0.23.0b0/LICENSE
--rw-r--r--   0 skieffer   (501) staff       (20)       71 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/NOTICE
--rw-r--r--   0 skieffer   (501) staff       (20)      434 2023-01-19 20:31:46.129271 pfsc-examp-0.23.0b0/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)       48 2023-01-19 18:19:45.000000 pfsc-examp-0.23.0b0/README.md
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-01-19 20:31:46.120041 pfsc-examp-0.23.0b0/pfsc_examp/
--rw-r--r--   0 skieffer   (501) staff       (20)     6873 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/__init__.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-01-19 20:31:46.122461 pfsc-examp-0.23.0b0/pfsc_examp/calculate/
--rw-r--r--   0 skieffer   (501) staff       (20)     2527 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/calculate/__init__.py
--rw-r--r--   0 skieffer   (501) staff       (20)     3997 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/calculate/server_calc.py
--rw-r--r--   0 skieffer   (501) staff       (20)     8130 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/canon_arithmeticus.py
--rw-r--r--   0 skieffer   (501) staff       (20)     1957 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/config.py
--rw-r--r--   0 skieffer   (501) staff       (20)     1684 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/contexts.py
--rw-r--r--   0 skieffer   (501) staff       (20)     8783 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/display.py
--rw-r--r--   0 skieffer   (501) staff       (20)     3130 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/excep.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-01-19 20:31:46.123225 pfsc-examp-0.23.0b0/pfsc_examp/parameters/
--rw-r--r--   0 skieffer   (501) staff       (20)     2421 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parameters/__init__.py
--rw-r--r--   0 skieffer   (501) staff       (20)    24991 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parameters/base.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-01-19 20:31:46.126125 pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/
--rw-r--r--   0 skieffer   (501) staff       (20)     1711 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/__init__.py
--rw-r--r--   0 skieffer   (501) staff       (20)     4706 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/divisor.py
--rw-r--r--   0 skieffer   (501) staff       (20)     6878 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/integer.py
--rw-r--r--   0 skieffer   (501) staff       (20)     7539 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/numberfield.py
--rw-r--r--   0 skieffer   (501) staff       (20)     6871 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/prime.py
--rw-r--r--   0 skieffer   (501) staff       (20)     4812 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/primeideal.py
--rw-r--r--   0 skieffer   (501) staff       (20)     5857 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/primres.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-01-19 20:31:46.128851 pfsc-examp-0.23.0b0/pfsc_examp/parse/
--rw-r--r--   0 skieffer   (501) staff       (20)        0 2023-01-19 18:32:23.000000 pfsc-examp-0.23.0b0/pfsc_examp/parse/__init__.py
--rw-r--r--   0 skieffer   (501) staff       (20)     3923 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parse/algebraic.py
--rw-r--r--   0 skieffer   (501) staff       (20)     3882 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parse/display.py
--rw-r--r--   0 skieffer   (501) staff       (20)     1503 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parse/excep.py
--rw-r--r--   0 skieffer   (501) staff       (20)     4420 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parse/polynom.py
--rw-r--r--   0 skieffer   (501) staff       (20)     5204 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parse/sympy_allowed.py
--rw-r--r--   0 skieffer   (501) staff       (20)     2781 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/parse/util.py
--rw-r--r--   0 skieffer   (501) staff       (20)     1684 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pfsc_examp/util.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-01-19 20:31:46.121863 pfsc-examp-0.23.0b0/pfsc_examp.egg-info/
--rw-r--r--   0 skieffer   (501) staff       (20)      434 2023-01-19 20:31:46.000000 pfsc-examp-0.23.0b0/pfsc_examp.egg-info/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)      991 2023-01-19 20:31:46.000000 pfsc-examp-0.23.0b0/pfsc_examp.egg-info/SOURCES.txt
--rw-r--r--   0 skieffer   (501) staff       (20)        1 2023-01-19 20:31:46.000000 pfsc-examp-0.23.0b0/pfsc_examp.egg-info/dependency_links.txt
--rw-r--r--   0 skieffer   (501) staff       (20)      150 2023-01-19 20:31:46.000000 pfsc-examp-0.23.0b0/pfsc_examp.egg-info/requires.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       11 2023-01-19 20:31:46.000000 pfsc-examp-0.23.0b0/pfsc_examp.egg-info/top_level.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       81 2023-01-19 20:31:13.000000 pfsc-examp-0.23.0b0/pyproject.toml
--rw-r--r--   0 skieffer   (501) staff       (20)      682 2023-01-19 20:31:46.129862 pfsc-examp-0.23.0b0/setup.cfg
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:47:09.258088 pfsc_examp-0.24.0/
+-rw-r--r--   0 skieffer   (501) staff       (20)    11359 2023-11-13 20:16:15.000000 pfsc_examp-0.24.0/LICENSE
+-rw-r--r--   0 skieffer   (501) staff       (20)       71 2023-11-13 20:16:15.000000 pfsc_examp-0.24.0/NOTICE
+-rw-r--r--   0 skieffer   (501) staff       (20)      825 2024-06-02 18:47:09.258026 pfsc_examp-0.24.0/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)       48 2023-11-13 20:16:15.000000 pfsc_examp-0.24.0/README.md
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:47:09.251628 pfsc_examp-0.24.0/pfsc_examp/
+-rw-r--r--   0 skieffer   (501) staff       (20)     7100 2024-06-01 20:32:56.000000 pfsc_examp-0.24.0/pfsc_examp/__init__.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:47:09.252621 pfsc_examp-0.24.0/pfsc_examp/calculate/
+-rw-r--r--   0 skieffer   (501) staff       (20)     2527 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/calculate/__init__.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     3997 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/calculate/server_calc.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     8130 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/canon_arithmeticus.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     1957 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/config.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     1684 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/contexts.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     8783 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/display.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     3045 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/excep.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:47:09.252978 pfsc_examp-0.24.0/pfsc_examp/parameters/
+-rw-r--r--   0 skieffer   (501) staff       (20)     2421 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parameters/__init__.py
+-rw-r--r--   0 skieffer   (501) staff       (20)    24652 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parameters/base.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:47:09.255048 pfsc_examp-0.24.0/pfsc_examp/parameters/types/
+-rw-r--r--   0 skieffer   (501) staff       (20)     1711 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parameters/types/__init__.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     4693 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parameters/types/divisor.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     6837 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parameters/types/integer.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     7470 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parameters/types/numberfield.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     6787 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parameters/types/prime.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     4741 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parameters/types/primeideal.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     5798 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parameters/types/primres.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:47:09.257018 pfsc_examp-0.24.0/pfsc_examp/parse/
+-rw-r--r--   0 skieffer   (501) staff       (20)        0 2023-11-13 20:16:15.000000 pfsc_examp-0.24.0/pfsc_examp/parse/__init__.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     3924 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parse/algebraic.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     3882 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parse/display.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     1503 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parse/excep.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     4420 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parse/polynom.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     5314 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parse/sympy_allowed.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     2781 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/parse/util.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     1684 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/pfsc_examp/util.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:47:09.257546 pfsc_examp-0.24.0/pfsc_examp.egg-info/
+-rw-r--r--   0 skieffer   (501) staff       (20)      825 2024-06-02 18:47:09.000000 pfsc_examp-0.24.0/pfsc_examp.egg-info/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)     1038 2024-06-02 18:47:09.000000 pfsc_examp-0.24.0/pfsc_examp.egg-info/SOURCES.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)        1 2024-06-02 18:47:09.000000 pfsc_examp-0.24.0/pfsc_examp.egg-info/dependency_links.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)      155 2024-06-02 18:47:09.000000 pfsc_examp-0.24.0/pfsc_examp.egg-info/requires.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       11 2024-06-02 18:47:09.000000 pfsc_examp-0.24.0/pfsc_examp.egg-info/top_level.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       81 2023-11-13 20:16:15.000000 pfsc_examp-0.24.0/pyproject.toml
+-rw-r--r--   0 skieffer   (501) staff       (20)      688 2024-06-02 18:47:09.258329 pfsc_examp-0.24.0/setup.cfg
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:47:09.257335 pfsc_examp-0.24.0/tests/
+-rw-r--r--   0 skieffer   (501) staff       (20)     5461 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/tests/test_display.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     4321 2024-06-01 20:16:54.000000 pfsc_examp-0.24.0/tests/test_parameters.py
```

### Comparing `pfsc-examp-0.23.0b0/LICENSE` & `pfsc_examp-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/__init__.py` & `pfsc_examp-0.24.0/pfsc_examp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -26,15 +26,15 @@
 from pfsc_examp.parameters.base import Parameter
 from pfsc_examp.display import make_disp
 from pfsc_examp.excep import ExampError, MalformedParamRawValue
 from pfsc_examp.util import adapt
 from pfsc_util.imports import from_import
 
 
-__version__ = "0.23.0b0"
+__version__ = "0.24.0"
 
 
 def make_examp_generator_obj_from_js(info, pane_id):
     """
     This is the factory function for Parameters and ExampDisplays, which is
     intended to be invoked from the JS side, in pfsc-ise.
 
@@ -85,14 +85,19 @@
     MALFORMED_PARAM_RAW_VALUE = 193
     EXAMP_ERROR = 4
     # Again, we want to be sure we're using an error code that doesn't collide
     # with other codes in pfsc-server, so we've set this one to be the same
     # over there.
     CONTROLLED_EVALUATION_EXCEPTION = 279
 
+    # Don't use anything in the range 10,000 - 10,999.
+    # This range is reserved for use by mathworker.js, on the client side.
+    RESERVED_FOR_MATHWORKER_ON_JS_SIDE_0 = 10000
+    RESERVED_FOR_MATHWORKER_ON_JS_SIDE_1 = 10999
+
 
 def rebuild_examp_generator_from_js(obj, value=None, write_html=False):
     to_js = from_import('pyodide', 'to_js')
     d = {
         'err_lvl': ErrCode.UNKNOWN,
         'err_msg': 'unknown error',
     }
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/calculate/__init__.py` & `pfsc_examp-0.24.0/pfsc_examp/calculate/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/calculate/server_calc.py` & `pfsc_examp-0.24.0/pfsc_examp/calculate/server_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/canon_arithmeticus.py` & `pfsc_examp-0.24.0/pfsc_examp/canon_arithmeticus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/config.py` & `pfsc_examp-0.24.0/pfsc_examp/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/contexts.py` & `pfsc_examp-0.24.0/pfsc_examp/contexts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/display.py` & `pfsc_examp-0.24.0/pfsc_examp/display.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/excep.py` & `pfsc_examp-0.24.0/pfsc_examp/excep.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -63,19 +63,14 @@
 
 
 class MissingParamArgType(ExampError):
     """No type was declared for a parameter arg"""
     pass
 
 
-class MissingName(ExampError):
-    """Parameter defn missing name arg."""
-    pass
-
-
 class MalformedExampImport(ExampError):
     """Import into a display was malformed."""
     pass
 
 
 class MissingExport(ExampError):
     """Display does not define an expected export."""
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parameters/__init__.py` & `pfsc_examp-0.24.0/pfsc_examp/parameters/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parameters/base.py` & `pfsc_examp-0.24.0/pfsc_examp/parameters/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -26,15 +26,14 @@
 from pfsc_examp.parse.excep import ParsingExcep
 from pfsc_examp.excep import (
     MissingParamArgError,
     MissingParameterError,
     MalformedParamRawValue,
     UnexpectedParamArgError,
     UnexpectedParamArgTypeError,
-    MissingName,
     UnresolvedParamArgError,
     MissingParamArgType,
 )
 from pfsc_examp.util import adapt
 from pfsc_util.imports import from_import
 
 
@@ -118,36 +117,32 @@
 
 
 class Parameter(ParametricValued):
     """
     The abstract base class for all parameter types.
     """
 
-    def __init__(self, parent, name,
-                 default=None, tex=None, descrip=None, params=None,
+    def __init__(self, parent, tex,
+                 default=None, descrip=None, params=None,
                  args=None, last_raw=None):
         """
         :param parent: reference to a governing object. Could be a
           PyodideWidgetStandIn when operating in Pyodide, or a ParamWidget when
           operating in pfsc-server.
 
-        :param name: (str) the name by which the parameter is known. Often
-          coincident with the desired TeX string.
+        :param tex: string to be used in TeX representations.
 
         :param default: some specification of a default value for this parameter.
           May be of various types; it is up to the subclass to interpret.
           If specified, will be passed through the same method (build_from_raw)
           as any user-selected value that may come down from the client side.
 
           May be left unspecified (None), and then the subclass's auto_build
           method will be engaged at build time.
 
-        :param tex: string to be used in TeX representations; if left None,
-          self.name will be used instead.
-
         :param descrip: optional string giving a textual description of this
           parameter, for the benefit of users; however, it is more common to
           let the description instead be generated by the subclass's
           auto_descrip method.
 
         :param params: dict mapping local names to libpaths of other parameters.
           The names appearing here may then occur within mathematical expressions
@@ -172,22 +167,18 @@
 
         :param last_raw: useful when rebuilding a parameter that has already
           been in use, in the ISE. You can pass the most recent raw value that
           this parameter has taken on, and it will be recorded as such here. In
           particular, it will take precedence over `self.default` when we build.
         """
         self.parent = parent
-        if not name:
-            raise MissingName
-        self.name = name
+        self.tex = tex
         self.default = default
         self.last_attempted_raw_value = last_raw
-        if tex is None:
-            tex = name
-        self.tex = tex
+
         self.descrip = descrip
         self.given_args = args or {}
         # Dict in which param name points to Parameter instance:
         self.resolved_params = {k: self.parent.get_generator(v)
                                 for k, v in (params or {}).items()}
         # Dict in which arg name points to Valued instance:
         self.resolved_args = self.resolve_args(self.given_args)
@@ -355,15 +346,14 @@
         Subclasses decide how this works in their `self.auto_build()` method.
         One common pattern is to pick a raw value, and pass it to
         `self.build_from_raw()`.
 
         There are optional prebuild and postbuild hooks that subclasses may
         override.
         """
-        #print(f'{self.name}: raw: {raw}, last: {self.last_attempted_raw_value}, default: {self.default}')
         raw = adapt(raw)
         if raw is not None:
             self.last_attempted_raw_value = raw
         self._value = None
 
         self.check_value_types()
         self.prebuild()
@@ -495,16 +485,18 @@
             Python has a `__globals__` attribute, through which all built-ins (incl
             `exec`) can be reached.)
 
             Instead, use the parsers defined under `pfsc.examp.parameters.parse`.
             If the parser you need isn't defined there yet, please consider writing
             it and contributing via pull request.
 
-        @param name: the name of the argument
-        @param raw: the raw value of the argument
+        @param name: the name of the argument.
+            Note: Although `name` is not used in this method, it may well be used in
+            subclass overrides of this method.
+        @param raw: the raw value of the argument.
 
         @return: an instance of `Valued`, or `None`
         """
         if isinstance(raw, (bool, int, float)):
             return NonParamValue(SS(raw))
 
         if isinstance(raw, str):
@@ -566,19 +558,21 @@
         Should honor `self.parent.context` when choosing phraseology.
 
         :param include_value: e.g. "$p$ a prime" if False,
           but "$p = 7$ a prime" if True.
         :param editable: only meaningful if `include_value` is True.
           In that case, `editable` True should yield e.g.
 
-            "$p$ <span class="edit_me">&nbsp;$= 7$</span> a prime"
+            "$p$ <span class="param_val">&nbsp;$= 7$</span> a prime"
 
           so that it's easy to edit the value on the client-side.
 
         :return: the description string
+
+        See Also: write_name_and_value()
         """
         raise NotImplementedError
 
     def write_chooser_widget(self):
         """
         Write HTML to describe the client-side chooser widget with which users
         may choose new values for this parameter.
@@ -587,32 +581,33 @@
 
         :return: HTML string
         """
         raise NotImplementedError
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-def write_radio_panel_chooser_widget(name, descrip, code_and_text, selected=None):
+
+def write_radio_panel_chooser_widget(descrip, code_and_text, selected=None):
     """
-    :param name: the name of the parameter (e.g. 'frp')
     :param descrip: the parameter's description (e.g. '$\\mathfrak{p}$ a prime ideal')
     :param code_and_text: list of pairs (c, t) in which t is the text that should
       appear on the button, e.g. '$(13, x^2 + 3 x + 1)$' and c the code that
       should be passed to the server when this option is selected,
       e.g. '0'. They can be strings, or anything else that formats to the
       desired string.
     :param selected: the code of the selected button
     :return: HTML string for the chooser widget
     """
     context = {}
     context.update(locals())
     return radio_panel_chooser_widget_template.render(context)
 
+
 radio_panel_chooser_widget_template = jinja2.Template("""
-<div class="chooser radio_panel_chooser" name="{{ name }}">
+<div class="chooser radio_panel_chooser">
     <div class="heading">{{ descrip }}</div>
     <div class="error_display"></div>
     <div class="radio_panel">
         {% for c, t in code_and_text %}
             {% if c == selected %}
                 <div tabindex="0" value="{{ c }}" display="{{ t }}" class="radio_panel_button rpb_selected">{{ t }}</div>
             {% else %}
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/__init__.py` & `pfsc_examp-0.24.0/pfsc_examp/parameters/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/divisor.py` & `pfsc_examp-0.24.0/pfsc_examp/parameters/types/divisor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -42,15 +42,15 @@
 
     Value type: Integer
 
     Default: int
 
     Args:
         Required:
-            dividing: int
+            dividing: int-valued
                 The number of which this is a divisor.
         Optional:
             sign: {-1, 0, 1}, default=1
                 1 if you want only positive divisors
                 -1 if you want only negative divisors
                 0 if you allow both positive and negative divisors
 
@@ -66,31 +66,31 @@
             'sign': {
                 'type': (One, Zero, NegativeOne,),
                 'default_cooked': Integer(1),
             },
         }
     }
 
-    def __init__(self, parent, name=None,
-                 default=None, tex=None, descrip=None, params=None,
+    def __init__(self, parent, tex=None,
+                 default=None, descrip=None, params=None,
                  args=None, last_raw=None, **other):
-        super().__init__(parent, name, default, tex, descrip, params, args, last_raw)
+        super().__init__(parent, tex, default, descrip, params, args, last_raw)
         self.divisors = []
         self.dividing = None
         self.sign = None
 
     def prebuild(self):
         # Store args as attributes
         self.dividing = self.resolved_args['dividing']
         self.sign = self.resolved_args['sign']
         # Compute all the divisors.
         n = self.dividing.value
         c = calculate(divisor_count, n)
         if c > 200:  # FIXME: make such upper bounds configurable.
-            msg = f'Parameter {self.name} has too many notes, er divisors.'
+            msg = f'Parameter {self.getLibpath()} has too many notes, er divisors.'
             raise MalformedParamRawValue(msg, self)
         self.divisors = calculate(divisors, n)
         s = self.sign.value
         if s == 0:
             self.divisors = list(reversed([-d for d in self.divisors])) + self.divisors
         elif s == -1:
             self.divisors = list(reversed([-d for d in self.divisors]))
@@ -111,10 +111,10 @@
         return '%s a divisor of $%s$' % (
             self.write_name_and_value(include_value, editable),
             self.dividing
         )
 
     def write_chooser_widget(self):
         return write_radio_panel_chooser_widget(
-            self.name, self.auto_descrip(), zip(self.divisors, self.divisors),
+            self.auto_descrip(), zip(self.divisors, self.divisors),
             self.value
         )
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/integer.py` & `pfsc_examp-0.24.0/pfsc_examp/parameters/types/integer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -34,45 +34,45 @@
     Value type: Integer
 
     Default: int
 
     Args:
       Required: None.
       Optional:
-        coprime_to: int
+        coprimeTo: int-valued
             Must be coprime to this.
-        dividing: int
+        dividing: int-valued
             Must divide this.
-        gt: int
+        gt: int-valued
             Must be greater than this.
-        lt: int
+        lt: int-valued
             Must be less than this.
     """
     
     arg_spec = {
         "OPT": {
-            'coprime_to': {
+            'coprimeTo': {
                 'type': Integer,
             },
             'dividing': {
                 'type': Integer,
             },
             'gt': {
                 'type': Integer,
             },
             'lt': {
                 'type': Integer,
             },
         }
     }
 
-    def __init__(self, parent, name=None,
-                 default=None, tex=None, descrip=None, params=None,
+    def __init__(self, parent, tex=None,
+                 default=None, descrip=None, params=None,
                  args=None, last_raw=None, **other):
-        super().__init__(parent, name, default, tex, descrip, params, args, last_raw)
+        super().__init__(parent, tex, default, descrip, params, args, last_raw)
 
     def get_name_for_extra(self, predicate_name):
         a = self.resolved_args.get(predicate_name, None)
         if a is None:
             return None
         else:
             return str(a)
@@ -87,20 +87,20 @@
         n = self.check_int(raw)
 
         # Note: when formatting error messages, we use the _name_ of the parameter
         # to which this one is supposed to relate in a given way; not the current
         # value. This is more informative for the user.
 
         D = self.get_arg_value('dividing')
-        C = self.get_arg_value('coprime_to')
+        C = self.get_arg_value('coprimeTo')
         G = self.get_arg_value('gt')
         L = self.get_arg_value('lt')
 
         D_name = self.get_name_for_extra('dividing')
-        C_name = self.get_name_for_extra('coprime_to')
+        C_name = self.get_name_for_extra('coprimeTo')
         G_name = self.get_name_for_extra('gt')
         L_name = self.get_name_for_extra('lt')
 
         if D is not None and D % n != 0:
             raise MalformedParamRawValue(f'Must divide ${D_name}$.', self)
 
         if C is not None and calculate(igcd, C, n) != 1:
@@ -113,15 +113,15 @@
             raise MalformedParamRawValue(f'Must be less than ${L_name}$.', self)
 
         return Integer(n)
 
     def auto_descrip(self, include_value=True, editable=True):
         # Start by getting any optional, related parameters.
         dividing_str = self.get_name_for_extra('dividing')
-        coprime_str = self.get_name_for_extra('coprime_to')
+        coprime_str = self.get_name_for_extra('coprimeTo')
         lb_str = self.get_name_for_extra('gt')
         ub_str = self.get_name_for_extra('lt')
 
         # Build the symbolic part
         symbolic_part = self.write_name_and_value(include_value=include_value, editable=editable)
         if not include_value:
             # If we do not want to include the value, then the symbolic
@@ -164,27 +164,26 @@
             if 0 < i == N - 1:
                 final += 'and '
             final += p
         return final
 
     def write_chooser_widget(self):
         return write_int_chooser_widget(
-            self.name,
             self.auto_descrip(),
             current_value=self.value
         )
 
 
 int_chooser_widget_template = jinja2.Template("""
-<div class="chooser int_chooser" name="{{ name }}">
+<div class="chooser int_chooser">
     <div class="heading">{{ descrip }}</div>
     <div class="error_display"></div>
     <input class="textfield" type="text" placeholder="Integer" value="{{current_value}}"/>
 </div>
 """)
 
 
-def write_int_chooser_widget(name, descrip, current_value):
+def write_int_chooser_widget(descrip, current_value):
     context = {}
     context.update(locals())
     return int_chooser_widget_template.render(context)
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/numberfield.py` & `pfsc_examp-0.24.0/pfsc_examp/parameters/types/numberfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -56,15 +56,15 @@
                 field; otherwise, we only describe the field as a quotient
                 mod a polynomial.
             var: str
                 Symbol name to use for the variable in the field's defining,
                 irreducible polynomial.
                 If not supplied, we use `x` for `cyc(n)`, or the
                 given variable for polynomials given explicitly.
-            root_idx: int
+            rootIdx: int
                 Root index, indicating which root of the minimal polynomial to
                 use as primitive element for the field. This is passed to
                 SymPy's `CRootOf`. Real roots come first, in increasing order,
                 followed by complex roots, which are sorted first by real part
                 (increasing) and then by imaginary part (increasing).
                 If not supplied, we use -1.
     """
@@ -73,25 +73,25 @@
         "OPT": {
             'gen': {
                 'type': Symbol,
             },
             'var': {
                 'type': Symbol,
             },
-            'root_idx': {
+            'rootIdx': {
                 'type': Integer,
                 'default_raw': -1,
             }
         }
     }
 
-    def __init__(self, parent, name=None,
-                 default=None, tex=None, descrip=None, params=None,
+    def __init__(self, parent, tex=None,
+                 default=None, descrip=None, params=None,
                  args=None, last_raw=None, **other):
-        super().__init__(parent, name, default, tex, descrip, params, args, last_raw)
+        super().__init__(parent, tex, default, descrip, params, args, last_raw)
         self.explicit_cyclo = False
         self.cyc_num = None
         self.raw = None
         self.validated = None
 
     def get_poly(self):
         return self.value.ext.root.minpoly
@@ -118,15 +118,15 @@
         if gen is not None:
             display_value = fr'\mathbb{{Q}}({gen}) \cong ' + display_value
         name_part = self.write_name_and_value(include_value, editable, display_value=display_value)
         noun_phrase = r'a number field over $\mathbb{Q}$'
         return f'{name_part} {noun_phrase}'
 
     def auto_build(self):
-        raw = 'cyc(4)'
+        raw = 'cyc(2)'
         return self.build_from_raw(raw)
 
     def build_from_raw(self, raw):
         """
         :return: AlgebraicField
         """
         raw = str(raw)  # Ensure that we have a string
@@ -157,31 +157,30 @@
             # Careful! `poly_value.is_irreducible` is a `@property` method,
             # so must use `getattr` here as the function:
             is_irred = calculate(getattr, poly_value, 'is_irreducible')
             if not is_irred:
                 msg = r'Polynomial must be irreducible over $\mathbb{Q}$.'
                 raise MalformedParamRawValue(msg, self)
 
-        i = self.resolved_args['root_idx'].value
+        i = self.resolved_args['rootIdx'].value
         root = calculate(construct_instance, CRootOf, poly_value, i)
         ext = calculate(construct_instance, AlgebraicNumber,
                         (poly_value, root),
                         alias=self.get_field_generator_symbol())
         field = calculate(QQ.algebraic_field, ext)
 
         return field
 
     def write_chooser_widget(self):
         context = {
-            'name': self.name,
             'descrip': self.auto_descrip(),
             'current_value': self.raw,
         }
         return nf_chooser_widget_template.render(context)
 
 nf_chooser_widget_template = jinja2.Template("""
-<div class="chooser nf_chooser" name="{{ name }}">
+<div class="chooser nf_chooser">
     <div class="heading">{{ descrip }}</div>
     <div class="error_display"></div>
     <input class="textfield polynomial_field" type="text" placeholder="Irreducible polynomial" value="{{current_value}}"/>
 </div>
 """)
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/prime.py` & `pfsc_examp-0.24.0/pfsc_examp/parameters/types/prime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -39,15 +39,15 @@
     Default: int
 
     Args:
       Required: None.
       Optional:
         odd: boolean, default=False
             True if you require that it be an odd prime
-        chooser_upper_bound: int
+        chooserUpperBound: int
             If positive, do not display primes larger than this in
             the chooser HTML. Note: This is not a *mathematical* constraint;
             you are not saying that the prime actually needs to be bounded
             for any mathematical reason. You are only saying that you want
             to limit the set of primes "on offer". So the reasons for the limit
             are practical ones, relating to computation time, or surveyability
             of displays.
@@ -55,31 +55,31 @@
 
     arg_spec = {
         "OPT": {
             'odd': {
                 'type': BooleanAtom,
                 'default_raw': False,
             },
-            'chooser_upper_bound': {
+            'chooserUpperBound': {
                 'type': Integer,
                 'default_raw': 0,
             },
         }
     }
 
-    def __init__(self, parent, name=None,
-                 default=None, tex=None, descrip=None, params=None,
+    def __init__(self, parent, tex=None,
+                 default=None, descrip=None, params=None,
                  args=None, last_raw=None, **other):
-        super().__init__(parent, name, default, tex, descrip, params, args, last_raw)
+        super().__init__(parent, tex, default, descrip, params, args, last_raw)
         self.odd_only = None
-        self.chooser_upper_bound = None
+        self.chooserUpperBound = None
 
     def prebuild(self):
         self.odd_only = self.resolved_args['odd']
-        self.chooser_upper_bound = self.resolved_args['chooser_upper_bound']
+        self.chooserUpperBound = self.resolved_args['chooserUpperBound']
 
     def auto_build(self):
         raw = 3 if self.odd_only.value else 2
         return self.build_from_raw(raw)
 
     def build_from_raw(self, raw):
         n = self.check_int(raw)
@@ -98,39 +98,38 @@
 
     def write_chooser_widget(self):
         # Booleans to control display of widgets:
         show_three_digit_primes = True
         show_free_box = True
         # Prepare our list of primes under 100 (possibly modified):
         pu100 = primes_under_100[1 if self.odd_only.value else 0:]
-        if 0 < self.chooser_upper_bound.value <= 100:
+        if 0 < self.chooserUpperBound.value <= 100:
             show_three_digit_primes = False
             show_free_box = False
-            pu100 = filter(lambda p: p <= self.chooser_upper_bound.value, pu100)
+            pu100 = filter(lambda p: p <= self.chooserUpperBound.value, pu100)
         # Prepare our list of three-digit primes (possibly modified):
         tdp = None
         if show_three_digit_primes:
             tdp = three_digit_primes[:]
-            if 100 < self.chooser_upper_bound.value <= 1000:
+            if 100 < self.chooserUpperBound.value <= 1000:
                 show_free_box = False
-                tdp = filter(lambda p: p <= self.chooser_upper_bound.value, tdp)
+                tdp = filter(lambda p: p <= self.chooserUpperBound.value, tdp)
         context = {
-            'name': self.name,
             'selected_prime': self.value,
             'descrip': self.auto_descrip(),
             'primes_under_100': pu100,
             'three_digit_primes': tdp,
             'show_tdp': show_three_digit_primes,
             'show_free_box': show_free_box,
         }
         return prime_chooser_widget_template.render(context)
 
 
 prime_chooser_widget_template = jinja2.Template("""
-<div class="chooser radio_panel_chooser prime_chooser" name="{{ name }}">
+<div class="chooser radio_panel_chooser prime_chooser">
     <div class="heading">{{ descrip }}</div>
     <div class="error_display"></div>
     {# #}
     {# Buttons for the primes under 100 #}
     <div class="radio_panel">
         {% for p in primes_under_100 %}
             {% if p == selected_prime %}
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/primeideal.py` & `pfsc_examp-0.24.0/pfsc_examp/parameters/types/primeideal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -39,35 +39,35 @@
     Value type: sympy.polys.numberfields.primes.PrimeIdeal
 
     Default: int
         Zero-based index into the list of PrimeIdeals computed by SymPy.
 
     Args:
         Required:
-            k: Libpath
+            k: param-valued
                 Must point to a param widget of `NumberField` type.
-            p: int
+            p: int-valued
                 The rational prime whose ideal divisors we are to represent.
     """
 
     arg_spec = {
         "REQ": {
             'k': {
                 'type': AlgebraicField,
             },
             'p': {
                 'type': Integer,
             }
         }
     }
 
-    def __init__(self, parent, name=None,
-                 default=None, tex=None, descrip=None, params=None,
+    def __init__(self, parent, tex=None,
+                 default=None, descrip=None, params=None,
                  args=None, last_raw=None, **other):
-        super().__init__(parent, name, default, tex, descrip, params, args, last_raw)
+        super().__init__(parent, tex, default, descrip, params, args, last_raw)
         self.field = None
         self.prime = None
         self.prime_ideals = None
         self.display_values = None
         self.selected_index = None
 
         self.last_field_value = None
@@ -84,15 +84,14 @@
 
         if K != K0 or p != p0:
             # `AlgebraicField.primes_above()` expects a raw `int`, not an `Integer`.
             self.prime_ideals = calculate(K.primes_above, int(p))
             self.display_values = [self.write_display_value_for_prime_ideal(P)
                                    for P in self.prime_ideals]
             self.last_attempted_raw_value = None
-            #print(f'{self.name}: reset last to None')
             self.last_field_value = K
             self.last_prime_value = p
 
     def write_display_value_for_prime_ideal(self, P):
         field_gen = self.field.get_field_generator_symbol()
         alpha = P.alpha.poly(x=field_gen).as_expr()
         p = self.prime.value
@@ -113,11 +112,11 @@
         return f'%s a prime ideal over $%s$ in $%s$' % (
             self.write_name_and_value(include_value, editable, display_value),
             self.prime.value, self.field.getTeX(as_name=True)
         )
 
     def write_chooser_widget(self):
         return write_radio_panel_chooser_widget(
-            self.name, self.auto_descrip(),
+            self.auto_descrip(),
             enumerate([f'${v}$' for v in self.display_values]),
             self.selected_index
         )
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parameters/types/primres.py` & `pfsc_examp-0.24.0/pfsc_examp/parameters/types/primres.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -34,31 +34,31 @@
 
     Value type: Integer
 
     Default: int
 
     Args:
         Required:
-            m: int
+            m: int-valued
                 The modulus.
         Optional: None.
     """
 
     arg_spec = {
         "REQ": {
             'm': {
                 'type': Integer,
             },
         },
     }
 
-    def __init__(self, parent, name=None,
-                 default=None, tex=None, descrip=None, params=None,
+    def __init__(self, parent, tex=None,
+                 default=None, descrip=None, params=None,
                  args=None, last_raw=None, **other):
-        super().__init__(parent, name, default, tex, descrip, params, args, last_raw)
+        super().__init__(parent, tex, default, descrip, params, args, last_raw)
         self.m = None
         # Depending on how big the modulus m is, we might store a list of all
         # of its primitive residues, or we might just store one primitive residue;
         # we might not store either of these if m is too large.
         self.all_options = []
         self.one_option = None
 
@@ -111,24 +111,23 @@
         free_option = True
         if self.all_options:
             ready_options = self.all_options
             free_option = False
         elif self.one_option:
             ready_options = [self.one_option]
         context = {
-            'name': self.name,
             'descrip': self.auto_descrip(),
             'selected_res': self.value,
             'ready_options': ready_options,
             'free_option': free_option,
         }
         return prim_res_chooser_widget_template.render(context)
 
 prim_res_chooser_widget_template = jinja2.Template("""
-<div class="chooser radio_panel_chooser prim_res_chooser" name="{{ name }}">
+<div class="chooser radio_panel_chooser prim_res_chooser">
     <div class="heading">{{ descrip }}</div>
     <div class="error_display"></div>
     {# #}
     {% if ready_options %}
         {# Buttons for ready-made options #}
         <div class="radio_panel">
             {% for r in ready_options %}
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parse/algebraic.py` & `pfsc_examp-0.24.0/pfsc_examp/parse/algebraic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -94,15 +94,15 @@
     @param raw_text: the string supposedly defining the algebraic function.
     @param max_len: maximum allowed length for the string. If `None`, we look
         for a value in the global config.
     @param max_depth: maximum allowed parenthesis depth for the string. If
         `None`, we look for a value in the global config.
     @return: SymPy Expr
     @raise: ParsingExcep if given text is too long, or has too deep parenthesis
-      nesting (important to avoid exceeding recusion stack max depth), or if
+      nesting (important to avoid exceeding recursion stack max depth), or if
       it simply doesn't parse as a valid algebraic function.
     """
     check_expr_dims(raw_text, max_len=max_len, max_depth=max_depth)
     try:
         tree = algebraic_func_parser.parse(raw_text)
     except LarkError as e:
         raise ParsingExcep("Expression not a valid algebraic function.\n" + str(e))
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parse/display.py` & `pfsc_examp-0.24.0/pfsc_examp/parse/display.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parse/excep.py` & `pfsc_examp-0.24.0/pfsc_examp/parse/excep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parse/polynom.py` & `pfsc_examp-0.24.0/pfsc_examp/parse/polynom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parse/sympy_allowed.py` & `pfsc_examp-0.24.0/pfsc_examp/parse/sympy_allowed.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -18,16 +18,17 @@
 
 """
 This module is where we define the set of allowed callables from SymPy.
 The set is expected to grow over time, in response to user demand.
 """
 
 from sympy import (
-    AlgebraicField, AlgebraicNumber, binomial, Expr, Integer, latex,
-    Matrix, mod_inverse, Poly, QQ, S, Symbol, symbols,
+    AlgebraicField, AlgebraicNumber, binomial, Expr, factorint,
+    Integer, isprime, latex,
+    Matrix, mod_inverse, Poly, primerange, QQ, S, Symbol, symbols,
 )
 from sympy.core.evalf import EvalfMixin
 from sympy.logic.boolalg import Boolean
 from sympy.polys.domains.domain import Domain
 from sympy.polys.matrices import DomainMatrix
 from sympy.polys.numberfields.modules import (
     ModuleElement, PowerBasis, Submodule
@@ -74,18 +75,21 @@
     # If you want a `Symbol`, you should use either `symbols()` or `Symbol()`.
     # If we allowed `S` for this purpose, users would find it confusing, since
     # `beta`, `gamma`, `zeta` would be exceptions, being recognized instead as
     # special functions.
     c(S, [u[int, float]], name="S"),
 
     c(binomial, [Int, Int]),
+    c(factorint, [Int]),
+    c(isprime, [Int]),
     c(latex, [[Expr], [Matrix]], {'order': s.CNAME}, incomplete=True),
     c(Matrix, [List[List[fiExpr]]], name="Matrix"),
     c(mod_inverse, [Int, Int]),
     c(Poly, [Expr, t(Symbol)], {'modulus': Int}, incomplete=True),
+    c(primerange, [Int]),
     c(Symbol, [s.UWORD]),
     c(symbols, [s.UWORD_CDL]),
 ]
 
 # These are callables not added to the namespace basis. Instead, we expect you
 # to access them through other objects you define or import from other displays
 # or parameters.
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/parse/util.py` & `pfsc_examp-0.24.0/pfsc_examp/parse/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp/util.py` & `pfsc_examp-0.24.0/pfsc_examp/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   Proofscape Examplorers                                                    #
 #                                                                             #
-#   Copyright (c) 2018-2023 Proofscape Contributors                           #
+#   Copyright (c) 2018-2024 Proofscape Contributors                           #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `pfsc-examp-0.23.0b0/pfsc_examp.egg-info/SOURCES.txt` & `pfsc_examp-0.24.0/pfsc_examp.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -28,8 +28,10 @@
 pfsc_examp/parameters/types/primres.py
 pfsc_examp/parse/__init__.py
 pfsc_examp/parse/algebraic.py
 pfsc_examp/parse/display.py
 pfsc_examp/parse/excep.py
 pfsc_examp/parse/polynom.py
 pfsc_examp/parse/sympy_allowed.py
-pfsc_examp/parse/util.py
+pfsc_examp/parse/util.py
+tests/test_display.py
+tests/test_parameters.py
```

### Comparing `pfsc-examp-0.23.0b0/setup.cfg` & `pfsc_examp-0.24.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -25,12 +25,13 @@
 
 [options.extras_require]
 dev = 
 	pytest
 	build
 	twine
 	invoke
+	dill
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

