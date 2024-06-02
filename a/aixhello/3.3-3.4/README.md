# Comparing `tmp/aixhello-3.3.tar.gz` & `tmp/aixhello-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-3.3.tar", last modified: Sun Jun  2 03:25:28 2024, max compression
+gzip compressed data, was "aixhello-3.4.tar", last modified: Sun Jun  2 04:21:42 2024, max compression
```

## Comparing `aixhello-3.3.tar` & `aixhello-3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 03:25:28.923957 aixhello-3.3/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.3/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-02 03:25:28.922958 aixhello-3.3/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 03:25:28.896556 aixhello-3.3/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.3/aixhello/__init__.py
--rw-rw-rw-   0        0        0   589974 2024-06-02 03:25:20.000000 aixhello-3.3/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-02 03:25:28.920544 aixhello-3.3/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-02 03:25:28.000000 aixhello-3.3/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-02 03:25:28.000000 aixhello-3.3/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 03:25:28.000000 aixhello-3.3/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-02 03:25:28.000000 aixhello-3.3/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 03:25:28.000000 aixhello-3.3/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-02 03:25:28.929971 aixhello-3.3/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-02 03:24:43.000000 aixhello-3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:21:42.605246 aixhello-3.4/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.4/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-02 04:21:42.605246 aixhello-3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 04:21:42.573837 aixhello-3.4/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.4/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   558293 2024-06-02 04:21:33.000000 aixhello-3.4/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-02 04:21:42.603240 aixhello-3.4/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-02 04:21:42.000000 aixhello-3.4/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-02 04:21:42.000000 aixhello-3.4/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 04:21:42.000000 aixhello-3.4/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-02 04:21:42.000000 aixhello-3.4/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 04:21:42.000000 aixhello-3.4/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-02 04:21:42.607260 aixhello-3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-02 04:21:05.000000 aixhello-3.4/setup.py
```

### Comparing `aixhello-3.3/LICENSE` & `aixhello-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-3.3/PKG-INFO` & `aixhello-3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.3
+Version: 3.4
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.3/README.md` & `aixhello-3.4/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-3.3/aixhello/xyello.c` & `aixhello-3.4/aixhello/xyello.c`

 * *Files 1% similar despite different names*

```diff
@@ -1935,28 +1935,37 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
-/* PyIntCompare.proto */
-static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
+/* KeywordStringCheck.proto */
+static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
+
+/* GetAttr3.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
+
+/* RaiseUnexpectedTypeError.proto */
+static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
 
 /* DictGetItem.proto */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
 #define __Pyx_PyObject_Dict_GetItem(obj, name)\
     (likely(PyDict_CheckExact(obj)) ?\
      __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
 #else
 #define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
 #define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
 #endif
 
+/* PyIntCompare.proto */
+static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
+
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* PyObjectCall2Args.proto */
@@ -2158,23 +2167,14 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
 
-/* KeywordStringCheck.proto */
-static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
-
-/* GetAttr3.proto */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
-
-/* RaiseUnexpectedTypeError.proto */
-static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
-
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* RaiseException.proto */
@@ -2303,161 +2303,158 @@
 
 /* Implementation of "aixhello.xyello" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_chr;
 static PyObject *__pyx_builtin_print;
 static PyObject *__pyx_builtin_sorted;
 /* #### Code section: string_decls ### */
-static const char __pyx_k_[] = "";
+static const char __pyx_k_[] = "*";
 static const char __pyx_k_e[] = "e";
 static const char __pyx_k_x[] = "x";
-static const char __pyx_k__6[] = "*";
-static const char __pyx_k__8[] = "...";
+static const char __pyx_k__4[] = ".";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_iv[] = "iv";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_re[] = "re";
 static const char __pyx_k_AES[] = "AES";
 static const char __pyx_k_CBC[] = "CBC";
-static const char __pyx_k__10[] = ".";
-static const char __pyx_k__35[] = "?";
+static const char __pyx_k__24[] = "?";
 static const char __pyx_k_chr[] = "chr";
 static const char __pyx_k_doc[] = "doc";
 static const char __pyx_k_dot[] = "dot";
 static const char __pyx_k_emb[] = "emb";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_msg[] = "msg";
 static const char __pyx_k_mth[] = "mth";
 static const char __pyx_k_new[] = "__new__";
-static const char __pyx_k_set[] = "$set";
 static const char __pyx_k_url[] = "url";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_json[] = "json";
 static const char __pyx_k_main[] = "__main__";
+static const char __pyx_k_meta[] = "$meta";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_norm[] = "norm";
+static const char __pyx_k_path[] = "path";
 static const char __pyx_k_post[] = "post";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_text[] = "text";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_chunk[] = "chunk";
 static const char __pyx_k_enkyc[] = "enkyc";
 static const char __pyx_k_error[] = "error";
+static const char __pyx_k_index[] = "index";
 static const char __pyx_k_input[] = "input";
+static const char __pyx_k_limit[] = "$limit";
 static const char __pyx_k_model[] = "model";
 static const char __pyx_k_modes[] = "modes";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_print[] = "print";
+static const char __pyx_k_query[] = "query";
+static const char __pyx_k_score[] = "score";
 static const char __pyx_k_state[] = "state";
 static const char __pyx_k_top_n[] = "top_n";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_Cipher[] = "Cipher";
 static const char __pyx_k_append[] = "append";
 static const char __pyx_k_base64[] = "base64";
 static const char __pyx_k_cipher[] = "cipher";
 static const char __pyx_k_create[] = "create";
 static const char __pyx_k_decode[] = "decode";
 static const char __pyx_k_dict_2[] = "_dict";
 static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_encode[] = "encode";
-static const char __pyx_k_filter[] = "filter";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_linalg[] = "linalg";
 static const char __pyx_k_openai[] = "openai";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_result[] = "result";
+static const char __pyx_k_search[] = "$search";
 static const char __pyx_k_sorted[] = "sorted";
 static const char __pyx_k_update[] = "update";
-static const char __pyx_k_upsert[] = "upsert";
 static const char __pyx_k_xyellw[] = "xyellw";
 static const char __pyx_k_api_key[] = "api_key";
 static const char __pyx_k_api_url[] = "api_url";
 static const char __pyx_k_backend[] = "backend";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_emb_vec[] = "emb_vec";
 static const char __pyx_k_headers[] = "headers";
 static const char __pyx_k_message[] = "message";
-static const char __pyx_k_payload[] = "payload";
 static const char __pyx_k_project[] = "$project";
 static const char __pyx_k_reverse[] = "reverse";
 static const char __pyx_k_strText[] = "strText";
 static const char __pyx_k_database[] = "database";
 static const char __pyx_k_filename[] = "filename";
 static const char __pyx_k_finalize[] = "finalize";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_pipeline[] = "pipeline";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_requests[] = "requests";
 static const char __pyx_k_response[] = "response";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_text_key[] = "text_key";
+static const char __pyx_k_wildcard[] = "wildcard";
 static const char __pyx_k_Decenigma[] = "Decenigma";
 static const char __pyx_k_Decipherx[] = "Decipherx";
 static const char __pyx_k_Encapseal[] = "Encapseal";
 static const char __pyx_k_api_key_2[] = "api-key";
 static const char __pyx_k_b64decode[] = "b64decode";
 static const char __pyx_k_b64encode[] = "b64encode";
 static const char __pyx_k_connParam[] = "connParam";
 static const char __pyx_k_decryptor[] = "decryptor";
 static const char __pyx_k_documents[] = "documents";
 static const char __pyx_k_embedding[] = "embedding";
 static const char __pyx_k_encryptor[] = "encryptor";
-static const char __pyx_k_file_data[] = "file_data";
-static const char __pyx_k_file_type[] = "file_type";
 static const char __pyx_k_filenames[] = "filenames";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_query_vec[] = "query_vec";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_algorithms[] = "algorithms";
 static const char __pyx_k_collection[] = "collection";
 static const char __pyx_k_dataSource[] = "dataSource";
-static const char __pyx_k_datasource[] = "datasource";
 static const char __pyx_k_embeddings[] = "embeddings";
 static const char __pyx_k_max_length[] = "max_length";
 static const char __pyx_k_pad_length[] = "pad_length";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_similarity[] = "similarity";
 static const char __pyx_k_text_embed[] = "text_embed";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_encoded_url[] = "encoded_url";
 static const char __pyx_k_padded_text[] = "padded_text";
-static const char __pyx_k_params_dict[] = "params_dict";
+static const char __pyx_k_searchScore[] = "searchScore";
+static const char __pyx_k_searchindex[] = "searchindex";
 static const char __pyx_k_status_code[] = "status_code";
 static const char __pyx_k_text_chunks[] = "text_chunks";
 static const char __pyx_k_top_results[] = "top_results";
 static const char __pyx_k_Content_Type[] = "Content-Type";
 static const char __pyx_k_cleaned_text[] = "cleaned_text";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_shorten_text[] = "shorten_text";
 static const char __pyx_k_similarities[] = "similarities";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_use_setstate[] = "use_setstate";
 static const char __pyx_k_vector_query[] = "vector_query";
-static const char __pyx_k_SaveToMongoDb[] = "SaveToMongoDb";
 static const char __pyx_k_decryptedText[] = "decryptedText";
-static const char __pyx_k_decrypted_url[] = "decrypted_url";
 static const char __pyx_k_encryptedText[] = "encryptedText";
 static const char __pyx_k_query_payload[] = "query_payload";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_response_data[] = "response_data";
 static const char __pyx_k_similar_score[] = "similar_score";
 static const char __pyx_k_vector_search[] = "vector_search";
 static const char __pyx_k_vectorizeText[] = "vectorizeText";
 static const char __pyx_k_extracted_text[] = "extracted_text";
 static const char __pyx_k_vectorizeEmbed[] = "vectorizeEmbed";
 static const char __pyx_k_aixhello_xyello[] = "aixhello.xyello";
-static const char __pyx_k_application_pdf[] = "application/pdf";
 static const char __pyx_k_default_backend[] = "default_backend";
 static const char __pyx_k_extracted_texts[] = "extracted_texts";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_text_embeddings[] = "text_embeddings";
 static const char __pyx_k_Unknown_filename[] = "Unknown filename";
 static const char __pyx_k_application_json[] = "application/json";
@@ -2467,17 +2464,14 @@
 static const char __pyx_k_y1c8_8BxP9XN_VKM[] = "y1c8@8BxP9XN#VKM";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_AuthenticationError[] = "AuthenticationError";
 static const char __pyx_k_aixhello_xyello_pyx[] = "aixhello\\xyello.pyx";
 static const char __pyx_k_pyx_unpickle_xyellw[] = "__pyx_unpickle_xyellw";
 static const char __pyx_k_similarities_values[] = "similarities_values";
-static const char __pyx_k_xyellw_shorten_text[] = "xyellw.shorten_text";
-static const char __pyx_k_xyellw_SaveToMongoDb[] = "xyellw.SaveToMongoDb";
-static const char __pyx_k_xyellw_vector_search[] = "xyellw.vector_search";
 static const char __pyx_k_xyellw_vectorizeText[] = "xyellw.vectorizeText";
 static const char __pyx_k_decoded_encryptedText[] = "decoded_encryptedText";
 static const char __pyx_k_decrypted_padded_text[] = "decrypted_padded_text";
 static const char __pyx_k_extracted_text_length[] = "extracted_text_length";
 static const char __pyx_k_xyellw_vectorizeEmbed[] = "xyellw.vectorizeEmbed";
 static const char __pyx_k_text_embedding_ada_002[] = "text-embedding-ada-002";
 static const char __pyx_k_xyellw___reduce_cython[] = "xyellw.__reduce_cython__";
@@ -2485,34 +2479,30 @@
 static const char __pyx_k_xyellw___setstate_cython[] = "xyellw.__setstate_cython__";
 static const char __pyx_k_vector_search_locals_lambda[] = "vector_search.<locals>.<lambda>";
 static const char __pyx_k_An_unexpected_error_occurred[] = "An unexpected error occurred";
 static const char __pyx_k_cryptography_hazmat_backends[] = "cryptography.hazmat.backends";
 static const char __pyx_k_Access_Control_Request_Headers[] = "Access-Control-Request-Headers";
 static const char __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN[] = "M#rztXq3z@U8rS5jN@PvE4W7F&J(#DhN";
 static const char __pyx_k_Request_failed_with_status_code[] = "Request failed with status code: ";
-static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4BFhKWk32xGPxL9k3jhhHkDqcCQrX37yfmobUNPTXxEGQ==";
+static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4AsrMkJF3D7AnEcHok5damnRp1itFTxnx2dNcFig8Q+Zg==";
 static const char __pyx_k_text_embeddings_key_not_found_i[] = "'text_embeddings' key not found in document with filename: ";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())";
-static const char __pyx_k_Successfully_save_to_the_databas[] = "Successfully save to the database.";
 static const char __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1[] = "aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1cmUvc0xwaG9RdURybDZv";
 static const char __pyx_k_cryptography_hazmat_primitives_c[] = "cryptography.hazmat.primitives.ciphers";
-static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4AsrMkJF3D7AnEcHok5damnRp1itFTxnx2dNcFig8Q+Zg==";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbed(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8vectorizeText(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_embed, PyObject *__pyx_v_text_key); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, PyObject *__pyx_v_vector_query, PyObject *__pyx_v_top_n); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14shorten_text(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_max_length); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_18__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_vector_search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, PyObject *__pyx_v_vector_query, PyObject *__pyx_v_top_n); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_2__pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
@@ -2537,14 +2527,15 @@
   #ifdef __Pyx_Coroutine_USED
   PyTypeObject *__pyx_CoroutineType;
   #endif
   #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_8aixhello_6xyello_xyellw;
   #endif
   PyTypeObject *__pyx_ptype_8aixhello_6xyello_xyellw;
+  PyObject *__pyx_n_s_;
   PyObject *__pyx_kp_u_;
   PyObject *__pyx_n_s_AES;
   PyObject *__pyx_kp_u_Access_Control_Request_Headers;
   PyObject *__pyx_kp_u_An_unexpected_error_occurred;
   PyObject *__pyx_n_s_AuthenticationError;
   PyObject *__pyx_n_s_CBC;
   PyObject *__pyx_n_s_Cipher;
@@ -2553,61 +2544,50 @@
   PyObject *__pyx_n_s_Decipherx;
   PyObject *__pyx_n_s_Encapseal;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_kp_u_Invalid_API_key_provided;
   PyObject *__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_kp_u_Request_failed_with_status_code;
-  PyObject *__pyx_n_s_SaveToMongoDb;
-  PyObject *__pyx_kp_u_Successfully_save_to_the_databas;
   PyObject *__pyx_kp_u_Unknown_filename;
-  PyObject *__pyx_kp_u__10;
-  PyObject *__pyx_n_s__35;
-  PyObject *__pyx_n_s__6;
-  PyObject *__pyx_kp_u__6;
-  PyObject *__pyx_kp_u__8;
+  PyObject *__pyx_n_s__24;
+  PyObject *__pyx_kp_u__4;
   PyObject *__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1;
   PyObject *__pyx_n_s_aixhello_xyello;
   PyObject *__pyx_kp_s_aixhello_xyello_pyx;
   PyObject *__pyx_n_s_algorithms;
   PyObject *__pyx_n_s_api_key;
   PyObject *__pyx_kp_u_api_key_2;
   PyObject *__pyx_n_s_api_url;
   PyObject *__pyx_n_s_append;
   PyObject *__pyx_kp_u_application_json;
-  PyObject *__pyx_kp_u_application_pdf;
   PyObject *__pyx_n_s_array;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_b64decode;
   PyObject *__pyx_n_s_b64encode;
   PyObject *__pyx_n_s_backend;
   PyObject *__pyx_n_s_base64;
   PyObject *__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn;
-  PyObject *__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2;
   PyObject *__pyx_n_s_chr;
   PyObject *__pyx_n_s_chunk;
   PyObject *__pyx_n_s_cipher;
   PyObject *__pyx_n_s_cleaned_text;
   PyObject *__pyx_n_s_cline_in_traceback;
-  PyObject *__pyx_n_s_collection;
   PyObject *__pyx_n_u_collection;
   PyObject *__pyx_n_s_connParam;
   PyObject *__pyx_n_s_create;
   PyObject *__pyx_n_s_cryptography_hazmat_backends;
   PyObject *__pyx_n_s_cryptography_hazmat_primitives_c;
   PyObject *__pyx_n_s_data;
   PyObject *__pyx_n_u_dataSource;
-  PyObject *__pyx_n_s_database;
   PyObject *__pyx_n_u_database;
-  PyObject *__pyx_n_s_datasource;
   PyObject *__pyx_n_s_decode;
   PyObject *__pyx_n_s_decoded_encryptedText;
   PyObject *__pyx_n_s_decryptedText;
   PyObject *__pyx_n_s_decrypted_padded_text;
-  PyObject *__pyx_n_s_decrypted_url;
   PyObject *__pyx_n_s_decryptor;
   PyObject *__pyx_n_s_default_backend;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_dict_2;
   PyObject *__pyx_kp_u_disable;
   PyObject *__pyx_n_s_doc;
   PyObject *__pyx_n_s_documents;
@@ -2619,81 +2599,83 @@
   PyObject *__pyx_n_s_embedding;
   PyObject *__pyx_n_s_embeddings;
   PyObject *__pyx_kp_u_enable;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_encoded_url;
   PyObject *__pyx_n_s_encryptedText;
   PyObject *__pyx_n_s_encryptor;
