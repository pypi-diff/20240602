# Comparing `tmp/pylemur-0.2.1.tar.gz` & `tmp/pylemur-0.2.2.tar.gz`

## Comparing `pylemur-0.2.1.tar` & `pylemur-0.2.2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pylemur-0.2.1/.codecov.yaml
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pylemur-0.2.1/.cruft.json
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pylemur-0.2.1/.editorconfig
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pylemur-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pylemur-0.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 pylemur-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/workflows/build.yaml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 pylemur-0.2.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/Makefile
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/changelog.md
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/conf.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/index.md
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/_static/.gitkeep
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/_static/css/custom.css
--rw-r--r--   0        0        0    69769 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/_static/images/equation_schematic.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0     9771 2020-02-02 00:00:00.000000 pylemur-0.2.1/docs/notebooks/Tutorial.myst
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/check_implementation.qmd
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/devel_experiments.qmd
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/kang_analysis_in_R.qmd
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/lemur_model_experiments.qmd
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/scanpy_experiments.qmd
--rw-r--r--   0        0        0   307919 2020-02-02 00:00:00.000000 pylemur-0.2.1/notebooks/test.ipynb
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/pl/__init__.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/pl/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/pp/__init__.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/pp/basic.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/__init__.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/_design_matrix_utils.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/_grassmann.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/_grassmann_lm.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/_lin_alg_wrappers.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/alignment.py
--rw-r--r--   0        0        0    19198 2020-02-02 00:00:00.000000 pylemur-0.2.1/src/pylemur/tl/lemur.py
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pylemur-0.2.1/tests/test_grasmann_lm.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pylemur-0.2.1/tests/test_grassmann.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 pylemur-0.2.1/tests/test_lin_alg_utils.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pylemur-0.2.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pylemur-0.2.1/LICENSE
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 pylemur-0.2.1/README.md
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 pylemur-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 pylemur-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pylemur-0.2.2/.codecov.yaml
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 pylemur-0.2.2/.cruft.json
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pylemur-0.2.2/.editorconfig
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pylemur-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pylemur-0.2.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 pylemur-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 pylemur-0.2.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pylemur-0.2.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pylemur-0.2.2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pylemur-0.2.2/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pylemur-0.2.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pylemur-0.2.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/Makefile
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/changelog.md
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/conf.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/index.md
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    69769 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/_static/images/equation_schematic.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0     9767 2020-02-02 00:00:00.000000 pylemur-0.2.2/docs/notebooks/Tutorial.myst
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 pylemur-0.2.2/notebooks/check_implementation.qmd
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pylemur-0.2.2/notebooks/devel_experiments.qmd
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pylemur-0.2.2/notebooks/kang_analysis_in_R.qmd
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pylemur-0.2.2/notebooks/lemur_model_experiments.qmd
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 pylemur-0.2.2/notebooks/scanpy_experiments.qmd
+-rw-r--r--   0        0        0   308138 2020-02-02 00:00:00.000000 pylemur-0.2.2/notebooks/test.ipynb
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/pl/__init__.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/pl/basic.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/pp/__init__.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/pp/basic.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/tl/__init__.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/tl/_design_matrix_utils.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/tl/_grassmann.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/tl/_grassmann_lm.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/tl/_lin_alg_wrappers.py
+-rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/tl/alignment.py
+-rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 pylemur-0.2.2/src/pylemur/tl/lemur.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 pylemur-0.2.2/tests/test_grasmann_lm.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pylemur-0.2.2/tests/test_grassmann.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 pylemur-0.2.2/tests/test_lemur.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 pylemur-0.2.2/tests/test_lin_alg_utils.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pylemur-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pylemur-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 pylemur-0.2.2/README.md
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 pylemur-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 pylemur-0.2.2/PKG-INFO
```

### Comparing `pylemur-0.2.1/.cruft.json` & `pylemur-0.2.2/.cruft.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'checkout'": "'v0.4.0'", "'commit'": "'87a407a65408d75a949c0b54b19fd287475a56f8'"}*

```diff
@@ -1,10 +1,10 @@
 {
-    "checkout": null,
-    "commit": "c6e5e5008a7b2915709b7def3cdcddcf6159c301",
+    "checkout": "v0.4.0",
+    "commit": "87a407a65408d75a949c0b54b19fd287475a56f8",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 ".github/workflows/build.yaml",
                 ".github/workflows/test.yaml",
                 "docs/_templates/autosummary/**.rst"
             ],
```

### Comparing `pylemur-0.2.1/.pre-commit-config.yaml` & `pylemur-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/CHANGELOG.md` & `pylemur-0.2.2/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -6,30 +6,36 @@
 and this project adheres to [Semantic Versioning][].
 
 [keep a changelog]: https://keepachangelog.com/en/1.0.0/
 [semantic versioning]: https://semver.org/spec/v2.0.0.html
 
 ## [Unreleased]
 
+## [0.2.2]
+
+-   Sync with cookiecutter-template update (version 0.4)
+-   Bump required Python version to `3.10`
+-   Allow data frames as design matrices
+-   Allow matrices as input to LEMUR()
+
 ## [0.2.1]
 
-- Change example gene to one with clearer differential expression pattern
-- Remove error output in `align_harmony
+-   Change example gene to one with clearer differential expression pattern
+-   Remove error output in `align_harmony
 
 ## [0.2.0]
 
 Major rewrite of the API. Instead of adding coefficients as custom fields
 to the input `AnnData` object, the API now follows an object-oriented style
-similar to scikit-learn or `SCVI`. This change was motivated by the feedback 
+similar to scikit-learn or `SCVI`. This change was motivated by the feedback
 during the submission to the `scverse` ecosystem.
