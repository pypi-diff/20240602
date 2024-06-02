# Comparing `tmp/organization_profile_local-0.0.7.tar.gz` & `tmp/organization_profile_local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "organization_profile_local-0.0.7.tar", last modified: Mon May 27 07:30:30 2024, max compression
+gzip compressed data, was "organization_profile_local-0.0.8.tar", last modified: Sun Jun  2 10:36:06 2024, max compression
```

## Comparing `organization_profile_local-0.0.7.tar` & `organization_profile_local-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:30:30.228272 organization_profile_local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-27 07:30:30.228272 organization_profile_local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 07:30:00.000000 organization_profile_local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:30:30.224272 organization_profile_local-0.0.7/organization_profile_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:30:30.224272 organization_profile_local-0.0.7/organization_profile_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:30:00.000000 organization_profile_local-0.0.7/organization_profile_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-27 07:30:00.000000 organization_profile_local-0.0.7/organization_profile_local/src/organization_profile_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-05-27 07:30:00.000000 organization_profile_local-0.0.7/organization_profile_local/src/organization_profiles_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:30:30.224272 organization_profile_local-0.0.7/organization_profile_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-27 07:30:30.000000 organization_profile_local-0.0.7/organization_profile_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-27 07:30:30.000000 organization_profile_local-0.0.7/organization_profile_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:30:30.000000 organization_profile_local-0.0.7/organization_profile_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-27 07:30:30.000000 organization_profile_local-0.0.7/organization_profile_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 07:30:30.000000 organization_profile_local-0.0.7/organization_profile_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-27 07:30:06.000000 organization_profile_local-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:30:30.228272 organization_profile_local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-27 07:30:00.000000 organization_profile_local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:36:06.025100 organization_profile_local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-06-02 10:36:06.021100 organization_profile_local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 10:35:30.000000 organization_profile_local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:36:06.021100 organization_profile_local-0.0.8/organization_profile_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:36:06.021100 organization_profile_local-0.0.8/organization_profile_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 10:35:30.000000 organization_profile_local-0.0.8/organization_profile_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-06-02 10:35:30.000000 organization_profile_local-0.0.8/organization_profile_local/src/organization_profile_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-06-02 10:35:30.000000 organization_profile_local-0.0.8/organization_profile_local/src/organization_profiles_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:36:06.021100 organization_profile_local-0.0.8/organization_profile_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-06-02 10:36:06.000000 organization_profile_local-0.0.8/organization_profile_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-06-02 10:36:06.000000 organization_profile_local-0.0.8/organization_profile_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:36:06.000000 organization_profile_local-0.0.8/organization_profile_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-02 10:36:06.000000 organization_profile_local-0.0.8/organization_profile_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-02 10:36:06.000000 organization_profile_local-0.0.8/organization_profile_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-06-02 10:35:36.000000 organization_profile_local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 10:36:06.025100 organization_profile_local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-06-02 10:35:30.000000 organization_profile_local-0.0.8/setup.py
```

### Comparing `organization_profile_local-0.0.7/PKG-INFO` & `organization_profile_local-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: organization-profile-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles organization-profile-local Python
 Home-page: https://github.com/circles-zone/organization-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `organization_profile_local-0.0.7/organization_profile_local/src/organization_profile_constants.py` & `organization_profile_local-0.0.8/organization_profile_local/src/organization_profile_constants.py`

 * *Files identical despite different names*

### Comparing `organization_profile_local-0.0.7/organization_profile_local/src/organization_profiles_local.py` & `organization_profile_local-0.0.8/organization_profile_local/src/organization_profiles_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,25 @@
                         object={"organization_id": organization_id, "profile_id": profile_id})
             logger.end(object={"organization_profile_id": organization_profile_id})
             return organization_profile_id
         organization_profile_id = self.insert_mapping(organization_id=organization_id, profile_id=profile_id)
         logger.end(object={"organization_profile_id": organization_profile_id})
         return organization_profile_id
 
+    def insert_multiple_mappings_if_not_exists(self, organization_ids: list[int], profile_ids: list[int]) -> list[int]:
+        logger.start(object={"organization_ids": organization_ids, "profile_ids": profile_ids})
+        organization_profile_ids = []
+        for organization_id in organization_ids:
+            for profile_id in profile_ids:
+                organization_profile_id = self.insert_mapping_if_not_exists(organization_id=organization_id,
+                                                                            profile_id=profile_id)
+                organization_profile_ids.append(organization_profile_id)
+        logger.end(object={"organization_profile_ids": organization_profile_ids})
+        return organization_profile_ids
+
     def get_profile_id_and_organization_id(self, organization_profile_id: int) -> dict[str, int]:
         logger.start(object={"organization_profile_id": organization_profile_id})
         result = self.select_one_dict_by_id(
             select_clause_value="organization_id, profile_id",
             id_column_name=DEFAULT_ID_COLUMN_NAME,
             id_column_value=organization_profile_id
         )
@@ -88,15 +99,14 @@
         )
         organization_ids_list = [organization_id for (organization_id,) in organization_ids_tuple_list]
         logger.end(object={"organization_ids_list": organization_ids_list})
         return organization_ids_list
 
     def get_organization_profile_id(self, organization_id: int, profile_id: int) -> int | None:
         logger.start(object={"organization_id": organization_id, "profile_id": profile_id})
-        organization_profile_id_dict = self.select_one_dict_by_where(
+        organization_profile_id = self.select_one_value_by_where(
             select_clause_value="organization_profile_id",
             where="organization_id = %s AND profile_id = %s",
             params=(organization_id, profile_id)
         )
-        organization_profile_id = organization_profile_id_dict.get("organization_profile_id", None)
         logger.end(object={"organization_profile_id": organization_profile_id})
         return organization_profile_id
```

### Comparing `organization_profile_local-0.0.7/organization_profile_local.egg-info/PKG-INFO` & `organization_profile_local-0.0.8/organization_profile_local.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: organization-profile-local
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyPI Package for Circles organization-profile-local Python
 Home-page: https://github.com/circles-zone/organization-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `organization_profile_local-0.0.7/setup.py` & `organization_profile_local-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "organization-profile-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.7',  # update only the minor version each time # https://pypi.org/project/organization-profile-local/
+    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/organization-profile-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles organization-profile-local Python",
     long_description="PyPI Package for Circles organization-profile-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/organization-profile-local-python-package",
     packages=[package_dir],
```
