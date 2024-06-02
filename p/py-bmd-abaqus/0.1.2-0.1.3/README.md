# Comparing `tmp/py_bmd_abaqus-0.1.2.tar.gz` & `tmp/py_bmd_abaqus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_bmd_abaqus-0.1.2.tar", max compression
+gzip compressed data, was "py_bmd_abaqus-0.1.3.tar", max compression
```

## Comparing `py_bmd_abaqus-0.1.2.tar` & `py_bmd_abaqus-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1108 2024-05-30 14:32:06.865334 py_bmd_abaqus-0.1.2/LICENSE
--rw-r--r--   0        0        0    23671 2024-05-30 23:14:21.581390 py_bmd_abaqus-0.1.2/py_BMD_abaqus.py
--rw-r--r--   0        0        0      862 2024-05-30 23:20:42.193881 py_bmd_abaqus-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1663 2024-05-29 21:02:24.848944 py_bmd_abaqus-0.1.2/README.md
--rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 py_bmd_abaqus-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1108 2024-05-30 14:32:06.865334 py_bmd_abaqus-0.1.3/LICENSE
+-rw-r--r--   0        0        0    23737 2024-06-01 02:53:40.334318 py_bmd_abaqus-0.1.3/py_BMD_abaqus.py
+-rw-r--r--   0        0        0      862 2024-06-02 05:04:54.837993 py_bmd_abaqus-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1663 2024-05-29 21:02:24.848944 py_bmd_abaqus-0.1.3/README.md
+-rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 py_bmd_abaqus-0.1.3/PKG-INFO
```

### Comparing `py_bmd_abaqus-0.1.2/LICENSE` & `py_bmd_abaqus-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_bmd_abaqus-0.1.2/py_BMD_abaqus.py` & `py_bmd_abaqus-0.1.3/py_BMD_abaqus.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             line = line.strip()
             # Check for section headers
             if "*Node" in line:
                 current_section = "node"
             elif "*Element" in line:
                 current_section = "element"
 
-            if any(keyword in line for keyword in ["*Nset", "*Elset", "*End", "*Assembly"]):
+            if any(keyword in line for keyword in ["*Nset", "*Elset", "*End", "*Assembly"]) and current_section == "Element":
                 done = True
 
             if done == False:
                 # Process lines based on the current section
                 if current_section == "node" and not (line.startswith("*Node") or "*End " in line or "0.,           0.,           0." in line):
                     # Split the line into columns and convert to NumPy array
                     node_info = np.array(line.split(','), dtype=float)
@@ -283,15 +283,15 @@
             line = line.strip()
             # Check for section headers
             if "*Node" in line:
                 current_section = "node"
             elif "*Element" in line:
                 current_section = "element"
 
-            if any(keyword in line for keyword in ["*Nset", "*Elset", "*End", "*Assembly"]):
+            if any(keyword in line for keyword in ["*Nset", "*Elset", "*End", "*Assembly"]) and current_section == "Element":
                 done = True
 
             if done == False:
                 # Process lines based on the current section
                 if current_section == "node" and not (line.startswith("*Node") or "*End " in line or "0.,           0.,           0." in line):
                     # Split the line into columns and convert to NumPy array
                     node_info = np.array(line.split(','), dtype=float)
```

### Comparing `py_bmd_abaqus-0.1.2/pyproject.toml` & `py_bmd_abaqus-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-bmd-abaqus"
-version = "0.1.2"
+version = "0.1.3"
 description = "This library was created in order to assign trabecular bone material property values to an ABAQUS CAE input mesh file (INP). This script uses the \"Pooled\" Morgan et al. Modulus-Density relationship - retrieved from DOI: 10.1016/s0021-9290(03)00071-x in order to calculate material modulus from density in g/cm^3. This tool also returns an array of element HU, density, or modulus values which can be used to easy evaluation of bone quality in the meshed region."
 authors = ["Dr. David E. Cunningham, Ph.D."]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `py_bmd_abaqus-0.1.2/README.md` & `py_bmd_abaqus-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `py_bmd_abaqus-0.1.2/PKG-INFO` & `py_bmd_abaqus-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-bmd-abaqus
-Version: 0.1.2
+Version: 0.1.3
 Summary: This library was created in order to assign trabecular bone material property values to an ABAQUS CAE input mesh file (INP). This script uses the "Pooled" Morgan et al. Modulus-Density relationship - retrieved from DOI: 10.1016/s0021-9290(03)00071-x in order to calculate material modulus from density in g/cm^3. This tool also returns an array of element HU, density, or modulus values which can be used to easy evaluation of bone quality in the meshed region.
 License: MIT
 Author: Dr. David E. Cunningham, Ph.D.
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

