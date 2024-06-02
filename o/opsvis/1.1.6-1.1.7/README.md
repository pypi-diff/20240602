# Comparing `tmp/opsvis-1.1.6.tar.gz` & `tmp/opsvis-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsvis-1.1.6.tar", last modified: Sun Jun  2 19:51:14 2024, max compression
+gzip compressed data, was "opsvis-1.1.7.tar", last modified: Sun Jun  2 20:14:59 2024, max compression
```

## Comparing `opsvis-1.1.6.tar` & `opsvis-1.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-06-02 19:51:14.195102 opsvis-1.1.6/
--rw-r--r--   0 sewi      (1000) sewi      (1000)    35149 2020-08-24 10:31:43.000000 opsvis-1.1.6/LICENSE
--rw-r--r--   0 sewi      (1000) sewi      (1000)     1068 2024-06-02 19:51:14.195102 opsvis-1.1.6/PKG-INFO
--rw-r--r--   0 sewi      (1000) sewi      (1000)      477 2021-09-28 08:54:43.000000 opsvis-1.1.6/README.md
-drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-06-02 19:51:14.195102 opsvis-1.1.6/opsvis/
--rw-r--r--   0 sewi      (1000) sewi      (1000)      154 2023-05-13 19:50:46.000000 opsvis-1.1.6/opsvis/__init__.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    20912 2023-05-14 06:27:30.000000 opsvis-1.1.6/opsvis/anim.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    47702 2023-11-10 08:58:20.000000 opsvis-1.1.6/opsvis/defo.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)     9113 2024-01-29 07:45:07.000000 opsvis-1.1.6/opsvis/fibsec.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)      195 2023-05-13 20:08:21.000000 opsvis-1.1.6/opsvis/importing_modules.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    92246 2024-06-02 19:48:12.000000 opsvis-1.1.6/opsvis/model.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    29911 2024-03-12 09:55:55.000000 opsvis-1.1.6/opsvis/secforces.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)     4621 2023-11-10 08:58:20.000000 opsvis-1.1.6/opsvis/settings.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    34781 2023-05-13 20:08:22.000000 opsvis-1.1.6/opsvis/stress.py
-drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-06-02 19:51:14.195102 opsvis-1.1.6/opsvis.egg-info/
--rw-r--r--   0 sewi      (1000) sewi      (1000)     1068 2024-06-02 19:51:14.000000 opsvis-1.1.6/opsvis.egg-info/PKG-INFO
--rw-r--r--   0 sewi      (1000) sewi      (1000)      357 2024-06-02 19:51:14.000000 opsvis-1.1.6/opsvis.egg-info/SOURCES.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)        1 2024-06-02 19:51:14.000000 opsvis-1.1.6/opsvis.egg-info/dependency_links.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)       11 2024-06-02 19:51:14.000000 opsvis-1.1.6/opsvis.egg-info/requires.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)        7 2024-06-02 19:51:14.000000 opsvis-1.1.6/opsvis.egg-info/top_level.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)      104 2021-09-23 09:12:02.000000 opsvis-1.1.6/pyproject.toml
--rw-r--r--   0 sewi      (1000) sewi      (1000)      704 2024-06-02 19:51:14.195102 opsvis-1.1.6/setup.cfg
+drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-06-02 20:14:59.007042 opsvis-1.1.7/
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    35149 2020-08-24 10:31:43.000000 opsvis-1.1.7/LICENSE
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     1068 2024-06-02 20:14:59.007042 opsvis-1.1.7/PKG-INFO
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      477 2021-09-28 08:54:43.000000 opsvis-1.1.7/README.md
+drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-06-02 20:14:59.007042 opsvis-1.1.7/opsvis/
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      154 2023-05-13 19:50:46.000000 opsvis-1.1.7/opsvis/__init__.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    20912 2023-05-14 06:27:30.000000 opsvis-1.1.7/opsvis/anim.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    47702 2023-11-10 08:58:20.000000 opsvis-1.1.7/opsvis/defo.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     9113 2024-01-29 07:45:07.000000 opsvis-1.1.7/opsvis/fibsec.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      195 2023-05-13 20:08:21.000000 opsvis-1.1.7/opsvis/importing_modules.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    92103 2024-06-02 20:13:58.000000 opsvis-1.1.7/opsvis/model.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    29911 2024-03-12 09:55:55.000000 opsvis-1.1.7/opsvis/secforces.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     4621 2023-11-10 08:58:20.000000 opsvis-1.1.7/opsvis/settings.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    34781 2023-05-13 20:08:22.000000 opsvis-1.1.7/opsvis/stress.py
+drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-06-02 20:14:59.007042 opsvis-1.1.7/opsvis.egg-info/
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     1068 2024-06-02 20:14:58.000000 opsvis-1.1.7/opsvis.egg-info/PKG-INFO
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      357 2024-06-02 20:14:59.000000 opsvis-1.1.7/opsvis.egg-info/SOURCES.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)        1 2024-06-02 20:14:58.000000 opsvis-1.1.7/opsvis.egg-info/dependency_links.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)       11 2024-06-02 20:14:58.000000 opsvis-1.1.7/opsvis.egg-info/requires.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)        7 2024-06-02 20:14:58.000000 opsvis-1.1.7/opsvis.egg-info/top_level.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      104 2021-09-23 09:12:02.000000 opsvis-1.1.7/pyproject.toml
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      704 2024-06-02 20:14:59.007042 opsvis-1.1.7/setup.cfg
```

### Comparing `opsvis-1.1.6/LICENSE` & `opsvis-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.6/PKG-INFO` & `opsvis-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsvis
-Version: 1.1.6
+Version: 1.1.7
 Summary: OpenSeesPy (OpenSees) Python postprocessing and visualization module
 Home-page: https://github.com/sewkokot/opsvis
 Author: Seweryn Kokot
 Author-email: sewkokot@gmail.com
 Project-URL: Bug Tracker, https://github.com/sewkokot/opsvis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `opsvis-1.1.6/opsvis/anim.py` & `opsvis-1.1.7/opsvis/anim.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.6/opsvis/defo.py` & `opsvis-1.1.7/opsvis/defo.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.6/opsvis/fibsec.py` & `opsvis-1.1.7/opsvis/fibsec.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.6/opsvis/model.py` & `opsvis-1.1.7/opsvis/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1269,17 +1269,16 @@
     """
 
     print('\nWarning! plot_supports_and_loads_2d has been removed.')  # noqa: E501
     print('\nWarning! Use plot_model(node_supports=True) for showing supports and')  # noqa: E501
     print('\nWarning! plot_loads_2d() for showing loads')  # noqa: E501
 
 
-def plot_loads_2d(nep=17, sfac=False, fig_wi_he=False,
-                  fig_lbrt=False, fmt_model_loads=fmt_model_loads,
-                  node_supports=True, truss_node_offset=0, ax=False):
+def plot_loads_2d(nep, sfac, fig_wi_he, fig_lbrt, fmt_model_loads,
+                  node_supports, truss_node_offset, ax):
     """Display the nodal and element loads applied to the 2d models.
 
     Args:
         nep (int): number of arrows when displacing element distributed loads
             (default: 17)
 
         node_supports (bool): True - show the node support conditions.
