# Comparing `tmp/knuckles-0.1.0.tar.gz` & `tmp/knuckles-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knuckles-0.1.0.tar", last modified: Sun Jun  2 00:50:06 2024, max compression
+gzip compressed data, was "knuckles-0.2.0.tar", last modified: Sun Jun  2 21:51:41 2024, max compression
```

## Comparing `knuckles-0.1.0.tar` & `knuckles-0.2.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:50:06.922774 knuckles-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-02 00:49:54.000000 knuckles-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-06-02 00:50:06.922774 knuckles-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-06-02 00:49:54.000000 knuckles-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-06-02 00:49:54.000000 knuckles-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:50:06.922774 knuckles-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:50:06.906774 knuckles-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:50:06.914774 knuckles-0.1.0/src/knuckles/
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_internet_radio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_jukebox.py
--rw-r--r--   0 runner    (1001) docker     (127)    25877 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_media_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_media_library_scanning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_media_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_podcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_searching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_sharing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_subsonic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_system.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/_user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:50:06.918774 knuckles-0.1.0/src/knuckles/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_album.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_artist_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_contributor.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_cover_art.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_genre.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_internet_radio_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_jukebox.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_lyrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_music_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_music_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_now_playing_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_play_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_podcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_replay_gain.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_scan_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_search_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_share.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_starred_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/models/_video.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:49:54.000000 knuckles-0.1.0/src/knuckles/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:50:06.918774 knuckles-0.1.0/src/knuckles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-06-02 00:50:06.000000 knuckles-0.1.0/src/knuckles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-06-02 00:50:06.000000 knuckles-0.1.0/src/knuckles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:50:06.000000 knuckles-0.1.0/src/knuckles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-06-02 00:50:06.000000 knuckles-0.1.0/src/knuckles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 00:50:06.000000 knuckles-0.1.0/src/knuckles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:41.670433 knuckles-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-02 21:51:29.000000 knuckles-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-06-02 21:51:41.666433 knuckles-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-06-02 21:51:29.000000 knuckles-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-06-02 21:51:29.000000 knuckles-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 21:51:41.670433 knuckles-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:41.658433 knuckles-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:41.662433 knuckles-0.2.0/src/knuckles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_internet_radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_jukebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25877 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_media_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_media_library_scanning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_media_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_podcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_searching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_subsonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:41.666433 knuckles-0.2.0/src/knuckles/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_album.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_artist_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_contributor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_cover_art.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_genre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_internet_radio_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_jukebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_music_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_music_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_now_playing_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_play_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_podcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_replay_gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_scan_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_share.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_starred_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:41.666433 knuckles-0.2.0/src/knuckles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-06-02 21:51:41.000000 knuckles-0.2.0/src/knuckles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-06-02 21:51:41.000000 knuckles-0.2.0/src/knuckles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 21:51:41.000000 knuckles-0.2.0/src/knuckles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-06-02 21:51:41.000000 knuckles-0.2.0/src/knuckles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 21:51:41.000000 knuckles-0.2.0/src/knuckles.egg-info/top_level.txt
```

### Comparing `knuckles-0.1.0/LICENSE.txt` & `knuckles-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/README.md` & `knuckles-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,17 @@
+<div align="center" markdown="1">
 # Knuckles
