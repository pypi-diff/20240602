# Comparing `tmp/simpleworkspace-1.2.214.tar.gz` & `tmp/simpleworkspace-1.2.215.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleworkspace-1.2.214.tar", last modified: Sun Jun  2 12:33:34 2024, max compression
+gzip compressed data, was "simpleworkspace-1.2.215.tar", last modified: Sun Jun  2 14:25:46 2024, max compression
```

## Comparing `simpleworkspace-1.2.214.tar` & `simpleworkspace-1.2.215.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.069491 simpleworkspace-1.2.214/
--rw-rw-rw-   0        0        0       22 2024-02-04 07:50:01.000000 simpleworkspace-1.2.214/MANIFEST.in
--rw-rw-rw-   0        0        0      177 2024-06-02 12:33:34.067496 simpleworkspace-1.2.214/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-06-02 12:32:22.000000 simpleworkspace-1.2.214/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-02 12:33:34.070488 simpleworkspace-1.2.214/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.791682 simpleworkspace-1.2.214/src/
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.865004 simpleworkspace-1.2.214/src/simpleworkspace/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.214/src/simpleworkspace/__init__.py
--rw-rw-rw-   0        0        0      453 2023-12-12 17:24:38.000000 simpleworkspace-1.2.214/src/simpleworkspace/__lazyimporter__.py
--rw-rw-rw-   0        0        0     2238 2024-06-02 11:57:50.000000 simpleworkspace-1.2.214/src/simpleworkspace/app.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.885947 simpleworkspace-1.2.214/src/simpleworkspace/assets/
--rw-rw-rw-   0        0        0      561 2024-02-26 13:54:52.000000 simpleworkspace-1.2.214/src/simpleworkspace/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.887942 simpleworkspace-1.2.214/src/simpleworkspace/assets/__pycache__/
--rw-rw-rw-   0        0        0      890 2024-04-15 18:36:31.000000 simpleworkspace-1.2.214/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.796668 simpleworkspace-1.2.214/src/simpleworkspace/assets/audio/
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.897916 simpleworkspace-1.2.214/src/simpleworkspace/assets/audio/alarms/
--rw-rw-rw-   0        0        0   115582 2024-02-26 13:54:53.000000 simpleworkspace-1.2.214/src/simpleworkspace/assets/audio/alarms/Siren.wav
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.918861 simpleworkspace-1.2.214/src/simpleworkspace/assets/audio/notifications/
--rw-rw-rw-   0        0        0   168352 2024-02-26 13:54:53.000000 simpleworkspace-1.2.214/src/simpleworkspace/assets/audio/notifications/Completed.wav
--rw-rw-rw-   0        0        0   159276 2024-02-26 13:54:53.000000 simpleworkspace-1.2.214/src/simpleworkspace/assets/audio/notifications/Error.wav
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.953280 simpleworkspace-1.2.214/src/simpleworkspace/assets/icons/
--rw-rw-rw-   0        0        0      864 2024-01-22 19:10:19.000000 simpleworkspace-1.2.214/src/simpleworkspace/assets/icons/ErrorCircle.png
--rw-rw-rw-   0        0        0      738 2024-01-22 19:10:19.000000 simpleworkspace-1.2.214/src/simpleworkspace/assets/icons/InfoCircle.png
--rw-rw-rw-   0        0        0      913 2024-01-22 19:10:19.000000 simpleworkspace-1.2.214/src/simpleworkspace/assets/icons/QuestionCircle.png
--rw-rw-rw-   0        0        0      643 2024-01-22 19:10:19.000000 simpleworkspace-1.2.214/src/simpleworkspace/assets/icons/WarningCircle.png
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.959264 simpleworkspace-1.2.214/src/simpleworkspace/collections/
--rw-rw-rw-   0        0        0        0 2023-12-09 17:26:55.000000 simpleworkspace-1.2.214/src/simpleworkspace/collections/__init__.py
--rw-rw-rw-   0        0        0      217 2023-12-12 17:24:38.000000 simpleworkspace-1.2.214/src/simpleworkspace/collections/loader.py
--rw-rw-rw-   0        0        0     8357 2023-12-23 08:45:05.000000 simpleworkspace-1.2.214/src/simpleworkspace/collections/observables.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.966246 simpleworkspace-1.2.214/src/simpleworkspace/db/
--rw-rw-rw-   0        0        0        0 2023-09-28 08:23:03.000000 simpleworkspace-1.2.214/src/simpleworkspace/db/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-11-25 10:02:31.000000 simpleworkspace-1.2.214/src/simpleworkspace/db/dbfactory.py
--rw-rw-rw-   0        0        0    26868 2024-01-17 11:30:30.000000 simpleworkspace-1.2.214/src/simpleworkspace/db/fluentsqlbuilder.py
--rw-rw-rw-   0        0        0      356 2023-12-12 17:24:38.000000 simpleworkspace-1.2.214/src/simpleworkspace/db/loader.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.970235 simpleworkspace-1.2.214/src/simpleworkspace/gui/
--rw-rw-rw-   0        0        0        0 2024-01-17 11:30:30.000000 simpleworkspace-1.2.214/src/simpleworkspace/gui/__init__.py
--rw-rw-rw-   0        0        0    19745 2024-02-04 07:50:01.000000 simpleworkspace-1.2.214/src/simpleworkspace/gui/dialogs.py
--rw-rw-rw-   0        0        0      199 2024-01-17 11:30:30.000000 simpleworkspace-1.2.214/src/simpleworkspace/gui/loader.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.978214 simpleworkspace-1.2.214/src/simpleworkspace/io/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.982203 simpleworkspace-1.2.214/src/simpleworkspace/io/audio/
--rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/audio/__init__.py
--rw-rw-rw-   0        0        0      184 2024-02-26 13:54:53.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/audio/loader.py
--rw-rw-rw-   0        0        0      720 2024-02-26 13:54:53.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/audio/play.py
--rw-rw-rw-   0        0        0     5574 2024-02-28 14:44:32.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/directory.py
--rw-rw-rw-   0        0        0     4101 2024-05-21 14:04:11.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/file.py
--rw-rw-rw-   0        0        0      603 2024-05-09 13:34:22.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/loader.py
--rw-rw-rw-   0        0        0     6180 2024-05-21 14:04:11.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/path.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.989184 simpleworkspace-1.2.214/src/simpleworkspace/io/readers/
--rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/readers/__init__.py
--rw-rw-rw-   0        0        0    13750 2024-05-21 14:04:11.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/readers/archive.py
--rw-rw-rw-   0        0        0     6265 2024-02-17 14:57:41.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/readers/csvreader.py
--rw-rw-rw-   0        0        0      423 2024-05-09 13:34:11.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/readers/loader.py
--rw-rw-rw-   0        0        0     2637 2024-02-26 13:54:53.000000 simpleworkspace-1.2.214/src/simpleworkspace/io/readers/logreader.py
--rw-rw-rw-   0        0        0     1256 2024-01-19 20:03:47.000000 simpleworkspace-1.2.214/src/simpleworkspace/loader.py
--rw-rw-rw-   0        0        0     6464 2024-02-04 13:21:24.000000 simpleworkspace-1.2.214/src/simpleworkspace/logproviders.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.813624 simpleworkspace-1.2.214/src/simpleworkspace/packages/
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.006139 simpleworkspace-1.2.214/src/simpleworkspace/packages/debug/
--rw-rw-rw-   0        0        0     2163 2024-02-04 07:50:01.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/debug/profiler.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.807640 simpleworkspace-1.2.214/src/simpleworkspace/packages/network/
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:33.808636 simpleworkspace-1.2.214/src/simpleworkspace/packages/network/servers/
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.010130 simpleworkspace-1.2.214/src/simpleworkspace/packages/network/servers/basicserver/
--rw-rw-rw-   0        0        0       71 2024-05-08 15:33:14.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.011126 simpleworkspace-1.2.214/src/simpleworkspace/packages/network/servers/basicserver/model/
--rw-rw-rw-   0        0        0     3293 2024-05-08 15:33:14.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
--rw-rw-rw-   0        0        0     9530 2024-05-08 15:33:14.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/network/servers/basicserver/server.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.013123 simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.015116 simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/
--rw-rw-rw-   0        0        0        0 2024-02-04 07:50:01.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.024097 simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
--rw-rw-rw-   0        0        0      717 2024-02-04 07:50:01.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
--rw-rw-rw-   0        0        0    38758 2024-02-04 07:50:01.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
--rw-rw-rw-   0        0        0     9974 2024-02-04 07:50:01.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
--rw-rw-rw-   0        0        0      348 2024-02-04 07:50:01.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
--rw-rw-rw-   0        0        0      768 2024-02-04 07:50:01.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
--rw-rw-rw-   0        0        0     4889 2024-06-02 08:30:18.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.029084 simpleworkspace-1.2.214/src/simpleworkspace/packages/taskscheduler/
--rw-rw-rw-   0        0        0       79 2023-09-16 11:15:10.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/taskscheduler/__init__.py
--rw-rw-rw-   0        0        0     8955 2024-05-08 15:33:14.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/taskscheduler/manager.py
--rw-rw-rw-   0        0        0     5302 2024-05-21 14:04:11.000000 simpleworkspace-1.2.214/src/simpleworkspace/packages/taskscheduler/model.py
--rw-rw-rw-   0        0        0     7383 2024-02-17 14:57:41.000000 simpleworkspace-1.2.214/src/simpleworkspace/settingsproviders.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.039571 simpleworkspace-1.2.214/src/simpleworkspace/types/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.214/src/simpleworkspace/types/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-02-17 14:57:41.000000 simpleworkspace-1.2.214/src/simpleworkspace/types/byte.py
--rw-rw-rw-   0        0        0     5736 2023-07-26 09:23:24.000000 simpleworkspace-1.2.214/src/simpleworkspace/types/iunit.py
--rw-rw-rw-   0        0        0      471 2023-12-12 17:24:38.000000 simpleworkspace-1.2.214/src/simpleworkspace/types/loader.py
--rw-rw-rw-   0        0        0      932 2023-07-26 09:23:24.000000 simpleworkspace-1.2.214/src/simpleworkspace/types/measurement.py
--rw-rw-rw-   0        0        0      556 2024-03-10 14:41:22.000000 simpleworkspace-1.2.214/src/simpleworkspace/types/os.py
--rw-rw-rw-   0        0        0     8342 2024-05-08 15:33:14.000000 simpleworkspace-1.2.214/src/simpleworkspace/types/time.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.060515 simpleworkspace-1.2.214/src/simpleworkspace/utility/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/__init__.py
--rw-rw-rw-   0        0        0      237 2023-04-09 11:23:10.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/bytes.py
--rw-rw-rw-   0        0        0     1916 2024-05-08 15:33:14.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/cache.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.064504 simpleworkspace-1.2.214/src/simpleworkspace/utility/concurrent/
--rw-rw-rw-   0        0        0      305 2024-06-02 08:24:36.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/concurrent/loader.py
--rw-rw-rw-   0        0        0     6150 2024-06-02 12:32:07.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/concurrent/locking.py
--rw-rw-rw-   0        0        0     1798 2024-06-02 08:26:06.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/concurrent/parallel.py
--rw-rw-rw-   0        0        0     7735 2024-02-11 09:17:40.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/console.py
--rw-rw-rw-   0        0        0     3157 2024-05-21 14:04:11.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/encryption.py
--rw-rw-rw-   0        0        0    14504 2024-05-08 15:33:14.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/linq.py
--rw-rw-rw-   0        0        0     1125 2024-06-02 08:25:43.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/loader.py
--rw-rw-rw-   0        0        0     4548 2024-03-03 10:52:37.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/module.py
--rw-rw-rw-   0        0        0    11289 2024-05-21 14:04:11.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/progressbar.py
--rw-rw-rw-   0        0        0     7218 2024-02-19 19:08:03.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/regex.py
--rw-rw-rw-   0        0        0     1897 2024-05-08 15:33:14.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/strings.py
--rw-rw-rw-   0        0        0     6760 2024-05-08 15:33:14.000000 simpleworkspace-1.2.214/src/simpleworkspace/utility/time.py
-drwxrwxrwx   0        0        0        0 2024-06-02 12:33:34.066498 simpleworkspace-1.2.214/src/simpleworkspace.egg-info/
--rw-rw-rw-   0        0        0      177 2024-06-02 12:33:33.000000 simpleworkspace-1.2.214/src/simpleworkspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3560 2024-06-02 12:33:33.000000 simpleworkspace-1.2.214/src/simpleworkspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 12:33:33.000000 simpleworkspace-1.2.214/src/simpleworkspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-06-02 12:33:33.000000 simpleworkspace-1.2.214/src/simpleworkspace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-06-02 12:33:33.000000 simpleworkspace-1.2.214/src/simpleworkspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:46.132869 simpleworkspace-1.2.215/
+-rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.215/MANIFEST.in
+-rw-rw-rw-   0        0        0      177 2024-06-02 14:25:46.126893 simpleworkspace-1.2.215/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-06-02 14:22:30.000000 simpleworkspace-1.2.215/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 14:25:46.133642 simpleworkspace-1.2.215/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.136496 simpleworkspace-1.2.215/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.348513 simpleworkspace-1.2.215/src/simpleworkspace/
+-rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.215/src/simpleworkspace/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.215/src/simpleworkspace/__lazyimporter__.py
+-rw-rw-rw-   0        0        0     2238 2024-06-02 13:52:20.000000 simpleworkspace-1.2.215/src/simpleworkspace/app.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.452730 simpleworkspace-1.2.215/src/simpleworkspace/assets/
+-rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.215/src/simpleworkspace/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.461288 simpleworkspace-1.2.215/src/simpleworkspace/assets/__pycache__/
+-rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.215/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.215/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.153747 simpleworkspace-1.2.215/src/simpleworkspace/assets/audio/
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.474727 simpleworkspace-1.2.215/src/simpleworkspace/assets/audio/alarms/
+-rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.215/src/simpleworkspace/assets/audio/alarms/Siren.wav
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.511510 simpleworkspace-1.2.215/src/simpleworkspace/assets/audio/notifications/
+-rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.215/src/simpleworkspace/assets/audio/notifications/Completed.wav
+-rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.215/src/simpleworkspace/assets/audio/notifications/Error.wav
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.547603 simpleworkspace-1.2.215/src/simpleworkspace/assets/icons/
+-rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.215/src/simpleworkspace/assets/icons/ErrorCircle.png
+-rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.215/src/simpleworkspace/assets/icons/InfoCircle.png
+-rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.215/src/simpleworkspace/assets/icons/QuestionCircle.png
+-rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.215/src/simpleworkspace/assets/icons/WarningCircle.png
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.591965 simpleworkspace-1.2.215/src/simpleworkspace/collections/
+-rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.215/src/simpleworkspace/collections/__init__.py
+-rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.215/src/simpleworkspace/collections/loader.py
+-rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.215/src/simpleworkspace/collections/observables.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.823410 simpleworkspace-1.2.215/src/simpleworkspace/db/
+-rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.215/src/simpleworkspace/db/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.215/src/simpleworkspace/db/dbfactory.py
+-rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.215/src/simpleworkspace/db/fluentsqlbuilder.py
+-rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.215/src/simpleworkspace/db/loader.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.922328 simpleworkspace-1.2.215/src/simpleworkspace/gui/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.215/src/simpleworkspace/gui/__init__.py
+-rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.215/src/simpleworkspace/gui/dialogs.py
+-rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.215/src/simpleworkspace/gui/loader.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:44.079720 simpleworkspace-1.2.215/src/simpleworkspace/io/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:44.135849 simpleworkspace-1.2.215/src/simpleworkspace/io/audio/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/audio/__init__.py
+-rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/audio/loader.py
+-rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/audio/play.py
+-rw-rw-rw-   0        0        0     5574 2024-05-10 07:59:18.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/directory.py
+-rw-rw-rw-   0        0        0     4101 2024-05-17 07:44:36.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/file.py
+-rw-rw-rw-   0        0        0      603 2024-05-09 18:37:59.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/loader.py
+-rw-rw-rw-   0        0        0     6180 2024-05-10 07:32:00.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/path.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:44.336192 simpleworkspace-1.2.215/src/simpleworkspace/io/readers/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/readers/__init__.py
+-rw-rw-rw-   0        0        0    13750 2024-05-12 06:37:39.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/readers/archive.py
+-rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/readers/csvreader.py
+-rw-rw-rw-   0        0        0      423 2024-05-09 18:37:59.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/readers/loader.py
+-rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.215/src/simpleworkspace/io/readers/logreader.py
+-rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.215/src/simpleworkspace/loader.py
+-rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.215/src/simpleworkspace/logproviders.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.235936 simpleworkspace-1.2.215/src/simpleworkspace/packages/
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:44.360897 simpleworkspace-1.2.215/src/simpleworkspace/packages/debug/
+-rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/debug/profiler.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.221705 simpleworkspace-1.2.215/src/simpleworkspace/packages/network/
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:43.223709 simpleworkspace-1.2.215/src/simpleworkspace/packages/network/servers/
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:44.497777 simpleworkspace-1.2.215/src/simpleworkspace/packages/network/servers/basicserver/
+-rw-rw-rw-   0        0        0       71 2024-04-21 07:34:26.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:44.585371 simpleworkspace-1.2.215/src/simpleworkspace/packages/network/servers/basicserver/model/
+-rw-rw-rw-   0        0        0     3293 2024-04-21 13:55:19.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
+-rw-rw-rw-   0        0        0     9530 2024-04-21 14:05:03.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/network/servers/basicserver/server.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:44.585371 simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:44.609740 simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/
+-rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:45.017119 simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
+-rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
+-rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
+-rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
+-rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
+-rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
+-rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:45.186425 simpleworkspace-1.2.215/src/simpleworkspace/packages/taskscheduler/
+-rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/taskscheduler/__init__.py
+-rw-rw-rw-   0        0        0     8955 2024-04-22 19:17:15.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/taskscheduler/manager.py
+-rw-rw-rw-   0        0        0     5302 2024-05-21 09:15:12.000000 simpleworkspace-1.2.215/src/simpleworkspace/packages/taskscheduler/model.py
+-rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.215/src/simpleworkspace/settingsproviders.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:45.437706 simpleworkspace-1.2.215/src/simpleworkspace/types/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.215/src/simpleworkspace/types/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.215/src/simpleworkspace/types/byte.py
+-rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.215/src/simpleworkspace/types/iunit.py
+-rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.215/src/simpleworkspace/types/loader.py
+-rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.215/src/simpleworkspace/types/measurement.py
+-rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.215/src/simpleworkspace/types/os.py
+-rw-rw-rw-   0        0        0     8342 2024-04-22 19:22:13.000000 simpleworkspace-1.2.215/src/simpleworkspace/types/time.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:46.057554 simpleworkspace-1.2.215/src/simpleworkspace/utility/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/bytes.py
+-rw-rw-rw-   0        0        0     1916 2024-04-22 19:17:15.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/cache.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:46.078870 simpleworkspace-1.2.215/src/simpleworkspace/utility/concurrent/
+-rw-rw-rw-   0        0        0      305 2024-06-02 13:52:21.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/concurrent/loader.py
+-rw-rw-rw-   0        0        0     6354 2024-06-02 14:02:53.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/concurrent/locking.py
+-rw-rw-rw-   0        0        0     1798 2024-06-02 13:52:21.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/concurrent/parallel.py
+-rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/console.py
+-rw-rw-rw-   0        0        0     3157 2024-05-13 19:52:32.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/encryption.py
+-rw-rw-rw-   0        0        0    14504 2024-04-25 16:58:27.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/linq.py
+-rw-rw-rw-   0        0        0     1125 2024-06-02 13:52:21.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/loader.py
+-rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/module.py
+-rw-rw-rw-   0        0        0    11289 2024-05-16 08:54:51.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/progressbar.py
+-rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/regex.py
+-rw-rw-rw-   0        0        0     1897 2024-05-08 10:41:26.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/strings.py
+-rw-rw-rw-   0        0        0     6760 2024-04-22 19:17:15.000000 simpleworkspace-1.2.215/src/simpleworkspace/utility/time.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:25:46.084865 simpleworkspace-1.2.215/src/simpleworkspace.egg-info/
+-rw-rw-rw-   0        0        0      177 2024-06-02 14:25:42.000000 simpleworkspace-1.2.215/src/simpleworkspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3624 2024-06-02 14:25:43.000000 simpleworkspace-1.2.215/src/simpleworkspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 14:25:42.000000 simpleworkspace-1.2.215/src/simpleworkspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-06-02 14:25:42.000000 simpleworkspace-1.2.215/src/simpleworkspace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-06-02 14:25:42.000000 simpleworkspace-1.2.215/src/simpleworkspace.egg-info/top_level.txt
```

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/app.py` & `simpleworkspace-1.2.215/src/simpleworkspace/app.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/assets/__init__.py` & `simpleworkspace-1.2.215/src/simpleworkspace/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc` & `simpleworkspace-1.2.215/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0x2c98dc65 (Mon Feb 26 13:54:52 2024 UTC)
+moddate:  0xe803da65 (Sat Feb 24 14:57:44 2024 UTC)
 files sz: 561
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -91,11 +91,11 @@
       '/audio/notifications/Completed.wav'
       '/audio/notifications/Error.wav'
       None
    names      ('os', 'path', '_path', 'dirname', 'abspath', '__file__', 'PATH_ASSETS', 'Icons_ErrorCircle_PNG', 'Icons_QuestionCircle_PNG', 'Icons_WarningCircle_PNG', 'Icons_InfoCircle_PNG', 'Audio_Alarms_Siren', 'Audio_Notification_Completed', 'Audio_Notification_Error')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'D:\\Documents\\Development\\PythonProjects\\Py_SimpleWorkspace\\src\\simpleworkspace\\assets\\__init__.py'
+   filename   'C:\\dev\\pythonProjects\\Python_SimpleWorkspace\\src\\simpleworkspace\\assets\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0244020a010a010a010a020a010a01
```

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/assets/audio/alarms/Siren.wav` & `simpleworkspace-1.2.215/src/simpleworkspace/assets/audio/alarms/Siren.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/assets/audio/notifications/Completed.wav` & `simpleworkspace-1.2.215/src/simpleworkspace/assets/audio/notifications/Completed.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/assets/audio/notifications/Error.wav` & `simpleworkspace-1.2.215/src/simpleworkspace/assets/audio/notifications/Error.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/assets/icons/ErrorCircle.png` & `simpleworkspace-1.2.215/src/simpleworkspace/assets/icons/ErrorCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/assets/icons/InfoCircle.png` & `simpleworkspace-1.2.215/src/simpleworkspace/assets/icons/InfoCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/assets/icons/QuestionCircle.png` & `simpleworkspace-1.2.215/src/simpleworkspace/assets/icons/QuestionCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/assets/icons/WarningCircle.png` & `simpleworkspace-1.2.215/src/simpleworkspace/assets/icons/WarningCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/collections/observables.py` & `simpleworkspace-1.2.215/src/simpleworkspace/collections/observables.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/db/dbfactory.py` & `simpleworkspace-1.2.215/src/simpleworkspace/db/dbfactory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/db/fluentsqlbuilder.py` & `simpleworkspace-1.2.215/src/simpleworkspace/db/fluentsqlbuilder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/gui/dialogs.py` & `simpleworkspace-1.2.215/src/simpleworkspace/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/io/audio/play.py` & `simpleworkspace-1.2.215/src/simpleworkspace/io/audio/play.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/io/directory.py` & `simpleworkspace-1.2.215/src/simpleworkspace/io/directory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/io/file.py` & `simpleworkspace-1.2.215/src/simpleworkspace/io/file.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/io/loader.py` & `simpleworkspace-1.2.215/src/simpleworkspace/io/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/io/path.py` & `simpleworkspace-1.2.215/src/simpleworkspace/io/path.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/io/readers/archive.py` & `simpleworkspace-1.2.215/src/simpleworkspace/io/readers/archive.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/io/readers/csvreader.py` & `simpleworkspace-1.2.215/src/simpleworkspace/io/readers/csvreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/io/readers/logreader.py` & `simpleworkspace-1.2.215/src/simpleworkspace/io/readers/logreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/loader.py` & `simpleworkspace-1.2.215/src/simpleworkspace/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/logproviders.py` & `simpleworkspace-1.2.215/src/simpleworkspace/logproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/packages/debug/profiler.py` & `simpleworkspace-1.2.215/src/simpleworkspace/packages/debug/profiler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py` & `simpleworkspace-1.2.215/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/packages/network/servers/basicserver/server.py` & `simpleworkspace-1.2.215/src/simpleworkspace/packages/network/servers/basicserver/server.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py` & `simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py` & `simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py` & `simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py` & `simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py` & `simpleworkspace-1.2.215/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/packages/taskscheduler/manager.py` & `simpleworkspace-1.2.215/src/simpleworkspace/packages/taskscheduler/manager.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/packages/taskscheduler/model.py` & `simpleworkspace-1.2.215/src/simpleworkspace/packages/taskscheduler/model.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/settingsproviders.py` & `simpleworkspace-1.2.215/src/simpleworkspace/settingsproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/types/byte.py` & `simpleworkspace-1.2.215/src/simpleworkspace/types/byte.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/types/iunit.py` & `simpleworkspace-1.2.215/src/simpleworkspace/types/iunit.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/types/measurement.py` & `simpleworkspace-1.2.215/src/simpleworkspace/types/measurement.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/types/os.py` & `simpleworkspace-1.2.215/src/simpleworkspace/types/os.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/types/time.py` & `simpleworkspace-1.2.215/src/simpleworkspace/types/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/cache.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/cache.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/concurrent/locking.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/concurrent/locking.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,32 +10,34 @@
 
     def __init__(self, id: str) -> None:
         import simpleworkspace.io.file, tempfile
 
         self.id = id
         self._currentOS = _OperatingSystemEnum.GetCurrentOS()
 
