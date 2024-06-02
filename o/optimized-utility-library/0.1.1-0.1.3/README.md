# Comparing `tmp/optimized-utility-library-0.1.1.tar.gz` & `tmp/optimized-utility-library-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimized-utility-library-0.1.1.tar", last modified: Sat Jun  1 13:40:52 2024, max compression
+gzip compressed data, was "optimized-utility-library-0.1.3.tar", last modified: Sun Jun  2 17:40:28 2024, max compression
```

## Comparing `optimized-utility-library-0.1.1.tar` & `optimized-utility-library-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:40:52.647033 optimized-utility-library-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-06-01 13:40:52.647033 optimized-utility-library-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:40:52.647033 optimized-utility-library-0.1.1/optimized_utility_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-06-01 13:40:52.000000 optimized-utility-library-0.1.1/optimized_utility_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-06-01 13:40:52.000000 optimized-utility-library-0.1.1/optimized_utility_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 13:40:52.000000 optimized-utility-library-0.1.1/optimized_utility_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-01 13:40:52.000000 optimized-utility-library-0.1.1/optimized_utility_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 13:40:52.000000 optimized-utility-library-0.1.1/optimized_utility_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 13:40:52.647033 optimized-utility-library-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:40:52.647033 optimized-utility-library-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/tests/test_directory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/tests/test_directory_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/tests/test_file_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/tests/test_image_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/tests/test_json_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/tests/test_llm_image_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:40:52.647033 optimized-utility-library-0.1.1/utility_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/utility_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:40:52.647033 optimized-utility-library-0.1.1/utility_lib/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/utility_lib/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/utility_lib/common/directory_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/utility_lib/common/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/utility_lib/common/image_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/utility_lib/common/json_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:40:52.647033 optimized-utility-library-0.1.1/utility_lib/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/utility_lib/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-06-01 13:40:40.000000 optimized-utility-library-0.1.1/utility_lib/llm/llm_image_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:40:28.309497 optimized-utility-library-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-06-02 17:40:28.309497 optimized-utility-library-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:40:28.305498 optimized-utility-library-0.1.3/optimized_utility_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-06-02 17:40:28.000000 optimized-utility-library-0.1.3/optimized_utility_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-06-02 17:40:28.000000 optimized-utility-library-0.1.3/optimized_utility_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:40:28.000000 optimized-utility-library-0.1.3/optimized_utility_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 17:40:28.000000 optimized-utility-library-0.1.3/optimized_utility_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 17:40:28.000000 optimized-utility-library-0.1.3/optimized_utility_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:40:28.309497 optimized-utility-library-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:40:28.305498 optimized-utility-library-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/tests/test_directory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/tests/test_file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/tests/test_image_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/tests/test_json_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/tests/test_llm_image_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:40:28.305498 optimized-utility-library-0.1.3/utility_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/utility_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:40:28.309497 optimized-utility-library-0.1.3/utility_lib/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/utility_lib/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/utility_lib/common/directory_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/utility_lib/common/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/utility_lib/common/image_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/utility_lib/common/json_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:40:28.309497 optimized-utility-library-0.1.3/utility_lib/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/utility_lib/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-06-02 17:40:21.000000 optimized-utility-library-0.1.3/utility_lib/llm/llm_image_operation.py
```

### Comparing `optimized-utility-library-0.1.1/optimized_utility_library.egg-info/SOURCES.txt` & `optimized-utility-library-0.1.3/optimized_utility_library.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 optimized_utility_library.egg-info/PKG-INFO
 optimized_utility_library.egg-info/SOURCES.txt
 optimized_utility_library.egg-info/dependency_links.txt
 optimized_utility_library.egg-info/requires.txt
 optimized_utility_library.egg-info/top_level.txt
 tests/__init__.py
 tests/test_directory_monitor.py
-tests/test_directory_operations.py
 tests/test_file_operations.py
 tests/test_image_operations.py
 tests/test_json_operations.py
 tests/test_llm_image_operations.py
 utility_lib/__init__.py
 utility_lib/common/__init__.py
 utility_lib/common/directory_operations.py
