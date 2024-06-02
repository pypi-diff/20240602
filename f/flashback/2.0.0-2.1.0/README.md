# Comparing `tmp/flashback-2.0.0.tar.gz` & `tmp/flashback-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashback-2.0.0.tar", last modified: Thu Oct  5 12:57:08 2023, max compression
+gzip compressed data, was "flashback-2.1.0.tar", last modified: Sun Jun  2 00:54:17 2024, max compression
```

## Comparing `flashback-2.0.0.tar` & `flashback-2.1.0.tar`

### file list

```diff
@@ -1,103 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.032098 flashback-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2023-10-05 12:56:37.000000 flashback-2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-10-05 12:56:37.000000 flashback-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-05 12:56:37.000000 flashback-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2023-10-05 12:57:08.032098 flashback-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2023-10-05 12:56:37.000000 flashback-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.004098 flashback-2.0.0/flashback/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.004098 flashback-2.0.0/flashback/accessing/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/accessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/accessing/dig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/borg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.008098 flashback-2.0.0/flashback/caching/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/caching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.012098 flashback-2.0.0/flashback/caching/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/caching/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/caching/adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/caching/adapters/disk_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/caching/adapters/memcached_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/caching/adapters/memory_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/caching/adapters/redis_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9412 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/caching/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/caching/cached.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/classproperty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.016098 flashback-2.0.0/flashback/debugging/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/caller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.016098 flashback-2.0.0/flashback/debugging/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/filters/call_highlight_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/filters/decorator_operator_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/filters/type_highlight_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/get_call_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/get_callable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/get_frameinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/profiled.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.016098 flashback-2.0.0/flashback/debugging/styles/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/styles/jellybeans.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/debugging/xp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/encrypted_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.024098 flashback-2.0.0/flashback/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/_inflect.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/adverbize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/camelize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/kebabize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.024098 flashback-2.0.0/flashback/formatting/locales/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/locales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/locales/de.py
--rw-r--r--   0 runner    (1001) docker     (127)    17353 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/locales/en.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/locales/es.py
--rw-r--r--   0 runner    (1001) docker     (127)    11522 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/locales/fr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/ordinalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/oxford_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/parameterize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/pascalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/pluralize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/singularize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/snakeize.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/transliterate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/formatting/truncate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.028098 flashback-2.0.0/flashback/i16g/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/i16g/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/i16g/locale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.028098 flashback-2.0.0/flashback/importing/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/importing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/importing/import_class_from_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/importing/import_module_from_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.032098 flashback-2.0.0/flashback/iterating/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/iterating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/iterating/chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/iterating/compact.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/iterating/flat_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/iterating/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/iterating/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/iterating/renumerate.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/iterating/uniq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.032098 flashback-2.0.0/flashback/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/logging/affixed_stream_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/logging/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/logging/muted.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/retryable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/sampled.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-10-05 12:56:37.000000 flashback-2.0.0/flashback/timeoutable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:57:08.004098 flashback-2.0.0/flashback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2023-10-05 12:57:07.000000 flashback-2.0.0/flashback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2023-10-05 12:57:07.000000 flashback-2.0.0/flashback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 12:57:07.000000 flashback-2.0.0/flashback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-05 12:57:07.000000 flashback-2.0.0/flashback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-05 12:57:07.000000 flashback-2.0.0/flashback.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-10-05 12:56:37.000000 flashback-2.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-10-05 12:56:37.000000 flashback-2.0.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-05 12:56:37.000000 flashback-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 12:57:08.032098 flashback-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2023-10-05 12:56:37.000000 flashback-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.661113 flashback-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-06-02 00:53:57.000000 flashback-2.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-02 00:53:57.000000 flashback-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-06-02 00:53:57.000000 flashback-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-06-02 00:54:17.661113 flashback-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-06-02 00:53:57.000000 flashback-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.649113 flashback-2.1.0/flashback/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.653113 flashback-2.1.0/flashback/accessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/accessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/accessing/dig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/accessing/pick.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/accessing/values_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/borg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.653113 flashback-2.1.0/flashback/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.653113 flashback-2.1.0/flashback/caching/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/disk_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/memcached_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/memory_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/adapters/redis_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/caching/cached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/classproperty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.653113 flashback-2.1.0/flashback/debugging/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/debugging/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/filters/call_highlight_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/filters/decorator_operator_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/filters/type_highlight_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/get_call_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/get_callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/get_frameinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/profiled.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/debugging/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/styles/jellybeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/debugging/xp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/encrypted_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/_inflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/adverbize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/camelize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/kebabize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/formatting/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/locales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/locales/de.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17353 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/locales/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/locales/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11522 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/locales/fr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/ordinalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/oxford_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/pascalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/pluralize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/singularize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/snakeize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/transliterate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/formatting/truncate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/i16g/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/i16g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/i16g/locale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.657113 flashback-2.1.0/flashback/importing/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/importing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/importing/import_class_from_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/importing/import_module_from_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.661113 flashback-2.1.0/flashback/iterating/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/compact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/flat_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/renumerate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/uniq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/iterating/uniq_by.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.661113 flashback-2.1.0/flashback/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/logging/affixed_stream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/logging/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/logging/muted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/retryable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/sampled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-06-02 00:53:57.000000 flashback-2.1.0/flashback/timeoutable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 00:54:17.653113 flashback-2.1.0/flashback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-06-02 00:54:17.000000 flashback-2.1.0/flashback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-06-02 00:54:17.000000 flashback-2.1.0/flashback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 00:54:17.000000 flashback-2.1.0/flashback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-02 00:54:17.000000 flashback-2.1.0/flashback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 00:54:17.000000 flashback-2.1.0/flashback.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-06-02 00:53:57.000000 flashback-2.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-06-02 00:53:57.000000 flashback-2.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-02 00:53:57.000000 flashback-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 00:54:17.661113 flashback-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-06-02 00:53:57.000000 flashback-2.1.0/setup.py
```

### Comparing `flashback-2.0.0/CHANGELOG.md` & `flashback-2.1.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # Changelog
 