-([Thanks]((https://github.com/scverse/ecosystem-packages/pull/156#issuecomment-2014676654)) Gregor).
+([Thanks](<(https://github.com/scverse/ecosystem-packages/pull/156#issuecomment-2014676654)>) Gregor).
 
 ### Changed
 
-- Instead of calling `fit = pylemur.tl.lemur(adata, ...)`, you now create a LEMUR model 
-(`model = pylemur.tl.LEMUR(adata, ...)`) and subsequently call `model.fit()`, `model.align_with_harmony()`, 
-and `model.predict()`.
-
+-   Instead of calling `fit = pylemur.tl.lemur(adata, ...)`, you now create a LEMUR model
+    (`model = pylemur.tl.LEMUR(adata, ...)`) and subsequently call `model.fit()`, `model.align_with_harmony()`,
+    and `model.predict()`.
 
 ## [0.1.0] - 2024-03-21
 
 -   Initial beta release of `pyLemur`
```

### Comparing `pylemur-0.2.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `pylemur-0.2.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/.github/workflows/build.yaml` & `pylemur-0.2.2/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/.github/workflows/release.yaml` & `pylemur-0.2.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/.github/workflows/test.yaml` & `pylemur-0.2.2/.github/workflows/test.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
         shell: bash -e {0} # -e to fail on error
 
     strategy:
       fail-fast: false
       matrix:
         include:
           - os: ubuntu-latest
-            python: "3.9"
+            python: "3.10"
           - os: ubuntu-latest
-            python: "3.11"
+            python: "3.12"
           - os: ubuntu-latest
-            python: "3.11"
+            python: "3.12"
             pip-flags: "--pre"
             name: PRE-RELEASE DEPENDENCIES
 
     name: ${{ matrix.name }} Python ${{ matrix.python }}
 
     env:
       OS: ${{ matrix.os }}
```

### Comparing `pylemur-0.2.1/docs/Makefile` & `pylemur-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/docs/conf.py` & `pylemur-0.2.2/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Configuration file for the Sphinx documentation builder.
-#
+
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Path setup --------------------------------------------------------------
 import sys
 from datetime import datetime
@@ -34,18 +34,18 @@
 
 templates_path = ["_templates"]
 nitpicky = True  # Warn about broken links
 needs_sphinx = "4.0"
 
 html_context = {
     "display_github": True,  # Integrate GitHub
-    "github_user": "const-ae",  # Username
-    "github_repo": project_name,  # Repo name
-    "github_version": "main",  # Version
-    "conf_py_path": "/docs/",  # Path in the checkout to the docs root
+    "github_user": "const-ae",
+    "github_repo": "https://github.com/const-ae/pyLemur",
+    "github_version": "main",
+    "conf_py_path": "/docs/",
 }
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings.
 # They can be extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
@@ -83,15 +83,15 @@
     "deflist",
     "dollarmath",
     "html_image",
     "html_admonition",
 ]
 myst_url_schemes = ("http", "https", "mailto")
 nb_output_stderr = "remove"
-nb_execution_mode = "auto"
+nb_execution_mode = "cache"
 nb_merge_streams = True
 typehints_defaults = "braces"
 
 source_suffix = {
     ".rst": "restructuredtext",
     ".ipynb": "myst-nb",
     ".myst": "myst-nb",
```

### Comparing `pylemur-0.2.1/docs/references.bib` & `pylemur-0.2.2/docs/references.bib`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/docs/_static/images/equation_schematic.png` & `pylemur-0.2.2/docs/_static/images/equation_schematic.png`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/docs/_templates/autosummary/class.rst` & `pylemur-0.2.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/docs/extensions/typed_returns.py` & `pylemur-0.2.2/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/docs/notebooks/Tutorial.myst` & `pylemur-0.2.2/docs/notebooks/Tutorial.myst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ---
 output_stderr: remove
 ---
 # Standard imports
 import numpy as np
 import scanpy as sc
 # pertpy is needed to download the Kang data
-import pertpy 
+import pertpy
 
 # This will download the data to ./data/kang_2018.h5ad
 adata = pertpy.data.kang_2018()
 # Store counts separately in the layers
 adata.layers["counts"] = adata.X.copy()
 ```
 
@@ -53,15 +53,15 @@
 ```
 
 ## Preprocessing
 
 LEMUR expects that the input has been variance-stabilized. Here, I will use the log-transformation as a simple, yet effective approach.
 In addition, I will only work on the $1\,000$ most variable genes to make the results easier to manage.
 ```{code-cell} ipython3
-# This follows the standard recommendation from scanpy 
+# This follows the standard recommendation from scanpy
 sc.pp.normalize_total(adata, target_sum = 1e4, inplace=True)
 sc.pp.log1p(adata)
 adata.layers["logcounts"] = adata.X.copy()
 sc.pp.highly_variable_genes(adata, n_top_genes=1000, flavor="cell_ranger")
 adata = adata[:, adata.var.highly_variable]
 adata
 ```
@@ -108,15 +108,15 @@
 ```{code-cell} ipython3
 import matplotlib.pyplot as plt
 adata.layers["diff"] = stim_pred - ctrl_pred
 # Also try CXCL10, IL8, and FBXO40
 sel_gene = "TSC22D3"
 
 fsize = plt.rcParams['figure.figsize']
-fig = plt.figure(figsize=(fsize[0] * 3, fsize[1])) 
+fig = plt.figure(figsize=(fsize[0] * 3, fsize[1]))
 axs = [fig.add_subplot(1, 3, i+1) for i in range(3)]
 for ax in axs:
     ax.set_aspect('equal')
 sc.pl.umap(adata, layer="diff", color=[sel_gene], cmap = plt.get_cmap("seismic"), vcenter=0,
     vmin=-4, vmax=4, title="Pred diff (stim - ctrl)", ax=axs[0], show=False)
 sc.pl.umap(adata[adata.obs["label"]=="ctrl"], layer="logcounts", color=[sel_gene], vmin = 0, vmax =4,
     title="Ctrl expr", ax=axs[1], show=False)
@@ -164,15 +164,15 @@
 plt.scatter(obs_diff, pred_diff, c = obs_diff,
     cmap = plt.get_cmap("seismic"), vmin=-5, vmax=5, marker="o",edgecolors= "black")
 plt.colorbar()
 plt.title( "LEMUR's DE predictions are accurate")
 plt.axline((0, 0), (1, 1), linewidth=1, color='black')
 ```
 
-Another advantage of LEMUR's parametricity is that you could train the model on a subset of the data and then apply it to the full data. 
+Another advantage of LEMUR's parametricity is that you could train the model on a subset of the data and then apply it to the full data.
 
 I will demonstrate this by training the same LEMUR model on 5% of the original data, then `transform` the full data, and finally compare the first three dimensions of the embedding against the embedding from the model trained on the full model.
 
 ```{code-cell} ipython3
 adata_subset = adata[np.random.choice(np.arange(adata.shape[0]), size = round(adata.shape[0] * 0.05)),]
 model_small = pylemur.tl.LEMUR(adata_subset, design = "~ label", n_embedding=15)
 model_small.fit().align_with_harmony()
```

### Comparing `pylemur-0.2.1/notebooks/check_implementation.qmd` & `pylemur-0.2.2/notebooks/check_implementation.qmd`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 title: "Compare implementation directly against R"
 author: Constantin Ahlmann-Eltze
 format:
     html:
         code-fold: false
         embed-resources: true
         highlight-style: github
-        toc: true 
-        code-line-numbers: true 
+        toc: true
+        code-line-numbers: true
 execute:
   keep-ipynb: true
 jupyter: python3
 ---
 
 
 ```{python}
@@ -27,15 +27,15 @@
 debugpy.wait_for_client()
 ```
 
 
 ```{python}
 import numpy as np
 import scanpy as sc
-import pertpy 
+import pertpy
 
 adata = pertpy.data.kang_2018()
 adata.layers["counts"] = adata.X.copy()
 ```
 
 
 ```{python}
```

### Comparing `pylemur-0.2.1/notebooks/devel_experiments.qmd` & `pylemur-0.2.2/notebooks/devel_experiments.qmd`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 title: "Quick check if new functions work as expected"
 author: Constantin Ahlmann-Eltze
 format:
     html:
         code-fold: false
         embed-resources: true
         highlight-style: github
-        toc: true 
-        code-line-numbers: true 
+        toc: true
+        code-line-numbers: true
 execute:
   keep-ipynb: true
 jupyter: python3
 ---
 
 
 ```{python}
@@ -57,15 +57,15 @@
 
 ```{python}
 row_groups(des)
 ```
 
 
 ```{python}
-# 400 cells, 30 features 
+# 400 cells, 30 features
 Y = np.random.rand(400, 30)
 ```
 
 
 ```{python}
 import sklearn.decomposition as skd
```

### Comparing `pylemur-0.2.1/notebooks/kang_analysis_in_R.qmd` & `pylemur-0.2.2/notebooks/kang_analysis_in_R.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -46,22 +46,22 @@
 
 pred_ctrl <- predict(fit, newcondition = cond(label = "ctrl"))
 pred_ctrl[1:3, 1:3]
 ```
 
 
 ```{r}
-py_pred <- t(as.matrix(readr::read_tsv("/var/folders/dc/tppjxs9x6ll378lq88lz1fm40000gq/T//Rtmpm5PTRh/pred_ctrl.tsv", col_names = FALSE)))    
+py_pred <- t(as.matrix(readr::read_tsv("/var/folders/dc/tppjxs9x6ll378lq88lz1fm40000gq/T//Rtmpm5PTRh/pred_ctrl.tsv", col_names = FALSE)))
 dimnames(py_pred) <- dimnames(fit)
 plot(py_pred[1,], pred_ctrl[1,])
 ```
 
 
 ```{r}
-py_emb <- t(as.matrix(readr::read_tsv("/var/folders/dc/tppjxs9x6ll378lq88lz1fm40000gq/T//Rtmpm5PTRh/embedding.tsv", col_names = FALSE)))    
+py_emb <- t(as.matrix(readr::read_tsv("/var/folders/dc/tppjxs9x6ll378lq88lz1fm40000gq/T//Rtmpm5PTRh/embedding.tsv", col_names = FALSE)))
 dimnames(py_emb) <- dimnames(fit$embedding)
 plot(py_emb[1,], fit$embedding[1,])
 ```
 
 ```{r}
 as_tibble(colData(fit)) %>%
     mutate(r_emb = t(fit$embedding),
```

### Comparing `pylemur-0.2.1/notebooks/lemur_model_experiments.qmd` & `pylemur-0.2.2/notebooks/lemur_model_experiments.qmd`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 title: "Play with scanpy"
 author: Constantin Ahlmann-Eltze
 format:
     html:
         code-fold: false
         embed-resources: true
         highlight-style: github
-        toc: true 
-        code-line-numbers: true 
+        toc: true
+        code-line-numbers: true
 execute:
   keep-ipynb: true
 jupyter: python3
 ---
 
 
 ```{python}
@@ -26,15 +26,15 @@
 print("Waiting for debugger attach")
 debugpy.wait_for_client()
 ```
 
 ```{python}
 import numpy as np
 import scanpy as sc
-import pertpy 
+import pertpy
 import scanpy.preprocessing._simple as simple
 
 adata = pertpy.data.kang_2018()
 adata.layers["counts"] = adata.X.copy()
 sf = np.array(adata.layers["counts"].sum(axis=1))
 sf = sf / np.median(sf)
 adata.layers["logcounts"] = sc.pp.log1p(adata.layers["counts"] / sf)
```

### Comparing `pylemur-0.2.1/notebooks/scanpy_experiments.qmd` & `pylemur-0.2.2/notebooks/scanpy_experiments.qmd`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 title: "Play with scanpy"
 author: Constantin Ahlmann-Eltze
 format:
     html:
         code-fold: false
         embed-resources: true
         highlight-style: github
-        toc: true 
-        code-line-numbers: true 
+        toc: true
+        code-line-numbers: true
 execute:
   keep-ipynb: true
 jupyter: python3
 ---
 
 
 ```{python}
@@ -26,15 +26,15 @@
 print("Waiting for debugger attach")
 debugpy.wait_for_client()
 ```
 
 ```{python}
 import numpy as np
 import scanpy as sc
-import pertpy 
+import pertpy
 
 adata = pertpy.data.kang_2018()
 adata
 ```
 
 ```{python}
 adata.obs
```

### Comparing `pylemur-0.2.1/notebooks/test.ipynb` & `pylemur-0.2.2/notebooks/test.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953792735042735%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '\\n'), (4, 'import pertpy\\n'), (5, 'import scanpy as "*

 * *            "sc\\n')], delete: [4, 2]}}, 1: {'source': {insert: [(1, '\\n'), (5, 'fsize = "*

 * *            'plt.rcParams["figure.figsize"]\\n\'), (6, \'fig = plt.figure(figsize=(fsize[0] * 3, '*

 * *            "fsize[1]))\\n'), (7, 'axs = [fig.add_subplot(1, 3, i + 1) for i in range(3)]\\n'), "*

 * *            '(9, \'    ax.set_aspect("equal")\\n\'), (10, \'sc.pl.umap(\\n\'), (11, \'    '*

 * *            'adata,\\n\'), (12,  […]*

```diff
@@ -4,17 +4,18 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Standard imports\n",
                 "import numpy as np\n",
-                "import scanpy as sc\n",
+                "\n",
                 "# pertpy is needed to download the Kang data\n",
-                "import pertpy \n",
+                "import pertpy\n",
+                "import scanpy as sc\n",
                 "\n",
                 "# This will download the data to ./data/kang_2018.h5ad\n",
                 "adata = pertpy.data.kang_2018()\n",
                 "# Store counts separately in the layers\n",
                 "adata.layers[\"counts\"] = adata.X.copy()"
             ]
         },
@@ -47,26 +48,35 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "import matplotlib.pyplot as plt\n",
-                "import numpy as np\n",
+                "\n",
                 "adata.layers[\"diff\"] = np.random.randn(*adata.shape)\n",
                 "sel_gene = \"TNFRSF18\"\n",
                 "\n",
-                "fsize = plt.rcParams['figure.figsize']\n",
-                "fig = plt.figure(figsize=(fsize[0] * 3, fsize[1])) \n",
-                "axs = [fig.add_subplot(1, 3, i+1) for i in range(3)]\n",
+                "fsize = plt.rcParams[\"figure.figsize\"]\n",
+                "fig = plt.figure(figsize=(fsize[0] * 3, fsize[1]))\n",
+                "axs = [fig.add_subplot(1, 3, i + 1) for i in range(3)]\n",
                 "for ax in axs:\n",
-                "    ax.set_aspect('equal')\n",
-                "sc.pl.umap(adata, layer=\"diff\", color=[sel_gene], cmap = plt.get_cmap(\"seismic\"), vcenter=0,\n",
-                "    vmin = -0.5, vmax =0.5, title=\"Pred diff (stim - ctrl)\", ax=axs[0], show=False)\n",
-                "\n"
+                "    ax.set_aspect(\"equal\")\n",
+                "sc.pl.umap(\n",
+                "    adata,\n",
+                "    layer=\"diff\",\n",
+                "    color=[sel_gene],\n",
+                "    cmap=plt.get_cmap(\"seismic\"),\n",
+                "    vcenter=0,\n",
+                "    vmin=-0.5,\n",
+                "    vmax=0.5,\n",
+                "    title=\"Pred diff (stim - ctrl)\",\n",
+                "    ax=axs[0],\n",
+                "    show=False,\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 30,
             "metadata": {},
             "outputs": [
@@ -115,16 +125,25 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "sc.pl.umap(adata, layer=\"diff\", color=[sel_gene, \"YBEY\"], cmap = plt.get_cmap(\"seismic\"), vcenter=0,\n",
-                "    vmin = -0.5, vmax =0.5, title=\"Pred diff (stim - ctrl)\", show=False)"
+                "sc.pl.umap(\n",
+                "    adata,\n",
+                "    layer=\"diff\",\n",
+                "    color=[sel_gene, \"YBEY\"],\n",
+                "    cmap=plt.get_cmap(\"seismic\"),\n",
+                "    vcenter=0,\n",
+                "    vmin=-0.5,\n",
+                "    vmax=0.5,\n",
+                "    title=\"Pred diff (stim - ctrl)\",\n",
+                "    show=False,\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 27,
             "metadata": {},
             "outputs": [
```

### Comparing `pylemur-0.2.1/src/pylemur/pl/basic.py` & `pylemur-0.2.2/src/pylemur/pl/basic.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/src/pylemur/tl/_design_matrix_utils.py` & `pylemur-0.2.2/src/pylemur/tl/_design_matrix_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Mapping
 
 import numpy as np
-from numpy.lib import NumpyVersion
 import pandas as pd
 
 # import patsy
 from formulaic import model_matrix
+from numpy.lib import NumpyVersion
 
 
 def handle_data(data, layer):
     Y = data.X if layer is None else data.layers[layer]
     if not isinstance(Y, np.ndarray):
         Y = Y.toarray()
     return Y
@@ -17,18 +17,21 @@
 
 def handle_design_parameter(design, obs_data):
     if isinstance(design, np.ndarray):
         if design.ndim == 1:
             # Throw error
             raise ValueError("design specified as a 1d array is not supported yet")
         elif design.ndim == 2:
-            design_matrix = design
+            design_matrix = pd.DataFrame(design)
             design_formula = None
         else:
             raise ValueError("design must be a 2d array")
+    elif isinstance(design, pd.DataFrame):
+        design_matrix = design
+        design_formula = None
     elif isinstance(design, list):
         return handle_design_parameter(" * ".join(design), obs_data)
     elif isinstance(design, str):
         # Check if design starts with a ~
         if design[0] != "~":
             design = "~" + design + " - 1"
         design_matrix, design_formula = convert_formula_to_design_matrix(design, obs_data)
@@ -50,16 +53,22 @@
     else:
         return pd.concat([a, b], axis=1)
 
 
 def make_data_frame(data, preferred_index=None):
     if data is None:
         return None
-    if isinstance(data, pd.DataFrame):
+    if isinstance(data, pd.DataFrame) and preferred_index is None:
         return data
+    if isinstance(data, pd.DataFrame) and preferred_index is not None:
+        if preferred_index.equals(data.index) or preferred_index.equals(data.index.map(str)):
+            data.index = preferred_index
+            return data
+        else:
+            raise ValueError("The index of adata.obs and obsData do not match")
     elif isinstance(data, Mapping):
         return pd.DataFrame(data, index=preferred_index)
     else:
         raise ValueError("data must be None, a pandas DataFrame or a Mapping object")
 
 
 def convert_formula_to_design_matrix(formula, obs_data):
@@ -71,15 +80,15 @@
         return design_matrix, formula
     else:
         raise ValueError("formula must be a string")
 
 
 def row_groups(matrix, return_reduced_matrix=False, return_group_ids=False):
     reduced_matrix, inv = np.unique(matrix, axis=0, return_inverse=True)
-    if NumpyVersion(np.__version__) >= '2.0.0rc':
+    if NumpyVersion(np.__version__) >= "2.0.0rc":
         inv = np.squeeze(inv)
     group_ids = np.unique(inv)
     if return_reduced_matrix and return_group_ids:
         return inv, reduced_matrix, group_ids
     elif return_reduced_matrix:
         return inv, reduced_matrix
     elif return_group_ids:
```

### Comparing `pylemur-0.2.1/src/pylemur/tl/_grassmann.py` & `pylemur-0.2.2/src/pylemur/tl/_grassmann.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/src/pylemur/tl/_grassmann_lm.py` & `pylemur-0.2.2/src/pylemur/tl/_grassmann_lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from pylemur.tl._design_matrix_utils import row_groups
 from pylemur.tl._grassmann import grassmann_log, grassmann_map
 from pylemur.tl._lin_alg_wrappers import fit_pca, ridge_regression
 
 
 def grassmann_geodesic_regression(coord_systems, design, base_point, weights=None):
     """
+    Fit geodesic regression on Grassmann manifolds
+
     Solve Sum_j d(U_j, Exp_p(Sum_k V_k:: * X_jk)) for V, where
     d(U, V) = ||Log(U, V)|| is the inverse of the exponential map on the Grassmann manifold.
 
     Parameters
     ----------
     coord_systems : a list of orthonormal 2D matrices (length n_groups)
     design : design matrix, shape (n_groups, n_coef)
@@ -29,17 +31,15 @@
 
     assert len(coord_systems) == n_obs
     for i in range(n_obs):
         assert coord_systems[i].shape == (n_emb, n_features)
     if weights is None:
         weights = np.ones(n_obs)
 
-    tangent_vecs = [
-        grassmann_log(base_point.T, coord_systems[i].T).T.reshape(n_emb * n_features) for i in range(n_obs)
-    ]
+    tangent_vecs = [grassmann_log(base_point.T, coord_systems[i].T).T.reshape(n_emb * n_features) for i in range(n_obs)]
     tangent_vecs = np.vstack(tangent_vecs)
     if tangent_vecs.shape[0] == 0:
         tangent_fit = np.zeros((0, n_coef))
     else:
         tangent_fit = ridge_regression(tangent_vecs, design, weights=weights)
 
     tangent_fit = tangent_fit.reshape((n_coef, n_emb, n_features)).transpose((1, 2, 0))
```

### Comparing `pylemur-0.2.1/src/pylemur/tl/_lin_alg_wrappers.py` & `pylemur-0.2.2/src/pylemur/tl/_lin_alg_wrappers.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/src/pylemur/tl/alignment.py` & `pylemur-0.2.2/src/pylemur/tl/alignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     n_obs = embedding.shape[0]
     des_row_groups, des_row_group_ids = row_groups(design_matrix, return_group_ids=True)
     n_groups = len(des_row_group_ids)
     if nclust is None:
         nclust = np.min([np.round(n_obs / 30.0), 100]).astype(int)
 
     phi = np.eye(n_groups)[:, des_row_groups]
-    phi_n = np.ones(n_groups)
+    # phi_n = np.ones(n_groups)
 
     N_b = phi.sum(axis=1)
     Pr_b = N_b / n_obs
     sigma = np.repeat(sigma, nclust)
 
     theta = np.repeat(theta, n_groups)
     theta = theta * (1 - np.exp(-((N_b / (nclust * tau)) ** 2)))
```

### Comparing `pylemur-0.2.1/src/pylemur/tl/lemur.py` & `pylemur-0.2.2/src/pylemur/tl/lemur.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import re
 import warnings
 from collections.abc import Iterable, Mapping
-from typing import Any, Literal, Union
+from typing import Any, Literal
 
 import anndata as ad
 import formulaic
 import numpy as np
+import pandas as pd
 from sklearn.exceptions import NotFittedError
 
-from pylemur.tl._design_matrix_utils import *
+from pylemur.tl._design_matrix_utils import handle_data, handle_design_parameter, handle_obs_data, row_groups
 from pylemur.tl._grassmann import grassmann_map
 from pylemur.tl._grassmann_lm import grassmann_lm, project_data_on_diffemb
-from pylemur.tl._lin_alg_wrappers import *
+from pylemur.tl._lin_alg_wrappers import fit_pca, multiply_along_axis, ridge_regression
 from pylemur.tl.alignment import (
     _align_impl,
     _apply_linear_transformation,
     _init_harmony,
     _reverse_linear_transformation,
 )
 
 
 class LEMUR:
-    """Fit the LEMUR model
+    r"""Fit the LEMUR model
 
     A python implementation of the LEMUR algorithm. For more details please refer
     to Ahlmann-Eltze (2024).
 
     Parameters
     ----------
     data
-        The AnnData object containing the variance stabilized data and the
+        The AnnData object (or a different matrix container) with the variance stabilized data and the
         cell-wise annotations in `data.obs`.
     design
         A specification of the experimental design. This can be a string,
         which is then parsed using `formulaic`. Alternatively, it can be a
         a list of strings, which are assumed to refer to the columns in
         `data.obs`. Finally, it can be a numpy array, representing a
         design matrix of size `n_cells` x `n_covariates`. If not provided,
@@ -50,55 +51,58 @@
         the linear coefficients are set to zero.
     layer
         The name of the layer to use in `data`. If `None`, the `X` slot is used.
     copy
         Whether to make a copy of `data`.
 
     Attributes
-    ----------    
-    embedding : :class:`~numpy.ndarray` (:math:`C \\times P`)
-        Low-dimensional representation of each cell 
+    ----------
+    embedding : :class:`~numpy.ndarray` (:math:`C \times P`)
+        Low-dimensional representation of each cell
     adata : :class:`~anndata.AnnData`
         A reference to (potentially a copy of) the input data.
-    data_matrix : :class:`~numpy.ndarray` (:math:`C \\times G`)
+    data_matrix : :class:`~numpy.ndarray` (:math:`C \times G`)
         A reference to the data matrix from the `adata` object.
     n_embedding : int
         The number of latent dimensions
-    design_matrix : :class:`~formulaic.model_matrix.ModelMatrix` (:math:`C \\times K`)
+    design_matrix : `ModelMatrix` (:math:`C \times K`)
         The design matrix that is used for the fit.
     formula : str
         The design formula specification.
-    coefficients : :class:`~numpy.ndarray` (:math:`P \\times G \\times K`)
+    coefficients : :class:`~numpy.ndarray` (:math:`P \times G \times K`)
         The 3D array of coefficients for the Grassmann regression.
-    alignment_coefficients : :class:`~numpy.ndarray` (:math:`P \\times (P+1) \\times K`)
+    alignment_coefficients : :class:`~numpy.ndarray` (:math:`P \times (P+1) \times K`)
         The 3D array of coefficients for the affine alignment.
-    linear_coefficients : :class:`~numpy.ndarray` (:math:`K\\times G`)
+    linear_coefficients : :class:`~numpy.ndarray` (:math:`K\times G`)
         The 2D array of coefficients for the linear offset per condition.
     linear_coefficient_estimator : str
         The linear coefficient estimation specification.
-    base_point :  :class:`~numpy.ndarray` (:math:`(P \\times G`))
+    base_point :  :class:`~numpy.ndarray` (:math:`(P \times G`))
         The 2D array representing the reference subspace.
-    
+
     Examples
     --------
-    >>> model = pylemur.tl.LEMUR(adata, design = "~ label + batch_cov", n_embedding=15)
+    >>> model = pylemur.tl.LEMUR(adata, design="~ label + batch_cov", n_embedding=15)
     >>> model.fit()
     >>> model.align_with_harmony()
-    >>> pred_expr = model.predict(new_condition = model.cond(label="treated"))
+    >>> pred_expr = model.predict(new_condition=model.cond(label="treated"))
     >>> emb_proj = model_small.transform(adata)
     """
 
-    def __init__(self,
-                 adata: ad.AnnData,
-                 design: Union[str, list[str], np.ndarray] = "~ 1",
-                 obs_data: Union[pd.DataFrame, Mapping[str, Iterable[Any]], None] = None,
-                 n_embedding: int = 15,
-                 linear_coefficient_estimator: Literal["linear", "zero"] = "linear",
-                 layer: Union[str, None] = None,
-                 copy: bool = True):
+    def __init__(
+        self,
+        adata: ad.AnnData | Any,
+        design: str | list[str] | np.ndarray = "~ 1",
+        obs_data: pd.DataFrame | Mapping[str, Iterable[Any]] | None = None,
+        n_embedding: int = 15,
+        linear_coefficient_estimator: Literal["linear", "zero"] = "linear",
+        layer: str | None = None,
+        copy: bool = True,
+    ):
+        adata = _handle_data_arg(adata)
         if copy:
             adata = adata.copy()
         self.adata = adata
 
         adata.obs = handle_obs_data(adata, obs_data)
         design_matrix, formula = handle_design_parameter(design, adata.obs)
         self.design_matrix = design_matrix
@@ -117,15 +121,15 @@
     def fit(self, verbose: bool = True):
         """Fit the LEMUR model
 
         Parameters
         ----------
         verbose
             Whether to print progress to the console.
-        
+
         Returns
         -------
         `self`
             The fitted LEMUR model.
         """
         Y = self.data_matrix
         design_matrix = self.design_matrix
@@ -145,26 +149,26 @@
         if verbose:
             print("Fit regression on latent spaces")
         coefficients = grassmann_lm(Y, design_matrix.to_numpy(), base_point)
         if verbose:
             print("Find shared embedding coordinates")
         embedding = project_data_on_diffemb(Y, design_matrix.to_numpy(), coefficients, base_point)
 
-        embedding, coefficients, base_point = order_axis_by_variance(embedding, coefficients, base_point)
+        embedding, coefficients, base_point = _order_axis_by_variance(embedding, coefficients, base_point)
 
         self.embedding = embedding
         self.alignment_coefficients = np.zeros((n_embedding, n_embedding + 1, design_matrix.shape[1]))
         self.coefficients = coefficients
         self.base_point = base_point
         self.linear_coefficients = lin_coef
 
         return self
 
     def align_with_harmony(
-        self, ridge_penalty: Union[float, list[float], np.ndarray] = 0.01, max_iter: int = 10, verbose: bool = True
+        self, ridge_penalty: float | list[float] | np.ndarray = 0.01, max_iter: int = 10, verbose: bool = True
     ):
         """Fine-tune the embedding with a parametric version of Harmony.
 
         Parameters
         ----------
         ridge_penalty
             The penalty controlling the flexibility of the alignment. Smaller
@@ -178,14 +182,20 @@
         Returns
         -------
         `self`
             The fitted LEMUR model with the updated embedding space stored in
             `model.embedding` attribute and an the updated alignment coefficients
             stored in `model.alignment_coefficients`.
         """
+        if self.embedding is None:
+            raise NotFittedError(
+                "self.embedding is None. Make sure to call 'model.fit()' "
+                + "before calling 'model.align_with_harmony()'."
+            )
+
         embedding = self.embedding.copy()
         design_matrix = self.design_matrix
         # Init harmony
         harm_obj = _init_harmony(embedding, design_matrix, verbose=verbose)
         for idx in range(max_iter):
             if verbose:
                 print(f"Alignment iteration {idx}")
@@ -209,19 +219,18 @@
                 if verbose:
                     print("Converged")
                 break
         self.alignment_coefficients = al_coef
         self.embedding = _apply_linear_transformation(embedding, al_coef, design_matrix)
         return self
 
-
     def align_with_grouping(
         self,
-        grouping: Union[list, np.ndarray, pd.Series],
-        ridge_penalty: Union[float, list[float], np.ndarray] = 0.01,
+        grouping: list | np.ndarray | pd.Series,
+        ridge_penalty: float | list[float] | np.ndarray = 0.01,
         preserve_position_of_NAs: bool = False,
         verbose: bool = True,
     ):
         """Fine-tune the embedding using annotated groups of cells.
 
         Parameters
         ----------
@@ -239,81 +248,96 @@
         Returns
         -------
         `self`
             The fitted LEMUR model with the updated embedding space stored in
             `model.embedding` attribute and an the updated alignment coefficients
             stored in `model.alignment_coefficients`.
         """
+        if self.embedding is None:
+            raise NotFittedError(
+                "self.embedding is None. Make sure to call 'model.fit()' "
+                + "before calling 'model.align_with_grouping()'."
+            )
         embedding = self.embedding.copy()
         design_matrix = self.design_matrix
         if isinstance(grouping, list):
             grouping = pd.Series(grouping)
 
         if isinstance(grouping, pd.Series):
             grouping = grouping.factorize()[0] * 1.0
             grouping[grouping == -1] = np.nan
 
         al_coef = _align_impl(
-            embedding, grouping, design_matrix, ridge_penalty=ridge_penalty, calculate_new_embedding=False, verbose=verbose
+            embedding,
+            grouping,
+            design_matrix,
+            ridge_penalty=ridge_penalty,
+            calculate_new_embedding=False,
+            verbose=verbose,
         )
         self.alignment_coefficients = al_coef
-        self.embedding =  _apply_linear_transformation(embedding, al_coef, design_matrix)
+        self.embedding = _apply_linear_transformation(embedding, al_coef, design_matrix)
         return self
 
-    def transform(self, adata: ad.AnnData, layer: Union[str, None] = None,
-                  obs_data: Union[pd.DataFrame, Mapping[str, Iterable[Any]], None] = None,
-                  return_type: Literal["embedding", "LEMUR"] = "embedding"):
+    def transform(
+        self,
+        adata: ad.AnnData,
+        layer: str | None = None,
+        obs_data: pd.DataFrame | Mapping[str, Iterable[Any]] | None = None,
+        return_type: Literal["embedding", "LEMUR"] = "embedding",
+    ):
         """Transform data using the fitted LEMUR model
 
         Parameters
         ----------
         adata
             The AnnData object to transform.
         obs_data
-            Optional set of annotations for each cell (same as `obs_data` in the 
+            Optional set of annotations for each cell (same as `obs_data` in the
             constructor).
         return_type
             Flag that decides if the function returns a full `LEMUR` object or
             only the embedding.
 
         Returns
         -------
         :class:`~pylemur.tl.LEMUR`
-            (if `return_type = "LEMUR"`) A new `LEMUR` object object with the embedding 
+            (if `return_type = "LEMUR"`) A new `LEMUR` object object with the embedding
             calculated for the input `adata`.
-        
+
         :class:`~numpy.ndarray`
             (if `return_type = "embedding"`) A 2D numpy array of the embedding matrix
             calculated for the input `adata` (with cells in the rows and latent dimensions
             in the columns).
         """
         Y = handle_data(adata, layer)
         adata.obs = handle_obs_data(adata, obs_data)
         design_matrix, _ = handle_design_parameter(self.formula, adata.obs)
         dm = design_matrix.to_numpy()
         Y_clean = Y - dm @ self.linear_coefficients
-        embedding = project_data_on_diffemb(Y_clean, design_matrix = dm, coefficients = self.coefficients,
-                                            base_point = self.base_point)
+        embedding = project_data_on_diffemb(
+            Y_clean, design_matrix=dm, coefficients=self.coefficients, base_point=self.base_point
+        )
         embedding = _apply_linear_transformation(embedding, self.alignment_coefficients, dm)
         if return_type == "embedding":
             return embedding
         elif return_type == "LEMUR":
             fit = LEMUR.copy()
             fit.adata = adata
             fit.design_matrix = design_matrix
             fit.embedding = embedding
             return fit
 
-
-    def predict(self,
-        embedding: Union[np.ndarray, None] = None,
-        new_design: Union[str, list[str], np.ndarray, None] = None,
-        new_condition: Union[np.ndarray, pd.DataFrame, None] = None,
-        obs_data: Union[pd.DataFrame, Mapping[str, Iterable[Any]], None] = None,
-        new_adata_layer: Union[None, str] = None
+    def predict(
+        self,
+        embedding: np.ndarray | None = None,
+        new_design: str | list[str] | np.ndarray | None = None,
+        new_condition: np.ndarray | pd.DataFrame | None = None,
+        obs_data: pd.DataFrame | Mapping[str, Iterable[Any]] | None = None,
+        new_adata_layer: None | str = None,
     ):
         """Predict the expression of cells in a specific condition
 
         Parameters
         ----------
         embedding
             The coordinates of the cells in the shared embedding space. If None,
@@ -341,15 +365,15 @@
         if embedding is None:
             if self.embedding is None:
                 raise NotFittedError("The model has not been fitted yet.")
             embedding = self.embedding
 
         if new_condition is not None:
             if new_design is not None:
-                warnings.warn("new_design is ignored if new_condition is provided.")
+                warnings.warn("new_design is ignored if new_condition is provided.", stacklevel=1)
 
             if isinstance(new_condition, pd.DataFrame):
                 new_design = new_condition.to_numpy()
             elif isinstance(new_condition, np.ndarray):
                 new_design = new_condition
             else:
                 raise ValueError("new_condition must be a created using 'cond(...)' or a numpy array.")
@@ -371,43 +395,44 @@
             new_design, return_reduced_matrix=True, return_group_ids=True
         )
         for id in des_row_group_ids:
             covars = reduced_design_matrix[id, :]
             subspace = grassmann_map(np.dot(coef, covars).T, self.base_point.T)
             alignment = _reverse_linear_transformation(al_coefs, covars)
             offset = np.dot(al_coefs[:, 0, :], covars)
-            approx[des_row_groups == id, :] += ((embedding[des_row_groups == id, :] - offset) @ alignment.T) @ subspace.T
+            approx[des_row_groups == id, :] += (
+                (embedding[des_row_groups == id, :] - offset) @ alignment.T
+            ) @ subspace.T
         if new_adata_layer is not None:
             self.adata.layers[new_adata_layer] = approx
             return self
         else:
             return approx
 
-
     def cond(self, **kwargs):
         """Define a condition for the `predict` function.
 
         Parameters
         ----------
         fit
             The AnnData object produced by `lemur`.
         kwargs
             Named arguments specifying the levels of the covariates from the
             design formula. If a covariate is not specified, the first level is
             used.
 
         Returns
         -------
-        :class:`~formulaic.model_matrix.ModelMatrix`
-            A ModelMatrix instance with one row with the same columns as the design matrix. 
-            
+        `ModelMatrix`
+            A ModelMatrix instance with one row with the same columns as the design matrix.
+
 
         Notes
         -----
-        Subtracting two `cond(...)` calls, produces a contrast vector; these are 
+        Subtracting two `cond(...)` calls, produces a contrast vector; these are
         commonly used in `R` to test for differences in a regression model.
         This pattern is inspired by the `R` package `glmGamPoi <https://bioconductor.org/packages/glmGamPoi/>`__.
         """
 
         # This is copied from https://github.com/scverse/multi-condition-comparisions/blob/main/src/multi_condition_comparisions/tl/de.py#L164
         def _get_var_from_colname(colname):
             regex = re.compile(r"^.+\[T\.(.+)\]$")
@@ -450,14 +475,20 @@
     def __str__(self):
         if self.embedding is None:
             return f"LEMUR model (not fitted yet) with {self.n_embedding} dimensions"
         else:
             return f"LEMUR model with {self.n_embedding} dimensions"
 
 
+def _handle_data_arg(data):
+    if isinstance(data, ad.AnnData):
+        return data
+    else:
+        return ad.AnnData(data)
+
 
-def order_axis_by_variance(embedding, coefficients, base_point):
+def _order_axis_by_variance(embedding, coefficients, base_point):
     U, d, Vt = np.linalg.svd(embedding, full_matrices=False)
     base_point = Vt @ base_point
     coefficients = np.einsum("pq,qij->pij", Vt, coefficients)
     embedding = U @ np.diag(d)
     return embedding, coefficients, base_point
```

### Comparing `pylemur-0.2.1/tests/test_grasmann_lm.py` & `pylemur-0.2.2/tests/test_grasmann_lm.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     # The projection and the embedding are rotated to each other
     # Remove rotation effect using orthogonal procrustes
     U, _, Vt = np.linalg.svd(proj.T @ pca.embedding, full_matrices=False)
     rot = U @ Vt
     assert np.allclose(proj @ rot, pca.embedding)
 
 
-def test_project_data_on_diffemb():
+def test_project_data_on_diffemb2():
     n_obs = 100
     base_point = grassmann_project(np.random.randn(5, 2)).T
     data = np.random.randn(n_obs, 5)
     des = np.ones((n_obs, 1))
     fit = grassmann_lm(data, des, base_point)
     pca = fit_pca(data, 2, center=False)
     angle = grassmann_angle_from_point(grassmann_map(fit[:, :, 0].T, base_point.T), pca.coord_system.T)
```

### Comparing `pylemur-0.2.1/tests/test_grassmann.py` & `pylemur-0.2.2/tests/test_grassmann.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/tests/test_lin_alg_utils.py` & `pylemur-0.2.2/tests/test_lin_alg_utils.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/.gitignore` & `pylemur-0.2.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -51,20 +51,19 @@
 /dist/
 /*.egg-info/
 
 # Tests and coverage
 /.pytest_cache/
 /.cache/
 /data/
+/node_modules/
 
 # docs
 /docs/generated/
 /docs/_build/
 
 # IDEs
 /.idea/
 /.vscode/
 
 # Data files from tutorial
 docs/notebooks/data/*
-
-
```

### Comparing `pylemur-0.2.1/LICENSE` & `pylemur-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylemur-0.2.1/README.md` & `pylemur-0.2.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,48 +6,71 @@
 [badge-tests]: https://img.shields.io/github/actions/workflow/status/const-ae/pyLemur/test.yaml?branch=main
 [link-tests]: https://github.com/const-ae/pyLemur/actions/workflows/test.yaml
 [link-docs]: https://pyLemur.readthedocs.io
 [badge-docs]: http://readthedocs.org/projects/pylemur/badge
 
 The Python implementation of the LEMUR method to analyze multi-condition single-cell data. For the more complete version in R, see [github.com/const-ae/lemur](https://github.com/const-ae/lemur). To learn more check-out the [function documentation](https://pylemur.readthedocs.io/page/api.html) and the [tutorial](https://pylemur.readthedocs.io/page/notebooks/Tutorial.html) at [pylemur.readthedocs.io](https://pylemur.readthedocs.io). To check-out the source code or submit an issue go to [github.com/const-ae/pyLemur](https://github.com/const-ae/pyLemur)
 
-
-
 ## Citation
 
-> Ahlmann-Eltze C, Huber W (2024). 
-“Analysis of multi-condition single-cell data with latent embedding multivariate regression.” bioRxiv. 
-[doi:10.1101/2023.03.06.531268](https://doi.org/10.1101/2023.03.06.531268).
+> Ahlmann-Eltze C, Huber W (2024).
+> “Analysis of multi-condition single-cell data with latent embedding multivariate regression.” bioRxiv.
+> [doi:10.1101/2023.03.06.531268](https://doi.org/10.1101/2023.03.06.531268).
 
 # Getting started
 
 ## Installation
 
-You need to have Python 3.9 or newer installed on your system. 
+You need to have Python 3.10 or newer installed on your system.
 There are several alternative options to install pyLemur:
 
-
 Install the latest release of `pyLemur` from [PyPI](https://pypi.org/project/pyLemur/):
+
 ```bash
 pip install pyLemur
 ```
 
-
 Alternatively, install the latest development version directly from Github:
+
 ```bash
 pip install git+https://github.com/const-ae/pyLemur.git@main
 ```
 
 ## Documentation
 
 For more information on the functions see the [API docs](https://pyLemur.readthedocs.io/page/api.html) and the [tutorial](https://pylemur.readthedocs.io/page/notebooks/Tutorial.html).
 
 ## Contact
 
 For questions and help requests, you can reach out in the [scverse discourse][scverse-discourse].
 If you found a bug, please use the [issue tracker][issue-tracker].
 
+[scverse-discourse]: https://discourse.scverse.org/
+[issue-tracker]: https://github.com/const-ae/pyLemur/issues
 
+## Building
 
+Build the documentation locally
 
-[scverse-discourse]: https://discourse.scverse.org/
-[issue-tracker]: https://github.com/const-ae/pyLemur/issues
+```
+cd docs
+make html
+open _build/html/index.html
+```
+
+Run the unit tests
+
+```
+pytest
+```
+
+Run pre-commit hooks manually
+
+```
+pre-commit run --all-files
+```
+
+or individually
+
+```
+ruff check
+```
```

### Comparing `pylemur-0.2.1/pyproject.toml` & `pylemur-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "pyLemur"
-version = "0.2.1"
+version = "0.2.2"
 description = "A Python implementation of the LEMUR algorithm for analyzing multi-condition single-cell RNA-seq data."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 license = {file = "LICENSE"}
 authors = [
     {name = "Constantin Ahlmann-Eltze"},
 ]
 maintainers = [
     {name = "Constantin Ahlmann-Eltze", email = "artjom31415@googlemail.com"},
 ]
@@ -34,15 +34,15 @@
     "pre-commit",
     "twine>=4.0.2",
 ]
 doc = [
     "docutils>=0.8,!=0.18.*,!=0.19.*",
     "sphinx>=4",
     "sphinx-book-theme>=1.0.0",
-    "myst-nb",
+    "myst-nb>=1.1.0",
     "sphinxcontrib-bibtex>=1.0.0",
     "sphinx-autodoc-typehints",
     "sphinxext-opengraph",
     "sphinx-design",
     # For notebooks
     "ipykernel",
     "ipython",
@@ -104,15 +104,15 @@
     "D104",
     # Missing docstring in public module
     "D100",
     # Missing docstring in __init__
     "D107",
     # Errors from function calls in argument defaults. These are fine when the result is immutable.
     "B008",
-    # __magic__ methods are are often self-explanatory, allow missing docstrings
+    # __magic__ methods are often self-explanatory, allow missing docstrings
     "D105",
     # first line should end with a period [Bug: doesn't work with single-line docstrings]
     "D400",
     # First line should be in imperative mood; try rephrasing
     "D401",
     ## Disable one in each pair of mutually incompatible rules
     # We don’t want a blank line before a class docstring
@@ -122,15 +122,20 @@
 ]
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.ruff.lint.per-file-ignores]
 "docs/*" = ["I"]
-"tests/*" = ["D"]
+"tests/*" = [
+    # Pydoc doesn't mattter in tests
+    "D",
+    # Ignore star imports in tests
+    "F403", "F405"
+]
 "*/__init__.py" = ["F401"]
 
 [tool.cruft]
 skip = [
     "tests",
     "src/**/__init__.py",
     "src/**/basic.py",
```

### Comparing `pylemur-0.2.1/PKG-INFO` & `pylemur-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyLemur
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python implementation of the LEMUR algorithm for analyzing multi-condition single-cell RNA-seq data.
 Project-URL: Documentation, https://pyLemur.readthedocs.io/
 Project-URL: Source, https://github.com/const-ae/pyLemur
 Project-URL: Home-page, https://github.com/const-ae/pyLemur
 Author: Constantin Ahlmann-Eltze
 Maintainer-email: Constantin Ahlmann-Eltze <artjom31415@googlemail.com>
 License: MIT License
@@ -25,15 +25,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Requires-Dist: anndata
 Requires-Dist: formulaic
 Requires-Dist: harmonypy
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: session-info
@@ -41,15 +41,15 @@
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: twine>=4.0.2; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: docutils!=0.18.*,!=0.19.*,>=0.8; extra == 'doc'
 Requires-Dist: ipykernel; extra == 'doc'
 Requires-Dist: ipython; extra == 'doc'
 Requires-Dist: matplotlib; extra == 'doc'
-Requires-Dist: myst-nb; extra == 'doc'
+Requires-Dist: myst-nb>=1.1.0; extra == 'doc'
 Requires-Dist: pandas; extra == 'doc'
 Requires-Dist: pertpy; extra == 'doc'
 Requires-Dist: scanpy; extra == 'doc'
 Requires-Dist: session-info; extra == 'doc'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'doc'
 Requires-Dist: sphinx-book-theme>=1.0.0; extra == 'doc'
 Requires-Dist: sphinx-copybutton; extra == 'doc'
@@ -70,48 +70,71 @@
 [badge-tests]: https://img.shields.io/github/actions/workflow/status/const-ae/pyLemur/test.yaml?branch=main
 [link-tests]: https://github.com/const-ae/pyLemur/actions/workflows/test.yaml
 [link-docs]: https://pyLemur.readthedocs.io
 [badge-docs]: http://readthedocs.org/projects/pylemur/badge
 
 The Python implementation of the LEMUR method to analyze multi-condition single-cell data. For the more complete version in R, see [github.com/const-ae/lemur](https://github.com/const-ae/lemur). To learn more check-out the [function documentation](https://pylemur.readthedocs.io/page/api.html) and the [tutorial](https://pylemur.readthedocs.io/page/notebooks/Tutorial.html) at [pylemur.readthedocs.io](https://pylemur.readthedocs.io). To check-out the source code or submit an issue go to [github.com/const-ae/pyLemur](https://github.com/const-ae/pyLemur)
 
-
-
 ## Citation
 
-> Ahlmann-Eltze C, Huber W (2024). 
-“Analysis of multi-condition single-cell data with latent embedding multivariate regression.” bioRxiv. 
-[doi:10.1101/2023.03.06.531268](https://doi.org/10.1101/2023.03.06.531268).
+> Ahlmann-Eltze C, Huber W (2024).
+> “Analysis of multi-condition single-cell data with latent embedding multivariate regression.” bioRxiv.
+> [doi:10.1101/2023.03.06.531268](https://doi.org/10.1101/2023.03.06.531268).
 
 # Getting started
 
 ## Installation
 
-You need to have Python 3.9 or newer installed on your system. 
+You need to have Python 3.10 or newer installed on your system.
 There are several alternative options to install pyLemur:
 
-
 Install the latest release of `pyLemur` from [PyPI](https://pypi.org/project/pyLemur/):
+
 ```bash
 pip install pyLemur
 ```
 
-
 Alternatively, install the latest development version directly from Github:
+
 ```bash
 pip install git+https://github.com/const-ae/pyLemur.git@main
 ```
 
 ## Documentation
 
 For more information on the functions see the [API docs](https://pyLemur.readthedocs.io/page/api.html) and the [tutorial](https://pylemur.readthedocs.io/page/notebooks/Tutorial.html).
 
 ## Contact
 
 For questions and help requests, you can reach out in the [scverse discourse][scverse-discourse].
 If you found a bug, please use the [issue tracker][issue-tracker].
 
+[scverse-discourse]: https://discourse.scverse.org/
+[issue-tracker]: https://github.com/const-ae/pyLemur/issues
 
+## Building
 
+Build the documentation locally
 
-[scverse-discourse]: https://discourse.scverse.org/
-[issue-tracker]: https://github.com/const-ae/pyLemur/issues
+```
+cd docs
+make html
+open _build/html/index.html
+```
+
+Run the unit tests
+
+```
+pytest
+```
+
+Run pre-commit hooks manually
+
+```
+pre-commit run --all-files
+```
+
+or individually
+
+```
+ruff check
+```
```

