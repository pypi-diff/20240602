# Comparing `tmp/cdt_path-2.1.5.tar.gz` & `tmp/cdt_path-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdt_path-2.1.5.tar", last modified: Mon May 27 13:49:29 2024, max compression
+gzip compressed data, was "cdt_path-2.2.1.tar", last modified: Sun Jun  2 10:40:47 2024, max compression
```

## Comparing `cdt_path-2.1.5.tar` & `cdt_path-2.2.1.tar`

### file list

```diff
@@ -1,59 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.288656 cdt_path-2.1.5/
--rw-rw-rw-   0        0        0      435 2024-05-27 13:49:29.287634 cdt_path-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      100 2024-05-23 07:09:32.000000 cdt_path-2.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.257239 cdt_path-2.1.5/cdt_path/
--rw-rw-rw-   0        0        0      596 2024-05-27 06:18:44.000000 cdt_path-2.1.5/cdt_path/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.263852 cdt_path-2.1.5/cdt_path/circumcircle/
--rw-rw-rw-   0        0        0        0 2024-05-14 14:48:14.000000 cdt_path-2.1.5/cdt_path/circumcircle/__init__.py
--rw-rw-rw-   0        0        0      648 2024-05-15 06:54:49.000000 cdt_path-2.1.5/cdt_path/circumcircle/calculate.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.263852 cdt_path-2.1.5/cdt_path/constrained_delaunay/
--rw-rw-rw-   0        0        0        0 2024-05-06 01:15:42.000000 cdt_path-2.1.5/cdt_path/constrained_delaunay/__init__.py
--rw-rw-rw-   0        0        0      117 2024-05-09 06:46:10.000000 cdt_path-2.1.5/cdt_path/constrained_delaunay/cdt_edge_additions.py
--rw-rw-rw-   0        0        0      352 2024-05-06 01:33:01.000000 cdt_path-2.1.5/cdt_path/constrained_delaunay/definition.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.267336 cdt_path-2.1.5/cdt_path/convex_hull/
--rw-rw-rw-   0        0        0      181 2024-04-13 02:40:26.000000 cdt_path-2.1.5/cdt_path/convex_hull/__init__.py
--rw-rw-rw-   0        0        0      202 2024-04-11 22:13:16.000000 cdt_path-2.1.5/cdt_path/convex_hull/display.py
--rw-rw-rw-   0        0        0     4543 2024-04-11 22:13:16.000000 cdt_path-2.1.5/cdt_path/convex_hull/divide_and_conquer.py
--rw-rw-rw-   0        0        0     1321 2024-04-11 22:13:16.000000 cdt_path-2.1.5/cdt_path/convex_hull/extreme_edge.py
--rw-rw-rw-   0        0        0     1225 2024-04-11 22:13:16.000000 cdt_path-2.1.5/cdt_path/convex_hull/gift_wrap.py
--rw-rw-rw-   0        0        0     3823 2024-05-27 13:38:41.000000 cdt_path-2.1.5/cdt_path/convex_hull/incremental.py
--rw-rw-rw-   0        0        0     1238 2024-04-11 22:13:16.000000 cdt_path-2.1.5/cdt_path/convex_hull/quick_hull.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.271241 cdt_path-2.1.5/cdt_path/delaunay/
--rw-rw-rw-   0        0        0       78 2024-04-18 11:20:20.000000 cdt_path-2.1.5/cdt_path/delaunay/__init__.py
--rw-rw-rw-   0        0        0     1219 2024-05-06 01:27:54.000000 cdt_path-2.1.5/cdt_path/delaunay/definition.py
--rw-rw-rw-   0        0        0     1080 2024-04-14 14:36:46.000000 cdt_path-2.1.5/cdt_path/delaunay/definition_Old_2.py
--rw-rw-rw-   0        0        0       75 2024-04-18 11:17:22.000000 cdt_path-2.1.5/cdt_path/delaunay/hhh.py
--rw-rw-rw-   0        0        0     3577 2024-04-15 03:58:05.000000 cdt_path-2.1.5/cdt_path/delaunay/incremental.py
--rw-rw-rw-   0        0        0     8444 2024-04-14 14:34:03.000000 cdt_path-2.1.5/cdt_path/delaunay/incremental_Old.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.271241 cdt_path-2.1.5/cdt_path/demo/
--rw-rw-rw-   0        0        0      348 2024-05-23 03:31:08.000000 cdt_path-2.1.5/cdt_path/demo/Interact_part.py
--rw-rw-rw-   0        0        0       21 2024-05-27 13:46:58.000000 cdt_path-2.1.5/cdt_path/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.275242 cdt_path-2.1.5/cdt_path/file/
--rw-rw-rw-   0        0        0       19 2024-05-22 13:26:45.000000 cdt_path-2.1.5/cdt_path/file/__init__.py
--rw-rw-rw-   0        0        0      116 2024-05-22 13:28:55.000000 cdt_path-2.1.5/cdt_path/file/load.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.275242 cdt_path-2.1.5/cdt_path/interact/
--rw-rw-rw-   0        0        0       66 2024-05-23 14:55:55.000000 cdt_path-2.1.5/cdt_path/interact/__init__.py
--rw-rw-rw-   0        0        0     3628 2024-05-25 13:59:10.000000 cdt_path-2.1.5/cdt_path/interact/base.py
--rw-rw-rw-   0        0        0      257 2024-05-23 03:30:04.000000 cdt_path-2.1.5/cdt_path/interact/border.py
--rw-rw-rw-   0        0        0     1447 2024-05-24 08:52:59.000000 cdt_path-2.1.5/cdt_path/interact/draw.py
--rw-rw-rw-   0        0        0     1523 2024-05-16 08:58:29.000000 cdt_path-2.1.5/cdt_path/interact/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.284631 cdt_path-2.1.5/cdt_path/manipulate/
--rw-rw-rw-   0        0        0       22 2024-05-21 13:38:19.000000 cdt_path-2.1.5/cdt_path/manipulate/__init__.py
--rw-rw-rw-   0        0        0     1000 2024-05-21 13:44:41.000000 cdt_path-2.1.5/cdt_path/manipulate/combine.py
--rw-rw-rw-   0        0        0       14 2024-05-12 06:05:36.000000 cdt_path-2.1.5/cdt_path/manipulate/save.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.287634 cdt_path-2.1.5/cdt_path/pathplan/
--rw-rw-rw-   0        0        0     3452 2024-05-23 11:51:41.000000 cdt_path-2.1.5/cdt_path/pathplan/A_star.py
--rw-rw-rw-   0        0        0     1373 2024-05-05 11:19:13.000000 cdt_path-2.1.5/cdt_path/pathplan/A_star_O.py
--rw-rw-rw-   0        0        0       68 2024-05-22 13:51:17.000000 cdt_path-2.1.5/cdt_path/pathplan/__init__.py
--rw-rw-rw-   0        0        0     1300 2024-05-22 13:01:38.000000 cdt_path-2.1.5/cdt_path/pathplan/funnel - 副本.py
--rw-rw-rw-   0        0        0     2707 2024-05-25 12:51:42.000000 cdt_path-2.1.5/cdt_path/pathplan/funnel.py
--rw-rw-rw-   0        0        0     1512 2024-05-25 15:57:56.000000 cdt_path-2.1.5/cdt_path/pathplan/utils.py
--rw-rw-rw-   0        0        0     2328 2024-04-11 22:13:16.000000 cdt_path-2.1.5/cdt_path/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:49:29.261239 cdt_path-2.1.5/cdt_path.egg-info/
--rw-rw-rw-   0        0        0      435 2024-05-27 13:49:29.000000 cdt_path-2.1.5/cdt_path.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1381 2024-05-27 13:49:29.000000 cdt_path-2.1.5/cdt_path.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 13:49:29.000000 cdt_path-2.1.5/cdt_path.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-27 13:49:29.000000 cdt_path-2.1.5/cdt_path.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 13:49:29.000000 cdt_path-2.1.5/cdt_path.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 13:49:29.288656 cdt_path-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0      727 2024-05-27 13:49:19.000000 cdt_path-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:40:47.804643 cdt_path-2.2.1/
+-rw-rw-rw-   0        0        0      435 2024-06-02 10:40:47.804643 cdt_path-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2024-05-23 07:09:32.000000 cdt_path-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 10:40:47.775167 cdt_path-2.2.1/cdt_path/
+-rw-rw-rw-   0        0        0      622 2024-05-30 12:43:44.000000 cdt_path-2.2.1/cdt_path/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:40:47.783170 cdt_path-2.2.1/cdt_path/circumcircle/
+-rw-rw-rw-   0        0        0        0 2024-05-14 14:48:14.000000 cdt_path-2.2.1/cdt_path/circumcircle/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-05-15 06:54:49.000000 cdt_path-2.2.1/cdt_path/circumcircle/calculate.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:40:47.788638 cdt_path-2.2.1/cdt_path/convex_hull/
+-rw-rw-rw-   0        0        0      181 2024-04-13 02:40:26.000000 cdt_path-2.2.1/cdt_path/convex_hull/__init__.py
+-rw-rw-rw-   0        0        0      202 2024-04-11 22:13:16.000000 cdt_path-2.2.1/cdt_path/convex_hull/display.py
+-rw-rw-rw-   0        0        0     4543 2024-04-11 22:13:16.000000 cdt_path-2.2.1/cdt_path/convex_hull/divide_and_conquer.py
+-rw-rw-rw-   0        0        0     1321 2024-04-11 22:13:16.000000 cdt_path-2.2.1/cdt_path/convex_hull/extreme_edge.py
+-rw-rw-rw-   0        0        0     1225 2024-04-11 22:13:16.000000 cdt_path-2.2.1/cdt_path/convex_hull/gift_wrap.py
+-rw-rw-rw-   0        0        0     3823 2024-05-27 13:38:41.000000 cdt_path-2.2.1/cdt_path/convex_hull/incremental.py
+-rw-rw-rw-   0        0        0     1238 2024-04-11 22:13:16.000000 cdt_path-2.2.1/cdt_path/convex_hull/quick_hull.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:40:47.792640 cdt_path-2.2.1/cdt_path/delaunay/
+-rw-rw-rw-   0        0        0       78 2024-04-18 11:20:20.000000 cdt_path-2.2.1/cdt_path/delaunay/__init__.py
+-rw-rw-rw-   0        0        0     1219 2024-05-06 01:27:54.000000 cdt_path-2.2.1/cdt_path/delaunay/definition.py
+-rw-rw-rw-   0        0        0     1080 2024-04-14 14:36:46.000000 cdt_path-2.2.1/cdt_path/delaunay/definition_Old_2.py
+-rw-rw-rw-   0        0        0       75 2024-04-18 11:17:22.000000 cdt_path-2.2.1/cdt_path/delaunay/hhh.py
+-rw-rw-rw-   0        0        0     3577 2024-04-15 03:58:05.000000 cdt_path-2.2.1/cdt_path/delaunay/incremental.py
+-rw-rw-rw-   0        0        0     8444 2024-04-14 14:34:03.000000 cdt_path-2.2.1/cdt_path/delaunay/incremental_Old.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:40:47.792640 cdt_path-2.2.1/cdt_path/demo/
+-rw-rw-rw-   0        0        0     6239 2024-05-27 14:01:04.000000 cdt_path-2.2.1/cdt_path/demo/Interact_part.py
+-rw-rw-rw-   0        0        0       21 2024-05-27 13:46:58.000000 cdt_path-2.2.1/cdt_path/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:40:47.792640 cdt_path-2.2.1/cdt_path/file/
+-rw-rw-rw-   0        0        0       19 2024-05-22 13:26:45.000000 cdt_path-2.2.1/cdt_path/file/__init__.py
+-rw-rw-rw-   0        0        0      116 2024-05-22 13:28:55.000000 cdt_path-2.2.1/cdt_path/file/load.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:40:47.796641 cdt_path-2.2.1/cdt_path/interact/
+-rw-rw-rw-   0        0        0       66 2024-05-23 14:55:55.000000 cdt_path-2.2.1/cdt_path/interact/__init__.py
+-rw-rw-rw-   0        0        0     3553 2024-06-02 09:42:30.000000 cdt_path-2.2.1/cdt_path/interact/base.py
+-rw-rw-rw-   0        0        0      257 2024-05-23 03:30:04.000000 cdt_path-2.2.1/cdt_path/interact/border.py
+-rw-rw-rw-   0        0        0     2035 2024-06-02 09:43:06.000000 cdt_path-2.2.1/cdt_path/interact/draw.py
+-rw-rw-rw-   0        0        0     1523 2024-05-16 08:58:29.000000 cdt_path-2.2.1/cdt_path/interact/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:40:47.796641 cdt_path-2.2.1/cdt_path/manipulate/
+-rw-rw-rw-   0        0        0       22 2024-05-21 13:38:19.000000 cdt_path-2.2.1/cdt_path/manipulate/__init__.py
+-rw-rw-rw-   0        0        0     1000 2024-05-21 13:44:41.000000 cdt_path-2.2.1/cdt_path/manipulate/combine.py
+-rw-rw-rw-   0        0        0       14 2024-05-12 06:05:36.000000 cdt_path-2.2.1/cdt_path/manipulate/save.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:40:47.804643 cdt_path-2.2.1/cdt_path/pathplan/
+-rw-rw-rw-   0        0        0     3452 2024-05-23 11:51:41.000000 cdt_path-2.2.1/cdt_path/pathplan/A_star.py
+-rw-rw-rw-   0        0        0     1373 2024-05-05 11:19:13.000000 cdt_path-2.2.1/cdt_path/pathplan/A_star_O.py
+-rw-rw-rw-   0        0        0       68 2024-05-22 13:51:17.000000 cdt_path-2.2.1/cdt_path/pathplan/__init__.py
+-rw-rw-rw-   0        0        0     1300 2024-05-22 13:01:38.000000 cdt_path-2.2.1/cdt_path/pathplan/funnel - 副本.py
+-rw-rw-rw-   0        0        0     2707 2024-05-25 12:51:42.000000 cdt_path-2.2.1/cdt_path/pathplan/funnel.py
+-rw-rw-rw-   0        0        0     1512 2024-05-25 15:57:56.000000 cdt_path-2.2.1/cdt_path/pathplan/utils.py
+-rw-rw-rw-   0        0        0     2328 2024-04-11 22:13:16.000000 cdt_path-2.2.1/cdt_path/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:40:47.779169 cdt_path-2.2.1/cdt_path.egg-info/
+-rw-rw-rw-   0        0        0      435 2024-06-02 10:40:47.000000 cdt_path-2.2.1/cdt_path.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2024-06-02 10:40:47.000000 cdt_path-2.2.1/cdt_path.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 10:40:47.000000 cdt_path-2.2.1/cdt_path.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-06-02 10:40:47.000000 cdt_path-2.2.1/cdt_path.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 10:40:47.000000 cdt_path-2.2.1/cdt_path.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 10:40:47.804643 cdt_path-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      727 2024-06-02 10:40:44.000000 cdt_path-2.2.1/setup.py
```

### Comparing `cdt_path-2.1.5/cdt_path/__init__.py` & `cdt_path-2.2.1/cdt_path/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from . import pathplan
 from . import manipulate
 from . import convex_hull
