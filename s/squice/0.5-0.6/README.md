# Comparing `tmp/squice-0.5.tar.gz` & `tmp/squice-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squice-0.5.tar", last modified: Mon May 27 17:25:22 2024, max compression
+gzip compressed data, was "squice-0.6.tar", last modified: Sun Jun  2 15:58:41 2024, max compression
```

## Comparing `squice-0.5.tar` & `squice-0.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.317177 squice-0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.305177 squice-0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.309177 squice-0.5/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-27 17:25:16.000000 squice-0.5/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.309177 squice-0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/lint_style.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/pydoctor.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/pytest_app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/pytest_lib.yml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-27 17:25:16.000000 squice-0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-27 17:25:16.000000 squice-0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-27 17:25:16.000000 squice-0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-27 17:25:16.000000 squice-0.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-27 17:25:16.000000 squice-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-27 17:25:22.317177 squice-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-27 17:25:16.000000 squice-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.309177 squice-0.5/app/
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-27 17:25:16.000000 squice-0.5/app/home.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.309177 squice-0.5/app/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-05-27 17:25:16.000000 squice-0.5/app/pages/2_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 17:25:16.000000 squice-0.5/app/pages/4_about.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.309177 squice-0.5/app/static/
--rw-r--r--   0 runner    (1001) docker     (127)   183520 2024-05-27 17:25:16.000000 squice-0.5/app/static/squice.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.305177 squice-0.5/app/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/app/tests/use_cases/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 17:25:16.000000 squice-0.5/app/tests/use_cases/test_add_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-27 17:25:16.000000 squice-0.5/citation.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-27 17:25:16.000000 squice-0.5/dev.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-27 17:25:16.000000 squice-0.5/docs/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-27 17:25:16.000000 squice-0.5/matrix (1).npy
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-27 17:25:16.000000 squice-0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-27 17:25:16.000000 squice-0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 17:25:16.000000 squice-0.5/requirements_lib.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-27 17:25:22.317177 squice-0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 17:25:16.000000 squice-0.5/src/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/src/squice/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-27 17:25:16.000000 squice-0.5/src/squice/BinaryFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-27 17:25:16.000000 squice-0.5/src/squice/DataLoaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-27 17:25:16.000000 squice-0.5/src/squice/GridMaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-27 17:25:16.000000 squice-0.5/src/squice/Matrix3d.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/squice/ModulePredict.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 17:25:16.000000 squice-0.5/src/squice/MtxDisplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-27 17:25:16.000000 squice-0.5/src/squice/MtxInterpolator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11412 2024-05-27 17:25:16.000000 squice-0.5/src/squice/SpaceTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-05-27 17:25:16.000000 squice-0.5/src/squice/VectorThree.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/squice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79087 2024-05-27 17:25:16.000000 squice-0.5/src/squice/_interpolator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.317177 squice-0.5/src/squice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-27 17:25:22.000000 squice-0.5/src/squice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-27 17:25:22.000000 squice-0.5/src/squice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:25:22.000000 squice-0.5/src/squice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 17:25:22.000000 squice-0.5/src/squice.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.313177 squice-0.5/src/tests/speed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/tests/speed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.317177 squice-0.5/src/tests/speed/data/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 17:25:16.000000 squice-0.5/src/tests/speed/data/speed_data.npy
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 17:25:16.000000 squice-0.5/src/tests/speed/data/speed_log.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-27 17:25:16.000000 squice-0.5/src/tests/speed/help_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-27 17:25:16.000000 squice-0.5/src/tests/speed/test_dataloaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.317177 squice-0.5/src/tests/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:16.000000 squice-0.5/src/tests/utility/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:25:22.317177 squice-0.5/src/tests/utility/data/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-27 17:25:16.000000 squice-0.5/src/tests/utility/data/data1.npy
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 17:25:16.000000 squice-0.5/src/tests/utility/data/data3d.npy
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-27 17:25:16.000000 squice-0.5/src/tests/utility/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-27 17:25:16.000000 squice-0.5/src/tests/utility/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-27 17:25:16.000000 squice-0.5/tmp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.762890 squice-0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.750890 squice-0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.754890 squice-0.6/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-06-02 15:58:36.000000 squice-0.6/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.754890 squice-0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-06-02 15:58:36.000000 squice-0.6/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-06-02 15:58:36.000000 squice-0.6/.github/workflows/lint_style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-02 15:58:36.000000 squice-0.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-06-02 15:58:36.000000 squice-0.6/.github/workflows/pydoctor.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-06-02 15:58:36.000000 squice-0.6/.github/workflows/pytest_app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-06-02 15:58:36.000000 squice-0.6/.github/workflows/pytest_lib.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-06-02 15:58:36.000000 squice-0.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-06-02 15:58:36.000000 squice-0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-06-02 15:58:36.000000 squice-0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-06-02 15:58:36.000000 squice-0.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-06-02 15:58:36.000000 squice-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-06-02 15:58:41.762890 squice-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-06-02 15:58:36.000000 squice-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.754890 squice-0.6/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-06-02 15:58:36.000000 squice-0.6/app/home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.754890 squice-0.6/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    16851 2024-06-02 15:58:36.000000 squice-0.6/app/pages/2_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-02 15:58:36.000000 squice-0.6/app/pages/4_about.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.754890 squice-0.6/app/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   183520 2024-06-02 15:58:36.000000 squice-0.6/app/static/squice.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.750890 squice-0.6/app/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.758890 squice-0.6/app/tests/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-02 15:58:36.000000 squice-0.6/app/tests/use_cases/test_add_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-06-02 15:58:36.000000 squice-0.6/citation.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-06-02 15:58:36.000000 squice-0.6/dev.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.758890 squice-0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-02 15:58:36.000000 squice-0.6/docs/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-06-02 15:58:36.000000 squice-0.6/matrix (1).npy
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-02 15:58:36.000000 squice-0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-02 15:58:36.000000 squice-0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-02 15:58:36.000000 squice-0.6/requirements_lib.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-06-02 15:58:41.762890 squice-0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.758890 squice-0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-02 15:58:36.000000 squice-0.6/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:36.000000 squice-0.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.758890 squice-0.6/src/squice/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-06-02 15:58:36.000000 squice-0.6/src/squice/BinaryFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-06-02 15:58:36.000000 squice-0.6/src/squice/DataLoaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-06-02 15:58:36.000000 squice-0.6/src/squice/GridMaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-06-02 15:58:36.000000 squice-0.6/src/squice/Matrix3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:36.000000 squice-0.6/src/squice/ModulePredict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-06-02 15:58:36.000000 squice-0.6/src/squice/MtxDisplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-06-02 15:58:36.000000 squice-0.6/src/squice/MtxInterpolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11398 2024-06-02 15:58:36.000000 squice-0.6/src/squice/SpaceTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-06-02 15:58:36.000000 squice-0.6/src/squice/VectorThree.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:36.000000 squice-0.6/src/squice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.762890 squice-0.6/src/squice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-06-02 15:58:41.000000 squice-0.6/src/squice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-06-02 15:58:41.000000 squice-0.6/src/squice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:58:41.000000 squice-0.6/src/squice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-02 15:58:41.000000 squice-0.6/src/squice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.758890 squice-0.6/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:36.000000 squice-0.6/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.758890 squice-0.6/src/tests/speed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:36.000000 squice-0.6/src/tests/speed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.762890 squice-0.6/src/tests/speed/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-02 15:58:36.000000 squice-0.6/src/tests/speed/data/speed_data.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-02 15:58:36.000000 squice-0.6/src/tests/speed/data/speed_log.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-06-02 15:58:36.000000 squice-0.6/src/tests/speed/help_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-06-02 15:58:36.000000 squice-0.6/src/tests/speed/test_dataloaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.762890 squice-0.6/src/tests/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:36.000000 squice-0.6/src/tests/utility/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:58:41.762890 squice-0.6/src/tests/utility/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-02 15:58:36.000000 squice-0.6/src/tests/utility/data/data1.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-02 15:58:36.000000 squice-0.6/src/tests/utility/data/data3d.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-06-02 15:58:36.000000 squice-0.6/src/tests/utility/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-06-02 15:58:36.000000 squice-0.6/src/tests/utility/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-06-02 15:58:36.000000 squice-0.6/src/tests/utility/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-06-02 15:58:36.000000 squice-0.6/tmp
```

### Comparing `squice-0.5/.github/scripts/release.py` & `squice-0.6/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `squice-0.5/.github/workflows/docker.yml` & `squice-0.6/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `squice-0.5/.github/workflows/lint_style.yml` & `squice-0.6/.github/workflows/lint_style.yml`

 * *Files identical despite different names*

### Comparing `squice-0.5/.github/workflows/pydoctor.yml` & `squice-0.6/.github/workflows/pydoctor.yml`

 * *Files identical despite different names*

### Comparing `squice-0.5/.github/workflows/pytest_app.yml` & `squice-0.6/.github/workflows/pytest_app.yml`

 * *Files identical despite different names*

### Comparing `squice-0.5/.github/workflows/pytest_lib.yml` & `squice-0.6/.github/workflows/pytest_lib.yml`

 * *Files identical despite different names*

### Comparing `squice-0.5/.gitignore` & `squice-0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `squice-0.5/Dockerfile` & `squice-0.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `squice-0.5/LICENSE` & `squice-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `squice-0.5/PKG-INFO` & `squice-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squice
-Version: 0.5
+Version: 0.6
 Summary: Example library for scientific software.
 Home-page: https://github.com/RachelAlcraft/squice
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/RachelAlcraft/squice/issues
 Project-URL: Documentation, https://rachelalcraft.github.io/squice
 Project-URL: Application demo, https://squice.streamlit.app
```

