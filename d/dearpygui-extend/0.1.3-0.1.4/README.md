# Comparing `tmp/dearpygui_extend-0.1.3.tar.gz` & `tmp/dearpygui_extend-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearpygui_extend-0.1.3.tar", last modified: Thu Jan 11 20:33:30 2024, max compression
+gzip compressed data, was "dearpygui_extend-0.1.4.tar", last modified: Sun Jun  2 18:17:17 2024, max compression
```

## Comparing `dearpygui_extend-0.1.3.tar` & `dearpygui_extend-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 fabriciochamon  (1000) fabriciochamon  (1000)        0 2024-01-11 20:33:30.023773 dearpygui_extend-0.1.3/
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     1072 2023-08-05 19:09:05.000000 dearpygui_extend-0.1.3/LICENSE
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     2879 2024-01-11 20:33:30.023773 dearpygui_extend-0.1.3/PKG-INFO
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     2416 2023-08-16 17:57:49.000000 dearpygui_extend-0.1.3/README.md
-drwxr-xr-x   0 fabriciochamon  (1000) fabriciochamon  (1000)        0 2024-01-11 20:33:30.022773 dearpygui_extend-0.1.3/dearpygui_extend/
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     7192 2024-01-11 20:31:01.000000 dearpygui_extend-0.1.3/dearpygui_extend/__init__.py
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)    79095 2023-12-21 21:33:18.000000 dearpygui_extend-0.1.3/dearpygui_extend/file_browser.py
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)    10660 2023-08-21 16:24:43.000000 dearpygui_extend-0.1.3/dearpygui_extend/layout.py
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     4848 2023-08-07 16:52:23.000000 dearpygui_extend-0.1.3/dearpygui_extend/movable_group.py
-drwxr-xr-x   0 fabriciochamon  (1000) fabriciochamon  (1000)        0 2024-01-11 20:33:30.022773 dearpygui_extend-0.1.3/dearpygui_extend.egg-info/
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     2879 2024-01-11 20:33:30.000000 dearpygui_extend-0.1.3/dearpygui_extend.egg-info/PKG-INFO
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)      391 2024-01-11 20:33:30.000000 dearpygui_extend-0.1.3/dearpygui_extend.egg-info/SOURCES.txt
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)        1 2024-01-11 20:33:30.000000 dearpygui_extend-0.1.3/dearpygui_extend.egg-info/dependency_links.txt
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)       20 2024-01-11 20:33:30.000000 dearpygui_extend-0.1.3/dearpygui_extend.egg-info/entry_points.txt
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)       48 2024-01-11 20:33:30.000000 dearpygui_extend-0.1.3/dearpygui_extend.egg-info/requires.txt
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)       17 2024-01-11 20:33:30.000000 dearpygui_extend-0.1.3/dearpygui_extend.egg-info/top_level.txt
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)       38 2024-01-11 20:33:30.023773 dearpygui_extend-0.1.3/setup.cfg
--rw-r--r--   0 fabriciochamon  (1000) fabriciochamon  (1000)      972 2024-01-11 20:32:17.000000 dearpygui_extend-0.1.3/setup.py
+drwxrwxr-x   0 fabriciochamon  (1000) fabriciochamon  (1000)        0 2024-06-02 18:17:17.676094 dearpygui_extend-0.1.4/
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     1072 2024-06-02 17:35:44.000000 dearpygui_extend-0.1.4/LICENSE
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     2879 2024-06-02 18:17:17.676094 dearpygui_extend-0.1.4/PKG-INFO
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     2416 2024-06-02 17:35:44.000000 dearpygui_extend-0.1.4/README.md
+drwxrwxr-x   0 fabriciochamon  (1000) fabriciochamon  (1000)        0 2024-06-02 18:17:17.676094 dearpygui_extend-0.1.4/dearpygui_extend/
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     7192 2024-06-02 17:35:44.000000 dearpygui_extend-0.1.4/dearpygui_extend/__init__.py
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)    79095 2024-06-02 17:35:44.000000 dearpygui_extend-0.1.4/dearpygui_extend/file_browser.py
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)    10653 2024-06-02 17:35:44.000000 dearpygui_extend-0.1.4/dearpygui_extend/layout.py
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     4848 2024-06-02 17:35:44.000000 dearpygui_extend-0.1.4/dearpygui_extend/movable_group.py
+drwxrwxr-x   0 fabriciochamon  (1000) fabriciochamon  (1000)        0 2024-06-02 18:17:17.676094 dearpygui_extend-0.1.4/dearpygui_extend.egg-info/
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)     2879 2024-06-02 18:17:17.000000 dearpygui_extend-0.1.4/dearpygui_extend.egg-info/PKG-INFO
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)      391 2024-06-02 18:17:17.000000 dearpygui_extend-0.1.4/dearpygui_extend.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)        1 2024-06-02 18:17:17.000000 dearpygui_extend-0.1.4/dearpygui_extend.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)       20 2024-06-02 18:17:17.000000 dearpygui_extend-0.1.4/dearpygui_extend.egg-info/entry_points.txt
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)       48 2024-06-02 18:17:17.000000 dearpygui_extend-0.1.4/dearpygui_extend.egg-info/requires.txt
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)       17 2024-06-02 18:17:17.000000 dearpygui_extend-0.1.4/dearpygui_extend.egg-info/top_level.txt
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)       38 2024-06-02 18:17:17.676094 dearpygui_extend-0.1.4/setup.cfg
+-rw-rw-r--   0 fabriciochamon  (1000) fabriciochamon  (1000)      972 2024-06-02 18:14:04.000000 dearpygui_extend-0.1.4/setup.py
```

### Comparing `dearpygui_extend-0.1.3/LICENSE` & `dearpygui_extend-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dearpygui_extend-0.1.3/PKG-INFO` & `dearpygui_extend-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearpygui_extend
-Version: 0.1.3
+Version: 0.1.4
 Summary: Extensions and custom widgets for Dear Py GUI
 Home-page: https://github.com/fabriciochamon/DearPyGui_Extend
 Author: Fabricio Chamon
 Author-email: fabricio.chamon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dearpygui_extend-0.1.3/README.md` & `dearpygui_extend-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dearpygui_extend-0.1.3/dearpygui_extend/__init__.py` & `dearpygui_extend-0.1.4/dearpygui_extend/__init__.py`

 * *Files identical despite different names*

### Comparing `dearpygui_extend-0.1.3/dearpygui_extend/file_browser.py` & `dearpygui_extend-0.1.4/dearpygui_extend/file_browser.py`

 * *Files identical despite different names*

### Comparing `dearpygui_extend-0.1.3/dearpygui_extend/layout.py` & `dearpygui_extend-0.1.4/dearpygui_extend/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
 					}
 					entry['size']=None if entry['level']==0 else entry['size']
 					layout_list.append(entry)
 					last_level = level
 			
 			return layout_list
 
