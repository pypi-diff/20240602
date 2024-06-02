# Comparing `tmp/heaobject-1.6.3.tar.gz` & `tmp/heaobject-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaobject-1.6.3.tar", last modified: Sat Jun  1 05:05:29 2024, max compression
+gzip compressed data, was "heaobject-1.6.4.tar", last modified: Sun Jun  2 16:06:22 2024, max compression
```

## Comparing `heaobject-1.6.3.tar` & `heaobject-1.6.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 05:05:29.369945 heaobject-1.6.3/
--rw-rw-rw-   0        0        0    11625 2023-06-22 19:55:16.000000 heaobject-1.6.3/LICENSE
--rw-rw-rw-   0        0        0     6492 2024-06-01 05:05:29.368901 heaobject-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     4986 2024-06-01 05:04:10.000000 heaobject-1.6.3/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 05:05:29.369945 heaobject-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     2603 2024-06-01 05:04:10.000000 heaobject-1.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:05:29.181307 heaobject-1.6.3/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 05:05:29.351263 heaobject-1.6.3/src/heaobject/
--rw-rw-rw-   0        0        0     1247 2023-10-30 17:37:04.000000 heaobject-1.6.3/src/heaobject/__init__.py
--rw-rw-rw-   0        0        0    11343 2024-05-31 23:54:03.000000 heaobject-1.6.3/src/heaobject/account.py
--rw-rw-rw-   0        0        0    15629 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/activity.py
--rw-rw-rw-   0        0        0     4030 2023-11-27 15:51:20.000000 heaobject-1.6.3/src/heaobject/aws.py
--rw-rw-rw-   0        0        0     6945 2023-12-12 22:05:30.000000 heaobject-1.6.3/src/heaobject/awss3key.py
--rw-rw-rw-   0        0        0     7587 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/bucket.py
--rw-rw-rw-   0        0        0     9988 2024-05-22 20:39:01.000000 heaobject-1.6.3/src/heaobject/data.py
--rw-rw-rw-   0        0        0     2604 2023-10-30 17:37:04.000000 heaobject-1.6.3/src/heaobject/dataadapter.py
--rw-rw-rw-   0        0        0      272 2023-06-22 19:55:16.000000 heaobject-1.6.3/src/heaobject/dataelement.py
--rw-rw-rw-   0        0        0     1601 2023-06-22 19:55:16.000000 heaobject-1.6.3/src/heaobject/datamodel.py
--rw-rw-rw-   0        0        0      430 2023-06-22 19:55:16.000000 heaobject-1.6.3/src/heaobject/datapattern.py
--rw-rw-rw-   0        0        0      238 2023-10-30 17:37:04.000000 heaobject-1.6.3/src/heaobject/datatransform.py
--rw-rw-rw-   0        0        0      353 2023-10-30 17:37:04.000000 heaobject-1.6.3/src/heaobject/error.py
--rw-rw-rw-   0        0        0    22016 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/folder.py
--rw-rw-rw-   0        0        0     4461 2024-06-01 05:04:10.000000 heaobject-1.6.3/src/heaobject/keychain.py
--rw-rw-rw-   0        0        0     2859 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/mimetype.py
--rw-rw-rw-   0        0        0    11772 2024-05-31 23:54:03.000000 heaobject-1.6.3/src/heaobject/organization.py
--rw-rw-rw-   0        0        0    13860 2024-06-01 05:04:10.000000 heaobject-1.6.3/src/heaobject/person.py
--rw-rw-rw-   0        0        0     5129 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/project.py
--rw-rw-rw-   0        0        0        0 2023-06-22 19:55:16.000000 heaobject-1.6.3/src/heaobject/py.typed
--rw-rw-rw-   0        0        0      211 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/record.py
--rw-rw-rw-   0        0        0    23497 2024-06-01 05:04:10.000000 heaobject-1.6.3/src/heaobject/registry.py
--rw-rw-rw-   0        0        0    80287 2024-06-01 05:04:10.000000 heaobject-1.6.3/src/heaobject/root.py
--rw-rw-rw-   0        0        0      597 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/settings.py
--rw-rw-rw-   0        0        0       66 2024-04-09 19:10:11.000000 heaobject-1.6.3/src/heaobject/source.py
--rw-rw-rw-   0        0        0     1165 2023-07-10 22:02:52.000000 heaobject-1.6.3/src/heaobject/source2target.py
--rw-rw-rw-   0        0        0     4074 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/storage.py
--rw-rw-rw-   0        0        0    10289 2024-04-22 18:44:54.000000 heaobject-1.6.3/src/heaobject/trash.py
--rw-rw-rw-   0        0        0     1217 2024-05-22 20:38:15.000000 heaobject-1.6.3/src/heaobject/user.py
--rw-rw-rw-   0        0        0      498 2023-10-30 17:37:04.000000 heaobject-1.6.3/src/heaobject/util.py
--rw-rw-rw-   0        0        0     7290 2024-05-22 20:39:01.000000 heaobject-1.6.3/src/heaobject/volume.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:05:29.367363 heaobject-1.6.3/src/heaobject.egg-info/
--rw-rw-rw-   0        0        0     6492 2024-06-01 05:05:29.000000 heaobject-1.6.3/src/heaobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      995 2024-06-01 05:05:29.000000 heaobject-1.6.3/src/heaobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 05:05:29.000000 heaobject-1.6.3/src/heaobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-06-01 05:05:29.000000 heaobject-1.6.3/src/heaobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-06-01 05:05:29.000000 heaobject-1.6.3/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 16:06:22.522901 heaobject-1.6.4/
+-rw-rw-rw-   0        0        0    11625 2023-06-22 19:55:16.000000 heaobject-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0     6590 2024-06-02 16:06:22.522901 heaobject-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5084 2024-06-02 16:03:28.000000 heaobject-1.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 16:06:22.523902 heaobject-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     2603 2024-06-02 16:03:46.000000 heaobject-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:06:22.298898 heaobject-1.6.4/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:06:22.503908 heaobject-1.6.4/src/heaobject/
+-rw-rw-rw-   0        0        0     1247 2023-10-30 17:37:04.000000 heaobject-1.6.4/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0    11343 2024-05-31 23:54:03.000000 heaobject-1.6.4/src/heaobject/account.py
+-rw-rw-rw-   0        0        0    15629 2024-04-16 21:52:49.000000 heaobject-1.6.4/src/heaobject/activity.py
+-rw-rw-rw-   0        0        0     4030 2023-11-27 15:51:20.000000 heaobject-1.6.4/src/heaobject/aws.py
+-rw-rw-rw-   0        0        0     6945 2023-12-12 22:05:30.000000 heaobject-1.6.4/src/heaobject/awss3key.py
+-rw-rw-rw-   0        0        0     7587 2024-04-16 21:52:49.000000 heaobject-1.6.4/src/heaobject/bucket.py
+-rw-rw-rw-   0        0        0     9988 2024-05-22 20:39:01.000000 heaobject-1.6.4/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     2604 2023-10-30 17:37:04.000000 heaobject-1.6.4/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2023-06-22 19:55:16.000000 heaobject-1.6.4/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2023-06-22 19:55:16.000000 heaobject-1.6.4/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2023-06-22 19:55:16.000000 heaobject-1.6.4/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      238 2023-10-30 17:37:04.000000 heaobject-1.6.4/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      353 2023-10-30 17:37:04.000000 heaobject-1.6.4/src/heaobject/error.py
+-rw-rw-rw-   0        0        0    22016 2024-04-16 21:52:49.000000 heaobject-1.6.4/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     4786 2024-06-02 15:56:41.000000 heaobject-1.6.4/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0     2859 2024-04-16 21:52:49.000000 heaobject-1.6.4/src/heaobject/mimetype.py
+-rw-rw-rw-   0        0        0    11772 2024-05-31 23:54:03.000000 heaobject-1.6.4/src/heaobject/organization.py
+-rw-rw-rw-   0        0        0    13860 2024-06-01 05:04:10.000000 heaobject-1.6.4/src/heaobject/person.py
+-rw-rw-rw-   0        0        0     5129 2024-04-16 21:52:49.000000 heaobject-1.6.4/src/heaobject/project.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 19:55:16.000000 heaobject-1.6.4/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      211 2024-04-16 21:52:49.000000 heaobject-1.6.4/src/heaobject/record.py
+-rw-rw-rw-   0        0        0    23442 2024-06-02 15:56:41.000000 heaobject-1.6.4/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    80287 2024-06-01 05:04:10.000000 heaobject-1.6.4/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      597 2024-04-16 21:52:49.000000 heaobject-1.6.4/src/heaobject/settings.py
+-rw-rw-rw-   0        0        0       66 2024-04-09 19:10:11.000000 heaobject-1.6.4/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1165 2023-07-10 22:02:52.000000 heaobject-1.6.4/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0     4074 2024-04-16 21:52:49.000000 heaobject-1.6.4/src/heaobject/storage.py
+-rw-rw-rw-   0        0        0    10289 2024-04-22 18:44:54.000000 heaobject-1.6.4/src/heaobject/trash.py
+-rw-rw-rw-   0        0        0     1217 2024-05-22 20:38:15.000000 heaobject-1.6.4/src/heaobject/user.py
+-rw-rw-rw-   0        0        0      498 2023-10-30 17:37:04.000000 heaobject-1.6.4/src/heaobject/util.py
+-rw-rw-rw-   0        0        0     7290 2024-05-22 20:39:01.000000 heaobject-1.6.4/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:06:22.521901 heaobject-1.6.4/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     6590 2024-06-02 16:06:22.000000 heaobject-1.6.4/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2024-06-02 16:06:22.000000 heaobject-1.6.4/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 16:06:22.000000 heaobject-1.6.4/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-06-02 16:06:22.000000 heaobject-1.6.4/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 16:06:22.000000 heaobject-1.6.4/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.6.3/LICENSE` & `heaobject-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/PKG-INFO` & `heaobject-1.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.6.3
+Version: 1.6.4
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,18 +33,21 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.4
+* Credential's expiration type changed from str to datetime
+* Added to AWS Credential the managed flag
+* Removed in Registry the check for NONE_USER to bypass having to be in is_creator_user list
+
 ## Version 1.6.3
