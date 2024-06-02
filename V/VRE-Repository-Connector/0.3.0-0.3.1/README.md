# Comparing `tmp/vre_repository_connector-0.3.0.tar.gz` & `tmp/vre_repository_connector-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vre_repository_connector-0.3.0.tar", max compression
+gzip compressed data, was "vre_repository_connector-0.3.1.tar", max compression
```

## Comparing `vre_repository_connector-0.3.0.tar` & `vre_repository_connector-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2024-05-31 13:15:46.462204 vre_repository_connector-0.3.0/LICENSE
--rw-r--r--   0        0        0     1314 2024-05-31 23:18:03.497382 vre_repository_connector-0.3.0/README.md
--rw-r--r--   0        0        0      815 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      351 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.0/vre_repository_connector/__init__.py
--rw-r--r--   0        0        0      201 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.0/vre_repository_connector/api/__init__.py
--rw-r--r--   0        0        0     2975 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.0/vre_repository_connector/api/base.py
--rw-r--r--   0        0        0    10248 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.0/vre_repository_connector/api/dbrepo.py
--rw-r--r--   0        0        0     6927 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.0/vre_repository_connector/api/inveniordm.py
--rw-r--r--   0        0        0     5567 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.0/vre_repository_connector/auto.py
--rw-r--r--   0        0        0     1131 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.0/vre_repository_connector/cli.py
--rw-r--r--   0        0        0      208 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.0/vre_repository_connector/utils.py
--rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 vre_repository_connector-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-31 13:15:46.462204 vre_repository_connector-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1314 2024-05-31 23:18:03.497382 vre_repository_connector-0.3.1/README.md
+-rw-r--r--   0        0        0      815 2024-06-02 21:57:46.056449 vre_repository_connector-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      351 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.1/vre_repository_connector/__init__.py
+-rw-r--r--   0        0        0      201 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.1/vre_repository_connector/api/__init__.py
+-rw-r--r--   0        0        0     3079 2024-06-02 21:57:46.056449 vre_repository_connector-0.3.1/vre_repository_connector/api/base.py
+-rw-r--r--   0        0        0    10395 2024-06-02 21:57:46.056449 vre_repository_connector-0.3.1/vre_repository_connector/api/dbrepo.py
+-rw-r--r--   0        0        0     7058 2024-06-02 21:57:46.056449 vre_repository_connector-0.3.1/vre_repository_connector/api/inveniordm.py
+-rw-r--r--   0        0        0     5567 2024-06-01 21:30:28.255277 vre_repository_connector-0.3.1/vre_repository_connector/auto.py
+-rw-r--r--   0        0        0     1305 2024-06-02 21:57:46.056449 vre_repository_connector-0.3.1/vre_repository_connector/cli.py
+-rw-r--r--   0        0        0      837 2024-06-02 21:57:46.056449 vre_repository_connector-0.3.1/vre_repository_connector/utils.py
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 vre_repository_connector-0.3.1/PKG-INFO
```

### Comparing `vre_repository_connector-0.3.0/LICENSE` & `vre_repository_connector-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.3.0/README.md` & `vre_repository_connector-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.3.0/pyproject.toml` & `vre_repository_connector-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "VRE-Repository-Connector"
-version = "0.3.0"
+version = "0.3.1"
 description = "Library for connecting the virtual research environment of TU Wien with its research data repositories"
 authors = ["Maximilian Moser <maximilian.moser@tuwien.ac.at>", "Sotirios Tsepelakis <sotirios.tsepelakis@tuwien.ac.at>", "Martin Weise <martin.weise@tuwien.ac.at>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.tuwien.ac.at/fairdata/vre-repository-connector"
 
 [tool.poetry.scripts]
```

### Comparing `vre_repository_connector-0.3.0/vre_repository_connector/api/base.py` & `vre_repository_connector-0.3.1/vre_repository_connector/api/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,7 +79,11 @@
         :param url: The URL from which to parse the container ID and file name.
         """
         return (None, None)
 
     def authenticate_interactive(self):
         """Shorthand for ``ask_credentials()`` into ``authenticate()``."""
         self.authenticate(**self.ask_credentials())
+
+    @property
+    def base_url(self) -> Optional[str]:
+        return getattr(self, "_base_url", None)
```

### Comparing `vre_repository_connector-0.3.0/vre_repository_connector/api/dbrepo.py` & `vre_repository_connector-0.3.1/vre_repository_connector/api/dbrepo.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     CreateTableColumn,
     CreateTableConstraints,
     DatatypeAnalysis,
 )
 from dbrepo.RestClient import RestClient
 from pandas import concat
 
-from ..utils import url_regex
+from ..utils import create_download_file, url_regex
 from .base import BaseWrapper
 
 db_tbl_regex = re.compile(r"(/api)?/database/([0-9]+)(/table/([0-9]+)(/.*)?)?")
 
 
 def columns_from_analysis(analysis: DatatypeAnalysis) -> List[CreateTableColumn]:
     """Turn the datatype analysis into a list of table column definitions."""
@@ -97,14 +97,15 @@
         """DBRepo constructor."""
         if match := url_regex.match(url):
             scheme, host = match.group(2) or "https", match.group(3)
             endpoint = f"{scheme}://{host}"
 
             logging.basicConfig(level=logging.WARNING)
             self.client = RestClient(endpoint=endpoint)
+            self._base_url = endpoint
 
         else:
             raise ValueError(f"Invalid DBRepo URL: {url}")
 
     def _create_database(self, name, container_id, is_public):
         """Create the database."""
         cdb = CreateDatabase(name=name, container_id=container_id, is_public=is_public)
@@ -286,10 +287,12 @@
             p += 1
 
         if data is None:
             return None
 
         # write the dataframe to a CSV file, with the columns in the same order
         # as they were uploaded, and without index column
-        name = f"{table_name}.csv"
-        data.to_csv(name, index=False, columns=[c.name for c in table.columns])
-        return name
+        file_path = create_download_file(
+            database_id, f"{table_name.rstrip('.csv')}.csv"
+        )
+        data.to_csv(file_path, index=False, columns=[c.name for c in table.columns])
+        return file_path
```

### Comparing `vre_repository_connector-0.3.0/vre_repository_connector/api/inveniordm.py` & `vre_repository_connector-0.3.1/vre_repository_connector/api/inveniordm.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 
 """Wrapper for InvenioRDM instances."""
 
 import getpass
 import os.path
 import pathlib
 import re
-import tempfile
 import urllib.parse
 from typing import Iterable, Optional, Tuple
 
 from inveniordm_py.client import InvenioAPI as InvenioRESTClient
 from inveniordm_py.files.metadata import FilesListMetadata, OutgoingStream
 from inveniordm_py.records.metadata import DraftMetadata
 from inveniordm_py.records.resources import Draft
 
-from ..utils import doi_regex, url_regex
+from ..utils import create_download_file, doi_regex, url_regex
 from .base import BaseWrapper
 
 recid_regex = re.compile(r"^.*(/api)?/records/(.*)$")
 recid_file_re = re.compile(r"(/api)?/records/([^/]+)(/files/([^/]+)(/content)?)?")
 
 
 class InvenioRDM(BaseWrapper):
@@ -38,14 +37,15 @@
             # Ensure the path in the URL starts with "/api",
             # as the InvenioAPI client can only fetch JSON
             if not parts.path.endswith("/api") and "/api/" not in parts.path:
                 parts = parts._replace(path="/api")
 
             self.url = urllib.parse.urlunparse(parts)
             self.client = InvenioRESTClient(base_url=self.url, access_token=api_token)
+            self._base_url = urllib.parse.urlunparse(parts._replace(path=""))
 
         else:
             raise ValueError(f"Invalid InvenioRDM URL: {url}")
 
     def ask_credentials(self):
         """Ask the user interactively for credentials."""
         print(f"(InvenioRDM) Enter your API token for '{self.url}'")
@@ -176,16 +176,16 @@
         """
         record = self.client.records(self._normalize_pid(record_pid))
 
         try:
             record.get()
             response = record.files(file_name).download()
 
-            with tempfile.NamedTemporaryFile(delete=False) as downloaded_file:
-
+            file_name = create_download_file(record_pid, file_name)
+            with open(file_name, "wb") as downloaded_file:
                 for chunk in response.iter_content(chunk_size=256):
                     downloaded_file.write(chunk)
 
             file_path = pathlib.Path(downloaded_file.name)
             return str(file_path)
 
         except Exception as e:
```

### Comparing `vre_repository_connector-0.3.0/vre_repository_connector/auto.py` & `vre_repository_connector-0.3.1/vre_repository_connector/auto.py`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.3.0/vre_repository_connector/cli.py` & `vre_repository_connector-0.3.1/vre_repository_connector/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # Copyright (C) 2024 TU Wien.
 #
 
 """CLI commands for the VRE Repository Connector."""
 
 import sys
+import urllib.parse
 
 import click
 
 from .auto import download, suggest_repository
 
 
 @click.group()
@@ -30,17 +31,19 @@
     "--select-interactive/--non-interactive",
     "-i/-I",
     default=True,
     help="Select the files to download interactively",
 )
 def download_files(url: str, all: bool, select_interactive: bool):
     """Download the files from the given URL."""
-    if suggest_repository(url) is None:
+    if (repo := suggest_repository(url)) is None:
         click.secho("Couldn't deduce a repository from the URL!", fg="red", err=True)
 
+    repo_type, host = type(repo).__name__, urllib.parse.urlparse(repo.base_url).netloc
+    click.echo(f"Downloading from {repo_type} @ {host}")
     files = download(url, all=all, interactive=select_interactive)
     if files is None:
         click.secho("No files downloaded.", fg="red", err=True)
         sys.exit(1)
 
     if isinstance(files, str):
         files = [files]
```

### Comparing `vre_repository_connector-0.3.0/PKG-INFO` & `vre_repository_connector-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VRE-Repository-Connector
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for connecting the virtual research environment of TU Wien with its research data repositories
 Home-page: https://gitlab.tuwien.ac.at/fairdata/vre-repository-connector
 License: MIT
 Author: Maximilian Moser
 Author-email: maximilian.moser@tuwien.ac.at
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
```

