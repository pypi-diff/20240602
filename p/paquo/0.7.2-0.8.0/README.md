# Comparing `tmp/paquo-0.7.2.tar.gz` & `tmp/paquo-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paquo-0.7.2.tar", last modified: Thu Feb 22 00:33:47 2024, max compression
+gzip compressed data, was "paquo-0.8.0.tar", last modified: Sun Jun  2 17:26:46 2024, max compression
```

## Comparing `paquo-0.7.2.tar` & `paquo-0.8.0.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:33:47.736148 paquo-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-22 00:33:40.000000 paquo-0.7.2/.bandit
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-22 00:33:40.000000 paquo-0.7.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-22 00:33:40.000000 paquo-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-02-22 00:33:40.000000 paquo-0.7.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 00:33:40.000000 paquo-0.7.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-02-22 00:33:40.000000 paquo-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 00:33:40.000000 paquo-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-22 00:33:40.000000 paquo-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-02-22 00:33:47.736148 paquo-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-02-22 00:33:40.000000 paquo-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:33:47.724148 paquo-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-22 00:33:40.000000 paquo-0.7.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:33:47.728148 paquo-0.7.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:33:47.728148 paquo-0.7.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   308228 2024-02-22 00:33:40.000000 paquo-0.7.2/docs/source/_static/screenshot_example_05.png
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-02-22 00:33:40.000000 paquo-0.7.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-02-22 00:33:40.000000 paquo-0.7.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-22 00:33:40.000000 paquo-0.7.2/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-02-22 00:33:40.000000 paquo-0.7.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-02-22 00:33:40.000000 paquo-0.7.2/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-02-22 00:33:40.000000 paquo-0.7.2/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-22 00:33:40.000000 paquo-0.7.2/environment.devenv.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:33:47.728148 paquo-0.7.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-22 00:33:40.000000 paquo-0.7.2/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-22 00:33:40.000000 paquo-0.7.2/examples/example_01_read_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-22 00:33:40.000000 paquo-0.7.2/examples/example_02_add_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-22 00:33:40.000000 paquo-0.7.2/examples/example_03_project_with_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-22 00:33:40.000000 paquo-0.7.2/examples/example_04_project_with_image_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-02-22 00:33:40.000000 paquo-0.7.2/examples/example_05_draw_tiles_on_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-02-22 00:33:40.000000 paquo-0.7.2/examples/prepare_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:33:47.728148 paquo-0.7.2/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-22 00:33:40.000000 paquo-0.7.2/extras/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:33:47.728148 paquo-0.7.2/extras/osx_app_shim/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-22 00:33:40.000000 paquo-0.7.2/extras/osx_app_shim/PaquoOpenQpZip.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-22 00:33:40.000000 paquo-0.7.2/extras/osx_app_shim/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:33:47.732149 paquo-0.7.2/paquo/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/.paquo.defaults.toml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-22 00:33:47.000000 paquo-0.7.2/paquo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    27229 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)    24850 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/java.py
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/jpype_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/pathobjects.py
--rw-r--r--   0 runner    (1001) docker     (127)    22602 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:33:47.736148 paquo-0.7.2/paquo/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/test_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/test_jpype_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/test_pathobjects.py
--rw-r--r--   0 runner    (1001) docker     (127)    12620 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/test_readonly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-22 00:33:40.000000 paquo-0.7.2/paquo/tests/test_repr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:33:47.736148 paquo-0.7.2/paquo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-02-22 00:33:47.000000 paquo-0.7.2/paquo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-22 00:33:47.000000 paquo-0.7.2/paquo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 00:33:47.000000 paquo-0.7.2/paquo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-22 00:33:47.000000 paquo-0.7.2/paquo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-22 00:33:47.000000 paquo-0.7.2/paquo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-22 00:33:47.000000 paquo-0.7.2/paquo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-22 00:33:40.000000 paquo-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-22 00:33:47.736148 paquo-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:46.932763 paquo-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-02 17:26:41.000000 paquo-0.8.0/.bandit
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-02 17:26:41.000000 paquo-0.8.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-02 17:26:41.000000 paquo-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-06-02 17:26:41.000000 paquo-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-02 17:26:41.000000 paquo-0.8.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-06-02 17:26:41.000000 paquo-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-02 17:26:41.000000 paquo-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-02 17:26:41.000000 paquo-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-06-02 17:26:46.932763 paquo-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-06-02 17:26:41.000000 paquo-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:46.920763 paquo-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-02 17:26:41.000000 paquo-0.8.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:46.920763 paquo-0.8.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:46.920763 paquo-0.8.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   308228 2024-06-02 17:26:41.000000 paquo-0.8.0/docs/source/_static/screenshot_example_05.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-06-02 17:26:41.000000 paquo-0.8.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-06-02 17:26:41.000000 paquo-0.8.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-06-02 17:26:41.000000 paquo-0.8.0/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-06-02 17:26:41.000000 paquo-0.8.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-06-02 17:26:41.000000 paquo-0.8.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-06-02 17:26:41.000000 paquo-0.8.0/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-06-02 17:26:41.000000 paquo-0.8.0/environment.devenv.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:41.000000 paquo-0.8.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:46.924763 paquo-0.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-06-02 17:26:41.000000 paquo-0.8.0/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-06-02 17:26:41.000000 paquo-0.8.0/examples/example_01_read_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-06-02 17:26:41.000000 paquo-0.8.0/examples/example_02_add_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-06-02 17:26:41.000000 paquo-0.8.0/examples/example_03_project_with_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-06-02 17:26:41.000000 paquo-0.8.0/examples/example_04_project_with_image_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-06-02 17:26:41.000000 paquo-0.8.0/examples/example_05_draw_tiles_on_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-06-02 17:26:41.000000 paquo-0.8.0/examples/prepare_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:46.924763 paquo-0.8.0/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-06-02 17:26:41.000000 paquo-0.8.0/extras/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:46.924763 paquo-0.8.0/extras/osx_app_shim/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-02 17:26:41.000000 paquo-0.8.0/extras/osx_app_shim/PaquoOpenQpZip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-06-02 17:26:41.000000 paquo-0.8.0/extras/osx_app_shim/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:46.928763 paquo-0.8.0/paquo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/.paquo.defaults.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-02 17:26:46.000000 paquo-0.8.0/paquo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    28944 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24850 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/java.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/jpype_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15066 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/pathobjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22602 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:46.932763 paquo-0.8.0/paquo/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13353 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/test_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/test_jpype_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/test_pathobjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12620 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/test_readonly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-06-02 17:26:41.000000 paquo-0.8.0/paquo/tests/test_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:26:46.932763 paquo-0.8.0/paquo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-06-02 17:26:46.000000 paquo-0.8.0/paquo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-06-02 17:26:46.000000 paquo-0.8.0/paquo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:26:46.000000 paquo-0.8.0/paquo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-02 17:26:46.000000 paquo-0.8.0/paquo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-06-02 17:26:46.000000 paquo-0.8.0/paquo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 17:26:46.000000 paquo-0.8.0/paquo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-06-02 17:26:41.000000 paquo-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-06-02 17:26:46.932763 paquo-0.8.0/setup.cfg
```

### Comparing `paquo-0.7.2/.pre-commit-config.yaml` & `paquo-0.8.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-added-large-files
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.15.1
+  rev: v3.15.2
   hooks:
   - id: pyupgrade
     args: [--py38-plus]
 - repo: https://github.com/pycqa/isort
   rev: 5.13.2
   hooks:
   - id: isort
     exclude: ^examples|^extras|^docs|tests.*|setup.py
 # - repo: https://github.com/psf/black
 #   rev: 22.6.0
 #   hooks:
 #   - id: black
 #     language_version: python3
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: 'v1.8.0'
+  rev: 'v1.10.0'
   hooks:
   - id: mypy
     exclude: ^examples|^extras|^docs|tests.*
     additional_dependencies: [packaging, ome-types]
 - repo: https://github.com/PyCQA/flake8
   rev: '7.0.0'
   hooks:
   - id: flake8
     additional_dependencies:
     - flake8-typing-imports==1.15.0
     language_version: python3
     exclude: "^(build|docs|examples|extras|setup.py)|tests[/]"
 - repo: https://github.com/PyCQA/bandit
