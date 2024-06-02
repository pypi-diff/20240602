# Comparing `tmp/retailtree-1.2.tar.gz` & `tmp/retailtree-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retailtree-1.2.tar", last modified: Wed May 15 14:17:30 2024, max compression
+gzip compressed data, was "retailtree-1.3.tar", last modified: Sun Jun  2 18:39:10 2024, max compression
```

## Comparing `retailtree-1.2.tar` & `retailtree-1.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:30.537652 retailtree-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-15 14:17:30.537652 retailtree-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-15 14:17:23.000000 retailtree-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:30.533652 retailtree-1.2/retailtree/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 14:17:23.000000 retailtree-1.2/retailtree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:30.537652 retailtree-1.2/retailtree/logics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:23.000000 retailtree-1.2/retailtree/logics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-15 14:17:23.000000 retailtree-1.2/retailtree/logics/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-15 14:17:23.000000 retailtree-1.2/retailtree/logics/right_left.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-15 14:17:23.000000 retailtree-1.2/retailtree/logics/top_bottom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-15 14:17:23.000000 retailtree-1.2/retailtree/logics/vp_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-15 14:17:23.000000 retailtree-1.2/retailtree/retailtree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:30.537652 retailtree-1.2/retailtree/structs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:23.000000 retailtree-1.2/retailtree/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-15 14:17:23.000000 retailtree-1.2/retailtree/structs/annotation_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:30.537652 retailtree-1.2/retailtree/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:23.000000 retailtree-1.2/retailtree/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-15 14:17:23.000000 retailtree-1.2/retailtree/utils/dist_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:30.537652 retailtree-1.2/retailtree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-15 14:17:30.000000 retailtree-1.2/retailtree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-15 14:17:30.000000 retailtree-1.2/retailtree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:17:30.000000 retailtree-1.2/retailtree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 14:17:30.000000 retailtree-1.2/retailtree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 14:17:30.000000 retailtree-1.2/retailtree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:17:30.537652 retailtree-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 14:17:23.000000 retailtree-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:30.537652 retailtree-1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:23.000000 retailtree-1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-15 14:17:23.000000 retailtree-1.2/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:39:10.024171 retailtree-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-06-02 18:39:10.024171 retailtree-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-06-02 18:39:00.000000 retailtree-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:39:10.020171 retailtree-1.3/retailtree/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-02 18:39:00.000000 retailtree-1.3/retailtree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:39:10.020171 retailtree-1.3/retailtree/logics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:39:00.000000 retailtree-1.3/retailtree/logics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-06-02 18:39:00.000000 retailtree-1.3/retailtree/logics/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-06-02 18:39:00.000000 retailtree-1.3/retailtree/logics/right_left.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-06-02 18:39:00.000000 retailtree-1.3/retailtree/logics/top_bottom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-06-02 18:39:00.000000 retailtree-1.3/retailtree/logics/vp_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-06-02 18:39:00.000000 retailtree-1.3/retailtree/retailtree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:39:10.020171 retailtree-1.3/retailtree/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:39:00.000000 retailtree-1.3/retailtree/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-06-02 18:39:00.000000 retailtree-1.3/retailtree/structs/annotation_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:39:10.020171 retailtree-1.3/retailtree/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:39:00.000000 retailtree-1.3/retailtree/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-02 18:39:00.000000 retailtree-1.3/retailtree/utils/dist_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:39:10.024171 retailtree-1.3/retailtree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-06-02 18:39:10.000000 retailtree-1.3/retailtree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-06-02 18:39:10.000000 retailtree-1.3/retailtree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:39:10.000000 retailtree-1.3/retailtree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 18:39:10.000000 retailtree-1.3/retailtree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-02 18:39:10.000000 retailtree-1.3/retailtree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:39:10.024171 retailtree-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-06-02 18:39:00.000000 retailtree-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:39:10.024171 retailtree-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:39:00.000000 retailtree-1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-06-02 18:39:00.000000 retailtree-1.3/tests/test_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-06-02 18:39:00.000000 retailtree-1.3/tests/test_tblr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-06-02 18:39:00.000000 retailtree-1.3/tests/test_wa.py
```

### Comparing `retailtree-1.2/PKG-INFO` & `retailtree-1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: retailtree
-Version: 1.2
-Description-Content-Type: text/markdown
-Requires-Dist: numpy
-
 # RetailTree
 
 RetailTree is a Python library designed for efficient management and querying of spatial data utilizing a tree-based data structure. Specifically, RetailTree employs a VP (Vantage Point) tree for optimized spatial data management.
 
 # Key Features
 
 - Nearest Neighbor Search: RetailTree enables finding the nearest neighbors in 2D space.
