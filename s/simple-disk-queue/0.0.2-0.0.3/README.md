# Comparing `tmp/simple_disk_queue-0.0.2.tar.gz` & `tmp/simple_disk_queue-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_disk_queue-0.0.2.tar", last modified: Mon Apr 29 21:13:03 2024, max compression
+gzip compressed data, was "simple_disk_queue-0.0.3.tar", last modified: Sun Jun  2 04:51:58 2024, max compression
```

## Comparing `simple_disk_queue-0.0.2.tar` & `simple_disk_queue-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2024-04-29 21:13:03.758756 simple_disk_queue-0.0.2/
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1051 2024-04-29 21:13:03.756756 simple_disk_queue-0.0.2/PKG-INFO
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      439 2024-04-29 21:12:11.000000 simple_disk_queue-0.0.2/README.md
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       38 2024-04-29 21:13:03.759756 simple_disk_queue-0.0.2/setup.cfg
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1115 2024-04-29 21:12:11.000000 simple_disk_queue-0.0.2/setup.py
-drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2024-04-29 21:13:03.728756 simple_disk_queue-0.0.2/simple_disk_queue/
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      303 2024-04-29 21:12:11.000000 simple_disk_queue-0.0.2/simple_disk_queue/__init__.py
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1897 2024-04-29 21:12:11.000000 simple_disk_queue-0.0.2/simple_disk_queue/_utils.py
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      422 2024-02-20 23:58:23.000000 simple_disk_queue-0.0.2/simple_disk_queue/config.py
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     6107 2024-04-29 21:12:12.000000 simple_disk_queue-0.0.2/simple_disk_queue/disk_queue.py
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      962 2024-04-29 21:12:12.000000 simple_disk_queue-0.0.2/simple_disk_queue/rw_lock.py
-drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2024-04-29 21:13:03.752756 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1051 2024-04-29 21:13:03.000000 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/PKG-INFO
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      369 2024-04-29 21:13:03.000000 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/SOURCES.txt
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)        1 2024-04-29 21:13:03.000000 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/dependency_links.txt
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       16 2024-04-29 21:13:03.000000 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/requires.txt
--rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       18 2024-04-29 21:13:03.000000 simple_disk_queue-0.0.2/simple_disk_queue.egg-info/top_level.txt
+drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2024-06-02 04:51:58.833109 simple_disk_queue-0.0.3/
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1273 2024-06-02 04:51:58.832109 simple_disk_queue-0.0.3/PKG-INFO
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      439 2024-04-29 21:12:11.000000 simple_disk_queue-0.0.3/README.md
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       38 2024-06-02 04:51:58.834109 simple_disk_queue-0.0.3/setup.cfg
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1115 2024-06-02 04:39:48.000000 simple_disk_queue-0.0.3/setup.py
+drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2024-06-02 04:51:58.805109 simple_disk_queue-0.0.3/simple_disk_queue/
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      304 2024-06-02 04:39:48.000000 simple_disk_queue-0.0.3/simple_disk_queue/__init__.py
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1890 2024-06-02 04:39:48.000000 simple_disk_queue-0.0.3/simple_disk_queue/_utils.py
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      421 2024-06-02 04:39:48.000000 simple_disk_queue-0.0.3/simple_disk_queue/config.py
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     6291 2024-06-02 04:39:48.000000 simple_disk_queue-0.0.3/simple_disk_queue/disk_queue.py
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1009 2024-06-02 04:39:48.000000 simple_disk_queue-0.0.3/simple_disk_queue/rw_lock.py
+drwxrwxr-x   0 zhenlin4 (1132177) zhenlin4 (1132177)        0 2024-06-02 04:51:58.827109 simple_disk_queue-0.0.3/simple_disk_queue.egg-info/
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)     1273 2024-06-02 04:51:58.000000 simple_disk_queue-0.0.3/simple_disk_queue.egg-info/PKG-INFO
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)      369 2024-06-02 04:51:58.000000 simple_disk_queue-0.0.3/simple_disk_queue.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)        1 2024-06-02 04:51:58.000000 simple_disk_queue-0.0.3/simple_disk_queue.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       16 2024-06-02 04:51:58.000000 simple_disk_queue-0.0.3/simple_disk_queue.egg-info/requires.txt
+-rw-rw-r--   0 zhenlin4 (1132177) zhenlin4 (1132177)       18 2024-06-02 04:51:58.000000 simple_disk_queue-0.0.3/simple_disk_queue.egg-info/top_level.txt
```

### Comparing `simple_disk_queue-0.0.2/PKG-INFO` & `simple_disk_queue-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_disk_queue
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create a disk-based queue
 Home-page: https://github.com/zlin7/python-simple_disk_queue
 Author: Zhen Lin
 Author-email: zhenlin4@illinois.edu
 License: MIT
 Description: 
         # Installation