-  rev: '1.7.7'
+  rev: '1.7.8'
   hooks:
   - id: bandit
     args: ["-lll", "--ini", ".bandit"]
```

### Comparing `paquo-0.7.2/CHANGELOG.md` & `paquo-0.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
 
+## [0.8.0] - 2024-06-02
+### Added
+- added support for PathCellObjects
+- added `.cells` and `.tiles` attributes to hierarchy
+
+### Fixed
+- fixed QuPath=0.5.1 download via get_qupath
+
 ## [0.7.2] - 2024-02-22
 ### Fixed
 - fixed QuPath=0.5.0 download via get_qupath
 
 ### Changed
 - ci: test against QuPath=0.5.0
 
@@ -149,15 +157,16 @@
 - `QuPathProject.add_image` is now calling `QuPathProject.save`
 
 ## [0.1.0] - 2020-08-12
 ### Added
 - initial release of paquo
 
 
-[Unreleased]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.7.2...HEAD
+[Unreleased]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.8.0...HEAD
+[0.7.2]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.7.2...v0.8.0
 [0.7.2]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.7.1...v0.7.2
 [0.7.1]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.7.0...v0.7.1
 [0.7.0]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.6.1...v0.7.0
 [0.6.1]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.6.0...v0.6.1
 [0.6.0]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.5.1...v0.6.0
 [0.5.1]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.5.0...v0.5.1
 [0.5.0]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.4.2...v0.5.0