-* credential's expiration type changed from str to datetime
-* registry in creator list no longer checks for NONE_USER
-* person now has access token object
+* Add to Person AccessToken object.
 
 ## Version 1.6.2
 * Fixed heaobject.account.AWSAccount.new_credentials() not setting the credentials' role.
 
 ## Version 1.6.1
 * For heaobject.organization.Organization, managers can now modify the manager and member lists.
```

### Comparing `heaobject-1.6.3/README.md` & `heaobject-1.6.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.4
+* Credential's expiration type changed from str to datetime
+* Added to AWS Credential the managed flag
+* Removed in Registry the check for NONE_USER to bypass having to be in is_creator_user list
+
 ## Version 1.6.3
-* credential's expiration type changed from str to datetime
-* registry in creator list no longer checks for NONE_USER
-* person now has access token object
+* Add to Person AccessToken object.
 
 ## Version 1.6.2
 * Fixed heaobject.account.AWSAccount.new_credentials() not setting the credentials' role.
 
 ## Version 1.6.1
 * For heaobject.organization.Organization, managers can now modify the manager and member lists.
```

### Comparing `heaobject-1.6.3/setup.py` & `heaobject-1.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.6.3',
+                 version='1.6.4',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
```

### Comparing `heaobject-1.6.3/src/heaobject/__init__.py` & `heaobject-1.6.4/src/heaobject/__init__.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/account.py` & `heaobject-1.6.4/src/heaobject/account.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/activity.py` & `heaobject-1.6.4/src/heaobject/activity.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/aws.py` & `heaobject-1.6.4/src/heaobject/aws.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/awss3key.py` & `heaobject-1.6.4/src/heaobject/awss3key.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/bucket.py` & `heaobject-1.6.4/src/heaobject/bucket.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/data.py` & `heaobject-1.6.4/src/heaobject/data.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/dataadapter.py` & `heaobject-1.6.4/src/heaobject/dataadapter.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/datamodel.py` & `heaobject-1.6.4/src/heaobject/datamodel.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/folder.py` & `heaobject-1.6.4/src/heaobject/folder.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/keychain.py` & `heaobject-1.6.4/src/heaobject/keychain.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 class AWSCredentials(Credentials):
     def __init__(self) -> None:
         super().__init__()
         self.__session_token: Optional[str] = None
         self.__expiration: Optional[str] = None
         self.__temporary = False
