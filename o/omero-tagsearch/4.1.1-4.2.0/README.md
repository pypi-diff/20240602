# Comparing `tmp/omero-tagsearch-4.1.1.tar.gz` & `tmp/omero-tagsearch-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-tagsearch-4.1.1.tar", last modified: Fri Apr 26 13:34:40 2024, max compression
+gzip compressed data, was "omero-tagsearch-4.2.0.tar", last modified: Sun Jun  2 13:14:37 2024, max compression
```

## Comparing `omero-tagsearch-4.1.1.tar` & `omero-tagsearch-4.2.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.090764 omero-tagsearch-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-26 13:34:40.090764 omero-tagsearch-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.082764 omero-tagsearch-4.1.1/omero_tagsearch/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.078764 omero-tagsearch-4.1.1/omero_tagsearch/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.078764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.082764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.082764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.js
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.086764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/
--rwxr-xr-x   0 runner    (1001) docker     (127)      646 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      872 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite@2x.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    12936 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    42443 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    26966 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.min.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    10751 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.min.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    42886 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    27375 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.086764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3467 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/chosen.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     6709 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/oss-credit.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.css
--rwxr-xr-x   0 runner    (1001) docker     (127)     6659 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     6928 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/style.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    85742 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)    86196 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.proto.html
--rwxr-xr-x   0 runner    (1001) docker     (127)    12053 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/options.html
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen.order.jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)    43811 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/jquery.form.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.086764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/css/
--rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/css/webtagging_search.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.086764 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder_image16.png
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder_plate16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder_screen16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/icon_user.png
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/image16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/run16.png
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/well16.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.078764 omero-tagsearch-4.1.1/omero_tagsearch/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.090764 omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/search_details.html
--rw-r--r--   0 runner    (1001) docker     (127)    14273 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/tagnav.html
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/tagnav_init.js.html
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    18192 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/omero_tagsearch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:34:40.082764 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-26 13:34:39.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-26 13:34:40.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:34:39.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:34:39.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 13:34:39.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 13:34:39.000000 omero-tagsearch-4.1.1/omero_tagsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-26 13:34:40.090764 omero-tagsearch-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-26 13:34:32.000000 omero-tagsearch-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.605001 omero-tagsearch-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-06-02 13:14:37.605001 omero-tagsearch-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.597001 omero-tagsearch-4.2.0/omero_tagsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.593001 omero-tagsearch-4.2.0/omero_tagsearch/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.593001 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.597001 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.597001 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.601001 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      646 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      872 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite@2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12936 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42443 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26966 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10751 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.min.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42886 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27375 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.601001 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3467 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/chosen.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6709 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/oss-credit.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6659 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6928 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/style.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    85742 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)    86196 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.proto.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12053 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/options.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen.order.jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43811 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/jquery.form.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.601001 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/css/webtagging_search.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.601001 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/folder16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/folder_image16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/folder_plate16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/folder_screen16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/icon_user.png
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/image16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/run16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/well16.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.593001 omero-tagsearch-4.2.0/omero_tagsearch/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.605001 omero-tagsearch-4.2.0/omero_tagsearch/templates/omero_tagsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/templates/omero_tagsearch/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/templates/omero_tagsearch/search_details.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14272 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/templates/omero_tagsearch/tagnav.html
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/templates/omero_tagsearch/tagnav_init.js.html
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/omero_tagsearch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:14:37.597001 omero-tagsearch-4.2.0/omero_tagsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-06-02 13:14:37.000000 omero-tagsearch-4.2.0/omero_tagsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-06-02 13:14:37.000000 omero-tagsearch-4.2.0/omero_tagsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 13:14:37.000000 omero-tagsearch-4.2.0/omero_tagsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 13:14:37.000000 omero-tagsearch-4.2.0/omero_tagsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-02 13:14:37.000000 omero-tagsearch-4.2.0/omero_tagsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 13:14:37.000000 omero-tagsearch-4.2.0/omero_tagsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-02 13:14:37.605001 omero-tagsearch-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-06-02 13:14:34.000000 omero-tagsearch-4.2.0/setup.py
```

### Comparing `omero-tagsearch-4.1.1/LICENSE.txt` & `omero-tagsearch-4.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/PKG-INFO` & `omero-tagsearch-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: omero-tagsearch
-Version: 4.1.1
+Version: 4.2.0
 Summary: OMERO webtagging tagsearch app
 Home-page: https://github.com/German-BioImaging/omero-tagsearch
 Author: D.P.W. Russell
 Author-email: dpwrussell@gmail.com
 Maintainer: Tom Boissonnet
 Maintainer-email: tom.boissonnet@hhu.de
 License: AGPL-3.0
