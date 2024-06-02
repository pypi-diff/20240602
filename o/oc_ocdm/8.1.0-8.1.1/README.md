# Comparing `tmp/oc_ocdm-8.1.0.tar.gz` & `tmp/oc_ocdm-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc_ocdm-8.1.0.tar", max compression
+gzip compressed data, was "oc_ocdm-8.1.1.tar", max compression
```

## Comparing `oc_ocdm-8.1.0.tar` & `oc_ocdm-8.1.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0      782 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/LICENSE.md
--rw-r--r--   0        0        0     4932 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/README.md
--rw-r--r--   0        0        0      913 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/__init__.py
--rw-r--r--   0        0        0     7810 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/abstract_entity.py
--rw-r--r--   0        0        0     2811 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/abstract_set.py
--rw-r--r--   0        0        0     1063 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/counter_handler/__init__.py
--rw-r--r--   0        0        0     6370 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/counter_handler/counter_handler.py
--rw-r--r--   0        0        0    18162 2024-05-19 12:11:08.241109 oc_ocdm-8.1.0/oc_ocdm/counter_handler/filesystem_counter_handler.py
--rw-r--r--   0        0        0    12389 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/counter_handler/in_memory_counter_handler.py
--rw-r--r--   0        0        0     3581 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/counter_handler/sqlite_counter_handler.py
--rw-r--r--   0        0        0     2588 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/decorators.py
--rw-r--r--   0        0        0      919 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/graph/__init__.py
--rw-r--r--   0        0        0      956 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/__init__.py
--rw-r--r--   0        0        0     1654 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/__init__.py
--rw-r--r--   0        0        0     8233 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/agent_role.py
--rw-r--r--   0        0        0     8869 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py
--rw-r--r--   0        0        0    48004 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py
--rw-r--r--   0        0        0    15906 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/citation.py
--rw-r--r--   0        0        0    21065 2024-05-19 11:18:15.261698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/discourse_element.py
--rw-r--r--   0        0        0     6171 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/pointer_list.py
--rw-r--r--   0        0        0     4807 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/reference_annotation.py
--rw-r--r--   0        0        0     9901 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/reference_pointer.py
--rw-r--r--   0        0        0    10104 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py
--rw-r--r--   0        0        0     8614 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/responsible_agent.py
--rw-r--r--   0        0        0     6443 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic_entity.py
--rw-r--r--   0        0        0    19946 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/graph/entities/identifier.py
--rw-r--r--   0        0        0    15326 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/graph/graph_entity.py
--rw-r--r--   0        0        0    19833 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/graph/graph_set.py
--rw-r--r--   0        0        0      937 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/metadata/__init__.py
--rw-r--r--   0        0        0      941 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/metadata/entities/__init__.py
--rw-r--r--   0        0        0    18784 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/metadata/entities/dataset.py
--rw-r--r--   0        0        0    12161 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/metadata/entities/distribution.py
--rw-r--r--   0        0        0     7405 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/metadata/metadata_entity.py
--rw-r--r--   0        0        0     6411 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/metadata/metadata_set.py
--rw-r--r--   0        0        0      913 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/prov/__init__.py
--rw-r--r--   0        0        0      888 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/prov/entities/__init__.py
--rw-r--r--   0        0        0    13309 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/prov/entities/snapshot_entity.py
--rw-r--r--   0        0        0     3673 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/prov/prov_entity.py
--rw-r--r--   0        0        0    16593 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/prov/prov_set.py
--rw-r--r--   0        0        0    11825 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/reader.py
--rw-r--r--   0        0        0      822 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/resources/__init__.py
--rw-r--r--   0        0        0     1361 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/resources/querymap.txt
--rw-r--r--   0        0        0    20997 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/resources/shacle.ttl
--rw-r--r--   0        0        0    12150 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/resources/shexc.txt
--rw-r--r--   0        0        0    12248 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/resources/shexc_closed.txt
--rw-r--r--   0        0        0    16455 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/storer.py
--rw-r--r--   0        0        0     1332 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/support/__init__.py
--rw-r--r--   0        0        0     3460 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/support/query_utils.py
--rw-r--r--   0        0        0     2550 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/support/reporter.py
--rw-r--r--   0        0        0    15410 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/support/support.py
--rw-r--r--   0        0        0      822 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/__init__.py
--rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/counter_handler/__init__.py
--rw-r--r--   0        0        0     8502 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py
--rw-r--r--   0        0        0    10970 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py
--rw-r--r--   0        0        0    69632 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/coverage/.coverage
--rw-r--r--   0        0        0      107 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/coverage/.coveragerc
--rw-r--r--   0        0        0      904 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/coverage/coverage.svg
--rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/__init__.py
--rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/__init__.py
--rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/__init__.py
--rw-r--r--   0        0        0     2608 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py
--rw-r--r--   0        0        0     2149 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py
--rw-r--r--   0        0        0    12323 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py
--rw-r--r--   0        0        0     6730 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_citation.py
--rw-r--r--   0        0        0     4776 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py
--rw-r--r--   0        0        0     1856 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py
--rw-r--r--   0        0        0     1696 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py
--rw-r--r--   0        0        0     2433 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py
--rw-r--r--   0        0        0     2908 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py
--rw-r--r--   0        0        0     2466 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py
--rw-r--r--   0        0        0     2903 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/test_bibliographic_entity.py
--rw-r--r--   0        0        0     7908 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/test_identifier.py
--rw-r--r--   0        0        0      940 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/test_graph_entity.py
--rw-r--r--   0        0        0     6500 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/graph/test_graph_set.py
--rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/metadata/__init__.py
--rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/metadata/entities/__init__.py
--rw-r--r--   0        0        0     4573 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/metadata/entities/test_dataset.py
--rw-r--r--   0        0        0     3507 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/metadata/entities/test_distribution.py
--rw-r--r--   0        0        0     2665 2024-05-19 11:18:15.265698 oc_ocdm-8.1.0/oc_ocdm/test/metadata/test_metadata_set.py
--rw-r--r--   0        0        0      837 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/prov/__init__.py
--rw-r--r--   0        0        0      837 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/prov/entities/__init__.py
--rw-r--r--   0        0        0     4141 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/prov/entities/test_snapshot_entity.py
--rw-r--r--   0        0        0    12288 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/prov/prov_counter.db
--rw-r--r--   0        0        0    12789 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/prov/test_prov_set.py
--rw-r--r--   0        0        0        0 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/reader/__init__.py
--rw-r--r--   0        0        0     2523 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/reader/br.nt
--rw-r--r--   0        0        0     1862 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/reader/test_reader.py
--rw-r--r--   0        0        0      822 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/resources/__init__.py
--rw-r--r--   0        0        0     6448 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/resources/data.json
--rw-r--r--   0        0        0     6448 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/resources/data_reader.json
--rw-r--r--   0        0        0     6449 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/resources/data_reader_invalid.json
--rw-r--r--   0        0        0     3602 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/resources/test_shacle.py
--rw-r--r--   0        0        0      826 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/storer/__init__.py
--rw-r--r--   0        0        0    14739 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/storer/test_storer.py
--rw-r--r--   0        0        0      837 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/support/__init__.py
--rw-r--r--   0        0        0     5356 2024-05-19 11:18:15.269698 oc_ocdm-8.1.0/oc_ocdm/test/support/test_support.py
--rw-r--r--   0        0        0     1558 2024-05-19 12:11:24.741184 oc_ocdm-8.1.0/pyproject.toml
--rw-r--r--   0        0        0     6442 1970-01-01 00:00:00.000000 oc_ocdm-8.1.0/PKG-INFO
+-rw-r--r--   0        0        0      782 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/LICENSE.md
+-rw-r--r--   0        0        0     4932 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/README.md
+-rw-r--r--   0        0        0      913 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/__init__.py
+-rw-r--r--   0        0        0     7810 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/abstract_entity.py
+-rw-r--r--   0        0        0     2811 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/abstract_set.py
+-rw-r--r--   0        0        0     1063 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/counter_handler/__init__.py
+-rw-r--r--   0        0        0     6370 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/counter_handler/counter_handler.py
+-rw-r--r--   0        0        0    18162 2024-05-19 12:11:08.241109 oc_ocdm-8.1.1/oc_ocdm/counter_handler/filesystem_counter_handler.py
+-rw-r--r--   0        0        0    12389 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/counter_handler/in_memory_counter_handler.py
+-rw-r--r--   0        0        0     3581 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/counter_handler/sqlite_counter_handler.py
+-rw-r--r--   0        0        0     2588 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/decorators.py
+-rw-r--r--   0        0        0      919 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/graph/__init__.py
+-rw-r--r--   0        0        0      956 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/__init__.py
+-rw-r--r--   0        0        0     1654 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/__init__.py
+-rw-r--r--   0        0        0     8233 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/agent_role.py
+-rw-r--r--   0        0        0     8869 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py
+-rw-r--r--   0        0        0    48004 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py
+-rw-r--r--   0        0        0    15906 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/citation.py
+-rw-r--r--   0        0        0    21065 2024-05-19 11:18:15.261698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/discourse_element.py
+-rw-r--r--   0        0        0     6171 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/pointer_list.py
+-rw-r--r--   0        0        0     4807 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/reference_annotation.py
+-rw-r--r--   0        0        0     9901 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/reference_pointer.py
+-rw-r--r--   0        0        0    10104 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py
+-rw-r--r--   0        0        0     8614 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/responsible_agent.py
+-rw-r--r--   0        0        0     6443 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic_entity.py
+-rw-r--r--   0        0        0    19946 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/graph/entities/identifier.py
+-rw-r--r--   0        0        0    15326 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/graph/graph_entity.py
+-rw-r--r--   0        0        0    19833 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/graph/graph_set.py
+-rw-r--r--   0        0        0      937 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/metadata/__init__.py
+-rw-r--r--   0        0        0      941 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/metadata/entities/__init__.py
+-rw-r--r--   0        0        0    18784 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/metadata/entities/dataset.py
+-rw-r--r--   0        0        0    12161 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/metadata/entities/distribution.py
+-rw-r--r--   0        0        0     7405 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/metadata/metadata_entity.py
+-rw-r--r--   0        0        0     6411 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/metadata/metadata_set.py
+-rw-r--r--   0        0        0      913 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/prov/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/prov/entities/__init__.py
+-rw-r--r--   0        0        0    13309 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/prov/entities/snapshot_entity.py
+-rw-r--r--   0        0        0     3673 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/prov/prov_entity.py
+-rw-r--r--   0        0        0    16593 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/prov/prov_set.py
+-rw-r--r--   0        0        0    11825 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/reader.py
+-rw-r--r--   0        0        0      822 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/resources/__init__.py
+-rw-r--r--   0        0        0     1361 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/resources/querymap.txt
+-rw-r--r--   0        0        0    20997 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/resources/shacle.ttl
+-rw-r--r--   0        0        0    12150 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/resources/shexc.txt
+-rw-r--r--   0        0        0    12248 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/resources/shexc_closed.txt
+-rw-r--r--   0        0        0    17290 2024-06-02 14:18:36.715939 oc_ocdm-8.1.1/oc_ocdm/storer.py
+-rw-r--r--   0        0        0     1332 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/support/__init__.py
+-rw-r--r--   0        0        0     3460 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/support/query_utils.py
+-rw-r--r--   0        0        0     2550 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/support/reporter.py
+-rw-r--r--   0        0        0    15410 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/support/support.py
+-rw-r--r--   0        0        0      822 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/counter_handler/__init__.py
+-rw-r--r--   0        0        0     8502 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py
+-rw-r--r--   0        0        0    10970 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py
+-rw-r--r--   0        0        0    69632 2024-06-02 14:13:23.213979 oc_ocdm-8.1.1/oc_ocdm/test/coverage/.coverage
+-rw-r--r--   0        0        0      107 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/coverage/.coveragerc
+-rw-r--r--   0        0        0      904 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/coverage/coverage.svg
+-rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/__init__.py
+-rw-r--r--   0        0        0     2608 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py
+-rw-r--r--   0        0        0     2149 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py
+-rw-r--r--   0        0        0    12323 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py
+-rw-r--r--   0        0        0     6730 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_citation.py
+-rw-r--r--   0        0        0     4776 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py
+-rw-r--r--   0        0        0     1856 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py
+-rw-r--r--   0        0        0     1696 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py
+-rw-r--r--   0        0        0     2433 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py
+-rw-r--r--   0        0        0     2908 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py
+-rw-r--r--   0        0        0     2466 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py
+-rw-r--r--   0        0        0     2903 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/test_bibliographic_entity.py
+-rw-r--r--   0        0        0     7908 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/test_identifier.py
+-rw-r--r--   0        0        0      940 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/test_graph_entity.py
+-rw-r--r--   0        0        0     6500 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/graph/test_graph_set.py
+-rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/metadata/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/metadata/entities/__init__.py
+-rw-r--r--   0        0        0     4573 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/metadata/entities/test_dataset.py
+-rw-r--r--   0        0        0     3507 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/metadata/entities/test_distribution.py
+-rw-r--r--   0        0        0     2665 2024-05-19 11:18:15.265698 oc_ocdm-8.1.1/oc_ocdm/test/metadata/test_metadata_set.py
+-rw-r--r--   0        0        0      837 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/prov/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/prov/entities/__init__.py
+-rw-r--r--   0        0        0     4141 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/prov/entities/test_snapshot_entity.py
+-rw-r--r--   0        0        0    12288 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/prov/prov_counter.db
+-rw-r--r--   0        0        0    12789 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/prov/test_prov_set.py
+-rw-r--r--   0        0        0        0 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/reader/__init__.py
+-rw-r--r--   0        0        0     2523 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/reader/br.nt
+-rw-r--r--   0        0        0     1862 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/reader/test_reader.py
+-rw-r--r--   0        0        0      822 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/resources/__init__.py
+-rw-r--r--   0        0        0     6448 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/resources/data.json
+-rw-r--r--   0        0        0     6448 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/resources/data_reader.json
+-rw-r--r--   0        0        0     6449 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/resources/data_reader_invalid.json
+-rw-r--r--   0        0        0     3602 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/resources/test_shacle.py
+-rw-r--r--   0        0        0      826 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/storer/__init__.py
+-rw-r--r--   0        0        0    14739 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/storer/test_storer.py
+-rw-r--r--   0        0        0      837 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/support/__init__.py
+-rw-r--r--   0        0        0     5356 2024-05-19 11:18:15.269698 oc_ocdm-8.1.1/oc_ocdm/test/support/test_support.py
+-rw-r--r--   0        0        0     1558 2024-06-02 14:19:23.019439 oc_ocdm-8.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6442 1970-01-01 00:00:00.000000 oc_ocdm-8.1.1/PKG-INFO
```

### Comparing `oc_ocdm-8.1.0/LICENSE.md` & `oc_ocdm-8.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/README.md` & `oc_ocdm-8.1.1/README.md`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/abstract_entity.py` & `oc_ocdm-8.1.1/oc_ocdm/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/abstract_set.py` & `oc_ocdm-8.1.1/oc_ocdm/abstract_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/counter_handler/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/counter_handler/counter_handler.py` & `oc_ocdm-8.1.1/oc_ocdm/counter_handler/counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/counter_handler/filesystem_counter_handler.py` & `oc_ocdm-8.1.1/oc_ocdm/counter_handler/filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/counter_handler/in_memory_counter_handler.py` & `oc_ocdm-8.1.1/oc_ocdm/counter_handler/in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/counter_handler/sqlite_counter_handler.py` & `oc_ocdm-8.1.1/oc_ocdm/counter_handler/sqlite_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/decorators.py` & `oc_ocdm-8.1.1/oc_ocdm/decorators.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/agent_role.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/agent_role.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/citation.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/citation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/discourse_element.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/discourse_element.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/pointer_list.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/pointer_list.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/reference_annotation.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/reference_annotation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/reference_pointer.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/reference_pointer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic/responsible_agent.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic/responsible_agent.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/bibliographic_entity.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/bibliographic_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/entities/identifier.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/entities/identifier.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/graph_entity.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/graph_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/graph/graph_set.py` & `oc_ocdm-8.1.1/oc_ocdm/graph/graph_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/metadata/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/metadata/entities/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/metadata/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/metadata/entities/dataset.py` & `oc_ocdm-8.1.1/oc_ocdm/metadata/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/metadata/entities/distribution.py` & `oc_ocdm-8.1.1/oc_ocdm/metadata/entities/distribution.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/metadata/metadata_entity.py` & `oc_ocdm-8.1.1/oc_ocdm/metadata/metadata_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/metadata/metadata_set.py` & `oc_ocdm-8.1.1/oc_ocdm/metadata/metadata_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/prov/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/prov/entities/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/prov/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/prov/entities/snapshot_entity.py` & `oc_ocdm-8.1.1/oc_ocdm/prov/entities/snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/prov/prov_entity.py` & `oc_ocdm-8.1.1/oc_ocdm/prov/prov_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/prov/prov_set.py` & `oc_ocdm-8.1.1/oc_ocdm/prov/prov_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/reader.py` & `oc_ocdm-8.1.1/oc_ocdm/reader.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/resources/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/resources/querymap.txt` & `oc_ocdm-8.1.1/oc_ocdm/resources/querymap.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/resources/shacle.ttl` & `oc_ocdm-8.1.1/oc_ocdm/resources/shacle.ttl`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/resources/shexc.txt` & `oc_ocdm-8.1.1/oc_ocdm/resources/shexc.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/resources/shexc_closed.txt` & `oc_ocdm-8.1.1/oc_ocdm/resources/shexc_closed.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/storer.py` & `oc_ocdm-8.1.1/oc_ocdm/storer.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS
 # ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS
 # SOFTWARE.
 from __future__ import annotations
 
 import json
 import os