```

### Comparing `optimized-utility-library-0.1.1/setup.py` & `optimized-utility-library-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='optimized-utility-library',
-    version='0.1.1',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'pillow',
         'ujson',
         'matplotlib',
         'setuptools',
         'opencv-python',
```

### Comparing `optimized-utility-library-0.1.1/tests/test_file_operations.py` & `optimized-utility-library-0.1.3/tests/test_file_operations.py`

 * *Files identical despite different names*

### Comparing `optimized-utility-library-0.1.1/tests/test_image_operations.py` & `optimized-utility-library-0.1.3/tests/test_image_operations.py`

 * *Files identical despite different names*

### Comparing `optimized-utility-library-0.1.1/tests/test_json_operations.py` & `optimized-utility-library-0.1.3/tests/test_json_operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,103 @@
 import json
 import math
 import time
-
 import pytest
 import ujson
 
 from utility_lib.common.json_operations import (
     get_json_key,
     load_json,
     save_json,
     update_json_key,
 )
 
+
 @pytest.fixture
 def json_test_file(tmp_path):
     file_path = tmp_path / "test.json"
-    content = {"key": "value"}
+    content = {
+        "key": "value",
+        "nested": {
+            "key1": "value1",
+            "key2": [i for i in range(10000)],
+            "key3": {
+                "subkey1": "subvalue1",
+                "subkey2": [f"item{i}" for i in range(10000)]
+            }
+        },
+        "large_array": [{"id": i, "name": f"name{i}"} for i in range(10000)]
+    }
     save_json(str(file_path), content)
     return str(file_path)
 
 
+def load_json_without_cache(json_path):
+    try:
+        with open(json_path, 'r') as file:
+            return json.load(file)
+    except Exception as e:
+        print(f"Failed to load JSON from {json_path}: {str(e)}")
+        return None
+
+
 def test_load_json(tmp_path):
     file_path = tmp_path / "test.json"
     content = {"key": "value"}
     file_path.write_text(json.dumps(content))
     loaded_content = load_json(str(file_path))
     assert loaded_content == content
 
+
 def test_load_invalid_json(tmp_path):
     file_path = tmp_path / "test.json"
     file_path.write_text("{invalid json}")
     loaded_content = load_json(str(file_path))
     assert loaded_content is None
 
+
 def test_save_json(tmp_path):
     file_path = tmp_path / "test.json"
     content = {"key": "value"}
     assert save_json(str(file_path), content)
     loaded_content = json.loads(file_path.read_text())
     assert loaded_content == content
 
+
 def test_save_invalid_json(tmp_path):
     file_path = tmp_path / "test.json"
     content = {"key": float("nan")}
     save_json(str(file_path), content)
     loaded_content = ujson.load(file_path.open())
     assert math.isnan(loaded_content["key"])
 
+
 def test_get_json_key():
     json_data = {"key1": "value1", "key2": "value2"}
     assert get_json_key(json_data, "key1") == "value1"
     assert get_json_key(json_data, "key3", "default") == "default"
 
+
 def test_get_json_key_with_default():
     json_data = {"key1": "value1"}
     assert get_json_key(json_data, "key2", "default") == "default"
 
+
 def test_update_json_key():
-    json_data = {"key1":"value1", "key2": "value2"}
+    json_data = {"key1": "value1", "key2": "value2"}
     assert update_json_key(json_data, "key1", "new_value")
     assert json_data["key1"] == "new_value"
 
+
 def test_update_json_key_new_key():
     json_data = {"key1": "value1"}
     assert update_json_key(json_data, "key2", "value2")
     assert json_data["key2"] == "value2"
 
+
 def test_update_json_key_invalid_key():
     json_data = {"key1": "value1"}
     result = update_json_key(json_data, "key2", "value2")
     assert result == True
     assert "key2" in json_data
 
     # Test with integer key
@@ -84,29 +112,43 @@
 
     # Test with invalid key type (e.g., list)
     result = update_json_key(json_data, ["list_key"], "value")
     assert result == False
 
 
 def test_load_json_performance(json_test_file):