@@ -16,50 +10,86 @@
   Supports retrieval of annotations based on their relative positions.
 - Annotations within Angle Range: Provides functionality to retrieve annotations within a specified angle range relative to a reference point.
 
 # Installation
 
 You can install retailTree via pip:
 
-```
+```python
 pip install retailtree
 ```
 
 # Usage
 
-```
+### Import necessary modules and functions
+
+```python
+# Imports
 from retailtree import RetailTree, Annotation
 from retailtree.utils.dist_func import manhattan, euclidean
+import json
+```
+
+### Sample Usage 1: Creating Annotations with Annotation Class using a sample JSON file
 
+```python
+# Define the path to the JSON file containing annotations
+file_path = './tests/test_data/test_data.json'
+
+# Open and load the JSON file
+with open(file_path, 'r') as file:
+    annotations = json.load(file)
+
+# Initialize a RetailTree object
+rt = RetailTree()
+
+# Iterate over the loaded annotations and create Annotation objects
+for ann in annotations:
+    # Create an Annotation object with the required properties
+    ann_obj = Annotation(id=ann['id'], x_min=ann['x_min'], y_min=ann['y_min'], x_max=ann['x_max'], y_max=ann['y_max'])
+    # Add the created Annotation object to the RetailTree
+    rt.add_annotation(ann_obj)
+```
+
+# OR
+
+### Sample Usage 2: Creating Annotations with Annotation Class
+
+```python
 # Create annotation object
 ann1 = Annotation(id=1, x_min=2, y_min=1, x_max=3, y_max=2)
-    ann2 = Annotation(id=2, x_min=1, y_min=2, x_max=2, y_max=3)
-    ann3 = Annotation(id=3, x_min=2, y_min=2, x_max=3, y_max=3)
-    ann4 = Annotation(id=4, x_min=3, y_min=2, x_max=4, y_max=3)
-    ann5 = Annotation(id=5, x_min=2, y_min=3, x_max=3, y_max=4)
-
+ann2 = Annotation(id=2, x_min=1, y_min=2, x_max=2, y_max=3)
+ann3 = Annotation(id=3, x_min=2, y_min=2, x_max=3, y_max=3)
+ann4 = Annotation(id=4, x_min=3, y_min=2, x_max=4, y_max=3)
+ann5 = Annotation(id=5, x_min=2, y_min=3, x_max=3, y_max=4)
 annotations = [ann1, ann2, ann3, ann4, ann5]
 
 # Create retailtree object
 rt = RetailTree()
 
 # Adding annotations to retailtree
 for ann in annotations:
   rt.add_annotation(ann)
+```
 
+## Building the Tree and Querying
 
-# Build tree
-rt.build_tree(dist_func=euclidean)
+### Building the Tree
 
-# Get neighbors-annotations within radius
+```python
+# Build the retail tree structure using the euclidean distance function
+rt.build_tree(dist_func=euclidean)
+```
+### Querying the Tree
+```python
+# Retrieve and print annotations within a radius.
 print(rt.neighbors(id=3, radius=1))
 
-# Get Top, Bottom, Right, Left annotations
+# Retrieve and print the Top, Bottom, Left, and Right neighboring annotations.
 print(rt.TBLR(id=3, radius=1, overlap=0.5))
 
-# Get neighboring annotations within a particular angle range
-print(rt.neighbors_wa(id=3, radius=1, amin=0, amax=180))
+# Retrieve and print neighboring annotations of the annotation.
+print(rt.neighbors_wa(id=3, radius=2, amin=0, amax=180))
 
-# Get annotation properties
+# Retrieve and print the coordinates of the annotation.
 print(rt.get(id=3).get_coords())
-
 ```
