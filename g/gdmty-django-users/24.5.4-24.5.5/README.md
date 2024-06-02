# Comparing `tmp/gdmty_django_users-24.5.4.tar.gz` & `tmp/gdmty_django_users-24.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmty_django_users-24.5.4.tar", last modified: Sat Jun  1 02:34:26 2024, max compression
+gzip compressed data, was "gdmty_django_users-24.5.5.tar", last modified: Sun Jun  2 03:54:59 2024, max compression
```

## Comparing `gdmty_django_users-24.5.4.tar` & `gdmty_django_users-24.5.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 02:34:26.161927 gdmty_django_users-24.5.4/
--rw-rw-rw-   0        0        0    35182 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.4/LICENSE
--rw-rw-rw-   0        0        0       51 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0    43714 2024-06-01 02:34:26.161927 gdmty_django_users-24.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     2113 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/README.md
--rw-rw-rw-   0        0        0     1527 2024-06-01 02:34:15.000000 gdmty_django_users-24.5.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-01 02:34:26.161927 gdmty_django_users-24.5.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-01 02:34:26.145283 gdmty_django_users-24.5.4/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 02:34:26.154786 gdmty_django_users-24.5.4/src/gdmty_django_users/
--rw-rw-rw-   0        0        0     1367 2024-06-01 02:34:15.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/__init__.py
--rw-rw-rw-   0        0        0     2477 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/admin.py
--rw-rw-rw-   0        0        0     1048 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/apps.py
--rw-rw-rw-   0        0        0     1437 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/decorators.py
--rw-rw-rw-   0        0        0     2332 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/managers.py
-drwxrwxrwx   0        0        0        0 2024-06-01 02:34:26.161927 gdmty_django_users-24.5.4/src/gdmty_django_users/migrations/
--rw-rw-rw-   0        0        0     3284 2024-05-10 04:28:25.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1333 2024-05-10 04:29:08.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py
--rw-rw-rw-   0        0        0      880 2024-06-01 02:15:27.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/migrations/0003_alter_user_groups_alter_user_user_permissions.py
--rw-rw-rw-   0        0        0        0 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/migrations/__init__.py
--rw-rw-rw-   0        0        0     3209 2024-05-31 21:39:31.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/models.py
--rw-rw-rw-   0        0        0     1819 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/permissions.py
--rw-rw-rw-   0        0        0     1763 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/serializers.py
--rw-rw-rw-   0        0        0     1065 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/settings.py
--rw-rw-rw-   0        0        0      910 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/tests.py
--rw-rw-rw-   0        0        0     1756 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/urls.py
--rw-rw-rw-   0        0        0     4811 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/viewsets.py
--rw-rw-rw-   0        0        0     1471 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.4/src/gdmty_django_users/wagtail_forms.py
-drwxrwxrwx   0        0        0        0 2024-06-01 02:34:26.161927 gdmty_django_users-24.5.4/src/gdmty_django_users.egg-info/
--rw-rw-rw-   0        0        0    43714 2024-06-01 02:34:26.000000 gdmty_django_users-24.5.4/src/gdmty_django_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-06-01 02:34:26.000000 gdmty_django_users-24.5.4/src/gdmty_django_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 02:34:26.000000 gdmty_django_users-24.5.4/src/gdmty_django_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2024-06-01 02:34:26.000000 gdmty_django_users-24.5.4/src/gdmty_django_users.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-06-01 02:34:26.000000 gdmty_django_users-24.5.4/src/gdmty_django_users.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 03:54:59.901087 gdmty_django_users-24.5.5/
+-rw-rw-rw-   0        0        0    35182 2024-03-16 06:30:23.000000 gdmty_django_users-24.5.5/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-03-16 06:30:23.000000 gdmty_django_users-24.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    43714 2024-06-02 03:54:59.901087 gdmty_django_users-24.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/README.md
+-rw-rw-rw-   0        0        0     1527 2024-06-02 03:54:25.000000 gdmty_django_users-24.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 03:54:59.901087 gdmty_django_users-24.5.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 03:54:59.877559 gdmty_django_users-24.5.5/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 03:54:59.890580 gdmty_django_users-24.5.5/src/gdmty_django_users/
+-rw-rw-rw-   0        0        0     1367 2024-06-02 03:54:25.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/__init__.py
+-rw-rw-rw-   0        0        0     2477 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/admin.py
+-rw-rw-rw-   0        0        0     1048 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/apps.py
+-rw-rw-rw-   0        0        0     1437 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/decorators.py
+-rw-rw-rw-   0        0        0     2332 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/managers.py
+drwxrwxrwx   0        0        0        0 2024-06-02 03:54:59.898970 gdmty_django_users-24.5.5/src/gdmty_django_users/migrations/
+-rw-rw-rw-   0        0        0     3284 2024-03-17 01:44:29.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1333 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py
+-rw-rw-rw-   0        0        0      880 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/migrations/0003_alter_user_groups_alter_user_user_permissions.py
+-rw-rw-rw-   0        0        0        0 2024-03-16 06:30:23.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3209 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/models.py
+-rw-rw-rw-   0        0        0     1819 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/permissions.py
+-rw-rw-rw-   0        0        0     1957 2024-06-02 03:53:42.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/serializers.py
+-rw-rw-rw-   0        0        0     1065 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/settings.py
+-rw-rw-rw-   0        0        0      910 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/tests.py
+-rw-rw-rw-   0        0        0     1756 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/urls.py
+-rw-rw-rw-   0        0        0     4811 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/viewsets.py
+-rw-rw-rw-   0        0        0     1471 2024-06-02 03:52:30.000000 gdmty_django_users-24.5.5/src/gdmty_django_users/wagtail_forms.py
+drwxrwxrwx   0        0        0        0 2024-06-02 03:54:59.898970 gdmty_django_users-24.5.5/src/gdmty_django_users.egg-info/
+-rw-rw-rw-   0        0        0    43714 2024-06-02 03:54:59.000000 gdmty_django_users-24.5.5/src/gdmty_django_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-06-02 03:54:59.000000 gdmty_django_users-24.5.5/src/gdmty_django_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 03:54:59.000000 gdmty_django_users-24.5.5/src/gdmty_django_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2024-06-02 03:54:59.000000 gdmty_django_users-24.5.5/src/gdmty_django_users.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-06-02 03:54:59.000000 gdmty_django_users-24.5.5/src/gdmty_django_users.egg-info/top_level.txt
```

### Comparing `gdmty_django_users-24.5.4/LICENSE` & `gdmty_django_users-24.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/PKG-INFO` & `gdmty_django_users-24.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.5.4
+Version: 24.5.5
 Summary: Extension of Django's AbstractBaseUser for user management, using email as user.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdmty_django_users-24.5.4/README.md` & `gdmty_django_users-24.5.5/README.md`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/pyproject.toml` & `gdmty_django_users-24.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdmty-django-users"
