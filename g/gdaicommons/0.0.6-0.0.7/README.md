# Comparing `tmp/gdaicommons-0.0.6.tar.gz` & `tmp/gdaicommons-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdaicommons-0.0.6.tar", last modified: Thu May 30 21:08:24 2024, max compression
+gzip compressed data, was "gdaicommons-0.0.7.tar", last modified: Sun Jun  2 00:11:08 2024, max compression
```

## Comparing `gdaicommons-0.0.6.tar` & `gdaicommons-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 21:08:24.163707 gdaicommons-0.0.6/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-26 09:35:40.000000 gdaicommons-0.0.6/LICENSE
--rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-30 21:08:24.163707 gdaicommons-0.0.6/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       15 2024-05-26 09:35:40.000000 gdaicommons-0.0.6/README.md
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      737 2024-05-30 21:08:05.000000 gdaicommons-0.0.6/pyproject.toml
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-30 21:08:24.163707 gdaicommons-0.0.6/setup.cfg
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 21:08:24.159707 gdaicommons-0.0.6/src/
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 21:08:24.159707 gdaicommons-0.0.6/src/gdaicommons/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-26 17:22:49.000000 gdaicommons-0.0.6/src/gdaicommons/__init__.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       28 2024-05-30 21:06:20.000000 gdaicommons-0.0.6/src/gdaicommons/constants.py
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 21:08:24.163707 gdaicommons-0.0.6/src/gdaicommons/nlp/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-30 05:04:54.000000 gdaicommons-0.0.6/src/gdaicommons/nlp/__init__.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     2765 2024-05-30 06:01:23.000000 gdaicommons-0.0.6/src/gdaicommons/nlp/fill_mask.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     2830 2024-05-30 06:08:30.000000 gdaicommons-0.0.6/src/gdaicommons/nlp/text2text_generation.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     1839 2024-05-30 06:01:23.000000 gdaicommons-0.0.6/src/gdaicommons/nlp/text_classification.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     2930 2024-05-30 06:01:23.000000 gdaicommons-0.0.6/src/gdaicommons/nlp/text_generation.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     1831 2024-05-30 06:01:23.000000 gdaicommons-0.0.6/src/gdaicommons/nlp/text_labelling.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     2817 2024-05-30 06:01:23.000000 gdaicommons-0.0.6/src/gdaicommons/nlp/text_summarization.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     8519 2024-05-30 21:07:13.000000 gdaicommons-0.0.6/src/gdaicommons/nlp/transformations.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      495 2024-05-30 21:03:17.000000 gdaicommons-0.0.6/src/gdaicommons/utils.py
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 21:08:24.163707 gdaicommons-0.0.6/src/gdaicommons.egg-info/
--rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-30 21:08:24.000000 gdaicommons-0.0.6/src/gdaicommons.egg-info/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      600 2024-05-30 21:08:24.000000 gdaicommons-0.0.6/src/gdaicommons.egg-info/SOURCES.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-30 21:08:24.000000 gdaicommons-0.0.6/src/gdaicommons.egg-info/dependency_links.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-30 21:08:24.000000 gdaicommons-0.0.6/src/gdaicommons.egg-info/top_level.txt
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 21:08:24.163707 gdaicommons-0.0.6/tests/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      833 2024-05-30 06:03:21.000000 gdaicommons-0.0.6/tests/test_suite.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-06-02 00:11:08.208611 gdaicommons-0.0.7/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-26 09:35:40.000000 gdaicommons-0.0.7/LICENSE
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-06-02 00:11:08.208611 gdaicommons-0.0.7/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       15 2024-05-26 09:35:40.000000 gdaicommons-0.0.7/README.md
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      737 2024-06-02 00:10:27.000000 gdaicommons-0.0.7/pyproject.toml
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-06-02 00:11:08.208611 gdaicommons-0.0.7/setup.cfg
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-06-02 00:11:08.208611 gdaicommons-0.0.7/src/
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-06-02 00:11:08.208611 gdaicommons-0.0.7/src/gdaicommons/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-26 17:22:49.000000 gdaicommons-0.0.7/src/gdaicommons/__init__.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       28 2024-05-30 21:06:20.000000 gdaicommons-0.0.7/src/gdaicommons/constants.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-06-02 00:11:08.208611 gdaicommons-0.0.7/src/gdaicommons/nlp/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-30 05:04:54.000000 gdaicommons-0.0.7/src/gdaicommons/nlp/__init__.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2813 2024-06-02 00:09:20.000000 gdaicommons-0.0.7/src/gdaicommons/nlp/fill_mask.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2878 2024-06-02 00:09:20.000000 gdaicommons-0.0.7/src/gdaicommons/nlp/text2text_generation.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     1887 2024-06-02 00:09:20.000000 gdaicommons-0.0.7/src/gdaicommons/nlp/text_classification.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2978 2024-06-02 00:09:20.000000 gdaicommons-0.0.7/src/gdaicommons/nlp/text_generation.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     1879 2024-06-02 00:09:20.000000 gdaicommons-0.0.7/src/gdaicommons/nlp/text_labelling.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2865 2024-06-02 00:09:20.000000 gdaicommons-0.0.7/src/gdaicommons/nlp/text_summarization.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     8519 2024-05-30 21:07:13.000000 gdaicommons-0.0.7/src/gdaicommons/nlp/transformations.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      495 2024-05-30 21:03:17.000000 gdaicommons-0.0.7/src/gdaicommons/utils.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-06-02 00:11:08.208611 gdaicommons-0.0.7/src/gdaicommons.egg-info/
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-06-02 00:11:08.000000 gdaicommons-0.0.7/src/gdaicommons.egg-info/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      600 2024-06-02 00:11:08.000000 gdaicommons-0.0.7/src/gdaicommons.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-06-02 00:11:08.000000 gdaicommons-0.0.7/src/gdaicommons.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-06-02 00:11:08.000000 gdaicommons-0.0.7/src/gdaicommons.egg-info/top_level.txt
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-06-02 00:11:08.208611 gdaicommons-0.0.7/tests/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      833 2024-05-30 06:03:21.000000 gdaicommons-0.0.7/tests/test_suite.py
```

### Comparing `gdaicommons-0.0.6/LICENSE` & `gdaicommons-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.6/PKG-INFO` & `gdaicommons-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdaicommons
-Version: 0.0.6
+Version: 0.0.7
 Summary: AI transformation libraries and utilities to run on Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gd-ai-commons
 Project-URL: Issues, https://github.com/godelgrid/gd-ai-commons/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdaicommons-0.0.6/pyproject.toml` & `gdaicommons-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gdaicommons"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "Mayank Bhargava", email = "mbhargava.gd@gmail.com" },
 ]
 description = "AI transformation libraries and utilities to run on Godel Grid data platform"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gdaicommons-0.0.6/src/gdaicommons/nlp/fill_mask.py` & `gdaicommons-0.0.7/src/gdaicommons/nlp/fill_mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         self._pipeline = pipeline(model=self._model, device=self._gpu_device,
                                   top_k=self._top_k_scores,
                                   task='fill-mask')
 
     def transform(self, data_list: List[Dict[str, Any]]):
         indexed_inputs = self._get_indexed_inputs(data_list)
         model_inputs = [d for _, d in indexed_inputs]
