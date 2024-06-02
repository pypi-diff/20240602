# Comparing `tmp/silvermirror-0.4.tar.gz` & `tmp/silvermirror-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silvermirror-0.4.tar", last modified: Fri Aug 13 22:17:04 2021, max compression
+gzip compressed data, was "silvermirror-0.5.tar", last modified: Sun Jun  2 20:31:08 2024, max compression
```

## Comparing `silvermirror-0.4.tar` & `silvermirror-0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2021-08-13 22:17:04.602450 silvermirror-0.4/
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      259 2021-08-13 22:17:04.602450 silvermirror-0.4/PKG-INFO
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       38 2021-08-13 22:17:04.602450 silvermirror-0.4/setup.cfg
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      839 2021-08-13 22:15:54.000000 silvermirror-0.4/setup.py
-drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2021-08-13 22:17:04.602450 silvermirror-0.4/silvermirror/
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        2 2021-04-24 21:46:04.000000 silvermirror-0.4/silvermirror/__init__.py
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     2292 2021-04-24 21:46:04.000000 silvermirror-0.4/silvermirror/config.py
--rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)     2546 2021-04-24 21:46:04.000000 silvermirror-0.4/silvermirror/hg.py
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      841 2021-04-24 21:46:04.000000 silvermirror-0.4/silvermirror/interface.py
--rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)     6469 2021-08-13 22:12:15.000000 silvermirror-0.4/silvermirror/unify.py
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      800 2021-04-24 22:10:07.000000 silvermirror-0.4/silvermirror/unison.py
--rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)      736 2021-04-24 21:46:04.000000 silvermirror-0.4/silvermirror/utils.py
-drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2021-08-13 22:17:04.602450 silvermirror-0.4/silvermirror.egg-info/
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      259 2021-08-13 22:17:04.000000 silvermirror-0.4/silvermirror.egg-info/PKG-INFO
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      440 2021-08-13 22:17:04.000000 silvermirror-0.4/silvermirror.egg-info/SOURCES.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2021-08-13 22:17:04.000000 silvermirror-0.4/silvermirror.egg-info/dependency_links.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      220 2021-08-13 22:17:04.000000 silvermirror-0.4/silvermirror.egg-info/entry_points.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2021-04-24 21:50:35.000000 silvermirror-0.4/silvermirror.egg-info/not-zip-safe
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       44 2021-08-13 22:17:04.000000 silvermirror-0.4/silvermirror.egg-info/requires.txt
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       13 2021-08-13 22:17:04.000000 silvermirror-0.4/silvermirror.egg-info/top_level.txt
-drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2021-08-13 22:17:04.602450 silvermirror-0.4/test/
--rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      214 2021-08-13 22:14:53.000000 silvermirror-0.4/test/test_unify.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:31:08.004940 silvermirror-0.5/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      248 2024-06-02 20:31:08.004940 silvermirror-0.5/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       38 2024-06-02 20:31:08.004940 silvermirror-0.5/setup.cfg
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      806 2024-06-02 20:30:38.000000 silvermirror-0.5/setup.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:31:08.004940 silvermirror-0.5/silvermirror/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        2 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/__init__.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)     2292 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/config.py
+-rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)     2557 2024-06-02 20:28:40.000000 silvermirror-0.5/silvermirror/hg.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      841 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/interface.py
+-rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)     6469 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/unify.py
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      800 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/unison.py
+-rwxrwxr-x   0 jhammel   (1000) jhammel   (1000)      736 2024-04-12 14:19:20.000000 silvermirror-0.5/silvermirror/utils.py
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:31:08.004940 silvermirror-0.5/silvermirror.egg-info/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      248 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/PKG-INFO
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      440 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/SOURCES.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/dependency_links.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      220 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/entry_points.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)        1 2024-04-12 14:45:45.000000 silvermirror-0.5/silvermirror.egg-info/not-zip-safe
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       44 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/requires.txt
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)       13 2024-06-02 20:31:07.000000 silvermirror-0.5/silvermirror.egg-info/top_level.txt
+drwxrwxr-x   0 jhammel   (1000) jhammel   (1000)        0 2024-06-02 20:31:08.004940 silvermirror-0.5/test/
+-rw-rw-r--   0 jhammel   (1000) jhammel   (1000)      214 2024-04-12 14:19:20.000000 silvermirror-0.5/test/test_unify.py
```

### Comparing `silvermirror-0.4/setup.py` & `silvermirror-0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from setuptools import setup
 
-version = '0.4'
+version = '0.5'
 
 setup(name='silvermirror',
       version=version,
       description="mirror files across hosts",
-      long_description="""\
-""",
       classifiers=[],
       keywords='mirror unison',
       author='Jeff Hammel',
       author_email='k0scist@gmail.com',
       url='http://k0s.org/hg/silvermirror',
       license='GPL',
       packages=['silvermirror'],
```

### Comparing `silvermirror-0.4/silvermirror/config.py` & `silvermirror-0.5/silvermirror/config.py`

 * *Files identical despite different names*

### Comparing `silvermirror-0.4/silvermirror/hg.py` & `silvermirror-0.5/silvermirror/hg.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,20 +73,20 @@
     # kill trailing slash
     options.host = options.host.rstrip('/')
 
     # get repositories
     repos = repositories(options.host)
     if options.list:
         for repo in repos:
-            print repo
-        sys.exit(0)
+            print(repo)
+        return
 
     # clone/update repos to directory
     if not os.path.exists(options.directory):
         os.mkdir(options.directory)
     for repo in repos:
         source = '{}/{}'.format(options.host, repo)
         dest = os.path.join(options.directory, repo)
         update(source, dest)
 
 if __name__ == '__main__':
-    main()
+    sys.exit(main() or 0)
```

### Comparing `silvermirror-0.4/silvermirror/interface.py` & `silvermirror-0.5/silvermirror/interface.py`

 * *Files identical despite different names*

### Comparing `silvermirror-0.4/silvermirror/unify.py` & `silvermirror-0.5/silvermirror/unify.py`

 * *Files identical despite different names*

### Comparing `silvermirror-0.4/silvermirror/unison.py` & `silvermirror-0.5/silvermirror/unison.py`

 * *Files identical despite different names*

### Comparing `silvermirror-0.4/silvermirror/utils.py` & `silvermirror-0.5/silvermirror/utils.py`

 * *Files identical despite different names*