-    iterations = 100000  # Increase iterations to reduce measurement noise
-
-    # Measure time without caching
-    start_time = time.time()
-    for _ in range(iterations):
-        load_json(json_test_file)
-    no_cache_duration = time.time() - start_time
-
-    # Clear cache to measure time with caching
-    global json_cache
-    json_cache = {}
-
-    # Measure time with caching
-    start_time = time.time()
-    for _ in range(iterations):
-        load_json(json_test_file)
-    cache_duration = time.time() - start_time
-
-    print(f"No cache duration: {no_cache_duration:.4f} seconds")
-    print(f"Cache duration: {cache_duration:.4f} seconds")
+    iterations = 5
+    cache_wins = 0
+    no_cache_wins = 0
+    total_runs = 5
+    no_cache_times = []
+    cache_times = []
+
+    for _ in range(total_runs):
+        # Measure time without caching
+        start_time = time.time()
+        for _ in range(iterations):
+            load_json_without_cache(json_test_file)
+        no_cache_duration = time.time() - start_time
+        no_cache_times.append(no_cache_duration)
+
+        # Measure time with caching
+        start_time = time.time()
+        for _ in range(iterations):
+            load_json(json_test_file)
+        cache_duration = time.time() - start_time
+        cache_times.append(cache_duration)
+
+        if cache_duration < no_cache_duration:
+            cache_wins += 1
+        else:
+            no_cache_wins += 1
+
+    avg_no_cache_time = sum(no_cache_times) / len(no_cache_times)
+    avg_cache_time = sum(cache_times) / len(cache_times)
+
+    print(f"\nAverage no cache duration: {avg_no_cache_time:.4f} seconds")
+    print(f"Average cache duration: {avg_cache_time:.4f} seconds")
+    print(f"Cache wins: {cache_wins}")
+    print(f"No cache wins: {no_cache_wins}")
 
-    assert cache_duration < no_cache_duration
+    assert cache_wins > no_cache_wins, "Caching did not provide a performance benefit in the majority of runs"
```

### Comparing `optimized-utility-library-0.1.1/tests/test_llm_image_operations.py` & `optimized-utility-library-0.1.3/tests/test_llm_image_operations.py`

 * *Files identical despite different names*

### Comparing `optimized-utility-library-0.1.1/utility_lib/common/directory_operations.py` & `optimized-utility-library-0.1.3/utility_lib/common/directory_operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,150 +1,202 @@
 import os
 import logging
+import ujson as json  # Use ujson for faster JSON operations
 from pathlib import Path
 
-# Configure logging
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+# Configure the logger for the library
+logger = logging.getLogger('utility_lib')
+logger.setLevel(logging.WARNING)
+logger.addHandler(logging.NullHandler())
 
+# Global cache dictionary
 cache = {}
 
+# Static directory to store state files
+STATEFILES_DIR = Path(__file__).parent / "statefiles"
+STATEFILES_DIR.mkdir(parents=True, exist_ok=True)
 
-def ensure_dir(directory):
+def setup_directories(config):
     """
-    Ensure that a directory exists, creating it if necessary.
+    Ensure all directories specified in the configuration exist.
 
     Args:
-        directory (str): The path to the directory to ensure exists.
+        config (dict): A dictionary where the values are paths to directories to ensure exist.
 
     Raises:
-        Exception: If there is an error creating the directory.
+        Exception: If there is an error creating any of the directories.
     """
     try:
-        Path(directory).mkdir(parents=True, exist_ok=True)
-        logging.info(f"Directory '{directory}' ensured.")
+        for path in config.values():
+            ensure_dir(path)
+        logger.info("All directories set up successfully.")
     except Exception as e:
-        logging.error(f"Failed to ensure directory {directory}: {str(e)}")
-
+        logger.error(f"Failed to set up directories: {str(e)}")
+        raise
 
-def list_files(directory, pattern="*", recursive=False):
+def ensure_dir(directory):
     """
-    List all files in a directory matching the pattern, optionally recursing through subdirectories.
+    Ensure that a directory exists, creating it if necessary.
 
     Args:
-        directory (str): The path to the directory to list files in.
-        pattern (str): The pattern to match files against. Defaults to "*".
-        recursive (bool): Whether to list files recursively. Defaults to False.
-
-    Returns:
-        list: A list of relative file paths matching the pattern.
+        directory (str): The path to the directory to ensure exists.
 
     Raises:
-        Exception: If there is an error listing the files.
+        Exception: If there is an error creating the directory.
     """
     try:
