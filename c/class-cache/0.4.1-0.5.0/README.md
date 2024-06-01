# Comparing `tmp/class_cache-0.4.1.tar.gz` & `tmp/class_cache-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_cache-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "class_cache-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `class_cache-0.4.1.tar` & `class_cache-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       77 2024-05-27 22:59:15.474911 class_cache-0.4.1/.markdownlint.json
--rw-r--r--   0        0        0      569 2024-05-27 22:59:15.474911 class_cache-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       61 2024-05-27 22:59:15.474911 class_cache-0.4.1/.taplo.toml
--rw-r--r--   0        0        0     3022 2024-05-27 22:59:15.474911 class_cache-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2024-05-27 22:59:15.474911 class_cache-0.4.1/LICENSE
--rw-r--r--   0        0        0     3331 2024-05-27 22:59:15.474911 class_cache-0.4.1/README.md
--rw-r--r--   0        0        0      141 2024-05-27 22:59:15.474911 class_cache-0.4.1/class_cache/__init__.py
--rw-r--r--   0        0        0     9441 2024-05-27 22:59:15.474911 class_cache-0.4.1/class_cache/backends.py
--rw-r--r--   0        0        0     3596 2024-05-27 22:59:15.474911 class_cache-0.4.1/class_cache/core.py
--rw-r--r--   0        0        0      229 2024-05-27 22:59:15.474911 class_cache-0.4.1/class_cache/types.py
--rw-r--r--   0        0        0      310 2024-05-27 22:59:15.474911 class_cache-0.4.1/class_cache/utils.py
--rw-r--r--   0        0        0     2141 2024-05-27 22:59:15.474911 class_cache-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4085 1970-01-01 00:00:00.000000 class_cache-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       77 2024-06-01 23:07:03.317229 class_cache-0.5.0/.markdownlint.json
+-rw-r--r--   0        0        0      569 2024-06-01 23:07:03.317229 class_cache-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       61 2024-06-01 23:07:03.317229 class_cache-0.5.0/.taplo.toml
+-rw-r--r--   0        0        0     3210 2024-06-01 23:07:03.317229 class_cache-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2024-06-01 23:07:03.317229 class_cache-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3331 2024-06-01 23:07:03.317229 class_cache-0.5.0/README.md
+-rw-r--r--   0        0        0      141 2024-06-01 23:07:03.317229 class_cache-0.5.0/class_cache/__init__.py
+-rw-r--r--   0        0        0    11828 2024-06-01 23:07:03.317229 class_cache-0.5.0/class_cache/backends.py
+-rw-r--r--   0        0        0     3596 2024-06-01 23:07:03.317229 class_cache-0.5.0/class_cache/core.py
+-rw-r--r--   0        0        0      229 2024-06-01 23:07:03.317229 class_cache-0.5.0/class_cache/types.py
+-rw-r--r--   0        0        0      310 2024-06-01 23:07:03.317229 class_cache-0.5.0/class_cache/utils.py
+-rw-r--r--   0        0        0     2194 2024-06-01 23:07:03.317229 class_cache-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 class_cache-0.5.0/PKG-INFO
```

### Comparing `class_cache-0.4.1/.pre-commit-config.yaml` & `class_cache-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `class_cache-0.4.1/CHANGELOG.md` & `class_cache-0.5.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.5.0 (2024-06-01)
+
+### Feature
+
+* feat(backend): add brotli compression wrapper ([`cfff762`](https://github.com/Rizhiy/class-cache/commit/cfff762c7e2131fde3b865a4422d6a616555dd04))
+
+
 ## v0.4.1 (2024-05-27)
 
 ### Fix
 
 * fix(backend): add proper extension for sqlite db files ([`f2063c6`](https://github.com/Rizhiy/class-cache/commit/f2063c6b69c00925b63143914d1efabc334352d5))
```

### Comparing `class_cache-0.4.1/LICENSE` & `class_cache-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `class_cache-0.4.1/README.md` & `class_cache-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `class_cache-0.4.1/class_cache/backends.py` & `class_cache-0.5.0/class_cache/backends.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import pickle  # noqa: S403
 import sqlite3
 from abc import ABC
 from collections import defaultdict
 from pathlib import Path
 from typing import Any, Iterable, Iterator, MutableMapping, TypeAlias, cast
 
