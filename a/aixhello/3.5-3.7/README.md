# Comparing `tmp/aixhello-3.5.tar.gz` & `tmp/aixhello-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-3.5.tar", last modified: Sun Jun  2 04:34:05 2024, max compression
+gzip compressed data, was "aixhello-3.7.tar", last modified: Sun Jun  2 04:40:52 2024, max compression
```

## Comparing `aixhello-3.5.tar` & `aixhello-3.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 04:34:05.924670 aixhello-3.5/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.5/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-02 04:34:05.924670 aixhello-3.5/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 04:34:05.900723 aixhello-3.5/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.5/aixhello/__init__.py
--rw-rw-rw-   0        0        0   585831 2024-06-02 04:33:58.000000 aixhello-3.5/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-02 04:34:05.923186 aixhello-3.5/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-02 04:34:05.000000 aixhello-3.5/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-02 04:34:05.000000 aixhello-3.5/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 04:34:05.000000 aixhello-3.5/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-02 04:34:05.000000 aixhello-3.5/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 04:34:05.000000 aixhello-3.5/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-02 04:34:05.931881 aixhello-3.5/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-02 04:32:29.000000 aixhello-3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:40:52.759701 aixhello-3.7/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.7/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-02 04:40:52.758701 aixhello-3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 04:40:52.737383 aixhello-3.7/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.7/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   588778 2024-06-02 04:40:43.000000 aixhello-3.7/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-02 04:40:52.757701 aixhello-3.7/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-02 04:40:52.000000 aixhello-3.7/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-02 04:40:52.000000 aixhello-3.7/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 04:40:52.000000 aixhello-3.7/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-02 04:40:52.000000 aixhello-3.7/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 04:40:52.000000 aixhello-3.7/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-02 04:40:52.764726 aixhello-3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-02 04:40:33.000000 aixhello-3.7/setup.py
```

### Comparing `aixhello-3.5/LICENSE` & `aixhello-3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-3.5/PKG-INFO` & `aixhello-3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.5
+Version: 3.7
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.5/README.md` & `aixhello-3.7/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-3.5/aixhello/xyello.c` & `aixhello-3.7/aixhello/xyello.c`

 * *Files 0% similar despite different names*

```diff
@@ -2259,35 +2259,38 @@
 
 /* GCCDiagnostics.proto */
 #if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* CIntFromPy.proto */
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
+
+/* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
 static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
 #define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
 #else
 typedef const char *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%.200s"
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
-
 /* CheckBinaryVersion.proto */
 static unsigned long __Pyx_get_runtime_version(void);
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
@@ -2508,15 +2511,15 @@
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbed(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8vectorizeText(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_embed, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, PyObject *__pyx_v_vector_query, PyObject *__pyx_v_top_n); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, int __pyx_v_vector_query, int __pyx_v_top_n); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
@@ -5931,16 +5934,16 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_connParam = 0;
   PyObject *__pyx_v_extracted_text_length = 0;
