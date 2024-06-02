# Comparing `tmp/types-shapely-2.0.0.20240527.tar.gz` & `tmp/types-shapely-2.0.0.20240602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-shapely-2.0.0.20240527.tar", last modified: Mon May 27 02:23:57 2024, max compression
+gzip compressed data, was "types-shapely-2.0.0.20240602.tar", last modified: Sun Jun  2 02:27:02 2024, max compression
```

## Comparing `types-shapely-2.0.0.20240527.tar` & `types-shapely-2.0.0.20240602.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:57.061278 types-shapely-2.0.0.20240527/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 02:23:56.000000 types-shapely-2.0.0.20240527/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 02:23:56.000000 types-shapely-2.0.0.20240527/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-27 02:23:57.061278 types-shapely-2.0.0.20240527/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 02:23:57.065279 types-shapely-2.0.0.20240527/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-27 02:23:56.000000 types-shapely-2.0.0.20240527/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:57.061278 types-shapely-2.0.0.20240527/shapely-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-27 02:23:56.000000 types-shapely-2.0.0.20240527/shapely-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/_enum.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/_geometry.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/_ragged_array.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/_typing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/affinity.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:57.061278 types-shapely-2.0.0.20240527/shapely-stubs/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/algorithms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/algorithms/cga.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/algorithms/polylabel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16149 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/constructive.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/coordinates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/coords.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/creation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/errors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:57.061278 types-shapely-2.0.0.20240527/shapely-stubs/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/geometry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11980 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/geometry/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/geometry/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/geometry/geo.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/geometry/linestring.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/geometry/multilinestring.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/geometry/multipoint.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/geometry/multipolygon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/geometry/point.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/geometry/polygon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/geos.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/io.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/lib.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/linear.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/measurement.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/ops.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/plotting.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/predicates.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/prepared.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:56.000000 types-shapely-2.0.0.20240527/shapely-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/set_operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/speedups.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/strtree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/testing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/validation.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:57.061278 types-shapely-2.0.0.20240527/shapely-stubs/vectorized/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/vectorized/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/wkb.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-27 02:23:40.000000 types-shapely-2.0.0.20240527/shapely-stubs/wkt.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:23:57.061278 types-shapely-2.0.0.20240527/types_shapely.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-27 02:23:57.000000 types-shapely-2.0.0.20240527/types_shapely.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-27 02:23:57.000000 types-shapely-2.0.0.20240527/types_shapely.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 02:23:57.000000 types-shapely-2.0.0.20240527/types_shapely.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 02:23:57.000000 types-shapely-2.0.0.20240527/types_shapely.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 02:23:57.000000 types-shapely-2.0.0.20240527/types_shapely.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:27:02.789536 types-shapely-2.0.0.20240602/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-02 02:27:00.000000 types-shapely-2.0.0.20240602/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 02:27:00.000000 types-shapely-2.0.0.20240602/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-06-02 02:27:02.789536 types-shapely-2.0.0.20240602/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 02:27:02.789536 types-shapely-2.0.0.20240602/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-06-02 02:27:00.000000 types-shapely-2.0.0.20240602/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:27:02.785536 types-shapely-2.0.0.20240602/shapely-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-02 02:27:00.000000 types-shapely-2.0.0.20240602/shapely-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/_enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/_geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/_ragged_array.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/_typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/affinity.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:27:02.789536 types-shapely-2.0.0.20240602/shapely-stubs/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/algorithms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/algorithms/cga.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/algorithms/polylabel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/constructive.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/coordinates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/coords.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/creation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/errors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:27:02.789536 types-shapely-2.0.0.20240602/shapely-stubs/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/geometry/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11980 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/geometry/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/geometry/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/geometry/geo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/geometry/linestring.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/geometry/multilinestring.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/geometry/multipoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/geometry/multipolygon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/geometry/point.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/geometry/polygon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/geos.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/io.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/linear.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/measurement.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/ops.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/plotting.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/predicates.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/prepared.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 02:27:00.000000 types-shapely-2.0.0.20240602/shapely-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/set_operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/speedups.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/strtree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/testing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/validation.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:27:02.789536 types-shapely-2.0.0.20240602/shapely-stubs/vectorized/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/vectorized/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/wkb.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-02 02:26:50.000000 types-shapely-2.0.0.20240602/shapely-stubs/wkt.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:27:02.789536 types-shapely-2.0.0.20240602/types_shapely.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-06-02 02:27:02.000000 types-shapely-2.0.0.20240602/types_shapely.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-06-02 02:27:02.000000 types-shapely-2.0.0.20240602/types_shapely.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 02:27:02.000000 types-shapely-2.0.0.20240602/types_shapely.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-02 02:27:02.000000 types-shapely-2.0.0.20240602/types_shapely.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 02:27:02.000000 types-shapely-2.0.0.20240602/types_shapely.egg-info/top_level.txt
```

### Comparing `types-shapely-2.0.0.20240527/PKG-INFO` & `types-shapely-2.0.0.20240602/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-shapely
-Version: 2.0.0.20240527
+Version: 2.0.0.20240602
 Summary: Typing stubs for shapely
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/shapely.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-shapely` aims to provide accurate annotations
 for `shapely==2.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/shapely. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6246a38e8ee671bc1260f11280bb22a70bd04b31` and was tested
-with mypy 1.10.0, pyright 1.1.364, and
+This package was generated from typeshed commit `e285e52e1385a3c63a850dd5a2e8b2c744d7293a` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
```

### Comparing `types-shapely-2.0.0.20240527/setup.py` & `types-shapely-2.0.0.20240602/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-shapely` aims to provide accurate annotations
 for `shapely==2.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/shapely. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6246a38e8ee671bc1260f11280bb22a70bd04b31` and was tested
