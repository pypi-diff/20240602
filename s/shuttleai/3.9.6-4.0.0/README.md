# Comparing `tmp/shuttleai-3.9.6.tar.gz` & `tmp/shuttleai-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.9.6.tar", last modified: Sat May 18 00:04:10 2024, max compression
+gzip compressed data, was "shuttleai-4.0.0.tar", max compression
```

## Comparing `shuttleai-3.9.6.tar` & `shuttleai-4.0.0.tar`

### file list

```diff
@@ -1,26 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 00:04:10.183763 shuttleai-3.9.6/
--rw-rw-rw-   0        0        0     4116 2024-05-18 00:04:10.176223 shuttleai-3.9.6/PKG-INFO
--rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.9.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-18 00:04:10.184761 shuttleai-3.9.6/setup.cfg
--rw-rw-rw-   0        0        0     1274 2024-05-18 00:03:00.000000 shuttleai-3.9.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 00:04:10.057989 shuttleai-3.9.6/shuttleai/
--rw-rw-rw-   0        0        0     1781 2024-04-27 00:33:36.000000 shuttleai-3.9.6/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.9.6/shuttleai/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-18 00:04:10.144561 shuttleai-3.9.6/shuttleai/client/
--rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.9.6/shuttleai/client/__init__.py
--rw-rw-rw-   0        0        0    17390 2024-05-18 00:02:49.000000 shuttleai-3.9.6/shuttleai/client/_async.py
--rw-rw-rw-   0        0        0    15212 2024-05-18 00:02:56.000000 shuttleai-3.9.6/shuttleai/client/_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-18 00:04:10.155119 shuttleai-3.9.6/shuttleai/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-27 00:24:28.000000 shuttleai-3.9.6/shuttleai/helpers/__init__.py
--rw-rw-rw-   0        0        0     2726 2024-04-27 00:26:00.000000 shuttleai-3.9.6/shuttleai/helpers/tool_calls.py
--rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.9.6/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-05-18 00:04:10.163663 shuttleai-3.9.6/shuttleai/schemas/
--rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.9.6/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     4108 2024-04-05 22:32:01.000000 shuttleai-3.9.6/shuttleai/schemas/schemas.py
-drwxrwxrwx   0        0        0        0 2024-05-18 00:04:10.168663 shuttleai-3.9.6/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     4116 2024-05-18 00:04:09.000000 shuttleai-3.9.6/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2024-05-18 00:04:09.000000 shuttleai-3.9.6/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 00:04:09.000000 shuttleai-3.9.6/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-18 00:04:09.000000 shuttleai-3.9.6/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2024-05-18 00:04:09.000000 shuttleai-3.9.6/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 00:04:09.000000 shuttleai-3.9.6/shuttleai.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1154 2024-06-02 04:27:26.093048 shuttleai-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0       33 2024-06-02 04:27:14.656264 shuttleai-4.0.0/README.md
+-rw-r--r--   0        0        0      167 2024-06-02 04:26:47.729775 shuttleai-4.0.0/shuttleai/__init__.py
+-rw-r--r--   0        0        0      824 2024-06-02 00:32:35.919932 shuttleai-4.0.0/shuttleai/_patch.py
+-rw-r--r--   0        0        0       76 2024-06-02 02:18:27.148187 shuttleai-4.0.0/shuttleai/client/__init__.py
+-rw-r--r--   0        0        0     6648 2024-06-02 04:04:56.617130 shuttleai-4.0.0/shuttleai/client/_async.py
+-rw-r--r--   0        0        0     6689 2024-06-02 04:06:06.921779 shuttleai-4.0.0/shuttleai/client/_sync.py
+-rw-r--r--   0        0        0     4541 2024-06-02 02:11:48.388511 shuttleai-4.0.0/shuttleai/client/base.py
+-rw-r--r--   0        0        0     1823 2024-06-02 00:35:28.615546 shuttleai-4.0.0/shuttleai/exceptions.py
+-rw-r--r--   0        0        0        0 2024-06-01 20:20:33.018948 shuttleai-4.0.0/shuttleai/py.typed
+-rw-r--r--   0        0        0       50 2024-06-02 02:15:22.440205 shuttleai-4.0.0/shuttleai/resources/__init__.py
+-rw-r--r--   0        0        0     5506 2024-06-02 01:46:04.821287 shuttleai-4.0.0/shuttleai/resources/chat.py
+-rw-r--r--   0        0        0     1640 2024-06-02 02:14:53.228145 shuttleai-4.0.0/shuttleai/resources/images.py
+-rw-r--r--   0        0        0        0 2024-06-01 20:25:06.853579 shuttleai-4.0.0/shuttleai/schemas/__init__.py
+-rw-r--r--   0        0        0     1751 2024-06-01 21:04:09.631938 shuttleai-4.0.0/shuttleai/schemas/chat_completion.py
+-rw-r--r--   0        0        0      294 2024-06-02 04:02:12.707552 shuttleai-4.0.0/shuttleai/schemas/common.py
+-rw-r--r--   0        0        0      391 2024-06-02 01:52:38.540553 shuttleai-4.0.0/shuttleai/schemas/images_generations.py
+-rw-r--r--   0        0        0        0 2024-06-01 20:47:13.984891 shuttleai-4.0.0/shuttleai/schemas/models/__init__.py
+-rw-r--r--   0        0        0     1006 2024-06-02 01:49:21.629939 shuttleai-4.0.0/shuttleai/schemas/models/capabilities.py
+-rw-r--r--   0        0        0     2672 2024-06-02 01:50:20.883859 shuttleai-4.0.0/shuttleai/schemas/models/models.py
+-rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 shuttleai-4.0.0/PKG-INFO
```

