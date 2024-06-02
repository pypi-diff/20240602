# Comparing `tmp/sklearntools-1.0.0.tar.gz` & `tmp/sklearntools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearntools-1.0.0.tar", last modified: Mon May 27 06:48:52 2024, max compression
+gzip compressed data, was "sklearntools-1.0.1.tar", last modified: Sun Jun  2 12:42:33 2024, max compression
```

## Comparing `sklearntools-1.0.0.tar` & `sklearntools-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 06:48:52.302112 sklearntools-1.0.0/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-27 06:48:52.301410 sklearntools-1.0.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-1.0.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-27 06:48:52.302395 sklearntools-1.0.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-27 06:48:45.000000 sklearntools-1.0.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 06:48:52.295793 sklearntools-1.0.0/sklearntools/
--rw-r--r--   0 summy      (501) staff       (20)     9936 2024-05-27 06:43:17.000000 sklearntools-1.0.0/sklearntools/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-27 06:48:52.300282 sklearntools-1.0.0/sklearntools.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-27 06:48:52.000000 sklearntools-1.0.0/sklearntools.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-27 06:48:52.000000 sklearntools-1.0.0/sklearntools.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 06:48:52.000000 sklearntools-1.0.0/sklearntools.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-27 06:48:52.000000 sklearntools-1.0.0/sklearntools.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-27 06:48:52.000000 sklearntools-1.0.0/sklearntools.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-27 06:48:52.000000 sklearntools-1.0.0/sklearntools.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-02 12:42:33.769450 sklearntools-1.0.1/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-06-02 12:42:33.768933 sklearntools-1.0.1/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-1.0.1/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-06-02 12:42:33.769763 sklearntools-1.0.1/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      882 2024-06-02 12:42:31.000000 sklearntools-1.0.1/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-02 12:42:33.758514 sklearntools-1.0.1/sklearntools/
+-rw-r--r--   0 summy      (501) staff       (20)     9930 2024-06-02 12:42:04.000000 sklearntools-1.0.1/sklearntools/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-06-02 12:42:33.768120 sklearntools-1.0.1/sklearntools.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-06-02 12:42:33.000000 sklearntools-1.0.1/sklearntools.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      258 2024-06-02 12:42:33.000000 sklearntools-1.0.1/sklearntools.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-02 12:42:33.000000 sklearntools-1.0.1/sklearntools.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-06-02 12:42:11.000000 sklearntools-1.0.1/sklearntools.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       32 2024-06-02 12:42:33.000000 sklearntools-1.0.1/sklearntools.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)       13 2024-06-02 12:42:33.000000 sklearntools-1.0.1/sklearntools.egg-info/top_level.txt
```

### Comparing `sklearntools-1.0.0/PKG-INFO` & `sklearntools-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

### Comparing `sklearntools-1.0.0/README.rst` & `sklearntools-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `sklearntools-1.0.0/setup.py` & `sklearntools-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='sklearntools',
     packages=['sklearntools'],
     description="Tools of sklearn.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.0',
+    version='1.0.1',
     install_requires=[
         'joblib>=1.1.0',
         'scikit-learn>=1.0',
     ],
     url='https://gitee.com/summry/sklearntools',
     author='summy',
     author_email='xiazhongbiao@126.com',
```

### Comparing `sklearntools-1.0.0/sklearntools/__init__.py` & `sklearntools-1.0.1/sklearntools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 	return params, score
 
 
 def _evaluate_params(model_name, classifier, X_train, X_test, y_train, y_test, param, iter_num):
 	results = Parallel(n_jobs=-1)(
 		delayed(_search_params)(model_name, classifier, X_train, X_test, y_train, y_test, param) for _ in range(iter_num))
 	counter = Counter([result[1] for result in results])
-	for score, count in sorted(counter.items(), key=lambda x: x[0], reverse=classifier):
+	for score, count in sorted(counter.items(), key=lambda x: x[0], reverse=True):
 		if classifier:
 			logger.info(f'\tscore: {score:.1%}\tcount: {count}')
 		else:
 			logger.info(f'\tscore: {score:.4f}\tcount: {count}')
 
 
 def multi_round_evaluate(X: np.ndarray, y: np.ndarray, *models, **kwargs):
```

### Comparing `sklearntools-1.0.0/sklearntools.egg-info/PKG-INFO` & `sklearntools-1.0.1/sklearntools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

