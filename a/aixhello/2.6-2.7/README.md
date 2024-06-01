# Comparing `tmp/aixhello-2.6.tar.gz` & `tmp/aixhello-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-2.6.tar", last modified: Sat Jun  1 22:30:56 2024, max compression
+gzip compressed data, was "aixhello-2.7.tar", last modified: Sat Jun  1 22:34:46 2024, max compression
```

## Comparing `aixhello-2.6.tar` & `aixhello-2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 22:30:56.800833 aixhello-2.6/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-2.6/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-2.6/MANIFEST.in
--rw-rw-rw-   0        0        0      650 2024-06-01 22:30:56.800833 aixhello-2.6/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 22:30:56.779857 aixhello-2.6/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-2.6/aixhello/__init__.py
--rw-rw-rw-   0        0        0   462529 2024-06-01 22:30:49.000000 aixhello-2.6/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-01 22:30:56.798833 aixhello-2.6/aixhello.egg-info/
--rw-rw-rw-   0        0        0      650 2024-06-01 22:30:56.000000 aixhello-2.6/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-01 22:30:56.000000 aixhello-2.6/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 22:30:56.000000 aixhello-2.6/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-01 22:30:56.000000 aixhello-2.6/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 22:30:56.000000 aixhello-2.6/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-01 22:30:56.802832 aixhello-2.6/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-01 22:30:24.000000 aixhello-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 22:34:46.583213 aixhello-2.7/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-2.7/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      650 2024-06-01 22:34:46.582211 aixhello-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-31 08:12:32.000000 aixhello-2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 22:34:46.562580 aixhello-2.7/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-2.7/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   460036 2024-06-01 22:34:38.000000 aixhello-2.7/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-01 22:34:46.581210 aixhello-2.7/aixhello.egg-info/
+-rw-rw-rw-   0        0        0      650 2024-06-01 22:34:46.000000 aixhello-2.7/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-01 22:34:46.000000 aixhello-2.7/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 22:34:46.000000 aixhello-2.7/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-01 22:34:46.000000 aixhello-2.7/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 22:34:46.000000 aixhello-2.7/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-01 22:34:46.585212 aixhello-2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-01 22:34:15.000000 aixhello-2.7/setup.py
```

### Comparing `aixhello-2.6/LICENSE` & `aixhello-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-2.6/PKG-INFO` & `aixhello-2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 2.6
+Version: 2.7
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-2.6/aixhello/xyello.c` & `aixhello-2.7/aixhello/xyello.c`

 * *Files 0% similar despite different names*

```diff
@@ -2207,21 +2207,21 @@
 int __pyx_module_is_main_aixhello__xyello = 0;
 
 /* Implementation of "aixhello.xyello" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_chr;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = "";
-static const char __pyx_k__9[] = "*";
+static const char __pyx_k__6[] = "*";
+static const char __pyx_k__8[] = ".";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_iv[] = "iv";
 static const char __pyx_k_AES[] = "AES";
 static const char __pyx_k_CBC[] = "CBC";
-static const char __pyx_k__11[] = ".";
-static const char __pyx_k__28[] = "?";
+static const char __pyx_k__25[] = "?";
 static const char __pyx_k_chr[] = "chr";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_msg[] = "msg";
 static const char __pyx_k_mth[] = "mth";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_set[] = "$set";
@@ -2346,15 +2346,15 @@
 static const char __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1[] = "aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1cmUvc0xwaG9RdURybDZv";
 static const char __pyx_k_cryptography_hazmat_primitives_c[] = "cryptography.hazmat.primitives.ciphers";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_params_dict, CYTHON_UNUSED PyObject *__pyx_v_collection, CYTHON_UNUSED PyObject *__pyx_v_database, CYTHON_UNUSED PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
@@ -2396,18 +2396,18 @@
   PyObject *__pyx_n_s_Decipherx;
   PyObject *__pyx_n_s_Embedshroud;
   PyObject *__pyx_n_s_Encapseal;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_n_s_SaveToMongoDb;
-  PyObject *__pyx_kp_u__11;
-  PyObject *__pyx_n_s__28;
-  PyObject *__pyx_n_s__9;
-  PyObject *__pyx_kp_u__9;
+  PyObject *__pyx_n_s__25;
+  PyObject *__pyx_n_s__6;
+  PyObject *__pyx_kp_u__6;
+  PyObject *__pyx_kp_u__8;
   PyObject *__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1;
   PyObject *__pyx_n_s_aixhello_xyello;
   PyObject *__pyx_kp_s_aixhello_xyello_pyx;
   PyObject *__pyx_n_s_algorithms;
   PyObject *__pyx_n_s_api_key;
   PyObject *__pyx_kp_u_api_key_2;
   PyObject *__pyx_n_s_api_url;
@@ -2529,34 +2529,31 @@
   PyObject *__pyx_int_222419149;
   PyObject *__pyx_int_228825662;
   PyObject *__pyx_int_238750788;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__3;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__5;
-  PyObject *__pyx_tuple__6;
   PyObject *__pyx_tuple__7;
-  PyObject *__pyx_tuple__8;
-  PyObject *__pyx_tuple__10;
-  PyObject *__pyx_tuple__12;
-  PyObject *__pyx_tuple__14;
-  PyObject *__pyx_tuple__16;
-  PyObject *__pyx_tuple__18;
-  PyObject *__pyx_tuple__20;
-  PyObject *__pyx_tuple__22;
-  PyObject *__pyx_tuple__24;
-  PyObject *__pyx_tuple__26;
-  PyObject *__pyx_codeobj__13;
-  PyObject *__pyx_codeobj__15;
-  PyObject *__pyx_codeobj__17;
-  PyObject *__pyx_codeobj__19;
-  PyObject *__pyx_codeobj__21;
-  PyObject *__pyx_codeobj__23;
-  PyObject *__pyx_codeobj__25;
-  PyObject *__pyx_codeobj__27;
+  PyObject *__pyx_tuple__9;
+  PyObject *__pyx_tuple__11;
+  PyObject *__pyx_tuple__13;
+  PyObject *__pyx_tuple__15;
+  PyObject *__pyx_tuple__17;
+  PyObject *__pyx_tuple__19;
+  PyObject *__pyx_tuple__21;
+  PyObject *__pyx_tuple__23;
+  PyObject *__pyx_codeobj__10;
+  PyObject *__pyx_codeobj__12;
+  PyObject *__pyx_codeobj__14;
+  PyObject *__pyx_codeobj__16;
+  PyObject *__pyx_codeobj__18;
+  PyObject *__pyx_codeobj__20;
+  PyObject *__pyx_codeobj__22;
+  PyObject *__pyx_codeobj__24;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2607,18 +2604,18 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_Decipherx);
   Py_CLEAR(clear_module_state->__pyx_n_s_Embedshroud);
   Py_CLEAR(clear_module_state->__pyx_n_s_Encapseal);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_SaveToMongoDb);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__11);
-  Py_CLEAR(clear_module_state->__pyx_n_s__28);
-  Py_CLEAR(clear_module_state->__pyx_n_s__9);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__9);
+  Py_CLEAR(clear_module_state->__pyx_n_s__25);
+  Py_CLEAR(clear_module_state->__pyx_n_s__6);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__6);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__8);
   Py_CLEAR(clear_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_CLEAR(clear_module_state->__pyx_n_s_aixhello_xyello);
   Py_CLEAR(clear_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithms);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_key);
   Py_CLEAR(clear_module_state->__pyx_kp_u_api_key_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_url);
@@ -2740,34 +2737,31 @@
   Py_CLEAR(clear_module_state->__pyx_int_222419149);
   Py_CLEAR(clear_module_state->__pyx_int_228825662);
   Py_CLEAR(clear_module_state->__pyx_int_238750788);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__5);
-  Py_CLEAR(clear_module_state->__pyx_tuple__6);
   Py_CLEAR(clear_module_state->__pyx_tuple__7);
-  Py_CLEAR(clear_module_state->__pyx_tuple__8);
-  Py_CLEAR(clear_module_state->__pyx_tuple__10);
-  Py_CLEAR(clear_module_state->__pyx_tuple__12);
-  Py_CLEAR(clear_module_state->__pyx_tuple__14);
-  Py_CLEAR(clear_module_state->__pyx_tuple__16);
-  Py_CLEAR(clear_module_state->__pyx_tuple__18);
-  Py_CLEAR(clear_module_state->__pyx_tuple__20);
-  Py_CLEAR(clear_module_state->__pyx_tuple__22);
-  Py_CLEAR(clear_module_state->__pyx_tuple__24);
-  Py_CLEAR(clear_module_state->__pyx_tuple__26);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__15);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__19);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__21);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__23);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__25);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__27);
+  Py_CLEAR(clear_module_state->__pyx_tuple__9);
+  Py_CLEAR(clear_module_state->__pyx_tuple__11);
+  Py_CLEAR(clear_module_state->__pyx_tuple__13);
+  Py_CLEAR(clear_module_state->__pyx_tuple__15);
+  Py_CLEAR(clear_module_state->__pyx_tuple__17);
+  Py_CLEAR(clear_module_state->__pyx_tuple__19);
+  Py_CLEAR(clear_module_state->__pyx_tuple__21);
+  Py_CLEAR(clear_module_state->__pyx_tuple__23);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__12);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__14);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__16);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__18);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__20);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__22);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -2796,18 +2790,18 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_Decipherx);
   Py_VISIT(traverse_module_state->__pyx_n_s_Embedshroud);
   Py_VISIT(traverse_module_state->__pyx_n_s_Encapseal);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_SaveToMongoDb);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__11);
-  Py_VISIT(traverse_module_state->__pyx_n_s__28);
-  Py_VISIT(traverse_module_state->__pyx_n_s__9);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__9);
+  Py_VISIT(traverse_module_state->__pyx_n_s__25);
+  Py_VISIT(traverse_module_state->__pyx_n_s__6);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__6);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__8);
   Py_VISIT(traverse_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_VISIT(traverse_module_state->__pyx_n_s_aixhello_xyello);
   Py_VISIT(traverse_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithms);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_key);
   Py_VISIT(traverse_module_state->__pyx_kp_u_api_key_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_url);
@@ -2929,34 +2923,31 @@
   Py_VISIT(traverse_module_state->__pyx_int_222419149);
   Py_VISIT(traverse_module_state->__pyx_int_228825662);
   Py_VISIT(traverse_module_state->__pyx_int_238750788);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__5);
-  Py_VISIT(traverse_module_state->__pyx_tuple__6);
   Py_VISIT(traverse_module_state->__pyx_tuple__7);
-  Py_VISIT(traverse_module_state->__pyx_tuple__8);
-  Py_VISIT(traverse_module_state->__pyx_tuple__10);
-  Py_VISIT(traverse_module_state->__pyx_tuple__12);
-  Py_VISIT(traverse_module_state->__pyx_tuple__14);
-  Py_VISIT(traverse_module_state->__pyx_tuple__16);
-  Py_VISIT(traverse_module_state->__pyx_tuple__18);
-  Py_VISIT(traverse_module_state->__pyx_tuple__20);
-  Py_VISIT(traverse_module_state->__pyx_tuple__22);
-  Py_VISIT(traverse_module_state->__pyx_tuple__24);
-  Py_VISIT(traverse_module_state->__pyx_tuple__26);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__15);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__19);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__21);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__23);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__25);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__27);
+  Py_VISIT(traverse_module_state->__pyx_tuple__9);
+  Py_VISIT(traverse_module_state->__pyx_tuple__11);
+  Py_VISIT(traverse_module_state->__pyx_tuple__13);
+  Py_VISIT(traverse_module_state->__pyx_tuple__15);
+  Py_VISIT(traverse_module_state->__pyx_tuple__17);
+  Py_VISIT(traverse_module_state->__pyx_tuple__19);
+  Py_VISIT(traverse_module_state->__pyx_tuple__21);
+  Py_VISIT(traverse_module_state->__pyx_tuple__23);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__12);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__14);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__16);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__18);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__20);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__22);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -2995,18 +2986,18 @@
 #define __pyx_n_s_Decipherx __pyx_mstate_global->__pyx_n_s_Decipherx
 #define __pyx_n_s_Embedshroud __pyx_mstate_global->__pyx_n_s_Embedshroud
 #define __pyx_n_s_Encapseal __pyx_mstate_global->__pyx_n_s_Encapseal
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN __pyx_mstate_global->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_n_s_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_SaveToMongoDb
-#define __pyx_kp_u__11 __pyx_mstate_global->__pyx_kp_u__11
-#define __pyx_n_s__28 __pyx_mstate_global->__pyx_n_s__28
-#define __pyx_n_s__9 __pyx_mstate_global->__pyx_n_s__9
-#define __pyx_kp_u__9 __pyx_mstate_global->__pyx_kp_u__9
+#define __pyx_n_s__25 __pyx_mstate_global->__pyx_n_s__25
+#define __pyx_n_s__6 __pyx_mstate_global->__pyx_n_s__6
+#define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
+#define __pyx_kp_u__8 __pyx_mstate_global->__pyx_kp_u__8
 #define __pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1 __pyx_mstate_global->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1
 #define __pyx_n_s_aixhello_xyello __pyx_mstate_global->__pyx_n_s_aixhello_xyello
 #define __pyx_kp_s_aixhello_xyello_pyx __pyx_mstate_global->__pyx_kp_s_aixhello_xyello_pyx
 #define __pyx_n_s_algorithms __pyx_mstate_global->__pyx_n_s_algorithms
 #define __pyx_n_s_api_key __pyx_mstate_global->__pyx_n_s_api_key
 #define __pyx_kp_u_api_key_2 __pyx_mstate_global->__pyx_kp_u_api_key_2
 #define __pyx_n_s_api_url __pyx_mstate_global->__pyx_n_s_api_url
@@ -3128,34 +3119,31 @@
 #define __pyx_int_222419149 __pyx_mstate_global->__pyx_int_222419149
 #define __pyx_int_228825662 __pyx_mstate_global->__pyx_int_228825662
 #define __pyx_int_238750788 __pyx_mstate_global->__pyx_int_238750788
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
-#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
-#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
-#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
-#define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
-#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
-#define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
-#define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
-#define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
-#define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
-#define __pyx_tuple__24 __pyx_mstate_global->__pyx_tuple__24
-#define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
-#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
-#define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
-#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
-#define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
-#define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
-#define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
-#define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
-#define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
+#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
+#define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
+#define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
+#define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
+#define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
+#define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
+#define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
+#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
+#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
+#define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
+#define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
+#define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
+#define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
+#define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
+#define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
+#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
 /* #### Code section: module_code ### */
 
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -4492,19 +4480,19 @@
 static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9SaveToMongoDb(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
-  PyObject *__pyx_v_params_dict = 0;
-  CYTHON_UNUSED PyObject *__pyx_v_collection = 0;
-  CYTHON_UNUSED PyObject *__pyx_v_database = 0;
-  CYTHON_UNUSED PyObject *__pyx_v_datasource = 0;
+  PyObject *__pyx_v_collection = 0;
+  PyObject *__pyx_v_database = 0;
+  PyObject *__pyx_v_datasource = 0;
   PyObject *__pyx_v_enkyc = 0;
+  PyObject *__pyx_v_params_dict = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[5] = {0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -4517,15 +4505,15 @@
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_params_dict,&__pyx_n_s_collection,&__pyx_n_s_database,&__pyx_n_s_datasource,&__pyx_n_s_enkyc,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_collection,&__pyx_n_s_database,&__pyx_n_s_datasource,&__pyx_n_s_enkyc,&__pyx_n_s_params_dict,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -4537,53 +4525,53 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_params_dict)) != 0)) {
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_collection)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_collection)) != 0)) {
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_database)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 1); __PYX_ERR(0, 60, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_database)) != 0)) {
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_datasource)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 2); __PYX_ERR(0, 60, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_datasource)) != 0)) {
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_enkyc)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 3); __PYX_ERR(0, 60, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
-        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_enkyc)) != 0)) {
+        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_params_dict)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 4); __PYX_ERR(0, 60, __pyx_L3_error)
         }
