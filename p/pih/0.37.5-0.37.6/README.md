# Comparing `tmp/pih-0.37.5.tar.gz` & `tmp/pih-0.37.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.37.5.tar", last modified: Fri May 31 07:39:56 2024, max compression
+gzip compressed data, was "pih-0.37.6.tar", last modified: Sun Jun  2 06:19:25 2024, max compression
```

## Comparing `pih-0.37.5.tar` & `pih-0.37.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 07:39:56.767637 pih-0.37.5/
--rw-rw-rw-   0        0        0      249 2024-05-31 07:39:56.736312 pih-0.37.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-31 07:39:53.396544 pih-0.37.5/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.37.5/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:39:54.104358 pih-0.37.5/pih/collections/
--rw-rw-rw-   0        0        0    30339 2024-05-17 03:55:00.000000 pih-0.37.5/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.37.5/pih/collections/service.py
--rw-rw-rw-   0        0        0   104226 2024-05-20 23:34:54.000000 pih-0.37.5/pih/console_api.py
--rw-rw-rw-   0        0        0     2549 2024-05-19 11:56:07.000000 pih-0.37.5/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:39:55.951937 pih-0.37.5/pih/consts/
--rw-rw-rw-   0        0        0    26746 2024-05-31 07:36:35.000000 pih-0.37.5/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3694 2024-05-18 23:37:39.000000 pih-0.37.5/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1768 2024-05-08 05:34:18.000000 pih-0.37.5/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      974 2024-04-21 23:56:33.000000 pih-0.37.5/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.37.5/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-05-20 02:54:33.000000 pih-0.37.5/pih/consts/errors.py
--rw-rw-rw-   0        0        0    30003 2024-04-22 02:31:56.000000 pih-0.37.5/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.37.5/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.37.5/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.37.5/pih/consts/hosts.py
--rw-rw-rw-   0        0        0      194 2024-04-17 15:27:11.000000 pih-0.37.5/pih/consts/iot.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.37.5/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.37.5/pih/consts/password.py
--rw-rw-rw-   0        0        0    12272 2024-05-13 03:26:35.000000 pih-0.37.5/pih/consts/paths.py
--rw-rw-rw-   0        0        0    16022 2024-05-21 01:27:45.000000 pih-0.37.5/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.37.5/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.37.5/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.37.5/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.37.5/pih/consts/service.py
--rw-rw-rw-   0        0        0     6540 2024-04-17 04:46:50.000000 pih-0.37.5/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12120 2024-05-12 15:14:12.000000 pih-0.37.5/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    17786 2024-05-31 07:35:10.000000 pih-0.37.5/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.37.5/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      233 2024-05-17 04:55:05.000000 pih-0.37.5/pih/consts/style.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.37.5/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   572684 2024-05-31 07:34:35.000000 pih-0.37.5/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:39:56.500996 pih-0.37.5/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.37.5/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.37.5/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.37.5/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.37.5/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:39:56.641546 pih-0.37.5/pih/tools/
--rw-rw-rw-   0        0        0    59109 2024-05-28 21:42:09.000000 pih-0.37.5/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.37.5/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.37.5/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:39:56.704042 pih-0.37.5/pih.egg-info/
--rw-rw-rw-   0        0        0      249 2024-05-31 07:39:52.000000 pih-0.37.5/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      976 2024-05-31 07:39:52.000000 pih-0.37.5/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 07:39:52.000000 pih-0.37.5/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-31 07:39:52.000000 pih-0.37.5/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-31 07:39:52.000000 pih-0.37.5/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 07:39:56.767637 pih-0.37.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 06:19:25.961859 pih-0.37.6/
+-rw-rw-rw-   0        0        0      249 2024-06-02 06:19:25.934199 pih-0.37.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 06:19:23.601651 pih-0.37.6/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.37.6/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 06:19:24.011015 pih-0.37.6/pih/collections/
+-rw-rw-rw-   0        0        0    30390 2024-06-02 05:41:57.000000 pih-0.37.6/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.37.6/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104105 2024-06-02 05:49:47.000000 pih-0.37.6/pih/console_api.py
+-rw-rw-rw-   0        0        0     2549 2024-05-19 11:56:07.000000 pih-0.37.6/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-06-02 06:19:25.508260 pih-0.37.6/pih/consts/
+-rw-rw-rw-   0        0        0    26746 2024-06-02 06:18:45.000000 pih-0.37.6/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3694 2024-05-18 23:37:39.000000 pih-0.37.6/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1768 2024-05-08 05:34:18.000000 pih-0.37.6/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      974 2024-04-21 23:56:33.000000 pih-0.37.6/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.37.6/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-05-20 02:54:33.000000 pih-0.37.6/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    30003 2024-04-22 02:31:56.000000 pih-0.37.6/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.37.6/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.37.6/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.37.6/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0      194 2024-04-17 15:27:11.000000 pih-0.37.6/pih/consts/iot.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.37.6/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1168 2024-06-02 06:17:29.000000 pih-0.37.6/pih/consts/password.py
+-rw-rw-rw-   0        0        0    12272 2024-05-13 03:26:35.000000 pih-0.37.6/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    16022 2024-05-21 01:27:45.000000 pih-0.37.6/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.37.6/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.37.6/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.37.6/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.37.6/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6540 2024-04-17 04:46:50.000000 pih-0.37.6/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12120 2024-05-12 15:14:12.000000 pih-0.37.6/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    17786 2024-05-31 07:35:10.000000 pih-0.37.6/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.37.6/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      233 2024-05-17 04:55:05.000000 pih-0.37.6/pih/consts/style.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.37.6/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   573820 2024-06-02 05:41:57.000000 pih-0.37.6/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-06-02 06:19:25.715468 pih-0.37.6/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.37.6/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.37.6/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.37.6/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.37.6/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-06-02 06:19:25.840450 pih-0.37.6/pih/tools/
+-rw-rw-rw-   0        0        0    59109 2024-05-28 21:42:09.000000 pih-0.37.6/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.37.6/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.37.6/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-06-02 06:19:25.887324 pih-0.37.6/pih.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-06-02 06:19:22.000000 pih-0.37.6/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2024-06-02 06:19:22.000000 pih-0.37.6/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 06:19:22.000000 pih-0.37.6/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-06-02 06:19:22.000000 pih-0.37.6/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-06-02 06:19:22.000000 pih-0.37.6/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 06:19:25.975854 pih-0.37.6/setup.cfg
```

### Comparing `pih-0.37.5/pih/collections/__init__.py` & `pih-0.37.6/pih/collections/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import ipih
 
 from enum import Enum
 from collections import namedtuple
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta, date
-from typing import Any, Tuple, List, Callable, TypeVar, Generic
+from typing import Any, Tuple, List, Callable, TypeVar, Generic, TypeAlias
 
