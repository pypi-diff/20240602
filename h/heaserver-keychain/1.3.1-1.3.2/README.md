# Comparing `tmp/heaserver_keychain-1.3.1.tar.gz` & `tmp/heaserver_keychain-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_keychain-1.3.1.tar", last modified: Sat Jun  1 14:16:18 2024, max compression
+gzip compressed data, was "heaserver_keychain-1.3.2.tar", last modified: Sun Jun  2 17:01:39 2024, max compression
```

## Comparing `heaserver_keychain-1.3.1.tar` & `heaserver_keychain-1.3.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.347507 heaserver_keychain-1.3.1/
--rw-rw-rw-   0        0        0      325 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/.gitignore
--rw-rw-rw-   0        0        0     1579 2024-06-01 14:02:42.000000 heaserver_keychain-1.3.1/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      272 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5525 2024-06-01 14:16:18.346506 heaserver_keychain-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4199 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/README.md
--rw-rw-rw-   0        0        0     2654 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/RELEASING.md
--rw-rw-rw-   0        0        0      588 2024-06-01 14:02:42.000000 heaserver_keychain-1.3.1/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.219910 heaserver_keychain-1.3.1/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.219910 heaserver_keychain-1.3.1/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.289512 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     4195 2024-05-22 20:33:47.000000 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      404 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     1083 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     7770 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      109 2024-06-01 13:52:52.000000 heaserver_keychain-1.3.1/pytest.ini
--rw-rw-rw-   0        0        0      248 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/requirements_dev.txt
--rw-rw-rw-   0        0        0     1167 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-06-01 14:16:18.347507 heaserver_keychain-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1830 2024-06-01 14:14:19.000000 heaserver_keychain-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.220925 heaserver_keychain-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.220925 heaserver_keychain-1.3.1/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.297512 heaserver_keychain-1.3.1/src/heaserver/keychain/
--rw-rw-rw-   0        0        0        0 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/src/heaserver/keychain/__init__.py
--rw-rw-rw-   0        0        0    40816 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/src/heaserver/keychain/service.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.303512 heaserver_keychain-1.3.1/src/heaserver/keychain/wstl/
--rw-rw-rw-   0        0        0    19645 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/src/heaserver/keychain/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.344506 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/
--rw-rw-rw-   0        0        0     5525 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1111 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-06-01 14:16:18.000000 heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.221918 heaserver_keychain-1.3.1/tests/
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.221918 heaserver_keychain-1.3.1/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-06-01 14:16:18.342522 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/
--rw-rw-rw-   0        0        0        0 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/__init__.py
--rw-rw-rw-   0        0        0     3828 2024-05-22 20:33:47.000000 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/permissionstestcase.py
--rw-rw-rw-   0        0        0      404 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/test_all.py
--rw-rw-rw-   0        0        0     1083 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     7582 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.1/tests/heaserver/keychaintest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.717843 heaserver_keychain-1.3.2/
+-rw-rw-rw-   0        0        0      325 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/.gitignore
+-rw-rw-rw-   0        0        0     1579 2024-06-02 16:37:55.000000 heaserver_keychain-1.3.2/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5728 2024-06-02 17:01:39.716844 heaserver_keychain-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4402 2024-06-02 16:47:05.000000 heaserver_keychain-1.3.2/README.md
+-rw-rw-rw-   0        0        0     2654 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/RELEASING.md
+-rw-rw-rw-   0        0        0      588 2024-06-02 16:37:55.000000 heaserver_keychain-1.3.2/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.590444 heaserver_keychain-1.3.2/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.590444 heaserver_keychain-1.3.2/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.660859 heaserver_keychain-1.3.2/integrationtests/heaserver/keychainintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/integrationtests/heaserver/keychainintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     4195 2024-05-22 20:33:47.000000 heaserver_keychain-1.3.2/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      404 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/integrationtests/heaserver/keychainintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     1083 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     7770 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.2/integrationtests/heaserver/keychainintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      109 2024-06-01 13:52:52.000000 heaserver_keychain-1.3.2/pytest.ini
+-rw-rw-rw-   0        0        0      248 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/requirements_dev.txt
+-rw-rw-rw-   0        0        0     1167 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.2/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 17:01:39.717843 heaserver_keychain-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1830 2024-06-02 17:01:11.000000 heaserver_keychain-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.591443 heaserver_keychain-1.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.591443 heaserver_keychain-1.3.2/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.669854 heaserver_keychain-1.3.2/src/heaserver/keychain/
+-rw-rw-rw-   0        0        0        0 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/src/heaserver/keychain/__init__.py
+-rw-rw-rw-   0        0        0    40570 2024-06-02 16:43:54.000000 heaserver_keychain-1.3.2/src/heaserver/keychain/service.py
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.675851 heaserver_keychain-1.3.2/src/heaserver/keychain/wstl/
+-rw-rw-rw-   0        0        0    19645 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.2/src/heaserver/keychain/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.715844 heaserver_keychain-1.3.2/src/heaserver_keychain.egg-info/
+-rw-rw-rw-   0        0        0     5728 2024-06-02 17:01:39.000000 heaserver_keychain-1.3.2/src/heaserver_keychain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1111 2024-06-02 17:01:39.000000 heaserver_keychain-1.3.2/src/heaserver_keychain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 17:01:39.000000 heaserver_keychain-1.3.2/src/heaserver_keychain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-06-02 17:01:39.000000 heaserver_keychain-1.3.2/src/heaserver_keychain.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-06-02 17:01:39.000000 heaserver_keychain-1.3.2/src/heaserver_keychain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 17:01:39.000000 heaserver_keychain-1.3.2/src/heaserver_keychain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.592443 heaserver_keychain-1.3.2/tests/
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.592443 heaserver_keychain-1.3.2/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-02 17:01:39.714850 heaserver_keychain-1.3.2/tests/heaserver/keychaintest/
+-rw-rw-rw-   0        0        0        0 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/tests/heaserver/keychaintest/__init__.py
+-rw-rw-rw-   0        0        0     3828 2024-05-22 20:33:47.000000 heaserver_keychain-1.3.2/tests/heaserver/keychaintest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      404 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/tests/heaserver/keychaintest/test_all.py
+-rw-rw-rw-   0        0        0     1083 2023-07-26 20:25:42.000000 heaserver_keychain-1.3.2/tests/heaserver/keychaintest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     7582 2024-06-01 14:04:48.000000 heaserver_keychain-1.3.2/tests/heaserver/keychaintest/testcase.py
```

### Comparing `heaserver_keychain-1.3.1/Dockerfile` & `heaserver_keychain-1.3.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/LICENSE` & `heaserver_keychain-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/PKG-INFO` & `heaserver_keychain-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-keychain
-Version: 1.3.1
+Version: 1.3.2
 Summary: a service for managing laboratory credentials
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-keychain,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,21 +21,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.6.2
+Requires-Dist: heaserver~=1.6.3
 
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
+
+## Version 1.3.2
+* Upgrading dependencies to get bug fixes affecting creating and deleting Managed Credentials.
+* Increased delay of background task that checks to see if credentials are expired.
+
 ## Version 1.3.1
 * Introduces Managed Credentials with ability create and specify life span of credential 
 
 ## Version 1.3.0
 * Now all Credentials objects have a role attribute, replacing the old AWSCredentials role_arn attribute.
 
 ## Version 1.2.0
