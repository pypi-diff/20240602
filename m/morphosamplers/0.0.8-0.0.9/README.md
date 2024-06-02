# Comparing `tmp/morphosamplers-0.0.8.tar.gz` & `tmp/morphosamplers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphosamplers-0.0.8.tar", last modified: Fri May  5 12:07:40 2023, max compression
+gzip compressed data, was "morphosamplers-0.0.9.tar", last modified: Mon Oct 23 17:27:50 2023, max compression
```

## Comparing `morphosamplers-0.0.8.tar` & `morphosamplers-0.0.9.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.179931 morphosamplers-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.179931 morphosamplers-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.179931 morphosamplers-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/examples/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/examples/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.179931 morphosamplers-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.179931 morphosamplers-0.0.8/src/morphosamplers/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/models/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/models/sphere.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/models/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/sample_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/point_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/pose_sampler_helical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/pose_sampler_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/test_point_sampler_equidistant.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_helical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/_sphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/point_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/pose_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/tests/test_point_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)    19179 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/surface_spline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/src/morphosamplers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/src/morphosamplers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-05 12:07:40.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-05 12:07:40.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:07:40.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:07:39.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 12:07:40.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 12:07:40.000000 morphosamplers-0.0.8/src/morphosamplers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:07:40.183931 morphosamplers-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/tests/test_spline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 12:07:23.000000 morphosamplers-0.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.693589 morphosamplers-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.681589 morphosamplers-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.681589 morphosamplers-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/.github_changelog_generator
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2023-10-23 17:27:50.693589 morphosamplers-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.681589 morphosamplers-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/examples/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/examples/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-23 17:27:50.693589 morphosamplers-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.677589 morphosamplers-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.685589 morphosamplers-0.0.9/src/morphosamplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/helical_filament.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.689589 morphosamplers-0.0.9/src/morphosamplers/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/models/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/models/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/sample_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10539 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.689589 morphosamplers-0.0.9/src/morphosamplers/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.689589 morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/point_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/pose_sampler_helical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/pose_sampler_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.689589 morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/tests/test_point_sampler_equidistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_helical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.689589 morphosamplers-0.0.9/src/morphosamplers/samplers/sphere_samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/sphere_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/sphere_samplers/_sphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/sphere_samplers/point_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/sphere_samplers/pose_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.689589 morphosamplers-0.0.9/src/morphosamplers/samplers/sphere_samplers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/samplers/sphere_samplers/tests/test_point_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11371 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19606 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/surface_spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10013 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/src/morphosamplers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.685589 morphosamplers-0.0.9/src/morphosamplers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2023-10-23 17:27:50.000000 morphosamplers-0.0.9/src/morphosamplers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-10-23 17:27:50.000000 morphosamplers-0.0.9/src/morphosamplers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 17:27:50.000000 morphosamplers-0.0.9/src/morphosamplers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 17:27:50.000000 morphosamplers-0.0.9/src/morphosamplers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-23 17:27:50.000000 morphosamplers-0.0.9/src/morphosamplers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-23 17:27:50.000000 morphosamplers-0.0.9/src/morphosamplers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 17:27:50.689589 morphosamplers-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/tests/test_spline_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2023-10-23 17:27:28.000000 morphosamplers-0.0.9/tox.ini
```

### Comparing `morphosamplers-0.0.8/.cruft.json` & `morphosamplers-0.0.9/.cruft.json`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/.github/workflows/ci.yml` & `morphosamplers-0.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/.github/workflows/cron.yml` & `morphosamplers-0.0.9/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/.gitignore` & `morphosamplers-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/.pre-commit-config.yaml` & `morphosamplers-0.0.9/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -3,50 +3,50 @@
   autofix_commit_msg: "style: [pre-commit.ci] auto fixes [...]"
   autoupdate_commit_msg: "ci: [pre-commit.ci] autoupdate"
 
 default_install_hook_types: [pre-commit, commit-msg]
 
 repos:
   - repo: https://github.com/compilerla/conventional-pre-commit
-    rev: v1.3.0
+    rev: v2.4.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.5.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/myint/autoflake
-    rev: v1.4
+    rev: v2.2.1
     hooks:
       - id: autoflake
         args: ["--in-place", "--remove-all-unused-imports"]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.34.0
+    rev: v3.15.0
     hooks:
       - id: pyupgrade
         args: [--py38-plus, --keep-runtime-typing]
 
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.9.1
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    rev: 6.1.0
     hooks:
       - id: flake8
         args:
           - "--max-line-length=88"
         additional_dependencies:
           - flake8-pyproject
           - flake8-bugbear
```

