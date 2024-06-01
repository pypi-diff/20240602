# Comparing `tmp/aixhello-2.1.tar.gz` & `tmp/aixhello-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-2.1.tar", last modified: Sat Jun  1 21:46:22 2024, max compression
+gzip compressed data, was "aixhello-2.2.tar", last modified: Sat Jun  1 22:18:10 2024, max compression
```

## Comparing `aixhello-2.1.tar` & `aixhello-2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 21:46:22.656191 aixhello-2.1/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-2.1/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      650 2024-06-01 21:46:22.655192 aixhello-2.1/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 21:46:22.636035 aixhello-2.1/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-2.1/aixhello/__init__.py
--rw-rw-rw-   0        0        0   422971 2024-06-01 21:46:16.000000 aixhello-2.1/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-01 21:46:22.654195 aixhello-2.1/aixhello.egg-info/
--rw-rw-rw-   0        0        0      650 2024-06-01 21:46:22.000000 aixhello-2.1/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-01 21:46:22.000000 aixhello-2.1/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:46:22.000000 aixhello-2.1/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-01 21:46:22.000000 aixhello-2.1/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 21:46:22.000000 aixhello-2.1/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-01 21:46:22.658201 aixhello-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-01 21:45:44.000000 aixhello-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:18:10.884793 aixhello-2.2/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-2.2/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      650 2024-06-01 22:18:10.884793 aixhello-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 22:18:10.862786 aixhello-2.2/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-2.2/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   457867 2024-06-01 22:18:03.000000 aixhello-2.2/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-01 22:18:10.882782 aixhello-2.2/aixhello.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-06-01 22:18:10.000000 aixhello-2.2/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-01 22:18:10.000000 aixhello-2.2/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 22:18:10.000000 aixhello-2.2/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-01 22:18:10.000000 aixhello-2.2/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 22:18:10.000000 aixhello-2.2/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-01 22:18:10.887781 aixhello-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-01 22:17:34.000000 aixhello-2.2/setup.py
```

### Comparing `aixhello-2.1/LICENSE` & `aixhello-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-2.1/PKG-INFO` & `aixhello-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 2.1
+Version: 2.2
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-2.1/aixhello/xyello.c` & `aixhello-2.2/aixhello/xyello.c`

 * *Files 2% similar despite different names*

```diff
@@ -1886,14 +1886,17 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* PyIntCompare.proto */
+static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
+
 /* KeywordStringCheck.proto */
 static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
 /* RaiseUnexpectedTypeError.proto */
@@ -2203,28 +2206,32 @@
 extern int __pyx_module_is_main_aixhello__xyello;
 int __pyx_module_is_main_aixhello__xyello = 0;
 
 /* Implementation of "aixhello.xyello" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_chr;
 /* #### Code section: string_decls ### */
-static const char __pyx_k__2[] = ".";
-static const char __pyx_k__3[] = "*";
+static const char __pyx_k_[] = "";
+static const char __pyx_k__9[] = "*";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_iv[] = "iv";
 static const char __pyx_k_AES[] = "AES";
 static const char __pyx_k_CBC[] = "CBC";
-static const char __pyx_k__18[] = "?";
+static const char __pyx_k__12[] = ".";
+static const char __pyx_k__29[] = "?";
 static const char __pyx_k_chr[] = "chr";
+static const char __pyx_k_get[] = "get";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_msg[] = "msg";
 static const char __pyx_k_mth[] = "mth";
 static const char __pyx_k_new[] = "__new__";
+static const char __pyx_k_set[] = "$set";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
+static const char __pyx_k_json[] = "json";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_post[] = "post";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_text[] = "text";
@@ -2237,92 +2244,117 @@
 static const char __pyx_k_Cipher[] = "Cipher";
 static const char __pyx_k_base64[] = "base64";
 static const char __pyx_k_cipher[] = "cipher";
 static const char __pyx_k_create[] = "create";
 static const char __pyx_k_decode[] = "decode";
 static const char __pyx_k_dict_2[] = "_dict";
 static const char __pyx_k_enable[] = "enable";
+static const char __pyx_k_enckyc[] = "enckyc";
 static const char __pyx_k_encode[] = "encode";
+static const char __pyx_k_filter[] = "filter";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_openai[] = "openai";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_update[] = "update";
+static const char __pyx_k_upsert[] = "upsert";
 static const char __pyx_k_xyellw[] = "xyellw";
 static const char __pyx_k_api_key[] = "api_key";
 static const char __pyx_k_api_url[] = "api_url";
 static const char __pyx_k_backend[] = "backend";
 static const char __pyx_k_disable[] = "disable";
+static const char __pyx_k_headers[] = "headers";
 static const char __pyx_k_message[] = "message";
+static const char __pyx_k_payload[] = "payload";
 static const char __pyx_k_strText[] = "strText";
+static const char __pyx_k_database[] = "database";
+static const char __pyx_k_filename[] = "filename";
 static const char __pyx_k_finalize[] = "finalize";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_requests[] = "requests";
 static const char __pyx_k_response[] = "response";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_text_key[] = "text_key";
 static const char __pyx_k_Decenigma[] = "Decenigma";
 static const char __pyx_k_Decipherx[] = "Decipherx";
 static const char __pyx_k_Encapseal[] = "Encapseal";
+static const char __pyx_k_api_key_2[] = "api-key";
 static const char __pyx_k_b64decode[] = "b64decode";
 static const char __pyx_k_b64encode[] = "b64encode";
 static const char __pyx_k_decryptor[] = "decryptor";
 static const char __pyx_k_embedding[] = "embedding";
 static const char __pyx_k_encryptor[] = "encryptor";
+static const char __pyx_k_file_data[] = "file_data";
+static const char __pyx_k_file_type[] = "file_type";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_algorithms[] = "algorithms";
+static const char __pyx_k_collection[] = "collection";
+static const char __pyx_k_dataSource[] = "dataSource";
 static const char __pyx_k_embeddings[] = "embeddings";
 static const char __pyx_k_pad_length[] = "pad_length";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_Embedshroud[] = "Embedshroud";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_encoded_url[] = "encoded_url";
 static const char __pyx_k_padded_text[] = "padded_text";
+static const char __pyx_k_params_dict[] = "params_dict";
+static const char __pyx_k_status_code[] = "status_code";
 static const char __pyx_k_text_chunks[] = "text_chunks";
+static const char __pyx_k_Content_Type[] = "Content-Type";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_use_setstate[] = "use_setstate";
+static const char __pyx_k_SaveToMongoDb[] = "SaveToMongoDb";
 static const char __pyx_k_decryptedText[] = "decryptedText";
+static const char __pyx_k_decrypted_url[] = "decrypted_url";
 static const char __pyx_k_encryptedText[] = "encryptedText";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_extracted_text[] = "extracted_text";
 static const char __pyx_k_aixhello_xyello[] = "aixhello.xyello";
+static const char __pyx_k_application_pdf[] = "application/pdf";
 static const char __pyx_k_default_backend[] = "default_backend";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
+static const char __pyx_k_text_embeddings[] = "text_embeddings";
+static const char __pyx_k_application_json[] = "application/json";
 static const char __pyx_k_xyellw_Decenigma[] = "xyellw.Decenigma";
 static const char __pyx_k_xyellw_Decipherx[] = "xyellw.Decipherx";
 static const char __pyx_k_xyellw_Encapseal[] = "xyellw.Encapseal";
 static const char __pyx_k_y1c8_8BxP9XN_VKM[] = "y1c8@8BxP9XN#VKM";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_xyellw_Embedshroud[] = "xyellw.Embedshroud";
 static const char __pyx_k_aixhello_xyello_pyx[] = "aixhello\\xyello.pyx";
 static const char __pyx_k_pyx_unpickle_xyellw[] = "__pyx_unpickle_xyellw";
