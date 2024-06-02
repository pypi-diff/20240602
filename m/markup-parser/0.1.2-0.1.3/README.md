# Comparing `tmp/markup-parser-0.1.2.tar.gz` & `tmp/markup_parser-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markup-parser-0.1.2.tar", last modified: Sun Aug 15 19:50:40 2021, max compression
+gzip compressed data, was "markup_parser-0.1.3.tar", last modified: Sun Jun  2 09:42:27 2024, max compression
```

## Comparing `markup-parser-0.1.2.tar` & `markup_parser-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,27 @@
-drwxr-xr-x   0 out-sokolov5-ae   (503) staff       (20)        0 2021-08-15 19:50:40.680965 markup-parser-0.1.2/
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)      411 2021-08-13 17:47:13.000000 markup-parser-0.1.2/Cargo.toml
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)     1073 2021-08-14 00:09:55.000000 markup-parser-0.1.2/LICENSE
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)       59 2021-08-13 22:47:14.000000 markup-parser-0.1.2/MANIFEST.in
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)     4226 2021-08-15 19:50:40.681131 markup-parser-0.1.2/PKG-INFO
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)     3351 2021-08-14 01:31:06.000000 markup-parser-0.1.2/README.md
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)        5 2021-08-15 19:47:25.000000 markup-parser-0.1.2/VERSION
-drwxr-xr-x   0 out-sokolov5-ae   (503) staff       (20)        0 2021-08-15 19:50:40.674748 markup-parser-0.1.2/markup_parser.egg-info/
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)     4226 2021-08-15 19:50:40.000000 markup-parser-0.1.2/markup_parser.egg-info/PKG-INFO
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)      678 2021-08-15 19:50:40.000000 markup-parser-0.1.2/markup_parser.egg-info/SOURCES.txt
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)        1 2021-08-15 19:50:40.000000 markup-parser-0.1.2/markup_parser.egg-info/dependency_links.txt
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)        1 2021-08-14 00:04:21.000000 markup-parser-0.1.2/markup_parser.egg-info/not-zip-safe
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)       14 2021-08-15 19:50:40.000000 markup-parser-0.1.2/markup_parser.egg-info/top_level.txt
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)       68 2021-08-15 19:46:23.000000 markup-parser-0.1.2/pyproject.toml
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)     1166 2021-08-15 19:50:40.681893 markup-parser-0.1.2/setup.cfg
--rwxr-xr-x   0 out-sokolov5-ae   (503) staff       (20)      149 2021-08-15 19:28:46.000000 markup-parser-0.1.2/setup.py
-drwxr-xr-x   0 out-sokolov5-ae   (503) staff       (20)        0 2021-08-15 19:50:40.675715 markup-parser-0.1.2/src/
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)     5854 2021-08-13 22:28:07.000000 markup-parser-0.1.2/src/lib.rs
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)       14 2021-08-13 19:19:35.000000 markup-parser-0.1.2/src/main.rs
-drwxr-xr-x   0 out-sokolov5-ae   (503) staff       (20)        0 2021-08-15 19:50:40.676786 markup-parser-0.1.2/src/markup_parser/
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)      112 2021-08-13 18:34:49.000000 markup-parser-0.1.2/src/markup_parser/__init__.py
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)      381 2021-08-13 19:55:20.000000 markup-parser-0.1.2/src/markup_parser/parser.py
-drwxr-xr-x   0 out-sokolov5-ae   (503) staff       (20)        0 2021-08-15 19:50:40.678897 markup-parser-0.1.2/src/test/
-drwxr-xr-x   0 out-sokolov5-ae   (503) staff       (20)        0 2021-08-15 19:50:40.680488 markup-parser-0.1.2/src/test/__pycache__/
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)     1265 2021-08-13 22:22:46.000000 markup-parser-0.1.2/src/test/__pycache__/test_parse_from_text.cpython-39-pytest-6.2.4.pyc
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)     1304 2021-08-13 23:39:41.000000 markup-parser-0.1.2/src/test/__pycache__/test_with_prefix.cpython-39-pytest-6.2.4.pyc
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)     1523 2021-08-14 01:48:04.000000 markup-parser-0.1.2/src/test/__pycache__/test_without_prefix.cpython-39-pytest-6.2.4.pyc
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)      287 2021-08-13 22:25:58.000000 markup-parser-0.1.2/src/test/test_with_prefix.html
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)      805 2021-08-13 23:38:19.000000 markup-parser-0.1.2/src/test/test_with_prefix.py
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)      336 2021-08-14 01:47:49.000000 markup-parser-0.1.2/src/test/test_without_prefix.html
--rw-r--r--   0 out-sokolov5-ae   (503) staff       (20)     1007 2021-08-14 01:48:02.000000 markup-parser-0.1.2/src/test/test_without_prefix.py
+drwxr-xr-x   0 bigpe      (502) staff       (20)        0 2024-06-02 09:42:27.747023 markup_parser-0.1.3/
+-rw-r--r--   0 bigpe      (502) staff       (20)      341 2024-06-02 09:15:33.000000 markup_parser-0.1.3/Cargo.toml
+-rw-r--r--   0 bigpe      (502) staff       (20)     1073 2024-06-02 08:58:32.000000 markup_parser-0.1.3/LICENSE
+-rw-r--r--   0 bigpe      (502) staff       (20)       59 2024-06-02 08:58:32.000000 markup_parser-0.1.3/MANIFEST.in
+-rw-r--r--   0 bigpe      (502) staff       (20)     4276 2024-06-02 09:42:27.746922 markup_parser-0.1.3/PKG-INFO
+-rw-r--r--   0 bigpe      (502) staff       (20)     3351 2024-06-02 08:58:32.000000 markup_parser-0.1.3/README.md
+-rw-r--r--   0 bigpe      (502) staff       (20)        5 2024-06-02 09:06:10.000000 markup_parser-0.1.3/VERSION
+drwxr-xr-x   0 bigpe      (502) staff       (20)        0 2024-06-02 09:42:27.746585 markup_parser-0.1.3/markup_parser.egg-info/
+-rw-r--r--   0 bigpe      (502) staff       (20)     4276 2024-06-02 09:42:27.000000 markup_parser-0.1.3/markup_parser.egg-info/PKG-INFO
+-rw-r--r--   0 bigpe      (502) staff       (20)      473 2024-06-02 09:42:27.000000 markup_parser-0.1.3/markup_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 bigpe      (502) staff       (20)        1 2024-06-02 09:42:27.000000 markup_parser-0.1.3/markup_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 bigpe      (502) staff       (20)        1 2024-06-02 09:29:25.000000 markup_parser-0.1.3/markup_parser.egg-info/not-zip-safe
+-rw-r--r--   0 bigpe      (502) staff       (20)       14 2024-06-02 09:42:27.000000 markup_parser-0.1.3/markup_parser.egg-info/top_level.txt
+-rw-r--r--   0 bigpe      (502) staff       (20)       68 2024-06-02 09:31:07.000000 markup_parser-0.1.3/pyproject.toml
+-rw-r--r--   0 bigpe      (502) staff       (20)     1206 2024-06-02 09:42:27.747545 markup_parser-0.1.3/setup.cfg
+-rwxr-xr-x   0 bigpe      (502) staff       (20)      188 2024-06-02 09:26:15.000000 markup_parser-0.1.3/setup.py
+drwxr-xr-x   0 bigpe      (502) staff       (20)        0 2024-06-02 09:42:27.744378 markup_parser-0.1.3/src/
+-rw-r--r--   0 bigpe      (502) staff       (20)     5854 2024-06-02 08:58:32.000000 markup_parser-0.1.3/src/lib.rs
+-rw-r--r--   0 bigpe      (502) staff       (20)       14 2024-06-02 08:58:32.000000 markup_parser-0.1.3/src/main.rs
+drwxr-xr-x   0 bigpe      (502) staff       (20)        0 2024-06-02 09:42:27.744989 markup_parser-0.1.3/src/markup_parser/
+-rw-r--r--   0 bigpe      (502) staff       (20)      112 2024-06-02 08:58:32.000000 markup_parser-0.1.3/src/markup_parser/__init__.py
+-rw-r--r--   0 bigpe      (502) staff       (20)      381 2024-06-02 08:58:32.000000 markup_parser-0.1.3/src/markup_parser/parser.py
+drwxr-xr-x   0 bigpe      (502) staff       (20)        0 2024-06-02 09:42:27.746245 markup_parser-0.1.3/src/test/
+-rw-r--r--   0 bigpe      (502) staff       (20)      287 2024-06-02 08:58:32.000000 markup_parser-0.1.3/src/test/test_with_prefix.html
+-rw-r--r--   0 bigpe      (502) staff       (20)      805 2024-06-02 08:58:32.000000 markup_parser-0.1.3/src/test/test_with_prefix.py
+-rw-r--r--   0 bigpe      (502) staff       (20)      336 2024-06-02 08:58:32.000000 markup_parser-0.1.3/src/test/test_without_prefix.html
+-rw-r--r--   0 bigpe      (502) staff       (20)     1007 2024-06-02 08:58:32.000000 markup_parser-0.1.3/src/test/test_without_prefix.py
```

### Comparing `markup-parser-0.1.2/LICENSE` & `markup_parser-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `markup-parser-0.1.2/PKG-INFO` & `markup_parser-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markup-parser
-Version: 0.1.2
+Version: 0.1.3
 Summary: Parse JS variables from HTML markup
 Home-page: https://github.com/bigpe/markup-parser
 Author: Aleskandr Sokolov
 Author-email: bigpewm@gmail.com
 License: MIT
 Keywords: html,parse,markup,js,variables,rust
 Platform: any
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Markup Parser
 #### Extract JS variables content from HTML markup
@@ -170,8 +171,7 @@
 ```python
 from markup_parser import var_from_url
 
 var_from_url('http://test.page', 'test_variable')
 
 # >>> You found me again!
 ```
-
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: markup-parser Version: 0.1.2 Summary: Parse JS
+Metadata-Version: 2.1 Name: markup-parser Version: 0.1.3 Summary: Parse JS
 variables from HTML markup Home-page: https://github.com/bigpe/markup-parser
 Author: Aleskandr Sokolov Author-email: bigpewm@gmail.com License: MIT
 Keywords: html,parse,markup,js,variables,rust Platform: any Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Requires-Python: >=3.6.0 Description-Content-
-Type: text/markdown License-File: LICENSE # Markup Parser #### Extract JS
-variables content from HTML markup [![Codecov](https://img.shields.io/badge/
-License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Build Status]
-(https://travis-ci.com/bigpe/markup-
-parser.svg?token=9PVJVxRxQ4uXFdey5v3k&branch=master)](https://travis-ci.com/
-bigpe/markup-parser) [![Versions](https://img.shields.io/pypi/pyversions/
-markup-parser.svg)](https://pypi.org/project/markup-parser/) [![Release](https:
-//img.shields.io/github/release/bigpe/markup-parser.svg)](https://github.com/
-bigpe/markup-parser/releases) ### ENG [RU](#ru) ## Installation ```shell pip
-install markup-parser ``` ## Usage ### Parse variable from html text: Test
-content ```html
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.6.0 Description-Content-Type: text/markdown
+License-File: LICENSE # Markup Parser #### Extract JS variables content from
+HTML markup [![Codecov](https://img.shields.io/badge/License-MIT-yellow.svg)]
+(https://opensource.org/licenses/MIT) [![Build Status](https://travis-ci.com/
+bigpe/markup-parser.svg?token=9PVJVxRxQ4uXFdey5v3k&branch=master)](https://
+travis-ci.com/bigpe/markup-parser) [![Versions](https://img.shields.io/pypi/
+pyversions/markup-parser.svg)](https://pypi.org/project/markup-parser/) [!
+[Release](https://img.shields.io/github/release/bigpe/markup-parser.svg)]
+(https://github.com/bigpe/markup-parser/releases) ### ENG [RU](#ru) ##
+Installation ```shell pip install markup-parser ``` ## Usage ### Parse variable
+from html text: Test content ```html
 ``` ```python import requests from markup_parser import var_from_html # Fetch
 html content by get request html_text = requests.get('http://test.html').text
 var_from_html(html_text, 'test_variable') # Parse from file var_from_html(open
 ('test.html').read(), 'test_variable') # >>> You found me ``` ### Parse
 variable from url: _* This variant not recommended if you need to specify
 custom headers, this feature may be added in future release_ Test content
 ```html
```

### Comparing `markup-parser-0.1.2/README.md` & `markup_parser-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `markup-parser-0.1.2/markup_parser.egg-info/PKG-INFO` & `markup_parser-0.1.3/markup_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markup-parser
-Version: 0.1.2
+Version: 0.1.3
 Summary: Parse JS variables from HTML markup
 Home-page: https://github.com/bigpe/markup-parser
 Author: Aleskandr Sokolov
 Author-email: bigpewm@gmail.com
 License: MIT
 Keywords: html,parse,markup,js,variables,rust
 Platform: any
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Markup Parser
 #### Extract JS variables content from HTML markup
@@ -170,8 +171,7 @@
 ```python
 from markup_parser import var_from_url
 
 var_from_url('http://test.page', 'test_variable')
 
 # >>> You found me again!
 ```
-
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: markup-parser Version: 0.1.2 Summary: Parse JS
+Metadata-Version: 2.1 Name: markup-parser Version: 0.1.3 Summary: Parse JS
 variables from HTML markup Home-page: https://github.com/bigpe/markup-parser
 Author: Aleskandr Sokolov Author-email: bigpewm@gmail.com License: MIT
 Keywords: html,parse,markup,js,variables,rust Platform: any Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Requires-Python: >=3.6.0 Description-Content-
-Type: text/markdown License-File: LICENSE # Markup Parser #### Extract JS
-variables content from HTML markup [![Codecov](https://img.shields.io/badge/
-License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Build Status]
-(https://travis-ci.com/bigpe/markup-
-parser.svg?token=9PVJVxRxQ4uXFdey5v3k&branch=master)](https://travis-ci.com/
-bigpe/markup-parser) [![Versions](https://img.shields.io/pypi/pyversions/
-markup-parser.svg)](https://pypi.org/project/markup-parser/) [![Release](https:
-//img.shields.io/github/release/bigpe/markup-parser.svg)](https://github.com/
-bigpe/markup-parser/releases) ### ENG [RU](#ru) ## Installation ```shell pip
-install markup-parser ``` ## Usage ### Parse variable from html text: Test
-content ```html
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.6.0 Description-Content-Type: text/markdown
+License-File: LICENSE # Markup Parser #### Extract JS variables content from
+HTML markup [![Codecov](https://img.shields.io/badge/License-MIT-yellow.svg)]
+(https://opensource.org/licenses/MIT) [![Build Status](https://travis-ci.com/
+bigpe/markup-parser.svg?token=9PVJVxRxQ4uXFdey5v3k&branch=master)](https://
+travis-ci.com/bigpe/markup-parser) [![Versions](https://img.shields.io/pypi/
+pyversions/markup-parser.svg)](https://pypi.org/project/markup-parser/) [!
+[Release](https://img.shields.io/github/release/bigpe/markup-parser.svg)]
+(https://github.com/bigpe/markup-parser/releases) ### ENG [RU](#ru) ##
+Installation ```shell pip install markup-parser ``` ## Usage ### Parse variable
+from html text: Test content ```html
 ``` ```python import requests from markup_parser import var_from_html # Fetch
 html content by get request html_text = requests.get('http://test.html').text
 var_from_html(html_text, 'test_variable') # Parse from file var_from_html(open
 ('test.html').read(), 'test_variable') # >>> You found me ``` ### Parse
 variable from url: _* This variant not recommended if you need to specify
 custom headers, this feature may be added in future release_ Test content
 ```html
```

### Comparing `markup-parser-0.1.2/setup.cfg` & `markup_parser-0.1.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 author = Aleskandr Sokolov
 author_email = bigpewm@gmail.com
 url = https://github.com/bigpe/markup-parser
 description = Parse JS variables from HTML markup
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
-license-file = LICENSE
+license_file = LICENSE
 keywords = html, parse, markup, js, variables, rust
 platform = any
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 zip_safe = False
 include_package_data = True
 python_requires = >= 3.6.0
 setup_requires =
```

### Comparing `markup-parser-0.1.2/src/lib.rs` & `markup_parser-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `markup-parser-0.1.2/src/test/test_with_prefix.py` & `markup_parser-0.1.3/src/test/test_with_prefix.py`

 * *Files identical despite different names*

### Comparing `markup-parser-0.1.2/src/test/test_without_prefix.py` & `markup_parser-0.1.3/src/test/test_without_prefix.py`

 * *Files identical despite different names*

