# Comparing `tmp/pyedaa_reports-0.8.0.tar.gz` & `tmp/pyedaa_reports-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedaa_reports-0.8.0.tar", last modified: Mon May  6 20:02:04 2024, max compression
+gzip compressed data, was "pyedaa_reports-0.9.0.tar", last modified: Sun Jun  2 08:26:48 2024, max compression
```

## Comparing `pyedaa_reports-0.8.0.tar` & `pyedaa_reports-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:04.289921 pyedaa_reports-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-06 20:02:04.289921 pyedaa_reports-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:04.277921 pyedaa_reports-0.8.0/pyEDAA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:04.281921 pyedaa_reports-0.8.0/pyEDAA/Reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:04.281921 pyedaa_reports-0.8.0/pyEDAA/Reports/CLI/
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/CLI/Unittesting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:04.281921 pyedaa_reports-0.8.0/pyEDAA/Reports/Dependency/
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/Dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:04.281921 pyedaa_reports-0.8.0/pyEDAA/Reports/DocumentationCoverage/
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/DocumentationCoverage/Python.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/DocumentationCoverage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:04.281921 pyedaa_reports-0.8.0/pyEDAA/Reports/Requirement/
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/Requirement/Python.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/Requirement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:04.281921 pyedaa_reports-0.8.0/pyEDAA/Reports/Unittesting/
--rw-r--r--   0 runner    (1001) docker     (127)    34218 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/Unittesting/JUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/Unittesting/OSVVM.py
--rw-r--r--   0 runner    (1001) docker     (127)    38772 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/Unittesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:04.285921 pyedaa_reports-0.8.0/pyEDAA/Reports/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/resources/Unittesting.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyEDAA/Reports/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:02:04.285921 pyedaa_reports-0.8.0/pyEDAA.Reports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-06 20:02:04.000000 pyedaa_reports-0.8.0/pyEDAA.Reports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-06 20:02:04.000000 pyedaa_reports-0.8.0/pyEDAA.Reports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:02:04.000000 pyedaa_reports-0.8.0/pyEDAA.Reports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 20:02:04.000000 pyedaa_reports-0.8.0/pyEDAA.Reports.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-06 20:02:04.000000 pyedaa_reports-0.8.0/pyEDAA.Reports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 20:02:04.000000 pyedaa_reports-0.8.0/pyEDAA.Reports.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:02:04.289921 pyedaa_reports-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-06 20:02:00.000000 pyedaa_reports-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.052017 pyedaa_reports-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-06-02 08:26:48.052017 pyedaa_reports-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.040017 pyedaa_reports-0.9.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.040017 pyedaa_reports-0.9.0/examples/Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.040017 pyedaa_reports-0.9.0/examples/Python/pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/examples/Python/pytest/TestModuleA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/examples/Python/pytest/TestModuleB.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.040017 pyedaa_reports-0.9.0/pyEDAA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.040017 pyedaa_reports-0.9.0/pyEDAA/Reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.044017 pyedaa_reports-0.9.0/pyEDAA/Reports/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/CLI/Unittesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.044017 pyedaa_reports-0.9.0/pyEDAA/Reports/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/Dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.044017 pyedaa_reports-0.9.0/pyEDAA/Reports/DocumentationCoverage/
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/DocumentationCoverage/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/DocumentationCoverage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.044017 pyedaa_reports-0.9.0/pyEDAA/Reports/OSVVM/
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/OSVVM/AlertLog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/OSVVM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.044017 pyedaa_reports-0.9.0/pyEDAA/Reports/Requirement/
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/Requirement/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/Requirement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.044017 pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.044017 pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/JUnit/
+-rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/JUnit/AntJUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/JUnit/CTestJUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16797 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/JUnit/GoogleTestJUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16794 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/JUnit/PyTestJUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38986 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/JUnit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/OSVVM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39259 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.044017 pyedaa_reports-0.9.0/pyEDAA/Reports/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/resources/Ant-JUnit.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/resources/CTest-JUnit.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/resources/Generic-JUnit.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/resources/GoogleTest-JUnit.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/resources/PyTest-JUnit.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyEDAA/Reports/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 08:26:48.044017 pyedaa_reports-0.9.0/pyEDAA.Reports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-06-02 08:26:48.000000 pyedaa_reports-0.9.0/pyEDAA.Reports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-06-02 08:26:48.000000 pyedaa_reports-0.9.0/pyEDAA.Reports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 08:26:48.000000 pyedaa_reports-0.9.0/pyEDAA.Reports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 08:26:48.000000 pyedaa_reports-0.9.0/pyEDAA.Reports.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-02 08:26:48.000000 pyedaa_reports-0.9.0/pyEDAA.Reports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 08:26:48.000000 pyedaa_reports-0.9.0/pyEDAA.Reports.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 08:26:48.052017 pyedaa_reports-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-06-02 08:26:41.000000 pyedaa_reports-0.9.0/setup.py
```

### Comparing `pyedaa_reports-0.8.0/LICENSE.md` & `pyedaa_reports-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.8.0/PKG-INFO` & `pyedaa_reports-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.8.0
+Version: 0.9.0
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
@@ -18,61 +18,61 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: pyTooling~=6.1
+Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: lxml~=5.1
 Provides-Extra: doc
+Requires-Dist: pyTooling~=6.1; extra == "doc"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
 Requires-Dist: docutils~=0.18.1; extra == "doc"
 Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: lxml~=5.1; extra == "doc"
-Requires-Dist: sphinx_reports~=0.6; extra == "doc"
 Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
-Requires-Dist: setuptools~=69.5; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
-Requires-Dist: pyTooling~=6.1; extra == "doc"
 Requires-Dist: sphinx~=7.3; extra == "doc"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
+Requires-Dist: lxml~=5.1; extra == "doc"
+Requires-Dist: setuptools~=70.0; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
 Provides-Extra: test
+Requires-Dist: pyTooling~=6.1; extra == "test"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
-Requires-Dist: lxml~=5.1; extra == "test"
-Requires-Dist: pytest~=8.2; extra == "test"
-Requires-Dist: typing_extensions~=4.11; extra == "test"
 Requires-Dist: mypy~=1.10; extra == "test"
-Requires-Dist: pytest-cov~=5.0; extra == "test"
-Requires-Dist: pyTooling~=6.1; extra == "test"
+Requires-Dist: typing_extensions~=4.12; extra == "test"
+Requires-Dist: pytest~=8.2; extra == "test"
 Requires-Dist: Coverage~=7.5; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