+strdict: TypeAlias = dict[str, Any]
 
 @dataclass
 class Host:
     name: str
     aliases: str | tuple[str, ...] | None = None
     ip: str | None = None
     description: str | None = None
@@ -596,15 +597,15 @@
     messageID: int | None = None
     type: int | None = None
 
 
 @dataclass
 class EventDS:
     name: str | None = None
-    parameters: dict | None = None
+    parameters: strdict | None = None
     timestamp: datetime | date | str | int | None = None
     id: int = 0
 
 
 @dataclass
 class Message:
     message: str | None = None
```

### Comparing `pih-0.37.5/pih/collections/service.py` & `pih-0.37.6/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/console_api.py` & `pih-0.37.6/pih/console_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -684,26 +684,25 @@
                                 ),
                             )
                         )
                     )
                     event_description = (
                         A.CT_E.POLIBASE_CREATION_ARCHIVED_DB_DUMP_COMPLETE
                     )
+
                     event = one(A.R_E.get_last(event_description))
                     self.output.write_line(
                         js(
                             (
                                 "",
                                 A.CT_V.BULLET,
                                 "Размер сжатого дампа бекапа базы данных:",
                                 self.bold(
                                     A.D_F.size(
-                                        event.parameters[
-                                            A.D.get(event_description).params[0].name
-                                        ],
+                                        A.D_Ex_E.value(event, 0),
                                         2,
                                         True,
                                     )
                                 ),
                             )
                         )
                     )
