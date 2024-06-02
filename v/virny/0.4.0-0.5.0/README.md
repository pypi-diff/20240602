# Comparing `tmp/virny-0.4.0.tar.gz` & `tmp/virny-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virny-0.4.0.tar", last modified: Mon Jan 29 22:13:06 2024, max compression
+gzip compressed data, was "virny-0.5.0.tar", last modified: Sun Jun  2 13:54:06 2024, max compression
```

## Comparing `virny-0.4.0.tar` & `virny-0.5.0.tar`

### file list

```diff
@@ -1,91 +1,100 @@
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.480355 virny-0.4.0/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1502 2023-09-28 20:03:51.000000 virny-0.4.0/LICENSE
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)       85 2023-09-28 20:03:51.000000 virny-0.4.0/MANIFEST.in
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     5723 2024-01-29 22:13:06.480228 virny-0.4.0/PKG-INFO
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4975 2024-01-29 22:06:49.000000 virny-0.4.0/README.md
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)       38 2024-01-29 22:13:06.480400 virny-0.4.0/setup.cfg
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     2524 2024-01-29 22:06:49.000000 virny-0.4.0/setup.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.442397 virny-0.4.0/tests/
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.443950 virny-0.4.0/tests/analyzers/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:06:49.000000 virny-0.4.0/tests/analyzers/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1827 2024-01-29 22:06:49.000000 virny-0.4.0/tests/analyzers/test_subgroup_error_analyzer.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.444390 virny-0.4.0/tests/custom_classes/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2023-09-28 20:03:51.000000 virny-0.4.0/tests/custom_classes/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     6629 2024-01-29 22:06:49.000000 virny-0.4.0/tests/custom_classes/test_metrics_composer.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.444566 virny-0.4.0/tests/metrics/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2023-09-28 20:03:51.000000 virny-0.4.0/tests/metrics/__init__.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.444749 virny-0.4.0/tests/preprocessing/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2023-09-28 20:03:51.000000 virny-0.4.0/tests/preprocessing/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     2096 2023-09-28 20:03:51.000000 virny-0.4.0/tests/preprocessing/test_basic_preprocessing.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.445129 virny-0.4.0/tests/user_interfaces/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:06:49.000000 virny-0.4.0/tests/user_interfaces/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     5683 2024-01-29 22:06:49.000000 virny-0.4.0/tests/user_interfaces/test_compute_model_metrics.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.446077 virny-0.4.0/tests/utils/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2023-09-28 20:03:51.000000 virny-0.4.0/tests/utils/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     2411 2024-01-29 22:06:49.000000 virny-0.4.0/tests/utils/test_common_helpers.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1565 2024-01-29 22:06:49.000000 virny-0.4.0/tests/utils/test_data_viz_utils.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     8136 2024-01-29 22:06:49.000000 virny-0.4.0/tests/utils/test_protected_groups_partitioning.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4472 2024-01-29 22:06:49.000000 virny-0.4.0/tests/utils/test_stability_utils.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.446546 virny-0.4.0/virny/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)       37 2023-09-28 20:03:51.000000 virny-0.4.0/virny/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)       63 2024-01-29 22:08:26.000000 virny-0.4.0/virny/__version__.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.448694 virny-0.4.0/virny/analyzers/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)      995 2024-01-29 22:06:49.000000 virny-0.4.0/virny/analyzers/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     6765 2024-01-29 22:06:49.000000 virny-0.4.0/virny/analyzers/abstract_overall_variance_analyzer.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     6668 2024-01-29 22:06:49.000000 virny-0.4.0/virny/analyzers/abstract_subgroup_analyzer.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     3157 2024-01-29 22:06:49.000000 virny-0.4.0/virny/analyzers/batch_overall_variance_analyzer.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     6488 2024-01-29 22:06:49.000000 virny-0.4.0/virny/analyzers/batch_overall_variance_analyzer_postprocessing.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1432 2024-01-29 22:06:49.000000 virny-0.4.0/virny/analyzers/subgroup_error_analyzer.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     8920 2024-01-29 22:06:49.000000 virny-0.4.0/virny/analyzers/subgroup_variance_analyzer.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     7088 2024-01-29 22:06:49.000000 virny-0.4.0/virny/analyzers/subgroup_variance_calculator.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)      292 2023-09-28 20:03:51.000000 virny-0.4.0/virny/api.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.449068 virny-0.4.0/virny/configs/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)       71 2023-09-28 20:03:51.000000 virny-0.4.0/virny/configs/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1766 2024-01-29 22:06:49.000000 virny-0.4.0/virny/configs/constants.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.450192 virny-0.4.0/virny/custom_classes/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)      558 2024-01-29 22:06:49.000000 virny-0.4.0/virny/custom_classes/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1880 2023-09-28 20:03:51.000000 virny-0.4.0/virny/custom_classes/base_dataset.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1264 2024-01-29 22:06:49.000000 virny-0.4.0/virny/custom_classes/base_inprocessing_wrapper.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)      633 2023-09-28 20:03:51.000000 virny-0.4.0/virny/custom_classes/custom_logger.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     5659 2024-01-29 22:06:49.000000 virny-0.4.0/virny/custom_classes/metrics_composer.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)    52712 2024-01-29 22:06:49.000000 virny-0.4.0/virny/custom_classes/metrics_interactive_visualizer.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)    16025 2024-01-29 22:06:49.000000 virny-0.4.0/virny/custom_classes/metrics_visualizer.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.475545 virny-0.4.0/virny/datasets/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)   391642 2023-09-28 20:03:51.000000 virny-0.4.0/virny/datasets/COMPAS.csv
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)      855 2024-01-29 22:06:49.000000 virny-0.4.0/virny/datasets/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1399 2023-09-28 20:03:51.000000 virny-0.4.0/virny/datasets/base.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)  2988234 2024-01-29 22:06:49.000000 virny-0.4.0/virny/datasets/credit_card_default_clean.csv
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)    31107 2024-01-29 22:06:49.000000 virny-0.4.0/virny/datasets/data_loaders.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)  7564965 2023-09-28 20:03:51.000000 virny-0.4.0/virny/datasets/givemesomecredit.csv
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)  1135557 2023-09-28 20:03:51.000000 virny-0.4.0/virny/datasets/law_school_clean.csv
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4383 2023-09-28 20:03:51.000000 virny-0.4.0/virny/datasets/ricci_race.csv
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)    69859 2024-01-29 22:06:49.000000 virny-0.4.0/virny/datasets/student_por_new.csv
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.476762 virny-0.4.0/virny/metrics/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1408 2024-01-29 22:06:49.000000 virny-0.4.0/virny/metrics/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     2438 2024-01-29 22:06:49.000000 virny-0.4.0/virny/metrics/accuracy_metrics.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     3482 2024-01-29 22:06:49.000000 virny-0.4.0/virny/metrics/stability_metrics.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1674 2024-01-29 22:06:49.000000 virny-0.4.0/virny/metrics/uncertainty_metrics.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.477159 virny-0.4.0/virny/preprocessing/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)      268 2023-09-28 20:03:51.000000 virny-0.4.0/virny/preprocessing/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4053 2023-09-28 20:03:51.000000 virny-0.4.0/virny/preprocessing/basic_preprocessing.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.478156 virny-0.4.0/virny/user_interfaces/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)      646 2024-01-29 22:06:49.000000 virny-0.4.0/virny/user_interfaces/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)    15001 2024-01-29 22:06:49.000000 virny-0.4.0/virny/user_interfaces/multiple_models_api.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     5370 2024-01-29 22:06:49.000000 virny-0.4.0/virny/user_interfaces/multiple_models_with_db_writer_api.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)    16343 2024-01-29 22:06:49.000000 virny-0.4.0/virny/user_interfaces/multiple_models_with_multiple_test_sets_api.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.479932 virny-0.4.0/virny/utils/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)      380 2024-01-29 22:06:49.000000 virny-0.4.0/virny/utils/__init__.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4637 2024-01-29 22:06:49.000000 virny-0.4.0/virny/utils/common_helpers.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     3455 2024-01-17 22:01:34.000000 virny-0.4.0/virny/utils/custom_initializers.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)    23376 2024-01-29 22:06:49.000000 virny-0.4.0/virny/utils/data_viz_utils.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     8188 2024-01-29 22:06:49.000000 virny-0.4.0/virny/utils/model_tuning_utils.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1827 2024-01-29 22:06:49.000000 virny-0.4.0/virny/utils/postprocessing_intervention_utils.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4778 2024-01-29 22:06:49.000000 virny-0.4.0/virny/utils/protected_groups_partitioning.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     3724 2024-01-29 22:06:49.000000 virny-0.4.0/virny/utils/stability_utils.py
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1982 2023-09-28 20:03:51.000000 virny-0.4.0/virny/utils/validation.py
-drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:13:06.447484 virny-0.4.0/virny.egg-info/
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     5723 2024-01-29 22:13:06.000000 virny-0.4.0/virny.egg-info/PKG-INFO
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)     2501 2024-01-29 22:13:06.000000 virny-0.4.0/virny.egg-info/SOURCES.txt
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)        1 2024-01-29 22:13:06.000000 virny-0.4.0/virny.egg-info/dependency_links.txt
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)      651 2024-01-29 22:13:06.000000 virny-0.4.0/virny.egg-info/requires.txt
--rw-r--r--   0 denys_herasymuk   (501) staff       (20)       12 2024-01-29 22:13:06.000000 virny-0.4.0/virny.egg-info/top_level.txt
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.757628 virny-0.5.0/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1502 2023-09-28 20:03:51.000000 virny-0.5.0/LICENSE
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)      100 2024-06-02 13:53:40.000000 virny-0.5.0/MANIFEST.in
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     6956 2024-06-02 13:54:06.757378 virny-0.5.0/PKG-INFO
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     6208 2024-06-02 13:53:40.000000 virny-0.5.0/README.md
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)       38 2024-06-02 13:54:06.757725 virny-0.5.0/setup.cfg
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     2524 2024-01-29 22:06:49.000000 virny-0.5.0/setup.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.731099 virny-0.5.0/tests/
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.732545 virny-0.5.0/tests/analyzers/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:06:49.000000 virny-0.5.0/tests/analyzers/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1699 2024-06-02 13:53:40.000000 virny-0.5.0/tests/analyzers/test_subgroup_error_analyzer.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.732876 virny-0.5.0/tests/custom_classes/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2023-09-28 20:03:51.000000 virny-0.5.0/tests/custom_classes/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     6629 2024-01-29 22:06:49.000000 virny-0.5.0/tests/custom_classes/test_metrics_composer.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.733122 virny-0.5.0/tests/metrics/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2023-09-28 20:03:51.000000 virny-0.5.0/tests/metrics/__init__.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.733300 virny-0.5.0/tests/preprocessing/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2023-09-28 20:03:51.000000 virny-0.5.0/tests/preprocessing/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     2096 2023-09-28 20:03:51.000000 virny-0.5.0/tests/preprocessing/test_basic_preprocessing.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.734208 virny-0.5.0/tests/user_interfaces/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2024-01-29 22:06:49.000000 virny-0.5.0/tests/user_interfaces/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     3783 2024-06-02 13:53:40.000000 virny-0.5.0/tests/user_interfaces/conftest.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     5917 2024-06-02 13:53:40.000000 virny-0.5.0/tests/user_interfaces/test_compute_model_metrics.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     5398 2024-06-02 13:53:40.000000 virny-0.5.0/tests/user_interfaces/test_multiple_models_api.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.735071 virny-0.5.0/tests/utils/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)        0 2023-09-28 20:03:51.000000 virny-0.5.0/tests/utils/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     2394 2024-06-02 13:53:40.000000 virny-0.5.0/tests/utils/test_common_helpers.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1565 2024-01-29 22:06:49.000000 virny-0.5.0/tests/utils/test_data_viz_utils.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     8136 2024-01-29 22:06:49.000000 virny-0.5.0/tests/utils/test_protected_groups_partitioning.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4593 2024-06-02 13:53:40.000000 virny-0.5.0/tests/utils/test_stability_utils.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.735586 virny-0.5.0/virny/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)       37 2023-09-28 20:03:51.000000 virny-0.5.0/virny/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)       63 2024-06-02 13:53:40.000000 virny-0.5.0/virny/__version__.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.737639 virny-0.5.0/virny/analyzers/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)      995 2024-01-29 22:06:49.000000 virny-0.5.0/virny/analyzers/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     7993 2024-06-02 13:53:40.000000 virny-0.5.0/virny/analyzers/abstract_overall_variance_analyzer.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     6569 2024-06-02 13:53:40.000000 virny-0.5.0/virny/analyzers/abstract_subgroup_analyzer.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     3355 2024-06-02 13:53:40.000000 virny-0.5.0/virny/analyzers/batch_overall_variance_analyzer.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     7338 2024-06-02 13:53:40.000000 virny-0.5.0/virny/analyzers/batch_overall_variance_analyzer_postprocessing.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1432 2024-01-29 22:06:49.000000 virny-0.5.0/virny/analyzers/subgroup_error_analyzer.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     9805 2024-06-02 13:53:40.000000 virny-0.5.0/virny/analyzers/subgroup_variance_analyzer.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     7088 2024-01-29 22:06:49.000000 virny-0.5.0/virny/analyzers/subgroup_variance_calculator.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)      292 2023-09-28 20:03:51.000000 virny-0.5.0/virny/api.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.738005 virny-0.5.0/virny/configs/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)       71 2023-09-28 20:03:51.000000 virny-0.5.0/virny/configs/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1734 2024-06-02 13:53:40.000000 virny-0.5.0/virny/configs/constants.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.739055 virny-0.5.0/virny/custom_classes/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)      558 2024-01-29 22:06:49.000000 virny-0.5.0/virny/custom_classes/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     2683 2024-06-02 13:53:40.000000 virny-0.5.0/virny/custom_classes/base_dataset.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1820 2024-06-02 13:53:40.000000 virny-0.5.0/virny/custom_classes/base_inprocessing_wrapper.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)      633 2023-09-28 20:03:51.000000 virny-0.5.0/virny/custom_classes/custom_logger.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     5659 2024-06-02 13:53:40.000000 virny-0.5.0/virny/custom_classes/metrics_composer.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)    52661 2024-06-02 13:53:40.000000 virny-0.5.0/virny/custom_classes/metrics_interactive_visualizer.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)    16010 2024-06-02 13:53:40.000000 virny-0.5.0/virny/custom_classes/metrics_visualizer.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.740514 virny-0.5.0/virny/datasets/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1066 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1399 2024-05-01 20:36:31.000000 virny-0.5.0/virny/datasets/base.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     3665 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/compas.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.752738 virny-0.5.0/virny/datasets/data/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)   391642 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/data/COMPAS.csv
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)  3274762 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/data/bank-full.csv
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)  2941524 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/data/cardio.csv
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)    98302 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/data/diabetes_dataset__2019.csv
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)   195697 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/data/german_data_credit.csv
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)  1135557 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/data/law_school_clean.csv
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4383 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/data/ricci_race.csv
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)    69859 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/data/student_por_new.csv
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     3609 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/education.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4926 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/finance.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)    15948 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/folktables.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4788 2024-06-02 13:53:40.000000 virny-0.5.0/virny/datasets/healthcare.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.753886 virny-0.5.0/virny/metrics/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1408 2024-01-29 22:06:49.000000 virny-0.5.0/virny/metrics/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     2393 2024-06-02 13:53:40.000000 virny-0.5.0/virny/metrics/accuracy_metrics.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     3482 2024-01-29 22:06:49.000000 virny-0.5.0/virny/metrics/stability_metrics.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1674 2024-01-29 22:06:49.000000 virny-0.5.0/virny/metrics/uncertainty_metrics.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.754361 virny-0.5.0/virny/preprocessing/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)      268 2023-09-28 20:03:51.000000 virny-0.5.0/virny/preprocessing/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4320 2024-06-02 13:53:40.000000 virny-0.5.0/virny/preprocessing/basic_preprocessing.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.754976 virny-0.5.0/virny/user_interfaces/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)      646 2024-01-29 22:06:49.000000 virny-0.5.0/virny/user_interfaces/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)    17143 2024-06-02 13:53:40.000000 virny-0.5.0/virny/user_interfaces/multiple_models_api.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     5644 2024-06-02 13:53:40.000000 virny-0.5.0/virny/user_interfaces/multiple_models_with_db_writer_api.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)    19041 2024-06-02 13:53:40.000000 virny-0.5.0/virny/user_interfaces/multiple_models_with_multiple_test_sets_api.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.756716 virny-0.5.0/virny/utils/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)      380 2024-01-29 22:06:49.000000 virny-0.5.0/virny/utils/__init__.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     5215 2024-06-02 13:53:40.000000 virny-0.5.0/virny/utils/common_helpers.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     3455 2024-01-17 22:01:34.000000 virny-0.5.0/virny/utils/custom_initializers.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)    25664 2024-06-02 13:53:40.000000 virny-0.5.0/virny/utils/data_viz_utils.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     8188 2024-01-29 22:06:49.000000 virny-0.5.0/virny/utils/model_tuning_utils.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1827 2024-01-29 22:06:49.000000 virny-0.5.0/virny/utils/postprocessing_intervention_utils.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     4830 2024-06-02 13:53:40.000000 virny-0.5.0/virny/utils/protected_groups_partitioning.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     3854 2024-06-02 13:53:40.000000 virny-0.5.0/virny/utils/stability_utils.py
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     1982 2023-09-28 20:03:51.000000 virny-0.5.0/virny/utils/validation.py
+drwxr-xr-x   0 denys_herasymuk   (501) staff       (20)        0 2024-06-02 13:54:06.736227 virny-0.5.0/virny.egg-info/
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     6956 2024-06-02 13:54:06.000000 virny-0.5.0/virny.egg-info/PKG-INFO
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)     2785 2024-06-02 13:54:06.000000 virny-0.5.0/virny.egg-info/SOURCES.txt
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)        1 2024-06-02 13:54:06.000000 virny-0.5.0/virny.egg-info/dependency_links.txt
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)      651 2024-06-02 13:54:06.000000 virny-0.5.0/virny.egg-info/requires.txt
+-rw-r--r--   0 denys_herasymuk   (501) staff       (20)       12 2024-06-02 13:54:06.000000 virny-0.5.0/virny.egg-info/top_level.txt
```

### Comparing `virny-0.4.0/LICENSE` & `virny-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/PKG-INFO` & `virny-0.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virny
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python library for in-depth profiling of model performance across overall and disparity dimensions
 Home-page: https://github.com/DataResponsibly/Virny
 Author: Denys Herasymuk
 Author-email: denis.gerasymuk799@gmail.com
 License: BSD-3
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -49,15 +49,16 @@
 </p>
 
 
 ## 📜 Description
 
 **Virny** is a Python library for in-depth profiling of model performance across overall and disparity dimensions. 
 In addition to its metric computation capabilities, the library provides an interactive tool called _VirnyView_ 
