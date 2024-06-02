# Comparing `tmp/mkdocs-juvix-plugin-0.2.4.tar.gz` & `tmp/mkdocs-juvix-plugin-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-juvix-plugin-0.2.4.tar", last modified: Fri Apr 26 18:18:24 2024, max compression
+gzip compressed data, was "mkdocs-juvix-plugin-0.2.5.tar", last modified: Sun Jun  2 12:29:35 2024, max compression
```

## Comparing `mkdocs-juvix-plugin-0.2.4.tar` & `mkdocs-juvix-plugin-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-26 18:18:24.742816 mkdocs-juvix-plugin-0.2.4/
--rw-r--r--   0 jonaprieto   (501) staff       (20)      493 2024-04-26 18:18:24.742538 mkdocs-juvix-plugin-0.2.4/PKG-INFO
--rw-r--r--   0 jonaprieto   (501) staff       (20)     1882 2024-04-19 12:50:37.000000 mkdocs-juvix-plugin-0.2.4/README.md
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-26 18:18:24.741084 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix/
--rw-r--r--   0 jonaprieto   (501) staff       (20)        0 2023-10-30 14:15:49.000000 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix/__init__.py
--rw-r--r--   0 jonaprieto   (501) staff       (20)    18591 2024-04-26 18:16:38.000000 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix/plugin.py
--rw-r--r--   0 jonaprieto   (501) staff       (20)     3364 2024-04-17 09:42:21.000000 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix/standalone.py
--rw-r--r--   0 jonaprieto   (501) staff       (20)     2438 2024-04-17 09:46:29.000000 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix/utils.py
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-04-26 18:18:24.742251 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix_plugin.egg-info/
--rw-r--r--   0 jonaprieto   (501) staff       (20)      493 2024-04-26 18:18:24.000000 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix_plugin.egg-info/PKG-INFO
--rw-r--r--   0 jonaprieto   (501) staff       (20)      375 2024-04-26 18:18:24.000000 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)        1 2024-04-26 18:18:24.000000 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)      107 2024-04-26 18:18:24.000000 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix_plugin.egg-info/entry_points.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       40 2024-04-26 18:18:24.000000 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix_plugin.egg-info/requires.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       13 2024-04-26 18:18:24.000000 mkdocs-juvix-plugin-0.2.4/mkdocs_juvix_plugin.egg-info/top_level.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       38 2024-04-26 18:18:24.742876 mkdocs-juvix-plugin-0.2.4/setup.cfg
--rw-r--r--   0 jonaprieto   (501) staff       (20)      827 2024-04-26 18:18:08.000000 mkdocs-juvix-plugin-0.2.4/setup.py
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-06-02 12:29:35.463801 mkdocs-juvix-plugin-0.2.5/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      492 2024-06-02 12:29:35.463513 mkdocs-juvix-plugin-0.2.5/PKG-INFO
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     1882 2024-06-02 12:26:54.000000 mkdocs-juvix-plugin-0.2.5/README.md
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-06-02 12:29:35.461418 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)        0 2023-10-30 14:15:49.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/__init__.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)    18558 2024-06-02 12:26:54.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/plugin.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     3364 2024-06-02 12:26:54.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/standalone.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     2438 2024-06-02 12:26:54.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/utils.py
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-06-02 12:29:35.463175 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      492 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      375 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)        1 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      107 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       40 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/requires.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       13 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/top_level.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       38 2024-06-02 12:29:35.463856 mkdocs-juvix-plugin-0.2.5/setup.cfg
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      826 2024-06-02 12:29:06.000000 mkdocs-juvix-plugin-0.2.5/setup.py
```

### Comparing `mkdocs-juvix-plugin-0.2.4/README.md` & `mkdocs-juvix-plugin-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-juvix-plugin-0.2.4/mkdocs_juvix/plugin.py` & `mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,21 +112,19 @@
         if not self.JUVIX_AVAILABLE:
             log.info(
                 "Juvix is not available on the system. check the JUVIX_BIN environment variable."
             )
 
         return config
 
-    def on_files(self, _files: Files, *, config: MkDocsConfig) -> Optional[Files]:
-
-        files = []
-        for file in _files:
-            if not ".juvix-build" in file.abs_src_path:
-                files.append(file)
-        return Files(files)
+    def on_files(self, files: Files, *, config: MkDocsConfig) -> Optional[Files]:
+        for file in files:
+            if ".juvix-build" in file.abs_src_path:
+                files.remove(file)
+        return files
 
     def on_page_read_source(self, page: Page, config: MkDocsConfig) -> Optional[str]:
 
         filepath = Path(page.file.abs_src_path)
 
         if not filepath.as_posix().endswith(".juvix.md"):
             return None
```

### Comparing `mkdocs-juvix-plugin-0.2.4/mkdocs_juvix/standalone.py` & `mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/standalone.py`

 * *Files identical despite different names*

### Comparing `mkdocs-juvix-plugin-0.2.4/mkdocs_juvix/utils.py` & `mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs-juvix-plugin-0.2.4/setup.py` & `mkdocs-juvix-plugin-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import find_packages, setup
 
 setup(
     name="mkdocs-juvix-plugin",
-    version="0.2.4",
+    version="0.2.5",
     description="A plugin to render Juvix code blocks in MkDocs.",
     long_description="",
     keywords="mkdocs",
     author="Jonathan Prieto-Cubides, and GitHub contributors",
     author_email="jonathan@heliax.dev",
     license="MIT",
-    python_requires=">=3.11",
+    python_requires=">=3.9",
     install_requires=["mkdocs >= 1.5.0", "pyYaml", "pymdown-extensions"],
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Programming Language :: Python",
     ],
     packages=find_packages(),
```

