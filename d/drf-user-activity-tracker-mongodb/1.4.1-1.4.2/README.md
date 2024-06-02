# Comparing `tmp/drf-user-activity-tracker-mongodb-1.4.1.tar.gz` & `tmp/drf-user-activity-tracker-mongodb-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-user-activity-tracker-mongodb-1.4.1.tar", last modified: Wed Dec 13 06:56:11 2023, max compression
+gzip compressed data, was "drf-user-activity-tracker-mongodb-1.4.2.tar", last modified: Sun Jun  2 12:48:46 2024, max compression
```

## Comparing `drf-user-activity-tracker-mongodb-1.4.1.tar` & `drf-user-activity-tracker-mongodb-1.4.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      780 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/setup.cfg
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       38 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/setup.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       85 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/pyproject.toml
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      382 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/MANIFEST.in
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    13321 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/PKG-INFO
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      732 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/permissions.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templates/
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templates/activity_log/
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templates/activity_log/admin/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9686 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1573 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9626 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/management/
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/management/commands/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      913 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2743 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/views.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2969 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/serializers.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/middleware/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/middleware/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9438 2023-12-13 06:54:45.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/tests.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/geo_databases/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  3039173 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  2315687 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     3815 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/admin.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      169 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/apps.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      600 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templatetags/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      786 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templatetags/tagger.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templatetags/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2893 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/events.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    11642 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/utils.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      325 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/urls.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/migrations/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      557 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/migrations/0001_initial.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/migrations/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      233 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/__init__.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      250 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/models.py
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2270 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/insert_log_into_database.py
-drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb.egg-info/
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        1 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb.egg-info/dependency_links.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       34 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb.egg-info/top_level.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       30 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb.egg-info/requires.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    13321 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb.egg-info/PKG-INFO
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1770 2023-12-13 06:56:11.000000 drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    10495 2023-12-13 06:55:19.000000 drf-user-activity-tracker-mongodb-1.4.1/README.md
--rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1073 2023-06-06 08:19:51.000000 drf-user-activity-tracker-mongodb-1.4.1/LICENSE
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.755200 drf-user-activity-tracker-mongodb-1.4.2/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1073 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/LICENSE
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      382 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/MANIFEST.in
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    10613 2024-06-02 12:48:46.755200 drf-user-activity-tracker-mongodb-1.4.2/PKG-INFO
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    10213 2024-06-02 11:39:21.000000 drf-user-activity-tracker-mongodb-1.4.2/README.md
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.755200 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      233 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     3974 2024-06-02 11:29:25.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/admin.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      169 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/apps.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2893 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/events.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.755200 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/geo_databases/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  2315687 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)  3039173 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2270 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/insert_log_into_database.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.751200 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/management/
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.755200 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/management/commands/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      913 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.755200 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/middleware/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/middleware/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9438 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.755200 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/migrations/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      557 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/migrations/0001_initial.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/migrations/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      250 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/models.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      732 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/permissions.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2969 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/serializers.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      600 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.751200 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templates/
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.751200 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templates/activity_log/
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.755200 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templates/activity_log/admin/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1573 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9686 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     9626 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.755200 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templatetags/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templatetags/__init__.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      786 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templatetags/tagger.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/tests.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      325 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/urls.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    11374 2024-06-02 11:29:39.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/utils.py
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     2743 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/views.py
+drwxrwxr-x   0 bigmo     (1000) bigmo     (1000)        0 2024-06-02 12:48:46.755200 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb.egg-info/
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)    10613 2024-06-02 12:48:46.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb.egg-info/PKG-INFO
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)     1770 2024-06-02 12:48:46.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)        1 2024-06-02 12:48:46.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       30 2024-06-02 12:48:46.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb.egg-info/requires.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       34 2024-06-02 12:48:46.000000 drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb.egg-info/top_level.txt
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       85 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/pyproject.toml
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)      780 2024-06-02 12:48:46.759200 drf-user-activity-tracker-mongodb-1.4.2/setup.cfg
+-rw-rw-r--   0 bigmo     (1000) bigmo     (1000)       38 2024-06-02 11:28:28.000000 drf-user-activity-tracker-mongodb-1.4.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/setup.cfg` & `drf-user-activity-tracker-mongodb-1.4.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-user-activity-tracker-mongodb
-version = 1.4.1
+version = 1.4.2
 description = A Django app to logs users activities in mongodb database.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bigmo94/drf-user-activity-tracker-mongodb
 author = Mohamad Rezaie
 author_email = m.rezaie94@gmail.com
 license = MIT
```

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/permissions.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/permissions.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v2.html`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_detail.html`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templates/activity_log/admin/change_list_v3.html`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/management/commands/get_url_names.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/views.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/views.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/serializers.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/middleware/activity_tracker_middleware.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/geo_databases/GeoIPv6.dat`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/geo_databases/GeoIP.dat`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/admin.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import importlib
+
 from django.conf import settings
 from django import get_version
 from django.contrib import admin
 from django.contrib import messages
 from django.core.paginator import PageNotAnInteger, EmptyPage
 from django.shortcuts import redirect, reverse
 from django.template.response import TemplateResponse
@@ -28,15 +30,18 @@
                 path(r'', self.activity_log_view, name=info),
                 path(r'<str:pk>/change/', self.activity_log_detail_view, name=detail)
             ]
 
         def activity_log_view(self, request):
             params = ParamsHandler(request)
 
-            url_names_list = get_all_url_names()
+            project_urls = f"{settings.ROOT_URLCONF}"
+            urls = getattr(importlib.import_module(project_urls), 'urlpatterns')
+
+            url_names_list = get_all_url_names(urls)
             url_name = params.get_url_name()
             search_value = params.get_search_value()
             status_code = params.get_status()
             time_delta = params.get_time_delta()
 
             data_count = MyCollection().data_count(url_name=url_name, user_id=search_value, status_code=status_code,
                                                    time_delta=time_delta)