@@ -15,15 +15,23 @@
         If you want to change it, see "Global Settings" below.
         
         # Quick Start
         
         An example can be found in `examples/test.py`.
         We can first call `init_queue()` to initialize the jobs, and then run `sdq.DiskQueue.run('test')` in different processes.
         
+        ## 0.0.3
+        ==================
+        1. bug fix
+        
         
+        ## 0.0.2
+        ==================
+        1. Use reference so we minimize the critical time
+        2. Added documentation and verbose mode
         
         
         ## 0.0.1
         ==================
         
         1. Core functionality: Add jobs to a queue and run jobs from a queue.
 Keywords: Job Scheduler,Disk-based Queue,Disk Queue Scheduler
```

### Comparing `simple_disk_queue-0.0.2/setup.py` & `simple_disk_queue-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md', encoding='utf-8') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='simple_disk_queue',
-    version='0.0.2',
+    version='0.0.3',
     description='Create a disk-based queue',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Zhen Lin',
     author_email='zhenlin4@illinois.edu',
```

### Comparing `simple_disk_queue-0.0.2/simple_disk_queue/_utils.py` & `simple_disk_queue-0.0.3/simple_disk_queue/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-""" Util functions
-"""
+"""Util functions"""
+
 import os
 import pickle
 
 from .rw_lock import FileLock
 
 PICKLE_PROTOCOL = 4
 
 
 def dump(obj, file, **kwargs):
-    """like pickle.dump but fix a default protocol for compatibility.
-    """
-    kwargs.setdefault('protocol', PICKLE_PROTOCOL)
+    """like pickle.dump but fix a default protocol for compatibility."""
+    kwargs.setdefault("protocol", PICKLE_PROTOCOL)
     return pickle.dump(obj, file, **kwargs)
 
 
 def to_pickle(obj, filepath, **kwargs):
-    """Like to_pickle in pandas, but avoids pandas dependency.
-    """
-    with open(filepath, 'wb') as fout:
+    """Like to_pickle in pandas, but avoids pandas dependency."""
+    with open(filepath, "wb") as fout:
         dump(obj, fout, **kwargs)
 
 
 def read_pickle(filepath, **kwargs):
-    """Like read_pickle in pandas, but avoids pandas dependency.
-    """
-    with open(filepath, 'rb') as fin:
+    """Like read_pickle in pandas, but avoids pandas dependency."""
+    with open(filepath, "rb") as fin:
         return pickle.load(fin, **kwargs)
 
+
 def locked_to_pickle(obj, filepath, **kwargs):
-    """Like to_pickle in pandas, but avoids pandas dependency and adds a lock.
-    """
+    """Like to_pickle in pandas, but avoids pandas dependency and adds a lock."""
     with FileLock(filepath):
         to_pickle(obj, filepath, **kwargs)
 
+
 def locked_read_pickle(filepath, **kwargs):
-    """Like read_pickle in pandas, but avoids pandas dependency and adds a lock.
-    """
+    """Like read_pickle in pandas, but avoids pandas dependency and adds a lock."""
     with FileLock(filepath):
         return read_pickle(filepath, **kwargs)
 
