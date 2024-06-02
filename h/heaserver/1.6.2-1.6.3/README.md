# Comparing `tmp/heaserver-1.6.2.tar.gz` & `tmp/heaserver-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-1.6.2.tar", last modified: Sat Jun  1 05:27:20 2024, max compression
+gzip compressed data, was "heaserver-1.6.3.tar", last modified: Sun Jun  2 16:30:09 2024, max compression
```

## Comparing `heaserver-1.6.2.tar` & `heaserver-1.6.3.tar`

### file list

```diff
@@ -1,356 +1,356 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.931228 heaserver-1.6.2/
--rw-rw-rw-   0        0        0      261 2023-06-07 14:42:11.000000 heaserver-1.6.2/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-06-07 14:43:05.000000 heaserver-1.6.2/.gitignore
--rw-rw-rw-   0        0        0    11625 2023-06-07 14:42:11.000000 heaserver-1.6.2/LICENSE
--rw-rw-rw-   0        0        0      243 2023-06-07 14:43:05.000000 heaserver-1.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9273 2024-06-01 05:27:20.931228 heaserver-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     7274 2024-06-01 04:55:54.000000 heaserver-1.6.2/README.md
--rw-rw-rw-   0        0        0     1612 2023-06-07 14:43:05.000000 heaserver-1.6.2/RELEASING.md
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.598992 heaserver-1.6.2/awss3integrationtests/
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.599521 heaserver-1.6.2/awss3integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.620911 heaserver-1.6.2/awss3integrationtests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-06-07 14:43:05.000000 heaserver-1.6.2/awss3integrationtests/heaserver/awss3tests/__init__.py
--rw-rw-rw-   0        0        0    34976 2024-04-03 19:49:45.000000 heaserver-1.6.2/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
--rw-rw-rw-   0        0        0     1416 2023-06-07 14:43:05.000000 heaserver-1.6.2/awss3integrationtests/heaserver/awss3tests/service.py
--rw-rw-rw-   0        0        0    19401 2024-04-11 00:17:34.000000 heaserver-1.6.2/awss3integrationtests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.622012 heaserver-1.6.2/awss3integrationtests/heaserver/awss3tests/wstl/
--rw-rw-rw-   0        0        0    16955 2023-06-07 14:43:05.000000 heaserver-1.6.2/awss3integrationtests/heaserver/awss3tests/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.600607 heaserver-1.6.2/awss3tests/
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.600607 heaserver-1.6.2/awss3tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.624195 heaserver-1.6.2/awss3tests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-06-07 14:43:05.000000 heaserver-1.6.2/awss3tests/heaserver/awss3tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.632491 heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/
--rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.22664
--rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.2560
--rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.26632
--rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29828
--rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.3260
--rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35416
--rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.37972
--rw-rw-rw-   0        0        0     3169 2023-10-09 18:20:45.000000 heaserver-1.6.2/awss3tests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.602261 heaserver-1.6.2/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.602776 heaserver-1.6.2/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.651481 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-06-07 14:42:11.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.666743 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/
--rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.20088
--rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.31660
--rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.33616
--rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.35072
--rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.39964
--rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.41268
--rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.5640
--rw-rw-rw-   0        0        0     2297 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.44660
--rw-rw-rw-   0        0        0      767 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.26264
--rw-rw-rw-   0        0        0      767 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.31660
--rw-rw-rw-   0        0        0      767 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.39964
--rw-rw-rw-   0        0        0     2115 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-311-pytest-7.4.4.pyc.5352
--rw-rw-rw-   0        0        0     1408 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.41268
--rw-rw-rw-   0        0        0     1408 2024-04-29 16:14:26.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.5352
--rw-rw-rw-   0        0        0     5994 2024-05-22 22:08:38.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
--rw-rw-rw-   0        0        0     6620 2023-11-27 15:30:20.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     6084 2024-05-22 22:08:38.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
--rw-rw-rw-   0        0        0     5709 2024-05-22 22:08:38.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5524 2024-05-22 22:08:38.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
--rw-rw-rw-   0        0        0    12856 2023-10-09 18:20:45.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/service.py
--rw-rw-rw-   0        0        0     1024 2023-10-09 18:20:45.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-06-07 14:43:05.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0      198 2023-06-07 14:43:05.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
--rw-rw-rw-   0        0        0      194 2023-06-07 14:42:11.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
--rw-rw-rw-   0        0        0      888 2023-07-10 19:44:11.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
--rw-rw-rw-   0        0        0      207 2023-06-07 14:43:05.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     4846 2024-05-22 22:08:38.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
--rw-rw-rw-   0        0        0     1011 2023-06-07 14:43:05.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0      521 2023-06-07 14:43:05.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
--rw-rw-rw-   0        0        0      404 2023-06-07 14:43:05.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
--rw-rw-rw-   0        0        0      203 2023-06-07 14:43:05.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.667816 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/wstl/
--rw-rw-rw-   0        0        0    16483 2024-05-22 22:08:38.000000 heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
--rw-rw-rw-   0        0        0      132 2024-03-29 14:06:55.000000 heaserver-1.6.2/pytest.ini
--rw-rw-rw-   0        0        0      237 2024-01-29 16:35:22.000000 heaserver-1.6.2/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 05:27:20.932256 heaserver-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     2874 2024-06-01 05:22:45.000000 heaserver-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.604373 heaserver-1.6.2/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.604373 heaserver-1.6.2/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.701262 heaserver-1.6.2/src/heaserver/service/
--rw-rw-rw-   0        0        0     1176 2023-10-09 18:20:45.000000 heaserver-1.6.2/src/heaserver/service/__init__.py
--rw-rw-rw-   0        0        0     7213 2024-01-29 16:35:22.000000 heaserver-1.6.2/src/heaserver/service/activity.py
--rw-rw-rw-   0        0        0    20215 2024-05-22 22:08:38.000000 heaserver-1.6.2/src/heaserver/service/aiohttp.py
--rw-rw-rw-   0        0        0     1688 2024-04-10 23:57:17.000000 heaserver-1.6.2/src/heaserver/service/appfactory.py
--rw-rw-rw-   0        0        0      758 2023-11-27 15:30:20.000000 heaserver-1.6.2/src/heaserver/service/appproperty.py
--rw-rw-rw-   0        0        0     8674 2024-06-01 04:55:54.000000 heaserver-1.6.2/src/heaserver/service/backgroundtasks.py
--rw-rw-rw-   0        0        0     1527 2024-05-22 22:08:38.000000 heaserver-1.6.2/src/heaserver/service/caching.py
--rw-rw-rw-   0        0        0       64 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/caching_strategy.py
--rw-rw-rw-   0        0        0    24632 2024-05-22 22:08:38.000000 heaserver-1.6.2/src/heaserver/service/client.py
--rw-rw-rw-   0        0        0     2460 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/config.py
--rw-rw-rw-   0        0        0      256 2023-11-06 22:30:27.000000 heaserver-1.6.2/src/heaserver/service/customhdrs.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.709432 heaserver-1.6.2/src/heaserver/service/db/
--rw-rw-rw-   0        0        0      392 2023-06-07 14:42:11.000000 heaserver-1.6.2/src/heaserver/service/db/__init__.py
--rw-rw-rw-   0        0        0    30275 2024-06-01 04:55:54.000000 heaserver-1.6.2/src/heaserver/service/db/aws.py
--rw-rw-rw-   0        0        0    58921 2024-03-29 20:23:19.000000 heaserver-1.6.2/src/heaserver/service/db/awsservicelib.py
--rw-rw-rw-   0        0        0    31373 2024-05-22 22:08:38.000000 heaserver-1.6.2/src/heaserver/service/db/database.py
--rw-rw-rw-   0        0        0     6599 2023-06-07 14:42:11.000000 heaserver-1.6.2/src/heaserver/service/db/dbapi2.py
--rw-rw-rw-   0        0        0    32607 2024-06-01 04:50:20.000000 heaserver-1.6.2/src/heaserver/service/db/mongo.py
--rw-rw-rw-   0        0        0     4515 2024-04-11 00:17:34.000000 heaserver-1.6.2/src/heaserver/service/db/mongoexpr.py
--rw-rw-rw-   0        0        0    28355 2024-05-22 22:08:38.000000 heaserver-1.6.2/src/heaserver/service/db/mongoservicelib.py
--rw-rw-rw-   0        0        0      252 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/defaults.py
--rw-rw-rw-   0        0        0      150 2023-10-09 18:20:45.000000 heaserver-1.6.2/src/heaserver/service/error.py
--rw-rw-rw-   0        0        0     4709 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/expression.py
--rw-rw-rw-   0        0        0      773 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/functional.py
--rw-rw-rw-   0        0        0    17784 2024-05-22 22:08:38.000000 heaserver-1.6.2/src/heaserver/service/heaobjectsupport.py
--rw-rw-rw-   0        0        0      683 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/jsonschema.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.713200 heaserver-1.6.2/src/heaserver/service/jsonschemafiles/
--rw-rw-rw-   0        0        0      606 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/jsonschemafiles/__init__.py
--rw-rw-rw-   0        0        0      787 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/jsonschemafiles/cjtemplate.json
--rw-rw-rw-   0        0        0       87 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/jsonschemafiles/nvpjson.json
--rw-rw-rw-   0        0        0     2214 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/jsonschemafiles/wstl.json
--rw-rw-rw-   0        0        0     4970 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/jsonschemafiles/wstlaction.json
--rw-rw-rw-   0        0        0      987 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/jsonschemavalidator.py
--rw-rw-rw-   0        0        0    21655 2023-10-24 14:35:41.000000 heaserver-1.6.2/src/heaserver/service/messagebroker.py
--rw-rw-rw-   0        0        0      539 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/mimetypes.py
--rw-rw-rw-   0        0        0      639 2023-06-07 14:42:11.000000 heaserver-1.6.2/src/heaserver/service/oidcclaimhdrs.py
--rw-rw-rw-   0        0        0     1558 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/openapi.py
--rw-rw-rw-   0        0        0        0 2023-06-07 14:42:11.000000 heaserver-1.6.2/src/heaserver/service/py.typed
--rw-rw-rw-   0        0        0      103 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/registryproperty.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.721340 heaserver-1.6.2/src/heaserver/service/representor/
--rw-rw-rw-   0        0        0     1426 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/representor/__init__.py
--rw-rw-rw-   0        0        0    26065 2024-04-29 19:37:46.000000 heaserver-1.6.2/src/heaserver/service/representor/cj.py
--rw-rw-rw-   0        0        0      170 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/representor/error.py
--rw-rw-rw-   0        0        0     7259 2023-11-27 15:30:20.000000 heaserver-1.6.2/src/heaserver/service/representor/factory.py
--rw-rw-rw-   0        0        0     2231 2023-11-27 15:30:20.000000 heaserver-1.6.2/src/heaserver/service/representor/nvpjson.py
--rw-rw-rw-   0        0        0     3244 2023-11-27 15:30:20.000000 heaserver-1.6.2/src/heaserver/service/representor/representor.py
--rw-rw-rw-   0        0        0     1551 2023-11-27 15:30:20.000000 heaserver-1.6.2/src/heaserver/service/representor/wstljson.py
--rw-rw-rw-   0        0        0     1742 2023-11-27 15:30:20.000000 heaserver-1.6.2/src/heaserver/service/representor/xwwwformurlencoded.py
--rw-rw-rw-   0        0        0      114 2023-06-07 14:42:11.000000 heaserver-1.6.2/src/heaserver/service/requestproperty.py
--rw-rw-rw-   0        0        0    29114 2024-04-03 19:49:45.000000 heaserver-1.6.2/src/heaserver/service/response.py
--rw-rw-rw-   0        0        0    16289 2024-06-01 04:55:54.000000 heaserver-1.6.2/src/heaserver/service/runner.py
--rw-rw-rw-   0        0        0       32 2024-03-29 20:23:19.000000 heaserver-1.6.2/src/heaserver/service/sources.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.738500 heaserver-1.6.2/src/heaserver/service/testcase/
--rw-rw-rw-   0        0        0      167 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/testcase/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/testcase/aiohttptestcase.py
--rw-rw-rw-   0        0        0     1508 2023-10-09 18:20:45.000000 heaserver-1.6.2/src/heaserver/service/testcase/awsdockermongo.py
--rw-rw-rw-   0        0        0     3944 2023-10-09 18:20:45.000000 heaserver-1.6.2/src/heaserver/service/testcase/awss3microservicetestcase.py
--rw-rw-rw-   0        0        0    15471 2023-07-25 21:24:15.000000 heaserver-1.6.2/src/heaserver/service/testcase/collection.py
--rw-rw-rw-   0        0        0     6655 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/testcase/docker.py
--rw-rw-rw-   0        0        0     8062 2023-11-27 15:30:20.000000 heaserver-1.6.2/src/heaserver/service/testcase/dockermongo.py
--rw-rw-rw-   0        0        0    41015 2024-05-22 22:08:38.000000 heaserver-1.6.2/src/heaserver/service/testcase/expectedvalues.py
--rw-rw-rw-   0        0        0    17534 2024-04-03 19:49:45.000000 heaserver-1.6.2/src/heaserver/service/testcase/microservicetestcase.py
--rw-rw-rw-   0        0        0   130477 2024-04-03 19:49:45.000000 heaserver-1.6.2/src/heaserver/service/testcase/mixin.py
--rw-rw-rw-   0        0        0    17917 2024-06-01 04:55:54.000000 heaserver-1.6.2/src/heaserver/service/testcase/mockaws.py
--rw-rw-rw-   0        0        0      662 2023-11-10 18:12:16.000000 heaserver-1.6.2/src/heaserver/service/testcase/mockdatabase.py
--rw-rw-rw-   0        0        0    21242 2023-11-27 15:30:20.000000 heaserver-1.6.2/src/heaserver/service/testcase/mockmongo.py
--rw-rw-rw-   0        0        0      555 2023-11-27 15:30:20.000000 heaserver-1.6.2/src/heaserver/service/testcase/simpleaiohttptestcase.py
--rw-rw-rw-   0        0        0     7531 2023-10-09 18:20:45.000000 heaserver-1.6.2/src/heaserver/service/testcase/swaggerui.py
--rw-rw-rw-   0        0        0    29140 2023-07-25 21:24:15.000000 heaserver-1.6.2/src/heaserver/service/testcase/testenv.py
--rw-rw-rw-   0        0        0     2132 2023-10-09 18:20:45.000000 heaserver-1.6.2/src/heaserver/service/testcase/util.py
--rw-rw-rw-   0        0        0     2877 2023-06-07 14:43:05.000000 heaserver-1.6.2/src/heaserver/service/uritemplate.py
--rw-rw-rw-   0        0        0    11832 2024-05-22 22:08:38.000000 heaserver-1.6.2/src/heaserver/service/util.py
--rw-rw-rw-   0        0        0    36804 2024-04-03 19:49:45.000000 heaserver-1.6.2/src/heaserver/service/wstl.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.930192 heaserver-1.6.2/src/heaserver.egg-info/
--rw-rw-rw-   0        0        0     9273 2024-06-01 05:27:20.000000 heaserver-1.6.2/src/heaserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    22899 2024-06-01 05:27:20.000000 heaserver-1.6.2/src/heaserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 05:27:20.000000 heaserver-1.6.2/src/heaserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      459 2024-06-01 05:27:20.000000 heaserver-1.6.2/src/heaserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-06-01 05:27:20.000000 heaserver-1.6.2/src/heaserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.606013 heaserver-1.6.2/tests/
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.606563 heaserver-1.6.2/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.778744 heaserver-1.6.2/tests/heaserver/servicetest/
--rw-rw-rw-   0        0        0        0 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.853377 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/
--rw-rw-rw-   0        0        0    11053 2024-03-28 23:13:33.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.25384
--rw-rw-rw-   0        0        0    14721 2024-05-30 17:03:07.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.13192
--rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.13688
--rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.20088
--rw-rw-rw-   0        0        0    15099 2024-03-28 23:13:33.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.22664
--rw-rw-rw-   0        0        0    14721 2024-04-30 14:25:46.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.23744
--rw-rw-rw-   0        0        0    15099 2024-03-28 23:13:33.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.25384
--rw-rw-rw-   0        0        0    14721 2024-05-21 18:56:21.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.28100
--rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.39288
--rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.39964
--rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.41428
--rw-rw-rw-   0        0        0    14721 2024-04-30 14:25:46.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.42872
--rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.44660
--rw-rw-rw-   0        0        0    14721 2024-05-21 18:56:21.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.5212
--rw-rw-rw-   0        0        0    14721 2024-04-30 14:25:46.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.6356
--rw-rw-rw-   0        0        0     5148 2024-03-28 23:13:33.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.26632
--rw-rw-rw-   0        0        0    13723 2024-04-22 16:36:50.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.41148
--rw-rw-rw-   0        0        0    13723 2024-04-22 16:36:50.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.5676
--rw-rw-rw-   0        0        0     1709 2023-10-09 18:55:18.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.2.pyc.40340
--rw-rw-rw-   0        0        0     2275 2024-03-28 23:13:33.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.22664
--rw-rw-rw-   0        0        0     2275 2024-03-28 23:13:33.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.26632
--rw-rw-rw-   0        0        0     2275 2024-03-28 23:13:33.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35416
--rw-rw-rw-   0        0        0     1372 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_functional.cpython-311-pytest-7.4.4.pyc.22664
--rw-rw-rw-   0        0        0     1205 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_get_all_components.cpython-311-pytest-7.4.4.pyc.23384
--rw-rw-rw-   0        0        0    13993 2024-04-22 16:36:51.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_heaobjectsupport.cpython-311-pytest-7.4.4.pyc.34244
--rw-rw-rw-   0        0        0     6047 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_jsonschemavalidator.cpython-310-pytest-7.4.2.pyc.40340
--rw-rw-rw-   0        0        0     2560 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_mimetypes.cpython-311-pytest-7.4.4.pyc.22664
--rw-rw-rw-   0        0        0      956 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_not_imported.cpython-310-pytest-7.4.2.pyc.18372
--rw-rw-rw-   0        0        0      956 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_not_imported.cpython-310-pytest-7.4.2.pyc.32764
--rw-rw-rw-   0        0        0     1486 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.2.pyc.6392
--rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.26632
--rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29828
--rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.31020
--rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.3260
--rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33324
--rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.36432
--rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.37972
--rw-rw-rw-   0        0        0     2018 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.18372
--rw-rw-rw-   0        0        0     2018 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.40340
--rw-rw-rw-   0        0        0     2018 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.7612
--rw-rw-rw-   0        0        0     1999 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-310-pytest-7.4.2.pyc.6392
--rw-rw-rw-   0        0        0     2595 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.3260
--rw-rw-rw-   0        0        0     2595 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.37972
--rw-rw-rw-   0        0        0      673 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.2.pyc.4048
--rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.25384
--rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.2560
--rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.31020
--rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.3260
--rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35416
--rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.37972
--rw-rw-rw-   0        0        0    21683 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.23384
--rw-rw-rw-   0        0        0    21683 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.31020
--rw-rw-rw-   0        0        0    21683 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3260
--rw-rw-rw-   0        0        0     1879 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.22664
--rw-rw-rw-   0        0        0     1879 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.26660
--rw-rw-rw-   0        0        0     1879 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35416
--rw-rw-rw-   0        0        0     1879 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.37972
--rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.23384
--rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.25384
--rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.2560
--rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.26632
--rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.26660
--rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.31020
--rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33324
--rw-rw-rw-   0        0        0    10601 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-310-pytest-7.4.2.pyc.11904
--rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.23384
--rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.25384
--rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.2560
--rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.26632
--rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.26660
--rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.3260
--rw-rw-rw-   0        0        0     6885 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-310-pytest-7.4.2.pyc.2600
--rw-rw-rw-   0        0        0    12010 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.2560
--rw-rw-rw-   0        0        0    12010 2024-03-28 23:13:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3260
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.854445 heaserver-1.6.2/tests/heaserver/servicetest/aiohttpdata/
--rw-rw-rw-   0        0        0      258 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
--rw-rw-rw-   0        0        0     6442 2023-11-27 15:30:20.000000 heaserver-1.6.2/tests/heaserver/servicetest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0    17429 2024-05-22 22:08:38.000000 heaserver-1.6.2/tests/heaserver/servicetest/componenttestcase.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.856600 heaserver-1.6.2/tests/heaserver/servicetest/db/
--rw-rw-rw-   0        0        0        0 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.867140 heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/
--rw-rw-rw-   0        0        0     1030 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-310-pytest-7.4.2.pyc.4048
--rw-rw-rw-   0        0        0     1030 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-310-pytest-7.4.2.pyc.6392
--rw-rw-rw-   0        0        0     1353 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.25384
--rw-rw-rw-   0        0        0     1353 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.26632
--rw-rw-rw-   0        0        0     1353 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.3260
--rw-rw-rw-   0        0        0     1353 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.35416
--rw-rw-rw-   0        0        0     5790 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-310-pytest-7.4.2.pyc.2600
--rw-rw-rw-   0        0        0     7933 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.22664
--rw-rw-rw-   0        0        0     7933 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.2560
--rw-rw-rw-   0        0        0     7933 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.36432
--rw-rw-rw-   0        0        0      551 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/test_mongo.py
--rw-rw-rw-   0        0        0     7303 2023-11-10 18:12:16.000000 heaserver-1.6.2/tests/heaserver/servicetest/db/test_mongoexpr.py
--rw-rw-rw-   0        0        0     5563 2024-05-22 22:08:38.000000 heaserver-1.6.2/tests/heaserver/servicetest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5931 2024-05-22 22:08:38.000000 heaserver-1.6.2/tests/heaserver/servicetest/organizationtestcase.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.881758 heaserver-1.6.2/tests/heaserver/servicetest/representor/
--rw-rw-rw-   0        0        0        0 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.928119 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/
--rw-rw-rw-   0        0        0    46148 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-310-pytest-7.4.2.pyc.11904
--rw-rw-rw-   0        0        0    62676 2024-04-03 20:15:45.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.17544
--rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.22664
--rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.23384
--rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.2560
--rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.26660
--rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.31020
--rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3260
--rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35416
--rw-rw-rw-   0        0        0     3716 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.11904
--rw-rw-rw-   0        0        0     3716 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.18372
--rw-rw-rw-   0        0        0     3716 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.40340
--rw-rw-rw-   0        0        0     6478 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.29828
--rw-rw-rw-   0        0        0     4816 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-310-pytest-7.4.2.pyc.40340
--rw-rw-rw-   0        0        0     4816 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-310-pytest-7.4.2.pyc.4048
--rw-rw-rw-   0        0        0     7295 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.2560
--rw-rw-rw-   0        0        0     7295 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.26660
--rw-rw-rw-   0        0        0     7295 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.31020
--rw-rw-rw-   0        0        0     7295 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.3260
--rw-rw-rw-   0        0        0      895 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-310-pytest-7.4.2.pyc.4048
--rw-rw-rw-   0        0        0     1336 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.22664
--rw-rw-rw-   0        0        0     1336 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.2560
--rw-rw-rw-   0        0        0     1336 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.26632
--rw-rw-rw-   0        0        0     1336 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.31020
--rw-rw-rw-   0        0        0     4182 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.2600
--rw-rw-rw-   0        0        0     4182 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.32764
--rw-rw-rw-   0        0        0     4182 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.4048
--rw-rw-rw-   0        0        0     4182 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.6392
--rw-rw-rw-   0        0        0     7770 2024-04-03 20:15:45.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.18204
--rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.23384
--rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.25384
--rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.26632
--rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3260
--rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35416
--rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37972
--rw-rw-rw-   0        0        0     7770 2024-04-03 20:15:45.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.42188
--rw-rw-rw-   0        0        0     3079 2023-10-09 18:55:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-310-pytest-7.4.2.pyc.18372
--rw-rw-rw-   0        0        0     4480 2024-04-03 20:15:45.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.17544
--rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23384
--rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.26632
--rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.26660
--rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29828
--rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33324
--rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.36432
--rw-rw-rw-   0        0        0      192 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/all.json
--rw-rw-rw-   0        0        0      268 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/all_cj_item_href.json
--rw-rw-rw-   0        0        0      268 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/all_cj_item_link.json
--rw-rw-rw-   0        0        0      642 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/all_cj_queries.json
--rw-rw-rw-   0        0        0     2670 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/all_cj_template.json
--rw-rw-rw-   0        0        0      267 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
--rw-rw-rw-   0        0        0      263 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
--rw-rw-rw-   0        0        0    62769 2024-04-03 19:49:45.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/test_cj.py
--rw-rw-rw-   0        0        0     2671 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/test_factory.py
--rw-rw-rw-   0        0        0     4181 2023-11-27 15:30:20.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/test_nvpjson.py
--rw-rw-rw-   0        0        0      281 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/test_supports_links.py
--rw-rw-rw-   0        0        0     5676 2024-04-03 19:49:45.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/test_wstljson.py
--rw-rw-rw-   0        0        0     2396 2024-03-29 20:23:19.000000 heaserver-1.6.2/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
--rw-rw-rw-   0        0        0    13067 2023-10-09 18:20:45.000000 heaserver-1.6.2/tests/heaserver/servicetest/service.py
--rw-rw-rw-   0        0        0     9455 2024-01-29 16:35:22.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_activity.py
--rw-rw-rw-   0        0        0     3976 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_aiohttp.py
--rw-rw-rw-   0        0        0     5968 2024-06-01 04:55:54.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_backgroundtasks.py
--rw-rw-rw-   0        0        0     2506 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_caching.py
--rw-rw-rw-   0        0        0     7131 2024-04-11 00:17:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1127 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_configuration.py
--rw-rw-rw-   0        0        0      819 2023-11-06 22:30:27.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_database_classes.py
--rw-rw-rw-   0        0        0      204 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_delete_component.py
--rw-rw-rw-   0        0        0     6181 2023-07-10 19:44:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_expression.py
--rw-rw-rw-   0        0        0      405 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_functional.py
--rw-rw-rw-   0        0        0      422 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_get_all_components.py
--rw-rw-rw-   0        0        0     3070 2023-07-10 19:44:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_get_component.py
--rw-rw-rw-   0        0        0      209 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     5366 2024-04-11 00:17:34.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_heaobjectsupport.py
--rw-rw-rw-   0        0        0     5746 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_jsonschemavalidator.py
--rw-rw-rw-   0        0        0      909 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_mimetypes.py
--rw-rw-rw-   0        0        0      331 2023-07-25 21:24:15.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_not_imported.py
--rw-rw-rw-   0        0        0     1005 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1274 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_post_component.py
--rw-rw-rw-   0        0        0     1265 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_put_component.py
--rw-rw-rw-   0        0        0      253 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_put_organization_permissions.py
--rw-rw-rw-   0        0        0     2488 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_response.py
--rw-rw-rw-   0        0        0      570 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_testenv.py
--rw-rw-rw-   0        0        0     1929 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_uritemplate.py
--rw-rw-rw-   0        0        0     8782 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_util.py
--rw-rw-rw-   0        0        0     6255 2023-06-07 14:43:05.000000 heaserver-1.6.2/tests/heaserver/servicetest/test_wstl.py
-drwxrwxrwx   0        0        0        0 2024-06-01 05:27:20.929150 heaserver-1.6.2/tests/heaserver/servicetest/wstl/
--rw-rw-rw-   0        0        0    16436 2023-10-09 18:20:45.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl/all.json
--rw-rw-rw-   0        0        0     1185 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_1.json
--rw-rw-rw-   0        0        0     1214 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_10a.json
--rw-rw-rw-   0        0        0     1240 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_10b.json
--rw-rw-rw-   0        0        0     2355 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_11.json
--rw-rw-rw-   0        0        0     1187 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_2.json
--rw-rw-rw-   0        0        0     1190 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_3.json
--rw-rw-rw-   0        0        0     1158 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_4.json
--rw-rw-rw-   0        0        0      269 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_5.json
--rw-rw-rw-   0        0        0      531 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_6.json
--rw-rw-rw-   0        0        0     1185 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_7.json
--rw-rw-rw-   0        0        0     1185 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_8.json
--rw-rw-rw-   0        0        0      204 2023-06-07 14:42:11.000000 heaserver-1.6.2/tests/heaserver/servicetest/wstl_9.json
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.414604 heaserver-1.6.3/
+-rw-rw-rw-   0        0        0      261 2023-06-07 14:42:11.000000 heaserver-1.6.3/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-06-07 14:43:05.000000 heaserver-1.6.3/.gitignore
+-rw-rw-rw-   0        0        0    11625 2023-06-07 14:42:11.000000 heaserver-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0      243 2023-06-07 14:43:05.000000 heaserver-1.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     9348 2024-06-02 16:30:09.413604 heaserver-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7349 2024-06-02 16:21:14.000000 heaserver-1.6.3/README.md
+-rw-rw-rw-   0        0        0     1612 2023-06-07 14:43:05.000000 heaserver-1.6.3/RELEASING.md
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.088142 heaserver-1.6.3/awss3integrationtests/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.088142 heaserver-1.6.3/awss3integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.117728 heaserver-1.6.3/awss3integrationtests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-06-07 14:43:05.000000 heaserver-1.6.3/awss3integrationtests/heaserver/awss3tests/__init__.py
+-rw-rw-rw-   0        0        0    34976 2024-04-03 19:49:45.000000 heaserver-1.6.3/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
+-rw-rw-rw-   0        0        0     1416 2023-06-07 14:43:05.000000 heaserver-1.6.3/awss3integrationtests/heaserver/awss3tests/service.py
+-rw-rw-rw-   0        0        0    19401 2024-04-11 00:17:34.000000 heaserver-1.6.3/awss3integrationtests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.118727 heaserver-1.6.3/awss3integrationtests/heaserver/awss3tests/wstl/
+-rw-rw-rw-   0        0        0    16955 2023-06-07 14:43:05.000000 heaserver-1.6.3/awss3integrationtests/heaserver/awss3tests/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.090143 heaserver-1.6.3/awss3tests/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.090143 heaserver-1.6.3/awss3tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.120726 heaserver-1.6.3/awss3tests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-06-07 14:43:05.000000 heaserver-1.6.3/awss3tests/heaserver/awss3tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.125769 heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/
+-rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.22664
+-rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.2560
+-rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.26632
+-rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29828
+-rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.3260
+-rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35416
+-rw-rw-rw-   0        0        0     5881 2024-03-28 23:13:35.000000 heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.37972
+-rw-rw-rw-   0        0        0     3169 2023-10-09 18:20:45.000000 heaserver-1.6.3/awss3tests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.092146 heaserver-1.6.3/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.092146 heaserver-1.6.3/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.143541 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-06-07 14:42:11.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.160000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/
+-rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.20088
+-rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.31660
+-rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.33616
+-rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.35072
+-rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.39964
+-rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.41268
+-rw-rw-rw-   0        0        0     3254 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.5640
+-rw-rw-rw-   0        0        0     2297 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.44660
+-rw-rw-rw-   0        0        0      767 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.26264
+-rw-rw-rw-   0        0        0      767 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.31660
+-rw-rw-rw-   0        0        0      767 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.39964
+-rw-rw-rw-   0        0        0     2115 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-311-pytest-7.4.4.pyc.5352
+-rw-rw-rw-   0        0        0     1408 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.41268
+-rw-rw-rw-   0        0        0     1408 2024-04-29 16:14:26.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.5352
+-rw-rw-rw-   0        0        0     5994 2024-05-22 22:08:38.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
+-rw-rw-rw-   0        0        0     6620 2023-11-27 15:30:20.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     6084 2024-05-22 22:08:38.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
+-rw-rw-rw-   0        0        0     5709 2024-05-22 22:08:38.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5524 2024-05-22 22:08:38.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
+-rw-rw-rw-   0        0        0    12856 2023-10-09 18:20:45.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/service.py
+-rw-rw-rw-   0        0        0     1024 2023-10-09 18:20:45.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-06-07 14:43:05.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      198 2023-06-07 14:43:05.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
+-rw-rw-rw-   0        0        0      194 2023-06-07 14:42:11.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
+-rw-rw-rw-   0        0        0      888 2023-07-10 19:44:11.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
+-rw-rw-rw-   0        0        0      207 2023-06-07 14:43:05.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     4846 2024-05-22 22:08:38.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
+-rw-rw-rw-   0        0        0     1011 2023-06-07 14:43:05.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      521 2023-06-07 14:43:05.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
+-rw-rw-rw-   0        0        0      404 2023-06-07 14:43:05.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
+-rw-rw-rw-   0        0        0      203 2023-06-07 14:43:05.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.160983 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/wstl/
+-rw-rw-rw-   0        0        0    16483 2024-05-22 22:08:38.000000 heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
+-rw-rw-rw-   0        0        0      132 2024-03-29 14:06:55.000000 heaserver-1.6.3/pytest.ini
+-rw-rw-rw-   0        0        0      237 2024-01-29 16:35:22.000000 heaserver-1.6.3/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 16:30:09.414604 heaserver-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     2874 2024-06-02 16:21:14.000000 heaserver-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.094144 heaserver-1.6.3/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.094144 heaserver-1.6.3/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.192145 heaserver-1.6.3/src/heaserver/service/
+-rw-rw-rw-   0        0        0     1176 2023-10-09 18:20:45.000000 heaserver-1.6.3/src/heaserver/service/__init__.py
+-rw-rw-rw-   0        0        0     7213 2024-01-29 16:35:22.000000 heaserver-1.6.3/src/heaserver/service/activity.py
+-rw-rw-rw-   0        0        0    20215 2024-05-22 22:08:38.000000 heaserver-1.6.3/src/heaserver/service/aiohttp.py
+-rw-rw-rw-   0        0        0     1688 2024-04-10 23:57:17.000000 heaserver-1.6.3/src/heaserver/service/appfactory.py
+-rw-rw-rw-   0        0        0      758 2023-11-27 15:30:20.000000 heaserver-1.6.3/src/heaserver/service/appproperty.py
+-rw-rw-rw-   0        0        0     8674 2024-06-01 04:55:54.000000 heaserver-1.6.3/src/heaserver/service/backgroundtasks.py
+-rw-rw-rw-   0        0        0     1527 2024-05-22 22:08:38.000000 heaserver-1.6.3/src/heaserver/service/caching.py
+-rw-rw-rw-   0        0        0       64 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/caching_strategy.py
+-rw-rw-rw-   0        0        0    24632 2024-05-22 22:08:38.000000 heaserver-1.6.3/src/heaserver/service/client.py
+-rw-rw-rw-   0        0        0     2460 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/config.py
+-rw-rw-rw-   0        0        0      256 2023-11-06 22:30:27.000000 heaserver-1.6.3/src/heaserver/service/customhdrs.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.199131 heaserver-1.6.3/src/heaserver/service/db/
+-rw-rw-rw-   0        0        0      392 2023-06-07 14:42:11.000000 heaserver-1.6.3/src/heaserver/service/db/__init__.py
+-rw-rw-rw-   0        0        0    30275 2024-06-01 04:55:54.000000 heaserver-1.6.3/src/heaserver/service/db/aws.py
+-rw-rw-rw-   0        0        0    58921 2024-03-29 20:23:19.000000 heaserver-1.6.3/src/heaserver/service/db/awsservicelib.py
+-rw-rw-rw-   0        0        0    31373 2024-05-22 22:08:38.000000 heaserver-1.6.3/src/heaserver/service/db/database.py
+-rw-rw-rw-   0        0        0     6599 2023-06-07 14:42:11.000000 heaserver-1.6.3/src/heaserver/service/db/dbapi2.py
+-rw-rw-rw-   0        0        0    32607 2024-06-01 04:50:20.000000 heaserver-1.6.3/src/heaserver/service/db/mongo.py
+-rw-rw-rw-   0        0        0     4515 2024-04-11 00:17:34.000000 heaserver-1.6.3/src/heaserver/service/db/mongoexpr.py
+-rw-rw-rw-   0        0        0    28355 2024-05-22 22:08:38.000000 heaserver-1.6.3/src/heaserver/service/db/mongoservicelib.py
+-rw-rw-rw-   0        0        0      252 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/defaults.py
+-rw-rw-rw-   0        0        0      150 2023-10-09 18:20:45.000000 heaserver-1.6.3/src/heaserver/service/error.py
+-rw-rw-rw-   0        0        0     4709 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/expression.py
+-rw-rw-rw-   0        0        0      773 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/functional.py
+-rw-rw-rw-   0        0        0    17784 2024-05-22 22:08:38.000000 heaserver-1.6.3/src/heaserver/service/heaobjectsupport.py
+-rw-rw-rw-   0        0        0      683 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/jsonschema.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.202147 heaserver-1.6.3/src/heaserver/service/jsonschemafiles/
+-rw-rw-rw-   0        0        0      606 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/jsonschemafiles/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/jsonschemafiles/cjtemplate.json
+-rw-rw-rw-   0        0        0       87 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/jsonschemafiles/nvpjson.json
+-rw-rw-rw-   0        0        0     2214 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/jsonschemafiles/wstl.json
+-rw-rw-rw-   0        0        0     4970 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/jsonschemafiles/wstlaction.json
+-rw-rw-rw-   0        0        0      987 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/jsonschemavalidator.py
+-rw-rw-rw-   0        0        0    21655 2023-10-24 14:35:41.000000 heaserver-1.6.3/src/heaserver/service/messagebroker.py
+-rw-rw-rw-   0        0        0      539 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/mimetypes.py
+-rw-rw-rw-   0        0        0      639 2023-06-07 14:42:11.000000 heaserver-1.6.3/src/heaserver/service/oidcclaimhdrs.py
+-rw-rw-rw-   0        0        0     1558 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/openapi.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 14:42:11.000000 heaserver-1.6.3/src/heaserver/service/py.typed
+-rw-rw-rw-   0        0        0      103 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/registryproperty.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.207252 heaserver-1.6.3/src/heaserver/service/representor/
+-rw-rw-rw-   0        0        0     1426 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/representor/__init__.py
+-rw-rw-rw-   0        0        0    26065 2024-04-29 19:37:46.000000 heaserver-1.6.3/src/heaserver/service/representor/cj.py
+-rw-rw-rw-   0        0        0      170 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/representor/error.py
+-rw-rw-rw-   0        0        0     7259 2023-11-27 15:30:20.000000 heaserver-1.6.3/src/heaserver/service/representor/factory.py
+-rw-rw-rw-   0        0        0     2231 2023-11-27 15:30:20.000000 heaserver-1.6.3/src/heaserver/service/representor/nvpjson.py
+-rw-rw-rw-   0        0        0     3244 2023-11-27 15:30:20.000000 heaserver-1.6.3/src/heaserver/service/representor/representor.py
+-rw-rw-rw-   0        0        0     1551 2023-11-27 15:30:20.000000 heaserver-1.6.3/src/heaserver/service/representor/wstljson.py
+-rw-rw-rw-   0        0        0     1742 2023-11-27 15:30:20.000000 heaserver-1.6.3/src/heaserver/service/representor/xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0      114 2023-06-07 14:42:11.000000 heaserver-1.6.3/src/heaserver/service/requestproperty.py
+-rw-rw-rw-   0        0        0    29114 2024-04-03 19:49:45.000000 heaserver-1.6.3/src/heaserver/service/response.py
+-rw-rw-rw-   0        0        0    16289 2024-06-01 04:55:54.000000 heaserver-1.6.3/src/heaserver/service/runner.py
+-rw-rw-rw-   0        0        0       32 2024-03-29 20:23:19.000000 heaserver-1.6.3/src/heaserver/service/sources.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.221253 heaserver-1.6.3/src/heaserver/service/testcase/
+-rw-rw-rw-   0        0        0      167 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/testcase/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/testcase/aiohttptestcase.py
+-rw-rw-rw-   0        0        0     1508 2023-10-09 18:20:45.000000 heaserver-1.6.3/src/heaserver/service/testcase/awsdockermongo.py
+-rw-rw-rw-   0        0        0     3944 2023-10-09 18:20:45.000000 heaserver-1.6.3/src/heaserver/service/testcase/awss3microservicetestcase.py
+-rw-rw-rw-   0        0        0    15471 2023-07-25 21:24:15.000000 heaserver-1.6.3/src/heaserver/service/testcase/collection.py
+-rw-rw-rw-   0        0        0     6655 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/testcase/docker.py
+-rw-rw-rw-   0        0        0     8062 2023-11-27 15:30:20.000000 heaserver-1.6.3/src/heaserver/service/testcase/dockermongo.py
+-rw-rw-rw-   0        0        0    41015 2024-05-22 22:08:38.000000 heaserver-1.6.3/src/heaserver/service/testcase/expectedvalues.py
+-rw-rw-rw-   0        0        0    17534 2024-04-03 19:49:45.000000 heaserver-1.6.3/src/heaserver/service/testcase/microservicetestcase.py
+-rw-rw-rw-   0        0        0   130477 2024-04-03 19:49:45.000000 heaserver-1.6.3/src/heaserver/service/testcase/mixin.py
+-rw-rw-rw-   0        0        0    17917 2024-06-01 04:55:54.000000 heaserver-1.6.3/src/heaserver/service/testcase/mockaws.py
+-rw-rw-rw-   0        0        0      662 2023-11-10 18:12:16.000000 heaserver-1.6.3/src/heaserver/service/testcase/mockdatabase.py
+-rw-rw-rw-   0        0        0    21242 2023-11-27 15:30:20.000000 heaserver-1.6.3/src/heaserver/service/testcase/mockmongo.py
+-rw-rw-rw-   0        0        0      555 2023-11-27 15:30:20.000000 heaserver-1.6.3/src/heaserver/service/testcase/simpleaiohttptestcase.py
+-rw-rw-rw-   0        0        0     7531 2023-10-09 18:20:45.000000 heaserver-1.6.3/src/heaserver/service/testcase/swaggerui.py
+-rw-rw-rw-   0        0        0    29140 2023-07-25 21:24:15.000000 heaserver-1.6.3/src/heaserver/service/testcase/testenv.py
+-rw-rw-rw-   0        0        0     2132 2023-10-09 18:20:45.000000 heaserver-1.6.3/src/heaserver/service/testcase/util.py
+-rw-rw-rw-   0        0        0     2877 2023-06-07 14:43:05.000000 heaserver-1.6.3/src/heaserver/service/uritemplate.py
+-rw-rw-rw-   0        0        0    11832 2024-05-22 22:08:38.000000 heaserver-1.6.3/src/heaserver/service/util.py
+-rw-rw-rw-   0        0        0    36804 2024-04-03 19:49:45.000000 heaserver-1.6.3/src/heaserver/service/wstl.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.413604 heaserver-1.6.3/src/heaserver.egg-info/
+-rw-rw-rw-   0        0        0     9348 2024-06-02 16:30:09.000000 heaserver-1.6.3/src/heaserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    22899 2024-06-02 16:30:09.000000 heaserver-1.6.3/src/heaserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 16:30:09.000000 heaserver-1.6.3/src/heaserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      459 2024-06-02 16:30:09.000000 heaserver-1.6.3/src/heaserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 16:30:09.000000 heaserver-1.6.3/src/heaserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.095729 heaserver-1.6.3/tests/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.095729 heaserver-1.6.3/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.269566 heaserver-1.6.3/tests/heaserver/servicetest/
+-rw-rw-rw-   0        0        0        0 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.338849 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/
+-rw-rw-rw-   0        0        0    11053 2024-03-28 23:13:33.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.25384
+-rw-rw-rw-   0        0        0    14721 2024-05-30 17:03:07.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.13192
+-rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.13688
+-rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.20088
+-rw-rw-rw-   0        0        0    15099 2024-03-28 23:13:33.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.22664
+-rw-rw-rw-   0        0        0    14721 2024-04-30 14:25:46.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.23744
+-rw-rw-rw-   0        0        0    15099 2024-03-28 23:13:33.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.25384
+-rw-rw-rw-   0        0        0    14721 2024-05-21 18:56:21.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.28100
+-rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.39288
+-rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.39964
+-rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.41428
+-rw-rw-rw-   0        0        0    14721 2024-04-30 14:25:46.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.42872
+-rw-rw-rw-   0        0        0    14721 2024-04-29 16:14:26.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.44660
+-rw-rw-rw-   0        0        0    14721 2024-05-21 18:56:21.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.5212
+-rw-rw-rw-   0        0        0    14721 2024-04-30 14:25:46.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.6356
+-rw-rw-rw-   0        0        0     5148 2024-03-28 23:13:33.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.26632
+-rw-rw-rw-   0        0        0    13723 2024-04-22 16:36:50.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.41148
+-rw-rw-rw-   0        0        0    13723 2024-04-22 16:36:50.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.5676
+-rw-rw-rw-   0        0        0     1709 2023-10-09 18:55:18.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.2.pyc.40340
+-rw-rw-rw-   0        0        0     2275 2024-03-28 23:13:33.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.22664
+-rw-rw-rw-   0        0        0     2275 2024-03-28 23:13:33.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.26632
+-rw-rw-rw-   0        0        0     2275 2024-03-28 23:13:33.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35416
+-rw-rw-rw-   0        0        0     1372 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_functional.cpython-311-pytest-7.4.4.pyc.22664
+-rw-rw-rw-   0        0        0     1205 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_get_all_components.cpython-311-pytest-7.4.4.pyc.23384
+-rw-rw-rw-   0        0        0    13993 2024-04-22 16:36:51.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_heaobjectsupport.cpython-311-pytest-7.4.4.pyc.34244
+-rw-rw-rw-   0        0        0     6047 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_jsonschemavalidator.cpython-310-pytest-7.4.2.pyc.40340
+-rw-rw-rw-   0        0        0     2560 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_mimetypes.cpython-311-pytest-7.4.4.pyc.22664
+-rw-rw-rw-   0        0        0      956 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_not_imported.cpython-310-pytest-7.4.2.pyc.18372
+-rw-rw-rw-   0        0        0      956 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_not_imported.cpython-310-pytest-7.4.2.pyc.32764
+-rw-rw-rw-   0        0        0     1486 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.2.pyc.6392
+-rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.26632
+-rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29828
+-rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.31020
+-rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.3260
+-rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33324
+-rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.36432
+-rw-rw-rw-   0        0        0     1946 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.37972
+-rw-rw-rw-   0        0        0     2018 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.18372
+-rw-rw-rw-   0        0        0     2018 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.40340
+-rw-rw-rw-   0        0        0     2018 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.7612
+-rw-rw-rw-   0        0        0     1999 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-310-pytest-7.4.2.pyc.6392
+-rw-rw-rw-   0        0        0     2595 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.3260
+-rw-rw-rw-   0        0        0     2595 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.37972
+-rw-rw-rw-   0        0        0      673 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.2.pyc.4048
+-rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.25384
+-rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.2560
+-rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.31020
+-rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.3260
+-rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35416
+-rw-rw-rw-   0        0        0      835 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.37972
+-rw-rw-rw-   0        0        0    21683 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.23384
+-rw-rw-rw-   0        0        0    21683 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.31020
+-rw-rw-rw-   0        0        0    21683 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3260
+-rw-rw-rw-   0        0        0     1879 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.22664
+-rw-rw-rw-   0        0        0     1879 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.26660
+-rw-rw-rw-   0        0        0     1879 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35416
+-rw-rw-rw-   0        0        0     1879 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.37972
+-rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.23384
+-rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.25384
+-rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.2560
+-rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.26632
+-rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.26660
+-rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.31020
+-rw-rw-rw-   0        0        0     3365 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33324
+-rw-rw-rw-   0        0        0    10601 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-310-pytest-7.4.2.pyc.11904
+-rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.23384
+-rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.25384
+-rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.2560
+-rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.26632
+-rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.26660
+-rw-rw-rw-   0        0        0    18121 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.3260
+-rw-rw-rw-   0        0        0     6885 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-310-pytest-7.4.2.pyc.2600
+-rw-rw-rw-   0        0        0    12010 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.2560
+-rw-rw-rw-   0        0        0    12010 2024-03-28 23:13:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3260
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.339849 heaserver-1.6.3/tests/heaserver/servicetest/aiohttpdata/
+-rw-rw-rw-   0        0        0      258 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6442 2023-11-27 15:30:20.000000 heaserver-1.6.3/tests/heaserver/servicetest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0    17429 2024-05-22 22:08:38.000000 heaserver-1.6.3/tests/heaserver/servicetest/componenttestcase.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.342850 heaserver-1.6.3/tests/heaserver/servicetest/db/
+-rw-rw-rw-   0        0        0        0 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.350417 heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/
+-rw-rw-rw-   0        0        0     1030 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-310-pytest-7.4.2.pyc.4048
+-rw-rw-rw-   0        0        0     1030 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-310-pytest-7.4.2.pyc.6392
+-rw-rw-rw-   0        0        0     1353 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.25384
+-rw-rw-rw-   0        0        0     1353 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.26632
+-rw-rw-rw-   0        0        0     1353 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.3260
+-rw-rw-rw-   0        0        0     1353 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.35416
+-rw-rw-rw-   0        0        0     5790 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-310-pytest-7.4.2.pyc.2600
+-rw-rw-rw-   0        0        0     7933 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.22664
+-rw-rw-rw-   0        0        0     7933 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.2560
+-rw-rw-rw-   0        0        0     7933 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.36432
+-rw-rw-rw-   0        0        0      551 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/test_mongo.py
+-rw-rw-rw-   0        0        0     7303 2023-11-10 18:12:16.000000 heaserver-1.6.3/tests/heaserver/servicetest/db/test_mongoexpr.py
+-rw-rw-rw-   0        0        0     5563 2024-05-22 22:08:38.000000 heaserver-1.6.3/tests/heaserver/servicetest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5931 2024-05-22 22:08:38.000000 heaserver-1.6.3/tests/heaserver/servicetest/organizationtestcase.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.369988 heaserver-1.6.3/tests/heaserver/servicetest/representor/
+-rw-rw-rw-   0        0        0        0 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.411604 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/
+-rw-rw-rw-   0        0        0    46148 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-310-pytest-7.4.2.pyc.11904
+-rw-rw-rw-   0        0        0    62676 2024-04-03 20:15:45.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.17544
+-rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.22664
+-rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.23384
+-rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.2560
+-rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.26660
+-rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.31020
+-rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3260
+-rw-rw-rw-   0        0        0    54554 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35416
+-rw-rw-rw-   0        0        0     3716 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.11904
+-rw-rw-rw-   0        0        0     3716 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.18372
+-rw-rw-rw-   0        0        0     3716 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.40340
+-rw-rw-rw-   0        0        0     6478 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.29828
+-rw-rw-rw-   0        0        0     4816 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-310-pytest-7.4.2.pyc.40340
+-rw-rw-rw-   0        0        0     4816 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-310-pytest-7.4.2.pyc.4048
+-rw-rw-rw-   0        0        0     7295 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.2560
+-rw-rw-rw-   0        0        0     7295 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.26660
+-rw-rw-rw-   0        0        0     7295 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.31020
+-rw-rw-rw-   0        0        0     7295 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.3260
+-rw-rw-rw-   0        0        0      895 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-310-pytest-7.4.2.pyc.4048
+-rw-rw-rw-   0        0        0     1336 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.22664
+-rw-rw-rw-   0        0        0     1336 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.2560
+-rw-rw-rw-   0        0        0     1336 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.26632
+-rw-rw-rw-   0        0        0     1336 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.31020
+-rw-rw-rw-   0        0        0     4182 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.2600
+-rw-rw-rw-   0        0        0     4182 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.32764
+-rw-rw-rw-   0        0        0     4182 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.4048
+-rw-rw-rw-   0        0        0     4182 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.6392
+-rw-rw-rw-   0        0        0     7770 2024-04-03 20:15:45.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.18204
+-rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.23384
+-rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.25384
+-rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.26632
+-rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3260
+-rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35416
+-rw-rw-rw-   0        0        0     6199 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37972
+-rw-rw-rw-   0        0        0     7770 2024-04-03 20:15:45.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.42188
+-rw-rw-rw-   0        0        0     3079 2023-10-09 18:55:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-310-pytest-7.4.2.pyc.18372
+-rw-rw-rw-   0        0        0     4480 2024-04-03 20:15:45.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.17544
+-rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23384
+-rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.26632
+-rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.26660
+-rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29828
+-rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33324
+-rw-rw-rw-   0        0        0     5076 2024-03-28 23:13:35.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.36432
+-rw-rw-rw-   0        0        0      192 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/all.json
+-rw-rw-rw-   0        0        0      268 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/all_cj_item_href.json
+-rw-rw-rw-   0        0        0      268 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/all_cj_item_link.json
+-rw-rw-rw-   0        0        0      642 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/all_cj_queries.json
+-rw-rw-rw-   0        0        0     2670 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/all_cj_template.json
+-rw-rw-rw-   0        0        0      267 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
+-rw-rw-rw-   0        0        0      263 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
+-rw-rw-rw-   0        0        0    62769 2024-04-03 19:49:45.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/test_cj.py
+-rw-rw-rw-   0        0        0     2671 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/test_factory.py
+-rw-rw-rw-   0        0        0     4181 2023-11-27 15:30:20.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/test_nvpjson.py
+-rw-rw-rw-   0        0        0      281 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/test_supports_links.py
+-rw-rw-rw-   0        0        0     5676 2024-04-03 19:49:45.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/test_wstljson.py
+-rw-rw-rw-   0        0        0     2396 2024-03-29 20:23:19.000000 heaserver-1.6.3/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0    13067 2023-10-09 18:20:45.000000 heaserver-1.6.3/tests/heaserver/servicetest/service.py
+-rw-rw-rw-   0        0        0     9455 2024-01-29 16:35:22.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_activity.py
+-rw-rw-rw-   0        0        0     3976 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_aiohttp.py
+-rw-rw-rw-   0        0        0     5968 2024-06-01 04:55:54.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_backgroundtasks.py
+-rw-rw-rw-   0        0        0     2506 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_caching.py
+-rw-rw-rw-   0        0        0     7131 2024-04-11 00:17:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1127 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_configuration.py
+-rw-rw-rw-   0        0        0      819 2023-11-06 22:30:27.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_database_classes.py
+-rw-rw-rw-   0        0        0      204 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_delete_component.py
+-rw-rw-rw-   0        0        0     6181 2023-07-10 19:44:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_expression.py
+-rw-rw-rw-   0        0        0      405 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_functional.py
+-rw-rw-rw-   0        0        0      422 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_get_all_components.py
+-rw-rw-rw-   0        0        0     3070 2023-07-10 19:44:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_get_component.py
+-rw-rw-rw-   0        0        0      209 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     5366 2024-04-11 00:17:34.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_heaobjectsupport.py
+-rw-rw-rw-   0        0        0     5746 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_jsonschemavalidator.py
+-rw-rw-rw-   0        0        0      909 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_mimetypes.py
+-rw-rw-rw-   0        0        0      331 2023-07-25 21:24:15.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_not_imported.py
+-rw-rw-rw-   0        0        0     1005 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1274 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_post_component.py
+-rw-rw-rw-   0        0        0     1265 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_put_component.py
+-rw-rw-rw-   0        0        0      253 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_put_organization_permissions.py
+-rw-rw-rw-   0        0        0     2488 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_response.py
+-rw-rw-rw-   0        0        0      570 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_testenv.py
+-rw-rw-rw-   0        0        0     1929 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_uritemplate.py
+-rw-rw-rw-   0        0        0     8782 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_util.py
+-rw-rw-rw-   0        0        0     6255 2023-06-07 14:43:05.000000 heaserver-1.6.3/tests/heaserver/servicetest/test_wstl.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:30:09.412604 heaserver-1.6.3/tests/heaserver/servicetest/wstl/
+-rw-rw-rw-   0        0        0    16436 2023-10-09 18:20:45.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl/all.json
+-rw-rw-rw-   0        0        0     1185 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_1.json
+-rw-rw-rw-   0        0        0     1214 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_10a.json
+-rw-rw-rw-   0        0        0     1240 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_10b.json
+-rw-rw-rw-   0        0        0     2355 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_11.json
+-rw-rw-rw-   0        0        0     1187 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_2.json
+-rw-rw-rw-   0        0        0     1190 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_3.json
+-rw-rw-rw-   0        0        0     1158 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_4.json
+-rw-rw-rw-   0        0        0      269 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_5.json
+-rw-rw-rw-   0        0        0      531 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_6.json
+-rw-rw-rw-   0        0        0     1185 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_7.json
+-rw-rw-rw-   0        0        0     1185 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_8.json
+-rw-rw-rw-   0        0        0      204 2023-06-07 14:42:11.000000 heaserver-1.6.3/tests/heaserver/servicetest/wstl_9.json
```

### Comparing `heaserver-1.6.2/LICENSE` & `heaserver-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/PKG-INFO` & `heaserver-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.6.2
+Version: 1.6.3
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaobject~=1.6.3
+Requires-Dist: heaobject~=1.6.4
 Requires-Dist: aiohttp[speedups]~=3.8.6
 Requires-Dist: hea-aiohttp-remotes~=1.2.1
 Requires-Dist: motor~=3.2.0
 Requires-Dist: motor-types~=1.0.0b2
 Requires-Dist: accept-types~=0.4.1
 Requires-Dist: mongoquery~=1.4.2
 Requires-Dist: jsonschema~=4.17.3
