# Comparing `tmp/scalex-1.0.3.tar.gz` & `tmp/scalex-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalex-1.0.3.tar", last modified: Tue Apr 16 23:10:20 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `scalex-1.0.3.tar` & `scalex-1.0.4.tar`

### file list

```diff
@@ -1,82 +1,65 @@
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.738808 scalex-1.0.3/
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)      121 2024-04-16 21:24:31.000000 scalex-1.0.3/.gitignore
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1073 2024-04-16 21:24:31.000000 scalex-1.0.3/LICENSE.txt
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     7320 2024-04-16 23:10:20.736808 scalex-1.0.3/PKG-INFO
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     6217 2024-04-16 22:10:50.000000 scalex-1.0.3/README.md
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     3779 2024-04-16 22:01:37.000000 scalex-1.0.3/SCALEX.py
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.505806 scalex-1.0.3/docs/
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)      638 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/Makefile
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)      799 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/make.bat
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.518806 scalex-1.0.3/docs/source/
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.520806 scalex-1.0.3/docs/source/_static/
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     6148 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/.DS_Store
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.554807 scalex-1.0.3/docs/source/_static/img/
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     6148 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/.DS_Store
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)    63250 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/cross-modality_integration.png
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     2994 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/logo_white.png
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)   264528 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/mouse_atlas_reference.png
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)   249863 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/pancreas_projection.png
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)    49732 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/pbmc_before_integration.png
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)    80122 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/pbmc_integration.png
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)    60360 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/query_kidney.png
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)    54065 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/query_tabula_muris_aging.png
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)   103354 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/scATAC_integration.png
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)   379113 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/_static/img/scalex.jpg
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.560807 scalex-1.0.3/docs/source/api/
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1889 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/api/index.rst
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     3190 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/conf.py
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)      192 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/contributors.rst
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1236 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/index.rst
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1054 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/installation.rst
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)      267 2024-04-16 22:11:29.000000 scalex-1.0.3/docs/source/news.rst
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.565807 scalex-1.0.3/docs/source/release/
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)      167 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/release/1.0.0.rst
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)       66 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/release/index.rst
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.599807 scalex-1.0.3/docs/source/tutorial/
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)   170454 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/tutorial/Integration_PBMC.ipynb
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)   435407 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/tutorial/Integration_cross-modality.ipynb
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)   358829 2024-04-16 21:24:31.000000 scalex-1.0.3/docs/source/tutorial/Integration_scATAC-seq.ipynb
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)  1415270 2024-04-16 21:24:32.000000 scalex-1.0.3/docs/source/tutorial/Projection_pancreas.ipynb
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1856 2024-04-16 21:24:32.000000 scalex-1.0.3/docs/source/tutorial/index.rst
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     3712 2024-04-16 21:24:32.000000 scalex-1.0.3/docs/source/usage.rst
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.615807 scalex-1.0.3/experiments/
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     3342 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/LISI.ipynb
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)   245692 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/NMI-ARI.ipynb
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)    47829 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/Silhouette_score & batch_entropy_mixing_score.ipynb
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     9228 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/dirichlet_regression.ipynb
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)    30433 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/overcorrection_score.ipynb
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)  1084713 2024-04-16 21:24:32.000000 scalex-1.0.3/experiments/projection.ipynb
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)      188 2024-04-16 22:25:18.000000 scalex-1.0.3/requirements.txt
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.688808 scalex-1.0.3/scalex/
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)      220 2024-04-16 22:35:39.000000 scalex-1.0.3/scalex/__init__.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)    21827 2024-04-16 22:27:20.000000 scalex-1.0.3/scalex/data.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)    10508 2024-04-16 23:05:40.000000 scalex-1.0.3/scalex/function.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)      839 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/logger.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2789 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/metrics.py
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.709808 scalex-1.0.3/scalex/net/
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/net/__init__.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     5616 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/net/layer.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)      514 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/net/loss.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2324 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/net/utils.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     7093 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/net/vae.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)    11068 2024-04-16 21:24:32.000000 scalex-1.0.3/scalex/plot.py
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.734808 scalex-1.0.3/scalex.egg-info/
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     7320 2024-04-16 23:10:19.000000 scalex-1.0.3/scalex.egg-info/PKG-INFO
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)     1913 2024-04-16 23:10:19.000000 scalex-1.0.3/scalex.egg-info/SOURCES.txt
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)        1 2024-04-16 23:10:19.000000 scalex-1.0.3/scalex.egg-info/dependency_links.txt
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)      188 2024-04-16 23:10:19.000000 scalex-1.0.3/scalex.egg-info/requires.txt
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)        7 2024-04-16 23:10:19.000000 scalex-1.0.3/scalex.egg-info/top_level.txt
--rw-r--r--   0 leixiong  (1316) kundaje  (65541)       38 2024-04-16 23:10:20.738808 scalex-1.0.3/setup.cfg
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     1782 2024-04-16 21:24:32.000000 scalex-1.0.3/setup.py
-drwxr-xr-x   0 leixiong  (1316) kundaje  (65541)        0 2024-04-16 23:10:20.732808 scalex-1.0.3/third_parties/
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2062 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/BBKNN.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     3033 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/Conos.R
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2654 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/DESC.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2546 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/FastMNN.R
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2704 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/Harmony.R
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2792 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/LIGER.R
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2023 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/Raw.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2253 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/Scanorama.py
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     3786 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/Seurat_v3.R
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2915 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/online_iNMF.R
--rwxr-xr-x   0 leixiong  (1316) kundaje  (65541)     2738 2024-04-16 21:24:32.000000 scalex-1.0.3/third_parties/scVI.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 scalex-1.0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 scalex-1.0.4/CHANGELOG.md
+-rwxr-xr-x   0        0        0     3779 2020-02-02 00:00:00.000000 scalex-1.0.4/SCALEX.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 scalex-1.0.4/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/make.bat
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/conf.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/contributors.rst
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/index.rst
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/installation.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/news.rst
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/usage.rst
+-rw-r--r--   0        0        0    63250 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/_static/img/cross-modality_integration.png
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/_static/img/logo_white.png
+-rw-r--r--   0        0        0   264528 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/_static/img/mouse_atlas_reference.png
+-rw-r--r--   0        0        0   249863 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/_static/img/pancreas_projection.png
+-rw-r--r--   0        0        0    49732 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/_static/img/pbmc_before_integration.png
+-rw-r--r--   0        0        0    80122 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/_static/img/pbmc_integration.png
+-rw-r--r--   0        0        0    60360 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/_static/img/query_kidney.png
+-rw-r--r--   0        0        0    54065 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/_static/img/query_tabula_muris_aging.png
+-rw-r--r--   0        0        0   103354 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/_static/img/scATAC_integration.png
+-rw-r--r--   0        0        0   379113 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/_static/img/scalex.jpg
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/api/index.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/release/1.0.0.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/release/index.rst
+-rw-r--r--   0        0        0   170454 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/tutorial/Integration_PBMC.ipynb
+-rw-r--r--   0        0        0   435407 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/tutorial/Integration_cross-modality.ipynb
+-rw-r--r--   0        0        0   358829 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/tutorial/Integration_scATAC-seq.ipynb
+-rw-r--r--   0        0        0  1415270 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/tutorial/Projection_pancreas.ipynb
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 scalex-1.0.4/docs/source/tutorial/index.rst
+-rwxr-xr-x   0        0        0     3342 2020-02-02 00:00:00.000000 scalex-1.0.4/experiments/LISI.ipynb
+-rwxr-xr-x   0        0        0   245692 2020-02-02 00:00:00.000000 scalex-1.0.4/experiments/NMI-ARI.ipynb
+-rwxr-xr-x   0        0        0    47829 2020-02-02 00:00:00.000000 scalex-1.0.4/experiments/Silhouette_score & batch_entropy_mixing_score.ipynb
+-rwxr-xr-x   0        0        0     9228 2020-02-02 00:00:00.000000 scalex-1.0.4/experiments/dirichlet_regression.ipynb
+-rwxr-xr-x   0        0        0    30433 2020-02-02 00:00:00.000000 scalex-1.0.4/experiments/overcorrection_score.ipynb
+-rwxr-xr-x   0        0        0  1084713 2020-02-02 00:00:00.000000 scalex-1.0.4/experiments/projection.ipynb
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 scalex-1.0.4/scalex/__init__.py
+-rwxr-xr-x   0        0        0    23005 2020-02-02 00:00:00.000000 scalex-1.0.4/scalex/data.py
+-rwxr-xr-x   0        0        0    14478 2020-02-02 00:00:00.000000 scalex-1.0.4/scalex/function.py
+-rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 scalex-1.0.4/scalex/logger.py
+-rwxr-xr-x   0        0        0     2789 2020-02-02 00:00:00.000000 scalex-1.0.4/scalex/metrics.py
+-rwxr-xr-x   0        0        0    11160 2020-02-02 00:00:00.000000 scalex-1.0.4/scalex/plot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scalex-1.0.4/scalex/net/__init__.py
+-rwxr-xr-x   0        0        0     5616 2020-02-02 00:00:00.000000 scalex-1.0.4/scalex/net/layer.py
+-rwxr-xr-x   0        0        0      514 2020-02-02 00:00:00.000000 scalex-1.0.4/scalex/net/loss.py
+-rwxr-xr-x   0        0        0     2324 2020-02-02 00:00:00.000000 scalex-1.0.4/scalex/net/utils.py
+-rwxr-xr-x   0        0        0     7513 2020-02-02 00:00:00.000000 scalex-1.0.4/scalex/net/vae.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scalex-1.0.4/tests/conftest.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 scalex-1.0.4/tests/test_scalex.py
+-rwxr-xr-x   0        0        0     2062 2020-02-02 00:00:00.000000 scalex-1.0.4/third_parties/BBKNN.py
+-rwxr-xr-x   0        0        0     3033 2020-02-02 00:00:00.000000 scalex-1.0.4/third_parties/Conos.R
+-rwxr-xr-x   0        0        0     2654 2020-02-02 00:00:00.000000 scalex-1.0.4/third_parties/DESC.py
+-rwxr-xr-x   0        0        0     2546 2020-02-02 00:00:00.000000 scalex-1.0.4/third_parties/FastMNN.R
+-rwxr-xr-x   0        0        0     2704 2020-02-02 00:00:00.000000 scalex-1.0.4/third_parties/Harmony.R
+-rwxr-xr-x   0        0        0     2792 2020-02-02 00:00:00.000000 scalex-1.0.4/third_parties/LIGER.R
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 scalex-1.0.4/third_parties/Raw.py
+-rwxr-xr-x   0        0        0     2253 2020-02-02 00:00:00.000000 scalex-1.0.4/third_parties/Scanorama.py
+-rwxr-xr-x   0        0        0     3786 2020-02-02 00:00:00.000000 scalex-1.0.4/third_parties/Seurat_v3.R
+-rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 scalex-1.0.4/third_parties/online_iNMF.R
+-rwxr-xr-x   0        0        0     2738 2020-02-02 00:00:00.000000 scalex-1.0.4/third_parties/scVI.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 scalex-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 scalex-1.0.4/LICENSE
+-rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 scalex-1.0.4/README.md
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 scalex-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 scalex-1.0.4/PKG-INFO
```