-  PyObject *__pyx_n_s_enkyc;
   PyObject *__pyx_n_u_enkyc;
   PyObject *__pyx_n_u_error;
   PyObject *__pyx_n_u_extracted_text;
   PyObject *__pyx_n_s_extracted_text_length;
   PyObject *__pyx_n_s_extracted_texts;
-  PyObject *__pyx_n_u_file_data;
-  PyObject *__pyx_n_u_file_type;
   PyObject *__pyx_n_u_filename;
   PyObject *__pyx_n_s_filenames;
-  PyObject *__pyx_n_u_filter;
   PyObject *__pyx_n_s_finalize;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_get;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_n_s_headers;
   PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_u_index;
   PyObject *__pyx_n_s_initializing;
   PyObject *__pyx_n_s_input;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_iv;
   PyObject *__pyx_n_s_json;
   PyObject *__pyx_n_s_key;
+  PyObject *__pyx_kp_u_limit;
   PyObject *__pyx_n_s_linalg;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_max_length;
   PyObject *__pyx_n_u_message;
+  PyObject *__pyx_kp_u_meta;
   PyObject *__pyx_n_s_model;
   PyObject *__pyx_n_s_modes;
   PyObject *__pyx_n_s_msg;
   PyObject *__pyx_n_s_mth;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_n_s_norm;
   PyObject *__pyx_n_s_np;
   PyObject *__pyx_n_s_numpy;
   PyObject *__pyx_n_s_openai;
   PyObject *__pyx_n_s_pad_length;
   PyObject *__pyx_n_s_padded_text;
-  PyObject *__pyx_n_s_params_dict;
-  PyObject *__pyx_n_s_payload;
+  PyObject *__pyx_n_u_path;
   PyObject *__pyx_n_s_pickle;
   PyObject *__pyx_n_s_pipeline;
   PyObject *__pyx_n_u_pipeline;
   PyObject *__pyx_n_s_post;
   PyObject *__pyx_n_s_print;
   PyObject *__pyx_kp_u_project;
   PyObject *__pyx_n_s_pyx_PickleError;
   PyObject *__pyx_n_s_pyx_checksum;
   PyObject *__pyx_n_s_pyx_result;
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_pyx_type;
   PyObject *__pyx_n_s_pyx_unpickle_xyellw;
+  PyObject *__pyx_n_u_query;
   PyObject *__pyx_n_s_query_payload;
   PyObject *__pyx_n_s_query_vec;
   PyObject *__pyx_n_s_re;
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_requests;
   PyObject *__pyx_n_s_response;
   PyObject *__pyx_n_s_response_data;
   PyObject *__pyx_n_s_result;
   PyObject *__pyx_n_s_reverse;
+  PyObject *__pyx_n_u_score;
+  PyObject *__pyx_kp_u_search;
+  PyObject *__pyx_n_u_searchScore;
+  PyObject *__pyx_n_u_searchindex;
   PyObject *__pyx_n_s_self;
-  PyObject *__pyx_kp_u_set;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_shorten_text;
   PyObject *__pyx_n_s_similar_score;
   PyObject *__pyx_n_s_similarities;
   PyObject *__pyx_n_s_similarities_values;
   PyObject *__pyx_n_u_similarity;
@@ -2701,83 +2683,70 @@
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_state;
   PyObject *__pyx_n_s_status_code;
   PyObject *__pyx_n_s_strText;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_text;
+  PyObject *__pyx_n_u_text;
   PyObject *__pyx_n_s_text_chunks;
   PyObject *__pyx_n_s_text_embed;
   PyObject *__pyx_kp_u_text_embedding_ada_002;
   PyObject *__pyx_n_u_text_embeddings;
   PyObject *__pyx_kp_u_text_embeddings_key_not_found_i;
   PyObject *__pyx_n_s_text_key;
   PyObject *__pyx_n_s_top_n;
   PyObject *__pyx_n_s_top_results;
   PyObject *__pyx_n_s_update;
-  PyObject *__pyx_n_u_update;
-  PyObject *__pyx_n_u_upsert;
   PyObject *__pyx_n_s_url;
   PyObject *__pyx_n_s_use_setstate;
   PyObject *__pyx_kp_u_utf_8;
   PyObject *__pyx_n_s_vector_query;
   PyObject *__pyx_n_s_vector_search;
   PyObject *__pyx_n_s_vector_search_locals_lambda;
   PyObject *__pyx_n_s_vectorizeEmbed;
   PyObject *__pyx_n_s_vectorizeText;
+  PyObject *__pyx_n_u_wildcard;
   PyObject *__pyx_n_s_x;
   PyObject *__pyx_n_s_xyellw;
   PyObject *__pyx_n_s_xyellw_Decenigma;
   PyObject *__pyx_n_s_xyellw_Decipherx;
   PyObject *__pyx_n_s_xyellw_Encapseal;
-  PyObject *__pyx_n_s_xyellw_SaveToMongoDb;
   PyObject *__pyx_n_s_xyellw___reduce_cython;
   PyObject *__pyx_n_s_xyellw___setstate_cython;
-  PyObject *__pyx_n_s_xyellw_shorten_text;
-  PyObject *__pyx_n_s_xyellw_vector_search;
   PyObject *__pyx_n_s_xyellw_vectorizeEmbed;
   PyObject *__pyx_n_s_xyellw_vectorizeText;
   PyObject *__pyx_kp_b_y1c8_8BxP9XN_VKM;
   PyObject *__pyx_int_1;
   PyObject *__pyx_int_5;
   PyObject *__pyx_int_200;
-  PyObject *__pyx_int_1000;
   PyObject *__pyx_int_222419149;
   PyObject *__pyx_int_228825662;
   PyObject *__pyx_int_238750788;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__3;
-  PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__5;
   PyObject *__pyx_tuple__7;
   PyObject *__pyx_tuple__9;
   PyObject *__pyx_tuple__11;
   PyObject *__pyx_tuple__13;
   PyObject *__pyx_tuple__15;
   PyObject *__pyx_tuple__17;
   PyObject *__pyx_tuple__19;
   PyObject *__pyx_tuple__21;
-  PyObject *__pyx_tuple__23;
-  PyObject *__pyx_tuple__25;
-  PyObject *__pyx_tuple__26;
-  PyObject *__pyx_tuple__28;
-  PyObject *__pyx_tuple__29;
-  PyObject *__pyx_tuple__31;
-  PyObject *__pyx_tuple__33;
+  PyObject *__pyx_tuple__22;
+  PyObject *__pyx_codeobj__6;
+  PyObject *__pyx_codeobj__8;
+  PyObject *__pyx_codeobj__10;
   PyObject *__pyx_codeobj__12;
   PyObject *__pyx_codeobj__14;
   PyObject *__pyx_codeobj__16;
   PyObject *__pyx_codeobj__18;
   PyObject *__pyx_codeobj__20;
-  PyObject *__pyx_codeobj__22;
-  PyObject *__pyx_codeobj__24;
-  PyObject *__pyx_codeobj__27;
-  PyObject *__pyx_codeobj__30;
-  PyObject *__pyx_codeobj__32;
-  PyObject *__pyx_codeobj__34;
+  PyObject *__pyx_codeobj__23;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2814,14 +2783,15 @@
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_8aixhello_6xyello_xyellw);
   Py_CLEAR(clear_module_state->__pyx_type_8aixhello_6xyello_xyellw);
+  Py_CLEAR(clear_module_state->__pyx_n_s_);
   Py_CLEAR(clear_module_state->__pyx_kp_u_);
   Py_CLEAR(clear_module_state->__pyx_n_s_AES);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Access_Control_Request_Headers);
   Py_CLEAR(clear_module_state->__pyx_kp_u_An_unexpected_error_occurred);
   Py_CLEAR(clear_module_state->__pyx_n_s_AuthenticationError);
   Py_CLEAR(clear_module_state->__pyx_n_s_CBC);
   Py_CLEAR(clear_module_state->__pyx_n_s_Cipher);
@@ -2830,61 +2800,50 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_Decipherx);
   Py_CLEAR(clear_module_state->__pyx_n_s_Encapseal);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_API_key_provided);
   Py_CLEAR(clear_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Request_failed_with_status_code);
-  Py_CLEAR(clear_module_state->__pyx_n_s_SaveToMongoDb);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Unknown_filename);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__10);
-  Py_CLEAR(clear_module_state->__pyx_n_s__35);
-  Py_CLEAR(clear_module_state->__pyx_n_s__6);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__6);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__8);
+  Py_CLEAR(clear_module_state->__pyx_n_s__24);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__4);
   Py_CLEAR(clear_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_CLEAR(clear_module_state->__pyx_n_s_aixhello_xyello);
   Py_CLEAR(clear_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithms);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_key);
   Py_CLEAR(clear_module_state->__pyx_kp_u_api_key_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_append);
   Py_CLEAR(clear_module_state->__pyx_kp_u_application_json);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_application_pdf);
   Py_CLEAR(clear_module_state->__pyx_n_s_array);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_b64decode);
   Py_CLEAR(clear_module_state->__pyx_n_s_b64encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_backend);
   Py_CLEAR(clear_module_state->__pyx_n_s_base64);
   Py_CLEAR(clear_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_chr);
   Py_CLEAR(clear_module_state->__pyx_n_s_chunk);
   Py_CLEAR(clear_module_state->__pyx_n_s_cipher);
   Py_CLEAR(clear_module_state->__pyx_n_s_cleaned_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
-  Py_CLEAR(clear_module_state->__pyx_n_s_collection);
   Py_CLEAR(clear_module_state->__pyx_n_u_collection);
   Py_CLEAR(clear_module_state->__pyx_n_s_connParam);
   Py_CLEAR(clear_module_state->__pyx_n_s_create);
   Py_CLEAR(clear_module_state->__pyx_n_s_cryptography_hazmat_backends);
   Py_CLEAR(clear_module_state->__pyx_n_s_cryptography_hazmat_primitives_c);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
   Py_CLEAR(clear_module_state->__pyx_n_u_dataSource);
-  Py_CLEAR(clear_module_state->__pyx_n_s_database);
   Py_CLEAR(clear_module_state->__pyx_n_u_database);
-  Py_CLEAR(clear_module_state->__pyx_n_s_datasource);
   Py_CLEAR(clear_module_state->__pyx_n_s_decode);
   Py_CLEAR(clear_module_state->__pyx_n_s_decoded_encryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_decryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_decrypted_padded_text);
-  Py_CLEAR(clear_module_state->__pyx_n_s_decrypted_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_decryptor);
   Py_CLEAR(clear_module_state->__pyx_n_s_default_backend);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict_2);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
   Py_CLEAR(clear_module_state->__pyx_n_s_doc);
   Py_CLEAR(clear_module_state->__pyx_n_s_documents);
@@ -2896,81 +2855,83 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_embedding);
   Py_CLEAR(clear_module_state->__pyx_n_s_embeddings);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_encoded_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptor);
-  Py_CLEAR(clear_module_state->__pyx_n_s_enkyc);
   Py_CLEAR(clear_module_state->__pyx_n_u_enkyc);
   Py_CLEAR(clear_module_state->__pyx_n_u_error);
   Py_CLEAR(clear_module_state->__pyx_n_u_extracted_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_extracted_text_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_extracted_texts);
-  Py_CLEAR(clear_module_state->__pyx_n_u_file_data);
-  Py_CLEAR(clear_module_state->__pyx_n_u_file_type);
   Py_CLEAR(clear_module_state->__pyx_n_u_filename);
   Py_CLEAR(clear_module_state->__pyx_n_s_filenames);
-  Py_CLEAR(clear_module_state->__pyx_n_u_filter);
   Py_CLEAR(clear_module_state->__pyx_n_s_finalize);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_get);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_headers);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_u_index);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
   Py_CLEAR(clear_module_state->__pyx_n_s_input);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_iv);
   Py_CLEAR(clear_module_state->__pyx_n_s_json);
   Py_CLEAR(clear_module_state->__pyx_n_s_key);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_limit);
   Py_CLEAR(clear_module_state->__pyx_n_s_linalg);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_max_length);
   Py_CLEAR(clear_module_state->__pyx_n_u_message);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_meta);
   Py_CLEAR(clear_module_state->__pyx_n_s_model);
   Py_CLEAR(clear_module_state->__pyx_n_s_modes);
   Py_CLEAR(clear_module_state->__pyx_n_s_msg);
   Py_CLEAR(clear_module_state->__pyx_n_s_mth);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_n_s_norm);
   Py_CLEAR(clear_module_state->__pyx_n_s_np);
   Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
   Py_CLEAR(clear_module_state->__pyx_n_s_openai);
   Py_CLEAR(clear_module_state->__pyx_n_s_pad_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_padded_text);
-  Py_CLEAR(clear_module_state->__pyx_n_s_params_dict);
-  Py_CLEAR(clear_module_state->__pyx_n_s_payload);
+  Py_CLEAR(clear_module_state->__pyx_n_u_path);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
   Py_CLEAR(clear_module_state->__pyx_n_s_pipeline);
   Py_CLEAR(clear_module_state->__pyx_n_u_pipeline);
   Py_CLEAR(clear_module_state->__pyx_n_s_post);
   Py_CLEAR(clear_module_state->__pyx_n_s_print);
   Py_CLEAR(clear_module_state->__pyx_kp_u_project);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_xyellw);
+  Py_CLEAR(clear_module_state->__pyx_n_u_query);
   Py_CLEAR(clear_module_state->__pyx_n_s_query_payload);
   Py_CLEAR(clear_module_state->__pyx_n_s_query_vec);
   Py_CLEAR(clear_module_state->__pyx_n_s_re);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_requests);
   Py_CLEAR(clear_module_state->__pyx_n_s_response);
   Py_CLEAR(clear_module_state->__pyx_n_s_response_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_reverse);
+  Py_CLEAR(clear_module_state->__pyx_n_u_score);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_search);
+  Py_CLEAR(clear_module_state->__pyx_n_u_searchScore);
+  Py_CLEAR(clear_module_state->__pyx_n_u_searchindex);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_set);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_shorten_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_similar_score);
   Py_CLEAR(clear_module_state->__pyx_n_s_similarities);
   Py_CLEAR(clear_module_state->__pyx_n_s_similarities_values);
   Py_CLEAR(clear_module_state->__pyx_n_u_similarity);
@@ -2978,83 +2939,70 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_status_code);
   Py_CLEAR(clear_module_state->__pyx_n_s_strText);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_text);
+  Py_CLEAR(clear_module_state->__pyx_n_u_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_text_chunks);
   Py_CLEAR(clear_module_state->__pyx_n_s_text_embed);
   Py_CLEAR(clear_module_state->__pyx_kp_u_text_embedding_ada_002);
   Py_CLEAR(clear_module_state->__pyx_n_u_text_embeddings);
   Py_CLEAR(clear_module_state->__pyx_kp_u_text_embeddings_key_not_found_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_text_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_top_n);
   Py_CLEAR(clear_module_state->__pyx_n_s_top_results);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
-  Py_CLEAR(clear_module_state->__pyx_n_u_update);
-  Py_CLEAR(clear_module_state->__pyx_n_u_upsert);
   Py_CLEAR(clear_module_state->__pyx_n_s_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
   Py_CLEAR(clear_module_state->__pyx_n_s_vector_query);
   Py_CLEAR(clear_module_state->__pyx_n_s_vector_search);
   Py_CLEAR(clear_module_state->__pyx_n_s_vector_search_locals_lambda);
   Py_CLEAR(clear_module_state->__pyx_n_s_vectorizeEmbed);
   Py_CLEAR(clear_module_state->__pyx_n_s_vectorizeText);
+  Py_CLEAR(clear_module_state->__pyx_n_u_wildcard);
   Py_CLEAR(clear_module_state->__pyx_n_s_x);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decipherx);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Encapseal);
-  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_SaveToMongoDb);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___setstate_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_shorten_text);
-  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vector_search);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vectorizeEmbed);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vectorizeText);
   Py_CLEAR(clear_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
   Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_5);
   Py_CLEAR(clear_module_state->__pyx_int_200);
-  Py_CLEAR(clear_module_state->__pyx_int_1000);
   Py_CLEAR(clear_module_state->__pyx_int_222419149);
   Py_CLEAR(clear_module_state->__pyx_int_228825662);
   Py_CLEAR(clear_module_state->__pyx_int_238750788);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
-  Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__5);
   Py_CLEAR(clear_module_state->__pyx_tuple__7);
   Py_CLEAR(clear_module_state->__pyx_tuple__9);
   Py_CLEAR(clear_module_state->__pyx_tuple__11);
   Py_CLEAR(clear_module_state->__pyx_tuple__13);
   Py_CLEAR(clear_module_state->__pyx_tuple__15);
   Py_CLEAR(clear_module_state->__pyx_tuple__17);
   Py_CLEAR(clear_module_state->__pyx_tuple__19);
   Py_CLEAR(clear_module_state->__pyx_tuple__21);
