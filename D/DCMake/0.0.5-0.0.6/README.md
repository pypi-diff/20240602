# Comparing `tmp/DCMake-0.0.5.tar.gz` & `tmp/DCMake-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DCMake-0.0.5.tar", last modified: Sun Jun  2 02:03:28 2024, max compression
+gzip compressed data, was "DCMake-0.0.6.tar", last modified: Sun Jun  2 02:12:34 2024, max compression
```

## Comparing `DCMake-0.0.5.tar` & `DCMake-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 02:03:28.849748 DCMake-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-06-02 02:03:28.834163 DCMake-0.0.5/DCMake.egg-info/
--rw-rw-rw-   0        0        0      526 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-06-02 02:03:27.000000 DCMake-0.0.5/DCMake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2023-12-03 06:25:44.000000 DCMake-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      526 2024-06-02 02:03:28.834163 DCMake-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-06-01 11:13:24.000000 DCMake-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 02:03:28.818499 DCMake-0.0.5/dcmake/
--rw-rw-rw-   0        0        0     1583 2024-06-02 01:18:17.000000 DCMake-0.0.5/dcmake/__init__.py
--rw-rw-rw-   0        0        0      290 2024-06-02 01:14:49.000000 DCMake-0.0.5/dcmake/config.py
--rw-rw-rw-   0        0        0      685 2024-06-02 01:56:56.000000 DCMake-0.0.5/dcmake/tool.py
--rw-rw-rw-   0        0        0     5518 2024-06-02 01:59:04.000000 DCMake-0.0.5/dcmake/url.py
--rw-rw-rw-   0        0        0       42 2024-06-02 02:03:28.849748 DCMake-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      759 2024-06-02 01:59:33.000000 DCMake-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 02:12:34.655970 DCMake-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-06-02 02:12:34.640350 DCMake-0.0.6/DCMake.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2023-12-03 06:25:44.000000 DCMake-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      526 2024-06-02 02:12:34.655970 DCMake-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-06-01 11:13:24.000000 DCMake-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 02:12:34.609099 DCMake-0.0.6/dcmake/
+-rw-rw-rw-   0        0        0     1583 2024-06-02 01:18:17.000000 DCMake-0.0.6/dcmake/__init__.py
+-rw-rw-rw-   0        0        0      290 2024-06-02 01:14:49.000000 DCMake-0.0.6/dcmake/config.py
+-rw-rw-rw-   0        0        0      685 2024-06-02 01:56:56.000000 DCMake-0.0.6/dcmake/tool.py
+-rw-rw-rw-   0        0        0     5671 2024-06-02 02:11:06.000000 DCMake-0.0.6/dcmake/url.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 02:12:34.655970 DCMake-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      759 2024-06-02 02:12:26.000000 DCMake-0.0.6/setup.py
```

### Comparing `DCMake-0.0.5/DCMake.egg-info/PKG-INFO` & `DCMake-0.0.6/DCMake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DCMake
-Version: 0.0.5
+Version: 0.0.6
 Summary: Download github repository to CMake Project
 Home-page: 
 Author: Tietu
 Author-email: yhy2637@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `DCMake-0.0.5/LICENSE` & `DCMake-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `DCMake-0.0.5/PKG-INFO` & `DCMake-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DCMake
-Version: 0.0.5
+Version: 0.0.6
 Summary: Download github repository to CMake Project
 Home-page: 
 Author: Tietu
 Author-email: yhy2637@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `DCMake-0.0.5/dcmake/__init__.py` & `DCMake-0.0.6/dcmake/__init__.py`

 * *Files identical despite different names*

### Comparing `DCMake-0.0.5/dcmake/tool.py` & `DCMake-0.0.6/dcmake/tool.py`

 * *Files identical despite different names*

### Comparing `DCMake-0.0.5/dcmake/url.py` & `DCMake-0.0.6/dcmake/url.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,19 +96,28 @@
     global gitCloneBool, cmakeConfigBool, cmakeBuildBool
     gitCloneBool = False
     cmakeConfigBool = False
     cmakeBuildBool = False
 
 def gitClone(url: str, path: str) -> bool:
     global gitCloneBool
-    subprocess.run(["git", "clone", "--recursive", url, path], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    try:
+        subprocess.run(["git", "clone", "--recursive", url, path], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    except Exception:
+        pass
     gitCloneBool = True
 
 def cmakeConfig(path: str) -> bool:
     global cmakeConfigBool
-    subprocess.run(["cmake", "--no-warn-unused-cli", "-DCMAKE_EXPORT_COMPILE_COMMANDS:BOOL=TRUE", "-S" + path, "-B" + path + "/build", "-G", "Visual Studio 17 2022", "-T", "host=x64", "-A", "x64"], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    try:
+        subprocess.run(["cmake", "--no-warn-unused-cli", "-DCMAKE_EXPORT_COMPILE_COMMANDS:BOOL=TRUE", "-S" + path, "-B" + path + "/build", "-G", "Visual Studio 17 2022", "-T", "host=x64", "-A", "x64"], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    except Exception:
+        pass
     cmakeConfigBool = True
 
 def cmakeBuild(path: str) -> bool:
     global cmakeBuildBool
-    subprocess.run(["cmake", "--build", path + "/build", "--config", "Release", "--target", "ALL_BUILD" ,"-j", f"{tool.getCPUThreads() * 2}", "--"], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    try:
+        subprocess.run(["cmake", "--build", path + "/build", "--config", "Release", "--target", "ALL_BUILD" ,"-j", f"{tool.getCPUThreads() * 2}", "--"], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    except Exception:
+        pass
     cmakeBuildBool = True
```

### Comparing `DCMake-0.0.5/setup.py` & `DCMake-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="DCMake",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(),
     install_requires=[
         "requests>=2.31.0",
         "tqdm>=4.66.4"
     ],
     entry_points={
         "console_scripts": [
```

