# Comparing `tmp/database_mysql_local-0.0.350.tar.gz` & `tmp/database_mysql_local-0.0.351.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.350.tar", last modified: Thu May 30 21:19:40 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.351.tar", last modified: Sun Jun  2 05:03:11 2024, max compression
```

## Comparing `database_mysql_local-0.0.350.tar` & `database_mysql_local-0.0.351.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:40.420416 database_mysql_local-0.0.350/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-30 21:19:40.420416 database_mysql_local-0.0.350/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:40.412417 database_mysql_local-0.0.350/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:40.420416 database_mysql_local-0.0.350/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    58695 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   253151 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   668288 2024-05-30 21:19:07.000000 database_mysql_local-0.0.350/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:40.420416 database_mysql_local-0.0.350/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-30 21:19:40.000000 database_mysql_local-0.0.350/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 21:19:40.000000 database_mysql_local-0.0.350/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:19:40.000000 database_mysql_local-0.0.350/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-30 21:19:40.000000 database_mysql_local-0.0.350/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 21:19:40.000000 database_mysql_local-0.0.350/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 21:18:49.000000 database_mysql_local-0.0.350/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:19:40.420416 database_mysql_local-0.0.350/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-30 21:18:41.000000 database_mysql_local-0.0.350/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:03:11.129712 database_mysql_local-0.0.351/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-06-02 05:03:11.129712 database_mysql_local-0.0.351/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:03:11.125712 database_mysql_local-0.0.351/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:03:11.129712 database_mysql_local-0.0.351/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58695 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   253151 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   671987 2024-06-02 05:02:34.000000 database_mysql_local-0.0.351/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:03:11.129712 database_mysql_local-0.0.351/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-06-02 05:03:11.000000 database_mysql_local-0.0.351/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-06-02 05:03:11.000000 database_mysql_local-0.0.351/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 05:03:11.000000 database_mysql_local-0.0.351/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-06-02 05:03:11.000000 database_mysql_local-0.0.351/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 05:03:11.000000 database_mysql_local-0.0.351/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-06-02 05:02:15.000000 database_mysql_local-0.0.351/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 05:03:11.129712 database_mysql_local-0.0.351/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-06-02 05:02:05.000000 database_mysql_local-0.0.351/setup.py
```

### Comparing `database_mysql_local-0.0.350/PKG-INFO` & `database_mysql_local-0.0.351/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.350
+Version: 0.0.351
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.350/README.md` & `database_mysql_local-0.0.351/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.351/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.351/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.351/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.351/database_mysql_local/src/generate_table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.351/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.351/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.351/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/point.py` & `database_mysql_local-0.0.351/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.351/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.351/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.351/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.351/database_mysql_local/src/table_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 table_definition = {
     'phone_table': {
         'table_definition_id': 1,
         'entity_type_id1': 26,
         'entity_type_id2': None,
         'schema': 'phone',
-        'view_name': None,
+        'view_name': 'phone_view',
         'seq': 0,
         'table_list_id': None,
         'is_created_updated_fields': 1,
         'is_logical_delete_fields': 1,
         'contact_mapping_table_id': None,
         'profile_mapping_table_id': 2,
         'is_ml_parent_table': 1,
@@ -26,16 +26,52 @@
         'is_history': None,
         'is_one_table_per_all_tenants': 0,
         'is_tree': None,
         'is_graph': None,
         'is_metrics': None,
         'is_visibility': None,
         'is_pii': None,
-        'is_sensative': None,
-        'sensative_columns': None,
+        'is_sensative': 1,
+        'sensative_columns': 'number_original,local_number_normalized,full_',
+        'description': None,
+        'end_timestamp': None,
+        'insert_is_undelete': None,
+        'is_dynamic': None,
+    },
+    'phone_view': {
+        'table_definition_id': 1,
+        'entity_type_id1': 26,
+        'entity_type_id2': None,
+        'schema': 'phone',
+        'view_name': 'phone_view',
+        'seq': 0,
+        'table_list_id': None,
+        'is_created_updated_fields': 1,
+        'is_logical_delete_fields': 1,
+        'contact_mapping_table_id': None,
+        'profile_mapping_table_id': 2,
+        'is_ml_parent_table': 1,
+        'is_ml_child_table': None,
+        'table_type': None,
+        'is_number_column': 1,
+        'is_test_data_column': None,
+        'is_main_column': None,
+        'is_single_and_multi_value': None,
+        'name_of_single_value_column': None,
+        'is_mapping_table': None,
+        'is_entity': None,
+        'is_history': None,
+        'is_one_table_per_all_tenants': 0,
+        'is_tree': None,
+        'is_graph': None,
+        'is_metrics': None,
+        'is_visibility': None,
+        'is_pii': None,
+        'is_sensative': 1,
+        'sensative_columns': 'number_original,local_number_normalized,full_',
         'description': None,
         'end_timestamp': None,
         'insert_is_undelete': None,
         'is_dynamic': None,
     },
     'phone_profile_table': {
         'table_definition_id': 2,
@@ -170,16 +206,16 @@
         'is_history': None,
         'is_one_table_per_all_tenants': 0,
         'is_tree': None,
         'is_graph': None,
         'is_metrics': None,
         'is_visibility': None,
         'is_pii': None,
-        'is_sensative': None,
-        'sensative_columns': None,
+        'is_sensative': 1,
+        'sensative_columns': 'email_address',
         'description': None,
         'end_timestamp': None,
         'insert_is_undelete': None,
         'is_dynamic': None,
     },
     'email_address_view': {
         'table_definition_id': 4,
@@ -206,16 +242,16 @@
         'is_history': None,
         'is_one_table_per_all_tenants': 0,
         'is_tree': None,
         'is_graph': None,
         'is_metrics': None,
         'is_visibility': None,
         'is_pii': None,
-        'is_sensative': None,
-        'sensative_columns': None,
+        'is_sensative': 1,
+        'sensative_columns': 'email_address',
         'description': None,
         'end_timestamp': None,
         'insert_is_undelete': None,
         'is_dynamic': None,
     },
     'user_table': {
         'table_definition_id': 5,
@@ -542,15 +578,15 @@
         'is_dynamic': None,
     },
     'user_external_table': {
         'table_definition_id': 12,
         'entity_type_id1': None,
         'entity_type_id2': None,
         'schema': 'user_external',
-        'view_name': None,
+        'view_name': 'user_external_view',
         'seq': 0,
         'table_list_id': None,
         'is_created_updated_fields': 1,
         'is_logical_delete_fields': 1,
         'contact_mapping_table_id': None,
         'profile_mapping_table_id': None,
         'is_ml_parent_table': None,
@@ -566,16 +602,52 @@
         'is_history': None,
         'is_one_table_per_all_tenants': 0,
         'is_tree': None,
         'is_graph': None,
         'is_metrics': None,
         'is_visibility': None,
         'is_pii': None,
-        'is_sensative': None,
-        'sensative_columns': None,
+        'is_sensative': 1,
+        'sensative_columns': 'access_token, refresh_token',
+        'description': None,
+        'end_timestamp': None,
+        'insert_is_undelete': None,
+        'is_dynamic': None,
+    },
+    'user_external_view': {
+        'table_definition_id': 12,
+        'entity_type_id1': None,
+        'entity_type_id2': None,
+        'schema': 'user_external',
+        'view_name': 'user_external_view',
+        'seq': 0,
+        'table_list_id': None,
+        'is_created_updated_fields': 1,
+        'is_logical_delete_fields': 1,
+        'contact_mapping_table_id': None,
+        'profile_mapping_table_id': None,
+        'is_ml_parent_table': None,
+        'is_ml_child_table': None,
+        'table_type': None,
+        'is_number_column': 1,
+        'is_test_data_column': None,
+        'is_main_column': None,
+        'is_single_and_multi_value': None,
+        'name_of_single_value_column': None,
+        'is_mapping_table': 0,
+        'is_entity': None,
+        'is_history': None,
+        'is_one_table_per_all_tenants': 0,
+        'is_tree': None,
+        'is_graph': None,
+        'is_metrics': None,
+        'is_visibility': None,
+        'is_pii': None,
+        'is_sensative': 1,
+        'sensative_columns': 'access_token, refresh_token',
         'description': None,
         'end_timestamp': None,
         'insert_is_undelete': None,
         'is_dynamic': None,
     },
     'location_table': {
         'table_definition_id': 13,
@@ -1298,15 +1370,15 @@
         'is_dynamic': None,
     },
     'user_pii_table': {
         'table_definition_id': 28,
         'entity_type_id1': None,
         'entity_type_id2': None,
         'schema': 'user_pii',
-        'view_name': None,
+        'view_name': 'user_pii_view',
         'seq': 0,
         'table_list_id': None,
         'is_created_updated_fields': 1,
         'is_logical_delete_fields': 1,
         'contact_mapping_table_id': None,
         'profile_mapping_table_id': None,
         'is_ml_parent_table': None,
@@ -1322,16 +1394,52 @@
         'is_history': None,
         'is_one_table_per_all_tenants': 0,
         'is_tree': None,
         'is_graph': None,
         'is_metrics': None,
         'is_visibility': None,
         'is_pii': None,
-        'is_sensative': None,
-        'sensative_columns': None,
+        'is_sensative': 1,
+        'sensative_columns': 'password_clear_text, password_encrypted',
+        'description': None,
+        'end_timestamp': None,
+        'insert_is_undelete': None,
+        'is_dynamic': None,
+    },
+    'user_pii_view': {
+        'table_definition_id': 28,
+        'entity_type_id1': None,
+        'entity_type_id2': None,
+        'schema': 'user_pii',
+        'view_name': 'user_pii_view',
+        'seq': 0,
+        'table_list_id': None,
+        'is_created_updated_fields': 1,
+        'is_logical_delete_fields': 1,
+        'contact_mapping_table_id': None,
+        'profile_mapping_table_id': None,
+        'is_ml_parent_table': None,
+        'is_ml_child_table': None,
+        'table_type': None,
+        'is_number_column': None,
+        'is_test_data_column': None,
+        'is_main_column': None,
+        'is_single_and_multi_value': None,
+        'name_of_single_value_column': None,
+        'is_mapping_table': None,
+        'is_entity': None,
+        'is_history': None,
+        'is_one_table_per_all_tenants': 0,
+        'is_tree': None,
+        'is_graph': None,
+        'is_metrics': None,
+        'is_visibility': None,
+        'is_pii': None,
+        'is_sensative': 1,
+        'sensative_columns': 'password_clear_text, password_encrypted',
         'description': None,
         'end_timestamp': None,
         'insert_is_undelete': None,
         'is_dynamic': None,
     },
     'star_transaction_table': {
         'table_definition_id': 29,
```

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.351/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.351/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.351/database_mysql_local.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.350
+Version: 0.0.351
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.350/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.351/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/pyproject.toml` & `database_mysql_local-0.0.351/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.350/setup.py` & `database_mysql_local-0.0.351/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.350',
+    version='0.0.351',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

