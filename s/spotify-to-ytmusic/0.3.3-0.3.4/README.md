# Comparing `tmp/spotify_to_ytmusic-0.3.3.tar.gz` & `tmp/spotify_to_ytmusic-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_to_ytmusic-0.3.3.tar", last modified: Mon Jan  1 18:51:17 2024, max compression
+gzip compressed data, was "spotify_to_ytmusic-0.3.4.tar", last modified: Sun Jun  2 13:32:51 2024, max compression
```

## Comparing `spotify_to_ytmusic-0.3.3.tar` & `spotify_to_ytmusic-0.3.4.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 18:51:17.671515 spotify_to_ytmusic-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 18:51:17.667515 spotify_to_ytmusic-0.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 18:51:17.667515 spotify_to_ytmusic-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-01-01 18:51:17.671515 spotify_to_ytmusic-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-01 18:51:17.671515 spotify_to_ytmusic-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 18:51:17.667515 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/settings.ini.example
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/spotify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 18:51:17.671515 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/utils/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/utils/match.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 18:51:17.671515 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-01-01 18:51:17.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-01-01 18:51:17.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 18:51:17.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-01 18:51:17.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-01 18:51:17.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-01 18:51:17.000000 spotify_to_ytmusic-0.3.3/spotify_to_ytmusic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 18:51:17.671515 spotify_to_ytmusic-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/tests/test_spotipy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 18:51:06.000000 spotify_to_ytmusic-0.3.3/tests/test_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:32:51.799725 spotify_to_ytmusic-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:32:51.795725 spotify_to_ytmusic-0.3.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:32:51.795725 spotify_to_ytmusic-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-06-02 13:32:51.799725 spotify_to_ytmusic-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    33519 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 13:32:51.799725 spotify_to_ytmusic-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:32:51.795725 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/settings.ini.example
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/spotify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:32:51.795725 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/utils/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/utils/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:32:51.799725 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-06-02 13:32:51.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-06-02 13:32:51.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 13:32:51.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-02 13:32:51.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 13:32:51.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-02 13:32:51.000000 spotify_to_ytmusic-0.3.4/spotify_to_ytmusic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:32:51.799725 spotify_to_ytmusic-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/tests/test_spotipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 13:32:47.000000 spotify_to_ytmusic-0.3.4/tests/test_youtube.py
```

### Comparing `spotify_to_ytmusic-0.3.3/.github/workflows/coverage.yml` & `spotify_to_ytmusic-0.3.4/.github/workflows/coverage.yml`

 * *Files 10% similar despite different names*

```diff
@@ -24,12 +24,13 @@
         pip install coverage
         cat <<< "$SETTINGS_INI" > spotify_to_ytmusic/settings.ini
         mkdir -p $XDG_CACHE_HOME/spotify_to_ytmusic
         cat <<< "$SPOTIPY_CACHE" > $XDG_CACHE_HOME/spotify_to_ytmusic/spotipy.cache
         coverage run
         coverage xml
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         file: coverage.xml
         flags: unittests
         fail_ci_if_error: true
+        token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `spotify_to_ytmusic-0.3.3/.github/workflows/pythonpublish.yml` & `spotify_to_ytmusic-0.3.4/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.3.3/.gitignore` & `spotify_to_ytmusic-0.3.4/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -106,8 +106,11 @@
 .mypy_cache/
 
 # specific
 .idea
 noresults.txt
 *.ini
 *.txt
-*.json
+*.json
+
+#PDM
+.pdm-python
```

### Comparing `spotify_to_ytmusic-0.3.3/LICENSE` & `spotify_to_ytmusic-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.3.3/PKG-INFO` & `spotify_to_ytmusic-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: spotify_to_ytmusic
-Version: 0.3.3
+Version: 0.3.4
 Summary: Transfer Spotify playlists to YouTube Music
-Author-email: sigma67 <ytmusicapi@gmail.com>
+Author-email: sigma67 <sigma67.github@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,49 +28,49 @@
 Project-URL: homepage, https://github.com/sigma67/spotify_to_ytmusic
 Project-URL: repository, https://github.com/sigma67/spotify_to_ytmusic
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: ytmusicapi>=1.4
+Requires-Dist: ytmusicapi>=1.7.3
 Requires-Dist: spotipy>=2.23.0
 Requires-Dist: platformdirs>=3.2
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
 
 spotify_to_ytmusic
 ####################
 