### Comparing `morphosamplers-0.0.8/LICENSE` & `morphosamplers-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/README.md` & `morphosamplers-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/examples/path.py` & `morphosamplers-0.0.9/examples/path.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/examples/sphere.py` & `morphosamplers-0.0.9/examples/sphere.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/pyproject.toml` & `morphosamplers-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.10",
 ]
 dynamic = ["version"]
 dependencies = [
     "einops",
     "numpy",
     "psygnal",
-    "pydantic",
+    "pydantic<2",
     "scipy",
     "typing-extensions"
 ]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
@@ -90,24 +90,35 @@
 src_paths = ["src/morphosamplers", "tests"]
 
 # https://flake8.pycqa.org/en/latest/user/options.html
 # https://gitlab.com/durko/flake8-pyprojecttoml
 [tool.flake8]
 exclude = "docs,.eggs,examples,_version.py"
 max-line-length = 88
-ignore = "E203"
 min-python-version = "3.8.0"
 docstring-convention = "all" # use numpy convention, while allowing D417
-extend-ignore = """
-E203  # whitespace before ':'
-D107,D203,D212,D213,D402,D413,D415,D416  # numpy
-D100  # missing docstring in public module
-D401  # imperative mood
-W503  # line break before binary operator
-"""
+ignore = [
+    # whitespace before ':'
+    "E203",
+    # numpy
+    "D107",
+    "D203",
+    "D212",
+    "D213",
+    "D402",
+    "D413",
+    "D415",
+    "D416",
+    # missing docstring in public module
+    "D100",
+    # imperative mood
+    "D401",
+    # line break before binary operator
+    "W503",
+]
 per-file-ignores = [
     "tests/*:D",
 ]
 
 
 # http://www.pydocstyle.org/en/stable/usage.html
 [tool.pydocstyle]
```

### Comparing `morphosamplers-0.0.8/src/morphosamplers/core.py` & `morphosamplers-0.0.9/src/morphosamplers/core.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/models/path.py` & `morphosamplers-0.0.9/src/morphosamplers/models/path.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/models/surface.py` & `morphosamplers-0.0.9/src/morphosamplers/models/surface.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/sample_types.py` & `morphosamplers-0.0.9/src/morphosamplers/sample_types.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/sampler.py` & `morphosamplers-0.0.9/src/morphosamplers/sampler.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/point_sampler.py` & `morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/point_sampler.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/pose_sampler_helical.py` & `morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/pose_sampler_helical.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/pose_sampler_parallel.py` & `morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/pose_sampler_parallel.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/test_point_sampler_equidistant.py` & `morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/tests/test_point_sampler_equidistant.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_parallel.py` & `morphosamplers-0.0.9/src/morphosamplers/samplers/path_samplers/tests/test_pose_sampler_parallel.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/_sphere_utils.py` & `morphosamplers-0.0.9/src/morphosamplers/samplers/sphere_samplers/_sphere_utils.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/pose_sampler.py` & `morphosamplers-0.0.9/src/morphosamplers/samplers/sphere_samplers/pose_sampler.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/samplers/sphere_samplers/tests/test_point_sampler.py` & `morphosamplers-0.0.9/src/morphosamplers/samplers/sphere_samplers/tests/test_point_sampler.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/spline.py` & `morphosamplers-0.0.9/src/morphosamplers/spline.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/src/morphosamplers/surface_spline.py` & `morphosamplers-0.0.9/src/morphosamplers/surface_spline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,89 @@
 """Tooling to fit and sample surfaces."""
 
-from typing import List, Tuple, Optional, Union
 import warnings
+from typing import List, Optional, Tuple, Union
 
-import numpy as np
 import einops
+import numpy as np
 from psygnal import EventedModel
