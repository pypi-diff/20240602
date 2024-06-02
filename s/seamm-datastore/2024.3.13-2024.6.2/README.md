# Comparing `tmp/seamm_datastore-2024.3.13.tar.gz` & `tmp/seamm_datastore-2024.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm_datastore-2024.3.13.tar", last modified: Wed Mar 13 16:13:47 2024, max compression
+gzip compressed data, was "seamm_datastore-2024.6.2.tar", last modified: Sun Jun  2 18:57:03 2024, max compression
```

## Comparing `seamm_datastore-2024.3.13.tar` & `seamm_datastore-2024.6.2.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.926979 seamm_datastore-2024.3.13/
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-03-13 16:13:47.926979 seamm_datastore-2024.3.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/requirements_install.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.930979 seamm_datastore-2024.3.13/seamm_datastore/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-13 16:13:47.930979 seamm_datastore-2024.3.13/seamm_datastore/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/connect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.918979 seamm_datastore-2024.3.13/seamm_datastore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.910979 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.914979 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.918979 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.918979 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/1/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/1/step.out
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.922979 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/band.out
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/charges.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/detailed.out
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/dftb_in.hsd
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/dftb_pin.hsd
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/geom.out.gen
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/geom.out.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/results.tag
--rw-r--r--   0 runner    (1001) docker     (127)    28636 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/step.out
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/final_structure.mmcif
--rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/flowchart.flow
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/job.out
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/job_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    73728 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/references.db
--rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/seamm.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.922979 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.922979 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/1/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/1/step.out
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.926979 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/band.out
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/charges.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/detailed.out
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/dftb_in.hsd
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/dftb_pin.hsd
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/geom.out.gen
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/geom.out.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/results.tag
--rw-r--r--   0 runner    (1001) docker     (127)    28636 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/step.out
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/final_structure.mmcif
--rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/flowchart.flow
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/job.out
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/job_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    73728 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/references.db
--rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/seamm.db
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/data/sample_flowchart_v2.flow
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.926979 seamm_datastore-2024.3.13/seamm_datastore/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.926979 seamm_datastore-2024.3.13/seamm_datastore/database/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/database/alembic/README
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/database/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/database/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.926979 seamm_datastore-2024.3.13/seamm_datastore/database/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/database/alembic/versions/7b24598d1fee_remove_path_add_flowchart_metadata_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/database/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/database/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    24775 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/database/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/database/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/flask_authorize_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.926979 seamm_datastore-2024.3.13/seamm_datastore/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/tests/test_seamm_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/seamm_datastore/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:13:47.926979 seamm_datastore-2024.3.13/seamm_datastore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-03-13 16:13:47.000000 seamm_datastore-2024.3.13/seamm_datastore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-03-13 16:13:47.000000 seamm_datastore-2024.3.13/seamm_datastore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 16:13:47.000000 seamm_datastore-2024.3.13/seamm_datastore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-13 16:13:47.000000 seamm_datastore-2024.3.13/seamm_datastore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-13 16:13:47.000000 seamm_datastore-2024.3.13/seamm_datastore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-13 16:13:47.930979 seamm_datastore-2024.3.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-03-13 16:13:28.000000 seamm_datastore-2024.3.13/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.415053 seamm_datastore-2024.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-06-02 18:57:03.415053 seamm_datastore-2024.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/requirements_install.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.415053 seamm_datastore-2024.6.2/seamm_datastore/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-02 18:57:03.415053 seamm_datastore-2024.6.2/seamm_datastore/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.403053 seamm_datastore-2024.6.2/seamm_datastore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.399052 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.399052 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.403053 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.403053 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/1/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/1/step.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.407053 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/band.out
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/charges.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/detailed.out
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/dftb_in.hsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/dftb_pin.hsd
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/geom.out.gen
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/geom.out.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/results.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    28636 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/step.out
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/final_structure.mmcif
+-rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/flowchart.flow
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/job.out
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/job_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    73728 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/references.db
+-rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/seamm.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.407053 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.407053 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/1/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/1/step.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.411053 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/band.out
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/charges.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/detailed.out
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/dftb_in.hsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/dftb_pin.hsd
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/geom.out.gen
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/geom.out.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/results.tag
+-rw-r--r--   0 runner    (1001) docker     (127)    28636 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/step.out
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/final_structure.mmcif
+-rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/flowchart.flow
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/job.out
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/job_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    73728 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/references.db
+-rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/seamm.db
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/data/sample_flowchart_v2.flow
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.411053 seamm_datastore-2024.6.2/seamm_datastore/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.411053 seamm_datastore-2024.6.2/seamm_datastore/database/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/database/alembic/README
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/database/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/database/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.411053 seamm_datastore-2024.6.2/seamm_datastore/database/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/database/alembic/versions/7b24598d1fee_remove_path_add_flowchart_metadata_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/database/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/database/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25094 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/database/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/database/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/flask_authorize_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.411053 seamm_datastore-2024.6.2/seamm_datastore/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/tests/test_seamm_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/seamm_datastore/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:57:03.411053 seamm_datastore-2024.6.2/seamm_datastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-06-02 18:57:03.000000 seamm_datastore-2024.6.2/seamm_datastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-06-02 18:57:03.000000 seamm_datastore-2024.6.2/seamm_datastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:57:03.000000 seamm_datastore-2024.6.2/seamm_datastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-06-02 18:57:03.000000 seamm_datastore-2024.6.2/seamm_datastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 18:57:03.000000 seamm_datastore-2024.6.2/seamm_datastore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-06-02 18:57:03.415053 seamm_datastore-2024.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-06-02 18:56:47.000000 seamm_datastore-2024.6.2/versioneer.py
```

### Comparing `seamm_datastore-2024.3.13/CODE_OF_CONDUCT.md` & `seamm_datastore-2024.6.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/LICENSE` & `seamm_datastore-2024.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/PKG-INFO` & `seamm_datastore-2024.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_datastore
-Version: 2024.3.13
+Version: 2024.6.2
 Summary: seamm_datastore
 Home-page: https://github.com/molssi-seamm/seamm_datastore
 Author: Jessica A. Nash (The Molecular Sciences Software Institute)
 Author-email: janash@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,datastore,dashboard
 Platform: Linux
