# Comparing `tmp/gink-0.20240601.1717210459.tar.gz` & `tmp/gink-0.20240602.1717352499.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240601.1717210459.tar", last modified: Sat Jun  1 02:54:22 2024, max compression
+gzip compressed data, was "gink-0.20240602.1717352499.tar", last modified: Sun Jun  2 18:21:46 2024, max compression
```

## Comparing `gink-0.20240601.1717210459.tar` & `gink-0.20240602.1717352499.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:54:22.493519 gink-0.20240601.1717210459/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-06-01 02:54:22.489519 gink-0.20240601.1717210459/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:54:22.473519 gink-0.20240601.1717210459/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7400 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/braid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:54:22.477519 gink-0.20240601.1717210459/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/header_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:54:22.485520 gink-0.20240601.1717210459/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/braid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/braid_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/bundle_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9124 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    57479 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/looping.py
--rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/relay.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/wsgi_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/impl/wsgi_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:54:22.489519 gink-0.20240601.1717210459/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_braid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-06-01 02:54:16.000000 gink-0.20240601.1717210459/gink/tests/test_wsgi_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:54:22.489519 gink-0.20240601.1717210459/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-06-01 02:54:22.000000 gink-0.20240601.1717210459/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-06-01 02:54:22.000000 gink-0.20240601.1717210459/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 02:54:22.000000 gink-0.20240601.1717210459/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-01 02:54:22.000000 gink-0.20240601.1717210459/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 02:54:22.000000 gink-0.20240601.1717210459/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 02:54:22.493519 gink-0.20240601.1717210459/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-06-01 02:54:19.000000 gink-0.20240601.1717210459/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:21:46.112299 gink-0.20240602.1717352499/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-06-02 18:21:46.112299 gink-0.20240602.1717352499/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:21:46.096299 gink-0.20240602.1717352499/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7392 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/braid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:21:46.100299 gink-0.20240602.1717352499/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/header_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:21:46.108299 gink-0.20240602.1717352499/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10233 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/braid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/braid_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/bundle_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9124 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57479 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/looping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/wsgi_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/impl/wsgi_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:21:46.112299 gink-0.20240602.1717352499/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_braid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10500 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-06-02 18:21:31.000000 gink-0.20240602.1717352499/gink/tests/test_wsgi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:21:46.112299 gink-0.20240602.1717352499/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-06-02 18:21:46.000000 gink-0.20240602.1717352499/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-06-02 18:21:46.000000 gink-0.20240602.1717352499/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:21:46.000000 gink-0.20240602.1717352499/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-02 18:21:46.000000 gink-0.20240602.1717352499/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-02 18:21:46.000000 gink-0.20240602.1717352499/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:21:46.112299 gink-0.20240602.1717352499/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-06-02 18:21:39.000000 gink-0.20240602.1717352499/setup.py
```

### Comparing `gink-0.20240601.1717210459/LICENSE` & `gink-0.20240602.1717352499/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/PKG-INFO` & `gink-0.20240602.1717352499/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240601.1717210459
+Version: 0.20240602.1717352499
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240601.1717210459/README.md` & `gink-0.20240602.1717352499/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/__init__.py` & `gink-0.20240602.1717352499/gink/__init__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/__main__.py` & `gink-0.20240602.1717352499/gink/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     ip_addr, port = parse_listen_on(args.wsgi_listen_on, "*", "8081")
     wsgi_listener = WsgiListener(app, ip_addr=ip_addr, port=int(port))
 
 auth_func = make_auth_func(args.auth_token) if args.auth_token else None
 
 if args.listen_on:
     ip_addr, port = parse_listen_on(args.listen_on, "*", "8080")
-    database.start_listening(ip_addr=ip_addr, port=port, auth_func=auth_func)
+    database.start_listening(addr=ip_addr, port=port, auth=auth_func)
 
 for target in (args.connect_to or []):
     auth_data = f"Token {args.auth_token}" if args.auth_token else None
     database.connect_to(target, auth_data=auth_data)
 
 if args.interactive:
     interactive = True
