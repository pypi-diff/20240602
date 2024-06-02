# Comparing `tmp/rolyson-0.1.tar.gz` & `tmp/rolyson-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rolyson-0.1.tar", last modified: Sun Jun  2 00:22:11 2024, max compression
+gzip compressed data, was "dist\rolyson-0.2.tar", last modified: Sun Jun  2 00:55:31 2024, max compression
```

## Comparing `rolyson-0.1.tar` & `rolyson-0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 00:22:11.000000 rolyson-0.1/
--rw-rw-rw-   0        0        0      517 2024-06-02 00:22:11.000000 rolyson-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-06-02 00:12:37.000000 rolyson-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 00:22:11.000000 rolyson-0.1/rolyson/
--rw-rw-rw-   0        0        0        0 2024-06-01 23:47:00.000000 rolyson-0.1/rolyson/__init__.py
--rw-rw-rw-   0        0        0       37 2024-06-01 23:47:51.000000 rolyson-0.1/rolyson/hello.py
-drwxrwxrwx   0        0        0        0 2024-06-02 00:22:11.000000 rolyson-0.1/rolyson.egg-info/
--rw-rw-rw-   0        0        0      517 2024-06-02 00:22:11.000000 rolyson-0.1/rolyson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-06-02 00:22:11.000000 rolyson-0.1/rolyson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 00:22:11.000000 rolyson-0.1/rolyson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-06-02 00:22:11.000000 rolyson-0.1/rolyson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 00:22:11.000000 rolyson-0.1/setup.cfg
--rw-rw-rw-   0        0        0      745 2024-06-02 00:13:05.000000 rolyson-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 00:55:31.000000 rolyson-0.2/
+-rw-rw-rw-   0        0        0      642 2024-06-02 00:55:31.000000 rolyson-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2024-06-02 00:55:19.000000 rolyson-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 00:55:31.000000 rolyson-0.2/rolyson/
+-rw-rw-rw-   0        0        0        0 2024-06-01 23:47:00.000000 rolyson-0.2/rolyson/__init__.py
+-rw-rw-rw-   0        0        0       37 2024-06-01 23:47:51.000000 rolyson-0.2/rolyson/hello.py
+-rw-rw-rw-   0        0        0     1900 2024-06-02 00:54:15.000000 rolyson-0.2/rolyson/validate.py
+drwxrwxrwx   0        0        0        0 2024-06-02 00:55:31.000000 rolyson-0.2/rolyson.egg-info/
+-rw-rw-rw-   0        0        0      642 2024-06-02 00:55:31.000000 rolyson-0.2/rolyson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2024-06-02 00:55:31.000000 rolyson-0.2/rolyson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 00:55:31.000000 rolyson-0.2/rolyson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 00:55:31.000000 rolyson-0.2/rolyson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 00:55:31.000000 rolyson-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      745 2024-06-02 00:55:12.000000 rolyson-0.2/setup.py
```

### Comparing `rolyson-0.1/PKG-INFO` & `rolyson-0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: rolyson
-Version: 0.1
+Version: 0.2
 Summary: Biblioteca de funções comuns para meus projetos Django
 Home-page: https://github.com/Rolyson/lib-rolyson
 Author: Rolyson
 Author-email: rolysonrocha@gmail.com
 License: UNKNOWN
 Description: Minha biblioteca
         
+        
+        pip install twine wheel
+        python setup.py sdist bdist_wheel
+        twine upload dist/*
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `rolyson-0.1/rolyson.egg-info/PKG-INFO` & `rolyson-0.2/rolyson.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: rolyson
-Version: 0.1
+Version: 0.2
 Summary: Biblioteca de funções comuns para meus projetos Django
 Home-page: https://github.com/Rolyson/lib-rolyson
 Author: Rolyson
 Author-email: rolysonrocha@gmail.com
 License: UNKNOWN
 Description: Minha biblioteca
         
+        
+        pip install twine wheel
+        python setup.py sdist bdist_wheel
+        twine upload dist/*
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `rolyson-0.1/setup.py` & `rolyson-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rolyson',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         # Adicione aqui as dependências, se houver
     ],
     description='Biblioteca de funções comuns para meus projetos Django',
     long_description=open('README.md').read(),
```

