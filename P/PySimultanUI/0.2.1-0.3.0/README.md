# Comparing `tmp/pysimultanui-0.2.1.tar.gz` & `tmp/pysimultanui-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysimultanui-0.2.1.tar", last modified: Fri May 10 08:44:37 2024, max compression
+gzip compressed data, was "pysimultanui-0.3.0.tar", last modified: Sun Jun  2 12:42:34 2024, max compression
```

## Comparing `pysimultanui-0.2.1.tar` & `pysimultanui-0.3.0.tar`

### file list

```diff
@@ -1,68 +1,74 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.547579 pysimultanui-0.2.1/
--rw-rw-rw-   0        0        0     1040 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0       97 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1776 2024-05-10 08:44:37.546040 pysimultanui-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      191 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/README.md
--rw-rw-rw-   0        0        0     1311 2024-05-10 08:44:19.000000 pysimultanui-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      189 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 08:44:37.547579 pysimultanui-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2089 2024-05-10 08:44:26.000000 pysimultanui-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.429952 pysimultanui-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.543788 pysimultanui-0.2.1/src/PySimultanUI.egg-info/
--rw-rw-rw-   0        0        0     1776 2024-05-10 08:44:37.000000 pysimultanui-0.2.1/src/PySimultanUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1554 2024-05-10 08:44:37.000000 pysimultanui-0.2.1/src/PySimultanUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 08:44:37.000000 pysimultanui-0.2.1/src/PySimultanUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-09 18:48:30.000000 pysimultanui-0.2.1/src/PySimultanUI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2024-05-10 08:44:37.000000 pysimultanui-0.2.1/src/PySimultanUI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.458553 pysimultanui-0.2.1/src/app/
--rw-rw-rw-   0        0        0        2 2024-04-27 13:04:42.000000 pysimultanui-0.2.1/src/app/__init__.py
--rw-rw-rw-   0        0        0      856 2024-04-27 13:04:42.000000 pysimultanui-0.2.1/src/app/auth.py
--rw-rw-rw-   0        0        0      557 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/app/home.py
--rw-rw-rw-   0        0        0     1190 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/app/login.py
--rw-rw-rw-   0        0        0      111 2024-04-27 13:04:42.000000 pysimultanui-0.2.1/src/app/menue.py
--rw-rw-rw-   0        0        0      304 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/app/project.py
--rw-rw-rw-   0        0        0     3630 2024-05-10 07:09:06.000000 pysimultanui-0.2.1/src/app/theme.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.470177 pysimultanui-0.2.1/src/core/
--rw-rw-rw-   0        0        0     1042 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/core/__init__.py
--rw-rw-rw-   0        0        0    14323 2024-05-10 07:37:08.000000 pysimultanui-0.2.1/src/core/edit_dialog.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.472741 pysimultanui-0.2.1/src/core/freecad_utils/
--rw-rw-rw-   0        0        0     2205 2024-05-10 08:30:36.000000 pysimultanui-0.2.1/src/core/freecad_utils/__init__.py
--rw-rw-rw-   0        0        0     5681 2024-05-10 07:44:30.000000 pysimultanui-0.2.1/src/core/freecad_utils/tools.py
--rw-rw-rw-   0        0        0       61 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/core/logging.py
--rw-rw-rw-   0        0        0     7740 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/core/method_mapper.py
--rw-rw-rw-   0        0        0     3080 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/core/navigation.py
--rw-rw-rw-   0        0        0    22200 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/core/project_manager.py
--rw-rw-rw-   0        0        0      591 2024-04-27 13:04:42.000000 pysimultanui-0.2.1/src/core/tools.py
--rw-rw-rw-   0        0        0     6329 2024-05-10 07:09:06.000000 pysimultanui-0.2.1/src/core/user.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.482702 pysimultanui-0.2.1/src/views/
--rw-rw-rw-   0        0        0      196 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/views/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.486472 pysimultanui-0.2.1/src/views/asset_view/
--rw-rw-rw-   0        0        0       76 2024-04-27 13:04:42.000000 pysimultanui-0.2.1/src/views/asset_view/__init__.py
--rw-rw-rw-   0        0        0     1991 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/views/asset_view/asset_manager.py
--rw-rw-rw-   0        0        0     1068 2024-05-05 18:09:42.000000 pysimultanui-0.2.1/src/views/asset_view/asset_view.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.529531 pysimultanui-0.2.1/src/views/component_dict_view/
--rw-rw-rw-   0        0        0      110 2024-05-05 18:09:42.000000 pysimultanui-0.2.1/src/views/component_dict_view/__init__.py
--rw-rw-rw-   0        0        0     1143 2024-05-10 07:09:06.000000 pysimultanui-0.2.1/src/views/component_dict_view/component_dict_manager.py
--rw-rw-rw-   0        0        0     7380 2024-05-10 07:09:06.000000 pysimultanui-0.2.1/src/views/component_dict_view/component_dict_view.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.532131 pysimultanui-0.2.1/src/views/component_list_view/
--rw-rw-rw-   0        0        0        0 2024-04-27 13:04:42.000000 pysimultanui-0.2.1/src/views/component_list_view/__init__.py
--rw-rw-rw-   0        0        0      704 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/views/component_list_view/component_list_manager.py
--rw-rw-rw-   0        0        0     9973 2024-05-10 08:40:54.000000 pysimultanui-0.2.1/src/views/component_list_view/component_list_view.py
--rw-rw-rw-   0        0        0     3237 2024-05-10 08:37:43.000000 pysimultanui-0.2.1/src/views/detail_views.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.536216 pysimultanui-0.2.1/src/views/geometry_view/
--rw-rw-rw-   0        0        0       88 2024-04-27 13:04:42.000000 pysimultanui-0.2.1/src/views/geometry_view/__init__.py
--rw-rw-rw-   0        0        0     6316 2024-05-10 08:01:11.000000 pysimultanui-0.2.1/src/views/geometry_view/geometry_manager.py
--rw-rw-rw-   0        0        0     6361 2024-05-09 17:45:30.000000 pysimultanui-0.2.1/src/views/geometry_view/geometry_view.py
--rw-rw-rw-   0        0        0     2834 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/views/geometry_view/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.540785 pysimultanui-0.2.1/src/views/mapped_cls/
--rw-rw-rw-   0        0        0       49 2024-04-27 13:04:42.000000 pysimultanui-0.2.1/src/views/mapped_cls/__init__.py
--rw-rw-rw-   0        0        0     2825 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/views/mapped_cls/mapped_cls_manager.py
--rw-rw-rw-   0        0        0    10882 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/views/mapped_cls/mapped_cls_view.py
--rw-rw-rw-   0        0        0     6503 2024-05-09 17:45:07.000000 pysimultanui-0.2.1/src/views/numpy_view.py
--rw-rw-rw-   0        0        0     6952 2024-05-09 17:44:27.000000 pysimultanui-0.2.1/src/views/pandas_df_view.py
--rw-rw-rw-   0        0        0     2230 2024-05-05 18:09:42.000000 pysimultanui-0.2.1/src/views/parameter_view.py
--rw-rw-rw-   0        0        0     2403 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/views/type_view.py
--rw-rw-rw-   0        0        0     7819 2024-05-10 07:09:06.000000 pysimultanui-0.2.1/src/views/type_view_manager.py
--rw-rw-rw-   0        0        0     7036 2024-05-09 17:27:15.000000 pysimultanui-0.2.1/src/views/view_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-10 08:44:37.542784 pysimultanui-0.2.1/tests/
--rw-rw-rw-   0        0        0    30486 2024-05-10 07:09:06.000000 pysimultanui-0.2.1/tests/test_py_simultan_ui.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.881379 pysimultanui-0.3.0/
+-rw-rw-rw-   0        0        0     1040 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       97 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2201 2024-06-02 12:42:34.880370 pysimultanui-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1412 2024-06-02 12:42:05.000000 pysimultanui-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      170 2024-06-02 12:41:08.000000 pysimultanui-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 12:42:34.881379 pysimultanui-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2089 2024-06-02 12:42:11.000000 pysimultanui-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.798540 pysimultanui-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.879164 pysimultanui-0.3.0/src/PySimultanUI.egg-info/
+-rw-rw-rw-   0        0        0     2201 2024-06-02 12:42:34.000000 pysimultanui-0.3.0/src/PySimultanUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1729 2024-06-02 12:42:34.000000 pysimultanui-0.3.0/src/PySimultanUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 12:42:34.000000 pysimultanui-0.3.0/src/PySimultanUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-09 18:48:30.000000 pysimultanui-0.3.0/src/PySimultanUI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      153 2024-06-02 12:42:34.000000 pysimultanui-0.3.0/src/PySimultanUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-02 12:42:34.000000 pysimultanui-0.3.0/src/PySimultanUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.825429 pysimultanui-0.3.0/src/app/
+-rw-rw-rw-   0        0        0        2 2024-04-27 13:04:42.000000 pysimultanui-0.3.0/src/app/__init__.py
+-rw-rw-rw-   0        0        0      856 2024-04-27 13:04:42.000000 pysimultanui-0.3.0/src/app/auth.py
+-rw-rw-rw-   0        0        0      557 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/src/app/home.py
+-rw-rw-rw-   0        0        0     1190 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/src/app/login.py
+-rw-rw-rw-   0        0        0      111 2024-04-27 13:04:42.000000 pysimultanui-0.3.0/src/app/menue.py
+-rw-rw-rw-   0        0        0      304 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/src/app/project.py
+-rw-rw-rw-   0        0        0     3543 2024-06-02 08:36:12.000000 pysimultanui-0.3.0/src/app/theme.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.838127 pysimultanui-0.3.0/src/core/
+-rw-rw-rw-   0        0        0     1042 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/src/core/__init__.py
+-rw-rw-rw-   0        0        0    16790 2024-06-02 09:24:44.000000 pysimultanui-0.3.0/src/core/edit_dialog.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.840648 pysimultanui-0.3.0/src/core/freecad_utils/
+-rw-rw-rw-   0        0        0     2920 2024-06-02 09:17:32.000000 pysimultanui-0.3.0/src/core/freecad_utils/__init__.py
+-rw-rw-rw-   0        0        0     5681 2024-05-10 07:44:30.000000 pysimultanui-0.3.0/src/core/freecad_utils/tools.py
+-rw-rw-rw-   0        0        0     6209 2024-06-02 08:36:12.000000 pysimultanui-0.3.0/src/core/geo_associations.py
+-rw-rw-rw-   0        0        0       61 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/src/core/logging.py
+-rw-rw-rw-   0        0        0    13569 2024-06-02 12:17:08.000000 pysimultanui-0.3.0/src/core/method_mapper.py
+-rw-rw-rw-   0        0        0     3080 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/src/core/navigation.py
+-rw-rw-rw-   0        0        0    22989 2024-06-02 08:36:12.000000 pysimultanui-0.3.0/src/core/project_manager.py
+-rw-rw-rw-   0        0        0      591 2024-04-27 13:04:42.000000 pysimultanui-0.3.0/src/core/tools.py
+-rw-rw-rw-   0        0        0     6854 2024-06-02 08:36:12.000000 pysimultanui-0.3.0/src/core/user.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.854833 pysimultanui-0.3.0/src/views/
+-rw-rw-rw-   0        0        0      196 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/src/views/__init__.py
+-rw-rw-rw-   0        0        0     6718 2024-06-02 08:36:12.000000 pysimultanui-0.3.0/src/views/array_view.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.858041 pysimultanui-0.3.0/src/views/asset_view/
+-rw-rw-rw-   0        0        0       76 2024-04-27 13:04:42.000000 pysimultanui-0.3.0/src/views/asset_view/__init__.py
+-rw-rw-rw-   0        0        0     5344 2024-06-02 08:36:12.000000 pysimultanui-0.3.0/src/views/asset_view/asset_manager.py
+-rw-rw-rw-   0        0        0     1068 2024-05-05 18:09:42.000000 pysimultanui-0.3.0/src/views/asset_view/asset_view.py
+-rw-rw-rw-   0        0        0     4774 2024-06-02 09:50:25.000000 pysimultanui-0.3.0/src/views/component_detail_base_view.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.862548 pysimultanui-0.3.0/src/views/component_dict_view/
+-rw-rw-rw-   0        0        0      110 2024-05-05 18:09:42.000000 pysimultanui-0.3.0/src/views/component_dict_view/__init__.py
+-rw-rw-rw-   0        0        0     1143 2024-05-10 07:09:06.000000 pysimultanui-0.3.0/src/views/component_dict_view/component_dict_manager.py
+-rw-rw-rw-   0        0        0    20237 2024-06-02 10:13:02.000000 pysimultanui-0.3.0/src/views/component_dict_view/component_dict_view.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.865973 pysimultanui-0.3.0/src/views/component_list_view/
+-rw-rw-rw-   0        0        0        0 2024-04-27 13:04:42.000000 pysimultanui-0.3.0/src/views/component_list_view/__init__.py
+-rw-rw-rw-   0        0        0      704 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/src/views/component_list_view/component_list_manager.py
+-rw-rw-rw-   0        0        0    14669 2024-06-02 09:49:26.000000 pysimultanui-0.3.0/src/views/component_list_view/component_list_view.py
+-rw-rw-rw-   0        0        0     3814 2024-06-02 10:44:25.000000 pysimultanui-0.3.0/src/views/detail_views.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.871383 pysimultanui-0.3.0/src/views/geometry_view/
+-rw-rw-rw-   0        0        0       88 2024-04-27 13:04:42.000000 pysimultanui-0.3.0/src/views/geometry_view/__init__.py
+-rw-rw-rw-   0        0        0    11397 2024-06-02 08:36:12.000000 pysimultanui-0.3.0/src/views/geometry_view/geometry_manager.py
+-rw-rw-rw-   0        0        0     7413 2024-06-02 09:59:27.000000 pysimultanui-0.3.0/src/views/geometry_view/geometry_view.py
+-rw-rw-rw-   0        0        0     2830 2024-06-02 08:36:12.000000 pysimultanui-0.3.0/src/views/geometry_view/tools.py
+-rw-rw-rw-   0        0        0     9658 2024-06-02 12:26:38.000000 pysimultanui-0.3.0/src/views/grid_view.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.875634 pysimultanui-0.3.0/src/views/mapped_cls/
+-rw-rw-rw-   0        0        0       49 2024-04-27 13:04:42.000000 pysimultanui-0.3.0/src/views/mapped_cls/__init__.py
+-rw-rw-rw-   0        0        0     2825 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/src/views/mapped_cls/mapped_cls_manager.py
+-rw-rw-rw-   0        0        0    21504 2024-06-02 10:11:02.000000 pysimultanui-0.3.0/src/views/mapped_cls/mapped_cls_view.py
+-rw-rw-rw-   0        0        0     5708 2024-06-02 10:05:30.000000 pysimultanui-0.3.0/src/views/numpy_view.py
+-rw-rw-rw-   0        0        0     6924 2024-06-02 10:07:10.000000 pysimultanui-0.3.0/src/views/pandas_df_view.py
+-rw-rw-rw-   0        0        0     2230 2024-05-05 18:09:42.000000 pysimultanui-0.3.0/src/views/parameter_view.py
+-rw-rw-rw-   0        0        0     2403 2024-05-09 17:27:15.000000 pysimultanui-0.3.0/src/views/type_view.py
+-rw-rw-rw-   0        0        0     7902 2024-06-02 08:36:12.000000 pysimultanui-0.3.0/src/views/type_view_manager.py
+-rw-rw-rw-   0        0        0     7057 2024-06-02 08:36:12.000000 pysimultanui-0.3.0/src/views/view_manager.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:42:34.878067 pysimultanui-0.3.0/tests/
+-rw-rw-rw-   0        0        0    39366 2024-06-02 11:22:16.000000 pysimultanui-0.3.0/tests/test_py_simultan_ui.py
+-rw-rw-rw-   0        0        0     2276 2024-06-02 08:36:12.000000 pysimultanui-0.3.0/tests/test_table.py
```

### Comparing `pysimultanui-0.2.1/LICENSE.txt` & `pysimultanui-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/pyproject.toml` & `pysimultanui-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [project]
 name = "PySimultanUI"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
     {name = "Max Bühler", email = "maximilian.buehler@tuwien.ac.at"}
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 license = {file = "LICENSE.txt"}
+dynamic = ["dependencies"]
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `pysimultanui-0.2.1/setup.py` & `pysimultanui-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 project_dir = Path(__file__).parent
 
 setuptools.setup(
     name="PySimultanUI",
-    version="0.2.1",
+    version="0.3.0",
     description="UI for PySimultan",
     # Allow UTF-8 characters in README with encoding argument.
     long_description=project_dir.joinpath("README.md").read_text(encoding="utf-8"),
     keywords=["python"],
     author="Max Buehler",
     url="",
     packages=setuptools.find_packages("src"),
```

