# Comparing `tmp/aixhello-2.7.tar.gz` & `tmp/aixhello-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-2.7.tar", last modified: Sat Jun  1 22:34:46 2024, max compression
+gzip compressed data, was "aixhello-3.0.tar", last modified: Sat Jun  1 22:52:14 2024, max compression
```

## Comparing `aixhello-2.7.tar` & `aixhello-3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 22:34:46.583213 aixhello-2.7/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-2.7/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      650 2024-06-01 22:34:46.582211 aixhello-2.7/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 22:34:46.562580 aixhello-2.7/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-2.7/aixhello/__init__.py
--rw-rw-rw-   0        0        0   460036 2024-06-01 22:34:38.000000 aixhello-2.7/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-01 22:34:46.581210 aixhello-2.7/aixhello.egg-info/
--rw-rw-rw-   0        0        0      650 2024-06-01 22:34:46.000000 aixhello-2.7/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-01 22:34:46.000000 aixhello-2.7/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 22:34:46.000000 aixhello-2.7/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-01 22:34:46.000000 aixhello-2.7/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 22:34:46.000000 aixhello-2.7/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-01 22:34:46.585212 aixhello-2.7/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-01 22:34:15.000000 aixhello-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:14.235448 aixhello-3.0/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.0/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-01 22:52:14.235448 aixhello-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:14.214449 aixhello-3.0/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.0/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   460705 2024-06-01 22:52:04.000000 aixhello-3.0/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-01 22:52:14.233446 aixhello-3.0/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-01 22:52:14.000000 aixhello-3.0/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-01 22:52:14.000000 aixhello-3.0/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 22:52:14.000000 aixhello-3.0/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-01 22:52:14.000000 aixhello-3.0/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 22:52:14.000000 aixhello-3.0/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-01 22:52:14.237448 aixhello-3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-01 22:51:41.000000 aixhello-3.0/setup.py
```

### Comparing `aixhello-2.7/LICENSE` & `aixhello-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-2.7/aixhello/xyello.c` & `aixhello-3.0/aixhello/xyello.c`

 * *Files 0% similar despite different names*

```diff
@@ -2339,21 +2339,22 @@
 static const char __pyx_k_xyellw___reduce_cython[] = "xyellw.__reduce_cython__";
 static const char __pyx_k_xyellw___setstate_cython[] = "xyellw.__setstate_cython__";
 static const char __pyx_k_cryptography_hazmat_backends[] = "cryptography.hazmat.backends";
 static const char __pyx_k_Access_Control_Request_Headers[] = "Access-Control-Request-Headers";
 static const char __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN[] = "M#rztXq3z@U8rS5jN@PvE4W7F&J(#DhN";
 static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4BFhKWk32xGPxL9k3jhhHkDqcCQrX37yfmobUNPTXxEGQ==";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())";
+static const char __pyx_k_Successfully_save_to_the_databas[] = "Successfully save to the database.";
 static const char __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1[] = "aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1cmUvc0xwaG9RdURybDZv";
 static const char __pyx_k_cryptography_hazmat_primitives_c[] = "cryptography.hazmat.primitives.ciphers";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
@@ -2396,14 +2397,15 @@
   PyObject *__pyx_n_s_Decipherx;
   PyObject *__pyx_n_s_Embedshroud;
   PyObject *__pyx_n_s_Encapseal;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_n_s_SaveToMongoDb;
+  PyObject *__pyx_kp_u_Successfully_save_to_the_databas;
   PyObject *__pyx_n_s__25;
   PyObject *__pyx_n_s__6;
   PyObject *__pyx_kp_u__6;
   PyObject *__pyx_kp_u__8;
   PyObject *__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1;
   PyObject *__pyx_n_s_aixhello_xyello;
   PyObject *__pyx_kp_s_aixhello_xyello_pyx;
