# Comparing `tmp/hugo-0.126.2.tar.gz` & `tmp/hugo-0.126.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugo-0.126.2.tar", last modified: Thu May 30 17:24:22 2024, max compression
+gzip compressed data, was "hugo-0.126.3.tar", last modified: Sun Jun  2 15:05:03 2024, max compression
```

## Comparing `hugo-0.126.2.tar` & `hugo-0.126.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:24:22.416744 hugo-0.126.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-30 17:24:18.000000 hugo-0.126.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 17:24:18.000000 hugo-0.126.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 17:24:18.000000 hugo-0.126.2/LICENSE-hugo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-30 17:24:18.000000 hugo-0.126.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-30 17:24:22.416744 hugo-0.126.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-05-30 17:24:18.000000 hugo-0.126.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-30 17:24:18.000000 hugo-0.126.2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:24:22.412744 hugo-0.126.2/hugo/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-30 17:24:18.000000 hugo-0.126.2/hugo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:24:22.416744 hugo-0.126.2/hugo/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 17:24:18.000000 hugo-0.126.2/hugo/binaries/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-30 17:24:18.000000 hugo-0.126.2/hugo/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:24:22.416744 hugo-0.126.2/hugo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-30 17:24:22.000000 hugo-0.126.2/hugo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 17:24:22.000000 hugo-0.126.2/hugo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:24:22.000000 hugo-0.126.2/hugo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 17:24:22.000000 hugo-0.126.2/hugo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 17:24:22.000000 hugo-0.126.2/hugo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-30 17:24:18.000000 hugo-0.126.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-30 17:24:22.416744 hugo-0.126.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-30 17:24:18.000000 hugo-0.126.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:05:03.932143 hugo-0.126.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-06-02 15:04:57.000000 hugo-0.126.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-02 15:04:57.000000 hugo-0.126.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-02 15:04:57.000000 hugo-0.126.3/LICENSE-hugo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-06-02 15:04:57.000000 hugo-0.126.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-06-02 15:05:03.932143 hugo-0.126.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-06-02 15:04:57.000000 hugo-0.126.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-06-02 15:04:57.000000 hugo-0.126.3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:05:03.932143 hugo-0.126.3/hugo/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-06-02 15:04:57.000000 hugo-0.126.3/hugo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:05:03.932143 hugo-0.126.3/hugo/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-02 15:04:57.000000 hugo-0.126.3/hugo/binaries/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-06-02 15:04:57.000000 hugo-0.126.3/hugo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:05:03.932143 hugo-0.126.3/hugo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-06-02 15:05:03.000000 hugo-0.126.3/hugo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-06-02 15:05:03.000000 hugo-0.126.3/hugo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:05:03.000000 hugo-0.126.3/hugo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 15:05:03.000000 hugo-0.126.3/hugo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-02 15:05:03.000000 hugo-0.126.3/hugo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-06-02 15:04:57.000000 hugo-0.126.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-02 15:05:03.932143 hugo-0.126.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-06-02 15:04:57.000000 hugo-0.126.3/setup.py
```

### Comparing `hugo-0.126.2/CODE_OF_CONDUCT.md` & `hugo-0.126.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hugo-0.126.2/LICENSE` & `hugo-0.126.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hugo-0.126.2/LICENSE-hugo.txt` & `hugo-0.126.3/LICENSE-hugo.txt`

 * *Files identical despite different names*

### Comparing `hugo-0.126.2/PKG-INFO` & `hugo-0.126.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugo
-Version: 0.126.2
+Version: 0.126.3
 Summary: Binaries for the Hugo static site generator, installable with pip
 Author-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 Maintainer-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/agriyakhetarpal/hugo-python-distributions
 Project-URL: Issues, https://github.com/agriyakhetarpal/hugo-python-distributions/issues
 Project-URL: Changelog, https://github.com/agriyakhetarpal/hugo-python-distributions/releases
```

### Comparing `hugo-0.126.2/README.md` & `hugo-0.126.3/README.md`

 * *Files identical despite different names*

### Comparing `hugo-0.126.2/SECURITY.md` & `hugo-0.126.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `hugo-0.126.2/hugo/cli.py` & `hugo-0.126.3/hugo/cli.py`

 * *Files identical despite different names*

### Comparing `hugo-0.126.2/hugo.egg-info/PKG-INFO` & `hugo-0.126.3/hugo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugo
-Version: 0.126.2
+Version: 0.126.3
 Summary: Binaries for the Hugo static site generator, installable with pip
 Author-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 Maintainer-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/agriyakhetarpal/hugo-python-distributions
 Project-URL: Issues, https://github.com/agriyakhetarpal/hugo-python-distributions/issues
 Project-URL: Changelog, https://github.com/agriyakhetarpal/hugo-python-distributions/releases
```

### Comparing `hugo-0.126.2/pyproject.toml` & `hugo-0.126.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hugo-0.126.2/setup.py` & `hugo-0.126.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import Command, Extension, setup
 from setuptools.command.build_ext import build_ext
 from setuptools.command.build_py import build_py
 from wheel.bdist_wheel import bdist_wheel
 
 # ------ Hugo build configuration and constants ------------------------------------
 
-HUGO_VERSION = "0.126.2"
+HUGO_VERSION = "0.126.3"
 # The Go toolchain will download the tarball into the hugo_cache/ directory.
 # We will point the build command to that location to build Hugo from source
 HUGO_CACHE_DIR = "hugo_cache"
 FILE_EXT = (
     ".exe" if (sys.platform == "win32" or os.environ.get("GOOS") == "windows") else ""
 )
 # The vendor name is used to set the vendorInfo variable in the Hugo binary
```

