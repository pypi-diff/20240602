# Comparing `tmp/aa_opcalendar-3.0.0b2.tar.gz` & `tmp/aa_opcalendar-3.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_opcalendar-3.0.0b2.tar", last modified: Wed May 29 14:48:49 2024, max compression
+gzip compressed data, was "aa_opcalendar-3.0.0b3.tar", last modified: Sun Jun  2 12:29:53 2024, max compression
```

## Comparing `aa_opcalendar-3.0.0b2.tar` & `aa_opcalendar-3.0.0b3.tar`

### file list

```diff
@@ -1,112 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.792685 aa_opcalendar-3.0.0b2/
--rwxrwxrwx   0 root         (0) root         (0)     1070 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      179 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10086 2024-05-29 14:48:49.792685 aa_opcalendar-3.0.0b2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     9185 2024-05-29 12:50:54.000000 aa_opcalendar-3.0.0b2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.792685 aa_opcalendar-3.0.0b2/aa_opcalendar.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10086 2024-05-29 14:48:49.000000 aa_opcalendar-3.0.0b2/aa_opcalendar.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3636 2024-05-29 14:48:49.000000 aa_opcalendar-3.0.0b2/aa_opcalendar.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-29 14:48:49.000000 aa_opcalendar-3.0.0b2/aa_opcalendar.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       62 2024-05-29 14:48:49.000000 aa_opcalendar-3.0.0b2/aa_opcalendar.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       34 2024-05-29 14:48:49.000000 aa_opcalendar-3.0.0b2/aa_opcalendar.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.772685 aa_opcalendar-3.0.0b2/eventcalendar/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/eventcalendar/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      403 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/eventcalendar/asgi.py
--rwxrwxrwx   0 root         (0) root         (0)      453 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/eventcalendar/helper.py
--rwxrwxrwx   0 root         (0) root         (0)     3217 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/eventcalendar/settings.py
--rwxrwxrwx   0 root         (0) root         (0)      938 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/eventcalendar/urls.py
--rwxrwxrwx   0 root         (0) root         (0)      747 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/eventcalendar/views.py
--rwxrwxrwx   0 root         (0) root         (0)      403 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/eventcalendar/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.788685 aa_opcalendar-3.0.0b2/opcalendar/
--rwxrwxrwx   0 root         (0) root         (0)      106 2024-05-29 14:48:14.000000 aa_opcalendar-3.0.0b2/opcalendar/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4254 2024-05-19 12:13:34.000000 aa_opcalendar-3.0.0b2/opcalendar/admin.py
--rwxrwxrwx   0 root         (0) root         (0)     3339 2024-05-20 14:29:05.000000 aa_opcalendar-3.0.0b2/opcalendar/app_settings.py
--rwxrwxrwx   0 root         (0) root         (0)      165 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/apps.py
--rwxrwxrwx   0 root         (0) root         (0)     1104 2024-05-29 12:51:05.000000 aa_opcalendar-3.0.0b2/opcalendar/auth_hooks.py
--rwxr-xr-x   0 root         (0) root         (0)    11174 2024-05-21 12:42:18.000000 aa_opcalendar-3.0.0b2/opcalendar/calendar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.788685 aa_opcalendar-3.0.0b2/opcalendar/cogs/
--rwxrwxrwx   0 root         (0) root         (0)     6898 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/cogs/ops.py
--rwxrwxrwx   0 root         (0) root         (0)      553 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/decorators.py
--rwxrwxrwx   0 root         (0) root         (0)     3984 2024-05-19 12:13:34.000000 aa_opcalendar-3.0.0b2/opcalendar/forms.py
--rwxrwxrwx   0 root         (0) root         (0)      772 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.788685 aa_opcalendar-3.0.0b2/opcalendar/migrations/
--rwxrwxrwx   0 root         (0) root         (0)     7318 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0001_initial.py
--rwxrwxrwx   0 root         (0) root         (0)      769 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0002_auto_20201104_1054.py
--rwxrwxrwx   0 root         (0) root         (0)      827 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0003_eventhost.py
--rwxrwxrwx   0 root         (0) root         (0)      539 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0004_event_host.py
--rwxrwxrwx   0 root         (0) root         (0)      569 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0005_auto_20201104_1127.py
--rwxrwxrwx   0 root         (0) root         (0)     1946 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0006_auto_20201104_1201.py
--rwxrwxrwx   0 root         (0) root         (0)      403 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0007_eventhost_twitter.py
--rwxrwxrwx   0 root         (0) root         (0)      358 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0008_auto_20201105_0846.py
--rwxrwxrwx   0 root         (0) root         (0)      913 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0009_auto_20201105_0859.py
--rwxrwxrwx   0 root         (0) root         (0)      635 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0010_auto_20201105_1602.py
--rwxrwxrwx   0 root         (0) root         (0)     1568 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0011_eventimport.py
--rwxrwxrwx   0 root         (0) root         (0)      576 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0012_auto_20210112_0934.py
--rwxrwxrwx   0 root         (0) root         (0)      661 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0013_eventimport_creator.py
--rwxrwxrwx   0 root         (0) root         (0)     1957 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0014_auto_20210113_0836.py
--rwxrwxrwx   0 root         (0) root         (0)      671 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0015_eventimport_eve_character.py
--rwxrwxrwx   0 root         (0) root         (0)     4088 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0016_auto_20210119_1545.py
--rwxrwxrwx   0 root         (0) root         (0)     1295 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0017_auto_20210119_1626.py
--rwxrwxrwx   0 root         (0) root         (0)      684 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0018_auto_20210119_1701.py
--rwxrwxrwx   0 root         (0) root         (0)      708 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0019_auto_20210125_1005.py
--rwxrwxrwx   0 root         (0) root         (0)      459 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0020_auto_20210125_1007.py
--rwxrwxrwx   0 root         (0) root         (0)      404 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0021_eventhost_logo_url.py
--rwxrwxrwx   0 root         (0) root         (0)     2983 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0022_auto_20210222_1255.py
--rwxrwxrwx   0 root         (0) root         (0)    13049 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0023_auto_20210330_0632.py
--rwxrwxrwx   0 root         (0) root         (0)     2617 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0024_auto_20210429_1111.py
--rwxr-xr-x   0 root         (0) root         (0)      995 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0025_auto_20220115_1101.py
--rwxr-xr-x   0 root         (0) root         (0)      791 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0026_alter_event_repeat_event.py
--rw-r--r--   0 root         (0) root         (0)     2305 2024-05-29 12:57:47.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/0027_eventmember_comment_eventmember_status_usersettings.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/migrations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    26776 2024-05-20 12:49:29.000000 aa_opcalendar-3.0.0b2/opcalendar/models.py
--rwxrwxrwx   0 root         (0) root         (0)      374 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/providers.py
--rwxrwxrwx   0 root         (0) root         (0)     7077 2024-05-20 14:43:05.000000 aa_opcalendar-3.0.0b2/opcalendar/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.772685 aa_opcalendar-3.0.0b2/opcalendar/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.792685 aa_opcalendar-3.0.0b2/opcalendar/static/opcalendar/
--rwxrwxrwx   0 root         (0) root         (0)     1204 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/static/opcalendar/calendar.png
--rwxrwxrwx   0 root         (0) root         (0)     2845 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/static/opcalendar/style_dark.css
--rwxr-xr-x   0 root         (0) root         (0)     6988 2024-05-18 11:32:45.000000 aa_opcalendar-3.0.0b2/opcalendar/static/opcalendar/style_light.css
--rwxrwxrwx   0 root         (0) root         (0)     1379 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/static/opcalendar/terminate.png
--rwxrwxrwx   0 root         (0) root         (0)   947196 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/swagger.json
--rwxrwxrwx   0 root         (0) root         (0)    14774 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.772685 aa_opcalendar-3.0.0b2/opcalendar/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.792685 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/
--rwxrwxrwx   0 root         (0) root         (0)      448 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/add_member.html
--rwxr-xr-x   0 root         (0) root         (0)     1255 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/base.html
--rwxr-xr-x   0 root         (0) root         (0)     2558 2024-05-21 12:42:18.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/calendar.html
--rwxr-xr-x   0 root         (0) root         (0)     1401 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/event-add.html
--rwxr-xr-x   0 root         (0) root         (0)     2392 2024-05-19 08:16:20.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/event-details.html
--rwxr-xr-x   0 root         (0) root         (0)      900 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/event-edit.html
--rwxrwxrwx   0 root         (0) root         (0)      384 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/event_delete.html
--rwxrwxrwx   0 root         (0) root         (0)     4607 2024-05-19 06:53:22.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/ingame-event-details.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.772685 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.792685 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/base/
--rw-r--r--   0 root         (0) root         (0)      943 2024-05-19 12:04:57.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/base/menu.html
--rw-r--r--   0 root         (0) root         (0)      247 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/base/stylesheets.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.792685 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/calendar/
--rw-r--r--   0 root         (0) root         (0)     1995 2024-05-20 13:01:40.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/calendar/legends.html
--rw-r--r--   0 root         (0) root         (0)      672 2024-05-19 06:58:32.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/calendar/navigation.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.792685 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/event_details/
--rw-r--r--   0 root         (0) root         (0)     1386 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/event_details/details.html
--rw-r--r--   0 root         (0) root         (0)     1651 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/event_details/host.html
--rw-r--r--   0 root         (0) root         (0)     1215 2024-05-18 08:14:23.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/event_details/navigation.html
--rw-r--r--   0 root         (0) root         (0)      945 2024-05-18 11:33:31.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/event_details/signups.html
--rw-r--r--   0 root         (0) root         (0)     1718 2024-05-18 11:34:28.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/event_details/signups_navigation.html
--rwxrwxrwx   0 root         (0) root         (0)      400 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/signup.html
--rw-rw-r--   0 root         (0) root         (0)     1026 2024-05-20 11:48:14.000000 aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/user_settings.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.792685 aa_opcalendar-3.0.0b2/opcalendar/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4316 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/tests/test_models.py
--rwxrwxrwx   0 root         (0) root         (0)    20005 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/tests/test_tasks.py
--rwxrwxrwx   0 root         (0) root         (0)     2880 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/tests/testdata.py
--rwxrwxrwx   0 root         (0) root         (0)     1909 2024-05-29 12:47:00.000000 aa_opcalendar-3.0.0b2/opcalendar/urls.py
--rwxrwxrwx   0 root         (0) root         (0)    10257 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/opcalendar/utils.py
--rwxr-xr-x   0 root         (0) root         (0)    18858 2024-05-29 14:44:35.000000 aa_opcalendar-3.0.0b2/opcalendar/views.py
--rwxrwxrwx   0 root         (0) root         (0)      187 2024-05-29 14:48:49.792685 aa_opcalendar-3.0.0b2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1488 2024-05-29 14:47:36.000000 aa_opcalendar-3.0.0b2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:48:49.792685 aa_opcalendar-3.0.0b2/testauth/
--rwxrwxrwx   0 root         (0) root         (0)       46 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/testauth/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      611 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/testauth/celery.py
--rwxrwxrwx   0 root         (0) root         (0)     9946 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/testauth/settings.py
--rwxrwxrwx   0 root         (0) root         (0)      120 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/testauth/urls.py
--rwxrwxrwx   0 root         (0) root         (0)      397 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b2/testauth/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.117589 aa_opcalendar-3.0.0b3/
+-rwxrwxrwx   0 root         (0) root         (0)     1070 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      179 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10319 2024-06-02 12:29:53.117589 aa_opcalendar-3.0.0b3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     9389 2024-06-02 10:51:10.000000 aa_opcalendar-3.0.0b3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.117589 aa_opcalendar-3.0.0b3/aa_opcalendar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10319 2024-06-02 12:29:53.000000 aa_opcalendar-3.0.0b3/aa_opcalendar.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3787 2024-06-02 12:29:53.000000 aa_opcalendar-3.0.0b3/aa_opcalendar.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-06-02 12:29:53.000000 aa_opcalendar-3.0.0b3/aa_opcalendar.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       76 2024-06-02 12:29:53.000000 aa_opcalendar-3.0.0b3/aa_opcalendar.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       34 2024-06-02 12:29:53.000000 aa_opcalendar-3.0.0b3/aa_opcalendar.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.097579 aa_opcalendar-3.0.0b3/eventcalendar/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/eventcalendar/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      403 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/eventcalendar/asgi.py
+-rwxrwxrwx   0 root         (0) root         (0)      453 2024-06-02 09:07:35.000000 aa_opcalendar-3.0.0b3/eventcalendar/helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3217 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/eventcalendar/settings.py
+-rwxrwxrwx   0 root         (0) root         (0)      940 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/eventcalendar/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)      748 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/eventcalendar/views.py
+-rwxrwxrwx   0 root         (0) root         (0)      403 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/eventcalendar/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.101581 aa_opcalendar-3.0.0b3/opcalendar/
+-rwxrwxrwx   0 root         (0) root         (0)      106 2024-06-02 12:27:23.000000 aa_opcalendar-3.0.0b3/opcalendar/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4256 2024-06-02 09:31:14.000000 aa_opcalendar-3.0.0b3/opcalendar/admin.py
+-rwxr-xr-x   0 root         (0) root         (0)     3469 2024-06-02 12:26:33.000000 aa_opcalendar-3.0.0b3/opcalendar/app_settings.py
+-rwxrwxrwx   0 root         (0) root         (0)      165 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/apps.py
+-rwxrwxrwx   0 root         (0) root         (0)     2006 2024-06-02 10:50:26.000000 aa_opcalendar-3.0.0b3/opcalendar/auth_hooks.py
+-rwxr-xr-x   0 root         (0) root         (0)    11232 2024-06-02 10:08:10.000000 aa_opcalendar-3.0.0b3/opcalendar/calendar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.101581 aa_opcalendar-3.0.0b3/opcalendar/cogs/
+-rwxrwxrwx   0 root         (0) root         (0)     6896 2024-06-02 09:31:14.000000 aa_opcalendar-3.0.0b3/opcalendar/cogs/ops.py
+-rwxrwxrwx   0 root         (0) root         (0)      553 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/decorators.py
+-rwxr-xr-x   0 root         (0) root         (0)     3985 2024-06-02 12:26:33.000000 aa_opcalendar-3.0.0b3/opcalendar/forms.py
+-rwxrwxrwx   0 root         (0) root         (0)      773 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.105583 aa_opcalendar-3.0.0b3/opcalendar/migrations/
+-rwxrwxrwx   0 root         (0) root         (0)     7318 2024-06-02 09:07:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0001_initial.py
+-rwxrwxrwx   0 root         (0) root         (0)      769 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0002_auto_20201104_1054.py
+-rwxrwxrwx   0 root         (0) root         (0)      827 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0003_eventhost.py
+-rwxrwxrwx   0 root         (0) root         (0)      539 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0004_event_host.py
+-rwxrwxrwx   0 root         (0) root         (0)      569 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0005_auto_20201104_1127.py
+-rwxrwxrwx   0 root         (0) root         (0)     1946 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0006_auto_20201104_1201.py
+-rwxrwxrwx   0 root         (0) root         (0)      403 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0007_eventhost_twitter.py
+-rwxrwxrwx   0 root         (0) root         (0)      358 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0008_auto_20201105_0846.py
+-rwxrwxrwx   0 root         (0) root         (0)      913 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0009_auto_20201105_0859.py
+-rwxrwxrwx   0 root         (0) root         (0)      635 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0010_auto_20201105_1602.py
+-rwxrwxrwx   0 root         (0) root         (0)     1568 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0011_eventimport.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0012_auto_20210112_0934.py
+-rwxrwxrwx   0 root         (0) root         (0)      661 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0013_eventimport_creator.py
+-rwxrwxrwx   0 root         (0) root         (0)     1957 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0014_auto_20210113_0836.py
+-rwxrwxrwx   0 root         (0) root         (0)      671 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0015_eventimport_eve_character.py
+-rwxrwxrwx   0 root         (0) root         (0)     4088 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0016_auto_20210119_1545.py
+-rwxrwxrwx   0 root         (0) root         (0)     1295 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0017_auto_20210119_1626.py
+-rwxrwxrwx   0 root         (0) root         (0)      684 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0018_auto_20210119_1701.py
+-rwxrwxrwx   0 root         (0) root         (0)      708 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0019_auto_20210125_1005.py
+-rwxrwxrwx   0 root         (0) root         (0)      459 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0020_auto_20210125_1007.py
+-rwxrwxrwx   0 root         (0) root         (0)      404 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0021_eventhost_logo_url.py
+-rwxrwxrwx   0 root         (0) root         (0)     2983 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0022_auto_20210222_1255.py
+-rwxrwxrwx   0 root         (0) root         (0)    13049 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0023_auto_20210330_0632.py
+-rwxrwxrwx   0 root         (0) root         (0)     2617 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0024_auto_20210429_1111.py
+-rwxr-xr-x   0 root         (0) root         (0)      995 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0025_auto_20220115_1101.py
+-rwxr-xr-x   0 root         (0) root         (0)      791 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0026_alter_event_repeat_event.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/0027_eventmember_comment_eventmember_status_usersettings.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/migrations/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    26776 2024-05-31 03:29:52.000000 aa_opcalendar-3.0.0b3/opcalendar/models.py
+-rwxrwxrwx   0 root         (0) root         (0)      376 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/providers.py
+-rwxrwxrwx   0 root         (0) root         (0)     7079 2024-06-02 09:31:14.000000 aa_opcalendar-3.0.0b3/opcalendar/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.093577 aa_opcalendar-3.0.0b3/opcalendar/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.105583 aa_opcalendar-3.0.0b3/opcalendar/static/opcalendar/
+-rwxrwxrwx   0 root         (0) root         (0)     1204 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/static/opcalendar/calendar.png
+-rwxr-xr-x   0 root         (0) root         (0)     4505 2024-06-02 10:21:30.000000 aa_opcalendar-3.0.0b3/opcalendar/static/opcalendar/style_opcalendar.css
+-rwxrwxrwx   0 root         (0) root         (0)     1379 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/static/opcalendar/terminate.png
+-rwxrwxrwx   0 root         (0) root         (0)   947196 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/swagger.json
+-rwxrwxrwx   0 root         (0) root         (0)    14774 2024-06-02 09:31:14.000000 aa_opcalendar-3.0.0b3/opcalendar/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.093577 aa_opcalendar-3.0.0b3/opcalendar/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.113587 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/
+-rwxrwxrwx   0 root         (0) root         (0)      448 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/add_member.html
+-rwxr-xr-x   0 root         (0) root         (0)      605 2024-06-02 08:41:57.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/base.html
+-rwxr-xr-x   0 root         (0) root         (0)     3932 2024-06-02 10:25:03.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/calendar.html
+-rwxr-xr-x   0 root         (0) root         (0)     1303 2024-06-02 12:26:33.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/event-add.html
+-rwxr-xr-x   0 root         (0) root         (0)     2392 2024-06-02 12:26:33.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/event-details.html
+-rwxr-xr-x   0 root         (0) root         (0)     1321 2024-06-02 08:02:50.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/event-edit.html
+-rwxrwxrwx   0 root         (0) root         (0)      384 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/event_delete.html
+-rwxrwxrwx   0 root         (0) root         (0)     4607 2024-05-19 06:53:22.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/ingame-event-details.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.097579 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.113587 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/base/
+-rw-r--r--   0 root         (0) root         (0)      943 2024-05-19 12:04:57.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/base/menu.html
+-rw-r--r--   0 root         (0) root         (0)      113 2024-06-02 08:43:40.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/base/stylesheets.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.113587 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/calendar/
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-06-02 10:24:24.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/calendar/legends.html
+-rw-r--r--   0 root         (0) root         (0)      672 2024-05-19 06:58:32.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/calendar/navigation.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.113587 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/event_details/
+-rw-r--r--   0 root         (0) root         (0)     1386 2024-06-02 12:26:33.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/event_details/details.html
+-rw-r--r--   0 root         (0) root         (0)     1651 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/event_details/host.html
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-05-18 08:14:23.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/event_details/navigation.html
+-rw-r--r--   0 root         (0) root         (0)      945 2024-05-18 11:33:31.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/event_details/signups.html
+-rw-r--r--   0 root         (0) root         (0)     1718 2024-05-18 11:34:28.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/event_details/signups_navigation.html
+-rwxrwxrwx   0 root         (0) root         (0)      400 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/signup.html
+-rw-rw-r--   0 root         (0) root         (0)     1026 2024-05-20 11:48:14.000000 aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/user_settings.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.113587 aa_opcalendar-3.0.0b3/opcalendar/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4316 2024-06-02 09:31:14.000000 aa_opcalendar-3.0.0b3/opcalendar/tests/test_models.py
+-rwxrwxrwx   0 root         (0) root         (0)    20005 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/opcalendar/tests/test_tasks.py
+-rwxrwxrwx   0 root         (0) root         (0)     2879 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/opcalendar/tests/testdata.py
+-rwxrwxrwx   0 root         (0) root         (0)     1909 2024-05-29 12:47:00.000000 aa_opcalendar-3.0.0b3/opcalendar/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)    10256 2024-06-02 09:31:14.000000 aa_opcalendar-3.0.0b3/opcalendar/utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    18860 2024-06-02 12:26:33.000000 aa_opcalendar-3.0.0b3/opcalendar/views.py
+-rwxrwxrwx   0 root         (0) root         (0)      187 2024-06-02 12:29:53.117589 aa_opcalendar-3.0.0b3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1513 2024-06-02 09:40:54.000000 aa_opcalendar-3.0.0b3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.113587 aa_opcalendar-3.0.0b3/testauth/
+-rwxrwxrwx   0 root         (0) root         (0)       46 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b3/testauth/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1405 2024-06-02 09:00:59.000000 aa_opcalendar-3.0.0b3/testauth/celery.py
+-rwxrwxrwx   0 root         (0) root         (0)     9946 2024-06-02 09:07:35.000000 aa_opcalendar-3.0.0b3/testauth/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.113587 aa_opcalendar-3.0.0b3/testauth/settings_aa3/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-06-02 08:59:10.000000 aa_opcalendar-3.0.0b3/testauth/settings_aa3/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8713 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/testauth/settings_aa3/base.py
+-rw-rw-r--   0 root         (0) root         (0)     2467 2024-06-02 09:07:23.000000 aa_opcalendar-3.0.0b3/testauth/settings_aa3/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 12:29:53.117589 aa_opcalendar-3.0.0b3/testauth/settings_aa4/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-06-02 08:59:54.000000 aa_opcalendar-3.0.0b3/testauth/settings_aa4/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9079 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/testauth/settings_aa4/base.py
+-rw-rw-r--   0 root         (0) root         (0)     2467 2024-06-02 09:07:20.000000 aa_opcalendar-3.0.0b3/testauth/settings_aa4/local.py
+-rwxrwxrwx   0 root         (0) root         (0)      173 2024-06-02 09:07:34.000000 aa_opcalendar-3.0.0b3/testauth/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)      397 2024-06-02 09:01:31.000000 aa_opcalendar-3.0.0b3/testauth/wsgi.py
```

### Comparing `aa_opcalendar-3.0.0b2/LICENSE` & `aa_opcalendar-3.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/PKG-INFO` & `aa_opcalendar-3.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-opcalendar
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: Event calendar plugin app for Alliance Auth
 Home-page: https://gitlab.com/paulipa/allianceauth-opcalendar
 Author: Ikarus Cesaille
 Author-email: contact@eve-linknet.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,14 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allianceauth<5.0.0,>=4
 Requires-Dist: feedparser
 Requires-Dist: ics>=0.7.2
 Requires-Dist: pytz
 Requires-Dist: django-ical
