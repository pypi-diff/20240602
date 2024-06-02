# Comparing `tmp/diti-0.0.4.tar.gz` & `tmp/diti-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diti-0.0.4.tar", last modified: Fri Dec  8 21:30:29 2023, max compression
+gzip compressed data, was "diti-0.0.6.tar", last modified: Sun Jun  2 16:44:47 2024, max compression
```

## Comparing `diti-0.0.4.tar` & `diti-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-12-08 21:30:29.366569 diti-0.0.4/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-10-14 09:35:39.000000 diti-0.0.4/LICENSE
--rw-r--r--   0 mujdecisy   (501) staff       (20)     6962 2023-12-08 21:30:29.366392 diti-0.0.4/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)     6612 2023-10-14 10:30:47.000000 diti-0.0.4/README.md
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-12-08 21:30:29.364539 diti-0.0.4/diti/
--rw-r--r--   0 mujdecisy   (501) staff       (20)      410 2023-12-08 21:30:04.000000 diti-0.0.4/diti/__init__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     4083 2023-10-14 09:18:14.000000 diti-0.0.4/diti/calcs.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)      309 2023-10-14 09:16:13.000000 diti-0.0.4/diti/constants.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2098 2023-10-24 19:51:15.000000 diti-0.0.4/diti/diti_interval.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     3817 2023-12-08 18:48:17.000000 diti-0.0.4/diti/diti_obj.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2471 2023-10-14 09:18:49.000000 diti-0.0.4/diti/diti_ops.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     8723 2023-10-14 09:22:00.000000 diti-0.0.4/diti/part_obj.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)    23492 2023-10-14 08:58:14.000000 diti-0.0.4/diti/timezones.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     1909 2023-10-14 09:16:52.000000 diti-0.0.4/diti/util.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-12-08 21:30:29.365386 diti-0.0.4/diti.egg-info/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     6962 2023-12-08 21:30:29.000000 diti-0.0.4/diti.egg-info/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)      395 2023-12-08 21:30:29.000000 diti-0.0.4/diti.egg-info/SOURCES.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-12-08 21:30:29.000000 diti-0.0.4/diti.egg-info/dependency_links.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        5 2023-12-08 21:30:29.000000 diti-0.0.4/diti.egg-info/requires.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        5 2023-12-08 21:30:29.000000 diti-0.0.4/diti.egg-info/top_level.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-12-08 21:30:29.366625 diti-0.0.4/setup.cfg
--rw-r--r--   0 mujdecisy   (501) staff       (20)      684 2023-12-08 21:30:24.000000 diti-0.0.4/setup.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-12-08 21:30:29.366102 diti-0.0.4/test/
--rw-r--r--   0 mujdecisy   (501) staff       (20)     9246 2023-10-14 09:20:51.000000 diti-0.0.4/test/test_calcs.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     6636 2023-10-14 09:20:04.000000 diti-0.0.4/test/test_edit.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     2567 2023-10-11 15:36:32.000000 diti-0.0.4/test/test_init.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     4516 2023-10-14 09:19:55.000000 diti-0.0.4/test/test_interval.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-06-02 16:44:47.844987 diti-0.0.6/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1076 2023-10-14 09:35:39.000000 diti-0.0.6/LICENSE
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     6962 2024-06-02 16:44:47.844823 diti-0.0.6/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     6612 2023-10-14 10:30:47.000000 diti-0.0.6/README.md
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-06-02 16:44:47.842751 diti-0.0.6/diti/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      410 2023-12-08 21:31:04.000000 diti-0.0.6/diti/__init__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     4083 2023-10-14 09:18:14.000000 diti-0.0.6/diti/calcs.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      309 2023-10-14 09:16:13.000000 diti-0.0.6/diti/constants.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2098 2023-10-24 19:51:15.000000 diti-0.0.6/diti/diti_interval.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3817 2023-12-08 18:48:17.000000 diti-0.0.6/diti/diti_obj.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2471 2023-10-14 09:18:49.000000 diti-0.0.6/diti/diti_ops.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     8723 2023-10-14 09:22:00.000000 diti-0.0.6/diti/part_obj.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)    23492 2023-10-14 08:58:14.000000 diti-0.0.6/diti/timezones.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1909 2023-10-14 09:16:52.000000 diti-0.0.6/diti/util.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-06-02 16:44:47.843750 diti-0.0.6/diti.egg-info/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     6962 2024-06-02 16:44:47.000000 diti-0.0.6/diti.egg-info/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      395 2024-06-02 16:44:47.000000 diti-0.0.6/diti.egg-info/SOURCES.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2024-06-02 16:44:47.000000 diti-0.0.6/diti.egg-info/dependency_links.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       14 2024-06-02 16:44:47.000000 diti-0.0.6/diti.egg-info/requires.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        5 2024-06-02 16:44:47.000000 diti-0.0.6/diti.egg-info/top_level.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2024-06-02 16:44:47.845060 diti-0.0.6/setup.cfg
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      696 2024-06-02 16:44:47.000000 diti-0.0.6/setup.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2024-06-02 16:44:47.844530 diti-0.0.6/test/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     9246 2023-10-14 09:20:51.000000 diti-0.0.6/test/test_calcs.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     6636 2023-10-14 09:20:04.000000 diti-0.0.6/test/test_edit.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     2567 2023-10-11 15:36:32.000000 diti-0.0.6/test/test_init.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     4516 2023-10-14 09:19:55.000000 diti-0.0.6/test/test_interval.py
```

### Comparing `diti-0.0.4/LICENSE` & `diti-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/PKG-INFO` & `diti-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diti
-Version: 0.0.4
+Version: 0.0.6
 Summary: diti to reduce your datetime operation pains
 Home-page: https://github.com/mujdecisy/diti
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,diti,datetime,timezone
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `diti-0.0.4/README.md` & `diti-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/diti/calcs.py` & `diti-0.0.6/diti/calcs.py`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/diti/diti_interval.py` & `diti-0.0.6/diti/diti_interval.py`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/diti/diti_obj.py` & `diti-0.0.6/diti/diti_obj.py`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/diti/diti_ops.py` & `diti-0.0.6/diti/diti_ops.py`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/diti/part_obj.py` & `diti-0.0.6/diti/part_obj.py`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/diti/timezones.py` & `diti-0.0.6/diti/timezones.py`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/diti/util.py` & `diti-0.0.6/diti/util.py`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/diti.egg-info/PKG-INFO` & `diti-0.0.6/diti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diti
-Version: 0.0.4
+Version: 0.0.6
 Summary: diti to reduce your datetime operation pains
 Home-page: https://github.com/mujdecisy/diti
 Author: mujdecisy
 Author-email: mujdecisy@gmail.com
 Keywords: python,diti,datetime,timezone
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `diti-0.0.4/setup.py` & `diti-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="diti",
-    version="0.0.4",
+    version="0.0.6",
     description="diti to reduce your datetime operation pains",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mujdecisy/diti",
     keywords=["python", "diti", "datetime", "timezone"],
     author="mujdecisy",
     author_email="mujdecisy@gmail.com",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     packages=["diti"],
     include_package_data=True,
-    install_requires=["pytz"]
+    install_requires=["pytz", "dateutil"]
 )
```

### Comparing `diti-0.0.4/test/test_calcs.py` & `diti-0.0.6/test/test_calcs.py`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/test/test_edit.py` & `diti-0.0.6/test/test_edit.py`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/test/test_init.py` & `diti-0.0.6/test/test_init.py`

 * *Files identical despite different names*

### Comparing `diti-0.0.4/test/test_interval.py` & `diti-0.0.6/test/test_interval.py`

 * *Files identical despite different names*

