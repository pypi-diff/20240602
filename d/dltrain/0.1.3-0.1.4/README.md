# Comparing `tmp/dltrain-0.1.3.tar.gz` & `tmp/dltrain-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dltrain-0.1.3.tar", last modified: Sun May 26 15:34:41 2024, max compression
+gzip compressed data, was "dltrain-0.1.4.tar", last modified: Sun Jun  2 07:15:44 2024, max compression
```

## Comparing `dltrain-0.1.3.tar` & `dltrain-0.1.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.300329 dltrain-0.1.3/
--rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     6988 2024-05-26 15:34:41.299329 dltrain-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6351 2024-05-26 15:34:09.000000 dltrain-0.1.3/README.md
--rw-rw-rw-   0        0        0      625 2024-05-21 08:07:45.000000 dltrain-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-26 15:34:41.300329 dltrain-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.079808 dltrain-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.158810 dltrain-0.1.3/src/dltrain/
--rw-rw-rw-   0        0        0      229 2024-05-05 13:13:52.000000 dltrain-0.1.3/src/dltrain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.259332 dltrain-0.1.3/src/dltrain/builder/
--rw-rw-rw-   0        0        0       32 2024-05-04 13:43:22.000000 dltrain-0.1.3/src/dltrain/builder/__init__.py
--rw-rw-rw-   0        0        0     1366 2024-05-23 07:36:29.000000 dltrain-0.1.3/src/dltrain/builder/base.py
--rw-rw-rw-   0        0        0     3219 2024-05-07 03:07:53.000000 dltrain-0.1.3/src/dltrain/builder/builder.py
--rw-rw-rw-   0        0        0      212 2024-05-04 13:37:24.000000 dltrain-0.1.3/src/dltrain/builder/core.py
--rw-rw-rw-   0        0        0      714 2024-05-05 13:08:13.000000 dltrain-0.1.3/src/dltrain/builder/criterion.py
--rw-rw-rw-   0        0        0     2264 2024-05-08 02:25:24.000000 dltrain-0.1.3/src/dltrain/builder/dataset.py
--rw-rw-rw-   0        0        0      721 2024-05-05 13:08:13.000000 dltrain-0.1.3/src/dltrain/builder/delineator.py
--rw-rw-rw-   0        0        0     1556 2024-05-05 13:08:13.000000 dltrain-0.1.3/src/dltrain/builder/evaluation.py
--rw-rw-rw-   0        0        0      488 2024-05-07 01:12:49.000000 dltrain-0.1.3/src/dltrain/builder/forward.py
--rw-rw-rw-   0        0        0      281 2024-05-07 03:07:32.000000 dltrain-0.1.3/src/dltrain/builder/inject.py
--rw-rw-rw-   0        0        0     1454 2024-05-21 09:17:11.000000 dltrain-0.1.3/src/dltrain/builder/model.py
--rw-rw-rw-   0        0        0     1169 2024-05-07 01:28:56.000000 dltrain-0.1.3/src/dltrain/builder/optimizer.py
--rw-rw-rw-   0        0        0      533 2024-05-04 13:52:21.000000 dltrain-0.1.3/src/dltrain/builder/scheduler.py
--rw-rw-rw-   0        0        0      834 2024-05-08 02:35:03.000000 dltrain-0.1.3/src/dltrain/builder/transforms.py
--rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.1.3/src/dltrain/checkpoint.py
--rw-rw-rw-   0        0        0     5857 2024-05-26 15:34:09.000000 dltrain-0.1.3/src/dltrain/dataset.py
--rw-rw-rw-   0        0        0     1300 2024-05-05 13:08:13.000000 dltrain-0.1.3/src/dltrain/delineator.py
--rw-rw-rw-   0        0        0      935 2024-05-03 11:30:58.000000 dltrain-0.1.3/src/dltrain/error.py
--rw-rw-rw-   0        0        0     3955 2024-05-26 15:27:39.000000 dltrain-0.1.3/src/dltrain/evaluation.py
--rw-rw-rw-   0        0        0     6478 2024-05-07 02:10:02.000000 dltrain-0.1.3/src/dltrain/forward.py
--rw-rw-rw-   0        0        0     1203 2024-05-07 03:07:32.000000 dltrain-0.1.3/src/dltrain/inject.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.296328 dltrain-0.1.3/src/dltrain/models/
--rw-rw-rw-   0        0        0      150 2024-05-21 09:08:46.000000 dltrain-0.1.3/src/dltrain/models/__init__.py
--rw-rw-rw-   0        0        0     1028 2024-05-21 09:08:46.000000 dltrain-0.1.3/src/dltrain/models/builder.py
--rw-rw-rw-   0        0        0     1617 2024-05-21 09:08:46.000000 dltrain-0.1.3/src/dltrain/models/component.py
--rw-rw-rw-   0        0        0     1975 2024-05-26 15:34:09.000000 dltrain-0.1.3/src/dltrain/models/model.py
--rw-rw-rw-   0        0        0     3040 2024-05-08 02:46:50.000000 dltrain-0.1.3/src/dltrain/models/wrapper.py
--rw-rw-rw-   0        0        0     1326 2024-05-23 06:05:54.000000 dltrain-0.1.3/src/dltrain/options.py
--rw-rw-rw-   0        0        0    13122 2024-05-21 08:05:29.000000 dltrain-0.1.3/src/dltrain/train.py
--rw-rw-rw-   0        0        0     1405 2024-05-08 02:35:03.000000 dltrain-0.1.3/src/dltrain/transform.py
--rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.1.3/src/dltrain/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.298329 dltrain-0.1.3/src/dltrain.egg-info/
--rw-rw-rw-   0        0        0     6988 2024-05-26 15:34:41.000000 dltrain-0.1.3/src/dltrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2024-05-26 15:34:41.000000 dltrain-0.1.3/src/dltrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 15:34:41.000000 dltrain-0.1.3/src/dltrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 15:34:41.000000 dltrain-0.1.3/src/dltrain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 07:15:44.998658 dltrain-0.1.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     6992 2024-06-02 07:15:44.996659 dltrain-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6355 2024-05-26 15:42:32.000000 dltrain-0.1.4/README.md
+-rw-rw-rw-   0        0        0      625 2024-05-26 15:47:47.000000 dltrain-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 07:15:44.998658 dltrain-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 07:15:44.930660 dltrain-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 07:15:44.954661 dltrain-0.1.4/src/dltrain/
+-rw-rw-rw-   0        0        0      229 2024-05-05 13:13:52.000000 dltrain-0.1.4/src/dltrain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:15:44.987658 dltrain-0.1.4/src/dltrain/builder/
+-rw-rw-rw-   0        0        0       32 2024-05-04 13:43:22.000000 dltrain-0.1.4/src/dltrain/builder/__init__.py
+-rw-rw-rw-   0        0        0     1366 2024-05-23 07:36:29.000000 dltrain-0.1.4/src/dltrain/builder/base.py
+-rw-rw-rw-   0        0        0     3219 2024-05-07 03:07:53.000000 dltrain-0.1.4/src/dltrain/builder/builder.py
+-rw-rw-rw-   0        0        0      212 2024-05-04 13:37:24.000000 dltrain-0.1.4/src/dltrain/builder/core.py
+-rw-rw-rw-   0        0        0      714 2024-05-05 13:08:13.000000 dltrain-0.1.4/src/dltrain/builder/criterion.py
+-rw-rw-rw-   0        0        0     2264 2024-06-02 07:13:44.000000 dltrain-0.1.4/src/dltrain/builder/dataset.py
+-rw-rw-rw-   0        0        0      721 2024-05-05 13:08:13.000000 dltrain-0.1.4/src/dltrain/builder/delineator.py
+-rw-rw-rw-   0        0        0     1556 2024-05-05 13:08:13.000000 dltrain-0.1.4/src/dltrain/builder/evaluation.py
+-rw-rw-rw-   0        0        0      488 2024-05-07 01:12:49.000000 dltrain-0.1.4/src/dltrain/builder/forward.py
+-rw-rw-rw-   0        0        0      281 2024-05-07 03:07:32.000000 dltrain-0.1.4/src/dltrain/builder/inject.py
+-rw-rw-rw-   0        0        0     1454 2024-05-21 09:17:11.000000 dltrain-0.1.4/src/dltrain/builder/model.py
+-rw-rw-rw-   0        0        0     1169 2024-05-07 01:28:56.000000 dltrain-0.1.4/src/dltrain/builder/optimizer.py
+-rw-rw-rw-   0        0        0      533 2024-05-04 13:52:21.000000 dltrain-0.1.4/src/dltrain/builder/scheduler.py
+-rw-rw-rw-   0        0        0      834 2024-05-08 02:35:03.000000 dltrain-0.1.4/src/dltrain/builder/transforms.py
+-rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.1.4/src/dltrain/checkpoint.py
+-rw-rw-rw-   0        0        0     5857 2024-05-26 15:34:09.000000 dltrain-0.1.4/src/dltrain/dataset.py
+-rw-rw-rw-   0        0        0     1300 2024-05-05 13:08:13.000000 dltrain-0.1.4/src/dltrain/delineator.py
+-rw-rw-rw-   0        0        0      935 2024-05-03 11:30:58.000000 dltrain-0.1.4/src/dltrain/error.py
+-rw-rw-rw-   0        0        0     3955 2024-05-26 15:27:39.000000 dltrain-0.1.4/src/dltrain/evaluation.py
+-rw-rw-rw-   0        0        0     6478 2024-05-07 02:10:02.000000 dltrain-0.1.4/src/dltrain/forward.py
+-rw-rw-rw-   0        0        0     1203 2024-05-07 03:07:32.000000 dltrain-0.1.4/src/dltrain/inject.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:15:44.993659 dltrain-0.1.4/src/dltrain/models/
+-rw-rw-rw-   0        0        0      150 2024-05-21 09:08:46.000000 dltrain-0.1.4/src/dltrain/models/__init__.py
+-rw-rw-rw-   0        0        0     1028 2024-05-21 09:08:46.000000 dltrain-0.1.4/src/dltrain/models/builder.py
+-rw-rw-rw-   0        0        0     1617 2024-05-21 09:08:46.000000 dltrain-0.1.4/src/dltrain/models/component.py
+-rw-rw-rw-   0        0        0     1975 2024-05-26 15:34:09.000000 dltrain-0.1.4/src/dltrain/models/model.py
+-rw-rw-rw-   0        0        0     3040 2024-05-08 02:46:50.000000 dltrain-0.1.4/src/dltrain/models/wrapper.py
+-rw-rw-rw-   0        0        0     1326 2024-05-23 06:05:54.000000 dltrain-0.1.4/src/dltrain/options.py
+-rw-rw-rw-   0        0        0    13122 2024-05-21 08:05:29.000000 dltrain-0.1.4/src/dltrain/train.py
+-rw-rw-rw-   0        0        0     1405 2024-05-08 02:35:03.000000 dltrain-0.1.4/src/dltrain/transform.py
+-rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.1.4/src/dltrain/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:15:44.994660 dltrain-0.1.4/src/dltrain.egg-info/
+-rw-rw-rw-   0        0        0     6992 2024-06-02 07:15:44.000000 dltrain-0.1.4/src/dltrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2024-06-02 07:15:44.000000 dltrain-0.1.4/src/dltrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 07:15:44.000000 dltrain-0.1.4/src/dltrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 07:15:44.000000 dltrain-0.1.4/src/dltrain.egg-info/top_level.txt
```

### Comparing `dltrain-0.1.3/LICENSE` & `dltrain-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/PKG-INFO` & `dltrain-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -164,7 +164,9 @@
 1、加入了TaskBuilder方便构造模型
 - 0.1.2<br/>
 1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)<br/>
 2、将models.py封装到models包，添加了许多拆箱可用模型
 - 0.1.3<br/>
 1、引入错误处理机制，防止由于EventHandler设置问题导致的结果保存错误<br/>
 2、引入VectorSequenceDataset<br/>