-        path = Path(directory)
-        if recursive:
-            files = list(path.rglob(pattern))
-        else:
-            files = list(path.glob(pattern))
-        return [str(f.relative_to(directory)) for f in files]
+        Path(directory).mkdir(parents=True, exist_ok=True)
     except Exception as e:
-        logging.error(f"Error listing files in {directory}: {str(e)}")
-        return []
-
+        logger.error(f"Failed to ensure directory {directory}: {str(e)}")
+        raise
 
-def setup_directories(config):
+def capture_directory_state(directory):
     """
-    Ensure all directories specified in the configuration exist.
+    Capture the current state of a directory by storing file paths and modification times in a dictionary.
 
     Args:
-        config (dict): A dictionary where the values are paths to directories to ensure exist.
+        directory (str): The path to the directory to capture the state of.
 
-    Raises:
-        Exception: If there is an error creating any of the directories.
+    Returns:
+        dict: A dictionary containing file paths as keys and modification times as values.
     """
-    try:
-        for path in config.values():
-            Path(path).mkdir(parents=True, exist_ok=True)
-        logging.info("All directories set up successfully.")
-    except Exception as e:
-        logging.error(f"Failed to set up directories: {str(e)}")
-
-
-def capture_directory_state(directory):
     state = {}
     for root, _, files in os.walk(directory):
         for file in files:
             file_path = os.path.join(root, file)
             mtime = os.path.getmtime(file_path)
             state[file_path] = mtime
     return state
 
+def get_state_file_path(directory):
+    """
+    Generate a state file path based on the monitored directory.
+
+    Args:
+        directory (str): The path to the directory to generate the state file path for.
+
+    Returns:
+        Path: The path to the state file.
+    """
+    directory_name = directory.replace("/", "_").replace("\\", "_").strip("_")
+    return STATEFILES_DIR / f"{directory_name}_state.json"
 
 def has_directory_changed(directory):
     """
-    Check if the directory has changed by comparing the current state with the previous state stored in the cache.
+    Check if a directory has changed by comparing the current state with the cached state.
 
     Args:
         directory (str): The path to the directory to check.
 
     Returns:
         bool: True if the directory has changed, False otherwise.
     """
-    global cache
+    state_file = get_state_file_path(directory)
 
-    current_state = capture_directory_state(directory)
+    if not state_file.exists():
+        state_file.touch()
+        with state_file.open('w') as file:
+            json.dump({}, file)
+        return False  # Assume no change for a new state file
 
-    if directory not in cache:
-        cache[directory] = current_state
-        return True
+    with state_file.open('r') as file:
+        previous_state = json.load(file)
+
+    current_state = capture_directory_state(directory)
 
-    if current_state != cache[directory]:
-        cache[directory] = current_state
+    if current_state != previous_state:
+        with state_file.open('w') as file:
+            json.dump(current_state, file)
         return True
 
     return False
 
+def list_files(directory, pattern="*", recursive=False):
+    """
+    List all files in a directory matching the pattern, optionally recursing through subdirectories.
+
+    Args:
+        directory (str): The path to the directory to list files in.
+        pattern (str): The pattern to match files against. Defaults to "*".
+        recursive (bool): Whether to list files recursively. Defaults to False.
+
+    Returns:
+        dict: A dictionary containing file paths as keys and modification times as values.
+
+    Raises:
+        Exception: If there is an error listing the files.
+    """
+    global cache
+    cache_key = (directory, pattern, recursive)
+
+    if cache_key in cache:
+        return cache[cache_key]
+
+    try:
+        path = Path(directory)
+        if recursive:
+            files = path.rglob(pattern)
+        else:
+            files = path.glob(pattern)
+
+        file_dict = {str(f.absolute()): os.path.getmtime(f) for f in files if f.is_file()}
+        cache[cache_key] = file_dict
+        return file_dict
+    except Exception as e:
+        logger.error(f"Error listing files in {directory}: {str(e)}")
+        raise
 
 def get_latest_files(directory, num_files=0, file_ext=None):
     """
     Get the latest files in the directory, optionally filtering by file extension and limiting the number of results.
 
     Args:
         directory (str): The path to the directory to list files in.
         num_files (int): The number of latest files to return. If 0, return all files. Defaults to 0.
-        file_ext (str): The file extension to filter by. If None, no filtering is applied. Defaults to None.
+        file_ext (str, optional): The file extension to filter by. If None, no filtering is applied. Defaults to None.
 
     Returns:
         list: A list of file paths sorted by modification time, newest first.
     """
     global cache
 
     # Check if the directory has changed
