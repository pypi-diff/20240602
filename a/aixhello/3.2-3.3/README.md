# Comparing `tmp/aixhello-3.2.tar.gz` & `tmp/aixhello-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-3.2.tar", last modified: Sun Jun  2 02:59:26 2024, max compression
+gzip compressed data, was "aixhello-3.3.tar", last modified: Sun Jun  2 03:25:28 2024, max compression
```

## Comparing `aixhello-3.2.tar` & `aixhello-3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 02:59:26.740756 aixhello-3.2/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.2/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-02 02:59:26.740756 aixhello-3.2/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 02:59:26.710209 aixhello-3.2/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.2/aixhello/__init__.py
--rw-rw-rw-   0        0        0   590146 2024-06-02 02:59:17.000000 aixhello-3.2/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-02 02:59:26.739755 aixhello-3.2/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-02 02:59:26.000000 aixhello-3.2/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-02 02:59:26.000000 aixhello-3.2/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 02:59:26.000000 aixhello-3.2/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-02 02:59:26.000000 aixhello-3.2/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 02:59:26.000000 aixhello-3.2/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-02 02:59:26.742792 aixhello-3.2/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-02 02:56:21.000000 aixhello-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 03:25:28.923957 aixhello-3.3/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.3/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-02 03:25:28.922958 aixhello-3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 03:25:28.896556 aixhello-3.3/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.3/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   589974 2024-06-02 03:25:20.000000 aixhello-3.3/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-02 03:25:28.920544 aixhello-3.3/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-02 03:25:28.000000 aixhello-3.3/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-02 03:25:28.000000 aixhello-3.3/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 03:25:28.000000 aixhello-3.3/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-02 03:25:28.000000 aixhello-3.3/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 03:25:28.000000 aixhello-3.3/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-02 03:25:28.929971 aixhello-3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-02 03:24:43.000000 aixhello-3.3/setup.py
```

### Comparing `aixhello-3.2/LICENSE` & `aixhello-3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-3.2/PKG-INFO` & `aixhello-3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.2
+Version: 3.3
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.2/README.md` & `aixhello-3.3/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-3.2/aixhello/xyello.c` & `aixhello-3.3/aixhello/xyello.c`

 * *Files 0% similar despite different names*

```diff
@@ -2447,14 +2447,15 @@
 static const char __pyx_k_query_payload[] = "query_payload";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_response_data[] = "response_data";
 static const char __pyx_k_similar_score[] = "similar_score";
 static const char __pyx_k_vector_search[] = "vector_search";
 static const char __pyx_k_vectorizeText[] = "vectorizeText";
 static const char __pyx_k_extracted_text[] = "extracted_text";
+static const char __pyx_k_vectorizeEmbed[] = "vectorizeEmbed";
 static const char __pyx_k_aixhello_xyello[] = "aixhello.xyello";
 static const char __pyx_k_application_pdf[] = "application/pdf";
 static const char __pyx_k_default_backend[] = "default_backend";
 static const char __pyx_k_extracted_texts[] = "extracted_texts";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_text_embeddings[] = "text_embeddings";
@@ -2462,31 +2463,30 @@
 static const char __pyx_k_application_json[] = "application/json";
 static const char __pyx_k_xyellw_Decenigma[] = "xyellw.Decenigma";
 static const char __pyx_k_xyellw_Decipherx[] = "xyellw.Decipherx";
 static const char __pyx_k_xyellw_Encapseal[] = "xyellw.Encapseal";
 static const char __pyx_k_y1c8_8BxP9XN_VKM[] = "y1c8@8BxP9XN#VKM";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_vectorizeEmbedding[] = "vectorizeEmbedding";
 static const char __pyx_k_AuthenticationError[] = "AuthenticationError";
 static const char __pyx_k_aixhello_xyello_pyx[] = "aixhello\\xyello.pyx";
 static const char __pyx_k_pyx_unpickle_xyellw[] = "__pyx_unpickle_xyellw";
 static const char __pyx_k_similarities_values[] = "similarities_values";
 static const char __pyx_k_xyellw_shorten_text[] = "xyellw.shorten_text";
 static const char __pyx_k_xyellw_SaveToMongoDb[] = "xyellw.SaveToMongoDb";
 static const char __pyx_k_xyellw_vector_search[] = "xyellw.vector_search";
 static const char __pyx_k_xyellw_vectorizeText[] = "xyellw.vectorizeText";
 static const char __pyx_k_decoded_encryptedText[] = "decoded_encryptedText";
 static const char __pyx_k_decrypted_padded_text[] = "decrypted_padded_text";
 static const char __pyx_k_extracted_text_length[] = "extracted_text_length";
