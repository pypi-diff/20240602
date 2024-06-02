# Comparing `tmp/pywise-0.7.0.tar.gz` & `tmp/pywise-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywise-0.7.0.tar", max compression
+gzip compressed data, was "pywise-0.8.0.tar", max compression
```

## Comparing `pywise-0.7.0.tar` & `pywise-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     7652 2024-05-30 07:20:08.830109 pywise-0.7.0/LICENSE
--rw-r--r--   0        0        0     6819 2024-05-30 07:20:57.500001 pywise-0.7.0/README.md
--rw-r--r--   0        0        0        0 2024-05-30 07:01:50.600121 pywise-0.7.0/core_utils/__init__.py
--rw-r--r--   0        0        0     2828 2024-05-30 07:20:08.830763 pywise-0.7.0/core_utils/archives.py
--rw-r--r--   0        0        0     2674 2024-05-30 07:44:07.390088 pywise-0.7.0/core_utils/collections.py
--rw-r--r--   0        0        0     6050 2024-05-30 07:20:08.831039 pywise-0.7.0/core_utils/common.py
--rw-r--r--   0        0        0     8956 2024-05-30 07:20:08.831238 pywise-0.7.0/core_utils/env.py
--rw-r--r--   0        0        0     2548 2024-05-30 07:20:08.831420 pywise-0.7.0/core_utils/format.py
--rw-r--r--   0        0        0     8635 2024-05-30 07:20:08.831614 pywise-0.7.0/core_utils/loggers.py
--rw-r--r--   0        0        0     3026 2024-05-30 07:20:08.831838 pywise-0.7.0/core_utils/schema.py
--rw-r--r--   0        0        0    22486 2024-05-30 07:20:08.832138 pywise-0.7.0/core_utils/serialization.py
--rw-r--r--   0        0        0     6438 2024-05-30 07:20:08.832577 pywise-0.7.0/core_utils/timer.py
--rw-r--r--   0        0        0     5543 2024-05-30 07:20:08.832811 pywise-0.7.0/core_utils/url_bucket_kv.py
--rw-r--r--   0        0        0     3248 2024-05-30 07:44:07.390411 pywise-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7532 1970-01-01 00:00:00.000000 pywise-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-05-30 07:47:19.895395 pywise-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6819 2024-05-30 07:47:19.895864 pywise-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 07:01:50.600121 pywise-0.8.0/core_utils/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-30 07:47:19.896280 pywise-0.8.0/core_utils/archives.py
+-rw-r--r--   0        0        0     2674 2024-05-30 07:47:19.896567 pywise-0.8.0/core_utils/collections.py
+-rw-r--r--   0        0        0     6098 2024-06-02 17:14:00.638719 pywise-0.8.0/core_utils/common.py
+-rw-r--r--   0        0        0     8956 2024-05-30 07:47:19.897265 pywise-0.8.0/core_utils/env.py
+-rw-r--r--   0        0        0     2548 2024-05-30 07:47:19.897568 pywise-0.8.0/core_utils/format.py
+-rw-r--r--   0        0        0      688 2024-06-02 17:14:00.638954 pywise-0.8.0/core_utils/io_utils.py
+-rw-r--r--   0        0        0     8635 2024-05-30 07:47:19.897835 pywise-0.8.0/core_utils/loggers.py
+-rw-r--r--   0        0        0     3146 2024-06-02 17:14:00.639249 pywise-0.8.0/core_utils/schema.py
+-rw-r--r--   0        0        0    22486 2024-05-30 07:47:19.898695 pywise-0.8.0/core_utils/serialization.py
+-rw-r--r--   0        0        0     6438 2024-05-30 07:47:19.899497 pywise-0.8.0/core_utils/timer.py
+-rw-r--r--   0        0        0     5543 2024-05-30 07:47:19.899762 pywise-0.8.0/core_utils/url_bucket_kv.py
+-rw-r--r--   0        0        0     3248 2024-06-02 17:14:00.639563 pywise-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7532 1970-01-01 00:00:00.000000 pywise-0.8.0/PKG-INFO
```

### Comparing `pywise-0.7.0/LICENSE` & `pywise-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywise-0.7.0/README.md` & `pywise-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pywise-0.7.0/core_utils/archives.py` & `pywise-0.8.0/core_utils/archives.py`

 * *Files identical despite different names*

### Comparing `pywise-0.7.0/core_utils/collections.py` & `pywise-0.8.0/core_utils/collections.py`

 * *Files identical despite different names*

### Comparing `pywise-0.7.0/core_utils/common.py` & `pywise-0.8.0/core_utils/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 
     if str(t).startswith("typing.Union"):
         try:
             args = get_args(t)
             if len(args) == 2 and args[1] == type(None):  # noqa: E721
                 # an Optional type is equivalent to Union[T, None]
                 return f"typing.Optional[{type_name(args[0])}]"