-.. image:: https://img.shields.io/pypi/dm/spotify_to_ytmusic?style=flat-square
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/spotify_to_ytmusic?style=flat-square
     :alt: PyPI Downloads
     :target: https://pypi.org/project/spotify_to_ytmusic/
 
-.. image:: https://img.shields.io/github/discussions/sigma67/spotify_to_ytmusic?style=flat-square
+.. |discuss| image:: https://img.shields.io/github/discussions/sigma67/spotify_to_ytmusic?style=flat-square
    :alt: Ask questions at Discussions
    :target: https://github.com/sigma67/spotify_to_ytmusic/discussions
 
-.. image:: https://img.shields.io/codecov/c/github/sigma67/spotify_to_ytmusic?style=flat-square
+.. |code-coverage| image:: https://img.shields.io/codecov/c/github/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Code coverage
     :target: https://codecov.io/gh/sigma67/spotify_to_ytmusic
 
-.. image:: https://img.shields.io/github/v/release/sigma67/spotify_to_ytmusic?style=flat-square
+.. |latest-release| image:: https://img.shields.io/github/v/release/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Latest release
     :target: https://github.com/sigma67/spotify_to_ytmusic/releases/latest
 
-.. image:: https://img.shields.io/github/commits-since/sigma67/spotify_to_ytmusic/latest?style=flat-square
+.. |commits-since-latest| image:: https://img.shields.io/github/commits-since/sigma67/spotify_to_ytmusic/latest?style=flat-square
     :alt: Commits since latest release
     :target: https://github.com/sigma67/spotify_to_ytmusic/commits
 
+
+|pypi-downloads| |discuss| |code-coverage| |latest-release| |commits-since-latest|
+
 A simple command line script to clone a Spotify playlist to YouTube Music.
 
 - Transfer a single Spotify playlist
 - Update a transferred playlist on YouTube Music
 - Transfer all playlists for a Spotify user
 - Remove playlists from YouTube Music
 
@@ -108,15 +108,15 @@
 
 .. code-block::
 
     spotify_to_ytmusic create <spotifylink>
 
 where ``<spotifylink>`` is a link like https://open.spotify.com/playlist/0S0cuX8pnvmF7gA47Eu63M
 
-The script will log its progress and output songs that were not found in YouTube Music to **noresults.txt**.
+The script will log its progress and output songs that were not found in YouTube Music to **noresults_youtube.txt**.
 
 Transfer all playlists of a Spotify user
 ----------------------------------------
 
 For migration purposes, it is possible to transfer all public playlists of a user by using the Spotify user's ID (unique username).
 
 .. code-block::
```

### Comparing `spotify_to_ytmusic-0.3.3/README.rst` & `spotify_to_ytmusic-0.3.4/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 spotify_to_ytmusic
 ####################
 
-.. image:: https://img.shields.io/pypi/dm/spotify_to_ytmusic?style=flat-square
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/spotify_to_ytmusic?style=flat-square
     :alt: PyPI Downloads
     :target: https://pypi.org/project/spotify_to_ytmusic/
 
-.. image:: https://img.shields.io/github/discussions/sigma67/spotify_to_ytmusic?style=flat-square
+.. |discuss| image:: https://img.shields.io/github/discussions/sigma67/spotify_to_ytmusic?style=flat-square
    :alt: Ask questions at Discussions
    :target: https://github.com/sigma67/spotify_to_ytmusic/discussions
 
-.. image:: https://img.shields.io/codecov/c/github/sigma67/spotify_to_ytmusic?style=flat-square
+.. |code-coverage| image:: https://img.shields.io/codecov/c/github/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Code coverage
     :target: https://codecov.io/gh/sigma67/spotify_to_ytmusic
 
-.. image:: https://img.shields.io/github/v/release/sigma67/spotify_to_ytmusic?style=flat-square
+.. |latest-release| image:: https://img.shields.io/github/v/release/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Latest release
     :target: https://github.com/sigma67/spotify_to_ytmusic/releases/latest
 
-.. image:: https://img.shields.io/github/commits-since/sigma67/spotify_to_ytmusic/latest?style=flat-square
+.. |commits-since-latest| image:: https://img.shields.io/github/commits-since/sigma67/spotify_to_ytmusic/latest?style=flat-square
     :alt: Commits since latest release
     :target: https://github.com/sigma67/spotify_to_ytmusic/commits
 
