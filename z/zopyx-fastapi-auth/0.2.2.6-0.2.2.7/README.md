# Comparing `tmp/zopyx_fastapi_auth-0.2.2.6.tar.gz` & `tmp/zopyx_fastapi_auth-0.2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zopyx_fastapi_auth-0.2.2.6.tar", last modified: Fri May 24 13:22:25 2024, max compression
+gzip compressed data, was "zopyx_fastapi_auth-0.2.2.7.tar", last modified: Sun Jun  2 17:22:06 2024, max compression
```

## Comparing `zopyx_fastapi_auth-0.2.2.6.tar` & `zopyx_fastapi_auth-0.2.2.7.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 13:22:25.194987 zopyx_fastapi_auth-0.2.2.6/
--rw-------   0 ajung     (1000) ajung     (1000)       98 2024-05-24 04:56:20.000000 zopyx_fastapi_auth-0.2.2.6/MANIFEST.in
--rw-r--r--   0 ajung     (1000) ajung     (1000)     6844 2024-05-24 13:22:25.194987 zopyx_fastapi_auth-0.2.2.6/PKG-INFO
--rw-------   0 ajung     (1000) ajung     (1000)     5788 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/README.md
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 13:22:25.186987 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/
--rw-------   0 ajung     (1000) ajung     (1000)       14 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/__init__.py
--rw-------   0 ajung     (1000) ajung     (1000)      347 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/auth_config.py
--rw-------   0 ajung     (1000) ajung     (1000)     2122 2024-05-24 04:50:07.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/auth_routes.py
--rw-------   0 ajung     (1000) ajung     (1000)     3008 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/demo_app.py
--rw-------   0 ajung     (1000) ajung     (1000)     2509 2024-05-24 05:58:47.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/dependencies.py
--rw-------   0 ajung     (1000) ajung     (1000)      290 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/jinja2_templates.py
--rw-------   0 ajung     (1000) ajung     (1000)      106 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/logger.py
--rw-------   0 ajung     (1000) ajung     (1000)      294 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/permissions.py
--rw-------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 13:22:04.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/py.typed
--rw-------   0 ajung     (1000) ajung     (1000)     1716 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/roles.py
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 13:22:25.186987 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/templates/
--rw-------   0 ajung     (1000) ajung     (1000)     1408 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/templates/base.html
--rw-------   0 ajung     (1000) ajung     (1000)      564 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/templates/demo.html
--rw-------   0 ajung     (1000) ajung     (1000)      881 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/templates/login.html
--rw-------   0 ajung     (1000) ajung     (1000)     2001 2024-05-24 05:50:58.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/user_cmd.py
--rw-------   0 ajung     (1000) ajung     (1000)     4500 2024-05-24 13:20:37.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/user_management_sqlobject.py
--rw-------   0 ajung     (1000) ajung     (1000)     2220 2024-05-24 11:13:37.000000 zopyx_fastapi_auth-0.2.2.6/fastapi_auth/users.py
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 13:22:25.190987 zopyx_fastapi_auth-0.2.2.6/images/
--rw-------   0 ajung     (1000) ajung     (1000)   172868 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/images/logged-in.png
--rw-------   0 ajung     (1000) ajung     (1000)    86854 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/images/login.png
--rw-------   0 ajung     (1000) ajung     (1000)     1143 2024-05-24 13:22:13.000000 zopyx_fastapi_auth-0.2.2.6/pyproject.toml
--rw-------   0 ajung     (1000) ajung     (1000)       38 2024-05-24 13:22:25.194987 zopyx_fastapi_auth-0.2.2.6/setup.cfg
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 13:22:25.186987 zopyx_fastapi_auth-0.2.2.6/static/
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 13:22:25.186987 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 13:22:25.194987 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/
--rw-------   0 ajung     (1000) ajung     (1000)    70329 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css
--rw-------   0 ajung     (1000) ajung     (1000)   203221 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    51795 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   115986 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    70403 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   203225 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    51870 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   116063 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    12065 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css
--rw-------   0 ajung     (1000) ajung     (1000)   129371 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    10126 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css
--rw-------   0 ajung     (1000) ajung     (1000)    51369 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    12058 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   129386 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    10198 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)    63943 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   107823 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css
--rw-------   0 ajung     (1000) ajung     (1000)   267535 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    85352 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   180381 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   107691 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   267476 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)    85281 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   180217 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   281046 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.css
--rw-------   0 ajung     (1000) ajung     (1000)   679755 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   232803 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   589892 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   280259 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css
--rw-------   0 ajung     (1000) ajung     (1000)   679615 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map
--rw-------   0 ajung     (1000) ajung     (1000)   232911 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css
--rw-------   0 ajung     (1000) ajung     (1000)   589087 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 13:22:25.194987 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/
--rw-------   0 ajung     (1000) ajung     (1000)   207819 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js
--rw-------   0 ajung     (1000) ajung     (1000)   444579 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map
--rw-------   0 ajung     (1000) ajung     (1000)    80721 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js
--rw-------   0 ajung     (1000) ajung     (1000)   332090 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map
--rw-------   0 ajung     (1000) ajung     (1000)   135829 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js
--rw-------   0 ajung     (1000) ajung     (1000)   305438 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map
--rw-------   0 ajung     (1000) ajung     (1000)    73935 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js
--rw-------   0 ajung     (1000) ajung     (1000)   222455 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map
--rw-------   0 ajung     (1000) ajung     (1000)   145401 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.js
--rw-------   0 ajung     (1000) ajung     (1000)   306606 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.js.map
--rw-------   0 ajung     (1000) ajung     (1000)    60635 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.min.js
--rw-------   0 ajung     (1000) ajung     (1000)   220561 2024-05-24 04:47:20.000000 zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map
-drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-24 13:22:25.194987 zopyx_fastapi_auth-0.2.2.6/zopyx_fastapi_auth.egg-info/
--rw-r--r--   0 ajung     (1000) ajung     (1000)     6844 2024-05-24 13:22:25.000000 zopyx_fastapi_auth-0.2.2.6/zopyx_fastapi_auth.egg-info/PKG-INFO
--rw-------   0 ajung     (1000) ajung     (1000)     3240 2024-05-24 13:22:25.000000 zopyx_fastapi_auth-0.2.2.6/zopyx_fastapi_auth.egg-info/SOURCES.txt
--rw-------   0 ajung     (1000) ajung     (1000)        1 2024-05-24 13:22:25.000000 zopyx_fastapi_auth-0.2.2.6/zopyx_fastapi_auth.egg-info/dependency_links.txt
--rw-------   0 ajung     (1000) ajung     (1000)       71 2024-05-24 13:22:25.000000 zopyx_fastapi_auth-0.2.2.6/zopyx_fastapi_auth.egg-info/entry_points.txt
--rw-------   0 ajung     (1000) ajung     (1000)      184 2024-05-24 13:22:25.000000 zopyx_fastapi_auth-0.2.2.6/zopyx_fastapi_auth.egg-info/requires.txt
--rw-------   0 ajung     (1000) ajung     (1000)       13 2024-05-24 13:22:25.000000 zopyx_fastapi_auth-0.2.2.6/zopyx_fastapi_auth.egg-info/top_level.txt
+drwx------   0 ajung      (501) staff       (20)        0 2024-06-02 17:22:06.796149 zopyx_fastapi_auth-0.2.2.7/
+-rw-------   0 ajung      (501) staff       (20)       98 2024-05-26 13:08:38.000000 zopyx_fastapi_auth-0.2.2.7/MANIFEST.in
+-rw-r--r--   0 ajung      (501) staff       (20)     9014 2024-06-02 17:22:06.795463 zopyx_fastapi_auth-0.2.2.7/PKG-INFO
+-rw-------   0 ajung      (501) staff       (20)     8008 2024-06-02 16:41:01.000000 zopyx_fastapi_auth-0.2.2.7/README.md
+drwx------   0 ajung      (501) staff       (20)        0 2024-06-02 17:22:06.301032 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/
+-rw-------   0 ajung      (501) staff       (20)       14 2024-05-19 14:39:22.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/__init__.py
+-rw-------   0 ajung      (501) staff       (20)      389 2024-06-02 17:10:53.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/auth_config.py
+-rw-------   0 ajung      (501) staff       (20)     2377 2024-06-02 17:15:26.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/auth_routes.py
+-rw-------   0 ajung      (501) staff       (20)      811 2024-05-30 07:25:55.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/authenticator_registry.py
+-rw-------   0 ajung      (501) staff       (20)     3220 2024-05-30 07:15:19.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/demo_app.py
+-rw-------   0 ajung      (501) staff       (20)     2476 2024-05-27 18:23:57.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/dependencies.py
+-rw-------   0 ajung      (501) staff       (20)      290 2024-05-21 18:43:26.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/jinja2_templates.py
+-rw-------   0 ajung      (501) staff       (20)      169 2024-06-02 17:11:29.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/logger.py
+-rw-------   0 ajung      (501) staff       (20)      294 2024-05-21 00:42:54.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/permissions.py
+-rw-------   0 ajung      (501) staff       (20)        0 2024-05-26 13:08:38.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/py.typed
+-rw-------   0 ajung      (501) staff       (20)     1716 2024-05-22 00:02:44.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/roles.py
+drwx------   0 ajung      (501) staff       (20)        0 2024-06-02 17:22:06.302245 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/templates/
+-rw-------   0 ajung      (501) staff       (20)     1408 2024-05-20 21:21:36.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/templates/base.html
+-rw-------   0 ajung      (501) staff       (20)      564 2024-05-20 23:56:11.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/templates/demo.html
+-rw-------   0 ajung      (501) staff       (20)      881 2024-05-20 16:51:19.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/templates/login.html
+-rw-------   0 ajung      (501) staff       (20)     2001 2024-05-26 13:08:38.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/user_cmd.py
+-rw-------   0 ajung      (501) staff       (20)     4830 2024-05-30 07:15:54.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/user_management_sqlobject.py
+-rw-------   0 ajung      (501) staff       (20)     2196 2024-05-27 18:24:32.000000 zopyx_fastapi_auth-0.2.2.7/fastapi_auth/users.py
+drwx------   0 ajung      (501) staff       (20)        0 2024-06-02 17:22:06.307429 zopyx_fastapi_auth-0.2.2.7/images/
+-rw-------   0 ajung      (501) staff       (20)   172868 2024-05-23 15:32:26.000000 zopyx_fastapi_auth-0.2.2.7/images/logged-in.png
+-rw-------   0 ajung      (501) staff       (20)    86854 2024-05-23 15:32:26.000000 zopyx_fastapi_auth-0.2.2.7/images/login.png
+-rw-------   0 ajung      (501) staff       (20)     1100 2024-06-02 17:21:33.000000 zopyx_fastapi_auth-0.2.2.7/pyproject.toml
+-rw-------   0 ajung      (501) staff       (20)       38 2024-06-02 17:22:06.796248 zopyx_fastapi_auth-0.2.2.7/setup.cfg
+drwx------   0 ajung      (501) staff       (20)        0 2024-06-02 17:22:06.294307 zopyx_fastapi_auth-0.2.2.7/static/
+drwx------   0 ajung      (501) staff       (20)        0 2024-06-02 17:22:06.294599 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/
+drwx------   0 ajung      (501) staff       (20)        0 2024-06-02 17:22:06.707803 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/
+-rw-------   0 ajung      (501) staff       (20)    70329 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css
+-rw-------   0 ajung      (501) staff       (20)   203221 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map
+-rw-------   0 ajung      (501) staff       (20)    51795 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css
+-rw-------   0 ajung      (501) staff       (20)   115986 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map
+-rw-------   0 ajung      (501) staff       (20)    70403 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css
+-rw-------   0 ajung      (501) staff       (20)   203225 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map
+-rw-------   0 ajung      (501) staff       (20)    51870 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css
+-rw-------   0 ajung      (501) staff       (20)   116063 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map
+-rw-------   0 ajung      (501) staff       (20)    12065 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css
+-rw-------   0 ajung      (501) staff       (20)   129371 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map
+-rw-------   0 ajung      (501) staff       (20)    10126 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css
+-rw-------   0 ajung      (501) staff       (20)    51369 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map
+-rw-------   0 ajung      (501) staff       (20)    12058 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css
+-rw-------   0 ajung      (501) staff       (20)   129386 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map
+-rw-------   0 ajung      (501) staff       (20)    10198 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css
+-rw-------   0 ajung      (501) staff       (20)    63943 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-------   0 ajung      (501) staff       (20)   107823 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css
+-rw-------   0 ajung      (501) staff       (20)   267535 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map
+-rw-------   0 ajung      (501) staff       (20)    85352 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css
+-rw-------   0 ajung      (501) staff       (20)   180381 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map
+-rw-------   0 ajung      (501) staff       (20)   107691 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css
+-rw-------   0 ajung      (501) staff       (20)   267476 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map
+-rw-------   0 ajung      (501) staff       (20)    85281 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css
+-rw-------   0 ajung      (501) staff       (20)   180217 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-------   0 ajung      (501) staff       (20)   281046 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.css
+-rw-------   0 ajung      (501) staff       (20)   679755 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.css.map
+-rw-------   0 ajung      (501) staff       (20)   232803 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.min.css
+-rw-------   0 ajung      (501) staff       (20)   589892 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map
+-rw-------   0 ajung      (501) staff       (20)   280259 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css
+-rw-------   0 ajung      (501) staff       (20)   679615 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map
+-rw-------   0 ajung      (501) staff       (20)   232911 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css
+-rw-------   0 ajung      (501) staff       (20)   589087 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map
+drwx------   0 ajung      (501) staff       (20)        0 2024-06-02 17:22:06.790449 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/
+-rw-------   0 ajung      (501) staff       (20)   207819 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js
+-rw-------   0 ajung      (501) staff       (20)   444579 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map
+-rw-------   0 ajung      (501) staff       (20)    80721 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js
+-rw-------   0 ajung      (501) staff       (20)   332090 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map
+-rw-------   0 ajung      (501) staff       (20)   135829 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js
+-rw-------   0 ajung      (501) staff       (20)   305438 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map
+-rw-------   0 ajung      (501) staff       (20)    73935 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js
+-rw-------   0 ajung      (501) staff       (20)   222455 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map
+-rw-------   0 ajung      (501) staff       (20)   145401 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.js
+-rw-------   0 ajung      (501) staff       (20)   306606 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.js.map
+-rw-------   0 ajung      (501) staff       (20)    60635 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.min.js
+-rw-------   0 ajung      (501) staff       (20)   220561 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map
+drwx------   0 ajung      (501) staff       (20)        0 2024-06-02 17:22:06.794452 zopyx_fastapi_auth-0.2.2.7/zopyx_fastapi_auth.egg-info/
+-rw-r--r--   0 ajung      (501) staff       (20)     9014 2024-06-02 17:22:06.000000 zopyx_fastapi_auth-0.2.2.7/zopyx_fastapi_auth.egg-info/PKG-INFO
+-rw-------   0 ajung      (501) staff       (20)     3279 2024-06-02 17:22:06.000000 zopyx_fastapi_auth-0.2.2.7/zopyx_fastapi_auth.egg-info/SOURCES.txt
+-rw-------   0 ajung      (501) staff       (20)        1 2024-06-02 17:22:06.000000 zopyx_fastapi_auth-0.2.2.7/zopyx_fastapi_auth.egg-info/dependency_links.txt
+-rw-------   0 ajung      (501) staff       (20)       71 2024-06-02 17:22:06.000000 zopyx_fastapi_auth-0.2.2.7/zopyx_fastapi_auth.egg-info/entry_points.txt
+-rw-------   0 ajung      (501) staff       (20)      184 2024-06-02 17:22:06.000000 zopyx_fastapi_auth-0.2.2.7/zopyx_fastapi_auth.egg-info/requires.txt
+-rw-------   0 ajung      (501) staff       (20)       13 2024-06-02 17:22:06.000000 zopyx_fastapi_auth-0.2.2.7/zopyx_fastapi_auth.egg-info/top_level.txt
```

### Comparing `zopyx_fastapi_auth-0.2.2.6/PKG-INFO` & `zopyx_fastapi_auth-0.2.2.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,28 @@
-Metadata-Version: 2.1
-Name: zopyx-fastapi-auth
-Version: 0.2.2.6
-Summary: FastAPI authentication and authorization
-Author-email: Andreas Jung <info@zopyx.com>
-Project-URL: homepage, https://github.com/zopyx/fastapi-auth
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-Requires-Dist: fastapi
-Requires-Dist: pydantic
-Requires-Dist: pydantic-settings
-Requires-Dist: uvicorn
-Requires-Dist: markdown
-Requires-Dist: starlette-session
-Requires-Dist: loguru
-Requires-Dist: bcrypt
-Requires-Dist: jinja2
-Requires-Dist: sqlmodel
-Requires-Dist: rich
-Requires-Dist: python-multipart
-Requires-Dist: typer
-Requires-Dist: typeguard
-Provides-Extra: dev
-Requires-Dist: tox; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-
 # zopyx-fastapi-auth
 
 An opionated authentication and authorization system for FastAPI.
 
 ## Features
 
 - a RDBMS-based user database (support for almost all databases through sqlmodel)
 - a commandline utility for adding, deleting users
 - roles and permissions
 - FastAPI endpoint protection based on permission or roles
 - fully tested, full test coverage, full mypy compliance, parameter checks at runtime
