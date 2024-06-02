# Comparing `tmp/sofapal-0.0.3.tar.gz` & `tmp/sofapal-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sofapal-0.0.3.tar", last modified: Fri May 31 22:50:53 2024, max compression
+gzip compressed data, was "sofapal-0.0.4.tar", last modified: Sun Jun  2 18:35:10 2024, max compression
```

## Comparing `sofapal-0.0.3.tar` & `sofapal-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-05-31 22:50:53.605445 sofapal-0.0.3/
--rw-r--r--   0 colinblount   (701) staff       (20)     1061 2024-05-31 14:50:40.000000 sofapal-0.0.3/LICENSE
--rw-r--r--   0 colinblount   (701) staff       (20)     3184 2024-05-31 22:50:53.605266 sofapal-0.0.3/PKG-INFO
--rw-r--r--   0 colinblount   (701) staff       (20)     2383 2024-05-31 22:46:02.000000 sofapal-0.0.3/README.md
-drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-05-31 22:50:53.604004 sofapal-0.0.3/pal/
--rw-r--r--   0 colinblount   (701) staff       (20)       62 2024-05-31 14:40:15.000000 sofapal-0.0.3/pal/__init__.py
--rw-r--r--   0 colinblount   (701) staff       (20)     3272 2024-05-31 22:04:14.000000 sofapal-0.0.3/pal/main.py
--rw-r--r--   0 colinblount   (701) staff       (20)       38 2024-05-31 22:50:53.605487 sofapal-0.0.3/setup.cfg
--rw-r--r--   0 colinblount   (701) staff       (20)     1237 2024-05-31 22:50:17.000000 sofapal-0.0.3/setup.py
-drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-05-31 22:50:53.605068 sofapal-0.0.3/sofapal.egg-info/
--rw-r--r--   0 colinblount   (701) staff       (20)     3184 2024-05-31 22:50:53.000000 sofapal-0.0.3/sofapal.egg-info/PKG-INFO
--rw-r--r--   0 colinblount   (701) staff       (20)      246 2024-05-31 22:50:53.000000 sofapal-0.0.3/sofapal.egg-info/SOURCES.txt
--rw-r--r--   0 colinblount   (701) staff       (20)        1 2024-05-31 22:50:53.000000 sofapal-0.0.3/sofapal.egg-info/dependency_links.txt
--rw-r--r--   0 colinblount   (701) staff       (20)       37 2024-05-31 22:50:53.000000 sofapal-0.0.3/sofapal.egg-info/entry_points.txt
--rw-r--r--   0 colinblount   (701) staff       (20)       11 2024-05-31 22:50:53.000000 sofapal-0.0.3/sofapal.egg-info/requires.txt
--rw-r--r--   0 colinblount   (701) staff       (20)        4 2024-05-31 22:50:53.000000 sofapal-0.0.3/sofapal.egg-info/top_level.txt
+drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-06-02 18:35:10.029594 sofapal-0.0.4/
+-rw-r--r--   0 colinblount   (701) staff       (20)     1061 2024-05-31 14:50:40.000000 sofapal-0.0.4/LICENSE
+-rw-r--r--   0 colinblount   (701) staff       (20)     4186 2024-06-02 18:35:10.029391 sofapal-0.0.4/PKG-INFO
+-rw-r--r--   0 colinblount   (701) staff       (20)     3360 2024-06-02 18:34:12.000000 sofapal-0.0.4/README.md
+drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-06-02 18:35:10.028120 sofapal-0.0.4/pal/
+-rw-r--r--   0 colinblount   (701) staff       (20)       62 2024-05-31 14:40:15.000000 sofapal-0.0.4/pal/__init__.py
+-rw-r--r--   0 colinblount   (701) staff       (20)     9195 2024-06-02 18:06:13.000000 sofapal-0.0.4/pal/main.py
+-rw-r--r--   0 colinblount   (701) staff       (20)      655 2024-06-01 23:42:03.000000 sofapal-0.0.4/pal/spinner_util.py
+-rw-r--r--   0 colinblount   (701) staff       (20)     1079 2024-06-02 18:06:02.000000 sofapal-0.0.4/pal/window_util.py
+-rw-r--r--   0 colinblount   (701) staff       (20)       38 2024-06-02 18:35:10.029638 sofapal-0.0.4/setup.cfg
+-rw-r--r--   0 colinblount   (701) staff       (20)     1214 2024-06-02 18:35:06.000000 sofapal-0.0.4/setup.py
+drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-06-02 18:35:10.029183 sofapal-0.0.4/sofapal.egg-info/
+-rw-r--r--   0 colinblount   (701) staff       (20)     4186 2024-06-02 18:35:10.000000 sofapal-0.0.4/sofapal.egg-info/PKG-INFO
+-rw-r--r--   0 colinblount   (701) staff       (20)      289 2024-06-02 18:35:10.000000 sofapal-0.0.4/sofapal.egg-info/SOURCES.txt
+-rw-r--r--   0 colinblount   (701) staff       (20)        1 2024-06-02 18:35:10.000000 sofapal-0.0.4/sofapal.egg-info/dependency_links.txt
+-rw-r--r--   0 colinblount   (701) staff       (20)       37 2024-06-02 18:35:10.000000 sofapal-0.0.4/sofapal.egg-info/entry_points.txt
+-rw-r--r--   0 colinblount   (701) staff       (20)       21 2024-06-02 18:35:10.000000 sofapal-0.0.4/sofapal.egg-info/requires.txt
+-rw-r--r--   0 colinblount   (701) staff       (20)        4 2024-06-02 18:35:10.000000 sofapal-0.0.4/sofapal.egg-info/top_level.txt
```

### Comparing `sofapal-0.0.3/LICENSE` & `sofapal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sofapal-0.0.3/PKG-INFO` & `sofapal-0.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sofapal
-Version: 0.0.3
+Version: 0.0.4
 Summary: A friend; a chum.
 Home-page: https://github.com/slumberdemon/pal
 Author: SlumberDemon
 Author-email: hi@sofa.sh
 License: MIT
 Project-URL: Bug Reports, https://github.com/slumberdemon/pal/issues
 Project-URL: Source, https://github.com/slumberdemon/pal
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: inquirerpy
+Requires-Dist: pytermgui
 
 # Pal
 
 A friend; a chum.
 
 ### Where
 