+
 		# recursively builds the table elements
 		def build_table(item, layout, parent_item=None, debug=False):
 
 			def get_layout_item(id, layout):
 				return [x for x in layout if x['id']==id][0]
 
 			def get_subelements(id, layout, etype='col'):
@@ -274,27 +275,25 @@
 					dpg.add_table_row(parent=tag_table, tag=tag_row)
 
 					for col in cols:
 						tag_cw = f'__layout_cw_{row["id"]}_{col["id"]}'
 						col_has_children = len(get_subelements(col['id'], layout, 'col'))>0 or len(get_subelements(col['id'], layout, 'row'))>0
 						user_data_cw = '' if row['size']==1 else {'type': '__layout_item', 'height': row_size}
 						dpg.add_child_window(tag=tag_cw, parent=tag_row, user_data=user_data_cw)
-						
 						if not col_has_children and col['tag'] is not None:
 							level0 = [x for x in layout if x['level']==0][0]
 							halign = col['halign']
 							valign = col['valign']
 							if halign is None:
 								halign = level0['halign'] if level0['halign'] is not None else 'left'
 							if valign is None:
 								valign = level0['valign'] if level0['valign'] is not None else 'top'
 
 							grp = dpg.add_group(tag=col['tag'], parent=tag_cw, user_data={'type': '__layout_content', 'halign': halign, 'valign': valign})
 							if debug: dpg.add_text(col['tag'], parent=grp)
-
 						build_table(col, layout, tag_cw, debug)
 
 					if has_rows: build_table(row, layout, tag_cw, debug)
 
 			self.root = tag_table
 			
 		parsedlayout = parse_layout(layout=self.layout)
```

### Comparing `dearpygui_extend-0.1.3/dearpygui_extend/movable_group.py` & `dearpygui_extend-0.1.4/dearpygui_extend/movable_group.py`

 * *Files identical despite different names*

### Comparing `dearpygui_extend-0.1.3/dearpygui_extend.egg-info/PKG-INFO` & `dearpygui_extend-0.1.4/dearpygui_extend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearpygui-extend
-Version: 0.1.3
+Version: 0.1.4
 Summary: Extensions and custom widgets for Dear Py GUI
 Home-page: https://github.com/fabriciochamon/DearPyGui_Extend
 Author: Fabricio Chamon
 Author-email: fabricio.chamon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dearpygui_extend-0.1.3/setup.py` & `dearpygui_extend-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dearpygui_extend",
-    version="0.1.3",
+    version="0.1.4",
     packages=['dearpygui_extend'],
     install_requires=[
-        'dearpygui==1.9.1',
-        'Fileseq==1.15.2',
+        'dearpygui>=1.9.1',
+        'Fileseq>=1.15.2',
         'future==0.18.3',
     ],
     entry_points={
         "console_scripts": [
             # If your project has command-line scripts, add their entry points here, e.g.
             # "my_script=my_package.my_module:main",
         ],
```

