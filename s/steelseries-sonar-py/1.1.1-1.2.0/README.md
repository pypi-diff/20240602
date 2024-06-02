# Comparing `tmp/steelseries_sonar_py-1.1.1.tar.gz` & `tmp/steelseries_sonar_py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steelseries_sonar_py-1.1.1.tar", last modified: Sun May 26 11:07:47 2024, max compression
+gzip compressed data, was "steelseries_sonar_py-1.2.0.tar", last modified: Sun Jun  2 14:02:21 2024, max compression
```

## Comparing `steelseries_sonar_py-1.1.1.tar` & `steelseries_sonar_py-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:07:47.240359 steelseries_sonar_py-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:07:47.236359 steelseries_sonar_py-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:07:47.236359 steelseries_sonar_py-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-26 11:07:42.000000 steelseries_sonar_py-1.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-26 11:07:42.000000 steelseries_sonar_py-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-26 11:07:42.000000 steelseries_sonar_py-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-26 11:07:47.240359 steelseries_sonar_py-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-26 11:07:42.000000 steelseries_sonar_py-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-26 11:07:42.000000 steelseries_sonar_py-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:07:47.240359 steelseries_sonar_py-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-26 11:07:42.000000 steelseries_sonar_py-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:07:47.236359 steelseries_sonar_py-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:07:47.236359 steelseries_sonar_py-1.1.1/src/steelseries_sonar_py/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 11:07:42.000000 steelseries_sonar_py-1.1.1/src/steelseries_sonar_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-26 11:07:42.000000 steelseries_sonar_py-1.1.1/src/steelseries_sonar_py/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-26 11:07:42.000000 steelseries_sonar_py-1.1.1/src/steelseries_sonar_py/sonar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:07:47.240359 steelseries_sonar_py-1.1.1/src/steelseries_sonar_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-26 11:07:47.000000 steelseries_sonar_py-1.1.1/src/steelseries_sonar_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-26 11:07:47.000000 steelseries_sonar_py-1.1.1/src/steelseries_sonar_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:07:47.000000 steelseries_sonar_py-1.1.1/src/steelseries_sonar_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-26 11:07:47.000000 steelseries_sonar_py-1.1.1/src/steelseries_sonar_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 11:07:47.000000 steelseries_sonar_py-1.1.1/src/steelseries_sonar_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-26 11:07:42.000000 steelseries_sonar_py-1.1.1/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:02:21.436680 steelseries_sonar_py-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:02:21.432680 steelseries_sonar_py-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:02:21.432680 steelseries_sonar_py-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-06-02 14:02:16.000000 steelseries_sonar_py-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-06-02 14:02:16.000000 steelseries_sonar_py-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-06-02 14:02:16.000000 steelseries_sonar_py-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-06-02 14:02:21.436680 steelseries_sonar_py-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-06-02 14:02:16.000000 steelseries_sonar_py-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-02 14:02:16.000000 steelseries_sonar_py-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 14:02:21.436680 steelseries_sonar_py-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-06-02 14:02:16.000000 steelseries_sonar_py-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:02:21.432680 steelseries_sonar_py-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:02:21.432680 steelseries_sonar_py-1.2.0/src/steelseries_sonar_py/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 14:02:16.000000 steelseries_sonar_py-1.2.0/src/steelseries_sonar_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-06-02 14:02:16.000000 steelseries_sonar_py-1.2.0/src/steelseries_sonar_py/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-06-02 14:02:16.000000 steelseries_sonar_py-1.2.0/src/steelseries_sonar_py/sonar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:02:21.436680 steelseries_sonar_py-1.2.0/src/steelseries_sonar_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-06-02 14:02:21.000000 steelseries_sonar_py-1.2.0/src/steelseries_sonar_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-06-02 14:02:21.000000 steelseries_sonar_py-1.2.0/src/steelseries_sonar_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 14:02:21.000000 steelseries_sonar_py-1.2.0/src/steelseries_sonar_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-02 14:02:21.000000 steelseries_sonar_py-1.2.0/src/steelseries_sonar_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 14:02:21.000000 steelseries_sonar_py-1.2.0/src/steelseries_sonar_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-06-02 14:02:16.000000 steelseries_sonar_py-1.2.0/test.py
```

### Comparing `steelseries_sonar_py-1.1.1/.github/workflows/publish.yml` & `steelseries_sonar_py-1.2.0/.github/workflows/publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         path: dist/
 
   publish-to-testpypi:
     name: Publish Python distribution to TestPyPI
     needs:
     - build
     runs-on: ubuntu-latest
