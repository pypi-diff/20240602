# Comparing `tmp/papers_dl-0.0.8.tar.gz` & `tmp/papers_dl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papers_dl-0.0.8.tar", last modified: Fri May 31 20:06:25 2024, max compression
+gzip compressed data, was "papers_dl-0.0.9.tar", last modified: Sun Jun  2 07:27:53 2024, max compression
```

## Comparing `papers_dl-0.0.8.tar` & `papers_dl-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-31 20:06:25.555890 papers_dl-0.0.8/
--rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.8/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     1700 2024-05-31 20:06:25.555544 papers_dl-0.0.8/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      381 2024-05-31 19:58:24.000000 papers_dl-0.0.8/README.md
--rw-r--r--   0 ben        (501) staff       (20)     1276 2024-05-07 21:38:53.000000 papers_dl-0.0.8/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2024-05-31 20:06:25.555969 papers_dl-0.0.8/setup.cfg
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-31 20:06:25.552251 papers_dl-0.0.8/src/
--rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-06 22:49:47.000000 papers_dl-0.0.8/src/__init__.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-31 20:06:25.555046 papers_dl-0.0.8/src/papers_dl.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     1700 2024-05-31 20:06:25.000000 papers_dl-0.0.8/src/papers_dl.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      389 2024-05-31 20:06:25.000000 papers_dl-0.0.8/src/papers_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-31 20:06:25.000000 papers_dl-0.0.8/src/papers_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       45 2024-05-31 20:06:25.000000 papers_dl-0.0.8/src/papers_dl.egg-info/entry_points.txt
--rw-r--r--   0 ben        (501) staff       (20)      411 2024-05-31 20:06:25.000000 papers_dl-0.0.8/src/papers_dl.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       40 2024-05-31 20:06:25.000000 papers_dl-0.0.8/src/papers_dl.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)     3625 2024-05-31 19:38:07.000000 papers_dl-0.0.8/src/papers_dl.py
--rw-r--r--   0 ben        (501) staff       (20)     2584 2024-05-31 20:05:32.000000 papers_dl-0.0.8/src/parse.py
--rw-r--r--   0 ben        (501) staff       (20)     8032 2024-05-26 19:19:04.000000 papers_dl-0.0.8/src/scihub.py
--rw-r--r--   0 ben        (501) staff       (20)       22 2024-05-31 20:06:20.000000 papers_dl-0.0.8/src/version.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-31 20:06:25.554509 papers_dl-0.0.8/tests/
--rw-r--r--   0 ben        (501) staff       (20)     1182 2024-05-31 18:22:02.000000 papers_dl-0.0.8/tests/test_cli.py
--rw-r--r--   0 ben        (501) staff       (20)      775 2024-05-26 19:19:04.000000 papers_dl-0.0.8/tests/test_fetch.py
--rw-r--r--   0 ben        (501) staff       (20)     2606 2024-05-31 18:26:26.000000 papers_dl-0.0.8/tests/test_parse.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-06-02 07:27:53.944487 papers_dl-0.0.9/
+-rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.9/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     1691 2024-06-02 07:27:53.944143 papers_dl-0.0.9/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      372 2024-06-02 07:27:14.000000 papers_dl-0.0.9/README.md
+-rw-r--r--   0 ben        (501) staff       (20)     1276 2024-05-07 21:38:53.000000 papers_dl-0.0.9/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2024-06-02 07:27:53.944576 papers_dl-0.0.9/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-06-02 07:27:53.940117 papers_dl-0.0.9/src/
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-06 22:49:47.000000 papers_dl-0.0.9/src/__init__.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-06-02 07:27:53.943450 papers_dl-0.0.9/src/papers_dl.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     1691 2024-06-02 07:27:53.000000 papers_dl-0.0.9/src/papers_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      389 2024-06-02 07:27:53.000000 papers_dl-0.0.9/src/papers_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-06-02 07:27:53.000000 papers_dl-0.0.9/src/papers_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       45 2024-06-02 07:27:53.000000 papers_dl-0.0.9/src/papers_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (501) staff       (20)      411 2024-06-02 07:27:53.000000 papers_dl-0.0.9/src/papers_dl.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       40 2024-06-02 07:27:53.000000 papers_dl-0.0.9/src/papers_dl.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)     3906 2024-06-02 07:08:37.000000 papers_dl-0.0.9/src/papers_dl.py
+-rw-r--r--   0 ben        (501) staff       (20)     2584 2024-05-31 20:05:32.000000 papers_dl-0.0.9/src/parse.py
+-rw-r--r--   0 ben        (501) staff       (20)     8754 2024-06-02 07:00:14.000000 papers_dl-0.0.9/src/scihub.py
+-rw-r--r--   0 ben        (501) staff       (20)       22 2024-06-01 22:59:36.000000 papers_dl-0.0.9/src/version.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-06-02 07:27:53.942958 papers_dl-0.0.9/tests/
+-rw-r--r--   0 ben        (501) staff       (20)     1182 2024-05-31 18:22:02.000000 papers_dl-0.0.9/tests/test_cli.py
+-rw-r--r--   0 ben        (501) staff       (20)      775 2024-05-26 19:19:04.000000 papers_dl-0.0.9/tests/test_fetch.py
+-rw-r--r--   0 ben        (501) staff       (20)     2606 2024-05-31 18:26:26.000000 papers_dl-0.0.9/tests/test_parse.py
```

### Comparing `papers_dl-0.0.8/LICENSE` & `papers_dl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.8/PKG-INFO` & `papers_dl-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papers-dl
-Version: 0.0.8
+Version: 0.0.9
 Summary: A command line application for downloading scientific papers
 Author-email: Ben Muthalaly <benmuthalaly@gmail.com>
 Project-URL: Homepage, https://github.com/benmuth/papers-dl
 Project-URL: Issues, https://github.com/benmuth/papers-dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,15 +38,15 @@
 Requires-Dist: w3lib==2.1.2
 
 # Overview
 `papers-dl` is a command line application for downloading scientific papers.
 
 ## Usage
 ```shell
-# parse certain identifier types from a file:
+# parse DOI identifiers from a file:
 papers-dl parse --match doi --path pages/my-paper.html
 
 # fetch given identifier from SciHub:
 papers-dl fetch "10.1016/j.cub.2019.11.030"
 ```
 
 This project started as a fork of [scihub.py](https://github.com/zaytoun/scihub.py).
```

### Comparing `papers_dl-0.0.8/pyproject.toml` & `papers_dl-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.8/src/papers_dl.egg-info/PKG-INFO` & `papers_dl-0.0.9/src/papers_dl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papers-dl
-Version: 0.0.8
+Version: 0.0.9
 Summary: A command line application for downloading scientific papers
 Author-email: Ben Muthalaly <benmuthalaly@gmail.com>
 Project-URL: Homepage, https://github.com/benmuth/papers-dl
 Project-URL: Issues, https://github.com/benmuth/papers-dl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,15 +38,15 @@
 Requires-Dist: w3lib==2.1.2
 
 # Overview
 `papers-dl` is a command line application for downloading scientific papers.
 
 ## Usage
 ```shell
-# parse certain identifier types from a file:
+# parse DOI identifiers from a file:
 papers-dl parse --match doi --path pages/my-paper.html
 
 # fetch given identifier from SciHub:
 papers-dl fetch "10.1016/j.cub.2019.11.030"
 ```
 
 This project started as a fork of [scihub.py](https://github.com/zaytoun/scihub.py).
```

### Comparing `papers_dl-0.0.8/src/papers_dl.py` & `papers_dl-0.0.9/src/papers_dl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,80 @@
 import argparse
 import os
 import sys
+import logging
+
 
 from scihub import SciHub
 from parse import parse_file, format_output, parse_ids_from_text, id_patterns
 import pdf2doi
 import json
 
 supported_fetch_identifier_types = ["doi", "pmid", "url", "isbn"]
 
+logging.basicConfig()
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+
 
-def save_scihub(identifier: str, out: str, user_agent: str, name: str | None = None):
+def save_scihub(
+    identifier: str, out: str, user_agent: str, name: str | None = None
+) -> str:
     """
     find a paper with the given identifier and download it to the output
     directory. If given, name will be the name of the output file. otherwise
     we attempt to find a title from the PDF contents.
     """
 
     sh = SciHub(user_agent)
-    print(f"Attempting to download from {identifier}")
+    logging.info(f"Attempting to download from {identifier}")
 
     result = sh.download(identifier, out)
     if not result:
-        return
+        return ""
 
-    print(f"Successfully downloaded file with identifier {identifier}")
+    logging.info(f"Successfully downloaded file with identifier {identifier}")
 
-    # try to find and use the actual title of the paper
+    logging.info("Finding paper title")
     pdf2doi.config.set("verbose", False)
     result_path = os.path.join(out, result["name"])
 
     try:
         result_info = pdf2doi.pdf2doi(result_path)
         validation_info = json.loads(result_info["validation_info"])
     except TypeError:
-        print("Invalid JSON!")
-        return
+        logging.error("Invalid JSON!")
+        return ""
 
     title = validation_info.get("title")
 
     file_name = name if name else title
     if file_name:
         file_name += ".pdf"
         new_path = os.path.join(out, file_name)
         os.rename(result_path, new_path)
-        print(f"File downloaded to {new_path}")
+        logging.info(f"File downloaded to {new_path}")
+        return new_path
+    return result_path
 
 
-def parse(args):
+def parse(args) -> str:
     # if a path isn't passed or is empty, read from stdin
     if not (hasattr(args, "path") and args.path):
         return format_output(parse_ids_from_text(sys.stdin.read(), args.match))
 
     return format_output(parse_file(args.path, args.match), args.format)
 
 
-def fetch(args):
-    save_scihub(args.query, args.output, args.user_agent)
+def fetch(args) -> str:
+    path = save_scihub(args.query, args.output, args.user_agent)
+    if path:
+        return path
+    else:
+        return "No paper found"
 
 
 def main():
     name = "papers-dl"
     parser = argparse.ArgumentParser(
         prog=name,
         description="Download scientific papers from the command line",
```

### Comparing `papers_dl-0.0.8/src/parse.py` & `papers_dl-0.0.9/src/parse.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.8/src/scihub.py` & `papers_dl-0.0.9/src/scihub.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 from bs4 import BeautifulSoup
 from retrying import retry
 
 import enum
 
 # log config
 logging.basicConfig()
-logger = logging.getLogger("Sci-Hub")
-logger.setLevel(logging.DEBUG)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 urllib3.disable_warnings()
 
 # URL-DIRECT - openly accessible paper
 # URL-NON-DIRECT - pay-walled paper
 # PMID - PubMed ID
 # DOI - digital object identifier
 IDClass = enum.Enum("identifier", ["URL-DIRECT", "URL-NON-DIRECT", "PMD", "DOI"])
 
 DEFAULT_USER_AGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3 Safari/605.1.15"
 
 
 class IdentifierNotFoundError(Exception):
+    "Error for when the identifier wasn't found at any SciHub url"
+
     pass
 
 
 class SiteAccessError(Exception):
     pass
 
 
@@ -96,81 +98,96 @@
 
     def download(self, identifier, destination="", path=None) -> dict[str, str] | None:
         """
         Downloads a paper from sci-hub given an indentifier (DOI, PMID, URL).
         Currently, this can potentially be blocked by a captcha if a certain
         limit has been reached.
         """
-        data = self.fetch(identifier)
-
-        # TODO: allow for passing in name
-        if data:
-            self._save(
-                data["pdf"],
-                os.path.join(destination, path if path else data["name"]),
-            )
-        return data
+        try:
+            data = self.fetch(identifier)
 
-    @retry(wait_random_min=100, wait_random_max=1000, stop_max_attempt_number=20)
-    def fetch(self, identifier) -> dict[str, str | bytes | None] | None:
+            # TODO: allow for passing in name
+            if data:
+                self._save(
+                    data["pdf"],
+                    os.path.join(destination, path if path else data["name"]),
+                )
+            return data
+        except IdentifierNotFoundError:
+            logger.error(f"Failed to find identifier {identifier}")
+
+    @retry(
+        wait_random_min=100,
+        wait_random_max=1000,
+        stop_max_attempt_number=20,
+        retry_on_exception=lambda e: not (
+            isinstance(e, IdentifierNotFoundError) or isinstance(e, IndexError)
+        ),
+    )
+    def fetch(self, identifier) -> dict | None:
         """
         Fetches the paper by first retrieving the direct link to the pdf.
         If the indentifier is a DOI, PMID, or URL pay-wall, then use Sci-Hub
         to access and download paper. Otherwise, just download paper directly.
         """
-        url = None
+        logger.info(f"Looking for {identifier}")
         try:
             # find the url to the pdf for a given identifier
             url = self._get_direct_url(identifier)
-            logger.info("Found potential source at %s", identifier)
+            logger.info(f"Found potential source at {url}")
 
             # verify=False is dangerous but sci-hub.io
             # requires intermediate certificates to verify
             # and requests doesn't know how to download them.
             # as a hacky fix, you can add them to your store
             # and verifying would work. will fix this later.
             # NOTE(ben): see this SO answer: https://stackoverflow.com/questions/27068163/python-requests-not-handling-missing-intermediate-certificate-only-from-one-mach
             res = self.sess.get(url, verify=True)
 
             if res.headers["Content-Type"] != "application/pdf":
-                logger.error(
-                    "Failed to fetch PDF with identifier %s (resolved url %s) due to captcha, changing url...",
-                    identifier,
-                    url,
-                )
-                self._change_base_url()
-                raise CaptchaNeededError("Failed to fetch PDF due to captcha")
+                if res.status_code == 404:
+                    logger.error(
+                        f"Couldn't find PDF with identifier {identifier} at URL {url}, changing base url..."
+                    )
+                    raise SiteAccessError("Couldn't find PDF")
+                else:
+                    logger.error(
+                        "Failed to fetch PDF with identifier %s at URL %s due to captcha, changing base URL...",
+                        identifier,
+                        url,
+                    )
+                    raise CaptchaNeededError("Failed to fetch PDF due to captcha")
             else:
                 return {
                     "pdf": res.content,
                     "url": url,
                     "name": self._generate_name(res),
                 }
 
         except Exception as e:
+            if len(self.available_base_url_list) < 1:
+                raise IdentifierNotFoundError
             logger.info(
-                "Cannot access %s: %s, changing url...",
-                self.available_base_url_list[0],
-                e,
+                f"Cannot access source from {self.available_base_url_list[0]}: {e}, changing base URL..."
             )
             self._change_base_url()
             raise SiteAccessError("Failed to access site")
 
-    def _get_direct_url(self, identifier: str) -> str | None:
+    def _get_direct_url(self, identifier: str) -> str:
         """
         Finds the direct source url for a given identifier.
         """
         id_type = self._classify(identifier)
 
         if id_type == IDClass["URL-DIRECT"]:
             return identifier
         else:
             return self._search_direct_url(identifier)
 
-    def _search_direct_url(self, identifier) -> str | None:
+    def _search_direct_url(self, identifier) -> str:
         """
         Sci-Hub embeds papers in an iframe. This function finds the actual
         source url which looks something like https://moscow.sci-hub.io/.../....pdf.
         """
 
         while True:
             res = self.sess.get(self.base_url + identifier, verify=True)
```

### Comparing `papers_dl-0.0.8/tests/test_cli.py` & `papers_dl-0.0.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.8/tests/test_fetch.py` & `papers_dl-0.0.9/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.8/tests/test_parse.py` & `papers_dl-0.0.9/tests/test_parse.py`

 * *Files identical despite different names*

