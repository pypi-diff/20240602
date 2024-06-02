# Comparing `tmp/scores-0.8.2.tar.gz` & `tmp/scores-0.8.3.tar.gz`

## Comparing `scores-0.8.2.tar` & `scores-0.8.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.8.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.8.2/environment.yml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.8.2/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.2/py.typed
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.8.2/readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.2/setup.cfg
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.8.2/.binder/postBuild
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.8.2/.binder/requirements.txt
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.2/.github/pull_request_template.md
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 scores-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 scores-0.8.2/.github/ISSUE_TEMPLATE/new_score.md
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.8.2/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.8.2/.github/workflows/run-pre-commit.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/__init__.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/functions.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/sample_data.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/typing.py
--rw-r--r--   0        0        0    12725 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/utils.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/categorical/__init__.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/categorical/binary_impl.py
--rw-r--r--   0        0        0    21558 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/categorical/contingency_impl.py
--rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/categorical/multicategorical_impl.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/continuous/__init__.py
--rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/continuous/flip_flop_impl.py
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/continuous/murphy_impl.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/continuous/quantile_loss_impl.py
--rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/continuous/standard_impl.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/emerging/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/pandas/__init__.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/pandas/continuous.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/pandas/typing.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/probability/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/probability/brier_impl.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/probability/checks.py
--rw-r--r--   0        0        0    37967 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/probability/crps_impl.py
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/probability/roc_impl.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/__init__.py
--rw-r--r--   0        0        0    12438 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/discretise.py
--rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/isoreg_impl.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/matching.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/cdf/__init__.py
--rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/processing/cdf/cdf_functions.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/stats/__init__.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/stats/statistical_tests/__init__.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/stats/statistical_tests/acovf.py
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.8.2/src/scores/stats/statistical_tests/diebold_mariano_impl.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.2/.gitignore
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.8.2/LICENSE
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 scores-0.8.2/README.md
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 scores-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 scores-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 scores-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 scores-0.8.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 scores-0.8.3/environment.yml
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 scores-0.8.3/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.3/py.typed
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 scores-0.8.3/readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.8.3/setup.cfg
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 scores-0.8.3/.binder/postBuild
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 scores-0.8.3/.binder/requirements.txt
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.3/.github/pull_request_template.md
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 scores-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 scores-0.8.3/.github/ISSUE_TEMPLATE/new_score.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 scores-0.8.3/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 scores-0.8.3/.github/workflows/run-pre-commit.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/__init__.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/functions.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/sample_data.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/typing.py
+-rw-r--r--   0        0        0    12725 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/utils.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/categorical/__init__.py
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/categorical/binary_impl.py
+-rw-r--r--   0        0        0    21558 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/categorical/contingency_impl.py
+-rw-r--r--   0        0        0    11009 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/categorical/multicategorical_impl.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/continuous/__init__.py
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/continuous/flip_flop_impl.py
+-rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/continuous/murphy_impl.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/continuous/quantile_loss_impl.py
+-rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/continuous/standard_impl.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/emerging/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/pandas/__init__.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/pandas/continuous.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/pandas/typing.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/probability/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/probability/brier_impl.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/probability/checks.py
+-rw-r--r--   0        0        0    37967 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/probability/crps_impl.py
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/probability/roc_impl.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/__init__.py
+-rw-r--r--   0        0        0    12438 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/discretise.py
+-rw-r--r--   0        0        0    29482 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/isoreg_impl.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/matching.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/cdf/__init__.py
+-rw-r--r--   0        0        0    16430 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/processing/cdf/cdf_functions.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/stats/__init__.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/stats/statistical_tests/__init__.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/stats/statistical_tests/acovf.py
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 scores-0.8.3/src/scores/stats/statistical_tests/diebold_mariano_impl.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scores-0.8.3/.gitignore
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.8.3/LICENSE
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 scores-0.8.3/README.md
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 scores-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 scores-0.8.3/PKG-INFO
```

### Comparing `scores-0.8.2/.pre-commit-config.yaml` & `scores-0.8.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/CODE_OF_CONDUCT.md` & `scores-0.8.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/readthedocs.yaml` & `scores-0.8.3/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/.binder/requirements.txt` & `scores-0.8.3/.binder/requirements.txt`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/.github/pull_request_template.md` & `scores-0.8.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md` & `scores-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/.github/ISSUE_TEMPLATE/new_score.md` & `scores-0.8.3/.github/ISSUE_TEMPLATE/new_score.md`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/.github/workflows/python-app.yml` & `scores-0.8.3/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/.github/workflows/run-pre-commit.yml` & `scores-0.8.3/.github/workflows/run-pre-commit.yml`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/__init__.py` & `scores-0.8.3/src/scores/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import scores.functions
 import scores.pandas
 import scores.probability
 import scores.processing
 import scores.sample_data
 import scores.stats.statistical_tests  # noqa: F401
 
-__version__ = "0.8.2"
+__version__ = "0.8.3"
 
 __all__ = [
     "scores.categorical",
     "scores.contingency",
     "scores.continuous",
     "scores.functions",
     "scores.pandas",
```

