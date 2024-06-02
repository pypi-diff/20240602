# Comparing `tmp/aliad-0.0.3.tar.gz` & `tmp/aliad-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliad-0.0.3.tar", last modified: Wed Dec  6 21:51:03 2023, max compression
+gzip compressed data, was "aliad-0.1.0.tar", last modified: Sun Jun  2 15:08:01 2024, max compression
```

## Comparing `aliad-0.0.3.tar` & `aliad-0.1.0.tar`

### file list

```diff
@@ -1,46 +1,56 @@
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.646912 aliad-0.0.3/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    11357 2023-10-08 21:02:33.000000 aliad-0.0.3/LICENSE
--rw-r--r--   0 chlcheng (102623) chlcheng (102623)      751 2023-12-06 21:51:03.646109 aliad-0.0.3/PKG-INFO
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       48 2023-10-08 21:02:33.000000 aliad-0.0.3/README.md
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.616671 aliad-0.0.3/aliad/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-10-08 21:03:03.000000 aliad-0.0.3/aliad/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       22 2023-12-06 05:20:22.000000 aliad-0.0.3/aliad/_version.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.624836 aliad-0.0.3/aliad/data/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       87 2023-11-07 11:16:55.000000 aliad-0.0.3/aliad/data/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    13046 2023-11-22 01:24:03.000000 aliad-0.0.3/aliad/data/partition.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    12856 2023-12-04 10:06:21.000000 aliad-0.0.3/aliad/data/point_cloud_dataset.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.626394 aliad-0.0.3/aliad/interface/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-10-19 19:08:21.000000 aliad-0.0.3/aliad/interface/__init__.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.629226 aliad-0.0.3/aliad/interface/awkward/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       61 2023-11-06 08:02:10.000000 aliad-0.0.3/aliad/interface/awkward/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3826 2023-11-07 00:03:17.000000 aliad-0.0.3/aliad/interface/awkward/momentum_4d_array_builder.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      142 2023-11-08 01:14:56.000000 aliad-0.0.3/aliad/interface/awkward/utils.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.631206 aliad-0.0.3/aliad/interface/fastjet/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       50 2023-11-06 08:01:40.000000 aliad-0.0.3/aliad/interface/fastjet/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3102 2023-11-06 09:47:36.000000 aliad-0.0.3/aliad/interface/fastjet/jet_clustering_tool.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.637708 aliad-0.0.3/aliad/interface/tensorflow/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-10-19 19:08:34.000000 aliad-0.0.3/aliad/interface/tensorflow/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     8027 2023-12-06 09:11:35.000000 aliad-0.0.3/aliad/interface/tensorflow/callbacks.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)    16046 2023-12-04 19:55:09.000000 aliad-0.0.3/aliad/interface/tensorflow/dataset.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     7241 2023-11-08 03:21:07.000000 aliad-0.0.3/aliad/interface/tensorflow/layers.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.639938 aliad-0.0.3/aliad/interface/tensorflow/modules/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      475 2023-11-08 03:19:42.000000 aliad-0.0.3/aliad/interface/tensorflow/modules/MLP.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-08 02:12:51.000000 aliad-0.0.3/aliad/interface/tensorflow/modules/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     6018 2023-10-25 01:31:28.000000 aliad-0.0.3/aliad/interface/tensorflow/operations.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1754 2023-11-08 03:22:02.000000 aliad-0.0.3/aliad/interface/tensorflow/utils.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.642527 aliad-0.0.3/aliad/utils/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-10-23 04:07:41.000000 aliad-0.0.3/aliad/utils/__init__.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-15 13:00:41.000000 aliad-0.0.3/aliad/utils/array_utils.py
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     3920 2023-10-23 05:44:37.000000 aliad-0.0.3/aliad/utils/system_utils.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.621132 aliad-0.0.3/aliad.egg-info/
--rw-r--r--   0 chlcheng (102623) chlcheng (102623)      751 2023-12-06 21:51:03.617641 aliad-0.0.3/aliad.egg-info/PKG-INFO
--rw-rw----   0 chlcheng (102623) chlcheng (102623)      960 2023-12-06 21:51:03.618630 aliad-0.0.3/aliad.egg-info/SOURCES.txt
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        1 2023-12-06 21:51:03.619809 aliad-0.0.3/aliad.egg-info/dependency_links.txt
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       41 2023-12-06 21:51:03.620430 aliad-0.0.3/aliad.egg-info/requires.txt
--rw-rw----   0 chlcheng (102623) chlcheng (102623)        6 2023-12-06 21:51:03.621593 aliad-0.0.3/aliad.egg-info/top_level.txt
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.644469 aliad-0.0.3/bin/
--rwxrwx---   0 chlcheng (102623) chlcheng (102623)       22 2023-10-08 21:33:14.000000 aliad-0.0.3/bin/aliad
--rw-rw----   0 chlcheng (102623) chlcheng (102623)       38 2023-12-06 21:51:03.647004 aliad-0.0.3/setup.cfg
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     1655 2023-11-09 19:30:41.000000 aliad-0.0.3/setup.py
-drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2023-12-06 21:51:03.645141 aliad-0.0.3/tests/
--rw-rw----   0 chlcheng (102623) chlcheng (102623)     2469 2023-10-23 02:41:06.000000 aliad-0.0.3/tests/test_data_preparation.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.903053 aliad-0.1.0/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    11357 2023-10-08 21:02:33.000000 aliad-0.1.0/LICENSE
+-rw-r--r--   0 chlcheng (102623) chlcheng (102623)      793 2024-06-02 15:08:01.902435 aliad-0.1.0/PKG-INFO
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       48 2023-10-08 21:02:33.000000 aliad-0.1.0/README.md
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.880213 aliad-0.1.0/aliad/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      109 2024-02-08 19:05:05.000000 aliad-0.1.0/aliad/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       22 2024-06-02 15:05:55.000000 aliad-0.1.0/aliad/_version.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.884245 aliad-0.1.0/aliad/components/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       37 2024-03-01 06:07:06.000000 aliad-0.1.0/aliad/components/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3353 2024-01-26 20:12:37.000000 aliad-0.1.0/aliad/components/evaluation.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1244 2024-03-05 07:36:17.000000 aliad-0.1.0/aliad/components/metrics.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     7524 2024-04-18 21:52:04.000000 aliad-0.1.0/aliad/components/model_output.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.885804 aliad-0.1.0/aliad/data/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       87 2023-11-07 11:16:55.000000 aliad-0.1.0/aliad/data/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    13550 2024-05-29 10:42:46.000000 aliad-0.1.0/aliad/data/partition.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    15126 2024-05-19 06:35:46.000000 aliad-0.1.0/aliad/data/point_cloud_dataset.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.886398 aliad-0.1.0/aliad/interface/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-10-19 19:08:21.000000 aliad-0.1.0/aliad/interface/__init__.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.888507 aliad-0.1.0/aliad/interface/awkward/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       61 2023-11-06 08:02:10.000000 aliad-0.1.0/aliad/interface/awkward/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3826 2023-11-07 00:03:17.000000 aliad-0.1.0/aliad/interface/awkward/momentum_4d_array_builder.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      142 2023-11-08 01:14:56.000000 aliad-0.1.0/aliad/interface/awkward/utils.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.889698 aliad-0.1.0/aliad/interface/fastjet/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       50 2023-11-06 08:01:40.000000 aliad-0.1.0/aliad/interface/fastjet/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3102 2023-11-06 09:47:36.000000 aliad-0.1.0/aliad/interface/fastjet/jet_clustering_tool.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.895398 aliad-0.1.0/aliad/interface/tensorflow/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       41 2024-05-30 05:57:46.000000 aliad-0.1.0/aliad/interface/tensorflow/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    20161 2024-05-27 08:18:31.000000 aliad-0.1.0/aliad/interface/tensorflow/callbacks.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    19951 2024-05-30 23:18:40.000000 aliad-0.1.0/aliad/interface/tensorflow/dataset.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     7340 2024-02-22 21:03:59.000000 aliad-0.1.0/aliad/interface/tensorflow/layers.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4038 2024-06-01 02:31:44.000000 aliad-0.1.0/aliad/interface/tensorflow/losses.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.897455 aliad-0.1.0/aliad/interface/tensorflow/models/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      475 2023-11-08 03:19:42.000000 aliad-0.1.0/aliad/interface/tensorflow/models/MLP.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4346 2024-02-29 09:27:48.000000 aliad-0.1.0/aliad/interface/tensorflow/models/MultiParticleNet.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       46 2024-02-08 02:44:35.000000 aliad-0.1.0/aliad/interface/tensorflow/models/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     6018 2023-10-25 01:31:28.000000 aliad-0.1.0/aliad/interface/tensorflow/operations.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      834 2024-04-24 22:14:47.000000 aliad-0.1.0/aliad/interface/tensorflow/regularizers.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3944 2024-05-30 23:14:23.000000 aliad-0.1.0/aliad/interface/tensorflow/tfrecord_maker.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1754 2023-11-08 03:22:02.000000 aliad-0.1.0/aliad/interface/tensorflow/utils.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.899085 aliad-0.1.0/aliad/utils/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-10-23 04:07:41.000000 aliad-0.1.0/aliad/utils/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-15 13:00:41.000000 aliad-0.1.0/aliad/utils/array_utils.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3920 2023-10-23 05:44:37.000000 aliad-0.1.0/aliad/utils/system_utils.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.882387 aliad-0.1.0/aliad.egg-info/
+-rw-r--r--   0 chlcheng (102623) chlcheng (102623)      793 2024-06-02 15:08:01.880709 aliad-0.1.0/aliad.egg-info/PKG-INFO
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1292 2024-06-02 15:08:01.881148 aliad-0.1.0/aliad.egg-info/SOURCES.txt
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        1 2024-06-02 15:08:01.881596 aliad-0.1.0/aliad.egg-info/dependency_links.txt
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       53 2024-06-02 15:08:01.882028 aliad-0.1.0/aliad.egg-info/requires.txt
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        6 2024-06-02 15:08:01.882447 aliad-0.1.0/aliad.egg-info/top_level.txt
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.899896 aliad-0.1.0/bin/
+-rwxrwx---   0 chlcheng (102623) chlcheng (102623)       22 2023-10-08 21:33:14.000000 aliad-0.1.0/bin/aliad
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       38 2024-06-02 15:08:01.903124 aliad-0.1.0/setup.cfg
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1693 2023-12-19 06:43:26.000000 aliad-0.1.0/setup.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-06-02 15:08:01.901233 aliad-0.1.0/tests/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2469 2023-10-23 02:41:06.000000 aliad-0.1.0/tests/test_data_preparation.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2667 2023-12-09 04:16:26.000000 aliad-0.1.0/tests/test_multigpu_tensorflow.py
```

### Comparing `aliad-0.0.3/LICENSE` & `aliad-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aliad-0.0.3/PKG-INFO` & `aliad-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: aliad
-Version: 0.0.3
+Version: 0.1.0
 Summary: A library for anomaly detection.
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: numba
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: click
 Requires-Dist: quickstats
 
 # ALiAD
 A Library for Anomaly Detection (ALiAD)
