# Comparing `tmp/vpx_rtp_py-0.1.3.tar.gz` & `tmp/vpx_rtp_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpx_rtp_py-0.1.3.tar", max compression
+gzip compressed data, was "vpx_rtp_py-0.2.0.tar", max compression
```

## Comparing `vpx_rtp_py-0.1.3.tar` & `vpx_rtp_py-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2024-06-02 06:19:58.301718 vpx_rtp_py-0.1.3/LICENSE
--rw-r--r--   0        0        0      363 2024-06-02 06:19:58.301718 vpx_rtp_py-0.1.3/README.md
--rw-r--r--   0        0        0     6753 2024-06-02 06:19:58.301718 vpx_rtp_py-0.1.3/build_cffi_bindings.py
--rw-r--r--   0        0        0     1285 2024-06-02 06:20:14.649822 vpx_rtp_py-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       22 2024-06-02 06:20:14.657822 vpx_rtp_py-0.1.3/vpx_rtp/__init__.py
--rw-r--r--   0        0        0      824 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/clock.py
--rw-r--r--   0        0        0       42 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/codecs/_vpx.pyi
--rw-r--r--   0        0        0    13852 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/codecs/vpx.py
--rw-r--r--   0        0        0     4293 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/jitterbuffer.py
--rw-r--r--   0        0        0        0 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/py.typed
--rw-r--r--   0        0        0     2749 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/rtcrtpparameters.py
--rw-r--r--   0        0        0    12565 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/rtp.py
--rw-r--r--   0        0        0       12 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/test.py
--rw-r--r--   0        0        0      978 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/utils.py
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 vpx_rtp_py-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/LICENSE
+-rw-r--r--   0        0        0      363 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/README.md
+-rw-r--r--   0        0        0     6753 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/build_cffi_bindings.py
+-rw-r--r--   0        0        0     1285 2024-06-02 08:08:44.625110 vpx_rtp_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-06-02 08:08:44.633110 vpx_rtp_py-0.2.0/vpx_rtp/__init__.py
+-rw-r--r--   0        0        0      824 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/vpx_rtp/clock.py
+-rw-r--r--   0        0        0       42 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/vpx_rtp/codecs/_vpx.pyi
+-rw-r--r--   0        0        0    14592 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/vpx_rtp/codecs/vpx.py
+-rw-r--r--   0        0        0     4293 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/vpx_rtp/jitterbuffer.py
+-rw-r--r--   0        0        0        0 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/vpx_rtp/py.typed
+-rw-r--r--   0        0        0     2749 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/vpx_rtp/rtcrtpparameters.py
+-rw-r--r--   0        0        0    12565 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/vpx_rtp/rtp.py
+-rw-r--r--   0        0        0       12 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/vpx_rtp/test.py
+-rw-r--r--   0        0        0      978 2024-06-02 08:08:28.128936 vpx_rtp_py-0.2.0/vpx_rtp/utils.py
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 vpx_rtp_py-0.2.0/PKG-INFO
```

### Comparing `vpx_rtp_py-0.1.3/LICENSE` & `vpx_rtp_py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.3/build_cffi_bindings.py` & `vpx_rtp_py-0.2.0/build_cffi_bindings.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.3/pyproject.toml` & `vpx_rtp_py-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vpx-rtp-py"
-version = "0.1.3"
+version = "0.2.0"
 description = "asyncio client library for tcp modbus devices"
 authors = ["Josh Gruenstein <josh@tutorintelligence.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "vpx_rtp" }]
 include = [ # include cffi compiled files in wheel as otherwise gitignored
     { path = "vpx_rtp", format = ["sdist", "wheel"] },
```

### Comparing `vpx_rtp_py-0.1.3/vpx_rtp/clock.py` & `vpx_rtp_py-0.2.0/vpx_rtp/clock.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.3/vpx_rtp/codecs/vpx.py` & `vpx_rtp_py-0.2.0/vpx_rtp/codecs/vpx.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import fractions
 import multiprocessing
 import random
+from enum import Enum
 from struct import pack, unpack_from
 from typing import List, Tuple, Type, TypeVar, cast
 
 from av import VideoFrame
 from av.packet import Packet
 
 from vpx_rtp.codecs._vpx import ffi, lib
@@ -23,14 +24,20 @@
 
 DESCRIPTOR_T = TypeVar("DESCRIPTOR_T", bound="VpxPayloadDescriptor")
 
 VP8_CODEC = RTCRtpCodecParameters(
     mimeType="video/VP8", clockRate=VIDEO_CLOCK_RATE, payloadType=100
 )
 
+VP9_CODEC = RTCRtpCodecParameters(
+    mimeType="video/VP9",
+    clockRate=VP8_CODEC.clockRate,
+    payloadType=VP8_CODEC.payloadType,
+)
+
 
 def convert_timebase(
     pts: int, from_base: fractions.Fraction, to_base: fractions.Fraction
 ) -> int:
     if from_base != to_base:
         pts = int(pts * from_base / to_base)
     return pts
@@ -178,20 +185,30 @@
 
 def _vpx_assert(err: int) -> None:
     if err != lib.VPX_CODEC_OK:
         reason = ffi.string(lib.vpx_codec_err_to_string(err))
         raise Exception("libvpx error: " + reason.decode("utf8"))
 
 
+class VpxCodec(Enum):
+    VP8 = VP8_CODEC
+    VP9 = VP9_CODEC
+
+
 class Vp8Decoder:
-    def __init__(self) -> None:
+    def __init__(self, codec: VpxCodec = VpxCodec.VP9) -> None:
         self.codec = ffi.new("vpx_codec_ctx_t *")
-        _vpx_assert(
-            lib.vpx_codec_dec_init(self.codec, lib.vpx_codec_vp8_dx(), ffi.NULL, 0)
-        )
+
+        match codec:
+            case VpxCodec.VP8:
+                dx = lib.vpx_codec_vp8_dx()
+            case VpxCodec.VP9:
+                dx = lib.vpx_codec_vp9_dx()
+
+        _vpx_assert(lib.vpx_codec_dec_init(self.codec, dx, ffi.NULL, 0))
 
         ppcfg = ffi.new("vp8_postproc_cfg_t *")
         ppcfg.post_proc_flag = lib.VP8_DEMACROBLOCK | lib.VP8_DEBLOCK
         ppcfg.deblocking_level = 3
         lib.vpx_codec_control_(self.codec, lib.VP8_SET_POSTPROC, ppcfg)
 
     def __del__(self) -> None:
@@ -237,25 +254,34 @@
 
                 frames.append(frame)
 
         return frames
 
 
 class Vp8Encoder:
-    def __init__(self) -> None:
-        self.cx = lib.vpx_codec_vp8_cx()
+    def __init__(
+        self, codec: VpxCodec = VpxCodec.VP9, target_bitrate: int = DEFAULT_BITRATE
+    ) -> None:
+        if target_bitrate < MIN_BITRATE or target_bitrate > MAX_BITRATE:
+            raise ValueError("Invalid target bitrate")
+
+        match codec:
+            case VpxCodec.VP8:
+                self.cx = lib.vpx_codec_vp8_cx()
+            case VpxCodec.VP9:
+                self.cx = lib.vpx_codec_vp9_cx()
 
         self.cfg = ffi.new("vpx_codec_enc_cfg_t *")
         lib.vpx_codec_enc_config_default(self.cx, self.cfg, 0)
 
         self.buffer = bytearray(8000)
         self.codec = None
         self.picture_id = random.randint(0, (1 << 15) - 1)
         self.timestamp_increment = VIDEO_CLOCK_RATE // MAX_FRAME_RATE
-        self.__target_bitrate = DEFAULT_BITRATE
+        self.__target_bitrate = target_bitrate
         self.__update_config_needed = False
 
     def __del__(self) -> None:
         if self.codec:
             lib.vpx_codec_destroy(self.codec)
 
     def encode(
```

### Comparing `vpx_rtp_py-0.1.3/vpx_rtp/jitterbuffer.py` & `vpx_rtp_py-0.2.0/vpx_rtp/jitterbuffer.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.3/vpx_rtp/rtcrtpparameters.py` & `vpx_rtp_py-0.2.0/vpx_rtp/rtcrtpparameters.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.3/vpx_rtp/rtp.py` & `vpx_rtp_py-0.2.0/vpx_rtp/rtp.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.3/vpx_rtp/utils.py` & `vpx_rtp_py-0.2.0/vpx_rtp/utils.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.3/PKG-INFO` & `vpx_rtp_py-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpx-rtp-py
-Version: 0.1.3
+Version: 0.2.0
 Summary: asyncio client library for tcp modbus devices
 License: MIT
 Author: Josh Gruenstein
 Author-email: josh@tutorintelligence.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