+from . import delaunay
+
 from .file import *
 from triangle import triangulate as _triangulate
 from .interact.base import Interact
 from .interact import border
 from matplotlib.tri import Triangulation as _Triangulation
 from .circumcircle.calculate import circumcircle
```

### Comparing `cdt_path-2.1.5/cdt_path/circumcircle/calculate.py` & `cdt_path-2.2.1/cdt_path/circumcircle/calculate.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/convex_hull/divide_and_conquer.py` & `cdt_path-2.2.1/cdt_path/convex_hull/divide_and_conquer.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/convex_hull/extreme_edge.py` & `cdt_path-2.2.1/cdt_path/convex_hull/extreme_edge.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/convex_hull/gift_wrap.py` & `cdt_path-2.2.1/cdt_path/convex_hull/gift_wrap.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/convex_hull/incremental.py` & `cdt_path-2.2.1/cdt_path/convex_hull/incremental.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/convex_hull/quick_hull.py` & `cdt_path-2.2.1/cdt_path/convex_hull/quick_hull.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/delaunay/definition.py` & `cdt_path-2.2.1/cdt_path/delaunay/definition.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/delaunay/definition_Old_2.py` & `cdt_path-2.2.1/cdt_path/delaunay/definition_Old_2.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/delaunay/incremental.py` & `cdt_path-2.2.1/cdt_path/delaunay/incremental.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/delaunay/incremental_Old.py` & `cdt_path-2.2.1/cdt_path/delaunay/incremental_Old.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/interact/base.py` & `cdt_path-2.2.1/cdt_path/interact/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.patches import Polygon
-# from matplotlib.tri import Triangulation
 from matplotlib.backend_bases import MouseButton