-to streamline responsible model selection and generate nutritional labels for ML models. 
+to streamline responsible model selection and generate nutritional labels for ML models.
+
 The Virny library was developed based on three fundamental principles: 
 
 1) easy extensibility of model analysis capabilities;
 
 2) compatibility to user-defined/custom datasets and model types;
 
 3) simple composition of disparity metrics based on the context of use.
@@ -82,41 +83,60 @@
 
 * [Introduction](https://dataresponsibly.github.io/Virny/)
 * [API Reference](https://dataresponsibly.github.io/Virny/api/overview/)
 * [Use Case Examples](https://dataresponsibly.github.io/Virny/examples/Multiple_Models_Interface_Use_Case/)
 * [Interactive Demo](https://huggingface.co/spaces/denys-herasymuk/virny-demo)
 
 
-## 💡 Features
+## 😎 Why Virny
+
+In contrast to existing fairness software libraries and model card generating frameworks, our system stands out in four key aspects:
+
+1. Virny facilitates the measurement of **all normatively important performance dimensions** (including _fairness_, _stability_, and _uncertainty_) for a set of initialized models, both overall and broken down by user-defined subgroups of interest.
+
+2. Virny enables data scientists to analyze performance using **multiple sensitive attributes** (including _non-binary_) and their _intersections_.
+
+3. Virny offers **diverse APIs for metric computation**, designed to analyze multiple models in a single execution, assessing stability and uncertainty on correct and incorrect predictions broken down by protected groups, and testing models on multiple test sets, including in-domain and out-of-domain.
+
+4. Virny implements streamlined flow design tailored for **responsible model selection**, reducing the complexity associated with numerous model types, performance dimensions, and data-centric and model-centric interventions.
+
+
+## 💡 List of Features
 
-* Entire pipeline for profiling model accuracy, stability, uncertainty, and fairness
+* Profiling of all normatively important performance dimensions: accuracy, stability, uncertainty, and fairness
 * Ability to analyze non-binary sensitive attributes and their intersections
-* Compatibility with [pre-, in-, and post-processors](https://aif360.readthedocs.io/en/latest/modules/algorithms.html#) for fairness enhancement from AIF360
 * Convenient metric computation interfaces: an interface for multiple models, an interface for multiple test sets, and an interface for saving results into a user-defined database
+* Interactive _VirnyView_ visualizer that profiles dataset properties related to protected groups, computes comprehensive [nutritional labels](http://sites.computer.org/debull/A19sept/p13.pdf) for individual models, compares multiple models according to multiple metrics, and guides users through model selection
+* Compatibility with [pre-, in-, and post-processors](https://aif360.readthedocs.io/en/latest/modules/algorithms.html#) for fairness enhancement from AIF360
 * An `error_analysis` computation mode to analyze model stability and confidence for correct and incorrect prodictions broken down by groups
 * Metric static and interactive visualizations
 * Data loaders with subsampling for popular fair-ML benchmark datasets
-* User-friendly parameters input via config yaml files
-* Check out [our documentation](https://dataresponsibly.github.io/Virny/) for a comprehensive overview
+* User-friendly parameters input via config yaml files 
 
+Check out [our documentation](https://dataresponsibly.github.io/Virny/) for a comprehensive overview.
 
-## 📖 Library Overview
 
-![Virny_Architecture](https://github.com/DataResponsibly/Virny/assets/42843889/91620e0f-11ff-4093-8fb6-c88c90bff711)
+## 🤗 Affiliations
+
+![NYU-UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-071bf184-f0e3-4a3e-94dc-c0d1c7784143.png)
 
-The software framework decouples the process of model profiling into several stages, including **subgroup metric computation**,
-**disparity metric composition**, and **metric visualization**. This separation empowers data scientists with greater control and
-flexibility in employing the library, both during model development and for post-deployment monitoring. The above figure demonstrates
-how the library constructs a pipeline for model analysis. Inputs to a user interface are shown in green, pipeline stages are shown in blue,
-and the output of each stage is shown in purple.
 
+## 💬 Citation
 
-## 🤗 Affiliations
+If Virny has been useful to you, and you would like to cite it in a scientific publication, please refer to the [paper](https://dl.acm.org/doi/abs/10.1145/3626246.3654738) published at SIGMOD:
 
-![NYU-UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-071bf184-f0e3-4a3e-94dc-c0d1c7784143.png)
+```bibtex
+@inproceedings{herasymuk2024responsible,
+  title={Responsible Model Selection with Virny and VirnyView},
+  author={Herasymuk, Denys and Arif Khan, Falaah and Stoyanovich, Julia},
+  booktitle={Companion of the 2024 International Conference on Management of Data},
+  pages={488--491},
+  year={2024}
+}
+```
 
 
 ## 📝 License
 
 **Virny** is free and open-source software licensed under the [3-clause BSD license](https://github.com/DataResponsibly/Virny/blob/main/LICENSE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: virny Version: 0.4.0 Summary: Python library for
+Metadata-Version: 2.1 Name: virny Version: 0.5.0 Summary: Python library for
 in-depth profiling of model performance across overall and disparity dimensions
 Home-page: https://github.com/DataResponsibly/Virny Author: Denys Herasymuk
 Author-email: denis.gerasymuk799@gmail.com License: BSD-3 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Operating
@@ -27,34 +27,50 @@
 notebook](https://huggingface.co/spaces/denys-herasymuk/virny-demo/blob/main/
 notebooks/ACS_Income_Demo.ipynb). ## ð  Installation Virny supports **Python
 3.8 and 3.9** and can be installed with `pip`: ```bash pip install virny ``` ##
 ð Documentation * [Introduction](https://dataresponsibly.github.io/Virny/) *
 [API Reference](https://dataresponsibly.github.io/Virny/api/overview/) * [Use
 Case Examples](https://dataresponsibly.github.io/Virny/examples/
 Multiple_Models_Interface_Use_Case/) * [Interactive Demo](https://
-huggingface.co/spaces/denys-herasymuk/virny-demo) ## ð¡ Features * Entire
-pipeline for profiling model accuracy, stability, uncertainty, and fairness *
-Ability to analyze non-binary sensitive attributes and their intersections *
+huggingface.co/spaces/denys-herasymuk/virny-demo) ## ð Why Virny In contrast
+to existing fairness software libraries and model card generating frameworks,
+our system stands out in four key aspects: 1. Virny facilitates the measurement
+of **all normatively important performance dimensions** (including _fairness_,
+_stability_, and _uncertainty_) for a set of initialized models, both overall
+and broken down by user-defined subgroups of interest. 2. Virny enables data
+scientists to analyze performance using **multiple sensitive attributes**
+(including _non-binary_) and their _intersections_. 3. Virny offers **diverse
+APIs for metric computation**, designed to analyze multiple models in a single
+execution, assessing stability and uncertainty on correct and incorrect
+predictions broken down by protected groups, and testing models on multiple
+test sets, including in-domain and out-of-domain. 4. Virny implements
+streamlined flow design tailored for **responsible model selection**, reducing
+the complexity associated with numerous model types, performance dimensions,
+and data-centric and model-centric interventions. ## ð¡ List of Features *
+Profiling of all normatively important performance dimensions: accuracy,
+stability, uncertainty, and fairness * Ability to analyze non-binary sensitive
+attributes and their intersections * Convenient metric computation interfaces:
+an interface for multiple models, an interface for multiple test sets, and an
+interface for saving results into a user-defined database * Interactive
+_VirnyView_ visualizer that profiles dataset properties related to protected
+groups, computes comprehensive [nutritional labels](http://sites.computer.org/
+debull/A19sept/p13.pdf) for individual models, compares multiple models
+according to multiple metrics, and guides users through model selection *
 Compatibility with [pre-, in-, and post-processors](https://
 aif360.readthedocs.io/en/latest/modules/algorithms.html#) for fairness
-enhancement from AIF360 * Convenient metric computation interfaces: an
-interface for multiple models, an interface for multiple test sets, and an
-interface for saving results into a user-defined database * An `error_analysis`
-computation mode to analyze model stability and confidence for correct and
-incorrect prodictions broken down by groups * Metric static and interactive
-visualizations * Data loaders with subsampling for popular fair-ML benchmark
-datasets * User-friendly parameters input via config yaml files * Check out
-[our documentation](https://dataresponsibly.github.io/Virny/) for a
-comprehensive overview ## ð Library Overview ![Virny_Architecture](https://
-github.com/DataResponsibly/Virny/assets/42843889/91620e0f-11ff-4093-8fb6-
-c88c90bff711) The software framework decouples the process of model profiling
-into several stages, including **subgroup metric computation**, **disparity
-metric composition**, and **metric visualization**. This separation empowers
-data scientists with greater control and flexibility in employing the library,
-both during model development and for post-deployment monitoring. The above
-figure demonstrates how the library constructs a pipeline for model analysis.
-Inputs to a user interface are shown in green, pipeline stages are shown in
-blue, and the output of each stage is shown in purple. ## ð¤ Affiliations !
-[NYU-UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-
-071bf184-f0e3-4a3e-94dc-c0d1c7784143.png) ## ð License **Virny** is free and
-open-source software licensed under the [3-clause BSD license](https://
+enhancement from AIF360 * An `error_analysis` computation mode to analyze model
+stability and confidence for correct and incorrect prodictions broken down by
+groups * Metric static and interactive visualizations * Data loaders with
+subsampling for popular fair-ML benchmark datasets * User-friendly parameters
+input via config yaml files Check out [our documentation](https://
+dataresponsibly.github.io/Virny/) for a comprehensive overview. ## ð¤
+Affiliations ![NYU-UCU-Logos](https://user-images.githubusercontent.com/
+42843889/216840888-071bf184-f0e3-4a3e-94dc-c0d1c7784143.png) ## ð¬ Citation
+If Virny has been useful to you, and you would like to cite it in a scientific
+publication, please refer to the [paper](https://dl.acm.org/doi/abs/10.1145/
+3626246.3654738) published at SIGMOD: ```bibtex @inproceedings
+{herasymuk2024responsible, title={Responsible Model Selection with Virny and
+VirnyView}, author={Herasymuk, Denys and Arif Khan, Falaah and Stoyanovich,
+Julia}, booktitle={Companion of the 2024 International Conference on Management
+of Data}, pages={488--491}, year={2024} } ``` ## ð License **Virny** is free
+and open-source software licensed under the [3-clause BSD license](https://
 github.com/DataResponsibly/Virny/blob/main/LICENSE).
```

### Comparing `virny-0.4.0/README.md` & `virny-0.5.0/virny.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: virny
+Version: 0.5.0
+Summary: Python library for in-depth profiling of model performance across overall and disparity dimensions
+Home-page: https://github.com/DataResponsibly/Virny
+Author: Denys Herasymuk
+Author-email: denis.gerasymuk799@gmail.com
+License: BSD-3
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
 # Virny Software Library
 
 <p align="left">
   <!-- Tests -->
   <a href="https://github.com/DataResponsibly/Virny/actions/workflows/ci.yml">
     <img src="https://github.com/DataResponsibly/Virny/actions/workflows/ci.yml/badge.svg" alt="CI Pipeline">
   </a>
@@ -28,15 +49,16 @@
 </p>
 
 
 ## 📜 Description
 
 **Virny** is a Python library for in-depth profiling of model performance across overall and disparity dimensions. 
 In addition to its metric computation capabilities, the library provides an interactive tool called _VirnyView_ 
-to streamline responsible model selection and generate nutritional labels for ML models. 
+to streamline responsible model selection and generate nutritional labels for ML models.
+
 The Virny library was developed based on three fundamental principles: 
 
 1) easy extensibility of model analysis capabilities;
 
 2) compatibility to user-defined/custom datasets and model types;
 
 3) simple composition of disparity metrics based on the context of use.
@@ -61,39 +83,60 @@
 
 * [Introduction](https://dataresponsibly.github.io/Virny/)
 * [API Reference](https://dataresponsibly.github.io/Virny/api/overview/)
 * [Use Case Examples](https://dataresponsibly.github.io/Virny/examples/Multiple_Models_Interface_Use_Case/)
 * [Interactive Demo](https://huggingface.co/spaces/denys-herasymuk/virny-demo)
 
 
-## 💡 Features
+## 😎 Why Virny
+
+In contrast to existing fairness software libraries and model card generating frameworks, our system stands out in four key aspects:
+
+1. Virny facilitates the measurement of **all normatively important performance dimensions** (including _fairness_, _stability_, and _uncertainty_) for a set of initialized models, both overall and broken down by user-defined subgroups of interest.
+
+2. Virny enables data scientists to analyze performance using **multiple sensitive attributes** (including _non-binary_) and their _intersections_.
 
-* Entire pipeline for profiling model accuracy, stability, uncertainty, and fairness
+3. Virny offers **diverse APIs for metric computation**, designed to analyze multiple models in a single execution, assessing stability and uncertainty on correct and incorrect predictions broken down by protected groups, and testing models on multiple test sets, including in-domain and out-of-domain.
+
+4. Virny implements streamlined flow design tailored for **responsible model selection**, reducing the complexity associated with numerous model types, performance dimensions, and data-centric and model-centric interventions.
+
+
+## 💡 List of Features
+
+* Profiling of all normatively important performance dimensions: accuracy, stability, uncertainty, and fairness
 * Ability to analyze non-binary sensitive attributes and their intersections
-* Compatibility with [pre-, in-, and post-processors](https://aif360.readthedocs.io/en/latest/modules/algorithms.html#) for fairness enhancement from AIF360
 * Convenient metric computation interfaces: an interface for multiple models, an interface for multiple test sets, and an interface for saving results into a user-defined database
+* Interactive _VirnyView_ visualizer that profiles dataset properties related to protected groups, computes comprehensive [nutritional labels](http://sites.computer.org/debull/A19sept/p13.pdf) for individual models, compares multiple models according to multiple metrics, and guides users through model selection
+* Compatibility with [pre-, in-, and post-processors](https://aif360.readthedocs.io/en/latest/modules/algorithms.html#) for fairness enhancement from AIF360
 * An `error_analysis` computation mode to analyze model stability and confidence for correct and incorrect prodictions broken down by groups
 * Metric static and interactive visualizations
 * Data loaders with subsampling for popular fair-ML benchmark datasets
-* User-friendly parameters input via config yaml files
-* Check out [our documentation](https://dataresponsibly.github.io/Virny/) for a comprehensive overview
+* User-friendly parameters input via config yaml files 
 
+Check out [our documentation](https://dataresponsibly.github.io/Virny/) for a comprehensive overview.
 
-## 📖 Library Overview
 
-![Virny_Architecture](https://github.com/DataResponsibly/Virny/assets/42843889/91620e0f-11ff-4093-8fb6-c88c90bff711)
+## 🤗 Affiliations
 
-The software framework decouples the process of model profiling into several stages, including **subgroup metric computation**,
-**disparity metric composition**, and **metric visualization**. This separation empowers data scientists with greater control and
-flexibility in employing the library, both during model development and for post-deployment monitoring. The above figure demonstrates
-how the library constructs a pipeline for model analysis. Inputs to a user interface are shown in green, pipeline stages are shown in blue,
-and the output of each stage is shown in purple.
+![NYU-UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-071bf184-f0e3-4a3e-94dc-c0d1c7784143.png)
 
 
-## 🤗 Affiliations
+## 💬 Citation
 
-![NYU-UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-071bf184-f0e3-4a3e-94dc-c0d1c7784143.png)
+If Virny has been useful to you, and you would like to cite it in a scientific publication, please refer to the [paper](https://dl.acm.org/doi/abs/10.1145/3626246.3654738) published at SIGMOD:
+
+```bibtex
+@inproceedings{herasymuk2024responsible,
+  title={Responsible Model Selection with Virny and VirnyView},
+  author={Herasymuk, Denys and Arif Khan, Falaah and Stoyanovich, Julia},
+  booktitle={Companion of the 2024 International Conference on Management of Data},
+  pages={488--491},
+  year={2024}
+}
+```
 
 
 ## 📝 License
 
 **Virny** is free and open-source software licensed under the [3-clause BSD license](https://github.com/DataResponsibly/Virny/blob/main/LICENSE).
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,17 @@
-# Virny Software Library
+Metadata-Version: 2.1 Name: virny Version: 0.5.0 Summary: Python library for
+in-depth profiling of model performance across overall and disparity dimensions
+Home-page: https://github.com/DataResponsibly/Virny Author: Denys Herasymuk
+Author-email: denis.gerasymuk799@gmail.com License: BSD-3 Platform: UNKNOWN
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: BSD License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Operating
+System :: OS Independent Description-Content-Type: text/markdown Provides-
+Extra: dev Provides-Extra: docs License-File: LICENSE # Virny Software Library
 _[_C_I_ _P_i_p_e_l_i_n_e_]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_[_p_y_p_i_]_[_b_s_d___3___l_i_c_e_n_s_e_][code_size][last_commit]
 ## ð Description **Virny** is a Python library for in-depth profiling of
 model performance across overall and disparity dimensions. In addition to its
 metric computation capabilities, the library provides an interactive tool
 called _VirnyView_ to streamline responsible model selection and generate
 nutritional labels for ML models. The Virny library was developed based on
 three fundamental principles: 1) easy extensibility of model analysis
@@ -18,34 +27,50 @@
 notebook](https://huggingface.co/spaces/denys-herasymuk/virny-demo/blob/main/
 notebooks/ACS_Income_Demo.ipynb). ## ð  Installation Virny supports **Python
 3.8 and 3.9** and can be installed with `pip`: ```bash pip install virny ``` ##
 ð Documentation * [Introduction](https://dataresponsibly.github.io/Virny/) *
 [API Reference](https://dataresponsibly.github.io/Virny/api/overview/) * [Use
 Case Examples](https://dataresponsibly.github.io/Virny/examples/
 Multiple_Models_Interface_Use_Case/) * [Interactive Demo](https://
-huggingface.co/spaces/denys-herasymuk/virny-demo) ## ð¡ Features * Entire
-pipeline for profiling model accuracy, stability, uncertainty, and fairness *
-Ability to analyze non-binary sensitive attributes and their intersections *
+huggingface.co/spaces/denys-herasymuk/virny-demo) ## ð Why Virny In contrast
+to existing fairness software libraries and model card generating frameworks,
+our system stands out in four key aspects: 1. Virny facilitates the measurement
+of **all normatively important performance dimensions** (including _fairness_,
+_stability_, and _uncertainty_) for a set of initialized models, both overall
+and broken down by user-defined subgroups of interest. 2. Virny enables data
+scientists to analyze performance using **multiple sensitive attributes**
+(including _non-binary_) and their _intersections_. 3. Virny offers **diverse
+APIs for metric computation**, designed to analyze multiple models in a single
+execution, assessing stability and uncertainty on correct and incorrect
+predictions broken down by protected groups, and testing models on multiple
+test sets, including in-domain and out-of-domain. 4. Virny implements
+streamlined flow design tailored for **responsible model selection**, reducing
+the complexity associated with numerous model types, performance dimensions,
+and data-centric and model-centric interventions. ## ð¡ List of Features *
+Profiling of all normatively important performance dimensions: accuracy,
+stability, uncertainty, and fairness * Ability to analyze non-binary sensitive
+attributes and their intersections * Convenient metric computation interfaces:
+an interface for multiple models, an interface for multiple test sets, and an
+interface for saving results into a user-defined database * Interactive
+_VirnyView_ visualizer that profiles dataset properties related to protected
+groups, computes comprehensive [nutritional labels](http://sites.computer.org/
+debull/A19sept/p13.pdf) for individual models, compares multiple models
+according to multiple metrics, and guides users through model selection *
 Compatibility with [pre-, in-, and post-processors](https://
 aif360.readthedocs.io/en/latest/modules/algorithms.html#) for fairness
-enhancement from AIF360 * Convenient metric computation interfaces: an
-interface for multiple models, an interface for multiple test sets, and an
-interface for saving results into a user-defined database * An `error_analysis`
-computation mode to analyze model stability and confidence for correct and
-incorrect prodictions broken down by groups * Metric static and interactive
-visualizations * Data loaders with subsampling for popular fair-ML benchmark
-datasets * User-friendly parameters input via config yaml files * Check out
-[our documentation](https://dataresponsibly.github.io/Virny/) for a
-comprehensive overview ## ð Library Overview ![Virny_Architecture](https://
-github.com/DataResponsibly/Virny/assets/42843889/91620e0f-11ff-4093-8fb6-
-c88c90bff711) The software framework decouples the process of model profiling
-into several stages, including **subgroup metric computation**, **disparity
-metric composition**, and **metric visualization**. This separation empowers
-data scientists with greater control and flexibility in employing the library,
-both during model development and for post-deployment monitoring. The above
-figure demonstrates how the library constructs a pipeline for model analysis.
-Inputs to a user interface are shown in green, pipeline stages are shown in
-blue, and the output of each stage is shown in purple. ## ð¤ Affiliations !
-[NYU-UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-
-071bf184-f0e3-4a3e-94dc-c0d1c7784143.png) ## ð License **Virny** is free and
-open-source software licensed under the [3-clause BSD license](https://
+enhancement from AIF360 * An `error_analysis` computation mode to analyze model
+stability and confidence for correct and incorrect prodictions broken down by
+groups * Metric static and interactive visualizations * Data loaders with
+subsampling for popular fair-ML benchmark datasets * User-friendly parameters
+input via config yaml files Check out [our documentation](https://
+dataresponsibly.github.io/Virny/) for a comprehensive overview. ## ð¤
+Affiliations ![NYU-UCU-Logos](https://user-images.githubusercontent.com/
+42843889/216840888-071bf184-f0e3-4a3e-94dc-c0d1c7784143.png) ## ð¬ Citation
+If Virny has been useful to you, and you would like to cite it in a scientific
+publication, please refer to the [paper](https://dl.acm.org/doi/abs/10.1145/
+3626246.3654738) published at SIGMOD: ```bibtex @inproceedings
+{herasymuk2024responsible, title={Responsible Model Selection with Virny and
+VirnyView}, author={Herasymuk, Denys and Arif Khan, Falaah and Stoyanovich,
+Julia}, booktitle={Companion of the 2024 International Conference on Management
+of Data}, pages={488--491}, year={2024} } ``` ## ð License **Virny** is free
+and open-source software licensed under the [3-clause BSD license](https://
 github.com/DataResponsibly/Virny/blob/main/LICENSE).
```

### Comparing `virny-0.4.0/setup.py` & `virny-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/tests/analyzers/test_subgroup_error_analyzer.py` & `virny-0.5.0/tests/analyzers/test_subgroup_error_analyzer.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,18 +24,16 @@
     expected_TNR = TN/(TN+FP)
     expected_PPV = TP/(TP+FP)
     expected_FNR = FN/(FN+TP)
     expected_FPR = FP/(FP+TN)
     expected_ACCURACY = (TP+TN)/(TP+TN+FP+FN)
     expected_F1 = (2*TP)/(2*TP+FP+FN)
     expected_SELECTION_RATE = (TP+FP)/(TP+FP+TN+FN)
-    expected_POSITIVE_RATE = (TP+FP)/(TP+FN)
 
     assert abs(prediction_metrics[TPR] - expected_TPR) < alpha
     assert abs(prediction_metrics[TNR] - expected_TNR) < alpha
     assert abs(prediction_metrics[PPV] - expected_PPV) < alpha
     assert abs(prediction_metrics[FNR] - expected_FNR) < alpha
     assert abs(prediction_metrics[FPR] - expected_FPR) < alpha
     assert abs(prediction_metrics[ACCURACY] - expected_ACCURACY) < alpha
     assert abs(prediction_metrics[F1] - expected_F1) < alpha
     assert abs(prediction_metrics[SELECTION_RATE] - expected_SELECTION_RATE) < alpha
-    assert abs(prediction_metrics[POSITIVE_RATE] - expected_POSITIVE_RATE) < alpha
```

### Comparing `virny-0.4.0/tests/custom_classes/test_metrics_composer.py` & `virny-0.5.0/tests/custom_classes/test_metrics_composer.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/tests/preprocessing/test_basic_preprocessing.py` & `virny-0.5.0/tests/preprocessing/test_basic_preprocessing.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/tests/user_interfaces/test_compute_model_metrics.py` & `virny-0.5.0/tests/user_interfaces/test_compute_model_metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,31 +7,35 @@
                    COMPAS_RF_expected_metrics)
 
 from virny.configs.constants import *
 from virny.utils.protected_groups_partitioning import create_test_protected_groups
 from virny.analyzers.subgroup_variance_calculator import SubgroupVarianceCalculator
 from virny.analyzers.subgroup_error_analyzer import SubgroupErrorAnalyzer
 from virny.utils.stability_utils import count_prediction_metrics
-from virny.datasets.data_loaders import CompasWithoutSensitiveAttrsDataset
+from virny.datasets import CompasWithoutSensitiveAttrsDataset
 from virny.preprocessing.basic_preprocessing import preprocess_dataset
 
 
 def test_subgroup_variance_and_error_analyzers(COMPAS_y_test, COMPAS_RF_bootstrap_predictions, COMPAS_RF_expected_preds,
                                                COMPAS_RF_expected_metrics):
     dataset_split_seed = 42
     test_set_fraction = 0.2
 
     data_loader = CompasWithoutSensitiveAttrsDataset()
     sensitive_attributes_dct = {'sex': 1, 'race': 'African-American', 'sex&race': None}
     column_transformer = ColumnTransformer(transformers=[
         ('categorical_features', OneHotEncoder(handle_unknown='ignore', sparse=False), data_loader.categorical_columns),
         ('numerical_features', StandardScaler(), data_loader.numerical_columns),
     ])
-    base_flow_dataset = preprocess_dataset(data_loader, column_transformer, test_set_fraction, dataset_split_seed)
-    test_protected_groups = create_test_protected_groups(base_flow_dataset.X_test, base_flow_dataset.init_features_df,
+    base_flow_dataset = preprocess_dataset(data_loader=data_loader,
+                                           column_transformer=column_transformer,
+                                           sensitive_attributes_dct=sensitive_attributes_dct,
+                                           test_set_fraction=test_set_fraction,
+                                           dataset_split_seed=dataset_split_seed)
+    test_protected_groups = create_test_protected_groups(base_flow_dataset.X_test, base_flow_dataset.init_sensitive_attrs_df,
                                                          sensitive_attributes_dct)
 
     y_preds, prediction_metrics = count_prediction_metrics(COMPAS_y_test, COMPAS_RF_bootstrap_predictions)
     y_preds = pd.Series(y_preds, index=base_flow_dataset.y_test.index)
     subgroup_variance_calculator = SubgroupVarianceCalculator(X_test=base_flow_dataset.X_test,
                                                               y_test=base_flow_dataset.y_test,
                                                               sensitive_attributes_dct=sensitive_attributes_dct,
@@ -72,16 +76,15 @@
                                     TPR,
                                     TNR,
                                     PPV,
                                     FNR,
                                     FPR,
                                     F1,
                                     ACCURACY,
-                                    SELECTION_RATE,
-                                    POSITIVE_RATE])
+                                    SELECTION_RATE])
     # Check stability metrics
     compare_metric_dfs(expected_composed_metrics_df=COMPAS_RF_expected_metrics,
                        actual_composed_metrics_df=metrics_df,
                        model_name='RandomForestClassifier',
                        groups=['overall', 'sex_priv', 'sex_dis', 'race_priv', 'race_dis', 'sex&race_priv', 'sex&race_dis'],
                        metrics_lst=[STD, IQR, JITTER, LABEL_STABILITY])
     # Check uncertainty metrics
```

### Comparing `virny-0.4.0/tests/utils/test_common_helpers.py` & `virny-0.5.0/tests/utils/test_common_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,10 +78,10 @@
 
 def test_confusion_matrix_metrics():
     y_true = np.array([0, 1, 0, 1, 0, 1, 0, 1, 0, 1])
     y_preds = np.array([0, 1, 0, 1, 0, 1, 0, 1, 0, 1])
 
     actual_metrics = confusion_matrix_metrics(y_true, y_preds)
 
-    required_fields = ['TPR', 'TNR', 'PPV', 'FNR', 'FPR', 'Accuracy', 'F1', 'Selection-Rate', 'Positive-Rate']
+    required_fields = ['TPR', 'TNR', 'PPV', 'FNR', 'FPR', 'Accuracy', 'F1', 'Selection-Rate']
     for field in required_fields:
         assert field in actual_metrics.keys()
```

### Comparing `virny-0.4.0/tests/utils/test_data_viz_utils.py` & `virny-0.5.0/tests/utils/test_data_viz_utils.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/tests/utils/test_protected_groups_partitioning.py` & `virny-0.5.0/tests/utils/test_protected_groups_partitioning.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/tests/utils/test_stability_utils.py` & `virny-0.5.0/tests/utils/test_stability_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 def test_generate_bootstrap_true1(compas_without_sensitive_attrs_dataset_class, config_params):
     column_transformer = ColumnTransformer(transformers=[
         ('categorical_features', OneHotEncoder(handle_unknown='ignore', sparse=False), compas_without_sensitive_attrs_dataset_class.categorical_columns),
         ('numerical_features', StandardScaler(), compas_without_sensitive_attrs_dataset_class.numerical_columns),
     ])
     base_flow_ds = preprocess_dataset(compas_without_sensitive_attrs_dataset_class,
                                       column_transformer,
+                                      sensitive_attributes_dct={'sex': 1, 'race': 'African-American', 'sex&race': None},
                                       test_set_fraction=0.2,
                                       dataset_split_seed=42)
     boostrap_size = int(config_params.bootstrap_fraction * base_flow_ds.X_train_val.shape[0])
     X_sample, y_sample = generate_bootstrap(base_flow_ds.X_train_val,
                                             base_flow_ds.y_train_val,
                                             boostrap_size,
                                             with_replacement=True)
```

### Comparing `virny-0.4.0/virny/analyzers/__init__.py` & `virny-0.5.0/virny/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/analyzers/abstract_overall_variance_analyzer.py` & `virny-0.5.0/virny/analyzers/abstract_overall_variance_analyzer.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,39 +31,42 @@
         Processed features test set
     y_test
         Targets test set
     dataset_name
         Name of dataset, used for correct results naming
     n_estimators
         Number of estimators in ensemble to measure base_model stability
+    random_state
+        [Optional] Controls the randomness of the bootstrap approach for model arbitrariness evaluation
     with_predict_proba
         [Optional] A flag if model can return probabilities for its predictions.
          If no, only metrics based on labels (not labels and probabilities) will be computed.
     notebook_logs_stdout
         [Optional] True, if this interface was execute in a Jupyter notebook,
          False, otherwise.
     verbose
         [Optional] Level of logs printing. The greater level provides more logs.
          As for now, 0, 1, 2 levels are supported.
 
     """
 
     def __init__(self, base_model, base_model_name: str, bootstrap_fraction: float,
                  X_train: pd.DataFrame, y_train: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame,
-                 dataset_name: str, n_estimators: int, with_predict_proba: bool = True,
+                 dataset_name: str, n_estimators: int, random_state: int = None, with_predict_proba: bool = True,
                  notebook_logs_stdout: bool = False, verbose: int = 0):
         self.base_model = base_model
         self.base_model_name = base_model_name
         self.bootstrap_fraction = bootstrap_fraction
         self.dataset_name = dataset_name
         self.n_estimators = n_estimators
         self.models_lst = [deepcopy(base_model) for _ in range(n_estimators)]
+        self.random_state = random_state
+        self.with_predict_proba = with_predict_proba
         self.models_predictions = None
         self.prediction_metrics = None
-        self.with_predict_proba = with_predict_proba
 
         self._notebook_logs_stdout = notebook_logs_stdout
         self._verbose = verbose
         self._logger = get_logger(verbose)
 
         self.X_train = X_train
         self.y_train = y_train
@@ -141,19 +144,37 @@
                  colour="blue",
                  mininterval=10,
                  file=sys.stdout)
 
         # Train and test each estimator in models_predictions
         for idx in cycle_range:
             classifier = self.models_lst[idx]
+
+            # If True, fit the classifier. Otherwise, use already fitted classifier.
             if with_fit:
-                X_sample, y_sample = generate_bootstrap(self.X_train, self.y_train, boostrap_size, with_replacement)
+                classifier_random_state = self.random_state + idx + 1 if self.random_state is not None else None
+                X_sample, y_sample = generate_bootstrap(features=self.X_train,
+                                                        labels=self.y_train,
+                                                        boostrap_size=boostrap_size,
+                                                        with_replacement=with_replacement,
+                                                        random_state=classifier_random_state)
+                if 'random_state' in classifier.get_params():
+                    classifier.set_params(random_state=classifier_random_state)
                 classifier = self._fit_model(classifier, X_sample, y_sample)
-            models_predictions[idx] = self._batch_predict_proba(classifier, self.X_test)
+
+            # Use a predict_proba method if the classifier supports it.
+            # Note that model predictions do not preserve X_test indexes.
+            # Indexes of the predictions will be aligned with X_test later in the pipeline.
+            if self.with_predict_proba:
+                models_predictions[idx] = self._batch_predict_proba(classifier, self.X_test)
+            else:
+                models_predictions[idx] = self._batch_predict(classifier, self.X_test)
+
             self.models_lst[idx] = classifier
+
             # Force garbage collection to avoid out of memory error
             if with_fit and ((idx + 1) % 10 == 0 or (idx + 1) == self.n_estimators):
                 gc.collect()
 
         if self._verbose >= 1:
             print('\n', flush=True)
         self._logger.info('Successfully tested classifiers by bootstrap')
```

### Comparing `virny-0.4.0/virny/analyzers/abstract_subgroup_analyzer.py` & `virny-0.5.0/virny/analyzers/abstract_subgroup_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import pandas as pd
 
 from colorama import Fore
 from datetime import datetime, timezone
 from abc import ABCMeta, abstractmethod
 
-from virny.configs.constants import (ComputationMode, TPR, TNR, PPV, FPR, FNR, ACCURACY, F1,
-                                     SELECTION_RATE, POSITIVE_RATE)
+from virny.configs.constants import ComputationMode, TPR, TNR, PPV, FPR, FNR, ACCURACY, F1, SELECTION_RATE
 
 
 class AbstractSubgroupAnalyzer(metaclass=ABCMeta):
     """
     Abstract class for a subgroup analyzer to compute metrics for subgroups.
 
     Parameters
@@ -90,15 +89,14 @@
                         TNR: None,
                         PPV: None,
                         FNR: None,
                         FPR: None,
                         ACCURACY: None,
                         F1: None,
                         SELECTION_RATE: None,
-                        POSITIVE_RATE: None,
                     }
                 else:
                     metrics_dct = self._compute_metrics(self.y_test[partition_indexes], y_preds[partition_indexes])
                 metrics_dct['Sample_Size'] = len(partition_indexes)
                 results[group_partition_name] = metrics_dct
 
         return results
```

### Comparing `virny-0.4.0/virny/analyzers/batch_overall_variance_analyzer.py` & `virny-0.5.0/virny/analyzers/batch_overall_variance_analyzer.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,38 +26,41 @@
         Targets test set
     target_column
         Name of the target column
     dataset_name
         Name of dataset, used for correct results naming
     n_estimators
         Number of estimators in ensemble to measure base_model stability
+    random_state
+        [Optional] Controls the randomness of the bootstrap approach for model arbitrariness evaluation
     with_predict_proba
         [Optional] A flag if model can return probabilities for its predictions.
          If no, only metrics based on labels (not labels and probabilities) will be computed.
     notebook_logs_stdout
         [Optional] True, if this interface was execute in a Jupyter notebook,
          False, otherwise.
     verbose
         [Optional] Level of logs printing. The greater level provides more logs.
          As for now, 0, 1, 2 levels are supported.
 
     """
     def __init__(self, base_model, base_model_name: str, bootstrap_fraction: float,
                  X_train: pd.DataFrame, y_train: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame,
-                 target_column: str, dataset_name: str, n_estimators: int, 
+                 target_column: str, dataset_name: str, n_estimators: int, random_state: int = None,
                  with_predict_proba: bool = True, notebook_logs_stdout: bool = False, verbose: int = 0):
         super().__init__(base_model=base_model,
                          base_model_name=base_model_name,
                          bootstrap_fraction=bootstrap_fraction,
                          X_train=X_train,
                          y_train=y_train,
                          X_test=X_test,
                          y_test=y_test,
                          dataset_name=dataset_name,
                          n_estimators=n_estimators,
+                         random_state=random_state,
                          with_predict_proba=with_predict_proba,
                          notebook_logs_stdout=notebook_logs_stdout,
                          verbose=verbose)
         self.target_column = target_column
 
     def _fit_model(self, classifier, X_train: np.ndarray, y_train: np.ndarray):
         """
```

### Comparing `virny-0.4.0/virny/analyzers/batch_overall_variance_analyzer_postprocessing.py` & `virny-0.5.0/virny/analyzers/batch_overall_variance_analyzer_postprocessing.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,29 +35,31 @@
         Targets test set
     target_column
         Name of the target column
     dataset_name
         Name of dataset, used for correct results naming
     n_estimators
         Number of estimators in ensemble to measure base_model stability
+    random_state
+        [Optional] Controls the randomness of the bootstrap approach for model arbitrariness evaluation
     with_predict_proba
         [Optional] A flag if model can return probabilities for its predictions.
          If no, only metrics based on labels (not labels and probabilities) will be computed.
     notebook_logs_stdout
         [Optional] True, if this interface was execute in a Jupyter notebook,
          False, otherwise.
     verbose
         [Optional] Level of logs printing. The greater level provides more logs.
          As for now, 0, 1, 2 levels are supported.
 
     """
     def __init__(self, postprocessor, sensitive_attribute: str, 
                  base_model, base_model_name: str, bootstrap_fraction: float,
                  X_train: pd.DataFrame, y_train: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame,
-                 target_column: str, dataset_name: str, n_estimators: int, 
+                 target_column: str, dataset_name: str, n_estimators: int, random_state: int = None,
                  with_predict_proba: bool = True, notebook_logs_stdout: bool = False, verbose: int = 0):
         if sensitive_attribute is None:
             raise ValueError('Sensitive attribute for postprocessing is not defined. '
                              'Please, set postprocessing_sensitive_attribute argument in the metric computation config.')
 
         super().__init__(base_model=base_model,
                          base_model_name=base_model_name,
@@ -65,14 +67,15 @@
                          X_train=X_train,
                          y_train=y_train,
                          X_test=X_test,
                          y_test=y_test,
                          target_column=target_column,
                          dataset_name=dataset_name,
                          n_estimators=n_estimators,
+                         random_state=random_state,
                          with_predict_proba=with_predict_proba,
                          notebook_logs_stdout=notebook_logs_stdout,
                          verbose=verbose)
 
         self.postprocessor = postprocessor
         self.sensitive_attribute = sensitive_attribute
         self.test_binary_label_dataset = construct_binary_label_dataset_from_df(X_test, y_test, target_column, sensitive_attribute)
@@ -113,26 +116,34 @@
                  mininterval=10,
                  file=sys.stdout)
 
         # Train and test each estimator in models_predictions
         for idx in cycle_range:
             classifier = self.models_lst[idx]
             if with_fit:
-                X_sample, y_sample = generate_bootstrap(self.X_train, self.y_train, boostrap_size, with_replacement)
+                classifier_random_state = self.random_state + idx + 1 if self.random_state is not None else None
+                X_sample, y_sample = generate_bootstrap(features=self.X_train,
+                                                        labels=self.y_train,
+                                                        boostrap_size=boostrap_size,
+                                                        with_replacement=with_replacement,
+                                                        random_state=classifier_random_state)
+                classifier.set_params(random_state=classifier_random_state)
                 classifier = self._fit_model(classifier, X_sample, y_sample)
                 
             # Force garbage collection to avoid out of memory error
             if with_fit and ((idx + 1) % 10 == 0 or (idx + 1) == self.n_estimators):
                 gc.collect()
 
             train_binary_label_dataset_sample = construct_binary_label_dataset_from_samples(X_sample, y_sample, self.X_train.columns, self.target_column, self.sensitive_attribute)
             train_binary_label_dataset_sample_pred = predict_on_binary_label_dataset(classifier, train_binary_label_dataset_sample)
             test_binary_label_dataset_pred = predict_on_binary_label_dataset(classifier, self.test_binary_label_dataset)
             postprocessor_fitted = self.postprocessor.fit(train_binary_label_dataset_sample, train_binary_label_dataset_sample_pred)
-            
+
+            # Note that model predictions do not preserve X_test indexes.
+            # Indexes of the predictions will be aligned with X_test later in the pipeline.
             models_predictions[idx] = postprocessor_fitted.predict(test_binary_label_dataset_pred).labels.ravel()
             self.models_lst[idx] = classifier
             
         if self._verbose >= 1:
             print('\n', flush=True)
         self._logger.info('Successfully tested classifiers by bootstrap')
```

### Comparing `virny-0.4.0/virny/analyzers/subgroup_error_analyzer.py` & `virny-0.5.0/virny/analyzers/subgroup_error_analyzer.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/analyzers/subgroup_variance_analyzer.py` & `virny-0.5.0/virny/analyzers/subgroup_variance_analyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 
-from virny.configs.constants import ModelSetting, ComputationMode
+from virny.configs.constants import ModelSetting
 from virny.custom_classes.base_dataset import BaseFlowDataset
 from virny.analyzers.subgroup_variance_calculator import SubgroupVarianceCalculator
 from virny.analyzers.batch_overall_variance_analyzer import BatchOverallVarianceAnalyzer
 from virny.analyzers.batch_overall_variance_analyzer_postprocessing import BatchOverallVarianceAnalyzerPostProcessing
 
 
 class SubgroupVarianceAnalyzer:
@@ -33,29 +33,37 @@
     test_protected_groups
         A dictionary of protected groups where keys are subgroup names,
          and values are X_test row indexes correspondent to this subgroup.
     postprocessor
         One of postprocessors from aif360 (https://aif360.readthedocs.io/en/stable/modules/algorithms.html#module-aif360.algorithms.postprocessing)
     postprocessing_sensitive_attribute
         A sensitive attribute to use for post-processing
+    random_state
+        [Optional] Controls the randomness of the bootstrap approach for model arbitrariness evaluation
     computation_mode
         [Optional] A non-default mode for metrics computation. Should be included in the ComputationMode enum.
+    with_predict_proba
+        [Optional] True, if models in models_config have a predict_proba method and can return probabilities for predictions,
+         False, otherwise. Note that if it is set to False, only metrics based on labels (not labels and probabilities) will be computed.
+         Ignored when a postprocessor is not None, and set to False in this case.
     notebook_logs_stdout
         [Optional] True, if this interface was execute in a Jupyter notebook,
          False, otherwise.
     verbose
         [Optional] Level of logs printing. The greater level provides more logs.
          As for now, 0, 1, 2 levels are supported.
 
     """
     def __init__(self, model_setting: ModelSetting, n_estimators: int, base_model, base_model_name: str,
                  bootstrap_fraction: float, dataset: BaseFlowDataset, dataset_name: str,
                  sensitive_attributes_dct: dict, test_protected_groups: dict, postprocessor=None,
-                 postprocessing_sensitive_attribute : str = None, computation_mode: str = None,
-                 notebook_logs_stdout: bool = False, verbose: int = 0):
+                 postprocessing_sensitive_attribute : str = None, random_state: int = None, computation_mode: str = None,
+                 with_predict_proba: bool = True, notebook_logs_stdout: bool = False, verbose: int = 0):
+
+        with_predict_proba = False if postprocessor is not None else with_predict_proba
         if model_setting == ModelSetting.BATCH:
             if postprocessor is not None:
                 print('Enabled a postprocessing mode')
                 overall_variance_analyzer = BatchOverallVarianceAnalyzerPostProcessing(postprocessor=postprocessor,
                                                                                        sensitive_attribute=postprocessing_sensitive_attribute,
                                                                                        base_model=base_model,
                                                                                        base_model_name=base_model_name,
@@ -63,40 +71,41 @@
                                                                                        X_train=dataset.X_train_val,
                                                                                        y_train=dataset.y_train_val,
                                                                                        X_test=dataset.X_test,
                                                                                        y_test=dataset.y_test,
                                                                                        dataset_name=dataset_name,
                                                                                        target_column=dataset.target,
                                                                                        n_estimators=n_estimators,
-                                                                                       with_predict_proba=False,
+                                                                                       random_state=random_state,
+                                                                                       with_predict_proba=with_predict_proba,
                                                                                        notebook_logs_stdout=notebook_logs_stdout,
                                                                                        verbose=verbose)
             else:
                 overall_variance_analyzer = BatchOverallVarianceAnalyzer(base_model=base_model,
                                                                          base_model_name=base_model_name,
                                                                          bootstrap_fraction=bootstrap_fraction,
                                                                          X_train=dataset.X_train_val,
                                                                          y_train=dataset.y_train_val,
                                                                          X_test=dataset.X_test,
                                                                          y_test=dataset.y_test,
                                                                          dataset_name=dataset_name,
                                                                          target_column=dataset.target,
                                                                          n_estimators=n_estimators,
+                                                                         random_state=random_state,
+                                                                         with_predict_proba=with_predict_proba,
                                                                          notebook_logs_stdout=notebook_logs_stdout,
                                                                          verbose=verbose)
         else:
             raise ValueError('model_setting is incorrect or not supported')
 
         self.dataset_name = overall_variance_analyzer.dataset_name
         self.n_estimators = overall_variance_analyzer.n_estimators
         self.base_model_name = overall_variance_analyzer.base_model_name
 
         self.__overall_variance_analyzer = overall_variance_analyzer
-
-        with_predict_proba = False if postprocessor is not None else True
         self.__subgroup_variance_calculator = SubgroupVarianceCalculator(X_test=dataset.X_test,
                                                                          y_test=dataset.y_test,
                                                                          sensitive_attributes_dct=sensitive_attributes_dct,
                                                                          test_protected_groups=test_protected_groups,
                                                                          computation_mode=computation_mode,
                                                                          with_predict_proba=with_predict_proba)
         self.overall_variance_metrics_dct = dict()
```

### Comparing `virny-0.4.0/virny/analyzers/subgroup_variance_calculator.py` & `virny-0.5.0/virny/analyzers/subgroup_variance_calculator.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/configs/constants.py` & `virny-0.5.0/virny/configs/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 TNR = 'TNR'
 PPV = 'PPV'
 FNR = 'FNR'
 FPR = 'FPR'
 F1 = 'F1'
 ACCURACY = 'Accuracy'
 SELECTION_RATE = 'Selection-Rate'
-POSITIVE_RATE = 'Positive-Rate'
 
 # Stability metrics
 STD = 'Std'
 IQR = 'IQR'
 JITTER = 'Jitter'
 LABEL_STABILITY = 'Label_Stability'
```

### Comparing `virny-0.4.0/virny/custom_classes/__init__.py` & `virny-0.5.0/virny/custom_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/custom_classes/base_inprocessing_wrapper.py` & `virny-0.5.0/virny/custom_classes/base_inprocessing_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,29 +9,43 @@
     @abc.abstractmethod
     def fit(self, X, y):
         """Fits an inprocessor based on X and y pandas dataframes. Returns self."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def predict_proba(self, X):
-        """Predicts using the fitted inprocessor based on X features pandas dataframe. Returns probabilities
-        for **ZERO** class. These probabilities will be used by Virny in the downstream metric computation."""
+        """
+        Predicts using the fitted inprocessor based on X features pandas dataframe. Returns probabilities
+        for **ZERO** class. These probabilities will be used by Virny in the downstream metric computation.
+
+        If the inprocessor does not support prediction probabilities, the implementation of this method can be skipped,
+         and with_predict_proba = False should be set in the metric computation interface.
+
+        Indexes from the returned array of predictions should start from zero.
+        """
         raise NotImplementedError
 
     @abc.abstractmethod
     def predict(self, X):
-        """Predicts using the fitted inprocessor based on X features pandas dataframe. Returns labels for each
-        sample."""
+        """
+        Predicts using the fitted inprocessor based on X features pandas dataframe. Returns labels for each
+        sample. Indexes from the returned array of predictions should start from zero.
+        """
         raise NotImplementedError
 
     @abc.abstractmethod
     def __copy__(self):
         raise NotImplementedError
 
     @abc.abstractmethod
     def __deepcopy__(self, memo):
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_params(self):
         """Returns parameters of the wrapper. Alignment with sklearn API."""
         raise NotImplementedError
+
+    @abc.abstractmethod
+    def set_params(self, random_state: int):
+        """Set a random state of the inprocessor."""
+        raise NotImplementedError
```

### Comparing `virny-0.4.0/virny/custom_classes/custom_logger.py` & `virny-0.5.0/virny/custom_classes/custom_logger.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/custom_classes/metrics_composer.py` & `virny-0.5.0/virny/custom_classes/metrics_composer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,24 +30,24 @@
         self.disparity_metric_functions = {
             # Error disparity metrics
             TPR: [(EQUALIZED_ODDS_TPR, self._difference_operation)],
             TNR: [(EQUALIZED_ODDS_TNR, self._difference_operation)],
             FPR: [(EQUALIZED_ODDS_FPR, self._difference_operation)],
             FNR: [(EQUALIZED_ODDS_FNR, self._difference_operation)],
             ACCURACY: [(ACCURACY_DIFFERENCE, self._difference_operation)],
-            POSITIVE_RATE: [(DISPARATE_IMPACT, self._ratio_operation)],
-            SELECTION_RATE: [(STATISTICAL_PARITY_DIFFERENCE, self._difference_operation)],
+            SELECTION_RATE: [(STATISTICAL_PARITY_DIFFERENCE, self._difference_operation),
+                             (DISPARATE_IMPACT, self._ratio_operation)],
             # Stability disparity metrics
             LABEL_STABILITY: [(LABEL_STABILITY_RATIO, self._ratio_operation),
                               (LABEL_STABILITY_DIFFERENCE, self._difference_operation)],
             JITTER: [(JITTER_DIFFERENCE, self._difference_operation)],
             IQR: [(IQR_DIFFERENCE, self._difference_operation)],
+            # Uncertainty disparity metrics
             STD: [(STD_DIFFERENCE, self._difference_operation),
                   (STD_RATIO, self._ratio_operation)],
-            # Uncertainty disparity metrics
             OVERALL_UNCERTAINTY: [(OVERALL_UNCERTAINTY_DIFFERENCE, self._difference_operation),
                                   (OVERALL_UNCERTAINTY_RATIO, self._ratio_operation)],
             ALEATORIC_UNCERTAINTY: [(ALEATORIC_UNCERTAINTY_DIFFERENCE, self._difference_operation),
                                     (ALEATORIC_UNCERTAINTY_RATIO, self._ratio_operation)],
             EPISTEMIC_UNCERTAINTY: [(EPISTEMIC_UNCERTAINTY_DIFFERENCE, self._difference_operation),
                                     (EPISTEMIC_UNCERTAINTY_RATIO, self._ratio_operation)],
         }
```

### Comparing `virny-0.4.0/virny/custom_classes/metrics_interactive_visualizer.py` & `virny-0.5.0/virny/custom_classes/metrics_interactive_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.group_names = list(self.sensitive_attributes_dct.keys())
 
         # Technical attributes
         self.demo = None
         self.max_groups = 8
 
         # Metric names
-        self.all_accuracy_metrics = [STATISTICAL_BIAS, TPR, TNR, PPV, FNR, FPR, F1, ACCURACY, POSITIVE_RATE]
+        self.all_accuracy_metrics = [STATISTICAL_BIAS, TPR, TNR, PPV, FNR, FPR, F1, ACCURACY]
         self.all_stability_metrics = [STD, IQR, JITTER, LABEL_STABILITY]
         self.all_uncertainty_metrics = [ALEATORIC_UNCERTAINTY, OVERALL_UNCERTAINTY, EPISTEMIC_UNCERTAINTY]
         self.all_error_disparity_metrics = [EQUALIZED_ODDS_TPR, EQUALIZED_ODDS_TNR, EQUALIZED_ODDS_FPR, EQUALIZED_ODDS_FNR, DISPARATE_IMPACT, STATISTICAL_PARITY_DIFFERENCE, ACCURACY_DIFFERENCE]
         self.all_stability_disparity_metrics = [LABEL_STABILITY_RATIO, LABEL_STABILITY_DIFFERENCE, IQR_DIFFERENCE, STD_DIFFERENCE, STD_RATIO, JITTER_DIFFERENCE]
         self.all_uncertainty_disparity_metrics = [OVERALL_UNCERTAINTY_DIFFERENCE, OVERALL_UNCERTAINTY_RATIO, ALEATORIC_UNCERTAINTY_DIFFERENCE, ALEATORIC_UNCERTAINTY_RATIO,
                                                   EPISTEMIC_UNCERTAINTY_DIFFERENCE, EPISTEMIC_UNCERTAINTY_RATIO]
 
@@ -363,15 +363,15 @@
                 with gr.Column():
                     gr.Markdown(
                         """
                         ### Overall Metric Constraints
                         """)
                     with gr.Row():
                         accuracy_metric_vw4 = gr.Dropdown(
-                            sorted([metric for metric in self.all_accuracy_metrics if metric not in (POSITIVE_RATE, SELECTION_RATE)]),
+                            sorted([metric for metric in self.all_accuracy_metrics if metric != SELECTION_RATE]),
                             value=ACCURACY, multiselect=False, label="Correctness Metric",
                             scale=2
                         )
                         accuracy_min_val_vw4 = gr.Text(value="0.0", label="Min value", scale=1)
                         accuracy_max_val_vw4 = gr.Text(value="1.0", label="Max value", scale=1)
                     with gr.Row():
                         subgroup_stability_metric_vw4 = gr.Dropdown(
@@ -387,15 +387,15 @@
                             value=ALEATORIC_UNCERTAINTY, multiselect=False, label="Uncertainty Metric",
                             scale=2
                         )
                         subgroup_uncertainty_min_val_vw4 = gr.Text(value="0.0", label="Min value", scale=1)
                         subgroup_uncertainty_max_val_vw4 = gr.Text(value="1.0", label="Max value", scale=1)
                     with gr.Row():
                         positive_rate_metric_vw4 = gr.Dropdown(
-                            [POSITIVE_RATE, SELECTION_RATE],
+                            [SELECTION_RATE],
                             value=SELECTION_RATE, multiselect=False, label="Representation Metric",
                             scale=2
                         )
                         positive_rate_min_val_vw4 = gr.Text(value="0.0", label="Min value", scale=1)
                         positive_rate_max_val_vw4 = gr.Text(value="1.0", label="Max value", scale=1)
 
                     btn_view4 = gr.Button("Submit")
```

### Comparing `virny-0.4.0/virny/custom_classes/metrics_visualizer.py` & `virny-0.5.0/virny/custom_classes/metrics_visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         sns.set_theme(style="whitegrid")
 
         self.dataset_name = dataset_name
         self.model_names = model_names
         self.sensitive_attributes_dct = sensitive_attributes_dct
 
         # Metric names
-        self.all_accuracy_metrics = [STATISTICAL_BIAS, TPR, TNR, PPV, FNR, FPR, F1, ACCURACY, POSITIVE_RATE]
+        self.all_accuracy_metrics = [STATISTICAL_BIAS, TPR, TNR, PPV, FNR, FPR, F1, ACCURACY]
         self.all_stability_metrics = [STD, IQR, JITTER, LABEL_STABILITY]
         self.all_uncertainty_metrics = [ALEATORIC_UNCERTAINTY, OVERALL_UNCERTAINTY, EPISTEMIC_UNCERTAINTY]
         self.all_error_disparity_metrics = [EQUALIZED_ODDS_TPR, EQUALIZED_ODDS_TNR, EQUALIZED_ODDS_FPR, EQUALIZED_ODDS_FNR, DISPARATE_IMPACT, STATISTICAL_PARITY_DIFFERENCE, ACCURACY_DIFFERENCE]
         self.all_stability_disparity_metrics = [LABEL_STABILITY_RATIO, LABEL_STABILITY_DIFFERENCE, IQR_DIFFERENCE, STD_DIFFERENCE, STD_RATIO, JITTER_DIFFERENCE]
         self.all_uncertainty_disparity_metrics = [OVERALL_UNCERTAINTY_DIFFERENCE, OVERALL_UNCERTAINTY_RATIO, ALEATORIC_UNCERTAINTY_DIFFERENCE, ALEATORIC_UNCERTAINTY_RATIO,
                                                   EPISTEMIC_UNCERTAINTY_DIFFERENCE, EPISTEMIC_UNCERTAINTY_RATIO]
```

### Comparing `virny-0.4.0/virny/datasets/COMPAS.csv` & `virny-0.5.0/virny/datasets/data/COMPAS.csv`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/datasets/__init__.py` & `virny-0.5.0/virny/datasets/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """
 This module contains sample datasets and data loaders.
 The purpose is to provide sample datasets for functionality testing and show examples of data loaders (aka dataset classes).
 """
-from .data_loaders import CompasWithoutSensitiveAttrsDataset, DiabetesDataset, CompasDataset, \
-    ACSIncomeDataset, ACSEmploymentDataset, ACSMobilityDataset, ACSTravelTimeDataset, ACSPublicCoverageDataset, \
-    RicciDataset, LawSchoolDataset, CreditCardDefaultDataset, StudentPerformancePortugueseDataset
+from .finance import GermanCreditDataset, BankMarketingDataset
+from .compas import CompasWithoutSensitiveAttrsDataset, CompasDataset
+from .healthcare import CardiovascularDiseaseDataset, DiabetesDataset2019, RicciDataset
+from .education import LawSchoolDataset, StudentPerformancePortugueseDataset
+from .folktables import (ACSIncomeDataset, ACSEmploymentDataset, ACSMobilityDataset, ACSTravelTimeDataset,
+                         ACSPublicCoverageDataset)
 
 
 __all__ = [
+    "GermanCreditDataset",
+    "BankMarketingDataset",
     "CompasWithoutSensitiveAttrsDataset",
     "CompasDataset",
-    "CreditCardDefaultDataset",
-    "DiabetesDataset",
+    "CardiovascularDiseaseDataset",
+    "DiabetesDataset2019",
     "RicciDataset",
-    "StudentPerformancePortugueseDataset",
     "LawSchoolDataset",
+    "StudentPerformancePortugueseDataset",
     "ACSIncomeDataset",
     "ACSEmploymentDataset",
     "ACSMobilityDataset",
     "ACSTravelTimeDataset",
     "ACSPublicCoverageDataset",
 ]
```

### Comparing `virny-0.4.0/virny/datasets/base.py` & `virny-0.5.0/virny/datasets/base.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/datasets/law_school_clean.csv` & `virny-0.5.0/virny/datasets/data/law_school_clean.csv`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/datasets/ricci_race.csv` & `virny-0.5.0/virny/datasets/data/ricci_race.csv`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/datasets/student_por_new.csv` & `virny-0.5.0/virny/datasets/data/student_por_new.csv`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/metrics/__init__.py` & `virny-0.5.0/virny/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/metrics/accuracy_metrics.py` & `virny-0.5.0/virny/metrics/accuracy_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,10 +78,9 @@
     metrics[TNR] = TN/(TN+FP)
     metrics[PPV] = TP/(TP+FP)
     metrics[FNR] = FN/(FN+TP)
     metrics[FPR] = FP/(FP+TN)
     metrics[ACCURACY] = (TP+TN)/(TP+TN+FP+FN)
     metrics[F1] = (2*TP)/(2*TP+FP+FN)
     metrics[SELECTION_RATE] = (TP+FP)/(TP+FP+TN+FN)
-    metrics[POSITIVE_RATE] = (TP+FP)/(TP+FN)
 
     return metrics
```

### Comparing `virny-0.4.0/virny/metrics/stability_metrics.py` & `virny-0.5.0/virny/metrics/stability_metrics.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/metrics/uncertainty_metrics.py` & `virny-0.5.0/virny/metrics/uncertainty_metrics.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/preprocessing/basic_preprocessing.py` & `virny-0.5.0/virny/preprocessing/basic_preprocessing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import pandas as pd
 from sklearn.compose import ColumnTransformer
 from sklearn.preprocessing import StandardScaler
 from sklearn.model_selection import train_test_split
 
-from virny.datasets.data_loaders import BaseDataLoader
+from virny.configs.constants import INTERSECTION_SIGN
+from virny.datasets.base import BaseDataLoader
 from virny.custom_classes.base_dataset import BaseFlowDataset
 
 
-def preprocess_dataset(data_loader: BaseDataLoader, column_transformer: ColumnTransformer,
+def preprocess_dataset(data_loader: BaseDataLoader, column_transformer: ColumnTransformer, sensitive_attributes_dct: dict,
                        test_set_fraction: float, dataset_split_seed: int) -> BaseFlowDataset:
     """
     Preprocess an input dataset using sklearn ColumnTransformer. Split the dataset on train and test using test_set_fraction.
      Create an instance of BaseFlowDataset.
 
     Parameters
     ----------
     data_loader
         Instance of BaseDataLoader that contains a target, numerical, and categorical columns.
     column_transformer
         Instance of sklearn ColumnTransformer to preprocess categorical and numerical columns.
+    sensitive_attributes_dct
+        Dictionary of sensitive attribute names and their disadvantaged values.
     test_set_fraction
         Fraction from 0 to 1. Used to split the input dataset on the train and test sets.
     dataset_split_seed
         Seed for dataset splitting.
 
     Return
     ----------
@@ -35,16 +38,17 @@
     # Split and preprocess the dataset
     X_train_val, X_test, y_train_val, y_test = train_test_split(data_loader.X_data, data_loader.y_data,
                                                                 test_size=test_set_fraction,
                                                                 random_state=dataset_split_seed)
     column_transformer = column_transformer.set_output(transform="pandas")  # Set transformer output to a pandas df
     X_train_features = column_transformer.fit_transform(X_train_val)
     X_test_features = column_transformer.transform(X_test)
+    sensitive_attrs = [attr for attr in sensitive_attributes_dct.keys() if INTERSECTION_SIGN not in attr]
 
-    return BaseFlowDataset(init_features_df=data_loader.full_df.drop(data_loader.target, axis=1, errors='ignore'),
+    return BaseFlowDataset(init_sensitive_attrs_df=data_loader.full_df[sensitive_attrs],
                            X_train_val=X_train_features,
                            X_test=X_test_features,
                            y_train_val=y_train_val,
                            y_test=y_test,
                            target=data_loader.target,
                            numerical_columns=data_loader.numerical_columns,
                            categorical_columns=data_loader.categorical_columns)
```

### Comparing `virny-0.4.0/virny/user_interfaces/__init__.py` & `virny-0.5.0/virny/user_interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/user_interfaces/multiple_models_api.py` & `virny-0.5.0/virny/user_interfaces/multiple_models_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from virny.analyzers.subgroup_variance_analyzer import SubgroupVarianceAnalyzer
 from virny.analyzers.subgroup_error_analyzer import SubgroupErrorAnalyzer
 from virny.utils.protected_groups_partitioning import create_test_protected_groups
 from virny.utils.common_helpers import save_metrics_to_file
 
 
 def compute_metrics_with_config(dataset: BaseFlowDataset, config, models_config: dict,
-                                save_results_dir_path: str, postprocessor=None,
+                                save_results_dir_path: str, postprocessor=None, with_predict_proba: bool = True,
                                 notebook_logs_stdout: bool = False, verbose: int = 0) -> dict:
     """
     Compute stability and accuracy metrics for each model in models_config. Arguments are defined as an input config object.
     Save results in `save_results_dir_path` folder.
 
     Return a dictionary where keys are model names, and values are metrics for sensitive attributes defined in config.
 
@@ -29,14 +29,18 @@
         Object that contains bootstrap_fraction, dataset_name, n_estimators, sensitive_attributes_dct attributes
     models_config
         Dictionary where keys are model names, and values are initialized models
     save_results_dir_path
         Location where to save result files with metrics
     postprocessor
         [Optional] Postprocessor object to apply to model predictions before metrics computation
+    with_predict_proba
+        [Optional] True, if models in models_config have a predict_proba method and can return probabilities for predictions,
+         False, otherwise. Note that if it is set to False, only metrics based on labels (not labels and probabilities) will be computed.
+         Ignored when a postprocessor is not None, and set to False in this case.
     notebook_logs_stdout
         [Optional] True, if this interface was execute in a Jupyter notebook,
          False, otherwise.
     verbose
         [Optional] Level of logs printing. The greater level provides more logs.
             As for now, 0, 1, 2 levels are supported. Currently, verbose works only with notebook_logs_stdout = False.
 
@@ -44,31 +48,28 @@
     # Currently, verbose works only with notebook_logs_stdout = False
     if notebook_logs_stdout:
         verbose = 0
 
     start_datetime = datetime.now(timezone.utc)
     os.makedirs(save_results_dir_path, exist_ok=True)
 
-    # Check if a type of postprocessing_sensitive_attribute is not NoneType.
-    # In other words, check if postprocessing_sensitive_attribute is defined in a config yaml.
-    postprocessing_sensitive_attribute = config.postprocessing_sensitive_attribute \
-        if type(config.postprocessing_sensitive_attribute) != type(None) else None
-
     model_metrics_dct = dict()
     models_metrics_dct = run_metrics_computation(dataset=dataset,
                                                  bootstrap_fraction=config.bootstrap_fraction,
                                                  dataset_name=config.dataset_name,
                                                  models_config=models_config,
                                                  n_estimators=config.n_estimators,
                                                  sensitive_attributes_dct=config.sensitive_attributes_dct,
+                                                 random_state=config.random_state,
                                                  model_setting=config.model_setting,
                                                  computation_mode=config.computation_mode,
                                                  postprocessor=postprocessor,
-                                                 postprocessing_sensitive_attribute=postprocessing_sensitive_attribute,
+                                                 postprocessing_sensitive_attribute=config.postprocessing_sensitive_attribute,
                                                  save_results=False,
+                                                 with_predict_proba=with_predict_proba,
                                                  notebook_logs_stdout=notebook_logs_stdout,
                                                  verbose=verbose)
 
     # Concatenate with previous results and save them in an overwrite mode each time for backups
     for model_name in models_metrics_dct.keys():
         model_metrics_df = models_metrics_dct[model_name]
         model_metrics_dct[model_name] = model_metrics_df
@@ -77,18 +78,20 @@
         model_metrics_dct[model_name].to_csv(f'{save_results_dir_path}/{result_filename}', index=False, mode='w')
 
     return model_metrics_dct
 
 
 def run_metrics_computation(dataset: BaseFlowDataset, bootstrap_fraction: float, dataset_name: str,
                             models_config: dict, n_estimators: int, sensitive_attributes_dct: dict,
-                            model_setting: str = ModelSetting.BATCH.value, computation_mode: str = None,
-                            postprocessor=None, postprocessing_sensitive_attribute: str = None,
+                            random_state: int = None, model_setting: str = ModelSetting.BATCH.value,
+                            computation_mode: str = None, postprocessor=None,
+                            postprocessing_sensitive_attribute: str = None,
                             save_results: bool = True, save_results_dir_path: str = None,
-                            notebook_logs_stdout: bool = False, verbose: int = 0) -> dict:
+                            with_predict_proba: bool = True, notebook_logs_stdout: bool = False,
+                            verbose: int = 0) -> dict:
     """
     Compute stability and accuracy metrics for each model in models_config.
     Save results in `save_results_dir_path` folder.
 
     Return a dictionary where keys are model names, and values are metrics for sensitive attributes defined in config.
 
     Parameters
@@ -102,26 +105,32 @@
     models_config
         Dictionary where keys are model names, and values are initialized models
     n_estimators
         Number of estimators for bootstrap to compute subgroup stability metrics
     sensitive_attributes_dct
         A dictionary where keys are sensitive attribute names (including attributes intersections),
          and values are privilege values for these attributes
+    random_state
+        [Optional] Controls the randomness of the bootstrap approach for model arbitrariness evaluation
     model_setting
         [Optional] Currently, only batch models are supported. Default: 'batch'.
     computation_mode
         [Optional] A non-default mode for metrics computation. Should be included in the ComputationMode enum.
     postprocessor
         [Optional] Postprocessor object to apply to model predictions before metrics computation
     postprocessing_sensitive_attribute
         [Optional] Sensitive attribute name to apply postprocessor only to this attribute predictions
     save_results
         [Optional] If to save result metrics in a file
     save_results_dir_path
         [Optional] Location where to save result files with metrics
+    with_predict_proba
+        [Optional] True, if models in models_config have a predict_proba method and can return probabilities for predictions,
+         False, otherwise. Note that if it is set to False, only metrics based on labels (not labels and probabilities) will be computed.
+         Ignored when a postprocessor is not None, and set to False in this case.
     notebook_logs_stdout
         [Optional] True, if this interface was execute in a Jupyter notebook,
          False, otherwise.
     verbose
         [Optional] Level of logs printing. The greater level provides more logs.
             As for now, 0, 1, 2 levels are supported.
 
@@ -140,46 +149,54 @@
                                       colour="red",
                                       file=sys.stdout):
         if verbose >= 1:
             print('\n\n', flush=True)
             print('#' * 30, f' [Model {model_idx + 1} / {num_models}] Analyze {model_name} ', '#' * 30)
         try:
             base_model = models_config[model_name]
+            computation_start_date_time = datetime.now()
             model_metrics_df = compute_one_model_metrics(base_model=base_model,
                                                          n_estimators=n_estimators,
                                                          dataset=dataset,
                                                          bootstrap_fraction=bootstrap_fraction,
                                                          sensitive_attributes_dct=sensitive_attributes_dct,
+                                                         random_state=random_state,
                                                          model_setting=model_setting,
                                                          computation_mode=computation_mode,
                                                          dataset_name=dataset_name,
                                                          base_model_name=model_name,
                                                          postprocessor=postprocessor,
                                                          postprocessing_sensitive_attribute=postprocessing_sensitive_attribute,
                                                          save_results=save_results,
                                                          save_results_dir_path=save_results_dir_path,
+                                                         with_predict_proba=with_predict_proba,
                                                          notebook_logs_stdout=notebook_logs_stdout,
                                                          verbose=verbose)
+            computation_end_date_time = datetime.now()
+            computation_runtime = (computation_end_date_time - computation_start_date_time).total_seconds() / 60.0
+            model_metrics_df['Runtime_in_Mins'] = computation_runtime
+
             models_metrics_dct[model_name] = model_metrics_df
 
         except Exception as err:
             print('#' * 20, f'ERROR with {model_name}', '#' * 20)
             traceback.print_exc()
 
         if verbose >= 1:
             print('\n\n\n')
 
     return models_metrics_dct
 
 
 def compute_one_model_metrics(base_model, n_estimators: int, dataset: BaseFlowDataset, bootstrap_fraction: float,
                               sensitive_attributes_dct: dict, dataset_name: str, base_model_name: str,
-                              postprocessor=None, postprocessing_sensitive_attribute: str = None,
-                              model_setting: str = ModelSetting.BATCH.value, computation_mode: str = None, save_results: bool = True,
-                              save_results_dir_path: str = None, notebook_logs_stdout: bool = False, verbose: int = 0):
+                              random_state: int = None, model_setting: str = ModelSetting.BATCH.value,
+                              computation_mode: str = None, postprocessor=None, postprocessing_sensitive_attribute: str = None,
+                              save_results: bool = True, save_results_dir_path: str = None, with_predict_proba: bool = True,
+                              notebook_logs_stdout: bool = False, verbose: int = 0):
     """
     Compute subgroup metrics for the base model.
     Save results in `save_results_dir_path` folder.
 
     Return a dataframe of model metrics.
 
     Parameters
@@ -195,37 +212,43 @@
     sensitive_attributes_dct
         A dictionary where keys are sensitive attribute names (including attributes intersections),
          and values are privilege values for these attributes
     dataset_name
         Dataset name to name a result file with metrics
     base_model_name
         Model name to name a result file with metrics
+    random_state
+        [Optional] Controls the randomness of the bootstrap approach for model arbitrariness evaluation
+    model_setting
+        [Optional] Currently, only batch models are supported. Default: 'batch'.
+    computation_mode
+        [Optional] A non-default mode for metrics computation. Should be included in the ComputationMode enum.
     postprocessor
         [Optional] Postprocessor object to apply to model predictions before metrics computation
     postprocessing_sensitive_attribute
         [Optional] Sensitive attribute name to apply postprocessor only to this attribute predictions
     save_results
         [Optional] If to save result metrics in a file
-    model_setting
-        [Optional] Currently, only batch models are supported. Default: 'batch'.
-    computation_mode
-        [Optional] A non-default mode for metrics computation. Should be included in the ComputationMode enum.
     save_results_dir_path
         [Optional] Location where to save result files with metrics
+    with_predict_proba
+        [Optional] True, if models in models_config have a predict_proba method and can return probabilities for predictions,
+         False, otherwise. Note that if it is set to False, only metrics based on labels (not labels and probabilities) will be computed.
+         Ignored when a postprocessor is not None, and set to False in this case.
     notebook_logs_stdout
         [Optional] True, if this interface was execute in a Jupyter notebook,
          False, otherwise.
     verbose
         [Optional] Level of logs printing. The greater level provides more logs.
             As for now, 0, 1, 2 levels are supported.
 
     """
     model_setting = ModelSetting.BATCH if model_setting is None else ModelSetting[model_setting.upper()]
 
-    test_protected_groups = create_test_protected_groups(dataset.X_test, dataset.init_features_df, sensitive_attributes_dct)
+    test_protected_groups = create_test_protected_groups(dataset.X_test, dataset.init_sensitive_attrs_df, sensitive_attributes_dct)
     if verbose >= 2:
         print('\nProtected groups splits:')
         for g in test_protected_groups.keys():
             print(g, test_protected_groups[g].shape)
 
     # Compute stability metrics for subgroups
     subgroup_variance_analyzer = SubgroupVarianceAnalyzer(model_setting=model_setting,
@@ -233,17 +256,19 @@
                                                           base_model=base_model,
                                                           base_model_name=base_model_name,
                                                           bootstrap_fraction=bootstrap_fraction,
                                                           dataset=dataset,
                                                           dataset_name=dataset_name,
                                                           sensitive_attributes_dct=sensitive_attributes_dct,
                                                           test_protected_groups=test_protected_groups,
+                                                          random_state=random_state,
                                                           computation_mode=computation_mode,
                                                           postprocessor=postprocessor,
                                                           postprocessing_sensitive_attribute=postprocessing_sensitive_attribute,
+                                                          with_predict_proba=with_predict_proba,
                                                           notebook_logs_stdout=notebook_logs_stdout,
                                                           verbose=verbose)
     y_preds, variance_metrics_df = subgroup_variance_analyzer.compute_metrics(save_results=False,
                                                                               result_filename=None,
                                                                               save_dir_path=None)
 
     # Compute error metrics for subgroups
@@ -260,14 +285,15 @@
     error_metrics_df = pd.DataFrame(dtc_res)
 
     metrics_df = pd.concat([variance_metrics_df, error_metrics_df])
     metrics_df = metrics_df.reset_index()
     metrics_df = metrics_df.rename(columns={"index": "Metric"})
     metrics_df['Model_Name'] = base_model_name
     metrics_df['Model_Params'] = str(base_model.get_params())
+    metrics_df['Virny_Random_State'] = random_state
 
     if save_results:
         # Save metrics
         result_filename = f'Metrics_{dataset_name}_{base_model_name}'
         save_metrics_to_file(metrics_df, result_filename, save_results_dir_path)
 
     return metrics_df
```

### Comparing `virny-0.4.0/virny/user_interfaces/multiple_models_with_db_writer_api.py` & `virny-0.5.0/virny/user_interfaces/multiple_models_with_db_writer_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from datetime import datetime, timezone
 
 from virny.custom_classes.base_dataset import BaseFlowDataset
 from virny.user_interfaces.multiple_models_api import run_metrics_computation
 
 
 def compute_metrics_with_db_writer(dataset: BaseFlowDataset, config, models_config: dict,
-                                   custom_tbl_fields_dct: dict, db_writer_func,
-                                   postprocessor=None, notebook_logs_stdout: bool = False, verbose: int = 0) -> dict:
+                                   custom_tbl_fields_dct: dict, db_writer_func, postprocessor=None,
+                                   with_predict_proba: bool = True, notebook_logs_stdout: bool = False,
+                                   verbose: int = 0) -> dict:
     """
     Compute stability and accuracy metrics for each model in models_config. Arguments are defined as an input config object.
     Save results to a database after each run appending fields and value from custom_tbl_fields_dct and using db_writer_func.
 
     Return a dictionary where keys are model names, and values are metrics for sensitive attributes defined in config.
 
     Parameters
@@ -24,44 +25,45 @@
         Dictionary where keys are model names, and values are initialized models
     custom_tbl_fields_dct
         Dictionary where keys are column names and values to add to inserted metrics during saving results to a database
     db_writer_func
         Python function object has one argument (run_models_metrics_df) and save this metrics df to a target database
     postprocessor
         [Optional] Postprocessor object to apply to model predictions before metrics computation
+    with_predict_proba
+        [Optional] True, if models in models_config have a predict_proba method and can return probabilities for predictions,
+         False, otherwise. Note that if it is set to False, only metrics based on labels (not labels and probabilities) will be computed.
+         Ignored when a postprocessor is not None, and set to False in this case.
     notebook_logs_stdout
         [Optional] True, if this interface was execute in a Jupyter notebook,
          False, otherwise.
     verbose
         [Optional] Level of logs printing. The greater level provides more logs.
             As for now, 0, 1, 2 levels are supported. Currently, verbose works only with notebook_logs_stdout = False.
 
     """
     # Currently, verbose works only with notebook_logs_stdout = False
     if notebook_logs_stdout:
         verbose = 0
 
-    # Check if a type of postprocessing_sensitive_attribute is not NoneType.
-    # In other words, check if postprocessing_sensitive_attribute is defined in a config yaml.
-    postprocessing_sensitive_attribute = config.postprocessing_sensitive_attribute \
-        if type(config.postprocessing_sensitive_attribute) != type(None) else None
-
     multiple_models_metrics_dct = dict()
     run_models_metrics_df = pd.DataFrame()
     models_metrics_dct = run_metrics_computation(dataset=dataset,
                                                  bootstrap_fraction=config.bootstrap_fraction,
                                                  dataset_name=config.dataset_name,
                                                  models_config=models_config,
                                                  n_estimators=config.n_estimators,
                                                  sensitive_attributes_dct=config.sensitive_attributes_dct,
+                                                 random_state=config.random_state,
                                                  model_setting=config.model_setting,
                                                  computation_mode=config.computation_mode,
                                                  postprocessor=postprocessor,
-                                                 postprocessing_sensitive_attribute=postprocessing_sensitive_attribute,
+                                                 postprocessing_sensitive_attribute=config.postprocessing_sensitive_attribute,
                                                  save_results=False,
+                                                 with_predict_proba=with_predict_proba,
                                                  notebook_logs_stdout=notebook_logs_stdout,
                                                  verbose=verbose)
 
     # Concatenate current run metrics with previous results and
     # create melted_model_metrics_df to save it in a database
     for model_name in models_metrics_dct.keys():
         model_metrics_df = models_metrics_dct[model_name]
```

### Comparing `virny-0.4.0/virny/user_interfaces/multiple_models_with_multiple_test_sets_api.py` & `virny-0.5.0/virny/user_interfaces/multiple_models_with_multiple_test_sets_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from virny.custom_classes.base_dataset import BaseFlowDataset
 from virny.analyzers.subgroup_variance_analyzer import SubgroupVarianceAnalyzer
 from virny.analyzers.subgroup_error_analyzer import SubgroupErrorAnalyzer
 
 
 def compute_metrics_with_multiple_test_sets(dataset: BaseFlowDataset, extra_test_sets_lst,
                                             config, models_config: dict, custom_tbl_fields_dct: dict,
-                                            db_writer_func, notebook_logs_stdout: bool = False, verbose: int = 0):
+                                            db_writer_func, with_predict_proba: bool = True,
+                                            notebook_logs_stdout: bool = False, verbose: int = 0):
     """
     Compute stability and accuracy metrics for each model in models_config based on dataset.X_test and each extra test set
      in extra_test_sets_lst. Arguments are defined as an input config object. Save results to a database after each run
       appending fields and value from custom_tbl_fields_dct and using db_writer_func.
       Index of each test set is also added as a separate column in out final records in the database
       (0 index -- for dataset.X_test, 1 and greater -- for each extra test set in extra_test_sets_lst, keeping the original sequence).
 
@@ -31,14 +32,18 @@
         Object that contains bootstrap_fraction, dataset_name, n_estimators, sensitive_attributes_dct attributes
     models_config
         Dictionary where keys are model names, and values are initialized models
     custom_tbl_fields_dct
         Dictionary where keys are column names and values to add to inserted metrics during saving results to a database
     db_writer_func
         Python function object has one argument (run_models_metrics_df) and save this metrics df to a target database
+    with_predict_proba
+        [Optional] True, if models in models_config have a predict_proba method and can return probabilities for predictions,
+         False, otherwise. Note that if it is set to False, only metrics based on labels (not labels and probabilities) will be computed.
+         Ignored when a postprocessor is not None, and set to False in this case.
     notebook_logs_stdout
         [Optional] True, if this interface was execute in a Jupyter notebook,
          False, otherwise.
     verbose
         [Optional] Level of logs printing. The greater level provides more logs.
             As for now, 0, 1, 2 levels are supported. Currently, verbose works only with notebook_logs_stdout = False.
 
@@ -50,16 +55,18 @@
     models_metrics_dct = run_metrics_computation_with_multiple_test_sets(dataset=dataset,
                                                                          bootstrap_fraction=config.bootstrap_fraction,
                                                                          dataset_name=config.dataset_name,
                                                                          extra_test_sets_lst=extra_test_sets_lst,
                                                                          models_config=models_config,
                                                                          n_estimators=config.n_estimators,
                                                                          sensitive_attributes_dct=config.sensitive_attributes_dct,
+                                                                         random_state=config.random_state,
                                                                          model_setting=config.model_setting,
                                                                          computation_mode=config.computation_mode,
+                                                                         with_predict_proba=with_predict_proba,
                                                                          notebook_logs_stdout=notebook_logs_stdout,
                                                                          verbose=verbose)
     # Concatenate current run metrics with previous results and
     # create melted_model_metrics_df to save it in a database
     run_models_metrics_df = pd.DataFrame()
     for model_name in models_metrics_dct.keys():
         model_metrics_dfs_lst = models_metrics_dct[model_name]
@@ -86,17 +93,18 @@
 
     if verbose >= 1:
         print('Metrics computation interface was successfully executed!')
 
 
 def run_metrics_computation_with_multiple_test_sets(dataset: BaseFlowDataset, bootstrap_fraction: float, dataset_name: str,
                                                     extra_test_sets_lst: list, models_config: dict, n_estimators: int,
-                                                    sensitive_attributes_dct: dict, model_setting: str = ModelSetting.BATCH.value,
-                                                    computation_mode: str = None, notebook_logs_stdout: bool = False,
-                                                    verbose: int = 0) -> dict:
+                                                    sensitive_attributes_dct: dict, random_state: int = None,
+                                                    model_setting: str = ModelSetting.BATCH.value,
+                                                    computation_mode: str = None, with_predict_proba: bool = True,
+                                                    notebook_logs_stdout: bool = False, verbose: int = 0) -> dict:
     """
     Compute stability and accuracy metrics for each model in models_config based on dataset.X_test and each extra test set
      in extra_test_sets_lst. Save results in `save_results_dir_path` folder.
 
     Return a dictionary where keys are model names, and values are metrics for sensitive attributes defined in config.
 
     Parameters
@@ -112,18 +120,24 @@
     models_config
         Dictionary where keys are model names, and values are initialized models
     n_estimators
         Number of estimators for bootstrap to compute subgroup stability metrics
     sensitive_attributes_dct
         A dictionary where keys are sensitive attribute names (including attributes intersections),
          and values are privilege values for these attributes
+    random_state
+        [Optional] Controls the randomness of the bootstrap approach for model arbitrariness evaluation
     model_setting
         Currently, only batch models are supported. Default: 'batch'.
     computation_mode
         [Optional] A non-default mode for metrics computation. Should be included in the ComputationMode enum.
+    with_predict_proba
+        [Optional] True, if models in models_config have a predict_proba method and can return probabilities for predictions,
+         False, otherwise. Note that if it is set to False, only metrics based on labels (not labels and probabilities) will be computed.
+         Ignored when a postprocessor is not None, and set to False in this case.
     notebook_logs_stdout
         [Optional] True, if this interface was execute in a Jupyter notebook,
          False, otherwise.
     verbose
         [Optional] Level of logs printing. The greater level provides more logs.
             As for now, 0, 1, 2 levels are supported.
 
@@ -141,44 +155,52 @@
                                       desc="Analyze multiple models",
                                       colour="red",
                                       file=sys.stdout):
         if verbose >= 1:
             print('#' * 30, f' [Model {model_idx + 1} / {num_models}] Analyze {model_name} ', '#' * 30)
         try:
             base_model = models_config[model_name]
+            computation_start_date_time = datetime.now()
             model_metrics_dfs_lst = compute_one_model_metrics_with_multiple_test_sets(base_model=base_model,
                                                                                       n_estimators=n_estimators,
                                                                                       dataset=dataset,
                                                                                       extra_test_sets_lst=extra_test_sets_lst,
                                                                                       bootstrap_fraction=bootstrap_fraction,
                                                                                       sensitive_attributes_dct=sensitive_attributes_dct,
+                                                                                      random_state=random_state,
                                                                                       model_setting=model_setting,
                                                                                       computation_mode=computation_mode,
                                                                                       dataset_name=dataset_name,
                                                                                       base_model_name=model_name,
+                                                                                      with_predict_proba=with_predict_proba,
                                                                                       notebook_logs_stdout=notebook_logs_stdout,
                                                                                       verbose=verbose)
+            computation_end_date_time = datetime.now()
+            computation_runtime = (computation_end_date_time - computation_start_date_time).total_seconds() / 60.0
+            for model_metrics_df in model_metrics_dfs_lst:
+                model_metrics_df['Runtime_in_Mins'] = computation_runtime
+
             models_metrics_dct[model_name] = model_metrics_dfs_lst
         except Exception as err:
             print('#' * 20, f'ERROR with {model_name}', '#' * 20)
             traceback.print_exc()
 
         if verbose >= 1:
             print('\n\n\n')
 
     return models_metrics_dct
 
 
 def compute_one_model_metrics_with_multiple_test_sets(base_model, n_estimators: int,
                                                       dataset: BaseFlowDataset, extra_test_sets_lst: list,
                                                       bootstrap_fraction: float, sensitive_attributes_dct: dict,
-                                                      dataset_name: str, base_model_name: str,
+                                                      dataset_name: str, base_model_name: str, random_state: int = None,
                                                       model_setting: str = ModelSetting.BATCH.value,
-                                                      computation_mode: str = None, notebook_logs_stdout: bool = False,
-                                                      verbose: int = 0):
+                                                      computation_mode: str = None, with_predict_proba: bool = True,
+                                                      notebook_logs_stdout: bool = False, verbose: int = 0):
     """
     Compute subgroup metrics for the base model based on dataset.X_test and each extra test set in extra_test_sets_lst.
     Save results in `save_results_dir_path` folder.
 
     Return a dataframe of model metrics.
 
     Parameters
@@ -186,29 +208,35 @@
     base_model
         Base model for metrics computation
     n_estimators
         Number of estimators for bootstrap to compute subgroup stability metrics
     dataset
         BaseFlowDataset object that contains all needed attributes like target, features, numerical_columns etc.
     extra_test_sets_lst
-        List of extra test sets like [(X_test1, y_test1, init_features_df1), (X_test2, y_test2, init_features_df2), ...]
+        List of extra test sets like [(X_test1, y_test1, init_sensitive_attrs_df1), (X_test2, y_test2, init_sensitive_attrs_df2), ...]
          to compute metrics.
     bootstrap_fraction
         Fraction of a train set in range [0.0 - 1.0] to fit models in bootstrap
     sensitive_attributes_dct
         A dictionary where keys are sensitive attribute names (including attributes intersections),
          and values are privilege values for these attributes
     dataset_name
         Dataset name to name a result file with metrics
     base_model_name
         Model name to name a result file with metrics
+    random_state
+        [Optional] Controls the randomness of the bootstrap approach for model arbitrariness evaluation
     model_setting
-        Currently, only batch models are supported. Default: 'batch'.
+        [Optional] Currently, only batch models are supported. Default: 'batch'.
     computation_mode
         [Optional] A non-default mode for metrics computation. Should be included in the ComputationMode enum.
+    with_predict_proba
+        [Optional] True, if models in models_config have a predict_proba method and can return probabilities for predictions,
+         False, otherwise. Note that if it is set to False, only metrics based on labels (not labels and probabilities) will be computed.
+         Ignored when a postprocessor is not None, and set to False in this case.
     notebook_logs_stdout
         [Optional] True, if this interface was execute in a Jupyter notebook,
          False, otherwise.
     verbose
         [Optional] Level of logs printing. The greater level provides more logs.
             As for now, 0, 1, 2 levels are supported.
 
@@ -219,22 +247,24 @@
                                                           base_model=base_model,
                                                           base_model_name=base_model_name,
                                                           bootstrap_fraction=bootstrap_fraction,
                                                           dataset=dataset,  # will be replaced in the below for-cycle
                                                           dataset_name=dataset_name,
                                                           sensitive_attributes_dct=sensitive_attributes_dct,
                                                           test_protected_groups=dict(),  # stub for this attribute
+                                                          random_state=random_state,
                                                           computation_mode=computation_mode,
+                                                          with_predict_proba=with_predict_proba,
                                                           notebook_logs_stdout=notebook_logs_stdout,
                                                           verbose=verbose)
 
-    test_sets_lst = [(dataset.X_test, dataset.y_test, dataset.init_features_df)] + extra_test_sets_lst
+    test_sets_lst = [(dataset.X_test, dataset.y_test, dataset.init_sensitive_attrs_df)] + extra_test_sets_lst
     all_test_sets_metrics_lst = []
-    for set_idx, (new_X_test, new_y_test, cur_init_features_df) in enumerate(test_sets_lst):
-        new_test_protected_groups = create_test_protected_groups(new_X_test, cur_init_features_df, sensitive_attributes_dct)
+    for set_idx, (new_X_test, new_y_test, cur_init_sensitive_attrs_df) in enumerate(test_sets_lst):
+        new_test_protected_groups = create_test_protected_groups(new_X_test, cur_init_sensitive_attrs_df, sensitive_attributes_dct)
         if verbose >= 2:
             print(f'\nProtected groups splits for test set index #{set_idx}:')
             for g in new_test_protected_groups.keys():
                 print(g, new_test_protected_groups[g].shape)
 
         # Replace test sets and protected groups for each new test set
         subgroup_variance_analyzer.set_test_sets(new_X_test, new_y_test)
@@ -260,11 +290,12 @@
         error_metrics_df = pd.DataFrame(dtc_res)
 
         metrics_df = pd.concat([variance_metrics_df, error_metrics_df])
         metrics_df = metrics_df.reset_index()
         metrics_df = metrics_df.rename(columns={"index": "Metric"})
         metrics_df['Model_Name'] = base_model_name
         metrics_df['Model_Params'] = str(base_model.get_params())
+        metrics_df['Virny_Random_State'] = random_state
 
         all_test_sets_metrics_lst.append(metrics_df)
 
     return all_test_sets_metrics_lst
```

### Comparing `virny-0.4.0/virny/utils/common_helpers.py` & `virny-0.5.0/virny/utils/common_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 
     Parameters
     ----------
     config_obj
         Object with parameters defined in a yaml file
 
     """
-    # ================== Required parameters ==================
+    # ============================================================================================================
+    # Required parameters
+    # ============================================================================================================
     if not isinstance(config_obj.dataset_name, str):
         raise ValueError('dataset_name must be string')
 
     if not isinstance(config_obj.bootstrap_fraction, float) \
             or config_obj.bootstrap_fraction < 0.0 \
             or config_obj.bootstrap_fraction > 1.0:
         raise ValueError('bootstrap_fraction must be float in [0.0, 1.0] range')
@@ -50,27 +52,37 @@
                                  f"Intersectional signs must be between all attributes in this intersectional attribute.")
 
             for attr in attrs:
                 if attr not in config_obj.sensitive_attributes_dct.keys():
                     raise ValueError('Intersectional attributes in sensitive_attributes_dct must contain '
                                      'single sensitive attributes that also exist in sensitive_attributes_dct')
 
-    # ================== Optional parameters ==================
+    # ============================================================================================================
+    # Optional parameters
+    # ============================================================================================================
     if config_obj.model_setting is not None \
             and not isinstance(config_obj.model_setting, str) \
             and config_obj.model_setting not in ModelSetting:
         raise ValueError('model_setting must be a string that is included in the ModelSetting enum. '
                          'Refer to this function documentation for more details!')
 
     if config_obj.computation_mode is not None \
             and not isinstance(config_obj.computation_mode, str) \
             and config_obj.computation_mode not in ComputationMode:
         raise ValueError('computation_mode must be a string that is included in the ComputationMode enum. '
                          'Refer to this function documentation for more details!')
 
+    # ============================================================================================================
+    # Default parameters
+    # ============================================================================================================
+    if 'postprocessing_sensitive_attribute' not in config_obj:
+        config_obj.postprocessing_sensitive_attribute = None
+    if 'random_state' not in config_obj:
+        config_obj.random_state = None
+
     return True
 
 
 def isfloat_regex(string):
     # We have defined a pattern for float value
     pattern = r'^[-+]?[0-9]*\.?[0-9]+([eE][-+]?[0-9]+)?$'
     # Find the match and convert to boolean
@@ -80,23 +92,14 @@
 def str_to_float(str_var: str, var_name: str):
     if isfloat_regex(str_var):
         return float(str_var)
     else:
         raise ValueError(f"{var_name} must be a float number with a '.' separator.")
 
 
-def reset_model_seed(model, new_seed, verbose):
-    if 'random_state' in model.get_params():
-        model.set_params(random_state=new_seed)
-        if verbose >= 1:
-            print('Model seed: ', model.get_params().get('random_state', None))
-
-    return model
-
-
 def save_metrics_to_file(metrics_df, result_filename, save_dir_path):
     os.makedirs(save_dir_path, exist_ok=True)
 
     now = datetime.now(timezone.utc)
     date_time_str = now.strftime("%Y%m%d__%H%M%S")
     filename = f"{result_filename}_{date_time_str}.csv"
     metrics_df.to_csv(f'{save_dir_path}/{filename}', index=False)
```

### Comparing `virny-0.4.0/virny/utils/custom_initializers.py` & `virny-0.5.0/virny/utils/custom_initializers.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/utils/data_viz_utils.py` & `virny-0.5.0/virny/utils/data_viz_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import seaborn as sns
 
 from matplotlib import pyplot as plt
 from altair.utils.schemapi import Undefined
 
 from virny.configs.constants import *
 from virny.utils.common_helpers import check_substring_in_list
+from virny.utils.protected_groups_partitioning import create_test_protected_groups
 
 
 def rank_with_tolerance(pd_series: pd.Series, tolerance: float = 0.001):
     """
     Rank a pandas series with defined tolerance.
     Ref: https://stackoverflow.com/questions/72956450/pandas-ranking-with-tolerance
 
@@ -97,28 +98,61 @@
     return sorted_matrix_by_rank
 
 
 def create_subgroup_sorted_matrix_by_rank(model_metrics_matrix, tolerance) -> np.array:
     models_distances_matrix = model_metrics_matrix.copy(deep=True).T
     metric_names = models_distances_matrix.columns
     for metric_name in metric_names:
-        if check_substring_in_list(metric_name, ['TPR', 'TNR', 'PPV', 'Accuracy', 'F1', 'Label_Stability', 'Positive-Rate']):
+        if check_substring_in_list(metric_name, ['TPR', 'TNR', 'PPV', 'Accuracy', 'F1', 'Label_Stability']):
             # Cast a metric to a case when the closer value to one is the better
             models_distances_matrix[metric_name] = 1 - models_distances_matrix[metric_name]
         models_distances_matrix[metric_name] = models_distances_matrix[metric_name].abs()
 
     models_distances_matrix = models_distances_matrix.T
     models_distances_df = pd.DataFrame(models_distances_matrix)
     sorted_matrix_by_rank = models_distances_df.apply(
         lambda row : rank_with_tolerance(row, tolerance), axis = 1
     )
 
     return sorted_matrix_by_rank
 
 
+def create_dataset_stats_bar_chart(X_data, y_data, sensitive_attrs_dct):
+    # Partition on protected groups
+    protected_groups = create_test_protected_groups(X_data, X_data, sensitive_attrs_dct)
+
+    # Create a df with group proportions and group base rates
+    subgroup_proportions_dct = compute_proportions(protected_groups, X_data)
+    subgroup_base_rates_dct = compute_base_rates(protected_groups, y_data)
+    subgroup_relative_base_rates_dct = dict()
+    for subgroup in subgroup_proportions_dct.keys():
+        pct = subgroup_base_rates_dct[subgroup]['percentage'] * subgroup_proportions_dct[subgroup]['percentage']
+        subgroup_relative_base_rates_dct[subgroup] = {'percentage': pct, 'num_rows': subgroup_base_rates_dct[subgroup]['num_rows']}
+
+    stats_df = pd.DataFrame(columns=['Subgroup', 'Percentage', 'Num_Rows', 'Statistics_Type'])
+    for subgroup in subgroup_proportions_dct.keys():
+        stats_df.loc[len(stats_df.index)] = [subgroup, subgroup_proportions_dct[subgroup]['percentage'],
+                                             subgroup_proportions_dct[subgroup]['num_rows'], 'Proportion']
+        stats_df.loc[len(stats_df.index)] = [subgroup, subgroup_relative_base_rates_dct[subgroup]['percentage'],
+                                             subgroup_relative_base_rates_dct[subgroup]['num_rows'], 'Base_Rate']
+
+    # Create a row facet bar chart
+    facet_sort_by_lst = ['overall'] + [grp for grp in stats_df.Subgroup.unique() if grp.lower() != 'overall']
+    col_facet_bar_chart = create_col_facet_bar_chart(stats_df,
+                                                     x_col='Statistics_Type',
+                                                     y_col='Num_Rows',
+                                                     facet_column_name='Subgroup',
+                                                     text_labels_column='Percentage',
+                                                     x_sort_by_lst=['Proportion', 'Base_Rate'],
+                                                     facet_sort_by_lst=facet_sort_by_lst,
+                                                     color_legend_title='Statistics Type',
+                                                     facet_title='')
+    return col_facet_bar_chart
+
+
 def create_col_facet_bar_chart(df, x_col, y_col, facet_column_name, text_labels_column, x_sort_by_lst=Undefined,
                                facet_sort_by_lst=Undefined, color_legend_title=Undefined, facet_title=Undefined):
     num_facets = len(df[facet_column_name].unique())
     max_y_axis_limit = df[y_col].max()
     base_font_size = 16
 
     # Set dynamic variables that adapt to the number of defined groups
@@ -389,15 +423,14 @@
         TPR: 'C1',
         TNR: 'C1',
         FNR: 'C1',
         FPR: 'C1',
         PPV: 'C1',
         ACCURACY: 'C1',
         F1: 'C1',
-        POSITIVE_RATE: 'C1',
         # C2
         EQUALIZED_ODDS_TPR: 'C2',
         EQUALIZED_ODDS_FPR: 'C2',
         EQUALIZED_ODDS_FNR: 'C2',
         DISPARATE_IMPACT: 'C2',
         STATISTICAL_PARITY_DIFFERENCE: 'C2',
         # C3
```

### Comparing `virny-0.4.0/virny/utils/model_tuning_utils.py` & `virny-0.5.0/virny/utils/model_tuning_utils.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/utils/postprocessing_intervention_utils.py` & `virny-0.5.0/virny/utils/postprocessing_intervention_utils.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny/utils/protected_groups_partitioning.py` & `virny-0.5.0/virny/utils/protected_groups_partitioning.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,42 +48,42 @@
 def check_sensitive_attrs_in_columns(df_columns, sensitive_attributes_dct):
     for sensitive_attr in sensitive_attributes_dct.keys():
         if INTERSECTION_SIGN not in sensitive_attr and sensitive_attr not in df_columns:
             return False
     return True
 
 
-def create_test_protected_groups(X_test: pd.DataFrame, init_features_df: pd.DataFrame, sensitive_attributes_dct: dict):
+def create_test_protected_groups(X_test: pd.DataFrame, init_sensitive_attrs_df: pd.DataFrame, sensitive_attributes_dct: dict):
     """
     Create protected groups based on a test feature set. Use a disadvantaged group as a reference group.
 
     Return a dictionary where keys are subgroup names, and values are X_test row indexes correspondent to this subgroup.
 
     Parameters
     ----------
     X_test
         Test feature set
-    init_features_df
-        Initial full dataset without preprocessing
+    init_sensitive_attrs_df
+        Initial full dataset of sensitive attributes without preprocessing
     sensitive_attributes_dct
         A dictionary where keys are sensitive attribute names (including attributes intersections),
          and values are disadvantaged values for these attributes
 
     """
     plain_sensitive_attributes = [attr for attr in sensitive_attributes_dct.keys() if INTERSECTION_SIGN not in attr]
 
     # Check spelling of sensitive attributes
     attrs_with_errors = []
     for attr in plain_sensitive_attributes:
-        if attr not in init_features_df.columns:
+        if attr not in init_sensitive_attrs_df.columns:
             attrs_with_errors.append(attr)
     if len(attrs_with_errors) > 0:
         raise ValueError(f"At least one of sensitive attributes is not in dataset columns. Check spelling of {attrs_with_errors} attributes.")
 
-    X_test_with_sensitive_attrs = init_features_df[plain_sensitive_attributes].loc[X_test.index]
+    X_test_with_sensitive_attrs = init_sensitive_attrs_df[plain_sensitive_attributes].loc[X_test.index]
     groups = dict()
     for attr in sensitive_attributes_dct.keys():
         attr = attr.strip()
         if INTERSECTION_SIGN in attr:
             single_attrs = attr.split(INTERSECTION_SIGN)
             single_attrs = [single_attr.strip() for single_attr in single_attrs]
             priv_grp_name = INTERSECTION_SIGN.join(single_attrs) + '_priv'
```

### Comparing `virny-0.4.0/virny/utils/stability_utils.py` & `virny-0.5.0/virny/utils/stability_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,15 +79,19 @@
         y_preds = np.array([int(x<0.5) for x in results.mean().values])
     else:
         y_preds = np.array([int(x>0.5) for x in results.mean().values])
 
     return y_preds, metrics_dct
 
 
-def generate_bootstrap(features, labels, boostrap_size, with_replacement=True):
-    bootstrap_index = np.random.choice(features.shape[0], size=boostrap_size, replace=with_replacement)
+def generate_bootstrap(features, labels, boostrap_size, with_replacement=True, random_state=None):
+    # Create a local random state
+    rng = np.random.RandomState(random_state)
+
+    # Generate bootstrapped indexes
+    bootstrap_index = rng.choice(features.shape[0], size=boostrap_size, replace=with_replacement)
     bootstrap_features = pd.DataFrame(features).iloc[bootstrap_index]
     bootstrap_labels = pd.DataFrame(labels).iloc[bootstrap_index]
     if len(bootstrap_features) == boostrap_size:
         return bootstrap_features, bootstrap_labels
     else:
         raise ValueError('Bootstrap samples are not of the size requested')
```

### Comparing `virny-0.4.0/virny/utils/validation.py` & `virny-0.5.0/virny/utils/validation.py`

 * *Files identical despite different names*

### Comparing `virny-0.4.0/virny.egg-info/SOURCES.txt` & `virny-0.5.0/virny.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 tests/analyzers/test_subgroup_error_analyzer.py
 tests/custom_classes/__init__.py
 tests/custom_classes/test_metrics_composer.py
 tests/metrics/__init__.py
 tests/preprocessing/__init__.py
 tests/preprocessing/test_basic_preprocessing.py
 tests/user_interfaces/__init__.py
+tests/user_interfaces/conftest.py
 tests/user_interfaces/test_compute_model_metrics.py
+tests/user_interfaces/test_multiple_models_api.py
 tests/utils/__init__.py
 tests/utils/test_common_helpers.py
 tests/utils/test_data_viz_utils.py
 tests/utils/test_protected_groups_partitioning.py
 tests/utils/test_stability_utils.py
 virny/__init__.py
 virny/__version__.py
@@ -37,23 +39,29 @@
 virny/custom_classes/__init__.py
 virny/custom_classes/base_dataset.py
 virny/custom_classes/base_inprocessing_wrapper.py
 virny/custom_classes/custom_logger.py
 virny/custom_classes/metrics_composer.py
 virny/custom_classes/metrics_interactive_visualizer.py
 virny/custom_classes/metrics_visualizer.py
-virny/datasets/COMPAS.csv
 virny/datasets/__init__.py
 virny/datasets/base.py
-virny/datasets/credit_card_default_clean.csv
-virny/datasets/data_loaders.py
-virny/datasets/givemesomecredit.csv
-virny/datasets/law_school_clean.csv
-virny/datasets/ricci_race.csv
-virny/datasets/student_por_new.csv
+virny/datasets/compas.py
+virny/datasets/education.py
+virny/datasets/finance.py
+virny/datasets/folktables.py
+virny/datasets/healthcare.py
+virny/datasets/data/COMPAS.csv
+virny/datasets/data/bank-full.csv
+virny/datasets/data/cardio.csv
+virny/datasets/data/diabetes_dataset__2019.csv
+virny/datasets/data/german_data_credit.csv
+virny/datasets/data/law_school_clean.csv
+virny/datasets/data/ricci_race.csv
+virny/datasets/data/student_por_new.csv
 virny/metrics/__init__.py
 virny/metrics/accuracy_metrics.py
 virny/metrics/stability_metrics.py
 virny/metrics/uncertainty_metrics.py
 virny/preprocessing/__init__.py
 virny/preprocessing/basic_preprocessing.py
 virny/user_interfaces/__init__.py
```

### Comparing `virny-0.4.0/virny.egg-info/requires.txt` & `virny-0.5.0/virny.egg-info/requires.txt`

 * *Files identical despite different names*

