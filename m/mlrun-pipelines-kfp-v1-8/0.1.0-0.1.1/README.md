# Comparing `tmp/mlrun_pipelines_kfp_v1_8-0.1.0.tar.gz` & `tmp/mlrun_pipelines_kfp_v1_8-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlrun_pipelines_kfp_v1_8-0.1.0.tar", last modified: Sun May 26 07:49:27 2024, max compression
+gzip compressed data, was "mlrun_pipelines_kfp_v1_8-0.1.1.tar", last modified: Sun Jun  2 06:30:01 2024, max compression
```

## Comparing `mlrun_pipelines_kfp_v1_8-0.1.0.tar` & `mlrun_pipelines_kfp_v1_8-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:27.913085 mlrun_pipelines_kfp_v1_8-0.1.0/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      334 2024-05-26 07:49:27.912539 mlrun_pipelines_kfp_v1_8-0.1.0/PKG-INFO
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       38 2024-05-26 07:49:27.913148 mlrun_pipelines_kfp_v1_8-0.1.0/setup.cfg
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     1313 2024-05-26 07:48:53.000000 mlrun_pipelines_kfp_v1_8-0.1.0/setup.py
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:27.904428 mlrun_pipelines_kfp_v1_8-0.1.0/src/
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:27.907260 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     1396 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/helpers.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     3959 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/mixins.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     5881 2024-05-26 07:29:59.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/models.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)    17761 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/mounts.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     9361 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/ops.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     4368 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/patcher.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     2463 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/utils.py
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:27.912223 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines_kfp_v1_8.egg-info/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      334 2024-05-26 07:49:27.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines_kfp_v1_8.egg-info/PKG-INFO
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      475 2024-05-26 07:49:27.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines_kfp_v1_8.egg-info/SOURCES.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)        1 2024-05-26 07:49:27.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines_kfp_v1_8.egg-info/dependency_links.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)        9 2024-05-26 07:49:27.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines_kfp_v1_8.egg-info/requires.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       16 2024-05-26 07:49:27.000000 mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines_kfp_v1_8.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:30:01.217132 mlrun_pipelines_kfp_v1_8-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-06-02 06:30:01.217132 mlrun_pipelines_kfp_v1_8-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 06:30:01.217132 mlrun_pipelines_kfp_v1_8-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-06-02 06:29:55.000000 mlrun_pipelines_kfp_v1_8-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:30:01.213132 mlrun_pipelines_kfp_v1_8-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:30:01.217132 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-06-02 06:29:55.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-06-02 06:29:55.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-06-02 06:29:55.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-06-02 06:29:55.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/mounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-06-02 06:29:55.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-06-02 06:29:55.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-06-02 06:29:55.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:30:01.217132 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines_kfp_v1_8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-06-02 06:30:01.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines_kfp_v1_8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-06-02 06:30:01.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines_kfp_v1_8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 06:30:01.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines_kfp_v1_8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 06:30:01.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines_kfp_v1_8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 06:30:01.000000 mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines_kfp_v1_8.egg-info/top_level.txt
```

### Comparing `mlrun_pipelines_kfp_v1_8-0.1.0/setup.py` & `mlrun_pipelines_kfp_v1_8-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import find_namespace_packages, setup
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("mlrun-kfp-setup")
 
 setup(
     name="mlrun-pipelines-kfp-v1-8",
-    version="0.1.0",
+    version="0.1.1",
     description="MLRun Pipelines package for providing KFP 1.8 compatibility",
     author="Yaron Haviv",
     author_email="yaronh@iguazio.com",
     license="Apache License 2.0",
     url="https://github.com/mlrun/mlrun",
     packages=find_namespace_packages(
         where="src/",
@@ -38,8 +38,10 @@
         "mlrun",
         "kfp",
     ],
     python_requires=">=3.9, <3.12",
     install_requires=[
         "kfp~=1.8",
     ],
+    long_description="MLRun Pipelines package for providing KFP 1.8 compatibility",
+    long_description_content_type="text/markdown",
 )
```

### Comparing `mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/helpers.py` & `mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/helpers.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/mixins.py` & `mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/mixins.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/models.py` & `mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/models.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/mounts.py` & `mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/mounts.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/ops.py` & `mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/ops.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     FUNCTION_ANNOTATION,
     PROJECT_ANNOTATION,
     RUN_ANNOTATION,
 )
 from mlrun_pipelines.common.ops import KFPMETA_DIR, PipelineRunType
 
 import mlrun
+import mlrun.common.constants as mlrun_constants
 import mlrun.common.runtimes.constants
 from mlrun.config import config
 from mlrun.utils import get_in
 
 # Disable the warning about reusing components
 dsl.ContainerOp._DISABLE_REUSABLE_COMPONENT_WARNING = True
 
@@ -205,21 +206,29 @@
         func_url = func_url[len("db://") :]
     cop.add_pod_annotation(RUN_ANNOTATION, kind)
     cop.add_pod_annotation(PROJECT_ANNOTATION, project or function.metadata.project)
     cop.add_pod_annotation(FUNCTION_ANNOTATION, func_url or function.uri)
 
 
 def add_labels(cop, function, scrape_metrics=False):
-    prefix = mlrun.runtimes.utils.mlrun_key
-    cop.add_pod_label(prefix + "class", function.kind)
-    cop.add_pod_label(prefix + "function", function.metadata.name)
-    cop.add_pod_label(prefix + "name", cop.human_name)
-    cop.add_pod_label(prefix + "project", function.metadata.project)
-    cop.add_pod_label(prefix + "tag", function.metadata.tag or "latest")
-    cop.add_pod_label(prefix + "scrape-metrics", "True" if scrape_metrics else "False")
+    cop.add_pod_label(mlrun_constants.MLRunInternalLabels.mlrun_class, function.kind)
+    cop.add_pod_label(
+        mlrun_constants.MLRunInternalLabels.function, function.metadata.name
+    )
+    cop.add_pod_label(mlrun_constants.MLRunInternalLabels.name, cop.human_name)
+    cop.add_pod_label(
+        mlrun_constants.MLRunInternalLabels.project, function.metadata.project
+    )
+    cop.add_pod_label(
+        mlrun_constants.MLRunInternalLabels.tag, function.metadata.tag or "latest"
+    )
+    cop.add_pod_label(
+        mlrun_constants.MLRunInternalLabels.scrape_metrics,
+        "True" if scrape_metrics else "False",
+    )
 
 
 def add_default_function_resources(
     container_op: dsl.ContainerOp,
 ) -> dsl.ContainerOp:
     default_resources = config.get_default_function_pod_resources()
     for resource_name, resource_value in default_resources["requests"].items():
```

### Comparing `mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/patcher.py` & `mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/patcher.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_v1_8-0.1.0/src/mlrun_pipelines/utils.py` & `mlrun_pipelines_kfp_v1_8-0.1.1/src/mlrun_pipelines/utils.py`

 * *Files identical despite different names*