-# import matplotlib.tri as tri
 from cdt_path.pathplan import *
 from . import border
 class Interact:
 	def __init__(self, ax, triang, title=True):
 		self.ax = ax
 		self.triang = triang
 		self.trifinder = triang.get_trifinder()
```

### Comparing `cdt_path-2.1.5/cdt_path/interact/utils.py` & `cdt_path-2.2.1/cdt_path/interact/utils.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/manipulate/combine.py` & `cdt_path-2.2.1/cdt_path/manipulate/combine.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/pathplan/A_star.py` & `cdt_path-2.2.1/cdt_path/pathplan/A_star.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/pathplan/A_star_O.py` & `cdt_path-2.2.1/cdt_path/pathplan/A_star_O.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/pathplan/funnel - 副本.py` & `cdt_path-2.2.1/cdt_path/pathplan/funnel - 副本.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/pathplan/funnel.py` & `cdt_path-2.2.1/cdt_path/pathplan/funnel.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/pathplan/utils.py` & `cdt_path-2.2.1/cdt_path/pathplan/utils.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path/utils.py` & `cdt_path-2.2.1/cdt_path/utils.py`

 * *Files identical despite different names*

### Comparing `cdt_path-2.1.5/cdt_path.egg-info/SOURCES.txt` & `cdt_path-2.2.1/cdt_path.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 cdt_path.egg-info/PKG-INFO
 cdt_path.egg-info/SOURCES.txt
 cdt_path.egg-info/dependency_links.txt
 cdt_path.egg-info/requires.txt
 cdt_path.egg-info/top_level.txt
 cdt_path/circumcircle/__init__.py
 cdt_path/circumcircle/calculate.py
-cdt_path/constrained_delaunay/__init__.py
-cdt_path/constrained_delaunay/cdt_edge_additions.py
-cdt_path/constrained_delaunay/definition.py
 cdt_path/convex_hull/__init__.py
 cdt_path/convex_hull/display.py
 cdt_path/convex_hull/divide_and_conquer.py
 cdt_path/convex_hull/extreme_edge.py
 cdt_path/convex_hull/gift_wrap.py
 cdt_path/convex_hull/incremental.py
 cdt_path/convex_hull/quick_hull.py
```

### Comparing `cdt_path-2.1.5/setup.py` & `cdt_path-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="cdt_path",
-    version='2.1.5',
+    version='2.2.1',
     author="CaiShu",
     author_email="caiyi@mail.ustc.edu.cn",
     description="Constrainted Delaunay Triangle for path-planning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # license="MIT",
     # url="https://gitee.com/DerrickChiu/function_tool.git",
```

