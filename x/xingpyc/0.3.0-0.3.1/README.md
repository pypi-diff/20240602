# Comparing `tmp/xingpyc-0.3.0.tar.gz` & `tmp/xingpyc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.3.0.tar", last modified: Thu May 30 07:49:30 2024, max compression
+gzip compressed data, was "xingpyc-0.3.1.tar", last modified: Sun Jun  2 13:17:41 2024, max compression
```

## Comparing `xingpyc-0.3.0.tar` & `xingpyc-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:49:30.119393 xingpyc-0.3.0/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-30 07:49:30.119209 xingpyc-0.3.0/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.3.0/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-30 07:49:24.000000 xingpyc-0.3.0/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-30 07:49:30.119443 xingpyc-0.3.0/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:49:30.117451 xingpyc-0.3.0/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:49:30.118070 xingpyc-0.3.0/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)    11293 2024-05-30 07:49:08.000000 xingpyc-0.3.0/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.3.0/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:49:30.118991 xingpyc-0.3.0/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-30 07:49:30.000000 xingpyc-0.3.0/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-30 07:49:30.000000 xingpyc-0.3.0/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-30 07:49:30.000000 xingpyc-0.3.0/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-30 07:49:30.000000 xingpyc-0.3.0/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-30 07:49:30.000000 xingpyc-0.3.0/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:49:30.118857 xingpyc-0.3.0/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.3.0/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-06-02 13:17:41.171267 xingpyc-0.3.1/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-06-02 13:17:41.171046 xingpyc-0.3.1/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.3.1/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-06-02 13:17:35.000000 xingpyc-0.3.1/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-06-02 13:17:41.171308 xingpyc-0.3.1/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-06-02 13:17:41.168424 xingpyc-0.3.1/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-06-02 13:17:41.169736 xingpyc-0.3.1/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)    12788 2024-06-02 13:17:28.000000 xingpyc-0.3.1/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.3.1/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-06-02 13:17:41.170791 xingpyc-0.3.1/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-06-02 13:17:41.000000 xingpyc-0.3.1/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-06-02 13:17:41.000000 xingpyc-0.3.1/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-06-02 13:17:41.000000 xingpyc-0.3.1/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-06-02 13:17:41.000000 xingpyc-0.3.1/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-06-02 13:17:41.000000 xingpyc-0.3.1/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-06-02 13:17:41.170600 xingpyc-0.3.1/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.3.1/tests/test1.py
```

### Comparing `xingpyc-0.3.0/PKG-INFO` & `xingpyc-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.3.0
+Version: 0.3.1
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.3.0/pyproject.toml` & `xingpyc-0.3.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.3.0/src/xingpyc/__init__.py` & `xingpyc-0.3.1/src/xingpyc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 
 import time
 import numpy as np
 from threading import Thread
 from io import BytesIO
 import PIL.Image as Image
 
-
 def image_to_png_bytestring(image):
     png_bytestring = BytesIO()
     image.save(png_bytestring, format="PNG")
     png_bytestring.seek(0)
     return png_bytestring.getvalue()
 
 def image_to_webp_bytestring(image,quality=80):
     webp_bytestring = BytesIO()
     image.save(webp_bytestring, format="WEBP", quality=quality)
     webp_bytestring.seek(0)
     return webp_bytestring.getvalue()
 
+def write_progress(task_name, progress):
+    with open(f"progress/{task_name}", "w") as f:
+        f.write(progress)
+
 # Redirect sys.stdout to the custom stream
 class XClient:
     def __init__(self, funcs, mode: str, ip=None, portOrInfo=None):
         """
         init a ComClient with AI functions
         funcs: a list of AI functions
         """
@@ -43,14 +46,19 @@
             os.remove(f"tasks/{task}")
         # results folder is for placing results from various AI functions, no matter binded to XClient or not
         if not os.path.exists("results"):
             os.mkdir("results")
         results = os.listdir("results")
         for result in results:
             os.remove(f"results/{result}")
+        if not os.path.exists("progress"):
+            os.mkdir("progress")
+        progresses = os.listdir("progress")
+        for p in progresses:
+            os.remove(f"progress/{p}")
         # message loop
         asyncio.get_event_loop().create_task(self.message_loop())
 
         # listening
         if mode == "server":
             print(
                 "\033[93m Server started on " + ip + ":" + str(portOrInfo) + " \033[0m"
@@ -141,15 +149,35 @@
                                 + f"{client_id}.{task_id.decode()}.{header}"
                             )
                             f.write(content)
                         del self.blockbuffers[client_id]  # clean buffer
                 except Exception as e:
                     print(f"Error in websocket communication: {e}")
                     return
-                
+            
+            ### here starts the progress reporting
+            ### here starts the progress reporting
+            ### here starts the progress reporting
+            if len(os.listdir("progress")) > 0:
+                for task_id in os.listdir("progress"):
+                    try:
+                        progress_content = open(f"progress/{task_id}", "r").read()
+                        if len(task_id) != 10:
+                            raise "invalid task id length!!"
+                        task_id_byte = task_id.encode("utf-8")
+                        progress_content = progress_content.encode("utf-8")
+                        if client_id == -1:
+                            print("start sending progress to cloud")
+                            self.cloudClient.send_bytes(b"progress  " + task_id_byte + progress_content)
+                            print("sent progress to cloud")
+                        else:
+                            await websocket.send(b"progress  " + task_id_byte + progress_content)
+                        os.remove(f"progress/{task_id}")
+                    except Exception as e:
+                        print(f"Error in sending message to websocket: {e}")
 
             ### here starts the result sending
             ### here starts the result sending
             ### here starts the result sending
             if len(os.listdir("results")) > 0:
                 for file in os.listdir("results"):
                     try:
```

### Comparing `xingpyc-0.3.0/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.3.1/src/xingpyc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.3.0
+Version: 0.3.1
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