-        self.lock_file = _os.path.join(tempfile.gettempdir(), f"pyswl_{simpleworkspace.io.file.SantizeFilename(id)}.lock")
+        self._context_lock_filepath = _os.path.join(tempfile.gettempdir(), f"pyswl_{simpleworkspace.io.file.SantizeFilename(id)}.lock")
         self._context_lock_fh = None
         self._context_mode = 0o644
+
+        self._pollinterval = _TimeSpan(seconds=1)
     
     @property
     def IsLocked(self):
         return self._context_lock_fh is not None
 
     def _Acquire_Unix(self):
         import fcntl
 
-        self._raise_on_not_writable_file(self.lock_file)
+        self._raise_on_not_writable_file(self._context_lock_filepath)
         
         open_flags = _os.O_RDWR | _os.O_TRUNC
-        if not _os.path.exists(self.lock_file):
+        if not _os.path.exists(self._context_lock_filepath):
             open_flags |= _os.O_CREAT
         
-        fh = _os.open(self.lock_file, open_flags, self._context_mode)
+        fh = _os.open(self._context_lock_filepath, open_flags, self._context_mode)
         with _suppress(PermissionError):  # This locked is not owned by this UID
             _os.fchmod(fh, self._context_mode)
         try:
             fcntl.flock(fh, fcntl.LOCK_EX | fcntl.LOCK_NB)
         except OSError as exception:
             _os.close(fh)
             if exception.errno == _errno.ENOSYS:  # NotImplemented error