-        except Exception:
-            pass
+        except Exception:  # pragma: no cover  # noqa
+            pass  # pragma: no cover
         return str(t)
 
     if issubclass(type(t), _GenericAlias):
         return str(t)
 
     if isinstance(t, TypeVar):  # type: ignore
         return str(t)  # type: ignore
```

### Comparing `pywise-0.7.0/core_utils/env.py` & `pywise-0.8.0/core_utils/env.py`

 * *Files identical despite different names*

### Comparing `pywise-0.7.0/core_utils/format.py` & `pywise-0.8.0/core_utils/format.py`

 * *Files identical despite different names*

### Comparing `pywise-0.7.0/core_utils/loggers.py` & `pywise-0.8.0/core_utils/loggers.py`

 * *Files identical despite different names*

### Comparing `pywise-0.7.0/core_utils/schema.py` & `pywise-0.8.0/core_utils/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
 def dict_type_representation(nt_or_dc_type: Type) -> Discover:
     """The dictionary JSON-like named attribute & expected type representation computed
     from the supplied NamedTuple-deriving or @dataclass decorated type.
     """
     try:
         return _dict_type(nt_or_dc_type)
-    except Exception as e:
-        raise TypeError(
+    except Exception as e:  # pragma: no cover
+        raise TypeError(  # pragma: no cover
             f"Failed to discover field-type attributes of type: '{nt_or_dc_type}",
             e,
         )
 
 
 def _dict_type(t: type):
     if is_typed_namedtuple(t) or is_dataclass(t):
@@ -68,26 +68,26 @@
         if "typing.Union" not in tn and "typing.Optional" not in tn:
             checkable_t: Type = checkable_type(t)
             if issubclass(checkable_t, Mapping):
                 try:
                     _args = get_args(t)
                     key_t: type = cast(type, _args[0])
                     val_t: type = cast(type, _args[1])
-                except Exception as e:
-                    raise TypeError(
+                except Exception as e:  # pragma: no cover
+                    raise TypeError(  # pragma: no cover
                         f"Could not extract key & value types from dict type: '{t}'"
                     ) from e
                 else:
                     k = _dict_type(key_t)
                     v = _dict_type(val_t)
                     return {k: v}
 
             elif issubclass(checkable_t, Iterable) and t != str:
                 try:
                     inner_t: type = cast(type, get_args(t)[0])
-                except Exception as e:
-                    raise TypeError(
+                except Exception as e:  # pragma: no cover
+                    raise TypeError(  # pragma: no cover
                         f"Could not extract inner type from iterable type: '{t}'"
                     ) from e
                 else:
                     return [_dict_type(inner_t)]
         return tn
```

### Comparing `pywise-0.7.0/core_utils/serialization.py` & `pywise-0.8.0/core_utils/serialization.py`

 * *Files identical despite different names*

### Comparing `pywise-0.7.0/core_utils/timer.py` & `pywise-0.8.0/core_utils/timer.py`

 * *Files identical despite different names*

### Comparing `pywise-0.7.0/core_utils/url_bucket_kv.py` & `pywise-0.8.0/core_utils/url_bucket_kv.py`

 * *Files identical despite different names*

### Comparing `pywise-0.7.0/pyproject.toml` & `pywise-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywise"
-version = "0.7.0"
+version = "0.8.0"
 description = "Robust serialization support for NamedTuple & @DataClass data types. Various utilities and Quality-of-Life helpers. Python 3.8+ dependency only."
 authors = ["Malcolm Greaves <greaves.malcolm@gmail.com>"]
 homepage = "https://github.com/malcolmgreaves/pywise"
 license = "L-GPL 3.0"
 readme = 'README.md'
 exclude = ['core_utils/support_for_testing.py'] # NEVER INCLUDE THIS FILE (!)
 packages = [
```

### Comparing `pywise-0.7.0/PKG-INFO` & `pywise-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywise
-Version: 0.7.0
+Version: 0.8.0
 Summary: Robust serialization support for NamedTuple & @DataClass data types. Various utilities and Quality-of-Life helpers. Python 3.8+ dependency only.
 Home-page: https://github.com/malcolmgreaves/pywise
 License: L-GPL 3.0
 Author: Malcolm Greaves
 Author-email: greaves.malcolm@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
```

