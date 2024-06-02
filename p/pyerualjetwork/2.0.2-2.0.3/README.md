# Comparing `tmp/pyerualjetwork-2.0.2.tar.gz` & `tmp/pyerualjetwork-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-2.0.2.tar", last modified: Sun Jun  2 19:04:22 2024, max compression
+gzip compressed data, was "pyerualjetwork-2.0.3.tar", last modified: Sun Jun  2 20:10:17 2024, max compression
```

## Comparing `pyerualjetwork-2.0.2.tar` & `pyerualjetwork-2.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 19:04:22.387241 pyerualjetwork-2.0.2/
--rw-rw-rw-   0        0        0      429 2024-06-02 19:04:22.386244 pyerualjetwork-2.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-02 19:04:22.361099 pyerualjetwork-2.0.2/plan/
--rw-rw-rw-   0        0        0      377 2024-06-02 19:03:35.000000 pyerualjetwork-2.0.2/plan/__init__.py
--rw-rw-rw-   0        0        0    33061 2024-06-02 18:28:02.000000 pyerualjetwork-2.0.2/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-06-02 19:04:22.383254 pyerualjetwork-2.0.2/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      429 2024-06-02 19:04:21.000000 pyerualjetwork-2.0.2/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-06-02 19:04:22.000000 pyerualjetwork-2.0.2/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 19:04:21.000000 pyerualjetwork-2.0.2/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-06-02 19:04:21.000000 pyerualjetwork-2.0.2/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-02 19:04:22.388240 pyerualjetwork-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      608 2024-06-02 19:04:06.000000 pyerualjetwork-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:10:17.316032 pyerualjetwork-2.0.3/
+-rw-rw-rw-   0        0        0      429 2024-06-02 20:10:17.315028 pyerualjetwork-2.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 20:10:17.291034 pyerualjetwork-2.0.3/plan/
+-rw-rw-rw-   0        0        0      377 2024-06-02 19:03:35.000000 pyerualjetwork-2.0.3/plan/__init__.py
+-rw-rw-rw-   0        0        0    32839 2024-06-02 20:09:22.000000 pyerualjetwork-2.0.3/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-06-02 20:10:17.311980 pyerualjetwork-2.0.3/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      429 2024-06-02 20:10:16.000000 pyerualjetwork-2.0.3/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-06-02 20:10:17.000000 pyerualjetwork-2.0.3/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 20:10:16.000000 pyerualjetwork-2.0.3/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-06-02 20:10:16.000000 pyerualjetwork-2.0.3/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 20:10:17.317035 pyerualjetwork-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      608 2024-06-02 20:10:07.000000 pyerualjetwork-2.0.3/setup.py
```

### Comparing `pyerualjetwork-2.0.2/plan/plan.py` & `pyerualjetwork-2.0.3/plan/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,34 +12,30 @@
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 # BUILD -----
 def fit(
     x_train: List[Union[int, float]],
     y_train: List[Union[int, float, str]], # At least two.. and one hot encoded
-    action_potential: List[Union[int, float]],
+    action_potential: Union[float],
 ) -> str:
         
     infoPLAN = """
     Creates and configures a PLAN model.
     
     Args:
         x_train (list[num]): List of input data.
         y_train (list[num]): List of y_train. (one hot encoded)
         action_potential (float): Input ACTION potential 
     
     Returns:
         list([num]): (Weight matrices list, train_predictions list, Trainacc).
         error handled ?: Process status ('e')
 """
-    if action_potential < 0 or action_potential > 1:
-        
-        print(Fore.RED + "ERROR101: ACTION potential value must be in range 0-1. from: fit",infoPLAN)
-        return 'e'
-        
+
     if len(x_train) != len(y_train):
        print(Fore.RED + "ERROR301: x_train list and y_train list must be same length. from: fit",infoPLAN)
        return 'e'
    
     class_count = set()
     for sublist in y_train:
       
@@ -47,15 +43,15 @@
     
     
     class_count = list(class_count)
     
     y_train = [tuple(sublist) for sublist in y_train]
     
     neurons = [len(class_count),len(class_count)]
-    layers = ['fex', 'cat']
+    layers = ['fex','cat']
     
     x_train[0] = np.array(x_train[0])
     x_train[0] = x_train[0].ravel()
     x_train_size = len(x_train[0])
     
     W = weight_identification(len(layers) - 1,len(class_count),neurons,x_train_size)
     Divides, Piece = synaptic_dividing(len(class_count),W)
@@ -89,15 +85,16 @@
 
         neural_layer = inp
         
         for Lindex, Layer in enumerate(layers):
             
             
             neural_layer = normalization(neural_layer)
-                
+            
+
             if Layer == 'fex':
                 neural_layer,W[Lindex] = fex(neural_layer, W[Lindex], action_potential, Piece[Windex], 1)
             elif Layer == 'cat':
                 neural_layer,W[Lindex] = cat(neural_layer, W[Lindex], action_potential, 1, Piece[Windex])
                 
         RealOutput = np.argmax(y_train[index])
         PredictedOutput = np.argmax(neural_layer)
@@ -359,15 +356,15 @@
         action_potential (num): Threshold value for comparison.
         isTrain (int): Flag indicating if the function is called during training (1 for training, 0 otherwise).
 
     Returns:
         tuple: A tuple containing the neural layer (vector) result and the possibly updated weight matrix.
     """
    
-    PruneIndex = np.where(Input == action_potential)
+    PruneIndex = np.where(Input == 0)
     
     if isTrain == 1:
      
         w = synaptic_pruning(w, PruneIndex, 'col', 0, 0, piece, isTrain)
      
     
     neural_layer = np.dot(w, Input)
@@ -969,8 +966,8 @@
     
 def get_acc():
         
     return 2
 
 def get_pot():
     
-    return 1
+    return 1
```

### Comparing `pyerualjetwork-2.0.2/setup.py` & `pyerualjetwork-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "2.0.2",
+      version = "2.0.3",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
       description= "Advanced python deep learning library. New features: More simple and practical, all functions and variables are snake_case. (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
```

