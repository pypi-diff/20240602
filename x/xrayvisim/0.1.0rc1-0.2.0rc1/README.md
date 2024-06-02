# Comparing `tmp/xrayvisim-0.1.0rc1.tar.gz` & `tmp/xrayvisim-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrayvisim-0.1.0rc1.tar", last modified: Mon Jun 27 21:14:52 2022, max compression
+gzip compressed data, was "xrayvisim-0.2.0rc1.tar", last modified: Sun Jun  2 14:03:50 2024, max compression
```

## Comparing `xrayvisim-0.1.0rc1.tar` & `xrayvisim-0.2.0rc1.tar`

### file list

```diff
@@ -1,69 +1,227 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.733642 xrayvisim-0.1.0rc1/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.729642 xrayvisim-0.1.0rc1/.circleci/
--rw-r--r--   0 vsts      (1001) docker     (121)     1991 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/.circleci/config.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      235 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/.circleci/early_exit.sh
--rw-r--r--   0 vsts      (1001) docker     (121)     2262 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (121)     1821 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 vsts      (1001) docker     (121)      540 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/.readthedocs.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      131 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/CHANGELOG.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1471 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/LICENSE.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      362 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     2967 2022-06-27 21:14:52.733642 xrayvisim-0.1.0rc1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     2005 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/README.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1841 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/azure-pipelines.yml
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.729642 xrayvisim-0.1.0rc1/changelog/
--rw-r--r--   0 vsts      (1001) docker     (121)     1886 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/changelog/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.729642 xrayvisim-0.1.0rc1/docs/
--rw-r--r--   0 vsts      (1001) docker     (121)     4581 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/docs/Makefile
--rw-r--r--   0 vsts      (1001) docker     (121)      171 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/docs/api.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     3660 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/docs/conf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      165 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     5457 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/docs/introduction.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     4513 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/docs/make.bat
--rw-r--r--   0 vsts      (1001) docker     (121)     4777 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/docs/tutorial.rst
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.729642 xrayvisim-0.1.0rc1/docs/whatsnew/
--rw-r--r--   0 vsts      (1001) docker     (121)      171 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/docs/whatsnew/changelog.rst
--rw-r--r--   0 vsts      (1001) docker     (121)       92 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/docs/whatsnew/index.rst
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.729642 xrayvisim-0.1.0rc1/examples/
--rw-r--r--   0 vsts      (1001) docker     (121)       46 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/examples/README.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.729642 xrayvisim-0.1.0rc1/hooks/
--rwxr-xr-x   0 vsts      (1001) docker     (121)      259 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/hooks/pre-commit
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.733642 xrayvisim-0.1.0rc1/licenses/
--rw-r--r--   0 vsts      (1001) docker     (121)     1488 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/licenses/LICENSE.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      162 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/licenses/README.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1659 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/licenses/TEMPLATE_LICENSE.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     2113 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)     2718 2022-06-27 21:14:52.737642 xrayvisim-0.1.0rc1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1770 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/setup.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1908 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/tox.ini
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.733642 xrayvisim-0.1.0rc1/xrayvisim.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     2967 2022-06-27 21:14:52.000000 xrayvisim-0.1.0rc1/xrayvisim.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1393 2022-06-27 21:14:52.000000 xrayvisim-0.1.0rc1/xrayvisim.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-27 21:14:52.000000 xrayvisim-0.1.0rc1/xrayvisim.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-27 21:14:52.000000 xrayvisim-0.1.0rc1/xrayvisim.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)      387 2022-06-27 21:14:52.000000 xrayvisim-0.1.0rc1/xrayvisim.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-06-27 21:14:52.000000 xrayvisim-0.1.0rc1/xrayvisim.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.733642 xrayvisim-0.1.0rc1/xrayvision/
--rw-r--r--   0 vsts      (1001) docker     (121)      344 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19588 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/clean.py
--rw-r--r--   0 vsts      (1001) docker     (121)      137 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.733642 xrayvisim-0.1.0rc1/xrayvision/data/
--rw-r--r--   0 vsts      (1001) docker     (121)      256 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/data/README.rst
--rw-r--r--   0 vsts      (1001) docker     (121)   103680 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/data/hsi_20020220_110600_1time_1energy.fits
--rw-r--r--   0 vsts      (1001) docker     (121)   227520 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/data/hsi_20020220_110600_1time_4energies.fits
--rw-r--r--   0 vsts      (1001) docker     (121)   434880 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/data/hsi_20020220_110600_9times_1energy.fits
--rw-r--r--   0 vsts      (1001) docker     (121)   161280 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/data/hsi_visibili_20131028_0156_20131028_0200_6_12.fits
--rw-r--r--   0 vsts      (1001) docker     (121)    28800 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/data/sample_rhessi_visibilities.fits
--rw-r--r--   0 vsts      (1001) docker     (121)    10702 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/imaging.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18783 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/mem.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-27 21:14:52.733642 xrayvisim-0.1.0rc1/xrayvision/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)      121 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4048 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/tests/test_clean.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8835 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/tests/test_imaging.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3300 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/tests/test_mem.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11269 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/tests/test_transform.py
--rw-r--r--   0 vsts      (1001) docker     (121)      144 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/tests/test_visibility.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8701 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/transform.py
--rw-r--r--   0 vsts      (1001) docker     (121)      726 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/utils.py
--rw-r--r--   0 vsts      (1001) docker     (121)      348 2022-06-27 21:14:51.000000 xrayvisim-0.1.0rc1/xrayvision/version.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2469 2022-06-27 21:14:24.000000 xrayvisim-0.1.0rc1/xrayvision/visibility.py
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.809003 xrayvisim-0.2.0rc1/
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.770296 xrayvisim-0.2.0rc1/.circleci/
+-rw-r--r--   0 sm         (502) staff       (20)     1991 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/.circleci/config.yml
+-rw-r--r--   0 sm         (502) staff       (20)      235 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/.circleci/early_exit.sh
+-rw-r--r--   0 sm         (502) staff       (20)      246 2024-04-16 20:09:39.000000 xrayvisim-0.2.0rc1/.editorconfig
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.765749 xrayvisim-0.2.0rc1/.github/
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.770440 xrayvisim-0.2.0rc1/.github/workflows/
+-rw-r--r--   0 sm         (502) staff       (20)     1245 2024-04-08 15:50:34.000000 xrayvisim-0.2.0rc1/.github/workflows/ci.yml
+-rw-r--r--   0 sm         (502) staff       (20)     2309 2024-05-17 17:01:43.000000 xrayvisim-0.2.0rc1/.gitignore
+-rw-r--r--   0 sm         (502) staff       (20)     1363 2024-06-02 12:23:46.000000 xrayvisim-0.2.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 sm         (502) staff       (20)      571 2024-05-17 17:01:43.000000 xrayvisim-0.2.0rc1/.readthedocs.yml
+-rw-r--r--   0 sm         (502) staff       (20)      131 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/CHANGELOG.rst
+-rw-r--r--   0 sm         (502) staff       (20)     1471 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/LICENSE.rst
+-rw-r--r--   0 sm         (502) staff       (20)      362 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/MANIFEST.in
+-rw-r--r--   0 sm         (502) staff       (20)     4498 2024-06-02 14:03:50.808937 xrayvisim-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 sm         (502) staff       (20)     1884 2024-06-02 14:02:14.000000 xrayvisim-0.2.0rc1/README.rst
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.773931 xrayvisim-0.2.0rc1/changelog/
+-rw-r--r--   0 sm         (502) staff       (20)       49 2024-05-08 15:31:17.000000 xrayvisim-0.2.0rc1/changelog/53.doc.rst
+-rw-r--r--   0 sm         (502) staff       (20)       38 2024-05-08 15:31:17.000000 xrayvisim-0.2.0rc1/changelog/53.trivial.rst
+-rw-r--r--   0 sm         (502) staff       (20)      250 2024-05-24 10:57:25.000000 xrayvisim-0.2.0rc1/changelog/55.feature.rst
+-rw-r--r--   0 sm         (502) staff       (20)      249 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/changelog/58.breaking.rst
+-rw-r--r--   0 sm         (502) staff       (20)      104 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/changelog/58.bugfix.rst
+-rw-r--r--   0 sm         (502) staff       (20)       84 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/changelog/58.docs.rst
+-rw-r--r--   0 sm         (502) staff       (20)       61 2024-05-17 17:00:29.000000 xrayvisim-0.2.0rc1/changelog/61.trivial.rst
+-rw-r--r--   0 sm         (502) staff       (20)      113 2024-05-24 14:03:14.000000 xrayvisim-0.2.0rc1/changelog/63.bugfix.rst
+-rw-r--r--   0 sm         (502) staff       (20)      101 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/changelog/64.feature.rst
+-rw-r--r--   0 sm         (502) staff       (20)      141 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/changelog/65.feature.rst
+-rw-r--r--   0 sm         (502) staff       (20)       86 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/changelog/66.bugfix.rst
+-rw-r--r--   0 sm         (502) staff       (20)       80 2024-06-02 14:02:14.000000 xrayvisim-0.2.0rc1/changelog/67.breaking.rst
+-rw-r--r--   0 sm         (502) staff       (20)       62 2024-06-02 14:02:14.000000 xrayvisim-0.2.0rc1/changelog/70.trivial.rst
+-rw-r--r--   0 sm         (502) staff       (20)     1886 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/changelog/README.rst
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.775122 xrayvisim-0.2.0rc1/docs/
+-rw-r--r--   0 sm         (502) staff       (20)     6148 2024-05-10 07:23:15.000000 xrayvisim-0.2.0rc1/docs/.DS_Store
+-rw-r--r--   0 sm         (502) staff       (20)     4581 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/docs/Makefile
+-rw-r--r--   0 sm         (502) staff       (20)     4551 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/docs/conf.py
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.775419 xrayvisim-0.2.0rc1/docs/discussions/
+-rw-r--r--   0 sm         (502) staff       (20)       39 2024-04-16 12:10:12.000000 xrayvisim-0.2.0rc1/docs/discussions/index.rst
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.766348 xrayvisim-0.2.0rc1/docs/generated/
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.781586 xrayvisim-0.2.0rc1/docs/generated/api/
+-rw-r--r--   0 sm         (502) staff       (20)       74 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.clean.clean.rst
+-rw-r--r--   0 sm         (502) staff       (20)       83 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.clean.ms_clean.rst
+-rw-r--r--   0 sm         (502) staff       (20)       86 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.clean.vis_clean.rst
+-rw-r--r--   0 sm         (502) staff       (20)       95 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.clean.vis_ms_clean.rst
+-rw-r--r--   0 sm         (502) staff       (20)      106 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.imaging.generate_header.rst
+-rw-r--r--   0 sm         (502) staff       (20)       94 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.imaging.get_weights.rst
+-rw-r--r--   0 sm         (502) staff       (20)       97 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.imaging.image_to_vis.rst
+-rw-r--r--   0 sm         (502) staff       (20)       91 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.imaging.map_to_vis.rst
+-rw-r--r--   0 sm         (502) staff       (20)      136 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.imaging.validate_and_expand_kwarg.rst
+-rw-r--r--   0 sm         (502) staff       (20)      100 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.imaging.vis_psf_image.rst
+-rw-r--r--   0 sm         (502) staff       (20)       94 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.imaging.vis_psf_map.rst
+-rw-r--r--   0 sm         (502) staff       (20)       97 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.imaging.vis_to_image.rst
+-rw-r--r--   0 sm         (502) staff       (20)       91 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.imaging.vis_to_map.rst
+-rw-r--r--   0 sm         (502) staff       (20)       99 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.mem._estimate_flux.rst
+-rw-r--r--   0 sm         (502) staff       (20)       93 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.mem._get_entropy.rst
+-rw-r--r--   0 sm         (502) staff       (20)      114 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.mem._get_fourier_matrix.rst
+-rw-r--r--   0 sm         (502) staff       (20)      123 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.mem._get_mean_visibilities.rst
+-rw-r--r--   0 sm         (502) staff       (20)       93 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.mem._optimise_fb.rst
+-rw-r--r--   0 sm         (502) staff       (20)      108 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.mem._proximal_entropy.rst
+-rw-r--r--   0 sm         (502) staff       (20)      111 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.mem._proximal_operator.rst
+-rw-r--r--   0 sm         (502) staff       (20)       66 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.mem.mem.rst
+-rw-r--r--   0 sm         (502) staff       (20)       84 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.transform.dft_map.rst
+-rw-r--r--   0 sm         (502) staff       (20)       96 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.transform.generate_uv.rst
+-rw-r--r--   0 sm         (502) staff       (20)       96 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.transform.generate_xy.rst
+-rw-r--r--   0 sm         (502) staff       (20)       87 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.transform.idft_map.rst
+-rw-r--r--   0 sm         (502) staff       (20)       89 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.utils.get_logger.rst
+-rw-r--r--   0 sm         (502) staff       (20)      524 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.visibility.VisMeta.rst
+-rw-r--r--   0 sm         (502) staff       (20)      548 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.visibility.VisMetaABC.rst
+-rw-r--r--   0 sm         (502) staff       (20)      844 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.visibility.Visibilities.rst
+-rw-r--r--   0 sm         (502) staff       (20)      883 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.visibility.VisibilitiesABC.rst
+-rw-r--r--   0 sm         (502) staff       (20)      113 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/api/xrayvision.visibility.Visibility.rst
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.785207 xrayvisim-0.2.0rc1/docs/generated/gallery/
+-rw-r--r--   0 sm         (502) staff       (20)    11672 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/gallery_jupyter.zip
+-rw-r--r--   0 sm         (502) staff       (20)     6827 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/gallery_python.zip
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.788195 xrayvisim-0.2.0rc1/docs/generated/gallery/images/
+-rw-r--r--   0 sm         (502) staff       (20)    41159 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/images/sphx_glr_rhessi_001.png
+-rw-r--r--   0 sm         (502) staff       (20)   130231 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/images/sphx_glr_rhessi_002.png
+-rw-r--r--   0 sm         (502) staff       (20)    64809 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/images/sphx_glr_stix_001.png
+-rw-r--r--   0 sm         (502) staff       (20)    58251 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/images/sphx_glr_stix_002.png
+-rw-r--r--   0 sm         (502) staff       (20)    50449 2024-05-24 12:59:24.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/images/sphx_glr_stix_003.png
+-rw-r--r--   0 sm         (502) staff       (20)    43668 2024-05-24 12:59:28.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/images/sphx_glr_stix_004.png
+-rw-r--r--   0 sm         (502) staff       (20)   176816 2024-05-24 12:59:29.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/images/sphx_glr_stix_005.png
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.789393 xrayvisim-0.2.0rc1/docs/generated/gallery/images/thumb/
+-rw-r--r--   0 sm         (502) staff       (20)    26513 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/images/thumb/sphx_glr_rhessi_thumb.png
+-rw-r--r--   0 sm         (502) staff       (20)    52124 2024-05-24 12:59:29.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/images/thumb/sphx_glr_stix_thumb.png
+-rw-r--r--   0 sm         (502) staff       (20)     1497 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/index.rst
+-rw-r--r--   0 sm         (502) staff       (20)     7061 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/rhessi.ipynb
+-rw-r--r--   0 sm         (502) staff       (20)     4215 2024-05-24 12:59:29.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/rhessi.py
+-rw-r--r--   0 sm         (502) staff       (20)       32 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/rhessi.py.md5
+-rw-r--r--   0 sm         (502) staff       (20)    10164 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/rhessi.rst
+-rw-r--r--   0 sm         (502) staff       (20)     7791 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/rhessi_codeobj.pickle
+-rw-r--r--   0 sm         (502) staff       (20)     1208 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/sg_execution_times.rst
+-rw-r--r--   0 sm         (502) staff       (20)     4393 2024-05-24 12:59:29.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/stix.ipynb
+-rw-r--r--   0 sm         (502) staff       (20)     2406 2024-05-24 12:59:20.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/stix.py
+-rw-r--r--   0 sm         (502) staff       (20)       32 2024-05-24 12:59:29.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/stix.py.md5
+-rw-r--r--   0 sm         (502) staff       (20)     8849 2024-05-24 12:59:29.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/stix.rst
+-rw-r--r--   0 sm         (502) staff       (20)     6664 2024-05-24 12:59:29.000000 xrayvisim-0.2.0rc1/docs/generated/gallery/stix_codeobj.pickle
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.797249 xrayvisim-0.2.0rc1/docs/generated/modules/
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.clean.clean.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.clean.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.clean.ms_clean.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.clean.vis_clean.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.clean.vis_ms_clean.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.imaging.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.imaging.generate_header.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.imaging.get_weights.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.imaging.image_to_vis.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.imaging.map_to_vis.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.imaging.validate_and_expand_kwarg.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.imaging.vis_psf_image.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.imaging.vis_psf_map.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.imaging.vis_to_image.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.imaging.vis_to_map.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.mem._estimate_flux.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.mem._get_entropy.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.mem._get_fourier_matrix.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.mem._get_mean_visibilities.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.mem._optimise_fb.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.mem._proximal_entropy.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.mem._proximal_operator.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.mem.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.mem.mem.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.transform.dft_map.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.transform.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.transform.generate_uv.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.transform.generate_xy.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.transform.idft_map.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.utils.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.utils.get_logger.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMeta.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMeta.instrument.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMeta.observer_coordinate.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMeta.spectral_range.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMeta.time_range.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMeta.vis_labels.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMetaABC.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMetaABC.instrument.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMetaABC.observer_coordinate.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMetaABC.spectral_range.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMetaABC.time_range.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisMetaABC.vis_labels.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibilities.amplitude.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibilities.amplitude_uncertainty.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibilities.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibilities.meta.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibilities.phase.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibilities.phase_center.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibilities.phase_uncertainty.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibilities.u.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibilities.uncertainty.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibilities.v.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibilities.visibilities.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisibilitiesABC.amplitude.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisibilitiesABC.amplitude_uncertainty.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisibilitiesABC.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisibilitiesABC.meta.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisibilitiesABC.phase.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisibilitiesABC.phase_center.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisibilitiesABC.phase_uncertainty.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisibilitiesABC.u.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisibilitiesABC.uncertainty.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisibilitiesABC.v.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.VisibilitiesABC.visibilities.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.Visibility.examples
+-rw-r--r--   0 sm         (502) staff       (20)        0 2024-05-24 12:59:44.000000 xrayvisim-0.2.0rc1/docs/generated/modules/xrayvision.visibility.examples
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.797646 xrayvisim-0.2.0rc1/docs/how_to_guides/
+-rw-r--r--   0 sm         (502) staff       (20)     4909 2024-04-16 11:47:38.000000 xrayvisim-0.2.0rc1/docs/how_to_guides/dev_guide.rst
+-rw-r--r--   0 sm         (502) staff       (20)       88 2024-04-15 20:01:31.000000 xrayvisim-0.2.0rc1/docs/how_to_guides/index.rst
+-rw-r--r--   0 sm         (502) staff       (20)     3324 2024-05-17 17:01:43.000000 xrayvisim-0.2.0rc1/docs/index.rst
+-rw-r--r--   0 sm         (502) staff       (20)     4513 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/docs/make.bat
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.799418 xrayvisim-0.2.0rc1/docs/reference/
+-rw-r--r--   0 sm         (502) staff       (20)      157 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/docs/reference/clean.rst
+-rw-r--r--   0 sm         (502) staff       (20)      200 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/docs/reference/imaging.rst
+-rw-r--r--   0 sm         (502) staff       (20)      146 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/docs/reference/index.rst
+-rw-r--r--   0 sm         (502) staff       (20)      149 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/docs/reference/mem.rst
+-rw-r--r--   0 sm         (502) staff       (20)      185 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/docs/reference/transform.rst
+-rw-r--r--   0 sm         (502) staff       (20)      153 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/docs/reference/utils.rst
+-rw-r--r--   0 sm         (502) staff       (20)      197 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/docs/reference/visibility.rst
+-rw-r--r--   0 sm         (502) staff       (20)     1210 2024-05-24 12:59:43.000000 xrayvisim-0.2.0rc1/docs/sg_execution_times.rst
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.799811 xrayvisim-0.2.0rc1/docs/tutorials/
+-rw-r--r--   0 sm         (502) staff       (20)       52 2024-04-16 11:47:38.000000 xrayvisim-0.2.0rc1/docs/tutorials/index.rst
+-rw-r--r--   0 sm         (502) staff       (20)     5591 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/docs/tutorials/introduction.rst
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.800316 xrayvisim-0.2.0rc1/docs/whatsnew/
+-rw-r--r--   0 sm         (502) staff       (20)      171 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/docs/whatsnew/changelog.rst
+-rw-r--r--   0 sm         (502) staff       (20)       93 2024-05-17 17:01:43.000000 xrayvisim-0.2.0rc1/docs/whatsnew/index.rst
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.801249 xrayvisim-0.2.0rc1/examples/
+-rw-r--r--   0 sm         (502) staff       (20)       46 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/examples/README.txt
+-rw-r--r--   0 sm         (502) staff       (20)     4903 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/examples/rhessi.py
+-rw-r--r--   0 sm         (502) staff       (20)     2602 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/examples/stix.py
+-rw-r--r--   0 sm         (502) staff       (20)     4633 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/examples/stix_vis.pkl
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.801494 xrayvisim-0.2.0rc1/hooks/
+-rwxr-xr-x   0 sm         (502) staff       (20)      259 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/hooks/pre-commit
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.802114 xrayvisim-0.2.0rc1/licenses/
+-rw-r--r--   0 sm         (502) staff       (20)     1488 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/licenses/LICENSE.rst
+-rw-r--r--   0 sm         (502) staff       (20)      162 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/licenses/README.rst
+-rw-r--r--   0 sm         (502) staff       (20)     1659 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/licenses/TEMPLATE_LICENSE.rst
+-rw-r--r--   0 sm         (502) staff       (20)     2101 2024-05-17 17:01:43.000000 xrayvisim-0.2.0rc1/pyproject.toml
+-rw-r--r--   0 sm         (502) staff       (20)     1111 2024-04-16 11:11:28.000000 xrayvisim-0.2.0rc1/ruff.toml
+-rw-r--r--   0 sm         (502) staff       (20)     2981 2024-06-02 14:03:50.809481 xrayvisim-0.2.0rc1/setup.cfg
+-rwxr-xr-x   0 sm         (502) staff       (20)     1749 2024-05-17 17:01:43.000000 xrayvisim-0.2.0rc1/setup.py
+-rw-r--r--   0 sm         (502) staff       (20)     2012 2024-05-17 17:01:43.000000 xrayvisim-0.2.0rc1/tox.ini
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.806942 xrayvisim-0.2.0rc1/xrayvisim.egg-info/
+-rw-r--r--   0 sm         (502) staff       (20)     4498 2024-06-02 14:03:50.000000 xrayvisim-0.2.0rc1/xrayvisim.egg-info/PKG-INFO
+-rw-r--r--   0 sm         (502) staff       (20)     9176 2024-06-02 14:03:50.000000 xrayvisim-0.2.0rc1/xrayvisim.egg-info/SOURCES.txt
+-rw-r--r--   0 sm         (502) staff       (20)        1 2024-06-02 14:03:50.000000 xrayvisim-0.2.0rc1/xrayvisim.egg-info/dependency_links.txt
+-rw-r--r--   0 sm         (502) staff       (20)        1 2023-10-09 10:35:46.000000 xrayvisim-0.2.0rc1/xrayvisim.egg-info/not-zip-safe
+-rw-r--r--   0 sm         (502) staff       (20)      505 2024-06-02 14:03:50.000000 xrayvisim-0.2.0rc1/xrayvisim.egg-info/requires.txt
+-rw-r--r--   0 sm         (502) staff       (20)       11 2024-06-02 14:03:50.000000 xrayvisim-0.2.0rc1/xrayvisim.egg-info/top_level.txt
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.804734 xrayvisim-0.2.0rc1/xrayvision/
+-rw-r--r--   0 sm         (502) staff       (20)      205 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/xrayvision/__init__.py
+-rw-r--r--   0 sm         (502) staff       (20)    21611 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/xrayvision/clean.py
+-rw-r--r--   0 sm         (502) staff       (20)      143 2024-05-17 17:01:43.000000 xrayvisim-0.2.0rc1/xrayvision/conftest.py
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.805197 xrayvisim-0.2.0rc1/xrayvision/data/
+-rw-r--r--   0 sm         (502) staff       (20)      256 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/xrayvision/data/README.rst
+-rwxr-xr-x   0 sm         (502) staff       (20)    10977 2024-04-08 11:24:24.000000 xrayvisim-0.2.0rc1/xrayvision/data/stix_vis.pkl
+-rw-r--r--   0 sm         (502) staff       (20)    10829 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/xrayvision/imaging.py
+-rw-r--r--   0 sm         (502) staff       (20)    18863 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/xrayvision/mem.py
+drwxr-xr-x   0 sm         (502) staff       (20)        0 2024-06-02 14:03:50.806713 xrayvisim-0.2.0rc1/xrayvision/tests/
+-rw-r--r--   0 sm         (502) staff       (20)      121 2023-10-05 11:28:57.000000 xrayvisim-0.2.0rc1/xrayvision/tests/__init__.py
+-rw-r--r--   0 sm         (502) staff       (20)     5353 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/xrayvision/tests/test_clean.py
+-rw-r--r--   0 sm         (502) staff       (20)    11734 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/xrayvision/tests/test_imaging.py
+-rw-r--r--   0 sm         (502) staff       (20)     3154 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/xrayvision/tests/test_mem.py
+-rw-r--r--   0 sm         (502) staff       (20)    16291 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/xrayvision/tests/test_transform.py
+-rw-r--r--   0 sm         (502) staff       (20)     4409 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/xrayvision/tests/test_visibility.py
+-rw-r--r--   0 sm         (502) staff       (20)    10358 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/xrayvision/transform.py
+-rw-r--r--   0 sm         (502) staff       (20)      825 2024-06-01 10:48:47.000000 xrayvisim-0.2.0rc1/xrayvision/utils.py
+-rw-r--r--   0 sm         (502) staff       (20)      348 2024-06-02 14:03:50.000000 xrayvisim-0.2.0rc1/xrayvision/version.py
+-rw-r--r--   0 sm         (502) staff       (20)    19281 2024-06-02 12:04:08.000000 xrayvisim-0.2.0rc1/xrayvision/visibility.py
```

### Comparing `xrayvisim-0.1.0rc1/.circleci/config.yml` & `xrayvisim-0.2.0rc1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `xrayvisim-0.1.0rc1/.gitignore` & `xrayvisim-0.2.0rc1/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -145,7 +145,13 @@
 # Specifc Template
 docs/_build
 docs/generated
 docs/api
 docs/whatsnew/latest_changelog.txt
 xrayvision/version.py
 htmlcov/
+sg_execution_times.rst
+
+.DS_Store
+
+# IDE
+.idea
```

