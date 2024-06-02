# Comparing `tmp/pytrydan-0.6.1.tar.gz` & `tmp/pytrydan-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrydan-0.6.1.tar", max compression
+gzip compressed data, was "pytrydan-0.7.0.tar", max compression
```

## Comparing `pytrydan-0.6.1.tar` & `pytrydan-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2024-05-11 13:49:57.271379 pytrydan-0.6.1/LICENSE
--rw-r--r--   0        0        0     4822 2024-05-11 13:49:57.271379 pytrydan-0.6.1/README.md
--rw-r--r--   0        0        0     3517 2024-05-11 13:49:57.963380 pytrydan-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      754 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/__init__.py
--rw-r--r--   0        0        0      102 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/__main__.py
--rw-r--r--   0        0        0     2003 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/cli.py
--rw-r--r--   0        0        0      340 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/const.py
--rw-r--r--   0        0        0      562 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/exceptions.py
--rw-r--r--   0        0        0     2053 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/main.py
--rw-r--r--   0        0        0     4129 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/models/trydan.py
--rw-r--r--   0        0        0        0 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/py.typed
--rw-r--r--   0        0        0     9434 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/trydan.py
--rw-r--r--   0        0        0     6029 1970-01-01 00:00:00.000000 pytrydan-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-06-02 11:07:38.478972 pytrydan-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4822 2024-06-02 11:07:38.478972 pytrydan-0.7.0/README.md
+-rw-r--r--   0        0        0     3517 2024-06-02 11:07:39.238975 pytrydan-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      754 2024-06-02 11:07:38.478972 pytrydan-0.7.0/src/pytrydan/__init__.py
+-rw-r--r--   0        0        0      102 2024-06-02 11:07:38.478972 pytrydan-0.7.0/src/pytrydan/__main__.py
+-rw-r--r--   0        0        0     2003 2024-06-02 11:07:38.478972 pytrydan-0.7.0/src/pytrydan/cli.py
+-rw-r--r--   0        0        0      340 2024-06-02 11:07:38.478972 pytrydan-0.7.0/src/pytrydan/const.py
+-rw-r--r--   0        0        0      562 2024-06-02 11:07:38.478972 pytrydan-0.7.0/src/pytrydan/exceptions.py
+-rw-r--r--   0        0        0     2053 2024-06-02 11:07:38.478972 pytrydan-0.7.0/src/pytrydan/main.py
+-rw-r--r--   0        0        0     4129 2024-06-02 11:07:38.478972 pytrydan-0.7.0/src/pytrydan/models/trydan.py
+-rw-r--r--   0        0        0        0 2024-06-02 11:07:38.478972 pytrydan-0.7.0/src/pytrydan/py.typed
+-rw-r--r--   0        0        0     9561 2024-06-02 11:07:38.478972 pytrydan-0.7.0/src/pytrydan/trydan.py
+-rw-r--r--   0        0        0     6029 1970-01-01 00:00:00.000000 pytrydan-0.7.0/PKG-INFO
```

### Comparing `pytrydan-0.6.1/LICENSE` & `pytrydan-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.1/README.md` & `pytrydan-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.1/pyproject.toml` & `pytrydan-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytrydan"
-version = "0.6.1"
+version = "0.7.0"
 description = "Library to interface with V2C EVSE Trydan"
 authors = ["Diogo Gomes <diogogomes@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dgomes/pytrydan"
 documentation = "https://pytrydan.readthedocs.io"
 classifiers = [
```

### Comparing `pytrydan-0.6.1/src/pytrydan/__init__.py` & `pytrydan-0.7.0/src/pytrydan/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.1/src/pytrydan/cli.py` & `pytrydan-0.7.0/src/pytrydan/cli.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.1/src/pytrydan/exceptions.py` & `pytrydan-0.7.0/src/pytrydan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.1/src/pytrydan/main.py` & `pytrydan-0.7.0/src/pytrydan/main.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.1/src/pytrydan/models/trydan.py` & `pytrydan-0.7.0/src/pytrydan/models/trydan.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.1/src/pytrydan/trydan.py` & `pytrydan-0.7.0/src/pytrydan/trydan.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,19 @@
         """Make a request to Trydan."""
         _LOGGER.debug("Requesting %s with timeout %s", url, self._timeout)
         response = await self._client.get(
             url,
             timeout=self._timeout,
         )
 
+        self.raw_data = {
+            "content": response.content,
+            "status_code": response.status_code,
+        }
+
         status_code = response.status_code
         if status_code in (HTTPStatus.UNAUTHORIZED, HTTPStatus.FORBIDDEN):
             raise TrydanCommunicationError(
                 f"Failed for {url} with status {status_code}"
             )
         if status_code != HTTPStatus.OK:
             raise TrydanInvalidResponse(f"Failed for {url} with status {status_code}")
```

### Comparing `pytrydan-0.6.1/PKG-INFO` & `pytrydan-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrydan
-Version: 0.6.1
+Version: 0.7.0
 Summary: Library to interface with V2C EVSE Trydan
 Home-page: https://github.com/dgomes/pytrydan
 License: MIT
 Author: Diogo Gomes
 Author-email: diogogomes@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytrydan Version: 0.6.1 Summary: Library to
+Metadata-Version: 2.1 Name: pytrydan Version: 0.7.0 Summary: Library to
 interface with V2C EVSE Trydan Home-page: https://github.com/dgomes/pytrydan
 License: MIT Author: Diogo Gomes Author-email: diogogomes@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

