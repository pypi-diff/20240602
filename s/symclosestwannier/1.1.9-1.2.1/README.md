# Comparing `tmp/symclosestwannier-1.1.9.tar.gz` & `tmp/symclosestwannier-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symclosestwannier-1.1.9.tar", last modified: Sun Feb  4 15:55:13 2024, max compression
+gzip compressed data, was "symclosestwannier-1.2.1.tar", last modified: Sun Jun  2 14:55:58 2024, max compression
```

## Comparing `symclosestwannier-1.1.9.tar` & `symclosestwannier-1.2.1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.292865 symclosestwannier-1.1.9/
--rw-r--r--   0 ro         (501) staff       (20)    18092 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/LICENSE
--rw-r--r--   0 ro         (501) staff       (20)       57 2023-12-19 03:46:59.000000 symclosestwannier-1.1.9/MANIFEST.in
--rw-r--r--   0 ro         (501) staff       (20)     2542 2024-02-04 15:55:13.292788 symclosestwannier-1.1.9/PKG-INFO
--rw-r--r--   0 ro         (501) staff       (20)     1805 2023-12-19 03:54:41.000000 symclosestwannier-1.1.9/README.md
--rw-r--r--   0 ro         (501) staff       (20)      887 2024-02-04 15:55:13.293142 symclosestwannier-1.1.9/setup.cfg
--rw-r--r--   0 ro         (501) staff       (20)       38 2023-12-19 03:47:00.000000 symclosestwannier-1.1.9/setup.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.283915 symclosestwannier-1.1.9/symclosestwannier/
--rw-r--r--   0 ro         (501) staff       (20)      106 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/__init__.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.287405 symclosestwannier-1.1.9/symclosestwannier/analyzer/
--rw-r--r--   0 ro         (501) staff       (20)     3455 2024-01-22 00:23:53.000000 symclosestwannier-1.1.9/symclosestwannier/analyzer/analyzer.py
--rw-r--r--   0 ro         (501) staff       (20)     4715 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/symclosestwannier/analyzer/band.py
--rw-r--r--   0 ro         (501) staff       (20)     1779 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/symclosestwannier/analyzer/get_band.py
--rw-r--r--   0 ro         (501) staff       (20)    18822 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/analyzer/get_response.py
--rw-r--r--   0 ro         (501) staff       (20)     9136 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/analyzer/response.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.290222 symclosestwannier-1.1.9/symclosestwannier/cw/
--rw-r--r--   0 ro         (501) staff       (20)     2807 2024-01-24 13:49:38.000000 symclosestwannier-1.1.9/symclosestwannier/cw/amn.py
--rw-r--r--   0 ro         (501) staff       (20)     8487 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/cw_creator.py
--rw-r--r--   0 ro         (501) staff       (20)     7116 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/cw_info.py
--rw-r--r--   0 ro         (501) staff       (20)     5529 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/symclosestwannier/cw/cw_manager.py
--rw-r--r--   0 ro         (501) staff       (20)    40198 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/cw_model.py
--rw-r--r--   0 ro         (501) staff       (20)     8123 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/cwin.py
--rw-r--r--   0 ro         (501) staff       (20)     3336 2024-01-31 04:41:33.000000 symclosestwannier-1.1.9/symclosestwannier/cw/eig.py
--rw-r--r--   0 ro         (501) staff       (20)     5137 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/mmn.py
--rw-r--r--   0 ro         (501) staff       (20)    11484 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/nnkp.py
--rw-r--r--   0 ro         (501) staff       (20)     5985 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/symclosestwannier/cw/spn.py
--rw-r--r--   0 ro         (501) staff       (20)     9558 2024-02-01 04:44:14.000000 symclosestwannier-1.1.9/symclosestwannier/cw/umat.py
--rw-r--r--   0 ro         (501) staff       (20)    18360 2024-02-04 08:23:06.000000 symclosestwannier-1.1.9/symclosestwannier/cw/win.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.290920 symclosestwannier-1.1.9/symclosestwannier/scripts/
--rw-r--r--   0 ro         (501) staff       (20)     2420 2024-01-23 05:22:29.000000 symclosestwannier-1.1.9/symclosestwannier/scripts/postcw.py
--rw-r--r--   0 ro         (501) staff       (20)     2462 2024-01-23 05:22:29.000000 symclosestwannier-1.1.9/symclosestwannier/scripts/pw2cw.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.292301 symclosestwannier-1.1.9/symclosestwannier/util/
--rw-r--r--   0 ro         (501) staff       (20)    22461 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/util/_utility.py
--rw-r--r--   0 ro         (501) staff       (20)     4222 2023-12-19 03:47:00.000000 symclosestwannier-1.1.9/symclosestwannier/util/band.py
--rw-r--r--   0 ro         (501) staff       (20)     3357 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/symclosestwannier/util/constants.py
--rw-r--r--   0 ro         (501) staff       (20)     8296 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/util/get_oper_R.py
--rw-r--r--   0 ro         (501) staff       (20)    16238 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/util/header.py
--rw-r--r--   0 ro         (501) staff       (20)    10854 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/util/message.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.285825 symclosestwannier-1.1.9/symclosestwannier.egg-info/
--rw-r--r--   0 ro         (501) staff       (20)     2542 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/PKG-INFO
--rw-r--r--   0 ro         (501) staff       (20)     1160 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/SOURCES.txt
--rw-r--r--   0 ro         (501) staff       (20)        1 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/dependency_links.txt
--rw-r--r--   0 ro         (501) staff       (20)      108 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/entry_points.txt
--rw-r--r--   0 ro         (501) staff       (20)       81 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/requires.txt
--rw-r--r--   0 ro         (501) staff       (20)       18 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/top_level.txt
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-06-02 14:55:58.590520 symclosestwannier-1.2.1/
+-rw-r--r--   0 ro         (501) staff       (20)    18092 2023-12-19 03:50:00.000000 symclosestwannier-1.2.1/LICENSE
+-rw-r--r--   0 ro         (501) staff       (20)       57 2023-12-19 03:46:59.000000 symclosestwannier-1.2.1/MANIFEST.in
+-rw-r--r--   0 ro         (501) staff       (20)     3159 2024-06-02 14:55:58.590319 symclosestwannier-1.2.1/PKG-INFO
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-06-02 14:55:58.582365 symclosestwannier-1.2.1/docs/
+-rw-r--r--   0 ro         (501) staff       (20)     1765 2024-03-04 07:53:52.000000 symclosestwannier-1.2.1/docs/README.md
+-rw-r--r--   0 ro         (501) staff       (20)     1826 2024-02-13 14:49:00.000000 symclosestwannier-1.2.1/pyproject.toml
+-rw-r--r--   0 ro         (501) staff       (20)       38 2024-06-02 14:55:58.590560 symclosestwannier-1.2.1/setup.cfg
+-rw-r--r--   0 ro         (501) staff       (20)       38 2023-12-19 03:47:00.000000 symclosestwannier-1.2.1/setup.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-06-02 14:55:58.582475 symclosestwannier-1.2.1/symclosestwannier/
+-rw-r--r--   0 ro         (501) staff       (20)      106 2024-06-02 14:55:41.000000 symclosestwannier-1.2.1/symclosestwannier/__init__.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-06-02 14:55:58.584801 symclosestwannier-1.2.1/symclosestwannier/analyzer/
+-rw-r--r--   0 ro         (501) staff       (20)     3924 2024-03-17 09:34:47.000000 symclosestwannier-1.2.1/symclosestwannier/analyzer/analyzer.py
+-rw-r--r--   0 ro         (501) staff       (20)     4707 2024-02-19 10:25:40.000000 symclosestwannier-1.2.1/symclosestwannier/analyzer/band.py
+-rw-r--r--   0 ro         (501) staff       (20)     1779 2024-02-08 09:10:50.000000 symclosestwannier-1.2.1/symclosestwannier/analyzer/get_band.py
+-rw-r--r--   0 ro         (501) staff       (20)    46866 2024-03-29 00:02:44.000000 symclosestwannier-1.2.1/symclosestwannier/analyzer/get_response.py
+-rw-r--r--   0 ro         (501) staff       (20)    12624 2024-03-05 09:02:21.000000 symclosestwannier-1.2.1/symclosestwannier/analyzer/response.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-06-02 14:55:58.587773 symclosestwannier-1.2.1/symclosestwannier/cw/
+-rw-r--r--   0 ro         (501) staff       (20)     2884 2024-03-04 07:53:52.000000 symclosestwannier-1.2.1/symclosestwannier/cw/amn.py
+-rw-r--r--   0 ro         (501) staff       (20)     8634 2024-05-11 02:09:33.000000 symclosestwannier-1.2.1/symclosestwannier/cw/cw_creator.py
+-rw-r--r--   0 ro         (501) staff       (20)     8012 2024-03-04 07:53:52.000000 symclosestwannier-1.2.1/symclosestwannier/cw/cw_info.py
+-rw-r--r--   0 ro         (501) staff       (20)     5543 2024-03-04 07:53:52.000000 symclosestwannier-1.2.1/symclosestwannier/cw/cw_manager.py
+-rw-r--r--   0 ro         (501) staff       (20)    42287 2024-05-11 02:09:33.000000 symclosestwannier-1.2.1/symclosestwannier/cw/cw_model.py
+-rw-r--r--   0 ro         (501) staff       (20)     9566 2024-06-02 14:55:41.000000 symclosestwannier-1.2.1/symclosestwannier/cw/cwin.py
+-rw-r--r--   0 ro         (501) staff       (20)     3377 2024-03-04 07:53:52.000000 symclosestwannier-1.2.1/symclosestwannier/cw/eig.py
+-rw-r--r--   0 ro         (501) staff       (20)     5219 2024-03-04 07:53:52.000000 symclosestwannier-1.2.1/symclosestwannier/cw/mmn.py
+-rw-r--r--   0 ro         (501) staff       (20)    11956 2024-03-04 07:53:52.000000 symclosestwannier-1.2.1/symclosestwannier/cw/nnkp.py
+-rw-r--r--   0 ro         (501) staff       (20)     5873 2024-03-04 07:54:08.000000 symclosestwannier-1.2.1/symclosestwannier/cw/spn.py
+-rw-r--r--   0 ro         (501) staff       (20)    10061 2024-03-04 07:53:52.000000 symclosestwannier-1.2.1/symclosestwannier/cw/umat.py
+-rw-r--r--   0 ro         (501) staff       (20)    22508 2024-05-11 02:09:33.000000 symclosestwannier-1.2.1/symclosestwannier/cw/win.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-06-02 14:55:58.588159 symclosestwannier-1.2.1/symclosestwannier/scripts/
+-rw-r--r--   0 ro         (501) staff       (20)     2420 2024-02-19 10:26:47.000000 symclosestwannier-1.2.1/symclosestwannier/scripts/postcw.py
+-rw-r--r--   0 ro         (501) staff       (20)     2478 2024-03-04 07:53:52.000000 symclosestwannier-1.2.1/symclosestwannier/scripts/pw2cw.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-06-02 14:55:58.589726 symclosestwannier-1.2.1/symclosestwannier/util/
+-rw-r--r--   0 ro         (501) staff       (20)    28728 2024-06-02 14:32:28.000000 symclosestwannier-1.2.1/symclosestwannier/util/_utility.py
+-rw-r--r--   0 ro         (501) staff       (20)     4222 2024-02-08 09:10:50.000000 symclosestwannier-1.2.1/symclosestwannier/util/band.py
+-rw-r--r--   0 ro         (501) staff       (20)     2617 2024-02-13 14:49:00.000000 symclosestwannier-1.2.1/symclosestwannier/util/constants.py
+-rw-r--r--   0 ro         (501) staff       (20)     8302 2024-05-11 02:09:33.000000 symclosestwannier-1.2.1/symclosestwannier/util/get_oper_R.py
+-rw-r--r--   0 ro         (501) staff       (20)    17272 2024-03-05 08:41:58.000000 symclosestwannier-1.2.1/symclosestwannier/util/header.py
+-rw-r--r--   0 ro         (501) staff       (20)    11515 2024-03-05 08:53:03.000000 symclosestwannier-1.2.1/symclosestwannier/util/message.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-06-02 14:55:58.583134 symclosestwannier-1.2.1/symclosestwannier.egg-info/
+-rw-r--r--   0 ro         (501) staff       (20)     3159 2024-06-02 14:55:58.000000 symclosestwannier-1.2.1/symclosestwannier.egg-info/PKG-INFO
+-rw-r--r--   0 ro         (501) staff       (20)     1170 2024-06-02 14:55:58.000000 symclosestwannier-1.2.1/symclosestwannier.egg-info/SOURCES.txt
+-rw-r--r--   0 ro         (501) staff       (20)        1 2024-06-02 14:55:58.000000 symclosestwannier-1.2.1/symclosestwannier.egg-info/dependency_links.txt
+-rw-r--r--   0 ro         (501) staff       (20)      108 2024-06-02 14:55:58.000000 symclosestwannier-1.2.1/symclosestwannier.egg-info/entry_points.txt
+-rw-r--r--   0 ro         (501) staff       (20)       98 2024-06-02 14:55:58.000000 symclosestwannier-1.2.1/symclosestwannier.egg-info/requires.txt
+-rw-r--r--   0 ro         (501) staff       (20)       18 2024-06-02 14:55:58.000000 symclosestwannier-1.2.1/symclosestwannier.egg-info/top_level.txt
```

### Comparing `symclosestwannier-1.1.9/LICENSE` & `symclosestwannier-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.9/PKG-INFO` & `symclosestwannier-1.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,64 @@
 Metadata-Version: 2.1
 Name: symclosestwannier
-Version: 1.1.9
+Version: 1.2.1
 Summary: A Python library for Symmetry-Adapted Closest Wannier (SymCW) Tight-Binding model based on Plane-Wave DFT calculation.
