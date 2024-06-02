# Comparing `tmp/aixhello-3.7.tar.gz` & `tmp/aixhello-3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-3.7.tar", last modified: Sun Jun  2 04:40:52 2024, max compression
+gzip compressed data, was "aixhello-3.8.tar", last modified: Sun Jun  2 04:43:44 2024, max compression
```

## Comparing `aixhello-3.7.tar` & `aixhello-3.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 04:40:52.759701 aixhello-3.7/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.7/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-02 04:40:52.758701 aixhello-3.7/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.7/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 04:40:52.737383 aixhello-3.7/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.7/aixhello/__init__.py
--rw-rw-rw-   0        0        0   588778 2024-06-02 04:40:43.000000 aixhello-3.7/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-02 04:40:52.757701 aixhello-3.7/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-02 04:40:52.000000 aixhello-3.7/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-02 04:40:52.000000 aixhello-3.7/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 04:40:52.000000 aixhello-3.7/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-02 04:40:52.000000 aixhello-3.7/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 04:40:52.000000 aixhello-3.7/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-02 04:40:52.764726 aixhello-3.7/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-02 04:40:33.000000 aixhello-3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:43:44.241149 aixhello-3.8/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.8/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-02 04:43:44.241149 aixhello-3.8/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 04:43:44.220991 aixhello-3.8/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.8/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   588475 2024-06-02 04:43:35.000000 aixhello-3.8/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-02 04:43:44.239147 aixhello-3.8/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-02 04:43:44.000000 aixhello-3.8/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-02 04:43:44.000000 aixhello-3.8/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 04:43:44.000000 aixhello-3.8/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-02 04:43:44.000000 aixhello-3.8/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 04:43:44.000000 aixhello-3.8/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-02 04:43:44.243147 aixhello-3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-02 04:43:28.000000 aixhello-3.8/setup.py
```

### Comparing `aixhello-3.7/LICENSE` & `aixhello-3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-3.7/PKG-INFO` & `aixhello-3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.7
+Version: 3.8
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.7/README.md` & `aixhello-3.8/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-3.7/aixhello/xyello.c` & `aixhello-3.8/aixhello/xyello.c`

 * *Files 0% similar despite different names*

```diff
@@ -2459,14 +2459,15 @@
 static const char __pyx_k_query_payload[] = "query_payload";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_response_data[] = "response_data";
 static const char __pyx_k_similar_score[] = "similar_score";
 static const char __pyx_k_vector_search[] = "vector_search";
 static const char __pyx_k_vectorizeText[] = "vectorizeText";
 static const char __pyx_k_extracted_text[] = "extracted_text";
+static const char __pyx_k_result_lentgth[] = "result_lentgth";
 static const char __pyx_k_vectorizeEmbed[] = "vectorizeEmbed";
 static const char __pyx_k_aixhello_xyello[] = "aixhello.xyello";
 static const char __pyx_k_application_pdf[] = "application/pdf";
 static const char __pyx_k_default_backend[] = "default_backend";
 static const char __pyx_k_extracted_texts[] = "extracted_texts";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
@@ -2484,15 +2485,14 @@
 static const char __pyx_k_pyx_unpickle_xyellw[] = "__pyx_unpickle_xyellw";
 static const char __pyx_k_similarities_values[] = "similarities_values";
 static const char __pyx_k_xyellw_SaveToMongoDb[] = "xyellw.SaveToMongoDb";
 static const char __pyx_k_xyellw_vector_search[] = "xyellw.vector_search";
 static const char __pyx_k_xyellw_vectorizeText[] = "xyellw.vectorizeText";
 static const char __pyx_k_decoded_encryptedText[] = "decoded_encryptedText";
 static const char __pyx_k_decrypted_padded_text[] = "decrypted_padded_text";
-static const char __pyx_k_extracted_text_length[] = "extracted_text_length";
 static const char __pyx_k_xyellw_vectorizeEmbed[] = "xyellw.vectorizeEmbed";
 static const char __pyx_k_text_embedding_ada_002[] = "text-embedding-ada-002";
 static const char __pyx_k_xyellw___reduce_cython[] = "xyellw.__reduce_cython__";
 static const char __pyx_k_Invalid_API_key_provided[] = "Invalid API key provided";
 static const char __pyx_k_xyellw___setstate_cython[] = "xyellw.__setstate_cython__";
 static const char __pyx_k_vector_search_locals_lambda[] = "vector_search.<locals>.<lambda>";
 static const char __pyx_k_An_unexpected_error_occurred[] = "An unexpected error occurred";
