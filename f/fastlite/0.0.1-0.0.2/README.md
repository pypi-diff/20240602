# Comparing `tmp/fastlite-0.0.1.tar.gz` & `tmp/fastlite-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlite-0.0.1.tar", last modified: Mon May 27 21:53:51 2024, max compression
+gzip compressed data, was "fastlite-0.0.2.tar", last modified: Sun Jun  2 04:59:40 2024, max compression
```

## Comparing `fastlite-0.0.1.tar` & `fastlite-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-27 21:53:51.696921 fastlite-0.0.1/
--rw-r--r--   0 jhoward    (501) staff       (20)    11357 2024-05-27 00:04:24.000000 fastlite-0.0.1/LICENSE
--rw-rw-r--   0 jhoward    (501) staff       (20)      111 2024-05-27 17:26:46.000000 fastlite-0.0.1/MANIFEST.in
--rw-r--r--   0 jhoward    (501) staff       (20)     1082 2024-05-27 21:53:51.696727 fastlite-0.0.1/PKG-INFO
--rw-r--r--   0 jhoward    (501) staff       (20)      287 2024-05-27 17:26:46.000000 fastlite-0.0.1/README.md
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-27 21:53:51.695474 fastlite-0.0.1/fastlite/
--rw-r--r--   0 jhoward    (501) staff       (20)       42 2024-05-27 18:13:46.000000 fastlite-0.0.1/fastlite/__init__.py
--rw-r--r--   0 jhoward    (501) staff       (20)     3804 2024-05-27 19:11:08.000000 fastlite-0.0.1/fastlite/_modidx.py
--rw-r--r--   0 jhoward    (501) staff       (20)     3267 2024-05-27 18:13:46.000000 fastlite-0.0.1/fastlite/core.py
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-27 21:53:51.696495 fastlite-0.0.1/fastlite.egg-info/
--rw-r--r--   0 jhoward    (501) staff       (20)     1082 2024-05-27 21:53:51.000000 fastlite-0.0.1/fastlite.egg-info/PKG-INFO
--rw-r--r--   0 jhoward    (501) staff       (20)      334 2024-05-27 21:53:51.000000 fastlite-0.0.1/fastlite.egg-info/SOURCES.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-27 21:53:51.000000 fastlite-0.0.1/fastlite.egg-info/dependency_links.txt
--rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-05-27 21:53:51.000000 fastlite-0.0.1/fastlite.egg-info/entry_points.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-27 17:28:08.000000 fastlite-0.0.1/fastlite.egg-info/not-zip-safe
--rw-r--r--   0 jhoward    (501) staff       (20)       37 2024-05-27 21:53:51.000000 fastlite-0.0.1/fastlite.egg-info/requires.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        9 2024-05-27 21:53:51.000000 fastlite-0.0.1/fastlite.egg-info/top_level.txt
--rw-r--r--   0 jhoward    (501) staff       (20)     1011 2024-05-27 18:25:39.000000 fastlite-0.0.1/settings.ini
--rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-05-27 21:53:51.696984 fastlite-0.0.1/setup.cfg
--rw-rw-r--   0 jhoward    (501) staff       (20)     2606 2024-05-27 17:26:46.000000 fastlite-0.0.1/setup.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-06-02 04:59:40.097289 fastlite-0.0.2/
+-rw-r--r--   0 jhoward    (501) staff       (20)    11357 2024-05-27 00:04:24.000000 fastlite-0.0.2/LICENSE
+-rw-rw-r--   0 jhoward    (501) staff       (20)      111 2024-05-27 17:26:46.000000 fastlite-0.0.2/MANIFEST.in
+-rw-r--r--   0 jhoward    (501) staff       (20)     7644 2024-06-02 04:59:40.097087 fastlite-0.0.2/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)     6849 2024-05-29 06:02:14.000000 fastlite-0.0.2/README.md
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-06-02 04:59:40.095787 fastlite-0.0.2/fastlite/
+-rw-r--r--   0 jhoward    (501) staff       (20)       61 2024-06-02 01:58:57.000000 fastlite-0.0.2/fastlite/__init__.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     4543 2024-06-02 01:58:57.000000 fastlite-0.0.2/fastlite/_modidx.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     5369 2024-06-02 01:58:57.000000 fastlite-0.0.2/fastlite/core.py
+-rw-r--r--   0 jhoward    (501) staff       (20)     8910 2024-06-01 18:43:58.000000 fastlite-0.0.2/fastlite/kw.py
+drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-06-02 04:59:40.096814 fastlite-0.0.2/fastlite.egg-info/
+-rw-r--r--   0 jhoward    (501) staff       (20)     7644 2024-06-02 04:59:40.000000 fastlite-0.0.2/fastlite.egg-info/PKG-INFO
+-rw-r--r--   0 jhoward    (501) staff       (20)      349 2024-06-02 04:59:40.000000 fastlite-0.0.2/fastlite.egg-info/SOURCES.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-06-02 04:59:40.000000 fastlite-0.0.2/fastlite.egg-info/dependency_links.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-06-02 04:59:40.000000 fastlite-0.0.2/fastlite.egg-info/entry_points.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-27 17:28:08.000000 fastlite-0.0.2/fastlite.egg-info/not-zip-safe
+-rw-r--r--   0 jhoward    (501) staff       (20)       37 2024-06-02 04:59:40.000000 fastlite-0.0.2/fastlite.egg-info/requires.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)        9 2024-06-02 04:59:40.000000 fastlite-0.0.2/fastlite.egg-info/top_level.txt
+-rw-r--r--   0 jhoward    (501) staff       (20)      853 2024-05-28 15:08:33.000000 fastlite-0.0.2/settings.ini
+-rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-06-02 04:59:40.097337 fastlite-0.0.2/setup.cfg
+-rw-rw-r--   0 jhoward    (501) staff       (20)     2606 2024-05-27 17:26:46.000000 fastlite-0.0.2/setup.py
```

### Comparing `fastlite-0.0.1/LICENSE` & `fastlite-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlite-0.0.1/fastlite/_modidx.py` & `fastlite-0.0.2/fastlite/_modidx.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,36 +4,43 @@
                 'doc_baseurl': '/fastlite',
                 'doc_host': 'https://AnswerDotAI.github.io',
                 'git_url': 'https://github.com/AnswerDotAI/fastlite',
                 'lib_path': 'fastlite'},
   'syms': { 'fastlite.core': { 'fastlite.core.Database.q': ('core.html#database.q', 'fastlite/core.py'),
                                'fastlite.core.Database.t': ('core.html#database.t', 'fastlite/core.py'),
                                'fastlite.core.Database.v': ('core.html#database.v', 'fastlite/core.py'),
+                               'fastlite.core.Table.__call__': ('core.html#table.__call__', 'fastlite/core.py'),
                                'fastlite.core.Table.__str__': ('core.html#table.__str__', 'fastlite/core.py'),
                                'fastlite.core.Table.c': ('core.html#table.c', 'fastlite/core.py'),
+                               'fastlite.core.Table.dataclass': ('core.html#table.dataclass', 'fastlite/core.py'),
+                               'fastlite.core.View.__call__': ('core.html#view.__call__', 'fastlite/core.py'),
                                'fastlite.core.View.__str__': ('core.html#view.__str__', 'fastlite/core.py'),
                                'fastlite.core.View.c': ('core.html#view.c', 'fastlite/core.py'),
                                'fastlite.core._Col': ('core.html#_col', 'fastlite/core.py'),
                                'fastlite.core._Col.__init__': ('core.html#_col.__init__', 'fastlite/core.py'),
                                'fastlite.core._Col.__repr__': ('core.html#_col.__repr__', 'fastlite/core.py'),
                                'fastlite.core._Col.__str__': ('core.html#_col.__str__', 'fastlite/core.py'),
                                'fastlite.core._ColsGetter': ('core.html#_colsgetter', 'fastlite/core.py'),
                                'fastlite.core._ColsGetter.__call__': ('core.html#_colsgetter.__call__', 'fastlite/core.py'),
+                               'fastlite.core._ColsGetter.__contains__': ('core.html#_colsgetter.__contains__', 'fastlite/core.py'),
                                'fastlite.core._ColsGetter.__dir__': ('core.html#_colsgetter.__dir__', 'fastlite/core.py'),
                                'fastlite.core._ColsGetter.__getattr__': ('core.html#_colsgetter.__getattr__', 'fastlite/core.py'),
                                'fastlite.core._ColsGetter.__init__': ('core.html#_colsgetter.__init__', 'fastlite/core.py'),
                                'fastlite.core._ColsGetter.__repr__': ('core.html#_colsgetter.__repr__', 'fastlite/core.py'),
                                'fastlite.core._Getter': ('core.html#_getter', 'fastlite/core.py'),
+                               'fastlite.core._Getter.__contains__': ('core.html#_getter.__contains__', 'fastlite/core.py'),
                                'fastlite.core._Getter.__getattr__': ('core.html#_getter.__getattr__', 'fastlite/core.py'),
                                'fastlite.core._Getter.__getitem__': ('core.html#_getter.__getitem__', 'fastlite/core.py'),
                                'fastlite.core._Getter.__init__': ('core.html#_getter.__init__', 'fastlite/core.py'),
                                'fastlite.core._Getter.__repr__': ('core.html#_getter.__repr__', 'fastlite/core.py'),
                                'fastlite.core._TablesGetter': ('core.html#_tablesgetter', 'fastlite/core.py'),
                                'fastlite.core._TablesGetter.__dir__': ('core.html#_tablesgetter.__dir__', 'fastlite/core.py'),
                                'fastlite.core._ViewsGetter': ('core.html#_viewsgetter', 'fastlite/core.py'),
                                'fastlite.core._ViewsGetter.__dir__': ('core.html#_viewsgetter.__dir__', 'fastlite/core.py'),
                                'fastlite.core._edge': ('core.html#_edge', 'fastlite/core.py'),
-                               'fastlite.core._edges': ('core.html#_edges', 'fastlite/core.py'),
+                               'fastlite.core._get_flds': ('core.html#_get_flds', 'fastlite/core.py'),
                                'fastlite.core._row': ('core.html#_row', 'fastlite/core.py'),
                                'fastlite.core._tnode': ('core.html#_tnode', 'fastlite/core.py'),
-                               'fastlite.core._tnodes': ('core.html#_tnodes', 'fastlite/core.py'),
-                               'fastlite.core.diagram': ('core.html#diagram', 'fastlite/core.py')}}}
+                               'fastlite.core.all_dcs': ('core.html#all_dcs', 'fastlite/core.py'),
+                               'fastlite.core.create_mod': ('core.html#create_mod', 'fastlite/core.py'),
+                               'fastlite.core.diagram': ('core.html#diagram', 'fastlite/core.py')},
+            'fastlite.kw': {}}}
```

### Comparing `fastlite-0.0.1/setup.py` & `fastlite-0.0.2/setup.py`

 * *Files identical despite different names*

