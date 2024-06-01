# Comparing `tmp/metabase-api-0.3.3.1.tar.gz` & `tmp/metabase-api-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabase-api-0.3.3.1.tar", last modified: Fri May 24 17:40:47 2024, max compression
+gzip compressed data, was "metabase-api-3.4.tar", last modified: Sat Jun  1 22:49:42 2024, max compression
```

## Comparing `metabase-api-0.3.3.1.tar` & `metabase-api-3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 17:40:47.082677 metabase-api-0.3.3.1/
--rw-rw-rw-   0        0        0     1080 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/LICENSE
--rw-rw-rw-   0        0        0    13254 2024-05-24 17:40:47.082677 metabase-api-0.3.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    12638 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 17:40:47.067045 metabase-api-0.3.3.1/metabase_api/
--rw-rw-rw-   0        0        0       39 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/metabase_api/__init__.py
--rw-rw-rw-   0        0        0    12728 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/metabase_api/_helper_methods.py
--rw-rw-rw-   0        0        0     1108 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/metabase_api/_rest_methods.py
--rw-rw-rw-   0        0        0    17174 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/metabase_api/copy_methods.py
--rw-rw-rw-   0        0        0    11866 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/metabase_api/create_methods.py
--rw-rw-rw-   0        0        0    15352 2024-05-24 17:37:54.000000 metabase-api-0.3.3.1/metabase_api/metabase_api.py
-drwxrwxrwx   0        0        0        0 2024-05-24 17:40:47.082677 metabase-api-0.3.3.1/metabase_api.egg-info/
--rw-rw-rw-   0        0        0    13254 2024-05-24 17:40:46.000000 metabase-api-0.3.3.1/metabase_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-05-24 17:40:46.000000 metabase-api-0.3.3.1/metabase_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 17:40:46.000000 metabase-api-0.3.3.1/metabase_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-24 17:40:46.000000 metabase-api-0.3.3.1/metabase_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-24 17:40:46.000000 metabase-api-0.3.3.1/metabase_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 17:40:47.082677 metabase-api-0.3.3.1/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-05-24 17:32:18.000000 metabase-api-0.3.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 17:40:47.082677 metabase-api-0.3.3.1/tests/
--rw-rw-rw-   0        0        0        1 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/tests/__init__.py
--rw-rw-rw-   0        0        0    11231 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/tests/test_metabase_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:49:42.379836 metabase-api-3.4/
+-rw-rw-rw-   0        0        0     1080 2024-06-01 21:27:38.000000 metabase-api-3.4/LICENSE
+-rw-rw-rw-   0        0        0    13078 2024-06-01 22:49:42.378834 metabase-api-3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12469 2024-06-01 21:46:34.000000 metabase-api-3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 22:49:42.362964 metabase-api-3.4/metabase_api/
+-rw-rw-rw-   0        0        0       39 2024-06-01 21:27:38.000000 metabase-api-3.4/metabase_api/__init__.py
+-rw-rw-rw-   0        0        0    12728 2024-06-01 21:27:38.000000 metabase-api-3.4/metabase_api/_helper_methods.py
+-rw-rw-rw-   0        0        0     1108 2024-06-01 21:27:38.000000 metabase-api-3.4/metabase_api/_rest_methods.py
+-rw-rw-rw-   0        0        0    17174 2024-06-01 21:27:38.000000 metabase-api-3.4/metabase_api/copy_methods.py
+-rw-rw-rw-   0        0        0    11866 2024-06-01 21:27:38.000000 metabase-api-3.4/metabase_api/create_methods.py
+-rw-rw-rw-   0        0        0    15514 2024-06-01 21:43:46.000000 metabase-api-3.4/metabase_api/metabase_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:49:42.372959 metabase-api-3.4/metabase_api.egg-info/
+-rw-rw-rw-   0        0        0    13078 2024-06-01 22:49:41.000000 metabase-api-3.4/metabase_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-06-01 22:49:42.000000 metabase-api-3.4/metabase_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 22:49:41.000000 metabase-api-3.4/metabase_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 22:49:41.000000 metabase-api-3.4/metabase_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-06-01 22:49:41.000000 metabase-api-3.4/metabase_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 22:49:42.379836 metabase-api-3.4/setup.cfg
+-rw-rw-rw-   0        0        0      685 2024-06-01 21:28:16.000000 metabase-api-3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:49:42.376818 metabase-api-3.4/tests/
+-rw-rw-rw-   0        0        0        1 2024-06-01 21:27:38.000000 metabase-api-3.4/tests/__init__.py
+-rw-rw-rw-   0        0        0    11672 2024-06-01 22:27:38.000000 metabase-api-3.4/tests/test_metabase_api.py
```

### Comparing `metabase-api-0.3.3.1/LICENSE` & `metabase-api-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.3.1/PKG-INFO` & `metabase-api-3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api
-Version: 0.3.3.1
+Version: 3.4
 Summary: A Python Wrapper for Metabase API
 Home-page: https://github.com/vvaezian/metabase_api_python
 Author: Vahid Vaezian
 Author-email: vahid.vaezian@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -178,10 +178,7 @@
 mb.move_to_archive('card', item_id=123)
 ```
 - #### `delete_item`
 Deletes the item (Card, Dashboard, Pulse). Currently Collections and Segments cannot be deleted using the Metabase API.
 ```python
 mb.delete_item('card', item_id=123)
 ```
-
-## Notes
-There are also two other Python wrappers for Metabase API [here](https://github.com/mertsalik/metabasepy) and [here](https://github.com/STUnitas/metabase-py).
```

