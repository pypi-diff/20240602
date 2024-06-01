# Comparing `tmp/sounderpy-3.0.4.dev3.tar.gz` & `tmp/sounderpy-3.0.4.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sounderpy-3.0.4.dev3.tar", last modified: Sat Jun  1 23:12:25 2024, max compression
+gzip compressed data, was "sounderpy-3.0.4.dev4.tar", last modified: Sat Jun  1 23:27:49 2024, max compression
```

## Comparing `sounderpy-3.0.4.dev3.tar` & `sounderpy-3.0.4.dev4.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:25.488763 sounderpy-3.0.4.dev3/
--rw-rw-rw-   0        0        0     1094 2024-01-08 16:49:48.000000 sounderpy-3.0.4.dev3/LICENSE
--rw-rw-rw-   0        0        0    11192 2024-06-01 23:12:25.483785 sounderpy-3.0.4.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     9760 2024-06-01 23:09:33.000000 sounderpy-3.0.4.dev3/README.md
--rw-rw-rw-   0        0        0     1378 2024-06-01 23:10:15.000000 sounderpy-3.0.4.dev3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-01 23:12:25.489768 sounderpy-3.0.4.dev3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:24.392497 sounderpy-3.0.4.dev3/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:24.456998 sounderpy-3.0.4.dev3/src/sounderpy/
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:24.492252 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/
--rw-rw-rw-   0        0        0       64 2023-06-15 13:50:54.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:24.510177 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/ci/
--rw-rw-rw-   0        0        0      439 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/ci/check_artifact_dir.py
--rw-rw-rw-   0        0        0      337 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/ci/screen.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:24.525517 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/datasources/
--rw-rw-rw-   0        0        0       41 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/datasources/__init__.py
--rw-rw-rw-   0        0        0    22995 2023-06-15 13:09:42.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/datasources/available.py
--rw-rw-rw-   0        0        0    19870 2023-06-15 13:09:42.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/datasources/data_source.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:24.412695 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:24.549196 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/io/
--rw-rw-rw-   0        0        0      115 2023-06-15 13:11:47.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:24.558982 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/plot/
--rw-rw-rw-   0        0        0       20 2023-06-15 13:11:48.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/plot/__init__.py
--rw-rw-rw-   0        0        0    13958 2023-12-20 17:12:24.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:24.810455 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/
--rw-rw-rw-   0        0        0       52 2023-06-15 13:35:03.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-06-15 13:09:48.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py
--rw-rw-rw-   0        0        0    18524 2023-06-15 13:09:48.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py
--rw-rw-rw-   0        0        0      891 2023-06-15 13:11:48.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py
--rw-rw-rw-   0        0        0     1054 2023-06-15 13:35:09.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py
--rw-rw-rw-   0        0        0     3433 2023-12-20 17:04:47.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py
--rw-rw-rw-   0        0        0     7972 2023-12-20 17:09:41.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py
--rw-rw-rw-   0        0        0     3890 2023-12-20 17:12:22.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py
--rw-rw-rw-   0        0        0    12670 2023-12-20 17:09:40.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py
--rw-rw-rw-   0        0        0   120008 2024-01-01 01:57:39.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py
--rw-rw-rw-   0        0        0    16042 2023-12-20 17:09:38.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py
--rw-rw-rw-   0        0        0    49972 2023-12-20 16:52:49.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py
--rw-rw-rw-   0        0        0     8133 2023-12-20 17:09:36.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py
--rw-rw-rw-   0        0        0     5849 2023-12-20 18:02:55.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py
--rw-rw-rw-   0        0        0    17031 2023-06-15 13:35:02.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py
--rw-rw-rw-   0        0        0     6846 2023-12-20 17:09:34.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py
--rw-rw-rw-   0        0        0    13328 2023-12-20 17:09:33.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py
--rw-rw-rw-   0        0        0    14047 2023-12-20 17:09:33.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py
--rw-rw-rw-   0        0        0     8649 2023-12-20 17:09:32.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py
--rw-rw-rw-   0        0        0    22092 2023-12-20 17:09:32.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py
--rw-rw-rw-   0        0        0    16016 2023-12-20 17:22:10.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:24.992362 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/
--rw-rw-rw-   0        0        0      925 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py
--rw-rw-rw-   0        0        0     2280 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py
--rw-rw-rw-   0        0        0     4008 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py
--rw-rw-rw-   0        0        0     4168 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py
--rw-rw-rw-   0        0        0     1205 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py
--rw-rw-rw-   0        0        0     3896 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py
--rw-rw-rw-   0        0        0     3532 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py
--rw-rw-rw-   0        0        0    10918 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py
--rw-rw-rw-   0        0        0      529 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py
--rw-rw-rw-   0        0        0    13676 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py
--rw-rw-rw-   0        0        0     1296 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py
--rw-rw-rw-   0        0        0     9568 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py
--rw-rw-rw-   0        0        0     3558 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:25.389878 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/
--rw-rw-rw-   0        0        0    40265 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py
--rw-rw-rw-   0        0        0      938 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py
--rw-rw-rw-   0        0        0     7734 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py
--rw-rw-rw-   0        0        0    21293 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py
--rw-rw-rw-   0        0        0     5589 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py
--rw-rw-rw-   0        0        0     9080 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py
--rw-rw-rw-   0        0        0    12439 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py
--rw-rw-rw-   0        0        0    15829 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py
--rw-rw-rw-   0        0        0    12108 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py
--rw-rw-rw-   0        0        0    52153 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py
--rw-rw-rw-   0        0        0    23498 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py
--rw-rw-rw-   0        0        0    34524 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py
--rw-rw-rw-   0        0        0    19031 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py
--rw-rw-rw-   0        0        0    10173 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py
--rw-rw-rw-   0        0        0    65020 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py
--rw-rw-rw-   0        0        0    11895 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py
--rw-rw-rw-   0        0        0    10152 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py
--rw-rw-rw-   0        0        0    15699 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py
--rw-rw-rw-   0        0        0    21968 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py
--rw-rw-rw-   0        0        0    11938 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py
--rw-rw-rw-   0        0        0    32304 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py
--rw-rw-rw-   0        0        0    10140 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py
--rw-rw-rw-   0        0        0    12890 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py
--rw-rw-rw-   0        0        0     7759 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py
--rw-rw-rw-   0        0        0    14588 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:25.457478 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/
--rw-rw-rw-   0        0        0       65 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/__init__.py
--rw-rw-rw-   0        0        0     4236 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/async.py
--rw-rw-rw-   0        0        0     4147 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py
--rw-rw-rw-   0        0        0     2512 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/config.py
--rw-rw-rw-   0        0        0     1660 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py
--rw-rw-rw-   0        0        0     1933 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/progress.py
--rw-rw-rw-   0        0        0      156 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/utils.py
--rw-rw-rw-   0        0        0     1329 2023-12-20 17:14:06.000000 sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py
--rw-rw-rw-   0        0        0      743 2024-03-17 22:48:51.000000 sounderpy-3.0.4.dev3/src/sounderpy/__init__.py
--rw-rw-rw-   0        0        0    44655 2024-06-01 23:09:12.000000 sounderpy-3.0.4.dev3/src/sounderpy/calc.py
--rw-rw-rw-   0        0        0   193634 2024-06-01 23:10:26.000000 sounderpy-3.0.4.dev3/src/sounderpy/plot.py
--rw-rw-rw-   0        0        0    98090 2024-06-01 23:11:10.000000 sounderpy-3.0.4.dev3/src/sounderpy/sounderpy.py
-drwxrwxrwx   0        0        0        0 2024-06-01 23:12:25.474809 sounderpy-3.0.4.dev3/src/sounderpy.egg-info/
--rw-rw-rw-   0        0        0    11192 2024-06-01 23:12:24.000000 sounderpy-3.0.4.dev3/src/sounderpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4156 2024-06-01 23:12:24.000000 sounderpy-3.0.4.dev3/src/sounderpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 23:12:24.000000 sounderpy-3.0.4.dev3/src/sounderpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2024-06-01 23:12:24.000000 sounderpy-3.0.4.dev3/src/sounderpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-06-01 23:12:24.000000 sounderpy-3.0.4.dev3/src/sounderpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.743059 sounderpy-3.0.4.dev4/
+-rw-rw-rw-   0        0        0     1094 2024-01-08 16:49:48.000000 sounderpy-3.0.4.dev4/LICENSE
+-rw-rw-rw-   0        0        0    11192 2024-06-01 23:27:49.732528 sounderpy-3.0.4.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     9760 2024-06-01 23:09:33.000000 sounderpy-3.0.4.dev4/README.md
+-rw-rw-rw-   0        0        0     1378 2024-06-01 23:27:19.000000 sounderpy-3.0.4.dev4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 23:27:49.743059 sounderpy-3.0.4.dev4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.036013 sounderpy-3.0.4.dev4/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.075252 sounderpy-3.0.4.dev4/src/sounderpy/
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.107728 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/
+-rw-rw-rw-   0        0        0       64 2023-06-15 13:50:54.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.119460 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/ci/
+-rw-rw-rw-   0        0        0      439 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/ci/check_artifact_dir.py
+-rw-rw-rw-   0        0        0      337 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/ci/screen.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.133418 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/datasources/
+-rw-rw-rw-   0        0        0       41 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/datasources/__init__.py
+-rw-rw-rw-   0        0        0    22995 2023-06-15 13:09:42.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/datasources/available.py
+-rw-rw-rw-   0        0        0    19870 2023-06-15 13:09:42.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/datasources/data_source.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.041016 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.141428 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/io/
+-rw-rw-rw-   0        0        0      115 2023-06-15 13:11:47.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.151806 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/plot/
+-rw-rw-rw-   0        0        0       20 2023-06-15 13:11:48.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/plot/__init__.py
+-rw-rw-rw-   0        0        0    13958 2023-12-20 17:12:24.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.283420 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/
+-rw-rw-rw-   0        0        0       52 2023-06-15 13:35:03.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-06-15 13:09:48.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py
+-rw-rw-rw-   0        0        0    18524 2023-06-15 13:09:48.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py
+-rw-rw-rw-   0        0        0      891 2023-06-15 13:11:48.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py
+-rw-rw-rw-   0        0        0     1054 2023-06-15 13:35:09.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py
+-rw-rw-rw-   0        0        0     3433 2023-12-20 17:04:47.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py
+-rw-rw-rw-   0        0        0     7972 2023-12-20 17:09:41.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py
+-rw-rw-rw-   0        0        0     3890 2023-12-20 17:12:22.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py
+-rw-rw-rw-   0        0        0    12670 2023-12-20 17:09:40.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py
+-rw-rw-rw-   0        0        0   120008 2024-01-01 01:57:39.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py
+-rw-rw-rw-   0        0        0    16042 2023-12-20 17:09:38.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py
+-rw-rw-rw-   0        0        0    49972 2023-12-20 16:52:49.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py
+-rw-rw-rw-   0        0        0     8133 2023-12-20 17:09:36.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py
+-rw-rw-rw-   0        0        0     5849 2023-12-20 18:02:55.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py
+-rw-rw-rw-   0        0        0    17031 2023-06-15 13:35:02.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py
+-rw-rw-rw-   0        0        0     6846 2023-12-20 17:09:34.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py
+-rw-rw-rw-   0        0        0    13328 2023-12-20 17:09:33.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py
+-rw-rw-rw-   0        0        0    14047 2023-12-20 17:09:33.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py
+-rw-rw-rw-   0        0        0     8649 2023-12-20 17:09:32.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py
+-rw-rw-rw-   0        0        0    22092 2023-12-20 17:09:32.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py
+-rw-rw-rw-   0        0        0    16016 2023-12-20 17:22:10.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.433317 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/
+-rw-rw-rw-   0        0        0      925 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py
+-rw-rw-rw-   0        0        0     2280 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py
+-rw-rw-rw-   0        0        0     4008 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py
+-rw-rw-rw-   0        0        0     4168 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py
+-rw-rw-rw-   0        0        0     1205 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3896 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py
+-rw-rw-rw-   0        0        0     3532 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py
+-rw-rw-rw-   0        0        0    10918 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py
+-rw-rw-rw-   0        0        0      529 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py
+-rw-rw-rw-   0        0        0    13676 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py
+-rw-rw-rw-   0        0        0     1296 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py
+-rw-rw-rw-   0        0        0     9568 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py
+-rw-rw-rw-   0        0        0     3558 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.661276 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/
+-rw-rw-rw-   0        0        0    40265 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py
+-rw-rw-rw-   0        0        0      938 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py
+-rw-rw-rw-   0        0        0     7734 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py
+-rw-rw-rw-   0        0        0    21293 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py
+-rw-rw-rw-   0        0        0     5589 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py
+-rw-rw-rw-   0        0        0     9080 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py
+-rw-rw-rw-   0        0        0    12439 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py
+-rw-rw-rw-   0        0        0    15829 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py
+-rw-rw-rw-   0        0        0    12108 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py
+-rw-rw-rw-   0        0        0    52153 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py
+-rw-rw-rw-   0        0        0    23498 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py
+-rw-rw-rw-   0        0        0    34524 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py
+-rw-rw-rw-   0        0        0    19031 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py
+-rw-rw-rw-   0        0        0    10173 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py
+-rw-rw-rw-   0        0        0    65020 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py
+-rw-rw-rw-   0        0        0    11895 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py
+-rw-rw-rw-   0        0        0    10152 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py
+-rw-rw-rw-   0        0        0    15699 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py
+-rw-rw-rw-   0        0        0    21968 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py
+-rw-rw-rw-   0        0        0    11938 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py
+-rw-rw-rw-   0        0        0    32304 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py
+-rw-rw-rw-   0        0        0    10140 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py
+-rw-rw-rw-   0        0        0    12890 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py
+-rw-rw-rw-   0        0        0     7759 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py
+-rw-rw-rw-   0        0        0    14588 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.719963 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/
+-rw-rw-rw-   0        0        0       65 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/__init__.py
+-rw-rw-rw-   0        0        0     4236 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/async.py
+-rw-rw-rw-   0        0        0     4147 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py
+-rw-rw-rw-   0        0        0     2512 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/config.py
+-rw-rw-rw-   0        0        0     1660 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py
+-rw-rw-rw-   0        0        0     1933 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/progress.py
+-rw-rw-rw-   0        0        0      156 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/utils.py
+-rw-rw-rw-   0        0        0     1329 2023-12-20 17:14:06.000000 sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py
+-rw-rw-rw-   0        0        0      743 2024-03-17 22:48:51.000000 sounderpy-3.0.4.dev4/src/sounderpy/__init__.py
+-rw-rw-rw-   0        0        0    44655 2024-06-01 23:09:12.000000 sounderpy-3.0.4.dev4/src/sounderpy/calc.py
+-rw-rw-rw-   0        0        0   193634 2024-06-01 23:10:26.000000 sounderpy-3.0.4.dev4/src/sounderpy/plot.py
+-rw-rw-rw-   0        0        0    98102 2024-06-01 23:27:04.000000 sounderpy-3.0.4.dev4/src/sounderpy/sounderpy.py
+drwxrwxrwx   0        0        0        0 2024-06-01 23:27:49.726939 sounderpy-3.0.4.dev4/src/sounderpy.egg-info/
+-rw-rw-rw-   0        0        0    11192 2024-06-01 23:27:48.000000 sounderpy-3.0.4.dev4/src/sounderpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4156 2024-06-01 23:27:49.000000 sounderpy-3.0.4.dev4/src/sounderpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 23:27:48.000000 sounderpy-3.0.4.dev4/src/sounderpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2024-06-01 23:27:48.000000 sounderpy-3.0.4.dev4/src/sounderpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-01 23:27:48.000000 sounderpy-3.0.4.dev4/src/sounderpy.egg-info/top_level.txt
```

### Comparing `sounderpy-3.0.4.dev3/LICENSE` & `sounderpy-3.0.4.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/PKG-INFO` & `sounderpy-3.0.4.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 3.0.4.dev3
+Version: 3.0.4.dev4
 Summary: Vertical Profile Data Retrieval and Analysis Tool For Python
 Author-email: "Kyle J Gillett, University of North Dakota" <kyle.gillett@und.edu>
 Project-URL: Docs, https://kylejgillett.github.io/sounderpy/
 Project-URL: Code, https://github.com/kylejgillett/sounderpy
 Project-URL: Operational Site, https://sounderpysoundings.anvil.app/
 Project-URL: PyPi, https://pypi.org/project/sounderpy/
 Project-URL: My Website, https://kylegillettphoto.com
