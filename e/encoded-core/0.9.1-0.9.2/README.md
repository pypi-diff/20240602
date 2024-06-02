# Comparing `tmp/encoded_core-0.9.1.tar.gz` & `tmp/encoded_core-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encoded_core-0.9.1.tar", max compression
+gzip compressed data, was "encoded_core-0.9.2.tar", max compression
```

## Comparing `encoded_core-0.9.1.tar` & `encoded_core-0.9.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1083 2024-06-01 13:45:01.689515 encoded_core-0.9.1/LICENSE
--rw-r--r--   0        0        0      174 2024-06-01 13:45:01.689515 encoded_core-0.9.1/README.rst
--rw-r--r--   0        0        0     3778 2024-06-01 13:45:01.689515 encoded_core-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2683 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/__init__.py
--rw-r--r--   0        0        0    32835 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/file_views.py
--rw-r--r--   0        0        0     4847 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/local_roles.py
--rw-r--r--   0        0        0    12807 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/page_views.py
--rw-r--r--   0        0        0      280 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/project_defs.py
--rw-r--r--   0        0        0     2490 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/qc_views.py
--rw-r--r--   0        0        0     1659 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/document.json
--rw-r--r--   0        0        0    14606 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/file.json
--rw-r--r--   0        0        0     4982 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/file_format.json
--rw-r--r--   0        0        0     4751 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/file_processed.json
--rw-r--r--   0        0        0     2161 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/file_reference.json
--rw-r--r--   0        0        0     1205 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/file_submitted.json
--rw-r--r--   0        0        0     1812 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/higlass_view_config.json
--rw-r--r--   0        0        0     1296 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/image.json
--rw-r--r--   0        0        0    13842 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/meta_workflow.json
--rw-r--r--   0        0        0    13367 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/meta_workflow_run.json
--rw-r--r--   0        0        0    16691 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/mixins.json
--rw-r--r--   0        0        0     5014 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/page.json
--rw-r--r--   0        0        0     1460 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/quality_metric.json
--rw-r--r--   0        0        0     3196 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/quality_metric_generic.json
--rw-r--r--   0        0        0     5660 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/software.json
--rw-r--r--   0        0        0     5340 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/static_section.json
--rw-r--r--   0        0        0    20417 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/tracking_item.json
--rw-r--r--   0        0        0     3396 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/user_content.json
--rw-r--r--   0        0        0    27190 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/workflow.json
--rw-r--r--   0        0        0    10478 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/workflow_run.json
--rw-r--r--   0        0        0     1914 2024-06-01 13:45:01.689515 encoded_core-0.9.1/src/encoded_core/schemas/workflow_run_awsem.json
--rw-r--r--   0        0        0        0 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/tests/__init__.py
--rw-r--r--   0        0        0    14054 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/tests/conftest.py
--rw-r--r--   0        0        0     1873 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/tests/conftest_settings.py
--rw-r--r--   0        0        0     7736 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/tests/datafixtures.py
--rw-r--r--   0        0        0     2171 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/tests/test_download_cli.py
--rw-r--r--   0        0        0    11010 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/tests/test_types_file.py
--rw-r--r--   0        0        0      262 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/tests/test_types_file_format.py
--rw-r--r--   0        0        0      239 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/tests/test_types_meta_workflow.py
--rw-r--r--   0        0        0      212 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/tests/test_types_software.py
--rw-r--r--   0        0        0      502 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/tests/test_types_workflow.py
--rw-r--r--   0        0        0       70 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/__init__.py
--rw-r--r--   0        0        0     1284 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/document.py
--rw-r--r--   0        0        0    20541 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/file.py
--rw-r--r--   0        0        0      789 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/file_format.py
--rw-r--r--   0        0        0     2297 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/file_processed.py
--rw-r--r--   0        0        0      462 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/file_reference.py
--rw-r--r--   0        0        0     1970 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/file_submitted.py
--rw-r--r--   0        0        0      584 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/higlass_view_config.py
--rw-r--r--   0        0        0     1040 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/image.py
--rw-r--r--   0        0        0     3217 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/meta_workflow.py
--rw-r--r--   0        0        0      858 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/page.py
--rw-r--r--   0        0        0     1314 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/quality_metric.py
--rw-r--r--   0        0        0      479 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/quality_metric_generic.py
--rw-r--r--   0        0        0     2750 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/software.py
--rw-r--r--   0        0        0     3847 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/tracking_item.py
--rw-r--r--   0        0        0     5468 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/user_content.py
--rw-r--r--   0        0        0    12886 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/types/workflow.py
--rw-r--r--   0        0        0     1522 2024-06-01 13:45:01.693516 encoded_core-0.9.1/src/encoded_core/upgrade.py
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 encoded_core-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-06-02 14:37:19.090987 encoded_core-0.9.2/LICENSE
+-rw-r--r--   0        0        0      174 2024-06-02 14:37:19.090987 encoded_core-0.9.2/README.rst
+-rw-r--r--   0        0        0     3778 2024-06-02 14:37:19.094987 encoded_core-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2683 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/__init__.py
+-rw-r--r--   0        0        0    32947 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/file_views.py
+-rw-r--r--   0        0        0     4847 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/local_roles.py
+-rw-r--r--   0        0        0    12807 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/page_views.py
+-rw-r--r--   0        0        0      280 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/project_defs.py
+-rw-r--r--   0        0        0     2490 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/qc_views.py
+-rw-r--r--   0        0        0     1659 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/document.json
+-rw-r--r--   0        0        0    14606 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/file.json
+-rw-r--r--   0        0        0     4982 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/file_format.json
+-rw-r--r--   0        0        0     4751 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/file_processed.json
+-rw-r--r--   0        0        0     2161 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/file_reference.json
+-rw-r--r--   0        0        0     1205 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/file_submitted.json
+-rw-r--r--   0        0        0     1812 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/higlass_view_config.json
+-rw-r--r--   0        0        0     1296 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/image.json
+-rw-r--r--   0        0        0    13842 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/meta_workflow.json
+-rw-r--r--   0        0        0    13367 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/meta_workflow_run.json
+-rw-r--r--   0        0        0    16691 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/mixins.json
+-rw-r--r--   0        0        0     5014 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/page.json
+-rw-r--r--   0        0        0     1460 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/quality_metric.json
+-rw-r--r--   0        0        0     3196 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/quality_metric_generic.json
+-rw-r--r--   0        0        0     5660 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/software.json
+-rw-r--r--   0        0        0     5340 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/static_section.json
+-rw-r--r--   0        0        0    20417 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/tracking_item.json
+-rw-r--r--   0        0        0     3396 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/user_content.json
+-rw-r--r--   0        0        0    27190 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/workflow.json
+-rw-r--r--   0        0        0    10478 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/workflow_run.json
+-rw-r--r--   0        0        0     1914 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/schemas/workflow_run_awsem.json
+-rw-r--r--   0        0        0        0 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/tests/__init__.py
+-rw-r--r--   0        0        0    14054 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/tests/conftest.py
+-rw-r--r--   0        0        0     1873 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/tests/conftest_settings.py
+-rw-r--r--   0        0        0     7736 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/tests/datafixtures.py
+-rw-r--r--   0        0        0     2171 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/tests/test_download_cli.py
+-rw-r--r--   0        0        0    11010 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/tests/test_types_file.py
+-rw-r--r--   0        0        0      262 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/tests/test_types_file_format.py
+-rw-r--r--   0        0        0      239 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/tests/test_types_meta_workflow.py
+-rw-r--r--   0        0        0      212 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/tests/test_types_software.py
+-rw-r--r--   0        0        0      502 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/tests/test_types_workflow.py
+-rw-r--r--   0        0        0       70 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/__init__.py
+-rw-r--r--   0        0        0     1284 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/document.py
+-rw-r--r--   0        0        0    20541 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/file.py
+-rw-r--r--   0        0        0      789 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/file_format.py
+-rw-r--r--   0        0        0     2297 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/file_processed.py
+-rw-r--r--   0        0        0      462 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/file_reference.py
+-rw-r--r--   0        0        0     1970 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/file_submitted.py
+-rw-r--r--   0        0        0      584 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/higlass_view_config.py
+-rw-r--r--   0        0        0     1040 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/image.py
+-rw-r--r--   0        0        0     3217 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/meta_workflow.py
+-rw-r--r--   0        0        0      858 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/page.py
+-rw-r--r--   0        0        0     1314 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/quality_metric.py
+-rw-r--r--   0        0        0      479 2024-06-02 14:37:19.094987 encoded_core-0.9.2/src/encoded_core/types/quality_metric_generic.py
+-rw-r--r--   0        0        0     2750 2024-06-02 14:37:19.098987 encoded_core-0.9.2/src/encoded_core/types/software.py
+-rw-r--r--   0        0        0     3847 2024-06-02 14:37:19.098987 encoded_core-0.9.2/src/encoded_core/types/tracking_item.py
+-rw-r--r--   0        0        0     5468 2024-06-02 14:37:19.098987 encoded_core-0.9.2/src/encoded_core/types/user_content.py
+-rw-r--r--   0        0        0    12886 2024-06-02 14:37:19.098987 encoded_core-0.9.2/src/encoded_core/types/workflow.py
+-rw-r--r--   0        0        0     1522 2024-06-02 14:37:19.098987 encoded_core-0.9.2/src/encoded_core/upgrade.py
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 encoded_core-0.9.2/PKG-INFO
```

### Comparing `encoded_core-0.9.1/LICENSE` & `encoded_core-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/pyproject.toml` & `encoded_core-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encoded-core"
-version = "0.9.1"
+version = "0.9.2"
 description = "Core data models for Park Lab ENCODE based projects"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/smaht-dac/encoded-core"
 repository = "https://github.com/smaht-dac/encoded-core"
 documentation = "https://github.com/smaht-dac/encoded-core"
