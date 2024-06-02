# Comparing `tmp/httpexec-1.0.2.tar.gz` & `tmp/httpexec-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpexec-1.0.2.tar", last modified: Mon Nov 27 20:08:03 2023, max compression
+gzip compressed data, was "httpexec-1.0.3.tar", last modified: Sun Jun  2 18:43:36 2024, max compression
```

## Comparing `httpexec-1.0.2.tar` & `httpexec-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 20:08:03.288216 httpexec-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-11-27 20:07:25.000000 httpexec-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14425 2023-11-27 20:08:03.288216 httpexec-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11484 2023-11-27 20:07:25.000000 httpexec-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2023-11-27 20:07:25.000000 httpexec-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 20:08:03.288216 httpexec-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 20:08:03.284216 httpexec-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 20:08:03.284216 httpexec-1.0.2/src/httpexec/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-27 20:07:25.000000 httpexec-1.0.2/src/httpexec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-11-27 20:07:25.000000 httpexec-1.0.2/src/httpexec/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2023-11-27 20:07:25.000000 httpexec-1.0.2/src/httpexec/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 20:08:03.284216 httpexec-1.0.2/src/httpexec/etc/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-27 20:07:25.000000 httpexec-1.0.2/src/httpexec/etc/defaults.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 20:08:03.284216 httpexec-1.0.2/src/httpexec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14425 2023-11-27 20:08:03.000000 httpexec-1.0.2/src/httpexec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-11-27 20:08:03.000000 httpexec-1.0.2/src/httpexec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 20:08:03.000000 httpexec-1.0.2/src/httpexec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-11-27 20:08:03.000000 httpexec-1.0.2/src/httpexec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-27 20:08:03.000000 httpexec-1.0.2/src/httpexec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:43:36.480793 httpexec-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-06-02 18:43:12.000000 httpexec-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14425 2024-06-02 18:43:36.480793 httpexec-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-06-02 18:43:12.000000 httpexec-1.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-06-02 18:43:12.000000 httpexec-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:43:36.480793 httpexec-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:43:36.476793 httpexec-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:43:36.480793 httpexec-1.0.3/src/httpexec/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-02 18:43:12.000000 httpexec-1.0.3/src/httpexec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-06-02 18:43:12.000000 httpexec-1.0.3/src/httpexec/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-06-02 18:43:12.000000 httpexec-1.0.3/src/httpexec/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:43:36.480793 httpexec-1.0.3/src/httpexec/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-02 18:43:12.000000 httpexec-1.0.3/src/httpexec/etc/defaults.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:43:36.480793 httpexec-1.0.3/src/httpexec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14425 2024-06-02 18:43:36.000000 httpexec-1.0.3/src/httpexec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-06-02 18:43:36.000000 httpexec-1.0.3/src/httpexec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:43:36.000000 httpexec-1.0.3/src/httpexec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-02 18:43:36.000000 httpexec-1.0.3/src/httpexec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 18:43:36.000000 httpexec-1.0.3/src/httpexec.egg-info/top_level.txt
```

### Comparing `httpexec-1.0.2/LICENSE` & `httpexec-1.0.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022-2023, Michael Klatt
+Copyright (c) 2022-2024, Michael Klatt
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `httpexec-1.0.2/PKG-INFO` & `httpexec-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: httpexec
-Version: 1.0.2
+Version: 1.0.3
 Summary: Execute CLI commands via a REST API.
 Author-email: Michael Klatt <mdklatt@alumni.ou.edu>
 License: The MIT License (MIT)
         
-        Copyright (c) 2022-2023, Michael Klatt
+        Copyright (c) 2022-2024, Michael Klatt
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `httpexec-1.0.2/README.rst` & `httpexec-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `httpexec-1.0.2/pyproject.toml` & `httpexec-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `httpexec-1.0.2/src/httpexec/__version__.py` & `httpexec-1.0.3/src/httpexec/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 internal code changes that do not affect the API. Development versions are
 incomplete states of a release .
 
 Version 0.x should be considered a development version with an unstable API,
 and backwards compatibility is not guaranteed for minor versions.
 
 """
-__version__ = "1.0.2"
+__version__ = "1.0.3"
```

### Comparing `httpexec-1.0.2/src/httpexec/asgi.py` & `httpexec-1.0.3/src/httpexec/asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     argv = [str(command)] + params.get("args", [])
     streams = {key: params.get(key, {}) for key in ("stdin", "stderr", "stdout")}
     env = params.get("environment", {})
     result = await _exec(argv, streams, env)
     return jsonify(result)
 
 
-async def _exec(argv: Sequence, streams: dict, env: dict) -> dict:
+async def _exec(argv: Sequence, streams: dict, env: dict | None) -> dict:
     """  Execute a command on the host.
 
     STDIN is decoded if necessary before executing the command, and STDERR
     and STDOUT are encoded for transmission back to the client.
 
     :param argv: command line arguments
     :param streams: STDIN, STDERR, and STDOUT parameters
@@ -128,15 +128,15 @@
         pipes["stdin"] = PIPE
         scheme = streams["stdin"].get("encode")
         if scheme is None:
             stdin = stdin.encode()
         else:
             decode = _encoding_schemes[scheme][1]
             stdin = decode(stdin)
-    env = environ | env  # update parent environment
+    env = environ | (env or {})  # update parent environment
     process = await create_subprocess_exec(*argv, **pipes, env=env)
     output = dict(zip(("stdout", "stderr"), await process.communicate(stdin)))
     for key, content in output.items():
         if content is None:
             continue
         scheme = streams[key].get("encode")
         if scheme is not None:
```

### Comparing `httpexec-1.0.2/src/httpexec.egg-info/PKG-INFO` & `httpexec-1.0.3/src/httpexec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: httpexec
-Version: 1.0.2
+Version: 1.0.3
 Summary: Execute CLI commands via a REST API.
 Author-email: Michael Klatt <mdklatt@alumni.ou.edu>
 License: The MIT License (MIT)
         
-        Copyright (c) 2022-2023, Michael Klatt
+        Copyright (c) 2022-2024, Michael Klatt
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

