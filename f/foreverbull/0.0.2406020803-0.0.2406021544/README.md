# Comparing `tmp/foreverbull-0.0.2406020803.tar.gz` & `tmp/foreverbull-0.0.2406021544.tar.gz`

## Comparing `foreverbull-0.0.2406020803.tar` & `foreverbull-0.0.2406021544.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/.dockerignore
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/Dockerfile
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/build_examples_docker.py
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/conftest.py
--rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/integration_test.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/zipline.Dockerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/examples/__init__.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/examples/multistep_with_namespace.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/examples/multistep_with_namespace_test.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/examples/non_parallel.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/examples/non_parallel_test.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/examples/parallel.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/examples/parallel_test.py
--rw-r--r--   0        0        0    14545 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/conftest.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/__main__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/conftest.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/data.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/data_test.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/exceptions.py
--rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/foreverbull.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/foreverbull_test.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/models.py
--rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/models_test.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/socket.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/testing.py
--rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/worker.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/worker_test.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/__init__.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/backtest.py
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/backtest_test.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/finance.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/finance_test.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/http.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/http_test.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/service.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/service_test.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/storage/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/storage/backtest.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/storage/backtest_test.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/storage/storage.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/broker/storage/storage_test.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/cli/__init__.py
--rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/cli/backtest.py
--rw-r--r--   0        0        0    10963 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/cli/backtest_test.py
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/cli/env.py
--rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/cli/env_test.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/cli/service.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/cli/service_test.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/entity/__init__.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/entity/backtest.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/entity/base.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/entity/finance.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull/entity/service.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull_zipline/__init__.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull_zipline/__main__.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull_zipline/broker.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull_zipline/conftest.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull_zipline/entity.py
--rw-r--r--   0        0        0    15409 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull_zipline/execution.py
--rw-r--r--   0        0        0    13869 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull_zipline/execution_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull_zipline/data_bundles/__init__.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/src/foreverbull_zipline/data_bundles/foreverbull.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/.gitignore
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/pyproject.toml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 foreverbull-0.0.2406020803/PKG-INFO
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/.dockerignore
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/Dockerfile
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/build_examples_docker.py
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/conftest.py
+-rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/integration_test.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/zipline.Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/examples/__init__.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/examples/multistep_with_namespace.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/examples/multistep_with_namespace_test.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/examples/non_parallel.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/examples/non_parallel_test.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/examples/parallel.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/examples/parallel_test.py
+-rw-r--r--   0        0        0    14545 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/conftest.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/__init__.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/__main__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/conftest.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/data.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/data_test.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/exceptions.py
+-rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/foreverbull.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/foreverbull_test.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/models.py
+-rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/models_test.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/socket.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/testing.py
+-rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/worker.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/worker_test.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/__init__.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/backtest.py
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/backtest_test.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/finance.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/finance_test.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/http.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/http_test.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/service.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/service_test.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/storage/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/storage/backtest.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/storage/backtest_test.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/storage/storage.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/broker/storage/storage_test.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/cli/__init__.py
+-rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/cli/backtest.py
+-rw-r--r--   0        0        0    10963 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/cli/backtest_test.py
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/cli/env.py
+-rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/cli/env_test.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/cli/service.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/cli/service_test.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/entity/__init__.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/entity/backtest.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/entity/base.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/entity/finance.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull/entity/service.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull_zipline/__init__.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull_zipline/__main__.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull_zipline/broker.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull_zipline/conftest.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull_zipline/entity.py
+-rw-r--r--   0        0        0    15409 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull_zipline/execution.py
+-rw-r--r--   0        0        0    13869 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull_zipline/execution_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull_zipline/data_bundles/__init__.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/src/foreverbull_zipline/data_bundles/foreverbull.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/.gitignore
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/pyproject.toml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 foreverbull-0.0.2406021544/PKG-INFO
```

### Comparing `foreverbull-0.0.2406020803/conftest.py` & `foreverbull-0.0.2406021544/conftest.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/integration_test.py` & `foreverbull-0.0.2406021544/integration_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/zipline.Dockerfile` & `foreverbull-0.0.2406021544/zipline.Dockerfile`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/examples/multistep_with_namespace.py` & `foreverbull-0.0.2406021544/examples/multistep_with_namespace.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/examples/non_parallel.py` & `foreverbull-0.0.2406021544/examples/non_parallel.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/examples/parallel.py` & `foreverbull-0.0.2406021544/examples/parallel.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/conftest.py` & `foreverbull-0.0.2406021544/src/conftest.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/data.py` & `foreverbull-0.0.2406021544/src/foreverbull/data.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/data_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/data_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/foreverbull.py` & `foreverbull-0.0.2406021544/src/foreverbull/foreverbull.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/foreverbull_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/foreverbull_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/models.py` & `foreverbull-0.0.2406021544/src/foreverbull/models.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/models_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/models_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/socket.py` & `foreverbull-0.0.2406021544/src/foreverbull/socket.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/testing.py` & `foreverbull-0.0.2406021544/src/foreverbull/testing.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/worker.py` & `foreverbull-0.0.2406021544/src/foreverbull/worker.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/worker_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/worker_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/broker/backtest.py` & `foreverbull-0.0.2406021544/src/foreverbull/broker/backtest.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/broker/backtest_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/broker/backtest_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/broker/http.py` & `foreverbull-0.0.2406021544/src/foreverbull/broker/http.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/broker/http_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/broker/http_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/broker/service.py` & `foreverbull-0.0.2406021544/src/foreverbull/broker/service.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/broker/service_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/broker/service_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/broker/storage/backtest.py` & `foreverbull-0.0.2406021544/src/foreverbull/broker/storage/backtest.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/broker/storage/backtest_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/broker/storage/backtest_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/broker/storage/storage.py` & `foreverbull-0.0.2406021544/src/foreverbull/broker/storage/storage.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/broker/storage/storage_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/broker/storage/storage_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/cli/backtest.py` & `foreverbull-0.0.2406021544/src/foreverbull/cli/backtest.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/cli/backtest_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/cli/backtest_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/cli/env.py` & `foreverbull-0.0.2406021544/src/foreverbull/cli/env.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/cli/env_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/cli/env_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/cli/service.py` & `foreverbull-0.0.2406021544/src/foreverbull/cli/service.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/cli/service_test.py` & `foreverbull-0.0.2406021544/src/foreverbull/cli/service_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/entity/backtest.py` & `foreverbull-0.0.2406021544/src/foreverbull/entity/backtest.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/entity/finance.py` & `foreverbull-0.0.2406021544/src/foreverbull/entity/finance.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull/entity/service.py` & `foreverbull-0.0.2406021544/src/foreverbull/entity/service.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull_zipline/__main__.py` & `foreverbull-0.0.2406021544/src/foreverbull_zipline/__main__.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull_zipline/broker.py` & `foreverbull-0.0.2406021544/src/foreverbull_zipline/broker.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull_zipline/conftest.py` & `foreverbull-0.0.2406021544/src/foreverbull_zipline/conftest.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull_zipline/entity.py` & `foreverbull-0.0.2406021544/src/foreverbull_zipline/entity.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull_zipline/execution.py` & `foreverbull-0.0.2406021544/src/foreverbull_zipline/execution.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull_zipline/execution_test.py` & `foreverbull-0.0.2406021544/src/foreverbull_zipline/execution_test.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/src/foreverbull_zipline/data_bundles/foreverbull.py` & `foreverbull-0.0.2406021544/src/foreverbull_zipline/data_bundles/foreverbull.py`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/.gitignore` & `foreverbull-0.0.2406021544/.gitignore`

 * *Files identical despite different names*

### Comparing `foreverbull-0.0.2406020803/pyproject.toml` & `foreverbull-0.0.2406021544/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "foreverbull"
 description = "foreverbull"
 authors = [{ name = "Henrik Nilsson", email = "henrik@lhjnilsson.com" }]
 packages = [{ include = "foreverbull", from = "src" }]