### Comparing `squice-0.5/README.md` & `squice-0.6/README.md`

 * *Files identical despite different names*

### Comparing `squice-0.5/app/home.py` & `squice-0.6/app/home.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,38 @@
 
 st.write(
     """
 *SQUICE* is a scientific data library for visualising and manipulating orthogonal
 numerical matrices. These matrices can be any kind of numerical data, including data or
 some kind of data in space.
 
+The documentation for the library classes and functions can be found at
+[pydoctor squice library doc](https://rachelalcraft.github.io/squice/)
+
+Issues can be raised here
+[squice github issues](https://github.com/RachelAlcraft/squice/issues)
+
+The library is on pypi: [squice on pypi](https://pypi.org/project/squice/)
+
 In addition to the ability to load or define 3d numpy matrices for the library, there
 is provided a simple means to convert electron density/microscopy and protein
 data into 3d matrices for visualisation as this was the motivating factor behind the
 library.
 
 This library was written under my split dual identity as a PhD student in Computational
 Biology at Birkbeck (University of London) and as a Research Software Engineer at
  the Institute of Cancer Research.
 
 The example page gives the ability to load or define matrix data and navigate
 the data with slices and interpolation choices. All code is given so you can replicate
 the functionality in your own scripts.
 
-*The ethos of this [scientific library structure]
-(https://github.com/RachelAlcraft/app-lib-py) is to use a functional app like
+*The ethos of this
+[scientific library structure](https://github.com/RachelAlcraft/app-lib-py)
+is to use a functional app like
 this to demonstrate the python library with all code given, democratising use of the
 tool across user groups of different resources and expertise.*
 
 ---
 
 With thanks to my supervisor at Birkbeck,
 [Dr Mark Williams](https://www.bbk.ac.uk/our-staff/profile/8006855/mark-williams),
@@ -51,7 +60,8 @@
 interpolation of numerical matrix data, 2024, doi:*"""
 )
 "---"
 st.caption(
     """~~ ~~ ~~ Contact: [Rachel by email](mailto:raye.alcraft.dev@gmail.com),
 :copyright: 2024 ~~ ~~ ~~"""
 )