### Comparing `pysimultanui-0.2.1/src/PySimultanUI.egg-info/SOURCES.txt` & `pysimultanui-0.3.0/src/PySimultanUI.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,34 +4,39 @@
 pyproject.toml
 requirements.txt
 setup.py
 src/PySimultanUI.egg-info/PKG-INFO
 src/PySimultanUI.egg-info/SOURCES.txt
 src/PySimultanUI.egg-info/dependency_links.txt
 src/PySimultanUI.egg-info/not-zip-safe
+src/PySimultanUI.egg-info/requires.txt
 src/PySimultanUI.egg-info/top_level.txt
 src/app/__init__.py
 src/app/auth.py
 src/app/home.py
 src/app/login.py
 src/app/menue.py
 src/app/project.py
 src/app/theme.py
 src/core/__init__.py
 src/core/edit_dialog.py
+src/core/geo_associations.py
 src/core/logging.py
 src/core/method_mapper.py
 src/core/navigation.py
 src/core/project_manager.py
 src/core/tools.py
 src/core/user.py
 src/core/freecad_utils/__init__.py
 src/core/freecad_utils/tools.py
 src/views/__init__.py
+src/views/array_view.py
+src/views/component_detail_base_view.py
 src/views/detail_views.py
+src/views/grid_view.py
 src/views/numpy_view.py
 src/views/pandas_df_view.py
 src/views/parameter_view.py
 src/views/type_view.py
 src/views/type_view_manager.py
 src/views/view_manager.py
 src/views/asset_view/__init__.py
