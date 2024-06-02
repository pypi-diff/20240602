# Comparing `tmp/ervdetective-1.0.6.tar.gz` & `tmp/ervdetective-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ervdetective-1.0.6.tar", last modified: Mon Apr 29 02:53:55 2024, max compression
+gzip compressed data, was "dist\ervdetective-1.0.7.tar", last modified: Sun Jun  2 09:15:22 2024, max compression
```

## Comparing `ervdetective-1.0.6.tar` & `ervdetective-1.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 02:53:55.000000 ervdetective-1.0.6/
--rw-rw-rw-   0        0        0    26526 2023-03-06 15:44:50.000000 ervdetective-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       50 2023-08-10 13:16:08.000000 ervdetective-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5707 2024-04-29 02:53:55.000000 ervdetective-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4449 2024-04-29 02:52:53.000000 ervdetective-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 02:53:55.000000 ervdetective-1.0.6/ervdetective/
-drwxrwxrwx   0        0        0        0 2024-04-29 02:53:55.000000 ervdetective-1.0.6/ervdetective/Internal_database/
-drwxrwxrwx   0        0        0        0 2024-04-29 02:53:55.000000 ervdetective-1.0.6/ervdetective/Internal_database/ERVprofiles/
--rw-rw-rw-   0        0        0   915480 2024-04-02 12:09:12.000000 ervdetective-1.0.6/ervdetective/Internal_database/ERVprofiles/ERVprofile.zip
-drwxrwxrwx   0        0        0        0 2024-04-29 02:53:55.000000 ervdetective-1.0.6/ervdetective/Internal_database/probe/
--rw-rw-rw-   0        0        0    68038 2024-04-29 02:26:23.000000 ervdetective-1.0.6/ervdetective/Internal_database/probe/ENV_probe.fasta
--rw-rw-rw-   0        0        0    42001 2024-02-27 11:42:33.000000 ervdetective-1.0.6/ervdetective/Internal_database/probe/GAG_probe.fasta
--rw-rw-rw-   0        0        0    18175 2024-02-27 11:50:30.000000 ervdetective-1.0.6/ervdetective/Internal_database/probe/RT_probe.fasta
--rw-rw-rw-   0        0        0      196 2023-08-22 02:57:04.000000 ervdetective-1.0.6/ervdetective/__init__.py
--rw-rw-rw-   0        0        0    13082 2024-04-29 02:12:05.000000 ervdetective-1.0.6/ervdetective/annotion_ervs.py
--rw-rw-rw-   0        0        0     8127 2024-04-05 02:50:41.000000 ervdetective-1.0.6/ervdetective/get_ervs.py
--rw-rw-rw-   0        0        0     9437 2024-04-29 02:11:33.000000 ervdetective-1.0.6/ervdetective/get_flank.py
--rw-rw-rw-   0        0        0    30750 2024-04-29 02:52:32.000000 ervdetective-1.0.6/ervdetective/main.py
--rw-rw-rw-   0        0        0    27346 2024-04-29 02:06:27.000000 ervdetective-1.0.6/ervdetective/map_genome.py
--rw-rw-rw-   0        0        0    11658 2024-04-02 11:21:18.000000 ervdetective-1.0.6/ervdetective/public_function.py
--rw-rw-rw-   0        0        0     8400 2024-04-29 02:10:09.000000 ervdetective-1.0.6/ervdetective/seqs_for_hmmer.py
--rw-rw-rw-   0        0        0     6194 2024-04-29 02:09:00.000000 ervdetective-1.0.6/ervdetective/simplify_gff3.py
--rw-rw-rw-   0        0        0     6806 2024-04-29 02:09:20.000000 ervdetective-1.0.6/ervdetective/simplify_hmmer.py
-drwxrwxrwx   0        0        0        0 2024-04-29 02:53:55.000000 ervdetective-1.0.6/ervdetective.egg-info/
--rw-rw-rw-   0        0        0     5707 2024-04-29 02:53:55.000000 ervdetective-1.0.6/ervdetective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2024-04-29 02:53:55.000000 ervdetective-1.0.6/ervdetective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 02:53:55.000000 ervdetective-1.0.6/ervdetective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-29 02:53:55.000000 ervdetective-1.0.6/ervdetective.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-04-29 02:53:55.000000 ervdetective-1.0.6/ervdetective.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 02:53:55.000000 ervdetective-1.0.6/ervdetective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 02:53:55.000000 ervdetective-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1619 2024-04-29 02:52:40.000000 ervdetective-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 09:15:22.000000 ervdetective-1.0.7/
+-rw-rw-rw-   0        0        0    26526 2023-03-06 15:44:50.000000 ervdetective-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-08-10 13:16:08.000000 ervdetective-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5915 2024-06-02 09:15:22.000000 ervdetective-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4449 2024-04-29 02:52:53.000000 ervdetective-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 09:15:22.000000 ervdetective-1.0.7/ervdetective/
+drwxrwxrwx   0        0        0        0 2024-06-02 09:15:22.000000 ervdetective-1.0.7/ervdetective/Internal_database/
+drwxrwxrwx   0        0        0        0 2024-06-02 09:15:22.000000 ervdetective-1.0.7/ervdetective/Internal_database/ERVprofiles/
+-rw-rw-rw-   0        0        0   915480 2024-04-02 12:09:12.000000 ervdetective-1.0.7/ervdetective/Internal_database/ERVprofiles/ERVprofile.zip
+drwxrwxrwx   0        0        0        0 2024-06-02 09:15:22.000000 ervdetective-1.0.7/ervdetective/Internal_database/probe/
+-rw-rw-rw-   0        0        0    68038 2024-04-29 02:26:23.000000 ervdetective-1.0.7/ervdetective/Internal_database/probe/ENV_probe.fasta
+-rw-rw-rw-   0        0        0    42001 2024-02-27 11:42:33.000000 ervdetective-1.0.7/ervdetective/Internal_database/probe/GAG_probe.fasta
+-rw-rw-rw-   0        0        0    18175 2024-02-27 11:50:30.000000 ervdetective-1.0.7/ervdetective/Internal_database/probe/RT_probe.fasta
+-rw-rw-rw-   0        0        0      196 2023-08-22 02:57:04.000000 ervdetective-1.0.7/ervdetective/__init__.py
+-rw-rw-rw-   0        0        0    13082 2024-04-29 02:12:05.000000 ervdetective-1.0.7/ervdetective/annotion_ervs.py
+-rw-rw-rw-   0        0        0     8127 2024-04-05 02:50:41.000000 ervdetective-1.0.7/ervdetective/get_ervs.py
+-rw-rw-rw-   0        0        0     9437 2024-04-29 02:11:33.000000 ervdetective-1.0.7/ervdetective/get_flank.py
+-rw-rw-rw-   0        0        0    30750 2024-06-02 09:14:17.000000 ervdetective-1.0.7/ervdetective/main.py
+-rw-rw-rw-   0        0        0    27346 2024-04-29 02:06:27.000000 ervdetective-1.0.7/ervdetective/map_genome.py
+-rw-rw-rw-   0        0        0    11658 2024-04-02 11:21:18.000000 ervdetective-1.0.7/ervdetective/public_function.py
+-rw-rw-rw-   0        0        0     8400 2024-04-29 02:10:09.000000 ervdetective-1.0.7/ervdetective/seqs_for_hmmer.py
+-rw-rw-rw-   0        0        0     6194 2024-04-29 02:09:00.000000 ervdetective-1.0.7/ervdetective/simplify_gff3.py
+-rw-rw-rw-   0        0        0     6806 2024-04-29 02:09:20.000000 ervdetective-1.0.7/ervdetective/simplify_hmmer.py
+drwxrwxrwx   0        0        0        0 2024-06-02 09:15:22.000000 ervdetective-1.0.7/ervdetective.egg-info/
+-rw-rw-rw-   0        0        0     5915 2024-06-02 09:15:21.000000 ervdetective-1.0.7/ervdetective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2024-06-02 09:15:21.000000 ervdetective-1.0.7/ervdetective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 09:15:21.000000 ervdetective-1.0.7/ervdetective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-06-02 09:15:21.000000 ervdetective-1.0.7/ervdetective.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-06-02 09:15:21.000000 ervdetective-1.0.7/ervdetective.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 09:15:21.000000 ervdetective-1.0.7/ervdetective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 09:15:22.000000 ervdetective-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1823 2024-06-02 09:13:28.000000 ervdetective-1.0.7/setup.py
```

### Comparing `ervdetective-1.0.6/LICENSE` & `ervdetective-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/PKG-INFO` & `ervdetective-1.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ervdetective
-Version: 1.0.6
+Version: 1.0.7
 Summary: An efficient pipeline for identification and annotation of endogenous retroviruses (ERVs)
 Home-page: https://github.com/ZhijianZhou01/ervdetective
 Author: Zhi-Jian Zhou
 Author-email: zjzhou@hnu.edu.cn
 Keywords: endogenous retroviruses,virus,evolution
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -14,14 +14,18 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ERVdetective: an efficient pipeline for identification and annotation of endogenous retroviruses (ERVs)
```

### Comparing `ervdetective-1.0.6/README.md` & `ervdetective-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/Internal_database/ERVprofiles/ERVprofile.zip` & `ervdetective-1.0.7/ervdetective/Internal_database/ERVprofiles/ERVprofile.zip`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/Internal_database/probe/ENV_probe.fasta` & `ervdetective-1.0.7/ervdetective/Internal_database/probe/ENV_probe.fasta`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/Internal_database/probe/GAG_probe.fasta` & `ervdetective-1.0.7/ervdetective/Internal_database/probe/GAG_probe.fasta`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/Internal_database/probe/RT_probe.fasta` & `ervdetective-1.0.7/ervdetective/Internal_database/probe/RT_probe.fasta`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/annotion_ervs.py` & `ervdetective-1.0.7/ervdetective/annotion_ervs.py`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/get_ervs.py` & `ervdetective-1.0.7/ervdetective/get_ervs.py`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/get_flank.py` & `ervdetective-1.0.7/ervdetective/get_flank.py`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/main.py` & `ervdetective-1.0.7/ervdetective/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
 
     print("\n" + "-------------------------------------------------")
 
     print("  Name: Endogenous retroviruses detective (ERVdetective)")
 
     print("  Description: An efficient pipeline for identification and annotation of endogenous retroviruses.")
 
-    print("  Version: 1.0.6 (2024-04-29)")
+    print("  Version: 1.0.7 (2024-04-30)")
 
     print("  Author: Zhi-Jian Zhou")
 
     print("-------------------------------------------------" + "\n")
 
 
     myargs = parameter()
```