### Comparing `xrayvisim-0.1.0rc1/.pre-commit-config.yaml` & `xrayvisim-0.2.0rc1/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,45 @@
 repos:
-# The warnings/errors we check for here are:
-  # E901 - SyntaxError or IndentationError
-  # E902 - IOError
-  # F822 - undefined name in __all__
-  # F823 - local variable name referenced before assignment
-  # Others are taken care of by autopep8
-  - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    # This should be before any formatting hooks like isort
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.3.5"
     hooks:
-      - id: flake8
-        args:
-          [
-            "--count",
-            "--select",
-            "E901,E902,F822,F823",
-          ]
-        exclude: ".*(.fits|.fts|.fit|.txt|tca.*|extern.*|.rst|.md)$"
-
-  - repo: https://github.com/myint/autoflake
-    rev: v1.4
-    hooks:
-      - id: autoflake
-        args:
-          [
-            "--in-place",
-            "--remove-all-unused-imports",
-            "--remove-unused-variable",
-          ]
-        exclude: ".*(.fits|.fts|.fit|.txt|tca.*|extern.*|.rst|.md|__init__.py|docs/conf.py)$"
-
+      - id: ruff
+        args: ["--fix"]
+      # Run the formatter.
+      - id: ruff-format
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.13.2
     hooks:
       - id: isort
-        args: ["--sp", "setup.cfg"]
-        exclude: ".*(.fits|.fts|.fit|.txt|tca.*|extern.*|.rst|.md|cm/__init__.py|docs/conf.py)$"
-
-  - repo: https://github.com/pre-commit/mirrors-autopep8
-    rev: v1.6.0
-    hooks:
-    -   id: autopep8
-        args: ["--in-place","--max-line-length", "200"]
-        exclude: ".*(.fits|.fts|.fit|.txt|tca.*|extern.*|.rst|.md|cm/__init__.py)$"
-
+        exclude: ".*(.fits|.fts|.fit|.header|.txt|tca.*|extern.*)$"
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.5.0
     hooks:
       - id: check-ast
       - id: check-case-conflict
       - id: trailing-whitespace
-        exclude: ".*(.fits|.fts|.fit|.txt)$"
+        exclude: ".*(.fits|.fts|.fit|.header|.txt)$"
       - id: check-yaml
       - id: debug-statements
       - id: check-added-large-files
+        args: ["--enforce-all", "--maxkb=1054"]
       - id: end-of-file-fixer
-        exclude: ".*(.fits|.fts|.fit|.txt|tca.*)$"
+        exclude: ".*(.fits|.fts|.fit|.header|.txt|tca.*|.json)$|^CITATION.rst$"
       - id: mixed-line-ending
-        exclude: ".*(.fits|.fts|.fit|.txt|tca.*)$"
+        exclude: ".*(.fits|.fts|.fit|.header|.txt|tca.*)$"
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: "v1.10.0"
+    hooks:
+      - id: mypy
+        additional_dependencies: [ "types-setuptools" ]
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.6
+    hooks:
+      - id: codespell
+        additional_dependencies:
+          - tomli
+        args: ["--write-changes"]
+
 ci:
-    autofix_prs: false
+  autofix_prs: false
+  autoupdate_schedule: "quarterly"
```

### Comparing `xrayvisim-0.1.0rc1/.readthedocs.yml` & `xrayvisim-0.2.0rc1/.readthedocs.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # .readthedocs.yml
 # Read the Docs configuration file
 # See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
 
 # Required
 version: 2
 
+build:
+  os: ubuntu-22.04
+  tools:
+    python: "3.9"
+  apt_packages:
+    - graphviz
+
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
+  builder: html
   configuration: docs/conf.py
+  fail_on_warning: true
 
-# Optionally build your docs in additional formats such as PDF and ePub
+# Optionally, build your docs in additional formats such as PDF and ePub
 formats: []
 
-# Optionally set the version of Python and requirements required to build your docs
 python:
-  version: 3.7
-  install:
-    - method: pip
-      path: .
-      extra_requirements:
+   install:
+     - method: pip
+       path: .
+       extra_requirements:
         - docs
-        - all
+        - map
```

### Comparing `xrayvisim-0.1.0rc1/LICENSE.rst` & `xrayvisim-0.2.0rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `xrayvisim-0.1.0rc1/changelog/README.rst` & `xrayvisim-0.2.0rc1/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `xrayvisim-0.1.0rc1/docs/Makefile` & `xrayvisim-0.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xrayvisim-0.1.0rc1/docs/conf.py` & `xrayvisim-0.2.0rc1/docs/conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,133 @@
-# -*- coding: utf-8 -*-
 #
 # Configuration file for the Sphinx documentation builder.
 #
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
 
 # -- Project information -----------------------------------------------------
 
-project = 'xrayvision'
-copyright = '2020, '
-author = ''
+project = "xrayvision"
+copyright = "2020, "
+author = ""
+
+import pathlib
 
 # The full version, including alpha/beta/rc tags
 from xrayvision import __version__
+
 release = __version__
-is_development = '.dev' in __version__
+is_development = ".dev" in __version__
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'matplotlib.sphinxext.plot_directive',
-    'sphinx.ext.autodoc',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.todo',
-    'sphinx.ext.coverage',
-    'sphinx.ext.inheritance_diagram',
-    'sphinx.ext.viewcode',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.doctest',
-    'sphinx.ext.mathjax',
-    'sphinx_changelog',
-    'sphinx_automodapi.automodapi',
-    'sphinx_automodapi.smart_resolver',
+    "matplotlib.sphinxext.plot_directive",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.inheritance_diagram",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.todo",
+    "sphinx.ext.viewcode",
+    "sphinx_automodapi.automodapi",
+    "sphinx_automodapi.smart_resolver",
+    "sphinx_changelog",
+    "sphinx_design",
+    "sphinx_gallery.gen_gallery",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ['_templates']
 
+# Set automodapi to generate files inside the generated directory
+automodapi_toctreedirnm = "generated/api"
+
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents. Set to the "smart" one.
-default_role = 'obj'
+default_role = "obj"
 
 # Disable having a separate return type row
-napoleon_use_rtype = False
+napoleon_use_rtype = True
 
 # Disable google style docstrings
 napoleon_google_docstring = False
 
+# until sphinx-gallery / sphinx is fixed https://github.com/sphinx-doc/sphinx/issues/12300
+suppress_warnings = ["config.cache"]
+
+autodoc_typehints = "description"
+autoclass_content = "init"
+
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/3/',
-               (None, 'http://data.astropy.org/intersphinx/python3.inv')),
-    'numpy': ('https://docs.scipy.org/doc/numpy/',
-              (None, 'http://data.astropy.org/intersphinx/numpy.inv')),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference/',
-              (None, 'http://data.astropy.org/intersphinx/scipy.inv')),
-    'matplotlib': ('https://matplotlib.org/',
-                   (None, 'http://data.astropy.org/intersphinx/matplotlib.inv')),
-    'astropy': ('http://docs.astropy.org/en/stable/', None),
-    'sunpy': ('https://docs.sunpy.org/en/stable/', None)}
+    "python": ("https://docs.python.org/3/", (None, "http://data.astropy.org/intersphinx/python3.inv")),
+    "numpy": ("https://docs.scipy.org/doc/numpy/", (None, "http://data.astropy.org/intersphinx/numpy.inv")),
+    "scipy": ("https://docs.scipy.org/doc/scipy/reference/", (None, "http://data.astropy.org/intersphinx/scipy.inv")),
+    "matplotlib": ("https://matplotlib.org/", (None, "http://data.astropy.org/intersphinx/matplotlib.inv")),
+    "astropy": ("http://docs.astropy.org/en/stable/", None),
+    "sunpy": ("https://docs.sunpy.org/en/stable/", None),
+}
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
-try:
-    from sunpy_sphinx_theme.conf import *
-except ImportError:
-    html_theme = 'default'
+html_theme = "pydata_sphinx_theme"
 
+html_theme_options = {
+    "logo": {"text": "xrayision"},
+}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ['_static']
 
 # Render inheritance diagrams in SVG
 graphviz_output_format = "svg"
 
 graphviz_dot_args = [
-    '-Nfontsize=10',
-    '-Nfontname=Helvetica Neue, Helvetica, Arial, sans-serif',
-    '-Efontsize=10',
-    '-Efontname=Helvetica Neue, Helvetica, Arial, sans-serif',
-    '-Gfontsize=10',
-    '-Gfontname=Helvetica Neue, Helvetica, Arial, sans-serif'
+    "-Nfontsize=10",
+    "-Nfontname=Helvetica Neue, Helvetica, Arial, sans-serif",
+    "-Efontsize=10",
+    "-Efontname=Helvetica Neue, Helvetica, Arial, sans-serif",
+    "-Gfontsize=10",
+    "-Gfontname=Helvetica Neue, Helvetica, Arial, sans-serif",
 ]
+
+# -- Options for the Sphinx gallery -------------------------------------------
+path = pathlib.Path.cwd()
+example_dir = path.parent.joinpath("examples")
+sphinx_gallery_conf = {
+    "backreferences_dir": str(path.joinpath("generated", "modules")),
+    "filename_pattern": "^((?!skip_).)*$",
+    "examples_dirs": example_dir,
+    "gallery_dirs": path.joinpath("generated", "gallery"),
+    "default_thumb_file": path.joinpath("logo", "sunpy_icon_128x128.png"),
+    "abort_on_example_error": False,
+    "plot_gallery": "True",
+    "remove_config_comments": True,
+    "only_warn_on_example_error": True,
+}
```

### Comparing `xrayvisim-0.1.0rc1/docs/introduction.rst` & `xrayvisim-0.2.0rc1/docs/tutorials/introduction.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,27 @@
         if noisy:
             data = data + np.random.normal(loc=0.0, scale=0.005, size=(65, 65));
 
         return data
 
     data = make_data()
 