+static const char __pyx_k_xyellw_vectorizeEmbed[] = "xyellw.vectorizeEmbed";
 static const char __pyx_k_text_embedding_ada_002[] = "text-embedding-ada-002";
 static const char __pyx_k_xyellw___reduce_cython[] = "xyellw.__reduce_cython__";
 static const char __pyx_k_Invalid_API_key_provided[] = "Invalid API key provided";
 static const char __pyx_k_xyellw___setstate_cython[] = "xyellw.__setstate_cython__";
-static const char __pyx_k_xyellw_vectorizeEmbedding[] = "xyellw.vectorizeEmbedding";
 static const char __pyx_k_vector_search_locals_lambda[] = "vector_search.<locals>.<lambda>";
 static const char __pyx_k_An_unexpected_error_occurred[] = "An unexpected error occurred";
 static const char __pyx_k_cryptography_hazmat_backends[] = "cryptography.hazmat.backends";
 static const char __pyx_k_Access_Control_Request_Headers[] = "Access-Control-Request-Headers";
 static const char __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN[] = "M#rztXq3z@U8rS5jN@PvE4W7F&J(#DhN";
 static const char __pyx_k_Request_failed_with_status_code[] = "Request failed with status code: ";
 static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4BFhKWk32xGPxL9k3jhhHkDqcCQrX37yfmobUNPTXxEGQ==";
@@ -2496,15 +2496,15 @@
 static const char __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1[] = "aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1cmUvc0xwaG9RdURybDZv";
 static const char __pyx_k_cryptography_hazmat_primitives_c[] = "cryptography.hazmat.primitives.ciphers";
 static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4AsrMkJF3D7AnEcHok5damnRp1itFTxnx2dNcFig8Q+Zg==";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbedding(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbed(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8vectorizeText(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_embed, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, PyObject *__pyx_v_vector_query, PyObject *__pyx_v_top_n); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14shorten_text(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_max_length); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_18__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
@@ -2718,27 +2718,27 @@
   PyObject *__pyx_n_u_upsert;
   PyObject *__pyx_n_s_url;
   PyObject *__pyx_n_s_use_setstate;
   PyObject *__pyx_kp_u_utf_8;
   PyObject *__pyx_n_s_vector_query;
   PyObject *__pyx_n_s_vector_search;
   PyObject *__pyx_n_s_vector_search_locals_lambda;
-  PyObject *__pyx_n_s_vectorizeEmbedding;
+  PyObject *__pyx_n_s_vectorizeEmbed;
   PyObject *__pyx_n_s_vectorizeText;
   PyObject *__pyx_n_s_x;
   PyObject *__pyx_n_s_xyellw;
   PyObject *__pyx_n_s_xyellw_Decenigma;
   PyObject *__pyx_n_s_xyellw_Decipherx;
   PyObject *__pyx_n_s_xyellw_Encapseal;
   PyObject *__pyx_n_s_xyellw_SaveToMongoDb;
   PyObject *__pyx_n_s_xyellw___reduce_cython;
   PyObject *__pyx_n_s_xyellw___setstate_cython;
   PyObject *__pyx_n_s_xyellw_shorten_text;
   PyObject *__pyx_n_s_xyellw_vector_search;
-  PyObject *__pyx_n_s_xyellw_vectorizeEmbedding;
+  PyObject *__pyx_n_s_xyellw_vectorizeEmbed;
   PyObject *__pyx_n_s_xyellw_vectorizeText;
   PyObject *__pyx_kp_b_y1c8_8BxP9XN_VKM;
   PyObject *__pyx_int_1;
   PyObject *__pyx_int_5;
   PyObject *__pyx_int_200;
   PyObject *__pyx_int_1000;
   PyObject *__pyx_int_222419149;
