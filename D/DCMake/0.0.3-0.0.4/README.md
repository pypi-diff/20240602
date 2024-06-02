# Comparing `tmp/DCMake-0.0.3.tar.gz` & `tmp/DCMake-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DCMake-0.0.3.tar", last modified: Sat Jun  1 12:39:14 2024, max compression
+gzip compressed data, was "DCMake-0.0.4.tar", last modified: Sat Jun  1 12:47:20 2024, max compression
```

## Comparing `DCMake-0.0.3.tar` & `DCMake-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 12:39:14.305261 DCMake-0.0.3/
-drwxrwxrwx   0        0        0        0 2024-06-01 12:39:14.295209 DCMake-0.0.3/DCMake.egg-info/
--rw-rw-rw-   0        0        0      526 2024-06-01 12:39:13.000000 DCMake-0.0.3/DCMake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-06-01 12:39:14.000000 DCMake-0.0.3/DCMake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 12:39:13.000000 DCMake-0.0.3/DCMake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-06-01 12:39:13.000000 DCMake-0.0.3/DCMake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-06-01 12:39:13.000000 DCMake-0.0.3/DCMake.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 12:39:13.000000 DCMake-0.0.3/DCMake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2023-12-03 06:25:44.000000 DCMake-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      526 2024-06-01 12:39:14.303238 DCMake-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-06-01 11:13:24.000000 DCMake-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 12:39:14.285166 DCMake-0.0.3/dcmake/
--rw-rw-rw-   0        0        0     1124 2024-06-01 12:21:11.000000 DCMake-0.0.3/dcmake/__init__.py
--rw-rw-rw-   0        0        0      589 2024-06-01 12:19:05.000000 DCMake-0.0.3/dcmake/tool.py
--rw-rw-rw-   0        0        0     2224 2024-06-01 12:31:23.000000 DCMake-0.0.3/dcmake/url.py
--rw-rw-rw-   0        0        0       42 2024-06-01 12:39:14.313297 DCMake-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      759 2024-06-01 12:39:00.000000 DCMake-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:47:20.870179 DCMake-0.0.4/
+drwxrwxrwx   0        0        0        0 2024-06-01 12:47:20.840016 DCMake-0.0.4/DCMake.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 12:47:20.000000 DCMake-0.0.4/DCMake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2023-12-03 06:25:44.000000 DCMake-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      526 2024-06-01 12:47:20.850054 DCMake-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-06-01 11:13:24.000000 DCMake-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 12:47:20.829948 DCMake-0.0.4/dcmake/
+-rw-rw-rw-   0        0        0     1124 2024-06-01 12:21:11.000000 DCMake-0.0.4/dcmake/__init__.py
+-rw-rw-rw-   0        0        0      589 2024-06-01 12:19:05.000000 DCMake-0.0.4/dcmake/tool.py
+-rw-rw-rw-   0        0        0     2224 2024-06-01 12:46:54.000000 DCMake-0.0.4/dcmake/url.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 12:47:20.870179 DCMake-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      759 2024-06-01 12:47:06.000000 DCMake-0.0.4/setup.py
```

### Comparing `DCMake-0.0.3/DCMake.egg-info/PKG-INFO` & `DCMake-0.0.4/DCMake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DCMake
-Version: 0.0.3
+Version: 0.0.4
 Summary: Download github repository to CMake Project
 Home-page: 
 Author: Tietu
 Author-email: yhy2637@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `DCMake-0.0.3/LICENSE` & `DCMake-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DCMake-0.0.3/PKG-INFO` & `DCMake-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DCMake
-Version: 0.0.3
+Version: 0.0.4
 Summary: Download github repository to CMake Project
 Home-page: 
 Author: Tietu
 Author-email: yhy2637@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `DCMake-0.0.3/dcmake/__init__.py` & `DCMake-0.0.4/dcmake/__init__.py`

 * *Files identical despite different names*

### Comparing `DCMake-0.0.3/dcmake/tool.py` & `DCMake-0.0.4/dcmake/tool.py`

 * *Files identical despite different names*

### Comparing `DCMake-0.0.3/dcmake/url.py` & `DCMake-0.0.4/dcmake/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,12 +33,12 @@
             subprocess.run(["cmake", "--build", path + "/build", "--config", "Release", "--target", "ALL_BUILD" ,"-j", f"{tool.getCPUThreads() * 2}", "--"])
             for root, _, files in os.walk(path + "/build/"):
                 for file in files:
                     if file.endswith(".lib"):
                         shutil.copy2(os.path.join(root, file), os.path.join(dirpath, "lib", file))
                     elif file.endswith(".dll") or file.endswith(".exe"):
                         shutil.copy2(os.path.join(root, file), os.path.join(dirpath, "bin", file))
-            shutil.rmtree("./" + path.split("/")[1], True)
+            shutil.rmtree("./" + path.split("/")[2], True)
             return True
         return False
     except Exception:
         return False
```

### Comparing `DCMake-0.0.3/setup.py` & `DCMake-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="DCMake",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     install_requires=[
         "requests>=2.31.0",
         "tqdm>=4.66.4"
     ],
     entry_points={
         "console_scripts": [
```

