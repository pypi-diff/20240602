# Comparing `tmp/test_dvs_printf-1.6.tar.gz` & `tmp/test_dvs_printf-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_dvs_printf-1.6.tar", last modified: Sun Jun  2 05:43:45 2024, max compression
+gzip compressed data, was "test_dvs_printf-1.8.tar", last modified: Sun Jun  2 06:15:19 2024, max compression
```

## Comparing `test_dvs_printf-1.6.tar` & `test_dvs_printf-1.8.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-06-02 05:43:45.493599 test_dvs_printf-1.6/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1070 2024-04-04 03:31:22.000000 test_dvs_printf-1.6/LICENSE
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      175 2024-06-02 05:06:41.000000 test_dvs_printf-1.6/MANIFEST.in
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4951 2024-06-02 05:43:45.493301 test_dvs_printf-1.6/PKG-INFO
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3823 2024-05-28 12:57:54.000000 test_dvs_printf-1.6/README.md
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)   418247 2024-04-04 03:31:22.000000 test_dvs_printf-1.6/card.png
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      104 2024-05-27 04:55:17.000000 test_dvs_printf-1.6/pyproject.toml
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)       38 2024-06-02 05:43:45.493649 test_dvs_printf-1.6/setup.cfg
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     2446 2024-06-02 05:43:10.000000 test_dvs_printf-1.6/setup.py
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-06-02 05:43:45.489857 test_dvs_printf-1.6/test_dvs_printf/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3066 2024-05-28 12:08:56.000000 test_dvs_printf-1.6/test_dvs_printf/__Loding__.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4377 2024-05-09 03:52:50.000000 test_dvs_printf-1.6/test_dvs_printf/__init.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1242 2024-05-28 12:08:57.000000 test_dvs_printf-1.6/test_dvs_printf/__init__.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10693 2024-05-28 12:08:53.000000 test_dvs_printf-1.6/test_dvs_printf/__printf__.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10813 2024-05-28 12:08:52.000000 test_dvs_printf-1.6/test_dvs_printf/oth_styles.py
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-06-02 05:43:45.492873 test_dvs_printf-1.6/test_dvs_printf.egg-info/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4951 2024-06-02 05:43:45.000000 test_dvs_printf-1.6/test_dvs_printf.egg-info/PKG-INFO
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      584 2024-06-02 05:43:45.000000 test_dvs_printf-1.6/test_dvs_printf.egg-info/SOURCES.txt
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)        1 2024-06-02 05:43:45.000000 test_dvs_printf-1.6/test_dvs_printf.egg-info/dependency_links.txt
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)        1 2024-06-02 05:43:36.000000 test_dvs_printf-1.6/test_dvs_printf.egg-info/not-zip-safe
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)       16 2024-06-02 05:43:45.000000 test_dvs_printf-1.6/test_dvs_printf.egg-info/top_level.txt
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-06-02 05:43:45.492579 test_dvs_printf-1.6/tests/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      885 2024-06-02 04:57:27.000000 test_dvs_printf-1.6/tests/test_Numpy.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      973 2024-06-02 04:57:37.000000 test_dvs_printf-1.6/tests/test_Pandas.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      967 2024-06-02 04:57:32.000000 test_dvs_printf-1.6/tests/test_PyTorch.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1228 2024-06-02 04:57:33.000000 test_dvs_printf-1.6/tests/test_Tensorflow.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      900 2024-06-02 04:57:19.000000 test_dvs_printf-1.6/tests/test__init__.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      377 2024-06-02 04:57:13.000000 test_dvs_printf-1.6/tests/test_arrayToList.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1548 2024-06-02 04:57:35.000000 test_dvs_printf-1.6/tests/test_listfunction.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      215 2024-06-02 04:57:24.000000 test_dvs_printf-1.6/tests/test_loding.py
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-06-02 06:15:19.956143 test_dvs_printf-1.8/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1070 2024-04-04 03:31:22.000000 test_dvs_printf-1.8/LICENSE
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)       90 2024-06-02 05:53:54.000000 test_dvs_printf-1.8/MANIFEST.in
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4995 2024-06-02 06:15:19.955908 test_dvs_printf-1.8/PKG-INFO
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3854 2024-06-02 06:06:18.000000 test_dvs_printf-1.8/README.md
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      104 2024-05-27 04:55:17.000000 test_dvs_printf-1.8/pyproject.toml
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)       38 2024-06-02 06:15:19.956183 test_dvs_printf-1.8/setup.cfg
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     2459 2024-06-02 06:15:08.000000 test_dvs_printf-1.8/setup.py
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-06-02 06:15:19.953312 test_dvs_printf-1.8/test_dvs_printf/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3066 2024-05-28 12:08:56.000000 test_dvs_printf-1.8/test_dvs_printf/__Loding__.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4377 2024-05-09 03:52:50.000000 test_dvs_printf-1.8/test_dvs_printf/__init.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1242 2024-05-28 12:08:57.000000 test_dvs_printf-1.8/test_dvs_printf/__init__.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10693 2024-05-28 12:08:53.000000 test_dvs_printf-1.8/test_dvs_printf/__printf__.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10813 2024-05-28 12:08:52.000000 test_dvs_printf-1.8/test_dvs_printf/oth_styles.py
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-06-02 06:15:19.955490 test_dvs_printf-1.8/test_dvs_printf.egg-info/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4995 2024-06-02 06:15:19.000000 test_dvs_printf-1.8/test_dvs_printf.egg-info/PKG-INFO
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      575 2024-06-02 06:15:19.000000 test_dvs_printf-1.8/test_dvs_printf.egg-info/SOURCES.txt
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)        1 2024-06-02 06:15:19.000000 test_dvs_printf-1.8/test_dvs_printf.egg-info/dependency_links.txt
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)        1 2024-06-02 06:15:14.000000 test_dvs_printf-1.8/test_dvs_printf.egg-info/not-zip-safe
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)       16 2024-06-02 06:15:19.000000 test_dvs_printf-1.8/test_dvs_printf.egg-info/top_level.txt
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-06-02 06:15:19.955284 test_dvs_printf-1.8/tests/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      885 2024-06-02 04:57:27.000000 test_dvs_printf-1.8/tests/test_Numpy.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      973 2024-06-02 04:57:37.000000 test_dvs_printf-1.8/tests/test_Pandas.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      967 2024-06-02 04:57:32.000000 test_dvs_printf-1.8/tests/test_PyTorch.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1228 2024-06-02 04:57:33.000000 test_dvs_printf-1.8/tests/test_Tensorflow.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      900 2024-06-02 04:57:19.000000 test_dvs_printf-1.8/tests/test__init__.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      377 2024-06-02 04:57:13.000000 test_dvs_printf-1.8/tests/test_arrayToList.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1548 2024-06-02 04:57:35.000000 test_dvs_printf-1.8/tests/test_listfunction.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      215 2024-06-02 04:57:24.000000 test_dvs_printf-1.8/tests/test_loding.py
```

### Comparing `test_dvs_printf-1.6/LICENSE` & `test_dvs_printf-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.6/PKG-INFO` & `test_dvs_printf-1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: test_dvs_printf
-Version: 1.6
+Version: 1.8
 Summary: Animated Visual appearance for console-based applications, with different animation styles
 Home-page: https://github.com/dhruvan-vyas/dvs_printf
 Author: Dhruvan Vyas
 License: MIT
 Project-URL: Source, https://github.com/dhruvan-vyas/dvs_printf
 Project-URL: Documentation, https://github.com/dhruvan-vyas/dvs_printf/blob/main/README.md
 Project-URL: Tracker, https://github.com/dhruvan-vyas/dvs_printf/issues
 Keywords: printf,animation,console,terminal
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <div class="onelinetext" align="center" style="padding-top:35px;">
 <h2>Simple and dynamic printing animation styles for Python project</h2> 
 
