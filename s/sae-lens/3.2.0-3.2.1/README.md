# Comparing `tmp/sae_lens-3.2.0.tar.gz` & `tmp/sae_lens-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-3.2.0.tar", max compression
+gzip compressed data, was "sae_lens-3.2.1.tar", max compression
```

## Comparing `sae_lens-3.2.0.tar` & `sae_lens-3.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-05-30 14:51:25.087422 sae_lens-3.2.0/LICENSE
--rw-r--r--   0        0        0     3381 2024-05-30 14:51:25.087422 sae_lens-3.2.0/README.md
--rw-r--r--   0        0        0     2068 2024-05-30 14:51:26.511422 sae_lens-3.2.0/pyproject.toml
--rw-r--r--   0        0        0      898 2024-05-30 14:51:26.507423 sae_lens-3.2.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0     3320 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    12561 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/analysis/hooked_sae_transformer.py
--rw-r--r--   0        0        0    17062 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20406 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     4052 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/batching.py
--rw-r--r--   0        0        0     6047 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/cache_activations_runner.py
--rw-r--r--   0        0        0    24486 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/config.py
--rw-r--r--   0        0        0    16161 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/dashboard_runner.py
--rw-r--r--   0        0        0     7966 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/evals.py
--rw-r--r--   0        0        0     1320 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/load_model.py
--rw-r--r--   0        0        0     5383 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/pretokenize_runner.py
--rw-r--r--   0        0        0     4833 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0    14329 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/sae.py
--rw-r--r--   0        0        0     6972 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/sae_training_runner.py
--rw-r--r--   0        0        0        0 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     8087 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     4752 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0     1783 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/toy_model_runner.py
--rw-r--r--   0        0        0        0 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0    21162 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     3779 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     5585 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0    14209 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/training/sae_trainer.py
--rw-r--r--   0        0        0    18456 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0     4850 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/training/train_toy_sae.py
--rw-r--r--   0        0        0    15495 2024-05-30 14:51:25.099423 sae_lens-3.2.0/sae_lens/training/training_sae.py
--rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 sae_lens-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-06-02 21:11:35.509813 sae_lens-3.2.1/LICENSE
+-rw-r--r--   0        0        0     3381 2024-06-02 21:11:35.509813 sae_lens-3.2.1/README.md
+-rw-r--r--   0        0        0     2007 2024-06-02 21:11:36.881817 sae_lens-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0      898 2024-06-02 21:11:36.881817 sae_lens-3.2.1/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0     3320 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    12561 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/hooked_sae_transformer.py
+-rw-r--r--   0        0        0    17062 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20406 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     4052 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/batching.py
+-rw-r--r--   0        0        0     6047 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/cache_activations_runner.py
+-rw-r--r--   0        0        0    24486 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/config.py
+-rw-r--r--   0        0        0    16161 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/dashboard_runner.py
+-rw-r--r--   0        0        0     7966 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/evals.py
+-rw-r--r--   0        0        0     1320 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/load_model.py
+-rw-r--r--   0        0        0     5383 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/pretokenize_runner.py
+-rw-r--r--   0        0        0     4833 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0    14329 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/sae.py
+-rw-r--r--   0        0        0     6972 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/sae_training_runner.py
+-rw-r--r--   0        0        0        0 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     8087 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     4752 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0     1783 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/toy_model_runner.py
+-rw-r--r--   0        0        0        0 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0    21162 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     3779 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     5585 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/optim.py
+-rw-r--r--   0        0        0    14209 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/sae_trainer.py
+-rw-r--r--   0        0        0    18481 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0     4850 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/train_toy_sae.py
+-rw-r--r--   0        0        0    15495 2024-06-02 21:11:35.521813 sae_lens-3.2.1/sae_lens/training/training_sae.py
+-rw-r--r--   0        0        0     4611 1970-01-01 00:00:00.000000 sae_lens-3.2.1/PKG-INFO
```

### Comparing `sae_lens-3.2.0/LICENSE` & `sae_lens-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/README.md` & `sae_lens-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/pyproject.toml` & `sae_lens-3.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 [tool.poetry]
 name = "sae-lens"
-version = "3.2.0"
+version = "3.2.1"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 transformer-lens = "^1.14.0"
 transformers = "^4.38.1"
-jupyter = "^1.0.0"
 plotly = "^5.19.0"
 plotly-express = "^0.4.1"
-nbformat = "^5.9.2"
-ipykernel = "^6.29.2"
 matplotlib = "^3.8.3"
 matplotlib-inline = "^0.1.6"
 datasets = "^2.17.1"
 babe = "^0.0.7"
 nltk = "^3.8.1"
 sae-vis = "^0.2.18"
-mkdocs = "^1.5.3"
-mkdocs-material = "^9.5.15"
-mkdocs-autorefs = "^1.0.1"
-mkdocs-section-index = "^0.3.8"
-mkdocstrings = "^0.24.1"
-mkdocstrings-python = "^1.9.0"
 safetensors = "^0.4.2"
 typer = "^0.12.3"
 mamba-lens = { version = "^0.0.4", optional = true }
 pyzmq = "26.0.0"
 automated-interpretability = "^0.0.3"
 python-dotenv = "^1.0.1"
 pyyaml = "^6.0.1"
@@ -47,14 +38,20 @@
 isort = "5.13.2"
 pyright = "^1.1.351"
 mamba-lens = "^0.0.4"
 ansible-lint = { version = "^24.2.3", markers = "platform_system != 'Windows'" }
 botocore = "^1.34.101"
 boto3 = "^1.34.101"
 docstr-coverage = "^2.3.2"
