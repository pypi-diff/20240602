# Comparing `tmp/sc3dg-0.0.7.tar.gz` & `tmp/sc3dg-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc3dg-0.0.7.tar", last modified: Sat Jun  1 10:25:57 2024, max compression
+gzip compressed data, was "sc3dg-0.0.8.tar", last modified: Sun Jun  2 12:43:51 2024, max compression
```

## Comparing `sc3dg-0.0.7.tar` & `sc3dg-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,46 @@
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:25:57.000000 sc3dg-0.0.7/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:25:57.000000 sc3dg-0.0.7/PKG-INFO
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.7/README.md
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:25:57.000000 sc3dg-0.0.7/sc3dg/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.7/sc3dg/__init__.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5510 2024-06-01 10:01:05.000000 sc3dg-0.0.7/sc3dg/main.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:25:57.000000 sc3dg-0.0.7/sc3dg/utils/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2024-06-01 10:18:22.000000 sc3dg-0.0.7/sc3dg/utils/Generate_scNanoHIC_pairs.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2024-06-01 10:18:22.000000 sc3dg-0.0.7/sc3dg/utils/ReformSAM.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      131 2024-06-01 10:21:06.000000 sc3dg-0.0.7/sc3dg/utils/__init__.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/analysis.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7503 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/assembly.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2555 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/download.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/embedding.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/general.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/help.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/plot.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    15197 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/scMethyl.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7287 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/scNano.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/scNano_barcode.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    13736 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/scSPRITE.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25080 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/scaffold.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/sciHic.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12315 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/sn_m3c.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5223 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/tools.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2024-06-01 10:18:23.000000 sc3dg-0.0.7/sc3dg/utils/visualize.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:25:57.000000 sc3dg-0.0.7/sc3dg.egg-info/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:25:56.000000 sc3dg-0.0.7/sc3dg.egg-info/PKG-INFO
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      689 2024-06-01 10:25:56.000000 sc3dg-0.0.7/sc3dg.egg-info/SOURCES.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-01 10:25:56.000000 sc3dg-0.0.7/sc3dg.egg-info/dependency_links.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       42 2024-06-01 10:25:56.000000 sc3dg-0.0.7/sc3dg.egg-info/entry_points.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      589 2024-06-01 10:25:56.000000 sc3dg-0.0.7/sc3dg.egg-info/requires.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-01 10:25:56.000000 sc3dg-0.0.7/sc3dg.egg-info/top_level.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-01 10:25:57.000000 sc3dg-0.0.7/setup.cfg
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      435 2021-02-01 02:56:12.000000 sc3dg-0.0.7/setup.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-02 12:43:51.000000 sc3dg-0.0.8/PKG-INFO
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.8/README.md
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.8/sc3dg/__init__.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg/anlysis/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    50821 2024-06-02 11:59:02.000000 sc3dg-0.0.8/sc3dg/anlysis/api.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5871 2024-06-02 10:58:47.000000 sc3dg-0.0.8/sc3dg/anlysis/embedding.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     4317 2024-06-02 10:58:46.000000 sc3dg-0.0.8/sc3dg/anlysis/genome.py
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      448 2024-06-02 12:39:48.000000 sc3dg-0.0.8/sc3dg/cli.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg/commands/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5372 2024-06-02 12:25:23.000000 sc3dg-0.0.8/sc3dg/commands/count.py
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)     7311 2024-06-02 12:39:30.000000 sc3dg-0.0.8/sc3dg/commands/impute.py
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)     3150 2024-06-02 12:37:19.000000 sc3dg-0.0.8/sc3dg/commands/model.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg/model/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)    32049 2024-06-02 11:23:14.000000 sc3dg-0.0.8/sc3dg/model/STARK_dyn_3dg.py
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)    23232 2024-06-02 12:36:53.000000 sc3dg-0.0.8/sc3dg/model/STARK_nuc_dynamics.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg/utils/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2024-06-01 10:18:22.000000 sc3dg-0.0.8/sc3dg/utils/Generate_scNanoHIC_pairs.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2024-06-01 10:18:22.000000 sc3dg-0.0.8/sc3dg/utils/ReformSAM.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      131 2024-06-01 10:21:06.000000 sc3dg-0.0.8/sc3dg/utils/__init__.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/analysis.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7503 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/assembly.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2555 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/download.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/embedding.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/general.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/help.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/plot.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    15197 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/scMethyl.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7287 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/scNano.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/scNano_barcode.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    13736 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/scSPRITE.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25080 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/scaffold.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/sciHic.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12315 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/sn_m3c.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5223 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/tools.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2024-06-01 10:18:23.000000 sc3dg-0.0.8/sc3dg/utils/visualize.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-02 12:43:51.000000 sc3dg-0.0.8/sc3dg.egg-info/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-02 12:43:49.000000 sc3dg-0.0.8/sc3dg.egg-info/PKG-INFO
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      896 2024-06-02 12:43:50.000000 sc3dg-0.0.8/sc3dg.egg-info/SOURCES.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-02 12:43:49.000000 sc3dg-0.0.8/sc3dg.egg-info/dependency_links.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       40 2024-06-02 12:43:49.000000 sc3dg-0.0.8/sc3dg.egg-info/entry_points.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      595 2024-06-02 12:43:49.000000 sc3dg-0.0.8/sc3dg.egg-info/requires.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-02 12:43:49.000000 sc3dg-0.0.8/sc3dg.egg-info/top_level.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-02 12:43:51.000000 sc3dg-0.0.8/setup.cfg
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      488 2021-02-02 05:13:23.000000 sc3dg-0.0.8/setup.py
```

### Comparing `sc3dg-0.0.7/README.md` & `sc3dg-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/main.py` & `sc3dg-0.0.8/sc3dg/commands/count.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,17 +95,18 @@
     
 
 
 
 
 
 