-
+        self.__managed = False
 
     @property  # type: ignore
     def session_token(self) -> Optional[str]:
         """
         The session token.
         """
         return self.__session_token
@@ -112,14 +112,23 @@
         """Whether or not to use AWS' temporary credentials generation mechanism. The default value is False."""
         return self.__temporary
 
     @temporary.setter
     def temporary(self, temporary: bool):
         self.__temporary = bool(temporary)
 
+    @property
+    def managed(self) -> bool:
+        """Flag to determine if AWS credential's lifecycle is managed by system. The default value is False."""
+        return self.__managed
+
+    @managed.setter
+    def managed(self, managed: bool):
+        self.__managed = bool(managed)
+
     def has_expired(self, exp_diff: int = 0):
         """
         This function assumes time will be provided in UTC per aws documentation
         and that the expiration time is a datetime str.
         :param exp_diff: the difference between expiration and current time in minutes (default to zero)
         :return: a boolean whether the token has expired or not
         :raise Value Error if expiration field cannot be parsed
```

### Comparing `heaobject-1.6.3/src/heaobject/mimetype.py` & `heaobject-1.6.4/src/heaobject/mimetype.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/organization.py` & `heaobject-1.6.4/src/heaobject/organization.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/person.py` & `heaobject-1.6.4/src/heaobject/person.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/project.py` & `heaobject-1.6.4/src/heaobject/project.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/registry.py` & `heaobject-1.6.4/src/heaobject/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,16 +161,14 @@
     def is_creator_user(self, sub: str) -> bool:
         """
         Returns whether the user is in the creator user list.
 
         :param sub: the user (required).
         :return: True or False.
         """
-        if sub == NONE_USER:
-            return True
         return sub in self.__creator_users
 
     @property
     def collection_accessor_users(self) -> list[str]:
         """
         Users who can access desktop objects managed by this resource via a Collection. An empty list means no one can
         access these objects via a Collection. Getting the users will return a de-duplicated list.
