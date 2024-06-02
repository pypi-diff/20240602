# Comparing `tmp/trieste-3.3.0.tar.gz` & `tmp/trieste-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trieste-3.3.0.tar", last modified: Wed May 29 10:35:53 2024, max compression
+gzip compressed data, was "trieste-3.3.1.tar", last modified: Sun Jun  2 17:53:04 2024, max compression
```

## Comparing `trieste-3.3.0.tar` & `trieste-3.3.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.552109 trieste-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 10:35:46.000000 trieste-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-29 10:35:53.552109 trieste-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-29 10:35:46.000000 trieste-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-29 10:35:46.000000 trieste-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:35:53.552109 trieste-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-29 10:35:46.000000 trieste-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.540109 trieste-3.3.0/trieste/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.544109 trieste-3.3.0/trieste/acquisition/
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.544109 trieste-3.3.0/trieste/acquisition/function/
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20754 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/active_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/continuous_thompson_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)    36585 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    77644 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    35334 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/greedy_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    33916 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/multi_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/function/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16951 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.544109 trieste-3.3.0/trieste/acquisition/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/multi_objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/multi_objective/dominance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/multi_objective/pareto.py
--rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/multi_objective/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    42509 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)   120442 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/acquisition/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29749 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/ask_tell_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    51213 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/bayesian_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.544109 trieste-3.3.0/trieste/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.548109 trieste-3.3.0/trieste/experimental/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/experimental/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/experimental/plotting/inequality_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    23612 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/experimental/plotting/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/experimental/plotting/plotting_plotly.py
--rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.548109 trieste-3.3.0/trieste/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.548109 trieste-3.3.0/trieste/models/gpflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27404 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/inducing_point_selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    91274 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    41061 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.548109 trieste-3.3.0/trieste/models/gpflux/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflux/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflux/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflux/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/gpflux/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.552109 trieste-3.3.0/trieste/models/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15525 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/architectures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/keras/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.552109 trieste-3.3.0/trieste/objectives/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/objectives/multi_objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/objectives/multifidelity_objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)    24268 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/objectives/single_objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/objectives/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/observer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54291 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.552109 trieste-3.3.0/trieste/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-29 10:35:46.000000 trieste-3.3.0/trieste/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:35:53.552109 trieste-3.3.0/trieste.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-29 10:35:53.000000 trieste-3.3.0/trieste.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-29 10:35:53.000000 trieste-3.3.0/trieste.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:35:53.000000 trieste-3.3.0/trieste.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-29 10:35:53.000000 trieste-3.3.0/trieste.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 10:35:53.000000 trieste-3.3.0/trieste.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.026213 trieste-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-02 17:52:55.000000 trieste-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-06-02 17:53:04.026213 trieste-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-06-02 17:52:55.000000 trieste-3.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-06-02 17:52:55.000000 trieste-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:53:04.026213 trieste-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-06-02 17:52:55.000000 trieste-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.014212 trieste-3.3.1/trieste/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.014212 trieste-3.3.1/trieste/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.018212 trieste-3.3.1/trieste/acquisition/function/
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20754 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/function/active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/function/continuous_thompson_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36585 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/function/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77644 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/function/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35334 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/function/greedy_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33916 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/function/multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/function/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16951 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.018212 trieste-3.3.1/trieste/acquisition/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/multi_objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/multi_objective/dominance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/multi_objective/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16733 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/multi_objective/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42509 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120442 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/acquisition/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32052 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/ask_tell_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51213 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/bayesian_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.018212 trieste-3.3.1/trieste/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.018212 trieste-3.3.1/trieste/experimental/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/experimental/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/experimental/plotting/inequality_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23612 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/experimental/plotting/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/experimental/plotting/plotting_plotly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.018212 trieste-3.3.1/trieste/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.022213 trieste-3.3.1/trieste/models/gpflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27404 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflow/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflow/inducing_point_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflow/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91274 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflow/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41061 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflow/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.022213 trieste-3.3.1/trieste/models/gpflux/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflux/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflux/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflux/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/gpflux/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31342 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.022213 trieste-3.3.1/trieste/models/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15525 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/keras/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/keras/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/keras/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26847 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/keras/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/keras/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/keras/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.026213 trieste-3.3.1/trieste/objectives/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/objectives/multi_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/objectives/multifidelity_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24268 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/objectives/single_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/objectives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54291 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.026213 trieste-3.3.1/trieste/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-06-02 17:52:55.000000 trieste-3.3.1/trieste/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:53:04.026213 trieste-3.3.1/trieste.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-06-02 17:53:03.000000 trieste-3.3.1/trieste.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-06-02 17:53:04.000000 trieste-3.3.1/trieste.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:53:03.000000 trieste-3.3.1/trieste.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-02 17:53:03.000000 trieste-3.3.1/trieste.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 17:53:03.000000 trieste-3.3.1/trieste.egg-info/top_level.txt
```

### Comparing `trieste-3.3.0/LICENSE` & `trieste-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/PKG-INFO` & `trieste-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trieste
-Version: 3.3.0
+Version: 3.3.1
 Summary: A Bayesian optimization research toolbox built on TensorFlow
 Home-page: https://github.com/secondmind-labs/trieste
 Author: The Trieste contributors
 Author-email: labs@secondmind.ai
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `trieste-3.3.0/README.md` & `trieste-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/pyproject.toml` & `trieste-3.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/setup.py` & `trieste-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/__init__.py` & `trieste-3.3.1/trieste/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/__init__.py` & `trieste-3.3.1/trieste/acquisition/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/combination.py` & `trieste-3.3.1/trieste/acquisition/combination.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/function/__init__.py` & `trieste-3.3.1/trieste/acquisition/function/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/function/active_learning.py` & `trieste-3.3.1/trieste/acquisition/function/active_learning.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/function/continuous_thompson_sampling.py` & `trieste-3.3.1/trieste/acquisition/function/continuous_thompson_sampling.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/function/entropy.py` & `trieste-3.3.1/trieste/acquisition/function/entropy.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/function/function.py` & `trieste-3.3.1/trieste/acquisition/function/function.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/function/greedy_batch.py` & `trieste-3.3.1/trieste/acquisition/function/greedy_batch.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/function/multi_objective.py` & `trieste-3.3.1/trieste/acquisition/function/multi_objective.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/function/utils.py` & `trieste-3.3.1/trieste/acquisition/function/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/interface.py` & `trieste-3.3.1/trieste/acquisition/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/multi_objective/__init__.py` & `trieste-3.3.1/trieste/acquisition/multi_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/multi_objective/dominance.py` & `trieste-3.3.1/trieste/acquisition/multi_objective/dominance.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/multi_objective/pareto.py` & `trieste-3.3.1/trieste/acquisition/multi_objective/pareto.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/multi_objective/partition.py` & `trieste-3.3.1/trieste/acquisition/multi_objective/partition.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/optimizer.py` & `trieste-3.3.1/trieste/acquisition/optimizer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/rule.py` & `trieste-3.3.1/trieste/acquisition/rule.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/sampler.py` & `trieste-3.3.1/trieste/acquisition/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/acquisition/utils.py` & `trieste-3.3.1/trieste/acquisition/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/ask_tell_optimization.py` & `trieste-3.3.1/trieste/ask_tell_optimization.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,18 @@
     record: Record[StateType, ProbabilisticModelType]
     """ A record of the current state of the optimization. """
 
     local_data_ixs: Optional[Sequence[TensorType]]
     """ Indices to the local data, for LocalDatasetsAcquisitionRule rules
     when `track_data` is `False`. """
 
+    local_data_len: Optional[int]
+    """ Length of the datasets, for LocalDatasetsAcquisitionRule rules
+    when `track_data` is `False`. """
+
 
 class AskTellOptimizerABC(ABC, Generic[SearchSpaceType, ProbabilisticModelType]):
     """
     This class provides Ask/Tell optimization interface. It is designed for those use cases
     when control of the optimization loop by Trieste is impossible or not desirable.
     For the default use case with model training, refer to :class:`AskTellOptimizer`.
     For more details about the Bayesian Optimization routine, refer to :class:`BayesianOptimizer`.
@@ -101,28 +105,30 @@
         search_space: SearchSpaceType,
         datasets: Mapping[Tag, Dataset],
         models: Mapping[Tag, ProbabilisticModelType],
         *,
         fit_model: bool = True,
         track_data: bool = True,
         local_data_ixs: Optional[Sequence[TensorType]] = None,
+        local_data_len: Optional[int] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
         search_space: SearchSpaceType,
         datasets: Mapping[Tag, Dataset],
         models: Mapping[Tag, ProbabilisticModelType],
         acquisition_rule: AcquisitionRule[TensorType, SearchSpaceType, ProbabilisticModelType],
         *,
         fit_model: bool = True,
         track_data: bool = True,
         local_data_ixs: Optional[Sequence[TensorType]] = None,
+        local_data_len: Optional[int] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
         search_space: SearchSpaceType,
@@ -132,41 +138,44 @@
             State[StateType | None, TensorType], SearchSpaceType, ProbabilisticModelType
         ],
         acquisition_state: StateType | None,
         *,
         fit_model: bool = True,
         track_data: bool = True,
         local_data_ixs: Optional[Sequence[TensorType]] = None,
+        local_data_len: Optional[int] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
         search_space: SearchSpaceType,
         datasets: Dataset,
         models: ProbabilisticModelType,
         *,
         fit_model: bool = True,
         track_data: bool = True,
         local_data_ixs: Optional[Sequence[TensorType]] = None,
+        local_data_len: Optional[int] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
         search_space: SearchSpaceType,
         datasets: Dataset,
         models: ProbabilisticModelType,
         acquisition_rule: AcquisitionRule[TensorType, SearchSpaceType, ProbabilisticModelType],
         *,
         fit_model: bool = True,
         track_data: bool = True,
         local_data_ixs: Optional[Sequence[TensorType]] = None,
+        local_data_len: Optional[int] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
         search_space: SearchSpaceType,
@@ -176,14 +185,15 @@
             State[StateType | None, TensorType], SearchSpaceType, ProbabilisticModelType
         ],
         acquisition_state: StateType | None = None,
         *,
         fit_model: bool = True,
         track_data: bool = True,
         local_data_ixs: Optional[Sequence[TensorType]] = None,
+        local_data_len: Optional[int] = None,
     ):
         ...
 
     def __init__(
         self,
         search_space: SearchSpaceType,
         datasets: Mapping[Tag, Dataset] | Dataset,
@@ -195,14 +205,15 @@
         ]
         | None = None,
         acquisition_state: StateType | None = None,
         *,
         fit_model: bool = True,
         track_data: bool = True,
         local_data_ixs: Optional[Sequence[TensorType]] = None,
+        local_data_len: Optional[int] = None,
     ):
         """
         :param search_space: The space over which to search for the next query point.
         :param datasets: Already observed input-output pairs for each tag.
         :param models: The model to use for each :class:`~trieste.data.Dataset` in
             ``datasets``.
         :param acquisition_rule: The acquisition rule, which defines how to search for a new point
@@ -215,14 +226,16 @@
             If `False`, the models are assumed to be optimized already.
         :param track_data: If `True` (default), the optimizer will track the changing
             datasets via a local copy. If `False`, it will infer new datasets from
             updates to the global datasets (optionally using `local_data_ixs` and indices passed
             in to `tell`).
         :param local_data_ixs: Indices to the local data in the initial datasets. If unspecified,
             assumes that the initial datasets are global.
+        :param local_data_len: Optional length of the data when the passed in `local_data_ixs`
+            were measured. If the data has increased since then, the indices are extended.
         :raise ValueError: If any of the following are true:
             - the keys in ``datasets`` and ``models`` do not match
             - ``datasets`` or ``models`` are empty
             - default acquisition is used but incompatible with other inputs
         """
         self._search_space = search_space
         self._acquisition_record = self._acquisition_state = acquisition_state
@@ -277,18 +290,37 @@
             num_local_datasets = self._acquisition_rule.num_local_datasets
             if self.track_data:
                 datasets = self._datasets = with_local_datasets(self._datasets, num_local_datasets)
             else:
                 self._dataset_len = self.dataset_len(self._datasets)
                 if local_data_ixs is not None:
                     self._dataset_ixs = list(local_data_ixs)
+                    if local_data_len is not None:
+                        # infer new dataset indices from change in dataset sizes
+                        num_new_points = self._dataset_len - local_data_len
+                        if num_new_points < 0 or num_new_points % num_local_datasets != 0:
+                            raise ValueError(
+                                "Cannot infer new data points as datasets haven't increased by "
+                                f"a multiple of {num_local_datasets}"
+                            )
+                        for i in range(num_local_datasets):
+                            self._dataset_ixs[i] = tf.concat(
+                                [
+                                    self._dataset_ixs[i],
+                                    tf.range(0, num_new_points, num_local_datasets)
+                                    + local_data_len
+                                    + i,
+                                ],
+                                -1,
+                            )
                 else:
                     self._dataset_ixs = [
                         tf.range(self._dataset_len) for _ in range(num_local_datasets)
                     ]
+
                 datasets = with_local_datasets(
                     self._datasets, num_local_datasets, self._dataset_ixs
                 )
             self._acquisition_rule.initialize_subspaces(search_space)
 
         filtered_datasets: Mapping[Tag, Dataset] | State[
             StateType | None, Mapping[Tag, Dataset]
@@ -349,14 +381,22 @@
         """Indices to the local data. Only stored for LocalDatasetsAcquisitionRule rules
         when `track_data` is `False`."""
         if isinstance(self._acquisition_rule, LocalDatasetsAcquisitionRule) and not self.track_data:
             return self._dataset_ixs
         return None
 
     @property
+    def local_data_len(self) -> Optional[int]:
+        """Data length. Only stored for LocalDatasetsAcquisitionRule rules
+        when `track_data` is `False`."""
+        if isinstance(self._acquisition_rule, LocalDatasetsAcquisitionRule) and not self.track_data:
+            return self._dataset_len
+        return None
+
+    @property
     def models(self) -> Mapping[Tag, ProbabilisticModelType]:
         """The current models."""
         return self._models
 
     @models.setter
     def models(self, models: Mapping[Tag, ProbabilisticModelType]) -> None:
         """Update the current models."""
@@ -416,26 +456,28 @@
             TensorType | State[StateType | None, TensorType],
             SearchSpaceType,
             ProbabilisticModelType,
         ]
         | None = None,
         track_data: bool = True,
         local_data_ixs: Optional[Sequence[TensorType]] = None,
+        local_data_len: Optional[int] = None,
     ) -> AskTellOptimizerType:
         """Creates new :class:`~AskTellOptimizer` instance from provided optimization state.
         Model training isn't triggered upon creation of the instance.
 
         :param record: Optimization state record.
         :param search_space: The space over which to search for the next query point.
         :param acquisition_rule: The acquisition rule, which defines how to search for a new point
             on each optimization step. Defaults to
             :class:`~trieste.acquisition.rule.EfficientGlobalOptimization` with default
             arguments.
         :param track_data: Whether the optimizer tracks the changing datasets via a local copy.
         :param local_data_ixs: Indices to local data for local rules with `track_data` False.
+        :param local_data_len: Original data length for local rules with `track_data` False.
         :return: New instance of :class:`~AskTellOptimizer`.
         """
         # we are recovering previously saved optimization state
         # so the model was already trained
         # thus there is no need to train it again
 
         # type ignore below is because this relies on subclasses not overriding __init__
@@ -445,14 +487,15 @@
             record.datasets,
             record.models,
             acquisition_rule=acquisition_rule,
             acquisition_state=record.acquisition_state,
             fit_model=False,
             track_data=track_data,
             local_data_ixs=local_data_ixs,
+            local_data_len=local_data_len,
         )
 
     def to_record(self, copy: bool = True) -> Record[StateType, ProbabilisticModelType]:
         """Collects the current state of the optimization, which includes datasets,
         models and acquisition state (if applicable).
 
         :param copy: Whether to return a copy of the current state or the original. Copying
@@ -517,14 +560,15 @@
         """
         return cls.from_record(  # type: ignore
             state.record,
             search_space,
             acquisition_rule,
             track_data=track_data,
             local_data_ixs=state.local_data_ixs,
+            local_data_len=state.local_data_len,
         )
 
     def to_state(
         self, copy: bool = False
     ) -> AskTellOptimizerState[StateType, ProbabilisticModelType]:
         """Returns the AskTellOptimizer state, comprising the current optimization state
         alongside any internal AskTellOptimizer state.
@@ -533,14 +577,15 @@
             is not supported for all model types. However, continuing the optimization will
             modify the original state.
         :return: An :class:`AskTellOptimizerState` object.
         """
         return AskTellOptimizerState(
             record=self.to_record(copy=copy),
             local_data_ixs=self.local_data_ixs,
+            local_data_len=self.local_data_len,
         )
 
     def ask(self) -> TensorType:
         """Suggests a point (or points in batch mode) to observe by optimizing the acquisition
         function. If the acquisition is stateful, its state is saved.
 
         :return: A :class:`TensorType` instance representing suggested point(s).
```