+
+|pypi-downloads| |discuss| |code-coverage| |latest-release| |commits-since-latest|
+
 A simple command line script to clone a Spotify playlist to YouTube Music.
 
 - Transfer a single Spotify playlist
 - Update a transferred playlist on YouTube Music
 - Transfer all playlists for a Spotify user
 - Remove playlists from YouTube Music
 
@@ -62,15 +65,15 @@
 
 .. code-block::
 
     spotify_to_ytmusic create <spotifylink>
 
 where ``<spotifylink>`` is a link like https://open.spotify.com/playlist/0S0cuX8pnvmF7gA47Eu63M
 
-The script will log its progress and output songs that were not found in YouTube Music to **noresults.txt**.
+The script will log its progress and output songs that were not found in YouTube Music to **noresults_youtube.txt**.
 
 Transfer all playlists of a Spotify user
 ----------------------------------------
 
 For migration purposes, it is possible to transfer all public playlists of a user by using the Spotify user's ID (unique username).
 
 .. code-block::
```

### Comparing `spotify_to_ytmusic-0.3.3/pyproject.toml` & `spotify_to_ytmusic-0.3.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 [project]
 name = "spotify_to_ytmusic"
 description = "Transfer Spotify playlists to YouTube Music"
 requires-python = ">=3.8"
-authors=[{name = "sigma67", email= "ytmusicapi@gmail.com"}]
+authors=[{name = "sigma67", email= "sigma67.github@gmail.com"}]
 license={file="LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
-    "ytmusicapi>=1.4",
+    "ytmusicapi>=1.7.3",
     "spotipy>=2.23.0",
-    "platformdirs>=3.2"
+    "platformdirs>=3.2",
 ]
 dynamic = ["version", "readme"]
 
-[project.optional-dependencies]
-dev = ['black', 'isort', 'coverage']
-
 [project.scripts]
 spotify_to_ytmusic = "spotify_to_ytmusic.main:main"
 
 [project.urls]
 homepage = "https://github.com/sigma67/spotify_to_ytmusic"
 repository = "https://github.com/sigma67/spotify_to_ytmusic"
 
@@ -50,7 +48,17 @@
 
 [tool.black]
 src_paths = ["spotify_to_ytmusic"]
 line-length = 99
 
 [tool.coverage.run]
 command_line = "-m unittest discover tests"
+
+[tool.pdm]
+distribution = true
+
+[tool.pdm.dev-dependencies]
+dev = [
+    "black>=24.4.2",
+    "isort>=5.13.2",
+    "coverage>=7.5.3",
+]
```

### Comparing `spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/controllers.py` & `spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/controllers.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/main.py` & `spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/main.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/settings.py` & `spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/settings.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/setup.py` & `spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/setup.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/spotify.py` & `spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/spotify.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/utils/match.py` & `spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/utils/match.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.3.3/spotify_to_ytmusic/ytmusic.py` & `spotify_to_ytmusic-0.3.4/spotify_to_ytmusic/ytmusic.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.3.3/spotify_to_ytmusic.egg-info/PKG-INFO` & `spotify_to_ytmusic-0.3.4/spotify_to_ytmusic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: spotify_to_ytmusic
-Version: 0.3.3
+Version: 0.3.4
 Summary: Transfer Spotify playlists to YouTube Music
-Author-email: sigma67 <ytmusicapi@gmail.com>
+Author-email: sigma67 <sigma67.github@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,49 +28,49 @@
 Project-URL: homepage, https://github.com/sigma67/spotify_to_ytmusic
 Project-URL: repository, https://github.com/sigma67/spotify_to_ytmusic
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: ytmusicapi>=1.4
+Requires-Dist: ytmusicapi>=1.7.3
 Requires-Dist: spotipy>=2.23.0
 Requires-Dist: platformdirs>=3.2
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
 
 spotify_to_ytmusic
 ####################
 
-.. image:: https://img.shields.io/pypi/dm/spotify_to_ytmusic?style=flat-square
+.. |pypi-downloads| image:: https://img.shields.io/pypi/dm/spotify_to_ytmusic?style=flat-square
     :alt: PyPI Downloads
     :target: https://pypi.org/project/spotify_to_ytmusic/
 