-  Py_CLEAR(clear_module_state->__pyx_tuple__23);
-  Py_CLEAR(clear_module_state->__pyx_tuple__25);
-  Py_CLEAR(clear_module_state->__pyx_tuple__26);
-  Py_CLEAR(clear_module_state->__pyx_tuple__28);
-  Py_CLEAR(clear_module_state->__pyx_tuple__29);
-  Py_CLEAR(clear_module_state->__pyx_tuple__31);
-  Py_CLEAR(clear_module_state->__pyx_tuple__33);
+  Py_CLEAR(clear_module_state->__pyx_tuple__22);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__8);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
   Py_CLEAR(clear_module_state->__pyx_codeobj__12);
   Py_CLEAR(clear_module_state->__pyx_codeobj__14);
   Py_CLEAR(clear_module_state->__pyx_codeobj__16);
   Py_CLEAR(clear_module_state->__pyx_codeobj__18);
   Py_CLEAR(clear_module_state->__pyx_codeobj__20);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__22);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__27);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__30);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__32);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__34);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__23);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -3069,14 +3017,15 @@
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_8aixhello_6xyello_xyellw);
   Py_VISIT(traverse_module_state->__pyx_type_8aixhello_6xyello_xyellw);
+  Py_VISIT(traverse_module_state->__pyx_n_s_);
   Py_VISIT(traverse_module_state->__pyx_kp_u_);
   Py_VISIT(traverse_module_state->__pyx_n_s_AES);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Access_Control_Request_Headers);
   Py_VISIT(traverse_module_state->__pyx_kp_u_An_unexpected_error_occurred);
   Py_VISIT(traverse_module_state->__pyx_n_s_AuthenticationError);
   Py_VISIT(traverse_module_state->__pyx_n_s_CBC);
   Py_VISIT(traverse_module_state->__pyx_n_s_Cipher);
@@ -3085,61 +3034,50 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_Decipherx);
   Py_VISIT(traverse_module_state->__pyx_n_s_Encapseal);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_API_key_provided);
   Py_VISIT(traverse_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Request_failed_with_status_code);
-  Py_VISIT(traverse_module_state->__pyx_n_s_SaveToMongoDb);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Unknown_filename);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__10);
-  Py_VISIT(traverse_module_state->__pyx_n_s__35);
-  Py_VISIT(traverse_module_state->__pyx_n_s__6);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__6);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__8);
+  Py_VISIT(traverse_module_state->__pyx_n_s__24);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__4);
   Py_VISIT(traverse_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_VISIT(traverse_module_state->__pyx_n_s_aixhello_xyello);
   Py_VISIT(traverse_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithms);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_key);
   Py_VISIT(traverse_module_state->__pyx_kp_u_api_key_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_append);
   Py_VISIT(traverse_module_state->__pyx_kp_u_application_json);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_application_pdf);
   Py_VISIT(traverse_module_state->__pyx_n_s_array);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_b64decode);
   Py_VISIT(traverse_module_state->__pyx_n_s_b64encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_backend);
   Py_VISIT(traverse_module_state->__pyx_n_s_base64);
   Py_VISIT(traverse_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_chr);
   Py_VISIT(traverse_module_state->__pyx_n_s_chunk);
   Py_VISIT(traverse_module_state->__pyx_n_s_cipher);
   Py_VISIT(traverse_module_state->__pyx_n_s_cleaned_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
-  Py_VISIT(traverse_module_state->__pyx_n_s_collection);
   Py_VISIT(traverse_module_state->__pyx_n_u_collection);
   Py_VISIT(traverse_module_state->__pyx_n_s_connParam);
   Py_VISIT(traverse_module_state->__pyx_n_s_create);
   Py_VISIT(traverse_module_state->__pyx_n_s_cryptography_hazmat_backends);
   Py_VISIT(traverse_module_state->__pyx_n_s_cryptography_hazmat_primitives_c);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
   Py_VISIT(traverse_module_state->__pyx_n_u_dataSource);
-  Py_VISIT(traverse_module_state->__pyx_n_s_database);
   Py_VISIT(traverse_module_state->__pyx_n_u_database);
-  Py_VISIT(traverse_module_state->__pyx_n_s_datasource);
   Py_VISIT(traverse_module_state->__pyx_n_s_decode);
   Py_VISIT(traverse_module_state->__pyx_n_s_decoded_encryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_decryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_decrypted_padded_text);
-  Py_VISIT(traverse_module_state->__pyx_n_s_decrypted_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_decryptor);
   Py_VISIT(traverse_module_state->__pyx_n_s_default_backend);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict_2);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
   Py_VISIT(traverse_module_state->__pyx_n_s_doc);
   Py_VISIT(traverse_module_state->__pyx_n_s_documents);
@@ -3151,81 +3089,83 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_embedding);
   Py_VISIT(traverse_module_state->__pyx_n_s_embeddings);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_encoded_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptor);
-  Py_VISIT(traverse_module_state->__pyx_n_s_enkyc);
   Py_VISIT(traverse_module_state->__pyx_n_u_enkyc);
   Py_VISIT(traverse_module_state->__pyx_n_u_error);
   Py_VISIT(traverse_module_state->__pyx_n_u_extracted_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_extracted_text_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_extracted_texts);
-  Py_VISIT(traverse_module_state->__pyx_n_u_file_data);
-  Py_VISIT(traverse_module_state->__pyx_n_u_file_type);
   Py_VISIT(traverse_module_state->__pyx_n_u_filename);
   Py_VISIT(traverse_module_state->__pyx_n_s_filenames);
-  Py_VISIT(traverse_module_state->__pyx_n_u_filter);
   Py_VISIT(traverse_module_state->__pyx_n_s_finalize);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_get);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_headers);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_u_index);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
   Py_VISIT(traverse_module_state->__pyx_n_s_input);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_iv);
   Py_VISIT(traverse_module_state->__pyx_n_s_json);
   Py_VISIT(traverse_module_state->__pyx_n_s_key);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_limit);
   Py_VISIT(traverse_module_state->__pyx_n_s_linalg);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_max_length);
   Py_VISIT(traverse_module_state->__pyx_n_u_message);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_meta);
   Py_VISIT(traverse_module_state->__pyx_n_s_model);
   Py_VISIT(traverse_module_state->__pyx_n_s_modes);
   Py_VISIT(traverse_module_state->__pyx_n_s_msg);
   Py_VISIT(traverse_module_state->__pyx_n_s_mth);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_n_s_norm);
   Py_VISIT(traverse_module_state->__pyx_n_s_np);
   Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
   Py_VISIT(traverse_module_state->__pyx_n_s_openai);
   Py_VISIT(traverse_module_state->__pyx_n_s_pad_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_padded_text);
-  Py_VISIT(traverse_module_state->__pyx_n_s_params_dict);
-  Py_VISIT(traverse_module_state->__pyx_n_s_payload);
+  Py_VISIT(traverse_module_state->__pyx_n_u_path);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
   Py_VISIT(traverse_module_state->__pyx_n_s_pipeline);
   Py_VISIT(traverse_module_state->__pyx_n_u_pipeline);
   Py_VISIT(traverse_module_state->__pyx_n_s_post);
   Py_VISIT(traverse_module_state->__pyx_n_s_print);
   Py_VISIT(traverse_module_state->__pyx_kp_u_project);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_xyellw);
+  Py_VISIT(traverse_module_state->__pyx_n_u_query);
   Py_VISIT(traverse_module_state->__pyx_n_s_query_payload);
   Py_VISIT(traverse_module_state->__pyx_n_s_query_vec);
   Py_VISIT(traverse_module_state->__pyx_n_s_re);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_requests);
   Py_VISIT(traverse_module_state->__pyx_n_s_response);
   Py_VISIT(traverse_module_state->__pyx_n_s_response_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_reverse);
+  Py_VISIT(traverse_module_state->__pyx_n_u_score);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_search);
+  Py_VISIT(traverse_module_state->__pyx_n_u_searchScore);
+  Py_VISIT(traverse_module_state->__pyx_n_u_searchindex);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_set);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_shorten_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_similar_score);
   Py_VISIT(traverse_module_state->__pyx_n_s_similarities);
   Py_VISIT(traverse_module_state->__pyx_n_s_similarities_values);
   Py_VISIT(traverse_module_state->__pyx_n_u_similarity);
@@ -3233,83 +3173,70 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_status_code);
   Py_VISIT(traverse_module_state->__pyx_n_s_strText);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_text);
+  Py_VISIT(traverse_module_state->__pyx_n_u_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_text_chunks);
   Py_VISIT(traverse_module_state->__pyx_n_s_text_embed);
   Py_VISIT(traverse_module_state->__pyx_kp_u_text_embedding_ada_002);
   Py_VISIT(traverse_module_state->__pyx_n_u_text_embeddings);
   Py_VISIT(traverse_module_state->__pyx_kp_u_text_embeddings_key_not_found_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_text_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_top_n);
   Py_VISIT(traverse_module_state->__pyx_n_s_top_results);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
-  Py_VISIT(traverse_module_state->__pyx_n_u_update);
-  Py_VISIT(traverse_module_state->__pyx_n_u_upsert);
   Py_VISIT(traverse_module_state->__pyx_n_s_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
   Py_VISIT(traverse_module_state->__pyx_n_s_vector_query);
   Py_VISIT(traverse_module_state->__pyx_n_s_vector_search);
   Py_VISIT(traverse_module_state->__pyx_n_s_vector_search_locals_lambda);
   Py_VISIT(traverse_module_state->__pyx_n_s_vectorizeEmbed);
   Py_VISIT(traverse_module_state->__pyx_n_s_vectorizeText);
+  Py_VISIT(traverse_module_state->__pyx_n_u_wildcard);
   Py_VISIT(traverse_module_state->__pyx_n_s_x);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decipherx);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Encapseal);
-  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_SaveToMongoDb);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___setstate_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_shorten_text);
-  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vector_search);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vectorizeEmbed);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vectorizeText);
   Py_VISIT(traverse_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
   Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_5);
   Py_VISIT(traverse_module_state->__pyx_int_200);
-  Py_VISIT(traverse_module_state->__pyx_int_1000);
   Py_VISIT(traverse_module_state->__pyx_int_222419149);
   Py_VISIT(traverse_module_state->__pyx_int_228825662);
   Py_VISIT(traverse_module_state->__pyx_int_238750788);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
-  Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__5);
   Py_VISIT(traverse_module_state->__pyx_tuple__7);
   Py_VISIT(traverse_module_state->__pyx_tuple__9);
   Py_VISIT(traverse_module_state->__pyx_tuple__11);
   Py_VISIT(traverse_module_state->__pyx_tuple__13);
   Py_VISIT(traverse_module_state->__pyx_tuple__15);
   Py_VISIT(traverse_module_state->__pyx_tuple__17);
   Py_VISIT(traverse_module_state->__pyx_tuple__19);
   Py_VISIT(traverse_module_state->__pyx_tuple__21);
-  Py_VISIT(traverse_module_state->__pyx_tuple__23);
-  Py_VISIT(traverse_module_state->__pyx_tuple__25);
-  Py_VISIT(traverse_module_state->__pyx_tuple__26);
-  Py_VISIT(traverse_module_state->__pyx_tuple__28);
-  Py_VISIT(traverse_module_state->__pyx_tuple__29);
-  Py_VISIT(traverse_module_state->__pyx_tuple__31);
-  Py_VISIT(traverse_module_state->__pyx_tuple__33);
+  Py_VISIT(traverse_module_state->__pyx_tuple__22);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__8);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
   Py_VISIT(traverse_module_state->__pyx_codeobj__12);
   Py_VISIT(traverse_module_state->__pyx_codeobj__14);
   Py_VISIT(traverse_module_state->__pyx_codeobj__16);
   Py_VISIT(traverse_module_state->__pyx_codeobj__18);
   Py_VISIT(traverse_module_state->__pyx_codeobj__20);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__22);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__27);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__30);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__32);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__34);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__23);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3334,14 +3261,15 @@
 #ifdef __Pyx_Coroutine_USED
 #define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
 #endif
 #if CYTHON_USE_MODULE_STATE
 #define __pyx_type_8aixhello_6xyello_xyellw __pyx_mstate_global->__pyx_type_8aixhello_6xyello_xyellw
 #endif
 #define __pyx_ptype_8aixhello_6xyello_xyellw __pyx_mstate_global->__pyx_ptype_8aixhello_6xyello_xyellw
+#define __pyx_n_s_ __pyx_mstate_global->__pyx_n_s_
 #define __pyx_kp_u_ __pyx_mstate_global->__pyx_kp_u_
 #define __pyx_n_s_AES __pyx_mstate_global->__pyx_n_s_AES
 #define __pyx_kp_u_Access_Control_Request_Headers __pyx_mstate_global->__pyx_kp_u_Access_Control_Request_Headers
 #define __pyx_kp_u_An_unexpected_error_occurred __pyx_mstate_global->__pyx_kp_u_An_unexpected_error_occurred
 #define __pyx_n_s_AuthenticationError __pyx_mstate_global->__pyx_n_s_AuthenticationError
 #define __pyx_n_s_CBC __pyx_mstate_global->__pyx_n_s_CBC
 #define __pyx_n_s_Cipher __pyx_mstate_global->__pyx_n_s_Cipher
@@ -3350,61 +3278,50 @@
 #define __pyx_n_s_Decipherx __pyx_mstate_global->__pyx_n_s_Decipherx
 #define __pyx_n_s_Encapseal __pyx_mstate_global->__pyx_n_s_Encapseal
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_kp_u_Invalid_API_key_provided __pyx_mstate_global->__pyx_kp_u_Invalid_API_key_provided
 #define __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN __pyx_mstate_global->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_kp_u_Request_failed_with_status_code __pyx_mstate_global->__pyx_kp_u_Request_failed_with_status_code
-#define __pyx_n_s_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_SaveToMongoDb
-#define __pyx_kp_u_Successfully_save_to_the_databas __pyx_mstate_global->__pyx_kp_u_Successfully_save_to_the_databas
 #define __pyx_kp_u_Unknown_filename __pyx_mstate_global->__pyx_kp_u_Unknown_filename
-#define __pyx_kp_u__10 __pyx_mstate_global->__pyx_kp_u__10
-#define __pyx_n_s__35 __pyx_mstate_global->__pyx_n_s__35
-#define __pyx_n_s__6 __pyx_mstate_global->__pyx_n_s__6
-#define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
-#define __pyx_kp_u__8 __pyx_mstate_global->__pyx_kp_u__8
+#define __pyx_n_s__24 __pyx_mstate_global->__pyx_n_s__24
+#define __pyx_kp_u__4 __pyx_mstate_global->__pyx_kp_u__4
 #define __pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1 __pyx_mstate_global->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1
 #define __pyx_n_s_aixhello_xyello __pyx_mstate_global->__pyx_n_s_aixhello_xyello
 #define __pyx_kp_s_aixhello_xyello_pyx __pyx_mstate_global->__pyx_kp_s_aixhello_xyello_pyx
 #define __pyx_n_s_algorithms __pyx_mstate_global->__pyx_n_s_algorithms
 #define __pyx_n_s_api_key __pyx_mstate_global->__pyx_n_s_api_key
 #define __pyx_kp_u_api_key_2 __pyx_mstate_global->__pyx_kp_u_api_key_2
 #define __pyx_n_s_api_url __pyx_mstate_global->__pyx_n_s_api_url
 #define __pyx_n_s_append __pyx_mstate_global->__pyx_n_s_append
 #define __pyx_kp_u_application_json __pyx_mstate_global->__pyx_kp_u_application_json
-#define __pyx_kp_u_application_pdf __pyx_mstate_global->__pyx_kp_u_application_pdf
 #define __pyx_n_s_array __pyx_mstate_global->__pyx_n_s_array
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_b64decode __pyx_mstate_global->__pyx_n_s_b64decode
 #define __pyx_n_s_b64encode __pyx_mstate_global->__pyx_n_s_b64encode
 #define __pyx_n_s_backend __pyx_mstate_global->__pyx_n_s_backend
 #define __pyx_n_s_base64 __pyx_mstate_global->__pyx_n_s_base64
 #define __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn __pyx_mstate_global->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn
-#define __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2 __pyx_mstate_global->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2
 #define __pyx_n_s_chr __pyx_mstate_global->__pyx_n_s_chr
 #define __pyx_n_s_chunk __pyx_mstate_global->__pyx_n_s_chunk
 #define __pyx_n_s_cipher __pyx_mstate_global->__pyx_n_s_cipher
 #define __pyx_n_s_cleaned_text __pyx_mstate_global->__pyx_n_s_cleaned_text
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
-#define __pyx_n_s_collection __pyx_mstate_global->__pyx_n_s_collection
 #define __pyx_n_u_collection __pyx_mstate_global->__pyx_n_u_collection
 #define __pyx_n_s_connParam __pyx_mstate_global->__pyx_n_s_connParam
 #define __pyx_n_s_create __pyx_mstate_global->__pyx_n_s_create
 #define __pyx_n_s_cryptography_hazmat_backends __pyx_mstate_global->__pyx_n_s_cryptography_hazmat_backends
 #define __pyx_n_s_cryptography_hazmat_primitives_c __pyx_mstate_global->__pyx_n_s_cryptography_hazmat_primitives_c
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
 #define __pyx_n_u_dataSource __pyx_mstate_global->__pyx_n_u_dataSource
-#define __pyx_n_s_database __pyx_mstate_global->__pyx_n_s_database
 #define __pyx_n_u_database __pyx_mstate_global->__pyx_n_u_database
-#define __pyx_n_s_datasource __pyx_mstate_global->__pyx_n_s_datasource
 #define __pyx_n_s_decode __pyx_mstate_global->__pyx_n_s_decode
 #define __pyx_n_s_decoded_encryptedText __pyx_mstate_global->__pyx_n_s_decoded_encryptedText
 #define __pyx_n_s_decryptedText __pyx_mstate_global->__pyx_n_s_decryptedText
 #define __pyx_n_s_decrypted_padded_text __pyx_mstate_global->__pyx_n_s_decrypted_padded_text