-    if has_directory_changed(directory):
-        logging.info(f"Directory '{directory}' has changed. Updating cache.")
-        files = []
-        for root, _, file_list in os.walk(directory):
-            for file in file_list:
-                file_path = os.path.join(root, file)
-                if not os.path.isfile(file_path):
-                    continue
-                if file_ext is None or file.lower().endswith(file_ext):
-                    files.append((file_path, os.path.getmtime(file_path)))
-
-        # Sort the files based on modification time (newest first)
-        files.sort(key=lambda x: x[1], reverse=True)
+    directory_changed = has_directory_changed(directory)
 
-        # Update the cache
+    if directory_changed or directory not in cache:
+        files = list_files(directory)
         cache[directory] = files
     else:
-        logging.info(f"Using cached data for directory '{directory}'.")
         files = cache[directory]
 
+    # Filter files by the specified extension using str.endswith()
+    if file_ext:
+        filtered_files = {file: mtime for file, mtime in files.items() if file.lower().endswith(file_ext.lower())}
+    else:
+        filtered_files = files
+
+    # Sort the filtered files based on modification time (newest first)
+    sorted_files = sorted(filtered_files.items(), key=lambda x: x[1], reverse=True)
+
     # Limit the number of files if num_files is specified
     if num_files > 0:
-        files = files[:num_files]
+        sorted_files = sorted_files[:num_files]
+
+    # Extract only the file paths from the sorted files
+    latest_files = [file for file, _ in sorted_files]
+
+    # Update the cache with the latest files and their modification times
+    cache[(directory, '*', False)] = {file: mtime for file, mtime in sorted_files}
 
-    return [file[0] for file in files]
+    return latest_files
+
+def clear_cache():
+    """
+    Clear the global cache.
+
+    This function is primarily used for testing purposes to ensure the cache is reset.
+    """
+    global cache
+    cache.clear()
 
 
-__all__ = ['ensure_dir', 'list_files', 'setup_directories', 'has_directory_changed', 'get_latest_files']
+__all__ = ['ensure_dir', 'list_files', 'setup_directories', 'has_directory_changed', 'get_latest_files', 'clear_cache']
```

### Comparing `optimized-utility-library-0.1.1/utility_lib/common/file_operations.py` & `optimized-utility-library-0.1.3/utility_lib/common/file_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import os
 import shutil
 import logging
 import csv
 from concurrent.futures import ThreadPoolExecutor
 from time import ctime
 
-# Configure logging
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+# Configure the logger for the library
+logger = logging.getLogger('utility_lib')
+logger.setLevel(logging.WARNING)
+
+# Add a default NullHandler to prevent "No handler found" warnings
+logger.addHandler(logging.NullHandler())
+
 
 # Global cache dictionary
 file_cache = {}
 
 
 def read_file(file_path):
     """
```

### Comparing `optimized-utility-library-0.1.1/utility_lib/common/image_operations.py` & `optimized-utility-library-0.1.3/utility_lib/common/image_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import os
 import logging
 from PIL import Image, UnidentifiedImageError
 from matplotlib import pyplot as plt
 import base64
 import cv2
 
-# Configure logging
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+# Configure the logger for the library
+logger = logging.getLogger('utility_lib')
+logger.setLevel(logging.WARNING)
+
+# Add a default NullHandler to prevent "No handler found" warnings
+logger.addHandler(logging.NullHandler())
+
 
 # Global cache dictionary
 file_cache = {}
 
 
 def display_img(filepath):
     """
```