```

### Comparing `encoded_core-0.9.1/src/encoded_core/__init__.py` & `encoded_core-0.9.2/src/encoded_core/__init__.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/file_views.py` & `encoded_core-0.9.2/src/encoded_core/file_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,16 +305,17 @@
     ga_config = request.registry.settings.get('ga_config')
 
     if ga_config:
         submitter_title = get_submitter_title(request, context, properties)
         exp_or_assay_type = get_experiment_or_assay_type(request, context, properties)
         file_type = get_file_type(request, context, properties)
         file_at_id = context.jsonld_id(request)
+        dataset = properties.get('dataset')
         update_google_analytics(context, request, ga_config, filename, file_size_downloaded, file_at_id, submitter_title,
-                                user_uuid, user_groups, exp_or_assay_type, file_type)
+                                user_uuid, user_groups, exp_or_assay_type, dataset, file_type)
 
     if asbool(request.params.get('soft')):
         expires = int(parse_qs(urlparse(location).query)['Expires'][0])
         return {
             '@type': ['SoftRedirect'],
             'location': location,
             'expires': datetime.datetime.fromtimestamp(expires, pytz.utc).isoformat(),
@@ -377,15 +378,15 @@
         if len(properties.get('data_category')) > 0:
             return properties.get('data_category')[0]
     # 4DN/fallback
     return properties.get('file_type') or 'other'
 
 
 def update_google_analytics(context, request, ga_config, filename, file_size_downloaded,
-                            file_at_id, submitter_title, user_uuid, user_groups, exp_or_assay_type, file_type='other'):
+                            file_at_id, submitter_title, user_uuid, user_groups, exp_or_assay_type, dataset, file_type='other'):
     """ Helper for @@download that updates GA in response to a download.
     """
     registry = request.registry
     ga4_secret = registry.settings.get('ga4.secret')
     if not ga4_secret:
         raise Exception("No valid GA4 api secret found")
 
