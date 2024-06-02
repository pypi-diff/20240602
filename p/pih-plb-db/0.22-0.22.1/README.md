# Comparing `tmp/pih-plb_db-0.22.tar.gz` & `tmp/pih-plb_db-0.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_db-0.22.tar", last modified: Sun May 26 11:56:11 2024, max compression
+gzip compressed data, was "pih-plb_db-0.22.1.tar", last modified: Sun Jun  2 01:44:41 2024, max compression
```

## Comparing `pih-plb_db-0.22.tar` & `pih-plb_db-0.22.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 11:56:11.838426 pih-plb_db-0.22/
--rw-rw-rw-   0        0        0      280 2024-05-26 11:56:11.807179 pih-plb_db-0.22/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-26 11:56:11.432193 pih-plb_db-0.22/PolibaseDatabaseService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.22/PolibaseDatabaseService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.22/PolibaseDatabaseService/__main__.py
--rw-rw-rw-   0        0        0     7279 2024-05-26 11:55:46.000000 pih-plb_db-0.22/PolibaseDatabaseService/api.py
--rw-rw-rw-   0        0        0      848 2024-05-26 11:55:56.000000 pih-plb_db-0.22/PolibaseDatabaseService/const.py
--rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.22/PolibaseDatabaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:56:11.775931 pih-plb_db-0.22/pih_plb_db.egg-info/
--rw-rw-rw-   0        0        0      280 2024-05-26 11:56:10.000000 pih-plb_db-0.22/pih_plb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-26 11:56:11.000000 pih-plb_db-0.22/pih_plb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 11:56:11.000000 pih-plb_db-0.22/pih_plb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-26 11:56:11.000000 pih-plb_db-0.22/pih_plb_db.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-26 11:56:11.000000 pih-plb_db-0.22/pih_plb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-26 11:56:11.000000 pih-plb_db-0.22/pih_plb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 11:56:11.838426 pih-plb_db-0.22/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 01:44:41.929109 pih-plb_db-0.22.1/
+-rw-rw-rw-   0        0        0      282 2024-06-02 01:44:41.897858 pih-plb_db-0.22.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 01:44:41.542914 pih-plb_db-0.22.1/PolibaseDatabaseService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.22.1/PolibaseDatabaseService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.22.1/PolibaseDatabaseService/__main__.py
+-rw-rw-rw-   0        0        0     7327 2024-06-02 01:43:23.000000 pih-plb_db-0.22.1/PolibaseDatabaseService/api.py
+-rw-rw-rw-   0        0        0      850 2024-06-02 01:39:17.000000 pih-plb_db-0.22.1/PolibaseDatabaseService/const.py
+-rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.22.1/PolibaseDatabaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-06-02 01:44:41.866618 pih-plb_db-0.22.1/pih_plb_db.egg-info/
+-rw-rw-rw-   0        0        0      282 2024-06-02 01:44:40.000000 pih-plb_db-0.22.1/pih_plb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-06-02 01:44:41.000000 pih-plb_db-0.22.1/pih_plb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 01:44:40.000000 pih-plb_db-0.22.1/pih_plb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-06-02 01:44:40.000000 pih-plb_db-0.22.1/pih_plb_db.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-06-02 01:44:40.000000 pih-plb_db-0.22.1/pih_plb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-06-02 01:44:40.000000 pih-plb_db-0.22.1/pih_plb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 01:44:41.965917 pih-plb_db-0.22.1/setup.cfg
```

### Comparing `pih-plb_db-0.22/PolibaseDatabaseService/api.py` & `pih-plb_db-0.22.1/PolibaseDatabaseService/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             os.path.getsize(A.PTH.join(polibase_folder_path, file_out_name)), not test
         )
 
         # step 4
         A.E.backup_notify_about_polibase_coping_archived_db_dumb_start(
             A.CT_H.NAS.ALIAS.upper()
         )
-        os.system(nas_copy_command)
+        A.L.debug_bot(j((nas_copy_command, ":", str(os.system(nas_copy_command)))))
         A.E.backup_notify_about_polibase_coping_archived_db_dumb_complete(
             A.CT_H.NAS.ALIAS.upper()
         )
 
         # step 5
         A.E.backup_notify_about_polibase_coping_db_dumb_start(
             A.CT_H.POLIBASE2.ALIAS.upper()
```

### Comparing `pih-plb_db-0.22/PolibaseDatabaseService/const.py` & `pih-plb_db-0.22.1/PolibaseDatabaseService/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "PolibaseDatabase"
 
 HOST = A.CT_H.POLIBASE
 
-VERSION: str = "0.22"
+VERSION: str = "0.22.1"
 
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     host=HOST.NAME,
     description="Polibase database service",
     commands=("create_polibase_database_backup",),
```

### Comparing `pih-plb_db-0.22/PolibaseDatabaseService/service.py` & `pih-plb_db-0.22.1/PolibaseDatabaseService/service.py`

 * *Files identical despite different names*

