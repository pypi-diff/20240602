# Comparing `tmp/mmdiary-0.3.0.tar.gz` & `tmp/mmdiary-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmdiary-0.3.0.tar", last modified: Thu May 23 00:03:56 2024, max compression
+gzip compressed data, was "mmdiary-0.4.0.tar", last modified: Sat Jun  1 23:22:12 2024, max compression
```

## Comparing `mmdiary-0.3.0.tar` & `mmdiary-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,45 @@
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.890636 mmdiary-0.3.0/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    35149 2024-05-14 21:19:42.000000 mmdiary-0.3.0/LICENSE
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    53035 2024-05-23 00:03:56.890636 mmdiary-0.3.0/PKG-INFO
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    11174 2024-05-22 23:57:28.000000 mmdiary-0.3.0/README.md
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     2227 2024-05-22 23:59:01.000000 mmdiary-0.3.0/pyproject.toml
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-05-23 00:03:56.890636 mmdiary-0.3.0/setup.cfg
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.826635 mmdiary-0.3.0/src/
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.826635 mmdiary-0.3.0/src/mmdiary/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/__init__.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.850636 mmdiary-0.3.0/src/mmdiary/notion/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/notion/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     3375 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/notion/cache.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     2174 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/notion/cleanup.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    15750 2024-05-15 23:08:07.000000 mmdiary-0.3.0/src/mmdiary/notion/uploader.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.850636 mmdiary-0.3.0/src/mmdiary/telegrambot/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/telegrambot/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     7859 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/telegrambot/telegrambot_service.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.854636 mmdiary-0.3.0/src/mmdiary/transcriber/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/transcriber/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     1011 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/transcriber/searcher.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4112 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/transcriber/transcriber.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    11389 2024-05-18 00:04:37.000000 mmdiary-0.3.0/src/mmdiary/transcriber/verifier.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.870636 mmdiary-0.3.0/src/mmdiary/utils/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/utils/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     8643 2024-05-22 23:57:34.000000 mmdiary-0.3.0/src/mmdiary/utils/datelib.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1947 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/utils/jsoncache.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1004 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/utils/log.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     5364 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/utils/medialib.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      368 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/utils/progressbar.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.890636 mmdiary-0.3.0/src/mmdiary/video/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/video/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     6134 2024-05-21 21:53:19.000000 mmdiary-0.3.0/src/mmdiary/video/processor.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    12810 2024-05-22 17:08:37.000000 mmdiary-0.3.0/src/mmdiary/video/uploader.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.826635 mmdiary-0.3.0/src/mmdiary.egg-info/
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    53035 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/PKG-INFO
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      887 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/SOURCES.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/dependency_links.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      583 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/entry_points.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      152 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/requires.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        8 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/top_level.txt
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-06-01 23:22:12.319151 mmdiary-0.4.0/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    35149 2024-05-14 21:19:42.000000 mmdiary-0.4.0/LICENSE
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    55305 2024-06-01 23:22:12.319151 mmdiary-0.4.0/PKG-INFO
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    13444 2024-06-01 22:45:41.000000 mmdiary-0.4.0/README.md
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     2350 2024-06-01 22:50:59.000000 mmdiary-0.4.0/pyproject.toml
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-06-01 23:22:12.319151 mmdiary-0.4.0/setup.cfg
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-06-01 23:22:11.343151 mmdiary-0.4.0/src/
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-06-01 23:22:11.347151 mmdiary-0.4.0/src/mmdiary/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/__init__.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-06-01 23:22:11.547151 mmdiary-0.4.0/src/mmdiary/notion/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/notion/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     3375 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/notion/cache.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     2174 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/notion/cleanup.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    16053 2024-05-30 10:43:11.000000 mmdiary-0.4.0/src/mmdiary/notion/uploader.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-06-01 23:22:11.611151 mmdiary-0.4.0/src/mmdiary/telegrambot/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/telegrambot/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     7859 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/telegrambot/telegrambot_service.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-06-01 23:22:11.727151 mmdiary-0.4.0/src/mmdiary/transcriber/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/transcriber/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     1011 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/transcriber/searcher.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4112 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/transcriber/transcriber.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    11389 2024-05-18 00:04:37.000000 mmdiary-0.4.0/src/mmdiary/transcriber/verifier.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-06-01 23:22:11.971151 mmdiary-0.4.0/src/mmdiary/utils/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/utils/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     8985 2024-05-29 22:34:18.000000 mmdiary-0.4.0/src/mmdiary/utils/datelib.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     2027 2024-06-01 22:45:42.000000 mmdiary-0.4.0/src/mmdiary/utils/jsoncache.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1004 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/utils/log.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     5408 2024-05-24 07:52:45.000000 mmdiary-0.4.0/src/mmdiary/utils/medialib.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      368 2024-05-14 21:19:42.000000 mmdiary-0.4.0/src/mmdiary/utils/progressbar.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1391 2024-05-28 15:12:51.000000 mmdiary-0.4.0/src/mmdiary/utils/proxypatch.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-06-01 23:22:12.027151 mmdiary-0.4.0/src/mmdiary/video/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-29 22:04:44.000000 mmdiary-0.4.0/src/mmdiary/video/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     6134 2024-05-21 21:53:19.000000 mmdiary-0.4.0/src/mmdiary/video/processor.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-06-01 23:22:12.247151 mmdiary-0.4.0/src/mmdiary/video/uploader/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      394 2024-05-29 22:45:13.000000 mmdiary-0.4.0/src/mmdiary/video/uploader/__init__.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      127 2024-05-29 22:42:26.000000 mmdiary-0.4.0/src/mmdiary/video/uploader/common.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     9747 2024-06-01 22:45:42.000000 mmdiary-0.4.0/src/mmdiary/video/uploader/dailymotion.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    15127 2024-06-01 23:00:11.000000 mmdiary-0.4.0/src/mmdiary/video/uploader/youtube.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-06-01 23:22:11.347151 mmdiary-0.4.0/src/mmdiary.egg-info/
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    55305 2024-06-01 23:22:08.000000 mmdiary-0.4.0/src/mmdiary.egg-info/PKG-INFO
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1045 2024-06-01 23:22:09.000000 mmdiary-0.4.0/src/mmdiary.egg-info/SOURCES.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-06-01 23:22:08.000000 mmdiary-0.4.0/src/mmdiary.egg-info/dependency_links.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      674 2024-06-01 23:22:08.000000 mmdiary-0.4.0/src/mmdiary.egg-info/entry_points.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      175 2024-06-01 23:22:08.000000 mmdiary-0.4.0/src/mmdiary.egg-info/requires.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        8 2024-06-01 23:22:08.000000 mmdiary-0.4.0/src/mmdiary.egg-info/top_level.txt
```

### Comparing `mmdiary-0.3.0/LICENSE` & `mmdiary-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdiary-0.3.0/PKG-INFO` & `mmdiary-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmdiary
-Version: 0.3.0
+Version: 0.4.0
 Summary: Multimedia Diary Tools
 Author-email: Alexander Bushnev <Alexander@Bushnev.pro>
 Maintainer-email: Alexander Bushnev <Alexander@Bushnev.pro>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -705,15 +705,15 @@
 # Multimedia Diary Tools 
 
 ![CodeQL](https://github.com/sashacmc/mmdiary/workflows/CodeQL/badge.svg)
 [![PyPI - Version](https://img.shields.io/pypi/v/mmdiary.svg)](https://pypi.org/project/mmdiary)
 [![PyPI - Downloads](https://pepy.tech/badge/mmdiary)](https://pepy.tech/project/mmdiary)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.commdiarym/psf/black)
 
-Multimedia Diary Tools is a Python toolkit designed to automate the process of managing multimedia content for diary entries. This toolkit offers functionalities to scan specified folders, identify audio and video files, perform speech-to-text transcription, merge video files, and upload the resulting video content to YouTube. Additionally, it integrates with Notion to create a calendar and populate it with transcribed text from audio and video notes, accompanied by links to the original media. A Telegram bot is also provided for easy access to audio notes.
+Multimedia Diary Tools is a Python toolkit designed to automate the process of managing multimedia content for diary entries. This toolkit offers functionalities to scan specified folders, identify audio and video files, perform speech-to-text transcription, merge video files, and upload the resulting video content to YouTube/Dailymotion. Additionally, it integrates with Notion to create a calendar and populate it with transcribed text from audio and video notes, accompanied by links to the original media. A Telegram bot is also provided for easy access to audio notes.
 
 ## Installation
 
 You can install MultiMedia Diary Tools via pip:
 
 ```bash
 pip install mmdiary
@@ -729,14 +729,15 @@
 - `MMDIARY_VIDEO_RES_DIR`: Results dir for video diary files
 - `MMDIARY_NOTION_API_KEY`: Your Notion API Key (see below).
 - `MMDIARY_NOTION_TOKEN`: Your Notion Auth Token v2 (see below).
 - `MMDIARY_NOTION_CACHE`: Notion uploader cache file
 - `MMDIARY_CACHE`: JSON processing cache file (to avoid reading all transribed files each run)
 - `MMDIARY_YOUTUBE_CLIENT_SECRETS`: Path to `client_secrets.json` (see below)
 - `MMDIARY_YOUTUBE_TOKEN`: Path to `token.json` (see below)
+- `MMDIARY_DAILYMOTION_ACCOUNTS`: Path to Dailymotion accounts configuration (see below)
 - `MMDIARY_NOTION_AUDIO_DB_ID`: Notion Audio DB ID (see below)
 - `MMDIARY_NOTION_VIDEO_DB_ID`: Notion Video DB ID (see below) 
 
 
 Example:
 
 ```bash
@@ -746,14 +747,15 @@
 export MMDIARY_VIDEO_RES_DIR="/path/to/wideo/result/dir"
 export MMDIARY_NOTION_API_KEY="your_notion_api_key_here"
 export MMDIARY_NOTION_TOKEN="your_notion_auth_token_v2_here"
 export MMDIARY_NOTION_CACHE="~/.mmdiary/notion_cache.pickle"
 export MMDIARY_CACHE="~/.mmdiary/json_cache.pickle"
 export MMDIARY_YOUTUBE_CLIENT_SECRETS="~/.mmdiary/client_secrets.json"
 export MMDIARY_YOUTUBE_TOKEN="~/.mmdiary/token.json"
+export MMDIARY_DAILYMOTION_ACCOUNTS="~/.mmdiary/dailymotion_accounts.json"
 export MMDIARY_NOTION_AUDIO_DB_ID="7da1480baa9f565198d3fa54c49b1b23"
 export MMDIARY_NOTION_VIDEO_DB_ID="25225aac51ea5cf0bcc74f8c225fbb63"
 ```
 
 ## Recommended Tools
 
 To ensure unique filenames for your files, it is recommended to use the [photo-importer](https://github.com/sashacmc/photo-importer) tool.
@@ -840,24 +842,84 @@
 
 2. **Submit the Request**:
    - Fill out the form with the necessary details about your project and the reasons for needing a higher quota.
    - Submit the form and wait for approval from the YouTube API team.
 
 ### Authenticating with YouTube API
 
-On the first run of `mmdiary-video-upload`, a URL will be provided. Follow these steps:
+On the first run of `mmdiary-video-upload-youtube`, a URL will be provided. Follow these steps:
 
 1. **Open the URL**:
    - Copy the provided URL and paste it into your web browser.
    - Select the Google account authorized for your `client_secrets.json`.
 
 2. **Enter the Authentication Code**:
    - Copy the authentication code provided after logging in.
    - Paste the authentication code into the prompt in your terminal.
    - This code will be saved in file specified by `MMDIARY_YOUTUBE_TOKEN` environment variable, and you won't need to repeat this process for future uploads.
+
+## Dailymotion Setup
+
+### Generating API Keys
+
+1. **Create a Dailymotion Account**:
+   - If you do not already have a Dailymotion account, create one at [Dailymotion](https://www.dailymotion.com).
+
+2. **Create an Application**:
+   - Go to the [Dailymotion Studio](https://www.dailymotion.com/partner/).
+   - Select "Organization setting/API keys"
+   - Click on "Generate API key" This will provide you with an `api_key` and `api_secret`.
+
+3. **Repeat for Multiple Accounts**:
+   - If you plan to use multiple Dailymotion accounts, repeat the process for each account to generate their respective `api_key` and `api_secret`.
+
+### Setting Up the Configuration File
+
+The configuration file should be a JSON file that contains the details of all Dailymotion accounts you wish to use. This file's path must be specified by the environment variable `MMDIARY_DAILYMOTION_ACCOUNTS`.
+
+### Note for Multiple Accounts
+
+A single Dailymotion account allows uploading only 15 videos per 24 hours. If you need to upload more videos within this period, you can set up multiple accounts.
+
+### Configuration File Format
+
+The configuration file should be structured as follows:
+
+```json
+{
+  "accounts": [
+    {
+      "name": "account01",
+      "username": "account01@example.com",
+      "password": "your_password",
+      "api_key": "your_api_key",
+      "api_secret": "your_api_secret"
+    },
+    {
+      "name": "account02",
+      "username": "account02@example.com",
+      "password": "your_password",
+      "api_key": "your_api_key",
+      "api_secret": "your_api_secret"
+    }
+  ]
+}
+```
+
+Replace the placeholder values with the actual account details, API keys, and API secrets.
+
+### Setting the Environment Variable
+
+To use the configuration file, set the environment variable `MMDIARY_DAILYMOTION_ACCOUNTS` to the path of your configuration file.
+
+Example for Unix-based systems:
+
+```bash
+export MMDIARY_DAILYMOTION_ACCOUNTS="~/.mmdiary/dailymotion_accounts.json"
+```
      
 ## Step-By-Step Process Overview
 
 ### Audio Diary
 
 #### Speech Recognition
 
@@ -895,21 +957,23 @@
 Use the `mmdiary-video-concat` utility to merge video files into a single daily video.
 
 Command:
 ```bash
 mmdiary-video-concat [dates ...]
 ```
 
-#### Upload to YouTube
+#### Upload to YouTube or Dailymotion
 
-Use the `mmdiary-video-upload` utility to upload the concatenated video to YouTube.
+Use the `mmdiary-video-upload-youtube` or `mmdiary-video-upload-dailymotion` utility to upload the concatenated video to YouTube/Dailymotion.
 
 Command:
 ```bash
-mmdiary-video-upload [dates ...]
+mmdiary-video-upload-youtube [dates ...]
+or
+mmdiary-video-upload-dailymotion [dates ...]
 ```
 
 #### Upload to Notion
 
 Use the `mmdiary-notion-upload` utility to upload the transcribed text with YouTube links to Notion.
 
 Command:
```

### Comparing `mmdiary-0.3.0/pyproject.toml` & `mmdiary-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mmdiary"
-version = "0.3.0"
+version = "0.4.0"
 description = "Multimedia Diary Tools"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["audio", "video", "multimedia", "tool", "youtube", "notion", "transcriber", "uploader"]
 
 authors = [
@@ -45,14 +45,16 @@
 	"notion_client",
 	"notion",
 	"progressbar2",
 	"python-telegram-bot",
 	"openai-whisper",
 	"photo_importer",
 	"mixvideoconcat",
+	"dailymotion",
+	"free-proxy",
 	"google-auth-oauthlib",
 	"google-api-python-client",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sashacmc/mmdiary"
 "Bug Reports" = "https://github.com/sashacmc/mmdiary/issues"
@@ -64,9 +66,10 @@
 mmdiary-notion-cleanup = "mmdiary.notion.cleanup:main"
 mmdiary-notion-cache = "mmdiary.notion.cache:main"
 mmdiary-telegrambot = "mmdiary.telegrambot.telegrambot_service:main"
 mmdiary-transcriber-run = "mmdiary.transcriber.transcriber:main"
 mmdiary-transcriber-verify = "mmdiary.transcriber.verifier:main"
 mmdiary-transcriber-search = "mmdiary.transcriber.searcher:main"
 mmdiary-video-concat = "mmdiary.video.processor:main"
-mmdiary-video-upload = "mmdiary.video.uploader:main"
+mmdiary-video-upload-youtube = "mmdiary.video.uploader.youtube:main"
+mmdiary-video-upload-dailymotion= "mmdiary.video.uploader.dailymotion:main"
 mmdiary-utils-datelib = "mmdiary.utils.datelib:main"
```

### Comparing `mmdiary-0.3.0/src/mmdiary/notion/cache.py` & `mmdiary-0.4.0/src/mmdiary/notion/cache.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.3.0/src/mmdiary/notion/cleanup.py` & `mmdiary-0.4.0/src/mmdiary/notion/cleanup.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.3.0/src/mmdiary/notion/uploader.py` & `mmdiary-0.4.0/src/mmdiary/notion/uploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from notion.block import AudioBlock, CalloutBlock, TextBlock, VideoBlock
 from notion.client import NotionClient
 from notion.collection import CollectionRowBlock
 from notion_client import Client
 
 from mmdiary.utils import log, medialib, progressbar
 from mmdiary.notion import cache
-from mmdiary.video.uploader import seconds_to_time
+from mmdiary.video.uploader import seconds_to_time, generate_video_url
 
 
 DESCRIPTION = """
 Uploads transcribed file(s) to the notion database.
 Please declare enviromnent variables before use:
     MMDIARY_NOTION_TOKEN - Notion web auth token, please obtain the `token_v2` value by inspectingn
         your browser cookies on a logged-in (non-guest) session on Notion.so
@@ -170,46 +170,47 @@
             "Video Diary",
             {
                 "source": "rich_text",
                 "processtime": "rich_text",
                 "Date": "date",
                 "Title": "title",
                 "Created time": "created_time",
+                "Provider": "rich_text",
+                "Account": "rich_text",
             },
         )
 
     def init_databases(self, parent_page_id):
         audio_db_id = self.__create_audio_database(parent_page_id)
         video_db_id = self.__create_video_database(parent_page_id)
 
         return audio_db_id, video_db_id
 
-    def __add_row(self, db_id, title, date, source, processtime, icon):
+    def __prop_rich_text(self, text):
+        return {
+            "type": "rich_text",
+            "rich_text": [
+                {
+                    "type": "text",
+                    "text": {"content": text},
+                },
+            ],
+        }
+
+    def __add_row(self, db_id, title, date, source, processtime, icon, provider=None, account=None):
         properties = {
             "title": {"title": [{"text": {"content": title}}]},
             "Date": {"type": "date", "date": {"start": date}},
-            "source": {
-                "type": "rich_text",
-                "rich_text": [
-                    {
-                        "type": "text",
-                        "text": {"content": source},
-                    },
-                ],
-            },
-            "processtime": {
-                "type": "rich_text",
-                "rich_text": [
-                    {
-                        "type": "text",
-                        "text": {"content": processtime},
-                    },
-                ],
-            },
+            "source": self.__prop_rich_text(source),
+            "processtime": self.__prop_rich_text(processtime),
         }
+        if provider is not None:
+            properties["Provider"] = self.__prop_rich_text(provider)
+        if account is not None:
+            properties["Account"] = self.__prop_rich_text(account)
 
         res = self.__notion_api.pages.create(
             parent={"database_id": db_id},
             icon={"type": "emoji", "emoji": icon},
             properties=properties,
         )
 
@@ -310,45 +311,47 @@
             self.__delete_page(None, bid)
             raise
 
         self.__status["created"] += 1
 
     def __create_video_page(self, file):
         if file.state() != "uploaded":
-            logging.debug("file not uploaded to YouTube yet: %s", file)
+            logging.debug("file not uploaded to video provider yet: %s", file)
             return
 
         if self.__dry_run:
             self.__status["created"] += 1
             return
 
         date = file.recorddate()
-        url = file.get_field("url")
+        provider = file.get_field("provider")
 
         bid = self.__add_row(
             self.__video_db_id,
             title=date,
             date=date,
             source=file.get_field("source"),
             processtime=file.get_field("processtime"),
+            provider=provider["name"],
+            account=provider["account"],
             icon="📹",
         )
         try:
             res = self.__notion.get_block(bid)
             video = res.children.add_new(VideoBlock)
-            video.set_source_url(url)
+            video.set_source_url(generate_video_url(provider))
 
             blocks = []
             pos = 0.0
             for video in file.get_field("videos"):
                 text = video["text"]
                 if text != "":
                     blocks += self.__gen_video_description_blocks(
                         seconds_to_time(int(pos)),
-                        f"{url}&t={int(pos)}s",
+                        generate_video_url(provider, pos),
                         medialib.get_time_from_timestring(video["timestamp"]),
                         text,
                     )
 
                 pos += float(video["duration"])
 
             for i in range(0, len(blocks), MAX_BLOCKS_BATCH_SIZE):
```

### Comparing `mmdiary-0.3.0/src/mmdiary/telegrambot/telegrambot_service.py` & `mmdiary-0.4.0/src/mmdiary/telegrambot/telegrambot_service.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.3.0/src/mmdiary/transcriber/searcher.py` & `mmdiary-0.4.0/src/mmdiary/transcriber/searcher.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.3.0/src/mmdiary/transcriber/transcriber.py` & `mmdiary-0.4.0/src/mmdiary/transcriber/transcriber.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.3.0/src/mmdiary/transcriber/verifier.py` & `mmdiary-0.4.0/src/mmdiary/transcriber/verifier.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.3.0/src/mmdiary/utils/datelib.py` & `mmdiary-0.4.0/src/mmdiary/utils/datelib.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,23 @@
                    (e.g. if video was deleted on the YouTube)
 """
 
 STATE_NONE = "none"
 STATE_INPROCESS = "inprocess"
 STATE_CONVERTED = "converted"
 STATE_UPLOADED = "uploaded"
+STATE_UPLOAD_VERIFICATION = "uploadverification"
 
 VALID_STATES = set(
     [
         STATE_NONE,
         STATE_INPROCESS,
         STATE_CONVERTED,
         STATE_UPLOADED,
+        STATE_UPLOAD_VERIFICATION,
     ]
 )
 
 
 class DateLib:
     def __init__(self):
         self.__scan_paths = list(
@@ -101,16 +103,21 @@
     def set_converted(self, date, fields):
         new_fields = {}
         if fields is not None:
             new_fields.update(fields)
         new_fields["state"] = STATE_CONVERTED
         self.results()[date].update_fields(new_fields)
 
-    def set_uploaded(self, date, url):
-        self.results()[date].update_fields({"state": STATE_UPLOADED, "url": url})
+    def set_uploaded(self, date, provider, for_verification=False):
+        self.results()[date].update_fields(
+            {
+                "state": STATE_UPLOAD_VERIFICATION if for_verification else STATE_UPLOADED,
+                "provider": provider,
+            }
+        )
 
     def set_state(self, date, state):
         if state not in VALID_STATES:
             raise UserWarning(f"Incorrect state: {state}")
         self.results()[date].update_fields({"state": state})
 
     def get_nonprocessed(self, masks=None):
@@ -134,16 +141,18 @@
             if mf.state() in states:
                 res.append(date)
         return sorted(self.__filter_by_masks(res, masks))
 
     def get_converted(self, masks=None):
         return self.__get_results_dates_by_state([STATE_CONVERTED], masks)
 
-    def get_uploaded(self, masks=None):
-        return self.__get_results_dates_by_state([STATE_UPLOADED], masks)
+    def get_uploaded(self, masks=None, for_verification=False):
+        return self.__get_results_dates_by_state(
+            [STATE_UPLOAD_VERIFICATION] if for_verification else [STATE_UPLOADED], masks
+        )
 
     def get_files_by_date(self, date, for_upload=False):
         mfs = self.sources()[date]
         if for_upload:
             mfs = list(filter(lambda mf: mf.json().get("upload", True), mfs))
         mfs.sort(key=lambda mf: mf.recordtime())
         return mfs
```

### Comparing `mmdiary-0.3.0/src/mmdiary/utils/jsoncache.py` & `mmdiary-0.4.0/src/mmdiary/utils/jsoncache.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,16 +22,18 @@
             return
         with open(self.__filename, "rb") as f:
             self.__data = pickle.load(f)
 
     def __save(self):
         if self.__filename is None or not self.__changed:
             return
-        with open(self.__filename, "wb") as f:
+        tmpfile = self.__filename + ".tmp"
+        with open(tmpfile, "wb") as f:
             pickle.dump(self.__data, f)
+        os.replace(tmpfile, self.__filename)
 
     def __load_json(self, filename):
         with open(filename, "r", encoding="utf-8") as f:
             return json.load(f)
 
     def __save_json(self, cont, filename):
         with open(filename, "w", encoding="utf-8") as f:
```

### Comparing `mmdiary-0.3.0/src/mmdiary/utils/log.py` & `mmdiary-0.4.0/src/mmdiary/utils/log.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.3.0/src/mmdiary/utils/medialib.py` & `mmdiary-0.4.0/src/mmdiary/utils/medialib.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         return filedname in self.json()
 
     def update_fields(self, fields):
         if self.have_json():
             self.json().update(fields)
         else:
             self.__json = fields
-        self.save_json(self.__json)
+        self.save_json({k: v for k, v in self.__json.items() if v is not None})
 
     def remove_json(self):
         if not self.__have_json:
             return
         os.unlink(self.json_name())
         self.__json = None
         self.__have_json = False
```

### Comparing `mmdiary-0.3.0/src/mmdiary/video/processor.py` & `mmdiary-0.4.0/src/mmdiary/video/processor.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.3.0/src/mmdiary.egg-info/PKG-INFO` & `mmdiary-0.4.0/src/mmdiary.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmdiary
-Version: 0.3.0
+Version: 0.4.0
 Summary: Multimedia Diary Tools
 Author-email: Alexander Bushnev <Alexander@Bushnev.pro>
 Maintainer-email: Alexander Bushnev <Alexander@Bushnev.pro>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -705,15 +705,15 @@
 # Multimedia Diary Tools 
 
 ![CodeQL](https://github.com/sashacmc/mmdiary/workflows/CodeQL/badge.svg)
 [![PyPI - Version](https://img.shields.io/pypi/v/mmdiary.svg)](https://pypi.org/project/mmdiary)
 [![PyPI - Downloads](https://pepy.tech/badge/mmdiary)](https://pepy.tech/project/mmdiary)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.commdiarym/psf/black)
 
-Multimedia Diary Tools is a Python toolkit designed to automate the process of managing multimedia content for diary entries. This toolkit offers functionalities to scan specified folders, identify audio and video files, perform speech-to-text transcription, merge video files, and upload the resulting video content to YouTube. Additionally, it integrates with Notion to create a calendar and populate it with transcribed text from audio and video notes, accompanied by links to the original media. A Telegram bot is also provided for easy access to audio notes.
+Multimedia Diary Tools is a Python toolkit designed to automate the process of managing multimedia content for diary entries. This toolkit offers functionalities to scan specified folders, identify audio and video files, perform speech-to-text transcription, merge video files, and upload the resulting video content to YouTube/Dailymotion. Additionally, it integrates with Notion to create a calendar and populate it with transcribed text from audio and video notes, accompanied by links to the original media. A Telegram bot is also provided for easy access to audio notes.
 
 ## Installation
 
 You can install MultiMedia Diary Tools via pip:
 
 ```bash
 pip install mmdiary
@@ -729,14 +729,15 @@
 - `MMDIARY_VIDEO_RES_DIR`: Results dir for video diary files
 - `MMDIARY_NOTION_API_KEY`: Your Notion API Key (see below).
 - `MMDIARY_NOTION_TOKEN`: Your Notion Auth Token v2 (see below).
 - `MMDIARY_NOTION_CACHE`: Notion uploader cache file
 - `MMDIARY_CACHE`: JSON processing cache file (to avoid reading all transribed files each run)
 - `MMDIARY_YOUTUBE_CLIENT_SECRETS`: Path to `client_secrets.json` (see below)
 - `MMDIARY_YOUTUBE_TOKEN`: Path to `token.json` (see below)
+- `MMDIARY_DAILYMOTION_ACCOUNTS`: Path to Dailymotion accounts configuration (see below)
 - `MMDIARY_NOTION_AUDIO_DB_ID`: Notion Audio DB ID (see below)
 - `MMDIARY_NOTION_VIDEO_DB_ID`: Notion Video DB ID (see below) 
 
 
 Example:
 
 ```bash
@@ -746,14 +747,15 @@
 export MMDIARY_VIDEO_RES_DIR="/path/to/wideo/result/dir"
 export MMDIARY_NOTION_API_KEY="your_notion_api_key_here"
 export MMDIARY_NOTION_TOKEN="your_notion_auth_token_v2_here"
 export MMDIARY_NOTION_CACHE="~/.mmdiary/notion_cache.pickle"
 export MMDIARY_CACHE="~/.mmdiary/json_cache.pickle"
 export MMDIARY_YOUTUBE_CLIENT_SECRETS="~/.mmdiary/client_secrets.json"
 export MMDIARY_YOUTUBE_TOKEN="~/.mmdiary/token.json"
+export MMDIARY_DAILYMOTION_ACCOUNTS="~/.mmdiary/dailymotion_accounts.json"
 export MMDIARY_NOTION_AUDIO_DB_ID="7da1480baa9f565198d3fa54c49b1b23"
 export MMDIARY_NOTION_VIDEO_DB_ID="25225aac51ea5cf0bcc74f8c225fbb63"
 ```
 
 ## Recommended Tools
 
 To ensure unique filenames for your files, it is recommended to use the [photo-importer](https://github.com/sashacmc/photo-importer) tool.
@@ -840,24 +842,84 @@
 
 2. **Submit the Request**:
    - Fill out the form with the necessary details about your project and the reasons for needing a higher quota.
    - Submit the form and wait for approval from the YouTube API team.
 
 ### Authenticating with YouTube API
 
-On the first run of `mmdiary-video-upload`, a URL will be provided. Follow these steps:
+On the first run of `mmdiary-video-upload-youtube`, a URL will be provided. Follow these steps:
 
 1. **Open the URL**:
    - Copy the provided URL and paste it into your web browser.
    - Select the Google account authorized for your `client_secrets.json`.
 
 2. **Enter the Authentication Code**:
    - Copy the authentication code provided after logging in.
    - Paste the authentication code into the prompt in your terminal.
    - This code will be saved in file specified by `MMDIARY_YOUTUBE_TOKEN` environment variable, and you won't need to repeat this process for future uploads.
+
+## Dailymotion Setup
+
+### Generating API Keys
+
+1. **Create a Dailymotion Account**:
+   - If you do not already have a Dailymotion account, create one at [Dailymotion](https://www.dailymotion.com).
+
+2. **Create an Application**:
+   - Go to the [Dailymotion Studio](https://www.dailymotion.com/partner/).
+   - Select "Organization setting/API keys"
+   - Click on "Generate API key" This will provide you with an `api_key` and `api_secret`.
+
+3. **Repeat for Multiple Accounts**:
+   - If you plan to use multiple Dailymotion accounts, repeat the process for each account to generate their respective `api_key` and `api_secret`.
+
+### Setting Up the Configuration File
+
+The configuration file should be a JSON file that contains the details of all Dailymotion accounts you wish to use. This file's path must be specified by the environment variable `MMDIARY_DAILYMOTION_ACCOUNTS`.
+
+### Note for Multiple Accounts
+
+A single Dailymotion account allows uploading only 15 videos per 24 hours. If you need to upload more videos within this period, you can set up multiple accounts.
+
+### Configuration File Format
+
+The configuration file should be structured as follows:
+
+```json
+{
+  "accounts": [
+    {
+      "name": "account01",
+      "username": "account01@example.com",
+      "password": "your_password",
+      "api_key": "your_api_key",
+      "api_secret": "your_api_secret"
+    },
+    {
+      "name": "account02",
+      "username": "account02@example.com",
+      "password": "your_password",
+      "api_key": "your_api_key",
+      "api_secret": "your_api_secret"
+    }
+  ]
+}
+```
+
+Replace the placeholder values with the actual account details, API keys, and API secrets.
+
+### Setting the Environment Variable
+
+To use the configuration file, set the environment variable `MMDIARY_DAILYMOTION_ACCOUNTS` to the path of your configuration file.
+
+Example for Unix-based systems:
+
+```bash
+export MMDIARY_DAILYMOTION_ACCOUNTS="~/.mmdiary/dailymotion_accounts.json"
+```
      
 ## Step-By-Step Process Overview
 
 ### Audio Diary
 
 #### Speech Recognition
 
@@ -895,21 +957,23 @@
 Use the `mmdiary-video-concat` utility to merge video files into a single daily video.
 
 Command:
 ```bash
 mmdiary-video-concat [dates ...]
 ```
 
-#### Upload to YouTube
+#### Upload to YouTube or Dailymotion
 
-Use the `mmdiary-video-upload` utility to upload the concatenated video to YouTube.
+Use the `mmdiary-video-upload-youtube` or `mmdiary-video-upload-dailymotion` utility to upload the concatenated video to YouTube/Dailymotion.
 
 Command:
 ```bash
-mmdiary-video-upload [dates ...]
+mmdiary-video-upload-youtube [dates ...]
+or
+mmdiary-video-upload-dailymotion [dates ...]
 ```
 
 #### Upload to Notion
 
 Use the `mmdiary-notion-upload` utility to upload the transcribed text with YouTube links to Notion.
 
 Command:
```

### Comparing `mmdiary-0.3.0/src/mmdiary.egg-info/SOURCES.txt` & `mmdiary-0.4.0/src/mmdiary.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,10 +20,14 @@
 src/mmdiary/transcriber/verifier.py
 src/mmdiary/utils/__init__.py
 src/mmdiary/utils/datelib.py
 src/mmdiary/utils/jsoncache.py
 src/mmdiary/utils/log.py
 src/mmdiary/utils/medialib.py
 src/mmdiary/utils/progressbar.py
+src/mmdiary/utils/proxypatch.py
 src/mmdiary/video/__init__.py
 src/mmdiary/video/processor.py
-src/mmdiary/video/uploader.py
+src/mmdiary/video/uploader/__init__.py
+src/mmdiary/video/uploader/common.py
+src/mmdiary/video/uploader/dailymotion.py
+src/mmdiary/video/uploader/youtube.py
```

