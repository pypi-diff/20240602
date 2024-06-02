# Comparing `tmp/url_remote-0.0.97.tar.gz` & `tmp/url_remote-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "url_remote-0.0.97.tar", last modified: Wed May 29 14:04:06 2024, max compression
+gzip compressed data, was "url_remote-0.0.98.tar", last modified: Sun Jun  2 01:39:55 2024, max compression
```

## Comparing `url_remote-0.0.97.tar` & `url_remote-0.0.98.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:04:06.639021 url_remote-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-29 14:04:06.639021 url_remote-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 14:03:53.000000 url_remote-0.0.97/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-29 14:03:59.000000 url_remote-0.0.97/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:04:06.639021 url_remote-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-29 14:03:53.000000 url_remote-0.0.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:04:06.635021 url_remote-0.0.97/url_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:04:06.639021 url_remote-0.0.97/url_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/action_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/api_version_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/authentiction_api_version_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/brand_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/component_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/entity_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/environment_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/our_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-29 14:03:53.000000 url_remote-0.0.97/url_remote/src/url_circlez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:04:06.639021 url_remote-0.0.97/url_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-29 14:04:06.000000 url_remote-0.0.97/url_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-29 14:04:06.000000 url_remote-0.0.97/url_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:04:06.000000 url_remote-0.0.97/url_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 14:04:06.000000 url_remote-0.0.97/url_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:39:55.065153 url_remote-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-06-02 01:39:55.065153 url_remote-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-06-02 01:39:42.000000 url_remote-0.0.98/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-02 01:39:48.000000 url_remote-0.0.98/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 01:39:55.065153 url_remote-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-06-02 01:39:42.000000 url_remote-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:39:55.061153 url_remote-0.0.98/url_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:39:55.065153 url_remote-0.0.98/url_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 01:39:42.000000 url_remote-0.0.98/url_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-06-02 01:39:42.000000 url_remote-0.0.98/url_remote/src/action_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-06-02 01:39:42.000000 url_remote-0.0.98/url_remote/src/api_version_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-02 01:39:42.000000 url_remote-0.0.98/url_remote/src/authentiction_api_version_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-02 01:39:42.000000 url_remote-0.0.98/url_remote/src/brand_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-02 01:39:42.000000 url_remote-0.0.98/url_remote/src/component_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-06-02 01:39:42.000000 url_remote-0.0.98/url_remote/src/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-06-02 01:39:42.000000 url_remote-0.0.98/url_remote/src/entity_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-02 01:39:42.000000 url_remote-0.0.98/url_remote/src/environment_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-06-02 01:39:42.000000 url_remote-0.0.98/url_remote/src/our_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-06-02 01:39:42.000000 url_remote-0.0.98/url_remote/src/url_circlez.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 01:39:55.065153 url_remote-0.0.98/url_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-06-02 01:39:55.000000 url_remote-0.0.98/url_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-06-02 01:39:55.000000 url_remote-0.0.98/url_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 01:39:55.000000 url_remote-0.0.98/url_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 01:39:55.000000 url_remote-0.0.98/url_remote.egg-info/top_level.txt
```

### Comparing `url_remote-0.0.97/README.md` & `url_remote-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.97/setup.py` & `url_remote-0.0.98/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "url-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.97',  # https://pypi.org/project/url-remote
+    version='0.0.98',  # https://pypi.org/project/url-remote
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="URL Local",
```

### Comparing `url_remote-0.0.97/url_remote/src/action_name_enum.py` & `url_remote-0.0.98/url_remote/src/action_name_enum.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.97/url_remote/src/api_version_dicts.py` & `url_remote-0.0.98/url_remote/src/api_version_dicts.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.97/url_remote/src/component_name_enum.py` & `url_remote-0.0.98/url_remote/src/component_name_enum.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.97/url_remote/src/domain.py` & `url_remote-0.0.98/url_remote/src/domain.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.97/url_remote/src/our_url.py` & `url_remote-0.0.98/url_remote/src/our_url.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 
 from .brand_name_enum import BrandName
 from .environment_name_enum import EnvironmentName
 
 
 class OurUrl:
     # static dict for domain mapping