-def main():
-    parser = argparse.ArgumentParser()
+def count():
+
 
+    parser = argparse.ArgumentParser()
     parser.add_argument('-o', '--output', help='save path',required=True,
                         default=None)
     parser.add_argument('-f', '--fastq', required=True,
                         default=None, 
                         help='fastq_dir, run all if -s is not be specfied',)
     parser.add_argument('--logging', help='logging', default='./log.log')
     parser.add_argument('-t', '--type',required=True,
@@ -132,11 +133,7 @@
                         help='scNano barcode for PCR and TN5, which should be stored in a folder and named as TN5.txt and PRC,index.txt.txt respectively')
     parser.add_argument('--zoomify-res', help='zoomify',type=str, default='10000,40000,100000,500000,1000000')
     
     args = parser.parse_args()
     run_pipeline(args)
 
 
-if __name__ == '__main__':
-    Time = time.time()
-    main()
-    print('=============time spen ', time.time() - Time, '===================')
```

### Comparing `sc3dg-0.0.7/sc3dg/utils/Generate_scNanoHIC_pairs.py` & `sc3dg-0.0.8/sc3dg/utils/Generate_scNanoHIC_pairs.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/ReformSAM.py` & `sc3dg-0.0.8/sc3dg/utils/ReformSAM.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/analysis.py` & `sc3dg-0.0.8/sc3dg/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/assembly.py` & `sc3dg-0.0.8/sc3dg/utils/assembly.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/download.py` & `sc3dg-0.0.8/sc3dg/utils/download.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/embedding.py` & `sc3dg-0.0.8/sc3dg/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/general.py` & `sc3dg-0.0.8/sc3dg/utils/general.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/help.py` & `sc3dg-0.0.8/sc3dg/utils/help.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/plot.py` & `sc3dg-0.0.8/sc3dg/utils/plot.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/scMethyl.py` & `sc3dg-0.0.8/sc3dg/utils/scMethyl.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/scNano.py` & `sc3dg-0.0.8/sc3dg/utils/scNano.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/scNano_barcode.py` & `sc3dg-0.0.8/sc3dg/utils/scNano_barcode.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/scSPRITE.py` & `sc3dg-0.0.8/sc3dg/utils/scSPRITE.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/scaffold.py` & `sc3dg-0.0.8/sc3dg/utils/scaffold.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/sciHic.py` & `sc3dg-0.0.8/sc3dg/utils/sciHic.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/sn_m3c.py` & `sc3dg-0.0.8/sc3dg/utils/sn_m3c.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/tools.py` & `sc3dg-0.0.8/sc3dg/utils/tools.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg/utils/visualize.py` & `sc3dg-0.0.8/sc3dg/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.7/sc3dg.egg-info/SOURCES.txt` & `sc3dg-0.0.8/sc3dg.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 README.md
 setup.py
 sc3dg/__init__.py
-sc3dg/main.py
+sc3dg/cli.py
 sc3dg.egg-info/PKG-INFO
 sc3dg.egg-info/SOURCES.txt
 sc3dg.egg-info/dependency_links.txt
 sc3dg.egg-info/entry_points.txt
 sc3dg.egg-info/requires.txt
 sc3dg.egg-info/top_level.txt
+sc3dg/anlysis/api.py
+sc3dg/anlysis/embedding.py
+sc3dg/anlysis/genome.py
+sc3dg/commands/count.py
+sc3dg/commands/impute.py
+sc3dg/commands/model.py
+sc3dg/model/STARK_dyn_3dg.py
+sc3dg/model/STARK_nuc_dynamics.py
 sc3dg/utils/Generate_scNanoHIC_pairs.py
 sc3dg/utils/ReformSAM.py
 sc3dg/utils/__init__.py
 sc3dg/utils/analysis.py
 sc3dg/utils/assembly.py
 sc3dg/utils/download.py
 sc3dg/utils/embedding.py
```

### Comparing `sc3dg-0.0.7/sc3dg.egg-info/requires.txt` & `sc3dg-0.0.8/sc3dg.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 numpy
+click
 pandas<2,>=1.5.1
 cython
 cmake
 pysam
 pairtools>=0.3.3
 biopython>=1.81
 anndata>=0.9.2
```