### Comparing `trieste-3.3.0/trieste/bayesian_optimizer.py` & `trieste-3.3.1/trieste/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/data.py` & `trieste-3.3.1/trieste/data.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/experimental/plotting/__init__.py` & `trieste-3.3.1/trieste/experimental/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/experimental/plotting/inequality_constraints.py` & `trieste-3.3.1/trieste/experimental/plotting/inequality_constraints.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/experimental/plotting/plotting.py` & `trieste-3.3.1/trieste/experimental/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/experimental/plotting/plotting_plotly.py` & `trieste-3.3.1/trieste/experimental/plotting/plotting_plotly.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/logging.py` & `trieste-3.3.1/trieste/logging.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/__init__.py` & `trieste-3.3.1/trieste/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflow/__init__.py` & `trieste-3.3.1/trieste/models/gpflow/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflow/builders.py` & `trieste-3.3.1/trieste/models/gpflow/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflow/inducing_point_selectors.py` & `trieste-3.3.1/trieste/models/gpflow/inducing_point_selectors.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflow/interface.py` & `trieste-3.3.1/trieste/models/gpflow/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflow/models.py` & `trieste-3.3.1/trieste/models/gpflow/models.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflow/optimizer.py` & `trieste-3.3.1/trieste/models/gpflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflow/sampler.py` & `trieste-3.3.1/trieste/models/gpflow/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflow/utils.py` & `trieste-3.3.1/trieste/models/gpflow/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflux/__init__.py` & `trieste-3.3.1/trieste/models/gpflux/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflux/builders.py` & `trieste-3.3.1/trieste/models/gpflux/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflux/interface.py` & `trieste-3.3.1/trieste/models/gpflux/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflux/models.py` & `trieste-3.3.1/trieste/models/gpflux/models.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/gpflux/sampler.py` & `trieste-3.3.1/trieste/models/gpflux/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/interfaces.py` & `trieste-3.3.1/trieste/models/interfaces.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/keras/__init__.py` & `trieste-3.3.1/trieste/models/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/keras/architectures.py` & `trieste-3.3.1/trieste/models/keras/architectures.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/keras/builders.py` & `trieste-3.3.1/trieste/models/keras/builders.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/keras/interface.py` & `trieste-3.3.1/trieste/models/keras/interface.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/keras/models.py` & `trieste-3.3.1/trieste/models/keras/models.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/keras/sampler.py` & `trieste-3.3.1/trieste/models/keras/sampler.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/keras/utils.py` & `trieste-3.3.1/trieste/models/keras/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/optimizer.py` & `trieste-3.3.1/trieste/models/optimizer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/models/utils.py` & `trieste-3.3.1/trieste/models/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/objectives/__init__.py` & `trieste-3.3.1/trieste/objectives/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/objectives/multi_objectives.py` & `trieste-3.3.1/trieste/objectives/multi_objectives.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/objectives/multifidelity_objectives.py` & `trieste-3.3.1/trieste/objectives/multifidelity_objectives.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/objectives/single_objectives.py` & `trieste-3.3.1/trieste/objectives/single_objectives.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/objectives/utils.py` & `trieste-3.3.1/trieste/objectives/utils.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/observer.py` & `trieste-3.3.1/trieste/observer.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/space.py` & `trieste-3.3.1/trieste/space.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/types.py` & `trieste-3.3.1/trieste/types.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/utils/__init__.py` & `trieste-3.3.1/trieste/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/utils/misc.py` & `trieste-3.3.1/trieste/utils/misc.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste/version.py` & `trieste-3.3.1/trieste/version.py`

 * *Files identical despite different names*

### Comparing `trieste-3.3.0/trieste.egg-info/PKG-INFO` & `trieste-3.3.1/trieste.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trieste
-Version: 3.3.0
+Version: 3.3.1
 Summary: A Bayesian optimization research toolbox built on TensorFlow
 Home-page: https://github.com/secondmind-labs/trieste
 Author: The Trieste contributors
 Author-email: labs@secondmind.ai
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `trieste-3.3.0/trieste.egg-info/SOURCES.txt` & `trieste-3.3.1/trieste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

