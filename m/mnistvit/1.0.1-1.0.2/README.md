# Comparing `tmp/mnistvit-1.0.1.tar.gz` & `tmp/mnistvit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnistvit-1.0.1.tar", last modified: Mon May 20 22:24:13 2024, max compression
+gzip compressed data, was "mnistvit-1.0.2.tar", last modified: Sun Jun  2 10:14:16 2024, max compression
```

## Comparing `mnistvit-1.0.1.tar` & `mnistvit-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-20 22:24:13.124329 mnistvit-1.0.1/
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)    35149 2024-02-19 12:26:31.000000 mnistvit-1.0.1/LICENSE
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)    42823 2024-05-20 22:24:13.124329 mnistvit-1.0.1/PKG-INFO
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     1376 2024-05-20 21:08:59.000000 mnistvit-1.0.1/README.md
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)      962 2024-05-20 22:22:44.000000 mnistvit-1.0.1/pyproject.toml
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       38 2024-05-20 22:24:13.124329 mnistvit-1.0.1/setup.cfg
-drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-20 22:24:13.120329 mnistvit-1.0.1/src/
-drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-20 22:24:13.124329 mnistvit-1.0.1/src/mnistvit/
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)      187 2024-05-20 21:07:20.000000 mnistvit-1.0.1/src/mnistvit/__init__.py
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       34 2024-05-20 21:08:56.000000 mnistvit-1.0.1/src/mnistvit/__main__.py
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     7629 2024-05-20 21:09:01.000000 mnistvit-1.0.1/src/mnistvit/model.py
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     7297 2024-05-20 21:09:01.000000 mnistvit-1.0.1/src/mnistvit/predict.py
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     4247 2024-05-20 21:09:01.000000 mnistvit-1.0.1/src/mnistvit/preprocess.py
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)    11772 2024-05-20 21:09:01.000000 mnistvit-1.0.1/src/mnistvit/train.py
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     8182 2024-05-20 21:09:01.000000 mnistvit-1.0.1/src/mnistvit/tune.py
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     1283 2024-05-20 21:08:52.000000 mnistvit-1.0.1/src/mnistvit/utils.py
-drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-20 22:24:13.124329 mnistvit-1.0.1/src/mnistvit.egg-info/
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)    42823 2024-05-20 22:24:13.000000 mnistvit-1.0.1/src/mnistvit.egg-info/PKG-INFO
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)      399 2024-05-20 22:24:13.000000 mnistvit-1.0.1/src/mnistvit.egg-info/SOURCES.txt
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)        1 2024-05-20 22:24:13.000000 mnistvit-1.0.1/src/mnistvit.egg-info/dependency_links.txt
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       43 2024-05-20 22:24:13.000000 mnistvit-1.0.1/src/mnistvit.egg-info/requires.txt
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)        9 2024-05-20 22:24:13.000000 mnistvit-1.0.1/src/mnistvit.egg-info/top_level.txt
+drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-06-02 10:14:16.898667 mnistvit-1.0.2/
+-rw-r--r--   0 asnelt    (1000) asnelt    (1000)    35149 2024-02-19 12:26:31.000000 mnistvit-1.0.2/LICENSE
+-rw-r--r--   0 asnelt    (1000) asnelt    (1000)    42824 2024-06-02 10:14:16.898667 mnistvit-1.0.2/PKG-INFO
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     1377 2024-06-02 08:32:29.000000 mnistvit-1.0.2/README.md
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)      962 2024-06-02 09:50:57.000000 mnistvit-1.0.2/pyproject.toml
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       38 2024-06-02 10:14:16.898667 mnistvit-1.0.2/setup.cfg
+drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-06-02 10:14:16.894667 mnistvit-1.0.2/src/
+drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-06-02 10:14:16.898667 mnistvit-1.0.2/src/mnistvit/
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)      187 2024-05-20 21:07:20.000000 mnistvit-1.0.2/src/mnistvit/__init__.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       34 2024-05-20 21:08:56.000000 mnistvit-1.0.2/src/mnistvit/__main__.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     7629 2024-05-20 21:09:01.000000 mnistvit-1.0.2/src/mnistvit/model.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     7297 2024-05-20 21:09:01.000000 mnistvit-1.0.2/src/mnistvit/predict.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     4247 2024-05-20 21:09:01.000000 mnistvit-1.0.2/src/mnistvit/preprocess.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)    11772 2024-05-20 21:09:01.000000 mnistvit-1.0.2/src/mnistvit/train.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     8182 2024-05-20 21:09:01.000000 mnistvit-1.0.2/src/mnistvit/tune.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     1283 2024-05-20 21:08:52.000000 mnistvit-1.0.2/src/mnistvit/utils.py
+drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-06-02 10:14:16.898667 mnistvit-1.0.2/src/mnistvit.egg-info/
+-rw-r--r--   0 asnelt    (1000) asnelt    (1000)    42824 2024-06-02 10:14:16.000000 mnistvit-1.0.2/src/mnistvit.egg-info/PKG-INFO
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)      399 2024-06-02 10:14:16.000000 mnistvit-1.0.2/src/mnistvit.egg-info/SOURCES.txt
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)        1 2024-06-02 10:14:16.000000 mnistvit-1.0.2/src/mnistvit.egg-info/dependency_links.txt
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       43 2024-06-02 10:14:16.000000 mnistvit-1.0.2/src/mnistvit.egg-info/requires.txt
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)        9 2024-06-02 10:14:16.000000 mnistvit-1.0.2/src/mnistvit.egg-info/top_level.txt
```

### Comparing `mnistvit-1.0.1/LICENSE` & `mnistvit-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mnistvit-1.0.1/PKG-INFO` & `mnistvit-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnistvit
-Version: 1.0.1
+Version: 1.0.2
 Summary: A vision transformer for training on MNIST
 Author-email: Arno Onken <asnelt@asnelt.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -727,15 +727,15 @@
 ```
 python -m mnistvit.train
 ```
 
 The script will produce a file `model.pt` containing the trained model.  Use the `-h`
 argument for a list of options.
 