@@ -46,8 +51,9 @@
 src/views/geometry_view/__init__.py
 src/views/geometry_view/geometry_manager.py
 src/views/geometry_view/geometry_view.py
 src/views/geometry_view/tools.py
 src/views/mapped_cls/__init__.py
 src/views/mapped_cls/mapped_cls_manager.py
 src/views/mapped_cls/mapped_cls_view.py
-tests/test_py_simultan_ui.py
+tests/test_py_simultan_ui.py
+tests/test_table.py
```

### Comparing `pysimultanui-0.2.1/src/app/auth.py` & `pysimultanui-0.3.0/src/app/auth.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/app/home.py` & `pysimultanui-0.3.0/src/app/home.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/app/login.py` & `pysimultanui-0.3.0/src/app/login.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/app/theme.py` & `pysimultanui-0.3.0/src/app/theme.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 
 
 @contextmanager
 def frame(navtitle: str):
 
     """Custom page frame to share the same styling and behavior across all pages"""
     # ui.colors(primary='#da291c', secondary='#941c13', accent='#941c13', positive='#53B689')
-    with ui.header().classes('justify-between h-25'):
+    with ui.header().classes('justify-between'):
 
         user = user_manager.users[app.storage.user['username']]
 
         # ui.image('web_ui/src/static_files/A1_Digital_identifier_pos_RGB.png').classes('w-32')
 
         with ui.column():
             ui.label('PY Simultan').classes('font-bold text-white text-xl')
-            ui.button(on_click=lambda: (user_manager.user[app.storage.user['username']].logout(),
+            ui.button(on_click=lambda: (user_manager.users[app.storage.user['username']].logout(),
                                         app.storage.user.clear(),
                                         ui.navigate.to('/login')), icon='logout')
 
         with ui.column():
             ui.label(f'Hello {user.name}').classes('text-white text-xl')
 
         # with ui.expansion('Menu', icon='select'):
         with ui.column():
             with ui.tabs() as tabs:
-                ui.button('Mapped Classes', icon='checklist_rtl', on_click=lambda: left_drawer.toggle())
+                # ui.button('Mapped Classes', icon='checklist_rtl', on_click=lambda: left_drawer.toggle())
                 ui.tab('Home', icon='home')
                 ui.tab('Project', icon='edit')
 
                 # ui.button(on_click=lambda: (app.storage.user.clear(),
                 #                             ui.open('/login')),
                 #           icon='logout').props('outline round').classes('text-black')
                 #
@@ -48,37 +48,36 @@
                 #                      icon='logout',
                 #                      on_click=lambda: (app.storage.user.clear(), ui.open('/login')))
 
                 # ui.space()
                 # if app.storage.user.get('username', False):
                 #     ui.label(f'{app.storage.user["username"]}').classes('mr-auto text-2xl')
 
-    with ui.left_drawer(bordered=True,
-                        top_corner=False,
-                        elevated=True,
-                        fixed=True,
-                        value=False).classes('bg-blue-100') as left_drawer:
-        user.navigation_drawer = left_drawer
+    # with ui.left_drawer(bordered=True,
+    #                     top_corner=False,
+    #                     elevated=True,
+    #                     fixed=True,
+    #                     value=False).classes('bg-blue-100') as left_drawer:
+    #     user.navigation_drawer = left_drawer
 
     # with ui.splitter() as splitter:
     #     with splitter.after:
     #         with ui.right_drawer(bordered=True,
     #                              top_corner=False,
     #                              elevated=True,
     #                              fixed=True,
-    #                              value=False).classes('w-full h-full') as detail_drawer:
-    #             with ui.card().classes('w-full h-full') as detail_view:
-    #                 core.detail_view = detail_view
+    #                              value=False).classes('w-full h-full') as detail_view:
+    #             core.detail_view = detail_view
 
     with ui.tab_panels(tabs, value='Home').classes('w-full h-full'):
         with ui.tab_panel('Project').classes('w-full h-full') as project_full_tab:
             with ui.splitter(value=60, limits=(10, 90)).classes('w-full h-full') as splitter:
-                with splitter.before:
+                with splitter.before as project_tab:
                     context.client.content.classes('h-[95vh]')
-                    user.project_tab = ui.scroll_area().classes('w-full h-full')
+                    user.project_tab = project_tab
                 with splitter.after:
-                    user.detail_view = ui.card().classes('w-full h-full')
+                    user.detail_view = ui.row().classes('w-full h-full')
 
         user.home_tab = ui.tab_panel('Home').classes('w-full h-full')
 
     with user.home_tab:
         home.content()
```

### Comparing `pysimultanui-0.2.1/src/core/__init__.py` & `pysimultanui-0.3.0/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/core/edit_dialog.py` & `pysimultanui-0.3.0/src/core/edit_dialog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 from nicegui import ui, app
 
+from numpy import ndarray
+
 from .. import user_manager
+from ..core.user import User
 from .. import core
 from PySimultan2.simultan_object import SimultanObject
 from PySimultan2.files import FileInfo
+from PySimultan2.multi_values import simultan_multi_value_field_3d_to_numpy
 from ..config import logger
 from math import inf
 
+from SIMULTAN.Data.MultiValues import (SimMultiValueField3D, SimMultiValueField3DParameterSource, SimMultiValueBigTable,
+                                       SimMultiValueBigTableHeader, SimMultiValueBigTableParameterSource)
+
+
 
 def get_value_content_type(value):
     if value is None:
         return 'None'
     if isinstance(value, str):
         return 'str'
     elif isinstance(value, int):
@@ -60,19 +68,19 @@
 
     @property
     def value(self):
         return int(self.value_input.value)
 
     @property
     def min(self):
-        return int(self.min_input.value)
+        return int(self.min_input.value) if self.min_input.value != '-inf' else -inf
 
     @property
     def max(self):
-        return int(self.max_input.value)
+        return int(self.max_input.value) if self.max_input.value != 'inf' else inf
 
     @property
     def unit(self):
         return self.unit_input.value
 
 
 class FloatEditDialog(IntEditDialog):
@@ -130,14 +138,15 @@
         if len(self.component_select.value) == 0:
             return None
         elif __len__ := len(self.component_select.value) == 1:
             return self.component_name_map[self.component_select.value[0]]
         else:
             return [self.component_name_map[x] for x in self.component_select.value]
 
+    @ui.refreshable
     def ui_content(self):
         with ui.card():
             ui.label('Select component')
             mapper = user_manager[app.storage.user['username']].mapper
             classes = mapper.mapped_classes
 
             if isinstance(self.component, SimultanObject):
@@ -162,15 +171,20 @@
 
         mapper = user_manager[app.storage.user['username']].mapper
 
         if 'All' in self.class_select.value:
             for cls in mapper.mapped_classes.values():
                 components.extend(cls.cls_instances)
         else:
-            for cls in [mapper.get_mapped_class(x) for x in self.class_select.value]:
+            if isinstance(self.class_select.value, str):
+                selected_val = [self.class_select.value]
+            else:
+                selected_val = self.class_select.value
+
+            for cls in [mapper.get_mapped_class(x) for x in selected_val]:
                 components.extend(cls.cls_instances)
 
         for component in components:
             self.component_name_map[f'{component.name} ({component.id})'] = component
 
         if isinstance(self.component, SimultanObject):
             select_value = [f'{self.component.name} ({self.component.id})']
@@ -223,15 +237,52 @@
     def value(self):
         if len(self.asset_select.value) == 0:
             return None
 
         return self.asset_name_map[self.asset_select.value]
 
 
-default_options = ['None', 'str', 'int', 'float', 'Component', 'Asset']
+class ArrayEditDialog(object):
+
+    def __init__(self, *args, **kwargs):
+        self.array_select = None
+        asset = kwargs.get('array', None)
+
+        self.array: SimMultiValueField3D = asset if isinstance(asset, ndarray) else None
+        self.content = kwargs.get('content', None)
+        self.parent = kwargs.get('parent', None)
+        self.dialog = None
+
+        self.array_name_map = {}
+
+    @property
+    def user(self) -> User:
+        return user_manager[app.storage.user['username']]
+
+    def ui_content(self):
+        with ui.card():
+            ui.label('Select Array')
+            arrays = self.user.array_manager.np_items
+            self.array_name_map = {x.Name: x for x in arrays.values()}
+            self.array_select = ui.select([x.Name for x in arrays.values()],
+                                          label='Select asset',
+                                          value=self.array.Name if self.array is not None else None,
+                                          on_change=self.array_select,
+                                          with_input=True
+                                          ).classes('w-64').props('use-chips')
+
+    @property
+    def value(self):
+        if len(self.array_select.value) == 0:
+            return None
+
+        return self.array_name_map[self.array_select.value]
+
+
+default_options = ['None', 'str', 'int', 'float', 'bool', 'Component', 'Asset', 'Array', 'Table']
 
 
 class ContentTypeChooser(object):
 
     def __init__(self, *args, **kwargs):
         self.content_type = kwargs.get('content_type', str)
         self.select = None
@@ -317,41 +368,49 @@
                                                    select_multiple=self.select_multiple)
             self.edit_dialog.ui_content()
         elif self.content_type.select.value == 'Asset':
             self.edit_dialog = AssetEditDialog(asset=self.component,
                                                content=self.content,
                                                parent=self.parent)
             self.edit_dialog.ui_content()
+        elif self.content_type.select.value == 'Array':
+            self.edit_dialog = ArrayEditDialog(array=self.component,
+                                               content=self.content,
+                                               parent=self.parent)
+            self.edit_dialog.ui_content()
         else:
             ui.label('Not implemented content type!')
 
     def on_type_change(self):
         self.ui_content.refresh()
 
     def close(self, *args, **kwargs):
         if self.dialog is not None:
             self.dialog.close()
             self.dialog = None
 
     def save(self, *args, **kwargs):
-        setattr(self.parent.component, self.content.property_name, self.edit_dialog.value)
 
+        setattr(self.parent.component, self.content.property_name, self.edit_dialog.value)
         if self.content_type.select.value in ['int', 'float']:
             if self.raw_val is None:
                 self.raw_val = self.parent.component.get_raw_attr(self.content.property_name)
             setattr(self.raw_val, 'ValueMin', self.edit_dialog.min)
             setattr(self.raw_val, 'ValueMax', self.edit_dialog.max)
             setattr(self.raw_val, 'Unit', self.edit_dialog.unit)
 
         logger.info(f'Updated {self.content.name} to {self.edit_dialog.value}')
 
         if self.parent is not None:
             self.parent.refresh()
         self.close()
 
+        from ..views.detail_views import show_detail
+        show_detail(value=self.parent.component)
+
 
 class DictEditDialog(object):
 
     def __init__(self, *args, **kwargs):
         self.component = kwargs.get('component', None)
         self._key = None
```

### Comparing `pysimultanui-0.2.1/src/core/freecad_utils/tools.py` & `pysimultanui-0.3.0/src/core/freecad_utils/tools.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/core/navigation.py` & `pysimultanui-0.3.0/src/core/navigation.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/core/project_manager.py` & `pysimultanui-0.3.0/src/core/project_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import os
 import asyncio
 from copy import deepcopy
+from ..core import mapper
 from logging import getLogger
 from typing import Optional, Type
 from datetime import datetime
 from nicegui import app, ui, events
 from PySimultan2.data_model import DataModel
 from PySimultan2.object_mapper import PythonMapper
-from PySimultan2.files import FileInfo
-from PySimultan2.geometry.geometry_base import GeometryModel
-from PySimultan2 import config as py_simultan_config
 
 from .. import user_manager
-from .. import core
 from ..core.user import UserManager, User
 from ..views.view_manager import ViewManager
 from ..views.asset_view import AssetManager
 from ..views.geometry_view import GeometryManager
 from ..core.navigation import Navigation
 # from ..views.geometry_view.geometry_file_manager import GeometryFileManager
 # from ..views.asset_view.asset_manager import AssetManager
@@ -383,26 +380,34 @@
         return self.user.mapper
 
     @mapper.setter
     def mapper(self, value: PythonMapper):
         self.user.mapper = value
 
     @property
+    def grid_view(self):
+        return self.user.grid_view
+
+    @property
     def view_manager(self) -> ViewManager:
         return self.user.view_manager
 
     @property
     def asset_manager(self) -> AssetManager:
         return self.user.asset_manager
 
     @property
     def geometry_manager(self) -> GeometryManager:
         return self.user.geometry_manager
 
     @property
+    def array_manager(self):
+        return self.user.array_manager
+
+    @property
     def navigation(self) -> Navigation:
         return self.user.navigation
 
     @property
     def detail_view(self):
         return self.user.detail_view
 
@@ -425,15 +430,15 @@
     @data_model.setter
     def data_model(self, value: Optional[DataModel]):
         logger.debug(f'Setting data model to {value}')
         self.user.data_model = value
         if self.user.data_model is not None:
             app.add_static_files('/assets', self.user.data_model.project.ProjectUnpackFolder.FullPath)
 
-        for item in [self.view_manager, self.asset_manager, self.geometry_manager]:
+        for item in [self.view_manager, self.asset_manager, self.geometry_manager, self.grid_view, self.array_manager]:
             if item is not None:
                 item.data_model = self.user.data_model
 
     @property
     def projects(self):
         # get list of files in project_dir
         self._projects = os.listdir(project_dir)
@@ -448,29 +453,42 @@
                        *args,
                        **kwargs):
 
         shutil.copyfileobj(e.content, open(f'{project_dir}/{e.name}', 'wb'))
         ui.notify(f'Project {e.name} uploaded!')
         self.project_list.ui_content.refresh()
 
