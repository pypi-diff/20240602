# Comparing `tmp/profile_local-0.0.81.tar.gz` & `tmp/profile-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile_local-0.0.81.tar", last modified: Sun Jun  2 00:05:44 2024, max compression
+gzip compressed data, was "profile-local-0.0.9.tar", last modified: Mon Sep  4 10:55:38 2023, max compression
```

## Comparing `profile_local-0.0.81.tar` & `profile-local-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:05:44.901954 profile_local-0.0.81/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-06-02 00:05:44.897954 profile_local-0.0.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-06-02 00:05:12.000000 profile_local-0.0.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:05:44.897954 profile_local-0.0.81/profile_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:05:44.897954 profile_local-0.0.81/profile_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:05:12.000000 profile_local-0.0.81/profile_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-06-02 00:05:12.000000 profile_local-0.0.81/profile_local/src/comprehensive_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-06-02 00:05:12.000000 profile_local-0.0.81/profile_local/src/constants_profile_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-06-02 00:05:12.000000 profile_local-0.0.81/profile_local/src/profiles_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:05:44.897954 profile_local-0.0.81/profile_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-06-02 00:05:44.000000 profile_local-0.0.81/profile_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-06-02 00:05:44.000000 profile_local-0.0.81/profile_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:05:44.000000 profile_local-0.0.81/profile_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-06-02 00:05:44.000000 profile_local-0.0.81/profile_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 00:05:44.000000 profile_local-0.0.81/profile_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-02 00:05:18.000000 profile_local-0.0.81/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:05:44.901954 profile_local-0.0.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-06-02 00:05:12.000000 profile_local-0.0.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:38.903556 profile-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (999)      469 2023-09-04 10:55:38.899556 profile-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1008 2023-09-04 10:55:12.000000 profile-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:38.899556 profile-local-0.0.9/profile_local/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:12.000000 profile-local-0.0.9/profile_local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:38.899556 profile-local-0.0.9/profile_local/src/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:12.000000 profile-local-0.0.9/profile_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      824 2023-09-04 10:55:12.000000 profile-local-0.0.9/profile_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5794 2023-09-04 10:55:12.000000 profile-local-0.0.9/profile_local/src/generic_profile_insert.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8565 2023-09-04 10:55:12.000000 profile-local-0.0.9/profile_local/src/profiles_local.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 10:55:38.899556 profile-local-0.0.9/profile_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      469 2023-09-04 10:55:38.000000 profile-local-0.0.9/profile_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      348 2023-09-04 10:55:38.000000 profile-local-0.0.9/profile_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 10:55:38.000000 profile-local-0.0.9/profile_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       14 2023-09-04 10:55:38.000000 profile-local-0.0.9/profile_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      499 2023-09-04 10:55:12.000000 profile-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-04 10:55:38.903556 profile-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)      753 2023-09-04 10:55:12.000000 profile-local-0.0.9/setup.py
```

### Comparing `profile_local-0.0.81/profile_local/src/constants_profile_local.py` & `profile-local-0.0.9/profile_local/src/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from language_remote.lang_code import LangCode
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
-DEFAULT_LANG_CODE = LangCode.ENGLISH
-
 PROFILE_LOCAL_PYTHON_PACKAGE_COMPONENT_ID = 170
 PROFILE_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME = 'profile-local python package'
 
-PROFILE_LOCAL_PYTHON_LOGGER_CODE = {
+OBJECT_TO_INSERT_CODE = {
     'component_id': PROFILE_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
     'component_name': PROFILE_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': 'tal.g@circ.zone'
 }
 
 OBJECT_TO_INSERT_TEST = {
```

