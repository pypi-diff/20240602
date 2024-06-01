# Comparing `tmp/ord_schema-0.3.76.tar.gz` & `tmp/ord_schema-0.3.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord_schema-0.3.76.tar", last modified: Fri May 17 10:51:17 2024, max compression
+gzip compressed data, was "ord_schema-0.3.77.tar", last modified: Sat Jun  1 22:41:24 2024, max compression
```

## Comparing `ord_schema-0.3.76.tar` & `ord_schema-0.3.77.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:51:17.426083 ord_schema-0.3.76/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-17 10:51:02.000000 ord_schema-0.3.76/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 10:51:02.000000 ord_schema-0.3.76/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 10:51:02.000000 ord_schema-0.3.76/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-17 10:51:17.426083 ord_schema-0.3.76/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-17 10:51:02.000000 ord_schema-0.3.76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:51:17.418083 ord_schema-0.3.76/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:51:17.418083 ord_schema-0.3.76/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (127)    36688 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:51:17.418083 ord_schema-0.3.76/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:51:17.422083 ord_schema-0.3.76/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/proto/dataset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    49481 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    92150 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/proto/reaction_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:51:17.422083 ord_schema-0.3.76/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    21548 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17564 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    47179 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (127)    23136 2024-05-17 10:51:02.000000 ord_schema-0.3.76/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:51:17.422083 ord_schema-0.3.76/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-17 10:51:17.000000 ord_schema-0.3.76/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-17 10:51:17.000000 ord_schema-0.3.76/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:51:17.000000 ord_schema-0.3.76/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-17 10:51:17.000000 ord_schema-0.3.76/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 10:51:17.000000 ord_schema-0.3.76/ord_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:51:17.422083 ord_schema-0.3.76/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-17 10:51:02.000000 ord_schema-0.3.76/proto/dataset.proto
--rw-r--r--   0 runner    (1001) docker     (127)    47240 2024-05-17 10:51:02.000000 ord_schema-0.3.76/proto/reaction.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-17 10:51:02.000000 ord_schema-0.3.76/proto/test.proto
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-17 10:51:02.000000 ord_schema-0.3.76/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:51:17.426083 ord_schema-0.3.76/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-17 10:51:07.000000 ord_schema-0.3.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:41:24.359417 ord_schema-0.3.77/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-06-01 22:41:11.000000 ord_schema-0.3.77/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 22:41:11.000000 ord_schema-0.3.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 22:41:11.000000 ord_schema-0.3.77/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-06-01 22:41:24.359417 ord_schema-0.3.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-06-01 22:41:11.000000 ord_schema-0.3.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:41:24.351416 ord_schema-0.3.77/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:41:24.351416 ord_schema-0.3.77/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36660 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27065 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:41:24.351416 ord_schema-0.3.77/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13978 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:41:24.355416 ord_schema-0.3.77/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/proto/dataset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49481 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92150 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/proto/reaction_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:41:24.355416 ord_schema-0.3.77/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21498 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17564 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47151 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23107 2024-06-01 22:41:11.000000 ord_schema-0.3.77/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:41:24.355416 ord_schema-0.3.77/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-06-01 22:41:24.000000 ord_schema-0.3.77/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-06-01 22:41:24.000000 ord_schema-0.3.77/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:41:24.000000 ord_schema-0.3.77/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-01 22:41:24.000000 ord_schema-0.3.77/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 22:41:24.000000 ord_schema-0.3.77/ord_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:41:24.355416 ord_schema-0.3.77/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-01 22:41:11.000000 ord_schema-0.3.77/proto/dataset.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    47240 2024-06-01 22:41:11.000000 ord_schema-0.3.77/proto/reaction.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-06-01 22:41:11.000000 ord_schema-0.3.77/proto/test.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-01 22:41:11.000000 ord_schema-0.3.77/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:41:24.359417 ord_schema-0.3.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-06-01 22:41:13.000000 ord_schema-0.3.77/setup.py
```

### Comparing `ord_schema-0.3.76/LICENSE` & `ord_schema-0.3.77/LICENSE`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/PKG-INFO` & `ord_schema-0.3.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.76
+Version: 0.3.77
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord_schema-0.3.76/README.md` & `ord_schema-0.3.77/README.md`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/__init__.py` & `ord_schema-0.3.77/ord_schema/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Generic helpers for ord_schema, including common message types."""
 from typing import Union
 
-from google.protobuf import descriptor
 import google.protobuf.message  # pytype: disable=import-error
+from google.protobuf import descriptor
 
 from ord_schema.proto import reaction_pb2
 
 # Commonly used types.
 FieldDescriptor = descriptor.FieldDescriptor
 Message = google.protobuf.message.Message
 ScalarType = Union[str, bytes, float, int, bool]
```

### Comparing `ord_schema-0.3.76/ord_schema/frozen_message.py` & `ord_schema-0.3.77/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/frozen_message_test.py` & `ord_schema-0.3.77/ord_schema/frozen_message_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 
 import dataclasses
 import os
 import tempfile
 
 import pytest
 
-from ord_schema import frozen_message
-from ord_schema import message_helpers
-from ord_schema.proto import reaction_pb2
-from ord_schema.proto import test_pb2
+from ord_schema import frozen_message, message_helpers
+from ord_schema.proto import reaction_pb2, test_pb2
 
 
 def _freeze(message) -> frozen_message.FrozenMessage:
     """Runs a round-trip to disk as an extra check for FrozenMessage."""
     with tempfile.TemporaryDirectory() as tempdir:
         filename = os.path.join(tempdir, "message.pbtxt")
         message_helpers.write_message(message, filename)
```

### Comparing `ord_schema-0.3.76/ord_schema/logging.py` & `ord_schema-0.3.77/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/macros/__init__.py` & `ord_schema-0.3.77/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/macros/solutions.py` & `ord_schema-0.3.77/ord_schema/macros/solutions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Macros for programmatic message creation."""
 from typing import Optional, Union
 
