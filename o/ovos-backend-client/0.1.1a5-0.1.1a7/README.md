# Comparing `tmp/ovos-backend-client-0.1.1a5.tar.gz` & `tmp/ovos-backend-client-0.1.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-backend-client-0.1.1a5.tar", last modified: Fri Feb  9 14:27:19 2024, max compression
+gzip compressed data, was "ovos-backend-client-0.1.1a7.tar", last modified: Sun Jun  2 03:22:53 2024, max compression
```

## Comparing `ovos-backend-client-0.1.1a5.tar` & `ovos-backend-client-0.1.1a7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 14:27:19.434791 ovos-backend-client-0.1.1a5/
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-09 14:27:19.434791 ovos-backend-client-0.1.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 14:27:19.430791 ovos-backend-client-0.1.1a5/ovos_backend_client/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34050 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 14:27:19.430791 ovos-backend-client-0.1.1a5/ovos_backend_client/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27506 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    43400 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/backends/offline.py
--rw-r--r--   0 runner    (1001) docker     (127)    39319 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/backends/personal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/pairing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16539 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 14:27:19.430791 ovos-backend-client-0.1.1a5/ovos_backend_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/ovos_backend_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 14:27:19.434791 ovos-backend-client-0.1.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-02-09 14:27:19.000000 ovos-backend-client-0.1.1a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 03:22:53.395280 ovos-backend-client-0.1.1a7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-02 03:22:53.395280 ovos-backend-client-0.1.1a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 03:22:53.395280 ovos-backend-client-0.1.1a7/ovos_backend_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34050 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 03:22:53.395280 ovos-backend-client-0.1.1a7/ovos_backend_client/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27506 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43496 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/backends/offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39319 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/backends/personal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16539 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/ovos_backend_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 03:22:53.395280 ovos-backend-client-0.1.1a7/ovos_backend_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-02 03:22:53.000000 ovos-backend-client-0.1.1a7/ovos_backend_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-06-02 03:22:53.000000 ovos-backend-client-0.1.1a7/ovos_backend_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 03:22:53.000000 ovos-backend-client-0.1.1a7/ovos_backend_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-02 03:22:53.000000 ovos-backend-client-0.1.1a7/ovos_backend_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-02 03:22:53.000000 ovos-backend-client-0.1.1a7/ovos_backend_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 03:22:53.395280 ovos-backend-client-0.1.1a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-06-02 03:22:52.000000 ovos-backend-client-0.1.1a7/setup.py
```

### Comparing `ovos-backend-client-0.1.1a5/CHANGELOG.md` & `ovos-backend-client-0.1.1a7/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 # Changelog
 
-## [0.1.1a5](https://github.com/OpenVoiceOS/ovos-backend-client/tree/0.1.1a5) (2024-02-09)
+## [0.1.1a7](https://github.com/OpenVoiceOS/ovos-backend-client/tree/0.1.1a7) (2024-06-02)
 
-[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.1.1a4...0.1.1a5)
+[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.1.1a6...0.1.1a7)
+
+**Fixed bugs:**
+
+- Use generic tempdir path for broad support [\#68](https://github.com/OpenVoiceOS/ovos-backend-client/issues/68)
+- fix: allow cross-platform tempdir usage [\#69](https://github.com/OpenVoiceOS/ovos-backend-client/pull/69) ([mikejgray](https://github.com/mikejgray))
+
+## [V0.1.1a6](https://github.com/OpenVoiceOS/ovos-backend-client/tree/V0.1.1a6) (2024-04-17)
+
+[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.1.1a5...V0.1.1a6)
+
+**Fixed bugs:**
+
+- improve geolocation [\#67](https://github.com/OpenVoiceOS/ovos-backend-client/pull/67) ([JarbasAl](https://github.com/JarbasAl))
+
+## [V0.1.1a5](https://github.com/OpenVoiceOS/ovos-backend-client/tree/V0.1.1a5) (2024-02-09)
+
+[Full Changelog](https://github.com/OpenVoiceOS/ovos-backend-client/compare/V0.1.1a4...V0.1.1a5)
 
 **Implemented enhancements:**
 
 - feat/refresh\_oauth\_token [\#65](https://github.com/OpenVoiceOS/ovos-backend-client/pull/65) ([JarbasAl](https://github.com/JarbasAl))
 
 **Fixed bugs:**
```

### Comparing `ovos-backend-client-0.1.1a5/LICENSE` & `ovos-backend-client-0.1.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/README.md` & `ovos-backend-client-0.1.1a7/README.md`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client/api.py` & `ovos-backend-client-0.1.1a7/ovos_backend_client/api.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client/backends/__init__.py` & `ovos-backend-client-0.1.1a7/ovos_backend_client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client/backends/base.py` & `ovos-backend-client-0.1.1a7/ovos_backend_client/backends/base.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client/backends/offline.py` & `ovos-backend-client-0.1.1a7/ovos_backend_client/backends/offline.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,14 +260,16 @@
         address = details.get("address")
         location = {
             "address": details["display_name"],
             "city": {
                 "code": address.get("postcode") or "",
                 "name": address.get("city") or
                         address.get("village") or
+                        address.get("town") or
+                        address.get("hamlet") or
                         address.get("county") or "",
                 "state": {
                     "code": address.get("state_code") or
                             address.get("ISO3166-2-lvl4") or
                             address.get("ISO3166-2-lvl6")
                             or "",
                     "name": address.get("state") or
```

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client/backends/personal.py` & `ovos-backend-client-0.1.1a7/ovos_backend_client/backends/personal.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client/cloud.py` & `ovos-backend-client-0.1.1a7/ovos_backend_client/cloud.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client/config.py` & `ovos-backend-client-0.1.1a7/ovos_backend_client/config.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client/database.py` & `ovos-backend-client-0.1.1a7/ovos_backend_client/database.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client/identity.py` & `ovos-backend-client-0.1.1a7/ovos_backend_client/identity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
 import os
 import shutil
 import time
 from os.path import isfile, dirname, expanduser
+from tempfile import tempdir
 
 from combo_lock import ComboLock
 from ovos_config.config import get_xdg_config_save_path
 from ovos_config.meta import get_xdg_base
 from ovos_utils.log import LOG
 
-identity_lock = ComboLock('/tmp/identity-lock')
+identity_lock = ComboLock(f'{tempdir}/identity-lock')
 
 
 def find_identity():
     locations = [
         IdentityManager.OLD_IDENTITY_FILE,  # old location
         IdentityManager.IDENTITY_FILE,  # xdg location
         "~/mycroft-config/identity/identity2.json",  # smartgic docker default loc
```

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client/pairing.py` & `ovos-backend-client-0.1.1a7/ovos_backend_client/pairing.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client/settings.py` & `ovos-backend-client-0.1.1a7/ovos_backend_client/settings.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/ovos_backend_client.egg-info/SOURCES.txt` & `ovos-backend-client-0.1.1a7/ovos_backend_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.1.1a5/setup.py` & `ovos-backend-client-0.1.1a7/setup.py`

 * *Files identical despite different names*

