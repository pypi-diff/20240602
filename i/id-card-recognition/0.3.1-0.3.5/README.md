# Comparing `tmp/id_card_recognition-0.3.1.tar.gz` & `tmp/id_card_recognition-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_card_recognition-0.3.1.tar", last modified: Sat Jun  1 13:22:08 2024, max compression
+gzip compressed data, was "id_card_recognition-0.3.5.tar", last modified: Sat Jun  1 13:25:28 2024, max compression
```

## Comparing `id_card_recognition-0.3.1.tar` & `id_card_recognition-0.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:22:08.715147 id_card_recognition-0.3.1/
--rw-r--r--   0 wangligang   (501) staff       (20)     2062 2024-06-01 13:22:08.714605 id_card_recognition-0.3.1/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)     1544 2024-06-01 13:22:06.000000 id_card_recognition-0.3.1/README.md
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:22:08.710066 id_card_recognition-0.3.1/id_card_recognition/
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.3.1/id_card_recognition/__init__.py
--rw-r--r--   0 wangligang   (501) staff       (20)     5353 2024-06-01 13:22:06.000000 id_card_recognition-0.3.1/id_card_recognition/recognition.py
--rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.3.1/id_card_recognition/utils.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:22:08.713952 id_card_recognition-0.3.1/id_card_recognition.egg-info/
--rw-r--r--   0 wangligang   (501) staff       (20)     2062 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/entry_points.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/requires.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/top_level.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 13:22:08.715244 id_card_recognition-0.3.1/setup.cfg
--rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 13:22:06.000000 id_card_recognition-0.3.1/setup.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:22:08.713297 id_card_recognition-0.3.1/tests/
--rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.3.1/tests/test_recognition.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:25:28.928877 id_card_recognition-0.3.5/
+-rw-r--r--   0 wangligang   (501) staff       (20)     2062 2024-06-01 13:25:28.928456 id_card_recognition-0.3.5/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)     1544 2024-06-01 13:22:06.000000 id_card_recognition-0.3.5/README.md
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:25:28.925307 id_card_recognition-0.3.5/id_card_recognition/
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.3.5/id_card_recognition/__init__.py
+-rw-r--r--   0 wangligang   (501) staff       (20)     5355 2024-06-01 13:25:08.000000 id_card_recognition-0.3.5/id_card_recognition/recognition.py
+-rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.3.5/id_card_recognition/utils.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:25:28.927911 id_card_recognition-0.3.5/id_card_recognition.egg-info/
+-rw-r--r--   0 wangligang   (501) staff       (20)     2062 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/entry_points.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/requires.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/top_level.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 13:25:28.929003 id_card_recognition-0.3.5/setup.cfg
+-rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 13:25:26.000000 id_card_recognition-0.3.5/setup.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:25:28.927548 id_card_recognition-0.3.5/tests/
+-rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.3.5/tests/test_recognition.py
```

### Comparing `id_card_recognition-0.3.1/PKG-INFO` & `id_card_recognition-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.3.1
+Version: 0.3.5
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `id_card_recognition-0.3.1/README.md` & `id_card_recognition-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.3.1/id_card_recognition/recognition.py` & `id_card_recognition-0.3.5/id_card_recognition/recognition.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
             total_tokens += tokens_used
 
             result["recognition_time"] = f"{recognition_time:.2f} 秒"
             result["cost"] = f"¥{cost_per_image:.6f}"
             result["tokens_used"] = tokens_used
 
             results.append(result)
-            print(f"文件 {image_file} 识别完成，耗时 {recognition_time:.2f} 秒。")
+            print(f"文件 {image_file} 识别完成，耗时 {recognition_time:.2f} 秒。\n")
 
         except Exception as e:
             error_result = {
                 "file": str(image_file),
                 "result": f"处理文件时出错: {e}"
             }
             results.append(error_result)
```

### Comparing `id_card_recognition-0.3.1/id_card_recognition/utils.py` & `id_card_recognition-0.3.5/id_card_recognition/utils.py`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.3.1/id_card_recognition.egg-info/PKG-INFO` & `id_card_recognition-0.3.5/id_card_recognition.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.3.1
+Version: 0.3.5
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `id_card_recognition-0.3.1/setup.py` & `id_card_recognition-0.3.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='id_card_recognition',
-    version='0.3.1',
+    version='0.3.5',
     packages=find_packages(),
     install_requires=[
         'requests',
         'natsort',
         'openai',
         'python-dotenv',
     ],
```

