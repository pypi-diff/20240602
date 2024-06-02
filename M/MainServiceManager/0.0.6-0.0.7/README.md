# Comparing `tmp/mainservicemanager-0.0.6.tar.gz` & `tmp/mainservicemanager-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainservicemanager-0.0.6.tar", max compression
+gzip compressed data, was "mainservicemanager-0.0.7.tar", max compression
```

## Comparing `mainservicemanager-0.0.6.tar` & `mainservicemanager-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.6/README.md
--rwxr-xr-x   0        0        0      736 2024-06-01 11:28:18.000000 mainservicemanager-0.0.6/pyproject.toml
--rwxr-xr-x   0        0        0      391 2024-06-01 11:28:12.000000 mainservicemanager-0.0.6/src/MainServiceManager/__init__.py
--rwxr-xr-x   0        0        0     4291 2024-06-01 11:23:27.000000 mainservicemanager-0.0.6/src/MainServiceManager/__main__.py
--rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.6/src/MainServiceManager/api.py
--rwxr-xr-x   0        0        0     7214 2024-06-01 08:54:08.000000 mainservicemanager-0.0.6/src/MainServiceManager/server.py
--rwxr-xr-x   0        0        0     6876 2024-06-01 09:36:36.000000 mainservicemanager-0.0.6/src/MainServiceManager/server_utils.py
--rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.7/README.md
+-rwxr-xr-x   0        0        0      736 2024-06-02 10:53:38.000000 mainservicemanager-0.0.7/pyproject.toml
+-rwxr-xr-x   0        0        0      391 2024-06-02 10:53:32.000000 mainservicemanager-0.0.7/src/MainServiceManager/__init__.py
+-rwxr-xr-x   0        0        0     4291 2024-06-01 11:23:26.000000 mainservicemanager-0.0.7/src/MainServiceManager/__main__.py
+-rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.7/src/MainServiceManager/api.py
+-rwxr-xr-x   0        0        0     7214 2024-06-01 08:54:08.000000 mainservicemanager-0.0.7/src/MainServiceManager/server.py
+-rwxr-xr-x   0        0        0     7419 2024-06-02 09:54:48.000000 mainservicemanager-0.0.7/src/MainServiceManager/server_utils.py
+-rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.7/PKG-INFO
```

### Comparing `mainservicemanager-0.0.6/README.md` & `mainservicemanager-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.6/pyproject.toml` & `mainservicemanager-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MainServiceManager"
-version = "0.0.6"
+version = "0.0.7"
 description = "Пользовательская программа для управления сервисами, аналогично systemd"
 authors = ["MainPlay TG <xbox.roman6666666666@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainServiceManager.py"
 packages = [
 { include = "MainServiceManager", from = "src" },
 ]
```

### Comparing `mainservicemanager-0.0.6/src/MainServiceManager/__main__.py` & `mainservicemanager-0.0.7/src/MainServiceManager/__main__.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.6/src/MainServiceManager/api.py` & `mainservicemanager-0.0.7/src/MainServiceManager/api.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.6/src/MainServiceManager/server.py` & `mainservicemanager-0.0.7/src/MainServiceManager/server.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.6/src/MainServiceManager/server_utils.py` & `mainservicemanager-0.0.7/src/MainServiceManager/server_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,28 +35,36 @@
       else:
         self.password=password
       try:
         self.read()
       except:
         self.close()
   def read(self,**kw):
+    if self.name=="admin":
+      return
     kw["path"]=self.path
     self.data=ms.json.read(**kw)
   def write(self,**kw):
+    if self.name=="admin":
+      return
     if not "mode" in kw:
       kw["mode"]="p"
     kw["data"]=self.data
     kw["path"]=self.path
     return ms.json.write(**kw)
   def reload(self):
+    if self.name=="admin":
+      return
     try:
       self.read()
     except:
       self.close()
   def close(self,kill:bool=False):
+    if self.name=="admin":
+      return
     while self.process:
       if kill:
         self.kill()
       else:
         self.stop()
         sleep(10)
         self.kill()
@@ -64,14 +72,16 @@
       if not k.startswith("__"):
         try:
           delattr(self,k)
         except:
           pass
     self.closed=True
   def enable(self,*,threaded=False):
+    if self.name=="admin":
+      return
     if self.process:
       return
     if not threaded:
       return Thread(target=self.enable,kwargs={"threaded":True}).start()
     self.enabled=True
     self.start(threaded=True)
     self.code=self.process.wait()
@@ -82,26 +92,30 @@
     if self["restart"]=="always":
       return self(threaded=True)
     if self["restart"]=="on_error":
       if self.code!=0:
         return self(threaded=True)
     self.enabled=False
   def disable(self):
+    if self.name=="admin":
+      return
     if self.enabled:
       self.enabled=False
       self.stop()
   def __call__(self,*args,**kw):
     return self.enable(*args,**kw)
   def __getitem__(self,k):
     return self.data.get(k)
   def __setitem__(self,k,v):
     self.data[k]=v
   def __hasitem__(self,k):
     return k in self.data
   def start(self,threaded=False,**kw):
+    if self.name=="admin":
+      return
     if self.process:
       return
     if not threaded:
       return Thread(target=self.start,kwargs={"threaded":True}).start()
     kw["args"]=self.data["args"]
     kw["stderr"]=subprocess.DEVNULL
     kw["stdin"]=subprocess.DEVNULL
@@ -124,27 +138,39 @@
       if hasattr(os,"setgroups"):
         kw["extra_groups"]=self["extra_groups"]
     self.process=subprocess.Popen(**kw)
     self.pid=self.process.pid
     if self["data_path"]:
       ms.json.write(self["data_path"],self.to_dict())
   def restart(self,kill=False):
+    if self.name=="admin":
+      return
+    if self.enabled:
+      self.enabled=False
+      enable=True
     while self.process:
       if kill:
         self.kill()
       else:
         self.stop()
-    self.start()
+    if enable:
+      self.enable()
+    else:
+      self.start()
   def send_signal(self,sig:int):
+    if self.name=="admin":
+      return
     if self.process:
       self.process.send_signal(sig)
   def stop(self):
     self.send_signal(signal.SIGINT)
+    self.enabled=False
   def kill(self):
     self.send_signal(signal.SIGKILL)
+    self.enabled=False
   def to_dict(self)->dict:
     return {"name":self.name,"path":self.path,"pid":self.pid,"password":self.password,"data":self.data}
   def to_json(self,**kw)->str:
     return ms.json.encode(self.to_dict(),**kw)
 def cfg_load(path:str=os.path.expanduser("~/.config/MainServiceManager/cfg.json"))->ms.cfg:
   cfg=ms.cfg(path,type="json")
   cfg.default={
```

### Comparing `mainservicemanager-0.0.6/PKG-INFO` & `mainservicemanager-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MainServiceManager
-Version: 0.0.6
+Version: 0.0.7
 Summary: Пользовательская программа для управления сервисами, аналогично systemd
 Home-page: https://github.com/MainPlay-TG/MainServiceManager.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