+    base_url = 'execute-api.us-east-1.amazonaws.com'
     domain_mapping = {
-        'auth.dvlp1.circ.zone': 'i4wp5o2381.execute-api.us-east-1.amazonaws.com',
-        'auth.play1.circ.zone': 'nmxjjpyrv9.execute-api.us-east-1.amazonaws.com',
-        'user-registration.dvlp1.circ.zone': 'lczo7l194b.execute-api.us-east-1.amazonaws.com',
-        'user-registration.play1.circ.zone': 't3tnkh0r64.execute-api.us-east-1.amazonaws.com',
-        'gender-detection.dvlp1.circ.zone': '353sstqmj5.execute-api.us-east-1.amazonaws.com',
-        'gender-detection.play1.circ.zone': '353sstqmj5.execute-api.us-east-1.amazonaws.com',
-        'group.dvlp1.circ.zone': '2mvpuqbhh1.execute-api.us-east-1.amazonaws.com',
-        'group.play1.circ.zone': 'ly0jegwkib.execute-api.us-east-1.amazonaws.com',
-        'group-profile.dvlp1.circ.zone': 'dot2ynvxwl.execute-api.us-east-1.amazonaws.com',
-        'group-profile.play1.circ.zone': 'wh1toflnza.execute-api.us-east-1.amazonaws.com',
-        'marketplace-goods.play1.circ.zone': 'vcev0rrt01.execute-api.us-east-1.amazonaws.com',
-        'logger.dvlp1.circ.zone': 't91y4nxsye.execute-api.us-east-1.amazonaws.com',
-        'logger.play1.circ.zone': 'fsujmjyfal.execute-api.us-east-1.amazonaws.com',
-        # 'event.play1.circ.zone': 'p89mpsr5m1.execute-api.us-east-1.amazonaws.com',
-        # 'event.play1.circ.zone': 'x8ql0j9cwf.execute-api.us-east-1.amazonaws.com',
-        'event.play1.circ.zone': '2iclscptqh.execute-api.us-east-1.amazonaws.com',
-        'event.dvlp1.circ.zone': 'wbq5liyk63.execute-api.us-east-1.amazonaws.com',
-        'storage.play1.circ.zone': 'wbq5liyk63.execute-api.us-east-1.amazonaws.com',  # TODO update
-        'storage.dvlp1.circ.zone': 'wbq5liyk63.execute-api.us-east-1.amazonaws.com',  # TODO update
-        'smartlink.play1.circ.zone': 'ezt1n60if7.execute-api.us-east-1.amazonaws.com',
-        'smartlink.dvlp1.circ.zone': 'u5ohxnpxug.execute-api.us-east-1.amazonaws.com',
-        'dialogWorkflow.play1.circ.zone': 'g91pb4afb1.execute-api.us-east-1.amazonaws.com/dev',
-        'dialogWorkflow.dvlp1.circ.zone': 'xoonx24zbg.execute-api.us-east-1.amazonaws.com/dev',
+        'auth.dvlp1.circ.zone': 'i4wp5o2381.' + base_url,
+        'auth.play1.circ.zone': 'nmxjjpyrv9.' + base_url,
+        'user-registration.dvlp1.circ.zone': 'lczo7l194b.' + base_url,
+        'user-registration.play1.circ.zone': 't3tnkh0r64.' + base_url,
+        'gender-detection.dvlp1.circ.zone': '353sstqmj5.' + base_url,  # TODO: update
+        'gender-detection.play1.circ.zone': '353sstqmj5.' + base_url,
+        'group.dvlp1.circ.zone': '2mvpuqbhh1.' + base_url,
+        'group.play1.circ.zone': 'ly0jegwkib.' + base_url,
+        'group-profile.dvlp1.circ.zone': 'dot2ynvxwl.' + base_url,
+        'group-profile.play1.circ.zone': 'wh1toflnza.' + base_url,
+        'marketplace-goods.play1.circ.zone': 'vcev0rrt01.' + base_url,
+        'logger.dvlp1.circ.zone': 't91y4nxsye.' + base_url,
+        'logger.play1.circ.zone': 'fsujmjyfal.' + base_url,
+        # 'event.play1.circ.zone': 'p89mpsr5m1.' + base_url,
+        # 'event.play1.circ.zone': 'x8ql0j9cwf.' + base_url,
+        'event.play1.circ.zone': 'g1u5iwrq0h.' + base_url,
+        'event.dvlp1.circ.zone': 'wbq5liyk63.' + base_url,  # TODO update
+        'storage.play1.circ.zone': 'wbq5liyk63.' + base_url,  # TODO update
+        'storage.dvlp1.circ.zone': 'wbq5liyk63.' + base_url,  # TODO update
+        'smartlink.play1.circ.zone': 'ezt1n60if7.' + base_url,
+        'smartlink.dvlp1.circ.zone': 'u5ohxnpxug.' + base_url,
+        'dialogWorkflow.play1.circ.zone': f'g91pb4afb1.{base_url}/dev',  # TODO: replace http with httpApi in yml to remove dev
+        'dialogWorkflow.dvlp1.circ.zone': f'xoonx24zbg.{base_url}/dev',
         # 'websocket.dvlp1.circ.zone': 'ws://23.22.217.199:8080',
         # 'websocket.play1.circ.zone': 'ws://23.22.217.199:8080',
     }
 
     @staticmethod
     def _base_domain(brand_name: str, environment_name: str) -> str:
         """
```

### Comparing `url_remote-0.0.97/url_remote.egg-info/SOURCES.txt` & `url_remote-0.0.98/url_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