-    def refresh_all_items(self, e):
-        self.view_manager.refresh_all_items()
+    def refresh_all_items(self, *args, **kwargs):
+        # self.view_manager.refresh_all_items()
+        self.grid_view.ui_content.refresh()
         self.asset_manager.update_items_views()
         self.geometry_manager.update_items_views()
-        self.navigation.ui_content.refresh()
+        # self.navigation.ui_content.refresh()
 
     def ui_content(self):
         with self.project_tab:
-            self.view_manager.ui_content()
-            self.asset_manager.ui_content()
-            self.geometry_manager.ui_content()
-            self.navigation.ui_content()
+            with ui.tabs() as tabs:
+                ui.tab('Components', icon='category', label='')
+                ui.tab('Assets', icon='description', label='')
+                ui.tab('Geometry', icon='shape_line', label='')
+                ui.tab('Arrays', icon='data_array', label='')
+
+            with ui.tab_panels(tabs, value='Components').classes('w-full h-full').props('vertical'):
+                with ui.tab_panel('Components').classes('w-full h-full'):
+                    self.grid_view.ui_content()
+                # self.view_manager.ui_content()
+                with ui.tab_panel('Assets').classes('w-full h-full'):
+                    self.asset_manager.ui_content()
+                with ui.tab_panel('Geometry').classes('w-full h-full'):
+                    self.geometry_manager.ui_content()
+
+                with ui.tab_panel('Arrays').classes('w-full h-full'):
+                    self.array_manager.ui_content()
 