+"---"
```

### Comparing `squice-0.5/app/static/squice.png` & `squice-0.6/app/static/squice.png`

 * *Files identical despite different names*

### Comparing `squice-0.5/dev.md` & `squice-0.6/dev.md`

 * *Files identical despite different names*

### Comparing `squice-0.5/setup.cfg` & `squice-0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `squice-0.5/src/squice/BinaryFile.py` & `squice-0.6/src/squice/BinaryFile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Class to load and handle binary data.
 This could be electron density data or numpy data.
 They feature header info followed by the boinary data.
 """
+
 from abc import ABC, abstractmethod
-import numpy as np
+
 
 ####################################################################################
 class BinaryFile(ABC):
     """Abstract class to various formats of binary data"""
 
     def __init__(self, filedata, header):
         self.filedata = filedata
@@ -19,19 +20,14 @@
         pass
 
 
 ####################################################################################
 class NumpyBinary(BinaryFile):
     """
     Features binray data in the format:
-    b"\x93NUMPY\x01\x00v\x00{
-        'descr': '<f8',
-        'fortran_order': False,
-        'shape': (3, 3, 3), } \n
-        {\x14\xaeG\xe1z\x84?\x00\x00\x00\...00\x00"
     https://numpy.org/doc/1.13/neps/npy-format.html
     """
 
     def load(self):
         """Load the numpy data"""
         # for i in range
         # val = int.from_bytes(ccp4_binary[i:i+inc], byteorder='little', signed=True)
```

### Comparing `squice-0.5/src/squice/DataLoaders.py` & `squice-0.6/src/squice/DataLoaders.py`

 * *Files identical despite different names*