```

### Comparing `seamm_datastore-2024.3.13/README.md` & `seamm_datastore-2024.6.2/README.md`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/connect.py` & `seamm_datastore-2024.6.2/seamm_datastore/connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,17 +148,14 @@
             self.login(username, password)
         else:
             self._user = None
 
         # Current user has to be bound before we can add anything else to be database.
         self.authorize = Authorize(current_user=self.current_user)
 
-        # Default group
-        self.default_group = Group.query.get(2).name
-
         # Now handle the project
         project = Project.query.filter_by(name=default_project).one_or_none()
         if not project:
             raise ValueError("Invalid project name given for default.")
 
         self.default_project = default_project
```

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/band.out` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/band.out`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/charges.dat` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/charges.dat`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/detailed.out` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/detailed.out`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/dftb_in.hsd` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/dftb_in.hsd`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/dftb_pin.hsd` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/dftb_pin.hsd`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/geom.out.gen` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/geom.out.gen`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/geom.out.xyz` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/geom.out.xyz`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/results.tag` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/results.tag`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/2/stdout.txt` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/2/stdout.txt`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/final_structure.mmcif` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/final_structure.mmcif`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/flowchart.flow` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/flowchart.flow`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/job.out` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/job.out`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/job_data.json` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/job_data.json`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/references.db` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/references.db`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000092/seamm.db` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000092/seamm.db`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/band.out` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/band.out`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/charges.dat` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/charges.dat`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/detailed.out` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/detailed.out`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/dftb_in.hsd` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/dftb_in.hsd`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/dftb_pin.hsd` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/dftb_pin.hsd`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/geom.out.gen` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/geom.out.gen`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/geom.out.xyz` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/geom.out.xyz`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/results.tag` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/results.tag`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/2/stdout.txt` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/2/stdout.txt`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/final_structure.mmcif` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/final_structure.mmcif`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/flowchart.flow` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/flowchart.flow`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/job.out` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/job.out`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/job_data.json` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/job_data.json`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/references.db` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/references.db`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/Projects/sample_project1/Job_000093/seamm.db` & `seamm_datastore-2024.6.2/seamm_datastore/data/Projects/sample_project1/Job_000093/seamm.db`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/data/sample_flowchart_v2.flow` & `seamm_datastore-2024.6.2/seamm_datastore/data/sample_flowchart_v2.flow`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/database/alembic/env.py` & `seamm_datastore-2024.6.2/seamm_datastore/database/alembic/env.py`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/database/alembic/versions/7b24598d1fee_remove_path_add_flowchart_metadata_.py` & `seamm_datastore-2024.6.2/seamm_datastore/database/alembic/versions/7b24598d1fee_remove_path_add_flowchart_metadata_.py`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/database/alembic.ini` & `seamm_datastore-2024.6.2/seamm_datastore/database/alembic.ini`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/database/build.py` & `seamm_datastore-2024.6.2/seamm_datastore/database/build.py`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/database/models.py` & `seamm_datastore-2024.6.2/seamm_datastore/database/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,20 +162,28 @@
             last_name=last_name,
             email=email,
         )
         for role_name in roles:
             role = Role.query.filter_by(name=role_name).one()
             new_user.roles.append(role)
 