+static const char __pyx_k_xyellw_SaveToMongoDb[] = "xyellw.SaveToMongoDb";
 static const char __pyx_k_decoded_encryptedText[] = "decoded_encryptedText";
 static const char __pyx_k_decrypted_padded_text[] = "decrypted_padded_text";
 static const char __pyx_k_text_embedding_ada_002[] = "text-embedding-ada-002";
 static const char __pyx_k_xyellw___reduce_cython[] = "xyellw.__reduce_cython__";
 static const char __pyx_k_xyellw___setstate_cython[] = "xyellw.__setstate_cython__";
 static const char __pyx_k_cryptography_hazmat_backends[] = "cryptography.hazmat.backends";
+static const char __pyx_k_Access_Control_Request_Headers[] = "Access-Control-Request-Headers";
 static const char __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN[] = "M#rztXq3z@U8rS5jN@PvE4W7F&J(#DhN";
+static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4BFhKWk32xGPxL9k3jhhHkDqcCQrX37yfmobUNPTXxEGQ==";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())";
 static const char __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1[] = "aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1cmUvc0xwaG9RdURybDZv";
 static const char __pyx_k_cryptography_hazmat_primitives_c[] = "cryptography.hazmat.primitives.ciphers";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_params_dict); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
@@ -2348,137 +2380,178 @@
   #ifdef __Pyx_Coroutine_USED
   PyTypeObject *__pyx_CoroutineType;
   #endif
   #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_8aixhello_6xyello_xyellw;
   #endif
   PyTypeObject *__pyx_ptype_8aixhello_6xyello_xyellw;
+  PyObject *__pyx_kp_u_;
   PyObject *__pyx_n_s_AES;
+  PyObject *__pyx_kp_u_Access_Control_Request_Headers;
   PyObject *__pyx_n_s_CBC;
   PyObject *__pyx_n_s_Cipher;
+  PyObject *__pyx_kp_u_Content_Type;
   PyObject *__pyx_n_s_Decenigma;
   PyObject *__pyx_n_s_Decipherx;
   PyObject *__pyx_n_s_Embedshroud;
   PyObject *__pyx_n_s_Encapseal;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
   PyObject *__pyx_n_s_PickleError;
-  PyObject *__pyx_n_s__18;
-  PyObject *__pyx_kp_u__2;
-  PyObject *__pyx_n_s__3;
+  PyObject *__pyx_n_s_SaveToMongoDb;
+  PyObject *__pyx_kp_u__12;
+  PyObject *__pyx_n_s__29;
+  PyObject *__pyx_n_s__9;
+  PyObject *__pyx_kp_u__9;
   PyObject *__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1;
   PyObject *__pyx_n_s_aixhello_xyello;
   PyObject *__pyx_kp_s_aixhello_xyello_pyx;
   PyObject *__pyx_n_s_algorithms;
   PyObject *__pyx_n_s_api_key;
+  PyObject *__pyx_kp_u_api_key_2;
   PyObject *__pyx_n_s_api_url;
+  PyObject *__pyx_kp_u_application_json;
+  PyObject *__pyx_kp_u_application_pdf;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_b64decode;
   PyObject *__pyx_n_s_b64encode;
   PyObject *__pyx_n_s_backend;
   PyObject *__pyx_n_s_base64;
+  PyObject *__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn;
   PyObject *__pyx_n_s_chr;
   PyObject *__pyx_n_s_chunk;
   PyObject *__pyx_n_s_cipher;
   PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_u_collection;
   PyObject *__pyx_n_s_create;
   PyObject *__pyx_n_s_cryptography_hazmat_backends;
   PyObject *__pyx_n_s_cryptography_hazmat_primitives_c;
   PyObject *__pyx_n_s_data;
+  PyObject *__pyx_n_u_dataSource;
+  PyObject *__pyx_n_u_database;
   PyObject *__pyx_n_s_decode;
   PyObject *__pyx_n_s_decoded_encryptedText;
   PyObject *__pyx_n_s_decryptedText;
   PyObject *__pyx_n_s_decrypted_padded_text;
+  PyObject *__pyx_n_s_decrypted_url;
   PyObject *__pyx_n_s_decryptor;
   PyObject *__pyx_n_s_default_backend;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_dict_2;
   PyObject *__pyx_kp_u_disable;
   PyObject *__pyx_n_s_embedding;
   PyObject *__pyx_n_s_embeddings;
   PyObject *__pyx_kp_u_enable;
+  PyObject *__pyx_n_u_enckyc;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_encoded_url;
   PyObject *__pyx_n_s_encryptedText;
   PyObject *__pyx_n_s_encryptor;
+  PyObject *__pyx_n_u_extracted_text;
+  PyObject *__pyx_n_u_file_data;
+  PyObject *__pyx_n_u_file_type;
+  PyObject *__pyx_n_u_filename;
+  PyObject *__pyx_n_u_filter;
   PyObject *__pyx_n_s_finalize;
   PyObject *__pyx_kp_u_gc;
+  PyObject *__pyx_n_s_get;
   PyObject *__pyx_n_s_getstate;
+  PyObject *__pyx_n_s_headers;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_initializing;
   PyObject *__pyx_n_s_input;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_iv;
+  PyObject *__pyx_n_s_json;
   PyObject *__pyx_n_s_key;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_u_message;
   PyObject *__pyx_n_s_model;
   PyObject *__pyx_n_s_modes;
   PyObject *__pyx_n_s_msg;
   PyObject *__pyx_n_s_mth;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_n_s_openai;
   PyObject *__pyx_n_s_pad_length;
   PyObject *__pyx_n_s_padded_text;
+  PyObject *__pyx_n_s_params_dict;
+  PyObject *__pyx_n_s_payload;
   PyObject *__pyx_n_s_pickle;
   PyObject *__pyx_n_s_post;
   PyObject *__pyx_n_s_pyx_PickleError;
   PyObject *__pyx_n_s_pyx_checksum;
   PyObject *__pyx_n_s_pyx_result;
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_pyx_type;
   PyObject *__pyx_n_s_pyx_unpickle_xyellw;
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_requests;
   PyObject *__pyx_n_s_response;
   PyObject *__pyx_n_s_self;
+  PyObject *__pyx_kp_u_set;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_state;
+  PyObject *__pyx_n_s_status_code;
   PyObject *__pyx_n_s_strText;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_text;
   PyObject *__pyx_n_s_text_chunks;
   PyObject *__pyx_kp_u_text_embedding_ada_002;
+  PyObject *__pyx_n_u_text_embeddings;
   PyObject *__pyx_n_s_text_key;
   PyObject *__pyx_n_s_update;
+  PyObject *__pyx_n_u_update;
+  PyObject *__pyx_n_u_upsert;
   PyObject *__pyx_n_s_use_setstate;
   PyObject *__pyx_kp_u_utf_8;
   PyObject *__pyx_n_s_xyellw;
   PyObject *__pyx_n_s_xyellw_Decenigma;
   PyObject *__pyx_n_s_xyellw_Decipherx;
   PyObject *__pyx_n_s_xyellw_Embedshroud;
   PyObject *__pyx_n_s_xyellw_Encapseal;
+  PyObject *__pyx_n_s_xyellw_SaveToMongoDb;
   PyObject *__pyx_n_s_xyellw___reduce_cython;
   PyObject *__pyx_n_s_xyellw___setstate_cython;
   PyObject *__pyx_kp_b_y1c8_8BxP9XN_VKM;
+  PyObject *__pyx_int_200;
   PyObject *__pyx_int_222419149;
   PyObject *__pyx_int_228825662;
   PyObject *__pyx_int_238750788;
-  PyObject *__pyx_tuple_;
+  PyObject *__pyx_tuple__2;
+  PyObject *__pyx_tuple__3;
   PyObject *__pyx_tuple__4;
+  PyObject *__pyx_tuple__5;
   PyObject *__pyx_tuple__6;
+  PyObject *__pyx_tuple__7;
   PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__10;