+Requires-Dist: lxml~=5.1; extra == "test"
 Provides-Extra: all
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
 Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: docutils~=0.18.1; extra == "all"
-Requires-Dist: lxml~=5.1; extra == "all"
-Requires-Dist: typing_extensions~=4.11; extra == "all"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
+Requires-Dist: setuptools~=70.0; extra == "all"
 Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: docutils~=0.18.1; extra == "all"
 Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
 Requires-Dist: pytest-cov~=5.0; extra == "all"
-Requires-Dist: pytest~=8.2; extra == "all"
 Requires-Dist: sphinx_reports~=0.6; extra == "all"
-Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
-Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
+Requires-Dist: typing_extensions~=4.12; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: sphinx_design>=0.5.0; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyedaa_reports-0.8.0/README.md` & `pyedaa_reports-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/CLI/__init__.py` & `pyedaa_reports-0.9.0/pyEDAA/Reports/CLI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/Dependency/__init__.py` & `pyedaa_reports-0.9.0/pyEDAA/Reports/Dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/DocumentationCoverage/Python.py` & `pyedaa_reports-0.9.0/pyEDAA/Reports/DocumentationCoverage/Python.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/DocumentationCoverage/__init__.py` & `pyedaa_reports-0.9.0/pyEDAA/Reports/DocumentationCoverage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 class Base(metaclass=ExtendedType, slots=True):
 	_parent: Nullable["Base"]
 	_name:   str
 	_status: CoverageState
 
 	def __init__(self, name: str, parent: Nullable["Base"] = None):
 		if name is None:
-			raise TypeError(f"Parameter 'name' must not be None.")
+			raise ValueError(f"Parameter 'name' must not be None.")
 
 		self._parent = parent
 		self._name = name
 		self._status = CoverageState.Unknown
 
 	@property
 	def Parent(self) -> Nullable["Base"]:
```

### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/Requirement/Python.py` & `pyedaa_reports-0.9.0/pyEDAA/Reports/Requirement/Python.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,12 +63,12 @@
 	def __init__(self, path: Path, parse: bool = False) -> None:
 		self._path = path
 
 		if parse:
 			self.Parse()
 
 	def Parse(self) -> None:
-		with self._path.open("r") as file:
+		with self._path.open("r", encoding="utf-8") as file:
 			lines = file.readline()
 
 		for line in lines:
 			pass
```

### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/Requirement/__init__.py` & `pyedaa_reports-0.9.0/pyEDAA/Reports/Requirement/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/Unittesting/JUnit.py` & `pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/JUnit/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,24 +31,27 @@
 #
 """
 Reader for JUnit unit testing summary files in XML format.
 """
 from datetime        import datetime, timedelta
 from enum            import Flag
 from pathlib         import Path
+from sys             import version_info
 from time            import perf_counter_ns
-from typing          import Optional as Nullable, Iterable, Dict, Any, Generator, Tuple, Union, TypeVar
+from typing          import Optional as Nullable, Iterable, Dict, Any, Generator, Tuple, Union, TypeVar, Type, ClassVar
 
-from lxml.etree                 import XMLParser, parse, XMLSchema, XMLSyntaxError, _ElementTree, _Element, _Comment
+from lxml.etree                 import XMLParser, parse, XMLSchema, XMLSyntaxError, _ElementTree, _Element, _Comment, XMLSchemaParseError
 from lxml.etree                 import ElementTree, Element, SubElement, tostring
+from pyTooling.Common           import getFullyQualifiedName, getResourceFile
 from pyTooling.Decorators       import export, readonly
+from pyTooling.Exceptions       import ToolingException
 from pyTooling.MetaClasses      import ExtendedType, mustoverride, abstractmethod
 from pyTooling.Tree             import Node
 
-from pyEDAA.Reports             import resources, getResourceFile
+from pyEDAA.Reports             import resources
 from pyEDAA.Reports.Unittesting import UnittestException, DuplicateTestsuiteException, DuplicateTestcaseException, \
 	TestsuiteKind
 from pyEDAA.Reports.Unittesting import TestcaseStatus, TestsuiteStatus, IterationScheme
 from pyEDAA.Reports.Unittesting import Document as ut_Document, TestsuiteSummary as ut_TestsuiteSummary
 from pyEDAA.Reports.Unittesting import Testsuite as ut_Testsuite, Testcase as ut_Testcase
 
 
@@ -88,15 +91,18 @@
 	_parent:         Nullable["Testsuite"]
 	_name:           str
 
 	def __init__(self, name: str, parent: Nullable["Testsuite"] = None):
 		if name is None:
 			raise ValueError(f"Parameter 'name' is None.")
 		elif not isinstance(name, str):
-			raise TypeError(f"Parameter 'name' is not of type 'str'.")
+			ex = TypeError(f"Parameter 'name' is not of type 'str'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(name)}'.")
+			raise ex
 
 		# TODO: check parameter parent
 
 		self._parent = parent
 		self._name = name
 
 	@readonly
@@ -164,15 +170,18 @@
 		duration:  Nullable[timedelta] = None,
 		status: TestcaseStatus = TestcaseStatus.Unknown,
 		assertionCount: Nullable[int] = None,
 		parent: Nullable["Testclass"] = None
 	):
 		if parent is not None:
 			if not isinstance(parent, Testclass):
-				raise TypeError(f"Parameter 'parent' is not of type 'Class'.")
+				ex = TypeError(f"Parameter 'parent' is not of type 'Testclass'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(parent)}'.")
+				raise ex
 
 			parent._testcases[name] = self
 
 		super().__init__(name, duration, assertionCount, parent)
 
 		self._status = status
 
@@ -196,26 +205,23 @@
 		return self.__class__(
 			self._name,
 			self._duration,
 			self._status,
 			self._assertionCount
 		)
 
-	def Aggregate(self, strict: bool = True) -> None:  # TestcaseAggregateReturnType:
+	def Aggregate(self) -> None:
 		if self._status is TestcaseStatus.Unknown:
 			if self._assertionCount is None:
 				self._status = TestcaseStatus.Passed
 			elif self._assertionCount == 0:
 				self._status = TestcaseStatus.Weak
 			else:
 				self._status = TestcaseStatus.Failed
 
