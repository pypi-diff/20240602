# Comparing `tmp/btrievepython-16.0.62.0.tar.gz` & `tmp/btrievepython-16.0.66.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrievepython-16.0.62.0.tar", last modified: Fri May 10 18:37:19 2024, max compression
+gzip compressed data, was "btrievepython-16.0.66.0.tar", last modified: Sat Jun  1 02:55:49 2024, max compression
```

## Comparing `btrievepython-16.0.62.0.tar` & `btrievepython-16.0.66.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 18:37:19.880313 btrievepython-16.0.62.0/
--rw-rw-rw-   0        0        0     1065 2024-05-10 16:53:44.000000 btrievepython-16.0.62.0/LICENSE.txt
--rw-rw-rw-   0        0        0       35 2024-05-10 16:53:44.000000 btrievepython-16.0.62.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2286 2024-05-10 18:37:19.880313 btrievepython-16.0.62.0/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-05-10 16:53:44.000000 btrievepython-16.0.62.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 18:37:19.876302 btrievepython-16.0.62.0/btrievePython/
--rw-rw-rw-   0        0        0   100785 2024-05-10 17:01:34.000000 btrievepython-16.0.62.0/btrievePython/__init__.py
--rw-rw-rw-   0        0        0   211140 2024-05-10 16:52:26.000000 btrievepython-16.0.62.0/btrievePython/btrieveC.h
--rw-rw-rw-   0        0        0   234858 2024-05-10 16:52:26.000000 btrievepython-16.0.62.0/btrievePython/btrieveCpp.h
--rw-rw-rw-   0        0        0   826683 2024-05-10 17:01:34.000000 btrievepython-16.0.62.0/btrievePython/btrievePython.cpp
-drwxrwxrwx   0        0        0        0 2024-05-10 18:37:19.878307 btrievepython-16.0.62.0/btrievePython/win32/
--rw-rw-rw-   0        0        0   178794 2024-05-10 17:01:14.000000 btrievepython-16.0.62.0/btrievePython/win32/btrieveCpp.lib
-drwxrwxrwx   0        0        0        0 2024-05-10 18:37:19.879320 btrievepython-16.0.62.0/btrievePython/win64/
--rw-rw-rw-   0        0        0   181814 2024-05-10 17:01:30.000000 btrievepython-16.0.62.0/btrievePython/win64/btrieveCpp.lib
-drwxrwxrwx   0        0        0        0 2024-05-10 18:37:19.879320 btrievepython-16.0.62.0/btrievePython.egg-info/
--rw-rw-rw-   0        0        0     2286 2024-05-10 18:37:19.000000 btrievepython-16.0.62.0/btrievePython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2024-05-10 18:37:19.000000 btrievepython-16.0.62.0/btrievePython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 18:37:19.000000 btrievepython-16.0.62.0/btrievePython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 18:37:19.000000 btrievepython-16.0.62.0/btrievePython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      886 2024-05-10 16:53:44.000000 btrievepython-16.0.62.0/pyproject.toml
--rw-rw-rw-   0        0        0      301 2024-05-10 18:37:19.880313 btrievepython-16.0.62.0/setup.cfg
--rw-rw-rw-   0        0        0     3965 2024-05-10 16:53:44.000000 btrievepython-16.0.62.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:55:49.154536 btrievepython-16.0.66.0/
+-rw-rw-rw-   0        0        0    44220 2024-06-01 02:31:28.000000 btrievepython-16.0.66.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       35 2024-06-01 01:06:18.000000 btrievepython-16.0.66.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    46895 2024-06-01 02:55:49.154536 btrievepython-16.0.66.0/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-06-01 01:06:18.000000 btrievepython-16.0.66.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 02:55:49.148535 btrievepython-16.0.66.0/btrievePython/
+-rw-rw-rw-   0        0        0   100785 2024-06-01 01:14:24.000000 btrievepython-16.0.66.0/btrievePython/__init__.py
+-rw-rw-rw-   0        0        0   211140 2024-06-01 01:05:00.000000 btrievepython-16.0.66.0/btrievePython/btrieveC.h
+-rw-rw-rw-   0        0        0   234858 2024-06-01 01:05:00.000000 btrievepython-16.0.66.0/btrievePython/btrieveCpp.h
+-rw-rw-rw-   0        0        0   826683 2024-06-01 01:14:24.000000 btrievepython-16.0.66.0/btrievePython/btrievePython.cpp
+drwxrwxrwx   0        0        0        0 2024-06-01 02:55:49.151535 btrievepython-16.0.66.0/btrievePython/win32/
+-rw-rw-rw-   0        0        0   178794 2024-06-01 01:14:08.000000 btrievepython-16.0.66.0/btrievePython/win32/btrieveCpp.lib
+drwxrwxrwx   0        0        0        0 2024-06-01 02:55:49.152535 btrievepython-16.0.66.0/btrievePython/win64/
+-rw-rw-rw-   0        0        0   181814 2024-06-01 01:14:20.000000 btrievepython-16.0.66.0/btrievePython/win64/btrieveCpp.lib
+drwxrwxrwx   0        0        0        0 2024-06-01 02:55:49.153535 btrievepython-16.0.66.0/btrievePython.egg-info/
+-rw-rw-rw-   0        0        0    46895 2024-06-01 02:55:49.000000 btrievepython-16.0.66.0/btrievePython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-06-01 02:55:49.000000 btrievepython-16.0.66.0/btrievePython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 02:55:49.000000 btrievepython-16.0.66.0/btrievePython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-06-01 02:55:49.000000 btrievepython-16.0.66.0/btrievePython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      884 2024-06-01 01:06:18.000000 btrievepython-16.0.66.0/pyproject.toml
+-rw-rw-rw-   0        0        0      309 2024-06-01 02:55:49.155536 btrievepython-16.0.66.0/setup.cfg
+-rw-rw-rw-   0        0        0     4076 2024-06-01 01:06:18.000000 btrievepython-16.0.66.0/setup.py
```

### Comparing `btrievepython-16.0.62.0/btrievePython/__init__.py` & `btrievepython-16.0.66.0/btrievePython/__init__.py`

 * *Files identical despite different names*

### Comparing `btrievepython-16.0.62.0/btrievePython/btrieveC.h` & `btrievepython-16.0.66.0/btrievePython/btrieveC.h`

 * *Files identical despite different names*

### Comparing `btrievepython-16.0.62.0/btrievePython/btrieveCpp.h` & `btrievepython-16.0.66.0/btrievePython/btrieveCpp.h`

 * *Files identical despite different names*

### Comparing `btrievepython-16.0.62.0/btrievePython/btrievePython.cpp` & `btrievepython-16.0.66.0/btrievePython/btrievePython.cpp`

 * *Files identical despite different names*

### Comparing `btrievepython-16.0.62.0/btrievePython/win32/btrieveCpp.lib` & `btrievepython-16.0.66.0/btrievePython/win32/btrieveCpp.lib`

 * *Files identical despite different names*

### Comparing `btrievepython-16.0.62.0/btrievePython/win64/btrieveCpp.lib` & `btrievepython-16.0.66.0/btrievePython/win64/btrieveCpp.lib`

 * *Files identical despite different names*

### Comparing `btrievepython-16.0.62.0/pyproject.toml` & `btrievepython-16.0.66.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = 'btrievePython'
-version = '16.00.062.000'
+version = '16.00.066.000'
 authors = [ { name = 'Actian Corporation' }, { email = 'community.admin@actian.com' } ]
 description = 'Btrieve Python provides a Client API for Actian Zen'
 readme = 'README.md'
 requires-python = '>=3.7'
 classifiers = [
-   'License :: OSI Approved :: MIT License',
+   'License :: Other/Proprietary License',
    #'Operating System :: Android',
    'Operating System :: MacOS',
    'Operating System :: Microsoft :: Windows',
    'Operating System :: POSIX :: Linux',
    #'Operating System :: iOS',
    'Programming Language :: C++',
    'Programming Language :: Python :: 3'
```

### Comparing `btrievepython-16.0.62.0/setup.py` & `btrievepython-16.0.66.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,40 +69,43 @@
         zenLibraryDir += '/lib'                        # /usr/local/actianzen/lib
     else:
         print(unableToLocate)
         exit(1)
 
 if (platform == 'win64'):
     setup(
+        packages=['btrievePython'],
         ext_modules = [
             Extension(
                 name = 'btrievePython._btrievePython',
                 sources = [ 'btrievePython/btrievePython.cpp' ],
                 library_dirs = [ 'btrievePython/win64', zenLibraryDir ],
                 # Not currently supported on Windows.  
                 #runtime_library_dirs = [ zenLibraryDir ],
                 libraries = [ 'btrieveCpp' ]
             )
         ]
     )
 elif (platform == 'win32'):
     setup(
+        packages=['btrievePython'],
         ext_modules = [
             Extension(
                 name = 'btrievePython._btrievePython',
                 sources = [ 'btrievePython/btrievePython.cpp' ],
                 library_dirs = [ 'btrievePython/win32', zenLibraryDir ],
                 # Not currently supported on Windows.  
                 #runtime_library_dirs = [ zenLibraryDir ],
                 libraries = [ 'btrieveCpp' ]
             )
         ]
     )
 else:
     setup(
+        packages=['btrievePython'],
         ext_modules = [
             Extension(
                 name = 'btrievePython._btrievePython',
                 sources = [ 'btrievePython/btrievePython.cpp' ],
                 library_dirs = [ 'btrievePython', zenLibraryDir ],
                 runtime_library_dirs = [ zenLibraryDir ],
                 libraries = [ 'btrieveCpp' ]
```

