# Comparing `tmp/En-transformer-1.6.5.tar.gz` & `tmp/en_transformer-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "En-transformer-1.6.5.tar", last modified: Wed Jan 17 23:24:16 2024, max compression
+gzip compressed data, was "en_transformer-1.6.6.tar", last modified: Sun Jun  2 15:20:16 2024, max compression
```

## Comparing `En-transformer-1.6.5.tar` & `en_transformer-1.6.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 23:24:16.528329 En-transformer-1.6.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 23:24:16.528329 En-transformer-1.6.5/En_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-17 23:24:16.000000 En-transformer-1.6.5/En_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-17 23:24:16.000000 En-transformer-1.6.5/En_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 23:24:16.000000 En-transformer-1.6.5/En_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-17 23:24:16.000000 En-transformer-1.6.5/En_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-17 23:24:16.000000 En-transformer-1.6.5/En_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-17 23:24:07.000000 En-transformer-1.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-17 23:24:16.528329 En-transformer-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-01-17 23:24:07.000000 En-transformer-1.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 23:24:16.524329 En-transformer-1.6.5/en_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-17 23:24:07.000000 En-transformer-1.6.5/en_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22202 2024-01-17 23:24:07.000000 En-transformer-1.6.5/en_transformer/en_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-01-17 23:24:07.000000 En-transformer-1.6.5/en_transformer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-17 23:24:16.528329 En-transformer-1.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-01-17 23:24:07.000000 En-transformer-1.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 23:24:16.528329 En-transformer-1.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-01-17 23:24:07.000000 En-transformer-1.6.5/tests/test_equivariance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:20:16.266332 en_transformer-1.6.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:20:16.266332 en_transformer-1.6.6/En_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-06-02 15:20:16.000000 en_transformer-1.6.6/En_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-02 15:20:16.000000 en_transformer-1.6.6/En_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 15:20:16.000000 en_transformer-1.6.6/En_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-02 15:20:16.000000 en_transformer-1.6.6/En_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 15:20:16.000000 en_transformer-1.6.6/En_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-06-02 15:20:11.000000 en_transformer-1.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-06-02 15:20:16.266332 en_transformer-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-06-02 15:20:11.000000 en_transformer-1.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:20:16.266332 en_transformer-1.6.6/en_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-02 15:20:11.000000 en_transformer-1.6.6/en_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22440 2024-06-02 15:20:11.000000 en_transformer-1.6.6/en_transformer/en_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-06-02 15:20:11.000000 en_transformer-1.6.6/en_transformer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-02 15:20:16.270332 en_transformer-1.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-06-02 15:20:11.000000 en_transformer-1.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 15:20:16.266332 en_transformer-1.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-06-02 15:20:11.000000 en_transformer-1.6.6/tests/test_equivariance.py
```

### Comparing `En-transformer-1.6.5/En_transformer.egg-info/PKG-INFO` & `en_transformer-1.6.6/En_transformer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: En-transformer
-Version: 1.6.5
+Version: 1.6.6
 Summary: E(n)-Equivariant Transformer
 Home-page: https://github.com/lucidrains/En-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: einops>=0.3
+Requires-Dist: einops>=0.8
 Requires-Dist: einx
 Requires-Dist: taylor-series-linear-attention>=0.1.4
 Requires-Dist: torch>=1.7
```

### Comparing `En-transformer-1.6.5/LICENSE` & `en_transformer-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `En-transformer-1.6.5/PKG-INFO` & `en_transformer-1.6.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: En-transformer
-Version: 1.6.5
+Version: 1.6.6
 Summary: E(n)-Equivariant Transformer
 Home-page: https://github.com/lucidrains/En-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: einops>=0.3
+Requires-Dist: einops>=0.8
 Requires-Dist: einx
 Requires-Dist: taylor-series-linear-attention>=0.1.4
 Requires-Dist: torch>=1.7
```

### Comparing `En-transformer-1.6.5/README.md` & `en_transformer-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `En-transformer-1.6.5/en_transformer/en_transformer.py` & `en_transformer-1.6.6/en_transformer/en_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,36 +158,43 @@
         dropout = 0.,
         num_global_linear_attn_heads = 0,
         linear_attn_dim_head = 8,
         gate_outputs = True,
         gate_init_bias = 10.
     ):
         super().__init__()
+        neighbors = default(neighbors, 0)
+        neighbors = max(neighbors, 0)
+
         self.scale = dim_head ** -0.5
         self.norm = LayerNorm(dim)
 
         self.neighbors = neighbors
         self.only_sparse_neighbors = only_sparse_neighbors
         self.valid_neighbor_radius = valid_neighbor_radius
 
         attn_inner_dim = heads * dim_head
         self.heads = heads
 
         self.has_linear_attn = num_global_linear_attn_heads > 0
 
-        self.linear_attn = TaylorSeriesLinearAttn(
-            dim = dim,
-            dim_head = linear_attn_dim_head,
-            heads = num_global_linear_attn_heads,
-            gate_value_heads = True,
-            combine_heads = False
-        )
+        linear_attn_dim_hidden = 0
+        if self.has_linear_attn:
+            self.linear_attn = TaylorSeriesLinearAttn(
+                dim = dim,
+                dim_head = linear_attn_dim_head,
+                heads = num_global_linear_attn_heads,
+                gate_value_heads = True,
+                combine_heads = False
+            )
+
+            linear_attn_dim_hidden = self.linear_attn.dim_hidden
 
         self.to_qkv = nn.Linear(dim, attn_inner_dim * 3, bias = False)
-        self.to_out = nn.Linear(attn_inner_dim + self.linear_attn.dim_hidden, dim)
+        self.to_out = nn.Linear(attn_inner_dim + linear_attn_dim_hidden, dim)
 
         self.gate_outputs = gate_outputs
         if gate_outputs:
             gate_linear = nn.Linear(dim, 2 * heads)
             nn.init.zeros_(gate_linear.weight)
             nn.init.constant_(gate_linear.bias, gate_init_bias)
```

### Comparing `En-transformer-1.6.5/setup.py` & `en_transformer-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'En-transformer',
   packages = find_packages(),
-  version = '1.6.5',
+  version = '1.6.6',
   license='MIT',
   description = 'E(n)-Equivariant Transformer',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/En-transformer',
   keywords = [
     'artificial intelligence',
     'deep learning',
     'equivariance',
     'transformer'
   ],
   install_requires=[
-    'einops>=0.3',
+    'einops>=0.8',
     'einx',
     'taylor-series-linear-attention>=0.1.4',
     'torch>=1.7'
   ],
   setup_requires=[
     'pytest-runner',
   ],
```

### Comparing `En-transformer-1.6.5/tests/test_equivariance.py` & `en_transformer-1.6.6/tests/test_equivariance.py`

 * *Files identical despite different names*

