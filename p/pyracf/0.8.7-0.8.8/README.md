# Comparing `tmp/pyracf-0.8.7.tar.gz` & `tmp/pyracf-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.8.7.tar", last modified: Sun Apr 28 08:56:34 2024, max compression
+gzip compressed data, was "pyracf-0.8.8.tar", last modified: Mon Apr 29 13:44:26 2024, max compression
```

## Comparing `pyracf-0.8.7.tar` & `pyracf-0.8.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-28 08:56:34.120563 pyracf-0.8.7/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2024-04-21 09:03:17.000000 pyracf-0.8.7/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2024-04-21 09:03:17.000000 pyracf-0.8.7/MANIFEST.in
--rw-r--r--   0 henri     (1000) henri     (1000)    17335 2024-04-28 08:56:34.116563 pyracf-0.8.7/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)    16727 2024-04-28 08:25:21.000000 pyracf-0.8.7/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)      161 2024-04-21 09:03:17.000000 pyracf-0.8.7/pyproject.toml
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-28 08:56:34.120563 pyracf-0.8.7/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-28 08:19:24.000000 pyracf-0.8.7/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-28 08:56:34.116563 pyracf-0.8.7/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-28 08:56:34.116563 pyracf-0.8.7/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    62293 2024-04-28 08:42:05.000000 pyracf-0.8.7/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-21 09:03:17.000000 pyracf-0.8.7/src/pyracf/getOffsets.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-21 09:03:17.000000 pyracf-0.8.7/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-28 08:56:34.116563 pyracf-0.8.7/src/pyracf.egg-info/
--rw-r--r--   0 henri     (1000) henri     (1000)    17335 2024-04-28 08:56:34.000000 pyracf-0.8.7/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      412 2024-04-28 08:56:34.000000 pyracf-0.8.7/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-28 08:56:34.000000 pyracf-0.8.7/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-28 08:56:34.000000 pyracf-0.8.7/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-28 08:56:34.000000 pyracf-0.8.7/src/pyracf.egg-info/top_level.txt
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-28 08:56:34.116563 pyracf-0.8.7/test/
--rw-rw-r--   0 henri     (1000) henri     (1000)      794 2024-04-21 09:03:17.000000 pyracf-0.8.7/test/test_connect_df.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     1461 2024-04-21 09:03:17.000000 pyracf-0.8.7/test/test_frame_dataset.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     1504 2024-04-21 09:03:17.000000 pyracf-0.8.7/test/test_frame_general.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     6654 2024-04-21 09:03:17.000000 pyracf-0.8.7/test/test_frames.py
--rw-rw-r--   0 henri     (1000) henri     (1000)      466 2024-04-21 09:03:17.000000 pyracf-0.8.7/test/test_parsed.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-29 13:44:26.026422 pyracf-0.8.8/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2024-04-21 09:03:17.000000 pyracf-0.8.8/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2024-04-21 09:03:17.000000 pyracf-0.8.8/MANIFEST.in
+-rw-r--r--   0 henri     (1000) henri     (1000)    17335 2024-04-29 13:44:26.026422 pyracf-0.8.8/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)    16727 2024-04-29 13:42:11.000000 pyracf-0.8.8/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)      161 2024-04-21 09:03:17.000000 pyracf-0.8.8/pyproject.toml
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-29 13:44:26.026422 pyracf-0.8.8/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-29 13:43:39.000000 pyracf-0.8.8/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-29 13:44:26.026422 pyracf-0.8.8/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-29 13:44:26.026422 pyracf-0.8.8/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    62293 2024-04-29 13:43:17.000000 pyracf-0.8.8/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-21 09:03:17.000000 pyracf-0.8.8/src/pyracf/getOffsets.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-21 09:03:17.000000 pyracf-0.8.8/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-29 13:44:26.026422 pyracf-0.8.8/src/pyracf.egg-info/
+-rw-r--r--   0 henri     (1000) henri     (1000)    17335 2024-04-29 13:44:26.000000 pyracf-0.8.8/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      412 2024-04-29 13:44:26.000000 pyracf-0.8.8/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-29 13:44:26.000000 pyracf-0.8.8/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-29 13:44:26.000000 pyracf-0.8.8/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-29 13:44:26.000000 pyracf-0.8.8/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-29 13:44:26.026422 pyracf-0.8.8/test/
+-rw-rw-r--   0 henri     (1000) henri     (1000)      794 2024-04-21 09:03:17.000000 pyracf-0.8.8/test/test_connect_df.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1461 2024-04-21 09:03:17.000000 pyracf-0.8.8/test/test_frame_dataset.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1504 2024-04-21 09:03:17.000000 pyracf-0.8.8/test/test_frame_general.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     6654 2024-04-21 09:03:17.000000 pyracf-0.8.8/test/test_frames.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)      466 2024-04-21 09:03:17.000000 pyracf-0.8.8/test/test_parsed.py
```

### Comparing `pyracf-0.8.7/LICENSE` & `pyracf-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.7/PKG-INFO` & `pyracf-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.7
+Version: 0.8.8
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyracf-0.8.7/README.md` & `pyracf-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.7/setup.py` & `pyracf-0.8.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.8.7",
+    version="0.8.8",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.8.7/src/pyracf/__init__.py` & `pyracf-0.8.8/src/pyracf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,23 +389,23 @@
             status = "Limbo"     
         return {'status': status, 'input-lines': self._unloadlines, 'lines-read': seen, 'lines-parsed': parsed, 'lines-per-second': speed, 'parse-time': parsetime}
 
     def parse_fancycli(self, recordtypes=_recordtype_info.keys(), save_pickles=False, prefix=''):
         print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - parsing {self._irrdbu00}')
         self.parse(recordtypes=recordtypes)
         print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - selected recordtypes: {",".join(recordtypes)}')
-        while self._state != self.STATE_CORRELATING:
+        while self._state <= self.STATE_CORRELATING:
             progress =  math.floor(((sum(r['seen'] for r in self._records.values() if r)) / self._unloadlines) * 63)
             pct = (progress/63) * 100 # not as strange as it seems:)
             done = progress * '▉'
             todo = (63-progress) * ' '
             print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - progress: {done}{todo} ({pct:.2f}%)'.center(80), end="\r")
             time.sleep(0.5)
         print('')
-        while self._state != self.STATE_READY:
+        while self._state <= self.STATE_READY:
              print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - correlating data {40*" "}', end="\r")
              time.sleep(0.5)
         # make completed line always show 100% :)
         print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - progress: {63*"▉"} ({100:.2f}%)'.center(80))
         for r in recordtypes:
             print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - recordtype {r} -> {self.parsed(self._recordtype_info[r]["name"])} records parsed')
         print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - total parse time: {(self._stoptime - self._starttime).total_seconds()} seconds')
```

### Comparing `pyracf-0.8.7/src/pyracf/getOffsets.py` & `pyracf-0.8.8/src/pyracf/getOffsets.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.7/src/pyracf/offsets.json` & `pyracf-0.8.8/src/pyracf/offsets.json`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.7/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.8.8/src/pyracf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.7
+Version: 0.8.8
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyracf-0.8.7/test/test_connect_df.py` & `pyracf-0.8.8/test/test_connect_df.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.7/test/test_frame_dataset.py` & `pyracf-0.8.8/test/test_frame_dataset.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.7/test/test_frame_general.py` & `pyracf-0.8.8/test/test_frame_general.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.7/test/test_frames.py` & `pyracf-0.8.8/test/test_frames.py`

 * *Files identical despite different names*