+        if not model_inputs:
+            return
         if self._mask_placeholder != '[MASK]':
             model_inputs = [str(d).replace(self._mask_placeholder, '[MASK]') for d in model_inputs]
         if self._mask_targets:
             model_outputs = self._pipeline(model_inputs, targets=self._mask_targets)
         else:
             model_outputs = self._pipeline(model_inputs)
         model_outputs = normalize_model_output(model_outputs)
```

### Comparing `gdaicommons-0.0.6/src/gdaicommons/nlp/text2text_generation.py` & `gdaicommons-0.0.7/src/gdaicommons/nlp/text2text_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         self._pipeline = pipeline(model=self._model, device=self._gpu_device,
                                   task='text2text-generation',
                                   **model_kwargs)
 
     def transform(self, data_list: List[Dict[str, Any]]):
         indexed_inputs = self._get_indexed_inputs(data_list)
         model_inputs = [d for _, d in indexed_inputs]
+        if not model_inputs:
+            return
         model_outputs = self._pipeline(model_inputs)
         self._set_all_scores(data_list, indexed_inputs, model_outputs)
 
     def _get_indexed_inputs(self, data_list: List[Dict[str, Any]]) -> List[Tuple[int, str]]:
         indexed_inputs = []
         for idx, data in enumerate(data_list):
             if self._input_field in data and data[self._input_field] is not None:
```

### Comparing `gdaicommons-0.0.6/src/gdaicommons/nlp/text_classification.py` & `gdaicommons-0.0.7/src/gdaicommons/nlp/text_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         self._pipeline = pipeline(model=self._model, device=self._gpu_device,
                                   top_k=None,
                                   task='text-classification')
 
     def transform(self, data_list: List[Dict[str, Any]]):
         indexed_inputs = self._get_indexed_inputs(data_list)
         model_inputs = [d for _, d in indexed_inputs]
+        if not model_inputs:
+            return
         model_outputs = self._pipeline(model_inputs)
         model_outputs = normalize_model_output(model_outputs)
         self._set_all_scores(data_list, indexed_inputs, model_outputs)
 
     def _get_indexed_inputs(self, data_list: List[Dict[str, Any]]) -> List[Tuple[int, str]]:
         indexed_inputs = []
         for idx, data in enumerate(data_list):
```

### Comparing `gdaicommons-0.0.6/src/gdaicommons/nlp/text_generation.py` & `gdaicommons-0.0.7/src/gdaicommons/nlp/text_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
         self._pipeline = pipeline(model=self._model, device=self._gpu_device,
                                   task='text-generation',
                                   **model_kwargs)
 
     def transform(self, data_list: List[Dict[str, Any]]):
         indexed_inputs = self._get_indexed_inputs(data_list)
         model_inputs = [d for _, d in indexed_inputs]
+        if not model_inputs:
+            return
         model_outputs = self._pipeline(model_inputs)
         model_outputs = normalize_model_output(model_outputs)
         self._set_all_scores(data_list, indexed_inputs, model_outputs)
 
     def _get_indexed_inputs(self, data_list: List[Dict[str, Any]]) -> List[Tuple[int, str]]:
         indexed_inputs = []
         for idx, data in enumerate(data_list):
```

### Comparing `gdaicommons-0.0.6/src/gdaicommons/nlp/text_labelling.py` & `gdaicommons-0.0.7/src/gdaicommons/nlp/text_labelling.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         self._pipeline = pipeline(model=self._model, device=self._gpu_device,
                                   top_k=len(labels),
                                   task='zero-shot-classification')
 
     def transform(self, data_list: List[Dict[str, Any]]):
         indexed_inputs = self._get_indexed_inputs(data_list)
         model_inputs = [d for _, d in indexed_inputs]
+        if not model_inputs:
+            return
         model_outputs = self._pipeline(model_inputs, candidate_labels=self._labels)
         self._set_all_scores(data_list, indexed_inputs, model_outputs)
 
     def _get_indexed_inputs(self, data_list: List[Dict[str, Any]]) -> List[Tuple[int, str]]:
         indexed_inputs = []
         for idx, data in enumerate(data_list):
             if self._input_field in data and data[self._input_field] is not None:
```

### Comparing `gdaicommons-0.0.6/src/gdaicommons/nlp/text_summarization.py` & `gdaicommons-0.0.7/src/gdaicommons/nlp/text_summarization.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         self._pipeline = pipeline(model=self._model, device=self._gpu_device,
                                   task='summarization',
                                   **model_kwargs)
 
     def transform(self, data_list: List[Dict[str, Any]]):
         indexed_inputs = self._get_indexed_inputs(data_list)
         model_inputs = [d for _, d in indexed_inputs]
+        if not model_inputs:
+            return
         model_outputs = self._pipeline(model_inputs)
         self._set_all_scores(data_list, indexed_inputs, model_outputs)
 
     def _get_indexed_inputs(self, data_list: List[Dict[str, Any]]) -> List[Tuple[int, str]]:
         indexed_inputs = []
         for idx, data in enumerate(data_list):
             if self._input_field in data and data[self._input_field] is not None:
```

### Comparing `gdaicommons-0.0.6/src/gdaicommons/nlp/transformations.py` & `gdaicommons-0.0.7/src/gdaicommons/nlp/transformations.py`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.6/src/gdaicommons.egg-info/PKG-INFO` & `gdaicommons-0.0.7/src/gdaicommons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdaicommons
-Version: 0.0.6
+Version: 0.0.7
 Summary: AI transformation libraries and utilities to run on Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gd-ai-commons
 Project-URL: Issues, https://github.com/godelgrid/gd-ai-commons/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdaicommons-0.0.6/src/gdaicommons.egg-info/SOURCES.txt` & `gdaicommons-0.0.7/src/gdaicommons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.6/tests/test_suite.py` & `gdaicommons-0.0.7/tests/test_suite.py`

 * *Files identical despite different names*