-from pydantic import PrivateAttr, conint, validator, root_validator
+from pydantic import PrivateAttr, conint, root_validator, validator
 from scipy.interpolate import splev, splprep
 from scipy.spatial.transform import Rotation
 
 from .spline import Spline3D
 from .utils import (
+    estimate_point_row_directions,
     extrapolate_point_rows_with_derivatives,
+    minimize_closed_point_row_pair_distance,
     minimize_point_row_pair_distance,
-    minimize_closed_point_strips_pair_distance,
-    estimate_point_row_directions,
 )
 
 
 class _SplineSurface(EventedModel):
     """Surface model based on splines."""
 
     points: List[np.ndarray]
     separation: float
     order: conint(ge=1, le=5) = 3
     smoothing: Optional[int] = None
     closed: bool = False
     inside_point: Optional[Union[np.ndarray, Tuple[float, float, float]]] = None
+    oversampling: int = 2
     _row_splines = PrivateAttr(List[Spline3D])
     _column_splines = PrivateAttr(List[Spline3D])
-    _oversampling_ratio = 10
 
     class Config:
         """Pydantic BaseModel configuration."""
 
         arbitrary_types_allowed = True
 
-    @validator('points')
+    @validator("points")
     def _validate_number_of_splines(v):
         points = np.atleast_2d(*v)
         if len(points) < 2:
-            raise ValueError('At least 2 arrays of points are necessary to define a surface.')
+            raise ValueError(
+                "At least 2 arrays of points are necessary to define a surface."
+            )
         return points
 
     @root_validator(skip_on_failure=True)
     def _validate_number_of_lines(cls, values):
-        points = values.get('points')
+        points = values.get("points")
         n_lines = len(points)
-        order = values.get('order')
+        order = values.get("order")
 
         # order needs to be reduced if it does not match the number of splines
         if order is not None and n_lines <= order:
             new_order = n_lines - 1
             warnings.warn(
-                f'Too few arrays of points for interpolation of order {order}. '
-                f'Decreasing order to {new_order} for interpolation between lines.'
+                f"Too few arrays of points for interpolation of order {order}. "
+                f"Decreasing order to {new_order} for interpolation between lines."
             )
             # we don't decrease the order here so we can still attempt to use the full
             # interpolation for individual splines, so we do it in _generate_column_splines
 
         return values
 
     def __init__(self, **kwargs):
         """Calculate the splines after validating the paramters."""
         super().__init__(**kwargs)
         self._prepare_splines()
 
     def __setattr__(self, name, value):
         super().__setattr__(name, value)
-        if name in ("points", "separation", "order", "closed"):
+        if name in ("points", "separation", "order", "closed", "oversampling"):
             self._prepare_splines()
 
     def _prepare_splines(self):
         self._generate_row_splines()
         self._generate_column_splines()
 
     @classmethod
-    def _fix_spline_edges(cls, splines, separation, order, closed):
+    def _fix_spline_edges(cls, splines, separation, order, closed, oversampling):
         """
         Generate new control points for each spline to ensure a minimally deformed grid.
 
         For open surfaces, splines are sampled with the same equidistance, and the resulting
         rows of points are then padded with NaNs at each end so that:
         - they have the same amount of samples
         - mean distance between samples at the same index in neighboring rows is minimised
@@ -89,81 +91,96 @@
         derivative.
 
         For closed surfaces, since they cannot be extended, each spline is sampled with the same
         number of points, which may result in a deformed grid. Each row is then aligned to minimise
         shear by minimising the mean distance between samples at the same intex in neighboring rows.
         """
         # sample splines to get equidistant points on z slices
-        separation = separation / cls._oversampling_ratio
+        separation = separation / oversampling
         us = [
-            spline._get_equidistant_spline_coordinate_values(separation=separation, approximate=True)
+            spline._get_equidistant_spline_coordinate_values(
+                separation=separation, approximate=True
+            )
             for spline in splines
         ]
 
         if closed:
             # We need the same amount of samples on each row to make a rectangular grid,
             # but we can't extend/pad a closed surface, so instead we take n_samples from each
             # so that on average we get a good approximation of the given separation
             n_points = [len(u) for u in us]
             diff = np.max(n_points) - np.min(n_points)
             if diff > 1:
-                warnings.warn('The grid is deformed by more than 1 separation in some places. '
-                              'This is inevitable with closed, non-cylindrical grids.')
+                warnings.warn(
+                    "The grid is deformed by more than 1 separation in some places. "
+                    "This is inevitable with closed, non-cylindrical grids."
+                )
             best_n = round(np.mean(n_points))
 
             points = [spline.sample(n_samples=best_n) for spline, u in zip(splines, us)]
 