@@ -79,7 +84,8 @@
         def activity_log_detail_view(self, request, pk=None):
             data = MyCollection().detail(pk)
             if not data:
                 messages.warning(request, f"Log with ID '{pk}' doesn’t exist. Perhaps it was deleted?")
                 return redirect(reverse('admin:index'))
             context = dict(self.admin_site.each_context(request), data=data)
             return TemplateResponse(request, "activity_log/admin/change_detail.html", context=context)
+
```

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/start_logger_when_server_starts.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/templatetags/tagger.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/templatetags/tagger.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/events.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/events.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/utils.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import collections.abc
-import importlib
 import re
 from math import ceil
 
 from bson import ObjectId
-from django.apps import apps
 from django.conf import settings
 from django.core.paginator import Paginator
+from django.urls import URLPattern, URLResolver
 from django.utils import timezone
 from django.utils.functional import cached_property
 from pymongo import MongoClient
 
 SENSITIVE_KEYS = ['password', 'access', 'refresh']
 if hasattr(settings, 'DRF_ACTIVITY_TRACKER_EXCLUDE_KEYS'):
     if isinstance(settings.DRF_ACTIVITY_TRACKER_EXCLUDE_KEYS, (list, tuple)):
@@ -142,36 +141,27 @@
         try:
             pk = ObjectId(pk)
         except:
             return None
         return self.collection.find_one({'_id': pk})
 
 
-def get_all_url_names():
-    list_of_all_urls = list()
-    list_of_url_name = list()
-    for name, app in apps.app_configs.items():
-        mod_to_import = f'{name}.urls'
-        try:
-            urls = getattr(importlib.import_module(mod_to_import), 'urlpatterns')
-            list_of_all_urls.extend(urls)
-        except ImportError as ex:
-            # is an app without urls
-            pass
-    for url in list_of_all_urls:
-        if hasattr(url, 'name'):
-            if url.name:
-                list_of_url_name.append(url.name)
-
-    if hasattr(settings, 'DRF_ACTIVITY_TRACKER_URL_NAMES'):
-        if isinstance(settings.DRF_ACTIVITY_TRACKER_EXCLUDE_KEYS, (list, tuple)):
-            list_of_url_name.extend(settings.DRF_ACTIVITY_TRACKER_URL_NAMES)
-
-    list_of_url_name.sort()
-    return list_of_url_name
+def get_all_url_names(urlpatterns):
+    """Recursively fetch URL names from urlpatterns."""
+    url_names = []
+
+    for pattern in urlpatterns:
+        if isinstance(pattern, URLPattern):  # A single URL pattern
+            if pattern.name:  # If the URL pattern has a name
+                full_name = pattern.name
+                url_names.append(full_name)
+        elif isinstance(pattern, URLResolver):  # A nested URL resolver
+            url_names.extend(get_all_url_names(pattern.url_patterns))
+    url_names.sort()
+    return url_names
 
 
 class ParamsHandler:
 
     def __init__(self, request):
         self.params = request.GET
 
@@ -332,7 +322,8 @@
     if created_time_after and not created_time_before:
         time_delta = {'$gte': created_time_after}
 
     if created_time_before and not created_time_after:
         time_delta = {'$lte': created_time_before}
 
     return time_delta
+
```

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/migrations/0001_initial.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb/insert_log_into_database.py` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb/insert_log_into_database.py`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt` & `drf-user-activity-tracker-mongodb-1.4.2/drf_user_activity_tracker_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/README.md` & `drf-user-activity-tracker-mongodb-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -295,11 +295,8 @@
 }
 DRF_ACTIVITI_API_LIMIT = 100  #for count of api results, default is 100.
 ```
 #### Prevent user to see some activities in history endpoint
 By default all activities are shown in user history endpoint. you can add specific url name that you don't want to show to the user in `DRF_ACTIVITI_API_UNNECESSARY_URL_NAME` attribute in settings.py and then the user can not be able to see them. 
 Note: This attribute must be a list.
 
-#### Excluding specific url names in django admin panel
-Note: In django admin panel you can filter logs by url name. some url name do not appear in filter list. you can set `DRF_ACTIVITY_TRACKER_URL_NAMES` in settings with the list of url names that you want to be filtered by.
-
```

#### html2text {}

```diff
@@ -123,12 +123,8 @@
 then copy the dictionary to settings.py: ```python
 DRF_ACTIVITY_TRACKER_EVENT_NAME = { 'user_register': 'Registeration', 'orders-
 redeem': 'Redeem Card', } DRF_ACTIVITI_API_LIMIT = 100 #for count of api
 results, default is 100. ``` #### Prevent user to see some activities in
 history endpoint By default all activities are shown in user history endpoint.
 you can add specific url name that you don't want to show to the user in
 `DRF_ACTIVITI_API_UNNECESSARY_URL_NAME` attribute in settings.py and then the
-user can not be able to see them. Note: This attribute must be a list. ####
-Excluding specific url names in django admin panel Note: In django admin panel
-you can filter logs by url name. some url name do not appear in filter list.
-you can set `DRF_ACTIVITY_TRACKER_URL_NAMES` in settings with the list of url
-names that you want to be filtered by.
+user can not be able to see them. Note: This attribute must be a list.
```

### Comparing `drf-user-activity-tracker-mongodb-1.4.1/LICENSE` & `drf-user-activity-tracker-mongodb-1.4.2/LICENSE`

 * *Files identical despite different names*