+
 def make_dir_if_necessary(dirname, max_depth=3):
     """Check if a directory exists. If not make it with lock.
     Will create nested directories (up to depth=max_depth).
 
     Args:
         dirname (_type_):
             Target directory.
         max_depth (int, optional):
             Maximum depth for nested creation.
             Defaults to 3.
     """
     if os.path.isdir(dirname):
         return
-    assert max_depth >= 0, f"Cannot make too many nested directories. Something could be wrong!, dirname={dirname}"
+    assert (
+        max_depth >= 0
+    ), f"Cannot make too many nested directories. Something could be wrong!, dirname={dirname}"
     if not os.path.isdir(os.path.dirname(dirname)):
         make_dir_if_necessary(os.path.dirname(dirname), max_depth - 1)
     fl = FileLock(dirname)
     with fl:
         print(f"{dirname} does not exist. Creating it for persist_to_disk")
         os.makedirs(dirname)
     return
```

### Comparing `simple_disk_queue-0.0.2/simple_disk_queue/disk_queue.py` & `simple_disk_queue-0.0.3/simple_disk_queue/disk_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-
-
-
 import hashlib
 import importlib
 import os
+import random
 from collections import deque
 from typing import Any, Callable, List, Optional, Tuple, Union
 
 from . import _utils
 from .config import Config, get_default_config
 from .rw_lock import FileLock, Timeout
 
 
-def _hash(x:int):
+def _hash(x: int):
     return int(hashlib.md5(str(x).encode()).hexdigest(), 16)
 
+
 class DiskQueue:
-    def __init__(self, id:str, config:Config=None, overwrite:bool=False, verbose:bool=False) -> None:
+    def __init__(
+        self,
+        id: str,
+        config: Config = None,
+        overwrite: bool = False,
+        verbose: bool = False,
+    ) -> None:
         """Initialize the DiskQueue object.
 
         :param id: The id of the queue. This is used to create the file name and to identify the queue.
         :type id: str
         :param config: Configurations , defaults to None.
             Right now it only specifies where all queues are stored, and there is no need to set it.
         :type config: Config, optional
@@ -79,16 +84,16 @@
             curr_queue = _utils.read_pickle(self.queue_file)
             if len(curr_queue):
                 job = curr_queue.popleft()
                 _utils.to_pickle(curr_queue, self.queue_file)
         if job is None:
             return None
         func_str, args, kwargs = job
-        _module = importlib.import_module('.'.join(func_str.split('.')[:-1]))
-        func = getattr(_module, func_str.split('.')[-1])
+        _module = importlib.import_module(".".join(func_str.split(".")[:-1]))
+        func = getattr(_module, func_str.split(".")[-1])
         return (func, args, kwargs)
 
     def peek_task(self):
         """Peek the next task from the queue.
 
         :return: (func_str, args, kwargs), where func_str is only a reference to the function.
         :rtype: Tuple[str, Tuple, dict]
@@ -102,15 +107,17 @@
             curr_queue = _utils.read_pickle(self.queue_file)
             curr_queue = list(curr_queue)
             random.shuffle(curr_queue)
             curr_queue = deque(curr_queue)
             _utils.to_pickle(curr_queue, self.queue_file)
 
     @classmethod
