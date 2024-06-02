# Comparing `tmp/yet_another_io_channels_library-0.2.4.tar.gz` & `tmp/yet_another_io_channels_library-0.2.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet_another_io_channels_library-0.2.4.tar", max compression
+gzip compressed data, was "yet_another_io_channels_library-0.2.4.post1.tar", max compression
```

## Comparing `yet_another_io_channels_library-0.2.4.tar` & `yet_another_io_channels_library-0.2.4.post1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2018-10-14 15:23:38.622748 yet_another_io_channels_library-0.2.4/LICENSE
--rw-r--r--   0        0        0     3934 2024-05-26 21:32:04.553960 yet_another_io_channels_library-0.2.4/README.md
--rw-r--r--   0        0        0       82 2018-10-25 07:44:24.040450 yet_another_io_channels_library-0.2.4/channels/__init__.py
--rw-r--r--   0        0        0     3766 2024-05-26 21:18:36.103891 yet_another_io_channels_library-0.2.4/channels/channel.py
--rw-r--r--   0        0        0     2744 2024-05-26 21:51:31.970060 yet_another_io_channels_library-0.2.4/channels/poller.py
--rw-r--r--   0        0        0      432 2024-05-26 20:52:25.346757 yet_another_io_channels_library-0.2.4/channels/testing.py
--rw-r--r--   0        0        0      434 2024-05-26 21:55:59.139083 yet_another_io_channels_library-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     4735 1970-01-01 00:00:00.000000 yet_another_io_channels_library-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2018-10-14 15:23:38.622748 yet_another_io_channels_library-0.2.4.post1/LICENSE
+-rw-r--r--   0        0        0     4167 2024-06-02 19:02:38.021427 yet_another_io_channels_library-0.2.4.post1/README.md
+-rw-r--r--   0        0        0       82 2018-10-25 07:44:24.040450 yet_another_io_channels_library-0.2.4.post1/channels/__init__.py
+-rw-r--r--   0        0        0     3766 2024-05-26 21:18:36.103891 yet_another_io_channels_library-0.2.4.post1/channels/channel.py
+-rw-r--r--   0        0        0     2744 2024-05-26 21:51:31.970060 yet_another_io_channels_library-0.2.4.post1/channels/poller.py
+-rw-r--r--   0        0        0      432 2024-05-26 20:52:25.346757 yet_another_io_channels_library-0.2.4.post1/channels/testing.py
+-rw-r--r--   0        0        0      440 2024-06-02 19:04:41.601437 yet_another_io_channels_library-0.2.4.post1/pyproject.toml
+-rw-r--r--   0        0        0     4974 1970-01-01 00:00:00.000000 yet_another_io_channels_library-0.2.4.post1/PKG-INFO
```

### Comparing `yet_another_io_channels_library-0.2.4/LICENSE` & `yet_another_io_channels_library-0.2.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `yet_another_io_channels_library-0.2.4/README.md` & `yet_another_io_channels_library-0.2.4.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 
 Simple wrapper around file objects and sockets that provides uniform
 interface to both.
 
 Example:
 
 ```python
