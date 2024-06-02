# Comparing `tmp/backends-1.6.3.tar.gz` & `tmp/backends-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backends-1.6.3.tar", last modified: Sun Apr 21 15:18:25 2024, max compression
+gzip compressed data, was "backends-1.6.4.tar", last modified: Sun Jun  2 15:10:45 2024, max compression
```

## Comparing `backends-1.6.3.tar` & `backends-1.6.4.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.652110 backends-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 15:18:11.000000 backends-1.6.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.632110 backends-1.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.636110 backends-1.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-21 15:18:11.000000 backends-1.6.3/.github/workflows/build_book.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-21 15:18:11.000000 backends-1.6.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-21 15:18:11.000000 backends-1.6.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-21 15:18:11.000000 backends-1.6.3/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-21 15:18:11.000000 backends-1.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-21 15:18:11.000000 backends-1.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-21 15:18:11.000000 backends-1.6.3/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-21 15:18:11.000000 backends-1.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-21 15:18:11.000000 backends-1.6.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-21 15:18:25.652110 backends-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-04-21 15:18:11.000000 backends-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.648110 backends-1.6.3/backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-21 15:18:25.000000 backends-1.6.3/backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-21 15:18:25.000000 backends-1.6.3/backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 15:18:25.000000 backends-1.6.3/backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-21 15:18:25.000000 backends-1.6.3/backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 15:18:25.000000 backends-1.6.3/backends.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-21 15:18:11.000000 backends-1.6.3/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.640110 backends-1.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-21 15:18:11.000000 backends-1.6.3/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-21 15:18:11.000000 backends-1.6.3/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-21 15:18:11.000000 backends-1.6.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-21 15:18:11.000000 backends-1.6.3/docs/chapter.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-21 15:18:11.000000 backends-1.6.3/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-04-21 15:18:11.000000 backends-1.6.3/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 15:18:11.000000 backends-1.6.3/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.644110 backends-1.6.3/lab/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-21 15:18:11.000000 backends-1.6.3/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 15:18:25.000000 backends-1.6.3/lab/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.644110 backends-1.6.3/lab/autograd/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-21 15:18:11.000000 backends-1.6.3/lab/autograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-21 15:18:11.000000 backends-1.6.3/lab/autograd/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-21 15:18:11.000000 backends-1.6.3/lab/autograd/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-21 15:18:11.000000 backends-1.6.3/lab/autograd/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-21 15:18:11.000000 backends-1.6.3/lab/autograd/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-21 15:18:11.000000 backends-1.6.3/lab/autograd/shaping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.644110 backends-1.6.3/lab/bvn_cdf/
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-21 15:18:11.000000 backends-1.6.3/lab/bvn_cdf/bvn_cdf.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    25945 2024-04-21 15:18:11.000000 backends-1.6.3/lab/bvn_cdf/tvpack.f
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-21 15:18:11.000000 backends-1.6.3/lab/bvn_cdf/tvpack.h
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-21 15:18:11.000000 backends-1.6.3/lab/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-21 15:18:11.000000 backends-1.6.3/lab/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    32852 2024-04-21 15:18:11.000000 backends-1.6.3/lab/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.644110 backends-1.6.3/lab/jax/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-21 15:18:11.000000 backends-1.6.3/lab/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-21 15:18:11.000000 backends-1.6.3/lab/jax/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-04-21 15:18:11.000000 backends-1.6.3/lab/jax/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-21 15:18:11.000000 backends-1.6.3/lab/jax/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-21 15:18:11.000000 backends-1.6.3/lab/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-21 15:18:11.000000 backends-1.6.3/lab/jax/shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-04-21 15:18:11.000000 backends-1.6.3/lab/linear_algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.644110 backends-1.6.3/lab/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-21 15:18:11.000000 backends-1.6.3/lab/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-21 15:18:11.000000 backends-1.6.3/lab/numpy/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-21 15:18:11.000000 backends-1.6.3/lab/numpy/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-21 15:18:11.000000 backends-1.6.3/lab/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-21 15:18:11.000000 backends-1.6.3/lab/numpy/shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-21 15:18:11.000000 backends-1.6.3/lab/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-21 15:18:11.000000 backends-1.6.3/lab/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-04-21 15:18:11.000000 backends-1.6.3/lab/shaping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.648110 backends-1.6.3/lab/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-21 15:18:11.000000 backends-1.6.3/lab/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-21 15:18:11.000000 backends-1.6.3/lab/tensorflow/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-21 15:18:11.000000 backends-1.6.3/lab/tensorflow/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-21 15:18:11.000000 backends-1.6.3/lab/tensorflow/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-21 15:18:11.000000 backends-1.6.3/lab/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-21 15:18:11.000000 backends-1.6.3/lab/tensorflow/shaping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.648110 backends-1.6.3/lab/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-21 15:18:11.000000 backends-1.6.3/lab/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-21 15:18:11.000000 backends-1.6.3/lab/torch/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-21 15:18:11.000000 backends-1.6.3/lab/torch/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-21 15:18:11.000000 backends-1.6.3/lab/torch/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-21 15:18:11.000000 backends-1.6.3/lab/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-21 15:18:11.000000 backends-1.6.3/lab/torch/shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-04-21 15:18:11.000000 backends-1.6.3/lab/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-21 15:18:11.000000 backends-1.6.3/lab/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-21 15:18:11.000000 backends-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 15:18:11.000000 backends-1.6.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-21 15:18:11.000000 backends-1.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-21 15:18:25.652110 backends-1.6.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4286 2024-04-21 15:18:11.000000 backends-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:18:25.648110 backends-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-21 15:18:11.000000 backends-1.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-21 15:18:11.000000 backends-1.6.3/tests/test_control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-21 15:18:11.000000 backends-1.6.3/tests/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-04-21 15:18:11.000000 backends-1.6.3/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-04-21 15:18:11.000000 backends-1.6.3/tests/test_linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-04-21 15:18:11.000000 backends-1.6.3/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-21 15:18:11.000000 backends-1.6.3/tests/test_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-04-21 15:18:11.000000 backends-1.6.3/tests/test_shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-04-21 15:18:11.000000 backends-1.6.3/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-21 15:18:11.000000 backends-1.6.3/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-21 15:18:11.000000 backends-1.6.3/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-21 15:18:11.000000 backends-1.6.3/todo.tasks
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.470333 backends-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-02 15:10:23.000000 backends-1.6.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.450333 backends-1.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.458333 backends-1.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-02 15:10:23.000000 backends-1.6.4/.github/workflows/build_book.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-06-02 15:10:23.000000 backends-1.6.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-06-02 15:10:23.000000 backends-1.6.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-06-02 15:10:23.000000 backends-1.6.4/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-06-02 15:10:23.000000 backends-1.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-06-02 15:10:23.000000 backends-1.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-02 15:10:23.000000 backends-1.6.4/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 15:10:23.000000 backends-1.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-02 15:10:23.000000 backends-1.6.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-06-02 15:10:45.470333 backends-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-06-02 15:10:23.000000 backends-1.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.470333 backends-1.6.4/backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-06-02 15:10:45.000000 backends-1.6.4/backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-06-02 15:10:45.000000 backends-1.6.4/backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:10:45.000000 backends-1.6.4/backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-02 15:10:45.000000 backends-1.6.4/backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 15:10:45.000000 backends-1.6.4/backends.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-06-02 15:10:23.000000 backends-1.6.4/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.458333 backends-1.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-06-02 15:10:23.000000 backends-1.6.4/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-02 15:10:23.000000 backends-1.6.4/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-06-02 15:10:23.000000 backends-1.6.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-02 15:10:23.000000 backends-1.6.4/docs/chapter.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 15:10:23.000000 backends-1.6.4/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-06-02 15:10:23.000000 backends-1.6.4/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-02 15:10:23.000000 backends-1.6.4/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.462333 backends-1.6.4/lab/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-06-02 15:10:23.000000 backends-1.6.4/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-02 15:10:45.000000 backends-1.6.4/lab/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.462333 backends-1.6.4/lab/autograd/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-06-02 15:10:23.000000 backends-1.6.4/lab/autograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-06-02 15:10:23.000000 backends-1.6.4/lab/autograd/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-06-02 15:10:23.000000 backends-1.6.4/lab/autograd/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-06-02 15:10:23.000000 backends-1.6.4/lab/autograd/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-06-02 15:10:23.000000 backends-1.6.4/lab/autograd/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-06-02 15:10:23.000000 backends-1.6.4/lab/autograd/shaping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.462333 backends-1.6.4/lab/bvn_cdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-06-02 15:10:23.000000 backends-1.6.4/lab/bvn_cdf/bvn_cdf.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    25945 2024-06-02 15:10:23.000000 backends-1.6.4/lab/bvn_cdf/tvpack.f
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-02 15:10:23.000000 backends-1.6.4/lab/bvn_cdf/tvpack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-06-02 15:10:23.000000 backends-1.6.4/lab/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-06-02 15:10:23.000000 backends-1.6.4/lab/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32852 2024-06-02 15:10:23.000000 backends-1.6.4/lab/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.466333 backends-1.6.4/lab/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-06-02 15:10:23.000000 backends-1.6.4/lab/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-06-02 15:10:23.000000 backends-1.6.4/lab/jax/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-06-02 15:10:23.000000 backends-1.6.4/lab/jax/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-06-02 15:10:23.000000 backends-1.6.4/lab/jax/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-06-02 15:10:23.000000 backends-1.6.4/lab/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-06-02 15:10:23.000000 backends-1.6.4/lab/jax/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-06-02 15:10:23.000000 backends-1.6.4/lab/linear_algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.466333 backends-1.6.4/lab/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-06-02 15:10:23.000000 backends-1.6.4/lab/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-06-02 15:10:23.000000 backends-1.6.4/lab/numpy/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-06-02 15:10:23.000000 backends-1.6.4/lab/numpy/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-06-02 15:10:23.000000 backends-1.6.4/lab/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-06-02 15:10:23.000000 backends-1.6.4/lab/numpy/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-06-02 15:10:23.000000 backends-1.6.4/lab/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-06-02 15:10:23.000000 backends-1.6.4/lab/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-06-02 15:10:23.000000 backends-1.6.4/lab/shaping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.466333 backends-1.6.4/lab/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-06-02 15:10:23.000000 backends-1.6.4/lab/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-06-02 15:10:23.000000 backends-1.6.4/lab/tensorflow/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-06-02 15:10:23.000000 backends-1.6.4/lab/tensorflow/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-06-02 15:10:23.000000 backends-1.6.4/lab/tensorflow/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-06-02 15:10:23.000000 backends-1.6.4/lab/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-06-02 15:10:23.000000 backends-1.6.4/lab/tensorflow/shaping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.466333 backends-1.6.4/lab/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-06-02 15:10:23.000000 backends-1.6.4/lab/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-06-02 15:10:23.000000 backends-1.6.4/lab/torch/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-06-02 15:10:23.000000 backends-1.6.4/lab/torch/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-06-02 15:10:23.000000 backends-1.6.4/lab/torch/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-06-02 15:10:23.000000 backends-1.6.4/lab/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-06-02 15:10:23.000000 backends-1.6.4/lab/torch/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-06-02 15:10:23.000000 backends-1.6.4/lab/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-06-02 15:10:23.000000 backends-1.6.4/lab/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-06-02 15:10:23.000000 backends-1.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-02 15:10:23.000000 backends-1.6.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-06-02 15:10:23.000000 backends-1.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-06-02 15:10:45.470333 backends-1.6.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4275 2024-06-02 15:10:23.000000 backends-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:10:45.470333 backends-1.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-02 15:10:23.000000 backends-1.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-06-02 15:10:23.000000 backends-1.6.4/tests/test_control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-06-02 15:10:23.000000 backends-1.6.4/tests/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19141 2024-06-02 15:10:23.000000 backends-1.6.4/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-06-02 15:10:23.000000 backends-1.6.4/tests/test_linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-06-02 15:10:23.000000 backends-1.6.4/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-06-02 15:10:23.000000 backends-1.6.4/tests/test_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-06-02 15:10:23.000000 backends-1.6.4/tests/test_shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-06-02 15:10:23.000000 backends-1.6.4/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-06-02 15:10:23.000000 backends-1.6.4/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-06-02 15:10:23.000000 backends-1.6.4/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-06-02 15:10:23.000000 backends-1.6.4/todo.tasks
```

### Comparing `backends-1.6.3/.github/workflows/build_book.yml` & `backends-1.6.4/.github/workflows/build_book.yml`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/.github/workflows/ci.yml` & `backends-1.6.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/.github/workflows/publish.yml` & `backends-1.6.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/.pre-commit-config.yaml` & `backends-1.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/LICENCE.txt` & `backends-1.6.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/PKG-INFO` & `backends-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: backends
-Version: 1.6.3
+Version: 1.6.4
 Summary: A generic interface for linear algebra backends
 Home-page: https://github.com/wesselb/lab
 Author: Wessel Bruinsma
 Author-email: wessel.p.bruinsma@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: numpy>=1.16
 Requires-Dist: scipy>=1.3
-Requires-Dist: fdm
 Requires-Dist: plum-dispatch>=2.3.5
 Requires-Dist: opt-einsum
 
 # [LAB](http://github.com/wesselb/lab)
 
 [![CI](https://github.com/wesselb/lab/workflows/CI/badge.svg?branch=master)](https://github.com/wesselb/lab/actions?query=workflow%3ACI)
 [![Coverage Status](https://coveralls.io/repos/github/wesselb/lab/badge.svg?branch=master&service=github)](https://coveralls.io/github/wesselb/lab?branch=master)
```

