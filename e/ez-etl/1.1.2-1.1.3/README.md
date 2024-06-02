# Comparing `tmp/ez-etl-1.1.2.tar.gz` & `tmp/ez-etl-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-etl-1.1.2.tar", last modified: Fri Mar  1 06:52:27 2024, max compression
+gzip compressed data, was "ez-etl-1.1.3.tar", last modified: Sun Jun  2 16:47:12 2024, max compression
```

## Comparing `ez-etl-1.1.2.tar` & `ez-etl-1.1.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-03-01 06:52:27.661941 ez-etl-1.1.2/
--rw-r--r--   0 xuwei      (501) staff       (20)    11357 2023-08-09 02:31:39.000000 ez-etl-1.1.2/LICENSE
--rw-r--r--   0 xuwei      (501) staff       (20)     1748 2024-03-01 06:52:27.661608 ez-etl-1.1.2/PKG-INFO
--rw-r--r--   0 xuwei      (501) staff       (20)     8444 2023-11-23 13:46:29.000000 ez-etl-1.1.2/README.md
-drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-03-01 06:52:27.635187 ez-etl-1.1.2/ez_etl.egg-info/
--rw-r--r--   0 xuwei      (501) staff       (20)     1748 2024-03-01 06:52:27.000000 ez-etl-1.1.2/ez_etl.egg-info/PKG-INFO
--rw-r--r--   0 xuwei      (501) staff       (20)     2355 2024-03-01 06:52:27.000000 ez-etl-1.1.2/ez_etl.egg-info/SOURCES.txt
--rw-r--r--   0 xuwei      (501) staff       (20)        1 2024-03-01 06:52:27.000000 ez-etl-1.1.2/ez_etl.egg-info/dependency_links.txt
--rw-r--r--   0 xuwei      (501) staff       (20)        1 2024-03-01 06:52:27.000000 ez-etl-1.1.2/ez_etl.egg-info/not-zip-safe
--rw-r--r--   0 xuwei      (501) staff       (20)      432 2024-03-01 06:52:27.000000 ez-etl-1.1.2/ez_etl.egg-info/requires.txt
--rw-r--r--   0 xuwei      (501) staff       (20)        6 2024-03-01 06:52:27.000000 ez-etl-1.1.2/ez_etl.egg-info/top_level.txt
-drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-03-01 06:52:27.635742 ez-etl-1.1.2/ezetl/
--rw-r--r--   0 xuwei      (501) staff       (20)     5266 2023-11-23 13:18:09.000000 ez-etl-1.1.2/ezetl/__init__.py
-drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-03-01 06:52:27.645331 ez-etl-1.1.2/ezetl/data_models/
--rw-r--r--   0 xuwei      (501) staff       (20)     2122 2024-01-10 03:44:51.000000 ez-etl-1.1.2/ezetl/data_models/__init__.py
--rw-r--r--   0 xuwei      (501) staff       (20)     5914 2023-11-21 08:09:28.000000 ez-etl-1.1.2/ezetl/data_models/akshare_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)     4573 2024-01-10 08:14:57.000000 ez-etl-1.1.2/ezetl/data_models/base_db_sql.py
--rw-r--r--   0 xuwei      (501) staff       (20)    14383 2023-11-24 07:57:09.000000 ez-etl-1.1.2/ezetl/data_models/base_db_table.py
--rw-r--r--   0 xuwei      (501) staff       (20)     7754 2023-11-22 02:09:55.000000 ez-etl-1.1.2/ezetl/data_models/ccxt_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)     2490 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/data_models/clickhouse_table.py
--rw-r--r--   0 xuwei      (501) staff       (20)    12124 2024-03-01 06:51:56.000000 ez-etl-1.1.2/ezetl/data_models/elasticsearch_index.py
--rw-r--r--   0 xuwei      (501) staff       (20)     9971 2024-01-10 09:57:02.000000 ez-etl-1.1.2/ezetl/data_models/file_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)      426 2023-11-24 09:04:41.000000 ez-etl-1.1.2/ezetl/data_models/hdfs_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)     1791 2023-11-24 07:55:28.000000 ez-etl-1.1.2/ezetl/data_models/hive_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)     4252 2024-01-11 09:13:20.000000 ez-etl-1.1.2/ezetl/data_models/http_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)    12775 2024-01-11 01:41:43.000000 ez-etl-1.1.2/ezetl/data_models/ixdb_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)     6096 2024-01-11 06:15:17.000000 ez-etl-1.1.2/ezetl/data_models/kafka_topic.py
--rw-r--r--   0 xuwei      (501) staff       (20)     9809 2023-09-12 10:26:28.000000 ez-etl-1.1.2/ezetl/data_models/minio_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)     9529 2024-01-11 07:23:39.000000 ez-etl-1.1.2/ezetl/data_models/mongo_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)     6441 2023-08-14 03:35:31.000000 ez-etl-1.1.2/ezetl/data_models/mysql_binlog.py
--rw-r--r--   0 xuwei      (501) staff       (20)      550 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/data_models/mysql_table.py
--rw-r--r--   0 xuwei      (501) staff       (20)    11813 2024-01-11 08:07:03.000000 ez-etl-1.1.2/ezetl/data_models/neo4j_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)     2170 2024-01-10 08:12:50.000000 ez-etl-1.1.2/ezetl/data_models/oracle_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)      827 2024-01-10 08:12:59.000000 ez-etl-1.1.2/ezetl/data_models/pgsql_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)     8361 2023-09-26 06:06:47.000000 ez-etl-1.1.2/ezetl/data_models/prometheus_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)    10534 2024-01-11 08:48:23.000000 ez-etl-1.1.2/ezetl/data_models/redis_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)     4130 2023-11-24 07:57:09.000000 ez-etl-1.1.2/ezetl/data_models/sqlserver_models.py
--rw-r--r--   0 xuwei      (501) staff       (20)     8478 2023-10-21 17:47:33.000000 ez-etl-1.1.2/ezetl/etl_task.py
-drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-03-01 06:52:27.646347 ez-etl-1.1.2/ezetl/examples/
--rw-r--r--   0 xuwei      (501) staff       (20)        0 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/__init__.py
-drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-03-01 06:52:27.648528 ez-etl-1.1.2/ezetl/examples/etl_demos/
--rw-r--r--   0 xuwei      (501) staff       (20)        0 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/etl_demos/__init__.py
--rw-r--r--   0 xuwei      (501) staff       (20)     1739 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/etl_demos/binlog2kafka.py
--rw-r--r--   0 xuwei      (501) staff       (20)     2321 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/etl_demos/csv2csv.py
--rw-r--r--   0 xuwei      (501) staff       (20)     4308 2023-11-22 09:12:00.000000 ez-etl-1.1.2/ezetl/examples/etl_demos/csv2mysql.py
--rw-r--r--   0 xuwei      (501) staff       (20)     2474 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/etl_demos/kafka2es.py
--rw-r--r--   0 xuwei      (501) staff       (20)     2242 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/etl_demos/kafka2ixdb.py
--rw-r--r--   0 xuwei      (501) staff       (20)     2673 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/etl_demos/mysql2es.py
--rw-r--r--   0 xuwei      (501) staff       (20)     1750 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/etl_demos/mysql2kafka.py
--rw-r--r--   0 xuwei      (501) staff       (20)     1982 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/etl_demos/mysql2mongodb.py
--rw-r--r--   0 xuwei      (501) staff       (20)     1752 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/etl_demos/mysql2n4j.py
-drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-03-01 06:52:27.649564 ez-etl-1.1.2/ezetl/examples/etl_task/
--rw-r--r--   0 xuwei      (501) staff       (20)        0 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/etl_task/__init__.py
--rw-r--r--   0 xuwei      (501) staff       (20)     2297 2023-08-09 03:19:52.000000 ez-etl-1.1.2/ezetl/examples/etl_task/batch_task_demo.py
--rw-r--r--   0 xuwei      (501) staff       (20)     2539 2023-08-09 03:19:52.000000 ez-etl-1.1.2/ezetl/examples/etl_task/etl_process_task_demo.py
--rw-r--r--   0 xuwei      (501) staff       (20)     2171 2023-11-21 07:14:24.000000 ez-etl-1.1.2/ezetl/examples/etl_task/stream_task_demo.py
-drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-03-01 06:52:27.652109 ez-etl-1.1.2/ezetl/examples/reader/
--rw-r--r--   0 xuwei      (501) staff       (20)        0 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/reader/__init__.py
--rw-r--r--   0 xuwei      (501) staff       (20)      659 2023-08-12 02:25:02.000000 ez-etl-1.1.2/ezetl/examples/reader/read_csv.py
--rw-r--r--   0 xuwei      (501) staff       (20)      851 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/reader/read_es.py
--rw-r--r--   0 xuwei      (501) staff       (20)      697 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/reader/read_kafka.py
--rw-r--r--   0 xuwei      (501) staff       (20)      882 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/reader/read_mongodb.py
--rw-r--r--   0 xuwei      (501) staff       (20)      910 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/reader/read_mysql.py
--rw-r--r--   0 xuwei      (501) staff       (20)      848 2023-08-11 03:05:19.000000 ez-etl-1.1.2/ezetl/examples/reader/read_mysql_binlog.py
--rw-r--r--   0 xuwei      (501) staff       (20)      821 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/examples/reader/read_n4j.py
-drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-03-01 06:52:27.654740 ez-etl-1.1.2/ezetl/libs/
--rw-r--r--   0 xuwei      (501) staff       (20)        0 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/libs/__init__.py
--rw-r--r--   0 xuwei      (501) staff       (20)    10750 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/libs/es.py
--rw-r--r--   0 xuwei      (501) staff       (20)     3214 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/libs/hdfs.py
--rw-r--r--   0 xuwei      (501) staff       (20)     4637 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/libs/ixdb.py
--rw-r--r--   0 xuwei      (501) staff       (20)     4496 2024-01-11 06:50:07.000000 ez-etl-1.1.2/ezetl/libs/kafka_utils.py
--rw-r--r--   0 xuwei      (501) staff       (20)     4583 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/libs/n4j.py
--rw-r--r--   0 xuwei      (501) staff       (20)     1139 2023-09-26 05:51:03.000000 ez-etl-1.1.2/ezetl/libs/prometheus.py
-drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-03-01 06:52:27.656872 ez-etl-1.1.2/ezetl/transform_algs/
--rw-r--r--   0 xuwei      (501) staff       (20)     1125 2023-08-10 07:28:08.000000 ez-etl-1.1.2/ezetl/transform_algs/__init__.py
--rw-r--r--   0 xuwei      (501) staff       (20)     6403 2024-01-10 03:24:29.000000 ez-etl-1.1.2/ezetl/transform_algs/content_algs.py
--rw-r--r--   0 xuwei      (501) staff       (20)     2307 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/transform_algs/count_algs.py
--rw-r--r--   0 xuwei      (501) staff       (20)     3978 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/transform_algs/filter_algs.py
--rw-r--r--   0 xuwei      (501) staff       (20)    10713 2023-08-10 07:20:28.000000 ez-etl-1.1.2/ezetl/transform_algs/map_algs.py
-drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-03-01 06:52:27.659905 ez-etl-1.1.2/ezetl/utils/
--rw-r--r--   0 xuwei      (501) staff       (20)     2465 2023-11-23 11:07:43.000000 ez-etl-1.1.2/ezetl/utils/__init__.py
--rw-r--r--   0 xuwei      (501) staff       (20)    16329 2023-09-05 10:25:15.000000 ez-etl-1.1.2/ezetl/utils/common_utils.py
--rw-r--r--   0 xuwei      (501) staff       (20)     6194 2023-11-24 08:07:48.000000 ez-etl-1.1.2/ezetl/utils/db_utils.py
--rw-r--r--   0 xuwei      (501) staff       (20)    22732 2023-09-05 08:21:50.000000 ez-etl-1.1.2/ezetl/utils/es_query_tool.py
--rw-r--r--   0 xuwei      (501) staff       (20)     2658 2023-08-09 02:31:39.000000 ez-etl-1.1.2/ezetl/utils/es_utils.py
--rw-r--r--   0 xuwei      (501) staff       (20)       38 2024-03-01 06:52:27.662013 ez-etl-1.1.2/setup.cfg
--rw-r--r--   0 xuwei      (501) staff       (20)     1717 2024-03-01 06:52:25.000000 ez-etl-1.1.2/setup.py
+drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-06-02 16:47:12.867051 ez-etl-1.1.3/
+-rw-r--r--   0 xuwei      (501) staff       (20)    11357 2023-08-09 02:31:39.000000 ez-etl-1.1.3/LICENSE
+-rw-r--r--   0 xuwei      (501) staff       (20)     1748 2024-06-02 16:47:12.866807 ez-etl-1.1.3/PKG-INFO
+-rw-r--r--   0 xuwei      (501) staff       (20)     8444 2023-11-23 13:46:29.000000 ez-etl-1.1.3/README.md
+drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-06-02 16:47:12.850152 ez-etl-1.1.3/ez_etl.egg-info/
+-rw-r--r--   0 xuwei      (501) staff       (20)     1748 2024-06-02 16:47:12.000000 ez-etl-1.1.3/ez_etl.egg-info/PKG-INFO
+-rw-r--r--   0 xuwei      (501) staff       (20)     2355 2024-06-02 16:47:12.000000 ez-etl-1.1.3/ez_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 xuwei      (501) staff       (20)        1 2024-06-02 16:47:12.000000 ez-etl-1.1.3/ez_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 xuwei      (501) staff       (20)        1 2024-06-02 16:47:12.000000 ez-etl-1.1.3/ez_etl.egg-info/not-zip-safe
+-rw-r--r--   0 xuwei      (501) staff       (20)      432 2024-06-02 16:47:12.000000 ez-etl-1.1.3/ez_etl.egg-info/requires.txt
+-rw-r--r--   0 xuwei      (501) staff       (20)        6 2024-06-02 16:47:12.000000 ez-etl-1.1.3/ez_etl.egg-info/top_level.txt
+drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-06-02 16:47:12.850553 ez-etl-1.1.3/ezetl/
+-rw-r--r--   0 xuwei      (501) staff       (20)     5266 2023-11-23 13:18:09.000000 ez-etl-1.1.3/ezetl/__init__.py
+drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-06-02 16:47:12.857819 ez-etl-1.1.3/ezetl/data_models/
+-rw-r--r--   0 xuwei      (501) staff       (20)     2122 2024-01-10 03:44:51.000000 ez-etl-1.1.3/ezetl/data_models/__init__.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     5914 2023-11-21 08:09:28.000000 ez-etl-1.1.3/ezetl/data_models/akshare_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     5251 2024-06-02 16:47:03.000000 ez-etl-1.1.3/ezetl/data_models/base_db_sql.py
+-rw-r--r--   0 xuwei      (501) staff       (20)    14748 2024-03-27 06:55:04.000000 ez-etl-1.1.3/ezetl/data_models/base_db_table.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     7754 2023-11-22 02:09:55.000000 ez-etl-1.1.3/ezetl/data_models/ccxt_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     2490 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/data_models/clickhouse_table.py
+-rw-r--r--   0 xuwei      (501) staff       (20)    12124 2024-03-01 06:51:56.000000 ez-etl-1.1.3/ezetl/data_models/elasticsearch_index.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     9971 2024-01-10 09:57:02.000000 ez-etl-1.1.3/ezetl/data_models/file_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)      426 2023-11-24 09:04:41.000000 ez-etl-1.1.3/ezetl/data_models/hdfs_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     1791 2023-11-24 07:55:28.000000 ez-etl-1.1.3/ezetl/data_models/hive_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     4252 2024-01-11 09:13:20.000000 ez-etl-1.1.3/ezetl/data_models/http_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)    12775 2024-01-11 01:41:43.000000 ez-etl-1.1.3/ezetl/data_models/ixdb_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     6096 2024-01-11 06:15:17.000000 ez-etl-1.1.3/ezetl/data_models/kafka_topic.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     9809 2023-09-12 10:26:28.000000 ez-etl-1.1.3/ezetl/data_models/minio_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     9529 2024-01-11 07:23:39.000000 ez-etl-1.1.3/ezetl/data_models/mongo_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     6441 2023-08-14 03:35:31.000000 ez-etl-1.1.3/ezetl/data_models/mysql_binlog.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     1133 2024-06-02 16:47:03.000000 ez-etl-1.1.3/ezetl/data_models/mysql_table.py
+-rw-r--r--   0 xuwei      (501) staff       (20)    11813 2024-01-11 08:07:03.000000 ez-etl-1.1.3/ezetl/data_models/neo4j_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     2170 2024-01-10 08:12:50.000000 ez-etl-1.1.3/ezetl/data_models/oracle_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)      827 2024-01-10 08:12:59.000000 ez-etl-1.1.3/ezetl/data_models/pgsql_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     8361 2023-09-26 06:06:47.000000 ez-etl-1.1.3/ezetl/data_models/prometheus_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)    10534 2024-01-11 08:48:23.000000 ez-etl-1.1.3/ezetl/data_models/redis_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     4130 2023-11-24 07:57:09.000000 ez-etl-1.1.3/ezetl/data_models/sqlserver_models.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     8478 2023-10-21 17:47:33.000000 ez-etl-1.1.3/ezetl/etl_task.py
+drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-06-02 16:47:12.858081 ez-etl-1.1.3/ezetl/examples/
+-rw-r--r--   0 xuwei      (501) staff       (20)        0 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/__init__.py
+drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-06-02 16:47:12.859794 ez-etl-1.1.3/ezetl/examples/etl_demos/
+-rw-r--r--   0 xuwei      (501) staff       (20)        0 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/etl_demos/__init__.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     1739 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/etl_demos/binlog2kafka.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     2321 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/etl_demos/csv2csv.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     4308 2023-11-22 09:12:00.000000 ez-etl-1.1.3/ezetl/examples/etl_demos/csv2mysql.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     2474 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/etl_demos/kafka2es.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     2242 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/etl_demos/kafka2ixdb.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     2673 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/etl_demos/mysql2es.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     1750 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/etl_demos/mysql2kafka.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     1982 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/etl_demos/mysql2mongodb.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     1752 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/etl_demos/mysql2n4j.py
+drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-06-02 16:47:12.860516 ez-etl-1.1.3/ezetl/examples/etl_task/
+-rw-r--r--   0 xuwei      (501) staff       (20)        0 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/etl_task/__init__.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     2297 2023-08-09 03:19:52.000000 ez-etl-1.1.3/ezetl/examples/etl_task/batch_task_demo.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     2539 2023-08-09 03:19:52.000000 ez-etl-1.1.3/ezetl/examples/etl_task/etl_process_task_demo.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     2171 2023-11-21 07:14:24.000000 ez-etl-1.1.3/ezetl/examples/etl_task/stream_task_demo.py
+drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-06-02 16:47:12.861930 ez-etl-1.1.3/ezetl/examples/reader/
+-rw-r--r--   0 xuwei      (501) staff       (20)        0 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/reader/__init__.py
+-rw-r--r--   0 xuwei      (501) staff       (20)      659 2023-08-12 02:25:02.000000 ez-etl-1.1.3/ezetl/examples/reader/read_csv.py
+-rw-r--r--   0 xuwei      (501) staff       (20)      851 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/reader/read_es.py
+-rw-r--r--   0 xuwei      (501) staff       (20)      697 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/reader/read_kafka.py
+-rw-r--r--   0 xuwei      (501) staff       (20)      882 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/reader/read_mongodb.py
+-rw-r--r--   0 xuwei      (501) staff       (20)      910 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/reader/read_mysql.py
+-rw-r--r--   0 xuwei      (501) staff       (20)      848 2023-08-11 03:05:19.000000 ez-etl-1.1.3/ezetl/examples/reader/read_mysql_binlog.py
+-rw-r--r--   0 xuwei      (501) staff       (20)      821 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/examples/reader/read_n4j.py
+drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-06-02 16:47:12.863071 ez-etl-1.1.3/ezetl/libs/
+-rw-r--r--   0 xuwei      (501) staff       (20)        0 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/libs/__init__.py
+-rw-r--r--   0 xuwei      (501) staff       (20)    10750 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/libs/es.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     3214 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/libs/hdfs.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     4637 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/libs/ixdb.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     4496 2024-01-11 06:50:07.000000 ez-etl-1.1.3/ezetl/libs/kafka_utils.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     4583 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/libs/n4j.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     1139 2023-09-26 05:51:03.000000 ez-etl-1.1.3/ezetl/libs/prometheus.py
+drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-06-02 16:47:12.864106 ez-etl-1.1.3/ezetl/transform_algs/
+-rw-r--r--   0 xuwei      (501) staff       (20)     1125 2023-08-10 07:28:08.000000 ez-etl-1.1.3/ezetl/transform_algs/__init__.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     6403 2024-01-10 03:24:29.000000 ez-etl-1.1.3/ezetl/transform_algs/content_algs.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     2307 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/transform_algs/count_algs.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     3978 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/transform_algs/filter_algs.py
+-rw-r--r--   0 xuwei      (501) staff       (20)    10713 2023-08-10 07:20:28.000000 ez-etl-1.1.3/ezetl/transform_algs/map_algs.py
+drwxr-xr-x   0 xuwei      (501) staff       (20)        0 2024-06-02 16:47:12.865498 ez-etl-1.1.3/ezetl/utils/
+-rw-r--r--   0 xuwei      (501) staff       (20)     2465 2023-11-23 11:07:43.000000 ez-etl-1.1.3/ezetl/utils/__init__.py
+-rw-r--r--   0 xuwei      (501) staff       (20)    16329 2023-09-05 10:25:15.000000 ez-etl-1.1.3/ezetl/utils/common_utils.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     6194 2023-11-24 08:07:48.000000 ez-etl-1.1.3/ezetl/utils/db_utils.py
+-rw-r--r--   0 xuwei      (501) staff       (20)    23057 2024-04-07 07:04:07.000000 ez-etl-1.1.3/ezetl/utils/es_query_tool.py
+-rw-r--r--   0 xuwei      (501) staff       (20)     2658 2023-08-09 02:31:39.000000 ez-etl-1.1.3/ezetl/utils/es_utils.py
+-rw-r--r--   0 xuwei      (501) staff       (20)       38 2024-06-02 16:47:12.867103 ez-etl-1.1.3/setup.cfg
+-rw-r--r--   0 xuwei      (501) staff       (20)     1717 2024-06-02 16:47:03.000000 ez-etl-1.1.3/setup.py
```

### Comparing `ez-etl-1.1.2/LICENSE` & `ez-etl-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/PKG-INFO` & `ez-etl-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-etl
-Version: 1.1.2
+Version: 1.1.3
 Summary: ez-etl is an open-source Extract, Transform, load (ETL) library written in Python. Just configure a dict to read data from various data sources. Use code or built-in conversion algorithms to transform the data into the target data format， and write it to the target data source. 
 Author: Xu Wei
 Author-email: 1013104194@qq.com
 License: Apache License 2.0
 Keywords: etl,extract,transform,load,excel,csv,mysql,kafka,elasticsearch,neo4j,influxdb,mongodb,clickhouse
 License-File: LICENSE
 Requires-Dist: requests>=2.25.1
