# Comparing `tmp/api_pipe-2.0.23.tar.gz` & `tmp/api_pipe-2.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_pipe-2.0.23.tar", max compression
+gzip compressed data, was "api_pipe-2.0.24.tar", max compression
```

## Comparing `api_pipe-2.0.23.tar` & `api_pipe-2.0.24.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       80 2024-05-30 05:39:30.477389 api_pipe-2.0.23/README.md
--rw-r--r--   0        0        0      561 2024-05-30 05:28:01.000000 api_pipe-2.0.23/pyproject.toml
--rw-r--r--   0        0        0       69 2024-05-30 05:28:01.000000 api_pipe-2.0.23/src/api_pipe/__init__.py
--rw-r--r--   0        0        0     8504 2024-05-30 05:39:30.478389 api_pipe-2.0.23/src/api_pipe/api.py
--rw-r--r--   0        0        0      827 2024-05-30 05:39:30.478389 api_pipe-2.0.23/src/api_pipe/config.py
--rw-r--r--   0        0        0      555 2024-05-30 05:39:30.478389 api_pipe-2.0.23/src/api_pipe/directory.py
--rw-r--r--   0        0        0     1577 2024-05-30 05:39:30.478389 api_pipe-2.0.23/src/api_pipe/error.py
--rw-r--r--   0        0        0     1491 2024-05-30 05:39:30.478389 api_pipe-2.0.23/src/api_pipe/logger.py
--rw-r--r--   0        0        0     3200 2024-05-30 05:39:30.478389 api_pipe-2.0.23/src/api_pipe/manual_test_run.py
--rw-r--r--   0        0        0     3570 2024-05-30 05:39:30.478389 api_pipe-2.0.23/src/api_pipe/params.py
--rw-r--r--   0        0        0     1056 2024-05-30 05:39:30.478389 api_pipe-2.0.23/src/api_pipe/params_schema.py
--rw-r--r--   0        0        0        3 2024-05-30 05:39:30.478389 api_pipe-2.0.23/src/api_pipe/steps/__init__.py
--rw-r--r--   0        0        0     2117 2024-05-30 05:39:30.478389 api_pipe-2.0.23/src/api_pipe/steps/fetch.py
--rw-r--r--   0        0        0     1900 2024-05-30 05:39:30.478389 api_pipe-2.0.23/src/api_pipe/steps/fetch_async.py
--rw-r--r--   0        0        0     1002 2024-05-30 05:39:30.479389 api_pipe-2.0.23/src/api_pipe/steps/filter.py
--rw-r--r--   0        0        0      649 2024-05-30 05:39:30.479389 api_pipe-2.0.23/src/api_pipe/steps/key.py
--rw-r--r--   0        0        0     1237 2024-05-30 05:39:30.479389 api_pipe-2.0.23/src/api_pipe/steps/map.py
--rw-r--r--   0        0        0      913 2024-05-30 05:39:30.479389 api_pipe-2.0.23/src/api_pipe/steps/select.py
--rw-r--r--   0        0        0      507 2024-05-30 05:39:30.479389 api_pipe-2.0.23/src/api_pipe/steps/to_json.py
--rw-r--r--   0        0        0      738 2024-05-30 05:39:30.479389 api_pipe-2.0.23/src/api_pipe/steps/to_python.py
--rw-r--r--   0        0        0      721 2024-05-30 05:39:30.479389 api_pipe-2.0.23/src/api_pipe/url.py
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 api_pipe-2.0.23/PKG-INFO
+-rw-r--r--   0        0        0       80 2024-06-02 01:16:04.619835 api_pipe-2.0.24/README.md
+-rw-r--r--   0        0        0      591 2024-06-02 01:11:17.000000 api_pipe-2.0.24/pyproject.toml
+-rw-r--r--   0        0        0      797 2024-06-02 01:11:17.000000 api_pipe-2.0.24/src/api_pipe/__init__.py
+-rw-r--r--   0        0        0     9232 2024-06-02 01:16:04.620835 api_pipe-2.0.24/src/api_pipe/api.py
+-rw-r--r--   0        0        0     1555 2024-06-02 01:16:04.620835 api_pipe-2.0.24/src/api_pipe/config.py
+-rw-r--r--   0        0        0     1284 2024-06-02 01:16:04.620835 api_pipe-2.0.24/src/api_pipe/directory.py
+-rw-r--r--   0        0        0     2305 2024-06-02 01:16:04.620835 api_pipe-2.0.24/src/api_pipe/error.py
+-rw-r--r--   0        0        0     2218 2024-06-02 01:16:04.620835 api_pipe-2.0.24/src/api_pipe/logger.py
+-rw-r--r--   0        0        0     3929 2024-06-02 01:16:04.621836 api_pipe-2.0.24/src/api_pipe/manual_test_run.py
+-rw-r--r--   0        0        0     4297 2024-06-02 01:16:04.621836 api_pipe-2.0.24/src/api_pipe/params.py
+-rw-r--r--   0        0        0     1784 2024-06-02 01:16:04.621836 api_pipe-2.0.24/src/api_pipe/params_schema.py
+-rw-r--r--   0        0        0      727 2024-06-02 01:16:04.621836 api_pipe-2.0.24/src/api_pipe/steps/__init__.py
+-rw-r--r--   0        0        0     2845 2024-06-02 01:16:04.621836 api_pipe-2.0.24/src/api_pipe/steps/fetch.py
+-rw-r--r--   0        0        0     2628 2024-06-02 01:16:04.621836 api_pipe-2.0.24/src/api_pipe/steps/fetch_async.py
+-rw-r--r--   0        0        0     1730 2024-06-02 01:16:04.621836 api_pipe-2.0.24/src/api_pipe/steps/filter.py
+-rw-r--r--   0        0        0     1377 2024-06-02 01:16:04.621836 api_pipe-2.0.24/src/api_pipe/steps/key.py
+-rw-r--r--   0        0        0     1965 2024-06-02 01:16:04.621836 api_pipe-2.0.24/src/api_pipe/steps/map.py
+-rw-r--r--   0        0        0     1641 2024-06-02 01:16:04.621836 api_pipe-2.0.24/src/api_pipe/steps/select.py
+-rw-r--r--   0        0        0     1235 2024-06-02 01:16:04.622835 api_pipe-2.0.24/src/api_pipe/steps/to_json.py
+-rw-r--r--   0        0        0     1466 2024-06-02 01:16:04.622835 api_pipe-2.0.24/src/api_pipe/steps/to_python.py
+-rw-r--r--   0        0        0     1449 2024-06-02 01:16:04.622835 api_pipe-2.0.24/src/api_pipe/url.py
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 api_pipe-2.0.24/PKG-INFO
```

### Comparing `api_pipe-2.0.23/src/api_pipe/api.py` & `api_pipe-2.0.24/src/api_pipe/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# Copyright (C) 2024 RomanLabs, Rafael Roman Otero
+# This file is part of API Pipe.
+#
+# API Pipe is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Lesser General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# API Pipe is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+# GNU Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public License
+# along with API Pipe. If not, see <http://www.gnu.org/licenses/>.
+
 '''
     API
 '''
 import httpx
 import itertools
 from typing import Any
 import json
```

### Comparing `api_pipe-2.0.23/src/api_pipe/steps/fetch.py` & `api_pipe-2.0.24/src/api_pipe/steps/fetch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# Copyright (C) 2024 RomanLabs, Rafael Roman Otero
+# This file is part of API Pipe.
+#
+# API Pipe is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Lesser General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# API Pipe is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+# GNU Lesser General Public License for more details.
+#
+# You should have received a copy of the GNU Lesser General Public License
+# along with API Pipe. If not, see <http://www.gnu.org/licenses/>.
+
 '''
     Step Fetch
 '''
 import json
 import time
 import httpx
 from httpx import Response
```