### Comparing `squice-0.5/src/squice/GridMaker.py` & `squice-0.6/src/squice/GridMaker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """
 GridMaker: makes a grid or chunk of points given the secified size and samples
 
 """
-import math
-import numpy as np
 
 from . import Matrix3d as d3
 
 
 class GridMaker(object):
     def get_unit_grid(self, width, samples, depth_samples=1):
-        side = int(math.floor(samples / 2))
         offset = (samples - 1) / 2
         gap = 1
         if samples > 1:
             gap = width / (samples - 1)
         # if there is a depth, there will be fewer samples
         if depth_samples > 1:
             return self.get_unit_grid3d(width, samples, depth_samples)
```

### Comparing `squice-0.5/src/squice/MtxInterpolator.py` & `squice-0.6/src/squice/MtxInterpolator.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,62 +2,74 @@
 Module to interpolate inside a numpy matrix with some bespoke methods
 """
 
 from abc import ABC, abstractmethod
 from .DataLoaders import NumpyNow
 from scipy.interpolate import RegularGridInterpolator
 import numpy as np
-import math
 
 
 ####################################################################################
 class MtxInterpolator(ABC):
     """
     Abstract class to define the methods for interpolation of a 3d numpy matrix.
     There are 3 methods of wrapping the data if it is out of bounds:
-    - cap : it is simply fixed at the bounds if it goes beyond
-    - periodic: it loops to make it a periodic shape eg 3.1 becomes 0.1 if the max is 3
-    - mirror: the edges reflect back, best only with small bleeds in the edge
-
+    cap : it is simply fixed at the bounds if it goes beyond
+    periodic: it loops to make it a periodic shape eg 3.1 becomes 0.1 if the max is 3
+    mirror: the edges reflect back, best only with small bleeds in the edge
 
     """
 
     def __init__(self, mtx, wrap="none"):
+        """
+        - mtx=numpy matrix
+        - wrap=["none","periodic"]
+        """
         self.mtx = mtx
         self.wrap = wrap
 
-    def get_value(self, x, y, z):
-        # 1. first validate inputs
+    # I need to work out these formula!!!! when negative what should the periodic be.
+
+    def convert_coord(self, x, y, z):
+        valid = True
         xx, yy, zz = self.mtx.shape
+
         if self.wrap == "periodic":
