# Comparing `tmp/isolate_proto-0.3.4.tar.gz` & `tmp/isolate_proto-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isolate_proto-0.3.4.tar", max compression
+gzip compressed data, was "isolate_proto-0.4.0.tar", last modified: Wed May  1 20:16:41 2024, max compression
```

## Comparing `isolate_proto-0.3.4.tar` & `isolate_proto-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,28 @@
--rw-r--r--   0        0        0      353 2024-03-19 21:17:59.675764 isolate_proto-0.3.4/README.md
--rw-r--r--   0        0        0      417 2024-03-19 21:18:12.631845 isolate_proto-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1337 2024-03-19 21:17:59.675764 isolate_proto-0.3.4/src/isolate_proto/__init__.py
--rw-r--r--   0        0        0     1013 2024-03-19 21:17:59.675764 isolate_proto-0.3.4/src/isolate_proto/configuration.py
--rw-r--r--   0        0        0     7470 2024-03-19 21:17:59.675764 isolate_proto-0.3.4/src/isolate_proto/controller.proto
--rw-r--r--   0        0        0    13684 2024-03-19 21:17:59.675764 isolate_proto-0.3.4/src/isolate_proto/controller_pb2.py
--rw-r--r--   0        0        0    42053 2024-03-19 21:17:59.675764 isolate_proto-0.3.4/src/isolate_proto/controller_pb2.pyi
--rw-r--r--   0        0        0    21801 2024-03-19 21:17:59.675764 isolate_proto-0.3.4/src/isolate_proto/controller_pb2_grpc.py
--rw-r--r--   0        0        0      264 2024-03-19 21:17:59.675764 isolate_proto-0.3.4/src/isolate_proto/health/__init__.py
--rw-r--r--   0        0        0      455 2024-03-19 21:17:59.675764 isolate_proto-0.3.4/src/isolate_proto/health/health.proto
--rw-r--r--   0        0        0     1819 2024-03-19 21:17:59.679764 isolate_proto-0.3.4/src/isolate_proto/health/health_pb2.py
--rw-r--r--   0        0        0     2546 2024-03-19 21:17:59.679764 isolate_proto-0.3.4/src/isolate_proto/health/health_pb2.pyi
--rw-r--r--   0        0        0     4040 2024-03-19 21:17:59.679764 isolate_proto-0.3.4/src/isolate_proto/health/health_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-03-19 21:17:59.679764 isolate_proto-0.3.4/src/isolate_proto/py.typed
--rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 isolate_proto-0.3.4/setup.py
--rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 isolate_proto-0.3.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:16:41.428489 isolate_proto-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-01 20:16:41.428489 isolate_proto-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 20:16:41.428489 isolate_proto-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:16:41.424489 isolate_proto-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:16:41.424489 isolate_proto-0.4.0/src/isolate_proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/controller.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/controller_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38472 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/controller_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24515 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/controller_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:16:41.428489 isolate_proto-0.4.0/src/isolate_proto/health/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/health/health.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/health/health_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/health/health_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/health/health_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/src/isolate_proto/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:16:41.428489 isolate_proto-0.4.0/src/isolate_proto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-01 20:16:41.000000 isolate_proto-0.4.0/src/isolate_proto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-01 20:16:41.000000 isolate_proto-0.4.0/src/isolate_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 20:16:41.000000 isolate_proto-0.4.0/src/isolate_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 20:16:41.000000 isolate_proto-0.4.0/src/isolate_proto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 20:16:41.000000 isolate_proto-0.4.0/src/isolate_proto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 20:16:41.428489 isolate_proto-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-01 20:16:35.000000 isolate_proto-0.4.0/tests/test_proto.py
```

### Comparing `isolate_proto-0.3.4/src/isolate_proto/__init__.py` & `isolate_proto-0.4.0/src/isolate_proto/__init__.py`

 * *Files identical despite different names*

### Comparing `isolate_proto-0.3.4/src/isolate_proto/configuration.py` & `isolate_proto-0.4.0/src/isolate_proto/configuration.py`

 * *Files identical despite different names*

### Comparing `isolate_proto-0.3.4/src/isolate_proto/controller.proto` & `isolate_proto-0.4.0/src/isolate_proto/controller.proto`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     rpc ListUserKeys (ListUserKeysRequest) returns (ListUserKeysResponse) {}
     // Revokes an authentication key for a user
     rpc RevokeUserKey (RevokeUserKeyRequest) returns (RevokeUserKeyResponse) {}
     // Register a funtion
     rpc RegisterApplication (RegisterApplicationRequest) returns (stream RegisterApplicationResult) {};
     // Update configuration of an existing application.
     rpc UpdateApplication (UpdateApplicationRequest) returns (UpdateApplicationResult) {};
+    // List functions
+    rpc ListApplications (ListApplicationsRequest) returns (ListApplicationsResult) {};
+    // Delete a function
+    rpc DeleteApplication (DeleteApplicationRequest) returns (DeleteApplicationResult) {};
     // Set alias to point to an existing application.
     rpc SetAlias (SetAliasRequest) returns (SetAliasResult) {};
     // Delete an alias.
     rpc DeleteAlias (DeleteAliasRequest) returns (DeleteAliasResult) {};
     // List aliased registered functions
     rpc ListAliases (ListAliasesRequest) returns (ListAliasesResult) {};
     // Sets a user secret.
@@ -193,14 +197,39 @@
     optional int32 min_concurrency = 5;
 }
 
 message UpdateApplicationResult {
     AliasInfo alias_info = 1;
 }
 
+message ListApplicationsRequest {
+    // Empty. For future use.
+}
+
+message ApplicationInfo {
+    string application_id = 1;
+    int32 max_concurrency = 2;
+    int32 max_multiplexing = 3;
+    int32 keep_alive = 4;
+    int32 active_runners = 6;
+    int32 min_concurrency = 7;
+}
+
+message ListApplicationsResult {
+    repeated ApplicationInfo applications = 1;
+}
+
+message DeleteApplicationRequest {
+    string application_id = 1;
+}
+
+message DeleteApplicationResult {
+    // Empty. For future use.
+}
+
 message SetAliasRequest {
     string alias = 1;
     string revision = 2;
     ApplicationAuthMode auth_mode = 3;
 }
 
 message SetAliasResult {
```

