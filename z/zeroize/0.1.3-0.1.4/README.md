# Comparing `tmp/zeroize-0.1.3.tar.gz` & `tmp/zeroize-0.1.4.tar.gz`

## Comparing `zeroize-0.1.3.tar` & `zeroize-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 zeroize-0.1.3/Cargo.toml
--rw-r--r--   0     1001      127     3526 2024-06-02 00:44:05.000000 zeroize-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      713 2024-06-02 00:44:05.000000 zeroize-0.1.3/.gitignore
--rw-r--r--   0     1001      127      395 2024-06-02 00:44:05.000000 zeroize-0.1.3/.gitpod
--rw-r--r--   0     1001      127    11357 2024-06-02 00:44:05.000000 zeroize-0.1.3/LICENSE
--rw-r--r--   0     1001      127     1717 2024-06-02 00:44:05.000000 zeroize-0.1.3/README.md
--rw-r--r--   0     1001      127      395 2024-06-02 00:44:05.000000 zeroize-0.1.3/main.py
--rw-r--r--   0     1001      127      638 2024-06-02 00:44:05.000000 zeroize-0.1.3/src/lib.rs
--rw-r--r--   0     1001      127      527 2024-06-02 00:44:05.000000 zeroize-0.1.3/tests/test_zeroize.py
--rw-r--r--   0     1001      127    10218 2024-06-02 00:44:05.000000 zeroize-0.1.3/Cargo.lock
--rw-r--r--   0     1001      127      983 2024-06-02 00:44:05.000000 zeroize-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 zeroize-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 zeroize-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-06-02 00:50:25.000000 zeroize-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      713 2024-06-02 00:50:25.000000 zeroize-0.1.4/.gitignore
+-rw-r--r--   0     1001      127      395 2024-06-02 00:50:25.000000 zeroize-0.1.4/.gitpod
+-rw-r--r--   0     1001      127    11357 2024-06-02 00:50:25.000000 zeroize-0.1.4/LICENSE
+-rw-r--r--   0     1001      127     1720 2024-06-02 00:50:25.000000 zeroize-0.1.4/README.md
+-rw-r--r--   0     1001      127      430 2024-06-02 00:50:25.000000 zeroize-0.1.4/main.py
+-rw-r--r--   0     1001      127      638 2024-06-02 00:50:25.000000 zeroize-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      127      527 2024-06-02 00:50:25.000000 zeroize-0.1.4/tests/test_zeroize.py
+-rw-r--r--   0     1001      127    10218 2024-06-02 00:50:25.000000 zeroize-0.1.4/Cargo.lock
+-rw-r--r--   0     1001      127      983 2024-06-02 00:50:25.000000 zeroize-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2605 1970-01-01 00:00:00.000000 zeroize-0.1.4/PKG-INFO
```

### Comparing `zeroize-0.1.3/.github/workflows/CI.yml` & `zeroize-0.1.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `zeroize-0.1.3/.gitignore` & `zeroize-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `zeroize-0.1.3/LICENSE` & `zeroize-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zeroize-0.1.3/README.md` & `zeroize-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,23 @@
 
 # regular array
 arr = bytearray(b'1234567890')
 # numpy array
 arr_np = np.array([0] * 10, dtype=np.uint8)
 arr_np[:] = arr
 assert arr_np.tobytes() == b'1234567890'
+
+print("zeroize'ing...: ")
 zeroize.zeroize1(arr)
 zeroize.zeroize_np(arr_np)
-print("zeroize'ing...: ")
+
 print("checking if is zeroized...")
 assert arr == bytearray(b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00')
 assert all(arr_np == 0)
+
 print("all good, bye!")
 ```
 # Building from source
 
 ## Browser
 
 [![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/radumarias/zeroize-python)
```

### Comparing `zeroize-0.1.3/src/lib.rs` & `zeroize-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `zeroize-0.1.3/tests/test_zeroize.py` & `zeroize-0.1.4/tests/test_zeroize.py`

 * *Files identical despite different names*

### Comparing `zeroize-0.1.3/Cargo.lock` & `zeroize-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "zeroize"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "numpy",
  "pyo3",
  "zeroize 1.8.1",
 ]
 
 [[package]]
```

### Comparing `zeroize-0.1.3/pyproject.toml` & `zeroize-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zeroize-0.1.3/PKG-INFO` & `zeroize-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: zeroize
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: Apache Software License
 License-File: LICENSE
 Summary: Securely clear secrets from memory. Built on stable Rust primitives which guarantee memory is zeroed using an operation will not be 'optimized away' by the compiler. Uses a portable pure Rust implementation that works everywhere.
 Keywords: memory,volatile,secure,memset,zero
@@ -31,20 +31,23 @@
 
 # regular array
 arr = bytearray(b'1234567890')
 # numpy array
 arr_np = np.array([0] * 10, dtype=np.uint8)
 arr_np[:] = arr
 assert arr_np.tobytes() == b'1234567890'
+
+print("zeroize'ing...: ")
 zeroize.zeroize1(arr)
 zeroize.zeroize_np(arr_np)
-print("zeroize'ing...: ")
+
 print("checking if is zeroized...")
 assert arr == bytearray(b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00')
 assert all(arr_np == 0)
+
 print("all good, bye!")
 ```
 # Building from source
 
 ## Browser
 
 [![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/radumarias/zeroize-python)
```

