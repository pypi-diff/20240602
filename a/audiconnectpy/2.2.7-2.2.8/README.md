# Comparing `tmp/audiconnectpy-2.2.7.tar.gz` & `tmp/audiconnectpy-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.2.7.tar", last modified: Mon May 27 12:36:23 2024, max compression
+gzip compressed data, was "audiconnectpy-2.2.8.tar", last modified: Sun Jun  2 17:25:59 2024, max compression
```

## Comparing `audiconnectpy-2.2.7.tar` & `audiconnectpy-2.2.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.850142 audiconnectpy-2.2.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.850142 audiconnectpy-2.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.850142 audiconnectpy-2.2.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/fixtures/audi1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/fixtures/audi2.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:59.791557 audiconnectpy-2.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:59.787557 audiconnectpy-2.2.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:59.787557 audiconnectpy-2.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:59.787557 audiconnectpy-2.2.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-06-02 17:25:59.791557 audiconnectpy-2.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:59.787557 audiconnectpy-2.2.8/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26651 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:59.791557 audiconnectpy-2.2.8/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-06-02 17:25:59.000000 audiconnectpy-2.2.8/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-06-02 17:25:59.000000 audiconnectpy-2.2.8/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:25:59.000000 audiconnectpy-2.2.8/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:25:59.000000 audiconnectpy-2.2.8/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-02 17:25:59.000000 audiconnectpy-2.2.8/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 17:25:59.000000 audiconnectpy-2.2.8/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:25:59.791557 audiconnectpy-2.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:59.791557 audiconnectpy-2.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:25:59.791557 audiconnectpy-2.2.8/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/tests/fixtures/audi1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/tests/fixtures/audi2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-06-02 17:25:41.000000 audiconnectpy-2.2.8/tests/test_home.py
```

### Comparing `audiconnectpy-2.2.7/.github/dependabot.yml` & `audiconnectpy-2.2.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/.github/workflows/auto-approve.yml` & `audiconnectpy-2.2.8/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.2.8/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.2.8/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/.github/workflows/release.yml` & `audiconnectpy-2.2.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/.gitignore` & `audiconnectpy-2.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/.pre-commit-config.yaml` & `audiconnectpy-2.2.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/LICENSE` & `audiconnectpy-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/PKG-INFO` & `audiconnectpy-2.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.7
+Version: 2.2.8
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.7/README.md` & `audiconnectpy-2.2.8/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/audiconnectpy/api.py` & `audiconnectpy-2.2.8/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/audiconnectpy/auth.py` & `audiconnectpy-2.2.8/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/audiconnectpy/const.py` & `audiconnectpy-2.2.8/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/audiconnectpy/helpers.py` & `audiconnectpy-2.2.8/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/audiconnectpy/model.py` & `audiconnectpy-2.2.8/audiconnectpy/model.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/audiconnectpy/vehicle.py` & `audiconnectpy-2.2.8/audiconnectpy/vehicle.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     uris: dict[str, Any] = field(init=False)
     fill_region: Any = field(init=False)
     auth: Any = field(init=False)
     spin: str | None = field(init=False, default=None)
     infos: Information | None = field(
         metadata=field_options(alias="vehicle"), default=None
     )
-    capabilities: list[str] | None = field(init=False, default=None)
+    capabilities: list[str] = field(init=False, default_factory=list)
     position: Position | None = field(init=False, default=None)
     location: Location | None = field(init=False, default=None)
     last_update: datetime | None = field(init=False, default=None)
 
     @property
     def api_level(self) -> dict[str, int]:
         """Return API Level."""
@@ -175,19 +175,22 @@
             values: list[dict[str, Any]] = ExtendedDict(capabilities).getr(
                 "userCapabilities.capabilitiesStatus.value", []
             )
             self.capabilities: list[str] = [
                 str(d) for capability in values if (d := capability.get("id"))
             ]
 
-        str_jobs = ",".join(self.capabilities)  # type: ignore
+        caps = ",".join(self.capabilities)
+
+        str_jobs: str = f"{caps},userCapabilities" if caps != "" else caps
+
         headers = await self.auth.async_get_headers(token_type="idk")
         data = await self.auth.request(
             "GET",
-            f"{self.uris['cv_url']}/vehicles/{self.vin}/selectivestatus?jobs={str_jobs},userCapabilities",
+            f"{self.uris['cv_url']}/vehicles/{self.vin}/selectivestatus?jobs={str_jobs}",
             headers=headers,
         )
         return data
 
     async def async_set_lock(self, lock: bool) -> None:
         """Set lock."""
         security_token = await self._async_get_security_token(
```

### Comparing `audiconnectpy-2.2.7/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.2.8/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.7
+Version: 2.2.8
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.7/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.2.8/audiconnectpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/example.py` & `audiconnectpy-2.2.8/example.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/pyproject.toml` & `audiconnectpy-2.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/tests/conftest.py` & `audiconnectpy-2.2.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/tests/fixtures/audi0.json` & `audiconnectpy-2.2.8/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/tests/fixtures/audi1.json` & `audiconnectpy-2.2.8/tests/fixtures/audi1.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/tests/fixtures/audi2.json` & `audiconnectpy-2.2.8/tests/fixtures/audi2.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.2.8/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/tests/fixtures/location.json` & `audiconnectpy-2.2.8/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.7/tests/test_home.py` & `audiconnectpy-2.2.8/tests/test_home.py`

 * *Files identical despite different names*

