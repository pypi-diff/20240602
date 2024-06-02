# Comparing `tmp/vpx_rtp_py-0.1.2.tar.gz` & `tmp/vpx_rtp_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpx_rtp_py-0.1.2.tar", max compression
+gzip compressed data, was "vpx_rtp_py-0.1.3.tar", max compression
```

## Comparing `vpx_rtp_py-0.1.2.tar` & `vpx_rtp_py-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/LICENSE
--rw-r--r--   0        0        0      363 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/README.md
--rw-r--r--   0        0        0     6753 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/build_cffi_bindings.py
--rw-r--r--   0        0        0     1285 2024-06-02 05:43:14.967742 vpx_rtp_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-06-02 05:43:14.971742 vpx_rtp_py-0.1.2/vpx_rtp/__init__.py
--rw-r--r--   0        0        0      824 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/clock.py
--rw-r--r--   0        0        0       42 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/codecs/_vpx.pyi
--rw-r--r--   0        0        0    13768 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/codecs/vpx.py
--rw-r--r--   0        0        0     4106 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/jitterbuffer.py
--rw-r--r--   0        0        0        0 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/py.typed
--rw-r--r--   0        0        0     2728 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/rtcrtpparameters.py
--rw-r--r--   0        0        0    12103 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/rtp.py
--rw-r--r--   0        0        0       12 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/test.py
--rw-r--r--   0        0        0      978 2024-06-02 05:42:59.019760 vpx_rtp_py-0.1.2/vpx_rtp/utils.py
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 vpx_rtp_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-06-02 06:19:58.301718 vpx_rtp_py-0.1.3/LICENSE
+-rw-r--r--   0        0        0      363 2024-06-02 06:19:58.301718 vpx_rtp_py-0.1.3/README.md
+-rw-r--r--   0        0        0     6753 2024-06-02 06:19:58.301718 vpx_rtp_py-0.1.3/build_cffi_bindings.py
+-rw-r--r--   0        0        0     1285 2024-06-02 06:20:14.649822 vpx_rtp_py-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-06-02 06:20:14.657822 vpx_rtp_py-0.1.3/vpx_rtp/__init__.py
+-rw-r--r--   0        0        0      824 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/clock.py
+-rw-r--r--   0        0        0       42 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/codecs/_vpx.pyi
+-rw-r--r--   0        0        0    13852 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/codecs/vpx.py
+-rw-r--r--   0        0        0     4293 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/jitterbuffer.py
+-rw-r--r--   0        0        0        0 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/py.typed
+-rw-r--r--   0        0        0     2749 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/rtcrtpparameters.py
+-rw-r--r--   0        0        0    12565 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/rtp.py
+-rw-r--r--   0        0        0       12 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/test.py
+-rw-r--r--   0        0        0      978 2024-06-02 06:19:58.305718 vpx_rtp_py-0.1.3/vpx_rtp/utils.py
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 vpx_rtp_py-0.1.3/PKG-INFO
```

### Comparing `vpx_rtp_py-0.1.2/LICENSE` & `vpx_rtp_py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.2/build_cffi_bindings.py` & `vpx_rtp_py-0.1.3/build_cffi_bindings.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.2/pyproject.toml` & `vpx_rtp_py-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vpx-rtp-py"
-version = "0.1.2"
+version = "0.1.3"
 description = "asyncio client library for tcp modbus devices"
 authors = ["Josh Gruenstein <josh@tutorintelligence.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "vpx_rtp" }]
 include = [ # include cffi compiled files in wheel as otherwise gitignored
     { path = "vpx_rtp", format = ["sdist", "wheel"] },
```

### Comparing `vpx_rtp_py-0.1.2/vpx_rtp/clock.py` & `vpx_rtp_py-0.1.3/vpx_rtp/clock.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.2/vpx_rtp/codecs/vpx.py` & `vpx_rtp_py-0.1.3/vpx_rtp/codecs/vpx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import fractions
 import multiprocessing
 import random
 from struct import pack, unpack_from
 from typing import List, Tuple, Type, TypeVar, cast
 
 from av import VideoFrame
-from av.frame import Frame
 from av.packet import Packet
 
 from vpx_rtp.codecs._vpx import ffi, lib
 from vpx_rtp.jitterbuffer import JitterFrame
 from vpx_rtp.rtcrtpparameters import RTCRtpCodecParameters
 
 VIDEO_CLOCK_RATE = 90000
@@ -47,20 +46,20 @@
     else:
         return 1
 
 
 class VpxPayloadDescriptor:
     def __init__(
         self,
-        partition_start,
-        partition_id,
-        picture_id=None,
-        tl0picidx=None,
-        tid=None,
-        keyidx=None,
+        partition_start: int,
+        partition_id: int,
+        picture_id: int | None = None,
+        tl0picidx: int | None = None,
+        tid: tuple[int, int] | None = None,
+        keyidx: int | None = None,
     ) -> None:
         self.partition_start = partition_start
         self.partition_id = partition_id
         self.picture_id = picture_id
         self.tl0picidx = tl0picidx
         self.tid = tid
         self.keyidx = keyidx
@@ -194,16 +193,16 @@
         ppcfg.post_proc_flag = lib.VP8_DEMACROBLOCK | lib.VP8_DEBLOCK
         ppcfg.deblocking_level = 3
         lib.vpx_codec_control_(self.codec, lib.VP8_SET_POSTPROC, ppcfg)
 
     def __del__(self) -> None:
         lib.vpx_codec_destroy(self.codec)
 
-    def decode(self, encoded_frame: JitterFrame) -> List[Frame]:
-        frames: List[Frame] = []
+    def decode(self, encoded_frame: JitterFrame) -> list[VideoFrame]:
+        frames = list[VideoFrame]()
         result = lib.vpx_codec_decode(
             self.codec,
             encoded_frame.data,
             len(encoded_frame.data),
             ffi.NULL,
             lib.VPX_DL_REALTIME,
         )
@@ -256,17 +255,16 @@
         self.__update_config_needed = False
 
     def __del__(self) -> None:
         if self.codec:
             lib.vpx_codec_destroy(self.codec)
 
     def encode(
-        self, frame: Frame, force_keyframe: bool = False
+        self, frame: VideoFrame, force_keyframe: bool = False
     ) -> Tuple[List[bytes], int]:
-        assert isinstance(frame, VideoFrame)
         if frame.format.name != "yuv420p":
             frame = frame.reformat(format="yuv420p")
 
         if self.codec and (frame.width != self.cfg.g_w or frame.height != self.cfg.g_h):
             lib.vpx_codec_destroy(self.codec)
             self.codec = None
 
@@ -367,14 +365,16 @@
         payloads = self._packetize(self.buffer[:length], self.picture_id)
         timestamp = convert_timebase(frame.pts, frame.time_base, VIDEO_TIME_BASE)
         self.picture_id = (self.picture_id + 1) % (1 << 15)
         return payloads, timestamp
 
     def pack(self, packet: Packet) -> Tuple[List[bytes], int]:
         payloads = self._packetize(bytes(packet), self.picture_id)
+
+        assert packet.pts is not None, "Packet must have a PTS"
         timestamp = convert_timebase(packet.pts, packet.time_base, VIDEO_TIME_BASE)
         self.picture_id = (self.picture_id + 1) % (1 << 15)
         return payloads, timestamp
 
     @property
     def target_bitrate(self) -> int:
         """
```

### Comparing `vpx_rtp_py-0.1.2/vpx_rtp/jitterbuffer.py` & `vpx_rtp_py-0.1.3/vpx_rtp/jitterbuffer.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     def _remove_frame(self, sequence_number: int) -> Optional[JitterFrame]:
         frame = None
         frames = 0
         packets = []
         remove = 0
         timestamp = None
 
+        assert self._origin is not None, "origin must be set"
+
         for count in range(self.capacity):
             pos = (self._origin + count) % self._capacity
             packet = self._packets[pos]
             if packet is None:
                 break
             if timestamp is None:
                 timestamp = packet.timestamp
@@ -94,25 +96,27 @@
 
             packets.append(packet)
 
         return None
 
     def remove(self, count: int) -> None:
         assert count <= self._capacity
-        for i in range(count):
+        assert self._origin is not None, "origin must be set"
+        for _ in range(count):
             pos = self._origin % self._capacity
             self._packets[pos] = None
             self._origin = uint16_add(self._origin, 1)
 
     def smart_remove(self, count: int) -> bool:
         """
         Makes sure that all packages belonging to the same frame are removed
         to prevent sending corrupted frames to the decoder.
         """
         timestamp = None
+        assert self._origin is not None, "origin must be set"
         for i in range(self._capacity):
             pos = self._origin % self._capacity
             packet = self._packets[pos]
             if packet is not None:
                 if i >= count and timestamp != packet.timestamp:
                     break
                 timestamp = packet.timestamp
```

### Comparing `vpx_rtp_py-0.1.2/vpx_rtp/rtcrtpparameters.py` & `vpx_rtp_py-0.1.3/vpx_rtp/rtcrtpparameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 @dataclass
 class RTCRtpCodecParameters:
     """
     The :class:`RTCRtpCodecParameters` dictionary provides information on
     codec settings.
     """
 
-    mimeType: str
-    "The codec MIME media type/subtype, for instance `'audio/PCMU'`."
-    clockRate: int
-    "The codec clock rate expressed in Hertz."
-    channels: Optional[int] = None
-    "The number of channels supported (e.g. two for stereo)."
-    payloadType: Optional[int] = None
-    "The value that goes in the RTP Payload Type Field."
-    rtcpFeedback: List["RTCRtcpFeedback"] = field(default_factory=list)
-    "Transport layer and codec-specific feedback messages for this codec."
-    parameters: ParametersDict = field(default_factory=dict)
-    "Codec-specific parameters available for signaling."
+    mimeType: str  # The codec MIME media type/subtype, for instance `'audio/PCMU'`.
+    clockRate: int  # The codec clock rate expressed in Hertz.
+    payloadType: int  # The value that goes in the RTP Payload Type Field.
+    channels: Optional[
+        int
+    ] = None  # The number of channels supported (e.g. two for stereo).
+    rtcpFeedback: List["RTCRtcpFeedback"] = field(
+        default_factory=list
+    )  # Transport layer and codec-specific feedback messages for this codec.
+    parameters: ParametersDict = field(
+        default_factory=dict
+    )  # Codec-specific parameters available for signaling.
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self.mimeType.split("/")[1]
 
-    def __str__(self):
+    def __str__(self) -> str:
         s = f"{self.name}/{self.clockRate}"
         if self.channels == 2:
             s += "/2"
         return s
 
 
 @dataclass
```

### Comparing `vpx_rtp_py-0.1.2/vpx_rtp/rtp.py` & `vpx_rtp_py-0.1.3/vpx_rtp/rtp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from dataclasses import dataclass
 from struct import pack, unpack, unpack_from
 from typing import Any, List, Optional, Tuple
 
+from typing_extensions import Self
+
 from vpx_rtp.rtcrtpparameters import RTCRtpParameters
 
 # used for NACK and retransmission
 RTP_HISTORY_SIZE = 128
 
 # reserved to avoid confusion with RTCP
 FORBIDDEN_PAYLOAD_TYPES = range(72, 77)
@@ -88,15 +90,15 @@
             elif x_id == self.__ids.audio_level:
                 vad_level = unpack("!B", x_value)[0]
                 values.audio_level = (vad_level & 0x80 == 0x80, vad_level & 0x7F)
             elif x_id == self.__ids.transport_sequence_number:
                 values.transport_sequence_number = unpack("!H", x_value)[0]
         return values
 
-    def set(self, values: HeaderExtensions):
+    def set(self, values: HeaderExtensions) -> tuple[int, bytes]:
         extensions = []
         if values.mid is not None and self.__ids.mid:
             extensions.append((self.__ids.mid, values.mid.encode("utf8")))
         if (
             values.repaired_rtp_stream_id is not None
             and self.__ids.repaired_rtp_stream_id
         ):
@@ -255,24 +257,37 @@
         self.sequence_number = sequence_number
         self.timestamp = timestamp
         self.ssrc = ssrc
         self.csrc: List[int] = []
         self.extensions = HeaderExtensions()
         self.payload = payload
         self.padding_size = 0
+        self._parsed_data: bytes | None = None
+
+    @property
+    def _data(self) -> bytes:
+        if self._parsed_data is None:
+            raise ValueError("RTP payload has not been parsed")
+        return self._parsed_data
+
+    @_data.setter
+    def _data(self, value: bytes) -> None:
+        self._parsed_data = value
 
     def __repr__(self) -> str:
         return (
             f"RtpPacket(seq={self.sequence_number}, ts={self.timestamp}, "
             f"marker={self.marker}, payload={self.payload_type}, "
             f"{len(self.payload)} bytes)"
         )
 
     @classmethod
-    def parse(cls, data: bytes, extensions_map=HeaderExtensionsMap()):
+    def parse(
+        cls, data: bytes, extensions_map: HeaderExtensionsMap = HeaderExtensionsMap()
+    ) -> Self:
         if len(data) < RTP_HEADER_LENGTH:
             raise ValueError(
                 f"RTP packet length is less than {RTP_HEADER_LENGTH} bytes"
             )
 
         v_p_x_cc, m_pt, sequence_number, timestamp, ssrc = unpack("!BBHLL", data[0:12])
         version = v_p_x_cc >> 6
@@ -317,15 +332,17 @@
             packet.padding_size = padding_len
             packet.payload = data[pos:-padding_len]
         else:
             packet.payload = data[pos:]
 
         return packet
 
-    def serialize(self, extensions_map=HeaderExtensionsMap()) -> bytes:
+    def serialize(
+        self, extensions_map: HeaderExtensionsMap = HeaderExtensionsMap()
+    ) -> bytes:
         extension_profile, extension_value = extensions_map.set(self.extensions)
         has_extension = bool(extension_value)
 
         padding = self.padding_size > 0
         data = pack(
             "!BBHLL",
             (self.version << 6)
```

### Comparing `vpx_rtp_py-0.1.2/vpx_rtp/utils.py` & `vpx_rtp_py-0.1.3/vpx_rtp/utils.py`

 * *Files identical despite different names*

### Comparing `vpx_rtp_py-0.1.2/PKG-INFO` & `vpx_rtp_py-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpx-rtp-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: asyncio client library for tcp modbus devices
 License: MIT
 Author: Josh Gruenstein
 Author-email: josh@tutorintelligence.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