### Comparing `scalex-1.0.3/PKG-INFO` & `scalex-1.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,62 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: scalex
-Version: 1.0.3
+Version: 1.0.4
 Summary: Online single-cell data integration through projecting heterogeneous datasets into a common cell-embedding space
-Home-page: https://github.com/jsxlei/scalex
 Author: Lei Xiong
-Author-email: jsxlei@gmail.com
 License: MIT
-Classifier: Development Status :: 4 - Beta
+License-File: LICENSE
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >3.6.0
-License-File: LICENSE.txt
+Requires-Python: >=3.7
+Requires-Dist: leidenalg>=0.8.3
+Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
-Requires-Dist: scipy>=1.13.0
+Requires-Dist: scanpy>=1.10.1
 Requires-Dist: scikit-learn>=1.4.2
+Requires-Dist: scipy>=1.13.0
+Requires-Dist: seaborn>=0.13.2
 Requires-Dist: torch>=2.2.2
-Requires-Dist: scanpy>=1.10.1
 Requires-Dist: tqdm>=4.66.2
-Requires-Dist: matplotlib>=3.8.4
-Requires-Dist: seaborn>=0.13.2
-Requires-Dist: leidenalg>=0.8.3
-Requires-Dist: sphinx_autodoc_typehints
-Requires-Dist: nbsphinx
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: twine>=4.0.2; extra == 'dev'
+Provides-Extra: doc
+Requires-Dist: docutils!=0.18.*,!=0.19.*,>=0.8; extra == 'doc'
+Requires-Dist: ipykernel; extra == 'doc'
+Requires-Dist: ipython; extra == 'doc'
+Requires-Dist: myst-nb; extra == 'doc'
+Requires-Dist: nbsphinx; extra == 'doc'
+Requires-Dist: pandas; extra == 'doc'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'doc'
+Requires-Dist: sphinx-book-theme>=1.0.0; extra == 'doc'
+Requires-Dist: sphinx-copybutton; extra == 'doc'
+Requires-Dist: sphinx>=4; extra == 'doc'
+Requires-Dist: sphinxcontrib-bibtex>=1.0.0; extra == 'doc'
+Requires-Dist: sphinxext-opengraph; extra == 'doc'
+Provides-Extra: test
+Requires-Dist: coverage; extra == 'test'
+Requires-Dist: pytest>=6.0; extra == 'test'
+Description-Content-Type: text/markdown
 
 [![Stars](https://img.shields.io/github/stars/jsxlei/scalex?logo=GitHub&color=yellow)](https://github.com/jsxlei/scalex/stargazers)
 [![PyPI](https://img.shields.io/pypi/v/scalex.svg)](https://pypi.org/project/scalex)
 [![Documentation Status](https://readthedocs.org/projects/scalex/badge/?version=latest)](https://scalex.readthedocs.io/en/latest/?badge=stable)
 [![Downloads](https://pepy.tech/badge/scalex)](https://pepy.tech/project/scalex)
 [![DOI](https://zenodo.org/badge/345941713.svg)](https://zenodo.org/badge/latestdoi/345941713)
 # [Online single-cell data integration through projecting heterogeneous datasets into a common cell-embedding space](https://www.nature.com/articles/s41467-022-33758-z)
 
 ![](docs/source/_static/img/scalex.jpg)
 
+
 ## News
 #### [2022-10-17] SCALEX is online at [Nature Communications](https://www.nature.com/articles/s41467-022-33758-z)
 
 ## [Documentation](https://scalex.readthedocs.io/en/latest/index.html) 
 ## [Tutorial](https://scalex.readthedocs.io/en/latest/tutorial/index.html) 
 ## Installation  	
 #### install from PyPI
@@ -58,17 +73,18 @@
     git clone git://github.com/jsxlei/scalex.git
     cd scalex
     python setup.py install
     
 SCALEX is implemented in [Pytorch](https://pytorch.org/) framework.  
 SCALEX can be run on CPU devices, and running SCALEX on GPU devices if available is recommended.   
 
-## Quick Start
+## Getting started
 
-SCALEX can both used under command line and API function in jupyter notebook
+SCALEX can both used under command line and API function in jupyter notebook   
+Please refer to the [Documentation](https://readthedocs.org/projects/scalex/badge/?version=latest) and [Tutorial](https://scalex.readthedocs.io/en/latest/tutorial/index.html)
 
 
 ### 1. API function
 
     from scalex import SCALEX
     adata = SCALEX(data_list, batch_categories)
     
@@ -83,15 +99,15 @@
 
 `batch_categories` is optional, name of each batch, will be range from 0 to N-1 if not provided
 
 ### 2. Command line
 #### Standard usage
 
 
-    SCALEX.py --data_list data1 data2 dataN --batch_categories batch_name1 batch_name2 batch_nameN 
+    SCALEX --data_list data1 data2 dataN --batch_categories batch_name1 batch_name2 batch_nameN 
     
     
 `--data_list`: data path of each batch of single-cell dataset, use `-d` for short
 
 `--batch_categories`: name of each batch, batch_categories will range from 0 to N-1 if not specified
 
     
@@ -101,38 +117,37 @@
 * **[adata.h5ad](https://anndata.readthedocs.io/en/stable/anndata.AnnData.html#anndata.AnnData)**:  preprocessed data and results including, latent, clustering and imputation
 * **umap.png**:  UMAP visualization of latent representations of cells 
 * **log.txt**:  log file of training process
 
 ### Other Common Usage
 #### Use h5ad file storing `anndata` as input, one or multiple separated files
 
-    SCALEX.py --data_list <filename.h5ad>
+    SCALEX --data_list <filename.h5ad>
 
 #### Specify batch in `anadata.obs` using `--batch_name` if only one concatenated h5ad file provided, batch_name can be e.g. conditions, samples, assays or patients, default is `batch`
 
-    SCALEX.py --data_list <filename.h5ad> --batch_name <specific_batch_name>
+    SCALEX --data_list <filename.h5ad> --batch_name <specific_batch_name>
     
     
 #### Integrate heterogenous scATAC-seq datasets, add option `--profile` ATAC
         
-    SCALEX.py --data_list <filename.h5ad> --profile ATAC
+    SCALEX --data_list <filename.h5ad> --profile ATAC
     
 #### Inputation simultaneously along with Integration, add option `--impute`, results are stored at anndata.layers['impute']
 
-    SCALEX.py --data_list <atac_filename.h5ad> --profile ATAC --impute True
+    SCALEX --data_list <atac_filename.h5ad> --profile ATAC --impute True
     
     
 #### Custom features through `--n_top_features` a filename contains features in one column format read
 
-    SCALEX.py --data_list <filename.h5ad> --n_top_features features.txt
-    
+    SCALEX --data_list <filename.h5ad> --n_top_features features.txt
     
 #### Use preprocessed data `--processed`
 
-    SCALEX.py --data_list <filename.h5ad> --processed
+    SCALEX --data_list <filename.h5ad> --processed
 
 #### Option
 
 * --**data_list**  
         A list of matrices file (each as a `batch`) or a single batch/batch-merged file.
 * --**batch_categories**  
         Categories for the batch annotation. By default, use increasing numbers if not given
@@ -178,12 +193,17 @@
     
 #### Help
 Look for more usage of SCALEX
 
 	SCALEX.py --help 
     
     
+## Release notes
 
-    
-    
+See the [changelog](https://github.com/jsxlei/SCALEX/CHANGELOG.md).  
+
+
+## Citation
 
+Xiong, L., Tian, K., Li, Y., Ning, W., Gao, X., & Zhang, Q. C. (2022). Online single-cell data integration through projecting heterogeneous datasets into a common cell-embedding space. Nature Communications, 13(1), 6118. https://doi.org/10.1038/s41467-022-33758-z
 
+
```

### Comparing `scalex-1.0.3/README.md` & `scalex-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![Documentation Status](https://readthedocs.org/projects/scalex/badge/?version=latest)](https://scalex.readthedocs.io/en/latest/?badge=stable)
 [![Downloads](https://pepy.tech/badge/scalex)](https://pepy.tech/project/scalex)
 [![DOI](https://zenodo.org/badge/345941713.svg)](https://zenodo.org/badge/latestdoi/345941713)
 # [Online single-cell data integration through projecting heterogeneous datasets into a common cell-embedding space](https://www.nature.com/articles/s41467-022-33758-z)
 
 ![](docs/source/_static/img/scalex.jpg)
 
+
 ## News
 #### [2022-10-17] SCALEX is online at [Nature Communications](https://www.nature.com/articles/s41467-022-33758-z)
 
 ## [Documentation](https://scalex.readthedocs.io/en/latest/index.html) 
 ## [Tutorial](https://scalex.readthedocs.io/en/latest/tutorial/index.html) 
 ## Installation  	
 #### install from PyPI
@@ -27,17 +28,18 @@
     git clone git://github.com/jsxlei/scalex.git
     cd scalex
     python setup.py install
     
 SCALEX is implemented in [Pytorch](https://pytorch.org/) framework.  
 SCALEX can be run on CPU devices, and running SCALEX on GPU devices if available is recommended.   
 
-## Quick Start
+## Getting started
 
-SCALEX can both used under command line and API function in jupyter notebook
+SCALEX can both used under command line and API function in jupyter notebook   
+Please refer to the [Documentation](https://readthedocs.org/projects/scalex/badge/?version=latest) and [Tutorial](https://scalex.readthedocs.io/en/latest/tutorial/index.html)
 
 
 ### 1. API function
 
     from scalex import SCALEX
     adata = SCALEX(data_list, batch_categories)
     
@@ -52,15 +54,15 @@
 
 `batch_categories` is optional, name of each batch, will be range from 0 to N-1 if not provided
 
 ### 2. Command line
 #### Standard usage
 
 
-    SCALEX.py --data_list data1 data2 dataN --batch_categories batch_name1 batch_name2 batch_nameN 
+    SCALEX --data_list data1 data2 dataN --batch_categories batch_name1 batch_name2 batch_nameN 
     
     
 `--data_list`: data path of each batch of single-cell dataset, use `-d` for short
 
 `--batch_categories`: name of each batch, batch_categories will range from 0 to N-1 if not specified
 
     
@@ -70,38 +72,37 @@
 * **[adata.h5ad](https://anndata.readthedocs.io/en/stable/anndata.AnnData.html#anndata.AnnData)**:  preprocessed data and results including, latent, clustering and imputation
 * **umap.png**:  UMAP visualization of latent representations of cells 
 * **log.txt**:  log file of training process
 
 ### Other Common Usage
 #### Use h5ad file storing `anndata` as input, one or multiple separated files
 
-    SCALEX.py --data_list <filename.h5ad>
+    SCALEX --data_list <filename.h5ad>
 
 #### Specify batch in `anadata.obs` using `--batch_name` if only one concatenated h5ad file provided, batch_name can be e.g. conditions, samples, assays or patients, default is `batch`
 
-    SCALEX.py --data_list <filename.h5ad> --batch_name <specific_batch_name>
+    SCALEX --data_list <filename.h5ad> --batch_name <specific_batch_name>
     
     
 #### Integrate heterogenous scATAC-seq datasets, add option `--profile` ATAC
         
-    SCALEX.py --data_list <filename.h5ad> --profile ATAC
+    SCALEX --data_list <filename.h5ad> --profile ATAC
     
 #### Inputation simultaneously along with Integration, add option `--impute`, results are stored at anndata.layers['impute']
 
-    SCALEX.py --data_list <atac_filename.h5ad> --profile ATAC --impute True
+    SCALEX --data_list <atac_filename.h5ad> --profile ATAC --impute True
     
     
 #### Custom features through `--n_top_features` a filename contains features in one column format read
 
-    SCALEX.py --data_list <filename.h5ad> --n_top_features features.txt
-    
+    SCALEX --data_list <filename.h5ad> --n_top_features features.txt
     
 #### Use preprocessed data `--processed`
 
-    SCALEX.py --data_list <filename.h5ad> --processed
+    SCALEX --data_list <filename.h5ad> --processed
 
 #### Option
 
 * --**data_list**  
         A list of matrices file (each as a `batch`) or a single batch/batch-merged file.
 * --**batch_categories**  
         Categories for the batch annotation. By default, use increasing numbers if not given
@@ -147,12 +148,17 @@
     
 #### Help
 Look for more usage of SCALEX
 
 	SCALEX.py --help 
     
     
+## Release notes
 
-    
-    
+See the [changelog](https://github.com/jsxlei/SCALEX/CHANGELOG.md).  
+
+
+## Citation
 
+Xiong, L., Tian, K., Li, Y., Ning, W., Gao, X., & Zhang, Q. C. (2022). Online single-cell data integration through projecting heterogeneous datasets into a common cell-embedding space. Nature Communications, 13(1), 6118. https://doi.org/10.1038/s41467-022-33758-z
 
+
```

### Comparing `scalex-1.0.3/SCALEX.py` & `scalex-1.0.4/SCALEX.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/Makefile` & `scalex-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/make.bat` & `scalex-1.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/_static/img/cross-modality_integration.png` & `scalex-1.0.4/docs/source/_static/img/cross-modality_integration.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/_static/img/logo_white.png` & `scalex-1.0.4/docs/source/_static/img/logo_white.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/_static/img/mouse_atlas_reference.png` & `scalex-1.0.4/docs/source/_static/img/mouse_atlas_reference.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/_static/img/pancreas_projection.png` & `scalex-1.0.4/docs/source/_static/img/pancreas_projection.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/_static/img/pbmc_before_integration.png` & `scalex-1.0.4/docs/source/_static/img/pbmc_before_integration.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/_static/img/pbmc_integration.png` & `scalex-1.0.4/docs/source/_static/img/pbmc_integration.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/_static/img/query_kidney.png` & `scalex-1.0.4/docs/source/_static/img/query_kidney.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/_static/img/query_tabula_muris_aging.png` & `scalex-1.0.4/docs/source/_static/img/query_tabula_muris_aging.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/_static/img/scATAC_integration.png` & `scalex-1.0.4/docs/source/_static/img/scATAC_integration.png`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/_static/img/scalex.jpg` & `scalex-1.0.4/docs/source/_static/img/scalex.jpg`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/api/index.rst` & `scalex-1.0.4/docs/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/conf.py` & `scalex-1.0.4/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = 'sphinx_book_theme'
 
 html_theme_options = dict(navigation_depth=4, logo_only=True)  # Only show the logo
 html_context = dict(
     display_github=True,  # Integrate GitHub
     github_user='jsxlei',  # Username
     github_repo='SCALEX',  # Repo name
     github_version='main',  # Version
```

### Comparing `scalex-1.0.3/docs/source/index.rst` & `scalex-1.0.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/installation.rst` & `scalex-1.0.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/tutorial/Integration_PBMC.ipynb` & `scalex-1.0.4/docs/source/tutorial/Integration_PBMC.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/tutorial/Integration_cross-modality.ipynb` & `scalex-1.0.4/docs/source/tutorial/Integration_cross-modality.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/tutorial/Integration_scATAC-seq.ipynb` & `scalex-1.0.4/docs/source/tutorial/Integration_scATAC-seq.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/tutorial/Projection_pancreas.ipynb` & `scalex-1.0.4/docs/source/tutorial/Projection_pancreas.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/tutorial/index.rst` & `scalex-1.0.4/docs/source/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/docs/source/usage.rst` & `scalex-1.0.4/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/experiments/LISI.ipynb` & `scalex-1.0.4/experiments/LISI.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/experiments/NMI-ARI.ipynb` & `scalex-1.0.4/experiments/NMI-ARI.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/experiments/Silhouette_score & batch_entropy_mixing_score.ipynb` & `scalex-1.0.4/experiments/Silhouette_score & batch_entropy_mixing_score.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/experiments/dirichlet_regression.ipynb` & `scalex-1.0.4/experiments/dirichlet_regression.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/experiments/overcorrection_score.ipynb` & `scalex-1.0.4/experiments/overcorrection_score.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/experiments/projection.ipynb` & `scalex-1.0.4/experiments/projection.ipynb`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/scalex/data.py` & `scalex-1.0.4/scalex/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,14 +224,16 @@
     Return
     -------
     The AnnData object after preprocessing.
     """
     if min_features is None: min_features = 600
     if n_top_features is None: n_top_features = 2000
     if target_sum is None: target_sum = 10000
+
+    # adata.layers['count'] = adata.X.copy()
     
     if log: log.info('Preprocessing')
     # if not issparse(adata.X):
     if type(adata.X) != csr.csr_matrix and (not backed) and (not adata.isbacked):
         adata.X = scipy.sparse.csr_matrix(adata.X)
     
     if not keep_mt:
@@ -247,15 +249,16 @@
 
     if log: log.info('Normalizing total per cell')
     sc.pp.normalize_total(adata, target_sum=target_sum)
     
     if log: log.info('Log1p transforming')
     sc.pp.log1p(adata)
     
-    adata.raw = adata
+    adata.raw = adata # keep the normalized and log1p transformed data as raw gene expression for differential expression analysis
+
     if log: log.info('Finding variable features')
     if type(n_top_features) == int and n_top_features>0:
         sc.pp.highly_variable_genes(adata, n_top_genes=n_top_features, batch_key='batch') #, inplace=False, subset=True)
         adata = adata[:, adata.var.highly_variable].copy()
     elif type(n_top_features) != int:
         adata = reindex(adata, n_top_features)
         
@@ -635,15 +638,17 @@
             n_top_features=n_top_features,
             keep_mt=keep_mt,
             chunk_size=chunk_size,
             backed=backed,
             log=log,
         )
     else:
-        if use_layer in adata.layers:
+        if use_layer == 'X':
+            adata.X = MaxAbsScaler().fit_transform(adata.X)
+        elif use_layer in adata.layers:
             adata.layers[use_layer] = MaxAbsScaler().fit_transform(adata.layers[use_layer])
         elif use_layer in adata.obsm:
             adata.obsm[use_layer] = MaxAbsScaler().fit_transform(adata.obsm[use_layer])
         else:
             raise ValueError("Not support use_layer: `{}` yet".format(use_layer))
     scdata = SingleCellDataset(adata, use_layer=use_layer) # Wrap AnnData into Pytorch Dataset
     trainloader = DataLoader(
@@ -656,7 +661,31 @@
 
     batch_sampler = BatchSampler(batch_size, adata.obs['batch'], drop_last=False)
     testloader = DataLoader(scdata, batch_sampler=batch_sampler, num_workers=num_workers)
     
     return adata, trainloader, testloader 
 
 
+
+
+def download_file(url, local_filename):
+    """
+    Downloads a file from a given URL and saves it to a local path using wget.
+
+    Args:
+    url (str): URL to the file.
+    local_filename (str): Local path where the file should be saved.
+
+    # URL of the file you want to download
+    url = "https://www.dropbox.com/scl/fi/dnwpv29kcfl449a8aikqi/pancreas.h5ad?dl=0"  # Changed dl=0 to dl=1 for direct download
+    # Local path to save the file, change '~/.scalex/pancreas.h5ad' to an absolute path if necessary
+    local_path = os.path.expanduser('~/.scalex/pancreas.h5ad')
+    """
+    # Ensure the directory exists
+    os.makedirs(os.path.dirname(local_filename), exist_ok=True)
+
+    # Use wget to download the file
+    try:
+        wget.download(url, local_filename)
+        print(f"File downloaded successfully: {local_filename}")
+    except Exception as e:
+        print(f"An error occurred while downloading the file: {e}")
```

### Comparing `scalex-1.0.3/scalex/logger.py` & `scalex-1.0.4/scalex/logger.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/scalex/metrics.py` & `scalex-1.0.4/scalex/metrics.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/scalex/net/layer.py` & `scalex-1.0.4/scalex/net/layer.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/scalex/net/loss.py` & `scalex-1.0.4/scalex/net/loss.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/scalex/net/utils.py` & `scalex-1.0.4/scalex/net/utils.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/scalex/net/vae.py` & `scalex-1.0.4/scalex/net/vae.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,28 @@
         """
         pretrained_dict = torch.load(path, map_location=lambda storage, loc: storage)                            
         model_dict = self.state_dict()
         pretrained_dict = {k: v for k, v in pretrained_dict.items() if k in model_dict}
         model_dict.update(pretrained_dict) 
         self.load_state_dict(model_dict)
         
+
+    def forward(self, x, y):
+        x, y = x.float(), y.long()
+
+        # loss
+        z, mu, var = self.encoder(x)
+        recon_x = self.decoder(z, y)
+        recon_loss = F.binary_cross_entropy(recon_x, x) * x.size(-1)  ## TO DO
+        kl_loss = kl_div(mu, var) 
+
+        # acc.append(pearson_corr_coef(recon_x, x))
+        loss = {'recon_loss':recon_loss, 'kl_loss':0.5*kl_loss} 
+        return z, recon_x, loss
+
     def encodeBatch(
             self, 
             dataloader, 
             device='cuda', 
             out='latent', 
             batch_id=None,
             return_idx=False,
```

### Comparing `scalex-1.0.3/scalex/plot.py` & `scalex-1.0.4/scalex/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,43 +54,46 @@
         embeddings used to visualize, default is X_umap for UMAP
     size
         dot size on the embedding
     """
     
     if groups is None:
         groups = adata.obs[groupby].cat.categories
-    for b in groups:
+
+    # Create subplots
+    num_plots = len(groups)
+    fig, axes = plt.subplots(num_plots, 1, figsize=(5, 5 * num_plots), squeeze=False)
+
+    for ax, b in zip(axes.flatten(), groups):
         adata.obs['tmp'] = adata.obs[color].astype(str)
-        adata.obs['tmp'][adata.obs[groupby]!=b] = ''
+        adata.obs.loc[adata.obs[groupby]!=b, 'tmp'] = ''
         if cond2 is not None:
-            adata.obs['tmp'][adata.obs[cond2]!=v2] = ''
+            adata.obs.loc[adata.obs[cond2]!=v2, 'tmp'] = ''
             groups = list(adata[(adata.obs[groupby]==b) & 
                                 (adata.obs[cond2]==v2)].obs[color].astype('category').cat.categories.values)
             size = min(size, 120000/len(adata[(adata.obs[groupby]==b) & (adata.obs[cond2]==v2)]))
         else:
             groups = list(adata[adata.obs[groupby]==b].obs[color].astype('category').cat.categories.values)
             size = min(size, 120000/len(adata[adata.obs[groupby]==b]))
         adata.obs['tmp'] = adata.obs['tmp'].astype('category')
         if color_map is not None:
             palette = [color_map[i] if i in color_map else 'gray' for i in adata.obs['tmp'].cat.categories]
         else:
             palette = None
 
         title = b if cond2 is None else v2+sep+b
-        if save is not None:
-            save_ = '_'+b+save
-            show = False
-        else:
-            save_ = None
-            show = True
-        sc.pl.embedding(adata, color='tmp', basis=basis, groups=groups, title=title, palette=palette, size=size, save=save_,
-                   legend_loc=legend_loc, legend_fontsize=legend_fontsize, legend_fontweight=legend_fontweight, show=show)
+
+        ax = sc.pl.embedding(adata, color='tmp', basis=basis, groups=groups, ax=ax, title=title, palette=palette, size=size, 
+                   legend_loc=legend_loc, legend_fontsize=legend_fontsize, legend_fontweight=legend_fontweight, wspace=0.25, show=False)
+
+
         del adata.obs['tmp']
         del adata.uns['tmp_colors']
-        
+    if save:
+        plt.savefig(save, bbox_inches='tight')
 
 def plot_meta(
         adata, 
         use_rep=None, 
         color='celltype', 
         batch='batch', 
         colors=None,
```

### Comparing `scalex-1.0.3/third_parties/BBKNN.py` & `scalex-1.0.4/third_parties/BBKNN.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/third_parties/Conos.R` & `scalex-1.0.4/third_parties/Conos.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/third_parties/DESC.py` & `scalex-1.0.4/third_parties/DESC.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/third_parties/FastMNN.R` & `scalex-1.0.4/third_parties/FastMNN.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/third_parties/Harmony.R` & `scalex-1.0.4/third_parties/Harmony.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/third_parties/LIGER.R` & `scalex-1.0.4/third_parties/LIGER.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/third_parties/Raw.py` & `scalex-1.0.4/third_parties/Raw.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/third_parties/Scanorama.py` & `scalex-1.0.4/third_parties/Scanorama.py`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/third_parties/Seurat_v3.R` & `scalex-1.0.4/third_parties/Seurat_v3.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/third_parties/online_iNMF.R` & `scalex-1.0.4/third_parties/online_iNMF.R`

 * *Files identical despite different names*

### Comparing `scalex-1.0.3/third_parties/scVI.py` & `scalex-1.0.4/third_parties/scVI.py`

 * *Files identical despite different names*

