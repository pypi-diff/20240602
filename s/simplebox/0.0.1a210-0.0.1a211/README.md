# Comparing `tmp/simplebox-0.0.1a210-py3-none-any.whl.zip` & `tmp/simplebox-0.0.1a211-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 470203 bytes, number of entries: 166
--rw-rw-rw-  2.0 fat     5191 b- defN 24-May-20 12:58 simplebox/__init__.py
+Zip file size: 470501 bytes, number of entries: 166
+-rw-rw-rw-  2.0 fat     5191 b- defN 24-Jun-02 14:52 simplebox/__init__.py
 -rw-rw-rw-  2.0 fat     2090 b- defN 24-Apr-07 16:46 simplebox/backend.py
 -rw-rw-rw-  2.0 fat    17626 b- defN 24-Apr-07 16:46 simplebox/character.py
--rw-rw-rw-  2.0 fat     4829 b- defN 24-Apr-14 15:04 simplebox/classes.py
+-rw-rw-rw-  2.0 fat     5933 b- defN 24-Jun-02 14:52 simplebox/classes.py
 -rw-rw-rw-  2.0 fat    16962 b- defN 24-Apr-20 14:21 simplebox/cmd.py
--rw-rw-rw-  2.0 fat     5481 b- defN 23-Nov-14 15:01 simplebox/converter.py
+-rw-rw-rw-  2.0 fat     5919 b- defN 24-Jun-02 15:14 simplebox/converter.py
 -rw-rw-rw-  2.0 fat     1638 b- defN 24-Apr-07 15:02 simplebox/enums.py
 -rw-rw-rw-  2.0 fat      306 b- defN 23-May-31 16:53 simplebox/generic.py
 -rw-rw-rw-  2.0 fat    60386 b- defN 24-May-20 13:15 simplebox/http.py
 -rw-rw-rw-  2.0 fat     5165 b- defN 24-Apr-27 14:18 simplebox/jsonparser.py
 -rw-rw-rw-  2.0 fat    21577 b- defN 24-Apr-27 14:26 simplebox/number.py
 -rw-rw-rw-  2.0 fat     1006 b- defN 24-Apr-07 17:05 simplebox/singleton.py
 -rw-rw-rw-  2.0 fat     1400 b- defN 24-Apr-07 17:02 simplebox/version.py
@@ -157,12 +157,12 @@
 -rw-rw-rw-  2.0 fat     2735 b- defN 24-Apr-27 14:18 simplebox/utils/locks.py
 -rw-rw-rw-  2.0 fat    14864 b- defN 24-Apr-28 15:25 simplebox/utils/objects.py
 -rw-rw-rw-  2.0 fat     3258 b- defN 24-Apr-14 14:42 simplebox/utils/optionals.py
 -rw-rw-rw-  2.0 fat     5653 b- defN 24-Apr-28 17:58 simplebox/utils/reflect.py
 -rw-rw-rw-  2.0 fat    19546 b- defN 24-Apr-07 15:48 simplebox/utils/strings.py
 -rw-rw-rw-  2.0 fat      247 b- defN 23-Feb-28 15:31 simplebox/valid/__init__.py
 -rw-rw-rw-  2.0 fat    17399 b- defN 24-May-06 14:40 simplebox/valid/_validator.py
--rw-rw-rw-  2.0 fat     1360 b- defN 24-May-20 13:15 simplebox-0.0.1a210.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-20 13:15 simplebox-0.0.1a210.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-20 13:15 simplebox-0.0.1a210.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    14453 b- defN 24-May-20 13:15 simplebox-0.0.1a210.dist-info/RECORD
-166 files, 1486712 bytes uncompressed, 447411 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 fat     1360 b- defN 24-Jun-02 15:14 simplebox-0.0.1a211.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-02 15:14 simplebox-0.0.1a211.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Jun-02 15:14 simplebox-0.0.1a211.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    14453 b- defN 24-Jun-02 15:14 simplebox-0.0.1a211.dist-info/RECORD
+166 files, 1488254 bytes uncompressed, 447709 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -480,20 +480,20 @@
 
 Filename: simplebox/valid/__init__.py
 Comment: 
 
 Filename: simplebox/valid/_validator.py
 Comment: 
 
