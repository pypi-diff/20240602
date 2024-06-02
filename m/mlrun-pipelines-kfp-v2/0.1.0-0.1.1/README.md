# Comparing `tmp/mlrun_pipelines_kfp_v2-0.1.0.tar.gz` & `tmp/mlrun_pipelines_kfp_v2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlrun_pipelines_kfp_v2-0.1.0.tar", last modified: Sun May 26 07:49:42 2024, max compression
+gzip compressed data, was "mlrun_pipelines_kfp_v2-0.1.1.tar", last modified: Sun Jun  2 06:29:37 2024, max compression
```

## Comparing `mlrun_pipelines_kfp_v2-0.1.0.tar` & `mlrun_pipelines_kfp_v2-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:42.457494 mlrun_pipelines_kfp_v2-0.1.0/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      346 2024-05-26 07:49:42.457136 mlrun_pipelines_kfp_v2-0.1.0/PKG-INFO
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       38 2024-05-26 07:49:42.457559 mlrun_pipelines_kfp_v2-0.1.0/setup.cfg
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     1325 2024-05-26 07:48:53.000000 mlrun_pipelines_kfp_v2-0.1.0/setup.py
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:42.448229 mlrun_pipelines_kfp_v2-0.1.0/src/
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:42.452005 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      871 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/helpers.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     3104 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/mixins.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     3875 2024-05-26 07:29:59.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/models.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)    10470 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/mounts.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)    12573 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/ops.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      571 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/patcher.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      829 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/utils.py
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:42.456804 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines_kfp_v2.egg-info/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      346 2024-05-26 07:49:42.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines_kfp_v2.egg-info/PKG-INFO
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      465 2024-05-26 07:49:42.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines_kfp_v2.egg-info/SOURCES.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)        1 2024-05-26 07:49:42.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines_kfp_v2.egg-info/dependency_links.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       23 2024-05-26 07:49:42.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines_kfp_v2.egg-info/requires.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       16 2024-05-26 07:49:42.000000 mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines_kfp_v2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:29:37.857076 mlrun_pipelines_kfp_v2-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-06-02 06:29:37.857076 mlrun_pipelines_kfp_v2-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 06:29:37.857076 mlrun_pipelines_kfp_v2-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-06-02 06:29:28.000000 mlrun_pipelines_kfp_v2-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:29:37.857076 mlrun_pipelines_kfp_v2-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:29:37.857076 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-06-02 06:29:28.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-06-02 06:29:28.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-06-02 06:29:28.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-06-02 06:29:28.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/mounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-06-02 06:29:28.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-06-02 06:29:28.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-06-02 06:29:28.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:29:37.857076 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines_kfp_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-06-02 06:29:37.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines_kfp_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-06-02 06:29:37.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines_kfp_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 06:29:37.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines_kfp_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 06:29:37.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines_kfp_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 06:29:37.000000 mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines_kfp_v2.egg-info/top_level.txt
```

### Comparing `mlrun_pipelines_kfp_v2-0.1.0/setup.py` & `mlrun_pipelines_kfp_v2-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import find_namespace_packages, setup
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("mlrun-kfp-setup")
 
 setup(
     name="mlrun-pipelines-kfp-v2",
-    version="0.1.0",
+    version="0.1.1",
     description="MLRun Pipelines package for providing KFP 2.* compatibility",
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
         "kfp[kubernetes]~=2.5.0",
     ],
+    long_description="MLRun Pipelines package for providing KFP 2.* compatibility",
+    long_description_content_type="text/markdown",
 )
```

### Comparing `mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/helpers.py` & `mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/helpers.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/mixins.py` & `mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/mixins.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/models.py` & `mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/models.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/mounts.py` & `mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/mounts.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/ops.py` & `mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     FUNCTION_ANNOTATION,
     PROJECT_ANNOTATION,
     RUN_ANNOTATION,
 )
 from mlrun_pipelines.common.ops import PipelineRunType
 
 import mlrun
+import mlrun.common.constants as mlrun_constants
 import mlrun.common.runtimes.constants
 from mlrun.config import config
 from mlrun.utils import get_in, logger
 
 
 def generate_kfp_dag_and_resolve_project(run, project=None):
     workflow = run.workflow_manifest()
@@ -174,22 +175,31 @@
         logger.warning(
             "Support for Pod labels is not yet available on the KFP 2 engine",
             project=function.metadata.project,
             function_name=function.metadata.name,
         )
         return
 
-    prefix = mlrun.runtimes.utils.mlrun_key
-    kfp_k8s.add_pod_label(task, prefix + "class", function.kind)
-    kfp_k8s.add_pod_label(task, prefix + "function", function.metadata.name)
-    kfp_k8s.add_pod_label(task, prefix + "name", task.name)
-    kfp_k8s.add_pod_label(task, prefix + "project", function.metadata.project)
-    kfp_k8s.add_pod_label(task, prefix + "tag", function.metadata.tag or "latest")
     kfp_k8s.add_pod_label(
-        task, prefix + "scrape-metrics", "True" if scrape_metrics else "False"
+        task, mlrun_constants.MLRunInternalLabels.mlrun_class, function.kind
+    )
+    kfp_k8s.add_pod_label(
+        task, mlrun_constants.MLRunInternalLabels.function, function.metadata.name
+    )
+    kfp_k8s.add_pod_label(task, mlrun_constants.MLRunInternalLabels.name, task.name)
+    kfp_k8s.add_pod_label(
+        task, mlrun_constants.MLRunInternalLabels.project, function.metadata.project
+    )
+    kfp_k8s.add_pod_label(
+        task, mlrun_constants.MLRunInternalLabels.tag, function.metadata.tag or "latest"
+    )
+    kfp_k8s.add_pod_label(
+        task,
+        mlrun_constants.MLRunInternalLabels.scrape_metrics,
+        "True" if scrape_metrics else "False",
     )
 
 
 def add_default_env(task):
     if hasattr(kfp_k8s, "use_field_path_as_env"):
         kfp_k8s.use_field_path_as_env(task, "MLRUN_NAMESPACE", "metadata.namespace")
     else:
```

### Comparing `mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/patcher.py` & `mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/patcher.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_v2-0.1.0/src/mlrun_pipelines/utils.py` & `mlrun_pipelines_kfp_v2-0.1.1/src/mlrun_pipelines/utils.py`

 * *Files identical despite different names*