-    full_uv = transform.generate_uv(65)
+    full_uv = transform.generate_uv(65*u.pix)
 
-    uu = transform.generate_uv(33)
-    vv = transform.generate_uv(33)
+    uu = transform.generate_uv(33*u.pix)
+    vv = transform.generate_uv(33*u.pix)
 
     uu, vv = np.meshgrid(uu, vv)
 
     # uv coordinates require unit
     uv = np.array([uu, vv]).reshape(2, 33**2)/u.arcsec
 
     full_vis = transform.dft_map(data, u=uv[0,:], v=uv[1,:])
 
-    res = transform.idft_map(full_vis, u=uv[0,:], v=uv[1,:], shape=(33, 33))
+    res = transform.idft_map(full_vis, u=uv[0,:], v=uv[1,:], weights=1/33**2, shape=(33, 33)*u.pix)
     # assert np.allclose(data, res)
 
     # Generate log spaced radial u, v sampeling
     half_log_space = np.logspace(np.log10(np.abs(uv[uv != 0]).value.min()), np.log10(np.abs(uv.value.max())), 10)
 
     theta = np.linspace(0, 2*np.pi, 31)
     theta = theta[np.newaxis,:]
@@ -73,17 +73,18 @@
 
     sub_uv = np.vstack([x.flatten(), y.flatten()])
     sub_uv = np.hstack([sub_uv, np.zeros((2,1))])/u.arcsec
 
     sub_vis = transform.dft_map(data, u=sub_uv[0,:], v=sub_uv[1,:])
 
     psf1 = transform.idft_map(np.full(sub_vis.size, 1), u=sub_uv[0,:], v=sub_uv[1,:],
-                              shape=(65, 65))
+                              weights=1/sub_vis.size, shape=(65, 65)*u.pix)
 
-    sub_res = transform.idft_map(sub_vis, u=sub_uv[0,:], v=sub_uv[1,:], shape=(65, 65))
+    sub_res = transform.idft_map(sub_vis, u=sub_uv[0,:], v=sub_uv[1,:],
+                                 weights=1/sub_vis.size, shape=(65, 65)*u.pix)
 
     xp = np.round(x * 33 + 33/2 - 0.5 + 16).astype(int)
     yp = np.round(y * 33 + 33/2 - 0.5 + 16).astype(int)
 
     sv = np.zeros((65, 65))
     sv[:,:] = 0
     sv[xp.flatten(), yp.flatten()] = 1
```

### Comparing `xrayvisim-0.1.0rc1/docs/make.bat` & `xrayvisim-0.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xrayvisim-0.1.0rc1/licenses/LICENSE.rst` & `xrayvisim-0.2.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `xrayvisim-0.1.0rc1/licenses/TEMPLATE_LICENSE.rst` & `xrayvisim-0.2.0rc1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `xrayvisim-0.1.0rc1/pyproject.toml` & `xrayvisim-0.2.0rc1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -13,27 +13,27 @@
   [ tool.gilesbot.pull_requests ]
     enabled = true
 
   [ tool.gilesbot.towncrier_changelog ]
     enabled = true
     verify_pr_number = true
     changelog_skip_label = "No Changelog Entry Needed"
-    help_url = "https://github.com/samaloney/xrayvision/blob/main/changelog/README.rst"
+    help_url = "https://github.com/TCDSolar/xrayvision/blob/main/changelog/README.rst"
 
-    changelog_missing_long = "There isn't a changelog file in this pull request. Please add a changelog file to the `changelog/` directory following the instructions in the changelog [README](https://https://github.com/samaloney/xrayvision/blob/main/changelog/README.rst)."
+    changelog_missing_long = "There isn't a changelog file in this pull request. Please add a changelog file to the `changelog/` directory following the instructions in the changelog [README](https://github.com/TCDSolar/xrayvision/blob/main/changelog/README.rst)."
 
-    type_incorrect_long = "The changelog file you added is not one of the allowed types. Please use one of the types described in the changelog [README](https://github.com/samaloney/xrayvision/blob/main/changelog/README.rst)"
+    type_incorrect_long = "The changelog file you added is not one of the allowed types. Please use one of the types described in the changelog [README](https://github.com/TCDSolar/xrayvision/blob/main/changelog/README.rst)"
 
     number_incorrect_long = "The number in the changelog file you added does not match the number of this pull request. Please rename the file."
 
 [tool.towncrier]
     package = "xrayvision"
     filename = "CHANGELOG.rst"
     directory = "changelog/"
-    issue_format = "`#{issue} <https://github.com/samaloney/xrayvision/pull/{issue}>`__"
+    issue_format = "`#{issue} <https://github.com/TCDSolar/xrayvision/pull/{issue}>`__"
 
     [[tool.towncrier.type]]
         directory = "breaking"
         name = "Backwards Incompatible Changes"
         showcontent = true
 
     [[tool.towncrier.type]]
```

### Comparing `xrayvisim-0.1.0rc1/setup.cfg` & `xrayvisim-0.2.0rc1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,108 @@
 [metadata]
 name = xrayvisim
 author = Shane Maloney
 author_email = shane.maloney@dias.ie
 license = BSD 3-Clause
 license_files = LICENSE.rst
-url = 
-description = An open-source Python library for Fourier or synthesis imaging of X-Rays.
+url = https://github.com/TCDSolar/xrayvision
+description = An open-source Python library for Fourier or synthesis X-Ray imaging instruments.
 long_description = file: README.rst
+long_description_content_type = text/x-rst
+platform = any
+keywords = solar physics, solar, sun, x-rays
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 zip_safe = False
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.9
 include_package_data = True
 setup_requires = setuptools_scm
 install_requires = 
 	astropy>=3.4.1
 	numpy>=1.17.0
 	scipy>=1.3.0
+	xarray
 
 [options.extras_require]
 map = 
 	sunpy[map]>=3.1.0
 test = 
 	matplotlib
 	pytest
 	pytest-astropy
 	pytest-cov
 docs = 
+	matplotlib
+	pydata-sphinx-theme
 	sphinx
 	sphinx-changelog
 	sphinx-automodapi