-Filename: simplebox-0.0.1a210.dist-info/METADATA
+Filename: simplebox-0.0.1a211.dist-info/METADATA
 Comment: 
 
-Filename: simplebox-0.0.1a210.dist-info/WHEEL
+Filename: simplebox-0.0.1a211.dist-info/WHEEL
 Comment: 
 
-Filename: simplebox-0.0.1a210.dist-info/top_level.txt
+Filename: simplebox-0.0.1a211.dist-info/top_level.txt
 Comment: 
 
-Filename: simplebox-0.0.1a210.dist-info/RECORD
+Filename: simplebox-0.0.1a211.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplebox/__init__.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
-__version__ = "0.0.1.alpha210"
+__version__ = "0.0.1.alpha211"
 
 banner = f"""
  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------.  .----------------. 
 | .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. || .--------------. |
 | |    _______   | || |     _____    | || | ____    ____ | || |   ______     | || |   _____      | || |  _________   | || |   ______     | || |     ____     | || |  ____  ____  | |
 | |   /  ___  |  | || |    |_   _|   | || ||_   \  /   _|| || |  |_   __ \   | || |  |_   _|     | || | |_   ___  |  | || |  |_   _ \    | || |   .'    `.   | || | |_  _||_  _| | |
 | |  |  (__ \_|  | || |      | |     | || |  |   \/   |  | || |    | |__) |  | || |    | |       | || |   | |_  \_|  | || |    | |_) |   | || |  /  .--.  \  | || |   \ \  / /   | |
```

## simplebox/classes.py

```diff
@@ -1,23 +1,26 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 import inspect
+import typing
 from types import GenericAlias
-from typing import _Final, Optional
+from typing import Optional
 
 from .exceptions import raise_exception, InstanceException
 
-__all__ = ['ForceType', 'StaticClass', 'Final', 'ConstructorIntercept']
+_Final = getattr(typing, "_Final")
+
+__all__ = ['ForceType', 'StaticClass', 'Final', 'End', 'ConstructorIntercept']
 
 
 class ForceType(object):
     """
     Given a type as the type of variable, an exception is thrown if the assigned type is inconsistent with that type.
 
-    Excample:
+    Example:
         class Person:
             age = ForceType(int) # ForceType(int, bool)
             name = ForceType(str)
 
             def __init__(self, age, name):
                 self.age = age
                 self.name = name
@@ -32,24 +35,24 @@
         self.__types_append = self.__types.append
         self.__types_name = []
         self.__types_name_append = self.__types_name.append
         for t in types:
             if t is None:  # NoneType begin with Python version 3.10+
                 self.__can_none = True
                 self.__types_name_append("NoneType")
-            elif issubclass(t_ := (type(t)), type):
+            elif issubclass(t_ := type(t), GenericAlias):
+                t_g_alias = type(t())
+                self.__types_append(t_g_alias)
+                self.__types_name_append(t_g_alias.__name__)
+            elif issubclass(t_, type):
                 self.__types_append(t)
                 self.__types_name_append(self.__get__name(t))
             elif issubclass(t_, _Final):
                 self.__types_append(getattr(t, "__origin__"))
                 self.__types_name_append(self.__get__name(t))
-            elif issubclass(t_, GenericAlias):
-                t_g_alias = type(t())
-                self.__types_append(t_g_alias)
-                self.__types_name_append(t_g_alias.__name__)
             else:
                 raise TypeError(f"expected 'type' type class, but found '{t_.__name__}'")
         self.__types: type[type, ...] = tuple(self.__types)
 
     @staticmethod
     def __get__name(t: type) -> str:
         if issubclass(type(t), _Final):