-  PyObject *__pyx_tuple__12;
-  PyObject *__pyx_tuple__14;
-  PyObject *__pyx_tuple__16;
-  PyObject *__pyx_codeobj__5;
-  PyObject *__pyx_codeobj__7;
-  PyObject *__pyx_codeobj__9;
-  PyObject *__pyx_codeobj__11;
-  PyObject *__pyx_codeobj__13;
-  PyObject *__pyx_codeobj__15;
-  PyObject *__pyx_codeobj__17;
+  PyObject *__pyx_tuple__11;
+  PyObject *__pyx_tuple__13;
+  PyObject *__pyx_tuple__15;
+  PyObject *__pyx_tuple__17;
+  PyObject *__pyx_tuple__19;
+  PyObject *__pyx_tuple__21;
+  PyObject *__pyx_tuple__23;
+  PyObject *__pyx_tuple__25;
+  PyObject *__pyx_tuple__27;
+  PyObject *__pyx_codeobj__14;
+  PyObject *__pyx_codeobj__16;
+  PyObject *__pyx_codeobj__18;
+  PyObject *__pyx_codeobj__20;
+  PyObject *__pyx_codeobj__22;
+  PyObject *__pyx_codeobj__24;
+  PyObject *__pyx_codeobj__26;
+  PyObject *__pyx_codeobj__28;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2515,137 +2588,178 @@
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_8aixhello_6xyello_xyellw);
   Py_CLEAR(clear_module_state->__pyx_type_8aixhello_6xyello_xyellw);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_);
   Py_CLEAR(clear_module_state->__pyx_n_s_AES);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Access_Control_Request_Headers);
   Py_CLEAR(clear_module_state->__pyx_n_s_CBC);
   Py_CLEAR(clear_module_state->__pyx_n_s_Cipher);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Content_Type);
   Py_CLEAR(clear_module_state->__pyx_n_s_Decenigma);
   Py_CLEAR(clear_module_state->__pyx_n_s_Decipherx);
   Py_CLEAR(clear_module_state->__pyx_n_s_Embedshroud);
   Py_CLEAR(clear_module_state->__pyx_n_s_Encapseal);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
-  Py_CLEAR(clear_module_state->__pyx_n_s__18);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__2);
-  Py_CLEAR(clear_module_state->__pyx_n_s__3);
+  Py_CLEAR(clear_module_state->__pyx_n_s_SaveToMongoDb);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__12);
+  Py_CLEAR(clear_module_state->__pyx_n_s__29);
+  Py_CLEAR(clear_module_state->__pyx_n_s__9);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__9);
   Py_CLEAR(clear_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_CLEAR(clear_module_state->__pyx_n_s_aixhello_xyello);
   Py_CLEAR(clear_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithms);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_key);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_api_key_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_url);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_application_json);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_application_pdf);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_b64decode);
   Py_CLEAR(clear_module_state->__pyx_n_s_b64encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_backend);
   Py_CLEAR(clear_module_state->__pyx_n_s_base64);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn);
   Py_CLEAR(clear_module_state->__pyx_n_s_chr);
   Py_CLEAR(clear_module_state->__pyx_n_s_chunk);
   Py_CLEAR(clear_module_state->__pyx_n_s_cipher);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_u_collection);
   Py_CLEAR(clear_module_state->__pyx_n_s_create);
   Py_CLEAR(clear_module_state->__pyx_n_s_cryptography_hazmat_backends);
   Py_CLEAR(clear_module_state->__pyx_n_s_cryptography_hazmat_primitives_c);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
+  Py_CLEAR(clear_module_state->__pyx_n_u_dataSource);
+  Py_CLEAR(clear_module_state->__pyx_n_u_database);
   Py_CLEAR(clear_module_state->__pyx_n_s_decode);
   Py_CLEAR(clear_module_state->__pyx_n_s_decoded_encryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_decryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_decrypted_padded_text);
+  Py_CLEAR(clear_module_state->__pyx_n_s_decrypted_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_decryptor);
   Py_CLEAR(clear_module_state->__pyx_n_s_default_backend);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict_2);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
   Py_CLEAR(clear_module_state->__pyx_n_s_embedding);
   Py_CLEAR(clear_module_state->__pyx_n_s_embeddings);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
+  Py_CLEAR(clear_module_state->__pyx_n_u_enckyc);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_encoded_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptor);
+  Py_CLEAR(clear_module_state->__pyx_n_u_extracted_text);
+  Py_CLEAR(clear_module_state->__pyx_n_u_file_data);
+  Py_CLEAR(clear_module_state->__pyx_n_u_file_type);
+  Py_CLEAR(clear_module_state->__pyx_n_u_filename);
+  Py_CLEAR(clear_module_state->__pyx_n_u_filter);
   Py_CLEAR(clear_module_state->__pyx_n_s_finalize);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_get);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
+  Py_CLEAR(clear_module_state->__pyx_n_s_headers);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
   Py_CLEAR(clear_module_state->__pyx_n_s_input);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_iv);
+  Py_CLEAR(clear_module_state->__pyx_n_s_json);
   Py_CLEAR(clear_module_state->__pyx_n_s_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_u_message);
   Py_CLEAR(clear_module_state->__pyx_n_s_model);
   Py_CLEAR(clear_module_state->__pyx_n_s_modes);
   Py_CLEAR(clear_module_state->__pyx_n_s_msg);
   Py_CLEAR(clear_module_state->__pyx_n_s_mth);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_n_s_openai);
   Py_CLEAR(clear_module_state->__pyx_n_s_pad_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_padded_text);
+  Py_CLEAR(clear_module_state->__pyx_n_s_params_dict);
+  Py_CLEAR(clear_module_state->__pyx_n_s_payload);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
   Py_CLEAR(clear_module_state->__pyx_n_s_post);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_xyellw);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_requests);
   Py_CLEAR(clear_module_state->__pyx_n_s_response);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_set);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_state);
+  Py_CLEAR(clear_module_state->__pyx_n_s_status_code);
   Py_CLEAR(clear_module_state->__pyx_n_s_strText);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_text_chunks);
   Py_CLEAR(clear_module_state->__pyx_kp_u_text_embedding_ada_002);
+  Py_CLEAR(clear_module_state->__pyx_n_u_text_embeddings);
   Py_CLEAR(clear_module_state->__pyx_n_s_text_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
+  Py_CLEAR(clear_module_state->__pyx_n_u_update);
+  Py_CLEAR(clear_module_state->__pyx_n_u_upsert);
   Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decipherx);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Embedshroud);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Encapseal);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_SaveToMongoDb);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
+  Py_CLEAR(clear_module_state->__pyx_int_200);
   Py_CLEAR(clear_module_state->__pyx_int_222419149);
   Py_CLEAR(clear_module_state->__pyx_int_228825662);
   Py_CLEAR(clear_module_state->__pyx_int_238750788);
-  Py_CLEAR(clear_module_state->__pyx_tuple_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__2);
+  Py_CLEAR(clear_module_state->__pyx_tuple__3);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
+  Py_CLEAR(clear_module_state->__pyx_tuple__5);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  Py_CLEAR(clear_module_state->__pyx_tuple__7);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__10);
-  Py_CLEAR(clear_module_state->__pyx_tuple__12);
-  Py_CLEAR(clear_module_state->__pyx_tuple__14);
-  Py_CLEAR(clear_module_state->__pyx_tuple__16);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__5);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__7);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__9);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__11);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__15);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
+  Py_CLEAR(clear_module_state->__pyx_tuple__11);
+  Py_CLEAR(clear_module_state->__pyx_tuple__13);
+  Py_CLEAR(clear_module_state->__pyx_tuple__15);
+  Py_CLEAR(clear_module_state->__pyx_tuple__17);
+  Py_CLEAR(clear_module_state->__pyx_tuple__19);
+  Py_CLEAR(clear_module_state->__pyx_tuple__21);
+  Py_CLEAR(clear_module_state->__pyx_tuple__23);
+  Py_CLEAR(clear_module_state->__pyx_tuple__25);
+  Py_CLEAR(clear_module_state->__pyx_tuple__27);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__14);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__16);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__18);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__20);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__22);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__26);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__28);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -2660,137 +2774,178 @@
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_8aixhello_6xyello_xyellw);
   Py_VISIT(traverse_module_state->__pyx_type_8aixhello_6xyello_xyellw);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_);
   Py_VISIT(traverse_module_state->__pyx_n_s_AES);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Access_Control_Request_Headers);
   Py_VISIT(traverse_module_state->__pyx_n_s_CBC);
   Py_VISIT(traverse_module_state->__pyx_n_s_Cipher);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Content_Type);
   Py_VISIT(traverse_module_state->__pyx_n_s_Decenigma);
   Py_VISIT(traverse_module_state->__pyx_n_s_Decipherx);
   Py_VISIT(traverse_module_state->__pyx_n_s_Embedshroud);
   Py_VISIT(traverse_module_state->__pyx_n_s_Encapseal);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