```

### Comparing `gink-0.20240601.1717210459/gink/braid.py` & `gink-0.20240602.1717352499/gink/braid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/behavior_pb2.py` & `gink-0.20240602.1717352499/gink/builders/behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/bundle_pb2.py` & `gink-0.20240602.1717352499/gink/builders/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/change_pb2.py` & `gink-0.20240602.1717352499/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/claim_pb2.py` & `gink-0.20240602.1717352499/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/clearance_pb2.py` & `gink-0.20240602.1717352499/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/container_pb2.py` & `gink-0.20240602.1717352499/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/entry_pb2.py` & `gink-0.20240602.1717352499/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/header_pb2.py` & `gink-0.20240602.1717352499/gink/builders/header_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/key_pb2.py` & `gink-0.20240602.1717352499/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/log_file_pb2.py` & `gink-0.20240602.1717352499/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/movement_pb2.py` & `gink-0.20240602.1717352499/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/muid_pb2.py` & `gink-0.20240602.1717352499/gink/builders/muid_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/pair_pb2.py` & `gink-0.20240602.1717352499/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/sync_message_pb2.py` & `gink-0.20240602.1717352499/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/builders/value_pb2.py` & `gink-0.20240602.1717352499/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/abstract_store.py` & `gink-0.20240602.1717352499/gink/impl/abstract_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/addressable.py` & `gink-0.20240602.1717352499/gink/impl/addressable.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/attribution.py` & `gink-0.20240602.1717352499/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/box.py` & `gink-0.20240602.1717352499/gink/impl/box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/braid.py` & `gink-0.20240602.1717352499/gink/impl/braid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/builders.py` & `gink-0.20240602.1717352499/gink/impl/builders.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/bundle_info.py` & `gink-0.20240602.1717352499/gink/impl/bundle_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/bundle_store.py` & `gink-0.20240602.1717352499/gink/impl/bundle_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/bundle_wrapper.py` & `gink-0.20240602.1717352499/gink/impl/bundle_wrapper.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/bundler.py` & `gink-0.20240602.1717352499/gink/impl/bundler.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/chain_tracker.py` & `gink-0.20240602.1717352499/gink/impl/chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/coding.py` & `gink-0.20240602.1717352499/gink/impl/coding.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/connection.py` & `gink-0.20240602.1717352499/gink/impl/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,41 +8,40 @@
 from logging import getLogger
 from abc import ABC, abstractmethod
 
 from .builders import SyncMessage
 from .chain_tracker import ChainTracker
 from .bundle_info import BundleInfo
 from .bundle_wrapper import BundleWrapper
+from .typedefs import AuthFunc
 
 
 class Connection(ABC):
     """ Manages a connection to another gink database.
 
         Eventually there will be two subclasses: one to manage websocket connections,
         and another subclass to manage raw socket connections.
     """
     on_ready: Callable
     def __init__(
-            self,
+            self, *,
             host: Optional[str] = None,
             port: Optional[int] = None,
             socket: Optional[Socket] = None,
-            greeting: Optional[SyncMessage] = None,
     ):
         if socket is None:
             assert host is not None and port is not None
             socket = Socket(AF_INET, SOCK_STREAM)
             socket.connect((host, port))
         self._socket = socket
         self._host = host
         self._port = port
         self._logger = getLogger(self.__class__.__name__)
         self._closed = False
         self._tracker: Optional[ChainTracker] = None
-        self._greeting = greeting
 
     def fileno(self):
         """ Return the file descriptor of the underlying socket.
         """
         return self._socket.fileno()
 
     def is_closed(self) -> bool:
```

### Comparing `gink-0.20240601.1717210459/gink/impl/container.py` & `gink-0.20240602.1717352499/gink/impl/container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/database.py` & `gink-0.20240602.1717352499/gink/impl/database.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/deferred.py` & `gink-0.20240602.1717352499/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/directory.py` & `gink-0.20240602.1717352499/gink/impl/directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/graph.py` & `gink-0.20240602.1717352499/gink/impl/graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/group.py` & `gink-0.20240602.1717352499/gink/impl/group.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/key_set.py` & `gink-0.20240602.1717352499/gink/impl/key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/lmdb_store.py` & `gink-0.20240602.1717352499/gink/impl/lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/lmdb_utilities.py` & `gink-0.20240602.1717352499/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/log_backed_store.py` & `gink-0.20240602.1717352499/gink/impl/log_backed_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/looping.py` & `gink-0.20240602.1717352499/gink/impl/looping.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/memory_store.py` & `gink-0.20240602.1717352499/gink/impl/memory_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/muid.py` & `gink-0.20240602.1717352499/gink/impl/muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/pair_map.py` & `gink-0.20240602.1717352499/gink/impl/pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/pair_set.py` & `gink-0.20240602.1717352499/gink/impl/pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/property.py` & `gink-0.20240602.1717352499/gink/impl/property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/relay.py` & `gink-0.20240602.1717352499/gink/impl/relay.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,117 +1,86 @@
 """ contains the Relay class """
 
 # standard python modules
 from typing import Set, Union, Iterable, List, Callable, Optional
 from threading import Lock
 from logging import getLogger
 from re import fullmatch, IGNORECASE