-#define __pyx_n_s_decrypted_url __pyx_mstate_global->__pyx_n_s_decrypted_url
 #define __pyx_n_s_decryptor __pyx_mstate_global->__pyx_n_s_decryptor
 #define __pyx_n_s_default_backend __pyx_mstate_global->__pyx_n_s_default_backend
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_dict_2 __pyx_mstate_global->__pyx_n_s_dict_2
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
 #define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
 #define __pyx_n_s_documents __pyx_mstate_global->__pyx_n_s_documents
@@ -3416,81 +3333,83 @@
 #define __pyx_n_s_embedding __pyx_mstate_global->__pyx_n_s_embedding
 #define __pyx_n_s_embeddings __pyx_mstate_global->__pyx_n_s_embeddings
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_encoded_url __pyx_mstate_global->__pyx_n_s_encoded_url
 #define __pyx_n_s_encryptedText __pyx_mstate_global->__pyx_n_s_encryptedText
 #define __pyx_n_s_encryptor __pyx_mstate_global->__pyx_n_s_encryptor
-#define __pyx_n_s_enkyc __pyx_mstate_global->__pyx_n_s_enkyc
 #define __pyx_n_u_enkyc __pyx_mstate_global->__pyx_n_u_enkyc
 #define __pyx_n_u_error __pyx_mstate_global->__pyx_n_u_error
 #define __pyx_n_u_extracted_text __pyx_mstate_global->__pyx_n_u_extracted_text
 #define __pyx_n_s_extracted_text_length __pyx_mstate_global->__pyx_n_s_extracted_text_length
 #define __pyx_n_s_extracted_texts __pyx_mstate_global->__pyx_n_s_extracted_texts
-#define __pyx_n_u_file_data __pyx_mstate_global->__pyx_n_u_file_data
-#define __pyx_n_u_file_type __pyx_mstate_global->__pyx_n_u_file_type
 #define __pyx_n_u_filename __pyx_mstate_global->__pyx_n_u_filename
 #define __pyx_n_s_filenames __pyx_mstate_global->__pyx_n_s_filenames
-#define __pyx_n_u_filter __pyx_mstate_global->__pyx_n_u_filter
 #define __pyx_n_s_finalize __pyx_mstate_global->__pyx_n_s_finalize
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_get __pyx_mstate_global->__pyx_n_s_get
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_n_s_headers __pyx_mstate_global->__pyx_n_s_headers
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_u_index __pyx_mstate_global->__pyx_n_u_index
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
 #define __pyx_n_s_input __pyx_mstate_global->__pyx_n_s_input
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_iv __pyx_mstate_global->__pyx_n_s_iv
 #define __pyx_n_s_json __pyx_mstate_global->__pyx_n_s_json
 #define __pyx_n_s_key __pyx_mstate_global->__pyx_n_s_key
+#define __pyx_kp_u_limit __pyx_mstate_global->__pyx_kp_u_limit
 #define __pyx_n_s_linalg __pyx_mstate_global->__pyx_n_s_linalg
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_max_length __pyx_mstate_global->__pyx_n_s_max_length
 #define __pyx_n_u_message __pyx_mstate_global->__pyx_n_u_message
+#define __pyx_kp_u_meta __pyx_mstate_global->__pyx_kp_u_meta
 #define __pyx_n_s_model __pyx_mstate_global->__pyx_n_s_model
 #define __pyx_n_s_modes __pyx_mstate_global->__pyx_n_s_modes
 #define __pyx_n_s_msg __pyx_mstate_global->__pyx_n_s_msg
 #define __pyx_n_s_mth __pyx_mstate_global->__pyx_n_s_mth
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_n_s_norm __pyx_mstate_global->__pyx_n_s_norm
 #define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
 #define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
 #define __pyx_n_s_openai __pyx_mstate_global->__pyx_n_s_openai
 #define __pyx_n_s_pad_length __pyx_mstate_global->__pyx_n_s_pad_length
 #define __pyx_n_s_padded_text __pyx_mstate_global->__pyx_n_s_padded_text
-#define __pyx_n_s_params_dict __pyx_mstate_global->__pyx_n_s_params_dict
-#define __pyx_n_s_payload __pyx_mstate_global->__pyx_n_s_payload
+#define __pyx_n_u_path __pyx_mstate_global->__pyx_n_u_path
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
 #define __pyx_n_s_pipeline __pyx_mstate_global->__pyx_n_s_pipeline
 #define __pyx_n_u_pipeline __pyx_mstate_global->__pyx_n_u_pipeline
 #define __pyx_n_s_post __pyx_mstate_global->__pyx_n_s_post
 #define __pyx_n_s_print __pyx_mstate_global->__pyx_n_s_print
 #define __pyx_kp_u_project __pyx_mstate_global->__pyx_kp_u_project
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
 #define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
 #define __pyx_n_s_pyx_unpickle_xyellw __pyx_mstate_global->__pyx_n_s_pyx_unpickle_xyellw
+#define __pyx_n_u_query __pyx_mstate_global->__pyx_n_u_query
 #define __pyx_n_s_query_payload __pyx_mstate_global->__pyx_n_s_query_payload
 #define __pyx_n_s_query_vec __pyx_mstate_global->__pyx_n_s_query_vec
 #define __pyx_n_s_re __pyx_mstate_global->__pyx_n_s_re
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_requests __pyx_mstate_global->__pyx_n_s_requests
 #define __pyx_n_s_response __pyx_mstate_global->__pyx_n_s_response
 #define __pyx_n_s_response_data __pyx_mstate_global->__pyx_n_s_response_data
 #define __pyx_n_s_result __pyx_mstate_global->__pyx_n_s_result
 #define __pyx_n_s_reverse __pyx_mstate_global->__pyx_n_s_reverse
+#define __pyx_n_u_score __pyx_mstate_global->__pyx_n_u_score
+#define __pyx_kp_u_search __pyx_mstate_global->__pyx_kp_u_search
+#define __pyx_n_u_searchScore __pyx_mstate_global->__pyx_n_u_searchScore
+#define __pyx_n_u_searchindex __pyx_mstate_global->__pyx_n_u_searchindex
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
-#define __pyx_kp_u_set __pyx_mstate_global->__pyx_kp_u_set
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_shorten_text __pyx_mstate_global->__pyx_n_s_shorten_text
 #define __pyx_n_s_similar_score __pyx_mstate_global->__pyx_n_s_similar_score
 #define __pyx_n_s_similarities __pyx_mstate_global->__pyx_n_s_similarities
 #define __pyx_n_s_similarities_values __pyx_mstate_global->__pyx_n_s_similarities_values
 #define __pyx_n_u_similarity __pyx_mstate_global->__pyx_n_u_similarity
@@ -3498,83 +3417,70 @@
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_state __pyx_mstate_global->__pyx_n_s_state
 #define __pyx_n_s_status_code __pyx_mstate_global->__pyx_n_s_status_code
 #define __pyx_n_s_strText __pyx_mstate_global->__pyx_n_s_strText
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_text __pyx_mstate_global->__pyx_n_s_text
+#define __pyx_n_u_text __pyx_mstate_global->__pyx_n_u_text
 #define __pyx_n_s_text_chunks __pyx_mstate_global->__pyx_n_s_text_chunks
 #define __pyx_n_s_text_embed __pyx_mstate_global->__pyx_n_s_text_embed
 #define __pyx_kp_u_text_embedding_ada_002 __pyx_mstate_global->__pyx_kp_u_text_embedding_ada_002
 #define __pyx_n_u_text_embeddings __pyx_mstate_global->__pyx_n_u_text_embeddings
 #define __pyx_kp_u_text_embeddings_key_not_found_i __pyx_mstate_global->__pyx_kp_u_text_embeddings_key_not_found_i
 #define __pyx_n_s_text_key __pyx_mstate_global->__pyx_n_s_text_key
 #define __pyx_n_s_top_n __pyx_mstate_global->__pyx_n_s_top_n
 #define __pyx_n_s_top_results __pyx_mstate_global->__pyx_n_s_top_results
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
-#define __pyx_n_u_update __pyx_mstate_global->__pyx_n_u_update
-#define __pyx_n_u_upsert __pyx_mstate_global->__pyx_n_u_upsert
 #define __pyx_n_s_url __pyx_mstate_global->__pyx_n_s_url
 #define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_n_s_vector_query __pyx_mstate_global->__pyx_n_s_vector_query
 #define __pyx_n_s_vector_search __pyx_mstate_global->__pyx_n_s_vector_search
 #define __pyx_n_s_vector_search_locals_lambda __pyx_mstate_global->__pyx_n_s_vector_search_locals_lambda
 #define __pyx_n_s_vectorizeEmbed __pyx_mstate_global->__pyx_n_s_vectorizeEmbed
 #define __pyx_n_s_vectorizeText __pyx_mstate_global->__pyx_n_s_vectorizeText
+#define __pyx_n_u_wildcard __pyx_mstate_global->__pyx_n_u_wildcard
 #define __pyx_n_s_x __pyx_mstate_global->__pyx_n_s_x
 #define __pyx_n_s_xyellw __pyx_mstate_global->__pyx_n_s_xyellw
 #define __pyx_n_s_xyellw_Decenigma __pyx_mstate_global->__pyx_n_s_xyellw_Decenigma
 #define __pyx_n_s_xyellw_Decipherx __pyx_mstate_global->__pyx_n_s_xyellw_Decipherx
 #define __pyx_n_s_xyellw_Encapseal __pyx_mstate_global->__pyx_n_s_xyellw_Encapseal
-#define __pyx_n_s_xyellw_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_xyellw_SaveToMongoDb
 #define __pyx_n_s_xyellw___reduce_cython __pyx_mstate_global->__pyx_n_s_xyellw___reduce_cython
 #define __pyx_n_s_xyellw___setstate_cython __pyx_mstate_global->__pyx_n_s_xyellw___setstate_cython
-#define __pyx_n_s_xyellw_shorten_text __pyx_mstate_global->__pyx_n_s_xyellw_shorten_text
-#define __pyx_n_s_xyellw_vector_search __pyx_mstate_global->__pyx_n_s_xyellw_vector_search
 #define __pyx_n_s_xyellw_vectorizeEmbed __pyx_mstate_global->__pyx_n_s_xyellw_vectorizeEmbed
 #define __pyx_n_s_xyellw_vectorizeText __pyx_mstate_global->__pyx_n_s_xyellw_vectorizeText
 #define __pyx_kp_b_y1c8_8BxP9XN_VKM __pyx_mstate_global->__pyx_kp_b_y1c8_8BxP9XN_VKM
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_5 __pyx_mstate_global->__pyx_int_5
 #define __pyx_int_200 __pyx_mstate_global->__pyx_int_200
-#define __pyx_int_1000 __pyx_mstate_global->__pyx_int_1000
 #define __pyx_int_222419149 __pyx_mstate_global->__pyx_int_222419149
 #define __pyx_int_228825662 __pyx_mstate_global->__pyx_int_228825662
 #define __pyx_int_238750788 __pyx_mstate_global->__pyx_int_238750788
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
-#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
 #define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
 #define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
 #define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
 #define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
 #define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
-#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
-#define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
-#define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
-#define __pyx_tuple__28 __pyx_mstate_global->__pyx_tuple__28
-#define __pyx_tuple__29 __pyx_mstate_global->__pyx_tuple__29
-#define __pyx_tuple__31 __pyx_mstate_global->__pyx_tuple__31
-#define __pyx_tuple__33 __pyx_mstate_global->__pyx_tuple__33
+#define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
+#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
+#define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
+#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
 #define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
 #define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
 #define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
 #define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
 #define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
-#define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
-#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
-#define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
-#define __pyx_codeobj__30 __pyx_mstate_global->__pyx_codeobj__30
-#define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
-#define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
+#define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
 /* #### Code section: module_code ### */
 
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -5541,392 +5447,330 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_11SaveToMongoDb = {"SaveToMongoDb", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_11__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
-  PyObject *__pyx_v_collection = 0;
-  PyObject *__pyx_v_database = 0;
-  PyObject *__pyx_v_datasource = 0;
-  PyObject *__pyx_v_enkyc = 0;
-  PyObject *__pyx_v_params_dict = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[5] = {0,0,0,0,0};
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_10__reduce_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self) {
+  PyObject *__pyx_v_state = 0;
+  PyObject *__pyx_v__dict = 0;
+  int __pyx_v_use_setstate;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
+
+  __Pyx_INCREF(__pyx_empty_tuple);
+  __pyx_v_state = __pyx_empty_tuple;
+
+  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v__dict = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  __pyx_t_2 = (__pyx_v__dict != Py_None);
+  if (__pyx_t_2) {
+
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_v__dict);
+    __Pyx_GIVEREF(__pyx_v__dict);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict)) __PYX_ERR(1, 8, __pyx_L1_error);
+    __pyx_t_3 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_3));
+    __pyx_t_3 = 0;
+
+    __pyx_v_use_setstate = 1;
+
+    goto __pyx_L3;
+  }
+
+  /*else*/ {
+    __pyx_v_use_setstate = 0;
+  }
+  __pyx_L3:;
+
+  if (__pyx_v_use_setstate) {
+
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pyx_unpickle_xyellw); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))))) __PYX_ERR(1, 13, __pyx_L1_error);
+    __Pyx_INCREF(__pyx_int_238750788);
+    __Pyx_GIVEREF(__pyx_int_238750788);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_238750788)) __PYX_ERR(1, 13, __pyx_L1_error);
+    __Pyx_INCREF(Py_None);
+    __Pyx_GIVEREF(Py_None);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None)) __PYX_ERR(1, 13, __pyx_L1_error);
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(1, 13, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_1);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_v_state)) __PYX_ERR(1, 13, __pyx_L1_error);
+    __pyx_t_3 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_4;
+    __pyx_t_4 = 0;
+    goto __pyx_L0;
+
+  }
+
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_xyellw); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))))) __PYX_ERR(1, 15, __pyx_L1_error);
+    __Pyx_INCREF(__pyx_int_238750788);
+    __Pyx_GIVEREF(__pyx_int_238750788);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_238750788)) __PYX_ERR(1, 15, __pyx_L1_error);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state)) __PYX_ERR(1, 15, __pyx_L1_error);
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_4);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_1);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error);
+    __pyx_t_4 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_3;
+    __pyx_t_3 = 0;
+    goto __pyx_L0;
+  }
+
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_state);
+  __Pyx_XDECREF(__pyx_v__dict);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_13__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v___pyx_state = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("SaveToMongoDb (wrapper)", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_collection,&__pyx_n_s_database,&__pyx_n_s_datasource,&__pyx_n_s_enkyc,&__pyx_n_s_params_dict,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
-        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
-        CYTHON_FALLTHROUGH;
-        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
-        CYTHON_FALLTHROUGH;
-        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_collection)) != 0)) {
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 16, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_database)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 1); __PYX_ERR(0, 81, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_datasource)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 2); __PYX_ERR(0, 81, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  3:
-        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_enkyc)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 3); __PYX_ERR(0, 81, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  4:
-        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_params_dict)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 4); __PYX_ERR(0, 81, __pyx_L3_error)
-        }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "SaveToMongoDb") < 0)) __PYX_ERR(0, 81, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 16, __pyx_L3_error)
       }
-    } else if (unlikely(__pyx_nargs != 5)) {
+    } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-      values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
-      values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
     }
-    __pyx_v_collection = ((PyObject*)values[0]);
-    __pyx_v_database = ((PyObject*)values[1]);
-    __pyx_v_datasource = ((PyObject*)values[2]);
-    __pyx_v_enkyc = ((PyObject*)values[3]);
-    __pyx_v_params_dict = values[4];
+    __pyx_v___pyx_state = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 81, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 16, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.SaveToMongoDb", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_collection), (&PyUnicode_Type), 1, "collection", 1))) __PYX_ERR(0, 81, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_database), (&PyUnicode_Type), 1, "database", 1))) __PYX_ERR(0, 81, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_datasource), (&PyUnicode_Type), 1, "datasource", 1))) __PYX_ERR(0, 81, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_enkyc), (&PyUnicode_Type), 1, "enkyc", 1))) __PYX_ERR(0, 81, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_collection, __pyx_v_database, __pyx_v_datasource, __pyx_v_enkyc, __pyx_v_params_dict);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_12__setstate_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict) {
-  PyObject *__pyx_v_decrypted_url = NULL;
-  PyObject *__pyx_v_payload = NULL;
-  PyObject *__pyx_v_headers = NULL;
-  PyObject *__pyx_v_response = NULL;
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("SaveToMongoDb", 1);
-
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
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
-  {
-    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  }
-  __pyx_v_decrypted_url = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_collection, __pyx_v_collection) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_database, __pyx_v_database) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_dataSource, __pyx_v_datasource) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_filename, __pyx_t_5) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filter, __pyx_t_2) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_filename, __pyx_t_6) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_data, __pyx_t_3) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_type, __pyx_kp_u_application_pdf) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
-
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_extracted_text, __pyx_t_6) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_text_embeddings, __pyx_t_3) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_set, __pyx_t_5) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_update, __pyx_t_2) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_upsert, Py_True) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-  __pyx_v_payload = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
-
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__6) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
-
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_v_enkyc) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
-  __pyx_v_headers = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_requests); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8aixhello_6xyello___pyx_unpickle_xyellw__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_v_decrypted_url);
-  __Pyx_GIVEREF(__pyx_v_decrypted_url);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_decrypted_url)) __PYX_ERR(0, 106, __pyx_L1_error);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_json, __pyx_v_payload) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_response = __pyx_t_3;
-  __pyx_t_3 = 0;
-
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_3, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 108, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__pyx_t_7) {
-
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_kp_u_Successfully_save_to_the_databas);
-    __pyx_r = __pyx_kp_u_Successfully_save_to_the_databas;
-    goto __pyx_L0;
-
-  }
-
-  /*else*/ {
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 111, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 111, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_error, __pyx_t_5) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_r = __pyx_t_3;
-    __pyx_t_3 = 0;
-    goto __pyx_L0;
-  }
 
 
   /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.SaveToMongoDb", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_decrypted_url);