@@ -12,15 +12,15 @@
 Requires-Dist: python-dateutil
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: openpyxl
 Requires-Dist: xlrd
 Requires-Dist: minio==7.1.1
 Requires-Dist: sqlalchemy>=1.2.0
 Requires-Dist: pymysql
-Requires-Dist: elasticsearch>=7.17.2
+Requires-Dist: elasticsearch>=7.15.2
 Requires-Dist: redis==4.0.2
 Requires-Dist: kafka-python==2.0.2
 Requires-Dist: mysql-replication==0.27
 Requires-Dist: minio==7.1.1
 Provides-Extra: all
 Requires-Dist: xorbits==0.3.2; extra == "all"
 Requires-Dist: pyarrow>=5.0.0; extra == "all"
```

### Comparing `ez-etl-1.1.2/README.md` & `ez-etl-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ez_etl.egg-info/PKG-INFO` & `ez-etl-1.1.3/ez_etl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-etl
-Version: 1.1.2
+Version: 1.1.3
 Summary: ez-etl is an open-source Extract, Transform, load (ETL) library written in Python. Just configure a dict to read data from various data sources. Use code or built-in conversion algorithms to transform the data into the target data format， and write it to the target data source. 
 Author: Xu Wei
 Author-email: 1013104194@qq.com
 License: Apache License 2.0
 Keywords: etl,extract,transform,load,excel,csv,mysql,kafka,elasticsearch,neo4j,influxdb,mongodb,clickhouse
 License-File: LICENSE
 Requires-Dist: requests>=2.25.1
