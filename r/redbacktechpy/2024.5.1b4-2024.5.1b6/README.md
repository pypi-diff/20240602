# Comparing `tmp/redbacktechpy-2024.5.1b4.tar.gz` & `tmp/redbacktechpy-2024.5.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbacktechpy-2024.5.1b4.tar", last modified: Sat Jun  1 20:33:04 2024, max compression
+gzip compressed data, was "redbacktechpy-2024.5.1b6.tar", last modified: Sat Jun  1 22:34:16 2024, max compression
```

## Comparing `redbacktechpy-2024.5.1b4.tar` & `redbacktechpy-2024.5.1b6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:33:04.647641 redbacktechpy-2024.5.1b4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 20:33:04.647641 redbacktechpy-2024.5.1b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 20:33:04.647641 redbacktechpy-2024.5.1b4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:33:04.643641 redbacktechpy-2024.5.1b4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:33:04.643641 redbacktechpy-2024.5.1b4/src/redbacktechpy/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    50891 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/redbacktech_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-01 20:33:00.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy/str_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:33:04.643641 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 20:33:04.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-01 20:33:04.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 20:33:04.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 20:33:04.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 20:33:04.000000 redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/src/redbacktechpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50889 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/redbacktech_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-01 22:34:11.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy/str_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 22:34:16.122722 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 22:34:16.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-01 22:34:16.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 22:34:16.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 22:34:16.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 22:34:16.000000 redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/top_level.txt
```

### Comparing `redbacktechpy-2024.5.1b4/LICENSE` & `redbacktechpy-2024.5.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b4/PKG-INFO` & `redbacktechpy-2024.5.1b6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b4
+Version: 2024.5.1b6
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `redbacktechpy-2024.5.1b4/pyproject.toml` & `redbacktechpy-2024.5.1b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "redbacktechpy"
-version = "2024.05.1b4"
+version = "2024.05.1b6"
 authors = [
   { name="Chris Abberley", email="unlisted@gmail.com" },
 ]
 description = "Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
```

### Comparing `redbacktechpy-2024.5.1b4/src/redbacktechpy/__init__.py` & `redbacktechpy-2024.5.1b6/src/redbacktechpy/__init__.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b4/src/redbacktechpy/constants.py` & `redbacktechpy-2024.5.1b6/src/redbacktechpy/constants.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b4/src/redbacktechpy/model.py` & `redbacktechpy-2024.5.1b6/src/redbacktechpy/model.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b4/src/redbacktechpy/redbacktech_client.py` & `redbacktechpy-2024.5.1b6/src/redbacktechpy/redbacktech_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,23 +60,23 @@
         await self.create_device_info()
         
         inverter_data: dict[str, Inverters] = {}
         battery_data: dict[str, Batterys] = {}
         entity_data: dict[str, RedbackEntitys] = {}
         device_info_data: dict[str, DeviceInfo] = {}
         
-        #if self._redback_devices is not None:
-        #    for device in self._redback_devices:
-        #        if device['device_type'] == 'inverter':
-        #            in_instance, in_id = await self._handle_inverter(device)
-        #            inverter_data[in_id] = in_instance
+        if self._redback_devices is not None:
+            for device in self._redback_devices:
+                if device['device_type'] == 'inverter':
+                    in_instance, in_id = await self._handle_inverter(device)
+                    inverter_data[in_id] = in_instance
                     
-        #        if device['device_type'] == 'battery':
-        #            bat_instance, bat_id = await self._handle_battery(device)
-        #            battery_data[bat_id] = bat_instance
+                if device['device_type'] == 'battery':
+                    bat_instance, bat_id = await self._handle_battery(device)
+                    battery_data[bat_id] = bat_instance
         if self._redback_entities is not None:
             for entity in self._redback_entities:
                 ent_instance, ent_id = await self._handle_entity(entity)
                 entity_data[ent_id] = ent_instance            
         
         if self._redback_device_info is not None:
             for device in self._redback_device_info:
@@ -295,26 +295,26 @@
             #Get the device info if it needs to be refreshed
             self._serial_numbers = await self.get_inverter_list()
             device_info = False
         
         for serial_number in self._serial_numbers:
             response1 = await self.get_static_by_serial(serial_number)
             response2 = await self.get_dynamic_by_serial(serial_number)
-            #self._flatInverters = await self._convert_static_by_serial_to_inverter_list(response1, response2)
-            #self._redback_devices.append(self._flatInverters)  ###
+            self._flatInverters = await self._convert_static_by_serial_to_inverter_list(response1, response2)
+            self._redback_devices.append(self._flatInverters)  ###
             await self._convert_responses_to_inverter_entities(response1, response2)
             await self._create_device_info_inverter(response1)
             #print(self._flatInverters['serial_number'])
             #response = await self.create_dynamic_info()
             if response1['Data']['Nodes'][0]['StaticData']['BatteryCount'] > 0:
                 soc_data = await self.get_config_by_serial(response1['Data']['Nodes'][0]['StaticData']['Id'])
-                #self._flatBatterys = await self._convert_static_by_serial_to_battery_list(response1, response2, soc_data)
+                self._flatBatterys = await self._convert_static_by_serial_to_battery_list(response1, response2, soc_data)
                 await self._convert_responses_to_battery_entities(response1, response2, soc_data)
                 await self._create_device_info_battery(response1)
-            #self._redback_devices.append(self._flatBatterys)
+                self._redback_devices.append(self._flatBatterys)
         self._device_info_refresh_time = datetime.now() + timedelta(seconds=DEVICEINFOREFRESH)
         return 
     
     async def create_dynamic_info(self) -> None:
 
         self._serial_numbers = await self.get_inverter_list()
         self._dynamic_data = []
@@ -366,17 +366,17 @@
         dataDict['export_all_time_energy_kwh'] = data2['Data']['ExportAllTimeEnergykWh']
         dataDict['import_all_time_energy_kwh'] = data2['Data']['ImportAllTimeEnergykWh']
         dataDict['load_all_time_energy_kwh'] = data2['Data']['LoadAllTimeEnergykWh']
         dataDict['status'] = data2['Data']['Status']
         dataDict['power_mode_inverter_mode'] = data2['Data']['Inverters'][0]['PowerMode']['InverterMode']
         dataDict['power_mode_power_w'] = data2['Data']['Inverters'][0]['PowerMode']['PowerW']
         for pv in data2['Data']['PVs']:
-            dataDict[f'pv_{pvId}_current_a'] = pv['CurrentA']
-            dataDict[f'pv_{pvId}_voltage_v'] = pv['VoltageV']
-            dataDict[f'pv_{pvId}_power_kw'] = pv['PowerkW']
+            dataDict[f'mppt_{pvId}_current_a'] = pv['CurrentA']
+            dataDict[f'mppt_{pvId}_voltage_v'] = pv['VoltageV']
+            dataDict[f'mppt_{pvId}_power_kw'] = pv['PowerkW']
             pvId += 1
         for phase in data2['Data']['Phases']:  
             phaseAlpha=phase['Id']
             dataDict[f'inverter_phase_{phaseAlpha}_active_exported_power_instantaneous_kw'] = phase['ActiveExportedPowerInstantaneouskW']
             dataDict[f'inverter_phase_{phaseAlpha}_active_imported_power_instantaneous_kw'] = phase['ActiveImportedPowerInstantaneouskW']
             dataDict[f'inverter_phase_{phaseAlpha}_voltage_instantaneous_v'] = phase['VoltageInstantaneousV']
             dataDict[f'inverter_phase_{phaseAlpha}_current_instantaneous_a'] = phase['CurrentInstantaneousA']
```

### Comparing `redbacktechpy-2024.5.1b4/src/redbacktechpy/str_enum.py` & `redbacktechpy-2024.5.1b6/src/redbacktechpy/str_enum.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b4/src/redbacktechpy.egg-info/PKG-INFO` & `redbacktechpy-2024.5.1b6/src/redbacktechpy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b4
+Version: 2024.5.1b6
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