```

### Comparing `paquo-0.7.2/CONTRIBUTING.md` & `paquo-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/LICENSE` & `paquo-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/PKG-INFO` & `paquo-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paquo
-Version: 0.7.2
+Version: 0.8.0
 Summary: library for interacting with QuPath
 Home-page: https://github.com/bayer-science-for-a-better-life/paquo
 Download-URL: https://github.com/bayer-science-for-a-better-life/paquo
 Author: Santiago Villalba, Andreas Poehlmann
 Author-email: santiago.villalba@bayer.com, andreas.poehlmann@bayer.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `paquo-0.7.2/README.md` & `paquo-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/docs/Makefile` & `paquo-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/docs/source/_static/screenshot_example_05.png` & `paquo-0.8.0/docs/source/_static/screenshot_example_05.png`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/docs/source/api.rst` & `paquo-0.8.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/docs/source/conf.py` & `paquo-0.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/docs/source/configuration.rst` & `paquo-0.8.0/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/docs/source/index.rst` & `paquo-0.8.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/docs/source/installation.rst` & `paquo-0.8.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/docs/source/quickstart.rst` & `paquo-0.8.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/environment.devenv.yml` & `paquo-0.8.0/environment.devenv.yml`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/examples/README.md` & `paquo-0.8.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/examples/example_01_read_annotations.py` & `paquo-0.8.0/examples/example_01_read_annotations.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/examples/example_02_add_annotations.py` & `paquo-0.8.0/examples/example_02_add_annotations.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/examples/example_03_project_with_classes.py` & `paquo-0.8.0/examples/example_03_project_with_classes.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/examples/example_04_project_with_image_metadata.py` & `paquo-0.8.0/examples/example_04_project_with_image_metadata.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/examples/example_05_draw_tiles_on_image.py` & `paquo-0.8.0/examples/example_05_draw_tiles_on_image.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/examples/prepare_resources.py` & `paquo-0.8.0/examples/prepare_resources.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/extras/README.md` & `paquo-0.8.0/extras/README.md`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/.paquo.defaults.toml` & `paquo-0.8.0/paquo/.paquo.defaults.toml`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/__main__.py` & `paquo-0.8.0/paquo/__main__.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/_cli.py` & `paquo-0.8.0/paquo/_cli.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/_config.py` & `paquo-0.8.0/paquo/_config.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/_logging.py` & `paquo-0.8.0/paquo/_logging.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/_repr.py` & `paquo-0.8.0/paquo/_repr.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/_utils.py` & `paquo-0.8.0/paquo/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -213,15 +213,19 @@
                 tf.extractall(tmp_dir)  # nosec: B202
                 for name in os.listdir(tmp_dir):
                     pth = os.path.join(tmp_dir, name)
                     if name.startswith("QuPath") and os.path.isdir(pth):
                         break
                 else:
                     raise RuntimeError("no qupath extracted?")
-            shutil.move(os.path.join(tmp_dir, name), qp_dst)
+            extract_dir = os.path.join(tmp_dir, name)
+            if os.path.isdir(os.path.join(extract_dir, "QuPath")):
+                # in some cases there is a nested QuPath directory
+                extract_dir = os.path.join(extract_dir, "QuPath")
+            shutil.move(extract_dir, qp_dst)
         return qp_dst
 
     elif system == "Darwin":
         if not Path(file).suffix == ".pkg":
             raise ValueError("file does not end with `.pkg`")
         if shutil.which("7z") is None:
             raise RuntimeError("7z is required, run: `brew install p7zip`")
```

