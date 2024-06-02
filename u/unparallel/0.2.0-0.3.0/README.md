# Comparing `tmp/unparallel-0.2.0.tar.gz` & `tmp/unparallel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unparallel-0.2.0.tar", max compression
+gzip compressed data, was "unparallel-0.3.0.tar", max compression
```

## Comparing `unparallel-0.2.0.tar` & `unparallel-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-12-29 14:08:38.303755 unparallel-0.2.0/LICENSE
--rw-r--r--   0        0        0     4987 2023-12-29 14:08:38.303755 unparallel-0.2.0/README.md
--rw-r--r--   0        0        0     3500 2023-12-29 14:08:38.303755 unparallel-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      357 2023-12-29 14:08:38.313755 unparallel-0.2.0/unparallel/__init__.py
--rw-r--r--   0        0        0     9996 2023-12-29 14:08:38.313755 unparallel-0.2.0/unparallel/unparallel.py
--rw-r--r--   0        0        0     6002 1970-01-01 00:00:00.000000 unparallel-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-03-02 16:43:45.111394 unparallel-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4956 2024-03-02 16:43:45.111394 unparallel-0.3.0/README.md
+-rw-r--r--   0        0        0     3555 2024-03-02 16:43:45.119394 unparallel-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      357 2024-03-02 16:43:45.119394 unparallel-0.3.0/unparallel/__init__.py
+-rw-r--r--   0        0        0    12919 2024-03-02 16:43:45.119394 unparallel-0.3.0/unparallel/unparallel.py
+-rw-r--r--   0        0        0      234 2024-03-02 16:43:45.119394 unparallel-0.3.0/unparallel/utils.py
+-rw-r--r--   0        0        0     5976 1970-01-01 00:00:00.000000 unparallel-0.3.0/PKG-INFO
```

### Comparing `unparallel-0.2.0/LICENSE` & `unparallel-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unparallel-0.2.0/README.md` & `unparallel-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,16 @@
 A simple example of doing several GET requests to an HTTP web service:
 
 ```python
 import asyncio
 from unparallel import up
 
 async def main():
-    url = "https://httpbin.org"
-    paths = [f"/get?i={i}" for i in range(5)]
-    results = await up(url, paths)
+    urls = [f"https://httpbin.org/get?i={i}" for i in range(5)]
+    results = await up(urls)
     print([item["args"] for item in results])
 
 asyncio.run(main())
 ```
 
 This prints:
 ```
@@ -58,18 +57,17 @@
 Similarly, we can do a bunch of POST requests. This time we will use a single path but multiple payloads:
 
 ```python
 import asyncio
 from unparallel import up
 
 async def main():
-    url = "https://httpbin.org"
-    path = "/post"
+    url = "https://httpbin.org/post"
     payloads = [{"obj_id": i} for i in range(5)]
-    results = await up(url, path, method="post", payloads=payloads)
+    results = await up(url, method="post", payloads=payloads)
     print([item["data"] for item in results])
 
 asyncio.run(main())
 ```
 
 This prints:
 ```
@@ -117,15 +115,15 @@
 from unparallel import up
 
 
 async def main():
     url = "https://httpbin.org"
     paths = [f"/get?i={i}" for i in range(20)]
 
-    results = await up(url, paths)
+    results = await up(paths, base_url=url)
 
     assert len(results) == 20
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `unparallel-0.2.0/pyproject.toml` & `unparallel-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "unparallel"
-version = "0.2.0"
+version = "0.3.0"
 description = "Create async web requests in no time"
 readme = "README.md"
 authors = ["RafaelWO <weingartner.rafael@hotmail.com>"]
 license = "MIT"
 repository = "https://github.com/RafaelWO/unparallel"
 homepage = "https://github.com/RafaelWO/unparallel"
 
@@ -30,36 +30,37 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 
 
 
 [tool.poetry.dependencies]
-python = ">=3.8"
+python = ">=3.8,<4.0"
 httpx = ">=0.21.0"
 tqdm = ">=4.61.2"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.1"
 black = "^23.11.0"
 isort = {extras = ["colors"], version = "^5.10.1"}
 mypy = "^1.7"
 mypy-extensions = "^1.0.0"
 pre-commit = "^3.5.0"
 pydocstyle = "^6.1.1"
 pylint = "^3.0.2"
-pytest = "^7.4.3"
+pytest = ">=7.4.3,<9.0.0"
 pyupgrade = "^3.8.0"
-safety = "^2.3.5"
+safety = ">=2.3.5,<4.0.0"
 coverage = "^7.3.2"
 coverage-badge = "^1.1.0"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.23.2"
 respx = "^0.20.2"
 bump2version = "^1.0.1"
+pytest-markdown-docs = "^0.5.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.5.1"
 mkdocstrings-python = "^1.7.5"
 mike = "^2.0.0"
 
 [tool.black]
@@ -93,15 +94,15 @@
 profile = "black"
 multi_line_output = 3
 indent = 4
 color_output = true
 
 [tool.mypy]
 # https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
-python_version = 3.8
+python_version = "3.8"
 pretty = true
 show_traceback = true
 color_output = true
 
 allow_redefinition = false
 check_untyped_defs = true
 disallow_any_generics = true
```

### Comparing `unparallel-0.2.0/PKG-INFO` & `unparallel-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: unparallel
-Version: 0.2.0
+Version: 0.3.0
 Summary: Create async web requests in no time
 Home-page: https://github.com/RafaelWO/unparallel
 License: MIT
 Keywords: async,http,requests,network
 Author: RafaelWO
 Author-email: weingartner.rafael@hotmail.com
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -62,17 +62,16 @@
 A simple example of doing several GET requests to an HTTP web service:
 
 ```python
 import asyncio
 from unparallel import up
 
 async def main():
-    url = "https://httpbin.org"
-    paths = [f"/get?i={i}" for i in range(5)]
-    results = await up(url, paths)
+    urls = [f"https://httpbin.org/get?i={i}" for i in range(5)]
+    results = await up(urls)
     print([item["args"] for item in results])
 
 asyncio.run(main())
 ```
 
 This prints:
 ```
@@ -84,18 +83,17 @@
 Similarly, we can do a bunch of POST requests. This time we will use a single path but multiple payloads:
 
 ```python
 import asyncio
 from unparallel import up
 
 async def main():
-    url = "https://httpbin.org"
-    path = "/post"
+    url = "https://httpbin.org/post"
     payloads = [{"obj_id": i} for i in range(5)]
-    results = await up(url, path, method="post", payloads=payloads)
+    results = await up(url, method="post", payloads=payloads)
     print([item["data"] for item in results])
 
 asyncio.run(main())
 ```
 
 This prints:
 ```
@@ -143,15 +141,15 @@
 from unparallel import up
 
 
 async def main():
     url = "https://httpbin.org"
     paths = [f"/get?i={i}" for i in range(20)]
 
-    results = await up(url, paths)
+    results = await up(paths, base_url=url)
 
     assert len(results) == 20
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