```

### Comparing `aliad-0.0.3/aliad/data/partition.py` & `aliad-0.1.0/aliad/data/partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import numpy as np
 
 def split_array(array, num_samples):
     if (num_samples is None) or (num_samples == 0):
         return None, array
     return array[:num_samples], array[num_samples:]
 
+def get_partition_ranges(n:int, m:int, drop_remainer:bool=False):
+    k = math.floor(n / m)
+    ranges = list(zip(range(0, n , k), range(k, n + 1, k)))
+    if not drop_remainer:
+        ranges[-1] = (ranges[-1][0], n)
+    return ranges
+
 def get_optimal_stratified_split(split_sizes:Dict, cls_sizes:Dict):
     def is_all_int(sizes_):
         return all(isinstance(size, Integral) for size in sizes_)
     split_sizes_ = list(split_sizes.values())
     if not is_all_int(split_sizes_):
         raise ValueError('split_sizes must be all integers')
     cls_sizes_ = list(cls_sizes.values())
@@ -38,15 +45,15 @@
                                 upper_bounds:Optional[np.ndarray]=None,
                                 backfill:bool=False):
     fractions = np.array(fractions)
     sum_frt = np.sum(fractions)
     if sum_frt > 1:
         raise ValueError('sum of fractions must not exceed 1')
     if not (fractions > 0).all():