-from socket import socketpair
+
 
 # gink modules
 from .abstract_store import AbstractStore
 from .bundle_info import BundleInfo
 from .connection import Connection
 from .websocket_connection import WebsocketConnection
 from .listener import Listener
 from .chain_tracker import ChainTracker
 from .lmdb_store import LmdbStore
 from .memory_store import MemoryStore
 from .bundle_wrapper import BundleWrapper
-from .utilities import (
-    experimental,
-)
 from .looping import Selectable, Finished
 from .bundle_store import BundleStore
+from .server import Server
 from .typedefs import AuthFunc
 
-class Relay:
+class Relay(Server):
 
     _store: BundleStore
-    _connections: Set[Connection]
-    _listeners: Set[Listener]
     _lock: Lock
     _not_acked: Set[BundleInfo]
 
     def __init__(self, store: Union[BundleStore, str, None] = None):
+        super().__init__()
         if isinstance(store, str):
             store = LmdbStore(store)
         if isinstance(store, type(None)):
             store = MemoryStore()
         assert isinstance(store, AbstractStore)
         self._store = store
-        self._connections = set()
-        self._listeners = set()
         self._logger = getLogger(self.__class__.__name__)
         self._callbacks: List[Callable[[BundleWrapper], None]] = list()
-        (self._socket_left, self._socket_rite) = socketpair()
-        self._indication_sent = False
+        self._connections: Set[Connection] = set()
         self._lock = Lock()
         self._not_acked = set()
         if self._store.is_selectable():
-            self._indicate_selectables_changed()
-
-    def fileno(self) -> int:
-        return self._socket_rite.fileno()
+            self._store.on_ready = self._on_store_ready
+            self._add_selectable(self._store)
 
-    @experimental
     def add_callback(self, callback: Callable[[BundleWrapper], None]):
         self._callbacks.append(callback)
 
-    def start_listening(self, ip_addr="", port: Union[str, int] = "8080", auth_func: Optional[AuthFunc]=None):
-        """ Listen for incoming connections on the given port.
-
-            Note that you'll still need to call "run" to actually accept those connections.
-        """
-        port = int(port)
-        self._logger.info("starting to listen on %r:%r", ip_addr, port)
-        listener = Listener(WebsocketConnection, ip_addr=ip_addr, port=port, auth_func=auth_func)
-        listener.on_ready = lambda: self._on_listener_ready(listener)
-        self._listeners.add(listener)
-        self._indicate_selectables_changed()
-
     def connect_to(self, target: str, auth_data: Optional[str] = None):
         """ initiate a connection to another gink instance """
         self._logger.info("initating connection to %s", target)
         match = fullmatch(r"(ws+://)?([a-z0-9.-]+)(?::(\d+))?(?:/+(.*))?$", target, IGNORECASE)
         assert match, f"can't connect to: {target}"
         prefix, host, port, path = match.groups()
         if prefix and prefix != "ws://":
             raise NotImplementedError("only vanilla websockets currently supported")
         port = port or "8080"
         path = path or "/"
-        greeting = self._store.get_chain_tracker().to_greeting_message()
+        sync_func = lambda _: self._store.get_chain_tracker().to_greeting_message()
         connection = WebsocketConnection(
             host=host,
             port=int(port),
             path=path,
-            greeting=greeting,
+            sync_func=sync_func,
             auth_data=auth_data,
             )
         connection.on_ready = lambda: self._on_connection_ready(connection)
         self._connections.add(connection)
         self._logger.debug("connection added")
-        self._indicate_selectables_changed()
+        self._add_selectable(connection)
 
     def _on_store_ready(self):
         self._store.refresh(self._on_bundle)
 
-    def _indicate_selectables_changed(self):
-        if not self._indication_sent:
-            self._socket_left.send(b'0x01')
-            self._indication_sent = True
-
     def close(self):
-        for connection in self._connections:
-            connection.close()
-        for listener in self._listeners:
-            listener.close()
         self._store.close()