-[![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://badge.fury.io/py/dvs-printf)
+[![PyPI Version (latest by date)](https://badge.fury.io/py/test-dvs-printf.svg?cachebuster=1)](https://badge.fury.io/py/dvs-printf)
 [![Build Status](https://github.com/dhruvan-vyas/dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/dhruvan-vyas/dvs_printf/actions)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/dhruvan-vyas/dvs_printf/releases/tag/v1.3)<br>
 ![Python Versions](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/LICENSE)
 [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)](https://www.python.org/dev/peps/pep-0008/) 
 </div>
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: test_dvs_printf Version: 1.6 Summary: Animated
+Metadata-Version: 2.1 Name: test_dvs_printf Version: 1.8 Summary: Animated
 Visual appearance for console-based applications, with different animation
 styles Home-page: https://github.com/dhruvan-vyas/dvs_printf Author: Dhruvan
 Vyas License: MIT Project-URL: Source, https://github.com/dhruvan-vyas/
 dvs_printf Project-URL: Documentation, https://github.com/dhruvan-vyas/
 dvs_printf/blob/main/README.md Project-URL: Tracker, https://github.com/
 dhruvan-vyas/dvs_printf/issues Keywords: printf,animation,console,terminal
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: Operating System :: OS
-Independent Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Terminals Classifier: Environment :: Console
-Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Operating System
+:: OS Independent Classifier: Topic :: Software Development :: Libraries ::
+Python Modules Classifier: Topic :: Terminals Classifier: Environment ::
+Console Requires-Python: >=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE
   ********** SSiimmppllee aanndd ddyynnaammiicc pprriinnttiinngg aanniimmaattiioonn ssttyylleess ffoorr PPyytthhoonn pprroojjeecctt **********
-   [![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://
-badge.fury.io/py/dvs-printf) [![Build Status](https://github.com/dhruvan-vyas/
- dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/
- dhruvan-vyas/dvs_printf/actions) [![GitHub release (latest by date)](https://
- img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/
-                  dhruvan-vyas/dvs_printf/releases/tag/v1.3)
+     [![PyPI Version (latest by date)](https://badge.fury.io/py/test-dvs-
+   printf.svg?cachebuster=1)](https://badge.fury.io/py/dvs-printf) [![Build
+     Status](https://github.com/dhruvan-vyas/dvs_printf/actions/workflows/
+module_test.yml/badge.svg)](https://github.com/dhruvan-vyas/dvs_printf/actions)
+ [![GitHub release (latest by date)](https://img.shields.io/github/v/release/
+dhruvan-vyas/dvs_printf)](https://github.com/dhruvan-vyas/dvs_printf/releases/
+                                   tag/v1.3)
             ![Python Versions](https://img.shields.io/badge/python-
 3.10%20%7C%203.11%20%7C%203.12-blue) [![License](https://img.shields.io/badge/
  license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/
 LICENSE) [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)]
                   (https://www.python.org/dev/peps/pep-0008/)
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_h_r_u_v_a_n_-_v_y_a_s_/_d_v_s___p_r_i_n_t_f_/_b_l_o_b_/_m_a_i_n_/_c_a_r_d_._p_n_g_?_r_a_w_=_t_r_u_e_]
 Enhanced way to handle console output for Python projects. The module offers
```

### Comparing `test_dvs_printf-1.6/README.md` & `test_dvs_printf-1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 <div class="onelinetext" align="center" style="padding-top:35px;">
 <h2>Simple and dynamic printing animation styles for Python project</h2> 
 
-[![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://badge.fury.io/py/dvs-printf)
+[![PyPI Version (latest by date)](https://badge.fury.io/py/test-dvs-printf.svg?cachebuster=1)](https://badge.fury.io/py/dvs-printf)
 [![Build Status](https://github.com/dhruvan-vyas/dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/dhruvan-vyas/dvs_printf/actions)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/dhruvan-vyas/dvs_printf/releases/tag/v1.3)<br>
 ![Python Versions](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/LICENSE)
 [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)](https://www.python.org/dev/peps/pep-0008/) 
 </div>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
   ********** SSiimmppllee aanndd ddyynnaammiicc pprriinnttiinngg aanniimmaattiioonn ssttyylleess ffoorr PPyytthhoonn pprroojjeecctt **********
-   [![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://
-badge.fury.io/py/dvs-printf) [![Build Status](https://github.com/dhruvan-vyas/
- dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/
- dhruvan-vyas/dvs_printf/actions) [![GitHub release (latest by date)](https://
- img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/
-                  dhruvan-vyas/dvs_printf/releases/tag/v1.3)
+     [![PyPI Version (latest by date)](https://badge.fury.io/py/test-dvs-
+   printf.svg?cachebuster=1)](https://badge.fury.io/py/dvs-printf) [![Build
+     Status](https://github.com/dhruvan-vyas/dvs_printf/actions/workflows/
+module_test.yml/badge.svg)](https://github.com/dhruvan-vyas/dvs_printf/actions)
+ [![GitHub release (latest by date)](https://img.shields.io/github/v/release/
+dhruvan-vyas/dvs_printf)](https://github.com/dhruvan-vyas/dvs_printf/releases/
+                                   tag/v1.3)
             ![Python Versions](https://img.shields.io/badge/python-
 3.10%20%7C%203.11%20%7C%203.12-blue) [![License](https://img.shields.io/badge/
  license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/
 LICENSE) [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)]
                   (https://www.python.org/dev/peps/pep-0008/)
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_h_r_u_v_a_n_-_v_y_a_s_/_d_v_s___p_r_i_n_t_f_/_b_l_o_b_/_m_a_i_n_/_c_a_r_d_._p_n_g_?_r_a_w_=_t_r_u_e_]
 Enhanced way to handle console output for Python projects. The module offers
```

### Comparing `test_dvs_printf-1.6/setup.py` & `test_dvs_printf-1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 # )
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='test_dvs_printf',
-    version='1.6',
+    version='1.8',
     description=
 "Animated Visual appearance for console-based applications, with different animation styles",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Dhruvan Vyas',
     url='https://github.com/dhruvan-vyas/dvs_printf',
     packages=find_packages(),
     python_requires='>=3.10',
     classifiers=[
-        'Development Status :: 4 - Beta',
+        "Development Status :: 5 - Production/Stable",
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Operating System :: OS Independent',
```

### Comparing `test_dvs_printf-1.6/test_dvs_printf/__Loding__.py` & `test_dvs_printf-1.8/test_dvs_printf/__Loding__.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.6/test_dvs_printf/__init.py` & `test_dvs_printf-1.8/test_dvs_printf/__init.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.6/test_dvs_printf/__init__.py` & `test_dvs_printf-1.8/test_dvs_printf/__init__.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.6/test_dvs_printf/__printf__.py` & `test_dvs_printf-1.8/test_dvs_printf/__printf__.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.6/test_dvs_printf/oth_styles.py` & `test_dvs_printf-1.8/test_dvs_printf/oth_styles.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.6/test_dvs_printf.egg-info/PKG-INFO` & `test_dvs_printf-1.8/test_dvs_printf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: test_dvs_printf
-Version: 1.6
+Version: 1.8
 Summary: Animated Visual appearance for console-based applications, with different animation styles
 Home-page: https://github.com/dhruvan-vyas/dvs_printf
 Author: Dhruvan Vyas
 License: MIT
 Project-URL: Source, https://github.com/dhruvan-vyas/dvs_printf
 Project-URL: Documentation, https://github.com/dhruvan-vyas/dvs_printf/blob/main/README.md
 Project-URL: Tracker, https://github.com/dhruvan-vyas/dvs_printf/issues
 Keywords: printf,animation,console,terminal
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <div class="onelinetext" align="center" style="padding-top:35px;">
 <h2>Simple and dynamic printing animation styles for Python project</h2> 
 
-[![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://badge.fury.io/py/dvs-printf)
+[![PyPI Version (latest by date)](https://badge.fury.io/py/test-dvs-printf.svg?cachebuster=1)](https://badge.fury.io/py/dvs-printf)
 [![Build Status](https://github.com/dhruvan-vyas/dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/dhruvan-vyas/dvs_printf/actions)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/dhruvan-vyas/dvs_printf/releases/tag/v1.3)<br>
 ![Python Versions](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/LICENSE)
 [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)](https://www.python.org/dev/peps/pep-0008/) 
 </div>
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: test_dvs_printf Version: 1.6 Summary: Animated
+Metadata-Version: 2.1 Name: test_dvs_printf Version: 1.8 Summary: Animated
 Visual appearance for console-based applications, with different animation
 styles Home-page: https://github.com/dhruvan-vyas/dvs_printf Author: Dhruvan
 Vyas License: MIT Project-URL: Source, https://github.com/dhruvan-vyas/
 dvs_printf Project-URL: Documentation, https://github.com/dhruvan-vyas/
 dvs_printf/blob/main/README.md Project-URL: Tracker, https://github.com/
 dhruvan-vyas/dvs_printf/issues Keywords: printf,animation,console,terminal
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: Operating System :: OS
-Independent Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Terminals Classifier: Environment :: Console
-Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Operating System
+:: OS Independent Classifier: Topic :: Software Development :: Libraries ::
+Python Modules Classifier: Topic :: Terminals Classifier: Environment ::
+Console Requires-Python: >=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE
   ********** SSiimmppllee aanndd ddyynnaammiicc pprriinnttiinngg aanniimmaattiioonn ssttyylleess ffoorr PPyytthhoonn pprroojjeecctt **********
-   [![PyPI Version](https://badge.fury.io/py/test-dvs-printf.svg)](https://
-badge.fury.io/py/dvs-printf) [![Build Status](https://github.com/dhruvan-vyas/
- dvs_printf/actions/workflows/module_test.yml/badge.svg)](https://github.com/
- dhruvan-vyas/dvs_printf/actions) [![GitHub release (latest by date)](https://
- img.shields.io/github/v/release/dhruvan-vyas/dvs_printf)](https://github.com/
-                  dhruvan-vyas/dvs_printf/releases/tag/v1.3)
+     [![PyPI Version (latest by date)](https://badge.fury.io/py/test-dvs-
+   printf.svg?cachebuster=1)](https://badge.fury.io/py/dvs-printf) [![Build
+     Status](https://github.com/dhruvan-vyas/dvs_printf/actions/workflows/
+module_test.yml/badge.svg)](https://github.com/dhruvan-vyas/dvs_printf/actions)
+ [![GitHub release (latest by date)](https://img.shields.io/github/v/release/
+dhruvan-vyas/dvs_printf)](https://github.com/dhruvan-vyas/dvs_printf/releases/
+                                   tag/v1.3)
             ![Python Versions](https://img.shields.io/badge/python-
 3.10%20%7C%203.11%20%7C%203.12-blue) [![License](https://img.shields.io/badge/
  license-MIT-blue.svg)](https://github.com/dhruvan-vyas/dvs_printf/blob/main/
 LICENSE) [![PEP8](https://img.shields.io/badge/PEP8-compliant-brightgreen.svg)]
                   (https://www.python.org/dev/peps/pep-0008/)
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_h_r_u_v_a_n_-_v_y_a_s_/_d_v_s___p_r_i_n_t_f_/_b_l_o_b_/_m_a_i_n_/_c_a_r_d_._p_n_g_?_r_a_w_=_t_r_u_e_]
 Enhanced way to handle console output for Python projects. The module offers
```

### Comparing `test_dvs_printf-1.6/test_dvs_printf.egg-info/SOURCES.txt` & `test_dvs_printf-1.8/test_dvs_printf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-card.png
 pyproject.toml
 setup.py
 test_dvs_printf/__Loding__.py
 test_dvs_printf/__init.py
 test_dvs_printf/__init__.py
 test_dvs_printf/__printf__.py
 test_dvs_printf/oth_styles.py
```

### Comparing `test_dvs_printf-1.6/tests/test_Numpy.py` & `test_dvs_printf-1.8/tests/test_Numpy.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.6/tests/test_Pandas.py` & `test_dvs_printf-1.8/tests/test_Pandas.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.6/tests/test_PyTorch.py` & `test_dvs_printf-1.8/tests/test_PyTorch.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.6/tests/test_Tensorflow.py` & `test_dvs_printf-1.8/tests/test_Tensorflow.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.6/tests/test__init__.py` & `test_dvs_printf-1.8/tests/test__init__.py`

 * *Files identical despite different names*

### Comparing `test_dvs_printf-1.6/tests/test_listfunction.py` & `test_dvs_printf-1.8/tests/test_listfunction.py`

 * *Files identical despite different names*