@@ -12,15 +12,15 @@
 Requires-Dist: python-dateutil
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: openpyxl
 Requires-Dist: xlrd
 Requires-Dist: minio==7.1.1
 Requires-Dist: sqlalchemy>=1.2.0
 Requires-Dist: pymysql
-Requires-Dist: elasticsearch>=7.17.2
+Requires-Dist: elasticsearch>=7.15.2
 Requires-Dist: redis==4.0.2
 Requires-Dist: kafka-python==2.0.2
 Requires-Dist: mysql-replication==0.27
 Requires-Dist: minio==7.1.1
 Provides-Extra: all
 Requires-Dist: xorbits==0.3.2; extra == "all"
 Requires-Dist: pyarrow>=5.0.0; extra == "all"
```

### Comparing `ez-etl-1.1.2/ez_etl.egg-info/SOURCES.txt` & `ez-etl-1.1.3/ez_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/__init__.py` & `ez-etl-1.1.3/ezetl/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/__init__.py` & `ez-etl-1.1.3/ezetl/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/akshare_models.py` & `ez-etl-1.1.3/ezetl/data_models/akshare_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/base_db_sql.py` & `ez-etl-1.1.3/ezetl/data_models/base_db_sql.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ezetl.data_models import DataModel
 from ezetl.utils.db_utils import get_database_engine
 from ezetl.utils.common_utils import gen_json_response
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy import text, MetaData
+from sqlalchemy.schema import CreateTable, Table
 
 
 class BaseDBSqlModel(DataModel):
 
     def __init__(self, model_info):
         super().__init__(model_info)
         self.db_type = self._source.get('type')