-To evaluate the test set accuracy of the model stored in`model.pt`:
+To evaluate the test set accuracy of the model stored in `model.pt`:
 ```
 python -m mnistvit.predict --use-accuracy
 ```
 
 To predict the class of the digit stored in the file `sample.jpg`:
 ```
 python -m mnistvit.predict --image-file sample.jpg
```

### Comparing `mnistvit-1.0.1/README.md` & `mnistvit-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ```
 python -m mnistvit.train
 ```
 
 The script will produce a file `model.pt` containing the trained model.  Use the `-h`
 argument for a list of options.
 
-To evaluate the test set accuracy of the model stored in`model.pt`:
+To evaluate the test set accuracy of the model stored in `model.pt`:
 ```
 python -m mnistvit.predict --use-accuracy
 ```
 
 To predict the class of the digit stored in the file `sample.jpg`:
 ```
 python -m mnistvit.predict --image-file sample.jpg
```

### Comparing `mnistvit-1.0.1/pyproject.toml` & `mnistvit-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mnistvit"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{name = "Arno Onken", email = "asnelt@asnelt.org"}]
 description = "A vision transformer for training on MNIST"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.10"
 dependencies = [
     "torch",
```

### Comparing `mnistvit-1.0.1/src/mnistvit/model.py` & `mnistvit-1.0.2/src/mnistvit/model.py`

 * *Files identical despite different names*

### Comparing `mnistvit-1.0.1/src/mnistvit/predict.py` & `mnistvit-1.0.2/src/mnistvit/predict.py`

 * *Files identical despite different names*

### Comparing `mnistvit-1.0.1/src/mnistvit/preprocess.py` & `mnistvit-1.0.2/src/mnistvit/preprocess.py`

 * *Files identical despite different names*

### Comparing `mnistvit-1.0.1/src/mnistvit/train.py` & `mnistvit-1.0.2/src/mnistvit/train.py`

 * *Files identical despite different names*

### Comparing `mnistvit-1.0.1/src/mnistvit/tune.py` & `mnistvit-1.0.2/src/mnistvit/tune.py`

 * *Files identical despite different names*

### Comparing `mnistvit-1.0.1/src/mnistvit/utils.py` & `mnistvit-1.0.2/src/mnistvit/utils.py`

 * *Files identical despite different names*

### Comparing `mnistvit-1.0.1/src/mnistvit.egg-info/PKG-INFO` & `mnistvit-1.0.2/src/mnistvit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnistvit
-Version: 1.0.1
+Version: 1.0.2
 Summary: A vision transformer for training on MNIST
 Author-email: Arno Onken <asnelt@asnelt.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -727,15 +727,15 @@
 ```
 python -m mnistvit.train
 ```
 
 The script will produce a file `model.pt` containing the trained model.  Use the `-h`
 argument for a list of options.
 
-To evaluate the test set accuracy of the model stored in`model.pt`:
+To evaluate the test set accuracy of the model stored in `model.pt`:
 ```
 python -m mnistvit.predict --use-accuracy
 ```
 
 To predict the class of the digit stored in the file `sample.jpg`:
 ```
 python -m mnistvit.predict --image-file sample.jpg
```

