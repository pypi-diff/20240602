# Comparing `tmp/sc3dg-0.0.8.tar.gz` & `tmp/sc3dg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc3dg-0.0.8.tar", last modified: Sun Jun  2 12:43:51 2024, max compression
+gzip compressed data, was "sc3dg-0.0.9.tar", last modified: Sun Jun  2 12:46:38 2024, max compression
```

## Comparing `sc3dg-0.0.8.tar` & `sc3dg-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-02 12:43:51.000000 sc3dg-0.0.8/PKG-INFO
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.8/README.md
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.8/sc3dg/__init__.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg/anlysis/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    50821 2024-06-02 11:59:02.000000 sc3dg-0.0.8/sc3dg/anlysis/api.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5871 2024-06-02 10:58:47.000000 sc3dg-0.0.8/sc3dg/anlysis/embedding.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     4317 2024-06-02 10:58:46.000000 sc3dg-0.0.8/sc3dg/anlysis/genome.py
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      448 2024-06-02 12:39:48.000000 sc3dg-0.0.8/sc3dg/cli.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg/commands/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5372 2024-06-02 12:25:23.000000 sc3dg-0.0.8/sc3dg/commands/count.py
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)     7311 2024-06-02 12:39:30.000000 sc3dg-0.0.8/sc3dg/commands/impute.py
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)     3150 2024-06-02 12:37:19.000000 sc3dg-0.0.8/sc3dg/commands/model.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg/model/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)    32049 2024-06-02 11:23:14.000000 sc3dg-0.0.8/sc3dg/model/STARK_dyn_3dg.py
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)    23232 2024-06-02 12:36:53.000000 sc3dg-0.0.8/sc3dg/model/STARK_nuc_dynamics.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg/utils/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2024-06-01 10:18:22.000000 sc3dg-0.0.8/sc3dg/utils/Generate_scNanoHIC_pairs.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2024-06-01 10:18:22.000000 sc3dg-0.0.8/sc3dg/utils/ReformSAM.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      131 2024-06-01 10:21:06.000000 sc3dg-0.0.8/sc3dg/utils/__init__.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/analysis.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7503 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/assembly.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2555 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/download.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/embedding.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/general.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/help.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/plot.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    15197 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/scMethyl.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7287 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/scNano.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/scNano_barcode.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    13736 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/scSPRITE.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25080 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/scaffold.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/sciHic.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12315 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/sn_m3c.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5223 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/tools.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/visualize.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg.egg-info/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-02 12:43:49.000000 sc3dg-0.0.8/sc3dg.egg-info/PKG-INFO
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      896 2024-06-02 12:43:50.000000 sc3dg-0.0.8/sc3dg.egg-info/SOURCES.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-02 12:43:49.000000 sc3dg-0.0.8/sc3dg.egg-info/dependency_links.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       40 2024-06-02 12:43:49.000000 sc3dg-0.0.8/sc3dg.egg-info/entry_points.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      595 2024-06-02 12:43:49.000000 sc3dg-0.0.8/sc3dg.egg-info/requires.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-02 12:43:49.000000 sc3dg-0.0.8/sc3dg.egg-info/top_level.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-02 12:43:51.000000 sc3dg-0.0.8/setup.cfg
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      488 2021-02-02 05:13:23.000000 sc3dg-0.0.8/setup.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:46:37.000000 sc3dg-0.0.9/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-02 12:46:37.000000 sc3dg-0.0.9/PKG-INFO
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.9/README.md
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:46:36.000000 sc3dg-0.0.9/sc3dg/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.9/sc3dg/__init__.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:46:36.000000 sc3dg-0.0.9/sc3dg/anlysis/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    50821 2024-06-02 11:59:02.000000 sc3dg-0.0.9/sc3dg/anlysis/api.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5871 2024-06-02 10:58:47.000000 sc3dg-0.0.9/sc3dg/anlysis/embedding.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     4317 2024-06-02 10:58:46.000000 sc3dg-0.0.9/sc3dg/anlysis/genome.py
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      448 2024-06-02 12:39:48.000000 sc3dg-0.0.9/sc3dg/cli.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:46:36.000000 sc3dg-0.0.9/sc3dg/commands/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5372 2024-06-02 12:25:23.000000 sc3dg-0.0.9/sc3dg/commands/count.py
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)     7311 2024-06-02 12:39:30.000000 sc3dg-0.0.9/sc3dg/commands/impute.py
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)     3125 2024-06-02 12:46:20.000000 sc3dg-0.0.9/sc3dg/commands/model.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:46:36.000000 sc3dg-0.0.9/sc3dg/model/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)    32049 2024-06-02 11:23:14.000000 sc3dg-0.0.9/sc3dg/model/STARK_dyn_3dg.py
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)    23232 2024-06-02 12:36:53.000000 sc3dg-0.0.9/sc3dg/model/STARK_nuc_dynamics.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:46:37.000000 sc3dg-0.0.9/sc3dg/utils/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2024-06-01 10:18:22.000000 sc3dg-0.0.9/sc3dg/utils/Generate_scNanoHIC_pairs.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2024-06-01 10:18:22.000000 sc3dg-0.0.9/sc3dg/utils/ReformSAM.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      131 2024-06-01 10:21:06.000000 sc3dg-0.0.9/sc3dg/utils/__init__.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/analysis.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7503 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/assembly.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2555 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/download.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/embedding.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/general.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/help.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/plot.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    15197 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/scMethyl.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7287 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/scNano.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/scNano_barcode.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    13736 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/scSPRITE.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25080 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/scaffold.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/sciHic.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12315 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/sn_m3c.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5223 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/tools.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2024-06-01 10:18:23.000000 sc3dg-0.0.9/sc3dg/utils/visualize.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:46:36.000000 sc3dg-0.0.9/sc3dg.egg-info/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-02 12:46:35.000000 sc3dg-0.0.9/sc3dg.egg-info/PKG-INFO
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      896 2024-06-02 12:46:36.000000 sc3dg-0.0.9/sc3dg.egg-info/SOURCES.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-02 12:46:35.000000 sc3dg-0.0.9/sc3dg.egg-info/dependency_links.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       40 2024-06-02 12:46:35.000000 sc3dg-0.0.9/sc3dg.egg-info/entry_points.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      595 2024-06-02 12:46:35.000000 sc3dg-0.0.9/sc3dg.egg-info/requires.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-02 12:46:35.000000 sc3dg-0.0.9/sc3dg.egg-info/top_level.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-02 12:46:37.000000 sc3dg-0.0.9/setup.cfg
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      488 2021-02-02 05:16:57.000000 sc3dg-0.0.9/setup.py
```

### Comparing `sc3dg-0.0.8/README.md` & `sc3dg-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/anlysis/api.py` & `sc3dg-0.0.9/sc3dg/anlysis/api.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/anlysis/embedding.py` & `sc3dg-0.0.9/sc3dg/anlysis/embedding.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/anlysis/genome.py` & `sc3dg-0.0.9/sc3dg/anlysis/genome.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/commands/count.py` & `sc3dg-0.0.9/sc3dg/commands/count.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/commands/impute.py` & `sc3dg-0.0.9/sc3dg/commands/impute.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/commands/model.py` & `sc3dg-0.0.9/sc3dg/commands/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from sc3dg.model.STARK_nuc_dynamics import calc_genome_structure
 from time import time
 import argparse