### Comparing `metabase-api-0.3.3.1/README.md` & `metabase-api-3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -165,10 +165,7 @@
 mb.move_to_archive('card', item_id=123)
 ```
 - #### `delete_item`
 Deletes the item (Card, Dashboard, Pulse). Currently Collections and Segments cannot be deleted using the Metabase API.
 ```python
 mb.delete_item('card', item_id=123)
 ```
-
-## Notes
-There are also two other Python wrappers for Metabase API [here](https://github.com/mertsalik/metabasepy) and [here](https://github.com/STUnitas/metabase-py).
```

### Comparing `metabase-api-0.3.3.1/metabase_api/_helper_methods.py` & `metabase-api-3.4/metabase_api/_helper_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.3.1/metabase_api/_rest_methods.py` & `metabase-api-3.4/metabase_api/_rest_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.3.1/metabase_api/copy_methods.py` & `metabase-api-3.4/metabase_api/copy_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.3.1/metabase_api/create_methods.py` & `metabase-api-3.4/metabase_api/create_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.3.1/metabase_api/metabase_api.py` & `metabase-api-3.4/metabase_api/metabase_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,40 +86,45 @@
         if item_type is not None:
             res = [ item for item in res if item['model'] == item_type ]
 
         return res
 
 
 
-    def get_card_data(self, card_name=None, card_id=None, collection_name=None, 
-                      collection_id=None, data_format='json', parameters=None):
+    def get_card_data(self, card_name=None, card_id=None, collection_name=None, collection_id=None, 
+                      data_format='json', parameters=None, format_rows=False):
         '''
         Run the query associated with a card and get the results.
-        The data_format keyword specifies the format of the returned data:
+
+        Keyword arguments:
+        data_format -- specifies the format of the returned data:
             - 'json': every row is a dictionary of <column-header, cell> key-value pairs    
             - 'csv': the entire result is returned as a string, where rows are separated by newlines and cells with commas.
-        To pass the filter values use 'parameters' param:
+        parameters -- can be used to pass filter values:
             The format is like [{"type":"category","value":["val1","val2"],"target":["dimension",["template-tag","filter_variable_name"]]}]
             See the network tab when exporting the results using the web interface to get the proper format pattern.
+        format_rows -- whether the returned results should be formatted or not
         '''
         assert data_format in [ 'json', 'csv' ]
         if parameters:
             assert type(parameters) == list
 
         if card_id is None:
             if card_name is None:
                 raise ValueError('Either card_id or card_name must be provided.')
             card_id = self.get_item_id(item_name=card_name,
                                        collection_name=collection_name,
                                        collection_id=collection_id,
                                        item_type='card')
 