### Comparing `ervdetective-1.0.6/ervdetective/map_genome.py` & `ervdetective-1.0.7/ervdetective/map_genome.py`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/public_function.py` & `ervdetective-1.0.7/ervdetective/public_function.py`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/seqs_for_hmmer.py` & `ervdetective-1.0.7/ervdetective/seqs_for_hmmer.py`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/simplify_gff3.py` & `ervdetective-1.0.7/ervdetective/simplify_gff3.py`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective/simplify_hmmer.py` & `ervdetective-1.0.7/ervdetective/simplify_hmmer.py`

 * *Files identical despite different names*

### Comparing `ervdetective-1.0.6/ervdetective.egg-info/PKG-INFO` & `ervdetective-1.0.7/ervdetective.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ervdetective
-Version: 1.0.6
+Version: 1.0.7
 Summary: An efficient pipeline for identification and annotation of endogenous retroviruses (ERVs)
 Home-page: https://github.com/ZhijianZhou01/ervdetective
 Author: Zhi-Jian Zhou
 Author-email: zjzhou@hnu.edu.cn
 Keywords: endogenous retroviruses,virus,evolution
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -14,14 +14,18 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ERVdetective: an efficient pipeline for identification and annotation of endogenous retroviruses (ERVs)
```

### Comparing `ervdetective-1.0.6/ervdetective.egg-info/SOURCES.txt` & `ervdetective-1.0.7/ervdetective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