+from channels import PipeChannel, SocketChannel
+
 pipe_chan = PipeChannel(sys.stdin.fileno(), sys.stdout.fileno())
 sock_chan = SocketChannel(socket.create_connection(('127.0.0.1', 8080))
 ```
 
 ## Classes
 
 ### Channel
+
 Channel is the base class for different channels. Every channel
 implements the following methods:
 
 ```python
 read(self)
 ```
 
@@ -48,14 +51,16 @@
 but any value other than `'line'` works.
 
 The following channel classes are implemented:
 
 ### PipeChannel
 
 ```python
+from channels import PipeChannel
+
 PipeChannel(faucet=None, sink=None, *, buffering='bytes')
 ```
 
 `faucet` should be a file descriptor open for reading. `sink` should
 be a file descriptor open for writing. If both are provided, the
 channel is bi-directional. Sets `faucet` to non-blocking mode.
 
@@ -65,38 +70,47 @@
 but there is data in buffer, calls to `read` will return lines from
 buffer until it is exhausted. Last line maybe an incomplete line (no
 `'\n'` in the end).
 
 ### SocketChannel
 
 ```python
+from channels import SocketChannel
+
 SocketChannel(sock, *, buffering='bytes')
 ```
 
 Wraps a socket for non-blocking IO. See PipeChannel for more info on
 `buffering` parameter.
 
 ### TestChannel
 
-(in package channels.testing)
+(in package `channels.testing`)
 
 ```python
+from channels.testing import TestChannel
+
 TestChannel(*, buffering='bytes')
 ```
 
 See PipeChannel for more info on `buffering` parameter.
 
 Provides `put` and `get` methods to to feed data to `read` and fetch
 "written" data respectively.
 
 ### Poller
+
+(in package `channels.poller`)
+
 Poller is a wrapper for `select.poll` that also supports accepting and
 keeping track of TCP/Unix clients.
 
 ```python
+from channels.poller import Poller
+
 Poller(*, buffering='bytes')
 ```
 
 Creates a poller object. All accepted client channels inherit the
 `buffering` parameter.
 
 ```python
```

### Comparing `yet_another_io_channels_library-0.2.4/channels/channel.py` & `yet_another_io_channels_library-0.2.4.post1/channels/channel.py`

 * *Files identical despite different names*

### Comparing `yet_another_io_channels_library-0.2.4/channels/poller.py` & `yet_another_io_channels_library-0.2.4.post1/channels/poller.py`

 * *Files identical despite different names*

### Comparing `yet_another_io_channels_library-0.2.4/PKG-INFO` & `yet_another_io_channels_library-0.2.4.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yet-another-io-channels-library
-Version: 0.2.4
+Version: 0.2.4.post1
 Summary: Simple IO channels library
 License: MIT
 Author: Ilya Konovalov
 Author-email: aragaer@gmail.com
 Requires-Python: >=3.4,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,21 +23,24 @@
 
 Simple wrapper around file objects and sockets that provides uniform
 interface to both.
 
 Example:
 
 ```python
+from channels import PipeChannel, SocketChannel
+
 pipe_chan = PipeChannel(sys.stdin.fileno(), sys.stdout.fileno())
 sock_chan = SocketChannel(socket.create_connection(('127.0.0.1', 8080))
 ```
 
 ## Classes
 
 ### Channel
+
 Channel is the base class for different channels. Every channel
 implements the following methods:
 
 ```python
 read(self)
 ```
 
@@ -69,14 +72,16 @@
 but any value other than `'line'` works.
 
 The following channel classes are implemented:
 
 ### PipeChannel
 
 ```python
+from channels import PipeChannel
+
 PipeChannel(faucet=None, sink=None, *, buffering='bytes')
 ```
 
 `faucet` should be a file descriptor open for reading. `sink` should
 be a file descriptor open for writing. If both are provided, the
 channel is bi-directional. Sets `faucet` to non-blocking mode.
 
@@ -86,38 +91,47 @@
 but there is data in buffer, calls to `read` will return lines from
 buffer until it is exhausted. Last line maybe an incomplete line (no
 `'\n'` in the end).
 
 ### SocketChannel
 
 ```python
+from channels import SocketChannel
+
 SocketChannel(sock, *, buffering='bytes')
 ```
 
 Wraps a socket for non-blocking IO. See PipeChannel for more info on
 `buffering` parameter.
 
 ### TestChannel
 
-(in package channels.testing)
+(in package `channels.testing`)
 
 ```python
+from channels.testing import TestChannel
+
 TestChannel(*, buffering='bytes')
 ```
 
 See PipeChannel for more info on `buffering` parameter.
 
 Provides `put` and `get` methods to to feed data to `read` and fetch
 "written" data respectively.
 
 ### Poller
+
+(in package `channels.poller`)
+
 Poller is a wrapper for `select.poll` that also supports accepting and
 keeping track of TCP/Unix clients.
 
 ```python
+from channels.poller import Poller
+
 Poller(*, buffering='bytes')
 ```
 
 Creates a poller object. All accepted client channels inherit the
 `buffering` parameter.
 
 ```python
```