-        raise ValueError('all fractions must be positibe')
+        raise ValueError('all fractions must be positive')
     exp_total = min(round(sum_frt * total), total)
     trial_sizes = np.round(total * fractions).astype(int)
     trial_total = np.sum(trial_sizes)
     if (trial_total == exp_total):
         return trial_sizes
     diff = exp_total - trial_total
     if upper_bounds is None:
@@ -69,31 +76,38 @@
         else:
             idx = indices[-1]
         trial_sizes[idx] += direction
         diff -= direction
     return trial_sizes
 
 def optimize_split_sizes(total_count:int,
-                         split_sizes:Dict, 
+                         split_sizes:Union[Dict, List], 
                          backfill:bool=False):
-    sizes = list(split_sizes.values())
+    
+    if isinstance(split_sizes, dict):
+        sizes = list(split_sizes.values())
+    else:
+        sizes = list(split_sizes)
+        
     all_int = all(isinstance(size, Integral) for size in sizes)
     if all_int:
         if np.sum(sizes) > total_count:
             raise ValueError('sum of split sizes must not exceed the total size')
         return {**split_sizes}
     sizes = np.array(sizes)
     all_frt = ((sizes > 0) & (sizes < 1)).all()
     if not all_frt:
-        raise ValueError('Sizes must be all integers or all fractions')
+        raise ValueError('sizes must be all integers or all fractions')
     sum_frt = np.sum(sizes)
     if sum_frt > 1:
         raise ValueError('sum of split fractions must not exceed 1')
     opt_sizes = optimize_fraction_partition(total_count, sizes, backfill=backfill)
-    return dict(zip(list(split_sizes), opt_sizes))
+    if isinstance(split_sizes, dict):
+        return dict(zip(list(split_sizes), opt_sizes))
+    return opt_sizes
 
 def get_train_val_test_split_sizes(total_size:int, test_size=None, val_size=None, train_size=None):
     split_sizes = {
         'train' : train_size,
         'val'   : val_size,
         'test'  : test_size
     }