-				if strict:
-					self._status = self._status & ~TestcaseStatus.Passed | TestcaseStatus.Failed
-
 			# TODO: check for setup errors
 			# TODO: check for teardown errors
 
 	@classmethod
 	def FromTestcase(cls, testcase: ut_Testcase) -> "Testcase":
 		return cls(
 			testcase._name,
@@ -237,16 +243,18 @@
 		node["status"] = self._status
 		node["assertionCount"] = self._assertionCount
 		node["duration"] = self._duration
 
 		return node
 
 	def __str__(self) -> str:
+		moduleName = self.__module__.split(".")[-1]
+		className = self.__class__.__name__
 		return (
-			f"<JUnit.Testcase {self._name}: {self._status.name} - asserts:{self._assertionCount}>"
+			f"<{moduleName}{className} {self._name}: {self._status.name} - asserts:{self._assertionCount}>"
 		)
 
 
 @export
 class TestsuiteBase(BaseWithProperties):
 	_startTime: Nullable[datetime]
 	_status:    TestsuiteStatus
@@ -338,16 +346,18 @@
 	def __init__(
 		self,
 		classname: str,
 		testcases: Nullable[Iterable["Testcase"]] = None,
 		parent: Nullable["Testsuite"] = None
 	):
 		if parent is not None:
-			if not isinstance(parent, Testsuite):
-				raise TypeError(f"Parameter 'parent' is not of type 'Testsuite'.")
+			# if not isinstance(parent, Testsuite):
+			# 	raise TypeError(f"Parameter 'parent' is not of type 'Testsuite'.")
+			#	ex.add_note(f"Got type '{getFullyQualifiedName(parent)}'.")
+			#	raise ex
 
 			parent._testclasses[classname] = self
 
 		super().__init__(classname, parent)
 
 		self._testcases = {}
 		if testcases is not None:
@@ -397,27 +407,29 @@
 			TestsuiteKind.Class,
 			# startTime=self._startTime,
 			# totalDuration=self._duration,
 			# status=self._status,
 			testcases=(tc.ToTestcase() for tc in self._testcases.values())
 		)
 
-	def __str__(self) -> str:
-		return (
-			f"<JUnit.Class {self._name}: {len(self._testcases)}>"
-		)
-
 	def ToTree(self) -> Node:
 		node = Node(
 			value=self._name,
 			children=(tc.ToTree() for tc in self._testcases.values())
 		)
 
 		return node
 
+	def __str__(self) -> str:
+		moduleName = self.__module__.split(".")[-1]
+		className = self.__class__.__name__
+		return (
+			f"<{moduleName}{className} {self._name}: {len(self._testcases)}>"
+		)
+
 
 @export
 class Testsuite(TestsuiteBase):
 	_hostname:    str
 	_testclasses: Dict[str, "Testclass"]
 
 	def __init__(
@@ -428,15 +440,18 @@
 		duration:  Nullable[timedelta] = None,
 		status: TestsuiteStatus = TestsuiteStatus.Unknown,
 		testclasses: Nullable[Iterable["Testclass"]] = None,
 		parent: Nullable["TestsuiteSummary"] = None
 	):
 		if parent is not None:
 			if not isinstance(parent, TestsuiteSummary):
-				raise TypeError(f"Parameter 'parent' is not of type 'TestsuiteSummary'.")
+				ex = TypeError(f"Parameter 'parent' is not of type 'TestsuiteSummary'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(parent)}'.")
+				raise ex
 
 			parent._testsuites[name] = self
 
 		super().__init__(name, startTime, duration, status, parent)
 
 		self._hostname = hostname
 
@@ -504,34 +519,34 @@
 			self._duration,
 			self._status
 		)
 
 	def Aggregate(self, strict: bool = True) -> TestsuiteAggregateReturnType:
 		tests, skipped, errored, failed, passed = super().Aggregate()
 
-		for testcase in self._testclasses.values():
-			_ = testcase.Aggregate(strict)
+		for testclass in self._testclasses.values():
+			_ = testclass.Aggregate(strict)
 
 			tests += 1
 
-			status = testcase._status
+			status = testclass._status
 			if status is TestcaseStatus.Unknown:
-				raise UnittestException(f"Found testcase '{testcase._name}' with state 'Unknown'.")
+				raise UnittestException(f"Found testclass '{testclass._name}' with state 'Unknown'.")
 			elif status is TestcaseStatus.Skipped:
 				skipped += 1
 			elif status is TestcaseStatus.Errored:
 				errored += 1
 			elif status is TestcaseStatus.Passed:
 				passed += 1
 			elif status is TestcaseStatus.Failed:
 				failed += 1
 			elif status & TestcaseStatus.Mask is not TestcaseStatus.Unknown:
-				raise UnittestException(f"Found testcase '{testcase._name}' with unsupported state '{status}'.")
+				raise UnittestException(f"Found testclass '{testclass._name}' with unsupported state '{status}'.")
 			else:
-				raise UnittestException(f"Internal error for testcase '{testcase._name}', field '_status' is '{status}'.")
+				raise UnittestException(f"Internal error for testclass '{testclass._name}', field '_status' is '{status}'.")
 
 		self._tests = tests
 		self._skipped = skipped
 		self._errored = errored
 		self._failed = failed
 		self._passed = passed
 
@@ -640,16 +655,18 @@
 		)
 		node["startTime"] = self._startTime
 		node["duration"] = self._duration
 
 		return node
 
 	def __str__(self) -> str:
+		moduleName = self.__module__.split(".")[-1]
+		className = self.__class__.__name__
 		return (
-			f"<JUnit.Testsuite {self._name}: {self._status.name} - tests:{self._tests}>"
+			f"<{moduleName}{className} {self._name}: {self._status.name} - tests:{self._tests}>"
 		)
 
 
 @export
 class TestsuiteSummary(TestsuiteBase):
 	_testsuites: Dict[str, Testsuite]
 
@@ -765,23 +782,29 @@
 		)
 		node["startTime"] = self._startTime
 		node["duration"] = self._duration
 
 		return node
 
 	def __str__(self) -> str:
+		moduleName = self.__module__.split(".")[-1]
+		className = self.__class__.__name__
 		return (
-			f"<JUnit.TestsuiteSummary {self._name}: {self._status.name} - tests:{self._tests}>"
+			f"<{moduleName}{className} {self._name}: {self._status.name} - tests:{self._tests}>"
 		)
 
 
 @export
 class Document(TestsuiteSummary, ut_Document):