-Download-URL: https://github.com/German-BioImaging/omero-tagsearch/archive/v4.1.1.tar.gz
+Download-URL: https://github.com/German-BioImaging/omero-tagsearch/archive/v4.2.0.tar.gz
 Keywords: OMERO.web,webtagging,tagsearch
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omero-tagsearch-4.1.1/README.rst` & `omero-tagsearch-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/forms.py` & `omero-tagsearch-4.2.0/omero_tagsearch/forms.py`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.js` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.min.js` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/arrayUtilities/jquery.arrayUtilities.min.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite.png` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite@2x.png` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.css` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.css`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.js` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.min.js` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.min.css` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.min.css`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.js` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.min.js` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/chosen.proto.min.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/chosen.png` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/chosen.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/oss-credit.png` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/oss-credit.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.css` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.css`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.js` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/prism.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/style.css` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/docsupport/style.css`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.html` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.html`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.proto.html` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/index.proto.html`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen/options.html` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen/options.html`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/chosen.order.jquery.js` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/chosen.order.jquery.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/3rd-party/jquery.form.js` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/3rd-party/jquery.form.js`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/css/bootstrap.css` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/css/webtagging_search.css` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/css/webtagging_search.css`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder16.png` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/folder16.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder_image16.png` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/folder_image16.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/folder_screen16.png` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/folder_screen16.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/icon_user.png` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/icon_user.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/run16.png` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/run16.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/static/tagsearch/image/well16.png` & `omero-tagsearch-4.2.0/omero_tagsearch/static/tagsearch/image/well16.png`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/search_details.html` & `omero-tagsearch-4.2.0/omero_tagsearch/templates/omero_tagsearch/search_details.html`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/tagnav.html` & `omero-tagsearch-4.2.0/omero_tagsearch/templates/omero_tagsearch/tagnav.html`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 {% include "webclient/base/includes/group_user_dropdown.html" %}
 
 </div>
 
 
 <div id="searching">
   <div class="left_panel_inner">
-      <form id="tagSearchForm" action="{% url 'wtsimages' %}" method="post" class="standard_form">{% csrf_token %}
+      <form id="tagSearchForm" action="{% url 'wtsimages' %}" method="get" class="standard_form">{% csrf_token %}
           <h2>{% trans "Tag Search" %}</h2>
           {# {{ tagnav_form.as_p }} #}
           {{ tagnav_form.non_field_errors }}
 
           {% if user_name %}
             <div id="id_userName" class="tagnav-user">
               <div class="tagnav-icon">&nbsp;</div>
```

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/templates/omero_tagsearch/tagnav_init.js.html` & `omero-tagsearch-4.2.0/omero_tagsearch/templates/omero_tagsearch/tagnav_init.js.html`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch/views.py` & `omero-tagsearch-4.2.0/omero_tagsearch/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,19 +279,19 @@
 # TODO Figure out what happened to render_response as it wasn't working on
 # production
 # @render_response()
 def tag_image_search(request, conn=None, **kwargs):
     import time
 
     start = time.time()
-    if request.method == "POST":
+    if request.method == "GET":
 
-        selected_tags = [int(x) for x in request.POST.getlist("selectedTags")]
-        excluded_tags = [int(x) for x in request.POST.getlist("excludedTags")]
-        operation = request.POST.get("operation")
+        selected_tags = [int(x) for x in request.GET.getlist("selectedTags")]
+        excluded_tags = [int(x) for x in request.GET.getlist("excludedTags")]
+        operation = request.GET.get("operation")
 
         # validate experimenter is in the active group
         active_group = (
             request.session.get("active_group")
             or conn.getEventContext().groupId
         )
         service_opts = conn.SERVICE_OPTS.copy()
```

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch.egg-info/PKG-INFO` & `omero-tagsearch-4.2.0/omero_tagsearch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: omero-tagsearch
-Version: 4.1.1
+Version: 4.2.0
 Summary: OMERO webtagging tagsearch app
 Home-page: https://github.com/German-BioImaging/omero-tagsearch
 Author: D.P.W. Russell
 Author-email: dpwrussell@gmail.com
 Maintainer: Tom Boissonnet
 Maintainer-email: tom.boissonnet@hhu.de
 License: AGPL-3.0
-Download-URL: https://github.com/German-BioImaging/omero-tagsearch/archive/v4.1.1.tar.gz
+Download-URL: https://github.com/German-BioImaging/omero-tagsearch/archive/v4.2.0.tar.gz
 Keywords: OMERO.web,webtagging,tagsearch
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omero-tagsearch-4.1.1/omero_tagsearch.egg-info/SOURCES.txt` & `omero-tagsearch-4.2.0/omero_tagsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omero-tagsearch-4.1.1/setup.py` & `omero-tagsearch-4.2.0/setup.py`

 * *Files identical despite different names*

