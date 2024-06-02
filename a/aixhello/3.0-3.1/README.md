# Comparing `tmp/aixhello-3.0.tar.gz` & `tmp/aixhello-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-3.0.tar", last modified: Sat Jun  1 22:52:14 2024, max compression
+gzip compressed data, was "aixhello-3.1.tar", last modified: Sat Jun  1 22:58:53 2024, max compression
```

## Comparing `aixhello-3.0.tar` & `aixhello-3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 22:52:14.235448 aixhello-3.0/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.0/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-01 22:52:14.235448 aixhello-3.0/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 22:52:14.214449 aixhello-3.0/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.0/aixhello/__init__.py
--rw-rw-rw-   0        0        0   460705 2024-06-01 22:52:04.000000 aixhello-3.0/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-01 22:52:14.233446 aixhello-3.0/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-01 22:52:14.000000 aixhello-3.0/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-01 22:52:14.000000 aixhello-3.0/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 22:52:14.000000 aixhello-3.0/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-01 22:52:14.000000 aixhello-3.0/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 22:52:14.000000 aixhello-3.0/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-01 22:52:14.237448 aixhello-3.0/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-01 22:51:41.000000 aixhello-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:58:53.568932 aixhello-3.1/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.1/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-01 22:58:53.568932 aixhello-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 22:58:53.546167 aixhello-3.1/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.1/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   479773 2024-06-01 22:58:46.000000 aixhello-3.1/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-01 22:58:53.566933 aixhello-3.1/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-01 22:58:53.000000 aixhello-3.1/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-01 22:58:53.000000 aixhello-3.1/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 22:58:53.000000 aixhello-3.1/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-01 22:58:53.000000 aixhello-3.1/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 22:58:53.000000 aixhello-3.1/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-01 22:58:53.570932 aixhello-3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-01 22:58:25.000000 aixhello-3.1/setup.py
```

### Comparing `aixhello-3.0/LICENSE` & `aixhello-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-3.0/PKG-INFO` & `aixhello-3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.0
+Version: 3.1
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.0/README.md` & `aixhello-3.1/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-3.0/aixhello/xyello.c` & `aixhello-3.1/aixhello/xyello.c`

 * *Files 1% similar despite different names*

```diff
@@ -1886,14 +1886,63 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* FastTypeChecks.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
+static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
+static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
+#else
+#define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
+#define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
+#define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
+#endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
+#define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* SwapException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
 /* PyIntCompare.proto */
 static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
 /* KeywordStringCheck.proto */
 static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
 
 /* GetAttr3.proto */