-            x = (math.floor(x) // xx) + (x - math.floor(x))
-            y = (math.floor(y) // yy) + (y - math.floor(y))
-            z = (math.floor(z) // zz) + (z - math.floor(z))
-        elif self.wrap == "mirror":
-            if x - xx - 1 > 0:
-                x = xx - (x - xx)
-            x = (math.floor(x) // xx) + (x - math.floor(x))
-            y = (math.floor(y) // yy) + (y - math.floor(y))
-            z = (math.floor(z) // zz) + (z - math.floor(z))
-        elif self.wrap == "cap":
-            x = min(x, xx - 1)
-            y = min(y, yy - 1)
-            z = min(z, zz - 1)
-            x = max(x, 0)
-            y = max(y, 0)
-            z = max(z, 0)
-        else:
-            x, y, z = round(x, 4), round(y, 4), round(z, 4)
-            if x > xx - 1 or y > yy - 1 or z > zz - 1:
-                return None
-            if x < 0 or y < 0 or z < 0:
-                return None
+            while x < 0:
+                x += xx - 1
+            while y < 0:
+                y += yy - 1
+            while z < 0:
+                z += zz - 1
+            while x > xx - 1:
+                x -= xx - 1
+            while y > yy - 1:
+                y -= yy - 1
+            while z > zz - 1:
+                z -= zz - 1
+
+        x, y, z = round(x, 4), round(y, 4), round(z, 4)
+        if x > xx - 1 or y > yy - 1 or z > zz - 1:
+            valid = False
+        if x < 0 or y < 0 or z < 0:
+            valid = False
 
+        return x, y, z, valid
+
+    def get_value(self, xi, yi, zi):
+        # 1. first validate inputs
+        x, y, z, valid = self.convert_coord(xi, yi, zi)
+        x, y, z = round(x, 4), round(y, 4), round(z, 4)
+        if not valid:
+            return None
         # 2. get the value from the interpolator
-        return self._get_value(x, y, z)
+        try:
+            return self._get_value(x, y, z)
+        except Exception as e:
+            print(e)
 
     @abstractmethod
     def _get_value(self, x, y, z):
         pass
 
     def get_val_slice(self, coords_mtx):
         """
```

### Comparing `squice-0.5/src/squice/SpaceTransform.py` & `squice-0.6/src/squice/SpaceTransform.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,28 +158,27 @@
         point2 = self.rotate(pointPrime.B, pointPrime.C, rotationYZ_4)
         pointPrime.B = point2.A
         pointPrime.C = point2.B
 
         return pointPrime
 
     def convert_coords(self, unit_coords):
-        coords = []
         # 2d or 3d?
-        if type(unit_coords) is d3.Matrix3d:
+        a, b, c = unit_coords.shape()
+        if c > 1:
             return self.convert_coords3d(unit_coords)
         else:
-            a, b = unit_coords.shape()
             mat2 = d3.Matrix3d(a, b)
             for i in range(a):
                 for j in range(b):
                     vec = v3.VectorThree(
                         unit_coords.get(i, j)[0], unit_coords.get(i, j)[1], 0
                     )
                     vec_t = self.apply_transformation(vec)
-                    mat2.add(i, j, vec_t)
+                    mat2.add(i, j, data=vec_t)
             return mat2
 
     def convert_coords3d(self, unit_coords):
         a, b, c = unit_coords.shape()
         mat3 = d3.Matrix3d(a, b, c)
         for i in range(a):
             for j in range(b):
@@ -269,16 +268,16 @@
                 # Math.Round(x2, 8);
                 v.B = y2
                 # Math.Round(y2, 8);
             return v
         else:
             return v3.VectorThree(x, y, 0)
 
-    def navigate(self, point, nav, nav_distance):
-        angle = 2 * self.M_PI / 90
+    def navigate(self, point, nav, nav_distance, angle_delta=1):
+        angle = angle_delta * 2 * self.M_PI / 90
         point = self.reverse_transformation(point)
         if nav == "DN":  #'DN'down
             point.A += nav_distance
         elif nav == "UP":  #'UP'up
             point.A -= nav_distance
         elif nav == "LE":  #'LE'left
             point.B += nav_distance
```

### Comparing `squice-0.5/src/squice/VectorThree.py` & `squice-0.6/src/squice/VectorThree.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,17 @@
                 self.C = v3.C
             else:
                 self.npy = np.array(abc)
                 self.A = self.npy[0]
                 self.B = self.npy[1]
                 self.C = self.npy[2]
 
+    def __str__(self) -> str:
+        return self.to_coords_str()
+
     def from_coords_str(self, coords):
         coords = coords.strip()
         if coords[0] == "(":
             coords = coords[1:]
         if coords[-1] == ")":
             coords = coords[:-1]
         a, b, c = coords.split(",")
```

### Comparing `squice-0.5/src/squice.egg-info/PKG-INFO` & `squice-0.6/src/squice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squice
-Version: 0.5
+Version: 0.6
 Summary: Example library for scientific software.
 Home-page: https://github.com/RachelAlcraft/squice
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/RachelAlcraft/squice/issues
 Project-URL: Documentation, https://rachelalcraft.github.io/squice
 Project-URL: Application demo, https://squice.streamlit.app
```

### Comparing `squice-0.5/src/squice.egg-info/SOURCES.txt` & `squice-0.6/src/squice.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 src/squice/Matrix3d.py
 src/squice/ModulePredict.py
 src/squice/MtxDisplay.py
 src/squice/MtxInterpolator.py
 src/squice/SpaceTransform.py
 src/squice/VectorThree.py
 src/squice/__init__.py
-src/squice/_interpolator.py
 src/squice.egg-info/PKG-INFO
 src/squice.egg-info/SOURCES.txt
 src/squice.egg-info/dependency_links.txt
 src/squice.egg-info/top_level.txt
 src/tests/__init__.py
 src/tests/speed/__init__.py
 src/tests/speed/help_speed.py
 src/tests/speed/test_dataloaders.py
 src/tests/speed/data/speed_data.npy
 src/tests/speed/data/speed_log.csv
 src/tests/utility/__init__.py
+src/tests/utility/test_grid.py
 src/tests/utility/test_loader.py
 src/tests/utility/test_slice.py
 src/tests/utility/data/data1.npy
 src/tests/utility/data/data3d.npy
```

### Comparing `squice-0.5/src/tests/speed/data/speed_log.csv` & `squice-0.6/src/tests/speed/data/speed_log.csv`

 * *Files identical despite different names*

### Comparing `squice-0.5/src/tests/speed/help_speed.py` & `squice-0.6/src/tests/speed/help_speed.py`

 * *Files identical despite different names*

### Comparing `squice-0.5/src/tests/speed/test_dataloaders.py` & `squice-0.6/src/tests/speed/test_dataloaders.py`

 * *Files identical despite different names*

### Comparing `squice-0.5/src/tests/utility/test_loader.py` & `squice-0.6/src/tests/utility/test_loader.py`

 * *Files identical despite different names*