-	_readerMode:       JUnitReaderMode
-	_xmlDocument:      Nullable[_ElementTree]
+	_TESTCASE:          ClassVar[Type[Testcase]] =         Testcase
+	_TESTCLASS:         ClassVar[Type[Testclass]] =        Testclass
+	_TESTSUITE:         ClassVar[Type[Testsuite]] =        Testsuite
+
+	_readerMode:        JUnitReaderMode
+	_xmlDocument:       Nullable[_ElementTree]
 
 	def __init__(self, xmlReportFile: Path, parse: bool = False, readerMode: JUnitReaderMode = JUnitReaderMode.Default):
 		super().__init__("Unprocessed JUnit XML file")
 		ut_Document.__init__(self, xmlReportFile)
 
 		self._readerMode = readerMode
 		self._xmlDocument = None
@@ -804,34 +827,49 @@
 		doc._passed = testsuiteSummary._passed
 
 		doc.AddTestsuites(Testsuite.FromTestsuite(testsuite) for testsuite in testsuiteSummary._testsuites.values())
 
 		return doc
 
 	def Read(self) -> None:
+		xmlSchemaFile = "Generic-JUnit.xsd"
+		self._Read(xmlSchemaFile)
+
+	def _Read(self, xmlSchemaFile: str) -> None:
 		if not self._path.exists():
 			raise UnittestException(f"JUnit XML file '{self._path}' does not exist.") \
 				from FileNotFoundError(f"File '{self._path}' not found.")
 
 		startAnalysis = perf_counter_ns()
 		try:
-			# xmlSchemaFile = getResourceFile(resources, "JUnit.xsd")
-			xmlSchemaFile = getResourceFile(resources, "Unittesting.xsd")
+			xmlSchemaResourceFile = getResourceFile(resources, xmlSchemaFile)
+		except ToolingException as ex:
+			raise UnittestException(f"Couldn't locate XML Schema '{xmlSchemaFile}' in package resources.") from ex
+
+		try:
 			schemaParser = XMLParser(ns_clean=True)
-			schemaRoot = parse(xmlSchemaFile, schemaParser)
+			schemaRoot = parse(xmlSchemaResourceFile, schemaParser)
+		except XMLSyntaxError as ex:
+			raise UnittestException(f"XML Syntax Error while parsing XML Schema '{xmlSchemaFile}'.") from ex
 
+		try:
 			junitSchema = XMLSchema(schemaRoot)
+		except XMLSchemaParseError as ex:
+			raise UnittestException(f"Error while parsing XML Schema '{xmlSchemaFile}'.")
+
+		try:
 			junitParser = XMLParser(schema=junitSchema, ns_clean=True)
 			junitDocument = parse(self._path, parser=junitParser)
 
 			self._xmlDocument = junitDocument
 		except XMLSyntaxError as ex:
-			print(ex)
-
-			print(junitParser.error_log)
+			if version_info >= (3, 11):  # pragma: no cover
+				for logEntry in junitParser.error_log:
+					ex.add_note(str(logEntry))
+			raise UnittestException(f"XML syntax or validation error for '{self._path}'.") from ex
 		except Exception as ex:
 			raise UnittestException(f"Couldn't open '{self._path}'.") from ex
 
 		endAnalysis = perf_counter_ns()
 		self._analysisDuration = (endAnalysis - startAnalysis) / 1e9
 
 	def Write(self, path: Nullable[Path] = None, overwrite: bool = False, regenerate: bool = False) -> None:
@@ -858,112 +896,183 @@
 			ex = UnittestException(f"JUnit XML file '{self._path}' needs to be read and analyzed by an XML parser.")
 			ex.add_note(f"Call 'JUnitDocument.Read()' or create document using 'JUnitDocument(path, parse=True)'.")
 			raise ex
 
 		startConversion = perf_counter_ns()
 		rootElement: _Element = self._xmlDocument.getroot()
 
-		self._name =      rootElement.attrib["name"]                              if "name"      in rootElement.attrib else "root"
-		self._startTime = datetime.fromisoformat(rootElement.attrib["timestamp"]) if "timestamp" in rootElement.attrib else None
-		self._duration =  timedelta(seconds=float(rootElement.attrib["time"]))    if "time"      in rootElement.attrib else None
-
-		# tests = rootElement.getAttribute("tests")
-		# skipped = rootElement.getAttribute("skipped")
-		# errors = rootElement.getAttribute("errors")
-		# failures = rootElement.getAttribute("failures")
-		# assertions = rootElement.getAttribute("assertions")
+		self._name = self._ParseName(rootElement, optional=True)
+		self._startTime = self._ParseTimestamp(rootElement, optional=True)
+		self._duration = self._ParseTime(rootElement, optional=True)
+
+		if False:  # self._readerMode is JUnitReaderMode.
+			self._tests = self._ParseTests(testsuitesNode)
+			self._skipped = self._ParseSkipped(testsuitesNode)
+			self._errored = self._ParseErrors(testsuitesNode)
+			self._failed = self._ParseFailures(testsuitesNode)
+			self._assertionCount = self._ParseAssertions(testsuitesNode)
 
 		for rootNode in rootElement.iterchildren(tag="testsuite"):  # type: _Element
 			self._ParseTestsuite(self, rootNode)
 
-		self.Aggregate()
+		if True:  # self._readerMode is JUnitReaderMode.
+			self.Aggregate()
+
 		endConversation = perf_counter_ns()
 		self._modelConversion = (endConversation - startConversion) / 1e9
 