@@ -2995,27 +2995,27 @@
   Py_CLEAR(clear_module_state->__pyx_n_u_upsert);
   Py_CLEAR(clear_module_state->__pyx_n_s_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
   Py_CLEAR(clear_module_state->__pyx_n_s_vector_query);
   Py_CLEAR(clear_module_state->__pyx_n_s_vector_search);
   Py_CLEAR(clear_module_state->__pyx_n_s_vector_search_locals_lambda);
-  Py_CLEAR(clear_module_state->__pyx_n_s_vectorizeEmbedding);
+  Py_CLEAR(clear_module_state->__pyx_n_s_vectorizeEmbed);
   Py_CLEAR(clear_module_state->__pyx_n_s_vectorizeText);
   Py_CLEAR(clear_module_state->__pyx_n_s_x);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decipherx);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Encapseal);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_SaveToMongoDb);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_shorten_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vector_search);
-  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vectorizeEmbedding);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vectorizeEmbed);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vectorizeText);
   Py_CLEAR(clear_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
   Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_5);
   Py_CLEAR(clear_module_state->__pyx_int_200);
   Py_CLEAR(clear_module_state->__pyx_int_1000);
   Py_CLEAR(clear_module_state->__pyx_int_222419149);
@@ -3250,27 +3250,27 @@
   Py_VISIT(traverse_module_state->__pyx_n_u_upsert);
   Py_VISIT(traverse_module_state->__pyx_n_s_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
   Py_VISIT(traverse_module_state->__pyx_n_s_vector_query);
   Py_VISIT(traverse_module_state->__pyx_n_s_vector_search);
   Py_VISIT(traverse_module_state->__pyx_n_s_vector_search_locals_lambda);
-  Py_VISIT(traverse_module_state->__pyx_n_s_vectorizeEmbedding);
+  Py_VISIT(traverse_module_state->__pyx_n_s_vectorizeEmbed);
   Py_VISIT(traverse_module_state->__pyx_n_s_vectorizeText);
   Py_VISIT(traverse_module_state->__pyx_n_s_x);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decipherx);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Encapseal);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_SaveToMongoDb);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_shorten_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vector_search);
-  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vectorizeEmbedding);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vectorizeEmbed);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vectorizeText);
   Py_VISIT(traverse_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
   Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_5);
   Py_VISIT(traverse_module_state->__pyx_int_200);
   Py_VISIT(traverse_module_state->__pyx_int_1000);
   Py_VISIT(traverse_module_state->__pyx_int_222419149);
@@ -3515,27 +3515,27 @@
 #define __pyx_n_u_upsert __pyx_mstate_global->__pyx_n_u_upsert
 #define __pyx_n_s_url __pyx_mstate_global->__pyx_n_s_url
 #define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_n_s_vector_query __pyx_mstate_global->__pyx_n_s_vector_query
 #define __pyx_n_s_vector_search __pyx_mstate_global->__pyx_n_s_vector_search
 #define __pyx_n_s_vector_search_locals_lambda __pyx_mstate_global->__pyx_n_s_vector_search_locals_lambda
-#define __pyx_n_s_vectorizeEmbedding __pyx_mstate_global->__pyx_n_s_vectorizeEmbedding
+#define __pyx_n_s_vectorizeEmbed __pyx_mstate_global->__pyx_n_s_vectorizeEmbed
 #define __pyx_n_s_vectorizeText __pyx_mstate_global->__pyx_n_s_vectorizeText
 #define __pyx_n_s_x __pyx_mstate_global->__pyx_n_s_x
 #define __pyx_n_s_xyellw __pyx_mstate_global->__pyx_n_s_xyellw
 #define __pyx_n_s_xyellw_Decenigma __pyx_mstate_global->__pyx_n_s_xyellw_Decenigma
 #define __pyx_n_s_xyellw_Decipherx __pyx_mstate_global->__pyx_n_s_xyellw_Decipherx
 #define __pyx_n_s_xyellw_Encapseal __pyx_mstate_global->__pyx_n_s_xyellw_Encapseal
 #define __pyx_n_s_xyellw_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_xyellw_SaveToMongoDb
 #define __pyx_n_s_xyellw___reduce_cython __pyx_mstate_global->__pyx_n_s_xyellw___reduce_cython
 #define __pyx_n_s_xyellw___setstate_cython __pyx_mstate_global->__pyx_n_s_xyellw___setstate_cython
 #define __pyx_n_s_xyellw_shorten_text __pyx_mstate_global->__pyx_n_s_xyellw_shorten_text
 #define __pyx_n_s_xyellw_vector_search __pyx_mstate_global->__pyx_n_s_xyellw_vector_search