-            with ui.page_sticky(position='bottom-right', x_offset=20, y_offset=20):
-                ui.button(on_click=self.refresh_all_items, icon='update').props('fab color=accent')
+            # self.navigation.ui_content()
 
         if self.data_model is None:
             selected = None
         else:
             selected = os.path.basename(self.data_model.project.ProjectFile.FullPath)
 
         self.project_list = ProjectList(project_manager=self,
@@ -486,14 +504,16 @@
         ui.upload(label='Upload simultan project',
                   on_upload=self.upload_project).on(
             'finish', lambda: ui.notify('Finish!')
         ).classes('max-w-full')
 
     def open_project(self, e: events.ClickEventArguments = None, *args, **kwargs):
 
+        self.mapper = self.mapper.copy()
+
         if e is not None:
             project = e.sender.project
         else:
             project = kwargs.get('project', None)
 
         logger.info(f'Opening project {project.project}')
```

### Comparing `pysimultanui-0.2.1/src/core/tools.py` & `pysimultanui-0.3.0/src/core/tools.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/core/user.py` & `pysimultanui-0.3.0/src/core/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from copy import deepcopy
 from typing import Union, Optional
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .method_mapper import MethodMapper
     from PySimultan2.data_model import DataModel
     from PySimultan2.object_mapper import PythonMapper
@@ -74,17 +75,19 @@
 class User:
 
     def __init__(self, *args, **kwargs):
 
         from ..core import method_mapper, mapper
 
         self._project_manager = None
+        self._grid_view = None
         self._view_manager = None
         self._asset_manager = None
         self._geometry_manager = None
+        self._array_manager = None
         self._navigation = None
         self._data_model = None
 
         self.user_manager = kwargs.get('user_manager', None)
         self.detail_history = DetailHistory()
 
         self.name = kwargs.get('name', None)
@@ -92,63 +95,77 @@
         self.password = kwargs.get('password', None)
 
         self.mapper: Optional[PythonMapper] = kwargs.get('mapper', mapper)
         self.method_mapper: Optional[MethodMapper] = kwargs.get('method_mapper', method_mapper)
         self.data_model: Union[DataModel, None] = kwargs.get('data_model', None)
 
         self.navigation_drawer = kwargs.get('navigation_drawer', None)
-        self.project_tab = kwargs.get('navigation_drawer', None)
-        self.detail_view = kwargs.get('navigation_drawer', None)
-        self.home_tab = kwargs.get('navigation_drawer', None)
+        self.project_tab = kwargs.get('project_tab', None)
+        self.detail_view = kwargs.get('detail_view', None)
+        self.home_tab = kwargs.get('home_tab', None)
 
     @property
     def data_model(self):
         return self._data_model
 
     @data_model.setter
     def data_model(self, value):
         self._data_model = value
         if self.detail_history is not None:
             self.detail_history = DetailHistory()
 
     @property
+    def grid_view(self):
+        if self._grid_view is None:
+            from ..views.grid_view import GridView
+            self._grid_view = GridView()
+        return self._grid_view
+
+    @property
     def project_manager(self):
         if self._project_manager is None:
             from .project_manager import ProjectManager
             self._project_manager = ProjectManager(user_manager=self.user_manager,
                                                    mapper=self.mapper)
         return self._project_manager
 
     @property
     def view_manager(self):
-        if self._view_manager is None:
-            from ..views.view_manager import ViewManager
-            self._view_manager = ViewManager(mapper=self.mapper,
-                                             parent=self.project_manager)
+        # if self._view_manager is None:
+        #     from ..views.view_manager import ViewManager
+        #     self._view_manager = ViewManager(mapper=self.mapper,
+        #                                      parent=self.project_manager)
         return self._view_manager
 
     @property
     def asset_manager(self):
         if self._asset_manager is None:
             from ..views.asset_view import AssetManager
             self._asset_manager = AssetManager()
         return self._asset_manager
 
     @property
+    def array_manager(self):
+        if self._array_manager is None:
+            from ..views.array_view import ArrayManager
+            self._array_manager = ArrayManager()
+        return self._array_manager
+
+    @property
     def geometry_manager(self):
         if self._geometry_manager is None:
             from ..views.geometry_view import GeometryManager
             self._geometry_manager = GeometryManager(data_model=self.data_model)
         return self._geometry_manager
 
     @property
     def navigation(self):
-        if self._navigation is None:
-            from .navigation import Navigation
-            self._navigation = Navigation()
+        # if self._navigation is None:
+        #     from .navigation import Navigation
+        #     self._navigation = Navigation()
         return self._navigation
 
     def logout(self):
         self.data_model = None
 
 
 class Admin(User):
```

### Comparing `pysimultanui-0.2.1/src/views/asset_view/asset_view.py` & `pysimultanui-0.3.0/src/views/asset_view/asset_view.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/views/component_dict_view/component_dict_manager.py` & `pysimultanui-0.3.0/src/views/component_dict_view/component_dict_manager.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/views/component_list_view/component_list_manager.py` & `pysimultanui-0.3.0/src/views/component_list_view/component_list_manager.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/views/detail_views.py` & `pysimultanui-0.3.0/src/views/detail_views.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 from pandas import DataFrame
 # import pandas as pd
 
 from nicegui import ui, app
 from logging import getLogger
 from PySimultan2.simultan_object import SimultanObject
 from PySimultan2.geometry import GeometryModel
-# from PySimultan2.default_types import ComponentDictionary, ComponentList
+from PySimultan2.default_types import ComponentDictionary, ComponentList
 
 from SIMULTAN.Data.MultiValues import (SimMultiValueField3D, SimMultiValueField3DParameterSource, SimMultiValueBigTable,
                                        SimMultiValueBigTableHeader, SimMultiValueBigTableParameterSource)
 
 from .. import user_manager
 
 from .pandas_df_view import DataFrameDetailView
 from .numpy_view import NDArrayDetailView
 from .geometry_view.geometry_view import GeometryDetailView
+from .component_list_view.component_list_view import ListDetailView
+from .component_dict_view.component_dict_view import DictDetailView
+from .mapped_cls.mapped_cls_view import MappedClsDetailView
 
 
 logger = getLogger('py_simultan_ui')
 
 
 def show_next_detail(*args, **kwargs):
     user = user_manager[app.storage.user['username']]
@@ -35,15 +38,15 @@
 def show_detail(value, *args, **kwargs):
     user = user_manager[app.storage.user['username']]
     user.detail_history.add_item(value)
     # current_detail = user.detail_history[-1] if user.detail_history else None
     logger.debug(f'Showing details for {value}')
     user.detail_view.clear()
     with user.detail_view:
-        with ui.card().classes('w-full h-full'):
+        with ui.card().classes('w-full'):
             with ui.row():
                 previous_detail = user.detail_history.get_previous_detail()
                 if previous_detail is not None:
                     ui.button(on_click=show_previous_detail,
                               icon='arrow_back').classes('q-mr-md')
                 ui.space()
                 next_detail = user.detail_history.get_next_detail()
@@ -55,14 +58,20 @@
 
             if isinstance(value, SimMultiValueBigTable):
                 detail_view = DataFrameDetailView(component=value, **kwargs)
             elif isinstance(value, SimMultiValueField3D):
                 detail_view = NDArrayDetailView(component=value, **kwargs)
             elif isinstance(value, GeometryModel):
                 detail_view = GeometryDetailView(component=value, **kwargs)
+            elif isinstance(value, ComponentList):
+                detail_view = ListDetailView(component=value, **kwargs)
+            elif isinstance(value, ComponentDictionary):
+                detail_view = DictDetailView(component=value, **kwargs)
+            elif isinstance(value, SimultanObject):
+                detail_view = MappedClsDetailView(component=value, **kwargs)
             else:
                 cls_view = user.view_manager.cls_views.get(value.__class__, None)
                 if cls_view is None:
                     ui.label(f'No view for {value.__class__}')
                     return
                 type_view = cls_view.get('type_view', None)
                 if type_view is None:
```

### Comparing `pysimultanui-0.2.1/src/views/geometry_view/tools.py` & `pysimultanui-0.3.0/src/views/geometry_view/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     stl_dir = os.path.join('/static/stl', str(geometry_model.key))
     if not os.path.exists(stl_dir):
         os.makedirs(stl_dir)
 
     file_lookup = {}
 
     for face in geometry_model.faces:
-
         face._wrapped_object.Color
-
         filename = os.path.join(stl_dir, f"{face.id}.stl")
         file_lookup[face.id] = (os.path.join('/stl', str(geometry_model.key), f"{face.id}.stl"),
                                 rgba_to_hex((getattr(face._wrapped_object.Color.Color,
                                                      key) for key in ('R', 'G', 'B', 'A')))
                                 )
         vertices, triangles = face.triangulate()
         write_stl_from_numpy(vertices, triangles, filename=filename)
```

### Comparing `pysimultanui-0.2.1/src/views/mapped_cls/mapped_cls_manager.py` & `pysimultanui-0.3.0/src/views/mapped_cls/mapped_cls_manager.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/views/numpy_view.py` & `pysimultanui-0.3.0/src/views/numpy_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,59 +21,49 @@
         self.component: SimMultiValueField3D = kwargs.get('component')
         self.parent = kwargs.get('parent')
         self.array = None
         self.dim_slider = None
         self.table = None
 
     def ui_content(self, *args, **kwargs):
-        from .detail_views import show_detail
-        detail_view = user_manager[app.storage.user['username']].detail_view
 
-        detail_view.clear()
-        with detail_view:
-            with ui.card().classes('w-full h-full'):
-                if kwargs.get('previous', None) is not None:
-                    with ui.row():
-                        ui.button(on_click=lambda e: show_detail(kwargs.get('previous')),
-                                  icon='arrow_back').classes('q-mr-md')
+        from .detail_views import show_detail
 
+        with ui.row().classes('w-full'):
+            ui.input(label='Name',
+                     value=self.component.Name).classes('w-full').bind_value(self.component, 'Name')
+        with ui.row().classes('w-full'):
+            ui.label('ID:').classes('w-full')
+            with ui.row():
+                with ui.row():
+                    ui.label(f'{self.component.Id.GlobalId.ToString()}')
                 with ui.row():
-                    ui.input(label='Name',
-                             value=self.component.Name).classes('w-full h-full').bind_value(self.component,
-                                                                                            'Name')
-                with ui.row().classes('w-full h-full'):
-                    ui.label('ID:')
-                    with ui.row():
-                        with ui.row():
-                            ui.label(f'{self.component.Id.GlobalId.ToString()}')
-                        with ui.row():
-                            ui.label(f'{self.component.Id.LocalId}')
-
-                self.array = simultan_multi_value_field_3d_to_numpy(self.component)
-
-                with ui.row().classes('w-full h-full'):
-                    with ui.column():
-                        ui.label('Shape:')
-                        ui.label(f'{self.array.shape}')
-
-                ui.separator()
-
-                self.table_ui_content()
-
-                with ui.card().classes('w-full h-full'):
-                    ui.label('Select dimension to display:')
-                    self.dim_slider = ui.slider(min=0, max=self.array.shape[0] - 1,
-                                                step=1,
-                                                value=0,
-                                                on_change=self.table_ui_content.refresh)
-                    ui.input('dim_slider',
-                             value='0').bind_value(self.dim_slider,
-                                                   'value',
-                                                   forward=lambda x: int(x),
-                                                   backward=lambda x: str(x))
+                    ui.label(f'{self.component.Id.LocalId}')
+
+        self.array = simultan_multi_value_field_3d_to_numpy(self.component)
+
+        with ui.row().classes('w-full'):
+            with ui.column():
+                ui.label('Shape:')
+                ui.label(f'{self.array.shape}')
+
+        ui.separator()
+
+        self.table_ui_content()
+
+        with ui.card().classes('w-full h-full'):
+            ui.label('Dimension to display:')
+            self.dim_slider = ui.slider(min=0, max=self.array.shape[0] - 1,
+                                        step=1,
+                                        value=0,
+                                        on_change=self.table_ui_content.refresh)
+            ui.input(value='0').bind_value(self.dim_slider,
+                                           'value',
+                                           forward=lambda x: int(x),
+                                           backward=lambda x: str(x))
 
     @ui.refreshable
     def table_ui_content(self):
 
         if self.array.shape.__len__() > 2:
             disp_array = self.array[int(self.dim_slider.value if self.dim_slider is not None else 0), :, :]
         else:
```

### Comparing `pysimultanui-0.2.1/src/views/pandas_df_view.py` & `pysimultanui-0.3.0/src/views/pandas_df_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,27 @@
         self.parent = kwargs.get('parent')
         self.array = None
         self.dim_slider = None
         self.table = None
 
     def ui_content(self, *args, **kwargs):
 
-        with ui.row().classes('w-full h-full'):
+        with ui.row().classes('w-full'):
             ui.input(label='Name',
-                     value=self.component.Name).classes('w-full h-full').bind_value(self.component,
+                     value=self.component.Name).classes('w-full').bind_value(self.component,
                                                                                     'Name')
-        with ui.row().classes('w-full h-full'):
+        with ui.row().classes('w-full'):
             with ui.column():
                 ui.label('ID:')
                 ui.label(f'{str(self.component.Id.GlobalId.ToString())}')
                 ui.label(f'{str(self.component.Id.LocalId)}')
 
         df = simultan_multi_value_big_table_to_pandas(self.component)
 
-        with ui.row().classes('w-full h-full'):
+        with ui.row().classes('w-full'):
             with ui.column():
                 ui.label('Shape:')
                 ui.label(f'{df.shape}')
 
         ui.separator()
 
         table = ui.table.from_pandas(df).classes('w-full h-full')
```

### Comparing `pysimultanui-0.2.1/src/views/parameter_view.py` & `pysimultanui-0.3.0/src/views/parameter_view.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/views/type_view.py` & `pysimultanui-0.3.0/src/views/type_view.py`

 * *Files identical despite different names*

### Comparing `pysimultanui-0.2.1/src/views/type_view_manager.py` & `pysimultanui-0.3.0/src/views/type_view_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,21 +99,23 @@
         self.ui_content.refresh()
 
     @ui.refreshable
     def ui_content(self):
 
         logger.info(f'Creating UI content for TVM {self.taxonomy}')
 
-        with ui.expansion(icon='format_list_bulleted',
-                          text=f'{self.item_view_name if self.item_view_name is not None else self.cls._taxonomy} '
-                               f'({len(self.items)})'
-                          ).classes('w-full h-full').bind_text_from(self,
-                                                                    'items',
-                                                                    lambda x: f'{self.item_view_name} ({len(x)})'
-                                                                    ) as self.expansion:
+        with ui.row().classes('w-full h-full') as self.expansion:
+
+        # with ui.expansion(icon='format_list_bulleted',
+        #                   text=f'{self.item_view_name if self.item_view_name is not None else self.cls._taxonomy} '
+        #                        f'({len(self.items)})'
+        #                   ).classes('w-full h-full').bind_text_from(self,
+        #                                                             'items',
+        #                                                             lambda x: f'{self.item_view_name} ({len(x)})'
+        #                                                             ) as self.expansion:
             self.ui_expand_content()
 
     @ui.refreshable
     def ui_expand_content(self):
 
         logger.info(f'Creating UI expand content for TVM {self.taxonomy}')
```

### Comparing `pysimultanui-0.2.1/src/views/view_manager.py` & `pysimultanui-0.3.0/src/views/view_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             # new_tvm.cls.__init__ = __init__
 
             new_tvm.item_view_cls = MappedClsView
             new_tvm.item_view_name = taxonomy
             new_tvm.view_manager = self
             self.cls_views[new_tvm.cls] = {'item_view_manager': new_tvm, 'type_view': MappedClsView}
 
-            with core.project_tab:
+            with self.user.project_manager.project_tab:
                 new_tvm.ui_content()
 
         return self.cls_views.get(cls, None)
 
     def create_tvms(self):
 
         logger.debug('Creating TypeViewManagers...')
```

### Comparing `pysimultanui-0.2.1/tests/test_py_simultan_ui.py` & `pysimultanui-0.3.0/tests/test_py_simultan_ui.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-from typing import List
+from typing import List, Optional
 import os
 import numpy as np
 import pandas as pd
 from py_simultan_ui.src.main_ui import run_ui
 from py_simultan_ui.src.core import mapper, method_mapper, mapped_method
 from PySimultan2.taxonomy_maps import TaxonomyMap, Content
 from PySimultan2 import DataModel
 from tests import resources
 from PySimultan2.geometry.geometry_base import (GeometryModel, SimultanLayer, SimultanVertex, SimultanEdge,
-                                                    SimultanEdgeLoop, SimultanFace, SimultanVolume)
+                                                SimultanEdgeLoop, SimultanFace, SimultanVolume)
 from PySimultan2.geometry.utils import create_cube
 # from py_simultan_ui.src.core.method_mapper import method_mapper, mapped_method
 
 project_dir = os.environ.get('PROJECT_DIR', '/simultan_projects')
 if not os.path.exists(project_dir):
     os.makedirs(project_dir)
 
