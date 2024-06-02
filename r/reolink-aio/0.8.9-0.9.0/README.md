# Comparing `tmp/reolink_aio-0.8.9.tar.gz` & `tmp/reolink_aio-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reolink_aio-0.8.9.tar", last modified: Sun Mar  3 16:52:03 2024, max compression
+gzip compressed data, was "reolink_aio-0.9.0.tar", last modified: Sun Jun  2 18:50:32 2024, max compression
```

## Comparing `reolink_aio-0.8.9.tar` & `reolink_aio-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/reolink_aio/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   229509 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/software_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15466 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/reolink_aio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/reolink_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-03 16:52:03.000000 reolink_aio-0.8.9/reolink_aio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:52:03.326796 reolink_aio-0.8.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    15443 2024-03-03 16:51:59.000000 reolink_aio-0.8.9/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:50:32.826558 reolink_aio-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-06-02 18:50:32.826558 reolink_aio-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:50:32.822558 reolink_aio-0.9.0/reolink_aio/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/reolink_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243797 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/reolink_aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/reolink_aio/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/reolink_aio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/reolink_aio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/reolink_aio/software_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/reolink_aio/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15466 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/reolink_aio/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/reolink_aio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:50:32.826558 reolink_aio-0.9.0/reolink_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-06-02 18:50:32.000000 reolink_aio-0.9.0/reolink_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-06-02 18:50:32.000000 reolink_aio-0.9.0/reolink_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:50:32.000000 reolink_aio-0.9.0/reolink_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:50:32.000000 reolink_aio-0.9.0/reolink_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 18:50:32.000000 reolink_aio-0.9.0/reolink_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-02 18:50:32.000000 reolink_aio-0.9.0/reolink_aio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:50:32.826558 reolink_aio-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:50:32.826558 reolink_aio-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15443 2024-06-02 18:50:25.000000 reolink_aio-0.9.0/tests/test.py
```

### Comparing `reolink_aio-0.8.9/LICENSE` & `reolink_aio-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.9/PKG-INFO` & `reolink_aio-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink_aio
-Version: 0.8.9
+Version: 0.9.0
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink_aio Version: 0.8.9 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink_aio Version: 0.9.0 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.8.9/README.md` & `reolink_aio-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.9/reolink_aio/api.py` & `reolink_aio-0.9.0/reolink_aio/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from orjson import JSONDecodeError, loads as json_loads  # pylint: disable=no-name-in-module
 from aiortsp.rtsp.connection import RTSPConnection  # type: ignore
 from aiortsp.rtsp.errors import RTSPError  # type: ignore
 import aiohttp
 
 from . import templates, typings