### Comparing `paquo-0.7.2/paquo/classes.py` & `paquo-0.8.0/paquo/classes.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/colors.py` & `paquo-0.8.0/paquo/colors.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/hierarchy.py` & `paquo-0.8.0/paquo/hierarchy.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from paquo.java import PathObjectHierarchy
 from paquo.java import PathTileObject
 from paquo.java import String
 from paquo.java import compatibility
 from paquo.pathobjects import BaseGeometry
 from paquo.pathobjects import PathROIObjectType
 from paquo.pathobjects import QuPathPathAnnotationObject
+from paquo.pathobjects import QuPathPathCellObject
 from paquo.pathobjects import QuPathPathDetectionObject
 from paquo.pathobjects import QuPathPathTileObject
 from paquo.pathobjects import fix_geojson_geometry
 
 __all__ = ["QuPathPathObjectHierarchy"]
 
 _logger = get_logger(__name__)
@@ -54,28 +55,32 @@
     """
 
     def __init__(
         self,
         hierarchy: 'QuPathPathObjectHierarchy',
         paquo_cls: Type[PathROIObjectType],
         mask: Optional[Union[slice, Sequence[int]]] = None,
+        readonly: Optional[bool] = None,
     ) -> None:
         """internal: not meant to be instantiated by the user"""
         self._hierarchy = hierarchy
         self._paquo_cls = paquo_cls
         if not (
             mask is None
             or isinstance(mask, slice)
             or (all(isinstance(x, int) for x in mask) and len(mask) > 0)
         ):
             raise TypeError(f"mask can be slice, or Sequence[int] or None. Got: {type(mask)!r}")
         self._mask: Optional[Union[slice, Sequence[int]]] = mask
+        self._init_readonly = readonly
 
     @property
     def _readonly(self) -> bool:
+        if self._init_readonly is not None:
+            return self._init_readonly
         # noinspection PyProtectedMember
         return self._hierarchy._readonly or self._mask is not None
 
     @property
     def _java_hierarchy(self):
         return self._hierarchy.java_object
 
@@ -269,14 +274,16 @@
             hierarchy = PathObjectHierarchy()
         self.java_object = hierarchy
         # internals
         self._image_name = str(image_name)
         self._readonly = bool(readonly)
         self._annotations = PathObjectProxy(self, paquo_cls=QuPathPathAnnotationObject)
         self._detections = PathObjectProxy(self, paquo_cls=QuPathPathDetectionObject)
+        self._cells = PathObjectProxy(self, paquo_cls=QuPathPathCellObject, readonly=True)
+        self._tiles = PathObjectProxy(self, paquo_cls=QuPathPathTileObject, readonly=True)
         # attrs
         self.autoflush = bool(autoflush)
 
     def __len__(self) -> int:
         """Number of objects in hierarchy (all types)"""
         return int(self.java_object.nObjects())
 
@@ -299,14 +306,16 @@
     def flush(self, invalidate_proxy_cache: bool = False):
         """flush changes to the hierarchy"""
         root = self.java_object.getRootObject()
         self.java_object.fireHierarchyChangedEvent(root)
         if invalidate_proxy_cache:
             self._annotations._list_invalidate_cache()
             self._detections._list_invalidate_cache()
+            self._cells._list_invalidate_cache()
+            self._tiles._list_invalidate_cache()
 
     @property
     def root(self) -> QuPathPathAnnotationObject:
         """the hierarchy root node
 
         This object has no roi and cannot be assigned another class.
         All other objects are descendants of this object if they are