### Comparing `backends-1.6.3/README.md` & `backends-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/backends.egg-info/PKG-INFO` & `backends-1.6.4/backends.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: backends
-Version: 1.6.3
+Version: 1.6.4
 Summary: A generic interface for linear algebra backends
 Home-page: https://github.com/wesselb/lab
 Author: Wessel Bruinsma
 Author-email: wessel.p.bruinsma@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: numpy>=1.16
 Requires-Dist: scipy>=1.3
-Requires-Dist: fdm
 Requires-Dist: plum-dispatch>=2.3.5
 Requires-Dist: opt-einsum
 
 # [LAB](http://github.com/wesselb/lab)
 
 [![CI](https://github.com/wesselb/lab/workflows/CI/badge.svg?branch=master)](https://github.com/wesselb/lab/actions?query=workflow%3ACI)
 [![Coverage Status](https://coveralls.io/repos/github/wesselb/lab/badge.svg?branch=master&service=github)](https://coveralls.io/github/wesselb/lab?branch=master)
```

### Comparing `backends-1.6.3/backends.egg-info/SOURCES.txt` & `backends-1.6.4/backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/benchmark.py` & `backends-1.6.4/benchmark.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/docs/_config.yml` & `backends-1.6.4/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/docs/api.rst` & `backends-1.6.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/docs/logo.png` & `backends-1.6.4/docs/logo.png`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/autograd/__init__.py` & `backends-1.6.4/lab/autograd/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/autograd/custom.py` & `backends-1.6.4/lab/autograd/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/autograd/generic.py` & `backends-1.6.4/lab/autograd/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/autograd/linear_algebra.py` & `backends-1.6.4/lab/autograd/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/autograd/random.py` & `backends-1.6.4/lab/autograd/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/autograd/shaping.py` & `backends-1.6.4/lab/autograd/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/bvn_cdf/bvn_cdf.pyx` & `backends-1.6.4/lab/bvn_cdf/bvn_cdf.pyx`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/bvn_cdf/tvpack.f` & `backends-1.6.4/lab/bvn_cdf/tvpack.f`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/control_flow.py` & `backends-1.6.4/lab/control_flow.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/custom.py` & `backends-1.6.4/lab/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/generic.py` & `backends-1.6.4/lab/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/jax/__init__.py` & `backends-1.6.4/lab/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/jax/custom.py` & `backends-1.6.4/lab/jax/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/jax/generic.py` & `backends-1.6.4/lab/jax/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/jax/linear_algebra.py` & `backends-1.6.4/lab/jax/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/jax/random.py` & `backends-1.6.4/lab/jax/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/jax/shaping.py` & `backends-1.6.4/lab/jax/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/linear_algebra.py` & `backends-1.6.4/lab/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/numpy/__init__.py` & `backends-1.6.4/lab/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/numpy/generic.py` & `backends-1.6.4/lab/numpy/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/numpy/linear_algebra.py` & `backends-1.6.4/lab/numpy/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/numpy/random.py` & `backends-1.6.4/lab/numpy/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/numpy/shaping.py` & `backends-1.6.4/lab/numpy/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/random.py` & `backends-1.6.4/lab/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/shape.py` & `backends-1.6.4/lab/shape.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/shaping.py` & `backends-1.6.4/lab/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/tensorflow/__init__.py` & `backends-1.6.4/lab/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/tensorflow/custom.py` & `backends-1.6.4/lab/tensorflow/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/tensorflow/generic.py` & `backends-1.6.4/lab/tensorflow/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/tensorflow/linear_algebra.py` & `backends-1.6.4/lab/tensorflow/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/tensorflow/random.py` & `backends-1.6.4/lab/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/tensorflow/shaping.py` & `backends-1.6.4/lab/tensorflow/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/torch/__init__.py` & `backends-1.6.4/lab/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/torch/custom.py` & `backends-1.6.4/lab/torch/custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/torch/generic.py` & `backends-1.6.4/lab/torch/generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/torch/linear_algebra.py` & `backends-1.6.4/lab/torch/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/torch/random.py` & `backends-1.6.4/lab/torch/random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/torch/shaping.py` & `backends-1.6.4/lab/torch/shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/types.py` & `backends-1.6.4/lab/types.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/lab/util.py` & `backends-1.6.4/lab/util.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/setup.py` & `backends-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
                 extra_link_args=extra_link_args,
             )
         )
 
 requirements = [
     "numpy>=1.16",
     "scipy>=1.3",
-    "fdm",
     "plum-dispatch>=2.3.5",
     "opt-einsum",
 ]
 
 setup(
     packages=find_packages(exclude=["docs"]),
     python_requires=">=3.8",
```

### Comparing `backends-1.6.3/tests/test_control_flow.py` & `backends-1.6.4/tests/test_control_flow.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/tests/test_custom.py` & `backends-1.6.4/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/tests/test_generic.py` & `backends-1.6.4/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/tests/test_linear_algebra.py` & `backends-1.6.4/tests/test_linear_algebra.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/tests/test_random.py` & `backends-1.6.4/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/tests/test_shape.py` & `backends-1.6.4/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/tests/test_shaping.py` & `backends-1.6.4/tests/test_shaping.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/tests/test_types.py` & `backends-1.6.4/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/tests/test_util.py` & `backends-1.6.4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/tests/util.py` & `backends-1.6.4/tests/util.py`

 * *Files identical despite different names*

### Comparing `backends-1.6.3/todo.tasks` & `backends-1.6.4/todo.tasks`

 * *Files identical despite different names*