+- a plugin system for arbitrary authentication/authorization (requires one class and one method to implement)
 
 
 ## Status
 
-- experimental
+- in production
+
+## Requirements
+
+- supports Python 3.10-3.12 (no support for Python 3.9 or lower, no support for Python 3.13 yet)
 
 ## Example usage
 
 - see `demo_app.py`
 
 ## Concepts
 
@@ -251,15 +223,62 @@
 
 ![Login into application](/images/login.png)
 
 ### After successfull login
 
 ![Login into application](/images/logged-in.png)
 
-## To do
-- a simple pluggable authentication system for integration of several user sources
 
+## Pluggable authenticators
+
+This module provides a flexible architecture that allows the use of multiple
+authentication and authorization backends within your FastAPI application. For
+instance, you can configure the authentication system to use the default
+Relational Database Management System (RDBMS)-based user management,
+supplemented with an additional plugin for Lightweight Directory Access Protocol
+(LDAP).
+
+### Example
+
+An `Authenticator` is required to implement an `authenticate(request: Request)`
+method. This method should extract the login parameters from a login request and
+return a `Users` object. Authenticators need to be registered with the
+`AUTHENTICATOR_REGISTRY`. The execution order of the Authenticators is
+determined by their `position` parameter. A `position` of `0` indicates that the
+Authenticator is the first to be used. A higher `position` value signifies a
+lower priority.
+
+```
+from fastapi import Request
+from fastapi.authenticator_registry import Authenticator, AUTHENTICATOR_REGISTRY
+from fastapi.users import User 
+
+class MyAuthenticator(Authenticator):
+
+    async def authenticate(request: Request) -> User:
+
+        # extract credentials from request
+        username = request.form....
+        password = request.form....
+
+        # perform authentication against your own authentication system
+        user_data = my_backend.authenticate_user(username, password)
+        
+        return User(name=user_data["name"], roles=[...])
+
+AUTHENTICATOR_REGISTRY.add_authenticator(MyAuthenticator(), 0)
+```
+
+## Provided routes
+
+The `demo_app.py` application demonstrates the integration of `/auth/login` and
+`/auth/logout` routes. You can find the implementation of these routes in
+`auth_routes.py`. This code is customizable, allowing you to adapt it to your
+specific requirements, as it includes some pre-configured decisions related to
+logging and UI integration. The essence of the login process resides in the
+`login_post()` function. Given its simplicity and brevity, you should find it
+straightforward to tailor the login procedure to your needs.
 
 ## Author
 
 Andreas Jung <info@zopyx.com>