```

### Comparing `heaserver_keychain-1.3.1/README.md` & `heaserver_keychain-1.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
+
+## Version 1.3.2
+* Upgrading dependencies to get bug fixes affecting creating and deleting Managed Credentials.
+* Increased delay of background task that checks to see if credentials are expired.
+
 ## Version 1.3.1
 * Introduces Managed Credentials with ability create and specify life span of credential 
 
 ## Version 1.3.0
 * Now all Credentials objects have a role attribute, replacing the old AWSCredentials role_arn attribute.
 
 ## Version 1.2.0
```

### Comparing `heaserver_keychain-1.3.1/RELEASING.md` & `heaserver_keychain-1.3.2/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/docker-entrypoint.sh` & `heaserver_keychain-1.3.2/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py` & `heaserver_keychain-1.3.2/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py` & `heaserver_keychain-1.3.2/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/integrationtests/heaserver/keychainintegrationtest/testcase.py` & `heaserver_keychain-1.3.2/integrationtests/heaserver/keychainintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/run-swaggerui.py` & `heaserver_keychain-1.3.2/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/setup.py` & `heaserver_keychain-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-keychain',
-    version='1.3.1',
+    version='1.3.2',
     description="a service for managing laboratory credentials",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.keychain'],
     package_data={'heaserver.keychain': ['wstl/*.json']},