@@ -2168,31 +2217,14 @@
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
-/* FastTypeChecks.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
-#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
-static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
-static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
-static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
-static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
-#else
-#define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
-#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
-#define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
-#define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
-#endif
-#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
-#define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
-
 /* CheckBinaryVersion.proto */
 static unsigned long __Pyx_get_runtime_version(void);
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
@@ -2207,14 +2239,15 @@
 int __pyx_module_is_main_aixhello__xyello = 0;
 
 /* Implementation of "aixhello.xyello" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_chr;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = "";
+static const char __pyx_k_e[] = "e";
 static const char __pyx_k__6[] = "*";
 static const char __pyx_k__8[] = ".";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_iv[] = "iv";
 static const char __pyx_k_AES[] = "AES";
 static const char __pyx_k_CBC[] = "CBC";
 static const char __pyx_k__25[] = "?";
@@ -2326,22 +2359,25 @@
 static const char __pyx_k_xyellw_Decenigma[] = "xyellw.Decenigma";
 static const char __pyx_k_xyellw_Decipherx[] = "xyellw.Decipherx";
 static const char __pyx_k_xyellw_Encapseal[] = "xyellw.Encapseal";
 static const char __pyx_k_y1c8_8BxP9XN_VKM[] = "y1c8@8BxP9XN#VKM";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_xyellw_Embedshroud[] = "xyellw.Embedshroud";
+static const char __pyx_k_AuthenticationError[] = "AuthenticationError";
 static const char __pyx_k_aixhello_xyello_pyx[] = "aixhello\\xyello.pyx";
 static const char __pyx_k_pyx_unpickle_xyellw[] = "__pyx_unpickle_xyellw";
 static const char __pyx_k_xyellw_SaveToMongoDb[] = "xyellw.SaveToMongoDb";
 static const char __pyx_k_decoded_encryptedText[] = "decoded_encryptedText";
 static const char __pyx_k_decrypted_padded_text[] = "decrypted_padded_text";
 static const char __pyx_k_text_embedding_ada_002[] = "text-embedding-ada-002";
 static const char __pyx_k_xyellw___reduce_cython[] = "xyellw.__reduce_cython__";
+static const char __pyx_k_Invalid_API_key_provided[] = "Invalid API key provided";
 static const char __pyx_k_xyellw___setstate_cython[] = "xyellw.__setstate_cython__";
+static const char __pyx_k_An_unexpected_error_occurred[] = "An unexpected error occurred";
 static const char __pyx_k_cryptography_hazmat_backends[] = "cryptography.hazmat.backends";
 static const char __pyx_k_Access_Control_Request_Headers[] = "Access-Control-Request-Headers";
 static const char __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN[] = "M#rztXq3z@U8rS5jN@PvE4W7F&J(#DhN";
 static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4BFhKWk32xGPxL9k3jhhHkDqcCQrX37yfmobUNPTXxEGQ==";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())";
 static const char __pyx_k_Successfully_save_to_the_databas[] = "Successfully save to the database.";
 static const char __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1[] = "aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1cmUvc0xwaG9RdURybDZv";
@@ -2386,22 +2422,25 @@
   #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_8aixhello_6xyello_xyellw;
   #endif
   PyTypeObject *__pyx_ptype_8aixhello_6xyello_xyellw;
   PyObject *__pyx_kp_u_;
   PyObject *__pyx_n_s_AES;
   PyObject *__pyx_kp_u_Access_Control_Request_Headers;
+  PyObject *__pyx_kp_u_An_unexpected_error_occurred;
+  PyObject *__pyx_n_s_AuthenticationError;
   PyObject *__pyx_n_s_CBC;
   PyObject *__pyx_n_s_Cipher;
   PyObject *__pyx_kp_u_Content_Type;
   PyObject *__pyx_n_s_Decenigma;
   PyObject *__pyx_n_s_Decipherx;
   PyObject *__pyx_n_s_Embedshroud;
   PyObject *__pyx_n_s_Encapseal;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+  PyObject *__pyx_kp_u_Invalid_API_key_provided;
   PyObject *__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_n_s_SaveToMongoDb;
   PyObject *__pyx_kp_u_Successfully_save_to_the_databas;
   PyObject *__pyx_n_s__25;
   PyObject *__pyx_n_s__6;
   PyObject *__pyx_kp_u__6;
@@ -2441,14 +2480,15 @@
   PyObject *__pyx_n_s_decrypted_padded_text;
   PyObject *__pyx_n_s_decrypted_url;
   PyObject *__pyx_n_s_decryptor;
   PyObject *__pyx_n_s_default_backend;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_dict_2;
   PyObject *__pyx_kp_u_disable;
+  PyObject *__pyx_n_s_e;
   PyObject *__pyx_n_s_embedding;
   PyObject *__pyx_n_s_embeddings;
   PyObject *__pyx_kp_u_enable;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_encoded_url;
   PyObject *__pyx_n_s_encryptedText;
   PyObject *__pyx_n_s_encryptor;
@@ -2595,22 +2635,25 @@
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_8aixhello_6xyello_xyellw);
   Py_CLEAR(clear_module_state->__pyx_type_8aixhello_6xyello_xyellw);
   Py_CLEAR(clear_module_state->__pyx_kp_u_);
   Py_CLEAR(clear_module_state->__pyx_n_s_AES);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Access_Control_Request_Headers);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_An_unexpected_error_occurred);
+  Py_CLEAR(clear_module_state->__pyx_n_s_AuthenticationError);
   Py_CLEAR(clear_module_state->__pyx_n_s_CBC);
   Py_CLEAR(clear_module_state->__pyx_n_s_Cipher);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Content_Type);
   Py_CLEAR(clear_module_state->__pyx_n_s_Decenigma);
   Py_CLEAR(clear_module_state->__pyx_n_s_Decipherx);
   Py_CLEAR(clear_module_state->__pyx_n_s_Embedshroud);
   Py_CLEAR(clear_module_state->__pyx_n_s_Encapseal);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_API_key_provided);
   Py_CLEAR(clear_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_SaveToMongoDb);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
   Py_CLEAR(clear_module_state->__pyx_n_s__25);
   Py_CLEAR(clear_module_state->__pyx_n_s__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
@@ -2650,14 +2693,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_decrypted_padded_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_decrypted_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_decryptor);
   Py_CLEAR(clear_module_state->__pyx_n_s_default_backend);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict_2);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_e);
   Py_CLEAR(clear_module_state->__pyx_n_s_embedding);
   Py_CLEAR(clear_module_state->__pyx_n_s_embeddings);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_encoded_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptor);
@@ -2782,22 +2826,25 @@
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_8aixhello_6xyello_xyellw);
   Py_VISIT(traverse_module_state->__pyx_type_8aixhello_6xyello_xyellw);
   Py_VISIT(traverse_module_state->__pyx_kp_u_);
   Py_VISIT(traverse_module_state->__pyx_n_s_AES);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Access_Control_Request_Headers);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_An_unexpected_error_occurred);
+  Py_VISIT(traverse_module_state->__pyx_n_s_AuthenticationError);
   Py_VISIT(traverse_module_state->__pyx_n_s_CBC);
   Py_VISIT(traverse_module_state->__pyx_n_s_Cipher);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Content_Type);
   Py_VISIT(traverse_module_state->__pyx_n_s_Decenigma);
   Py_VISIT(traverse_module_state->__pyx_n_s_Decipherx);
   Py_VISIT(traverse_module_state->__pyx_n_s_Embedshroud);
   Py_VISIT(traverse_module_state->__pyx_n_s_Encapseal);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_API_key_provided);
   Py_VISIT(traverse_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_SaveToMongoDb);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
   Py_VISIT(traverse_module_state->__pyx_n_s__25);
   Py_VISIT(traverse_module_state->__pyx_n_s__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
@@ -2837,14 +2884,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_decrypted_padded_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_decrypted_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_decryptor);
   Py_VISIT(traverse_module_state->__pyx_n_s_default_backend);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict_2);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_e);
   Py_VISIT(traverse_module_state->__pyx_n_s_embedding);
   Py_VISIT(traverse_module_state->__pyx_n_s_embeddings);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_encoded_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptor);
@@ -2979,22 +3027,25 @@
 #if CYTHON_USE_MODULE_STATE
 #define __pyx_type_8aixhello_6xyello_xyellw __pyx_mstate_global->__pyx_type_8aixhello_6xyello_xyellw
 #endif
 #define __pyx_ptype_8aixhello_6xyello_xyellw __pyx_mstate_global->__pyx_ptype_8aixhello_6xyello_xyellw
 #define __pyx_kp_u_ __pyx_mstate_global->__pyx_kp_u_
 #define __pyx_n_s_AES __pyx_mstate_global->__pyx_n_s_AES
 #define __pyx_kp_u_Access_Control_Request_Headers __pyx_mstate_global->__pyx_kp_u_Access_Control_Request_Headers
+#define __pyx_kp_u_An_unexpected_error_occurred __pyx_mstate_global->__pyx_kp_u_An_unexpected_error_occurred
+#define __pyx_n_s_AuthenticationError __pyx_mstate_global->__pyx_n_s_AuthenticationError
 #define __pyx_n_s_CBC __pyx_mstate_global->__pyx_n_s_CBC
 #define __pyx_n_s_Cipher __pyx_mstate_global->__pyx_n_s_Cipher
 #define __pyx_kp_u_Content_Type __pyx_mstate_global->__pyx_kp_u_Content_Type
 #define __pyx_n_s_Decenigma __pyx_mstate_global->__pyx_n_s_Decenigma
 #define __pyx_n_s_Decipherx __pyx_mstate_global->__pyx_n_s_Decipherx
 #define __pyx_n_s_Embedshroud __pyx_mstate_global->__pyx_n_s_Embedshroud
 #define __pyx_n_s_Encapseal __pyx_mstate_global->__pyx_n_s_Encapseal
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
+#define __pyx_kp_u_Invalid_API_key_provided __pyx_mstate_global->__pyx_kp_u_Invalid_API_key_provided
 #define __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN __pyx_mstate_global->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_n_s_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_SaveToMongoDb
 #define __pyx_kp_u_Successfully_save_to_the_databas __pyx_mstate_global->__pyx_kp_u_Successfully_save_to_the_databas
 #define __pyx_n_s__25 __pyx_mstate_global->__pyx_n_s__25
 #define __pyx_n_s__6 __pyx_mstate_global->__pyx_n_s__6
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
@@ -3034,14 +3085,15 @@
 #define __pyx_n_s_decrypted_padded_text __pyx_mstate_global->__pyx_n_s_decrypted_padded_text
 #define __pyx_n_s_decrypted_url __pyx_mstate_global->__pyx_n_s_decrypted_url
 #define __pyx_n_s_decryptor __pyx_mstate_global->__pyx_n_s_decryptor
 #define __pyx_n_s_default_backend __pyx_mstate_global->__pyx_n_s_default_backend
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_dict_2 __pyx_mstate_global->__pyx_n_s_dict_2
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
+#define __pyx_n_s_e __pyx_mstate_global->__pyx_n_s_e
 #define __pyx_n_s_embedding __pyx_mstate_global->__pyx_n_s_embedding
 #define __pyx_n_s_embeddings __pyx_mstate_global->__pyx_n_s_embeddings
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_encoded_url __pyx_mstate_global->__pyx_n_s_encoded_url
 #define __pyx_n_s_encryptedText __pyx_mstate_global->__pyx_n_s_encryptedText
 #define __pyx_n_s_encryptor __pyx_mstate_global->__pyx_n_s_encryptor
@@ -4354,149 +4406,347 @@
 }
 
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key) {
   PyObject *__pyx_v_embeddings = NULL;
   PyObject *__pyx_v_chunk = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_embedding = NULL;
+  CYTHON_UNUSED PyObject *__pyx_v_e = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  Py_ssize_t __pyx_t_5;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
+  Py_ssize_t __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
+  int __pyx_t_10;
+  PyObject *__pyx_t_11 = NULL;
+  int __pyx_t_12;
+  char const *__pyx_t_13;
+  PyObject *__pyx_t_14 = NULL;
+  PyObject *__pyx_t_15 = NULL;
+  PyObject *__pyx_t_16 = NULL;
+  PyObject *__pyx_t_17 = NULL;
+  PyObject *__pyx_t_18 = NULL;
+  PyObject *__pyx_t_19 = NULL;
+  char const *__pyx_t_20;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Embedshroud", 1);
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  __pyx_t_4 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-      __pyx_t_4 = 1;
-    }
-  }
-  #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_text_key};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  }
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_openai); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_t_2, __pyx_n_s_api_key, __pyx_t_1) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_6 = NULL;
+      __pyx_t_7 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_6)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_6);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __pyx_t_7 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_v_text_key};
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_openai); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      if (__Pyx_PyObject_SetAttrStr(__pyx_t_5, __pyx_n_s_api_key, __pyx_t_4) < 0) __PYX_ERR(0, 50, __pyx_L3_error)
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_v_embeddings = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
+      __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_v_embeddings = ((PyObject*)__pyx_t_5);
+      __pyx_t_5 = 0;
+
+      if (unlikely(__pyx_v_text_chunks == Py_None)) {
+        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+        __PYX_ERR(0, 52, __pyx_L3_error)
+      }
+      __pyx_t_5 = __pyx_v_text_chunks; __Pyx_INCREF(__pyx_t_5);
+      __pyx_t_8 = 0;
+      for (;;) {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 52, __pyx_L3_error)
+          #endif
+          if (__pyx_t_8 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_8); __Pyx_INCREF(__pyx_t_4); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 52, __pyx_L3_error)
+        #else
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+        __Pyx_XDECREF_SET(__pyx_v_chunk, __pyx_t_4);
+        __pyx_t_4 = 0;
 
-  if (unlikely(__pyx_v_text_chunks == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 51, __pyx_L1_error)
-  }
-  __pyx_t_2 = __pyx_v_text_chunks; __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_5 = 0;
-  for (;;) {
-    {
-      Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
-      #if !CYTHON_ASSUME_SAFE_MACROS
-      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
-      #endif
-      if (__pyx_t_5 >= __pyx_temp) break;
-    }
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 51, __pyx_L1_error)
-    #else
-    __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    #endif
-    __Pyx_XDECREF_SET(__pyx_v_chunk, __pyx_t_1);
-    __pyx_t_1 = 0;
+        __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_openai); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 53, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_create); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+        __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 54, __pyx_L3_error)
+
+        __pyx_t_9 = PyList_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 55, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __Pyx_INCREF(__pyx_v_chunk);
+        __Pyx_GIVEREF(__pyx_v_chunk);
+        if (__Pyx_PyList_SET_ITEM(__pyx_t_9, 0, __pyx_v_chunk)) __PYX_ERR(0, 55, __pyx_L3_error);
+        if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_input, __pyx_t_9) < 0) __PYX_ERR(0, 54, __pyx_L3_error)
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+
+        __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 53, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_response, __pyx_t_9);
+        __pyx_t_9 = 0;
+
+        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 57, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_9, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 57, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_embedding); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 57, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_embedding, __pyx_t_9);
+        __pyx_t_9 = 0;
 
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_openai); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_create); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_embeddings, __pyx_v_embedding); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 58, __pyx_L3_error)
 
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
+      }
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_INCREF(__pyx_v_chunk);
-    __Pyx_GIVEREF(__pyx_v_chunk);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_v_chunk)) __PYX_ERR(0, 54, __pyx_L1_error);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_input, __pyx_t_6) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_XDECREF(__pyx_r);
+      __Pyx_INCREF(__pyx_v_embeddings);
+      __pyx_r = __pyx_v_embeddings;
+      goto __pyx_L7_try_return;
 
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_response, __pyx_t_6);
-    __pyx_t_6 = 0;
+    }
+    __pyx_L3_error:;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_embedding); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_embedding, __pyx_t_6);
-    __pyx_t_6 = 0;
+    __Pyx_ErrFetch(&__pyx_t_5, &__pyx_t_9, &__pyx_t_6);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_openai); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L5_except_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_AuthenticationError); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 60, __pyx_L5_except_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_7 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_5, __pyx_t_11);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __Pyx_ErrRestore(__pyx_t_5, __pyx_t_9, __pyx_t_6);
+    __pyx_t_5 = 0; __pyx_t_9 = 0; __pyx_t_6 = 0;
+    if (__pyx_t_7) {
+      __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_9, &__pyx_t_5) < 0) __PYX_ERR(0, 60, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_9);
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_9);
+      __pyx_v_e = __pyx_t_9;
+      /*try:*/ {
+
+        __Pyx_XDECREF(__pyx_r);
+        __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 61, __pyx_L17_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_error, __pyx_kp_u_Invalid_API_key_provided) < 0) __PYX_ERR(0, 61, __pyx_L17_error)
+        __pyx_r = __pyx_t_11;
+        __pyx_t_11 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        goto __pyx_L16_return;
+      }
 