```

### Comparing `pih-0.37.5/pih/console_api_wrapper.py` & `pih-0.37.6/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/__init__.py` & `pih-0.37.6/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ZabbixResourceDescriptionDelegated,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.37.5"
+VERSION: str = "0.37.6"
 
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
```

### Comparing `pih-0.37.5/pih/consts/ad.py` & `pih-0.37.6/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/addresses.py` & `pih-0.37.6/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/date_time.py` & `pih-0.37.6/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/errors.py` & `pih-0.37.6/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/events.py` & `pih-0.37.6/pih/consts/events.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/hosts.py` & `pih-0.37.6/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/names.py` & `pih-0.37.6/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/password.py` & `pih-0.37.6/pih/consts/password.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,22 +19,23 @@
             3, "", RULES.DEFAULT_ORDER_LIST, 0, 3, 0, 0, False
         )
         NORMAL: PasswordSettings = PasswordSettings(
             8, "!@#", RULES.DEFAULT_ORDER_LIST, 3, 3, 1, 1, False
         )
         STRONG: PasswordSettings = PasswordSettings(
             10,
-            "#%+\-!=@()_",
+            r"#%+\-!=@()_",
             RULES.DEFAULT_ORDER_LIST,
             3,
             3,
             2,
             2,
             True,
         )
         DEFAULT: PasswordSettings = NORMAL
         PC: PasswordSettings = NORMAL
         EMAIL: PasswordSettings = NORMAL
 
+    @staticmethod
     def get(name: str) -> SETTINGS:
         return PASSWORD.__getattribute__(PASSWORD.SETTINGS, name)
```

### Comparing `pih-0.37.5/pih/consts/paths.py` & `pih-0.37.6/pih/consts/paths.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/polibase.py` & `pih-0.37.6/pih/consts/polibase.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/service.py` & `pih-0.37.6/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/service_commands.py` & `pih-0.37.6/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/service_roles.py` & `pih-0.37.6/pih/consts/service_roles.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/consts/settings.py` & `pih-0.37.6/pih/consts/settings.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/pih.py` & `pih-0.37.6/pih/pih.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from contextlib import contextmanager, redirect_stdout
 from pkg_resources import parse_version, working_set
 from urllib.parse import unquote, quote_plus, quote
 from concurrent.futures import ThreadPoolExecutor
 from requests import ConnectTimeout, Response
 from colorama import Back, Style, Fore, ansi
 from datetime import datetime, timedelta, date
-from typing import Any, Callable, TypeAlias
 from collections import defaultdict
 from prettytable import PrettyTable
 from colorama.ansi import CSI, OSC
 from transliterate import translit
+from typing import Any, Callable
 from concurrent import futures
 from random import randrange
 from threading import Thread
 from string import Formatter
 from grpc import StatusCode
 from getpass import getpass
 from functools import cache
@@ -55,15 +55,15 @@
 from pih.consts.settings import SETTINGS
 from pih.consts.ssh_hosts import SSHHosts
 from pih.consts.rpc import RPC as CONST_RPC
 from pih.consts.addresses import ADDRESSES, EMAIL_COLLECTION
 from pih.tools.service import ServiceRoleTool, ServiceTool, ServiceAdminTool
 from pih.consts.service import SUPPORT_NAME_PREFIX, EVENT_LISTENER_NAME_PREFIX
 
-strdict: TypeAlias = dict[str, Any]
+
 
 
 class PIHThreadPoolExecutor(ThreadPoolExecutor):
 
     wrapper: Callable
 
     def submit(self, fn, /, *args, **kwargs):
@@ -2888,15 +2888,15 @@
             try:
                 yield True
             except Exception as error:
                 PIH.ERROR.global_except_hook(error)
             finally:
                 if nn(final_action):
                     final_action()
-                    
+
         @staticmethod
         @contextmanager
         def detect_suppressing(final_action: Callable[[], None] | None = None):
             try:
                 yield True
             except BaseException:
                 pass