-  Py_VISIT(traverse_module_state->__pyx_n_s__18);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__2);
-  Py_VISIT(traverse_module_state->__pyx_n_s__3);
+  Py_VISIT(traverse_module_state->__pyx_n_s_SaveToMongoDb);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__12);
+  Py_VISIT(traverse_module_state->__pyx_n_s__29);
+  Py_VISIT(traverse_module_state->__pyx_n_s__9);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__9);
   Py_VISIT(traverse_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_VISIT(traverse_module_state->__pyx_n_s_aixhello_xyello);
   Py_VISIT(traverse_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithms);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_key);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_api_key_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_url);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_application_json);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_application_pdf);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_b64decode);
   Py_VISIT(traverse_module_state->__pyx_n_s_b64encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_backend);
   Py_VISIT(traverse_module_state->__pyx_n_s_base64);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn);
   Py_VISIT(traverse_module_state->__pyx_n_s_chr);
   Py_VISIT(traverse_module_state->__pyx_n_s_chunk);
   Py_VISIT(traverse_module_state->__pyx_n_s_cipher);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_u_collection);
   Py_VISIT(traverse_module_state->__pyx_n_s_create);
   Py_VISIT(traverse_module_state->__pyx_n_s_cryptography_hazmat_backends);
   Py_VISIT(traverse_module_state->__pyx_n_s_cryptography_hazmat_primitives_c);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
+  Py_VISIT(traverse_module_state->__pyx_n_u_dataSource);
+  Py_VISIT(traverse_module_state->__pyx_n_u_database);
   Py_VISIT(traverse_module_state->__pyx_n_s_decode);
   Py_VISIT(traverse_module_state->__pyx_n_s_decoded_encryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_decryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_decrypted_padded_text);
+  Py_VISIT(traverse_module_state->__pyx_n_s_decrypted_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_decryptor);
   Py_VISIT(traverse_module_state->__pyx_n_s_default_backend);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict_2);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
   Py_VISIT(traverse_module_state->__pyx_n_s_embedding);
   Py_VISIT(traverse_module_state->__pyx_n_s_embeddings);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
+  Py_VISIT(traverse_module_state->__pyx_n_u_enckyc);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_encoded_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptor);
+  Py_VISIT(traverse_module_state->__pyx_n_u_extracted_text);
+  Py_VISIT(traverse_module_state->__pyx_n_u_file_data);
+  Py_VISIT(traverse_module_state->__pyx_n_u_file_type);
+  Py_VISIT(traverse_module_state->__pyx_n_u_filename);
+  Py_VISIT(traverse_module_state->__pyx_n_u_filter);
   Py_VISIT(traverse_module_state->__pyx_n_s_finalize);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_get);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
+  Py_VISIT(traverse_module_state->__pyx_n_s_headers);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
   Py_VISIT(traverse_module_state->__pyx_n_s_input);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_iv);
+  Py_VISIT(traverse_module_state->__pyx_n_s_json);
   Py_VISIT(traverse_module_state->__pyx_n_s_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_u_message);
   Py_VISIT(traverse_module_state->__pyx_n_s_model);
   Py_VISIT(traverse_module_state->__pyx_n_s_modes);
   Py_VISIT(traverse_module_state->__pyx_n_s_msg);
   Py_VISIT(traverse_module_state->__pyx_n_s_mth);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_n_s_openai);
   Py_VISIT(traverse_module_state->__pyx_n_s_pad_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_padded_text);
+  Py_VISIT(traverse_module_state->__pyx_n_s_params_dict);
+  Py_VISIT(traverse_module_state->__pyx_n_s_payload);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
   Py_VISIT(traverse_module_state->__pyx_n_s_post);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_xyellw);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_requests);
   Py_VISIT(traverse_module_state->__pyx_n_s_response);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_set);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_state);
+  Py_VISIT(traverse_module_state->__pyx_n_s_status_code);
   Py_VISIT(traverse_module_state->__pyx_n_s_strText);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_text_chunks);
   Py_VISIT(traverse_module_state->__pyx_kp_u_text_embedding_ada_002);
+  Py_VISIT(traverse_module_state->__pyx_n_u_text_embeddings);
   Py_VISIT(traverse_module_state->__pyx_n_s_text_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
+  Py_VISIT(traverse_module_state->__pyx_n_u_update);
+  Py_VISIT(traverse_module_state->__pyx_n_u_upsert);
   Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decipherx);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Embedshroud);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Encapseal);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_SaveToMongoDb);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
+  Py_VISIT(traverse_module_state->__pyx_int_200);
   Py_VISIT(traverse_module_state->__pyx_int_222419149);
   Py_VISIT(traverse_module_state->__pyx_int_228825662);
   Py_VISIT(traverse_module_state->__pyx_int_238750788);
-  Py_VISIT(traverse_module_state->__pyx_tuple_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__2);
+  Py_VISIT(traverse_module_state->__pyx_tuple__3);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
+  Py_VISIT(traverse_module_state->__pyx_tuple__5);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  Py_VISIT(traverse_module_state->__pyx_tuple__7);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__10);
-  Py_VISIT(traverse_module_state->__pyx_tuple__12);
-  Py_VISIT(traverse_module_state->__pyx_tuple__14);
-  Py_VISIT(traverse_module_state->__pyx_tuple__16);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__5);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__7);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__9);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__11);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__15);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
+  Py_VISIT(traverse_module_state->__pyx_tuple__11);
+  Py_VISIT(traverse_module_state->__pyx_tuple__13);
+  Py_VISIT(traverse_module_state->__pyx_tuple__15);
+  Py_VISIT(traverse_module_state->__pyx_tuple__17);
+  Py_VISIT(traverse_module_state->__pyx_tuple__19);
+  Py_VISIT(traverse_module_state->__pyx_tuple__21);
+  Py_VISIT(traverse_module_state->__pyx_tuple__23);
+  Py_VISIT(traverse_module_state->__pyx_tuple__25);
+  Py_VISIT(traverse_module_state->__pyx_tuple__27);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__14);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__16);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__18);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__20);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__22);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__26);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__28);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -2815,137 +2970,178 @@
 #ifdef __Pyx_Coroutine_USED
 #define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
 #endif
 #if CYTHON_USE_MODULE_STATE
 #define __pyx_type_8aixhello_6xyello_xyellw __pyx_mstate_global->__pyx_type_8aixhello_6xyello_xyellw
 #endif
 #define __pyx_ptype_8aixhello_6xyello_xyellw __pyx_mstate_global->__pyx_ptype_8aixhello_6xyello_xyellw
+#define __pyx_kp_u_ __pyx_mstate_global->__pyx_kp_u_
 #define __pyx_n_s_AES __pyx_mstate_global->__pyx_n_s_AES
+#define __pyx_kp_u_Access_Control_Request_Headers __pyx_mstate_global->__pyx_kp_u_Access_Control_Request_Headers
 #define __pyx_n_s_CBC __pyx_mstate_global->__pyx_n_s_CBC
 #define __pyx_n_s_Cipher __pyx_mstate_global->__pyx_n_s_Cipher