+Requires-Dist: requests-mock
 
 # Operation Calendar
 
 An operation calendar app for Alliance Auth to display fleet operations and other events.
 
 ![release](https://img.shields.io/pypi/v/aa-opcalendar??label=release) ![python](https://img.shields.io/pypi/pyversions/aa-opcalendar?) ![license](https://img.shields.io/badge/license-MIT-green)
 
@@ -55,14 +56,15 @@
  	* Custom tickers
  	* Custom colors
  	* Pre-fill text to add on events with the category
 * Multihost support
 * Discord notifications
 	* Webhook
 	* For: new, edited and deleted events
+* Counter on menu for events that the user has not signed or rejected from
 
 ![screenshot](https://i.imgur.com/92nBoO7.jpg)
 ![screenshot](https://i.imgur.com/Mbvq3So.jpg)
 Dark and white themes
 
 ![screenshot](https://i.imgur.com/IAZ5GRi.jpg)
 aa-moonmining support
@@ -112,14 +114,15 @@
 OPCALENDAR_NOTIFY_IMPORTS | Wheter to send out discord notifications for ingame and public NPSI events | True
 OPCALENDAR_DISPLAY_STRUCTURETIMERS | whether we should inculde timers from the structuretimers plugin in the calendar. Inherits view permissions from aa-structuretimers | True
 OPCALENDAR_DISPLAY_MOONMINING | whether we should inculde extractions from the aa-moonmining plugin in the calendar. Inherits view permissions from aa-moonmining | True
 OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL | whether we display external hosts such as ingame hosts in the discord ops command filters | False
 OPCALENDAR_DISPLAY_MOONMINING_TAGS | Display the rarity tag of aa-moonmining moons if the moonmining plugin is installed | True
 OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME | Displays aa-moonmining extraction time based on arrival time. Set to False to display as auto fracture time | True
 OPCALENDAR_NOTIFY_REPEAT_EVENTS | If repeated events should also be created as webhook pings on discord. Can create spam if the event repeat is set to high | True
+OPCALENDAR_SHOW_EVENT_COUNTER | Shows a counter next to the opcalendar menu for events that the user has not responded to | True
 
 
 ## Setup
 Before you are able to create new events on the front end you will need to setup the needed categories and visibility filters for your events.
 
 ### 1. Host
 Hosts are for identifying reasons. If you run a single corporation or alliance entity you most likely only want one host. If you want to extend the calendar with other hosts such as NPSI communities you can create a host for each different entity.
```

### Comparing `aa_opcalendar-3.0.0b2/README.md` & `aa_opcalendar-3.0.0b3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
  	* Custom tickers
  	* Custom colors
  	* Pre-fill text to add on events with the category
 * Multihost support
 * Discord notifications
 	* Webhook
 	* For: new, edited and deleted events
+* Counter on menu for events that the user has not signed or rejected from
 
 ![screenshot](https://i.imgur.com/92nBoO7.jpg)
 ![screenshot](https://i.imgur.com/Mbvq3So.jpg)
 Dark and white themes
 
 ![screenshot](https://i.imgur.com/IAZ5GRi.jpg)
 aa-moonmining support
@@ -86,14 +87,15 @@
 OPCALENDAR_NOTIFY_IMPORTS | Wheter to send out discord notifications for ingame and public NPSI events | True
 OPCALENDAR_DISPLAY_STRUCTURETIMERS | whether we should inculde timers from the structuretimers plugin in the calendar. Inherits view permissions from aa-structuretimers | True
 OPCALENDAR_DISPLAY_MOONMINING | whether we should inculde extractions from the aa-moonmining plugin in the calendar. Inherits view permissions from aa-moonmining | True
 OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL | whether we display external hosts such as ingame hosts in the discord ops command filters | False
 OPCALENDAR_DISPLAY_MOONMINING_TAGS | Display the rarity tag of aa-moonmining moons if the moonmining plugin is installed | True
 OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME | Displays aa-moonmining extraction time based on arrival time. Set to False to display as auto fracture time | True
 OPCALENDAR_NOTIFY_REPEAT_EVENTS | If repeated events should also be created as webhook pings on discord. Can create spam if the event repeat is set to high | True
+OPCALENDAR_SHOW_EVENT_COUNTER | Shows a counter next to the opcalendar menu for events that the user has not responded to | True
 
 
 ## Setup
 Before you are able to create new events on the front end you will need to setup the needed categories and visibility filters for your events.
 
 ### 1. Host
 Hosts are for identifying reasons. If you run a single corporation or alliance entity you most likely only want one host. If you want to extend the calendar with other hosts such as NPSI communities you can create a host for each different entity.
```

### Comparing `aa_opcalendar-3.0.0b2/aa_opcalendar.egg-info/PKG-INFO` & `aa_opcalendar-3.0.0b3/aa_opcalendar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-opcalendar
-Version: 3.0.0b2
+Version: 3.0.0b3
 Summary: Event calendar plugin app for Alliance Auth
 Home-page: https://gitlab.com/paulipa/allianceauth-opcalendar
 Author: Ikarus Cesaille
 Author-email: contact@eve-linknet.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,14 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allianceauth<5.0.0,>=4
 Requires-Dist: feedparser
 Requires-Dist: ics>=0.7.2
 Requires-Dist: pytz
 Requires-Dist: django-ical
+Requires-Dist: requests-mock
 
 # Operation Calendar
 
 An operation calendar app for Alliance Auth to display fleet operations and other events.
 
 ![release](https://img.shields.io/pypi/v/aa-opcalendar??label=release) ![python](https://img.shields.io/pypi/pyversions/aa-opcalendar?) ![license](https://img.shields.io/badge/license-MIT-green)
 
@@ -55,14 +56,15 @@
  	* Custom tickers
  	* Custom colors
  	* Pre-fill text to add on events with the category
 * Multihost support
 * Discord notifications
 	* Webhook
 	* For: new, edited and deleted events
+* Counter on menu for events that the user has not signed or rejected from
 
 ![screenshot](https://i.imgur.com/92nBoO7.jpg)
 ![screenshot](https://i.imgur.com/Mbvq3So.jpg)
 Dark and white themes
 
 ![screenshot](https://i.imgur.com/IAZ5GRi.jpg)
 aa-moonmining support
@@ -112,14 +114,15 @@
 OPCALENDAR_NOTIFY_IMPORTS | Wheter to send out discord notifications for ingame and public NPSI events | True
 OPCALENDAR_DISPLAY_STRUCTURETIMERS | whether we should inculde timers from the structuretimers plugin in the calendar. Inherits view permissions from aa-structuretimers | True
 OPCALENDAR_DISPLAY_MOONMINING | whether we should inculde extractions from the aa-moonmining plugin in the calendar. Inherits view permissions from aa-moonmining | True
 OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL | whether we display external hosts such as ingame hosts in the discord ops command filters | False
 OPCALENDAR_DISPLAY_MOONMINING_TAGS | Display the rarity tag of aa-moonmining moons if the moonmining plugin is installed | True
 OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME | Displays aa-moonmining extraction time based on arrival time. Set to False to display as auto fracture time | True
 OPCALENDAR_NOTIFY_REPEAT_EVENTS | If repeated events should also be created as webhook pings on discord. Can create spam if the event repeat is set to high | True
+OPCALENDAR_SHOW_EVENT_COUNTER | Shows a counter next to the opcalendar menu for events that the user has not responded to | True
 
 
 ## Setup
 Before you are able to create new events on the front end you will need to setup the needed categories and visibility filters for your events.
 
 ### 1. Host
 Hosts are for identifying reasons. If you run a single corporation or alliance entity you most likely only want one host. If you want to extend the calendar with other hosts such as NPSI communities you can create a host for each different entity.
```

### Comparing `aa_opcalendar-3.0.0b2/aa_opcalendar.egg-info/SOURCES.txt` & `aa_opcalendar-3.0.0b3/aa_opcalendar.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,15 @@
 opcalendar/migrations/0023_auto_20210330_0632.py
 opcalendar/migrations/0024_auto_20210429_1111.py
 opcalendar/migrations/0025_auto_20220115_1101.py
 opcalendar/migrations/0026_alter_event_repeat_event.py
 opcalendar/migrations/0027_eventmember_comment_eventmember_status_usersettings.py
 opcalendar/migrations/__init__.py
 opcalendar/static/opcalendar/calendar.png
-opcalendar/static/opcalendar/style_dark.css
-opcalendar/static/opcalendar/style_light.css
+opcalendar/static/opcalendar/style_opcalendar.css
 opcalendar/static/opcalendar/terminate.png
 opcalendar/templates/opcalendar/add_member.html
 opcalendar/templates/opcalendar/base.html
 opcalendar/templates/opcalendar/calendar.html
 opcalendar/templates/opcalendar/event-add.html
 opcalendar/templates/opcalendar/event-details.html
 opcalendar/templates/opcalendar/event-edit.html
@@ -88,8 +87,14 @@
 opcalendar/tests/test_models.py
 opcalendar/tests/test_tasks.py
 opcalendar/tests/testdata.py
 testauth/__init__.py
 testauth/celery.py
 testauth/settings.py
 testauth/urls.py
-testauth/wsgi.py
+testauth/wsgi.py
+testauth/settings_aa3/__init__.py
+testauth/settings_aa3/base.py
+testauth/settings_aa3/local.py
+testauth/settings_aa4/__init__.py
+testauth/settings_aa4/base.py
+testauth/settings_aa4/local.py
```

### Comparing `aa_opcalendar-3.0.0b2/eventcalendar/settings.py` & `aa_opcalendar-3.0.0b3/eventcalendar/settings.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/eventcalendar/urls.py` & `aa_opcalendar-3.0.0b3/eventcalendar/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 Class-based views
     1. Add an import:  from other_app.views import Home
     2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
+
 from django.contrib import admin
-from django.urls import path, include
+from django.urls import include, path
+
 from .views import signup, user_logout
 
 urlpatterns = [
     path("admin/", admin.site.urls),
     path("signup/", signup, name="signup"),
     path("logout/", user_logout, name="logout"),
     path("", include("opcalendar.urls")),
```

### Comparing `aa_opcalendar-3.0.0b2/eventcalendar/views.py` & `aa_opcalendar-3.0.0b3/eventcalendar/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from django.shortcuts import render, redirect
 from django.contrib.auth import authenticate, login, logout
+from django.shortcuts import redirect, render
+
 from opcalendar.forms import SignupForm
 
 
 def signup(request):
     forms = SignupForm()
     if request.method == "POST":
         forms = SignupForm(request.POST)
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/admin.py` & `aa_opcalendar-3.0.0b3/opcalendar/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from django.contrib import admin
 from django.utils.safestring import mark_safe
+
 from opcalendar.models import (
     Event,
     EventCategory,
-    WebHook,
     EventHost,
     EventImport,
-    Owner,
-    IngameEvents,
-    EventVisibility,
     EventMember,
+    EventVisibility,
+    IngameEvents,
+    Owner,
     UserSettings,
+    WebHook,
 )
-from .forms import EventVisibilityAdminForm, EventCategoryAdminForm
+
+from .forms import EventCategoryAdminForm, EventVisibilityAdminForm
 
 
 def custom_filter(title):
     """
     custom filter for model properties
     :param title:
     :return:
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/app_settings.py` & `aa_opcalendar-3.0.0b3/opcalendar/app_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import re
+
 from django.conf import settings
+
 from .utils import clean_setting
-import re
 
 
 def get_site_url():  # regex sso url
     regex = r"^(.+)\/s.+"
     matches = re.finditer(regex, settings.ESI_SSO_CALLBACK_URL, re.MULTILINE)
     url = "http://"
 
@@ -47,14 +49,17 @@
 OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL = clean_setting(
     "OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL", False
 )
 
 # whether events with repeat should be sent over the webhook
 OPCALENDAR_NOTIFY_REPEAT_EVENTS = clean_setting("OPCALENDAR_NOTIFY_REPEAT_EVENTS", True)
 
+# whether the event counter will be shown
+OPCALENDAR_SHOW_EVENT_COUNTER = clean_setting("OPCALENDAR_SHOW_EVENT_COUNTER", True)
+
 OPCALENDAR_EVE_UNI_URL = "https://portal.eveuniversity.org/api/getcalendar"
 OPCALENDAR_SPECTRE_URL = "https://www.spectre-fleet.space/engagement/events/rss"
 OPCALENDAR_FUNINC_URL = "https://calendar.google.com/calendar/ical/og3uh76l8ul3dfgbie03fbbgs8%40group.calendar.google.com/private-f466889b44741fd7249e99e21ac171ff/basic.ics"
 OPCALENDAR_FRIDAY_YARRRR_URL = "https://calendar.google.com/calendar/ical/vl43scrg7olk01fv7g79hsbe74%40group.calendar.google.com/public/basic.ics"
 OPCALENDAR_REDEMPTION_ROAD_URL = "https://calendar.google.com/calendar/ical/5o3gpum6ek2irk12f0hnhfdtrs%40group.calendar.google.com/public/basic.ics"
 OPCALENDAR_CAS_URL = "https://calendar.google.com/calendar/ical/0sqru3js6pb1p71e7n1ko91rqs%40group.calendar.google.com/public/basic.ics"
 OPCALENDAR_FWAMING_DWAGONS_URL = "https://calendar.google.com/calendar/ical/l0mnjo7ormaq9gomap0cke4kqk%40group.calendar.google.com/public/basic.ics"
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/calendar.py` & `aa_opcalendar-3.0.0b3/opcalendar/calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from calendar import HTMLCalendar
-from datetime import date
+from datetime import date, datetime
 from itertools import chain
-from datetime import datetime
-from django.db.models import Q, F
-from django.utils import timezone
+
 from allianceauth.services.hooks import get_extension_logger
+from django.db.models import F, Q
+from django.utils import timezone
 
-from .models import Event, IngameEvents
 from .app_settings import (
-    OPCALENDAR_DISPLAY_STRUCTURETIMERS,
     OPCALENDAR_DISPLAY_MOONMINING,
     OPCALENDAR_DISPLAY_MOONMINING_TAGS,
+    OPCALENDAR_DISPLAY_STRUCTURETIMERS,
+    moonmining_active,
+    structuretimers_active,
 )
-
-from .app_settings import structuretimers_active, moonmining_active
+from .models import Event, IngameEvents
 
 if structuretimers_active():
     from structuretimers.models import Timer
 
 if moonmining_active():
     from moonmining.models import Extraction
 
@@ -51,28 +51,32 @@
                 (
                     (event, f"ingame-{event.event_id}")
                     for event in ingame_events_per_day
                 ),
                 ((event, f"struct-{event.id}") for event in structuretimers_per_day),
                 ((event, f"moon-{event.id}") for event in moonmining_per_day),
             ),
-            key=lambda item: item[0].start_time
-            if hasattr(item[0], "start_time")
-            else item[0].chunk_arrival_at,
+            key=lambda item: (
+                item[0].start_time
+                if hasattr(item[0], "start_time")
+                else item[0].chunk_arrival_at
+            ),
         )
 
         d = ""
         standardized_events_per_day = []
         if day != 0:
             for event, unique_id in all_events_per_day:
                 standardized_event = {
                     "id": unique_id,
-                    "start_time": event.start_time
-                    if hasattr(event, "start_time")
-                    else event.chunk_arrival_at,
+                    "start_time": (
+                        event.start_time
+                        if hasattr(event, "start_time")
+                        else event.chunk_arrival_at
+                    ),
                     "end_time": getattr(event, "end_time", None),
                     "title": getattr(event, "title", "Unnamed Event"),
                     "description": getattr(event, "description", ""),
                     "type": type(event).__name__,
                 }
                 standardized_events_per_day.append(standardized_event)
 
@@ -114,15 +118,15 @@
                             )
                             if OPCALENDAR_DISPLAY_MOONMINING_TAGS
                             else "<span>" + structure[3:] + "</span>"
                         )
 
                         # Generate the HTML for the Extraction event
                         d += (
-                            f'<a class="nostyling" href="/moonmining/extraction/{unique_id}?new_page=yes">'
+                            f'<a class="nostyling" href="/moonmining/extraction/{event.id}?new_page=yes">'
                             f'<div class="event {"past-event" if datetime.now(timezone.utc) > event.chunk_arrival_at else "future-event"} event-moonmining">'
                             f'<span id="event-time-{unique_id}">{event.chunk_arrival_at.strftime("%H:%M")}</span>'
                             f"<span>{event.refinery.moon.eve_moon.name}</span>"
                             f'<div class="event-moon-details">'
                             f"{display_name}"
                             f"</div>"
                             f"</div>"
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/cogs/ops.py` & `aa_opcalendar-3.0.0b3/opcalendar/cogs/ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # Cog Stuff
-from discord.ext import commands
-from discord.embeds import Embed
-from discord.colour import Color
-from discord.commands import Option
-
-# AA Contexts
-from aadiscordbot.app_settings import get_site_url
-from allianceauth.services.modules.discord.models import DiscordUser
+import logging
 
 # OPCALENDAR
 import operator
-from opcalendar.models import Event, IngameEvents, EventHost
-from django.db.models import Q, F
-from itertools import chain
-from app_utils.urls import static_file_absolute_url
-from datetime import datetime
 import os
+from datetime import datetime
+from itertools import chain
 
-import logging
-
+# AA Contexts
+from aadiscordbot.app_settings import get_site_url
+from allianceauth.services.modules.discord.models import DiscordUser
+from app_utils.urls import static_file_absolute_url
+from discord.colour import Color
+from discord.commands import Option
+from discord.embeds import Embed
+from discord.ext import commands
 from django.conf import settings
-from opcalendar.app_settings import (
-    OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL,
-)
+from django.db.models import F, Q
+
+from opcalendar.app_settings import OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL
+from opcalendar.models import Event, EventHost, IngameEvents
 
 logger = logging.getLogger(__name__)
 
 # i dont want to do this, but the below object get wont work without it, investigate.
 os.environ["DJANGO_ALLOW_ASYNC_UNSAFE"] = "true"
 
 
@@ -188,15 +185,15 @@
 
         embed.description = "List view of the next 10 upcoming operations for {}. A calendar view is located in [here]({}/opcalendar).\n\nFiltering: To filter events for a specific host add the name after the command ie. `/ops my coalition`\n\nAvailable hosts: *{}*".format(
             host, url, hosts
         )
 
         # Format all events and ingame events
         for event in all_events:
-            if type(event) == Event:
+            if isinstance(event, Event):
                 embed.add_field(
                     name="Event: {0} {1}".format(
                         event.title, event.operation_type.ticker
                     ),
                     value="Host: {0}\nFC: {1}\nDoctrine: {2}\nLocation: {3}\nTime: {4}\n[Details]({5}/opcalendar/event/{6}/details/)\n".format(
                         event.host,
                         event.fc,
@@ -204,15 +201,15 @@
                         event.formup_system,
                         event.start_time,
                         url,
                         event.id,
                     ),
                     inline=False,
                 )
-            if type(event) == IngameEvents:
+            if isinstance(event, IngameEvents):
                 embed.add_field(
                     name="Ingame Event: {0}".format(event.title),
                     value="Host: {0}\n Time:{1}\n[Details]({2}/opcalendar/ingame/event/{3}/details/)".format(
                         event.owner_name,
                         event.start_time,
                         url,
                         event.event_id,
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/decorators.py` & `aa_opcalendar-3.0.0b3/opcalendar/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/forms.py` & `aa_opcalendar-3.0.0b3/opcalendar/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from allianceauth.services.hooks import get_extension_logger
+from django import forms
 from django.forms import ModelForm
+from django.forms.widgets import TextInput
+
 from opcalendar.models import (
     Event,
-    EventMember,
     EventCategory,
     EventHost,
+    EventMember,
     EventVisibility,
     UserSettings,
 )
-from django.forms.widgets import TextInput
-from django import forms
-from allianceauth.services.hooks import get_extension_logger
 
 logger = get_extension_logger(__name__)
 
 
 class EventForm(ModelForm):
     class Meta:
         model = Event
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/helpers.py` & `aa_opcalendar-3.0.0b3/opcalendar/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+
 from django.utils import timezone
 
 
 class time_helpers:
     @staticmethod
     def convert_timedelta(duration):
         # days = duration.days
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0001_initial.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by Django 3.1.2 on 2020-11-04 10:42
 
-from django.conf import settings
-from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
+from django.conf import settings
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [
         ("eveonline", "0012_index_additions"),
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0002_auto_20201104_1054.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0002_auto_20201104_1054.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0003_eventhost.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0003_eventhost.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0004_event_host.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0005_auto_20201104_1127.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Generated by Django 3.1.2 on 2020-11-04 11:26
+# Generated by Django 3.1.2 on 2020-11-04 11:27
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
-        ("opcalendar", "0003_eventhost"),
+        ("opcalendar", "0004_event_host"),
     ]
 
     operations = [
-        migrations.AddField(
+        migrations.AlterField(
             model_name="event",
             name="host",
             field=models.ForeignKey(
                 default=1,
+                null=True,
                 on_delete=django.db.models.deletion.CASCADE,
                 to="opcalendar.eventhost",
             ),
         ),
     ]
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0005_auto_20201104_1127.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0004_event_host.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# Generated by Django 3.1.2 on 2020-11-04 11:27
+# Generated by Django 3.1.2 on 2020-11-04 11:26
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
-        ("opcalendar", "0004_event_host"),
+        ("opcalendar", "0003_eventhost"),
     ]
 
     operations = [
-        migrations.AlterField(
+        migrations.AddField(
             model_name="event",
             name="host",
             field=models.ForeignKey(
                 default=1,
-                null=True,
                 on_delete=django.db.models.deletion.CASCADE,
                 to="opcalendar.eventhost",
             ),
         ),
     ]
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0006_auto_20201104_1201.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0006_auto_20201104_1201.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0009_auto_20201105_0859.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0009_auto_20201105_0859.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 3.1.2 on 2020-11-05 08:59
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("opcalendar", "0008_auto_20201105_0846"),
     ]
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0010_auto_20201105_1602.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0010_auto_20201105_1602.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0011_eventimport.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0011_eventimport.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 3.1.2 on 2021-01-08 08:47
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("opcalendar", "0010_auto_20201105_1602"),
     ]
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0012_auto_20210112_0934.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0012_auto_20210112_0934.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0013_eventimport_creator.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0013_eventimport_creator.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by Django 3.1.2 on 2021-01-13 08:28
 
+import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
-import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("opcalendar", "0012_auto_20210112_0934"),
     ]
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0014_auto_20210113_0836.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0014_auto_20210113_0836.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by Django 3.1.2 on 2021-01-13 08:36
 
+import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
-import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("opcalendar", "0013_eventimport_creator"),
     ]
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0015_eventimport_eve_character.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0015_eventimport_eve_character.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 3.1.2 on 2021-01-13 09:15
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("eveonline", "0012_index_additions"),
         ("opcalendar", "0014_auto_20210113_0836"),
     ]
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0016_auto_20210119_1545.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0016_auto_20210119_1545.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 3.1.2 on 2021-01-19 15:45
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("eveonline", "0012_index_additions"),
         ("authentication", "0017_remove_fleetup_permission"),
         ("opcalendar", "0015_eventimport_eve_character"),
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0017_auto_20210119_1626.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0017_auto_20210119_1626.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 3.1.2 on 2021-01-19 16:26
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("eveonline", "0012_index_additions"),
         ("authentication", "0017_remove_fleetup_permission"),
         ("opcalendar", "0016_auto_20210119_1545"),
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0018_auto_20210119_1701.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0018_auto_20210119_1701.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0019_auto_20210125_1005.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0019_auto_20210125_1005.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0022_auto_20210222_1255.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0022_auto_20210222_1255.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0023_auto_20210330_0632.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0023_auto_20210330_0632.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by Django 3.1.7 on 2021-03-30 06:32
 
-from django.conf import settings
-from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
+from django.conf import settings
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("authentication", "0017_remove_fleetup_permission"),
         ("auth", "0012_alter_user_first_name_max_length"),
         ("eveonline", "0014_auto_20210105_1413"),
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0024_auto_20210429_1111.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0024_auto_20210429_1111.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0025_auto_20220115_1101.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0025_auto_20220115_1101.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0026_alter_event_repeat_event.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0026_alter_event_repeat_event.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/migrations/0027_eventmember_comment_eventmember_status_usersettings.py` & `aa_opcalendar-3.0.0b3/opcalendar/migrations/0027_eventmember_comment_eventmember_status_usersettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Generated by Django 4.2.11 on 2024-05-29 12:54
 
 from django.conf import settings
 from django.db import migrations, models
+
 import opcalendar.models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("opcalendar", "0026_alter_event_repeat_event"),
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/models.py` & `aa_opcalendar-3.0.0b3/opcalendar/models.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/signals.py` & `aa_opcalendar-3.0.0b3/opcalendar/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from django.dispatch import receiver
+import datetime
+
+from allianceauth.services.hooks import get_extension_logger
 from django.db.models.signals import post_save, pre_delete
-from .models import Event, IngameEvents
+from django.dispatch import receiver
 from django.utils import timezone
-import datetime
 from esi.clients import EsiClientProvider
+
 from .app_settings import (
     OPCALENDAR_NOTIFY_IMPORTS,
     OPCALENDAR_NOTIFY_REPEAT_EVENTS,
     get_site_url,
 )
-from allianceauth.services.hooks import get_extension_logger
+from .models import Event, IngameEvents
 
 logger = get_extension_logger(__name__)
 
 RED = 16711710
 BLUE = 42751
 GREEN = 6684416
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/static/opcalendar/calendar.png` & `aa_opcalendar-3.0.0b3/opcalendar/static/opcalendar/calendar.png`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/static/opcalendar/style_dark.css` & `aa_opcalendar-3.0.0b3/opcalendar/static/opcalendar/style_opcalendar.css`

 * *Files 21% similar despite different names*

```diff
@@ -15,34 +15,35 @@
 
 .allianceauth-opcalendar .nostyling{
   text-decoration: none !important;
 }
 
 .allianceauth-opcalendar .btn {
     outline: none;
-    color: black;
+    color: white;
     /* background-color: transparent; */
     box-shadow: 0 0 0 0;
     margin-right:3px;
 }
 
-.allianceauth-opcalendar .event{
-  background-image: none;
-  border-radius: 0;
-  background: #eeeeee;
-  border: none;
-  color: black;
-  font-size: .75em;
-  padding: 0 .75em;
-  line-height: 2em;
-  white-space: nowrap;
-  overflow: hidden;
-  text-overflow: ellipsis;
-  margin-bottom: 1px;
-  position: relative;
+/* Updated event styles */
+.allianceauth-opcalendar .event {
+    background-image: none;
+    border-radius: 4px;
+    background: var(--bs-light);
+    border: none;
+    color: black;
+    font-size: .75em;
+    padding: 0 .75em;
+    line-height: 2em;
+    white-space: nowrap;
+    overflow: hidden;
+    text-overflow: ellipsis;
+    margin-bottom: 3px;
+    position: relative;
 }
 
 .allianceauth-opcalendar .event span {
     display: block;
 }
 
 .allianceauth-opcalendar .event img {
@@ -93,14 +94,15 @@
   width: 15%;
   padding: 0px 5px 0px 5px;
 }
 
 .allianceauth-opcalendar .month {
   font-size: 25px;
   background: #32394e;
+  color: white;
 }
 
 .allianceauth-opcalendar .date {
   font-size: 16px;
   padding: 5px;
 }
 
@@ -155,7 +157,75 @@
   display:table-cell;
   vertical-align:middle;
 }
 
 .allianceauth-opcalendar .calendar .event-moon-name{
   margin-left: 5px;
 }
+
+/* Label classes to fallback for Bootstrap 3 */
+.allianceauth-opcalendar .label {
+    display: inline;
+    padding: .2em .6em .3em;
+    font-size: 75%;
+    color: #fff;
+    vertical-align: baseline;
+    border-radius: .25em;
+}
+
+.allianceauth-opcalendar .label:empty {
+    display: none;
+}
+
+.allianceauth-opcalendar .label-default {
+    background-color: #95a5a6;
+}
+
+.allianceauth-opcalendar .label-default[href]:focus,
+.allianceauth-opcalendar .label-default[href]:hover {
+    background-color: #798d8f;
+}
+
+.allianceauth-opcalendar .label-primary {
+    background-color: #2C3E50;
+}
+
+.allianceauth-opcalendar .label-primary[href]:focus,
+.allianceauth-opcalendar .label-primary[href]:hover {
+    background-color: #1a242f;
+}
+
+.allianceauth-opcalendar .label-success {
+    background-color: #5cb85c;
+}
+
+.allianceauth-opcalendar .label-success[href]:focus,
+.allianceauth-opcalendar .label-success[href]:hover {
+    background-color: #449d44;
+}
+
+.allianceauth-opcalendar .label-info {
+    background-color: #5bc0de;
+}
+
+.allianceauth-opcalendar .label-info[href]:focus,
+.allianceauth-opcalendar .label-info[href]:hover {
+    background-color: #31b0d5;
+}
+
+.allianceauth-opcalendar .label-warning {
+    background-color: #f0ad4e;
+}
+
+.allianceauth-opcalendar .label-warning[href]:focus,
+.allianceauth-opcalendar .label-warning[href]:hover {
+    background-color: #ec971f;
+}
+
+.allianceauth-opcalendar .label-danger {
+    background-color: #d9534f;
+}
+
+.allianceauth-opcalendar .label-danger[href]:focus,
+.allianceauth-opcalendar .label-danger[href]:hover {
+    background-color: #c9302c;
+}
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/static/opcalendar/terminate.png` & `aa_opcalendar-3.0.0b3/opcalendar/static/opcalendar/terminate.png`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/swagger.json` & `aa_opcalendar-3.0.0b3/opcalendar/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/tasks.py` & `aa_opcalendar-3.0.0b3/opcalendar/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/event-details.html` & `aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/event-details.html`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/ingame-event-details.html` & `aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/ingame-event-details.html`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/base/menu.html` & `aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/base/menu.html`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/calendar/legends.html` & `aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/calendar/legends.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load i18n %}
 
 <div class="card">
-    <div class="card-header">{% trans "Legend & Filters:" %}</div>
+    <div class="card-header">{% trans "Legend & Filters" %}</div>
     <div class="card-body">
         <div class="legend">
             <span class="event show-all">{% trans "Show all" %}</span>
             <span class="event external">External NPSI</span>
             <span class="event ingame-event">{% trans "Ingame" %}</span>
             {% for event in visibility %}
                 <style>.{{ event.get_visibility_class }}:before {border-color: transparent {{ event.color }} transparent transparent;border-style: solid;}</style>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% load i18n %}
-{% trans "Legend & Filters:" %}
+{% trans "Legend & Filters" %}
 {% trans "Show all" %} External NPSI {% trans "Ingame" %} {% for event in
 visibility %}
 {{ event.name }} {% endfor %} {% if moonmining_active %} {% trans "Moon Mining"
 %} {% endif %} {% if structuretimers_active %} {% trans "Timers" %} {% endif %}
 {% for event in category %} {{ event.name }} {% endfor %}
 {% trans "Current Eve Time:" %}
 {% if user_settings.use_local_times %} {% trans "Displaying times in:" %} {{%%
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/calendar/navigation.html` & `aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/calendar/navigation.html`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/event_details/details.html` & `aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/event_details/details.html`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/event_details/host.html` & `aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/event_details/host.html`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/event_details/navigation.html` & `aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/event_details/navigation.html`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/event_details/signups.html` & `aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/event_details/signups.html`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/partials/event_details/signups_navigation.html` & `aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/partials/event_details/signups_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/templates/opcalendar/user_settings.html` & `aa_opcalendar-3.0.0b3/opcalendar/templates/opcalendar/user_settings.html`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/tests/test_models.py` & `aa_opcalendar-3.0.0b3/opcalendar/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime as dt
 from unittest.mock import patch
 
-from django.db.models import signals
 from allianceauth.tests.auth_utils import AuthUtils
+from django.db.models import signals
 from pytz import utc
 
-from ..models import EventCategory, EventHost, IngameEvents, Owner, Event
+from ..models import Event, EventCategory, EventHost, IngameEvents, Owner
 from ..signals import fleet_deleted, fleet_saved
 from ..utils import NoSocketsTestCase, add_character_to_user_2, add_new_token
 from .testdata import (
     COLOR_PURPLE,
     esi_get_characters_character_id_calendar,
     esi_get_characters_character_id_calendar_event_id,
 )
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/tests/test_tasks.py` & `aa_opcalendar-3.0.0b3/opcalendar/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/tests/testdata.py` & `aa_opcalendar-3.0.0b3/opcalendar/tests/testdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 from pathlib import Path
 
 from bravado.exception import HTTPNotFound
-from ics import Calendar, Event
-
 from django.utils.dateparse import parse_datetime
+from ics import Calendar, Event
 
 from ..utils import BravadoOperationStub, BravadoResponseStub
 
 COLOR_PURPLE = "#8e44ad"
 
 
 def _load_testdata() -> dict:
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/urls.py` & `aa_opcalendar-3.0.0b3/opcalendar/urls.py`

 * *Files identical despite different names*

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/utils.py` & `aa_opcalendar-3.0.0b3/opcalendar/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-import socket
-from datetime import datetime, timedelta
 import random
+import socket
 import string
+from datetime import datetime, timedelta
 from typing import Any
+
+from allianceauth.authentication.models import CharacterOwnership
+from allianceauth.eveonline.models import EveCharacter
+from allianceauth.services.hooks import get_extension_logger
+from allianceauth.tests.auth_utils import AuthUtils
+from django.conf import settings
 from django.contrib import messages
 from django.contrib.auth.models import User
-from django.conf import settings
 from django.contrib.messages.constants import DEBUG, ERROR, INFO, SUCCESS, WARNING
 from django.test import TestCase
 from django.utils.html import format_html
-
 from esi.models import Scope, Token
 
-from allianceauth.authentication.models import CharacterOwnership
-from allianceauth.eveonline.models import EveCharacter
-from allianceauth.services.hooks import get_extension_logger
-from allianceauth.tests.auth_utils import AuthUtils
-
 logger = get_extension_logger(__name__)
 
 
 def clean_setting(
     name: str,
     default_value: object,
     min_value: int = None,
```

### Comparing `aa_opcalendar-3.0.0b2/opcalendar/views.py` & `aa_opcalendar-3.0.0b3/opcalendar/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
     IngameEvents,
     Owner,
     UserSettings,
 )
 
 from . import tasks
 from .app_settings import (
+    OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME,
     get_site_url,
     moonmining_active,
     structuretimers_active,
-    OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME,
 )
 from .calendar import Calendar
 from .forms import EventEditForm, EventForm, UserSettingsForm
 from .utils import messages_plus
 
 logger = get_extension_logger(__name__)
 
@@ -194,17 +194,17 @@
         context["category"] = EventCategory.objects.all()
         context["visibility"] = EventVisibility.objects.all()
         context["calendar"] = mark_safe(html_cal)
         context["prev_month"] = prev_month(d)
         context["next_month"] = next_month(d)
         context["all_events_per_month"] = all_events_per_month
         context["user_settings"] = user_settings
-        context[
-            "OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME"
-        ] = OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME
+        context["OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME"] = (
+            OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME
+        )
 
         return context
 
 
 @login_required
 @permission_required("opcalendar.create_event")
 def create_event(request):
```

### Comparing `aa_opcalendar-3.0.0b2/setup.py` & `aa_opcalendar-3.0.0b3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
+
 from setuptools import find_packages, setup
 
 from opcalendar import __version__
 
-
 # read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
@@ -38,9 +38,10 @@
     ],
     install_requires=[
         "allianceauth<5.0.0,>=4",
         "feedparser",
         "ics>=0.7.2",
         "pytz",
         "django-ical",
+        "requests-mock",
     ],
 )
```

### Comparing `aa_opcalendar-3.0.0b2/testauth/settings.py` & `aa_opcalendar-3.0.0b3/testauth/settings.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 This settings file contains everything needed for Alliance Auth projects to function.
 It gets overwritten by the 'allianceauth update' command.
 If you wish to make changes, overload the setting in your project's settings file (local.py).
 """
 
 import os
 
-from django.contrib import messages
 from celery.schedules import crontab
+from django.contrib import messages
 
 INSTALLED_APPS = [
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
```