-    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_embeddings, __pyx_v_embedding); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
+      /*finally:*/ {
+        __pyx_L17_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0;
+          __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+          __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16) < 0)) __Pyx_ErrFetch(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16);
+          __Pyx_XGOTREF(__pyx_t_14);
+          __Pyx_XGOTREF(__pyx_t_15);
+          __Pyx_XGOTREF(__pyx_t_16);
+          __Pyx_XGOTREF(__pyx_t_17);
+          __Pyx_XGOTREF(__pyx_t_18);
+          __Pyx_XGOTREF(__pyx_t_19);
+          __pyx_t_7 = __pyx_lineno; __pyx_t_12 = __pyx_clineno; __pyx_t_13 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_17);
+            __Pyx_XGIVEREF(__pyx_t_18);
+            __Pyx_XGIVEREF(__pyx_t_19);
+            __Pyx_ExceptionReset(__pyx_t_17, __pyx_t_18, __pyx_t_19);
+          }
+          __Pyx_XGIVEREF(__pyx_t_14);
+          __Pyx_XGIVEREF(__pyx_t_15);
+          __Pyx_XGIVEREF(__pyx_t_16);
+          __Pyx_ErrRestore(__pyx_t_14, __pyx_t_15, __pyx_t_16);
+          __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0;
+          __pyx_lineno = __pyx_t_7; __pyx_clineno = __pyx_t_12; __pyx_filename = __pyx_t_13;
+          goto __pyx_L5_except_error;
+        }
+        __pyx_L16_return: {
+          __pyx_t_19 = __pyx_r;
+          __pyx_r = 0;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
+          __pyx_r = __pyx_t_19;
+          __pyx_t_19 = 0;
+          goto __pyx_L6_except_return;
+        }
+      }
+    }
 