-  __Pyx_XDECREF(__pyx_v_payload);
-  __Pyx_XDECREF(__pyx_v_headers);
-  __Pyx_XDECREF(__pyx_v_response);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_1vector_search(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_13vector_search = {"vector_search", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_1vector_search = {"vector_search", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_1vector_search, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_1vector_search(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
+  PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_connParam = 0;
   PyObject *__pyx_v_extracted_text_length = 0;
   PyObject *__pyx_v_vector_query = 0;
   PyObject *__pyx_v_top_n = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[4] = {0,0,0,0};
+  PyObject* values[5] = {0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("vector_search (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
@@ -5934,127 +5778,141 @@
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_connParam,&__pyx_n_s_extracted_text_length,&__pyx_n_s_vector_query,&__pyx_n_s_top_n,0};
-    values[3] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)__pyx_int_5));
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_connParam,&__pyx_n_s_extracted_text_length,&__pyx_n_s_vector_query,&__pyx_n_s_top_n,0};
+    values[4] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)__pyx_int_5)));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_connParam)) != 0)) {
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_extracted_text_length)) != 0)) {
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_connParam)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("vector_search", 0, 3, 4, 1); __PYX_ERR(0, 114, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vector_search", 0, 4, 5, 1); __PYX_ERR(0, 81, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vector_query)) != 0)) {
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_extracted_text_length)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("vector_search", 0, 3, 4, 2); __PYX_ERR(0, 114, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vector_search", 0, 4, 5, 2); __PYX_ERR(0, 81, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vector_query)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("vector_search", 0, 4, 5, 3); __PYX_ERR(0, 81, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_top_n);
-          if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
+          if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vector_search") < 0)) __PYX_ERR(0, 114, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vector_search") < 0)) __PYX_ERR(0, 81, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
-        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_connParam = values[0];
-    __pyx_v_extracted_text_length = values[1];
-    __pyx_v_vector_query = values[2];
-    __pyx_v_top_n = values[3];
+    __pyx_v_self = values[0];
+    __pyx_v_connParam = values[1];
+    __pyx_v_extracted_text_length = values[2];
+    __pyx_v_vector_query = values[3];
+    __pyx_v_top_n = values[4];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("vector_search", 0, 3, 4, __pyx_nargs); __PYX_ERR(0, 114, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("vector_search", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 81, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.vector_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_connParam, __pyx_v_extracted_text_length, __pyx_v_vector_query, __pyx_v_top_n);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_vector_search(__pyx_self, __pyx_v_self, __pyx_v_connParam, __pyx_v_extracted_text_length, __pyx_v_vector_query, __pyx_v_top_n);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search_lambda(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_13vector_search_lambda(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_13vector_search_lambda = {"lambda", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search_lambda, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search_lambda(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_13vector_search_lambda = {"lambda", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_13vector_search_lambda, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_13vector_search_lambda(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_x = 0;
@@ -6090,41 +5948,41 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 168, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 150, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda") < 0)) __PYX_ERR(0, 168, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda") < 0)) __PYX_ERR(0, 150, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_x = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lambda", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 168, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("lambda", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 150, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.vector_search.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_lambda_funcdef_lambda(__pyx_self, __pyx_v_x);
 
   /* function exit code */
   {
@@ -6142,33 +6000,33 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_x, __pyx_n_u_similarity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_x, __pyx_n_u_similarity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.vector_search.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, PyObject *__pyx_v_vector_query, PyObject *__pyx_v_top_n) {
+static PyObject *__pyx_pf_8aixhello_6xyello_vector_search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, PyObject *__pyx_v_vector_query, PyObject *__pyx_v_top_n) {
   PyObject *__pyx_v_url = NULL;
   PyObject *__pyx_v_headers = NULL;
   PyObject *__pyx_v_pipeline = NULL;
   PyObject *__pyx_v_query_payload = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_similarities = NULL;
   PyObject *__pyx_v_response_data = NULL;
@@ -6204,15 +6062,15 @@
   PyObject *__pyx_t_13 = NULL;
   int __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("vector_search", 1);
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -6221,352 +6079,392 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #endif
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2};
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_url = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__6) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u_) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
 
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_enkyc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_enkyc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_t_2) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_t_2) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_headers = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_filename, __pyx_int_1) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_extracted_text, __pyx_int_1) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_text_embeddings, __pyx_int_1) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_project, __pyx_t_2) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_searchindex); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_index, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_query, __pyx_v_vector_query) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
+
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_wildcard, __pyx_kp_u_) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_path, __pyx_t_5) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_text, __pyx_t_3) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_search, __pyx_t_2) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error);
-  __pyx_t_1 = 0;
-  __pyx_v_pipeline = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_dataSource); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_dataSource, __pyx_t_1) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_filename, __pyx_int_1) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_extracted_text, __pyx_int_1) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_text_embeddings, __pyx_int_1) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
 
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_database); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_database, __pyx_t_1) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_meta, __pyx_n_u_searchScore) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_score, __pyx_t_5) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_project, __pyx_t_3) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_collection); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_collection, __pyx_t_1) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_limit, __pyx_v_top_n) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
 
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_pipeline, __pyx_v_pipeline) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
-  __pyx_v_query_payload = ((PyObject*)__pyx_t_2);
+  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_2);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 2, __pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error);
+  __pyx_t_1 = 0;
   __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+  __pyx_v_pipeline = ((PyObject*)__pyx_t_5);
+  __pyx_t_5 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_requests); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_post); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_v_url);
-  __Pyx_GIVEREF(__pyx_v_url);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_url)) __PYX_ERR(0, 142, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_json, __pyx_v_query_payload) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_dataSource); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_dataSource, __pyx_t_3) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_response = __pyx_t_5;
-  __pyx_t_5 = 0;
 
-  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 144, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_v_similarities = __pyx_t_5;
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_database); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_database, __pyx_t_3) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_collection); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_collection, __pyx_t_3) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_pipeline, __pyx_v_pipeline) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_v_query_payload = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_requests); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_post); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_5, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 146, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_v_url);
+  __Pyx_GIVEREF(__pyx_v_url);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_url)) __PYX_ERR(0, 124, __pyx_L1_error);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 124, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_json, __pyx_v_query_payload) < 0) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_response = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_similarities = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_6 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_1, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_6) {
 
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = NULL;
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_5 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_2);
+    if (likely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_4 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
-      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 147, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __pyx_v_response_data = __pyx_t_5;
-    __pyx_t_5 = 0;
+    __pyx_v_response_data = __pyx_t_1;
+    __pyx_t_1 = 0;
 
-    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_response_data, __pyx_n_u_documents); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_v_documents = __pyx_t_5;
-    __pyx_t_5 = 0;
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_response_data, __pyx_n_u_documents); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_v_documents = __pyx_t_1;
+    __pyx_t_1 = 0;
 
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = NULL;
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 132, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_3);
+    if (unlikely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_2)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
         __pyx_t_4 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_vector_query};
-      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_vector_query};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __pyx_v_query_vec = __pyx_t_5;
-    __pyx_t_5 = 0;
+    __pyx_v_query_vec = __pyx_t_1;
+    __pyx_t_1 = 0;
 
     if (likely(PyList_CheckExact(__pyx_v_documents)) || PyTuple_CheckExact(__pyx_v_documents)) {
-      __pyx_t_5 = __pyx_v_documents; __Pyx_INCREF(__pyx_t_5);
+      __pyx_t_1 = __pyx_v_documents; __Pyx_INCREF(__pyx_t_1);
       __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_documents); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 152, __pyx_L1_error)
+      __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_documents); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 134, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_8)) {
-        if (likely(PyList_CheckExact(__pyx_t_5))) {
+        if (likely(PyList_CheckExact(__pyx_t_1))) {
           {
-            Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
+            Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 152, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 134, __pyx_L1_error)
             #endif
             if (__pyx_t_7 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 152, __pyx_L1_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 134, __pyx_L1_error)
           #else
-          __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 134, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           {
-            Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
+            Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 152, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 134, __pyx_L1_error)
             #endif
             if (__pyx_t_7 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 152, __pyx_L1_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 134, __pyx_L1_error)
           #else
-          __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 134, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
-        __pyx_t_2 = __pyx_t_8(__pyx_t_5);
-        if (unlikely(!__pyx_t_2)) {
+        __pyx_t_5 = __pyx_t_8(__pyx_t_1);
+        if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 152, __pyx_L1_error)
+            else __PYX_ERR(0, 134, __pyx_L1_error)
           }
           break;
         }
-        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_GOTREF(__pyx_t_5);
       }
-      __Pyx_XDECREF_SET(__pyx_v_doc, __pyx_t_2);
-      __pyx_t_2 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_doc, __pyx_t_5);
+      __pyx_t_5 = 0;
 
-      __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_text_embeddings, __pyx_v_doc, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 153, __pyx_L1_error)
+      __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_text_embeddings, __pyx_v_doc, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 135, __pyx_L1_error)
       if (__pyx_t_6) {
 
-        __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_text_embeddings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_XDECREF_SET(__pyx_v_embeddings, __pyx_t_2);
-        __pyx_t_2 = 0;
+        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_text_embeddings); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 136, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __Pyx_XDECREF_SET(__pyx_v_embeddings, __pyx_t_5);
+        __pyx_t_5 = 0;
 
         if (likely(PyList_CheckExact(__pyx_v_embeddings)) || PyTuple_CheckExact(__pyx_v_embeddings)) {
-          __pyx_t_2 = __pyx_v_embeddings; __Pyx_INCREF(__pyx_t_2);
+          __pyx_t_5 = __pyx_v_embeddings; __Pyx_INCREF(__pyx_t_5);
           __pyx_t_9 = 0;
           __pyx_t_10 = NULL;
         } else {
-          __pyx_t_9 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_embeddings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 155, __pyx_L1_error)
+          __pyx_t_9 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_embeddings); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_5);
+          __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 137, __pyx_L1_error)
         }
         for (;;) {
           if (likely(!__pyx_t_10)) {
-            if (likely(PyList_CheckExact(__pyx_t_2))) {
+            if (likely(PyList_CheckExact(__pyx_t_5))) {
               {
-                Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+                Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
                 #if !CYTHON_ASSUME_SAFE_MACROS
-                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 155, __pyx_L1_error)
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 137, __pyx_L1_error)
                 #endif
                 if (__pyx_t_9 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_3); __pyx_t_9++; if (unlikely((0 < 0))) __PYX_ERR(0, 155, __pyx_L1_error)
+              __pyx_t_2 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely((0 < 0))) __PYX_ERR(0, 137, __pyx_L1_error)
               #else
-              __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
-              __Pyx_GOTREF(__pyx_t_3);
+              __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_2);
               #endif
             } else {
               {
-                Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+                Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
                 #if !CYTHON_ASSUME_SAFE_MACROS
-                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 155, __pyx_L1_error)
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 137, __pyx_L1_error)
                 #endif
                 if (__pyx_t_9 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_3); __pyx_t_9++; if (unlikely((0 < 0))) __PYX_ERR(0, 155, __pyx_L1_error)
+              __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely((0 < 0))) __PYX_ERR(0, 137, __pyx_L1_error)
               #else
-              __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
-              __Pyx_GOTREF(__pyx_t_3);
+              __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_2);
               #endif
             }
           } else {
-            __pyx_t_3 = __pyx_t_10(__pyx_t_2);
-            if (unlikely(!__pyx_t_3)) {
+            __pyx_t_2 = __pyx_t_10(__pyx_t_5);
+            if (unlikely(!__pyx_t_2)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                else __PYX_ERR(0, 155, __pyx_L1_error)
+                else __PYX_ERR(0, 137, __pyx_L1_error)
               }
               break;
             }
-            __Pyx_GOTREF(__pyx_t_3);
+            __Pyx_GOTREF(__pyx_t_2);
           }
-          __Pyx_XDECREF_SET(__pyx_v_emb, __pyx_t_3);
-          __pyx_t_3 = 0;
+          __Pyx_XDECREF_SET(__pyx_v_emb, __pyx_t_2);
+          __pyx_t_2 = 0;
 
-          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 156, __pyx_L1_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_array); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 138, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = NULL;
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          __pyx_t_3 = NULL;
           __pyx_t_4 = 0;
           #if CYTHON_UNPACK_METHODS
           if (unlikely(PyMethod_Check(__pyx_t_11))) {
-            __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_11);
-            if (likely(__pyx_t_1)) {
+            __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_11);
+            if (likely(__pyx_t_3)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
-              __Pyx_INCREF(__pyx_t_1);
+              __Pyx_INCREF(__pyx_t_3);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_11, function);
               __pyx_t_4 = 1;
             }
           }
           #endif
           {
-            PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_emb};
-            __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-            __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-            if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_3);
+            PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_emb};
+            __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+            __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+            if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           }
-          __Pyx_XDECREF_SET(__pyx_v_emb_vec, __pyx_t_3);
-          __pyx_t_3 = 0;
+          __Pyx_XDECREF_SET(__pyx_v_emb_vec, __pyx_t_2);
+          __pyx_t_2 = 0;
 
-          __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_dot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_dot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           __pyx_t_11 = NULL;
           __pyx_t_4 = 0;
           #if CYTHON_UNPACK_METHODS
-          if (unlikely(PyMethod_Check(__pyx_t_1))) {
-            __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_1);
+          if (unlikely(PyMethod_Check(__pyx_t_3))) {
+            __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_3);
             if (likely(__pyx_t_11)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
               __Pyx_INCREF(__pyx_t_11);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_1, function);
+              __Pyx_DECREF_SET(__pyx_t_3, function);
               __pyx_t_4 = 1;
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_v_query_vec, __pyx_v_emb_vec};
-            __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+            __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
             __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-            if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_3);
-            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+            if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_2);
+            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           }
-          __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_linalg); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_linalg); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_norm); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_norm); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __pyx_t_12 = NULL;
           __pyx_t_4 = 0;
           #if CYTHON_UNPACK_METHODS
           if (likely(PyMethod_Check(__pyx_t_11))) {
             __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
@@ -6577,26 +6475,26 @@
               __Pyx_DECREF_SET(__pyx_t_11, function);
               __pyx_t_4 = 1;
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_v_query_vec};
-            __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+            __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
             __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_1);
+            if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           }
-          __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_linalg); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_linalg); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_norm); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_norm); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __pyx_t_13 = NULL;
           __pyx_t_4 = 0;
           #if CYTHON_UNPACK_METHODS
           if (likely(PyMethod_Check(__pyx_t_12))) {
             __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_12);
@@ -6609,376 +6507,376 @@
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_13, __pyx_v_emb_vec};
             __pyx_t_11 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
             __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-            if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 157, __pyx_L1_error)
+            if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 139, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_11);
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           }
-          __pyx_t_12 = PyNumber_Multiply(__pyx_t_1, __pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __pyx_t_12 = PyNumber_Multiply(__pyx_t_3, __pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_11 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __pyx_t_11 = __Pyx_PyNumber_Divide(__pyx_t_2, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 139, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_XDECREF_SET(__pyx_v_similar_score, __pyx_t_11);
           __pyx_t_11 = 0;
 
-          __pyx_t_11 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_extracted_text); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 158, __pyx_L1_error)
+          __pyx_t_11 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_extracted_text); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 140, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_XDECREF_SET(__pyx_v_cleaned_text, __pyx_t_11);
           __pyx_t_11 = 0;
 
-          __pyx_t_11 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 160, __pyx_L1_error)
+          __pyx_t_11 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 142, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_filename); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 160, __pyx_L1_error)
+          __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_filename); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 142, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
-          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_filename, __pyx_t_12) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_filename, __pyx_t_12) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_shorten_text); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 161, __pyx_L1_error)
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_shorten_text); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 143, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_3);
+          __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
           __Pyx_INCREF(__pyx_v_cleaned_text);
           __Pyx_GIVEREF(__pyx_v_cleaned_text);
-          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_cleaned_text)) __PYX_ERR(0, 161, __pyx_L1_error);
-          __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_max_length, __pyx_v_extracted_text_length) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-          __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 161, __pyx_L1_error)
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_cleaned_text)) __PYX_ERR(0, 143, __pyx_L1_error);
+          __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_length, __pyx_v_extracted_text_length) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
+          __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 143, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_extracted_text, __pyx_t_13) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_extracted_text, __pyx_t_13) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
-          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_similarity, __pyx_v_similar_score) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_similarity, __pyx_v_similar_score) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
 