+import time
 from datetime import datetime
 from typing import TYPE_CHECKING
 from zipfile import ZIP_DEFLATED, ZipFile
 
 from rdflib import ConjunctiveGraph
 from SPARQLWrapper import SPARQLWrapper
 
@@ -307,36 +308,50 @@
     def execute_query(self, query_string: str, triplestore_url: str) -> bool:
         self.repok.new_article()
         self.reperr.new_article()
 
         return self._query(query_string, triplestore_url)
 
     def _query(self, query_string: str, triplestore_url: str, base_dir: str = None,
-               added_statements: int = 0, removed_statements: int = 0) -> bool:
+            added_statements: int = 0, removed_statements: int = 0) -> bool:
         if query_string != "":
-            try:
-                sparql: SPARQLWrapper = SPARQLWrapper(triplestore_url)
-                sparql.setQuery(query_string)
-                sparql.setMethod('POST')
-
-                sparql.query()
-
-                self.repok.add_sentence(
-                    f"Triplestore updated with {added_statements} added statements and "
-                    f"with {removed_statements} removed statements.")
-
-                return True
-
-            except Exception as e:
-                self.reperr.add_sentence("[3] "
-                                         "Graph was not loaded into the "
-                                         f"triplestore due to communication problems: {e}")
-                if base_dir is not None:
-                    tp_err_dir: str = base_dir + os.sep + "tp_err"
-                    if not os.path.exists(tp_err_dir):
-                        os.makedirs(tp_err_dir)
-                    cur_file_err: str = tp_err_dir + os.sep + \
-                        datetime.now().strftime('%Y-%m-%d-%H-%M-%S-%f_not_uploaded.txt')
-                    with open(cur_file_err, 'wt', encoding='utf-8') as f:
-                        f.write(query_string)
+            attempt = 0
+            max_attempts = 3
+            wait_time = 5  # Initial wait time in seconds
+
+            while attempt < max_attempts:
+                try:
+                    sparql: SPARQLWrapper = SPARQLWrapper(triplestore_url)
+                    sparql.setQuery(query_string)
+                    sparql.setMethod('POST')
+
+                    sparql.query()
+
+                    self.repok.add_sentence(
+                        f"Triplestore updated with {added_statements} added statements and "
+                        f"with {removed_statements} removed statements.")
+
+                    return True
+
+                except Exception as e:
+                    attempt += 1
+                    self.reperr.add_sentence("[3] "
+                                            f"Attempt {attempt} failed. Graph was not loaded into the "
+                                            f"triplestore due to communication problems: {e}")
+                    if attempt < max_attempts:
+                        self.reperr.add_sentence(f"Retrying in {wait_time} seconds...")
+                        time.sleep(wait_time)
+                        wait_time *= 2  # Double the wait time for the next attempt
+
+                    if base_dir is not None and attempt == max_attempts:
+                        self.reperr.add_sentence("[3] "
+                                                "Graph was not loaded into the "
+                                                f"triplestore due to communication problems: {e}")
+                        tp_err_dir: str = base_dir + os.sep + "tp_err"
+                        if not os.path.exists(tp_err_dir):
+                            os.makedirs(tp_err_dir)
+                        cur_file_err: str = tp_err_dir + os.sep + \
+                            datetime.now().strftime('%Y-%m-%d-%H-%M-%S-%f_not_uploaded.txt')
+                        with open(cur_file_err, 'wt', encoding='utf-8') as f:
+                            f.write(query_string)
 
         return False