```

### Comparing `sounderpy-3.0.4.dev3/README.md` & `sounderpy-3.0.4.dev4/README.md`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/pyproject.toml` & `sounderpy-3.0.4.dev4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sounderpy"
-version = "3.0.4dev3"
+version = "3.0.4dev4"
 authors = [
   { name="Kyle J Gillett, University of North Dakota", email="kyle.gillett@und.edu" },
 ]
 description = "Vertical Profile Data Retrieval and Analysis Tool For Python"
 readme = "README.md"
 keywords = ["meteorology", "science", "data-analysis", "weather", "forecasting"]
 requires-python = ">=3.1"
```

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/datasources/available.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/datasources/available.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/datasources/data_source.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/datasources/data_source.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/async.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/async.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/config.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/config.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/progress.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/progress.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py` & `sounderpy-3.0.4.dev4/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/__init__.py` & `sounderpy-3.0.4.dev4/src/sounderpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/calc.py` & `sounderpy-3.0.4.dev4/src/sounderpy/calc.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/plot.py` & `sounderpy-3.0.4.dev4/src/sounderpy/plot.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy/sounderpy.py` & `sounderpy-3.0.4.dev4/src/sounderpy/sounderpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -896,42 +896,42 @@
     
     # make sure variables are in the correct case
     model   = str.lower(model)
     station = str.upper(station)
 
     # remove '#' for URL
     if '#' in station: 
