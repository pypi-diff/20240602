# Comparing `tmp/DCMake-0.0.6.tar.gz` & `tmp/DCMake-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DCMake-0.0.6.tar", last modified: Sun Jun  2 02:12:34 2024, max compression
+gzip compressed data, was "DCMake-0.0.7.tar", last modified: Sun Jun  2 13:59:18 2024, max compression
```

## Comparing `DCMake-0.0.6.tar` & `DCMake-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 02:12:34.655970 DCMake-0.0.6/
-drwxrwxrwx   0        0        0        0 2024-06-02 02:12:34.640350 DCMake-0.0.6/DCMake.egg-info/
--rw-rw-rw-   0        0        0      526 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-06-02 02:12:34.000000 DCMake-0.0.6/DCMake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2023-12-03 06:25:44.000000 DCMake-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      526 2024-06-02 02:12:34.655970 DCMake-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-06-01 11:13:24.000000 DCMake-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 02:12:34.609099 DCMake-0.0.6/dcmake/
--rw-rw-rw-   0        0        0     1583 2024-06-02 01:18:17.000000 DCMake-0.0.6/dcmake/__init__.py
--rw-rw-rw-   0        0        0      290 2024-06-02 01:14:49.000000 DCMake-0.0.6/dcmake/config.py
--rw-rw-rw-   0        0        0      685 2024-06-02 01:56:56.000000 DCMake-0.0.6/dcmake/tool.py
--rw-rw-rw-   0        0        0     5671 2024-06-02 02:11:06.000000 DCMake-0.0.6/dcmake/url.py
--rw-rw-rw-   0        0        0       42 2024-06-02 02:12:34.655970 DCMake-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      759 2024-06-02 02:12:26.000000 DCMake-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 13:59:18.874225 DCMake-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-06-02 13:59:18.842962 DCMake-0.0.7/DCMake.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-06-02 13:59:14.000000 DCMake-0.0.7/DCMake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-06-02 13:59:14.000000 DCMake-0.0.7/DCMake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 13:59:14.000000 DCMake-0.0.7/DCMake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-06-02 13:59:14.000000 DCMake-0.0.7/DCMake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-06-02 13:59:14.000000 DCMake-0.0.7/DCMake.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-02 13:59:14.000000 DCMake-0.0.7/DCMake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2023-12-03 06:25:44.000000 DCMake-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      526 2024-06-02 13:59:18.842962 DCMake-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-06-01 11:13:24.000000 DCMake-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 13:59:18.827339 DCMake-0.0.7/dcmake/
+-rw-rw-rw-   0        0        0     2353 2024-06-02 13:57:54.000000 DCMake-0.0.7/dcmake/__init__.py
+-rw-rw-rw-   0        0        0      290 2024-06-02 01:14:49.000000 DCMake-0.0.7/dcmake/config.py
+-rw-rw-rw-   0        0        0      685 2024-06-02 01:56:56.000000 DCMake-0.0.7/dcmake/tool.py
+-rw-rw-rw-   0        0        0     5671 2024-06-02 02:11:06.000000 DCMake-0.0.7/dcmake/url.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 13:59:18.874225 DCMake-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      759 2024-06-02 13:59:00.000000 DCMake-0.0.7/setup.py
```

### Comparing `DCMake-0.0.6/DCMake.egg-info/PKG-INFO` & `DCMake-0.0.7/DCMake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DCMake
-Version: 0.0.6
+Version: 0.0.7
 Summary: Download github repository to CMake Project
 Home-page: 
 Author: Tietu
 Author-email: yhy2637@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `DCMake-0.0.6/LICENSE` & `DCMake-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `DCMake-0.0.6/PKG-INFO` & `DCMake-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DCMake
-Version: 0.0.6
+Version: 0.0.7
 Summary: Download github repository to CMake Project
 Home-page: 
 Author: Tietu
 Author-email: yhy2637@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `DCMake-0.0.6/dcmake/__init__.py` & `DCMake-0.0.7/dcmake/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,47 @@
-import argparse
+import argparse, os
 
 if __name__ == "__main__":
     import url, config, tool
 else:
     import dcmake.url as url
     import dcmake.tool as tool
     import dcmake.config as config
 
 def main():
     parser = argparse.ArgumentParser(description="Download github repository to CMake Project")
     parser.add_argument("-i", "--install", help="install github repository")
     parser.add_argument("-u", "--url", help="download file url")
     parser.add_argument("-o", "--output", help="output file path")
+    parser.add_argument("-uz", "--unzip", help="unzip file", action="store_true")
+    parser.add_argument("-c", "--clean", help="clean file", action="store_true")
     parser.add_argument("-v", "--version", help="DCMake Version", action="version", version=config.version)
 
     args = parser.parse_args()
 
     if not args.url is None or not args.output is None:
-        print(args.url)
         if args.url.find(";") == -1: FileDownload = url.downloadFile(args.url, args.output)
         else:
             FileDownload = url.downloadFileList(args.url, args.output)
         if FileDownload:
             print(f"{config.colors["green"]}Download Success{config.colors["end"]}")
         else:
             print(f"{config.colors["red"]}Download Failed{config.colors["end"]}")
+        if not args.unzip is None:
+            if args.url.find(";") == -1:
+                fileName = args.url.split('/')[-1]
+                tool.unzipFile(f"{args.output}/{fileName}", args.output)
+                os.remove(f"{args.output}/{fileName}")
+            else:
+                for file in args.url.split(";"):
+                    fileName = file.spilt("/")[-1]
+                    if fileName.endswith(".zip"):
+                        tool.unzipFile(f"{args.output}/{fileName}", args.output)
+                    if not args.clean is None:
+                        os.remove(f"{args.output}/{fileName}")
 
     if not args.install is None:
         if tool.checkGitAndCMake():
             if url.install(args.install):
                 print(f"{config.colors["green"]}Install Success{config.colors["end"]}")
             else:
                 print(f"{config.colors["red"]}Install Failed{config.colors["end"]}")
```

### Comparing `DCMake-0.0.6/dcmake/tool.py` & `DCMake-0.0.7/dcmake/tool.py`

 * *Files identical despite different names*

### Comparing `DCMake-0.0.6/dcmake/url.py` & `DCMake-0.0.7/dcmake/url.py`

 * *Files identical despite different names*

### Comparing `DCMake-0.0.6/setup.py` & `DCMake-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="DCMake",
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(),
     install_requires=[
         "requests>=2.31.0",
         "tqdm>=4.66.4"
     ],
     entry_points={
         "console_scripts": [
```

