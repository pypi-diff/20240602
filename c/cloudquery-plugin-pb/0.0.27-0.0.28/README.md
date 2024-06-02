# Comparing `tmp/cloudquery_plugin_pb-0.0.27.tar.gz` & `tmp/cloudquery_plugin_pb-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudquery_plugin_pb-0.0.27.tar", last modified: Tue May  7 09:38:13 2024, max compression
+gzip compressed data, was "cloudquery_plugin_pb-0.0.28.tar", last modified: Sun Jun  2 16:24:39 2024, max compression
```

## Comparing `cloudquery_plugin_pb-0.0.27.tar` & `cloudquery_plugin_pb-0.0.28.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:38:13.615018 cloudquery_plugin_pb-0.0.27/
--rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-07 09:38:13.615018 cloudquery_plugin_pb-0.0.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:38:13.611018 cloudquery_plugin_pb-0.0.27/cloudquery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:38:13.611018 cloudquery_plugin_pb-0.0.27/cloudquery/discovery_v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/cloudquery/discovery_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/cloudquery/discovery_v1/discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/cloudquery/discovery_v1/discovery_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/cloudquery/discovery_v1/discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/cloudquery/discovery_v1/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:38:13.611018 cloudquery_plugin_pb-0.0.27/cloudquery/plugin_v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/cloudquery/plugin_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/cloudquery/plugin_v3/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/cloudquery/plugin_v3/plugin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/cloudquery/plugin_v3/plugin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18843 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/cloudquery/plugin_v3/plugin_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/cloudquery/plugin_v3/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:38:13.615018 cloudquery_plugin_pb-0.0.27/cloudquery_plugin_pb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-07 09:38:13.000000 cloudquery_plugin_pb-0.0.27/cloudquery_plugin_pb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-07 09:38:13.000000 cloudquery_plugin_pb-0.0.27/cloudquery_plugin_pb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:38:13.000000 cloudquery_plugin_pb-0.0.27/cloudquery_plugin_pb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 09:38:13.000000 cloudquery_plugin_pb-0.0.27/cloudquery_plugin_pb.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:38:13.000000 cloudquery_plugin_pb-0.0.27/cloudquery_plugin_pb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 09:38:13.000000 cloudquery_plugin_pb-0.0.27/cloudquery_plugin_pb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 09:38:13.000000 cloudquery_plugin_pb-0.0.27/cloudquery_plugin_pb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 09:38:13.615018 cloudquery_plugin_pb-0.0.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-07 09:38:02.000000 cloudquery_plugin_pb-0.0.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:24:39.402156 cloudquery_plugin_pb-0.0.28/
+-rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-06-02 16:24:39.402156 cloudquery_plugin_pb-0.0.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:24:39.398156 cloudquery_plugin_pb-0.0.28/cloudquery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:24:39.402156 cloudquery_plugin_pb-0.0.28/cloudquery/discovery_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/cloudquery/discovery_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/cloudquery/discovery_v1/discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/cloudquery/discovery_v1/discovery_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/cloudquery/discovery_v1/discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/cloudquery/discovery_v1/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:24:39.402156 cloudquery_plugin_pb-0.0.28/cloudquery/plugin_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/cloudquery/plugin_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/cloudquery/plugin_v3/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/cloudquery/plugin_v3/plugin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/cloudquery/plugin_v3/plugin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20878 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/cloudquery/plugin_v3/plugin_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/cloudquery/plugin_v3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:24:39.402156 cloudquery_plugin_pb-0.0.28/cloudquery_plugin_pb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-06-02 16:24:39.000000 cloudquery_plugin_pb-0.0.28/cloudquery_plugin_pb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-06-02 16:24:39.000000 cloudquery_plugin_pb-0.0.28/cloudquery_plugin_pb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:24:39.000000 cloudquery_plugin_pb-0.0.28/cloudquery_plugin_pb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 16:24:39.000000 cloudquery_plugin_pb-0.0.28/cloudquery_plugin_pb.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:24:39.000000 cloudquery_plugin_pb-0.0.28/cloudquery_plugin_pb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-02 16:24:39.000000 cloudquery_plugin_pb-0.0.28/cloudquery_plugin_pb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 16:24:39.000000 cloudquery_plugin_pb-0.0.28/cloudquery_plugin_pb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-02 16:24:39.402156 cloudquery_plugin_pb-0.0.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-06-02 16:24:29.000000 cloudquery_plugin_pb-0.0.28/setup.py
```

### Comparing `cloudquery_plugin_pb-0.0.27/LICENSE` & `cloudquery_plugin_pb-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudquery_plugin_pb-0.0.27/PKG-INFO` & `cloudquery_plugin_pb-0.0.28/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-pb
-Version: 0.0.27
+Version: 0.0.28
 Summary: CloudQuery Plugin client and server library
 Home-page: https://github.com/cloudquery/plugin-pb-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery_plugin_pb-0.0.27/README.md` & `cloudquery_plugin_pb-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `cloudquery_plugin_pb-0.0.27/cloudquery/discovery_v1/discovery_pb2.py` & `cloudquery_plugin_pb-0.0.28/cloudquery/discovery_v1/discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudquery_plugin_pb-0.0.27/cloudquery/discovery_v1/discovery_pb2.pyi` & `cloudquery_plugin_pb-0.0.28/cloudquery/discovery_v1/discovery_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cloudquery_plugin_pb-0.0.27/cloudquery/discovery_v1/discovery_pb2_grpc.py` & `cloudquery_plugin_pb-0.0.28/cloudquery/discovery_v1/discovery_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
 from cloudquery.discovery_v1 import discovery_pb2 as cloudquery_dot_discovery__v1_dot_discovery__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