-            points = minimize_closed_point_strips_pair_distance(points, expected_dist=separation)
+            points = minimize_closed_point_row_pair_distance(
+                points, expected_dist=separation
+            )
             masks = [np.ones(len(p), dtype=bool) for p in points]
         else:
             points = [spline.sample(u) for spline, u in zip(splines, us)]
             derivatives = [
-                spline.sample(u, derivative_order=1)
-                for spline, u in zip(splines, us)
+                spline.sample(u, derivative_order=1) for spline, u in zip(splines, us)
             ]
 
             # flip directions of annotations if necessary
             directions = estimate_point_row_directions(points)
             # coordinates can be simply inverted
             points = [pts[::dir] for pts, dir in zip(points, directions)]
             # directions need to be inverted *and* flipped (since they are a vector)
-            derivatives = [der[::dir] * dir for der, dir in zip(derivatives, directions)]
+            derivatives = [
+                der[::dir] * dir for der, dir in zip(derivatives, directions)
+            ]
 
             # extrapolate where nans are present by extending along the spline direction
             points = minimize_point_row_pair_distance(points, expected_dist=separation)
 
             masks = [~np.isnan(p[:, 0]) for p in points]  # just one dim is enough
             points = extrapolate_point_rows_with_derivatives(
                 points, derivatives, separation
             )
 
         return points, masks
 
     def _generate_row_splines(self):
         self._row_splines = [
-            Spline3D(points=p, order=self.order, smoothing=self.smoothing, closed=self.closed)
+            Spline3D(
+                points=p, order=self.order, smoothing=self.smoothing, closed=self.closed
+            )
             for p in self.points
         ]
 
     def _generate_column_splines(self):
         # fix edge artifacts by extending splines until we have a grid
-        control_points, masks = self._fix_spline_edges(self._row_splines, self.separation, self.order, self.closed)
+        control_points, masks = self._fix_spline_edges(
+            self._row_splines,
+            self.separation,
+            self.order,
+            self.closed,
+            self.oversampling,
+        )
 
         if self.closed:
             # _fix_spline_edges returns strips including the extrema, so we need to remove
             # one of them if the surface is closed to avoid duplication
             control_points = [p[:-1] for p in control_points]
 
         # _fix_spline_edges oversamples to avoid artifacts, so we only take every N points
-        control_points = np.stack(control_points)[:, ::self._oversampling_ratio]
-        masks = np.stack(masks)[:, ::self._oversampling_ratio]
+        control_points = np.stack(control_points)[:, ::self.oversampling]
+        masks = np.stack(masks)[:, ::self.oversampling]
 
         # stack points in the other direction, so we get the column-splines
-        stacked = einops.rearrange(control_points, 'row column xyz -> column row xyz')
-        masks_stacked = einops.rearrange(masks, 'row column -> column row')
+        stacked = einops.rearrange(control_points, "row column xyz -> column row xyz")
+        masks_stacked = einops.rearrange(masks, "row column -> column row")
 
         # order needs to be reduced if it does not match the number of splines
         if len(self.points) <= self.order:
             order = len(self.points) - 1
         else:
             order = self.order
 
@@ -188,34 +205,37 @@
     def grid_shape(self):
         return (len(self._grid_splines), len(self._grid_meta_splines))
 
     def _generate_grid_splines(self):
         # we finally create grid-like splines with optimized spacing
         # though not optimal for consistent spacing, we have to use the same n
         # for each spline, otherwise we end up with offset points in each lines
+        separation = self.separation / self.oversampling
         us = [
             spline._get_equidistant_spline_coordinate_values(
-                separation=self.separation,
-                approximate=True
+                separation=separation, approximate=True
             )
             for spline in self._column_splines
         ]
         n_points = [len(u) for u in us]
         diff = np.max(n_points) - np.min(n_points)
         if diff > 1:
-            warnings.warn('The grid is deformed by more than 1 separation in some places. '
-                          'Consider passing points that belong to parallel planes, or splitting '
-                          'the surface in quasi-planar patches.')
+            warnings.warn(
+                "The grid is deformed by more than 1 separation in some places. "
+                "Consider passing points that belong to parallel planes, or splitting "
+                "the surface in quasi-planar patches."
+            )
         best_n = int(round(np.mean(n_points)))
         u = np.linspace(0, 1, best_n)
         # TODO: actually use non-approximate linspace (with remainder) so we get as close as possible to
         #       a real grid. The problem with this is that we won't reach exactly the last spline
 
