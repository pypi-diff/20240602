# Comparing `tmp/fastapi-mongo-0.0.3.tar.gz` & `tmp/fastapi-mongo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-mongo-0.0.3.tar", last modified: Sun Jun  2 06:17:55 2024, max compression
+gzip compressed data, was "fastapi-mongo-0.0.4.tar", last modified: Sun Jun  2 06:23:33 2024, max compression
```

## Comparing `fastapi-mongo-0.0.3.tar` & `fastapi-mongo-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 anurag    (1000) anurag    (1000)        0 2024-06-02 06:17:55.679568 fastapi-mongo-0.0.3/
--rw-rw-r--   0 anurag    (1000) anurag    (1000)     1071 2024-06-01 08:10:44.000000 fastapi-mongo-0.0.3/LICENSE
--rw-rw-r--   0 anurag    (1000) anurag    (1000)      621 2024-06-02 06:17:55.678568 fastapi-mongo-0.0.3/PKG-INFO
-drwxrwxr-x   0 anurag    (1000) anurag    (1000)        0 2024-06-02 06:17:55.678568 fastapi-mongo-0.0.3/fastapi_mongo.egg-info/
--rw-rw-r--   0 anurag    (1000) anurag    (1000)      621 2024-06-02 06:17:55.000000 fastapi-mongo-0.0.3/fastapi_mongo.egg-info/PKG-INFO
--rw-rw-r--   0 anurag    (1000) anurag    (1000)      340 2024-06-02 06:17:55.000000 fastapi-mongo-0.0.3/fastapi_mongo.egg-info/SOURCES.txt
--rw-rw-r--   0 anurag    (1000) anurag    (1000)        1 2024-06-02 06:17:55.000000 fastapi-mongo-0.0.3/fastapi_mongo.egg-info/dependency_links.txt
--rw-rw-r--   0 anurag    (1000) anurag    (1000)       82 2024-06-02 06:17:55.000000 fastapi-mongo-0.0.3/fastapi_mongo.egg-info/entry_points.txt
--rw-rw-r--   0 anurag    (1000) anurag    (1000)       75 2024-06-02 06:17:55.000000 fastapi-mongo-0.0.3/fastapi_mongo.egg-info/requires.txt
--rw-rw-r--   0 anurag    (1000) anurag    (1000)        8 2024-06-02 06:17:55.000000 fastapi-mongo-0.0.3/fastapi_mongo.egg-info/top_level.txt
-drwxrwxr-x   0 anurag    (1000) anurag    (1000)        0 2024-06-02 06:17:55.678568 fastapi-mongo-0.0.3/package/
--rw-rw-r--   0 anurag    (1000) anurag    (1000)        0 2024-06-02 05:32:16.000000 fastapi-mongo-0.0.3/package/__init__.py
--rw-rw-r--   0 anurag    (1000) anurag    (1000)      673 2024-06-02 03:52:22.000000 fastapi-mongo-0.0.3/package/build_structure.py
--rw-rw-r--   0 anurag    (1000) anurag    (1000)     1168 2024-06-02 05:34:11.000000 fastapi-mongo-0.0.3/package/create_json.py
--rw-rw-r--   0 anurag    (1000) anurag    (1000)    15734 2024-06-02 05:44:27.000000 fastapi-mongo-0.0.3/package/folder_structure.json
--rw-rw-r--   0 anurag    (1000) anurag    (1000)       38 2024-06-02 06:17:55.679568 fastapi-mongo-0.0.3/setup.cfg
--rw-rw-r--   0 anurag    (1000) anurag    (1000)     1102 2024-06-02 06:17:33.000000 fastapi-mongo-0.0.3/setup.py
+drwxrwxr-x   0 anurag    (1000) anurag    (1000)        0 2024-06-02 06:23:33.294825 fastapi-mongo-0.0.4/
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)     1071 2024-06-01 08:10:44.000000 fastapi-mongo-0.0.4/LICENSE
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)      621 2024-06-02 06:23:33.294825 fastapi-mongo-0.0.4/PKG-INFO
+drwxrwxr-x   0 anurag    (1000) anurag    (1000)        0 2024-06-02 06:23:33.293825 fastapi-mongo-0.0.4/fastapi_mongo.egg-info/
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)      621 2024-06-02 06:23:33.000000 fastapi-mongo-0.0.4/fastapi_mongo.egg-info/PKG-INFO
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)      340 2024-06-02 06:23:33.000000 fastapi-mongo-0.0.4/fastapi_mongo.egg-info/SOURCES.txt
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)        1 2024-06-02 06:23:33.000000 fastapi-mongo-0.0.4/fastapi_mongo.egg-info/dependency_links.txt
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)       82 2024-06-02 06:23:33.000000 fastapi-mongo-0.0.4/fastapi_mongo.egg-info/entry_points.txt
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)       86 2024-06-02 06:23:33.000000 fastapi-mongo-0.0.4/fastapi_mongo.egg-info/requires.txt
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)        8 2024-06-02 06:23:33.000000 fastapi-mongo-0.0.4/fastapi_mongo.egg-info/top_level.txt
+drwxrwxr-x   0 anurag    (1000) anurag    (1000)        0 2024-06-02 06:23:33.294825 fastapi-mongo-0.0.4/package/
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)        0 2024-06-02 05:32:16.000000 fastapi-mongo-0.0.4/package/__init__.py
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)      673 2024-06-02 03:52:22.000000 fastapi-mongo-0.0.4/package/build_structure.py
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)     1168 2024-06-02 05:34:11.000000 fastapi-mongo-0.0.4/package/create_json.py
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)    15734 2024-06-02 05:44:27.000000 fastapi-mongo-0.0.4/package/folder_structure.json
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)       38 2024-06-02 06:23:33.294825 fastapi-mongo-0.0.4/setup.cfg
+-rw-rw-r--   0 anurag    (1000) anurag    (1000)     1117 2024-06-02 06:23:25.000000 fastapi-mongo-0.0.4/setup.py
```

### Comparing `fastapi-mongo-0.0.3/LICENSE` & `fastapi-mongo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-mongo-0.0.3/PKG-INFO` & `fastapi-mongo-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mongo
-Version: 0.0.3
+Version: 0.0.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fastapi-mongo-0.0.3/fastapi_mongo.egg-info/PKG-INFO` & `fastapi-mongo-0.0.4/fastapi_mongo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mongo
-Version: 0.0.3
+Version: 0.0.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fastapi-mongo-0.0.3/package/build_structure.py` & `fastapi-mongo-0.0.4/package/build_structure.py`

 * *Files identical despite different names*

### Comparing `fastapi-mongo-0.0.3/package/create_json.py` & `fastapi-mongo-0.0.4/package/create_json.py`

 * *Files identical despite different names*

### Comparing `fastapi-mongo-0.0.3/package/folder_structure.json` & `fastapi-mongo-0.0.4/package/folder_structure.json`

 * *Files identical despite different names*

### Comparing `fastapi-mongo-0.0.3/setup.py` & `fastapi-mongo-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fastapi-mongo',
-    version='0.0.3',
+    version='0.0.4',
     long_description='This is a simple package that helps you to create a FastAPI project with MongoDB it comes with default crud operations and database setup just configure your environment variables and you are good to go.',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
@@ -15,14 +15,14 @@
     ],
     packages=find_packages(),
     data_files=[
         ('', ['package/folder_structure.json']),
     ],
     include_package_data=True,
     install_requires=["fastapi", "pymongo", "python-dotenv",
-                      "uvicorn", "passlib", "python-jose", "python-multipart"],
+                      "uvicorn", "passlib", "python-jose", "python-multipart", 'setupttols',],
     entry_points={
         'console_scripts': [
             'build=package.build_structure:create_files_and_dirs_from_json',
         ],
     },
 )
```