```

### Comparing `heaobject-1.6.3/src/heaobject/root.py` & `heaobject-1.6.4/src/heaobject/root.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/settings.py` & `heaobject-1.6.4/src/heaobject/settings.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/source2target.py` & `heaobject-1.6.4/src/heaobject/source2target.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/storage.py` & `heaobject-1.6.4/src/heaobject/storage.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/trash.py` & `heaobject-1.6.4/src/heaobject/trash.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/user.py` & `heaobject-1.6.4/src/heaobject/user.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject/volume.py` & `heaobject-1.6.4/src/heaobject/volume.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.3/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.6.4/src/heaobject.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.6.3
+Version: 1.6.4
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,18 +33,21 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.4
+* Credential's expiration type changed from str to datetime
+* Added to AWS Credential the managed flag
+* Removed in Registry the check for NONE_USER to bypass having to be in is_creator_user list
+
 ## Version 1.6.3
-* credential's expiration type changed from str to datetime
-* registry in creator list no longer checks for NONE_USER
-* person now has access token object
+* Add to Person AccessToken object.
 
 ## Version 1.6.2
 * Fixed heaobject.account.AWSAccount.new_credentials() not setting the credentials' role.
 
 ## Version 1.6.1
 * For heaobject.organization.Organization, managers can now modify the manager and member lists.
```

### Comparing `heaobject-1.6.3/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.6.4/src/heaobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

