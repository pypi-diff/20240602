# Comparing `tmp/gridengine_framework-0.8.5.tar.gz` & `tmp/gridengine_framework-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridengine_framework-0.8.5.tar", last modified: Wed May  1 07:43:51 2024, max compression
+gzip compressed data, was "gridengine_framework-0.8.6.tar", last modified: Sun Jun  2 04:17:25 2024, max compression
```

## Comparing `gridengine_framework-0.8.5.tar` & `gridengine_framework-0.8.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.756724 gridengine_framework-0.8.5/
--rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.8.5/LICENSE
--rw-r--r--   0 boss      (1000) boss      (1002)     5832 2024-05-01 07:43:51.756724 gridengine_framework-0.8.5/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     5300 2024-05-01 07:43:13.000000 gridengine_framework-0.8.5/README.md
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.750058 gridengine_framework-0.8.5/grid_engine/
--rw-r--r--   0 boss      (1000) boss      (1002)      370 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     1293 2024-04-27 03:09:12.000000 gridengine_framework-0.8.5/grid_engine/__log__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4931 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/__main__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_blueprint/
--rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3624 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/__main__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2689 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/_floorplan_classes.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3820 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/_floorplan_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)    17503 2024-05-01 07:41:54.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/_grid_blueprint.py
--rw-r--r--   0 boss      (1000) boss      (1002)    18503 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/_grid_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)    10986 2024-04-24 16:18:00.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/_terrain_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)      272 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/objects.json
--rw-r--r--   0 boss      (1000) boss      (1002)     1615 2024-04-22 04:53:36.000000 gridengine_framework-0.8.5/grid_engine/_blueprint/terrains.json
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_cell/
--rw-r--r--   0 boss      (1000) boss      (1002)       22 2024-04-22 05:54:10.000000 gridengine_framework-0.8.5/grid_engine/_cell/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    32408 2024-05-01 07:24:21.000000 gridengine_framework-0.8.5/grid_engine/_cell/cell.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4756 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_dungeon.py
--rw-r--r--   0 boss      (1000) boss      (1002)    54929 2024-05-01 07:43:06.000000 gridengine_framework-0.8.5/grid_engine/_grid.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_feature/
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_feature/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2975 2024-04-25 05:52:12.000000 gridengine_framework-0.8.5/grid_engine/_grid_feature/grid_feature.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_group/
--rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_grid_group/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3648 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/_grid_group/grid_group.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_object/
--rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/__init__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_item/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_item/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_item/grid_item.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2767 2024-04-25 07:25:29.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_object.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_structure/
--rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_structure/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2216 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_structure/grid_structure.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_zone/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_zone/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.8.5/grid_engine/_grid_object/grid_zone/grid_zone.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.753391 gridengine_framework-0.8.5/grid_engine/_terraform/
--rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.8.5/grid_engine/_terraform/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    13627 2024-05-01 07:41:17.000000 gridengine_framework-0.8.5/grid_engine/_terraform/terraformer.py
--rw-r--r--   0 boss      (1000) boss      (1002)     6614 2024-04-24 16:17:44.000000 gridengine_framework-0.8.5/grid_engine/_utility.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2925 2024-04-23 13:22:30.000000 gridengine_framework-0.8.5/grid_engine/layout_test.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-05-01 07:43:51.756724 gridengine_framework-0.8.5/gridengine_framework.egg-info/
--rw-r--r--   0 boss      (1000) boss      (1002)     5832 2024-05-01 07:43:51.000000 gridengine_framework-0.8.5/gridengine_framework.egg-info/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     1439 2024-05-01 07:43:51.000000 gridengine_framework-0.8.5/gridengine_framework.egg-info/SOURCES.txt
--rw-r--r--   0 boss      (1000) boss      (1002)        1 2024-05-01 07:43:51.000000 gridengine_framework-0.8.5/gridengine_framework.egg-info/dependency_links.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-05-01 07:43:51.000000 gridengine_framework-0.8.5/gridengine_framework.egg-info/requires.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       12 2024-05-01 07:43:51.000000 gridengine_framework-0.8.5/gridengine_framework.egg-info/top_level.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       38 2024-05-01 07:43:51.756724 gridengine_framework-0.8.5/setup.cfg
--rw-r--r--   0 boss      (1000) boss      (1002)      903 2024-05-01 07:43:29.000000 gridengine_framework-0.8.5/setup.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.312435 gridengine_framework-0.8.6/
+-rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.8.6/LICENSE
+-rw-r--r--   0 boss      (1000) boss      (1002)     5832 2024-06-02 04:17:25.312435 gridengine_framework-0.8.6/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     5300 2024-05-01 07:43:13.000000 gridengine_framework-0.8.6/README.md
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.305768 gridengine_framework-0.8.6/grid_engine/
+-rw-r--r--   0 boss      (1000) boss      (1002)      370 2024-04-23 13:22:30.000000 gridengine_framework-0.8.6/grid_engine/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     1293 2024-04-27 03:09:12.000000 gridengine_framework-0.8.6/grid_engine/__log__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4931 2024-04-23 13:22:30.000000 gridengine_framework-0.8.6/grid_engine/__main__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.309102 gridengine_framework-0.8.6/grid_engine/_blueprint/
+-rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.8.6/grid_engine/_blueprint/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3624 2024-04-23 13:22:30.000000 gridengine_framework-0.8.6/grid_engine/_blueprint/__main__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2689 2024-04-23 13:22:30.000000 gridengine_framework-0.8.6/grid_engine/_blueprint/_floorplan_classes.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3820 2024-04-23 13:22:30.000000 gridengine_framework-0.8.6/grid_engine/_blueprint/_floorplan_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    17503 2024-05-01 07:41:54.000000 gridengine_framework-0.8.6/grid_engine/_blueprint/_grid_blueprint.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    18503 2024-04-23 13:22:30.000000 gridengine_framework-0.8.6/grid_engine/_blueprint/_grid_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    10986 2024-04-24 16:18:00.000000 gridengine_framework-0.8.6/grid_engine/_blueprint/_terrain_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)      272 2024-04-23 13:22:30.000000 gridengine_framework-0.8.6/grid_engine/_blueprint/objects.json
+-rw-r--r--   0 boss      (1000) boss      (1002)     1615 2024-04-22 04:53:36.000000 gridengine_framework-0.8.6/grid_engine/_blueprint/terrains.json
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.309102 gridengine_framework-0.8.6/grid_engine/_cell/
+-rw-r--r--   0 boss      (1000) boss      (1002)       22 2024-04-22 05:54:10.000000 gridengine_framework-0.8.6/grid_engine/_cell/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    32408 2024-05-15 03:05:10.000000 gridengine_framework-0.8.6/grid_engine/_cell/cell.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4756 2024-04-23 13:22:30.000000 gridengine_framework-0.8.6/grid_engine/_dungeon.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    54929 2024-05-01 07:43:06.000000 gridengine_framework-0.8.6/grid_engine/_grid.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.309102 gridengine_framework-0.8.6/grid_engine/_grid_feature/
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.8.6/grid_engine/_grid_feature/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2975 2024-04-25 05:52:12.000000 gridengine_framework-0.8.6/grid_engine/_grid_feature/grid_feature.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.309102 gridengine_framework-0.8.6/grid_engine/_grid_group/
+-rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-23 13:22:30.000000 gridengine_framework-0.8.6/grid_engine/_grid_group/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3648 2024-04-23 13:22:30.000000 gridengine_framework-0.8.6/grid_engine/_grid_group/grid_group.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.309102 gridengine_framework-0.8.6/grid_engine/_grid_object/
+-rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.8.6/grid_engine/_grid_object/__init__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.309102 gridengine_framework-0.8.6/grid_engine/_grid_object/grid_item/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.6/grid_engine/_grid_object/grid_item/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.8.6/grid_engine/_grid_object/grid_item/grid_item.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2767 2024-04-25 07:25:29.000000 gridengine_framework-0.8.6/grid_engine/_grid_object/grid_object.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.309102 gridengine_framework-0.8.6/grid_engine/_grid_object/grid_structure/
+-rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.8.6/grid_engine/_grid_object/grid_structure/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3793 2024-06-02 04:14:26.000000 gridengine_framework-0.8.6/grid_engine/_grid_object/grid_structure/grid_structure.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.309102 gridengine_framework-0.8.6/grid_engine/_grid_object/grid_zone/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.6/grid_engine/_grid_object/grid_zone/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.8.6/grid_engine/_grid_object/grid_zone/grid_zone.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.309102 gridengine_framework-0.8.6/grid_engine/_terraform/
+-rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.8.6/grid_engine/_terraform/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    13627 2024-05-01 07:41:17.000000 gridengine_framework-0.8.6/grid_engine/_terraform/terraformer.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     6614 2024-04-24 16:17:44.000000 gridengine_framework-0.8.6/grid_engine/_utility.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2925 2024-04-23 13:22:30.000000 gridengine_framework-0.8.6/grid_engine/layout_test.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-06-02 04:17:25.312435 gridengine_framework-0.8.6/gridengine_framework.egg-info/
+-rw-r--r--   0 boss      (1000) boss      (1002)     5832 2024-06-02 04:17:25.000000 gridengine_framework-0.8.6/gridengine_framework.egg-info/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     1439 2024-06-02 04:17:25.000000 gridengine_framework-0.8.6/gridengine_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)        1 2024-06-02 04:17:25.000000 gridengine_framework-0.8.6/gridengine_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-06-02 04:17:25.000000 gridengine_framework-0.8.6/gridengine_framework.egg-info/requires.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       12 2024-06-02 04:17:25.000000 gridengine_framework-0.8.6/gridengine_framework.egg-info/top_level.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       38 2024-06-02 04:17:25.312435 gridengine_framework-0.8.6/setup.cfg
+-rw-r--r--   0 boss      (1000) boss      (1002)      903 2024-06-02 04:17:17.000000 gridengine_framework-0.8.6/setup.py
```

### Comparing `gridengine_framework-0.8.5/LICENSE` & `gridengine_framework-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/PKG-INFO` & `gridengine_framework-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridengine_framework
-Version: 0.8.5
+Version: 0.8.6
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gridengine_framework-0.8.5/README.md` & `gridengine_framework-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/__log__.py` & `gridengine_framework-0.8.6/grid_engine/__log__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/__main__.py` & `gridengine_framework-0.8.6/grid_engine/__main__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_blueprint/__main__.py` & `gridengine_framework-0.8.6/grid_engine/_blueprint/__main__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_blueprint/_floorplan_classes.py` & `gridengine_framework-0.8.6/grid_engine/_blueprint/_floorplan_classes.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_blueprint/_floorplan_processing.py` & `gridengine_framework-0.8.6/grid_engine/_blueprint/_floorplan_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_blueprint/_grid_blueprint.py` & `gridengine_framework-0.8.6/grid_engine/_blueprint/_grid_blueprint.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_blueprint/_grid_processing.py` & `gridengine_framework-0.8.6/grid_engine/_blueprint/_grid_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_blueprint/_terrain_processing.py` & `gridengine_framework-0.8.6/grid_engine/_blueprint/_terrain_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_blueprint/terrains.json` & `gridengine_framework-0.8.6/grid_engine/_blueprint/terrains.json`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_cell/cell.py` & `gridengine_framework-0.8.6/grid_engine/_cell/cell.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_dungeon.py` & `gridengine_framework-0.8.6/grid_engine/_dungeon.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_grid.py` & `gridengine_framework-0.8.6/grid_engine/_grid.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_grid_feature/grid_feature.py` & `gridengine_framework-0.8.6/grid_engine/_grid_feature/grid_feature.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_grid_group/grid_group.py` & `gridengine_framework-0.8.6/grid_engine/_grid_group/grid_group.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_grid_object/grid_item/grid_item.py` & `gridengine_framework-0.8.6/grid_engine/_grid_object/grid_item/grid_item.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_grid_object/grid_object.py` & `gridengine_framework-0.8.6/grid_engine/_grid_object/grid_object.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_grid_object/grid_zone/grid_zone.py` & `gridengine_framework-0.8.6/grid_engine/_grid_object/grid_zone/grid_zone.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_terraform/terraformer.py` & `gridengine_framework-0.8.6/grid_engine/_terraform/terraformer.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/_utility.py` & `gridengine_framework-0.8.6/grid_engine/_utility.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/grid_engine/layout_test.py` & `gridengine_framework-0.8.6/grid_engine/layout_test.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/gridengine_framework.egg-info/PKG-INFO` & `gridengine_framework-0.8.6/gridengine_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridengine-framework
-Version: 0.8.5
+Version: 0.8.6
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gridengine_framework-0.8.5/gridengine_framework.egg-info/SOURCES.txt` & `gridengine_framework-0.8.6/gridengine_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.5/setup.py` & `gridengine_framework-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
     
 setup(
     name='gridengine_framework',
-    version='0.8.5',
+    version='0.8.6',
     description='A framework for generating and manipulating grid-based game worlds',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='James Evans',
     author_email='joesaysahoy@gmail.com',
     url='https://github.com/primal-coder/grid-engine',
     packages=find_packages(),
```

