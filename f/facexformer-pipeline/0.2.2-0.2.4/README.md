# Comparing `tmp/facexformer_pipeline-0.2.2.tar.gz` & `tmp/facexformer_pipeline-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facexformer_pipeline-0.2.2.tar", last modified: Wed May 15 15:41:43 2024, max compression
+gzip compressed data, was "facexformer_pipeline-0.2.4.tar", last modified: Sun Jun  2 09:34:07 2024, max compression
```

## Comparing `facexformer_pipeline-0.2.2.tar` & `facexformer_pipeline-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:41:43.759518 facexformer_pipeline-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-15 15:41:43.759518 facexformer_pipeline-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:41:43.755518 facexformer_pipeline-0.2.2/facexformer_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/facexformer_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:41:43.755518 facexformer_pipeline-0.2.2/facexformer_pipeline/network/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:41:43.755518 facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11176 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/facexformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/task_postprocesser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/facexformer_pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:41:43.759518 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-15 15:41:43.000000 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-15 15:41:43.000000 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:41:43.000000 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 15:41:43.000000 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 15:41:43.000000 facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:41:43.759518 facexformer_pipeline-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-15 15:41:38.000000 facexformer_pipeline-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:34:07.619109 facexformer_pipeline-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-06-02 09:34:07.619109 facexformer_pipeline-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-06-02 09:34:03.000000 facexformer_pipeline-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:34:07.615109 facexformer_pipeline-0.2.4/facexformer_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 09:34:03.000000 facexformer_pipeline-0.2.4/facexformer_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-06-02 09:34:03.000000 facexformer_pipeline-0.2.4/facexformer_pipeline/facexformer_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:34:07.619109 facexformer_pipeline-0.2.4/facexformer_pipeline/network/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-02 09:34:03.000000 facexformer_pipeline-0.2.4/facexformer_pipeline/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:34:07.619109 facexformer_pipeline-0.2.4/facexformer_pipeline/network/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-02 09:34:03.000000 facexformer_pipeline-0.2.4/facexformer_pipeline/network/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11176 2024-06-02 09:34:03.000000 facexformer_pipeline-0.2.4/facexformer_pipeline/network/models/facexformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-06-02 09:34:03.000000 facexformer_pipeline-0.2.4/facexformer_pipeline/network/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-06-02 09:34:03.000000 facexformer_pipeline-0.2.4/facexformer_pipeline/task_postprocesser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-06-02 09:34:03.000000 facexformer_pipeline-0.2.4/facexformer_pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 09:34:07.619109 facexformer_pipeline-0.2.4/facexformer_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-06-02 09:34:07.000000 facexformer_pipeline-0.2.4/facexformer_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-06-02 09:34:07.000000 facexformer_pipeline-0.2.4/facexformer_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 09:34:07.000000 facexformer_pipeline-0.2.4/facexformer_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-02 09:34:07.000000 facexformer_pipeline-0.2.4/facexformer_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 09:34:07.000000 facexformer_pipeline-0.2.4/facexformer_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 09:34:07.619109 facexformer_pipeline-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-06-02 09:34:03.000000 facexformer_pipeline-0.2.4/setup.py
```

### Comparing `facexformer_pipeline-0.2.2/PKG-INFO` & `facexformer_pipeline-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facexformer_pipeline
-Version: 0.2.2
+Version: 0.2.4
 Summary: A module to run facexformer model as pipeline
 Author: Enes Kuzucu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `facexformer_pipeline-0.2.2/README.md` & `facexformer_pipeline-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `facexformer_pipeline-0.2.2/facexformer_pipeline/facexformer_pipeline.py` & `facexformer_pipeline-0.2.4/facexformer_pipeline/facexformer_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,16 +163,16 @@
 
         image = unnormalize(model_ready_image[0].detach().cpu())
         image = image.permute(1, 2, 0).numpy()
         image = (image * 255).astype(np.uint8)
         image = image[:, :, ::-1]
         results['image'] = image
         results['transformed_image'] = model_ready_image[0]
-
-        results['scaled_landmarks'] =self.scale_landmarks_to_original_image(original_image,results['landmark_list'] )
+        if 1 in self.active_tasks:
+            results['scaled_landmarks'] =self.scale_landmarks_to_original_image(original_image,results['landmark_list'] )
         return results
 
 def main():
     image_path = "sample_image.jpg"
     uih = UniversalImageInputHandler(image_path, debug=False)
     COMPATIBLE, img = uih.COMPATIBLE, uih.img
     pipeline = FacexformerPipeline(debug=False, tasks=['headpose', 'landmark', 'attributes'])
```

### Comparing `facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/facexformer.py` & `facexformer_pipeline-0.2.4/facexformer_pipeline/network/models/facexformer.py`

 * *Files identical despite different names*

### Comparing `facexformer_pipeline-0.2.2/facexformer_pipeline/network/models/transformer.py` & `facexformer_pipeline-0.2.4/facexformer_pipeline/network/models/transformer.py`

 * *Files identical despite different names*

### Comparing `facexformer_pipeline-0.2.2/facexformer_pipeline/task_postprocesser.py` & `facexformer_pipeline-0.2.4/facexformer_pipeline/task_postprocesser.py`

 * *Files identical despite different names*

### Comparing `facexformer_pipeline-0.2.2/facexformer_pipeline/utils.py` & `facexformer_pipeline-0.2.4/facexformer_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/PKG-INFO` & `facexformer_pipeline-0.2.4/facexformer_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facexformer_pipeline
-Version: 0.2.2
+Version: 0.2.4
 Summary: A module to run facexformer model as pipeline
 Author: Enes Kuzucu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `facexformer_pipeline-0.2.2/facexformer_pipeline.egg-info/SOURCES.txt` & `facexformer_pipeline-0.2.4/facexformer_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `facexformer_pipeline-0.2.2/setup.py` & `facexformer_pipeline-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 import subprocess
 import os
 
 
 setup(
     name='facexformer_pipeline',  # Package name
-    version='0.2.2',  # Version of your package
+    version='0.2.4',  # Version of your package
     author='Enes Kuzucu',  # Your name
 
     description='A module to run facexformer model as pipeline',  # Short description
     long_description=open('README.md').read(),  # Long description from a README file
     long_description_content_type='text/markdown',  # Type of the long description
 #     url='https://github.com/karaposu/image-input-handler',  # URL to the repository
     packages=find_packages(),  # Automatically find packages in the directory
```