+#define __pyx_kp_u_Content_Type __pyx_mstate_global->__pyx_kp_u_Content_Type
 #define __pyx_n_s_Decenigma __pyx_mstate_global->__pyx_n_s_Decenigma
 #define __pyx_n_s_Decipherx __pyx_mstate_global->__pyx_n_s_Decipherx
 #define __pyx_n_s_Embedshroud __pyx_mstate_global->__pyx_n_s_Embedshroud
 #define __pyx_n_s_Encapseal __pyx_mstate_global->__pyx_n_s_Encapseal
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN __pyx_mstate_global->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
-#define __pyx_n_s__18 __pyx_mstate_global->__pyx_n_s__18
-#define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
-#define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
+#define __pyx_n_s_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_SaveToMongoDb
+#define __pyx_kp_u__12 __pyx_mstate_global->__pyx_kp_u__12
+#define __pyx_n_s__29 __pyx_mstate_global->__pyx_n_s__29
+#define __pyx_n_s__9 __pyx_mstate_global->__pyx_n_s__9
+#define __pyx_kp_u__9 __pyx_mstate_global->__pyx_kp_u__9
 #define __pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1 __pyx_mstate_global->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1
 #define __pyx_n_s_aixhello_xyello __pyx_mstate_global->__pyx_n_s_aixhello_xyello
 #define __pyx_kp_s_aixhello_xyello_pyx __pyx_mstate_global->__pyx_kp_s_aixhello_xyello_pyx
 #define __pyx_n_s_algorithms __pyx_mstate_global->__pyx_n_s_algorithms
 #define __pyx_n_s_api_key __pyx_mstate_global->__pyx_n_s_api_key
+#define __pyx_kp_u_api_key_2 __pyx_mstate_global->__pyx_kp_u_api_key_2
 #define __pyx_n_s_api_url __pyx_mstate_global->__pyx_n_s_api_url
+#define __pyx_kp_u_application_json __pyx_mstate_global->__pyx_kp_u_application_json
+#define __pyx_kp_u_application_pdf __pyx_mstate_global->__pyx_kp_u_application_pdf
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_b64decode __pyx_mstate_global->__pyx_n_s_b64decode
 #define __pyx_n_s_b64encode __pyx_mstate_global->__pyx_n_s_b64encode
 #define __pyx_n_s_backend __pyx_mstate_global->__pyx_n_s_backend
 #define __pyx_n_s_base64 __pyx_mstate_global->__pyx_n_s_base64
+#define __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn __pyx_mstate_global->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn
 #define __pyx_n_s_chr __pyx_mstate_global->__pyx_n_s_chr
 #define __pyx_n_s_chunk __pyx_mstate_global->__pyx_n_s_chunk
 #define __pyx_n_s_cipher __pyx_mstate_global->__pyx_n_s_cipher
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_u_collection __pyx_mstate_global->__pyx_n_u_collection
 #define __pyx_n_s_create __pyx_mstate_global->__pyx_n_s_create
 #define __pyx_n_s_cryptography_hazmat_backends __pyx_mstate_global->__pyx_n_s_cryptography_hazmat_backends
 #define __pyx_n_s_cryptography_hazmat_primitives_c __pyx_mstate_global->__pyx_n_s_cryptography_hazmat_primitives_c
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
+#define __pyx_n_u_dataSource __pyx_mstate_global->__pyx_n_u_dataSource
+#define __pyx_n_u_database __pyx_mstate_global->__pyx_n_u_database
 #define __pyx_n_s_decode __pyx_mstate_global->__pyx_n_s_decode
 #define __pyx_n_s_decoded_encryptedText __pyx_mstate_global->__pyx_n_s_decoded_encryptedText
 #define __pyx_n_s_decryptedText __pyx_mstate_global->__pyx_n_s_decryptedText
 #define __pyx_n_s_decrypted_padded_text __pyx_mstate_global->__pyx_n_s_decrypted_padded_text
+#define __pyx_n_s_decrypted_url __pyx_mstate_global->__pyx_n_s_decrypted_url
 #define __pyx_n_s_decryptor __pyx_mstate_global->__pyx_n_s_decryptor
 #define __pyx_n_s_default_backend __pyx_mstate_global->__pyx_n_s_default_backend
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_dict_2 __pyx_mstate_global->__pyx_n_s_dict_2
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
 #define __pyx_n_s_embedding __pyx_mstate_global->__pyx_n_s_embedding
 #define __pyx_n_s_embeddings __pyx_mstate_global->__pyx_n_s_embeddings
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
+#define __pyx_n_u_enckyc __pyx_mstate_global->__pyx_n_u_enckyc
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_encoded_url __pyx_mstate_global->__pyx_n_s_encoded_url
 #define __pyx_n_s_encryptedText __pyx_mstate_global->__pyx_n_s_encryptedText
 #define __pyx_n_s_encryptor __pyx_mstate_global->__pyx_n_s_encryptor
+#define __pyx_n_u_extracted_text __pyx_mstate_global->__pyx_n_u_extracted_text
+#define __pyx_n_u_file_data __pyx_mstate_global->__pyx_n_u_file_data
+#define __pyx_n_u_file_type __pyx_mstate_global->__pyx_n_u_file_type
+#define __pyx_n_u_filename __pyx_mstate_global->__pyx_n_u_filename
+#define __pyx_n_u_filter __pyx_mstate_global->__pyx_n_u_filter
 #define __pyx_n_s_finalize __pyx_mstate_global->__pyx_n_s_finalize
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
+#define __pyx_n_s_get __pyx_mstate_global->__pyx_n_s_get
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
+#define __pyx_n_s_headers __pyx_mstate_global->__pyx_n_s_headers
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
 #define __pyx_n_s_input __pyx_mstate_global->__pyx_n_s_input
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_iv __pyx_mstate_global->__pyx_n_s_iv
+#define __pyx_n_s_json __pyx_mstate_global->__pyx_n_s_json
 #define __pyx_n_s_key __pyx_mstate_global->__pyx_n_s_key
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_u_message __pyx_mstate_global->__pyx_n_u_message
 #define __pyx_n_s_model __pyx_mstate_global->__pyx_n_s_model
 #define __pyx_n_s_modes __pyx_mstate_global->__pyx_n_s_modes
 #define __pyx_n_s_msg __pyx_mstate_global->__pyx_n_s_msg
 #define __pyx_n_s_mth __pyx_mstate_global->__pyx_n_s_mth
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_n_s_openai __pyx_mstate_global->__pyx_n_s_openai
 #define __pyx_n_s_pad_length __pyx_mstate_global->__pyx_n_s_pad_length
 #define __pyx_n_s_padded_text __pyx_mstate_global->__pyx_n_s_padded_text
+#define __pyx_n_s_params_dict __pyx_mstate_global->__pyx_n_s_params_dict
+#define __pyx_n_s_payload __pyx_mstate_global->__pyx_n_s_payload
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
 #define __pyx_n_s_post __pyx_mstate_global->__pyx_n_s_post
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
 #define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
 #define __pyx_n_s_pyx_unpickle_xyellw __pyx_mstate_global->__pyx_n_s_pyx_unpickle_xyellw
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_requests __pyx_mstate_global->__pyx_n_s_requests
 #define __pyx_n_s_response __pyx_mstate_global->__pyx_n_s_response
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
+#define __pyx_kp_u_set __pyx_mstate_global->__pyx_kp_u_set
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_state __pyx_mstate_global->__pyx_n_s_state
+#define __pyx_n_s_status_code __pyx_mstate_global->__pyx_n_s_status_code
 #define __pyx_n_s_strText __pyx_mstate_global->__pyx_n_s_strText
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_text __pyx_mstate_global->__pyx_n_s_text
 #define __pyx_n_s_text_chunks __pyx_mstate_global->__pyx_n_s_text_chunks
 #define __pyx_kp_u_text_embedding_ada_002 __pyx_mstate_global->__pyx_kp_u_text_embedding_ada_002