-          __pyx_t_14 = __Pyx_PyObject_Append(__pyx_v_similarities, __pyx_t_11); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 159, __pyx_L1_error)
+          __pyx_t_14 = __Pyx_PyObject_Append(__pyx_v_similarities, __pyx_t_11); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 141, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
         }
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
         goto __pyx_L6;
       }
 
       /*else*/ {
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 165, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 147, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 147, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_t_11, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_11, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 147, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_text_embeddings_key_not_found_i, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 165, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_text_embeddings_key_not_found_i, __pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 147, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 147, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
       __pyx_L6:;
 
     }
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 168, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_similarities);
     __Pyx_GIVEREF(__pyx_v_similarities);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_similarities)) __PYX_ERR(0, 168, __pyx_L1_error);
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_11 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13vector_search_lambda, 0, __pyx_n_s_vector_search_locals_lambda, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_similarities)) __PYX_ERR(0, 150, __pyx_L1_error);
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_11 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_13vector_search_lambda, 0, __pyx_n_s_vector_search_locals_lambda, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 150, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_key, __pyx_t_11) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_key, __pyx_t_11) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_reverse, Py_True) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_reverse, Py_True) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 150, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_similarities, __pyx_t_11);
     __pyx_t_11 = 0;
 
-    __pyx_t_11 = __Pyx_PyObject_GetSlice(__pyx_v_similarities, 0, 0, NULL, &__pyx_v_top_n, NULL, 0, 0, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetSlice(__pyx_v_similarities, 0, 0, NULL, &__pyx_v_top_n, NULL, 0, 0, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __pyx_v_top_results = __pyx_t_11;
     __pyx_t_11 = 0;
 
     { /* enter inner scope */
-      __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 172, __pyx_L13_error)
+      __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 154, __pyx_L13_error)
       __Pyx_GOTREF(__pyx_t_11);
       if (likely(PyList_CheckExact(__pyx_v_top_results)) || PyTuple_CheckExact(__pyx_v_top_results)) {
-        __pyx_t_2 = __pyx_v_top_results; __Pyx_INCREF(__pyx_t_2);
+        __pyx_t_5 = __pyx_v_top_results; __Pyx_INCREF(__pyx_t_5);
         __pyx_t_7 = 0;
         __pyx_t_8 = NULL;
       } else {
-        __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_top_results); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L13_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 172, __pyx_L13_error)
+        __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_top_results); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L13_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 154, __pyx_L13_error)
       }
       for (;;) {
         if (likely(!__pyx_t_8)) {
-          if (likely(PyList_CheckExact(__pyx_t_2))) {
+          if (likely(PyList_CheckExact(__pyx_t_5))) {
             {
-              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 172, __pyx_L13_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 154, __pyx_L13_error)
               #endif
               if (__pyx_t_7 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 172, __pyx_L13_error)
+            __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 154, __pyx_L13_error)
             #else
-            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 172, __pyx_L13_error)
-            __Pyx_GOTREF(__pyx_t_5);
+            __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L13_error)
+            __Pyx_GOTREF(__pyx_t_1);
             #endif
           } else {
             {
-              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 172, __pyx_L13_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 154, __pyx_L13_error)
               #endif
               if (__pyx_t_7 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 172, __pyx_L13_error)
+            __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 154, __pyx_L13_error)
             #else
-            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 172, __pyx_L13_error)
-            __Pyx_GOTREF(__pyx_t_5);
+            __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L13_error)
+            __Pyx_GOTREF(__pyx_t_1);
             #endif
           }
         } else {
-          __pyx_t_5 = __pyx_t_8(__pyx_t_2);
-          if (unlikely(!__pyx_t_5)) {
+          __pyx_t_1 = __pyx_t_8(__pyx_t_5);
+          if (unlikely(!__pyx_t_1)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 172, __pyx_L13_error)
+              else __PYX_ERR(0, 154, __pyx_L13_error)
             }
             break;
           }
-          __Pyx_GOTREF(__pyx_t_5);
+          __Pyx_GOTREF(__pyx_t_1);
         }
-        __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_result, __pyx_t_5);
-        __pyx_t_5 = 0;
-        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_7genexpr__pyx_v_result, __pyx_n_u_extracted_text); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 172, __pyx_L13_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_11, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 172, __pyx_L13_error)
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_result, __pyx_t_1);
+        __pyx_t_1 = 0;
+        __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_7genexpr__pyx_v_result, __pyx_n_u_extracted_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L13_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_11, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 154, __pyx_L13_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF(__pyx_7genexpr__pyx_v_result); __pyx_7genexpr__pyx_v_result = 0;
       goto __pyx_L17_exit_scope;
       __pyx_L13_error:;
       __Pyx_XDECREF(__pyx_7genexpr__pyx_v_result); __pyx_7genexpr__pyx_v_result = 0;
       goto __pyx_L1_error;
       __pyx_L17_exit_scope:;
     } /* exit inner scope */
     __pyx_v_extracted_texts = ((PyObject*)__pyx_t_11);
     __pyx_t_11 = 0;
 
     { /* enter inner scope */
-      __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 173, __pyx_L20_error)
+      __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 155, __pyx_L20_error)
       __Pyx_GOTREF(__pyx_t_11);
       if (likely(PyList_CheckExact(__pyx_v_top_results)) || PyTuple_CheckExact(__pyx_v_top_results)) {
-        __pyx_t_2 = __pyx_v_top_results; __Pyx_INCREF(__pyx_t_2);
+        __pyx_t_5 = __pyx_v_top_results; __Pyx_INCREF(__pyx_t_5);
         __pyx_t_7 = 0;
         __pyx_t_8 = NULL;
       } else {
-        __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_top_results); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L20_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 173, __pyx_L20_error)
+        __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_top_results); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 155, __pyx_L20_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 155, __pyx_L20_error)
       }
       for (;;) {
         if (likely(!__pyx_t_8)) {
-          if (likely(PyList_CheckExact(__pyx_t_2))) {
+          if (likely(PyList_CheckExact(__pyx_t_5))) {
             {
-              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 173, __pyx_L20_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 155, __pyx_L20_error)
               #endif
               if (__pyx_t_7 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 173, __pyx_L20_error)
+            __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 155, __pyx_L20_error)
             #else
-            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L20_error)
-            __Pyx_GOTREF(__pyx_t_5);
+            __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L20_error)
+            __Pyx_GOTREF(__pyx_t_1);
             #endif
           } else {
             {
-              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 173, __pyx_L20_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 155, __pyx_L20_error)
               #endif
               if (__pyx_t_7 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 173, __pyx_L20_error)
+            __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 155, __pyx_L20_error)
             #else
-            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L20_error)
-            __Pyx_GOTREF(__pyx_t_5);
+            __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L20_error)
+            __Pyx_GOTREF(__pyx_t_1);
             #endif
           }
         } else {
-          __pyx_t_5 = __pyx_t_8(__pyx_t_2);
-          if (unlikely(!__pyx_t_5)) {
+          __pyx_t_1 = __pyx_t_8(__pyx_t_5);
+          if (unlikely(!__pyx_t_1)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 173, __pyx_L20_error)
+              else __PYX_ERR(0, 155, __pyx_L20_error)
             }
             break;
           }
-          __Pyx_GOTREF(__pyx_t_5);
+          __Pyx_GOTREF(__pyx_t_1);
         }
-        __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_result, __pyx_t_5);
-        __pyx_t_5 = 0;
-        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr1__pyx_v_result, __pyx_n_u_similarity); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L20_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_11, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 173, __pyx_L20_error)
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_result, __pyx_t_1);
+        __pyx_t_1 = 0;
+        __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr1__pyx_v_result, __pyx_n_u_similarity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L20_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_11, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 155, __pyx_L20_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_result); __pyx_8genexpr1__pyx_v_result = 0;
       goto __pyx_L24_exit_scope;
       __pyx_L20_error:;
       __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_result); __pyx_8genexpr1__pyx_v_result = 0;
       goto __pyx_L1_error;
       __pyx_L24_exit_scope:;
     } /* exit inner scope */
     __pyx_v_similarities_values = ((PyObject*)__pyx_t_11);
     __pyx_t_11 = 0;
 
     { /* enter inner scope */
-      __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 174, __pyx_L27_error)
+      __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 156, __pyx_L27_error)
       __Pyx_GOTREF(__pyx_t_11);
       if (likely(PyList_CheckExact(__pyx_v_top_results)) || PyTuple_CheckExact(__pyx_v_top_results)) {
-        __pyx_t_2 = __pyx_v_top_results; __Pyx_INCREF(__pyx_t_2);
+        __pyx_t_5 = __pyx_v_top_results; __Pyx_INCREF(__pyx_t_5);
         __pyx_t_7 = 0;
         __pyx_t_8 = NULL;
       } else {
-        __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_top_results); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L27_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 174, __pyx_L27_error)
+        __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_top_results); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 156, __pyx_L27_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 156, __pyx_L27_error)
       }
       for (;;) {
         if (likely(!__pyx_t_8)) {
-          if (likely(PyList_CheckExact(__pyx_t_2))) {
+          if (likely(PyList_CheckExact(__pyx_t_5))) {
             {
-              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 174, __pyx_L27_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 156, __pyx_L27_error)
               #endif
               if (__pyx_t_7 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 174, __pyx_L27_error)
+            __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 156, __pyx_L27_error)
             #else
-            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L27_error)
-            __Pyx_GOTREF(__pyx_t_5);
+            __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L27_error)
+            __Pyx_GOTREF(__pyx_t_1);
             #endif
           } else {
             {
-              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 174, __pyx_L27_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 156, __pyx_L27_error)
               #endif
               if (__pyx_t_7 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 174, __pyx_L27_error)
+            __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 156, __pyx_L27_error)
             #else
-            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L27_error)
-            __Pyx_GOTREF(__pyx_t_5);
+            __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L27_error)
+            __Pyx_GOTREF(__pyx_t_1);
             #endif
           }
         } else {
-          __pyx_t_5 = __pyx_t_8(__pyx_t_2);
-          if (unlikely(!__pyx_t_5)) {
+          __pyx_t_1 = __pyx_t_8(__pyx_t_5);
+          if (unlikely(!__pyx_t_1)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 174, __pyx_L27_error)
+              else __PYX_ERR(0, 156, __pyx_L27_error)
             }
             break;
           }
-          __Pyx_GOTREF(__pyx_t_5);
+          __Pyx_GOTREF(__pyx_t_1);
         }
-        __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_result, __pyx_t_5);
-        __pyx_t_5 = 0;
-        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr2__pyx_v_result, __pyx_n_u_filename); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L27_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_11, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 174, __pyx_L27_error)
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_result, __pyx_t_1);
+        __pyx_t_1 = 0;
+        __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr2__pyx_v_result, __pyx_n_u_filename); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L27_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_11, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 156, __pyx_L27_error)
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_result); __pyx_8genexpr2__pyx_v_result = 0;
       goto __pyx_L31_exit_scope;
       __pyx_L27_error:;
       __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_result); __pyx_8genexpr2__pyx_v_result = 0;
       goto __pyx_L1_error;
       __pyx_L31_exit_scope:;
     } /* exit inner scope */
     __pyx_v_filenames = ((PyObject*)__pyx_t_11);
     __pyx_t_11 = 0;
 
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_INCREF(__pyx_v_extracted_texts);
     __Pyx_GIVEREF(__pyx_v_extracted_texts);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_v_extracted_texts)) __PYX_ERR(0, 176, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_v_extracted_texts)) __PYX_ERR(0, 158, __pyx_L1_error);
     __Pyx_INCREF(__pyx_v_similarities_values);
     __Pyx_GIVEREF(__pyx_v_similarities_values);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_v_similarities_values)) __PYX_ERR(0, 176, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_v_similarities_values)) __PYX_ERR(0, 158, __pyx_L1_error);
     __Pyx_INCREF(__pyx_v_filenames);
     __Pyx_GIVEREF(__pyx_v_filenames);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_v_filenames)) __PYX_ERR(0, 176, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_v_filenames)) __PYX_ERR(0, 158, __pyx_L1_error);
     __pyx_r = __pyx_t_11;
     __pyx_t_11 = 0;
     goto __pyx_L0;
 
   }
 
   /*else*/ {
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 161, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_t_11, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_11, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Request_failed_with_status_code, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Request_failed_with_status_code, __pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 161, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __pyx_r = __pyx_t_11;
     __pyx_t_11 = 0;
     goto __pyx_L0;
   }
 
 
@@ -6987,15 +6885,15 @@
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.vector_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_url);
   __Pyx_XDECREF(__pyx_v_headers);
   __Pyx_XDECREF(__pyx_v_pipeline);
   __Pyx_XDECREF(__pyx_v_query_payload);
   __Pyx_XDECREF(__pyx_v_response);
