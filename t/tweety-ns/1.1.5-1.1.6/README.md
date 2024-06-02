# Comparing `tmp/tweety_ns-1.1.5.tar.gz` & `tmp/tweety_ns-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety_ns-1.1.5.tar", last modified: Sun Apr 28 18:06:24 2024, max compression
+gzip compressed data, was "tweety_ns-1.1.6.tar", last modified: Sun Jun  2 18:01:52 2024, max compression
```

## Comparing `tweety_ns-1.1.5.tar` & `tweety_ns-1.1.6.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.247461 tweety_ns-1.1.5/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-28 18:06:24.247461 tweety_ns-1.1.5/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety_ns-1.1.5/README.md
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety_ns-1.1.5/pyproject.toml
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      671 2024-04-28 18:06:24.247461 tweety_ns-1.1.5/setup.cfg
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      785 2024-04-28 18:03:59.000000 tweety_ns-1.1.5/setup.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.239461 tweety_ns-1.1.5/src/
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.243461 tweety_ns-1.1.5/src/tweety/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      276 2024-04-28 18:03:47.000000 tweety_ns-1.1.5/src/tweety/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     7526 2024-04-27 08:15:36.000000 tweety_ns-1.1.5/src/tweety/auth.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    31976 2024-04-27 09:34:06.000000 tweety_ns-1.1.5/src/tweety/bot.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    99908 2024-04-28 16:22:34.000000 tweety_ns-1.1.5/src/tweety/builder.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.243461 tweety_ns-1.1.5/src/tweety/events/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety_ns-1.1.5/src/tweety/events/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2083 2024-04-27 09:38:42.000000 tweety_ns-1.1.5/src/tweety/events/newmessage.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    22029 2024-04-14 08:52:30.000000 tweety_ns-1.1.5/src/tweety/exceptions_.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2343 2024-04-23 07:03:34.000000 tweety_ns-1.1.5/src/tweety/filters.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    21533 2024-04-28 17:21:24.000000 tweety_ns-1.1.5/src/tweety/http.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2362 2024-04-10 16:34:41.000000 tweety_ns-1.1.5/src/tweety/session.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.247461 tweety_ns-1.1.5/src/tweety/types/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1363 2024-04-28 17:55:38.000000 tweety_ns-1.1.5/src/tweety/types/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3094 2024-04-28 09:58:11.000000 tweety_ns-1.1.5/src/tweety/types/base.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1172 2024-01-20 09:02:27.000000 tweety_ns-1.1.5/src/tweety/types/bookmarks.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3256 2024-01-20 09:00:34.000000 tweety_ns-1.1.5/src/tweety/types/community.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4054 2024-02-22 14:22:03.000000 tweety_ns-1.1.5/src/tweety/types/follow.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      987 2024-01-20 08:43:34.000000 tweety_ns-1.1.5/src/tweety/types/gifs.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    23118 2024-04-28 17:55:38.000000 tweety_ns-1.1.5/src/tweety/types/inbox.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1444 2024-03-03 17:35:17.000000 tweety_ns-1.1.5/src/tweety/types/likes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4302 2024-01-20 08:28:50.000000 tweety_ns-1.1.5/src/tweety/types/lists.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1511 2024-01-19 19:19:11.000000 tweety_ns-1.1.5/src/tweety/types/mentions.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     9173 2024-04-28 17:48:11.000000 tweety_ns-1.1.5/src/tweety/types/n_types.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1351 2024-01-19 19:15:58.000000 tweety_ns-1.1.5/src/tweety/types/notification.py
--rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1103 2024-03-20 05:31:04.000000 tweety_ns-1.1.5/src/tweety/types/places.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-01-19 19:12:37.000000 tweety_ns-1.1.5/src/tweety/types/retweets.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3806 2024-02-03 16:37:11.000000 tweety_ns-1.1.5/src/tweety/types/search.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1216 2024-01-31 06:59:29.000000 tweety_ns-1.1.5/src/tweety/types/topic.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    58815 2024-04-14 08:56:44.000000 tweety_ns-1.1.5/src/tweety/types/twDataTypes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12236 2024-04-12 07:15:06.000000 tweety_ns-1.1.5/src/tweety/types/usertweet.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety_ns-1.1.5/src/tweety/updates.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    39586 2024-04-28 18:03:47.000000 tweety_ns-1.1.5/src/tweety/user.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     6771 2024-04-28 18:03:47.000000 tweety_ns-1.1.5/src/tweety/utils.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-28 18:06:24.247461 tweety_ns-1.1.5/src/tweety_ns.egg-info/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-28 18:06:24.000000 tweety_ns-1.1.5/src/tweety_ns.egg-info/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1026 2024-04-28 18:06:24.000000 tweety_ns-1.1.5/src/tweety_ns.egg-info/SOURCES.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-04-28 18:06:24.000000 tweety_ns-1.1.5/src/tweety_ns.egg-info/dependency_links.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-04-28 18:06:24.000000 tweety_ns-1.1.5/src/tweety_ns.egg-info/requires.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-04-28 18:06:24.000000 tweety_ns-1.1.5/src/tweety_ns.egg-info/top_level.txt
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-06-02 18:01:52.538658 tweety_ns-1.1.6/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-06-02 18:01:52.538658 tweety_ns-1.1.6/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety_ns-1.1.6/README.md
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety_ns-1.1.6/pyproject.toml
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)      671 2024-06-02 18:01:52.538658 tweety_ns-1.1.6/setup.cfg
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)      759 2024-06-02 16:34:21.000000 tweety_ns-1.1.6/setup.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-06-02 18:01:52.534658 tweety_ns-1.1.6/src/
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-06-02 18:01:52.534658 tweety_ns-1.1.6/src/tweety/
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)      259 2024-06-02 17:45:20.000000 tweety_ns-1.1.6/src/tweety/__init__.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     7214 2024-06-02 17:45:09.000000 tweety_ns-1.1.6/src/tweety/auth.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)    33846 2024-06-02 17:23:58.000000 tweety_ns-1.1.6/src/tweety/bot.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)   102150 2024-06-02 16:34:21.000000 tweety_ns-1.1.6/src/tweety/builder.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)      437 2024-06-02 17:29:43.000000 tweety_ns-1.1.6/src/tweety/constants.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-06-02 18:01:52.534658 tweety_ns-1.1.6/src/tweety/events/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety_ns-1.1.6/src/tweety/events/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2083 2024-04-27 09:38:42.000000 tweety_ns-1.1.6/src/tweety/events/newmessage.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)    22217 2024-06-02 16:34:21.000000 tweety_ns-1.1.6/src/tweety/exceptions.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)      103 2024-06-02 16:34:21.000000 tweety_ns-1.1.6/src/tweety/exceptions_.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2343 2024-04-23 07:03:34.000000 tweety_ns-1.1.6/src/tweety/filters.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)    21748 2024-06-02 17:36:25.000000 tweety_ns-1.1.6/src/tweety/http.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     2290 2024-06-02 16:34:21.000000 tweety_ns-1.1.6/src/tweety/session.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-06-02 18:01:52.538658 tweety_ns-1.1.6/src/tweety/types/
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1471 2024-06-02 17:32:09.000000 tweety_ns-1.1.6/src/tweety/types/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3189 2024-06-02 17:56:19.000000 tweety_ns-1.1.6/src/tweety/types/base.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1183 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/bookmarks.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3247 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/community.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     4855 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/follow.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      998 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/gifs.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)    22548 2024-06-02 17:32:24.000000 tweety_ns-1.1.6/src/tweety/types/inbox.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1426 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/likes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4313 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/lists.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1463 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/mentions.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     8662 2024-06-02 17:34:42.000000 tweety_ns-1.1.6/src/tweety/types/n_types.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1366 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/notification.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1114 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/places.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-06-02 17:25:44.000000 tweety_ns-1.1.6/src/tweety/types/retweets.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3786 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/search.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1227 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/topic.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)    58670 2024-06-02 17:32:09.000000 tweety_ns-1.1.6/src/tweety/types/twDataTypes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12222 2024-06-02 17:26:20.000000 tweety_ns-1.1.6/src/tweety/types/usertweet.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety_ns-1.1.6/src/tweety/updates.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)    39550 2024-06-02 16:34:21.000000 tweety_ns-1.1.6/src/tweety/user.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     7152 2024-06-02 17:58:38.000000 tweety_ns-1.1.6/src/tweety/utils.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-06-02 18:01:52.538658 tweety_ns-1.1.6/src/tweety_ns.egg-info/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-06-02 18:01:52.000000 tweety_ns-1.1.6/src/tweety_ns.egg-info/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1075 2024-06-02 18:01:52.000000 tweety_ns-1.1.6/src/tweety_ns.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-06-02 18:01:52.000000 tweety_ns-1.1.6/src/tweety_ns.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-06-02 18:01:52.000000 tweety_ns-1.1.6/src/tweety_ns.egg-info/requires.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-06-02 18:01:52.000000 tweety_ns-1.1.6/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety_ns-1.1.5/PKG-INFO` & `tweety_ns-1.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.5
+Version: 1.1.6
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety_ns-1.1.5/README.md` & `tweety_ns-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.5/setup.cfg` & `tweety_ns-1.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tweety-ns
-version = 1.1.5
+version = 1.1.6
 author = Tayyab Kharl
 author_email = tayyabmahr@gmail.com
 description = An easy Twitter Scraper
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mahrtayyab/tweety
 project_urls =
