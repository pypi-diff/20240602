# Comparing `tmp/rl_test_task_1-0.1.3.tar.gz` & `tmp/rl_test_task_1-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl_test_task_1-0.1.3.tar", last modified: Sun Jun  2 15:13:11 2024, max compression
+gzip compressed data, was "rl_test_task_1-0.1.4.tar", last modified: Sun Jun  2 15:34:03 2024, max compression
```

## Comparing `rl_test_task_1-0.1.3.tar` & `rl_test_task_1-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:11.820765 rl_test_task_1-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-02 15:13:11.820765 rl_test_task_1-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:11.812765 rl_test_task_1-0.1.3/rl_test_task_1/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:11.816765 rl_test_task_1-0.1.3/rl_test_task_1/data_exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_exporters/data_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:11.816765 rl_test_task_1-0.1.3/rl_test_task_1/data_exporters/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_exporters/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_exporters/exceptions/unsupported_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_exporters/generic_data_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_exporters/persons_data_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:11.816765 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/inputs_data_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:11.816765 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/models/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/models/input.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/models/person.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:11.820765 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/parsers/input_data_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/parsers/output_data_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/rl_test_task_1/data_providers/persons_data_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:13:11.820765 rl_test_task_1-0.1.3/rl_test_task_1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-02 15:13:11.000000 rl_test_task_1-0.1.3/rl_test_task_1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-06-02 15:13:11.000000 rl_test_task_1-0.1.3/rl_test_task_1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:13:11.000000 rl_test_task_1-0.1.3/rl_test_task_1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-02 15:13:11.000000 rl_test_task_1-0.1.3/rl_test_task_1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 15:13:11.000000 rl_test_task_1-0.1.3/rl_test_task_1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:13:11.820765 rl_test_task_1-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-06-02 15:13:02.000000 rl_test_task_1-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:03.394392 rl_test_task_1-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-02 15:34:03.394392 rl_test_task_1-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:03.390392 rl_test_task_1-0.1.4/rl_test_task_1/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:03.394392 rl_test_task_1-0.1.4/rl_test_task_1/data_exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_exporters/data_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:03.394392 rl_test_task_1-0.1.4/rl_test_task_1/data_exporters/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_exporters/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_exporters/exceptions/unsupported_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_exporters/generic_data_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_exporters/persons_data_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:03.394392 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/inputs_data_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:03.394392 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/models/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/models/person.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:03.394392 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/parsers/input_data_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/parsers/output_data_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/rl_test_task_1/data_providers/persons_data_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:34:03.394392 rl_test_task_1-0.1.4/rl_test_task_1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-02 15:34:03.000000 rl_test_task_1-0.1.4/rl_test_task_1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-06-02 15:34:03.000000 rl_test_task_1-0.1.4/rl_test_task_1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:34:03.000000 rl_test_task_1-0.1.4/rl_test_task_1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-02 15:34:03.000000 rl_test_task_1-0.1.4/rl_test_task_1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 15:34:03.000000 rl_test_task_1-0.1.4/rl_test_task_1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 15:34:03.394392 rl_test_task_1-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-06-02 15:33:53.000000 rl_test_task_1-0.1.4/setup.py
```

### Comparing `rl_test_task_1-0.1.3/rl_test_task_1/client.py` & `rl_test_task_1-0.1.4/rl_test_task_1/client.py`

 * *Files identical despite different names*

### Comparing `rl_test_task_1-0.1.3/rl_test_task_1/data_exporters/data_exporter.py` & `rl_test_task_1-0.1.4/rl_test_task_1/data_exporters/data_exporter.py`

 * *Files identical despite different names*

### Comparing `rl_test_task_1-0.1.3/rl_test_task_1/data_exporters/generic_data_exporter.py` & `rl_test_task_1-0.1.4/rl_test_task_1/data_exporters/generic_data_exporter.py`

 * *Files identical despite different names*

### Comparing `rl_test_task_1-0.1.3/rl_test_task_1/data_exporters/persons_data_exporter.py` & `rl_test_task_1-0.1.4/rl_test_task_1/data_exporters/persons_data_exporter.py`

 * *Files identical despite different names*

### Comparing `rl_test_task_1-0.1.3/rl_test_task_1/data_providers/inputs_data_provider.py` & `rl_test_task_1-0.1.4/rl_test_task_1/data_providers/inputs_data_provider.py`

 * *Files identical despite different names*

### Comparing `rl_test_task_1-0.1.3/rl_test_task_1/data_providers/parsers/input_data_parser.py` & `rl_test_task_1-0.1.4/rl_test_task_1/data_providers/parsers/input_data_parser.py`

 * *Files identical despite different names*

### Comparing `rl_test_task_1-0.1.3/rl_test_task_1/data_providers/persons_data_provider.py` & `rl_test_task_1-0.1.4/rl_test_task_1/data_providers/persons_data_provider.py`

 * *Files identical despite different names*

### Comparing `rl_test_task_1-0.1.3/rl_test_task_1.egg-info/SOURCES.txt` & `rl_test_task_1-0.1.4/rl_test_task_1.egg-info/SOURCES.txt`

 * *Files identical despite different names*