@@ -2511,15 +2511,15 @@
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbed(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8vectorizeText(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_embed, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, int __pyx_v_vector_query, int __pyx_v_top_n); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, int __pyx_v_result_lentgth, PyObject *__pyx_v_vector_query, int __pyx_v_top_n); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
@@ -2632,15 +2632,14 @@
   PyObject *__pyx_n_s_encoded_url;
   PyObject *__pyx_n_s_encryptedText;
   PyObject *__pyx_n_s_encryptor;
   PyObject *__pyx_n_s_enkyc;
   PyObject *__pyx_n_u_enkyc;
   PyObject *__pyx_n_u_error;
   PyObject *__pyx_n_u_extracted_text;
-  PyObject *__pyx_n_s_extracted_text_length;
   PyObject *__pyx_n_s_extracted_texts;
   PyObject *__pyx_n_u_file_data;
   PyObject *__pyx_n_u_file_type;
   PyObject *__pyx_n_u_filename;
   PyObject *__pyx_n_s_filenames;
   PyObject *__pyx_n_u_filter;
   PyObject *__pyx_n_s_finalize;
@@ -2697,14 +2696,15 @@
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_requests;
   PyObject *__pyx_n_s_response;
   PyObject *__pyx_n_s_response_data;
   PyObject *__pyx_n_s_result;
+  PyObject *__pyx_n_s_result_lentgth;
   PyObject *__pyx_n_s_reverse;
   PyObject *__pyx_n_u_score;
   PyObject *__pyx_kp_u_search;
   PyObject *__pyx_n_u_searchScore;
   PyObject *__pyx_n_u_searchindex;
   PyObject *__pyx_n_s_self;
   PyObject *__pyx_kp_u_set;
@@ -2912,15 +2912,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_encoded_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptor);
   Py_CLEAR(clear_module_state->__pyx_n_s_enkyc);
   Py_CLEAR(clear_module_state->__pyx_n_u_enkyc);
   Py_CLEAR(clear_module_state->__pyx_n_u_error);
   Py_CLEAR(clear_module_state->__pyx_n_u_extracted_text);
-  Py_CLEAR(clear_module_state->__pyx_n_s_extracted_text_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_extracted_texts);
   Py_CLEAR(clear_module_state->__pyx_n_u_file_data);
   Py_CLEAR(clear_module_state->__pyx_n_u_file_type);
   Py_CLEAR(clear_module_state->__pyx_n_u_filename);
   Py_CLEAR(clear_module_state->__pyx_n_s_filenames);
   Py_CLEAR(clear_module_state->__pyx_n_u_filter);
   Py_CLEAR(clear_module_state->__pyx_n_s_finalize);
@@ -2977,14 +2976,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_requests);
   Py_CLEAR(clear_module_state->__pyx_n_s_response);
   Py_CLEAR(clear_module_state->__pyx_n_s_response_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_result);
+  Py_CLEAR(clear_module_state->__pyx_n_s_result_lentgth);
   Py_CLEAR(clear_module_state->__pyx_n_s_reverse);
   Py_CLEAR(clear_module_state->__pyx_n_u_score);
   Py_CLEAR(clear_module_state->__pyx_kp_u_search);
   Py_CLEAR(clear_module_state->__pyx_n_u_searchScore);
   Py_CLEAR(clear_module_state->__pyx_n_u_searchindex);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_kp_u_set);
@@ -3170,15 +3170,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_encoded_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptor);
   Py_VISIT(traverse_module_state->__pyx_n_s_enkyc);
   Py_VISIT(traverse_module_state->__pyx_n_u_enkyc);
   Py_VISIT(traverse_module_state->__pyx_n_u_error);
   Py_VISIT(traverse_module_state->__pyx_n_u_extracted_text);