-	def _ParseTestsuite(self, parent: TestsuiteSummary, testsuitesNode: _Element) -> None:
-		name = testsuitesNode.attrib["name"]
+	def _ParseName(self, element: _Element, default: str = "root", optional: bool = True) -> str:
+		if "name" in element.attrib:
+			return element.attrib["name"]
+		elif not optional:
+			raise UnittestException(f"Required parameter 'name' not found in tag '{element.tag}'.")
+		else:
+			return default
+
+	def _ParseTimestamp(self, element: _Element, optional: bool = True) -> Nullable[datetime]:
+		if "timestamp" in element.attrib:
+			timestamp = element.attrib["timestamp"]
+			return datetime.fromisoformat(timestamp)
+		elif not optional:
+			raise UnittestException(f"Required parameter 'timestamp' not found in tag '{element.tag}'.")
+		else:
+			return None
+
+	def _ParseTime(self, element: _Element, optional: bool = True) -> Nullable[timedelta]:
+		if "time" in element.attrib:
+			time = element.attrib["time"]
+			return timedelta(seconds=float(time))
+		elif not optional:
+			raise UnittestException(f"Required parameter 'time' not found in tag '{element.tag}'.")
+		else:
+			return None
+
+	def _ParseHostname(self, element: _Element, default: str = "localhost", optional: bool = True) -> str:
+		if "hostname" in element.attrib:
+			return element.attrib["hostname"]
+		elif not optional:
+			raise UnittestException(f"Required parameter 'hostname' not found in tag '{element.tag}'.")
+		else:
+			return default
+
+	def _ParseClassname(self, element: _Element, optional: bool = True) -> str:
+		if "classname" in element.attrib:
+			return element.attrib["classname"]
+		elif not optional:
+			raise UnittestException(f"Required parameter 'classname' not found in tag '{element.tag}'.")
+
+	def _ParseTests(self, element: _Element, default: Nullable[int] = None, optional: bool = True) -> Nullable[int]:
+		if "tests" in element.attrib:
+			return int(element.attrib["tests"])
+		elif not optional:
+			raise UnittestException(f"Required parameter 'tests' not found in tag '{element.tag}'.")
+		else:
+			return default
+
+	def _ParseSkipped(self, element: _Element, default: Nullable[int] = None, optional: bool = True) -> Nullable[int]:
+		if "skipped" in element.attrib:
+			return int(element.attrib["skipped"])
+		elif not optional:
+			raise UnittestException(f"Required parameter 'skipped' not found in tag '{element.tag}'.")
+		else:
+			return default
 