+## 2.1.0 (06/02/2024)
+
+- Added `iterating/uniq_by` to remove duplicates from an iterable while keeping the items' order with a user-supplied callable
+- Added `accessing/pick` to fetch key/value pairs with given keys from a dictionary
+- Added `accessing/values_at` to retrieves values from each given keys in dictionary
+- Updated `accessing/dig` to support sequences and their indices
+- Fixed `iterating/flat_map` to correctly load flatten method
+- Typed the methods listed above
+- Updated dependencies
+
 ## 2.0.0 (05/10/2023)
 
 - Dropped support for Python 3.7
-- Added python 3.11 in the CI tests
+- Added python 3.12 in the CI tests
 - Updated dependencies
 
 ## 1.4.2 (04/07/2023)
 
 - Updated dependencies
 - Updated github actions
 - Updated pypi upload
```

### Comparing `flashback-2.0.0/LICENSE` & `flashback-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/PKG-INFO` & `flashback-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashback
-Version: 2.0.0
+Version: 2.1.0
 Summary: An utility library for python
 Home-page: https://github.com/PaulRenvoise/flashback
 Author: Paul Renvoisé
 Author-email: renvoisepaul@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -53,15 +53,17 @@
 ```
 
 ## Contents
 
 Flashback's helpers are currently organised within 7 modules, and global helpers:
 
 - `accessing/`
-    - `dig()` recursively fetch keys in a nested dict
+    - `dig()` recursively fetch keys and indices in a nested dict or sequence
+    - `values_at()` retrieves values from each given keys in dictionary
+    - `pick()` fetches key/value pairs with given keys from a dictionary
 - `caching/`
     - `Cache` supports several cache stores: in-memory, disk, Redis, and Memcached
     - `@cached` caches a callable's return value based on its arguments
 - `debugging/`
     - `xp()` prints debug information about its given arguments
     - `@profiled` collects and dumps profiling stats over a callable's execution
     - `caller()` allows a developer to print debug information about a callable's caller
@@ -82,14 +84,15 @@
     - `singularize()` returns the singular form of a given word
     - `pluralize()` returns the plural form of a given word
 - `iterating/`
     - `renumerate()` enumerates an iterable starting from its end
     - `chunks()` splits an iterable into smaller chunks, padding them if requested
     - `partition()` splits an iterable into items validating a predicate and the ones that don't
     - `uniq()` removes duplicates from an iterable while keeping the items' order
+    - `uniq_by()` removes duplicates defined via a user-supplied callable from an iterable while keeping the items' order
     - `compact()` removes None values from an iterable
     - `flatten()` unpacks nested iterable into the given iterable
     - `flat_map()` applies a function to every item and nested item of the given iterable
 - `i16g/`
     - `Locale` dynamically loads localization files from a package path
 - `importing/`
     - `import_class_from_path()` fetches a class from a package path and returns it
```