-  Py_VISIT(traverse_module_state->__pyx_n_s_extracted_text_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_extracted_texts);
   Py_VISIT(traverse_module_state->__pyx_n_u_file_data);
   Py_VISIT(traverse_module_state->__pyx_n_u_file_type);
   Py_VISIT(traverse_module_state->__pyx_n_u_filename);
   Py_VISIT(traverse_module_state->__pyx_n_s_filenames);
   Py_VISIT(traverse_module_state->__pyx_n_u_filter);
   Py_VISIT(traverse_module_state->__pyx_n_s_finalize);
@@ -3235,14 +3234,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_requests);
   Py_VISIT(traverse_module_state->__pyx_n_s_response);
   Py_VISIT(traverse_module_state->__pyx_n_s_response_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_result);
+  Py_VISIT(traverse_module_state->__pyx_n_s_result_lentgth);
   Py_VISIT(traverse_module_state->__pyx_n_s_reverse);
   Py_VISIT(traverse_module_state->__pyx_n_u_score);
   Py_VISIT(traverse_module_state->__pyx_kp_u_search);
   Py_VISIT(traverse_module_state->__pyx_n_u_searchScore);
   Py_VISIT(traverse_module_state->__pyx_n_u_searchindex);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_kp_u_set);
@@ -3438,15 +3438,14 @@
 #define __pyx_n_s_encoded_url __pyx_mstate_global->__pyx_n_s_encoded_url
 #define __pyx_n_s_encryptedText __pyx_mstate_global->__pyx_n_s_encryptedText
 #define __pyx_n_s_encryptor __pyx_mstate_global->__pyx_n_s_encryptor
 #define __pyx_n_s_enkyc __pyx_mstate_global->__pyx_n_s_enkyc
 #define __pyx_n_u_enkyc __pyx_mstate_global->__pyx_n_u_enkyc
 #define __pyx_n_u_error __pyx_mstate_global->__pyx_n_u_error
 #define __pyx_n_u_extracted_text __pyx_mstate_global->__pyx_n_u_extracted_text
-#define __pyx_n_s_extracted_text_length __pyx_mstate_global->__pyx_n_s_extracted_text_length
 #define __pyx_n_s_extracted_texts __pyx_mstate_global->__pyx_n_s_extracted_texts
 #define __pyx_n_u_file_data __pyx_mstate_global->__pyx_n_u_file_data
 #define __pyx_n_u_file_type __pyx_mstate_global->__pyx_n_u_file_type
 #define __pyx_n_u_filename __pyx_mstate_global->__pyx_n_u_filename
 #define __pyx_n_s_filenames __pyx_mstate_global->__pyx_n_s_filenames
 #define __pyx_n_u_filter __pyx_mstate_global->__pyx_n_u_filter
 #define __pyx_n_s_finalize __pyx_mstate_global->__pyx_n_s_finalize
@@ -3503,14 +3502,15 @@
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_requests __pyx_mstate_global->__pyx_n_s_requests
 #define __pyx_n_s_response __pyx_mstate_global->__pyx_n_s_response
 #define __pyx_n_s_response_data __pyx_mstate_global->__pyx_n_s_response_data
 #define __pyx_n_s_result __pyx_mstate_global->__pyx_n_s_result
+#define __pyx_n_s_result_lentgth __pyx_mstate_global->__pyx_n_s_result_lentgth
 #define __pyx_n_s_reverse __pyx_mstate_global->__pyx_n_s_reverse
 #define __pyx_n_u_score __pyx_mstate_global->__pyx_n_u_score
 #define __pyx_kp_u_search __pyx_mstate_global->__pyx_kp_u_search
 #define __pyx_n_u_searchScore __pyx_mstate_global->__pyx_n_u_searchScore
 #define __pyx_n_u_searchindex __pyx_mstate_global->__pyx_n_u_searchindex
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_kp_u_set __pyx_mstate_global->__pyx_kp_u_set
@@ -5933,16 +5933,16 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_connParam = 0;
-  PyObject *__pyx_v_extracted_text_length = 0;
-  int __pyx_v_vector_query;
+  int __pyx_v_result_lentgth;
+  PyObject *__pyx_v_vector_query = 0;
   int __pyx_v_top_n;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[4] = {0,0,0,0};
   int __pyx_lineno = 0;
