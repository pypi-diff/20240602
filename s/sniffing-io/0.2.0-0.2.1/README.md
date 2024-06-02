# Comparing `tmp/sniffing_io-0.2.0.tar.gz` & `tmp/sniffing_io-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffing_io-0.2.0.tar", last modified: Thu May 30 18:41:29 2024, max compression
+gzip compressed data, was "sniffing_io-0.2.1.tar", last modified: Sun Jun  2 07:23:45 2024, max compression
```

## Comparing `sniffing_io-0.2.0.tar` & `sniffing_io-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 18:41:29.891383 sniffing_io-0.2.0/
--rw-rw-rw-   0        0        0       44 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6214 2024-05-30 18:41:29.891383 sniffing_io-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5339 2024-03-07 09:00:19.000000 sniffing_io-0.2.0/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 sniffing_io-0.2.0/build.py
--rw-rw-rw-   0        0        0       13 2024-05-14 06:59:25.000000 sniffing_io-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 18:41:29.891383 sniffing_io-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1546 2024-05-30 18:39:41.000000 sniffing_io-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:41:29.890382 sniffing_io-0.2.0/sniffing_io.egg-info/
--rw-rw-rw-   0        0        0     6214 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/sniffing_io.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/sniffing_io.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/sniffing_io.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/sniffing_io.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/sniffing_io.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 18:41:29.889381 sniffing_io-0.2.0/sniffingio/
--rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing_io-0.2.0/sniffingio/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing_io-0.2.0/sniffingio/callbacks.py
--rw-rw-rw-   0        0        0      904 2024-05-30 18:24:06.000000 sniffing_io-0.2.0/sniffingio/data.py
--rw-rw-rw-   0        0        0    10667 2024-05-30 18:28:33.000000 sniffing_io-0.2.0/sniffingio/filters.py
--rw-rw-rw-   0        0        0     2514 2024-05-30 17:52:46.000000 sniffing_io-0.2.0/sniffingio/sniff.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:23:45.611850 sniffing_io-0.2.1/
+-rw-rw-rw-   0        0        0       44 2024-06-02 07:23:45.000000 sniffing_io-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6214 2024-06-02 07:23:45.611850 sniffing_io-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5339 2024-03-07 09:00:19.000000 sniffing_io-0.2.1/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 sniffing_io-0.2.1/build.py
+-rw-rw-rw-   0        0        0       13 2024-05-14 06:59:25.000000 sniffing_io-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 07:23:45.611850 sniffing_io-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2024-06-02 07:23:42.000000 sniffing_io-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:23:45.610781 sniffing_io-0.2.1/sniffing_io.egg-info/
+-rw-rw-rw-   0        0        0     6214 2024-06-02 07:23:45.000000 sniffing_io-0.2.1/sniffing_io.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-06-02 07:23:45.000000 sniffing_io-0.2.1/sniffing_io.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 07:23:45.000000 sniffing_io-0.2.1/sniffing_io.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-06-02 07:23:45.000000 sniffing_io-0.2.1/sniffing_io.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-02 07:23:45.000000 sniffing_io-0.2.1/sniffing_io.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 07:23:45.610576 sniffing_io-0.2.1/sniffingio/
+-rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing_io-0.2.1/sniffingio/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing_io-0.2.1/sniffingio/callbacks.py
+-rw-rw-rw-   0        0        0      904 2024-05-30 18:24:06.000000 sniffing_io-0.2.1/sniffingio/data.py
+-rw-rw-rw-   0        0        0    10749 2024-06-02 07:23:06.000000 sniffing_io-0.2.1/sniffingio/filters.py
+-rw-rw-rw-   0        0        0     2514 2024-05-30 17:52:46.000000 sniffing_io-0.2.1/sniffingio/sniff.py
```

### Comparing `sniffing_io-0.2.0/PKG-INFO` & `sniffing_io-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffing-io
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 Home-page: https://github.com/Shahaf-F-S/sniffing-io
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sniffing_io-0.2.0/README.md` & `sniffing_io-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sniffing_io-0.2.0/build.py` & `sniffing_io-0.2.1/build.py`

 * *Files identical despite different names*

### Comparing `sniffing_io-0.2.0/setup.py` & `sniffing_io-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sniffing-io',
-        version='0.2.0',
+        version='0.2.1',
         description=(
             "A simple package for packet sniffing, "
             "with static/dynamic filtering options, "
             "real-time reaction, I/O operations and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sniffing_io-0.2.0/sniffing_io.egg-info/PKG-INFO` & `sniffing_io-0.2.1/sniffing_io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffing-io
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 Home-page: https://github.com/Shahaf-F-S/sniffing-io
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sniffing_io-0.2.0/sniffingio/callbacks.py` & `sniffing_io-0.2.1/sniffingio/callbacks.py`

 * *Files identical despite different names*

### Comparing `sniffing_io-0.2.0/sniffingio/data.py` & `sniffing_io-0.2.1/sniffingio/data.py`

 * *Files identical despite different names*

### Comparing `sniffing_io-0.2.0/sniffingio/filters.py` & `sniffing_io-0.2.1/sniffingio/filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,53 +11,71 @@
 __all__ = [
     "PacketFilterOperand",
     "PacketFilter",
     "PacketFilterIntersection",
     "PacketFilterOperator",
     "PacketFilterUnion",
     "PacketFilterNegation",
-    "BasePacketFilterUnion",
+    "UnionUtils",
     "BasePacketFilter",
     "StaticPacketFilter",
-    "BasePacketFilterOperator",
-    "BasePacketFilterIntersection",
+    "Utils",
+    "IntersectionUtils",
     "format_packet_filters",
     "LivePacketFilter",
     "dump_packet_filter",
     "load_packet_filter",
     "PacketFilterValues",
-    "Types",
     "Names",
     "pf",
     "pfv"
 ]
 
 def wrap(value: str) -> str:
 
     if (" " in value) and not (value.startswith("(") and value.endswith(")")):
         value = f"({value})"
 
     return value
 
 class Names:
 
+    IP = 'ip'
     HOST = 'host'
     PORT = 'port'
     SRC = 'src'
     DST = 'dst'
-
-class Types:
-
+    ETHER = 'ether'
+    NET = 'net'
+    MASK = 'mask'
     TCP = 'tcp'
     UDP = 'udp'
     ICMP = 'icmp'
     SMTP = 'smtp'
     MAC = 'mac'
+    PORT_RANGE = 'portrange'
+    LESS = 'less'
+    GREATER = 'greater'
+    PROTO = 'proto'
+    BROADCAST = 'broadcast'
+    MULTICAST = 'multicast'
+    VLAN = 'vlan'
+    MPLS = 'mpls'
+    ARP = 'arp'
+    FDDI = 'fddi'
+    IP6 = 'ip6'
+    LINK = 'link'
+    PPP = 'ppp'
+    RADIO = 'radio'
+    RARP = 'rarp'
+    SLIP = 'slip'
+    TR = 'tr'
+    WLAN = 'wlan'
 
-class BasePacketFilterOperator(metaclass=ABCMeta):
+class Utils(metaclass=ABCMeta):
 
     @staticmethod
     def format_join(values: Iterable[str], joiner: str) -> str:
 
         if not values:
             return ""
 
@@ -66,33 +84,29 @@
         if len(values) == 1:
             return wrap(values[0])
 
         data = f" {joiner} ".join(wrap(value) for value in values if value)
 
         return f"({data})"
 
-class BasePacketFilterUnion(BasePacketFilterOperator, metaclass=ABCMeta):
+class UnionUtils(Utils, metaclass=ABCMeta):
 
     @classmethod
     def format_union(cls, values: Iterable[str]) -> str:
 
         return cls.format_join(values, joiner="or")
 
-class BasePacketFilterIntersection(BasePacketFilterOperator, metaclass=ABCMeta):
+class IntersectionUtils(Utils, metaclass=ABCMeta):
 
     @classmethod
     def format_intersection(cls, values: Iterable[str]) -> str:
 
         return cls.format_join(values, joiner="and")
 
-class BasePacketFilter(
-    BasePacketFilterUnion,
-    BasePacketFilterIntersection,
-    metaclass=ABCMeta
-):
+class BasePacketFilter(UnionUtils, IntersectionUtils, metaclass=ABCMeta):
 
     @abstractmethod
     def format(self) -> str:
 
         return ""
 
 @dataclass(slots=True, frozen=True)
@@ -180,26 +194,26 @@
     filters: tuple[PacketFilterOperand, ...]
 
     def __len__(self) -> int:
 
         return len(self.filters)
 
 @dataclass(slots=True, frozen=True)
-class PacketFilterUnion(PacketFilterOperator, BasePacketFilterUnion):
+class PacketFilterUnion(PacketFilterOperator, UnionUtils):
 
     def format(self) -> str:
 
         return self.format_union((f.format() for f in self.filters or ()))
 
     def match(self, packet: Packet) -> bool:
 
         return any(f.match(packet) for f in self.filters)
 
 @dataclass(slots=True, frozen=True)
-class PacketFilterIntersection(PacketFilterOperator, BasePacketFilterIntersection):
+class PacketFilterIntersection(PacketFilterOperator, IntersectionUtils):
 
     def format(self) -> str:
 
         return self.format_intersection((f.format() for f in self.filters or ()))
 
     def match(self, packet: Packet) -> bool:
 
@@ -219,26 +233,15 @@
         if not data:
             return ""
 
         return f"(not {data})"
 
     def match(self, packet: Packet) -> bool:
 
-        return self.filter.match(packet)
-
-def layers_names(packet: Packet) -> list[str]:
-
-    names = [packet.name]
-
-    while packet.payload:
-        packet = packet.payload
-
-        names.append(packet.name)
-
-    return names
+        return not self.filter.match(packet)
 
 @dataclass(slots=True, frozen=True)
 class PacketFilterValues[T](PacketFilterOperand):
 
     types: list[str] = None
     names: list[str] = None
     values: list[T] = None
@@ -356,15 +359,17 @@
             if not layer_filter.match(layer):
                 return False
 
         return True
 
     def format(self) -> str:
 
-        return self.format_intersection(layer.format() for layer in self.layers)
+        return self.format_intersection(
+            layer.format() for layer in self.layers if layer is not None
+        )
 
 def format_packet_filters(
         filters: BasePacketFilter | Iterable[BasePacketFilter],
         joiner: PacketFilterOperator = PacketFilterUnion
 ) -> str:
 
     if joiner is None:
```

### Comparing `sniffing_io-0.2.0/sniffingio/sniff.py` & `sniffing_io-0.2.1/sniffingio/sniff.py`

 * *Files identical despite different names*

