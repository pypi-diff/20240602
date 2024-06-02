# Comparing `tmp/id_card_recognition-0.3.5.tar.gz` & `tmp/id_card_recognition-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_card_recognition-0.3.5.tar", last modified: Sat Jun  1 13:25:28 2024, max compression
+gzip compressed data, was "id_card_recognition-0.3.6.tar", last modified: Sun Jun  2 00:31:04 2024, max compression
```

## Comparing `id_card_recognition-0.3.5.tar` & `id_card_recognition-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:25:28.928877 id_card_recognition-0.3.5/
--rw-r--r--   0 wangligang   (501) staff       (20)     2062 2024-06-01 13:25:28.928456 id_card_recognition-0.3.5/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)     1544 2024-06-01 13:22:06.000000 id_card_recognition-0.3.5/README.md
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:25:28.925307 id_card_recognition-0.3.5/id_card_recognition/
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.3.5/id_card_recognition/__init__.py
--rw-r--r--   0 wangligang   (501) staff       (20)     5355 2024-06-01 13:25:08.000000 id_card_recognition-0.3.5/id_card_recognition/recognition.py
--rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.3.5/id_card_recognition/utils.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:25:28.927911 id_card_recognition-0.3.5/id_card_recognition.egg-info/
--rw-r--r--   0 wangligang   (501) staff       (20)     2062 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/entry_points.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/requires.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 13:25:28.000000 id_card_recognition-0.3.5/id_card_recognition.egg-info/top_level.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 13:25:28.929003 id_card_recognition-0.3.5/setup.cfg
--rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 13:25:26.000000 id_card_recognition-0.3.5/setup.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:25:28.927548 id_card_recognition-0.3.5/tests/
--rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.3.5/tests/test_recognition.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:31:04.274351 id_card_recognition-0.3.6/
+-rw-r--r--   0 wangligang   (501) staff       (20)     2143 2024-06-02 00:31:04.273843 id_card_recognition-0.3.6/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)     1625 2024-06-02 00:30:40.000000 id_card_recognition-0.3.6/README.md
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:31:04.270181 id_card_recognition-0.3.6/id_card_recognition/
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.3.6/id_card_recognition/__init__.py
+-rw-r--r--   0 wangligang   (501) staff       (20)     5355 2024-06-01 13:25:08.000000 id_card_recognition-0.3.6/id_card_recognition/recognition.py
+-rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.3.6/id_card_recognition/utils.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:31:04.273308 id_card_recognition-0.3.6/id_card_recognition.egg-info/
+-rw-r--r--   0 wangligang   (501) staff       (20)     2143 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/entry_points.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/requires.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-02 00:31:04.000000 id_card_recognition-0.3.6/id_card_recognition.egg-info/top_level.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-02 00:31:04.274498 id_card_recognition-0.3.6/setup.cfg
+-rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-02 00:30:40.000000 id_card_recognition-0.3.6/setup.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-02 00:31:04.272816 id_card_recognition-0.3.6/tests/
+-rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.3.6/tests/test_recognition.py
```

### Comparing `id_card_recognition-0.3.5/PKG-INFO` & `id_card_recognition-0.3.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.3.5
+Version: 0.3.6
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,16 +24,16 @@
 
 ### 创建 .env 文件
 
 在项目根目录下创建一个 `.env` 文件，并添加以下内容：
 
 ```env
 API_KEY= 你的 moonshot AI 秘钥
-IMAGE_DIRECTORY= 需要识别的身份证照片存放路径，默认为 ./images
-RESULT_FILE_NAME= 识别结果文件名称，默认为 result.txt
+IMAGE_DIRECTORY= 需要识别的身份证照片存放路径，默认为 ./images，图片名称可以是'.png', '.jpg', '.jpeg', '.bmp', '.gif'
+RESULT_FILE_NAME= 识别结果文件名称，为文本文件，默认为 result.txt
 CHOSEN_MODEL_NAME= 选择的模型名称，默认为 "moonshot-v1-8k"
 ```
 
 ### 示例 .env 文件
 
 ```env
 API_KEY=sk-XXXXXXXXXXX
```

### Comparing `id_card_recognition-0.3.5/README.md` & `id_card_recognition-0.3.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 ### 创建 .env 文件
 
 在项目根目录下创建一个 `.env` 文件，并添加以下内容：
 
 ```env
 API_KEY= 你的 moonshot AI 秘钥
-IMAGE_DIRECTORY= 需要识别的身份证照片存放路径，默认为 ./images
-RESULT_FILE_NAME= 识别结果文件名称，默认为 result.txt
+IMAGE_DIRECTORY= 需要识别的身份证照片存放路径，默认为 ./images，图片名称可以是'.png', '.jpg', '.jpeg', '.bmp', '.gif'
+RESULT_FILE_NAME= 识别结果文件名称，为文本文件，默认为 result.txt
 CHOSEN_MODEL_NAME= 选择的模型名称，默认为 "moonshot-v1-8k"
 ```
 
 ### 示例 .env 文件
 
 ```env
 API_KEY=sk-XXXXXXXXXXX
```

### Comparing `id_card_recognition-0.3.5/id_card_recognition/recognition.py` & `id_card_recognition-0.3.6/id_card_recognition/recognition.py`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.3.5/id_card_recognition/utils.py` & `id_card_recognition-0.3.6/id_card_recognition/utils.py`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.3.5/id_card_recognition.egg-info/PKG-INFO` & `id_card_recognition-0.3.6/id_card_recognition.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.3.5
+Version: 0.3.6
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,16 +24,16 @@
 
 ### 创建 .env 文件
 
 在项目根目录下创建一个 `.env` 文件，并添加以下内容：
 
 ```env
 API_KEY= 你的 moonshot AI 秘钥
-IMAGE_DIRECTORY= 需要识别的身份证照片存放路径，默认为 ./images
-RESULT_FILE_NAME= 识别结果文件名称，默认为 result.txt
+IMAGE_DIRECTORY= 需要识别的身份证照片存放路径，默认为 ./images，图片名称可以是'.png', '.jpg', '.jpeg', '.bmp', '.gif'
+RESULT_FILE_NAME= 识别结果文件名称，为文本文件，默认为 result.txt
 CHOSEN_MODEL_NAME= 选择的模型名称，默认为 "moonshot-v1-8k"
 ```
 
 ### 示例 .env 文件
 
 ```env
 API_KEY=sk-XXXXXXXXXXX
```

### Comparing `id_card_recognition-0.3.5/setup.py` & `id_card_recognition-0.3.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='id_card_recognition',
-    version='0.3.5',
+    version='0.3.6',
     packages=find_packages(),
     install_requires=[
         'requests',
         'natsort',
         'openai',
         'python-dotenv',
     ],
```