-        equidistant_points = [spline.sample(u) for spline in self._column_splines]
-        masks = [spline.get_mask_for_u(u) for spline in self._column_splines]
+        equidistant_points = [spline.sample(u)[::self.oversampling] for spline in self._column_splines]
+        masks = [spline.get_mask_for_u(u)[::self.oversampling] for spline in self._column_splines]
+
         self._mask = np.concatenate(np.stack(masks, axis=1))
 
         # these last splines should not be oversampled, because we want exact
         # positions for our knots, which we save in self._meta_meta_splines_u
         splines = []
         for p in np.stack(equidistant_points, axis=1):
             splines.append(splprep(p.T, s=0, k=self.order))
@@ -234,15 +254,15 @@
         Samples are optimized for consistent separation and grid-like ordering, which
         results in many discarded edges if the input differs a lot from a rectangle.
 
         The sampled array has shape (rows * columns, 3) for a grid of shape
         (rows, columns) and follows the (rows, columns) order.
         """
         equidistant_points = [
-            einops.rearrange(splev(u, tck), 'xyz column -> column xyz')
+            einops.rearrange(splev(u, tck), "xyz column -> column xyz")
             for tck, u in self._grid_splines
         ]
         return np.concatenate(equidistant_points)
 
     @property
     def mask(self):
         return self._mask
@@ -251,24 +271,24 @@
         """Sample an approximately equidistant grid of orientations on the surface.
 
         Follows the same pattern as GriddedSplineSurface.sample(). Orientations are
         generated so that the basis z vector is aligned to the surface normal, while
         x and y vectors are aligned to the row and column splines respectively.
         """
         equidistant_x_vecs = [
-            einops.rearrange(splev(u, tck, der=1), 'xyz column -> column xyz')
+            einops.rearrange(splev(u, tck, der=1), "xyz column -> column xyz")
             for tck, u in self._grid_splines
         ]
         equidistant_y_vecs = [
-            einops.rearrange(splev(u, tck, der=1), 'xyz row -> row xyz')
+            einops.rearrange(splev(u, tck, der=1), "xyz row -> row xyz")
             for tck, u in self._grid_meta_splines
         ]
 
-        x = einops.rearrange(equidistant_x_vecs, 'row column xyz -> (row column) xyz')
-        y = einops.rearrange(equidistant_y_vecs, 'column row xyz -> (row column) xyz')
+        x = einops.rearrange(equidistant_x_vecs, "row column xyz -> (row column) xyz")
+        y = einops.rearrange(equidistant_y_vecs, "column row xyz -> (row column) xyz")
 
         y /= np.linalg.norm(y, axis=1, keepdims=True)
         x /= np.linalg.norm(x, axis=1, keepdims=True)
 
         z = np.cross(x, y)
         z /= np.linalg.norm(z, axis=1, keepdims=True)
 
@@ -348,31 +368,38 @@
         super()._prepare_splines()
         self._generate_offset_splines()
 
     def _generate_offset_splines(self):
         # we finally create grid-like splines with optimized spacing
         # though not optimal for consistent spacing, we have to use the same n
         # for each spline, otherwise we end up with offset points in each lines
-        us = [spline._get_equidistant_spline_coordinate_values(separation=self.separation, approximate=True) for spline in self._column_splines]
+        separation = self.separation / self.oversampling
+        us = [
+            spline._get_equidistant_spline_coordinate_values(
+                separation=separation, approximate=True
+            )
+            for spline in self._column_splines
+        ]
         best_n = int(np.mean([len(u) for u in us]))
 
         us = []
         for i, spline in enumerate(self._column_splines):
             if i % 2:
                 us.append(np.linspace(0, 1, best_n))
             else:
                 offset = self.separation / spline._length / 2
                 us.append(np.linspace(offset, 1 - offset, best_n - 1))
 
         equidistant_points = [
-            spline.sample(u)
-            for spline, u in zip(self._column_splines, us)
+            spline.sample(u)[::self.oversampling] for spline, u in zip(self._column_splines, us)
         ]
 
-        masks = [spline.get_mask_for_u(u) for spline, u in zip(self._column_splines, us)]
+        masks = [
+            spline.get_mask_for_u(u)[::self.oversampling] for spline, u in zip(self._column_splines, us)
+        ]
         masks_even = np.concatenate(np.stack(masks[::2], axis=1))
         masks_odd = np.concatenate(np.stack(masks[1::2], axis=1))
         self._mask = np.concatenate([masks_even, masks_odd])
 
         # alternate each row spline to have points on same level
         splines_even = []
         for p in np.stack(equidistant_points[::2], axis=1):
@@ -398,18 +425,15 @@
         """Sample an approximately equidistant grid of points on the surface.
 
         Samples are optimized for consistent separation and grid-like ordering, which
         results in many discarded edges if the input differs a lot from a rectangle.
         """
         pts = []
         for splines in (self._row_splines_even, self._row_splines_odd):
-            equidistant_points = [
-                np.stack(splev(u, tck), axis=1)
-                for tck, u in splines
-            ]
+            equidistant_points = [np.stack(splev(u, tck), axis=1) for tck, u in splines]
             pts.append(np.concatenate(equidistant_points))
         return np.concatenate(pts)
 
     @property
     def mask(self):
         return self._mask
 
@@ -417,25 +441,23 @@
         """Sample an approximately equidistant grid of orientations on the surface."""
         rots = []
         for splines, meta_splines in (
             (self._row_splines_even, self._column_splines_even),
             (self._row_splines_odd, self._column_splines_odd),
         ):
             equidistant_x_vecs = [
-                np.stack(splev(u, tck, der=1), axis=1)
-                for tck, u in splines
+                np.stack(splev(u, tck, der=1), axis=1) for tck, u in splines
             ]
             equidistant_y_vecs = [
-                np.stack(splev(u, tck, der=1), axis=1)
-                for tck, u in meta_splines
+                np.stack(splev(u, tck, der=1), axis=1) for tck, u in meta_splines
             ]
 
             x = np.concatenate(equidistant_x_vecs)
             # y vectors are generated on column-by-column basis, so we need to swap axes
-            y = einops.rearrange(equidistant_y_vecs, 'column row xyz-> row column xyz')
+            y = einops.rearrange(equidistant_y_vecs, "column row xyz-> row column xyz")
             y = np.concatenate(equidistant_y_vecs)
 
             x /= np.linalg.norm(x, axis=1, keepdims=True)
             y /= np.linalg.norm(y, axis=1, keepdims=True)
 
             z = np.cross(x, y)
             z /= np.linalg.norm(z, axis=1, keepdims=True)
```

### Comparing `morphosamplers-0.0.8/src/morphosamplers/utils.py` & `morphosamplers-0.0.9/src/morphosamplers/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Utility functions."""
 
