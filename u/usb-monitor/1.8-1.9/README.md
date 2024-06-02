# Comparing `tmp/usb-monitor-1.8.tar.gz` & `tmp/usb-monitor-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usb-monitor-1.8.tar", last modified: Fri Mar 31 21:33:03 2023, max compression
+gzip compressed data, was "usb-monitor-1.9.tar", last modified: Sat Apr  1 23:40:39 2023, max compression
```

## Comparing `usb-monitor-1.8.tar` & `usb-monitor-1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 21:33:03.937516 usb-monitor-1.8/
--rw-rw-rw-   0        0        0     1089 2023-03-24 16:59:27.000000 usb-monitor-1.8/LICENSE
--rw-rw-rw-   0        0        0     9134 2023-03-31 21:33:03.937516 usb-monitor-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     7745 2023-03-31 10:20:52.000000 usb-monitor-1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-03-31 21:33:03.937516 usb-monitor-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1739 2023-03-31 21:32:59.000000 usb-monitor-1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 21:33:03.921890 usb-monitor-1.8/usb_monitor.egg-info/
--rw-rw-rw-   0        0        0     9134 2023-03-31 21:33:03.000000 usb-monitor-1.8/usb_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      574 2023-03-31 21:33:03.000000 usb-monitor-1.8/usb_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 21:33:03.000000 usb-monitor-1.8/usb_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-03-31 21:33:03.000000 usb-monitor-1.8/usb_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-31 21:33:03.000000 usb-monitor-1.8/usb_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-31 21:33:03.937516 usb-monitor-1.8/usbmonitor/
--rw-rw-rw-   0        0        0      244 2023-03-28 10:21:11.000000 usb-monitor-1.8/usbmonitor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 21:33:03.937516 usb-monitor-1.8/usbmonitor/__platform_specific_detectors/
--rw-rw-rw-   0        0        0        0 2023-03-28 10:02:06.000000 usb-monitor-1.8/usbmonitor/__platform_specific_detectors/__init__.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 10:20:59.000000 usb-monitor-1.8/usbmonitor/__platform_specific_detectors/_constants.py
--rw-rw-rw-   0        0        0     4356 2023-03-29 21:29:52.000000 usb-monitor-1.8/usbmonitor/__platform_specific_detectors/_linux_usb_detector.py
--rw-rw-rw-   0        0        0     8243 2023-03-28 13:14:44.000000 usb-monitor-1.8/usbmonitor/__platform_specific_detectors/_usb_detector_base.py
--rw-rw-rw-   0        0        0     6262 2023-03-30 09:58:02.000000 usb-monitor-1.8/usbmonitor/__platform_specific_detectors/_windows_usb_detector.py
--rw-rw-rw-   0        0        0     1103 2023-03-29 22:02:05.000000 usb-monitor-1.8/usbmonitor/attributes.py
--rw-rw-rw-   0        0        0     6048 2023-03-28 12:45:12.000000 usb-monitor-1.8/usbmonitor/usbmonitor.py
+drwxrwxrwx   0        0        0        0 2023-04-01 23:40:39.178976 usb-monitor-1.9/
+-rw-rw-rw-   0        0        0     1089 2023-03-24 16:59:27.000000 usb-monitor-1.9/LICENSE
+-rw-rw-rw-   0        0        0    11117 2023-04-01 23:40:39.178976 usb-monitor-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9728 2023-04-01 23:38:15.000000 usb-monitor-1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-01 23:40:39.178976 usb-monitor-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1739 2023-04-01 23:40:30.000000 usb-monitor-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-01 23:40:39.083540 usb-monitor-1.9/usb_monitor.egg-info/
+-rw-rw-rw-   0        0        0    11117 2023-04-01 23:40:38.000000 usb-monitor-1.9/usb_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2023-04-01 23:40:38.000000 usb-monitor-1.9/usb_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-01 23:40:38.000000 usb-monitor-1.9/usb_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-04-01 23:40:38.000000 usb-monitor-1.9/usb_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-01 23:40:38.000000 usb-monitor-1.9/usb_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-01 23:40:39.126400 usb-monitor-1.9/usbmonitor/
+-rw-rw-rw-   0        0        0      244 2023-03-28 10:21:11.000000 usb-monitor-1.9/usbmonitor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-01 23:40:39.178976 usb-monitor-1.9/usbmonitor/__platform_specific_detectors/
+-rw-rw-rw-   0        0        0        0 2023-03-28 10:02:06.000000 usb-monitor-1.9/usbmonitor/__platform_specific_detectors/__init__.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 10:20:59.000000 usb-monitor-1.9/usbmonitor/__platform_specific_detectors/_constants.py
+-rw-rw-rw-   0        0        0     4356 2023-03-29 21:29:52.000000 usb-monitor-1.9/usbmonitor/__platform_specific_detectors/_linux_usb_detector.py
+-rw-rw-rw-   0        0        0     8243 2023-03-28 13:14:44.000000 usb-monitor-1.9/usbmonitor/__platform_specific_detectors/_usb_detector_base.py
+-rw-rw-rw-   0        0        0     6262 2023-03-30 09:58:02.000000 usb-monitor-1.9/usbmonitor/__platform_specific_detectors/_windows_usb_detector.py
+-rw-rw-rw-   0        0        0     1103 2023-03-29 22:02:05.000000 usb-monitor-1.9/usbmonitor/attributes.py
+-rw-rw-rw-   0        0        0     6048 2023-03-28 12:45:12.000000 usb-monitor-1.9/usbmonitor/usbmonitor.py
```

### Comparing `usb-monitor-1.8/LICENSE` & `usb-monitor-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `usb-monitor-1.8/PKG-INFO` & `usb-monitor-1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usb-monitor
-Version: 1.8
+Version: 1.9
 Summary: USBMonitor is an easy-to-use cross-platform library for USB device monitoring that simplifies tracking of connections, disconnections, and examination of connected device attributes on both Windows and Linux, freeing the user from platform-specific details or incompatibilities.
 Home-page: https://github.com/Eric-Canas/USBMonitor
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -60,51 +60,95 @@
 monitor.start_monitoring(on_connect=on_connect, on_disconnect=on_disconnect)
 
 # ... Rest of your code ...
 
 # If you don't need it anymore stop the daemon
 monitor.stop_monitoring()
 ```