@@ -4106,24 +4106,35 @@
                         ),
                         show_output,
                     )
                 )
             )
 
         @staticmethod
-        def process_is_exists(
-            pid: int,
+        def check_process_is_running(
+            pid_or_name: int | str,
             host: str | None = None,
             login: str | None = None,
             password: str | None = None,
-        ) -> str:
+        ) -> bool:
+            value_is_str: bool = isinstance(pid_or_name, str)
+            if value_is_str:
+                pid_or_name = PIH.PATH.add_extension(pid_or_name, FILE.EXTENSION.EXE)
             command_list: list[str] = [
                 "tasklist",
                 "/fi",
-                js(("pid", "eq", pid)),
+                esc(
+                    js(
+                        (
+                            ["pid", "imagename"][value_is_str],
+                            "eq",
+                            pid_or_name,
+                        )
+                    )
+                ),
                 "/fo",
                 "list",
             ]
             login = PIH.DATA.FORMAT.login(
                 login
                 or PIH.DATA.VARIABLE.ENVIRONMENT.value(LINK.ADMINISTRATOR_LOGIN, False)
                 or AD.ADMINISTRATOR_LOGIN
@@ -5447,27 +5458,29 @@
                         can_use_standalone
                         or nn(service_description.standalone_name)
                         and service_description.use_standalone
                     )
                     if PIH.SYS.is_virtual_environment():
                         ipih_install = False
                         pih_install = False
+                        """
                         if as_standalone:
                             PIH.output.error(
                                 js(
                                     (
                                         "Sorry, you can not start service",
                                         esc(service_description.name),
                                         "in standalone mode for virtual environment.",
                                         nl(),
                                         "Service will be started in normal mode.",
                                     )
                                 )
                             )
                         as_standalone = False
+                        """
                     #
                     if pih_install:
                         pih_version_list: list[str] = PIH.UPDATER.versions(PIH.NAME)
                         pih_last_version: str = one(pih_version_list)
                         if nn(pih_version) and pih_version not in pih_version_list:
                             pih_version = None
                         pih_version = pih_version or pih_last_version
@@ -6913,23 +6926,25 @@
                         return None
                     for index, name in enumerate(event_ds.parameters):
                         if index == param_index:
                             return event_ds.parameters[name]
 
                 @staticmethod
                 def value(
-                    event_ds: EventDS | None, name_holder: str | ParamItem | None = None
+                    value: EventDS | None, name_holder: str | ParamItem | int | None = None
                 ) -> Any:
-                    if n(event_ds):
+                    if n(value):
                         return None
+                    if isinstance(name_holder, int):
+                        return DataTool.by_index(DataTool.to_list(value.parameters), name_holder)
                     return (
-                        event_ds.parameters
+                        value.parameters
                         if n(name_holder)
                         else DataTool.if_is_in(
-                            event_ds.parameters,
+                            value.parameters,
                             (
                                 name_holder
                                 if isinstance(name_holder, str)
                                 else name_holder.name
                             ),
                         )
                     )
@@ -8822,29 +8837,31 @@
                     PIH.RESULT.NOTES._all(
                         cached,
                         local,
                         CONST.FILES.SECTION,
                         Events.SAVE_FILE_FROM_KNOWLEDGE_BASE,
                     ),
                 )
-                
+
             @staticmethod
             def by_name(value: str) -> Result[File]:
                 return PIH.RESULT.FILES.find(value, strict_equality=True)
 
             @staticmethod
             def find(
                 value: str | None = None,
                 command_type: CommandTypes | None = None,
                 exclude_private_files: bool = False,
                 strict_equality: bool = False,
             ) -> Result[list[File]]:
                 value = lw(value)