```

### Comparing `zopyx_fastapi_auth-0.2.2.6/fastapi_auth/auth_routes.py` & `zopyx_fastapi_auth-0.2.2.7/fastapi_auth/auth_routes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from typing import Optional
 
-from fastapi import Depends, Form, Request, APIRouter
+from fastapi import Depends, Request, APIRouter
 from fastapi.responses import HTMLResponse, RedirectResponse
 from starlette import status
 
 from .dependencies import get_user
 from .logger import LOG
 from .users import User, ANONYMOUS_USER
-from .user_management_sqlobject import get_user_from_fastapi_request, authenticate_user_for_fastapi
+from .user_management_sqlobject import authenticate_user_for_fastapi
 from .jinja2_templates import templates
 
 from starlette.middleware.sessions import SessionMiddleware
 
 from .auth_config import AUTH_SETTINGS
 
+from .authenticator_registry import AUTHENTICATOR_REGISTRY
+
 LIFE_TIME = 3600 * 24
 
 
 router = APIRouter()
 
 
 def install_middleware(app):
@@ -51,28 +53,33 @@
     message = "You have been logged out."
     return RedirectResponse(url=f"/?message={message}")
 
 
 @router.post("/login")
 async def login_post(
     request: Request,
-    username: str = Form(...),
-    password: str = Form(...),
 ):
