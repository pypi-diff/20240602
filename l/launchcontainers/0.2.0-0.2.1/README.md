# Comparing `tmp/launchcontainers-0.2.0.tar.gz` & `tmp/launchcontainers-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchcontainers-0.2.0.tar", max compression
+gzip compressed data, was "launchcontainers-0.2.1.tar", max compression
```

## Comparing `launchcontainers-0.2.0.tar` & `launchcontainers-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1268 2024-03-13 13:14:08.835946 launchcontainers-0.2.0/LICENSE
--rwxr-xr-x   0        0        0     1517 2024-05-28 10:11:57.442938 launchcontainers-0.2.0/README.md
--rwxr-xr-x   0        0        0     1435 2024-05-28 10:12:28.089313 launchcontainers-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0      815 2024-03-13 13:14:10.126085 launchcontainers-0.2.0/src/__init__.py
--rwxr-xr-x   0        0        0    21045 2024-05-28 10:11:57.748009 launchcontainers-0.2.0/src/launch.py
--rwxr-xr-x   0        0        0      814 2024-03-13 13:14:10.217982 launchcontainers-0.2.0/src/prepare_inputs/__init__.py
--rwxr-xr-x   0        0        0    23960 2024-03-13 13:14:10.286713 launchcontainers-0.2.0/src/prepare_inputs/_version.py
--rwxr-xr-x   0        0        0     9332 2024-03-13 13:14:10.332443 launchcontainers-0.2.0/src/prepare_inputs/check_parser.py
--rwxr-xr-x   0        0        0     7166 2024-05-28 10:11:57.783613 launchcontainers-0.2.0/src/prepare_inputs/dask_scheduler_config.py
--rwxr-xr-x   0        0        0    17635 2024-05-28 10:11:58.459389 launchcontainers-0.2.0/src/prepare_inputs/prepare.py
--rwxr-xr-x   0        0        0    33548 2024-05-28 10:11:58.518098 launchcontainers-0.2.0/src/prepare_inputs/prepare_dwi.py
--rwxr-xr-x   0        0        0      620 2024-03-13 13:14:10.452740 launchcontainers-0.2.0/src/prepare_inputs/prepare_prf.py
--rwxr-xr-x   0        0        0     9275 2024-05-28 10:11:59.148485 launchcontainers-0.2.0/src/prepare_inputs/utils.py
--rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 launchcontainers-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1268 2024-05-30 22:14:45.340027 launchcontainers-0.2.1/LICENSE
+-rwxr-xr-x   0        0        0     1517 2024-05-30 22:14:45.340027 launchcontainers-0.2.1/README.md
+-rwxr-xr-x   0        0        0     1435 2024-06-02 14:21:40.023575 launchcontainers-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0      815 2024-05-30 22:14:45.345027 launchcontainers-0.2.1/src/__init__.py
+-rwxr-xr-x   0        0        0    21155 2024-06-02 11:50:18.482486 launchcontainers-0.2.1/src/launch.py
+-rwxr-xr-x   0        0        0      814 2024-05-30 22:14:45.346027 launchcontainers-0.2.1/src/prepare_inputs/__init__.py
+-rwxr-xr-x   0        0        0    23960 2024-05-30 22:14:45.346027 launchcontainers-0.2.1/src/prepare_inputs/_version.py
+-rwxr-xr-x   0        0        0     9332 2024-05-30 22:14:45.346027 launchcontainers-0.2.1/src/prepare_inputs/check_parser.py
+-rwxr-xr-x   0        0        0     7166 2024-05-30 22:14:45.346027 launchcontainers-0.2.1/src/prepare_inputs/dask_scheduler_config.py
+-rwxr-xr-x   0        0        0    17635 2024-05-30 22:14:45.346027 launchcontainers-0.2.1/src/prepare_inputs/prepare.py
+-rwxr-xr-x   0        0        0    33548 2024-05-30 22:14:45.346027 launchcontainers-0.2.1/src/prepare_inputs/prepare_dwi.py
+-rwxr-xr-x   0        0        0      620 2024-05-30 22:14:45.346027 launchcontainers-0.2.1/src/prepare_inputs/prepare_prf.py
+-rwxr-xr-x   0        0        0     9275 2024-05-30 22:14:45.346027 launchcontainers-0.2.1/src/prepare_inputs/utils.py
+-rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 launchcontainers-0.2.1/PKG-INFO
```

### Comparing `launchcontainers-0.2.0/LICENSE` & `launchcontainers-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.2.0/README.md` & `launchcontainers-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.2.0/pyproject.toml` & `launchcontainers-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "launchcontainers"
-version = "0.2.0"
+version = "0.2.1"
 description = "Launch Containers Package"
 authors = [ "BCBL", 
             "Garikoitz Lerma-Usabiaga",
             "Leandro Lecca",
             "Mengxing Liu",
             "Yongning Lei"
             ]