```

### Comparing `retailtree-1.2/retailtree/logics/overlap.py` & `retailtree-1.3/retailtree/logics/overlap.py`

 * *Files identical despite different names*

### Comparing `retailtree-1.2/retailtree/logics/right_left.py` & `retailtree-1.3/retailtree/logics/right_left.py`

 * *Files identical despite different names*

### Comparing `retailtree-1.2/retailtree/logics/top_bottom.py` & `retailtree-1.3/retailtree/logics/top_bottom.py`

 * *Files identical despite different names*

### Comparing `retailtree-1.2/retailtree/logics/vp_tree.py` & `retailtree-1.3/retailtree/logics/vp_tree.py`

 * *Files identical despite different names*

### Comparing `retailtree-1.2/retailtree/retailtree.py` & `retailtree-1.3/retailtree/retailtree.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,25 +53,21 @@
 
         obj = VPTree(annotations, dist_func)
         self.tree = obj
 
     def __get_neighbors_radius(self):
         """
         Method to get the radius within which neighbors will be searched for.
-        If number of annotations is greater than 10, random annotations are considered.
-
         Radius is the max of the diagonals of the annotations considered.
         """
         radius = self.__neighbors_radius
         if not radius:
             annotation_bucket = list(self.annotations.values())
-            if len(annotation_bucket) > 10:
-                random_annotations = sample(annotation_bucket, 10)
-            else:
-                random_annotations = annotation_bucket
+
+            random_annotations = annotation_bucket
             distance = [math.sqrt(pow(annotation.width, 2) + pow(
                 annotation.length, 2)) for annotation in random_annotations]
             radius = max(distance)
             self.__neighbors_radius = radius
         return radius
 
     def __fetch_neighbors(self, id: int, radius=1):
```

### Comparing `retailtree-1.2/retailtree/structs/annotation_struct.py` & `retailtree-1.3/retailtree/structs/annotation_struct.py`

 * *Files identical despite different names*

### Comparing `retailtree-1.2/retailtree.egg-info/PKG-INFO` & `retailtree-1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retailtree
-Version: 1.2
+Version: 1.3
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
 # RetailTree
 
 RetailTree is a Python library designed for efficient management and querying of spatial data utilizing a tree-based data structure. Specifically, RetailTree employs a VP (Vantage Point) tree for optimized spatial data management.
 
@@ -16,50 +16,86 @@
   Supports retrieval of annotations based on their relative positions.
 - Annotations within Angle Range: Provides functionality to retrieve annotations within a specified angle range relative to a reference point.
 
 # Installation
 
 You can install retailTree via pip:
 
-```
+```python
 pip install retailtree
 ```
 
 # Usage
 
-```
+### Import necessary modules and functions
+
+```python
+# Imports
 from retailtree import RetailTree, Annotation
 from retailtree.utils.dist_func import manhattan, euclidean
+import json
+```
+
+### Sample Usage 1: Creating Annotations with Annotation Class using a sample JSON file
+
+```python
+# Define the path to the JSON file containing annotations
+file_path = './tests/test_data/test_data.json'
+
+# Open and load the JSON file
+with open(file_path, 'r') as file:
+    annotations = json.load(file)
+
+# Initialize a RetailTree object
+rt = RetailTree()
+
+# Iterate over the loaded annotations and create Annotation objects
+for ann in annotations:
+    # Create an Annotation object with the required properties
+    ann_obj = Annotation(id=ann['id'], x_min=ann['x_min'], y_min=ann['y_min'], x_max=ann['x_max'], y_max=ann['y_max'])
+    # Add the created Annotation object to the RetailTree
+    rt.add_annotation(ann_obj)
+```
+
+# OR
 
+### Sample Usage 2: Creating Annotations with Annotation Class
+
+```python
 # Create annotation object
 ann1 = Annotation(id=1, x_min=2, y_min=1, x_max=3, y_max=2)
-    ann2 = Annotation(id=2, x_min=1, y_min=2, x_max=2, y_max=3)
-    ann3 = Annotation(id=3, x_min=2, y_min=2, x_max=3, y_max=3)
-    ann4 = Annotation(id=4, x_min=3, y_min=2, x_max=4, y_max=3)
-    ann5 = Annotation(id=5, x_min=2, y_min=3, x_max=3, y_max=4)
-
+ann2 = Annotation(id=2, x_min=1, y_min=2, x_max=2, y_max=3)
+ann3 = Annotation(id=3, x_min=2, y_min=2, x_max=3, y_max=3)
+ann4 = Annotation(id=4, x_min=3, y_min=2, x_max=4, y_max=3)
+ann5 = Annotation(id=5, x_min=2, y_min=3, x_max=3, y_max=4)
 annotations = [ann1, ann2, ann3, ann4, ann5]
 
 # Create retailtree object
 rt = RetailTree()
 
 # Adding annotations to retailtree
 for ann in annotations:
   rt.add_annotation(ann)
+```
 