-requires-python = ">=3.11.0,<3.12"
+requires-python = ">=3.11.0"
 dependencies = [
   "pydantic>=2.0.2,<3.0.0",
   "pynng>=0.8.0,<1.0.0",
   "minio>=7.1.14,<8.0.0",
   "pandas>=2.0.3,<3.0.0",
   "requests>=2.26.0,<3.0.0",
   "sqlalchemy>=2.0.19,<3.0.0",
```

### Comparing `foreverbull-0.0.2406020803/PKG-INFO` & `foreverbull-0.0.2406021544/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: foreverbull
-Version: 0.0.2406020803
+Version: 0.0.2406021544
 Summary: foreverbull
 Author-email: Henrik Nilsson <henrik@lhjnilsson.com>
-Requires-Python: <3.12,>=3.11.0
+Requires-Python: >=3.11.0
 Requires-Dist: click<9.0.0,>=8.0.1
 Requires-Dist: cython<4.0,>=3.0.0
 Requires-Dist: docker<8.0.0,>=7.0.0
 Requires-Dist: minio<8.0.0,>=7.1.14
 Requires-Dist: pandas-datareader<1.0.0,>=0.10.0
 Requires-Dist: pandas<3.0.0,>=2.0.3
 Requires-Dist: psycopg2-binary<3.0.0,>=2.9.1
```