-        if groups is None:
-            groups = [Group.query.get(2).name]
-
-        for group_name in groups:
-            group = Group.query.filter_by(name=group_name).one()
-            new_user.groups.append(group)
+        if not groups:
+            new_group = Group.create(username, [])
+            new_user.groups.append(new_group)
+        else:
+            for group_name in groups:
+                group = Group.query.filter_by(name=group_name).one()
+                new_user.groups.append(group)
+
+        if not roles:
+            new_user.roles.append(Role.query.filter_by(name="user").one())
+        else:
+            for role in roles:
+                role = Role.query.filter_by(name=role).one()
+                new_user.roles.append(role)
 
         return new_user
 
 
 class Group(Base):
     __tablename__ = "groups"
```

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/database/schema.py` & `seamm_datastore-2024.6.2/seamm_datastore/database/schema.py`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/flask_authorize_patch.py` & `seamm_datastore-2024.6.2/seamm_datastore/flask_authorize_patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,17 +93,24 @@
     return PermissionsAssociationMixin
 
 
 class AccessControlPermissionsMixin(PermissionsMixin):
     @classmethod
     def authorized(cls, check):
         from flask_authorize.plugin import CURRENT_USER
+        from sqlalchemy.sql.expression import true
 
         current_user = CURRENT_USER()
 
+        # check if the user is an admin
+        # return True if admin - they're allowed to do anything!
+        if current_user:
+            if "admin" in [x.name for x in current_user.roles]:
+                return true()
+
         ret = super().authorized(check)
 
         clauses = []
 
         # Check user for special permissions
         if hasattr(current_user, f"special_{cls.__tablename__}"):
             clauses.append(
@@ -128,15 +135,16 @@
                 for x in group_list
                 for y in x
                 if y.entity_id in [n.id for n in current_user.groups]
                 if check in y.permissions
             ]
             clauses.append(cls.id.in_(overlapping_groups))
 
-        return or_(ret, or_(False, *clauses))
+        check = or_(ret, or_(False, *clauses))
+        return check
 
 
 def allowed(self, *args, **kwargs):  # pragma: no cover
     from flask_authorize.plugin import CURRENT_USER
 
     # look to flask-login for current user
     user = kwargs.get("user")
@@ -148,14 +156,19 @@
         user = user()
 
     # don't allow anything for anonymous users
     if user is None:
         if not current_app.config["AUTHORIZE_ALLOW_ANONYMOUS_ACTIONS"]:
             return False
 
+    # check if the user is an admin
+    # return True if admin - they're allowed to do anything!
+    if "admin" in [x.name for x in user.roles]:
+        return True
+
     # authorize if user has relevant role
     if len(self.has_role):
         if user_has_role(user, self.has_role):
             return True
         elif not len(self.permission) and not len(self.create):
             return False
```

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/tests/conftest.py` & `seamm_datastore-2024.6.2/seamm_datastore/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/tests/test_create.py` & `seamm_datastore-2024.6.2/seamm_datastore/tests/test_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     )
 
 
 def test_create_user(connection):
     user = connection.User.create(username="test", password="test")
 
     assert user.username == "test"
-    assert user.groups[0].name == connection.default_group
+    assert user.groups[0].name == user.username
 
 
 def test_add_job(connection):
     from pathlib import Path
     from dateutil import parser
 
     from seamm_datastore import session_scope
```

### Comparing `seamm_datastore-2024.3.13/seamm_datastore/tests/test_methods.py` & `seamm_datastore-2024.6.2/seamm_datastore/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/seamm_datastore.egg-info/PKG-INFO` & `seamm_datastore-2024.6.2/seamm_datastore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_datastore
-Version: 2024.3.13
+Version: 2024.6.2
 Summary: seamm_datastore
 Home-page: https://github.com/molssi-seamm/seamm_datastore
 Author: Jessica A. Nash (The Molecular Sciences Software Institute)
 Author-email: janash@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,datastore,dashboard
 Platform: Linux
```

### Comparing `seamm_datastore-2024.3.13/seamm_datastore.egg-info/SOURCES.txt` & `seamm_datastore-2024.6.2/seamm_datastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/setup.py` & `seamm_datastore-2024.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `seamm_datastore-2024.3.13/versioneer.py` & `seamm_datastore-2024.6.2/versioneer.py`

 * *Files identical despite different names*