-  PyObject *__pyx_v_vector_query = 0;
-  PyObject *__pyx_v_top_n = 0;
+  int __pyx_v_vector_query;
+  int __pyx_v_top_n;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[4] = {0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -6022,16 +6025,16 @@
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
     __pyx_v_connParam = values[0];
     __pyx_v_extracted_text_length = ((PyObject*)values[1]);
-    __pyx_v_vector_query = ((PyObject*)values[2]);
-    __pyx_v_top_n = ((PyObject*)values[3]);
+    __pyx_v_vector_query = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_vector_query == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
+    __pyx_v_top_n = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_top_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("vector_search", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 113, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
@@ -6042,16 +6045,14 @@
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_extracted_text_length), (&PyUnicode_Type), 1, "extracted_text_length", 1))) __PYX_ERR(0, 113, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vector_query), (&PyUnicode_Type), 1, "vector_query", 1))) __PYX_ERR(0, 113, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_top_n), (&PyUnicode_Type), 1, "top_n", 1))) __PYX_ERR(0, 113, __pyx_L1_error)
   __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_connParam, __pyx_v_extracted_text_length, __pyx_v_vector_query, __pyx_v_top_n);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6185,15 +6186,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, PyObject *__pyx_v_vector_query, PyObject *__pyx_v_top_n) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, int __pyx_v_vector_query, int __pyx_v_top_n) {
   PyObject *__pyx_v_url = NULL;
   PyObject *__pyx_v_headers = NULL;
   PyObject *__pyx_v_pipeline = NULL;
   PyObject *__pyx_v_query_payload = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_similarities = NULL;
   PyObject *__pyx_v_response_data = NULL;
@@ -6280,15 +6281,18 @@
   __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_searchindex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_index, __pyx_t_3) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_query, __pyx_v_vector_query) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_vector_query); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_query, __pyx_t_5) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_wildcard, __pyx_kp_u__6) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_path, __pyx_t_5) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_text, __pyx_t_3) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
@@ -6311,15 +6315,18 @@
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_score, __pyx_t_5) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_project, __pyx_t_3) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_limit, __pyx_v_top_n) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_top_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_limit, __pyx_t_5) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error);
@@ -6418,32 +6425,35 @@
     __pyx_t_1 = 0;
 
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = NULL;
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_vector_query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_2)) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
         __pyx_t_4 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_vector_query};
+      PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_2};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_v_query_vec = __pyx_t_1;
     __pyx_t_1 = 0;
 
@@ -6771,15 +6781,15 @@
     __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_similarities, __pyx_t_11);
     __pyx_t_11 = 0;
 