-  }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_12 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_12) {
+      __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_9, &__pyx_t_6) < 0) __PYX_ERR(0, 62, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_9);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_INCREF(__pyx_t_9);
+      __pyx_v_e = __pyx_t_9;
+      /*try:*/ {
+
+        __Pyx_XDECREF(__pyx_r);
+        __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 63, __pyx_L28_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_error, __pyx_kp_u_An_unexpected_error_occurred) < 0) __PYX_ERR(0, 63, __pyx_L28_error)
+        __pyx_r = __pyx_t_11;
+        __pyx_t_11 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        goto __pyx_L27_return;
+      }
 
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_embeddings);
-  __pyx_r = __pyx_v_embeddings;
-  goto __pyx_L0;
+      /*finally:*/ {
+        __pyx_L28_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_19 = 0; __pyx_t_18 = 0; __pyx_t_17 = 0; __pyx_t_16 = 0; __pyx_t_15 = 0; __pyx_t_14 = 0;
+          __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+          __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_16, &__pyx_t_15, &__pyx_t_14);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_19, &__pyx_t_18, &__pyx_t_17) < 0)) __Pyx_ErrFetch(&__pyx_t_19, &__pyx_t_18, &__pyx_t_17);
+          __Pyx_XGOTREF(__pyx_t_19);
+          __Pyx_XGOTREF(__pyx_t_18);
+          __Pyx_XGOTREF(__pyx_t_17);
+          __Pyx_XGOTREF(__pyx_t_16);
+          __Pyx_XGOTREF(__pyx_t_15);
+          __Pyx_XGOTREF(__pyx_t_14);
+          __pyx_t_12 = __pyx_lineno; __pyx_t_7 = __pyx_clineno; __pyx_t_20 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_16);
+            __Pyx_XGIVEREF(__pyx_t_15);
+            __Pyx_XGIVEREF(__pyx_t_14);
+            __Pyx_ExceptionReset(__pyx_t_16, __pyx_t_15, __pyx_t_14);
+          }
+          __Pyx_XGIVEREF(__pyx_t_19);
+          __Pyx_XGIVEREF(__pyx_t_18);
+          __Pyx_XGIVEREF(__pyx_t_17);
+          __Pyx_ErrRestore(__pyx_t_19, __pyx_t_18, __pyx_t_17);
+          __pyx_t_19 = 0; __pyx_t_18 = 0; __pyx_t_17 = 0; __pyx_t_16 = 0; __pyx_t_15 = 0; __pyx_t_14 = 0;
+          __pyx_lineno = __pyx_t_12; __pyx_clineno = __pyx_t_7; __pyx_filename = __pyx_t_20;
+          goto __pyx_L5_except_error;
+        }
+        __pyx_L27_return: {
+          __pyx_t_14 = __pyx_r;
+          __pyx_r = 0;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
+          __pyx_r = __pyx_t_14;
+          __pyx_t_14 = 0;
+          goto __pyx_L6_except_return;
+        }
+      }
+    }
+    goto __pyx_L5_except_error;
+
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L7_try_return:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L0;
+    __pyx_L6_except_return:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L0;
+  }
 
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_11);
   __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_embeddings);
   __Pyx_XDECREF(__pyx_v_chunk);
   __Pyx_XDECREF(__pyx_v_response);
   __Pyx_XDECREF(__pyx_v_embedding);