@@ -358,14 +367,19 @@
         obj = QuPathPathDetectionObject.from_shapely(
             roi, path_class, measurements,
             path_class_probability=path_class_probability
         )
         self._detections.add(obj)
         return obj
 
+    @property
+    def tiles(self) -> PathObjectProxy[QuPathPathTileObject]:
+        """all tiles provided as a flattened read-only set-like proxy"""
+        return self._tiles
+
     def add_tile(self,
                  roi: BaseGeometry,
                  path_class: Optional[QuPathPathClass] = None,
                  measurements: Optional[dict] = None,
                  *,
                  path_class_probability: float = math.nan) -> QuPathPathTileObject:
         """convenience method for adding tile detections
@@ -379,14 +393,42 @@
         obj = QuPathPathTileObject.from_shapely(
             roi, path_class, measurements,
             path_class_probability=path_class_probability
         )
         self._detections.add(obj)
         return obj
 
+    @property
+    def cells(self) -> PathObjectProxy[QuPathPathCellObject]:
+        """all cells provided as a flattened read-only set-like proxy"""
+        return self._cells
+
+    def add_cell(self,
+                 roi: BaseGeometry,
+                 path_class: Optional[QuPathPathClass] = None,
+                 measurements: Optional[dict] = None,
+                 *,
+                 path_class_probability: float = math.nan,
+                 nucleus_roi: BaseGeometry) -> QuPathPathCellObject:
+        """convenience method for adding cell detections
+
+        Notes
+        -----
+        these will be added to self.detections, as they are a subclass of detections
+        """
+        if self._readonly:
+            raise OSError("project in readonly mode")
+        obj = QuPathPathCellObject.from_shapely(
+            roi, path_class, measurements,
+            path_class_probability=path_class_probability,
+            nucleus_roi=nucleus_roi
+        )
+        self._detections.add(obj)
+        return obj
+
     def to_geojson(self) -> list:
         """return all annotations as a list of geojson features"""
         gson = GsonTools.getInstance()
         geojson = gson.toJson(self.java_object.getAnnotationObjects())
         return list(json.loads(str(geojson)))
 
     def load_geojson(
@@ -664,15 +706,15 @@
             if isinstance(ome_shape, list):
                 roi.union.extend(ome_shape)
             else:
                 roi.union.append(ome_shape)
 
             # --- add the annotation to the ome structure
             ome.rois.append(roi)
-            ome.structured_annotations.append(map_annotation)
+            ome.structured_annotations.append(map_annotation)  # type: ignore[union-attr]
 
         return to_xml(ome)
 
     def __repr__(self):
         return f"Hierarchy(image={self._image_name}, annotations={len(self._annotations)}, detections={len(self._detections)})"
 
     def _repr_html_(self):
```

### Comparing `paquo-0.7.2/paquo/images.py` & `paquo-0.8.0/paquo/images.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/java.py` & `paquo-0.8.0/paquo/java.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 
 PathDetectionObject = JClass("qupath.lib.objects.PathDetectionObject")
 PathIO = JClass("qupath.lib.io.PathIO")
 PathObjectHierarchy = JClass('qupath.lib.objects.hierarchy.PathObjectHierarchy')
 PathObjects = JClass("qupath.lib.objects.PathObjects")
 PathROIObject = JClass("qupath.lib.objects.PathROIObject")
 PathTileObject = JClass("qupath.lib.objects.PathTileObject")
+PathCellObject = JClass("qupath.lib.objects.PathCellObject")
 Point2 = JClass("qupath.lib.geom.Point2")
 ProjectIO = JClass('qupath.lib.projects.ProjectIO')
 Projects = JClass('qupath.lib.projects.Projects')
 ROI = JClass("qupath.lib.roi.interfaces.ROI")
 ROIs = JClass("qupath.lib.roi.ROIs")
 ServerTools = JClass('qupath.lib.images.servers.ServerTools')
```

### Comparing `paquo-0.7.2/paquo/jpype_backend.py` & `paquo-0.8.0/paquo/jpype_backend.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/pathobjects.py` & `paquo-0.8.0/paquo/pathobjects.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from paquo._utils import cached_property
 from paquo.classes import QuPathPathClass
 from paquo.java import ROI
 from paquo.java import GeometryTools
 from paquo.java import GsonTools
 from paquo.java import PathAnnotationObject
+from paquo.java import PathCellObject
 from paquo.java import PathDetectionObject
 from paquo.java import PathObjects
 from paquo.java import PathROIObject
 from paquo.java import PathTileObject
 from paquo.java import String
 from paquo.java import WKBReader
 from paquo.java import WKBWriter
@@ -31,14 +32,15 @@
 __all__ = [
     "fix_geojson_geometry",
     "BaseGeometry",
     "PathROIObjectType",
     "QuPathPathAnnotationObject",
     "QuPathPathDetectionObject",
     "QuPathPathTileObject",
+    "QuPathPathCellObject",
 ]
 
 
 def _shapely_geometry_to_qupath_roi(geometry: BaseGeometry, image_plane=None) -> ROI:
     """convert a shapely geometry into a qupath ROI
 
     uses well known binary WKB as intermediate representation