+
+
```

### Comparing `dltrain-0.1.3/README.md` & `dltrain-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -150,7 +150,9 @@
 1、加入了TaskBuilder方便构造模型
 - 0.1.2<br/>
 1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)<br/>
 2、将models.py封装到models包，添加了许多拆箱可用模型
 - 0.1.3<br/>
 1、引入错误处理机制，防止由于EventHandler设置问题导致的结果保存错误<br/>
 2、引入VectorSequenceDataset<br/>
+
+
```

### Comparing `dltrain-0.1.3/pyproject.toml` & `dltrain-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dltrain"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="XiaosYu", email="lijingyu_ai@163.com" },
 ]
 description = "This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dltrain-0.1.3/src/dltrain/builder/base.py` & `dltrain-0.1.4/src/dltrain/builder/base.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/builder/builder.py` & `dltrain-0.1.4/src/dltrain/builder/builder.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/builder/criterion.py` & `dltrain-0.1.4/src/dltrain/builder/criterion.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/builder/dataset.py` & `dltrain-0.1.4/src/dltrain/builder/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ctypes import Union
+from typing import Union
 
 import numpy as np
 import torch
 
 from torch.utils.data import Dataset
 from ..dataset import (PyTorchNativeDataset, ImageCategoricalDataset, VectorCategoricalDataset, DLDataset,
                        VectorRegressionDataset)