@@ -43,22 +45,22 @@
                 raise NotImplementedError(msg) from exception
         else:
             self._context_lock_fh = fh
 
     def _Acquire_Windows(self):
         import msvcrt
 
-        self._raise_on_not_writable_file(self.lock_file)
+        self._raise_on_not_writable_file(self._context_lock_filepath)
         flags = (
             _os.O_RDWR  # open for read and write
             | _os.O_CREAT  # create file if not exists
             | _os.O_TRUNC  # truncate file if not empty
         )
         try:
-            fh = _os.open(self.lock_file, flags, self._context_mode)
+            fh = _os.open(self._context_lock_filepath, flags, self._context_mode)
         except OSError as exception:
             if exception.errno != _errno.EACCES:  # has no access to this lock
                 raise
         else:
             try:
                 msvcrt.locking(fh, msvcrt.LK_NBLCK, 1)
             except OSError as exception:
@@ -85,17 +87,17 @@
 
         fh = _cast(int, self._context_lock_fh)
         self._context_lock_fh = None
         msvcrt.locking(fh, msvcrt.LK_UNLCK, 1)
         _os.close(fh)
 
         with _suppress(OSError):  # Probably another instance of the application had acquired the file lock.
-            _os.unlink(self.lock_file)
+            _os.unlink(self._context_lock_filepath)
     
