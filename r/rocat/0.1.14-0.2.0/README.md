# Comparing `tmp/rocat-0.1.14.tar.gz` & `tmp/rocat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocat-0.1.14.tar", last modified: Fri Apr  5 05:06:35 2024, max compression
+gzip compressed data, was "rocat-0.2.0.tar", last modified: Sat Jun  1 23:35:27 2024, max compression
```

## Comparing `rocat-0.1.14.tar` & `rocat-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 05:06:35.809868 rocat-0.1.14/
--rw-rw-rw-   0        0        0     1081 2024-04-05 05:02:16.000000 rocat-0.1.14/LICENSE
--rw-rw-rw-   0        0        0       28 2024-04-05 05:02:16.000000 rocat-0.1.14/MANIFEST.in
--rw-rw-rw-   0        0        0     2170 2024-04-05 05:06:35.808866 rocat-0.1.14/PKG-INFO
--rw-rw-rw-   0        0        0     1789 2024-04-05 05:02:16.000000 rocat-0.1.14/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 05:06:35.789867 rocat-0.1.14/rocat/
--rw-rw-rw-   0        0        0      146 2024-04-05 05:02:16.000000 rocat-0.1.14/rocat/__init__.py
--rw-rw-rw-   0        0        0     2479 2024-04-05 05:02:16.000000 rocat-0.1.14/rocat/chatbot_modules.py
-drwxrwxrwx   0        0        0        0 2024-04-05 05:06:35.807867 rocat-0.1.14/rocat.egg-info/
--rw-rw-rw-   0        0        0     2170 2024-04-05 05:06:35.000000 rocat-0.1.14/rocat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-04-05 05:06:35.000000 rocat-0.1.14/rocat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 05:06:35.000000 rocat-0.1.14/rocat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-05 05:06:35.000000 rocat-0.1.14/rocat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-05 05:06:35.000000 rocat-0.1.14/rocat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 05:06:35.809868 rocat-0.1.14/setup.cfg
--rw-rw-rw-   0        0        0      722 2024-04-05 05:04:36.000000 rocat-0.1.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:35:27.349848 rocat-0.2.0/
+-rw-rw-rw-   0        0        0     1081 2024-05-28 06:15:40.000000 rocat-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4581 2024-06-01 23:35:27.348851 rocat-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3551 2024-05-28 08:33:31.000000 rocat-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 23:35:27.338883 rocat-0.2.0/rocat/
+-rw-rw-rw-   0        0        0      869 2024-05-28 08:57:15.000000 rocat-0.2.0/rocat/__init__.py
+-rw-rw-rw-   0        0        0     1162 2024-05-28 08:32:13.000000 rocat-0.2.0/rocat/__main__.py
+-rw-rw-rw-   0        0        0     2623 2024-05-28 08:58:20.000000 rocat-0.2.0/rocat/ai_functions.py
+-rw-rw-rw-   0        0        0     2116 2024-05-28 08:58:23.000000 rocat-0.2.0/rocat/config.py
+-rw-rw-rw-   0        0        0    12217 2024-05-28 08:58:41.000000 rocat-0.2.0/rocat/file_utils.py
+-rw-rw-rw-   0        0        0     7451 2024-05-28 08:54:53.000000 rocat-0.2.0/rocat/language_model.py
+-rw-rw-rw-   0        0        0      838 2024-05-28 08:56:06.000000 rocat-0.2.0/rocat/language_utils.py
+-rw-rw-rw-   0        0        0      480 2024-05-28 08:56:10.000000 rocat-0.2.0/rocat/main.py
+-rw-rw-rw-   0        0        0      807 2024-05-28 08:56:11.000000 rocat-0.2.0/rocat/template_utils.py
+-rw-rw-rw-   0        0        0     2215 2024-05-28 08:58:58.000000 rocat-0.2.0/rocat/web_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:35:27.347854 rocat-0.2.0/rocat.egg-info/
+-rw-rw-rw-   0        0        0     4581 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      303 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-01 23:35:27.000000 rocat-0.2.0/rocat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 23:35:27.349848 rocat-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1462 2024-06-01 23:34:42.000000 rocat-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:35:27.347854 rocat-0.2.0/tests/
+-rw-rw-rw-   0        0        0     2055 2024-05-28 06:15:40.000000 rocat-0.2.0/tests/test.py
+-rw-rw-rw-   0        0        0     3341 2024-05-28 09:06:39.000000 rocat-0.2.0/tests/test_file_utils.py
+-rw-rw-rw-   0        0        0     1137 2024-05-28 09:03:24.000000 rocat-0.2.0/tests/test_web_utils.py
```

### Comparing `rocat-0.1.14/LICENSE` & `rocat-0.2.0/LICENSE`

 * *Files identical despite different names*