@@ -29,14 +30,33 @@
             if flag:
                 return True, '连接成功'
             else:
                 return False, '连接失败'
         except Exception as e:
             return False, f'{e}'
 
+    def get_metadata(self):
+        '''
+        获取数据库元数据信息
+        '''
+        metadata = MetaData()
+        metadata.reflect(bind=self.db_engine)
+        create_sql_list = []
+        for table_name in metadata.tables:
+            table = Table(table_name, metadata, autoload_with=self.db_engine)
+            create_sql = str(CreateTable(table).compile(self.db_engine))
+            create_sql_list.append(create_sql)
+        tables_info = '\n'.join(create_sql_list)
+        metadata_info = f"""
+数据源类型: {self.db_type}
+各数据表结构信息:
+{tables_info}
+        """
+        return metadata_info
+
     def gen_models(self):
         '''
         生成子数据模型
         '''
         metadata = MetaData()
         metadata.reflect(bind=self.db_engine)
         model_list = []
```

### Comparing `ez-etl-1.1.2/ezetl/data_models/base_db_table.py` & `ez-etl-1.1.3/ezetl/data_models/base_db_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from ezetl.data_models import DataModel
 from ezetl.utils.db_utils import get_database_engine, get_database_model
 from ezetl.utils.common_utils import trans_rule_value, gen_json_response