-    def run(cls, id:str, max_attempts:int=30, verbose=False, raise_error=False) -> None:
+    def run(
+        cls, id: str, max_attempts: int = 30, verbose=False, raise_error=False
+    ) -> None:
         """Run a queue with the given id.
 
         :param id: id of the queue to run
         :type id: str
         :param max_attempts: Maximum number of attempts to try, defaults to 30
         :type max_attempts: int, optional
         :param verbose: Verbose mode or not, defaults to False
@@ -125,41 +132,45 @@
         while failed_cnt < max_attempts:
             job = queue.pop_task()
             if job is None:
                 break
             func, args, kwargs = job
             try:
                 if verbose:
-                    print(f"Running job {func.__module__}.{func.__name__} {args} {kwargs}")
+                    print(
+                        f"Running job {func.__module__}.{func.__name__} {args} {kwargs}"
+                    )
                 func(*args, **kwargs)
             except KeyboardInterrupt as err:
                 queue.add_task(func, *args, **kwargs)
                 raise err
             except Exception as err:
                 if raise_error:
                     raise err
                 failed_cnt += 1
                 if verbose:
-                    print(f"Job {func.__module__}.{func.__name__} {args} {kwargs} failed with error {err}")
+                    print(
+                        f"Job {func.__module__}.{func.__name__} {args} {kwargs} failed with error {err}"
+                    )
                 queue.add_task(func, *args, **kwargs)
 
     @classmethod
-    def exists(cls, id:str):
+    def exists(cls, id: str):
         return os.path.isfile(cls.queue_file(id))
 
     @classmethod
-    def queue_file(cls, id:str):
+    def queue_file(cls, id: str):
         config = get_default_config()
         return os.path.join(config.get_queue_location(), f"{id}.pkl")
 
     @classmethod
-    def clear(cls, id:str):
+    def clear(cls, id: str):
         """Clear the queue with the given id.
 
         :param id: id of the queue to clear
         :type id: str
         """
         queue_file = cls.queue_file(id)
         if not cls.exists(id):
             return
         with FileLock(queue_file):
-            os.remove(queue_file)
+            os.remove(queue_file)
```

### Comparing `simple_disk_queue-0.0.2/simple_disk_queue/rw_lock.py` & `simple_disk_queue-0.0.3/simple_disk_queue/rw_lock.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from filelock import FileLock as RawFileLock
 from filelock import Timeout
 
 assert Timeout is not None
 
 
+# TODO: This is still not a read-write lock but just a lock
 class FileLock(object):
-    """A wrapper for filelock.FileLock
-    """
+    """A wrapper for filelock.FileLock"""
 
     def __init__(self, protected_file_path, timeout=5, verbose=False):
-        """ Prepare the file locker. Specify the file to lock and optionally
-                the maximum timeout and the delay between each attempt to lock.
+        """Prepare the file locker. Specify the file to lock and optionally
+        the maximum timeout and the delay between each attempt to lock.
         """
         self.lock_path = protected_file_path + ".lock"
         self.lock = RawFileLock(self.lock_path, timeout=timeout)
         self.verbose = verbose
 
     def __enter__(self):
         if self.verbose:
@@ -25,8 +25,8 @@
 
     def __exit__(self, *args, **kwargs):
         if self.verbose:
             print(f"Critical time: {time.time() - self._start_time:.2f}s")
         return self.lock.__exit__(*args, **kwargs)
 
     def __del__(self):
-        return self.lock.__del__()
+        return self.lock.__del__()
```

### Comparing `simple_disk_queue-0.0.2/simple_disk_queue.egg-info/PKG-INFO` & `simple_disk_queue-0.0.3/simple_disk_queue.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-disk-queue
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create a disk-based queue
 Home-page: https://github.com/zlin7/python-simple_disk_queue
 Author: Zhen Lin
 Author-email: zhenlin4@illinois.edu
 License: MIT
 Description: 
         # Installation
@@ -15,15 +15,23 @@
         If you want to change it, see "Global Settings" below.
         
         # Quick Start
         
         An example can be found in `examples/test.py`.
         We can first call `init_queue()` to initialize the jobs, and then run `sdq.DiskQueue.run('test')` in different processes.
         
+        ## 0.0.3
+        ==================
+        1. bug fix
+        
         
+        ## 0.0.2
+        ==================
+        1. Use reference so we minimize the critical time
+        2. Added documentation and verbose mode
         
         
         ## 0.0.1
         ==================
         
         1. Core functionality: Add jobs to a queue and run jobs from a queue.
 Keywords: Job Scheduler,Disk-based Queue,Disk Queue Scheduler
```

