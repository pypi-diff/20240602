# Comparing `tmp/pyerualjetwork-1.3.9.tar.gz` & `tmp/pyerualjetwork-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.3.9.tar", last modified: Fri May 31 06:14:59 2024, max compression
+gzip compressed data, was "pyerualjetwork-2.0.tar", last modified: Sun Jun  2 18:33:15 2024, max compression
```

## Comparing `pyerualjetwork-1.3.9.tar` & `pyerualjetwork-2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 06:14:59.481341 pyerualjetwork-1.3.9/
--rw-rw-rw-   0        0        0      391 2024-05-31 06:14:59.480344 pyerualjetwork-1.3.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-31 06:14:59.415131 pyerualjetwork-1.3.9/plan/
--rw-rw-rw-   0        0        0      375 2024-05-29 18:09:13.000000 pyerualjetwork-1.3.9/plan/__init__.py
--rw-rw-rw-   0        0        0    44861 2024-05-31 01:55:55.000000 pyerualjetwork-1.3.9/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-31 06:14:59.476358 pyerualjetwork-1.3.9/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      391 2024-05-31 06:14:58.000000 pyerualjetwork-1.3.9/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-31 06:14:58.000000 pyerualjetwork-1.3.9/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 06:14:58.000000 pyerualjetwork-1.3.9/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-31 06:14:58.000000 pyerualjetwork-1.3.9/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 06:14:59.481341 pyerualjetwork-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0      570 2024-05-31 01:16:47.000000 pyerualjetwork-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:33:15.715473 pyerualjetwork-2.0/
+-rw-rw-rw-   0        0        0      427 2024-06-02 18:33:15.713478 pyerualjetwork-2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-02 18:33:15.682059 pyerualjetwork-2.0/plan/
+-rw-rw-rw-   0        0        0      375 2024-06-02 18:31:11.000000 pyerualjetwork-2.0/plan/__init__.py
+-rw-rw-rw-   0        0        0    33061 2024-06-02 18:28:02.000000 pyerualjetwork-2.0/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:33:15.711494 pyerualjetwork-2.0/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      427 2024-06-02 18:33:14.000000 pyerualjetwork-2.0/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-06-02 18:33:15.000000 pyerualjetwork-2.0/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 18:33:14.000000 pyerualjetwork-2.0/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-06-02 18:33:14.000000 pyerualjetwork-2.0/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 18:33:15.716470 pyerualjetwork-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      606 2024-06-02 18:32:45.000000 pyerualjetwork-2.0/setup.py
```

### Comparing `pyerualjetwork-1.3.9/plan/plan.py` & `pyerualjetwork-2.0/plan/plan.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,237 +9,112 @@
 from typing import List, Union
 import math
 from scipy.special import expit, softmax
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 # BUILD -----
-def TrainPLAN(
-    x_train: List[Union[int, float]], 
+def fit(
+    x_train: List[Union[int, float]],
     y_train: List[Union[int, float, str]], # At least two.. and one hot encoded
-    class_count: int,
-    layers: List[str],
-    neurons: List[Union[int, float]],
-    membran_thresholds: List[str],
-    membran_potentials: List[Union[int, float]],
-    normalizations: List[str],
-    activations: List[str],
-    visualize: str
+    action_potential: List[Union[int, float]],
 ) -> str:
         
     infoPLAN = """
     Creates and configures a PLAN model.
     
     Args:
         x_train (list[num]): List of input data.
         y_train (list[num]): List of y_train. (one hot encoded)
-        class_count (int): Number of classes.
-        layers (list[str]): List of layer names. (options: 'fex' (Feature Extraction), 'cat' (Catalyser))
-        neurons (list[num]): List of neuron counts for each layer.
-        membran_thresholds (list[str]): List of membran_thresholds.
-        membran_potentials (list[num]): List of membran_potentials.
-        normalizations (List[str]): Whether normalization will be performed at indexed layers ("y" or "n").
-        activations (list[str]): List of activation functions.
-        visualize (str): visualize Training procces or not visualize ('y' or 'n')
+        action_potential (float): Input ACTION potential 
     
     Returns:
         list([num]): (Weight matrices list, train_predictions list, Trainacc).
         error handled ?: Process status ('e')
 """
+    if action_potential < 0 or action_potential > 1:
         
-    if visualize != 'y' and visualize != 'n':
-        print(Fore.RED + "ERROR109: visualize parameter must be 'y' or 'n'. TrainPLAN",infoPLAN)
+        print(Fore.RED + "ERROR101: ACTION potential value must be in range 0-1. from: fit",infoPLAN)
         return 'e'
         
-    
-    LastNeuron = neurons[-1:][0]
-    if LastNeuron != class_count:
-            print(Fore.RED + "ERROR108: Last layer of neuron count must be equal class count. from: TrainPLAN",infoPLAN)
-            return 'e'
-    
-    if len(normalizations) != len(membran_potentials):
-        
-            print(Fore.RED + "ERROR307: Normalization list length must be equal to length of membran_thresholds List,membran_potentials List,layers List,neurons List. from: TrainPLAN",infoPLAN)
-            return 'e'
-    
     if len(x_train) != len(y_train):
-        print(Fore.RED + "ERROR301: x_train list and y_train list must be same length.",infoPLAN)
-        return 'e'
-    
-    for i, Value in enumerate(membran_potentials):
-        
-        if normalizations[i] != 'y' and normalizations[i] != 'n':
-                print(Fore.RED + "ERROR105: Normalization list must be 'y' or 'n'.",infoPLAN)
-                return 'e'
-            
-        if membran_thresholds[i] == 'none':
-            print(Fore.MAGENTA + "WARNING102: We are advise to do not put 'none' Threshold sign. But some cases improves performance of the model from: TrainPLAN",infoPLAN  + Style.RESET_ALL)
-            time.sleep(3)
-            
-        if isinstance(Value, str):
-            print(Fore.RED + "ERROR201: MEMBRAN POTENTIALS must be numeric. from: TrainPLAN")
-            return 'e'
-        
-        if isinstance(neurons[i], str):
-            print(Fore.RED + "ERROR202: neurons list must be numeric.")
-            return 'e'
-    
-    if len(membran_thresholds) != len(membran_potentials):
-        print(Fore.RED + "ERROR302: MEMBRAN THRESHOLDS list and MEMBRAN POTENTIALS list must be same length. from: TrainPLAN",infoPLAN)
-        return 'e'
-    
-    if len(layers) != len(neurons):
-        print(Fore.RED + "ERROR303: layers list and neurons list must same length. from: TrainPLAN",infoPLAN)
-        return 'e'
-    
-    if len(membran_potentials) != len(layers) or len(membran_thresholds) != len(layers):
-        print(Fore.RED + "ERROR306: MEMBRAN POTENTIALS and MEMBRAN THRESHOLDS lists length must be same layers list length. from: TrainPLAN",infoPLAN)
-        return 'e'
-    
-    
-    for Activation in activations:
-        if Activation != 'softmax' and Activation != 'sigmoid' and Activation != 'relu' and Activation != 'none':
-            print(Fore.RED + "ERROR108: activations list must be 'sigmoid' or 'softmax' or 'relu' or 'none' from: TrainPLAN",infoPLAN)
-            return 'e'
-    
-
-    for index, Neuron in enumerate(neurons):
-        if Neuron < 1:
-            print(Fore.RED + "ERROR101: neurons list must be positive non zero integer. from: TrainPLAN",infoPLAN)
-            return 'e'
-        
-        if index + 1 != len(neurons) and Neuron % 2 != 0:
-            print(Fore.MAGENTA + "WARNING101: We strongly advise to do Neuron counts be should even numbers. from: TrainPLAN",infoPLAN)
-            time.sleep(3)
-            
-        if Neuron < class_count:
-            print(Fore.RED + "ERROR102: Neuron count must be greater than class count(For PLAN). from: TrainPLAN")
-            return 'e'
-        
-        if layers[index] != 'fex' and layers[index] != 'cat':
-            print(Fore.RED + "ERROR107: layers list must be 'fex'(Feature Extraction Layer) or 'cat' (Catalyser Layer). from: TrainPLAN",infoPLAN)
-            return 'e'
-    
-    if len(membran_thresholds) != len(membran_potentials):
-        print(Fore.RED + "ERROR305: MEMBRAN THRESHOLDS list and MEMBRAN POTENTIALS list must be same length. from: TrainPLAN",infoPLAN)
-        return 'e'
-    
-    
-    for i, Sign in enumerate(membran_thresholds):
-        if Sign != '>' and Sign != '<' and Sign != '==' and Sign != '!=' and Sign != 'none':
-            print(Fore.RED + "ERROR104: MEMBRAN THRESHOLDS must be '>' or '<' or '==' or '!='. or 'none' WE SUGGEST '<' FOR FEX LAYER AND '==' FOR CAT LAYER (Your data, your hyperparameter) from: TrainPLAN",infoPLAN)
-            return 'e'
-        
-        if layers[i] == 'fex' and Sign == 'none':
-            print(Fore.RED + "ERROR109: at layer type 'fex', pairing with 'none' Threshold is not acceptlable. if you want to 'none' put '==' and make threshold value '0'. from: TrainPLAN ",infoPLAN)
-            return 'e'
-        
-    Uniquey_train = set()
+       print(Fore.RED + "ERROR301: x_train list and y_train list must be same length. from: fit",infoPLAN)
+       return 'e'
+   
+    class_count = set()
     for sublist in y_train:
       
-        Uniquey_train.add(tuple(sublist))
+        class_count.add(tuple(sublist))
     
     
-    Uniquey_train = list(Uniquey_train)
+    class_count = list(class_count)
     
     y_train = [tuple(sublist) for sublist in y_train]
     
-    
-    if len(Uniquey_train) != class_count:
-        print(Fore.RED + "ERROR106: Label variety length must be same Class Count. from: TrainPLAN",infoPLAN)
-        return 'e'
+    neurons = [len(class_count),len(class_count)]
+    layers = ['fex', 'cat']
     
     x_train[0] = np.array(x_train[0])
     x_train[0] = x_train[0].ravel()
     x_train_size = len(x_train[0])
     
-    W = WeightIdentification(len(layers) - 1,class_count,neurons,x_train_size)
-    Divides, Piece = SynapticDividing(class_count,W)
+    W = weight_identification(len(layers) - 1,len(class_count),neurons,x_train_size)
+    Divides, Piece = synaptic_dividing(len(class_count),W)
     trained_W = [1] * len(W)
     print(Fore.GREEN + "Train Started with 0 ERROR" + Style.RESET_ALL,)
     train_predictions = [None] * len(y_train)
     true = 0
     start_time = time.time()
     for index, inp in enumerate(x_train):
         uni_start_time = time.time()
         inp = np.array(inp)
         inp = inp.ravel()
         
         if x_train_size != len(inp):
-            print(Fore.RED +"ERROR304: All input matrices or vectors in x_train list, must be same size. from: TrainPLAN",infoPLAN + Style.RESET_ALL)
+            print(Fore.RED +"ERROR304: All input matrices or vectors in x_train list, must be same size. from: fit",infoPLAN + Style.RESET_ALL)
             return 'e'
         
         
-        for Ulindex, Ul in enumerate(Uniquey_train):
+        for Ulindex, Ul in enumerate(class_count):
             
             if Ul == y_train[index]:
                 for Windex, w in enumerate(W):
                     for i, ul in enumerate(Ul):
                         if ul == 1.0:
                             k = i
 
                     cs = Divides[int(k)][Windex][0]
 
        
-                    W[Windex] = SynapticPruning(w, cs, 'row', int(k),class_count,Piece[Windex],1)
+                    W[Windex] = synaptic_pruning(w, cs, 'row', int(k),len(class_count),Piece[Windex],1)
 
         neural_layer = inp
         
         for Lindex, Layer in enumerate(layers):
             
-            if normalizations[Lindex] == 'y':
-                neural_layer = Normalization(neural_layer)
-                
-            if activations[Lindex] == 'relu':
-                neural_layer = Relu(neural_layer)
-            elif activations[Lindex] == 'sigmoid':
-                neural_layer = Sigmoid(neural_layer)
-            elif activations[Lindex] == 'softmax':
-                neural_layer = Softmax(neural_layer)
+            
+            neural_layer = normalization(neural_layer)
                 
             if Layer == 'fex':
-                neural_layer,W[Lindex] = Fex(neural_layer, W[Lindex], membran_thresholds[Lindex], membran_potentials[Lindex], Piece[Windex],1)
+                neural_layer,W[Lindex] = fex(neural_layer, W[Lindex], action_potential, Piece[Windex], 1)
             elif Layer == 'cat':
-                neural_layer,W[Lindex] = Cat(neural_layer, W[Lindex], membran_thresholds[Lindex], membran_potentials[Lindex],1, Piece[Windex])
+                neural_layer,W[Lindex] = cat(neural_layer, W[Lindex], action_potential, 1, Piece[Windex])
                 
         RealOutput = np.argmax(y_train[index])
         PredictedOutput = np.argmax(neural_layer)
         if RealOutput == PredictedOutput:
             true += 1
         acc = true / len(y_train)
         train_predictions[index] = PredictedOutput
         
-        if visualize == 'y':
-        
-            y_trainVisual = np.copy(y_train) 
-            y_trainVisual = np.argmax(y_trainVisual, axis=1)
-            
-            plt.figure(figsize=(12, 6))
-            sns.kdeplot(y_trainVisual, label='Real Outputs', fill=True)
-            sns.kdeplot(train_predictions, label='Predictions', fill=True)
-            plt.legend()
-            plt.xlabel('Class')
-            plt.ylabel('Data size')
-            plt.title('Predictions and Real Outputs for Training KDE Plot')
-            plt.show()
-            
-            if index + 1 != len(x_train):
-            
-                plt.close('all')
-        
-        if index == 0:
-            for i, w in enumerate(W):
-                trained_W[i] = w
-                     
-        else:
-            for i, w in enumerate(W):
-                trained_W[i] = trained_W[i] + w
+        for i, w in enumerate(W):
+            trained_W[i] = trained_W[i] + w
 
          
-        W = WeightIdentification(len(layers) - 1,class_count,neurons,x_train_size)
+        W = weight_identification(len(layers) - 1, len(class_count), neurons, x_train_size)
          
                
         uni_end_time = time.time()
         
         calculating_est = round((uni_end_time - uni_start_time) * (len(x_train) - index),3)
         
         if calculating_est < 60:
@@ -281,15 +156,15 @@
     
     
 
     return trained_W,train_predictions,acc
         
 # FUNCTIONS -----
 
-def WeightIdentification(
+def weight_identification(
     layer_count,      # int: Number of layers in the neural network.
     class_count,      # int: Number of classes in the classification task.
     neurons,         # list[num]: List of neuron counts for each layer.
     x_train_size        # int: Size of the input data.
 ) -> str:
     """
     Identifies the weights for a neural network model.
@@ -310,15 +185,15 @@
     W[0] = np.ones((neurons[0],x_train_size))
     ws = layer_count - 1
     for w in range(ws):
         W[w + 1] = np.ones((neurons[w + 1],neurons[w]))
     W[layer_count] = np.ones((class_count,neurons[layer_count - 1]))
     return W
 
-def SynapticPruning(
+def synaptic_pruning(
     w,            # list[list[num]]: Weight matrix of the neural network.
     cs,           # list[list[num]]: Synaptic connections between neurons.
     key,          # int: key for identifying synaptic connections.
     Class,        # int: Class label for the current training instance.
     class_count, # int: Total number of classes in the dataset.
     piece, # ???
     is_training # int: 1 or 0
@@ -371,34 +246,34 @@
                 w[cs:,:] = 0
     
             elif key == 'col':
     
                 w[:,cs] = 0
     
             else:
-                print(Fore.RED + "ERROR103: SynapticPruning func's key parameter must be 'row' or 'col' from: SynapticPruning" + infoPruning)
+                print(Fore.RED + "ERROR103: synaptic_pruning func's key parameter must be 'row' or 'col' from: synaptic_pruning" + infoPruning)
                 return 'e'
         else:
             if key == 'row':
     
                 w[cs:,:] = 0
     
                 ce = int(round(w.shape[0] - cs / class_count))
                 w[ce-1::-1,:] = 0
     
             elif key == 'col':
     
                 w[:,cs] = 0
     
             else:
-                print(Fore.RED + "ERROR103: SynapticPruning func's key parameter must be 'row' or 'col' from: SynapticPruning" + infoPruning + Style.RESET_ALL)
+                print(Fore.RED + "ERROR103: synaptic_pruning func's key parameter must be 'row' or 'col' from: synaptic_pruning" + infoPruning + Style.RESET_ALL)
                 return 'e'
     return w
 
-def SynapticDividing(
+def synaptic_dividing(
     class_count,    # int: Total number of classes in the dataset.
     W              # list[list[num]]: Weight matrix of the neural network.
 ) -> str:
     """
     Divides the synaptic weights of a neural network model based on class count.
 
     Args:
@@ -435,89 +310,76 @@
             
         j = 0
         cs = 0
         
     return Divides, Piece
         
 
-def Fex(
+def fex(
     Input,               # list[num]: Input data.
-    w,                   # list[list[num]]: Weight matrix of the neural network.
-    membran_threshold,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
-    membran_potential, # num: Threshold value for comparison.
+    w,                   # list[list[num]]: Weight matrix of the neural network.,
+    action_potential, # num: Threshold value for comparison.
     piece, # ???
     is_training # num: 1 or 0
 ) -> tuple:
     """
     Applies feature extraction process to the input data using synaptic pruning.
 
     Args:
         Input (list[num]): Input data.
         w (list[list[num]]): Weight matrix of the neural network.
-        membran_threshold (str): Sign for threshold comparison ('<', '>', '==', '!=').
-        membran_potential (num): Threshold value for comparison.
+        ACTION_threshold (str): Sign for threshold comparison ('<', '>', '==', '!=').
+        action_potential (num): Threshold value for comparison.
 
     Returns:
         tuple: A tuple (vector) containing the neural layer result and the updated weight matrix.
     """
 
-    if membran_threshold == '<':
-        PruneIndex = np.where(Input < membran_potential)
-    elif membran_threshold == '>': 
-        PruneIndex = np.where(Input > membran_potential)
-    elif membran_threshold == '==':
-        PruneIndex = np.where(Input == membran_potential)
-    elif membran_threshold == '!=':
-        PruneIndex = np.where(Input != membran_potential)
 
-    w = SynapticPruning(w, PruneIndex, 'col', 0, 0, piece, is_training)
+    PruneIndex = np.where(Input < action_potential)
+    w = synaptic_pruning(w, PruneIndex, 'col', 0, 0, piece, is_training)
 
     neural_layer = np.dot(w, Input)
+    
     return neural_layer,w
 
-def Cat(
+def cat(
     Input,               # list[num]: Input data.
     w,                   # list[list[num]]: Weight matrix of the neural network.
-    membran_threshold,      # str: Sign for threshold comparison ('<', '>', '==', '!=').
-    membran_potential,      # num: Threshold value for comparison.
+    action_potential,      # num: Threshold value for comparison.
     isTrain,
     piece              # int: Flag indicating if the function is called during training (1 for training, 0 otherwise).
 ) -> tuple:
     """
     Applies categorization process to the input data using synaptic pruning if specified.
 
     Args:
         Input (list[num]): Input data.
         w (list[list[num]]): Weight matrix of the neural network.
-        membran_threshold (str): Sign for threshold comparison ('<', '>', '==', '!=').
-        membran_potential (num): Threshold value for comparison.
+        ACTION_threshold (str): Sign for threshold comparison ('<', '>', '==', '!=').
+        action_potential (num): Threshold value for comparison.
         isTrain (int): Flag indicating if the function is called during training (1 for training, 0 otherwise).
 
     Returns:
         tuple: A tuple containing the neural layer (vector) result and the possibly updated weight matrix.
     """
-
-    if membran_threshold == '<':     
-        PruneIndex = np.where(Input < membran_potential)
-    elif membran_threshold == '>':     
-        PruneIndex = np.where(Input > membran_potential)
-    elif membran_threshold == '==':
-        PruneIndex = np.where(Input == membran_potential)
-    elif membran_threshold == '!=':     
-        PruneIndex = np.where(Input != membran_potential)
-    if isTrain == 1 and membran_threshold != 'none':
+   
+    PruneIndex = np.where(Input == action_potential)
+    
+    if isTrain == 1:
      
-            w = SynapticPruning(w, PruneIndex, 'col', 0, 0, piece, isTrain)
+        w = synaptic_pruning(w, PruneIndex, 'col', 0, 0, piece, isTrain)
      
     
     neural_layer = np.dot(w, Input)
+    
     return neural_layer,w
 
 
-def Normalization(
+def normalization(
     Input  # list[num]: Input data to be normalized.
 ):
     """
     Normalizes the input data using maximum absolute scaling.
 
     Args:
         Input (list[num]): Input data to be normalized.
@@ -582,257 +444,225 @@
 
     
     return np.maximum(0, x)
 
 
 
 
-def TestPLAN(
+def evaluate(
     x_test,         # list[list[num]]: Test input data.
     y_test,         # list[num]: Test labels.
-    layers,             # list[str]: List of layer names.
-    membran_thresholds,     # list[str]: List of MEMBRAN THRESHOLDS for each layer.
-    membran_potentials,    # list[num]: List of MEMBRAN POTENTIALS for each layer.
-    normalizations,    # str: Whether normalization will be performed ("y" or "n").
-    activations,       # str: Activation function list for the neural network.
+    action_potential,    # list[num]: List of ACTION POTENTIALS for each layer.
     visualize,         # visualize Testing procces or not visualize ('y' or 'n')
     W                  # list[list[num]]: Weight matrix of the neural network.
 ) -> tuple:
-    infoTestModel =  """
+  infoTestModel =  """
     Tests the neural network model with the given test data.
 
     Args:
         x_test (list[list[num]]): Test input data.
         y_test (list[num]): Test labels.
-        layers (list[str]): List of layer names.
-        membran_thresholds (list[str]): List of MEMBRAN THRESHOLDS for each layer.
-        membran_potentials (list[num]): List of MEMBRAN POTENTIALS for each layer.
-        normalizatios list([str]): Whether normalization will be performed ("yes" or "no").
-        activations (list[str]): Activation function for the neural network.
+        action_potential (float): Input ACTION potential 
+        visualize (str): Visualize test progress ? ('y' or 'n')
         W (list[list[num]]): Weight matrix of the neural network.
 
     Returns:
         tuple: A tuple containing the predicted labels and the accuracy of the model.
     """
+    
+  layers = ['fex','cat']
 
 
-    try:
-        Wc = [0] * len(W)
-        true = 0
-        TestPredictions = [None] * len(y_test)
-        for i, w in enumerate(W):
-            Wc[i] = np.copy(w)
-            print('\rCopying weights.....',i+1,'/',len(W),end = "")
-                
-        print(Fore.GREEN + "\n\nTest Started with 0 ERROR\n" + Style.RESET_ALL)
-        start_time = time.time()
-        for inpIndex,Input in enumerate(x_test):
-            Input = np.array(Input)
-            Input = Input.ravel()
-            uni_start_time = time.time()
-            neural_layer = Input
-            
-            for index, Layer in enumerate(layers):
-                if normalizations[index] == 'y':
-                    neural_layer = Normalization(neural_layer)
-                if activations[index] == 'relu':
-                        neural_layer = Relu(neural_layer)
-                elif activations[index] == 'sigmoid':
-                        neural_layer = Sigmoid(neural_layer)
-                elif activations[index] == 'softmax':
-                        neural_layer = Softmax(neural_layer)
-                        
-                if layers[index] == 'fex':
-                    neural_layer,useless = Fex(neural_layer, W[index], membran_thresholds[index], membran_potentials[index],0,0)
-                if layers[index] == 'cat':
-                    neural_layer,useless = Cat(neural_layer, W[index], membran_thresholds[index], membran_potentials[index],0,0)
-            for i, w in enumerate(Wc):
-                W[i] = np.copy(w)
-            RealOutput = np.argmax(y_test[inpIndex])
-            PredictedOutput = np.argmax(neural_layer)
-            if RealOutput == PredictedOutput:
-                true += 1
-            acc = true / len(y_test)
-            TestPredictions[inpIndex] = PredictedOutput
-            
-            if visualize == 'y':
+  try:
+    Wc = [0] * len(W)
+    true = 0
+    TestPredictions = [None] * len(y_test)
+    for i, w in enumerate(W):
+        Wc[i] = np.copy(w)
+        print('\rCopying weights.....',i+1,'/',len(W),end = "")
             
-                y_testVisual = np.copy(y_test) 
-                y_testVisual = np.argmax(y_testVisual, axis=1)
-                
-                plt.figure(figsize=(12, 6))
-                sns.kdeplot(y_testVisual, label='Real Outputs', fill=True)
-                sns.kdeplot(TestPredictions, label='Predictions', fill=True)
-                plt.legend()
-                plt.xlabel('Class')
-                plt.ylabel('Data size')
-                plt.title('Predictions and Real Outputs for Testing KDE Plot')
-                plt.show()
-                
-                if inpIndex + 1 != len(x_test):
-                
-                    plt.close('all')
+    print(Fore.GREEN + "\n\nTest Started with 0 ERROR\n" + Style.RESET_ALL)
+    start_time = time.time()
+    for inpIndex,Input in enumerate(x_test):
+        Input = np.array(Input)
+        Input = Input.ravel()
+        uni_start_time = time.time()
+        neural_layer = Input
+        
+        for index, Layer in enumerate(layers):
             
-            uni_end_time = time.time()
-                
-            calculating_est = round((uni_end_time - uni_start_time) * (len(x_test) - inpIndex),3)
-                
-            if calculating_est < 60:
-                print('\rest......(sec):',calculating_est,'\n',end= "")
-                print('\rTest accuracy: ' ,acc ,"\n", end="")
-            
-            elif calculating_est > 60 and calculating_est < 3600:
-                print('\rest......(min):',calculating_est/60,'\n',end= "")
-                print('\rTest accuracy: ' ,acc ,"\n", end="")
-            
-            elif calculating_est > 3600:
-                print('\rest......(h):',calculating_est/3600,'\n',end= "")
-                print('\rTest accuracy: ' ,acc ,"\n", end="")
+            neural_layer = normalization(neural_layer)
+
+            if layers[index] == 'fex':
+                neural_layer = fex(neural_layer, W[index],  action_potential, 0, 0)[0]
+            if layers[index] == 'cat':
+                neural_layer = cat(neural_layer, W[index],  action_potential, 0, 0)[0]
                 
-        EndTime = time.time()
         for i, w in enumerate(Wc):
             W[i] = np.copy(w)
-
-        calculating_est = round(EndTime - start_time,2)
+        RealOutput = np.argmax(y_test[inpIndex])
+        PredictedOutput = np.argmax(neural_layer)
+        if RealOutput == PredictedOutput:
+            true += 1
+        acc = true / len(y_test)
+        TestPredictions[inpIndex] = PredictedOutput
         
-        print(Fore.GREEN + "\nTest Finished with 0 ERROR\n")
+        if visualize == 'y':
         
-        if calculating_est < 60:
-            print('Total testing time(sec): ',calculating_est)
+            y_testVisual = np.copy(y_test) 
+            y_testVisual = np.argmax(y_testVisual, axis=1)
             
-        elif calculating_est > 60 and calculating_est < 3600:
-            print('Total testing time(min): ',calculating_est/60)
+            plt.figure(figsize=(12, 6))
+            sns.kdeplot(y_testVisual, label='Real Outputs', fill=True)
+            sns.kdeplot(TestPredictions, label='Predictions', fill=True)
+            plt.legend()
+            plt.xlabel('Class')
+            plt.ylabel('Data size')
+            plt.title('Predictions and Real Outputs for Testing KDE Plot')
+            plt.show()
+            
+            if inpIndex + 1 != len(x_test):
+            
+                plt.close('all')
+        
+        uni_end_time = time.time()
+            
+        calculating_est = round((uni_end_time - uni_start_time) * (len(x_test) - inpIndex),3)
             
+        if calculating_est < 60:
+            print('\rest......(sec):',calculating_est,'\n',end= "")
+            print('\rTest accuracy: ' ,acc ,"\n", end="")
+        
+        elif calculating_est > 60 and calculating_est < 3600:
+            print('\rest......(min):',calculating_est/60,'\n',end= "")
+            print('\rTest accuracy: ' ,acc ,"\n", end="")
+        
         elif calculating_est > 3600:
-            print('Total testing time(h): ',calculating_est/3600)
+            print('\rest......(h):',calculating_est/3600,'\n',end= "")
+            print('\rTest accuracy: ' ,acc ,"\n", end="")
             
-        if acc >= 0.8:
-            print(Fore.GREEN + '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)
+    EndTime = time.time()
+    for i, w in enumerate(Wc):
+        W[i] = np.copy(w)
+
+    calculating_est = round(EndTime - start_time,2)
+    
+    print(Fore.GREEN + "\nTest Finished with 0 ERROR\n")
+    
+    if calculating_est < 60:
+        print('Total testing time(sec): ',calculating_est)
         
-        elif acc < 0.8 and acc > 0.6:
-            print(Fore.MAGENTA + '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)
+    elif calculating_est > 60 and calculating_est < 3600:
+        print('Total testing time(min): ',calculating_est/60)
+        
+    elif calculating_est > 3600:
+        print('Total testing time(h): ',calculating_est/3600)
         
-        elif acc <= 0.6:
-            print(Fore.RED+ '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)  
+    if acc >= 0.8:
+        print(Fore.GREEN + '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)
+    
+    elif acc < 0.8 and acc > 0.6:
+        print(Fore.MAGENTA + '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)
+    
+    elif acc <= 0.6:
+        print(Fore.RED+ '\nTotal Test accuracy: ' ,acc, '\n' + Style.RESET_ALL)  
 
         
     
-    except:
+  except:
         
-        print(Fore.RED + "ERROR: Testing model parameters like 'layers' 'MembranCounts' must be same as trained model. Check parameters. Are you sure weights are loaded ? from: TestPLAN" + infoTestModel + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Testing model parameters like 'action_potential' must be same as trained model. Check parameters. Are you sure weights are loaded ? from: evaluate" + infoTestModel + Style.RESET_ALL)
         return 'e'
    
 
    
-    return W,TestPredictions,acc
+  return W,TestPredictions,acc
 
-def SavePLAN(model_name,
+def save_model(model_name,
              model_type,
-             layers,
              class_count,
-             membran_thresholds,
-             membran_potentials,
-             normalizations,
-             activations,
+             action_potential,
              test_acc,
-             log_type,
              weights_type,
              weights_format,
              model_path,
              W
  ):
     
-    infoSavePLAN = """
+    infosave_model = """
     Function to save a deep learning model.
 
     Arguments:
     model_name (str): Name of the model.
     model_type (str): Type of the model.(options: PLAN)
-    layers (list): List containing 'fex' and 'cat' layers.
     class_count (int): Number of classes.
-    membran_thresholds (list): List containing MEMBRAN THRESHOLDS.
-    membran_potentials (list): List containing MEMBRAN POTENTIALS.
-    DoNormalization (str): is that normalized data ? 'y' or 'n'.
-    activations (list): List containing activation functions for each layer.
+    action_potential (list): List containing ACTION POTENTIALS.
     test_acc (float): Test accuracy of the model.
-    log_type (str): Type of log to save (options: 'csv', 'txt', 'hdf5').
     weights_type (str): Type of weights to save (options: 'txt', 'npy', 'mat').
     WeightFormat (str): Format of the weights (options: 'd', 'f', 'raw').
     model_path (str): Path where the model will be saved. For example: C:/Users/beydili/Desktop/denemePLAN/
     W: Weights of the model.
     
     Returns:
     str: Message indicating if the model was saved successfully or encountered an error.
     """
     
     # Operations to be performed by the function will be written here
     pass
 
-    if log_type != 'csv' and  log_type != 'txt' and log_type != 'hdf5':
-        print(Fore.RED + "ERROR109: Save Log Type (File Extension) must be 'csv' or 'txt' or 'hdf5' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
-        return 'e'
-    
+    layers = ['fex','cat']    
+
     if weights_type != 'txt' and  weights_type != 'npy' and weights_type != 'mat':
-        print(Fore.RED + "ERROR110: Save Weight type (File Extension) Type must be 'txt' or 'npy' or 'mat' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR110: Save Weight type (File Extension) Type must be 'txt' or 'npy' or 'mat' from: save_model" + infosave_model + Style.RESET_ALL)
         return 'e'
     
     if weights_format != 'd' and  weights_format != 'f' and weights_format != 'raw':
-        print(Fore.RED + "ERROR111: Weight Format Type must be 'd' or 'f' or 'raw' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR111: Weight Format Type must be 'd' or 'f' or 'raw' from: save_model" + infosave_model + Style.RESET_ALL)
         return 'e'
     
     NeuronCount = 0
     SynapseCount = 0
+    
     try:
         for w in W:
             NeuronCount += np.shape(w)[0]
             SynapseCount += np.shape(w)[0] * np.shape(w)[1]
     except:
         
-        print(Fore.RED + "ERROR: Weight matrices has a problem from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Weight matrices has a problem from: save_model" + infosave_model + Style.RESET_ALL)
         return 'e'
     import pandas as pd
     from datetime import datetime
     from scipy import io
     
     data = {'MODEL NAME': model_name,
             'MODEL TYPE': model_type,
             'LAYERS': layers,
             'LAYER COUNT': len(layers),
             'CLASS COUNT': class_count,
-            'MEMBRAN THRESHOLDS': membran_thresholds,
-            'MEMBRAN POTENTIALS': membran_potentials,
-            'NORMALIZATION': normalizations,
-            'ACTIVATIONS': activations,
+            'ACTION POTENTIAL': action_potential,
             'NEURON COUNT': NeuronCount,
             'SYNAPSE COUNT': SynapseCount,
             'TEST ACCURACY': test_acc,
             'SAVE DATE': datetime.now(),
             'WEIGHTS TYPE': weights_type,
             'WEIGHTS FORMAT': weights_format,
             'MODEL PATH': model_path
             }
     try:
         
         df = pd.DataFrame(data)
-        
-        if  log_type == 'csv':
-        
-            df.to_csv(model_path + model_name + '.csv', sep='\t', index=False)
-            
-        elif log_type == 'txt':
-            
-            df.to_csv(model_path + model_name + '.txt', sep='\t', index=False)
-            
-        elif log_type == 'hdf5':
+
             
-            df.to_hdf(model_path + model_name + '.h5', key='data', mode='w')
+        df.to_csv(model_path + model_name + '.txt', sep='\t', index=False)
             
+
     except:
         
-        print(Fore.RED + "ERROR: Model log not saved probably model_path incorrect. Check the log parameters from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Model log not saved probably model_path incorrect. Check the log parameters from: save_model" + infosave_model + Style.RESET_ALL)
         return 'e'
     try:
         
         if weights_type == 'txt' and weights_format == 'd':
             
             for i, w in enumerate(W):
                 np.savetxt(model_path + model_name +  str(i+1) + 'w.txt' ,  w, fmt='%d')
@@ -886,70 +716,59 @@
             
             for i, w in enumerate(W):
                 w = {'w': w}
                 io.savemat(model_path + model_name + str(i+1) + 'w.mat', w)
             
     except:
         
-        print(Fore.RED + "ERROR: Model Weights not saved. Check the Weight parameters. SaveFilePath expl: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Model Weights not saved. Check the Weight parameters. SaveFilePath expl: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: save_model" + infosave_model + Style.RESET_ALL)
         return 'e'
     print(df)
     message = (
         Fore.GREEN + "Model Saved Successfully\n" +
         Fore.MAGENTA + "Don't forget, if you want to load model: model log file and weight files must be in the same directory." + 
         Style.RESET_ALL
         )
     
     return print(message)
 
 
-def LoadPLAN(model_name,
+def load_model(model_name,
              model_path,
-             log_type,
 ):
-   infoLoadPLAN = """
+   infoload_model = """
    Function to load a deep learning model.
 
    Arguments:
    model_name (str): Name of the model.
    model_path (str): Path where the model is saved.
    log_type (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
 
    Returns:
-   lists: W(list[num]), layers, membran_thresholds, membran_potentials, Normalization,activations
+   lists: W(list[num]), action_potential, df (DataFrame of the model)
     """
    pass
 
     
    import pandas as pd
    import scipy.io as sio
    
    try:
-   
-       if log_type == 'csv':
-           df = pd.read_csv(model_path + model_name + '.' + log_type)
-        
-    
-       if log_type == 'txt':
-           df = pd.read_csv(model_path + model_name + '.' + log_type, delimiter='\t')
-        
+
+       df = pd.read_csv(model_path + model_name + '.' + 'txt', delimiter='\t')
     
-       if log_type == 'hdf5':
-           df = pd.read_hdf(model_path + model_name + '.' + log_type)
    except:
-       print(Fore.RED + "ERROR: Model Path error. accaptable form: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: LoadPLAN" + infoLoadPLAN + Style.RESET_ALL)
+       
+       print(Fore.RED + "ERROR: Model Path error. accaptable form: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: load_model" + infoload_model + Style.RESET_ALL)
 
    model_name = str(df['MODEL NAME'].iloc[0])
    layers = df['LAYERS'].tolist()
    layer_count = int(df['LAYER COUNT'].iloc[0])
    class_count = int(df['CLASS COUNT'].iloc[0])
-   membran_thresholds = df['MEMBRAN THRESHOLDS'].tolist()
-   membran_potentials = df['MEMBRAN POTENTIALS'].tolist()
-   normalizations = df['NORMALIZATION'].tolist()
-   activations = df['ACTIVATIONS'].tolist()
+   action_potential = int(df['ACTION POTENTIAL'].iloc[0])
    NeuronCount = int(df['NEURON COUNT'].iloc[0])
    SynapseCount = int(df['SYNAPSE COUNT'].iloc[0])
    test_acc = int(df['TEST ACCURACY'].iloc[0])
    model_type = str(df['MODEL TYPE'].iloc[0])
    WeightType = str(df['WEIGHTS TYPE'].iloc[0])
    WeightFormat = str(df['WEIGHTS FORMAT'].iloc[0])
    model_path = str(df['MODEL PATH'].iloc[0])
@@ -962,160 +781,140 @@
    elif WeightType == 'npy':
        for i in range(layer_count):    
            W[i] = np.load(model_path + model_name + str(i+1) + 'w.npy')
    elif WeightType == 'mat':
        for i in range(layer_count):  
            W[i] = sio.loadmat(model_path + model_name + str(i+1) + 'w.mat')
    else:
-        raise ValueError(Fore.RED + "Incorrect weight type value. Value must be 'txt', 'npy' or 'mat' from: LoadPLAN."  + infoLoadPLAN + Style.RESET_ALL)
+        raise ValueError(Fore.RED + "Incorrect weight type value. Value must be 'txt', 'npy' or 'mat' from: load_model."  + infoload_model + Style.RESET_ALL)
    print(Fore.GREEN + "Model loaded succesfully" + Style.RESET_ALL)     
-   return W,layers,membran_thresholds,membran_potentials,normalizations,activations,df
+   return W,action_potential,df
 
-def PredictFromDiscPLAN(Input,model_name,model_path,log_type):
-    infoPredictFromDİscPLAN = """
+def predict_model_ssd(Input,model_name,model_path):
+    
+    infopredict_model_ssd = """
     Function to make a prediction using a divided pruning deep learning neural network (PLAN).
 
     Arguments:
     Input (list or ndarray): Input data for the model (single vector or single matrix).
     model_name (str): Name of the model.
     model_path (str): Path where the model is saved.
-    log_type (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
-
     Returns:
     ndarray: Output from the model.
     """
-    W,layers,membran_thresholds,membran_potentials,normalizations,activations = LoadPLAN(model_name,model_path,
-                                                                                  log_type)[0:6]
+    W,action_potential = load_model(model_name,model_path)[0:2]
+    
+    layers = ['fex','cat']
+    
     Wc = [0] * len(W)
     for i, w in enumerate(W):
         Wc[i] = np.copy(w)
     try:
         neural_layer = Input
         neural_layer = np.array(neural_layer)
         neural_layer = neural_layer.ravel()
         for index, Layer in enumerate(layers):                                                                          
-            if Normalization == 'y':
-                neural_layer = Normalization(neural_layer)
-            if activations[index] == 'relu':
-                neural_layer = Relu(neural_layer)
-            elif activations[index] == 'sigmoid':
-                neural_layer = Sigmoid(neural_layer)
-            elif activations[index] == 'softmax':
-                neural_layer = Softmax(neural_layer)
+
+            neural_layer = normalization(neural_layer)
                                 
             if layers[index] == 'fex':
-                neural_layer,useless = Fex(neural_layer, W[index],
-                                          membran_thresholds[index],
-                                          membran_potentials[index],0,0)
+                neural_layer = fex(neural_layer, W[index], action_potential,0, 0)[0]
             if layers[index] == 'cat':
-                neural_layer,useless = Cat(neural_layer, W[index],
-                                          membran_thresholds[index],
-                                          membran_potentials[index],
-                                          0,0)
+                neural_layer = cat(neural_layer, W[index], action_potential, 0, 0)[0]
     except:
-       print(Fore.RED + "ERROR: The input was probably entered incorrectly. from: PredictFromDiscPLAN"  + infoPredictFromDİscPLAN + Style.RESET_ALL)
+       print(Fore.RED + "ERROR: The input was probably entered incorrectly. from: predict_model_ssd"  + infopredict_model_ssd + Style.RESET_ALL)
        return 'e'
     for i, w in enumerate(Wc):
         W[i] = np.copy(w)
     return neural_layer
 
 
-def PredictFromRamPLAN(Input,layers,membran_thresholds,membran_potentials,normalizations,activations,W):
-    infoPredictFromRamPLAN = """
+def predict_model_ram(Input,action_potential,W):
+    
+    infopredict_model_ram = """
     Function to make a prediction using a pruning learning artificial neural network (PLAN)
     from weights and parameters stored in memory.
 
     Arguments:
     Input (list or ndarray): Input data for the model (single vector or single matrix).
-    layers (list): Number and types of layers.
-    membran_thresholds (list): MEMBRAN THRESHOLDS.
-    membran_potentials (list): MEMBRAN POTENTIALS.
-    DoNormalization (str): Whether to normalize ('y' or 'n').
-    activations (list): Activation functions for each layer.
+    action_potential (list): ACTION POTENTIAL.
     W (list of ndarrays): Weights of the model.
 
     Returns:
     ndarray: Output from the model.
     """
     
+    layers = ['fex','cat']
+    
     Wc = [0] * len(W)
     for i, w in enumerate(W):
         Wc[i] = np.copy(w)
     try:
         neural_layer = Input
         neural_layer = np.array(neural_layer)
         neural_layer = neural_layer.ravel()
         for index, Layer in enumerate(layers):                                                                          
-            if normalizations[index] == 'y':
-                neural_layer = Normalization(neural_layer)
-            if activations[index] == 'relu':
-                neural_layer = Relu(neural_layer)
-            elif activations[index] == 'sigmoid':
-                neural_layer = Sigmoid(neural_layer)
-            elif activations[index] == 'softmax':
-                neural_layer = Softmax(neural_layer)
-                                
+
+            neural_layer = normalization(neural_layer)
+                                  
             if layers[index] == 'fex':
-                neural_layer,useless = Fex(neural_layer, W[index],
-                                          membran_thresholds[index],
-                                          membran_potentials[index],0,0)
+                neural_layer = fex(neural_layer, W[index], action_potential,0, 0)[0]
             if layers[index] == 'cat':
-                neural_layer,useless = Cat(neural_layer, W[index],
-                                          membran_thresholds[index],
-                                          membran_potentials[index],
-                                          0,0)
+                neural_layer = cat(neural_layer, W[index], action_potential, 0, 0)[0]
+                
     except:
-        print(Fore.RED + "ERROR: Unexpected input or wrong model parameters from: PredictFromRamPLAN."  + infoPredictFromRamPLAN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Unexpected input or wrong model parameters from: predict_model_ram."  + infopredict_model_ram + Style.RESET_ALL)
         return 'e'
     for i, w in enumerate(Wc):
         W[i] = np.copy(w)
     return neural_layer
     
 
-def AutoBalancer(x_train, y_train, class_count):
-   infoAutoBalancer = """
+def auto_balancer(x_train, y_train, class_count):
+    
+   infoauto_balancer = """
    Function to balance the training data across different classes.
 
    Arguments:
    x_train (list): Input data for training.
    y_train (list): Labels corresponding to the input data.
    class_count (int): Number of classes.
 
    Returns:
    tuple: A tuple containing balanced input data and labels.
    """
    try:
         ClassIndices = {i: np.where(np.array(y_train)[:, i] == 1)[0] for i in range(class_count)}
-        class_counts = [len(ClassIndices[i]) for i in range(class_count)]
+        classes = [len(ClassIndices[i]) for i in range(class_count)]
         
-        if len(set(class_counts)) == 1:
-            print(Fore.WHITE + "INFO: All training data have already balanced. from: AutoBalancer"  + Style.RESET_ALL)
+        if len(set(classes)) == 1:
+            print(Fore.WHITE + "INFO: All training data have already balanced. from: auto_balancer"  + Style.RESET_ALL)
             return x_train, y_train
         
-        MinCount = min(class_counts)
+        MinCount = min(classes)
         
         BalancedIndices = []
         for i in range(class_count):
             if len(ClassIndices[i]) > MinCount:
                 SelectedIndices = np.random.choice(ClassIndices[i], MinCount, replace=False)
             else:
                 SelectedIndices = ClassIndices[i]
             BalancedIndices.extend(SelectedIndices)
         
         BalancedInputs = [x_train[idx] for idx in BalancedIndices]
         BalancedLabels = [y_train[idx] for idx in BalancedIndices]
         
-        print(Fore.GREEN + "All Training Data Succesfully Balanced from: " + str(len(x_train)) + " to: " + str(len(BalancedInputs)) + ". from: AutoBalancer " + Style.RESET_ALL)
+        print(Fore.GREEN + "All Training Data Succesfully Balanced from: " + str(len(x_train)) + " to: " + str(len(BalancedInputs)) + ". from: auto_balancer " + Style.RESET_ALL)
    except:
-        print(Fore.RED + "ERROR: Inputs and labels must be same length check parameters" + infoAutoBalancer)
+        print(Fore.RED + "ERROR: Inputs and labels must be same length check parameters" + infoauto_balancer)
         return 'e'
         
    return BalancedInputs, BalancedLabels
    
-def SyntheticAugmentation(x, y, class_count):
+def synthetic_augmentation(x, y, class_count):
     """
     Generates synthetic examples to balance classes with fewer examples.
     
     Arguments:
     x -- Input dataset (examples) - list format
     y -- Class labels (one-hot encoded) - list format
     class_count -- Number of classes
@@ -1152,22 +951,26 @@
                 y_balanced.append(y[class_indices[0]])  # The new example has the same class label
                 
                 num_samples += 1
     
     return np.array(x_balanced), np.array(y_balanced)
 
    
-def GetWeights():
+def get_weights():
         
     return 0
     
-def GetDf():
+def get_df():
         
-    return 6
+    return 2
     
-def GetPreds():
+def get_preds():
         
     return 1
     
-def GetAcc():
+def get_acc():
         
     return 2
+
+def get_pot():
+    
+    return 1
```

### Comparing `pyerualjetwork-1.3.9/setup.py` & `pyerualjetwork-2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.3.9",
+      version = "2.0",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
-      description= "Advanced python deep learning library. MASSIVE Technic Update, unlocked class limits. (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
+      description= "Advanced python deep learning library. New features: More simple and practical, all functions and variables are snake_case. (Documentation in desc. Examples in GİTHUB: https://github.com/HCB06/PyerualJetwork)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks'],
 
       
       )
```