@@ -421,14 +422,15 @@
                     "action": "Range Query" if request.range else "File Download",
                     "file_name": filename,
                     "file_extension": file_extension,
                     "link_url": request.url,
                     "file_size": file_size_downloaded,
                     "downloads": 0 if request.range else 1,
                     "experiment_type": exp_or_assay_type or "None",
+                    "dataset": dataset or "None",
                     "lab": submitter_title or "None",
                     # Product Category from @type, e.g. "File/FileProcessed"
                     "file_classification": "/".join(item_types),
                     "file_type": file_type,
                     "items": [
                         {
                             "item_id": file_at_id,
```

### Comparing `encoded_core-0.9.1/src/encoded_core/local_roles.py` & `encoded_core-0.9.2/src/encoded_core/local_roles.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/page_views.py` & `encoded_core-0.9.2/src/encoded_core/page_views.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/qc_views.py` & `encoded_core-0.9.2/src/encoded_core/qc_views.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/document.json` & `encoded_core-0.9.2/src/encoded_core/schemas/document.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/file.json` & `encoded_core-0.9.2/src/encoded_core/schemas/file.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/file_format.json` & `encoded_core-0.9.2/src/encoded_core/schemas/file_format.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/file_processed.json` & `encoded_core-0.9.2/src/encoded_core/schemas/file_processed.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/file_reference.json` & `encoded_core-0.9.2/src/encoded_core/schemas/file_reference.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/file_submitted.json` & `encoded_core-0.9.2/src/encoded_core/schemas/file_submitted.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/higlass_view_config.json` & `encoded_core-0.9.2/src/encoded_core/schemas/higlass_view_config.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/image.json` & `encoded_core-0.9.2/src/encoded_core/schemas/image.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/meta_workflow.json` & `encoded_core-0.9.2/src/encoded_core/schemas/meta_workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/meta_workflow_run.json` & `encoded_core-0.9.2/src/encoded_core/schemas/meta_workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/mixins.json` & `encoded_core-0.9.2/src/encoded_core/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/page.json` & `encoded_core-0.9.2/src/encoded_core/schemas/page.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/quality_metric.json` & `encoded_core-0.9.2/src/encoded_core/schemas/quality_metric.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/quality_metric_generic.json` & `encoded_core-0.9.2/src/encoded_core/schemas/quality_metric_generic.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/software.json` & `encoded_core-0.9.2/src/encoded_core/schemas/software.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/static_section.json` & `encoded_core-0.9.2/src/encoded_core/schemas/static_section.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/tracking_item.json` & `encoded_core-0.9.2/src/encoded_core/schemas/tracking_item.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/user_content.json` & `encoded_core-0.9.2/src/encoded_core/schemas/user_content.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/workflow.json` & `encoded_core-0.9.2/src/encoded_core/schemas/workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/workflow_run.json` & `encoded_core-0.9.2/src/encoded_core/schemas/workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/schemas/workflow_run_awsem.json` & `encoded_core-0.9.2/src/encoded_core/schemas/workflow_run_awsem.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/tests/conftest.py` & `encoded_core-0.9.2/src/encoded_core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/tests/conftest_settings.py` & `encoded_core-0.9.2/src/encoded_core/tests/conftest_settings.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/tests/datafixtures.py` & `encoded_core-0.9.2/src/encoded_core/tests/datafixtures.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/tests/test_download_cli.py` & `encoded_core-0.9.2/src/encoded_core/tests/test_download_cli.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/tests/test_types_file.py` & `encoded_core-0.9.2/src/encoded_core/tests/test_types_file.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/document.py` & `encoded_core-0.9.2/src/encoded_core/types/document.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/file.py` & `encoded_core-0.9.2/src/encoded_core/types/file.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/file_format.py` & `encoded_core-0.9.2/src/encoded_core/types/file_format.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/file_processed.py` & `encoded_core-0.9.2/src/encoded_core/types/file_processed.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/file_submitted.py` & `encoded_core-0.9.2/src/encoded_core/types/file_submitted.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/higlass_view_config.py` & `encoded_core-0.9.2/src/encoded_core/types/higlass_view_config.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/image.py` & `encoded_core-0.9.2/src/encoded_core/types/image.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/meta_workflow.py` & `encoded_core-0.9.2/src/encoded_core/types/meta_workflow.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/page.py` & `encoded_core-0.9.2/src/encoded_core/types/page.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/quality_metric.py` & `encoded_core-0.9.2/src/encoded_core/types/quality_metric.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/software.py` & `encoded_core-0.9.2/src/encoded_core/types/software.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/tracking_item.py` & `encoded_core-0.9.2/src/encoded_core/types/tracking_item.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/user_content.py` & `encoded_core-0.9.2/src/encoded_core/types/user_content.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/types/workflow.py` & `encoded_core-0.9.2/src/encoded_core/types/workflow.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/src/encoded_core/upgrade.py` & `encoded_core-0.9.2/src/encoded_core/upgrade.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.9.1/PKG-INFO` & `encoded_core-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encoded-core
-Version: 0.9.1
+Version: 0.9.2
 Summary: Core data models for Park Lab ENCODE based projects
 Home-page: https://github.com/smaht-dac/encoded-core
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 3 - Alpha
```