-        self._socket_left.close()
-        self._socket_rite.close()
+        super().close()
 
     def _on_bundle(self, bundle_wrapper: BundleWrapper) -> None:
         """ Sends a bundle either created locally or received from a peer to other peers.
         """
         for peer in self._connections:
             peer.send_bundle(bundle_wrapper)
         for callback in self._callbacks:
@@ -127,28 +96,24 @@
                         self._store.get_bundles(connection.send_bundle, peer_has=thing)
                     elif isinstance(thing, BundleInfo):  # an ack:
                         self._not_acked.discard(thing)
                     else:
                         raise AssertionError("unexpected object")
             except Finished:
                 self._connections.remove(connection)
+                self._remove_selectable(connection)
                 raise
 
     def _on_listener_ready(self, listener: Listener) -> Iterable[Selectable]:
-        sync_message = self._store.get_chain_tracker().to_greeting_message()
-        connection: Connection = listener.accept(sync_message)
+        (socket, addr) = listener.accept()
+        connection: Connection = WebsocketConnection(
+            socket=socket,
+            host=addr[0],
+            port=addr[1],
+            sync_func=lambda _: self._store.get_chain_tracker().to_greeting_message(),
+            auth_func=listener.get_auth(),
+        )
         connection.on_ready = lambda: self._on_connection_ready(connection)
         self._connections.add(connection)
-        self._logger.info("accepted incoming connection from %s", connection)
+        self._add_selectable(connection)
+        self._logger.info("accepted incoming connection from %s", addr)
         return [connection]
-
-    def on_ready(self) -> Iterable[Selectable]:
-        if self._indication_sent:
-            self._socket_rite.recv(1)
-            self._indication_sent = False
-        if self._store.is_selectable():
-            self._store.on_ready = self._on_store_ready
-            yield self._store
-        for listener in self._listeners:
-            yield listener
-        for connection in self._connections:
-            yield connection
```

### Comparing `gink-0.20240601.1717210459/gink/impl/selectable_console.py` & `gink-0.20240602.1717352499/gink/impl/selectable_console.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/sequence.py` & `gink-0.20240602.1717352499/gink/impl/sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/tuples.py` & `gink-0.20240602.1717352499/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/utilities.py` & `gink-0.20240602.1717352499/gink/impl/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from datetime import datetime, date, timedelta
 from re import fullmatch, IGNORECASE
 from psutil import pid_exists
 
 from .typedefs import MuTimestamp, Medallion, GenericTimestamp
 from .tuples import Chain
 from .builders import ClaimBuilder
-from .typedefs import AuthFunc, AUTH_BOTH, AUTH_NONE
+from .typedefs import AuthFunc, AUTH_FULL, AUTH_NONE
 
 def make_auth_func(token: str) -> AuthFunc:
-    def auth_func(data: str) -> int:
-        return AUTH_BOTH if fullmatch(f"token\s+{token}\s*", data, IGNORECASE) else AUTH_NONE
+    def auth_func(data: str, *_) -> int:
+        return AUTH_FULL if fullmatch(f"token\s+{token}\s*", data, IGNORECASE) else AUTH_NONE
     return auth_func
 
 def encodeToHex(string: str) -> str:
     """
     Takes a string and encodes it into a hex string prefixed with '0x'.
     """
     # Adding 0x so we can easily determine if a subprotocol is a hex string