### Comparing `flashback-2.0.0/README.md` & `flashback-2.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 ```
 
 ## Contents
 
 Flashback's helpers are currently organised within 7 modules, and global helpers:
 
 - `accessing/`
-    - `dig()` recursively fetch keys in a nested dict
+    - `dig()` recursively fetch keys and indices in a nested dict or sequence
+    - `values_at()` retrieves values from each given keys in dictionary
+    - `pick()` fetches key/value pairs with given keys from a dictionary
 - `caching/`
     - `Cache` supports several cache stores: in-memory, disk, Redis, and Memcached
     - `@cached` caches a callable's return value based on its arguments
 - `debugging/`
     - `xp()` prints debug information about its given arguments
     - `@profiled` collects and dumps profiling stats over a callable's execution
     - `caller()` allows a developer to print debug information about a callable's caller
@@ -55,14 +57,15 @@
     - `singularize()` returns the singular form of a given word
     - `pluralize()` returns the plural form of a given word
 - `iterating/`
     - `renumerate()` enumerates an iterable starting from its end
     - `chunks()` splits an iterable into smaller chunks, padding them if requested
     - `partition()` splits an iterable into items validating a predicate and the ones that don't
     - `uniq()` removes duplicates from an iterable while keeping the items' order
+    - `uniq_by()` removes duplicates defined via a user-supplied callable from an iterable while keeping the items' order
     - `compact()` removes None values from an iterable
     - `flatten()` unpacks nested iterable into the given iterable
     - `flat_map()` applies a function to every item and nested item of the given iterable
 - `i16g/`
     - `Locale` dynamically loads localization files from a package path
 - `importing/`
     - `import_class_from_path()` fetches a class from a package path and returns it
```

### Comparing `flashback-2.0.0/flashback/__init__.py` & `flashback-2.1.0/flashback/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     "deprecated",
     "retryable",
     "sampled",
     "timed",
     "timeoutable",
 )
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
```

### Comparing `flashback-2.0.0/flashback/borg.py` & `flashback-2.1.0/flashback/borg.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/caching/adapters/base.py` & `flashback-2.1.0/flashback/caching/adapters/base.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/caching/adapters/disk_adapter.py` & `flashback-2.1.0/flashback/caching/adapters/disk_adapter.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/caching/adapters/memcached_adapter.py` & `flashback-2.1.0/flashback/caching/adapters/memcached_adapter.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/caching/adapters/memory_adapter.py` & `flashback-2.1.0/flashback/caching/adapters/memory_adapter.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/caching/adapters/redis_adapter.py` & `flashback-2.1.0/flashback/caching/adapters/redis_adapter.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/caching/cache.py` & `flashback-2.1.0/flashback/caching/cache.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/caching/cached.py` & `flashback-2.1.0/flashback/caching/cached.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/classproperty.py` & `flashback-2.1.0/flashback/classproperty.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/debugging/caller.py` & `flashback-2.1.0/flashback/debugging/caller.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/debugging/filters/call_highlight_filter.py` & `flashback-2.1.0/flashback/debugging/filters/call_highlight_filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,9 +47,8 @@
             if previous_ttype in Name and value == "(":
                 stack.append((Name.Function, previous_value))
             else:
                 stack.append((previous_ttype, previous_value))
 
             stack.append((ttype, value))
 