-data_model = DataModel.create_new_project(project_path=os.path.join(project_dir, 'steady_state.simultan'),
-                                          user_name='admin',
-                                          password='admin')
+new_data_model = DataModel.create_new_project(project_path=os.path.join(project_dir, 'steady_state.simultan'),
+                                              user_name='admin',
+                                              password='admin')
 
 
-def create_geometry_model(name='new_geometry_test'):
+def create_geometry_model(name='new_geometry_test',
+                          data_model: DataModel = new_data_model):
     return GeometryModel(name=name,
                          data_model=data_model)
 
 
 def create_classes() -> dict[str, type]:
 
     class TypeTestClass(object):
@@ -68,15 +69,15 @@
             self.density = kwargs.get('density', 1000)
             self.specific_heat = kwargs.get('specific_heat', 800)
 
     class WallLayer(object):
         def __init__(self, *args, **kwargs):
             self.name = kwargs.get('name')
             self.thickness = kwargs.get('thickness', 0.10)
-            self.material: Material = kwargs.get('material')
+            self.material: Optional[Material] = kwargs.get('material', None)
 
         @property
         def r_value(self):
             return self.thickness / self.material.thermal_conductivity
 
     class Construction(object):
         def __init__(self, *args, **kwargs):
@@ -143,23 +144,50 @@
             phi_hc_id = sum(x.heat_flux for x in self.sources)
 
             t_steady = (sum(x[0] for x in phi_ti) + phi_hc_id) / sum(x[1] for x in phi_ti)
             self.steady_state_temperature = t_steady
 
             return t_steady
 
+    class Volume(object):
+        def __init__(self, *args, **kwargs):
+            self.name = kwargs.get('name')
+            self.geometry_file = kwargs.get('geometry_file')
+
+    class Mesh(object):
+        def __init__(self, *args, **kwargs):
+            self.name = kwargs.get('name')
+            self.mesh_file = kwargs.get('mesh_file')
+
+    class Assembly(object):
+        def __init__(self, *args, **kwargs):
+            self.name = kwargs.get('name', 'Unnamed Assembly')
+            self.volumes = kwargs.get('volumes', [])
+            self.mesh = kwargs.get('mesh', None)
+            self.features = kwargs.get('features', [])
+
+    class ReferenceFace(object):
+        def __init__(self, *args, **kwargs):
+            self.construction: Construction = kwargs.get('construction')
+            self.assembly: Assembly = kwargs.get('assembly')
+            self.mesh_size = 15
+
     cls_dict = {'Material': Material,
                 'WallLayer': WallLayer,
                 'Wall': Wall,
                 'Zone': Zone,
                 'TemperatureBoundaryCondition': TemperatureBoundaryCondition,
                 'HeatFluxBoundaryCondition': HeatFluxBoundaryCondition,
                 'Source': Source,
                 'Construction': Construction,
-                'TypeTestClass': TypeTestClass}
+                'TypeTestClass': TypeTestClass,
+                'Assembly': Assembly,
+                'ReferenceFace': ReferenceFace,
+                'Volume': Volume,
+                'Mesh': Mesh}
 
     return cls_dict
 
 
 def create_mapped_classes(classes: dict[str, type]) -> dict[str, type]:
 
     def create_contents() -> dict[str, Content]:
@@ -295,54 +323,96 @@
         contents['str_value'] = Content(text_or_key='str_value',
                                         property_name='str_value',
                                         type=str,
                                         unit=None,
                                         documentation='str_value')
 
         contents['bool_value'] = Content(text_or_key='bool_value',
-                                            property_name='bool_value',
-                                            type=bool,
-                                            unit=None,
-                                            documentation='bool_value')
+                                         property_name='bool_value',
+                                         type=bool,
+                                         unit=None,
+                                         documentation='bool_value')
 
         contents['list_value'] = Content(text_or_key='list_value',
-                                            property_name='list_value',
-                                            type=list,
-                                            unit=None,
-                                            documentation='list_value')
+                                         property_name='list_value',
+                                         type=list,
+                                         unit=None,
+                                         documentation='list_value')
 
         contents['dict_value'] = Content(text_or_key='dict_value',
-                                            property_name='dict_value',
-                                            type=dict,
-                                            unit=None,
-                                            documentation='dict_value')
+                                         property_name='dict_value',
+                                         type=dict,
+                                         unit=None,
+                                         documentation='dict_value')
 
         contents['none_value'] = Content(text_or_key='none_value',
-                                            property_name='none_value',
-                                            type=None,
-                                            unit=None,
-                                            documentation='none_value')
+                                         property_name='none_value',
+                                         type=None,
+                                         unit=None,
+                                         documentation='none_value')
 
         contents['obj_value'] = Content(text_or_key='obj_value',
                                         property_name='obj_value',
                                         type=None,
                                         unit=None,
                                         documentation='obj_value')
 
         contents['numpy_value'] = Content(text_or_key='numpy_value',
-                                            property_name='numpy_value',
-                                            type=None,
-                                            unit=None,
-                                            documentation='numpy_value')
+                                          property_name='numpy_value',
+                                          type=None,
+                                          unit=None,
+                                          documentation='numpy_value')
 
         contents['pandas_value'] = Content(text_or_key='pandas_value',
-                                            property_name='pandas_value',
+                                           property_name='pandas_value',
+                                           type=None,
+                                           unit=None,
+                                           documentation='pandas_value')
+
+        contents['assembly'] = Content(text_or_key='assembly',
+                                       property_name='assembly',
+                                       type=None,
+                                       unit=None,
+                                       documentation='assembly')
+
+        contents['volumes'] = Content(text_or_key='volumes',
+                                      property_name='volumes',
+                                      type=None,
+                                      unit=None,
+                                      documentation='volumes')
+
+        contents['features'] = Content(text_or_key='features',
+                                       property_name='features',
+                                       type=None,
+                                       unit=None,
+                                       documentation='features')
+
+        contents['mesh'] = Content(text_or_key='mesh',
+                                   property_name='mesh',
+                                   type=None,
+                                   unit=None,
+                                   documentation='mesh')
+
+        contents['geometry_file'] = Content(text_or_key='geometry_file',
+                                            property_name='geometry_file',
                                             type=None,
                                             unit=None,
-                                            documentation='pandas_value')
+                                            documentation='geometry_file')
+
+        contents['mesh_file'] = Content(text_or_key='mesh_file',
+                                        property_name='mesh_file',
+                                        type=None,
+                                        unit=None,
+                                        documentation='mesh_file')
+
+        contents['mesh_size'] = Content(text_or_key='mesh_size',
+                                        property_name='mesh_size',
+                                        type=float,
+                                        unit='cm',
+                                        documentation='mesh_size')
 
         return contents
 
     def create_mapped_type_test_class(cls, contents: dict[str, Content]):
         cls_map = TaxonomyMap(taxonomy_name='PySimultan',
                               taxonomy_key='PySimultan',
                               taxonomy_entry_name='TypeTestClass',
@@ -467,185 +537,297 @@
                                        contents['heat_flux']],
                               )
 
         mapper.register(cls_map.taxonomy_entry_key, cls, taxonomy_map=cls_map)
         mapped_cls = mapper.get_mapped_class(cls_map.taxonomy_entry_key)
         return mapped_cls
 
+    def create_reference_face_cls(cls, contents: dict[str, Content]):
+        cls_map = TaxonomyMap(taxonomy_name='PySimultan',
+                              taxonomy_key='PySimultan',
+                              taxonomy_entry_name='ReferenceFace',
+                              taxonomy_entry_key='ReferenceFace',
+                              content=[contents['construction'],
+                                       contents['assembly'],
+                                       contents['mesh_size']
+                                       ],
+                              )
+        mapper.register(cls_map.taxonomy_entry_key, cls, taxonomy_map=cls_map)
+        mapped_cls = mapper.get_mapped_class(cls_map.taxonomy_entry_key)
+        return mapped_cls
+
+    def create_assembly_cls(cls, contents: dict[str, Content]):
+
+        cls_map = TaxonomyMap(taxonomy_name='PySimultan',
+                              taxonomy_key='PySimultan',
+                              taxonomy_entry_name='Assembly',
+                              taxonomy_entry_key='Assembly',
+                              content=[contents['volumes'],
+                                       contents['mesh'],
+                                       contents['features']],
+                              )
+
+        mapper.register(cls_map.taxonomy_entry_key, cls, taxonomy_map=cls_map)
+        mapped_cls = mapper.get_mapped_class(cls_map.taxonomy_entry_key)
+        return mapped_cls
+
+    def create_volume_cls(cls, contents: dict[str, Content]):
+        cls_map = TaxonomyMap(taxonomy_name='PySimultan',
+                              taxonomy_key='PySimultan',
+                              taxonomy_entry_name='Volume',
+                              taxonomy_entry_key='Volume',
+                              content=[contents['geometry_file']],
+                              )
+
+        mapper.register(cls_map.taxonomy_entry_key, cls, taxonomy_map=cls_map)
+        mapped_cls = mapper.get_mapped_class(cls_map.taxonomy_entry_key)
+        return mapped_cls
+
+    def create_mesh_cls(cls, contents: dict[str, Content]):
+        cls_map = TaxonomyMap(taxonomy_name='PySimultan',
+                              taxonomy_key='PySimultan',
+                              taxonomy_entry_name='Mesh',
+                              taxonomy_entry_key='Mesh',
+                              content=[contents['mesh_file']],
+                              )
+
+        mapper.register(cls_map.taxonomy_entry_key, cls, taxonomy_map=cls_map)
+        mapped_cls = mapper.get_mapped_class(cls_map.taxonomy_entry_key)
+        return mapped_cls
+
     tax_contents = create_contents()
 
     mapped_type_test_class = create_mapped_type_test_class(classes['TypeTestClass'], tax_contents)
     mapped_material_cls = create_mapped_material(classes['Material'], tax_contents)
     mapped_layer_cls = create_layer_cls(classes['WallLayer'], tax_contents)
     mapped_construction_cls = create_construction_cls(classes['Construction'], tax_contents)
     mapped_wall_cls = create_wall_cls(classes['Wall'], tax_contents)
     mapped_zone_cls = create_zone_cls(classes['Zone'], tax_contents)
     mapped_temperature_bc_cls = create_temperature_bc_cls(classes['TemperatureBoundaryCondition'], tax_contents)
     mapped_heat_flux_bc_cls = create_heat_flux_bc_cls(classes['HeatFluxBoundaryCondition'], tax_contents)
     mapped_source_cls = create_source_cls(classes['Source'], tax_contents)
+    mapped_reference_face_cls = create_reference_face_cls(classes['ReferenceFace'], tax_contents)
+    mapped_assembly_cls = create_assembly_cls(classes['Assembly'], tax_contents)
+    mapped_volume_cls = create_volume_cls(classes['Volume'], tax_contents)
+    mapped_mesh_cls = create_mesh_cls(classes['Mesh'], tax_contents)
 
     mapped_cls_dict = {'Material': mapped_material_cls,
                        'Layer': mapped_layer_cls,
                        'Construction': mapped_construction_cls,
                        'Wall': mapped_wall_cls,
                        'Zone': mapped_zone_cls,
                        'TemperatureBoundaryCondition': mapped_temperature_bc_cls,
                        'HeatFluxBoundaryCondition': mapped_heat_flux_bc_cls,
                        'Source': mapped_source_cls,
-                       'TypeTestClass': mapped_type_test_class}
+                       'TypeTestClass': mapped_type_test_class,
+                       'Assembly': mapped_assembly_cls,
+                       'ReferenceFace': mapped_reference_face_cls,
+                       'Volume': mapped_volume_cls,
+                       'Mesh': mapped_mesh_cls}
 
     return mapped_cls_dict
 
 