-                search_function: Callable[[File], bool] = (
-                    lambda item: StringTool.contains(nns(item.title), nns(value)) if strict_equality else StringTool.full_right_intersection_by_tokens(
+                search_function: Callable[[File], bool] = lambda item: (
+                    StringTool.contains(nns(item.title), nns(value))
+                    if strict_equality
+                    else StringTool.full_right_intersection_by_tokens(
                         nns(item.title),
                         nns(value),
                         (" ", CONST.NAME_SPLITTER, CONST.SPLITTER, ","),
                     )
                 )
                 was_updated: bool = False
                 section: str = CONST.FILES.SECTION
@@ -8926,15 +8943,15 @@
                 catch_exceptions: bool = False,
                 use_default_stdout: bool = False,
             ) -> str | strdict | None:
                 file: File | None = one(PIH.RESULT.FILES.by_name(file_search_request))
                 if n(file):
                     return None
                 return PIH.EXECUTOR.execute_python_localy(
-                    nnt(file).text,  
+                    nnt(file).text,
                     parameters,
                     stdout_redirect,
                     catch_exceptions,
                     use_default_stdout,
                 )
 
             @staticmethod
@@ -11328,14 +11345,24 @@
                 r"^[a-z]+[a-z_0-9]{"
                 + str(CONST.NAME_POLICY.PART_ITEM_MIN_LENGTH - 1)
                 + ",}"
             )
             return re.fullmatch(pattern, value, re.IGNORECASE) is not None
 
         class COMPUTER:
+            
+            @staticmethod
+            def process_is_running(
+                pid_or_name: int | str,
+                host: str | None = None,
+                login: str | None = None,
+                password: str | None = None,
+            ) -> bool:
+                return PIH.EXECUTOR.check_process_is_running(pid_or_name, host, login, password)
+            
             @staticmethod
             def windows_service_running(
                 name: str, host: str, host_check_for_accessibility: bool = True
             ) -> bool | None:
                 accessable: bool | None = None
                 if host_check_for_accessibility:
                     accessable = PIH.CHECK.COMPUTER.accessibility(host)
@@ -11397,15 +11424,17 @@
             @staticmethod
             def rebootable(workstation: ComputerDescription) -> bool:
                 return PIH.CHECK.WORKSTATION.property(
                     workstation, AD.ComputerProperties.Rebootable
                 )
 
         @staticmethod
-        def telephone_number(value: str | int | None, international: bool = False) -> bool:
+        def telephone_number(
+            value: str | int | None, international: bool = False
+        ) -> bool:
             return (
                 ne(value)
                 and re.fullmatch(
                     ("" if international else r"^\+") + "[0-9]{11,13}$", str(value)
                 )
                 is not None
             )
@@ -12086,15 +12115,18 @@
                     value: str,
                     profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
                 ) -> bool:
                     profile, profile_value = (
                         PIH.MESSAGE.WHATSAPP.WAPPI._get_profile_value(profile)
                     )
                     url: str | None = None
-                    payload: dict = {"recipient": recipient, "body": PIH.DATA.FORMAT.whatsapp_message(value)}
+                    payload: dict = {
+                        "recipient": recipient,
+                        "body": PIH.DATA.FORMAT.whatsapp_message(value),
+                    }
                     url = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_MESSAGE
                     url = j((url, profile_value))
                     try:
                         response: Response = requests.post(
                             url,
                             data=dumps(payload),
                             headers=PIH.MESSAGE.WHATSAPP.WAPPI._get_header(profile),
@@ -12313,15 +12345,17 @@
 
             @staticmethod
             def send_to_user(
                 user: User,
                 message: Any,
                 via_wappi: bool = True,
                 use_alternative: bool = True,
-                wappi_profile: CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None = None,
+                wappi_profile: (
+                    CONST.MESSAGE.WHATSAPP.WAPPI.Profiles | str | None
+                ) = None,
             ) -> bool:
                 return PIH.MESSAGE.WHATSAPP.send(
                     user.telephoneNumber,
                     message,
                     via_wappi,
                     use_alternative,
                     EnumTool.get_value(
```

### Comparing `pih-0.37.5/pih/rpc/__init__.py` & `pih-0.37.6/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.37.6/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.37.6/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/tools/__init__.py` & `pih-0.37.6/pih/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/tools/service.py` & `pih-0.37.6/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih/widgets.py` & `pih-0.37.6/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.5/pih.egg-info/SOURCES.txt` & `pih-0.37.6/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

