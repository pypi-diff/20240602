# Comparing `tmp/pp_weight_estimation-1.1.41.tar.gz` & `tmp/pp_weight_estimation-1.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pp_weight_estimation-1.1.41.tar", last modified: Sat Jun  1 03:39:40 2024, max compression
+gzip compressed data, was "pp_weight_estimation-1.1.42.tar", last modified: Sat Jun  1 14:47:41 2024, max compression
```

## Comparing `pp_weight_estimation-1.1.41.tar` & `pp_weight_estimation-1.1.42.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.41/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/pp_weight_estimation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/pp_weight_estimation/core/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/core/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    11113 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/core/function_test.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     6734 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/core/get_weight.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/core/gpt_support.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1923 2024-06-01 03:39:23.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/core/s3_io.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/pp_weight_estimation/utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/utils/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1000 2024-05-23 00:53:12.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/utils/slack_connect.py
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/utils/visulizer.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-06-01 03:39:32.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/version.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-01 03:39:40.000000 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-06-01 03:39:40.000000 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-06-01 03:39:40.000000 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-06-01 03:39:40.000000 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-06-01 03:39:40.000000 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.41/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.41/scripts/weight_pred.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.41/setup.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/tests/
--rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.41/tests/test_function_test.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 14:47:41.649794 pp_weight_estimation-1.1.42/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-01 14:47:41.649794 pp_weight_estimation-1.1.42/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.42/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 14:47:41.645794 pp_weight_estimation-1.1.42/pp_weight_estimation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.42/pp_weight_estimation/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 14:47:41.645794 pp_weight_estimation-1.1.42/pp_weight_estimation/core/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.42/pp_weight_estimation/core/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    11113 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.42/pp_weight_estimation/core/function_test.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     6734 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.42/pp_weight_estimation/core/get_weight.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.42/pp_weight_estimation/core/gpt_support.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1993 2024-06-01 14:46:28.000000 pp_weight_estimation-1.1.42/pp_weight_estimation/core/s3_io.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 14:47:41.649794 pp_weight_estimation-1.1.42/pp_weight_estimation/utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.42/pp_weight_estimation/utils/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1000 2024-05-23 00:53:12.000000 pp_weight_estimation-1.1.42/pp_weight_estimation/utils/slack_connect.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.42/pp_weight_estimation/utils/visulizer.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-06-01 14:47:33.000000 pp_weight_estimation-1.1.42/pp_weight_estimation/version.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 14:47:41.649794 pp_weight_estimation-1.1.42/pp_weight_estimation.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-01 14:47:41.000000 pp_weight_estimation-1.1.42/pp_weight_estimation.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-06-01 14:47:41.000000 pp_weight_estimation-1.1.42/pp_weight_estimation.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-06-01 14:47:41.000000 pp_weight_estimation-1.1.42/pp_weight_estimation.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-06-01 14:47:41.000000 pp_weight_estimation-1.1.42/pp_weight_estimation.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-06-01 14:47:41.000000 pp_weight_estimation-1.1.42/pp_weight_estimation.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.42/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 14:47:41.645794 pp_weight_estimation-1.1.42/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.42/scripts/weight_pred.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-06-01 14:47:41.649794 pp_weight_estimation-1.1.42/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.42/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 14:47:41.649794 pp_weight_estimation-1.1.42/tests/
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.42/tests/test_function_test.py
```

### Comparing `pp_weight_estimation-1.1.41/pp_weight_estimation/core/function_test.py` & `pp_weight_estimation-1.1.42/pp_weight_estimation/core/function_test.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.41/pp_weight_estimation/core/get_weight.py` & `pp_weight_estimation-1.1.42/pp_weight_estimation/core/get_weight.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.41/pp_weight_estimation/core/gpt_support.py` & `pp_weight_estimation-1.1.42/pp_weight_estimation/core/gpt_support.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.41/pp_weight_estimation/core/s3_io.py` & `pp_weight_estimation-1.1.42/pp_weight_estimation/core/s3_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,21 +52,22 @@
     Downloads a dataframe from S3
     """
     if client is None:
         client = get_client()
     response = get_response(client, bucket, key)
     return pd.read_csv(response['Body'])
 
-def upload_image(image, bucket, key, client=None):
+def upload_image(image_path, bucket, key, client=None):
     """
-    Uploads an image to S3
+    Uploads an image/object to S3
     """
     if client is None:
         client = get_client()
-    client.put_object(Bucket=bucket, Key=key, Body=image)
+    #client.put_object(Bucket=bucket, Key=key, Body=image)
+    client.upload_file(image_path,Bucket=bucket,Key=key)
 
 def download_image(bucket, key, client=None):
     """
     Downloads an image from S3
     """
     if client is None:
         client = get_client()
```

### Comparing `pp_weight_estimation-1.1.41/pp_weight_estimation/utils/slack_connect.py` & `pp_weight_estimation-1.1.42/pp_weight_estimation/utils/slack_connect.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/SOURCES.txt` & `pp_weight_estimation-1.1.42/pp_weight_estimation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.41/setup.py` & `pp_weight_estimation-1.1.42/setup.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.41/tests/test_function_test.py` & `pp_weight_estimation-1.1.42/tests/test_function_test.py`

 * *Files identical despite different names*

