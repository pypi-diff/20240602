# Comparing `tmp/cmn_ai-0.0.1.tar.gz` & `tmp/cmn_ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmn_ai-0.0.1.tar", max compression
+gzip compressed data, was "cmn_ai-0.0.2.tar", max compression
```

## Comparing `cmn_ai-0.0.1.tar` & `cmn_ai-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/LICENSE
--rw-r--r--   0        0        0     1429 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/README.md
--rw-r--r--   0        0        0       29 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/callbacks/__init__.py
--rw-r--r--   0        0        0     2563 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/callbacks/core.py
--rw-r--r--   0        0        0     8199 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/callbacks/hook.py
--rw-r--r--   0        0        0     3277 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/callbacks/schedule.py
--rw-r--r--   0        0        0    14489 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/callbacks/training.py
--rw-r--r--   0        0        0    14314 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/learner.py
--rw-r--r--   0        0        0     2645 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/losses.py
--rw-r--r--   0        0        0     5012 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/plot.py
--rw-r--r--   0        0        0        0 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/tabular/__init__.py
--rw-r--r--   0        0        0     5752 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/tabular/eda.py
--rw-r--r--   0        0        0     3984 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/tabular/preprocessing.py
--rw-r--r--   0        0        0        0 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/text/__init__.py
--rw-r--r--   0        0        0     1688 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/text/data.py
--rw-r--r--   0        0        0        0 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/utils/__init__.py
--rw-r--r--   0        0        0    14492 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/utils/data.py
--rw-r--r--   0        0        0     1542 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/utils/processors.py
--rw-r--r--   0        0        0     4457 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/utils/utils.py
--rw-r--r--   0        0        0        0 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/vision/__init__.py
--rw-r--r--   0        0        0     1577 2023-05-19 17:45:55.092238 cmn_ai-0.0.1/cmn_ai/vision/data.py
--rw-r--r--   0        0        0     1252 2023-05-19 17:45:55.096238 cmn_ai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2314 1970-01-01 00:00:00.000000 cmn_ai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2019 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/README.md
+-rw-r--r--   0        0        0       29 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/callbacks/__init__.py
+-rw-r--r--   0        0        0     2635 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/callbacks/core.py
+-rw-r--r--   0        0        0     9206 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/callbacks/hook.py
+-rw-r--r--   0        0        0     4879 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/callbacks/schedule.py
+-rw-r--r--   0        0        0    17295 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/callbacks/training.py
+-rw-r--r--   0        0        0    17037 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/learner.py
+-rw-r--r--   0        0        0     2689 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/losses.py
+-rw-r--r--   0        0        0     4945 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/plot.py
+-rw-r--r--   0        0        0        0 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/tabular/__init__.py
+-rw-r--r--   0        0        0     5762 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/tabular/eda.py
+-rw-r--r--   0        0        0     3985 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/tabular/preprocessing.py
+-rw-r--r--   0        0        0       27 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/text/__init__.py
+-rw-r--r--   0        0        0     1678 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/text/data.py
+-rw-r--r--   0        0        0        0 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/utils/__init__.py
+-rw-r--r--   0        0        0    18263 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/utils/data.py
+-rw-r--r--   0        0        0     2595 2024-06-02 00:41:07.847997 cmn_ai-0.0.2/cmn_ai/utils/processors.py
+-rw-r--r--   0        0        0     4450 2024-06-02 00:41:07.851997 cmn_ai-0.0.2/cmn_ai/utils/utils.py
+-rw-r--r--   0        0        0       60 2024-06-02 00:41:07.851997 cmn_ai-0.0.2/cmn_ai/vision/__init__.py
+-rw-r--r--   0        0        0      945 2024-06-02 00:41:07.851997 cmn_ai-0.0.2/cmn_ai/vision/core.py
+-rw-r--r--   0        0        0     1506 2024-06-02 00:41:07.851997 cmn_ai-0.0.2/cmn_ai/vision/data.py
+-rw-r--r--   0        0        0     1270 2024-06-02 00:41:07.851997 cmn_ai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2992 1970-01-01 00:00:00.000000 cmn_ai-0.0.2/PKG-INFO
```

### Comparing `cmn_ai-0.0.1/LICENSE` & `cmn_ai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmn_ai-0.0.1/README.md` & `cmn_ai-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,50 @@
 
 I am a big believer in **Boyd's Law**, which states that _speed of iteration beats quality of iteration_. Following this principle, I created `cmn_ai` to incorporate the most common tasks we encounter in ML/AI from data exploration to model development and training. Additionally, I baked into it some of the best practices I learned in my career so I don't have to repeat myself on every project I work on.
 
 It is worth noting that the majority of the DL code such as [`Learner`](cmn_ai/learner.py) and callbacks assume that [`pytorch`](https://pytorch.org/) is used as the underlying DL library. Also, tabular data preprocessors/models are compatible with [`sklearn`](https://github.com/scikit-learn/scikit-learn) so they can be used easily with its `Pipeline` or `ColumnTransformer`.
 
 Given the nature of the progress in ML/AI, I will always keep adding more functionalities as time passes.
 
+## Installation
+
+The easiest way to install `cmn_ai` is by using `pip`:
+
+```sh
+pip install cmn-ai
+```
+
+## Documentation
+
+The official documentation is hosted on https://imaddabbura.github.io/cmn_ai/.
+
+## Development setup
+
+The fastest way to setup the development environment is to use `poetry`. You can install `poetry` using `pip` (or `conda`).
+
+```sh
+pip install poetry
+```
+
+Then install `cmn_ai` from source as follows:
+
+```sh
+git clone https://github.com/ImadDabbura/cmn_ai
+cd cmn_ai
+poetry install
+```
+
+## Tests
+
+To run tests, run the following command:
+
+```sh
+poetry run pytest
+```
+
 ## Contributing
 
 `cmn_ai` is not open now for contribution because there are some infrastructure work I need to finish to make it ready for more contributors.
 
 ## License
 
 `cmn_ai` has Apache License, as found in the [LICENCE](LICENSE) file.
```

### Comparing `cmn_ai-0.0.1/cmn_ai/callbacks/core.py` & `cmn_ai-0.0.2/cmn_ai/callbacks/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,90 @@
 """
 The main module that has the definition of the `Callback` base class as
 well as all the Exceptions that a callback may raise.
 """
+
 import re
 from typing import Any
 
 
 class CancelFitException(Exception):
-    """Stop training and move to after_fit."""
+    """Stop training and move to `after_fit`."""
 
 
 class CancelEpochException(Exception):
-    """Stop current epoch and move to after_epoch."""
+    """Stop current epoch and move to `after_epoch`."""
 
 
 class CancelTrainException(Exception):
-    """Stop training current epoch and move to after_train."""
+    """Stop training current epoch and move to `after_train`."""
 
 
-class CancelValidException(Exception):
-    """Stop validation phase and move after_validate."""
+class CancelValidateException(Exception):
+    """Stop validation phase and move to `after_validate`."""
 
 
 class CancelBatchException(Exception):
-    """Stop current batch and move to after_batch."""
+    """Stop current batch and move to `after_batch`."""
 
 
 class CancelStepException(Exception):
-    """Skip stepping the optimizer."""
+    """Skip stepping the optimizer and move to `after_step`."""
 
 
 class CancelBackwardException(Exception):
-    """Skip the backward pass and move to after_backward."""
+    """Skip the backward pass and move to `after_backward`."""
 
 
 class Callback:
     """Base class for all callbacks."""
 
     order: int = 0
 
     def set_learner(self, learner) -> None:
         """
-        Set the learner as an attribute so that callbacks can access learner's
-        attributes without the need to pass `learner` for every single method
-        in every callback.
+        Set the learner as an attribute so that callbacks can access
+        learner's attributes without the need to pass `learner` for
+        every single method in every callback.
 
         Parameters
         ----------
         learner : Learner
-            Learner that the callback will be called when some events happens.
+            Learner that the callback will be called when some events
+            happens.
         """
         self.learner = learner
 
     def __getattr__(self, k) -> Any:
         """
-        This would allow us to use `self.obj` instead of `self.learner.obj`
-        when we know `obj` is in learner because it will only be called when
-        `getattribute` returns `AttributeError`.
+        This would allow us to use `self.obj` instead of
+        `self.learner.obj` when we know `obj` is in learner because it
+        will only be called when `getattribute` returns `AttributeError`.
         """
         return getattr(self.learner, k)
 
     @property
     def name(self) -> str:
         """
-        Returns the name of the callback after removing the word `callback`
-        and then convert it to snake (split words by underscores).
+        Returns the name of the callback after removing the word
+        `callback` and then convert it to snake (split words by
+        underscores).
         """
         name = re.sub(r"Callback$", "", self.__class__.__name__)
         return Callback.camel2snake(name or "callback")
 
     def __call__(self, event_nm: str) -> Any | None:
         method = getattr(self, event_nm, None)
         if method is not None:
             method()
 
     @staticmethod
     def camel2snake(name: str) -> str:
         """
-        Convert name of callback by inserting underscores between small and capital
-        letters. For example, `TestCallback` becomes `test_callback`.
+        Convert name of callback by inserting underscores between small
+        and capital letters. For example, `TestCallback` becomes
+        `test_callback`.
         """
         pattern1 = re.compile("(.)([A-Z][a-z]+)")
         pattern2 = re.compile("([a-z0-9])([A-Z])")
         name = re.sub(pattern1, r"\1_\2", name)
         return re.sub(pattern2, r"\1_\2", name).lower()
```

### Comparing `cmn_ai-0.0.1/cmn_ai/callbacks/hook.py` & `cmn_ai-0.0.2/cmn_ai/callbacks/hook.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 """
-Hooks are very useful to inspect what is happening during the forward and
-backward passes such as computing stats of the activations and gradients.
+Hooks are very useful to inspect what is happening during the forward
+and backward passes such as computing stats of the activations and
+gradients.
 
 The module contains the following classes:
 
 - `Hook`: Registers forward or backward hook for a single module
 - `Hooks`: Registers forward or backward hook for multiple modules
 - `HooksCallback`: Use callbacks to register and manage hooks
-- `ActivationStats`: Computes means/stds for either activation or gradients
-    and plot the computed stats.
+- `ActivationStats`: Computes means/stds for either activation or
+    gradients and plot the computed stats.
 """
+
 from __future__ import annotations
 
 from functools import partial
 from typing import Callable, Iterable, Iterator
 
-import fastcore.all as fc
 import matplotlib.pyplot as plt
 import torch
 import torch.nn as nn
-from matplotlib.image import AxesImage
 from torch import Tensor
 
 from ..plot import get_grid, show_image
+from ..utils.utils import listify
 from .core import Callback
 
 
 class Hook:
     """
     Register either a forward or a backward hook on the module.
-
-    Parameters
-    ----------
-    module : nn.Module
-        The module to register the hook on.
-    func : Callable
-        The hook to be registered.
-    is_forward : bool, default=True
-        Whether to register `func` as a forward or backward hook.
     """
 
     def __init__(
         self,
         module: nn.Module,
         func: Callable,
         is_forward: bool = True,
         **kwargs,
     ) -> None:
+        """
+        Parameters
+        ----------
+        module : nn.Module
+            The module to register the hook on.
+        func : Callable
+            The hook to be registered.
+        is_forward : bool, default=True
+            Whether to register `func` as a forward or backward hook.
+        """
         self.is_forward = is_forward
         if self.is_forward:
             self.hook = module.register_forward_hook(
                 partial(func, self, **kwargs)
             )
         else:
             self.hook = module.register_backward_hook(
@@ -67,36 +69,35 @@
         self.hook.remove()
 
     def __del__(self) -> None:
         self.remove()
 
 
 class Hooks:
-    """"""
-
     """
     Register hooks on all modules.
-
-    Parameters
-    ----------
-    modules : nn.Module or Iterable[nn.Module]
-        The module to register the hook on.
-    func : Callable
-        The hook to be registered.
-    is_forward : bool, default=True
-        Whether to register `func` as a forward or backward hook.
     """
 
     def __init__(
         self,
-        modules: nn.Module | Iterable[nn.Module],
+        modules: Iterable[nn.Module],
         func: Callable,
         is_forward: bool = True,
         **kwargs,
     ) -> None:
+        """
+        Parameters
+        ----------
+        modules : Iterable[nn.Module]
+            The module to register the hook on.
+        func : Callable
+            The hook to be registered.
+        is_forward : bool, default=True
+            Whether to register `func` as a forward or backward hook.
+        """
         self.hooks = [
             Hook(module, func, is_forward, **kwargs) for module in modules
         ]
 
     def __getitem__(self, idx) -> Hook:
         return self.hooks[idx]
 
@@ -180,47 +181,48 @@
     """
     res = torch.stack(hook.stats[2]).t().float()
     return res[slice(*bins_range)].sum(0) / res.sum(0)
 
 
 class HooksCallback(Callback):
     """
-    Base call to run hooks on modules as a callback.
-
-    Parameters
-    ----------
-    hookfunc : Callable
-        The hook to be registered.
-    on_train : bool, default=True
-        Whether to run the hook on modules during training.
-    on_valid : bool, default=False
-        Whether to run the hook on modules during validation.
-    modules : nn.Module | Iterable[nn.Module] | None, default=None
-        Modules to register the hook on. Default to all modules.
-    is_forward : bool, default=True
-        Whether to register `func` as a forward or backward hook.
+    Base class to run hooks on modules as a callback.
     """
 
     def __init__(
         self,
         hookfunc: Callable,
         on_train: bool = True,
         on_valid: bool = False,
         modules: nn.Module | Iterable[nn.Module] | None = None,
         is_forward: bool = True,
     ) -> None:
+        """
+        Parameters
+        ----------
+        hookfunc : Callable
+            The hook to be registered.
+        on_train : bool, default=True
+            Whether to run the hook on modules during training.
+        on_valid : bool, default=False
+            Whether to run the hook on modules during validation.
+        modules : nn.Module | Iterable[nn.Module] | None, default=None
+            Modules to register the hook on. Default to all modules.
+        is_forward : bool, default=True
+            Whether to register `func` as a forward or backward hook.
+        """
         self.hookfunc = hookfunc
         self.on_train = on_train
         self.on_valid = on_valid
-        self.modules = modules
+        self.modules = listify(modules)
         self.is_forward = is_forward
 
     def before_fit(self) -> None:
-        if self.modules is None:
-            self.modules = self.model.modules()
+        if not self.modules:
+            self.modules = self.model.children()
         self.hooks = Hooks(self.modules, self._hookfunc, self.is_forward)
 
     def _hookfunc(self, *args, **kwargs):
         if (self.on_train and self.training) or (
             self.on_valid and not self.training
         ):
             self.hookfunc(*args, **kwargs)
@@ -235,57 +237,86 @@
         return len(self.hooks)
 
 
 class ActivationStats(HooksCallback):
     """
     Plot the means, std, histogram, and dead activations of all modules'
     activations if `is_forward` else gradients.
-
-    Parameters
-    ----------
-    modules : nn.Module | Iterable[nn.Module] | None, default=None
-        Modules to register the hook on. Default to all modules.
-    is_forward : bool, default=True
-        Whether to register `func` as a forward or backward hook.
-    bins : int, default=40
-        Number of histogram bins.
-    bins_range : Iterable, default=(0, 10)
-        lower/upper end of the histogram's bins range.
     """
 
     def __init__(
         self,
         modules: nn.Module | Iterable[nn.Module] | None = None,
         is_forward: bool = True,
         bins: int = 40,
         bins_range: list | tuple = (0, 10),
     ) -> None:
-        self.bins_range = bins_range
+        """
+        Parameters
+        ----------
+        modules : nn.Module | Iterable[nn.Module] | None, default=None
+            Modules to register the hook on. Default to all modules.
+        is_forward : bool, default=True
+            Whether to register `func` as a forward or backward hook.
+        bins : int, default=40
+            Number of histogram bins.
+        bins_range : Iterable, default=(0, 10)
+            Lower/Upper end of the histogram's bins range.
+        """
         super().__init__(
             partial(compute_stats, bins=bins, bins_range=bins_range),
-            is_forward=is_forward,
             modules=modules,
+            is_forward=is_forward,
         )
 
     def plot_hist(self, figsize=(11, 5)) -> None:
+        """
+        Plot histogram of activations/gradients as a heatmap.
+
+        Parameters
+        ----------
+        figsize : tuple, de
+            Width, height of the heatmap figure.
+        """
         _, axes = get_grid(len(self), figsize=figsize)
         for ax, h in zip(axes.flat, self):
-            show_image(get_hist(h), ax, origin="lower")
+            show_image(get_hist(h), ax, origin="lower", cmap="viridis")
 
-    def dead_chart(self, figsize=(11, 5)) -> None:
+    def dead_chart(self, bins_range, figsize=(11, 5)) -> None:
+        """
+        Plot a line chart of the "dead" activations percentage from all
+        activations.
+
+        Parameters
+        ----------
+        bins_range : list | tuple
+            Bins range around zero. Bins that are considered dead
+            activations/gradients.
+        figsize : tuple, default=(11, 5)
+            Width, height of the figure.
+        """
         _, axes = get_grid(len(self), figsize=figsize)
         for ax, h in zip(axes.flatten(), self):
-            ax.plot(get_min(h, self.bins_range))
+            ax.plot(get_min(h, bins_range))
             ax.set_ylim(0, 1)
 
     def plot_stats(self, figsize=(10, 4)) -> None:
+        """
+        Plot means of standard deviation of activations/gradients for
+        each layer that has a registered hook.
+
+        Parameters
+        ----------
+        figsize : tuple, default=(10, 4)
+            Width, height of the figure.
+        """
         _, axes = plt.subplots(1, 2, figsize=figsize)
         for h in self:
             axes[0].plot(h.stats[0])
             axes[1].plot(h.stats[1])
         axes[0].set_title(
             f"Means of {'activations' if self.is_forward else 'gradients'}"
         )
         axes[1].set_title(
             f"Stdevs of {'activations' if self.is_forward else 'gradients'}"
         )
-        plt.legend(fc.L.range(self))
+        plt.legend(range(len(self)))
```

### Comparing `cmn_ai-0.0.1/cmn_ai/callbacks/training.py` & `cmn_ai-0.0.2/cmn_ai/callbacks/training.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,53 +15,62 @@
 CancelBatchException
     Stop current batch and move to after_batch.
 CancelStepException
     Skip stepping the optimizer.
 CancelBackwardException
     Skip the backward pass and move to after_backward.
 """
+
 import tempfile
 import time
 from copy import copy
 from functools import partial
 from pathlib import Path
 from typing import Callable, Iterable
 
 import fastcore.all as fc
 import matplotlib.pyplot as plt
+import seaborn as sns
 import torch
 from fastprogress.fastprogress import format_time, master_bar, progress_bar
 from torch.optim.lr_scheduler import ExponentialLR
 from torcheval.metrics import Mean
 
 from ..losses import NoneReduce, reduce_loss
 from ..plot import get_grid
 from ..utils.data import default_device, to_cpu, to_device
 from ..utils.utils import listify
-from .core import Callback, CancelFitException, CancelValidException
-from .schedule import exp_sched
+from .core import Callback, CancelFitException, CancelValidateException
 
 
 class DeviceCallback(Callback):
     """Move batch and model to `device`."""
 
-    def __init__(self, device: torch.device = default_device) -> None:
+    def __init__(self, device: str | torch.device = default_device) -> None:
+        """
+        Parameters
+        ----------
+        device : str | torch.device
+            Device to copy batch to.
+        """
         self.device = device
 
     def before_fit(self) -> None:
         self.model.to(self.device)
 
     def before_batch(self) -> None:
         self.learner.batch = to_device(self.batch, self.device)
+        self.learner.xb = self.batch[: self.n_inp]
+        self.learner.yb = self.batch[self.n_inp :]
 
 
 class TrainEvalCallback(Callback):
     """
-    Tracks the number of iterations and epoch done and set training and eval
-    modes.
+    Tracks the number of iterations, percentage of training, and set
+    training and eval modes.
     """
 
     order = -10
 
     def before_fit(self) -> None:
         self.learner.n_iters = 0
         self.learner.pct_train = 0
@@ -79,43 +88,44 @@
     def before_validate(self) -> None:
         self.model.eval()
         self.learner.training = False
 
 
 class ProgressCallback(Callback):
     """
-    Track progress of training using progress bar as well as to plot losses
-    (train and valid), which allows us to have live feedback of the model's
-    performance while it is still training.
-
-    Parameters
-    ----------
-    plot : bool, default=True
-        Whether to plot train/valid losses during training.
+    Track progress of training using progress bar as well as to plot
+    losses (train and valid), which allows us to have live feedback of
+    the model's performance while it is still training.
     """
 
     order = -20
 
     def __init__(self, plot: bool = True) -> None:
+        """
+        Parameters
+        ----------
+        plot : bool, default=True
+            Whether to plot train/valid losses during training.
+        """
         self.plot = plot
-        self.train_losses = []
-        self.valid_losses = []
 
     def before_fit(self) -> None:
+        self.train_losses = []
+        self.valid_losses = []
         self.learner.epochs = self.mbar = master_bar(range(self.n_epochs))
         self.mbar.on_iter_begin()
         # Overwrite default learner logger
         self.learner.logger = partial(self.mbar.write, table=True)
 
     def after_fit(self) -> None:
         self.mbar.on_iter_end()
 
     def after_batch(self):
         self.pb.update(self.iter)
-        self.pb.comment = f"{self.loss:.3f}"
+        self.pb.comment = f"{self.loss:.3f}"  # noqa: E231
         if self.plot and hasattr(self.learner, "metrics") and self.training:
             self.train_losses.append(self.loss.item())
             if self.valid_losses:
                 self.mbar.update_graph(
                     [
                         [fc.L.range(self.train_losses), self.train_losses],
                         [
@@ -160,22 +170,23 @@
     def set_pb(self) -> None:
         self.pb = progress_bar(self.dl, leave=False, parent=self.mbar)
         self.mbar.update(self.epoch)
 
 
 class Recorder(Callback):
     """
-    Keep track of losses and learning rates as training progress so we can
-    plot them later.
+    Keep track of losses and `params` of the optimizer such as
+    learning rates as training progress so we can plot them later.
     """
 
     order = 50
 
     def __init__(self, *params: tuple[str]) -> None:
         self.params = listify(params)
+        sns.set()
 
     def before_fit(self) -> None:
         self.params_records = {
             params: [[] for _ in self.opt.param_groups]
             for params in self.params
         }
         self.losses = []
@@ -189,53 +200,58 @@
                     param_record.append(pg[param])
             self.losses.append(to_cpu(self.loss))
 
     def plot_params(
         self,
         params: str | Iterable[str] = "lr",
         pgid: int = -1,
-        skip_last: int = 0,
         figsize: tuple = (8, 6),
     ) -> None:
         """
         Plot all `params` values across all iterations of training.
         """
         params = listify(params)
         _, axes = get_grid(len(params), figsize=figsize)
         for (
             ax,
             param,
         ) in zip(axes.flatten(), params):
             ax.plot(self.params_records[param][pgid], label=param)
             ax.legend()
+        plt.xlabel("Iteration")
 
     def plot_loss(self, skip_last: int = 0) -> None:
         """
         Plot losses, optionally skip last `skip_last` losses.
         """
         n = len(self.losses) - skip_last
         plt.plot(self.losses[:n])
+        plt.xlabel("Iteration")
+        plt.ylabel("Loss")
 
     def plot(self, pgid: int = -1, skip_last: int = 0) -> None:
         """
         Plot loss vs lr (log-scale) across all iterations of training.
         """
         n = len(self.losses) - skip_last
         plt.xscale("log")
         plt.plot(
             self.params_records["lr"][pgid][:n],
             self.losses[:n],
         )
+        plt.xlabel("Learning rate")
+        plt.ylabel("Loss")
 
 
 class ModelResetter(Callback):
     """
-    Reset model's parameters. This is very useful in the context of NLP since
-    we always reset hidden state. The assumption here is that `model` has a
-    `reset` method that knows which parameters to reset and how.
+    Reset model's parameters. This is very useful in the context of NLP
+    since we always reset hidden state. The assumption here is that
+    `model` has a `reset` method that knows which parameters to reset
+    and how.
     """
 
     def before_train(self) -> None:
         self.model.reset()
 
     def before_validate(self) -> None:
         self.model.reset()
@@ -245,116 +261,167 @@
 
 
 # TODO: Change loss to smooth_loss
 class LRFinder(Callback):
     """
     Try different learning rates using exponential schedule to help pick
     the best learning rate following [Cyclical Learning Rates for Training
-    Neural Networks](https://arxiv.org/pdf/1506.01186.pdf). When done, plot
-    learning rate vs loss.
-
-    Parameters
-    ----------
-    start_lr : float, default=1e-7
-        Start learning rate.
-    end_lr : float, default=10.0
-        Last learning rate in the schedule.
-    num_iter : int, default=100
-        Number of iterations to run the training.
-    stop_div : bool, default
-        Whether to stop training if loss diverges (loss > 4 * best_loss).
-    max_mult : int, default=4
-        Divergence threshold. If loss >= max_mult * minimum loss, stop
-        training.
+    Neural Networks](https://arxiv.org/pdf/1506.01186.pdf). When done,
+    plot learning rate vs loss.
     """
 
     def __init__(
         self,
         gamma: int = 1.3,
         num_iter: int = 100,
         stop_div: bool = True,
         max_mult: int = 4,
     ) -> None:
+        """
+        Parameters
+        ----------
+        end_lr : float, default=10.0
+            Last learning rate in the schedule.
+        num_iter : int, default=100
+            Number of iterations to run the training.
+        stop_div : bool, default
+            Whether to stop training if loss diverges (loss > 4 * best_loss).
+        max_mult : int, default=4
+            Divergence threshold. If loss >= max_mult * minimum loss, stop
+            training.
+        """
         self.gamma = gamma
         self.num_iter = num_iter
         self.stop_div = stop_div
         self.max_mult = max_mult
 
     def before_fit(self) -> None:
         self.scheduler = ExponentialLR(self.opt, self.gamma)
-        path = self.path / self.model_dir
-        path.mkdir(parents=True, exist_ok=True)
-        self.tmp_d = tempfile.TemporaryDirectory(dir=path)
+        self.model_dir_path.mkdir(parents=True, exist_ok=True)
+        self.tmp_d = tempfile.TemporaryDirectory(dir=self.model_dir_path)
         self.tmp_p = Path(self.tmp_d.name).stem
-        self.save_model(path / self.tmp_p / "_tmp.pth", with_opt=True)
+        self.save_model(
+            self.model_dir_path / self.tmp_p / "_tmp.pth", with_opt=True
+        )
         self.best_loss = float("inf")
 
     def after_batch(self) -> None:
         if self.loss < self.best_loss:
             self.best_loss = self.loss
         if self.loss > self.max_mult * self.best_loss and self.stop_div:
             raise CancelFitException()
         if self.n_iters >= self.num_iter:
             raise CancelFitException()
         self.scheduler.step()
 
     def before_validate(self) -> None:
-        raise CancelValidException()
+        raise CancelValidateException()
 
     def after_fit(self) -> None:
         self.opt.zero_grad()
-        tmp_f = self.path / self.model_dir / self.tmp_p / "_tmp.pth"
+        tmp_f = self.model_dir_path / self.tmp_p / "_tmp.pth"
         if tmp_f.exists():
             self.load_model(tmp_f, with_opt=True)
             self.tmp_d.cleanup()
+        self.recorder.plot()
 
 
 class BatchTransform(Callback):
     """
-    Transform X as a batch using `tfm` callable before every batch.
+    Transform batch using `tfm` callable before every batch.
     Apply transformation `tfm` on the batch as a whole.
-
-    Parameters
-    ----------
-    tfm : Callback
-        Transformation to apply on the batch.
-    on_train : bool, default=True
-        Whether to apply the transformation during training.
-    on_valid : bool, default=True
-        Whether to apply the transformation during validation.
     """
 
-    order = 2
+    # So transforms run on the device
+    order = DeviceCallback.order + 1
 
     def __init__(
         self, tfm: Callback, on_train: bool = True, on_valid: bool = True
     ) -> None:
+        """
+        Parameters
+        ----------
+        tfm : Callback
+            Transformation to apply on the batch.
+        on_train : bool, default=True
+            Whether to apply the transformation during training.
+        on_valid : bool, default=True
+            Whether to apply the transformation during validation.
+        """
         self.tfm = tfm
         self.on_train = on_train
         self.on_valid = on_valid
 
     def before_batch(self) -> None:
         if (self.on_train and self.training) or (
             self.on_valid and not self.training
         ):
             self.learner.batch = self.tfm(self.batch)
+            self.learner.xb = self.batch[: self.n_inp]
+            self.learner.yb = self.batch[self.n_inp :]
 
 
-class SingleBatchCB(Callback):
+class BatchTransformX(Callback):
     """
-    Run 1 training/validation batch and stop by raising `CancelFitException`.
-    Useful for debugging or want to check few parameters after 1 batch.
+    Transform X using `tfm` callable before every batch.
+    Apply transformation `tfm` on the batch as a whole.
+    """
+
+    order = DeviceCallback.order + 1
+
+    def __init__(
+        self, tfm: Callback, on_train: bool = True, on_valid: bool = True
+    ) -> None:
+        """
+        Parameters
+        ----------
+        tfm : Callback
+            Transformation to apply on the batch.
+        on_train : bool, default=True
+            Whether to apply the transformation during training.
+        on_valid : bool, default=True
+            Whether to apply the transformation during validation.
+        """
+        self.tfm = tfm
+        self.on_train = on_train
+        self.on_valid = on_valid
+
+    def before_batch(self) -> None:
+        if (self.on_train and self.training) or (
+            self.on_valid and not self.training
+        ):
+            self.learner.xb = self.tfm(self.xb)
+
+
+class SingleBatchCallback(Callback):
+    """
+    Run 1 training/validation batch and stop by raising
+    `CancelFitException`. Useful for debugging or want to check few
+    parameters after 1 batch.
     """
 
     order = 1
 
     def after_batch(self) -> None:
         raise CancelFitException()
 
 
+class SingleBatchForwardCallback(Callback):
+    """
+    Run 1 training/validation batch and stop after forward pass (after
+    computing loss) by raising `CancelFitException`. Useful for debugging
+    or want to check few parameters after 1 batch.
+    """
+
+    order = 1
+
+    def after_loss(self) -> None:
+        raise CancelFitException()
+
+
 class MetricsCallback(Callback):
     """
     Compute/update given metrics and log it using `learner` defined logger
     after every `train`/`validate` epoch. Metrics have to implement `reset`
     and `compute` methods. Highly recommended to use metrics from
     `torcheval` package or inherit from its Metrics baseclass for custom
     metrics.
@@ -365,15 +432,15 @@
         for metric in metrics:
             self.metrics[type(metric).__name__] = metric
         self.all_metrics = {"loss": Mean()}
         self.all_metrics.update(copy(self.metrics))
 
     def _compute(self):
         for metric in self.all_metrics.values():
-            self.stats.append(f"{metric.compute():.3f}")
+            self.stats.append(f"{metric.compute():.3f}")  # noqa: E231
         self.stats.append("train" if self.training else "eval")
         self.stats.append(format_time(time.time() - self.start_time))
 
     def _reset(self):
         [metric.reset() for metric in self.all_metrics.values()]
         self.stats = [str(self.epoch + 1)]
         self.start_time = time.time()
@@ -407,29 +474,31 @@
             metric.update(to_cpu(self.preds), to_cpu(*self.yb))
         self.all_metrics["loss"].update(
             to_cpu(self.learner.loss), weight=len(self.learner.xb[0])
         )
 
 
 class Mixup(Callback):
+    """
+    Train the model with a mix of samples from each batch in the training
+    data. Instead of feeding the model with raw data, we use linear
+    combination of the input using `alpha` from beta distribution. This
+    means that the labels would also be the linear combination of the
+    labels and not the original labels. The implementation is largely
+    based on this [paper](https://arxiv.org/abs/1710.09412).
+    """
+
     order = 90
 
     def __init__(self, alpha: float = 0.4) -> None:
         """
-        Train the model with a mix of samples from each batch in the training
-        data. Instead of feeding the model with raw data, we use linear
-        combination of the input using `alpha` from beta distribution. This
-        means that the labels would also be the linear combination of the
-        labels and not the original labels. The implementation is largely
-        based on this [paper](https://arxiv.org/abs/1710.09412).
-
         Parameters
         ----------
         alpha : float, default=0.4
-            Concetration for Beta distribution.
+            Concentration for Beta distribution.
         """
         self.distrib = torch.distributions.beta.Beta(
             torch.tensor([alpha]), torch.tensor([alpha])
         )
 
     def before_fit(self) -> None:
         self.learner.loss_func, self.old_loss_func = (
@@ -437,17 +506,31 @@
             self.learner.loss_func,
         )
 
     def after_fit(self) -> None:
         self.learner.loss_func = self.old_loss_func
 
     def before_batch(self) -> None:
-        λ = self.distrib.sample((len(self.learner.xb),)).to(
-            self.learner.xb[0].device
-        )
+        """
+        Steps taken before passing inputs to the model:
+
+        - Draw from a beta distribution a sample of size of `batch_size`.
+          Each image would have its own `λ`.
+        - To avoid having two images combined together with the same `λ`,
+          we take the max of `λ` and `1 - λ` so even if they were combined
+          together they would lead to a different image.
+        - Shuffle the batch before computing the linear combination.
+        - Change the batch input to be the linear combination of both the
+          original image and the shuffled images.
+
+        The loss would be the linear combination of the loss of the
+        original images with the original target and the shuffled image
+        with the shuffled target weighted by `λ`.
+        """
+        λ = self.distrib.sample((len(self.xb),)).to(self.xb[0].device)
         λ = torch.stack([λ, 1 - λ], dim=1)
         self.λ = λ.max(1)[0].view(-1, 1, 1, 1)
         shuffle = torch.randperm(len(self.xb[0]))
         self.learner.xb = [
             x * self.λ + x[shuffle] * (1 - self.λ) for x in self.xb
         ]
         self.yb1 = [y[shuffle] for y in self.yb]
@@ -458,8 +541,7 @@
         with NoneReduce(self.old_loss_func) as loss_func:
             loss1 = loss_func(pred, yb)
             loss2 = loss_func(pred, *self.yb1)
         loss = loss1 * self.λ + loss2 * (1 - self.λ)
         return reduce_loss(
             loss, getattr(self.old_loss_func, "reduction", "mean")
         )
-
```

### Comparing `cmn_ai-0.0.1/cmn_ai/learner.py` & `cmn_ai-0.0.2/cmn_ai/learner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,87 @@
 """
 `Learner` is a basic class that provides useful functionalities:
 
-1. Tweaking/customization of the training loop using a system of callbacks through Exceptions
-2. Loading/saving model
-3. Fit the model
-4. Get model summary
-5. Learning rate finder
-
-The training loop consists of a minimal set of instructions; looping through the data we:
-
-- compute the output of the model from the input
-- calculate a loss between this output and the desired target
-- compute the gradients of this loss with respect to all the model parameters
-- update the parameters accordingly
-- zero all the gradients
-
-Any tweak of this training loop is defined in a [Callback][cmn_ai.callbacks.core.Callback].
-A callback can implement actions on the following events:
+- Tweaking/customization of the training loop using a system of
+callbacks through Exceptions
+- Loading/saving model
+- Fit the model
+- Get model summary
+- Learning rate finder
+
+The training loop consists of a minimal set of instructions; looping
+through the data we:
+
+- Compute the output of the model from the input
+- Calculate a loss between this output and the desired target
+- Compute the gradients of this loss with respect to model parameters
+- Update the parameters accordingly
+- Zero all the gradients
+
+Any tweak of this training loop is defined in a [Callback]
+[cmn_ai.callbacks.core.Callback]. A callback can implement actions on
+the following events:
 
 - `before_fit`: called before doing anything, ideal for initial setup
-- `before_epoch`: called at the beginning of each epoch, useful for any behavior you need to reset at each epoch
-- `before_train`: called at the beginning of the training part of an epoch
-- `before_batch`: called at the beginning of each batch, just after drawing said batch. It can be used to do any setup necessary for the batch (like hyper-parameter scheduling) or to change the input/target before it goes in the model (change of the input with techniques like mixup for instance)
-- `after_pred`: called after computing the output of the model on the batch. It can be used to change that output before it's fed to the loss
-- `after_loss`: called after the loss has been computed, but before the backward pass. It can be used to add any penalty to the loss (AR or TAR in RNN training for instance)
-- `after_backward`: called after the backward pass, but before the update of the parameters. It can be used to do any change to the gradients before said update (gradient clipping for instance)
-- `after_step`: called after the step and before the gradients are zeroed
-- `after_cancel_batch`: reached immediately after a `CancelBatchException` before proceeding to `after_batch`
-- `after_batch`: called at the end of a batch, for any clean-up before the next one
-- `after_cancel_train`: reached immediately after a `CancelTrainException` before proceeding to `after_train`
+- `before_epoch`: called at the beginning of each epoch, useful for any
+behavior you need to reset at each epoch
+- `before_train`: called at the beginning of the training part of an
+epoch
+- `before_batch`: called at the beginning of each batch, just after
+drawing said batch. It can be used to do any setup necessary for the
+batch (like hyper-parameter scheduling) or to change the input/target
+before it goes in the model (change of the input with techniques like
+mixup for instance)
+- `after_pred`: called after computing the output of the model on the
+batch. It can be used to change that output before it's fed to the loss
+function
+- `after_loss`: called after the loss has been computed, but before the
+backward pass. It can be used to add any penalty to the loss (AR or TAR
+in RNN training for instance)
+- `after_cancel_backward`: reached immediately after
+  [CancelBackwardException][cmn_ai.callbacks.core.CancelBackwardException]
+- `after_backward`: called after the backward pass, but before updating
+the parameters. It can be used to do any change to the
+gradients before any updates (gradient clipping for instance)
+- `after_cancel_step`: reached immediately after
+  [CancelStepException][cmn_ai.callbacks.core.CancelStepException]
+- `after_step`: called after the step and before gradients are zeroed
+- `after_cancel_batch`: reached immediately after
+  [CancelBatchException][cmn_ai.callbacks.core.CancelBatchException]
+before proceeding to `after_batch`
+- `after_batch`: called at the end of a batch, for any clean-up before
+the next one
+- `after_cancel_train`: reached immediately after
+  [CancelTrainException][cmn_ai.callbacks.core.CancelTrainException]
+before proceeding to `after_train`
 - `after_train`: called at the end of the training phase of an epoch
-- `before_validate`: called at the beginning of the validation phase of an epoch, useful for any setup needed specifically for validation
-- `after_cancel_validate`: reached immediately after a `CancelValidateException` before proceeding to `after_validate`
-- `after_validate`: called at the end of the validation part of an epoch
-- `after_cancel_epoch`: reached immediately after a `CancelEpochException` before proceeding to `after_epoch`
-- `after_epoch`: called at the end of an epoch, for any clean-up before the next one
-- `after_cancel_fit`: reached immediately after a `CancelFitException` before proceeding to `after_fit`
-- `after_fit`: called at the end of training, for final clean-up
+- `before_validate`: called at the beginning of the validation phase of
+an epoch, useful for any setup needed specifically for validation
+- `after_cancel_validate`: reached immediately after
+[CancelValidateException][cmn_ai.callbacks.core.CancelValidateException]
+before proceeding to `after_validate`
+- `after_validate`: called at the end of the validation phase of an
+epoch
+- `after_cancel_epoch`: reached immediately after
+  [CancelEpochException][cmn_ai.callbacks.core.CancelEpochException]
+before proceeding to `after_epoch`
+- `after_epoch`: called at the end of an epoch, for any clean-up before
+the next one
+- `after_cancel_fit`: reached immediately after
+  [CancelFitException][cmn_ai.callbacks.core.CancelFitException]
+before proceeding to `after_fit`
+- `after_fit`: called at the end of training, for any final clean-up
 """
+
 from __future__ import annotations
 
 import pickle
 from collections.abc import Callable, Iterable
 from pathlib import Path
 
-import fastcore.all as fc
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as opt
 from torch import tensor
 from torch.utils.data import DataLoader
 from torchinfo import summary
@@ -57,22 +90,23 @@
     Callback,
     CancelBackwardException,
     CancelBatchException,
     CancelEpochException,
     CancelFitException,
     CancelStepException,
     CancelTrainException,
-    CancelValidException,
+    CancelValidateException,
 )
 from .callbacks.training import (
     LRFinder,
     ProgressCallback,
     Recorder,
     TrainEvalCallback,
 )
+from .utils.data import DataLoaders
 from .utils.utils import listify
 
 
 def params_getter(model: nn.Module) -> Iterable[nn.Parameter]:
     """
     Get all parameters of `model` recursively.
 
@@ -92,100 +126,124 @@
 class Learner:
     """
     Learner is a basic class that handles training loop of pytorch model
     and utilize a systems of callbacks that makes training loop very
     customizable and extensible. You just need to provide a list of
     callbacks and callback functions.
 
-    Parameters
+    Attributes
     ----------
     model : nn.Module
-        pytorch's model.
-    dls : Iterable of Dataloaders.
-        train and valid data loaders.
-    n_inp : int, default=1
+        Pytorch's model.
+    dls : DataLoaders
+        Train and valid data loaders.
+    n_inp : int
         Number of inputs to the model.
-    loss_func : Callable, default=`MSE`
+    loss_func : Callable[[tensor, tensor], tensor]
         Loss function.
-    opt_func : Optimizer, default=`SGD`
+    opt_func : opt.Optimizer
         Optimizer function/class.
-    lr : float, default=`1e-2`
+    lr : float
         Learning rate.
-    splitter : Callable, default=`params_getter`
-        Function to split model's parameters into groups, default all
-        parameters belong to 1 group.
-    callbacks : Iterable, default=None
+    splitter : Callable[[nn.Module], Iterable[nn.Parameter]]
+        Function to split model's parameters into groups.
+    path : Path
+        Path to save all artifacts.
+    model_dir_path : Path
+        Model directory path.
+    callbacks : Iterable[Callable] | None, default=None
         Iterable of callbacks of type `Callback`.
-    default_callbacks : bool, default=True
-        Whether to add `TrainEvalCallback`, `ProgressCallback`, and `Recorder`
-        to the list of callbacks.
-
-    Attributes
-    ----------
     logger : Any
-        Logger to log metrics. Default is `print` but is typically modified by
-        callbacks such as `ProgressCallback`.
+        Logger to log metrics. Default is `print` but is typically
+        modified by callbacks such as `ProgressCallback`.
     callbacks: list[Callback]
-        List of all the used callbacks by `learner.`
+        List of all the used callbacks by `learner`. \
+        [`TrainEvalCallback`][cmn_ai.callbacks.training.TrainEvalCallback] is
+        added by `learner`, so no need to add it.
     """
 
     def __init__(
         self,
         model: nn.Module,
-        dls: Iterable[DataLoader],
+        dls: DataLoaders,
         n_inp: int = 1,
         loss_func: Callable[[tensor, tensor], tensor] = F.mse_loss,
         opt_func: opt.Optimizer = opt.SGD,
         lr: float = 1e-2,
-        splitter: Callable = params_getter,
-        path: str = ".",
+        splitter: Callable[
+            [nn.Module], Iterable[nn.Parameter]
+        ] = params_getter,
+        path: str | Path = ".",
         model_dir: str = "models",
         callbacks: Iterable[Callback] | None = None,
-        default_callbacks: bool = True,
     ) -> None:
+        """
+        Parameters
+        ----------
+        model : nn.Module
+            Pytorch's model.
+        dls : DataLoaders
+            Train and valid data loaders.
+        n_inp : int, default=1
+            Number of inputs to the model.
+        loss_func : Callable[[tensor, tensor], tensor],\
+                default=F.mse_loss
+            Loss function.
+        opt_func : opt.Optimizer, default=opt.SGD
+            Optimizer function/class.
+        lr : float, default=`1e-2`
+            Learning rate.
+        splitter : Callable[[nn.Module], Iterable[nn.Parameter]],\
+                default=`params_getter`
+            Function to split model's parameters into groups, default
+            all parameters belong to 1 group.
+        path : str, default="."
+            Path to save all artifacts.
+        model_dir : str, default="models"
+            Model directory name relative to `path`.
+        callbacks : Iterable[Callable] | None, default=None
+            Iterable of callbacks of type `Callback`.
+        """
         self.model = model
         self.dls = dls
         self.n_inp = n_inp
         self.loss_func = loss_func
         self.opt_func = opt_func
         self.opt = None
         self.lr = lr
         self.splitter = splitter
         self.path = Path(path)
-        self.model_dir = Path(model_dir)
+        self.model_dir_path = self.path / Path(model_dir)
         self.logger = print
-        self.callbacks = fc.L()
-        if default_callbacks:
-            callbacks += [
-                TrainEvalCallback(),
-                ProgressCallback(),
-                Recorder("lr"),
-            ]
-        self.add_callbacks(callbacks)
+        self.callbacks = []
+        callbacks = listify(callbacks) + [
+            TrainEvalCallback(),
+        ]
+        self._add_callbacks(callbacks)
 
     def _with_events(self, func, event_nm, exc):
         try:
-            self.callback(f"before_{event_nm}")
+            self._callback(f"before_{event_nm}")
             func()
         except exc:
-            self.callback(f"after_cancel_{event_nm}")
+            self._callback(f"after_cancel_{event_nm}")
         finally:
-            self.callback(f"after_{event_nm}")
+            self._callback(f"after_{event_nm}")
 
     def _backward(self):
         self.loss.backward()
 
     def _step(self):
         self.opt.step()
 
     def _one_batch(self):
         self.preds = self.model(*self.xb)
-        self.callback("after_predict")
+        self._callback("after_predict")
         self.loss = self.loss_func(self.preds, *self.yb)
-        self.callback("after_loss")
+        self._callback("after_loss")
         if self.training:
             self._with_events(
                 self._backward, "backward", CancelBackwardException
             )
             self._with_events(self._step, "step", CancelStepException)
             self.opt.zero_grad()
 
@@ -193,24 +251,22 @@
         self.iters = len(self.dl)
         for self.iter, self.batch in enumerate(self.dl):
             self.xb = self.batch[: self.n_inp]
             self.yb = self.batch[self.n_inp :]
             self._with_events(self._one_batch, "batch", CancelBatchException)
 
     def _one_epoch_train(self):
-        self.model.train()
         self.dl = self.dls.train
         self._with_events(self._all_batches, "train", CancelTrainException)
 
     def _one_epoch_validate(self):
-        self.model.eval()
         self.dl = self.dls.valid
         with torch.no_grad():
             self._with_events(
-                self._all_batches, "validate", CancelValidException
+                self._all_batches, "validate", CancelValidateException
             )
 
     def _one_epoch(self):
         if self.run_train:
             self._one_epoch_train()
         if self.run_valid:
             self._one_epoch_validate()
@@ -219,51 +275,52 @@
         for epoch in range(self.n_epochs):
             self.epoch = epoch
             self._with_events(self._one_epoch, "epoch", CancelEpochException)
 
     def fit(
         self,
         n_epochs: int = 1,
-        train: bool = True,
-        valid: bool = True,
-        callbacks: Iterable | None = None,
+        run_train: bool = True,
+        run_valid: bool = True,
+        callbacks: Iterable[Callback] | None = None,
         lr: float | None = None,
         reset_opt: bool = False,
     ) -> None:
         """
         Fit the model for `n_epochs`.
 
         Parameters
         ----------
         n_epochs : int, default=1
             Number epochs to train the model.
-        train : bool, default=True
+        run_train : bool, default=True
             Whether to run training passes.
-        valid : bool, default=True
+        run_valid : bool, default=True
             Whether to run validation passes.
-        callbacks : Iterable | None, default=None
-            Callbacks to add the existing callbacks. The added callbacks will
-            be removed when before `fit` returns.
+        callbacks : Iterable[Callback] | None, default=None
+            Callbacks to add to the existing callbacks. The added
+            callbacks will be removed  before `fit` returns.
         lr : float | None, default=None
-            Learning rate. If None, use `lr` passed when created `Learner`.
+            Learning rate. If None, `lr` passed to `Learner` will be
+            used.
         reset_opt : bool, default=False
             Whether to reset the optimizer.
         """
-        self.run_train = train
-        self.run_valid = valid
-        callbacks = self.add_callbacks(callbacks)
+        self.run_train = run_train
+        self.run_valid = run_valid
+        callbacks = self._add_callbacks(callbacks)
         self.n_epochs = n_epochs
         if lr is None:
             lr = self.lr
         if reset_opt or not self.opt:
-            self.opt = self.opt_func(self.model.parameters(), lr)
+            self.opt = self.opt_func(self.splitter(self.model), lr)
         try:
             self._with_events(self._fit, "fit", CancelFitException)
         finally:
-            self.remove_callbacks(callbacks)
+            self._remove_callbacks(callbacks)
 
     def lr_find(
         self,
         start_lr: float = 1e-7,
         gamma: float = 1.3,
         num_iter: int = 100,
         stop_div: bool = True,
@@ -290,74 +347,78 @@
             training.
         """
         n_epochs = num_iter // len(self.dls.train) + 1
         callbacks = [
             LRFinder(gamma, num_iter, stop_div, max_mult),
             Recorder("lr"),
         ]
-        self.fit(n_epochs, valid=False, callbacks=callbacks, lr=start_lr)
-        self.recorder.plot()
+        self.fit(n_epochs, run_valid=False, callbacks=callbacks, lr=start_lr)
 
     def save_model(
         self,
-        path: str | Path,
+        path: str | Path | None = None,
         with_opt: bool = False,
         with_epoch: bool = False,
         with_loss: bool = False,
         pickle_protocol: int = pickle.HIGHEST_PROTOCOL,
     ) -> None:
         """
         Save the model and optionally the optimizer, epoch, and the loss.
         Useful for checkpointing.
 
         Parameters
         ----------
-        path : str | Path
-            File path to save the model.
+        path : str | Path | None, default=None
+            File path to save the model. If None, use
+            `learner.model_dir_path`/model.
         with_opt : bool, default=False
             Whether to save the optimizer state.
         with_epoch : bool, default=False
             Whether to save the current epoch number.
         with_loss : bool, default=False
             Whether to save the current loss.
         pickle_protocol : int, default=pickle.HIGHEST_PROTOCOL
             Protocol used by pickler when saving the checkpoint.
         """
+        if path is None:
+            path = self.model_dir_path / "model"
         checkpoint = {
             "model_state_dict": self.model.state_dict(),
         }
         if with_opt:
             checkpoint["optimizer_state_dict"] = self.opt.state_dict()
         if with_epoch:
             checkpoint["epoch"] = self.epoch
         if with_loss:
             checkpoint["loss"] = self.loss
         torch.save(checkpoint, path, pickle_protocol=pickle_protocol)
 
     def load_model(
         self,
-        path: str | Path,
+        path: str | Path | None = None,
         with_opt: bool = False,
         with_epoch: bool = False,
         with_loss: bool = False,
     ) -> None:
         """
         Load the model and optionally the optimizer, epoch, and the loss.
 
         Parameters
         ----------
-        path : str | Path
-            Model's file path.
+        path : str | Path | None, default=None
+            Model's file path. If None, use `learner.model_dir_path`/model.
         with_opt : bool, default=False
             Whether to load the optimizer state.
         with_epoch : bool, default=False
             Whether to load the current epoch number.
         with_loss : bool, default=False
             Whether to load the current loss.
         """
+        if path is None:
+            path = self.model_dir_path / "model"
         checkpoint = torch.load(path)
         self.model.load_state_dict(checkpoint["model_state_dict"])
         if with_opt:
             self.opt.load_state_dict(checkpoint["optimizer_state_dict"])
         if with_epoch:
             self.epoch = checkpoint["epoch"]
         if with_loss:
@@ -367,30 +428,30 @@
     def training(self) -> bool:
         return self.model.training
 
     @training.setter
     def training(self, v) -> None:
         self.model.training = v
 
-    def add_callbacks(self, cbs):
+    def _add_callbacks(self, cbs):
         added_callbacks = []
         for cb in listify(cbs):
             if not hasattr(self, cb.name):
                 cb.set_learner(self)
                 setattr(self, cb.name, cb)
                 self.callbacks.append(cb)
                 added_callbacks.append(cb)
         return added_callbacks
 
-    def remove_callbacks(self, cbs):
+    def _remove_callbacks(self, cbs):
         for cb in listify(cbs):
             delattr(self, cb.name)
             self.callbacks.remove(cb)
 
-    def callback(self, event_nm):
+    def _callback(self, event_nm):
         for cb in sorted(self.callbacks, key=lambda x: x.order):
             cb(event_nm)
 
     def summary(self, verbose: int = 2, **kwargs):
         """Use `torchinfo` package to print out the model summary."""
         return summary(
             self.model,
@@ -401,7 +462,37 @@
                 "num_params",
                 "mult_adds",
                 "params_percent",
             ],
             verbose=verbose,
             **kwargs,
         )
+
+    def show_batch(
+        self,
+        sample_sz: int = 1,
+        callbacks: Iterable[Callable] | None = None,
+        **kwargs,
+    ):
+        """
+        Show `sample_sz` batch of input. The input would be what the
+        model would see when making predictions. Therefore, all
+        transformations and other augmentation will be applied to the
+        input.
+
+
+        Parameters
+        ----------
+        sample_sz : int, default=1
+            Number of input samples to show.
+        callbacks : Iterable[Callback] | None, default=None
+            Callbacks to add to the existing callbacks. The added
+            callbacks will be removed  before `show_batch` returns.
+
+        Raises
+        ------
+        NotImplementedError
+            Different types of `Learner`'s must implement their own
+            version depending on the type of input data. For example,
+            `VisionLearner`'s would show images.
+        """
+        raise NotImplementedError()
```

### Comparing `cmn_ai-0.0.1/cmn_ai/plot.py` & `cmn_ai-0.0.2/cmn_ai/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,11 +177,10 @@
     nrows : int, default=None
         Number of rows in the grid.
     ncols : int, default=None
         Number of columns in the grid.
     titles : list, default=None
         List of titles for each image.
     """
-    "Show all images `ims` as subplots with `rows` using `titles`"
     axs = get_grid(len(images), nrows, ncols, **kwargs)[1].flat
     for im, t, ax in zip_longest(images, titles or [], axs):
         show_image(im, ax=ax, title=t)
```

### Comparing `cmn_ai-0.0.1/cmn_ai/tabular/eda.py` & `cmn_ai-0.0.2/cmn_ai/tabular/eda.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     res = res[res > 0.0].sort_values(ascending=False)
     if not formatted:
         return res
     return (
         pd.DataFrame(res)
         .reset_index()
         .rename(columns={"index": "feature", 0: "na_percentages"})
-        .style.hide_index()
+        .style.hide(axis="index")
         .background_gradient(cmap=sns.light_palette("red", as_cmap=True))
         .format({"na_percentages": "{:.3%}"})
     )
 
 
 def get_ecdf(a: list | np.array | pd.Series) -> np.array:
     """
@@ -100,15 +100,15 @@
     """
     Plot individual and cumulative of the variance explained by each PCA
     component.
 
     Parameters
     ----------
     pca_transformer : PCA
-        PCA transformer.
+        Fitted PCA transformer.
     figsize : tuple, default=(12, 6)
         Figure size.
     """
     var_ratio = pca_transformer.explained_variance_ratio_
     cum_var_exp = np.cumsum(var_ratio)
     plt.figure(figsize=figsize)
     plt.bar(
@@ -131,38 +131,38 @@
     plt.title("PCA on training data", {"fontsize": 18})
 
 
 def plot_corr_matrix(
     df: pd.DataFrame, method: str = "pearson", figsize: tuple = (12, 6)
 ) -> None:
     """
-    Plot correlation matrix using `method`.
+    Plot `method` correlation matrix heatmap.
 
     Parameters
     ----------
     df : pd.DataFrame
         Dataframe to compute correlation.
     method : str, default='pearson'
         Method of correlation.
     figsize : tuple, default=(12, 6)
         Figure size.
     """
     corr_matrix = df.corr(method=method).round(2)
     mask = np.zeros_like(corr_matrix)
     mask[np.triu_indices_from(mask, k=1)] = True
 
-    # Plot the heat map
     sns.set(font_scale=1.2)
     plt.style.use("seaborn-v0_8-white")
     plt.figure(figsize=figsize)
     cmap = sns.diverging_palette(0, 120, as_cmap=True)
     sns.heatmap(
         corr_matrix,
         mask=mask,
         annot=True,
+        fmt=".1f",
         cmap=cmap,
         center=0,
         square=True,
         linewidths=0.1,
         cbar_kws={"shrink": 0.5},
         xticklabels=df.columns,
         yticklabels=df.columns,
```

### Comparing `cmn_ai-0.0.1/cmn_ai/tabular/preprocessing.py` & `cmn_ai-0.0.2/cmn_ai/tabular/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Most datasets need to be preprocessed/transformed before they can be passed to
 the model. This module includes common transformers that are compatible with
 [`sklearn`](www.scikit-learn.org) `Pipeline` or `ColumnTransformer`.
 """
+
 from __future__ import annotations
 
 from itertools import product
 from typing import Iterable
 
 import numpy as np
 import pandas as pd
@@ -18,37 +19,36 @@
     """
     Transform date features by deriving useful date/time attributes:
 
     - date attributes: `Year, Month, Week, Day, Dayofweek, Dayofyear,
     Is_month_end, Is_month_start, Is_quarter_end, Is_quarter_start,
     Is_year_end, Is_year_start`.
     - time attributes: `Hour, Minute, Second`.
-
-    Parameters
-    ----------
-    date_feats : Iterable, default=None
-        Date features to transform. If None, all features with `datetime64`
-        data type will be used.
-    time : bool, default=False
-        Whether to add time-related derived features such as Hour/Minute/...
-    drop : bool, default=True
-        Whether to drop date features used.
     """
 
     def __init__(
         self,
         date_feats: Iterable[str] | None = None,
         time: bool = False,
         drop: bool = True,
     ) -> None:
-        """Initialize self."""
+        """
+        Parameters
+        ----------
+        date_feats : Iterable, default=None
+            Date features to transform. If None, all features with `datetime64`
+            data type will be used.
+        time : bool, default=False
+            Whether to add time-related derived features such as Hour/Minute/...
+        drop : bool, default=True
+            Whether to drop date features used.
+        """
         self.date_feats = date_feats
         self.time = time
         self.drop = drop
-        self.dates_min = {}
         self.attrs = [
             "Year",
             "Month",
             "Week",
             "Day",
             "Dayofweek",
             "Dayofyear",
```

### Comparing `cmn_ai-0.0.1/cmn_ai/text/data.py` & `cmn_ai-0.0.2/cmn_ai/text/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,51 +5,50 @@
 
 from ..utils.data import ItemList, get_files
 
 
 class TextList(ItemList):
     """
     Build a text list from list of files in the `path` end with
-    extensions, optionally recursively.
-
-    Parameters
-    ----------
-    path : str | Path
-        Path for the root directory to search for files.
-    extensions : str | Iterable[str] | None, default=IMAGE_EXTENSIONS
-        Suffixes of filenames to look for.
-    include : Iterable[str] | None, default=None
-        Top-level Director(y|ies) under `path` to use to search for files.
-    recurse : bool, default=True
-        Whether to search subdirectories recursively.
-    tfms : Callable | None, default=None
-        Transformations to apply items before returning them.
-    Returns
-    -------
-    list[str]
-        List of filenames that ends with `extensions` under `path`.
+    `extensions`, optionally recursively.
     """
 
     @classmethod
     def from_files(
         cls,
         path: str | Path,
         extensions: Iterable[str] | str = ".txt",
         include: Iterable[str] | None = None,
         recurse: bool = True,
         tfms: Callable | None = None,
-        **kwargs,
+        encoding="utf8",
     ) -> TextList:
         """
-        Build an text list from list of files in the `path` end with
-        extensions, optionally recursively.
+        Parameters
+        ----------
+        path : str | Path
+            Path for the root directory to search for files.
+        extensions : str | Iterable[str] | None, default=IMAGE_EXTENSIONS
+            Suffixes of filenames to look for.
+        include : Iterable[str] | None, default=None
+            Top-level Director(y|ies) under `path` to use to search for
+            files.
+        recurse : bool, default=True
+            Whether to search subdirectories recursively.
+        tfms : Callable | None, default=None
+            Transformations to apply items before returning them.
+        encoding : str, default=utf8
+            Name of encoding used to decode files.
         """
         return cls(
-            get_files(path, extensions, include, recurse), path, tfms, **kwargs
+            get_files(path, extensions, include, recurse),
+            path,
+            tfms,
+            encoding=encoding,
         )
 
     def get(self, i):
         """Returns text in the file as string if `i` is path to a file."""
         if isinstance(i, Path):
-            with open(i, encoding="utf8") as f:
+            with open(i, encoding=self.encoding) as f:
                 return f.read()
         return i
```

### Comparing `cmn_ai-0.0.1/cmn_ai/utils/data.py` & `cmn_ai-0.0.2/cmn_ai/utils/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
-This modules includes most of the utilities related to working data in general,
-and with `pytorch` related data in specific. It includes functions from
-composing transforms and getting train/valid `DataLoader`s to splitting and
-labeling `Dataset`s.
+This module includes most of the utilities related to working with data
+in general, and with `pytorch`'s related data in specific. It includes
+functions from composing transforms and getting train/valid
+`DataLoader`s to splitting and labeling `Dataset`s.
 """
+
 from __future__ import annotations
 
 import os
 from collections import UserList
 from collections.abc import Iterable, Sequence
 from operator import itemgetter
 from pathlib import Path
@@ -17,48 +18,48 @@
 import numpy as np
 import torch
 from datasets.dataset_dict import DatasetDict
 from torch import Tensor
 from torch.utils.data import DataLoader, Dataset, default_collate
 
 from .processors import Processor
-from .utils import listify, setify
+from .utils import listify
+
+default_device = "cuda" if torch.cuda.is_available() else "cpu"
 
 
 def get_dls(
     train_ds: Dataset, valid_ds: Dataset, batch_size: int, **kwargs
 ) -> tuple[DataLoader]:
     """
-    Returns two dataloaders: 1 for training and 1 for 1 for validation. The
-    validation dataloader has twice the batch size and doesn't shuffle data.
+    Returns two dataloaders: 1 for training and 1 for validation. The
+    validation dataloader has twice the batch size and doesn't shuffle
+    data.
     """
     return (
         DataLoader(train_ds, batch_size=batch_size, shuffle=True, **kwargs),
         DataLoader(
             valid_ds, batch_size=batch_size * 2, shuffle=False, **kwargs
         ),
     )
 
 
-default_device = "cuda" if torch.cuda.is_available() else "cpu"
-
-
 def to_device(
     x: Tensor | Iterable[Tensor] | Mapping[str, Tensor],
-    device: str = default_device,
+    device: str | torch.device = default_device,
 ):
     """
     Copy tensor(s) to device. If the tensor is already on the device,
     returns the tensor itself.
 
     Parameters
     ----------
     x : Tensor | Iterable[Tensor] | Mapping[str, Tensor]
-        Tensor or collection of tensors to move to devive.
-    device : str, default='cuda` if available else 'cpu'
+        Tensor or collection of tensors to move to device.
+    device : str | torch.device, default='cuda:0` if available else 'cpu'
         Device to copy the tensor to.
 
     Returns
     -------
     out : Tensor | Iterable[Tensor] | Mapping[str, Tensor]
         Copied tensor(s) on the `device`.
     """
@@ -67,92 +68,105 @@
     if isinstance(x, Mapping):
         return {k: v.to(device) for k, v in x.items()}
     return type(x)(to_device(o, device) for o in x)
 
 
 def to_cpu(x: Tensor | Iterable[Tensor] | Mapping[str, Tensor]):
     """
-    Copy tensor(s) to CPU. If a tensor is already on the CPU, returns the
-    tensor itself; otherwise, returns a copy of the tensor.
+    Copy tensor(s) to CPU. If a tensor is already on the CPU, returns
+    the tensor itself; otherwise, returns a copy of the tensor.
     """
     if isinstance(x, Mapping):
         return {k: to_cpu(v) for k, v in x.items()}
     if isinstance(x, list):
         return [to_cpu(o) for o in x]
     if isinstance(x, tuple):
         return tuple(to_cpu(list(x)))
     res = x.detach().cpu()
     return res.float() if res.dtype == torch.float16 else res
 
 
 def collate_dict(ds: DatasetDict) -> Callable:
     """
-    Collate inputs from HF Dataset dictionary and returns list of inputs after
-    applying pytorch's default collate function.
+    Collate inputs from HF Dataset dictionary and returns list of
+    inputs after applying pytorch's default collate function.
 
     Parameters
     ----------
     ds : DatasetDict
         HF Dataset dictionary.
 
     Returns
     -------
-    function : tuple
+    Callable
         Wrapper function that returns tuple of collated inputs.
     """
     get = itemgetter(*ds.features)
 
     def _f(batch):
+        # default_collate(batch) -> dictionary where values are stacked
+        # tensors
+        # get() would return the tuple of stacked tensors instead of
+        # dictionary
         return get(default_collate(batch))
 
     return _f
 
 
-def collate_device(device: torch.device) -> Callable:
+def collate_device(device: str | torch.device) -> Callable:
     """
     Collate inputs from batch and copy it to `device`.
 
     Parameters
     ----------
-    device : torch.device
+    device : str | torch.device
         Device to copy batch to.
 
     Returns
     -------
-    function : callable
+    Callable
         Wrapper function that returns tuple of collated inputs.
     """
 
     def _f(batch):
         return to_device(default_collate(batch), device)
 
     return _f
 
 
 class DataLoaders:
-    def __init__(self, *dls):
+    """Create train/valid DataLoaders."""
+
+    def __init__(self, *dls) -> None:
+        """
+        Parameters
+        ----------
+        dls
+            list of DataLoaders.
+        """
         self.train, self.valid = dls[:2]
 
     @classmethod
     def from_dd(
         cls, dd: DatasetDict, batch_size: int, **kwargs
     ) -> DataLoaders:
         """
         Create train/valid data loaders from HF Dataset dictionary.
 
         Parameters
         ----------
         dd : DatasetDict
-            HF Dataset dictionary.
+            HF Dataset dictionary. Must have at least two datasets: train and
+            valid/test datasets.
         batch_size : int
             batch size passed to DataLoader.
 
         Returns
         -------
-        DataLoaders
+        tuple[DataLoader]
             Train/valid data loaders.
         """
         return cls(
             *get_dls(
                 *dd.values(),
                 batch_size=batch_size,
                 collate_fn=collate_dict(dd["train"]),
@@ -161,17 +175,17 @@
         )
 
 
 def compose(
     x: Any, funcs: Callable, *args, order: str = "order", **kwargs
 ) -> Any:
     """
-    Applies transformations in `funcs` to the input `x` in  `order` order.
+    Applies transformations in `funcs` to the input `x` in  `order`.
     """
-    for func in sorted(listify(funcs), key=lambda x: getattr(x, order, 0)):
+    for func in sorted(listify(funcs), key=lambda o: getattr(o, order, 0)):
         x = func(x, *args, **kwargs)
     return x
 
 
 def _get_files(path, fs, extensions=None):
     """Get filenames in `path` that have extension `extensions`."""
     path = Path(path)
@@ -207,16 +221,15 @@
 
     Returns
     -------
     list[str]
         List of filenames that ends with `extensions` under `path`.
     """
     path = Path(path)
-    extensions = setify(extensions)
-    extensions = {e.lower() for e in extensions}
+    extensions = {e.lower() for e in listify(extensions)}
     if recurse:
         res = []
         for i, (p, d, fs) in enumerate(os.walk(path)):
             if include is not None and i == 0:
                 d[:] = [o for o in d if o in include]
             else:
                 d[:] = [o for o in d if not o.startswith(".")]
@@ -226,71 +239,91 @@
         fs = [o.name for o in os.scandir(path) if o.is_file()]
         return _get_files(path, fs, extensions)
 
 
 class ListContainer(UserList):
     """
     Extend builtin list by changing the creation of the list from the given
-    items and and changing repr to return first 10 items along with total
-    number items and the class name. This will be the base class where other
+    items and changing repr to return first 10 items along with total number of
+    items and the class name. This will be the base class where other
     containers will inherit from.
-
-    Parameters
-    ----------
-    items : Any
-        Items to create list from.
     """
 
     def __init__(self, items) -> None:
+        """
+        Parameters
+        ----------
+        items : Any
+            Items to create list from.
+        """
         self.data = listify(items)
 
     def __repr__(self) -> str:
-        res = (
-            f"{self.__class__.__name__}: ({len(self.data):,} items)\n"
-            f"{self.data[:10]}"
-        )
+        cls_nm = self.__class__.__name__
+        res = f"{cls_nm}: ({len(self.data) :,} items)\n{self.data[:10]}"  # noqa: E231
         if len(self) > 10:
             res = res[:-1] + ", ...]"
         return res
 
 
 class ItemList(ListContainer):
     """
-    Base class for all type of datasets such as image, text, etc.
-
-    Parameters
-    ----------
-    items : Sequence
-        Items to create list.
-    path : str | Path, default="."
-        Path of the items that were used to create the list.
-    tfms : Callable | None, default=None
-        Transformations to apply items before returning them.
+    Base class for all types of datasets such as image, text, etc.
     """
 
     def __init__(
         self,
         items: Sequence,
         path: str | Path = ".",
         tfms: Callable | None = None,
+        **kwargs,
     ) -> None:
+        """
+        Parameters
+        ----------
+        items : Sequence
+            Items to create list.
+        path : str | Path, default="."
+            Path of the items that were used to create the list.
+        tfms : Callable | None, default=None
+            Transformations to apply on items before returning them.
+        """
         super().__init__(items)
         self.path = Path(path)
         self.tfms = tfms
+        self.__dict__.update(kwargs)
 
     def __repr__(self) -> str:
         return super().__repr__() + f"\nPath: {self.path.resolve()}"
 
-    def new(self, items, cls=None) -> ItemList:
+    def new(self, items: Sequence, cls: ItemList | None = None) -> ItemList:
+        """
+        Create a new instance of the `ItemList` with `items`.
+
+        Parameters
+        ----------
+        items : Sequence
+            The items to create the list from.
+        cls : ItemList | None, default=None
+            The class to instantiate. If None, the same class will be used.
+
+        Returns
+        -------
+        ItemList
+            The new instance of the `ItemList`.
+        """
         if cls is None:
             cls = self.__class__
         return cls(items, self.path, self.tfms)
 
     def get(self, item):
-        """Every class that inherits from ItemList has to override this method."""
+        """
+        Every class that inherits from `ItemList` has to override this
+        method.
+        """
         return item
 
     def _get(self, item):
         """Returns items after applying all transforms `tfms`."""
         return compose(self.get(item), self.tfms)
 
     def __getitem__(self, idx):
@@ -298,59 +331,60 @@
         if isinstance(items, UserList):
             return [self._get(item) for item in items]
         return self._get(items)
 
 
 def random_splitter(f_name: str, p_valid: float = 0.2) -> bool:
     """
-    Randomly split items with `p_valid` probability to be in the validation set.
+    Randomly split items with `p_valid` probability to be in the
+    validation set.
 
     Parameters
     ----------
     f_name : str
-        Item's filename. Not used here, but left for API consistency with
-        other splitters.
+        Item's filename. Not used here, but left for API consistency
+        with other splitters.
     p_valid : float, optional
         Probability of the item to be in the validation set.
 
     Returns
     -------
     bool
-        Whether the item is in training or validation directories.
+        True if the item is in validation else False (training).
     """
     return np.random.random() < p_valid
 
 
 def grandparent_splitter(
     f_name: str | Path, valid_name: str = "valid", train_name: str = "train"
 ) -> bool | None:
     """
     Split items based on whether they fall under validation or training
-    directories. This assumes that the directory structure is train/label/items
-    or valid/label/items.
+    directories. This assumes that the directory structure is
+    train/label/items or valid/label/items.
 
     Parameters
     ----------
     f_name : str | Path
         Item's filename.
     valid_name : str, default="valid"
         Name of the directory that holds the validation items.
     train_name : str, default="train"
         Name of the directory that holds the training items.
 
     Returns
     -------
     bool | None
-        Whether the item is in training or validation directories.
+        True if the item is in validation else False (training).
         If neither, returns None.
     """
     gp = Path(f_name).parent.parent.name
     if gp == valid_name:
         return True
-    elif gp == train_name:
+    if gp == train_name:
         return False
     return
 
 
 def split_by_func(items: Iterable, func: Callable) -> tuple[list, list]:
     """
     Split items into train/valid lists using `func`.
@@ -373,72 +407,83 @@
     train = [o for o, m in zip(items, mask) if m is False]
     return train, val
 
 
 class SplitData:
     """
     Split Item list into train and validation data lists.
-
-    Parameters
-    ----------
-    train : ItemList
-        Training items.
-    valid : ItemList
-        Validation items.
     """
 
     def __init__(self, train: ItemList, valid: ItemList) -> None:
+        """
+        Parameters
+        ----------
+        train : ItemList
+            Training items.
+        valid : ItemList
+            Validation items.
+        """
         self.train = train
         self.valid = valid
 
     def __getattr__(self, k):
         return getattr(self.train, k)
 
-    # This is needed if we want to pickle SplitData objects and be able to load
-    # it back without recursion errors
+    # This is needed if we want to pickle SplitData objects and be able
+    # to load it back without recursion errors
     def __setstate__(self, data):
         self.__dict__.update(data)
 
     @classmethod
-    def split_by_func(cls, item_list, split_func) -> SplitData:
+    def split_by_func(
+        cls, item_list: ItemList, split_func: Callable
+    ) -> SplitData:
         """
-        Split item list by splitter function and returns a SplitData object.
+        Split item list by splitter function and returns a SplitData
+        object.
         """
+        # We need to use `data` attribute to get the item list so when
+        # we index into it we get the element itself, not the
+        # transformed element.
         train_files, val_files = split_by_func(item_list.data, split_func)
+        # Because files would be of type list, change type to its
+        # original type with the original path/transforms
         train_list, val_list = map(item_list.new, (train_files, val_files))
         return cls(train_list, val_list)
 
     def to_dls(
         self, batch_size: int = 32, **kwargs
     ) -> tuple[DataLoader, DataLoader]:
         """
-        Returns a tuple of training and validation DataLoaders object using
+        Returns a tuple of training and validation DataLoaders using
         train and valid datasets.
         """
         return get_dls(self.train, self.valid, batch_size, **kwargs)
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}\n---------\nTrain - {self.train}\n\n"
             f"Valid - {self.valid}\n"
         )
 
 
 class LabeledData:
+    """
+    Create a labeled data and expose both x & y as item lists after
+    passing them through all processors.
+    """
+
     def __init__(
         self,
         x: ItemList,
         y: ItemList,
         proc_x: Processor | Iterable[Processor] | None = None,
         proc_y: Processor | Iterable[Processor] | None = None,
     ) -> None:
         """
-        Create a labeled data and expose both x & y as item lists after passing
-        them through all processors.
-
         Parameters
         ----------
         x : ItemList
             Input items to the model.
         y : ItemList
             Label items.
         proc_x : Processor | Iterable[Processor] | None, default=None
@@ -448,45 +493,113 @@
         """
         self.x = self.process(x, proc_x)
         self.y = self.process(y, proc_y)
         self.proc_x = proc_x
         self.proc_y = proc_y
 
     def process(self, item_list, proc):
+        """
+        Applies processors to an ItemList.
+
+        Parameters
+        ----------
+        item_list : ItemList
+            The ItemList to process.
+        proc : Processor | Iterable[Processor]
+            The processor or list of processors to apply.
+
+        Returns
+        -------
+        ItemList
+            The processed ItemList.
+        """
         return item_list.new(compose(item_list.data, proc))
 
     def __repr__(self):
         return f"{self.__class__.__name__}\nx: {self.x}\ny: {self.y}\n"
 
     def __getitem__(self, idx):
         return self.x[idx], self.y[idx]
 
     def __len__(self):
         return len(self.x)
 
     def x_obj(self, idx):
-        return self.obj(self.x, idx, self.proc_x)
+        """
+        Returns the input object at index idx after applying all
+        processors in proc_x.
 
-    def y_obj(self, idx):
-        return self.obj(self.y, idx, self.proc_y)
+        Parameters
+        ----------
+        idx : int
+            Index of the input object to retrieve.
+
+        Returns
+        -------
+        Any
+            The input object at index idx after applying all processors
+            in proc_x.
+        """
+        return self._obj(self.x, idx, self.proc_x)
 
-    def obj(self, items, idx, procs):
+    def y_obj(self, idx: int) -> Any:
+        """
+        Returns the label object at index idx after applying all
+        processors in proc_y.
+
+        Parameters
+        ----------
+        idx : int
+            Index of the label object to retrieve.
+
+        Returns
+        -------
+        Any
+            The label object at index idx after applying all processors
+            in proc_y.
+        """
+        return self._obj(self.y, idx, self.proc_y)
+
+    def _obj(self, items, idx, procs):
         item = items[idx]
         for proc in reversed(listify(procs)):
             item = proc.deprocess(item)
         return item
 
     @staticmethod
     def _label_by_func(ds, label_func, cls=ItemList):
         return cls([label_func(o) for o in ds.data], path=ds.path)
 
     @classmethod
     def label_by_func(
-        cls, item_list, label_func, proc_x=None, proc_y=None
+        cls,
+        item_list: ItemList,
+        label_func: Callable,
+        proc_x: Callable | None = None,
+        proc_y: Callable | None = None,
     ) -> LabeledData:
+        """
+        Label an ItemList using a labeling function.
+
+        Parameters
+        ----------
+        item_list : ItemList
+            The ItemList to be labeled.
+        label_func : Callable
+            The function to be used for labeling.
+        proc_x : Callable | None, default=None
+            The processor to be applied to the input data.
+        proc_y : Callable | None, default=None
+            The processor to be applied to the label data.
+
+        Returns
+        -------
+        LabeledData
+            The labeled ItemList.
+        """
         return cls(
             item_list,
             LabeledData._label_by_func(item_list, label_func),
             proc_x=proc_x,
             proc_y=proc_y,
         )
 
@@ -495,22 +608,48 @@
     """
     Label a file based on its parent directory.
 
     Parameters
     ----------
     f_name : str | Path
         Filename to get the parent directory.
+
+    Returns
+    -------
+    str
+        Name of the parent directory.
     """
     return Path(f_name).parent.name
 
 
 def label_by_func(
-    splitted_data, label_func, proc_x=None, proc_y=None
+    splitted_data: SplitData,
+    label_func: Callable,
+    proc_x: Callable | None = None,
+    proc_y: Callable | None = None,
 ) -> SplitData:
-    """Label splitted data using `label_func`."""
+    """
+    Label splitted data using `label_func`.
+
+    Parameters
+    ----------
+    splitted_data : SplitData
+        The splitted data to be labeled.
+    label_func : Callable
+        The function to be used for labeling.
+    proc_x : Callable | None, default=None
+        The processor to be applied to the input data.
+    proc_y : Callable | None, default=None
+        The processor to be applied to the label data.
+
+    Returns
+    -------
+    SplitData
+        The labeled splitted data.
+    """
     train = LabeledData.label_by_func(
         splitted_data.train, label_func, proc_x=proc_x, proc_y=proc_y
     )
     valid = LabeledData.label_by_func(
         splitted_data.valid, label_func, proc_x=proc_x, proc_y=proc_y
     )
     return SplitData(train, valid)
```

### Comparing `cmn_ai-0.0.1/cmn_ai/utils/utils.py` & `cmn_ai-0.0.2/cmn_ai/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Useful Python utilities."""
+
 from __future__ import annotations
 
 import gc
 import random
 import sys
 import traceback
 from collections.abc import Iterable
@@ -19,24 +20,24 @@
     Parameters
     ----------
     obj : Any
         Object to turn into a list.
 
     Returns
     -------
-    out : list
+    list
         Returns list of the provided `obj`.
     """
     if obj is None:
         return []
-    elif isinstance(obj, list):
+    if isinstance(obj, list):
         return obj
-    elif isinstance(obj, str):
+    if isinstance(obj, str):
         return [obj]
-    elif isinstance(obj, Iterable):
+    if isinstance(obj, Iterable):
         return list(obj)
     return [obj]
 
 
 def tuplify(obj: Any) -> tuple:
     """
     Change type of any object into a tuple.
@@ -44,15 +45,15 @@
     Parameters
     ----------
     obj : Any
         Object to turn into a tuple.
 
     Returns
     -------
-    out : tuple
+    tuple
         Returns tuple of the provided `obj`.
     """
     if isinstance(obj, tuple):
         return obj
     return tuple(listify(obj))
 
 
@@ -63,48 +64,48 @@
     Parameters
     ----------
     obj : Any
         Object to turn into a set.
 
     Returns
     -------
-    out : set
+    set
         Returns set of the provided `obj`.
     """
     if isinstance(obj, set):
         return obj
     return set(listify(obj))
 
 
 def uniqueify(x: Iterable, sort: bool = False) -> list:
     """
-    Returns a list unique elements in any iterable, optionally sorted.
+    Returns a list of unique elements in any iterable, optionally sorted.
 
     Parameters
     ----------
     x : Iterable
-        iterable to get unique elements from.
+        Iterable to get unique elements from.
     sort : bool, default=False
-        whether to sort the unique elements in the list.
+        Whether to sort the unique elements in the list.
 
     Returns
     -------
-    output : list
-        List containing the unique elements.
+    list
+        List containing the unique elements, optionally sorted.
     """
     output = listify(setify(x))
     if sort:
         output.sort()
     return output
 
 
 def set_seed(seed: int = 42, deterministic: bool = False) -> None:
     """
-    Set seeds for generating random numbers for pytorch, numpy, and random
-    packages.
+    Set seeds for generating random numbers for pytorch, numpy, and
+    random packages.
 
     Parameters
     ----------
     seed : int, default=42
         Desired seed.
     deterministic : bool, default=False
         Whether pytorch uses deterministic algorithms.
@@ -113,17 +114,17 @@
     torch.manual_seed(seed)
     random.seed(seed)
     np.random.seed(seed)
 
 
 def clean_ipython_history():
     """
-    Clean IPython history. This is very useful when we have output cells with
-    large tensors.
-    Credit: code in this function mainly copied from IPython source/
+    Clean IPython history. This is very useful when we have output
+    cells with large tensors.
+    Credit: code in this function mainly copied from IPython source.
     """
     if "get_ipython" not in globals():
         return
     ip = get_ipython()  # noqa: F821
     user_ns = ip.user_ns
     ip.displayhook.flush()
     pc = ip.displayhook.prompt_count + 1
@@ -134,32 +135,33 @@
     hm.input_hist_parsed[:] = [""] * pc
     hm.input_hist_raw[:] = [""] * pc
     hm._i = hm._ii = hm._iii = hm._i00 = ""
 
 
 def clean_traceback():
     """
-    Clean memory used by traceback objects. It comes in handy when traceback
-    has big tensors attached to a traceback while the operation raised
-    `Exception`. This will lead to the tensor keeps occupying GPU memory and
-    get `OOM` error even if we try to clean up the GPU memory.
+    Clean memory used by traceback objects. It comes in handy when
+    traceback has big tensors attached to a traceback while the
+    operation raised `Exception`. This will lead to the tensor keeps
+    occupying GPU memory and get `OOM` error even if we try to clean up
+    the GPU memory.
     """
     if hasattr(sys, "last_traceback"):
         traceback.clear_frames(sys.last_traceback)
         delattr(sys, "last_traceback")
     if hasattr(sys, "last_type"):
         delattr(sys, "last_type")
     if hasattr(sys, "last_value"):
         delattr(sys, "last_value")
 
 
 def clean_memory():
     """
-    Clean memory occupied by traceback objects, IPython history, and empty GPU
-    cache.
+    Clean memory occupied by traceback objects, IPython history, and
+    empty GPU cache.
     """
     clean_traceback()
     clean_ipython_history()
     gc.collect()
     torch.cuda.empty_cache()
 
 
@@ -173,13 +175,12 @@
     ----------
     precision : int, default=2
         Number of digits of precision for floating point output.
     linewidth : int, default=125
         Number of characters per line before inserting line breaks.
     sci_mode : bool, default=False
         Whether to enable scientific notation.
-
     """
     torch.set_printoptions(
         precision=precision, linewidth=linewidth, sci_mode=sci_mode
     )
     np.set_printoptions(precision=precision, linewidth=linewidth)
```

### Comparing `cmn_ai-0.0.1/cmn_ai/vision/data.py` & `cmn_ai-0.0.2/cmn_ai/vision/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,44 +12,39 @@
     k for k, v in mimetypes.types_map.items() if v.startswith("image/")
 ]
 
 
 class ImageList(ItemList):
     """
     Build an image list from list of files in the `path` end with
-    extensions, optionally recursively.
-
-    Parameters
-    ----------
-    path : str | Path
-        Path for the root directory to search for files.
-    extensions : str | Iterable[str] | None, default=IMAGE_EXTENSIONS
-        Suffixes of filenames to look for.
-    include : Iterable[str] | None, default=None
-        Top-level Director(y|ies) under `path` to use to search for files.
-    recurse : bool, default=True
-        Whether to search subdirectories recursively.
-    tfms : Callable | None, default=None
-        Transformations to apply items before returning them.
-    Returns
-    -------
-    list[str]
-        List of filenames that ends with `extensions` under `path`.
+    `extensions`, optionally recursively.
     """
 
     @classmethod
     def from_files(
         cls,
         path: str | Path,
         extensions: Iterable[str] | str = IMAGE_EXTENSIONS,
         include: Iterable[str] | None = None,
         recurse: bool = True,
         tfms: Callable | None = None,
-        **kwargs,
     ) -> ImageList:
-        return cls(
-            get_files(path, extensions, include, recurse), path, tfms, **kwargs
-        )
+        """
+        Parameters
+        ----------
+        path : str | Path
+            Path for the root directory to search for files.
+        extensions : str | Iterable[str] | None, default=IMAGE_EXTENSIONS
+            Suffixes of filenames to look for.
+        include : Iterable[str] | None, default=None
+            Top-level Director(y|ies) under `path` to use to search for
+            files.
+        recurse : bool, default=True
+            Whether to search subdirectories recursively.
+        tfms : Callable | None, default=None
+            Transformations to apply items before returning them.
+        """
+        return cls(get_files(path, extensions, include, recurse), path, tfms)
 
     def get(self, item) -> PIL.Image:
         """Open an image using PIL."""
         return PIL.Image.open(item)
```

### Comparing `cmn_ai-0.0.1/pyproject.toml` & `cmn_ai-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "cmn-ai"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["ImadDabbura <imad.dabbura@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "cmn_ai"}]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
-pandas = "^1.5.3"
+python = ">=3.10"
+pandas = "^2.1.4"
 seaborn = "^0.12.2"
 numpy = "^1.24.2"
 matplotlib = "^3.7.1"
-scikit-learn = "^1.2.2"
-torch = "^2.0.0"
-torchvision = "^0.15.1"
+scikit-learn = "^1.4.0"
 fastprogress = "^1.0.3"
 fastcore = "^1.5.29"
 scipy = "^1.10.1"
 torchinfo = "^1.7.2"
 torcheval = "^0.0.6"
 datasets = "^2.12.0"
+torch = "^2.3.0"
+torchvision = "^0.18.0"
+pyarrow-hotfix = "^0.6"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 pytest = "^7.2.1"
```

### Comparing `cmn_ai-0.0.1/PKG-INFO` & `cmn_ai-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: cmn-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: ImadDabbura
 Author-email: imad.dabbura@hotmail.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: datasets (>=2.12.0,<3.0.0)
 Requires-Dist: fastcore (>=1.5.29,<2.0.0)
 Requires-Dist: fastprogress (>=1.0.3,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
+Requires-Dist: pandas (>=2.1.4,<3.0.0)
+Requires-Dist: pyarrow-hotfix (>=0.6,<0.7)
+Requires-Dist: scikit-learn (>=1.4.0,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
-Requires-Dist: torch (>=2.0.0,<3.0.0)
+Requires-Dist: torch (>=2.3.0,<3.0.0)
 Requires-Dist: torcheval (>=0.0.6,<0.0.7)
 Requires-Dist: torchinfo (>=1.7.2,<2.0.0)
-Requires-Dist: torchvision (>=0.15.1,<0.16.0)
+Requires-Dist: torchvision (>=0.18.0,<0.19.0)
 Description-Content-Type: text/markdown
 
 # Welcome to `cmn_ai`
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
@@ -32,14 +34,50 @@
 
 I am a big believer in **Boyd's Law**, which states that _speed of iteration beats quality of iteration_. Following this principle, I created `cmn_ai` to incorporate the most common tasks we encounter in ML/AI from data exploration to model development and training. Additionally, I baked into it some of the best practices I learned in my career so I don't have to repeat myself on every project I work on.
 
 It is worth noting that the majority of the DL code such as [`Learner`](cmn_ai/learner.py) and callbacks assume that [`pytorch`](https://pytorch.org/) is used as the underlying DL library. Also, tabular data preprocessors/models are compatible with [`sklearn`](https://github.com/scikit-learn/scikit-learn) so they can be used easily with its `Pipeline` or `ColumnTransformer`.
 
 Given the nature of the progress in ML/AI, I will always keep adding more functionalities as time passes.
 
+## Installation
+
+The easiest way to install `cmn_ai` is by using `pip`:
+
+```sh
+pip install cmn-ai
+```
+
+## Documentation
+
+The official documentation is hosted on https://imaddabbura.github.io/cmn_ai/.
+
+## Development setup
+
+The fastest way to setup the development environment is to use `poetry`. You can install `poetry` using `pip` (or `conda`).
+
+```sh
+pip install poetry
+```
+
+Then install `cmn_ai` from source as follows:
+
+```sh
+git clone https://github.com/ImadDabbura/cmn_ai
+cd cmn_ai
+poetry install
+```
+
+## Tests
+
+To run tests, run the following command:
+
+```sh
+poetry run pytest
+```
+
 ## Contributing
 
 `cmn_ai` is not open now for contribution because there are some infrastructure work I need to finish to make it ready for more contributors.
 
 ## License
 
 `cmn_ai` has Apache License, as found in the [LICENCE](LICENSE) file.
```

