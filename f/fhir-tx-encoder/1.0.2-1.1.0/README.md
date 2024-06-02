# Comparing `tmp/fhir_tx_encoder-1.0.2.tar.gz` & `tmp/fhir_tx_encoder-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhir_tx_encoder-1.0.2.tar", last modified: Tue Oct 31 05:22:20 2023, max compression
+gzip compressed data, was "fhir_tx_encoder-1.1.0.tar", last modified: Sun Jun  2 04:51:39 2024, max compression
```

## Comparing `fhir_tx_encoder-1.0.2.tar` & `fhir_tx_encoder-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 05:22:20.980267 fhir_tx_encoder-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-31 05:22:04.000000 fhir_tx_encoder-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2023-10-31 05:22:20.980267 fhir_tx_encoder-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2023-10-31 05:22:04.000000 fhir_tx_encoder-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 05:22:20.980267 fhir_tx_encoder-1.0.2/fhir_tx/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-10-31 05:22:04.000000 fhir_tx_encoder-1.0.2/fhir_tx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2023-10-31 05:22:04.000000 fhir_tx_encoder-1.0.2/fhir_tx/closure.py
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2023-10-31 05:22:04.000000 fhir_tx_encoder-1.0.2/fhir_tx/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 05:22:20.980267 fhir_tx_encoder-1.0.2/fhir_tx_encoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2023-10-31 05:22:20.000000 fhir_tx_encoder-1.0.2/fhir_tx_encoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-10-31 05:22:20.000000 fhir_tx_encoder-1.0.2/fhir_tx_encoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 05:22:20.000000 fhir_tx_encoder-1.0.2/fhir_tx_encoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-31 05:22:20.000000 fhir_tx_encoder-1.0.2/fhir_tx_encoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-31 05:22:20.000000 fhir_tx_encoder-1.0.2/fhir_tx_encoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 05:22:20.980267 fhir_tx_encoder-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-10-31 05:22:04.000000 fhir_tx_encoder-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 04:51:39.186349 fhir_tx_encoder-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-02 04:51:29.000000 fhir_tx_encoder-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-06-02 04:51:39.186349 fhir_tx_encoder-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-06-02 04:51:29.000000 fhir_tx_encoder-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 04:51:39.186349 fhir_tx_encoder-1.1.0/fhir_tx/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-06-02 04:51:29.000000 fhir_tx_encoder-1.1.0/fhir_tx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-06-02 04:51:29.000000 fhir_tx_encoder-1.1.0/fhir_tx/closure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-06-02 04:51:29.000000 fhir_tx_encoder-1.1.0/fhir_tx/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 04:51:39.186349 fhir_tx_encoder-1.1.0/fhir_tx_encoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-06-02 04:51:39.000000 fhir_tx_encoder-1.1.0/fhir_tx_encoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-06-02 04:51:39.000000 fhir_tx_encoder-1.1.0/fhir_tx_encoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 04:51:39.000000 fhir_tx_encoder-1.1.0/fhir_tx_encoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 04:51:39.000000 fhir_tx_encoder-1.1.0/fhir_tx_encoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 04:51:39.000000 fhir_tx_encoder-1.1.0/fhir_tx_encoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 04:51:39.186349 fhir_tx_encoder-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-06-02 04:51:29.000000 fhir_tx_encoder-1.1.0/setup.py
```

### Comparing `fhir_tx_encoder-1.0.2/LICENSE` & `fhir_tx_encoder-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fhir_tx_encoder-1.0.2/PKG-INFO` & `fhir_tx_encoder-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhir_tx_encoder
-Version: 1.0.2
+Version: 1.1.0
 Summary: Tools for encoding FHIR terminology concepts for machine learning
 Author: Australian e-Health Research Centre, CSIRO
 Author-email: ontoserver-support@csiro.au
 License: Apache 2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fhir_tx_encoder-1.0.2/README.md` & `fhir_tx_encoder-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fhir_tx_encoder-1.0.2/fhir_tx/__init__.py` & `fhir_tx_encoder-1.1.0/fhir_tx/__init__.py`

 * *Files identical despite different names*

### Comparing `fhir_tx_encoder-1.0.2/fhir_tx/closure.py` & `fhir_tx_encoder-1.1.0/fhir_tx/closure.py`

 * *Files identical despite different names*

### Comparing `fhir_tx_encoder-1.0.2/fhir_tx/encoder.py` & `fhir_tx_encoder-1.1.0/fhir_tx/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,20 +49,22 @@
     :type displays_: list[str]
     """
 
     def __init__(
         self,
         scope: str,
         tx_url: str = "https://tx.ontoserver.csiro.au/fhir",
+        subsumption: bool = True,
         properties: list[str] = None,
         batch_size: int = 50000,
     ):
         """
         :param scope: A FHIR ValueSet URI that defines the scope of the codes to be encoded.
         :param tx_url: A FHIR terminology server endpoint.
