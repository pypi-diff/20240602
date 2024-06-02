# Comparing `tmp/sif_tools-0.3.0-py3-none-any.whl.zip` & `tmp/sif_tools-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 20458 bytes, number of entries: 15
+Zip file size: 21423 bytes, number of entries: 15
 -rw-r--r--  2.0 unx    11034 b- defN 24-Jun-01 17:59 sif_tools/SIFopen.py
--rw-r--r--  2.0 unx     8457 b- defN 24-Jun-01 23:42 sif_tools/SIFplot.py
--rw-r--r--  2.0 unx     1588 b- defN 24-Jun-01 23:06 sif_tools/SIFpy.py
--rw-r--r--  2.0 unx       55 b- defN 24-Jun-01 23:31 sif_tools/__init__.py
+-rw-r--r--  2.0 unx     8461 b- defN 24-Jun-02 10:21 sif_tools/SIFplot.py
+-rw-r--r--  2.0 unx     4624 b- defN 24-Jun-02 10:53 sif_tools/SIFpy.py
+-rw-r--r--  2.0 unx       70 b- defN 24-Jun-02 10:45 sif_tools/__init__.py
 -rw-r--r--  2.0 unx      460 b- defN 24-Jun-01 23:31 sif_tools/__main__.py
--rw-r--r--  2.0 unx     7523 b- defN 24-Jun-01 23:14 sif_tools/utils.py
+-rw-r--r--  2.0 unx     7543 b- defN 24-Jun-02 10:23 sif_tools/utils.py
 -rw-r--r--  2.0 unx     6318 b- defN 24-Jun-01 23:18 sif_tools/CommandLine/CommandLineInterface.py
 -rw-r--r--  2.0 unx     2249 b- defN 24-Jun-01 23:35 sif_tools/CommandLine/CommandLineTools.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jun-01 22:31 sif_tools/CommandLine/__init__.py
--rw-r--r--  2.0 unx    14874 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4017 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1239 b- defN 24-Jun-02 00:19 sif_tools-0.3.0.dist-info/RECORD
-15 files, 57970 bytes uncompressed, 18400 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx    14874 b- defN 24-Jun-02 10:56 sif_tools-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4100 b- defN 24-Jun-02 10:56 sif_tools-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-02 10:56 sif_tools-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 24-Jun-02 10:56 sif_tools-0.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Jun-02 10:56 sif_tools-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1239 b- defN 24-Jun-02 10:56 sif_tools-0.3.1.dist-info/RECORD
+15 files, 61128 bytes uncompressed, 19365 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: sif_tools/CommandLine/CommandLineTools.py
 Comment: 
 
 Filename: sif_tools/CommandLine/__init__.py
 Comment: 
 
-Filename: sif_tools-0.3.0.dist-info/LICENSE
+Filename: sif_tools-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: sif_tools-0.3.0.dist-info/METADATA
+Filename: sif_tools-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: sif_tools-0.3.0.dist-info/WHEEL
+Filename: sif_tools-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: sif_tools-0.3.0.dist-info/entry_points.txt
+Filename: sif_tools-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: sif_tools-0.3.0.dist-info/top_level.txt
+Filename: sif_tools-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sif_tools-0.3.0.dist-info/RECORD
+Filename: sif_tools-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sif_tools/SIFplot.py

```diff
@@ -119,15 +119,15 @@
             plt.ylabel("Counts")
             plt.title(f"Plot of {filename}")
             plt.show()
 
         return
 
     @staticmethod
-    def hyperspectrum(directory: list[str], window:str = 'SHG', reduce_noise:bool = False, colorscheme:str = 'Blues'):
+    def hyperspectrum(directory: list[str], window:str = 'pinched', reduce_noise:bool = False, colorscheme:str = 'Blues'):
         """
         Generates a heatmap from hyperspectral data.
 
         Args:
             directory (list[str]): Directory containing spectrum files.
             window (str, optional): The window of data to be sliced for plotting. Defaults to 'SHG'.
             reduce_noise (bool, optional): Whether to reduce noise in the data. Defaults to False.
```

## sif_tools/SIFpy.py