-    def Acquire(self, blocking=False, timeout:int=None):
+    def Acquire(self, blocking=False, timeout:_TimeSpan=None):
         """Tries to aquire a system wide file lock
 
         :param blocking: when blocking is true, waits until a lock is received or timeout
         :param timeout: total seconds to wait before timing out
         """
         import time
         from simpleworkspace.utility.time import StopWatch
@@ -113,18 +115,18 @@
             
             if(self.IsLocked):
                 break
 
             if(blocking is False):
                 raise TimeoutError(f'Failed to immediately acquire lock on "{self.id}"')
 
-            if(timeout is not None) and (stopwatch.GetElapsedSeconds() > timeout):
-                raise TimeoutError(f'Timeout acquiring lock on {self.id} for {timeout} seconds')
+            if(timeout is not None) and (stopwatch.GetElapsedSeconds() > timeout.TotalSeconds):
+                raise TimeoutError(f'Timeout acquiring lock on {self.id} for {timeout.TotalSeconds} seconds')
             
-            time.sleep(1)
+            time.sleep(self._pollinterval.TotalSeconds)
 
     def Release(self):
         if(not self.IsLocked):
             return
         
         if(self._currentOS == _OperatingSystemEnum.Windows):
             self._Release_Windows()
```

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/concurrent/parallel.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/concurrent/parallel.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/console.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/console.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/encryption.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/encryption.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/linq.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/linq.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/loader.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/module.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/module.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/progressbar.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/progressbar.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/regex.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/regex.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/strings.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/strings.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace/utility/time.py` & `simpleworkspace-1.2.215/src/simpleworkspace/utility/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.214/src/simpleworkspace.egg-info/SOURCES.txt` & `simpleworkspace-1.2.215/src/simpleworkspace.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/simpleworkspace/settingsproviders.py
 src/simpleworkspace.egg-info/PKG-INFO
 src/simpleworkspace.egg-info/SOURCES.txt
 src/simpleworkspace.egg-info/dependency_links.txt
 src/simpleworkspace.egg-info/requires.txt
 src/simpleworkspace.egg-info/top_level.txt
 src/simpleworkspace/assets/__init__.py
+src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
 src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
 src/simpleworkspace/assets/audio/alarms/Siren.wav
 src/simpleworkspace/assets/audio/notifications/Completed.wav
 src/simpleworkspace/assets/audio/notifications/Error.wav
 src/simpleworkspace/assets/icons/ErrorCircle.png
 src/simpleworkspace/assets/icons/InfoCircle.png
 src/simpleworkspace/assets/icons/QuestionCircle.png
```