+        :param subsumption: Whether to include subsumption relationships in the encoding.
         :param properties: A list of properties to include in the encoding. A single value of "*"
             will include all properties.
         :param batch_size: The number of codes to send to the terminology server at a time when
             running queries.
         """
         print(f"Expanding value set: {scope}")
         coding_batches = self._expand_scope(scope, tx_url, properties, batch_size)
@@ -72,23 +74,24 @@
         ohe = OneHotEncoder(categories=[self.codes_])
         # Use a lil_matrix as an intermediate representation that enables efficient updates.
         self._encoded = lil_matrix(
             ohe.fit_transform(np.array(self.codes_).reshape(-1, 1))
         )
         print(self._encoded.shape)
 
-        # Create an index of code -> index, which we use to update the correct row and column in the
-        # matrix when making subsumption updates.
+        # Create an index of code -> index, which we use to update the correct row and column in
+        # the matrix when making subsumption updates.
         print("Creating index...", end=" ")
         self._index = {value: index for index, value in enumerate(ohe.categories_[0])}
         print(f"{len(self._index)} items")
 
-        print("Applying transitive closure...")
-        self._apply_closure(coding_batches, tx_url)
-        print(f"Subsumption encoding complete: {self._encoded.shape}")
+        if subsumption:
+            print("Applying transitive closure...")
+            self._apply_closure(coding_batches, tx_url)
+            print(f"Subsumption encoding complete: {self._encoded.shape}")
 
         self.feature_names_ = self.codes_
         if properties is not None:
             print("Encoding properties...", end=" ")
             dv = DictVectorizer()
             encoded_properties = dv.fit_transform(self.properties_)
             self._encoded = hstack([self._encoded, encoded_properties])
@@ -197,15 +200,15 @@
         Retrieve the encodings for a two-dimensional array of codes.
         """
         if not isinstance(X, np.ndarray):
             raise ValueError("X must be a Numpy array")
         if len(X.shape) != 2:
             raise ValueError("X must be a two-dimensional array")
 
-        stacked = hstack([self.transform_column(x) for x in X])
+        stacked = hstack([self.transform_column(X[:, y]) for y in range(X.shape[1])])
         return stacked
 
     def fit(self, X, y=None):
         """
         Does nothing, but required for compatibility with scikit-learn pipelines.
         """
         return self
```

### Comparing `fhir_tx_encoder-1.0.2/fhir_tx_encoder.egg-info/PKG-INFO` & `fhir_tx_encoder-1.1.0/fhir_tx_encoder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fhir-tx-encoder
-Version: 1.0.2
+Name: fhir_tx_encoder
+Version: 1.1.0
 Summary: Tools for encoding FHIR terminology concepts for machine learning
 Author: Australian e-Health Research Centre, CSIRO
 Author-email: ontoserver-support@csiro.au
 License: Apache 2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fhir_tx_encoder-1.0.2/setup.py` & `fhir_tx_encoder-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="fhir_tx_encoder",
-    version="1.0.2",
+    version="1.1.0",
     description="Tools for encoding FHIR terminology concepts for machine learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Australian e-Health Research Centre, CSIRO",
     author_email="ontoserver-support@csiro.au",
     license="Apache 2.0",
     packages=["fhir_tx"],
```