+## Building the Tree and Querying
 
-# Build tree
-rt.build_tree(dist_func=euclidean)
+### Building the Tree
 
-# Get neighbors-annotations within radius
+```python
+# Build the retail tree structure using the euclidean distance function
+rt.build_tree(dist_func=euclidean)
+```
+### Querying the Tree
+```python
+# Retrieve and print annotations within a radius.
 print(rt.neighbors(id=3, radius=1))
 
-# Get Top, Bottom, Right, Left annotations
+# Retrieve and print the Top, Bottom, Left, and Right neighboring annotations.
 print(rt.TBLR(id=3, radius=1, overlap=0.5))
 
-# Get neighboring annotations within a particular angle range
-print(rt.neighbors_wa(id=3, radius=1, amin=0, amax=180))
+# Retrieve and print neighboring annotations of the annotation.
+print(rt.neighbors_wa(id=3, radius=2, amin=0, amax=180))
 
-# Get annotation properties
+# Retrieve and print the coordinates of the annotation.
 print(rt.get(id=3).get_coords())
-
 ```
```

### Comparing `retailtree-1.2/tests/tests.py` & `retailtree-1.3/tests/test_tblr.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import json
 
 
 class TestAnnotation(unittest.TestCase):
 
     def setUp(self):
         # Build tree before every test case
-        file_path = './tests/test_data/ideal_test_data.json'
-        file_path_output = './tests/test_data/output_ideal_test_data.json'
+        file_path = './tests/test_data/test_data.json'
+        file_path_output = './tests/test_data/tblr_output.json'
         # Annotations data2
         with open(file_path, 'r') as file:
             self.annotation_data_json = json.load(file)
 
         with open(file_path_output, 'r') as file:
             self.annotation_output_data = json.load(file)
 
@@ -21,50 +21,50 @@
             ann = Annotation(data['id'], data['x_min'],
                              data['y_min'], data['x_max'], data['y_max'])
             self.RT.add_annotation(ann)
 
         self.RT.build_tree()
         self.assertIsNotNone(self.RT.tree)
 
-    def test_find_neighbors_0(self):
+    def test_tblr_0(self):
         self.assertEqual(self.RT.TBLR(
             id=0, radius=2), self.annotation_output_data[0])
 
-    def test_find_neighbors_1(self):
+    def test_tblr_1(self):
         self.assertEqual(self.RT.TBLR(
             id=1, radius=2), self.annotation_output_data[1])
 
-    def test_find_neighbors_2(self):
+    def test_tblr_2(self):
         self.assertEqual(self.RT.TBLR(
             id=2, radius=2), self.annotation_output_data[2])
 
-    def test_find_neighbors_3(self):
+    def test_tblr_3(self):
         self.assertEqual(self.RT.TBLR(
             id=3, radius=2), self.annotation_output_data[3])
 
-    def test_find_neighbors_4(self):
+    def test_tblr_4(self):
         self.assertEqual(self.RT.TBLR(
             id=4, radius=2), self.annotation_output_data[4])
 
-    def test_find_neighbors_5(self):
+    def test_tblr_5(self):
         self.assertEqual(self.RT.TBLR(
             id=5, radius=2), self.annotation_output_data[5])
 
-    def test_find_neighbors_6(self):
+    def test_tblr_6(self):
         self.assertEqual(self.RT.TBLR(
             id=6, radius=2), self.annotation_output_data[6])
 
-    def test_find_neighbors_7(self):
+    def test_tblr_7(self):
         self.assertEqual(self.RT.TBLR(
             id=7, radius=2), self.annotation_output_data[7])
 
-    def test_find_neighbors_8(self):
+    def test_tblr_8(self):
         self.assertEqual(self.RT.TBLR(
             id=8, radius=2), self.annotation_output_data[8])
 
-    def test_find_neighbors_9(self):
+    def test_tblr_9(self):
         self.assertEqual(self.RT.TBLR(
             id=9, radius=2), self.annotation_output_data[9])
 
 
 if __name__ == '__main__':
     unittest.main()
```