@@ -1598,17 +1597,16 @@
 
     ax.axis('equal')
     ax.grid(False)
 
     return ax
 
 
-def plot_loads_3d(nep=11, sfac=False, fig_wi_he=False,
-                  fig_lbrt=False, fmt_model_loads=fmt_model_loads,
-                  node_supports=True, truss_node_offset=0, ax=False):
+def plot_loads_3d(nep, sfac, fig_wi_he, fig_lbrt, fmt_model_loads,
+                  node_supports, local_axes, ax):
     """Display the nodal and element loads applied to the 2d models.
 
     Args:
         nep (int): number of arrows when displacing element distributed loads
             (default: 11)
 
         node_supports (bool): True - show the node support conditions.
```

### Comparing `opsvis-1.1.6/opsvis/secforces.py` & `opsvis-1.1.7/opsvis/secforces.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.6/opsvis/settings.py` & `opsvis-1.1.7/opsvis/settings.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.6/opsvis/stress.py` & `opsvis-1.1.7/opsvis/stress.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.6/opsvis.egg-info/PKG-INFO` & `opsvis-1.1.7/opsvis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsvis
-Version: 1.1.6
+Version: 1.1.7
 Summary: OpenSeesPy (OpenSees) Python postprocessing and visualization module
 Home-page: https://github.com/sewkokot/opsvis
 Author: Seweryn Kokot
 Author-email: sewkokot@gmail.com
 Project-URL: Bug Tracker, https://github.com/sewkokot/opsvis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `opsvis-1.1.6/setup.cfg` & `opsvis-1.1.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = opsvis
-version = 1.1.6
+version = 1.1.7
 author = Seweryn Kokot
 author_email = sewkokot@gmail.com
 description = OpenSeesPy (OpenSees) Python postprocessing and visualization module
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sewkokot/opsvis
 project_urls =
```