```

### Comparing `gink-0.20240601.1717210459/gink/impl/watcher.py` & `gink-0.20240602.1717352499/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/websocket_connection.py` & `gink-0.20240602.1717352499/gink/impl/websocket_connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Contains the WsPeer class to manage a connection to a websocket (gink) peer. """
 
 # batteries included python imports
 from typing import Iterable, Optional, Callable
+from pathlib import Path
 from socket import (
     socket as Socket,
     SHUT_WR, SHUT_RDWR
 )
 
 from .utilities import decodeFromHex, encodeToHex
 
@@ -24,56 +25,61 @@
 
 # builders
 from .builders import SyncMessage
 
 # gink modules
 from .connection import Connection
 from .looping import Finished
-from .typedefs import AuthFunc, AUTH_BOTH
+from .typedefs import AuthFunc, AUTH_FULL, AUTH_RITE
 
 
 class WebsocketConnection(Connection):
     """ Manages the connection to one peer via a websocket.
 
         Set force_to_be_client to indicate that the provided socket is a client connection.
         If there's no socket provided then one will be established, and force_to_be_client is implied.
     """
     PROTOCOL = "gink"
     on_ready: Callable
+    _path: Optional[str]
     def __init__(
-            self,
+            self, *,
             host: Optional[str] = None,
             port: Optional[int] = None,
             socket: Optional[Socket] = None,
             force_to_be_client: bool = False,
             path: Optional[str] = None,
-            greeting: Optional[SyncMessage] = None,
+            sync_func: Optional[Callable[[Path], SyncMessage]] = None,
             auth_func: Optional[AuthFunc] = None,
             auth_data: Optional[str] = None,
+            permissions: int = AUTH_FULL,
     ):
-        Connection.__init__(self, socket=socket, host=host, port=port, greeting=greeting)
+        Connection.__init__(self, socket=socket, host=host, port=port)
         if socket is None:
             force_to_be_client = True
         connection_type = ConnectionType.CLIENT if force_to_be_client else ConnectionType.SERVER
         self._ws = WSConnection(connection_type=connection_type)
         self._ws_closed = False
         self._buffered: bytes = b""
         self._ready = False
         if force_to_be_client:
             subprotocols = [self.PROTOCOL]
             if auth_data:
                 subprotocols.append(encodeToHex(auth_data))
             host = host or "localhost"
-            path = path or "/"
-            request = Request(host=host, target=path, subprotocols=subprotocols)
+            self._path = path or "/"
+            request = Request(host=host, target=self._path, subprotocols=subprotocols)
             self._socket.send(self._ws.send(request))
+        else:
+            self._path = None
         self._logger.debug("finished setup")
         self._socket.settimeout(0.2)
         self._auth_func = auth_func
-        self._permissions: int = 0 if auth_func else AUTH_BOTH
+        self._sync_func = sync_func
+        self._permissions: int = 0 if auth_func else permissions
 
     def is_alive(self) -> bool:
         return not (self._ws_closed or self._closed)
 
     def __repr__(self):
         return f"{self.__class__.__name__}(host={self._host!r})"
 
@@ -83,30 +89,36 @@
         data = self._socket.recv(4096 * 4096)
         if not data:
             self._ws_closed = True
             raise Finished()
         self._ws.receive_data(data)
         for event in self._ws.events():
             if isinstance(event, Request):
+                if "?" in event.target:
+                    (self._path, _) = event.target.split("?", 2)
+                else:
+                    self._path = event.target
                 if self._auth_func:
                     for protocol in event.subprotocols:
                         if protocol.lower().startswith("0x"):
                             decoded = decodeFromHex(protocol)
-                            self._permissions |= self._auth_func(decoded)
+                            assert self._path is not None
+                            self._permissions |= self._auth_func(decoded, Path(self._path))
                 if not self._permissions:
                     self._logger.warning("could not authenticated connection")
                     self._socket.send(self._ws.send(RejectConnection()))
                 elif "gink" not in event.subprotocols:
                     self._logger.warning("got a non gink connection attempt")
                     self._socket.send(self._ws.send(RejectConnection()))
                 else:
                     self._logger.debug("got a Request, sending an AcceptConnection")
                     self._socket.send(self._ws.send(AcceptConnection("gink")))
                     self._logger.info("Server connection established!")
-                    self._send_greeting()
+                    if self._permissions & AUTH_RITE:
+                        self._send_greeting()
                     self._ready = True
             elif isinstance(event, CloseConnection):
                 self._logger.info("got close msg, code=%d, reason=%s", event.code, event.reason)
                 try:
                     self._socket.send(self._ws.send(event.response()))
                 except BrokenPipeError:
                     self._logger.warning("could not send websocket close ack")
@@ -130,24 +142,26 @@
             elif isinstance(event, Ping):
                 self._logger.debug("received ping")
                 self._socket.send(self._ws.send(event.response()))
             elif isinstance(event, Pong):
                 self._logger.debug("received pong")
             elif isinstance(event, AcceptConnection):
                 self._logger.info("Client connection established!")
-                self._send_greeting()
+                if self._permissions & AUTH_RITE:
+                    self._send_greeting()
                 self._ready = True
             else:
                 self._logger.warning("got an unexpected event type: %s", event)
 
     def _send_greeting(self):
-        if self._greeting is None:
-            self._logger.warning("no greeting message to send")
+        if self._sync_func is None or self._path is None:
+            self._logger.warning("cannot send greeting message")
             return
-        sent = self.send(self._greeting)
+        greeting = self._sync_func(Path(self._path))
+        sent = self.send(greeting)
         self._logger.debug("sent greeting of %d bytes", sent)
 
     def send(self, sync_message: SyncMessage) -> int:
         assert not self._closed
         data = self._ws.send(BytesMessage(sync_message.SerializeToString()))
         return self._socket.send(data)
```

### Comparing `gink-0.20240601.1717210459/gink/impl/wsgi_connection.py` & `gink-0.20240602.1717352499/gink/impl/wsgi_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/impl/wsgi_listener.py` & `gink-0.20240602.1717352499/gink/impl/wsgi_listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_box.py` & `gink-0.20240602.1717352499/gink/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_braid.py` & `gink-0.20240602.1717352499/gink/tests/test_braid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_chain_tracker.py` & `gink-0.20240602.1717352499/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_change_set_info.py` & `gink-0.20240602.1717352499/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_code_values.py` & `gink-0.20240602.1717352499/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_container.py` & `gink-0.20240602.1717352499/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_database.py` & `gink-0.20240602.1717352499/gink/tests/test_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,18 +106,15 @@
     for store_class in [
         LogBackedStore,
         LmdbStore,
     ]:
         if system() != 'Linux':
             return
         path1 = Path("/tmp/test1.gink")
-        path2 = Path("/tmp/test2.gink")
-
         path1.unlink(missing_ok=True)
-        path2.unlink(missing_ok=True)
 
         store1a = store_class(path1)
         store1b = store_class(path1)
 
         db1a = Database(store1a)
         db1b = Database(store1b)
 
@@ -125,15 +122,15 @@
         root1b = Directory(arche=True, database=db1b)
 
         loop(db1b, until=.01)
         bundle_infos = list()
         db1b.add_callback(lambda bw: bundle_infos.append(bw.get_info()))
         root1a.set("foo", "bar", comment="abc")
         loop(db1b, until=.01)
-        assert bundle_infos and bundle_infos[-1].comment == "abc"
+        assert bundle_infos and bundle_infos[-1].comment == "abc", (bundle_infos, store_class)
         found = root1b.get("foo")
         assert found == "bar", found
 
 
 def test_dump():
     """
         currently only tests that dump doesn't crash, in the future