@@ -47,18 +47,21 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.6.3
+* Upgrading heaobject dependency to get bug fixes.
+
 ## Version 1.6.2
-* Added ability to toggle aws key duration depending on if system credential manager or any other user
-* Background tasks now pass the aiohttp app object as a parameter of the coroutine added to the queue
-* Added the scheduled_cleanup_ctx manager for scheduling reoccurring tasks with a delay optionally
+* Added ability to toggle aws key duration depending on if system credential manager or any other user.
+* Background tasks now pass the aiohttp app object as a parameter of the coroutine added to the queue.
+* Added the scheduled_cleanup_ctx manager for scheduling reoccurring tasks with a delay optionally.
 * Prevent the id field from appearing in mongodb when a new desktop object is inserted.
 
 
 ## Version 1.6.0
 * Improved docstrings.
 * New heaobject dependency.
 * Removed account_type_names parameters from heaserver.service.db.database.get_volumes and heaserver.service.db.database.Database.get_volumes.
```

### Comparing `heaserver-1.6.2/README.md` & `heaserver-1.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.6.3
+* Upgrading heaobject dependency to get bug fixes.
+
 ## Version 1.6.2
-* Added ability to toggle aws key duration depending on if system credential manager or any other user
-* Background tasks now pass the aiohttp app object as a parameter of the coroutine added to the queue
-* Added the scheduled_cleanup_ctx manager for scheduling reoccurring tasks with a delay optionally
+* Added ability to toggle aws key duration depending on if system credential manager or any other user.
+* Background tasks now pass the aiohttp app object as a parameter of the coroutine added to the queue.
+* Added the scheduled_cleanup_ctx manager for scheduling reoccurring tasks with a delay optionally.
 * Prevent the id field from appearing in mongodb when a new desktop object is inserted.
 
 
 ## Version 1.6.0
 * Improved docstrings.
 * New heaobject dependency.
 * Removed account_type_names parameters from heaserver.service.db.database.get_volumes and heaserver.service.db.database.Database.get_volumes.
