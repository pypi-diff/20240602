# Comparing `tmp/pymodins-2.0.5.tar.gz` & `tmp/pymodins-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-fpoh04em\pymodins-2.0.5.tar", last modified: Sun Jun  2 18:58:23 2024, max compression
+gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-nq35zjv7\pymodins-2.0.6.tar", last modified: Sun Jun  2 19:08:19 2024, max compression
```

## Comparing `pymodins-2.0.5.tar` & `pymodins-2.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 18:58:23.280909 pymodins-2.0.5/
--rw-rw-rw-   0        0        0     1133 2024-06-02 18:25:44.000000 pymodins-2.0.5/LICENSE
--rw-rw-rw-   0        0        0     4384 2024-06-02 18:58:23.277428 pymodins-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3733 2024-06-02 18:25:47.000000 pymodins-2.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 18:58:23.240975 pymodins-2.0.5/pymodins/
--rw-rw-rw-   0        0        0      331 2024-06-02 18:58:00.000000 pymodins-2.0.5/pymodins/__init__.py
--rw-rw-rw-   0        0        0    60418 2024-06-02 18:55:56.000000 pymodins-2.0.5/pymodins/installer.py
-drwxrwxrwx   0        0        0        0 2024-06-02 18:58:23.274466 pymodins-2.0.5/pymodins.egg-info/
--rw-rw-rw-   0        0        0     4384 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 18:58:23.281841 pymodins-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0      966 2024-06-02 18:57:56.000000 pymodins-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:08:19.943999 pymodins-2.0.6/
+-rw-rw-rw-   0        0        0     1133 2024-06-02 18:25:44.000000 pymodins-2.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4406 2024-06-02 19:08:19.940515 pymodins-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3733 2024-06-02 18:25:47.000000 pymodins-2.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 19:08:19.910436 pymodins-2.0.6/pymodins/
+-rw-rw-rw-   0        0        0      331 2024-06-02 19:07:49.000000 pymodins-2.0.6/pymodins/__init__.py
+-rw-rw-rw-   0        0        0    60371 2024-06-02 19:03:55.000000 pymodins-2.0.6/pymodins/installer.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:08:19.937574 pymodins-2.0.6/pymodins.egg-info/
+-rw-rw-rw-   0        0        0     4406 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 19:08:19.000000 pymodins-2.0.6/pymodins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 19:08:19.943999 pymodins-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-06-02 19:08:02.000000 pymodins-2.0.6/setup.py
```

### Comparing `pymodins-2.0.5/LICENSE` & `pymodins-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodins-2.0.5/PKG-INFO` & `pymodins-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.5
+Version: 2.0.6
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
-Author-email: nandhan2003alamelu@gmail.com 
+Author-email: nandhan2003alamelu@gmail.com
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer,Nandhan-KA,PYMODINS,pymodins
+Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
 Requires-Dist: pymsgbox
 
 # PYMODINS
```

### Comparing `pymodins-2.0.5/README.md` & `pymodins-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pymodins-2.0.5/pymodins/installer.py` & `pymodins-2.0.6/pymodins/installer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1209,15 +1209,15 @@
                     print("(2)", versions[1])
                     python_folder = versions[int(
                         input("Select your Python folder (1 or 2): ")) - 1]
                 else:
                     python_folder = str(*versions)
 
                 for module in modules:
-                    if module == 'rust' or  module == 'build' or module ==  'pep517':
+                    if module == 'rust':
                         pymsgbox.alert("This Modules Required VSBuild Tools")
                         print("Installing VSBuild Tools")
                         install_vscode_build_tools()
                         clear
                         print("Module rust needs to be installed separately.")
                         x = input("Do you want to install Rust? (y/n): ").lower()
                         if x == "y":
@@ -1296,15 +1296,14 @@
         banner()
         Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
         return
     
     else:
         banner_nointernet()
 
-
 def install_jupyter_modules():
     if internet():
         upgrade_pip()
         banner()
         sys_info()
         selected_option = 10
         selected_module_type = module_types[selected_option]
```

### Comparing `pymodins-2.0.5/pymodins.egg-info/PKG-INFO` & `pymodins-2.0.6/pymodins.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.5
+Version: 2.0.6
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
-Author-email: nandhan2003alamelu@gmail.com 
+Author-email: nandhan2003alamelu@gmail.com
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer,Nandhan-KA,PYMODINS,pymodins
+Platform: win32
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
 Requires-Dist: pymsgbox
 
 # PYMODINS
```