@@ -109,14 +123,16 @@
     
 def get_split_indices(total_size:int, split_sizes:Union[int, Dict], stratify=None, shuffle=True, seed=None):
     if isinstance(split_sizes, int):
         split_sizes = [split_sizes] * (total_size // split_sizes) + [total_size % split_sizes]
     if isinstance(split_sizes, (list, tuple)):
         split_sizes = {i: size for i, size in enumerate(split_sizes)}
     split_sizes_ = np.array(list(split_sizes.values()))
+    if np.any(split_sizes_ <= 0):
+        raise ValueError('split sizes must be positive')
     if not np.issubdtype(split_sizes_.dtype, np.integer):
         raise ValueError('split sizes must be all integers')
     total_split_size = np.sum(split_sizes_)
     if total_split_size > total_size:
         raise ValueError('sum of split sizes must not exceed the total size')
     if stratify is not None:
         assert len(stratify) == total_size
```

### Comparing `aliad-0.0.3/aliad/data/point_cloud_dataset.py` & `aliad-0.1.0/aliad/data/point_cloud_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 from typing import Dict, List, Optional, Union
 import numpy as np
 import awkward as ak
 
 from quickstats import AbstractObject, semistaticmethod
 from quickstats.utils.common_utils import combine_dict
 
-from aliad.interface.awkward.utils import get_record_outer_shapes
-
 class PointCloudDataset(AbstractObject):
     """
     This loader will load data in memory. Improvements to be made to load lazily.
     """
     DEFAULT_FEATURE_DICT = {
         "part_coords"   : ["part_delta_eta", "part_delta_phi"],
         "part_features" : ["part_pt", "part_delta_eta", "part_delta_phi", "part_delta_R"],
@@ -41,37 +39,85 @@
         self._feature_metadata = None
 
     def __len__(self):
         return self._labels.shape[0]
 
     def convert_to_tfrecords(self, filenames:Union[Dict, str], outname:str,
                              samples:Optional[List[str]]=None,
-                             aux_features:Dict=None):
+                             aux_features:Dict=None,
+                             num_shards:Optional[int]=None,
+                             cache:bool=True):
+        """
+        """
         import tensorflow as tf
-        from aliad.interface.tensorflow.dataset import ndarray_to_tfrecords
+        from aliad.interface.tensorflow.dataset import array_to_tfrecords
+        from aliad.data.partition import get_partition_ranges
+        
         samples = self.resolve_samples(samples)
-        writer = tf.io.TFRecordWriter(outname)
-        metadata = {'features': None, 'sample_size': {}}
-        self.stdout.info(f'Created TFRecordWriter for the output "{outname}"')
-        for sample in samples:
-            self.stdout.info(f'Writing to tfrecord for the sample "{sample}"')
+
+        def save_metadata(metadata:Dict, outname:str, indent:int=2):
+            with open(outname, 'w') as f:
+                json.dump(metadata, f, indent=indent)
+
+        def get_metadata_outname(tfrecord_outname:str):
+            return f'{os.path.splitext(tfrecord_outname)[0]}_metadata.json'
+
+        def get_features(sample:str):
             self.load(filenames, samples=[sample])
             features = {**self.X}
             features['label']  = self.y
             features['weight'] = self.weight
-            if aux_features is not None:
+            if (aux_features is not None) and (sample in aux_features):
                 features.update(aux_features[sample])
-            metadata_ = ndarray_to_tfrecords(writer, **features)
-            metadata['features'] = metadata_['features']
-            metadata['sample_size'][sample] = metadata_['size']
-            self.clear()
-        metadata_outname = f'{os.path.splitext(outname)[0]}_metadata.json'
-        with open(metadata_outname, 'w') as f:
-            json.dump(metadata, f, indent=2)
-            self.stdout.info(f'Saved tfrecord metadata to "{metadata_outname}"')
+            return features
+            
+        if (num_shards is None):
+            metadata_outname = get_metadata_outname(outname)
+            if cache and os.path.exists(metadata_outname):
+                self.stdout.info(f'Cached TFRecord output from "{outname}"')
+                return None
+            writer = tf.io.TFRecordWriter(outname)
+            metadata = {}
+            metadata['sample_size'] = {}
+            metadata['size'] = 0
+            self.stdout.info(f'Creating TFRecord data for the sample "{sample}"')
+            for sample in samples:
+                features = get_features(sample)
+                sample_metadata = array_to_tfrecords(writer, **features)
+                metadata['featues'] = sample_metadata['features']
+                metadata['sample_size'][sample] = sample_metadata['size']
+                metadata['size'] += sample_metadata['size']
+                self.clear()
+            save_metadata(metadata, metadata_outname)
+            writer.close()
+        else:
+            if len(samples) > 1:
+                raise ValueError('num_shards option not allowed when number of samples > 1')
+            if '{shard_index}' not in outname:
+                tokens = os.path.splitext(outname)
+                outname = f"{tokens[0]}_shard_{{shard_index}}{tokens[1]}"
+            outnames = [outname.format(shard_index=i) for i in range(num_shards)]
+            metadata_outnames = [get_metadata_outname(outname) for outname in outnames]
+            if all(os.path.exists(filename) for filename in metadata_outnames):
+                self.stdout.info(f'Cached TFRecord output from "{outname}"')
+                return None
+            sample = samples[0]
+            self.stdout.info(f'Creating TFRecord data for the sample "{sample}"')
+            features = get_features(sample)
+            sample_size = features['label'].shape[0]
+            partition_ranges = get_partition_ranges(sample_size, num_shards)
+            silent_flag = False
+            for index, prange in enumerate(partition_ranges):
+                part_features = {key:arrays[prange[0]:prange[1]] for key, arrays in features.items()}
+                writer = tf.io.TFRecordWriter(outnames[index])
+                metadata = array_to_tfrecords(writer, silent=silent_flag,
+                                              **part_features)
+                silent_flag = True
+                metadata["sample_size"] = {sample: sample_size}
+                save_metadata(metadata, metadata_outnames[index])
             
     def set_class_labels(self, class_labels:Dict):
         class_labels = combine_dict(class_labels)
         label_map = {}
         for class_value, labels in class_labels.items():
             for label in labels:
                 if label in label_map:
@@ -176,16 +222,16 @@
                 jet_feature_arrays = []
                 jet_mask_arrays = []
                 for i in range(1, self.num_jets + 1):
                     self.stdout.info(f'Jet index: {i}')
                     jet_key = f'j{i}'
                     feature_arrays = []
                     mask_array = None
+                    self.stdout.info(f'Loading data for the features {", ".join(columns)}')
                     for column in columns:
-                        self.stdout.info(f'Loading data for the feature "{column}"')
                         arrays = sample_arrays[jet_key][column]
                         if self.is_ragged(arrays):
                             # only get the mask once per jet
                             if (mask_array is None):
                                 mask_array = self.get_mask_array(arrays, self.pad_size,
                                                                  sample_size=sample_size)
                             arrays = self.get_padded_array(arrays, self.pad_size,
```

### Comparing `aliad-0.0.3/aliad/interface/awkward/momentum_4d_array_builder.py` & `aliad-0.1.0/aliad/interface/awkward/momentum_4d_array_builder.py`

 * *Files identical despite different names*

### Comparing `aliad-0.0.3/aliad/interface/fastjet/jet_clustering_tool.py` & `aliad-0.1.0/aliad/interface/fastjet/jet_clustering_tool.py`

 * *Files identical despite different names*

### Comparing `aliad-0.0.3/aliad/interface/tensorflow/dataset.py` & `aliad-0.1.0/aliad/interface/tensorflow/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,58 @@
 from functools import partial
-from typing import Optional, Tuple, Union, Iterable, Callable, Dict, List
+import json
+from typing import Optional, Tuple, Union, Iterable, Callable, Dict, List, Any
+
 import numpy as np
 import tensorflow as tf
 
 from tensorflow.keras import Input
 
-from aliad.data.partition import get_split_indices, get_train_val_test_split_sizes
+from quickstats import VerbosePrint
+from quickstats.utils.string_utils import get_field_names
+from aliad.data.partition import (
+    get_split_indices, get_train_val_test_split_sizes,
+    get_partition_ranges
+)
 
 def apply_pipelines(ds:tf.data.Dataset,
-                    batch_size: int = 32,
+                    batch_size: Optional[int] = None,
                     shuffle: bool = True,
                     seed: Optional[int] = None,
-                    drop_remainder: bool = True,
+                    drop_remainder: bool = False,
                     buffer_size: Optional[int] = None,
                     cache:bool = False,
                     prefetch:bool = True,
-                    repeat:bool = False) -> tf.data.Dataset:
+                    repeat:bool = False,
+                    reshuffle_each_iteration:bool=False,
+                    distribute_strategy=None) -> tf.data.Dataset:
     if cache:
         ds = ds.cache()
 
     if shuffle:
-        ds = ds.shuffle(buffer_size=buffer_size, seed=seed, reshuffle_each_iteration=True)
+        if buffer_size is None:
+            sample_size = ds.cardinality().numpy()
+            if sample_size < 0:
+                raise RuntimeError('buffer_size must be given when shuffle is True while'
+                                   'cardinality of dataset can not be determined')
+            buffer_size = sample_size            
+        ds = ds.shuffle(buffer_size=buffer_size, seed=seed,
+                        reshuffle_each_iteration=reshuffle_each_iteration)
 
     if batch_size is not None:
         ds = ds.batch(batch_size, drop_remainder=drop_remainder)
 
-    if repeat:
+    if repeat or (distribute_strategy is not None):
         ds = ds.repeat()
 
-    if prefetch:
+    if prefetch and (distribute_strategy is None):
         ds = ds.prefetch(tf.data.AUTOTUNE)
+
+    if (distribute_strategy is not None):
+        ds = distribute_strategy.experimental_distribute_dataset(ds)
     return ds
 
 def prepare_dataset(*X: Union[np.ndarray, tf.Tensor], 
                     y: Union[np.ndarray, tf.Tensor],
                     weight: Optional[Union[np.ndarray, tf.Tensor]]=None,
                     batch_size: int = 32,
                     shuffle: bool = True,
@@ -118,61 +137,57 @@
                              buffer_size=buffer_size, 
                              prefetch=prefetch,
                              drop_remainder=drop_remainder,
                              cache=cache, 
                              repeat=repeat)
     return ds
 
-def get_tf_inputs(metadata:Dict):
-    Inputs = {}
-    for label, feature_metadata  in metadata.items():
-        Inputs[label] = Input(name=label, **feature_metadata)
-    return Inputs
-
-def get_feature_method(array:np.ndarray):
-    """match appropriate tf.train.Feature class with dtype of ndarray. """
-    dtype_ = array.dtype.name
-    if dtype_ in ['float32']:
-        # note FloatList converts float/double to float
-        return lambda array_: tf.train.Feature(float_list=tf.train.FloatList(value=array_))
-    elif dtype_ in ['float64', 'bool']:
-        return lambda array_: tf.train.Feature(bytes_list=tf.train.BytesList(value=[array_.tobytes()]))
-    elif dtype_ in ['int64']:
-        return lambda array_: tf.train.Feature(int64_list=tf.train.Int64List(value=array_))
-    else:  
-        raise ValueError('array must have dtype of float32, float64, or int64')
-
-def get_feature_description(array:tf.Tensor):
-        """match appropriate tf.train.Feature class with dtype of ndarray. """
-        dtype_ = array.dtype.name
-        if dtype_ in ['float32', 'int64']:
-            return tf.io.FixedLenFeature([np.prod(array.shape[1:])], dtype=dtype_)
-        elif dtype_ in ['float64', 'bool']:
-            return tf.io.FixedLenFeature([], dtype=tf.string)
-        else:
-            raise ValueError('array must have dtype of float32, float64, or int64')
+def feature_selector(inner_slices:List[str], outer_slices:List[str]):
+    def map_fn(X):
+        return tuple(X[ins] for ins in inner_slices), *(X[outs] for outs in outer_slices)
+    return map_fn
+
+def get_symbolic_inputs(metadata_map:Dict, downcast:bool=False,
+                        keys:Optional[List[str]]=None):
+    """symbolic tensor or placeholders"""
+    inputs = {}
+    if keys is None:
+        keys = list(metadata_map.keys())
+    for key in keys:
+        metadata = metadata_map[key]
+        if downcast and (metadata['dtype'] == 'float64'):
+            metadata = dict(metadata)
+            metadata['dtype'] = 'float32'
+        inputs[key] = Input(name=key, **metadata)
+    return inputs
         
-def get_ndarray_tfrecord_example_parser(metadata:Dict):
-    Inputs = get_tf_inputs(metadata)
+def get_tfrecord_array_parser(feature_metadata:Dict, downcast:bool=False,
+                              keys:Optional[List[str]]=None):
+    keys = keys or list(feature_metadata)
+    inputs = get_symbolic_inputs(feature_metadata, keys=keys)
     feature_description = {}
     feature_parser = {}
-    for label, input_ in Inputs.items():
+    for label, input_ in inputs.items():
         feature_description[label] = get_feature_description(input_)
         dtype = input_.dtype
         shape = input_.shape[1:]
         if dtype.name in ['bool', 'float64']:
-            feature_parser[label] = (lambda example, out_type=dtype, shape=shape:
-                                     tf.reshape(tf.io.decode_raw(example, out_type=out_type), shape))
+            if downcast and dtype.name == 'float64':
+                feature_parser[label] = (lambda example, shape=shape:
+                                         tf.cast(tf.reshape(tf.io.decode_raw(example, out_type='float64'), shape), dtype='float32'))
+            else:
+                feature_parser[label] = (lambda example, out_type=dtype, shape=shape:
+                                         tf.reshape(tf.io.decode_raw(example, out_type=out_type), shape))
         else:
             feature_parser[label] = (lambda example, shape=shape:
                                      tf.reshape(example, shape))
     
     def get_parsed_example(example):
         parsed_example = tf.io.parse_single_example(example, feature_description)
-        for label, input_ in Inputs.items():
+        for label, input_ in inputs.items():
             parsed_example[label] = feature_parser[label](parsed_example[label])
         return parsed_example
         
     return get_parsed_example
 
 def tfds_to_tfrecords(ds, writer:"tf.io.TFRecordWriter"):
     if isinstance(writer, str):
@@ -202,76 +217,169 @@
         writer.write(serialized)
         size += 1
     metadata = {
         "features": feature_metadata,
         "size": size
     }
     return metadata
-        
 
-def ndarray_to_tfrecords(writer:"tf.io.TFRecordWriter", **X):
-    if isinstance(writer, str):
-        writer = tf.io.TFRecordWriter(writer)
-    def _make_proper_array(label, x_):
-        if x_.ndim == 1:
-            print(f'Warning: array "{label}" of dimension = 1 will be reshaped to dimension 2')
-            x_ = x_.reshape((x_.shape[0], 1))
-        shape = x_.shape[1:]
-        dtype_ = x_.dtype.name
-        if x_.ndim > 2:
-            print(f'Warning: array "{label}" of dimension > 2 will be reshaped to dimension 2')
-            x_ = x_.reshape((x_.shape[0], np.prod(x_.shape[1:])))
-        if dtype_ not in ['float32', 'float64', 'int64', 'bool']:
-            raise ValueError(f'invalid input "{label}": array must have dtype of float32, float64, bool or int64')
-        if dtype_ in ['bool', 'float64']:
-            print(f'Warning: {dtype_} array "{label}" will be converted into bytes')
-        metadata = {"shape": shape, "dtype": dtype_}
-        return x_, metadata
-    def _validate_arrays(**X_):
-        valid_X_ = {}
-        metadata = {}
-        sizes = []
-        invalid_X_ = {}
-        for i, (label, x_) in enumerate(X_.items()):
-            if not isinstance(x_, np.ndarray):
-                valid_X_[label] = None
-                metadata[label] = None
-                invalid_X_[label] = x_
-                continue
-            valid_X_[label], metadata_ = _make_proper_array(label, x_)
-            metadata[label] = metadata_
-            sizes.append(x_.shape[0])
-        if np.unique(sizes).shape[0] != 1:
-            raise ValueError('input arrays have inconsistent batch sizes')
-        size = sizes[0]
-        for label, x_ in invalid_X_.items():
-            np_x_ = np.array(x_)
-            if np_x_.shape == ():
-                np_x_ = np_x_.reshape(1)
-            new_shape = (size,) + tuple(np.ones(np_x_.ndim, dtype='int64'))
-            print(f'Warning: input "{label}" is not a np array, it will be broadcasted into np.ndarray with shape {new_shape}')
-            np_x_ = np.tile(np_x_, new_shape)
-            valid_X_[label], metadata_ = _make_proper_array(label, np_x_)
-            metadata[label] = metadata_
-        metadata_ = {"features": metadata, "size": size}
-        return valid_X_, metadata_
-    valid_X, metadata = _validate_arrays(**X)
-    feature_methods = {}
-    for label, array in valid_X.items():
-        feature_methods[label] = get_feature_method(array)
-    for i in range(metadata['size']):
-        feature = {}
-        for label, method in feature_methods.items():
-            feature[label] = method(valid_X[label][i])
-        features = tf.train.Features(feature=feature)
-        example = tf.train.Example(features=features)
+def get_feature_description(array:tf.Tensor):
+    dtype_ = array.dtype.name
+    if dtype_ in ['float32', 'int64']:
+        return tf.io.FixedLenFeature([np.prod(array.shape[1:])], dtype=dtype_)
+    elif dtype_ in ['float64', 'bool']:
+        return tf.io.FixedLenFeature([], dtype=tf.string)
+    else:
+        raise ValueError('array must have dtype of float32, float64, or int64')
+
+def float_feature(array: np.ndarray) -> tf.train.Feature:
+    """
+    Converts a numpy array of floats to a TensorFlow float_list Feature.
+
+    Parameters
+    ----------
+    array : np.ndarray
+        Input array with dtype float32.
+
+    Returns
+    -------
+    tf.train.Feature
+        A TensorFlow Feature containing the float list.
+    """
+    return tf.train.Feature(float_list=tf.train.FloatList(value=array))
+
+def bytes_feature(array: np.ndarray) -> tf.train.Feature:
+    """
+    Converts a numpy array to a TensorFlow bytes_list Feature.
+
+    Parameters
+    ----------
+    array : np.ndarray
+        Input array with any dtype.
+
+    Returns
+    -------
+    tf.train.Feature
+        A TensorFlow Feature containing the bytes list.
+    """
+    return tf.train.Feature(bytes_list=tf.train.BytesList(value=[array.tobytes()]))
+
+def int64_feature(array: np.ndarray) -> tf.train.Feature:
+    """
+    Converts a numpy array of int64s to a TensorFlow int64_list Feature.
+
+    Parameters
+    ----------
+    array : np.ndarray
+        Input array with dtype int64.
+
+    Returns
+    -------
+    tf.train.Feature
+        A TensorFlow Feature containing the int64 list.
+    """
+    return tf.train.Feature(int64_list=tf.train.Int64List(value=array))
+
+def get_feature_method(array:np.ndarray):
+    """Match appropriate tf.train.Feature class with dtype of an array. """
+    dtype = array.dtype.name
+    if dtype in ['float32']:
+        # note FloatList converts float/double to float
+        return float_feature
+    elif dtype in ['float64', 'bool']:
+        return bytes_feature
+    elif dtype in ['int64']:
+        return int64_feature
+    else:  
+        raise ValueError('array must have dtype of float32, float64, or int64')
+
+def write_tfrecord(writer: tf.io.TFRecordWriter, **X: Any) -> Dict[str, Any]:
+    """
+    Write array data to a TFRecord file.
+
+    Parameters
+    ----------
+    writer : tf.io.TFRecordWriter
+        A TFRecordWriter instance.
+    **X : Any
+        Key-value pairs where the key is the label and the value is the data.
+
+    Returns
+    -------
+    dict
+        A dictionary containing metadata about the features.
+    """
+    
+    def _regularize_array(x: np.ndarray) -> (np.ndarray, Dict[str, Any]):
+        if x.ndim == 1:
+            x = x.reshape((x.shape[0], 1))
+        shape = x.shape[1:]
+        # contract to 2D, will be reshaped after decoding
+        if x.ndim > 2:
+            x = x.reshape((x.shape[0], np.prod(x.shape[1:])))
+        dtype = x.dtype.name
+        if dtype not in ['float32', 'float64', 'bool', 'int64']:
+            raise ValueError('Array must have dtype of float32, float64, bool or int64')
+        feature_metadata = {"shape": shape, "dtype": dtype}
+        return x, feature_metadata
+
+    valid_X = {}
+    invalid_X = {}
+    metadata = {"features": {}}
+    sizes = []
+
+    for label, x in X.items():
+        if not isinstance(x, np.ndarray):
+            invalid_X[label] = x
+            valid_X[label] = None
+            metadata["features"][label] = None
+            continue
+        valid_X[label], feature_metadata = _regularize_array(x)
+        metadata["features"][label] = feature_metadata
+        sizes.append(x.shape[0])
+
+    if np.unique(sizes).shape[0] != 1:
+        raise ValueError('Arrays have inconsistent batch sizes')
+    size = sizes[0]
+    metadata['size'] = size
+
+    # forcing all arrays to have the same batchsize
+    for label, x in invalid_X.items():
+        x = np.array(x)
+        if x.shape == ():
+            x = x.reshape(1)
+        new_shape = (size,) + tuple(np.ones(x.ndim, dtype='int64'))
+        tiled_x = np.tile(x, new_shape)
+        valid_X[label], feature_metadata = _regularize_array(tiled_x)
+        metadata["features"][label] = feature_metadata
+
+    feature_methods = {label: get_feature_method(x) for label, x in valid_X.items()}
+
+    # bottleneck is here
+    for i in range(size):
+        feature = {label: method(valid_X[label][i]) for label, method in feature_methods.items()}
+        example = tf.train.Example(features=tf.train.Features(feature=feature))
         serialized = example.SerializeToString()
         writer.write(serialized)
+
     return metadata
 
+def arrays_to_sharded_tfrecords(filename_fmt:str, num_shards:int, parallel:int=0, **X):
+    if "shard_index" not in get_field_names(filename_fmt):
+        raise ValueError('filename_fmt must contain the field name "shard_index"')
+    array_sizes = [len(x) for x in X.values()]
+    if np.unique(array_sizes).shape[0] != 1:
+        raise ValueError('input arrays have inconsistent batch sizes')
+    array_size = array_sizes[0]
+    partition_ranges = get_partition_ranges(array_size, num_shards)
+    part_X = []
+    for i, prange in enumerate(partition_ranges):
+        part_x = {key:x[prange[0]:prange[1]] for key, x in X.items()}
+        part_X.append(part_x)
+
 def select_dataset_by_index(ds, indices):
     # Make a tensor of type tf.int64 to match the one by Dataset.enumerate(). 
     indices_ts = tf.constant(indices, dtype='int64')
     def is_index_in(index, rest):
         return tf.math.reduce_any(tf.math.equal(index, indices_ts))
     def drop_index(index, rest):
         return rest
@@ -340,8 +448,32 @@
                                   shuffle=shuffle_index, seed=seed)   
     return ds_splits
 
 """
 tf.data.TFRecordDataset(filenames, num_parallel_reads=tf.data.AUTOTUNE)
 tf.data.Dataset.list_files(pattern).interleave(tf.data.TFRecordDataset, cycle_length=tf.data.AUTOTUNE, num_parallel_calls=tf.data.AUTOTUNE)
 
-"""
+"""
+
+def count_elements(dataset: tf.data.Dataset):
+    return dataset.reduce(0, lambda x, _ : x + 1).numpy()
+
+def concatenate_datasets(datasets: List[tf.data.Dataset]):
+    ds = datasets[0]
+    for ds_i in datasets[1:]:
+        ds = ds.concatenate(ds_i)
+    return ds
+
+def get_tfrecord_dataset(filenames:List[str], parse_fn,
+                         dataset_options:Optional[Dict]=None,
+                         map_options:Optional[Dict]=None):
+    if dataset_options is None:
+        dataset_options = {}
+    if map_options is None:
+        map_options = {}
+    if 'num_parallel_reads' not in dataset_options:
+        dataset_options['num_parallel_reads'] = tf.data.AUTOTUNE
+    if 'num_parallel_calls' not in map_options:
+        map_options['num_parallel_calls'] = tf.data.AUTOTUNE
+    ds = tf.data.TFRecordDataset(filenames, **dataset_options)
+    ds = ds.map(parse_fn, **map_options)
+    return ds
```

### Comparing `aliad-0.0.3/aliad/interface/tensorflow/layers.py` & `aliad-0.1.0/aliad/interface/tensorflow/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional, Tuple, List
 
 import tensorflow as tf
 
 from tensorflow.keras.layers import (BatchNormalization, Activation,
                                      Conv2D, Conv3D, Dense, Dropout)
+from tensorflow.keras.initializers import GlorotNormal
 
 from .operations import (transpose_last_n_dimensions, trim_elements,
                          generate_batch_indices, merge_dimensions)
 
 def DMatrix(A:tf.Tensor, B:tf.Tensor, name:str="DMatrix") -> tf.Tensor:
     """
 