```diff
@@ -1,33 +1,49 @@
 import os
 import numpy as np
+from scipy.interpolate import interp1d
 
 from .utils import MATH, FILE
 
-def sif2array(target, reduce_noise=False, window=None):
+@staticmethod
+def sif2array(target:str, reduce_noise:bool=False, window:str=None):
     """
     Convert SIF (Spectral Image Format) files to a NumPy array.
 
     This function processes SIF files from a given target (file or directory),
     optionally reduces noise, and slices the data to a specified window.
 
     Parameters:
     ----------
     target : str
         Path to a SIF file or a directory containing SIF files.
     reduce_noise : bool, optional
         If True, applies noise reduction to the data (default is False).
     window : str, optional
-        Specify the window for slicing the data. If None, the full data is used (default is None).
+        Specify the window for slicing the data. The window slices around the center wavelength:
+        - 'reduced': slices 10% of entries from each end
+        - 'narrow' : slices 25% of entries from each end
+        - 'pinched'    : slices 33% of entries from each end
 
     Returns:
     -------
     numpy.ndarray
         A NumPy array containing the combined spectral data from the SIF file(s).
         Each row corresponds to a pair of wavelength and count.
+
+    Examples:
+    ---------
+    To use the full data without slicing:
+        convert_sif_to_array(target='path/to/sif', reduce_noise=True, window=None)
+
+    To slice the first 100 data points:
+        convert_sif_to_array(target='path/to/sif', reduce_noise=True, window='0:100')
+
+    To slice from the 50th to the 200th data point:
+        convert_sif_to_array(target='path/to/sif', reduce_noise=True, window='50:200')
     """
     # Check if the target is a file or a directory
     if os.path.isfile(target):
         paths = [target]
     else:
         paths = FILE.extract_files_from_folder(target)
 
@@ -47,7 +63,62 @@
         data_list.append(np.column_stack((wavelengths, counts)))
 
     # Combine all data arrays into one ndarray
     if len(data_list) == 1:
         return data_list[0]
     else:
         return np.vstack(data_list)
+
+@staticmethod
+def hyperspectrum(directory:str, background:str, reduce_noise=True, window='pinched'):
+    
+    # check if directory is directory
+    if os.path.isfile(directory):
+        raise Exception("'directory' parameter has to be a directory, not a file.")
+    else:
+        files = FILE.extract_files_from_folder(directory)
+    
+    # access and treat background image
+    files.remove(background) # remove background file from list of files
+    # Parse and process the background file
+    background_data, _ = FILE.parse(os.path.join(directory, background))
+    background_data = MATH.slice_window(background_data, window=window)
+    bg_wavelengths, bg_counts = background_data[:, 0], background_data[:, 1]
+    if reduce_noise: # remove spikes using gradient method with 3-sigma threshold.
+        bg_wavelengths, bg_counts = MATH.gradient_n_sigma(bg_wavelengths, bg_counts)
+
+    positions = FILE.extract_positions(files)
+
+    pixels = []
+    for file in files:
+        data, _ = FILE.parse(os.path.join(directory, file))
+
+        data = MATH.slice_window(data, window=window)
+        wavelengths, counts = data[:, 0], data[:, 1]
+
+        if reduce_noise:
+            wavelengths, counts = MATH.gradient_n_sigma(wavelengths, counts)
+        
+        # Interpolate background counts to match the wavelengths of the current data
+        bg_interp = interp1d(bg_wavelengths, bg_counts, kind='linear', bounds_error=False, fill_value=0)
+        bg_counts_interpolated = bg_interp(wavelengths)
+
+        # Ensure counts do not go below zero after background subtraction
+        adjusted_counts = np.maximum(counts - bg_counts_interpolated, 0)
+        
+        pixels.append(int(np.sum(adjusted_counts)))
+    
+    normalized_pixels = MATH.normalize_array(np.array(pixels))
+    # Create a dictionary to hold the pixel values by position
+    counts_by_position = {(float(pos[1]), float(pos[2])): normalized_pixels for pos, normalized_pixels in zip(positions, normalized_pixels)}
+
+    # Determine the grid size
+    max_x = int(max(float(pos[1]) for pos in positions)) + 1
+    max_y = int(max(float(pos[2]) for pos in positions)) + 1
+    heatmap_data = np.zeros((max_y, max_x))
+
+    # Fill the heatmap data based on the positions
+    for pos, count in counts_by_position.items():
+        x, y = int(pos[0]), int(pos[1])
+        heatmap_data[y, x] = count
+
+    return heatmap_data
```

## sif_tools/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .SIFpy import sif2array
+from .SIFpy import sif2array, hyperspectrum
 from .__main__ import main
```

## sif_tools/utils.py

```diff
@@ -194,30 +194,31 @@
 
         Parameters
         ----------
         data: np.ndarray
             Data array to be sliced.
         
         window: str