-def generate_3d( pair_file_path,
-                pdb_file_path
+def generate_3d( pair_file_path:str,
+                pdb_file_path:str,
                 num_models:int, 
-                iter_steps:int=10,
-                iter_res:list=[8e6, 4e6, 2e6, 4e5, 2e5, 1e5]):
+                iter_steps:int,
+                iter_res:list):
 
     # Number of alternative conformations to generate from repeat calculations
     # with different random starting coordinates
     num_models = num_models
 
     # Parameters to setup restraints and starting coords
     general_calc_params = {'dist_power_law': -0.33,
```

### Comparing `sc3dg-0.0.8/sc3dg/model/STARK_dyn_3dg.py` & `sc3dg-0.0.9/sc3dg/model/STARK_dyn_3dg.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/model/STARK_nuc_dynamics.py` & `sc3dg-0.0.9/sc3dg/model/STARK_nuc_dynamics.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/Generate_scNanoHIC_pairs.py` & `sc3dg-0.0.9/sc3dg/utils/Generate_scNanoHIC_pairs.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/ReformSAM.py` & `sc3dg-0.0.9/sc3dg/utils/ReformSAM.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/analysis.py` & `sc3dg-0.0.9/sc3dg/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/assembly.py` & `sc3dg-0.0.9/sc3dg/utils/assembly.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/download.py` & `sc3dg-0.0.9/sc3dg/utils/download.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/embedding.py` & `sc3dg-0.0.9/sc3dg/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/general.py` & `sc3dg-0.0.9/sc3dg/utils/general.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/help.py` & `sc3dg-0.0.9/sc3dg/utils/help.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/plot.py` & `sc3dg-0.0.9/sc3dg/utils/plot.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/scMethyl.py` & `sc3dg-0.0.9/sc3dg/utils/scMethyl.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/scNano.py` & `sc3dg-0.0.9/sc3dg/utils/scNano.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/scNano_barcode.py` & `sc3dg-0.0.9/sc3dg/utils/scNano_barcode.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/scSPRITE.py` & `sc3dg-0.0.9/sc3dg/utils/scSPRITE.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/scaffold.py` & `sc3dg-0.0.9/sc3dg/utils/scaffold.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/sciHic.py` & `sc3dg-0.0.9/sc3dg/utils/sciHic.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/sn_m3c.py` & `sc3dg-0.0.9/sc3dg/utils/sn_m3c.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/tools.py` & `sc3dg-0.0.9/sc3dg/utils/tools.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg/utils/visualize.py` & `sc3dg-0.0.9/sc3dg/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg.egg-info/SOURCES.txt` & `sc3dg-0.0.9/sc3dg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.8/sc3dg.egg-info/requires.txt` & `sc3dg-0.0.9/sc3dg.egg-info/requires.txt`

 * *Files identical despite different names*