-from ord_schema.proto import reaction_pb2
 from ord_schema import units
+from ord_schema.proto import reaction_pb2
 
 UNITS_RESOLVER = units.UnitResolver()
 CONCENTRATION_RESOLVER = units.UnitResolver(units.CONCENTRATION_UNIT_SYNONYMS, forbidden_units={})
 
 
 def simple_solution(
     solvent_smiles: str,
```

### Comparing `ord_schema-0.3.76/ord_schema/macros/solutions_test.py` & `ord_schema-0.3.77/ord_schema/macros/solutions_test.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # limitations under the License.
 """Tests for ord_schema.macros.solutions."""
 import itertools
 
 import pytest
 from google.protobuf import text_format
 
-from ord_schema.proto import reaction_pb2
-from ord_schema.macros import solutions
 from ord_schema import validations
+from ord_schema.macros import solutions
+from ord_schema.proto import reaction_pb2
 
 
 def test_simple_solution():
     """Simple input/output pair test."""
     solvent_pbtxt = """
         identifiers {
             type: SMILES
```

### Comparing `ord_schema-0.3.76/ord_schema/macros/workups.py` & `ord_schema-0.3.77/ord_schema/macros/workups.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     workups.filter(keep_phase='filtrate'),
     workups.rotovap(),
     reaction_pb2.ReactionWorkup(type='OTHER_CHROMATOGRAPHY'),
 ])
 """
 from collections.abc import Iterable
 
-from ord_schema.proto import reaction_pb2
 from ord_schema import units
+from ord_schema.proto import reaction_pb2
 
 UNITS_RESOLVER = units.UnitResolver()
 CONCENTRATION_RESOLVER = units.UnitResolver(units.CONCENTRATION_UNIT_SYNONYMS)
 
 
 def add_solution(
     solution: Iterable[reaction_pb2.Compound], workup_type: str = "ADDITION"
```

### Comparing `ord_schema-0.3.76/ord_schema/message_helpers.py` & `ord_schema-0.3.77/ord_schema/message_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,24 +22,23 @@
 import warnings
 from collections.abc import Iterable, Mapping, Sequence
 from typing import Optional, Type, TypeVar, Union
 
 import pandas as pd
 import requests
 from google import protobuf  # pytype: disable=import-error
-from google.protobuf import json_format
 from google.protobuf import text_format  # pytype: disable=import-error
+from google.protobuf import json_format
 from rdkit import Chem
 from rdkit.Chem import rdChemReactions
 from werkzeug import security
 
 import ord_schema
 from ord_schema import units
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
+from ord_schema.proto import dataset_pb2, reaction_pb2
 
 _COMPOUND_IDENTIFIER_LOADERS = {
     reaction_pb2.CompoundIdentifier.SMILES: Chem.MolFromSmiles,
     reaction_pb2.CompoundIdentifier.INCHI: Chem.MolFromInchi,
     reaction_pb2.CompoundIdentifier.MOLBLOCK: Chem.MolFromMolBlock,
 }
 MessageType = TypeVar("MessageType")  # Generic for setting return types; pylint: disable=invalid-name.
```

### Comparing `ord_schema-0.3.76/ord_schema/message_helpers_test.py` & `ord_schema-0.3.77/ord_schema/message_helpers_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,21 +14,19 @@
 """Tests for ord_schema.message_helpers."""
 
 import tempfile
 import time
 
 import pandas as pd
 import pytest
-from google.protobuf import json_format
-from google.protobuf import text_format
+from google.protobuf import json_format, text_format
 from rdkit import Chem
 
 from ord_schema import message_helpers
-from ord_schema.proto import reaction_pb2
-from ord_schema.proto import test_pb2
+from ord_schema.proto import reaction_pb2, test_pb2
 
 _BENZENE_MOLBLOCK = """241
   -OEChem-07232015262D
 
  12 12  0     0  0  0  0  0  0999 V2000
     2.8660    1.0000    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0
     2.0000    0.5000    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0
```

### Comparing `ord_schema-0.3.76/ord_schema/orm/__init__.py` & `ord_schema-0.3.77/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/orm/conftest.py` & `ord_schema-0.3.77/ord_schema/orm/conftest.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/orm/database.py` & `ord_schema-0.3.77/ord_schema/orm/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Functions for creating/managing the PostgreSQL database."""
-import time
 import os
+import time
 from unittest.mock import patch
 
 from sqlalchemy import cast, delete, func, select, text, update
 from sqlalchemy.dialects.postgresql import insert
 from sqlalchemy.engine import Engine
-from sqlalchemy.exc import OperationalError, NotSupportedError
+from sqlalchemy.exc import NotSupportedError, OperationalError
 from sqlalchemy.orm import Session
 
 from ord_schema.logging import get_logger
 from ord_schema.orm.mappers import Base, Mappers, from_proto
 from ord_schema.orm.rdkit_mappers import CString, FingerprintType, RDKitMol, RDKitReaction
 from ord_schema.proto import dataset_pb2
```

### Comparing `ord_schema-0.3.76/ord_schema/orm/database_test.py` & `ord_schema-0.3.77/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/orm/mappers.py` & `ord_schema-0.3.77/ord_schema/orm/mappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,25 +31,23 @@
 from hashlib import md5
 from operator import attrgetter
 from typing import Any, Mapping, Optional, Type
 
 from google.protobuf.descriptor import Descriptor, FieldDescriptor
 from google.protobuf.message import Message
 from inflection import underscore
-from sqlalchemy import Boolean, Column, Enum, Float, Integer, ForeignKey, LargeBinary, String, Text
+from sqlalchemy import Boolean, Column, Enum, Float, ForeignKey, Integer, LargeBinary, String, Text
 from sqlalchemy.dialects.postgresql import ARRAY
 from sqlalchemy.orm import relationship
 
 import ord_schema.orm.rdkit_mappers  # pylint: disable=unused-import
 from ord_schema import message_helpers
 from ord_schema.logging import get_logger
 from ord_schema.orm import Base
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
-
+from ord_schema.proto import dataset_pb2, reaction_pb2
 
 logger = get_logger(__name__)
 
 
 def get_message_type(full_name: str) -> Any:
     """Fetches the class for a protocol buffer message type."""
     if not full_name.startswith("ord."):
```

### Comparing `ord_schema-0.3.76/ord_schema/orm/mappers_test.py` & `ord_schema-0.3.77/ord_schema/orm/mappers_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for ord_schema.orm.mappers."""
 import os
+
 import pytest
 
 from ord_schema.message_helpers import load_message
 from ord_schema.orm.mappers import from_proto, to_proto
 from ord_schema.proto.dataset_pb2 import Dataset
```

### Comparing `ord_schema-0.3.76/ord_schema/orm/rdkit_mappers.py` & `ord_schema-0.3.77/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/orm/rdkit_mappers_test.py` & `ord_schema-0.3.77/ord_schema/orm/rdkit_mappers_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for ord_schema.orm.rdkit_mappers."""
 import pytest
 from sqlalchemy import select
 from sqlalchemy.exc import ProgrammingError
+
 from ord_schema.orm.mappers import Mappers
 from ord_schema.orm.rdkit_mappers import FingerprintType, RDKitMol
 
 
 def test_tanimoto_operator(test_session):
     try:
         query = (
```

### Comparing `ord_schema-0.3.76/ord_schema/proto/__init__.py` & `ord_schema-0.3.77/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/proto/dataset_pb2.py` & `ord_schema-0.3.77/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/proto/dataset_pb2.pyi` & `ord_schema-0.3.77/ord_schema/proto/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/proto/dataset_pb2_test.py` & `ord_schema-0.3.77/ord_schema/proto/dataset_pb2_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for ord_schema.proto.dataset_pb2."""
 
 import pytest
 
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
+from ord_schema.proto import dataset_pb2, reaction_pb2
 
 
 @pytest.fixture
 def serialized_dataset() -> bytes:
     dataset = dataset_pb2.Dataset()
     dataset.name = "test"
     dataset.description = "test dataset"
```

### Comparing `ord_schema-0.3.76/ord_schema/proto/reaction_pb2.py` & `ord_schema-0.3.77/ord_schema/proto/reaction_pb2.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/proto/reaction_pb2.pyi` & `ord_schema-0.3.77/ord_schema/proto/reaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/proto/reaction_pb2_test.py` & `ord_schema-0.3.77/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/proto/test_pb2.py` & `ord_schema-0.3.77/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/resolvers.py` & `ord_schema-0.3.77/ord_schema/resolvers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Name/string resolution to structured messages or identifiers."""
 import email.message
 import re
+import urllib.error
 import urllib.parse
 import urllib.request
-import urllib.error
 
 from rdkit import Chem
 
-from ord_schema.logging import get_logger
 from ord_schema import message_helpers
+from ord_schema.logging import get_logger
 from ord_schema.proto import reaction_pb2
 
 logger = get_logger(__name__)
 
 _COMPOUND_STRUCTURAL_IDENTIFIERS = [
     reaction_pb2.CompoundIdentifier.SMILES,
     reaction_pb2.CompoundIdentifier.INCHI,
```

### Comparing `ord_schema-0.3.76/ord_schema/resolvers_test.py` & `ord_schema-0.3.77/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/scripts/__init__.py` & `ord_schema-0.3.77/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/scripts/build_dataset.py` & `ord_schema-0.3.77/ord_schema/scripts/build_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,17 @@
     --description=<str>     Description for this dataset
     --no-validate           If set, do run validations on reactions
 """
 import glob
 
 import docopt
 
+from ord_schema import message_helpers, validations
 from ord_schema.logging import get_logger
-from ord_schema import message_helpers
-from ord_schema import validations
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
+from ord_schema.proto import dataset_pb2, reaction_pb2
 
 logger = get_logger(__name__)
 
 
 def main(kwargs):
     filenames = glob.glob(kwargs["--input"], recursive=True)
     logger.info("Found %d Reaction protos", len(filenames))
```

### Comparing `ord_schema-0.3.76/ord_schema/scripts/build_dataset_test.py` & `ord_schema-0.3.77/ord_schema/scripts/build_dataset_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,16 @@
 # limitations under the License.
 """Tests for ord_schema.scripts.build_dataset."""
 import os
 
 import docopt
 import pytest
 
-from ord_schema import message_helpers
-from ord_schema import validations
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
+from ord_schema import message_helpers, validations
+from ord_schema.proto import dataset_pb2, reaction_pb2
 from ord_schema.scripts import build_dataset
 
 
 @pytest.fixture
 def dirname(tmp_path) -> str:
     reaction1 = reaction_pb2.Reaction()
     dummy_input = reaction1.inputs["dummy_input"]
```

### Comparing `ord_schema-0.3.76/ord_schema/scripts/check_pb.py` & `ord_schema-0.3.77/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/scripts/check_pb_test.py` & `ord_schema-0.3.77/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/scripts/enumerate_dataset.py` & `ord_schema-0.3.77/ord_schema/scripts/enumerate_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,16 @@
     --template=<str>        Path to a Reaction pbtxt file defining a template
     --spreadsheet=<str>     Path to a spreadsheet file with a header row matching template placeholders
     --output=<str>          Filename for output Dataset
     --no-validate           If set, do not validate Reaction protos
 """
 import docopt
 
+from ord_schema import message_helpers, templating
 from ord_schema.logging import get_logger
-from ord_schema import message_helpers
-from ord_schema import templating
 
 logger = get_logger(__name__)
 
 
 def main(kwargs):
     with open(kwargs["--template"]) as f:
         template_string = f.read()
```

### Comparing `ord_schema-0.3.76/ord_schema/scripts/enumerate_dataset_test.py` & `ord_schema-0.3.77/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 """Tests for ord_schema.scripts.enumerate_dataset."""
 import os
 
 import docopt
 import pandas as pd
 import pytest
 
-from ord_schema import message_helpers
-from ord_schema import validations
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
+from ord_schema import message_helpers, validations
+from ord_schema.proto import dataset_pb2, reaction_pb2
 from ord_schema.scripts import enumerate_dataset
 
 
 @pytest.fixture
 def setup(tmp_path) -> tuple[str, str, str]:
     dirname = tmp_path.as_posix()
     template_string = """
```

### Comparing `ord_schema-0.3.76/ord_schema/scripts/parse_uspto.py` & `ord_schema-0.3.77/ord_schema/scripts/parse_uspto.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,20 +39,17 @@
 from xml.etree import ElementTree
 
 import docopt
 import joblib
 from rdkit import RDLogger
 
 import ord_schema
+from ord_schema import message_helpers, units, validations
 from ord_schema.logging import get_logger
-from ord_schema import message_helpers
-from ord_schema import units
-from ord_schema import validations
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
+from ord_schema.proto import dataset_pb2, reaction_pb2
 
 logger = get_logger(__name__)
 RDLogger.DisableLog("rdApp.*")  # Disable RDKit logging.
 
 # XML namespaces.
 NAMESPACES = {
     "cml": "http://www.xml-cml.org/schema",
```

### Comparing `ord_schema-0.3.76/ord_schema/scripts/process_dataset.py` & `ord_schema-0.3.77/ord_schema/scripts/process_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,18 +52,16 @@
 from collections.abc import Iterable, Mapping
 from typing import Optional
 
 import docopt
 import github
 from rdkit import RDLogger
 
+from ord_schema import message_helpers, updates, validations
 from ord_schema.logging import get_logger
-from ord_schema import message_helpers
-from ord_schema import updates
-from ord_schema import validations
 from ord_schema.proto import dataset_pb2
 
 logger = get_logger(__name__)
 
 
 # pylint: disable=too-many-branches,too-many-locals
```

### Comparing `ord_schema-0.3.76/ord_schema/scripts/process_dataset_test.py` & `ord_schema-0.3.77/ord_schema/scripts/process_dataset_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 import subprocess
 from typing import Optional
 
 import docopt
 import pytest
 from rdkit import RDLogger
 
+from ord_schema import message_helpers, validations
 from ord_schema.logging import get_logger
-from ord_schema import message_helpers
-from ord_schema import validations
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
+from ord_schema.proto import dataset_pb2, reaction_pb2
 from ord_schema.scripts import process_dataset
 
 logger = get_logger(__name__)
 
 
 class TestProcessDataset:
     @pytest.fixture
```

### Comparing `ord_schema-0.3.76/ord_schema/scripts/validate_dataset.py` & `ord_schema-0.3.77/ord_schema/scripts/validate_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 import glob
 import re
 from collections.abc import Iterable
 
 import docopt
 from rdkit import RDLogger
 
+from ord_schema import message_helpers, validations
 from ord_schema.logging import get_logger
-from ord_schema import message_helpers
-from ord_schema import validations
 from ord_schema.proto import dataset_pb2
 
 logger = get_logger(__name__)
 
 
 def filter_filenames(filenames: Iterable[str], pattern: str) -> list[str]:
     """Filters filenames according to a regex pattern."""
```

### Comparing `ord_schema-0.3.76/ord_schema/scripts/validate_dataset_test.py` & `ord_schema-0.3.77/ord_schema/scripts/validate_dataset_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,16 @@
 # limitations under the License.
 """Tests for ord_schema.scripts.validate_dataset."""
 import os
 
 import docopt
 import pytest
 
-from ord_schema import message_helpers
-from ord_schema import validations
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
+from ord_schema import message_helpers, validations
+from ord_schema.proto import dataset_pb2, reaction_pb2
 from ord_schema.scripts import validate_dataset
 
 
 @pytest.fixture
 def setup(tmp_path) -> str:
     test_subdirectory = tmp_path.as_posix()
     reaction1 = reaction_pb2.Reaction()
```

### Comparing `ord_schema-0.3.76/ord_schema/templating.py` & `ord_schema-0.3.77/ord_schema/templating.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 from typing import BinaryIO, Optional, Union
 
 import pandas as pd
 from google.protobuf import text_format  # pytype: disable=import-error
 
 import ord_schema
 from ord_schema import validations
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
-
+from ord_schema.proto import dataset_pb2, reaction_pb2
 
 # pylint: disable=too-many-branches
 
 
 def read_spreadsheet(file_name_or_buffer: Union[str, BinaryIO], suffix: Optional[str] = None) -> pd.DataFrame:
     """Reads a {csv, xls, xlsx} spreadsheet file.
```

### Comparing `ord_schema-0.3.76/ord_schema/templating_test.py` & `ord_schema-0.3.77/ord_schema/templating_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 
 import pandas as pd
 import pytest
 from google.protobuf import text_format
 from rdkit import Chem
 
 from ord_schema import templating
-from ord_schema.proto import reaction_pb2
-from ord_schema.proto import dataset_pb2
+from ord_schema.proto import dataset_pb2, reaction_pb2
 
 
 @pytest.fixture
 def valid_reaction() -> reaction_pb2.Reaction:
     message = reaction_pb2.Reaction()
     dummy_input = message.inputs["in"]
     outcome = message.outcomes.add()
```

### Comparing `ord_schema-0.3.76/ord_schema/units.py` & `ord_schema-0.3.77/ord_schema/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Helpers for translating strings with units."""
 
 import re
-from typing import Optional, Type, Union, Tuple
+from typing import Optional, Tuple, Type, Union
 
 import numpy as np
 
 import ord_schema
 from ord_schema.proto import reaction_pb2
 
 # Accepted synonyms for units. Note that all values will be converted to
```

### Comparing `ord_schema-0.3.76/ord_schema/units_test.py` & `ord_schema-0.3.77/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema/updates.py` & `ord_schema-0.3.77/ord_schema/updates.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 # limitations under the License.
 """Automated updates for Reaction messages."""
 
 import datetime
 import re
 import uuid
 
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
+from ord_schema.proto import dataset_pb2, reaction_pb2
 
 _COMPOUND_STRUCTURAL_IDENTIFIERS = [
     reaction_pb2.CompoundIdentifier.SMILES,
     reaction_pb2.CompoundIdentifier.INCHI,
     reaction_pb2.CompoundIdentifier.MOLBLOCK,
     reaction_pb2.CompoundIdentifier.CXSMILES,
     reaction_pb2.CompoundIdentifier.XYZ,
```

### Comparing `ord_schema-0.3.76/ord_schema/updates_test.py` & `ord_schema-0.3.77/ord_schema/updates_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for ord_schema.updates."""
 
 import pytest
 
 from ord_schema import updates
-from ord_schema.proto import reaction_pb2
-from ord_schema.proto import dataset_pb2
+from ord_schema.proto import dataset_pb2, reaction_pb2
 
 
 class TestUpdateReaction:
     def test_with_updates_simple(self):
         message = reaction_pb2.Reaction()
         updates.update_reaction(message)
         assert message != reaction_pb2.Reaction()
```

### Comparing `ord_schema-0.3.76/ord_schema/validations.py` & `ord_schema-0.3.77/ord_schema/validations.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 """Helpers validating specific Message types."""
 import dataclasses
 import math
 import os
 import re
 import warnings
 from collections.abc import Mapping
-from typing import Any, Optional
 from enum import IntEnum
+from typing import Any, Optional
 
 from dateutil import parser
 from rdkit import Chem
 from rdkit import __version__ as RDKIT_VERSION
 
 import ord_schema
-from ord_schema.logging import get_logger
 from ord_schema import message_helpers
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
+from ord_schema.logging import get_logger
+from ord_schema.proto import dataset_pb2, reaction_pb2
 
 logger = get_logger(__name__)
 
 
 # pylint: disable=too-many-branches
```

### Comparing `ord_schema-0.3.76/ord_schema/validations_test.py` & `ord_schema-0.3.77/ord_schema/validations_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 import sys
 import warnings
 
 import pytest
 from google.protobuf import text_format
 
 from ord_schema import validations
-from ord_schema.proto import dataset_pb2
-from ord_schema.proto import reaction_pb2
-
+from ord_schema.proto import dataset_pb2, reaction_pb2
 
 # pylint: disable=too-many-public-methods
 
 
 @pytest.fixture(autouse=True)
 def setup():
     # Redirect warning messages to stdout so they can be filtered from the other test output.
```

### Comparing `ord_schema-0.3.76/ord_schema.egg-info/PKG-INFO` & `ord_schema-0.3.77/ord_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.76
+Version: 0.3.77
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord_schema-0.3.76/ord_schema.egg-info/SOURCES.txt` & `ord_schema-0.3.77/ord_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/ord_schema.egg-info/requires.txt` & `ord_schema-0.3.77/ord_schema.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/proto/dataset.proto` & `ord_schema-0.3.77/proto/dataset.proto`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/proto/reaction.proto` & `ord_schema-0.3.77/proto/reaction.proto`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/proto/test.proto` & `ord_schema-0.3.77/proto/test.proto`

 * *Files identical despite different names*

### Comparing `ord_schema-0.3.76/setup.py` & `ord_schema-0.3.77/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Installer script."""
 import setuptools
 
-
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.76",
+    version="0.3.77",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