```

### Comparing `gink-0.20240601.1717210459/gink/tests/test_demo.py` & `gink-0.20240602.1717352499/gink/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_directory.py` & `gink-0.20240602.1717352499/gink/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_graph.py` & `gink-0.20240602.1717352499/gink/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_key_set.py` & `gink-0.20240602.1717352499/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_lmdb_store.py` & `gink-0.20240602.1717352499/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_logbackedstore.py` & `gink-0.20240602.1717352499/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_muid.py` & `gink-0.20240602.1717352499/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_names.py` & `gink-0.20240602.1717352499/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_pair_map.py` & `gink-0.20240602.1717352499/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_pair_set.py` & `gink-0.20240602.1717352499/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_property.py` & `gink-0.20240602.1717352499/gink/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_role.py` & `gink-0.20240602.1717352499/gink/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_sequence.py` & `gink-0.20240602.1717352499/gink/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_store.py` & `gink-0.20240602.1717352499/gink/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_websocket_connection.py` & `gink-0.20240602.1717352499/gink/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink/tests/test_wsgi_server.py` & `gink-0.20240602.1717352499/gink/tests/test_wsgi_server.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240601.1717210459/gink.egg-info/PKG-INFO` & `gink-0.20240602.1717352499/gink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240601.1717210459
+Version: 0.20240602.1717352499
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240601.1717210459/gink.egg-info/SOURCES.txt` & `gink-0.20240602.1717352499/gink.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 gink/impl/muid.py
 gink/impl/pair_map.py
 gink/impl/pair_set.py
 gink/impl/property.py
 gink/impl/relay.py
 gink/impl/selectable_console.py
 gink/impl/sequence.py
+gink/impl/server.py
 gink/impl/tuples.py
 gink/impl/typedefs.py
 gink/impl/utilities.py
 gink/impl/watcher.py
 gink/impl/websocket_connection.py
 gink/impl/wsgi_connection.py
 gink/impl/wsgi_listener.py
```

### Comparing `gink-0.20240601.1717210459/setup.py` & `gink-0.20240602.1717352499/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240601.1717210459',
+    version='0.20240602.1717352499',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
```