-        for items in stack:
-            yield items
+        yield from stack
```

### Comparing `flashback-2.0.0/flashback/debugging/filters/decorator_operator_filter.py` & `flashback-2.1.0/flashback/debugging/filters/decorator_operator_filter.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/debugging/filters/type_highlight_filter.py` & `flashback-2.1.0/flashback/debugging/filters/type_highlight_filter.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/debugging/formatter.py` & `flashback-2.1.0/flashback/debugging/formatter.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/debugging/get_call_context.py` & `flashback-2.1.0/flashback/debugging/get_call_context.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/debugging/get_callable.py` & `flashback-2.1.0/flashback/debugging/get_callable.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/debugging/get_frameinfo.py` & `flashback-2.1.0/flashback/debugging/get_frameinfo.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/debugging/parser.py` & `flashback-2.1.0/flashback/debugging/parser.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/debugging/profiled.py` & `flashback-2.1.0/flashback/debugging/profiled.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/debugging/styles/jellybeans.py` & `flashback-2.1.0/flashback/debugging/styles/jellybeans.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/debugging/xp.py` & `flashback-2.1.0/flashback/debugging/xp.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/deprecated.py` & `flashback-2.1.0/flashback/deprecated.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/encrypted_file.py` & `flashback-2.1.0/flashback/encrypted_file.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/__init__.py` & `flashback-2.1.0/flashback/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/_inflect.py` & `flashback-2.1.0/flashback/formatting/_inflect.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/adverbize.py` & `flashback-2.1.0/flashback/formatting/adverbize.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/camelize.py` & `flashback-2.1.0/flashback/formatting/camelize.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/kebabize.py` & `flashback-2.1.0/flashback/formatting/kebabize.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/locales/de.py` & `flashback-2.1.0/flashback/formatting/locales/de.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/locales/en.py` & `flashback-2.1.0/flashback/formatting/locales/en.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/locales/es.py` & `flashback-2.1.0/flashback/formatting/locales/es.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/locales/fr.py` & `flashback-2.1.0/flashback/formatting/locales/fr.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/ordinalize.py` & `flashback-2.1.0/flashback/formatting/ordinalize.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/oxford_join.py` & `flashback-2.1.0/flashback/formatting/oxford_join.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/parameterize.py` & `flashback-2.1.0/flashback/formatting/parameterize.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/pascalize.py` & `flashback-2.1.0/flashback/formatting/pascalize.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/pluralize.py` & `flashback-2.1.0/flashback/formatting/pluralize.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/singularize.py` & `flashback-2.1.0/flashback/formatting/singularize.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/snakeize.py` & `flashback-2.1.0/flashback/formatting/snakeize.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/transliterate.py` & `flashback-2.1.0/flashback/formatting/transliterate.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/formatting/truncate.py` & `flashback-2.1.0/flashback/formatting/truncate.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/i16g/locale.py` & `flashback-2.1.0/flashback/i16g/locale.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/importing/import_class_from_path.py` & `flashback-2.1.0/flashback/importing/import_class_from_path.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/importing/import_module_from_path.py` & `flashback-2.1.0/flashback/importing/import_module_from_path.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/iterating/chunks.py` & `flashback-2.1.0/flashback/iterating/chunks.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/iterating/compact.py` & `flashback-2.1.0/flashback/iterating/compact.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/iterating/flat_map.py` & `flashback-2.1.0/flashback/iterating/flat_map.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from . import flatten
+from __future__ import annotations
 
+from typing import Any, Callable, Sequence
 
-def flat_map(func, iterable):
+from .flatten import flatten
+
+
+def flat_map(func: Callable[[Any], Any], iterable: Sequence[Any]) -> map:
     """
     Applies the function `func` to each item and nested item of `iterable`.
 
     Examples:
         ```python
         from flashback.iterating import flat_map
 
@@ -17,15 +21,16 @@
         #=> 8
         #=> 10
 
         assert list(flat_map(lambda x: x / 2, [1, {2, 3}, (4,), range(5, 6)]) == [0.5, 1, 1.5, 2, 2.5, 3]
         ```
 
     Params:
-        iterable (Iterable<Any>): the iterable to flatten and map
+        func: the callable to apply on each item of the iterable
+        iterable: the iterable to flatten and map
 
     Returns:
-        map<Any>: the flattened and mapped iterable
+        the flattened and mapped iterable
     """
     flattened_iterable = flatten(iterable)
 
     return map(func, flattened_iterable)
```

### Comparing `flashback-2.0.0/flashback/iterating/flatten.py` & `flashback-2.1.0/flashback/iterating/flatten.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/iterating/partition.py` & `flashback-2.1.0/flashback/iterating/partition.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/iterating/renumerate.py` & `flashback-2.1.0/flashback/iterating/renumerate.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/iterating/uniq.py` & `flashback-2.1.0/flashback/iterating/uniq.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-def uniq(iterable):
+from __future__ import annotations
+
+from typing import Any, Iterable
+
+
+def uniq(iterable: Iterable[Any]) -> tuple[Any]:
     """
     Removes duplicates items from `iterable` while keeping their order.
 
     Examples:
         ```python
         from flashback.iterating import uniq
 
@@ -14,18 +19,18 @@
         #=> 19475
 
         # Keeps order
         assert set([1, 1, 3, 4, 5, 5]) != uniq([1, 1, 3, 4, 5, 5])
         ```
 
     Params:
-        iterable (Iterable<Any>): the iterable to remove duplicates from
+        iterable: the iterable to remove duplicates from
 
     Returns:
-        tuple<Any>: the iterable without duplicates
+        the iterable without duplicates
     """
     unique = []
     seen = set()
 
     for item in iterable:
         repr_item = repr(item)
         if repr_item in seen:
```

### Comparing `flashback-2.0.0/flashback/logging/__init__.py` & `flashback-2.1.0/flashback/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/logging/affixed_stream_handler.py` & `flashback-2.1.0/flashback/logging/affixed_stream_handler.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/logging/configurations.py` & `flashback-2.1.0/flashback/logging/configurations.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/logging/muted.py` & `flashback-2.1.0/flashback/logging/muted.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/retryable.py` & `flashback-2.1.0/flashback/retryable.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/sampled.py` & `flashback-2.1.0/flashback/sampled.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/sentinel.py` & `flashback-2.1.0/flashback/sentinel.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/singleton.py` & `flashback-2.1.0/flashback/singleton.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/timed.py` & `flashback-2.1.0/flashback/timed.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback/timeoutable.py` & `flashback-2.1.0/flashback/timeoutable.py`

 * *Files identical despite different names*

### Comparing `flashback-2.0.0/flashback.egg-info/PKG-INFO` & `flashback-2.1.0/flashback.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashback
-Version: 2.0.0
+Version: 2.1.0
 Summary: An utility library for python
 Home-page: https://github.com/PaulRenvoise/flashback
 Author: Paul Renvoisé
 Author-email: renvoisepaul@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -53,15 +53,17 @@
 ```
 
 ## Contents
 
 Flashback's helpers are currently organised within 7 modules, and global helpers:
 
 - `accessing/`
-    - `dig()` recursively fetch keys in a nested dict
+    - `dig()` recursively fetch keys and indices in a nested dict or sequence
+    - `values_at()` retrieves values from each given keys in dictionary
+    - `pick()` fetches key/value pairs with given keys from a dictionary
 - `caching/`
     - `Cache` supports several cache stores: in-memory, disk, Redis, and Memcached
     - `@cached` caches a callable's return value based on its arguments
 - `debugging/`
     - `xp()` prints debug information about its given arguments
     - `@profiled` collects and dumps profiling stats over a callable's execution
     - `caller()` allows a developer to print debug information about a callable's caller
@@ -82,14 +84,15 @@
     - `singularize()` returns the singular form of a given word
     - `pluralize()` returns the plural form of a given word
 - `iterating/`
     - `renumerate()` enumerates an iterable starting from its end
     - `chunks()` splits an iterable into smaller chunks, padding them if requested
     - `partition()` splits an iterable into items validating a predicate and the ones that don't
     - `uniq()` removes duplicates from an iterable while keeping the items' order
+    - `uniq_by()` removes duplicates defined via a user-supplied callable from an iterable while keeping the items' order
     - `compact()` removes None values from an iterable
     - `flatten()` unpacks nested iterable into the given iterable
     - `flat_map()` applies a function to every item and nested item of the given iterable
 - `i16g/`
     - `Locale` dynamically loads localization files from a package path
 - `importing/`
     - `import_class_from_path()` fetches a class from a package path and returns it
```

### Comparing `flashback-2.0.0/flashback.egg-info/SOURCES.txt` & `flashback-2.1.0/flashback.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 flashback.egg-info/PKG-INFO
 flashback.egg-info/SOURCES.txt
 flashback.egg-info/dependency_links.txt
 flashback.egg-info/requires.txt
 flashback.egg-info/top_level.txt
 flashback/accessing/__init__.py
 flashback/accessing/dig.py
+flashback/accessing/pick.py
+flashback/accessing/values_at.py
 flashback/caching/__init__.py
 flashback/caching/cache.py
 flashback/caching/cached.py
 flashback/caching/adapters/__init__.py
 flashback/caching/adapters/base.py
 flashback/caching/adapters/disk_adapter.py
 flashback/caching/adapters/memcached_adapter.py
@@ -76,11 +78,12 @@
 flashback/iterating/chunks.py
 flashback/iterating/compact.py
 flashback/iterating/flat_map.py
 flashback/iterating/flatten.py
 flashback/iterating/partition.py
 flashback/iterating/renumerate.py
 flashback/iterating/uniq.py
+flashback/iterating/uniq_by.py
 flashback/logging/__init__.py
 flashback/logging/affixed_stream_handler.py
 flashback/logging/configurations.py
 flashback/logging/muted.py
```

### Comparing `flashback-2.0.0/setup.py` & `flashback-2.1.0/setup.py`

 * *Files identical despite different names*