@@ -7019,478 +6917,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_15shorten_text(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_3__pyx_unpickle_xyellw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_15shorten_text = {"shorten_text", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_15shorten_text, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_15shorten_text(PyObject *__pyx_v_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_text = 0;
-  PyObject *__pyx_v_max_length = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[2] = {0,0};
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("shorten_text (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_text,&__pyx_n_s_max_length,0};
-    values[1] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)__pyx_int_1000));
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_length);
-          if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "shorten_text") < 0)) __PYX_ERR(0, 183, __pyx_L3_error)
-      }
-    } else {
-      switch (__pyx_nargs) {
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_text = values[0];
-    __pyx_v_max_length = values[1];
-  }
-  goto __pyx_L6_skip;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("shorten_text", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 183, __pyx_L3_error)
-  __pyx_L6_skip:;
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.shorten_text", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_14shorten_text(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text, __pyx_v_max_length);
-
-  /* function exit code */
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14shorten_text(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_max_length) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  Py_ssize_t __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("shorten_text", 1);
-
-  __pyx_t_1 = PyObject_Length(__pyx_v_text); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 184, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_v_max_length, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 184, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__pyx_t_4) {
-
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_v_text, 0, 0, NULL, &__pyx_v_max_length, NULL, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_kp_u__8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
-    goto __pyx_L0;
-
-  }
-
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(__pyx_v_text);
-  __pyx_r = __pyx_v_text;
-  goto __pyx_L0;
-
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.shorten_text", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-
-/* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_17__reduce_cython__(PyObject *__pyx_v_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_17__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_17__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_17__reduce_cython__(PyObject *__pyx_v_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  if (unlikely(__pyx_nargs > 0)) {
-    __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
-  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_16__reduce_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self) {
-  PyObject *__pyx_v_state = 0;
-  PyObject *__pyx_v__dict = 0;
-  int __pyx_v_use_setstate;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
-
-  __Pyx_INCREF(__pyx_empty_tuple);
-  __pyx_v_state = __pyx_empty_tuple;
-
-  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v__dict = __pyx_t_1;
-  __pyx_t_1 = 0;
-
-  __pyx_t_2 = (__pyx_v__dict != Py_None);
-  if (__pyx_t_2) {
-
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_INCREF(__pyx_v__dict);
-    __Pyx_GIVEREF(__pyx_v__dict);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict)) __PYX_ERR(1, 8, __pyx_L1_error);
-    __pyx_t_3 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 8, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_3));
-    __pyx_t_3 = 0;
-
-    __pyx_v_use_setstate = 1;
-
-    goto __pyx_L3;
-  }
-
-  /*else*/ {
-    __pyx_v_use_setstate = 0;
-  }
-  __pyx_L3:;
-
-  if (__pyx_v_use_setstate) {
-
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pyx_unpickle_xyellw); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))))) __PYX_ERR(1, 13, __pyx_L1_error);
-    __Pyx_INCREF(__pyx_int_238750788);
-    __Pyx_GIVEREF(__pyx_int_238750788);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_238750788)) __PYX_ERR(1, 13, __pyx_L1_error);
-    __Pyx_INCREF(Py_None);
-    __Pyx_GIVEREF(Py_None);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None)) __PYX_ERR(1, 13, __pyx_L1_error);
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GIVEREF(__pyx_t_3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(1, 13, __pyx_L1_error);
-    __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error);
-    __Pyx_INCREF(__pyx_v_state);
-    __Pyx_GIVEREF(__pyx_v_state);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_v_state)) __PYX_ERR(1, 13, __pyx_L1_error);
-    __pyx_t_3 = 0;
-    __pyx_t_1 = 0;
-    __pyx_r = __pyx_t_4;
-    __pyx_t_4 = 0;
-    goto __pyx_L0;
-
-  }
-
-  /*else*/ {
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_xyellw); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))))) __PYX_ERR(1, 15, __pyx_L1_error);
-    __Pyx_INCREF(__pyx_int_238750788);
-    __Pyx_GIVEREF(__pyx_int_238750788);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_238750788)) __PYX_ERR(1, 15, __pyx_L1_error);
-    __Pyx_INCREF(__pyx_v_state);
-    __Pyx_GIVEREF(__pyx_v_state);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state)) __PYX_ERR(1, 15, __pyx_L1_error);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_4);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error);
-    __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error);
-    __pyx_t_4 = 0;
-    __pyx_t_1 = 0;
-    __pyx_r = __pyx_t_3;
-    __pyx_t_3 = 0;
-    goto __pyx_L0;
-  }
-
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_state);
-  __Pyx_XDECREF(__pyx_v__dict);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-
-/* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_19__setstate_cython__(PyObject *__pyx_v_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_19__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_19__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_19__setstate_cython__(PyObject *__pyx_v_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v___pyx_state = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[1] = {0};
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 16, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 16, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 1)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-    }
-    __pyx_v___pyx_state = values[0];
-  }
-  goto __pyx_L6_skip;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 16, __pyx_L3_error)
-  __pyx_L6_skip:;
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_18__setstate_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v___pyx_state);
-
-  /* function exit code */
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_18__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
-
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(1, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_8aixhello_6xyello___pyx_unpickle_xyellw__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-
-  /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-
-/* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_1__pyx_unpickle_xyellw(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw = {"__pyx_unpickle_xyellw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_1__pyx_unpickle_xyellw, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_1__pyx_unpickle_xyellw(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_3__pyx_unpickle_xyellw = {"__pyx_unpickle_xyellw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_3__pyx_unpickle_xyellw, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_3__pyx_unpickle_xyellw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_type = 0;
@@ -7586,28 +7029,28 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.__pyx_unpickle_xyellw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_2__pyx_unpickle_xyellw(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_8aixhello_6xyello_2__pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
@@ -7616,15 +7059,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_xyellw", 1);
 
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
@@ -7832,19 +7275,16 @@
 
 static PyMethodDef __pyx_methods_8aixhello_6xyello_xyellw[] = {
   {"Decipherx", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"Encapseal", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"Decenigma", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"vectorizeEmbed", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbed, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"vectorizeText", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"SaveToMongoDb", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"vector_search", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"shorten_text", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_15shorten_text, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_17__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_19__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
 static PyType_Slot __pyx_type_8aixhello_6xyello_xyellw_slots[] = {
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8aixhello_6xyello_xyellw},
   {Py_tp_methods, (void *)__pyx_methods_8aixhello_6xyello_xyellw},
   {Py_tp_new, (void *)__pyx_tp_new_8aixhello_6xyello_xyellw},
@@ -7953,14 +7393,15 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_n_s_, __pyx_k_, sizeof(__pyx_k_), 0, 0, 1, 1},
     {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
     {&__pyx_n_s_AES, __pyx_k_AES, sizeof(__pyx_k_AES), 0, 0, 1, 1},
     {&__pyx_kp_u_Access_Control_Request_Headers, __pyx_k_Access_Control_Request_Headers, sizeof(__pyx_k_Access_Control_Request_Headers), 0, 1, 0, 0},
     {&__pyx_kp_u_An_unexpected_error_occurred, __pyx_k_An_unexpected_error_occurred, sizeof(__pyx_k_An_unexpected_error_occurred), 0, 1, 0, 0},
     {&__pyx_n_s_AuthenticationError, __pyx_k_AuthenticationError, sizeof(__pyx_k_AuthenticationError), 0, 0, 1, 1},
     {&__pyx_n_s_CBC, __pyx_k_CBC, sizeof(__pyx_k_CBC), 0, 0, 1, 1},
     {&__pyx_n_s_Cipher, __pyx_k_Cipher, sizeof(__pyx_k_Cipher), 0, 0, 1, 1},
@@ -7969,61 +7410,50 @@
     {&__pyx_n_s_Decipherx, __pyx_k_Decipherx, sizeof(__pyx_k_Decipherx), 0, 0, 1, 1},
     {&__pyx_n_s_Encapseal, __pyx_k_Encapseal, sizeof(__pyx_k_Encapseal), 0, 0, 1, 1},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_kp_u_Invalid_API_key_provided, __pyx_k_Invalid_API_key_provided, sizeof(__pyx_k_Invalid_API_key_provided), 0, 1, 0, 0},
     {&__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, sizeof(__pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN), 0, 0, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_kp_u_Request_failed_with_status_code, __pyx_k_Request_failed_with_status_code, sizeof(__pyx_k_Request_failed_with_status_code), 0, 1, 0, 0},
-    {&__pyx_n_s_SaveToMongoDb, __pyx_k_SaveToMongoDb, sizeof(__pyx_k_SaveToMongoDb), 0, 0, 1, 1},
-    {&__pyx_kp_u_Successfully_save_to_the_databas, __pyx_k_Successfully_save_to_the_databas, sizeof(__pyx_k_Successfully_save_to_the_databas), 0, 1, 0, 0},
     {&__pyx_kp_u_Unknown_filename, __pyx_k_Unknown_filename, sizeof(__pyx_k_Unknown_filename), 0, 1, 0, 0},
-    {&__pyx_kp_u__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 1, 0, 0},
-    {&__pyx_n_s__35, __pyx_k__35, sizeof(__pyx_k__35), 0, 0, 1, 1},
-    {&__pyx_n_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 1},
-    {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
-    {&__pyx_kp_u__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 1, 0, 0},
+    {&__pyx_n_s__24, __pyx_k__24, sizeof(__pyx_k__24), 0, 0, 1, 1},
+    {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
     {&__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, sizeof(__pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1), 0, 1, 0, 1},
     {&__pyx_n_s_aixhello_xyello, __pyx_k_aixhello_xyello, sizeof(__pyx_k_aixhello_xyello), 0, 0, 1, 1},
     {&__pyx_kp_s_aixhello_xyello_pyx, __pyx_k_aixhello_xyello_pyx, sizeof(__pyx_k_aixhello_xyello_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_algorithms, __pyx_k_algorithms, sizeof(__pyx_k_algorithms), 0, 0, 1, 1},
     {&__pyx_n_s_api_key, __pyx_k_api_key, sizeof(__pyx_k_api_key), 0, 0, 1, 1},
     {&__pyx_kp_u_api_key_2, __pyx_k_api_key_2, sizeof(__pyx_k_api_key_2), 0, 1, 0, 0},
     {&__pyx_n_s_api_url, __pyx_k_api_url, sizeof(__pyx_k_api_url), 0, 0, 1, 1},
     {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
     {&__pyx_kp_u_application_json, __pyx_k_application_json, sizeof(__pyx_k_application_json), 0, 1, 0, 0},
-    {&__pyx_kp_u_application_pdf, __pyx_k_application_pdf, sizeof(__pyx_k_application_pdf), 0, 1, 0, 0},
     {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_b64decode, __pyx_k_b64decode, sizeof(__pyx_k_b64decode), 0, 0, 1, 1},
     {&__pyx_n_s_b64encode, __pyx_k_b64encode, sizeof(__pyx_k_b64encode), 0, 0, 1, 1},
     {&__pyx_n_s_backend, __pyx_k_backend, sizeof(__pyx_k_backend), 0, 0, 1, 1},
     {&__pyx_n_s_base64, __pyx_k_base64, sizeof(__pyx_k_base64), 0, 0, 1, 1},
     {&__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn, __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn, sizeof(__pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn), 0, 1, 0, 0},
-    {&__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2, __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2, sizeof(__pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2), 0, 1, 0, 0},
     {&__pyx_n_s_chr, __pyx_k_chr, sizeof(__pyx_k_chr), 0, 0, 1, 1},
     {&__pyx_n_s_chunk, __pyx_k_chunk, sizeof(__pyx_k_chunk), 0, 0, 1, 1},
     {&__pyx_n_s_cipher, __pyx_k_cipher, sizeof(__pyx_k_cipher), 0, 0, 1, 1},
     {&__pyx_n_s_cleaned_text, __pyx_k_cleaned_text, sizeof(__pyx_k_cleaned_text), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-    {&__pyx_n_s_collection, __pyx_k_collection, sizeof(__pyx_k_collection), 0, 0, 1, 1},
     {&__pyx_n_u_collection, __pyx_k_collection, sizeof(__pyx_k_collection), 0, 1, 0, 1},
     {&__pyx_n_s_connParam, __pyx_k_connParam, sizeof(__pyx_k_connParam), 0, 0, 1, 1},
     {&__pyx_n_s_create, __pyx_k_create, sizeof(__pyx_k_create), 0, 0, 1, 1},
     {&__pyx_n_s_cryptography_hazmat_backends, __pyx_k_cryptography_hazmat_backends, sizeof(__pyx_k_cryptography_hazmat_backends), 0, 0, 1, 1},
     {&__pyx_n_s_cryptography_hazmat_primitives_c, __pyx_k_cryptography_hazmat_primitives_c, sizeof(__pyx_k_cryptography_hazmat_primitives_c), 0, 0, 1, 1},
     {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
     {&__pyx_n_u_dataSource, __pyx_k_dataSource, sizeof(__pyx_k_dataSource), 0, 1, 0, 1},
-    {&__pyx_n_s_database, __pyx_k_database, sizeof(__pyx_k_database), 0, 0, 1, 1},
     {&__pyx_n_u_database, __pyx_k_database, sizeof(__pyx_k_database), 0, 1, 0, 1},
-    {&__pyx_n_s_datasource, __pyx_k_datasource, sizeof(__pyx_k_datasource), 0, 0, 1, 1},
     {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
     {&__pyx_n_s_decoded_encryptedText, __pyx_k_decoded_encryptedText, sizeof(__pyx_k_decoded_encryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_decryptedText, __pyx_k_decryptedText, sizeof(__pyx_k_decryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_decrypted_padded_text, __pyx_k_decrypted_padded_text, sizeof(__pyx_k_decrypted_padded_text), 0, 0, 1, 1},
-    {&__pyx_n_s_decrypted_url, __pyx_k_decrypted_url, sizeof(__pyx_k_decrypted_url), 0, 0, 1, 1},
     {&__pyx_n_s_decryptor, __pyx_k_decryptor, sizeof(__pyx_k_decryptor), 0, 0, 1, 1},
     {&__pyx_n_s_default_backend, __pyx_k_default_backend, sizeof(__pyx_k_default_backend), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_n_s_dict_2, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
     {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
     {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
     {&__pyx_n_s_documents, __pyx_k_documents, sizeof(__pyx_k_documents), 0, 0, 1, 1},
@@ -8035,81 +7465,83 @@
     {&__pyx_n_s_embedding, __pyx_k_embedding, sizeof(__pyx_k_embedding), 0, 0, 1, 1},
     {&__pyx_n_s_embeddings, __pyx_k_embeddings, sizeof(__pyx_k_embeddings), 0, 0, 1, 1},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_encoded_url, __pyx_k_encoded_url, sizeof(__pyx_k_encoded_url), 0, 0, 1, 1},
     {&__pyx_n_s_encryptedText, __pyx_k_encryptedText, sizeof(__pyx_k_encryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_encryptor, __pyx_k_encryptor, sizeof(__pyx_k_encryptor), 0, 0, 1, 1},
-    {&__pyx_n_s_enkyc, __pyx_k_enkyc, sizeof(__pyx_k_enkyc), 0, 0, 1, 1},
     {&__pyx_n_u_enkyc, __pyx_k_enkyc, sizeof(__pyx_k_enkyc), 0, 1, 0, 1},
     {&__pyx_n_u_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 1, 0, 1},
     {&__pyx_n_u_extracted_text, __pyx_k_extracted_text, sizeof(__pyx_k_extracted_text), 0, 1, 0, 1},
     {&__pyx_n_s_extracted_text_length, __pyx_k_extracted_text_length, sizeof(__pyx_k_extracted_text_length), 0, 0, 1, 1},
     {&__pyx_n_s_extracted_texts, __pyx_k_extracted_texts, sizeof(__pyx_k_extracted_texts), 0, 0, 1, 1},
-    {&__pyx_n_u_file_data, __pyx_k_file_data, sizeof(__pyx_k_file_data), 0, 1, 0, 1},
-    {&__pyx_n_u_file_type, __pyx_k_file_type, sizeof(__pyx_k_file_type), 0, 1, 0, 1},
     {&__pyx_n_u_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 1, 0, 1},
     {&__pyx_n_s_filenames, __pyx_k_filenames, sizeof(__pyx_k_filenames), 0, 0, 1, 1},
-    {&__pyx_n_u_filter, __pyx_k_filter, sizeof(__pyx_k_filter), 0, 1, 0, 1},
     {&__pyx_n_s_finalize, __pyx_k_finalize, sizeof(__pyx_k_finalize), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
     {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_n_s_headers, __pyx_k_headers, sizeof(__pyx_k_headers), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_u_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 1, 0, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
     {&__pyx_n_s_input, __pyx_k_input, sizeof(__pyx_k_input), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_iv, __pyx_k_iv, sizeof(__pyx_k_iv), 0, 0, 1, 1},
     {&__pyx_n_s_json, __pyx_k_json, sizeof(__pyx_k_json), 0, 0, 1, 1},
     {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
+    {&__pyx_kp_u_limit, __pyx_k_limit, sizeof(__pyx_k_limit), 0, 1, 0, 0},
     {&__pyx_n_s_linalg, __pyx_k_linalg, sizeof(__pyx_k_linalg), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_max_length, __pyx_k_max_length, sizeof(__pyx_k_max_length), 0, 0, 1, 1},
     {&__pyx_n_u_message, __pyx_k_message, sizeof(__pyx_k_message), 0, 1, 0, 1},
+    {&__pyx_kp_u_meta, __pyx_k_meta, sizeof(__pyx_k_meta), 0, 1, 0, 0},
     {&__pyx_n_s_model, __pyx_k_model, sizeof(__pyx_k_model), 0, 0, 1, 1},
     {&__pyx_n_s_modes, __pyx_k_modes, sizeof(__pyx_k_modes), 0, 0, 1, 1},
     {&__pyx_n_s_msg, __pyx_k_msg, sizeof(__pyx_k_msg), 0, 0, 1, 1},
     {&__pyx_n_s_mth, __pyx_k_mth, sizeof(__pyx_k_mth), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_n_s_norm, __pyx_k_norm, sizeof(__pyx_k_norm), 0, 0, 1, 1},
     {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
     {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
     {&__pyx_n_s_openai, __pyx_k_openai, sizeof(__pyx_k_openai), 0, 0, 1, 1},
     {&__pyx_n_s_pad_length, __pyx_k_pad_length, sizeof(__pyx_k_pad_length), 0, 0, 1, 1},
     {&__pyx_n_s_padded_text, __pyx_k_padded_text, sizeof(__pyx_k_padded_text), 0, 0, 1, 1},
-    {&__pyx_n_s_params_dict, __pyx_k_params_dict, sizeof(__pyx_k_params_dict), 0, 0, 1, 1},
-    {&__pyx_n_s_payload, __pyx_k_payload, sizeof(__pyx_k_payload), 0, 0, 1, 1},
+    {&__pyx_n_u_path, __pyx_k_path, sizeof(__pyx_k_path), 0, 1, 0, 1},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
     {&__pyx_n_s_pipeline, __pyx_k_pipeline, sizeof(__pyx_k_pipeline), 0, 0, 1, 1},
     {&__pyx_n_u_pipeline, __pyx_k_pipeline, sizeof(__pyx_k_pipeline), 0, 1, 0, 1},
     {&__pyx_n_s_post, __pyx_k_post, sizeof(__pyx_k_post), 0, 0, 1, 1},
     {&__pyx_n_s_print, __pyx_k_print, sizeof(__pyx_k_print), 0, 0, 1, 1},
     {&__pyx_kp_u_project, __pyx_k_project, sizeof(__pyx_k_project), 0, 1, 0, 0},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_xyellw, __pyx_k_pyx_unpickle_xyellw, sizeof(__pyx_k_pyx_unpickle_xyellw), 0, 0, 1, 1},
+    {&__pyx_n_u_query, __pyx_k_query, sizeof(__pyx_k_query), 0, 1, 0, 1},
     {&__pyx_n_s_query_payload, __pyx_k_query_payload, sizeof(__pyx_k_query_payload), 0, 0, 1, 1},
     {&__pyx_n_s_query_vec, __pyx_k_query_vec, sizeof(__pyx_k_query_vec), 0, 0, 1, 1},
     {&__pyx_n_s_re, __pyx_k_re, sizeof(__pyx_k_re), 0, 0, 1, 1},
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
     {&__pyx_n_s_requests, __pyx_k_requests, sizeof(__pyx_k_requests), 0, 0, 1, 1},
     {&__pyx_n_s_response, __pyx_k_response, sizeof(__pyx_k_response), 0, 0, 1, 1},
     {&__pyx_n_s_response_data, __pyx_k_response_data, sizeof(__pyx_k_response_data), 0, 0, 1, 1},
     {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
     {&__pyx_n_s_reverse, __pyx_k_reverse, sizeof(__pyx_k_reverse), 0, 0, 1, 1},
+    {&__pyx_n_u_score, __pyx_k_score, sizeof(__pyx_k_score), 0, 1, 0, 1},
+    {&__pyx_kp_u_search, __pyx_k_search, sizeof(__pyx_k_search), 0, 1, 0, 0},
+    {&__pyx_n_u_searchScore, __pyx_k_searchScore, sizeof(__pyx_k_searchScore), 0, 1, 0, 1},
+    {&__pyx_n_u_searchindex, __pyx_k_searchindex, sizeof(__pyx_k_searchindex), 0, 1, 0, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
-    {&__pyx_kp_u_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 1, 0, 0},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_shorten_text, __pyx_k_shorten_text, sizeof(__pyx_k_shorten_text), 0, 0, 1, 1},
     {&__pyx_n_s_similar_score, __pyx_k_similar_score, sizeof(__pyx_k_similar_score), 0, 0, 1, 1},
     {&__pyx_n_s_similarities, __pyx_k_similarities, sizeof(__pyx_k_similarities), 0, 0, 1, 1},
     {&__pyx_n_s_similarities_values, __pyx_k_similarities_values, sizeof(__pyx_k_similarities_values), 0, 0, 1, 1},
     {&__pyx_n_u_similarity, __pyx_k_similarity, sizeof(__pyx_k_similarity), 0, 1, 0, 1},
@@ -8117,163 +7549,130 @@
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
     {&__pyx_n_s_status_code, __pyx_k_status_code, sizeof(__pyx_k_status_code), 0, 0, 1, 1},
     {&__pyx_n_s_strText, __pyx_k_strText, sizeof(__pyx_k_strText), 0, 0, 1, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 0, 1, 1},
+    {&__pyx_n_u_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 1, 0, 1},
     {&__pyx_n_s_text_chunks, __pyx_k_text_chunks, sizeof(__pyx_k_text_chunks), 0, 0, 1, 1},
     {&__pyx_n_s_text_embed, __pyx_k_text_embed, sizeof(__pyx_k_text_embed), 0, 0, 1, 1},
     {&__pyx_kp_u_text_embedding_ada_002, __pyx_k_text_embedding_ada_002, sizeof(__pyx_k_text_embedding_ada_002), 0, 1, 0, 0},
     {&__pyx_n_u_text_embeddings, __pyx_k_text_embeddings, sizeof(__pyx_k_text_embeddings), 0, 1, 0, 1},
     {&__pyx_kp_u_text_embeddings_key_not_found_i, __pyx_k_text_embeddings_key_not_found_i, sizeof(__pyx_k_text_embeddings_key_not_found_i), 0, 1, 0, 0},
     {&__pyx_n_s_text_key, __pyx_k_text_key, sizeof(__pyx_k_text_key), 0, 0, 1, 1},
     {&__pyx_n_s_top_n, __pyx_k_top_n, sizeof(__pyx_k_top_n), 0, 0, 1, 1},
     {&__pyx_n_s_top_results, __pyx_k_top_results, sizeof(__pyx_k_top_results), 0, 0, 1, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
-    {&__pyx_n_u_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 1, 0, 1},
-    {&__pyx_n_u_upsert, __pyx_k_upsert, sizeof(__pyx_k_upsert), 0, 1, 0, 1},
     {&__pyx_n_s_url, __pyx_k_url, sizeof(__pyx_k_url), 0, 0, 1, 1},
     {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
     {&__pyx_n_s_vector_query, __pyx_k_vector_query, sizeof(__pyx_k_vector_query), 0, 0, 1, 1},
     {&__pyx_n_s_vector_search, __pyx_k_vector_search, sizeof(__pyx_k_vector_search), 0, 0, 1, 1},
     {&__pyx_n_s_vector_search_locals_lambda, __pyx_k_vector_search_locals_lambda, sizeof(__pyx_k_vector_search_locals_lambda), 0, 0, 1, 1},
     {&__pyx_n_s_vectorizeEmbed, __pyx_k_vectorizeEmbed, sizeof(__pyx_k_vectorizeEmbed), 0, 0, 1, 1},
     {&__pyx_n_s_vectorizeText, __pyx_k_vectorizeText, sizeof(__pyx_k_vectorizeText), 0, 0, 1, 1},
+    {&__pyx_n_u_wildcard, __pyx_k_wildcard, sizeof(__pyx_k_wildcard), 0, 1, 0, 1},
     {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw, __pyx_k_xyellw, sizeof(__pyx_k_xyellw), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decenigma, __pyx_k_xyellw_Decenigma, sizeof(__pyx_k_xyellw_Decenigma), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decipherx, __pyx_k_xyellw_Decipherx, sizeof(__pyx_k_xyellw_Decipherx), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Encapseal, __pyx_k_xyellw_Encapseal, sizeof(__pyx_k_xyellw_Encapseal), 0, 0, 1, 1},
-    {&__pyx_n_s_xyellw_SaveToMongoDb, __pyx_k_xyellw_SaveToMongoDb, sizeof(__pyx_k_xyellw_SaveToMongoDb), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___reduce_cython, __pyx_k_xyellw___reduce_cython, sizeof(__pyx_k_xyellw___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___setstate_cython, __pyx_k_xyellw___setstate_cython, sizeof(__pyx_k_xyellw___setstate_cython), 0, 0, 1, 1},
-    {&__pyx_n_s_xyellw_shorten_text, __pyx_k_xyellw_shorten_text, sizeof(__pyx_k_xyellw_shorten_text), 0, 0, 1, 1},
-    {&__pyx_n_s_xyellw_vector_search, __pyx_k_xyellw_vector_search, sizeof(__pyx_k_xyellw_vector_search), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_vectorizeEmbed, __pyx_k_xyellw_vectorizeEmbed, sizeof(__pyx_k_xyellw_vectorizeEmbed), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_vectorizeText, __pyx_k_xyellw_vectorizeText, sizeof(__pyx_k_xyellw_vectorizeText), 0, 0, 1, 1},
     {&__pyx_kp_b_y1c8_8BxP9XN_VKM, __pyx_k_y1c8_8BxP9XN_VKM, sizeof(__pyx_k_y1c8_8BxP9XN_VKM), 0, 0, 0, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 165, __pyx_L1_error)
-  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 147, __pyx_L1_error)
+  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 150, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_u_filename, __pyx_kp_u_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_u_filename, __pyx_kp_u_Unknown_filename); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_file_data, __pyx_kp_u_); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_extracted_text, __pyx_kp_u_); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-
-  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_text_embeddings, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 11, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 11, __pyx_L1_error)
 
-  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_u_filename, __pyx_kp_u_Unknown_filename); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 18, __pyx_L1_error)
 
-  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 33, __pyx_L1_error)
 
-  __pyx_tuple__11 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 11, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeEmbed, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 50, __pyx_L1_error)
 
-  __pyx_tuple__13 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_text_embed, __pyx_n_s_text_key, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeText, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 67, __pyx_L1_error)
 
-  __pyx_tuple__15 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(1, 1, __pyx_L1_error)
 
-  __pyx_tuple__17 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeEmbed, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(1, 16, __pyx_L1_error)
 
-  __pyx_tuple__19 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_text_embed, __pyx_n_s_text_key, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(27, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_extracted_text_length, __pyx_n_s_vector_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_similarities, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_query_vec, __pyx_n_s_doc, __pyx_n_s_embeddings, __pyx_n_s_emb, __pyx_n_s_emb_vec, __pyx_n_s_similar_score, __pyx_n_s_cleaned_text, __pyx_n_s_top_results, __pyx_n_s_extracted_texts, __pyx_n_s_similarities_values, __pyx_n_s_filenames, __pyx_n_s_result, __pyx_n_s_result, __pyx_n_s_result); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeText, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 67, __pyx_L1_error)
-
-  __pyx_tuple__21 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vector_search, 81, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(1, ((PyObject *)__pyx_int_5)); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SaveToMongoDb, 81, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 81, __pyx_L1_error)
 
-  __pyx_tuple__23 = PyTuple_Pack(27, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_extracted_text_length, __pyx_n_s_vector_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_similarities, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_query_vec, __pyx_n_s_doc, __pyx_n_s_embeddings, __pyx_n_s_emb, __pyx_n_s_emb_vec, __pyx_n_s_similar_score, __pyx_n_s_cleaned_text, __pyx_n_s_top_results, __pyx_n_s_extracted_texts, __pyx_n_s_similarities_values, __pyx_n_s_filenames, __pyx_n_s_result, __pyx_n_s_result, __pyx_n_s_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 114, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vector_search, 114, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_int_5); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 114, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
-
-  __pyx_tuple__26 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_text, __pyx_n_s_max_length); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_shorten_text, 183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_int_1000); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-
-  __pyx_tuple__29 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(1, 1, __pyx_L1_error)
-
-  __pyx_tuple__31 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(1, 16, __pyx_L1_error)
-
-  __pyx_tuple__33 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_5 = PyInt_FromLong(5); if (unlikely(!__pyx_int_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_200 = PyInt_FromLong(200); if (unlikely(!__pyx_int_200)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_1000 = PyInt_FromLong(1000); if (unlikely(!__pyx_int_1000)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_222419149 = PyInt_FromLong(222419149L); if (unlikely(!__pyx_int_222419149)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_228825662 = PyInt_FromLong(228825662L); if (unlikely(!__pyx_int_228825662)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_238750788 = PyInt_FromLong(238750788L); if (unlikely(!__pyx_int_238750788)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -8719,77 +8118,63 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decipherx, __pyx_t_2) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Encapseal, __pyx_t_2) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decenigma, __pyx_t_2) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbed, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeEmbed, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbed, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeEmbed, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorizeEmbed, __pyx_t_2) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorizeText, __pyx_t_2) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11SaveToMongoDb, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SaveToMongoDb, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_SaveToMongoDb, __pyx_t_2) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
-
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13vector_search, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vector_search, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__25);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vector_search, __pyx_t_2) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
-
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_15shorten_text, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_shorten_text, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__28);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_shorten_text, __pyx_t_2) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_17__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_19__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1vector_search, 0, __pyx_n_s_vector_search, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__21);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_vector_search, __pyx_t_2) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_3__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_xyellw, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -10360,14 +9745,155 @@
     PyErr_SetExcInfo(*type, *value, *tb);
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #endif
 
+/* KeywordStringCheck */
+static int __Pyx_CheckKeywordStrings(
+    PyObject *kw,
+    const char* function_name,
+    int kw_allowed)
+{
+    PyObject* key = 0;
+    Py_ssize_t pos = 0;
+#if CYTHON_COMPILING_IN_PYPY
+    if (!kw_allowed && PyDict_Next(kw, &pos, &key, 0))
+        goto invalid_keyword;
+    return 1;
+#else
+    if (CYTHON_METH_FASTCALL && likely(PyTuple_Check(kw))) {
+        Py_ssize_t kwsize;
+#if CYTHON_ASSUME_SAFE_MACROS
+        kwsize = PyTuple_GET_SIZE(kw);
+#else
+        kwsize = PyTuple_Size(kw);
+        if (kwsize < 0) return 0;
+#endif
+        if (unlikely(kwsize == 0))
+            return 1;
+        if (!kw_allowed) {
+#if CYTHON_ASSUME_SAFE_MACROS
+            key = PyTuple_GET_ITEM(kw, 0);
+#else
+            key = PyTuple_GetItem(kw, pos);
+            if (!key) return 0;
+#endif
+            goto invalid_keyword;
+        }
+#if PY_VERSION_HEX < 0x03090000
+        for (pos = 0; pos < kwsize; pos++) {
+#if CYTHON_ASSUME_SAFE_MACROS
+            key = PyTuple_GET_ITEM(kw, pos);
+#else
+            key = PyTuple_GetItem(kw, pos);
+            if (!key) return 0;
+#endif
+            if (unlikely(!PyUnicode_Check(key)))
+                goto invalid_keyword_type;
+        }
+#endif
+        return 1;
+    }
+    while (PyDict_Next(kw, &pos, &key, 0)) {
+        #if PY_MAJOR_VERSION < 3
+        if (unlikely(!PyString_Check(key)))
+        #endif
+            if (unlikely(!PyUnicode_Check(key)))
+                goto invalid_keyword_type;
+    }
+    if (!kw_allowed && unlikely(key))
+        goto invalid_keyword;
+    return 1;
+invalid_keyword_type:
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() keywords must be strings", function_name);
+    return 0;
+#endif
+invalid_keyword:
+    #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() got an unexpected keyword argument '%.200s'",
+        function_name, PyString_AsString(key));
+    #else
+    PyErr_Format(PyExc_TypeError,
+        "%s() got an unexpected keyword argument '%U'",
+        function_name, key);
+    #endif
+    return 0;
+}
+
+/* GetAttr3 */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
+static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        return NULL;
+    __Pyx_PyErr_Clear();
+    Py_INCREF(d);
+    return d;
+}
+#endif
+static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
+    PyObject *r;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    int res = PyObject_GetOptionalAttr(o, n, &r);
+    return (res != 0) ? r : __Pyx_NewRef(d);
+#else
+  #if CYTHON_USE_TYPE_SLOTS
+    if (likely(PyString_Check(n))) {
+        r = __Pyx_PyObject_GetAttrStrNoError(o, n);
+        if (unlikely(!r) && likely(!PyErr_Occurred())) {
+            r = __Pyx_NewRef(d);
+        }
+        return r;
+    }
+  #endif
+    r = PyObject_GetAttr(o, n);
+    return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
+#endif
+}
+
+/* RaiseUnexpectedTypeError */
+static int
+__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
+{
+    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
+                 expected, obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return 0;
+}
+
+/* DictGetItem */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
+    PyObject *value;
+    value = PyDict_GetItemWithError(d, key);
+    if (unlikely(!value)) {
+        if (!PyErr_Occurred()) {
+            if (unlikely(PyTuple_Check(key))) {
+                PyObject* args = PyTuple_Pack(1, key);
+                if (likely(args)) {
+                    PyErr_SetObject(PyExc_KeyError, args);
+                    Py_DECREF(args);
+                }
+            } else {
+                PyErr_SetObject(PyExc_KeyError, key);
+            }
+        }
+        return NULL;
+    }
+    Py_INCREF(value);
+    return value;
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
@@ -10432,38 +9958,14 @@
 #endif
         return ((double)a == (double)b);
     }
     return __Pyx_PyObject_IsTrueAndDecref(
         PyObject_RichCompare(op1, op2, Py_EQ));
 }
 