@@ -4597,19 +4585,19 @@
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
       values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
     }
-    __pyx_v_params_dict = values[0];
-    __pyx_v_collection = ((PyObject*)values[1]);
-    __pyx_v_database = ((PyObject*)values[2]);
-    __pyx_v_datasource = ((PyObject*)values[3]);
-    __pyx_v_enkyc = ((PyObject*)values[4]);
+    __pyx_v_collection = ((PyObject*)values[0]);
+    __pyx_v_database = ((PyObject*)values[1]);
+    __pyx_v_datasource = ((PyObject*)values[2]);
+    __pyx_v_enkyc = ((PyObject*)values[3]);
+    __pyx_v_params_dict = values[4];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 60, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
@@ -4623,15 +4611,15 @@
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_collection), (&PyUnicode_Type), 1, "collection", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_database), (&PyUnicode_Type), 1, "database", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_datasource), (&PyUnicode_Type), 1, "datasource", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_enkyc), (&PyUnicode_Type), 1, "enkyc", 1))) __PYX_ERR(0, 60, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_params_dict, __pyx_v_collection, __pyx_v_database, __pyx_v_datasource, __pyx_v_enkyc);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_collection, __pyx_v_database, __pyx_v_datasource, __pyx_v_enkyc, __pyx_v_params_dict);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -4640,15 +4628,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_params_dict, CYTHON_UNUSED PyObject *__pyx_v_collection, CYTHON_UNUSED PyObject *__pyx_v_database, CYTHON_UNUSED PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict) {
   PyObject *__pyx_v_decrypted_url = NULL;
   PyObject *__pyx_v_payload = NULL;
   PyObject *__pyx_v_headers = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -4688,131 +4676,113 @@
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_decrypted_url = __pyx_t_1;
   __pyx_t_1 = 0;
 
   __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_collection, __pyx_t_3) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_collection, __pyx_v_collection) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_database, __pyx_t_2) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_database, __pyx_v_database) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 66, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_dataSource, __pyx_t_3) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_dataSource, __pyx_v_datasource) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
 
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_filename, __pyx_t_5) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filter, __pyx_t_3) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_filename, __pyx_t_5) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filter, __pyx_t_2) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
 
   __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_filename, __pyx_t_6) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_data, __pyx_t_2) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_data, __pyx_t_3) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_type, __pyx_kp_u_application_pdf) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_extracted_text, __pyx_t_6) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_text_embeddings, __pyx_t_2) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_set, __pyx_t_5) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_update, __pyx_t_3) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_text_embeddings, __pyx_t_3) < 0) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_set, __pyx_t_5) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_update, __pyx_t_2) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_upsert, Py_True) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
   __pyx_v_payload = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__9) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__6) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
 
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_v_enkyc) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   __pyx_v_headers = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_requests); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_decrypted_url);
   __Pyx_GIVEREF(__pyx_v_decrypted_url);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_decrypted_url)) __PYX_ERR(0, 85, __pyx_L1_error);
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_json, __pyx_v_payload) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_response = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_v_response = __pyx_t_3;
+  __pyx_t_3 = 0;
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_2, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 87, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_3, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_7) {
 
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_1 = NULL;
     __pyx_t_4 = 0;
@@ -4826,36 +4796,36 @@
         __Pyx_DECREF_SET(__pyx_t_5, function);
         __pyx_t_4 = 1;
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
-      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+      __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
+    __pyx_r = __pyx_t_3;
+    __pyx_t_3 = 0;
     goto __pyx_L0;
 
   }
 
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_error, __pyx_t_5) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_error, __pyx_t_5) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_r = __pyx_t_2;
-    __pyx_t_2 = 0;
+    __pyx_r = __pyx_t_3;
+    __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -5306,15 +5276,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_xyellw", 1);
 
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__10, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__7, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
@@ -5654,18 +5624,18 @@
     {&__pyx_n_s_Decipherx, __pyx_k_Decipherx, sizeof(__pyx_k_Decipherx), 0, 0, 1, 1},
     {&__pyx_n_s_Embedshroud, __pyx_k_Embedshroud, sizeof(__pyx_k_Embedshroud), 0, 0, 1, 1},
     {&__pyx_n_s_Encapseal, __pyx_k_Encapseal, sizeof(__pyx_k_Encapseal), 0, 0, 1, 1},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, sizeof(__pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN), 0, 0, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_SaveToMongoDb, __pyx_k_SaveToMongoDb, sizeof(__pyx_k_SaveToMongoDb), 0, 0, 1, 1},