-	sunpy-sphinx-theme
+	sphinx-design
+	sphinx-gallery
+	sphinxext-opengraph
 
 [options.package_data]
 xrayvision = data/*
 
 [tool:pytest]
 testpaths = "xrayvision" "docs"
 norecursedirs = ".tox" "build" "docs[\/]_build" "docs[\/]generated" "*.egg-info" "examples" "xrayvision[/\]_dev" ".jupyter" ".history" "tools"
 doctest_optionflags = NORMALIZE_WHITESPACE FLOAT_CMP ELLIPSIS
 doctest_plus = enabled
 text_file_format = rst
 addopts = --doctest-rst
 remote_data_strict = True
-
-[pycodestyle]
-max_line_length = 100
-
-[flake8]
-max-line-length = 100
-exclude = 
-	.git,
-	__pycache__,
-	docs/conf.py,
-	build,
-	sunpy/data/sample.py,
-	sunpy/extern/**,
-	sunpy/__init__.py,
-rst-directives = 
-	plot
+filterwarnings = 
 
 [isort]
-balanced_wrapping = True
-skip = sunpy/extern/,sunpy/cm/__init__.py,docs/conf.py,sunpy/__init__.py
+balanced_wrapping = true
+extend_skip = 
+	docs/conf.py,
+	xrayvision/__init__.py,
 default_section = THIRDPARTY
-include_trailing_comma = True
-known_astropy = astropy
-known_first_party = xrayvision
-length_sort = False
+include_trailing_comma = true
+known_first_party = stixpy
+length_sort = false
 length_sort_sections = stdlib
-line_length = 100
+line_length = 120
 multi_line_output = 3
 no_lines_before = LOCALFOLDER
-sections = STDLIB, THIRDPARTY, ASTROPY, FIRSTPARTY, LOCALFOLDER
+sections = STDLIB, THIRDPARTY, FIRSTPARTY, LOCALFOLDER
+
+[codespell]
+skip = ,*.fits,*.fts,*.header,*.json,*.xsh,*cache*,*egg*,*extern*,.git,.idea,.tox,_build,*truncated,*.svg,.asv_env,.history
+ignore-words-list = 
+	alog,
+	nd,
+	nin,
+	observ,
+	ot,
+	te,
+	upto,
+	afile,
+	precessed,
+	process,
+	technik
+
+[mypy]
+disable_error_code = import-untyped
 
 [coverage:run]
 omit = 
 	xrayvision/_sunpy_init*
 	xrayvision/conftest.py
 	xrayvision/*setup_package*
 	xrayvision/tests/*
```

### Comparing `xrayvisim-0.1.0rc1/setup.py` & `xrayvisim-0.2.0rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 from itertools import chain
 
 from setuptools import setup  # isort:skip
+
 try:
     # Recommended for setuptools 61.0.0+
     # (though may disappear in the future)
     from setuptools.config.setupcfg import read_configuration
 except ImportError:
     from setuptools.config import read_configuration
 
 ################################################################################
 # Programmatically generate some extras combos.
 ################################################################################
-extras = read_configuration("setup.cfg")['options']['extras_require']
+extras = read_configuration("setup.cfg")["options"]["extras_require"]
 
 # Dev is everything
-extras['dev'] = list(chain(*extras.values()))
+extras["dev"] = list(chain(*extras.values()))
 
 # All is everything but tests and docs
 exclude_keys = ("tests", "docs", "dev")
 ex_extras = dict(filter(lambda i: i[0] not in exclude_keys, extras.items()))
 # Concatenate all the values together for 'all'
-extras['all'] = list(chain.from_iterable(ex_extras.values()))
+extras["all"] = list(chain.from_iterable(ex_extras.values()))
 
 ################################################################################
 # Version configuration and setup call
 ################################################################################
 
 VERSION_TEMPLATE = """
 # Note that we need to fall back to the hard-coded version if either
@@ -39,11 +40,9 @@
     __version__ = get_version(root='..', relative_to=__file__)
 except Exception:
     __version__ = '{version}'
 """.lstrip()
 
 setup(
     extras_require=extras,
-    use_scm_version={'write_to': os.path.join('xrayvision', 'version.py'),
-                     'write_to_template': VERSION_TEMPLATE},
-
+    use_scm_version={"write_to": os.path.join("xrayvision", "version.py"), "write_to_template": VERSION_TEMPLATE},
 )
```

### Comparing `xrayvisim-0.1.0rc1/tox.ini` & `xrayvisim-0.2.0rc1/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{37,38,39}
+    py{39,310,311,312}
     build_docs
     codestyle
 isolated_build = true
 # This is included for testing of the template. You can remove it safely.
 skip_missing_interpreters = True
 requires =
     setuptools >=56, !=61.0.0
@@ -15,22 +15,22 @@
 
 # The following option combined with the use of the tox-pypi-filter above allows
 # project-wide pinning of dependencies, e.g. if new versions of pytest do not
 # work correctly with pytest-astropy plugins. Most of the time the pinnings file
 # should be empty.
 pypi_filter_requirements = https://raw.githubusercontent.com/sunpy/package-template/master/sunpy_version_pins.txt
 
-# Pass through the following environemnt variables which may be needed for the CI
-passenv = HOME WINDIR LC_ALL LC_CTYPE CC CI TRAVIS
+# Pass through the following environment variables which may be needed for the CI
+passenv = HOME, WINDIR, LC_ALL, LC_CTYPE, CC, CI, TRAVIS
 
 # Run the tests in a temporary directory to make sure that we don't import
 # the package from the source tree
 changedir = .tmp/{envname}
 
-# tox environments are constructued with so-called 'factors' (or terms)
+# tox environments are constructed with so-called 'factors' (or terms)
 # separated by hyphens, e.g. test-devdeps-cov. Lines below starting with factor:
 # will only take effect if that factor is included in the environment name. To
 # see a list of example environments that can be run, along with a description,
 # run:
 #
 #     tox -l -v
 #
@@ -43,22 +43,27 @@
     all
     tests
 commands =
     pytest --pyargs xrayvision {toxinidir}/docs --cov xrayvision --cov-config={toxinidir}/setup.cfg {posargs}
 
 
 [testenv:build_docs]
+allowlist_externals = sphinx-build
 changedir = docs
 description = invoke sphinx-build to build the HTML docs
-extras = docs
+extras =
+    docs
+    map
 commands =
+    pip freeze --all --no-input
     sphinx-build -W -b html . _build/html {posargs}
 
 
 [testenv:codestyle]
 skip_install = true
 description = Run all style and file checks with pre-commit
 deps =
     pre-commit
 commands =
+    python -V
     pre-commit install-hooks
     pre-commit run --all-files
```

### Comparing `xrayvisim-0.1.0rc1/xrayvision/clean.py` & `xrayvisim-0.2.0rc1/xrayvision/clean.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,44 +2,51 @@
 CLEAN algorithms.
 
 The CLEAN algorithm solves the deconvolution problem by assuming a model for the true sky intensity
 which is a collection of point sources or in the case of multiscale clean a collection of
 appropriate component shapes at different scales.
 
 """
+
 import logging
+from typing import Union, Optional
+from collections.abc import Iterable
 
+import astropy.units as u
 import numpy as np
+from astropy.convolution import Gaussian2DKernel
+from astropy.units import Quantity
+from numpy.typing import NDArray
 from scipy import signal
-from scipy.ndimage.interpolation import shift
+from scipy.ndimage import shift
 from sunpy.map.map_factory import Map
 
-from astropy.convolution import Gaussian2DKernel
+from xrayvision.imaging import vis_psf_image, vis_to_map
+from xrayvision.visibility import Visibilities
 
-from xrayvision.imaging import vis_psf_image
+__all__ = ["clean", "vis_clean", "ms_clean", "vis_ms_clean"]
 
-__all__ = ['clean', 'vis_clean', 'ms_clean', 'vis_ms_clean']
 
 logger = logging.getLogger(__name__)
-logger.setLevel('DEBUG')
+logger.setLevel("DEBUG")
 
 __common_clean_doc__ = r"""
-    clean_beam_width : `float`
+    clean_beam_width :
         The width of the gaussian to convolve the model with. If set to 0.0 \
         the gaussian to convolution is disabled
-    gain : `float`
+    gain :
         The gain per loop or loop gain
-    thres : `float`
+    thres :
         Terminates clean when ``residual.max() <= thres``
-    niter : `int`
+    niter :
         Maximum number of iterations to perform
 
     Returns
     -------
-    `numpy.ndarray`
+    :
         The CLEAN image 2D
 
     Notes
     -----
     The CLEAN algorithm can be summarised in pesudo code as follows:
 
     .. math::
@@ -55,156 +62,182 @@
        & \qquad i = i + 1 \\
        & \textbf{done} \\
        & \textbf{return}\  M,\ I^{Res}
 
     """
 
 
-def clean(dirty_map, dirty_beam, pixel=None, clean_beam_width=4.0,
-          gain=0.1, thres=0.01, niter=5000):
+@u.quantity_input
+def clean(
+    dirty_map: Quantity,
+    dirty_beam: Quantity,
+    pixel_size: Quantity[u.arcsec / u.pix] = None,
+    clean_beam_width: Optional[Quantity[u.arcsec]] = 4.0 * u.arcsec,
+    gain: Optional[float] = 0.1,
+    thres: Optional[float] = None,
+    niter: int = 5000,
+) -> Union[Quantity, NDArray[np.float64]]:
     r"""
     Clean the image using Hogbom's original method.
 
     CLEAN iteratively subtracts the PSF or dirty beam from the dirty map to create the residual.
-    At each iteration the location of the maximum residual is found and a shifted dirty beam is
-    subtracted that location updating the residual. This process continues until either `niter`
-    iterations is reached or the maximum residual <= `thres`.
+    At each iteration, the location of the maximum residual is found and a shifted dirty beam is
+    subtracted at that location. This process continues until either `niter` iterations are reached or
+    the maximum residual <= `thres`.
 
     Parameters
     ----------
-    dirty_map : `numpy.ndarray`
+    dirty_map :
         The dirty map to be cleaned 2D
-    dirty_beam : `numpy.ndarray`
+    dirty_beam :
         The dirty beam or point spread function (PSF) 2D must
-    pixel :
-        Size of a pixel
+    pixel_size :
+        The pixel size in arcsec
     """
     # Ensure both beam and map are even/odd on same axes
-    if not [x % 2 == 0 for x in dirty_map.shape] == [x % 2 == 0 for x in dirty_beam.shape]:
-        raise ValueError('')
+    # if not [x % 2 == 0 for x in dirty_map.shape] == [x % 2 == 0 for x in dirty_beam.shape]:
+    #     raise ValueError('')
     pad = [0 if x % 2 == 0 else 1 for x in dirty_map.shape]
 
-    # Assume beam, map center is in middle
-    beam_center = (dirty_beam.shape[0] - 1)/2.0, (dirty_beam.shape[1] - 1)/2.0
-    map_center = (dirty_map.shape[0] - 1)/2.0, (dirty_map.shape[1] - 1)/2.0
+    # Assume beam, map phase_center is in middle
+    beam_center = (dirty_beam.shape[0] - 1) / 2.0, (dirty_beam.shape[1] - 1) / 2.0
+    map_center = (dirty_map.shape[0] - 1) / 2.0, (dirty_map.shape[1] - 1) / 2.0
 
     # Work out size of map for slicing over-sized dirty beam
     shape = dirty_map.shape
     height = shape[0] // 2
     width = shape[1] // 2
 
     # max_beam = dirty_beam.max()
 
     # Model for sources
     model = np.zeros(dirty_map.shape)
-    componets = []
+    components = []
     for i in range(niter):
         # Find max in dirty map and save to point source
         mx, my = np.unravel_index(dirty_map.argmax(), dirty_map.shape)
         imax = dirty_map[mx, my]
         # TODO check if correct and how to undo
         # imax = imax * max_beam
         model[mx, my] += gain * imax
 
-        logger.info(f"Iter: {i}, strength: {imax}, location: {mx, my}")
+        if i % 25 == 0:
+            logger.debug(f"Iter: {i}, strength: {imax}, location: {mx, my}")
 
         offset = map_center[0] - mx, map_center[1] - my
         shifted_beam_center = int(beam_center[0] + offset[0]), int(beam_center[1] + offset[1])
         xr = slice(shifted_beam_center[0] - height, shifted_beam_center[0] + height + pad[0])
         yr = slice(shifted_beam_center[1] - width, shifted_beam_center[1] + width + pad[0])
 
         shifted = dirty_beam[xr, yr]
 
         comp = imax * gain * shifted
 
-        componets.append((mx, my, comp[mx, my]))
+        components.append((mx, my, comp[mx, my]))
 
         dirty_map = np.subtract(dirty_map, comp)
 
-        # if dirty_map.max() <= thres:
-        #      logger.info("Threshold reached")
-        #      break
-        # # el
-        # if np.abs(dirty_map.min()) > dirty_map.max():
-        #     logger.info("Largest residual negative")
-        #     break
+        if thres:
+            if np.abs(dirty_map).max() <= thres:
+                logger.info("Threshold reached")
+                break
+
+        if np.abs(dirty_map.min()) > dirty_map.max():
+            logger.info("Largest residual negative")
+            break
 
     else:
         print("Max iterations reached")
 
-    if clean_beam_width != 0.0:
-        # Convert from FWHM to StDev
-        x_stdev = (clean_beam_width/pixel[0] / (2.0 * np.sqrt(2.0 * np.log(2.0)))).value
-        y_stdev = (clean_beam_width/pixel[1] / (2.0 * np.sqrt(2.0 * np.log(2.0)))).value
-        clean_beam = Gaussian2DKernel(x_stdev, y_stdev, x_size=dirty_beam.shape[1],
-                                      y_size=dirty_beam.shape[0]).array
+    if clean_beam_width is not None:
+        # Convert from FWHM to StDev   FWHM = sigma*(8ln2)**0.5 = 2.3548200450309493
+        x_stdev = (clean_beam_width / pixel_size[1]).to_value(u.pix) / 2.3548200450309493
+        y_stdev = (clean_beam_width / pixel_size[0]).to_value(u.pix) / 2.3548200450309493
+        clean_beam = Gaussian2DKernel(x_stdev, y_stdev, x_size=dirty_beam.shape[1], y_size=dirty_beam.shape[0]).array
         # Normalise beam
         clean_beam = clean_beam / clean_beam.max()
 
         # Convolve clean beam with model and scale
-        clean_map = (signal.convolve2d(model, clean_beam/clean_beam.sum(), mode='same')
-                     / (pixel[0]*pixel[1]))
+        clean_map = signal.convolve2d(model, clean_beam / clean_beam.sum(), mode="same") / (
+            pixel_size[0].value * pixel_size[1].value
+        )
 
         # Scale residual map with model and scale
-        dirty_map = dirty_map / clean_beam.sum() / (pixel[0] * pixel[1])
-        return clean_map+dirty_map, model, dirty_map
+        dirty_map = dirty_map / clean_beam.sum() / (pixel_size[0].value * pixel_size[1].value)
+        return clean_map + dirty_map, model, dirty_map
 
-    return model+dirty_map, model, dirty_map
+    return model + dirty_map, model, dirty_map
 
 
-clean.__doc__ += __common_clean_doc__
+clean.__doc__ += __common_clean_doc__  # type: ignore
 
 
-def vis_clean(vis, shape, pixel, clean_beam_width=4.0, niter=100, map=True, **kwargs):
+@u.quantity_input
+def vis_clean(
+    vis: Visibilities,
+    shape: Quantity[u.pix],
+    pixel_size: Quantity[u.arcsec / u.pix],
+    clean_beam_width: Optional[Quantity[u.arcsec]] = 4.0,
+    niter: Optional[int] = 5000,
+    map: Optional[bool] = True,
+    gain: Optional[float] = 0.1,
+    **kwargs,
+):
     r"""
     Clean the visibilities using Hogbom's original method.
 
     A wrapper around lower level `clean` which calculates the dirty map and psf
 
     Parameters
     ----------
-    vis : `xrayvision.visibilty.Visibly`
+    vis :
         The visibilities to clean
     shape :
         Size of map
-    pixel :
-        Size of pixel
-    map : `boolean` optional
-        Return an `sunpy.map.Map` by default or data only if `False`
+    pixel_size :
+        The pixel size in arcsec
+    map :
+        Return a `sunpy.map.Map` by default or array only if `False`
     """
 
-    dirty_map = vis_to_map(vis, shape=shape, pixel_size=pixel)
-    dirty_beam = vis_psf_image(vis, shape=shape*3, pixel_size=pixel, map=False)
-    clean_map, model, residual = clean(dirty_map.data, dirty_beam.value, pixel=pixel,
-                                       clean_beam_width=clean_beam_width, niter=niter, **kwargs)
+    dirty_map = vis_to_map(vis, shape=shape, pixel_size=pixel_size, **kwargs)
+    dirty_beam_shape = [x.value * 3 + 1 if x.value * 3 % 2 == 0 else x.value * 3 for x in shape] * shape.unit
+    dirty_beam = vis_psf_image(vis, shape=dirty_beam_shape, pixel_size=pixel_size, **kwargs)
+    clean_map, model, residual = clean(
+        dirty_map.data,
+        dirty_beam.value,
+        pixel_size=pixel_size,
+        clean_beam_width=clean_beam_width,
+        gain=gain,
+        niter=niter,
+    )
     if not map:
         return clean_map, model, residual
 
     return [Map((data, dirty_map.meta)) for data in (clean_map, model, residual)]
 
 
-vis_clean.__doc__ += __common_clean_doc__
-
+vis_clean.__doc__ += __common_clean_doc__  # type: ignore
 
 __common_ms_clean_doc__ = r"""
     scales : array-like, optional, optional
         The scales to use eg ``[1, 2, 4, 8]``
-    clean_beam_width : `float`
+    clean_beam_width :
         The width of the gaussian to convolve the model with. If set to 0.0 the gaussian \
         convolution is disabled
-    gain : `float`
+    gain :
         The gain per loop or loop gain
-    thres : `float`
+    thres :
         Terminates clean when `residuals.max() <= thres``
-    niter : `int`
+    niter :
         Maximum number of iterations to perform
 
     Returns
     -------
-    `numpy.ndarray`
+    :
         Cleaned image
 
     Notes
     -----
     This is an implementation of the multiscale clean algorithm as outlined in [R1]_ adapted for \
     x-ray Fourier observations.
 
@@ -216,93 +249,108 @@
     ----------
     .. [R1] Cornwell, T. J., "Multiscale CLEAN Deconvolution of Radio Synthesis Images", IEEE Journal of Selected Topics in Signal Processing, vol 2, p793-801, Paper_ #noqa
 
     .. _Paper: https://ieeexplore.ieee.org/document/4703304/
     """
 
 
-def ms_clean(dirty_map, dirty_beam, pixel, scales=None,
-             clean_beam_width=4.0, gain=0.1, thres=0.01, niter=5000):
+@u.quantity_input
+def ms_clean(
+    dirty_map: Quantity,
+    dirty_beam: Quantity,
+    pixel_size: Quantity[u.arcsec / u.pix],
+    scales: Union[Iterable, NDArray, None] = None,
+    clean_beam_width: Quantity = 4.0 * u.arcsec,
+    gain: float = 0.1,
+    thres: float = 0.01,
+    niter: int = 5000,
+) -> Union[Quantity, NDArray[np.float64]]:
     r"""
     Clean the map using a multiscale clean algorithm.
 
     Parameters
     ----------
-    dirty_map : `numpy.ndarray`
+    dirty_map :
         The 2D dirty map to be cleaned
-    dirty_beam : `numpy.ndarray`
+    dirty_beam :
         The 2D dirty beam should have the same dimensions as `dirty_map`
+    pixel_size :
+        The pixel size in arcsec
     """
     # Compute the number of dyadic scales, their sizes and scale biases
-    number_of_scales = np.floor(np.log2(min(dirty_map.shape))).astype(int)
-    scale_sizes = 2**np.arange(number_of_scales)
+    number_of_scales: int = np.floor(np.log2(min(dirty_map.shape))).astype(int)
+    scale_sizes: NDArray[np.int_] = 2 ** np.arange(number_of_scales)
 
     if scales:
         scales = np.array(scales)
         number_of_scales = len(scales)
         scale_sizes = scales
 
     scale_sizes = np.where(scale_sizes == 0, 1, scale_sizes)
 
     scale_biases = 1 - 0.6 * scale_sizes / scale_sizes.max()
 
     model = np.zeros(dirty_map.shape)
 
-    map_center = (dirty_map.shape[0] - 1)/2.0, (dirty_map.shape[1] - 1)/2.0
+    map_center = (dirty_map.shape[0] - 1) / 2.0, (dirty_map.shape[1] - 1) / 2.0
     height = dirty_map.shape[0] // 2
     width = dirty_map.shape[1] // 2
     pad = [0 if x % 2 == 0 else 1 for x in dirty_map.shape]
 
     # Pre-compute scales, residual maps and dirty beams at each scale and dirty beam cross terms
     scales = np.zeros((dirty_map.shape[0], dirty_map.shape[1], number_of_scales))
     scaled_residuals = np.zeros((dirty_map.shape[0], dirty_map.shape[1], number_of_scales))
     scaled_dirty_beams = np.zeros((dirty_beam.shape[0], dirty_beam.shape[1], number_of_scales))
     max_scaled_dirty_beams = np.zeros(number_of_scales)
     cross_terms = {}
 
     for i, scale in enumerate(scale_sizes):
-        scales[:, :, i] = component(scale=scale, shape=dirty_map.shape)
-        scaled_residuals[:, :, i] = signal.convolve(dirty_map, scales[:, :, i], mode='same')
-        scaled_dirty_beams[:, :, i] = signal.convolve(dirty_beam, scales[:, :, i], mode='same')
+        scales[:, :, i] = _component(scale=scale, shape=dirty_map.shape)
+        scaled_residuals[:, :, i] = signal.convolve(dirty_map, scales[:, :, i], mode="same")
+        scaled_dirty_beams[:, :, i] = signal.convolve(dirty_beam, scales[:, :, i], mode="same")
         max_scaled_dirty_beams[i] = scaled_dirty_beams[:, :, i].max()
         for j in range(i, number_of_scales):
             cross_terms[(i, j)] = signal.convolve(
-                signal.convolve(dirty_beam, scales[:, :, i], mode='same'),
-                scales[:, :, j], mode='same')
+                signal.convolve(dirty_beam, scales[:, :, i], mode="same"), scales[:, :, j], mode="same"
+            )
 
     # Clean loop
     for i in range(niter):
         # print(f'Clean loop {i}')
         # For each scale find the strength and location of max residual
         # Chose scale with has maximum strength
-        max_index = np.argmax(scaled_residuals)
-        max_x, max_y, max_scale = np.unravel_index(max_index, scaled_residuals.shape)
+        max_index: int = np.argmax(scaled_residuals).astype(int)
+        max_x: int
+        max_y: int
+        max_scale: int
+        max_x, max_y, max_scale = (int(x) for x in np.unravel_index(max_index, scaled_residuals.shape))
 
         strength = scaled_residuals[max_x, max_y, max_scale]
 
         # Adjust for the max of scaled beam
         strength = strength / max_scaled_dirty_beams[max_scale]
 
         logger.info(f"Iter: {i}, max scale: {max_scale}, strength: {strength}")
 
         # Loop gain and scale dependent bias
         strength = strength * scale_biases[max_scale] * gain
 
-        beam_center = [(scaled_dirty_beams[:, :, max_scale].shape[0] - 1) / 2.0,
-                       (scaled_dirty_beams[:, :, max_scale].shape[1] - 1) / 2.0]
+        beam_center = [
+            (scaled_dirty_beams[:, :, max_scale].shape[0] - 1) / 2.0,
+            (scaled_dirty_beams[:, :, max_scale].shape[1] - 1) / 2.0,
+        ]
 
         offset = map_center[0] - max_x, map_center[1] - max_y
         shifted_beam_center = int(beam_center[0] + offset[0]), int(beam_center[1] + offset[1])
         xr = slice(shifted_beam_center[0] - height, shifted_beam_center[0] + height + pad[0])
         yr = slice(shifted_beam_center[1] - width, shifted_beam_center[1] + width + pad[0])
 
         # shifted = dirty_beam[xr, yr]
 
-        comp = strength * shift(scales[:, :, max_scale],
-                                (max_x - map_center[0], max_y - map_center[1]), order=0)
+        comp = strength * shift(scales[:, :, max_scale], (max_x - map_center[0], max_y - map_center[1]), order=0)
 
         # comp = strength * scales[xr, yr]
 
         # Add this component to current model
         model = np.add(model, comp)
 
         # Update all images using precomputed terms
@@ -316,81 +364,114 @@
             #                         (max_x - beam_center[0], max_y - beam_center[1]), order=0)
 
             comp = strength * cross_term[xr, yr]
 
             scaled_residuals[:, :, j] = np.subtract(scaled_residuals[:, :, j], comp)
 
         # End max(res(a)) or niter
-        if scaled_residuals[:, :, max_scale].max() <= thres:
+        if np.abs(scaled_residuals[:, :, max_scale].max()) <= thres:
             logger.info("Threshold reached")
-            # break
+            break
 
         # Largest scales largest residual is negative
         if np.abs(scaled_residuals[:, :, 0].min()) > scaled_residuals[:, :, 0].max():
             logger.info("Max scale residual negative")
             break
 
     else:
         logger.info("Max iterations reached")
 
-    # Convolve model with clean beam  B_G * I^M
-    if clean_beam_width != 0.0:
-        x_stdev = (clean_beam_width/pixel[0] / (2.0 * np.sqrt(2.0 * np.log(2.0)))).value
-        y_stdev = (clean_beam_width/pixel[1] / (2.0 * np.sqrt(2.0 * np.log(2.0)))).value
-        clean_beam = Gaussian2DKernel(x_stdev, y_stdev, x_size=dirty_beam.shape[1],
-                                      y_size=dirty_beam.shape[0]).array
+    # Convolve model with clean beam B_G * I^M
+    if clean_beam_width is not None:
+        x_stdev = ((clean_beam_width / pixel_size[0]).to_value(u.pix) / (2.0 * np.sqrt(2.0 * np.log(2.0)))).value
+        y_stdev = ((clean_beam_width / pixel_size[1]).to_value(u.pix) / (2.0 * np.sqrt(2.0 * np.log(2.0)))).value
+        clean_beam = Gaussian2DKernel(x_stdev, y_stdev, x_size=dirty_beam.shape[1], y_size=dirty_beam.shape[0]).array
 
         # Normalise beam
         clean_beam = clean_beam / clean_beam.max()
 
-        clean_map = signal.convolve2d(model, clean_beam, mode='same') / (pixel[0]*pixel[1])
+        clean_map = signal.convolve2d(model, clean_beam, mode="same") / (pixel_size[0] * pixel_size[1])
 
         # Scale residual map with model and scale
-        dirty_map = (scaled_residuals / clean_beam.sum() / (pixel[0] * pixel[1])).sum(axis=2)
+        dirty_map = (scaled_residuals / clean_beam.sum() / (pixel_size[0] * pixel_size[1])).sum(axis=2)
 
-        return clean_map+dirty_map, model, dirty_map
+        return clean_map + dirty_map, model, dirty_map
     # Add residuals B_G * I^M + I^R
     return model, scaled_residuals.sum(axis=2)
 
 
-ms_clean.__doc__ += __common_ms_clean_doc__
+ms_clean.__doc__ += __common_ms_clean_doc__  # type: ignore
 
 
-def vis_ms_clean(vis, shape, pixel, scales=None, clean_beam_width=4.0,
-                 gain=0.1, thres=0.01, niter=5000, map=True):
+def vis_ms_clean(
+    vis: Visibilities,
+    shape: Quantity[u.pix],
+    pixel_size: Quantity[u.arcsec / u.pix],
+    scales: Optional[Iterable],
+    clean_beam_width: Optional[Quantity[u.arcsec]] = 4.0,
+    niter: Optional[int] = 5000,
+    map: Optional[bool] = True,
+    gain: Optional[float] = 0.1,
+    thres: Optional[float] = 0.01,
+) -> Union[Quantity, NDArray[np.float64]]:
     r"""
     Clean the visibilities using a multiscale clean method.
 
     A wrapper around `ms_clean` which calculates the dirty map and psf.
 
     Parameters
     ----------
-    vis : `xrayvision.visibilty.Visibly`
+    vis :
         The visibilities to clean
     shape :
         Size of map
-    pixel :
-        Size of pixel
+    pixel_size :
+        The pixel size in arcsec
+    scales : array-like, optional, optional
+        The scales to use eg ``[1, 2, 4, 8]``
+    clean_beam_width :
+        The width of the gaussian to convolve the model with. If set to 0.0 the gaussian \
+        convolution is disabled
+    gain :
+        The gain per loop or loop gain
+    thres :
+        Terminates clean when `residuals.max() <= thres``
+    niter :
+        Maximum number of iterations to perform
+    map :
+        Return a `sunpy.map.Map` by default or array only if `False`
+
+    Returns
+    -------
+    :
+        Cleaned image
 
     """
-    dirty_map = vis_to_map(vis, shape=shape, pixel_size=pixel)
-    dirty_beam = vis_psf_image(vis, shape=shape * 3, pixel_size=pixel, map=False)
-    clean_map, model, residual = ms_clean(dirty_map.data, dirty_beam, scales=scales,
-                                          clean_beam_width=clean_beam_width, gain=gain,
-                                          thres=thres, niter=niter)
+    dirty_map = vis_to_map(vis, shape=shape, pixel_size=pixel_size)
+    dirty_beam = vis_psf_image(vis, shape=shape * 3, pixel_size=pixel_size)
+    clean_map, model, residual = ms_clean(
+        dirty_map.data,
+        dirty_beam,
+        pixel_size=pixel_size,
+        scales=scales,
+        clean_beam_width=clean_beam_width,
+        gain=gain,
+        thres=thres,
+        niter=niter,
+    )
     if not map:
         return clean_map, model, residual
 
     return [Map((data, dirty_map.meta)) for data in (clean_map, model, residual)]
 
 
-vis_ms_clean.__doc__ += __common_ms_clean_doc__
+# vis_ms_clean.__doc__ += __common_ms_clean_doc__
 
 
-def radial_prolate_sphereoidal(nu):
+def _radial_prolate_sphereoidal(nu):
     r"""
     Calculate prolate spheroidal wave function approximation.
 
     Parameters
     ----------
     nu : `float`
         The radial value to evaluate the function at
@@ -454,20 +535,20 @@
             top += p[k, part] * np.power(delnusq, k)
 
         bot = q[0, part]
         for k in range(1, n_q):
             bot += q[k, part] * np.power(delnusq, k)
 
         if bot != 0.0:
-            return top/bot
+            return top / bot
         else:
             return 0
 
 
-def vec_radial_prolate_sphereoidal(nu):
+def _vec_radial_prolate_sphereoidal(nu):
     r"""
     Calculate prolate spheroidal wave function approximation.
 
     Parameters
     ----------
     nu : `float` array
         The radial value to evaluate the function at
@@ -531,22 +612,22 @@
     bot[upper] = q[0, 1]
 
     j = np.arange(1, n_q)
     bot[lower] += np.sum(q[j, 0, np.newaxis] * np.power(delnusq[lower], j[..., np.newaxis]), axis=0)
     bot[upper] += np.sum(q[j, 1, np.newaxis] * np.power(delnusq[upper], j[..., np.newaxis]), axis=0)
 
     out = np.zeros(nu.shape)
-    out[bot != 0] = top[bot != 0]/bot[bot != 0]
+    out[bot != 0] = top[bot != 0] / bot[bot != 0]
     out = np.where(nu <= 0, 1.0, out)
     out = np.where(nu >= 1, 0.0, out)
 
     return out
 
 
-def component(scale, shape):
+def _component(scale, shape):
     r"""
 
     Parameters
     ----------
     scale
 
     Returns
@@ -565,22 +646,22 @@
     refx, refy = (np.array(shape) - 1) / 2.0
 
     if scale == 0.0:
         wave_amp = np.zeros(shape)
         wave_amp[int(refx), int(refy)] = 1
         return wave_amp
 
-    xy = np.mgrid[0:shape[0]:1, 0:shape[1]:1]
-    radii_squared = ((xy[0, :, :] - refx) / scale)**2 + ((xy[1, :, :] - refy) / scale)**2
+    xy = np.mgrid[0 : shape[0] : 1, 0 : shape[1] : 1]
+    radii_squared = ((xy[0, :, :] - refx) / scale) ** 2 + ((xy[1, :, :] - refy) / scale) ** 2
 
     rad_zeros_indices = radii_squared <= 0.0
     amp_zero_indices = radii_squared >= 1.0
 
-    wave_amp = vec_radial_prolate_sphereoidal(np.sqrt(radii_squared.reshape(radii_squared.size)))
+    wave_amp = _vec_radial_prolate_sphereoidal(np.sqrt(radii_squared.reshape(radii_squared.size)))
     wave_amp = wave_amp.reshape(shape)
-    wave_amp[rad_zeros_indices] = vec_radial_prolate_sphereoidal([0])[0]
+    wave_amp[rad_zeros_indices] = _vec_radial_prolate_sphereoidal([0])[0]
 
     wave_amp = wave_amp * (1 - radii_squared)
 
     wave_amp[amp_zero_indices] = 0.0
 
     return wave_amp
```

### Comparing `xrayvisim-0.1.0rc1/xrayvision/imaging.py` & `xrayvisim-0.2.0rc1/xrayvision/imaging.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,66 @@
-import numpy as np
-from sunpy.map import Map
+from typing import Optional
 
 import astropy.units as apu
+import numpy as np
+from astropy.units import Quantity
+from sunpy.map import GenericMap, Map
 
 from xrayvision.transform import dft_map, idft_map
-from xrayvision.visibility import Visibility
+from xrayvision.visibility import Visibilities
 
-__all__ = ['get_weights', 'validate_and_expand_kwarg', 'vis_psf_image', 'vis_psf_map',
-           'vis_to_image', 'vis_to_map', 'generate_header', 'image_to_vis', 'map_to_vis']
+__all__ = [
+    "get_weights",
+    "validate_and_expand_kwarg",
+    "vis_psf_image",
+    "vis_psf_map",
+    "vis_to_image",
+    "vis_to_map",
+    "generate_header",
+    "image_to_vis",
+    "map_to_vis",
+]
 
-ANGLE = apu.get_physical_type('angle')
+ANGLE = apu.get_physical_type(apu.deg)
+WEIGHT_SCHEMES = ("natural", "uniform")
 
 
-def get_weights(vis, natural=True, norm=True):
+def get_weights(vis: Visibilities, scheme: str = "natural", norm: bool = True) -> np.ndarray:
     r"""
-    Return natural spatial frequency weight factor for each visibility.
+    Return spatial frequency weight factors for each visibility.
 
     Defaults to use natural weighting scheme given by `(vis.u**2 + vis.v**2)^{1/2}`.
 
     Parameters
     ----------
-    vis : `xrayvision.visibility.Visibility`
+    vis :
         Input visibilities
-    natural : `boolean` optional
-        Use natural or uniform weighting scheme
-    norm : `boolean`
-        Normalise the weighs before returning
+    scheme :
+        Weighting scheme to use, defaults to natural
+    norm :
+        Normalise the weighs before returning, defaults to True.
 
     Returns
     -------
-    `weights`
 
     """
+    if scheme not in WEIGHT_SCHEMES:
+        raise ValueError(f"Invalid weighting scheme {scheme}, must be one of: {WEIGHT_SCHEMES}")
     weights = np.sqrt(vis.u**2 + vis.v**2).value
-    if not natural:
-        weights = np.ones_like(vis.vis, dtype=float)
+    if scheme == "natural":
+        weights = np.ones_like(vis.visibilities, dtype=float)
 
     if norm:
         weights /= weights.sum()
 
     return weights
 
 
-def validate_and_expand_kwarg(q, name=''):
+@apu.quantity_input()
+def validate_and_expand_kwarg(q: Quantity, name: Optional[str] = "") -> Quantity:
     r"""
     Expand a scalar or array of size one to size two by repeating.
 
     Parameters
     ----------
     q : `astropy.units.quantity.Quantity`
         Input value
@@ -68,244 +82,285 @@
 
     """
     q = np.atleast_1d(q)
     if q.shape == (1,):
         q = np.repeat(q, 2)
 
     if q.shape != (2,):
-        raise ValueError(f'{name} argument must be scalar or an 1D array of size 1 or 2.')
+        raise ValueError(f"{name} argument must be scalar or an 1D array of size 1 or 2.")
 
     return q
 
 
-@apu.quantity_input(shape=apu.pixel, pixel_size='angle')
-def vis_psf_image(vis, *, shape=(65, 65)*apu.pixel, pixel_size=2*apu.arcsec, natural=True):
+@apu.quantity_input
+def image_to_vis(
+    image: Quantity,
+    *,
+    u: Quantity[apu.arcsec**-1],
+    v: Quantity[apu.arcsec**-1],
+    phase_center: Optional[Quantity[apu.arcsec]] = (0.0, 0.0) * apu.arcsec,
+    pixel_size: Optional[Quantity[apu.arcsec / apu.pix]] = 1.0 * apu.arcsec / apu.pix,
+) -> Visibilities:
+    r"""
+    Return a Visibilities object created from the image and u, v sampling.
+
+    Parameters
+    ----------
+    image :
+        The 2D input image
+    u :
+        Array of u coordinates where the visibilities will be evaluated
+    v :
+        Array of v coordinates where the visibilities will be evaluated
+    phase_center :
+        The coordinates the phase_center.
+    pixel_size :
+        Size of pixels, if only one value is passed, assume square pixels (repeating the value).
+
+    Returns
+    -------
+    :
+        The new Visibilities object
+
     """
-    Create the point spread function for given u, v point of the visibilities.
+    pixel_size = validate_and_expand_kwarg(pixel_size, "pixel_size")
+    if not (apu.get_physical_type((1 / u).unit) == ANGLE and apu.get_physical_type((1 / v).unit) == ANGLE):
+        raise ValueError("u and v must be inverse angle (e.g. 1/deg or 1/arcsec")
+    vis = dft_map(
+        image, u=u, v=v, phase_center=[0.0, 0.0] * apu.arcsec, pixel_size=pixel_size
+    )  # TODO: adapt to generic map center
+    return Visibilities(vis, u=u, v=v, phase_center=phase_center)
+
+
+@apu.quantity_input()
+def vis_to_image(
+    vis: Visibilities,
+    shape: Quantity[apu.pix] = (65, 65) * apu.pixel,
+    pixel_size: Optional[Quantity[apu.arcsec / apu.pix]] = 1 * apu.arcsec / apu.pix,
+    scheme: str = "natural",
+) -> Quantity:
+    """
+    Create an image by 'back projecting' the given visibilities onto the sky.
 
     Parameters
     ----------
-    vis : `xrayvision.visibility.Visibility`
+    vis :
         Input visibilities
-    shape : `astropy.units.quantity.Quantity`, optional
-        Shape of the image, if only one value is given assume square (repeating the value).
-    pixel_size : `astropy.units.quantity.Quantity`, optional
-        Size of pixels, if only one value is given assume square pixels (repeating the value).
-    natural : `boolean` optional
-        Weight scheme use natural by default, uniform if `False`
+    shape :
+        Shape of the image, if only one value is passed assume square (repeating the value).
+    pixel_size :
+        Size of pixels, if only one value is passed assume square pixels (repeating the value).
+    scheme :
+        Weight scheme natural by default.
 
     Returns
     -------
-    `astropy.units.quantity.Quantity`
-        Point spread function
+    `~astropy.units.Quantity`
+        Back projection image
 
     """
-    shape = validate_and_expand_kwarg(shape, 'shape')
-    pixel_size = validate_and_expand_kwarg(pixel_size, 'pixel_size')
-    shape = shape.to_value(apu.pixel)
-    weights = get_weights(vis, natural=natural)
+    shape = validate_and_expand_kwarg(shape, "shape")
+    pixel_size = validate_and_expand_kwarg(pixel_size, "pixel_size")
+    shape = shape.to(apu.pixel)
+    weights = get_weights(vis, scheme=scheme)
+    bp_arr = idft_map(
+        vis.visibilities,
+        u=vis.u,
+        v=vis.v,
+        shape=shape,
+        weights=weights,
+        pixel_size=pixel_size,
+        phase_center=[0.0, 0.0] * apu.arcsec,  # TODO update to have generic image center
+    )
 
-    # Make sure psf is always odd so power is in exactly one pixel
-    m, n = [s//2 * 2 + 1 for s in shape]
-    psf_arr = idft_map(np.ones(vis.vis.shape)*vis.vis.unit, u=vis.u, v=vis.v,
-                       shape=(m, n), weights=weights, pixel_size=pixel_size)
-    return psf_arr
+    return bp_arr
 
 
-@apu.quantity_input(shape=apu.pixel, pixel_size='angle')
-def vis_psf_map(vis, *, shape=(65, 65)*apu.pixel, pixel_size=2*apu.arcsec, natural=True):
+@apu.quantity_input
+def vis_psf_map(
+    vis: Visibilities,
+    *,
+    shape: Quantity[apu.pix] = (65, 65) * apu.pixel,
+    pixel_size: Optional[Quantity[apu.arcsec / apu.pix]] = 1 * apu.arcsec / apu.pix,
+    scheme: Optional[str] = "natural",
+) -> GenericMap:
     r"""
     Create a map of the point spread function for given the visibilities.
 
     Parameters
     ----------
-    vis : `xrayvision.visibility.Visibility`
+    vis :
         Input visibilities
-    shape : `astropy.units.quantity.Quantity`, optional
-        Shape of the image, if only one value is given assume square (repeating the value).
-    pixel_size : `Tuple[~astropy.units.Quantity]`, optional
-        Size of pixels, if only one value is given assume square pixels (repeating the value).
-    natural : `boolean` optional
-        Weight scheme use natural by default, uniform if `False`
+    shape :
+        Shape of the image, if only one value is passed, assume square (repeating the value).
+    pixel_size :
+        Size of pixels, if only one value is passed, assume square pixels (repeating the value).
+    scheme :
+        Weight scheme to use natural by default.
 
     Returns
     -------
-
+    :
+        Map of the point spread function
     """
-    shape = validate_and_expand_kwarg(shape, 'shape')
-    pixel_size = validate_and_expand_kwarg(pixel_size, 'pixel_size')
+    shape = validate_and_expand_kwarg(shape, "shape")
+    pixel_size = validate_and_expand_kwarg(pixel_size, "pixel_size")
     header = generate_header(vis, shape=shape, pixel_size=pixel_size)
-    psf = vis_psf_image(vis, shape=shape, pixel_size=pixel_size, natural=natural)
+    psf = vis_psf_image(vis, shape=shape, pixel_size=pixel_size, scheme=scheme)
     return Map((psf, header))
 
 
-@apu.quantity_input(shape=apu.pixel, pixel_size='angle')
-def vis_to_image(vis, shape=(65, 65)*apu.pixel, pixel_size=2*apu.arcsec, natural=True):
+@apu.quantity_input()
+def vis_psf_image(
+    vis: Visibilities,
+    *,
+    shape: Quantity[apu.pix] = (65, 65) * apu.pixel,
+    pixel_size: Quantity[apu.arcsec / apu.pix] = 1 * apu.arcsec / apu.pix,
+    scheme: str = "natural",
+) -> Quantity:
     """
-    Create an image by 'back projecting' the given visibilities onto the sky.
+    Create the point spread function for given u, v point of the visibilities.
 
     Parameters
     ----------
-    vis : `xrayvision.visibility.Visibility`
+    vis :
         Input visibilities
-    shape : `~astropy.units.Quantity`
-        Shape of the image, if only one value is given assume square (repeating the value).
-    pixel_size : `~astropy.units.Quantity`
-        Size of pixels, if only one value is given assume square pixels (repeating the value).
-    natural : `boolean` optional
-        Weight scheme use natural by default, uniform if `False`
+    shape :
+        Shape of the image, if only one value passed, assume square (repeating the value).
+    pixel_size :
+        Size of pixels, if only one value is passed, assume square pixels (repeating the value).
+    scheme :
+        Weight scheme, natural by default.
 
     Returns
     -------
-    `~astropy.units.Quantity`
-        Back projection image
+    :
+        Point spread function
 
     """
-    shape = validate_and_expand_kwarg(shape, 'shape')
-    pixel_size = validate_and_expand_kwarg(pixel_size, 'pixel_size')
-    shape = shape.to_value(apu.pixel)
-    weights = get_weights(vis, natural=natural)
-    bp_arr = idft_map(vis.vis, u=vis.u, v=vis.v, shape=shape,
-                      weights=weights, pixel_size=pixel_size, center=vis.center)
+    shape = validate_and_expand_kwarg(shape, "shape")
+    pixel_size = validate_and_expand_kwarg(pixel_size, "pixel_size")
+    shape = shape.to(apu.pixel)
+    weights = get_weights(vis, scheme=scheme)
 
-    return bp_arr
+    # Make sure psf is always odd so power is in exactly one pixel
+    shape = [s // 2 * 2 + 1 for s in shape.to_value(apu.pix)] * shape.unit
+    psf_arr = idft_map(
+        np.ones(vis.visibilities.shape) * vis.visibilities.unit,
+        u=vis.u,
+        v=vis.v,
+        shape=shape,
+        weights=weights,
+        pixel_size=pixel_size,
+    )
+    return psf_arr
 
 
-@apu.quantity_input(shape=apu.pixel, pixel_size='angle')
-def vis_to_map(vis, shape=(65, 65)*apu.pixel, pixel_size=2*apu.arcsec, natural=True):
+@apu.quantity_input()
+def vis_to_map(
+    vis: Visibilities,
+    shape: Quantity[apu.pix] = (65, 65) * apu.pixel,
+    pixel_size: Optional[Quantity[apu.arcsec / apu.pix]] = 1 * apu.arcsec / apu.pixel,
+    scheme: Optional[str] = "natural",
+) -> GenericMap:
     r"""
     Create a map by performing a back projection of inverse transform on the visibilities.
 
     Parameters
     ----------
-    vis : `xrayvision.visibility.Visibility`
+    vis :
         Input visibilities
-    shape : `int` (m, n)
-        Shape of the image, if only one value is given assume square (repeating the value).
-    pixel_size : `float` (dx, dy), optional
-        Size of pixels, if only one value is given assume square pixels (repeating the value).
-    natural : `boolean` optional
-        Weight scheme use natural by default, uniform if `False`.
+    shape :
+        Shape of the image, if only one value is passed, assume square (repeating the value).
+    pixel_size :
+        Size of pixels, if only one value is passed, assume square pixels (repeating the value).
+    scheme :
+        Weight scheme natural by default.
 
     Returns
     -------
-    `sunpy.map.Map`
-        Map object with the map created from the visibilities and the metadata will contain the
-        offset and the pixel size
+    :
+        Map object with the map created from the visibilities and the metadata will contain the offset and the pixel size
 
     """
-    shape = validate_and_expand_kwarg(shape, 'shape')
-    pixel_size = validate_and_expand_kwarg(pixel_size, 'pixel_size')
+    shape = validate_and_expand_kwarg(shape, "shape")
+    pixel_size = validate_and_expand_kwarg(pixel_size, "pixel_size")
     header = generate_header(vis, shape=shape, pixel_size=pixel_size)
 
-    image = vis_to_image(vis, shape=shape, pixel_size=pixel_size, natural=natural)
+    image = vis_to_image(vis, shape=shape, pixel_size=pixel_size, scheme=scheme)
     return Map((image, header))
 
 
-def generate_header(vis, *, shape, pixel_size):
+@apu.quantity_input()
+def generate_header(vis: Visibilities, *, shape: Quantity[apu.pix], pixel_size: Quantity[apu.arcsec / apu.pix]) -> dict:
     r"""
     Generate a map head given the visibilities, pixel size and shape
 
     Parameters
     ----------
     vis :
-    shape : `~astropy.units.Quantity`
-        Shape of the image, if only one value is given assume square (repeating the value).
-    pixel_size : `~astropy.units.Quantity`
-        Size of pixels, if only one value is given assume square pixels (repeating the value)
-    Returns
-    -------
-
-    """
-    header = {'crval1': vis.center[0, 0].value if vis.center.ndim == 2 else vis.center[0].value,
-              'crval2': vis.center[0, 1].value if vis.center.ndim == 2 else vis.center[1].value,
-              'cdelt1': pixel_size[0].value,
-              'cdelt2': pixel_size[1].value,
-              'ctype1': 'HPLN-TAN',
-              'ctype2': 'HPLT-TAN',
-              'naxis': 2,
-              'naxis1': shape[0].value,
-              'naxis2': shape[1].value,
-              'cunit1': 'arcsec', 'cunit2': 'arcsec'}
-    if vis.center:
-        header['crval1'] = vis.center[0].value
-        header['crval2'] = vis.center[1].value
-    if pixel_size:
-        if pixel_size.ndim == 0:
-            header['cdelt1'] = pixel_size.value
-            header['cdelt2'] = pixel_size.value
-        elif pixel_size.ndim == 1 and pixel_size.size == 2:
-            header['cdelt1'] = pixel_size[0].value
-            header['cdelt2'] = pixel_size[1].value
-        else:
-            raise ValueError(f"pixel_size can have a length of 1 or 2 not {pixel_size.shape}")
-    return header
-
-
-@apu.quantity_input(center='angle', pixel_size='angle')
-def image_to_vis(image, *, u, v, center=(0.0, 0.0) * apu.arcsec, pixel_size=2.0*apu.arcsec):
-    r"""
-    Return a Visibility created from the image and u, v sampling.
-
-    Parameters
-    ----------
-    image : `numpy.ndarray`
-        The 2D input image
-    u : `astropy.units.Quantity`
-        Array of u coordinates where the visibilities will be evaluated
-    v : `astropy.units.Quantity`
-        Array of v coordinates where the visibilities will be evaluated
-    center : `~astropy.units.Quantity` (x, y)
-        The coordinates of the center of the image.
-    pixel_size : `~astropy.units.Quantity`
-        Size of pixels, if only one value is given assume square pixels (repeating the value).
+        Input visibilities.
+    shape :
+        Shape of the image, if only one value is passed assume square (repeating the value).
+    pixel_size :
+        Size of pixels, if only one value is passed assume square pixels (repeating the value)
 
     Returns
     -------
-    `Visibility`
-
-        The new visibility object
-
+    :
     """
-    pixel_size = validate_and_expand_kwarg(pixel_size, 'pixel_size')
-    if not apu.get_physical_type(1/u) == ANGLE and apu.get_physical_type(1 / v) == ANGLE:
-        raise ValueError('u and v must be inverse angle (e.g. 1/deg or 1/arcsec')
-    vis = dft_map(image, u=u, v=v, center=center, pixel_size=pixel_size)
-    return Visibility(vis, u=u, v=v, center=center)
+    header = {
+        "crval1": (vis.phase_center[1]).to_value(apu.arcsec),
+        "crval2": (vis.phase_center[0]).to_value(apu.arcsec),
+        "cdelt1": (pixel_size[1] * apu.pix).to_value(apu.arcsec),
+        "cdelt2": (pixel_size[0] * apu.pix).to_value(apu.arcsec),
+        "ctype1": "HPLN-TAN",
+        "ctype2": "HPLT-TAN",
+        "naxis": 2,
+        "naxis1": shape[1].value,
+        "naxis2": shape[0].value,
+        "cunit1": "arcsec",
+        "cunit2": "arcsec",
+    }
+    return header
 
 
-def map_to_vis(amap, *, u, v):
+@apu.quantity_input()
+def map_to_vis(amap: GenericMap, *, u: Quantity[1 / apu.arcsec], v: Quantity[1 / apu.arcsec]) -> Visibilities:
     r"""
-    Return a Visibility object created from the map and u, v sampling.
+    Return a Visibilities object created from the map, sampling it at give `u`, `v` coordinates.
 
     Parameters
     ----------
-    amap : `sunpy.map.Map`
-        The input map
-    u : `numpy.ndarray`
+    amap :
+        Input map.
+    u :
         Array of u coordinates where the visibilities will be evaluated
-    v : `numpy.ndarray`
+    v :
         Array of v coordinates where the visibilities will be evaluated
 
     Returns
     -------
-    `Visibility`
-        The new visibility object
+    :
+        The new Visibilities object
 
     """
-    if not apu.get_physical_type(1/u) == ANGLE and apu.get_physical_type(1 / v) == ANGLE:
-        raise ValueError('u and v must be inverse angle (e.g. 1/deg or 1/arcsec')
+    if not apu.get_physical_type(1 / u) == ANGLE and apu.get_physical_type(1 / v) == ANGLE:
+        raise ValueError("u and v must be inverse angle (e.g. 1/deg or 1/arcsec")
     meta = amap.meta
-    new_pos = np.array([0., 0.])
+    new_pos = np.array([0.0, 0.0])
     if "crval1" in meta:
-        new_pos[0] = float(meta["crval1"])
+        new_pos[1] = float(meta["crval1"])
     if "crval2" in meta:
-        new_pos[1] = float(meta["crval2"])
+        new_pos[0] = float(meta["crval2"])
 
-    new_psize = np.array([1., 1.])
+    new_psize = np.array([1.0, 1.0])
     if "cdelt1" in meta:
-        new_psize[0] = float(meta["cdelt1"])
+        new_psize[1] = float(meta["cdelt1"])
     if "cdelt2" in meta:
-        new_psize[1] = float(meta["cdelt2"])
+        new_psize[0] = float(meta["cdelt2"])
+
+    vis = image_to_vis(
+        amap.quantity, u=u, v=v, pixel_size=new_psize * apu.arcsec / apu.pix, phase_center=new_pos * apu.arcsec
+    )
 
-    return image_to_vis(amap.data, u=u, v=v, center=new_pos * apu.arcsec,
-                        pixel_size=new_psize * apu.arcsec)
+    return vis
```

### Comparing `xrayvisim-0.1.0rc1/xrayvision/mem.py` & `xrayvisim-0.2.0rc1/xrayvision/mem.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 r"""
 Implementation of Maximum Entropy Method
 """
 
 from types import SimpleNamespace
+from typing import Union, Optional
 
+import astropy.units as apu
 import numpy as np
+from astropy.units import Quantity
 from numpy.linalg import norm
+from numpy.typing import NDArray
+from sunpy.map import Map
 
-import astropy.units as apu
-
+from xrayvision.imaging import generate_header
 from xrayvision.transform import generate_xy
 from xrayvision.utils import get_logger
 
-__all__ = ['get_entropy', 'get_fourier_matrix', 'estimate_flux', 'get_mean_visibilities',
-           'proximal_entropy', 'proximal_operator', 'optimise_fb', 'mem']
+__all__ = [
+    "_get_entropy",
+    "_get_fourier_matrix",
+    "_estimate_flux",
+    "_get_mean_visibilities",
+    "_proximal_entropy",
+    "_proximal_operator",
+    "_optimise_fb",
+    "mem",
+]
 
+from xrayvision.visibility import Visibilities
 
-logger = get_logger(__name__, 'DEBUG')
+logger = get_logger(__name__, "DEBUG")
 
 
-def get_entropy(image, flux):
+def _get_entropy(image, flux):
     r"""
     Return the entropy of an image.
 
     The entropy is defined as
 
     .. math::
 
@@ -39,57 +52,57 @@
     flux :
         Total flux divided by the number of pixels of the image
 
     Returns
     -------
 
     """
-    return np.sum(image*np.log(image/(flux*np.e)))
+    return np.sum(image * np.log(image / (flux * np.e)))
 
 
-def get_fourier_matrix(vis, shape=[64, 64]*apu.pix, pixel_size=[4.0312500, 4.0312500]*apu.arcsec):
+def _get_fourier_matrix(vis, shape=(64, 64) * apu.pix, pixel_size=(4.0312500, 4.0312500) * apu.arcsec):
     r"""
     Return the complex Fourier matrix used to compute the value of the visibilities.
 
     Generate the complex Fourier matrix :math:`Hv` used to compute the value of the
     visibilities. If :math:`\vec{x}` is the vectorised image, then
     :math:`v = \mathbf{\mathit{Hv}} \vec{x}` is the vector containing the complex visibilities
 
     Parameters
     ----------
     vis :
-        Visibly object containg u, v sampling
+        Visibly object containing u, v sampling
     shape :
         Shape of the images
     pixel_size
         Size of the pixels
 
     Returns
     -------
     The complex Fourier matrix
     """
-    m, n = shape.to_value('pix')
-    y = generate_xy(m, 0 * apu.arcsec, pixel_size[1])
-    x = generate_xy(n, 0 * apu.arcsec, pixel_size[0])
-    x, y = np.meshgrid(x, y)
+    m, n = shape.to("pix")
+    y = generate_xy(m, phase_center=0 * apu.arcsec, pixel_size=pixel_size[1])
+    x = generate_xy(n, phase_center=0 * apu.arcsec, pixel_size=pixel_size[0])
+    x, y = np.meshgrid(x, y, indexing="ij")
     uv = np.vstack([vis.u, vis.v])
     # Check apu are correct for exp need to be dimensionless and then remove apu for speed
-    if (vis.u * x[0, 0]).unit == apu.dimensionless_unscaled and \
-            (vis.v * y[0, 0]).unit == apu.dimensionless_unscaled:
+    if (vis.u * x[0, 0]).unit == apu.dimensionless_unscaled and (vis.v * y[0, 0]).unit == apu.dimensionless_unscaled:
         uv = uv.value
         x = x.value
         y = y.value
 
-        Hv = np.exp(1j * 2 * np.pi * (x[..., np.newaxis] * uv[np.newaxis, 0, :]
-                                      + y[..., np.newaxis] * uv[np.newaxis, 1, :]))
+        Hv = np.exp(
+            1j * 2 * np.pi * (x[..., np.newaxis] * uv[np.newaxis, 0, :] + y[..., np.newaxis] * uv[np.newaxis, 1, :])
+        )
 
-        return Hv * pixel_size[0] * pixel_size[1]
+        return Hv * pixel_size[0].value * pixel_size[1].value
 
 
-def estimate_flux(vis, shape, pixel, maxiter=1000, tol=1e-3):
+def _estimate_flux(vis, shape, pixel, maxiter=1000, tol=1e-3):
     r"""
     Estimate the total flux in the image by solving an optimisation problem.
 
     This function estimates the total flux of an event by solving the problem
 
     .. math::
 
@@ -113,41 +126,43 @@
     maxiter : int
         Maximum number of iterations
     tol :
         Tolerance at which to stop
 
     Returns
     -------
-    Esimated total flux
+    Estimated total flux
 
     """
 
     Hv, Lip, Visib = _prepare_for_optimise(pixel, shape, vis)
 
     # PROJECTED LANDWEBER
     # should have same apu as image ct/ keV cm s arcsec**2
-    x = np.zeros(shape.to_value('pix').astype(int)).flatten()
+    x = np.zeros(shape.to_value("pix").astype(int)).flatten()
 
     for i in range(maxiter):
         x_old = x[:]
 
         # GRADIENT STEP
-        grad = 2. * np.matmul((np.matmul(Hv,  x).value - Visib).T, Hv)
-        y = x - 1. / Lip * grad
+        grad = 2.0 * np.matmul((np.matmul(Hv, x).value - Visib).T, Hv)
+        y = x - 1.0 / Lip * grad
 
         # PROJECTION ON THE POSITIVE ORTHANT
         x = y.clip(min=0.0)
         tmp = x[:]
         Hvx = np.matmul(Hv, tmp)
 
         diff_V = Hvx - Visib
-        chi2 = (diff_V ** 2.).sum()
+        chi2 = (diff_V**2.0).sum()
 
-        logger.info(f'Iter: {i}, Chi2: {chi2}')
-        if np.sqrt(((x - x_old) ** 2.).sum()) < tol * np.sqrt((x_old ** 2.).sum()):
+        if i % 25 == 0:
+            logger.info(f"Iter: {i}, Chi2: {chi2}")
+
+        if np.sqrt(((x - x_old) ** 2.0).sum()) < tol * np.sqrt((x_old**2.0).sum()):
             break
 
     return x.sum() * pixel[0] * pixel[1]
 
 
 def _prepare_for_optimise(pixel, shape, vis):
     r"""
@@ -166,46 +181,50 @@
         Size of pixels
 
 
     Returns
     -------
 
     """
-    Hv = get_fourier_matrix(vis, shape, pixel)
+    Hv = _get_fourier_matrix(vis, shape, pixel)
     # Division of real and imaginary part of the matrix 'Hv'
     ReHv = np.real(Hv)
     ImHv = np.imag(Hv)
     # 'Hv' is composed by the union of its real and imaginary part
     Hv = np.concatenate([ReHv, ImHv], axis=-1)
     # Division of real and imaginary part of the visibilities
-    ReV = np.real(vis.vis)
-    ImV = np.imag(vis.vis)
+    ReV = np.real(vis.visibilities)
+    ImV = np.imag(vis.visibilities)
     # 'Visib' is composed by the real and imaginary part of the visibilities
     Visib = np.concatenate([ReV, ImV], axis=-1)
     # Standard deviation of the real and imaginary part of the visibilities
-    sigma_Re = vis.amplitude_error
-    sigma_Im = vis.amplitude_error
+    if vis.amplitude_uncertainty is None:
+        sigma_Re = np.ones_like(ReV)
+        sigma_Im = np.ones_like(ImV)
+    else:
+        sigma_Re = vis.amplitude_uncertainty
+        sigma_Im = vis.amplitude_uncertainty
     # 'sigma': standard deviation of the data contained in 'Visib'
     sigma = np.concatenate([sigma_Re, sigma_Im], axis=-1)
     # RESCALING of 'Hv' AND 'Visib'(NEEDED FOR COMPUTING THE VALUE OF THE \chi ** 2; FUNCTION)
     # The vector 'Visib' and every column of 'Hv' are divided by 'sigma'
     Visib = Visib / sigma
-    ones = np.ones(shape.to_value('pix').astype(int))
+    ones = np.ones(shape.to_value("pix").astype(int))
     sigma1 = sigma * ones[..., np.newaxis]
     Hv = Hv / sigma1
     # COMPUTATION OF THE LIPSCHITZ CONSTANT; 'Lip' OF THE GRADIENT OF  THE \chi ** 2
     # FUNCTION (NEEDED TO GUARANTEE THE CONVERGENCE OF THE ALGORITHM)
     Hv = Hv.transpose(2, 0, 1).reshape(Hv.shape[2], -1)
     HvHvT = np.matmul(Hv, Hv.T)
     # TODO magic number
     Lip = 2.1 * norm(HvHvT, 2)
     return Hv, Lip, Visib
 
 
-def get_mean_visibilities(vis, shape, pixel):
+def _get_mean_visibilities(vis, shape, pixel):
     r"""
     Return the mean visibilities sampling the same call in the discretisation of the (u,v) plane.
 
     Parameters
     ----------
     vis :
         Input visibilities
@@ -215,80 +234,85 @@
         Size of pixels
 
     Returns
     -------
     Mean Visibilities
     """
 
+    if vis.amplitude_uncertainty is None:
+        amplitude_uncertainty = np.ones_like(vis.visibilities)
+    else:
+        amplitude_uncertainty = vis.amplitude_uncertainty
+
     imsize2 = shape[0] / 2
-    pixel_size = 1/(shape[0]*pixel[0])
+    pixel_size = 1 / (shape[0] * pixel[0])
 
     iu = vis.u / pixel_size
     iv = vis.v / pixel_size
     ru = np.around(iu)
     rv = np.around(iv)
 
     # index of the u coordinates of the sampling frequencies in the discretisation of the u axis
-    ru = ru + imsize2
+    ru = ru * apu.pix + imsize2.to(apu.pix)
     # index of the v coordinates of the sampling frequencies in the discretisation of the v axis
-    rv = rv + imsize2
+    rv = rv * apu.pix + imsize2.to(apu.pix)
 
     # matrix that represents the discretization of the (u,v)-plane
-    iuarr = np.zeros(shape.to_value('pixel').astype(int))
+    iuarr = np.zeros(shape.to_value("pixel").astype(int))
 
     count = 0
     n_vis = vis.u.shape[0]
     u = np.zeros(n_vis) * (1 / apu.arcsec)
     v = np.zeros(n_vis) * (1 / apu.arcsec)
     den = np.zeros(n_vis)
-    weights = np.zeros_like(vis.amplitude_error**2)
-    visib = np.zeros_like(vis.vis)
+    weights = np.ones_like(vis.visibilities**2)
+    visib = np.zeros_like(vis.visibilities)
     for ip in range(n_vis):
         # what about 0.5 pix offset
-        i = ru[ip].to_value('pix').astype(int)
-        j = rv[ip].to_value('pix').astype(int)
+        i = ru[ip].to_value("pix").astype(int)
+        j = rv[ip].to_value("pix").astype(int)
         # (i, j) is the position of the spatial frequency in
         # the discretization of the (u,v)-plane 'iuarr'
-        if iuarr[i, j] == 0.:
+        if iuarr[i, j] == 0.0:
             u[count] = vis.u[ip]
             v[count] = vis.v[ip]
             # we save in 'u' and 'v' the u and v coordinates of the first frequency that corresponds
             # to the position (i, j) of the discretization of the (u,v)-plane 'iuarr'
 
-            visib[count] = vis.vis[ip]
-            weights[count] = vis.amplitude_error[ip]**2.
-            den[count] = 1.
+            visib[count] = vis.visibilities[ip]
+            weights[count] = amplitude_uncertainty[ip] ** 2.0
+            den[count] = 1.0
             iuarr[i, j] = count
 
             count += 1
         else:
             # Save the sum of the visibilities that correspond to the same position (i, j)
-            visib[iuarr[i, j].astype(int)] += vis.vis[ip]
+            visib[iuarr[i, j].astype(int)] += vis.visibilities[ip]
             # Save the number of the visibilities that correspond to the same position (i, j)
-            den[iuarr[i, j].astype(int)] += 1.
+            den[iuarr[i, j].astype(int)] += 1.0
             # Save the sum of the variances of the amplitudes of the visibilities that
             # correspond to the same position (i, j)
-            weights[iuarr[i, j].astype(int)] += vis.amplitude_error[ip]**2
+            weights[iuarr[i, j].astype(int)] += amplitude_uncertainty[ip] ** 2
 
     u = u[:count]
     v = v[:count]
     visib = visib[:count]
     den = den[:count]
 
     # computation of the mean value of the visibilities that correspond to the same
     # position in the discretization of the (u,v)-plane
-    visib = visib/den
+    visib = visib / den
     # computation of the mean value of the standard deviation of the visibilities that
     # correspond to the same position in the discretization of the (u,v)-plane
-    weights = np.sqrt(weights[:count])/den
+    weights = np.sqrt(weights[:count]) / den
 
-    return SimpleNamespace(u=u, v=v, vis=visib, amplitude_error=weights)
+    return SimpleNamespace(u=u, v=v, visibilities=visib, amplitude_uncertainty=weights)
 
 
-def proximal_entropy(y, m, lamba, Lip, tol=10**-10):
+def _proximal_entropy(y, m, lamba, Lip, tol=10**-10):
     r"""
     This function computes the value of the proximity operator of the entropy function subject to
     positivity constraint, i.e. it solves the problem
 
                  argmin_x 1/2*|| y-x ||^2 + \lambda/Lip * H(x)
                  subject to x >= 0
 
@@ -305,32 +329,32 @@
 
     Returns
     -------
 
     """
     # INITIALIZATION OF THE BISECTION METHOD
     # TODO where does this number come from
-    a = np.full_like(y, 1e-24*y.unit)
+    a = np.full_like(y, 1e-24 * y.unit)
     b = np.where(y > m, y, m)
 
-    while np.max(b - a) > tol*y.unit:
+    while np.max(b - a) > tol * y.unit:
         c = (a + b) / 2
         f_c = c - y + lamba / Lip * np.log(c / m)
 
         tmp1 = f_c <= 0
         tmp2 = f_c >= 0
 
         a[tmp1] = c[tmp1]
         b[tmp2] = c[tmp2]
 
     c = (a + b) / 2
     return c
 
 
-def proximal_operator(z, f, m, lamb, Lip, niter=250):
+def _proximal_operator(z, f, m, lamb, Lip, niter=250):
     r"""
     Computes the value of the proximity operator of the entropy function subject to
     positivity constraint and flux constraint by means of a Dykstra-like proximal algorithm
     (see Combettes, Pesquet, "Proximal Splitting Methods in Signal Processing", (2011)).
     The problem to solve is:
 
                        argmin_x 1/2*|| x - y ||^2 + \lambda/Lip * H(x)
@@ -353,31 +377,30 @@
 
     # INITIALIZATION OF THE DYKSTRA - LIKE SPLITTING
     x = z[:]
     p = np.zeros_like(x)
     q = np.zeros_like(x)
 
     for i in range(niter):
-
         tmp = x + p
         # Projection on the hyperplane that represents the flux constraint
         y = tmp + (f - tmp.sum()) / tmp.size
         p = x + p - y
 
-        x = proximal_entropy(y + q, m, lamb, Lip)
+        x = _proximal_entropy(y + q, m, lamb, Lip)
 
         if np.abs(x.sum() - f) <= 0.01 * f:
             break
 
         q = y + q - x
 
     return x, i
 
 
-def optimise_fb(Hv, Visib, Lip, flux, lambd, shape, pixel, maxiter, tol):
+def _optimise_fb(Hv, Visib, Lip, flux, lambd, shape, pixel, maxiter, tol):
     r"""
     Solve the optimization problem using a forward-backward splitting algorithm
 
     .. math::
 
         \underset{x}{\mathrm{argmin}} \quad \chi^{2}(x) + \lambda H(x)
 
@@ -415,59 +438,57 @@
     -------
     MEM Image
     """
 
     # 'f': value of the total flux of the image (taking into account the area of the pixel)
     f = flux / (pixel[0] * pixel[1])
     # 'm': total flux divided by the number of pixels of the image
-    m = f / np.prod(shape.to_value('pix'))
+    m = f / np.prod(shape.to_value("pix"))
 
     # INITIALIZATION
 
     # 'x': constant image with total flux equal to 'f'
-    x = np.ones(shape.to_value('pix').astype(int)) + 1.
+    x = np.ones(shape.to_value("pix").astype(int)) + 1.0
     x = x / x.sum() * f
     z = x
     t = 1.0
 
     # COMPUTATION OF THE OBJECTIVE FUNCTION 'J'
 
     tmp = x.flatten()[:]
     Hvx = np.matmul(Hv, tmp)
-    f_R = get_entropy(x, m)
+    f_R = _get_entropy(x, m)
 
     diff_V = Hvx - Visib
     f_0 = (diff_V**2).sum()
     J = f_0 + lambd * f_R
 
     n_iterations = 0  # number of iterations done in the proximal steps to update the minimizer
     for i in range(maxiter):
-
         J_old = np.copy(J)
         x_old = np.copy(x)
         t_old = np.copy(t)
 
         # GRADIENT STEP
-        grad = 2 * np.matmul((np.matmul(Hv, z.flatten()) - Visib),
-                             Hv).reshape(*shape.to_value('pix').astype(int))
+        grad = 2 * np.matmul((np.matmul(Hv, z.flatten()) - Visib), Hv).reshape(*shape.to_value("pix").astype(int))
         y = z - 1 / Lip * grad
 
         # PROXIMAL STEP
-        p, pi = proximal_operator(y, f, m, lambd, Lip)
+        p, pi = _proximal_operator(y, f, m, lambd, Lip)
 
         # COMPUTATION OF THE OBJECTIVE FUNCTION 'Jp' IN 'p'
         tmp = p.flatten()
         Hvp = np.matmul(Hv, tmp)
-        f_Rp = get_entropy(p, m)
+        f_Rp = _get_entropy(p, m)
 
         diff_Vp = Hvp - Visib
         f_0 = (diff_Vp**2).sum()
         Jp = f_0 + lambd * f_Rp
 
-        # CHEK OF THE MONOTONICITY
+        # CHECK OF THE MONOTONICITY
         # we update 'x' only if 'Jp' is less than or equal to 'J_old'
         check = True
         if Jp > J_old:
             x[:] = x_old
             J = J_old
             check = False
             n_iterations += pi
@@ -477,21 +498,22 @@
             n_iterations = 0
 
         if n_iterations >= 500:
             break  # if the number of iterations done to update 'x' is too big, then break
 
         # ACCELERATION
 
-        t = (1 + np.sqrt(1. + 4. * t_old ** 2.)) / 2.
-        tau = (t_old - 1.) / t
+        t = (1 + np.sqrt(1.0 + 4.0 * t_old**2.0)) / 2.0
+        tau = (t_old - 1.0) / t
         z = x + tau * (x - x_old) + (t_old / t) * (p - x)
 
-        logger.info(f'Iter: {i}, Obj function: {J}')
+        if i % 25 == 0:
+            logger.info(f"Iter: {i}, Obj function: {J}")
 
-        if check and (np.sqrt(((x - x_old)**2.).sum()) < tol * np.sqrt((x_old**2).sum())):
+        if check and (np.sqrt(((x - x_old) ** 2.0).sum()) < tol * np.sqrt((x_old**2).sum())):
             break
 
     return x_old
 
 
 def resistant_mean(data, sigma_cut):
     r"""
@@ -521,117 +543,92 @@
     median_abs_deviation = np.median(abs_deviation) / mad_scale
     if median_abs_deviation < mad_lim:
         median_abs_deviation = np.mean(abs_deviation) / mad_scale2
 
     cutoff = sigma_cut * median_abs_deviation
     good_index = np.where(abs_deviation <= cutoff)
     if not good_index[0].size > 0:
-        raise ValueError('Unable to compute mean')
+        raise ValueError("Unable to compute mean")
 
     good_points = data[good_index]
     mean = np.mean(good_points)
-    sigma = np.sqrt((((good_points - mean)**2).sum()) / good_points.size)
+    sigma = np.sqrt((((good_points - mean) ** 2).sum()) / good_points.size)
 
     # Compensate Sigma for truncation (formula by HF):
     if sigma_cut <= 4.50:
         sigma = sigma / np.polyval(sig_coeff[::-1], sigma_cut)
 
     cutoff = sigma_cut * sigma
 
     good_index = np.where(abs_deviation <= cutoff)
     good_points = data[good_index]
 
     mean = np.mean(good_points)
-    sigma = np.sqrt((((good_points - mean)**2).sum()) / good_points.size)
+    sigma = np.sqrt((((good_points - mean) ** 2).sum()) / good_points.size)
 
     if sigma_cut <= 4.50:
         sigma = sigma / np.polyval(sig_coeff[::-1], sigma_cut)
 
     # Now the standard deviation of the mean:
     sigma = sigma / np.sqrt(good_points.size - 1)
 
     return mean, sigma
 
 
-def get_percent_lambda(vis):
+@apu.quantity_input
+def mem(
+    vis: Visibilities,
+    shape: Quantity[apu.pix],
+    pixel_size: Quantity[apu.arcsec / apu.pix],
+    *,
+    percent_lambda: Optional[Quantity[apu.percent]] = 0.02 * apu.percent,
+    maxiter: int = 1000,
+    tol: float = 1e-3,
+    map: bool = True,
+) -> Union[Quantity, NDArray[np.float64]]:
     r"""
-    Return 'percent_lambda' use with MEM
-
-    Calculate the signal-to-noise ratio (SNR) for the given visibility bag by trying to use the
-    coarser sub-collimators adding finer ones until there are at least 2 visiblities, then use
-    resistant mean of of abs(obsvis) / sigamp
-
-    Parameters
-    ----------
-    vis
-
-    Returns
-    -------
-
-    """
-    # Loop through ISCs starting with 3-10, but if we don't have at least 2 vis, lower isc_min to
-    # include next one down, etc.
-
-    # TODO this start at 3 not 10?
-    isc_min = 3
-    nbig = 0
-    isc_sizes = np.array([float(s[:-1]) for s in vis.label])
-    while isc_min >= 0 and nbig < 2:
-        ibig = np.argwhere(isc_sizes >= isc_min)
-        isc_min = isc_min - 1
-
-    # If still don't have at least 2 vis, return -1, otherwise calculate mean
-    # (but reject points > sigma away from mean)
-    if ibig.size < 2:
-        snr_value = -1
-    else:
-        snr_value, _ = resistant_mean(
-            (np.abs(vis.vis[ibig])/vis.amplitude_error[ibig]).flatten(), 3)
-
-    # TODO magic numbers
-    percent_lambda = 2 / (snr_value**2 + 90)
-
-    return percent_lambda
-
-
-def mem(vis, percent_lambda=None, shape=None, pixel=None, maxiter=1000, tol=1e-3):
-    r"""
-    Maximum Entropy Method for visibility based image reconstruction
+    Maximum Entropy Method visibility based image reconstruction
 
     Parameters
     ----------
     vis :
         Input Visibilities
-    percent_lambda
-        value used to compute the regularization parameter as a percentage of a maximum value
-        automatically overestimated by the algorithm. Must be in the range [0.0001,0.2]
-    shape
+    shape :
         Image size
-    pixel
+    pixel_size :
         Pixel size
-    maxiter : int
-        Maximum number of iterations of the optimization loop
+    percent_lambda
+        Value used to compute the regularization parameter as a percentage of a maximum value
+        automatically overestimated by the algorithm. Must be in the range [0.0001,0.2]
+    maxiter :
+        Maximum number of iterations of the optimisation loop
     tol : float
         tolerance value used in the stopping rule ( || x - x_old || <= tol || x_old ||)
-
+    map :
+        Return a sunpy map or bare array
     Returns
     -------
 
     """
-    total_flux = estimate_flux(vis, shape, pixel)
-    if percent_lambda is None:
-        percent_lambda = get_percent_lambda(vis)
+    total_flux = _estimate_flux(vis, shape, pixel_size)
 
-    mean_vis = get_mean_visibilities(vis, shape, pixel)
-    Hv, Lip, Visib = _prepare_for_optimise(pixel, shape, mean_vis)
+    mean_vis = _get_mean_visibilities(vis, shape, pixel_size)
+    Hv, Lip, Visib = _prepare_for_optimise(pixel_size, shape, mean_vis)
 
     # should have same apu as image ct/ keV cm s arcsec**2
-    x = np.zeros(shape.to_value('pix').astype(int)).flatten()
+    x = np.zeros(shape.to_value("pix").astype(int)).flatten()
 
     # COMPUTATION OF THE; OBJECTIVE; FUNCTION; 'chi2'
-    x = x + total_flux/(shape[0]*shape[1]*pixel[0]*pixel[1]).value
+    x = x + total_flux / (shape[0] * shape[1] * pixel_size[0] * pixel_size[1]).value
     Hvx = np.matmul(Hv, x)
 
-    lambd = 2 * np.abs((np.matmul((Hvx.value - Visib), Hv))).max()*percent_lambda
+    lambd = 2 * np.abs(np.matmul((Hvx.value - Visib), Hv)).max() * percent_lambda
+
+    im = _optimise_fb(Hv, Visib, Lip, total_flux, lambd, shape, pixel_size, maxiter, tol)
+
+    # This is needed to match IDL output
+    # im = np.rot90(im, -1)
 
-    im = optimise_fb(Hv, Visib, Lip, total_flux, lambd, shape, pixel, maxiter, tol)
+    if map:
+        header = generate_header(vis, shape=shape, pixel_size=pixel_size)
+        return Map((im, header))
     return im
```

### Comparing `xrayvisim-0.1.0rc1/xrayvision/tests/test_mem.py` & `xrayvisim-0.2.0rc1/xrayvision/tests/test_mem.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-import numpy as np
-
 import astropy.units as u
+import numpy as np
 from astropy.convolution.kernels import Gaussian2DKernel
+from numpy.testing import assert_allclose
 
 from xrayvision.imaging import image_to_vis
 from xrayvision.mem import mem, resistant_mean
 
 
 def test_resistant_mean():
-    x = np.array([-0.61566182, -0.3362035, -0.73589487, -0.13014149, -0.91786147,
-                  -0.02883366, 1.37688696, -0.22389746, -1.37010835, 0.21693273,
-                  -0.82412723, 0.56856134, -0.36824209, -0.65785301, 0.10807291,
-                  -0.16730037, -0.30308355, 0.12605051, -1.14017418, -1.36991364,
-                  -0.45275646, 0.31636448, -0.1316372, -1.19194891, 0.58557167,
-                  1.18596057, 0.01104923, 0.61225975, 0.133178, -0.37117463,
-                  -0.14882964, -0.59864443, -0.49450362, 0.83710754, -0.51270022,
-                  0.87380341, 0.52904637, 0.37973441, 0.34061863, -0.10493781,
-                  0.86224542, -0.84283578, -0.35069229, -1.29952663, 0.39678443,
-                  -0.94903521, 0.008999, 0.52126955, 0.24956007, -2.18242896,
-                  0.15877853, -0.99771069, -0.14426402, 1.48957386, -0.68078661,
-                  1.07328579, -2.57370777, 2.26526367, 1.20964125, -1.26854227,
-                  0.20587741, -0.12066582, -0.78971368, -0.36412889, 0.12816666,
-                  -0.50670234, 1.19987195, 1.29270178, 1.03906824, 1.41541003,
-                  0.15639539, 0.92386204, -2.62109581, 0.68909503, -0.34981646,
-                  0.93647975, -0.32268089, 1.67739013, -0.29216895, -2.30162528,
-                  -0.89649313, 0.37481482, -2.18661087, 0.2190169, -0.30387412,
-                  0.84001059, -0.25604226, 0.50463104, -1.25674997, 0.66314647,
-                  -0.0073464, -0.59719724, 0.64527612, 1.25720287, 0.5032624,
-                  0.07773715, 0.29573575, -0.80567372, -1.92934995, -2.0358119])
+    # fmt: off
+    x = np.array(
+        [-0.61566182, -0.3362035, -0.73589487, -0.13014149, -0.91786147, -0.02883366, 1.37688696, -0.22389746,
+         -1.37010835, 0.21693273, -0.82412723, 0.56856134, -0.36824209, -0.65785301, 0.10807291, -0.16730037,
+         -0.30308355, 0.12605051, -1.14017418, -1.36991364, -0.45275646, 0.31636448, -0.1316372, -1.19194891,
+         0.58557167, 1.18596057, 0.01104923, 0.61225975, 0.133178, -0.37117463, -0.14882964, -0.59864443, -0.49450362,
+         0.83710754, -0.51270022, 0.87380341, 0.52904637, 0.37973441, 0.34061863, -0.10493781, 0.86224542, -0.84283578,
+         -0.35069229, -1.29952663, 0.39678443, -0.94903521, 0.008999, 0.52126955, 0.24956007, -2.18242896, 0.15877853,
+         -0.99771069, -0.14426402, 1.48957386, -0.68078661, 1.07328579, -2.57370777, 2.26526367, 1.20964125,
+         -1.26854227, 0.20587741, -0.12066582, -0.78971368, -0.36412889, 0.12816666, -0.50670234, 1.19987195,
+         1.29270178, 1.03906824, 1.41541003, 0.15639539, 0.92386204, -2.62109581, 0.68909503, -0.34981646, 0.93647975,
+         -0.32268089, 1.67739013, -0.29216895, -2.30162528, -0.89649313, 0.37481482, -2.18661087, 0.2190169,
+         -0.30387412, 0.84001059, -0.25604226, 0.50463104, -1.25674997, 0.66314647, -0.0073464, -0.59719724, 0.64527612,
+         1.25720287, 0.5032624, 0.07773715, 0.29573575, -0.80567372, -1.92934995, -2.0358119,]
+    )
+    # fmt: on
     rmean, rsigma = resistant_mean(x, 3)
     # values for IDL routine "RESISTANT_Mean, xx, 3, rmean, rsig, num"
     assert np.allclose(rmean, -0.10947954)
     assert np.allclose(rsigma, 0.096651256)
 
 
 def test_mem():
@@ -41,29 +37,28 @@
     # data[13,13] = 10.0
     # data[12:14,12:14] = 10.0/4.0
 
     # half_log_space = np.logspace(np.log10(0.03030303), np.log10(0.48484848), 10)
     # RHESSI like spatial res
     half_log_space = 1 / 10 ** np.logspace(np.log10(0.665), np.log10(2.56), 10)[::-1]
 
-    theta = np.linspace(-1*np.pi/2, np.pi/2, 33)[1:-1]
+    theta = np.linspace(-1 * np.pi / 2, np.pi / 2, 33)[1:-1]
     theta = theta[np.newaxis, :]
     theta = np.repeat(theta, 5, axis=0)
 
     # Since the source is only 3 * 2 = 6 arecsec don't use the finest resolutions
     r = half_log_space[:5]
     r = r[:, np.newaxis]
     r = np.repeat(r, 31, axis=1)
 
     x = r * np.sin(theta)
     y = r * np.cos(theta)
 
     sub_uv = np.vstack([x.flatten(), y.flatten()]) / u.arcsec
     # sub_uv = np.hstack([sub_uv, np.zeros((2, 1))]) / u.arcsec
 
-    vis = image_to_vis(data, u=sub_uv[0, :], v=sub_uv[1, :], pixel_size=2*u.arcsec)
-    setattr(vis, 'amplitude_error', np.sqrt(np.abs(vis.vis)))
-    setattr(vis, 'label', [str(x) for x in np.sqrt((x**2 + y**2)).flatten()])
-
-    res = mem(vis, percent_lambda=None, shape=(m, n)*u.pix, pixel=[2, 2]*u.arcsec,
-              maxiter=1000, tol=1e-3)
-    np.testing.assert_allclose(res.value - data/4, 0.0, atol=1e-3)
+    vis = image_to_vis(data * u.dimensionless_unscaled, u=sub_uv[0, :], v=sub_uv[1, :], pixel_size=2 * u.arcsec / u.pix)
+    setattr(vis, "amplitude_error", np.sqrt(np.abs(vis.visibilities)))
+    setattr(vis, "label", [str(x) for x in np.sqrt(x**2 + y**2).flatten()])
+
+    res = mem(vis, shape=(m, n) * u.pix, pixel_size=[2, 2] * u.arcsec / u.pix, maxiter=1000, tol=1e-3)
+    assert_allclose(res.data, data, atol=1e-1)
```

### Comparing `xrayvisim-0.1.0rc1/xrayvision/transform.py` & `xrayvisim-0.2.0rc1/xrayvision/transform.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,202 +1,260 @@
 """
 Discrete Fourier Transform (DFT) and Inverse Discrete Fourier Transform (IDFT) related functions.
 
 There are two implementations one a standard DFT `dft` and IDFT `idft` in terms of pixel space, i.e.
-the input has no positional information other than an arbitary 0 origin and a length. The second
+the input has no positional information other than an arbitrary 0 origin and a length. The second
 takes inputs which have positional information `dft_map` and the inverse `idft_map`
 
 """
-import numpy as np
+
+from typing import Union, Optional
 
 import astropy.units as apu
+import numpy as np
+import numpy.typing as npt
+from astropy.units import Quantity
 from astropy.units.core import UnitsError
 
+__all__ = ["generate_xy", "generate_uv", "dft_map", "idft_map"]
+
 
-@apu.quantity_input(center='angle', pixel_size='angle')
-def generate_xy(number_pixels, center=0.0 * apu.arcsec, pixel_size=1.0 * apu.arcsec):
+@apu.quantity_input()
+def generate_xy(
+    number_pixels: Quantity[apu.pix],
+    *,
+    phase_center: Optional[Quantity[apu.arcsec]] = 0.0 * apu.arcsec,
+    pixel_size: Optional[Quantity[apu.arcsec / apu.pix]] = 1.0 * apu.arcsec / apu.pix,
+) -> Quantity[apu.arcsec]:
     """
-    Generate the x or y coordinates given the number of pixels, center and pixel size.
+    Generate the x or y coordinates given the number of pixels, phase_center and pixel size.
 
     Parameters
     ----------
     number_pixels : `int`
         Number of pixels
-    center : `float`, optional
+    phase_center : `float`, optional
         Center coordinates
     pixel_size : `float`, optional
         Size of pixel in physical units (e.g. arcsecs, meters)
 
     Returns
     -------
-    `numpy.array`
+    :
         The generated x, y coordinates
 
     See Also
     --------
-    `generate_uv` : Generates corresponding coordinates but un u, v space
+    generate_uv:
+        Generates corresponding coordinates but in Fourier or u, v space.
 
     Examples
     --------
-    >>> generate_xy(9)
+    >>> import astropy.units as apu
+    >>> generate_xy(9*apu.pix)
     <Quantity [-4., -3., -2., -1.,  0.,  1.,  2.,  3.,  4.] arcsec>
 
-    >>> generate_xy(9, pixel_size=2.5 * apu.arcsec)
-    <Quantity [-10. , -7.5, -5. , -2.5,  0. ,  2.5,  5. ,  7.5, 10. ] arcsec>
+    >>> generate_xy(9*apu.pix, pixel_size=2.5 * apu.arcsec/apu.pix)
+    <Quantity [-10. ,  -7.5,  -5. ,  -2.5,   0. ,   2.5,   5. ,   7.5,  10. ] arcsec>
 
-    >>> generate_xy(9, center=10 * apu.arcsec, pixel_size=2.5 * apu.arcsec)
+    >>> generate_xy(9*apu.pix, phase_center=10 * apu.arcsec, pixel_size=2.5 * apu.arcsec/apu.pix)
     <Quantity [ 0. ,  2.5,  5. ,  7.5, 10. , 12.5, 15. , 17.5, 20. ] arcsec>
 
     """
-    x = (np.arange(number_pixels) - number_pixels / 2 + 0.5) * pixel_size + center
+    x = (
+        np.arange(number_pixels.to_value(apu.pixel)) - (number_pixels.to_value(apu.pix) / 2) + 0.5
+    ) * apu.pix * pixel_size + phase_center
     return x
 
 
-@apu.quantity_input(center='angle', pixel_size='angle')
-def generate_uv(number_pixels, center=0.0 * apu.arcsec, pixel_size=1.0 * apu.arcsec):
+@apu.quantity_input()
+def generate_uv(
+    number_pixels: Quantity[apu.pix],
+    *,
+    phase_center: Optional[Quantity[apu.arcsec]] = 0.0 * apu.arcsec,
+    pixel_size: Optional[Quantity[apu.arcsec / apu.pix]] = 1.0 * apu.arcsec / apu.pix,
+) -> Quantity[1 / apu.arcsec]:
     """
-    Generate the u or v  coordinates given the number of pixels, center and pixel size.
+    Generate the u or v coordinates given the number of pixels, phase_center and pixel size.
 
     Parameters
     ----------
     number_pixels : `int`
         Number of pixels
-    center : `float`, optional
+    phase_center : `float`, optional
         Center coordinates
     pixel_size : `float`, optional
         Size of pixel in physical units (e.g. arcsecs, meters)
 
     Returns
     -------
-    `numpy.array`
-        The generated u, v coordinates
+    :
+        The generated u, v coordinates.
 
     See Also
     --------
-    `generate_xy` : Generates corresponding coordinate but un x, y space
+    generate_xy:
+        Generates corresponding coordinates but in Fourier or u, v space.
 
     Examples
     --------
-    >>> generate_uv(9)
+    >>> import astropy.units as apu
+    >>> generate_uv(9*apu.pix)
     <Quantity [-0.44444444, -0.33333333, -0.22222222, -0.11111111,  0.        ,
                 0.11111111,  0.22222222,  0.33333333,  0.44444444] 1 / arcsec>
 
-    >>> generate_uv(9, pixel_size=2.5 * apu.arcsec)
+    >>> generate_uv(9*apu.pix, pixel_size=2.5 * apu.arcsec/apu.pix)
     <Quantity [-0.17777778, -0.13333333, -0.08888889, -0.04444444,  0.        ,
                 0.04444444,  0.08888889,  0.13333333,  0.17777778] 1 / arcsec>
 
-    >>> generate_uv(9, center=10 * apu.arcsec, pixel_size=2.5 * apu.arcsec)
+    >>> generate_uv(9*apu.pix, phase_center=10 * apu.arcsec, pixel_size=2.5 * apu.arcsec/apu.pix)
     <Quantity [-0.07777778, -0.03333333,  0.01111111,  0.05555556,  0.1       ,
                 0.14444444,  0.18888889,  0.23333333,  0.27777778] 1 / arcsec>
 
     """
-    x = (np.arange(number_pixels) - number_pixels / 2 + 0.5) * (1 / (pixel_size * number_pixels))
-    if center.value != 0.0:
-        x += 1 / center
+    # x = (np.arange(number_pixels) - number_pixels / 2 + 0.5) / (pixel_size * number_pixels)
+
+    x = (np.arange(number_pixels.to_value(apu.pixel)) - (number_pixels.to_value(apu.pix) / 2) + 0.5) / (
+        pixel_size * number_pixels
+    )
+
+    if phase_center.value != 0.0:  # type: ignore
+        x += 1 / phase_center  # type: ignore
     return x
 
 
-@apu.quantity_input(center='angle', pixel_size='angle')
-def dft_map(input_array, *, u, v, center=(0.0, 0.0) * apu.arcsec, pixel_size=(1.0, 1.0) * apu.arcsec):
+@apu.quantity_input()
+def dft_map(
+    input_array: Union[Quantity, npt.NDArray],
+    *,
+    u: Quantity[1 / apu.arcsec],
+    v: Quantity[1 / apu.arcsec],
+    phase_center: Quantity[apu.arcsec] = (0.0, 0.0) * apu.arcsec,
+    pixel_size: Quantity[apu.arcsec / apu.pix] = (1.0, 1.0) * apu.arcsec / apu.pix,
+) -> Union[Quantity, npt.NDArray]:
     r"""
     Discrete Fourier transform in terms of coordinates returning 1-D array complex visibilities.
 
     Parameters
     ----------
-    input_array : `numpy.ndarray`
+    input_array :
         Input array to be transformed should be 2D (m, n)
-    uv : `numpy.array`
-        Array of 2xN u, v coordinates where the visibilities will be evaluated
-    center : `float` (x, y), optional
-        Coordinates of the center of the map e.g. ``(0,0)`` or ``[5.0, -2.0]``
+    u :
+        Array of 2xN u coordinates where the visibilities are evaluated.
+    v :
+        Array of 2xN v coordinates where the visibilities are evaluated.
+    phase_center :
+        Coordinates of the phase_center of the map e.g. ``(0,0)`` or ``[5.0, -2.0]``.
     pixel_size : `float` (dx, dy), optional
-        The pixel size in x and y directions, need not be square e.g. ``(1, 3)``
+        The pixel size need not be square e.g. ``(1, 3)``.
 
     Returns
     -------
-    `numpy.ndarray`
-        Array of N `complex` visibilities evaluated at the u, v coordinates given bu `uv`
+    :
+        Array of N `complex` visibilities evaluated at the given `u`, `v` coordinates.
 
     """
-    m, n = input_array.shape
-
-    y = generate_xy(m, center[1], pixel_size[1])
-    x = generate_xy(n, center[0], pixel_size[0])
+    m, n = input_array.shape * apu.pix
+    x = generate_xy(m, phase_center=phase_center[0], pixel_size=pixel_size[0])  # type: ignore
+    y = generate_xy(n, phase_center=phase_center[1], pixel_size=pixel_size[1])  # type: ignore
 
-    x, y = np.meshgrid(x, y)
+    x, y = np.meshgrid(x, y, indexing="ij")
     uv = np.vstack([u, v])
     # Check units are correct for exp need to be dimensionless and then remove units for speed
-    if (uv[0, :] * x[0, 0]).unit == apu.dimensionless_unscaled and \
-            (uv[1, :] * y[0, 0]).unit == apu.dimensionless_unscaled:
-
-        uv = uv.value
+    if (uv[0, :] * x[0, 0]).unit == apu.dimensionless_unscaled and (
+        uv[1, :] * y[0, 0]
+    ).unit == apu.dimensionless_unscaled:
+        uv = uv.value  # type: ignore
         x = x.value
         y = y.value
 
-        vis = np.sum(input_array[..., np.newaxis] * np.exp(-2j * np.pi * (
-            x[..., np.newaxis] * uv[np.newaxis, 0, :] + y[..., np.newaxis] * uv[np.newaxis, 1, :])),
-            axis=(0, 1))
+        vis = np.sum(
+            input_array[..., np.newaxis]
+            * np.exp(
+                2j * np.pi * (x[..., np.newaxis] * uv[np.newaxis, 0, :] + y[..., np.newaxis] * uv[np.newaxis, 1, :])
+            ),
+            axis=(0, 1),
+        )
 
         return vis
     else:
-        raise UnitsError("Incompatible units on uv {uv.unit} should cancel with xy "
-                         "to leave a dimensionless quantity")
-
-
-@apu.quantity_input(center='angle', pixel_size='angle')
-def idft_map(input_vis, *, u, v, shape, weights=None, center=(0.0, 0.0) * apu.arcsec,
-             pixel_size=(1.0, 1.0) * apu.arcsec):
+        raise UnitsError(
+            "Incompatible units on uv {uv.unit} should cancel with xy " "to leave a dimensionless quantity"
+        )
+
+
+@apu.quantity_input
+def idft_map(
+    input_vis: Union[Quantity, npt.NDArray],
+    *,
+    u: Quantity[1 / apu.arcsec],
+    v: Quantity[1 / apu.arcsec],
+    shape: Quantity[apu.pix],
+    weights: Optional[npt.NDArray] = None,
+    phase_center: Quantity[apu.arcsec] = (0.0, 0.0) * apu.arcsec,
+    pixel_size: Quantity[apu.arcsec / apu.pix] = (1.0, 1.0) * apu.arcsec / apu.pix,
+) -> Union[Quantity, npt.NDArray]:
     r"""
     Inverse discrete Fourier transform in terms of coordinates returning a 2D real array or image.
 
     Parameters
     ----------
-    uv : `numpy.ndarray`
-        Array of 2xN u, v coordinates corresponding to the input visibilities in `input_vis`
-    input_vis : `numpy.ndarray`
-        Array of N `complex` input visibilities
-    shape : `float` (m,n)
-        The shape of the output array to create
-    weights : `numpy.ndarray`
-        Array of weights for visibilities
-    center : `float` (x, y), optional
-        Coordinates of the center of the map e.g. ``(0,0)`` or ``[5.0, -2.0]``
-    pixel_size : `float` (dx, dy), optional
-        The pixel size in x and y directions, need not be square e.g. ``(1, 3)``
+    input_vis :
+        Input array of N complex visibilities to be transformed to a 2D array.
+    u :
+        Array of N u coordinates corresponding to the input visibilities in `input_vis`
+    v :
+        Array of N v coordinates corresponding to the input visibilities in `input_vis`
+    shape :
+        The shape of the output array to create.
+    weights :
+        Array of weights for visibilities.
+    phase_center :
+        Coordinates of the phase_center of the map e.g. ``(0,0)`` or ``[5.0, -2.0]``.
+    pixel_size :
+        The pixel size this need not be square e.g. ``(1, 3)``.
 
     Returns
     -------
-    `numpy.ndarray`
-        The complex visibilities evaluated at the u, v coordinates
+    :
+        2D image obtained from the visibilities evaluated at the given `u`, `v` coordinates.
 
     """
     m, n = shape
-    y = generate_xy(m, center[1], pixel_size[1])
-    x = generate_xy(n, center[0], pixel_size[0])
-    x, y = np.meshgrid(x, y)
+    x = generate_xy(m, phase_center=phase_center[0], pixel_size=pixel_size[0])  # type: ignore
+    y = generate_xy(n, phase_center=phase_center[1], pixel_size=pixel_size[1])  # type: ignore
+
+    x, y = np.meshgrid(x, y, indexing="ij")
 
     if weights is None:
         weights = np.ones(input_vis.shape)
     uv = np.vstack([u, v])
     # Check units are correct for exp need to be dimensionless and then remove units for speed
-    if (uv[0, :] * x[0, 0]).unit == apu.dimensionless_unscaled and \
-            (uv[1, :] * y[0, 0]).unit == apu.dimensionless_unscaled:
-
-        uv = uv.value
+    if (uv[0, :] * x[0, 0]).unit == apu.dimensionless_unscaled and (
+        uv[1, :] * y[0, 0]
+    ).unit == apu.dimensionless_unscaled:
+        uv = uv.value  # type: ignore
         x = x.value
         y = y.value
 
-        image = np.sum(input_vis * weights * np.exp(2j * np.pi * (
-            x[..., np.newaxis] * uv[np.newaxis, 0, :] + y[..., np.newaxis] * uv[np.newaxis, 1, :])),
-            axis=2)
+        image = np.sum(
+            input_vis
+            * weights
+            * np.exp(
+                -2j * np.pi * (x[..., np.newaxis] * uv[np.newaxis, 0, :] + y[..., np.newaxis] * uv[np.newaxis, 1, :])
+            ),
+            axis=2,
+        )
 
         return np.real(image)
     else:
-        raise UnitsError("Incompatible units on uv {uv.unit} should cancel with xy "
-                         "to leave a dimensionless quantity")
+        raise UnitsError(
+            "Incompatible units on uv {uv.unit} should cancel with xy " "to leave a dimensionless quantity"
+        )
+
 
 # def dft(im, uv):
 #     """
 #     Discrete Fourier transform of the input array or image calculated at the given u, v
 #     coordinates
 #
 #     Loops over a list of u, v coordinates rather than looping over u and v separately
@@ -208,15 +266,15 @@
 #
 #     uv : `numpy.ndarray`
 #         Array of u, v coordinates where visibilities will be calculated
 #
 #     Returns
 #     -------
 #     vis : `numpy.ndarray`
-#         The complex visibilities evaluated at the u, v coordinates given bu `uv`
+#         The complex visibilities evaluated at the u, v coordinates given by `uv`
 #
 #     """
 #     m, n = im.shape
 #     size = im.size
 #     vis = np.zeros(size, dtype=complex)
 #     xy = np.mgrid[0:m, 0:n].reshape(2, size)
 #     for i in range(uv.shape[1]):
```

### Comparing `xrayvisim-0.1.0rc1/xrayvision/utils.py` & `xrayvisim-0.2.0rc1/xrayvision/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
+from typing import Union, Optional
 
 
-def get_logger(name, level=logging.WARNING):
+def get_logger(name: str, level: Optional[Union[int, str]] = logging.WARNING) -> logging.Logger:
     """
     Return a configured logger instance.
 
     Parameters
     ----------
     name : `str`
         Name of the logger
@@ -14,15 +15,16 @@
 
     Returns
     -------
     `logging.Logger`
         Configured logger
     """
     logger = logging.getLogger(name)
-    logger.setLevel(level)
+    logger.setLevel(level)  # type: ignore
     handler = logging.StreamHandler()
-    handler.setLevel(level)
-    formatter = logging.Formatter('%(asctime)s %(levelname)s %(name)s %(lineno)s: %(message)s',
-                                  datefmt='%Y-%m-%dT%H:%M:%SZ')
+    handler.setLevel(level)  # type: ignore
+    formatter = logging.Formatter(
+        "%(asctime)s %(levelname)s %(name)s %(lineno)s: %(message)s", datefmt="%Y-%m-%dT%H:%M:%SZ"
+    )
     handler.setFormatter(formatter)
     logger.addHandler(handler)
     return logger
```