```

### Comparing `launchcontainers-0.2.0/src/__init__.py` & `launchcontainers-0.2.1/src/__init__.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.2.0/src/launch.py` & `launchcontainers-0.2.1/src/launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 """
 import os
 import subprocess as sp
+from subprocess import Popen
 import numpy as np
 import logging
 
 # modules in lc
 
 from bids import BIDSLayout
 from dask.distributed import progress
@@ -58,14 +59,15 @@
     homedir = os.path.join(basedir, "singularity_home")
     container = lc_config["general"]["container"]
     host = lc_config["general"]["host"]
     containerdir = lc_config["general"]["containerdir"]
 
     # Information relevant to the host and container
     jobqueue_config = lc_config["host_options"][host]
+    launch_mode = jobqueue_config["launch_mode"]
     version = lc_config["container_specific"][container]["version"]
     use_module = jobqueue_config["use_module"]
     bind_options = jobqueue_config["bind_options"]
 
     # Location of the Singularity Image File (.sif)
     container_name = os.path.join(containerdir, f"{container}_{version}.sif")
     # Define the directory and the file name to output the log of each subject
@@ -237,29 +239,29 @@
             "\n"
             + f"the DWI PIPELINE command is not assigned, please check your config.yaml[general][host] session\n"
         )
         raise ValueError("cmd is not defined, aborting")
 
     # GLU: I don't think this is right, run is done below, I will make it work just for local but not in here,
     #      it is good that this function just creates the cmd, I would keep it like that
-    if run_lc:
-        return(sp.run(cmd, shell = True))
+    if (run_lc and host != "local") or (run_lc and host == "local" and launch_mode == "dask_worker"):
+       return(sp.run(cmd, shell = True))
     else:
         return cmd
     #     sp.run(cmd, shell=True)
     #return cmd
 
 
 # %% the launchcontainer
 def launchcontainer(
     dir_analysis,
     lc_config,
     sub_ses_list,
     parser_namespace,
-    path_to_analysis_container_specific_config,
+    path_to_analysis_container_specific_config
 ):
     """
     This function launches containers generically in different Docker/Singularity HPCs
     This function is going to assume that all files are where they need to be.
 
     Args:
         dir_analysis (str): _description_
@@ -286,15 +288,14 @@
 
     lc_configs = []
     subs = []
     sess = []
     dir_analysiss = []
     paths_to_analysis_config_json = []
     run_lcs = []
-
     # PREPARATION mode
     if not run_lc:
         logger.critical(
             f"\nlaunchcontainers.py was run in PREPARATION mode (without option --run_lc)\n"
             f"Please check that: \n"
             f"    (1) launchcontainers.py prepared the input data properly\n"
             f"    (2) the command created for each subject is properly formed\n"
@@ -374,17 +375,17 @@
 
     if run_lc and host == "local":
         if launch_mode == "parallel":
             logger.critical(
                 f"\nLocally launching {len(commands)} jobs in parallel, check "
                 f"your server's memory, some jobs might fail\n"
             )
-            for i, cmd in enumerate(commands):
-                logger.critical(f"LAUNCHING JOB {1}/{len(commands)}:\n{cmd}\n")
-                sp.run(cmd, shell=True)
+            procs = [ Popen(i, shell=True) for i in commands ]
+            for p in procs:
+                p.wait()
         elif launch_mode == "dask_worker":
             logger.critical(
                 f"\nLocally launching {len(commands)} jobs with dask-worker, "
                 f" keep an eye on your server's memory\n"
             )
             run_dask(
                 jobqueue_config, 
@@ -523,14 +524,14 @@
 
     # Run mode
     launchcontainer(
         dir_analysis,
         lc_config,
         sub_ses_list,
         parser_namespace,
-        path_to_analysis_container_specific_config,
+        path_to_analysis_container_specific_config
     )
 
 
 # #%%
 if __name__ == "__main__":
     main()
```

### Comparing `launchcontainers-0.2.0/src/prepare_inputs/__init__.py` & `launchcontainers-0.2.1/src/prepare_inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.2.0/src/prepare_inputs/_version.py` & `launchcontainers-0.2.1/src/prepare_inputs/_version.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.2.0/src/prepare_inputs/check_parser.py` & `launchcontainers-0.2.1/src/prepare_inputs/check_parser.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.2.0/src/prepare_inputs/dask_scheduler_config.py` & `launchcontainers-0.2.1/src/prepare_inputs/dask_scheduler_config.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.2.0/src/prepare_inputs/prepare.py` & `launchcontainers-0.2.1/src/prepare_inputs/prepare.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.2.0/src/prepare_inputs/prepare_dwi.py` & `launchcontainers-0.2.1/src/prepare_inputs/prepare_dwi.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.2.0/src/prepare_inputs/prepare_prf.py` & `launchcontainers-0.2.1/src/prepare_inputs/prepare_prf.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.2.0/src/prepare_inputs/utils.py` & `launchcontainers-0.2.1/src/prepare_inputs/utils.py`

 * *Files identical despite different names*

### Comparing `launchcontainers-0.2.0/PKG-INFO` & `launchcontainers-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchcontainers
-Version: 0.2.0
+Version: 0.2.1
 Summary: Launch Containers Package
 Home-page: https://github.com/garikoitz/launchcontainers
 License: MIT
 Keywords: HPC,MRI,RTP2,DWI,dMRI
 Author: BCBL
 Maintainer: Garikoitz Lerma-Usabiaga
 Requires-Python: >=3.10,<3.11
```