@@ -157,15 +159,15 @@
 
     @classmethod
     def from_shapely(cls: Type[PathROIObjectType],
                      roi: BaseGeometry,
                      path_class: Optional[QuPathPathClass] = None,
                      measurements: Optional[dict] = None,
                      *,
-                     path_class_probability: float = math.nan) -> PathROIObjectType:
+                     path_class_probability: float = math.nan) -> "PathROIObjectType":
         """create a Path Object from a shapely shape
 
         Parameters
         ----------
         roi:
             a shapely shape as the region of interest of the annotation
         path_class:
@@ -374,7 +376,61 @@
     java_class_factory = PathObjects.createDetectionObject
 
 
 class QuPathPathTileObject(QuPathPathDetectionObject):
 
     java_class = PathTileObject
     java_class_factory = PathObjects.createTileObject
+
+
+class QuPathPathCellObject(QuPathPathDetectionObject):
+
+    java_class = PathCellObject
+    java_class_factory = PathObjects.createCellObject
+
+    @property
+    def nucleus_roi(self) -> BaseGeometry:
+        """the nucleus roi as a shapely shape"""
+        roi = self.java_object.getNucleusROI()
+        return _qupath_roi_to_shapely_geometry(roi)
+
+    @classmethod
+    def from_shapely(cls,
+                     roi: BaseGeometry,
+                     path_class: Optional[QuPathPathClass] = None,
+                     measurements: Optional[dict] = None,
+                     *,
+                     path_class_probability: float = math.nan,
+                     nucleus_roi: Optional[BaseGeometry] = None) -> "QuPathPathCellObject":
+        """create a Path Object from a shapely shape
+
+        Parameters
+        ----------
+        roi:
+            a shapely shape as the region of interest of the annotation
+        path_class:
+            a paquo QuPathPathClass to mark the annotation type
+        measurements:
+            dict holding static measurements for annotation object
+        path_class_probability:
+            keyword only argument defining the probability of the class
+            (default NaN)
+        nucleus_roi:
+            a roi for a nucleus
+
+        """
+        if not isinstance(roi, BaseGeometry):
+            raise TypeError("roi needs to be an instance of shapely.geometry.base.BaseGeometry")
+        if not isinstance(nucleus_roi, BaseGeometry):
+            raise TypeError("nucleus_roi needs to be an instance of shapely.geometry.base.BaseGeometry")
+
+        qupath_path_class = path_class.java_object if path_class is not None else None
+        qupath_roi = _shapely_geometry_to_qupath_roi(roi)
+        qupath_additional_roi = _shapely_geometry_to_qupath_roi(nucleus_roi)
+        java_obj = cls.java_class_factory(qupath_roi, qupath_additional_roi, qupath_path_class, None)
+
+        if not math.isnan(path_class_probability):
+            java_obj.setPathClass(java_obj.getPathClass(), path_class_probability)
+        obj = cls(java_obj)
+        if measurements is not None:
+            obj.measurements.update(measurements)
+        return obj
```

### Comparing `paquo-0.7.2/paquo/projects.py` & `paquo-0.8.0/paquo/projects.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/tests/conftest.py` & `paquo-0.8.0/paquo/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/tests/test_classes.py` & `paquo-0.8.0/paquo/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/tests/test_colors.py` & `paquo-0.8.0/paquo/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/tests/test_config.py` & `paquo-0.8.0/paquo/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/tests/test_hierarchy.py` & `paquo-0.8.0/paquo/tests/test_hierarchy.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,18 @@
     )
     empty_hierarchy.add_detection(
         roi=shapely.geometry.Polygon.from_bounds(0, 0, 5, 5)
     )
     empty_hierarchy.add_tile(
         roi=shapely.geometry.Polygon.from_bounds(0, 0, 5, 5)
     )
-
+    empty_hierarchy.add_cell(
+        roi=shapely.geometry.Polygon.from_bounds(0, 0, 5, 5),
+        nucleus_roi=shapely.geometry.Polygon.from_bounds(1.25, 1.25, 3.75, 3.75)
+    )
 
 def test_attach_detections(empty_hierarchy):
     h = empty_hierarchy
     detections = _make_polygon_detections(10)
 
     # add many
     h.detections.update(detections)
@@ -103,14 +106,29 @@
     detections = _make_polygon_detections(7)
     h.annotations.update(annotations)
     h.detections.update(detections)
     assert len(h.annotations) == 5
     assert len(h.detections) == 7
 
 
+def test_add_cells(empty_hierarchy):
+    h = empty_hierarchy
+    roi = shapely.geometry.Polygon.from_bounds(0, 0, 5, 5)
+    nucleus_roi = shapely.geometry.Polygon.from_bounds(1, 1, 4, 4)
+
+    h.add_cell(roi=roi, nucleus_roi=nucleus_roi)
+
+    assert len(h.detections) == 1
+    assert len(h.cells) == 1
+
+    cell = h.cells[0]
+    assert shapely.equals(cell.roi, roi)
+    assert shapely.equals(cell.nucleus_roi, nucleus_roi)
+
+
 def test_geojson_roundtrip_via_geojson(empty_hierarchy):
     h = empty_hierarchy
     annotations = _make_polygon_annotations(10)
 
     h.annotations.update(annotations)
     assert len(h) == len(annotations)
     geojson = h.to_geojson()
```

### Comparing `paquo-0.7.2/paquo/tests/test_images.py` & `paquo-0.8.0/paquo/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/tests/test_jpype_backend.py` & `paquo-0.8.0/paquo/tests/test_jpype_backend.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/tests/test_main.py` & `paquo-0.8.0/paquo/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/tests/test_pathobjects.py` & `paquo-0.8.0/paquo/tests/test_pathobjects.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 import shapely.geometry
 from shapely import Polygon
 
 from paquo._utils import QuPathVersion
 from paquo.classes import QuPathPathClass
-from paquo.pathobjects import QuPathPathAnnotationObject
+from paquo.pathobjects import QuPathPathAnnotationObject, QuPathPathCellObject
 from paquo.projects import QuPathProject
 
 
 def test_qupath_to_shapely_conversion():
     from paquo.java import ROIs
     from paquo.pathobjects import _qupath_roi_to_shapely_geometry
     from shapely.geometry import Point
@@ -150,14 +150,36 @@
 
     # repr
     ao.name = "abc"
     ao.update_path_class(QuPathPathClass('myclass'))
     assert repr(ao)
 
 
+def test_pathcellobject():
+
+    roi = shapely.geometry.Polygon.from_bounds(10, 20, 100, 200)
+    nucleus_roi = shapely.geometry.Polygon.from_bounds(14, 26, 90, 190)
+
+    with pytest.raises(TypeError):
+        # noinspection PyTypeChecker
+        QuPathPathCellObject.from_shapely(roi=123, nucleus_roi=123)
+    with pytest.raises(TypeError):
+        # noinspection PyTypeChecker
+        QuPathPathCellObject.from_shapely(roi=roi)
+
+    cell = QuPathPathCellObject.from_shapely(
+        roi,
+        path_class=QuPathPathClass('myclass'),
+        nucleus_roi=nucleus_roi,
+    )
+
+    assert shapely.equals(cell.roi, roi)
+    assert shapely.equals(cell.nucleus_roi, nucleus_roi)
+
+
 def test_measurements():
     ao = QuPathPathAnnotationObject.from_shapely(
         shapely.geometry.Point(1, 1),
         path_class=QuPathPathClass('myclass'),
         measurements={'measurement1': 1.23},
         path_class_probability=0.5,
     )
```

### Comparing `paquo-0.7.2/paquo/tests/test_projects.py` & `paquo-0.8.0/paquo/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo/tests/test_readonly.py` & `paquo-0.8.0/paquo/tests/test_readonly.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,16 @@
         with pytest.raises(IOError):
             h.callmethod("add_annotation", '--placeholder--')
         with pytest.raises(IOError):
             h.callmethod("add_detection", '--placeholder--')
         with pytest.raises(IOError):
             h.callmethod("add_tile", '--placeholder--')
         with pytest.raises(IOError):
+            h.callmethod("add_cell", '--placeholder--', nucleus_roi='--placeholder--')
+        with pytest.raises(IOError):
             h.callmethod("load_geojson", '--placeholder--')
 
         # autoflush has no influence
         h.setattr("autoflush", False)
         h.callmethod("no_autoflush")
         h.callmethod("flush")
```

### Comparing `paquo-0.7.2/paquo/tests/test_repr.py` & `paquo-0.8.0/paquo/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/paquo.egg-info/PKG-INFO` & `paquo-0.8.0/paquo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paquo
-Version: 0.7.2
+Version: 0.8.0
 Summary: library for interacting with QuPath
 Home-page: https://github.com/bayer-science-for-a-better-life/paquo
 Download-URL: https://github.com/bayer-science-for-a-better-life/paquo
 Author: Santiago Villalba, Andreas Poehlmann
 Author-email: santiago.villalba@bayer.com, andreas.poehlmann@bayer.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `paquo-0.7.2/paquo.egg-info/SOURCES.txt` & `paquo-0.8.0/paquo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 CHANGELOG.md
 CODEOWNERS
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 environment.devenv.yml
+environment.yml
 pyproject.toml
 setup.cfg
 docs/Makefile
 docs/source/api.rst
 docs/source/conf.py
 docs/source/configuration.rst
 docs/source/index.rst
@@ -35,14 +36,15 @@
 paquo/_config.py
 paquo/_logging.py
 paquo/_repr.py
 paquo/_utils.py
 paquo/_version.py
 paquo/classes.py
 paquo/colors.py
+paquo/environment.yml
 paquo/hierarchy.py
 paquo/images.py
 paquo/java.py
 paquo/jpype_backend.py
 paquo/pathobjects.py
 paquo/projects.py
 paquo/py.typed
```

### Comparing `paquo-0.7.2/pyproject.toml` & `paquo-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `paquo-0.7.2/setup.cfg` & `paquo-0.8.0/setup.cfg`

 * *Files identical despite different names*