+#define __pyx_n_u_text_embeddings __pyx_mstate_global->__pyx_n_u_text_embeddings
 #define __pyx_n_s_text_key __pyx_mstate_global->__pyx_n_s_text_key
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
+#define __pyx_n_u_update __pyx_mstate_global->__pyx_n_u_update
+#define __pyx_n_u_upsert __pyx_mstate_global->__pyx_n_u_upsert
 #define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_n_s_xyellw __pyx_mstate_global->__pyx_n_s_xyellw
 #define __pyx_n_s_xyellw_Decenigma __pyx_mstate_global->__pyx_n_s_xyellw_Decenigma
 #define __pyx_n_s_xyellw_Decipherx __pyx_mstate_global->__pyx_n_s_xyellw_Decipherx
 #define __pyx_n_s_xyellw_Embedshroud __pyx_mstate_global->__pyx_n_s_xyellw_Embedshroud
 #define __pyx_n_s_xyellw_Encapseal __pyx_mstate_global->__pyx_n_s_xyellw_Encapseal
+#define __pyx_n_s_xyellw_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_xyellw_SaveToMongoDb
 #define __pyx_n_s_xyellw___reduce_cython __pyx_mstate_global->__pyx_n_s_xyellw___reduce_cython
 #define __pyx_n_s_xyellw___setstate_cython __pyx_mstate_global->__pyx_n_s_xyellw___setstate_cython
 #define __pyx_kp_b_y1c8_8BxP9XN_VKM __pyx_mstate_global->__pyx_kp_b_y1c8_8BxP9XN_VKM
+#define __pyx_int_200 __pyx_mstate_global->__pyx_int_200
 #define __pyx_int_222419149 __pyx_mstate_global->__pyx_int_222419149
 #define __pyx_int_228825662 __pyx_mstate_global->__pyx_int_228825662
 #define __pyx_int_238750788 __pyx_mstate_global->__pyx_int_238750788