-from typing import Tuple, Union
 import warnings
+from typing import Tuple, Union
 
 import numpy as np
 from scipy.spatial import KDTree
 
 
 def _project_vector_onto_plane(vector, plane_normal):
     """Project vector onto a plane defined by its normal.
@@ -19,15 +19,19 @@
     proj_plane = vector - normal_component * plane_normal
     proj_plane /= np.linalg.norm(proj_plane)
     return proj_plane
 
 
 def coaxial_y_vectors_from_z_vectors(
     z: np.ndarray,
-    initial_y_vector: Union[np.ndarray, Tuple[float, float, float]] = (0.3234, 0.6543, 0.978),
+    initial_y_vector: Union[np.ndarray, Tuple[float, float, float]] = (
+        0.3234,
+        0.6543,
+        0.978,
+    ),
 ) -> np.ndarray:
     """Calculate y vectors starting from z vectors.
 
     This function will return the set of unit vectors perpendicular to the z-vectors
     which are maximally coaxial to their neighbours. It assumes that z vectors (n, 3)
     vary smoothly with increasing n.
 
@@ -47,17 +51,19 @@
     """
     # normalise z vectors and initialise y
     z = z.copy()
     z /= np.linalg.norm(z, axis=1, keepdims=True)
     y = np.empty((len(z), 3))
 
     if np.dot(initial_y_vector, z[0]) == 1:
-        raise ValueError('cannot generate y vectors because the provided initial_y_vector '
-                         'and the first z vector are perfectly aligned.')
-    # normalise initial y vector so that the subsequent dot product is a projection
+        raise ValueError(
+            "cannot generate y vectors because the provided initial_y_vector "
+            "and the first z vector are perfectly aligned."
+        )
+    # normalise initial y vector so that dot product is the projection
     initial_y_vector = initial_y_vector / np.linalg.norm(initial_y_vector)
 
     # initialise first y
     y[0] = _project_vector_onto_plane(initial_y_vector, z[0])
 
     # update y vectors in order
     for i in range(len(y) - 1):
@@ -87,29 +93,32 @@
         mask = np.ones(len(coords), np.bool)
         mask[biggest[1:]] = False
         coords = coords[mask]
 
     return coords
 
 
-def minimize_closed_point_strips_pair_distance(strips, expected_dist=None):
+def minimize_closed_point_row_pair_distance(strips, expected_dist=None):
     # assume closed, circular strips with equal length
     result = [strips[0]]
     ln = len(strips[0])
     for arr, next in zip(strips, strips[1:]):
         best_dist = None
         for i in range(ln):
             next_rolled = np.roll(next, i, axis=0)
             roll_dist = np.linalg.norm(arr - next, axis=1)
             avg_dist = np.mean(roll_dist)
             if best_dist is None or avg_dist < best_dist:
                 best_dist = avg_dist
                 best_arr = next_rolled
         if expected_dist is not None and best_dist >= expected_dist * np.sqrt(2):
-            warnings.warn('The grid is sheared by more than 1 separation in some places', stacklevel=2)
+            warnings.warn(
+                "The grid is sheared by more than 1 separation in some places",
+                stacklevel=2,
+            )
         result.append(best_arr)
     return result
 
 
 def estimate_point_row_directions(rows):
     """
     Guess the directionality of rows of points relative to each other.