-version = "24.5.4"
+version = "24.5.5"
 description = "Extension of Django's AbstractBaseUser for user management, using email as user."
 readme = "README.md"
 authors = [{ name="Gobierno de Monterrey", email="cesar.benjamin@monterrey.gob.mx" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
@@ -31,15 +31,15 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 "Homepage" = "https://github.com/gobiernodigitalmonterrey/gdmty-django-users"
 "Bug Tracker" = "https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues"
 
 [tool.bumpver]
-current_version = "24.5.4"
+current_version = "24.5.5"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/__init__.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 
 """
 
 __title__ = "gdmty_django_users"
-__version__ = "24.5.4"
+__version__ = "24.5.5"
 __description__ = "Django module for Users models and permission adding reCAPTCHA token verification."
 __url__ = "https://github.com/SIGAMty/gdmty-django-recaptcha-enterprise"
 __author__ = "César Benjamín"
 __author_email__ = "mathereall@gmail.com"
 __license__ = "GNU Affero General Public License v3 or later (AGPLv3+)"
 __keywords__ = ["django", "users"]
 VERSION = __version__
```

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/admin.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/admin.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/apps.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/apps.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/decorators.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/decorators.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/managers.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/managers.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/migrations/0001_initial.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/migrations/0003_alter_user_groups_alter_user_user_permissions.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/migrations/0003_alter_user_groups_alter_user_user_permissions.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/models.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/models.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/permissions.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/permissions.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/serializers.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,22 +23,23 @@
 
 
 class UserSerializer(serializers.ModelSerializer):
 
     class Meta:
         model = User
         exclude = ['password', 'first_name', 'last_name', 'is_staff', 'is_superuser', 'user_permissions', 'safe_delete',
-                   'is_active']
-        read_only_fields = ['last_login', 'username', 'date_joined', 'email', 'groups']
+                   'is_active', 'email_verificado']
+        read_only_fields = ['id', 'last_login', 'username', 'date_joined', 'email', 'groups']
 
 
 class AdminUserSerializer(serializers.ModelSerializer):
     class Meta:
         model = User
-        exclude = ['password', 'first_name', 'last_name']
+        exclude = ['password', 'first_name', 'last_name', 'is_staff', 'is_superuser', 'user_permissions', 'safe_delete', 'email_verificado']
+        read_only_fields = ['id', 'last_login', 'username', 'date_joined', 'email']
 
 
 class GroupSerializer(serializers.ModelSerializer):
     class Meta:
         model = Group
         fields = '__all__'
```

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/settings.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/settings.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/tests.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/tests.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/urls.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/urls.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/viewsets.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/viewsets.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users/wagtail_forms.py` & `gdmty_django_users-24.5.5/src/gdmty_django_users/wagtail_forms.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users.egg-info/PKG-INFO` & `gdmty_django_users-24.5.5/src/gdmty_django_users.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.5.4
+Version: 24.5.5
 Summary: Extension of Django's AbstractBaseUser for user management, using email as user.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdmty_django_users-24.5.4/src/gdmty_django_users.egg-info/SOURCES.txt` & `gdmty_django_users-24.5.5/src/gdmty_django_users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