-def init_project():
-    geo_model = create_geometry_model(name='new_geometry_test')
-
+def create_new_steady_state_zone(mapped_classes,
+                                 data_model: Optional[DataModel] = None):
+    geo_model = create_geometry_model(name='new_geometry_test',
+                                      data_model=data_model)
     cube = create_cube(data_model, geo_model, scale=10)
-
-    classes = create_classes()
-    mapped_classes = create_mapped_classes(classes)
-
     TypeTestClass = mapped_classes['TypeTestClass']
     Material = mapped_classes['Material']
     WallLayer = mapped_classes['Layer']
     Construction = mapped_classes['Construction']
     Wall = mapped_classes['Wall']
     Zone = mapped_classes['Zone']
     TemperatureBoundaryCondition = mapped_classes['TemperatureBoundaryCondition']
     HeatFluxBoundaryCondition = mapped_classes['HeatFluxBoundaryCondition']
     Source = mapped_classes['Source']
-
-    type_test = TypeTestClass(name='type_test',
-                              int_value=1,
-                              float_value=1.0,
-                              str_value='test',
-                              bool_value=True,
-                              list_value=[Material(name='material 1'),
-                                          Material(name='material 2'),
-                                          Material(name='material 3')],
-                              dict_value={'a': 1, 'b': 2},
-                              none_value=None,
-                              obj_value=Material(name='material'),
-                              numpy_value=np.array([
-                                  [[1, 2, 3], [4, 5, 6], [7, 8, 9]],
-                                  [[10, 11, 12], [13, 14, 15], [16, 17, 18]],
-                                  [[19, 20, 21], [22, 23, 24], [25, 26, 27]],
-                                  [[28, 29, 30], [31, 32, 33], [34, 35, 36]]
-                              ]),
-                              pandas_value=pd.DataFrame({'a': [1, 2, 3], 'b': [4, 5, 6]}),
-                              file_value=None)
+    Assembly = mapped_classes['Assembly']
+    ReferenceFace = mapped_classes['ReferenceFace']
+    Volume = mapped_classes['Volume']
+    Mesh = mapped_classes['Mesh']
 
     t_out_1 = TemperatureBoundaryCondition(name='t_out_1',
-                                           temperature=273.15)
+                                           temperature=273.15,
+                                           data_model=data_model)
 
     t_out_2 = TemperatureBoundaryCondition(name='t_out_2',
-                                           temperature=283.15)
+                                           temperature=283.15,
+                                           data_model=data_model)
 
     concrete = Material(name='concrete',
                         thermal_conductivity=1.5,
                         density=2000,
-                        specific_heat=800)
+                        specific_heat=800,
+                        data_model=data_model)
 
     insulation = Material(name='insulation',
                           thermal_conductivity=0.03,
                           density=150,
-                          specific_heat=1500)
+                          specific_heat=1500,
+                          data_model=data_model)
 
     plaster = Material(name='plaster',
                        thermal_conductivity=0.6,
                        density=1200,
-                       specific_heat=700)
+                       specific_heat=700,
+                       data_model=data_model)
 
     construction_1 = Construction(name='construction_1',
                                   layers=[WallLayer(name='concrete_layer', thickness=0.2, material=concrete),
                                           WallLayer(name='insulation_layer', thickness=0.1, material=insulation),
-                                          WallLayer(name='plaster_layer', thickness=0.01, material=plaster)])
+                                          WallLayer(name='plaster_layer', thickness=0.01, material=plaster)],
+                                  data_model=data_model)
 
     construction_2 = Construction(name='construction_2',
                                   layers=[WallLayer(name='concrete_layer', thickness=0.15, material=concrete),
                                           WallLayer(name='insulation_layer', thickness=0.2, material=insulation)
-                                          ]
+                                          ],
+                                  data_model=data_model
                                   )
 
     wall1 = Wall(name='Wall1',
                  r_si=0.13,
                  r_se=0.04,
                  construction=construction_1,
-                 boundary_condition=t_out_1)
+                 boundary_condition=t_out_1,
+                 data_model=data_model)
     wall1.associate(cube.faces[0])
 
     wall2 = Wall(name='Wall2',
                  r_si=0.13,
                  r_se=0.04,
                  construction=construction_2,
-                 boundary_condition=t_out_2)
+                 boundary_condition=t_out_2,
+                 data_model=data_model)
     wall2.associate(cube.faces[1])
 
     wall3 = Wall(name='Wall3',
                  r_si=0.13,
                  r_se=0.04,
                  construction=construction_1,
-                 boundary_condition=t_out_1)
+                 boundary_condition=t_out_1,
+                 data_model=data_model)
     wall3.associate(cube.faces[2])
 
     wall4 = Wall(name='Wall4',
                  r_si=0.13,
                  r_se=0.04,
                  construction=construction_2,
-                 boundary_condition=t_out_2)
+                 boundary_condition=t_out_2,
+                 data_model=data_model)
     wall4.associate(cube.faces[3])
 
     wall5 = Wall(name='Wall5',
                  r_si=0.13,
                  r_se=0.04,
                  construction=construction_2,
-                 boundary_condition=t_out_1)
+                 boundary_condition=t_out_1,
+                 data_model=data_model)
     wall5.associate(cube.faces[4])
 
     wall6 = Wall(name='Wall6',
                  r_si=0.13,
                  r_se=0.04,
                  construction=construction_2,
-                 boundary_condition=t_out_2)
+                 boundary_condition=t_out_2,
+                 data_model=data_model)
     wall6.associate(cube.faces[5])
 
     convective_heat_source = Source(name='convective_heat_source',
-                                    heat_flux=1000)
+                                    heat_flux=1000,
+                                    data_model=data_model)
 
     zone1 = Zone(name='zone_1',
                  walls=[wall1, wall2, wall3, wall4, wall5, wall6],
-                 sources=[convective_heat_source])
+                 sources=[convective_heat_source],
+                 data_model=data_model)
     zone1.associate(cube)
 
     print(cube.components)
     print(list(zone1.associated_geometry))
 
     steady_state_temperature = zone1.calculate_steady_state_temperature()
     print(steady_state_temperature)
 
+
+def init_project(data_model: DataModel = None) -> dict[str, type]:
+
+    classes = create_classes()
+    mapped_classes = create_mapped_classes(classes)
+
+    TypeTestClass = mapped_classes['TypeTestClass']
+    Material = mapped_classes['Material']
+    WallLayer = mapped_classes['Layer']
+    Construction = mapped_classes['Construction']
+    Wall = mapped_classes['Wall']
+    Zone = mapped_classes['Zone']
+    TemperatureBoundaryCondition = mapped_classes['TemperatureBoundaryCondition']
+    HeatFluxBoundaryCondition = mapped_classes['HeatFluxBoundaryCondition']
+    Source = mapped_classes['Source']
+    Assembly = mapped_classes['Assembly']
+    ReferenceFace = mapped_classes['ReferenceFace']
+    Volume = mapped_classes['Volume']
+    Mesh = mapped_classes['Mesh']
+
+    type_test = TypeTestClass(name='type_test',
+                              int_value=1,
+                              float_value=1.0,
+                              str_value='test',
+                              bool_value=True,
+                              list_value=[Material(name='material 1'),
+                                          Material(name='material 2'),
+                                          Material(name='material 3')],
+                              dict_value={'a': 1, 'b': 2},
+                              none_value=None,
+                              obj_value=Material(name='material'),
+                              numpy_value=np.array([
+                                  [[1, 2, 3], [4, 5, 6], [7, 8, 9]],
+                                  [[10, 11, 12], [13, 14, 15], [16, 17, 18]],
+                                  [[19, 20, 21], [22, 23, 24], [25, 26, 27]],
+                                  [[28, 29, 30], [31, 32, 33], [34, 35, 36]]
+                              ]),
+                              pandas_value=pd.DataFrame({'a': [1, 2, 3], 'b': [4, 5, 6]}),
+                              file_value=None)
+
+    create_new_steady_state_zone(mapped_classes,
+                                 data_model=data_model)
+
     data_model.save()
     data_model.cleanup()
     mapper.clear()
 
+    return mapped_classes
+
 
-def map_methods():
+def map_methods(mapped_classes):
     cls = mapper.get_mapped_class('Zone')
     method_mapper.register_method(cls=cls,
                                   name='calculate_steady_state_temperature',
                                   method=cls.calculate_steady_state_temperature,
                                   args=[],
                                   kwargs={})
 
     method_mapper.register_method(cls=cls,
                                   name='calculate_area',
                                   method=cls.calculate_area,
                                   args=[],
                                   kwargs={})
 
+    method_mapper.register_method(name='Create new steady state zone',
+                                  method=create_new_steady_state_zone,
+                                  args=[mapped_classes],
+                                  add_data_model_to_kwargs=True)
+
+    method_mapper.register_method(name='Say hello',
+                                  method=lambda: print('Hello!'),
+                                  args=[],
+                                  kwargs={})
+
 
 mapper.clear()
 
-init_project()
-map_methods()
+mapped_classes = init_project(data_model=new_data_model)
+map_methods(mapped_classes)
 run_ui()
 
 print('Test passed 48 47 2')
```