-#define __pyx_n_s_xyellw_vectorizeEmbedding __pyx_mstate_global->__pyx_n_s_xyellw_vectorizeEmbedding
+#define __pyx_n_s_xyellw_vectorizeEmbed __pyx_mstate_global->__pyx_n_s_xyellw_vectorizeEmbed
 #define __pyx_n_s_xyellw_vectorizeText __pyx_mstate_global->__pyx_n_s_xyellw_vectorizeText
 #define __pyx_kp_b_y1c8_8BxP9XN_VKM __pyx_mstate_global->__pyx_kp_b_y1c8_8BxP9XN_VKM
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_5 __pyx_mstate_global->__pyx_int_5
 #define __pyx_int_200 __pyx_mstate_global->__pyx_int_200
 #define __pyx_int_1000 __pyx_mstate_global->__pyx_int_1000
 #define __pyx_int_222419149 __pyx_mstate_global->__pyx_int_222419149
@@ -4659,23 +4659,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbedding(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbed(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbedding = {"vectorizeEmbedding", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbedding, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbedding(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbed = {"vectorizeEmbed", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbed, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbed(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_text_chunks = 0;
@@ -4686,15 +4686,15 @@
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[2] = {0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("vectorizeEmbedding (wrapper)", 0);
+  __Pyx_RefNannySetupContext("vectorizeEmbed (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
@@ -4724,49 +4724,49 @@
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("vectorizeEmbedding", 1, 2, 2, 1); __PYX_ERR(0, 50, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vectorizeEmbed", 1, 2, 2, 1); __PYX_ERR(0, 50, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vectorizeEmbedding") < 0)) __PYX_ERR(0, 50, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vectorizeEmbed") < 0)) __PYX_ERR(0, 50, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_text_chunks = ((PyObject*)values[0]);
     __pyx_v_text_key = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("vectorizeEmbedding", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 50, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("vectorizeEmbed", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 50, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbedding", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbed", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_chunks), (&PyList_Type), 1, "text_chunks", 1))) __PYX_ERR(0, 50, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_key), (&PyUnicode_Type), 1, "text_key", 1))) __PYX_ERR(0, 50, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbedding(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text_chunks, __pyx_v_text_key);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbed(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text_chunks, __pyx_v_text_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -4775,15 +4775,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbedding(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbed(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key) {
   PyObject *__pyx_v_embeddings = NULL;
   PyObject *__pyx_v_chunk = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_embedding = NULL;
   CYTHON_UNUSED PyObject *__pyx_v_e = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -4806,15 +4806,15 @@
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
   char const *__pyx_t_20;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("vectorizeEmbedding", 1);
+  __Pyx_RefNannySetupContext("vectorizeEmbed", 1);
 
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
@@ -4942,15 +4942,15 @@
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_7 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_5, __pyx_t_11);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_ErrRestore(__pyx_t_5, __pyx_t_9, __pyx_t_6);
     __pyx_t_5 = 0; __pyx_t_9 = 0; __pyx_t_6 = 0;
     if (__pyx_t_7) {
-      __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbedding", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbed", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_9, &__pyx_t_5) < 0) __PYX_ERR(0, 62, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_9);
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_9);
       __pyx_v_e = __pyx_t_9;
       /*try:*/ {
@@ -5010,15 +5010,15 @@
           goto __pyx_L6_except_return;
         }
       }
     }
 
     __pyx_t_12 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_12) {
-      __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbedding", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbed", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_9, &__pyx_t_6) < 0) __PYX_ERR(0, 64, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_9);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_9);
       __pyx_v_e = __pyx_t_9;
       /*try:*/ {
@@ -5105,15 +5105,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbedding", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbed", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_embeddings);
   __Pyx_XDECREF(__pyx_v_chunk);
   __Pyx_XDECREF(__pyx_v_response);
   __Pyx_XDECREF(__pyx_v_embedding);
   __Pyx_XDECREF(__pyx_v_e);