-        station = station.replace('#', '%23')
+        url_station = station.replace('#', '%23')
     
     # GET MOST-RECENT RUNS FROM PSU SERVERS 
     # if date variables (year, month, day) are not given, the user has 'selected' a most
     # recent forecast run, get that from PSU
     if run_year == None:
         if model not in ['gfs', 'nam', 'namnest', 'rap', 'hrrr', 'sref', 'hiresw']:
             raise ValueError(f"{model} is not a valid model option. Valid models include ['GFS', 'NAM', 'NAMNEST', 'RAP', 'HRRR', 'SREF', 'HIRESW']")
         if model == 'gfs':
             model3 = 'gfs3' 
         else:
             model3 = model
-        data_conn = f'http://www.meteo.psu.edu/bufkit/data/{model.upper()}/{model3}_{station.lower()}.buf'
+        data_conn = f'http://www.meteo.psu.edu/bufkit/data/{model.upper()}/{model3}_{url_station.lower()}.buf'
      
     
     # GET ARCHIVE DATA FROM THE IEM SERVERS. CORRECT GFS & NAM MODEL NAMES
     # if date variables (year, month, day) are given, the user has 'selected' a 
     # archived forecast for the given date 
     else:
         if model not in ['gfs', 'nam', 'namnest', 'rap', 'hrrr']:
             raise ValueError(f"{model} is not a valid model option. Valid models include ['GFS', 'NAM', 'NAMNEST', 'RAP', 'HRRR']")
         if model == 'namnest':
             model = 'nam4km'
         if model == 'gfs':
             model3 = 'gfs3' 
         else:
             model3 = model