-from fasteners import InterProcessReaderWriterLock
+import brotli
 from marisa_trie import Trie
 from replete.consistent_hash import consistent_hash
+from replete.flock import FileLock
 
 from class_cache.types import KeyType, ValueType
 from class_cache.utils import get_class_cache_dir
 
 ID_TYPE: TypeAlias = str | int | None
 
 
@@ -54,22 +55,22 @@
 
     def __init__(self, id_: ID_TYPE = None, max_block_size=1024 * 1024) -> None:
         super().__init__(id_)
         self._dir = self.ROOT_DIR / str(self.id)
         self._dir.mkdir(exist_ok=True, parents=True)
         self._max_block_size = max_block_size
         self._meta_path = self._dir / "meta.json"
-        self._lock = InterProcessReaderWriterLock(self._dir / "lock.file")
+        self._lock = FileLock(self._meta_path)
         self._check_meta()
 
     @property
     def dir(self) -> Path:
         return self._dir
 
-    # Helper methods, don't acquire locks inside them
+    # Helper methods, they don't acquire locks, so should only be used inside methods that do
     def _read_meta(self) -> META_TYPE:
         with self._meta_path.open() as f:
             return json.load(f)
 
     def _write_meta(self, meta: META_TYPE) -> None:
         with self._meta_path.open("w") as f:
             json.dump(meta, f)
@@ -84,14 +85,16 @@
         return f"{consistent_hash(key):x}"
 
     def _get_block_id_for_key(self, key: KeyType, prefix_len=1) -> str:
         key_hash = self._get_key_hash(key)
 
         blocks_trie = Trie(self.get_all_block_ids())
         prefixes = blocks_trie.prefixes(key_hash)
+        if prefix_len > len(key_hash):
+            raise ValueError("Got prefix_len that is larger than key_hash len.")
         return key_hash[:prefix_len] if not prefixes else max(prefixes, key=len)
 
     def _get_block(self, block_id: str) -> dict[KeyType, ValueType]:
         try:
             with self.get_path_for_block_id(block_id).open("rb") as f:
                 return pickle.load(f)  # noqa: S301
         except FileNotFoundError:
@@ -106,17 +109,16 @@
         meta["len"] += change
         self._write_meta(meta)
 
     def _get_block_for_key(self, key: KeyType) -> dict[KeyType, ValueType]:
         return self._get_block(self._get_block_id_for_key(key))
 
     def get_all_block_ids(self) -> Iterable[str]:
-        yield from (path.name.split(".")[0] for path in self._dir.glob(f"*{self.BLOCK_SUFFIX}"))
-
-    # Helper methods end
+        with self._lock.read_lock():
+            yield from (path.name.split(".")[0] for path in self._dir.glob(f"*{self.BLOCK_SUFFIX}"))
 
     def _check_meta(self) -> None:
         with self._lock.read_lock():
             if self._meta_path.exists():
                 return
             if list(self.get_all_block_ids()):
                 raise ValueError(f"Found existing blocks without meta file in {self._dir}")
@@ -129,18 +131,17 @@
 
     def __len__(self) -> int:
         with self._lock.read_lock():
             return self._read_meta()["len"]
 
     def __iter__(self) -> Iterator[KeyType]:
         # TODO: Optimise this
-        # TODO: This should also use a read lock, but it seems to be not working, see:
-        # https://github.com/harlowja/fasteners/issues/115
-        for block_id in self.get_all_block_ids():
-            yield from self._get_block(block_id).keys()
+        with self._lock.read_lock():
+            for block_id in self.get_all_block_ids():
+                yield from self._get_block(block_id).keys()
 
     def __getitem__(self, key: KeyType) -> ValueType:
         with self._lock.read_lock():
             return self._get_block_for_key(key)[key]
 
     def __setitem__(self, key: KeyType, value: ValueType, prefix_len=1) -> None:
         with self._lock.write_lock():
@@ -240,14 +241,84 @@
     def __delitem__(self, key: KeyType) -> None:
         key_str = self._encode(key)
         self._cursor.execute(f"DELETE FROM {self.DATA_TABLE_NAME} WHERE key=?", (key_str,))
         self._con.commit()
 
     def clear(self) -> None:
         self._cursor.execute(f"DROP TABLE IF EXISTS {self.DATA_TABLE_NAME}")
+        self._con.commit()
         self._check_table()
 
     def __del__(self):
         self._con.commit()
         self._con.close()
 
     # TODO: implement *_many methods