-    __pyx_t_11 = __Pyx_PyObject_GetSlice(__pyx_v_similarities, 0, 0, NULL, &__pyx_v_top_n, NULL, 0, 0, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetSlice(__pyx_v_similarities, 0, __pyx_v_top_n, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __pyx_v_top_results = __pyx_t_11;
     __pyx_t_11 = 0;
 
     { /* enter inner scope */
       __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 186, __pyx_L13_error)
       __Pyx_GOTREF(__pyx_t_11);
@@ -12974,173 +12984,173 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntFromPy */
-static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
+    const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if ((sizeof(long) < sizeof(long))) {
-            __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
+        if ((sizeof(int) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (long) val;
+            return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (unlikely(__Pyx_PyLong_IsNeg(x))) {
                 goto raise_neg_overflow;
             } else if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_DigitCount(x)) {
                     case 2:
-                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
-                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
-                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
-                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                             }
                         }
                         break;
                 }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (long) -1;
+                    return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if ((sizeof(long) <= sizeof(unsigned long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
+            if ((sizeof(int) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_SignedDigitCount(x)) {
                     case -2:
-                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case 2:
-                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case -3:
-                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case -4:
-                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                 }
             }
 #endif
-            if ((sizeof(long) <= sizeof(long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
+            if ((sizeof(int) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-            long val;
+            int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
 #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -13159,341 +13169,261 @@
                 long idigit;
                 int chunk_size = (sizeof(long) < 8) ? 30 : 62;
                 if (unlikely(!PyLong_CheckExact(v))) {
                     PyObject *tmp = v;
                     v = PyNumber_Long(v);
                     assert(PyLong_CheckExact(v));
                     Py_DECREF(tmp);
-                    if (unlikely(!v)) return (long) -1;
+                    if (unlikely(!v)) return (int) -1;
                 }
 #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                 if (Py_SIZE(x) == 0)
-                    return (long) 0;
+                    return (int) 0;
                 is_negative = Py_SIZE(x) < 0;
 #else
                 {
                     int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                     if (unlikely(result < 0))
-                        return (long) -1;
+                        return (int) -1;
                     is_negative = result == 1;
                 }
 #endif
                 if (is_unsigned && unlikely(is_negative)) {
                     goto raise_neg_overflow;
                 } else if (is_negative) {
                     stepval = PyNumber_Invert(v);
                     if (unlikely(!stepval))
-                        return (long) -1;
+                        return (int) -1;
                 } else {
                     stepval = __Pyx_NewRef(v);
                 }
-                val = (long) 0;
+                val = (int) 0;
                 mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
                 shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
-                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
                     PyObject *tmp, *digit;
                     digit = PyNumber_And(stepval, mask);
                     if (unlikely(!digit)) goto done;
                     idigit = PyLong_AsLong(digit);
                     Py_DECREF(digit);
                     if (unlikely(idigit < 0)) goto done;
                     tmp = PyNumber_Rshift(stepval, shift);
                     if (unlikely(!tmp)) goto done;
                     Py_DECREF(stepval); stepval = tmp;
-                    val |= ((long) idigit) << bits;
+                    val |= ((int) idigit) << bits;
                     #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                     if (Py_SIZE(stepval) == 0)
                         goto unpacking_done;
                     #endif
                 }
                 idigit = PyLong_AsLong(stepval);
                 if (unlikely(idigit < 0)) goto done;
-                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
                 if (unlikely(idigit >= (1L << remaining_bits)))
                     goto raise_overflow;
-                val |= ((long) idigit) << bits;
+                val |= ((int) idigit) << bits;
             #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
             unpacking_done:
             #endif
                 if (!is_unsigned) {
-                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
                         goto raise_overflow;
                     if (is_negative)
                         val = ~val;
                 }
                 ret = 0;
             done:
                 Py_XDECREF(shift);
                 Py_XDECREF(mask);
                 Py_XDECREF(stepval);
 #endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-            return (long) -1;
+            return (int) -1;
         }
     } else {
-        long val;
+        int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (long) -1;
-        val = __Pyx_PyInt_As_long(tmp);
+        if (!tmp) return (int) -1;
+        val = __Pyx_PyInt_As_int(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to long");
-    return (long) -1;
+        "value too large to convert to int");
+    return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to long");
-    return (long) -1;
-}
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-#else
-        PyObject *from_bytes, *result = NULL;
-        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
-        if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
-        if (!py_bytes) goto limited_bad;
-        order_str = PyUnicode_FromString(little ? "little" : "big");
-        if (!order_str) goto limited_bad;
-        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
-        if (!arg_tuple) goto limited_bad;
-        if (!is_unsigned) {
-            kwds = PyDict_New();
-            if (!kwds) goto limited_bad;
-            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
-        }
-        result = PyObject_Call(from_bytes, arg_tuple, kwds);
-        limited_bad:
-        Py_XDECREF(kwds);
-        Py_XDECREF(arg_tuple);
-        Py_XDECREF(order_str);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(from_bytes);
-        return result;
-#endif
-    }
-}
-
-/* FormatTypeName */
-#if CYTHON_COMPILING_IN_LIMITED_API
-static __Pyx_TypeName
-__Pyx_PyType_GetName(PyTypeObject* tp)
-{
-    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
-                                               __pyx_n_s_name);
-    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
-        PyErr_Clear();
-        Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__30);
-    }
-    return name;
+        "can't convert negative value to int");
+    return (int) -1;
 }
-#endif
 
 /* CIntFromPy */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
+    const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if ((sizeof(int) < sizeof(long))) {
-            __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
+        if ((sizeof(long) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (int) val;
+            return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (unlikely(__Pyx_PyLong_IsNeg(x))) {
                 goto raise_neg_overflow;
             } else if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_DigitCount(x)) {
                     case 2:
-                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
-                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
-                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
-                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                             }
                         }
                         break;
                 }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (int) -1;
+                    return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if ((sizeof(int) <= sizeof(unsigned long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
+            if ((sizeof(long) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_SignedDigitCount(x)) {
                     case -2:
-                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case 2:
-                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case -3:
-                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case -4:
-                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                 }
             }
 #endif
-            if ((sizeof(int) <= sizeof(long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
+            if ((sizeof(long) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-            int val;
+            long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
 #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -13512,101 +13442,245 @@
                 long idigit;
                 int chunk_size = (sizeof(long) < 8) ? 30 : 62;
                 if (unlikely(!PyLong_CheckExact(v))) {
                     PyObject *tmp = v;
                     v = PyNumber_Long(v);
                     assert(PyLong_CheckExact(v));
                     Py_DECREF(tmp);
-                    if (unlikely(!v)) return (int) -1;
+                    if (unlikely(!v)) return (long) -1;
                 }
 #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                 if (Py_SIZE(x) == 0)
-                    return (int) 0;
+                    return (long) 0;
                 is_negative = Py_SIZE(x) < 0;
 #else
                 {
                     int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                     if (unlikely(result < 0))
-                        return (int) -1;
+                        return (long) -1;
                     is_negative = result == 1;
                 }
 #endif
                 if (is_unsigned && unlikely(is_negative)) {
                     goto raise_neg_overflow;
                 } else if (is_negative) {
                     stepval = PyNumber_Invert(v);
                     if (unlikely(!stepval))
-                        return (int) -1;
+                        return (long) -1;
                 } else {
                     stepval = __Pyx_NewRef(v);
                 }
-                val = (int) 0;
+                val = (long) 0;
                 mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
                 shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
-                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
                     PyObject *tmp, *digit;
                     digit = PyNumber_And(stepval, mask);
                     if (unlikely(!digit)) goto done;
                     idigit = PyLong_AsLong(digit);
                     Py_DECREF(digit);
                     if (unlikely(idigit < 0)) goto done;
                     tmp = PyNumber_Rshift(stepval, shift);
                     if (unlikely(!tmp)) goto done;
                     Py_DECREF(stepval); stepval = tmp;
-                    val |= ((int) idigit) << bits;
+                    val |= ((long) idigit) << bits;
                     #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                     if (Py_SIZE(stepval) == 0)
                         goto unpacking_done;
                     #endif
                 }
                 idigit = PyLong_AsLong(stepval);
                 if (unlikely(idigit < 0)) goto done;
-                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
                 if (unlikely(idigit >= (1L << remaining_bits)))
                     goto raise_overflow;
-                val |= ((int) idigit) << bits;
+                val |= ((long) idigit) << bits;
             #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
             unpacking_done:
             #endif
                 if (!is_unsigned) {
-                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
                         goto raise_overflow;
                     if (is_negative)
                         val = ~val;
                 }
                 ret = 0;
             done:
                 Py_XDECREF(shift);
                 Py_XDECREF(mask);
                 Py_XDECREF(stepval);
 #endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-            return (int) -1;
+            return (long) -1;
         }
     } else {
-        int val;
+        long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (int) -1;
-        val = __Pyx_PyInt_As_int(tmp);
+        if (!tmp) return (long) -1;
+        val = __Pyx_PyInt_As_long(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to int");
-    return (int) -1;
+        "value too large to convert to long");
+    return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to int");
-    return (int) -1;
+        "can't convert negative value to long");
+    return (long) -1;
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
+/* FormatTypeName */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XDECREF(name);
+        name = __Pyx_NewRef(__pyx_n_s__30);
+    }
+    return name;
+}
+#endif
+
 /* CheckBinaryVersion */
 static unsigned long __Pyx_get_runtime_version(void) {
 #if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
     return Py_Version & ~0xFFUL;
 #else
     const char* rt_version = Py_GetVersion();
     unsigned long version = 0;
```

### Comparing `aixhello-3.5/aixhello.egg-info/PKG-INFO` & `aixhello-3.7/aixhello.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.5
+Version: 3.7
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.5/setup.py` & `aixhello-3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='3.5',  # Increment the version number
+    version='3.7',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

