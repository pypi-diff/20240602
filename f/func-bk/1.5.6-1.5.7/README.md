# Comparing `tmp/func_bk-1.5.6.tar.gz` & `tmp/func_bk-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_bk-1.5.6.tar", last modified: Sat Jun  1 16:05:23 2024, max compression
+gzip compressed data, was "func_bk-1.5.7.tar", last modified: Sat Jun  1 16:13:55 2024, max compression
```

## Comparing `func_bk-1.5.6.tar` & `func_bk-1.5.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 16:05:23.480341 func_bk-1.5.6/
--rw-rw-rw-   0        0        0     3482 2024-06-01 16:05:23.480341 func_bk-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2024-06-01 12:58:41.000000 func_bk-1.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 16:05:23.474339 func_bk-1.5.6/func_bk/
--rw-rw-rw-   0        0        0     2574 2024-06-01 12:17:14.000000 func_bk-1.5.6/func_bk/__init__.py
--rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.5.6/func_bk/django.py
--rw-rw-rw-   0        0        0     3603 2024-06-01 16:04:01.000000 func_bk-1.5.6/func_bk/fast_api.py
-drwxrwxrwx   0        0        0        0 2024-06-01 16:05:23.479339 func_bk-1.5.6/func_bk.egg-info/
--rw-rw-rw-   0        0        0     3482 2024-06-01 16:05:23.000000 func_bk-1.5.6/func_bk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-06-01 16:05:23.000000 func_bk-1.5.6/func_bk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 16:05:23.000000 func_bk-1.5.6/func_bk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-06-01 16:05:23.000000 func_bk-1.5.6/func_bk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-06-01 16:05:23.000000 func_bk-1.5.6/func_bk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-06-01 16:05:23.481342 func_bk-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-06-01 12:17:34.000000 func_bk-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:13:55.040236 func_bk-1.5.7/
+-rw-rw-rw-   0        0        0     3482 2024-06-01 16:13:55.039236 func_bk-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2024-06-01 12:58:41.000000 func_bk-1.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 16:13:55.033235 func_bk-1.5.7/func_bk/
+-rw-rw-rw-   0        0        0     2574 2024-06-01 12:17:14.000000 func_bk-1.5.7/func_bk/__init__.py
+-rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.5.7/func_bk/django.py
+-rw-rw-rw-   0        0        0     3683 2024-06-01 16:13:51.000000 func_bk-1.5.7/func_bk/fast_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 16:13:55.039236 func_bk-1.5.7/func_bk.egg-info/
+-rw-rw-rw-   0        0        0     3482 2024-06-01 16:13:54.000000 func_bk-1.5.7/func_bk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-06-01 16:13:54.000000 func_bk-1.5.7/func_bk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 16:13:54.000000 func_bk-1.5.7/func_bk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-06-01 16:13:54.000000 func_bk-1.5.7/func_bk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-06-01 16:13:54.000000 func_bk-1.5.7/func_bk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-06-01 16:13:55.041235 func_bk-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-06-01 12:17:34.000000 func_bk-1.5.7/setup.py
```

### Comparing `func_bk-1.5.6/PKG-INFO` & `func_bk-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.5.6
+Version: 1.5.7
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

### Comparing `func_bk-1.5.6/README.md` & `func_bk-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `func_bk-1.5.6/func_bk/__init__.py` & `func_bk-1.5.7/func_bk/__init__.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.5.6/func_bk/django.py` & `func_bk-1.5.7/func_bk/django.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.5.6/func_bk/fast_api.py` & `func_bk-1.5.7/func_bk/fast_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,28 +75,29 @@
 
 class Label():
     type: str
     id: str
     placeholder: str
     help_text: str
     style_input:str
-    def __init__(self,atype,aid,place = None,help = None,style = None):
+    def __init__(self,atype:str,aid:str,place:str = None,help:str = None,style:str = None):
         self.type=atype
         self.id=aid
         self.placeholder=place
         self.help_text=help
         self.style_input=style
 
 
-
 class BForm():
     def labels(self):
         a=[]
-        for i in type(self).__dict__.items():
-            a.append(i)
+        cls=type(self)
+        for i in cls.__dict__.items():
+            if isinstance(i, Label):
+                a.append(i)   
         return a
 
     def as_p(self):
         a=''
         all=self.labels()
 
         for i in all:
```

### Comparing `func_bk-1.5.6/func_bk.egg-info/PKG-INFO` & `func_bk-1.5.7/func_bk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.5.6
+Version: 1.5.7
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