-.. image:: https://img.shields.io/github/discussions/sigma67/spotify_to_ytmusic?style=flat-square
+.. |discuss| image:: https://img.shields.io/github/discussions/sigma67/spotify_to_ytmusic?style=flat-square
    :alt: Ask questions at Discussions
    :target: https://github.com/sigma67/spotify_to_ytmusic/discussions
 
-.. image:: https://img.shields.io/codecov/c/github/sigma67/spotify_to_ytmusic?style=flat-square
+.. |code-coverage| image:: https://img.shields.io/codecov/c/github/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Code coverage
     :target: https://codecov.io/gh/sigma67/spotify_to_ytmusic
 
-.. image:: https://img.shields.io/github/v/release/sigma67/spotify_to_ytmusic?style=flat-square
+.. |latest-release| image:: https://img.shields.io/github/v/release/sigma67/spotify_to_ytmusic?style=flat-square
     :alt: Latest release
     :target: https://github.com/sigma67/spotify_to_ytmusic/releases/latest
 
-.. image:: https://img.shields.io/github/commits-since/sigma67/spotify_to_ytmusic/latest?style=flat-square
+.. |commits-since-latest| image:: https://img.shields.io/github/commits-since/sigma67/spotify_to_ytmusic/latest?style=flat-square
     :alt: Commits since latest release
     :target: https://github.com/sigma67/spotify_to_ytmusic/commits
 
+
+|pypi-downloads| |discuss| |code-coverage| |latest-release| |commits-since-latest|
+
 A simple command line script to clone a Spotify playlist to YouTube Music.
 
 - Transfer a single Spotify playlist
 - Update a transferred playlist on YouTube Music
 - Transfer all playlists for a Spotify user
 - Remove playlists from YouTube Music
 
@@ -108,15 +108,15 @@
 
 .. code-block::
 
     spotify_to_ytmusic create <spotifylink>
 
 where ``<spotifylink>`` is a link like https://open.spotify.com/playlist/0S0cuX8pnvmF7gA47Eu63M
 
-The script will log its progress and output songs that were not found in YouTube Music to **noresults.txt**.
+The script will log its progress and output songs that were not found in YouTube Music to **noresults_youtube.txt**.
 
 Transfer all playlists of a Spotify user
 ----------------------------------------
 
 For migration purposes, it is possible to transfer all public playlists of a user by using the Spotify user's ID (unique username).
 
 .. code-block::
```

### Comparing `spotify_to_ytmusic-0.3.3/spotify_to_ytmusic.egg-info/SOURCES.txt` & `spotify_to_ytmusic-0.3.4/spotify_to_ytmusic.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 LICENSE
 README.rst
+pdm.lock
 pyproject.toml
 .github/dependabot.yml
 .github/workflows/coverage.yml
 .github/workflows/pythonpublish.yml
 spotify_to_ytmusic/__init__.py
 spotify_to_ytmusic/controllers.py
 spotify_to_ytmusic/main.py
@@ -18,11 +19,12 @@
 spotify_to_ytmusic.egg-info/dependency_links.txt
 spotify_to_ytmusic.egg-info/entry_points.txt
 spotify_to_ytmusic.egg-info/requires.txt
 spotify_to_ytmusic.egg-info/top_level.txt
 spotify_to_ytmusic/utils/__init__.py
 spotify_to_ytmusic/utils/browser.py
 spotify_to_ytmusic/utils/match.py
+tests/__init__.py
 tests/test_cli.py
 tests/test_parsing.py
 tests/test_spotipy.py
 tests/test_youtube.py
```

### Comparing `spotify_to_ytmusic-0.3.3/tests/test_cli.py` & `spotify_to_ytmusic-0.3.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.3.3/tests/test_parsing.py` & `spotify_to_ytmusic-0.3.4/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.3.3/tests/test_spotipy.py` & `spotify_to_ytmusic-0.3.4/tests/test_spotipy.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,8 +12,8 @@
             "https://open.spotify.com/playlist/03ICMYsVsC4I2SZnERcQJb"
         )
         self.assertEqual(len(data), 3)
         self.assertGreater(len(data["tracks"]), 190)
 
     def test_getUserPlaylists(self):
         playlists = self.spotify.getUserPlaylists("spinninrecordsofficial")
-        self.assertGreater(len(playlists), 50)
+        self.assertGreater(len(playlists), 40)
```