@@ -5956,15 +5956,15 @@
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_connParam,&__pyx_n_s_extracted_text_length,&__pyx_n_s_vector_query,&__pyx_n_s_top_n,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_connParam,&__pyx_n_s_result_lentgth,&__pyx_n_s_vector_query,&__pyx_n_s_top_n,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -5982,15 +5982,15 @@
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_extracted_text_length)) != 0)) {
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_result_lentgth)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("vector_search", 1, 4, 4, 1); __PYX_ERR(0, 113, __pyx_L3_error)
         }
@@ -6024,16 +6024,16 @@
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
     __pyx_v_connParam = values[0];
-    __pyx_v_extracted_text_length = ((PyObject*)values[1]);
-    __pyx_v_vector_query = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_vector_query == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
+    __pyx_v_result_lentgth = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_result_lentgth == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
+    __pyx_v_vector_query = ((PyObject*)values[2]);
     __pyx_v_top_n = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_top_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("vector_search", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 113, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
@@ -6044,16 +6044,16 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_extracted_text_length), (&PyUnicode_Type), 1, "extracted_text_length", 1))) __PYX_ERR(0, 113, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_connParam, __pyx_v_extracted_text_length, __pyx_v_vector_query, __pyx_v_top_n);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vector_query), (&PyUnicode_Type), 1, "vector_query", 1))) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_connParam, __pyx_v_result_lentgth, __pyx_v_vector_query, __pyx_v_top_n);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -6186,15 +6186,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, int __pyx_v_vector_query, int __pyx_v_top_n) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, int __pyx_v_result_lentgth, PyObject *__pyx_v_vector_query, int __pyx_v_top_n) {
   PyObject *__pyx_v_url = NULL;
   PyObject *__pyx_v_headers = NULL;
   PyObject *__pyx_v_pipeline = NULL;
   PyObject *__pyx_v_query_payload = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_similarities = NULL;
   PyObject *__pyx_v_response_data = NULL;
@@ -6281,18 +6281,15 @@
   __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_searchindex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_index, __pyx_t_3) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_vector_query); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_query, __pyx_t_5) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_query, __pyx_v_vector_query) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
 
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_wildcard, __pyx_kp_u__6) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_path, __pyx_t_5) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_text, __pyx_t_3) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
@@ -6425,35 +6422,32 @@
     __pyx_t_1 = 0;
 
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_vector_query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = NULL;
+    __pyx_t_2 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_3)) {
+      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
         __pyx_t_4 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_2};
+      PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_vector_query};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_v_query_vec = __pyx_t_1;
     __pyx_t_1 = 0;
 
@@ -6720,15 +6714,18 @@
           __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_INCREF(__pyx_v_cleaned_text);
           __Pyx_GIVEREF(__pyx_v_cleaned_text);
           if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_cleaned_text)) __PYX_ERR(0, 175, __pyx_L1_error);
           __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