-        # add the filter values (if any)
         import json
-        params_json = {'parameters':json.dumps(parameters)}
+        params_json = { 
+            'parameters':json.dumps(parameters), 
+            'format_rows':'true' if format_rows else 'false' 
+        }
 
         # get the results
         res = self.post("/api/card/{}/query/{}".format(card_id, data_format), 'raw', data=params_json)
 
         # return the results in the requested format
         if data_format == 'json':
             return json.loads(res.text)
```

### Comparing `metabase-api-0.3.3.1/metabase_api.egg-info/PKG-INFO` & `metabase-api-3.4/metabase_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api
-Version: 0.3.3.1
+Version: 3.4
 Summary: A Python Wrapper for Metabase API
 Home-page: https://github.com/vvaezian/metabase_api_python
 Author: Vahid Vaezian
 Author-email: vahid.vaezian@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -178,10 +178,7 @@
 mb.move_to_archive('card', item_id=123)
 ```
 - #### `delete_item`
 Deletes the item (Card, Dashboard, Pulse). Currently Collections and Segments cannot be deleted using the Metabase API.
 ```python
 mb.delete_item('card', item_id=123)
 ```
-
-## Notes
-There are also two other Python wrappers for Metabase API [here](https://github.com/mertsalik/metabasepy) and [here](https://github.com/STUnitas/metabase-py).
```

### Comparing `metabase-api-0.3.3.1/setup.py` & `metabase-api-3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="metabase-api",
-    version="0.3.3.1",
+    version="3.4",
     author="Vahid Vaezian",
     author_email="vahid.vaezian@gmail.com",
     description="A Python Wrapper for Metabase API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vvaezian/metabase_api_python",
     packages=setuptools.find_packages(),
```

### Comparing `metabase-api-0.3.3.1/tests/test_metabase_api.py` & `metabase-api-3.4/tests/test_metabase_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,14 +248,25 @@
 
 
 
   def test_get_card_data(self):
     # json
     res = mb.get_card_data(card_id=1)
     json_data = [
+      {'col1': 'row1 cell1', 'col2': 1},
+      {'col1': None, 'col2': 2},
+      {'col1': 'row3 cell1', 'col2': None},
+      {'col1': None, 'col2': None},
+      {'col1': 'row5 cell1', 'col2': 5}
+    ]
+    self.assertEqual(res, json_data)
+
+    # formatted rows (in json export mode, Null values in varchar columns become '' and numbers become strings, e.g. 123 -> '123')
+    res = mb.get_card_data(card_id=1, format_rows=True)
+    json_data = [
       {'col1': 'row1 cell1', 'col2': '1'},
       {'col1': '', 'col2': '2'},
       {'col1': 'row3 cell1', 'col2': None},
       {'col1': '', 'col2': None},
       {'col1': 'row5 cell1', 'col2': '5'}
     ]
     self.assertEqual(res, json_data)
@@ -263,15 +274,15 @@
     # csv
     res = mb.get_card_data(card_id=1, data_format='csv')
     csv_data = 'col1,col2\nrow1 cell1,1\n,2\nrow3 cell1,\n,\nrow5 cell1,5\n'
     self.assertEqual(res, csv_data)
 
     # filtered data
     res = mb.get_card_data(card_id=2, parameters=[{"type":"string/=","value":['row1 cell1', 'row3 cell1'],"target":["dimension",["template-tag","test_filter"]]}])
-    filtered_data = [{'col1': 'row1 cell1', 'col2': '1'}, {'col1': 'row3 cell1', 'col2': None}]
+    filtered_data = [{'col1': 'row1 cell1', 'col2': 1}, {'col1': 'row3 cell1', 'col2': None}]
     self.assertEqual(res, filtered_data)
 
 
 
   def test_clone_card(self):
     # native question
     res = mb.clone_card(2, 9, 10, new_card_name='test_clone_native', new_card_collection_id=1, return_card=True)
```