+GRPC_GENERATED_VERSION = '1.64.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
 
 try:
     from grpc._utilities import first_version_is_lower
@@ -64,14 +64,15 @@
                     request_deserializer=cloudquery_dot_discovery__v1_dot_discovery__pb2.GetVersions.Request.FromString,
                     response_serializer=cloudquery_dot_discovery__v1_dot_discovery__pb2.GetVersions.Response.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'cloudquery.discovery.v1.Discovery', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('cloudquery.discovery.v1.Discovery', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class Discovery(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
```

### Comparing `cloudquery_plugin_pb-0.0.27/cloudquery/plugin_v3/arrow.py` & `cloudquery_plugin_pb-0.0.28/cloudquery/plugin_v3/arrow.py`

 * *Files identical despite different names*

### Comparing `cloudquery_plugin_pb-0.0.27/cloudquery/plugin_v3/plugin_pb2.py` & `cloudquery_plugin_pb-0.0.28/cloudquery/plugin_v3/plugin_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!cloudquery/plugin_v3/plugin.proto\x12\x14\x63loudquery.plugin.v3\x1a\x1fgoogle/protobuf/timestamp.proto\".\n\x07GetName\x1a\t\n\x07Request\x1a\x18\n\x08Response\x12\x0c\n\x04name\x18\x01 \x01(\t\"4\n\nGetVersion\x1a\t\n\x07Request\x1a\x1b\n\x08Response\x12\x0f\n\x07version\x18\x01 \x01(\t\"P\n\rGetSpecSchema\x1a\t\n\x07Request\x1a\x34\n\x08Response\x12\x18\n\x0bjson_schema\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_json_schema\"Y\n\x04Init\x1a\x45\n\x07Request\x12\x0c\n\x04spec\x18\x01 \x01(\x0c\x12\x15\n\rno_connection\x18\x02 \x01(\x08\x12\x15\n\rinvocation_id\x18\x03 \x01(\t\x1a\n\n\x08Response\"v\n\tGetTables\x1aM\n\x07Request\x12\x0e\n\x06tables\x18\x01 \x03(\t\x12\x13\n\x0bskip_tables\x18\x02 \x03(\t\x12\x1d\n\x15skip_dependent_tables\x18\x03 \x01(\x08\x1a\x1a\n\x08Response\x12\x0e\n\x06tables\x18\x01 \x03(\x0c\"\xbd\x05\n\x04Sync\x1a\x1f\n\rMessageInsert\x12\x0e\n\x06record\x18\x01 \x01(\x0c\x1a$\n\x13MessageMigrateTable\x12\r\n\x05table\x18\x01 \x01(\x0c\x1a\xa4\x01\n\x13MessageDeleteRecord\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12;\n\x0cwhere_clause\x18\x02 \x03(\x0b\x32%.cloudquery.plugin.v3.PredicatesGroup\x12<\n\x0ftable_relations\x18\x03 \x03(\x0b\x32#.cloudquery.plugin.v3.TableRelation\x1a\x38\n\x0e\x42\x61\x63kendOptions\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x12\n\nconnection\x18\x02 \x01(\t\x1a\xa6\x01\n\x07Request\x12\x0e\n\x06tables\x18\x01 \x03(\t\x12\x13\n\x0bskip_tables\x18\x02 \x03(\t\x12\x1d\n\x15skip_dependent_tables\x18\x03 \x01(\x08\x12\x1b\n\x13\x64\x65terministic_cq_id\x18\x04 \x01(\x08\x12:\n\x07\x62\x61\x63kend\x18\x05 \x01(\x0b\x32).cloudquery.plugin.v3.Sync.BackendOptions\x1a\xe3\x01\n\x08Response\x12G\n\rmigrate_table\x18\x01 \x01(\x0b\x32..cloudquery.plugin.v3.Sync.MessageMigrateTableH\x00\x12:\n\x06insert\x18\x02 \x01(\x0b\x32(.cloudquery.plugin.v3.Sync.MessageInsertH\x00\x12G\n\rdelete_record\x18\x03 \x01(\x0b\x32..cloudquery.plugin.v3.Sync.MessageDeleteRecordH\x00\x42\t\n\x07message\"<\n\x04Read\x1a\x18\n\x07Request\x12\r\n\x05table\x18\x01 \x01(\x0c\x1a\x1a\n\x08Response\x12\x0e\n\x06record\x18\x01 \x01(\x0c\"9\n\rTableRelation\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x14\n\x0cparent_table\x18\x02 \x01(\t\"{\n\tPredicate\x12:\n\x08operator\x18\x01 \x01(\x0e\x32(.cloudquery.plugin.v3.Predicate.Operator\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0e\n\x06record\x18\x03 \x01(\x0c\"\x12\n\x08Operator\x12\x06\n\x02\x45Q\x10\x00\"\xb2\x01\n\x0fPredicatesGroup\x12I\n\rgrouping_type\x18\x01 \x01(\x0e\x32\x32.cloudquery.plugin.v3.PredicatesGroup.GroupingType\x12\x33\n\npredicates\x18\x02 \x03(\x0b\x32\x1f.cloudquery.plugin.v3.Predicate\"\x1f\n\x0cGroupingType\x12\x07\n\x03\x41ND\x10\x00\x12\x06\n\x02OR\x10\x01\"\xc3\x05\n\x05Write\x1a;\n\x13MessageMigrateTable\x12\r\n\x05table\x18\x01 \x01(\x0c\x12\x15\n\rmigrate_force\x18\x02 \x01(\x08\x1a\x1f\n\rMessageInsert\x12\x0e\n\x06record\x18\x01 \x01(\x0c\x1a\x7f\n\x12MessageDeleteStale\x12\x11\n\x05table\x18\x01 \x01(\x0c\x42\x02\x18\x01\x12\x13\n\x0bsource_name\x18\x02 \x01(\t\x12-\n\tsync_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ntable_name\x18\x04 \x01(\t\x1a\xa4\x01\n\x13MessageDeleteRecord\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12;\n\x0cwhere_clause\x18\x02 \x03(\x0b\x32%.cloudquery.plugin.v3.PredicatesGroup\x12<\n\x0ftable_relations\x18\x03 \x03(\x0b\x32#.cloudquery.plugin.v3.TableRelation\x1a\xa7\x02\n\x07Request\x12H\n\rmigrate_table\x18\x01 \x01(\x0b\x32/.cloudquery.plugin.v3.Write.MessageMigrateTableH\x00\x12;\n\x06insert\x18\x02 \x01(\x0b\x32).cloudquery.plugin.v3.Write.MessageInsertH\x00\x12@\n\x06\x64\x65lete\x18\x03 \x01(\x0b\x32..cloudquery.plugin.v3.Write.MessageDeleteStaleH\x00\x12H\n\rdelete_record\x18\x04 \x01(\x0b\x32/.cloudquery.plugin.v3.Write.MessageDeleteRecordH\x00\x42\t\n\x07message\x1a\n\n\x08Response\"\x1e\n\x05\x43lose\x1a\t\n\x07Request\x1a\n\n\x08Response2\xb2\x06\n\x06Plugin\x12X\n\x07GetName\x12%.cloudquery.plugin.v3.GetName.Request\x1a&.cloudquery.plugin.v3.GetName.Response\x12\x61\n\nGetVersion\x12(.cloudquery.plugin.v3.GetVersion.Request\x1a).cloudquery.plugin.v3.GetVersion.Response\x12j\n\rGetSpecSchema\x12+.cloudquery.plugin.v3.GetSpecSchema.Request\x1a,.cloudquery.plugin.v3.GetSpecSchema.Response\x12O\n\x04Init\x12\".cloudquery.plugin.v3.Init.Request\x1a#.cloudquery.plugin.v3.Init.Response\x12^\n\tGetTables\x12\'.cloudquery.plugin.v3.GetTables.Request\x1a(.cloudquery.plugin.v3.GetTables.Response\x12Q\n\x04Sync\x12\".cloudquery.plugin.v3.Sync.Request\x1a#.cloudquery.plugin.v3.Sync.Response0\x01\x12Q\n\x04Read\x12\".cloudquery.plugin.v3.Read.Request\x1a#.cloudquery.plugin.v3.Read.Response0\x01\x12T\n\x05Write\x12#.cloudquery.plugin.v3.Write.Request\x1a$.cloudquery.plugin.v3.Write.Response(\x01\x12R\n\x05\x43lose\x12#.cloudquery.plugin.v3.Close.Request\x1a$.cloudquery.plugin.v3.Close.ResponseBS\n\x17io.cloudquery.plugin.v3P\x01Z6github.com/cloudquery/plugin-pb-go/pb/plugin/v3;pluginb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!cloudquery/plugin_v3/plugin.proto\x12\x14\x63loudquery.plugin.v3\x1a\x1fgoogle/protobuf/timestamp.proto\".\n\x07GetName\x1a\t\n\x07Request\x1a\x18\n\x08Response\x12\x0c\n\x04name\x18\x01 \x01(\t\"4\n\nGetVersion\x1a\t\n\x07Request\x1a\x1b\n\x08Response\x12\x0f\n\x07version\x18\x01 \x01(\t\"P\n\rGetSpecSchema\x1a\t\n\x07Request\x1a\x34\n\x08Response\x12\x18\n\x0bjson_schema\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_json_schema\"Y\n\x04Init\x1a\x45\n\x07Request\x12\x0c\n\x04spec\x18\x01 \x01(\x0c\x12\x15\n\rno_connection\x18\x02 \x01(\x08\x12\x15\n\rinvocation_id\x18\x03 \x01(\t\x1a\n\n\x08Response\"v\n\tGetTables\x1aM\n\x07Request\x12\x0e\n\x06tables\x18\x01 \x03(\t\x12\x13\n\x0bskip_tables\x18\x02 \x03(\t\x12\x1d\n\x15skip_dependent_tables\x18\x03 \x01(\x08\x1a\x1a\n\x08Response\x12\x0e\n\x06tables\x18\x01 \x03(\x0c\"\xbd\x05\n\x04Sync\x1a\x1f\n\rMessageInsert\x12\x0e\n\x06record\x18\x01 \x01(\x0c\x1a$\n\x13MessageMigrateTable\x12\r\n\x05table\x18\x01 \x01(\x0c\x1a\xa4\x01\n\x13MessageDeleteRecord\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12;\n\x0cwhere_clause\x18\x02 \x03(\x0b\x32%.cloudquery.plugin.v3.PredicatesGroup\x12<\n\x0ftable_relations\x18\x03 \x03(\x0b\x32#.cloudquery.plugin.v3.TableRelation\x1a\x38\n\x0e\x42\x61\x63kendOptions\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x12\n\nconnection\x18\x02 \x01(\t\x1a\xa6\x01\n\x07Request\x12\x0e\n\x06tables\x18\x01 \x03(\t\x12\x13\n\x0bskip_tables\x18\x02 \x03(\t\x12\x1d\n\x15skip_dependent_tables\x18\x03 \x01(\x08\x12\x1b\n\x13\x64\x65terministic_cq_id\x18\x04 \x01(\x08\x12:\n\x07\x62\x61\x63kend\x18\x05 \x01(\x0b\x32).cloudquery.plugin.v3.Sync.BackendOptions\x1a\xe3\x01\n\x08Response\x12G\n\rmigrate_table\x18\x01 \x01(\x0b\x32..cloudquery.plugin.v3.Sync.MessageMigrateTableH\x00\x12:\n\x06insert\x18\x02 \x01(\x0b\x32(.cloudquery.plugin.v3.Sync.MessageInsertH\x00\x12G\n\rdelete_record\x18\x03 \x01(\x0b\x32..cloudquery.plugin.v3.Sync.MessageDeleteRecordH\x00\x42\t\n\x07message\"<\n\x04Read\x1a\x18\n\x07Request\x12\r\n\x05table\x18\x01 \x01(\x0c\x1a\x1a\n\x08Response\x12\x0e\n\x06record\x18\x01 \x01(\x0c\"9\n\rTableRelation\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12\x14\n\x0cparent_table\x18\x02 \x01(\t\"{\n\tPredicate\x12:\n\x08operator\x18\x01 \x01(\x0e\x32(.cloudquery.plugin.v3.Predicate.Operator\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0e\n\x06record\x18\x03 \x01(\x0c\"\x12\n\x08Operator\x12\x06\n\x02\x45Q\x10\x00\"\xb2\x01\n\x0fPredicatesGroup\x12I\n\rgrouping_type\x18\x01 \x01(\x0e\x32\x32.cloudquery.plugin.v3.PredicatesGroup.GroupingType\x12\x33\n\npredicates\x18\x02 \x03(\x0b\x32\x1f.cloudquery.plugin.v3.Predicate\"\x1f\n\x0cGroupingType\x12\x07\n\x03\x41ND\x10\x00\x12\x06\n\x02OR\x10\x01\"\xc3\x05\n\x05Write\x1a;\n\x13MessageMigrateTable\x12\r\n\x05table\x18\x01 \x01(\x0c\x12\x15\n\rmigrate_force\x18\x02 \x01(\x08\x1a\x1f\n\rMessageInsert\x12\x0e\n\x06record\x18\x01 \x01(\x0c\x1a\x7f\n\x12MessageDeleteStale\x12\x11\n\x05table\x18\x01 \x01(\x0c\x42\x02\x18\x01\x12\x13\n\x0bsource_name\x18\x02 \x01(\t\x12-\n\tsync_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ntable_name\x18\x04 \x01(\t\x1a\xa4\x01\n\x13MessageDeleteRecord\x12\x12\n\ntable_name\x18\x01 \x01(\t\x12;\n\x0cwhere_clause\x18\x02 \x03(\x0b\x32%.cloudquery.plugin.v3.PredicatesGroup\x12<\n\x0ftable_relations\x18\x03 \x03(\x0b\x32#.cloudquery.plugin.v3.TableRelation\x1a\xa7\x02\n\x07Request\x12H\n\rmigrate_table\x18\x01 \x01(\x0b\x32/.cloudquery.plugin.v3.Write.MessageMigrateTableH\x00\x12;\n\x06insert\x18\x02 \x01(\x0b\x32).cloudquery.plugin.v3.Write.MessageInsertH\x00\x12@\n\x06\x64\x65lete\x18\x03 \x01(\x0b\x32..cloudquery.plugin.v3.Write.MessageDeleteStaleH\x00\x12H\n\rdelete_record\x18\x04 \x01(\x0b\x32/.cloudquery.plugin.v3.Write.MessageDeleteRecordH\x00\x42\t\n\x07message\x1a\n\n\x08Response\"\x1e\n\x05\x43lose\x1a\t\n\x07Request\x1a\n\n\x08Response\"y\n\x0eTestConnection\x1a\x17\n\x07Request\x12\x0c\n\x04spec\x18\x01 \x01(\x0c\x1aN\n\x08Response\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x14\n\x0c\x66\x61ilure_code\x18\x02 \x01(\t\x12\x1b\n\x13\x66\x61ilure_description\x18\x03 \x01(\t2\xa1\x07\n\x06Plugin\x12X\n\x07GetName\x12%.cloudquery.plugin.v3.GetName.Request\x1a&.cloudquery.plugin.v3.GetName.Response\x12\x61\n\nGetVersion\x12(.cloudquery.plugin.v3.GetVersion.Request\x1a).cloudquery.plugin.v3.GetVersion.Response\x12j\n\rGetSpecSchema\x12+.cloudquery.plugin.v3.GetSpecSchema.Request\x1a,.cloudquery.plugin.v3.GetSpecSchema.Response\x12O\n\x04Init\x12\".cloudquery.plugin.v3.Init.Request\x1a#.cloudquery.plugin.v3.Init.Response\x12^\n\tGetTables\x12\'.cloudquery.plugin.v3.GetTables.Request\x1a(.cloudquery.plugin.v3.GetTables.Response\x12Q\n\x04Sync\x12\".cloudquery.plugin.v3.Sync.Request\x1a#.cloudquery.plugin.v3.Sync.Response0\x01\x12Q\n\x04Read\x12\".cloudquery.plugin.v3.Read.Request\x1a#.cloudquery.plugin.v3.Read.Response0\x01\x12T\n\x05Write\x12#.cloudquery.plugin.v3.Write.Request\x1a$.cloudquery.plugin.v3.Write.Response(\x01\x12R\n\x05\x43lose\x12#.cloudquery.plugin.v3.Close.Request\x1a$.cloudquery.plugin.v3.Close.Response\x12m\n\x0eTestConnection\x12,.cloudquery.plugin.v3.TestConnection.Request\x1a-.cloudquery.plugin.v3.TestConnection.ResponseBS\n\x17io.cloudquery.plugin.v3P\x01Z6github.com/cloudquery/plugin-pb-go/pb/plugin/v3;pluginb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'cloudquery.plugin_v3.plugin_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\027io.cloudquery.plugin.v3P\001Z6github.com/cloudquery/plugin-pb-go/pb/plugin/v3;plugin'
@@ -101,10 +101,16 @@
   _globals['_WRITE_RESPONSE']._serialized_end=124
   _globals['_CLOSE']._serialized_start=2328
   _globals['_CLOSE']._serialized_end=2358
   _globals['_CLOSE_REQUEST']._serialized_start=103
   _globals['_CLOSE_REQUEST']._serialized_end=112
   _globals['_CLOSE_RESPONSE']._serialized_start=114
   _globals['_CLOSE_RESPONSE']._serialized_end=124
-  _globals['_PLUGIN']._serialized_start=2361
-  _globals['_PLUGIN']._serialized_end=3179
+  _globals['_TESTCONNECTION']._serialized_start=2360
+  _globals['_TESTCONNECTION']._serialized_end=2481
+  _globals['_TESTCONNECTION_REQUEST']._serialized_start=284
+  _globals['_TESTCONNECTION_REQUEST']._serialized_end=307
+  _globals['_TESTCONNECTION_RESPONSE']._serialized_start=2403
+  _globals['_TESTCONNECTION_RESPONSE']._serialized_end=2481
+  _globals['_PLUGIN']._serialized_start=2484
+  _globals['_PLUGIN']._serialized_end=3413
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cloudquery_plugin_pb-0.0.27/cloudquery/plugin_v3/plugin_pb2.pyi` & `cloudquery_plugin_pb-0.0.28/cloudquery/plugin_v3/plugin_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -234,7 +234,25 @@
     class Request(_message.Message):
         __slots__ = ()
         def __init__(self) -> None: ...
     class Response(_message.Message):
         __slots__ = ()
         def __init__(self) -> None: ...
     def __init__(self) -> None: ...
+
+class TestConnection(_message.Message):
+    __slots__ = ()
+    class Request(_message.Message):
+        __slots__ = ("spec",)
+        SPEC_FIELD_NUMBER: _ClassVar[int]
+        spec: bytes
+        def __init__(self, spec: _Optional[bytes] = ...) -> None: ...
+    class Response(_message.Message):
+        __slots__ = ("success", "failure_code", "failure_description")
+        SUCCESS_FIELD_NUMBER: _ClassVar[int]
+        FAILURE_CODE_FIELD_NUMBER: _ClassVar[int]
+        FAILURE_DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+        success: bool
+        failure_code: str
+        failure_description: str
+        def __init__(self, success: bool = ..., failure_code: _Optional[str] = ..., failure_description: _Optional[str] = ...) -> None: ...
+    def __init__(self) -> None: ...
```

### Comparing `cloudquery_plugin_pb-0.0.27/cloudquery/plugin_v3/plugin_pb2_grpc.py` & `cloudquery_plugin_pb-0.0.28/cloudquery/plugin_v3/plugin_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 import warnings
 
 from cloudquery.plugin_v3 import plugin_pb2 as cloudquery_dot_plugin__v3_dot_plugin__pb2
 
-GRPC_GENERATED_VERSION = '1.63.0'
+GRPC_GENERATED_VERSION = '1.64.0'
 GRPC_VERSION = grpc.__version__
 EXPECTED_ERROR_RELEASE = '1.65.0'
 SCHEDULED_RELEASE_DATE = 'June 25, 2024'
 _version_not_supported = False
 
 try:
     from grpc._utilities import first_version_is_lower
@@ -80,14 +80,19 @@
                 response_deserializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.Write.Response.FromString,
                 _registered_method=True)
         self.Close = channel.unary_unary(
                 '/cloudquery.plugin.v3.Plugin/Close',
                 request_serializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.Close.Request.SerializeToString,
                 response_deserializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.Close.Response.FromString,
                 _registered_method=True)
+        self.TestConnection = channel.unary_unary(
+                '/cloudquery.plugin.v3.Plugin/TestConnection',
+                request_serializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.TestConnection.Request.SerializeToString,
+                response_deserializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.TestConnection.Response.FromString,
+                _registered_method=True)
 
 
 class PluginServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetName(self, request, context):
         """Get the name of the plugin
@@ -151,14 +156,21 @@
     def Close(self, request, context):
         """Send signal to flush and close open connections
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def TestConnection(self, request, context):
+        """Validate and test the connections used by the plugin
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_PluginServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetName': grpc.unary_unary_rpc_method_handler(
                     servicer.GetName,
                     request_deserializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.GetName.Request.FromString,
                     response_serializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.GetName.Response.SerializeToString,
@@ -199,18 +211,24 @@
                     response_serializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.Write.Response.SerializeToString,
             ),
             'Close': grpc.unary_unary_rpc_method_handler(
                     servicer.Close,
                     request_deserializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.Close.Request.FromString,
                     response_serializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.Close.Response.SerializeToString,
             ),
+            'TestConnection': grpc.unary_unary_rpc_method_handler(
+                    servicer.TestConnection,
+                    request_deserializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.TestConnection.Request.FromString,
+                    response_serializer=cloudquery_dot_plugin__v3_dot_plugin__pb2.TestConnection.Response.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'cloudquery.plugin.v3.Plugin', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('cloudquery.plugin.v3.Plugin', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class Plugin(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
@@ -449,9 +467,36 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+            _registered_method=True)
+
+    @staticmethod
+    def TestConnection(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/cloudquery.plugin.v3.Plugin/TestConnection',
+            cloudquery_dot_plugin__v3_dot_plugin__pb2.TestConnection.Request.SerializeToString,
+            cloudquery_dot_plugin__v3_dot_plugin__pb2.TestConnection.Response.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
             _registered_method=True)
```

### Comparing `cloudquery_plugin_pb-0.0.27/cloudquery_plugin_pb.egg-info/PKG-INFO` & `cloudquery_plugin_pb-0.0.28/cloudquery_plugin_pb.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-pb
-Version: 0.0.27
+Version: 0.0.28
 Summary: CloudQuery Plugin client and server library
 Home-page: https://github.com/cloudquery/plugin-pb-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery_plugin_pb-0.0.27/cloudquery_plugin_pb.egg-info/SOURCES.txt` & `cloudquery_plugin_pb-0.0.28/cloudquery_plugin_pb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudquery_plugin_pb-0.0.27/setup.py` & `cloudquery_plugin_pb-0.0.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("cloudquery")
 ]
 setuptools.setup(
     name=name,
-    version="0.0.27",
+    version="0.0.28",
     description=description,
     long_description=long_description,
     author="CloudQuery LTD",
     author_email="pypi-packages@cloudquery.io",
     license="MPL-2.0",
     url=url,
     classifiers=[
```

