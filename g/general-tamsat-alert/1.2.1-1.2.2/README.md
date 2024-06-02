# Comparing `tmp/general_tamsat_alert-1.2.1.tar.gz` & `tmp/general_tamsat_alert-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general_tamsat_alert-1.2.1.tar", last modified: Sun Apr  7 17:52:56 2024, max compression
+gzip compressed data, was "general_tamsat_alert-1.2.2.tar", last modified: Sat Jun  1 23:59:12 2024, max compression
```

## Comparing `general_tamsat_alert-1.2.1.tar` & `general_tamsat_alert-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-07 17:52:56.177369 general_tamsat_alert-1.2.1/
--rw-r--r--   0 john      (1001) john      (1001)      761 2024-04-07 17:52:56.177369 general_tamsat_alert-1.2.1/PKG-INFO
--rw-rw-r--   0 john      (1001) john      (1001)      448 2024-02-18 17:35:53.000000 general_tamsat_alert-1.2.1/README.md
--rw-rw-r--   0 john      (1001) john      (1001)      536 2024-04-07 17:52:27.000000 general_tamsat_alert-1.2.1/pyproject.toml
--rw-rw-r--   0 john      (1001) john      (1001)       38 2024-04-07 17:52:56.177369 general_tamsat_alert-1.2.1/setup.cfg
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-07 17:52:56.177369 general_tamsat_alert-1.2.1/src/
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-07 17:52:56.177369 general_tamsat_alert-1.2.1/src/general_tamsat_alert/
--rw-rw-r--   0 john      (1001) john      (1001)     7072 2024-04-07 17:52:17.000000 general_tamsat_alert-1.2.1/src/general_tamsat_alert/__init__.py
--rw-rw-r--   0 john      (1001) john      (1001)     5946 2024-04-07 09:22:22.000000 general_tamsat_alert-1.2.1/src/general_tamsat_alert/ensembles.py
--rw-rw-r--   0 john      (1001) john      (1001)     3269 2024-04-02 15:01:21.000000 general_tamsat_alert-1.2.1/src/general_tamsat_alert/misc.py
--rw-rw-r--   0 john      (1001) john      (1001)     4790 2024-04-07 17:52:17.000000 general_tamsat_alert-1.2.1/src/general_tamsat_alert/periodicity.py
--rw-rw-r--   0 john      (1001) john      (1001)     1881 2024-04-02 15:14:12.000000 general_tamsat_alert-1.2.1/src/general_tamsat_alert/roc_auc.py
--rw-rw-r--   0 john      (1001) john      (1001)     3652 2024-04-02 15:06:02.000000 general_tamsat_alert-1.2.1/src/general_tamsat_alert/weighting_functions.py
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-07 17:52:56.177369 general_tamsat_alert-1.2.1/src/general_tamsat_alert.egg-info/
--rw-r--r--   0 john      (1001) john      (1001)      761 2024-04-07 17:52:56.000000 general_tamsat_alert-1.2.1/src/general_tamsat_alert.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1001) john      (1001)      545 2024-04-07 17:52:56.000000 general_tamsat_alert-1.2.1/src/general_tamsat_alert.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1001) john      (1001)        1 2024-04-07 17:52:56.000000 general_tamsat_alert-1.2.1/src/general_tamsat_alert.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1001) john      (1001)       27 2024-04-07 17:52:56.000000 general_tamsat_alert-1.2.1/src/general_tamsat_alert.egg-info/requires.txt
--rw-rw-r--   0 john      (1001) john      (1001)       21 2024-04-07 17:52:56.000000 general_tamsat_alert-1.2.1/src/general_tamsat_alert.egg-info/top_level.txt
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-07 17:52:56.177369 general_tamsat_alert-1.2.1/tests/
--rw-rw-r--   0 john      (1001) john      (1001)        0 2023-12-29 18:10:31.000000 general_tamsat_alert-1.2.1/tests/test_ensembles.py
--rw-rw-r--   0 john      (1001) john      (1001)     1764 2023-12-29 19:04:08.000000 general_tamsat_alert-1.2.1/tests/test_periodicity.py
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-06-01 23:59:12.306108 general_tamsat_alert-1.2.2/
+-rw-r--r--   0 john      (1001) john      (1001)      802 2024-06-01 23:59:12.306108 general_tamsat_alert-1.2.2/PKG-INFO
+-rw-rw-r--   0 john      (1001) john      (1001)      490 2024-06-01 22:33:11.000000 general_tamsat_alert-1.2.2/README.md
+-rw-rw-r--   0 john      (1001) john      (1001)      536 2024-06-01 23:58:59.000000 general_tamsat_alert-1.2.2/pyproject.toml
+-rw-rw-r--   0 john      (1001) john      (1001)       38 2024-06-01 23:59:12.310108 general_tamsat_alert-1.2.2/setup.cfg
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-06-01 23:59:12.306108 general_tamsat_alert-1.2.2/src/
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-06-01 23:59:12.306108 general_tamsat_alert-1.2.2/src/general_tamsat_alert/
+-rw-rw-r--   0 john      (1001) john      (1001)     8717 2024-06-01 23:53:03.000000 general_tamsat_alert-1.2.2/src/general_tamsat_alert/__init__.py
+-rw-rw-r--   0 john      (1001) john      (1001)     6555 2024-06-01 23:18:26.000000 general_tamsat_alert-1.2.2/src/general_tamsat_alert/ensembles.py
+-rw-rw-r--   0 john      (1001) john      (1001)     3732 2024-06-01 23:22:20.000000 general_tamsat_alert-1.2.2/src/general_tamsat_alert/misc.py
+-rw-rw-r--   0 john      (1001) john      (1001)     4790 2024-04-07 17:52:17.000000 general_tamsat_alert-1.2.2/src/general_tamsat_alert/periodicity.py
+-rw-rw-r--   0 john      (1001) john      (1001)     1881 2024-04-02 15:14:12.000000 general_tamsat_alert-1.2.2/src/general_tamsat_alert/roc_auc.py
+-rw-rw-r--   0 john      (1001) john      (1001)     3652 2024-04-02 15:06:02.000000 general_tamsat_alert-1.2.2/src/general_tamsat_alert/weighting_functions.py
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-06-01 23:59:12.306108 general_tamsat_alert-1.2.2/src/general_tamsat_alert.egg-info/
+-rw-r--r--   0 john      (1001) john      (1001)      802 2024-06-01 23:59:12.000000 general_tamsat_alert-1.2.2/src/general_tamsat_alert.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1001) john      (1001)      571 2024-06-01 23:59:12.000000 general_tamsat_alert-1.2.2/src/general_tamsat_alert.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1001) john      (1001)        1 2024-06-01 23:59:12.000000 general_tamsat_alert-1.2.2/src/general_tamsat_alert.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1001) john      (1001)       27 2024-06-01 23:59:12.000000 general_tamsat_alert-1.2.2/src/general_tamsat_alert.egg-info/requires.txt
+-rw-rw-r--   0 john      (1001) john      (1001)       21 2024-06-01 23:59:12.000000 general_tamsat_alert-1.2.2/src/general_tamsat_alert.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-06-01 23:59:12.306108 general_tamsat_alert-1.2.2/tests/
+-rw-rw-r--   0 john      (1001) john      (1001)      551 2024-06-01 23:57:04.000000 general_tamsat_alert-1.2.2/tests/test_do_forecast.py
+-rw-rw-r--   0 john      (1001) john      (1001)        0 2023-12-29 18:10:31.000000 general_tamsat_alert-1.2.2/tests/test_ensembles.py
+-rw-rw-r--   0 john      (1001) john      (1001)     1765 2024-06-01 23:07:54.000000 general_tamsat_alert-1.2.2/tests/test_periodicity.py
```

### Comparing `general_tamsat_alert-1.2.1/PKG-INFO` & `general_tamsat_alert-1.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: general_tamsat_alert
-Version: 1.2.1
+Version: 1.2.2
 Author-email: John Ellis <12johnellis@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: xarray
 Requires-Dist: scipy
 Requires-Dist: fastroc
 