-    user = await get_user_from_fastapi_request(request)
+    for authenticator in AUTHENTICATOR_REGISTRY.authenticators:
+        LOG.debug(f"Trying to authenticate with {authenticator.name}")
+        try:
+            user = await authenticator.authenticate(request)
+        except Exception as e:
+            LOG.error(f"Error authenticating with {authenticator.name}: {e}")
+            user = None
+        if user:
+            break
 
     if user:
         authenticate_user_for_fastapi(user=user, request=request)
         message = f"Welcome {user.name}. You are now logged in."
         LOG.info(f"User {user.name} logged in")
         return RedirectResponse(f"/?message={message}", status_code=status.HTTP_302_FOUND)
 
     else:
         message = "You could not be logged in. Please try again."
-        LOG.error(message)
         return templates.TemplateResponse(
             request,
             "login.html",
             {
                 "user": ANONYMOUS_USER,
                 "error_message": message,
             },
```

### Comparing `zopyx_fastapi_auth-0.2.2.6/fastapi_auth/demo_app.py` & `zopyx_fastapi_auth-0.2.2.7/fastapi_auth/demo_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 from .auth_routes import router as auth_router, install_middleware
 from .dependencies import get_user
 from .users import User
 from .jinja2_templates import templates
 from .roles import ROLES_REGISTRY, Role
 from .permissions import Permission
 from .dependencies import Protected
+from .authenticator_registry import AUTHENTICATOR_REGISTRY
+from .user_management_sqlobject import DefaultAuthenticator
+
+
+AUTHENTICATOR_REGISTRY.add_authenticator(authenticator=DefaultAuthenticator(), position=0)
 
 # Your FastAPI app
 app = FastAPI()
 # install the session middleware
 install_middleware(app)
 
 # add endpoints for authentication examples
```

### Comparing `zopyx_fastapi_auth-0.2.2.6/fastapi_auth/dependencies.py` & `zopyx_fastapi_auth-0.2.2.7/fastapi_auth/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # from .user import User, get_user, Unauthorized
 
 from .users import User, ANONYMOUS_USER
 from .roles import Role
 from .permissions import Permission
 from .logger import LOG
 
+
 class Unauthorized(Exception):
     """ """
 
 
 def get_user(request: Request) -> User:
     """This dependency return either an authenticated user depending on the
     presented token or an anonymous user if no token is presented."""
@@ -21,15 +22,15 @@
     if "user" not in request.session:
         return ANONYMOUS_USER
     return User(**request.session["user"])
 
 
 class Protected:
     """A dependency to protect routes.  The user must have the required
-    permission or role to access the route.  Using a permission and role(s) are
+    permission or a role to access the route.  Using a permission and role(s) are
     mutually exclusive. You must specify either a permission or a list of roles.
     This dependency should be used for authenticated routes only. only.  The
     authenticated user must either have a specified role or one of its role must
     support the required permission.
     """
 
     @typechecked
@@ -51,15 +52,15 @@
         self.required_roles = required_roles
 
     @typechecked
     def __call__(
         self,
         user: User = Depends(get_user),
     ) -> User:
-        # If the user is anonymous, return the anonymous user
+        # check for roles
         for rr in self.required_roles:
             for user_role in user.roles:
                 if user_role == rr:
                     return user
 
         # If the user has the required permission, return the user
         if self.required_permission:
```

### Comparing `zopyx_fastapi_auth-0.2.2.6/fastapi_auth/roles.py` & `zopyx_fastapi_auth-0.2.2.7/fastapi_auth/roles.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/fastapi_auth/templates/base.html` & `zopyx_fastapi_auth-0.2.2.7/fastapi_auth/templates/base.html`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/fastapi_auth/templates/demo.html` & `zopyx_fastapi_auth-0.2.2.7/fastapi_auth/templates/demo.html`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/fastapi_auth/templates/login.html` & `zopyx_fastapi_auth-0.2.2.7/fastapi_auth/templates/login.html`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/fastapi_auth/user_cmd.py` & `zopyx_fastapi_auth-0.2.2.7/fastapi_auth/user_cmd.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/fastapi_auth/user_management_sqlobject.py` & `zopyx_fastapi_auth-0.2.2.7/fastapi_auth/user_management_sqlobject.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from datetime import datetime, timedelta, timezone
 
 import bcrypt
 from fastapi import Request
 from sqlmodel import Field, Session, SQLModel, create_engine, select
 from typeguard import typechecked
-
+from .authenticator_registry import Authenticator
 from .auth_config import AUTH_SETTINGS
 from .roles import ROLES_REGISTRY
 from .logger import LOG
 
 # AuthUser is an alias in order to avoid name clash with the SQLModel User class below
 from .users import User as AuthUser
 
@@ -24,15 +24,14 @@
 class User(SQLModel, table=True):
     username: str = Field(primary_key=True)
     password: str
     roles: str
     created: datetime = Field(default_factory=utc_now)
 
 
-
 class UserManagement:
     """Class for managing users in a SQL database."""
 
     @typechecked
     def __init__(self, db_uri: str) -> None:
         LOG.info(f"Connecting to database {db_uri}")
         self.engine = create_engine(db_uri)
@@ -128,7 +127,17 @@
     return user
 
 
 @typechecked
 def authenticate_user_for_fastapi(user: AuthUser, request: Request) -> None:
     """Authenticate the user for a FastAPI request by assigning the user to the session."""
     request.session["user"] = user.model_dump(exclude={"created"})
+
+
+class DefaultAuthenticator(Authenticator):
+    """Default authenticator for user management."""
+
+    name = "DefaultAuthenticator"
+
+    @typechecked
+    async def authenticate(self, request: Request) -> AuthUser | None:
+        return await get_user_from_fastapi_request(request)
```

### Comparing `zopyx_fastapi_auth-0.2.2.6/fastapi_auth/users.py` & `zopyx_fastapi_auth-0.2.2.7/fastapi_auth/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,24 @@
 
 
 class User(BaseModel):
     """Users"""
 
     # Name of user
     name: str = Field(..., description="Name of the user")
+
     # Description of user
     description: str = Field(..., description="Description of the user")
+
     # Is user anonymous
     is_anonymous: bool = True
+
     # Roles of user
     roles: list[Role] = []
+
     # Properties of user
     properties: dict = {}
 
     def __str__(self) -> str:
         """Return a string representation of the user."""
         self_str = super().__str__()
         return f"{self.__class__.__name__}({self_str})"
@@ -34,26 +38,26 @@
     @typechecked
     def has_role_by_name(self, role_name: str) -> bool:
         """Check if the user has the required role (by name)."""
         for role in self.roles:
             if role.name == role_name:
                 return True
         return False
-    
+
     def role_names(self) -> list[str]:
         """Return a list of role names."""
         return [role.name for role in self.roles]
-    
+
     def all_permissions(self) -> list[Permission]:
         """Return a list of all permissions."""
         permissions = []
         for role in self.roles:
             permissions.extend(role.permissions)
         return permissions
-                    
+
     def all_permission_names(self) -> list[str]:
         """Return a list of all permission names."""
         permissions = self.all_permissions()
         return [permission.name for permission in permissions]
 
     @typechecked
     def has_permission(self, permission: Permission) -> bool:
```

### Comparing `zopyx_fastapi_auth-0.2.2.6/images/logged-in.png` & `zopyx_fastapi_auth-0.2.2.7/images/logged-in.png`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/images/login.png` & `zopyx_fastapi_auth-0.2.2.7/images/login.png`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/pyproject.toml` & `zopyx_fastapi_auth-0.2.2.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [project]
 name = "zopyx-fastapi-auth"
 description = "FastAPI authentication and authorization"
-version = "0.2.2.6"
+version = "0.2.2.7"
 readme = "README.md"
 authors = [
     { name = "Andreas Jung", email = "info@zopyx.com" }
 ]
 classifiers = [
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "fastapi",
     "pydantic",
```

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.min.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.js` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.js.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.min.js` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map` & `zopyx_fastapi_auth-0.2.2.7/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.2.2.6/zopyx_fastapi_auth.egg-info/SOURCES.txt` & `zopyx_fastapi_auth-0.2.2.7/zopyx_fastapi_auth.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 MANIFEST.in
 README.md
 pyproject.toml
 fastapi_auth/__init__.py
 fastapi_auth/auth_config.py
 fastapi_auth/auth_routes.py
+fastapi_auth/authenticator_registry.py
 fastapi_auth/demo_app.py
 fastapi_auth/dependencies.py
 fastapi_auth/jinja2_templates.py
 fastapi_auth/logger.py
 fastapi_auth/permissions.py
 fastapi_auth/py.typed
 fastapi_auth/roles.py
```