@@ -86,32 +89,63 @@
     def __call__(cls, *args, **kwargs):
         raise_exception(InstanceException(f"Class '{cls.__name__}' cannot be instantiated!!!"))
 
 
 class Final(type):
     """
     Classes that are prohibited from being inherited.
+    The difference with 'End' is that 'Final' does not need to be instantiated to detect whether it inherits,
+    but 'End' needs to be instantiated before it can be checked.
     usage:
 
-        class People(metaclass=Final):
+        class Parent(metaclass=Final):
             pass
 
 
-        class Child(People):
+        class Child(Parent):
             pass
 
-        compile and run python script  # raise exception: type 'People' is not an acceptable base type
+        compile and run python script  # raise exception: Class 'Parent' is a Final type, cannot be inherited
     """
+
     def __new__(mcs, name, bases, dict, *args, **kwargs):
         for base in bases:
             if isinstance(base, Final):
-                raise TypeError("Class '{0}' is a final type, cannot be inherited".format(base.__name__))
+                raise TypeError("Class '{0}' is a Final type, cannot be inherited".format(base.__name__))
         return super().__new__(mcs, name, bases, dict, **kwargs)
 
 
+class End:
+    """
+    Classes that are prohibited from being inherited.
+    The difference with 'Final' is that 'Final' does not need to be instantiated to detect whether it inherits,
+    but 'End' needs to be instantiated before it can be checked.
+
+    Example:
+        class Parent(End):
+            pass
+
+
+        class Child(Parent):
+            pass
+
+        Child()  # raise exception: Class 'Parent' is an End type, cannot be inherited
+    """
+    def __new__(cls, *args, **kwargs):
+        cls.__handler(cls, 1)
+
+    @classmethod
+    def __handler(cls, base: type, dep):
+        for clz in base.__bases__:
+            if clz.__name__ == End.__name__ and dep > 1:
+                raise TypeError("Class '{0}' is an End type, cannot be inherited".format(base.__name__))
+            else:
+                cls.__handler(clz, dep + 1)
+
+
 class ConstructorIntercept(type):
     """
     Some classes are not allowed to be accessed or instantiated externally,
     so use ConstructorIntercept to decorate classes that need to be restricted.
     For example, providing services externally through the wrapper function
 
     Subclasses will also be affected, i.e. subclasses also need to be instantiated together in the current file,
```

## simplebox/converter.py

```diff
@@ -51,26 +51,28 @@
     BB = Integer(1 << 93)
     NB = Integer(1 << 103)
     DB = Integer(1 << 113)
 
     @staticmethod
     def format(value: [float, int, '_UnitEnum', '_Converter'], precision: int) -> str:
         """
+        Format the value into the specified storage unit.
+        float, int it will be handled in Bytes.
         ex:
             StorageUnit.format(StorageUnit.MB, 2)           >> 1.0M  # Special form, the unit base is 1 case
             StorageUnit.format(StorageUnit.MB.of(2), 2)     >> 2.0M
             StorageUnit.format(StorageUnit.MB.of(10000), 2) >> 9.77GB