+mkdocs = "^1.5.3"
+mkdocs-material = "^9.5.15"
+mkdocs-autorefs = "^1.0.1"
+mkdocs-section-index = "^0.3.8"
+mkdocstrings = "^0.24.1"
+mkdocstrings-python = "^1.9.0"
 
 [tool.poetry.extras]
 mamba = ["mamba-lens"]
 
 
 [tool.isort]
 profile = "black"
```

### Comparing `sae_lens-3.2.0/sae_lens/__init__.py` & `sae_lens-3.2.1/sae_lens/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.2.0"
+__version__ = "3.2.1"
 
 
 from .analysis.hooked_sae_transformer import HookedSAETransformer
 from .cache_activations_runner import CacheActivationsRunner
 from .config import (
     CacheActivationsRunnerConfig,
     LanguageModelSAERunnerConfig,
```

### Comparing `sae_lens-3.2.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-3.2.1/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/analysis/hooked_sae_transformer.py` & `sae_lens-3.2.1/sae_lens/analysis/hooked_sae_transformer.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-3.2.1/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-3.2.1/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/analysis/tsea.py` & `sae_lens-3.2.1/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/batching.py` & `sae_lens-3.2.1/sae_lens/batching.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/cache_activations_runner.py` & `sae_lens-3.2.1/sae_lens/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/config.py` & `sae_lens-3.2.1/sae_lens/config.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/dashboard_runner.py` & `sae_lens-3.2.1/sae_lens/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/evals.py` & `sae_lens-3.2.1/sae_lens/evals.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/load_model.py` & `sae_lens-3.2.1/sae_lens/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/pretokenize_runner.py` & `sae_lens-3.2.1/sae_lens/pretokenize_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/pretrained_saes.yaml` & `sae_lens-3.2.1/sae_lens/pretrained_saes.yaml`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/sae.py` & `sae_lens-3.2.1/sae_lens/sae.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/sae_training_runner.py` & `sae_lens-3.2.1/sae_lens/sae_training_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/toolkit/pretrained_sae_loaders.py` & `sae_lens-3.2.1/sae_lens/toolkit/pretrained_sae_loaders.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-3.2.1/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-3.2.1/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/toy_model_runner.py` & `sae_lens-3.2.1/sae_lens/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/training/activations_store.py` & `sae_lens-3.2.1/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/training/geometric_median.py` & `sae_lens-3.2.1/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/training/optim.py` & `sae_lens-3.2.1/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/training/sae_trainer.py` & `sae_lens-3.2.1/sae_lens/training/sae_trainer.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/training/toy_models.py` & `sae_lens-3.2.1/sae_lens/training/toy_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from dataclasses import dataclass
 from typing import Any, Callable, List, Optional, Tuple, Union, cast
 
 import einops
 import numpy as np
 import torch
 import torch as t
-from IPython.display import clear_output
 from jaxtyping import Float
 from matplotlib import pyplot as plt
 from matplotlib.animation import FuncAnimation
 from matplotlib.widgets import Slider  # , Button
 from torch import Tensor, nn
 from torch.nn import functional as F
 from tqdm import tqdm
@@ -473,14 +472,16 @@
             fig, cast(Any, update), frames=n_timesteps, interval=0.04, repeat=False
         )
         ani.save(save, writer="pillow", fps=25)
     elif colab:
         ani = FuncAnimation(
             fig, cast(Any, update), frames=n_timesteps, interval=0.04, repeat=False
         )
+        from IPython.display import clear_output  # type: ignore
+
         clear_output()
         return ani
 
 
 def parse_colors_for_superposition_plot(
     colors: Optional[Union[Tuple[int, int], List[str], Tensor]],
     n_feats: int,
```

### Comparing `sae_lens-3.2.0/sae_lens/training/train_toy_sae.py` & `sae_lens-3.2.1/sae_lens/training/train_toy_sae.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/sae_lens/training/training_sae.py` & `sae_lens-3.2.1/sae_lens/training/training_sae.py`

 * *Files identical despite different names*

### Comparing `sae_lens-3.2.0/PKG-INFO` & `sae_lens-3.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 3.2.0
+Version: 3.2.1
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: mamba
 Requires-Dist: automated-interpretability (>=0.0.3,<0.0.4)
 Requires-Dist: babe (>=0.0.7,<0.0.8)
 Requires-Dist: datasets (>=2.17.1,<3.0.0)
-Requires-Dist: ipykernel (>=6.29.2,<7.0.0)
-Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: mamba-lens (>=0.0.4,<0.0.5) ; extra == "mamba"
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: matplotlib-inline (>=0.1.6,<0.2.0)
-Requires-Dist: mkdocs (>=1.5.3,<2.0.0)
-Requires-Dist: mkdocs-autorefs (>=1.0.1,<2.0.0)
-Requires-Dist: mkdocs-material (>=9.5.15,<10.0.0)
-Requires-Dist: mkdocs-section-index (>=0.3.8,<0.4.0)
-Requires-Dist: mkdocstrings (>=0.24.1,<0.25.0)
-Requires-Dist: mkdocstrings-python (>=1.9.0,<2.0.0)
-Requires-Dist: nbformat (>=5.9.2,<6.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: plotly (>=5.19.0,<6.0.0)
 Requires-Dist: plotly-express (>=0.4.1,<0.5.0)
 Requires-Dist: pytest-profiling (>=1.7.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: pyzmq (==26.0.0)
```

