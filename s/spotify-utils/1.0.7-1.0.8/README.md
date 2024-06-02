# Comparing `tmp/spotify_utils-1.0.7.tar.gz` & `tmp/spotify_utils-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_utils-1.0.7.tar", max compression
+gzip compressed data, was "spotify_utils-1.0.8.tar", max compression
```

## Comparing `spotify_utils-1.0.7.tar` & `spotify_utils-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34888 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/LICENSE
--rw-r--r--   0        0        0     7570 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/README.md
--rw-r--r--   0        0        0      744 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/spotify_utils/__init__.py
--rw-r--r--   0        0        0      501 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/spotify_utils/config.py
--rw-r--r--   0        0        0      473 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/spotify_utils/main.py
--rw-r--r--   0        0        0        0 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/spotify_utils/settings.toml
--rw-r--r--   0        0        0        0 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/spotify_utils/src/__init__.py
--rw-r--r--   0        0        0      794 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/spotify_utils/src/auth.py
--rw-r--r--   0        0        0      733 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/spotify_utils/src/file_operations.py
--rw-r--r--   0        0        0     7346 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/spotify_utils/src/playlists.py
--rw-r--r--   0        0        0      114 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/spotify_utils/src/user.py
--rw-r--r--   0        0        0     5395 2024-06-02 15:41:58.000000 spotify_utils-1.0.7/spotify_utils/templates/playlists.html
--rw-r--r--   0        0        0     8573 1970-01-01 00:00:00.000000 spotify_utils-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    34888 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/LICENSE
+-rw-r--r--   0        0        0     7570 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/README.md
+-rw-r--r--   0        0        0      744 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/spotify_utils/__init__.py
+-rw-r--r--   0        0        0      501 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/spotify_utils/config.py
+-rw-r--r--   0        0        0      473 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/spotify_utils/main.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/spotify_utils/settings.toml
+-rw-r--r--   0        0        0        0 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/spotify_utils/src/__init__.py
+-rw-r--r--   0        0        0      794 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/spotify_utils/src/auth.py
+-rw-r--r--   0        0        0      733 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/spotify_utils/src/file_operations.py
+-rw-r--r--   0        0        0     7346 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/spotify_utils/src/playlists.py
+-rw-r--r--   0        0        0      114 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/spotify_utils/src/user.py
+-rw-r--r--   0        0        0     5395 2024-06-02 16:12:56.000000 spotify_utils-1.0.8/spotify_utils/templates/playlists.html
+-rw-r--r--   0        0        0     8573 1970-01-01 00:00:00.000000 spotify_utils-1.0.8/PKG-INFO
```

### Comparing `spotify_utils-1.0.7/LICENSE` & `spotify_utils-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_utils-1.0.7/README.md` & `spotify_utils-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `spotify_utils-1.0.7/pyproject.toml` & `spotify_utils-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotify-utils"
-version = "1.0.7"
+version = "1.0.8"
 description = "An awesome and easy-to-use CLI for various Spotify® utility tasks"
 license = "GPL-3.0-only"
 authors = ["Fabian Eulitz <dev@sustineo.de>"]
 repository = "https://gitlab.com/sustineo/spotify-utils"
 keywords = ["spotify", "CLI", "utilities"]
 readme = "README.md"
```

### Comparing `spotify_utils-1.0.7/spotify_utils/src/auth.py` & `spotify_utils-1.0.8/spotify_utils/src/auth.py`

 * *Files identical despite different names*

### Comparing `spotify_utils-1.0.7/spotify_utils/src/file_operations.py` & `spotify_utils-1.0.8/spotify_utils/src/file_operations.py`

 * *Files identical despite different names*

### Comparing `spotify_utils-1.0.7/spotify_utils/src/playlists.py` & `spotify_utils-1.0.8/spotify_utils/src/playlists.py`

 * *Files identical despite different names*

### Comparing `spotify_utils-1.0.7/spotify_utils/templates/playlists.html` & `spotify_utils-1.0.8/spotify_utils/templates/playlists.html`

 * *Files identical despite different names*

### Comparing `spotify_utils-1.0.7/PKG-INFO` & `spotify_utils-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-utils
-Version: 1.0.7
+Version: 1.0.8
 Summary: An awesome and easy-to-use CLI for various Spotify® utility tasks
 Home-page: https://gitlab.com/sustineo/spotify-utils
 License: GPL-3.0-only
 Keywords: spotify,CLI,utilities
 Author: Fabian Eulitz
 Author-email: dev@sustineo.de
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spotify-utils Version: 1.0.7 Summary: An awesome
+Metadata-Version: 2.1 Name: spotify-utils Version: 1.0.8 Summary: An awesome
 and easy-to-use CLI for various SpotifyÂ® utility tasks Home-page: https://
 gitlab.com/sustineo/spotify-utils License: GPL-3.0-only Keywords:
 spotify,CLI,utilities Author: Fabian Eulitz Author-email: dev@sustineo.de
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

