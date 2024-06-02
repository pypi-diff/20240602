# Comparing `tmp/copilothistoryexporter-1.0.2.9.tar.gz` & `tmp/copilothistoryexporter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/copilothistoryexporter-1.0.2.9.tar", last modified: Sun Jun  2 19:12:59 2024, max compression
+gzip compressed data, was "copilothistoryexporter-1.0.3.tar", last modified: Sun Jun  2 19:34:28 2024, max compression
```

## Comparing `copilothistoryexporter-1.0.2.9.tar` & `copilothistoryexporter-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 19:12:59.000000 copilothistoryexporter-1.0.2.9/
-drwxr-xr-x   0 mustafakilic   (501) staff       (20)        0 2024-06-02 19:12:59.000000 copilothistoryexporter-1.0.2.9/copilothistoryexporter.egg-info/
--rw-r--r--   0 mustafakilic   (501) staff       (20)      375 2024-06-02 19:12:59.000000 copilothistoryexporter-1.0.2.9/copilothistoryexporter.egg-info/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)      296 2024-06-02 19:12:59.000000 copilothistoryexporter-1.0.2.9/copilothistoryexporter.egg-info/SOURCES.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       81 2024-06-02 19:12:59.000000 copilothistoryexporter-1.0.2.9/copilothistoryexporter.egg-info/entry_points.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)       58 2024-06-02 19:12:59.000000 copilothistoryexporter-1.0.2.9/copilothistoryexporter.egg-info/requires.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 19:12:59.000000 copilothistoryexporter-1.0.2.9/copilothistoryexporter.egg-info/top_level.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)        1 2024-06-02 19:12:59.000000 copilothistoryexporter-1.0.2.9/copilothistoryexporter.egg-info/dependency_links.txt
--rw-r--r--   0 mustafakilic   (501) staff       (20)      375 2024-06-02 19:12:59.000000 copilothistoryexporter-1.0.2.9/PKG-INFO
--rw-r--r--   0 mustafakilic   (501) staff       (20)     2232 2024-06-02 16:13:30.000000 copilothistoryexporter-1.0.2.9/README.md
--rw-r--r--   0 mustafakilic   (501) staff       (20)      730 2024-06-02 19:12:49.000000 copilothistoryexporter-1.0.2.9/setup.py
--rw-r--r--   0 mustafakilic   (501) staff       (20)       38 2024-06-02 19:12:59.000000 copilothistoryexporter-1.0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:34:28.306039 copilothistoryexporter-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 19:34:08.000000 copilothistoryexporter-1.0.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-06-02 19:34:28.306039 copilothistoryexporter-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-06-02 19:34:08.000000 copilothistoryexporter-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:34:28.306039 copilothistoryexporter-1.0.3/copilothistoryexporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-06-02 19:34:28.000000 copilothistoryexporter-1.0.3/copilothistoryexporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-02 19:34:28.000000 copilothistoryexporter-1.0.3/copilothistoryexporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:34:28.000000 copilothistoryexporter-1.0.3/copilothistoryexporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 19:34:28.000000 copilothistoryexporter-1.0.3/copilothistoryexporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-02 19:34:28.000000 copilothistoryexporter-1.0.3/copilothistoryexporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:34:28.000000 copilothistoryexporter-1.0.3/copilothistoryexporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 19:34:28.306039 copilothistoryexporter-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-06-02 19:34:08.000000 copilothistoryexporter-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `copilothistoryexporter-1.0.2.9/README.md` & `copilothistoryexporter-1.0.3/README.md`

 * *Files identical despite different names*