-		kwargs = {}
-		if "timestamp" in testsuitesNode.attrib:
-			kwargs["startTime"] = datetime.fromisoformat(testsuitesNode.attrib["timestamp"])
-		if "time" in testsuitesNode.attrib:
-			kwargs["duration"] = timedelta(seconds=float(testsuitesNode.attrib["time"]))
-		if "hostname" in testsuitesNode.attrib:
-			kwargs["hostname"] = testsuitesNode.attrib["hostname"]
-
-		newTestsuite = Testsuite(
-			name,
-			**kwargs,
+	def _ParseErrors(self, element: _Element, default: Nullable[int] = None, optional: bool = True) -> Nullable[int]:
+		if "errors" in element.attrib:
+			return int(element.attrib["errors"])
+		elif not optional:
+			raise UnittestException(f"Required parameter 'errors' not found in tag '{element.tag}'.")
+		else:
+			return default
+
+	def _ParseFailures(self, element: _Element, default: Nullable[int] = None, optional: bool = True) -> Nullable[int]:
+		if "failures" in element.attrib:
+			return int(element.attrib["failures"])
+		elif not optional:
+			raise UnittestException(f"Required parameter 'failures' not found in tag '{element.tag}'.")
+		else:
+			return default
+
+	def _ParseAssertions(self, element: _Element, default: Nullable[int] = None, optional: bool = True) -> Nullable[int]:
+		if "assertions" in element.attrib:
+			return int(element.attrib["assertions"])
+		elif not optional:
+			raise UnittestException(f"Required parameter 'assertions' not found in tag '{element.tag}'.")
+		else:
+			return default
+
+	def _ParseTestsuite(self, parent: TestsuiteSummary, testsuitesNode: _Element) -> None:
+		newTestsuite = self._TESTSUITE(
+			self._ParseName(testsuitesNode, optional=False),
+			self._ParseHostname(testsuitesNode, optional=True),
+			self._ParseTimestamp(testsuitesNode, optional=True),
+			self._ParseTime(testsuitesNode, optional=True),
 			parent=parent
 		)
 
-		# if self._readerMode is JUnitReaderMode.Default:
-		# 	currentTestsuite = parent
-		# elif self._readerMode is JUnitReaderMode.DecoupleTestsuiteHierarchyAndTestcaseClassName:
-		# 	currentTestsuite = newTestsuite
-		# else:
-		# 	raise UnittestException(f"Unknown reader mode '{self._readerMode}'.")
+		if False:  # self._readerMode is JUnitReaderMode.
+			self._tests = self._ParseTests(testsuitesNode)
+			self._skipped = self._ParseSkipped(testsuitesNode)
+			self._errored = self._ParseErrors(testsuitesNode)
+			self._failed = self._ParseFailures(testsuitesNode)
+			self._assertionCount = self._ParseAssertions(testsuitesNode)
+
+		self._ParseTestsuiteChildren(testsuitesNode, newTestsuite)
 
+	def _ParseTestsuiteChildren(self, testsuitesNode: _Element, newTestsuite: Testsuite) -> None:
 		for node in testsuitesNode.iterchildren():   # type: _Element
 			# if node.tag == "testsuite":
 			# 	self._ParseTestsuite(newTestsuite, node)
 			# el
 			if node.tag == "testcase":
 				self._ParseTestcase(newTestsuite, node)
 
-	def _ParseTestcase(self, parent: Testsuite, testsuiteNode: _Element) -> None:
-		name = testsuiteNode.attrib["name"]
-		className = testsuiteNode.attrib["classname"]
-		time = float(testsuiteNode.attrib["time"])
-
-		# if self._readerMode is JUnitReaderMode.Default:
-		# 	currentTestsuite = self
-		# elif self._readerMode is JUnitReaderMode.DecoupleTestsuiteHierarchyAndTestcaseClassName:
-		# 	currentTestsuite = parentTestsuite
-		# else:
-		# 	raise UnittestException(f"Unknown reader mode '{self._readerMode}'.")
-
-		# testsuitePath = className.split(".")
-		# for testsuiteName in testsuitePath:
-		# 	try:
-		# 		currentTestsuite = currentTestsuite._testsuites[testsuiteName]
-		# 	except KeyError:
-		# 		currentTestsuite._testsuites[testsuiteName] = new = Testsuite(testsuiteName)
-		# 		currentTestsuite = new
+	def _ParseTestcase(self, parent: Testsuite, testcaseNode: _Element) -> None:
+		className = self._ParseClassname(testcaseNode, optional=False)
+		testclass = self._FindOrCreateTestclass(parent, className)
+
+		newTestcase = self._TESTCASE(
+			self._ParseName(testcaseNode, optional=False),
+			self._ParseTime(testcaseNode, optional=False),
+			assertionCount=self._ParseAssertions(testcaseNode),
+			parent=testclass
+		)
 
+		self._ParseTestcaseChildren(testcaseNode, newTestcase)
+
+	def _FindOrCreateTestclass(self, parent: Testsuite, className: str) -> Testclass:
 		if className in parent._testclasses:
-			testclass = parent._testclasses[className]
+			return parent._testclasses[className]
 		else:
-			testclass = Testclass(className, parent=parent)
-
-		testcase = Testcase(name, duration=timedelta(seconds=time), parent=testclass)
+			return self._TESTCLASS(className, parent=parent)
 
-		for node in testsuiteNode.iterchildren():   # type: _Element
+	def _ParseTestcaseChildren(self, testcaseNode: _Element, newTestcase: Testcase) -> None:
+		for node in testcaseNode.iterchildren():   # type: _Element
 			if isinstance(node, _Comment):
 				pass
 			elif isinstance(node, _Element):
 				if node.tag == "skipped":
-					testcase._status = TestcaseStatus.Skipped
+					newTestcase._status = TestcaseStatus.Skipped
 				elif node.tag == "failure":
-					testcase._status = TestcaseStatus.Failed
+					newTestcase._status = TestcaseStatus.Failed
 				elif node.tag == "error":
-					testcase._status = TestcaseStatus.Errored
+					newTestcase._status = TestcaseStatus.Errored
 				elif node.tag == "system-out":
 					pass
 				elif node.tag == "system-err":
 					pass
 				elif node.tag == "properties":
 					pass
 				else:
 					raise UnittestException(f"Unknown element '{node.tag}' in junit file.")
 			else:
 				pass
 
-		if testcase._status is TestcaseStatus.Unknown:
-			testcase._status = TestcaseStatus.Passed
+		if newTestcase._status is TestcaseStatus.Unknown:
+			newTestcase._status = TestcaseStatus.Passed
 
 	def Generate(self, overwrite: bool = False) -> None:
 		if self._xmlDocument is not None:
 			raise UnittestException(f"Internal XML document is populated with data.")
 
 		rootElement = Element("testsuites")
 		rootElement.attrib["name"] = self._name
@@ -1019,10 +1128,12 @@
 			failureElement = SubElement(testcaseElement, "failure")
 		elif testcase._status is TestcaseStatus.Skipped:
 			skippedElement = SubElement(testcaseElement, "skipped")
 		else:
 			errorElement = SubElement(testcaseElement, "error")
 
 	def __str__(self) -> str:
+		moduleName = self.__module__.split(".")[-1]
+		className = self.__class__.__name__
 		return (
-			f"<JUnit.Document {self._name} ({self._path}): {self._status.name} - suites/tests:{self.TestsuiteCount}/{self.TestcaseCount}>"
+			f"<{moduleName}{className} {self._name} ({self._path}): {self._status.name} - suites/tests:{self.TestsuiteCount}/{self.TestcaseCount}>"
 		)
```

### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/Unittesting/OSVVM.py` & `pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/OSVVM.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,22 @@
 # See the License for the specific language governing permissions and                                                  #
 # limitations under the License.                                                                                       #
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """Reader for OSVVM test report summary files in YAML format."""
-from datetime             import timedelta, datetime
-from pathlib              import Path
-from time                 import perf_counter_ns
-from typing               import Optional as Nullable
-
-from ruamel.yaml          import YAML
-from pyTooling.Decorators import export, notimplemented
+from datetime              import timedelta, datetime
+from pathlib               import Path
+from time                  import perf_counter_ns
+from typing                import Optional as Nullable
+
+from ruamel.yaml           import YAML
+from pyTooling.Decorators  import export, notimplemented
+from ruamel.yaml.timestamp import TimeStamp
 
 from pyEDAA.Reports.Unittesting import UnittestException, Document, TestcaseStatus
 from pyEDAA.Reports.Unittesting import TestsuiteSummary as ut_TestsuiteSummary, Testsuite as ut_Testsuite
 from pyEDAA.Reports.Unittesting import Testcase as ut_Testcase
 
 
 @export
@@ -49,25 +50,25 @@
 
 @export
 class UnittestException(UnittestException, OsvvmException):
 	pass
 
 
 @export
-class TestsuiteSummary(ut_TestsuiteSummary):
+class Testcase(ut_Testcase):
 	pass
 
 
 @export
 class Testsuite(ut_Testsuite):
 	pass
 
 
 @export
-class Testcase(ut_Testcase):
+class TestsuiteSummary(ut_TestsuiteSummary):
 	pass
 
 
 @export
 class OsvvmYamlDocument(TestsuiteSummary, Document):
 	_yamlDocument: Nullable[YAML]
 
@@ -109,26 +110,29 @@
 		# 	self.Generate(overwrite=True)
 
 		if self._yamlDocument is None:
 			ex = UnittestException(f"Internal YAML document tree is empty and needs to be generated before write is possible.")
 			ex.add_note(f"Call 'OsvvmYamlDocument.Generate()' or 'OsvvmYamlDocument.Write(..., regenerate=True)'.")
 			raise ex
 
-		# with path.open("w") as file:
+		# with path.open("w", encoding="utf-8") as file:
 		# 	self._yamlDocument.writexml(file, addindent="\t", encoding="utf-8", newl="\n")
 
 	def Parse(self) -> None:
 		if self._yamlDocument is None:
 			ex = UnittestException(f"OSVVM YAML file '{self._path}' needs to be read and analyzed by a YAML parser.")
 			ex.add_note(f"Call 'OsvvmYamlDocument.Read()' or create document using 'OsvvmYamlDocument(path, parse=True)'.")
 			raise ex
 
 		startConversion = perf_counter_ns()
-		self._startTime = datetime.fromisoformat(self._yamlDocument["Date"])
-		# yamlBuild = self._yamlDocument["BuildInfo"]
+		startTime = self._yamlDocument["Date"]
+		if isinstance(startTime, TimeStamp):
+			self._startTime = startTime
+		else:
+			self._startTime = datetime.fromisoformat(startTime)
 
 		for yamlTestsuite in self._yamlDocument['TestSuites']:
 			self._ParseTestsuite(self, yamlTestsuite)
 
 		self.Aggregate()
 		endConversation = perf_counter_ns()
 		self._modelConversion = (endConversation - startConversion) / 1e9
@@ -139,19 +143,20 @@
 
 		testsuite = Testsuite(
 			testsuiteName,
 			totalDuration=totalDuration,
 			parent=parentTestsuite
 		)
 
-		for yamlTestcase in yamlTestsuite['TestCases']:
-			self._ParseTestcase(testsuite, yamlTestcase)
+		if yamlTestsuite['TestCases'] is not None:
+			for yamlTestcase in yamlTestsuite['TestCases']:
+				self._ParseTestcase(testsuite, yamlTestcase)
 
 	def _ParseTestcase(self, parentTestsuite: Testsuite, yamlTestcase) -> None:
-		testcaseName = yamlTestcase["Name"]
+		testcaseName = yamlTestcase["TestCaseName"]
 		totalDuration = timedelta(seconds=float(yamlTestcase["ElapsedTime"]))
 		yamlStatus = yamlTestcase["Status"].lower()
 		yamlResults = yamlTestcase["Results"]
 		assertionCount = int(yamlResults["AffirmCount"])
 		passedAssertionCount = int(yamlResults["PassedCount"])
 		totalErrors = int(yamlResults["TotalErrors"])
 		warningCount = int(yamlResults["AlertCount"]["Warning"])
```

### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/Unittesting/__init__.py` & `pyedaa_reports-0.9.0/pyEDAA/Reports/Unittesting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """Abstraction of testsuites and testcases."""
 from datetime              import timedelta, datetime
 from enum                  import Flag, IntEnum
 from pathlib               import Path
+from sys                   import version_info
 from typing                import Optional as Nullable, Dict, Iterable, Any, Tuple, Generator, Union, List, Generic, TypeVar
 
+from pyTooling.Common      import getFullyQualifiedName
 from pyTooling.Decorators  import export, readonly
 from pyTooling.MetaClasses import ExtendedType, abstractmethod
 from pyTooling.Tree        import Node
 
 from pyEDAA.Reports        import ReportException
 
 
@@ -187,15 +189,18 @@
 		errorCount: int = 0,
 		fatalCount: int = 0,
 		parent: Nullable["Testsuite"] = None
 	):
 		if name is None:
 			raise ValueError(f"Parameter 'name' is None.")
 		elif not isinstance(name, str):