@@ -7830,15 +7830,15 @@
   #endif
 }
 
 static PyMethodDef __pyx_methods_8aixhello_6xyello_xyellw[] = {
   {"Decipherx", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"Encapseal", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"Decenigma", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"vectorizeEmbedding", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbedding, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"vectorizeEmbed", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbed, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"vectorizeText", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"SaveToMongoDb", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"vector_search", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"shorten_text", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_15shorten_text, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_17__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_19__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
@@ -8134,27 +8134,27 @@
     {&__pyx_n_u_upsert, __pyx_k_upsert, sizeof(__pyx_k_upsert), 0, 1, 0, 1},
     {&__pyx_n_s_url, __pyx_k_url, sizeof(__pyx_k_url), 0, 0, 1, 1},
     {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
     {&__pyx_n_s_vector_query, __pyx_k_vector_query, sizeof(__pyx_k_vector_query), 0, 0, 1, 1},
     {&__pyx_n_s_vector_search, __pyx_k_vector_search, sizeof(__pyx_k_vector_search), 0, 0, 1, 1},
     {&__pyx_n_s_vector_search_locals_lambda, __pyx_k_vector_search_locals_lambda, sizeof(__pyx_k_vector_search_locals_lambda), 0, 0, 1, 1},
-    {&__pyx_n_s_vectorizeEmbedding, __pyx_k_vectorizeEmbedding, sizeof(__pyx_k_vectorizeEmbedding), 0, 0, 1, 1},
+    {&__pyx_n_s_vectorizeEmbed, __pyx_k_vectorizeEmbed, sizeof(__pyx_k_vectorizeEmbed), 0, 0, 1, 1},
     {&__pyx_n_s_vectorizeText, __pyx_k_vectorizeText, sizeof(__pyx_k_vectorizeText), 0, 0, 1, 1},
     {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw, __pyx_k_xyellw, sizeof(__pyx_k_xyellw), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decenigma, __pyx_k_xyellw_Decenigma, sizeof(__pyx_k_xyellw_Decenigma), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decipherx, __pyx_k_xyellw_Decipherx, sizeof(__pyx_k_xyellw_Decipherx), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Encapseal, __pyx_k_xyellw_Encapseal, sizeof(__pyx_k_xyellw_Encapseal), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_SaveToMongoDb, __pyx_k_xyellw_SaveToMongoDb, sizeof(__pyx_k_xyellw_SaveToMongoDb), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___reduce_cython, __pyx_k_xyellw___reduce_cython, sizeof(__pyx_k_xyellw___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___setstate_cython, __pyx_k_xyellw___setstate_cython, sizeof(__pyx_k_xyellw___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_shorten_text, __pyx_k_xyellw_shorten_text, sizeof(__pyx_k_xyellw_shorten_text), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_vector_search, __pyx_k_xyellw_vector_search, sizeof(__pyx_k_xyellw_vector_search), 0, 0, 1, 1},
-    {&__pyx_n_s_xyellw_vectorizeEmbedding, __pyx_k_xyellw_vectorizeEmbedding, sizeof(__pyx_k_xyellw_vectorizeEmbedding), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_vectorizeEmbed, __pyx_k_xyellw_vectorizeEmbed, sizeof(__pyx_k_xyellw_vectorizeEmbed), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_vectorizeText, __pyx_k_xyellw_vectorizeText, sizeof(__pyx_k_xyellw_vectorizeText), 0, 0, 1, 1},
     {&__pyx_kp_b_y1c8_8BxP9XN_VKM, __pyx_k_y1c8_8BxP9XN_VKM, sizeof(__pyx_k_y1c8_8BxP9XN_VKM), 0, 0, 0, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
@@ -8210,15 +8210,15 @@
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
   __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 33, __pyx_L1_error)
 
   __pyx_tuple__17 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeEmbedding, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeEmbed, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 50, __pyx_L1_error)
 
   __pyx_tuple__19 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_text_embed, __pyx_n_s_text_key, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
   __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeText, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 67, __pyx_L1_error)
 
   __pyx_tuple__21 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 81, __pyx_L1_error)
@@ -8737,17 +8737,17 @@
 
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decenigma, __pyx_t_2) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbedding, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeEmbedding, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbed, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeEmbed, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorizeEmbedding, __pyx_t_2) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorizeEmbed, __pyx_t_2) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorizeText, __pyx_t_2) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
```

### Comparing `aixhello-3.2/aixhello.egg-info/PKG-INFO` & `aixhello-3.3/aixhello.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.2
+Version: 3.3
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.2/setup.py` & `aixhello-3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='3.2',  # Increment the version number
+    version='3.3',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