```

### Comparing `oc_ocdm-8.1.0/oc_ocdm/support/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/support/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/support/query_utils.py` & `oc_ocdm-8.1.1/oc_ocdm/support/query_utils.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/support/reporter.py` & `oc_ocdm-8.1.1/oc_ocdm/support/reporter.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/support/support.py` & `oc_ocdm-8.1.1/oc_ocdm/support/support.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/counter_handler/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py` & `oc_ocdm-8.1.1/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py` & `oc_ocdm-8.1.1/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/coverage/.coverage` & `oc_ocdm-8.1.1/oc_ocdm/test/coverage/.coverage`

 * *Files 1% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -14,15 +14,15 @@
     --  'has_arcs' boolean      -- Is this data recording branches?
     --  'sys_argv' text         -- The coverage command line that recorded the data.
     --  'version' text          -- The version of coverage.py that made the file.
     --  'when' text             -- Datetime when the file was created.
 );
 INSERT INTO meta VALUES('sys_argv','[''python -m unittest'', ''discover'', ''-s'', ''oc_ocdm/test'', ''-p'', ''test_*.py'']');
 INSERT INTO meta VALUES('version','6.5.0');
-INSERT INTO meta VALUES('when','2024-04-04 21:08:54');
+INSERT INTO meta VALUES('when','2024-05-19 12:21:31');
 INSERT INTO meta VALUES('has_arcs','0');
 CREATE TABLE file (
     -- A row per file measured.
     id integer primary key,
     path text,
     unique (path)
 );
@@ -122,29 +122,29 @@
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'02');
 INSERT INTO line_bits VALUES(2,1,X'0000cb77affbfdbbffffefdffbfbfbbffd7dfdfdaff704');
 INSERT INTO line_bits VALUES(3,1,X'00000d');
-INSERT INTO line_bits VALUES(4,1,X'00007dfb17a043f13706c60840fc756a036eaeebfdf6beee3f63f8120300dc032edfb207dc0a08feba');
+INSERT INTO line_bits VALUES(4,1,X'00007dfb17a040f13706c60840fc756a036eaeebfdf6beee3f21f8120100dc032edfb207dc0a08faba');
 INSERT INTO line_bits VALUES(5,1,X'000006');
-INSERT INTO line_bits VALUES(6,1,X'000055c1fffffeffffffffffffffffffffffffffffdffff37f63b5e099bbbb9c0200879ba1f301');
+INSERT INTO line_bits VALUES(6,1,X'000055c1fffffeffffffffffffffffffffffffffffdfff937f63b5e099bbbb9c0200879ba1f301');
 INSERT INTO line_bits VALUES(7,1,X'00006d61282e00090a604101408205c002340b00fe029fbbcf06');
 INSERT INTO line_bits VALUES(8,1,X'000062');
-INSERT INTO line_bits VALUES(9,1,X'00007d410900a8f195feafc11bf7defdffa45ce6cc98978097879387938097006060415ef4fae55e0600000080e2ef73');
+INSERT INTO line_bits VALUES(9,1,X'00007d410900a8f195feafc11bf7defdffa45ce6cc98978097879387938097002060411ad4f8e55e0600000080e2ef73');
 INSERT INTO line_bits VALUES(10,1,X'000015fbfdfc121001');
 INSERT INTO line_bits VALUES(11,1,X'000015cc03e73c9cee6b');
-INSERT INTO line_bits VALUES(12,1,X'0000d5456b6dd5f4ffdc87ff5be77af7bbdef5ee77bdfb5def7af7bbdefd5fe9df5700c0f3ffffff02fe02020202020202fe02');
+INSERT INTO line_bits VALUES(12,1,X'0000d5456b6dd5f4ffd487ff5ba77af5ab5ef5ea57bdfa55af7af5abdefd5fe9df5700c0f3ffffff02fe02020202020202fe02');
 INSERT INTO line_bits VALUES(13,1,X'0000ad301405be011880');
-INSERT INTO line_bits VALUES(14,1,X'0000bd7ba432304600000400000200e0f77bfeffdfff8b8b8bb8b84bff9f');
+INSERT INTO line_bits VALUES(14,1,X'0000bd7ba432304600000400000200e0f77bfeffdffe8b8b8bb8b84bfb9f');
 INSERT INTO line_bits VALUES(15,1,X'00000e');
 INSERT INTO line_bits VALUES(16,1,X'0000d9010060000006006000c00060');
-INSERT INTO line_bits VALUES(17,1,X'0000bdcc2c20fb6f0000000200b60080edbdddbbfe8faebd7fb77a7fffa974f7277bf3bd00000002b02100db');
-INSERT INTO line_bits VALUES(18,1,X'0000954cfc0d00c0f66d2900c0be3d0500d8b7cd02806d29005b5200b60c');
+INSERT INTO line_bits VALUES(17,1,X'0000bdcc2c20fb2f0000000208000004006c0100db7bbb77fd1f5d7bff6ef5fefe53e9ee4ff6e67901000004604300b601');
+INSERT INTO line_bits VALUES(18,1,X'0000954cfc0500c0f66d2900c0be3d0500d8b7cd02806d29005b5200b60c');
 INSERT INTO line_bits VALUES(19,1,X'000006');
 INSERT INTO line_bits VALUES(20,1,X'0000556401d020c137003400a40020e1df0d');
 INSERT INTO line_bits VALUES(21,1,X'0000ad1200d03f0c');
 INSERT INTO line_bits VALUES(22,1,X'00002dce1800809ea060030006000d001800a00100038006000d00e006006800001a0034006800d000a00140030006000d001a00f40506');
 INSERT INTO line_bits VALUES(23,1,X'0000fe07');
 INSERT INTO line_bits VALUES(24,1,X'000055cc0600000000821b002c487003c082040bc002b0002c08');
 INSERT INTO line_bits VALUES(25,1,X'00005598c1000000000206008005098001d000000430002c08');
@@ -153,22 +153,22 @@
 INSERT INTO line_bits VALUES(28,1,X'00005598610000000000000103c08204c00068000002180016240006400300100003a0010008180016246000106000001000140014001400140014001400140004');
 INSERT INTO line_bits VALUES(29,1,X'000055cc18000000040cc08204c00068');
 INSERT INTO line_bits VALUES(30,1,X'000055cc800100000430005810');
 INSERT INTO line_bits VALUES(31,1,X'00005598610000000010300058900006000b12c000604102600068');
 INSERT INTO line_bits VALUES(32,1,X'00002dce0c00000000020c000b123000c02948c00000a7200106800509000580');
 INSERT INTO line_bits VALUES(33,1,X'000055660c000000000206000b1230002c48c000b02001064003');
 INSERT INTO line_bits VALUES(34,1,X'000006');
-INSERT INTO line_bits VALUES(35,1,X'0000b5f0f6ff3bffbff1d102605e3313400000000010');
-INSERT INTO line_bits VALUES(36,1,X'0000f54bd3d935eec2bbde5b004bc11710');
+INSERT INTO line_bits VALUES(35,1,X'0000b5f0f6ff3bf1bff1d102605e3313400000000010');
+INSERT INTO line_bits VALUES(36,1,X'0000f54bd3d935aec2ab5e5b004bc11710');
 INSERT INTO line_bits VALUES(37,1,X'000006');
 INSERT INTO line_bits VALUES(38,1,X'000075c10c000000000000000206800509180016246000b02001038005091880060020c0003400000103c08204c0003400000106800509800168');
 INSERT INTO line_bits VALUES(39,1,X'0000d5c20c00000000002060005890800160410206000b123000589080016041020680050918001604');
 INSERT INTO line_bits VALUES(40,1,X'000006');
-INSERT INTO line_bits VALUES(41,1,X'0000d58241ffcdef633477');
-INSERT INTO line_bits VALUES(42,1,X'0000dd45ebd1bcffd771fbfbeeef9f6d59766fbfff992e77fbdb0f00006f01807cb7eee7bd02');
+INSERT INTO line_bits VALUES(41,1,X'0000d58241ff4dec633477');
+INSERT INTO line_bits VALUES(42,1,X'0000dd45ebd1bcffd771fbfbeeef9f6d19766fbfff992e77fbdb0f00006d01807cb7eee7bd02');
 INSERT INTO line_bits VALUES(43,1,X'000002');
 INSERT INTO line_bits VALUES(44,1,X'0000d50583a0018005091a00b020c102c08204b701d000000418002c48d00060418206002c48b001b020');
 INSERT INTO line_bits VALUES(45,1,X'0000ca041e0100023e080092');
 INSERT INTO line_bits VALUES(46,1,X'0000a5bdbffffdefbff7fbefbfbff7f7bffffdfbfefe7dbfdff7f727');
 INSERT INTO line_bits VALUES(47,1,X'02');
 INSERT INTO line_bits VALUES(48,1,X'02');
 INSERT INTO line_bits VALUES(49,1,X'02');
```

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/coverage/coverage.svg` & `oc_ocdm-8.1.1/oc_ocdm/test/coverage/coverage.svg`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_citation.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_citation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/test_bibliographic_entity.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/test_bibliographic_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/entities/test_identifier.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/entities/test_identifier.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/test_graph_entity.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/test_graph_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/graph/test_graph_set.py` & `oc_ocdm-8.1.1/oc_ocdm/test/graph/test_graph_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/metadata/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/metadata/entities/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/metadata/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/metadata/entities/test_dataset.py` & `oc_ocdm-8.1.1/oc_ocdm/test/metadata/entities/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/metadata/entities/test_distribution.py` & `oc_ocdm-8.1.1/oc_ocdm/test/metadata/entities/test_distribution.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/metadata/test_metadata_set.py` & `oc_ocdm-8.1.1/oc_ocdm/test/metadata/test_metadata_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/prov/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/prov/entities/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/prov/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/prov/entities/test_snapshot_entity.py` & `oc_ocdm-8.1.1/oc_ocdm/test/prov/entities/test_snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/prov/prov_counter.db` & `oc_ocdm-8.1.1/oc_ocdm/test/prov/prov_counter.db`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/prov/test_prov_set.py` & `oc_ocdm-8.1.1/oc_ocdm/test/prov/test_prov_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/reader/br.nt` & `oc_ocdm-8.1.1/oc_ocdm/test/reader/br.nt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/reader/test_reader.py` & `oc_ocdm-8.1.1/oc_ocdm/test/reader/test_reader.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/resources/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/resources/data.json` & `oc_ocdm-8.1.1/oc_ocdm/test/resources/data.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/resources/data_reader.json` & `oc_ocdm-8.1.1/oc_ocdm/test/resources/data_reader.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/resources/data_reader_invalid.json` & `oc_ocdm-8.1.1/oc_ocdm/test/resources/data_reader_invalid.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/resources/test_shacle.py` & `oc_ocdm-8.1.1/oc_ocdm/test/resources/test_shacle.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/storer/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/storer/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/storer/test_storer.py` & `oc_ocdm-8.1.1/oc_ocdm/test/storer/test_storer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/support/__init__.py` & `oc_ocdm-8.1.1/oc_ocdm/test/support/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/oc_ocdm/test/support/test_support.py` & `oc_ocdm-8.1.1/oc_ocdm/test/support/test_support.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-8.1.0/pyproject.toml` & `oc_ocdm-8.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oc_ocdm"
-version = "8.1.0"
+version = "8.1.1"
 description = "Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel."
 authors = [
     "Silvio Peroni <essepuntato@gmail.com>",
     "Marilena Daquino <marilena.daquino2@unibo.it>",
     "Fabio Mariani <fabio.mariani6@studio.unibo.it>",
     "Simone Persiani <iosonopersia@gmail.com>",
     "Arcangelo Massari <arcangelo.massari@unibo.it>"
```

### Comparing `oc_ocdm-8.1.0/PKG-INFO` & `oc_ocdm-8.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oc_ocdm
-Version: 8.1.0
+Version: 8.1.1
 Summary: Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel.
 Home-page: https://opencitations.net
 License: ISC
 Keywords: opencitations,openscience,datamodel,mapping
 Author: Silvio Peroni
 Author-email: essepuntato@gmail.com
 Requires-Python: >=3.8,<4.0
```