+
+
+class BackendWrapper(BaseBackend[KeyType, ValueType]):
+    """
+    :param backend: backend to be wrapped
+    """
+
+    def __init__(self, *args, backend_type: type[BaseBackend], **kwargs) -> None:
+        super().__init__()
+        self._backend = backend_type(*args, **kwargs)
+
+    def __contains__(self, key: KeyType) -> bool:
+        return key in self._backend
+
+    def __len__(self) -> int:
+        return len(self._backend)
+
+    def __iter__(self) -> Iterator[KeyType]:
+        yield from self._backend
+
+    def __getitem__(self, key: KeyType) -> ValueType:
+        return self._backend[key]
+
+    def __setitem__(self, key: KeyType, value: ValueType) -> None:
+        self._backend[key] = value
+
+    def __delitem__(self, key: KeyType) -> None:
+        del self._backend[key]
+
+    def contains_many(self, keys: Iterable[KeyType]) -> Iterator[tuple[KeyType, bool]]:
+        yield from self._backend.contains_many(keys)
+
+    def get_many(self, keys: Iterable[KeyType]) -> Iterator[tuple[KeyType, ValueType]]:
+        yield from self._backend.get_many(keys)
+
+    def set_many(self, items: Iterable[tuple[KeyType, ValueType]]) -> None:
+        self._backend.set_many(items)
+
+    def del_many(self, keys: Iterable[KeyType]) -> None:
+        self._backend.del_many(keys)
+
+    def clear(self) -> None:
+        self._backend.clear()
+
+
+class BrotliCompressWrapper(BackendWrapper[KeyType, ValueType]):
+    def _encode(self, obj: KeyType | ValueType) -> bytes:
+        return brotli.compress(pickle.dumps(obj, pickle.HIGHEST_PROTOCOL))
+
+    def _decode(self, stored: bytes) -> KeyType | ValueType:
+        return pickle.loads(brotli.decompress(stored))  # noqa: S301
+
+    def __contains__(self, key: KeyType) -> bool:
+        return super().__contains__(key)
+
+    def __iter__(self) -> Iterator[KeyType]:
+        yield from super().__iter__()
+
+    def __getitem__(self, key: KeyType) -> ValueType:
+        return self._decode(super().__getitem__(key))
+
+    def __setitem__(self, key: KeyType, value: ValueType) -> None:
+        self._backend[key] = self._encode(value)
+
+    def __delitem__(self, key: KeyType) -> None:
+        return super().__delitem__(key)
+
+    def set_many(self, items: Iterable[tuple[KeyType, ValueType]]) -> None:
+        return super().set_many((key, self._encode(value)) for key, value in items)
```

### Comparing `class_cache-0.4.1/class_cache/core.py` & `class_cache-0.5.0/class_cache/core.py`

 * *Files identical despite different names*

### Comparing `class_cache-0.4.1/pyproject.toml` & `class_cache-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "class-cache"
 maintainers = [{ name = "Artem Vasenin", email = "vasart169@gmail.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dynamic = ["description", "version"]
-dependencies = ["Pympler", "fasteners", "marisa-trie", "replete"]
+dependencies = ["Pympler", "brotli", "marisa-trie", "replete>=2.3.1"]
 
 [project.urls]
 Home = "https://github.com/Rizhiy/class-cache"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "replete[testing]"]
 dev = ["black", "class-cache[test]", "numpy", "pre-commit", "ruff"]
@@ -28,14 +28,17 @@
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--doctest-modules --ignore=benchmark"
 
 [tool.black]
 line-length = 120
 # skip-magic-trailing-comma = true
+[tool.isort]
+profile = "black"
+line_length = 120
 
 [tool.yamlfix]
 line_length = 120
 section_whitelines = 1
 
 [tool.pyright]
 strictParameterNoneValue = false
```

### Comparing `class_cache-0.4.1/PKG-INFO` & `class_cache-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: class-cache
-Version: 0.4.1
+Version: 0.5.0
 Summary: Caching for class based generators
 Maintainer-email: Artem Vasenin <vasart169@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: Pympler
-Requires-Dist: fasteners
+Requires-Dist: brotli
 Requires-Dist: marisa-trie
-Requires-Dist: replete
+Requires-Dist: replete>=2.3.1
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: class-cache[test] ; extra == "dev"
 Requires-Dist: numpy ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
```