-        data_conn = f'https://mtarchive.geol.iastate.edu/{run_year}/{run_month}/{run_day}/bufkit/{run_hour}/{model}/{model3}_{station.lower()}.buf'  
+        data_conn = f'https://mtarchive.geol.iastate.edu/{run_year}/{run_month}/{run_day}/bufkit/{run_hour}/{model}/{model3}_{url_station.lower()}.buf'  
 
 
     # Check to make sure the user-defined site ID is a valid bufkit site before continuing 
     try:  
         # GET BUFKIT STATIONS LISTING FROM SOUNDERPY GITHUB REPO
         BUFKIT_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/src/BUFKIT-STATIONS-MASTER.txt', 
                                       skiprows=7, skipinitialspace = True)
```

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy.egg-info/PKG-INFO` & `sounderpy-3.0.4.dev4/src/sounderpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 3.0.4.dev3
+Version: 3.0.4.dev4
 Summary: Vertical Profile Data Retrieval and Analysis Tool For Python
 Author-email: "Kyle J Gillett, University of North Dakota" <kyle.gillett@und.edu>
 Project-URL: Docs, https://kylejgillett.github.io/sounderpy/
 Project-URL: Code, https://github.com/kylejgillett/sounderpy
 Project-URL: Operational Site, https://sounderpysoundings.anvil.app/
 Project-URL: PyPi, https://pypi.org/project/sounderpy/
 Project-URL: My Website, https://kylegillettphoto.com
```

### Comparing `sounderpy-3.0.4.dev3/src/sounderpy.egg-info/SOURCES.txt` & `sounderpy-3.0.4.dev4/src/sounderpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