+  __Pyx_XDECREF(__pyx_v_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
@@ -4560,60 +4810,60 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_collection)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_database)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 1); __PYX_ERR(0, 60, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 1); __PYX_ERR(0, 65, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_datasource)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 2); __PYX_ERR(0, 60, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 2); __PYX_ERR(0, 65, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_enkyc)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 3); __PYX_ERR(0, 60, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 3); __PYX_ERR(0, 65, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_params_dict)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 4); __PYX_ERR(0, 60, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 4); __PYX_ERR(0, 65, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "SaveToMongoDb") < 0)) __PYX_ERR(0, 60, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "SaveToMongoDb") < 0)) __PYX_ERR(0, 65, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 5)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -4624,32 +4874,32 @@
     __pyx_v_database = ((PyObject*)values[1]);
     __pyx_v_datasource = ((PyObject*)values[2]);
     __pyx_v_enkyc = ((PyObject*)values[3]);
     __pyx_v_params_dict = values[4];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 60, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 65, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.SaveToMongoDb", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_collection), (&PyUnicode_Type), 1, "collection", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_database), (&PyUnicode_Type), 1, "database", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_datasource), (&PyUnicode_Type), 1, "datasource", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_enkyc), (&PyUnicode_Type), 1, "enkyc", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_collection), (&PyUnicode_Type), 1, "collection", 1))) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_database), (&PyUnicode_Type), 1, "database", 1))) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_datasource), (&PyUnicode_Type), 1, "datasource", 1))) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_enkyc), (&PyUnicode_Type), 1, "enkyc", 1))) __PYX_ERR(0, 65, __pyx_L1_error)
   __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_collection, __pyx_v_database, __pyx_v_datasource, __pyx_v_enkyc, __pyx_v_params_dict);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4678,15 +4928,15 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("SaveToMongoDb", 1);
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -4698,138 +4948,138 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_decrypted_url = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_collection, __pyx_v_collection) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_collection, __pyx_v_collection) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
 
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_database, __pyx_v_database) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_database, __pyx_v_database) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
 
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_dataSource, __pyx_v_datasource) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_dataSource, __pyx_v_datasource) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
 
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_filename, __pyx_t_5) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_filename, __pyx_t_5) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filter, __pyx_t_2) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filter, __pyx_t_2) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_filename, __pyx_t_6) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_filename, __pyx_t_6) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_data, __pyx_t_3) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_data, __pyx_t_3) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_type, __pyx_kp_u_application_pdf) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_type, __pyx_kp_u_application_pdf) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_extracted_text, __pyx_t_6) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_extracted_text, __pyx_t_6) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_text_embeddings, __pyx_t_3) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_text_embeddings, __pyx_t_3) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_set, __pyx_t_5) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_set, __pyx_t_5) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_update, __pyx_t_2) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_update, __pyx_t_2) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_upsert, Py_True) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_upsert, Py_True) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   __pyx_v_payload = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__6) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__6) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
 
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_v_enkyc) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_v_enkyc) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
   __pyx_v_headers = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_requests); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_requests); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_decrypted_url);
   __Pyx_GIVEREF(__pyx_v_decrypted_url);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_decrypted_url)) __PYX_ERR(0, 85, __pyx_L1_error);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_decrypted_url)) __PYX_ERR(0, 90, __pyx_L1_error);
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_json, __pyx_v_payload) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_json, __pyx_v_payload) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_response = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_3, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_3, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_7) {
 
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_kp_u_Successfully_save_to_the_databas);
     __pyx_r = __pyx_kp_u_Successfully_save_to_the_databas;
     goto __pyx_L0;
 
   }
 
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_error, __pyx_t_5) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_error, __pyx_t_5) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
 