+Output
 Linux | Windows
 :---: | :---:
 ![](https://raw.githubusercontent.com/Eric-Canas/USBMonitor/main/resources/linux_monitor.gif) | ![](https://raw.githubusercontent.com/Eric-Canas/USBMonitor/main/resources/windows_monitor.gif)
 
+Sometimes, when initializing your software, you may seek to confirm which USB devices are indeed connected. 
+
+```python
+from usbmonitor import USBMonitor
+from usbmonitor.attributes import ID_MODEL, ID_MODEL_ID, ID_VENDOR_ID
+
+# Create the USBMonitor instance
+monitor = USBMonitor()
+
+# Get the current devices
+devices_dict = monitor.get_current_available_devices()
+
+# Print them
+for device_id, device_info in devices_dict.items():
+    print(f"{device_id} -- {device_info[ID_MODEL]} ({device_info[ID_MODEL_ID]} - {device_info[ID_VENDOR_ID]})")
+```
+Output
+```bash
+/dev/bus/usb/001/001 -- xHCI_Host_Controller (0002 - 1d6b)
+/dev/bus/usb/001/002 -- USB2.0_Hub (3431 - 2109)
+/dev/bus/usb/001/003 -- USB_Optical_Mouse (c077 - 046d)
+/dev/bus/usb/001/004 -- USB_Compliant_Keypad (9881 - 05a4)
+/dev/bus/usb/002/001 -- xHCI_Host_Controller (0003 - 1d6b)
+```
+
+
 
 ## API Reference
 
 ### USBMonitor.start_monitoring(on_connect = None, on_disconnect = None, check_every_seconds = 0.5)
-Starts a daemon that continuously monitors the connected USB devices in order to detect new connections or disconnections. When a device is disconnected, the `on_disconnect` callback function is invoked with the Device ID as the first argument and the dictionary of device information as the second argument. Similarly, when a new device is connected, the `on_connect` callback function is called with the same arguments. This allows developers to promptly respond to any changes in the connected USB devices and perform necessary actions.
+Starts a daemon that continuously monitors the connected USB devices in order to detect new connections or disconnections. When a device is disconnected, the `on_disconnect` callback function is invoked with the Device ID as the first argument and the [dictionary of device information](#device-properties) as the second argument. Similarly, when a new device is connected, the `on_connect` callback function is called with the same arguments. This allows developers to promptly respond to any changes in the connected USB devices and perform necessary actions.
 
 - `on_connect`: **callable | None**. The function to call every time a device is **added**. It is expected to have the following format `on_connect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `on_disconnect`: **callable | None**. The function to call every time a device is **removed**. It is expected to have the following format `on_disconnect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `check_every_seconds`: **int | float**. Seconds to wait between each check for changes in the USB devices. Default value is 0.5 seconds.
 
 ### USBMonitor.stop_monitoring(warn_if_was_stopped=True)
 Stops the monitoring of USB devices. This function will **stop** the daemon launched by `USBMonitor.start_monitoring`
 
 - `warn_if_was_stopped`: **bool**. If set to `True`, this function will issue a warning if the monitoring of USB devices was already stopped (the daemon was not running).
 
 
 ### USBMonitor.get_current_available_devices()
-Returns a dictionary of the currently available devices, where the key is the `Device ID` and the value is a dictionary containing the device's information. All the keys of this dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They always correspond with the default Linux device properties (independently of the OS where the library is running).
+Returns a dictionary of the currently available devices, where the key is the `Device ID` and the value is a [dictionary containing the device's information](#device-properties). All the keys of this dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They always correspond with the default Linux device properties (independently of the OS where the library is running).
 
 - Returns: **dict[str, dict[str, str|tuple[str, ...]]]**: A dictionary containing the currently available devices. All values are strings except for `ID_USB_INTERFACES`, which is a `tuple` of `string`
 
 
 
 ### USBMonitor.changes_from_last_check(update_last_check_devices = True)
-Returns a tuple of two dictionaries, one containing the devices that have been *removed* since the last check, and another one containing the devices that have been *added*. Both dictionaries will have the `Device ID` as key and all the device information as value. Remember that all the keys of this dictionary can be found at can be found at `attributes.DEVICE_ATTRIBUTES`.
+Returns a tuple of two dictionaries, one containing the devices that have been *removed* since the last check, and another one containing the devices that have been *added*. Both dictionaries will have the `Device ID` as key and all the device information as value. Remember that all the [keys of this dictionary](#device-properties) can be found at can be found at `attributes.DEVICE_ATTRIBUTES`.
 
 - `update_last_check_devices`: **bool**. If `True` it will update the internal `USBMonitor.last_check_devices` attribute. So the next time you'll call this method, it will check for differences against the devices found in that current call. If `False` it won't update the `USBMonitor.last_check_devices` attribute. 
 
 - Returns: **tuple[dict[str, dict[str, str|tuple[str, ...]]], dict[str, dict[str, str|tuple[str, ...]]]]**: A `tuple` containing two `dictionaries`. The first `dictionary` contains the information of the devices that were **removed** since the last check and the second dictionary contains the information of the new **added** devices. All values are `strings` except for `ID_USB_INTERFACES`, which is a `tuple` of `string`.
 
 ### USBMonitor.check_changes(on_connect = None, on_disconnect = None, update_last_check_devices = True)
-Checks for any new connections or disconnections of USB devices since the last check. If a device has been removed, the `on_disconnect` function will be called with the `Device ID` as the first argument and the dictionary of device information as the second argument. The same will occur with the `on_connect` function if any new device have been added. Internally this function will just run `USBMonitor.changes_from_last_check` and will execute the callbacks for each returned device
+Checks for any new connections or disconnections of USB devices since the last check. If a device has been removed, the `on_disconnect` function will be called with the `Device ID` as the first argument and the [dictionary with the device's information](#device-properties) as the second argument. The same will occur with the `on_connect` function if any new device have been added. Internally this function will just run `USBMonitor.changes_from_last_check` and will execute the callbacks for each returned device
 
 - `on_connect`: **callable | None**. The function to call when a device is added. It is expected to have the following format `on_connect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `on_disconnect`: **callable | None**. The function to call when a device is removed. It is expected to have the following format `on_disconnect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `update_last_check_devices`: **bool**. If `True` it will update the internal `USBMonitor.last_check_devices` attribute. So the next time you'll call this method, it will check for differences against the devices found in that current call. If `False` it won't update the `USBMonitor.last_check_devices` attribute. 
 
 ### Device Properties
 
+The `device_info` returned by most functions will contain the following information:
+
+Key | Value Description | Example
+:-- | :-- | :--
+`'ID_MODEL_ID'` | The product ID of the USB device. | `'0892'`
+`'ID_MODEL'` | The name of the USB device model. | `'HD_Pro_Webcam_C920'`
+`'ID_MODEL_FROM_DATABASE'` | Device model name, retrieved from the device database.| `'OrbiCam'`
+`'ID_VENDOR'` | The name of the USB device vendor | `'046d'`
+`'ID_VENDOR_ID'` | The vendor ID of the USB device. | `'046d'`
+`'ID_VENDOR_FROM_DATABASE'` | USB device vendor's name, from the device database. | `'Logitech, Inc.'`
+`'DEVNAME'` | The device name or path  | `'/dev/bus/usb/001/003'`
+`'ID_USB_INTERFACES'` |	A `tuple` representing the USB device's interfaces. | `('0e0100', '0e0200', '010100', '010200')`
+`'DEVTYPE'` | Should always be `'usb_device'`. | `'usb_device'`
+
+Note that, depending on the device and the OS, some of this information may be incomplete or certain attributes may overlap with others.
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usb-monitor Version: 1.8 Summary: USBMonitor is an
+Metadata-Version: 2.1 Name: usb-monitor Version: 1.9 Summary: USBMonitor is an
 easy-to-use cross-platform library for USB device monitoring that simplifies
 tracking of connections, disconnections, and examination of connected device
 attributes on both Windows and Linux, freeing the user from platform-specific
 details or incompatibilities. Home-page: https://github.com/Eric-Canas/
 USBMonitor Author: Eric-Canas Author-email: eric@ericcanas.com License: MIT
 Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
@@ -43,52 +43,65 @@
 [ID_MODEL_ID]} - {device_info[ID_VENDOR_ID]})" # Define the `on_connect` and
 `on_disconnect` callbacks on_connect = lambda device_id, device_info: print
 (f"Connected: {device_info_str(device_info=device_info)}") on_disconnect =
 lambda device_id, device_info: print(f"Disconnected: {device_info_str
 (device_info=device_info)}") # Create the USBMonitor instance monitor =
 USBMonitor() # Start the daemon monitor.start_monitoring(on_connect=on_connect,
 on_disconnect=on_disconnect) # ... Rest of your code ... # If you don't need it
-anymore stop the daemon monitor.stop_monitoring() ``` Linux | Windows :---: | :
----: ![](https://raw.githubusercontent.com/Eric-Canas/USBMonitor/main/
+anymore stop the daemon monitor.stop_monitoring() ``` Output Linux | Windows :-
+--: | :---: ![](https://raw.githubusercontent.com/Eric-Canas/USBMonitor/main/
 resources/linux_monitor.gif) | ![](https://raw.githubusercontent.com/Eric-
-Canas/USBMonitor/main/resources/windows_monitor.gif) ## API Reference ###
+Canas/USBMonitor/main/resources/windows_monitor.gif) Sometimes, when
+initializing your software, you may seek to confirm which USB devices are
+indeed connected. ```python from usbmonitor import USBMonitor from
+usbmonitor.attributes import ID_MODEL, ID_MODEL_ID, ID_VENDOR_ID # Create the
+USBMonitor instance monitor = USBMonitor() # Get the current devices
+devices_dict = monitor.get_current_available_devices() # Print them for
+device_id, device_info in devices_dict.items(): print(f"{device_id} --
+{device_info[ID_MODEL]} ({device_info[ID_MODEL_ID]} - {device_info
+[ID_VENDOR_ID]})") ``` Output ```bash /dev/bus/usb/001/001 -
+- xHCI_Host_Controller (0002 - 1d6b) /dev/bus/usb/001/002 -- USB2.0_Hub (3431 -
+2109) /dev/bus/usb/001/003 -- USB_Optical_Mouse (c077 - 046d) /dev/bus/usb/001/
+004 -- USB_Compliant_Keypad (9881 - 05a4) /dev/bus/usb/002/001 -
+- xHCI_Host_Controller (0003 - 1d6b) ``` ## API Reference ###
 USBMonitor.start_monitoring(on_connect = None, on_disconnect = None,
 check_every_seconds = 0.5) Starts a daemon that continuously monitors the
 connected USB devices in order to detect new connections or disconnections.
 When a device is disconnected, the `on_disconnect` callback function is invoked
-with the Device ID as the first argument and the dictionary of device
-information as the second argument. Similarly, when a new device is connected,
-the `on_connect` callback function is called with the same arguments. This
-allows developers to promptly respond to any changes in the connected USB
-devices and perform necessary actions. - `on_connect`: **callable | None**. The
-function to call every time a device is **added**. It is expected to have the
-following format `on_connect(device_id: str, device_info: dict[str, dict[str,
-str|tuple[str, ...]]])` - `on_disconnect`: **callable | None**. The function to
-call every time a device is **removed**. It is expected to have the following
-format `on_disconnect(device_id: str, device_info: dict[str, dict[str,
-str|tuple[str, ...]]])` - `check_every_seconds`: **int | float**. Seconds to
-wait between each check for changes in the USB devices. Default value is 0.5
+with the Device ID as the first argument and the [dictionary of device
+information](#device-properties) as the second argument. Similarly, when a new
+device is connected, the `on_connect` callback function is called with the same
+arguments. This allows developers to promptly respond to any changes in the
+connected USB devices and perform necessary actions. - `on_connect`: **callable
+| None**. The function to call every time a device is **added**. It is expected
+to have the following format `on_connect(device_id: str, device_info: dict[str,
+dict[str, str|tuple[str, ...]]])` - `on_disconnect`: **callable | None**. The
+function to call every time a device is **removed**. It is expected to have the
+following format `on_disconnect(device_id: str, device_info: dict[str, dict
+[str, str|tuple[str, ...]]])` - `check_every_seconds`: **int | float**. Seconds
+to wait between each check for changes in the USB devices. Default value is 0.5
 seconds. ### USBMonitor.stop_monitoring(warn_if_was_stopped=True) Stops the
 monitoring of USB devices. This function will **stop** the daemon launched by
 `USBMonitor.start_monitoring` - `warn_if_was_stopped`: **bool**. If set to
 `True`, this function will issue a warning if the monitoring of USB devices was
 already stopped (the daemon was not running). ###
 USBMonitor.get_current_available_devices() Returns a dictionary of the
 currently available devices, where the key is the `Device ID` and the value is
-a dictionary containing the device's information. All the keys of this
-dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They always
-correspond with the default Linux device properties (independently of the OS
-where the library is running). - Returns: **dict[str, dict[str, str|tuple[str,
-...]]]**: A dictionary containing the currently available devices. All values
-are strings except for `ID_USB_INTERFACES`, which is a `tuple` of `string` ###
-USBMonitor.changes_from_last_check(update_last_check_devices = True) Returns a
-tuple of two dictionaries, one containing the devices that have been *removed*
-since the last check, and another one containing the devices that have been
-*added*. Both dictionaries will have the `Device ID` as key and all the device
-information as value. Remember that all the keys of this dictionary can be
+a [dictionary containing the device's information](#device-properties). All the
+keys of this dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They
+always correspond with the default Linux device properties (independently of
+the OS where the library is running). - Returns: **dict[str, dict[str,
+str|tuple[str, ...]]]**: A dictionary containing the currently available
+devices. All values are strings except for `ID_USB_INTERFACES`, which is a
+`tuple` of `string` ### USBMonitor.changes_from_last_check
+(update_last_check_devices = True) Returns a tuple of two dictionaries, one
+containing the devices that have been *removed* since the last check, and
+another one containing the devices that have been *added*. Both dictionaries
+will have the `Device ID` as key and all the device information as value.
+Remember that all the [keys of this dictionary](#device-properties) can be
 found at can be found at `attributes.DEVICE_ATTRIBUTES`. -
 `update_last_check_devices`: **bool**. If `True` it will update the internal
 `USBMonitor.last_check_devices` attribute. So the next time you'll call this
 method, it will check for differences against the devices found in that current
 call. If `False` it won't update the `USBMonitor.last_check_devices` attribute.
 - Returns: **tuple[dict[str, dict[str, str|tuple[str, ...]]], dict[str, dict
 [str, str|tuple[str, ...]]]]**: A `tuple` containing two `dictionaries`. The
@@ -96,22 +109,35 @@
 **removed** since the last check and the second dictionary contains the
 information of the new **added** devices. All values are `strings` except for
 `ID_USB_INTERFACES`, which is a `tuple` of `string`. ###
 USBMonitor.check_changes(on_connect = None, on_disconnect = None,
 update_last_check_devices = True) Checks for any new connections or
 disconnections of USB devices since the last check. If a device has been
 removed, the `on_disconnect` function will be called with the `Device ID` as
-the first argument and the dictionary of device information as the second
-argument. The same will occur with the `on_connect` function if any new device
-have been added. Internally this function will just run
-`USBMonitor.changes_from_last_check` and will execute the callbacks for each
-returned device - `on_connect`: **callable | None**. The function to call when
-a device is added. It is expected to have the following format `on_connect
+the first argument and the [dictionary with the device's information](#device-
+properties) as the second argument. The same will occur with the `on_connect`
+function if any new device have been added. Internally this function will just
+run `USBMonitor.changes_from_last_check` and will execute the callbacks for
+each returned device - `on_connect`: **callable | None**. The function to call
+when a device is added. It is expected to have the following format `on_connect
 (device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])` -
 `on_disconnect`: **callable | None**. The function to call when a device is
 removed. It is expected to have the following format `on_disconnect(device_id:
 str, device_info: dict[str, dict[str, str|tuple[str, ...]]])` -
 `update_last_check_devices`: **bool**. If `True` it will update the internal
 `USBMonitor.last_check_devices` attribute. So the next time you'll call this
 method, it will check for differences against the devices found in that current
 call. If `False` it won't update the `USBMonitor.last_check_devices` attribute.
-### Device Properties
+### Device Properties The `device_info` returned by most functions will contain
+the following information: Key | Value Description | Example :-- | :-- | :-
+- `'ID_MODEL_ID'` | The product ID of the USB device. | `'0892'` `'ID_MODEL'` |
+The name of the USB device model. | `'HD_Pro_Webcam_C920'`
+`'ID_MODEL_FROM_DATABASE'` | Device model name, retrieved from the device
+database.| `'OrbiCam'` `'ID_VENDOR'` | The name of the USB device vendor |
+`'046d'` `'ID_VENDOR_ID'` | The vendor ID of the USB device. | `'046d'`
+`'ID_VENDOR_FROM_DATABASE'` | USB device vendor's name, from the device
+database. | `'Logitech, Inc.'` `'DEVNAME'` | The device name or path | `'/dev/
+bus/usb/001/003'` `'ID_USB_INTERFACES'` | A `tuple` representing the USB
+device's interfaces. | `('0e0100', '0e0200', '010100', '010200')` `'DEVTYPE'` |
+Should always be `'usb_device'`. | `'usb_device'` Note that, depending on the
+device and the OS, some of this information may be incomplete or certain
+attributes may overlap with others.
```

### Comparing `usb-monitor-1.8/README.md` & `usb-monitor-1.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -31,49 +31,93 @@
 monitor.start_monitoring(on_connect=on_connect, on_disconnect=on_disconnect)
 
 # ... Rest of your code ...
 
 # If you don't need it anymore stop the daemon
 monitor.stop_monitoring()
 ```
+Output
 Linux | Windows
 :---: | :---:
 ![](https://raw.githubusercontent.com/Eric-Canas/USBMonitor/main/resources/linux_monitor.gif) | ![](https://raw.githubusercontent.com/Eric-Canas/USBMonitor/main/resources/windows_monitor.gif)
 
+Sometimes, when initializing your software, you may seek to confirm which USB devices are indeed connected. 
+
+```python
+from usbmonitor import USBMonitor
+from usbmonitor.attributes import ID_MODEL, ID_MODEL_ID, ID_VENDOR_ID
+
+# Create the USBMonitor instance
+monitor = USBMonitor()
+
+# Get the current devices
+devices_dict = monitor.get_current_available_devices()
+
+# Print them
+for device_id, device_info in devices_dict.items():
+    print(f"{device_id} -- {device_info[ID_MODEL]} ({device_info[ID_MODEL_ID]} - {device_info[ID_VENDOR_ID]})")
+```
+Output
+```bash
+/dev/bus/usb/001/001 -- xHCI_Host_Controller (0002 - 1d6b)
+/dev/bus/usb/001/002 -- USB2.0_Hub (3431 - 2109)
+/dev/bus/usb/001/003 -- USB_Optical_Mouse (c077 - 046d)
+/dev/bus/usb/001/004 -- USB_Compliant_Keypad (9881 - 05a4)
+/dev/bus/usb/002/001 -- xHCI_Host_Controller (0003 - 1d6b)
+```
+
+
 
 ## API Reference
 
 ### USBMonitor.start_monitoring(on_connect = None, on_disconnect = None, check_every_seconds = 0.5)
-Starts a daemon that continuously monitors the connected USB devices in order to detect new connections or disconnections. When a device is disconnected, the `on_disconnect` callback function is invoked with the Device ID as the first argument and the dictionary of device information as the second argument. Similarly, when a new device is connected, the `on_connect` callback function is called with the same arguments. This allows developers to promptly respond to any changes in the connected USB devices and perform necessary actions.
+Starts a daemon that continuously monitors the connected USB devices in order to detect new connections or disconnections. When a device is disconnected, the `on_disconnect` callback function is invoked with the Device ID as the first argument and the [dictionary of device information](#device-properties) as the second argument. Similarly, when a new device is connected, the `on_connect` callback function is called with the same arguments. This allows developers to promptly respond to any changes in the connected USB devices and perform necessary actions.
 
 - `on_connect`: **callable | None**. The function to call every time a device is **added**. It is expected to have the following format `on_connect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `on_disconnect`: **callable | None**. The function to call every time a device is **removed**. It is expected to have the following format `on_disconnect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `check_every_seconds`: **int | float**. Seconds to wait between each check for changes in the USB devices. Default value is 0.5 seconds.
 
 ### USBMonitor.stop_monitoring(warn_if_was_stopped=True)
 Stops the monitoring of USB devices. This function will **stop** the daemon launched by `USBMonitor.start_monitoring`
 
 - `warn_if_was_stopped`: **bool**. If set to `True`, this function will issue a warning if the monitoring of USB devices was already stopped (the daemon was not running).
 
 
 ### USBMonitor.get_current_available_devices()
-Returns a dictionary of the currently available devices, where the key is the `Device ID` and the value is a dictionary containing the device's information. All the keys of this dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They always correspond with the default Linux device properties (independently of the OS where the library is running).
+Returns a dictionary of the currently available devices, where the key is the `Device ID` and the value is a [dictionary containing the device's information](#device-properties). All the keys of this dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They always correspond with the default Linux device properties (independently of the OS where the library is running).
 
 - Returns: **dict[str, dict[str, str|tuple[str, ...]]]**: A dictionary containing the currently available devices. All values are strings except for `ID_USB_INTERFACES`, which is a `tuple` of `string`
 
 
 
 ### USBMonitor.changes_from_last_check(update_last_check_devices = True)
-Returns a tuple of two dictionaries, one containing the devices that have been *removed* since the last check, and another one containing the devices that have been *added*. Both dictionaries will have the `Device ID` as key and all the device information as value. Remember that all the keys of this dictionary can be found at can be found at `attributes.DEVICE_ATTRIBUTES`.
+Returns a tuple of two dictionaries, one containing the devices that have been *removed* since the last check, and another one containing the devices that have been *added*. Both dictionaries will have the `Device ID` as key and all the device information as value. Remember that all the [keys of this dictionary](#device-properties) can be found at can be found at `attributes.DEVICE_ATTRIBUTES`.
 
 - `update_last_check_devices`: **bool**. If `True` it will update the internal `USBMonitor.last_check_devices` attribute. So the next time you'll call this method, it will check for differences against the devices found in that current call. If `False` it won't update the `USBMonitor.last_check_devices` attribute. 
 
 - Returns: **tuple[dict[str, dict[str, str|tuple[str, ...]]], dict[str, dict[str, str|tuple[str, ...]]]]**: A `tuple` containing two `dictionaries`. The first `dictionary` contains the information of the devices that were **removed** since the last check and the second dictionary contains the information of the new **added** devices. All values are `strings` except for `ID_USB_INTERFACES`, which is a `tuple` of `string`.
 
 ### USBMonitor.check_changes(on_connect = None, on_disconnect = None, update_last_check_devices = True)
-Checks for any new connections or disconnections of USB devices since the last check. If a device has been removed, the `on_disconnect` function will be called with the `Device ID` as the first argument and the dictionary of device information as the second argument. The same will occur with the `on_connect` function if any new device have been added. Internally this function will just run `USBMonitor.changes_from_last_check` and will execute the callbacks for each returned device
+Checks for any new connections or disconnections of USB devices since the last check. If a device has been removed, the `on_disconnect` function will be called with the `Device ID` as the first argument and the [dictionary with the device's information](#device-properties) as the second argument. The same will occur with the `on_connect` function if any new device have been added. Internally this function will just run `USBMonitor.changes_from_last_check` and will execute the callbacks for each returned device
 
 - `on_connect`: **callable | None**. The function to call when a device is added. It is expected to have the following format `on_connect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `on_disconnect`: **callable | None**. The function to call when a device is removed. It is expected to have the following format `on_disconnect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `update_last_check_devices`: **bool**. If `True` it will update the internal `USBMonitor.last_check_devices` attribute. So the next time you'll call this method, it will check for differences against the devices found in that current call. If `False` it won't update the `USBMonitor.last_check_devices` attribute. 
 
 ### Device Properties
+
+The `device_info` returned by most functions will contain the following information:
+
+Key | Value Description | Example
+:-- | :-- | :--
+`'ID_MODEL_ID'` | The product ID of the USB device. | `'0892'`
+`'ID_MODEL'` | The name of the USB device model. | `'HD_Pro_Webcam_C920'`
+`'ID_MODEL_FROM_DATABASE'` | Device model name, retrieved from the device database.| `'OrbiCam'`
+`'ID_VENDOR'` | The name of the USB device vendor | `'046d'`
+`'ID_VENDOR_ID'` | The vendor ID of the USB device. | `'046d'`
+`'ID_VENDOR_FROM_DATABASE'` | USB device vendor's name, from the device database. | `'Logitech, Inc.'`
+`'DEVNAME'` | The device name or path  | `'/dev/bus/usb/001/003'`
+`'ID_USB_INTERFACES'` |	A `tuple` representing the USB device's interfaces. | `('0e0100', '0e0200', '010100', '010200')`
+`'DEVTYPE'` | Should always be `'usb_device'`. | `'usb_device'`
+
+Note that, depending on the device and the OS, some of this information may be incomplete or certain attributes may overlap with others.
+
```

#### html2text {}

```diff
@@ -26,52 +26,64 @@
 `on_connect` and `on_disconnect` callbacks on_connect = lambda device_id,
 device_info: print(f"Connected: {device_info_str(device_info=device_info)}")
 on_disconnect = lambda device_id, device_info: print(f"Disconnected:
 {device_info_str(device_info=device_info)}") # Create the USBMonitor instance
 monitor = USBMonitor() # Start the daemon monitor.start_monitoring
 (on_connect=on_connect, on_disconnect=on_disconnect) # ... Rest of your code
 ... # If you don't need it anymore stop the daemon monitor.stop_monitoring()
-``` Linux | Windows :---: | :---: ![](https://raw.githubusercontent.com/Eric-
-Canas/USBMonitor/main/resources/linux_monitor.gif) | ![](https://
+``` Output Linux | Windows :---: | :---: ![](https://raw.githubusercontent.com/
+Eric-Canas/USBMonitor/main/resources/linux_monitor.gif) | ![](https://
 raw.githubusercontent.com/Eric-Canas/USBMonitor/main/resources/
-windows_monitor.gif) ## API Reference ### USBMonitor.start_monitoring
-(on_connect = None, on_disconnect = None, check_every_seconds = 0.5) Starts a
-daemon that continuously monitors the connected USB devices in order to detect
-new connections or disconnections. When a device is disconnected, the
-`on_disconnect` callback function is invoked with the Device ID as the first
-argument and the dictionary of device information as the second argument.
-Similarly, when a new device is connected, the `on_connect` callback function
-is called with the same arguments. This allows developers to promptly respond
-to any changes in the connected USB devices and perform necessary actions. -
-`on_connect`: **callable | None**. The function to call every time a device is
-**added**. It is expected to have the following format `on_connect(device_id:
-str, device_info: dict[str, dict[str, str|tuple[str, ...]]])` -
-`on_disconnect`: **callable | None**. The function to call every time a device
-is **removed**. It is expected to have the following format `on_disconnect
-(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])` -
-`check_every_seconds`: **int | float**. Seconds to wait between each check for
-changes in the USB devices. Default value is 0.5 seconds. ###
-USBMonitor.stop_monitoring(warn_if_was_stopped=True) Stops the monitoring of
-USB devices. This function will **stop** the daemon launched by
+windows_monitor.gif) Sometimes, when initializing your software, you may seek
+to confirm which USB devices are indeed connected. ```python from usbmonitor
+import USBMonitor from usbmonitor.attributes import ID_MODEL, ID_MODEL_ID,
+ID_VENDOR_ID # Create the USBMonitor instance monitor = USBMonitor() # Get the
+current devices devices_dict = monitor.get_current_available_devices() # Print
+them for device_id, device_info in devices_dict.items(): print(f"{device_id} -
+- {device_info[ID_MODEL]} ({device_info[ID_MODEL_ID]} - {device_info
+[ID_VENDOR_ID]})") ``` Output ```bash /dev/bus/usb/001/001 -
+- xHCI_Host_Controller (0002 - 1d6b) /dev/bus/usb/001/002 -- USB2.0_Hub (3431 -
+2109) /dev/bus/usb/001/003 -- USB_Optical_Mouse (c077 - 046d) /dev/bus/usb/001/
+004 -- USB_Compliant_Keypad (9881 - 05a4) /dev/bus/usb/002/001 -
+- xHCI_Host_Controller (0003 - 1d6b) ``` ## API Reference ###
+USBMonitor.start_monitoring(on_connect = None, on_disconnect = None,
+check_every_seconds = 0.5) Starts a daemon that continuously monitors the
+connected USB devices in order to detect new connections or disconnections.
+When a device is disconnected, the `on_disconnect` callback function is invoked
+with the Device ID as the first argument and the [dictionary of device
+information](#device-properties) as the second argument. Similarly, when a new
+device is connected, the `on_connect` callback function is called with the same
+arguments. This allows developers to promptly respond to any changes in the
+connected USB devices and perform necessary actions. - `on_connect`: **callable
+| None**. The function to call every time a device is **added**. It is expected
+to have the following format `on_connect(device_id: str, device_info: dict[str,
+dict[str, str|tuple[str, ...]]])` - `on_disconnect`: **callable | None**. The
+function to call every time a device is **removed**. It is expected to have the
+following format `on_disconnect(device_id: str, device_info: dict[str, dict
+[str, str|tuple[str, ...]]])` - `check_every_seconds`: **int | float**. Seconds
+to wait between each check for changes in the USB devices. Default value is 0.5
+seconds. ### USBMonitor.stop_monitoring(warn_if_was_stopped=True) Stops the
+monitoring of USB devices. This function will **stop** the daemon launched by
 `USBMonitor.start_monitoring` - `warn_if_was_stopped`: **bool**. If set to
 `True`, this function will issue a warning if the monitoring of USB devices was
 already stopped (the daemon was not running). ###
 USBMonitor.get_current_available_devices() Returns a dictionary of the
 currently available devices, where the key is the `Device ID` and the value is
-a dictionary containing the device's information. All the keys of this
-dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They always
-correspond with the default Linux device properties (independently of the OS
-where the library is running). - Returns: **dict[str, dict[str, str|tuple[str,
-...]]]**: A dictionary containing the currently available devices. All values
-are strings except for `ID_USB_INTERFACES`, which is a `tuple` of `string` ###
-USBMonitor.changes_from_last_check(update_last_check_devices = True) Returns a
-tuple of two dictionaries, one containing the devices that have been *removed*
-since the last check, and another one containing the devices that have been
-*added*. Both dictionaries will have the `Device ID` as key and all the device
-information as value. Remember that all the keys of this dictionary can be
+a [dictionary containing the device's information](#device-properties). All the
+keys of this dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They
+always correspond with the default Linux device properties (independently of
+the OS where the library is running). - Returns: **dict[str, dict[str,
+str|tuple[str, ...]]]**: A dictionary containing the currently available
+devices. All values are strings except for `ID_USB_INTERFACES`, which is a
+`tuple` of `string` ### USBMonitor.changes_from_last_check
+(update_last_check_devices = True) Returns a tuple of two dictionaries, one
+containing the devices that have been *removed* since the last check, and
+another one containing the devices that have been *added*. Both dictionaries
+will have the `Device ID` as key and all the device information as value.
+Remember that all the [keys of this dictionary](#device-properties) can be
 found at can be found at `attributes.DEVICE_ATTRIBUTES`. -
 `update_last_check_devices`: **bool**. If `True` it will update the internal
 `USBMonitor.last_check_devices` attribute. So the next time you'll call this
 method, it will check for differences against the devices found in that current
 call. If `False` it won't update the `USBMonitor.last_check_devices` attribute.
 - Returns: **tuple[dict[str, dict[str, str|tuple[str, ...]]], dict[str, dict
 [str, str|tuple[str, ...]]]]**: A `tuple` containing two `dictionaries`. The
@@ -79,22 +91,35 @@
 **removed** since the last check and the second dictionary contains the
 information of the new **added** devices. All values are `strings` except for
 `ID_USB_INTERFACES`, which is a `tuple` of `string`. ###
 USBMonitor.check_changes(on_connect = None, on_disconnect = None,
 update_last_check_devices = True) Checks for any new connections or
 disconnections of USB devices since the last check. If a device has been
 removed, the `on_disconnect` function will be called with the `Device ID` as
-the first argument and the dictionary of device information as the second
-argument. The same will occur with the `on_connect` function if any new device
-have been added. Internally this function will just run
-`USBMonitor.changes_from_last_check` and will execute the callbacks for each
-returned device - `on_connect`: **callable | None**. The function to call when
-a device is added. It is expected to have the following format `on_connect
+the first argument and the [dictionary with the device's information](#device-
+properties) as the second argument. The same will occur with the `on_connect`
+function if any new device have been added. Internally this function will just
+run `USBMonitor.changes_from_last_check` and will execute the callbacks for
+each returned device - `on_connect`: **callable | None**. The function to call
+when a device is added. It is expected to have the following format `on_connect
 (device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])` -
 `on_disconnect`: **callable | None**. The function to call when a device is
 removed. It is expected to have the following format `on_disconnect(device_id:
 str, device_info: dict[str, dict[str, str|tuple[str, ...]]])` -
 `update_last_check_devices`: **bool**. If `True` it will update the internal
 `USBMonitor.last_check_devices` attribute. So the next time you'll call this
 method, it will check for differences against the devices found in that current
 call. If `False` it won't update the `USBMonitor.last_check_devices` attribute.
-### Device Properties
+### Device Properties The `device_info` returned by most functions will contain
+the following information: Key | Value Description | Example :-- | :-- | :-
+- `'ID_MODEL_ID'` | The product ID of the USB device. | `'0892'` `'ID_MODEL'` |
+The name of the USB device model. | `'HD_Pro_Webcam_C920'`
+`'ID_MODEL_FROM_DATABASE'` | Device model name, retrieved from the device
+database.| `'OrbiCam'` `'ID_VENDOR'` | The name of the USB device vendor |
+`'046d'` `'ID_VENDOR_ID'` | The vendor ID of the USB device. | `'046d'`
+`'ID_VENDOR_FROM_DATABASE'` | USB device vendor's name, from the device
+database. | `'Logitech, Inc.'` `'DEVNAME'` | The device name or path | `'/dev/
+bus/usb/001/003'` `'ID_USB_INTERFACES'` | A `tuple` representing the USB
+device's interfaces. | `('0e0100', '0e0200', '010100', '010200')` `'DEVTYPE'` |
+Should always be `'usb_device'`. | `'usb_device'` Note that, depending on the
+device and the OS, some of this information may be incomplete or certain
+attributes may overlap with others.
```

### Comparing `usb-monitor-1.8/setup.py` & `usb-monitor-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='usb-monitor',
-    version='1.8',
+    version='1.9',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/USBMonitor',
     description='USBMonitor is an easy-to-use cross-platform library for USB device monitoring that simplifies '
                 'tracking of connections, disconnections, and examination of connected device attributes on both '
                 'Windows and Linux, freeing the user from platform-specific details or incompatibilities.',
```

### Comparing `usb-monitor-1.8/usb_monitor.egg-info/PKG-INFO` & `usb-monitor-1.9/usb_monitor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usb-monitor
-Version: 1.8
+Version: 1.9
 Summary: USBMonitor is an easy-to-use cross-platform library for USB device monitoring that simplifies tracking of connections, disconnections, and examination of connected device attributes on both Windows and Linux, freeing the user from platform-specific details or incompatibilities.
 Home-page: https://github.com/Eric-Canas/USBMonitor
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -60,51 +60,95 @@
 monitor.start_monitoring(on_connect=on_connect, on_disconnect=on_disconnect)
 
 # ... Rest of your code ...
 
 # If you don't need it anymore stop the daemon
 monitor.stop_monitoring()
 ```
+Output
 Linux | Windows
 :---: | :---:
 ![](https://raw.githubusercontent.com/Eric-Canas/USBMonitor/main/resources/linux_monitor.gif) | ![](https://raw.githubusercontent.com/Eric-Canas/USBMonitor/main/resources/windows_monitor.gif)
 
+Sometimes, when initializing your software, you may seek to confirm which USB devices are indeed connected. 
+
+```python
+from usbmonitor import USBMonitor
+from usbmonitor.attributes import ID_MODEL, ID_MODEL_ID, ID_VENDOR_ID
+
+# Create the USBMonitor instance
+monitor = USBMonitor()
+
+# Get the current devices
+devices_dict = monitor.get_current_available_devices()
+
+# Print them
+for device_id, device_info in devices_dict.items():
+    print(f"{device_id} -- {device_info[ID_MODEL]} ({device_info[ID_MODEL_ID]} - {device_info[ID_VENDOR_ID]})")
+```
+Output
+```bash
+/dev/bus/usb/001/001 -- xHCI_Host_Controller (0002 - 1d6b)
+/dev/bus/usb/001/002 -- USB2.0_Hub (3431 - 2109)
+/dev/bus/usb/001/003 -- USB_Optical_Mouse (c077 - 046d)
+/dev/bus/usb/001/004 -- USB_Compliant_Keypad (9881 - 05a4)
+/dev/bus/usb/002/001 -- xHCI_Host_Controller (0003 - 1d6b)
+```
+
+
 
 ## API Reference
 
 ### USBMonitor.start_monitoring(on_connect = None, on_disconnect = None, check_every_seconds = 0.5)
-Starts a daemon that continuously monitors the connected USB devices in order to detect new connections or disconnections. When a device is disconnected, the `on_disconnect` callback function is invoked with the Device ID as the first argument and the dictionary of device information as the second argument. Similarly, when a new device is connected, the `on_connect` callback function is called with the same arguments. This allows developers to promptly respond to any changes in the connected USB devices and perform necessary actions.
+Starts a daemon that continuously monitors the connected USB devices in order to detect new connections or disconnections. When a device is disconnected, the `on_disconnect` callback function is invoked with the Device ID as the first argument and the [dictionary of device information](#device-properties) as the second argument. Similarly, when a new device is connected, the `on_connect` callback function is called with the same arguments. This allows developers to promptly respond to any changes in the connected USB devices and perform necessary actions.
 
 - `on_connect`: **callable | None**. The function to call every time a device is **added**. It is expected to have the following format `on_connect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `on_disconnect`: **callable | None**. The function to call every time a device is **removed**. It is expected to have the following format `on_disconnect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `check_every_seconds`: **int | float**. Seconds to wait between each check for changes in the USB devices. Default value is 0.5 seconds.
 
 ### USBMonitor.stop_monitoring(warn_if_was_stopped=True)
 Stops the monitoring of USB devices. This function will **stop** the daemon launched by `USBMonitor.start_monitoring`
 
 - `warn_if_was_stopped`: **bool**. If set to `True`, this function will issue a warning if the monitoring of USB devices was already stopped (the daemon was not running).
 
 
 ### USBMonitor.get_current_available_devices()
-Returns a dictionary of the currently available devices, where the key is the `Device ID` and the value is a dictionary containing the device's information. All the keys of this dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They always correspond with the default Linux device properties (independently of the OS where the library is running).
+Returns a dictionary of the currently available devices, where the key is the `Device ID` and the value is a [dictionary containing the device's information](#device-properties). All the keys of this dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They always correspond with the default Linux device properties (independently of the OS where the library is running).
 
 - Returns: **dict[str, dict[str, str|tuple[str, ...]]]**: A dictionary containing the currently available devices. All values are strings except for `ID_USB_INTERFACES`, which is a `tuple` of `string`
 
 
 
 ### USBMonitor.changes_from_last_check(update_last_check_devices = True)
-Returns a tuple of two dictionaries, one containing the devices that have been *removed* since the last check, and another one containing the devices that have been *added*. Both dictionaries will have the `Device ID` as key and all the device information as value. Remember that all the keys of this dictionary can be found at can be found at `attributes.DEVICE_ATTRIBUTES`.
+Returns a tuple of two dictionaries, one containing the devices that have been *removed* since the last check, and another one containing the devices that have been *added*. Both dictionaries will have the `Device ID` as key and all the device information as value. Remember that all the [keys of this dictionary](#device-properties) can be found at can be found at `attributes.DEVICE_ATTRIBUTES`.
 
 - `update_last_check_devices`: **bool**. If `True` it will update the internal `USBMonitor.last_check_devices` attribute. So the next time you'll call this method, it will check for differences against the devices found in that current call. If `False` it won't update the `USBMonitor.last_check_devices` attribute. 
 
 - Returns: **tuple[dict[str, dict[str, str|tuple[str, ...]]], dict[str, dict[str, str|tuple[str, ...]]]]**: A `tuple` containing two `dictionaries`. The first `dictionary` contains the information of the devices that were **removed** since the last check and the second dictionary contains the information of the new **added** devices. All values are `strings` except for `ID_USB_INTERFACES`, which is a `tuple` of `string`.
 
 ### USBMonitor.check_changes(on_connect = None, on_disconnect = None, update_last_check_devices = True)
-Checks for any new connections or disconnections of USB devices since the last check. If a device has been removed, the `on_disconnect` function will be called with the `Device ID` as the first argument and the dictionary of device information as the second argument. The same will occur with the `on_connect` function if any new device have been added. Internally this function will just run `USBMonitor.changes_from_last_check` and will execute the callbacks for each returned device
+Checks for any new connections or disconnections of USB devices since the last check. If a device has been removed, the `on_disconnect` function will be called with the `Device ID` as the first argument and the [dictionary with the device's information](#device-properties) as the second argument. The same will occur with the `on_connect` function if any new device have been added. Internally this function will just run `USBMonitor.changes_from_last_check` and will execute the callbacks for each returned device
 
 - `on_connect`: **callable | None**. The function to call when a device is added. It is expected to have the following format `on_connect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `on_disconnect`: **callable | None**. The function to call when a device is removed. It is expected to have the following format `on_disconnect(device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])`
 - `update_last_check_devices`: **bool**. If `True` it will update the internal `USBMonitor.last_check_devices` attribute. So the next time you'll call this method, it will check for differences against the devices found in that current call. If `False` it won't update the `USBMonitor.last_check_devices` attribute. 
 
 ### Device Properties
 
+The `device_info` returned by most functions will contain the following information:
+
+Key | Value Description | Example
+:-- | :-- | :--
+`'ID_MODEL_ID'` | The product ID of the USB device. | `'0892'`
+`'ID_MODEL'` | The name of the USB device model. | `'HD_Pro_Webcam_C920'`
+`'ID_MODEL_FROM_DATABASE'` | Device model name, retrieved from the device database.| `'OrbiCam'`
+`'ID_VENDOR'` | The name of the USB device vendor | `'046d'`
+`'ID_VENDOR_ID'` | The vendor ID of the USB device. | `'046d'`
+`'ID_VENDOR_FROM_DATABASE'` | USB device vendor's name, from the device database. | `'Logitech, Inc.'`
+`'DEVNAME'` | The device name or path  | `'/dev/bus/usb/001/003'`
+`'ID_USB_INTERFACES'` |	A `tuple` representing the USB device's interfaces. | `('0e0100', '0e0200', '010100', '010200')`
+`'DEVTYPE'` | Should always be `'usb_device'`. | `'usb_device'`
+
+Note that, depending on the device and the OS, some of this information may be incomplete or certain attributes may overlap with others.
+
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usb-monitor Version: 1.8 Summary: USBMonitor is an
+Metadata-Version: 2.1 Name: usb-monitor Version: 1.9 Summary: USBMonitor is an
 easy-to-use cross-platform library for USB device monitoring that simplifies
 tracking of connections, disconnections, and examination of connected device
 attributes on both Windows and Linux, freeing the user from platform-specific
 details or incompatibilities. Home-page: https://github.com/Eric-Canas/
 USBMonitor Author: Eric-Canas Author-email: eric@ericcanas.com License: MIT
 Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
@@ -43,52 +43,65 @@
 [ID_MODEL_ID]} - {device_info[ID_VENDOR_ID]})" # Define the `on_connect` and
 `on_disconnect` callbacks on_connect = lambda device_id, device_info: print
 (f"Connected: {device_info_str(device_info=device_info)}") on_disconnect =
 lambda device_id, device_info: print(f"Disconnected: {device_info_str
 (device_info=device_info)}") # Create the USBMonitor instance monitor =
 USBMonitor() # Start the daemon monitor.start_monitoring(on_connect=on_connect,
 on_disconnect=on_disconnect) # ... Rest of your code ... # If you don't need it
-anymore stop the daemon monitor.stop_monitoring() ``` Linux | Windows :---: | :
----: ![](https://raw.githubusercontent.com/Eric-Canas/USBMonitor/main/
+anymore stop the daemon monitor.stop_monitoring() ``` Output Linux | Windows :-
+--: | :---: ![](https://raw.githubusercontent.com/Eric-Canas/USBMonitor/main/
 resources/linux_monitor.gif) | ![](https://raw.githubusercontent.com/Eric-
-Canas/USBMonitor/main/resources/windows_monitor.gif) ## API Reference ###
+Canas/USBMonitor/main/resources/windows_monitor.gif) Sometimes, when
+initializing your software, you may seek to confirm which USB devices are
+indeed connected. ```python from usbmonitor import USBMonitor from
+usbmonitor.attributes import ID_MODEL, ID_MODEL_ID, ID_VENDOR_ID # Create the
+USBMonitor instance monitor = USBMonitor() # Get the current devices
+devices_dict = monitor.get_current_available_devices() # Print them for
+device_id, device_info in devices_dict.items(): print(f"{device_id} --
+{device_info[ID_MODEL]} ({device_info[ID_MODEL_ID]} - {device_info
+[ID_VENDOR_ID]})") ``` Output ```bash /dev/bus/usb/001/001 -
+- xHCI_Host_Controller (0002 - 1d6b) /dev/bus/usb/001/002 -- USB2.0_Hub (3431 -
+2109) /dev/bus/usb/001/003 -- USB_Optical_Mouse (c077 - 046d) /dev/bus/usb/001/
+004 -- USB_Compliant_Keypad (9881 - 05a4) /dev/bus/usb/002/001 -
+- xHCI_Host_Controller (0003 - 1d6b) ``` ## API Reference ###
 USBMonitor.start_monitoring(on_connect = None, on_disconnect = None,
 check_every_seconds = 0.5) Starts a daemon that continuously monitors the
 connected USB devices in order to detect new connections or disconnections.
 When a device is disconnected, the `on_disconnect` callback function is invoked