### Comparing `isolate_proto-0.3.4/src/isolate_proto/controller_pb2.py` & `isolate_proto-0.4.0/src/isolate_proto/controller_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,113 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: controller.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from isolate.connections.grpc.definitions import common_pb2 as common__pb2
 from isolate.server.definitions import server_pb2 as server__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x10\x63ontroller.proto\x12\ncontroller\x1a\x0c\x63ommon.proto\x1a\x0cserver.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto"\xde\x01\n\tHostedMap\x12,\n\x0c\x65nvironments\x18\x01 \x03(\x0b\x32\x16.EnvironmentDefinition\x12\x42\n\x14machine_requirements\x18\x02 \x01(\x0b\x32\x1f.controller.MachineRequirementsH\x00\x88\x01\x01\x12#\n\x08\x66unction\x18\x03 \x01(\x0b\x32\x11.SerializedObject\x12!\n\x06inputs\x18\x04 \x03(\x0b\x32\x11.SerializedObjectB\x17\n\x15_machine_requirements"\xf6\x01\n\tHostedRun\x12,\n\x0c\x65nvironments\x18\x01 \x03(\x0b\x32\x16.EnvironmentDefinition\x12\x42\n\x14machine_requirements\x18\x02 \x01(\x0b\x32\x1f.controller.MachineRequirementsH\x00\x88\x01\x01\x12#\n\x08\x66unction\x18\x03 \x01(\x0b\x32\x11.SerializedObject\x12*\n\nsetup_func\x18\x04 \x01(\x0b\x32\x11.SerializedObjectH\x01\x88\x01\x01\x42\x17\n\x15_machine_requirementsB\r\n\x0b_setup_func"\x88\x01\n\x14\x43reateUserKeyRequest\x12\x35\n\x05scope\x18\x01 \x01(\x0e\x32&.controller.CreateUserKeyRequest.Scope\x12\x12\n\x05\x61lias\x18\x02 \x01(\tH\x00\x88\x01\x01"\x1b\n\x05Scope\x12\t\n\x05\x41\x44MIN\x10\x00\x12\x07\n\x03\x41PI\x10\x01\x42\x08\n\x06_alias";\n\x15\x43reateUserKeyResponse\x12\x12\n\nkey_secret\x18\x01 \x01(\t\x12\x0e\n\x06key_id\x18\x02 \x01(\t"\x15\n\x13ListUserKeysRequest"B\n\x14ListUserKeysResponse\x12*\n\tuser_keys\x18\x01 \x03(\x0b\x32\x17.controller.UserKeyInfo"&\n\x14RevokeUserKeyRequest\x12\x0e\n\x06key_id\x18\x01 \x01(\t"\x17\n\x15RevokeUserKeyResponse"\x93\x01\n\x0bUserKeyInfo\x12\x0e\n\x06key_id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x05scope\x18\x03 \x01(\x0e\x32&.controller.CreateUserKeyRequest.Scope\x12\r\n\x05\x61lias\x18\x04 \x01(\t"\xb1\x01\n\x0fHostedRunResult\x12\x0e\n\x06run_id\x18\x01 \x01(\t\x12\x30\n\x06status\x18\x02 \x01(\x0b\x32\x1b.controller.HostedRunStatusH\x00\x88\x01\x01\x12\x12\n\x04logs\x18\x03 \x03(\x0b\x32\x04.Log\x12,\n\x0creturn_value\x18\x04 \x01(\x0b\x32\x11.SerializedObjectH\x01\x88\x01\x01\x42\t\n\x07_statusB\x0f\n\r_return_value"\x80\x01\n\x0fHostedRunStatus\x12\x30\n\x05state\x18\x01 \x01(\x0e\x32!.controller.HostedRunStatus.State";\n\x05State\x12\x0f\n\x0bIN_PROGRESS\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\x14\n\x10INTERNAL_FAILURE\x10\x02"\xb4\x03\n\x13MachineRequirements\x12\x14\n\x0cmachine_type\x18\x01 \x01(\t\x12\x17\n\nkeep_alive\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x17\n\nbase_image\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x19\n\x0c\x65xposed_port\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x16\n\tscheduler\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x37\n\x11scheduler_options\x18\x08 \x01(\x0b\x32\x17.google.protobuf.StructH\x04\x88\x01\x01\x12\x1d\n\x10max_multiplexing\x18\x06 \x01(\x05H\x05\x88\x01\x01\x12\x1c\n\x0fmax_concurrency\x18\t \x01(\x05H\x06\x88\x01\x01\x12\x1c\n\x0fmin_concurrency\x18\n \x01(\x05H\x07\x88\x01\x01\x42\r\n\x0b_keep_aliveB\r\n\x0b_base_imageB\x0f\n\r_exposed_portB\x0c\n\n_schedulerB\x14\n\x12_scheduler_optionsB\x13\n\x11_max_multiplexingB\x12\n\x10_max_concurrencyB\x12\n\x10_min_concurrency"\xf5\x03\n\x1aRegisterApplicationRequest\x12,\n\x0c\x65nvironments\x18\x01 \x03(\x0b\x32\x16.EnvironmentDefinition\x12\x42\n\x14machine_requirements\x18\x02 \x01(\x0b\x32\x1f.controller.MachineRequirementsH\x00\x88\x01\x01\x12#\n\x08\x66unction\x18\x03 \x01(\x0b\x32\x11.SerializedObject\x12*\n\nsetup_func\x18\x04 \x01(\x0b\x32\x11.SerializedObjectH\x01\x88\x01\x01\x12\x1d\n\x10\x61pplication_name\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x37\n\tauth_mode\x18\x06 \x01(\x0e\x32\x1f.controller.ApplicationAuthModeH\x03\x88\x01\x01\x12 \n\x0fmax_concurrency\x18\x07 \x01(\x05\x42\x02\x18\x01H\x04\x88\x01\x01\x12.\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.StructH\x05\x88\x01\x01\x42\x17\n\x15_machine_requirementsB\r\n\x0b_setup_funcB\x13\n\x11_application_nameB\x0c\n\n_auth_modeB\x12\n\x10_max_concurrencyB\x0b\n\t_metadata"7\n\x1dRegisterApplicationResultType\x12\x16\n\x0e\x61pplication_id\x18\x01 \x01(\t"z\n\x19RegisterApplicationResult\x12\x12\n\x04logs\x18\x01 \x03(\x0b\x32\x04.Log\x12>\n\x06result\x18\x02 \x01(\x0b\x32).controller.RegisterApplicationResultTypeH\x00\x88\x01\x01\x42\t\n\x07_result"\xf4\x01\n\x18UpdateApplicationRequest\x12\x18\n\x10\x61pplication_name\x18\x01 \x01(\t\x12\x17\n\nkeep_alive\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x1d\n\x10max_multiplexing\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12\x1c\n\x0fmax_concurrency\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1c\n\x0fmin_concurrency\x18\x05 \x01(\x05H\x03\x88\x01\x01\x42\r\n\x0b_keep_aliveB\x13\n\x11_max_multiplexingB\x12\n\x10_max_concurrencyB\x12\n\x10_min_concurrency"D\n\x17UpdateApplicationResult\x12)\n\nalias_info\x18\x01 \x01(\x0b\x32\x15.controller.AliasInfo"f\n\x0fSetAliasRequest\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12\x10\n\x08revision\x18\x02 \x01(\t\x12\x32\n\tauth_mode\x18\x03 \x01(\x0e\x32\x1f.controller.ApplicationAuthMode"\x10\n\x0eSetAliasResult"#\n\x12\x44\x65leteAliasRequest\x12\r\n\x05\x61lias\x18\x01 \x01(\t"%\n\x11\x44\x65leteAliasResult\x12\x10\n\x08revision\x18\x01 \x01(\t"\x14\n\x12ListAliasesRequest";\n\x11ListAliasesResult\x12&\n\x07\x61liases\x18\x01 \x03(\x0b\x32\x15.controller.AliasInfo"\xd8\x01\n\tAliasInfo\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12\x10\n\x08revision\x18\x02 \x01(\t\x12\x32\n\tauth_mode\x18\x03 \x01(\x0e\x32\x1f.controller.ApplicationAuthMode\x12\x17\n\x0fmax_concurrency\x18\x04 \x01(\x05\x12\x18\n\x10max_multiplexing\x18\x05 \x01(\x05\x12\x12\n\nkeep_alive\x18\x06 \x01(\x05\x12\x16\n\x0e\x61\x63tive_runners\x18\x07 \x01(\x05\x12\x17\n\x0fmin_concurrency\x18\x08 \x01(\x05">\n\x10SetSecretRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\x05value\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_value"\x13\n\x11SetSecretResponse"\x14\n\x12ListSecretsRequest"^\n\x06Secret\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x35\n\x0c\x63reated_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x42\x0f\n\r_created_time":\n\x13ListSecretsResponse\x12#\n\x07secrets\x18\x01 \x03(\x0b\x32\x12.controller.Secret"(\n\x17ListAliasRunnersRequest\x12\r\n\x05\x61lias\x18\x01 \x01(\t"C\n\x18ListAliasRunnersResponse\x12\'\n\x07runners\x18\x01 \x03(\x0b\x32\x16.controller.RunnerInfo"i\n\nRunnerInfo\x12\x11\n\trunner_id\x18\x01 \x01(\t\x12\x1a\n\x12in_flight_requests\x18\x02 \x01(\x05\x12\x1c\n\x14\x65xpiration_countdown\x18\x03 \x01(\x05\x12\x0e\n\x06uptime\x18\x04 \x01(\x02*:\n\x13\x41pplicationAuthMode\x12\x0b\n\x07PRIVATE\x10\x00\x12\n\n\x06PUBLIC\x10\x01\x12\n\n\x06SHARED\x10\x02\x32\xc8\x08\n\x11IsolateController\x12=\n\x03Run\x12\x15.controller.HostedRun\x1a\x1b.controller.HostedRunResult"\x00\x30\x01\x12=\n\x03Map\x12\x15.controller.HostedMap\x1a\x1b.controller.HostedRunResult"\x00\x30\x01\x12V\n\rCreateUserKey\x12 .controller.CreateUserKeyRequest\x1a!.controller.CreateUserKeyResponse"\x00\x12S\n\x0cListUserKeys\x12\x1f.controller.ListUserKeysRequest\x1a .controller.ListUserKeysResponse"\x00\x12V\n\rRevokeUserKey\x12 .controller.RevokeUserKeyRequest\x1a!.controller.RevokeUserKeyResponse"\x00\x12h\n\x13RegisterApplication\x12&.controller.RegisterApplicationRequest\x1a%.controller.RegisterApplicationResult"\x00\x30\x01\x12`\n\x11UpdateApplication\x12$.controller.UpdateApplicationRequest\x1a#.controller.UpdateApplicationResult"\x00\x12\x45\n\x08SetAlias\x12\x1b.controller.SetAliasRequest\x1a\x1a.controller.SetAliasResult"\x00\x12N\n\x0b\x44\x65leteAlias\x12\x1e.controller.DeleteAliasRequest\x1a\x1d.controller.DeleteAliasResult"\x00\x12N\n\x0bListAliases\x12\x1e.controller.ListAliasesRequest\x1a\x1d.controller.ListAliasesResult"\x00\x12J\n\tSetSecret\x12\x1c.controller.SetSecretRequest\x1a\x1d.controller.SetSecretResponse"\x00\x12P\n\x0bListSecrets\x12\x1e.controller.ListSecretsRequest\x1a\x1f.controller.ListSecretsResponse"\x00\x12_\n\x10ListAliasRunners\x12#.controller.ListAliasRunnersRequest\x1a$.controller.ListAliasRunnersResponse"\x00\x62\x06proto3'
-)
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63ontroller.proto\x12\ncontroller\x1a\x0c\x63ommon.proto\x1a\x0cserver.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xde\x01\n\tHostedMap\x12,\n\x0c\x65nvironments\x18\x01 \x03(\x0b\x32\x16.EnvironmentDefinition\x12\x42\n\x14machine_requirements\x18\x02 \x01(\x0b\x32\x1f.controller.MachineRequirementsH\x00\x88\x01\x01\x12#\n\x08\x66unction\x18\x03 \x01(\x0b\x32\x11.SerializedObject\x12!\n\x06inputs\x18\x04 \x03(\x0b\x32\x11.SerializedObjectB\x17\n\x15_machine_requirements\"\xf6\x01\n\tHostedRun\x12,\n\x0c\x65nvironments\x18\x01 \x03(\x0b\x32\x16.EnvironmentDefinition\x12\x42\n\x14machine_requirements\x18\x02 \x01(\x0b\x32\x1f.controller.MachineRequirementsH\x00\x88\x01\x01\x12#\n\x08\x66unction\x18\x03 \x01(\x0b\x32\x11.SerializedObject\x12*\n\nsetup_func\x18\x04 \x01(\x0b\x32\x11.SerializedObjectH\x01\x88\x01\x01\x42\x17\n\x15_machine_requirementsB\r\n\x0b_setup_func\"\x88\x01\n\x14\x43reateUserKeyRequest\x12\x35\n\x05scope\x18\x01 \x01(\x0e\x32&.controller.CreateUserKeyRequest.Scope\x12\x12\n\x05\x61lias\x18\x02 \x01(\tH\x00\x88\x01\x01\"\x1b\n\x05Scope\x12\t\n\x05\x41\x44MIN\x10\x00\x12\x07\n\x03\x41PI\x10\x01\x42\x08\n\x06_alias\";\n\x15\x43reateUserKeyResponse\x12\x12\n\nkey_secret\x18\x01 \x01(\t\x12\x0e\n\x06key_id\x18\x02 \x01(\t\"\x15\n\x13ListUserKeysRequest\"B\n\x14ListUserKeysResponse\x12*\n\tuser_keys\x18\x01 \x03(\x0b\x32\x17.controller.UserKeyInfo\"&\n\x14RevokeUserKeyRequest\x12\x0e\n\x06key_id\x18\x01 \x01(\t\"\x17\n\x15RevokeUserKeyResponse\"\x93\x01\n\x0bUserKeyInfo\x12\x0e\n\x06key_id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x05scope\x18\x03 \x01(\x0e\x32&.controller.CreateUserKeyRequest.Scope\x12\r\n\x05\x61lias\x18\x04 \x01(\t\"\xb1\x01\n\x0fHostedRunResult\x12\x0e\n\x06run_id\x18\x01 \x01(\t\x12\x30\n\x06status\x18\x02 \x01(\x0b\x32\x1b.controller.HostedRunStatusH\x00\x88\x01\x01\x12\x12\n\x04logs\x18\x03 \x03(\x0b\x32\x04.Log\x12,\n\x0creturn_value\x18\x04 \x01(\x0b\x32\x11.SerializedObjectH\x01\x88\x01\x01\x42\t\n\x07_statusB\x0f\n\r_return_value\"\x80\x01\n\x0fHostedRunStatus\x12\x30\n\x05state\x18\x01 \x01(\x0e\x32!.controller.HostedRunStatus.State\";\n\x05State\x12\x0f\n\x0bIN_PROGRESS\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\x14\n\x10INTERNAL_FAILURE\x10\x02\"\xb4\x03\n\x13MachineRequirements\x12\x14\n\x0cmachine_type\x18\x01 \x01(\t\x12\x17\n\nkeep_alive\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x17\n\nbase_image\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x19\n\x0c\x65xposed_port\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x16\n\tscheduler\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x37\n\x11scheduler_options\x18\x08 \x01(\x0b\x32\x17.google.protobuf.StructH\x04\x88\x01\x01\x12\x1d\n\x10max_multiplexing\x18\x06 \x01(\x05H\x05\x88\x01\x01\x12\x1c\n\x0fmax_concurrency\x18\t \x01(\x05H\x06\x88\x01\x01\x12\x1c\n\x0fmin_concurrency\x18\n \x01(\x05H\x07\x88\x01\x01\x42\r\n\x0b_keep_aliveB\r\n\x0b_base_imageB\x0f\n\r_exposed_portB\x0c\n\n_schedulerB\x14\n\x12_scheduler_optionsB\x13\n\x11_max_multiplexingB\x12\n\x10_max_concurrencyB\x12\n\x10_min_concurrency\"\xf5\x03\n\x1aRegisterApplicationRequest\x12,\n\x0c\x65nvironments\x18\x01 \x03(\x0b\x32\x16.EnvironmentDefinition\x12\x42\n\x14machine_requirements\x18\x02 \x01(\x0b\x32\x1f.controller.MachineRequirementsH\x00\x88\x01\x01\x12#\n\x08\x66unction\x18\x03 \x01(\x0b\x32\x11.SerializedObject\x12*\n\nsetup_func\x18\x04 \x01(\x0b\x32\x11.SerializedObjectH\x01\x88\x01\x01\x12\x1d\n\x10\x61pplication_name\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x37\n\tauth_mode\x18\x06 \x01(\x0e\x32\x1f.controller.ApplicationAuthModeH\x03\x88\x01\x01\x12 \n\x0fmax_concurrency\x18\x07 \x01(\x05\x42\x02\x18\x01H\x04\x88\x01\x01\x12.\n\x08metadata\x18\x08 \x01(\x0b\x32\x17.google.protobuf.StructH\x05\x88\x01\x01\x42\x17\n\x15_machine_requirementsB\r\n\x0b_setup_funcB\x13\n\x11_application_nameB\x0c\n\n_auth_modeB\x12\n\x10_max_concurrencyB\x0b\n\t_metadata\"7\n\x1dRegisterApplicationResultType\x12\x16\n\x0e\x61pplication_id\x18\x01 \x01(\t\"z\n\x19RegisterApplicationResult\x12\x12\n\x04logs\x18\x01 \x03(\x0b\x32\x04.Log\x12>\n\x06result\x18\x02 \x01(\x0b\x32).controller.RegisterApplicationResultTypeH\x00\x88\x01\x01\x42\t\n\x07_result\"\xf4\x01\n\x18UpdateApplicationRequest\x12\x18\n\x10\x61pplication_name\x18\x01 \x01(\t\x12\x17\n\nkeep_alive\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x1d\n\x10max_multiplexing\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12\x1c\n\x0fmax_concurrency\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1c\n\x0fmin_concurrency\x18\x05 \x01(\x05H\x03\x88\x01\x01\x42\r\n\x0b_keep_aliveB\x13\n\x11_max_multiplexingB\x12\n\x10_max_concurrencyB\x12\n\x10_min_concurrency\"D\n\x17UpdateApplicationResult\x12)\n\nalias_info\x18\x01 \x01(\x0b\x32\x15.controller.AliasInfo\"\x19\n\x17ListApplicationsRequest\"\xa1\x01\n\x0f\x41pplicationInfo\x12\x16\n\x0e\x61pplication_id\x18\x01 \x01(\t\x12\x17\n\x0fmax_concurrency\x18\x02 \x01(\x05\x12\x18\n\x10max_multiplexing\x18\x03 \x01(\x05\x12\x12\n\nkeep_alive\x18\x04 \x01(\x05\x12\x16\n\x0e\x61\x63tive_runners\x18\x06 \x01(\x05\x12\x17\n\x0fmin_concurrency\x18\x07 \x01(\x05\"K\n\x16ListApplicationsResult\x12\x31\n\x0c\x61pplications\x18\x01 \x03(\x0b\x32\x1b.controller.ApplicationInfo\"2\n\x18\x44\x65leteApplicationRequest\x12\x16\n\x0e\x61pplication_id\x18\x01 \x01(\t\"\x19\n\x17\x44\x65leteApplicationResult\"f\n\x0fSetAliasRequest\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12\x10\n\x08revision\x18\x02 \x01(\t\x12\x32\n\tauth_mode\x18\x03 \x01(\x0e\x32\x1f.controller.ApplicationAuthMode\"\x10\n\x0eSetAliasResult\"#\n\x12\x44\x65leteAliasRequest\x12\r\n\x05\x61lias\x18\x01 \x01(\t\"%\n\x11\x44\x65leteAliasResult\x12\x10\n\x08revision\x18\x01 \x01(\t\"\x14\n\x12ListAliasesRequest\";\n\x11ListAliasesResult\x12&\n\x07\x61liases\x18\x01 \x03(\x0b\x32\x15.controller.AliasInfo\"\xd8\x01\n\tAliasInfo\x12\r\n\x05\x61lias\x18\x01 \x01(\t\x12\x10\n\x08revision\x18\x02 \x01(\t\x12\x32\n\tauth_mode\x18\x03 \x01(\x0e\x32\x1f.controller.ApplicationAuthMode\x12\x17\n\x0fmax_concurrency\x18\x04 \x01(\x05\x12\x18\n\x10max_multiplexing\x18\x05 \x01(\x05\x12\x12\n\nkeep_alive\x18\x06 \x01(\x05\x12\x16\n\x0e\x61\x63tive_runners\x18\x07 \x01(\x05\x12\x17\n\x0fmin_concurrency\x18\x08 \x01(\x05\">\n\x10SetSecretRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\x05value\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_value\"\x13\n\x11SetSecretResponse\"\x14\n\x12ListSecretsRequest\"^\n\x06Secret\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x35\n\x0c\x63reated_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x88\x01\x01\x42\x0f\n\r_created_time\":\n\x13ListSecretsResponse\x12#\n\x07secrets\x18\x01 \x03(\x0b\x32\x12.controller.Secret\"(\n\x17ListAliasRunnersRequest\x12\r\n\x05\x61lias\x18\x01 \x01(\t\"C\n\x18ListAliasRunnersResponse\x12\'\n\x07runners\x18\x01 \x03(\x0b\x32\x16.controller.RunnerInfo\"i\n\nRunnerInfo\x12\x11\n\trunner_id\x18\x01 \x01(\t\x12\x1a\n\x12in_flight_requests\x18\x02 \x01(\x05\x12\x1c\n\x14\x65xpiration_countdown\x18\x03 \x01(\x05\x12\x0e\n\x06uptime\x18\x04 \x01(\x02*:\n\x13\x41pplicationAuthMode\x12\x0b\n\x07PRIVATE\x10\x00\x12\n\n\x06PUBLIC\x10\x01\x12\n\n\x06SHARED\x10\x02\x32\x89\n\n\x11IsolateController\x12=\n\x03Run\x12\x15.controller.HostedRun\x1a\x1b.controller.HostedRunResult\"\x00\x30\x01\x12=\n\x03Map\x12\x15.controller.HostedMap\x1a\x1b.controller.HostedRunResult\"\x00\x30\x01\x12V\n\rCreateUserKey\x12 .controller.CreateUserKeyRequest\x1a!.controller.CreateUserKeyResponse\"\x00\x12S\n\x0cListUserKeys\x12\x1f.controller.ListUserKeysRequest\x1a .controller.ListUserKeysResponse\"\x00\x12V\n\rRevokeUserKey\x12 .controller.RevokeUserKeyRequest\x1a!.controller.RevokeUserKeyResponse\"\x00\x12h\n\x13RegisterApplication\x12&.controller.RegisterApplicationRequest\x1a%.controller.RegisterApplicationResult\"\x00\x30\x01\x12`\n\x11UpdateApplication\x12$.controller.UpdateApplicationRequest\x1a#.controller.UpdateApplicationResult\"\x00\x12]\n\x10ListApplications\x12#.controller.ListApplicationsRequest\x1a\".controller.ListApplicationsResult\"\x00\x12`\n\x11\x44\x65leteApplication\x12$.controller.DeleteApplicationRequest\x1a#.controller.DeleteApplicationResult\"\x00\x12\x45\n\x08SetAlias\x12\x1b.controller.SetAliasRequest\x1a\x1a.controller.SetAliasResult\"\x00\x12N\n\x0b\x44\x65leteAlias\x12\x1e.controller.DeleteAliasRequest\x1a\x1d.controller.DeleteAliasResult\"\x00\x12N\n\x0bListAliases\x12\x1e.controller.ListAliasesRequest\x1a\x1d.controller.ListAliasesResult\"\x00\x12J\n\tSetSecret\x12\x1c.controller.SetSecretRequest\x1a\x1d.controller.SetSecretResponse\"\x00\x12P\n\x0bListSecrets\x12\x1e.controller.ListSecretsRequest\x1a\x1f.controller.ListSecretsResponse\"\x00\x12_\n\x10ListAliasRunners\x12#.controller.ListAliasRunnersRequest\x1a$.controller.ListAliasRunnersResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "controller_pb2", _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'controller_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-    DESCRIPTOR._options = None
-    _REGISTERAPPLICATIONREQUEST.fields_by_name["max_concurrency"]._options = None
-    _REGISTERAPPLICATIONREQUEST.fields_by_name[
-        "max_concurrency"
-    ]._serialized_options = b"\030\001"
-    _globals["_APPLICATIONAUTHMODE"]._serialized_start = 3868
-    _globals["_APPLICATIONAUTHMODE"]._serialized_end = 3926
-    _globals["_HOSTEDMAP"]._serialized_start = 156
-    _globals["_HOSTEDMAP"]._serialized_end = 378
-    _globals["_HOSTEDRUN"]._serialized_start = 381
-    _globals["_HOSTEDRUN"]._serialized_end = 627
-    _globals["_CREATEUSERKEYREQUEST"]._serialized_start = 630
-    _globals["_CREATEUSERKEYREQUEST"]._serialized_end = 766
-    _globals["_CREATEUSERKEYREQUEST_SCOPE"]._serialized_start = 729
-    _globals["_CREATEUSERKEYREQUEST_SCOPE"]._serialized_end = 756
-    _globals["_CREATEUSERKEYRESPONSE"]._serialized_start = 768
-    _globals["_CREATEUSERKEYRESPONSE"]._serialized_end = 827
-    _globals["_LISTUSERKEYSREQUEST"]._serialized_start = 829
-    _globals["_LISTUSERKEYSREQUEST"]._serialized_end = 850
-    _globals["_LISTUSERKEYSRESPONSE"]._serialized_start = 852
-    _globals["_LISTUSERKEYSRESPONSE"]._serialized_end = 918
-    _globals["_REVOKEUSERKEYREQUEST"]._serialized_start = 920
-    _globals["_REVOKEUSERKEYREQUEST"]._serialized_end = 958
-    _globals["_REVOKEUSERKEYRESPONSE"]._serialized_start = 960
-    _globals["_REVOKEUSERKEYRESPONSE"]._serialized_end = 983
-    _globals["_USERKEYINFO"]._serialized_start = 986
-    _globals["_USERKEYINFO"]._serialized_end = 1133
-    _globals["_HOSTEDRUNRESULT"]._serialized_start = 1136
-    _globals["_HOSTEDRUNRESULT"]._serialized_end = 1313
-    _globals["_HOSTEDRUNSTATUS"]._serialized_start = 1316
-    _globals["_HOSTEDRUNSTATUS"]._serialized_end = 1444
-    _globals["_HOSTEDRUNSTATUS_STATE"]._serialized_start = 1385
-    _globals["_HOSTEDRUNSTATUS_STATE"]._serialized_end = 1444
-    _globals["_MACHINEREQUIREMENTS"]._serialized_start = 1447
-    _globals["_MACHINEREQUIREMENTS"]._serialized_end = 1883
-    _globals["_REGISTERAPPLICATIONREQUEST"]._serialized_start = 1886
-    _globals["_REGISTERAPPLICATIONREQUEST"]._serialized_end = 2387
-    _globals["_REGISTERAPPLICATIONRESULTTYPE"]._serialized_start = 2389
-    _globals["_REGISTERAPPLICATIONRESULTTYPE"]._serialized_end = 2444
-    _globals["_REGISTERAPPLICATIONRESULT"]._serialized_start = 2446
-    _globals["_REGISTERAPPLICATIONRESULT"]._serialized_end = 2568
-    _globals["_UPDATEAPPLICATIONREQUEST"]._serialized_start = 2571
-    _globals["_UPDATEAPPLICATIONREQUEST"]._serialized_end = 2815
-    _globals["_UPDATEAPPLICATIONRESULT"]._serialized_start = 2817
-    _globals["_UPDATEAPPLICATIONRESULT"]._serialized_end = 2885
-    _globals["_SETALIASREQUEST"]._serialized_start = 2887
-    _globals["_SETALIASREQUEST"]._serialized_end = 2989
-    _globals["_SETALIASRESULT"]._serialized_start = 2991
-    _globals["_SETALIASRESULT"]._serialized_end = 3007
-    _globals["_DELETEALIASREQUEST"]._serialized_start = 3009
-    _globals["_DELETEALIASREQUEST"]._serialized_end = 3044
-    _globals["_DELETEALIASRESULT"]._serialized_start = 3046
-    _globals["_DELETEALIASRESULT"]._serialized_end = 3083
-    _globals["_LISTALIASESREQUEST"]._serialized_start = 3085
-    _globals["_LISTALIASESREQUEST"]._serialized_end = 3105
-    _globals["_LISTALIASESRESULT"]._serialized_start = 3107
-    _globals["_LISTALIASESRESULT"]._serialized_end = 3166
-    _globals["_ALIASINFO"]._serialized_start = 3169
-    _globals["_ALIASINFO"]._serialized_end = 3385
-    _globals["_SETSECRETREQUEST"]._serialized_start = 3387
-    _globals["_SETSECRETREQUEST"]._serialized_end = 3449
-    _globals["_SETSECRETRESPONSE"]._serialized_start = 3451
-    _globals["_SETSECRETRESPONSE"]._serialized_end = 3470
-    _globals["_LISTSECRETSREQUEST"]._serialized_start = 3472
-    _globals["_LISTSECRETSREQUEST"]._serialized_end = 3492
-    _globals["_SECRET"]._serialized_start = 3494
-    _globals["_SECRET"]._serialized_end = 3588
-    _globals["_LISTSECRETSRESPONSE"]._serialized_start = 3590
-    _globals["_LISTSECRETSRESPONSE"]._serialized_end = 3648
-    _globals["_LISTALIASRUNNERSREQUEST"]._serialized_start = 3650
-    _globals["_LISTALIASRUNNERSREQUEST"]._serialized_end = 3690
-    _globals["_LISTALIASRUNNERSRESPONSE"]._serialized_start = 3692
-    _globals["_LISTALIASRUNNERSRESPONSE"]._serialized_end = 3759
-    _globals["_RUNNERINFO"]._serialized_start = 3761
-    _globals["_RUNNERINFO"]._serialized_end = 3866
-    _globals["_ISOLATECONTROLLER"]._serialized_start = 3929
-    _globals["_ISOLATECONTROLLER"]._serialized_end = 5025
+  DESCRIPTOR._options = None
+  _globals['_REGISTERAPPLICATIONREQUEST'].fields_by_name['max_concurrency']._options = None
+  _globals['_REGISTERAPPLICATIONREQUEST'].fields_by_name['max_concurrency']._serialized_options = b'\030\001'
+  _globals['_APPLICATIONAUTHMODE']._serialized_start=4215
+  _globals['_APPLICATIONAUTHMODE']._serialized_end=4273
+  _globals['_HOSTEDMAP']._serialized_start=156
+  _globals['_HOSTEDMAP']._serialized_end=378
+  _globals['_HOSTEDRUN']._serialized_start=381
+  _globals['_HOSTEDRUN']._serialized_end=627
+  _globals['_CREATEUSERKEYREQUEST']._serialized_start=630
+  _globals['_CREATEUSERKEYREQUEST']._serialized_end=766
+  _globals['_CREATEUSERKEYREQUEST_SCOPE']._serialized_start=729
+  _globals['_CREATEUSERKEYREQUEST_SCOPE']._serialized_end=756
+  _globals['_CREATEUSERKEYRESPONSE']._serialized_start=768
+  _globals['_CREATEUSERKEYRESPONSE']._serialized_end=827
+  _globals['_LISTUSERKEYSREQUEST']._serialized_start=829
+  _globals['_LISTUSERKEYSREQUEST']._serialized_end=850
+  _globals['_LISTUSERKEYSRESPONSE']._serialized_start=852
+  _globals['_LISTUSERKEYSRESPONSE']._serialized_end=918
+  _globals['_REVOKEUSERKEYREQUEST']._serialized_start=920
+  _globals['_REVOKEUSERKEYREQUEST']._serialized_end=958
+  _globals['_REVOKEUSERKEYRESPONSE']._serialized_start=960
+  _globals['_REVOKEUSERKEYRESPONSE']._serialized_end=983
+  _globals['_USERKEYINFO']._serialized_start=986
+  _globals['_USERKEYINFO']._serialized_end=1133
+  _globals['_HOSTEDRUNRESULT']._serialized_start=1136
+  _globals['_HOSTEDRUNRESULT']._serialized_end=1313
+  _globals['_HOSTEDRUNSTATUS']._serialized_start=1316
+  _globals['_HOSTEDRUNSTATUS']._serialized_end=1444
+  _globals['_HOSTEDRUNSTATUS_STATE']._serialized_start=1385
+  _globals['_HOSTEDRUNSTATUS_STATE']._serialized_end=1444
+  _globals['_MACHINEREQUIREMENTS']._serialized_start=1447
+  _globals['_MACHINEREQUIREMENTS']._serialized_end=1883
+  _globals['_REGISTERAPPLICATIONREQUEST']._serialized_start=1886
+  _globals['_REGISTERAPPLICATIONREQUEST']._serialized_end=2387
+  _globals['_REGISTERAPPLICATIONRESULTTYPE']._serialized_start=2389
+  _globals['_REGISTERAPPLICATIONRESULTTYPE']._serialized_end=2444
+  _globals['_REGISTERAPPLICATIONRESULT']._serialized_start=2446
+  _globals['_REGISTERAPPLICATIONRESULT']._serialized_end=2568
+  _globals['_UPDATEAPPLICATIONREQUEST']._serialized_start=2571
+  _globals['_UPDATEAPPLICATIONREQUEST']._serialized_end=2815
+  _globals['_UPDATEAPPLICATIONRESULT']._serialized_start=2817
+  _globals['_UPDATEAPPLICATIONRESULT']._serialized_end=2885
+  _globals['_LISTAPPLICATIONSREQUEST']._serialized_start=2887
+  _globals['_LISTAPPLICATIONSREQUEST']._serialized_end=2912
+  _globals['_APPLICATIONINFO']._serialized_start=2915
+  _globals['_APPLICATIONINFO']._serialized_end=3076
+  _globals['_LISTAPPLICATIONSRESULT']._serialized_start=3078
+  _globals['_LISTAPPLICATIONSRESULT']._serialized_end=3153
+  _globals['_DELETEAPPLICATIONREQUEST']._serialized_start=3155
+  _globals['_DELETEAPPLICATIONREQUEST']._serialized_end=3205
+  _globals['_DELETEAPPLICATIONRESULT']._serialized_start=3207
+  _globals['_DELETEAPPLICATIONRESULT']._serialized_end=3232
+  _globals['_SETALIASREQUEST']._serialized_start=3234
+  _globals['_SETALIASREQUEST']._serialized_end=3336
+  _globals['_SETALIASRESULT']._serialized_start=3338
+  _globals['_SETALIASRESULT']._serialized_end=3354
+  _globals['_DELETEALIASREQUEST']._serialized_start=3356
+  _globals['_DELETEALIASREQUEST']._serialized_end=3391
+  _globals['_DELETEALIASRESULT']._serialized_start=3393
+  _globals['_DELETEALIASRESULT']._serialized_end=3430
+  _globals['_LISTALIASESREQUEST']._serialized_start=3432
+  _globals['_LISTALIASESREQUEST']._serialized_end=3452
+  _globals['_LISTALIASESRESULT']._serialized_start=3454
+  _globals['_LISTALIASESRESULT']._serialized_end=3513
+  _globals['_ALIASINFO']._serialized_start=3516
+  _globals['_ALIASINFO']._serialized_end=3732
+  _globals['_SETSECRETREQUEST']._serialized_start=3734
+  _globals['_SETSECRETREQUEST']._serialized_end=3796
+  _globals['_SETSECRETRESPONSE']._serialized_start=3798
+  _globals['_SETSECRETRESPONSE']._serialized_end=3817
+  _globals['_LISTSECRETSREQUEST']._serialized_start=3819
+  _globals['_LISTSECRETSREQUEST']._serialized_end=3839
+  _globals['_SECRET']._serialized_start=3841
+  _globals['_SECRET']._serialized_end=3935
+  _globals['_LISTSECRETSRESPONSE']._serialized_start=3937
+  _globals['_LISTSECRETSRESPONSE']._serialized_end=3995
+  _globals['_LISTALIASRUNNERSREQUEST']._serialized_start=3997
+  _globals['_LISTALIASRUNNERSREQUEST']._serialized_end=4037
+  _globals['_LISTALIASRUNNERSRESPONSE']._serialized_start=4039
+  _globals['_LISTALIASRUNNERSRESPONSE']._serialized_end=4106
+  _globals['_RUNNERINFO']._serialized_start=4108
+  _globals['_RUNNERINFO']._serialized_end=4213
+  _globals['_ISOLATECONTROLLER']._serialized_start=4276
+  _globals['_ISOLATECONTROLLER']._serialized_end=5565
 # @@protoc_insertion_point(module_scope)
```

### Comparing `isolate_proto-0.3.4/src/isolate_proto/controller_pb2_grpc.py` & `isolate_proto-0.4.0/src/isolate_proto/controller_pb2_grpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,611 +11,534 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Run = channel.unary_stream(
-            "/controller.IsolateController/Run",
-            request_serializer=controller__pb2.HostedRun.SerializeToString,
-            response_deserializer=controller__pb2.HostedRunResult.FromString,
-        )
+                '/controller.IsolateController/Run',
+                request_serializer=controller__pb2.HostedRun.SerializeToString,
+                response_deserializer=controller__pb2.HostedRunResult.FromString,
+                )
         self.Map = channel.unary_stream(
-            "/controller.IsolateController/Map",
-            request_serializer=controller__pb2.HostedMap.SerializeToString,
-            response_deserializer=controller__pb2.HostedRunResult.FromString,
-        )
+                '/controller.IsolateController/Map',
+                request_serializer=controller__pb2.HostedMap.SerializeToString,
+                response_deserializer=controller__pb2.HostedRunResult.FromString,
+                )
         self.CreateUserKey = channel.unary_unary(
-            "/controller.IsolateController/CreateUserKey",
-            request_serializer=controller__pb2.CreateUserKeyRequest.SerializeToString,
-            response_deserializer=controller__pb2.CreateUserKeyResponse.FromString,
-        )
+                '/controller.IsolateController/CreateUserKey',
+                request_serializer=controller__pb2.CreateUserKeyRequest.SerializeToString,
+                response_deserializer=controller__pb2.CreateUserKeyResponse.FromString,
+                )
         self.ListUserKeys = channel.unary_unary(
-            "/controller.IsolateController/ListUserKeys",
-            request_serializer=controller__pb2.ListUserKeysRequest.SerializeToString,
-            response_deserializer=controller__pb2.ListUserKeysResponse.FromString,
-        )
+                '/controller.IsolateController/ListUserKeys',
+                request_serializer=controller__pb2.ListUserKeysRequest.SerializeToString,
+                response_deserializer=controller__pb2.ListUserKeysResponse.FromString,
+                )
         self.RevokeUserKey = channel.unary_unary(
-            "/controller.IsolateController/RevokeUserKey",
-            request_serializer=controller__pb2.RevokeUserKeyRequest.SerializeToString,
-            response_deserializer=controller__pb2.RevokeUserKeyResponse.FromString,
-        )
+                '/controller.IsolateController/RevokeUserKey',
+                request_serializer=controller__pb2.RevokeUserKeyRequest.SerializeToString,
+                response_deserializer=controller__pb2.RevokeUserKeyResponse.FromString,
+                )
         self.RegisterApplication = channel.unary_stream(
-            "/controller.IsolateController/RegisterApplication",
-            request_serializer=controller__pb2.RegisterApplicationRequest.SerializeToString,
-            response_deserializer=controller__pb2.RegisterApplicationResult.FromString,
-        )
+                '/controller.IsolateController/RegisterApplication',
+                request_serializer=controller__pb2.RegisterApplicationRequest.SerializeToString,
+                response_deserializer=controller__pb2.RegisterApplicationResult.FromString,
+                )
         self.UpdateApplication = channel.unary_unary(
-            "/controller.IsolateController/UpdateApplication",
-            request_serializer=controller__pb2.UpdateApplicationRequest.SerializeToString,
-            response_deserializer=controller__pb2.UpdateApplicationResult.FromString,
-        )
+                '/controller.IsolateController/UpdateApplication',
+                request_serializer=controller__pb2.UpdateApplicationRequest.SerializeToString,
+                response_deserializer=controller__pb2.UpdateApplicationResult.FromString,
+                )
+        self.ListApplications = channel.unary_unary(
+                '/controller.IsolateController/ListApplications',
+                request_serializer=controller__pb2.ListApplicationsRequest.SerializeToString,
+                response_deserializer=controller__pb2.ListApplicationsResult.FromString,
+                )
+        self.DeleteApplication = channel.unary_unary(
+                '/controller.IsolateController/DeleteApplication',
+                request_serializer=controller__pb2.DeleteApplicationRequest.SerializeToString,
+                response_deserializer=controller__pb2.DeleteApplicationResult.FromString,
+                )
         self.SetAlias = channel.unary_unary(
-            "/controller.IsolateController/SetAlias",
-            request_serializer=controller__pb2.SetAliasRequest.SerializeToString,
-            response_deserializer=controller__pb2.SetAliasResult.FromString,
-        )
+                '/controller.IsolateController/SetAlias',
+                request_serializer=controller__pb2.SetAliasRequest.SerializeToString,
+                response_deserializer=controller__pb2.SetAliasResult.FromString,
+                )
         self.DeleteAlias = channel.unary_unary(
-            "/controller.IsolateController/DeleteAlias",
-            request_serializer=controller__pb2.DeleteAliasRequest.SerializeToString,
-            response_deserializer=controller__pb2.DeleteAliasResult.FromString,
-        )
+                '/controller.IsolateController/DeleteAlias',
+                request_serializer=controller__pb2.DeleteAliasRequest.SerializeToString,
+                response_deserializer=controller__pb2.DeleteAliasResult.FromString,
+                )
         self.ListAliases = channel.unary_unary(
-            "/controller.IsolateController/ListAliases",
-            request_serializer=controller__pb2.ListAliasesRequest.SerializeToString,
-            response_deserializer=controller__pb2.ListAliasesResult.FromString,
-        )
+                '/controller.IsolateController/ListAliases',
+                request_serializer=controller__pb2.ListAliasesRequest.SerializeToString,
+                response_deserializer=controller__pb2.ListAliasesResult.FromString,
+                )
         self.SetSecret = channel.unary_unary(
-            "/controller.IsolateController/SetSecret",
-            request_serializer=controller__pb2.SetSecretRequest.SerializeToString,
-            response_deserializer=controller__pb2.SetSecretResponse.FromString,
-        )
+                '/controller.IsolateController/SetSecret',
+                request_serializer=controller__pb2.SetSecretRequest.SerializeToString,
+                response_deserializer=controller__pb2.SetSecretResponse.FromString,
+                )
         self.ListSecrets = channel.unary_unary(
-            "/controller.IsolateController/ListSecrets",
-            request_serializer=controller__pb2.ListSecretsRequest.SerializeToString,
-            response_deserializer=controller__pb2.ListSecretsResponse.FromString,
-        )
+                '/controller.IsolateController/ListSecrets',
+                request_serializer=controller__pb2.ListSecretsRequest.SerializeToString,
+                response_deserializer=controller__pb2.ListSecretsResponse.FromString,
+                )
         self.ListAliasRunners = channel.unary_unary(
-            "/controller.IsolateController/ListAliasRunners",
-            request_serializer=controller__pb2.ListAliasRunnersRequest.SerializeToString,
-            response_deserializer=controller__pb2.ListAliasRunnersResponse.FromString,
-        )
+                '/controller.IsolateController/ListAliasRunners',
+                request_serializer=controller__pb2.ListAliasRunnersRequest.SerializeToString,
+                response_deserializer=controller__pb2.ListAliasRunnersResponse.FromString,
+                )
 
 
 class IsolateControllerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Run(self, request, context):
         """Run the given function on the specified environment. Streams logs
         and the result originating from that function.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def Map(self, request, context):
-        """Run the given function in parallel with the given inputs"""
+        """Run the given function in parallel with the given inputs
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def CreateUserKey(self, request, context):
-        """Creates an authentication key for a user"""
+        """Creates an authentication key for a user
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def ListUserKeys(self, request, context):
-        """Lists the user's authentication keys"""
+        """Lists the user's authentication keys
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def RevokeUserKey(self, request, context):
-        """Revokes an authentication key for a user"""
+        """Revokes an authentication key for a user
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def RegisterApplication(self, request, context):
-        """Register a funtion"""
+        """Register a funtion
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def UpdateApplication(self, request, context):
-        """Update configuration of an existing application."""
+        """Update configuration of an existing application.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ListApplications(self, request, context):
+        """List functions
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteApplication(self, request, context):
+        """Delete a function
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def SetAlias(self, request, context):
-        """Set alias to point to an existing application."""
+        """Set alias to point to an existing application.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def DeleteAlias(self, request, context):
-        """Delete an alias."""
+        """Delete an alias.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def ListAliases(self, request, context):
-        """List aliased registered functions"""
+        """List aliased registered functions
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def SetSecret(self, request, context):
-        """Sets a user secret."""
+        """Sets a user secret.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def ListSecrets(self, request, context):
-        """Lists all secrets"""
+        """Lists all secrets
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def ListAliasRunners(self, request, context):
-        """List alias runners in detail"""
+        """List alias runners in detail
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_IsolateControllerServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "Run": grpc.unary_stream_rpc_method_handler(
-            servicer.Run,
-            request_deserializer=controller__pb2.HostedRun.FromString,
-            response_serializer=controller__pb2.HostedRunResult.SerializeToString,
-        ),
-        "Map": grpc.unary_stream_rpc_method_handler(
-            servicer.Map,
-            request_deserializer=controller__pb2.HostedMap.FromString,
-            response_serializer=controller__pb2.HostedRunResult.SerializeToString,
-        ),
-        "CreateUserKey": grpc.unary_unary_rpc_method_handler(
-            servicer.CreateUserKey,
-            request_deserializer=controller__pb2.CreateUserKeyRequest.FromString,
-            response_serializer=controller__pb2.CreateUserKeyResponse.SerializeToString,
-        ),
-        "ListUserKeys": grpc.unary_unary_rpc_method_handler(
-            servicer.ListUserKeys,
-            request_deserializer=controller__pb2.ListUserKeysRequest.FromString,
-            response_serializer=controller__pb2.ListUserKeysResponse.SerializeToString,
-        ),
-        "RevokeUserKey": grpc.unary_unary_rpc_method_handler(
-            servicer.RevokeUserKey,
-            request_deserializer=controller__pb2.RevokeUserKeyRequest.FromString,
-            response_serializer=controller__pb2.RevokeUserKeyResponse.SerializeToString,
-        ),
-        "RegisterApplication": grpc.unary_stream_rpc_method_handler(
-            servicer.RegisterApplication,
-            request_deserializer=controller__pb2.RegisterApplicationRequest.FromString,
-            response_serializer=controller__pb2.RegisterApplicationResult.SerializeToString,
-        ),
-        "UpdateApplication": grpc.unary_unary_rpc_method_handler(
-            servicer.UpdateApplication,
-            request_deserializer=controller__pb2.UpdateApplicationRequest.FromString,
-            response_serializer=controller__pb2.UpdateApplicationResult.SerializeToString,
-        ),
-        "SetAlias": grpc.unary_unary_rpc_method_handler(
-            servicer.SetAlias,
-            request_deserializer=controller__pb2.SetAliasRequest.FromString,
-            response_serializer=controller__pb2.SetAliasResult.SerializeToString,
-        ),
-        "DeleteAlias": grpc.unary_unary_rpc_method_handler(
-            servicer.DeleteAlias,
-            request_deserializer=controller__pb2.DeleteAliasRequest.FromString,
-            response_serializer=controller__pb2.DeleteAliasResult.SerializeToString,
-        ),
-        "ListAliases": grpc.unary_unary_rpc_method_handler(
-            servicer.ListAliases,
-            request_deserializer=controller__pb2.ListAliasesRequest.FromString,
-            response_serializer=controller__pb2.ListAliasesResult.SerializeToString,
-        ),
-        "SetSecret": grpc.unary_unary_rpc_method_handler(
-            servicer.SetSecret,
-            request_deserializer=controller__pb2.SetSecretRequest.FromString,
-            response_serializer=controller__pb2.SetSecretResponse.SerializeToString,
-        ),
-        "ListSecrets": grpc.unary_unary_rpc_method_handler(
-            servicer.ListSecrets,
-            request_deserializer=controller__pb2.ListSecretsRequest.FromString,
-            response_serializer=controller__pb2.ListSecretsResponse.SerializeToString,
-        ),
-        "ListAliasRunners": grpc.unary_unary_rpc_method_handler(
-            servicer.ListAliasRunners,
-            request_deserializer=controller__pb2.ListAliasRunnersRequest.FromString,
-            response_serializer=controller__pb2.ListAliasRunnersResponse.SerializeToString,
-        ),
+            'Run': grpc.unary_stream_rpc_method_handler(
+                    servicer.Run,
+                    request_deserializer=controller__pb2.HostedRun.FromString,
+                    response_serializer=controller__pb2.HostedRunResult.SerializeToString,
+            ),
+            'Map': grpc.unary_stream_rpc_method_handler(
+                    servicer.Map,
+                    request_deserializer=controller__pb2.HostedMap.FromString,
+                    response_serializer=controller__pb2.HostedRunResult.SerializeToString,
+            ),
+            'CreateUserKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateUserKey,
+                    request_deserializer=controller__pb2.CreateUserKeyRequest.FromString,
+                    response_serializer=controller__pb2.CreateUserKeyResponse.SerializeToString,
+            ),
+            'ListUserKeys': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListUserKeys,
+                    request_deserializer=controller__pb2.ListUserKeysRequest.FromString,
+                    response_serializer=controller__pb2.ListUserKeysResponse.SerializeToString,
+            ),
+            'RevokeUserKey': grpc.unary_unary_rpc_method_handler(
+                    servicer.RevokeUserKey,
+                    request_deserializer=controller__pb2.RevokeUserKeyRequest.FromString,
+                    response_serializer=controller__pb2.RevokeUserKeyResponse.SerializeToString,
+            ),
+            'RegisterApplication': grpc.unary_stream_rpc_method_handler(
+                    servicer.RegisterApplication,
+                    request_deserializer=controller__pb2.RegisterApplicationRequest.FromString,
+                    response_serializer=controller__pb2.RegisterApplicationResult.SerializeToString,
+            ),
+            'UpdateApplication': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateApplication,
+                    request_deserializer=controller__pb2.UpdateApplicationRequest.FromString,
+                    response_serializer=controller__pb2.UpdateApplicationResult.SerializeToString,
+            ),
+            'ListApplications': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListApplications,
+                    request_deserializer=controller__pb2.ListApplicationsRequest.FromString,
+                    response_serializer=controller__pb2.ListApplicationsResult.SerializeToString,
+            ),
+            'DeleteApplication': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteApplication,
+                    request_deserializer=controller__pb2.DeleteApplicationRequest.FromString,
+                    response_serializer=controller__pb2.DeleteApplicationResult.SerializeToString,
+            ),
+            'SetAlias': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetAlias,
+                    request_deserializer=controller__pb2.SetAliasRequest.FromString,
+                    response_serializer=controller__pb2.SetAliasResult.SerializeToString,
+            ),
+            'DeleteAlias': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteAlias,
+                    request_deserializer=controller__pb2.DeleteAliasRequest.FromString,
+                    response_serializer=controller__pb2.DeleteAliasResult.SerializeToString,
+            ),
+            'ListAliases': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListAliases,
+                    request_deserializer=controller__pb2.ListAliasesRequest.FromString,
+                    response_serializer=controller__pb2.ListAliasesResult.SerializeToString,
+            ),
+            'SetSecret': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetSecret,
+                    request_deserializer=controller__pb2.SetSecretRequest.FromString,
+                    response_serializer=controller__pb2.SetSecretResponse.SerializeToString,
+            ),
+            'ListSecrets': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListSecrets,
+                    request_deserializer=controller__pb2.ListSecretsRequest.FromString,
+                    response_serializer=controller__pb2.ListSecretsResponse.SerializeToString,
+            ),
+            'ListAliasRunners': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListAliasRunners,
+                    request_deserializer=controller__pb2.ListAliasRunnersRequest.FromString,
+                    response_serializer=controller__pb2.ListAliasRunnersResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "controller.IsolateController", rpc_method_handlers
-    )
+            'controller.IsolateController', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class IsolateController(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def Run(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_stream(
-            request,
+    def Run(request,
             target,
-            "/controller.IsolateController/Run",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/controller.IsolateController/Run',
             controller__pb2.HostedRun.SerializeToString,
             controller__pb2.HostedRunResult.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def Map(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_stream(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def Map(request,
             target,
-            "/controller.IsolateController/Map",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/controller.IsolateController/Map',
             controller__pb2.HostedMap.SerializeToString,
             controller__pb2.HostedRunResult.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def CreateUserKey(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CreateUserKey(request,
             target,
-            "/controller.IsolateController/CreateUserKey",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/CreateUserKey',
             controller__pb2.CreateUserKeyRequest.SerializeToString,
             controller__pb2.CreateUserKeyResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def ListUserKeys(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListUserKeys(request,
             target,
-            "/controller.IsolateController/ListUserKeys",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/ListUserKeys',
             controller__pb2.ListUserKeysRequest.SerializeToString,
             controller__pb2.ListUserKeysResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def RevokeUserKey(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def RevokeUserKey(request,
             target,
-            "/controller.IsolateController/RevokeUserKey",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/RevokeUserKey',
             controller__pb2.RevokeUserKeyRequest.SerializeToString,
             controller__pb2.RevokeUserKeyResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def RegisterApplication(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_stream(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def RegisterApplication(request,
             target,
-            "/controller.IsolateController/RegisterApplication",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/controller.IsolateController/RegisterApplication',
             controller__pb2.RegisterApplicationRequest.SerializeToString,
             controller__pb2.RegisterApplicationResult.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def UpdateApplication(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UpdateApplication(request,
             target,
-            "/controller.IsolateController/UpdateApplication",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/UpdateApplication',
             controller__pb2.UpdateApplicationRequest.SerializeToString,
             controller__pb2.UpdateApplicationResult.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def SetAlias(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListApplications(request,
             target,
-            "/controller.IsolateController/SetAlias",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/ListApplications',
+            controller__pb2.ListApplicationsRequest.SerializeToString,
+            controller__pb2.ListApplicationsResult.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteApplication(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/DeleteApplication',
+            controller__pb2.DeleteApplicationRequest.SerializeToString,
+            controller__pb2.DeleteApplicationResult.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetAlias(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/SetAlias',
             controller__pb2.SetAliasRequest.SerializeToString,
             controller__pb2.SetAliasResult.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def DeleteAlias(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteAlias(request,
             target,
-            "/controller.IsolateController/DeleteAlias",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/DeleteAlias',
             controller__pb2.DeleteAliasRequest.SerializeToString,
             controller__pb2.DeleteAliasResult.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def ListAliases(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListAliases(request,
             target,
-            "/controller.IsolateController/ListAliases",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/ListAliases',
             controller__pb2.ListAliasesRequest.SerializeToString,
             controller__pb2.ListAliasesResult.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def SetSecret(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetSecret(request,
             target,
-            "/controller.IsolateController/SetSecret",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/SetSecret',
             controller__pb2.SetSecretRequest.SerializeToString,
             controller__pb2.SetSecretResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def ListSecrets(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListSecrets(request,
             target,
-            "/controller.IsolateController/ListSecrets",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/ListSecrets',
             controller__pb2.ListSecretsRequest.SerializeToString,
             controller__pb2.ListSecretsResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
-
-    @staticmethod
-    def ListAliasRunners(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListAliasRunners(request,
             target,
-            "/controller.IsolateController/ListAliasRunners",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/controller.IsolateController/ListAliasRunners',
             controller__pb2.ListAliasRunnersRequest.SerializeToString,
             controller__pb2.ListAliasRunnersResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `isolate_proto-0.3.4/src/isolate_proto/health/health_pb2.py` & `isolate_proto-0.4.0/src/isolate_proto/health/health_pb2.py`

 * *Files identical despite different names*

### Comparing `isolate_proto-0.3.4/src/isolate_proto/health/health_pb2.pyi` & `isolate_proto-0.4.0/src/isolate_proto/health/health_pb2.pyi`

 * *Files identical despite different names*

### Comparing `isolate_proto-0.3.4/src/isolate_proto/health/health_pb2_grpc.py` & `isolate_proto-0.4.0/src/isolate_proto/health/health_pb2_grpc.py`

 * *Files identical despite different names*