-    install_requires=['heaserver~=1.6.2'],
+    install_requires=['heaserver~=1.6.3'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver_keychain-1.3.1/src/heaserver/keychain/service.py` & `heaserver_keychain-1.3.2/src/heaserver/keychain/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -704,15 +704,14 @@
     """
     return await mongoservicelib.delete(request, MONGODB_CREDENTIALS_COLLECTION)
 
 
 @routes.delete('/credentials/{id}/managedawscredential')
 @routes.delete('/credentials/{id}/managedawscredential/')
 async def delete_aws_credential(request: web.Request) -> web.Response:
-    _logger.debug("Deleting managed credentials ")
     sub = request.headers.get(SUB, None)
     try:
 
         aws_cred = await _get_aws_cred(request)
         if aws_cred is None:
             return response.status_not_found("Could not get credential")
 
@@ -732,15 +731,14 @@
                 role_name: str = aws_cred.role[r_index:]
                 admin_cred = AWSCredentials()
                 admin_cred.role = await _get_admin_aws_role_arn(request=request, arn=aws_cred.role)
                 # force token to be expired to get new one for client
                 admin_cred = await request.app[HEA_DB].generate_cloud_credentials(request, admin_cred.role, usr_id)
                 admin_cred.id = usr_id
 
-                _logger.debug("About the get the admin credential CLIENT")
                 async with aws.IAMClientContext(request=request, credentials=admin_cred) as iam_admin_client:
                     try:
                         r_policies = await loop.run_in_executor(None,
                                                                 partial(iam_admin_client.list_attached_role_policies,
                                                                         RoleName=role_name))
                         await loop.run_in_executor(None, partial(_delete_managed_user, iam_client=iam_admin_client,
                                                                  username=aws_cred.name,
@@ -872,16 +870,14 @@
         exp_aws_creds = []
 
         async for cred in client.get_all(app=app, url=URL(component.base_url) / 'credentials',
                                          type_=AWSCredentials, headers=headers_):
 
             if cred.has_expired():
                 exp_aws_creds.append(cred)
-            else:
-                _logger.debug("creds expiration %s and the name %s" % (cred.expiration, cred.name))
 
         expired_aws_creds = [cred async for cred in client.get_all(app=app, url=URL(component.base_url) / 'credentials',
                                                                    type_=AWSCredentials, headers=headers_) if cred.managed and cred.has_expired()]
         _logger.debug("Managed Credentials to be deleted: %s" % expired_aws_creds)
 
         async def delete_credential(app_, url, headers):
             await client.delete(app_, url, headers)
@@ -930,9 +926,9 @@
 
 def main() -> None:
     config = init_cmd_line(description='a service for managing laboratory/user credentials',
                            default_port=8080)
     start(package_name='heaserver-keychain', db=aws.S3WithMongoManager,
           wstl_builder_factory=builder_factory(__package__),
           cleanup_ctx=[publisher_cleanup_context_factory(config),
-                       scheduled_cleanup_ctx(coro=delete_managed_coro, delay=20)],
+                       scheduled_cleanup_ctx(coro=delete_managed_coro, delay=3600)],
           config=config)
```

### Comparing `heaserver_keychain-1.3.1/src/heaserver/keychain/wstl/all.json` & `heaserver_keychain-1.3.2/src/heaserver/keychain/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/PKG-INFO` & `heaserver_keychain-1.3.2/src/heaserver_keychain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-keychain
-Version: 1.3.1
+Version: 1.3.2
 Summary: a service for managing laboratory credentials
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-keychain,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,21 +21,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.6.2
+Requires-Dist: heaserver~=1.6.3
 
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
+
+## Version 1.3.2
+* Upgrading dependencies to get bug fixes affecting creating and deleting Managed Credentials.
+* Increased delay of background task that checks to see if credentials are expired.
+
 ## Version 1.3.1
 * Introduces Managed Credentials with ability create and specify life span of credential 
 
 ## Version 1.3.0
 * Now all Credentials objects have a role attribute, replacing the old AWSCredentials role_arn attribute.
 
 ## Version 1.2.0
```

### Comparing `heaserver_keychain-1.3.1/src/heaserver_keychain.egg-info/SOURCES.txt` & `heaserver_keychain-1.3.2/src/heaserver_keychain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/tests/heaserver/keychaintest/permissionstestcase.py` & `heaserver_keychain-1.3.2/tests/heaserver/keychaintest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/tests/heaserver/keychaintest/test_all_with_bad_permissions.py` & `heaserver_keychain-1.3.2/tests/heaserver/keychaintest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.3.1/tests/heaserver/keychaintest/testcase.py` & `heaserver_keychain-1.3.2/tests/heaserver/keychaintest/testcase.py`

 * *Files identical despite different names*