-          if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_length, __pyx_v_extracted_text_length) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
+          __pyx_t_13 = __Pyx_PyInt_From_int(__pyx_v_result_lentgth); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 175, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_13);
+          if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_length, __pyx_t_13) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 175, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_extracted_text, __pyx_t_13) < 0) __PYX_ERR(0, 174, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
@@ -7948,15 +7945,14 @@
     {&__pyx_n_s_encoded_url, __pyx_k_encoded_url, sizeof(__pyx_k_encoded_url), 0, 0, 1, 1},
     {&__pyx_n_s_encryptedText, __pyx_k_encryptedText, sizeof(__pyx_k_encryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_encryptor, __pyx_k_encryptor, sizeof(__pyx_k_encryptor), 0, 0, 1, 1},
     {&__pyx_n_s_enkyc, __pyx_k_enkyc, sizeof(__pyx_k_enkyc), 0, 0, 1, 1},
     {&__pyx_n_u_enkyc, __pyx_k_enkyc, sizeof(__pyx_k_enkyc), 0, 1, 0, 1},
     {&__pyx_n_u_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 1, 0, 1},
     {&__pyx_n_u_extracted_text, __pyx_k_extracted_text, sizeof(__pyx_k_extracted_text), 0, 1, 0, 1},
-    {&__pyx_n_s_extracted_text_length, __pyx_k_extracted_text_length, sizeof(__pyx_k_extracted_text_length), 0, 0, 1, 1},
     {&__pyx_n_s_extracted_texts, __pyx_k_extracted_texts, sizeof(__pyx_k_extracted_texts), 0, 0, 1, 1},
     {&__pyx_n_u_file_data, __pyx_k_file_data, sizeof(__pyx_k_file_data), 0, 1, 0, 1},
     {&__pyx_n_u_file_type, __pyx_k_file_type, sizeof(__pyx_k_file_type), 0, 1, 0, 1},
     {&__pyx_n_u_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 1, 0, 1},
     {&__pyx_n_s_filenames, __pyx_k_filenames, sizeof(__pyx_k_filenames), 0, 0, 1, 1},
     {&__pyx_n_u_filter, __pyx_k_filter, sizeof(__pyx_k_filter), 0, 1, 0, 1},
     {&__pyx_n_s_finalize, __pyx_k_finalize, sizeof(__pyx_k_finalize), 0, 0, 1, 1},
@@ -8013,14 +8009,15 @@
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
     {&__pyx_n_s_requests, __pyx_k_requests, sizeof(__pyx_k_requests), 0, 0, 1, 1},
     {&__pyx_n_s_response, __pyx_k_response, sizeof(__pyx_k_response), 0, 0, 1, 1},
     {&__pyx_n_s_response_data, __pyx_k_response_data, sizeof(__pyx_k_response_data), 0, 0, 1, 1},
     {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
+    {&__pyx_n_s_result_lentgth, __pyx_k_result_lentgth, sizeof(__pyx_k_result_lentgth), 0, 0, 1, 1},
     {&__pyx_n_s_reverse, __pyx_k_reverse, sizeof(__pyx_k_reverse), 0, 0, 1, 1},
     {&__pyx_n_u_score, __pyx_k_score, sizeof(__pyx_k_score), 0, 1, 0, 1},
     {&__pyx_kp_u_search, __pyx_k_search, sizeof(__pyx_k_search), 0, 1, 0, 0},
     {&__pyx_n_u_searchScore, __pyx_k_searchScore, sizeof(__pyx_k_searchScore), 0, 1, 0, 1},
     {&__pyx_n_u_searchindex, __pyx_k_searchindex, sizeof(__pyx_k_searchindex), 0, 1, 0, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
     {&__pyx_kp_u_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 1, 0, 0},
@@ -8141,15 +8138,15 @@
   __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeText, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 67, __pyx_L1_error)
 
   __pyx_tuple__20 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
   __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SaveToMongoDb, 81, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 81, __pyx_L1_error)
 
-  __pyx_tuple__22 = PyTuple_Pack(27, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_extracted_text_length, __pyx_n_s_vector_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_similarities, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_query_vec, __pyx_n_s_doc, __pyx_n_s_embeddings, __pyx_n_s_emb, __pyx_n_s_emb_vec, __pyx_n_s_similar_score, __pyx_n_s_cleaned_text, __pyx_n_s_top_results, __pyx_n_s_extracted_texts, __pyx_n_s_similarities_values, __pyx_n_s_filenames, __pyx_n_s_result, __pyx_n_s_result, __pyx_n_s_result); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(27, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_result_lentgth, __pyx_n_s_vector_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_similarities, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_query_vec, __pyx_n_s_doc, __pyx_n_s_embeddings, __pyx_n_s_emb, __pyx_n_s_emb_vec, __pyx_n_s_similar_score, __pyx_n_s_cleaned_text, __pyx_n_s_top_results, __pyx_n_s_extracted_texts, __pyx_n_s_similarities_values, __pyx_n_s_filenames, __pyx_n_s_result, __pyx_n_s_result, __pyx_n_s_result); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
   __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vector_search, 113, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 113, __pyx_L1_error)
 
   __pyx_tuple__24 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
```

### Comparing `aixhello-3.7/aixhello.egg-info/PKG-INFO` & `aixhello-3.8/aixhello.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.7
+Version: 3.8
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.7/setup.py` & `aixhello-3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='3.7',  # Increment the version number
+    version='3.8',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

