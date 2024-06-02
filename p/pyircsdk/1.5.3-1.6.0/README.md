# Comparing `tmp/pyircsdk-1.5.3.tar.gz` & `tmp/pyircsdk-1.6.0.tar.gz`

## Comparing `pyircsdk-1.5.3.tar` & `pyircsdk-1.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/__about__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/__init__.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/command.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/message.py
--rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/pyircsdk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/event/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyircsdk/event/event.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/LICENSE
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/README.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/pyircsdk/__about__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/pyircsdk/__init__.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/pyircsdk/command.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/pyircsdk/message.py
+-rw-r--r--   0        0        0     9290 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/pyircsdk/pyircsdk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/pyircsdk/event/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/pyircsdk/event/event.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/README.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 pyircsdk-1.6.0/PKG-INFO
```

### Comparing `pyircsdk-1.5.3/pyircsdk/command.py` & `pyircsdk-1.6.0/pyircsdk/command.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.3/pyircsdk/message.py` & `pyircsdk-1.6.0/pyircsdk/message.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.3/pyircsdk/pyircsdk.py` & `pyircsdk-1.6.0/pyircsdk/pyircsdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 @dataclass
 class IRCSDKConfig:
     host: str
     port: int
     nick: str
     channel: str
+    channels: list[str]
     user: str
     realname: str
     password: str
     ssl: bool
     nickservFormat: str
     nickservPassword: str
     nodataTimeout: int
@@ -98,17 +99,20 @@
                 self.event.on('raw', self.handle_raw_message)
                 if self.config.password:
                     self.sendPassword(self.config.password)
 
                 self.setUser(self.config.user, self.config.realname)
                 self.setNick(self.config.nick)
 
-                self.event.on('connected', lambda data: self.nickServIdentify(self.config.nickservFormat,
-                                                                              self.config.nickservPassword))
-                self.event.on('connected', lambda data: self.join(self.config.channel))
+                self.event.on('connected', lambda data: self.nickServIdentify(self.config.nickservFormat, self.config.nickservPassword))
+                if self.config.channels:
+                    self.event.on('connected', lambda data: [self.join(channel) for channel in self.config.channels])
+                else:
+                    self.event.on('connected', lambda data: self.join(self.config.channel))
+
                 self.startRecv()
                 break
             except socket.error as e:
                 print(f"Connection failed: {e}")
                 self.irc.close()  # Make sure to close the socket on failure
                 if attempt < retries - 1:
                     print(f"Waiting for {wait_secs} seconds before retrying...")
```

### Comparing `pyircsdk-1.5.3/pyircsdk/event/event.py` & `pyircsdk-1.6.0/pyircsdk/event/event.py`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.3/.gitignore` & `pyircsdk-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.3/LICENSE` & `pyircsdk-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.3/README.md` & `pyircsdk-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyircsdk-1.5.3/pyproject.toml` & `pyircsdk-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "pyircsdk"
 authors = [
   { name="Bludot", email="admin@floretos.com" },
 ]
-version = "1.5.3"
+version = "1.6.0"
 description = "pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyircsdk-1.5.3/PKG-INFO` & `pyircsdk-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyircsdk
-Version: 1.5.3
+Version: 1.6.0
 Summary: pyIRCSDK is a Python library for creating IRC bots and clients. It is designed to provide granular access to raw mesages and to provide an event emitter like interface for handling messages.
 Project-URL: Homepage, https://github.com/bludot/pyircsdk
 Project-URL: Issues, https://github.com/bludot/pyircsdk/issues
 Author-email: Bludot <admin@floretos.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