-Home-page: https://github.com/CMT-MU/SymClosestWannier
-Author: Rikuto Oiwa
-Author-email: ro.qp.07@gmail.com
-License: MIT
+Author-email: Rikuto Oiwa <ro.qp.07@gmail.com>
+License: GPL
+Project-URL: Homepage, https://github.com/CMT-MU/SymClosestWannier
+Project-URL: Issues, https://github.com/CMT-MU/SymClosestWannier/issues
 Keywords: dft,wannier function,tight-binding model,symmetry,materials science
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gcoreutils
 Requires-Dist: multipie
 Requires-Dist: xmltodict
 Requires-Dist: fortio
 Requires-Dist: h5py
 Provides-Extra: dev
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: sphinx-rtd-theme; extra == "dev"
-Requires-Dist: ipython; extra == "dev"
+Requires-Dist: jupyter-book; extra == "dev"
+Requires-Dist: ghp-import; extra == "dev"
+Requires-Dist: jupytext; extra == "dev"
+Requires-Dist: multipie; extra == "dev"
+Requires-Dist: qtdraw; extra == "dev"
+
+# [SymClosestWannier](https://cmt-mu.github.io/SymClosestWannier/)
+
+- **Overview**:
+    A Python library to create Symmetry-adapted Closest Wannier (SymCW) tight-binding models based on the Symmetry-Adapted Multipole Basis (SAMB) [1] and the Closest Wannier formalism developed by Taisuke Ozaki [2].
+
+    > [1] Hiroaki Kusunose, Rikuto Oiwa, and Satoru Hayami, Symmetry-adapted modeling for molecules and crystals, Phys. Rev. B 107, 195118 (2023).
+    > DOI: https://doi.org/10.1103/PhysRevB.107.195118.<br>
+    > [2] Taisuke Ozaki, Closest Wannier functions to a given set of localized orbitals, arXiv:2306.15296, (2023).
+    > URL: https://arxiv.org/abs/2306.15296v2.
+
+- **Authors**: Rikuto Oiwa
+
+- **Installation**: SymClosestWannier can be installed from PyPI using pip on Python >= 3.9:
+    ```
+    pip install symclosestwannier
+    ```
+    You can also visit [PyPI](https://pypi.org/project/symclosestwannier/) or [GitHub](https://github.com/CMT-MU/SymClosestWannier/) to download the source.
+
+- **Citing SymClosestWannier**: If you are using SymClosestWannier in your scientific research, please help our scientific visibility by citing our work:
+
+    > Rikuto Oiwa, Akane Inda, Satoru Hayami, Takuya Nomoto, Ryotaro Arita, and Hiroaki Kusunose, in preparation.<br>
+    > DOI: []()
+
+- **Requirements**:
+  - Symmetry-Adapted Multipole Basis (SAMB) for molecular or crystal are optionally generated by [MultiPie](https://github.com/CMT-MU/MultiPie).
+  - MultiPie library optionally requires [TeXLive](https://www.tug.org/texlive/) environment to create LaTeX and PDF files.
+  - Molecular or crystal structure files are optionally generated by [QtDraw](https://github.com/CMT-MU/QtDraw).
 
-# SymClosestWannier
-
-A Python library to create Symmetry-adapted Closest Wannier (SymCW) tight-binding models based on the Symmetry-Adapted Multipole Basis (SAMB) [1] and the Closest Wannier formalism developed by Taisuke Ozaki [2].
-
-
-[1] Hiroaki Kusunose, Rikuto Oiwa, and Satoru Hayami, Symmetry-adapted modeling for molecules and crystals, Phys. Rev. B 107, 195118 (2023).
-
-DOI: https://doi.org/10.1103/PhysRevB.107.195118.
-
-[2] Taisuke Ozaki, Closest Wannier functions to a given set of localized orbitals, arXiv:2306.15296, (2023).
-
-URL: https://arxiv.org/abs/2306.15296v2.
-
-
-## Installation
-
-SymClosestWannier can be installed from PyPI using pip on Python >= 3.9:
-```
-pip install symclosestwannier
-```
-You can also visit [PyPI](https://pypi.org/project/symclosestwannier/) or [GitHub](https://github.com/CMT-MU/SymClosestWannier/) to download the source.
-
-
-## Authors
-
-Rikuto Oiwa
-
-
-## Citing SymClosestWannier
-
-If you are using SymClosestWannier in your scientific research, please help our scientific visibility by citing our work:
-
-> Rikuto Oiwa, Akane Inda, Satoru Hayami, Takuya Nomoto, Ryotaro Arita, and Hiroaki Kusunose, in preparation.
->
-> DOI: []()
-
-
-
-## Requirements
-- Symmetry-Adapted Multipole Basis (SAMB) for molecular or crystal are optionally generated by [MultiPie](https://github.com/CMT-MU/MultiPie).
-- MultiPie library optionally requires [TeXLive](https://www.tug.org/texlive/) environment to create LaTeX and PDF files.
-- Molecular or crystal structure files are optionally generated by [QtDraw](https://github.com/CMT-MU/QtDraw).
-
-
-## Documentation
-
-Refer to the [documentation](https://cmt-mu.github.io/SymClosestWannier/) for detailed installation and usage.
-
-
-## To Do
-
-- add function fo automatically set ket_amn.
-- add function to read seedname.uHu, seedname.uIu files.
+- **To Do**:
+  - add function to read seedname.uHu, seedname.uIu files.
```

### Comparing `symclosestwannier-1.1.9/README.md` & `symclosestwannier-1.2.1/docs/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,30 @@
-# SymClosestWannier
+# [SymClosestWannier](https://cmt-mu.github.io/SymClosestWannier/)
 
-A Python library to create Symmetry-adapted Closest Wannier (SymCW) tight-binding models based on the Symmetry-Adapted Multipole Basis (SAMB) [1] and the Closest Wannier formalism developed by Taisuke Ozaki [2].
+- **Overview**:
+    A Python library to create Symmetry-adapted Closest Wannier (SymCW) tight-binding models based on the Symmetry-Adapted Multipole Basis (SAMB) [1] and the Closest Wannier formalism developed by Taisuke Ozaki [2].
 
+    > [1] Hiroaki Kusunose, Rikuto Oiwa, and Satoru Hayami, Symmetry-adapted modeling for molecules and crystals, Phys. Rev. B 107, 195118 (2023).
+    > DOI: https://doi.org/10.1103/PhysRevB.107.195118.<br>
+    > [2] Taisuke Ozaki, Closest Wannier functions to a given set of localized orbitals, arXiv:2306.15296, (2023).
+    > URL: https://arxiv.org/abs/2306.15296v2.
 
-[1] Hiroaki Kusunose, Rikuto Oiwa, and Satoru Hayami, Symmetry-adapted modeling for molecules and crystals, Phys. Rev. B 107, 195118 (2023).
+- **Authors**: Rikuto Oiwa
 
-DOI: https://doi.org/10.1103/PhysRevB.107.195118.
+- **Installation**: SymClosestWannier can be installed from PyPI using pip on Python >= 3.9:
+    ```
+    pip install symclosestwannier
+    ```
+    You can also visit [PyPI](https://pypi.org/project/symclosestwannier/) or [GitHub](https://github.com/CMT-MU/SymClosestWannier/) to download the source.
 
-[2] Taisuke Ozaki, Closest Wannier functions to a given set of localized orbitals, arXiv:2306.15296, (2023).
+- **Citing SymClosestWannier**: If you are using SymClosestWannier in your scientific research, please help our scientific visibility by citing our work:
 
-URL: https://arxiv.org/abs/2306.15296v2.
+    > Rikuto Oiwa, Akane Inda, Satoru Hayami, Takuya Nomoto, Ryotaro Arita, and Hiroaki Kusunose, in preparation.<br>
+    > DOI: []()
 
+- **Requirements**:
+  - Symmetry-Adapted Multipole Basis (SAMB) for molecular or crystal are optionally generated by [MultiPie](https://github.com/CMT-MU/MultiPie).
+  - MultiPie library optionally requires [TeXLive](https://www.tug.org/texlive/) environment to create LaTeX and PDF files.
+  - Molecular or crystal structure files are optionally generated by [QtDraw](https://github.com/CMT-MU/QtDraw).
 
-## Installation
-
-SymClosestWannier can be installed from PyPI using pip on Python >= 3.9:
-```
-pip install symclosestwannier
-```
-You can also visit [PyPI](https://pypi.org/project/symclosestwannier/) or [GitHub](https://github.com/CMT-MU/SymClosestWannier/) to download the source.
-
-
-## Authors
-
-Rikuto Oiwa
-
-
-## Citing SymClosestWannier
-
-If you are using SymClosestWannier in your scientific research, please help our scientific visibility by citing our work:
-
-> Rikuto Oiwa, Akane Inda, Satoru Hayami, Takuya Nomoto, Ryotaro Arita, and Hiroaki Kusunose, in preparation.
->
-> DOI: []()
-
-
-
-## Requirements
-- Symmetry-Adapted Multipole Basis (SAMB) for molecular or crystal are optionally generated by [MultiPie](https://github.com/CMT-MU/MultiPie).
-- MultiPie library optionally requires [TeXLive](https://www.tug.org/texlive/) environment to create LaTeX and PDF files.
-- Molecular or crystal structure files are optionally generated by [QtDraw](https://github.com/CMT-MU/QtDraw).
-
-
-## Documentation
-
-Refer to the [documentation](https://cmt-mu.github.io/SymClosestWannier/) for detailed installation and usage.
-
-
-## To Do
-
-- add function fo automatically set ket_amn.
-- add function to read seedname.uHu, seedname.uIu files.
+- **To Do**:
+  - add function to read seedname.uHu, seedname.uIu files.
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/analyzer/analyzer.py` & `symclosestwannier-1.2.1/symclosestwannier/analyzer/analyzer.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,42 +52,60 @@
         topdir=cwin["outdir"], verbose=cwin["verbose"], parallel=cwin["parallel"], formatter=cwin["formatter"]
     )
 
     filename = os.path.join(cwin["outdir"], "{}".format(f"{seedname}.hdf5"))
     info, data = CWModel.read_info_data(filename)
     cwi = CWInfo("./", seedname, dic=info)
     cwi |= cwin | win
+
+    if cwi["restart"] == "sym":
+        cwi["restart"] = "cw"
+
     cw_model = CWModel(cwi, cwm, dic=data)
 
     cwi = cw_model._cwi
 
     outfile = f"{seedname}.cwpout"
 
     cwm.log(cw_open_msg(), stamp=None, end="\n", file=outfile, mode="w")
     cwm.log(system_msg(cwi), stamp=None, end="\n", file=outfile, mode="a")
 
     # ******************** #
     #       Response       #
     # ******************** #
 
-    res = Response(cwi, cwm)
+    if type(cw_model["Hr_sym"]) == np.ndarray:
+        Hr = np.array(cw_model["Hr_sym"], dtype=np.complex128)
+    elif type(cw_model["Hr"]) == np.ndarray:
+        Hr = np.array(cw_model["Hr"], dtype=np.complex128)
+    else:
+        Hr = None
+
+    res = Response(cwi, cwm, HH_R=Hr)
 
     # ******************** #
     #         Band         #
     # ******************** #
 
     band = Band(cwi, cwm)
 
     # ******************** #
     #        Output        #
     # ******************** #
 
     cwm.log(cw_start_output_msg(), stamp=None, end="\n", file=outfile, mode="a")
     cwm.set_stamp()
 
-    res.write_kubo()
+    if cwi["berry_task"] == "ahc":
+        res.write_ahc()
+
+    if cwi["berry_task"] == "kubo":
+        res.write_kubo()
+
+    if cwi["spin_moment"]:
+        res.write_spin()
 
     cwm.log(f"\n\n  * total elapsed_time:", file=outfile, mode="a")
     cwm.log(cw_end_output_msg(), stamp=None, end="\n", file=outfile, mode="a")
 
     cwm.log(f"  * total elapsed_time:", stamp="start", file=outfile, mode="a")
     cwm.log(postcw_end_msg(), stamp=None, end="\n", file=outfile, mode="a")
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/analyzer/band.py` & `symclosestwannier-1.2.1/symclosestwannier/analyzer/band.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,26 @@
 
 # ==================================================
 class Band(dict):
     """
     Analyze band related properties of Closest Wannier (CW) tight-binding (TB) model.
 
     Attributes:
-        _cwi (SystemInfo): CWInfo.
+        _cwi (CWInfo): CWInfo.
         _cwm (CWManager): CWManager.
         _outfile (str): output file, seedname.cwout.
     """
 
     # ==================================================
     def __init__(self, cwi, cwm):
         """
         initialize the class.
 
         Args:
-            cwi (SystemInfo): CWInfo.
+            cwi (CWInfo): CWInfo.
             cwm (CWManager): CWManager.
         """
         self._cwi = cwi
         self._cwm = cwm
         self._outfile = f"{self._cwi['seedname']}.cwpout"
 
         self.set_operators()
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/analyzer/get_band.py` & `symclosestwannier-1.2.1/symclosestwannier/analyzer/get_band.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/amn.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/amn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Amn manages overlap matrix elements in seedname.amn file, A_{mn}(k) = <ψ^{KS}_{m}(k)|φ_{n}(k)>.
 - ψ^{KS}_{m}(k): Kohn-Sham orbitals (KSOs).
 - φ_{n}(k): pseudo atomic (PAOs) orbitals.
 """
+
 import os
 import gzip
 import tarfile
 import itertools
 
 import numpy as np
 
@@ -23,15 +24,15 @@
         _topdir (str): top directory.
         _seedname (str): seedname.
     """
 
     # ==================================================
     def __init__(self, topdir=None, seedname="cwannier", dic=None):
         """
-        initialize the class.
+        Amn manages overlap matrix elements in seedname.amn file, A_{mn}(k) = <ψ^{KS}_{m}(k)|φ_{n}(k)>.
 
         Args:
             topdir (str, optional): directory of seedname.amn file.
             seedname (str, optional): seedname.
             dic (dict, optional): dictionary of Amn.
         """
         super().__init__()
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/cw_creator.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/cw_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,24 +110,27 @@
 
     if cwi["write_spn"]:
         pass
 
     if cwi["symmetrization"]:
         if cwi["write_hr"]:
             filename = os.path.join(cwi["mp_outdir"], "{}".format(f"{cwi['mp_seedname']}_hr_sym.dat.cw"))
-            cw_model.write_or(cw_model["Hr_sym"], filename, cw_model["rpoints_mp"], header=CWModel._hr_header())
+            cw_model.write_or(cw_model["Hr_sym"], filename, header=CWModel._hr_header())
 
             filename = os.path.join(cwi["mp_outdir"], "{}".format(f"{cwi['mp_seedname']}_hr_nonortho_sym.dat.cw"))
-            cw_model.write_or(
-                cw_model["Hr_nonortho_sym"], filename, cw_model["rpoints_mp"], header=CWModel._hr_header()
-            )
+            cw_model.write_or(cw_model["Hr_nonortho_sym"], filename, header=CWModel._hr_header())
 
         if cwi["write_sr"]:
             filename = os.path.join(cwi["mp_outdir"], "{}".format(f"{cwi['mp_seedname']}_sr_sym.dat.cw"))
-            cw_model.write_or(cw_model["Sr_sym"], filename, cw_model["rpoints_mp"], header=CWModel._sr_header())
+            cw_model.write_or(cw_model["Sr_sym"], filename, header=CWModel._sr_header())
+
+        if cwi["write_tb"]:
+            AA_R = get_oper_R("AA_R", cwi)
+            filename = os.path.join(cwi["mp_outdir"], "{}".format(f"{cwi['mp_seedname']}_tb_sym.dat.cw"))
+            cw_model.write_tb(cw_model["Hr_sym"], AA_R, filename)
 
         filename = os.path.join(cwi["mp_outdir"], "{}".format(f"{cwi['mp_seedname']}_z.dat.cw"))
         cw_model.write_samb_coeffs(filename, type="z")
 
         filename = os.path.join(cwi["mp_outdir"], "{}".format(f"{cwi['mp_seedname']}_z_nonortho.dat.cw"))
         cw_model.write_samb_coeffs(filename, type="z_nonortho")
 
@@ -183,15 +186,15 @@
                 ref_filename = f"{rel}/{seedname}.band.gnu"
             elif os.path.isfile(f"{seedname}.band.gnu.dat"):
                 ref_filename = f"{rel}/{seedname}.band.gnu.dat"
             else:
                 ref_filename = None
 
             Hk_sym_path = cw_model.fourier_transform_r_to_k(
-                cw_model["Hr_sym"], cwi["kpoints_path"], cw_model["rpoints_mp"], atoms_frac=atoms_frac
+                cw_model["Hr_sym"], cwi["kpoints_path"], cwi["irvec"], cwi["ndegen"], atoms_frac=atoms_frac
             )
             Ek, Uk = np.linalg.eigh(Hk_sym_path)
 
             output_linear_dispersion(
                 cwi["mp_outdir"],
                 cwi["mp_seedname"] + "_band.txt",
                 k_linear,
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/cw_info.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/cw_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from symclosestwannier.cw.nnkp import Nnkp
 from symclosestwannier.cw.eig import Eig
 from symclosestwannier.cw.amn import Amn
 from symclosestwannier.cw.mmn import Mmn
 from symclosestwannier.cw.umat import Umat
 from symclosestwannier.cw.spn import Spn
 
-from symclosestwannier.util._utility import wigner_seitz
+from symclosestwannier.util._utility import wigner_seitz, convert_w90_orbital
 
 _class_map = {"cwin": CWin, "win": Win, "nnkp": Nnkp, "eig": Eig, "amn": Amn, "mmn": Mmn, "umat": Umat, "spn": Spn}
 
 
 # ==================================================
 class CWInfo(dict):
     """
@@ -44,15 +44,15 @@
         _topdir (str): top directory.
         _seedname (str): seedname.
     """
 
     # ==================================================
     def __init__(self, topdir=None, seedname="cwannier", dic=None):
         """
-        initialize the class.
+        CWInfo manages information for CWModel, CWin, Win, Nnkp, Eig, Amn, Mmn, Umat, Spn.
 
         Args:
             topdir (str, optional): directory of seedname.cwin file.
             seedname (str, optional): seedname.
             dic (dict, optional): dictionary of CWin.
         """
         super().__init__()
@@ -64,15 +64,15 @@
             self.update(self.read(topdir, seedname))
         else:
             self.update(dic)
 
     # ==================================================
     def read(self, topdir, seedname):
         """
-        read seedname.cwin/win/eig/amn/mmn/nnkp files.
+        read seedname.cwin/win/nnkp/eig/amn/(mmn)/(umat)/(spn) files.
 
         Args:
             topdir (str): directory of seedname.cwin/win/eig/amn/mmn/nnkp files.
             seedname (str): seedname.
 
         Returns:
             dict: system information.
@@ -85,15 +85,15 @@
         for name, C in _class_map.items():
             if name == "umat" and (d["restart"] != "w90"):
                 continue
             if name == "mmn":
                 if not np.any([d["write_rmn"], d["write_vmn"], d["write_tb"], d["berry"]]):
                     continue
             if name == "spn":
-                if not np.any([d["write_spn"], d["spin_decomp"]]):
+                if not np.any([d["write_spn"], d["spin_decomp"], d["spin_moment"], d["zeeman_interaction"]]):
                     continue
 
             info = C(topdir, seedname)
             for k, v in info.items():
                 for name_, info_ in info_list:
                     if k in info_:
                         v_ = info_[k]
@@ -104,15 +104,21 @@
                         else:
                             if v != v_:
                                 raise Exception(f"The value of {k} in {name} and {name_} is inconsistent.")
 
             info_list.append((name, info))
             d.update(info)
 
+        if d["zeeman_interaction"]:
+            if not d["spinors"]:
+                raise Exception("WFs are not spinors.")
+
+        #
         # additional information
+        #
         A = np.array(d["A"])
         irvec, ndegen = wigner_seitz(A, d["mp_grid"])
 
         if d["kpoint"] is not None and d["kpoint_path"] is not None:
             kpoint = {i: NSArray(j, "vector", fmt="value") for i, j in d["kpoint"].items()}
             kpoint_path = d["kpoint_path"]
             N1 = d["N1"]
@@ -126,14 +132,30 @@
         d["unit_cell_volume"] = np.dot(A[0], np.cross(A[1], A[2]))
         d["irvec"] = irvec.tolist()
         d["ndegen"] = ndegen.tolist()
         d["kpoints_path"] = kpoints_path
         d["k_linear"] = k_linear
         d["k_dis_pos"] = k_dis_pos
 
+        # ket
+        if d["ket_amn"] == "auto":
+            ket_amn = [] * d["num_wann"]
+            for pos_idx, l, m, r, s in zip(d["nw2n"], d["nw2l"], d["nw2m"], d["nw2r"], d["nw2s"]):
+                pos = d["atom_pos_r"][pos_idx]
+
+                name = ""
+                for name_, pos_ in d["atoms_frac"].items():
+                    if np.allclose(np.array(pos), np.array(pos_), rtol=1e-04, atol=1e-04):
+                        name = f"{name_[0]}_{name_[1]}"
+
+                orb = convert_w90_orbital(l, m, r, s)
+                ket_amn.append(f"{orb}@{name}")
+
+            d["ket_amn"] = ket_amn
+
         return d
 
     # ==================================================
     def write(self, topdir, seedname):
         """
         read seedname.cwin/win/eig/amn/mmn/nnkp files.
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/cw_manager.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/cw_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 CWManager manages current directory and formatter.
 """
+
 import os
 import sys
 import codecs
 import time
 import pickle
 import subprocess
 from gcoreutils.io_util import read_dict, write_dict
@@ -15,15 +16,15 @@
     """
     manage directory, read, write etc.
     """
 
     # ==================================================
     def __init__(self, topdir=None, verbose=False, parallel=True, formatter=True):
         """
-        initialize the class.
+        manage directory, read, write etc.
 
         Args:
             topdir (str, optional): top directory for output, ends without slash.
             verbose (bool, optional): verbose parallel info. ?
             parallel (bool, optional): use parallel code ?
             formatter (bool, optional): format by using black ?
         """
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/cw_model.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/cw_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 import numpy as np
 from numpy import linalg as npl
 from scipy import linalg as spl
 
 from gcoreutils.nsarray import NSArray
 from multipie.tag.tag_multipole import TagMultipole
 from multipie.model.construct_model import construct_samb_matrix
+from multipie.data.data_transform_matrix import _data_trans_lattice_p
 
 
 from symclosestwannier.util.message import (
     cw_start_msg,
     cw_start_msg_w90,
 )
 from symclosestwannier.util.header import (
@@ -64,15 +65,17 @@
     matrix_dict_k,
     dict_to_matrix,
     sort_ket_matrix_k,
     sort_ket_matrix_dict,
     samb_decomp_operator,
     construct_Or,
     construct_Ok,
+    spin_zeeman_interaction,
 )
+from symclosestwannier.util.get_oper_R import get_oper_R
 
 _default = {
     "Sk": None,
     "Hk": None,
     "Hk_nonortho": None,
     #
     "Sr": None,
@@ -88,41 +91,39 @@
     "Sk_sym": None,
     "Hk_sym": None,
     "Hk_nonortho_sym": None,
     "Sr_sym": None,
     "Hr_sym": None,
     "Hr_nonortho_sym": None,
     #
-    "rpoints_mp": None,
-    #
     "Ek_RMSE_grid": None,
     "Ek_RMSE_path": None,
     #
     "matrix_dict": None,
 }
 
 
 # ==================================================
 class CWModel(dict):
     """
     Closest Wannier (CW) tight-binding (TB) model based on Plane-Wave (PW) DFT calculation.
 
     Attributes:
-        _cwi (SystemInfo): CWInfo.
+        _cwi (CWInfo): CWInfo.
         _cwm (CWManager): CWManager.
         _outfile (str): output file, seedname.cwout.
     """
 
     # ==================================================
     def __init__(self, cwi, cwm, dic=None):
         """
-        initialize the class.
+        Closest Wannier (CW) tight-binding (TB) model based on Plane-Wave (PW) DFT calculation.
 
         Args:
-            cwi (SystemInfo, optional): CWInfo.
+            cwi (CWInfo, optional): CWInfo.
             cwm (CWManager,optional): CWManager.
             dic (dict, optional): dictionary of data.
         """
         super().__init__()
 
         self._cwi = cwi
         self._cwm = cwm
@@ -156,14 +157,24 @@
         Sk = Ak.transpose(0, 2, 1).conjugate() @ Ak
         Sk = 0.5 * (Sk + np.einsum("kmn->knm", Sk).conj())
 
         diag_Ek = np.array([np.diag(Ek[k]) for k in range(self._cwi["num_k"])])
         Hk = Uk.transpose(0, 2, 1).conjugate() @ diag_Ek @ Uk
         Hk = 0.5 * (Hk + np.einsum("kmn->knm", Hk).conj())
 
+        if self._cwi["zeeman_interaction"]:
+            B = self._cwi["magnetic_field"]
+            theta = self._cwi["magnetic_field_theta"]
+            phi = self._cwi["magnetic_field_phi"]
+            g_factor = self._cwi["g_factor"]
+
+            pauli_spin = Uk.transpose(0, 2, 1).conjugate() @ self._cwi["pauli_spn"] @ Uk
+            H_zeeman = spin_zeeman_interaction(B, theta, phi, pauli_spin, g_factor, self._cwi["num_wann"])
+            Hk += H_zeeman
+
         S2k = np.array([spl.sqrtm(Sk[k]) for k in range(self._cwi["num_k"])])
         Hk_nonortho = S2k @ Hk @ S2k
 
         Sr = CWModel.fourier_transform_k_to_r(Sk, self._cwi["kpoints"], self._cwi["irvec"])
         Hr = CWModel.fourier_transform_k_to_r(Hk, self._cwi["kpoints"], self._cwi["irvec"])
         Hr_nonortho = CWModel.fourier_transform_k_to_r(Hk_nonortho, self._cwi["kpoints"], self._cwi["irvec"])
 
@@ -332,14 +343,24 @@
             Uk = Ak @ S2k_inv
 
         # projection from KS energies to Closest Wannnier Hamiltonian
         diag_Ek = np.array([np.diag(Ek[k]) for k in range(self._cwi["num_k"])])
         Hk = Uk.transpose(0, 2, 1).conjugate() @ diag_Ek @ Uk
         Hk = 0.5 * (Hk + np.einsum("kmn->knm", Hk).conj())
 
+        if self._cwi["zeeman_interaction"]:
+            B = self._cwi["magnetic_field"]
+            theta = self._cwi["magnetic_field_theta"]
+            phi = self._cwi["magnetic_field_phi"]
+            g_factor = self._cwi["g_factor"]
+
+            pauli_spin = Uk.transpose(0, 2, 1).conjugate() @ self._cwi["pauli_spn"] @ Uk
+            H_zeeman = spin_zeeman_interaction(B, theta, phi, pauli_spin, g_factor, self._cwi["num_wann"])
+            Hk += H_zeeman
+
         S2k = np.array([spl.sqrtm(Sk[k]) for k in range(self._cwi["num_k"])])
         Hk_nonortho = S2k @ Hk @ S2k
 
         Sr = CWModel.fourier_transform_k_to_r(Sk, self._cwi["kpoints"], self._cwi["irvec"])
         Hr = CWModel.fourier_transform_k_to_r(Hk, self._cwi["kpoints"], self._cwi["irvec"])
         Hr_nonortho = CWModel.fourier_transform_k_to_r(Hk_nonortho, self._cwi["kpoints"], self._cwi["irvec"])
 
@@ -397,48 +418,60 @@
             (zj, tag_dict[zj]): {tuple(sp.sympify(k)): complex(sp.sympify(v)) for k, v in d.items()}
             for zj, d in mat["matrix"].items()
         }
         mat["matrix"] = {
             zj: {tuple(sp.sympify(k)): complex(sp.sympify(v)) for k, v in d.items()} for zj, d in mat["matrix"].items()
         }
 
+        A = None
+        A_samb = None
+
         lattice = model["info"]["group"][1].split("/")[1].replace(" ", "")[0]
         if lattice != "P":
             cell_site = {}
             for site, v in mat["cell_site"].items():
                 if "(" in site and ")" in site:
                     if "(1)" in site:
                         cell_site[site[:-3]] = v
                 else:
                     cell_site[site] = v
 
             mat["cell_site"] = cell_site
 
+        if not mat["molecule"]:
+            A = self._cwi["unit_cell_cart"]
+            A_samb = NSArray(mat["A"], style="matrix", fmt="value").T
+            if lattice != "P":
+                # 4x4 matrix to convert from conventioanl to primitive coordinate.
+                latticeP = {
+                    lat: np.array(NSArray(d).numpy().tolist(), dtype=float) for lat, d in _data_trans_lattice_p.items()
+                }
+                lattice_const = model["info"]["cell"]["a"]
+                A_samb = lattice_const * latticeP[lattice][:-1, :-1]
+                print(A_samb)
         #####
 
         atoms_list = list(self._cwi["atoms_frac"].values())
         atoms_frac = np.array([atoms_list[i] for i in self._cwi["nw2n"]])
 
         atoms_frac_samb = [
             NSArray(mat["cell_site"][ket_samb[a].split("@")[1]][0], style="vector", fmt="value").tolist()
             for a in range(self._cwi["num_wann"])
         ]
 
-        if not mat["molecule"]:
-            A = self._cwi["unit_cell_cart"]
-            A_samb = NSArray(mat["A"], style="matrix", fmt="value").T
-        else:
-            A = None
-            A_samb = None
-
         msg = "    - decomposing Hamiltonian as linear combination of SAMBs ... "
         self._cwm.log(msg, None, end="", file=self._outfile, mode="a")
         self._cwm.set_stamp()
 
-        z = CWModel.samb_decomp_operator(Hr_dict, Zr_dict, A, atoms_frac, ket_amn, A_samb, atoms_frac_samb, ket_samb)
+        if mat["molecule"]:
+            z = CWModel.samb_decomp_operator(Hr_dict, Zr_dict, ket=ket_amn, ket_samb=ket_samb)
+        else:
+            z = CWModel.samb_decomp_operator(
+                Hr_dict, Zr_dict, A, atoms_frac, ket_amn, A_samb, atoms_frac_samb, ket_samb
+            )
 
         self._cwm.log("done", file=self._outfile, mode="a")
 
         #####
 
         msg = "    - decomposing overlap as linear combination of SAMBs ... "
         self._cwm.log(msg, None, end="", file=self._outfile, mode="a")
@@ -460,31 +493,44 @@
 
         #####
 
         msg = "    - constructing symmetrized TB Hamiltonian ... "
         self._cwm.log(msg, None, end="", file=self._outfile, mode="a")
         self._cwm.set_stamp()
 
-        rpoints_mp = [(n1, n2, n3) for Zj_dict in Zr_dict.values() for (n1, n2, n3, _, _) in Zj_dict.keys()]
-        rpoints_mp = sorted(list(set(rpoints_mp)), key=rpoints_mp.index)
-
-        Sr_sym = CWModel.construct_Or(list(s.values()), self._cwi["num_wann"], rpoints_mp, mat)
-        Hr_sym = CWModel.construct_Or(list(z.values()), self._cwi["num_wann"], rpoints_mp, mat)
-        Hr_nonortho_sym = CWModel.construct_Or(list(z_nonortho.values()), self._cwi["num_wann"], rpoints_mp, mat)
+        Sr_sym = CWModel.construct_Or(list(s.values()), self._cwi["num_wann"], self._cwi["irvec"], mat)
+        Hr_sym = CWModel.construct_Or(list(z.values()), self._cwi["num_wann"], self._cwi["irvec"], mat)
+        Hr_nonortho_sym = CWModel.construct_Or(
+            list(z_nonortho.values()), self._cwi["num_wann"], self._cwi["irvec"], mat
+        )
 
         if self._cwi["tb_gauge"]:
-            Sk_sym = CWModel.fourier_transform_r_to_k(Sr_sym, self._cwi["kpoints"], rpoints_mp, atoms_frac=atoms_frac_samb)
-            Hk_sym = CWModel.fourier_transform_r_to_k(Hr_sym, self._cwi["kpoints"], rpoints_mp, atoms_frac=atoms_frac_samb)
+            Sk_sym = CWModel.fourier_transform_r_to_k(
+                Sr_sym, self._cwi["kpoints"], self._cwi["irvec"], self._cwi["ndegen"], atoms_frac=atoms_frac_samb
+            )
+            Hk_sym = CWModel.fourier_transform_r_to_k(
+                Hr_sym, self._cwi["kpoints"], self._cwi["irvec"], self._cwi["ndegen"], atoms_frac=atoms_frac_samb
+            )
             Hk_nonortho_sym = CWModel.fourier_transform_r_to_k(
-                Hr_nonortho_sym, self._cwi["kpoints"], rpoints_mp, atoms_frac=atoms_frac_samb
+                Hr_nonortho_sym,
+                self._cwi["kpoints"],
+                self._cwi["irvec"],
+                self._cwi["ndegen"],
+                atoms_frac=atoms_frac_samb,
             )
         else:
-            Sk_sym = CWModel.fourier_transform_r_to_k(Sr_sym, self._cwi["kpoints"], rpoints_mp)
-            Hk_sym = CWModel.fourier_transform_r_to_k(Hr_sym, self._cwi["kpoints"], rpoints_mp)
-            Hk_nonortho_sym = CWModel.fourier_transform_r_to_k(Hr_nonortho_sym, self._cwi["kpoints"], rpoints_mp)
+            Sk_sym = CWModel.fourier_transform_r_to_k(
+                Sr_sym, self._cwi["kpoints"], self._cwi["irvec"], self._cwi["ndegen"]
+            )
+            Hk_sym = CWModel.fourier_transform_r_to_k(
+                Hr_sym, self._cwi["kpoints"], self._cwi["irvec"], self._cwi["ndegen"]
+            )
+            Hk_nonortho_sym = CWModel.fourier_transform_r_to_k(
+                Hr_nonortho_sym, self._cwi["kpoints"], self._cwi["irvec"], self._cwi["ndegen"]
+            )
         self._cwm.log("done", file=self._outfile, mode="a")
 
         #####
 
         msg = "    - evaluating fitting accuracy ... "
         self._cwm.log(msg, None, end="\n", file=self._outfile, mode="a")
         self._cwm.set_stamp()
@@ -504,18 +550,24 @@
             Hk_path = CWModel.fourier_transform_r_to_k(
                 self["Hr"], self._cwi["kpoints_path"], self._cwi["irvec"], self._cwi["ndegen"]
             )
             Ek_path, _ = np.linalg.eigh(Hk_path)
 
             if self._cwi["tb_gauge"]:
                 Hk_sym_path = CWModel.fourier_transform_r_to_k(
-                    Hr_sym, self._cwi["kpoints_path"], rpoints_mp, atoms_frac=atoms_frac_samb
+                    Hr_sym,
+                    self._cwi["kpoints_path"],
+                    self._cwi["irvec"],
+                    self._cwi["ndegen"],
+                    atoms_frac=atoms_frac_samb,
                 )
             else:
-                Hk_sym_path = CWModel.fourier_transform_r_to_k(Hr_sym, self._cwi["kpoints_path"], rpoints_mp)
+                Hk_sym_path = CWModel.fourier_transform_r_to_k(
+                    Hr_sym, self._cwi["kpoints_path"], self._cwi["irvec"], self._cwi["ndegen"]
+                )
 
             Ek_path_sym, _ = np.linalg.eigh(Hk_sym_path)
 
             num_k, num_wann = Ek_path_sym.shape
             Ek_RMSE_path = np.sum(np.abs(Ek_path_sym - Ek_path)) / num_k / num_wann * 1000  # [meV]
 
             msg = f"     * RMSE of eigen values between CW and Symmetry-Adapted CW models (path) = {'{:.4f}'.format(Ek_RMSE_path)} [meV]"
@@ -527,15 +579,15 @@
 
         msg = "    - evaluating expectation value of {Zj} at T = 0 ... "
         self._cwm.log(msg, None, end="\n", file=self._outfile, mode="a")
         self._cwm.set_stamp()
 
         # Zk = construct_samb_matrix(mat, np.array(self._cwi["kpoints"]))
         # Ek, Uk = np.linalg.eigh(Hk_sym)
-        # Z_exp = thermal_avg(Zk, Ek, Uk, ef=self._cwi["fermi_energy"], T=0.0)
+        # Z_exp = thermal_avg(Zk.tolist(), Ek, Uk, self._cwi["fermi_energy"], T=0.0)
         # z_exp = {key: Z_exp[i] for i, key in enumerate(z.keys())}
         z_exp = {}
 
         self._cwm.log("done", None, end="\n", file=self._outfile, mode="a")
 
         #####
 
@@ -549,16 +601,14 @@
                 "Sk_sym": Sk_sym,
                 "Hk_sym": Hk_sym,
                 "Hk_nonortho_sym": Hk_nonortho_sym,
                 "Sr_sym": Sr_sym,
                 "Hr_sym": Hr_sym,
                 "Hr_nonortho_sym": Hr_nonortho_sym,
                 #
-                "rpoints_mp": rpoints_mp,
-                #
                 "Ek_RMSE_grid": Ek_RMSE_grid,
                 "Ek_RMSE_path": Ek_RMSE_path,
                 #
                 "matrix_dict": mat,
             }
         )
 
@@ -932,17 +982,17 @@
         """
         num_wann = self._cwi["num_wann"]
         unit_cell_cart = np.array(self._cwi["unit_cell_cart"])
         Or = np.array(Or)
         Or_str = "# created by pw2cw \n"
         Or_str += "# written {}\n".format(datetime.datetime.now().strftime("on %d%b%Y at %H:%M:%S"))
 
-        Or_str += " {0[0]:15.6f} {0[1]:15.6f} {0[2]:15.6f}\n".format(unit_cell_cart[0, :])
-        Or_str += " {0[0]:15.6f} {0[1]:15.6f} {0[2]:15.6f}\n".format(unit_cell_cart[1, :])
-        Or_str += " {0[0]:15.6f} {0[1]:15.6f} {0[2]:15.6f}\n".format(unit_cell_cart[2, :])
+        Or_str += " {0[0]:18.15f} {0[1]:18.15f} {0[2]:18.15f}\n".format(unit_cell_cart[0, :])
+        Or_str += " {0[0]:18.15f} {0[1]:18.15f} {0[2]:18.15f}\n".format(unit_cell_cart[1, :])
+        Or_str += " {0[0]:18.15f} {0[1]:18.15f} {0[2]:18.15f}\n".format(unit_cell_cart[2, :])
 
         if rpoints is None:
             rpoints = np.array(self._cwi["irvec"])
             ndegen = np.array(self._cwi["ndegen"])
             Or_str += "{:12d}\n{:12d}\n".format(num_wann, len(ndegen))
             Or_str += textwrap.fill("".join(["{:5d}".format(x) for x in ndegen]), 75, drop_whitespace=False)
             Or_str += "\n"
@@ -955,18 +1005,18 @@
         for irpts in range(len(rpoints)):
             for i, j in itertools.product(range(num_wann), repeat=2):
                 v = rpoints[irpts, :]
                 line = "{:5d}{:5d}{:5d}{:5d}{:5d}  ".format(
                     int(round(v[0])), int(round(v[1])), int(round(v[2])), j + 1, i + 1
                 )
                 if vec:
-                    line += "".join([" {:>12.6f} {:>12.6f}".format(x.real, x.imag) for x in Or[:, irpts, j, i]])
+                    line += "".join([" {:>15.8E} {:>15.8E}".format(x.real, x.imag) for x in Or[:, irpts, j, i]])
                 else:
                     x = Or[irpts, j, i]
-                    line += " {:>12.6f} {:>12.6f}".format(x.real, x.imag)
+                    line += " {:>15.8E} {:>15.8E}".format(x.real, x.imag)
                 line += "\n"
 
                 Or_str += line
 
         self._cwm.write(filename, Or_str, header, None)
 
     # ==================================================
@@ -982,17 +1032,17 @@
         """
         num_wann = self._cwi["num_wann"]
         unit_cell_cart = np.array(self._cwi["unit_cell_cart"])
         Hr = np.array(Hr)
         tb_str = "# created by pw2cw \n"
         tb_str += "# written {}\n".format(datetime.datetime.now().strftime("on %d%b%Y at %H:%M:%S"))
 
-        tb_str += " {0[0]:15.6f} {0[1]:15.6f} {0[2]:15.6f}\n".format(unit_cell_cart[0, :])
-        tb_str += " {0[0]:15.6f} {0[1]:15.6f} {0[2]:15.6f}\n".format(unit_cell_cart[1, :])
-        tb_str += " {0[0]:15.6f} {0[1]:15.6f} {0[2]:15.6f}\n".format(unit_cell_cart[2, :])
+        tb_str += " {0[0]:18.15f} {0[1]:18.15f} {0[2]:18.15f}\n".format(unit_cell_cart[0, :])
+        tb_str += " {0[0]:18.15f} {0[1]:18.15f} {0[2]:18.15f}\n".format(unit_cell_cart[1, :])
+        tb_str += " {0[0]:18.15f} {0[1]:18.15f} {0[2]:18.15f}\n".format(unit_cell_cart[2, :])
 
         if rpoints is None:
             rpoints = np.array(self._cwi["irvec"])
             ndegen = np.array(self._cwi["ndegen"])
             tb_str += "{:12d}\n{:12d}\n".format(num_wann, len(ndegen))
             tb_str += textwrap.fill("".join(["{:5d}".format(x) for x in ndegen]), 75, drop_whitespace=False)
             tb_str += "\n\n"
@@ -1007,30 +1057,30 @@
             v = rpoints[irpts, :]
             tb_str += "{:5d}{:5d}{:5d}".format(int(round(v[0])), int(round(v[1])), int(round(v[2])))
             tb_str += "\n"
             for i, j in itertools.product(range(num_wann), repeat=2):
                 v = rpoints[irpts, :]
                 line = "{:5d}{:5d}  ".format(j + 1, i + 1)
                 x = Hr[irpts, j, i]
-                line += " {:>12.6f} {:>12.6f}".format(x.real, x.imag)
+                line += " {:>15.8E} {:>15.8E}".format(x.real, x.imag)
                 line += "\n"
 
                 tb_str += line
 
             tb_str += "\n"
 
         # _r
         for irpts in range(len(rpoints)):
             v = rpoints[irpts, :]
             tb_str += "{:5d}{:5d}{:5d}".format(int(round(v[0])), int(round(v[1])), int(round(v[2])))
             tb_str += "\n"
             for i, j in itertools.product(range(num_wann), repeat=2):
                 v = rpoints[irpts, :]
                 line = "{:5d}{:5d}  ".format(j + 1, i + 1)
-                line += "".join([" {:>12.6f} {:>12.6f}".format(x.real, x.imag) for x in Ar[:, irpts, j, i]])
+                line += "".join([" {:>15.8E} {:>15.8E}".format(x.real, x.imag) for x in Ar[:, irpts, j, i]])
                 line += "\n"
 
                 tb_str += line
 
             tb_str += "\n"
 
         self._cwm.write(filename, tb_str, None, None)
@@ -1059,15 +1109,15 @@
             raise Exception(f"invalid type = {type} was given. choose from 'z'/'z_nonortho'/'s'.")
 
         o_str = "# created by pw2cw \n"
         o_str += "# written {}\n".format(datetime.datetime.now().strftime("on %d%b%Y at %H:%M:%S"))
 
         o_str = "".join(
             [
-                "{:>7d}   {:>15}   {:>15}   {:>12.6f} \n ".format(j + 1, zj, tag, v)
+                "{:>7d}   {:>15}   {:>15}   {:>15.8E} \n ".format(j + 1, zj, tag, v)
                 for j, ((zj, tag), v) in enumerate(o.items())
             ]
         )
 
         self._cwm.write(filename, o_str, header, None)
 
     # ==================================================
@@ -1079,13 +1129,13 @@
             filename (str): file name.
         """
         z_exp_str = "# created by pw2cw \n"
         z_exp_str += "# written {}\n".format(datetime.datetime.now().strftime("on %d%b%Y at %H:%M:%S"))
 
         z_exp_str = "".join(
             [
-                "{:>7d}   {:>15}   {:>15}   {:>12.6f} \n ".format(j + 1, zj, tag, v)
+                "{:>7d}   {:>15}   {:>15}   {:>15.8E} \n ".format(j + 1, zj, tag, v)
                 for j, ((zj, tag), v) in enumerate(self["z_exp"].items())
             ]
         )
 
         self._cwm.write(filename, z_exp_str, z_exp_header, None)
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/cwin.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/cwin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 CWin manages input file for pw2cw, seedname.cwin file.
 """
+
 import os
 
 
 _default = {
     "seedname": "cwannier",
     "outdir": "./",
     "restart": "cw",
@@ -18,16 +19,18 @@
     "delta": 1e-12,
     "svd": False,
     #
     "verbose": False,
     "parallel": False,
     "formatter": False,
     #
-    "transl_inv": True, # use Eq.(31) of Marzari&Vanderbilt PRB 56, 12847 (1997) for band-diagonal position matrix elements.
-    "tb_gauge": False, # tb gauge?
+    "transl_inv": True,
+    "use_degen_pert": False,
+    "degen_thr": 0.0,
+    "tb_gauge": False,
     #
     "write_hr": False,
     "write_sr": False,
     "write_u_matrices": False,
     "write_rmn": False,
     "write_vmn": False,
     "write_tb": False,
@@ -38,14 +41,20 @@
     "mp_seedname": "default",
     "ket_amn": None,
     "irreps": "all",
     #
     "a": None,
     "N1": 50,
     "fermi_energy": 0.0,
+    #
+    "zeeman_interaction": False,
+    "magnetic_field": 0.0,
+    "magnetic_field_theta": 0.0,
+    "magnetic_field_phi": 0.0,
+    "g_factor": 2.0,
 }
 
 
 # ==================================================
 class CWin(dict):
     """
     CWin manages input file for pw2cw, seedname.cwin file.
@@ -54,15 +63,15 @@
         _topdir (str): top directory.
         _seedname (str): seedname.
     """
 
     # ==================================================
     def __init__(self, topdir=None, seedname="cwannier", dic=None):
         """
-        initialize the class.
+        CWin manages input file for pw2cw, seedname.cwin file.
 
         Args:
             topdir (str, optional): directory of seedname.cwin file.
             seedname (str, optional): seedname.
             dic (dict, optional): dictionary of CWin.
         """
         super().__init__()
@@ -98,46 +107,56 @@
                 - smearing_temp_min : smearing temperature for lower window (float), [0.01].
                 - delta             : small constant to avoid ill-conditioning of overlap matrices (float), [1e-12].
                 - svd               : implement singular value decomposition ? otherwise adopt Lowdin's orthogonalization method (bool), [False].
                 - verbose           : verbose calculation info (bool, optional), [False].
                 - parallel          : use parallel code? (bool), [False].
                 - formatter         : format by using black? (bool), [False].
                 - transl_inv        : use Eq.(31) of Marzari&Vanderbilt PRB 56, 12847 (1997) for band-diagonal position matrix elements? (bool), [True].
+                - use_degen_pert    : use degenerate perturbation theory when bands are degenerate and band derivatives are needed? (bool), [False].
+                - degen_thr         : threshold to exclude degenerate bands from the calculation, [0.0].
                 - tb_gauge          : use tb gauge? (bool), [False].
                 - write_hr          : write seedname_hr.py ? (bool), [False].
                 - write_sr          : write seedname_sr.py ? (bool), [False].
                 - write_u_matrices  : write seedname_u.dat and seedname_u_dis.dat ? (bool), [False].
                 - write_rmn         : write seedname_r.dat ? (bool), [False].
                 - write_vmn         : write seedname_v.dat ? (bool), [False].
                 - write_tb          : write seedname_tb.dat ? (bool), [False].
                 - write_spn         : write seedname.spn.cw ? (bool), [False].
 
             # only used for symmetrization.
                 - symmetrization    : symmetrize ? (bool), [False].
                 - mp_outdir         : output files for multipie are found in this directory (str). ["./"].
                 - mp_seedname       : seedname for seedname_model.py, seedname_samb.py and seedname_matrix.py files (str), ["default"].
-                - ket_amn           : ket basis list in the seedname.amn file. The format of each ket must be same as the "ket" in sambname_model.py file. See sambname["info"]["ket"] in sambname_model.py file for the format (list), [None].
+                - ket_amn           : ket basis list in the seedname.amn file. If ket_amn == auto, the list of orbitals are set automatically, or it can be set manually. The format of each ket must be same as the "ket" in sambname_model.py file. See sambname["info"]["ket"] in sambname_model.py file for the format (list), [None].
                 - irreps            : list of irreps to be considered (str/list), ["all"].
 
             # only used for band dispersion calculation.
                 - a                 : lattice parameter (in Ang) used to correct units of k points in reference band data, [None].
-                - fermi_energy      : fermi energy used for band shift, [None].
                 - N1                : number of divisions for high symmetry lines (int, optional), [50].
+                - fermi_energy      : fermi energy, [0.0].
+
+            # only used for when zeeman interaction is considered.
+                - zeeman_interaction   : consider zeeman interaction ? (bool), [False].
+                - magnetic_field       : strength of the magnetic field (float), [0.0].
+                - magnetic_field_theta : angle from the z-axis of the magnetic field (float), [0.0].
+                - magnetic_field_phi   : angle from the x-axis of the magnetic field (float), [0.0].
+                - g_factor             : spin g factor (float), [2.0].
         """
         if os.path.exists(file_name):
             with open(file_name) as fp:
                 cwin_data = fp.readlines()
         else:
             raise Exception("failed to read cwin file: " + file_name)
 
         # default
         d = CWin._default().copy()
 
         for line in cwin_data:
             line = line.replace("\n", "")
+            line = line.lstrip()
 
             if len([vi for vi in line.split(" ") if vi != ""]) == 0:
                 continue
 
             key = line.split("=")[0]
             key = key.replace(" ", "")
 
@@ -146,21 +165,26 @@
 
             if "=" in line:
                 v = (line.split("=")[1].split("!")[0]).replace(" ", "")
             elif ":" in line:
                 v = (line.split(":")[1].split("!")[0]).replace(" ", "")
 
             if key == "ket_amn":
-                v = "".join(v)
+                if "[" in v or "]" in v:
+                    v = "".join(v)
 
             d[key] = self._str_to(key, v)
         assert not (
             d["restart"] == "w90" and d["symmetrization"]
         ), "Symmetrization cannot be performed when restart == w90."
 
+        assert not (
+            d["disentangle"] and d["dis_win_emax"] is None or d["dis_win_emin"] is None
+        ), "dis_win_emax and dis_win_emin must be specified when disentangle == true."
+
         return d
 
     # ==================================================
     def _str_to(self, key, v):
         v = str(v).replace("'", "").replace('"', "")
 
         if key in ("seedname", "mp_seedname"):
@@ -175,36 +199,42 @@
             "dis_win_emax",
             "dis_win_emin",
             "smearing_temp_max",
             "smearing_temp_min",
             "delta",
             "a",
             "fermi_energy",
+            "degen_thr",
+            "magnetic_field",
+            "magnetic_field_theta",
+            "magnetic_field_phi",
+            "g_factor",
         ):
             v = float(v)
         elif key == "N1":
             v = int(v)
         elif key == "ket_amn":
-            if "(" in str(v) and ")" in str(v):
-                v = [str(o) if i == 0 else f"({str(o)}" for i, o in enumerate(v[1:-1].split(",("))]
-            else:
-                v = [str(o) for o in v[1:-1].split(",")]
+            if "[" in v or "]" in v:
+                if "(" in str(v) and ")" in str(v):
+                    v = [str(o) if i == 0 else f"({str(o)}" for i, o in enumerate(v[1:-1].split(",("))]
+                else:
+                    v = [str(o) for o in v[1:-1].split(",")]
         elif key == "irreps":
             if "[" in v and "]" in v:
                 v = [str(o) for o in v[1:-1].split(",")]
             else:
                 if v not in ("all", "full"):
                     raise Exception(f"invalid irreps = {v} was given. choose from 'all'/'full'.")
         else:
             if v.lower() in ("true", ".true."):
                 v = True
             elif v.lower() in ("false", ".false."):
                 v = False
             else:
-                raise Exception(f"invalid {k} = {v} was given. choose from 'true'/'.true.'/'false'/'.false.'.")
+                raise Exception(f"invalid {key} = {v} was given. choose from 'true'/'.true.'/'false'/'.false.'.")
 
         return v
 
     # ==================================================
     @classmethod
     def _default(cls):
         return _default
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/eig.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/eig.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Eig manages Kohn-Sham energies in seedname.eig file, E_{m}(k).
 """
+
 import os
 import gzip
 import tarfile
 import itertools
 import datetime
 
 import numpy as np
@@ -22,15 +23,15 @@
         _topdir (str): top directory.
         _seedname (str): seedname.
     """
 
     # ==================================================
     def __init__(self, topdir=None, seedname="cwannier", dic=None):
         """
-        initialize the class.
+        Eig manages Kohn-Sham energies in seedname.eig file, E_{m}(k).
 
         Args:
             topdir (str, optional): directory of seedname.eig file.
             seedname (str, optional): seedname.
             dic (dict, optional): dictionary of Eig.
         """
         super().__init__()
@@ -87,15 +88,14 @@
         write eig data.
 
         Args:
             file_name (str, optional): file name.
         """
         Ek = np.array(self["Ek"])
 
-
         with open(file_name, "w") as fp:
             fp.write("# created by eig.py\n")
             fp.write("# written {}\n".format(datetime.datetime.now().strftime("on %d%b%Y at %H:%M:%S")))
             for ik, n in itertools.product(range(self["num_k"]), range(self["num_bands"])):
                 fp.write("{0}  {1}  {2:<18.12f}\n".format(n + 1, ik + 1, Ek[ik, n]))
 
         print(f"  * wrote '{file_name}'.")
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/mmn.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/mmn.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         _seedname (str): seedname.
         _npar (int): # of cpu core.
     """
 
     # ==================================================
     def __init__(self, topdir=None, seedname="cwannier", dic=None, npar=multiprocessing.cpu_count()):
         """
-        initialize the class.
+        Mmn manages overlap matrix elements in seedname.mmn file, M_{mn}(k,b) = <u^{KS}_{m}(k)|u^{KS}_{n}(k+b)>.
 
         Args:
             topdir (str, optional): directory of seedname.mmn file.
             seedname (str, optional): seedname.
             dic (dict, optional): dictionary of Mmn.
             npar (int, optional): # of cpu core.
         """
@@ -67,15 +67,15 @@
             file_name (str, optional): file name.
 
         Returns:
             dict:
                 - num_k     : # of k points (int), [1].
                 - num_bands : # of bands passed to the code (int), [1].
                 - num_b     : # of b-vectors (int), [1].
-                - nnkpts    : nearest-nmmnhbour k-points (list), [None].
+                - nnkpts    : nearest-neighbor k-points (list), [None].
                 - Mkb       : Overlap matrix elements, M_{mn}(k,b) = <u^{KS}_{m}(k)|u^{KS}_{n}(k+b)> (list), [None].
         """
         if os.path.exists(file_name):
             fp = open(file_name, "r")
         elif os.path.exists(file_name + ".gz"):
             fp = gzip.open(file_name + ".gz", "rt")
         elif os.path.exists(file_name + ".tar.gz"):
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/nnkp.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/nnkp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Nnkp manages information needed to determine the required overlap elements Mmn(k,b) and projections A_{mn}(k).
 """
+
 import os
 import gzip
 import tarfile
 import itertools
 
 import numpy as np
 import scipy.linalg
@@ -20,14 +21,15 @@
     "kpoints": [[0, 0, 0]],
     "kpoints_wo_shift": [[0, 0, 0]],
     "nnkpts": None,
     "nw2n": None,
     "nw2l": None,
     "nw2m": None,
     "nw2r": None,
+    "nw2s": None,
     "atom_orb": None,
     "atom_pos": None,
     "atom_pos_r": None,
     "bvec_cart": None,
     "bvec_crys": None,
     "wb": None,
 }
@@ -42,15 +44,15 @@
         _topdir (str): top directory.
         _seedname (str): seedname.
     """
 
     # ==================================================
     def __init__(self, topdir=None, seedname="cwannier", dic=None):
         """
-        initialize the class.
+        Nnkp manages information needed to determine the required overlap elements Mmn(k,b) and projections A_{mn}(k).
 
         Args:
             topdir (str, optional): directory of seedname.nnkp file.
             seedname (str, optional): seedname.
             dic (dict, optional): dictionary of Nnkp.
         """
         super().__init__()
@@ -83,14 +85,15 @@
                 - kpoints          : k-points, [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].
                 - kpoints_wo_shift : k-points without shift, [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].
                 - nnkpts           : nearest-neighbour k-points (list), [None].
                 - nw2n             : atom position index of each WFs (list), [None].
                 - nw2l             : l specifies the angular part Θlm(θ, φ) (list), [None].
                 - nw2m             : m specifies the angular part Θlm(θ, φ) (list), [None].
                 - nw2r             : r specifies the radial part Rr(r) (list), [None].
+                - nw2s             : s specifies the spin, 1(up)/-1(dn) (list), [None].
                 - atom_orb         : WFs indexes of each atom (list), [None].
                 - atom_pos         : atom position index of each atom (list), [None].
                 - atom_pos_r       : atom position of each atom in fractional coordinates with respect to the lattice vectors (list), [None].
                 - bvec_cart        : b-vectors (cartesian coordinate) (list), [None].
                 - bvec_crys        : b-vectors (crystal coordinate) (list), [None].
                 - wb               : weight for each k-points and nearest-neighbour k-points (list), [None].
         """
@@ -135,28 +138,33 @@
                 if "begin projections" in line or "begin spinor_projections" in line:
                     spinors = "begin spinor_projections" in line
                     d["num_wann"] = int(nnkp_data[i + 1])
                     nw2n = np.zeros([d["num_wann"]], dtype=int)
                     nw2l = np.zeros([d["num_wann"]], dtype=int)
                     nw2m = np.zeros([d["num_wann"]], dtype=int)
                     nw2r = np.zeros([d["num_wann"]], dtype=int)
+                    nw2s = np.zeros([d["num_wann"]], dtype=int)
                     atom_orb_strlist = []
                     atom_pos_strlist = []
                     # read projections
                     for j in range(d["num_wann"]):
                         if spinors:
                             proj_str = nnkp_data[i + 2 + 3 * j]
                         else:
                             proj_str = nnkp_data[i + 2 + 2 * j]
                         proj_dat = proj_str.split()
                         nw2l[j] = int(proj_dat[3])
                         nw2m[j] = int(proj_dat[4])
                         nw2r[j] = int(proj_dat[5])
+                        if spinors:
+                            spn_dat = nnkp_data[i + 2 + 3 * j + 2].split()[0]
+                            nw2s[j] = int(spn_dat)
                         atom_orb_strlist.append(proj_str[0:40])
                         atom_pos_strlist.append(proj_str[0:35])
+
                     atom_orb_uniq = sorted(set(atom_orb_strlist), key=atom_orb_strlist.index)
                     atom_pos_uniq = sorted(set(atom_pos_strlist), key=atom_pos_strlist.index)
                     atom_orb = []
                     for orb_str in atom_orb_uniq:
                         indexes = [j for j, x in enumerate(atom_orb_strlist) if x == orb_str]
                         atom_orb.append(indexes)
                     atom_pos = []
@@ -173,14 +181,15 @@
                                 nw2n[n] = i
 
                     d["num_atom"] = num_atom
                     d["nw2n"] = nw2n.tolist()
                     d["nw2l"] = nw2l.tolist()
                     d["nw2m"] = nw2m.tolist()
                     d["nw2r"] = nw2r.tolist()
+                    d["nw2s"] = nw2s.tolist()
                     d["atom_orb"] = atom_orb
                     d["atom_pos"] = atom_pos
                     d["atom_pos_r"] = atom_pos_r
 
             bvec_cart = np.zeros([d["num_b"], 3])
             bvec_crys = np.zeros([d["num_b"], 3])
             bbmat = np.zeros([d["num_b"], 9])
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/spn.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/spn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """
-Spn manages matrix elements of Spin operator in seedname.spn file.
+Spn manages matrix elements of Pauli spin operator in seedname.spn file.
 """
+
 import os
 import gzip
 import tarfile
 
 import numpy as np
 
 from symclosestwannier.util._utility import FortranFileR, FortranFileW
 
-_default = {"num_k": 1, "num_bands": 1, "Sk": None}
+_default = {"num_k": 1, "num_bands": 1, "pauli_spn": None}
 
 
 # ==================================================
 class Spn(dict):
     """
-    Spn manages matrix elements of Spin operator in seedname.spn file.
+    Spn manages matrix elements of Pauli spin operator in seedname.spn file.
 
     Attributes:
         _topdir (str): top directory.
         _seedname (str): seedname.
         _spn_formatted (bool): formatted file?
     """
 
     # ==================================================
     def __init__(self, topdir=None, seedname="cwannier", spn_formatted=False, dic=None):
         """
-        initialize the class.
+        Spn manages matrix elements of Pauli spin operator in seedname.spn file.
 
         Args:
             topdir (str, optional): directory of seedname.spn file.
             seedname (str, optional): seedname.
             spn_formatted (bool, optional): formatted file?
             dic (dict, optional): dictionary of Spn.
         """
@@ -54,19 +55,15 @@
         Args:
             file_name (str, optional): file name.
 
         Returns:
             dict:
                 - num_k     : # of k points (int), [1].
                 - num_bands : # of bands passed to the code (int), [1].
-                - num_wann  : # of WFs (int), [1].
-                - k-points  : [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].,
-                - Uoptk     : num_wann×num_wann full unitary matrix (ndarray), [None].
-                - Udisk     : num_wann×num_bands partial unitary matrix (ndarray), [None].
-                - Uk        : num_wann×num_bands full unitary matrix (ndarray), [None].
+                - Spnk      : num_bands×num_bands matrix elementes of Pauli spin operators (ndarray), [None].
         """
         if os.path.exists(file_name):
             pass
         elif os.path.exists(file_name + ".gz"):
             pass
         elif os.path.exists(file_name + ".tar.gz"):
             pass
@@ -80,15 +77,15 @@
         else:
             f_spn_in = FortranFileR(file_name)
             SPNheader = f_spn_in.read_record(dtype="c")
             num_bands, num_k = f_spn_in.read_record(dtype=np.int32)
             SPNheader = "".join(a.decode("ascii") for a in SPNheader)
 
         indm, indn = np.tril_indices(num_bands)
-        Sk = np.zeros((3, num_k, num_bands, num_bands), dtype=complex)
+        pauli_spn = np.zeros((3, num_k, num_bands, num_bands), dtype=complex)
 
         for ik in range(num_k):
             A = np.zeros((3, num_bands, num_bands), dtype=complex)
             if self._spn_formatted:
                 tmp = np.array(
                     [f_spn_in.readline().split() for i in range(3 * num_bands * (num_bands + 1) // 2)], dtype=float
                 )
@@ -97,17 +94,20 @@
                 tmp = f_spn_in.read_record(dtype=np.complex128)
             A[:, indn, indm] = tmp.reshape(3, num_bands * (num_bands + 1) // 2, order="F")
             check = np.einsum("ijj->", np.abs(A.imag))
             A[:, indm, indn] = A[:, indn, indm].conj()
             if check > 1e-10:
                 raise RuntimeError("REAL DIAG CHECK FAILED : {0}".format(check))
 
-            Sk[:, ik, :, :] = A
+            pauli_spn[:, ik, :, :] = A
+
+        pauli_spn = pauli_spn[:, :, 120:, 120:]
+        num_bands = pauli_spn.shape[2]
 
-        d = {"num_k": num_k, "num_bands": num_bands, "Sk": Sk.tolist()}
+        d = {"num_k": num_k, "num_bands": num_bands, "pauli_spn": pauli_spn.tolist()}
 
         return d
 
     # # ==================================================
     # def write(self, file_name="cwannier.spn"):
     #     """
     #     write spn data.
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/umat.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/umat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Umat manages unitary matrix elements in seedname_u.mat (Uopt(k)) and seedname_u_dis.mat (Udis(k)) files, U(k) = Uopt(k)@Udis(k).
 - Uopt(k): num_wann×num_wann unitary matrix.
 - Udis(k): num_wann×num_bands partial unitary matrix.
 - U(k): num_wann×num_bands partial unitary matrix.
 """
+
 import os
 import gzip
 import tarfile
 import datetime
 
 import numpy as np
 
@@ -16,14 +17,15 @@
 
 
 _default = {
     "num_k": 1,
     "num_bands": 1,
     "num_wann": 1,
     "kpoints": [[0, 0, 0]],
+    "kpoints_wo_shift": [[0, 0, 0]],
     "Uoptk": None,
     "Udisk": None,
     "Uk": None,
 }
 
 
 # ==================================================
@@ -35,15 +37,15 @@
         _topdir (str): top directory.
         _seedname (str): seedname.
     """
 
     # ==================================================
     def __init__(self, topdir=None, seedname="cwannier", dic=None):
         """
-        initialize the class.
+        Umat manages unitary matrix elements in seedname_u.mat (Uopt(k)) and seedname_u_dis.mat (Udis(k)) files, U(k) = Uopt(k)@Udis(k).
 
         Args:
             topdir (str, optional): directory of seedname.amn file.
             seedname (str, optional): seedname.
             dic (dict, optional): dictionary of Amn.
         """
         super().__init__()
@@ -65,21 +67,22 @@
 
         Args:
             u_file_name (str, optional): file name for seedname_u.mat.
             u_dis_file_name (str, optional): file name for seedname_u_dis.mat.
 
         Returns:
             dict:
-                - num_k     : # of k points (int), [1].
-                - num_bands : # of bands passed to the code (int), [1].
-                - num_wann  : # of WFs (int), [1].
-                - k-points  : [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].,
-                - Uoptk     : num_wann×num_wann full unitary matrix (ndarray), [None].
-                - Udisk     : num_wann×num_bands partial unitary matrix (ndarray), [None].
-                - Uk        : num_wann×num_bands full unitary matrix (ndarray), [None].
+                - num_k            : # of k points (int), [1].
+                - num_bands        : # of bands passed to the code (int), [1].
+                - num_wann         : # of WFs (int), [1].
+                - k-points         : [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].,
+                - kpoints_wo_shift : k-points without shift, [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].
+                - Uoptk            : num_wann×num_wann full unitary matrix (ndarray), [None].
+                - Udisk            : num_wann×num_bands partial unitary matrix (ndarray), [None].
+                - Uk               : num_wann×num_bands full unitary matrix (ndarray), [None].
         """
         # Uoptk
         if os.path.exists(u_file_name):
             with open(u_file_name) as fp:
                 u_mat_data = fp.readlines()
         elif os.path.exists(u_file_name + ".gz"):
             with gzip.open(u_file_name + ".gz", "rt") as fp:
@@ -90,19 +93,21 @@
         else:
             raise Exception("failed to read u.mat file: " + u_file_name)
 
         d = Umat._default().copy()
 
         num_k, num_wann, _ = [int(x) for x in u_mat_data[1].split()]
 
-        kpoints = np.zeros([num_k, 3], dtype=float)
+        kpoints_wo_shift = np.zeros([num_k, 3], dtype=float)
         Uoptk = np.zeros([num_k, num_wann, num_wann], dtype=complex)
         u_mat_data = u_mat_data[3:]
         for k in range(num_k):
-            kpoints[k] = np.array([float(vi) for vi in u_mat_data[k * (num_wann * num_wann + 2)].split() if vi != ""])
+            kpoints_wo_shift[k] = np.array(
+                [float(vi) for vi in u_mat_data[k * (num_wann * num_wann + 2)].split() if vi != ""]
+            )
             u = u_mat_data[k * (num_wann * num_wann + 2) + 1 : k * (num_wann * num_wann + 2) + 1 + num_wann * num_wann]
             for j in range(num_wann):  # col
                 for i in range(num_wann):  # row
                     v = [float(vi) for vi in u[j * num_wann + i].split() if vi != ""]
                     Uoptk[k, i, j] = v[0] + 1j * v[1]
 
         # Udisk
@@ -157,19 +162,22 @@
                     )
                 Udisk_[ik, inside_win_true_or_false[ik]] = Udisk[ik, : num_inside_win_k[ik], :]
 
             Udisk = Udisk_
 
         Uk = Udisk @ Uoptk
 
+        kpoints = np.mod(kpoints_wo_shift, 1)  # 0 <= kj < 1.0
+
         d = {
             "num_k": num_k,
             "num_bands": num_bands,
             "num_wann": num_wann,
             "kpoints": kpoints.tolist(),
+            "kpoints_wo_shift": kpoints_wo_shift.tolist(),
             "Uoptk": Uoptk.tolist(),
             "Udisk": Udisk.tolist(),
             "Uk": Uk.tolist(),
         }
 
         return d
 
@@ -183,15 +191,15 @@
         """
         with open(file_name, "w") as fp:
             fp.write("# created by umat.py\n")
             fp.write("# written {}\n".format(datetime.datetime.now().strftime("on %d%b%Y at %H:%M:%S")))
             fp.write("{} {} {}\n\n".format(self["num_k"], self["num_wann"], self["num_wann"]))
 
             for k in range(self["num_k"]):
-                kv = self["kpoints"][k]
+                kv = self["kpoints_wo_shift"][k]
                 fp.write("{0:18.12f} {1:18.12f} {2:18.12f} \n".format(kv[0], kv[1], kv[2]))
                 for i in range(self["num_wann"]):
                     for j in range(self["num_wann"]):
                         fp.write("{0.real:18.12f}  {0.imag:18.12f} \n".format(self["Uoptk"][k][j][i]))
 
                 fp.write("\n")
 
@@ -207,15 +215,15 @@
         """
         with open(file_name, "w") as fp:
             fp.write("# created by umat.py\n")
             fp.write("# written {}\n".format(datetime.datetime.now().strftime("on %d%b%Y at %H:%M:%S")))
             fp.write("{} {} {}\n\n".format(self["num_k"], self["num_wann"], self["num_bands"]))
 
             for k in range(self["num_k"]):
-                kv = self["kpoints"][k]
+                kv = self["kpoints_wo_shift"][k]
                 fp.write("{0:18.12f} {1:18.12f} {2:18.12f} \n".format(kv[0], kv[1], kv[2]))
                 for i in range(self["num_wann"]):
                     for j in range(self["num_bands"]):
                         fp.write("{0.real:18.12f}  {0.imag:18.12f} \n".format(self["Udisk"][k][j][i]))
 
                 fp.write("\n")
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/cw/win.py` & `symclosestwannier-1.2.1/symclosestwannier/cw/win.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Win manages input file for wannier90.x, seedname.win file.
 """
+
 import os
 import numpy as np
 
 from gcoreutils.nsarray import NSArray
 
 
 _default = {
@@ -16,42 +17,55 @@
     "dis_num_iter": 0,
     "num_iter": 200,
     "dis_froz_max": +100000,
     "dis_froz_min": -100000,
     "dis_win_max": +100000,
     "dis_win_min": -100000,
     "dis_mix_ratio": 0.5,
+    "exclude_bands": None,
     #
     "mp_grid": [1, 1, 1],
     "kpoints": [[0, 0, 0]],
     "kpoint": None,
     "kpoint_path": None,
     "unit_cell_cart": None,
     "atoms_frac": None,
     "atoms_cart": None,
+    "spinors": False,
+    "spin_moment": False,
     #
     "kmesh": [1, 1, 1],
     "kmesh_spacing": [1, 1, 1],
-    "adpt_smr": True,
+    "adpt_smr": False,
     "adpt_smr_fac": np.sqrt(2),
     "adpt_smr_max": 1.0,
     "smr_type": "gauss",
     "smr_fixed_en_width": 0.0,
     "spin_decomp": False,
     # berry
     "berry": False,
     "berry_task": "",
     "berry_kmesh": [1, 1, 1],
     "berry_kmesh_spacing": [1, 1, 1],
+    # berry curvature, ahc, shc
+    "berry_curv_unit": "ang2",
+    "berry_curv_adpt_kmesh": 1,
+    "berry_curv_adpt_kmesh_thresh": 100,
+    "fermi_energy": 0.0,
+    "fermi_energy_max": None,
+    "fermi_energy_min": None,
+    "fermi_energy_step": 0.01,
+    "fermi_energy_list": None,
+    "num_fermi": 0,
     # kubo
     "kubo_freq_max": None,
     "kubo_freq_min": 0.0,
     "kubo_freq_step": 0.01,
     "kubo_eigval_max": +100000,
-    "kubo_adpt_smr": True,
+    "kubo_adpt_smr": False,
     "kubo_adpt_smr_fac": np.sqrt(2),
     "kubo_adpt_smr_max": 1.0,
     "kubo_smr_fixed_en_width": 0.0,
     "kubo_smr_type": "gauss",
     # gyrotropic
     "gyrotropic": False,
     # boltzwann
@@ -68,15 +82,15 @@
         _topdir (str): top directory.
         _seedname (str): seedname.
     """
 
     # ==================================================
     def __init__(self, topdir=None, seedname="cwannier", dic=None):
         """
-        initialize the class.
+        Win manages input file for wannier90.x, seedname.win file.
 
         Args:
             topdir (str, optional): directory of seedname.win file.
             seedname (str, optional): seedname.
             dic (dict, optional): dictionary of Win.
         """
         super().__init__()
@@ -97,64 +111,80 @@
         read seedname.win file.
 
         Args:
             file_name (str, optional): file name.
 
         Returns:
             dict: dictionary form of seedname.win.
-                - num_k               : # of k points (int), [1].
-                - num_bands           : # of bands passed to the code (int), [1].
-                - num_wann            : # of WFs (int), [1].
-                - kpoint*             : representative k points, [1].
-                - kpoint_path*        : high-symmetry line in k-space, [None].
-                - unit_cell_cart*     : transform matrix, [a1,a2,a3], [None].
-                - atoms_frac*         : atomic positions in fractional coordinates with respect to the lattice vectors, {atom: [r1,r2,r3]} [None].
-                - atoms_cart*         : atomic positions in cartesian coordinates, {atom: [rx,ry,rz]} [None].
-                - dis_num_iter*       : # of iterations for disentanglement (int), [0].
-                - num_iter*           : # of iterations for maximal localization (int), [200].
-                - dis_froz_max        : top of the inner (frozen) energy window (float), [+100000].
-                - dis_froz_min        : bottom of the inner (frozen) energy window (float), [-100000].
-                - dis_win_max         : top of the outer energy window (float), [+100000].
-                - dis_win_min         : bottom of the outer energy window (float), [-100000].
-                - dis_mix_ratio       : mixing ratio during the disentanglement (float), [0.5].
-                - mp_grid             : dimensions of the Monkhorst-Pack grid of k-points (list), [[1, 1, 1]],
-                - kpoints             : k-points used in DFT calculation, [[k1, k2, k3]] (crystal coordinate).
-                - kpoint              : representative k points (dict), [None].
-                - kpoint_path         : k-points along high symmetry line in Brillouin zonen, [[k1, k2, k3]] (crystal coordinate) (str), [None].
-                - unit_cell_cart      : transform matrix, [a1,a2,a3] (list), [None].
+                - num_k           : # of k points (int), [1].
+                - num_bands       : # of bands passed to the code (int), [1].
+                - num_wann        : # of WFs (int), [1].
+                - kpoint*         : representative k points, [1].
+                - kpoint_path*    : high-symmetry line in k-space, [None].
+                - unit_cell_cart* : transform matrix, [a1,a2,a3], [None].
+                - atoms_frac*     : atomic positions in fractional coordinates with respect to the lattice vectors, {atom: [r1,r2,r3]} [None].
+                - atoms_cart*     : atomic positions in cartesian coordinates, {atom: [rx,ry,rz]} [None].
+                - spinors         : WFs are spinors? (bool) [False].
+                - spin_moment     : Determines whether to evaluate the spin moment (bool), [False].
+                - dis_num_iter*   : # of iterations for disentanglement (int), [0].
+                - num_iter*       : # of iterations for maximal localization (int), [200].
+                - dis_froz_max    : top of the inner (frozen) energy window (float), [+100000].
+                - dis_froz_min    : bottom of the inner (frozen) energy window (float), [-100000].
+                - dis_win_max     : top of the outer energy window (float), [+100000].
+                - dis_win_min     : bottom of the outer energy window (float), [-100000].
+                - dis_mix_ratio   : mixing ratio during the disentanglement (float), [0.5].
+                - mp_grid         : dimensions of the Monkhorst-Pack grid of k-points (list), [[1, 1, 1]],
+                - kpoints         : k-points used in DFT calculation, [[k1, k2, k3]] (crystal coordinate).
+                - kpoint          : representative k points (dict), [None].
+                - kpoint_path     : k-points along high symmetry line in Brillouin zonen, [[k1, k2, k3]] (crystal coordinate) (str), [None].
+                - unit_cell_cart  : transform matrix, [a1,a2,a3] (list), [None].
 
             # only used for postcw calculation (same as postw90).
-                - kmesh               : dimensions of the Monkhorst-Pack grid of k-points for response calculation (list), [[1, 1, 1]].
-                - kmesh_spacing       : minimum distance for neighboring k points along each of the three directions in k space (The units are [Ang])(list), [1,1,1]].
-                - adpt_smr            : Determines whether to use an adaptive scheme for broadening the DOS and similar quantities defined on the energy axis (bool), [True].
-                - adpt_smr_fac        : The width ηnk of the broadened delta function used to determine the contribution to the spectral property (DOS, ...) from band n at point k (float), [sqrt(2)].
-                - adpt_smr_max        : Maximum allowed value for the adaptive energy smearing [eV] (float), [1.0].
-                - smr_type            : Defines the analytical form used for the broadened delta function in the computation of the DOS and similar quantities defined on the energy axis, gauss/m-pN/m-v or cold/f-d (str), [gauss].
-                - smr_fixed_en_width  : Energy width for the smearing function for the DOS. Used only if adpt_smr is false (The units are [eV]) (flaot), [0.0].
-                - spin_decomp         : If true, extra columns are added to some output files (such as seedname-dos.dat for the dos module, and analogously for the berry and BoltzWann modules) (bool), [False].
+                - kmesh                        : dimensions of the Monkhorst-Pack grid of k-points for response calculation (list), [[1, 1, 1]].
+                - kmesh_spacing                : minimum distance for neighboring k points along each of the three directions in k space (The units are [Ang])(list), [1,1,1]].
+                - adpt_smr                     : Determines whether to use an adaptive scheme for broadening the DOS and similar quantities defined on the energy axis (bool), [True].
+                - adpt_smr_fac                 : The width ηnk of the broadened delta function used to determine the contribution to the spectral property (DOS, ...) from band n at point k (float), [sqrt(2)].
+                - adpt_smr_max                 : Maximum allowed value for the adaptive energy smearing [eV] (float), [1.0].
+                - smr_type                     : Defines the analytical form used for the broadened delta function in the computation of the DOS and similar quantities defined on the energy axis, gauss/m-pN/m-v or cold/f-d (str), [gauss].
+                - smr_fixed_en_width           : Energy width for the smearing function for the DOS. Used only if adpt_smr is false (The units are [eV]) (flaot), [0.0].
+                - spin_decomp                  : If true, extra columns are added to some output files (such as seedname-dos.dat for the dos module, and analogously for the berry and BoltzWann modules) (bool), [False].
+
             # berry
-                - berry               : Determines whether to enter the berry routines (bool), [False].
-                - berry_task          : The quantity to compute when berry=true, ahc/morb/kubo/sc/shc/kdotp/me (str).
-                - berry_kmesh         : Overrides the kmesh global variable.
-                - berry_kmesh_spacing : Overrides the kmesh_spacing global variable.
+                - berry                        : Determines whether to enter the berry routines (bool), [False].
+                - berry_task                   : The quantity to compute when berry=true, ahc/morb/kubo/sc/shc/kdotp/me (str).
+                - berry_kmesh                  : Overrides the kmesh global variable.
+                - berry_kmesh_spacing          : Overrides the kmesh_spacing global variable.
+
+            # berry curvature, ahc, shc
+                - berry_curv_unit              : Unit of Berry curvature, ang2/bohr2, ['ang2'].
+                - berry_curv_adpt_kmesh        : Linear dimension of the adaptively refined k-mesh used to compute the anomalous/spin Hall conductivity, [1].
+                - berry_curv_adpt_kmesh_thresh : Threshold magnitude of the Berry curvature for adaptive refinement, [100].
+                - fermi_energy                 : fermi energy (float), [0.0].
+                - fermi_energy_max             : Upper limit of the Fermi energy range (float), [None].
+                - fermi_energy_min             : Lower limit of the Fermi energy range (float), [None].
+                - fermi_energy_step            : Step for increasing the Fermi energy in the specified range. (The units are [eV]) (float), [0.01].
+                - fermi_energy_list            : list of fermi energy (list), [None].
+                - num_fermi                    : number of fermi energies (int), [0].
+
             # kubo
-                - kubo_freq_max       : Upper limit of the frequency range for computing the optical conductivity, JDOS and ac SHC. (The units are [eV]) (float), [If an inner energy window was specified, the default value is dis_froz_max-fermi_energy+0.6667. Otherwise it is the difference between the maximum and the minimum energy eigenvalue stored in seedname.eig, plus 0.6667.].
-                - kubo_freq_min       : Lower limit of the frequency range for computing the optical conductivity, JDOS and ac SHC. (The units are [eV]) (float), [0.0].
-                - kubo_freq_step      : Difference between consecutive values of the optical frequency between kubo_freq_min and kubo_freq_max. (The units are [eV]) (float), [0.01].
-                - kubo_eigval_max     : Maximum energy eigenvalue of the eigenstates to be included in the evaluation of the optical conductivity, JDOS and ac SHC. (The units are [eV]) (float), [If an inner energy window was specified, the default value is the upper bound of the inner energy window plus 0.6667. Otherwise it is the maximum energy eigenvalue stored in seedname.eig plus 0.6667.].
-                - kubo_adpt_smr       : Overrides the adpt_smr global variable.
-                - kubo_adpt_smr_fac   : Overrides the adpt_smr_fac global variable.
-                - kubo_adpt_smr_max   : Overrides the adpt_smr_max global variable.
+                - kubo_freq_max           : Upper limit of the frequency range for computing the optical conductivity, JDOS and ac SHC. (The units are [eV]) (float), [If an inner energy window was specified, the default value is dis_froz_max-fermi_energy+0.6667. Otherwise it is the difference between the maximum and the minimum energy eigenvalue stored in seedname.eig, plus 0.6667.].
+                - kubo_freq_min           : Lower limit of the frequency range for computing the optical conductivity, JDOS and ac SHC. (The units are [eV]) (float), [0.0].
+                - kubo_freq_step          : Difference between consecutive values of the optical frequency between kubo_freq_min and kubo_freq_max. (The units are [eV]) (float), [0.01].
+                - kubo_eigval_max         : Maximum energy eigenvalue of the eigenstates to be included in the evaluation of the optical conductivity, JDOS and ac SHC. (The units are [eV]) (float), [If an inner energy window was specified, the default value is the upper bound of the inner energy window plus 0.6667. Otherwise it is the maximum energy eigenvalue stored in seedname.eig plus 0.6667.].
+                - kubo_adpt_smr           : Overrides the adpt_smr global variable.
+                - kubo_adpt_smr_fac       : Overrides the adpt_smr_fac global variable.
+                - kubo_adpt_smr_max       : Overrides the adpt_smr_max global variable.
                 - kubo_smr_fixed_en_width : Overrides the smr_fixed_en_width global variable.
-                - kubo_smr_type       : Overrides the smr_type global variable.
-            # ahc
+                - kubo_smr_type           : Overrides the smr_type global variable.
+
             # morb
-            # shc
+
             # gyrotropic
                 - gyrotropic          : Determines whether to enter the gyrotropic routines (bool), [False].
+
             # boltzwann
                 - boltzwann           : Determines whether to enter the boltzwann routines (bool), [False].
         """
         if os.path.exists(file_name):
             with open(file_name) as fp:
                 win_data = fp.readlines()
         else:
@@ -177,25 +207,29 @@
             d["dis_num_iter"] = 0
         d["num_iter"] = self._get_param_keyword(win_data, "num_iter", 200, dtype=int)
         d["dis_froz_max"] = self._get_param_keyword(win_data, "dis_froz_max", +100000, dtype=float)
         d["dis_froz_min"] = self._get_param_keyword(win_data, "dis_froz_min", -100000, dtype=float)
         d["dis_win_max"] = self._get_param_keyword(win_data, "dis_win_max", +100000, dtype=float)
         d["dis_win_min"] = self._get_param_keyword(win_data, "dis_win_min", -100000, dtype=float)
         d["dis_mix_ratio"] = self._get_param_keyword(win_data, "dis_mix_ratio", 0.5, dtype=float)
+        d["exclude_bands"] = self._get_param_keyword(win_data, "exclude_bands", None, dtype=str)
+
+        d["spinors"] = self._get_param_keyword(win_data, "spinors", False, dtype=bool)
+        d["spin_moment"] = self._get_param_keyword(win_data, "spin_moment", False, dtype=bool)
 
         for i, line in enumerate(win_data_lower):
             if "begin kpoints" in line:
                 kpoints = np.genfromtxt(win_data[i + 1 : i + 1 + d["num_k"]], dtype=float)
                 kpoints = np.mod(kpoints, 1)  # 0 <= kj < 1.0
                 if kpoints.ndim == 1:
                     d["kpoints"] = [kpoints.tolist()]
                 else:
                     d["kpoints"] = kpoints.tolist()
 
-                d["kpoints"] = [kpt[:3] for kpt in kpoints]
+                d["kpoints"] = [kpt[:3] for kpt in d["kpoints"]]
 
             if "begin kpoint_path" in line:
                 k_data = win_data[i + 1 : win_data_lower.index("end kpoint_path")]
                 k_data = [[vi for vi in v.split()] for v in k_data]
                 kpoint = {}
                 kpoint_path = ""
                 cnt = 1
@@ -287,15 +321,15 @@
         d["atoms_frac_shift"] = {k: [float(v[0]), float(v[1]), float(v[2])] for k, v in dic.items()}
 
         # postcw
         kmesh = self._get_param_keyword(win_data, "kmesh", "1  1  1", dtype=str)
         d["kmesh"] = [int(x) for x in kmesh.split()]
         kmesh_spacing = self._get_param_keyword(win_data, "kmesh_spacing", "1  1  1", dtype=str)
         d["kmesh_spacing"] = [int(x) for x in kmesh_spacing.split()]
-        d["adpt_smr"] = self._get_param_keyword(win_data, "adpt_smr", True, dtype=bool)
+        d["adpt_smr"] = self._get_param_keyword(win_data, "adpt_smr", False, dtype=bool)
         d["adpt_smr_fac"] = self._get_param_keyword(win_data, "adpt_smr_fac", np.sqrt(2), dtype=float)
         d["adpt_smr_max"] = self._get_param_keyword(win_data, "adpt_smr_max", 1.0, dtype=float)
         d["smr_type"] = self._get_param_keyword(win_data, "smr_type", "gauss", dtype=str).replace(" ", "")
         d["smr_fixed_en_width"] = self._get_param_keyword(win_data, "smr_fixed_en_width", 0.0, dtype=float)
         d["spin_decomp"] = self._get_param_keyword(win_data, "spin_decomp", False, dtype=bool)
 
         d["berry"] = self._get_param_keyword(win_data, "berry", False, dtype=bool)
@@ -308,31 +342,85 @@
         berry_kmesh_spacing = self._get_param_keyword(win_data, "berry_kmesh_spacing", "1  1  1", dtype=str)
         d["berry_kmesh_spacing"] = [int(x) for x in berry_kmesh_spacing.split()]
 
         d["kubo_freq_max"] = self._get_param_keyword(win_data, "kubo_freq_max", 1.0, dtype=float)
         d["kubo_freq_min"] = self._get_param_keyword(win_data, "kubo_freq_min", 0.0, dtype=float)
         d["kubo_freq_step"] = self._get_param_keyword(win_data, "kubo_freq_step", 0.01, dtype=float)
         d["kubo_eigval_max"] = self._get_param_keyword(win_data, "kubo_eigval_max", +100000, dtype=float)
-        d["kubo_adpt_smr"] = self._get_param_keyword(win_data, "kubo_adpt_smr", True, dtype=bool)
+        d["kubo_adpt_smr"] = self._get_param_keyword(win_data, "kubo_adpt_smr", False, dtype=bool)
         d["kubo_adpt_smr_fac"] = self._get_param_keyword(win_data, "kubo_adpt_smr_fac", np.sqrt(2), dtype=float)
         d["kubo_adpt_smr_max"] = self._get_param_keyword(win_data, "kubo_adpt_smr_max", 1.0, dtype=float)
         d["kubo_smr_type"] = self._get_param_keyword(win_data, "smr_type", "gauss", dtype=str).replace(" ", "")
         d["kubo_smr_fixed_en_width"] = self._get_param_keyword(win_data, "kubo_smr_fixed_en_width", 0.0, dtype=float)
 
         d["gyrotropic"] = self._get_param_keyword(win_data, "gyrotropic", False, dtype=bool)
         d["boltzwann"] = self._get_param_keyword(win_data, "boltzwann", False, dtype=bool)
 
+        num_fermi = 0
+        found_fermi_energy = False
+        fermi_energy_max = 0.0
+        fermi_energy_min = 0.0
+        fermi_energy_step = 0.0
+        fermi_energy_list = []
+
+        fermi_energy = self._get_param_keyword(win_data, "fermi_energy", 0.0, dtype=float)
+
+        if fermi_energy is not None:
+            # found_fermi_energy = True
+            num_fermi = 1
+
+        fermi_energy_scan = False
+        fermi_energy_min = self._get_param_keyword(win_data, "fermi_energy_min", None, dtype=float)
+        if fermi_energy_min is not None:
+            if found_fermi_energy:
+                raise Exception("Error: Cannot specify both fermi_energy and fermi_energy_min")
+
+            fermi_energy_scan = True
+            fermi_energy_max = fermi_energy_min + 1.0
+            fermi_energy_max = self._get_param_keyword(win_data, "fermi_energy_max", None, dtype=float)
+
+            if fermi_energy_max is not None and fermi_energy_max <= fermi_energy_min:
+                raise Exception("Error: fermi_energy_max must be larger than fermi_energy_min")
+
+            fermi_energy_step = 0.01
+            fermi_energy_step = self._get_param_keyword(win_data, "fermi_energy_step", None, dtype=float)
+
+            if fermi_energy_step is not None and fermi_energy_step <= 0.0:
+                raise Exception("Error: fermi_energy_step must be positive")
+
+            num_fermi = int(abs((fermi_energy_max - fermi_energy_min) / fermi_energy_step)) + 1
+
+        if found_fermi_energy:
+            fermi_energy_list = [fermi_energy]
+        elif fermi_energy_scan:
+            if num_fermi == 1:
+                fermi_energy_step = 0.0
+            else:
+                fermi_energy_step = (fermi_energy_max - fermi_energy_min) / float(num_fermi - 1)
+
+            fermi_energy_list = [fermi_energy_min + i * fermi_energy_step for i in range(num_fermi)]
+        else:
+            fermi_energy_list = [0.0]
+
+        d["fermi_energy"] = fermi_energy
+        d["fermi_energy_max"] = fermi_energy_max
+        d["fermi_energy_min"] = fermi_energy_min
+        d["fermi_energy_step"] = fermi_energy_step
+        d["fermi_energy_list"] = fermi_energy_list
+        d["num_fermi"] = num_fermi
+
         return d
 
     # ==================================================
     def _get_param_keyword(self, lines, keyword, default_value=None, dtype=int):
         data = None
         keys = []
         for line in lines:
             line = line.replace("\n", "")
+            line = line.lstrip()
             if line.startswith(keyword):
                 if len(line.split("=")) > 1:
                     key = line.split("=")[0]
                     key = key.replace(" ", "")
                     if key == keyword:
                         data = line.split("=")[1].split("!")[0]
                     assert key not in keys, key + " is defined more than once"
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/scripts/postcw.py` & `symclosestwannier-1.2.1/symclosestwannier/scripts/postcw.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.9/symclosestwannier/scripts/pw2cw.py` & `symclosestwannier-1.2.1/symclosestwannier/scripts/pw2cw.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 # ================================================== pw2cw
 @click.command()
 @click.option("-i", "--input", is_flag=True, help="Show input format, and exit.")
 @click.option("-v", "--version", is_flag=True, help="Show version, and exit.")
 @click.argument("seedname", nargs=-1)
 def cmd(seedname, input, version):
     """
+    run pw2cw.
+
     create Closest Wannier tight-binding model from input.
 
         seedname : seedname for seedname.cwin file (w or w/o `.cwin`).
     """
     if input:
         click.echo(cwin_header)
         exit()
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/util/_utility.py` & `symclosestwannier-1.2.1/symclosestwannier/util/_utility.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 """
 utility codes.
 """
 
 import numpy as np
+from sympy.physics.quantum import TensorProduct
 import fortio, scipy.io
+import multiprocessing
+from joblib import Parallel, delayed, wrap_non_picklable_objects
 
 from gcoreutils.nsarray import NSArray
 
+from symclosestwannier.util.constants import bohr_magn_SI, joul_to_eV
+
 M_ZERO = np.finfo(float).eps
 
+_num_proc = multiprocessing.cpu_count()
+
 
 # ==================================================
 class FortranFileR(fortio.FortranFile):
     def __init__(self, filename):
         try:
             super().__init__(filename, mode="r", header_dtype="uint32", auto_endian=True, check_file=True)
         except ValueError:
@@ -28,17 +35,17 @@
 
 # ==================================================
 def is_zero(x):
     return np.abs(x) < M_ZERO * 100
 
 
 # ==================================================
-def fermi(x, T=0.01):
+def fermi(x, T=0.0):
     if T == 0.0:
-        return x < 0.0
+        return np.vectorize(float)(x < 0.0)
 
     return 0.5 * (1.0 - np.tanh(0.5 * x / T))
 
 
 # ==================================================
 def fermi_dt(x, T=0.01):
     return fermi(x, T) * fermi(-x, T) / T
@@ -52,14 +59,77 @@
 # ==================================================
 def weight_proj(e, e0, e1, T0, T1, delta=10e-12):
     """weight function for projection"""
     return fermi(e0 - e, T0) + fermi(e - e1, T1) - 1.0 + delta
 
 
 # ==================================================
+def convert_w90_orbital(l, m, r, s):
+    """
+    convert orbital in the Wannier90 format into the MultiPie format.
+
+    Args:
+        nw2l (list): l specifies the angular part Θlm(θ, φ).
+        nw2m (list): m specifies the angular part Θlm(θ, φ).
+        nw2r (list): r specifies the radial part Rr(r).
+        nw2s (list): s specifies the spin, 1(up)/-1(dn).
+
+    Returns:
+        str: converted orbital.
+    """
+    orbital = ""
+
+    if l == 0 and m == 1:
+        orbital = "s"
+    elif l == 1:
+        if m == 1:
+            orbital = "pz"
+        elif m == 2:
+            orbital = "px"
+        elif m == 3:
+            orbital = "py"
+    elif l == 2:
+        if m == 1:
+            orbital = "du"  # dz2
+        elif m == 2:
+            orbital = "dzx"  # dxz
+        elif m == 3:
+            orbital = "dyz"
+        elif m == 4:
+            orbital = "dv"  # dx2-y2
+        elif m == 5:
+            orbital = "dxy"
+    elif l == 3:
+        if m == 1:
+            orbital = "faz"  # fz3
+        elif m == 2:
+            orbital = "fx"  # fxz2
+        elif m == 3:
+            orbital = "fy"  # fyz2
+        elif m == 4:
+            orbital = "fbz"  # fz(x2-y2)
+        elif m == 5:
+            orbital = "fxyz"
+        elif m == 6:
+            orbital = "f2"  # fx(x2-3y2)
+        elif m == 7:
+            orbital = "f1"  # fy(3x2-y2)
+
+    if orbital == "":
+        raise Exception(f"invalid orbital projection was given, (l={l},m={m},r={r},s={s}).")
+
+    if s == 1:
+        orbital = f"({orbital},U)".replace("'", "")
+    elif s == -1:
+        orbital = f"({orbital},D)".replace("'", "")
+
+    return orbital
+
+
+# ==================================================
 def iterate_nd(size, pm=False):
     a = -size[0] if pm else 0
     b = size[0] + 1 if pm else size[0]
     if len(size) == 1:
         return np.array([(i,) for i in range(a, b)])
     else:
         return np.array([(i,) + tuple(j) for i in range(a, b) for j in iterate_nd(size[1:], pm=pm)])
@@ -163,14 +233,15 @@
     irvec = np.array(irvec, dtype=float)
     Nr = irvec.shape[0]
     if ndegen is None:
         weight = np.array([1.0 for i in range(Nr)])
     else:
         ndegen = np.array(ndegen)
         weight = np.array([1.0 / ndegen[i] for i in range(Nr)])
+
     kpoints = np.array(kpoints, dtype=float)
 
     kR = np.einsum("ka,Ra->kR", kpoints, irvec, optimize=True)
     phase_R = np.exp(+2 * np.pi * 1j * kR)
 
     if atoms_frac is not None:
         tau = np.array(atoms_frac)
@@ -181,35 +252,95 @@
     else:
         Ok = np.einsum("R,kR,Rmn->kmn", weight, phase_R, Or, optimize=True)
 
     return Ok
 
 
 # ==================================================
-def fourier_transform_r_to_k_vec(Or_vec, kpoints, irvec, ndegen=None, atoms_frac=None):
+def fourier_transform_r_to_k_vec(
+    Or_vec, kpoints, irvec, ndegen=None, atoms_frac=None, unit_cell_cart=None, pseudo=False
+):
     """
     fourier transformation of an arbitrary operator from real-space representation into k-space representation.
 
     Args:
         Or_vec (ndarray): real-space representation of the given operator, [O_{ab}^{x}(R), O_{ab}^{y}(R), O_{ab}^{z}(R)].
         kpoints (ndarray): k-points used in DFT calculation, [[k1, k2, k3]] (crystal coordinate).
         irvec (ndarray): irreducible R vectors (crystal coordinate, [[n1,n2,n3]], nj: integer).
         ndegen (ndarray, optional): number of degeneracy at each R.
         atoms_frac (ndarray, optional): atom's position in fractional coordinates.
+        unit_cell_cart (ndarray): transform matrix, [a1,a2,a3], [None].
+        pseudo (bool, optional): calculate pseudo vector?
 
     Returns:
         ndarray: k-space representation of the given operator, O_{ab}(k) = <φ_{a}(k)|O|φ_{b}(k)>.
     """
-    Ok_x = fourier_transform_r_to_k(Or_vec[0], kpoints, irvec, ndegen, atoms_frac)
-    Ok_y = fourier_transform_r_to_k(Or_vec[1], kpoints, irvec, ndegen, atoms_frac)
-    Ok_z = fourier_transform_r_to_k(Or_vec[2], kpoints, irvec, ndegen, atoms_frac)
+    Or_vec = np.array(Or_vec, dtype=complex)
+    irvec = np.array(irvec, dtype=float)
+    Nr = irvec.shape[0]
+    if ndegen is None:
+        weight = np.array([1.0 for _ in range(Nr)])
+    else:
+        ndegen = np.array(ndegen)
+        weight = np.array([1.0 / ndegen[i] for i in range(Nr)])
+    kpoints = np.array(kpoints, dtype=float)
+
+    kR = np.einsum("ka,Ra->kR", kpoints, irvec, optimize=True)
+    phase_R = np.exp(+2 * np.pi * 1j * kR)
+
+    if atoms_frac is not None:
+        tau = np.array(atoms_frac)
+        ktau = np.einsum("ka,ma->km", kpoints, tau, optimize=True)
+        eiktau = np.exp(-2 * np.pi * 1j * ktau)
+
+        Ok_true_vec = np.einsum(
+            "R,kR,km,aRmn,kn->akmn", weight, phase_R, eiktau, Or_vec, eiktau.conjugate(), optimize=True
+        )
+    else:
+        Ok_true_vec = np.einsum("R,kR,aRmn->akmn", weight, phase_R, Or_vec, optimize=True)
+
+    if not pseudo:
+        return Ok_true_vec
+    else:
+        A = np.array(unit_cell_cart)
+        irvec_cart = np.array([np.array(R) @ np.array(A) for R in irvec])
 
-    Ok_vec = np.array([Ok_x, Ok_y, Ok_z])
+        Ok_pseudo_vec = np.zeros(Ok_true_vec.shape, dtype=np.complex128)
+        ab_list = [(1, 2), (2, 0), (0, 1)]
+        if atoms_frac is not None:
+            atoms_cart = np.array([np.array(r) @ np.array(A) for r in atoms_frac])
+            bond_cart = np.array([[[(R + rn) - rm for rn in atoms_cart] for rm in atoms_cart] for R in irvec_cart])
+            for c, (a, b) in enumerate(ab_list):
+                Ok_pseudo_vec[c] = 1.0j * np.einsum(
+                    "R,kR,Rmn,km,Rmn,kn->kmn",
+                    weight,
+                    phase_R,
+                    bond_cart[:, :, :, a],
+                    eiktau,
+                    Or_vec[b],
+                    eiktau.conjugate(),
+                    optimize=True,
+                )
+                -1.0j * np.einsum(
+                    "R,kR,Rmn,km,Rmn,kn->kmn",
+                    weight,
+                    phase_R,
+                    bond_cart[:, :, :, b],
+                    eiktau,
+                    Or_vec[a],
+                    eiktau.conjugate(),
+                    optimize=True,
+                )
+        else:
+            for c, (a, b) in enumerate(ab_list):
+                Ok_pseudo_vec[c] = 1.0j * np.einsum(
+                    "R,kR,R,Rmn->kmn", weight, phase_R, irvec_cart[:, a], Or_vec[b], optimize=True
+                ) - 1.0j * np.einsum("R,kR,R,Rmn->kmn", weight, phase_R, irvec_cart[:, b], Or_vec[a], optimize=True)
 
-    return Ok_vec
+        return Ok_true_vec, Ok_pseudo_vec
 
 
 # ==================================================
 def fourier_transform_r_to_k_new(Or, kpoints, unit_cell_cart, irvec, ndegen=None, atoms_frac=None):
     """
     fourier transformation of an arbitrary operator from real-space representation into k-space representation.
 
@@ -448,85 +579,80 @@
 def samb_decomp_operator(
     Or_dict, Zr_dict, A=None, atoms_frac=None, ket=None, A_samb=None, atoms_frac_samb=None, ket_samb=None
 ):
     """
     decompose arbitrary operator into linear combination of SAMBs.
 
     Args:
-        Or_dict (dict): dictionary form of an arbitrary operator matrix in reak-space/k-space representation.
+        Or_dict (dict): dictionary form of an arbitrary operator matrix in real-space/k-space representation.
         Zr_dict (dict): dictionary form of SAMBs.
         A (list/ndarray, optional): real lattice vectors for the given operator, A = [a1,a2,a3] (list), [[[1,0,0], [0,1,0], [0,0,1]]].
         atoms_frac (ndarray, optional): atom's position in fractional coordinates for the given operator.
         ket (list, optional): ket basis list, orbital@site.
         A_samb (list/ndarray, optional): real lattice vectors for SAMBs, A = [a1,a2,a3] (list), [[[1,0,0], [0,1,0], [0,0,1]]].
         atoms_frac_samb (ndarray, optional): atom's position in fractional coordinates for SAMBs.
         ket_samb (list, optional): ket basis list for SAMBs, orbital@site.
 
     Returns:
         z (dict): parameter set, {tag: z_j}.
     """
     Or_dict = sort_ket_matrix_dict(Or_dict, ket, ket_samb)
 
-    if A is None or (A is not None and np.allclose(A, A_samb, rtol=1e-05, atol=1e-05)):
-        z = {
-            tag: np.real(np.sum([v * Or_dict.get((-k[0], -k[1], -k[2], k[4], k[3]), 0) for k, v in d.items()]))
-            for tag, d in Zr_dict.items()
-        }
-    else:
-        A = np.array(A, dtype=float)
-        A_samb = np.array(A_samb, dtype=float)
-        atoms_frac = np.array(sort_ket_list(atoms_frac, ket, ket_samb), dtype=float)
-        atoms_frac_samb = np.array(atoms_frac_samb, dtype=float)
-
-        Or = {}
-        for (R1, R2, R3, m, n), v in Or_dict.items():
-            if np.abs(v) < 1e-12:
-                continue
-
-            R = np.array([R1, R2, R3], dtype=float)
-            rm = atoms_frac[m]
-            rn = atoms_frac[n]
-            bond = (R + rm - rn) @ A
-
-            if (m, n) in Or:
-                Or[(m, n)].append((bond, R1, R2, R3, v))
-            else:
-                Or[(m, n)] = [(bond, R1, R2, R3, v)]
-
-        Zr_dict_ = {}
-        for tag, d in Zr_dict.items():
-            dic = {}
-            for (R1, R2, R3, m, n), v in d.items():
+    if A is not None:
+        if not np.allclose(A, A_samb, rtol=1e-03, atol=1e-03):
+            print("yes!!!")
+            print(A)
+            print(A_samb)
+            A = np.array(A, dtype=float)
+            A_samb = np.array(A_samb, dtype=float)
+            atoms_frac = np.array(sort_ket_list(atoms_frac, ket, ket_samb), dtype=float)
+            atoms_frac_samb = np.array(atoms_frac_samb, dtype=float)
+
+            Or_dict_ = {}
+            for (R1, R2, R3, m, n), v in Or_dict.items():
                 if np.abs(v) < 1e-12:
                     continue
 
                 R = np.array([R1, R2, R3], dtype=float)
-                rm = atoms_frac_samb[m]
-                rn = atoms_frac_samb[n]
-                bond = (R + rm - rn) @ A_samb
-
-                if (m, n) in dic:
-                    dic[(m, n)].append((bond, R1, R2, R3, v))
-                else:
-                    dic[(m, n)] = [(bond, R1, R2, R3, v)]
-
-            Zr_dict_[tag] = dic
-
-        z = {
-            tag: np.sum(
-                [
-                    np.real(v * v_)
-                    for m, n in d.keys()
-                    for bond, R1, R2, R3, v in d[(m, n)]
-                    for bond_, R1_, R2_, R3_, v_ in Or[(n, m)]
-                    if np.allclose(bond, -bond_, rtol=1e-04, atol=1e-04)
-                ]
-            )
-            for tag, d in Zr_dict_.items()
-        }
+                rm = atoms_frac[m]
+                rn = atoms_frac[n]
+                bond = ((R + rn) - rm) @ A
+
+                bond = tuple([format(bi, ".2f") for bi in bond])
+                bond = tuple([float(bi) for bi in bond])
+
+                Or_dict_[(*bond, m, n)] = v
+
+            Or_dict = Or_dict_
+
+            Zr_dict_ = {}
+            for tag, d in Zr_dict.items():
+                dic = {}
+                for (R1, R2, R3, m, n), v in d.items():
+                    if np.abs(v) < 1e-12:
+                        continue
+
+                    R = np.array([R1, R2, R3], dtype=float)
+                    rm = atoms_frac_samb[m]
+                    rn = atoms_frac_samb[n]
+                    bond = ((R + rn) - rm) @ A_samb
+
+                    bond = tuple([format(bi, ".2f") for bi in bond])
+                    bond = tuple([float(bi) for bi in bond])
+
+                    dic[(*bond, m, n)] = v
+
+                Zr_dict_[tag] = dic
+
+            Zr_dict = Zr_dict_
+
+    z = {
+        tag: np.real(np.sum([v * Or_dict.get((-k[0], -k[1], -k[2], k[4], k[3]), 0) for k, v in d.items()]))
+        for tag, d in Zr_dict.items()
+    }
 
     return z
 
 
 # ==================================================
 def construct_Or(z, num_wann, rpoints, matrix_dict):
     """
@@ -541,15 +667,16 @@
     Returns:
         ndarray: matrix, [#r, dim, dim].
     """
     Or_dict = {(n1, n2, n3, a, b): 0.0 for (n1, n2, n3) in rpoints for a in range(num_wann) for b in range(num_wann)}
     for j, d in enumerate(matrix_dict["matrix"].values()):
         zj = z[j]
         for (n1, n2, n3, a, b), v in d.items():
-            Or_dict[(n1, n2, n3, a, b)] += zj * v
+            if (n1, n2, n3, a, b) in Or_dict:
+                Or_dict[(n1, n2, n3, a, b)] += zj * v
 
     Or = np.array(
         [
             [[Or_dict.get((n1, n2, n3, a, b), 0.0) for b in range(num_wann)] for a in range(num_wann)]
             for (n1, n2, n3) in rpoints
         ]
     )
@@ -583,46 +710,127 @@
     Or = construct_Or(z, num_wann, rpoints, matrix_dict)
     Ok = fourier_transform_r_to_k(Or, kpoints, rpoints, atoms_frac=atoms_frac)
 
     return Ok
 
 
 # ==================================================
-def thermal_avg(O, E, U, ef=0.0, T=0.0):
+def thermal_avg(O, E, U, ef=0.0, T=0.0, num_k=0):
     """
     thermal average of the given operator,
     <O> = 1 / Nk * \sum_{n,k} fermi_dirac[E_{n}(k)] O_{nn}(k)
 
     Args:
         O (ndarray): operator or list of operator.
         E (ndarray): eigen values.
         U (ndarray): eigen vectors.
         ef (float, optional): fermi energy.
         T (float, optional): temperature.
 
     Returns:
         ndarray: thermal average of the given operator.
     """
+    if type(O) != list:
+        single_operator = True
+        O = [O]
+    else:
+        single_operator = False
+
+    if ef is None:
+        ef = 0.0
+
     fk = fermi(E - ef, T)
 
     O = np.array(O)
     E = np.array(E)
     U = np.array(U)
 
-    num_k = E.shape[0]
-
-    if O.ndim == 2:
-        O = np.array([O])
+    if num_k == 0:
+        num_k = E.shape[0]
 
     O_exp = []
     for i, Oi in enumerate(O):
         UdoU = U.transpose(0, 2, 1).conjugate() @ Oi @ U
         UdoU_diag = np.diagonal(UdoU.transpose(1, 2, 0))
         Oi_exp = np.sum(fk * UdoU_diag) / num_k
         O_exp.append(np.real(Oi_exp))
 
         if np.imag(Oi_exp) > 1e-7:
             raise Exception(f"expectation value of {i+1}th operator is wrong : {Oi_exp}")
 
-    O_exp = np.array(O_exp)
+    if single_operator:
+        O_exp = O_exp[0]
+    else:
+        O_exp = np.array(O_exp)
 
     return O_exp
+
+
+# ==================================================
+def Rx(theta):
+    return np.array(
+        [
+            [1, 0, 0],
+            [0, np.cos(theta), -np.sin(theta)],
+            [0, np.sin(theta), np.cos(theta)],
+        ]
+    )
+
+
+def Ry(theta):
+    return np.array(
+        [
+            [np.cos(theta), 0, np.sin(theta)],
+            [0, 1, 0],
+            [-np.sin(theta), 0, np.cos(theta)],
+        ]
+    )
+
+
+def Rz(theta):
+    return np.array(
+        [
+            [np.cos(theta), -np.sin(theta), 0],
+            [np.sin(theta), np.cos(theta), 0],
+            [0, 0, 1],
+        ]
+    )
+
+
+# ==================================================
+def pauli_spn_x(dim):
+    Identity = np.eye(int(dim / 2))
+    sig_x = np.array([[0.0, 1.0], [1.0, 0.0]])
+    return TensorProduct(Identity, sig_x)
+
+
+# ==================================================
+def pauli_spn_y(dim):
+    Identity = np.eye(int(dim / 2))
+    sig_y = np.array([[0.0, -1.0j], [1.0j, 0.0]])
+    return TensorProduct(Identity, sig_y)
+
+
+# ==================================================
+def pauli_spn_z(dim):
+    Identity = np.eye(int(dim / 2))
+    sig_z = np.array([[1.0, 0.0], [0.0, -1.0]])
+    return TensorProduct(Identity, sig_z)
+
+
+# ==================================================
+def spn_operator(pauli_spn=None, g_factor=2.0, dim=2):
+    if pauli_spn is None:
+        pauli_spn = np.array([pauli_spn_x(dim), pauli_spn_y(dim), pauli_spn_z(dim)])
+
+    mu_B = bohr_magn_SI * joul_to_eV
+    return -0.5 * g_factor * mu_B * pauli_spn
+
+
+# ==================================================
+def spin_zeeman_interaction(B, theta=0.0, phi=0.0, pauli_spn=None, g_factor=2.0, dim=2):
+    spin_oper = spn_operator(pauli_spn, g_factor, dim)
+    B_vec = B * np.array([np.sin(theta) * np.cos(phi), np.sin(theta) * np.sin(phi), np.cos(theta)])
+
+    H_zeeman = -sum([spin_oper[i] * B_vec[i] for i in range(3)])
+
+    return H_zeeman
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/util/band.py` & `symclosestwannier-1.2.1/symclosestwannier/util/band.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.9/symclosestwannier/util/get_oper_R.py` & `symclosestwannier-1.2.1/symclosestwannier/util/get_oper_R.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # ==================================================
 def get_oper_R(name, cwi):
     """
     wrapper for getting matrix elements of the operator.
 
     Args:
-        cwi (SystemInfo): CWInfo.
+        cwi (CWInfo): CWInfo.
 
     Returns:
         ndarray: matrix elements of the operator.
     """
     d = {
         "HH_R": get_HH_R,  # <0n|H|Rm>
         "AA_R": get_AA_R,  # <0n|r|Rm>
@@ -52,15 +52,15 @@
 
 # ==================================================
 def get_HH_R(cwi):
     """
     matrix elements of real-space Hamiltonian, <0n|H|Rm>.
 
     Args:
-        cwi (SystemInfo): CWInfo.
+        cwi (CWInfo): CWInfo.
 
     Returns:
         ndarray: Hamiltonian, HH_R(len(irvec), num_wann, num_wann).
     """
     Ek = np.array(cwi["Ek"])
     Uk = np.array(cwi["Uk"])
     num_k = cwi["num_k"]
@@ -68,32 +68,32 @@
     diag_Ek = np.array([np.diag(Ek[k]) for k in range(num_k)])
     HH_k = Uk.transpose(0, 2, 1).conjugate() @ diag_Ek @ Uk
     HH_k = 0.5 * (HH_k + np.einsum("kmn->knm", HH_k).conj())
 
     kpoints = np.array(cwi["kpoints"])
     irvec = np.array(cwi["irvec"])
 
-    # if cwi["tb_gauge"]:
-    #     atoms_list = list(cwi["atoms_frac"].values())
-    #     atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
-    # else:
-    #     atoms_frac = None
+    if cwi["tb_gauge"]:
+        atoms_list = list(cwi["atoms_frac"].values())
+        atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
+    else:
+        atoms_frac = None
 
-    HH_R = fourier_transform_k_to_r(HH_k, kpoints, irvec)
+    HH_R = fourier_transform_k_to_r(HH_k, kpoints, irvec, atoms_frac)
 
     return HH_R
 
 
 # ==================================================
 def get_AA_R(cwi):
     """
     matrix elements of real-space position operator, <0n|r|Rm>.
 
     Args:
-        cwi (SystemInfo): CWInfo.
+        cwi (CWInfo): CWInfo.
 
     Returns:
         ndarray: position operator, AA_R(3, len(irvec), num_wann, num_wann).
     """
     Mkb = np.array(cwi["Mkb"])
     Uk = np.array(cwi["Uk"])
 
@@ -111,21 +111,21 @@
     # Use Eq.(31) of Marzari&Vanderbilt PRB 56, 12847 (1997) for band-diagonal position matrix.
     if cwi["transl_inv"]:
         AA_k_diag = -1 * np.einsum("kb,kba,kbnn->akn", wk, bveck, np.imag(np.log(Mkb_w)), optimize=True)
         np.einsum("aknn->akn", AA_k)[:] = AA_k_diag
 
     AA_k = 0.5 * (AA_k + np.einsum("akmn->aknm", AA_k).conj())
 
-    # if cwi["tb_gauge"]:
-    #     atoms_list = list(cwi["atoms_frac"].values())
-    #     atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
-    # else:
-    #     atoms_frac = None
+    if cwi["tb_gauge"]:
+        atoms_list = list(cwi["atoms_frac"].values())
+        atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
+    else:
+        atoms_frac = None
 
-    AA_R = np.array([fourier_transform_k_to_r(AA_k[i], kpoints, irvec) for i in range(3)])
+    AA_R = np.array([fourier_transform_k_to_r(AA_k[i], kpoints, irvec, atoms_frac) for i in range(3)])
 
     return AA_R
 
 
 # ==================================================
 def get_BB_R():
     """<0|H(r-R)|R>"""
@@ -140,23 +140,24 @@
 
 # ==================================================
 def get_SS_R(cwi):
     """
     matrix elements of real-space spin operator, <0n|sigma_x,y,z|Rm>.
 
     Args:
-        cwi (SystemInfo): CWInfo.
+        cwi (CWInfo): CWInfo.
 
     Returns:
         ndarray: spin operator, SS_R(3, len(irvec), num_wann, num_wann).
     """
-    Sk = np.array(cwi["Sk"])
+    pauli_spn = np.array(cwi["pauli_spn"])
     Uk = np.array(cwi["Uk"])
 
-    SS_k = Uk.transpose(0, 2, 1).conjugate() @ Sk @ Uk
+    SS_k = Uk.transpose(0, 2, 1).conjugate() @ pauli_spn @ Uk
+
     SS_k = 0.5 * (SS_k + np.einsum("akmn->aknm", SS_k).conj())
 
     kpoints = np.array(cwi["kpoints"])
     irvec = np.array(cwi["irvec"])
 
     if cwi["tb_gauge"]:
         atoms_list = list(cwi["atoms_frac"].values())
@@ -206,15 +207,15 @@
 
 # ==================================================
 def get_berry_phase_R(cwi):
     """
     matrix elements of real-space spin operator, <0n|A_x,y,z|Rm>.
 
     Args:
-        cwi (SystemInfo): CWInfo.
+        cwi (CWInfo): CWInfo.
 
     Returns:
         ndarray: spin operator, SS_R(3, len(irvec), num_wann, num_wann).
     """
     Mkb = np.array(cwi["Mkb"])
     Uk = np.array(cwi["Uk"])
     num_wann = cwi["num_wann"]
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/util/header.py` & `symclosestwannier-1.2.1/symclosestwannier/util/header.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,30 +14,36 @@
     "smearing_temp_min": "smearing temperature for lower window (float), [0.01].",
     "delta": "small constant to avoid ill-conditioning of overlap matrices (float), [1e-12].",
     "svd": "implement singular value decomposition ? otherwise adopt Lowdin's orthogonalization method (bool), [False].",
     "verbose": "verbose calculation info (bool, optional), [False].",
     "parallel": "use parallel code? (bool), [False].",
     "formatter": "format by using black? (bool), [False].",
     "transl_inv": "use Eq.(31) of Marzari&Vanderbilt PRB 56, 12847 (1997) for band-diagonal position matrix elements? (bool), [True].",
-    "tb_gauge"          : "use tb gauge? (bool), [False].",
+    "use_degen_pert": "use degenerate perturbation theory when bands are degenerate and band derivatives are needed? (bool), [False].",
+    "degen_thr": "threshold to exclude degenerate bands from the calculation, [0.0].",
+    "tb_gauge": "use tb gauge? (bool), [False].",
     "write_hr": "write seedname_hr.dat ? (bool), [False].",
     "write_sr": "write seedname_sr.dat ? (bool), [False].",
     "write_u_matrices": "write seedname_u.dat and seedname_u_dis.dat ? (bool), [False].",
     "write_rmn": "write seedname_r.dat ? (bool), [False].",
     "write_vmn": "write seedname_v.dat ? (bool), [False].",
     "write_tb": "write seedname_tb.dat ? (bool), [False].",
     "write_spn": "write seedname.spn.cw ? (bool), [False].",
     "symmetrization": "symmetrize ? (bool), [False].",
     "mp_outdir": "output files for multipie are found in this directory (str). ['./'].",
     "mp_seedname": "seedname for seedname_model.py, seedname_samb.py and seedname_matrix.py files (str), ['default'].",
-    "ket_amn": "ket basis list in the seedname.amn file. The format of each ket must be same as the 'ket' in sambname_model.py file. See sambname['info']['ket'] in sambname_model.py file for the format (list), [None].",
-    "irreps": "list of irreps to be considered (str/list), [None].",
+    "ket_amn": "ket basis list in the seedname.amn file. If ket_amn == auto, the list of orbitals are set automatically, or it can be set manually. The format of each ket must be same as the 'ket' in sambname_model.py file. See sambname['info']['ket'] in sambname_model.py file for the format (list), [None].",
     "a": "lattice parameter (in Ang) used to correct units of k points in reference band data (float, optional), [1.0].",
     "N1": "number of divisions for high symmetry lines (int, optional), [50].",
-    "fermi_energy": "fermi energy used for band shift (float, optional), [0.0].",
+    "fermi_energy": "fermi energy (float, optional), [0.0].",
+    "zeeman_interaction": "consider zeeman interaction ? (bool), [False].",
+    "magnetic_field": "strength of the magnetic field (float), [0.0].",
+    "magnetic_field_theta": "angle from the z-axis of the magnetic field (float), [0.0].",
+    "magnetic_field_phi": "angle from the x-axis of the magnetic field (float), [0.0].",
+    "g_factor": "spin g factor (float), [2.0].",
 }
 
 win_info = {
     "seedname": "seedname (str), [cwannier].",
     "num_k": "# of k points (int), [1].",
     "num_bands": "# of bands passed to the code (int), [1].",
     "num_wann": "# of WFs (int), [1].",
@@ -53,28 +59,34 @@
     "mp_grid": "dimensions of the Monkhorst-Pack grid of k-points (list), [[0, 0, 0]].",
     "kpoints": "k-points, [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].",
     "kpoint": "representative k points (dict), [None].",
     "kpoint_path": "k-points along high symmetry line in Brillouin zonen, [[k1, k2, k3]] (crystal coordinate) (str), [None].",
     "unit_cell_cart": "transform matrix, [a1,a2,a3], [None].",
     "atoms_frac": "atomic positions in fractional coordinates with respect to the lattice vectors, {atom: [r1,r2,r3]} [None].",
     "atoms_cart": "atomic positions in cartesian coordinates, {atom: [rx,ry,rz]} [None].",
+    "spinors": "WFs are spinors? (bool) [False].",
+    "spin_moment": "Determines whether to evaluate the spin moment (bool), [False].",
     #
     "kmesh": "dimensions of the Monkhorst-Pack grid of k-points for response calculation (list), [[1, 1, 1]].",
     "kmesh_spacing": "minimum distance for neighboring k points along each of the three directions in k space (list), [1,1,1]].",
     "adpt_smr": "Determines whether to use an adaptive scheme for broadening the DOS and similar quantities defined on the energy axis (bool), [True].",
     "adpt_smr_fac": "The width ηnk of the broadened delta function used to determine the contribution to the spectral property (DOS, ...) from band n at point k (float), [sqrt(2)].",
     "adpt_smr_max": "Maximum allowed value for the adaptive energy smearing [eV] (float), [1.0].",
     "smr_type": "Defines the analytical form used for the broadened delta function in the computation of the DOS and similar quantities defined on the energy axis, gauss/m-pN/m-v or cold/f-d (str), [gauss].",
     "smr_fixed_en_width": "Energy width for the smearing function for the DOS. Used only if adpt_smr is false (The units are [eV]) (flaot), [0.0].",
     "spin_decomp": "If true, extra columns are added to some output files (such as seedname-dos.dat for the dos module, and analogously for the berry and BoltzWann modules) (bool), [False].",
     # berry
     "berry": "Determines whether to enter the berry routines (bool), [False].",
     "berry_task": "The quantity to compute when berry=true, ahc/morb/kubo/sc/shc/kdotp/me (str).",
     "berry_kmesh": "Overrides the kmesh global variable.",
     "berry_kmesh_spacing": "Overrides the kmesh_spacing global variable.",
+    # berry curvature, ahc, shc
+    "berry_curv_unit": " Unit of Berry curvature, ang2/bohr2, ['ang2']",
+    "berry_curv_adpt_kmesh": "Linear dimension of the adaptively refined k-mesh used to compute the anomalous/spin Hall conductivity, [1]",
+    "berry_curv_adpt_kmesh_thresh": "Threshold magnitude of the Berry curvature for adaptive refinement, [100]",
     # kubo
     "kubo_freq_max": "Upper limit of the frequency range for computing the optical conductivity, JDOS and ac SHC. (The units are [eV]) (float), [If an inner energy window was specified, the default value is dis_froz_max-fermi_energy+0.6667. Otherwise it is the difference between the maximum and the minimum energy eigenvalue stored in seedname.eig, plus 0.6667.].",
     "kubo_freq_min": "Lower limit of the frequency range for computing the optical conductivity, JDOS and ac SHC. (The units are [eV]) (float), [0.0].",
     "kubo_freq_step": "Difference between consecutive values of the optical frequency between kubo_freq_min and kubo_freq_max. (The units are [eV]) (float), [0.01].",
     "kubo_eigval_max": "Maximum energy eigenvalue of the eigenstates to be included in the evaluation of the optical conductivity, JDOS and ac SHC. (The units are [eV]) (float), [If an inner energy window was specified, the default value is the upper bound of the inner energy window plus 0.6667. Otherwise it is the maximum energy eigenvalue stored in seedname.eig plus 0.6667.].",
     "kubo_adpt_smr": "Overrides the adpt_smr global variable.",
     "kubo_adpt_smr_fac": "Overrides the adpt_smr_fac global variable.",
@@ -97,14 +109,15 @@
     "kpoints": "k-points, [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].",
     "kpoints_wo_shift": "k-points without shift, [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].",
     "nnkpts": "nearest-neighbour k-points (list), [None].",
     "nw2n": "atom position index of each WFs (list), [None].",
     "nw2l": "l specifies the angular part Θlm(θ, φ) (list), [None].",
     "nw2m": "m specifies the angular part Θlm(θ, φ) (list), [None].",
     "nw2r": "r specifies the radial part Rr(r) (list), [None].",
+    "nw2s": "s specifies the spin, 1(up)/-1(dn) (list), [None].",
     "atom_orb": "WFs indexes of each atom (list), [None].",
     "atom_pos": "atom position index of each atom (list), [None].",
     "atom_pos_r": "atom position of each atom in fractional coordinates with respect to the lattice vectors (list), [None].",
     "bvec_cart": "b-vectors (cartesian coordinate) (list), [None].",
     "bvec_crys": "b-vectors (crystal coordinate) (list), [None].",
     "wb": " weight for each k-points and nearest-neighbour k-points (list), [None].",
 }
@@ -212,16 +225,14 @@
     "Sk_sym": "Symmetrized overlap matrix elements in k-space (ndarray).",
     "Hk_sym": "Symmetrized Hamiltonian matrix elements in k-space (orthogonal) (ndarray).",
     "Hk_nonortho_sym": "Symmetrized Hamiltonian matrix elements in k-space (non-orthogonal) (ndarray).",
     "Sr_sym": "Symmetrized overlap matrix elements in real-space (ndarray).",
     "Hr_sym": "Symmetrized Hamiltonian matrix elements in real-space (orthogonal) (ndarray).",
     "Hr_nonortho_sym": "Symmetrized Hamiltonian matrix elements in real-space (non-orthogonal) (ndarray).",
     #
-    "rpoints_mp": "lattice points data included in matrix_dict, [[r1, r2, r3]] (crystal coordinate) (ndarray).",
-    #
     "Ek_RMSE_grid": "mean squared error of eigen energies between symmetrized and non-symmetrized closed wannier TB model (grid) (float).",
     "Ek_RMSE_path": "mean squared error of eigen energies between symmetrized and non-symmetrized closed wannier TB model (path) (float).",
     #
     "matrix_dict": "dictionary form of the real-space representation of symmetry-adapted multipole basis (SAMB) (dict).",
 }
 
 cw_data_header = """
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier/util/message.py` & `symclosestwannier-1.2.1/symclosestwannier/util/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
              |         Phys. Rev. B 107, 195118 (2023)           |
              |                                                   |
              |                                                   |
              | Copyright (c) 2023-                               |
              |     The SymClosestWwannier Developer Group and    |
              |        individual contributors                    |
              |                                                   |
-             |       Release: 1.1.9       22th January 2024      |
+             |       Release: 1.1.19       22th January 2024      |
              |                                                   |
              | This program is free software; you can            |
              | redistribute it and/or modify it under the terms  |
              | of the GNU General Public License as published by |
              | the Free Software Foundation; either version 2 of |
              | the License, or (at your option) any later version|
              |                                                   |
@@ -255,14 +255,40 @@
 *----------------------------------------------------------------------------*
 
 """
 
     return msg
 
 
+# ==================================================
+def cw_start_expectation_msg():
+    msg = """
+
+*----------------------------------------------------------------------------*
+                                cw_expectation
+*----------------------------------------------------------------------------*
+
+"""
+
+    return msg
+
+
+# ==================================================
+def cw_end_expectation_msg():
+    msg = """
+
+*----------------------------------------------------------------------------*
+                            cw_expectation: All done
+*----------------------------------------------------------------------------*
+
+"""
+
+    return msg
+
+
 # ==================================================
 def cw_start_band_msg():
     msg = """
 
 *----------------------------------------------------------------------------*
                                    cw_band
 *----------------------------------------------------------------------------*
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier.egg-info/PKG-INFO` & `symclosestwannier-1.2.1/symclosestwannier.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,64 @@
 Metadata-Version: 2.1
 Name: symclosestwannier
-Version: 1.1.9
+Version: 1.2.1
 Summary: A Python library for Symmetry-Adapted Closest Wannier (SymCW) Tight-Binding model based on Plane-Wave DFT calculation.
-Home-page: https://github.com/CMT-MU/SymClosestWannier
-Author: Rikuto Oiwa
-Author-email: ro.qp.07@gmail.com
-License: MIT
+Author-email: Rikuto Oiwa <ro.qp.07@gmail.com>
+License: GPL
+Project-URL: Homepage, https://github.com/CMT-MU/SymClosestWannier
+Project-URL: Issues, https://github.com/CMT-MU/SymClosestWannier/issues
 Keywords: dft,wannier function,tight-binding model,symmetry,materials science
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gcoreutils
 Requires-Dist: multipie
 Requires-Dist: xmltodict
 Requires-Dist: fortio
 Requires-Dist: h5py
 Provides-Extra: dev
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: sphinx-rtd-theme; extra == "dev"
-Requires-Dist: ipython; extra == "dev"
+Requires-Dist: jupyter-book; extra == "dev"
+Requires-Dist: ghp-import; extra == "dev"
+Requires-Dist: jupytext; extra == "dev"
+Requires-Dist: multipie; extra == "dev"
+Requires-Dist: qtdraw; extra == "dev"
+
+# [SymClosestWannier](https://cmt-mu.github.io/SymClosestWannier/)
+
+- **Overview**:
+    A Python library to create Symmetry-adapted Closest Wannier (SymCW) tight-binding models based on the Symmetry-Adapted Multipole Basis (SAMB) [1] and the Closest Wannier formalism developed by Taisuke Ozaki [2].
+
+    > [1] Hiroaki Kusunose, Rikuto Oiwa, and Satoru Hayami, Symmetry-adapted modeling for molecules and crystals, Phys. Rev. B 107, 195118 (2023).
+    > DOI: https://doi.org/10.1103/PhysRevB.107.195118.<br>
+    > [2] Taisuke Ozaki, Closest Wannier functions to a given set of localized orbitals, arXiv:2306.15296, (2023).
+    > URL: https://arxiv.org/abs/2306.15296v2.
+
+- **Authors**: Rikuto Oiwa
+
+- **Installation**: SymClosestWannier can be installed from PyPI using pip on Python >= 3.9:
+    ```
+    pip install symclosestwannier
+    ```
+    You can also visit [PyPI](https://pypi.org/project/symclosestwannier/) or [GitHub](https://github.com/CMT-MU/SymClosestWannier/) to download the source.
+
+- **Citing SymClosestWannier**: If you are using SymClosestWannier in your scientific research, please help our scientific visibility by citing our work:
+
+    > Rikuto Oiwa, Akane Inda, Satoru Hayami, Takuya Nomoto, Ryotaro Arita, and Hiroaki Kusunose, in preparation.<br>
+    > DOI: []()
+
+- **Requirements**:
+  - Symmetry-Adapted Multipole Basis (SAMB) for molecular or crystal are optionally generated by [MultiPie](https://github.com/CMT-MU/MultiPie).
+  - MultiPie library optionally requires [TeXLive](https://www.tug.org/texlive/) environment to create LaTeX and PDF files.
+  - Molecular or crystal structure files are optionally generated by [QtDraw](https://github.com/CMT-MU/QtDraw).
 
-# SymClosestWannier
-
-A Python library to create Symmetry-adapted Closest Wannier (SymCW) tight-binding models based on the Symmetry-Adapted Multipole Basis (SAMB) [1] and the Closest Wannier formalism developed by Taisuke Ozaki [2].
-
-
-[1] Hiroaki Kusunose, Rikuto Oiwa, and Satoru Hayami, Symmetry-adapted modeling for molecules and crystals, Phys. Rev. B 107, 195118 (2023).
-
-DOI: https://doi.org/10.1103/PhysRevB.107.195118.
-
-[2] Taisuke Ozaki, Closest Wannier functions to a given set of localized orbitals, arXiv:2306.15296, (2023).
-
-URL: https://arxiv.org/abs/2306.15296v2.
-
-
-## Installation
-
-SymClosestWannier can be installed from PyPI using pip on Python >= 3.9:
-```
-pip install symclosestwannier
-```
-You can also visit [PyPI](https://pypi.org/project/symclosestwannier/) or [GitHub](https://github.com/CMT-MU/SymClosestWannier/) to download the source.
-
-
-## Authors
-
-Rikuto Oiwa
-
-
-## Citing SymClosestWannier
-
-If you are using SymClosestWannier in your scientific research, please help our scientific visibility by citing our work:
-
-> Rikuto Oiwa, Akane Inda, Satoru Hayami, Takuya Nomoto, Ryotaro Arita, and Hiroaki Kusunose, in preparation.
->
-> DOI: []()
-
-
-
-## Requirements
-- Symmetry-Adapted Multipole Basis (SAMB) for molecular or crystal are optionally generated by [MultiPie](https://github.com/CMT-MU/MultiPie).
-- MultiPie library optionally requires [TeXLive](https://www.tug.org/texlive/) environment to create LaTeX and PDF files.
-- Molecular or crystal structure files are optionally generated by [QtDraw](https://github.com/CMT-MU/QtDraw).
-
-
-## Documentation
-
-Refer to the [documentation](https://cmt-mu.github.io/SymClosestWannier/) for detailed installation and usage.
-
-
-## To Do
-
-- add function fo automatically set ket_amn.
-- add function to read seedname.uHu, seedname.uIu files.
+- **To Do**:
+  - add function to read seedname.uHu, seedname.uIu files.
```

### Comparing `symclosestwannier-1.1.9/symclosestwannier.egg-info/SOURCES.txt` & `symclosestwannier-1.2.1/symclosestwannier.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 MANIFEST.in
-README.md
-setup.cfg
+pyproject.toml
 setup.py
+docs/README.md
 symclosestwannier/__init__.py
 symclosestwannier.egg-info/PKG-INFO
 symclosestwannier.egg-info/SOURCES.txt
 symclosestwannier.egg-info/dependency_links.txt
 symclosestwannier.egg-info/entry_points.txt
 symclosestwannier.egg-info/requires.txt
 symclosestwannier.egg-info/top_level.txt
```

