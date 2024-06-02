# Comparing `tmp/core-system-utils-0.0.1.tar.gz` & `tmp/core-system-utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-system-utils-0.0.1.tar", last modified: Wed May 29 04:33:41 2024, max compression
+gzip compressed data, was "core-system-utils-0.0.2.tar", last modified: Sun Jun  2 05:11:02 2024, max compression
```

## Comparing `core-system-utils-0.0.1.tar` & `core-system-utils-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-05-29 04:33:41.432190 core-system-utils-0.0.1/
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      551 2024-05-29 04:33:41.432190 core-system-utils-0.0.1/PKG-INFO
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      176 2024-05-29 04:31:03.000000 core-system-utils-0.0.1/README.md
-drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-05-29 04:33:41.432190 core-system-utils-0.0.1/core_system_utils/
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      108 2024-05-29 04:29:58.000000 core-system-utils-0.0.1/core_system_utils/__init__.py
--rw-rw-r--   0 parzival  (1000) parzival  (1000)     4879 2024-05-29 04:28:49.000000 core-system-utils-0.0.1/core_system_utils/proc_handler.py
-drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-05-29 04:33:41.432190 core-system-utils-0.0.1/core_system_utils.egg-info/
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      551 2024-05-29 04:33:41.000000 core-system-utils-0.0.1/core_system_utils.egg-info/PKG-INFO
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      246 2024-05-29 04:33:41.000000 core-system-utils-0.0.1/core_system_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 parzival  (1000) parzival  (1000)        1 2024-05-29 04:33:41.000000 core-system-utils-0.0.1/core_system_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 parzival  (1000) parzival  (1000)       18 2024-05-29 04:33:41.000000 core-system-utils-0.0.1/core_system_utils.egg-info/top_level.txt
--rw-rw-r--   0 parzival  (1000) parzival  (1000)       38 2024-05-29 04:33:41.432190 core-system-utils-0.0.1/setup.cfg
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      719 2024-05-29 04:33:16.000000 core-system-utils-0.0.1/setup.py
+drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-06-02 05:11:02.894291 core-system-utils-0.0.2/
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      551 2024-06-02 05:11:02.894291 core-system-utils-0.0.2/PKG-INFO
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      176 2024-05-29 04:31:03.000000 core-system-utils-0.0.2/README.md
+drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-06-02 05:11:02.894291 core-system-utils-0.0.2/core_system_utils/
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      301 2024-06-02 05:05:36.000000 core-system-utils-0.0.2/core_system_utils/__init__.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)     1696 2024-06-02 03:47:21.000000 core-system-utils-0.0.2/core_system_utils/energy.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)     7114 2024-06-02 05:01:49.000000 core-system-utils-0.0.2/core_system_utils/filesystem.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)     5110 2024-06-02 03:57:10.000000 core-system-utils-0.0.2/core_system_utils/find_utils.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)     4841 2024-06-02 03:58:47.000000 core-system-utils-0.0.2/core_system_utils/proc_handler.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      795 2024-05-29 03:52:38.000000 core-system-utils-0.0.2/core_system_utils/shell.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      889 2024-06-02 05:02:50.000000 core-system-utils-0.0.2/core_system_utils/tester.py
+drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-06-02 05:11:02.894291 core-system-utils-0.0.2/core_system_utils.egg-info/
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      551 2024-06-02 05:11:02.000000 core-system-utils-0.0.2/core_system_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      393 2024-06-02 05:11:02.000000 core-system-utils-0.0.2/core_system_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)        1 2024-06-02 05:11:02.000000 core-system-utils-0.0.2/core_system_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)       18 2024-06-02 05:11:02.000000 core-system-utils-0.0.2/core_system_utils.egg-info/top_level.txt
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)       38 2024-06-02 05:11:02.894291 core-system-utils-0.0.2/setup.cfg
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      719 2024-06-02 05:10:59.000000 core-system-utils-0.0.2/setup.py
```

### Comparing `core-system-utils-0.0.1/PKG-INFO` & `core-system-utils-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-system-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: jacob.h.barrow
 Author-email: jacob.h.barrow@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `core-system-utils-0.0.1/core_system_utils/proc_handler.py` & `core-system-utils-0.0.2/core_system_utils/proc_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import List, Tuple, Optional, NoReturn, TypeAlias, Any, TypedDict
+from typing import List, Tuple, Optional, NoReturn, Any, TypedDict
 from pathlib import Path
 from abc import ABC, abstractmethod
 
-File_Contents: TypeAlias = str
-
 import re
 
+type File_Contents = str
+type SystemPtr = Tuple[str, SystemUtils]
+type Data = Tuple[Any]
+
 # Get the general idea of what the memory/cpu environment is... asynchroneous ops
 class ProcHandler(ABC):    
     
     @classmethod
     def read_file(cls, path_of_interest: Path) -> File_Contents:        
         with open(str(path_of_interest)) as reader:
             return reader.read().strip()              
@@ -80,17 +82,14 @@
         return result_json 
 
 class SystemUtils(ABC):
     @abstractmethod
     def get_data(self) -> None:
         raise NotImplementedError("Implement this!")
         
-SystemPtr: TypeAlias = Tuple[str, SystemUtils]
-Data: TypeAlias = Tuple[Any]
-        
 class CompositeSystem(SystemUtils):
     def __init__(self) -> None:
         self.system_ptrs: List[SystemPtr] = []
         
     def get_data(self) -> None:
         for name, system_ptr in self.system_ptrs:
             with system_ptr() as item:
```

### Comparing `core-system-utils-0.0.1/core_system_utils.egg-info/PKG-INFO` & `core-system-utils-0.0.2/core_system_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-system-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: jacob.h.barrow
 Author-email: jacob.h.barrow@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `core-system-utils-0.0.1/setup.py` & `core-system-utils-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.core import setup, Extension
 
 with open("README.md") as _file:
     long_description = _file.read()
 
 setuptools.setup(
         name= "core-system-utils",
-        version = "0.0.1",
+        version = "0.0.2",
         author = "jacob.h.barrow",
         author_email = "jacob.h.barrow@gmail.com",
         long_description = long_description,
         long_description_content_type = "text/markdown",
         url = "",
         packages=setuptools.find_packages(),
         install_requires = [
```