-            StorageUnit.format(16777216, 2)                 >> 2.0M
+            StorageUnit.format(2097152, 2)                  >> 2.0M
         """
         if isinstance(value, _UnitEnum):
             _value = value.value
         elif isinstance(value, _Converter):
             _value = value.to(StorageUnit.BIT)
         else:
-            _value = value
+            _value = StorageUnit.BYTE.of(value).to(StorageUnit.BIT)
         if _value >= StorageUnit.DB.value:
             return f"{round(_value / StorageUnit.DB.value, precision)}DB"
         elif _value >= StorageUnit.NB.value:
             return f"{round(_value / StorageUnit.NB.value, precision)}NB"
         elif _value >= StorageUnit.BB.value:
             return f"{round(_value / StorageUnit.BB.value, precision)}BB"
         elif _value >= StorageUnit.YB.value:
@@ -85,16 +87,18 @@
             return f"{round(_value / StorageUnit.TB.value, precision)}TB"
         elif _value >= StorageUnit.GB.value:
             return f"{round(_value / StorageUnit.GB.value, precision)}GB"
         elif _value >= StorageUnit.MB.value:
             return f"{round(_value / StorageUnit.MB.value, precision)}MB"
         elif _value >= StorageUnit.KB.value:
             return f"{round(_value / StorageUnit.KB.value, precision)}KB"
+        elif _value >= StorageUnit.BYTE.value:
+            return f"{round(_value / StorageUnit.BYTE.value, precision)}B"
         else:
-            return f"{round(_value, precision)}B"
+            return f"{round(_value, precision)}bit"
 
 
 class TimeUnit(_UnitEnum):
     """
     Time unit conversion tool
     """
     NANO_SECOND = Integer(1)
@@ -104,26 +108,28 @@
     MINUTE = Integer(1 * 1000 * 1000 * 1000 * 60)
     HOUR = Integer(1 * 1000 * 1000 * 1000 * 60 * 60)
     DAY = Integer(1 * 1000 * 1000 * 1000 * 60 * 60 * 24)
 
     @staticmethod
     def format(value: [float, int, '_UnitEnum', '_Converter'], precision: int) -> str:
         """
+        Format the value to the specified unit of time.
+        float, int it will be handled in millisecond.
         ex:
             TimeUnit.format(TimeUnit.HOUR, 2)           >> 1.0Hour(s)
             TimeUnit.format(TimeUnit.HOUR.of(2), 2)     >> 2.0Hour(s)
             TimeUnit.format(TimeUnit.HOUR.of(333), 2)   >> 13.88Day(s)