```

### Comparing `tweety_ns-1.1.5/setup.py` & `tweety_ns-1.1.6/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from distutils.core import setup
-
-setup(
-    name='tweety-ns',
-    packages=['tweety', 'tweety.types', 'tweety.events'],
-    version='1.1.5',
-    license='MIT',
-    description='An easy Twitter Scraper',
-    author='Tayyab Kharl',
-    author_email='tayyabmahr@gmail.com',
-    url='https://github.com/mahrtayyab/tweety',
-    keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
-    install_requires=[
-        'beautifulsoup4',
-        'openpyxl',
-        'httpx',
-        'dateutils',
-    ],
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3'
-    ],
-)
+from distutils.core import setup
+
+setup(
+    name='tweety-ns',
+    packages=['tweety', 'tweety.types', 'tweety.events'],
+    version='1.1.6',
+    license='MIT',
+    description='An easy Twitter Scraper',
+    author='Tayyab Kharl',
+    author_email='tayyabmahr@gmail.com',
+    url='https://github.com/mahrtayyab/tweety',
+    keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
+    install_requires=[
+        'beautifulsoup4',
+        'openpyxl',
+        'httpx',
+        'dateutils',
+    ],
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3'
+    ],
+)
```

### Comparing `tweety_ns-1.1.5/src/tweety/auth.py` & `tweety_ns-1.1.6/src/tweety/auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,191 +1,190 @@
-import getpass
-from http.cookiejar import MozillaCookieJar
-from typing import Union
-from .exceptions_ import InvalidCredentials, DeniedLogin, ActionRequired
-from .builder import FlowData
-from .types.n_types import Cookies
-from .utils import find_objects
-
-
-class AuthMethods:
-
-    def connect(self):
-        """
-        This method will be used to connect to already saved session in disk
-        """
-
-        if not self.session.logged_in:
-            return
-
-        self.request.set_cookies(str(self.session))
-        self.user = self.get_user_info(self.request.username)
-        self.request.set_user(self.user)
-        self.session.set_session_user(self.user)
-        self._is_connected = True
-        self.is_user_authorized = True
-        return self.user
-
-    def start(
-            self,
-            username=None,
-            password=None,
-            *,
-            extra=None
-    ):
-        """
-        Interactive Version of `sign_in` which will ask user for inputs
-        Most of the time , this would be the only method you will be working with,
-        it will check for existing sessions and login to it if available
-
-        :param username: (`str`) Username of the user
-        :param password: (`str`) Password of the user
-        :param extra: (`str`) If you have 2-Factor authentication enabled and already have a code ,
-                                or any other action required for completing the login process
-                                it will be passed to this parameter
-        :return: .types.twDataTypes.User (the user which is authenticated)
-        """
-
-        if self.session.logged_in:
-            try:
-                return self.connect()
-            except InvalidCredentials:
-                self.request.set_cookies("", False)
-                pass
-
-        username = input('Please enter the Username: ') if not username else username
-        password = getpass.getpass('Please enter your password: ') if not password else password
-
-        _extra_once = False
-        while not self.logged_in:
-            try:
-                return self.sign_in(username, password, extra=extra)
-            except ActionRequired as e:
-                action = input(f"\rAction Required :> {str(e.message)} : ")
-                _extra_once = True
-                return self.sign_in(username, password, extra=action)
-            except InvalidCredentials as ask_info:
-                if _extra_once:
-                    action = input(f"\rAction Required :> {str(ask_info.message)} : ")
-                    return self.sign_in(username, password, extra=action)
-                else:
-                    raise ask_info
-
-    def sign_in(
-            self,
-            username,
-            password,
-            *,
-            extra=None
-    ):
-        """
-        - This method can be used to sign in to Twitter using username and password
-        - It will also check for the saved session for the username in the disk
-
-        :param username: (`str`) Username of the user
-        :param password: (`str`) Password of the user
-        :param extra: (`str`) If you have 2-Factor authentication enabled and already have a code ,
-                                or any other action required for completing the login process
-                                it will be passed to this parameter
-        :return: .types.twDataTypes.User (the user which is authenticated)
-        """
-
-        if self.session.logged_in and self.session.user['username'].lower() == username.lower():
-            try:
-                return self.connect()
-            except InvalidCredentials:
-                self.request.set_cookies("", False)
-                pass
-
-        self._username = username
-        self._password = password
-        self._extra = extra
-
-        if not self._login_flow:
-            self._login_flow = FlowData()
-
-        if not self._login_flow_state:
-            self._login_flow_state = self._login_flow.initial_state
-
-        return self._login()
-
-    def load_cookies(
-            self,
-            cookies: Union[str, dict, MozillaCookieJar]
-    ):
-        """
-        This method can be used to load the already authenticated cookies from Twitter
-
-        :param cookies:  (`str`, `dict`, `MozillaCookieJar`) The Cookies to load
-        :return: .types.twDataTypes.User (the user which is authenticated)
-        """
-        self.cookies = Cookies(cookies, False)
-        self.logged_in = True
-        self.session.save_session(self.cookies)
-        return self.connect()
-
-    def load_auth_token(self, auth_token):
-        URL = "https://twitter.com/i/api/1.1/account/update_profile.json"
-        temp_cookie = {"auth_token": auth_token}
-        res = self.request.session.post(URL, cookies=temp_cookie)
-        ct0 = res.cookies.get('ct0')
-
-        if not ct0:
-            raise DeniedLogin(response=res, message="Auth Token isn't Valid")
-
-        temp_cookie['ct0'] = ct0
-        return self.load_cookies(temp_cookie)
-
-    @staticmethod
-    def _get_action_text(response):
-        primary_message = find_objects(response, 'primary_text', None, none_value={})
-        secondary_message = find_objects(response, 'secondary_text', None, none_value={})
-        if primary_message:
-            if isinstance(primary_message, list):
-                primary_message = primary_message[0]
-
-            primary_message = primary_message.get('text', '')
-
-        if secondary_message:
-            if isinstance(secondary_message, list):
-                secondary_message = secondary_message[0]
-            secondary_message = secondary_message.get('text', '')
-        return f"{primary_message}. {secondary_message}"
-
-    def _login(self):
-        _username, _password, _extra = self._username, self._password, self._extra
-
-        while not self.logged_in:
-            _login_payload = self._login_flow.get(self._login_flow_state, json_=self._last_json, username=_username, password=_password, extra=_extra)
-            response = self.request.login(self._login_url, _payload=_login_payload)
-
-            self._last_json = response.json()
-
-            if response.cookies.get("att"):
-                self.request.add_header("Att", response.cookies.get("att"))
-
-            if self._last_json.get('status') != "success":
-                raise DeniedLogin(response=response, message=response.text)
-
-            self._login_url = self._login_url.split("?")[0]
-            subtask = self._last_json["subtasks"][0].get("subtask_id")
-            self._login_flow_state = subtask
-
-            if subtask in ("LoginTwoFactorAuthChallenge", "LoginAcid", "LoginEnterAlternateIdentifierSubtask") and not _extra:
-                message = self._get_action_text(self._last_json)
-                raise ActionRequired(0, "ActionRequired", response, message)
-
-            if subtask == "DenyLoginSubtask":
-                reason = self._get_action_text(self._last_json)
-                raise DeniedLogin(response=response, message=reason)
-
-            if subtask == "LoginSuccessSubtask":
-                self.request.remove_header("Att")
-                self.logged_in = True
-                self.cookies = Cookies(dict(response.cookies))
-                self.session.save_session(self.cookies)
-                return self.connect()
-
-        raise DeniedLogin(response=response, message="Unknown Error Occurred")
-
-
-
+import getpass
+from http.cookiejar import MozillaCookieJar
+from typing import Union
+from .exceptions import InvalidCredentials, DeniedLogin, ActionRequired
+from .builder import FlowData
+from .types.n_types import Cookies
+from .utils import find_objects
+
+
+class AuthMethods:
+
+    def connect(self):
+        """
+        This method will be used to connect to already saved session in disk
+        """
+
+        if not self.session.logged_in:
+            return
+
+        self.request.set_cookies(str(self.session))
+        self.user = self.get_user_info(self.request.username)
+        self.request.set_user(self.user)
+        self.session.set_session_user(self.user)
+        self._is_connected = True
+        self.is_user_authorized = True
+        return self.user
+
+    def start(
+            self,
+            username=None,
+            password=None,
+            *,
+            extra=None
+    ):
+        """
+        Interactive Version of `sign_in` which will ask user for inputs
+        Most of the time , this would be the only method you will be working with,
+        it will check for existing sessions and login to it if available
+
+        :param username: (`str`) Username of the user
+        :param password: (`str`) Password of the user
+        :param extra: (`str`) If you have 2-Factor authentication enabled and already have a code ,
+                                or any other action required for completing the login process
+                                it will be passed to this parameter
+        :return: .types.twDataTypes.User (the user which is authenticated)
+        """
+
+        if self.session.logged_in:
+            try:
+                return self.connect()
+            except InvalidCredentials:
+                self.request.set_cookies("", False)
+                pass
+
+        username = input('Please enter the Username: ') if not username else username
+        password = getpass.getpass('Please enter your password: ') if not password else password
+
+        _extra = extra
+        _extra_once = False
+        while not self.logged_in:
+            try:
+                return self.sign_in(username, password, extra=_extra)
+            except ActionRequired as e:
+                _extra = input(f"\rAction Required :> {str(e.message)} : ")
+                _extra_once = True
+            except InvalidCredentials as ask_info:
+                if _extra_once:
+                    _extra = input(f"\rAction Required :> {str(ask_info.message)} : ")
+                else:
+                    raise ask_info
+
+    def sign_in(
+            self,
+            username,
+            password,
+            *,
+            extra=None
+    ):
+        """
+        - This method can be used to sign in to Twitter using username and password
+        - It will also check for the saved session for the username in the disk
+
+        :param username: (`str`) Username of the user
+        :param password: (`str`) Password of the user
+        :param extra: (`str`) If you have 2-Factor authentication enabled and already have a code ,
+                                or any other action required for completing the login process
+                                it will be passed to this parameter
+        :return: .types.twDataTypes.User (the user which is authenticated)
+        """
+
+        if self.session.logged_in and self.session.user['username'].lower() == username.lower():
+            try:
+                return self.connect()
+            except InvalidCredentials:
+                self.request.set_cookies("", False)
+                pass
+
+        self._username = username
+        self._password = password
+        self._extra = extra
+
+        if not self._login_flow:
+            self._login_flow = FlowData()
+
+        if not self._login_flow_state:
+            self._login_flow_state = self._login_flow.initial_state
+
+        return self._login()
+
+    def load_cookies(
+            self,
+            cookies: Union[str, dict, MozillaCookieJar]
+    ):
+        """
+        This method can be used to load the already authenticated cookies from Twitter
+
+        :param cookies:  (`str`, `dict`, `MozillaCookieJar`) The Cookies to load
+        :return: .types.twDataTypes.User (the user which is authenticated)
+        """
+        self.cookies = Cookies(cookies, False)
+        self.logged_in = True
+        self.session.save_session(self.cookies)
+        return self.connect()
+
+    def load_auth_token(self, auth_token):
+        URL = "https://twitter.com/i/api/1.1/account/update_profile.json"
+        temp_cookie = {"auth_token": auth_token}
+        res = self.request.session.post(URL, cookies=temp_cookie)
+        ct0 = res.cookies.get('ct0')
+
+        if not ct0:
+            raise DeniedLogin(response=res, message="Auth Token isn't Valid")
+
+        temp_cookie['ct0'] = ct0
+        return self.load_cookies(temp_cookie)
+
+    @staticmethod
+    def _get_action_text(response):
+        primary_message = find_objects(response, 'primary_text', None, none_value={})
+        secondary_message = find_objects(response, 'secondary_text', None, none_value={})
+        if primary_message:
+            if isinstance(primary_message, list):
+                primary_message = primary_message[0]
+
+            primary_message = primary_message.get('text', '')
+
+        if secondary_message:
+            if isinstance(secondary_message, list):
+                secondary_message = secondary_message[0]
+            secondary_message = secondary_message.get('text', '')
+        return f"{primary_message}. {secondary_message}"
+
+    def _login(self):
+        _username, _password, _extra = self._username, self._password, self._extra
+
+        while not self.logged_in:
+            _login_payload = self._login_flow.get(self._login_flow_state, json_=self._last_json, username=_username, password=_password, extra=_extra)
+            response = self.request.login(self._login_url, _payload=_login_payload)
+
+            self._last_json = response.json()
+
+            if response.cookies.get("att"):
+                self.request.add_header("Att", response.cookies.get("att"))
+
+            if self._last_json.get('status') != "success":
+                raise DeniedLogin(response=response, message=response.text)
+
+            self._login_url = self._login_url.split("?")[0]
+            subtask = self._last_json["subtasks"][0].get("subtask_id")
+            self._login_flow_state = subtask
+
+            if subtask in ("LoginTwoFactorAuthChallenge", "LoginAcid", "LoginEnterAlternateIdentifierSubtask") and not _extra:
+                message = self._get_action_text(self._last_json)
+                raise ActionRequired(0, "ActionRequired", response, message)
+
+            if subtask == "DenyLoginSubtask":
+                reason = self._get_action_text(self._last_json)
+                raise DeniedLogin(response=response, message=reason)
+
+            if subtask == "LoginSuccessSubtask":
+                self.request.remove_header("Att")
+                self.logged_in = True
+                self.cookies = Cookies(dict(response.cookies))
+                self.session.save_session(self.cookies)
+                return self.connect()
+
+        raise DeniedLogin(response=response, message="Unknown Error Occurred")
+
+
+
```

### Comparing `tweety_ns-1.1.5/src/tweety/bot.py` & `tweety_ns-1.1.6/src/tweety/bot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,864 +1,937 @@
-import warnings
-from typing import Union
-from .utils import find_objects, AuthRequired, get_user_from_typehead, get_tweet_id, check_translation_lang
-from .types import (Proxy, TweetComments, UserTweets, Search, User, Tweet, Trends, Community, CommunityTweets,
-                    CommunityMembers, UserFollowers, UserFollowings, TweetHistory, UserMedia, GifSearch,
-                    ShortUser, TypeHeadSearch, TweetTranslate, AudioSpace, UserHighlights, UserLikes, Places)
-from .exceptions_ import *
-from .session import Session, MemorySession, FileSession
-from .http import Request
-
-
-class BotMethods:
-    LOGIN_URL = "https://api.twitter.com/1.1/onboarding/task.json?flow_name=login"
-
-    def __init__(self, session_name: Union[str, Session], proxy: Union[dict, Proxy] = None, **httpx_kwargs):
-        """
-        Constructor of the Twitter Public class
-
-        :param: session_name: (`str`, `Session`) This is the name of the session which will be saved and can be loaded later
-        :param: proxy: (`dict` or `Proxy`) Provide the proxy you want to use while making a request
-        """
-
-        self._login_url = self.LOGIN_URL
-        self._username = None
-        self._password = None
-        self._extra = None
-        self._login_flow = None
-        self._login_flow_state = None
-        self._last_json = {}
-        self._cached_users = {}
-        self._proxy = proxy.get_dict() if isinstance(proxy, Proxy) else proxy
-        self._event_builders = []
-
-        if isinstance(session_name, MemorySession):
-            self.session = session_name(self)
-        elif isinstance(session_name, FileSession):
-            self.session = session_name
-        else:
-            self.session = FileSession(self, session_name)
-
-        self.logged_in = False
-        self.is_user_authorized = False
-        self.request = self.http = Request(self, max_retries=10, proxy=self._proxy, **httpx_kwargs)
-        self.user = None
-
-    def get_user_info(self, username: Union[str, int, list] = None):
-        """
-        Get the User Info of the specified username
-
-        :param: username: (`str` | `int` | List[`str`, `int`]) username or user_id to get information of
-
-        :return: .types.twDataTypes.User
-        """
-
-        if not username and self.user is not None:
-            username = self.user.username
-
-        if isinstance(username, list):
-            for i in username:
-                if not str(i).isdigit():
-                    raise ValueError("Only Accept List of User IDs.")
-
-        if isinstance(username, list) or str(username).isdigit() or isinstance(username, int):
-            usernames = [username] if not isinstance(username, list) else username
-            users_raw = self.request.get_users_by_rest_id(usernames)
-            users = find_objects(users_raw, "users", None, recursive=False, none_value=[])
-
-            parsed_users = []
-            for user in users:
-                try:
-                    this_user = User(self, user)
-                    parsed_users.append(this_user)
-                    self._cached_users[str(this_user.username).lower()] = this_user.id
-                except Exception as e:
-                    warnings.warn(f"UsersByRestId Error: {str(e)}")
-
-            if len(usernames) == 1 and len(parsed_users) > 0:
-                return parsed_users[0]
-            elif len(usernames) == 1 and len(parsed_users) == 0:
-                return None
-            elif len(usernames) > 1 and len(parsed_users) == 0:
-                return []
-            else:
-                return parsed_users
-        else:
-            user_raw = self.request.get_user(username)
-            user = User(self, user_raw)
-            self._cached_users[str(username).lower()] = user.id
-            return user
-
-    @property
-    def user_id(self) -> int:
-        """
-        Get the user unique twitter id of authenticated user
-
-        :return: int
-        """
-        return self.user.id if self.user else None
-
-    @property
-    def cache(self):
-        return self._cached_users
-
-    def get_user_id(self, username: str):
-        return self._get_user_id(username)
-
-    def _get_user_id(self, username):
-        if isinstance(username, (User, ShortUser)):
-            user_id = username.id
-        elif isinstance(username, int) or (isinstance(username, str) and str(username).isdigit()):
-            user_id = username
-        elif self._cached_users.get(username.lower()):
-            user_id = self._cached_users[username.lower()]
-        else:
-            user = get_user_from_typehead(username, self.typehead_user_search(username))
-
-            if not user:
-                user = self.get_user_info(username)
-
-            if user:
-                user_id = user.id
-            else:
-                raise UserNotFound()
-        return user_id
-
-    def get_tweets(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            replies: bool = False,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ) -> UserTweets:
-        """
-         Get the tweets from a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: replies: (`boolean`) get the replied tweets of the user too
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: .types.usertweet.UserTweets
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        user_id = self._get_user_id(username)
-
-        userTweets = UserTweets(user_id, self, pages, replies, wait_time, cursor)
-
-        list(userTweets.generator())
-
-        return userTweets
-
-    def iter_tweets(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            replies: bool = False,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-
-        """
-         Generator for getting the tweets from a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: replies: (`boolean`) get the replied tweets of the user too
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: (.types.usertweet.UserTweets, list[.types.twDataTypes.Tweet])
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        user_id = self._get_user_id(username)
-
-        userTweets = UserTweets(user_id, self, pages, replies, wait_time, cursor)
-
-        return userTweets.generator()
-
-    def get_user_highlights(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            replies: bool = False,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-        """
-         Get the tweets from a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: replies: (`boolean`) get the replied tweets of the user too
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: .types.usertweet.userHighlights
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        user_id = self._get_user_id(username)
-
-        userHighlights = UserHighlights(user_id, self, pages, replies, wait_time, cursor)
-
-        list(userHighlights.generator())
-
-        return userHighlights
-
-    def iter_user_highlights(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            replies: bool = False,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-
-        """
-         Generator for getting the tweets from a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: replies: (`boolean`) get the replied tweets of the user too
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: (.types.usertweet.UserHighlights, list[.types.twDataTypes.Tweet])
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        user_id = self._get_user_id(username)
-
-        userHighlights = UserHighlights(user_id, self, pages, replies, wait_time, cursor)
-
-        return userHighlights.generator()
-
-    def get_user_likes(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            replies: bool = False,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-        """
-         Get the liked tweets of a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: replies: (`boolean`) get the replied tweets of the user too
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: .types.usertweet.userLikes
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        user_id = self._get_user_id(username)
-
-        userLikes = UserLikes(user_id, self, pages, replies, wait_time, cursor)
-
-        list(userLikes.generator())
-
-        return userLikes
-
-    def iter_user_likes(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            replies: bool = False,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-
-        """
-         Generator for getting the liked tweets of a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: replies: (`boolean`) get the replied tweets of the user too
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: (.types.usertweet.UserLikes, list[.types.twDataTypes.Tweet])
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        user_id = self._get_user_id(username)
-
-        userLikes = UserLikes(user_id, self, pages, replies, wait_time, cursor)
-
-        return userLikes.generator()
-
-    @AuthRequired
-    def get_user_media(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ) -> UserMedia:
-        """
-         Get the media from a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: .types.usertweet.UserMedia
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        user_id = self._get_user_id(username)
-
-        userMedia = UserMedia(user_id, self, pages, wait_time, cursor)
-
-        list(userMedia.generator())
-
-        return userMedia
-
-    @AuthRequired
-    def iter_user_media(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-
-        """
-         Generator for getting the media from a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: (.types.usertweet.UserMedia, list[.types.twDataTypes.Tweet])
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        user_id = self._get_user_id(username)
-
-        userMedia = UserMedia(user_id, self, pages, wait_time, cursor)
-
-        return userMedia.generator()
-
-    @AuthRequired
-    def get_trends(self):
-        """
-        Get the Trends from you locale
-
-        :return: list of .types.twDataTypes.Trends
-        """
-        trends = []
-        response = self.request.get_trends()
-
-        entries = find_objects(response, "addEntries", None)
-        if not entries or len(entries) == 0:
-            return trends
-
-        for entry in entries['entries']:
-            if str(entry['entryId']) == "trends":
-                for item in entry['content']['timelineModule']['items']:
-                    trends.append(Trends(self, item))
-
-        return trends
-
-    @AuthRequired
-    def search(
-            self,
-            keyword: str,
-            pages: int = 1,
-            filter_: str = None,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ) -> Search:
-
-        """
-        Search for a keyword or hashtag on Twitter
-
-        :param: keyword: (`str`) The keyword which is supposed to be searched
-        :param: pages: (`int`) The number of pages to get
-        :param: filter_: (
-           `str`| `filters.SearchFilters.Users()`| `filters.SearchFilters.Latest()` | `filters.SearchFilters.Photos()` | `filters.SearchFilters.Videos()`
-        )
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-
-        :return: .types.search.Search
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        search = Search(keyword, self, pages, filter_, wait_time, cursor)
-
-        list(search.generator())
-
-        return search
-
-    @AuthRequired
-    def iter_search(
-            self,
-            keyword: str,
-            pages: int = 1,
-            filter_: str = None,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-        """
-        Search for a keyword or hashtag on Twitter
-
-        :param: keyword: (`str`) The keyword which is supposed to be searched
-        :param: pages: (`int`) The number of pages to get
-        :param: filter_: (
-           `str`| `filters.SearchFilters.Users()`| `filters.SearchFilters.Latest()` | `filters.SearchFilters.Photos()` | `filters.SearchFilters.Videos()`
-        )
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-
-        :return: (.types.search.Search, list[.types.twDataTypes.Tweet])
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        search = Search(keyword, self, pages, filter_, wait_time, cursor)
-
-        return search.generator()
-
-    @AuthRequired
-    def typehead_user_search(self, keyword):
-        return TypeHeadSearch(self, keyword, "users")
-
-    @AuthRequired
-    def get_audio_space(self, space_id: Union[str, Tweet]) -> AudioSpace:
-        """
-
-        :param: space_id: ID of the Audio Space , or the Tweet Object that Space Audio is part of.
-        :return: .types.twDataTypes.AudioSpace
-        """
-
-        if isinstance(space_id, Tweet):
-            space_id = space_id.audio_space_id
-
-        space = self.http.get_audio_space(space_id)
-
-        if not find_objects(space, "metadata", None):
-            raise AudioSpaceNotFound(404, "BadRequest", response=space)
-
-        return AudioSpace(self, space)
-
-    @AuthRequired
-    def get_community(self, community_id):
-        """
-
-        :param: community_id: ID of the community to get
-        :return:
-        """
-
-        response = self.http.get_community(community_id)
-        return Community(self, response)
-
-    @AuthRequired
-    def iter_community_tweets(
-            self,
-            community_id: Union[str, int, Community],
-            pages: int = 1,
-            filter_: str = None,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-
-        """
-         Generator for getting the tweets from a community
-
-        :param: community_id: (`str` | `int` | `Community`) ID of the community whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: filter_: (`str`) Filter the Tweets
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: (.types.community.CommunityTweets, list[.types.twDataTypes.Tweet])
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        if isinstance(community_id, Community):
-            community_id = community_id.id
-
-        communityTweets = CommunityTweets(community_id, self, pages, filter_, wait_time, cursor)
-
-        return communityTweets.generator()
-
-    @AuthRequired
-    def get_community_tweets(
-            self,
-            community_id: Union[str, int, Community],
-            pages: int = 1,
-            filter_: str = None,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-
-        """
-         Getting the tweets from a community
-
-        :param: community_id: (`str` | `int` | `Community`) ID of the community whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: filter_: (`str`) Filter the Tweets
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: .types.community.CommunityTweets
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        if isinstance(community_id, Community):
-            community_id = community_id.id
-
-        communityTweets = CommunityTweets(community_id, self, pages, filter_, wait_time, cursor)
-
-        list(communityTweets.generator())
-
-        return communityTweets
-
-    @AuthRequired
-    def get_community_members(
-            self,
-            community_id: Union[str, int, Community],
-            pages: int = 1,
-            filter_: str = None,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-        """
-         Getting the Members from a community
-
-        :param: community_id: (`str` | `int` | `Community`) ID of the community whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: filter_: (`str`) Filter the Members
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: .types.community.CommunityMembers
-        """
-
-        if wait_time is None:
-            wait_time = 0
-
-        if isinstance(community_id, Community):
-            community_id = community_id.id
-
-        communityTweets = CommunityMembers(community_id, self, pages, filter_, wait_time, cursor)
-
-        list(communityTweets.generator())
-
-        return communityTweets
-
-    @AuthRequired
-    def iter_community_members(
-            self,
-            community_id: Union[str, int, Community],
-            pages: int = 1,
-            filter_: str = None,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-        """
-         Getting the Members from a community
-
-        :param: community_id: (`str` | `int` | `Community`) ID of the community whom to get the tweets of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: filter_: (`str`) Filter the Members
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: (.types.community.CommunityMembers, [.types.twDataTypes.User])
-        """
-
-        if wait_time is None:
-            wait_time = 0
-
-        if isinstance(community_id, Community):
-            community_id = community_id.id
-
-        communityTweets = CommunityMembers(community_id, self, pages, filter_, wait_time, cursor)
-
-        return communityTweets.generator()
-
-    @AuthRequired
-    def get_user_followers(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ) -> UserFollowers:
-        """
-         Get the followers of a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the followers of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: .types.follow.UserFollowers
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        if not username:
-            username = self.me.username
-
-        user_id = self._get_user_id(username)
-
-        userFollowers = UserFollowers(user_id, self, pages, wait_time, cursor)
-
-        list(userFollowers.generator())
-
-        return userFollowers
-
-    @AuthRequired
-    def iter_user_followers(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-
-        """
-         Generator for getting the followers from a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the followers of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: (.types.follow.UserFollowers, list[.types.twDataTypes.User])
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        if not username:
-            username = self.me.username
-
-        user_id = self._get_user_id(username)
-
-        userFollowers = UserFollowers(user_id, self, pages, wait_time, cursor)
-
-        return userFollowers.generator()
-
-    @AuthRequired
-    def get_user_followings(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ) -> UserFollowings:
-        """
-         Get the Followings of a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the followings of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: .types.follow.UserFollowings
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        if not username:
-            username = self.me.username
-
-        user_id = self._get_user_id(username)
-
-        userFollowings = UserFollowings(user_id, self, pages, wait_time, cursor)
-
-        list(userFollowings.generator())
-
-        return userFollowings
-
-    @AuthRequired
-    def iter_user_followings(
-            self,
-            username: Union[str, int, User],
-            pages: int = 1,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None
-    ):
-
-        """
-         Generator for getting the followings from a user
-
-        :param: username: (`str` | `int` | `User`) username of the user whom to get the followings of
-        :param: pages: (`int`) number of pages to be scraped
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-
-        :return: (.types.follow.UserFollowings, list[.types.twDataTypes.User])
-        """
-        if wait_time is None:
-            wait_time = 0
-
-        if not username:
-            username = self.me.username
-
-        user_id = self._get_user_id(username)
-
-        userFollowings = UserFollowings(user_id, self, pages, wait_time, cursor)
-
-        return userFollowings.generator()
-
-    @AuthRequired
-    def get_tweet_comments(
-            self,
-            tweet_id: Union[str, Tweet],
-            pages: int = 1,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None,
-            get_hidden: bool = False
-    ):
-        """
-
-        :param: tweet_id: Tweet ID or the Tweet Object of which the Comments to get
-        :param: pages: (`int`) The number of pages to get
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-        :param: get_hidden: (`bool`) get the hidden comments (most likely offensive comments)
-        :return: .types.likes.TweetLikes
-        """
-
-        tweetId = get_tweet_id(tweet_id)
-
-        comments = TweetComments(tweetId, self, get_hidden, pages, wait_time, cursor)
-        list(comments.generator())
-        return comments
-
-    @AuthRequired
-    def iter_tweet_comments(
-            self,
-            tweet_id: Union[str, Tweet],
-            pages: int = 1,
-            wait_time: Union[int, list, tuple] = 2,
-            cursor: str = None,
-            get_hidden: bool = False
-    ):
-        """
-
-        :param: tweet_id: Tweet ID or the Tweet Object of which the Likes to get
-        :param: pages: (`int`) The number of pages to get
-        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
-        :param: cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
-        :param: get_hidden: (`bool`) get the hidden comments (most likely offensive comments)
-
-        :return: (.types.likes.TweetLikes, list[.types.twDataTypes.User])
-        """
-
-        tweetId = get_tweet_id(tweet_id)
-
-        comments = TweetComments(tweetId, self, get_hidden, pages, wait_time, cursor)
-
-        return comments.generator()
-
-    @AuthRequired
-    def tweet_edit_history(self, identifier) -> TweetHistory:
-        """
-        Get Edit History of a Tweet
-
-        :param identifier: (`str`) The unique identifier of the tweet , either the `Tweet id` or `Tweet Link`
-
-        :return: .types.usertweet.TweetHistory
-        """
-
-        tweetId = get_tweet_id(identifier)
-        return TweetHistory(tweetId, self)
-
-    def tweet_detail(self, identifier: str) -> Tweet:
-        """
-        Get Detail of a single tweet
-
-        :param: identifier: (`str`) The unique identifier of the tweet , either the `Tweet id` or `Tweet Link`
-
-        :return: .types.twDataTypes.Tweet
-        """
-
-        tweetId = get_tweet_id(identifier)
-
-        response = self.request.get_tweet_detail(tweetId)
-
-        if self.user is None:
-            if find_objects(response, "tweetResult", None):
-                return Tweet(self, response, response)
-        else:
-            _tweet_before = []
-            entries = find_objects(response, "type", "TimelineAddEntries")
-
-            if not entries or len(entries) == 0:
-                raise InvalidTweetIdentifier(response=response)
-
-            for entry in entries['entries']:
-                if str(entry['entryId']).split("-")[0] == "tweet":
-                    tweet = Tweet(self, entry, response)
-
-                    if str(tweet.id) == str(tweetId):
-                        tweet.threads.extend(_tweet_before)
-                        return tweet
-                    else:
-                        _tweet_before.append(tweet)
-
-        raise InvalidTweetIdentifier(response=response)
-
-    def translate_tweet(self, tweet_id, language):
-        """
-            Translate Tweet in another Language
-
-            :param tweet_id: Tweet ID of the Tweet to be translated
-            :param language: In which Language you want to translate the Tweet (see tweety.filters.Language)
-            :return: .types.twDataTypes.TweetTranslate
-        """
-
-        tweetId = get_tweet_id(tweet_id)
-        language = check_translation_lang(language)
-        response = self.http.get_tweet_translation(tweetId, language)
-        return TweetTranslate(self, response)
-
-    def search_gifs(self, search_term, pages=1, cursor=None, wait_time=2):
-        search = GifSearch(search_term, self, pages, cursor, wait_time)
-        list(search.generator())
-        return search
-
-    def iter_search_gifs(self, search_term, pages=1, cursor=None, wait_time=2):
-        search = GifSearch(search_term, self, pages, cursor, wait_time)
-        return search.generator()
-
-    def search_place(self, lat=None, long=None, search_term=None):
-        """
-        Search Place either using `search_term` , or `latitude` and `longitude`
-
-        :param lat: Latitude of Place
-        :param long: Longitude of Place
-        :param search_term: Search Term of Place
-        :return: .type.places.Places
-        """
-
-        return Places(self, lat, long, search_term)
-
+import warnings
+from typing import Union
+from .utils import (find_objects, AuthRequired, get_user_from_typehead, get_tweet_id, check_translation_lang,
+                    is_tweet_protected)
+from .types import (Proxy, TweetComments, UserTweets, Search, User, Tweet, Trends, Community, CommunityTweets,
+                    CommunityMembers, UserFollowers, UserFollowings, TweetHistory, UserMedia, GifSearch,
+                    ShortUser, TypeHeadSearch, TweetTranslate, AudioSpace, UserHighlights, UserLikes, Places,
+                    UserSubscribers)
+from .exceptions import *
+from .session import Session, MemorySession, FileSession
+from .http import Request
+
+
+class BotMethods:
+    LOGIN_URL = "https://api.twitter.com/1.1/onboarding/task.json?flow_name=login"
+
+    def __init__(self, session_name: Union[str, Session], proxy: Union[dict, Proxy] = None, **httpx_kwargs):
+        """
+        Constructor of the Twitter Public class
+
+        :param: session_name: (`str`, `Session`) This is the name of the session which will be saved and can be loaded later
+        :param: proxy: (`dict` or `Proxy`) Provide the proxy you want to use while making a request
+        """
+
+        self._login_url = self.LOGIN_URL
+        self._username = None
+        self._password = None
+        self._extra = None
+        self._login_flow = None
+        self._login_flow_state = None
+        self._last_json = {}
+        self._cached_users = {}
+        self._proxy = proxy.get_dict() if isinstance(proxy, Proxy) else proxy
+        self._event_builders = []
+
+        if isinstance(session_name, MemorySession):
+            self.session = session_name(self)
+        elif isinstance(session_name, FileSession):
+            self.session = session_name
+        else:
+            self.session = FileSession(self, session_name)
+
+        self.logged_in = False
+        self.is_user_authorized = False
+        self.request = self.http = Request(self, max_retries=10, proxy=self._proxy, **httpx_kwargs)
+        self.user = None
+
+    def get_user_info(self, username: Union[str, int, list] = None):
+        """
+        Get the User Info of the specified username
+
+        :param: username: (`str` | `int` | List[`str`, `int`]) username or user_id to get information of
+
+        :return: .types.twDataTypes.User
+        """
+
+        if not username and self.user is not None:
+            username = self.user.username
+
+        if isinstance(username, list):
+            for i in username:
+                if not str(i).isdigit():
+                    raise ValueError("Only Accept List of User IDs.")
+
+        if isinstance(username, list) or str(username).isdigit() or isinstance(username, int):
+            usernames = [username] if not isinstance(username, list) else username
+            users_raw = self.request.get_users_by_rest_id(usernames)
+            users = find_objects(users_raw, "users", None, recursive=False, none_value=[])
+
+            parsed_users = []
+            for user in users:
+                try:
+                    this_user = User(self, user)
+                    parsed_users.append(this_user)
+                    self._cached_users[str(this_user.username).lower()] = this_user.id
+                except Exception as e:
+                    warnings.warn(f"UsersByRestId Error: {str(e)}")
+
+            if len(usernames) == 1 and len(parsed_users) > 0:
+                return parsed_users[0]
+            elif len(usernames) == 1 and len(parsed_users) == 0:
+                return None
+            elif len(usernames) > 1 and len(parsed_users) == 0:
+                return []
+            else:
+                return parsed_users
+        else:
+            user_raw = self.request.get_user(username)
+            user = User(self, user_raw)
+            self._cached_users[str(username).lower()] = user.id
+            return user
+
+    @property
+    def user_id(self) -> int:
+        """
+        Get the user unique twitter id of authenticated user
+
+        :return: int
+        """
+        return self.user.id if self.user else None
+
+    @property
+    def cache(self):
+        return self._cached_users
+
+    def get_user_id(self, username: str):
+        return self._get_user_id(username)
+
+    def _get_user_id(self, username):
+        if isinstance(username, (User, ShortUser)):
+            user_id = username.id
+        elif isinstance(username, int) or (isinstance(username, str) and str(username).isdigit()):
+            user_id = username
+        elif self._cached_users.get(username.lower()):
+            user_id = self._cached_users[username.lower()]
+        else:
+            user = None
+            try:
+                user = get_user_from_typehead(username, self.typehead_user_search(username))
+            except AuthenticationRequired:
+                # We can only get user using `get_user_info` when unauthenticated
+                pass
+
+            if not user:
+                user = self.get_user_info(username)
+
+            if user:
+                user_id = user.id
+            else:
+                raise UserNotFound()
+        return user_id
+
+    def get_tweets(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            replies: bool = False,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ) -> UserTweets:
+        """
+         Get the tweets from a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: replies: (`boolean`) get the replied tweets of the user too
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: .types.usertweet.UserTweets
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        user_id = self._get_user_id(username)
+
+        userTweets = UserTweets(user_id, self, pages, replies, wait_time, cursor)
+
+        list(userTweets.generator())
+
+        return userTweets
+
+    def iter_tweets(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            replies: bool = False,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+
+        """
+         Generator for getting the tweets from a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: replies: (`boolean`) get the replied tweets of the user too
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: (.types.usertweet.UserTweets, list[.types.twDataTypes.Tweet])
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        user_id = self._get_user_id(username)
+
+        userTweets = UserTweets(user_id, self, pages, replies, wait_time, cursor)
+
+        return userTweets.generator()
+
+    def get_user_highlights(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            replies: bool = False,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+        """
+         Get the tweets from a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: replies: (`boolean`) get the replied tweets of the user too
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: .types.usertweet.userHighlights
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        user_id = self._get_user_id(username)
+
+        userHighlights = UserHighlights(user_id, self, pages, replies, wait_time, cursor)
+
+        list(userHighlights.generator())
+
+        return userHighlights
+
+    def iter_user_highlights(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            replies: bool = False,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+
+        """
+         Generator for getting the tweets from a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: replies: (`boolean`) get the replied tweets of the user too
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: (.types.usertweet.UserHighlights, list[.types.twDataTypes.Tweet])
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        user_id = self._get_user_id(username)
+
+        userHighlights = UserHighlights(user_id, self, pages, replies, wait_time, cursor)
+
+        return userHighlights.generator()
+
+    def get_user_likes(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            replies: bool = False,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+        """
+         Get the liked tweets of a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: replies: (`boolean`) get the replied tweets of the user too
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: .types.usertweet.userLikes
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        user_id = self._get_user_id(username)
+
+        userLikes = UserLikes(user_id, self, pages, replies, wait_time, cursor)
+
+        list(userLikes.generator())
+
+        return userLikes
+
+    def iter_user_likes(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            replies: bool = False,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+
+        """
+         Generator for getting the liked tweets of a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: replies: (`boolean`) get the replied tweets of the user too
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: (.types.usertweet.UserLikes, list[.types.twDataTypes.Tweet])
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        user_id = self._get_user_id(username)
+
+        userLikes = UserLikes(user_id, self, pages, replies, wait_time, cursor)
+
+        return userLikes.generator()
+
+    @AuthRequired
+    def get_user_media(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ) -> UserMedia:
+        """
+         Get the media from a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: .types.usertweet.UserMedia
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        user_id = self._get_user_id(username)
+
+        userMedia = UserMedia(user_id, self, pages, wait_time, cursor)
+
+        list(userMedia.generator())
+
+        return userMedia
+
+    @AuthRequired
+    def iter_user_media(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+
+        """
+         Generator for getting the media from a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: (.types.usertweet.UserMedia, list[.types.twDataTypes.Tweet])
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        user_id = self._get_user_id(username)
+
+        userMedia = UserMedia(user_id, self, pages, wait_time, cursor)
+
+        return userMedia.generator()
+
+    @AuthRequired
+    def get_trends(self):
+        """
+        Get the Trends from you locale
+
+        :return: list of .types.twDataTypes.Trends
+        """
+        trends = []
+        response = self.request.get_trends()
+
+        entries = find_objects(response, "addEntries", None)
+        if not entries or len(entries) == 0:
+            return trends
+
+        for entry in entries['entries']:
+            if str(entry['entryId']) == "trends":
+                for item in entry['content']['timelineModule']['items']:
+                    trends.append(Trends(self, item))
+
+        return trends
+
+    @AuthRequired
+    def search(
+            self,
+            keyword: str,
+            pages: int = 1,
+            filter_: str = None,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ) -> Search:
+
+        """
+        Search for a keyword or hashtag on Twitter
+
+        :param: keyword: (`str`) The keyword which is supposed to be searched
+        :param: pages: (`int`) The number of pages to get
+        :param: filter_: (
+           `str`| `filters.SearchFilters.Users()`| `filters.SearchFilters.Latest()` | `filters.SearchFilters.Photos()` | `filters.SearchFilters.Videos()`
+        )
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+
+        :return: .types.search.Search
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        search = Search(keyword, self, pages, filter_, wait_time, cursor)
+
+        list(search.generator())
+
+        return search
+
+    @AuthRequired
+    def iter_search(
+            self,
+            keyword: str,
+            pages: int = 1,
+            filter_: str = None,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+        """
+        Search for a keyword or hashtag on Twitter
+
+        :param: keyword: (`str`) The keyword which is supposed to be searched
+        :param: pages: (`int`) The number of pages to get
+        :param: filter_: (
+           `str`| `filters.SearchFilters.Users()`| `filters.SearchFilters.Latest()` | `filters.SearchFilters.Photos()` | `filters.SearchFilters.Videos()`
+        )
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+
+        :return: (.types.search.Search, list[.types.twDataTypes.Tweet])
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        search = Search(keyword, self, pages, filter_, wait_time, cursor)
+
+        return search.generator()
+
+    @AuthRequired
+    def typehead_user_search(self, keyword):
+        return TypeHeadSearch(self, keyword, "users")
+
+    @AuthRequired
+    def get_audio_space(self, space_id: Union[str, Tweet]) -> AudioSpace:
+        """
+
+        :param: space_id: ID of the Audio Space , or the Tweet Object that Space Audio is part of.
+        :return: .types.twDataTypes.AudioSpace
+        """
+
+        if isinstance(space_id, Tweet):
+            space_id = space_id.audio_space_id
+
+        space = self.http.get_audio_space(space_id)
+
+        if not find_objects(space, "metadata", None):
+            raise AudioSpaceNotFound(404, "BadRequest", response=space)
+
+        return AudioSpace(self, space)
+
+    @AuthRequired
+    def get_community(self, community_id):
+        """
+
+        :param: community_id: ID of the community to get
+        :return:
+        """
+
+        response = self.http.get_community(community_id)
+        return Community(self, response)
+
+    @AuthRequired
+    def iter_community_tweets(
+            self,
+            community_id: Union[str, int, Community],
+            pages: int = 1,
+            filter_: str = None,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+
+        """
+         Generator for getting the tweets from a community
+
+        :param: community_id: (`str` | `int` | `Community`) ID of the community whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: filter_: (`str`) Filter the Tweets
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: (.types.community.CommunityTweets, list[.types.twDataTypes.Tweet])
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        if isinstance(community_id, Community):
+            community_id = community_id.id
+
+        communityTweets = CommunityTweets(community_id, self, pages, filter_, wait_time, cursor)
+
+        return communityTweets.generator()
+
+    @AuthRequired
+    def get_community_tweets(
+            self,
+            community_id: Union[str, int, Community],
+            pages: int = 1,
+            filter_: str = None,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+
+        """
+         Getting the tweets from a community
+
+        :param: community_id: (`str` | `int` | `Community`) ID of the community whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: filter_: (`str`) Filter the Tweets
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: .types.community.CommunityTweets
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        if isinstance(community_id, Community):
+            community_id = community_id.id
+
+        communityTweets = CommunityTweets(community_id, self, pages, filter_, wait_time, cursor)
+
+        list(communityTweets.generator())
+
+        return communityTweets
+
+    @AuthRequired
+    def get_community_members(
+            self,
+            community_id: Union[str, int, Community],
+            pages: int = 1,
+            filter_: str = None,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+        """
+         Getting the Members from a community
+
+        :param: community_id: (`str` | `int` | `Community`) ID of the community whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: filter_: (`str`) Filter the Members
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: .types.community.CommunityMembers
+        """
+
+        if wait_time is None:
+            wait_time = 0
+
+        if isinstance(community_id, Community):
+            community_id = community_id.id
+
+        communityTweets = CommunityMembers(community_id, self, pages, filter_, wait_time, cursor)
+
+        list(communityTweets.generator())
+
+        return communityTweets
+
+    @AuthRequired
+    def iter_community_members(
+            self,
+            community_id: Union[str, int, Community],
+            pages: int = 1,
+            filter_: str = None,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+        """
+         Getting the Members from a community
+
+        :param: community_id: (`str` | `int` | `Community`) ID of the community whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: filter_: (`str`) Filter the Members
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: (.types.community.CommunityMembers, [.types.twDataTypes.User])
+        """
+
+        if wait_time is None:
+            wait_time = 0
+
+        if isinstance(community_id, Community):
+            community_id = community_id.id
+
+        communityTweets = CommunityMembers(community_id, self, pages, filter_, wait_time, cursor)
+
+        return communityTweets.generator()
+
+    @AuthRequired
+    def get_user_followers(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ) -> UserFollowers:
+        """
+         Get the followers of a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the followers of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: .types.follow.UserFollowers
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        if not username:
+            username = self.me.username
+
+        user_id = self._get_user_id(username)
+
+        userFollowers = UserFollowers(user_id, self, pages, wait_time, cursor)
+
+        list(userFollowers.generator())
+
+        return userFollowers
+
+    @AuthRequired
+    def iter_user_followers(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+
+        """
+         Generator for getting the followers from a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the followers of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: (.types.follow.UserFollowers, list[.types.twDataTypes.User])
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        if not username:
+            username = self.me.username
+
+        user_id = self._get_user_id(username)
+
+        userFollowers = UserFollowers(user_id, self, pages, wait_time, cursor)
+
+        return userFollowers.generator()
+
+    @AuthRequired
+    def get_user_followings(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ) -> UserFollowings:
+        """
+         Get the Followings of a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the followings of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: .types.follow.UserFollowings
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        if not username:
+            username = self.me.username
+
+        user_id = self._get_user_id(username)
+
+        userFollowings = UserFollowings(user_id, self, pages, wait_time, cursor)
+
+        list(userFollowings.generator())
+
+        return userFollowings
+
+    @AuthRequired
+    def iter_user_followings(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+
+        """
+         Generator for getting the followings from a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the followings of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: (.types.follow.UserFollowings, list[.types.twDataTypes.User])
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        if not username:
+            username = self.me.username
+
+        user_id = self._get_user_id(username)
+
+        userFollowings = UserFollowings(user_id, self, pages, wait_time, cursor)
+
+        return userFollowings.generator()
+
+    @AuthRequired
+    def get_user_subscribers(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ) -> UserFollowings:
+        """
+         Get the Subscribers of a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the followings of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: .types.follow.UserSubscribers
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        if not username:
+            username = self.me.username
+
+        user_id = self._get_user_id(username)
+
+        userSubscribers = UserSubscribers(user_id, self, pages, wait_time, cursor)
+
+        list(userSubscribers.generator())
+
+        return userSubscribers
+
+    @AuthRequired
+    def iter_user_subscribers(
+            self,
+            username: Union[str, int, User],
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None
+    ):
+
+        """
+         Generator for getting the Subscribers from a user
+
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the followings of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+
+        :return: (.types.follow.UserSubscribers, list[.types.twDataTypes.User])
+        """
+        if wait_time is None:
+            wait_time = 0
+
+        if not username:
+            username = self.me.username
+
+        user_id = self._get_user_id(username)
+
+        userSubscribers = UserSubscribers(user_id, self, pages, wait_time, cursor)
+
+        return userSubscribers.generator()
+
+    @AuthRequired
+    def get_tweet_comments(
+            self,
+            tweet_id: Union[str, Tweet],
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None,
+            get_hidden: bool = False
+    ):
+        """
+
+        :param: tweet_id: Tweet ID or the Tweet Object of which the Comments to get
+        :param: pages: (`int`) The number of pages to get
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+        :param: get_hidden: (`bool`) get the hidden comments (most likely offensive comments)
+        :return: .types.likes.TweetLikes
+        """
+
+        tweetId = get_tweet_id(tweet_id)
+
+        comments = TweetComments(tweetId, self, get_hidden, pages, wait_time, cursor)
+        list(comments.generator())
+        return comments
+
+    @AuthRequired
+    def iter_tweet_comments(
+            self,
+            tweet_id: Union[str, Tweet],
+            pages: int = 1,
+            wait_time: Union[int, list, tuple] = 2,
+            cursor: str = None,
+            get_hidden: bool = False
+    ):
+        """
+
+        :param: tweet_id: Tweet ID or the Tweet Object of which the Likes to get
+        :param: pages: (`int`) The number of pages to get
+        :param: wait_time: (`int`, `list`, `tuple`) seconds to wait between multiple requests
+        :param: cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+        :param: get_hidden: (`bool`) get the hidden comments (most likely offensive comments)
+
+        :return: (.types.likes.TweetLikes, list[.types.twDataTypes.User])
+        """
+
+        tweetId = get_tweet_id(tweet_id)
+
+        comments = TweetComments(tweetId, self, get_hidden, pages, wait_time, cursor)
+
+        return comments.generator()
+
+    @AuthRequired
+    def tweet_edit_history(self, identifier) -> TweetHistory:
+        """
+        Get Edit History of a Tweet
+
+        :param identifier: (`str`) The unique identifier of the tweet , either the `Tweet id` or `Tweet Link`
+
+        :return: .types.usertweet.TweetHistory
+        """
+
+        tweetId = get_tweet_id(identifier)
+        return TweetHistory(tweetId, self)
+
+    def tweet_detail(self, identifier: str) -> Tweet:
+        """
+        Get Detail of a single tweet
+
+        :param: identifier: (`str`) The unique identifier of the tweet , either the `Tweet id` or `Tweet Link`
+
+        :return: .types.twDataTypes.Tweet
+        """
+
+        tweetId = get_tweet_id(identifier)
+
+        response = self.request.get_tweet_detail(tweetId)
+
+        if self.user is None:
+            if find_objects(response, "tweetResult", None):
+                return Tweet(self, response, response)
+        else:
+            _tweet_before = []
+            entries = find_objects(response, "type", "TimelineAddEntries")
+
+            if not entries or len(entries) == 0:
+                raise InvalidTweetIdentifier(response=response)
+
+            for entry in entries['entries']:
+                if str(entry['entryId']).split("-")[0] == "tweet":
+                    # ignore these protected tweets that are not what we are looking for
+                    # otherwise it will throw exception
+                    if not (is_tweet_protected(entry) and str(entry['entryId'].split("-")[1]) != str(tweetId)):
+                        tweet = Tweet(self, entry, response)
+
+                        if str(tweet.id) == str(tweetId):
+                            tweet.threads.extend(_tweet_before)
+                            return tweet
+                        else:
+                            _tweet_before.append(tweet)
+
+        raise InvalidTweetIdentifier(response=response)
+
+    def translate_tweet(self, tweet_id, language):
+        """
+            Translate Tweet in another Language
+
+            :param tweet_id: Tweet ID of the Tweet to be translated
+            :param language: In which Language you want to translate the Tweet (see tweety.filters.Language)
+            :return: .types.twDataTypes.TweetTranslate
+        """
+
+        tweetId = get_tweet_id(tweet_id)
+        language = check_translation_lang(language)
+        response = self.http.get_tweet_translation(tweetId, language)
+        return TweetTranslate(self, response)
+
+    def search_gifs(self, search_term, pages=1, cursor=None, wait_time=2):
+        search = GifSearch(search_term, self, pages, cursor, wait_time)
+        list(search.generator())
+        return search
+
+    def iter_search_gifs(self, search_term, pages=1, cursor=None, wait_time=2):
+        search = GifSearch(search_term, self, pages, cursor, wait_time)
+        return search.generator()
+
+    def search_place(self, lat=None, long=None, search_term=None):
+        """
+        Search Place either using `search_term` , or `latitude` and `longitude`
+
+        :param lat: Latitude of Place
+        :param long: Longitude of Place
+        :param search_term: Search Term of Place
+        :return: .type.places.Places
+        """
+
+        return Places(self, lat, long, search_term)
+
```

### Comparing `tweety_ns-1.1.5/src/tweety/builder.py` & `tweety_ns-1.1.6/src/tweety/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import urllib
 from urllib.parse import urlencode
 import random
-from .exceptions_ import DeniedLogin
 from functools import wraps
+from .exceptions import DeniedLogin
 from . import utils
-from .types import HOME_TIMELINE_TYPE_FOR_YOU, HOME_TIMELINE_TYPE_FOLLOWING
+from .types import HOME_TIMELINE_TYPE_FOR_YOU
 
 REQUEST_USER_AGENT = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36'
 REQUEST_PLATFORMS = ['Linux', 'Windows']
 
 
 def return_with_headers(func):
     @wraps(func)
@@ -96,14 +96,15 @@
     URL_AUSER_GET_LIST_TWEETS = "https://twitter.com/i/api/graphql/TXyJ3x6-VnEbkV09UzebUQ/ListLatestTweetsTimeline"  # noqa
     URL_AUSER_ADD_LIST_MEMBER = "https://twitter.com/i/api/graphql/sw71TVciw1b2nRwV6eDZNA/ListAddMember"  # noqa
     URL_AUSER_DELETE_LIST_MEMBER = "https://twitter.com/i/api/graphql/kHdBGndqf_JX3ef1T1931A/ListRemoveMember"  # noqa
     URL_AUSER_CREATE_LIST = "https://twitter.com/i/api/graphql/nHFMQuE4PMED1R0JTN4d-Q/CreateList"  # noqa
     URL_AUSER_DELETE_LIST = "https://twitter.com/i/api/graphql/UnN9Th1BDbeLjpgjGSpL3Q/DeleteList"  # noqa
     URL_AUSER_GET_USER_FOLLOWERS = "https://twitter.com/i/api/graphql/ihMPm0x-pC35X86L_nUp_Q/Followers"  # noqa
     URL_AUSER_GET_USER_FOLLOWINGS = "https://twitter.com/i/api/graphql/bX-gXhcglOa--1gzgDlb8A/Following"  # noqa
+    URL_AUSER_GET_USER_SUBSCRIBERS = "https://twitter.com/i/api/graphql/NHT8e7FjnCS3TP0QfP_OUQ/UserCreatorSubscriptions"  # noqa
     # URL_AUSER_GET_MUTUAL_FRIENDS = "https://twitter.com/i/api/1.1/friends/following/list.json"  # noqa
     URL_AUSER_GET_MUTUAL_FRIENDS = "https://twitter.com/i/api/graphql/35Y2QFmL84HIisnm-FHAng/FollowersYouKnow"  # noqa
     URL_AUSER_GET_BLOCKED_USERS = "https://twitter.com/i/api/graphql/f87G4V_l5E9rJ-Ylw0D-yQ/BlockedAccountsAll"  # noqa
     URL_PIN_TWEET = "https://twitter.com/i/api/graphql/VIHsNu89pK-kW35JpHq7Xw/PinTweet"  # noqa
 
     def __init__(self):
         self.cookies = None
@@ -1440,14 +1441,43 @@
         if cursor:
             variables['cursor'] = cursor
 
         params = {'variables': str(json.dumps(variables)), 'features': str(json.dumps(features))}
         return "GET", self._build(self.URL_AUSER_GET_USER_FOLLOWINGS, urlencode(params))
 
     @return_with_headers
+    def get_user_subscribers(self, user_id, cursor=None):
+        variables = {"userId": str(user_id), "count": 20, "includePromotedContent": False}
+        features = {"rweb_tipjar_consumption_enabled": True, "responsive_web_graphql_exclude_directive_enabled": True,
+                    "verified_phone_label_enabled": False, "creator_subscriptions_tweet_preview_api_enabled": True,
+                    "responsive_web_graphql_timeline_navigation_enabled": True,
+                    "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
+                    "communities_web_enable_tweet_community_results_fetch": True,
+                    "c9s_tweet_anatomy_moderator_badge_enabled": True, "articles_preview_enabled": True,
+                    "tweetypie_unmention_optimization_enabled": True, "responsive_web_edit_tweet_api_enabled": True,
+                    "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
+                    "view_counts_everywhere_api_enabled": True,
+                    "longform_notetweets_consumption_enabled": True,
+                    "responsive_web_twitter_article_tweet_consumption_enabled": True,
+                    "tweet_awards_web_tipping_enabled": False,
+                    "creator_subscriptions_quote_tweet_preview_enabled": False,
+                    "freedom_of_speech_not_reach_fetch_enabled": True,
+                    "standardized_nudges_misinfo": True,
+                    "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": True,
+                    "tweet_with_visibility_results_prefer_gql_media_interstitial_enabled": True,
+                    "rweb_video_timestamps_enabled": True, "longform_notetweets_rich_text_read_enabled": True,
+                    "longform_notetweets_inline_media_enabled": True, "responsive_web_enhance_cards_enabled": False}
+
+        if cursor:
+            variables['cursor'] = cursor
+
+        params = {'variables': str(json.dumps(variables)), 'features': str(json.dumps(features))}
+        return "GET", self._build(self.URL_AUSER_GET_USER_SUBSCRIBERS, urlencode(params))
+
+    @return_with_headers
     def get_community(self, community_id):
         variables = {"communityId": community_id, "withDmMuting": False, "withSafetyModeUserFields": False}
         features = {"responsive_web_graphql_exclude_directive_enabled": True,
                     "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
                     "responsive_web_graphql_timeline_navigation_enabled": True, "verified_phone_label_enabled": False}
 
         params = {'variables': str(json.dumps(variables)), 'features': str(json.dumps(features))}
```

### Comparing `tweety_ns-1.1.5/src/tweety/events/newmessage.py` & `tweety_ns-1.1.6/src/tweety/events/newmessage.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.5/src/tweety/exceptions_.py` & `tweety_ns-1.1.6/src/tweety/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,207 +1,219 @@
-
-TWITTER_ERRORS = {0: 'DefaultApiError', 3: 'InvalidCoordinates', 4: 'InvalidGranularity', 5: 'InvalidAccuracy', 6: 'NoDataForPoint', 7: 'NoDataForPointRadius', 8: 'InvalidId', 9: 'InvalidMaxResults', 10: 'RockdoveError', 11: 'InvalidIp', 12: 'MustProvideCoordinatesIpQueryOrAttributes', 13: 'NoLocationForIp', 14: 'OverlimitAddressBookApi', 15: 'AddressBookDarkmoded', 16: 'AddressBookPermissionsError', 17: 'AddressBookLookupNotFound', 18: 'TooManyTerms', 19: 'RetweetDarkmoded', 20: 'NoScreenNameProvided', 21: 'ContributorsNotEnabled', 22: 'NotAuthorizedToViewUser', 23: 'BulkLookupDarkmoded', 24: 'UnsupportedProfileImageSize', 25: 'MissingQuery', 26: 'AutocompleteMustBeTrueOrFalse', 27: 'AccountLocked', 28: 'GenericDarkmode', 29: 'TimeOut', 30: 'WoeidDataUnavailable', 31: 'InvalidTimescale', 32: 'InvalidCredentials', 33: 'OverLimit', 34: 'GenericNotFound', 35: 'TrendDataUnavailable', 36: 'CantReportYourselfAsSpam', 37: 'GenericAccessDenied', 38: 'MissingParameter', 39: 'InvalidCreationToken', 41: 'RockdoveInvalidArgumentError', 42: 'InvalidAttribute', 43: 'AttributeAccessDenied', 44: 'InvalidParameter', 46: 'InvalidPlaceJson', 47: 'InvalidRequestUrl', 48: 'TimeoutRequestRainbird', 49: 'NoFollowRequest', 50: 'GenericUserNotFound', 51: 'PromotedContentOfflineError', 52: 'PromotedSearchNoQuery', 53: 'BasicAuthDisabled', 54: 'CassowaryError', 55: 'ResourceNotFound', 56: 'InvalidEmailAddress', 57: 'PasswordResetPermissionsError', 58: 'PasswordResetExpiredToken', 59: 'PasswordResetInvalidHash', 60: 'PasswordResetMismatchedEntries', 61: 'ClientNotPermitted', 62: 'CustomSaveErrors', 63: 'OtherUserSuspended', 64: 'CurrentUserSuspended', 65: 'StrictMustBeTrueOrFalse', 66: 'RequireActivityMustBeTrueOrFalse', 67: 'BackendServiceUnavailable', 68: 'EndpointDeprecated', 69: 'TalonUrlMalware', 70: 'InvalidPromotedContentLogEvent', 71: 'EmailDeliveryError', 72: 'ApplicationNotFound', 73: 'ApplicationNotDeleted', 74: 'ApplicationDomainNotRevoked', 75: 'ApplicationKeysNotReset', 76: 'ApplicationImageNotProcessed', 77: 'ApplicationNoManageRight', 78: 'ApplicationNoAdminRight', 79: 'InvalidTrimPlace', 80: 'CurationDarkmoded', 81: 'ContributorsAccessLevelNotValid', 82: 'ContributorsTargetUserNotSpecified', 83: 'ContributorsTargetUserNotValid', 84: 'TalonUrlUnrenderable', 85: 'ValidationFailure', 86: 'WrongHttpMethod', 87: 'ClientNotPrivileged', 88: 'RateLimitExceeded', 89: 'BadOauthToken', 90: 'ContributionNotPermitted', 91: 'InvalidUtf8', 92: 'SslRequired', 93: 'DmAccessRequired', 94: 'PageIsForbidden', 95: 'InvalidLanguage', 96: 'InvalidIds', 97: 'EndpointFeatureDeprecated', 98: 'FlagPossiblySensitiveScribeError', 99: 'AuthenticityTokenError', 100: 'GenericThriftException', 101: 'InvalidReverseAuthCredentials', 102: 'DarkmodedFeature', 103: 'TrendsAvailableTransientException', 104: 'ListAdminRightsError', 105: 'MaximumMembersExceeded', 106: 'AddBlockedUserError', 107: 'NoTargetUser', 108: 'TargetUserNotFound', 109: 'TargetUserNotRelatedToList', 110: 'ListNotAMemberError', 111: 'TargetUserSuspended', 112: 'InsufficientListParameters', 113: 'InsufficientTargetUserParameters', 114: 'InvalidCurrentPassword', 115: 'ListUnauthorizedSubscriptionError', 116: 'PasswordSmsResetPwSeedNotExist', 117: 'PasswordSmsResetOptOut', 118: 'ArgumentTooLarge', 119: 'NarrowcastNotSupported', 120: 'AccountUpdateFailure', 121: 'InvalidHexColor', 122: 'UpdateProfileColorsError', 123: 'ImageUpdateError', 124: 'AttributeUpdateError', 125: 'GeolocationError', 126: 'LoggedOut', 127: 'ArchiveDeprecated', 128: 'LocationUpdateFailure', 129: 'EmailRateLimitExceeded', 130: 'OverCapacity', 131: 'InternalError', 132: 'UnusedBackgroundUploadError', 133: 'NoSelectedBackgroundError', 134: 'TooManyDevices', 135: 'OauthTimestampException', 136: 'BlockedUserError', 137: 'PushForbidden', 138: 'FollowingInformationUnavailable', 139: 'DuplicateFavorite', 140: 'FollowingStatusUnauthorized', 141: 'InactiveUser', 142: 'ProtectedStatusFavoriteError', 143: 'FavoriteRateLimitExceeded', 144: 'StatusNotFound', 145: 'RecordInvalid', 146: 'OtherUserNotBlocked', 147: 'SelfBlockError', 148: 'UnsupportedDevice', 149: 'InvalidEnabledFor', 150: 'DirectMessageOtherUserNotFollowing', 151: 'MessageSendError', 152: 'DirectMessageDestroyPermissionsError', 153: 'DirectMessageDeleteError', 154: 'DirectMessageNotFound', 155: 'MessageSendUnknownError', 156: 'DowntimeAlert', 157: 'VerifiedDeviceNotFound', 158: 'SelfFollowError', 159: 'GenericSuspended', 160: 'DuplicateFollowRequest', 161: 'FollowRateLimitExceeded', 162: 'FollowBlockedUserError', 163: 'IndeterminateSource', 164: 'TargetUserNotSpecified', 165: 'MultipleMissingParameters', 166: 'MultipleUserNotFound', 167: 'FollowError', 168: 'StatusNotFoundForbidden', 169: 'StatusRelatedResultsForbidden', 170: 'ForbiddenMissingParameter', 171: 'SearchDeletionError', 172: 'SearchCreationError', 173: 'ConfirmEmailExpiredCode', 174: 'ConfirmEmailInvalidCode', 175: 'ConfirmEmailInvalidStateChange', 176: 'ConfirmEmailAlreadyConfirmed', 177: 'ConfirmEmailSuccessChanged', 178: 'ConfirmEmailSuccessNew', 179: 'StatusViewForbidden', 180: 'GenericEndpointOffline', 181: 'TimeParameterOrderError', 182: 'ParameterDeprecated', 183: 'StatusActionPermissionError', 184: 'StatusUpdateError', 185: 'OverStatusUpdateLimit', 186: 'StatusTooLongError', 187: 'DuplicateStatusError', 188: 'StatusMalwareError', 189: 'StatusCreationError', 190: 'UnknownInterpreterError', 191: 'OverPhotoLimit', 192: 'OverMediaEntitiesPerUpdateLimit', 193: 'MediaTooLarge', 194: 'StatusUpdateForbidden', 195: 'InvalidRequestUrlForbidden', 196: 'TimelineAuthorizationRequired', 197: 'CategoryNotFound', 198: 'ContactLoadError', 199: 'IdsOfContactsError', 200: 'GenericForbidden', 201: 'GetRequired', 202: 'InternalApplicationAuthenticationDenied', 203: 'DeviceError', 204: 'DestinationError', 205: 'SpamRateLimitExceeded', 206: 'InvalidDeviceRelationship', 207: 'AlreadyActivated', 208: 'FormatNotSupported', 209: 'DirectMessageMustFollowFirst', 210: 'TokenLimitExceeded', 211: 'InvalidBrandBanner', 212: 'ProfileBannerUploadsDisabled', 213: 'ProcessingInProgress', 214: 'GenericBadRequest', 215: 'BadAuthenticationData', 216: 'ShareViaEmailRateLimitExceeded', 217: 'ProtectedStatusShareViaEmailError', 218: 'RestrictedAccessShareViaEmailError', 219: 'ShareViaEmailIpRateLimitExceeded', 220: 'RestrictedAuthToken', 221: 'CursorInvalid', 222: 'TieredActionSignupSpammer', 223: 'EmailTweetSendingError', 224: 'MissingEmailAddress', 225: 'TieredActionFollowSpammer', 226: 'TieredActionTweetSpammer', 227: 'TieredActionFollowCreeper', 228: 'TieredActionTweetCreeper', 229: 'AmbiguousCredentials', 230: 'UserSleeping', 231: 'RequiresLoginVerification', 232: 'CannotEnableLoginVerificationPhone', 233: 'CannotEnableLoginVerificationAlreadyEnabled', 234: 'CannotEnableLoginVerificationUnconfirmedEmail', 235: 'ExpiredLoginVerificationRequest', 236: 'IncorrectChallengeResponse', 237: 'MissingLoginVerificationRequest', 238: 'NewPasswordWeak', 239: 'BadGuestToken', 240: 'TieredActionSignupSpammerPhoneVerify', 241: 'RejectedLoginVerificationRequest', 242: 'DeactivatedUser', 243: 'OverLimitLogin', 244: 'ForcePasswordReset', 245: 'OverLimitLoginVerificationStart', 246: 'OverLimitLoginVerificationAttempt', 247: 'CannotEnableLoginVerificationPush', 248: 'LoginVerificationAlreadyEnabled', 249: 'CloudIpRestricted', 250: 'UserMustBeAlcoholAgeScreened', 251: 'EndpointRetired', 252: 'DmSpamTimeout', 253: 'NotYetApprovedLoginVerification', 254: 'OfflineCodeSync', 255: 'RequiresTemporaryPassword', 256: 'CannotFollowFromCountry', 257: 'BadDeviceToken', 258: 'AppsCreateRequiresConfirmedEmail', 259: 'AppsCreateRequiresVerifiedPhone', 260: 'AppsCreateRejectedForAbuse', 261: 'AppInReadOnlyMode', 262: 'CurrentUserNeedsPhoneVerification', 263: 'TieredActionChallengeCaptcha', 264: 'TargetUserNotFollowing', 265: 'TargetUserNotFavoriteFollowing', 266: 'FailureSendingLoginVerificationRequest', 267: 'InvalidCredentialsOneFactorEligible', 268: 'MissingOneFactorLoginVerificationParams', 269: 'UserIsNotSdkUser', 270: 'AppsUpdateSettingsRequiresVerifiedPhone', 271: 'SelfMuteError', 272: 'NotMutingTargetUser', 273: 'ScheduledInPast', 274: 'ScheduledTooFarInFuture', 275: 'TooLateToEdit', 276: 'ScheduleInvalid', 277: 'DirectMessageRecipientDoesNotFollowSenderWithUnverifiedPhoneNumber', 278: 'DirectMessageUserNotInConversation', 279: 'DirectMessageConversationNotFound', 280: 'DirectMessageTooManyParticipants', 281: 'DirectMessageTooFewParticipants', 282: 'DirectMessageRecipientBlocksSender', 283: 'TieredActionFavoriteSpammer', 284: 'DeviceRegistrationGeneralError', 285: 'DeviceAlreadyRegistered', 286: 'DeviceOperatorUnsupported', 287: 'UserAlreadyHasVerifiedPhone', 288: 'CannotReuseCurrentPassword', 289: 'DevicePinInvalid', 290: 'DevicePinRequired', 291: 'UnexpectedDeviceProvided', 292: 'TieredActionConversationSpammer', 293: 'SmsVerifyGeneralError', 294: 'SmsVerifyInvalidPin', 295: 'SmsVerifyRateLimitExceeded', 296: 'DtabOverrideDarkmoded', 297: 'DirectMessageCannotHaveBothTweetAndMedia', 298: 'DirectMessageTweetNotFound', 299: 'DeviceRegistrationRateExceeded', 300: 'DeviceRegistrationInvalidInput', 301: 'DeviceRegistrationPending', 302: 'DeviceRegistrationOperationFailed', 303: 'DeviceRegistrationPhoneNormalizationFailed', 304: 'DeviceRegistrationPhoneCountryDetectionFailed', 305: 'CannotIdentifyByEmail', 306: 'TieredActionAccessTokenGrantSpam', 307: 'TieredActionAccessTokenRevokeSpam', 308: 'NoSmsVerifyExists', 309: 'DeviceNotVerified', 310: 'ExpiredPin', 311: 'DirectMessageDuplicate', 312: 'LocationNameMustBeSpecified', 313: 'EULANotAccepted', 314: 'VideoTranscodingError', 315: 'ClientCaptchaRequired', 316: 'CannotContributeToYourself', 317: 'AccountHasTooManyContributors', 318: 'AccountHasTooManyContributees', 319: 'CannotChangePassword', 320: 'ContributorsAccessLevelInsufficient', 321: 'DirectMessageConversationNameTooLong', 322: 'DirectMessageGenericUserCouldNotBeAdded', 323: 'AnimatedGifMultipleImages', 324: 'InvalidMediaId', 325: 'MediaNotFound', 326: 'AccessDeniedByBouncer', 327: 'AlreadyRetweeted', 328: 'InvalidRetweetForStatus', 329: 'NonsupportingClientRequiresLoginVerification', 330: 'ContributorsGenericUserCouldNotBeAdded', 331: 'MobileSettingsUserNotFound', 332: 'MobileSettingsTemplateNotFound', 333: 'MobileSettingsFileNotFound', 334: 'MobileSettingsUnsupportedTransport', 335: 'MobileSettingsSettingNotFound', 336: 'MobileSettingsInvalidValueFound', 337: 'MobileSettingsSettingObjectNotFound', 338: 'MobileSettingsEnabledForMissing', 339: 'MobileSettingsNoDevicesFound', 340: 'MobileSettingsNoIncomingPushSettings', 341: 'MobileSettingsNoIncomingSmsSettings', 342: 'MobileSettingsIncorrectApplicationId', 343: 'MobileSettingsNoIncomingSettings', 344: 'UserActionRateLimitExceeded', 345: 'OneFactorMethodIsNotSupported', 346: 'UserIsNotOneFactorEligible', 347: 'InvalidRequestToken', 348: 'ClientApplicationNotPermitted', 349: 'DirectMessageCannotDmOtherUser', 350: 'OauthException', 351: 'MobileSettingsCouldNotUpdateSleep', 352: 'ParameterLimitExceeded', 353: 'DeniedByApiCsrfProtection', 354: 'DirectMessageTooLongError', 355: 'GenericConflict', 356: 'GenericValidationFailure', 357: 'RequiredFieldMissing', 358: 'JsonProcessingError', 359: 'ValueTooLarge', 360: 'ValueTooSmall', 361: 'ValueCannotBeEmpty', 362: 'TimeNotFuture', 363: 'InvalidCountryCodes', 364: 'InvalidTimeGranularity', 365: 'InvalidUUID', 366: 'InvalidValues', 367: 'SizeOutOfRange', 368: 'TimeNotPast', 369: 'InvalidJsonSyntax', 370: 'DigitsCannotReuseCurrentEmail', 371: 'MentionLimitInTweetExceeded', 372: 'UrlLimitInTweetExceeded', 373: 'HashtagLimitInTweetExceeded', 374: 'ExpiredQrCode', 375: 'InvalidQrCode', 376: 'MissingCredentials', 377: 'TokenRetrievalException', 378: 'TokenMissing', 379: 'DataminrUserNotLinked', 380: 'ABLiveSyncIsDisabled', 381: 'SoftUserCreationSpamDenied', 382: 'SoftUserActionSpamDenied', 383: 'CashtagLimitInTweetExceeded', 384: 'HashtagLengthLimitInTweetExceeded', 385: 'InReplyToTweetNotFound', 386: 'AttachmentTypesLimitInTweetExceeded', 387: 'NotEnoughFollowers', 388: 'FeatureAccessLimited', 389: 'DirectMessagesSenderBlocksRecipient', 390: 'SearchRecordingNotFound', 391: 'MaximumSearchRecordingsExceeded', 392: 'SessionNotFound', 393: 'SessionModificationNotAuthorized', 394: 'SessionModificationFailed', 395: 'VoiceVerifyRateLimitExceeded', 396: 'BlockUserFailed', 397: 'InvalidMetricsJson', 398: 'OnboardingFlowFailure', 399: 'OnboardingFlowRetriableFailure', 400: 'NoTwoFactorAuthMethodFound', 401: 'MomentCapsuleAccessError', 402: 'CannotEnrollLoginVerificationNotYetEnabled', 403: 'IneligibleFor2faAfterModification', 404: 'CookiesRequired', 405: 'DuplicateBookmark', 406: 'ProtectedTweetBookmarkError', 407: 'DirectMessageInactiveDevice', 408: 'InvalidUrl', 409: 'BirthdateRequired', 410: 'PasswordVerificationRequired', 411: 'DirectMessageSenderInSecretDmsDisabledCountry', 412: 'DirectMessageRecipientInSecretDmsDisabledCountry', 413: 'DirectMessageSenderDeviceIsNotActiveForSecretDms', 414: 'DirectMessageRecipientDeviceIsNotActiveForSecretDms', 415: 'CallbackUrlLocked', 416: 'InvalidOrSuspendedApp', 417: 'InvalidDesktopCallback', 418: 'DirectMessageSenderIsNotRegisteredForSecretDms', 419: 'DirectMessageRecipientIsNotRegisteredForSecretDms', 420: 'ReservedErrorCode', 421: 'TweetIsBounced', 422: 'TweetIsBounceDeleted', 423: 'InvalidHeaders', 424: 'MomentUnavailableForNewsCamera', 425: 'TweetEngagementsLimited', 426: 'InvalidRequestIpv6Token', 427: 'IpResolverNotAvailable', 428: 'ValidIpv6TokenRequired', 429: 'HarmfulLink', 430: 'ConversationControlNotAllowed', 431: 'ConversationControlNotSupported', 432: 'ConversationControlNotAuthorized', 433: 'ConversationControlReplyRestricted', 434: 'NotMutingTargetList', 435: 'ConversationControlInvalidParameter', 436: 'PassswordRequiredForEmailUpdate', 437: 'NewPasswordShort', 438: 'NewPasswordLong', 439: 'NudgeReceived', 440: 'CommunityUserNotAuthorized', 441: 'CommunityNotFound', 442: 'CommunityRetweetNotAllowed', 443: 'CommunityInvalidParams', 444: 'CommunityReplyTweetNotAllowed', 445: 'RestrictedSession', 446: 'TokenSecurityLevelAgreementPolicyFailure', 447: 'SuperFollowsCreateNotAuthorized', 448: 'SuperFollowsInvalidParams', 449: 'TOOMomentsList', 450: 'CommunityProtectedUserCannotTweet', 451: 'ExclusiveTweetEngagementNotAllowed', 452: 'SteamCreationException', 453: 'V11Restricted', 454: 'SteamGetException', 455: 'TrustedFriendsInvalidParams', 456: 'TrustedFriendsRetweetNotAllowed', 457: 'TrustedFriendsEngagementNotAllowed', 458: 'CollabTweetInvalidParams', 459: 'TrustedFriendsCreateNotAllowed', 460: 'TrustedFriendsQuoteTweetNotAllowed', 461: 'StaleTweetEngagementNotAllowed', 462: 'StaleTweetQuoteTweetNotAllowed', 463: 'RetweetIdBookmarkError', 464: 'FieldEditNotAllowed', 465: 'StaleTweetRetweetNotAllowed', 466: 'NotEligibleForEdit', 467: 'V11TierRestricted', 468: 'DirectMessageUnregisteredDevice', 469: 'DirectMessageSenderIsNotBlueVerifiedForSecretDms', 470: 'DirectMessageRecipientIsNotBlueVerifiedForSecretDms', 471: 'ConversationKeysNotProvidedForNewSecretConversation', 472: 'ConversationKeysProvidedForExistingSecretConvo', 473: 'InvalidConversationKeysProvidedForNewSecretConvo', 474: 'DirectMessageReplyNotInConversation', 475: 'DirectMessageConversationMetadataNotFound', 476: 'DirectMessageSenderIsNotVerifiedForMessageRequests', 477: 'DirectMessageSenderIsNotVerifiedRateLimited'}
-
-
-class TwitterError(Exception):
-    """
-        Base Exception raised when error Occurs.
-
-        Attributes:
-            message -- explanation of the error
-    """
-
-    def __init__(
-            self,
-            error_code,
-            error_name,
-            response,
-            message
-    ):
-        self.message = message
-        self.error_code = error_code
-        self.error_name = error_name
-        self.response = response
-
-        if self.response is not None and not isinstance(self.response, dict) and not self.response.json() and self.response.text:
-            self.message = self.response.text
-        elif str(self.error_code) == "404":
-            self.message = "Page not Found. Most likely you need elevated authorization to access this resource"
-
-        super().__init__(self.message)
-
-
-class UserNotFound(TwitterError):
-    """Exception raised when user isn't found.
-
-    Attributes:
-        message -- explanation of the error
-    """
-
-    def __init__(self, error_code=50, error_name="GenericUserNotFound", response=None, message="The User Account wasn't Found or is Protected", **kw):
-        super().__init__(error_code, error_name, response, message)
-
-
-class GuestTokenNotFound(TwitterError):
-    """
-    Exception Raised when the guest token wasn't found after specific number of retires
-
-    Attributes:
-        message -- explanation of the error
-    """
-
-    def __init__(self, error_code=404, error_name="GuestTokenNotFound", response=None, message="The Guest Token couldn't be obtained", **kw):
-        super().__init__(error_code, error_name, response, message)
-
-
-class InvalidTweetIdentifier(TwitterError):
-    """
-        Exception Raised when the tweet identifier is invalid
-
-        Attributes:
-            message -- explanation of the error
-    """
-
-    def __init__(self, error_code=144, error_name="StatusNotFound", response=None, message="The Tweet Identifier is Invalid", **kw):
-        super().__init__(error_code, error_name, response, message)
-
-
-class RateLimitReached(TwitterError):
-    """
-        Exception Raised when the tweet identifier is invalid
-
-        Attributes:
-            message -- explanation of the error
-    """
-
-    def __init__(self, error_code, error_name, response, message="You have exceeded the Twitter Rate Limit", **kw):
-        super().__init__(error_code, error_name, response, message)
-        self.retry_after = kw.get('retry_after')  # Number of seconds required for rate limit to be reset
-
-
-class ProxyParseError(TwitterError):
-    """
-    Exception Raised when an error occurs while parsing the provided proxy
-
-    Attributes:
-        message -- explanation of the error
-    """
-
-    def __init__(self, message="Error while parsing the Proxy, please make sure you are passing the right formatted proxy", **kw):
-        super().__init__(0, "ProxyParseError", None, message)
-
-
-class UserProtected(TwitterError):
-    """
-    Exception Raised when an error occurs when the queried User isn't available / Protected
-
-    Attributes:
-        message -- explanation of the error
-    """
-
-    def __init__(self, error_code=403, error_name="UserUnavailable", response=None, message=None, **kw):
-
-        if not message:
-            message = "The User is Protected OR Unavailable, please make sure you are authenticated and authorized"
-
-        super().__init__(error_code, error_name, response, message)
-
-
-class DeniedLogin(TwitterError):
-    """
-        Exception Raised when the Twitter deny the login request ,
-        could be due to multiple login attempts (or failed attempts)
-
-        Attributes:
-            message -- explanation of the error
-    """
-
-    def __init__(self, error_code=37, error_name="GenericAccessDenied", response=None, message=None, **kw):
-        super().__init__(error_code, error_name, response, message)
-
-
-class ActionRequired(TwitterError):
-    """
-        Exception Raised when the Twitter Login Request require an additional step from the user
-
-        Attributes:
-            message -- explanation of the error
-    """
-
-    def __init__(self, error_code, error_name, response, message, **kw):
-        super().__init__(error_code, error_name, response, message)
-
-
-class InvalidCredentials(TwitterError):
-    """
-        Exception Raised when cookies credentials are invalid
-
-        Attributes:
-            message -- explanation of the error
-    """
-
-    def __init__(self, error_code, error_name, response, message="The Cookies are Invalid", **kw):
-        super().__init__(error_code, error_name, response, message)
-
-
-class InvalidBroadcast(TwitterError):
-    """
-        Exception Raised when cookies are required for making a specific request
-
-        Attributes:
-            message -- explanation of the error
-    """
-
-    def __init__(self, error_code, error_name, response, message="The Broadcast doesn't exists", **kw):
-        super().__init__(error_code, error_name, response, message)
-
-
-class AuthenticationRequired(TwitterError):
-    """
-        Exception Raised when cookies are required for making a specific request
-
-        Attributes:
-            message -- explanation of the error
-    """
-
-    def __init__(self, error_code, error_name, response, message="You need to be authenticated and connected to make this request", **kw):
-        super().__init__(error_code, error_name, response, message)
-
-
-class ListNotFound(TwitterError):
-    """
-        Exception Raised when queried list wasn't found
-
-        Attributes:
-            message -- explanation of the error
-    """
-
-    def __init__(self, error_code, error_name, response, message="List not Found", **kw):
-        super().__init__(error_code, error_name, response, message)
-
-
-class AudioSpaceNotFound(TwitterError):
-    """
-        Exception Raised when queried Audio Space isn't found
-
-        Attributes:
-            message -- explanation of the error
-    """
-
-    def __init__(self, error_code, error_name, response, message="Audio Space not found", **kw):
-        super().__init__(error_code, error_name, response, message)
-
-
-class ProtectedTweet(TwitterError):
-    """
-        Exception Raised when queried Tweet is protected, and you need authorization to access it
-
-        Attributes:
-            message -- explanation of the error
-    """
-
-    def __init__(self, error_code, error_name, response, message="Tweet is private/protected", **kw):
-        super().__init__(error_code, error_name, response, message)
-
-
-# For Backward Compatibility
+
+TWITTER_ERRORS = {0: 'DefaultApiError', 3: 'InvalidCoordinates', 4: 'InvalidGranularity', 5: 'InvalidAccuracy', 6: 'NoDataForPoint', 7: 'NoDataForPointRadius', 8: 'InvalidId', 9: 'InvalidMaxResults', 10: 'RockdoveError', 11: 'InvalidIp', 12: 'MustProvideCoordinatesIpQueryOrAttributes', 13: 'NoLocationForIp', 14: 'OverlimitAddressBookApi', 15: 'AddressBookDarkmoded', 16: 'AddressBookPermissionsError', 17: 'AddressBookLookupNotFound', 18: 'TooManyTerms', 19: 'RetweetDarkmoded', 20: 'NoScreenNameProvided', 21: 'ContributorsNotEnabled', 22: 'NotAuthorizedToViewUser', 23: 'BulkLookupDarkmoded', 24: 'UnsupportedProfileImageSize', 25: 'MissingQuery', 26: 'AutocompleteMustBeTrueOrFalse', 27: 'AccountLocked', 28: 'GenericDarkmode', 29: 'TimeOut', 30: 'WoeidDataUnavailable', 31: 'InvalidTimescale', 32: 'InvalidCredentials', 33: 'OverLimit', 34: 'GenericNotFound', 35: 'TrendDataUnavailable', 36: 'CantReportYourselfAsSpam', 37: 'GenericAccessDenied', 38: 'MissingParameter', 39: 'InvalidCreationToken', 41: 'RockdoveInvalidArgumentError', 42: 'InvalidAttribute', 43: 'AttributeAccessDenied', 44: 'InvalidParameter', 46: 'InvalidPlaceJson', 47: 'InvalidRequestUrl', 48: 'TimeoutRequestRainbird', 49: 'NoFollowRequest', 50: 'GenericUserNotFound', 51: 'PromotedContentOfflineError', 52: 'PromotedSearchNoQuery', 53: 'BasicAuthDisabled', 54: 'CassowaryError', 55: 'ResourceNotFound', 56: 'InvalidEmailAddress', 57: 'PasswordResetPermissionsError', 58: 'PasswordResetExpiredToken', 59: 'PasswordResetInvalidHash', 60: 'PasswordResetMismatchedEntries', 61: 'ClientNotPermitted', 62: 'CustomSaveErrors', 63: 'OtherUserSuspended', 64: 'CurrentUserSuspended', 65: 'StrictMustBeTrueOrFalse', 66: 'RequireActivityMustBeTrueOrFalse', 67: 'BackendServiceUnavailable', 68: 'EndpointDeprecated', 69: 'TalonUrlMalware', 70: 'InvalidPromotedContentLogEvent', 71: 'EmailDeliveryError', 72: 'ApplicationNotFound', 73: 'ApplicationNotDeleted', 74: 'ApplicationDomainNotRevoked', 75: 'ApplicationKeysNotReset', 76: 'ApplicationImageNotProcessed', 77: 'ApplicationNoManageRight', 78: 'ApplicationNoAdminRight', 79: 'InvalidTrimPlace', 80: 'CurationDarkmoded', 81: 'ContributorsAccessLevelNotValid', 82: 'ContributorsTargetUserNotSpecified', 83: 'ContributorsTargetUserNotValid', 84: 'TalonUrlUnrenderable', 85: 'ValidationFailure', 86: 'WrongHttpMethod', 87: 'ClientNotPrivileged', 88: 'RateLimitExceeded', 89: 'BadOauthToken', 90: 'ContributionNotPermitted', 91: 'InvalidUtf8', 92: 'SslRequired', 93: 'DmAccessRequired', 94: 'PageIsForbidden', 95: 'InvalidLanguage', 96: 'InvalidIds', 97: 'EndpointFeatureDeprecated', 98: 'FlagPossiblySensitiveScribeError', 99: 'AuthenticityTokenError', 100: 'GenericThriftException', 101: 'InvalidReverseAuthCredentials', 102: 'DarkmodedFeature', 103: 'TrendsAvailableTransientException', 104: 'ListAdminRightsError', 105: 'MaximumMembersExceeded', 106: 'AddBlockedUserError', 107: 'NoTargetUser', 108: 'TargetUserNotFound', 109: 'TargetUserNotRelatedToList', 110: 'ListNotAMemberError', 111: 'TargetUserSuspended', 112: 'InsufficientListParameters', 113: 'InsufficientTargetUserParameters', 114: 'InvalidCurrentPassword', 115: 'ListUnauthorizedSubscriptionError', 116: 'PasswordSmsResetPwSeedNotExist', 117: 'PasswordSmsResetOptOut', 118: 'ArgumentTooLarge', 119: 'NarrowcastNotSupported', 120: 'AccountUpdateFailure', 121: 'InvalidHexColor', 122: 'UpdateProfileColorsError', 123: 'ImageUpdateError', 124: 'AttributeUpdateError', 125: 'GeolocationError', 126: 'LoggedOut', 127: 'ArchiveDeprecated', 128: 'LocationUpdateFailure', 129: 'EmailRateLimitExceeded', 130: 'OverCapacity', 131: 'InternalError', 132: 'UnusedBackgroundUploadError', 133: 'NoSelectedBackgroundError', 134: 'TooManyDevices', 135: 'OauthTimestampException', 136: 'BlockedUserError', 137: 'PushForbidden', 138: 'FollowingInformationUnavailable', 139: 'DuplicateFavorite', 140: 'FollowingStatusUnauthorized', 141: 'InactiveUser', 142: 'ProtectedStatusFavoriteError', 143: 'FavoriteRateLimitExceeded', 144: 'StatusNotFound', 145: 'RecordInvalid', 146: 'OtherUserNotBlocked', 147: 'SelfBlockError', 148: 'UnsupportedDevice', 149: 'InvalidEnabledFor', 150: 'DirectMessageOtherUserNotFollowing', 151: 'MessageSendError', 152: 'DirectMessageDestroyPermissionsError', 153: 'DirectMessageDeleteError', 154: 'DirectMessageNotFound', 155: 'MessageSendUnknownError', 156: 'DowntimeAlert', 157: 'VerifiedDeviceNotFound', 158: 'SelfFollowError', 159: 'GenericSuspended', 160: 'DuplicateFollowRequest', 161: 'FollowRateLimitExceeded', 162: 'FollowBlockedUserError', 163: 'IndeterminateSource', 164: 'TargetUserNotSpecified', 165: 'MultipleMissingParameters', 166: 'MultipleUserNotFound', 167: 'FollowError', 168: 'StatusNotFoundForbidden', 169: 'StatusRelatedResultsForbidden', 170: 'ForbiddenMissingParameter', 171: 'SearchDeletionError', 172: 'SearchCreationError', 173: 'ConfirmEmailExpiredCode', 174: 'ConfirmEmailInvalidCode', 175: 'ConfirmEmailInvalidStateChange', 176: 'ConfirmEmailAlreadyConfirmed', 177: 'ConfirmEmailSuccessChanged', 178: 'ConfirmEmailSuccessNew', 179: 'StatusViewForbidden', 180: 'GenericEndpointOffline', 181: 'TimeParameterOrderError', 182: 'ParameterDeprecated', 183: 'StatusActionPermissionError', 184: 'StatusUpdateError', 185: 'OverStatusUpdateLimit', 186: 'StatusTooLongError', 187: 'DuplicateStatusError', 188: 'StatusMalwareError', 189: 'StatusCreationError', 190: 'UnknownInterpreterError', 191: 'OverPhotoLimit', 192: 'OverMediaEntitiesPerUpdateLimit', 193: 'MediaTooLarge', 194: 'StatusUpdateForbidden', 195: 'InvalidRequestUrlForbidden', 196: 'TimelineAuthorizationRequired', 197: 'CategoryNotFound', 198: 'ContactLoadError', 199: 'IdsOfContactsError', 200: 'GenericForbidden', 201: 'GetRequired', 202: 'InternalApplicationAuthenticationDenied', 203: 'DeviceError', 204: 'DestinationError', 205: 'SpamRateLimitExceeded', 206: 'InvalidDeviceRelationship', 207: 'AlreadyActivated', 208: 'FormatNotSupported', 209: 'DirectMessageMustFollowFirst', 210: 'TokenLimitExceeded', 211: 'InvalidBrandBanner', 212: 'ProfileBannerUploadsDisabled', 213: 'ProcessingInProgress', 214: 'GenericBadRequest', 215: 'BadAuthenticationData', 216: 'ShareViaEmailRateLimitExceeded', 217: 'ProtectedStatusShareViaEmailError', 218: 'RestrictedAccessShareViaEmailError', 219: 'ShareViaEmailIpRateLimitExceeded', 220: 'RestrictedAuthToken', 221: 'CursorInvalid', 222: 'TieredActionSignupSpammer', 223: 'EmailTweetSendingError', 224: 'MissingEmailAddress', 225: 'TieredActionFollowSpammer', 226: 'TieredActionTweetSpammer', 227: 'TieredActionFollowCreeper', 228: 'TieredActionTweetCreeper', 229: 'AmbiguousCredentials', 230: 'UserSleeping', 231: 'RequiresLoginVerification', 232: 'CannotEnableLoginVerificationPhone', 233: 'CannotEnableLoginVerificationAlreadyEnabled', 234: 'CannotEnableLoginVerificationUnconfirmedEmail', 235: 'ExpiredLoginVerificationRequest', 236: 'IncorrectChallengeResponse', 237: 'MissingLoginVerificationRequest', 238: 'NewPasswordWeak', 239: 'BadGuestToken', 240: 'TieredActionSignupSpammerPhoneVerify', 241: 'RejectedLoginVerificationRequest', 242: 'DeactivatedUser', 243: 'OverLimitLogin', 244: 'ForcePasswordReset', 245: 'OverLimitLoginVerificationStart', 246: 'OverLimitLoginVerificationAttempt', 247: 'CannotEnableLoginVerificationPush', 248: 'LoginVerificationAlreadyEnabled', 249: 'CloudIpRestricted', 250: 'UserMustBeAlcoholAgeScreened', 251: 'EndpointRetired', 252: 'DmSpamTimeout', 253: 'NotYetApprovedLoginVerification', 254: 'OfflineCodeSync', 255: 'RequiresTemporaryPassword', 256: 'CannotFollowFromCountry', 257: 'BadDeviceToken', 258: 'AppsCreateRequiresConfirmedEmail', 259: 'AppsCreateRequiresVerifiedPhone', 260: 'AppsCreateRejectedForAbuse', 261: 'AppInReadOnlyMode', 262: 'CurrentUserNeedsPhoneVerification', 263: 'TieredActionChallengeCaptcha', 264: 'TargetUserNotFollowing', 265: 'TargetUserNotFavoriteFollowing', 266: 'FailureSendingLoginVerificationRequest', 267: 'InvalidCredentialsOneFactorEligible', 268: 'MissingOneFactorLoginVerificationParams', 269: 'UserIsNotSdkUser', 270: 'AppsUpdateSettingsRequiresVerifiedPhone', 271: 'SelfMuteError', 272: 'NotMutingTargetUser', 273: 'ScheduledInPast', 274: 'ScheduledTooFarInFuture', 275: 'TooLateToEdit', 276: 'ScheduleInvalid', 277: 'DirectMessageRecipientDoesNotFollowSenderWithUnverifiedPhoneNumber', 278: 'DirectMessageUserNotInConversation', 279: 'DirectMessageConversationNotFound', 280: 'DirectMessageTooManyParticipants', 281: 'DirectMessageTooFewParticipants', 282: 'DirectMessageRecipientBlocksSender', 283: 'TieredActionFavoriteSpammer', 284: 'DeviceRegistrationGeneralError', 285: 'DeviceAlreadyRegistered', 286: 'DeviceOperatorUnsupported', 287: 'UserAlreadyHasVerifiedPhone', 288: 'CannotReuseCurrentPassword', 289: 'DevicePinInvalid', 290: 'DevicePinRequired', 291: 'UnexpectedDeviceProvided', 292: 'TieredActionConversationSpammer', 293: 'SmsVerifyGeneralError', 294: 'SmsVerifyInvalidPin', 295: 'SmsVerifyRateLimitExceeded', 296: 'DtabOverrideDarkmoded', 297: 'DirectMessageCannotHaveBothTweetAndMedia', 298: 'DirectMessageTweetNotFound', 299: 'DeviceRegistrationRateExceeded', 300: 'DeviceRegistrationInvalidInput', 301: 'DeviceRegistrationPending', 302: 'DeviceRegistrationOperationFailed', 303: 'DeviceRegistrationPhoneNormalizationFailed', 304: 'DeviceRegistrationPhoneCountryDetectionFailed', 305: 'CannotIdentifyByEmail', 306: 'TieredActionAccessTokenGrantSpam', 307: 'TieredActionAccessTokenRevokeSpam', 308: 'NoSmsVerifyExists', 309: 'DeviceNotVerified', 310: 'ExpiredPin', 311: 'DirectMessageDuplicate', 312: 'LocationNameMustBeSpecified', 313: 'EULANotAccepted', 314: 'VideoTranscodingError', 315: 'ClientCaptchaRequired', 316: 'CannotContributeToYourself', 317: 'AccountHasTooManyContributors', 318: 'AccountHasTooManyContributees', 319: 'CannotChangePassword', 320: 'ContributorsAccessLevelInsufficient', 321: 'DirectMessageConversationNameTooLong', 322: 'DirectMessageGenericUserCouldNotBeAdded', 323: 'AnimatedGifMultipleImages', 324: 'InvalidMediaId', 325: 'MediaNotFound', 326: 'AccessDeniedByBouncer', 327: 'AlreadyRetweeted', 328: 'InvalidRetweetForStatus', 329: 'NonsupportingClientRequiresLoginVerification', 330: 'ContributorsGenericUserCouldNotBeAdded', 331: 'MobileSettingsUserNotFound', 332: 'MobileSettingsTemplateNotFound', 333: 'MobileSettingsFileNotFound', 334: 'MobileSettingsUnsupportedTransport', 335: 'MobileSettingsSettingNotFound', 336: 'MobileSettingsInvalidValueFound', 337: 'MobileSettingsSettingObjectNotFound', 338: 'MobileSettingsEnabledForMissing', 339: 'MobileSettingsNoDevicesFound', 340: 'MobileSettingsNoIncomingPushSettings', 341: 'MobileSettingsNoIncomingSmsSettings', 342: 'MobileSettingsIncorrectApplicationId', 343: 'MobileSettingsNoIncomingSettings', 344: 'UserActionRateLimitExceeded', 345: 'OneFactorMethodIsNotSupported', 346: 'UserIsNotOneFactorEligible', 347: 'InvalidRequestToken', 348: 'ClientApplicationNotPermitted', 349: 'DirectMessageCannotDmOtherUser', 350: 'OauthException', 351: 'MobileSettingsCouldNotUpdateSleep', 352: 'ParameterLimitExceeded', 353: 'DeniedByApiCsrfProtection', 354: 'DirectMessageTooLongError', 355: 'GenericConflict', 356: 'GenericValidationFailure', 357: 'RequiredFieldMissing', 358: 'JsonProcessingError', 359: 'ValueTooLarge', 360: 'ValueTooSmall', 361: 'ValueCannotBeEmpty', 362: 'TimeNotFuture', 363: 'InvalidCountryCodes', 364: 'InvalidTimeGranularity', 365: 'InvalidUUID', 366: 'InvalidValues', 367: 'SizeOutOfRange', 368: 'TimeNotPast', 369: 'InvalidJsonSyntax', 370: 'DigitsCannotReuseCurrentEmail', 371: 'MentionLimitInTweetExceeded', 372: 'UrlLimitInTweetExceeded', 373: 'HashtagLimitInTweetExceeded', 374: 'ExpiredQrCode', 375: 'InvalidQrCode', 376: 'MissingCredentials', 377: 'TokenRetrievalException', 378: 'TokenMissing', 379: 'DataminrUserNotLinked', 380: 'ABLiveSyncIsDisabled', 381: 'SoftUserCreationSpamDenied', 382: 'SoftUserActionSpamDenied', 383: 'CashtagLimitInTweetExceeded', 384: 'HashtagLengthLimitInTweetExceeded', 385: 'InReplyToTweetNotFound', 386: 'AttachmentTypesLimitInTweetExceeded', 387: 'NotEnoughFollowers', 388: 'FeatureAccessLimited', 389: 'DirectMessagesSenderBlocksRecipient', 390: 'SearchRecordingNotFound', 391: 'MaximumSearchRecordingsExceeded', 392: 'SessionNotFound', 393: 'SessionModificationNotAuthorized', 394: 'SessionModificationFailed', 395: 'VoiceVerifyRateLimitExceeded', 396: 'BlockUserFailed', 397: 'InvalidMetricsJson', 398: 'OnboardingFlowFailure', 399: 'OnboardingFlowRetriableFailure', 400: 'NoTwoFactorAuthMethodFound', 401: 'MomentCapsuleAccessError', 402: 'CannotEnrollLoginVerificationNotYetEnabled', 403: 'IneligibleFor2faAfterModification', 404: 'CookiesRequired', 405: 'DuplicateBookmark', 406: 'ProtectedTweetBookmarkError', 407: 'DirectMessageInactiveDevice', 408: 'InvalidUrl', 409: 'BirthdateRequired', 410: 'PasswordVerificationRequired', 411: 'DirectMessageSenderInSecretDmsDisabledCountry', 412: 'DirectMessageRecipientInSecretDmsDisabledCountry', 413: 'DirectMessageSenderDeviceIsNotActiveForSecretDms', 414: 'DirectMessageRecipientDeviceIsNotActiveForSecretDms', 415: 'CallbackUrlLocked', 416: 'InvalidOrSuspendedApp', 417: 'InvalidDesktopCallback', 418: 'DirectMessageSenderIsNotRegisteredForSecretDms', 419: 'DirectMessageRecipientIsNotRegisteredForSecretDms', 420: 'ReservedErrorCode', 421: 'TweetIsBounced', 422: 'TweetIsBounceDeleted', 423: 'InvalidHeaders', 424: 'MomentUnavailableForNewsCamera', 425: 'TweetEngagementsLimited', 426: 'InvalidRequestIpv6Token', 427: 'IpResolverNotAvailable', 428: 'ValidIpv6TokenRequired', 429: 'HarmfulLink', 430: 'ConversationControlNotAllowed', 431: 'ConversationControlNotSupported', 432: 'ConversationControlNotAuthorized', 433: 'ConversationControlReplyRestricted', 434: 'NotMutingTargetList', 435: 'ConversationControlInvalidParameter', 436: 'PassswordRequiredForEmailUpdate', 437: 'NewPasswordShort', 438: 'NewPasswordLong', 439: 'NudgeReceived', 440: 'CommunityUserNotAuthorized', 441: 'CommunityNotFound', 442: 'CommunityRetweetNotAllowed', 443: 'CommunityInvalidParams', 444: 'CommunityReplyTweetNotAllowed', 445: 'RestrictedSession', 446: 'TokenSecurityLevelAgreementPolicyFailure', 447: 'SuperFollowsCreateNotAuthorized', 448: 'SuperFollowsInvalidParams', 449: 'TOOMomentsList', 450: 'CommunityProtectedUserCannotTweet', 451: 'ExclusiveTweetEngagementNotAllowed', 452: 'SteamCreationException', 453: 'V11Restricted', 454: 'SteamGetException', 455: 'TrustedFriendsInvalidParams', 456: 'TrustedFriendsRetweetNotAllowed', 457: 'TrustedFriendsEngagementNotAllowed', 458: 'CollabTweetInvalidParams', 459: 'TrustedFriendsCreateNotAllowed', 460: 'TrustedFriendsQuoteTweetNotAllowed', 461: 'StaleTweetEngagementNotAllowed', 462: 'StaleTweetQuoteTweetNotAllowed', 463: 'RetweetIdBookmarkError', 464: 'FieldEditNotAllowed', 465: 'StaleTweetRetweetNotAllowed', 466: 'NotEligibleForEdit', 467: 'V11TierRestricted', 468: 'DirectMessageUnregisteredDevice', 469: 'DirectMessageSenderIsNotBlueVerifiedForSecretDms', 470: 'DirectMessageRecipientIsNotBlueVerifiedForSecretDms', 471: 'ConversationKeysNotProvidedForNewSecretConversation', 472: 'ConversationKeysProvidedForExistingSecretConvo', 473: 'InvalidConversationKeysProvidedForNewSecretConvo', 474: 'DirectMessageReplyNotInConversation', 475: 'DirectMessageConversationMetadataNotFound', 476: 'DirectMessageSenderIsNotVerifiedForMessageRequests', 477: 'DirectMessageSenderIsNotVerifiedRateLimited'}
+
+
+class TwitterError(Exception):
+    """
+        Base Exception raised when error Occurs.
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(
+            self,
+            error_code,
+            error_name,
+            response,
+            message
+    ):
+        self.message = message
+        self.error_code = error_code
+        self.error_name = error_name
+        self.response = response
+
+        if self.response is not None and not isinstance(self.response, dict) and not self.response.json() and self.response.text:
+            self.message = self.response.text
+        elif str(self.error_code) == "404":
+            self.message = "Page not Found. Most likely you need elevated authorization to access this resource"
+
+        super().__init__(self.message)
+
+
+class UserNotFound(TwitterError):
+    """Exception raised when user isn't found.
+
+    Attributes:
+        message -- explanation of the error
+    """
+
+    def __init__(self, error_code=50, error_name="GenericUserNotFound", response=None, message="The User Account wasn't Found or is Protected", **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+class GuestTokenNotFound(TwitterError):
+    """
+    Exception Raised when the guest token wasn't found after specific number of retires
+
+    Attributes:
+        message -- explanation of the error
+    """
+
+    def __init__(self, error_code=404, error_name="GuestTokenNotFound", response=None, message="The Guest Token couldn't be obtained", **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+class InvalidTweetIdentifier(TwitterError):
+    """
+        Exception Raised when the tweet identifier is invalid
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code=144, error_name="StatusNotFound", response=None, message="The Tweet Identifier is Invalid", **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+class RateLimitReached(TwitterError):
+    """
+        Exception Raised when the tweet identifier is invalid
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code, error_name, response, message="You have exceeded the Twitter Rate Limit", **kw):
+        super().__init__(error_code, error_name, response, message)
+        self.retry_after = kw.get('retry_after')  # Number of seconds required for rate limit to be reset
+
+
+class ProxyParseError(TwitterError):
+    """
+    Exception Raised when an error occurs while parsing the provided proxy
+
+    Attributes:
+        message -- explanation of the error
+    """
+
+    def __init__(self, message="Error while parsing the Proxy, please make sure you are passing the right formatted proxy", **kw):
+        super().__init__(0, "ProxyParseError", None, message)
+
+
+class UserProtected(TwitterError):
+    """
+    Exception Raised when an error occurs when the queried User isn't available / Protected
+
+    Attributes:
+        message -- explanation of the error
+    """
+
+    def __init__(self, error_code=403, error_name="UserUnavailable", response=None, message=None, **kw):
+
+        if not message:
+            message = "The User is Protected OR Unavailable, please make sure you are authenticated and authorized"
+
+        super().__init__(error_code, error_name, response, message)
+
+
+class DeniedLogin(TwitterError):
+    """
+        Exception Raised when the Twitter deny the login request ,
+        could be due to multiple login attempts (or failed attempts)
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code=37, error_name="GenericAccessDenied", response=None, message=None, **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+class ActionRequired(TwitterError):
+    """
+        Exception Raised when the Twitter Login Request require an additional step from the user
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code, error_name, response, message, **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+class InvalidCredentials(TwitterError):
+    """
+        Exception Raised when cookies credentials are invalid
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code, error_name, response, message="The Cookies are Invalid", **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+class InvalidBroadcast(TwitterError):
+    """
+        Exception Raised when cookies are required for making a specific request
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code, error_name, response, message="The Broadcast doesn't exists", **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+class AuthenticationRequired(TwitterError):
+    """
+        Exception Raised when cookies are required for making a specific request
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code, error_name, response, message="You need to be authenticated and connected to make this request", **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+class ListNotFound(TwitterError):
+    """
+        Exception Raised when queried list wasn't found
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code, error_name, response, message="List not Found", **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+class AudioSpaceNotFound(TwitterError):
+    """
+        Exception Raised when queried Audio Space isn't found
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code, error_name, response, message="Audio Space not found", **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+class ProtectedTweet(TwitterError):
+    """
+        Exception Raised when queried Tweet is protected, and you need authorization to access it
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code, error_name, response, message="Tweet is private/protected", **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+class LockedAccount(TwitterError):
+    """
+        Exception Raised when Twitter Account is locked at most likely require to pass captcha to unlock
+
+        Attributes:
+            message -- explanation of the error
+    """
+
+    def __init__(self, error_code, error_name, response, message="Your Account is Locked", **kw):
+        super().__init__(error_code, error_name, response, message)
+
+
+# For Backward Compatibility
 UnknownError = TwitterError
```

### Comparing `tweety_ns-1.1.5/src/tweety/filters.py` & `tweety_ns-1.1.6/src/tweety/filters.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.5/src/tweety/http.py` & `tweety_ns-1.1.6/src/tweety/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import os
 import re
 import warnings
 from typing import Callable
 from urllib.parse import quote
 import httpx
-from .exceptions_ import GuestTokenNotFound, UnknownError, UserNotFound, InvalidCredentials
+from .exceptions import GuestTokenNotFound, TwitterError, UserNotFound, InvalidCredentials
 from .types.n_types import GenericError
 from .utils import custom_json, GUEST_TOKEN_REGEX
 from .builder import UrlBuilder
 
 httpx.Response.json = custom_json
 
 
@@ -79,15 +79,15 @@
         if ignore_none_data and len(response.text) == 0:
             return None
 
         if (not response_json and response.text and response.text.lower() == "rate limit exceeded") or response.status_code == 429:
             response_json = {"errors": [{"code": 88, "message": "Rate limit exceeded."}]}
 
         if not response_json:
-            raise UnknownError(
+            raise TwitterError(
                 error_code=response.status_code,
                 error_name="Server Error",
                 response=response,
                 message="Unknown Error Occurs on Twitter"
             )
 
         if response_json.get("errors") and not response_json.get('data'):
@@ -436,14 +436,19 @@
         return response
 
     def get_user_followings(self, user_id, cursor=None):
         request_data = self.__builder.get_user_followings(user_id, cursor)
         response = self.__get_response__(**request_data)
         return response
 
+    def get_user_subscribers(self, user_id, cursor=None):
+        request_data = self.__builder.get_user_subscribers(user_id, cursor)
+        response = self.__get_response__(**request_data)
+        return response
+
     def toggle_user_notifications(self, user_id, action):
         request_data = self.__builder.toggle_user_notifications(user_id, action)
         response = self.__get_response__(**request_data)
         return response
 
     def get_lists(self, cursor=None):
         request_data = self.__builder.get_lists(cursor)
```

### Comparing `tweety_ns-1.1.5/src/tweety/session.py` & `tweety_ns-1.1.6/src/tweety/session.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import json
-import os.path
-
-
-class Session:
-    def __init__(self, client):
-        self._client = client
-        self.user = None
-        self.logged_in = False
-        self.cookies = ""
-
-    def cookies_dict(self):
-        result = {}
-        split = str(self.cookies).split(";")
-        for i in split:
-            try:
-                key, value = i.split("=")
-                result[key] = value
-            except:
-                pass
-
-        return result
-
-    def __str__(self):
-        return self.cookies
-
-
-class MemorySession(Session):
-
-    def __init__(self):
-        super().__init__(None)
-
-    def __call__(self, client):
-        self._client = client
-        return self
-
-    def set_session_user(self, user):
-        self.user = dict(user)
-
-    def save_session(self, cookies):
-        self.cookies = str(cookies)
-        self.logged_in = True
-
-
-class FileSession(Session):
-    def __init__(self, client, session_name):
-        super().__init__(client)
-        self.session_name = os.path.basename(session_name)
-        self.session_file_path = self._get_session_file_path(session_name, self.session_name)
-        self._load_session()
-
-    @staticmethod
-    def _get_session_file_path(session_path, session_name):
-        _session = session_name.replace(".tw_session", "")
-        directory = os.path.dirname(session_path) or os.getcwd()
-        return os.path.abspath(os.path.join(directory, f"{_session}.tw_session"))
-
-    def _load_session(self):
-        if os.path.exists(self.session_file_path):
-            with open(self.session_file_path, "r") as f:
-                session_data = json.load(f)
-                self.cookies = session_data['cookies']
-                self.user = session_data['user']
-
-            self.logged_in = True
-
-    def set_session_user(self, user):
-        self.user = dict(user)
-
-        with open(self.session_file_path, "w") as f:
-            session_data = dict(cookies=str(self.cookies), user=dict(user))
-            json.dump(session_data, f, indent=4, default=str)
-
-    def save_session(self, cookies):
-        self.cookies = str(cookies)
-        self.logged_in = True
-        with open(self.session_file_path, "w") as f:
-            session_data = dict(cookies=str(cookies))
-            json.dump(session_data, f, indent=4)
-
+import json
+import os.path
+
+
+class Session:
+    def __init__(self, client):
+        self._client = client
+        self.user = None
+        self.logged_in = False
+        self.cookies = ""
+
+    def cookies_dict(self):
+        result = {}
+        split = str(self.cookies).split(";")
+        for i in split:
+            try:
+                key, value = i.split("=")
+                result[key] = value
+            except:
+                pass
+
+        return result
+
+    def __str__(self):
+        return self.cookies
+
+
+class MemorySession(Session):
+
+    def __init__(self):
+        super().__init__(None)
+
+    def __call__(self, client):
+        self._client = client
+        return self
+
+    def set_session_user(self, user):
+        self.user = dict(user)
+
+    def save_session(self, cookies):
+        self.cookies = str(cookies)
+        self.logged_in = True
+
+
+class FileSession(Session):
+    def __init__(self, client, session_name):
+        super().__init__(client)
+        self.session_name = os.path.basename(session_name)
+        self.session_file_path = self._get_session_file_path(session_name, self.session_name)
+        self._load_session()
+
+    @staticmethod
+    def _get_session_file_path(session_path, session_name):
+        _session = session_name.replace(".tw_session", "")
+        directory = os.path.dirname(session_path) or os.getcwd()
+        return os.path.abspath(os.path.join(directory, f"{_session}.tw_session"))
+
+    def _load_session(self):
+        if os.path.exists(self.session_file_path):
+            with open(self.session_file_path, "r") as f:
+                session_data = json.load(f)
+                self.cookies = session_data['cookies']
+                self.user = session_data.get('user', {})
+
+            self.logged_in = True
+
+    def set_session_user(self, user):
+        self.user = dict(user)
+
+        with open(self.session_file_path, "w") as f:
+            session_data = dict(cookies=str(self.cookies), user=dict(user))
+            json.dump(session_data, f, indent=4, default=str)
+
+    def save_session(self, cookies):
+        self.cookies = str(cookies)
+        self.logged_in = True
+        with open(self.session_file_path, "w") as f:
+            session_data = dict(cookies=str(cookies))
+            json.dump(session_data, f, indent=4)
+
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/__init__.py` & `tweety_ns-1.1.6/src/tweety/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,34 +28,39 @@
     Topic,
     TweetTranslate,
     TweetAnalytics,
     Place
 )
 from .n_types import (
     UploadedMedia,
-    Proxy,
-    PROXY_TYPE_SOCKS4,
-    PROXY_TYPE_SOCKS5,
-    PROXY_TYPE_HTTP,
-    HOME_TIMELINE_TYPE_FOLLOWING,
-    HOME_TIMELINE_TYPE_FOR_YOU,
-    INBOX_PAGE_TYPES,
-    INBOX_PAGE_TYPE_TRUSTED,
-    INBOX_PAGE_TYPE_UNTRUSTED
+    Proxy
 )
 from .search import Search, TypeHeadSearch
 from .usertweet import UserTweets, SelfTimeline, TweetComments, TweetHistory, UserMedia, UserHighlights, UserLikes
 from .mentions import Mention
 from .inbox import Inbox, SendMessage, Media, Conversation
 from .bookmarks import Bookmarks
 from .likes import TweetLikes
 from .retweets import TweetRetweets
 from .community import CommunityTweets, CommunityMembers
 from .notification import TweetNotifications
 from .lists import Lists, ListMembers, ListTweets
-from .follow import UserFollowers, UserFollowings, MutualFollowers, BlockedUsers
+from .follow import UserFollowers, UserFollowings, MutualFollowers, BlockedUsers, UserSubscribers
 from .gifs import GifSearch
 from .topic import TopicTweets
 from .places import Places
+from ..constants import (
+    PROXY_TYPE_SOCKS4,
+    PROXY_TYPE_SOCKS5,
+    PROXY_TYPE_HTTP,
+    HOME_TIMELINE_TYPE_FOLLOWING,
+    HOME_TIMELINE_TYPE_FOR_YOU,
+    INBOX_PAGE_TYPES,
+    INBOX_PAGE_TYPE_TRUSTED,
+    INBOX_PAGE_TYPE_UNTRUSTED,
+    MEDIA_TYPE_GIF,
+    MEDIA_TYPE_IMAGE,
+    MEDIA_TYPE_VIDEO
+)
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/base.py` & `tweety_ns-1.1.6/src/tweety/types/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import time
-
 from tweety.types import ShortUser
-
-from . import User, Tweet
+from .twDataTypes import User, Tweet
 from ..utils import find_objects, parse_wait_time
 
 
 class BaseGeneratorClass(dict):
 
     @staticmethod
     def _get_cursor_(response, cursor_key="Bottom"):
@@ -69,15 +67,17 @@
 
             if not self.is_next_page:
                 break
 
             this_page += 1
 
             if this_page != self.pages:
-                time.sleep(parse_wait_time(self.wait_time))
+                this_wait_time = parse_wait_time(self.wait_time)
+                print(this_wait_time)
+                time.sleep(this_wait_time)
 
 
 
         return self
 
     def __repr__(self):
         class_name = self.__class__.__name__
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/bookmarks.py` & `tweety_ns-1.1.6/src/tweety/types/bookmarks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import Tweet, Excel
+from .twDataTypes import Tweet, Excel
 from .base import BaseGeneratorClass
 
 
 class Bookmarks(BaseGeneratorClass):
     _RESULT_ATTR = "tweets"
 
     def __init__(self, user_id, client, pages=1, wait_time=2, cursor=None):
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/community.py` & `tweety_ns-1.1.6/src/tweety/types/community.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import traceback
-
-from . import SelfThread, Tweet, Excel, User
+from .twDataTypes import SelfThread, Tweet, Excel, User
 from .base import BaseGeneratorClass
 from ..utils import find_objects
 
 
 class CommunityTweets(BaseGeneratorClass):
     OBJECTS_TYPES = {
         "tweet": Tweet,
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/follow.py` & `tweety_ns-1.1.6/src/tweety/types/follow.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,144 +1,177 @@
-import traceback
-
-from .twDataTypes import User
-from .base import BaseGeneratorClass
-
-
-class UserFollowers(BaseGeneratorClass):
-    _RESULT_ATTR = "users"
-
-    def __init__(self, user_id, client, pages=1, wait_time=2, cursor=None):
-        super().__init__()
-        self.users = []
-        self.cursor = cursor
-        self.cursor_top = cursor
-        self.is_next_page = True
-        self.client = client
-        self.user_id = user_id
-        self.pages = pages
-        self.wait_time = wait_time
-
-    def get_page(self, cursor):
-        _users = []
-        response = self.client.http.get_user_followers(self.user_id, cursor=cursor)
-
-        entries = self._get_entries(response)
-
-        for entry in entries:
-            try:
-
-                parsed = User(self.client, entry, None)
-                if parsed:
-                    _users.append(parsed)
-            except:
-                pass
-
-        cursor = self._get_cursor_(response)
-        cursor_top = self._get_cursor_(response, "Top")
-
-        return _users, cursor, cursor_top
-
-
-class UserFollowings(BaseGeneratorClass):
-    _RESULT_ATTR = "users"
-
-    def __init__(self, user_id, client, pages=1, wait_time=2, cursor=None):
-        super().__init__()
-        self.users = []
-        self.cursor = cursor
-        self.cursor_top = cursor
-        self.is_next_page = True
-        self.client = client
-        self.user_id = user_id
-        self.pages = pages
-        self.wait_time = wait_time
-
-    def get_page(self, cursor):
-        _users = []
-        response = self.client.http.get_user_followings(self.user_id, cursor=cursor)
-
-        entries = self._get_entries(response)
-
-        for entry in entries:
-            try:
-
-                parsed = User(self.client, entry, None)
-                if parsed:
-                    _users.append(parsed)
-            except:
-                pass
-
-        cursor = self._get_cursor_(response)
-        cursor_top = self._get_cursor_(response, "Top")
-
-        return _users, cursor, cursor_top
-
-
-class MutualFollowers(BaseGeneratorClass):
-    _RESULT_ATTR = "users"
-
-    def __init__(self, user_id, client, pages=1, wait_time=2, cursor=None):
-        super().__init__()
-        self.users = []
-        self.cursor = cursor
-        self.cursor_top = cursor
-        self.is_next_page = True
-        self.client = client
-        self.user_id = user_id
-        self.pages = pages
-        self.wait_time = wait_time
-
-    def get_page(self, cursor):
-        _users = []
-        response = self.client.http.get_mutual_friends(self.user_id, cursor=cursor)
-
-        entries = self._get_entries(response)
-
-        for entry in entries:
-            try:
-
-                parsed = User(self.client, entry, None)
-                if parsed:
-                    _users.append(parsed)
-            except:
-                pass
-
-        cursor = self._get_cursor_(response)
-        cursor_top = self._get_cursor_(response, "Top")
-
-        return _users, cursor, cursor_top
-
-
-class BlockedUsers(BaseGeneratorClass):
-    _RESULT_ATTR = "users"
-
-    def __init__(self, client, pages=1, wait_time=2, cursor=None):
-        super().__init__()
-        self.users = []
-        self.cursor = cursor
-        self.cursor_top = cursor
-        self.is_next_page = True
-        self.client = client
-        self.pages = pages
-        self.user_id = self.client.me.id
-        self.wait_time = wait_time
-
-    def get_page(self, cursor):
-        _users = []
-        response = self.client.http.get_blocked_users(cursor=cursor)
-
-        entries = self._get_entries(response)
-
-        for entry in entries:
-            try:
-
-                parsed = User(self.client, entry, None)
-                if parsed:
-                    _users.append(parsed)
-            except:
-                pass
-
-        cursor = self._get_cursor_(response)
-        cursor_top = self._get_cursor_(response, "Top")
-
-        return _users, cursor, cursor_top
+from .twDataTypes import User
+from .base import BaseGeneratorClass
+
+
+class UserFollowers(BaseGeneratorClass):
+    _RESULT_ATTR = "users"
+
+    def __init__(self, user_id, client, pages=1, wait_time=2, cursor=None):
+        super().__init__()
+        self.users = []
+        self.cursor = cursor
+        self.cursor_top = cursor
+        self.is_next_page = True
+        self.client = client
+        self.user_id = user_id
+        self.pages = pages
+        self.wait_time = wait_time
+
+    def get_page(self, cursor):
+        _users = []
+        response = self.client.http.get_user_followers(self.user_id, cursor=cursor)
+
+        entries = self._get_entries(response)
+
+        for entry in entries:
+            try:
+
+                parsed = User(self.client, entry, None)
+                if parsed:
+                    _users.append(parsed)
+            except:
+                pass
+
+        cursor = self._get_cursor_(response)
+        cursor_top = self._get_cursor_(response, "Top")
+
+        return _users, cursor, cursor_top
+
+
+class UserFollowings(BaseGeneratorClass):
+    _RESULT_ATTR = "users"
+
+    def __init__(self, user_id, client, pages=1, wait_time=2, cursor=None):
+        super().__init__()
+        self.users = []
+        self.cursor = cursor
+        self.cursor_top = cursor
+        self.is_next_page = True
+        self.client = client
+        self.user_id = user_id
+        self.pages = pages
+        self.wait_time = wait_time
+
+    def get_page(self, cursor):
+        _users = []
+        response = self.client.http.get_user_followings(self.user_id, cursor=cursor)
+
+        entries = self._get_entries(response)
+
+        for entry in entries:
+            try:
+
+                parsed = User(self.client, entry, None)
+                if parsed:
+                    _users.append(parsed)
+            except:
+                pass
+
+        cursor = self._get_cursor_(response)
+        cursor_top = self._get_cursor_(response, "Top")
+
+        return _users, cursor, cursor_top
+
+
+class UserSubscribers(BaseGeneratorClass):
+    _RESULT_ATTR = "users"
+
+    def __init__(self, user_id, client, pages=1, wait_time=2, cursor=None):
+        super().__init__()
+        self.users = []
+        self.cursor = cursor
+        self.cursor_top = cursor
+        self.is_next_page = True
+        self.client = client
+        self.user_id = user_id
+        self.pages = pages
+        self.wait_time = wait_time
+
+    def get_page(self, cursor):
+        _users = []
+        response = self.client.http.get_user_subscribers(self.user_id, cursor=cursor)
+
+        entries = self._get_entries(response)
+
+        for entry in entries:
+            try:
+
+                parsed = User(self.client, entry, None)
+                if parsed:
+                    _users.append(parsed)
+            except:
+                pass
+
+        cursor = self._get_cursor_(response)
+        cursor_top = self._get_cursor_(response, "Top")
+
+        return _users, cursor, cursor_top
+
+
+class MutualFollowers(BaseGeneratorClass):
+    _RESULT_ATTR = "users"
+
+    def __init__(self, user_id, client, pages=1, wait_time=2, cursor=None):
+        super().__init__()
+        self.users = []
+        self.cursor = cursor
+        self.cursor_top = cursor
+        self.is_next_page = True
+        self.client = client
+        self.user_id = user_id
+        self.pages = pages
+        self.wait_time = wait_time
+
+    def get_page(self, cursor):
+        _users = []
+        response = self.client.http.get_mutual_friends(self.user_id, cursor=cursor)
+
+        entries = self._get_entries(response)
+
+        for entry in entries:
+            try:
+
+                parsed = User(self.client, entry, None)
+                if parsed:
+                    _users.append(parsed)
+            except:
+                pass
+
+        cursor = self._get_cursor_(response)
+        cursor_top = self._get_cursor_(response, "Top")
+
+        return _users, cursor, cursor_top
+
+
+class BlockedUsers(BaseGeneratorClass):
+    _RESULT_ATTR = "users"
+
+    def __init__(self, client, pages=1, wait_time=2, cursor=None):
+        super().__init__()
+        self.users = []
+        self.cursor = cursor
+        self.cursor_top = cursor
+        self.is_next_page = True
+        self.client = client
+        self.pages = pages
+        self.user_id = self.client.me.id
+        self.wait_time = wait_time
+
+    def get_page(self, cursor):
+        _users = []
+        response = self.client.http.get_blocked_users(cursor=cursor)
+
+        entries = self._get_entries(response)
+
+        for entry in entries:
+            try:
+
+                parsed = User(self.client, entry, None)
+                if parsed:
+                    _users.append(parsed)
+            except:
+                pass
+
+        cursor = self._get_cursor_(response)
+        cursor_top = self._get_cursor_(response, "Top")
+
+        return _users, cursor, cursor_top
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/gifs.py` & `tweety_ns-1.1.6/src/tweety/types/gifs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import Gif
+from .twDataTypes import Gif
 from .base import BaseGeneratorClass
 
 
 class GifSearch(BaseGeneratorClass):
     _RESULT_ATTR = "gifs"
 
     def __init__(self, search_term, client, pages=1, cursor=None, wait_time=2):
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/likes.py` & `tweety_ns-1.1.6/src/tweety/types/likes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import traceback
-
 from .base import BaseGeneratorClass
 from .twDataTypes import User
 
 
 class TweetLikes(BaseGeneratorClass):
     _RESULT_ATTR = "users"
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/lists.py` & `tweety_ns-1.1.6/src/tweety/types/lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import User, List, Tweet, SelfThread
+from .twDataTypes import User, List, Tweet, SelfThread
 from .base import BaseGeneratorClass
 from ..utils import find_objects
 
 
 class Lists(BaseGeneratorClass):
     _RESULT_ATTR = "lists"
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/mentions.py` & `tweety_ns-1.1.6/src/tweety/types/mentions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import traceback
-
-from . import Tweet
+from .twDataTypes import Tweet
 from .base import BaseGeneratorClass
 
 
 class Mention(BaseGeneratorClass):
     _RESULT_ATTR = "tweets"
 
     def __init__(self, user_id, client, pages=1, wait_time=2, cursor=None):
@@ -31,15 +29,14 @@
             tweet['author'], tweet['rest_id'], tweet['__typename'] = user, tweet_id, "Tweet"
 
             try:
                 parsed = Tweet(self.client, tweet, response)
                 if parsed:
                     _tweets.append(parsed)
             except:
-                traceback.print_exc()
                 pass
 
         cursor = self._get_cursor_(response)
         cursor_top = self._get_cursor_(response, "Top")
 
         return _tweets, cursor, cursor_top
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/n_types.py` & `tweety_ns-1.1.6/src/tweety/types/n_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,258 +1,251 @@
-import datetime
-import os
-import time
-from http.cookiejar import MozillaCookieJar
-from httpx._content import encode_multipart_data
-from . import Gif
-from ..utils import calculate_md5, get_random_string, check_if_file_is_image
-from ..exceptions_ import *
-
-PROXY_TYPE_SOCKS4 = SOCKS4 = 1
-PROXY_TYPE_SOCKS5 = SOCKS5 = 2
-PROXY_TYPE_HTTP = HTTP = 3
-HOME_TIMELINE_TYPE_FOR_YOU = "HomeTimeline"
-HOME_TIMELINE_TYPE_FOLLOWING = "HomeLatestTimeline"
-INBOX_PAGE_TYPE_TRUSTED = "trusted"
-INBOX_PAGE_TYPE_UNTRUSTED = "untrusted"
-INBOX_PAGE_TYPES = (INBOX_PAGE_TYPE_TRUSTED, INBOX_PAGE_TYPE_UNTRUSTED)
-
-
-class Proxy:
-    def __init__(self, host: str, port: int, proxy_type: int, username: str = None, password: str = None):
-        self.host = host
-        self.password = password
-        self.proxy_type = proxy_type
-        self.username = username
-        self.port = port
-        self.proxy = self.__parse__()
-
-    def __iter__(self):
-        for k, v in self.proxy.items():
-            yield k, v
-
-    def __proxy_url__(self):
-        if self.username and self.password:
-            return "{}:{}@{}:{}".format(
-                self.username, self.password, self.host, self.port
-            )
-        else:
-            return "{}:{}".format(self.host, self.port)
-
-    def __parse__(self):
-        proxy_url = self.__proxy_url__()
-        if self.proxy_type == HTTP:
-            http_url = "http://{}".format(proxy_url)
-            return dict.fromkeys(['http://', 'https://'], http_url)
-        elif self.proxy_type == SOCKS4:
-            socks_url = "socks4://{}".format(proxy_url)
-            return dict.fromkeys(['http://', 'https://'], socks_url)
-        elif self.proxy_type == SOCKS5:
-            socks_url = "socks5://{}".format(proxy_url)
-            return dict.fromkeys(['http://', 'https://'], socks_url)
-
-        raise ProxyParseError()
-
-    def get_dict(self):
-        return self.proxy
-
-
-class GenericError:
-    EXCEPTIONS = {
-        32: InvalidCredentials,
-        144: InvalidTweetIdentifier,
-        88: RateLimitReached,
-        477: RateLimitReached,
-        399: InvalidCredentials,
-        220: InvalidCredentials,
-        214: InvalidBroadcast,
-        366: InvalidTweetIdentifier,
-    }
-
-    def __init__(self, response, error_code, message=None):
-        self.response = response
-        self.error_code = error_code
-        self.message = message
-        self.retry_after = self._get_retry_after()
-        self._raise_exception()
-
-    def _get_retry_after(self):
-        if all(key in self.response.headers for key in ['x-rate-limit-reset', 'x-rate-limit-remaining']):
-            epochLimitTime = int(self.response.headers['x-rate-limit-reset'])
-            epochCurrentTime = int(datetime.datetime.now().timestamp())
-            return epochLimitTime - epochCurrentTime
-
-        return None
-
-    def _raise_exception(self):
-        if self.EXCEPTIONS.get(self.error_code):
-            raise self.EXCEPTIONS[self.error_code](
-                error_code=self.error_code,
-                error_name=TWITTER_ERRORS[self.error_code],
-                response=self.response,
-                message=self.message,
-                retry_after=self.retry_after
-            )
-
-        raise TwitterError(
-            error_code=self.error_code,
-            error_name=TWITTER_ERRORS.get(self.error_code, 0),
-            response=self.response,
-            message="[{}] {}".format(self.error_code, self.message)
-        )
-
-
-class Cookies:
-    def __init__(self, cookies, is_http_response=False):
-        self._raw_cookies = cookies
-        self._is_http_response = is_http_response
-        self.parse_cookies()
-
-    def parse_cookies(self):
-        if isinstance(self._raw_cookies, MozillaCookieJar):
-            for i in self._raw_cookies:
-                setattr(self, i.name, i.value)
-        else:
-            if self._is_http_response:
-                # TODO : Find a proper way to parse
-                n = [0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30]
-                for k, p in enumerate(self._raw_cookies.split(",")):
-                    if k in n:
-                        key, value = str(p.split(';')[0]).split("=", 1)
-                        setattr(self, key.strip(), value.strip())
-            else:
-                true_cookies = dict()
-                if isinstance(self._raw_cookies, str):
-                    cookie_list = self._raw_cookies.split(";")
-                    for cookie in cookie_list:
-                        split_cookie = cookie.strip().split("=", 1)
-
-                        if len(split_cookie) >= 2:
-                            cookie_key = split_cookie[0]
-                            cookie_value = split_cookie[1]
-                            true_cookies[cookie_key] = cookie_value
-                elif isinstance(self._raw_cookies, dict):
-                    true_cookies = self._raw_cookies
-                else:
-                    raise TypeError("cookies should be of class 'str', 'dict' or 'MozillaCookieJar' not {}".format(self._raw_cookies.__class__))
-
-                for key, value in true_cookies.items():
-                    setattr(self, key.strip(), value.strip())
-
-    def to_dict(self):
-        result = {}
-        for k, v in vars(self).items():
-
-            if not k.startswith("_"):
-                result[k] = v
-
-        return result
-
-    def __str__(self):
-        string = ""
-        for k, v in vars(self).items():
-
-            if not k.startswith("_"):
-                string += f"{k}={v};"
-
-        return string
-
-
-class UploadedMedia:
-    FILE_CHUNK_SIZE = 2 * 1024 * 1024  # 2 mb
-
-    def __init__(
-            self,
-            file_path,
-            client,
-            alt_text=None,
-            sensitive_media_warning=None,
-            media_category="tweet_image"
-    ):
-        self.media_id = None
-        self._file = file_path
-        self._client = client
-        self._alt_text = alt_text
-        self._sensitive_media_warning = sensitive_media_warning if sensitive_media_warning else []
-        self._source_url = self._get_source_url()
-        self.size = self._get_size()
-        self.mime_type = self.get_mime_type()
-        self._media_category = self._get_media_category(media_category)
-        self.md5_hash = calculate_md5(self._file)
-
-    def _get_source_url(self):
-        if isinstance(self._file, Gif):
-            return self._file.url
-        elif str(self._file).startswith("https://"):
-            return self._file
-
-        return None
-
-    def _get_media_category(self, category):
-        media_for = category.split("_")[0]
-        media_type = self.mime_type.split("/")[0]
-        return f"{media_for}_{media_type}" if "gif" not in self.mime_type else f"{media_for}_gif"
-
-    def _get_size(self):
-        if not self._source_url:
-            return os.path.getsize(self._file)
-        return 0
-
-    def get_mime_type(self):
-        return check_if_file_is_image(self._file)
-
-    @staticmethod
-    def _create_boundary():
-        return bytes(f'------WebKitFormBoundary{get_random_string(16)}', "utf-8")
-
-    def _initiate_upload(self):
-        response = self._client.http.upload_media_init(self.size, self.mime_type, self._media_category, source_url=self._source_url)
-        return response['media_id_string']
-
-    def _append_upload(self, media_id):
-        with open(self._file, "rb") as f:
-            segments, remainder = divmod(self.size, self.FILE_CHUNK_SIZE)
-            segments += bool(remainder)
-
-            for segment_index in range(segments):
-                boundary = self._create_boundary()
-                headers, multipart = encode_multipart_data({}, {"media": ('blob', f.read(self.FILE_CHUNK_SIZE), "application/octet-stream")}, boundary)
-                self._client.http.upload_media_append(media_id, multipart, headers, segment_index)
-
-    def set_metadata(self):
-        self._client.http.set_media_set_metadata(self.media_id, self._alt_text, self._sensitive_media_warning)
-
-    def _finish_upload(self, media_id):
-        if not self._source_url:
-            response = self._client.http.upload_media_finalize(media_id, self.md5_hash)
-        else:
-            response = {"processing_info": {"state": "pending", "check_after_secs": 1}}
-
-        if not response.get('processing_info'):
-            return
-
-        while True:
-            processing_info = response['processing_info']
-
-            if processing_info.get('state') in ('pending', 'in_progress') and 'error' not in processing_info:
-                time.sleep(processing_info['check_after_secs'])
-                response = self._client.http.upload_media_status(self.media_id)
-            else:
-                return
-
-    def upload(self):
-        self.media_id = self._initiate_upload()
-
-        if not self._source_url:
-            self._append_upload(self.media_id)
-
-        self._finish_upload(self.media_id)
-
-        if self._alt_text:
-            self.set_metadata()
-
-        return self
-
-
-
-
-
+import datetime
+import os
+import time
+from http.cookiejar import MozillaCookieJar
+from httpx._content import encode_multipart_data
+from .. import constants
+from . import Gif
+from ..utils import calculate_md5, get_random_string, check_if_file_is_image
+from ..exceptions import *
+
+
+class Proxy:
+    def __init__(self, host: str, port: int, proxy_type: int, username: str = None, password: str = None):
+        self.host = host
+        self.password = password
+        self.proxy_type = proxy_type
+        self.username = username
+        self.port = port
+        self.proxy = self.__parse__()
+
+    def __iter__(self):
+        for k, v in self.proxy.items():
+            yield k, v
+
+    def __proxy_url__(self):
+        if self.username and self.password:
+            return "{}:{}@{}:{}".format(
+                self.username, self.password, self.host, self.port
+            )
+        else:
+            return "{}:{}".format(self.host, self.port)
+
+    def __parse__(self):
+        proxy_url = self.__proxy_url__()
+        if self.proxy_type == constants.HTTP:
+            http_url = "http://{}".format(proxy_url)
+            return dict.fromkeys(['http://', 'https://'], http_url)
+        elif self.proxy_type == constants.SOCKS4:
+            socks_url = "socks4://{}".format(proxy_url)
+            return dict.fromkeys(['http://', 'https://'], socks_url)
+        elif self.proxy_type == constants.SOCKS5:
+            socks_url = "socks5://{}".format(proxy_url)
+            return dict.fromkeys(['http://', 'https://'], socks_url)
+
+        raise ProxyParseError()
+
+    def get_dict(self):
+        return self.proxy
+
+
+class GenericError:
+    EXCEPTIONS = {
+        32: InvalidCredentials,
+        144: InvalidTweetIdentifier,
+        88: RateLimitReached,
+        477: RateLimitReached,
+        399: InvalidCredentials,
+        220: InvalidCredentials,
+        214: InvalidBroadcast,
+        366: InvalidTweetIdentifier,
+        326: LockedAccount
+    }
+
+    def __init__(self, response, error_code, message=None):
+        self.response = response
+        self.error_code = error_code
+        self.message = message
+        self.retry_after = self._get_retry_after()
+        self._raise_exception()
+
+    def _get_retry_after(self):
+        if all(key in self.response.headers for key in ['x-rate-limit-reset', 'x-rate-limit-remaining']):
+            epochLimitTime = int(self.response.headers['x-rate-limit-reset'])
+            epochCurrentTime = int(datetime.datetime.now().timestamp())
+            return epochLimitTime - epochCurrentTime
+
+        return None
+
+    def _raise_exception(self):
+        if self.EXCEPTIONS.get(self.error_code):
+            raise self.EXCEPTIONS[self.error_code](
+                error_code=self.error_code,
+                error_name=TWITTER_ERRORS[self.error_code],
+                response=self.response,
+                message=self.message,
+                retry_after=self.retry_after
+            )
+
+        raise TwitterError(
+            error_code=self.error_code,
+            error_name=TWITTER_ERRORS.get(self.error_code, 0),
+            response=self.response,
+            message="[{}] {}".format(self.error_code, self.message)
+        )
+
+
+class Cookies:
+    def __init__(self, cookies, is_http_response=False):
+        self._raw_cookies = cookies
+        self._is_http_response = is_http_response
+        self.parse_cookies()
+
+    def parse_cookies(self):
+        if isinstance(self._raw_cookies, MozillaCookieJar):
+            for i in self._raw_cookies:
+                setattr(self, i.name, i.value)
+        else:
+            if self._is_http_response:
+                # TODO : Find a proper way to parse
+                n = [0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30]
+                for k, p in enumerate(self._raw_cookies.split(",")):
+                    if k in n:
+                        key, value = str(p.split(';')[0]).split("=", 1)
+                        setattr(self, key.strip(), value.strip())
+            else:
+                true_cookies = dict()
+                if isinstance(self._raw_cookies, str):
+                    cookie_list = self._raw_cookies.split(";")
+                    for cookie in cookie_list:
+                        split_cookie = cookie.strip().split("=", 1)
+
+                        if len(split_cookie) >= 2:
+                            cookie_key = split_cookie[0]
+                            cookie_value = split_cookie[1]
+                            true_cookies[cookie_key] = cookie_value
+                elif isinstance(self._raw_cookies, dict):
+                    true_cookies = self._raw_cookies
+                else:
+                    raise TypeError("cookies should be of class 'str', 'dict' or 'MozillaCookieJar' not {}".format(self._raw_cookies.__class__))
+
+                for key, value in true_cookies.items():
+                    setattr(self, key.strip(), value.strip())
+
+    def to_dict(self):
+        result = {}
+        for k, v in vars(self).items():
+
+            if not k.startswith("_"):
+                result[k] = v
+
+        return result
+
+    def __str__(self):
+        string = ""
+        for k, v in vars(self).items():
+
+            if not k.startswith("_"):
+                string += f"{k}={v};"
+
+        return string
+
+
+class UploadedMedia:
+    FILE_CHUNK_SIZE = 2 * 1024 * 1024  # 2 mb
+
+    def __init__(
+            self,
+            file_path,
+            client,
+            alt_text=None,
+            sensitive_media_warning=None,
+            media_category="tweet_image"
+    ):
+        self.media_id = None
+        self._file = file_path
+        self._client = client
+        self._alt_text = alt_text
+        self._sensitive_media_warning = sensitive_media_warning if sensitive_media_warning else []
+        self._source_url = self._get_source_url()
+        self.size = self._get_size()
+        self.mime_type = self.get_mime_type()
+        self._media_category = self._get_media_category(media_category)
+        self.md5_hash = calculate_md5(self._file)
+
+    def _get_source_url(self):
+        if isinstance(self._file, Gif):
+            return self._file.url
+        elif str(self._file).startswith("https://"):
+            return self._file
+
+        return None
+
+    def _get_media_category(self, category):
+        media_for = category.split("_")[0]
+        media_type = self.mime_type.split("/")[0]
+        return f"{media_for}_{media_type}" if "gif" not in self.mime_type else f"{media_for}_gif"
+
+    def _get_size(self):
+        if not self._source_url:
+            return os.path.getsize(self._file)
+        return 0
+
+    def get_mime_type(self):
+        return check_if_file_is_image(self._file)
+
+    @staticmethod
+    def _create_boundary():
+        return bytes(f'------WebKitFormBoundary{get_random_string(16)}', "utf-8")
+
+    def _initiate_upload(self):
+        response = self._client.http.upload_media_init(self.size, self.mime_type, self._media_category, source_url=self._source_url)
+        return response['media_id_string']
+
+    def _append_upload(self, media_id):
+        with open(self._file, "rb") as f:
+            segments, remainder = divmod(self.size, self.FILE_CHUNK_SIZE)
+            segments += bool(remainder)
+
+            for segment_index in range(segments):
+                boundary = self._create_boundary()
+                headers, multipart = encode_multipart_data({}, {"media": ('blob', f.read(self.FILE_CHUNK_SIZE), "application/octet-stream")}, boundary)
+                self._client.http.upload_media_append(media_id, multipart, headers, segment_index)
+
+    def set_metadata(self):
+        self._client.http.set_media_set_metadata(self.media_id, self._alt_text, self._sensitive_media_warning)
+
+    def _finish_upload(self, media_id):
+        if not self._source_url:
+            response = self._client.http.upload_media_finalize(media_id, self.md5_hash)
+        else:
+            response = {"processing_info": {"state": "pending", "check_after_secs": 1}}
+
+        if not response.get('processing_info'):
+            return
+
+        while True:
+            processing_info = response['processing_info']
+
+            if processing_info.get('state') in ('pending', 'in_progress') and 'error' not in processing_info:
+                time.sleep(processing_info['check_after_secs'])
+                response = self._client.http.upload_media_status(self.media_id)
+            else:
+                return
+
+    def upload(self):
+        self.media_id = self._initiate_upload()
+
+        if not self._source_url:
+            self._append_upload(self.media_id)
+
+        self._finish_upload(self.media_id)
+
+        if self._alt_text:
+            self.set_metadata()
+
+        return self
+
+
+
+
+
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/notification.py` & `tweety_ns-1.1.6/src/tweety/types/notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .base import BaseGeneratorClass
-from . import *
+from .twDataTypes import Tweet
 
 
 class TweetNotifications(BaseGeneratorClass):
     _RESULT_ATTR = "tweets"
 
     def __init__(self, user_id, client, pages=1, wait_time=2, cursor=None):
         super().__init__()
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/places.py` & `tweety_ns-1.1.6/src/tweety/types/places.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import Place
+from .twDataTypes import Place
 
 
 class Places(dict):
     def __init__(self, client, lat, long, search_term):
         super().__init__()
         self.lat = lat
         self.client = client
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/retweets.py` & `tweety_ns-1.1.6/src/tweety/types/retweets.py`

 * *Files identical despite different names*

### Comparing `tweety_ns-1.1.5/src/tweety/types/search.py` & `tweety_ns-1.1.6/src/tweety/types/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import traceback
-
 from . import Tweet, Excel, User, List
 from .base import BaseGeneratorClass
 from .twDataTypes import SelfThread
 
 
 class Search(BaseGeneratorClass):
     OBJECTS_TYPES = {
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/topic.py` & `tweety_ns-1.1.6/src/tweety/types/topic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .base import BaseGeneratorClass
-from . import Topic, Tweet
+from .twDataTypes import Topic, Tweet
 
 
 class TopicTweets(BaseGeneratorClass):
     _RESULT_ATTR = "tweets"
 
     def __init__(self, topic_id, client, pages=1, cursor=None, wait_time=2):
         super().__init__()
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/twDataTypes.py` & `tweety_ns-1.1.6/src/tweety/types/twDataTypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os.path
 import html
 import warnings
 from typing import Callable, Union
 from dateutil import parser
 import openpyxl
 import dateutil
-from ..exceptions_ import UserNotFound, UserProtected, ProtectedTweet
+from ..constants import MEDIA_TYPE_VIDEO, MEDIA_TYPE_GIF, MEDIA_TYPE_IMAGE
+from ..exceptions import UserNotFound, UserProtected, ProtectedTweet
 from ..utils import *
 
 
 def deprecated(func):
     """
 
     This is a decorator which can be used to mark functions
@@ -91,48 +92,44 @@
         return 1
 
     def _set_headers(self):
         for index, value in enumerate(WORKBOOK_HEADERS, start=1):
             self.worksheet.cell(row=1, column=index).value = value
 
     def _write_tweet(self, tweet):
-        self.worksheet[f'A{self.max_row + 1}'] = tweet.date
+        self.worksheet[f'A{self.max_row + 1}'] = tweet.date.replace(tzinfo=None)
         self.worksheet[f'B{self.max_row + 1}'] = tweet.author.name
         self.worksheet[f'C{self.max_row + 1}'] = tweet.id
         self.worksheet[f'D{self.max_row + 1}'] = tweet.text
         self.worksheet[f'E{self.max_row + 1}'] = tweet.is_retweet
         self.worksheet[f'F{self.max_row + 1}'] = tweet.is_reply
         self.worksheet[f'G{self.max_row + 1}'] = tweet.language
         self.worksheet[f'H{self.max_row + 1}'] = tweet.likes
         self.worksheet[f'I{self.max_row + 1}'] = tweet.retweet_counts
         self.worksheet[f'J{self.max_row + 1}'] = tweet.source
-        self.worksheet[f'K{self.max_row + 1}'] = ",".join(
-            [media.expanded_url for media in tweet.media]) if tweet.media else ""
-        self.worksheet[f'L{self.max_row + 1}'] = ",".join(
-            [user_mention.screen_name for user_mention in tweet.user_mentions]) if tweet.user_mentions else ""
-        self.worksheet[f'M{self.max_row + 1}'] = ",".join(
-            [url['expanded_url'] for url in tweet.urls]) if tweet.urls else ""
-        self.worksheet[f'N{self.max_row + 1}'] = ",".join(
-            [hashtag['text'] for hashtag in tweet.hashtags]) if tweet.hashtags else ""
-        self.worksheet[f'O{self.max_row + 1}'] = ",".join([symbol for symbol in tweet.symbols]) if tweet.symbols else ""
+        self.worksheet[f'K{self.max_row + 1}'] = iterable_to_string(tweet.media, ",", "direct_url")
+        self.worksheet[f'L{self.max_row + 1}'] = iterable_to_string(tweet.user_mentions, ",", "screen_name")
+        self.worksheet[f'M{self.max_row + 1}'] = iterable_to_string(tweet.urls, ",", "expanded_url")
+        self.worksheet[f'N{self.max_row + 1}'] = iterable_to_string(tweet.hashtags, ",", "text")
+        self.worksheet[f'O{self.max_row + 1}'] = iterable_to_string(tweet.symbols, ",", "text")
         self.max_row += 1
 
     def _write_data(self):
         for tweet in self.tweets:
             if isinstance(tweet, Tweet):
                 self._write_tweet(tweet)
             elif isinstance(tweet, SelfThread):
                 for _threadedTweet in tweet:
                     self._write_tweet(_threadedTweet)
 
         if not self.filename:
             self.filename = f"tweets-{self.author}.xlsx"
 
         try:
-            self.workbook.remove("sheet")
+            self.workbook.remove(self.workbook["Sheet"])
         except ValueError:
             pass
 
         self.workbook.save(self.filename)
 
 
 class EditControl(_TwType):
@@ -243,15 +240,15 @@
     def get_comments(self, pages=1, wait_time=2, cursor=None, get_hidden=False):
         return self._client.get_tweet_comments(self.id, pages, wait_time, cursor, get_hidden)
 
     def iter_comments(self, pages=1, wait_time=2, cursor=None, get_hidden=False):
         return self._client.iter_tweet_comments(self.id, pages, wait_time, cursor, get_hidden)
 
     def _check_if_protected(self):
-        is_protected = find_objects(self._raw, "__typename", ["TweetUnavailable", "TweetTombstone"], recursive=False)
+        is_protected = is_tweet_protected(self._raw)
 
         if is_protected and is_protected.get('reason') == "Protected":
             raise ProtectedTweet(403, "TweetUnavailable", response=self._raw)
         elif is_protected and is_protected.get('reason') == "NsfwLoggedOut":
             raise AuthenticationRequired(401, "NsfwLoggedOut", response=self._raw, message="This Tweet is flagged as NSFW, make sure you are logged-in and brithday is updated in your account.")
         elif is_protected and is_protected.get('reason') == "Suspended":
             raise UserProtected(error_code="UserSuspended", response=self._raw, message="The Author of this Tweet is Suspended")
@@ -834,15 +831,15 @@
         self.sizes = [MediaSize(self._client, v, k) for k, v in self._raw.get("sizes", {}).items() if
                       self._raw.get('sizes')]
         self.original_info = self._raw.get("original_info")
         self.file_format = self._get_file_format()
         self.source_user = self._get_source_user()
         self.streams = []
 
-        if self.type == "video" or self.type == "animated_gif":
+        if self.type in (MEDIA_TYPE_VIDEO, MEDIA_TYPE_GIF):
             self._parse_video_streams()
 
     def __eq__(self, other):
         if isinstance(other, Media):
             return self.id == other.id
         elif isinstance(other, (int, str)):
             return str(self.id) == str(other)
@@ -851,38 +848,38 @@
 
     def _get_direct_url(self):
         url = self._raw.get("media_url_https")
         return url
 
     def _get_file_format(self):
         filename = os.path.basename(self.media_url_https).split("?")[0]
-        return filename.split(".")[-1] if self.type == "photo" else "mp4"
+        return filename.split(".")[-1] if self.type == MEDIA_TYPE_IMAGE else "mp4"
 
     def _parse_video_streams(self):
         videoDict = self._raw.get("video_info")
 
         if not videoDict:
             return
 
         for i in videoDict.get("variants"):
             if not i.get("content_type").split("/")[-1] == "x-mpegURL":
                 self.streams.append(Stream(self._client, i, videoDict.get("duration_millis", 0), videoDict.get("aspect_ratio")))
 
     def best_stream(self):
-        if self.type == "photo":
+        if self.type == MEDIA_TYPE_IMAGE:
             return self
-        elif self.type == "video":
+        elif self.type == MEDIA_TYPE_VIDEO:
             _res = [eval(stream.res) for stream in self.streams if stream.res]
             max_res = max(_res)
             for stream in self.streams:
                 if eval(stream.res) == max_res:
                     file_format = stream.content_type.split("/")[-1]
                     if not file_format == "x-mpegURL":
                         return stream
-        elif self.type == "animated_gif":
+        elif self.type == MEDIA_TYPE_GIF:
             for stream in self.streams:
                 file_format = stream.content_type.split("/")[-1]
                 if not file_format == "x-mpegURL":
                     return stream
         return None
 
     def __repr__(self):
```

### Comparing `tweety_ns-1.1.5/src/tweety/types/usertweet.py` & `tweety_ns-1.1.6/src/tweety/types/usertweet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from .twDataTypes import SelfThread, ConversationThread
-from ..exceptions_ import UserProtected, UserNotFound
-from . import Tweet, Excel
+from .twDataTypes import SelfThread, ConversationThread, Tweet, Excel
+from ..exceptions import UserProtected, UserNotFound
 from .base import BaseGeneratorClass, find_objects
 
 
 class UserTweets(BaseGeneratorClass):
     OBJECTS_TYPES = {
         "tweet": Tweet,
         "homeConversation": SelfThread,
```

### Comparing `tweety_ns-1.1.5/src/tweety/user.py` & `tweety_ns-1.1.6/src/tweety/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Union, Tuple, List
-from .exceptions_ import ListNotFound
+from .exceptions import ListNotFound
 from .types.inbox import Message, Conversation
 from .utils import create_conversation_id, AuthRequired, find_objects, get_tweet_id
 from .types import (User, Mention, Inbox, UploadedMedia, SendMessage, Tweet, Bookmarks, SelfTimeline, TweetLikes,
                     TweetRetweets, Poll, Choice, TweetNotifications, Lists, List as TwList, ListMembers, ListTweets,
                     Topic, TopicTweets, MutualFollowers, HOME_TIMELINE_TYPE_FOR_YOU, TweetAnalytics, BlockedUsers,
                     ShortUser, Place, INBOX_PAGE_TYPE_TRUSTED)
-from .filters import SearchFilters
 
 
 @AuthRequired
 class UserMethods:
 
     @property
     def me(self) -> User:
```

### Comparing `tweety_ns-1.1.5/src/tweety/utils.py` & `tweety_ns-1.1.6/src/tweety/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,241 +1,263 @@
-import base64
-import datetime
-import hashlib
-import inspect
-import json
-import os.path
-import random
-import re
-import string
-import sys
-import uuid
-from dateutil import parser as date_parser
-from urllib.parse import urlparse
-from .exceptions_ import AuthenticationRequired
-from .filters import Language
-
-GUEST_TOKEN_REGEX = re.compile("gt=(.*?);")
-MIME_TYPES = {
-    "png": "image/png",
-    "jpg": "image/jpeg",
-    "jfif": "image/jpeg",
-    "jpeg": "image/jpeg",
-    "gif": "image/gif",
-    "webp": "image/webp",
-    "mp4": "video/mp4",
-    "mov": "video/quicktime",
-    "m4v": "video/x-m4v"
-}
-
-WORKBOOK_HEADERS = ['Date', 'Author', 'id', 'text', 'is_retweet', 'is_reply', 'language', 'likes',
-                    'retweet_count', 'source', 'medias', 'user_mentioned', 'urls', 'hashtags', 'symbols']
-
-SENSITIVE_MEDIA_TAGS = ['adult_content', 'graphic_violence', 'other']
-
-
-def AuthRequired(cls):
-    def method_wrapper_decorator(func):
-        def wrapper(self, *args, **kwargs):
-            if self.me is None:
-                raise AuthenticationRequired(200, "GenericForbidden", None)
-
-            return func(self, *args, **kwargs)
-
-        return wrapper
-
-    if inspect.isclass(cls):
-        for name, method in vars(cls).items():
-            if name != "__init__" and callable(method):
-                setattr(cls, name, method_wrapper_decorator(method))
-        return cls
-    return method_wrapper_decorator(cls)
-
-
-def replace_between_indexes(original_string, from_index, to_index, replacement_text):
-    new_string = original_string[:from_index] + replacement_text + original_string[to_index:]
-    return new_string
-
-
-def decodeBase64(encoded_string):
-    return str(base64.b64decode(bytes(encoded_string, "utf-8")))[2:-1]
-
-
-def bar_progress(filename, total, current, width=80):
-    progress_message = f"[{filename}] Downloading: %d%% [%d / %d] bytes" % (current / total * 100, current, total)
-    sys.stdout.write("\r" + progress_message)
-    sys.stdout.flush()
-
-
-def parse_wait_time(wait_time):
-    if not wait_time:
-        return 0
-
-    if isinstance(wait_time, (tuple, list)):
-        return random.randint(*wait_time)
-
-    return int(wait_time)
-
-
-def get_next_index(iterable, current_index, __default__=None):
-    try:
-        _ = iterable[current_index + 1]
-        return current_index + 1
-    except IndexError:
-        return __default__
-
-def custom_json(self, **kwargs):
-    try:
-        return json.loads(self.content, **kwargs)
-    except:
-        return None
-
-
-def create_request_id():
-    return str(uuid.uuid1())
-
-
-def create_conversation_id(sender, receiver):
-    sender = int(sender)
-    receiver = int(receiver)
-
-    if sender > receiver:
-        return f"{receiver}-{sender}"
-    else:
-        return f"{sender}-{receiver}"
-
-
-def create_query_id():
-    return get_random_string(22)
-
-
-def check_if_file_is_image(file):
-    if not os.path.exists(file) and not str(file).startswith("https://"):
-        raise ValueError("Path {} doesn't exists".format(file))
-
-    file = file.split("?")[0]
-    file_extension = file.split(".")[-1]
-
-    if file_extension not in list(MIME_TYPES.keys()):
-        raise ValueError("File Extension '{}' is not supported. Use any of {}".format(
-            file_extension, list(MIME_TYPES.keys())
-        ))
-
-    return MIME_TYPES[file_extension]
-
-
-def get_random_string(length):
-    return ''.join(random.choices(string.ascii_letters + string.digits, k=int(length)))
-
-
-def calculate_md5(file_path):
-    if str(file_path).startswith("https://"):
-        return None
-
-    md5_hash = hashlib.md5()
-    with open(file_path, "rb") as file:
-        for chunk in iter(lambda: file.read(4096), b""):
-            md5_hash.update(chunk)
-    return md5_hash.hexdigest()
-
-
-def create_media_entities(files):
-    entities = []
-    for file in files:
-        media_id = file.media_id if hasattr(file, "media_id") else file
-        entities.append({
-            "media_id": media_id,
-            "tagged_users": []
-        })
-
-    return entities
-
-
-def check_sensitive_media_tags(tags):
-    return [tag for tag in tags if tag in SENSITIVE_MEDIA_TAGS]
-
-
-def find_objects(obj, key, value, recursive=True, none_value=None):
-    results = []
-
-    def find_matching_objects(_obj, _key, _value):
-        if isinstance(_obj, dict):
-            if _key in _obj:
-                found = False
-                if _value is None:
-                    found = True
-                    results.append(_obj[_key])
-                elif (isinstance(_value, list) and _obj[_key] in _value) or _obj[_key] == _value:
-                    found = True
-                    results.append(_obj)
-
-                if not recursive and found:
-                    return results[0]
-
-            for sub_obj in _obj.values():
-                find_matching_objects(sub_obj, _key, _value)
-        elif isinstance(_obj, list):
-            for item in _obj:
-                find_matching_objects(item, _key, _value)
-
-    find_matching_objects(obj, key, value)
-
-    if len(results) == 1:
-        return results[0]
-
-    if len(results) == 0:
-        return none_value
-
-    if not recursive:
-        return results[0]
-
-    return results
-
-
-def create_pool(duration: int, *choices):
-    data = {
-        "twitter:long:duration_minutes": duration,
-        "twitter:api:api:endpoint": "1",
-        "twitter:card": f"poll{len(choices)}choice_text_only"
-    }
-
-    for index, choice in enumerate(choices, start=1):
-        key = f"twitter:string:choice{index}_label"
-        data[key] = choice
-
-    return data
-
-
-def parse_time(time):
-    if not time:
-        return None
-
-    if isinstance(time, int) or str(time).isdigit():
-        try:
-            return datetime.datetime.fromtimestamp(int(time))
-        except (OSError, ValueError):
-            return datetime.datetime.fromtimestamp(int(time) / 1000)
-
-    return date_parser.parse(time)
-
-
-def get_user_from_typehead(target_username, users):
-    for user in users:
-        if str(user.username).lower() == str(target_username).lower():
-            return user
-    return None
-
-
-def get_tweet_id(tweet_identifier):
-    if str(tweet_identifier.__class__.__name__) == "Tweet":
-        return tweet_identifier.id
-    else:
-        return urlparse(str(tweet_identifier)).path.split("/")[-1]
-
-
-def check_translation_lang(lang):
-    for k, v in vars(Language).items():
-        if not str(k).startswith("_"):
-            if str(k).lower() == str(lang).lower() or str(v).lower() == str(lang).lower():
-                return v
-
-    raise ValueError(f"Language {lang} is not supported")
+import base64
+import datetime
+import hashlib
+import inspect
+import json
+import os.path
+import random
+import re
+import string
+import sys
+import uuid
+from typing import Union
+from dateutil import parser as date_parser
+from urllib.parse import urlparse
+from .exceptions import AuthenticationRequired
+from .filters import Language
+
+GUEST_TOKEN_REGEX = re.compile("gt=(.*?);")
+MIME_TYPES = {
+    "png": "image/png",
+    "jpg": "image/jpeg",
+    "jfif": "image/jpeg",
+    "jpeg": "image/jpeg",
+    "gif": "image/gif",
+    "webp": "image/webp",
+    "mp4": "video/mp4",
+    "mov": "video/quicktime",
+    "m4v": "video/x-m4v"
+}
+
+WORKBOOK_HEADERS = ['Date', 'Author', 'id', 'text', 'is_retweet', 'is_reply', 'language', 'likes',
+                    'retweet_count', 'source', 'medias', 'user_mentioned', 'urls', 'hashtags', 'symbols']
+
+SENSITIVE_MEDIA_TAGS = ['adult_content', 'graphic_violence', 'other']
+
+
+def AuthRequired(cls):
+    def method_wrapper_decorator(func):
+        def wrapper(self, *args, **kwargs):
+            if self.me is None:
+                raise AuthenticationRequired(200, "GenericForbidden", None)
+
+            return func(self, *args, **kwargs)
+
+        return wrapper
+
+    if inspect.isclass(cls):
+        for name, method in vars(cls).items():
+            if name != "__init__" and callable(method):
+                setattr(cls, name, method_wrapper_decorator(method))
+        return cls
+    return method_wrapper_decorator(cls)
+
+
+def replace_between_indexes(original_string, from_index, to_index, replacement_text):
+    new_string = original_string[:from_index] + replacement_text + original_string[to_index:]
+    return new_string
+
+
+def decodeBase64(encoded_string):
+    return str(base64.b64decode(bytes(encoded_string, "utf-8")))[2:-1]
+
+
+def bar_progress(filename, total, current, width=80):
+    progress_message = f"[{filename}] Downloading: %d%% [%d / %d] bytes" % (current / total * 100, current, total)
+    sys.stdout.write("\r" + progress_message)
+    sys.stdout.flush()
+
+
+def parse_wait_time(wait_time):
+    if not wait_time:
+        return 0
+
+    if isinstance(wait_time, (tuple, list)):
+
+        if len(wait_time) == 1:
+            return int(wait_time[0])
+
+        wait_time = [int(i) for i in wait_time[:2]]
+        return random.randint(*wait_time)
+
+    return int(wait_time)
+
+
+def get_next_index(iterable, current_index, __default__=None):
+    try:
+        _ = iterable[current_index + 1]
+        return current_index + 1
+    except IndexError:
+        return __default__
+
+
+def custom_json(self, **kwargs):
+    try:
+        return json.loads(self.content, **kwargs)
+    except:
+        return None
+
+
+def create_request_id():
+    return str(uuid.uuid1())
+
+
+def create_conversation_id(sender, receiver):
+    sender = int(sender)
+    receiver = int(receiver)
+
+    if sender > receiver:
+        return f"{receiver}-{sender}"
+    else:
+        return f"{sender}-{receiver}"
+
+
+def create_query_id():
+    return get_random_string(22)
+
+
+def check_if_file_is_image(file):
+    if not str(file).startswith("https://") and not os.path.exists(file):
+        raise ValueError("Path {} doesn't exists".format(file))
+
+    file = file.split("?")[0]
+    file_extension = file.split(".")[-1]
+
+    if file_extension not in list(MIME_TYPES.keys()):
+        raise ValueError("File Extension '{}' is not supported. Use any of {}".format(
+            file_extension, list(MIME_TYPES.keys())
+        ))
+
+    return MIME_TYPES[file_extension]
+
+
+def get_random_string(length):
+    return ''.join(random.choices(string.ascii_letters + string.digits, k=int(length)))
+
+
+def calculate_md5(file_path):
+    if str(file_path).startswith("https://"):
+        return None
+
+    md5_hash = hashlib.md5()
+    with open(file_path, "rb") as file:
+        for chunk in iter(lambda: file.read(4096), b""):
+            md5_hash.update(chunk)
+    return md5_hash.hexdigest()
+
+
+def create_media_entities(files):
+    entities = []
+    for file in files:
+        media_id = file.media_id if hasattr(file, "media_id") else file
+        entities.append({
+            "media_id": media_id,
+            "tagged_users": []
+        })
+
+    return entities
+
+
+def check_sensitive_media_tags(tags):
+    return [tag for tag in tags if tag in SENSITIVE_MEDIA_TAGS]
+
+
+def find_objects(obj, key, value, recursive=True, none_value=None):
+    results = []
+
+    def find_matching_objects(_obj, _key, _value):
+        if isinstance(_obj, dict):
+            if _key in _obj:
+                found = False
+                if _value is None:
+                    found = True
+                    results.append(_obj[_key])
+                elif (isinstance(_value, list) and _obj[_key] in _value) or _obj[_key] == _value:
+                    found = True
+                    results.append(_obj)
+
+                if not recursive and found:
+                    return results[0]
+
+            for sub_obj in _obj.values():
+                find_matching_objects(sub_obj, _key, _value)
+        elif isinstance(_obj, list):
+            for item in _obj:
+                find_matching_objects(item, _key, _value)
+
+    find_matching_objects(obj, key, value)
+
+    if len(results) == 1:
+        return results[0]
+
+    if len(results) == 0:
+        return none_value
+
+    if not recursive:
+        return results[0]
+
+    return results
+
+
+def create_pool(duration: int, *choices):
+    data = {
+        "twitter:long:duration_minutes": duration,
+        "twitter:api:api:endpoint": "1",
+        "twitter:card": f"poll{len(choices)}choice_text_only"
+    }
+
+    for index, choice in enumerate(choices, start=1):
+        key = f"twitter:string:choice{index}_label"
+        data[key] = choice
+
+    return data
+
+
+def parse_time(time):
+    if not time:
+        return None
+
+    if isinstance(time, int) or str(time).isdigit():
+        try:
+            return datetime.datetime.fromtimestamp(int(time))
+        except (OSError, ValueError):
+            return datetime.datetime.fromtimestamp(int(time) / 1000)
+
+    return date_parser.parse(time)
+
+
+def get_user_from_typehead(target_username, users):
+    for user in users:
+        if str(user.username).lower() == str(target_username).lower():
+            return user
+    return None
+
+
+def get_tweet_id(tweet_identifier):
+    if str(tweet_identifier.__class__.__name__) == "Tweet":
+        return tweet_identifier.id
+    else:
+        return urlparse(str(tweet_identifier)).path.split("/")[-1]
+
+
+def is_tweet_protected(raw):
+    return find_objects(raw, "__typename", ["TweetUnavailable", "TweetTombstone"], recursive=False)
+
+
+def check_translation_lang(lang):
+    for k, v in vars(Language).items():
+        if not str(k).startswith("_"):
+            if str(k).lower() == str(lang).lower() or str(v).lower() == str(lang).lower():
+                return v
+
+    raise ValueError(f"Language {lang} is not supported")
+
+
+def iterable_to_string(__iterable__: Union[list, tuple], __delimiter__: str = ",", __attr__: str = None):
+    if not isinstance(__iterable__, (list, tuple)) or len(__iterable__) == 0:
+        return ""
+
+    if __attr__:
+        __iterable__ = [str(getattr(i, __attr__)) for i in __iterable__]
+
+    return __delimiter__.join(__iterable__)
+
```

### Comparing `tweety_ns-1.1.5/src/tweety_ns.egg-info/PKG-INFO` & `tweety_ns-1.1.6/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.5
+Version: 1.1.6
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety_ns-1.1.5/src/tweety_ns.egg-info/SOURCES.txt` & `tweety_ns-1.1.6/src/tweety_ns.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/tweety/__init__.py
 src/tweety/auth.py
 src/tweety/bot.py
 src/tweety/builder.py
+src/tweety/constants.py
+src/tweety/exceptions.py
 src/tweety/exceptions_.py
 src/tweety/filters.py
 src/tweety/http.py
 src/tweety/session.py
 src/tweety/updates.py
 src/tweety/user.py
 src/tweety/utils.py
```