@@ -5620,22 +5870,25 @@
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
     {&__pyx_n_s_AES, __pyx_k_AES, sizeof(__pyx_k_AES), 0, 0, 1, 1},
     {&__pyx_kp_u_Access_Control_Request_Headers, __pyx_k_Access_Control_Request_Headers, sizeof(__pyx_k_Access_Control_Request_Headers), 0, 1, 0, 0},
+    {&__pyx_kp_u_An_unexpected_error_occurred, __pyx_k_An_unexpected_error_occurred, sizeof(__pyx_k_An_unexpected_error_occurred), 0, 1, 0, 0},
+    {&__pyx_n_s_AuthenticationError, __pyx_k_AuthenticationError, sizeof(__pyx_k_AuthenticationError), 0, 0, 1, 1},
     {&__pyx_n_s_CBC, __pyx_k_CBC, sizeof(__pyx_k_CBC), 0, 0, 1, 1},
     {&__pyx_n_s_Cipher, __pyx_k_Cipher, sizeof(__pyx_k_Cipher), 0, 0, 1, 1},
     {&__pyx_kp_u_Content_Type, __pyx_k_Content_Type, sizeof(__pyx_k_Content_Type), 0, 1, 0, 0},
     {&__pyx_n_s_Decenigma, __pyx_k_Decenigma, sizeof(__pyx_k_Decenigma), 0, 0, 1, 1},
     {&__pyx_n_s_Decipherx, __pyx_k_Decipherx, sizeof(__pyx_k_Decipherx), 0, 0, 1, 1},
     {&__pyx_n_s_Embedshroud, __pyx_k_Embedshroud, sizeof(__pyx_k_Embedshroud), 0, 0, 1, 1},
     {&__pyx_n_s_Encapseal, __pyx_k_Encapseal, sizeof(__pyx_k_Encapseal), 0, 0, 1, 1},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+    {&__pyx_kp_u_Invalid_API_key_provided, __pyx_k_Invalid_API_key_provided, sizeof(__pyx_k_Invalid_API_key_provided), 0, 1, 0, 0},
     {&__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, sizeof(__pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN), 0, 0, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_SaveToMongoDb, __pyx_k_SaveToMongoDb, sizeof(__pyx_k_SaveToMongoDb), 0, 0, 1, 1},
     {&__pyx_kp_u_Successfully_save_to_the_databas, __pyx_k_Successfully_save_to_the_databas, sizeof(__pyx_k_Successfully_save_to_the_databas), 0, 1, 0, 0},
     {&__pyx_n_s__25, __pyx_k__25, sizeof(__pyx_k__25), 0, 0, 1, 1},
     {&__pyx_n_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
@@ -5675,14 +5928,15 @@
     {&__pyx_n_s_decrypted_padded_text, __pyx_k_decrypted_padded_text, sizeof(__pyx_k_decrypted_padded_text), 0, 0, 1, 1},
     {&__pyx_n_s_decrypted_url, __pyx_k_decrypted_url, sizeof(__pyx_k_decrypted_url), 0, 0, 1, 1},
     {&__pyx_n_s_decryptor, __pyx_k_decryptor, sizeof(__pyx_k_decryptor), 0, 0, 1, 1},
     {&__pyx_n_s_default_backend, __pyx_k_default_backend, sizeof(__pyx_k_default_backend), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_n_s_dict_2, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
     {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
+    {&__pyx_n_s_e, __pyx_k_e, sizeof(__pyx_k_e), 0, 0, 1, 1},
     {&__pyx_n_s_embedding, __pyx_k_embedding, sizeof(__pyx_k_embedding), 0, 0, 1, 1},
     {&__pyx_n_s_embeddings, __pyx_k_embeddings, sizeof(__pyx_k_embeddings), 0, 0, 1, 1},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_encoded_url, __pyx_k_encoded_url, sizeof(__pyx_k_encoded_url), 0, 0, 1, 1},
     {&__pyx_n_s_encryptedText, __pyx_k_encryptedText, sizeof(__pyx_k_encryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_encryptor, __pyx_k_encryptor, sizeof(__pyx_k_encryptor), 0, 0, 1, 1},
@@ -5774,27 +6028,27 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_u_filename, __pyx_kp_u_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_u_filename, __pyx_kp_u_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_file_data, __pyx_kp_u_); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_file_data, __pyx_kp_u_); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_extracted_text, __pyx_kp_u_); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_extracted_text, __pyx_kp_u_); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_text_embeddings, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_text_embeddings, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   __pyx_tuple__7 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
@@ -5809,23 +6063,23 @@
   __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   __pyx_tuple__13 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
   __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 31, __pyx_L1_error)
 
