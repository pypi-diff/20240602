# Comparing `tmp/wfmplan-0.2.0.tar.gz` & `tmp/wfmplan-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wfmplan-0.2.0.tar", last modified: Fri Mar 29 21:36:56 2024, max compression
+gzip compressed data, was "wfmplan-0.2.2.tar", last modified: Sun Jun  2 16:15:58 2024, max compression
```

## Comparing `wfmplan-0.2.0.tar` & `wfmplan-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 21:36:56.380000 wfmplan-0.2.0/
--rw-rw-rw-   0        0        0     1069 2024-03-29 21:18:14.000000 wfmplan-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       86 2024-03-29 21:18:00.000000 wfmplan-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      313 2024-03-29 21:36:58.000000 wfmplan-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-29 21:36:56.410000 wfmplan-0.2.0/WFMPlan/
--rw-rw-rw-   0        0        0     3679 2024-03-29 21:20:10.000000 wfmplan-0.2.0/WFMPlan/ErlangC.py
--rw-rw-rw-   0        0        0       28 2024-03-29 21:20:30.000000 wfmplan-0.2.0/WFMPlan/__init__.py
--rw-rw-rw-   0        0        0       97 2024-03-29 04:19:30.000000 wfmplan-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 21:36:58.000000 wfmplan-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      428 2024-03-29 21:35:58.000000 wfmplan-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-29 21:36:56.450000 wfmplan-0.2.0/wfmplan.egg-info/
--rw-rw-rw-   0        0        0      313 2024-03-29 21:36:58.000000 wfmplan-0.2.0/wfmplan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-03-29 21:36:58.000000 wfmplan-0.2.0/wfmplan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 21:36:58.000000 wfmplan-0.2.0/wfmplan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-29 21:36:58.000000 wfmplan-0.2.0/wfmplan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-29 21:36:58.000000 wfmplan-0.2.0/wfmplan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:15:58.956600 wfmplan-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-06-02 16:15:48.000000 wfmplan-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-06-02 16:15:58.956600 wfmplan-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-06-02 16:15:48.000000 wfmplan-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:15:58.956600 wfmplan-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-06-02 16:15:48.000000 wfmplan-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:15:58.952600 wfmplan-0.2.2/wfmplan/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:15:58.952600 wfmplan-0.2.2/wfmplan/AgentOptimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-06-02 16:15:48.000000 wfmplan-0.2.2/wfmplan/AgentOptimizer/BatchOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-06-02 16:15:48.000000 wfmplan-0.2.2/wfmplan/AgentOptimizer/Optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-02 16:15:48.000000 wfmplan-0.2.2/wfmplan/AgentOptimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-02 16:15:48.000000 wfmplan-0.2.2/wfmplan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:15:58.956600 wfmplan-0.2.2/wfmplan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 16:15:58.000000 wfmplan-0.2.2/wfmplan.egg-info/top_level.txt
```

### Comparing `wfmplan-0.2.0/LICENSE.txt` & `wfmplan-0.2.2/LICENSE.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-Copyright 2024 Rishi Laddha
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
+MIT License
+
+Copyright (c) 2024 Rishi Laddha
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