-from .enums import DayNightEnum, StatusLedEnum, SpotlightModeEnum, PtzEnum, GuardEnum, TrackMethodEnum, SubType, VodRequestType
+from .enums import BatteryEnum, DayNightEnum, StatusLedEnum, SpotlightModeEnum, PtzEnum, GuardEnum, TrackMethodEnum, SubType, VodRequestType
 from .exceptions import (
     ApiError,
     CredentialsInvalidError,
     InvalidContentTypeError,
     InvalidParameterError,
     LoginError,
     NoDataError,
@@ -76,14 +76,27 @@
 DUAL_LENS_SINGLE_MOTION_MODELS: set[str] = {
     "Reolink TrackMix PoE",
     "Reolink TrackMix WiFi",
     "RLC-81MA",
 }
 DUAL_LENS_MODELS: set[str] = DUAL_LENS_DUAL_MOTION_MODELS | DUAL_LENS_SINGLE_MOTION_MODELS
 
+WAKING_COMMANDS = [
+    "GetWhiteLed",
+    "GetZoomFocus",
+    "GetAudioCfg",
+    "GetPtzGuard",
+    "GetAutoReply",
+    "GetPtzTraceSection",
+    "GetAiCfg",
+    "GetAiAlarm",
+    "GetPtzCurPos",
+    "GetAudioAlarm",
+]
+
 
 ##########################################################################################################################################################
 # API class
 ##########################################################################################################################################################
 class Host:
     """Reolink network API class."""
 
@@ -151,14 +164,15 @@
         ##############################################################################
         # Channels of cameras, used in this NVR ([0] for a directly connected camera)
         self._GetChannelStatus_present: bool = False
         self._GetChannelStatus_has_name: bool = False
         self._channels: list[int] = []
         self._stream_channels: list[int] = []
         self._channel_names: dict[int, str] = {}
+        self._channel_uids: dict[int, str] = {}
         self._channel_models: dict[int, str] = {}
         self._channel_sw_versions: dict[int, str] = {}
         self._channel_sw_version_objects: dict[int, SoftwareVersion] = {}
         self._is_doorbell: dict[int, bool] = {}
 
         ##############################################################################
         # API-versions and capabilities
@@ -190,14 +204,15 @@
         ##############################################################################
         # Saved settings response-blocks
         # Host-level
         self._time_settings: Optional[dict] = None
         self._host_time_difference: float = 0
         self._ntp_settings: Optional[dict] = None
         self._netport_settings: Optional[dict] = None
+        self._push_config: dict = {}
         # Camera-level
         self._zoom_focus_settings: dict[int, dict] = {}
         self._zoom_focus_range: dict[int, dict] = {}
         self._auto_focus_settings: dict[int, dict] = {}
         self._isp_settings: dict[int, dict] = {}
         self._image_settings: dict[int, dict] = {}
         self._ftp_settings: dict[int, dict] = {}
@@ -209,15 +224,19 @@
         self._ptz_patrol_settings: dict[int, dict] = {}
         self._ptz_guard_settings: dict[int, dict] = {}
         self._ptz_position: dict[int, dict] = {}
         self._email_settings: dict[int, dict] = {}
         self._ir_settings: dict[int, dict] = {}
         self._status_led_settings: dict[int, dict] = {}
         self._whiteled_settings: dict[int, dict] = {}
+        self._sleep: dict[int, bool] = {}
+        self._battery: dict[int, dict] = {}
+        self._pir: dict[int, dict] = {}
         self._recording_settings: dict[int, dict] = {}
+        self._manual_record_settings: dict[int, dict] = {}
         self._md_alarm_settings: dict[int, dict] = {}
         self._ai_alarm_settings: dict[int, dict] = {}
         self._audio_settings: dict[int, dict] = {}
         self._audio_alarm_settings: dict[int, dict] = {}
         self._buzzer_settings: dict[int, dict] = {}
         self._auto_track_settings: dict[int, dict] = {}
         self._auto_track_range: dict[int, dict] = {}
@@ -504,32 +523,52 @@
 
     def _hide_password(self, content: str | bytes | dict | list) -> str:
         redacted = str(content)
         if self._password:
             redacted = redacted.replace(self._password, "<password>")
         if self._token:
             redacted = redacted.replace(self._token, "<token>")
+        if self._nvr_uid:
+            redacted = redacted.replace(self._nvr_uid, "<uid>")
         return redacted
 
     ##############################################################################
     # Channel-level getters/setters
 
-    def camera_name(self, channel: int | None) -> Optional[str]:
+    def camera_name(self, channel: int | None) -> str:
         if channel is None:
             return self.nvr_name
 
         if channel not in self._channel_names and channel in self._stream_channels and channel != 0:
             return self.camera_name(0)  # Dual lens cameras
         if channel not in self._channel_names:
             if len(self._channels) == 1:
                 return self.nvr_name
             return "Unknown"
         return self._channel_names[channel]
 
-    def camera_model(self, channel: int) -> Optional[str]:
+    def camera_uid(self, channel: int | None) -> str:
+        if channel is None:
+            return self.uid
+        if channel not in self._channel_uids and channel in self._stream_channels and channel != 0:
+            return f"{self.camera_uid(0)}_{channel}"  # Dual lens cameras
+        if channel not in self._channel_uids:
+            return "Unknown"
+        return self._channel_uids[channel]
+
+    def channel_for_uid(self, uid: str) -> int:
+        """Returns the channel belonging to a UID"""
+        channel = -1
+        for ch, ch_uid in self._channel_uids.items():
+            if ch_uid.startswith(uid):
+                channel = ch
+                break
+        return channel
+
+    def camera_model(self, channel: int) -> str:
         if channel not in self._channel_models and channel in self._stream_channels and channel != 0:
             return self.camera_model(0)  # Dual lens cameras
         if channel not in self._channel_models:
             return "Unknown"
         return self._channel_models[channel]
 
     def camera_sw_version(self, channel: int) -> str:
@@ -589,15 +628,15 @@
     def ai_supported_types(self, channel: int) -> list[str]:
         """Return a list of supported AI types."""
         if channel not in self._ai_detection_support:
             return []
 
         ai_types = []
         for key, value in self._ai_detection_support[channel].items():
-            if value:
+            if value and key != "other":
                 ai_types.append(key)
 
         return ai_types
 
     def audio_alarm_enabled(self, channel: int) -> bool:
         if channel not in self._audio_alarm_settings:
             return False
@@ -610,25 +649,32 @@
     def ir_enabled(self, channel: int) -> bool:
         return channel in self._ir_settings and self._ir_settings[channel]["IrLights"]["state"] == "Auto"
 
     def status_led_enabled(self, channel: int) -> bool:
         if channel not in self._status_led_settings:
             return False
 
-        if self.is_doorbell(channel):
-            return self._status_led_settings[channel]["PowerLed"].get("eDoorbellLightState", "Off") == "On"
-
         return self._status_led_settings[channel]["PowerLed"].get("state", "Off") == "On"
 
     def doorbell_led(self, channel: int) -> str:
         if channel not in self._status_led_settings:
             return "Off"
 
         return self._status_led_settings[channel]["PowerLed"].get("eDoorbellLightState", "Off")
 
+    def doorbell_led_list(self, channel: int) -> list[str]:
+        mode_values = []
+        if self.api_version("supportDoorbellLightKeepOff", channel) > 0:
+            mode_values.append(StatusLedEnum.stayoff)
+        mode_values.extend([StatusLedEnum.auto, StatusLedEnum.alwaysonatnight])
+        if self.api_version("supportDoorbellLightKeepOn", channel) > 0:
+            mode_values.append(StatusLedEnum.alwayson)
+
+        return [val.name for val in mode_values]
+
     def ftp_enabled(self, channel: int | None = None) -> bool:
         if channel is None:
             if self.api_version("GetFtp") >= 1:
                 return all(self._ftp_settings[ch]["Ftp"]["enable"] == 1 for ch in self._channels if ch in self._ftp_settings)
 
             return all(self._ftp_settings[ch]["Ftp"]["schedule"]["enable"] == 1 for ch in self._channels if ch in self._ftp_settings)
 
@@ -653,14 +699,17 @@
         if self.api_version("GetEmail") >= 1:
             return self._email_settings[channel]["Email"]["scheduleEnable"] == 1
 
         return self._email_settings[channel]["Email"]["schedule"]["enable"] == 1
 
     def push_enabled(self, channel: int | None = None) -> bool:
         if channel is None:
+            if self.supported(None, "push_config"):
+                return self._push_config["PushCfg"]["enable"] == 1
+
             if self.api_version("GetPush") >= 1:
                 return all(self._push_settings[ch]["Push"]["enable"] == 1 for ch in self._channels if ch in self._push_settings)
 
             return all(self._push_settings[ch]["Push"]["schedule"]["enable"] == 1 for ch in self._channels if ch in self._push_settings)
 
         if channel not in self._push_settings:
             return False
@@ -681,14 +730,20 @@
             return False
 
         if self.api_version("GetRec") >= 1:
             return self._recording_settings[channel]["Rec"]["scheduleEnable"] == 1
 
         return self._recording_settings[channel]["Rec"]["schedule"]["enable"] == 1
 
+    def manual_record_enabled(self, channel: int) -> bool:
+        if channel not in self._manual_record_settings:
+            return False
+
+        return self._manual_record_settings[channel]["Rec"]["enable"] == 1
+
     def buzzer_enabled(self, channel: int | None = None) -> bool:
         if channel is None:
             return all(self._buzzer_settings[ch]["Buzzer"]["enable"] == 1 for ch in self._channels if ch in self._buzzer_settings)
 
         if channel not in self._buzzer_settings:
             return False
 
@@ -728,14 +783,38 @@
     def whiteled_settings(self, channel: int) -> Optional[dict]:
         """Return the spotlight state."""
         if channel in self._whiteled_settings:
             return self._whiteled_settings[channel]
 
         return None
 
+    def battery_percentage(self, channel: int) -> Optional[int]:
+        if channel not in self._battery:
+            return None
+
+        return self._battery[channel]["batteryPercent"]
+
+    def battery_temperature(self, channel: int) -> Optional[int]:
+        if channel not in self._battery:
+            return None
+
+        return self._battery[channel]["temperature"]
+
+    def battery_status(self, channel: int) -> int:
+        if channel not in self._battery:
+            return BatteryEnum.discharging.value
+
+        return self._battery[channel]["chargeStatus"]
+
+    def sleeping(self, channel: int) -> bool:
+        if channel not in self._sleep:
+            return False
+
+        return self._sleep[channel]
+
     def daynight_state(self, channel: int) -> Optional[str]:
         if channel not in self._isp_settings:
             return None
 
         return self._isp_settings[channel]["Isp"]["dayNight"]
 
     def HDR_on(self, channel: int) -> bool | None:
@@ -806,15 +885,15 @@
         if channel not in self._audio_settings:
             return False
 
         return self._audio_settings[channel]["AudioCfg"].get("visitorLoudspeaker") == 1
 
     def quick_reply_dict(self, channel: int) -> dict[int, str]:
         if channel not in self._audio_file_list:
-            return {}
+            return {-1: "off"}
 
         audio_dict = {-1: "off"}
         for audio_file in self._audio_file_list[channel]["AudioFileList"]:
             audio_dict[audio_file["id"]] = audio_file["fileName"]
         return audio_dict
 
     def quick_reply_enabled(self, channel: int) -> bool:
@@ -838,14 +917,32 @@
 
     def audio_alarm_settings(self, channel: int) -> dict:
         if channel in self._audio_alarm_settings:
             return self._audio_alarm_settings[channel]
 
         return {}
 
+    def pir_enabled(self, channel: int) -> bool | None:
+        if channel not in self._pir:
+            return None
+
+        return self._pir[channel]["enable"] > 0
+
+    def pir_reduce_alarm(self, channel: int) -> bool | None:
+        if channel not in self._pir:
+            return None
+
+        return self._pir[channel]["reduceAlarm"] > 0
+
+    def pir_sensitivity(self, channel: int) -> int:
+        if channel not in self._pir:
+            return 0
+
+        return 101 - self._pir[channel]["sensitive"]
+
     def md_sensitivity(self, channel: int) -> int:
         if channel not in self._md_alarm_settings:
             return 0
 
         if self.api_version("GetMdAlarm") >= 1:
             if self._md_alarm_settings[channel]["MdAlarm"].get("useNewSens", 0) == 1:
                 return 51 - self._md_alarm_settings[channel]["MdAlarm"]["newSens"]["sensDef"]
@@ -1054,14 +1151,17 @@
 
         if self._ftp_settings:
             self._capabilities["Host"].append("ftp")
 
         if self._push_settings:
             self._capabilities["Host"].append("push")
 
+        if self._push_config.get("PushCfg", {}).get("enable") is not None:
+            self._capabilities["Host"].append("push_config")
+
         if self._recording_settings:
             self._capabilities["Host"].append("recording")
 
         if self._email_settings:
             self._capabilities["Host"].append("email")
 
         if self.api_version("supportBuzzer") > 0:
@@ -1079,14 +1179,17 @@
         if self.api_version("reboot") > 0:
             self._capabilities["Host"].append("reboot")
 
         # Channel capabilities
         for channel in self._channels:
             self._capabilities[channel] = []
 
+            if self.camera_uid(channel) != "Unknown":
+                self._capabilities[channel].append("UID")
+
             if self.is_nvr and self.api_version("supportAutoTrackStream", channel) > 0:
                 self._capabilities[channel].append("autotrack_stream")
 
             if channel in self._motion_detection_states:
                 self._capabilities[channel].append("motion_detection")
 
             if self.api_version("supportAiAnimal", channel) and self.ai_supported(channel, PET_DETECTION_TYPE):
@@ -1103,24 +1206,27 @@
 
             if channel in self._push_settings and (self.api_version("GetPush") < 1 or "scheduleEnable" in self._push_settings[channel]["Push"]):
                 self._capabilities[channel].append("push")
 
             if channel in self._recording_settings and (self.api_version("GetRec") < 1 or "scheduleEnable" in self._recording_settings[channel]["Rec"]):
                 self._capabilities[channel].append("recording")
 
+            if channel in self._manual_record_settings and "enable" in self._recording_settings[channel]["Rec"]:
+                self._capabilities[channel].append("manual_record")
+
             if channel in self._email_settings and (self.api_version("GetEmail") < 1 or "scheduleEnable" in self._email_settings[channel]["Email"]):
                 self._capabilities[channel].append("email")
 
             if channel in self._buzzer_settings and self.api_version("supportBuzzer") > 0 and "scheduleEnable" in self._buzzer_settings[channel]["Buzzer"]:
                 self._capabilities[channel].append("buzzer")
 
             if self.api_version("ledControl", channel) > 0 and channel in self._ir_settings:
                 self._capabilities[channel].append("ir_lights")
 
-            if self.api_version("powerLed", channel) > 0:
+            if self.api_version("powerLed", channel) > 0 or self.api_version("indicatorLight", channel) > 0:
                 # powerLed == statusLed = doorbell_led
                 self._capabilities[channel].append("status_led")  # internal use only
                 self._capabilities[channel].append("power_led")
             if self.api_version("supportDoorbellLight", channel) > 0 or self.is_doorbell(channel):
                 # powerLed == statusLed = doorbell_led
                 self._capabilities[channel].append("status_led")  # internal use only
                 self._capabilities[channel].append("doorbell_led")
@@ -1138,15 +1244,15 @@
 
             if (self.api_version("supportAudioFileList", channel) > 0) or (not self.is_nvr and self.api_version("supportAudioFileList") > 0):
                 if self.api_version("supportAutoReply", channel) > 0 or (not self.is_nvr and self.api_version("supportAutoReply") > 0):
                     self._capabilities[channel].append("quick_reply")
                 if self.api_version("supportAudioPlay", channel) > 0:
                     self._capabilities[channel].append("play_quick_reply")
 
-            if self.api_version("alarmAudio", channel) > 0 and channel in self._audio_alarm_settings:
+            if (self.api_version("alarmAudio", channel) > 0 or self.api_version("supportAudioAlarm", channel) > 0) and channel in self._audio_alarm_settings:
                 self._capabilities[channel].append("siren")
                 self._capabilities[channel].append("siren_play")  # if self.api_version("supportAoAdjust", channel) > 0
 
             if self.audio_record(channel) is not None:
                 self._capabilities[channel].append("audio")
 
             ptz_ver = self.api_version("ptzType", channel)
@@ -1202,15 +1308,24 @@
                     self._capabilities[channel].append("auto_track_disappear_time")
                 if self.auto_track_stop_time(channel) > 0:
                     self._capabilities[channel].append("auto_track_stop_time")
 
             if self.api_version("supportAITrackLimit", channel) > 0:
                 self._capabilities[channel].append("auto_track_limit")
 
-            if channel in self._md_alarm_settings:
+            if self.api_version("battery", channel) > 0:
+                self._capabilities[channel].append("battery")
+                if channel in self._sleep:
+                    self._capabilities[channel].append("sleep")
+                    if "sleep" not in self._capabilities["Host"]:
+                        self._capabilities["Host"].append("sleep")
+            if self.api_version("mdWithPir", channel) > 0:
+                self._capabilities[channel].append("PIR")
+
+            if channel in self._md_alarm_settings and not self.supported(channel, "PIR"):
                 self._capabilities[channel].append("md_sensitivity")
 
             if self.api_version("supportAiSensitivity", channel) > 0:
                 self._capabilities[channel].append("ai_sensitivity")
 
             if self.api_version("supportAiStayTime", channel) > 0:
                 self._capabilities[channel].append("ai_delay")
@@ -1277,90 +1392,102 @@
                 ch_body = [{"cmd": "GetIsp", "action": 0, "param": {"channel": channel}}]
 
             if channel > 0 and self.model in DUAL_LENS_DUAL_MOTION_MODELS:
                 body.extend(ch_body)
                 channels.extend([channel] * len(ch_body))
                 continue
 
-            if cmd == "GetIrLights":
+            if cmd == "GetIrLights" and self.supported(channel, "ir_lights"):
                 ch_body = [{"cmd": "GetIrLights", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetPowerLed":
+            elif cmd == "GetPowerLed" and self.supported(channel, "status_led"):
                 ch_body = [{"cmd": "GetPowerLed", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetWhiteLed":
+            elif cmd == "GetWhiteLed" and self.supported(channel, "floodLight"):
                 ch_body = [{"cmd": "GetWhiteLed", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetWebHook":
+            elif cmd == "GetBatteryInfo" and self.supported(channel, "battery"):
+                ch_body = [{"cmd": "GetBatteryInfo", "action": 0, "param": {"channel": channel}}]
+            elif cmd == "GetPirInfo" and self.supported(channel, "PIR"):
+                ch_body = [{"cmd": "GetPirInfo", "action": 0, "param": {"channel": channel}}]
+            elif cmd == "GetWebHook" and self.supported(channel, "webhook"):
                 ch_body = [{"cmd": "GetWebHook", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetPtzPreset":
+            elif cmd == "GetPtzPreset" and self.supported(channel, "ptz_presets"):
                 ch_body = [{"cmd": "GetPtzPreset", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetPtzPatrol":
+            elif cmd == "GetPtzPatrol" and self.supported(channel, "ptz_patrol"):
                 ch_body = [{"cmd": "GetPtzPatrol", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetAutoFocus":
+            elif cmd == "GetAutoFocus" and self.supported(channel, "auto_focus"):
                 ch_body = [{"cmd": "GetAutoFocus", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetZoomFocus":
+            elif cmd == "GetZoomFocus" and self.supported(channel, "zoom"):
                 ch_body = [{"cmd": "GetZoomFocus", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetPtzGuard":
+            elif cmd == "GetPtzGuard" and self.supported(channel, "ptz_guard"):
                 ch_body = [{"cmd": "GetPtzGuard", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetPtzCurPos":
+            elif cmd == "GetPtzCurPos" and self.supported(channel, "ptz_position"):
                 ch_body = [{"cmd": "GetPtzCurPos", "action": 0, "param": {"PtzCurPos": {"channel": channel}}}]
-            elif cmd == "GetAiCfg":
+            elif cmd == "GetAiCfg" and self.supported(channel, "auto_track"):
                 ch_body = [{"cmd": "GetAiCfg", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetPtzTraceSection":
+            elif cmd == "GetPtzTraceSection" and self.supported(channel, "auto_track_limit"):
                 ch_body = [{"cmd": "GetPtzTraceSection", "action": 0, "param": {"PtzTraceSection": {"channel": channel}}}]
-            elif cmd == "GetAudioCfg":
+            elif cmd == "GetAudioCfg" and self.supported(channel, "volume"):
                 ch_body = [{"cmd": "GetAudioCfg", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetAudioFileList":
+            elif cmd == "GetAudioFileList" and self.supported(channel, "quick_reply"):
                 ch_body = [{"cmd": "GetAudioFileList", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetAutoReply":
+            elif cmd == "GetAutoReply" and self.supported(channel, "quick_reply"):
                 ch_body = [{"cmd": "GetAutoReply", "action": 0, "param": {"channel": channel}}]
+            elif cmd == "GetManualRec" and self.supported(channel, "manual_record"):
+                ch_body.append({"cmd": "GetManualRec", "action": 0, "param": {"channel": channel}})
             elif cmd == "GetOsd":
                 ch_body = [{"cmd": "GetOsd", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetImage":
+            elif cmd == "GetImage" and (
+                self.supported(channel, "isp_hue")
+                or self.supported(channel, "isp_satruation")
+                or self.supported(channel, "isp_sharpen")
+                or self.supported(channel, "isp_contrast")
+                or self.supported(channel, "isp_bright")
+            ):
                 ch_body = [{"cmd": "GetImage", "action": 0, "param": {"channel": channel}}]
-            elif cmd == "GetBuzzerAlarmV20":
+            elif cmd == "GetBuzzerAlarmV20" and (self.supported(channel, "buzzer") or (self.supported(None, "buzzer") and channel == 0)):
                 ch_body = [{"cmd": "GetBuzzerAlarmV20", "action": 0, "param": {"channel": channel}}]
-            elif cmd in ["GetAlarm", "GetMdAlarm"]:
+            elif cmd in ["GetAlarm", "GetMdAlarm"] and self.supported(channel, "md_sensitivity"):
                 if self.api_version("GetMdAlarm") >= 1:
                     ch_body = [{"cmd": "GetMdAlarm", "action": 0, "param": {"channel": channel}}]
                 else:
                     ch_body = [{"cmd": "GetAlarm", "action": 0, "param": {"Alarm": {"channel": channel, "type": "md"}}}]
-            elif cmd == "GetAiAlarm":
+            elif cmd == "GetAiAlarm" and self.supported(channel, "ai_sensitivity"):
                 ch_body = []
                 for ai_type in self.ai_supported_types(channel):
                     ch_body.append({"cmd": "GetAiAlarm", "action": 0, "param": {"channel": channel, "ai_type": ai_type}})
-            elif cmd in ["GetEmail", "GetEmailV20"]:
+            elif cmd in ["GetEmail", "GetEmailV20"] and (self.supported(channel, "email") or (self.supported(None, "email") and channel == 0)):
                 if self.api_version("GetEmail") >= 1:
                     ch_body = [{"cmd": "GetEmailV20", "action": 0, "param": {"channel": channel}}]
                 else:
                     ch_body = [{"cmd": "GetEmail", "action": 0, "param": {"channel": channel}}]
-            elif cmd in ["GetPush", "GetPushV20"]:
+            elif cmd in ["GetPush", "GetPushV20"] and (self.supported(channel, "push") or (self.supported(None, "push") and channel == 0)):
                 if self.api_version("GetPush") >= 1:
                     ch_body = [{"cmd": "GetPushV20", "action": 0, "param": {"channel": channel}}]
                 else:
                     ch_body = [{"cmd": "GetPush", "action": 0, "param": {"channel": channel}}]
-            elif cmd in ["GetFtp", "GetFtpV20"]:
+            elif cmd in ["GetFtp", "GetFtpV20"] and (self.supported(channel, "ftp") or (self.supported(None, "ftp") and channel == 0)):
                 if self.api_version("GetFtp") >= 1:
                     ch_body = [{"cmd": "GetFtpV20", "action": 0, "param": {"channel": channel}}]
                 else:
                     ch_body = [{"cmd": "GetFtp", "action": 0, "param": {"channel": channel}}]
-            elif cmd in ["GetRec", "GetRecV20"]:
+            elif cmd in ["GetRec", "GetRecV20"] and (self.supported(channel, "recording") or (self.supported(None, "recording") and channel == 0)):
                 if self.api_version("GetRec") >= 1:
                     ch_body = [{"cmd": "GetRecV20", "action": 0, "param": {"channel": channel}}]
                 else:
                     ch_body = [{"cmd": "GetRec", "action": 0, "param": {"channel": channel}}]
-            elif cmd in ["GetAudioAlarm", "GetAudioAlarmV20"]:
+            elif cmd in ["GetAudioAlarm", "GetAudioAlarmV20"] and self.supported(channel, "siren"):
                 if self.api_version("GetAudioAlarm") >= 1:
                     ch_body = [{"cmd": "GetAudioAlarmV20", "action": 0, "param": {"channel": channel}}]
                 else:
                     ch_body = [{"cmd": "GetAudioAlarm", "action": 0, "param": {"channel": channel}}]
             body.extend(ch_body)
             channels.extend([channel] * len(ch_body))
 
         if not channels:
-            if cmd == "Getchannelstatus":
-                body = [{"cmd": "Getchannelstatus"}]
+            if cmd == "GetChannelstatus":
+                body = [{"cmd": "GetChannelstatus"}]
             elif cmd == "GetDevInfo":
                 body = [{"cmd": "GetDevInfo", "action": 0, "param": {}}]
             elif cmd == "GetLocalLink":
                 body = [{"cmd": "GetLocalLink", "action": 0, "param": {}}]
             elif cmd == "GetWifiSignal":
                 body = [{"cmd": "GetWifiSignal", "action": 0, "param": {}}]
             elif cmd == "GetNetPort":
@@ -1369,14 +1496,16 @@
                 body = [{"cmd": "GetHddInfo", "action": 0, "param": {}}]
             elif cmd == "GetUser":
                 body = [{"cmd": "GetUser", "action": 0, "param": {}}]
             elif cmd == "GetNtp":
                 body = [{"cmd": "GetNtp", "action": 0, "param": {}}]
             elif cmd == "GetTime":
                 body = [{"cmd": "GetTime", "action": 0, "param": {}}]
+            elif cmd == "GetPushCfg":
+                body = [{"cmd": "GetPushCfg", "action": 0, "param": {}}]
             elif cmd == "GetAbility":
                 body = [{"cmd": "GetAbility", "action": 0, "param": {"User": {"userName": self._username}}}]
 
         if body:
             try:
                 json_data = await self.send(body, expected_response_type="json")
             except InvalidContentTypeError as err:
@@ -1387,133 +1516,156 @@
             if channels:
                 self.map_channels_json_response(json_data, channels)
             else:
                 self.map_host_json_response(json_data)
 
         return
 
-    async def get_states(self, cmd_list: list[str] | None = None) -> None:
+    async def get_states(self, cmd_list: dict[str, list[int]] | None = None, wake: bool = True) -> None:
         body = []
         channels = []
         if cmd_list is None:
-            cmd_list = []
+            cmd_list = {}
+
+        any_battery = any(self.supported(ch, "battery") for ch in self._channels)
+        if any_battery and wake:
+            _LOGGER.debug("Host %s:%s: Waking the battery cameras for the get_states update", self._host, self._port)
+
+        def inc_host_cmd(cmd):
+            return (cmd in cmd_list or not cmd_list) and (wake or not any_battery or cmd not in WAKING_COMMANDS)
+
+        def inc_cmd(cmd, channel):
+            return (channel in cmd_list.get(cmd, []) or not cmd_list) and (wake or cmd not in WAKING_COMMANDS or not self.supported(channel, "battery"))
 
         for channel in self._stream_channels:
             ch_body = []
-            if "GetEnc" in cmd_list or not cmd_list:
+            if inc_cmd("GetEnc", channel):
                 ch_body.append({"cmd": "GetEnc", "action": 0, "param": {"channel": channel}})
             body.extend(ch_body)
             channels.extend([channel] * len(ch_body))
 
         for channel in self._channels:
             ch_body = []
-            if "GetIsp" in cmd_list or not cmd_list:
+            if inc_cmd("GetIsp", channel):
                 ch_body.append({"cmd": "GetIsp", "action": 0, "param": {"channel": channel}})
 
             if self.api_version("GetEvents") >= 1:
                 ch_body.append({"cmd": "GetEvents", "action": 0, "param": {"channel": channel}})
             else:
                 ch_body.append({"cmd": "GetMdState", "action": 0, "param": {"channel": channel}})
                 if self.ai_supported(channel):
                     ch_body.append({"cmd": "GetAiState", "action": 0, "param": {"channel": channel}})
 
-            if self.supported(channel, "ir_lights") and ("GetIrLights" in cmd_list or not cmd_list):
+            if self.supported(channel, "ir_lights") and inc_cmd("GetIrLights", channel):
                 ch_body.append({"cmd": "GetIrLights", "action": 0, "param": {"channel": channel}})
 
-            if self.supported(channel, "floodLight") and ("GetWhiteLed" in cmd_list or not cmd_list):
+            if self.supported(channel, "floodLight") and inc_cmd("GetWhiteLed", channel):
                 ch_body.append({"cmd": "GetWhiteLed", "action": 0, "param": {"channel": channel}})
 
-            if self.supported(channel, "status_led") and ("GetPowerLed" in cmd_list or not cmd_list):
+            if self.supported(channel, "battery") and inc_cmd("GetBatteryInfo", channel):
+                ch_body.append({"cmd": "GetBatteryInfo", "action": 0, "param": {"channel": channel}})
+
+            if self.supported(channel, "PIR") and inc_cmd("GetPirInfo", channel):
+                ch_body.append({"cmd": "GetPirInfo", "action": 0, "param": {"channel": channel}})
+
+            if self.supported(channel, "status_led") and inc_cmd("GetPowerLed", channel):
                 ch_body.append({"cmd": "GetPowerLed", "action": 0, "param": {"channel": channel}})
 
-            if self.supported(channel, "zoom") and ("GetZoomFocus" in cmd_list or not cmd_list):
+            if self.supported(channel, "zoom") and inc_cmd("GetZoomFocus", channel):
                 ch_body.append({"cmd": "GetZoomFocus", "action": 0, "param": {"channel": channel}})
 
-            if self.supported(channel, "auto_focus") and ("GetAutoFocus" in cmd_list or not cmd_list):
+            if self.supported(channel, "auto_focus") and inc_cmd("GetAutoFocus", channel):
                 ch_body.append({"cmd": "GetAutoFocus", "action": 0, "param": {"channel": channel}})
 
-            if self.supported(channel, "ptz_guard") and ("GetPtzGuard" in cmd_list or not cmd_list):
+            if self.supported(channel, "ptz_guard") and inc_cmd("GetPtzGuard", channel):
                 ch_body.append({"cmd": "GetPtzGuard", "action": 0, "param": {"channel": channel}})
 
-            if self.supported(channel, "ptz_position") and ("GetPtzCurPos" in cmd_list or not cmd_list):
+            if self.supported(channel, "ptz_position") and inc_cmd("GetPtzCurPos", channel):
                 ch_body.append({"cmd": "GetPtzCurPos", "action": 0, "param": {"PtzCurPos": {"channel": channel}}})
 
-            if self.supported(channel, "auto_track") and ("GetAiCfg" in cmd_list or not cmd_list):
+            if self.supported(channel, "auto_track") and inc_cmd("GetAiCfg", channel):
                 ch_body.append({"cmd": "GetAiCfg", "action": 0, "param": {"channel": channel}})
 
-            if self.supported(channel, "auto_track_limit") and ("GetPtzTraceSection" in cmd_list or not cmd_list):
+            if self.supported(channel, "auto_track_limit") and inc_cmd("GetPtzTraceSection", channel):
                 ch_body.append({"cmd": "GetPtzTraceSection", "action": 0, "param": {"PtzTraceSection": {"channel": channel}}})
 
-            if self.supported(channel, "volume") and ("GetAudioCfg" in cmd_list or not cmd_list):
+            if self.supported(channel, "volume") and inc_cmd("GetAudioCfg", channel):
                 ch_body.append({"cmd": "GetAudioCfg", "action": 0, "param": {"channel": channel}})
 
-            if self.supported(channel, "quick_reply") and ("GetAutoReply" in cmd_list or not cmd_list):
+            if self.supported(channel, "quick_reply") and inc_cmd("GetAutoReply", channel):
                 ch_body.append({"cmd": "GetAutoReply", "action": 0, "param": {"channel": channel}})
 
+            if self.supported(channel, "manual_record") and inc_cmd("GetManualRec", channel):
+                ch_body.append({"cmd": "GetManualRec", "action": 0, "param": {"channel": channel}})
+
             if (
                 self.supported(channel, "isp_hue")
                 or self.supported(channel, "isp_satruation")
                 or self.supported(channel, "isp_sharpen")
                 or self.supported(channel, "isp_contrast")
                 or self.supported(channel, "isp_bright")
-            ) and ("GetImage" in cmd_list or not cmd_list):
+            ) and inc_cmd("GetImage", channel):
                 ch_body.append({"cmd": "GetImage", "action": 0, "param": {"channel": channel}})
 
-            if (self.supported(channel, "buzzer") or (self.supported(None, "buzzer") and channel == 0)) and ("GetBuzzerAlarmV20" in cmd_list or not cmd_list):
+            if (self.supported(channel, "buzzer") or (self.supported(None, "buzzer") and channel == 0)) and inc_cmd("GetBuzzerAlarmV20", channel):
                 ch_body.append({"cmd": "GetBuzzerAlarmV20", "action": 0, "param": {"channel": channel}})
 
-            if (self.supported(channel, "email") or (self.supported(None, "email") and channel == 0)) and ("GetEmail" in cmd_list or not cmd_list):
+            if (self.supported(channel, "email") or (self.supported(None, "email") and channel == 0)) and inc_cmd("GetEmail", channel):
                 if self.api_version("GetEmail") >= 1:
                     ch_body.append({"cmd": "GetEmailV20", "action": 0, "param": {"channel": channel}})
                 else:
                     ch_body.append({"cmd": "GetEmail", "action": 0, "param": {"channel": channel}})
 
-            if (self.supported(channel, "push") or (self.supported(None, "push") and channel == 0)) and ("GetPush" in cmd_list or not cmd_list):
+            if (self.supported(channel, "push") or (self.supported(None, "push") and channel == 0)) and inc_cmd("GetPush", channel):
                 if self.api_version("GetPush") >= 1:
                     ch_body.append({"cmd": "GetPushV20", "action": 0, "param": {"channel": channel}})
                 else:
                     ch_body.append({"cmd": "GetPush", "action": 0, "param": {"channel": channel}})
 
-            if (self.supported(channel, "ftp") or (self.supported(None, "ftp") and channel == 0)) and ("GetFtp" in cmd_list or not cmd_list):
+            if (self.supported(channel, "ftp") or (self.supported(None, "ftp") and channel == 0)) and inc_cmd("GetFtp", channel):
                 if self.api_version("GetFtp") >= 1:
                     ch_body.append({"cmd": "GetFtpV20", "action": 0, "param": {"channel": channel}})
                 else:
                     ch_body.append({"cmd": "GetFtp", "action": 0, "param": {"channel": channel}})
 
-            if (self.supported(channel, "recording") or (self.supported(None, "recording") and channel == 0)) and ("GetRec" in cmd_list or not cmd_list):
+            if (self.supported(channel, "recording") or (self.supported(None, "recording") and channel == 0)) and inc_cmd("GetRec", channel):
                 if self.api_version("GetRec") >= 1:
                     ch_body.append({"cmd": "GetRecV20", "action": 0, "param": {"channel": channel}})
                 else:
                     ch_body.append({"cmd": "GetRec", "action": 0, "param": {"channel": channel}})
 
-            if self.supported(channel, "siren") and ("GetAudioAlarm" in cmd_list or not cmd_list):
+            if self.supported(channel, "siren") and inc_cmd("GetAudioAlarm", channel):
                 if self.api_version("GetAudioAlarm") >= 1:
                     ch_body.append({"cmd": "GetAudioAlarmV20", "action": 0, "param": {"channel": channel}})
                 else:
                     ch_body.append({"cmd": "GetAudioAlarm", "action": 0, "param": {"channel": channel}})
 
-            if self.supported(channel, "md_sensitivity") and ("GetMdAlarm" in cmd_list or not cmd_list):
+            if self.supported(channel, "md_sensitivity") and inc_cmd("GetMdAlarm", channel):
                 if self.api_version("GetMdAlarm") >= 1:
                     ch_body.append({"cmd": "GetMdAlarm", "action": 0, "param": {"channel": channel}})
                 else:
                     ch_body.append({"cmd": "GetAlarm", "action": 0, "param": {"Alarm": {"channel": channel, "type": "md"}}})
 
-            if self.supported(channel, "ai_sensitivity") and ("GetAiAlarm" in cmd_list or not cmd_list):
+            if self.supported(channel, "ai_sensitivity") and inc_cmd("GetAiAlarm", channel):
                 for ai_type in self.ai_supported_types(channel):
                     ch_body.append({"cmd": "GetAiAlarm", "action": 0, "param": {"channel": channel, "ai_type": ai_type}})
 
             body.extend(ch_body)
             channels.extend([channel] * len(ch_body))
 
         # host states
         host_body = []
-        if self.supported(None, "wifi") and self.wifi_connection and ("GetWifiSignal" in cmd_list or not cmd_list):
+        if self.supported(None, "wifi") and self.wifi_connection and inc_host_cmd("GetWifiSignal"):
             host_body.append({"cmd": "GetWifiSignal", "action": 0, "param": {}})
-        if self.supported(None, "hdd") and ("GetHddInfo" in cmd_list or not cmd_list):
+        if self.supported(None, "hdd") and inc_host_cmd("GetHddInfo"):
             host_body.append({"cmd": "GetHddInfo", "action": 0, "param": {}})
+        if self.supported(None, "sleep") and inc_host_cmd("GetChannelstatus"):
+            host_body.append({"cmd": "GetChannelstatus", "action": 0, "param": {}})
+        if self.supported(None, "push_config") and (inc_host_cmd("GetPush") or inc_host_cmd("GetPushCfg")):
+            host_body.append({"cmd": "GetPushCfg", "action": 0, "param": {}})
 
         body.extend(host_body)
         channels.extend([-1] * len(host_body))
 
         if not body:
             _LOGGER.debug(
                 "Host %s:%s: get_states, no channels connected so skipping request.",
@@ -1531,23 +1683,24 @@
             raise NoDataError(f"Host: {self._host}:{self._port}: error obtaining channel-state response") from err
 
         self.map_channels_json_response(json_data, channels)
 
     async def get_host_data(self) -> None:
         """Fetch the host settings/capabilities."""
         body: typings.reolink_json = [
-            {"cmd": "Getchannelstatus"},
+            {"cmd": "GetChannelstatus"},
             {"cmd": "GetDevInfo", "action": 0, "param": {}},
             {"cmd": "GetLocalLink", "action": 0, "param": {}},
             {"cmd": "GetNetPort", "action": 0, "param": {}},
             {"cmd": "GetP2p", "action": 0, "param": {}},
             {"cmd": "GetHddInfo", "action": 0, "param": {}},
             {"cmd": "GetUser", "action": 0, "param": {}},
             {"cmd": "GetNtp", "action": 0, "param": {}},
             {"cmd": "GetTime", "action": 0, "param": {}},
+            {"cmd": "GetPushCfg", "action": 0, "param": {}},
             {"cmd": "GetAbility", "action": 0, "param": {"User": {"userName": self._username}}},
         ]
 
         try:
             json_data = await self.send(body, expected_response_type="json")
         except InvalidContentTypeError as err:
             raise InvalidContentTypeError(f"Get host-settings error: {str(err)}") from err
@@ -1604,24 +1757,25 @@
                 continue
 
             ch_body.extend(
                 [
                     {"cmd": "GetWhiteLed", "action": 0, "param": {"channel": channel}},
                     {"cmd": "GetIrLights", "action": 0, "param": {"channel": channel}},
                     {"cmd": "GetAudioCfg", "action": 0, "param": {"channel": channel}},
+                    {"cmd": "GetManualRec", "action": 0, "param": {"channel": channel}},
                 ]
             )
             # one time values
             ch_body.append({"cmd": "GetOsd", "action": 0, "param": {"channel": channel}})
             if self.supported(channel, "quick_reply"):
                 ch_body.append({"cmd": "GetAudioFileList", "action": 0, "param": {"channel": channel}})
             if self.supported(channel, "webhook"):
                 ch_body.append({"cmd": "GetWebHook", "action": 0, "param": {"channel": channel}})
             # checking range
-            if self.supported(channel, "zoom_basic"):
+            if self.supported(channel, "zoom_basic") or self.api_version("supportDigitalZoom", channel) > 0:
                 ch_body.append({"cmd": "GetZoomFocus", "action": 1, "param": {"channel": channel}})
             if self.supported(channel, "pan_tilt") and self.api_version("ptzPreset", channel) >= 1:
                 ch_body.append({"cmd": "GetPtzPreset", "action": 0, "param": {"channel": channel}})
                 ch_body.append({"cmd": "GetPtzPatrol", "action": 0, "param": {"channel": channel}})
                 ch_body.append({"cmd": "GetPtzGuard", "action": 0, "param": {"channel": channel}})
                 ch_body.append({"cmd": "GetPtzCurPos", "action": 0, "param": {"PtzCurPos": {"channel": channel}}})
             if self.supported(channel, "auto_track"):
@@ -1707,15 +1861,19 @@
                 await self.get_rtsp_stream_source(channel, "sub")
                 await self.get_rtsp_stream_source(channel, "main")
 
     async def get_motion_state(self, channel: int) -> Optional[bool]:
         if channel not in self._channels:
             return None
 
-        body = [{"cmd": "GetMdState", "action": 0, "param": {"channel": channel}}]
+        if self.api_version("GetEvents") >= 1:
+            # Needed because battery cams use PIR detection with the "other" item
+            body = [{"cmd": "GetEvents", "action": 0, "param": {"channel": channel}}]
+        else:
+            body = [{"cmd": "GetMdState", "action": 0, "param": {"channel": channel}}]
 
         try:
             json_data = await self.send(body, expected_response_type="json")
         except InvalidContentTypeError:
             _LOGGER.error(
                 "Host %s:%s: error translating motion detection state response for channel %s.",
                 self._host,
@@ -1992,15 +2150,24 @@
         except ReolinkError:
             pass
 
         if not self.supported(None, "update"):
             raise NotSupportedError(f"update_firmware: not supported by {self.nvr_name}")
 
         body = [{"cmd": "UpgradeOnline"}]
-        await self.send_setting(body)
+        try:
+            await self.send_setting(body)
+        except ApiError as err:
+            if err.rspCode == -30:  # same version
+                raise ApiError(
+                    "Reolink device could not find new firmware, "
+                    "try downloading from the Reolink download center (https://reolink.com/download-center) and update manually",
+                    rspCode=err.rspCode,
+                ) from err
+            raise err
 
     async def update_progress(self) -> bool | int:
         """check progress of firmware update, returns False if not in progress."""
         if not self.supported(None, "update"):
             raise NotSupportedError(f"update_progress: not supported by {self.nvr_name}")
 
         body = [{"cmd": "UpgradeStatus"}]
@@ -2024,15 +2191,15 @@
 
         body = [{"cmd": "Reboot"}]
         json_data = await self.send(body, expected_response_type="json")
 
         if json_data[0]["code"] != 0 or json_data[0].get("value", {}).get("rspCode", -1) != 200:
             rspCode = json_data[0].get("value", json_data[0]["error"])["rspCode"]
             detail = json_data[0].get("value", json_data[0]["error"]).get("detail", "")
-            raise ApiError(f"Reboot: API returned error code {json_data[0]['code']}, response code {rspCode}/{detail}")
+            raise ApiError(f"Reboot: API returned error code {json_data[0]['code']}, response code {rspCode}/{detail}", rspCode=rspCode)
 
     async def get_snapshot(self, channel: int, stream: Optional[str] = None) -> bytes | None:
         """Get the still image."""
         if channel not in self._stream_channels:
             return None
 
         if stream is None:
@@ -2048,14 +2215,21 @@
             stream = stream.removeprefix("snapshots_")
 
         if stream not in ["main", "sub"]:
             stream = "main"
 
         param["snapType"] = stream
 
+        if stream == "sub":
+            height = self._enc_settings.get(channel, {}).get("Enc", {}).get(f"{stream}Stream", {}).get("height")
+            width = self._enc_settings.get(channel, {}).get("Enc", {}).get(f"{stream}Stream", {}).get("width")
+            if height is not None and width is not None:
+                param["width"] = width
+                param["height"] = height
+
         body: typings.reolink_json = [{}]
         response = await self.send(body, param, expected_response_type="image/jpeg")
         if response is None or response == b"":
             _LOGGER.error(
                 "Host: %s:%s: error obtaining still image response for channel %s.",
                 self._host,
                 self._port,
@@ -2145,14 +2319,16 @@
 
         if stream is None:
             stream = self._stream
 
         if channel in self._rtsp_verified and stream in self._rtsp_verified[channel]:
             return self._rtsp_verified[channel][stream]
 
+        _LOGGER.debug("Checking RTSP urls host %s:%s, channel %s, stream %s", self._host, self._port, channel, stream)
+
         if self.api_version("rtsp") >= 3 and stream == "main" and channel in self._rtsp_mainStream:
             if await self._check_rtsp_url(self._rtsp_mainStream[channel], channel, stream):
                 return self._rtsp_mainStream[channel]
         if self.api_version("rtsp") >= 3 and stream == "sub" and channel in self._rtsp_subStream:
             if await self._check_rtsp_url(self._rtsp_subStream[channel], channel, stream):
                 return self._rtsp_subStream[channel]
 
@@ -2200,15 +2376,15 @@
             return url
 
         url = f"rtsp://{self._username}:{password}@{self._host}:{self._rtsp_port}/Preview_{channel_str}_{stream}"
         if await self._check_rtsp_url(url, channel, stream):
             return url
 
         # return the first tried URL (based on camera capabilities as above)
-        _LOGGER.error("Host %s:%s, could not verify a working RTSP url for stream %s", self._host, self._port, stream)
+        _LOGGER.error("Host %s:%s, could not verify a working RTSP url for channel %s, stream %s", self._host, self._port, channel, stream)
         return self._rtsp_verified[channel][stream]
 
     async def get_stream_source(self, channel: int, stream: Optional[str] = None) -> Optional[str]:
         """Return the stream source url."""
         try:
             await self.login()
         except LoginError:
@@ -2361,58 +2537,71 @@
             raise UnexpectedDataError(f"Host {self._host}:{self._port}: Download VOD: no 'content_length' in the response")
         if response.content_disposition is None or response.content_disposition.filename is None:
             response.release()
             raise UnexpectedDataError(f"Host {self._host}:{self._port}: Download VOD: no 'content_disposition.filename' in the response")
 
         return typings.VOD_download(response.content_length, response.content_disposition.filename, response.content, response.release, response.headers.get("ETag"))
 
+    def ensure_channel_uid_unique(self):
+        """Make sure the channel UIDs are all unique."""
+        rev_channel_uids = {}
+        for key, value in self._channel_uids.items():
+            rev_channel_uids.setdefault(value, set()).add(key)
+        duplicate_uids = [values for key, values in rev_channel_uids.items() if len(values) > 1]
+        for duplicate in duplicate_uids:
+            for ch in duplicate:
+                self._channel_uids[ch] = f"{self._channel_uids[ch]}_{ch}"
+
     def map_host_json_response(self, json_data: typings.reolink_json):
         """Map the JSON objects to internal cache-objects."""
         for data in json_data:
             try:
                 if data["code"] == 1:  # Error, like "ability error"
                     continue
 
                 if data["cmd"] == "GetChannelstatus":
+                    cur_status = data["value"]["status"]
+
                     if not self._GetChannelStatus_present and (self._nvr_num_channels == 0 or len(self._channels) == 0):
                         self._channels.clear()
                         self._is_doorbell.clear()
 
-                        cur_value = data["value"]
-                        self._nvr_num_channels = cur_value["count"]
-
+                        self._nvr_num_channels = data["value"]["count"]
                         if self._nvr_num_channels > 0:
-                            cur_status = cur_value["status"]
-
                             # Not all Reolink devices respond with "name" attribute.
                             if "name" in cur_status[0]:
                                 self._GetChannelStatus_has_name = True
                                 self._channel_names.clear()
                             else:
                                 self._GetChannelStatus_has_name = False
 
                             for ch_info in cur_status:
                                 if ch_info["online"] == 1:
                                     cur_channel = ch_info["channel"]
 
-                                    if self._GetChannelStatus_has_name:
-                                        self._channel_names[cur_channel] = ch_info["name"]
-
                                     if "typeInfo" in ch_info:  # Not all Reolink devices respond with "typeInfo" attribute.
                                         self._channel_models[cur_channel] = ch_info["typeInfo"]
                                         self._is_doorbell[cur_channel] = "Doorbell" in self._channel_models[cur_channel]
 
+                                    if "uid" in ch_info:
+                                        self._channel_uids[cur_channel] = ch_info["uid"]
+
                                     self._channels.append(cur_channel)
+
+                            self.ensure_channel_uid_unique()
                         else:
                             self._channel_names.clear()
-                    elif self._GetChannelStatus_has_name:
-                        cur_status = data["value"]["status"]
-                        for ch_info in cur_status:
-                            if ch_info["online"] == 1:
-                                self._channel_names[ch_info["channel"]] = ch_info["name"]
+
+                    for ch_info in cur_status:
+                        if ch_info["online"] == 1:
+                            cur_channel = ch_info["channel"]
+                            if "name" in ch_info:
+                                self._channel_names[cur_channel] = ch_info["name"]
+                            if "sleep" in ch_info:
+                                self._sleep[cur_channel] = ch_info["sleep"] == 1
 
                     if not self._GetChannelStatus_present:
                         self._GetChannelStatus_present = True
 
                     break
 
             except Exception as err:  # pylint: disable=bare-except
@@ -2428,16 +2617,16 @@
         for data in json_data:
             try:
                 if data["code"] == 1:  # Error, like "ability error"
                     continue
 
                 if data["cmd"] == "GetDevInfo":
                     dev_info = data["value"]["DevInfo"]
-                    self._is_nvr = dev_info.get("exactType", "IPC") in ["NVR", "WIFI_NVR"]
-                    self._is_nvr = self._is_nvr or dev_info.get("type", "IPC") == "NVR"
+                    self._is_nvr = dev_info.get("exactType", "IPC") in ["NVR", "WIFI_NVR", "HOMEHUB"]
+                    self._is_nvr = self._is_nvr or dev_info.get("type", "IPC") in ["NVR", "WIFI_NVR", "HOMEHUB"]
                     self._nvr_serial = dev_info["serial"]
                     self._nvr_name = dev_info["name"]
                     self._nvr_model = dev_info["model"]
                     self._nvr_hw_version = dev_info["hardVer"]
                     self._nvr_sw_version = dev_info["firmVer"]
                     if self._nvr_sw_version is not None:
                         self._nvr_sw_version_object = SoftwareVersion(self._nvr_sw_version)
@@ -2497,14 +2686,17 @@
                 elif data["cmd"] == "GetTime":
                     time_diffrence = (datetime.now() - reolink_time_to_datetime(data["value"]["Time"])).total_seconds()
                     if abs(time_diffrence) < 10:
                         time_diffrence = 0
                     self._host_time_difference = time_diffrence
                     self._time_settings = data["value"]
 
+                elif data["cmd"] == "GetPushCfg":
+                    self._push_config = data["value"]
+
                 elif data["cmd"] == "GetAbility":
                     self._abilities = data["value"]["Ability"]
 
             except Exception as err:  # pylint: disable=bare-except
                 _LOGGER.error(
                     "Host %s:%s failed mapping JSON data: %s, traceback:\n%s\n",
                     self._host,
@@ -2552,16 +2744,20 @@
                     if "ai" in data["value"]:
                         self._ai_detection_states[channel] = {}
                         self._ai_detection_support[channel] = {}
                         for key, value in data["value"]["ai"].items():
                             supported: bool = value.get("support", 0) == 1
                             self._ai_detection_states[channel][key] = supported and value.get("alarm_state", 0) == 1
                             self._ai_detection_support[channel][key] = supported
+                        if "other" in data["value"]["ai"]:  # Battery cams use PIR detection with the "other" item
+                            if data["value"]["ai"]["other"].get("support", 0) == 1:
+                                self._motion_detection_states[channel] = data["value"]["ai"]["other"]["alarm_state"] == 1
                     if "md" in data["value"]:
-                        self._motion_detection_states[channel] = data["value"]["md"]["alarm_state"] == 1
+                        if data["value"]["md"].get("support", 1) == 1:  # Battery cams use PIR detection with the "other" item
+                            self._motion_detection_states[channel] = data["value"]["md"]["alarm_state"] == 1
                     if "visitor" in data["value"]:
                         value = data["value"]["visitor"]
                         supported = value.get("support", 0) == 1
                         self._visitor_states[channel] = supported and value.get("alarm_state", 0) == 1
                         self._is_doorbell[channel] = supported
 
                 elif data["cmd"] == "GetMdState":
@@ -2679,20 +2875,29 @@
                     # response_channel = data["value"]["PowerLed"]["channel"]
                     self._status_led_settings[channel] = data["value"]
 
                 elif data["cmd"] == "GetWhiteLed":
                     response_channel = data["value"]["WhiteLed"]["channel"]
                     self._whiteled_settings[channel] = data["value"]
 
+                elif data["cmd"] == "GetBatteryInfo":
+                    self._battery[channel] = data["value"]["Battery"]
+
+                elif data["cmd"] == "GetPirInfo":
+                    self._pir[channel] = data["value"]["pirInfo"]
+
                 elif data["cmd"] == "GetRec":
                     self._recording_settings[channel] = data["value"]
 
                 elif data["cmd"] == "GetRecV20":
                     self._recording_settings[channel] = data["value"]
 
+                elif data["cmd"] == "GetManualRec":
+                    self._manual_record_settings[channel] = data["value"]
+
                 elif data["cmd"] == "GetPtzPreset":
                     self._ptz_presets_settings[channel] = data["value"]
                     self._ptz_presets[channel] = {}
                     for preset in data["value"]["PtzPreset"]:
                         if int(preset["enable"]) == 1:
                             preset_name = preset["name"]
                             preset_id = int(preset["id"])
@@ -3244,20 +3449,24 @@
 
         body: typings.reolink_json
         on_off = 1 if enable else 0
         if channel is None:
             if self.api_version("GetPush") >= 1:
                 body = [{"cmd": "SetPushV20", "action": 0, "param": {"Push": {"enable": on_off}}}]
                 await self.send_setting(body)
+                if self.supported(None, "push_config"):
+                    await self.get_state(cmd="GetPushCfg")
                 return
 
             for ch in self._channels:
                 if self.supported(ch, "push"):
                     body = [{"cmd": "SetPush", "action": 0, "param": {"Push": {"schedule": {"enable": on_off, "channel": ch}}}}]
                     await self.send_setting(body)
+            if self.supported(None, "push_config"):
+                await self.get_state(cmd="GetPushCfg")
             return
 
         if channel not in self._channels:
             raise InvalidParameterError(f"set_push: no camera connected to channel '{channel}'")
 
         if self.api_version("GetPush") >= 1:
             body = [{"cmd": "SetPushV20", "action": 0, "param": {"Push": {"scheduleEnable": on_off, "schedule": {"channel": channel}}}}]
@@ -3348,14 +3557,25 @@
         if self.api_version("GetRec") >= 1:
             body = [{"cmd": "SetRecV20", "action": 0, "param": {"Rec": {"scheduleEnable": on_off, "schedule": {"channel": channel}}}}]
         else:
             body = [{"cmd": "SetRec", "action": 0, "param": {"Rec": {"schedule": {"enable": on_off, "channel": channel}}}}]
 
         await self.send_setting(body)
 
+    async def set_manual_record(self, channel: int, enable: bool) -> None:
+        """Start/Stop manual recording."""
+        if not self.supported(channel, "manual_record"):
+            raise NotSupportedError(f"set_manual_record: manual recording on camera {self.camera_name(channel)} is not available")
+        if channel not in self._channels:
+            raise InvalidParameterError(f"set_manual_record: no camera connected to channel '{channel}'")
+
+        on_off = 1 if enable else 0
+        body = [{"cmd": "SetManualRec", "action": 0, "param": {"Rec": {"channel": channel, "enable": on_off}}}]
+        await self.send_setting(body)
+
     async def set_buzzer(self, channel: int | None, enable: bool) -> None:
         """Set the NVR buzzer parameter."""
         if not self.supported(channel, "buzzer"):
             raise NotSupportedError(f"set_buzzer: NVR buzzer on camera {self.camera_name(channel)} is not available")
 
         body: typings.reolink_json
         on_off = 1 if enable else 0
@@ -3395,30 +3615,30 @@
                 "action": 0,
                 "param": {"IrLights": {"channel": channel, "state": state}},
             }
         ]
 
         await self.send_setting(body)
 
-    async def set_status_led(self, channel: int, state: bool | str) -> None:
+    async def set_status_led(self, channel: int, state: bool | str, doorbell: bool = False) -> None:
         if channel not in self._channels:
             raise InvalidParameterError(f"set_status_led: no camera connected to channel '{channel}'")
         if not self.supported(channel, "status_led"):
             raise NotSupportedError(f"set_status_led: Status led on camera {self.camera_name(channel)} is not available")
 
         if isinstance(state, bool):
             value = "On" if state else "Off"
         else:
             value = state
 
         val_list = [val.value for val in StatusLedEnum]
         if value not in val_list:
             raise InvalidParameterError(f"set_status_led: value {value} not in {val_list}")
 
-        if self.is_doorbell(channel):
+        if doorbell:
             param = {"channel": channel, "eDoorbellLightState": value}
         else:
             param = {"channel": channel, "state": value}
 
         body: typings.reolink_json = [{"cmd": "SetPowerLed", "action": 0, "param": {"PowerLed": param}}]
         await self.send_setting(body)
 
@@ -3595,17 +3815,14 @@
         if time is not None:
             params["timeout"] = time
 
         body = [{"cmd": "SetAutoReply", "action": 0, "param": {"AutoReply": params}}]
         await self.send_setting(body)
 
     async def set_audio_alarm(self, channel: int, enable: bool) -> None:
-        # fairly basic only either turns it off or on
-        # called in its simple form by set_siren
-
         if channel not in self._channels:
             raise InvalidParameterError(f"set_audio_alarm: no camera connected to channel '{channel}'")
         if not self.supported(channel, "siren"):
             raise NotSupportedError(f"set_audio_alarm: AudioAlarm on camera {self.camera_name(channel)} is not available")
 
         if self.api_version("GetAudioAlarm") >= 1:
             body = [{"cmd": "SetAudioAlarmV20", "param": {"Audio": {"enable": 1 if enable else 0, "schedule": {"channel": channel}}}}]
@@ -3623,17 +3840,14 @@
                     },
                 }
             ]
 
         await self.send_setting(body)
 
     async def set_siren(self, channel: int, enable: bool = True, duration: int | None = 2) -> None:
-        # Uses API AudioAlarmPlay with manual switch
-        # uncertain if there may be a glitch - dont know if there is API I have yet to find
-        # which sets AudioLevel
         if channel not in self._channels:
             raise InvalidParameterError(f"set_siren: no camera connected to channel '{channel}'")
         if duration is not None and not isinstance(duration, int):
             raise InvalidParameterError(f"set_siren: duration '{duration}' is not integer")
         if not self.supported(channel, "siren_play"):
             raise NotSupportedError(f"set_siren: AudioAlarmPlay on camera {self.camera_name(channel)} is not available")
 
@@ -3734,14 +3948,36 @@
             raise NotSupportedError(f"set_motion_detection: alarm on camera {self.camera_name(channel)} is not available")
 
         body: typings.reolink_json = [{"cmd": "SetAlarm", "action": 0, "param": self._md_alarm_settings[channel]}]
         body[0]["param"]["Alarm"]["enable"] = 1 if enable else 0
 
         await self.send_setting(body)
 
+    async def set_pir(self, channel: int, enable: bool | None = None, reduce_alarm: bool | None = None, sensitivity: int | None = None) -> None:
+        """Set PIR settings."""
+        if channel not in self._channels:
+            raise InvalidParameterError(f"set_pir: no camera connected to channel '{channel}'")
+        if channel not in self._pir:
+            raise NotSupportedError(f"set_pir: PIR settings on camera {self.camera_name(channel)} are not available")
+        if sensitivity is not None and not isinstance(sensitivity, int):
+            raise InvalidParameterError(f"set_pir: sensitivity '{sensitivity}' is not integer")
+        if sensitivity is not None and (sensitivity < 1 or sensitivity > 100):
+            raise InvalidParameterError(f"set_pir: sensitivity {sensitivity} not in range 1...100")
+
+        pir = {"channel": channel}
+        if enable is not None:
+            pir["enable"] = 1 if enable else 0
+        if reduce_alarm is not None:
+            pir["reduceAlarm"] = 1 if reduce_alarm else 0
+        if sensitivity is not None:
+            pir["sensitive"] = int(101 - sensitivity)
+
+        body: typings.reolink_json = [{"cmd": "SetPirInfo", "action": 0, "param": {"pirInfo": pir}}]
+        await self.send_setting(body)
+
     async def set_md_sensitivity(self, channel: int, value: int) -> None:
         """Set motion detection sensitivity.
         Here the camera web and windows application show a completely different value than set.
         So the calculation <51 - value> makes the "real" value.
         """
         if channel not in self._channels:
             raise InvalidParameterError(f"set_md_sensitivity: no camera connected to channel '{channel}'")
@@ -3963,15 +4199,15 @@
         _LOGGER.debug("Response from cmd '%s' from %s:%s: %s", command, self._host, self._port, json_data)
 
         try:
             if json_data[0]["code"] != 0 or json_data[0].get("value", {}).get("rspCode", -1) != 200:
                 _LOGGER.debug("ApiError for command '%s', response: %s", command, json_data)
                 rspCode = json_data[0].get("value", json_data[0]["error"])["rspCode"]
                 detail = json_data[0].get("value", json_data[0]["error"]).get("detail", "")
-                raise ApiError(f"cmd '{command}': API returned error code {json_data[0]['code']}, response code {rspCode}/{detail}")
+                raise ApiError(f"cmd '{command}': API returned error code {json_data[0]['code']}, response code {rspCode}/{detail}", rspCode=rspCode)
         except KeyError as err:
             raise UnexpectedDataError(f"Host {self._host}:{self._port}: received an unexpected response from command '{command}': {json_data}") from err
 
         if command[:3] == "Set":
             getcmd = command.replace("Set", "Get")
             if wait_before_get > 0:
                 await asyncio.sleep(wait_before_get)
@@ -4174,32 +4410,37 @@
                 elif cur_command in ["Snap", "Download"]:
                     _LOGGER_DATA.debug("%s/%s:%s::send() HTTP Response (snapshot/download) data scrapped because it's too large.", self.nvr_name, self._host, self._port)
                 else:
                     _LOGGER_DATA.debug("%s/%s:%s::send() HTTP Response data:\n%s\n", self.nvr_name, self._host, self._port, self._hide_password(data))
 
             if len(data) < 500 and response.content_type == "text/html":
                 if isinstance(data, bytes):
-                    login_err = b'"detail" : "invalid user"' in data or b'"detail" : "login failed"' in data or b'detail" : "please login first' in data
+                    login_err = b'detail" : "please login first' in data and cur_command != "Logout"
+                    cred_err = (
+                        b'"detail" : "invalid user"' in data or b'"detail" : "login failed"' in data or b'"detail" : "password wrong"' in data
+                    ) and cur_command != "Logout"
                 else:
-                    login_err = (
-                        '"detail" : "invalid user"' in data or '"detail" : "login failed"' in data or 'detail" : "please login first' in data
+                    login_err = ('"detail" : "please login first"' in data) and cur_command != "Logout"
+                    cred_err = (
+                        '"detail" : "invalid user"' in data or '"detail" : "login failed"' in data or '"detail" : "password wrong"' in data
                     ) and cur_command != "Logout"
-                if login_err:
+                if login_err or cred_err:
                     response.release()
-                    if is_login_logout:
-                        raise CredentialsInvalidError()
-
+                    await self.expire_session()
+                    if cred_err and cur_command == "Login":
+                        raise CredentialsInvalidError(f"Host {self._host}:{self._port}: Invalid credentials during login")
                     if retry <= 0:
-                        raise CredentialsInvalidError()
+                        if cred_err:
+                            raise CredentialsInvalidError(f"Host {self._host}:{self._port}: Invalid credentials after retries")
+                        raise LoginError(f"Host {self._host}:{self._port}: Received 'please login first'")
                     _LOGGER.debug(
                         'Host %s:%s: "invalid login" response, trying to login again and retry the command.',
                         self._host,
                         self._port,
                     )
-                    await self.expire_session()
                     return await self.send(body, param, expected_response_type, retry)
 
             if is_login_logout and response.status == 300:
                 response.release()
                 raise ApiError(f"API returned HTTP status ERROR code {response.status}/{response.reason}, this may happen if you use HTTP and the camera expects HTTPS")
 
             if response.status == 502 and retry > 0:
@@ -4272,14 +4513,32 @@
                         self._host,
                         self._port,
                         len(json_data),
                         len(body),
                     )
                     await self.expire_session(unsubscribe=False)
                     return await self.send(body, param, expected_response_type, retry)
+                # retry commands that have not been received by the camera (battery cam waking from sleep)
+                retry_cmd = []
+                retry_idxs = []
+                for idx, cmd_data in enumerate(json_data):
+                    if cmd_data["code"] != 0 and cmd_data.get("error", {}).get("rspCode", 0) in [-12, -13, -17]:
+                        retry_cmd.append(body[idx])
+                        retry_idxs.append(idx)
+                if retry_cmd and retry > 0:
+                    _LOGGER.debug(
+                        "cmd %s: returned response code %s/%s, retrying in 1.0 s",
+                        [cmd.get("cmd") for cmd in retry_cmd],
+                        [json_data[idx].get("error", {}).get("rspCode") for idx in retry_idxs],
+                        [json_data[idx].get("error", {}).get("detail") for idx in retry_idxs],
+                    )
+                    await asyncio.sleep(1.0)  # give the battery cam time to wake
+                    retry_data = await self.send(retry_cmd, param, expected_response_type, retry)
+                    for idx, retry_resp in enumerate(retry_data):
+                        json_data[retry_idxs[idx]] = retry_resp
                 return json_data
 
             if expected_response_type == "image/jpeg" and isinstance(data, bytes):
                 return data
 
             if expected_response_type == "text/html" and isinstance(data, str):
                 return data
@@ -4321,16 +4580,15 @@
             await self.expire_session()
             raise err
         except ApiError as err:
             _LOGGER.error("Host %s:%s: API error: %s.", self._host, self._port, str(err))
             await self.expire_session(unsubscribe=False)
             raise err
         except CredentialsInvalidError as err:
-            _LOGGER.error("Host %s:%s: login attempt failed.", self._host, self._port)
-            await self.expire_session()
+            _LOGGER.error(str(err))
             raise err
         except InvalidContentTypeError as err:
             _LOGGER.debug("Host %s:%s: content type error: %s.", self._host, self._port, str(err))
             await self.expire_session(unsubscribe=False)
             raise err
         except Exception as err:
             _LOGGER.error('Host %s:%s: unknown exception "%s" occurred, traceback:\n%s\n', self._host, self._port, str(err), traceback.format_exc())
@@ -4382,15 +4640,15 @@
             raise InvalidContentTypeError(f"Error translating JSON response: {str(err)}, from {URL}, " f"content type '{response.content_type}', data:\n{data}\n") from err
 
         if json_data is None:
             raise NoDataError(f"Request to {URL} returned no data: {data}")
 
         resp_code = json_data.get("result", {}).get("code")
         if resp_code != 0:
-            raise ApiError(f"Request to {URL} returned error code {resp_code}, data:\n{json_data}")
+            raise ApiError(f"Request to {URL} returned error code {resp_code}, data:\n{json_data}", rspCode=resp_code)
 
         return json_data
 
     ##############################################################################
     # WEBHOOK managing
     async def webhook_add(self, channel: int, webhook_url: str):
         """
@@ -4609,14 +4867,16 @@
         headers = templates.HEADERS
         if sub_type == SubType.push:
             headers.update(templates.SUBSCRIBE_ACTION)
             template = templates.SUBSCRIBE_XML
         elif sub_type == SubType.long_poll:
             headers.update(templates.PULLPOINT_ACTION)
             template = templates.PULLPOINT_XML
+        else:
+            raise SubscriptionError(f"Host {self._host}:{self._port}: subscription type '{sub_type}' not supported")
 
         parameters = {
             "InitialTerminationTime": f"PT{SUBSCRIPTION_TERMINATION_TIME}M",
         }
         if webhook_url is not None and sub_type == SubType.push:
             parameters["Address"] = webhook_url
```

### Comparing `reolink_aio-0.8.9/reolink_aio/enums.py` & `reolink_aio-0.9.0/reolink_aio/enums.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,7 +76,15 @@
     """Options for AI Track Method"""
 
     # off = 0
     # pantilt = 1
     digital = 2
     digitalfirst = 3
     pantiltfirst = 4
+
+
+class BatteryEnum(Enum):
+    """Battery status"""
+
+    discharging = 0
+    charging = 1
+    chargecomplete = 2
```

### Comparing `reolink_aio-0.8.9/reolink_aio/exceptions.py` & `reolink_aio-0.9.0/reolink_aio/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """Reolink NVR/camera API."""
 
+from __future__ import annotations
 from asyncio import TimeoutError as AsyncioTimeoutError
 
 
 class ReolinkError(Exception):
     """Base Reolink error class"""
 
 
 class ApiError(ReolinkError):
     """Raised when API returns an error code"""
 
+    def __init__(self, message: str, rspCode: int | None = None):
+        super().__init__(message)
+        self.rspCode = rspCode
+
 
 class InvalidContentTypeError(ReolinkError):
     """Raised when a command returns an unexpected content type"""
 
 
 class CredentialsInvalidError(ReolinkError):
     """Raised when an API call returns credentials issue"""
```

### Comparing `reolink_aio-0.8.9/reolink_aio/software_version.py` & `reolink_aio-0.9.0/reolink_aio/software_version.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.9/reolink_aio/templates.py` & `reolink_aio-0.9.0/reolink_aio/templates.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.9/reolink_aio/typings.py` & `reolink_aio-0.9.0/reolink_aio/typings.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.9/reolink_aio/utils.py` & `reolink_aio-0.9.0/reolink_aio/utils.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.8.9/reolink_aio.egg-info/PKG-INFO` & `reolink_aio-0.9.0/reolink_aio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink_aio
-Version: 0.8.9
+Version: 0.9.0
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink_aio Version: 0.8.9 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink_aio Version: 0.9.0 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.8.9/setup.py` & `reolink_aio-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='reolink_aio',
-      version='0.8.9',
+      version='0.9.0',
       description='Reolink NVR/cameras API package',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/starkillerOG/reolink_aio',
       author='starkillerOG',
       author_email='starkiller.og@gmail.com',
       license='MIT',
```

### Comparing `reolink_aio-0.8.9/tests/test.py` & `reolink_aio-0.9.0/tests/test.py`

 * *Files identical despite different names*