-with mypy 1.10.0, pyright 1.1.364, and
+This package was generated from typeshed commit `e285e52e1385a3c63a850dd5a2e8b2c744d7293a` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.0.0.20240527",
+      version="2.0.0.20240602",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/shapely.md",
```

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/__init__.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/_geometry.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/_geometry.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -158,17 +158,17 @@
 def get_num_geometries(geometry: OptGeoArrayLikeSeq, **kwargs) -> NDArray[np.int64]: ...
 @overload
 def get_precision(geometry: Geometry | None, **kwargs) -> float: ...
 @overload
 def get_precision(geometry: OptGeoArrayLikeSeq, **kwargs) -> NDArray[np.float64]: ...
 
 class SetPrecisionMode(ParamEnum):
-    valid_output: int
-    pointwise: int
-    keep_collapsed: int
+    valid_output = 0  # noqa: Y052
+    pointwise = 1  # noqa: Y052
+    keep_collapsed = 2  # noqa: Y052
 
 @overload
 def set_precision(geometry: OptGeoT, grid_size: float, mode: _PrecisionMode = "valid_output", **kwargs) -> OptGeoT: ...
 @overload
 def set_precision(
     geometry: OptGeoArrayLikeSeq, grid_size: float, mode: _PrecisionMode = "valid_output", **kwargs
 ) -> GeoArray: ...
```

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/_typing.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/_typing.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/affinity.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/affinity.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/algorithms/polylabel.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/algorithms/polylabel.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/constructive.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/constructive.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,22 @@
     "voronoi_polygons",
     "oriented_envelope",
     "minimum_rotated_rectangle",
     "minimum_bounding_circle",
 ]
 
 class BufferCapStyle(ParamEnum):
-    round: int
-    flat: int
-    square: int
+    round = 1  # noqa: Y052
+    flat = 2  # noqa: Y052
+    square = 3  # noqa: Y052
 
 class BufferJoinStyle(ParamEnum):
-    round: int
-    mitre: int
-    bevel: int
+    round = 1  # noqa: Y052
+    mitre = 2  # noqa: Y052
+    bevel = 3  # noqa: Y052
 
 @overload
 def boundary(geometry: Point | MultiPoint, **kwargs) -> GeometryCollection: ...
 @overload
 def boundary(geometry: LineString | MultiLineString, **kwargs) -> MultiPoint: ...
 @overload
 def boundary(geometry: Polygon | MultiPolygon, **kwargs) -> MultiLineString: ...
```

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/coordinates.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/coordinates.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/coords.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/coords.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/creation.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/creation.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/errors.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/geometry/__init__.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/geometry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/geometry/base.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/geometry/base.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/geometry/collection.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/geometry/collection.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/geometry/linestring.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/geometry/linestring.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/geometry/multilinestring.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/geometry/multilinestring.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/geometry/multipoint.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/geometry/multipoint.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/geometry/multipolygon.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/geometry/multipolygon.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/geometry/point.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/geometry/point.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/geometry/polygon.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/geometry/polygon.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/io.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/io.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/lib.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/lib.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/linear.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/linear.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/measurement.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/measurement.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/ops.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/ops.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/plotting.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/plotting.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/predicates.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/predicates.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/prepared.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/prepared.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/set_operations.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/set_operations.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/strtree.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/strtree.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 __all__ = ["STRtree"]
 
 _BinaryPredicate: TypeAlias = Literal[
     "intersects", "within", "contains", "overlaps", "crosses", "touches", "covers", "covered_by", "contains_properly"
 ]
 
 class BinaryPredicate(ParamEnum):
-    intersects: int
-    within: int
-    contains: int
-    overlaps: int
-    crosses: int
-    touches: int
-    covers: int
-    covered_by: int
-    contains_properly: int
+    intersects = 1  # noqa: Y052
+    within = 2  # noqa: Y052
+    contains = 3  # noqa: Y052
+    overlaps = 4  # noqa: Y052
+    crosses = 5  # noqa: Y052
+    touches = 6  # noqa: Y052
+    covers = 7  # noqa: Y052
+    covered_by = 8  # noqa: Y052
+    contains_properly = 9  # noqa: Y052
 
 class STRtree:
     def __init__(self, geoms: GeoArrayLikeSeq, node_capacity: SupportsIndex = 10) -> None: ...
     def __len__(self) -> int: ...
     @property
     def geometries(self) -> GeoArray: ...
     @overload
```

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/vectorized/__init__.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/vectorized/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/shapely-stubs/wkb.pyi` & `types-shapely-2.0.0.20240602/shapely-stubs/wkb.pyi`

 * *Files identical despite different names*

### Comparing `types-shapely-2.0.0.20240527/types_shapely.egg-info/PKG-INFO` & `types-shapely-2.0.0.20240602/types_shapely.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-shapely
-Version: 2.0.0.20240527
+Version: 2.0.0.20240602
 Summary: Typing stubs for shapely
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/shapely.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-shapely` aims to provide accurate annotations
 for `shapely==2.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/shapely. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6246a38e8ee671bc1260f11280bb22a70bd04b31` and was tested
-with mypy 1.10.0, pyright 1.1.364, and
+This package was generated from typeshed commit `e285e52e1385a3c63a850dd5a2e8b2c744d7293a` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
```

### Comparing `types-shapely-2.0.0.20240527/types_shapely.egg-info/SOURCES.txt` & `types-shapely-2.0.0.20240602/types_shapely.egg-info/SOURCES.txt`

 * *Files identical despite different names*