-    {&__pyx_kp_u__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 1, 0, 0},
-    {&__pyx_n_s__28, __pyx_k__28, sizeof(__pyx_k__28), 0, 0, 1, 1},
-    {&__pyx_n_s__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 0, 1, 1},
-    {&__pyx_kp_u__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 1, 0, 0},
+    {&__pyx_n_s__25, __pyx_k__25, sizeof(__pyx_k__25), 0, 0, 1, 1},
+    {&__pyx_n_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 1},
+    {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
+    {&__pyx_kp_u__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 1, 0, 0},
     {&__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, sizeof(__pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1), 0, 1, 0, 1},
     {&__pyx_n_s_aixhello_xyello, __pyx_k_aixhello_xyello, sizeof(__pyx_k_aixhello_xyello), 0, 0, 1, 1},
     {&__pyx_kp_s_aixhello_xyello_pyx, __pyx_k_aixhello_xyello_pyx, sizeof(__pyx_k_aixhello_xyello_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_algorithms, __pyx_k_algorithms, sizeof(__pyx_k_algorithms), 0, 0, 1, 1},
     {&__pyx_n_s_api_key, __pyx_k_api_key, sizeof(__pyx_k_api_key), 0, 0, 1, 1},
     {&__pyx_kp_u_api_key_2, __pyx_k_api_key_2, sizeof(__pyx_k_api_key_2), 0, 1, 0, 0},
     {&__pyx_n_s_api_url, __pyx_k_api_url, sizeof(__pyx_k_api_url), 0, 0, 1, 1},
@@ -5796,85 +5766,73 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_u_collection, __pyx_kp_u_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_u_filename, __pyx_kp_u_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_database, __pyx_kp_u_); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_file_data, __pyx_kp_u_); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_dataSource, __pyx_kp_u_); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_extracted_text, __pyx_kp_u_); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_filename, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_text_embeddings, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_u_file_data, __pyx_kp_u_); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 71, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-
-  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_u_extracted_text, __pyx_kp_u_); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_u_text_embeddings, __pyx_kp_u_); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 74, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-
-  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-
-  __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 9, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 9, __pyx_L1_error)
-
-  __pyx_tuple__14 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 16, __pyx_L1_error)
-
-  __pyx_tuple__16 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 31, __pyx_L1_error)
-
-  __pyx_tuple__18 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 48, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Embedshroud, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 48, __pyx_L1_error)
-
-  __pyx_tuple__20 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_params_dict, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SaveToMongoDb, 60, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 60, __pyx_L1_error)
-
-  __pyx_tuple__22 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(1, 1, __pyx_L1_error)
-
-  __pyx_tuple__24 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 16, __pyx_L1_error)
-
-  __pyx_tuple__26 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 9, __pyx_L1_error)
+
+  __pyx_tuple__11 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 16, __pyx_L1_error)
+
+  __pyx_tuple__13 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 31, __pyx_L1_error)
+
+  __pyx_tuple__15 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Embedshroud, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 48, __pyx_L1_error)
+
+  __pyx_tuple__17 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SaveToMongoDb, 60, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 60, __pyx_L1_error)
+
+  __pyx_tuple__19 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(1, 16, __pyx_L1_error)
+
+  __pyx_tuple__23 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -6321,57 +6279,57 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_openai, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_openai, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decipherx, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Encapseal, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decenigma, __pyx_t_2) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Embedshroud, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Embedshroud, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Embedshroud, __pyx_t_2) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9SaveToMongoDb, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SaveToMongoDb, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9SaveToMongoDb, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SaveToMongoDb, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_SaveToMongoDb, __pyx_t_2) < 0) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_xyellw, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -7855,15 +7813,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__11);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__8);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -8683,15 +8641,15 @@
         return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
     }
     return module;
 }
 #endif
 static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__9;
+    PyObject *module, *from_list, *star = __pyx_n_s__6;
     CYTHON_UNUSED_VAR(parts_tuple);
     from_list = PyList_New(1);
     if (unlikely(!from_list))
         return NULL;
     Py_INCREF(star);
     PyList_SET_ITEM(from_list, 0, star);
     module = __Pyx_Import(name, from_list, 0);
@@ -10596,15 +10554,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__28);
+        name = __Pyx_NewRef(__pyx_n_s__25);
     }
     return name;
 }
 #endif
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
```

### Comparing `aixhello-2.6/aixhello.egg-info/PKG-INFO` & `aixhello-2.7/aixhello.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 2.6
+Version: 2.7
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-2.6/setup.py` & `aixhello-2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='2.6',  # Increment the version number
+    version='2.7',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