-  __pyx_tuple__15 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Embedshroud, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Embedshroud, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 48, __pyx_L1_error)
 
-  __pyx_tuple__17 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SaveToMongoDb, 60, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SaveToMongoDb, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 65, __pyx_L1_error)
 
   __pyx_tuple__19 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
   __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 16, __pyx_L1_error)
@@ -6311,17 +6565,17 @@
 
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Embedshroud, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Embedshroud, __pyx_t_2) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9SaveToMongoDb, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SaveToMongoDb, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9SaveToMongoDb, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SaveToMongoDb, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_SaveToMongoDb, __pyx_t_2) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_SaveToMongoDb, __pyx_t_2) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -7561,14 +7815,361 @@
     if (likely(tp->tp_setattr))
         return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
 #endif
     return PyObject_SetAttr(obj, attr_name, value);
 }
 #endif
 
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #endif
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+  #endif
+}
+#endif
+
+/* FastTypeChecks */
+#if CYTHON_COMPILING_IN_CPYTHON
+static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
+    while (a) {
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
+        if (a == b)
+            return 1;
+    }
+    return b == &PyBaseObject_Type;
+}
+static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (a == b) return 1;
+    mro = a->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(a, b);
+}
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
+#if PY_MAJOR_VERSION == 2
+static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
+    PyObject *exception, *value, *tb;
+    int res;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&exception, &value, &tb);
+    res = exc_type1 ? PyObject_IsSubclass(err, exc_type1) : 0;
+    if (unlikely(res == -1)) {
+        PyErr_WriteUnraisable(err);
+        res = 0;
+    }
+    if (!res) {
+        res = PyObject_IsSubclass(err, exc_type2);
+        if (unlikely(res == -1)) {
+            PyErr_WriteUnraisable(err);
+            res = 0;
+        }
+    }
+    __Pyx_ErrRestore(exception, value, tb);
+    return res;
+}
+#else
+static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    }
+}
+#endif
+static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    assert(PyExceptionClass_Check(exc_type));
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        PyObject *t = PyTuple_GET_ITEM(tuple, i);
+        #if PY_MAJOR_VERSION < 3
+        if (likely(exc_type == t)) return 1;
+        #endif
+        if (likely(PyExceptionClass_Check(t))) {
+            if (__Pyx_inner_PyErr_GivenExceptionMatches2(exc_type, NULL, t)) return 1;
+        } else {
+        }
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject* exc_type) {
+    if (likely(err == exc_type)) return 1;
+    if (likely(PyExceptionClass_Check(err))) {
+        if (likely(PyExceptionClass_Check(exc_type))) {
+            return __Pyx_inner_PyErr_GivenExceptionMatches2(err, NULL, exc_type);
+        } else if (likely(PyTuple_Check(exc_type))) {
+            return __Pyx_PyErr_GivenExceptionMatchesTuple(err, exc_type);
+        } else {
+        }
+    }
+    return PyErr_GivenExceptionMatches(err, exc_type);
+}
+static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *exc_type1, PyObject *exc_type2) {
+    assert(PyExceptionClass_Check(exc_type1));
+    assert(PyExceptionClass_Check(exc_type2));
+    if (likely(err == exc_type1 || err == exc_type2)) return 1;
+    if (likely(PyExceptionClass_Check(err))) {
+        return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
+    }
+    return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* SwapException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_value = exc_info->exc_value;
+    exc_info->exc_value = *value;
+    if (tmp_value == NULL || tmp_value == Py_None) {
+        Py_XDECREF(tmp_value);
+        tmp_value = NULL;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+    } else {
+        tmp_type = (PyObject*) Py_TYPE(tmp_value);
+        Py_INCREF(tmp_type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        tmp_tb = ((PyBaseExceptionObject*) tmp_value)->traceback;
+        Py_XINCREF(tmp_tb);
+        #else
+        tmp_tb = PyException_GetTraceback(tmp_value);
+        #endif
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = *type;
+    exc_info->exc_value = *value;
+    exc_info->exc_traceback = *tb;
+  #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = *type;
+    tstate->exc_value = *value;
+    tstate->exc_traceback = *tb;
+  #endif
+    *type = tmp_type;
+    *value = tmp_value;
+    *tb = tmp_tb;
+}
+#else
+static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    PyErr_GetExcInfo(&tmp_type, &tmp_value, &tmp_tb);
+    PyErr_SetExcInfo(*type, *value, *tb);
+    *type = tmp_type;
+    *value = tmp_value;
+    *tb = tmp_tb;
+}
+#endif
+
 /* PyIntCompare */
 static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace) {
     CYTHON_MAYBE_UNUSED_VAR(intval);
     CYTHON_UNUSED_VAR(inplace);
     if (op1 == op2) {
         return 1;
     }
@@ -10841,130 +11442,14 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
-/* FastTypeChecks */
-#if CYTHON_COMPILING_IN_CPYTHON
-static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
-    while (a) {
-        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
-        if (a == b)
-            return 1;
-    }
-    return b == &PyBaseObject_Type;
-}
-static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
-    PyObject *mro;
-    if (a == b) return 1;
-    mro = a->tp_mro;
-    if (likely(mro)) {
-        Py_ssize_t i, n;
-        n = PyTuple_GET_SIZE(mro);
-        for (i = 0; i < n; i++) {
-            if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
-                return 1;
-        }
-        return 0;
-    }
-    return __Pyx_InBases(a, b);
-}
-static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
-    PyObject *mro;
-    if (cls == a || cls == b) return 1;
-    mro = cls->tp_mro;
-    if (likely(mro)) {
-        Py_ssize_t i, n;
-        n = PyTuple_GET_SIZE(mro);
-        for (i = 0; i < n; i++) {
-            PyObject *base = PyTuple_GET_ITEM(mro, i);
-            if (base == (PyObject *)a || base == (PyObject *)b)
-                return 1;
-        }
-        return 0;
-    }
-    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
-}
-#if PY_MAJOR_VERSION == 2
-static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
-    PyObject *exception, *value, *tb;
-    int res;
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&exception, &value, &tb);
-    res = exc_type1 ? PyObject_IsSubclass(err, exc_type1) : 0;
-    if (unlikely(res == -1)) {
-        PyErr_WriteUnraisable(err);
-        res = 0;
-    }
-    if (!res) {
-        res = PyObject_IsSubclass(err, exc_type2);
-        if (unlikely(res == -1)) {
-            PyErr_WriteUnraisable(err);
-            res = 0;
-        }
-    }
-    __Pyx_ErrRestore(exception, value, tb);
-    return res;
-}
-#else
-static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    if (exc_type1) {
-        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
-    } else {
-        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
-    }
-}
-#endif
-static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    assert(PyExceptionClass_Check(exc_type));
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        PyObject *t = PyTuple_GET_ITEM(tuple, i);
-        #if PY_MAJOR_VERSION < 3
-        if (likely(exc_type == t)) return 1;
-        #endif
-        if (likely(PyExceptionClass_Check(t))) {
-            if (__Pyx_inner_PyErr_GivenExceptionMatches2(exc_type, NULL, t)) return 1;
-        } else {
-        }
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject* exc_type) {
-    if (likely(err == exc_type)) return 1;
-    if (likely(PyExceptionClass_Check(err))) {
-        if (likely(PyExceptionClass_Check(exc_type))) {
-            return __Pyx_inner_PyErr_GivenExceptionMatches2(err, NULL, exc_type);
-        } else if (likely(PyTuple_Check(exc_type))) {
-            return __Pyx_PyErr_GivenExceptionMatchesTuple(err, exc_type);
-        } else {
-        }
-    }
-    return PyErr_GivenExceptionMatches(err, exc_type);
-}
-static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *exc_type1, PyObject *exc_type2) {
-    assert(PyExceptionClass_Check(exc_type1));
-    assert(PyExceptionClass_Check(exc_type2));
-    if (likely(err == exc_type1 || err == exc_type2)) return 1;
-    if (likely(PyExceptionClass_Check(err))) {
-        return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
-    }
-    return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
-}
-#endif
-
 /* CheckBinaryVersion */
 static unsigned long __Pyx_get_runtime_version(void) {
 #if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
     return Py_Version & ~0xFFUL;
 #else
     const char* rt_version = Py_GetVersion();
     unsigned long version = 0;
```

### Comparing `aixhello-3.0/aixhello.egg-info/PKG-INFO` & `aixhello-3.1/aixhello.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.0
+Version: 3.1
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.0/setup.py` & `aixhello-3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='3.0',  # Increment the version number
+    version='3.1',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