```

### Comparing `dltrain-0.1.3/src/dltrain/builder/delineator.py` & `dltrain-0.1.4/src/dltrain/builder/delineator.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/builder/evaluation.py` & `dltrain-0.1.4/src/dltrain/builder/evaluation.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/builder/model.py` & `dltrain-0.1.4/src/dltrain/builder/model.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/builder/optimizer.py` & `dltrain-0.1.4/src/dltrain/builder/optimizer.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/builder/scheduler.py` & `dltrain-0.1.4/src/dltrain/builder/scheduler.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/builder/transforms.py` & `dltrain-0.1.4/src/dltrain/builder/transforms.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/checkpoint.py` & `dltrain-0.1.4/src/dltrain/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/dataset.py` & `dltrain-0.1.4/src/dltrain/dataset.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/delineator.py` & `dltrain-0.1.4/src/dltrain/delineator.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/error.py` & `dltrain-0.1.4/src/dltrain/error.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/evaluation.py` & `dltrain-0.1.4/src/dltrain/evaluation.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/forward.py` & `dltrain-0.1.4/src/dltrain/forward.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/inject.py` & `dltrain-0.1.4/src/dltrain/inject.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/models/builder.py` & `dltrain-0.1.4/src/dltrain/models/builder.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/models/component.py` & `dltrain-0.1.4/src/dltrain/models/component.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/models/model.py` & `dltrain-0.1.4/src/dltrain/models/model.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/models/wrapper.py` & `dltrain-0.1.4/src/dltrain/models/wrapper.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/options.py` & `dltrain-0.1.4/src/dltrain/options.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/train.py` & `dltrain-0.1.4/src/dltrain/train.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/transform.py` & `dltrain-0.1.4/src/dltrain/transform.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain/utils.py` & `dltrain-0.1.4/src/dltrain/utils.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.3/src/dltrain.egg-info/PKG-INFO` & `dltrain-0.1.4/src/dltrain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -164,7 +164,9 @@
 1、加入了TaskBuilder方便构造模型
 - 0.1.2<br/>
 1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)<br/>
 2、将models.py封装到models包，添加了许多拆箱可用模型
 - 0.1.3<br/>
 1、引入错误处理机制，防止由于EventHandler设置问题导致的结果保存错误<br/>
 2、引入VectorSequenceDataset<br/>
+
+
```

### Comparing `dltrain-0.1.3/src/dltrain.egg-info/SOURCES.txt` & `dltrain-0.1.4/src/dltrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

