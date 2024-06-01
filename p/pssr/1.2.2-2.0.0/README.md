# Comparing `tmp/pssr-1.2.2.tar.gz` & `tmp/pssr-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssr-1.2.2.tar", max compression
+gzip compressed data, was "pssr-2.0.0.tar", max compression
```

## Comparing `pssr-1.2.2.tar` & `pssr-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.2.2/LICENSE
--rw-r--r--   0        0        0     1135 2024-04-28 22:05:02.396223 pssr-1.2.2/README.md
--rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.2.2/pssr/__init__.py
--rw-r--r--   0        0        0     5574 2024-05-07 03:46:32.512042 pssr-1.2.2/pssr/__main__.py
--rw-r--r--   0        0        0     4678 2024-05-02 02:57:56.749173 pssr-1.2.2/pssr/crappifiers.py
--rw-r--r--   0        0        0    32650 2024-05-07 03:25:12.982266 pssr-1.2.2/pssr/data.py
--rw-r--r--   0        0        0     2662 2024-05-02 00:48:45.425156 pssr-1.2.2/pssr/loss.py
--rw-r--r--   0        0        0      111 2024-05-02 18:58:16.599258 pssr-1.2.2/pssr/models/__init__.py
--rw-r--r--   0        0        0     4671 2024-05-02 16:04:40.293835 pssr-1.2.2/pssr/models/_blocks.py
--rw-r--r--   0        0        0     8046 2024-05-01 15:20:32.105611 pssr-1.2.2/pssr/models/_rdnet.py
--rw-r--r--   0        0        0     7682 2024-05-06 03:52:11.907243 pssr-1.2.2/pssr/models/rdresunet.py
--rw-r--r--   0        0        0     6955 2024-05-07 02:36:15.775241 pssr-1.2.2/pssr/models/resunet.py
--rw-r--r--   0        0        0    34796 2024-05-07 03:10:57.785540 pssr-1.2.2/pssr/models/swinir.py
--rw-r--r--   0        0        0    11516 2024-05-07 03:33:47.653002 pssr-1.2.2/pssr/predict.py
--rw-r--r--   0        0        0    14608 2024-05-06 04:09:07.918747 pssr-1.2.2/pssr/train.py
--rw-r--r--   0        0        0     1133 2024-05-07 03:47:03.696502 pssr-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 pssr-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1144 2024-05-28 04:16:18.687108 pssr-2.0.0/README.md
+-rw-r--r--   0        0        0      141 2024-05-25 03:02:49.403312 pssr-2.0.0/pssr/__init__.py
+-rw-r--r--   0        0        0     7641 2024-06-01 21:42:07.657572 pssr-2.0.0/pssr/__main__.py
+-rw-r--r--   0        0        0     4684 2024-05-09 22:07:47.490900 pssr-2.0.0/pssr/crappifiers.py
+-rw-r--r--   0        0        0    31972 2024-06-01 22:02:06.007695 pssr-2.0.0/pssr/data.py
+-rw-r--r--   0        0        0      111 2024-05-02 18:58:16.599258 pssr-2.0.0/pssr/models/__init__.py
+-rw-r--r--   0        0        0     4671 2024-05-02 16:04:40.293835 pssr-2.0.0/pssr/models/_blocks.py
+-rw-r--r--   0        0        0     8022 2024-05-25 02:59:50.517525 pssr-2.0.0/pssr/models/_rdnet.py
+-rw-r--r--   0        0        0    11063 2024-06-01 20:47:20.307004 pssr-2.0.0/pssr/models/rdresunet.py
+-rw-r--r--   0        0        0     7014 2024-06-01 20:47:27.819447 pssr-2.0.0/pssr/models/resunet.py
+-rw-r--r--   0        0        0    34865 2024-06-01 20:47:33.127760 pssr-2.0.0/pssr/models/swinir.py
+-rw-r--r--   0        0        0       48 2024-06-01 20:02:46.919021 pssr-2.0.0/pssr/napari/__init__.py
+-rw-r--r--   0        0        0     7094 2024-06-01 20:57:03.978416 pssr-2.0.0/pssr/napari/_util.py
+-rw-r--r--   0        0        0      395 2024-06-01 21:32:01.836099 pssr-2.0.0/pssr/napari/napari.yaml
+-rw-r--r--   0        0        0    14467 2024-06-01 21:29:50.647984 pssr-2.0.0/pssr/napari/widgets.py
+-rw-r--r--   0        0        0    12887 2024-06-01 20:50:32.118462 pssr-2.0.0/pssr/predict.py
+-rw-r--r--   0        0        0    16117 2024-06-01 22:08:42.148198 pssr-2.0.0/pssr/train.py
+-rw-r--r--   0        0        0     3222 2024-06-01 20:50:00.360546 pssr-2.0.0/pssr/util.py
+-rw-r--r--   0        0        0     1324 2024-06-01 22:37:04.348472 pssr-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 pssr-2.0.0/PKG-INFO
```

### Comparing `pssr-1.2.2/LICENSE` & `pssr-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pssr-1.2.2/README.md` & `pssr-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 containing various improvements and new features.
 
 The **PSSR** User Guide and full API Reference is available in the [PSSR Documentation](https://ucsdmanorlab.github.io/PSSR).
 
 If you have never used **PSSR** before, [Getting Started](https://ucsdmanorlab.github.io/PSSR/guide/start.html) outlines installation and basic usage.
 Full reference and explanations of all **PSSR** tools is available in [API Reference](https://ucsdmanorlab.github.io/PSSR/reference/api.html).
 
-The package is still in development. All code can be found at [https://github.com/ucsdmanorlab/PSSR](https://github.com/ucsdmanorlab/PSSR).
+This package is under continuous development. All code can be found at [https://github.com/ucsdmanorlab/PSSR](https://github.com/ucsdmanorlab/PSSR).
 If you experience any bugs, unexpected behaviors, or have any suggestions, make sure to [open a ticket](https://github.com/ucsdmanorlab/PSSR/issues).
```

### Comparing `pssr-1.2.2/pssr/crappifiers.py` & `pssr-2.0.0/pssr/crappifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         """
         raise NotImplementedError('"crappify" method not implemented.')
     
     def __call__(self, image : np.ndarray):
         return self.crappify(image)
 
 class MultiCrappifier(Crappifier):
-    def __init__(self, *args : Crappifier, clip : bool = True):
+    def __init__(self, *args : list[Crappifier], clip : bool = True):
         r"""Chains multiple crappifiers sequentially for degrading low resolution images.
 
         Args:
             args (Crappifier) : Crappifiers to be applied in order from first to last.
 
             clip (bool) : Clip values to image range between each crappifier step. Default is True.
         """
```

### Comparing `pssr-1.2.2/pssr/data.py` & `pssr-2.0.0/pssr/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import torch, glob, os, random, czifile, tifffile, psutil, warnings
 import numpy as np
 from torch.utils.data import Dataset
 from pathlib import Path
 from tqdm import tqdm
 from PIL import Image
 from .crappifiers import Crappifier, Poisson
+from .util import _force_list
 
 class ImageDataset(Dataset):
-    def __init__(self, path : Path, hr_res : int = 512, lr_scale : int = 4, crappifier : Crappifier = Poisson(), n_frames : int = None, mode : str = "L", extension : str = "tif", val_split : float = 0.1, rotation : bool = True, split_seed : int = 0, transforms : list[torch.nn.Module] = None):
+    def __init__(self, path : Path, hr_res : int = 512, lr_scale : int = 4, crappifier : Crappifier = Poisson(), n_frames : list[int] = -1, extension : str = "tif", val_split : float = 0.1, rotation : bool = True, split_seed : int = 0, transforms : list[torch.nn.Module] = None):
         r"""Training dataset for loading high-resolution images from individual files and returning high-low-resolution pairs, the latter receiving crappification.
 
         Dataset used for pre-tiled image files. For image sheets (e.g. .czi files), use :class:`SlidingDataset`.
 
         LR mode (dataset loads only unmodified low-resolution images for prediction) can be enabled by
         either inputting images less than or equal to LR size (``hr_res``/``lr_scale``) or by setting ``lr_scale`` = None and ``hr_res`` = LR resolution.
 
@@ -20,37 +21,35 @@
 
             hr_res (int) : Resolution of high-resolution images. Images larger than this will be downscaled to this resolution. Images smaller will be padded. Default is 512.
 
             lr_scale (int) : Downscaling factor for low-resolution images to simulate undersampling. Choose a power of 2 for best results. Default is 4.
 
             crappifier (Crappifier) : Crappifier for degrading low-resolution images to simulate undersampling. Not used in LR mode. Default is :class:`Poisson`.
 
-            n_frames (int) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of None uses all stacked image frames. Default is None.
-
-            mode (str) : Color mode for loading images, e.g. "L" for grayscale, "RGB" for color. Default is "L".
+            n_frames (list[int]) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of -1 uses all stacked image frames. Default is -1.
 
             extension (str) : File extension of images. Default is "tif".
 
             val_split (float) : Proportion of images to be held out for evaluation/prediction. Default is 0.1.
 
             rotation (bool) : Whether to randomly rotate and/or flip images when loading data. Only used during training if applicable. Default is True.
 
             split_seed (int) : Seed for random train/evaluation data splitting. A value of None splits the last images as evaluation. Default is 0.
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.path = Path(path) if type(path) is str else path
-        if not self.path.exists(): raise FileNotFoundError(f'Path "{self.path}" does not exist.')
+        if not path or not self.path.exists(): raise FileNotFoundError(f'Path "{self.path}" does not exist.')
 
-        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.path))
+        self.hr_files = _root_glob(f"*.{extension}", root_dir=self.path)
         if not len(self.hr_files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{self.path}".')
 
-        self.mode = mode.upper()
-        self.n_frames = _get_n_frames(n_frames, self.mode)
+        self.mode = "L"
+        self.n_frames = _get_n_frames(n_frames)
 
         self.slices, max_size = [], 0
         for image_idx in range(len(self.hr_files)):
             image = Image.open(Path(self.path, self.hr_files[image_idx]))
             self.slices.append(1 if self.n_frames is None else image.n_frames // self.n_frames[0])
             max_size = max(max(image.size), max_size)
 
@@ -86,15 +85,15 @@
         return f'ImageDataset from path "{self.path}"\n{len(self.hr_files)} files with {len(self)} total frame slices\nLR mode {"enabled" if self.is_lr else "disabled"}'
 
     def _get_name(self, idx):
         image_idx, idx = _get_image_idx(idx, self.slices)
         return self.hr_files[image_idx].split('.')[0] + (f"_{idx}" if self.n_frames is not None else "")
 
 class SlidingDataset(Dataset):
-    def __init__(self, path : Path, hr_res : int = 512, lr_scale : int = 4, crappifier : Crappifier = Poisson(), overlap : int = 128, n_frames : int = None, stack : str = "TZ", mode : str = "L", extension : str = "czi", preload : bool = True, val_split : float = 0.1, rotation : bool = True, split_seed : int = 0, transforms : list[torch.nn.Module] = None):
+    def __init__(self, path : Path, hr_res : int = 512, lr_scale : int = 4, crappifier : Crappifier = Poisson(), overlap : int = 128, n_frames : list[int] = -1, stack : str = "TZ", extension : str = "czi", preload : bool = True, val_split : float = 0.1, rotation : bool = True, split_seed : int = 0, transforms : list[torch.nn.Module] = None):
         r"""Training dataset for loading high-resolution image tiles from image sheets and returning high-low-resolution pairs, the latter receiving crappification.
 
         Dataset used for image sheets (e.g. .czi files). For pre-tiled image files, use :class:`ImageDataset`.
 
         LR mode (dataset loads only unmodified low-resolution images for prediction) can be enabled by setting ``lr_scale`` = None and ``hr_res`` = LR resolution.
 
         Args:
@@ -104,45 +103,43 @@
 
             lr_scale (int) : Downscaling factor for low-resolution images to simulate undersampling. Choose a power of 2 for best results. Default is 4.
 
             crappifier (Crappifier) : Crappifier for degrading low-resolution images to simulate undersampling. Not used in LR mode. Default is :class:`Poisson`.
 
             overlap (int) : Overlapping pixels between neighboring tiles to increase effective dataset size. Default is 128.
 
-            n_frames (int) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of None uses all stacked image frames. Default is None.
+            n_frames (list[int]) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of -1 uses all stacked image frames. Default is -1.
 
             stack (str) : Multiframe stack handling mode, e.g "T" for time stack, "Z" for z dimension stack, "TZ" or "ZT" for both, determining flattenting order. Only applicable if loading from czi. Default is "TZ".
 
-            mode (str) : Color mode for loading images, e.g. "L" for grayscale, "RGB" for color. Default is "L".
-
             extension (str) : File extension of images. Default is "czi".
 
             preload (bool) : Whether to preload images in memory (not VRAM) for faster dataloading. Default is True.
 
             val_split (float) : Proportion of images to be held out for evaluation/prediction. Default is 0.1.
 
             rotation (bool) : Whether to randomly rotate and/or flip images when loading data. Only used during training if applicable. Default is True.
 
             split_seed (int) : Seed for random train/evaluation data splitting. A value of None splits the last images as evaluation. Default is 0.
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.path = Path(path) if type(path) is str else path
-        if not self.path.exists(): raise FileNotFoundError(f'Path "{self.path}" does not exist.')
+        if not path or not self.path.exists(): raise FileNotFoundError(f'Path "{self.path}" does not exist.')
         
-        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.path))
+        self.hr_files = _root_glob(f"*.{extension}", root_dir=self.path)
         if not len(self.hr_files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{self.path}".')
 
         overlap = 0 if overlap is None else overlap
         if not hr_res > overlap: raise ValueError(f"hr_res must be greater than overlap. Given values are {hr_res} and {overlap} respectively.")
         self.stride = hr_res - overlap
         self.stack = stack.upper()
-        self.mode = mode.upper()
-        self.n_frames = _get_n_frames(n_frames, self.mode)
+        self.mode = "L"
+        self.n_frames = _get_n_frames(n_frames)
         
         self.preload = _preload(preload, [self.path], [self.hr_files], self.mode, self.stack)
 
         self.tiles, self.slices = [], []
         for image_idx in range(len(self.hr_files)):
             image = self.preload[image_idx] if self.preload else _load_sheet(self.path, self.hr_files[image_idx], self.stack, self.mode)
             tiles_x, tiles_y = _n_tiles(image, hr_res, self.stride)
@@ -180,29 +177,27 @@
         return f'SlidingDataset from path "{self.path}"\n{len(self.hr_files)} files with {len(self)} total frame slices\nLR mode {"enabled" if self.is_lr else "disabled"}'
     
     def _get_name(self, idx):
         image_idx, idx = _get_image_idx(idx, self.slices, self.tiles)
         return f"{self.hr_files[image_idx].split('.')[0]}_{idx}"
 
 class PairedImageDataset(Dataset):
-    def __init__(self, hr_path : Path, lr_path : Path, hr_res : int = 512, lr_scale : int = 4, n_frames : int = None, mode : str = "L", extension : str = "tif", val_split : float = 1, rotation : bool = True, split_seed : int = None, transforms : list[torch.nn.Module] = None):
+    def __init__(self, hr_path : Path, lr_path : Path, hr_res : int = 512, lr_scale : int = 4, n_frames : list[int] = -1, extension : str = "tif", val_split : float = 1, rotation : bool = True, split_seed : int = None, transforms : list[torch.nn.Module] = None):
         r"""Testing dataset for loading paired high-low-resolution images without using crappification. Can also be used for approximating :class:`Crappifier` parameters.
 
         Args:
             hr_path (Path) : Path to folder containing high-resolution images. Can also be a str.
 
             lr_path (Path) : Path to folder containing low-resolution images. Can also be a str.
 
             hr_res (int) : Resolution of high-resolution images. Images larger than this will be downscaled to this resolution. Images smaller will be padded. Default is 512.
 
             lr_scale (int) : Downscaling factor for low-resolution images to simulate undersampling. Choose a power of 2 for best results. Default is 4.
 
-            n_frames (int) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of None uses all stacked image frames. Default is None.
-
-            mode (str) : Color mode for loading images, e.g. "L" for grayscale, "RGB" for color. Default is "L".
+            n_frames (list[int]) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of -1 uses all stacked image frames. Default is -1.
 
             extension (str) : File extension of images. Default is "tif".
 
             val_split (float) : Proportion of images to be held out for evaluation/prediction. Default is 1.
 
             rotation (bool) : Whether to randomly rotate and/or flip images when loading data. Only used during training if applicable. Default is True.
 
@@ -210,25 +205,25 @@
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.hr_path = Path(hr_path) if type(hr_path) is str else hr_path
         self.lr_path = Path(lr_path) if type(lr_path) is str else lr_path
         for path in [self.hr_path, self.lr_path]:
-            if not path.exists(): raise FileNotFoundError(f'Path "{path}" does not exist.')
+            if not path or not path.exists(): raise FileNotFoundError(f'Path "{path}" does not exist.')
         if self.hr_path == self.lr_path: warnings.warn("hr_path is equal to lr_path! Consider using ImageDataset instead.", stacklevel=2)
 
-        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.hr_path))
-        self.lr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.lr_path))
+        self.hr_files = _root_glob(f"*.{extension}", root_dir=self.hr_path)
+        self.lr_files = _root_glob(f"*.{extension}", root_dir=self.lr_path)
         for files, path in zip([self.hr_files, self.lr_files], [self.hr_path, self.lr_path]):
             if not len(files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{path}".')
         if len(self.hr_files) != len(self.lr_files): raise FileNotFoundError(f"Mismatch between amounts of high-low-resolution images. Found {len(self.hr_files)} high-resolution and {len(self.lr_files)} low-resolution images.")
 
-        self.mode = mode.upper()
-        self.n_frames = _get_n_frames(n_frames, self.mode)
+        self.mode = "L"
+        self.n_frames = _get_n_frames(n_frames)
 
         self.slices, max_size = [], 0
         for image_idx in range(len(self.hr_files)):
             image = Image.open(Path(self.hr_path, self.hr_files[image_idx]))
             self.slices.append(1 if self.n_frames is None else image.n_frames // self.n_frames[0])
             max_size = max(max(image.size), max_size)
 
@@ -259,15 +254,15 @@
         return f'PairedImageDataset from paths "{self.hr_path}" and "{self.lr_path}"\n{len(self.hr_files)} paired files with {len(self)} total frame slices'
 
     def _get_name(self, idx):
         image_idx, idx = _get_image_idx(idx, self.slices)
         return self.lr_files[image_idx].split('.')[0] + (f"_{idx}" if self.n_frames is not None else "")
 
 class PairedSlidingDataset(Dataset):
-    def __init__(self, hr_path : Path, lr_path : Path, hr_res : int = 512, lr_scale : int = 4, overlap : int = 128, n_frames : int = None, stack : str = "TZ", mode : str = "L", extension : str = "czi", preload : bool = True, val_split : float = 1, rotation : bool = True, split_seed : int = None, transforms : list[torch.nn.Module] = None):
+    def __init__(self, hr_path : Path, lr_path : Path, hr_res : int = 512, lr_scale : int = 4, overlap : int = 128, n_frames : list[int] = -1, stack : str = "TZ", extension : str = "czi", preload : bool = True, val_split : float = 1, rotation : bool = True, split_seed : int = None, transforms : list[torch.nn.Module] = None):
         r"""Testing dataset for loading high-low-resolution image tiles from image sheets without crappification. Can also be used for approximating :class:`Crappifier` parameters.
 
         Dataset used for image sheets (e.g. .czi files). For pre-tiled image files, use :class:`ImageDataset`.
 
         Args:
             hr_path (Path) : Path to folder containing high-resolution images. Can also be a str.
 
@@ -275,20 +270,18 @@
 
             hr_res (int) : Resolution of high-resolution images. Images larger than this will be downscaled to this resolution. Images smaller will be padded. Default is 512.
 
             lr_scale (int) : Downscaling factor for low-resolution images to simulate undersampling. Choose a power of 2 for best results. Default is 4.
 
             overlap (int) : Overlapping pixels between neighboring tiles to increase effective dataset size. Default is 128.
 
-            n_frames (int) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of None uses all stacked image frames. Default is None.
+            n_frames (list[int]) : Amount of stacked frames per image, disregarding color channels. Can also be list of low-resolution and high-resolution stack amounts respectively. A value of -1 uses all stacked image frames. Default is -1.
 
             stack (str) : Multiframe stack handling mode, e.g "T" for time stack, "Z" for z dimension stack, "TZ" or "ZT" for both, determining flattenting order. Only applicable if loading from czi. Default is "TZ".
 
-            mode (str) : Color mode for loading images, e.g. "L" for grayscale, "RGB" for color. Default is "L".
-
             extension (str) : File extension of images. Default is "czi".
 
             preload (bool) : Whether to preload images in memory (not VRAM) for faster dataloading. Default is True.
 
             val_split (float) : Proportion of images to be held out for evaluation/prediction. Default is 1.
 
             rotation (bool) : Whether to randomly rotate and/or flip images when loading data. Only used during training if applicable. Default is True.
@@ -297,29 +290,29 @@
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.hr_path = Path(hr_path) if type(hr_path) is str else hr_path
         self.lr_path = Path(lr_path) if type(lr_path) is str else lr_path
         for path in [self.hr_path, self.lr_path]:
-            if not path.exists(): raise FileNotFoundError(f'Path "{path}" does not exist.')
+            if not path or not path.exists(): raise FileNotFoundError(f'Path "{path}" does not exist.')
         if self.hr_path == self.lr_path: warnings.warn("hr_path is equal to lr_path! Consider using SlidingDataset instead.", stacklevel=2)
         
-        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.hr_path))
-        self.lr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.lr_path))
+        self.hr_files = _root_glob(f"*.{extension}", root_dir=self.hr_path)
+        self.lr_files = _root_glob(f"*.{extension}", root_dir=self.lr_path)
         for files, path in zip([self.hr_files, self.lr_files], [self.hr_path, self.lr_path]):
             if not len(files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{path}".')
         if len(self.hr_files) != len(self.lr_files): raise FileNotFoundError(f"Mismatch between amounts of high-low-resolution images. Found {len(self.hr_files)} high-resolution and {len(self.lr_files)} low-resolution images.")
 
         overlap = 0 if overlap is None else overlap
         if not hr_res > overlap: raise ValueError(f"hr_res must be greater than overlap. Given values are {hr_res} and {overlap} respectively.")
         self.stride = hr_res - overlap
         self.stack = stack.upper()
-        self.mode = mode.upper()
-        self.n_frames = _get_n_frames(n_frames, self.mode)
+        self.mode = "L"
+        self.n_frames = _get_n_frames(n_frames)
 
         self.preload = _preload(preload, [self.hr_path, self.lr_path], [self.hr_files, self.lr_files], self.mode, self.stack)
 
         self.tiles, self.slices = [], []
         for image_idx in range(len(self.hr_files)):
             image = self.preload[0][image_idx] if self.preload else _load_sheet(self.hr_path, self.hr_files[image_idx], self.stack, self.mode)
             tiles_x, tiles_y = _n_tiles(image, hr_res, self.stride)
@@ -562,38 +555,33 @@
         return image[...,center - half:center + half + 1,:,:]
 
 def _seek_channel(image, idx):
     # Because we can't have nice things...
     image.seek(idx)
     return image
 
+def _root_glob(search, root_dir):
+    files = glob.glob(f"{root_dir}/{search}")
+    return sorted([item.split("/")[-1] for item in files])
+
 def _n_tiles(image, size, stride):
     x, y = image.shape[-2:]
 
     tiles_x = max(0, (x - size) // stride + 1)
     tiles_y = max(0, (y - size) // stride + 1)
     return tiles_x, tiles_y
 
-def _get_n_frames(n_frames, mode):
-    if n_frames is None:
-        return n_frames
+def _get_n_frames(n_frames):
+    if n_frames in [None, -1, [-1]]:
+        return None
     
     n_frames = _force_list(n_frames)
     n_frames = n_frames*2 if len(n_frames) == 1 else n_frames
-    n_frames = [item*3 for item in n_frames] if mode == "RGB" else n_frames
     return n_frames # [in (low-resolution), out (high-resolution)]
 
-def _force_list(item):
-    # Because we still can't have nice things...
-    if type(item) is int:
-        return [item]
-    elif type(item) is not list:
-        return list(item)
-    return item
-
 def _get_image_idx(idx, slices, tiles=None):
     tiles = [1]*len(slices) if tiles is None else tiles
 
     image_idx = 0
     for slice, tile in zip(slices, tiles):
         if idx < slice * tile:
             return image_idx, idx
```

### Comparing `pssr-1.2.2/pssr/loss.py` & `pssr-2.0.0/pssr/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import torch, math
+import torch, math, inspect
 import torch.nn.functional as F
 import torch.nn as nn
 import numpy as np
 from pytorch_msssim import SSIM, MS_SSIM
 
 class SSIMLoss(nn.Module):
     def __init__(self, channels : int = 1, mix : float = .8, win_size : int = 11, win_sigma : float = 1.5, ms : bool = True, kwargs = None):
@@ -56,7 +56,25 @@
 
         image_range (int) : Value range of image. Default is 255.
     """
     return math.sqrt(mse) * image_range
 
 def _psnr_metric(mse : float):
     return 20 * torch.log10(1 / torch.sqrt(mse))
+
+def _force_list(item):
+    if type(item) is not list:
+        try:
+            return list(item)
+        except:
+            return [item]
+    return item
+
+def _get_callbacks(raw):
+    callbacks = [] if raw is None else _force_list(raw)
+    callback_locals = [len([arg for arg in inspect.getfullargspec(callback).args if arg != "self"]) == 1 for callback in callbacks]
+    return callbacks, callback_locals
+
+def _tab_string(text):
+    lines = text.split("\n")
+    indented_lines = ["\t" + line for line in lines]
+    return "\n".join(indented_lines)
```

### Comparing `pssr-1.2.2/pssr/models/_blocks.py` & `pssr-2.0.0/pssr/models/_blocks.py`

 * *Files identical despite different names*

### Comparing `pssr-1.2.2/pssr/models/_rdnet.py` & `pssr-2.0.0/pssr/models/_rdnet.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 class RDNet(nn.Module):
     def __init__(
         self,
         in_channels=1,
         n_init_features=128,
         patch_size=2,
         growth_rates=(64, 104, 128, 128, 128, 128, 224),
-        ds_blocks=(None, True, True, False, False, False, True),
+        ds_blocks=(False, True, True, False, False, False, True),
         block_type=["Block", "Block", "BlockESE", "BlockESE", "BlockESE", "BlockESE", "BlockESE"],
         n_blocks=(3, 3, 3, 3, 3, 3, 3),
         bottleneck_width_ratio=4,
-        drop_rate=0.0,
         drop_path_rate=0.0,
         transition_compression_ratio=0.5,
         ls_init_value=1e-6,
     ):
         super().__init__()
 
         block_type = [block_type] * len(growth_rates) if type(block_type) is str else block_type
+        block_type = ["BlockESE" if block else "Block" for block in block_type]
+            
         n_blocks = [n_blocks] * len(growth_rates) if type(n_blocks) is int else n_blocks
 
         if not len(growth_rates) == len(ds_blocks): raise ValueError(f"growth_rates and ds_blocks must have the same length. Given values are {len(growth_rates)} and {len(ds_blocks)} respectively.")
         if not len(growth_rates) == len(block_type): raise ValueError(f"growth_rates and block_type must have the same length. Given values are {len(growth_rates)} and {len(block_type)} respectively.")
         if not len(growth_rates) == len(n_blocks): raise ValueError(f"growth_rates and n_blocks must have the same length. Given values are {len(growth_rates)} and {len(n_blocks)} respectively.")
 
         # Stem
@@ -63,15 +64,14 @@
                 num_features = compressed_num_features
 
             stage = DenseStage(
                 num_block=n_blocks[i],
                 num_input_features=num_features,
                 growth_rate=growth_rates[i],
                 bottleneck_width_ratio=bottleneck_width_ratio,
-                drop_rate=drop_rate,
                 drop_path_rates=dp_rates[i],
                 ls_init_value=ls_init_value,
                 block_type=block_type[i],
             )
             dense_stage_layers.append(stage)
             num_features += n_blocks[i] * growth_rates[i]
 
@@ -140,22 +140,20 @@
 class DenseBlock(nn.Module):
     def __init__(
         self,
         num_input_features,
         growth_rate,
         bottleneck_width_ratio,
         drop_path_rate,
-        drop_rate=0.0,
         rand_gather_step_prob=0.0,
         block_idx=0,
         block_type="Block",
         ls_init_value=1e-6,
     ):
         super().__init__()
-        self.drop_rate = drop_rate
         self.drop_path_rate = drop_path_rate
         self.rand_gather_step_prob = rand_gather_step_prob
         self.block_idx = block_idx
         self.growth_rate = growth_rate
 
         self.gamma = nn.Parameter(ls_init_value * torch.ones(growth_rate)) if ls_init_value > 0 else None
         growth_rate = int(growth_rate)
```

### Comparing `pssr-1.2.2/pssr/models/rdresunet.py` & `pssr-2.0.0/pssr/models/resunet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,150 +1,139 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ._blocks import PSP_Pooling, Reconstruction, get_resblock
-from ._rdnet import RDNet
-from ..data import _force_list
+from ..util import _force_list
 
-class RDResUNet(nn.Module):
+class ResUNet(nn.Module):
     def __init__(
             self,
-            channels : int = 1,
-            hidden : list[int] = [1024, 1024, 512, 256],
+            channels : list[int] = 1,
+            hidden : list[int] = [64, 128, 256, 512, 1024],
             scale : int = 4,
             depth : int = 3,
             dilations : list[list[int]] = None,
             pool_sizes : list[int] = None,
             encoder_pool : bool = False,
-            rdnet_kwargs = None
         ):
-        r"""A RDNet (Revitalized DenseNet) encoder and ResUNet decoder with an additional image upscaling block. RDNet is detailed in Kim et al., 2024.
-        If ``dilations`` is provided, the decoder is instead a Atrous Residual UNet as detailed in Diakogiannis et al., 2019.
+        r"""A Residual UNet as detailed in Zhang et al., 2017 with an additional image upscaling block.
+        If ``dilations`` is provided, instead use a Atrous Residual UNet as detailed in Diakogiannis et al., 2019.
 
-        Channel sizes hidden[0] (and hidden[-1] if encoder_pool is True) must be divisible by pool_sizes.
+        Channel sizes hidden[0] (and hidden[-1] if encoder_pool is True) must be divisible by pool_sizes if provided.
 
         Args:
-            channels (int) : Number of channels in image data. Can also be a list of in channels and out channels respectively.
+            channels (list[int]) : Number of channels in image data. Can also be a list of in channels (low-resolution) and out channels (high-resolution) respectively.
 
-            hidden (list[int]) : Elementwise list of hidden layer channels of ResUNet decoder. Each element must have a corresponding skip connection in the RDNet encoder, provided after each downsample block.
+            hidden (list[int]) : Elementwise list of channels per residual block controlling width and length of model.
 
             scale (int) : Upscaling factor for predictions. Choose a power of 2 for best results. Default is 4.
 
-            depth (int) : Number of hidden layers per decoder residual block. Default is 3.
-            
+            depth (int) : Number of hidden layers per residual block. Default is 3.
+
             dilations (list[list[int]]) : List of dilation values per layer. If value is None, atrous convolutions will not be used. Default is None.
 
             pool_sizes (list[int]) : Pooling ratios for PSP pooling. If value is None, PSP pooling will not be used. Default is None.
 
             encoder_pool (bool) : Whether to include additional PSP pooling layer at end of encoder. Should not be used if last layer has a size of less than 16 pixels. Default is False.
-
-            rdnet_kwargs (dict[str, Any]) : Keyword arguments for RDNet. Default is None.
         """
         super().__init__()
-        rdnet_kwargs = {} if rdnet_kwargs is None else rdnet_kwargs
         channels = _force_list(channels)
         channels = channels*2 if len(channels) == 1 else channels
 
         if dilations and len(dilations) != len(hidden): raise ValueError(f"Amount of dilations must equal amount of hidden residual blocks. Given values are {len(dilations)} and {len(hidden)} respectively.")
 
         if pool_sizes:
             if hidden[0] % len(pool_sizes) != 0: raise ValueError(f"hidden[0] must be divisible by len(pool_sizes). Given values are {hidden[0]} and {len(pool_sizes)} respectively.")
             if encoder_pool and hidden[-1] % len(pool_sizes) != 0: raise ValueError(f"hidden[-1] must be divisible by len(pool_sizes) if encoder_pool is True. Given values are {hidden[-1]} and {len(pool_sizes)} respectively.")
         else:
             if encoder_pool: raise ValueError(f"encoder_pool cannot be True if pool_sizes are not provided.")
 
         self.norm = nn.BatchNorm2d(channels[0]) if not dilations else None
 
-        self.encoder = RDNet(in_channels=channels[0], **rdnet_kwargs)
-        skips = [feature["num_chs"] for feature in self.encoder.feature_info]
-        skips.reverse()
-
-        if len(skips) != len(hidden): raise ValueError(f"Each encoder skip connection must have a corresponding decoder hidden layer. There are {len(skips)} skip connections but {len(hidden)} hidden layers.")
-        
-        self.ratios = [1] + [2]*(len(skips)-1) + [rdnet_kwargs.get("patch_size", 2)]
-
-        layers = [0, *hidden]
-        self.decoder = nn.ModuleList()
-        for layer_idx in range(len(layers)-1):
-            self.decoder.append(get_resblock(in_channels=layers[layer_idx]//self.ratios[layer_idx]**2+skips[layer_idx], out_channels=layers[layer_idx+1], dilations=dilations[layer_idx] if dilations else None, depth=depth))
+        self.encoder, self.decoder = nn.ModuleList(), nn.ModuleList()
+        layers = [channels[0], *hidden]
+        n_layers = len(layers) - 1
+        for layer_idx in range(n_layers):
+            self.encoder.append(get_resblock(in_channels=layers[layer_idx], out_channels=layers[layer_idx+1], dilations=dilations[layer_idx] if dilations else None, depth=depth))
+            if layer_idx + 1 < n_layers:
+                self.decoder.append(get_resblock(in_channels=layers[-layer_idx-1]-int(layers[-layer_idx-2]/2), out_channels=layers[-layer_idx-2], dilations=dilations[-layer_idx-1] if dilations else None, depth=depth))
 
-        self.encoder_pool = PSP_Pooling(skips[0], pool_sizes) if pool_sizes and encoder_pool else None
-        self.reconstruction_pool = PSP_Pooling(hidden[-1]//self.ratios[-1]**2, pool_sizes) if pool_sizes else None
+        self.encoder_pool = PSP_Pooling(hidden[-1], pool_sizes) if pool_sizes and encoder_pool else None
+        self.reconstruction_pool = PSP_Pooling(hidden[0], pool_sizes) if pool_sizes else None
 
-        self.reconstruction = Reconstruction(channels[0], channels[1], hidden[-1]//self.ratios[-1]**2, scale)
-
-        self.skips = skips
+        self.reconstruction = Reconstruction(channels[0], channels[1], hidden[0], scale)
 
     def forward(self, x):
         x = x / 128 - 1 # Scale input approx from [0, 255] to [-1, 1]
         if self.norm is not None:
             x = self.norm(x)
 
         skips = [x]
-        skips.extend(self.encoder(x))
+        for idx, layer in enumerate(self.encoder):
+            x = layer(x) # ResBlock
+
+            if idx + 1 < len(self.encoder): # Downscale
+                skips.append(x)
+                x = F.max_pool2d(x, kernel_size=2)
 
         if self.encoder_pool is not None:
-            skips[-1] = self.encoder_pool(skips[-1])
+            x = self.encoder_pool(x)
 
         for idx, layer in enumerate(self.decoder):
-            x = torch.cat([x, skips.pop()], dim=1) if idx != 0 else skips.pop()
+            x = x = F.pixel_shuffle(x, 2) # Upscale
+
+            x = torch.cat([x, skips.pop()], dim=1) # ResBlock
             x = layer(x)
 
-            x = F.pixel_shuffle(x, self.ratios[idx+1])
-        
         if self.reconstruction_pool is not None:
             x = self.reconstruction_pool(x)
-        
-        x = torch.cat([x, skips.pop()], dim=1)
+
+        x = torch.cat([x, skips.pop()], dim=1) # Final skip connection before reconstruction
         if len(skips) != 0: raise IndexError(f"Skip connection mismatch between encoder and decoder. {len(skips)} skip connections are unused.")
 
         x = self.reconstruction(x)
 
         x = x * 128 + 128 # Scale output approx from [-1, 1] to [0, 255]
         return x
-
+    
     def extra_repr(self):
-        return f"{'Atrous ' if self.norm is None else ''}RDResUNet with {self.reconstruction.scale}x upscaling\nSkip connection sizes: {self.skips}\n{len(self.decoder)} residual blocks with {self.decoder[0].depth} hidden layers each\nPSP pooling {'enabled' if self.reconstruction_pool else 'disabled'}"
+        return f"{'Atrous ' if self.norm is None else ''}ResUNet with {self.reconstruction.scale}x upscaling\n{len(self.encoder)} residual decoder blocks with {self.encoder[0].depth} hidden layers each\nPSP pooling {'enabled' if self.reconstruction_pool else 'disabled'}"
 
-class RDResUNetA():
+class ResUNetA():
     def __new__(cls,
             channels : int = 1,
-            hidden : list[int] = [1024, 1024, 512, 256],
+            hidden : list[int] = [64, 128, 256, 512, 1024],
             scale : int = 4,
             depth : int = 3,
-            dilations : list[list[int]] = [[1],[1],[1,3],[1,3,15]],
+            dilations : list[list[int]] = [[1,3,15,31],[1,3,15],[1,3],[1],[1]],
             pool_sizes : list[int] = [1, 2, 4, 8],
             encoder_pool : bool = False,
-            rdnet_kwargs = None
         ):
-        r""":class:`RDResUNet` wrapper of Atrous Residual UNet as detailed in Diakogiannis et al., 2019.
+        r""":class:`ResUNet` wrapper of Atrous Residual UNet as detailed in Diakogiannis et al., 2019.
         Provides alternative default arguments for an atrous network.
 
         Channel sizes hidden[0] (and hidden[-1] if encoder_pool is True) must be divisible by pool_sizes.
 
         Args:
             channels (int) : Number of channels in image data. Can also be a list of in channels and out channels respectively.
 
-            hidden (list[int]) : Elementwise list of hidden layer channels of ResUNet decoder. Each element must have a corresponding skip connection in the RDNet encoder, provided after each downsample block.
+            hidden (list[int]) : Elementwise list of channels per residual block controlling width and length of model.
 
             scale (int) : Upscaling factor for predictions. Choose a power of 2 for best results. Default is 4.
 
-            depth (int) : Number of hidden layers per decoder residual block. Default is 3.
-            
-            dilations (list[list[int]]) : List of dilation values per layer. If value is None, atrous convolutions will not be used. Default is [[1,3,15],[1,3],[1],[1]].
+            depth (int) : Number of hidden layers per residual block. Default is 3.
+
+            dilations (list[list[int]]) : List of dilation values per layer. If value is None, atrous convolutions will not be used. Default is [[1,3,15,31],[1,3,15],[1,3],[1],[1]].
 
             pool_sizes (list[int]) : Pooling ratios for PSP pooling. If value is None, PSP pooling will not be used. Default is [1, 2, 4, 8].
 
             encoder_pool (bool) : Whether to include additional PSP pooling layer at end of encoder. Should not be used if last layer has a size of less than 16 pixels. Default is False.
-
-            rdnet_kwargs (dict[str, Any]) : Keyword arguments for RDNet. Default is None.
         """
-        return RDResUNet(
+        return ResUNet(
             channels,
             hidden,
             scale,
             depth,
             dilations,
             pool_sizes,
             encoder_pool,
-            rdnet_kwargs,
         )
```

### Comparing `pssr-1.2.2/pssr/models/swinir.py` & `pssr-2.0.0/pssr/models/swinir.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.checkpoint as checkpoint
 from timm.layers import DropPath, to_2tuple, trunc_normal_
-from ..data import _force_list
+from ..util import _force_list
 
 class SwinIR(nn.Module):
     def __init__(
             self,
-            img_size : int = 128,
-            channels : int = 1,
+            image_size : int = 128,
+            channels : list[int] = 1,
             scale : int = 4,
             embed_dim : int = 96,
             mlp_ratio : int = 2,
             depths : list[int] = [4, 4, 4, 4],
             num_heads : list[int] = [6, 6, 6, 6],
             window_size : int = 8,
             patch_size : int = 1,
@@ -36,17 +36,17 @@
             patch_norm : bool = True,
             use_checkpoint : bool = False,
             resi_connection : str = "1conv",
         ):
         """SwinIR as detailed in Liang et al., 2021.
         
         Args:
-            img_size (int) : Input image size. 
+            image_size (int) : Input image size. 
 
-            channels (int) : Number of channels in image data. Can also be a list of in channels and out channels respectively.
+            channels (list[int]) : Number of channels in image data. Can also be a list of in channels (low-resolution) and out channels (high-resolution) respectively.
 
             scale (int) : Upscaling factor for predictions. Choose a power of 2 for best results. Default is 4.
 
             embed_dim (int) : Number of channels in patch embedding dimension. Default is 96.
 
             mlp_ratio (int) : Ratio of hidden channels to embedding channels. Default is 2.
 
@@ -66,15 +66,15 @@
 
             drop_rate (float) : Dropout rate during training. Default is 0.
 
             attn_drop_rate (float) : Attention dropout rate during training. Default is 0.
 
             drop_path_rate (float) : Stochastic depth rate. Default is 0.1.
 
-            norm_layer (nn.Module) : Normalization layer. Default is nn.LayerNorm.
+            norm_layer (nn.Module) : Data normalization layer. Default is :class:`nn.LayerNorm`.
 
             ape (bool) : Whether to add absolute position embedding to patch embedding. Default is False.
 
             patch_norm (bool) : Whether to use normalization after patch embedding. Default is False.
 
             use_checkpoint (bool) : Whether to use checkpointing to save memory. Default is False.
 
@@ -108,23 +108,23 @@
         self.ape = ape
         self.patch_norm = patch_norm
         self.num_features = embed_dim
         self.mlp_ratio = mlp_ratio
 
         # split image into non-overlapping patches
         self.patch_embed = PatchEmbed(
-            img_size=img_size, patch_size=patch_size, in_chans=embed_dim, embed_dim=embed_dim,
+            img_size=image_size, patch_size=patch_size, in_chans=embed_dim, embed_dim=embed_dim,
             norm_layer=norm_layer if self.patch_norm else None)
         num_patches = self.patch_embed.num_patches
         patches_resolution = self.patch_embed.patches_resolution
         self.patches_resolution = patches_resolution
 
         # merge non-overlapping patches into image
         self.patch_unembed = PatchUnEmbed(
-            img_size=img_size, patch_size=patch_size, in_chans=embed_dim, embed_dim=embed_dim,
+            img_size=image_size, patch_size=patch_size, in_chans=embed_dim, embed_dim=embed_dim,
             norm_layer=norm_layer if self.patch_norm else None)
 
         # absolute position embedding
         if self.ape:
             self.absolute_pos_embed = nn.Parameter(torch.zeros(1, num_patches, embed_dim))
             trunc_normal_(self.absolute_pos_embed, std=.02)
```

### Comparing `pssr-1.2.2/pssr/predict.py` & `pssr-2.0.0/pssr/predict.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import numpy as np
 from torch.utils.data import Dataset
 from skimage.metrics import peak_signal_noise_ratio, structural_similarity
 from skimage.transform import resize
 from tqdm import tqdm
 from PIL import Image
 from .data import _RandomIterIdx, _slice_center
-from .loss import pixel_metric
+from .util import _get_callbacks, pixel_metric
 
-def predict_images(model : nn.Module, dataset : Dataset, device : str = "cpu", norm : bool = False, prefix : str = None, out_dir : str = "preds"):
+def predict_images(model : nn.Module, dataset : Dataset, device : str = "cpu", norm : bool = False, prefix : str = None, out_dir : str = "preds", callbacks = None):
     r"""Predicts high-resolution images from low-resolution images using a given model.
     
     Only uses evaluation images if applicable. Set ``val_split=1`` in dataset to use all images.
 
     Args:
         model (nn.Module) : Model to recieve low-resolution images.
 
@@ -22,20 +22,24 @@
         device (str) : Device to train model on. Default is "cpu".
 
         norm (bool) : Whether to normalize prediction image intensities to ground truth, which must be provided by a paired dataset. Default is False.
 
         prefix (str) : Prefix to append at the beginning the output file name. Default is None.
 
         out_dir (str) : Directory to save images. A value of None returns images. Default is "preds".
+
+        callbacks (list[Callable]) : Callbacks after each prediction. Can optionally specify an argument for locals to be passed. Default is None.
     
     Returns:
         images (list[np.ndarray]) : Returns predicted images if ``out_dir`` is None.
     """
     if norm and dataset.is_lr: raise ValueError("Dataset must be paired with high-low-resolution images for normalization.")
 
+    callbacks, callback_locals = _get_callbacks(callbacks)
+
     model.to(device)
     model.eval()
 
     progress = tqdm(dataset.val_idx)
     outs = []
     with torch.no_grad():
         for idx in progress:
@@ -48,22 +52,28 @@
             if norm:
                 _, hr_hat = normalize_preds(_pred_array(dataset[idx][0]), hr_hat)
 
             crop_res = dataset.crop_res if not dataset.is_lr else dataset.crop_res * (hr_hat.shape[-1]//lr.shape[-1])
             hr_hat = hr_hat[:,:crop_res,:crop_res]
             outs.append(hr_hat)
 
+            for idx, callback in enumerate(callbacks):
+                if callback_locals[idx]:
+                    callback(locals())
+                else:
+                    callback()
+
     if out_dir:
         os.makedirs(out_dir, exist_ok=True)
         for idx, hr_hat in enumerate(outs):
             tifffile.imwrite(f"{out_dir}/{prefix+'_' if prefix else ''}{dataset._get_name(idx)}.tif", np.asarray(hr_hat))
     else:
         return outs
 
-def predict_collage(model : nn.Module, dataset : Dataset, device : str = "cpu", norm : bool = True, n_images : int = None, prefix : str = None, out_dir : str = "preds"):
+def predict_collage(model : nn.Module, dataset : Dataset, device : str = "cpu", norm : bool = True, n_images : int = None, prefix : str = None, out_dir : str = "preds", callbacks = None):
     r"""Saves to file an image collage of vertically stacked instances of horizontally aligned low-resolution, PSSR upscaled, and high-resolution images in that order.
     Only the center frame of each slice is displayed.
 
     Only uses evaluation images if applicable. Set ``val_split=1`` in dataset to use all images.
 
     Args:
         model (nn.Module) : Model to recieve low-resolution images.
@@ -75,39 +85,49 @@
         norm (bool) : Whether to normalize prediction image intensities to ground truth. Default is True.
 
         n_images (int) : Number of images to concatenate. Set to None to use all validation images, maximum 50. Default is None.
 
         prefix (str) : Prefix to append at the beginning the output file name. Default is None.
 
         out_dir (str) : Directory to save collage. Default is "preds".
+
+        callbacks (list[Callable]) : Callbacks after each prediction. Can optionally specify an argument for locals to be passed. Default is None.
     """
     if dataset.is_lr: raise ValueError("Dataset cannot be in LR mode when creating a collage.")
 
+    callbacks, callback_locals = _get_callbacks(callbacks)
     n_images = min(50, len(dataset)) if n_images is None else n_images
 
     model.to(device)
     model.eval()
 
     collage = Image.new("L", (dataset.crop_res*3, dataset.crop_res*n_images))
     with torch.no_grad():
-        for idx, data_idx in enumerate(_RandomIterIdx(dataset.val_idx, seed=True)):
+        # Only shuffle if val_split < 1
+        for idx, data_idx in enumerate(_RandomIterIdx(dataset.val_idx, seed=True) if len(dataset.val_idx) < len(dataset) else dataset.val_idx):
             hr, lr = dataset[data_idx]
             hr, lr = hr.to(device).unsqueeze(0), lr.to(device).unsqueeze(0)
 
             hr_hat = model(lr)
 
             collage.paste(_collage_preds(lr, hr_hat, hr, norm, 1, dataset.crop_res, dataset.lr_scale), (0, dataset.crop_res*idx))
 
+            for idx, callback in enumerate(callbacks):
+                if callback_locals[idx]:
+                    callback(locals())
+                else:
+                    callback()
+
             if idx >= n_images - 1:
                 break
 
     os.makedirs(out_dir, exist_ok=True)
     collage.save(f"{out_dir}/{prefix+'_' if prefix else ''}collage_{n_images}.png")
 
-def test_metrics(model : nn.Module, dataset : Dataset, device : str = "cpu", metrics : list[str] = ["mse", "pixel", "psnr", "ssim"], avg : bool = True, norm : bool = True):
+def test_metrics(model : nn.Module, dataset : Dataset, device : str = "cpu", metrics : list[str] = ["mse", "pixel", "psnr", "ssim"], avg : bool = True, norm : bool = True, callbacks = None):
     r"""Computes image restoration metrics of predicted vs ground truth images.
 
     Only uses evaluation images if applicable. Set ``val_split=1`` in dataset to use all images.
 
     Args:
         model (nn.Module) : Model to recieve low-resolution images.
 
@@ -116,18 +136,21 @@
         device (str) : Device to train model on. Default is "cpu".
 
         metrics (list[str]) : Metrics to calculate out of "mse", "pixel", "psnr", and "ssim". Default is all.
 
         avg (bool) : Whether to return a single averaged value per metric. Default is True.
 
         norm (bool) : Whether to normalize prediction image intensities to ground truth. Default is True.
+
+        callbacks (list[Callable]) : Callbacks after each prediction. Can optionally specify an argument for locals to be passed. Default is None.
     
     Returns:
         metrics (dict[str, Any]) : Dictionary of metric names and outputs.
     """
+    callbacks, callback_locals = _get_callbacks(callbacks)
     image_range = 255
 
     metrics = [metrics] if type(metrics) is str else metrics
     metrics = {metric:[] for metric in metrics}
     use_mse = True if any(x in metrics.keys() for x in ["mse", "pixel"]) else False
 
     model.to(device)
@@ -156,14 +179,20 @@
                     metrics["mse"].append(mse)
                 if "pixel" in metrics:
                     metrics["pixel"].append(pixel_metric(mse, image_range))
                 if "psnr" in metrics:
                     metrics["psnr"].append(peak_signal_noise_ratio(hr[idx], hr_hat[idx], data_range=image_range))
                 if "ssim" in metrics:
                     metrics["ssim"].append(structural_similarity(hr[idx].squeeze(), hr_hat[idx].squeeze(), data_range=image_range))
+            
+            for idx, callback in enumerate(callbacks):
+                if callback_locals[idx]:
+                    callback(locals())
+                else:
+                    callback()
 
     return {metric:(sum(values)/len(values) if avg else values) for metric, values in metrics.items()}
 
 def normalize_preds(hr : np.ndarray, hr_hat : np.ndarray, pmin : float = 0.1, pmax : float = 99.9):
     r"""Normalizes prediction image intensities to ground truth for fair benchmarking.
 
     Args:
```

### Comparing `pssr-1.2.2/pssr/train.py` & `pssr-2.0.0/pssr/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pytorch_msssim import ssim
 from skopt import gp_minimize
 from skopt.space import Dimension
 from tqdm import tqdm
 from PIL import Image
 from .crappifiers import Crappifier
 from .data import _RandomIterIdx, _invert_idx
-from .loss import SSIMLoss, pixel_metric, _psnr_metric
+from .util import SSIMLoss, _get_callbacks, pixel_metric, _psnr_metric
 from .predict import _collage_preds
 from .models._blocks import GradHist
 
 Image.MAX_IMAGE_PIXELS = None
 
 def train_paired(
         model : nn.Module,
@@ -25,15 +25,16 @@
         epochs : int,
         device : str = "cpu",
         scheduler : torch.optim.lr_scheduler = None,
         log_frequency : int = 50,
         checkpoint_dir : str = None,
         collage_dir : str = None,
         clamp : bool = False,
-        dataloader_kwargs = None
+        dataloader_kwargs = None,
+        callbacks = None,
     ):
     r"""Trains model on paired high-low-resolution crappified data.
 
     Args:
         model (nn.Module) : Model to train on paired data.
 
         dataset (Dataset) : Paired image dataset to load data from.
@@ -56,24 +57,28 @@
 
         collage_dir (str) : Directory to save validation collages each epoch. A value of None skips the collage. Default is None.
 
         clamp (bool) : Whether to clamp model image output before weight calculation. Default is False.
 
         dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch ``Dataloader``. Default is None.
 
+        callbacks (list[Callable]) : Callbacks after each training batch. Can optionally specify an argument for locals to be passed. Default is None.
+
     Returns:
         train_losses (list[float]) : List of losses during training.
 
         val_losses (list[float]) : Validation losses per epoch.
     """
     dataloader_kwargs = {} if dataloader_kwargs is None else dataloader_kwargs
+    callbacks, callback_locals = _get_callbacks(callbacks)
+    image_range = 255
+
     train_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(_invert_idx(dataset.val_idx, len(dataset))), **dataloader_kwargs)
     val_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(dataset.val_idx, seed=True), **dataloader_kwargs)
     include_metric = True if type(scheduler) == torch.optim.lr_scheduler.ReduceLROnPlateau else False
-    image_range = 255
 
     model.to(device)
 
     train_losses, val_losses = [], []
     for epoch in range(epochs):
         # Train
         model.train()
@@ -93,43 +98,56 @@
             optim.zero_grad()
 
             if batch_idx % log_frequency == 0 or batch_idx == len(progress) - 1:
                 train_losses.append(loss.item())
 
                 mse = nn.functional.mse_loss(hr_hat/image_range, hr/image_range)
                 progress.set_description(f"pixel[{pixel_metric(mse, image_range):.2f}], psnr[{_psnr_metric(mse):.2f}], ssim[{ssim(hr_hat, hr, data_range=image_range):.3f}]")
+            
+            if batch_idx == max(len(progress), 2) - 2:
+                # Accessible from callbacks via locals
+                last_full = [lr.cpu(), hr_hat.cpu(), hr.cpu()]
+            
+            for idx, callback in enumerate(callbacks):
+                if callback_locals[idx]:
+                    callback(locals())
+                else:
+                    callback()
 
         # Validation
         model.eval()
+        print(f"Epoch {epoch} validation...")
 
         val_loss = []
         progress = tqdm(val_dataloader)
-        progress.set_description(f"Epoch {epoch} validation...")
 
         with torch.no_grad():
-            for hr, lr in progress:
+            for batch_idx, (hr, lr) in enumerate(progress):
                 hr, lr = hr.to(device), lr.to(device)
 
                 hr_hat = model(lr)
                 if clamp:
                     hr_hat = torch.clamp(hr_hat, 0, image_range)
 
                 loss = loss_fn(hr_hat/image_range, hr/image_range)
                 val_loss.append(loss.item())
 
+                if batch_idx == max(len(progress), 2) - 2:
+                    last_full_val = [lr.cpu(), hr_hat.cpu(), hr.cpu()]
+
         val_loss = sum(val_loss) / len(val_loss)
         val_losses.append(val_loss)
         print(f"Epoch {epoch} validation loss: {val_loss:4f}\n")
 
         if checkpoint_dir and epoch < epochs - 1:
             os.makedirs(checkpoint_dir, exist_ok=True)
             torch.save(model.state_dict(), f"{checkpoint_dir}/checkpoint{epoch}_{model.__class__.__name__}_{val_loss:.4f}.pth")
 
         if collage_dir:
-            collage = _collage_preds(lr, hr_hat, hr, crop_res=dataset.crop_res, lr_scale=dataset.lr_scale)
+            collage = _collage_preds(*last_full_val, crop_res=dataset.crop_res, lr_scale=dataset.lr_scale)
             os.makedirs(collage_dir, exist_ok=True)
             collage.save(f"{collage_dir}/epoch{epoch}_loss{val_loss:.4f}.png")
 
         if scheduler:
             if include_metric:
                 scheduler.step(val_loss)
             else:
@@ -184,26 +202,30 @@
 
         collage_dir (str) : Directory to save validation collages each epoch. A value of None skips the collage. Default is None.
 
         clamp (bool) : Whether to clamp model image output before weight calculation. Default is False.
 
         dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch ``Dataloader``. Default is None.
 
+        callbacks (list[Callable]) : Callbacks after each training batch. Can optionally specify an argument for locals to be passed. Default is None.
+
     Returns:
         train_losses (list[float]) : List of losses during training.
 
         val_losses (list[float]) : Validation losses per epoch.
     """
     dataloader_kwargs = {} if dataloader_kwargs is None else dataloader_kwargs
+    callbacks, callback_locals = _get_callbacks(callbacks)
+    image_range = 255
+
     train_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(_invert_idx(dataset.val_idx, len(dataset))), **dataloader_kwargs)
     val_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(dataset.val_idx, seed=True), **dataloader_kwargs)
     include_metric = True if type(scheduler) == torch.optim.lr_scheduler.ReduceLROnPlateau else False
 
     model.to(device)
-    model.train()
 
     # Leave on cpu?
     hist_fn = GradHist(sigma=sigma)
     ssim_loss = SSIMLoss(ms=False)
 
     train_losses, val_losses = [], []
     for epoch in range(epochs):
@@ -215,15 +237,15 @@
         for batch_idx, (hr, lr) in enumerate(progress):
             scale = int(hr.shape[-1]/lr.shape[-1])
             ds_hr = hr[:, :, ::scale, ::scale]
             ds_hr = ds_hr.to(device)
 
             lr_hat = model(ds_hr)
             if clamp:
-                lr_hat = torch.clamp(lr_hat, 0, 255)
+                lr_hat = torch.clamp(lr_hat, 0, image_range)
 
             loss = _crappifier_loss(lr.to(device), lr_hat, ds_hr, hist_fn, ssim_loss)
             loss.backward()
 
             if clip is not None and clip > 0:
                 nn.utils.clip_grad_value_(model.parameters(), clip)
 
@@ -231,44 +253,57 @@
             optim.zero_grad()
 
             if batch_idx % log_frequency == 0 or batch_idx == len(progress) - 1:
                 train_losses.append(loss.item())
 
                 progress.set_description(f"loss[{loss.item():.4f}]")
 
+            if batch_idx == max(len(progress), 2) - 2:
+                # Accessible from callbacks via locals
+                last_full = [lr.cpu(), lr_hat.cpu(), hr.cpu()]
+
+            for idx, callback in enumerate(callbacks):
+                if callback_locals[idx]:
+                    callback(locals())
+                else:
+                    callback()
+
         # Validation
         model.eval()
+        print(f"Epoch {epoch} validation...")
 
         val_loss = []
         progress = tqdm(val_dataloader)
-        progress.set_description(f"Epoch {epoch} validation...")
 
         with torch.no_grad():
-            for hr, lr in progress:
+            for batch_idx, (hr, lr) in enumerate(progress):
                 scale = int(hr.shape[-1]/lr.shape[-1])
                 ds_hr = hr[:, :, ::scale, ::scale]
                 ds_hr = ds_hr.to(device)
 
                 lr_hat = model(ds_hr)
                 if clamp:
-                    lr_hat = torch.clamp(lr_hat, 0, 255)
+                    lr_hat = torch.clamp(lr_hat, 0, image_range)
 
                 loss = _crappifier_loss(lr.to(device), lr_hat, ds_hr, hist_fn, ssim_loss)
                 val_loss.append(loss.item())
 
+                if batch_idx == max(len(progress), 2) - 2:
+                    last_full_val = [lr.cpu(), lr_hat.cpu(), hr.cpu()]
+
         val_loss = sum(val_loss) / len(val_loss)
         val_losses.append(val_loss)
         print(f"Epoch {epoch} validation loss: {val_loss:4f}\n")
 
         if checkpoint_dir and epoch < epochs - 1:
             os.makedirs(checkpoint_dir, exist_ok=True)
             torch.save(model.state_dict(), f"{checkpoint_dir}/checkpoint{epoch}_{model.__class__.__name__}_{val_loss:.4f}.pth")
 
         if collage_dir:
-            collage = _collage_preds(lr, lr_hat, hr, crop_res=dataset.crop_res, lr_scale=dataset.lr_scale)
+            collage = _collage_preds(*last_full_val, crop_res=dataset.crop_res, lr_scale=dataset.lr_scale)
             os.makedirs(collage_dir, exist_ok=True)
             collage.save(f"{collage_dir}/epoch{epoch}_loss{val_loss:.4f}.png")
 
         if scheduler:
             if include_metric:
                 scheduler.step(val_loss)
             else:
```

### Comparing `pssr-1.2.2/pyproject.toml` & `pssr-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 [tool.poetry]
 name = "pssr"
-version = "1.2.2"
+version = "2.0.0"
 description = "Point-Scanning Super-Resolution"
 authors = ["Hayden Stites"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/ucsdmanorlab/PSSR"
 documentation = "https://ucsdmanorlab.github.io/PSSR/"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Environment :: GPU :: NVIDIA CUDA",
+    "Framework :: napari",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Documentation :: Sphinx",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 torch = ">=1.11.0"
 numpy = "^1.22.4"
 pillow = ">=9.1.0"
 czifile = "^2019.7.2"
 tifffile = ">=2019.7.26"
 scikit-image = ">=0.18.0"
 scikit-optimize = ">=0.9.0"
 tqdm = "^4.0.0"
 pytorch-msssim = "^1.0.0"
 psutil = ">=5.0.0"
 timm = ">=0.8.0"
 
+napari = {version = "^0.4.13", optional = true}
+
+[tool.poetry.extras]
+napari = ["napari"]
+
 [tool.poetry.scripts]
 pssr = "pssr.__main__:main"
 
+[tool.poetry.plugins."napari.manifest"]
+pssr = "pssr.napari:napari.yaml"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pssr-1.2.2/PKG-INFO` & `pssr-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: pssr
-Version: 1.2.2
+Version: 2.0.0
 Summary: Point-Scanning Super-Resolution
 Home-page: https://github.com/ucsdmanorlab/PSSR
 License: MIT
 Author: Hayden Stites
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU :: NVIDIA CUDA
+Classifier: Framework :: napari
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
+Provides-Extra: napari
 Requires-Dist: czifile (>=2019.7.2,<2020.0.0)
+Requires-Dist: napari (>=0.4.13,<0.5.0) ; extra == "napari"
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pillow (>=9.1.0)
 Requires-Dist: psutil (>=5.0.0)
 Requires-Dist: pytorch-msssim (>=1.0.0,<2.0.0)
 Requires-Dist: scikit-image (>=0.18.0)
 Requires-Dist: scikit-optimize (>=0.9.0)
 Requires-Dist: tifffile (>=2019.7.26)
@@ -40,10 +44,10 @@
 containing various improvements and new features.
 
 The **PSSR** User Guide and full API Reference is available in the [PSSR Documentation](https://ucsdmanorlab.github.io/PSSR).
 
 If you have never used **PSSR** before, [Getting Started](https://ucsdmanorlab.github.io/PSSR/guide/start.html) outlines installation and basic usage.
 Full reference and explanations of all **PSSR** tools is available in [API Reference](https://ucsdmanorlab.github.io/PSSR/reference/api.html).
 
-The package is still in development. All code can be found at [https://github.com/ucsdmanorlab/PSSR](https://github.com/ucsdmanorlab/PSSR).
+This package is under continuous development. All code can be found at [https://github.com/ucsdmanorlab/PSSR](https://github.com/ucsdmanorlab/PSSR).
 If you experience any bugs, unexpected behaviors, or have any suggestions, make sure to [open a ticket](https://github.com/ucsdmanorlab/PSSR/issues).
```