@@ -100,14 +101,15 @@
              channels:Tuple[int],
              K:int=16,
              batchnorm:bool=True,
              rel_fts:bool=True,
              activation:str='relu',
              pooling:str='average',
              name:str='EdgeConv',
+             seed:Optional[int]=None,
              conv_type:str='3D'):
     """
     Args
         channels: Tuple of int
             Number of output channels in each convolution
         points: Tensor of shape (nevent, njet, nparticle, ncoords)
             Coordinates of the point cloud particles
@@ -139,15 +141,15 @@
             kernal_size = (1, 1, 1)
         else:
             raise ValueError('conv type must be either "2D" or "3D"')
         for idx, channel in enumerate(channels):
             x = conv_fn(channel, kernel_size=kernal_size, strides=1,
                         data_format='channels_last',
                         use_bias=use_bias,
-                        kernel_initializer='glorot_normal',
+                        kernel_initializer=GlorotNormal(seed),
                         name=f'{name}_conv{idx}')(x)
             if batchnorm:
                 x = BatchNormalization(name=f'{name}_bn{idx}')(x)
             if activation:
                 x = Activation(activation, name=f'{name}_act{idx}')(x)
         # shape after pooling: (batch dims..., npoints, nchannel)
         if pooling == 'max':
@@ -155,15 +157,15 @@
         else:
             fts = tf.reduce_mean(x, axis=-2)
 
         # shortcut
         sc = conv_fn(channels[-1], kernel_size=kernal_size, strides=1,
                      data_format='channels_last',
                      use_bias=use_bias,
-                     kernel_initializer='glorot_normal',
+                     kernel_initializer=GlorotNormal(seed),
                      name=f'{name}_sc_conv')(tf.expand_dims(features, axis=-2))
         if batchnorm:
             sc = BatchNormalization(name=f'{name}_sc_bn')(sc)
         sc = tf.squeeze(sc, axis=-2)
         x = tf.add(sc, fts)
         # shape: (batch dims..., npoints, nchannel)
         if activation:
```

### Comparing `aliad-0.0.3/aliad/interface/tensorflow/operations.py` & `aliad-0.1.0/aliad/interface/tensorflow/operations.py`

 * *Files identical despite different names*

### Comparing `aliad-0.0.3/aliad/interface/tensorflow/utils.py` & `aliad-0.1.0/aliad/interface/tensorflow/utils.py`

 * *Files identical despite different names*

### Comparing `aliad-0.0.3/aliad/utils/system_utils.py` & `aliad-0.1.0/aliad/utils/system_utils.py`

 * *Files identical despite different names*

### Comparing `aliad-0.0.3/aliad.egg-info/PKG-INFO` & `aliad-0.1.0/aliad.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: aliad
-Version: 0.0.3
+Version: 0.1.0
 Summary: A library for anomaly detection.
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: numba
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: click
 Requires-Dist: quickstats
 
 # ALiAD
 A Library for Anomaly Detection (ALiAD)
```

### Comparing `aliad-0.0.3/aliad.egg-info/SOURCES.txt` & `aliad-0.1.0/aliad.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,29 +4,38 @@
 aliad/__init__.py
 aliad/_version.py
 aliad.egg-info/PKG-INFO
 aliad.egg-info/SOURCES.txt
 aliad.egg-info/dependency_links.txt
 aliad.egg-info/requires.txt
 aliad.egg-info/top_level.txt
+aliad/components/__init__.py
+aliad/components/evaluation.py
+aliad/components/metrics.py
+aliad/components/model_output.py
 aliad/data/__init__.py
 aliad/data/partition.py
 aliad/data/point_cloud_dataset.py
 aliad/interface/__init__.py
 aliad/interface/awkward/__init__.py
 aliad/interface/awkward/momentum_4d_array_builder.py
 aliad/interface/awkward/utils.py
 aliad/interface/fastjet/__init__.py
 aliad/interface/fastjet/jet_clustering_tool.py
 aliad/interface/tensorflow/__init__.py
 aliad/interface/tensorflow/callbacks.py
 aliad/interface/tensorflow/dataset.py
 aliad/interface/tensorflow/layers.py
+aliad/interface/tensorflow/losses.py
 aliad/interface/tensorflow/operations.py
+aliad/interface/tensorflow/regularizers.py
+aliad/interface/tensorflow/tfrecord_maker.py
 aliad/interface/tensorflow/utils.py
-aliad/interface/tensorflow/modules/MLP.py
-aliad/interface/tensorflow/modules/__init__.py
+aliad/interface/tensorflow/models/MLP.py
+aliad/interface/tensorflow/models/MultiParticleNet.py
+aliad/interface/tensorflow/models/__init__.py
 aliad/utils/__init__.py
 aliad/utils/array_utils.py
 aliad/utils/system_utils.py
 bin/aliad
-tests/test_data_preparation.py
+tests/test_data_preparation.py
+tests/test_multigpu_tensorflow.py
```

### Comparing `aliad-0.0.3/setup.py` & `aliad-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
           'numpy',
+          'scipy',
+          'numba',
           'pandas',
           'matplotlib',
           'click',
           'quickstats'
       ],
     scripts=[f'bin/{PACKAGENAME}'],
     python_requires='>=3.8',
```

### Comparing `aliad-0.0.3/tests/test_data_preparation.py` & `aliad-0.1.0/tests/test_data_preparation.py`

 * *Files identical despite different names*