-#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
+#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
+#define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
+#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
-#define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
-#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
-#define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
-#define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
-#define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
-#define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
-#define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
-#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
-#define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
-#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
+#define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
+#define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
+#define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
+#define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
+#define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
+#define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
+#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
+#define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
+#define __pyx_tuple__27 __pyx_mstate_global->__pyx_tuple__27
+#define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
+#define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
+#define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
+#define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
+#define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
+#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
+#define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
+#define __pyx_codeobj__28 __pyx_mstate_global->__pyx_codeobj__28
 /* #### Code section: module_code ### */
 
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -4267,23 +4463,353 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9SaveToMongoDb(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_9SaveToMongoDb = {"SaveToMongoDb", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9SaveToMongoDb, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9SaveToMongoDb(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_params_dict = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("SaveToMongoDb (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_params_dict,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_params_dict)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "SaveToMongoDb") < 0)) __PYX_ERR(0, 60, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_params_dict = values[0];
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 60, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.SaveToMongoDb", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_params_dict);
+
+  /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_params_dict) {
+  PyObject *__pyx_v_decrypted_url = NULL;
+  PyObject *__pyx_v_payload = NULL;
+  PyObject *__pyx_v_headers = NULL;
+  PyObject *__pyx_v_response = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("SaveToMongoDb", 1);
+
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
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
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_v_decrypted_url = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_collection, __pyx_t_3) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_database, __pyx_t_2) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_dataSource, __pyx_t_3) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_filename, __pyx_t_5) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filter, __pyx_t_3) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_filename, __pyx_t_6) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_data, __pyx_t_2) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_type, __pyx_kp_u_application_pdf) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_extracted_text, __pyx_t_6) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_text_embeddings, __pyx_t_2) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_set, __pyx_t_5) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_update, __pyx_t_3) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_upsert, Py_True) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_v_payload = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__9) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_t_5) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_v_headers = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_requests); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_v_decrypted_url);
+  __Pyx_GIVEREF(__pyx_v_decrypted_url);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_decrypted_url)) __PYX_ERR(0, 85, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_json, __pyx_v_payload) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_response = __pyx_t_2;
+  __pyx_t_2 = 0;
+
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_2, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__pyx_t_7) {
+
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = NULL;
+    __pyx_t_4 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_1)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_1);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_4 = 1;
+      }
+    }
+    #endif
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
+    __pyx_r = __pyx_t_2;
+    __pyx_t_2 = 0;
+    goto __pyx_L0;
+
+  }
+
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_r = __pyx_t_2;
+    __pyx_t_2 = 0;
+    goto __pyx_L0;
+  }
+
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.SaveToMongoDb", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_decrypted_url);
+  __Pyx_XDECREF(__pyx_v_payload);
+  __Pyx_XDECREF(__pyx_v_headers);
+  __Pyx_XDECREF(__pyx_v_response);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_9__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9__reduce_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_11__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -4300,22 +4826,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_8__reduce_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_10__reduce_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
@@ -4433,23 +4959,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_11__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11__setstate_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_13__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_state = 0;
@@ -4515,28 +5041,28 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_10__setstate_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_12__setstate_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v___pyx_state);
 
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
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 1);
@@ -4700,15 +5226,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_xyellw", 1);
 
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple_, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__11, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
@@ -4915,16 +5441,17 @@
 }
 
 static PyMethodDef __pyx_methods_8aixhello_6xyello_xyellw[] = {
   {"Decipherx", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"Encapseal", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"Decenigma", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"Embedshroud", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"SaveToMongoDb", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9SaveToMongoDb, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
 static PyType_Slot __pyx_type_8aixhello_6xyello_xyellw_slots[] = {
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8aixhello_6xyello_xyellw},
   {Py_tp_methods, (void *)__pyx_methods_8aixhello_6xyello_xyellw},
   {Py_tp_new, (void *)__pyx_tp_new_8aixhello_6xyello_xyellw},
@@ -5033,116 +5560,146 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
     {&__pyx_n_s_AES, __pyx_k_AES, sizeof(__pyx_k_AES), 0, 0, 1, 1},
+    {&__pyx_kp_u_Access_Control_Request_Headers, __pyx_k_Access_Control_Request_Headers, sizeof(__pyx_k_Access_Control_Request_Headers), 0, 1, 0, 0},
     {&__pyx_n_s_CBC, __pyx_k_CBC, sizeof(__pyx_k_CBC), 0, 0, 1, 1},
     {&__pyx_n_s_Cipher, __pyx_k_Cipher, sizeof(__pyx_k_Cipher), 0, 0, 1, 1},
+    {&__pyx_kp_u_Content_Type, __pyx_k_Content_Type, sizeof(__pyx_k_Content_Type), 0, 1, 0, 0},
     {&__pyx_n_s_Decenigma, __pyx_k_Decenigma, sizeof(__pyx_k_Decenigma), 0, 0, 1, 1},
     {&__pyx_n_s_Decipherx, __pyx_k_Decipherx, sizeof(__pyx_k_Decipherx), 0, 0, 1, 1},
     {&__pyx_n_s_Embedshroud, __pyx_k_Embedshroud, sizeof(__pyx_k_Embedshroud), 0, 0, 1, 1},
     {&__pyx_n_s_Encapseal, __pyx_k_Encapseal, sizeof(__pyx_k_Encapseal), 0, 0, 1, 1},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, sizeof(__pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN), 0, 0, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-    {&__pyx_n_s__18, __pyx_k__18, sizeof(__pyx_k__18), 0, 0, 1, 1},
-    {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-    {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
+    {&__pyx_n_s_SaveToMongoDb, __pyx_k_SaveToMongoDb, sizeof(__pyx_k_SaveToMongoDb), 0, 0, 1, 1},
+    {&__pyx_kp_u__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 1, 0, 0},
+    {&__pyx_n_s__29, __pyx_k__29, sizeof(__pyx_k__29), 0, 0, 1, 1},
+    {&__pyx_n_s__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 0, 1, 1},
+    {&__pyx_kp_u__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 1, 0, 0},
     {&__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, sizeof(__pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1), 0, 1, 0, 1},
     {&__pyx_n_s_aixhello_xyello, __pyx_k_aixhello_xyello, sizeof(__pyx_k_aixhello_xyello), 0, 0, 1, 1},
     {&__pyx_kp_s_aixhello_xyello_pyx, __pyx_k_aixhello_xyello_pyx, sizeof(__pyx_k_aixhello_xyello_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_algorithms, __pyx_k_algorithms, sizeof(__pyx_k_algorithms), 0, 0, 1, 1},
     {&__pyx_n_s_api_key, __pyx_k_api_key, sizeof(__pyx_k_api_key), 0, 0, 1, 1},
+    {&__pyx_kp_u_api_key_2, __pyx_k_api_key_2, sizeof(__pyx_k_api_key_2), 0, 1, 0, 0},
     {&__pyx_n_s_api_url, __pyx_k_api_url, sizeof(__pyx_k_api_url), 0, 0, 1, 1},
+    {&__pyx_kp_u_application_json, __pyx_k_application_json, sizeof(__pyx_k_application_json), 0, 1, 0, 0},
+    {&__pyx_kp_u_application_pdf, __pyx_k_application_pdf, sizeof(__pyx_k_application_pdf), 0, 1, 0, 0},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_b64decode, __pyx_k_b64decode, sizeof(__pyx_k_b64decode), 0, 0, 1, 1},
     {&__pyx_n_s_b64encode, __pyx_k_b64encode, sizeof(__pyx_k_b64encode), 0, 0, 1, 1},
     {&__pyx_n_s_backend, __pyx_k_backend, sizeof(__pyx_k_backend), 0, 0, 1, 1},
     {&__pyx_n_s_base64, __pyx_k_base64, sizeof(__pyx_k_base64), 0, 0, 1, 1},
+    {&__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn, __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn, sizeof(__pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn), 0, 1, 0, 0},
     {&__pyx_n_s_chr, __pyx_k_chr, sizeof(__pyx_k_chr), 0, 0, 1, 1},
     {&__pyx_n_s_chunk, __pyx_k_chunk, sizeof(__pyx_k_chunk), 0, 0, 1, 1},
     {&__pyx_n_s_cipher, __pyx_k_cipher, sizeof(__pyx_k_cipher), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_u_collection, __pyx_k_collection, sizeof(__pyx_k_collection), 0, 1, 0, 1},
     {&__pyx_n_s_create, __pyx_k_create, sizeof(__pyx_k_create), 0, 0, 1, 1},
     {&__pyx_n_s_cryptography_hazmat_backends, __pyx_k_cryptography_hazmat_backends, sizeof(__pyx_k_cryptography_hazmat_backends), 0, 0, 1, 1},
     {&__pyx_n_s_cryptography_hazmat_primitives_c, __pyx_k_cryptography_hazmat_primitives_c, sizeof(__pyx_k_cryptography_hazmat_primitives_c), 0, 0, 1, 1},
     {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
+    {&__pyx_n_u_dataSource, __pyx_k_dataSource, sizeof(__pyx_k_dataSource), 0, 1, 0, 1},
+    {&__pyx_n_u_database, __pyx_k_database, sizeof(__pyx_k_database), 0, 1, 0, 1},
     {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
     {&__pyx_n_s_decoded_encryptedText, __pyx_k_decoded_encryptedText, sizeof(__pyx_k_decoded_encryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_decryptedText, __pyx_k_decryptedText, sizeof(__pyx_k_decryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_decrypted_padded_text, __pyx_k_decrypted_padded_text, sizeof(__pyx_k_decrypted_padded_text), 0, 0, 1, 1},
+    {&__pyx_n_s_decrypted_url, __pyx_k_decrypted_url, sizeof(__pyx_k_decrypted_url), 0, 0, 1, 1},
     {&__pyx_n_s_decryptor, __pyx_k_decryptor, sizeof(__pyx_k_decryptor), 0, 0, 1, 1},
     {&__pyx_n_s_default_backend, __pyx_k_default_backend, sizeof(__pyx_k_default_backend), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_n_s_dict_2, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
     {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
     {&__pyx_n_s_embedding, __pyx_k_embedding, sizeof(__pyx_k_embedding), 0, 0, 1, 1},
     {&__pyx_n_s_embeddings, __pyx_k_embeddings, sizeof(__pyx_k_embeddings), 0, 0, 1, 1},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
+    {&__pyx_n_u_enckyc, __pyx_k_enckyc, sizeof(__pyx_k_enckyc), 0, 1, 0, 1},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_encoded_url, __pyx_k_encoded_url, sizeof(__pyx_k_encoded_url), 0, 0, 1, 1},
     {&__pyx_n_s_encryptedText, __pyx_k_encryptedText, sizeof(__pyx_k_encryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_encryptor, __pyx_k_encryptor, sizeof(__pyx_k_encryptor), 0, 0, 1, 1},
+    {&__pyx_n_u_extracted_text, __pyx_k_extracted_text, sizeof(__pyx_k_extracted_text), 0, 1, 0, 1},
+    {&__pyx_n_u_file_data, __pyx_k_file_data, sizeof(__pyx_k_file_data), 0, 1, 0, 1},
+    {&__pyx_n_u_file_type, __pyx_k_file_type, sizeof(__pyx_k_file_type), 0, 1, 0, 1},
+    {&__pyx_n_u_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 1, 0, 1},
+    {&__pyx_n_u_filter, __pyx_k_filter, sizeof(__pyx_k_filter), 0, 1, 0, 1},
     {&__pyx_n_s_finalize, __pyx_k_finalize, sizeof(__pyx_k_finalize), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
+    {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+    {&__pyx_n_s_headers, __pyx_k_headers, sizeof(__pyx_k_headers), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
     {&__pyx_n_s_input, __pyx_k_input, sizeof(__pyx_k_input), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_iv, __pyx_k_iv, sizeof(__pyx_k_iv), 0, 0, 1, 1},
+    {&__pyx_n_s_json, __pyx_k_json, sizeof(__pyx_k_json), 0, 0, 1, 1},
     {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_u_message, __pyx_k_message, sizeof(__pyx_k_message), 0, 1, 0, 1},
     {&__pyx_n_s_model, __pyx_k_model, sizeof(__pyx_k_model), 0, 0, 1, 1},
     {&__pyx_n_s_modes, __pyx_k_modes, sizeof(__pyx_k_modes), 0, 0, 1, 1},
     {&__pyx_n_s_msg, __pyx_k_msg, sizeof(__pyx_k_msg), 0, 0, 1, 1},
     {&__pyx_n_s_mth, __pyx_k_mth, sizeof(__pyx_k_mth), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_n_s_openai, __pyx_k_openai, sizeof(__pyx_k_openai), 0, 0, 1, 1},
     {&__pyx_n_s_pad_length, __pyx_k_pad_length, sizeof(__pyx_k_pad_length), 0, 0, 1, 1},
     {&__pyx_n_s_padded_text, __pyx_k_padded_text, sizeof(__pyx_k_padded_text), 0, 0, 1, 1},
+    {&__pyx_n_s_params_dict, __pyx_k_params_dict, sizeof(__pyx_k_params_dict), 0, 0, 1, 1},
+    {&__pyx_n_s_payload, __pyx_k_payload, sizeof(__pyx_k_payload), 0, 0, 1, 1},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
     {&__pyx_n_s_post, __pyx_k_post, sizeof(__pyx_k_post), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_xyellw, __pyx_k_pyx_unpickle_xyellw, sizeof(__pyx_k_pyx_unpickle_xyellw), 0, 0, 1, 1},
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
     {&__pyx_n_s_requests, __pyx_k_requests, sizeof(__pyx_k_requests), 0, 0, 1, 1},
     {&__pyx_n_s_response, __pyx_k_response, sizeof(__pyx_k_response), 0, 0, 1, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
+    {&__pyx_kp_u_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 1, 0, 0},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
+    {&__pyx_n_s_status_code, __pyx_k_status_code, sizeof(__pyx_k_status_code), 0, 0, 1, 1},
     {&__pyx_n_s_strText, __pyx_k_strText, sizeof(__pyx_k_strText), 0, 0, 1, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 0, 1, 1},
     {&__pyx_n_s_text_chunks, __pyx_k_text_chunks, sizeof(__pyx_k_text_chunks), 0, 0, 1, 1},
     {&__pyx_kp_u_text_embedding_ada_002, __pyx_k_text_embedding_ada_002, sizeof(__pyx_k_text_embedding_ada_002), 0, 1, 0, 0},
+    {&__pyx_n_u_text_embeddings, __pyx_k_text_embeddings, sizeof(__pyx_k_text_embeddings), 0, 1, 0, 1},
     {&__pyx_n_s_text_key, __pyx_k_text_key, sizeof(__pyx_k_text_key), 0, 0, 1, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
+    {&__pyx_n_u_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 1, 0, 1},
+    {&__pyx_n_u_upsert, __pyx_k_upsert, sizeof(__pyx_k_upsert), 0, 1, 0, 1},
     {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
     {&__pyx_n_s_xyellw, __pyx_k_xyellw, sizeof(__pyx_k_xyellw), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decenigma, __pyx_k_xyellw_Decenigma, sizeof(__pyx_k_xyellw_Decenigma), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decipherx, __pyx_k_xyellw_Decipherx, sizeof(__pyx_k_xyellw_Decipherx), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Embedshroud, __pyx_k_xyellw_Embedshroud, sizeof(__pyx_k_xyellw_Embedshroud), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Encapseal, __pyx_k_xyellw_Encapseal, sizeof(__pyx_k_xyellw_Encapseal), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_SaveToMongoDb, __pyx_k_xyellw_SaveToMongoDb, sizeof(__pyx_k_xyellw_SaveToMongoDb), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___reduce_cython, __pyx_k_xyellw___reduce_cython, sizeof(__pyx_k_xyellw___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___setstate_cython, __pyx_k_xyellw___setstate_cython, sizeof(__pyx_k_xyellw___setstate_cython), 0, 0, 1, 1},
     {&__pyx_kp_b_y1c8_8BxP9XN_VKM, __pyx_k_y1c8_8BxP9XN_VKM, sizeof(__pyx_k_y1c8_8BxP9XN_VKM), 0, 0, 0, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
@@ -5155,62 +5712,100 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  __pyx_tuple_ = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_u_collection, __pyx_kp_u_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_database, __pyx_kp_u_); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
-  __pyx_tuple__4 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_dataSource, __pyx_kp_u_); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 9, __pyx_L1_error)
 
-  __pyx_tuple__6 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_filename, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+
+  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_u_file_data, __pyx_kp_u_); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 16, __pyx_L1_error)
 
-  __pyx_tuple__8 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_u_extracted_text, __pyx_kp_u_); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+
+  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_u_text_embeddings, __pyx_kp_u_); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 31, __pyx_L1_error)
 
-  __pyx_tuple__10 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(2, __pyx_n_u_enckyc, __pyx_kp_u_); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Embedshroud, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 48, __pyx_L1_error)
 
-  __pyx_tuple__12 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(1, 1, __pyx_L1_error)
-
-  __pyx_tuple__14 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 16, __pyx_L1_error)
-
-  __pyx_tuple__16 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+
+  __pyx_tuple__13 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 9, __pyx_L1_error)
+
+  __pyx_tuple__15 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 16, __pyx_L1_error)
+
+  __pyx_tuple__17 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 31, __pyx_L1_error)
+
+  __pyx_tuple__19 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Embedshroud, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 48, __pyx_L1_error)
+
+  __pyx_tuple__21 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SaveToMongoDb, 60, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 60, __pyx_L1_error)
+
+  __pyx_tuple__23 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  __pyx_tuple__25 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(1, 16, __pyx_L1_error)
+
+  __pyx_tuple__27 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  __pyx_int_200 = PyInt_FromLong(200); if (unlikely(!__pyx_int_200)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_222419149 = PyInt_FromLong(222419149L); if (unlikely(!__pyx_int_222419149)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_228825662 = PyInt_FromLong(228825662L); if (unlikely(!__pyx_int_228825662)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_238750788 = PyInt_FromLong(238750788L); if (unlikely(!__pyx_int_238750788)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -5646,51 +6241,57 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_openai, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_openai, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decipherx, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Encapseal, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decenigma, __pyx_t_2) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Embedshroud, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Embedshroud, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Embedshroud, __pyx_t_2) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9SaveToMongoDb, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SaveToMongoDb, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_SaveToMongoDb, __pyx_t_2) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
+
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_xyellw, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -6914,14 +7515,86 @@
     if (likely(tp->tp_setattr))
         return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
 #endif
     return PyObject_SetAttr(obj, attr_name, value);
 }
 #endif
 
+/* PyIntCompare */
+static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace) {
+    CYTHON_MAYBE_UNUSED_VAR(intval);
+    CYTHON_UNUSED_VAR(inplace);
+    if (op1 == op2) {
+        return 1;
+    }
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_CheckExact(op1))) {
+        const long b = intval;
+        long a = PyInt_AS_LONG(op1);
+        return (a == b);
+    }
+    #endif
+    #if CYTHON_USE_PYLONG_INTERNALS
+    if (likely(PyLong_CheckExact(op1))) {
+        int unequal;
+        unsigned long uintval;
+        Py_ssize_t size = __Pyx_PyLong_DigitCount(op1);
+        const digit* digits = __Pyx_PyLong_Digits(op1);
+        if (intval == 0) {
+            return (__Pyx_PyLong_IsZero(op1) == 1);
+        } else if (intval < 0) {
+            if (__Pyx_PyLong_IsNonNeg(op1))
+                return 0;
+            intval = -intval;
+        } else {
+            if (__Pyx_PyLong_IsNeg(op1))
+                return 0;
+        }
+        uintval = (unsigned long) intval;
+#if PyLong_SHIFT * 4 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 4)) {
+            unequal = (size != 5) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[4] != ((uintval >> (4 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 3 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 3)) {
+            unequal = (size != 4) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 2 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 2)) {
+            unequal = (size != 3) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 1 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 1)) {
+            unequal = (size != 2) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+            unequal = (size != 1) || (((unsigned long) digits[0]) != (uintval & (unsigned long) PyLong_MASK));
+        return (unequal == 0);
+    }
+    #endif
+    if (PyFloat_CheckExact(op1)) {
+        const long b = intval;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        double a = __pyx_PyFloat_AsDouble(op1);
+#else
+        double a = PyFloat_AS_DOUBLE(op1);
+#endif
+        return ((double)a == (double)b);
+    }
+    return __Pyx_PyObject_IsTrueAndDecref(
+        PyObject_RichCompare(op1, op2, Py_EQ));
+}
+
 /* KeywordStringCheck */
 static int __Pyx_CheckKeywordStrings(
     PyObject *kw,
     const char* function_name,
     int kw_allowed)
 {
     PyObject* key = 0;
@@ -7102,15 +7775,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__2);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__12);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -7930,15 +8603,15 @@
         return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
     }
     return module;
 }
 #endif
 static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__3;
+    PyObject *module, *from_list, *star = __pyx_n_s__9;
     CYTHON_UNUSED_VAR(parts_tuple);
     from_list = PyList_New(1);
     if (unlikely(!from_list))
         return NULL;
     Py_INCREF(star);
     PyList_SET_ITEM(from_list, 0, star);
     module = __Pyx_Import(name, from_list, 0);
@@ -9843,15 +10516,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__18);
+        name = __Pyx_NewRef(__pyx_n_s__29);
     }
     return name;
 }
 #endif
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
```

### Comparing `aixhello-2.1/aixhello.egg-info/PKG-INFO` & `aixhello-2.2/aixhello.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 2.1
+Version: 2.2
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-2.1/setup.py` & `aixhello-2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='2.1',  # Increment the version number
+    version='2.2',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

