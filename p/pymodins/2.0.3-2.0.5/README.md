# Comparing `tmp/pymodins-2.0.3.tar.gz` & `tmp/pymodins-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-2ozr1yeo\pymodins-2.0.3.tar", last modified: Tue May 28 09:17:16 2024, max compression
+gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-fpoh04em\pymodins-2.0.5.tar", last modified: Sun Jun  2 18:58:23 2024, max compression
```

## Comparing `pymodins-2.0.3.tar` & `pymodins-2.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 09:17:16.838189 pymodins-2.0.3/
--rw-rw-rw-   0        0        0     1085 2024-05-17 08:05:08.000000 pymodins-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     4355 2024-05-28 09:17:16.833621 pymodins-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3733 2024-05-27 12:55:01.000000 pymodins-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 09:17:16.808206 pymodins-2.0.3/pymodins/
--rw-rw-rw-   0        0        0      331 2024-05-26 16:45:06.000000 pymodins-2.0.3/pymodins/__init__.py
--rw-rw-rw-   0        0        0    56322 2024-05-28 09:16:36.000000 pymodins-2.0.3/pymodins/installer.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:17:16.829781 pymodins-2.0.3/pymodins.egg-info/
--rw-rw-rw-   0        0        0     4355 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-28 09:17:16.000000 pymodins-2.0.3/pymodins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 09:17:16.838189 pymodins-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      934 2024-05-26 09:49:24.000000 pymodins-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:58:23.280909 pymodins-2.0.5/
+-rw-rw-rw-   0        0        0     1133 2024-06-02 18:25:44.000000 pymodins-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4384 2024-06-02 18:58:23.277428 pymodins-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3733 2024-06-02 18:25:47.000000 pymodins-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 18:58:23.240975 pymodins-2.0.5/pymodins/
+-rw-rw-rw-   0        0        0      331 2024-06-02 18:58:00.000000 pymodins-2.0.5/pymodins/__init__.py
+-rw-rw-rw-   0        0        0    60418 2024-06-02 18:55:56.000000 pymodins-2.0.5/pymodins/installer.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:58:23.274466 pymodins-2.0.5/pymodins.egg-info/
+-rw-rw-rw-   0        0        0     4384 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 18:58:23.000000 pymodins-2.0.5/pymodins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 18:58:23.281841 pymodins-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      966 2024-06-02 18:57:56.000000 pymodins-2.0.5/setup.py
```

### Comparing `pymodins-2.0.3/LICENSE` & `pymodins-2.0.5/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-MIT License
+                            MIT License
 