### Comparing `scores-0.8.2/src/scores/functions.py` & `scores-0.8.3/src/scores/functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/sample_data.py` & `scores-0.8.3/src/scores/sample_data.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/typing.py` & `scores-0.8.3/src/scores/typing.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/utils.py` & `scores-0.8.3/src/scores/utils.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/categorical/__init__.py` & `scores-0.8.3/src/scores/categorical/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/categorical/binary_impl.py` & `scores-0.8.3/src/scores/categorical/binary_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/categorical/contingency_impl.py` & `scores-0.8.3/src/scores/categorical/contingency_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
         How well did the forecast separate the "yes" events from the "no" events?
         Range: -1 to 1, 0 indicates no skill. Perfect score: 1.
 
         https://www.cawcr.gov.au/projects/verification/#HK
         """
         cd = self.counts
         component_a = cd["tp_count"] / (cd["tp_count"] + cd["fn_count"])
-        component_b = cd["fn_count"] / (cd["fn_count"] + cd["tn_count"])
+        component_b = cd["fp_count"] / (cd["fp_count"] + cd["tn_count"])
         skill_score = component_a - component_b
         return skill_score
 
     def true_skill_statistic(self):
         """
         Identical to Peirce's skill score and to Hanssen and Kuipers discriminant
         How well did the forecast separate the "yes" events from the "no" events?
```

### Comparing `scores-0.8.2/src/scores/categorical/multicategorical_impl.py` & `scores-0.8.3/src/scores/categorical/multicategorical_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/continuous/__init__.py` & `scores-0.8.3/src/scores/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/continuous/flip_flop_impl.py` & `scores-0.8.3/src/scores/continuous/flip_flop_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/continuous/murphy_impl.py` & `scores-0.8.3/src/scores/continuous/murphy_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/continuous/quantile_loss_impl.py` & `scores-0.8.3/src/scores/continuous/quantile_loss_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/continuous/standard_impl.py` & `scores-0.8.3/src/scores/continuous/standard_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/pandas/continuous.py` & `scores-0.8.3/src/scores/pandas/continuous.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/probability/__init__.py` & `scores-0.8.3/src/scores/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/probability/brier_impl.py` & `scores-0.8.3/src/scores/probability/brier_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/probability/checks.py` & `scores-0.8.3/src/scores/probability/checks.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/probability/crps_impl.py` & `scores-0.8.3/src/scores/probability/crps_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/probability/roc_impl.py` & `scores-0.8.3/src/scores/probability/roc_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/processing/__init__.py` & `scores-0.8.3/src/scores/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/processing/discretise.py` & `scores-0.8.3/src/scores/processing/discretise.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/processing/isoreg_impl.py` & `scores-0.8.3/src/scores/processing/isoreg_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/processing/matching.py` & `scores-0.8.3/src/scores/processing/matching.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/processing/cdf/cdf_functions.py` & `scores-0.8.3/src/scores/processing/cdf/cdf_functions.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/stats/statistical_tests/acovf.py` & `scores-0.8.3/src/scores/stats/statistical_tests/acovf.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/src/scores/stats/statistical_tests/diebold_mariano_impl.py` & `scores-0.8.3/src/scores/stats/statistical_tests/diebold_mariano_impl.py`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/.gitignore` & `scores-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/LICENSE` & `scores-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/README.md` & `scores-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/pyproject.toml` & `scores-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scores-0.8.2/PKG-INFO` & `scores-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scores
-Version: 0.8.2
+Version: 0.8.3
 Summary: Scores is a package containing mathematical functions for the verification, evaluation and optimisation of forecasts, predictions or models.
 Project-URL: Repository, https://github.com/nci/scores
 Project-URL: Documentation, https://scores.readthedocs.io/en/latest/
 Author-email: Tennessee Leeuwenburg <tennessee.leeuwenburg@bom.gov.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