-# General TAMSAT Alert
+# General TAMSAT Alert 
+## v1.2.1  DOI: 10.5281/zenodo.10955490
 
 A library to perform analysis of time series data in the way used in TAMSAT Alert.
 
 ## Installation
 ### From PyPI
 `pip install general-tamsat-alert`
 ### From source
```

### Comparing `general_tamsat_alert-1.2.1/pyproject.toml` & `general_tamsat_alert-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "general_tamsat_alert"
-version = "1.2.1"
+version = "1.2.2"
 dependencies = [
     "numpy",
     "xarray",
     "scipy",
     "fastroc",
 ]
 authors = [
```

### Comparing `general_tamsat_alert-1.2.1/src/general_tamsat_alert/__init__.py` & `general_tamsat_alert-1.2.2/src/general_tamsat_alert/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,38 @@
 import numpy as np
 import xarray as xr
+import datetime
 
 from .periodicity import get_periodicity
 from . import weighting_functions as wfs
 from .ensembles import get_ensembles
 from . import misc
 
 
 def get_index(da, axis_label, value):
     indices = np.arange(len(da[axis_label]), dtype=np.int64)
     nearest_value = da[axis_label].sel({axis_label: value}, method="nearest")
+
+    # Assume the values on the time axis label are increasing
+    max_value = da[axis_label].values[-1]
+    min_value = da[axis_label].values[0]
+    if value > max_value:
+        delta = value - max_value
+        max_index = get_index(da, axis_label, max_value)
+        if max_value - delta >= min_value:
+            opposite = get_index(da, axis_label, max_value - delta)
+            return (max_index - opposite) + max_index
+        else:
+            try:
+                max_delta = max_value - da[axis_label].values.min()
+                max_index_delta = da[axis_label].values.shape[0]
+                return round(max_index_delta * delta / max_delta + max_index)
+            except TypeError:
+                raise TypeError("Unable to extrapolate time index from non-numeric data")
+
     return indices[da[axis_label].isin(nearest_value)][0]
 
 
 def do_forecast(
     datafile,
     field_name,
     init_date,
@@ -21,44 +40,57 @@
     poi_end,
     time_label="time",
     period=12,
     weights_flag=0,
     weighting_data_file=None,
     weighting_strength=1,
     do_increments=1,
+    suppress_datetime_conversion=False
 ):
 
     '''
     Function that ingests time series data and produces ensemble forecasts using the TAMSAT-ALERT method
     
     Input parameters
     ----------------
-    :param datafile: netcdf file containing the time series data on which to base the forecasts. The datafile must include a time axis, but the format is otherwise flexible
+    :param datafile: netcdf file containing the time series data on which to base the forecasts. The datafile must
+                     include a time axis, but the format is otherwise flexible
     :param field_name: name of the variable to be forecast
     :param init_date: initiation date of the forecast (datetime object)
     :param poi_start: date of the start of the period of interest (datetime object)
     :param poi_end: date of the end of the period of interest (datetime object)
-    :param time_label [default 'time']: time axis label in the netcdf file
-    :param period [default 12]: period of the data to be used for deriving the climatology
-    :param weights_flag [default 0]: type of ensemble weighting to be used:
+    :param time_label: [default 'time'] time axis label in the netcdf file
+    :param period: [default 12] period of the data to be used for deriving the climatology
+    :param weights_flag: [default 0] type of ensemble weighting to be used:
         0: No weighting
         1: Weighting using the proximity of the ensemble member year to the initiation date
         2: Weighting using a monthly data included in weighting_data_file
-    :param weighting_data_file [default 'None']: text file containing the data to be used for weighting. The data are in the format used for the NOAA composite and correlation site (format described here: https://psl.noaa.gov/data/composites/createtime.html)
-    :param weighting_strength [default 1]: coefficient specifying the strength of the weighting used when weights_flag is set to 1 or 2. 0 indicates no weighting; floats >0 indicates weighting is applied. Users should experiment to find the most appropriate weighting strength
-    :param do_increments [default 1]: flag specifying whether or not the ensemble members should be incremented from the initial state. Set do_increments to 0 for no incrementing; 1 for incrementing
-    
+    :param weighting_data_file: [default 'None'] text file containing the data to be used for weighting. The data are
+                                in the format used for the NOAA composite and correlation site (format described here:
+                                https://psl.noaa.gov/data/composites/createtime.html)
+    :param weighting_strength: [default 1] coefficient specifying the strength of the weighting used when weights_flag
+                                is set to 1 or 2. 0 indicates no weighting; floats >0 indicates weighting is applied.
+                                Users should experiment to find the most appropriate weighting strength
+    :param do_increments: [default 1] flag specifying whether or not the ensemble members should be incremented from
+                                the initial state. Set do_increments to 0 for no incrementing; 1 for incrementing
+    :param suppress_datetime_conversion: [default False] whether to suppress the conversion of datetime.datetimes to
+                                np.datetime64 for poi_start, poi_end, time_label
+
     Returns
     -------
-    xarray dataset on the same grid and using the same dimensions as datafile, with an additional dimension 'ensemble' specifying the ensemble number. The dataset includes the following variables:
-    ensemble_out: array containing the full forecast ensemble (dimensions <datafile geographical dimensions>, <datafile time dimension>, ensemble)
-    weights: array containing the the weights applied to each ensemble member at each point in space (dimensions <datafile geographical dimensions>, ensemble). Note that in the current version of the code, weights is constant over the geographical domain
-    ens_mean: weighted ensemble mean (dimensions <datafile geographic dimensions>)
-    ens_std: weighted ensemble standard deviation (dimensions <datafile geographic dimensions>)
-    clim: climatology of the data in datafile (based on the user specified periodicity)
+    xarray dataset on the same grid and using the same dimensions as datafile, with an additional dimension 'ensemble'
+    specifying the ensemble number. The dataset includes the following variables:
+        ensemble_out: array containing the full forecast ensemble (dimensions <datafile geographical dimensions>,
+                      <datafile time dimension>, ensemble)
+        weights: array containing the the weights applied to each ensemble member at each point in space (dimensions
+                 <datafile geographical dimensions>, ensemble). Note that in the current version of the code,
+                 weights is constant over the geographical domain
+        ens_mean: weighted ensemble mean (dimensions <datafile geographic dimensions>)
+        ens_std: weighted ensemble standard deviation (dimensions <datafile geographic dimensions>)
+        clim: climatology of the data in datafile (based on the user specified periodicity)
     
     Example function call:
     ---------------------
     import datetime as dtmod
     from general_tamsat_alert import do_forecast
     
     
@@ -93,14 +125,24 @@
 
     weighting_functions = {
         0: wfs.no_weights_builder(),
         1: wfs.weight_time_builder(period, weighting_strength),
         2: wfs.weight_value_builder(weighting_data, weighting_strength),
     }
 
+    if not suppress_datetime_conversion:
+        if isinstance(init_date, datetime.datetime):
+            init_date = np.datetime64(init_date)
+
+        if isinstance(poi_start, datetime.datetime):
+            poi_start = np.datetime64(poi_start)
+
+        if isinstance(poi_end, datetime.datetime):
+            poi_end = np.datetime64(poi_end)
+
     init_index = get_index(da, time_label, init_date)
     poi_start_index = get_index(da, time_label, poi_start)
     poi_end_index = get_index(da, time_label, poi_end)
 
 
     # Calculate inputs for get_ensembles
     ensemble_start = init_index
```

### Comparing `general_tamsat_alert-1.2.1/src/general_tamsat_alert/ensembles.py` & `general_tamsat_alert-1.2.2/src/general_tamsat_alert/ensembles.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import xarray as xr
 import numpy as np
+
 from typing import List, Tuple, Hashable
 
 from . import weighting_functions as wfs
+from . import misc
 
 
 def get_ensembles(
         da: xr.DataArray,
         period: int,
         ensemble_length: int,
         initiation_index: int,
@@ -31,26 +33,40 @@
     :param ensemble_length:
     :param initiation_index:
     :param look_back:
     :param wf:
     :param time_label:
     :return:
     """
-    time = da[time_label].values[
-        initiation_index - look_back : initiation_index + ensemble_length
-    ]
+
+    invalid_init_date = False
+
+    if initiation_index + ensemble_length >= da[time_label].values.shape[0]:
+        invalid_init_date = True
+        try:
+            time = misc.extrapolate_time_label(da[time_label], initiation_index, initiation_index - look_back, initiation_index + ensemble_length, period)
+        except TypeError:
+            time = np.arange(initiation_index - look_back, initiation_index + ensemble_length)
+    else:
+        time = da[time_label].values[
+            initiation_index - look_back : initiation_index + ensemble_length
+        ]
 
     start_times = np.arange(
         initiation_index % period, len(da[time_label]) - ensemble_length, period
     )
     start_times = start_times[(start_times != initiation_index)]
-    start_times = np.insert(start_times, 0, initiation_index)
+    if not invalid_init_date:
+        start_times = np.insert(start_times, 0, initiation_index)
 
     ensemble_count = len(start_times)
-    ensemble_indices = np.arange(0, ensemble_count)
+    if not invalid_init_date:
+        ensemble_indices = np.arange(0, ensemble_count)
+    else:
+        ensemble_indices = np.arange(1, ensemble_count+1)
 
     coords = [da[i].values for i in da.dims if i != time_label] + [ensemble_indices]
     dims = [i for i in da.dims if i != time_label] + ["ensemble"]
 
     data = np.empty([len(i) for i in [time] + coords])
     ensembles = xr.DataArray(
         data, coords=[time] + coords, dims=[time_label] + dims, name="data",
```

### Comparing `general_tamsat_alert-1.2.1/src/general_tamsat_alert/misc.py` & `general_tamsat_alert-1.2.2/src/general_tamsat_alert/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 import xarray as xr
 import numpy as np
 
 
+def extrapolate_time_label(time_axis: xr.DataArray, initiation_index: int, start_index: int, end_index: int, period: int) -> xr.DataArray:
+    adjusted_start = start_index % period
+    offset = start_index - adjusted_start
+    adjusted_end = end_index - offset
+    adjusted_initiation = initiation_index - offset
+
+    delta = time_axis.values[initiation_index] - time_axis.values[adjusted_initiation]
+    return time_axis[adjusted_start : adjusted_end] + delta
+
+
 def read_noaa_data_file(
     fname: str,
     time_axis: xr.DataArray = None,
     time_label: str = "time",
     replace_given_nan_value=True,
 ):
     """
```

### Comparing `general_tamsat_alert-1.2.1/src/general_tamsat_alert/periodicity.py` & `general_tamsat_alert-1.2.2/src/general_tamsat_alert/periodicity.py`

 * *Files identical despite different names*

### Comparing `general_tamsat_alert-1.2.1/src/general_tamsat_alert/roc_auc.py` & `general_tamsat_alert-1.2.2/src/general_tamsat_alert/roc_auc.py`

 * *Files identical despite different names*

### Comparing `general_tamsat_alert-1.2.1/src/general_tamsat_alert/weighting_functions.py` & `general_tamsat_alert-1.2.2/src/general_tamsat_alert/weighting_functions.py`

 * *Files identical despite different names*

### Comparing `general_tamsat_alert-1.2.1/src/general_tamsat_alert.egg-info/PKG-INFO` & `general_tamsat_alert-1.2.2/src/general_tamsat_alert.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: general_tamsat_alert
-Version: 1.2.1
+Version: 1.2.2
 Author-email: John Ellis <12johnellis@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: xarray
 Requires-Dist: scipy
 Requires-Dist: fastroc
 
-# General TAMSAT Alert
+# General TAMSAT Alert 
+## v1.2.1  DOI: 10.5281/zenodo.10955490
 
 A library to perform analysis of time series data in the way used in TAMSAT Alert.
 
 ## Installation
 ### From PyPI
 `pip install general-tamsat-alert`
 ### From source
```

### Comparing `general_tamsat_alert-1.2.1/tests/test_periodicity.py` & `general_tamsat_alert-1.2.2/tests/test_periodicity.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
     assert len(get_non_nan_indices(ds, "precip", step=1)) == 324
     assert len(get_non_nan_indices(ds, "precip", step=10)) == 4
 
 def test_get_periodicity():
     assert get_periodicity(ds, 'ndvi') == 24
     assert get_periodicity(ds, 'ndvi', point={'lon': 0, 'lat': 0}) == 24
     with pytest.raises(OverflowError):
-        get_periodicity(ds, 'ndvi', point={'lon':4, 'lat':12})
+        get_periodicity(ds, 'ndvi', point={'lon':4, 'lat':12})
```

