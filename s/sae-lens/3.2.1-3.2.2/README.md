# Comparing `tmp/sae_lens-3.2.1.tar.gz` & `tmp/sae_lens-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-3.2.1.tar", max compression
+gzip compressed data, was "sae_lens-3.2.2.tar", max compression
```

## Comparing `sae_lens-3.2.1.tar` & `sae_lens-3.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-06-02 21:11:35.509813 sae_lens-3.2.1/LICENSE
--rw-r--r--   0        0        0     3381 2024-06-02 21:11:35.509813 sae_lens-3.2.1/README.md
--rw-r--r--   0        0        0     2007 2024-06-02 21:11:36.881817 sae_lens-3.2.1/pyproject.toml
--rw-r--r--   0        0        0      898 2024-06-02 21:11:36.881817 sae_lens-3.2.1/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0     3320 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    12561 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/hooked_sae_transformer.py
--rw-r--r--   0        0        0    17062 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20406 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     4052 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/batching.py
--rw-r--r--   0        0        0     6047 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/cache_activations_runner.py
--rw-r--r--   0        0        0    24486 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/config.py
--rw-r--r--   0        0        0    16161 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/dashboard_runner.py
--rw-r--r--   0        0        0     7966 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/evals.py
--rw-r--r--   0        0        0     1320 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/load_model.py
--rw-r--r--   0        0        0     5383 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/pretokenize_runner.py
--rw-r--r--   0        0        0     4833 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0    14329 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/sae.py
--rw-r--r--   0        0        0     6972 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/sae_training_runner.py
--rw-r--r--   0        0        0        0 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     8087 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     4752 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0     1783 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/toy_model_runner.py
--rw-r--r--   0        0        0        0 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/__init__.py
--rw-r--r--   0        0        0    21162 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     3779 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     5585 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/optim.py
--rw-r--r--   0        0        0    14209 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/sae_trainer.py
--rw-r--r--   0        0        0    18481 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0     4850 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/train_toy_sae.py
--rw-r--r--   0        0        0    15495 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/training_sae.py
--rw-r--r--   0        0        0     4611 1970-01-01 00:00:00.000000 sae_lens-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-06-02 21:34:11.605923 sae_lens-3.2.2/LICENSE
+-rw-r--r--   0        0        0     3381 2024-06-02 21:34:11.605923 sae_lens-3.2.2/README.md
+-rw-r--r--   0        0        0     2007 2024-06-02 21:34:13.101925 sae_lens-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0      898 2024-06-02 21:34:13.101925 sae_lens-3.2.2/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0     3320 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    12561 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/analysis/hooked_sae_transformer.py
+-rw-r--r--   0        0        0    17062 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20406 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     4052 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/batching.py
+-rw-r--r--   0        0        0     6047 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/cache_activations_runner.py
+-rw-r--r--   0        0        0    24486 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/config.py
+-rw-r--r--   0        0        0    16161 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/dashboard_runner.py
+-rw-r--r--   0        0        0     7966 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/evals.py
+-rw-r--r--   0        0        0     1320 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/load_model.py
+-rw-r--r--   0        0        0     5383 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/pretokenize_runner.py
+-rw-r--r--   0        0        0     4833 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0    14329 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/sae.py
+-rw-r--r--   0        0        0     6972 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/sae_training_runner.py
+-rw-r--r--   0        0        0        0 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     8087 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     4752 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0     1783 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/toy_model_runner.py
+-rw-r--r--   0        0        0        0 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0    21163 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     3779 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     5585 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/training/optim.py
+-rw-r--r--   0        0        0    14209 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/training/sae_trainer.py
+-rw-r--r--   0        0        0    18481 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0     4850 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/training/train_toy_sae.py
+-rw-r--r--   0        0        0    15495 2024-06-02 21:34:11.617923 sae_lens-3.2.2/sae_lens/training/training_sae.py
+-rw-r--r--   0        0        0     4611 1970-01-01 00:00:00.000000 sae_lens-3.2.2/PKG-INFO
```

### Comparing `sae_lens-3.2.1/LICENSE` & `sae_lens-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/README.md` & `sae_lens-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/pyproject.toml` & `sae_lens-3.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "3.2.1"
+version = "3.2.2"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `sae_lens-3.2.1/sae_lens/__init__.py` & `sae_lens-3.2.2/sae_lens/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.2.1"
+__version__ = "3.2.2"
 
 
 from .analysis.hooked_sae_transformer import HookedSAETransformer
 from .cache_activations_runner import CacheActivationsRunner
 from .config import (
     CacheActivationsRunnerConfig,
     LanguageModelSAERunnerConfig,
```

### Comparing `sae_lens-3.2.1/sae_lens/analysis/feature_statistics.py` & `sae_lens-3.2.2/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/analysis/hooked_sae_transformer.py` & `sae_lens-3.2.2/sae_lens/analysis/hooked_sae_transformer.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-3.2.2/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-3.2.2/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/analysis/tsea.py` & `sae_lens-3.2.2/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/batching.py` & `sae_lens-3.2.2/sae_lens/batching.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/cache_activations_runner.py` & `sae_lens-3.2.2/sae_lens/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/config.py` & `sae_lens-3.2.2/sae_lens/config.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/dashboard_runner.py` & `sae_lens-3.2.2/sae_lens/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/evals.py` & `sae_lens-3.2.2/sae_lens/evals.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/load_model.py` & `sae_lens-3.2.2/sae_lens/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/pretokenize_runner.py` & `sae_lens-3.2.2/sae_lens/pretokenize_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/pretrained_saes.yaml` & `sae_lens-3.2.2/sae_lens/pretrained_saes.yaml`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/sae.py` & `sae_lens-3.2.2/sae_lens/sae.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/sae_training_runner.py` & `sae_lens-3.2.2/sae_lens/sae_training_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/toolkit/pretrained_sae_loaders.py` & `sae_lens-3.2.2/sae_lens/toolkit/pretrained_sae_loaders.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-3.2.2/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-3.2.2/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/toy_model_runner.py` & `sae_lens-3.2.2/sae_lens/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/training/activations_store.py` & `sae_lens-3.2.2/sae_lens/training/activations_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -534,15 +534,15 @@
     def _get_next_dataset_tokens(self) -> torch.Tensor:
         device = self.device
         if not self.is_dataset_tokenized:
             s = next(self.iterable_dataset)[self.tokens_column]
             tokens = (
                 self.model.to_tokens(
                     s,
-                    truncate=True,
+                    truncate=False,
                     move_to_device=True,
                     prepend_bos=self.prepend_bos,
                 )
                 .squeeze(0)
                 .to(device)
             )
             assert (
```

### Comparing `sae_lens-3.2.1/sae_lens/training/geometric_median.py` & `sae_lens-3.2.2/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/training/optim.py` & `sae_lens-3.2.2/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/training/sae_trainer.py` & `sae_lens-3.2.2/sae_lens/training/sae_trainer.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/training/toy_models.py` & `sae_lens-3.2.2/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/training/train_toy_sae.py` & `sae_lens-3.2.2/sae_lens/training/train_toy_sae.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/sae_lens/training/training_sae.py` & `sae_lens-3.2.2/sae_lens/training/training_sae.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.1/PKG-INFO` & `sae_lens-3.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 3.2.1
+Version: 3.2.2
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

