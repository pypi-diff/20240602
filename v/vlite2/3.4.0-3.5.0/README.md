# Comparing `tmp/vlite2-3.4.0.tar.gz` & `tmp/vlite2-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlite2-3.4.0.tar", last modified: Wed Feb 14 01:35:51 2024, max compression
+gzip compressed data, was "vlite2-3.5.0.tar", last modified: Sun Jun  2 19:38:10 2024, max compression
```

## Comparing `vlite2-3.4.0.tar` & `vlite2-3.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 raydelv    (501) staff       (20)        0 2024-02-14 01:35:51.557752 vlite2-3.4.0/
--rw-r--r--   0 raydelv    (501) staff       (20)    34523 2023-11-27 04:55:35.000000 vlite2-3.4.0/LICENSE
--rw-r--r--   0 raydelv    (501) staff       (20)      293 2024-02-14 01:35:51.557625 vlite2-3.4.0/PKG-INFO
--rw-r--r--   0 raydelv    (501) staff       (20)     4073 2024-02-14 01:35:45.000000 vlite2-3.4.0/README.md
--rw-r--r--   0 raydelv    (501) staff       (20)       38 2024-02-14 01:35:51.557806 vlite2-3.4.0/setup.cfg
--rw-r--r--   0 raydelv    (501) staff       (20)      570 2024-02-14 01:35:06.000000 vlite2-3.4.0/setup.py
-drwxr-xr-x   0 raydelv    (501) staff       (20)        0 2024-02-14 01:35:51.556041 vlite2-3.4.0/test/
--rw-r--r--   0 raydelv    (501) staff       (20)    26441 2024-02-14 01:33:13.000000 vlite2-3.4.0/test/test.py
-drwxr-xr-x   0 raydelv    (501) staff       (20)        0 2024-02-14 01:35:51.556678 vlite2-3.4.0/vlite2/
--rw-r--r--   0 raydelv    (501) staff       (20)       90 2024-02-14 01:27:54.000000 vlite2-3.4.0/vlite2/__init__.py
--rw-r--r--   0 raydelv    (501) staff       (20)     4868 2024-02-14 01:29:41.000000 vlite2-3.4.0/vlite2/ingestors.py
--rw-r--r--   0 raydelv    (501) staff       (20)     7856 2024-02-14 01:27:04.000000 vlite2-3.4.0/vlite2/main.py
--rw-r--r--   0 raydelv    (501) staff       (20)     2218 2024-02-14 01:23:07.000000 vlite2-3.4.0/vlite2/model.py
--rw-r--r--   0 raydelv    (501) staff       (20)      892 2024-02-14 01:07:32.000000 vlite2-3.4.0/vlite2/utils.py
-drwxr-xr-x   0 raydelv    (501) staff       (20)        0 2024-02-14 01:35:51.557450 vlite2-3.4.0/vlite2.egg-info/
--rw-r--r--   0 raydelv    (501) staff       (20)      293 2024-02-14 01:35:51.000000 vlite2-3.4.0/vlite2.egg-info/PKG-INFO
--rw-r--r--   0 raydelv    (501) staff       (20)      274 2024-02-14 01:35:51.000000 vlite2-3.4.0/vlite2.egg-info/SOURCES.txt
--rw-r--r--   0 raydelv    (501) staff       (20)        1 2024-02-14 01:35:51.000000 vlite2-3.4.0/vlite2.egg-info/dependency_links.txt
--rw-r--r--   0 raydelv    (501) staff       (20)       74 2024-02-14 01:35:51.000000 vlite2-3.4.0/vlite2.egg-info/requires.txt
--rw-r--r--   0 raydelv    (501) staff       (20)        7 2024-02-14 01:35:51.000000 vlite2-3.4.0/vlite2.egg-info/top_level.txt
+drwxr-xr-x   0 raydelv    (501) staff       (20)        0 2024-06-02 19:38:10.629468 vlite2-3.5.0/
+-rw-r--r--   0 raydelv    (501) staff       (20)    34523 2023-11-27 04:55:35.000000 vlite2-3.5.0/LICENSE
+-rw-r--r--   0 raydelv    (501) staff       (20)      293 2024-06-02 19:38:10.629339 vlite2-3.5.0/PKG-INFO
+-rw-r--r--   0 raydelv    (501) staff       (20)    10853 2024-06-02 19:37:27.000000 vlite2-3.5.0/README.md
+-rw-r--r--   0 raydelv    (501) staff       (20)       38 2024-06-02 19:38:10.629533 vlite2-3.5.0/setup.cfg
+-rw-r--r--   0 raydelv    (501) staff       (20)      570 2024-06-02 19:37:30.000000 vlite2-3.5.0/setup.py
+drwxr-xr-x   0 raydelv    (501) staff       (20)        0 2024-06-02 19:38:10.627869 vlite2-3.5.0/test/
+-rw-r--r--   0 raydelv    (501) staff       (20)    27098 2024-06-02 19:35:46.000000 vlite2-3.5.0/test/test.py
+drwxr-xr-x   0 raydelv    (501) staff       (20)        0 2024-06-02 19:38:10.628549 vlite2-3.5.0/vlite2/
+-rw-r--r--   0 raydelv    (501) staff       (20)       90 2024-02-14 01:27:54.000000 vlite2-3.5.0/vlite2/__init__.py
+-rw-r--r--   0 raydelv    (501) staff       (20)     4868 2024-02-14 01:29:41.000000 vlite2-3.5.0/vlite2/ingestors.py
+-rw-r--r--   0 raydelv    (501) staff       (20)     8635 2024-06-02 19:36:34.000000 vlite2-3.5.0/vlite2/main.py
+-rw-r--r--   0 raydelv    (501) staff       (20)     2232 2024-06-02 19:28:04.000000 vlite2-3.5.0/vlite2/model.py
+-rw-r--r--   0 raydelv    (501) staff       (20)      892 2024-06-02 19:21:52.000000 vlite2-3.5.0/vlite2/utils.py
+drwxr-xr-x   0 raydelv    (501) staff       (20)        0 2024-06-02 19:38:10.629149 vlite2-3.5.0/vlite2.egg-info/
+-rw-r--r--   0 raydelv    (501) staff       (20)      293 2024-06-02 19:38:10.000000 vlite2-3.5.0/vlite2.egg-info/PKG-INFO
+-rw-r--r--   0 raydelv    (501) staff       (20)      274 2024-06-02 19:38:10.000000 vlite2-3.5.0/vlite2.egg-info/SOURCES.txt
+-rw-r--r--   0 raydelv    (501) staff       (20)        1 2024-06-02 19:38:10.000000 vlite2-3.5.0/vlite2.egg-info/dependency_links.txt
+-rw-r--r--   0 raydelv    (501) staff       (20)       74 2024-06-02 19:38:10.000000 vlite2-3.5.0/vlite2.egg-info/requires.txt
+-rw-r--r--   0 raydelv    (501) staff       (20)        7 2024-06-02 19:38:10.000000 vlite2-3.5.0/vlite2.egg-info/top_level.txt
```

### Comparing `vlite2-3.4.0/LICENSE` & `vlite2-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vlite2-3.4.0/setup.py` & `vlite2-3.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vlite2',
-    version='3.4.0',
+    version='3.5.0',
     author='Ray Del Vecchio',
     author_email='ray@cerebralvalley.ai',
     description='Improved simple vector database, with many advanced proprietary features. Original VLite by @sdan.',
     url='https://github.com/raydelvecchio/vlite-v2',
     packages=find_packages(),
     install_requires=[
         'numpy',
```

### Comparing `vlite2-3.4.0/test/test.py` & `vlite2-3.5.0/test/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import glob
 import sys
+import numpy as np
 sys.path.append(os.path.join(os.path.dirname(__file__), '../'))
 import unittest
 from vlite2 import VLite2
 
 
 class TestVLite(unittest.TestCase):
     def setUp(self):
@@ -42,14 +43,26 @@
 
         print(self.vlite.retrieve('Star Wars', top_k=2, autocut=True))
         print("[test_autocut] with 2 clusters")
 
         print(self.vlite.retrieve('Star Wars', top_k=3, autocut=True, get_metadata=True, get_similarities=True))
         print("[test_autocut] with 3 clusters")
 
+    def test_random_vector_retrieve(self):
+        self.vlite.ingest("Hello there", metadata={"test": "123"})
+        self.vlite.ingest("I am obi wan")
+        self.vlite.ingest("Ray Del Vecchio")
+        self.vlite.ingest("Ivan is cool")
+        self.vlite.ingest("What's up")
+        self.vlite.ingest("Testing these functions")
+        self.vlite.ingest("Vectors are lit")
+        self.vlite.ingest("Minecraft")
+        random_vector = np.random.rand(self.vlite._VLite2__embed_model.dimension).astype(np.float32)
+        print(self.vlite.retrieve(vector=random_vector, top_k=3))
+        print("[test_random_vector_retrieve] complete")
 
 if __name__ == '__main__':
     unittest.main(exit=False)
 
     files_to_delete = glob.glob('*.index') + glob.glob('*.info')
     for file_path in files_to_delete:
         try:
```

### Comparing `vlite2-3.4.0/vlite2/ingestors.py` & `vlite2-3.5.0/vlite2/ingestors.py`

 * *Files identical despite different names*

### Comparing `vlite2-3.4.0/vlite2/main.py` & `vlite2-3.5.0/vlite2/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         Ingests the input text and returns the DOCUMENT ID (not chunk ID) associated with it in the database.
         """
         if not isinstance(text, str):
             raise TypeError("The 'text' argument must be a string.")
         if metadata and not isinstance(metadata, dict):
             raise TypeError("The 'metadata' argument must be a dict.")
 
+        if not text:
+            raise ValueError("Must input valid text, not null or empty values")
+
         chunks = chop_and_chunk(text, max_seq_length=max_seq_length)
         encoded_chunks = self.__embed_model.embed(texts=chunks, device=self.device)  # this is a numpy array, where each row is the vector for each chunk in chunks
         
         keys = np.arange(self.__chunk_id, self.__chunk_id + len(chunks))
         self.__index.add(keys=keys, vectors=encoded_chunks)  # if you pass in ndarray, ndarray for keys, vectors, it processes in a batch add matching key to row (see USearch docs)
 
         for chunk in chunks:
@@ -61,28 +64,40 @@
             self.__chunk_id += 1
 
         self.__document_id += 1
         self.save()
 
         return self.__document_id - 1
 
-    def retrieve(self, text: str, top_k: int = 3, autocut: bool = False, autocut_amount: int = 25, get_metadata: bool = False, get_similarities: bool = False, progress: bool = False) -> dict:
+    def retrieve(self, text: str = None, vector: np.ndarray = None, top_k: int = 3, autocut: bool = False, autocut_amount: int = 25, get_metadata: bool = False, get_similarities: bool = False, progress: bool = False) -> dict:
         """
-        Method to retrieve vectors given text. Will always return the text, and can specify what else
+        Method to retrieve vectors given text or a vector. Will always return the text, and can specify what else
         we want to return with the get_THING flag. If we set autocut=True, top_k will function as the number of
         CLUSTERS to return, not results. autocut_amount is how many items we run the autocut algorithm over.
         """
-        if not isinstance(text, str):
+        if text is not None and not isinstance(text, str):
             raise TypeError("The 'text' argument must be a string.")
+        if vector is not None and not isinstance(vector, np.ndarray):
+            raise TypeError("The 'vector' argument must be a numpy array.")
+        if vector is not None and vector.shape[0] != self.__embed_model.dimension:
+            raise ValueError(f"The 'vector' argument must have the size {self.__embed_model.dimension}.")
         if top_k <= 0:
             raise Exception("Please input k >= 1.")
+        
+        if text is None and vector is None:
+            raise ValueError("Must input either valid text or a vector, not null or empty values")
 
         count = autocut_amount if autocut else top_k  # sets the amount of elements we want to autocut over here
 
-        matches: Matches = self.__index.search(self.__embed_model.embed(texts=text, device=self.device), count=count, log=progress)
+        if text is not None:
+            query_vector = self.__embed_model.embed(texts=[text], device=self.device)[0]
+        else:
+            query_vector = vector
+
+        matches: Matches = self.__index.search(query_vector, count=count, log=progress)
         matches = matches.to_list()
 
         indices = [match[0] for match in matches]  # indices of the top matches used to retrieve the text and metadata
         scores = [match[1] for match in matches]  # cosine similarity scores in order of descending similarity (ascending value when returned by usearch)
 
         if autocut:
             sim_diff = np.diff(scores)
```

### Comparing `vlite2-3.4.0/vlite2/model.py` & `vlite2-3.5.0/vlite2/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, model_name='all-MiniLM-L6-v2'):
         self.tokenizer = AutoTokenizer.from_pretrained(f"sentence-transformers/{model_name}", use_fast=True)
 
         self.model = AutoModel.from_pretrained(f"sentence-transformers/{model_name}")
         self.dimension = self.model.embeddings.position_embeddings.embedding_dim
         self.max_seq_length = self.model.embeddings.position_embeddings.num_embeddings
 
-    def embed(self, texts, max_seq_length=256, device="mps"):
+    def embed(self, texts, max_seq_length: int = 256, device: str = "mps"):
         if(torch.backends.mps.is_available()):
             dev = torch.device("mps")
         else:
             dev = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
         device = torch.device(dev)
         self.model.to(device)
```

### Comparing `vlite2-3.4.0/vlite2/utils.py` & `vlite2-3.5.0/vlite2/utils.py`

 * *Files identical despite different names*

