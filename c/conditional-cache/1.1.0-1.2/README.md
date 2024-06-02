# Comparing `tmp/conditional-cache-1.1.0.tar.gz` & `tmp/conditional_cache-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conditional-cache-1.1.0.tar", last modified: Tue Mar 12 20:15:58 2024, max compression
+gzip compressed data, was "conditional_cache-1.2.tar", last modified: Sun Jun  2 08:39:24 2024, max compression
```

## Comparing `conditional-cache-1.1.0.tar` & `conditional_cache-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 20:15:58.642545 conditional-cache-1.1.0/
--rw-rw-rw-   0        0        0     1089 2023-06-19 11:41:28.000000 conditional-cache-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1318 2024-03-12 20:15:58.641019 conditional-cache-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      112 2024-03-11 09:41:37.000000 conditional-cache-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-12 20:15:58.625955 conditional-cache-1.1.0/conditional_cache/
--rw-rw-rw-   0        0        0      178 2024-03-12 20:06:29.000000 conditional-cache-1.1.0/conditional_cache/__init__.py
--rw-rw-rw-   0        0        0     2674 2024-03-12 19:57:39.000000 conditional-cache-1.1.0/conditional_cache/conditional_cache.py
-drwxrwxrwx   0        0        0        0 2024-03-12 20:15:58.639019 conditional-cache-1.1.0/conditional_cache.egg-info/
--rw-rw-rw-   0        0        0     1318 2024-03-12 20:15:57.000000 conditional-cache-1.1.0/conditional_cache.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-03-12 20:15:58.000000 conditional-cache-1.1.0/conditional_cache.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 20:15:57.000000 conditional-cache-1.1.0/conditional_cache.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-12 20:15:57.000000 conditional-cache-1.1.0/conditional_cache.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-12 20:15:57.000000 conditional-cache-1.1.0/conditional_cache.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-12 20:15:58.642545 conditional-cache-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1414 2024-03-12 20:15:49.000000 conditional-cache-1.1.0/setup.py
+drwxr-xr-x   0 haru       (501) staff       (20)        0 2024-06-02 08:39:24.965741 conditional_cache-1.2/
+-rw-r--r--   0 haru       (501) staff       (20)     1068 2024-06-02 08:29:40.000000 conditional_cache-1.2/LICENSE
+-rw-r--r--   0 haru       (501) staff       (20)     5094 2024-06-02 08:39:24.965456 conditional_cache-1.2/PKG-INFO
+-rw-r--r--   0 haru       (501) staff       (20)     3918 2024-06-02 08:29:40.000000 conditional_cache-1.2/README.md
+drwxr-xr-x   0 haru       (501) staff       (20)        0 2024-06-02 08:39:24.963177 conditional_cache-1.2/conditional_cache/
+-rw-r--r--   0 haru       (501) staff       (20)      177 2024-06-02 08:29:40.000000 conditional_cache-1.2/conditional_cache/__init__.py
+-rw-r--r--   0 haru       (501) staff       (20)     2593 2024-06-02 08:29:40.000000 conditional_cache-1.2/conditional_cache/conditional_cache.py
+drwxr-xr-x   0 haru       (501) staff       (20)        0 2024-06-02 08:39:24.965087 conditional_cache-1.2/conditional_cache.egg-info/
+-rw-r--r--   0 haru       (501) staff       (20)     5094 2024-06-02 08:39:24.000000 conditional_cache-1.2/conditional_cache.egg-info/PKG-INFO
+-rw-r--r--   0 haru       (501) staff       (20)      299 2024-06-02 08:39:24.000000 conditional_cache-1.2/conditional_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 haru       (501) staff       (20)        1 2024-06-02 08:39:24.000000 conditional_cache-1.2/conditional_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 haru       (501) staff       (20)       14 2024-06-02 08:39:24.000000 conditional_cache-1.2/conditional_cache.egg-info/requires.txt
+-rw-r--r--   0 haru       (501) staff       (20)       18 2024-06-02 08:39:24.000000 conditional_cache-1.2/conditional_cache.egg-info/top_level.txt
+-rw-r--r--   0 haru       (501) staff       (20)       38 2024-06-02 08:39:24.965794 conditional_cache-1.2/setup.cfg
+-rw-r--r--   0 haru       (501) staff       (20)     1377 2024-06-02 08:37:07.000000 conditional_cache-1.2/setup.py
```

### Comparing `conditional-cache-1.1.0/conditional_cache/conditional_cache.py` & `conditional_cache-1.2/conditional_cache/conditional_cache.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from __future__ import annotations
-from functools import wraps, _make_key
-from circular_dict import CircularDict
-from time import time
-
-def conditional_lru_cache(maxsize: int=128, typed: bool = False, condition: callable = lambda x: True):
-    cache = CircularDict(maxlen=maxsize)
-
-    def decorator(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            # create a hashable cache key
-            key = _make_key(args, kwargs, typed)
-
-            # Attempt to get the cached value
-            if key in cache:
-                return cache[key]
-
-            # Call the actual function
-            result = func(*args, **kwargs)
-
-            # Conditionally cache the result
-            if condition(result):
-                cache[key] = result
-
-            return result
-
-        # Expose a method to remove an item from the cache
-        def cache_remove(*args, **kwargs):
-            key = _make_key(args, kwargs, typed)
-            cache.pop(key, None)  # Use pop to avoid KeyError if the key is not present
-
-
-        wrapper.cache_remove = cache_remove
-        # Expose a method to clear the full cache
-        wrapper.cache_clear = lambda: cache.clear()
-
-        return wrapper
-
-    return decorator
-
-def conditional_ttl_cache(maxsize: int = 128, typed: int = False, ttl: int = 60, condition: callable = lambda x: True):
-    cache = CircularDict(maxlen=maxsize)
-
-    def decorator(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            # create a hashable cache key
-            key = _make_key(args, kwargs, typed)
-
-            # Attempt to get the cached value
-            if key in cache:
-                value_timestamp, value = cache[key]
-                if time() - value_timestamp < ttl:
-                    return value
-                else:
-                    # If the item has expired, remove it from the cache
-                    del cache[key]
-
-            # Call the actual function
-            result = func(*args, **kwargs)
-
-            # Conditionally cache the result
-            if condition(result):
-                # Store with current timestamp
-                cache[key] = (time(), result)
-
-            return result
-
-        # Expose a method to remove an item from the cache
-        def cache_remove(*args, **kwargs):
-            key = _make_key(args, kwargs, typed)
-            if key in cache:
-                del cache[key]
-
-        wrapper.cache_remove = cache_remove
-        # Expose a method to clear the full cache
-        wrapper.cache_clear = lambda: cache.clear()
-
-        return wrapper
-
+from __future__ import annotations
+from functools import wraps, _make_key
+from circular_dict import CircularDict
+from time import time
+
+def conditional_lru_cache(maxsize: int=128, typed: bool = False, condition: callable = lambda x: True):
+    cache = CircularDict(maxlen=maxsize)
+
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            # create a hashable cache key
+            key = _make_key(args, kwargs, typed)
+
+            # Attempt to get the cached value
+            if key in cache:
+                return cache[key]
+
+            # Call the actual function
+            result = func(*args, **kwargs)
+
+            # Conditionally cache the result
+            if condition(result):
+                cache[key] = result
+
+            return result
+
+        # Expose a method to remove an item from the cache
+        def cache_remove(*args, **kwargs):
+            key = _make_key(args, kwargs, typed)
+            cache.pop(key, None)  # Use pop to avoid KeyError if the key is not present
+
+
+        wrapper.cache_remove = cache_remove
+        # Expose a method to clear the full cache
+        wrapper.cache_clear = lambda: cache.clear()
+
+        return wrapper
+
+    return decorator
+
+def conditional_ttl_cache(maxsize: int = 128, typed: int = False, ttl: int = 60, condition: callable = lambda x: True):
+    cache = CircularDict(maxlen=maxsize)
+
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            # create a hashable cache key
+            key = _make_key(args, kwargs, typed)
+
+            # Attempt to get the cached value
+            if key in cache:
+                value_timestamp, value = cache[key]
+                if time() - value_timestamp < ttl:
+                    return value
+                else:
+                    # If the item has expired, remove it from the cache
+                    del cache[key]
+
+            # Call the actual function
+            result = func(*args, **kwargs)
+
+            # Conditionally cache the result
+            if condition(result):
+                # Store with current timestamp
+                cache[key] = (time(), result)
+
+            return result
+
+        # Expose a method to remove an item from the cache
+        def cache_remove(*args, **kwargs):
+            key = _make_key(args, kwargs, typed)
+            if key in cache:
+                del cache[key]
+
+        wrapper.cache_remove = cache_remove
+        # Expose a method to clear the full cache
+        wrapper.cache_clear = lambda: cache.clear()
+
+        return wrapper
+
     return decorator
```

### Comparing `conditional-cache-1.1.0/setup.py` & `conditional_cache-1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='conditional-cache',
-    version='1.1.0',
-    author='Eric-Canas',
-    author_email='eric@ericcanas.com',
-    url='https://github.com/Eric-Canas/ConditionalCache',
-    description='Conditional cache is a wrapper over functools.lru_cache that allows '
-                'for conditionally caching based on the output of the function.',
-    long_description=open('README.md', 'r').read(),
-    long_description_content_type='text/markdown',
-    license='MIT',
-    packages=find_packages(),
-    install_requires=[
-        'circular-dict',
-    ],
-    python_requires='>=3.6',
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Operating System :: OS Independent',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Utilities',
-        'Topic :: System :: Hardware'
-    ],
+from setuptools import setup, find_packages
+
+setup(
+    name='conditional-cache',
+    version='1.2',
+    author='Eric-Canas',
+    author_email='eric@ericcanas.com',
+    url='https://github.com/Eric-Canas/ConditionalCache',
+    description='Conditional cache is a wrapper over functools.lru_cache that allows '
+                'for conditionally caching based on the output of the function.',
+    long_description=open('README.md', 'r').read(),
+    long_description_content_type='text/markdown',
+    license='MIT',
+    packages=find_packages(),
+    install_requires=[
+        'circular-dict',
+    ],
+    python_requires='>=3.6',
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Operating System :: OS Independent',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Utilities',
+        'Topic :: System :: Hardware'
+    ],
 )
```