-            TimeUnit.format(1699972914979, 2)           >> 28.33Min(s)
+            TimeUnit.format(1699800, 2)                 >> 28.33Min(s)
         """
         if isinstance(value, _UnitEnum):
             _value = value.value
         elif isinstance(value, _Converter):
             _value = value.to(TimeUnit.NANO_SECOND)
         else:
-            _value = value
+            _value = TimeUnit.MILLI_SECOND.of(value).to(TimeUnit.NANO_SECOND)
         if _value >= TimeUnit.DAY.value:
             return f"{round(_value / TimeUnit.DAY.value, precision)}Day(s)"
         elif _value >= TimeUnit.HOUR.value:
             return f"{round(_value / TimeUnit.HOUR.value, precision)}Hour(s)"
         elif _value >= TimeUnit.MINUTE.value:
             return f"{round(_value / TimeUnit.MINUTE.value, precision)}Min(s)"
         elif _value >= TimeUnit.SECOND.value:
```

## Comparing `simplebox-0.0.1a210.dist-info/METADATA` & `simplebox-0.0.1a211.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplebox
-Version: 0.0.1a210
+Version: 0.0.1a211
 Summary: 简易工具箱。
 Author: fuck
 License: MIT Licence
 Keywords: pip,simplebox,backend,fast,fasttools,box,simple
 Platform: any
 Requires-Python: >=3.9
 Requires-Dist: psutil (==5.9.2)
```

## Comparing `simplebox-0.0.1a210.dist-info/RECORD` & `simplebox-0.0.1a211.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-simplebox/__init__.py,sha256=piqAGi_fZJ0kIOY6Bhug-RQMjZJDpN0bBqJYugBnsVI,5191
+simplebox/__init__.py,sha256=Y1JLNYnEC7NLiMvPbKGKN_Kfc20b44zF3XUIyO82rh4,5191
 simplebox/backend.py,sha256=yR3gveO0iKcTKWKW5K57513u-s7O3oGes84Kp8HUZho,2090
 simplebox/character.py,sha256=NEbQqFmD3rpkl_E3MeES7rRfAmtc_DJHoKcF8GNK92g,17626
-simplebox/classes.py,sha256=vGD0PVglh-Nlz8I3PTqDmDquQf_Z2BNoXIvp9aRS140,4829
+simplebox/classes.py,sha256=5-1WHsPzDiSPZLGt9j8gZQWxtSQ78xc3-0h324Khs6w,5933
 simplebox/cmd.py,sha256=5SK-ne4vAyjNdEztS0TyMWUuQC6bBc4RCtnbdQBvVF4,16962
-simplebox/converter.py,sha256=DZ_sb-ZBIorTZAlpuNyGjxnlPAjtSp7yKMIDSiwws0g,5481
+simplebox/converter.py,sha256=MTw7j8fpUd1u4ynTuKqlJa0svGpAs4hokDgHd5F8Hs0,5919
 simplebox/enums.py,sha256=KzziG7TboPMIENPrc4HrsUagSEMd4JfLFG6Bn2T0HAs,1638
 simplebox/generic.py,sha256=tBDzlqFHQ7I6bb8_iC9PEqyMaD0sxJee9a7zR3YwxRw,306
 simplebox/http.py,sha256=S0yx0Prd6PuTx5uPSCgSb-1gl7QeM9BASrUPvAnc1b4,60386
 simplebox/jsonparser.py,sha256=QD_nY7PCdTOXBjpRZ6iysx386pmS2kMULGRmsMRaVUo,5165
 simplebox/number.py,sha256=hpSLKIoRFnjt-lk4SUCvYNKbcBD8lP_vaOFtD4JQIUQ,21577
 simplebox/singleton.py,sha256=zhyjjhQfg9Y1UYgYFYF31ybNjX0A0oMzBaOG1UZerXo,1006
 simplebox/version.py,sha256=5H3eNzxQOzLT5meyjzOZ1-dg1R9U3h5lCGNzWXwU4Lg,1400
@@ -156,11 +156,11 @@
 simplebox/utils/locks.py,sha256=KP_utNUBYeWjJhsWzu1-rn5sG6jzi2cDrFXtSmgJCHE,2735
 simplebox/utils/objects.py,sha256=jaTS8DaHdrdspANFzol2ad6UKRQnFCPCvHHnSu5R2d4,14864
 simplebox/utils/optionals.py,sha256=XDlteLGkfbWHOgJPdGykE-a79Ae-P7Fbfsabmiwdjuw,3258
 simplebox/utils/reflect.py,sha256=ih_-fw49DzYSNyauvDbpEW5ixf5wi5UVhE6nlq_zfUk,5653
 simplebox/utils/strings.py,sha256=yvdvMVI-ULs-DIWElpmjdYHp9CPLbETc5M-16L9gflk,19546
 simplebox/valid/__init__.py,sha256=7deSv2vW7Wj-83Db3JbO0SZK9Pf-G9pDqbCAgkxr8PI,247
 simplebox/valid/_validator.py,sha256=MPJRmSsrPLq3ZaKzqPs71iZYP5dRzpI1K2dUF6oqFDI,17399
-simplebox-0.0.1a210.dist-info/METADATA,sha256=Ae2IImBQNYfM7AiLJnPAOjc2afMf3LX3WNBgGnGscSM,1360
-simplebox-0.0.1a210.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-simplebox-0.0.1a210.dist-info/top_level.txt,sha256=96Ce93hfSG2V2dNspzU_GDarYqtHFh9siA46UaMcdjo,10
-simplebox-0.0.1a210.dist-info/RECORD,,
+simplebox-0.0.1a211.dist-info/METADATA,sha256=ThhnmVR7xXjRKSmJ9SQnAIQYR9OVguePrfTsK1bVzRo,1360
+simplebox-0.0.1a211.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+simplebox-0.0.1a211.dist-info/top_level.txt,sha256=96Ce93hfSG2V2dNspzU_GDarYqtHFh9siA46UaMcdjo,10
+simplebox-0.0.1a211.dist-info/RECORD,,
```