-Copyright (c) 2024 Nandhan
+                    Copyright (c) 2024 Nandhan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pymodins-2.0.3/PKG-INFO` & `pymodins-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.3
+Version: 2.0.5
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com 
-Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer
+Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer,Nandhan-KA,PYMODINS,pymodins
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
```

### Comparing `pymodins-2.0.3/README.md` & `pymodins-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pymodins-2.0.3/pymodins/installer.py` & `pymodins-2.0.5/pymodins/installer.py`

 * *Files 22% similar despite different names*

```diff
@@ -38,22 +38,42 @@
 |_____|    |______|  |_____||_____|`.___.'|______.'|_____||_____|\____| \______.' 
                                                                                 
     """
     console.print(ascii_art, style="bold yellow")
     console.print("Creator: Nandhan K", style="bold cyan")
     console.print("Github: @github.com/Nandhan-KA", style="bold yellow")
 
+def banner_nointernet():
+    console = Console()
+    ascii_art="""              
+ _______  ____  ____  ____    ____   ___   ______   _____  ____  _____   ______   
+|_   __ \|_  _||_  _||_   \  /   _|.'   `.|_   _ `.|_   _||_   \|_   _|.' ____ \  
+  | |__) | \ \  / /    |   \/   | /  .-.  \ | | `. \ | |    |   \ | |  | (___ \_| 
+  |  ___/   \ \/ /     | |\  /| | | |   | | | |  | | | |    | |\ \| |   _.____`.  
+ _| |_      _|  |_    _| |_\/_| |_\  `-'  /_| |_.' /_| |_  _| |_\   |_ | \____) | 
+|_____|    |______|  |_____||_____|`.___.'|______.'|_____||_____|\____| \______.' 
+                                                                                
+    """
+    console.print(ascii_art, style="bold yellow")
+    console.print("\t Creator: Nandhan K", style="bold cyan")
+    console.print("\t Github: @github.com/Nandhan-KA", style="bold yellow")
+    console.print(" \n \t This Project Requires Internet Connection 🌐 ", style="bold yellow")
+
+import sys
+import subprocess
+
 def sys_info():
     print("System Platform:", sys.platform)
-    print("Python verion:", sys.version)
+    print("Python version:", sys.version)
     try:
         pip_version = subprocess.check_output(['pip', '--version']).decode().strip()
         print("pip version:", pip_version)
     except Exception as e:
-        print("Error:", e,"Reinstall Python with PIP and add PIP to the System PATH")
+        print("Error:", e, "Reinstall Python with PIP and add PIP to the System PATH")
+
 
 def upgrade_pip():
     try:
         installed_version = pip.__version__
 
         latest_pip_version_output = subprocess.check_output(['pip', 'install', '--upgrade', 'pip']).decode().strip()
         print("Latest pip version output:", latest_pip_version_output)
@@ -200,16 +220,31 @@
 ]
 
 jupyter_modules = [
     'jupyter',
     'notebook', 'jupyterlab', 'nbconvert', 'nbformat', 'ipywidgets', 'ipykernel', 'voila', 'jupyter_contrib_nbextensions', 'jupyter_dash', 'jupyter_bokeh', 'jupytext', 'jupyterhub', 'jupyter_client', 'qtconsole'
 ]
 
+# Module Types
+module_types = [
+        None,
+        'Basic Modules',
+        'Advanced Modules',
+        'Science Modules',
+        'Computer Vision Modules',
+        'Machine Learning Modules',
+        'Deep Learning Modules',
+        'Full Stack Development Modules',
+        'Network Modules',
+        'Build Modules',
+        'Jupyter Modules'
+    ]
+
 def installer():
-    if internet():
+    if internet() and sys.platform == 'win32':
         upgrade_pip()
         clear()
         banner()
         sys_info()
         
         module_types = [
             'Basic Modules', 'Advanced Modules', 'Science Modules', 'Computer Vision Modules',
@@ -350,1027 +385,1010 @@
 
             else:
                 print("Invalid selection. Please enter a valid number.")
 
         except Exception as e:
             print("Error:", e, "\nPlease try again.")
             installer()
+            
+    elif internet() and sys.platform == "linux":
+        banner()
+        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        return
+    
     else:
-        print("No Internet Connection")
+        banner_nointernet()
 
 
 def run():
     installer()
 
 def install_basic_modules():
-    banner()
-    selected_option = 1
-    clear()
-    module_types = [
-        None,
-        'Basic Modules',
-        'Advanced Modules',
-        'Science Modules',
-        'Computer Vision Modules',
-        'Machine Learning Modules',
-        'Deep Learning Modules',
-        'Full Stack Development Modules',
-        'Network Modules',
-        'Build Modules',
-        'Jupyter Modules'
-    ]
-
-    selected_module_type = module_types[selected_option]
-
-    if selected_module_type:
-        print(f"\nSelected Module Type: {selected_module_type}")
-        print("Modules:")
-        modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-        for i, module in enumerate(modules, 1):
-            print(f"{i}. {module}")
-
-        install_option = input(
-            "Do you want to install all modules in this section? (Yes/No): ").lower()
-        clear()
-        if install_option in ["yes", "y"]:
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
-
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
+    if internet() and sys.platform == 'win32':
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 1
 
-            for module in modules:
-                clear()
-                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
-                os.system(command)
-                log_mod(selected_module_type, module, python_folder)
+        selected_module_type = module_types[selected_option]
 
-            print("\nAll modules installed successfully.")
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
-        else:
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
             print("Modules:")
             modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
+                selected_module_type.lower().replace(" ", "_")]
             for i, module in enumerate(modules, 1):
                 print(f"{i}. {module}")
 
-            module_index = int(input(
-                "Enter the number corresponding to the module to install (type '0' to exit): "))
-
-            if module_index == 0:
-                print(
-                    "\nReload this program to install new modules of Python.")
-                sys.exit()
-
-            selected_module = modules[module_index - 1]
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
-
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
-            command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
-            os.system(command)
-
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
-
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
 
-def install_advanced_modules():
-    banner()
-    selected_option = 2
-    clear()
-    module_types = [
-        None,
-        'Basic Modules',
-        'Advanced Modules',
-        'Science Modules',
-        'Computer Vision Modules',
-        'Machine Learning Modules',
-        'Deep Learning Modules',
-        'Full Stack Development Modules',
-        'Network Modules',
-        'Build Modules',
-        'Jupyter Modules'
-    ]
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
 
-    selected_module_type = module_types[selected_option]
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
 
-    if selected_module_type:
-        print(f"\nSelected Module Type: {selected_module_type}")
-        print("Modules:")
-        modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-        for i, module in enumerate(modules, 1):
-            print(f"{i}. {module}")
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
 
-        install_option = input(
-            "Do you want to install all modules in this section? (Yes/No): ").lower()
-        clear()
-        if install_option in ["yes", "y"]:
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
 
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+                    
+    elif internet() and sys.platform == "linux":
+        banner()
+        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        return
+    
+    else:
+        banner_nointernet()
 
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
+def install_advanced_modules():
+    if internet():
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 2
+        
 
-            for module in modules:
-                clear()
-                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
-                os.system(command)
-                log_mod(selected_module_type, module, python_folder)
+        selected_module_type = module_types[selected_option]
 
-            print("\nAll modules installed successfully.")
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
-        else:
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
             print("Modules:")
             modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
+                selected_module_type.lower().replace(" ", "_")]
             for i, module in enumerate(modules, 1):
                 print(f"{i}. {module}")
-                
-            module_index = int(input(
-                "Enter the number corresponding to the module to install (type '0' to exit): "))
-
-            if module_index == 0:
-                print(
-                    "\nReload this program to install new modules of Python.")
-                sys.exit()
-
-            selected_module = modules[module_index - 1]
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
-
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
-            command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
-            os.system(command)
-
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
 
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
 
-def install_machinelearning_modules():
-    banner()
-    selected_option = 5
-    clear()
-    module_types = [
-        None,
-        'Basic Modules',
-        'Advanced Modules',
-        'Science Modules',
-        'Computer Vision Modules',
-        'Machine Learning Modules',
-        'Deep Learning Modules',
-        'Full Stack Development Modules',
-        'Network Modules',
-        'Build Modules',
-        'Jupyter Modules'
-    ]
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
 
-    selected_module_type = module_types[selected_option]
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+                    
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
 
-    if selected_module_type:
-        print(f"\nSelected Module Type: {selected_module_type}")
-        print("Modules:")
-        modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-        for i, module in enumerate(modules, 1):
-            print(f"{i}. {module}")
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
 
-        install_option = input(
-            "Do you want to install all modules in this section? (Yes/No): ").lower()
-        clear()
-        if install_option in ["yes", "y"]:
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            
+    elif internet() and sys.platform == "linux":
+        banner()
+        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        return
+    
+    else:
+        banner_nointernet()
 
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
 
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
+def install_machinelearning_modules():
+    if internet():
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 5
+        
 
-            for module in modules:
-                clear()
-                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
-                os.system(command)
-                log_mod(selected_module_type, module, python_folder)
+        selected_module_type = module_types[selected_option]
 
-            print("\nAll modules installed successfully.")
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
-        else:
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
             print("Modules:")
             modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
+                selected_module_type.lower().replace(" ", "_")]
             for i, module in enumerate(modules, 1):
                 print(f"{i}. {module}")
-            module_index = int(input(
-                "Enter the number corresponding to the module to install (type '0' to exit): "))
-
-            if module_index == 0:
-                print(
-                    "\nReload this program to install new modules of Python.")
-                sys.exit()
-
-            selected_module = modules[module_index - 1]
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
-
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
-            command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
-            os.system(command)
-
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
 
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
 
-def install_deeplearning_modules():
-    banner()
-    selected_option = 6
-    clear()
-    module_types = [
-        None,
-        'Basic Modules',
-        'Advanced Modules',
-        'Science Modules',
-        'Computer Vision Modules',
-        'Machine Learning Modules',
-        'Deep Learning Modules',
-        'Full Stack Development Modules',
-        'Network Modules',
-        'Build Modules',
-        'Jupyter Modules'
-    ]
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
 
-    selected_module_type = module_types[selected_option]
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
 
-    if selected_module_type:
-        print(f"\nSelected Module Type: {selected_module_type}")
-        print("Modules:")
-        modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-        for i, module in enumerate(modules, 1):
-            print(f"{i}. {module}")
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
 
-        install_option = input(
-            "Do you want to install all modules in this section? (Yes/No): ").lower()
-        clear()
-        if install_option in ["yes", "y"]:
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            
+    elif internet() and sys.platform == "linux":
+        banner()
+        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        return
+    
+    else:
+        banner_nointernet()
 
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
 
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
+def install_deeplearning_modules():
+    if internet():
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 6
+        
 
-            for module in modules:
-                clear()
-                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
-                os.system(command)
-                log_mod(selected_module_type, module, python_folder)
+        selected_module_type = module_types[selected_option]
 
-            print("\nAll modules installed successfully.")
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
-        else:
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
             print("Modules:")
             modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
+                selected_module_type.lower().replace(" ", "_")]
             for i, module in enumerate(modules, 1):
                 print(f"{i}. {module}")
-            module_index = int(input(
-                "Enter the number corresponding to the module to install (type '0' to exit): "))
-
-            if module_index == 0:
-                print(
-                    "\nReload this program to install new modules of Python.")
-                sys.exit()
-
-            selected_module = modules[module_index - 1]
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
-
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
-            command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
-            os.system(command)
-
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
 
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
 
-def install_fullstack_modules():
-    banner()
-    selected_option = 7
-    clear()
-    module_types = [
-        None,
-        'Basic Modules',
-        'Advanced Modules',
-        'Science Modules',
-        'Computer Vision Modules',
-        'Machine Learning Modules',
-        'Deep Learning Modules',
-        'Full Stack Development Modules',
-        'Network Modules',
-        'Build Modules',
-        'Jupyter Modules'
-    ]
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
 
-    selected_module_type = module_types[selected_option]
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
 
-    if selected_module_type:
-        print(f"\nSelected Module Type: {selected_module_type}")
-        print("Modules:")
-        modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-        for i, module in enumerate(modules, 1):
-            print(f"{i}. {module}")
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
 
-        install_option = input(
-            "Do you want to install all modules in this section? (Yes/No): ").lower()
-        clear()
-        if install_option in ["yes", "y"]:
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            
+    elif internet() and sys.platform == "linux":
+        banner()
+        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        return
+    
+    else:
+        banner_nointernet()
 
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
 
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
+def install_fullstack_modules():
+    if internet():
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 7
+        
 
-            for module in modules:
-                clear()
-                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
-                os.system(command)
-                log_mod(selected_module_type, module, python_folder)
+        selected_module_type = module_types[selected_option]
 
-            print("\nAll modules installed successfully.")
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
-        else:
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
             print("Modules:")
             modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
+                selected_module_type.lower().replace(" ", "_")]
             for i, module in enumerate(modules, 1):
                 print(f"{i}. {module}")
-            module_index = int(input(
-                "Enter the number corresponding to the module to install (type '0' to exit): "))
-
-            if module_index == 0:
-                print(
-                    "\nReload this program to install new modules of Python.")
-                sys.exit()
-
-            selected_module = modules[module_index - 1]
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
-
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
-            command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
-            os.system(command)
-
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
 
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
 
-def install_science_modules():
-    banner()
-    selected_option = 3
-    clear()
-    module_types = [
-        None,
-        'Basic Modules',
-        'Advanced Modules',
-        'Science Modules',
-        'Computer Vision Modules',
-        'Machine Learning Modules',
-        'Deep Learning Modules',
-        'Full Stack Development Modules',
-        'Network Modules',
-        'Build Modules',
-        'Jupyter Modules'
-    ]
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
 
-    selected_module_type = module_types[selected_option]
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
 
-    if selected_module_type:
-        print(f"\nSelected Module Type: {selected_module_type}")
-        print("Modules:")
-        modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-        for i, module in enumerate(modules, 1):
-            print(f"{i}. {module}")
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
 
-        install_option = input(
-            "Do you want to install all modules in this section? (Yes/No): ").lower()
-        clear()
-        if install_option in ["yes", "y"]:
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            
+    elif internet() and sys.platform == "linux":
+        banner()
+        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        return
+    
+    else:
+        banner_nointernet()
 
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
 
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
+def install_science_modules():
+    if internet():
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 3
+        
 
-            for module in modules:
-                clear()
-                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
-                os.system(command)
-                log_mod(selected_module_type, module, python_folder)
+        selected_module_type = module_types[selected_option]
 
-            print("\nAll modules installed successfully.")
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
-        else:
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
             print("Modules:")
             modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
+                selected_module_type.lower().replace(" ", "_")]
             for i, module in enumerate(modules, 1):
                 print(f"{i}. {module}")
-            module_index = int(input(
-                "Enter the number corresponding to the module to install (type '0' to exit): "))
 
-            if module_index == 0:
-                print(
-                    "\nReload this program to install new modules of Python.")
-                sys.exit()
-
-            selected_module = modules[module_index - 1]
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
-
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
+
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
             else:
-                python_folder = str(*versions)
-            command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
-            os.system(command)
-
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
 
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
+
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            
+    elif internet() and sys.platform == "linux":
+        banner()
+        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        return
+    
+    else:
+        banner_nointernet()
+
+      
 def install_computervision_modules():
-    banner()
-    selected_option = 4
-    clear()
-    module_types = [
-        None,
-        'Basic Modules',
-        'Advanced Modules',
-        'Science Modules',
-        'Computer Vision Modules',
-        'Machine Learning Modules',
-        'Deep Learning Modules',
-        'Full Stack Development Modules',
-        'Network Modules',
-        'Build Modules',
-        'Jupyter Modules'
-    ]
+    if internet():
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 4
+        
 
-    selected_module_type = module_types[selected_option]
+        selected_module_type = module_types[selected_option]
 
-    if selected_module_type:
-        print(f"\nSelected Module Type: {selected_module_type}")
-        print("Modules:")
-        modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-        for i, module in enumerate(modules, 1):
-            print(f"{i}. {module}")
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
+            print("Modules:")
+            modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
 
-        install_option = input(
-            "Do you want to install all modules in this section? (Yes/No): ").lower()
-        clear()
-        if install_option in ["yes", "y"]:
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
 
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+                for module in modules:
+                    if module == 'dlib':
+                        pymsgbox.alert("This Modules Required VSBuild Tools")
+                        print("Module dlib has to be installed after you have installed visual studio build tools")
+                        x = input("Do you want to install VS Build Tools? (y/n): ").lower()
+                        if x == "y":
+                            if install_vscode_build_tools():
+                                print("Build tools installed successfully.")
+                            else:
+                                print("Failed to install build tools.")
+                                continue  
+                            
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
 
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
             else:
-                python_folder = str(*versions)
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
 
-            for module in modules:
-                if module == 'dlib':
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                    
+                if selected_module == 'dlib':
                     pymsgbox.alert("This Modules Required VSBuild Tools")
                     print("Module dlib has to be installed after you have installed visual studio build tools")
                     x = input("Do you want to install VS Build Tools? (y/n): ").lower()
                     if x == "y":
                         if install_vscode_build_tools():
                             print("Build tools installed successfully.")
                         else:
                             print("Failed to install build tools.")
-                            continue  
-                        
-                clear()
-                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                                
+                    
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
                 os.system(command)
-                log_mod(selected_module_type, module, python_folder)
 
-            print("\nAll modules installed successfully.")
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
-        else:
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            
+    elif internet() and sys.platform == "linux":
+        banner()
+        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        return
+    
+    else:
+        banner_nointernet()
+
+       
+def install_network_modules():
+    if internet():
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 8
+        
+
+        selected_module_type = module_types[selected_option]
+
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
             print("Modules:")
             modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
+                selected_module_type.lower().replace(" ", "_")]
             for i, module in enumerate(modules, 1):
                 print(f"{i}. {module}")
-            module_index = int(input(
-                "Enter the number corresponding to the module to install (type '0' to exit): "))
 
-            if module_index == 0:
-                print(
-                    "\nReload this program to install new modules of Python.")
-                sys.exit()
-
-            selected_module = modules[module_index - 1]
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
-
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
-                
-            if selected_module == 'dlib':
-                pymsgbox.alert("This Modules Required VSBuild Tools")
-                print("Module dlib has to be installed after you have installed visual studio build tools")
-                x = input("Do you want to install VS Build Tools? (y/n): ").lower()
-                if x == "y":
-                    if install_vscode_build_tools():
-                        print("Build tools installed successfully.")
-                    else:
-                        print("Failed to install build tools.")
-                            
-                
-            command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
-            os.system(command)
-
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
 
-def install_network_modules():
-    banner()
-    selected_option = 8
-    clear()
-    module_types = [
-        None,
-        'Basic Modules',
-        'Advanced Modules',
-        'Science Modules',
-        'Computer Vision Modules',
-        'Machine Learning Modules',
-        'Deep Learning Modules',
-        'Full Stack Development Modules',
-        'Network Modules',
-        'Build Modules',
-        'Jupyter Modules'
-    ]
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
 
-    selected_module_type = module_types[selected_option]
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            else:
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
 
-    if selected_module_type:
-        print(f"\nSelected Module Type: {selected_module_type}")
-        print("Modules:")
-        modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-        for i, module in enumerate(modules, 1):
-            print(f"{i}. {module}")
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
+                os.system(command)
 
-        install_option = input(
-            "Do you want to install all modules in this section? (Yes/No): ").lower()
-        clear()
-        if install_option in ["yes", "y"]:
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            
+    elif internet() and sys.platform == "linux":
+        banner()
+        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        return
+    
+    else:
+        banner_nointernet()
 
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
 
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
+def install_build_modules():
+    if internet():
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 9
+        
 
-            for module in modules:
-                clear()
-                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
-                os.system(command)
-                log_mod(selected_module_type, module, python_folder)
+        selected_module_type = module_types[selected_option]
 
-            print("\nAll modules installed successfully.")
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
-        else:
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
             print("Modules:")
             modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
+                selected_module_type.lower().replace(" ", "_")]
             for i, module in enumerate(modules, 1):
                 print(f"{i}. {module}")
-            module_index = int(input(
-                "Enter the number corresponding to the module to install (type '0' to exit): "))
-
-            if module_index == 0:
-                print(
-                    "\nReload this program to install new modules of Python.")
-                sys.exit()
-
-            selected_module = modules[module_index - 1]
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
-
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
-            command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
-            os.system(command)
-
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
 
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
 
-def install_build_modules():
-    banner()
-    selected_option = 9
-    clear()
-    module_types = [
-        None,
-        'Basic Modules',
-        'Advanced Modules',
-        'Science Modules',
-        'Computer Vision Modules',
-        'Machine Learning Modules',
-        'Deep Learning Modules',
-        'Full Stack Development Modules',
-        'Network Modules',
-        'Build Modules',
-        'Jupyter Modules'
-    ]
-
-    selected_module_type = module_types[selected_option]
-
-    if selected_module_type:
-        print(f"\nSelected Module Type: {selected_module_type}")
-        print("Modules:")
-        modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-        for i, module in enumerate(modules, 1):
-            print(f"{i}. {module}")
-
-        install_option = input(
-            "Do you want to install all modules in this section? (Yes/No): ").lower()
-        clear()
-        if install_option in ["yes", "y"]:
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+                for module in modules:
+                    if module == 'rust' or  module == 'build' or module ==  'pep517':
+                        pymsgbox.alert("This Modules Required VSBuild Tools")
+                        print("Installing VSBuild Tools")
+                        install_vscode_build_tools()
+                        clear
+                        print("Module rust needs to be installed separately.")
+                        x = input("Do you want to install Rust? (y/n): ").lower()
+                        if x == "y":
+                            if install_rust():
+                                print("Rust installed successfully.")
+                            else:
+                                print("Failed to install Rust. Opening the Rust installation webpage.")
+                                webbrowser.open('https://www.rust-lang.org/tools/install')
+                                break 
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
 
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
             else:
-                python_folder = str(*versions)
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
 
-            for module in modules:
-                if module == 'rust':
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions) 
+                    
+                if selected_module == 'rust':
                     pymsgbox.alert("This Modules Required VSBuild Tools")
                     print("Installing VSBuild Tools")
                     install_vscode_build_tools()
                     clear
+                    pymsgbox.alert("This Modules Required VSBuild Tools")
                     print("Module rust needs to be installed separately.")
                     x = input("Do you want to install Rust? (y/n): ").lower()
                     if x == "y":
                         if install_rust():
                             print("Rust installed successfully.")
                         else:
                             print("Failed to install Rust. Opening the Rust installation webpage.")
                             webbrowser.open('https://www.rust-lang.org/tools/install')
-                            break  
-
-                    
-                clear()
-                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                            
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
                 os.system(command)
-                log_mod(selected_module_type, module, python_folder)
-
-            print("\nAll modules installed successfully.")
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
-        else:
-            print("Modules:")
-            modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-            for i, module in enumerate(modules, 1):
-                print(f"{i}. {module}")
-            module_index = int(input(
-                "Enter the number corresponding to the module to install (type '0' to exit): "))
-
-            if module_index == 0:
-                print(
-                    "\nReload this program to install new modules of Python.")
-                sys.exit()
-
-            selected_module = modules[module_index - 1]
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
-
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions) 
-                
-            if selected_module == 'rust':
-                pymsgbox.alert("This Modules Required VSBuild Tools")
-                print("Installing VSBuild Tools")
-                install_vscode_build_tools()
-                clear
-                pymsgbox.alert("This Modules Required VSBuild Tools")
-                print("Module rust needs to be installed separately.")
-                x = input("Do you want to install Rust? (y/n): ").lower()
-                if x == "y":
-                    if install_rust():
-                        print("Rust installed successfully.")
-                    else:
-                        print("Failed to install Rust. Opening the Rust installation webpage.")
-                        webbrowser.open('https://www.rust-lang.org/tools/install')
-                        
-            command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
-            os.system(command)
 
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            
+    elif internet() and sys.platform == "linux":
+        banner()
+        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        return
+    
+    else:
+        banner_nointernet()
 
 
 def install_jupyter_modules():
-    banner()
-    selected_option = 10
-    clear()
-    module_types = [
-        None,
-        'Basic Modules',
-        'Advanced Modules',
-        'Science Modules',
-        'Computer Vision Modules',
-        'Machine Learning Modules',
-        'Deep Learning Modules',
-        'Full Stack Development Modules',
-        'Network Modules',
-        'Build Modules',
-        'Jupyter Modules'
-    ]
-
-    selected_module_type = module_types[selected_option]
+    if internet():
+        upgrade_pip()
+        banner()
+        sys_info()
+        selected_option = 10
+        selected_module_type = module_types[selected_option]
 
-    if selected_module_type:
-        print(f"\nSelected Module Type: {selected_module_type}")
-        print("Modules:")
-        modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-        for i, module in enumerate(modules, 1):
-            print(f"{i}. {module}")
+        if selected_module_type:
+            print(f"\nSelected Module Type: {selected_module_type}")
+            print("Modules:")
+            modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
 
-        install_option = input(
-            "Do you want to install all modules in this section? (Yes/No): ").lower()
-        clear()
-        if install_option in ["yes", "y"]:
+            install_option = input(
+                "Do you want to install all modules in this section? (Yes/No): ").lower()
+            clear()
+            if install_option in ["yes", "y"]:
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
 
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+                for module in modules:
+                    clear()
+                    command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                    os.system(command)
+                    log_mod(selected_module_type, module, python_folder)
 
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
+                print("\nAll modules installed successfully.")
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
             else:
-                python_folder = str(*versions)
+                print("Modules:")
+                modules = globals()[
+                selected_module_type.lower().replace(" ", "_")]
+                for i, module in enumerate(modules, 1):
+                    print(f"{i}. {module}")
+                module_index = int(input(
+                    "Enter the number corresponding to the module to install (type '0' to exit): "))
 
-            for module in modules:
-                clear()
-                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
+                if module_index == 0:
+                    print(
+                        "\nReload this program to install new modules of Python.")
+                    sys.exit()
+
+                selected_module = modules[module_index - 1]
+
+                versions = os.listdir(
+                    f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
+
+                if len(versions) == 2:
+                    print(f"\nYou have two folders in your Python installation:")
+                    print("(1)", versions[0])
+                    print("(2)", versions[1])
+                    python_folder = versions[int(
+                        input("Select your Python folder (1 or 2): ")) - 1]
+                else:
+                    python_folder = str(*versions)
+                command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
                 os.system(command)
-                log_mod(selected_module_type, module, python_folder)
 
-            print("\nAll modules installed successfully.")
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
-        else:
-            print("Modules:")
-            modules = globals()[
-            selected_module_type.lower().replace(" ", "_")]
-            for i, module in enumerate(modules, 1):
-                print(f"{i}. {module}")
-            module_index = int(input(
-                "Enter the number corresponding to the module to install (type '0' to exit): "))
+                more = input("Do you want to install more? (Yes/No): ")
+                if more.lower() in ["no", "n"]:
+                    print(f"{user} Thank you for using.")
+                    sys.exit()
+                elif more.lower() in ["yes", "y"]:
+                    installer()
+            
+    elif internet() and sys.platform == "linux":
+        banner()
+        Console.print(" \t This program is designed to run on Windows systems only.", style="bold yellow")
+        return
+    
+    else:
+        banner_nointernet()
 
-            if module_index == 0:
-                print(
-                    "\nReload this program to install new modules of Python.")
-                sys.exit()
-
-            selected_module = modules[module_index - 1]
-
-            versions = os.listdir(
-                f"C:\\Users\\{user}\\AppData\\Local\\Programs\\Python")
-
-            if len(versions) == 2:
-                print(f"\nYou have two folders in your Python installation:")
-                print("(1)", versions[0])
-                print("(2)", versions[1])
-                python_folder = versions[int(
-                    input("Select your Python folder (1 or 2): ")) - 1]
-            else:
-                python_folder = str(*versions)
-            command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
-            os.system(command)
-
-            more = input("Do you want to install more? (Yes/No): ")
-            if more.lower() in ["no", "n"]:
-                print(f"{user} Thank you for using.")
-                sys.exit()
-            elif more.lower() in ["yes", "y"]:
-                installer()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymodins-2.0.3/pymodins.egg-info/PKG-INFO` & `pymodins-2.0.5/pymodins.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 2.0.3
+Version: 2.0.5
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com 
-Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer
+Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer,Nandhan-KA,PYMODINS,pymodins
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
```

### Comparing `pymodins-2.0.3/setup.py` & `pymodins-2.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pymodins",
-    version="2.0.3",
+    version="2.0.5",
     packages=find_packages(),
     install_requires=[
         "rich",
         "pymsgbox"
     ],
     entry_points={
         "console_scripts": [
             "pymodins=pymodins.installer:run",
         ],
     },
     author="Nandhan K",
     author_email="nandhan2003alamelu@gmail.com ",
     description="A module to install various Python packages.",
-    keywords="Python Module Installer, Python Package Installer, python modules installer, python package installer",
+    keywords="Python Module Installer, Python Package Installer, python modules installer, python package installer, Nandhan-KA, PYMODINS, pymodins",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/Nandhan-KA/pymodins",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

