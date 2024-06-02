# Comparing `tmp/mlrun_pipelines_kfp_common-0.1.0.tar.gz` & `tmp/mlrun_pipelines_kfp_common-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlrun_pipelines_kfp_common-0.1.0.tar", last modified: Sun May 26 07:49:12 2024, max compression
+gzip compressed data, was "mlrun_pipelines_kfp_common-0.1.1.tar", last modified: Sun Jun  2 06:29:33 2024, max compression
```

## Comparing `mlrun_pipelines_kfp_common-0.1.0.tar` & `mlrun_pipelines_kfp_common-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:12.746271 mlrun_pipelines_kfp_common-0.1.0/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      312 2024-05-26 07:49:12.745829 mlrun_pipelines_kfp_common-0.1.0/PKG-INFO
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       38 2024-05-26 07:49:12.746327 mlrun_pipelines_kfp_common-0.1.0/setup.cfg
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     1272 2024-05-26 07:48:53.000000 mlrun_pipelines_kfp_common-0.1.0/setup.py
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:12.736978 mlrun_pipelines_kfp_common-0.1.0/src/
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:12.736755 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:12.739193 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/common/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      571 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/common/__init__.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     4507 2024-05-26 07:29:59.000000 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/common/helpers.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     3523 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/common/models.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)     1747 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/common/mounts.py
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)    22762 2024-05-26 07:29:53.000000 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/common/ops.py
-drwxr-xr-x   0 Liran_Ben_Gida   (502) staff       (20)        0 2024-05-26 07:49:12.745489 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines_kfp_common.egg-info/
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      312 2024-05-26 07:49:12.000000 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines_kfp_common.egg-info/PKG-INFO
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)      409 2024-05-26 07:49:12.000000 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines_kfp_common.egg-info/SOURCES.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)        1 2024-05-26 07:49:12.000000 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines_kfp_common.egg-info/dependency_links.txt
--rw-r--r--   0 Liran_Ben_Gida   (502) staff       (20)       16 2024-05-26 07:49:12.000000 mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines_kfp_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:29:33.673259 mlrun_pipelines_kfp_common-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-02 06:29:33.673259 mlrun_pipelines_kfp_common-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 06:29:33.673259 mlrun_pipelines_kfp_common-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-06-02 06:29:26.000000 mlrun_pipelines_kfp_common-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:29:33.669259 mlrun_pipelines_kfp_common-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:29:33.669259 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:29:33.669259 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-06-02 06:29:26.000000 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-06-02 06:29:26.000000 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-06-02 06:29:26.000000 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-06-02 06:29:26.000000 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/common/mounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22988 2024-06-02 06:29:26.000000 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/common/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:29:33.673259 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines_kfp_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-02 06:29:33.000000 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines_kfp_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-06-02 06:29:33.000000 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines_kfp_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 06:29:33.000000 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines_kfp_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 06:29:33.000000 mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines_kfp_common.egg-info/top_level.txt
```

### Comparing `mlrun_pipelines_kfp_common-0.1.0/setup.py` & `mlrun_pipelines_kfp_common-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from setuptools import find_namespace_packages, setup
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("mlrun-kfp-setup")
 
 setup(
     name="mlrun-pipelines-kfp-common",
-    version="0.1.0",
-    description="MLRun Pipelines package for providing KFP 1.8 compatibility",
+    version="0.1.1",
+    description="MLRun Pipelines package for providing KFP common functionality",
     author="Yaron Haviv",
     author_email="yaronh@iguazio.com",
     license="Apache License 2.0",
     url="https://github.com/mlrun/mlrun",
     packages=find_namespace_packages(
         where="src/",
         include=[
@@ -35,8 +35,10 @@
     ),
     package_dir={"": "src"},
     keywords=[
         "mlrun",
         "kfp",
     ],
     python_requires=">=3.9, <3.12",
+    long_description="MLRun Pipelines package for providing KFP common functionality",
+    long_description_content_type="text/markdown",
 )
```

### Comparing `mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/common/__init__.py` & `mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/common/helpers.py` & `mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/common/helpers.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/common/models.py` & `mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/common/models.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/common/mounts.py` & `mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/common/mounts.py`

 * *Files identical despite different names*

### Comparing `mlrun_pipelines_kfp_common-0.1.0/src/mlrun_pipelines/common/ops.py` & `mlrun_pipelines_kfp_common-0.1.1/src/mlrun_pipelines/common/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import os
 from copy import deepcopy
 from typing import Union
 
 import mlrun_pipelines.common.models
 
 import mlrun
+import mlrun.common.constants
 from mlrun.config import config
 from mlrun.errors import err_to_str
 from mlrun.model import HyperParamOptions, RunSpec
 from mlrun.utils import (
     dict_to_yaml,
     gen_md_table,
     get_artifact_target,
@@ -456,15 +457,22 @@
     if not run_db:
         run_db = mlrun.db.get_run_db()
 
     # enrich DAG with mlrun run info
     runs = run_db.list_runs(project=project, labels=f"workflow={run_id}")
 
     for run in runs:
-        step = get_in(run, ["metadata", "labels", "mlrun/runner-pod"])
+        step = get_in(
+            run,
+            [
+                "metadata",
+                "labels",
+                mlrun.common.constants.MLRunInternalLabels.runner_pod,
+            ],
+        )
         if step and step in dag:
             dag[step]["run_uid"] = get_in(run, "metadata.uid")
             dag[step]["kind"] = get_in(run, "metadata.labels.kind")
             error = get_in(run, "status.error")
             if error:
                 dag[step]["error"] = error
 
@@ -610,15 +618,17 @@
         target = output_spec.get("inline", target)
 
         out_dict[key] = get_artifact_target(output, project=project)
 
         if target.startswith("v3io:///"):
             target = target.replace("v3io:///", "http://v3io-webapi:8081/")
 
-        user = labels.get("v3io_user", "") or os.environ.get("V3IO_USERNAME", "")
+        user = labels.get(
+            mlrun.common.constants.MLRunInternalLabels.v3io_user, ""
+        ) or os.environ.get("V3IO_USERNAME", "")
         if target.startswith("/User/"):
             user = user or "admin"
             target = "http://v3io-webapi:8081/users/" + user + target[5:]
 
         viewer = output_spec.get("viewer", "")
         if viewer in ["web-app", "chart"]:
             meta = {"type": "web-app", "source": target}
```