-with the Device ID as the first argument and the dictionary of device
-information as the second argument. Similarly, when a new device is connected,
-the `on_connect` callback function is called with the same arguments. This
-allows developers to promptly respond to any changes in the connected USB
-devices and perform necessary actions. - `on_connect`: **callable | None**. The
-function to call every time a device is **added**. It is expected to have the
-following format `on_connect(device_id: str, device_info: dict[str, dict[str,
-str|tuple[str, ...]]])` - `on_disconnect`: **callable | None**. The function to
-call every time a device is **removed**. It is expected to have the following
-format `on_disconnect(device_id: str, device_info: dict[str, dict[str,
-str|tuple[str, ...]]])` - `check_every_seconds`: **int | float**. Seconds to
-wait between each check for changes in the USB devices. Default value is 0.5
+with the Device ID as the first argument and the [dictionary of device
+information](#device-properties) as the second argument. Similarly, when a new
+device is connected, the `on_connect` callback function is called with the same
+arguments. This allows developers to promptly respond to any changes in the
+connected USB devices and perform necessary actions. - `on_connect`: **callable
+| None**. The function to call every time a device is **added**. It is expected
+to have the following format `on_connect(device_id: str, device_info: dict[str,
+dict[str, str|tuple[str, ...]]])` - `on_disconnect`: **callable | None**. The
+function to call every time a device is **removed**. It is expected to have the
+following format `on_disconnect(device_id: str, device_info: dict[str, dict
+[str, str|tuple[str, ...]]])` - `check_every_seconds`: **int | float**. Seconds
+to wait between each check for changes in the USB devices. Default value is 0.5
 seconds. ### USBMonitor.stop_monitoring(warn_if_was_stopped=True) Stops the
 monitoring of USB devices. This function will **stop** the daemon launched by
 `USBMonitor.start_monitoring` - `warn_if_was_stopped`: **bool**. If set to
 `True`, this function will issue a warning if the monitoring of USB devices was
 already stopped (the daemon was not running). ###
 USBMonitor.get_current_available_devices() Returns a dictionary of the
 currently available devices, where the key is the `Device ID` and the value is
-a dictionary containing the device's information. All the keys of this
-dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They always
-correspond with the default Linux device properties (independently of the OS
-where the library is running). - Returns: **dict[str, dict[str, str|tuple[str,
-...]]]**: A dictionary containing the currently available devices. All values
-are strings except for `ID_USB_INTERFACES`, which is a `tuple` of `string` ###
-USBMonitor.changes_from_last_check(update_last_check_devices = True) Returns a
-tuple of two dictionaries, one containing the devices that have been *removed*
-since the last check, and another one containing the devices that have been
-*added*. Both dictionaries will have the `Device ID` as key and all the device
-information as value. Remember that all the keys of this dictionary can be
+a [dictionary containing the device's information](#device-properties). All the
+keys of this dictionary can be found at `attributes.DEVICE_ATTRIBUTES`. They
+always correspond with the default Linux device properties (independently of
+the OS where the library is running). - Returns: **dict[str, dict[str,
+str|tuple[str, ...]]]**: A dictionary containing the currently available
+devices. All values are strings except for `ID_USB_INTERFACES`, which is a
+`tuple` of `string` ### USBMonitor.changes_from_last_check
+(update_last_check_devices = True) Returns a tuple of two dictionaries, one
+containing the devices that have been *removed* since the last check, and
+another one containing the devices that have been *added*. Both dictionaries
+will have the `Device ID` as key and all the device information as value.
+Remember that all the [keys of this dictionary](#device-properties) can be
 found at can be found at `attributes.DEVICE_ATTRIBUTES`. -
 `update_last_check_devices`: **bool**. If `True` it will update the internal
 `USBMonitor.last_check_devices` attribute. So the next time you'll call this
 method, it will check for differences against the devices found in that current
 call. If `False` it won't update the `USBMonitor.last_check_devices` attribute.
 - Returns: **tuple[dict[str, dict[str, str|tuple[str, ...]]], dict[str, dict
 [str, str|tuple[str, ...]]]]**: A `tuple` containing two `dictionaries`. The
@@ -96,22 +109,35 @@
 **removed** since the last check and the second dictionary contains the
 information of the new **added** devices. All values are `strings` except for
 `ID_USB_INTERFACES`, which is a `tuple` of `string`. ###
 USBMonitor.check_changes(on_connect = None, on_disconnect = None,
 update_last_check_devices = True) Checks for any new connections or
 disconnections of USB devices since the last check. If a device has been
 removed, the `on_disconnect` function will be called with the `Device ID` as
-the first argument and the dictionary of device information as the second
-argument. The same will occur with the `on_connect` function if any new device
-have been added. Internally this function will just run
-`USBMonitor.changes_from_last_check` and will execute the callbacks for each
-returned device - `on_connect`: **callable | None**. The function to call when
-a device is added. It is expected to have the following format `on_connect
+the first argument and the [dictionary with the device's information](#device-
+properties) as the second argument. The same will occur with the `on_connect`
+function if any new device have been added. Internally this function will just
+run `USBMonitor.changes_from_last_check` and will execute the callbacks for
+each returned device - `on_connect`: **callable | None**. The function to call
+when a device is added. It is expected to have the following format `on_connect
 (device_id: str, device_info: dict[str, dict[str, str|tuple[str, ...]]])` -
 `on_disconnect`: **callable | None**. The function to call when a device is
 removed. It is expected to have the following format `on_disconnect(device_id:
 str, device_info: dict[str, dict[str, str|tuple[str, ...]]])` -
 `update_last_check_devices`: **bool**. If `True` it will update the internal
 `USBMonitor.last_check_devices` attribute. So the next time you'll call this
 method, it will check for differences against the devices found in that current
 call. If `False` it won't update the `USBMonitor.last_check_devices` attribute.
-### Device Properties
+### Device Properties The `device_info` returned by most functions will contain
+the following information: Key | Value Description | Example :-- | :-- | :-
+- `'ID_MODEL_ID'` | The product ID of the USB device. | `'0892'` `'ID_MODEL'` |
+The name of the USB device model. | `'HD_Pro_Webcam_C920'`
+`'ID_MODEL_FROM_DATABASE'` | Device model name, retrieved from the device
+database.| `'OrbiCam'` `'ID_VENDOR'` | The name of the USB device vendor |
+`'046d'` `'ID_VENDOR_ID'` | The vendor ID of the USB device. | `'046d'`
+`'ID_VENDOR_FROM_DATABASE'` | USB device vendor's name, from the device
+database. | `'Logitech, Inc.'` `'DEVNAME'` | The device name or path | `'/dev/
+bus/usb/001/003'` `'ID_USB_INTERFACES'` | A `tuple` representing the USB
+device's interfaces. | `('0e0100', '0e0200', '010100', '010200')` `'DEVTYPE'` |
+Should always be `'usb_device'`. | `'usb_device'` Note that, depending on the
+device and the OS, some of this information may be incomplete or certain
+attributes may overlap with others.
```

### Comparing `usb-monitor-1.8/usb_monitor.egg-info/SOURCES.txt` & `usb-monitor-1.9/usb_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `usb-monitor-1.8/usbmonitor/__platform_specific_detectors/_constants.py` & `usb-monitor-1.9/usbmonitor/__platform_specific_detectors/_constants.py`

 * *Files identical despite different names*

### Comparing `usb-monitor-1.8/usbmonitor/__platform_specific_detectors/_linux_usb_detector.py` & `usb-monitor-1.9/usbmonitor/__platform_specific_detectors/_linux_usb_detector.py`

 * *Files identical despite different names*

### Comparing `usb-monitor-1.8/usbmonitor/__platform_specific_detectors/_usb_detector_base.py` & `usb-monitor-1.9/usbmonitor/__platform_specific_detectors/_usb_detector_base.py`

 * *Files identical despite different names*

### Comparing `usb-monitor-1.8/usbmonitor/__platform_specific_detectors/_windows_usb_detector.py` & `usb-monitor-1.9/usbmonitor/__platform_specific_detectors/_windows_usb_detector.py`

 * *Files identical despite different names*

### Comparing `usb-monitor-1.8/usbmonitor/attributes.py` & `usb-monitor-1.9/usbmonitor/attributes.py`

 * *Files identical despite different names*

### Comparing `usb-monitor-1.8/usbmonitor/usbmonitor.py` & `usb-monitor-1.9/usbmonitor/usbmonitor.py`

 * *Files identical despite different names*

