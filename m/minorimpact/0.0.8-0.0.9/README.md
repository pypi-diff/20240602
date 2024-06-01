# Comparing `tmp/minorimpact-0.0.8.tar.gz` & `tmp/minorimpact-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minorimpact-0.0.8.tar", last modified: Mon Sep 27 18:17:45 2021, max compression
+gzip compressed data, was "minorimpact-0.0.9.tar", last modified: Mon Sep 27 23:57:29 2021, max compression
```

## Comparing `minorimpact-0.0.8.tar` & `minorimpact-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pgillan    (501) staff       (20)        0 2021-09-27 18:17:45.555198 minorimpact-0.0.8/
--rw-r--r--   0 pgillan    (501) staff       (20)      254 2021-09-27 18:17:45.554948 minorimpact-0.0.8/PKG-INFO
--rw-r--r--   0 pgillan    (501) staff       (20)      133 2021-09-22 17:20:32.000000 minorimpact-0.0.8/README.md
-drwxr-xr-x   0 pgillan    (501) staff       (20)        0 2021-09-27 18:17:45.553152 minorimpact-0.0.8/minorimpact/
--rw-r--r--   0 pgillan    (501) staff       (20)     4868 2021-09-27 18:16:46.000000 minorimpact-0.0.8/minorimpact/__init__.py
--rw-r--r--   0 pgillan    (501) staff       (20)     1820 2021-09-24 19:34:39.000000 minorimpact-0.0.8/minorimpact/config.py
--rwxr-xr-x   0 pgillan    (501) staff       (20)     2193 2020-09-09 03:01:11.000000 minorimpact-0.0.8/minorimpact/curses.py
-drwxr-xr-x   0 pgillan    (501) staff       (20)        0 2021-09-27 18:17:45.554617 minorimpact-0.0.8/minorimpact.egg-info/
--rw-r--r--   0 pgillan    (501) staff       (20)      254 2021-09-27 18:17:45.000000 minorimpact-0.0.8/minorimpact.egg-info/PKG-INFO
--rw-r--r--   0 pgillan    (501) staff       (20)      260 2021-09-27 18:17:45.000000 minorimpact-0.0.8/minorimpact.egg-info/SOURCES.txt
--rw-r--r--   0 pgillan    (501) staff       (20)        1 2021-09-27 18:17:45.000000 minorimpact-0.0.8/minorimpact.egg-info/dependency_links.txt
--rw-r--r--   0 pgillan    (501) staff       (20)        7 2021-09-27 18:17:45.000000 minorimpact-0.0.8/minorimpact.egg-info/requires.txt
--rw-r--r--   0 pgillan    (501) staff       (20)       12 2021-09-27 18:17:45.000000 minorimpact-0.0.8/minorimpact.egg-info/top_level.txt
--rw-r--r--   0 pgillan    (501) staff       (20)       38 2021-09-27 18:17:45.555283 minorimpact-0.0.8/setup.cfg
--rwxr-xr-x   0 pgillan    (501) staff       (20)      492 2021-09-22 17:14:24.000000 minorimpact-0.0.8/setup.py
+drwxr-xr-x   0 pgillan    (501) staff       (20)        0 2021-09-27 23:57:29.338614 minorimpact-0.0.9/
+-rw-r--r--   0 pgillan    (501) staff       (20)      420 2021-09-27 23:57:29.338367 minorimpact-0.0.9/PKG-INFO
+-rw-r--r--   0 pgillan    (501) staff       (20)      133 2021-09-22 17:20:32.000000 minorimpact-0.0.9/README.md
+drwxr-xr-x   0 pgillan    (501) staff       (20)        0 2021-09-27 23:57:29.336243 minorimpact-0.0.9/minorimpact/
+-rw-r--r--   0 pgillan    (501) staff       (20)     5633 2021-09-27 23:57:04.000000 minorimpact-0.0.9/minorimpact/__init__.py
+-rw-r--r--   0 pgillan    (501) staff       (20)     1922 2021-09-27 21:00:54.000000 minorimpact-0.0.9/minorimpact/config.py
+-rwxr-xr-x   0 pgillan    (501) staff       (20)     2193 2020-09-09 03:01:11.000000 minorimpact-0.0.9/minorimpact/curses.py
+drwxr-xr-x   0 pgillan    (501) staff       (20)        0 2021-09-27 23:57:29.338052 minorimpact-0.0.9/minorimpact.egg-info/
+-rw-r--r--   0 pgillan    (501) staff       (20)      420 2021-09-27 23:57:29.000000 minorimpact-0.0.9/minorimpact.egg-info/PKG-INFO
+-rw-r--r--   0 pgillan    (501) staff       (20)      260 2021-09-27 23:57:29.000000 minorimpact-0.0.9/minorimpact.egg-info/SOURCES.txt
+-rw-r--r--   0 pgillan    (501) staff       (20)        1 2021-09-27 23:57:29.000000 minorimpact-0.0.9/minorimpact.egg-info/dependency_links.txt
+-rw-r--r--   0 pgillan    (501) staff       (20)        7 2021-09-27 23:57:29.000000 minorimpact-0.0.9/minorimpact.egg-info/requires.txt
+-rw-r--r--   0 pgillan    (501) staff       (20)       12 2021-09-27 23:57:29.000000 minorimpact-0.0.9/minorimpact.egg-info/top_level.txt
+-rw-r--r--   0 pgillan    (501) staff       (20)       38 2021-09-27 23:57:29.338709 minorimpact-0.0.9/setup.cfg
+-rwxr-xr-x   0 pgillan    (501) staff       (20)      648 2021-09-27 18:22:57.000000 minorimpact-0.0.9/setup.py
```

### Comparing `minorimpact-0.0.8/minorimpact/config.py` & `minorimpact-0.0.9/minorimpact/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import configparser
 import os
 import os.path
 import re
 import sys
 
 def getConfig(config = None, interpolation = None, script_name = None, verbose = False):
+    """Attempts to scan the environment for a configuration file and parse it with configparser."""
     home = os.environ['HOME'] if 'HOME' in os.environ else ''
     config_basename = None
     config_filename = None
 
     if script_name is None:
         script_name = re.sub('\.py$', '', os.path.basename(sys.argv[0])) 
 
@@ -24,15 +25,15 @@
         if (re.match('/', config)): 
             config_filename = config
             config_basename = os.path.basename(config_filename)
         else:
             config_basename = config
 
     if (config_filename is None):
-        for path in [home + '/.conf/' + script_name, home, '/etc']:
+        for path in [home + '/.config/' + script_name, home, '/etc']:
             if (verbose is True): print(f"checking {path}/ ... ", end='')
             test_filename = f'{path}/{config_basename}'
             if (os.path.exists(test_filename)):
                 if (verbose is True): print("found")
                 config_filename = test_filename
                 break
             if (verbose is True): print("not found")
```

### Comparing `minorimpact-0.0.8/minorimpact/curses.py` & `minorimpact-0.0.9/minorimpact/curses.py`

 * *Files identical despite different names*