-/* DictGetItem */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
-        return NULL;
-    }
-    Py_INCREF(value);
-    return value;
-}
-#endif
-
 /* PyObjectCall2Args */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args[3] = {NULL, arg1, arg2};
     return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectGetMethod */
@@ -11854,131 +11356,14 @@
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
-/* KeywordStringCheck */
-static int __Pyx_CheckKeywordStrings(
-    PyObject *kw,
-    const char* function_name,
-    int kw_allowed)
-{
-    PyObject* key = 0;
-    Py_ssize_t pos = 0;
-#if CYTHON_COMPILING_IN_PYPY
-    if (!kw_allowed && PyDict_Next(kw, &pos, &key, 0))
-        goto invalid_keyword;
-    return 1;
-#else
-    if (CYTHON_METH_FASTCALL && likely(PyTuple_Check(kw))) {
-        Py_ssize_t kwsize;
-#if CYTHON_ASSUME_SAFE_MACROS
-        kwsize = PyTuple_GET_SIZE(kw);
-#else
-        kwsize = PyTuple_Size(kw);
-        if (kwsize < 0) return 0;
-#endif
-        if (unlikely(kwsize == 0))
-            return 1;
-        if (!kw_allowed) {
-#if CYTHON_ASSUME_SAFE_MACROS
-            key = PyTuple_GET_ITEM(kw, 0);
-#else
-            key = PyTuple_GetItem(kw, pos);
-            if (!key) return 0;
-#endif
-            goto invalid_keyword;
-        }
-#if PY_VERSION_HEX < 0x03090000
-        for (pos = 0; pos < kwsize; pos++) {
-#if CYTHON_ASSUME_SAFE_MACROS
-            key = PyTuple_GET_ITEM(kw, pos);
-#else
-            key = PyTuple_GetItem(kw, pos);
-            if (!key) return 0;
-#endif
-            if (unlikely(!PyUnicode_Check(key)))
-                goto invalid_keyword_type;
-        }
-#endif
-        return 1;
-    }
-    while (PyDict_Next(kw, &pos, &key, 0)) {
-        #if PY_MAJOR_VERSION < 3
-        if (unlikely(!PyString_Check(key)))
-        #endif
-            if (unlikely(!PyUnicode_Check(key)))
-                goto invalid_keyword_type;
-    }
-    if (!kw_allowed && unlikely(key))
-        goto invalid_keyword;
-    return 1;
-invalid_keyword_type:
-    PyErr_Format(PyExc_TypeError,
-        "%.200s() keywords must be strings", function_name);
-    return 0;
-#endif
-invalid_keyword:
-    #if PY_MAJOR_VERSION < 3
-    PyErr_Format(PyExc_TypeError,
-        "%.200s() got an unexpected keyword argument '%.200s'",
-        function_name, PyString_AsString(key));
-    #else
-    PyErr_Format(PyExc_TypeError,
-        "%s() got an unexpected keyword argument '%U'",
-        function_name, key);
-    #endif
-    return 0;
-}
-
-/* GetAttr3 */
-#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
-static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        return NULL;
-    __Pyx_PyErr_Clear();
-    Py_INCREF(d);
-    return d;
-}
-#endif
-static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
-    PyObject *r;
-#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
-    int res = PyObject_GetOptionalAttr(o, n, &r);
-    return (res != 0) ? r : __Pyx_NewRef(d);
-#else
-  #if CYTHON_USE_TYPE_SLOTS
-    if (likely(PyString_Check(n))) {
-        r = __Pyx_PyObject_GetAttrStrNoError(o, n);
-        if (unlikely(!r) && likely(!PyErr_Occurred())) {
-            r = __Pyx_NewRef(d);
-        }
-        return r;
-    }
-  #endif
-    r = PyObject_GetAttr(o, n);
-    return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
-#endif
-}
-
-/* RaiseUnexpectedTypeError */
-static int
-__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
-{
-    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
-                 expected, obj_type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
-    return 0;
-}
-
 /* Import */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *module = 0;
     PyObject *empty_dict = 0;
     PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
@@ -12042,15 +11427,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__10);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__4);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -12696,15 +12081,15 @@
         return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
     }
     return module;
 }
 #endif
 static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__6;
+    PyObject *module, *from_list, *star = __pyx_n_s_;
     CYTHON_UNUSED_VAR(parts_tuple);
     from_list = PyList_New(1);
     if (unlikely(!from_list))
         return NULL;
     Py_INCREF(star);
     PyList_SET_ITEM(from_list, 0, star);
     module = __Pyx_Import(name, from_list, 0);
@@ -13432,15 +12817,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__35);
+        name = __Pyx_NewRef(__pyx_n_s__24);
     }
     return name;
 }
 #endif
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
```

### Comparing `aixhello-3.3/aixhello.egg-info/PKG-INFO` & `aixhello-3.4/aixhello.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.3
+Version: 3.4
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.3/setup.py` & `aixhello-3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='3.3',  # Increment the version number
+    version='3.4',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