-from sqlalchemy import not_
+from sqlalchemy import not_, inspect, MetaData
 from sqlalchemy.sql.schema import Table
 from sqlalchemy import Column, String, Integer, Text, SmallInteger, DateTime, TIMESTAMP, Float
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.schema import CreateTable
 
 
 class BaseDBTableModel(DataModel):
+    '''
+    '''
 
     def __init__(self, model_info):
         super().__init__(model_info)
         self.db_type = self._source.get('type')
         self.conn_conf = self._source['conn_conf']
         self.conn_conf['type'] = self.db_type
         model_conf = self._model['model_conf']
@@ -54,14 +56,27 @@
             if self.table is not None:
                 return True, '连接成功'
             else:
                 return False, '连接失败'
         except Exception as e:
             return False, str(e)[:100]
 
+    def get_metadata(self):
+        '''
+        获取数据库元数据信息
+        '''
+        create_sql = str(CreateTable(self.table).compile(self.db_engine))
+        print(create_sql)
+        metadata_info = f"""
+数据源类型: {self.db_type}
+各数据表结构信息:
+{create_sql}
+        """
+        return metadata_info
+
     def get_res_fields(self):
         '''
         获取字段列表
         '''
         res_fields = []
         try:
             for column in self.table.columns:
@@ -177,15 +192,16 @@
             return False, str(e)
 
     def check_field(self, field_info, res_fields):
         '''
         检察字段是否存在且一致
         '''
         for field in res_fields:
-            if field['field_value'] == field_info['field_value'] and field['type'] == field_info['type'] and field['length'] == field_info['length'] and field['nullable'] == field_info['nullable']:
+            if field['field_value'] == field_info['field_value'] and field['type'] == field_info['type'] and field[
+                'length'] == field_info['length'] and field['nullable'] == field_info['nullable']:
                 print(field_info, field)
                 return True
         return False
 
     def set_field(self, field):
         '''
         设置字段
@@ -217,42 +233,42 @@
         '''
         获取可筛选项
         :return:
         '''
         rules = [{
             'name': '等于',
             'value': 'equal',
-          }, {
+        }, {
             'name': '不等于',
             'value': 'f_equal'
-          }, {
+        }, {
             'name': '包含',
             'value': 'contain'
-          }, {
+        }, {
             'name': '不包含',
             'value': 'f_contain'
-          }, {
+        }, {
             'name': '大于',
             'value': 'gt'
-          }, {
+        }, {
             'name': '大于等于',
             'value': 'gte'
-          }, {
+        }, {
             'name': '小于',
             'value': 'lt'
-          }, {
+        }, {
             'name': '小于等于',
             'value': 'lte'
-          }, {
+        }, {
             'name': '从大到小排序',
             'value': 'sort_desc'
-          }, {
+        }, {
             'name': '从小到大排序',
             'value': 'sort_asc'
-          }
+        }
         ]
         return rules
 
     def gen_extract_rules(self, model):
         '''
         解析筛选规则
         :return:
```

### Comparing `ez-etl-1.1.2/ezetl/data_models/ccxt_models.py` & `ez-etl-1.1.3/ezetl/data_models/ccxt_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/clickhouse_table.py` & `ez-etl-1.1.3/ezetl/data_models/clickhouse_table.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/elasticsearch_index.py` & `ez-etl-1.1.3/ezetl/data_models/elasticsearch_index.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/file_models.py` & `ez-etl-1.1.3/ezetl/data_models/file_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/hive_models.py` & `ez-etl-1.1.3/ezetl/data_models/hive_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/http_models.py` & `ez-etl-1.1.3/ezetl/data_models/http_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/ixdb_models.py` & `ez-etl-1.1.3/ezetl/data_models/ixdb_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/kafka_topic.py` & `ez-etl-1.1.3/ezetl/data_models/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/minio_models.py` & `ez-etl-1.1.3/ezetl/data_models/minio_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/mongo_models.py` & `ez-etl-1.1.3/ezetl/data_models/mongo_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/mysql_binlog.py` & `ez-etl-1.1.3/ezetl/data_models/mysql_binlog.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/neo4j_models.py` & `ez-etl-1.1.3/ezetl/data_models/neo4j_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/oracle_models.py` & `ez-etl-1.1.3/ezetl/data_models/oracle_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/pgsql_models.py` & `ez-etl-1.1.3/ezetl/data_models/pgsql_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/prometheus_models.py` & `ez-etl-1.1.3/ezetl/data_models/prometheus_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/redis_models.py` & `ez-etl-1.1.3/ezetl/data_models/redis_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/data_models/sqlserver_models.py` & `ez-etl-1.1.3/ezetl/data_models/sqlserver_models.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/etl_task.py` & `ez-etl-1.1.3/ezetl/etl_task.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_demos/binlog2kafka.py` & `ez-etl-1.1.3/ezetl/examples/etl_demos/binlog2kafka.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_demos/csv2csv.py` & `ez-etl-1.1.3/ezetl/examples/etl_demos/csv2csv.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_demos/csv2mysql.py` & `ez-etl-1.1.3/ezetl/examples/etl_demos/csv2mysql.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_demos/kafka2es.py` & `ez-etl-1.1.3/ezetl/examples/etl_demos/kafka2es.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_demos/kafka2ixdb.py` & `ez-etl-1.1.3/ezetl/examples/etl_demos/kafka2ixdb.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_demos/mysql2es.py` & `ez-etl-1.1.3/ezetl/examples/etl_demos/mysql2es.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_demos/mysql2kafka.py` & `ez-etl-1.1.3/ezetl/examples/etl_demos/mysql2kafka.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_demos/mysql2mongodb.py` & `ez-etl-1.1.3/ezetl/examples/etl_demos/mysql2mongodb.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_demos/mysql2n4j.py` & `ez-etl-1.1.3/ezetl/examples/etl_demos/mysql2n4j.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_task/batch_task_demo.py` & `ez-etl-1.1.3/ezetl/examples/etl_task/batch_task_demo.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_task/etl_process_task_demo.py` & `ez-etl-1.1.3/ezetl/examples/etl_task/etl_process_task_demo.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/etl_task/stream_task_demo.py` & `ez-etl-1.1.3/ezetl/examples/etl_task/stream_task_demo.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/reader/read_csv.py` & `ez-etl-1.1.3/ezetl/examples/reader/read_csv.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/reader/read_es.py` & `ez-etl-1.1.3/ezetl/examples/reader/read_es.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/reader/read_kafka.py` & `ez-etl-1.1.3/ezetl/examples/reader/read_kafka.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/reader/read_mongodb.py` & `ez-etl-1.1.3/ezetl/examples/reader/read_mongodb.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/reader/read_mysql.py` & `ez-etl-1.1.3/ezetl/examples/reader/read_mysql.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/reader/read_mysql_binlog.py` & `ez-etl-1.1.3/ezetl/examples/reader/read_mysql_binlog.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/examples/reader/read_n4j.py` & `ez-etl-1.1.3/ezetl/examples/reader/read_n4j.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/libs/es.py` & `ez-etl-1.1.3/ezetl/libs/es.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/libs/hdfs.py` & `ez-etl-1.1.3/ezetl/libs/hdfs.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/libs/ixdb.py` & `ez-etl-1.1.3/ezetl/libs/ixdb.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/libs/kafka_utils.py` & `ez-etl-1.1.3/ezetl/libs/kafka_utils.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/libs/n4j.py` & `ez-etl-1.1.3/ezetl/libs/n4j.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/libs/prometheus.py` & `ez-etl-1.1.3/ezetl/libs/prometheus.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/transform_algs/__init__.py` & `ez-etl-1.1.3/ezetl/transform_algs/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/transform_algs/content_algs.py` & `ez-etl-1.1.3/ezetl/transform_algs/content_algs.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/transform_algs/count_algs.py` & `ez-etl-1.1.3/ezetl/transform_algs/count_algs.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/transform_algs/filter_algs.py` & `ez-etl-1.1.3/ezetl/transform_algs/filter_algs.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/transform_algs/map_algs.py` & `ez-etl-1.1.3/ezetl/transform_algs/map_algs.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/utils/__init__.py` & `ez-etl-1.1.3/ezetl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/utils/common_utils.py` & `ez-etl-1.1.3/ezetl/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/utils/db_utils.py` & `ez-etl-1.1.3/ezetl/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/ezetl/utils/es_query_tool.py` & `ez-etl-1.1.3/ezetl/utils/es_query_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,46 +445,53 @@
         if content_tag == '0':
             contents = []
         elif content_tag == '1':
             contents = []
             for i in data_li:
                 if '*' not in valid_fields:
                     i['_source'] = {k: v for k, v in i['_source'].items() if k in valid_fields}