@@ -31,28 +32,33 @@
 ```sh
 pip3 install -U sofapal
 ```
 
 #### Development
 
 ```sh
+# clone repository
 pip install -U git+https://github.com/slumberdemon/pal
+# create a virtual environment in the .venv directory
+python3 -m venv .venv
+# set up the current shell to use that virtual environment
+source .venv/bin/activate
 ```
 
 ### Why
 
 Pal is a command-line interface that includes a range of general features and functions. Pal is a personal exploration into creating a command-line interface using Python with aims to use as few dependencies as possible.
 
 ### How
 
 ```shell
 pal
 ```
 
-Pal loads configs from the `.pal` folder located in `$HOME`. Example configs can be found in the in [`.pal`](https://github.com/SlumberDemon/pal/tree/main/.pal). Therefore when adding/creating configurations make sure they are in that folder.
+Pal loads configs from the `.pal` folder located in `$HOME`. Example configs can be found in [`.pal`](https://github.com/SlumberDemon/pal/tree/main/.pal). Therefore when adding/creating configurations make sure they are in that folder.
 
 #### Create
 
 Pal enables for quick project creation using user-created templates. Templates are written in shell and are provided one argument.
 
 > Pal runs templates like this: `bash template.sh {name}`.
 
@@ -67,14 +73,16 @@
 This file is stored in the `templates` folder. In the example `$1` is used to access the name of the project provided by pal.
 
 It's recommended that the file name is in this format: `language-language-tool.sh`. This will make it easier to search for this template with pal.
 
 ```shell
 usage: pal create [-h] [-n NAME] [-e {zed,code}]
 
+Create project using a template
+
 options:
   -h, --help            show this help message and exit
   -n NAME, --name NAME  Name of the project
   -e {zed,code}, --editor {zed,code}
                         Code editor to open project with
 ```
 
@@ -111,7 +119,32 @@
 positional arguments:
   query
 
 options:
   -h, --help    show this help message and exit
   -e, --engine  Select engine to use
 ```
+
+#### Weather
+
+Pal can display information on the weather. Pal needs an [`weatherapi`](https://www.weatherapi.com) api key to do so.
+
+Setup for weather is easy and can be done with the following.
+
+```shell
+pal weather
+```
+
+Running with the command with no configs for the first time will start the interactive configuration process. For more information on manual setup, see the examples.
+
+```shell
+usage: pal weather [-h] [-s] [-l LOCATION] [-w]
+
+Weather information
+
+options:
+  -h, --help            show this help message and exit
+  -s, --search          Search location to get information from
+  -l LOCATION, --location LOCATION
+                        Location to get information from
+  -w, --window          Disables displaying weather information via a window
+```
```

### Comparing `sofapal-0.0.3/README.md` & `sofapal-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -9,28 +9,33 @@
 ```sh
 pip3 install -U sofapal
 ```
 
 #### Development
 
 ```sh
+# clone repository
 pip install -U git+https://github.com/slumberdemon/pal
+# create a virtual environment in the .venv directory
+python3 -m venv .venv
+# set up the current shell to use that virtual environment
+source .venv/bin/activate
 ```
 
 ### Why
 
 Pal is a command-line interface that includes a range of general features and functions. Pal is a personal exploration into creating a command-line interface using Python with aims to use as few dependencies as possible.
 
 ### How
 
 ```shell
 pal
 ```
 
-Pal loads configs from the `.pal` folder located in `$HOME`. Example configs can be found in the in [`.pal`](https://github.com/SlumberDemon/pal/tree/main/.pal). Therefore when adding/creating configurations make sure they are in that folder.
+Pal loads configs from the `.pal` folder located in `$HOME`. Example configs can be found in [`.pal`](https://github.com/SlumberDemon/pal/tree/main/.pal). Therefore when adding/creating configurations make sure they are in that folder.
 
 #### Create
 
 Pal enables for quick project creation using user-created templates. Templates are written in shell and are provided one argument.
 
 > Pal runs templates like this: `bash template.sh {name}`.
 
@@ -45,14 +50,16 @@
 This file is stored in the `templates` folder. In the example `$1` is used to access the name of the project provided by pal.
 
 It's recommended that the file name is in this format: `language-language-tool.sh`. This will make it easier to search for this template with pal.
 
 ```shell
 usage: pal create [-h] [-n NAME] [-e {zed,code}]
 
+Create project using a template
+
 options:
   -h, --help            show this help message and exit
   -n NAME, --name NAME  Name of the project
   -e {zed,code}, --editor {zed,code}
                         Code editor to open project with
 ```
 
@@ -89,7 +96,32 @@
 positional arguments:
   query
 
 options:
   -h, --help    show this help message and exit
   -e, --engine  Select engine to use
 ```
+
+#### Weather
+
+Pal can display information on the weather. Pal needs an [`weatherapi`](https://www.weatherapi.com) api key to do so.
+
+Setup for weather is easy and can be done with the following.
+
+```shell
+pal weather
+```
+
+Running with the command with no configs for the first time will start the interactive configuration process. For more information on manual setup, see the examples.
+
+```shell
+usage: pal weather [-h] [-s] [-l LOCATION] [-w]
+
+Weather information
+
+options:
+  -h, --help            show this help message and exit
+  -s, --search          Search location to get information from
+  -l LOCATION, --location LOCATION
+                        Location to get information from
+  -w, --window          Disables displaying weather information via a window
+```
```

### Comparing `sofapal-0.0.3/setup.py` & `sofapal-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 HERE = Path(__file__).parent
 README = (HERE / "README.md").read_text("utf-8")
 
 
 setup(
     name="sofapal",
-    version="0.0.3",
+    version="0.0.4",
     description="A friend; a chum.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/slumberdemon/pal",
     author="SlumberDemon",
     author_email="hi@sofa.sh",
     license="MIT",
@@ -24,19 +24,15 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     packages=find_packages(where="."),
-    install_requires=["inquirerpy"],
+    install_requires=["inquirerpy", "pytermgui"],
     package_dir={"": "."},
-    entry_points={
-        "console_scripts": [
-            "pal=pal.main:run",
-        ],
-    },
+    entry_points={"console_scripts": ["pal=pal.main:run",],},
     project_urls={
         "Bug Reports": "https://github.com/slumberdemon/pal/issues",
         "Source": "https://github.com/slumberdemon/pal",
     },
 )
```

### Comparing `sofapal-0.0.3/sofapal.egg-info/PKG-INFO` & `sofapal-0.0.4/sofapal.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sofapal
-Version: 0.0.3
+Version: 0.0.4
 Summary: A friend; a chum.
 Home-page: https://github.com/slumberdemon/pal
 Author: SlumberDemon
 Author-email: hi@sofa.sh
 License: MIT
 Project-URL: Bug Reports, https://github.com/slumberdemon/pal/issues
 Project-URL: Source, https://github.com/slumberdemon/pal
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: inquirerpy
+Requires-Dist: pytermgui
 
 # Pal
 
 A friend; a chum.
 
 ### Where
 
@@ -31,28 +32,33 @@
 ```sh
 pip3 install -U sofapal
 ```
 
 #### Development
 
 ```sh
+# clone repository
 pip install -U git+https://github.com/slumberdemon/pal
+# create a virtual environment in the .venv directory
+python3 -m venv .venv
+# set up the current shell to use that virtual environment
+source .venv/bin/activate
 ```
 
 ### Why
 
 Pal is a command-line interface that includes a range of general features and functions. Pal is a personal exploration into creating a command-line interface using Python with aims to use as few dependencies as possible.
 
 ### How
 
 ```shell
 pal
 ```
 
-Pal loads configs from the `.pal` folder located in `$HOME`. Example configs can be found in the in [`.pal`](https://github.com/SlumberDemon/pal/tree/main/.pal). Therefore when adding/creating configurations make sure they are in that folder.
+Pal loads configs from the `.pal` folder located in `$HOME`. Example configs can be found in [`.pal`](https://github.com/SlumberDemon/pal/tree/main/.pal). Therefore when adding/creating configurations make sure they are in that folder.
 
 #### Create
 
 Pal enables for quick project creation using user-created templates. Templates are written in shell and are provided one argument.
 
 > Pal runs templates like this: `bash template.sh {name}`.
 
@@ -67,14 +73,16 @@
 This file is stored in the `templates` folder. In the example `$1` is used to access the name of the project provided by pal.
 
 It's recommended that the file name is in this format: `language-language-tool.sh`. This will make it easier to search for this template with pal.
 
 ```shell
 usage: pal create [-h] [-n NAME] [-e {zed,code}]
 
+Create project using a template
+
 options:
   -h, --help            show this help message and exit
   -n NAME, --name NAME  Name of the project
   -e {zed,code}, --editor {zed,code}
                         Code editor to open project with
 ```
 
@@ -111,7 +119,32 @@
 positional arguments:
   query
 
 options:
   -h, --help    show this help message and exit
   -e, --engine  Select engine to use
 ```
+
+#### Weather
+
+Pal can display information on the weather. Pal needs an [`weatherapi`](https://www.weatherapi.com) api key to do so.
+
+Setup for weather is easy and can be done with the following.
+
+```shell
+pal weather
+```
+
+Running with the command with no configs for the first time will start the interactive configuration process. For more information on manual setup, see the examples.
+
+```shell
+usage: pal weather [-h] [-s] [-l LOCATION] [-w]
+
+Weather information
+
+options:
+  -h, --help            show this help message and exit
+  -s, --search          Search location to get information from
+  -l LOCATION, --location LOCATION
+                        Location to get information from
+  -w, --window          Disables displaying weather information via a window
+```
```