+    if: github.event_name == 'push'
 
     environment:
       name: testpypi
       url: https://test.pypi.org/p/steelseries-sonar-py
 
     permissions:
       id-token: write  # IMPORTANT: mandatory for trusted publishing
```

### Comparing `steelseries_sonar_py-1.1.1/.gitignore` & `steelseries_sonar_py-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `steelseries_sonar_py-1.1.1/LICENSE` & `steelseries_sonar_py-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `steelseries_sonar_py-1.1.1/PKG-INFO` & `steelseries_sonar_py-1.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,18 @@
-Metadata-Version: 2.1
-Name: steelseries-sonar-py
-Version: 1.1.1
-Summary: Simple Python wrapper for the SteelSeries Sonar API
-Home-page: https://github.com/Mark7888/steelseries-sonar-py
-Author: Mark7888
-Author-email: l.mark7888@gmail.com
-Project-URL: Documentation, https://github.com/Mark7888/steelseries-sonar-py/blob/master/README.md
-Project-URL: Bug Reports, https://github.com/Mark7888/steelseries-sonar-py/issues
-Project-URL: Source Code, https://github.com/Mark7888/steelseries-sonar-py
-Keywords: steelseries,sonar,volume,control,sonar-api
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.1
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
 [![publish](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml/badge.svg?event=push)](https://github.com/Mark7888/steelseries-sonar-py/actions/workflows/publish.yml)
 [![Downloads](https://static.pepy.tech/badge/steelseries-sonar-py)](https://pepy.tech/project/steelseries-sonar-py)
 
 # SteelSeries Sonar Python API
 
+**Streamer mode currently in development!**
+
 ## Overview
 
-This Python package provides a convenient interface for interacting with the SteelSeries Sonar application API. The Sonar application allows users to control and display volumes for various audio channels.
+This Python package provides a convenient interface for interacting with the SteelSeries Sonar application API.    
+The Sonar application allows users to control and display volumes for various audio channels.
 
 ## Installation
 
 To use this package, follow these steps:
 
 1. Install the package using pip:
 
@@ -58,105 +26,160 @@
    from steelseries_sonar_py import Sonar
    ```
 
 ## Usage
 
 ### Initializing the Sonar Object
 
-The Sonar class accepts two optional parameters during initialization:
-`streamer_mode`: Set to True to use streamer mode (default is False).
-`app_data_path`: Specify a custom path for the SteelSeries Engine 3 coreProps.json file (default is the default installation path: `C:\\ProgramData\\SteelSeries\\SteelSeries Engine 3\\coreProps.json`).
+The Sonar class accepts two optional parameters during initialization:   
+`streamer_mode`: Set to True to use streamer mode (default is False).   
+`app_data_path`: Specify a custom path for the SteelSeries Engine 3 coreProps.json file   
+(default is the default installation path: `C:\\ProgramData\\SteelSeries\\SteelSeries Engine 3\\coreProps.json`).
 
 ```python
-sonar = Sonar(streamer_mode=True, app_data_path="C:\\path\\to\\coreProps.json")
+sonar = Sonar(app_data_path="C:\\path\\to\\coreProps.json")
+```
+or
+```python
+sonar = Sonar(app_data_path="C:\\path\\to\\coreProps.json", streamer_mode=True)
+```
+
+### Streamer Mode
+
+The SteelSeries Sonar Python API supports streamer mode, which allows users to manage two separate sliders: `streaming` and `monitoring`. These sliders enable fine-tuned control over different audio channels.
+
+To check if the streamer mode is enabled, use:
+
+```python
+is_streaming = sonar.is_streamer_mode()
+print("Is Streamer Mode:", is_streaming)
+```
+
+To enable or disable streamer mode, use:
+
+```python
+# Enable streamer mode
+sonar.set_streamer_mode(True)
+
+# Disable streamer mode
+sonar.set_streamer_mode(False)
 ```
 
 ### Retrieving Volume Information
 
 Retrieve information about the current volume settings for all channels:
 
 ```python
 volume_data = sonar.get_volume_data()
 print(volume_data)
 ```
 
 ### Setting Volume for a Channel
 
-Set the volume for a specific channel. The `channel` parameter should be one of the following: "master", "game", "chatRender", "media", "aux", "chatCapture". The `volume` parameter should be a float between 0 and 1:
+Set the volume for a specific channel. The `channel` parameter should be one of the following:   
+`master`, `game`, `chatRender`, `media`, `aux`, `chatCapture`. The `volume` parameter should be a float between 0 and 1.   
+Additionally, an optional `streamer_slider` parameter can be provided, with values "streaming" (default) or "monitoring":
 
 ```python
 channel = "master"
 volume = 0.75
+streamer_slider = "streaming"  # or "monitoring"
 
-result = sonar.set_volume(channel, volume)
+result = sonar.set_volume(channel, volume, streamer_slider=streamer_slider)
 print(result)
 ```
 
 ### Muting/Unmuting a Channel
 
-Toggle mute status for a specific channel. The `channel` parameter should be one of the following: `master`, `game`, `chatRender`, `media`, `aux`, `chatCapture`. The `muted` parameter should be a boolean indicating whether to mute (`True`) or unmute (`False`) the channel:
+Toggle mute status for a specific channel. The `channel` parameter should be one of the following:   
+`master`, `game`, `chatRender`, `media`, `aux`, `chatCapture`. The `muted` parameter should be a boolean indicating whether to mute (`True`) or unmute (`False`) the channel.   
+Additionally, an optional `streamer_slider` parameter can be provided, with values "streaming" (default) or "monitoring":
 
 ```python
 channel = "game"
 muted = True
+streamer_slider = "monitoring"
 
-result = sonar.mute_channel(channel, muted)
+result = sonar.mute_channel(channel, muted, streamer_slider=streamer_slider)
 print(result)
 ```
 
 ### Chatmix
 
-Chatmix value between `-1 and 1` to focus sound from the `game` or `chatRender` channel:
+Retrieve chat-mix data:
+
+```python
+chatmix_data = sonar.get_chat_mix_data()
+print(chatmix_data)
+```
+
+Set chat-mix value between `-1 and 1` to focus sound from the `game` or `chatRender` channel:
 
 ```python
-result = sonar.chat_mix(0.5)
+result = sonar.set_chat_mix(0.5)
 print(result)
 ```
 
 ## Exceptions
 
-The package introduces a set of exceptions that might be raised during usage. It is advisable to handle these exceptions accordingly in your code. You can import them from `steelseries_sonar_py.exceptions`. Here is the list of potential exceptions:
+The package introduces a set of exceptions that might be raised during usage.    
+It is advisable to handle these exceptions accordingly in your code.   
+You can import them from `steelseries_sonar_py.exceptions`. Here is the list of potential exceptions:
 
 - `EnginePathNotFoundError`: Raised when SteelSeries Engine 3 is not installed or not in the default location.
 - `ServerNotAccessibleError`: Raised when the SteelSeries server is not accessible. Provides the HTTP status code.
 - `SonarNotEnabledError`: Raised when SteelSeries Sonar is not enabled.
 - `ServerNotReadyError`: Raised when SteelSeries Sonar is not ready.
 - `ServerNotRunningError`: Raised when SteelSeries Sonar is not running.
 - `WebServerAddressNotFoundError`: Raised when the web server address is not found.
 - `ChannelNotFoundError`: Raised when the specified channel is not found.
 - `InvalidVolumeError`: Raised when an invalid volume value is provided.
+- `InvalidMixVolumeError`: Raised when an invalid mix volume value is provided.
+- `SliderNotFoundError`: Raised when an unknown slider name is provided as `streamer_slider` value.
 
 ## Example
 
 Here is a complete example demonstrating the usage of the SteelSeries Sonar Python API:
 
 ```python
 from steelseries_sonar_py import Sonar
 from steelseries_sonar_py.exceptions import EnginePathNotFoundError
 
 # Initialize Sonar object
 try:
-    sonar = Sonar(streamer_mode=False, app_data_path="C:\\path\\to\\coreProps.json")
+    sonar = Sonar(app_data_path="C:\\path\\to\\coreProps.json")
 except EnginePathNotFoundError:
     print("Engine not found!")
     quit()
 
 # Retrieve volume data
 volume_data = sonar.get_volume_data()
 print("Volume Data:", volume_data)
 
 # Set volume for the 'master' channel
 channel = "master"
 volume = 0.8
-result = sonar.set_volume(channel, volume)
+streamer_slider = "streaming"
+result = sonar.set_volume(channel, volume, streamer_slider=streamer_slider)
 print(f"Set volume for {channel}:", result)
 
 # Mute the 'game' channel
 channel = "game"
 muted = True
-result = sonar.mute_channel(channel, muted)
+streamer_slider = "monitoring"
+result = sonar.mute_channel(channel, muted, streamer_slider=streamer_slider)
 print(f"Mute {channel}:", result)
+
+# Retrieve chat-mix data
+chatmix_data = sonar.get_chat_mix_data()
+print("Chatmix Data:", chatmix_data)
+
+# Set chat-mix value
+result = sonar.set_chat_mix(0.5)
+print("Set Chatmix:", result)
 ```
 
 ## Special Thanks
 
-Thanks to two contributors who made this package possible - [wex](https://github.com/wex/sonar-rev) for figuring out the API and [TotalPanther317](https://github.com/TotalPanther317/steelseries-sonar-py) for understanding streamer mode. Grateful for their efforts!
+Thanks to all contributors who made this package possible - [wex](https://github.com/wex/sonar-rev) for figuring out the API, [TotalPanther317](https://github.com/TotalPanther317/steelseries-sonar-py) for understanding streamer mode and [cookie](https://github.com/cookie0o) for features like chat mix and streamer mode detection. Grateful for their efforts!
+
+This documentation now reflects the latest changes and additions to the SteelSeries Sonar Python API.
```

### Comparing `steelseries_sonar_py-1.1.1/setup.py` & `steelseries_sonar_py-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `steelseries_sonar_py-1.1.1/src/steelseries_sonar_py/exceptions.py` & `steelseries_sonar_py-1.2.0/src/steelseries_sonar_py/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,21 +34,28 @@
 class ChannelNotFoundError(Exception):
     def __init__(self, channel):
         self.channel = channel
 
     def __str__(self):
         return f"Channel '{self.channel}' not found"
 
+class SliderNotFoundError(Exception):
+    def __init__(self, slider):
+        self.slider = slider
+
+    def __str__(self):
+        return f"Slider '{self.slider}' not found"
+
 
 class InvalidVolumeError(Exception):
     def __init__(self, volume):
         self.volume = volume
 
     def __str__(self):
         return f"Invalid volume '{self.volume}'! Value must be between 0 and 1!"
 
 class InvalidMixVolumeError(Exception):
     def __init__(self, mix_volume):
         self.mix_volume = mix_volume
 
     def __str__(self):
-        return f"Invalid mix volume '{self.mix_volume}'! Value must be between -1 and 1!"
+        return f"Invalid mix volume '{self.mix_volume}'! Value must be between -1 and 1!"
```

