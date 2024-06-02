# Comparing `tmp/coders-utils-0.0.1.tar.gz` & `tmp/coders-utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coders-utils-0.0.1.tar", last modified: Wed May 29 04:14:27 2024, max compression
+gzip compressed data, was "coders-utils-0.0.2.tar", last modified: Sun Jun  2 03:29:51 2024, max compression
```

## Comparing `coders-utils-0.0.1.tar` & `coders-utils-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-05-29 04:14:27.371842 coders-utils-0.0.1/
--rwxr-xr-x   0 parzival  (1000) parzival  (1000)     1070 2023-02-08 04:36:20.000000 coders-utils-0.0.1/LICENSE
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      567 2024-05-29 04:14:27.371842 coders-utils-0.0.1/PKG-INFO
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      175 2024-05-29 04:12:09.000000 coders-utils-0.0.1/README.md
-drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-05-29 04:14:27.371842 coders-utils-0.0.1/coders_utils/
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      225 2024-05-29 04:12:44.000000 coders-utils-0.0.1/coders_utils/__init__.py
--rw-rw-r--   0 parzival  (1000) parzival  (1000)     2241 2024-05-29 04:08:52.000000 coders-utils-0.0.1/coders_utils/file_iterators.py
--rw-rw-r--   0 parzival  (1000) parzival  (1000)     3588 2024-05-29 04:01:38.000000 coders-utils-0.0.1/coders_utils/find_utils.py
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      557 2024-05-29 04:08:46.000000 coders-utils-0.0.1/coders_utils/linux_admin_ops.py
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      795 2024-05-29 03:52:38.000000 coders-utils-0.0.1/coders_utils/shell.py
-drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-05-29 04:14:27.371842 coders-utils-0.0.1/coders_utils.egg-info/
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      567 2024-05-29 04:14:27.000000 coders-utils-0.0.1/coders_utils.egg-info/PKG-INFO
--rw-rw-r--   0 parzival  (1000) parzival  (1000)      342 2024-05-29 04:14:27.000000 coders-utils-0.0.1/coders_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 parzival  (1000) parzival  (1000)        1 2024-05-29 04:14:27.000000 coders-utils-0.0.1/coders_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 parzival  (1000) parzival  (1000)        9 2024-05-29 04:14:27.000000 coders-utils-0.0.1/coders_utils.egg-info/requires.txt
--rw-rw-r--   0 parzival  (1000) parzival  (1000)       13 2024-05-29 04:14:27.000000 coders-utils-0.0.1/coders_utils.egg-info/top_level.txt
--rw-rw-r--   0 parzival  (1000) parzival  (1000)       38 2024-05-29 04:14:27.371842 coders-utils-0.0.1/setup.cfg
--rwxr-xr-x   0 parzival  (1000) parzival  (1000)      737 2024-05-29 04:10:48.000000 coders-utils-0.0.1/setup.py
+drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-06-02 03:29:51.289822 coders-utils-0.0.2/
+-rwxr-xr-x   0 parzival  (1000) parzival  (1000)     1070 2023-02-08 04:36:20.000000 coders-utils-0.0.2/LICENSE
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      567 2024-06-02 03:29:51.289822 coders-utils-0.0.2/PKG-INFO
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      175 2024-05-29 04:12:09.000000 coders-utils-0.0.2/README.md
+drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-06-02 03:29:51.289822 coders-utils-0.0.2/coders_utils/
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      427 2024-06-02 03:29:12.000000 coders-utils-0.0.2/coders_utils/__init__.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)     2143 2024-06-01 18:35:09.000000 coders-utils-0.0.2/coders_utils/codecs.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)     3526 2024-06-01 19:03:14.000000 coders-utils-0.0.2/coders_utils/cyber_utils.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)     4716 2024-06-01 21:40:40.000000 coders-utils-0.0.2/coders_utils/date_utils.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)     5072 2024-06-02 03:13:35.000000 coders-utils-0.0.2/coders_utils/file_handlers.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)     2908 2024-06-01 18:55:58.000000 coders-utils-0.0.2/coders_utils/identifiers.py
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)     3723 2024-06-02 03:17:26.000000 coders-utils-0.0.2/coders_utils/regex_manager.py
+drwxrwxr-x   0 parzival  (1000) parzival  (1000)        0 2024-06-02 03:29:51.289822 coders-utils-0.0.2/coders_utils.egg-info/
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      567 2024-06-02 03:29:51.000000 coders-utils-0.0.2/coders_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)      396 2024-06-02 03:29:51.000000 coders-utils-0.0.2/coders_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)        1 2024-06-02 03:29:51.000000 coders-utils-0.0.2/coders_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)       16 2024-06-02 03:29:51.000000 coders-utils-0.0.2/coders_utils.egg-info/requires.txt
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)       13 2024-06-02 03:29:51.000000 coders-utils-0.0.2/coders_utils.egg-info/top_level.txt
+-rw-rw-r--   0 parzival  (1000) parzival  (1000)       38 2024-06-02 03:29:51.289822 coders-utils-0.0.2/setup.cfg
+-rwxr-xr-x   0 parzival  (1000) parzival  (1000)      759 2024-06-02 03:29:37.000000 coders-utils-0.0.2/setup.py
```

### Comparing `coders-utils-0.0.1/LICENSE` & `coders-utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coders-utils-0.0.1/PKG-INFO` & `coders-utils-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coders-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: jacob.h.barrow
 Author-email: jacob.h.barrow@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `coders-utils-0.0.1/coders_utils/file_iterators.py` & `coders-utils-0.0.2/coders_utils/identifiers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,107 @@
-from aiofiles import open as async_open
+from random import randint
 
-class File_Iterator:
-    def __init__(self, location, validation_ptr=None):
-        with open(location) as reader:
-            self.data = reader.read().strip().split('\n')
-        
-        self.validation_ptr = validation_ptr
-        self.index = 0
-        self.length = len(self.data)
+class UUID:
+    hexMap = {idx: str(idx) for idx in range(10)}
+    hexMap[10] = 'a'
+    hexMap[11] = 'b'
+    hexMap[12] = 'c'
+    hexMap[13] = 'd'
+    hexMap[14] = 'e'
+    hexMap[15] = 'f'
+
+    def __init__(self, version = 4, n = 4):
+        if version > 4 or version < 0:
+            raise Exception("Version outside the range!")
+
+        if n > 15 or n < 0:
+            raise Exception("Variant amount is outside the range!")
+
+        self.n = n
+        self.version = version
+        self.uuid = ""
+
+    def getHexRange(self, num):
+        return "".join(self.getNextHex() for _ in range(num))
+
+    def getUuid(self):
+        result = self.getHexRange(8) + "-" + self.getHexRange(4)
+        result += "-" + self.getNextHex(bitsLeft = 0, val = self.version) + self.getHexRange(3)
+        
+        bitAmount = self.n
+        count = 1
+        while bitAmount > 1:
+            bitAmount >>= 1
+            count += 1
+
+        result += "-" + self.getNextHex(bitsLeft = 4 - count, val = self.n) + self.getHexRange(3)
+        result += "-" + self.getHexRange(12)
+
+        return result
+
+    def str2Hex(self, binString):
+        hexString = ""
+
+        for idx in range(0, len(binString), 4):
+            hexString += self.hexMap[int(binString[idx:idx+4], 2)]
+
+        return hexString
+
+    def getNextHex(self, bitsLeft = 4, val = -1):
+        binString = "".join([str(randint(0, 1)) for _ in range(bitsLeft)])
+        if val != -1:
+            binString = bin(val)[2:] + binString
+        return self.str2Hex(binString)
+
+### - Collection -> sized, iterable, container
+class UUID_Handler:
+    # Variant 4 -> access to all four bits in N encoding
+    # N must be less than 16
+    def __init__(self, amount = 10, version = 4, n = 1):
+        try:
+            self.uuidObj = UUID(version = version, n = n)
+        except Exception as e:
+            raise Exception(e.str)
+
+        self.amount = amount
         
     def __iter__(self):
         return self
-    
+
     def __next__(self):
-        ans = found = False
-        while not found and self.index < self.length:
-            value = self.data[self.index]
-            ans = value
-            
-            if self.validation_ptr:
-                if self.validation_ptr(value):
-                    found = True
-            else:
-                found=True
-            self.index += 1
-            
-        if self.index >= self.length and not found:
+        if self.amount:
+            self.amount -= 1
+            return self.uuidObj.getUuid()
+        else:
             raise StopIteration()
+    
+class Controlled_UUID:
+    uuids_given = {}
+    
+    def __new__(cls):
+        if not hasattr(cls, 'instance'):
+            cls.instance = super(Controlled_UUID, cls).__new__(cls)
+        return cls.instance
         
-        return ans
-     
-class File_AsyncIterator:
-    def __init__(self, location, validation_ptr=None):
-        self.location = location
-        self.file = None
-        self.validation_ptr = validation_ptr
+    def get_uuid(self):
+        new, res = False, False
         
-    async def read_line(self):
-        return await self.file.readline()
+        while not new:
+            res = UUID().getUuid()
+            
+            try:
+                self.uuids_given[res]
+            except:
+                new = True
+                self.uuids_given[res] = True
         
-    def __aiter__(self):
-        return self
+        return res
+        
+def get_new_uuid() -> str:
+    return Controlled_UUID().get_uuid()
     
-    async def __anext__(self):
-        if self.file == None:
-            self.file = await async_open(self.location)
-
-        while (val := await self.read_line()).strip():
-            if self.validation_ptr:
-                if self.validation_ptr(val):
-                    return val
-            else:
-                return val
-                
-        raise StopAsyncIteration
-            
 if __name__ == "__main__":
-    import asyncio
+    print(get_new_uuid())
     
-    from .linux_admin_ops import *
+    print(Controlled_UUID().get_uuid())
     
-    print("Trying Sync")
-    class Get_Users:
-        def __iter__(self):
-            return File_Iterator('/etc/group', validation_ptr=check_valid_group)
-        
-    for item in Get_Users():
-        display_item(item)
-    
-    print("\nTrying Async")
-    class Get_Users_Async:
-        def __aiter__(self):
-            return File_AsyncIterator('/etc/group', validation_ptr=check_valid_group)
-        
-    async def main():
-        async for item in Get_Users_Async():
-            display_item(item)
-            
-    asyncio.run(main())
+    print(Controlled_UUID.uuids_given.keys())
```

### Comparing `coders-utils-0.0.1/coders_utils.egg-info/PKG-INFO` & `coders-utils-0.0.2/coders_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coders-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: jacob.h.barrow
 Author-email: jacob.h.barrow@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `coders-utils-0.0.1/setup.py` & `coders-utils-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 from distutils.core import setup, Extension
 
 with open("README.md") as _file:
     long_description = _file.read()
 
 setuptools.setup(
         name= "coders-utils",
-        version = "0.0.1",
+        version = "0.0.2",
         author = "jacob.h.barrow",
         author_email = "jacob.h.barrow@gmail.com",
         long_description = long_description,
         long_description_content_type = "text/markdown",
         url = "",
         packages=setuptools.find_packages(),
         install_requires = [
-            "aiofiles"
+            "aiofiles",
+            "PyYAML"
         ], 
         license = "MIT",
         classifiers =  [
             "License :: OSI Approved :: MIT License",
             "Programming Language :: Python",
             "Programming Language :: Python :: 3",
         ],
```