-> A [OpenSubsonic](https://opensubsonic.netlify.app/) API wrapper for Python 3.11.0+.
+
+![PyPI - Version](https://img.shields.io/pypi/v/knuckles)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/knuckles)
+![GitHub Actions - PyPI Publishing](https://github.com/kutu-dev/knuckles/actions/workflows/publish.yml/badge.svg)
+![GitHub Actions - Docs Deploying](https://github.com/kutu-dev/knuckles/actions/workflows/docs.yml/badge.svg)
+
+An unopinionated [OpenSubsonic](https://opensubsonic.netlify.app/) API wrapper for Python.
+</div>
 
 ## Compatiblity
 Knuckles **only** works with servers compatible with the REST API version 1.4.0 onwards (Subsonic 4.2+).
 It follows strictly the [OpenSubsonic API Spec](https://opensubsonic.netlify.app/docs/opensubsonic-api/), being fully retro-compatible with the original [Subsonic API](https://subsonic.org/pages/api.jsp).
 
 ## Getting Started
 
@@ -39,11 +47,11 @@
 ping = server.ping()
 
 # Print the supported version of the OpenSubsonic REST API
 print(ping.version)
 ```
 
 ### Learning More
-To start making more complex interactions with the API make use of [the reference](https://kutu-dev.github.io/knuckles/reference/Api/). Enjoy coding and good luck!
+To start making more complex interactions with the API make use of [the API reference](https://kutu-dev.github.io/knuckles/reference/Api/). Enjoy coding and good luck!
 
 ## Acknowledgements
 Created with :heart: by [Jorge "Kutu" Dobón Blanco](https://dobon.dev).
```

### Comparing `knuckles-0.1.0/src/knuckles/__init__.py` & `knuckles-0.2.0/src/knuckles/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from importlib.metadata import version
+
 from ._api import RequestMethod
 from ._media_retrieval import SubtitlesFileFormat
 from ._subsonic import Subsonic
 from .models._album import Album, AlbumInfo, Disc, RecordLabel, ReleaseDate
 from .models._artist import Artist, ArtistInfo
 from .models._artist_index import ArtistIndex
 from .models._bookmark import Bookmark
@@ -24,15 +26,18 @@
 from .models._share import Share
 from .models._song import Song
 from .models._starred_content import StarredContent
 from .models._system import License, SubsonicResponse
 from .models._user import User
 from .models._video import AudioTrack, Captions, Video, VideoInfo
 
+__version__ = version("knuckles")
+
 __all__ = [
+    "__version__",
     "Subsonic",
     "RequestMethod",
     "SubtitlesFileFormat",
     "RecordLabel",
     "Disc",
     "ReleaseDate",
     "AlbumInfo",
```

### Comparing `knuckles-0.1.0/src/knuckles/_api.py` & `knuckles-0.2.0/src/knuckles/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import hashlib
-import json
 import secrets
 from enum import Enum
 from typing import Any
 from urllib.parse import ParseResult, urlparse
 
 import requests
 from requests import Response
@@ -142,15 +141,15 @@
                 `response` object of the executed request.
         """
 
         match self.request_method:
             case RequestMethod.POST:
                 return requests.post(
                     url=f"{self.url}/rest/{endpoint}",
-                    data=json.dumps(self._generate_params(extra_params)),
+                    data=self._generate_params(extra_params),
                 )
 
             case RequestMethod.GET | _:
                 return requests.get(
                     url=f"{self.url}/rest/{endpoint}",
                     params=self._generate_params(extra_params),
                 )
```

### Comparing `knuckles-0.1.0/src/knuckles/_bookmarks.py` & `knuckles-0.2.0/src/knuckles/_bookmarks.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_browsing.py` & `knuckles-0.2.0/src/knuckles/_browsing.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_chat.py` & `knuckles-0.2.0/src/knuckles/_chat.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_internet_radio.py` & `knuckles-0.2.0/src/knuckles/_internet_radio.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_jukebox.py` & `knuckles-0.2.0/src/knuckles/_jukebox.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_lists.py` & `knuckles-0.2.0/src/knuckles/_lists.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_media_annotation.py` & `knuckles-0.2.0/src/knuckles/_media_annotation.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_media_library_scanning.py` & `knuckles-0.2.0/src/knuckles/_media_library_scanning.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_media_retrieval.py` & `knuckles-0.2.0/src/knuckles/_media_retrieval.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_playlists.py` & `knuckles-0.2.0/src/knuckles/_playlists.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_podcast.py` & `knuckles-0.2.0/src/knuckles/_podcast.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_searching.py` & `knuckles-0.2.0/src/knuckles/_searching.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_sharing.py` & `knuckles-0.2.0/src/knuckles/_sharing.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_subsonic.py` & `knuckles-0.2.0/src/knuckles/_subsonic.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self,
         url: str,
         user: str,
         password: str,
         client: str,
         use_https: bool = True,
         use_token: bool = True,
-        request_method: RequestMethod = RequestMethod.POST,
+        request_method: RequestMethod = RequestMethod.GET,
     ) -> None:
         """Construction method of the Subsonic object used to
         interact with the OpenSubsonic REST API.
 
         Args:
             url: The URL of the Subsonic server to connect to.
             user: The name of the user to authenticate.
```

### Comparing `knuckles-0.1.0/src/knuckles/_system.py` & `knuckles-0.2.0/src/knuckles/_system.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/_user_management.py` & `knuckles-0.2.0/src/knuckles/_user_management.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/exceptions.py` & `knuckles-0.2.0/src/knuckles/exceptions.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_album.py` & `knuckles-0.2.0/src/knuckles/models/_album.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_artist.py` & `knuckles-0.2.0/src/knuckles/models/_artist.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_artist_index.py` & `knuckles-0.2.0/src/knuckles/models/_artist_index.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_bookmark.py` & `knuckles-0.2.0/src/knuckles/models/_bookmark.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_chat_message.py` & `knuckles-0.2.0/src/knuckles/models/_chat_message.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_contributor.py` & `knuckles-0.2.0/src/knuckles/models/_contributor.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_genre.py` & `knuckles-0.2.0/src/knuckles/models/_genre.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_internet_radio_station.py` & `knuckles-0.2.0/src/knuckles/models/_internet_radio_station.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_jukebox.py` & `knuckles-0.2.0/src/knuckles/models/_jukebox.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_lyrics.py` & `knuckles-0.2.0/src/knuckles/models/_lyrics.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_music_directory.py` & `knuckles-0.2.0/src/knuckles/models/_music_directory.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_music_folder.py` & `knuckles-0.2.0/src/knuckles/models/_music_folder.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_now_playing_entry.py` & `knuckles-0.2.0/src/knuckles/models/_now_playing_entry.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_play_queue.py` & `knuckles-0.2.0/src/knuckles/models/_play_queue.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_playlist.py` & `knuckles-0.2.0/src/knuckles/models/_playlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             it use the `add_songs` and `remove_songs` methods.
 
         Returns:
             The object itself.
         """
 
         self._subsonic.playlists.update_playlist(
-            self.id, self.name, self.comment, self.public
+            self.id, comment=self.comment, public=self.public
         )
 
         return self
 
     def delete(self) -> Self:
         """Delete the playlist from the server.
```

### Comparing `knuckles-0.1.0/src/knuckles/models/_podcast.py` & `knuckles-0.2.0/src/knuckles/models/_podcast.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_replay_gain.py` & `knuckles-0.2.0/src/knuckles/models/_replay_gain.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_scan_status.py` & `knuckles-0.2.0/src/knuckles/models/_scan_status.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_search_result.py` & `knuckles-0.2.0/src/knuckles/models/_search_result.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_share.py` & `knuckles-0.2.0/src/knuckles/models/_share.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_song.py` & `knuckles-0.2.0/src/knuckles/models/_song.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_starred_content.py` & `knuckles-0.2.0/src/knuckles/models/_starred_content.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_system.py` & `knuckles-0.2.0/src/knuckles/models/_system.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_user.py` & `knuckles-0.2.0/src/knuckles/models/_user.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles/models/_video.py` & `knuckles-0.2.0/src/knuckles/models/_video.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.1.0/src/knuckles.egg-info/SOURCES.txt` & `knuckles-0.2.0/src/knuckles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