-			raise TypeError(f"Parameter 'name' is not of type 'str'.")
+			ex = TypeError(f"Parameter 'name' is not of type 'str'.")
+			if version_info >= (3, 11):  # pragma: no cover
+				ex.add_note(f"Got type '{getFullyQualifiedName(name)}'.")
+			raise ex
 
 		self._parent = parent
 		self._name = name
 
 		if testDuration is not None:
 			if setupDuration is not None:
 				if teardownDuration is not None:
@@ -330,15 +335,18 @@
 		warningCount: int = 0,
 		errorCount: int = 0,
 		fatalCount: int = 0,
 		parent: Nullable["Testsuite"] = None
 	):
 		if parent is not None:
 			if not isinstance(parent, Testsuite):
-				raise TypeError(f"Parameter 'parent' is not of type 'Testsuite'.")
+				ex = TypeError(f"Parameter 'parent' is not of type 'Testsuite'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(parent)}'.")
+				raise ex
 
 			parent._testcases[name] = self
 
 		super().__init__(name, startTime, setupDuration, testDuration, teardownDuration, totalDuration, warningCount, errorCount, fatalCount, parent)
 
 		self._status = status
 
@@ -473,15 +481,18 @@
 		errorCount: int = 0,
 		fatalCount: int = 0,
 		testsuites: Nullable[Iterable[TestsuiteType]] = None,
 		parent: Nullable["Testsuite"] = None
 	):
 		if parent is not None:
 			if not isinstance(parent, TestsuiteBase):
-				raise TypeError(f"Parameter 'parent' is not of type 'TestsuiteBase'.")
+				ex = TypeError(f"Parameter 'parent' is not of type 'TestsuiteBase'.")
+				if version_info >= (3, 11):  # pragma: no cover
+					ex.add_note(f"Got type '{getFullyQualifiedName(parent)}'.")
+				raise ex
 
 			parent._testsuites[name] = self
 
 		super().__init__(name, startTime, setupDuration, testDuration, teardownDuration, totalDuration, warningCount, errorCount, fatalCount, parent)
 
 		self._kind = kind
 		self._status = status
@@ -983,15 +994,15 @@
 
 	def __init__(
 		self,
 		testcase: Testcase,
 		parent: Nullable["Testsuite"] = None
 	):
 		if testcase is None:
-			raise TypeError(f"Parameter 'testcase' is None.")
+			raise ValueError(f"Parameter 'testcase' is None.")
 
 		super().__init__(
 			testcase._name,
 			testcase._startTime,
 			testcase._setupDuration, testcase._testDuration, testcase._teardownDuration, testcase._totalDuration,
 			TestcaseStatus.Unknown,
 			testcase._assertionCount, testcase._failedAssertionCount, testcase._passedAssertionCount,
@@ -1077,15 +1088,15 @@
 		self,
 		testsuite: Testsuite,
 		addTestsuites: bool = False,
 		addTestcases: bool = False,
 		parent: Nullable["Testsuite"] = None
 	):
 		if testsuite is None:
-			raise TypeError(f"Parameter 'testsuite' is None.")
+			raise ValueError(f"Parameter 'testsuite' is None.")
 
 		super().__init__(
 			testsuite._name,
 			testsuite._kind,
 			testsuite._startTime,
 			testsuite._setupDuration, testsuite._testDuration, testsuite._teardownDuration, testsuite._totalDuration,
 			TestsuiteStatus.Unknown,
```

### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/__init__.py` & `pyedaa_reports-0.9.0/pyEDAA/Reports/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,33 +31,25 @@
 """
 Various report abstract data models and report format converters.
 """
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
 __copyright__ = "2021-2024, Electronic Design Automation Abstraction (EDA²)"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.8.0"
+__version__ =   "0.9.0"
 __keywords__ =  ["Reports", "Abstract Model", "Data Model", "Unit Testing", "Testcase", "Testsuite", "OSVVM", "YAML", "XML"]
 
 from enum                 import Enum
-from importlib.resources  import files
-from pathlib              import Path
 from sys                  import version_info
-from types                import ModuleType
-from typing               import List, Union
+from typing               import List
 
 from pyTooling.Decorators import export
 
 
 @export
-def getResourceFile(module: Union[str, ModuleType], filename: str) -> Path:
-	return files(module) / filename
-
-
-@export
 class ReportException(Exception):
 	# WORKAROUND: for Python <3.11
 	# Implementing a dummy method for Python versions before
 	__notes__: List[str]
 	if version_info < (3, 11):  # pragma: no cover
 		def add_note(self, message: str) -> None:
 			try:
```

### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/resources/Unittesting.xsd` & `pyedaa_reports-0.9.0/pyEDAA/Reports/resources/PyTest-JUnit.xsd`

 * *Files 1% similar despite different names*

#### Comparing `pyedaa_reports-0.8.0/pyEDAA/Reports/resources/Unittesting.xsd` & `pyedaa_reports-0.9.0/pyEDAA/Reports/resources/PyTest-JUnit.xsd`

```diff
@@ -61,15 +61,15 @@
       <xsd:element name="system-err" type="literalblock" minOccurs="0">
         <xsd:annotation>
           <xsd:documentation xml:lang="en"/>
         </xsd:annotation>
       </xsd:element>
     </xsd:sequence>
     <xsd:attribute name="name" type="xsd:string" use="required"/>
-    <xsd:attribute name="classname" type="xsd:string" use="optional"/>
+    <xsd:attribute name="classname" type="xsd:string" use="required"/>
     <xsd:attribute name="time" type="xsd:float" use="optional"/>
     <xsd:attribute name="assertions" type="xsd:nonNegativeInteger" use="optional"/>
     <xsd:attribute name="file" type="xsd:string" use="optional"/>
     <xsd:attribute name="line" type="xsd:nonNegativeInteger" use="optional"/>
   </xsd:complexType>
   <xsd:complexType name="testsuite">
     <xsd:sequence minOccurs="0" maxOccurs="unbounded">
```

### Comparing `pyedaa_reports-0.8.0/pyEDAA.Reports.egg-info/PKG-INFO` & `pyedaa_reports-0.9.0/pyEDAA.Reports.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.8.0
+Version: 0.9.0
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
@@ -18,61 +18,61 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: pyTooling~=6.1
+Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: lxml~=5.1
 Provides-Extra: doc
+Requires-Dist: pyTooling~=6.1; extra == "doc"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
 Requires-Dist: docutils~=0.18.1; extra == "doc"
 Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: lxml~=5.1; extra == "doc"
-Requires-Dist: sphinx_reports~=0.6; extra == "doc"
 Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
-Requires-Dist: setuptools~=69.5; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
-Requires-Dist: pyTooling~=6.1; extra == "doc"
 Requires-Dist: sphinx~=7.3; extra == "doc"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
+Requires-Dist: lxml~=5.1; extra == "doc"
+Requires-Dist: setuptools~=70.0; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
 Provides-Extra: test
+Requires-Dist: pyTooling~=6.1; extra == "test"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
-Requires-Dist: lxml~=5.1; extra == "test"
-Requires-Dist: pytest~=8.2; extra == "test"
-Requires-Dist: typing_extensions~=4.11; extra == "test"
 Requires-Dist: mypy~=1.10; extra == "test"
-Requires-Dist: pytest-cov~=5.0; extra == "test"
-Requires-Dist: pyTooling~=6.1; extra == "test"
+Requires-Dist: typing_extensions~=4.12; extra == "test"
+Requires-Dist: pytest~=8.2; extra == "test"
 Requires-Dist: Coverage~=7.5; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
+Requires-Dist: lxml~=5.1; extra == "test"
 Provides-Extra: all
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
 Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: docutils~=0.18.1; extra == "all"
-Requires-Dist: lxml~=5.1; extra == "all"
-Requires-Dist: typing_extensions~=4.11; extra == "all"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
+Requires-Dist: setuptools~=70.0; extra == "all"
 Requires-Dist: mypy~=1.10; extra == "all"
+Requires-Dist: docutils~=0.18.1; extra == "all"
 Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
 Requires-Dist: pytest-cov~=5.0; extra == "all"
-Requires-Dist: pytest~=8.2; extra == "all"
 Requires-Dist: sphinx_reports~=0.6; extra == "all"
-Requires-Dist: sphinx_design>=0.5.0; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
-Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
+Requires-Dist: typing_extensions~=4.12; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: sphinx_design>=0.5.0; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyedaa_reports-0.8.0/pyEDAA.Reports.egg-info/requires.txt` & `pyedaa_reports-0.9.0/pyEDAA.Reports.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-ruamel.yaml~=0.18.6
 pyTooling~=6.1
+ruamel.yaml~=0.18.6
 lxml~=5.1
 
 [all]
 ruamel.yaml~=0.18.6
-sphinx_rtd_theme~=2.0.0
-pyTooling~=6.1
-sphinxcontrib-mermaid>=0.9.2
-autoapi>=2.0.1
-Coverage~=7.5
+pytest~=8.2
+sphinx~=7.3
 colorama>=0.4.6
-docutils~=0.18.1
-lxml~=5.1
-typing_extensions~=4.11
+sphinx_rtd_theme~=2.0.0
+setuptools~=70.0
 mypy~=1.10
+docutils~=0.18.1
 sphinx_autodoc_typehints~=2.1
 pytest-cov~=5.0
-pytest~=8.2
 sphinx_reports~=0.6
-sphinx_design>=0.5.0
-setuptools~=69.5
-sphinx~=7.3
+pyTooling~=6.1
+typing_extensions~=4.12
+sphinxcontrib-mermaid>=0.9.2
 sphinx-copybutton>=0.5.2
+lxml~=5.1
+autoapi>=2.0.1
+sphinx_design>=0.5.0
+Coverage~=7.5
 
 [doc]
+pyTooling~=6.1
 ruamel.yaml~=0.18.6
-colorama>=0.4.6
 docutils~=0.18.1
 autoapi>=2.0.1
-lxml~=5.1
-sphinx_reports~=0.6
 sphinx_design>=0.5.0
-sphinx_rtd_theme~=2.0.0
-setuptools~=69.5
-sphinx_autodoc_typehints~=2.1
-pyTooling~=6.1
 sphinx~=7.3
-sphinx-copybutton>=0.5.2
+sphinx_autodoc_typehints~=2.1
+colorama>=0.4.6
+sphinx_rtd_theme~=2.0.0
 sphinxcontrib-mermaid>=0.9.2
+sphinx-copybutton>=0.5.2
+lxml~=5.1
+setuptools~=70.0
+sphinx_reports~=0.6
 
 [test]
+pyTooling~=6.1
 ruamel.yaml~=0.18.6
-lxml~=5.1
-pytest~=8.2
-typing_extensions~=4.11
 mypy~=1.10
-pytest-cov~=5.0
-pyTooling~=6.1
+typing_extensions~=4.12
+pytest~=8.2
 Coverage~=7.5
+pytest-cov~=5.0
+lxml~=5.1
```

### Comparing `pyedaa_reports-0.8.0/pyproject.toml` & `pyedaa_reports-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.8.0/setup.py` & `pyedaa_reports-0.9.0/setup.py`

 * *Files identical despite different names*