-            Type of windowing to apply. Options are 'narrow', 'reduced', 'SHG'.
+            Type of windowing to apply. Options are 'reduced', 'narrow' and 'pinched'.
         
         Returns
         -------
         np.ndarray
             The sliced data array.
         """
-        if window == 'narrow':
-            remove_count = len(data) // 4
-            data = data[remove_count:-remove_count]
 
-        elif window == 'reduced':
+        if window == 'reduced':
             remove_count = len(data) // 10
             data = data[remove_count:-remove_count]
+        
+        elif window == 'narrow':
+            remove_count = len(data) // 4
+            data = data[remove_count:-remove_count]
 
-        elif window == 'SHG':
+        elif window == 'pinched':
             remove_count = len(data) // 3
             data = data[remove_count:-remove_count]
 
         return data
 
     def normalize_array(array):
         array_min = np.min(array)
```

## Comparing `sif_tools-0.3.0.dist-info/LICENSE` & `sif_tools-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sif_tools-0.3.0.dist-info/METADATA` & `sif_tools-0.3.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sif_tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: A light-weight package for Andor SIF file analysis
 Home-page: https://github.com/BjornFS/SIF-Tools
 Author: Bjorn F. Schroder N.
 Author-email: Bjornfschroder@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -56,14 +56,16 @@
 ```python 
 from sif_tools import sif2array
 
 file = '/Users/user/location/file.sif'
 data = sif2array(target=file, reduce_noise=False, window='narrow')
 ```
 
+See [examples](https://github.com/BjornFS/SIF-Tools/tree/main/examples) for more.
+
 ### Running SIF-Toolkit from the Command Line
 
 A client has been included, consisting of ```CommandLineInterface``` & ```CommandLineTools```, which is run from ```__main__.py``` :
 
 ```bash
 sif-tools
 ```
```

## Comparing `sif_tools-0.3.0.dist-info/RECORD` & `sif_tools-0.3.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 sif_tools/SIFopen.py,sha256=X5LUT6Jj3rBaSoMpGObfk_iIRsG7s-XXfJuA5bG2eAY,11034
-sif_tools/SIFplot.py,sha256=eeBRjc_uLp1SlDFiIGJ_A0ZCV1vqEYcPKlikkcE8r3o,8457
-sif_tools/SIFpy.py,sha256=tCG00H1bplEolEhpJPubVpbrUN_8ZmzDG-EZPZjB0oY,1588
-sif_tools/__init__.py,sha256=p85vqN2shbLq5sAMRCBpt8c0vIYltBlPtqa5Zy4oxac,55
+sif_tools/SIFplot.py,sha256=g2aXfj3jZSyyS9xqYaF7dA-ii38tV6k6dvWJYqqmQOw,8461
+sif_tools/SIFpy.py,sha256=hz9HyVWGTHRb6O4p-dPvHjJ8uQWPP2f1p2MVA8bKH9U,4624
+sif_tools/__init__.py,sha256=9W3ATgNvc2o4vPmIkrB_2S8Sbl4xFHQZ8JrStMUYIVQ,70
 sif_tools/__main__.py,sha256=iR9cpEf_WFEyC-uxVbTEXJHIQjA_XKYwi-StpbMJpNk,460
-sif_tools/utils.py,sha256=uKP4bTmItwtDfzlv_CRyjpq4Axbl1QF8oox9iparSU0,7523
+sif_tools/utils.py,sha256=HdNchlExt_NOCOgDT8BBEBm-4rN1BRO4vT8NuJ_izrw,7543
 sif_tools/CommandLine/CommandLineInterface.py,sha256=6GIp8BN1GjJOVVfHhwE2-RpxbLUd-RJ84-XA2geYz38,6318
 sif_tools/CommandLine/CommandLineTools.py,sha256=fWa6nPUgH83vLIJPHFbYGMqUFIaoq9ORwqf7BJs1z9g,2249
 sif_tools/CommandLine/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sif_tools-0.3.0.dist-info/LICENSE,sha256=baLxFkeB7Yhvfd2bvZHGsxrX8T_0FeM0SOf8iPapzw8,14874
-sif_tools-0.3.0.dist-info/METADATA,sha256=Ey7z29gRy0qO9SnDpox44DhDXwrWR80ZaAsIBcABB6s,4017
-sif_tools-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-sif_tools-0.3.0.dist-info/entry_points.txt,sha256=DqG3nDHpwF6a9Pi-8ic6LnI9j5GbrFF-VZHepRl22HM,54
-sif_tools-0.3.0.dist-info/top_level.txt,sha256=8EV42y0oQ9ntR0iu1o7m8YbEoQeY9FvOzrc1RJhEgzo,10
-sif_tools-0.3.0.dist-info/RECORD,,
+sif_tools-0.3.1.dist-info/LICENSE,sha256=baLxFkeB7Yhvfd2bvZHGsxrX8T_0FeM0SOf8iPapzw8,14874
+sif_tools-0.3.1.dist-info/METADATA,sha256=-0rajaoioj6jqyh7CfCOLbisXDheljQUIudJxouB0D0,4100
+sif_tools-0.3.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+sif_tools-0.3.1.dist-info/entry_points.txt,sha256=DqG3nDHpwF6a9Pi-8ic6LnI9j5GbrFF-VZHepRl22HM,54
+sif_tools-0.3.1.dist-info/top_level.txt,sha256=8EV42y0oQ9ntR0iu1o7m8YbEoQeY9FvOzrc1RJhEgzo,10
+sif_tools-0.3.1.dist-info/RECORD,,
```

