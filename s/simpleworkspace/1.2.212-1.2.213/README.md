# Comparing `tmp/simpleworkspace-1.2.212.tar.gz` & `tmp/simpleworkspace-1.2.213.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleworkspace-1.2.212.tar", last modified: Sun Jun  2 11:59:32 2024, max compression
+gzip compressed data, was "simpleworkspace-1.2.213.tar", last modified: Sun Jun  2 12:18:17 2024, max compression
```

## Comparing `simpleworkspace-1.2.212.tar` & `simpleworkspace-1.2.213.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.513763 simpleworkspace-1.2.212/
--rw-rw-rw-   0        0        0       22 2024-02-04 07:50:01.000000 simpleworkspace-1.2.212/MANIFEST.in
--rw-rw-rw-   0        0        0      177 2024-06-02 11:59:32.511768 simpleworkspace-1.2.212/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-06-02 11:58:14.000000 simpleworkspace-1.2.212/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-02 11:59:32.514760 simpleworkspace-1.2.212/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.248865 simpleworkspace-1.2.212/src/
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.283775 simpleworkspace-1.2.212/src/simpleworkspace/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.212/src/simpleworkspace/__init__.py
--rw-rw-rw-   0        0        0      453 2023-12-12 17:24:38.000000 simpleworkspace-1.2.212/src/simpleworkspace/__lazyimporter__.py
--rw-rw-rw-   0        0        0     2238 2024-06-02 11:57:50.000000 simpleworkspace-1.2.212/src/simpleworkspace/app.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.302242 simpleworkspace-1.2.212/src/simpleworkspace/assets/
--rw-rw-rw-   0        0        0      561 2024-02-26 13:54:52.000000 simpleworkspace-1.2.212/src/simpleworkspace/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.304236 simpleworkspace-1.2.212/src/simpleworkspace/assets/__pycache__/
--rw-rw-rw-   0        0        0      890 2024-04-15 18:36:31.000000 simpleworkspace-1.2.212/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.253851 simpleworkspace-1.2.212/src/simpleworkspace/assets/audio/
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.313235 simpleworkspace-1.2.212/src/simpleworkspace/assets/audio/alarms/
--rw-rw-rw-   0        0        0   115582 2024-02-26 13:54:53.000000 simpleworkspace-1.2.212/src/simpleworkspace/assets/audio/alarms/Siren.wav
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.332211 simpleworkspace-1.2.212/src/simpleworkspace/assets/audio/notifications/
--rw-rw-rw-   0        0        0   168352 2024-02-26 13:54:53.000000 simpleworkspace-1.2.212/src/simpleworkspace/assets/audio/notifications/Completed.wav
--rw-rw-rw-   0        0        0   159276 2024-02-26 13:54:53.000000 simpleworkspace-1.2.212/src/simpleworkspace/assets/audio/notifications/Error.wav
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.369118 simpleworkspace-1.2.212/src/simpleworkspace/assets/icons/
--rw-rw-rw-   0        0        0      864 2024-01-22 19:10:19.000000 simpleworkspace-1.2.212/src/simpleworkspace/assets/icons/ErrorCircle.png
--rw-rw-rw-   0        0        0      738 2024-01-22 19:10:19.000000 simpleworkspace-1.2.212/src/simpleworkspace/assets/icons/InfoCircle.png
--rw-rw-rw-   0        0        0      913 2024-01-22 19:10:19.000000 simpleworkspace-1.2.212/src/simpleworkspace/assets/icons/QuestionCircle.png
--rw-rw-rw-   0        0        0      643 2024-01-22 19:10:19.000000 simpleworkspace-1.2.212/src/simpleworkspace/assets/icons/WarningCircle.png
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.379094 simpleworkspace-1.2.212/src/simpleworkspace/collections/
--rw-rw-rw-   0        0        0        0 2023-12-09 17:26:55.000000 simpleworkspace-1.2.212/src/simpleworkspace/collections/__init__.py
--rw-rw-rw-   0        0        0      217 2023-12-12 17:24:38.000000 simpleworkspace-1.2.212/src/simpleworkspace/collections/loader.py
--rw-rw-rw-   0        0        0     8357 2023-12-23 08:45:05.000000 simpleworkspace-1.2.212/src/simpleworkspace/collections/observables.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.387070 simpleworkspace-1.2.212/src/simpleworkspace/db/
--rw-rw-rw-   0        0        0        0 2023-09-28 08:23:03.000000 simpleworkspace-1.2.212/src/simpleworkspace/db/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-11-25 10:02:31.000000 simpleworkspace-1.2.212/src/simpleworkspace/db/dbfactory.py
--rw-rw-rw-   0        0        0    26868 2024-01-17 11:30:30.000000 simpleworkspace-1.2.212/src/simpleworkspace/db/fluentsqlbuilder.py
--rw-rw-rw-   0        0        0      356 2023-12-12 17:24:38.000000 simpleworkspace-1.2.212/src/simpleworkspace/db/loader.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.392571 simpleworkspace-1.2.212/src/simpleworkspace/gui/
--rw-rw-rw-   0        0        0        0 2024-01-17 11:30:30.000000 simpleworkspace-1.2.212/src/simpleworkspace/gui/__init__.py
--rw-rw-rw-   0        0        0    19745 2024-02-04 07:50:01.000000 simpleworkspace-1.2.212/src/simpleworkspace/gui/dialogs.py
--rw-rw-rw-   0        0        0      199 2024-01-17 11:30:30.000000 simpleworkspace-1.2.212/src/simpleworkspace/gui/loader.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.400550 simpleworkspace-1.2.212/src/simpleworkspace/io/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.404539 simpleworkspace-1.2.212/src/simpleworkspace/io/audio/
--rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/audio/__init__.py
--rw-rw-rw-   0        0        0      184 2024-02-26 13:54:53.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/audio/loader.py
--rw-rw-rw-   0        0        0      720 2024-02-26 13:54:53.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/audio/play.py
--rw-rw-rw-   0        0        0     5574 2024-02-28 14:44:32.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/directory.py
--rw-rw-rw-   0        0        0     4101 2024-05-21 14:04:11.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/file.py
--rw-rw-rw-   0        0        0      603 2024-05-09 13:34:22.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/loader.py
--rw-rw-rw-   0        0        0     6180 2024-05-21 14:04:11.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/path.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.411520 simpleworkspace-1.2.212/src/simpleworkspace/io/readers/
--rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/readers/__init__.py
--rw-rw-rw-   0        0        0    13750 2024-05-21 14:04:11.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/readers/archive.py
--rw-rw-rw-   0        0        0     6265 2024-02-17 14:57:41.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/readers/csvreader.py
--rw-rw-rw-   0        0        0      423 2024-05-09 13:34:11.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/readers/loader.py
--rw-rw-rw-   0        0        0     2637 2024-02-26 13:54:53.000000 simpleworkspace-1.2.212/src/simpleworkspace/io/readers/logreader.py
--rw-rw-rw-   0        0        0     1256 2024-01-19 20:03:47.000000 simpleworkspace-1.2.212/src/simpleworkspace/loader.py
--rw-rw-rw-   0        0        0     6464 2024-02-04 13:21:24.000000 simpleworkspace-1.2.212/src/simpleworkspace/logproviders.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.269809 simpleworkspace-1.2.212/src/simpleworkspace/packages/
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.413515 simpleworkspace-1.2.212/src/simpleworkspace/packages/debug/
--rw-rw-rw-   0        0        0     2163 2024-02-04 07:50:01.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/debug/profiler.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.262827 simpleworkspace-1.2.212/src/simpleworkspace/packages/network/
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.264823 simpleworkspace-1.2.212/src/simpleworkspace/packages/network/servers/
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.416506 simpleworkspace-1.2.212/src/simpleworkspace/packages/network/servers/basicserver/
--rw-rw-rw-   0        0        0       71 2024-05-08 15:33:14.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.417504 simpleworkspace-1.2.212/src/simpleworkspace/packages/network/servers/basicserver/model/
--rw-rw-rw-   0        0        0     3293 2024-05-08 15:33:14.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
--rw-rw-rw-   0        0        0     9530 2024-05-08 15:33:14.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/network/servers/basicserver/server.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.419498 simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.420496 simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/
--rw-rw-rw-   0        0        0        0 2024-02-04 07:50:01.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.457399 simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
--rw-rw-rw-   0        0        0      717 2024-02-04 07:50:01.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
--rw-rw-rw-   0        0        0    38758 2024-02-04 07:50:01.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
--rw-rw-rw-   0        0        0     9974 2024-02-04 07:50:01.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
--rw-rw-rw-   0        0        0      348 2024-02-04 07:50:01.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
--rw-rw-rw-   0        0        0      768 2024-02-04 07:50:01.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
--rw-rw-rw-   0        0        0     4889 2024-06-02 08:30:18.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.463383 simpleworkspace-1.2.212/src/simpleworkspace/packages/taskscheduler/
--rw-rw-rw-   0        0        0       79 2023-09-16 11:15:10.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/taskscheduler/__init__.py
--rw-rw-rw-   0        0        0     8955 2024-05-08 15:33:14.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/taskscheduler/manager.py
--rw-rw-rw-   0        0        0     5302 2024-05-21 14:04:11.000000 simpleworkspace-1.2.212/src/simpleworkspace/packages/taskscheduler/model.py
--rw-rw-rw-   0        0        0     7383 2024-02-17 14:57:41.000000 simpleworkspace-1.2.212/src/simpleworkspace/settingsproviders.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.473356 simpleworkspace-1.2.212/src/simpleworkspace/types/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.212/src/simpleworkspace/types/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-02-17 14:57:41.000000 simpleworkspace-1.2.212/src/simpleworkspace/types/byte.py
--rw-rw-rw-   0        0        0     5736 2023-07-26 09:23:24.000000 simpleworkspace-1.2.212/src/simpleworkspace/types/iunit.py
--rw-rw-rw-   0        0        0      471 2023-12-12 17:24:38.000000 simpleworkspace-1.2.212/src/simpleworkspace/types/loader.py
--rw-rw-rw-   0        0        0      932 2023-07-26 09:23:24.000000 simpleworkspace-1.2.212/src/simpleworkspace/types/measurement.py
--rw-rw-rw-   0        0        0      556 2024-03-10 14:41:22.000000 simpleworkspace-1.2.212/src/simpleworkspace/types/os.py
--rw-rw-rw-   0        0        0     8342 2024-05-08 15:33:14.000000 simpleworkspace-1.2.212/src/simpleworkspace/types/time.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.503789 simpleworkspace-1.2.212/src/simpleworkspace/utility/
--rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/__init__.py
--rw-rw-rw-   0        0        0      237 2023-04-09 11:23:10.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/bytes.py
--rw-rw-rw-   0        0        0     1916 2024-05-08 15:33:14.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/cache.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.507778 simpleworkspace-1.2.212/src/simpleworkspace/utility/concurrent/
--rw-rw-rw-   0        0        0      305 2024-06-02 08:24:36.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/concurrent/loader.py
--rw-rw-rw-   0        0        0     5849 2024-06-02 11:55:04.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/concurrent/locking.py
--rw-rw-rw-   0        0        0     1798 2024-06-02 08:26:06.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/concurrent/parallel.py
--rw-rw-rw-   0        0        0     7735 2024-02-11 09:17:40.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/console.py
--rw-rw-rw-   0        0        0     3157 2024-05-21 14:04:11.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/encryption.py
--rw-rw-rw-   0        0        0    14504 2024-05-08 15:33:14.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/linq.py
--rw-rw-rw-   0        0        0     1125 2024-06-02 08:25:43.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/loader.py
--rw-rw-rw-   0        0        0     4548 2024-03-03 10:52:37.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/module.py
--rw-rw-rw-   0        0        0    11289 2024-05-21 14:04:11.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/progressbar.py
--rw-rw-rw-   0        0        0     7218 2024-02-19 19:08:03.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/regex.py
--rw-rw-rw-   0        0        0     1897 2024-05-08 15:33:14.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/strings.py
--rw-rw-rw-   0        0        0     6760 2024-05-08 15:33:14.000000 simpleworkspace-1.2.212/src/simpleworkspace/utility/time.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:59:32.510770 simpleworkspace-1.2.212/src/simpleworkspace.egg-info/
--rw-rw-rw-   0        0        0      177 2024-06-02 11:59:32.000000 simpleworkspace-1.2.212/src/simpleworkspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3560 2024-06-02 11:59:32.000000 simpleworkspace-1.2.212/src/simpleworkspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 11:59:32.000000 simpleworkspace-1.2.212/src/simpleworkspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-06-02 11:59:32.000000 simpleworkspace-1.2.212/src/simpleworkspace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-06-02 11:59:32.000000 simpleworkspace-1.2.212/src/simpleworkspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:17.003709 simpleworkspace-1.2.213/
+-rw-rw-rw-   0        0        0       22 2024-02-04 07:50:01.000000 simpleworkspace-1.2.213/MANIFEST.in
+-rw-rw-rw-   0        0        0      177 2024-06-02 12:18:17.000720 simpleworkspace-1.2.213/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-06-02 12:17:05.000000 simpleworkspace-1.2.213/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 12:18:17.003709 simpleworkspace-1.2.213/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.734197 simpleworkspace-1.2.213/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.768935 simpleworkspace-1.2.213/src/simpleworkspace/
+-rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.213/src/simpleworkspace/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-12-12 17:24:38.000000 simpleworkspace-1.2.213/src/simpleworkspace/__lazyimporter__.py
+-rw-rw-rw-   0        0        0     2238 2024-06-02 11:57:50.000000 simpleworkspace-1.2.213/src/simpleworkspace/app.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.866134 simpleworkspace-1.2.213/src/simpleworkspace/assets/
+-rw-rw-rw-   0        0        0      561 2024-02-26 13:54:52.000000 simpleworkspace-1.2.213/src/simpleworkspace/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.868128 simpleworkspace-1.2.213/src/simpleworkspace/assets/__pycache__/
+-rw-rw-rw-   0        0        0      890 2024-04-15 18:36:31.000000 simpleworkspace-1.2.213/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.740185 simpleworkspace-1.2.213/src/simpleworkspace/assets/audio/
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.870123 simpleworkspace-1.2.213/src/simpleworkspace/assets/audio/alarms/
+-rw-rw-rw-   0        0        0   115582 2024-02-26 13:54:53.000000 simpleworkspace-1.2.213/src/simpleworkspace/assets/audio/alarms/Siren.wav
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.875109 simpleworkspace-1.2.213/src/simpleworkspace/assets/audio/notifications/
+-rw-rw-rw-   0        0        0   168352 2024-02-26 13:54:53.000000 simpleworkspace-1.2.213/src/simpleworkspace/assets/audio/notifications/Completed.wav
+-rw-rw-rw-   0        0        0   159276 2024-02-26 13:54:53.000000 simpleworkspace-1.2.213/src/simpleworkspace/assets/audio/notifications/Error.wav
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.882090 simpleworkspace-1.2.213/src/simpleworkspace/assets/icons/
+-rw-rw-rw-   0        0        0      864 2024-01-22 19:10:19.000000 simpleworkspace-1.2.213/src/simpleworkspace/assets/icons/ErrorCircle.png
+-rw-rw-rw-   0        0        0      738 2024-01-22 19:10:19.000000 simpleworkspace-1.2.213/src/simpleworkspace/assets/icons/InfoCircle.png
+-rw-rw-rw-   0        0        0      913 2024-01-22 19:10:19.000000 simpleworkspace-1.2.213/src/simpleworkspace/assets/icons/QuestionCircle.png
+-rw-rw-rw-   0        0        0      643 2024-01-22 19:10:19.000000 simpleworkspace-1.2.213/src/simpleworkspace/assets/icons/WarningCircle.png
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.886080 simpleworkspace-1.2.213/src/simpleworkspace/collections/
+-rw-rw-rw-   0        0        0        0 2023-12-09 17:26:55.000000 simpleworkspace-1.2.213/src/simpleworkspace/collections/__init__.py
+-rw-rw-rw-   0        0        0      217 2023-12-12 17:24:38.000000 simpleworkspace-1.2.213/src/simpleworkspace/collections/loader.py
+-rw-rw-rw-   0        0        0     8357 2023-12-23 08:45:05.000000 simpleworkspace-1.2.213/src/simpleworkspace/collections/observables.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.893062 simpleworkspace-1.2.213/src/simpleworkspace/db/
+-rw-rw-rw-   0        0        0        0 2023-09-28 08:23:03.000000 simpleworkspace-1.2.213/src/simpleworkspace/db/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-11-25 10:02:31.000000 simpleworkspace-1.2.213/src/simpleworkspace/db/dbfactory.py
+-rw-rw-rw-   0        0        0    26868 2024-01-17 11:30:30.000000 simpleworkspace-1.2.213/src/simpleworkspace/db/fluentsqlbuilder.py
+-rw-rw-rw-   0        0        0      356 2023-12-12 17:24:38.000000 simpleworkspace-1.2.213/src/simpleworkspace/db/loader.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.897050 simpleworkspace-1.2.213/src/simpleworkspace/gui/
+-rw-rw-rw-   0        0        0        0 2024-01-17 11:30:30.000000 simpleworkspace-1.2.213/src/simpleworkspace/gui/__init__.py
+-rw-rw-rw-   0        0        0    19745 2024-02-04 07:50:01.000000 simpleworkspace-1.2.213/src/simpleworkspace/gui/dialogs.py
+-rw-rw-rw-   0        0        0      199 2024-01-17 11:30:30.000000 simpleworkspace-1.2.213/src/simpleworkspace/gui/loader.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.903035 simpleworkspace-1.2.213/src/simpleworkspace/io/
+-rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.908022 simpleworkspace-1.2.213/src/simpleworkspace/io/audio/
+-rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/audio/__init__.py
+-rw-rw-rw-   0        0        0      184 2024-02-26 13:54:53.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/audio/loader.py
+-rw-rw-rw-   0        0        0      720 2024-02-26 13:54:53.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/audio/play.py
+-rw-rw-rw-   0        0        0     5574 2024-02-28 14:44:32.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/directory.py
+-rw-rw-rw-   0        0        0     4101 2024-05-21 14:04:11.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/file.py
+-rw-rw-rw-   0        0        0      603 2024-05-09 13:34:22.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/loader.py
+-rw-rw-rw-   0        0        0     6180 2024-05-21 14:04:11.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/path.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.914006 simpleworkspace-1.2.213/src/simpleworkspace/io/readers/
+-rw-rw-rw-   0        0        0        0 2024-02-26 13:54:53.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/readers/__init__.py
+-rw-rw-rw-   0        0        0    13750 2024-05-21 14:04:11.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/readers/archive.py
+-rw-rw-rw-   0        0        0     6265 2024-02-17 14:57:41.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/readers/csvreader.py
+-rw-rw-rw-   0        0        0      423 2024-05-09 13:34:11.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/readers/loader.py
+-rw-rw-rw-   0        0        0     2637 2024-02-26 13:54:53.000000 simpleworkspace-1.2.213/src/simpleworkspace/io/readers/logreader.py
+-rw-rw-rw-   0        0        0     1256 2024-01-19 20:03:47.000000 simpleworkspace-1.2.213/src/simpleworkspace/loader.py
+-rw-rw-rw-   0        0        0     6464 2024-02-04 13:21:24.000000 simpleworkspace-1.2.213/src/simpleworkspace/logproviders.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.753152 simpleworkspace-1.2.213/src/simpleworkspace/packages/
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.916000 simpleworkspace-1.2.213/src/simpleworkspace/packages/debug/
+-rw-rw-rw-   0        0        0     2163 2024-02-04 07:50:01.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/debug/profiler.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.749161 simpleworkspace-1.2.213/src/simpleworkspace/packages/network/
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.750158 simpleworkspace-1.2.213/src/simpleworkspace/packages/network/servers/
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.917994 simpleworkspace-1.2.213/src/simpleworkspace/packages/network/servers/basicserver/
+-rw-rw-rw-   0        0        0       71 2024-05-08 15:33:14.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.919988 simpleworkspace-1.2.213/src/simpleworkspace/packages/network/servers/basicserver/model/
+-rw-rw-rw-   0        0        0     3293 2024-05-08 15:33:14.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
+-rw-rw-rw-   0        0        0     9530 2024-05-08 15:33:14.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/network/servers/basicserver/server.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.922982 simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.923978 simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/
+-rw-rw-rw-   0        0        0        0 2024-02-04 07:50:01.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.931957 simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
+-rw-rw-rw-   0        0        0      717 2024-02-04 07:50:01.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
+-rw-rw-rw-   0        0        0    38758 2024-02-04 07:50:01.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
+-rw-rw-rw-   0        0        0     9974 2024-02-04 07:50:01.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
+-rw-rw-rw-   0        0        0      348 2024-02-04 07:50:01.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
+-rw-rw-rw-   0        0        0      768 2024-02-04 07:50:01.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
+-rw-rw-rw-   0        0        0     4889 2024-06-02 08:30:18.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.935946 simpleworkspace-1.2.213/src/simpleworkspace/packages/taskscheduler/
+-rw-rw-rw-   0        0        0       79 2023-09-16 11:15:10.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/taskscheduler/__init__.py
+-rw-rw-rw-   0        0        0     8955 2024-05-08 15:33:14.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/taskscheduler/manager.py
+-rw-rw-rw-   0        0        0     5302 2024-05-21 14:04:11.000000 simpleworkspace-1.2.213/src/simpleworkspace/packages/taskscheduler/model.py
+-rw-rw-rw-   0        0        0     7383 2024-02-17 14:57:41.000000 simpleworkspace-1.2.213/src/simpleworkspace/settingsproviders.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.946920 simpleworkspace-1.2.213/src/simpleworkspace/types/
+-rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.213/src/simpleworkspace/types/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-02-17 14:57:41.000000 simpleworkspace-1.2.213/src/simpleworkspace/types/byte.py
+-rw-rw-rw-   0        0        0     5736 2023-07-26 09:23:24.000000 simpleworkspace-1.2.213/src/simpleworkspace/types/iunit.py
+-rw-rw-rw-   0        0        0      471 2023-12-12 17:24:38.000000 simpleworkspace-1.2.213/src/simpleworkspace/types/loader.py
+-rw-rw-rw-   0        0        0      932 2023-07-26 09:23:24.000000 simpleworkspace-1.2.213/src/simpleworkspace/types/measurement.py
+-rw-rw-rw-   0        0        0      556 2024-03-10 14:41:22.000000 simpleworkspace-1.2.213/src/simpleworkspace/types/os.py
+-rw-rw-rw-   0        0        0     8342 2024-05-08 15:33:14.000000 simpleworkspace-1.2.213/src/simpleworkspace/types/time.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.981772 simpleworkspace-1.2.213/src/simpleworkspace/utility/
+-rw-rw-rw-   0        0        0        0 2023-07-30 11:39:31.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-04-09 11:23:10.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/bytes.py
+-rw-rw-rw-   0        0        0     1916 2024-05-08 15:33:14.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/cache.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.994736 simpleworkspace-1.2.213/src/simpleworkspace/utility/concurrent/
+-rw-rw-rw-   0        0        0      305 2024-06-02 08:24:36.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/concurrent/loader.py
+-rw-rw-rw-   0        0        0     6124 2024-06-02 12:08:46.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/concurrent/locking.py
+-rw-rw-rw-   0        0        0     1798 2024-06-02 08:26:06.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/concurrent/parallel.py
+-rw-rw-rw-   0        0        0     7735 2024-02-11 09:17:40.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/console.py
+-rw-rw-rw-   0        0        0     3157 2024-05-21 14:04:11.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/encryption.py
+-rw-rw-rw-   0        0        0    14504 2024-05-08 15:33:14.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/linq.py
+-rw-rw-rw-   0        0        0     1125 2024-06-02 08:25:43.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/loader.py
+-rw-rw-rw-   0        0        0     4548 2024-03-03 10:52:37.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/module.py
+-rw-rw-rw-   0        0        0    11289 2024-05-21 14:04:11.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/progressbar.py
+-rw-rw-rw-   0        0        0     7218 2024-02-19 19:08:03.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/regex.py
+-rw-rw-rw-   0        0        0     1897 2024-05-08 15:33:14.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/strings.py
+-rw-rw-rw-   0        0        0     6760 2024-05-08 15:33:14.000000 simpleworkspace-1.2.213/src/simpleworkspace/utility/time.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:18:16.998723 simpleworkspace-1.2.213/src/simpleworkspace.egg-info/
+-rw-rw-rw-   0        0        0      177 2024-06-02 12:18:16.000000 simpleworkspace-1.2.213/src/simpleworkspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3560 2024-06-02 12:18:16.000000 simpleworkspace-1.2.213/src/simpleworkspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 12:18:16.000000 simpleworkspace-1.2.213/src/simpleworkspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-06-02 12:18:16.000000 simpleworkspace-1.2.213/src/simpleworkspace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-06-02 12:18:16.000000 simpleworkspace-1.2.213/src/simpleworkspace.egg-info/top_level.txt
```

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/app.py` & `simpleworkspace-1.2.213/src/simpleworkspace/app.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/assets/__init__.py` & `simpleworkspace-1.2.213/src/simpleworkspace/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc` & `simpleworkspace-1.2.213/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/assets/audio/alarms/Siren.wav` & `simpleworkspace-1.2.213/src/simpleworkspace/assets/audio/alarms/Siren.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/assets/audio/notifications/Completed.wav` & `simpleworkspace-1.2.213/src/simpleworkspace/assets/audio/notifications/Completed.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/assets/audio/notifications/Error.wav` & `simpleworkspace-1.2.213/src/simpleworkspace/assets/audio/notifications/Error.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/assets/icons/ErrorCircle.png` & `simpleworkspace-1.2.213/src/simpleworkspace/assets/icons/ErrorCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/assets/icons/InfoCircle.png` & `simpleworkspace-1.2.213/src/simpleworkspace/assets/icons/InfoCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/assets/icons/QuestionCircle.png` & `simpleworkspace-1.2.213/src/simpleworkspace/assets/icons/QuestionCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/assets/icons/WarningCircle.png` & `simpleworkspace-1.2.213/src/simpleworkspace/assets/icons/WarningCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/collections/observables.py` & `simpleworkspace-1.2.213/src/simpleworkspace/collections/observables.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/db/dbfactory.py` & `simpleworkspace-1.2.213/src/simpleworkspace/db/dbfactory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/db/fluentsqlbuilder.py` & `simpleworkspace-1.2.213/src/simpleworkspace/db/fluentsqlbuilder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/gui/dialogs.py` & `simpleworkspace-1.2.213/src/simpleworkspace/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/io/audio/play.py` & `simpleworkspace-1.2.213/src/simpleworkspace/io/audio/play.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/io/directory.py` & `simpleworkspace-1.2.213/src/simpleworkspace/io/directory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/io/file.py` & `simpleworkspace-1.2.213/src/simpleworkspace/io/file.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/io/loader.py` & `simpleworkspace-1.2.213/src/simpleworkspace/io/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/io/path.py` & `simpleworkspace-1.2.213/src/simpleworkspace/io/path.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/io/readers/archive.py` & `simpleworkspace-1.2.213/src/simpleworkspace/io/readers/archive.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/io/readers/csvreader.py` & `simpleworkspace-1.2.213/src/simpleworkspace/io/readers/csvreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/io/readers/logreader.py` & `simpleworkspace-1.2.213/src/simpleworkspace/io/readers/logreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/loader.py` & `simpleworkspace-1.2.213/src/simpleworkspace/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/logproviders.py` & `simpleworkspace-1.2.213/src/simpleworkspace/logproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/packages/debug/profiler.py` & `simpleworkspace-1.2.213/src/simpleworkspace/packages/debug/profiler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py` & `simpleworkspace-1.2.213/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/packages/network/servers/basicserver/server.py` & `simpleworkspace-1.2.213/src/simpleworkspace/packages/network/servers/basicserver/server.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py` & `simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py` & `simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py` & `simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py` & `simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py` & `simpleworkspace-1.2.213/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/packages/taskscheduler/manager.py` & `simpleworkspace-1.2.213/src/simpleworkspace/packages/taskscheduler/manager.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/packages/taskscheduler/model.py` & `simpleworkspace-1.2.213/src/simpleworkspace/packages/taskscheduler/model.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/settingsproviders.py` & `simpleworkspace-1.2.213/src/simpleworkspace/settingsproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/types/byte.py` & `simpleworkspace-1.2.213/src/simpleworkspace/types/byte.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/types/iunit.py` & `simpleworkspace-1.2.213/src/simpleworkspace/types/iunit.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/types/measurement.py` & `simpleworkspace-1.2.213/src/simpleworkspace/types/measurement.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/types/os.py` & `simpleworkspace-1.2.213/src/simpleworkspace/types/os.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/types/time.py` & `simpleworkspace-1.2.213/src/simpleworkspace/types/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/cache.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/cache.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/concurrent/locking.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/concurrent/locking.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os as _os
 from simpleworkspace.types.os import OperatingSystemEnum as _OperatingSystemEnum
 from typing import cast as _cast
 import errno as _errno
 from contextlib import suppress as _suppress
+from simpleworkspace.types.time import TimeSpan as _TimeSpan
 
 class FileLock:
     """Create a system-wide exclusive lock for a given global name."""
 
     def __init__(self, id: str) -> None:
         import simpleworkspace.io.file, tempfile
 
@@ -86,15 +87,20 @@
         self._context_lock_fh = None
         msvcrt.locking(fh, msvcrt.LK_UNLCK, 1)
         _os.close(fh)
 
         with _suppress(OSError):  # Probably another instance of the application had acquired the file lock.
             _os.unlink(self.lock_file)
     
-    def Acquire(self, blocking=False, timeoutMS=None):
+    def Acquire(self, blocking=False, timeout:int=None):
+        """Tries to aquire a system wide file lock
+
+        :param blocking: when blocking is true, waits until a lock is received or timeout
+        :param timeout: total seconds to wait before timing out
+        """
         import time
         from simpleworkspace.utility.time import StopWatch
 
         if(self.IsLocked):
             return
     
         stopwatch = StopWatch()
@@ -106,16 +112,16 @@
             
             if(self.IsLocked):
                 break
 
             if(blocking is False):
                 raise TimeoutError(f'Failed to immediately acquire lock on "{self.id}"')
 
-            if(timeoutMS is not None) and (stopwatch.GetElapsedMilliseconds() > timeoutMS):
-                raise TimeoutError(f'Timeout acquiring lock on {self.id} for {timeoutMS} MS')
+            if(timeout is not None) and (stopwatch.GetElapsedSeconds() > timeout):
+                raise TimeoutError(f'Timeout acquiring lock on {self.id} for {timeout} seconds')
             
             time.sleep(1)
 
     def Release(self):
         if(not self.IsLocked):
             return
```

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/concurrent/parallel.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/concurrent/parallel.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/console.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/console.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/encryption.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/encryption.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/linq.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/linq.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/loader.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/module.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/module.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/progressbar.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/progressbar.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/regex.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/regex.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/strings.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/strings.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace/utility/time.py` & `simpleworkspace-1.2.213/src/simpleworkspace/utility/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.212/src/simpleworkspace.egg-info/SOURCES.txt` & `simpleworkspace-1.2.213/src/simpleworkspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