@@ -2604,14 +2606,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_Decipherx);
   Py_CLEAR(clear_module_state->__pyx_n_s_Embedshroud);
   Py_CLEAR(clear_module_state->__pyx_n_s_Encapseal);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_SaveToMongoDb);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
   Py_CLEAR(clear_module_state->__pyx_n_s__25);
   Py_CLEAR(clear_module_state->__pyx_n_s__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__8);
   Py_CLEAR(clear_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_CLEAR(clear_module_state->__pyx_n_s_aixhello_xyello);
   Py_CLEAR(clear_module_state->__pyx_kp_s_aixhello_xyello_pyx);
@@ -2790,14 +2793,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_Decipherx);
   Py_VISIT(traverse_module_state->__pyx_n_s_Embedshroud);
   Py_VISIT(traverse_module_state->__pyx_n_s_Encapseal);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_SaveToMongoDb);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
   Py_VISIT(traverse_module_state->__pyx_n_s__25);
   Py_VISIT(traverse_module_state->__pyx_n_s__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__8);
   Py_VISIT(traverse_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_VISIT(traverse_module_state->__pyx_n_s_aixhello_xyello);
   Py_VISIT(traverse_module_state->__pyx_kp_s_aixhello_xyello_pyx);
@@ -2986,14 +2990,15 @@
 #define __pyx_n_s_Decipherx __pyx_mstate_global->__pyx_n_s_Decipherx
 #define __pyx_n_s_Embedshroud __pyx_mstate_global->__pyx_n_s_Embedshroud
 #define __pyx_n_s_Encapseal __pyx_mstate_global->__pyx_n_s_Encapseal
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN __pyx_mstate_global->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_n_s_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_SaveToMongoDb
+#define __pyx_kp_u_Successfully_save_to_the_databas __pyx_mstate_global->__pyx_kp_u_Successfully_save_to_the_databas
 #define __pyx_n_s__25 __pyx_mstate_global->__pyx_n_s__25
 #define __pyx_n_s__6 __pyx_mstate_global->__pyx_n_s__6
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
 #define __pyx_kp_u__8 __pyx_mstate_global->__pyx_kp_u__8
 #define __pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1 __pyx_mstate_global->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1
 #define __pyx_n_s_aixhello_xyello __pyx_mstate_global->__pyx_n_s_aixhello_xyello
 #define __pyx_kp_s_aixhello_xyello_pyx __pyx_mstate_global->__pyx_kp_s_aixhello_xyello_pyx
@@ -4344,121 +4349,147 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key) {
   PyObject *__pyx_v_embeddings = NULL;
   PyObject *__pyx_v_chunk = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_embedding = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
+  PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  int __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Embedshroud", 1);
 
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_openai); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_api_key, __pyx_v_text_key) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_text_key};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_openai); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_t_2, __pyx_n_s_api_key, __pyx_t_1) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_embeddings = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_embeddings = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
 
   if (unlikely(__pyx_v_text_chunks == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
     __PYX_ERR(0, 51, __pyx_L1_error)
   }
-  __pyx_t_1 = __pyx_v_text_chunks; __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = 0;
+  __pyx_t_2 = __pyx_v_text_chunks; __Pyx_INCREF(__pyx_t_2);
+  __pyx_t_5 = 0;
   for (;;) {
     {
-      Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+      Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
       #if !CYTHON_ASSUME_SAFE_MACROS
       if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
       #endif
-      if (__pyx_t_2 >= __pyx_temp) break;
+      if (__pyx_t_5 >= __pyx_temp) break;
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
+    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
     #else
-    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     #endif
-    __Pyx_XDECREF_SET(__pyx_v_chunk, __pyx_t_3);
-    __pyx_t_3 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_chunk, __pyx_t_1);
+    __pyx_t_1 = 0;
 
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_openai); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_openai); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_create); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_create); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
 
-    __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 54, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_v_chunk);
     __Pyx_GIVEREF(__pyx_v_chunk);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_v_chunk)) __PYX_ERR(0, 54, __pyx_L1_error);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_input, __pyx_t_5) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_v_chunk)) __PYX_ERR(0, 54, __pyx_L1_error);
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_input, __pyx_t_6) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_response, __pyx_t_5);
-    __pyx_t_5 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_response, __pyx_t_6);
+    __pyx_t_6 = 0;
 
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_embedding); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_embedding, __pyx_t_5);
-    __pyx_t_5 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_embedding); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_embedding, __pyx_t_6);
+    __pyx_t_6 = 0;
 
-    __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_embeddings, __pyx_v_embedding); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_embeddings, __pyx_v_embedding); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
 
   }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_embeddings);
   __pyx_r = __pyx_v_embeddings;
   goto __pyx_L0;
 
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_embeddings);
   __Pyx_XDECREF(__pyx_v_chunk);
   __Pyx_XDECREF(__pyx_v_response);
   __Pyx_XDECREF(__pyx_v_embedding);
@@ -4778,40 +4809,16 @@
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_3, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_7) {
 
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_1 = NULL;
-    __pyx_t_4 = 0;
-    #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_1);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
-        __pyx_t_4 = 1;
-      }
-    }
-    #endif
-    {
-      PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
-      __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    }
-    __pyx_r = __pyx_t_3;
-    __pyx_t_3 = 0;
+    __Pyx_INCREF(__pyx_kp_u_Successfully_save_to_the_databas);
+    __pyx_r = __pyx_kp_u_Successfully_save_to_the_databas;
     goto __pyx_L0;
 
   }
 
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
@@ -5624,14 +5631,15 @@
     {&__pyx_n_s_Decipherx, __pyx_k_Decipherx, sizeof(__pyx_k_Decipherx), 0, 0, 1, 1},
     {&__pyx_n_s_Embedshroud, __pyx_k_Embedshroud, sizeof(__pyx_k_Embedshroud), 0, 0, 1, 1},
     {&__pyx_n_s_Encapseal, __pyx_k_Encapseal, sizeof(__pyx_k_Encapseal), 0, 0, 1, 1},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, sizeof(__pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN), 0, 0, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_SaveToMongoDb, __pyx_k_SaveToMongoDb, sizeof(__pyx_k_SaveToMongoDb), 0, 0, 1, 1},
+    {&__pyx_kp_u_Successfully_save_to_the_databas, __pyx_k_Successfully_save_to_the_databas, sizeof(__pyx_k_Successfully_save_to_the_databas), 0, 1, 0, 0},
     {&__pyx_n_s__25, __pyx_k__25, sizeof(__pyx_k__25), 0, 0, 1, 1},
     {&__pyx_n_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
     {&__pyx_kp_u__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 1, 0, 0},
     {&__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, sizeof(__pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1), 0, 1, 0, 1},
     {&__pyx_n_s_aixhello_xyello, __pyx_k_aixhello_xyello, sizeof(__pyx_k_aixhello_xyello), 0, 0, 1, 1},
     {&__pyx_kp_s_aixhello_xyello_pyx, __pyx_k_aixhello_xyello_pyx, sizeof(__pyx_k_aixhello_xyello_pyx), 0, 0, 1, 0},
```

### Comparing `aixhello-2.7/setup.py` & `aixhello-3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='2.7',  # Increment the version number
+    version='3.0',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