```

### Comparing `heaserver-1.6.2/RELEASING.md` & `heaserver-1.6.3/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py` & `heaserver-1.6.3/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3integrationtests/heaserver/awss3tests/service.py` & `heaserver-1.6.3/awss3integrationtests/heaserver/awss3tests/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3integrationtests/heaserver/awss3tests/test_all.py` & `heaserver-1.6.3/awss3integrationtests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3integrationtests/heaserver/awss3tests/wstl/all.json` & `heaserver-1.6.3/awss3integrationtests/heaserver/awss3tests/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.22664` & `heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.22664`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.2560` & `heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.2560`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.26632` & `heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.26632`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29828` & `heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29828`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.3260` & `heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.3260`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35416` & `heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35416`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.37972` & `heaserver-1.6.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.37972`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/awss3tests/heaserver/awss3tests/test_all.py` & `heaserver-1.6.3/awss3tests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.20088` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.20088`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.31660` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.31660`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.33616` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.33616`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.35072` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.35072`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.39964` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.39964`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.41268` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.41268`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.5640` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.5640`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.44660` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.44660`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.26264` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.26264`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.31660` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.31660`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.39964` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-311-pytest-7.4.4.pyc.39964`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-311-pytest-7.4.4.pyc.5352` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-311-pytest-7.4.4.pyc.5352`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.41268` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.41268`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.5352` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.5352`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/service.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_client.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_get_component.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/test_post_component.py` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/integrationtests/heaserver/serviceintegrationtest/wstl/all.json` & `heaserver-1.6.3/integrationtests/heaserver/serviceintegrationtest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/setup.py` & `heaserver-1.6.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='heaserver',
-      version='1.6.2',
+      version='1.6.3',
       description='The server side of HEA.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://risr.hci.utah.edu',
       author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
       author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
       package_dir={'': 'src'},
       packages=find_namespace_packages(where='src'),
       package_data={'heaserver.service': ['py.typed', 'jsonschemafiles/*']},
       install_requires=[
-          'heaobject~=1.6.3',
+          'heaobject~=1.6.4',
           'aiohttp[speedups]~=3.8.6',
           'hea-aiohttp-remotes~=1.2.1',  # replace with aiohttp-remotes if they incorporate our patch.
           'motor~=3.2.0',
           'motor-types~=1.0.0b2',
           'accept-types~=0.4.1',
           'mongoquery~=1.4.2',
           'jsonschema~=4.17.3',
```

### Comparing `heaserver-1.6.2/src/heaserver/service/__init__.py` & `heaserver-1.6.3/src/heaserver/service/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/activity.py` & `heaserver-1.6.3/src/heaserver/service/activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/aiohttp.py` & `heaserver-1.6.3/src/heaserver/service/aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/appfactory.py` & `heaserver-1.6.3/src/heaserver/service/appfactory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/appproperty.py` & `heaserver-1.6.3/src/heaserver/service/appproperty.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/backgroundtasks.py` & `heaserver-1.6.3/src/heaserver/service/backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/caching.py` & `heaserver-1.6.3/src/heaserver/service/caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/client.py` & `heaserver-1.6.3/src/heaserver/service/client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/config.py` & `heaserver-1.6.3/src/heaserver/service/config.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/db/aws.py` & `heaserver-1.6.3/src/heaserver/service/db/aws.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/db/awsservicelib.py` & `heaserver-1.6.3/src/heaserver/service/db/awsservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/db/database.py` & `heaserver-1.6.3/src/heaserver/service/db/database.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/db/dbapi2.py` & `heaserver-1.6.3/src/heaserver/service/db/dbapi2.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/db/mongo.py` & `heaserver-1.6.3/src/heaserver/service/db/mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/db/mongoexpr.py` & `heaserver-1.6.3/src/heaserver/service/db/mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/db/mongoservicelib.py` & `heaserver-1.6.3/src/heaserver/service/db/mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/expression.py` & `heaserver-1.6.3/src/heaserver/service/expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/functional.py` & `heaserver-1.6.3/src/heaserver/service/functional.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/heaobjectsupport.py` & `heaserver-1.6.3/src/heaserver/service/heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/jsonschema.py` & `heaserver-1.6.3/src/heaserver/service/jsonschema.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/jsonschemafiles/__init__.py` & `heaserver-1.6.3/src/heaserver/service/jsonschemafiles/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/jsonschemafiles/cjtemplate.json` & `heaserver-1.6.3/src/heaserver/service/jsonschemafiles/cjtemplate.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/jsonschemafiles/wstl.json` & `heaserver-1.6.3/src/heaserver/service/jsonschemafiles/wstl.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/jsonschemafiles/wstlaction.json` & `heaserver-1.6.3/src/heaserver/service/jsonschemafiles/wstlaction.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/jsonschemavalidator.py` & `heaserver-1.6.3/src/heaserver/service/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/messagebroker.py` & `heaserver-1.6.3/src/heaserver/service/messagebroker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/mimetypes.py` & `heaserver-1.6.3/src/heaserver/service/mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/oidcclaimhdrs.py` & `heaserver-1.6.3/src/heaserver/service/oidcclaimhdrs.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/openapi.py` & `heaserver-1.6.3/src/heaserver/service/openapi.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/representor/__init__.py` & `heaserver-1.6.3/src/heaserver/service/representor/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/representor/cj.py` & `heaserver-1.6.3/src/heaserver/service/representor/cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/representor/factory.py` & `heaserver-1.6.3/src/heaserver/service/representor/factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/representor/nvpjson.py` & `heaserver-1.6.3/src/heaserver/service/representor/nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/representor/representor.py` & `heaserver-1.6.3/src/heaserver/service/representor/representor.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/representor/wstljson.py` & `heaserver-1.6.3/src/heaserver/service/representor/wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/representor/xwwwformurlencoded.py` & `heaserver-1.6.3/src/heaserver/service/representor/xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/response.py` & `heaserver-1.6.3/src/heaserver/service/response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/runner.py` & `heaserver-1.6.3/src/heaserver/service/runner.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/aiohttptestcase.py` & `heaserver-1.6.3/src/heaserver/service/testcase/aiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/awsdockermongo.py` & `heaserver-1.6.3/src/heaserver/service/testcase/awsdockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/awss3microservicetestcase.py` & `heaserver-1.6.3/src/heaserver/service/testcase/awss3microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/collection.py` & `heaserver-1.6.3/src/heaserver/service/testcase/collection.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/docker.py` & `heaserver-1.6.3/src/heaserver/service/testcase/docker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/dockermongo.py` & `heaserver-1.6.3/src/heaserver/service/testcase/dockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/expectedvalues.py` & `heaserver-1.6.3/src/heaserver/service/testcase/expectedvalues.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/microservicetestcase.py` & `heaserver-1.6.3/src/heaserver/service/testcase/microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/mixin.py` & `heaserver-1.6.3/src/heaserver/service/testcase/mixin.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/mockaws.py` & `heaserver-1.6.3/src/heaserver/service/testcase/mockaws.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/mockdatabase.py` & `heaserver-1.6.3/src/heaserver/service/testcase/mockdatabase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/mockmongo.py` & `heaserver-1.6.3/src/heaserver/service/testcase/mockmongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/simpleaiohttptestcase.py` & `heaserver-1.6.3/src/heaserver/service/testcase/simpleaiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/swaggerui.py` & `heaserver-1.6.3/src/heaserver/service/testcase/swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/testenv.py` & `heaserver-1.6.3/src/heaserver/service/testcase/testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/testcase/util.py` & `heaserver-1.6.3/src/heaserver/service/testcase/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/uritemplate.py` & `heaserver-1.6.3/src/heaserver/service/uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/util.py` & `heaserver-1.6.3/src/heaserver/service/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver/service/wstl.py` & `heaserver-1.6.3/src/heaserver/service/wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/src/heaserver.egg-info/PKG-INFO` & `heaserver-1.6.3/src/heaserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.6.2
+Version: 1.6.3
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaobject~=1.6.3
+Requires-Dist: heaobject~=1.6.4
 Requires-Dist: aiohttp[speedups]~=3.8.6
 Requires-Dist: hea-aiohttp-remotes~=1.2.1
 Requires-Dist: motor~=3.2.0
 Requires-Dist: motor-types~=1.0.0b2
 Requires-Dist: accept-types~=0.4.1
 Requires-Dist: mongoquery~=1.4.2
 Requires-Dist: jsonschema~=4.17.3
@@ -47,18 +47,21 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.6.3
+* Upgrading heaobject dependency to get bug fixes.
+
 ## Version 1.6.2
-* Added ability to toggle aws key duration depending on if system credential manager or any other user
-* Background tasks now pass the aiohttp app object as a parameter of the coroutine added to the queue
-* Added the scheduled_cleanup_ctx manager for scheduling reoccurring tasks with a delay optionally
+* Added ability to toggle aws key duration depending on if system credential manager or any other user.
+* Background tasks now pass the aiohttp app object as a parameter of the coroutine added to the queue.
+* Added the scheduled_cleanup_ctx manager for scheduling reoccurring tasks with a delay optionally.
 * Prevent the id field from appearing in mongodb when a new desktop object is inserted.
 
 
 ## Version 1.6.0
 * Improved docstrings.
 * New heaobject dependency.
 * Removed account_type_names parameters from heaserver.service.db.database.get_volumes and heaserver.service.db.database.Database.get_volumes.
```

### Comparing `heaserver-1.6.2/src/heaserver.egg-info/SOURCES.txt` & `heaserver-1.6.3/src/heaserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.25384` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.25384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.13192` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.13192`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.13688` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.13688`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.20088` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.20088`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.22664` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.22664`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.23744` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.23744`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.25384` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.25384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.28100` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.28100`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.39288` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.39288`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.39964` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.39964`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.41428` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.41428`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.42872` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.42872`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.44660` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.44660`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.5212` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.5212`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.6356` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_backgroundtasks.cpython-311-pytest-7.4.4.pyc.6356`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.26632` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.26632`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.41148` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.41148`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.5676` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.5676`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.2.pyc.40340` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.2.pyc.40340`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.22664` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.22664`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.26632` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.26632`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35416` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35416`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_functional.cpython-311-pytest-7.4.4.pyc.22664` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_functional.cpython-311-pytest-7.4.4.pyc.22664`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_get_all_components.cpython-311-pytest-7.4.4.pyc.23384` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_get_all_components.cpython-311-pytest-7.4.4.pyc.23384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_heaobjectsupport.cpython-311-pytest-7.4.4.pyc.34244` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_heaobjectsupport.cpython-311-pytest-7.4.4.pyc.34244`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_jsonschemavalidator.cpython-310-pytest-7.4.2.pyc.40340` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_jsonschemavalidator.cpython-310-pytest-7.4.2.pyc.40340`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_mimetypes.cpython-311-pytest-7.4.4.pyc.22664` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_mimetypes.cpython-311-pytest-7.4.4.pyc.22664`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_not_imported.cpython-310-pytest-7.4.2.pyc.18372` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_not_imported.cpython-310-pytest-7.4.2.pyc.18372`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_not_imported.cpython-310-pytest-7.4.2.pyc.32764` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_not_imported.cpython-310-pytest-7.4.2.pyc.32764`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.2.pyc.6392` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.2.pyc.6392`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.26632` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.26632`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29828` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29828`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.31020` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.31020`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.3260` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.3260`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33324` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33324`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.36432` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.36432`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.37972` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.37972`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.18372` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.18372`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.40340` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.40340`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.7612` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-310-pytest-7.4.2.pyc.7612`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-310-pytest-7.4.2.pyc.6392` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-310-pytest-7.4.2.pyc.6392`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.3260` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.3260`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.37972` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.37972`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.2.pyc.4048` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.2.pyc.4048`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.25384` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.25384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.2560` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.2560`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.31020` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.31020`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.3260` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.3260`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35416` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35416`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.37972` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.37972`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.23384` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.23384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.31020` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.31020`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3260` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3260`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.22664` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.22664`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.26660` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.26660`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35416` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35416`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.37972` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.37972`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.23384` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.23384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.25384` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.25384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.2560` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.2560`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.26632` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.26632`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.26660` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.26660`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.31020` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.31020`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33324` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33324`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-310-pytest-7.4.2.pyc.11904` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-310-pytest-7.4.2.pyc.11904`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.23384` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.23384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.25384` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.25384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.2560` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.2560`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.26632` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.26632`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.26660` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.26660`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.3260` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.3260`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-310-pytest-7.4.2.pyc.2600` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-310-pytest-7.4.2.pyc.2600`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.2560` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.2560`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3260` & `heaserver-1.6.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3260`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/componentpermissionstestcase.py` & `heaserver-1.6.3/tests/heaserver/servicetest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/componenttestcase.py` & `heaserver-1.6.3/tests/heaserver/servicetest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-310-pytest-7.4.2.pyc.4048` & `heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-310-pytest-7.4.2.pyc.4048`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-310-pytest-7.4.2.pyc.6392` & `heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-310-pytest-7.4.2.pyc.6392`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.25384` & `heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.25384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.26632` & `heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.26632`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.3260` & `heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.3260`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.35416` & `heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.35416`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-310-pytest-7.4.2.pyc.2600` & `heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-310-pytest-7.4.2.pyc.2600`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.22664` & `heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.22664`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.2560` & `heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.2560`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.36432` & `heaserver-1.6.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.36432`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/test_mongo.py` & `heaserver-1.6.3/tests/heaserver/servicetest/db/test_mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/db/test_mongoexpr.py` & `heaserver-1.6.3/tests/heaserver/servicetest/db/test_mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/organizationpermissionstestcase.py` & `heaserver-1.6.3/tests/heaserver/servicetest/organizationpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/organizationtestcase.py` & `heaserver-1.6.3/tests/heaserver/servicetest/organizationtestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-310-pytest-7.4.2.pyc.11904` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-310-pytest-7.4.2.pyc.11904`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.17544` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.17544`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.22664` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.22664`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.23384` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.23384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.2560` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.2560`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.26660` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.26660`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.31020` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.31020`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3260` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3260`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35416` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35416`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.11904` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.11904`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.18372` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.18372`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.40340` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-310-pytest-7.4.2.pyc.40340`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.29828` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.29828`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-310-pytest-7.4.2.pyc.40340` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-310-pytest-7.4.2.pyc.40340`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-310-pytest-7.4.2.pyc.4048` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-310-pytest-7.4.2.pyc.4048`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.2560` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.2560`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.26660` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.26660`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.31020` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.31020`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.3260` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.3260`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-310-pytest-7.4.2.pyc.4048` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-310-pytest-7.4.2.pyc.4048`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.22664` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.22664`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.2560` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.2560`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.26632` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.26632`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.31020` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.31020`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.2600` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.2600`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.32764` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.32764`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.4048` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.4048`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.6392` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-310-pytest-7.4.2.pyc.6392`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.18204` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.18204`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.23384` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.23384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.25384` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.25384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.26632` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.26632`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3260` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3260`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35416` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35416`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37972` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37972`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.42188` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.42188`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-310-pytest-7.4.2.pyc.18372` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-310-pytest-7.4.2.pyc.18372`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.17544` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.17544`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23384` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23384`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.26632` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.26632`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.26660` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.26660`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29828` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29828`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33324` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33324`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.36432` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.36432`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/all_cj_queries.json` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/all_cj_queries.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/all_cj_template.json` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/all_cj_template.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/test_cj.py` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/test_cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/test_factory.py` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/test_factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/test_nvpjson.py` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/test_nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/test_wstljson.py` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/test_wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py` & `heaserver-1.6.3/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/service.py` & `heaserver-1.6.3/tests/heaserver/servicetest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_activity.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_aiohttp.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_backgroundtasks.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_caching.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_client.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_component_with_bad_permissions.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_configuration.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_configuration.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_database_classes.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_database_classes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_expression.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_get_component.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_heaobjectsupport.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_jsonschemavalidator.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_mimetypes.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_organization_with_bad_permissions.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_post_component.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_put_component.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_put_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_response.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_testenv.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_uritemplate.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_util.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/test_wstl.py` & `heaserver-1.6.3/tests/heaserver/servicetest/test_wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/wstl/all.json` & `heaserver-1.6.3/tests/heaserver/servicetest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/wstl_1.json` & `heaserver-1.6.3/tests/heaserver/servicetest/wstl_1.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/wstl_10a.json` & `heaserver-1.6.3/tests/heaserver/servicetest/wstl_10a.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/wstl_10b.json` & `heaserver-1.6.3/tests/heaserver/servicetest/wstl_10b.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/wstl_11.json` & `heaserver-1.6.3/tests/heaserver/servicetest/wstl_11.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/wstl_2.json` & `heaserver-1.6.3/tests/heaserver/servicetest/wstl_2.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/wstl_3.json` & `heaserver-1.6.3/tests/heaserver/servicetest/wstl_3.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/wstl_4.json` & `heaserver-1.6.3/tests/heaserver/servicetest/wstl_4.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/wstl_6.json` & `heaserver-1.6.3/tests/heaserver/servicetest/wstl_6.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/wstl_7.json` & `heaserver-1.6.3/tests/heaserver/servicetest/wstl_7.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.6.2/tests/heaserver/servicetest/wstl_8.json` & `heaserver-1.6.3/tests/heaserver/servicetest/wstl_8.json`

 * *Files identical despite different names*