@@ -180,29 +189,35 @@
 
             if avg_dist < best_dist:
                 # if we got a lower average, save this as the best offset
                 best_dist = avg_dist
                 best_roll_idx = i
 
         if expected_dist is not None and best_dist >= expected_dist * np.sqrt(2):
-            warnings.warn('The grid is sheared by more than 1 separation in some places', stacklevel=2)
+            warnings.warn(
+                "The grid is sheared by more than 1 separation in some places",
+                stacklevel=2,
+            )
 
         # we have the offset that minimises distances
         offset = best_roll_idx - len(next)
         total_offset = offset + offsets[-1]
         offsets.append(total_offset)
 
     # construct final aligned arrays by offsetting each row by the optimal offset and padding
     # everything so that the lengths are all equal
     aligned = []
     min_idx = min(offsets)
     max_idx = max(o + len(a) for o, a in zip(offsets, rows))
     for arr, offset in zip(rows, offsets):
         padded = np.pad(
-            arr, ((offset - min_idx, max_idx - offset - len(arr)), (0, 0)), mode='constant', constant_values=np.nan
+            arr,
+            ((offset - min_idx, max_idx - offset - len(arr)), (0, 0)),
+            mode="constant",
+            constant_values=np.nan,
         )
         aligned.append(padded)
     return aligned
 
 
 def extrapolate_point_rows_with_derivatives(strips, derivatives, separation):
     """
```

### Comparing `morphosamplers-0.0.8/src/morphosamplers.egg-info/SOURCES.txt` & `morphosamplers-0.0.9/src/morphosamplers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 .github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/cron.yml
 examples/path.py
 examples/sphere.py
 src/morphosamplers/__init__.py
 src/morphosamplers/core.py
+src/morphosamplers/helical_filament.py
 src/morphosamplers/sample_types.py
 src/morphosamplers/sampler.py
 src/morphosamplers/spline.py
 src/morphosamplers/surface_spline.py
 src/morphosamplers/utils.py
 src/morphosamplers.egg-info/PKG-INFO
 src/morphosamplers.egg-info/SOURCES.txt
```

### Comparing `morphosamplers-0.0.8/tests/test_sampling.py` & `morphosamplers-0.0.9/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/tests/test_spline_model.py` & `morphosamplers-0.0.9/tests/test_spline_model.py`

 * *Files identical despite different names*

### Comparing `morphosamplers-0.0.8/tox.ini` & `morphosamplers-0.0.9/tox.ini`

 * *Files identical despite different names*