+                if 'highlight' in i:
+                    i['_source']['_highlight'] = i['highlight']
                 dic = {
                     '_id': i['_id'],
                     '_index': i['_index'],
                     '_score': i['_score'],
                     '_type': i['_type'],
                     **i['_source']
                 }
                 contents.append(dic)
         elif content_tag == '2':
             contents = {}
             for i in data_li:
                 if '*' not in valid_fields:
                     i['_source'] = {k: v for k, v in i['_source'].items() if k in valid_fields}
+                if 'highlight' in i:
+                    i['_source']['_highlight'] = i['highlight']
                 source_dict = i['_source']
                 for k, v in source_dict.items():
                     if k not in contents:
                         contents[k] = [v]
                     else:
                         contents[k].append(v)
         else:
             contents = []
             for i in data_li:
                 if '*' not in valid_fields:
                     i['_source'] = {k: v for k, v in i['_source'].items() if k in valid_fields}
+                if 'highlight' in i:
+                    i['_source']['_highlight'] = i['highlight']
                 contents.append(i)
         return contents
 
     def gen_result(self, result, valid_fields=['*']):
         '''
         组合返回结果
         :return:
         '''
+        print(result)
         total = result['hits']['total']['value']
         data_li = result['hits']['hits']
         contents = self.gen_contents(data_li, valid_fields)
         aggregations = result.get('aggregations', {})
         if self.api_test != 0:
             res_data = {
                 'data': {
```

### Comparing `ez-etl-1.1.2/ezetl/utils/es_utils.py` & `ez-etl-1.1.3/ezetl/utils/es_utils.py`

 * *Files identical despite different names*

### Comparing `ez-etl-1.1.2/setup.py` & `ez-etl-1.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '1.1.2'
+version = '1.1.3'
 
 setup(
     name='ez-etl',
     version=version,
     description="ez-etl is an open-source Extract, Transform, load (ETL) library written in Python. Just configure a dict to read data from various data sources. Use code or built-in conversion algorithms to transform the data into the target data format， and write it to the target data source. ",
     packages=find_packages(),
     include_package_data=True,
@@ -22,15 +22,15 @@
         "python-dateutil",
         "pandas>=1.0.0",
         "openpyxl",
         "xlrd",
         "minio==7.1.1",
         "sqlalchemy>=1.2.0",
         "pymysql",
-        "elasticsearch>=7.17.2",
+        "elasticsearch>=7.15.2",
         "redis==4.0.2",
         "kafka-python==2.0.2",
         "mysql-replication==0.27",
         "minio==7.1.1"
     ],
     extras_require={
         'all': [
```

