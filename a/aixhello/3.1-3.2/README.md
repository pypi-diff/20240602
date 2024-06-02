# Comparing `tmp/aixhello-3.1.tar.gz` & `tmp/aixhello-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-3.1.tar", last modified: Sat Jun  1 22:58:53 2024, max compression
+gzip compressed data, was "aixhello-3.2.tar", last modified: Sun Jun  2 02:59:26 2024, max compression
```

## Comparing `aixhello-3.1.tar` & `aixhello-3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 22:58:53.568932 aixhello-3.1/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.1/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-01 22:58:53.568932 aixhello-3.1/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 22:58:53.546167 aixhello-3.1/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.1/aixhello/__init__.py
--rw-rw-rw-   0        0        0   479773 2024-06-01 22:58:46.000000 aixhello-3.1/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-01 22:58:53.566933 aixhello-3.1/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-01 22:58:53.000000 aixhello-3.1/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-01 22:58:53.000000 aixhello-3.1/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 22:58:53.000000 aixhello-3.1/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-01 22:58:53.000000 aixhello-3.1/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 22:58:53.000000 aixhello-3.1/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-01 22:58:53.570932 aixhello-3.1/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-01 22:58:25.000000 aixhello-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 02:59:26.740756 aixhello-3.2/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.2/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-02 02:59:26.740756 aixhello-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 02:59:26.710209 aixhello-3.2/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.2/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   590146 2024-06-02 02:59:17.000000 aixhello-3.2/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-02 02:59:26.739755 aixhello-3.2/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-02 02:59:26.000000 aixhello-3.2/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-02 02:59:26.000000 aixhello-3.2/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 02:59:26.000000 aixhello-3.2/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-02 02:59:26.000000 aixhello-3.2/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 02:59:26.000000 aixhello-3.2/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-02 02:59:26.742792 aixhello-3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-02 02:56:21.000000 aixhello-3.2/setup.py
```

### Comparing `aixhello-3.1/LICENSE` & `aixhello-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-3.1/PKG-INFO` & `aixhello-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.1
+Version: 3.2
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.1/README.md` & `aixhello-3.2/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-3.1/aixhello/xyello.c` & `aixhello-3.2/aixhello/xyello.c`

 * *Files 10% similar despite different names*

```diff
@@ -1938,98 +1938,73 @@
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
 /* PyIntCompare.proto */
 static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
-/* KeywordStringCheck.proto */
-static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
-
-/* GetAttr3.proto */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
-
-/* RaiseUnexpectedTypeError.proto */
-static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
+/* DictGetItem.proto */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
+#define __Pyx_PyObject_Dict_GetItem(obj, name)\
+    (likely(PyDict_CheckExact(obj)) ?\
+     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
+#else
+#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
+#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
+#endif
 
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+/* PyObjectCall2Args.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
-/* ImportFrom.proto */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
+/* PyObjectGetMethod.proto */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+/* PyObjectCallMethod1.proto */
+static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
 
-/* GetAttr.proto */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
+/* append.proto */
+static CYTHON_INLINE int __Pyx_PyObject_Append(PyObject* L, PyObject* x);
 
-/* HasAttr.proto */
-#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
-#define __Pyx_HasAttr(o, n)  PyObject_HasAttrWithError(o, n)
-#else
-static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
+/* PyObjectFormatSimple.proto */
+#if CYTHON_COMPILING_IN_PYPY
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#elif PY_MAJOR_VERSION < 3
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyString_CheckExact(s)) ? PyUnicode_FromEncodedObject(s, NULL, "strict") :\
+        PyObject_Format(s, f))
+#elif CYTHON_USE_TYPE_SLOTS
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyLong_CheckExact(s)) ? PyLong_Type.tp_repr(s) :\
+        likely(PyFloat_CheckExact(s)) ? PyFloat_Type.tp_repr(s) :\
+        PyObject_Format(s, f))
+#else
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
 #endif
 
 /* IncludeStructmemberH.proto */
 #include <structmember.h>
 
 /* FixUpExtensionType.proto */
 #if CYTHON_USE_TYPE_SPECS
 static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
-/* PyObjectCallNoArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-
-/* PyObjectGetMethod.proto */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
-
-/* PyObjectCallMethod0.proto */
-static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
-
-/* ValidateBasesTuple.proto */
-#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
-static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
-#endif
-
-/* PyType_Ready.proto */
-CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
-
-/* PyObject_GenericGetAttrNoDict.proto */
-#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
-#else
-#define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
-#endif
-
-/* PyObject_GenericGetAttr.proto */
-#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
-static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
-#else
-#define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
-#endif
-
-/* SetupReduce.proto */
-#if !CYTHON_COMPILING_IN_LIMITED_API
-static int __Pyx_setup_reduce(PyObject* type_obj);
-#endif
-
-/* ImportDottedModule.proto */
-static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
-#if PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
-#endif
-
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
@@ -2162,14 +2137,102 @@
 /* CythonFunction.proto */
 static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 
+/* ListCompAppend.proto */
+#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
+static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
+    PyListObject* L = (PyListObject*) list;
+    Py_ssize_t len = Py_SIZE(list);
+    if (likely(L->allocated > len)) {
+        Py_INCREF(x);
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+        L->ob_item[len] = x;
+        #else
+        PyList_SET_ITEM(list, len, x);
+        #endif
+        __Pyx_SET_SIZE(list, len + 1);
+        return 0;
+    }
+    return PyList_Append(list, x);
+}
+#else
+#define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
+#endif
+
+/* KeywordStringCheck.proto */
+static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
+
+/* GetAttr3.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
+
+/* RaiseUnexpectedTypeError.proto */
+static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
+
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+
+/* ImportFrom.proto */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
+/* GetAttr.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
+
+/* HasAttr.proto */
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+#define __Pyx_HasAttr(o, n)  PyObject_HasAttrWithError(o, n)
+#else
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
+#endif
+
+/* PyObjectCallNoArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+
+/* PyObjectCallMethod0.proto */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
+
+/* ValidateBasesTuple.proto */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
+#endif
+
+/* PyType_Ready.proto */
+CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
+
+/* PyObject_GenericGetAttrNoDict.proto */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
+#endif
+
+/* PyObject_GenericGetAttr.proto */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
+#endif
+
+/* SetupReduce.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_setup_reduce(PyObject* type_obj);
+#endif
+
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
+#endif
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -2237,163 +2300,218 @@
 #define __Pyx_MODULE_NAME "aixhello.xyello"
 extern int __pyx_module_is_main_aixhello__xyello;
 int __pyx_module_is_main_aixhello__xyello = 0;
 
 /* Implementation of "aixhello.xyello" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_chr;
+static PyObject *__pyx_builtin_print;
+static PyObject *__pyx_builtin_sorted;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = "";
 static const char __pyx_k_e[] = "e";
+static const char __pyx_k_x[] = "x";
 static const char __pyx_k__6[] = "*";
-static const char __pyx_k__8[] = ".";
+static const char __pyx_k__8[] = "...";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_iv[] = "iv";
+static const char __pyx_k_np[] = "np";
+static const char __pyx_k_re[] = "re";
 static const char __pyx_k_AES[] = "AES";
 static const char __pyx_k_CBC[] = "CBC";
-static const char __pyx_k__25[] = "?";
+static const char __pyx_k__10[] = ".";
+static const char __pyx_k__35[] = "?";
 static const char __pyx_k_chr[] = "chr";
+static const char __pyx_k_doc[] = "doc";
+static const char __pyx_k_dot[] = "dot";
+static const char __pyx_k_emb[] = "emb";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_msg[] = "msg";
 static const char __pyx_k_mth[] = "mth";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_set[] = "$set";
+static const char __pyx_k_url[] = "url";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_json[] = "json";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
+static const char __pyx_k_norm[] = "norm";
 static const char __pyx_k_post[] = "post";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_text[] = "text";
+static const char __pyx_k_array[] = "array";
 static const char __pyx_k_chunk[] = "chunk";
 static const char __pyx_k_enkyc[] = "enkyc";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_input[] = "input";
 static const char __pyx_k_model[] = "model";
 static const char __pyx_k_modes[] = "modes";
+static const char __pyx_k_numpy[] = "numpy";
+static const char __pyx_k_print[] = "print";
 static const char __pyx_k_state[] = "state";
+static const char __pyx_k_top_n[] = "top_n";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_Cipher[] = "Cipher";
+static const char __pyx_k_append[] = "append";
 static const char __pyx_k_base64[] = "base64";
 static const char __pyx_k_cipher[] = "cipher";
 static const char __pyx_k_create[] = "create";
 static const char __pyx_k_decode[] = "decode";
 static const char __pyx_k_dict_2[] = "_dict";
 static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_filter[] = "filter";
 static const char __pyx_k_import[] = "__import__";
+static const char __pyx_k_linalg[] = "linalg";
 static const char __pyx_k_openai[] = "openai";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
+static const char __pyx_k_result[] = "result";
+static const char __pyx_k_sorted[] = "sorted";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_upsert[] = "upsert";
 static const char __pyx_k_xyellw[] = "xyellw";
 static const char __pyx_k_api_key[] = "api_key";
 static const char __pyx_k_api_url[] = "api_url";
 static const char __pyx_k_backend[] = "backend";
 static const char __pyx_k_disable[] = "disable";
+static const char __pyx_k_emb_vec[] = "emb_vec";
 static const char __pyx_k_headers[] = "headers";
 static const char __pyx_k_message[] = "message";
 static const char __pyx_k_payload[] = "payload";
+static const char __pyx_k_project[] = "$project";
+static const char __pyx_k_reverse[] = "reverse";
 static const char __pyx_k_strText[] = "strText";
 static const char __pyx_k_database[] = "database";
 static const char __pyx_k_filename[] = "filename";
 static const char __pyx_k_finalize[] = "finalize";
 static const char __pyx_k_getstate[] = "__getstate__";
+static const char __pyx_k_pipeline[] = "pipeline";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_requests[] = "requests";
 static const char __pyx_k_response[] = "response";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_text_key[] = "text_key";
 static const char __pyx_k_Decenigma[] = "Decenigma";
 static const char __pyx_k_Decipherx[] = "Decipherx";
 static const char __pyx_k_Encapseal[] = "Encapseal";
 static const char __pyx_k_api_key_2[] = "api-key";
 static const char __pyx_k_b64decode[] = "b64decode";
 static const char __pyx_k_b64encode[] = "b64encode";
+static const char __pyx_k_connParam[] = "connParam";
 static const char __pyx_k_decryptor[] = "decryptor";
+static const char __pyx_k_documents[] = "documents";
 static const char __pyx_k_embedding[] = "embedding";
 static const char __pyx_k_encryptor[] = "encryptor";
 static const char __pyx_k_file_data[] = "file_data";
 static const char __pyx_k_file_type[] = "file_type";
+static const char __pyx_k_filenames[] = "filenames";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
+static const char __pyx_k_query_vec[] = "query_vec";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_algorithms[] = "algorithms";
 static const char __pyx_k_collection[] = "collection";
 static const char __pyx_k_dataSource[] = "dataSource";
 static const char __pyx_k_datasource[] = "datasource";
 static const char __pyx_k_embeddings[] = "embeddings";
+static const char __pyx_k_max_length[] = "max_length";
 static const char __pyx_k_pad_length[] = "pad_length";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
-static const char __pyx_k_Embedshroud[] = "Embedshroud";
+static const char __pyx_k_similarity[] = "similarity";
+static const char __pyx_k_text_embed[] = "text_embed";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_encoded_url[] = "encoded_url";
 static const char __pyx_k_padded_text[] = "padded_text";
 static const char __pyx_k_params_dict[] = "params_dict";
 static const char __pyx_k_status_code[] = "status_code";
 static const char __pyx_k_text_chunks[] = "text_chunks";
+static const char __pyx_k_top_results[] = "top_results";
 static const char __pyx_k_Content_Type[] = "Content-Type";
+static const char __pyx_k_cleaned_text[] = "cleaned_text";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
+static const char __pyx_k_shorten_text[] = "shorten_text";
+static const char __pyx_k_similarities[] = "similarities";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_use_setstate[] = "use_setstate";
+static const char __pyx_k_vector_query[] = "vector_query";
 static const char __pyx_k_SaveToMongoDb[] = "SaveToMongoDb";
 static const char __pyx_k_decryptedText[] = "decryptedText";
 static const char __pyx_k_decrypted_url[] = "decrypted_url";
 static const char __pyx_k_encryptedText[] = "encryptedText";
+static const char __pyx_k_query_payload[] = "query_payload";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_response_data[] = "response_data";
+static const char __pyx_k_similar_score[] = "similar_score";
+static const char __pyx_k_vector_search[] = "vector_search";
+static const char __pyx_k_vectorizeText[] = "vectorizeText";
 static const char __pyx_k_extracted_text[] = "extracted_text";
 static const char __pyx_k_aixhello_xyello[] = "aixhello.xyello";
 static const char __pyx_k_application_pdf[] = "application/pdf";
 static const char __pyx_k_default_backend[] = "default_backend";
+static const char __pyx_k_extracted_texts[] = "extracted_texts";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_text_embeddings[] = "text_embeddings";
+static const char __pyx_k_Unknown_filename[] = "Unknown filename";
 static const char __pyx_k_application_json[] = "application/json";
 static const char __pyx_k_xyellw_Decenigma[] = "xyellw.Decenigma";
 static const char __pyx_k_xyellw_Decipherx[] = "xyellw.Decipherx";
 static const char __pyx_k_xyellw_Encapseal[] = "xyellw.Encapseal";
 static const char __pyx_k_y1c8_8BxP9XN_VKM[] = "y1c8@8BxP9XN#VKM";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_xyellw_Embedshroud[] = "xyellw.Embedshroud";
+static const char __pyx_k_vectorizeEmbedding[] = "vectorizeEmbedding";
 static const char __pyx_k_AuthenticationError[] = "AuthenticationError";
 static const char __pyx_k_aixhello_xyello_pyx[] = "aixhello\\xyello.pyx";
 static const char __pyx_k_pyx_unpickle_xyellw[] = "__pyx_unpickle_xyellw";
+static const char __pyx_k_similarities_values[] = "similarities_values";
+static const char __pyx_k_xyellw_shorten_text[] = "xyellw.shorten_text";
 static const char __pyx_k_xyellw_SaveToMongoDb[] = "xyellw.SaveToMongoDb";
+static const char __pyx_k_xyellw_vector_search[] = "xyellw.vector_search";
+static const char __pyx_k_xyellw_vectorizeText[] = "xyellw.vectorizeText";
 static const char __pyx_k_decoded_encryptedText[] = "decoded_encryptedText";
 static const char __pyx_k_decrypted_padded_text[] = "decrypted_padded_text";
+static const char __pyx_k_extracted_text_length[] = "extracted_text_length";
 static const char __pyx_k_text_embedding_ada_002[] = "text-embedding-ada-002";
 static const char __pyx_k_xyellw___reduce_cython[] = "xyellw.__reduce_cython__";
 static const char __pyx_k_Invalid_API_key_provided[] = "Invalid API key provided";
 static const char __pyx_k_xyellw___setstate_cython[] = "xyellw.__setstate_cython__";
+static const char __pyx_k_xyellw_vectorizeEmbedding[] = "xyellw.vectorizeEmbedding";
+static const char __pyx_k_vector_search_locals_lambda[] = "vector_search.<locals>.<lambda>";
 static const char __pyx_k_An_unexpected_error_occurred[] = "An unexpected error occurred";
 static const char __pyx_k_cryptography_hazmat_backends[] = "cryptography.hazmat.backends";
 static const char __pyx_k_Access_Control_Request_Headers[] = "Access-Control-Request-Headers";
 static const char __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN[] = "M#rztXq3z@U8rS5jN@PvE4W7F&J(#DhN";
+static const char __pyx_k_Request_failed_with_status_code[] = "Request failed with status code: ";
 static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4BFhKWk32xGPxL9k3jhhHkDqcCQrX37yfmobUNPTXxEGQ==";
+static const char __pyx_k_text_embeddings_key_not_found_i[] = "'text_embeddings' key not found in document with filename: ";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())";
 static const char __pyx_k_Successfully_save_to_the_databas[] = "Successfully save to the database.";
 static const char __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1[] = "aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1cmUvc0xwaG9RdURybDZv";
 static const char __pyx_k_cryptography_hazmat_primitives_c[] = "cryptography.hazmat.primitives.ciphers";
+static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4AsrMkJF3D7AnEcHok5damnRp1itFTxnx2dNcFig8Q+Zg==";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbedding(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8vectorizeText(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_embed, PyObject *__pyx_v_text_key); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
+static PyObject *__pyx_lambda_funcdef_lambda(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, PyObject *__pyx_v_vector_query, PyObject *__pyx_v_top_n); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14shorten_text(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_max_length); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_18__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
@@ -2429,47 +2547,54 @@
   PyObject *__pyx_kp_u_An_unexpected_error_occurred;
   PyObject *__pyx_n_s_AuthenticationError;
   PyObject *__pyx_n_s_CBC;
   PyObject *__pyx_n_s_Cipher;
   PyObject *__pyx_kp_u_Content_Type;
   PyObject *__pyx_n_s_Decenigma;
   PyObject *__pyx_n_s_Decipherx;
-  PyObject *__pyx_n_s_Embedshroud;
   PyObject *__pyx_n_s_Encapseal;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_kp_u_Invalid_API_key_provided;
   PyObject *__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
   PyObject *__pyx_n_s_PickleError;
+  PyObject *__pyx_kp_u_Request_failed_with_status_code;
   PyObject *__pyx_n_s_SaveToMongoDb;
   PyObject *__pyx_kp_u_Successfully_save_to_the_databas;
-  PyObject *__pyx_n_s__25;
+  PyObject *__pyx_kp_u_Unknown_filename;
+  PyObject *__pyx_kp_u__10;
+  PyObject *__pyx_n_s__35;
   PyObject *__pyx_n_s__6;
   PyObject *__pyx_kp_u__6;
   PyObject *__pyx_kp_u__8;
   PyObject *__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1;
   PyObject *__pyx_n_s_aixhello_xyello;
   PyObject *__pyx_kp_s_aixhello_xyello_pyx;
   PyObject *__pyx_n_s_algorithms;
   PyObject *__pyx_n_s_api_key;
   PyObject *__pyx_kp_u_api_key_2;
   PyObject *__pyx_n_s_api_url;
+  PyObject *__pyx_n_s_append;
   PyObject *__pyx_kp_u_application_json;
   PyObject *__pyx_kp_u_application_pdf;
+  PyObject *__pyx_n_s_array;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_b64decode;
   PyObject *__pyx_n_s_b64encode;
   PyObject *__pyx_n_s_backend;
   PyObject *__pyx_n_s_base64;
   PyObject *__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn;
+  PyObject *__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2;
   PyObject *__pyx_n_s_chr;
   PyObject *__pyx_n_s_chunk;
   PyObject *__pyx_n_s_cipher;
+  PyObject *__pyx_n_s_cleaned_text;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_collection;
   PyObject *__pyx_n_u_collection;
+  PyObject *__pyx_n_s_connParam;
   PyObject *__pyx_n_s_create;
   PyObject *__pyx_n_s_cryptography_hazmat_backends;
   PyObject *__pyx_n_s_cryptography_hazmat_primitives_c;
   PyObject *__pyx_n_s_data;
   PyObject *__pyx_n_u_dataSource;
   PyObject *__pyx_n_s_database;
   PyObject *__pyx_n_u_database;
@@ -2480,98 +2605,146 @@
   PyObject *__pyx_n_s_decrypted_padded_text;
   PyObject *__pyx_n_s_decrypted_url;
   PyObject *__pyx_n_s_decryptor;
   PyObject *__pyx_n_s_default_backend;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_dict_2;
   PyObject *__pyx_kp_u_disable;
+  PyObject *__pyx_n_s_doc;
+  PyObject *__pyx_n_s_documents;
+  PyObject *__pyx_n_u_documents;
+  PyObject *__pyx_n_s_dot;
   PyObject *__pyx_n_s_e;
+  PyObject *__pyx_n_s_emb;
+  PyObject *__pyx_n_s_emb_vec;
   PyObject *__pyx_n_s_embedding;
   PyObject *__pyx_n_s_embeddings;
   PyObject *__pyx_kp_u_enable;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_encoded_url;
   PyObject *__pyx_n_s_encryptedText;
   PyObject *__pyx_n_s_encryptor;
   PyObject *__pyx_n_s_enkyc;
+  PyObject *__pyx_n_u_enkyc;
   PyObject *__pyx_n_u_error;
   PyObject *__pyx_n_u_extracted_text;
+  PyObject *__pyx_n_s_extracted_text_length;
+  PyObject *__pyx_n_s_extracted_texts;
   PyObject *__pyx_n_u_file_data;
   PyObject *__pyx_n_u_file_type;
   PyObject *__pyx_n_u_filename;
+  PyObject *__pyx_n_s_filenames;
   PyObject *__pyx_n_u_filter;
   PyObject *__pyx_n_s_finalize;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_get;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_n_s_headers;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_initializing;
   PyObject *__pyx_n_s_input;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_iv;
   PyObject *__pyx_n_s_json;
   PyObject *__pyx_n_s_key;
+  PyObject *__pyx_n_s_linalg;
   PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_max_length;
   PyObject *__pyx_n_u_message;
   PyObject *__pyx_n_s_model;
   PyObject *__pyx_n_s_modes;
   PyObject *__pyx_n_s_msg;
   PyObject *__pyx_n_s_mth;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_new;
+  PyObject *__pyx_n_s_norm;
+  PyObject *__pyx_n_s_np;
+  PyObject *__pyx_n_s_numpy;
   PyObject *__pyx_n_s_openai;
   PyObject *__pyx_n_s_pad_length;
   PyObject *__pyx_n_s_padded_text;
   PyObject *__pyx_n_s_params_dict;
   PyObject *__pyx_n_s_payload;
   PyObject *__pyx_n_s_pickle;
+  PyObject *__pyx_n_s_pipeline;
+  PyObject *__pyx_n_u_pipeline;
   PyObject *__pyx_n_s_post;
+  PyObject *__pyx_n_s_print;
+  PyObject *__pyx_kp_u_project;
   PyObject *__pyx_n_s_pyx_PickleError;
   PyObject *__pyx_n_s_pyx_checksum;
   PyObject *__pyx_n_s_pyx_result;
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_pyx_type;
   PyObject *__pyx_n_s_pyx_unpickle_xyellw;
+  PyObject *__pyx_n_s_query_payload;
+  PyObject *__pyx_n_s_query_vec;
+  PyObject *__pyx_n_s_re;
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_requests;
   PyObject *__pyx_n_s_response;
+  PyObject *__pyx_n_s_response_data;
+  PyObject *__pyx_n_s_result;
+  PyObject *__pyx_n_s_reverse;
   PyObject *__pyx_n_s_self;
   PyObject *__pyx_kp_u_set;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
+  PyObject *__pyx_n_s_shorten_text;
+  PyObject *__pyx_n_s_similar_score;
+  PyObject *__pyx_n_s_similarities;
+  PyObject *__pyx_n_s_similarities_values;
+  PyObject *__pyx_n_u_similarity;
+  PyObject *__pyx_n_s_sorted;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_state;
   PyObject *__pyx_n_s_status_code;
   PyObject *__pyx_n_s_strText;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_text;
   PyObject *__pyx_n_s_text_chunks;
+  PyObject *__pyx_n_s_text_embed;
   PyObject *__pyx_kp_u_text_embedding_ada_002;
   PyObject *__pyx_n_u_text_embeddings;
+  PyObject *__pyx_kp_u_text_embeddings_key_not_found_i;
   PyObject *__pyx_n_s_text_key;
+  PyObject *__pyx_n_s_top_n;
+  PyObject *__pyx_n_s_top_results;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_u_update;
   PyObject *__pyx_n_u_upsert;
+  PyObject *__pyx_n_s_url;
   PyObject *__pyx_n_s_use_setstate;
   PyObject *__pyx_kp_u_utf_8;
+  PyObject *__pyx_n_s_vector_query;
+  PyObject *__pyx_n_s_vector_search;
+  PyObject *__pyx_n_s_vector_search_locals_lambda;
+  PyObject *__pyx_n_s_vectorizeEmbedding;
+  PyObject *__pyx_n_s_vectorizeText;
+  PyObject *__pyx_n_s_x;
   PyObject *__pyx_n_s_xyellw;
   PyObject *__pyx_n_s_xyellw_Decenigma;
   PyObject *__pyx_n_s_xyellw_Decipherx;
-  PyObject *__pyx_n_s_xyellw_Embedshroud;
   PyObject *__pyx_n_s_xyellw_Encapseal;
   PyObject *__pyx_n_s_xyellw_SaveToMongoDb;
   PyObject *__pyx_n_s_xyellw___reduce_cython;
   PyObject *__pyx_n_s_xyellw___setstate_cython;
+  PyObject *__pyx_n_s_xyellw_shorten_text;
+  PyObject *__pyx_n_s_xyellw_vector_search;
+  PyObject *__pyx_n_s_xyellw_vectorizeEmbedding;
+  PyObject *__pyx_n_s_xyellw_vectorizeText;
   PyObject *__pyx_kp_b_y1c8_8BxP9XN_VKM;
+  PyObject *__pyx_int_1;
+  PyObject *__pyx_int_5;
   PyObject *__pyx_int_200;
+  PyObject *__pyx_int_1000;
   PyObject *__pyx_int_222419149;
   PyObject *__pyx_int_228825662;
   PyObject *__pyx_int_238750788;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__3;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__5;
@@ -2580,22 +2753,31 @@
   PyObject *__pyx_tuple__11;
   PyObject *__pyx_tuple__13;
   PyObject *__pyx_tuple__15;
   PyObject *__pyx_tuple__17;
   PyObject *__pyx_tuple__19;
   PyObject *__pyx_tuple__21;
   PyObject *__pyx_tuple__23;
-  PyObject *__pyx_codeobj__10;
+  PyObject *__pyx_tuple__25;
+  PyObject *__pyx_tuple__26;
+  PyObject *__pyx_tuple__28;
+  PyObject *__pyx_tuple__29;
+  PyObject *__pyx_tuple__31;
+  PyObject *__pyx_tuple__33;
   PyObject *__pyx_codeobj__12;
   PyObject *__pyx_codeobj__14;
   PyObject *__pyx_codeobj__16;
   PyObject *__pyx_codeobj__18;
   PyObject *__pyx_codeobj__20;
   PyObject *__pyx_codeobj__22;
   PyObject *__pyx_codeobj__24;
+  PyObject *__pyx_codeobj__27;
+  PyObject *__pyx_codeobj__30;
+  PyObject *__pyx_codeobj__32;
+  PyObject *__pyx_codeobj__34;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2642,47 +2824,54 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_An_unexpected_error_occurred);
   Py_CLEAR(clear_module_state->__pyx_n_s_AuthenticationError);
   Py_CLEAR(clear_module_state->__pyx_n_s_CBC);
   Py_CLEAR(clear_module_state->__pyx_n_s_Cipher);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Content_Type);
   Py_CLEAR(clear_module_state->__pyx_n_s_Decenigma);
   Py_CLEAR(clear_module_state->__pyx_n_s_Decipherx);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Embedshroud);
   Py_CLEAR(clear_module_state->__pyx_n_s_Encapseal);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_API_key_provided);
   Py_CLEAR(clear_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Request_failed_with_status_code);
   Py_CLEAR(clear_module_state->__pyx_n_s_SaveToMongoDb);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
-  Py_CLEAR(clear_module_state->__pyx_n_s__25);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Unknown_filename);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__10);
+  Py_CLEAR(clear_module_state->__pyx_n_s__35);
   Py_CLEAR(clear_module_state->__pyx_n_s__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__8);
   Py_CLEAR(clear_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_CLEAR(clear_module_state->__pyx_n_s_aixhello_xyello);
   Py_CLEAR(clear_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithms);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_key);
   Py_CLEAR(clear_module_state->__pyx_kp_u_api_key_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_url);
+  Py_CLEAR(clear_module_state->__pyx_n_s_append);
   Py_CLEAR(clear_module_state->__pyx_kp_u_application_json);
   Py_CLEAR(clear_module_state->__pyx_kp_u_application_pdf);
+  Py_CLEAR(clear_module_state->__pyx_n_s_array);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_b64decode);
   Py_CLEAR(clear_module_state->__pyx_n_s_b64encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_backend);
   Py_CLEAR(clear_module_state->__pyx_n_s_base64);
   Py_CLEAR(clear_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_chr);
   Py_CLEAR(clear_module_state->__pyx_n_s_chunk);
   Py_CLEAR(clear_module_state->__pyx_n_s_cipher);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cleaned_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_collection);
   Py_CLEAR(clear_module_state->__pyx_n_u_collection);
+  Py_CLEAR(clear_module_state->__pyx_n_s_connParam);
   Py_CLEAR(clear_module_state->__pyx_n_s_create);
   Py_CLEAR(clear_module_state->__pyx_n_s_cryptography_hazmat_backends);
   Py_CLEAR(clear_module_state->__pyx_n_s_cryptography_hazmat_primitives_c);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
   Py_CLEAR(clear_module_state->__pyx_n_u_dataSource);
   Py_CLEAR(clear_module_state->__pyx_n_s_database);
   Py_CLEAR(clear_module_state->__pyx_n_u_database);
@@ -2693,98 +2882,146 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_decrypted_padded_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_decrypted_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_decryptor);
   Py_CLEAR(clear_module_state->__pyx_n_s_default_backend);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict_2);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_doc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_documents);
+  Py_CLEAR(clear_module_state->__pyx_n_u_documents);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dot);
   Py_CLEAR(clear_module_state->__pyx_n_s_e);
+  Py_CLEAR(clear_module_state->__pyx_n_s_emb);
+  Py_CLEAR(clear_module_state->__pyx_n_s_emb_vec);
   Py_CLEAR(clear_module_state->__pyx_n_s_embedding);
   Py_CLEAR(clear_module_state->__pyx_n_s_embeddings);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_encoded_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptor);
   Py_CLEAR(clear_module_state->__pyx_n_s_enkyc);
+  Py_CLEAR(clear_module_state->__pyx_n_u_enkyc);
   Py_CLEAR(clear_module_state->__pyx_n_u_error);
   Py_CLEAR(clear_module_state->__pyx_n_u_extracted_text);
+  Py_CLEAR(clear_module_state->__pyx_n_s_extracted_text_length);
+  Py_CLEAR(clear_module_state->__pyx_n_s_extracted_texts);
   Py_CLEAR(clear_module_state->__pyx_n_u_file_data);
   Py_CLEAR(clear_module_state->__pyx_n_u_file_type);
   Py_CLEAR(clear_module_state->__pyx_n_u_filename);
+  Py_CLEAR(clear_module_state->__pyx_n_s_filenames);
   Py_CLEAR(clear_module_state->__pyx_n_u_filter);
   Py_CLEAR(clear_module_state->__pyx_n_s_finalize);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_get);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_headers);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
   Py_CLEAR(clear_module_state->__pyx_n_s_input);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_iv);
   Py_CLEAR(clear_module_state->__pyx_n_s_json);
   Py_CLEAR(clear_module_state->__pyx_n_s_key);
+  Py_CLEAR(clear_module_state->__pyx_n_s_linalg);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_max_length);
   Py_CLEAR(clear_module_state->__pyx_n_u_message);
   Py_CLEAR(clear_module_state->__pyx_n_s_model);
   Py_CLEAR(clear_module_state->__pyx_n_s_modes);
   Py_CLEAR(clear_module_state->__pyx_n_s_msg);
   Py_CLEAR(clear_module_state->__pyx_n_s_mth);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
+  Py_CLEAR(clear_module_state->__pyx_n_s_norm);
+  Py_CLEAR(clear_module_state->__pyx_n_s_np);
+  Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
   Py_CLEAR(clear_module_state->__pyx_n_s_openai);
   Py_CLEAR(clear_module_state->__pyx_n_s_pad_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_padded_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_params_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_payload);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pipeline);
+  Py_CLEAR(clear_module_state->__pyx_n_u_pipeline);
   Py_CLEAR(clear_module_state->__pyx_n_s_post);
+  Py_CLEAR(clear_module_state->__pyx_n_s_print);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_project);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_xyellw);
+  Py_CLEAR(clear_module_state->__pyx_n_s_query_payload);
+  Py_CLEAR(clear_module_state->__pyx_n_s_query_vec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_re);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_requests);
   Py_CLEAR(clear_module_state->__pyx_n_s_response);
+  Py_CLEAR(clear_module_state->__pyx_n_s_response_data);
+  Py_CLEAR(clear_module_state->__pyx_n_s_result);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reverse);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_kp_u_set);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_shorten_text);
+  Py_CLEAR(clear_module_state->__pyx_n_s_similar_score);
+  Py_CLEAR(clear_module_state->__pyx_n_s_similarities);
+  Py_CLEAR(clear_module_state->__pyx_n_s_similarities_values);
+  Py_CLEAR(clear_module_state->__pyx_n_u_similarity);
+  Py_CLEAR(clear_module_state->__pyx_n_s_sorted);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_status_code);
   Py_CLEAR(clear_module_state->__pyx_n_s_strText);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_text_chunks);
+  Py_CLEAR(clear_module_state->__pyx_n_s_text_embed);
   Py_CLEAR(clear_module_state->__pyx_kp_u_text_embedding_ada_002);
   Py_CLEAR(clear_module_state->__pyx_n_u_text_embeddings);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_text_embeddings_key_not_found_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_text_key);
+  Py_CLEAR(clear_module_state->__pyx_n_s_top_n);
+  Py_CLEAR(clear_module_state->__pyx_n_s_top_results);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_u_update);
   Py_CLEAR(clear_module_state->__pyx_n_u_upsert);
+  Py_CLEAR(clear_module_state->__pyx_n_s_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
+  Py_CLEAR(clear_module_state->__pyx_n_s_vector_query);
+  Py_CLEAR(clear_module_state->__pyx_n_s_vector_search);
+  Py_CLEAR(clear_module_state->__pyx_n_s_vector_search_locals_lambda);
+  Py_CLEAR(clear_module_state->__pyx_n_s_vectorizeEmbedding);
+  Py_CLEAR(clear_module_state->__pyx_n_s_vectorizeText);
+  Py_CLEAR(clear_module_state->__pyx_n_s_x);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decipherx);
-  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Embedshroud);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Encapseal);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_SaveToMongoDb);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_shorten_text);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vector_search);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vectorizeEmbedding);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vectorizeText);
   Py_CLEAR(clear_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
+  Py_CLEAR(clear_module_state->__pyx_int_1);
+  Py_CLEAR(clear_module_state->__pyx_int_5);
   Py_CLEAR(clear_module_state->__pyx_int_200);
+  Py_CLEAR(clear_module_state->__pyx_int_1000);
   Py_CLEAR(clear_module_state->__pyx_int_222419149);
   Py_CLEAR(clear_module_state->__pyx_int_228825662);
   Py_CLEAR(clear_module_state->__pyx_int_238750788);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__5);
@@ -2793,22 +3030,31 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__11);
   Py_CLEAR(clear_module_state->__pyx_tuple__13);
   Py_CLEAR(clear_module_state->__pyx_tuple__15);
   Py_CLEAR(clear_module_state->__pyx_tuple__17);
   Py_CLEAR(clear_module_state->__pyx_tuple__19);
   Py_CLEAR(clear_module_state->__pyx_tuple__21);
   Py_CLEAR(clear_module_state->__pyx_tuple__23);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
+  Py_CLEAR(clear_module_state->__pyx_tuple__25);
+  Py_CLEAR(clear_module_state->__pyx_tuple__26);
+  Py_CLEAR(clear_module_state->__pyx_tuple__28);
+  Py_CLEAR(clear_module_state->__pyx_tuple__29);
+  Py_CLEAR(clear_module_state->__pyx_tuple__31);
+  Py_CLEAR(clear_module_state->__pyx_tuple__33);
   Py_CLEAR(clear_module_state->__pyx_codeobj__12);
   Py_CLEAR(clear_module_state->__pyx_codeobj__14);
   Py_CLEAR(clear_module_state->__pyx_codeobj__16);
   Py_CLEAR(clear_module_state->__pyx_codeobj__18);
   Py_CLEAR(clear_module_state->__pyx_codeobj__20);
   Py_CLEAR(clear_module_state->__pyx_codeobj__22);
   Py_CLEAR(clear_module_state->__pyx_codeobj__24);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__27);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__30);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__32);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__34);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -2833,47 +3079,54 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_An_unexpected_error_occurred);
   Py_VISIT(traverse_module_state->__pyx_n_s_AuthenticationError);
   Py_VISIT(traverse_module_state->__pyx_n_s_CBC);
   Py_VISIT(traverse_module_state->__pyx_n_s_Cipher);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Content_Type);
   Py_VISIT(traverse_module_state->__pyx_n_s_Decenigma);
   Py_VISIT(traverse_module_state->__pyx_n_s_Decipherx);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Embedshroud);
   Py_VISIT(traverse_module_state->__pyx_n_s_Encapseal);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_API_key_provided);
   Py_VISIT(traverse_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Request_failed_with_status_code);
   Py_VISIT(traverse_module_state->__pyx_n_s_SaveToMongoDb);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
-  Py_VISIT(traverse_module_state->__pyx_n_s__25);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Unknown_filename);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__10);
+  Py_VISIT(traverse_module_state->__pyx_n_s__35);
   Py_VISIT(traverse_module_state->__pyx_n_s__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__8);
   Py_VISIT(traverse_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_VISIT(traverse_module_state->__pyx_n_s_aixhello_xyello);
   Py_VISIT(traverse_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithms);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_key);
   Py_VISIT(traverse_module_state->__pyx_kp_u_api_key_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_url);
+  Py_VISIT(traverse_module_state->__pyx_n_s_append);
   Py_VISIT(traverse_module_state->__pyx_kp_u_application_json);
   Py_VISIT(traverse_module_state->__pyx_kp_u_application_pdf);
+  Py_VISIT(traverse_module_state->__pyx_n_s_array);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_b64decode);
   Py_VISIT(traverse_module_state->__pyx_n_s_b64encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_backend);
   Py_VISIT(traverse_module_state->__pyx_n_s_base64);
   Py_VISIT(traverse_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_chr);
   Py_VISIT(traverse_module_state->__pyx_n_s_chunk);
   Py_VISIT(traverse_module_state->__pyx_n_s_cipher);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cleaned_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_collection);
   Py_VISIT(traverse_module_state->__pyx_n_u_collection);
+  Py_VISIT(traverse_module_state->__pyx_n_s_connParam);
   Py_VISIT(traverse_module_state->__pyx_n_s_create);
   Py_VISIT(traverse_module_state->__pyx_n_s_cryptography_hazmat_backends);
   Py_VISIT(traverse_module_state->__pyx_n_s_cryptography_hazmat_primitives_c);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
   Py_VISIT(traverse_module_state->__pyx_n_u_dataSource);
   Py_VISIT(traverse_module_state->__pyx_n_s_database);
   Py_VISIT(traverse_module_state->__pyx_n_u_database);
@@ -2884,98 +3137,146 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_decrypted_padded_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_decrypted_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_decryptor);
   Py_VISIT(traverse_module_state->__pyx_n_s_default_backend);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict_2);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_doc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_documents);
+  Py_VISIT(traverse_module_state->__pyx_n_u_documents);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dot);
   Py_VISIT(traverse_module_state->__pyx_n_s_e);
+  Py_VISIT(traverse_module_state->__pyx_n_s_emb);
+  Py_VISIT(traverse_module_state->__pyx_n_s_emb_vec);
   Py_VISIT(traverse_module_state->__pyx_n_s_embedding);
   Py_VISIT(traverse_module_state->__pyx_n_s_embeddings);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_encoded_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptor);
   Py_VISIT(traverse_module_state->__pyx_n_s_enkyc);
+  Py_VISIT(traverse_module_state->__pyx_n_u_enkyc);
   Py_VISIT(traverse_module_state->__pyx_n_u_error);
   Py_VISIT(traverse_module_state->__pyx_n_u_extracted_text);
+  Py_VISIT(traverse_module_state->__pyx_n_s_extracted_text_length);
+  Py_VISIT(traverse_module_state->__pyx_n_s_extracted_texts);
   Py_VISIT(traverse_module_state->__pyx_n_u_file_data);
   Py_VISIT(traverse_module_state->__pyx_n_u_file_type);
   Py_VISIT(traverse_module_state->__pyx_n_u_filename);
+  Py_VISIT(traverse_module_state->__pyx_n_s_filenames);
   Py_VISIT(traverse_module_state->__pyx_n_u_filter);
   Py_VISIT(traverse_module_state->__pyx_n_s_finalize);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_get);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_headers);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
   Py_VISIT(traverse_module_state->__pyx_n_s_input);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_iv);
   Py_VISIT(traverse_module_state->__pyx_n_s_json);
   Py_VISIT(traverse_module_state->__pyx_n_s_key);
+  Py_VISIT(traverse_module_state->__pyx_n_s_linalg);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_max_length);
   Py_VISIT(traverse_module_state->__pyx_n_u_message);
   Py_VISIT(traverse_module_state->__pyx_n_s_model);
   Py_VISIT(traverse_module_state->__pyx_n_s_modes);
   Py_VISIT(traverse_module_state->__pyx_n_s_msg);
   Py_VISIT(traverse_module_state->__pyx_n_s_mth);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
+  Py_VISIT(traverse_module_state->__pyx_n_s_norm);
+  Py_VISIT(traverse_module_state->__pyx_n_s_np);
+  Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
   Py_VISIT(traverse_module_state->__pyx_n_s_openai);
   Py_VISIT(traverse_module_state->__pyx_n_s_pad_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_padded_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_params_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_payload);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pipeline);
+  Py_VISIT(traverse_module_state->__pyx_n_u_pipeline);
   Py_VISIT(traverse_module_state->__pyx_n_s_post);
+  Py_VISIT(traverse_module_state->__pyx_n_s_print);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_project);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_xyellw);
+  Py_VISIT(traverse_module_state->__pyx_n_s_query_payload);
+  Py_VISIT(traverse_module_state->__pyx_n_s_query_vec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_re);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_requests);
   Py_VISIT(traverse_module_state->__pyx_n_s_response);
+  Py_VISIT(traverse_module_state->__pyx_n_s_response_data);
+  Py_VISIT(traverse_module_state->__pyx_n_s_result);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reverse);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_kp_u_set);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_shorten_text);
+  Py_VISIT(traverse_module_state->__pyx_n_s_similar_score);
+  Py_VISIT(traverse_module_state->__pyx_n_s_similarities);
+  Py_VISIT(traverse_module_state->__pyx_n_s_similarities_values);
+  Py_VISIT(traverse_module_state->__pyx_n_u_similarity);
+  Py_VISIT(traverse_module_state->__pyx_n_s_sorted);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_status_code);
   Py_VISIT(traverse_module_state->__pyx_n_s_strText);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_text_chunks);
+  Py_VISIT(traverse_module_state->__pyx_n_s_text_embed);
   Py_VISIT(traverse_module_state->__pyx_kp_u_text_embedding_ada_002);
   Py_VISIT(traverse_module_state->__pyx_n_u_text_embeddings);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_text_embeddings_key_not_found_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_text_key);
+  Py_VISIT(traverse_module_state->__pyx_n_s_top_n);
+  Py_VISIT(traverse_module_state->__pyx_n_s_top_results);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_u_update);
   Py_VISIT(traverse_module_state->__pyx_n_u_upsert);
+  Py_VISIT(traverse_module_state->__pyx_n_s_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
+  Py_VISIT(traverse_module_state->__pyx_n_s_vector_query);
+  Py_VISIT(traverse_module_state->__pyx_n_s_vector_search);
+  Py_VISIT(traverse_module_state->__pyx_n_s_vector_search_locals_lambda);
+  Py_VISIT(traverse_module_state->__pyx_n_s_vectorizeEmbedding);
+  Py_VISIT(traverse_module_state->__pyx_n_s_vectorizeText);
+  Py_VISIT(traverse_module_state->__pyx_n_s_x);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decipherx);
-  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Embedshroud);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Encapseal);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_SaveToMongoDb);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_shorten_text);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vector_search);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vectorizeEmbedding);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vectorizeText);
   Py_VISIT(traverse_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
+  Py_VISIT(traverse_module_state->__pyx_int_1);
+  Py_VISIT(traverse_module_state->__pyx_int_5);
   Py_VISIT(traverse_module_state->__pyx_int_200);
+  Py_VISIT(traverse_module_state->__pyx_int_1000);
   Py_VISIT(traverse_module_state->__pyx_int_222419149);
   Py_VISIT(traverse_module_state->__pyx_int_228825662);
   Py_VISIT(traverse_module_state->__pyx_int_238750788);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__5);
@@ -2984,22 +3285,31 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__11);
   Py_VISIT(traverse_module_state->__pyx_tuple__13);
   Py_VISIT(traverse_module_state->__pyx_tuple__15);
   Py_VISIT(traverse_module_state->__pyx_tuple__17);
   Py_VISIT(traverse_module_state->__pyx_tuple__19);
   Py_VISIT(traverse_module_state->__pyx_tuple__21);
   Py_VISIT(traverse_module_state->__pyx_tuple__23);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
+  Py_VISIT(traverse_module_state->__pyx_tuple__25);
+  Py_VISIT(traverse_module_state->__pyx_tuple__26);
+  Py_VISIT(traverse_module_state->__pyx_tuple__28);
+  Py_VISIT(traverse_module_state->__pyx_tuple__29);
+  Py_VISIT(traverse_module_state->__pyx_tuple__31);
+  Py_VISIT(traverse_module_state->__pyx_tuple__33);
   Py_VISIT(traverse_module_state->__pyx_codeobj__12);
   Py_VISIT(traverse_module_state->__pyx_codeobj__14);
   Py_VISIT(traverse_module_state->__pyx_codeobj__16);
   Py_VISIT(traverse_module_state->__pyx_codeobj__18);
   Py_VISIT(traverse_module_state->__pyx_codeobj__20);
   Py_VISIT(traverse_module_state->__pyx_codeobj__22);
   Py_VISIT(traverse_module_state->__pyx_codeobj__24);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__27);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__30);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__32);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__34);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3034,47 +3344,54 @@
 #define __pyx_kp_u_An_unexpected_error_occurred __pyx_mstate_global->__pyx_kp_u_An_unexpected_error_occurred
 #define __pyx_n_s_AuthenticationError __pyx_mstate_global->__pyx_n_s_AuthenticationError
 #define __pyx_n_s_CBC __pyx_mstate_global->__pyx_n_s_CBC
 #define __pyx_n_s_Cipher __pyx_mstate_global->__pyx_n_s_Cipher
 #define __pyx_kp_u_Content_Type __pyx_mstate_global->__pyx_kp_u_Content_Type
 #define __pyx_n_s_Decenigma __pyx_mstate_global->__pyx_n_s_Decenigma
 #define __pyx_n_s_Decipherx __pyx_mstate_global->__pyx_n_s_Decipherx
-#define __pyx_n_s_Embedshroud __pyx_mstate_global->__pyx_n_s_Embedshroud
 #define __pyx_n_s_Encapseal __pyx_mstate_global->__pyx_n_s_Encapseal
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_kp_u_Invalid_API_key_provided __pyx_mstate_global->__pyx_kp_u_Invalid_API_key_provided
 #define __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN __pyx_mstate_global->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
+#define __pyx_kp_u_Request_failed_with_status_code __pyx_mstate_global->__pyx_kp_u_Request_failed_with_status_code
 #define __pyx_n_s_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_SaveToMongoDb
 #define __pyx_kp_u_Successfully_save_to_the_databas __pyx_mstate_global->__pyx_kp_u_Successfully_save_to_the_databas
-#define __pyx_n_s__25 __pyx_mstate_global->__pyx_n_s__25
+#define __pyx_kp_u_Unknown_filename __pyx_mstate_global->__pyx_kp_u_Unknown_filename
+#define __pyx_kp_u__10 __pyx_mstate_global->__pyx_kp_u__10
+#define __pyx_n_s__35 __pyx_mstate_global->__pyx_n_s__35
 #define __pyx_n_s__6 __pyx_mstate_global->__pyx_n_s__6
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
 #define __pyx_kp_u__8 __pyx_mstate_global->__pyx_kp_u__8
 #define __pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1 __pyx_mstate_global->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1
 #define __pyx_n_s_aixhello_xyello __pyx_mstate_global->__pyx_n_s_aixhello_xyello
 #define __pyx_kp_s_aixhello_xyello_pyx __pyx_mstate_global->__pyx_kp_s_aixhello_xyello_pyx
 #define __pyx_n_s_algorithms __pyx_mstate_global->__pyx_n_s_algorithms
 #define __pyx_n_s_api_key __pyx_mstate_global->__pyx_n_s_api_key
 #define __pyx_kp_u_api_key_2 __pyx_mstate_global->__pyx_kp_u_api_key_2
 #define __pyx_n_s_api_url __pyx_mstate_global->__pyx_n_s_api_url
+#define __pyx_n_s_append __pyx_mstate_global->__pyx_n_s_append
 #define __pyx_kp_u_application_json __pyx_mstate_global->__pyx_kp_u_application_json
 #define __pyx_kp_u_application_pdf __pyx_mstate_global->__pyx_kp_u_application_pdf
+#define __pyx_n_s_array __pyx_mstate_global->__pyx_n_s_array
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_b64decode __pyx_mstate_global->__pyx_n_s_b64decode
 #define __pyx_n_s_b64encode __pyx_mstate_global->__pyx_n_s_b64encode
 #define __pyx_n_s_backend __pyx_mstate_global->__pyx_n_s_backend
 #define __pyx_n_s_base64 __pyx_mstate_global->__pyx_n_s_base64
 #define __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn __pyx_mstate_global->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn
+#define __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2 __pyx_mstate_global->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2
 #define __pyx_n_s_chr __pyx_mstate_global->__pyx_n_s_chr
 #define __pyx_n_s_chunk __pyx_mstate_global->__pyx_n_s_chunk
 #define __pyx_n_s_cipher __pyx_mstate_global->__pyx_n_s_cipher
+#define __pyx_n_s_cleaned_text __pyx_mstate_global->__pyx_n_s_cleaned_text
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_collection __pyx_mstate_global->__pyx_n_s_collection
 #define __pyx_n_u_collection __pyx_mstate_global->__pyx_n_u_collection
+#define __pyx_n_s_connParam __pyx_mstate_global->__pyx_n_s_connParam
 #define __pyx_n_s_create __pyx_mstate_global->__pyx_n_s_create
 #define __pyx_n_s_cryptography_hazmat_backends __pyx_mstate_global->__pyx_n_s_cryptography_hazmat_backends
 #define __pyx_n_s_cryptography_hazmat_primitives_c __pyx_mstate_global->__pyx_n_s_cryptography_hazmat_primitives_c
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
 #define __pyx_n_u_dataSource __pyx_mstate_global->__pyx_n_u_dataSource
 #define __pyx_n_s_database __pyx_mstate_global->__pyx_n_s_database
 #define __pyx_n_u_database __pyx_mstate_global->__pyx_n_u_database
@@ -3085,98 +3402,146 @@
 #define __pyx_n_s_decrypted_padded_text __pyx_mstate_global->__pyx_n_s_decrypted_padded_text
 #define __pyx_n_s_decrypted_url __pyx_mstate_global->__pyx_n_s_decrypted_url
 #define __pyx_n_s_decryptor __pyx_mstate_global->__pyx_n_s_decryptor
 #define __pyx_n_s_default_backend __pyx_mstate_global->__pyx_n_s_default_backend
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_dict_2 __pyx_mstate_global->__pyx_n_s_dict_2
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
+#define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
+#define __pyx_n_s_documents __pyx_mstate_global->__pyx_n_s_documents
+#define __pyx_n_u_documents __pyx_mstate_global->__pyx_n_u_documents
+#define __pyx_n_s_dot __pyx_mstate_global->__pyx_n_s_dot
 #define __pyx_n_s_e __pyx_mstate_global->__pyx_n_s_e
+#define __pyx_n_s_emb __pyx_mstate_global->__pyx_n_s_emb
+#define __pyx_n_s_emb_vec __pyx_mstate_global->__pyx_n_s_emb_vec
 #define __pyx_n_s_embedding __pyx_mstate_global->__pyx_n_s_embedding
 #define __pyx_n_s_embeddings __pyx_mstate_global->__pyx_n_s_embeddings
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_encoded_url __pyx_mstate_global->__pyx_n_s_encoded_url
 #define __pyx_n_s_encryptedText __pyx_mstate_global->__pyx_n_s_encryptedText
 #define __pyx_n_s_encryptor __pyx_mstate_global->__pyx_n_s_encryptor
 #define __pyx_n_s_enkyc __pyx_mstate_global->__pyx_n_s_enkyc
+#define __pyx_n_u_enkyc __pyx_mstate_global->__pyx_n_u_enkyc
 #define __pyx_n_u_error __pyx_mstate_global->__pyx_n_u_error
 #define __pyx_n_u_extracted_text __pyx_mstate_global->__pyx_n_u_extracted_text
+#define __pyx_n_s_extracted_text_length __pyx_mstate_global->__pyx_n_s_extracted_text_length
+#define __pyx_n_s_extracted_texts __pyx_mstate_global->__pyx_n_s_extracted_texts
 #define __pyx_n_u_file_data __pyx_mstate_global->__pyx_n_u_file_data
 #define __pyx_n_u_file_type __pyx_mstate_global->__pyx_n_u_file_type
 #define __pyx_n_u_filename __pyx_mstate_global->__pyx_n_u_filename
+#define __pyx_n_s_filenames __pyx_mstate_global->__pyx_n_s_filenames
 #define __pyx_n_u_filter __pyx_mstate_global->__pyx_n_u_filter
 #define __pyx_n_s_finalize __pyx_mstate_global->__pyx_n_s_finalize
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_get __pyx_mstate_global->__pyx_n_s_get
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_n_s_headers __pyx_mstate_global->__pyx_n_s_headers
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
 #define __pyx_n_s_input __pyx_mstate_global->__pyx_n_s_input
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_iv __pyx_mstate_global->__pyx_n_s_iv
 #define __pyx_n_s_json __pyx_mstate_global->__pyx_n_s_json
 #define __pyx_n_s_key __pyx_mstate_global->__pyx_n_s_key
+#define __pyx_n_s_linalg __pyx_mstate_global->__pyx_n_s_linalg
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_max_length __pyx_mstate_global->__pyx_n_s_max_length
 #define __pyx_n_u_message __pyx_mstate_global->__pyx_n_u_message
 #define __pyx_n_s_model __pyx_mstate_global->__pyx_n_s_model
 #define __pyx_n_s_modes __pyx_mstate_global->__pyx_n_s_modes
 #define __pyx_n_s_msg __pyx_mstate_global->__pyx_n_s_msg
 #define __pyx_n_s_mth __pyx_mstate_global->__pyx_n_s_mth
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
+#define __pyx_n_s_norm __pyx_mstate_global->__pyx_n_s_norm
+#define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
+#define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
 #define __pyx_n_s_openai __pyx_mstate_global->__pyx_n_s_openai
 #define __pyx_n_s_pad_length __pyx_mstate_global->__pyx_n_s_pad_length
 #define __pyx_n_s_padded_text __pyx_mstate_global->__pyx_n_s_padded_text
 #define __pyx_n_s_params_dict __pyx_mstate_global->__pyx_n_s_params_dict
 #define __pyx_n_s_payload __pyx_mstate_global->__pyx_n_s_payload
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
+#define __pyx_n_s_pipeline __pyx_mstate_global->__pyx_n_s_pipeline
+#define __pyx_n_u_pipeline __pyx_mstate_global->__pyx_n_u_pipeline
 #define __pyx_n_s_post __pyx_mstate_global->__pyx_n_s_post
+#define __pyx_n_s_print __pyx_mstate_global->__pyx_n_s_print
+#define __pyx_kp_u_project __pyx_mstate_global->__pyx_kp_u_project
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
 #define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
 #define __pyx_n_s_pyx_unpickle_xyellw __pyx_mstate_global->__pyx_n_s_pyx_unpickle_xyellw
+#define __pyx_n_s_query_payload __pyx_mstate_global->__pyx_n_s_query_payload
+#define __pyx_n_s_query_vec __pyx_mstate_global->__pyx_n_s_query_vec
+#define __pyx_n_s_re __pyx_mstate_global->__pyx_n_s_re
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_requests __pyx_mstate_global->__pyx_n_s_requests
 #define __pyx_n_s_response __pyx_mstate_global->__pyx_n_s_response
+#define __pyx_n_s_response_data __pyx_mstate_global->__pyx_n_s_response_data
+#define __pyx_n_s_result __pyx_mstate_global->__pyx_n_s_result
+#define __pyx_n_s_reverse __pyx_mstate_global->__pyx_n_s_reverse
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_kp_u_set __pyx_mstate_global->__pyx_kp_u_set
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
+#define __pyx_n_s_shorten_text __pyx_mstate_global->__pyx_n_s_shorten_text
+#define __pyx_n_s_similar_score __pyx_mstate_global->__pyx_n_s_similar_score
+#define __pyx_n_s_similarities __pyx_mstate_global->__pyx_n_s_similarities
+#define __pyx_n_s_similarities_values __pyx_mstate_global->__pyx_n_s_similarities_values
+#define __pyx_n_u_similarity __pyx_mstate_global->__pyx_n_u_similarity
+#define __pyx_n_s_sorted __pyx_mstate_global->__pyx_n_s_sorted
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_state __pyx_mstate_global->__pyx_n_s_state
 #define __pyx_n_s_status_code __pyx_mstate_global->__pyx_n_s_status_code
 #define __pyx_n_s_strText __pyx_mstate_global->__pyx_n_s_strText
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_text __pyx_mstate_global->__pyx_n_s_text
 #define __pyx_n_s_text_chunks __pyx_mstate_global->__pyx_n_s_text_chunks
+#define __pyx_n_s_text_embed __pyx_mstate_global->__pyx_n_s_text_embed
 #define __pyx_kp_u_text_embedding_ada_002 __pyx_mstate_global->__pyx_kp_u_text_embedding_ada_002
 #define __pyx_n_u_text_embeddings __pyx_mstate_global->__pyx_n_u_text_embeddings
+#define __pyx_kp_u_text_embeddings_key_not_found_i __pyx_mstate_global->__pyx_kp_u_text_embeddings_key_not_found_i
 #define __pyx_n_s_text_key __pyx_mstate_global->__pyx_n_s_text_key
+#define __pyx_n_s_top_n __pyx_mstate_global->__pyx_n_s_top_n
+#define __pyx_n_s_top_results __pyx_mstate_global->__pyx_n_s_top_results
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_u_update __pyx_mstate_global->__pyx_n_u_update
 #define __pyx_n_u_upsert __pyx_mstate_global->__pyx_n_u_upsert
+#define __pyx_n_s_url __pyx_mstate_global->__pyx_n_s_url
 #define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
+#define __pyx_n_s_vector_query __pyx_mstate_global->__pyx_n_s_vector_query
+#define __pyx_n_s_vector_search __pyx_mstate_global->__pyx_n_s_vector_search
+#define __pyx_n_s_vector_search_locals_lambda __pyx_mstate_global->__pyx_n_s_vector_search_locals_lambda
+#define __pyx_n_s_vectorizeEmbedding __pyx_mstate_global->__pyx_n_s_vectorizeEmbedding
+#define __pyx_n_s_vectorizeText __pyx_mstate_global->__pyx_n_s_vectorizeText
+#define __pyx_n_s_x __pyx_mstate_global->__pyx_n_s_x
 #define __pyx_n_s_xyellw __pyx_mstate_global->__pyx_n_s_xyellw
 #define __pyx_n_s_xyellw_Decenigma __pyx_mstate_global->__pyx_n_s_xyellw_Decenigma
 #define __pyx_n_s_xyellw_Decipherx __pyx_mstate_global->__pyx_n_s_xyellw_Decipherx
-#define __pyx_n_s_xyellw_Embedshroud __pyx_mstate_global->__pyx_n_s_xyellw_Embedshroud
 #define __pyx_n_s_xyellw_Encapseal __pyx_mstate_global->__pyx_n_s_xyellw_Encapseal
 #define __pyx_n_s_xyellw_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_xyellw_SaveToMongoDb
 #define __pyx_n_s_xyellw___reduce_cython __pyx_mstate_global->__pyx_n_s_xyellw___reduce_cython
 #define __pyx_n_s_xyellw___setstate_cython __pyx_mstate_global->__pyx_n_s_xyellw___setstate_cython
+#define __pyx_n_s_xyellw_shorten_text __pyx_mstate_global->__pyx_n_s_xyellw_shorten_text
+#define __pyx_n_s_xyellw_vector_search __pyx_mstate_global->__pyx_n_s_xyellw_vector_search
+#define __pyx_n_s_xyellw_vectorizeEmbedding __pyx_mstate_global->__pyx_n_s_xyellw_vectorizeEmbedding
+#define __pyx_n_s_xyellw_vectorizeText __pyx_mstate_global->__pyx_n_s_xyellw_vectorizeText
 #define __pyx_kp_b_y1c8_8BxP9XN_VKM __pyx_mstate_global->__pyx_kp_b_y1c8_8BxP9XN_VKM
+#define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
+#define __pyx_int_5 __pyx_mstate_global->__pyx_int_5
 #define __pyx_int_200 __pyx_mstate_global->__pyx_int_200
+#define __pyx_int_1000 __pyx_mstate_global->__pyx_int_1000
 #define __pyx_int_222419149 __pyx_mstate_global->__pyx_int_222419149
 #define __pyx_int_228825662 __pyx_mstate_global->__pyx_int_228825662
 #define __pyx_int_238750788 __pyx_mstate_global->__pyx_int_238750788
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
@@ -3185,22 +3550,31 @@
 #define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
 #define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
 #define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
 #define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
 #define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
-#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
+#define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
+#define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
+#define __pyx_tuple__28 __pyx_mstate_global->__pyx_tuple__28
+#define __pyx_tuple__29 __pyx_mstate_global->__pyx_tuple__29
+#define __pyx_tuple__31 __pyx_mstate_global->__pyx_tuple__31
+#define __pyx_tuple__33 __pyx_mstate_global->__pyx_tuple__33
 #define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
 #define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
 #define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
 #define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
 #define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
 #define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
 #define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
+#define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
+#define __pyx_codeobj__30 __pyx_mstate_global->__pyx_codeobj__30
+#define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
+#define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
 /* #### Code section: module_code ### */
 
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -3249,45 +3623,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_msg)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 9, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 11, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Decipherx") < 0)) __PYX_ERR(0, 9, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Decipherx") < 0)) __PYX_ERR(0, 11, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_msg = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("Decipherx", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 9, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Decipherx", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 11, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.Decipherx", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_msg), (&PyUnicode_Type), 1, "msg", 1))) __PYX_ERR(0, 9, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_msg), (&PyUnicode_Type), 1, "msg", 1))) __PYX_ERR(0, 11, __pyx_L1_error)
   __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_msg);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -3316,17 +3690,17 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Decipherx", 1);
 
   __Pyx_INCREF(__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   __pyx_v_encoded_url = __pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
@@ -3339,19 +3713,19 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_encoded_url};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
@@ -3364,48 +3738,48 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_kp_u_utf_8};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_v_api_url = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_requests); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_requests); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_api_url);
   __Pyx_GIVEREF(__pyx_v_api_url);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_api_url)) __PYX_ERR(0, 13, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_api_url)) __PYX_ERR(0, 15, __pyx_L1_error);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_message, __pyx_v_msg) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_t_3) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_message, __pyx_v_msg) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_t_3) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_response = __pyx_t_3;
   __pyx_t_3 = 0;
 
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
 
   /* function exit code */
@@ -3475,45 +3849,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_strText)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 16, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 18, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Encapseal") < 0)) __PYX_ERR(0, 16, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Encapseal") < 0)) __PYX_ERR(0, 18, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_strText = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("Encapseal", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 16, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Encapseal", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 18, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.Encapseal", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_strText), (&PyUnicode_Type), 1, "strText", 1))) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_strText), (&PyUnicode_Type), 1, "strText", 1))) __PYX_ERR(0, 18, __pyx_L1_error)
   __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_strText);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -3553,17 +3927,17 @@
 
   __Pyx_INCREF(__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   __pyx_v_key = __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
 
   __Pyx_INCREF(__pyx_kp_b_y1c8_8BxP9XN_VKM);
   __pyx_v_iv = __pyx_kp_b_y1c8_8BxP9XN_VKM;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_algorithms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_algorithms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_AES); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_AES); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -3576,22 +3950,22 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_key};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_mth = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_backend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_backend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -3603,26 +3977,26 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_backend = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Cipher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Cipher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_modes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_modes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CBC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CBC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
@@ -3635,38 +4009,38 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_iv};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_mth);
   __Pyx_GIVEREF(__pyx_v_mth);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_mth)) __PYX_ERR(0, 21, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_mth)) __PYX_ERR(0, 23, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_backend, __pyx_v_backend) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_backend, __pyx_v_backend) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cipher = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher, __pyx_n_s_encryptor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher, __pyx_n_s_encryptor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
@@ -3678,45 +4052,45 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_encryptor = __pyx_t_2;
   __pyx_t_2 = 0;
 
   if (unlikely(__pyx_v_strText == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 25, __pyx_L1_error)
+    __PYX_ERR(0, 27, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_strText); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 25, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t((16 - __Pyx_mod_Py_ssize_t(__pyx_t_6, 16))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_strText); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t((16 - __Pyx_mod_Py_ssize_t(__pyx_t_6, 16))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_pad_length = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_v_pad_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_v_pad_length); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_2, __pyx_v_pad_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_2, __pyx_v_pad_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_v_strText, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_v_strText, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_padded_text = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_encryptor, __pyx_n_s_update); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_encryptor, __pyx_n_s_update); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_padded_text, __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_padded_text, __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_7 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_7)) {
@@ -3728,15 +4102,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_kp_u_utf_8};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_t_1 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
@@ -3751,19 +4125,19 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_t_5};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_encryptor, __pyx_n_s_finalize); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_encryptor, __pyx_n_s_finalize); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_1 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_1)) {
@@ -3775,29 +4149,29 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyNumber_Add(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Add(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_encryptedText = __pyx_t_5;
   __pyx_t_5 = 0;
 
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
@@ -3810,19 +4184,19 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_encryptedText};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 29, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 31, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
@@ -3835,15 +4209,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_utf_8};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 29, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 31, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
@@ -3922,45 +4296,45 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_encryptedText)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 33, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Decenigma") < 0)) __PYX_ERR(0, 31, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Decenigma") < 0)) __PYX_ERR(0, 33, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_encryptedText = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("Decenigma", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 31, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Decenigma", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 33, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.Decenigma", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_encryptedText), (&PyUnicode_Type), 1, "encryptedText", 1))) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_encryptedText), (&PyUnicode_Type), 1, "encryptedText", 1))) __PYX_ERR(0, 33, __pyx_L1_error)
   __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_encryptedText);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -3999,17 +4373,17 @@
 
   __Pyx_INCREF(__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   __pyx_v_key = __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
 
   __Pyx_INCREF(__pyx_kp_b_y1c8_8BxP9XN_VKM);
   __pyx_v_iv = __pyx_kp_b_y1c8_8BxP9XN_VKM;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_algorithms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_algorithms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_AES); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_AES); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -4022,22 +4396,22 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_key};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_mth = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_backend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_backend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -4049,26 +4423,26 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_backend = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Cipher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Cipher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_modes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_modes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CBC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CBC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
@@ -4081,38 +4455,38 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_iv};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_mth);
   __Pyx_GIVEREF(__pyx_v_mth);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_mth)) __PYX_ERR(0, 36, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_mth)) __PYX_ERR(0, 38, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_backend, __pyx_v_backend) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_backend, __pyx_v_backend) < 0) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cipher = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher, __pyx_n_s_decryptor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_cipher, __pyx_n_s_decryptor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
@@ -4124,24 +4498,24 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_decryptor = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_base64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
@@ -4154,22 +4528,22 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_encryptedText};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __pyx_v_decoded_encryptedText = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptor, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptor, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_3)) {
@@ -4181,19 +4555,19 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_decoded_encryptedText};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptor, __pyx_n_s_finalize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptor, __pyx_n_s_finalize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
@@ -4205,40 +4579,40 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_decrypted_padded_text = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_decrypted_padded_text, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_decrypted_padded_text, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_pad_length = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  __pyx_t_3 = PyNumber_Negative(__pyx_v_pad_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Negative(__pyx_v_pad_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_v_decrypted_padded_text, 0, 0, NULL, &__pyx_t_3, NULL, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_v_decrypted_padded_text, 0, 0, NULL, &__pyx_t_3, NULL, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_decryptedText = __pyx_t_5;
   __pyx_t_5 = 0;
 
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptedText, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_decryptedText, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
@@ -4250,15 +4624,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_kp_u_utf_8};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 46, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 48, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
@@ -4285,23 +4659,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbedding(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_7Embedshroud = {"Embedshroud", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbedding = {"vectorizeEmbedding", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbedding, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbedding(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_text_chunks = 0;
@@ -4312,15 +4686,15 @@
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[2] = {0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("Embedshroud (wrapper)", 0);
+  __Pyx_RefNannySetupContext("vectorizeEmbedding (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
@@ -4340,59 +4714,59 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_chunks)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 48, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_key)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 48, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("Embedshroud", 1, 2, 2, 1); __PYX_ERR(0, 48, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vectorizeEmbedding", 1, 2, 2, 1); __PYX_ERR(0, 50, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "Embedshroud") < 0)) __PYX_ERR(0, 48, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vectorizeEmbedding") < 0)) __PYX_ERR(0, 50, __pyx_L3_error)
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
-  __Pyx_RaiseArgtupleInvalid("Embedshroud", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 48, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("vectorizeEmbedding", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 50, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbedding", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_chunks), (&PyList_Type), 1, "text_chunks", 1))) __PYX_ERR(0, 48, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_key), (&PyUnicode_Type), 1, "text_key", 1))) __PYX_ERR(0, 48, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text_chunks, __pyx_v_text_key);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_chunks), (&PyList_Type), 1, "text_chunks", 1))) __PYX_ERR(0, 50, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_key), (&PyUnicode_Type), 1, "text_key", 1))) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbedding(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text_chunks, __pyx_v_text_key);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -4401,15 +4775,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6Embedshroud(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbedding(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key) {
   PyObject *__pyx_v_embeddings = NULL;
   PyObject *__pyx_v_chunk = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_embedding = NULL;
   CYTHON_UNUSED PyObject *__pyx_v_e = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -4432,26 +4806,26 @@
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
   char const *__pyx_t_20;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("Embedshroud", 1);
+  __Pyx_RefNannySetupContext("vectorizeEmbedding", 1);
 
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_6 = NULL;
       __pyx_t_7 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_6)) {
@@ -4463,92 +4837,92 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_v_text_key};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 50, __pyx_L3_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_openai); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 50, __pyx_L3_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_openai); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 52, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (__Pyx_PyObject_SetAttrStr(__pyx_t_5, __pyx_n_s_api_key, __pyx_t_4) < 0) __PYX_ERR(0, 50, __pyx_L3_error)
+      if (__Pyx_PyObject_SetAttrStr(__pyx_t_5, __pyx_n_s_api_key, __pyx_t_4) < 0) __PYX_ERR(0, 52, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L3_error)
+      __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_v_embeddings = ((PyObject*)__pyx_t_5);
       __pyx_t_5 = 0;
 
       if (unlikely(__pyx_v_text_chunks == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-        __PYX_ERR(0, 52, __pyx_L3_error)
+        __PYX_ERR(0, 54, __pyx_L3_error)
       }
       __pyx_t_5 = __pyx_v_text_chunks; __Pyx_INCREF(__pyx_t_5);
       __pyx_t_8 = 0;
       for (;;) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 52, __pyx_L3_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 54, __pyx_L3_error)
           #endif
           if (__pyx_t_8 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_8); __Pyx_INCREF(__pyx_t_4); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 52, __pyx_L3_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_8); __Pyx_INCREF(__pyx_t_4); __pyx_t_8++; if (unlikely((0 < 0))) __PYX_ERR(0, 54, __pyx_L3_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
         __Pyx_XDECREF_SET(__pyx_v_chunk, __pyx_t_4);
         __pyx_t_4 = 0;
 
-        __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_openai); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L3_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_openai); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 55, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 53, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 55, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_create); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_create); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 55, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-        __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 56, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
-        if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 54, __pyx_L3_error)
+        if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 56, __pyx_L3_error)
 
-        __pyx_t_9 = PyList_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 55, __pyx_L3_error)
+        __pyx_t_9 = PyList_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 57, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_INCREF(__pyx_v_chunk);
         __Pyx_GIVEREF(__pyx_v_chunk);
-        if (__Pyx_PyList_SET_ITEM(__pyx_t_9, 0, __pyx_v_chunk)) __PYX_ERR(0, 55, __pyx_L3_error);
-        if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_input, __pyx_t_9) < 0) __PYX_ERR(0, 54, __pyx_L3_error)
+        if (__Pyx_PyList_SET_ITEM(__pyx_t_9, 0, __pyx_v_chunk)) __PYX_ERR(0, 57, __pyx_L3_error);
+        if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_input, __pyx_t_9) < 0) __PYX_ERR(0, 56, __pyx_L3_error)
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-        __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 53, __pyx_L3_error)
+        __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 55, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_XDECREF_SET(__pyx_v_response, __pyx_t_9);
         __pyx_t_9 = 0;
 
-        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 57, __pyx_L3_error)
+        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 59, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_9, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 57, __pyx_L3_error)
+        __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_9, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 59, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_embedding); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 57, __pyx_L3_error)
+        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_embedding); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 59, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_XDECREF_SET(__pyx_v_embedding, __pyx_t_9);
         __pyx_t_9 = 0;
 
-        __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_embeddings, __pyx_v_embedding); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 58, __pyx_L3_error)
+        __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_embeddings, __pyx_v_embedding); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 60, __pyx_L3_error)
 
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_embeddings);
       __pyx_r = __pyx_v_embeddings;
@@ -4558,37 +4932,37 @@
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     __Pyx_ErrFetch(&__pyx_t_5, &__pyx_t_9, &__pyx_t_6);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_openai); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L5_except_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_openai); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L5_except_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_AuthenticationError); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 60, __pyx_L5_except_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_AuthenticationError); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 62, __pyx_L5_except_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_7 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_5, __pyx_t_11);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_ErrRestore(__pyx_t_5, __pyx_t_9, __pyx_t_6);
     __pyx_t_5 = 0; __pyx_t_9 = 0; __pyx_t_6 = 0;
     if (__pyx_t_7) {
-      __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_9, &__pyx_t_5) < 0) __PYX_ERR(0, 60, __pyx_L5_except_error)
+      __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbedding", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_9, &__pyx_t_5) < 0) __PYX_ERR(0, 62, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_9);
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_9);
       __pyx_v_e = __pyx_t_9;
       /*try:*/ {
 
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 61, __pyx_L17_error)
+        __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 63, __pyx_L17_error)
         __Pyx_GOTREF(__pyx_t_11);
-        if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_error, __pyx_kp_u_Invalid_API_key_provided) < 0) __PYX_ERR(0, 61, __pyx_L17_error)
+        if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_error, __pyx_kp_u_Invalid_API_key_provided) < 0) __PYX_ERR(0, 63, __pyx_L17_error)
         __pyx_r = __pyx_t_11;
         __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L16_return;
       }
@@ -4636,27 +5010,27 @@
           goto __pyx_L6_except_return;
         }
       }
     }
 
     __pyx_t_12 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_12) {
-      __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_9, &__pyx_t_6) < 0) __PYX_ERR(0, 62, __pyx_L5_except_error)
+      __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbedding", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_9, &__pyx_t_6) < 0) __PYX_ERR(0, 64, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_9);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_9);
       __pyx_v_e = __pyx_t_9;
       /*try:*/ {
 
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 63, __pyx_L28_error)
+        __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 65, __pyx_L28_error)
         __Pyx_GOTREF(__pyx_t_11);
-        if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_error, __pyx_kp_u_An_unexpected_error_occurred) < 0) __PYX_ERR(0, 63, __pyx_L28_error)
+        if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_error, __pyx_kp_u_An_unexpected_error_occurred) < 0) __PYX_ERR(0, 65, __pyx_L28_error)
         __pyx_r = __pyx_t_11;
         __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L27_return;
       }
@@ -4731,38 +5105,459 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.Embedshroud", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeEmbedding", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_embeddings);
   __Pyx_XDECREF(__pyx_v_chunk);
   __Pyx_XDECREF(__pyx_v_response);
   __Pyx_XDECREF(__pyx_v_embedding);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9SaveToMongoDb(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9vectorizeText(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_9vectorizeText = {"vectorizeText", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9vectorizeText(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_text_embed = 0;
+  PyObject *__pyx_v_text_key = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[2] = {0,0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("vectorizeText (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_text_embed,&__pyx_n_s_text_key,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_embed)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 67, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_key)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 67, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("vectorizeText", 1, 2, 2, 1); __PYX_ERR(0, 67, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vectorizeText") < 0)) __PYX_ERR(0, 67, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 2)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+    }
+    __pyx_v_text_embed = ((PyObject*)values[0]);
+    __pyx_v_text_key = ((PyObject*)values[1]);
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("vectorizeText", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 67, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeText", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_embed), (&PyUnicode_Type), 1, "text_embed", 1))) __PYX_ERR(0, 67, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_key), (&PyUnicode_Type), 1, "text_key", 1))) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_8vectorizeText(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text_embed, __pyx_v_text_key);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
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
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8vectorizeText(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_embed, PyObject *__pyx_v_text_key) {
+  PyObject *__pyx_v_response = NULL;
+  PyObject *__pyx_v_embedding = NULL;
+  CYTHON_UNUSED PyObject *__pyx_v_e = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  int __pyx_t_10;
+  char const *__pyx_t_11;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  PyObject *__pyx_t_14 = NULL;
+  PyObject *__pyx_t_15 = NULL;
+  PyObject *__pyx_t_16 = NULL;
+  PyObject *__pyx_t_17 = NULL;
+  char const *__pyx_t_18;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("vectorizeText", 1);
+
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 69, __pyx_L3_error)
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
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 69, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_openai); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 69, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      if (__Pyx_PyObject_SetAttrStr(__pyx_t_5, __pyx_n_s_api_key, __pyx_t_4) < 0) __PYX_ERR(0, 69, __pyx_L3_error)
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_openai); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_embeddings); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_create); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_model, __pyx_kp_u_text_embedding_ada_002) < 0) __PYX_ERR(0, 71, __pyx_L3_error)
+
+      __pyx_t_6 = PyList_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_INCREF(__pyx_v_text_embed);
+      __Pyx_GIVEREF(__pyx_v_text_embed);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_v_text_embed)) __PYX_ERR(0, 72, __pyx_L3_error);
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_input, __pyx_t_6) < 0) __PYX_ERR(0, 71, __pyx_L3_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 70, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_v_response = __pyx_t_6;
+      __pyx_t_6 = 0;
+
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_data); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 74, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_embedding); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_v_embedding = __pyx_t_6;
+      __pyx_t_6 = 0;
+
+      __Pyx_XDECREF(__pyx_r);
+      __Pyx_INCREF(__pyx_v_embedding);
+      __pyx_r = __pyx_v_embedding;
+      goto __pyx_L7_try_return;
+
+    }
+    __pyx_L3_error:;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+    __Pyx_ErrFetch(&__pyx_t_6, &__pyx_t_4, &__pyx_t_5);
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_openai); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 76, __pyx_L5_except_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_AuthenticationError); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 76, __pyx_L5_except_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_7 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_6, __pyx_t_9);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_ErrRestore(__pyx_t_6, __pyx_t_4, __pyx_t_5);
+    __pyx_t_6 = 0; __pyx_t_4 = 0; __pyx_t_5 = 0;
+    if (__pyx_t_7) {
+      __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeText", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_6) < 0) __PYX_ERR(0, 76, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_4);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_INCREF(__pyx_t_4);
+      __pyx_v_e = __pyx_t_4;
+      /*try:*/ {
+
+        __Pyx_XDECREF(__pyx_r);
+        __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 77, __pyx_L14_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_error, __pyx_kp_u_Invalid_API_key_provided) < 0) __PYX_ERR(0, 77, __pyx_L14_error)
+        __pyx_r = __pyx_t_9;
+        __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        goto __pyx_L13_return;
+      }
+
+      /*finally:*/ {
+        __pyx_L14_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0;
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_15, &__pyx_t_16, &__pyx_t_17);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_12, &__pyx_t_13, &__pyx_t_14) < 0)) __Pyx_ErrFetch(&__pyx_t_12, &__pyx_t_13, &__pyx_t_14);
+          __Pyx_XGOTREF(__pyx_t_12);
+          __Pyx_XGOTREF(__pyx_t_13);
+          __Pyx_XGOTREF(__pyx_t_14);
+          __Pyx_XGOTREF(__pyx_t_15);
+          __Pyx_XGOTREF(__pyx_t_16);
+          __Pyx_XGOTREF(__pyx_t_17);
+          __pyx_t_7 = __pyx_lineno; __pyx_t_10 = __pyx_clineno; __pyx_t_11 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_15);
+            __Pyx_XGIVEREF(__pyx_t_16);
+            __Pyx_XGIVEREF(__pyx_t_17);
+            __Pyx_ExceptionReset(__pyx_t_15, __pyx_t_16, __pyx_t_17);
+          }
+          __Pyx_XGIVEREF(__pyx_t_12);
+          __Pyx_XGIVEREF(__pyx_t_13);
+          __Pyx_XGIVEREF(__pyx_t_14);
+          __Pyx_ErrRestore(__pyx_t_12, __pyx_t_13, __pyx_t_14);
+          __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0;
+          __pyx_lineno = __pyx_t_7; __pyx_clineno = __pyx_t_10; __pyx_filename = __pyx_t_11;
+          goto __pyx_L5_except_error;
+        }
+        __pyx_L13_return: {
+          __pyx_t_17 = __pyx_r;
+          __pyx_r = 0;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
+          __pyx_r = __pyx_t_17;
+          __pyx_t_17 = 0;
+          goto __pyx_L6_except_return;
+        }
+      }
+    }
+
+    __pyx_t_10 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_10) {
+      __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeText", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_4, &__pyx_t_5) < 0) __PYX_ERR(0, 78, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_4);
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_4);
+      __pyx_v_e = __pyx_t_4;
+      /*try:*/ {
+
+        __Pyx_XDECREF(__pyx_r);
+        __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 79, __pyx_L25_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_error, __pyx_kp_u_An_unexpected_error_occurred) < 0) __PYX_ERR(0, 79, __pyx_L25_error)
+        __pyx_r = __pyx_t_9;
+        __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        goto __pyx_L24_return;
+      }
+
+      /*finally:*/ {
+        __pyx_L25_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_17 = 0; __pyx_t_16 = 0; __pyx_t_15 = 0; __pyx_t_14 = 0; __pyx_t_13 = 0; __pyx_t_12 = 0;
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_14, &__pyx_t_13, &__pyx_t_12);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_17, &__pyx_t_16, &__pyx_t_15) < 0)) __Pyx_ErrFetch(&__pyx_t_17, &__pyx_t_16, &__pyx_t_15);
+          __Pyx_XGOTREF(__pyx_t_17);
+          __Pyx_XGOTREF(__pyx_t_16);
+          __Pyx_XGOTREF(__pyx_t_15);
+          __Pyx_XGOTREF(__pyx_t_14);
+          __Pyx_XGOTREF(__pyx_t_13);
+          __Pyx_XGOTREF(__pyx_t_12);
+          __pyx_t_10 = __pyx_lineno; __pyx_t_7 = __pyx_clineno; __pyx_t_18 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_14);
+            __Pyx_XGIVEREF(__pyx_t_13);
+            __Pyx_XGIVEREF(__pyx_t_12);
+            __Pyx_ExceptionReset(__pyx_t_14, __pyx_t_13, __pyx_t_12);
+          }
+          __Pyx_XGIVEREF(__pyx_t_17);
+          __Pyx_XGIVEREF(__pyx_t_16);
+          __Pyx_XGIVEREF(__pyx_t_15);
+          __Pyx_ErrRestore(__pyx_t_17, __pyx_t_16, __pyx_t_15);
+          __pyx_t_17 = 0; __pyx_t_16 = 0; __pyx_t_15 = 0; __pyx_t_14 = 0; __pyx_t_13 = 0; __pyx_t_12 = 0;
+          __pyx_lineno = __pyx_t_10; __pyx_clineno = __pyx_t_7; __pyx_filename = __pyx_t_18;
+          goto __pyx_L5_except_error;
+        }
+        __pyx_L24_return: {
+          __pyx_t_12 = __pyx_r;
+          __pyx_r = 0;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
+          __pyx_r = __pyx_t_12;
+          __pyx_t_12 = 0;
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
+
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorizeText", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_response);
+  __Pyx_XDECREF(__pyx_v_embedding);
+  __Pyx_XDECREF(__pyx_v_e);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_9SaveToMongoDb = {"SaveToMongoDb", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9SaveToMongoDb, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_9SaveToMongoDb(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_11SaveToMongoDb = {"SaveToMongoDb", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_collection = 0;
@@ -4810,60 +5605,60 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_collection)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_database)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 1); __PYX_ERR(0, 65, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 1); __PYX_ERR(0, 81, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_datasource)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 2); __PYX_ERR(0, 65, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 2); __PYX_ERR(0, 81, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_enkyc)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 3); __PYX_ERR(0, 65, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 3); __PYX_ERR(0, 81, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_params_dict)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 65, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 4); __PYX_ERR(0, 65, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 4); __PYX_ERR(0, 81, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "SaveToMongoDb") < 0)) __PYX_ERR(0, 65, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "SaveToMongoDb") < 0)) __PYX_ERR(0, 81, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 5)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -4874,33 +5669,33 @@
     __pyx_v_database = ((PyObject*)values[1]);
     __pyx_v_datasource = ((PyObject*)values[2]);
     __pyx_v_enkyc = ((PyObject*)values[3]);
     __pyx_v_params_dict = values[4];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 65, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 81, __pyx_L3_error)
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
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_collection), (&PyUnicode_Type), 1, "collection", 1))) __PYX_ERR(0, 65, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_database), (&PyUnicode_Type), 1, "database", 1))) __PYX_ERR(0, 65, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_datasource), (&PyUnicode_Type), 1, "datasource", 1))) __PYX_ERR(0, 65, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_enkyc), (&PyUnicode_Type), 1, "enkyc", 1))) __PYX_ERR(0, 65, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_collection, __pyx_v_database, __pyx_v_datasource, __pyx_v_enkyc, __pyx_v_params_dict);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_collection), (&PyUnicode_Type), 1, "collection", 1))) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_database), (&PyUnicode_Type), 1, "database", 1))) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_datasource), (&PyUnicode_Type), 1, "datasource", 1))) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_enkyc), (&PyUnicode_Type), 1, "enkyc", 1))) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_collection, __pyx_v_database, __pyx_v_datasource, __pyx_v_enkyc, __pyx_v_params_dict);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -4909,15 +5704,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict) {
   PyObject *__pyx_v_decrypted_url = NULL;
   PyObject *__pyx_v_payload = NULL;
   PyObject *__pyx_v_headers = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -4928,15 +5723,15 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("SaveToMongoDb", 1);
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -4948,138 +5743,138 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_decrypted_url = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_collection, __pyx_v_collection) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_collection, __pyx_v_collection) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
 
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_database, __pyx_v_database) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_database, __pyx_v_database) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
 
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_dataSource, __pyx_v_datasource) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_dataSource, __pyx_v_datasource) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
 
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_filename, __pyx_t_5) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_filename, __pyx_t_5) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filter, __pyx_t_2) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filter, __pyx_t_2) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_filename, __pyx_t_6) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_filename, __pyx_t_6) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_data, __pyx_t_3) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_data, __pyx_t_3) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_type, __pyx_kp_u_application_pdf) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_file_type, __pyx_kp_u_application_pdf) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_extracted_text, __pyx_t_6) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_extracted_text, __pyx_t_6) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_params_dict, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_text_embeddings, __pyx_t_3) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_text_embeddings, __pyx_t_3) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_set, __pyx_t_5) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_set, __pyx_t_5) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_update, __pyx_t_2) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_update, __pyx_t_2) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_upsert, Py_True) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_upsert, Py_True) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
   __pyx_v_payload = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__6) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__6) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
 
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_v_enkyc) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_v_enkyc) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
   __pyx_v_headers = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_requests); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_requests); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_post); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_decrypted_url);
   __Pyx_GIVEREF(__pyx_v_decrypted_url);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_decrypted_url)) __PYX_ERR(0, 90, __pyx_L1_error);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_decrypted_url)) __PYX_ERR(0, 106, __pyx_L1_error);
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_json, __pyx_v_payload) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_json, __pyx_v_payload) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_response = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_3, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 92, __pyx_L1_error)
+  __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_3, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_7) {
 
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_kp_u_Successfully_save_to_the_databas);
     __pyx_r = __pyx_kp_u_Successfully_save_to_the_databas;
     goto __pyx_L0;
 
   }
 
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_error, __pyx_t_5) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_error, __pyx_t_5) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
 
@@ -5100,23 +5895,1311 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_13vector_search = {"vector_search", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_connParam = 0;
+  PyObject *__pyx_v_extracted_text_length = 0;
+  PyObject *__pyx_v_vector_query = 0;
+  PyObject *__pyx_v_top_n = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[4] = {0,0,0,0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("vector_search (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_connParam,&__pyx_n_s_extracted_text_length,&__pyx_n_s_vector_query,&__pyx_n_s_top_n,0};
+    values[3] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)__pyx_int_5));
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_connParam)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_extracted_text_length)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("vector_search", 0, 3, 4, 1); __PYX_ERR(0, 114, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vector_query)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("vector_search", 0, 3, 4, 2); __PYX_ERR(0, 114, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_top_n);
+          if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vector_search") < 0)) __PYX_ERR(0, 114, __pyx_L3_error)
+      }
+    } else {
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_connParam = values[0];
+    __pyx_v_extracted_text_length = values[1];
+    __pyx_v_vector_query = values[2];
+    __pyx_v_top_n = values[3];
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("vector_search", 0, 3, 4, __pyx_nargs); __PYX_ERR(0, 114, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_connParam, __pyx_v_extracted_text_length, __pyx_v_vector_query, __pyx_v_top_n);
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
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search_lambda(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_13vector_search_lambda = {"lambda", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search_lambda, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search_lambda(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_x = 0;
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
+  __Pyx_RefNannySetupContext("lambda (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_x,0};
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
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 168, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda") < 0)) __PYX_ERR(0, 168, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_x = values[0];
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("lambda", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 168, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_lambda_funcdef_lambda(__pyx_self, __pyx_v_x);
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
+static PyObject *__pyx_lambda_funcdef_lambda(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_x) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("lambda", 1);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_x, __pyx_n_u_similarity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_extracted_text_length, PyObject *__pyx_v_vector_query, PyObject *__pyx_v_top_n) {
+  PyObject *__pyx_v_url = NULL;
+  PyObject *__pyx_v_headers = NULL;
+  PyObject *__pyx_v_pipeline = NULL;
+  PyObject *__pyx_v_query_payload = NULL;
+  PyObject *__pyx_v_response = NULL;
+  PyObject *__pyx_v_similarities = NULL;
+  PyObject *__pyx_v_response_data = NULL;
+  PyObject *__pyx_v_documents = NULL;
+  PyObject *__pyx_v_query_vec = NULL;
+  PyObject *__pyx_v_doc = NULL;
+  PyObject *__pyx_v_embeddings = NULL;
+  PyObject *__pyx_v_emb = NULL;
+  PyObject *__pyx_v_emb_vec = NULL;
+  PyObject *__pyx_v_similar_score = NULL;
+  PyObject *__pyx_v_cleaned_text = NULL;
+  PyObject *__pyx_v_top_results = NULL;
+  PyObject *__pyx_v_extracted_texts = NULL;
+  PyObject *__pyx_v_similarities_values = NULL;
+  PyObject *__pyx_v_filenames = NULL;
+  PyObject *__pyx_7genexpr__pyx_v_result = NULL;
+  PyObject *__pyx_8genexpr1__pyx_v_result = NULL;
+  PyObject *__pyx_8genexpr2__pyx_v_result = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  Py_ssize_t __pyx_t_7;
+  PyObject *(*__pyx_t_8)(PyObject *);
+  Py_ssize_t __pyx_t_9;
+  PyObject *(*__pyx_t_10)(PyObject *);
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  int __pyx_t_14;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("vector_search", 1);
+
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
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
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_v_url = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__6) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_enkyc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_t_2) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_headers = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_filename, __pyx_int_1) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_extracted_text, __pyx_int_1) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_text_embeddings, __pyx_int_1) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_project, __pyx_t_2) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error);
+  __pyx_t_1 = 0;
+  __pyx_v_pipeline = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_dataSource); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_dataSource, __pyx_t_1) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_database); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_database, __pyx_t_1) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_collection); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_collection, __pyx_t_1) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_pipeline, __pyx_v_pipeline) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_v_query_payload = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_requests); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_post); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_v_url);
+  __Pyx_GIVEREF(__pyx_v_url);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_url)) __PYX_ERR(0, 142, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_json, __pyx_v_query_payload) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_response = __pyx_t_5;
+  __pyx_t_5 = 0;
+
+  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_v_similarities = __pyx_t_5;
+  __pyx_t_5 = 0;
+
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_5, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 146, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__pyx_t_6) {
+
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_2 = NULL;
+    __pyx_t_4 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_2)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_2);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_4 = 1;
+      }
+    }
+    #endif
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
+      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 147, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
+    __pyx_v_response_data = __pyx_t_5;
+    __pyx_t_5 = 0;
+
+    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_response_data, __pyx_n_u_documents); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_v_documents = __pyx_t_5;
+    __pyx_t_5 = 0;
+
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = NULL;
+    __pyx_t_4 = 0;
+    #if CYTHON_UNPACK_METHODS
+    if (unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_3)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_3);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __pyx_t_4 = 1;
+      }
+    }
+    #endif
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_vector_query};
+      __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    }
+    __pyx_v_query_vec = __pyx_t_5;
+    __pyx_t_5 = 0;
+
+    if (likely(PyList_CheckExact(__pyx_v_documents)) || PyTuple_CheckExact(__pyx_v_documents)) {
+      __pyx_t_5 = __pyx_v_documents; __Pyx_INCREF(__pyx_t_5);
+      __pyx_t_7 = 0;
+      __pyx_t_8 = NULL;
+    } else {
+      __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_documents); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 152, __pyx_L1_error)
+    }
+    for (;;) {
+      if (likely(!__pyx_t_8)) {
+        if (likely(PyList_CheckExact(__pyx_t_5))) {
+          {
+            Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
+            #if !CYTHON_ASSUME_SAFE_MACROS
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 152, __pyx_L1_error)
+            #endif
+            if (__pyx_t_7 >= __pyx_temp) break;
+          }
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 152, __pyx_L1_error)
+          #else
+          __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        } else {
+          {
+            Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
+            #if !CYTHON_ASSUME_SAFE_MACROS
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 152, __pyx_L1_error)
+            #endif
+            if (__pyx_t_7 >= __pyx_temp) break;
+          }
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_2); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 152, __pyx_L1_error)
+          #else
+          __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        }
+      } else {
+        __pyx_t_2 = __pyx_t_8(__pyx_t_5);
+        if (unlikely(!__pyx_t_2)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(0, 152, __pyx_L1_error)
+          }
+          break;
+        }
+        __Pyx_GOTREF(__pyx_t_2);
+      }
+      __Pyx_XDECREF_SET(__pyx_v_doc, __pyx_t_2);
+      __pyx_t_2 = 0;
+
+      __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_text_embeddings, __pyx_v_doc, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 153, __pyx_L1_error)
+      if (__pyx_t_6) {
+
+        __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_text_embeddings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_XDECREF_SET(__pyx_v_embeddings, __pyx_t_2);
+        __pyx_t_2 = 0;
+
+        if (likely(PyList_CheckExact(__pyx_v_embeddings)) || PyTuple_CheckExact(__pyx_v_embeddings)) {
+          __pyx_t_2 = __pyx_v_embeddings; __Pyx_INCREF(__pyx_t_2);
+          __pyx_t_9 = 0;
+          __pyx_t_10 = NULL;
+        } else {
+          __pyx_t_9 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_embeddings); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 155, __pyx_L1_error)
+        }
+        for (;;) {
+          if (likely(!__pyx_t_10)) {
+            if (likely(PyList_CheckExact(__pyx_t_2))) {
+              {
+                Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+                #if !CYTHON_ASSUME_SAFE_MACROS
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 155, __pyx_L1_error)
+                #endif
+                if (__pyx_t_9 >= __pyx_temp) break;
+              }
+              #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+              __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_3); __pyx_t_9++; if (unlikely((0 < 0))) __PYX_ERR(0, 155, __pyx_L1_error)
+              #else
+              __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_3);
+              #endif
+            } else {
+              {
+                Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+                #if !CYTHON_ASSUME_SAFE_MACROS
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 155, __pyx_L1_error)
+                #endif
+                if (__pyx_t_9 >= __pyx_temp) break;
+              }
+              #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+              __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_9); __Pyx_INCREF(__pyx_t_3); __pyx_t_9++; if (unlikely((0 < 0))) __PYX_ERR(0, 155, __pyx_L1_error)
+              #else
+              __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
+              __Pyx_GOTREF(__pyx_t_3);
+              #endif
+            }
+          } else {
+            __pyx_t_3 = __pyx_t_10(__pyx_t_2);
+            if (unlikely(!__pyx_t_3)) {
+              PyObject* exc_type = PyErr_Occurred();
+              if (exc_type) {
+                if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+                else __PYX_ERR(0, 155, __pyx_L1_error)
+              }
+              break;
+            }
+            __Pyx_GOTREF(__pyx_t_3);
+          }
+          __Pyx_XDECREF_SET(__pyx_v_emb, __pyx_t_3);
+          __pyx_t_3 = 0;
+
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 156, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_11);
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __pyx_t_1 = NULL;
+          __pyx_t_4 = 0;
+          #if CYTHON_UNPACK_METHODS
+          if (unlikely(PyMethod_Check(__pyx_t_11))) {
+            __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_11);
+            if (likely(__pyx_t_1)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
+              __Pyx_INCREF(__pyx_t_1);
+              __Pyx_INCREF(function);
+              __Pyx_DECREF_SET(__pyx_t_11, function);
+              __pyx_t_4 = 1;
+            }
+          }
+          #endif
+          {
+            PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_emb};
+            __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+            __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+            if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_3);
+            __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+          }
+          __Pyx_XDECREF_SET(__pyx_v_emb_vec, __pyx_t_3);
+          __pyx_t_3 = 0;
+
+          __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_11);
+          __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_dot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+          __pyx_t_11 = NULL;
+          __pyx_t_4 = 0;
+          #if CYTHON_UNPACK_METHODS
+          if (unlikely(PyMethod_Check(__pyx_t_1))) {
+            __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_1);
+            if (likely(__pyx_t_11)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+              __Pyx_INCREF(__pyx_t_11);
+              __Pyx_INCREF(function);
+              __Pyx_DECREF_SET(__pyx_t_1, function);
+              __pyx_t_4 = 1;
+            }
+          }
+          #endif
+          {
+            PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_v_query_vec, __pyx_v_emb_vec};
+            __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+            __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+            if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_3);
+            __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          }
+          __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_11);
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_linalg); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_norm); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_11);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __pyx_t_12 = NULL;
+          __pyx_t_4 = 0;
+          #if CYTHON_UNPACK_METHODS
+          if (likely(PyMethod_Check(__pyx_t_11))) {
+            __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
+            if (likely(__pyx_t_12)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
+              __Pyx_INCREF(__pyx_t_12);
+              __Pyx_INCREF(function);
+              __Pyx_DECREF_SET(__pyx_t_11, function);
+              __pyx_t_4 = 1;
+            }
+          }
+          #endif
+          {
+            PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_v_query_vec};
+            __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+            __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_1);
+            __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+          }
+          __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_linalg); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_13);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_norm); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __pyx_t_13 = NULL;
+          __pyx_t_4 = 0;
+          #if CYTHON_UNPACK_METHODS
+          if (likely(PyMethod_Check(__pyx_t_12))) {
+            __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_12);
+            if (likely(__pyx_t_13)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+              __Pyx_INCREF(__pyx_t_13);
+              __Pyx_INCREF(function);
+              __Pyx_DECREF_SET(__pyx_t_12, function);
+              __pyx_t_4 = 1;
+            }
+          }
+          #endif
+          {
+            PyObject *__pyx_callargs[2] = {__pyx_t_13, __pyx_v_emb_vec};
+            __pyx_t_11 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+            __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+            if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 157, __pyx_L1_error)
+            __Pyx_GOTREF(__pyx_t_11);
+            __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          }
+          __pyx_t_12 = PyNumber_Multiply(__pyx_t_1, __pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+          __pyx_t_11 = __Pyx_PyNumber_Divide(__pyx_t_3, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 157, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_11);
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_XDECREF_SET(__pyx_v_similar_score, __pyx_t_11);
+          __pyx_t_11 = 0;
+
+          __pyx_t_11 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_extracted_text); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 158, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_11);
+          __Pyx_XDECREF_SET(__pyx_v_cleaned_text, __pyx_t_11);
+          __pyx_t_11 = 0;
+
+          __pyx_t_11 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 160, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_11);
+          __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_filename); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 160, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_filename, __pyx_t_12) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_shorten_text); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 161, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_INCREF(__pyx_v_cleaned_text);
+          __Pyx_GIVEREF(__pyx_v_cleaned_text);
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_cleaned_text)) __PYX_ERR(0, 161, __pyx_L1_error);
+          __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_max_length, __pyx_v_extracted_text_length) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+          __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 161, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_13);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_extracted_text, __pyx_t_13) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+
+          if (PyDict_SetItem(__pyx_t_11, __pyx_n_u_similarity, __pyx_v_similar_score) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+
+          __pyx_t_14 = __Pyx_PyObject_Append(__pyx_v_similarities, __pyx_t_11); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 159, __pyx_L1_error)
+          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+
+        }
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+        goto __pyx_L6;
+      }
+
+      /*else*/ {
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 165, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_t_11, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_text_embeddings_key_not_found_i, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 165, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      }
+      __pyx_L6:;
+
+    }
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 168, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_INCREF(__pyx_v_similarities);
+    __Pyx_GIVEREF(__pyx_v_similarities);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_similarities)) __PYX_ERR(0, 168, __pyx_L1_error);
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_11 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13vector_search_lambda, 0, __pyx_n_s_vector_search_locals_lambda, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_key, __pyx_t_11) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_reverse, Py_True) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 168, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF_SET(__pyx_v_similarities, __pyx_t_11);
+    __pyx_t_11 = 0;
+
+    __pyx_t_11 = __Pyx_PyObject_GetSlice(__pyx_v_similarities, 0, 0, NULL, &__pyx_v_top_n, NULL, 0, 0, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __pyx_v_top_results = __pyx_t_11;
+    __pyx_t_11 = 0;
+
+    { /* enter inner scope */
+      __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 172, __pyx_L13_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      if (likely(PyList_CheckExact(__pyx_v_top_results)) || PyTuple_CheckExact(__pyx_v_top_results)) {
+        __pyx_t_2 = __pyx_v_top_results; __Pyx_INCREF(__pyx_t_2);
+        __pyx_t_7 = 0;
+        __pyx_t_8 = NULL;
+      } else {
+        __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_top_results); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L13_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 172, __pyx_L13_error)
+      }
+      for (;;) {
+        if (likely(!__pyx_t_8)) {
+          if (likely(PyList_CheckExact(__pyx_t_2))) {
+            {
+              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+              #if !CYTHON_ASSUME_SAFE_MACROS
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 172, __pyx_L13_error)
+              #endif
+              if (__pyx_t_7 >= __pyx_temp) break;
+            }
+            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+            __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 172, __pyx_L13_error)
+            #else
+            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 172, __pyx_L13_error)
+            __Pyx_GOTREF(__pyx_t_5);
+            #endif
+          } else {
+            {
+              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+              #if !CYTHON_ASSUME_SAFE_MACROS
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 172, __pyx_L13_error)
+              #endif
+              if (__pyx_t_7 >= __pyx_temp) break;
+            }
+            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+            __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 172, __pyx_L13_error)
+            #else
+            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 172, __pyx_L13_error)
+            __Pyx_GOTREF(__pyx_t_5);
+            #endif
+          }
+        } else {
+          __pyx_t_5 = __pyx_t_8(__pyx_t_2);
+          if (unlikely(!__pyx_t_5)) {
+            PyObject* exc_type = PyErr_Occurred();
+            if (exc_type) {
+              if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+              else __PYX_ERR(0, 172, __pyx_L13_error)
+            }
+            break;
+          }
+          __Pyx_GOTREF(__pyx_t_5);
+        }
+        __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_result, __pyx_t_5);
+        __pyx_t_5 = 0;
+        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_7genexpr__pyx_v_result, __pyx_n_u_extracted_text); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 172, __pyx_L13_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_11, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 172, __pyx_L13_error)
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_XDECREF(__pyx_7genexpr__pyx_v_result); __pyx_7genexpr__pyx_v_result = 0;
+      goto __pyx_L17_exit_scope;
+      __pyx_L13_error:;
+      __Pyx_XDECREF(__pyx_7genexpr__pyx_v_result); __pyx_7genexpr__pyx_v_result = 0;
+      goto __pyx_L1_error;
+      __pyx_L17_exit_scope:;
+    } /* exit inner scope */
+    __pyx_v_extracted_texts = ((PyObject*)__pyx_t_11);
+    __pyx_t_11 = 0;
+
+    { /* enter inner scope */
+      __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 173, __pyx_L20_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      if (likely(PyList_CheckExact(__pyx_v_top_results)) || PyTuple_CheckExact(__pyx_v_top_results)) {
+        __pyx_t_2 = __pyx_v_top_results; __Pyx_INCREF(__pyx_t_2);
+        __pyx_t_7 = 0;
+        __pyx_t_8 = NULL;
+      } else {
+        __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_top_results); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L20_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 173, __pyx_L20_error)
+      }
+      for (;;) {
+        if (likely(!__pyx_t_8)) {
+          if (likely(PyList_CheckExact(__pyx_t_2))) {
+            {
+              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+              #if !CYTHON_ASSUME_SAFE_MACROS
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 173, __pyx_L20_error)
+              #endif
+              if (__pyx_t_7 >= __pyx_temp) break;
+            }
+            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+            __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 173, __pyx_L20_error)
+            #else
+            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L20_error)
+            __Pyx_GOTREF(__pyx_t_5);
+            #endif
+          } else {
+            {
+              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+              #if !CYTHON_ASSUME_SAFE_MACROS
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 173, __pyx_L20_error)
+              #endif
+              if (__pyx_t_7 >= __pyx_temp) break;
+            }
+            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+            __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 173, __pyx_L20_error)
+            #else
+            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L20_error)
+            __Pyx_GOTREF(__pyx_t_5);
+            #endif
+          }
+        } else {
+          __pyx_t_5 = __pyx_t_8(__pyx_t_2);
+          if (unlikely(!__pyx_t_5)) {
+            PyObject* exc_type = PyErr_Occurred();
+            if (exc_type) {
+              if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+              else __PYX_ERR(0, 173, __pyx_L20_error)
+            }
+            break;
+          }
+          __Pyx_GOTREF(__pyx_t_5);
+        }
+        __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_result, __pyx_t_5);
+        __pyx_t_5 = 0;
+        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr1__pyx_v_result, __pyx_n_u_similarity); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L20_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_11, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 173, __pyx_L20_error)
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_result); __pyx_8genexpr1__pyx_v_result = 0;
+      goto __pyx_L24_exit_scope;
+      __pyx_L20_error:;
+      __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_result); __pyx_8genexpr1__pyx_v_result = 0;
+      goto __pyx_L1_error;
+      __pyx_L24_exit_scope:;
+    } /* exit inner scope */
+    __pyx_v_similarities_values = ((PyObject*)__pyx_t_11);
+    __pyx_t_11 = 0;
+
+    { /* enter inner scope */
+      __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 174, __pyx_L27_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      if (likely(PyList_CheckExact(__pyx_v_top_results)) || PyTuple_CheckExact(__pyx_v_top_results)) {
+        __pyx_t_2 = __pyx_v_top_results; __Pyx_INCREF(__pyx_t_2);
+        __pyx_t_7 = 0;
+        __pyx_t_8 = NULL;
+      } else {
+        __pyx_t_7 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_top_results); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L27_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 174, __pyx_L27_error)
+      }
+      for (;;) {
+        if (likely(!__pyx_t_8)) {
+          if (likely(PyList_CheckExact(__pyx_t_2))) {
+            {
+              Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+              #if !CYTHON_ASSUME_SAFE_MACROS
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 174, __pyx_L27_error)
+              #endif
+              if (__pyx_t_7 >= __pyx_temp) break;
+            }
+            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+            __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 174, __pyx_L27_error)
+            #else
+            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L27_error)
+            __Pyx_GOTREF(__pyx_t_5);
+            #endif
+          } else {
+            {
+              Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+              #if !CYTHON_ASSUME_SAFE_MACROS
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 174, __pyx_L27_error)
+              #endif
+              if (__pyx_t_7 >= __pyx_temp) break;
+            }
+            #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+            __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_7); __Pyx_INCREF(__pyx_t_5); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 174, __pyx_L27_error)
+            #else
+            __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L27_error)
+            __Pyx_GOTREF(__pyx_t_5);
+            #endif
+          }
+        } else {
+          __pyx_t_5 = __pyx_t_8(__pyx_t_2);
+          if (unlikely(!__pyx_t_5)) {
+            PyObject* exc_type = PyErr_Occurred();
+            if (exc_type) {
+              if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+              else __PYX_ERR(0, 174, __pyx_L27_error)
+            }
+            break;
+          }
+          __Pyx_GOTREF(__pyx_t_5);
+        }
+        __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_result, __pyx_t_5);
+        __pyx_t_5 = 0;
+        __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_8genexpr2__pyx_v_result, __pyx_n_u_filename); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L27_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_11, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 174, __pyx_L27_error)
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_result); __pyx_8genexpr2__pyx_v_result = 0;
+      goto __pyx_L31_exit_scope;
+      __pyx_L27_error:;
+      __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_result); __pyx_8genexpr2__pyx_v_result = 0;
+      goto __pyx_L1_error;
+      __pyx_L31_exit_scope:;
+    } /* exit inner scope */
+    __pyx_v_filenames = ((PyObject*)__pyx_t_11);
+    __pyx_t_11 = 0;
+
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_INCREF(__pyx_v_extracted_texts);
+    __Pyx_GIVEREF(__pyx_v_extracted_texts);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_v_extracted_texts)) __PYX_ERR(0, 176, __pyx_L1_error);
+    __Pyx_INCREF(__pyx_v_similarities_values);
+    __Pyx_GIVEREF(__pyx_v_similarities_values);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_v_similarities_values)) __PYX_ERR(0, 176, __pyx_L1_error);
+    __Pyx_INCREF(__pyx_v_filenames);
+    __Pyx_GIVEREF(__pyx_v_filenames);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_v_filenames)) __PYX_ERR(0, 176, __pyx_L1_error);
+    __pyx_r = __pyx_t_11;
+    __pyx_t_11 = 0;
+    goto __pyx_L0;
+
+  }
+
+  /*else*/ {
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_t_11, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Request_failed_with_status_code, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_text); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __pyx_r = __pyx_t_11;
+    __pyx_t_11 = 0;
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
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_url);
+  __Pyx_XDECREF(__pyx_v_headers);
+  __Pyx_XDECREF(__pyx_v_pipeline);
+  __Pyx_XDECREF(__pyx_v_query_payload);
+  __Pyx_XDECREF(__pyx_v_response);
+  __Pyx_XDECREF(__pyx_v_similarities);
+  __Pyx_XDECREF(__pyx_v_response_data);
+  __Pyx_XDECREF(__pyx_v_documents);
+  __Pyx_XDECREF(__pyx_v_query_vec);
+  __Pyx_XDECREF(__pyx_v_doc);
+  __Pyx_XDECREF(__pyx_v_embeddings);
+  __Pyx_XDECREF(__pyx_v_emb);
+  __Pyx_XDECREF(__pyx_v_emb_vec);
+  __Pyx_XDECREF(__pyx_v_similar_score);
+  __Pyx_XDECREF(__pyx_v_cleaned_text);
+  __Pyx_XDECREF(__pyx_v_top_results);
+  __Pyx_XDECREF(__pyx_v_extracted_texts);
+  __Pyx_XDECREF(__pyx_v_similarities_values);
+  __Pyx_XDECREF(__pyx_v_filenames);
+  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_result);
+  __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_result);
+  __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_result);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_15shorten_text(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_15shorten_text = {"shorten_text", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_15shorten_text, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_15shorten_text(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_text = 0;
+  PyObject *__pyx_v_max_length = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[2] = {0,0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("shorten_text (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_text,&__pyx_n_s_max_length,0};
+    values[1] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)__pyx_int_1000));
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_length);
+          if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "shorten_text") < 0)) __PYX_ERR(0, 183, __pyx_L3_error)
+      }
+    } else {
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_text = values[0];
+    __pyx_v_max_length = values[1];
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("shorten_text", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 183, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.shorten_text", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_14shorten_text(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text, __pyx_v_max_length);
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
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14shorten_text(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_max_length) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("shorten_text", 1);
+
+  __pyx_t_1 = PyObject_Length(__pyx_v_text); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_v_max_length, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 184, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__pyx_t_4) {
+
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_v_text, 0, 0, NULL, &__pyx_v_max_length, NULL, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_kp_u__8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_r = __pyx_t_2;
+    __pyx_t_2 = 0;
+    goto __pyx_L0;
+
+  }
+
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_text);
+  __pyx_r = __pyx_v_text;
+  goto __pyx_L0;
+
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.shorten_text", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_17__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_11__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_17__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_17__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_17__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -5133,22 +7216,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_10__reduce_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_16__reduce_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
@@ -5266,23 +7349,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_19__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_13__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_19__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_19__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_19__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_state = 0;
@@ -5348,28 +7431,28 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_12__setstate_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_18__setstate_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v___pyx_state);
 
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
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_18__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 1);
@@ -5533,15 +7616,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_xyellw", 1);
 
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__7, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
@@ -5747,18 +7830,21 @@
   #endif
 }
 
 static PyMethodDef __pyx_methods_8aixhello_6xyello_xyellw[] = {
   {"Decipherx", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"Encapseal", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"Decenigma", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"Embedshroud", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"SaveToMongoDb", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9SaveToMongoDb, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"vectorizeEmbedding", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbedding, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"vectorizeText", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"SaveToMongoDb", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"vector_search", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13vector_search, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"shorten_text", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_15shorten_text, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_17__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_19__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
 static PyType_Slot __pyx_type_8aixhello_6xyello_xyellw_slots[] = {
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8aixhello_6xyello_xyellw},
   {Py_tp_methods, (void *)__pyx_methods_8aixhello_6xyello_xyellw},
   {Py_tp_new, (void *)__pyx_tp_new_8aixhello_6xyello_xyellw},
@@ -5877,47 +7963,54 @@
     {&__pyx_kp_u_An_unexpected_error_occurred, __pyx_k_An_unexpected_error_occurred, sizeof(__pyx_k_An_unexpected_error_occurred), 0, 1, 0, 0},
     {&__pyx_n_s_AuthenticationError, __pyx_k_AuthenticationError, sizeof(__pyx_k_AuthenticationError), 0, 0, 1, 1},
     {&__pyx_n_s_CBC, __pyx_k_CBC, sizeof(__pyx_k_CBC), 0, 0, 1, 1},
     {&__pyx_n_s_Cipher, __pyx_k_Cipher, sizeof(__pyx_k_Cipher), 0, 0, 1, 1},
     {&__pyx_kp_u_Content_Type, __pyx_k_Content_Type, sizeof(__pyx_k_Content_Type), 0, 1, 0, 0},
     {&__pyx_n_s_Decenigma, __pyx_k_Decenigma, sizeof(__pyx_k_Decenigma), 0, 0, 1, 1},
     {&__pyx_n_s_Decipherx, __pyx_k_Decipherx, sizeof(__pyx_k_Decipherx), 0, 0, 1, 1},
-    {&__pyx_n_s_Embedshroud, __pyx_k_Embedshroud, sizeof(__pyx_k_Embedshroud), 0, 0, 1, 1},
     {&__pyx_n_s_Encapseal, __pyx_k_Encapseal, sizeof(__pyx_k_Encapseal), 0, 0, 1, 1},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_kp_u_Invalid_API_key_provided, __pyx_k_Invalid_API_key_provided, sizeof(__pyx_k_Invalid_API_key_provided), 0, 1, 0, 0},
     {&__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, sizeof(__pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN), 0, 0, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
+    {&__pyx_kp_u_Request_failed_with_status_code, __pyx_k_Request_failed_with_status_code, sizeof(__pyx_k_Request_failed_with_status_code), 0, 1, 0, 0},
     {&__pyx_n_s_SaveToMongoDb, __pyx_k_SaveToMongoDb, sizeof(__pyx_k_SaveToMongoDb), 0, 0, 1, 1},
     {&__pyx_kp_u_Successfully_save_to_the_databas, __pyx_k_Successfully_save_to_the_databas, sizeof(__pyx_k_Successfully_save_to_the_databas), 0, 1, 0, 0},
-    {&__pyx_n_s__25, __pyx_k__25, sizeof(__pyx_k__25), 0, 0, 1, 1},
+    {&__pyx_kp_u_Unknown_filename, __pyx_k_Unknown_filename, sizeof(__pyx_k_Unknown_filename), 0, 1, 0, 0},
+    {&__pyx_kp_u__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 1, 0, 0},
+    {&__pyx_n_s__35, __pyx_k__35, sizeof(__pyx_k__35), 0, 0, 1, 1},
     {&__pyx_n_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
     {&__pyx_kp_u__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 1, 0, 0},
     {&__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, sizeof(__pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1), 0, 1, 0, 1},
     {&__pyx_n_s_aixhello_xyello, __pyx_k_aixhello_xyello, sizeof(__pyx_k_aixhello_xyello), 0, 0, 1, 1},
     {&__pyx_kp_s_aixhello_xyello_pyx, __pyx_k_aixhello_xyello_pyx, sizeof(__pyx_k_aixhello_xyello_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_algorithms, __pyx_k_algorithms, sizeof(__pyx_k_algorithms), 0, 0, 1, 1},
     {&__pyx_n_s_api_key, __pyx_k_api_key, sizeof(__pyx_k_api_key), 0, 0, 1, 1},
     {&__pyx_kp_u_api_key_2, __pyx_k_api_key_2, sizeof(__pyx_k_api_key_2), 0, 1, 0, 0},
     {&__pyx_n_s_api_url, __pyx_k_api_url, sizeof(__pyx_k_api_url), 0, 0, 1, 1},
+    {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
     {&__pyx_kp_u_application_json, __pyx_k_application_json, sizeof(__pyx_k_application_json), 0, 1, 0, 0},
     {&__pyx_kp_u_application_pdf, __pyx_k_application_pdf, sizeof(__pyx_k_application_pdf), 0, 1, 0, 0},
+    {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_b64decode, __pyx_k_b64decode, sizeof(__pyx_k_b64decode), 0, 0, 1, 1},
     {&__pyx_n_s_b64encode, __pyx_k_b64encode, sizeof(__pyx_k_b64encode), 0, 0, 1, 1},
     {&__pyx_n_s_backend, __pyx_k_backend, sizeof(__pyx_k_backend), 0, 0, 1, 1},
     {&__pyx_n_s_base64, __pyx_k_base64, sizeof(__pyx_k_base64), 0, 0, 1, 1},
     {&__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn, __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn, sizeof(__pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn), 0, 1, 0, 0},
+    {&__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2, __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2, sizeof(__pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2), 0, 1, 0, 0},
     {&__pyx_n_s_chr, __pyx_k_chr, sizeof(__pyx_k_chr), 0, 0, 1, 1},
     {&__pyx_n_s_chunk, __pyx_k_chunk, sizeof(__pyx_k_chunk), 0, 0, 1, 1},
     {&__pyx_n_s_cipher, __pyx_k_cipher, sizeof(__pyx_k_cipher), 0, 0, 1, 1},
+    {&__pyx_n_s_cleaned_text, __pyx_k_cleaned_text, sizeof(__pyx_k_cleaned_text), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_collection, __pyx_k_collection, sizeof(__pyx_k_collection), 0, 0, 1, 1},
     {&__pyx_n_u_collection, __pyx_k_collection, sizeof(__pyx_k_collection), 0, 1, 0, 1},
+    {&__pyx_n_s_connParam, __pyx_k_connParam, sizeof(__pyx_k_connParam), 0, 0, 1, 1},
     {&__pyx_n_s_create, __pyx_k_create, sizeof(__pyx_k_create), 0, 0, 1, 1},
     {&__pyx_n_s_cryptography_hazmat_backends, __pyx_k_cryptography_hazmat_backends, sizeof(__pyx_k_cryptography_hazmat_backends), 0, 0, 1, 1},
     {&__pyx_n_s_cryptography_hazmat_primitives_c, __pyx_k_cryptography_hazmat_primitives_c, sizeof(__pyx_k_cryptography_hazmat_primitives_c), 0, 0, 1, 1},
     {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
     {&__pyx_n_u_dataSource, __pyx_k_dataSource, sizeof(__pyx_k_dataSource), 0, 1, 0, 1},
     {&__pyx_n_s_database, __pyx_k_database, sizeof(__pyx_k_database), 0, 0, 1, 1},
     {&__pyx_n_u_database, __pyx_k_database, sizeof(__pyx_k_database), 0, 1, 0, 1},
@@ -5928,184 +8021,259 @@
     {&__pyx_n_s_decrypted_padded_text, __pyx_k_decrypted_padded_text, sizeof(__pyx_k_decrypted_padded_text), 0, 0, 1, 1},
     {&__pyx_n_s_decrypted_url, __pyx_k_decrypted_url, sizeof(__pyx_k_decrypted_url), 0, 0, 1, 1},
     {&__pyx_n_s_decryptor, __pyx_k_decryptor, sizeof(__pyx_k_decryptor), 0, 0, 1, 1},
     {&__pyx_n_s_default_backend, __pyx_k_default_backend, sizeof(__pyx_k_default_backend), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_n_s_dict_2, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
     {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
+    {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
+    {&__pyx_n_s_documents, __pyx_k_documents, sizeof(__pyx_k_documents), 0, 0, 1, 1},
+    {&__pyx_n_u_documents, __pyx_k_documents, sizeof(__pyx_k_documents), 0, 1, 0, 1},
+    {&__pyx_n_s_dot, __pyx_k_dot, sizeof(__pyx_k_dot), 0, 0, 1, 1},
     {&__pyx_n_s_e, __pyx_k_e, sizeof(__pyx_k_e), 0, 0, 1, 1},
+    {&__pyx_n_s_emb, __pyx_k_emb, sizeof(__pyx_k_emb), 0, 0, 1, 1},
+    {&__pyx_n_s_emb_vec, __pyx_k_emb_vec, sizeof(__pyx_k_emb_vec), 0, 0, 1, 1},
     {&__pyx_n_s_embedding, __pyx_k_embedding, sizeof(__pyx_k_embedding), 0, 0, 1, 1},
     {&__pyx_n_s_embeddings, __pyx_k_embeddings, sizeof(__pyx_k_embeddings), 0, 0, 1, 1},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_encoded_url, __pyx_k_encoded_url, sizeof(__pyx_k_encoded_url), 0, 0, 1, 1},
     {&__pyx_n_s_encryptedText, __pyx_k_encryptedText, sizeof(__pyx_k_encryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_encryptor, __pyx_k_encryptor, sizeof(__pyx_k_encryptor), 0, 0, 1, 1},
     {&__pyx_n_s_enkyc, __pyx_k_enkyc, sizeof(__pyx_k_enkyc), 0, 0, 1, 1},
+    {&__pyx_n_u_enkyc, __pyx_k_enkyc, sizeof(__pyx_k_enkyc), 0, 1, 0, 1},
     {&__pyx_n_u_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 1, 0, 1},
     {&__pyx_n_u_extracted_text, __pyx_k_extracted_text, sizeof(__pyx_k_extracted_text), 0, 1, 0, 1},
+    {&__pyx_n_s_extracted_text_length, __pyx_k_extracted_text_length, sizeof(__pyx_k_extracted_text_length), 0, 0, 1, 1},
+    {&__pyx_n_s_extracted_texts, __pyx_k_extracted_texts, sizeof(__pyx_k_extracted_texts), 0, 0, 1, 1},
     {&__pyx_n_u_file_data, __pyx_k_file_data, sizeof(__pyx_k_file_data), 0, 1, 0, 1},
     {&__pyx_n_u_file_type, __pyx_k_file_type, sizeof(__pyx_k_file_type), 0, 1, 0, 1},
     {&__pyx_n_u_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 1, 0, 1},
+    {&__pyx_n_s_filenames, __pyx_k_filenames, sizeof(__pyx_k_filenames), 0, 0, 1, 1},
     {&__pyx_n_u_filter, __pyx_k_filter, sizeof(__pyx_k_filter), 0, 1, 0, 1},
     {&__pyx_n_s_finalize, __pyx_k_finalize, sizeof(__pyx_k_finalize), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
     {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_n_s_headers, __pyx_k_headers, sizeof(__pyx_k_headers), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
     {&__pyx_n_s_input, __pyx_k_input, sizeof(__pyx_k_input), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_iv, __pyx_k_iv, sizeof(__pyx_k_iv), 0, 0, 1, 1},
     {&__pyx_n_s_json, __pyx_k_json, sizeof(__pyx_k_json), 0, 0, 1, 1},
     {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
+    {&__pyx_n_s_linalg, __pyx_k_linalg, sizeof(__pyx_k_linalg), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_max_length, __pyx_k_max_length, sizeof(__pyx_k_max_length), 0, 0, 1, 1},
     {&__pyx_n_u_message, __pyx_k_message, sizeof(__pyx_k_message), 0, 1, 0, 1},
     {&__pyx_n_s_model, __pyx_k_model, sizeof(__pyx_k_model), 0, 0, 1, 1},
     {&__pyx_n_s_modes, __pyx_k_modes, sizeof(__pyx_k_modes), 0, 0, 1, 1},
     {&__pyx_n_s_msg, __pyx_k_msg, sizeof(__pyx_k_msg), 0, 0, 1, 1},
     {&__pyx_n_s_mth, __pyx_k_mth, sizeof(__pyx_k_mth), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
+    {&__pyx_n_s_norm, __pyx_k_norm, sizeof(__pyx_k_norm), 0, 0, 1, 1},
+    {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
+    {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
     {&__pyx_n_s_openai, __pyx_k_openai, sizeof(__pyx_k_openai), 0, 0, 1, 1},
     {&__pyx_n_s_pad_length, __pyx_k_pad_length, sizeof(__pyx_k_pad_length), 0, 0, 1, 1},
     {&__pyx_n_s_padded_text, __pyx_k_padded_text, sizeof(__pyx_k_padded_text), 0, 0, 1, 1},
     {&__pyx_n_s_params_dict, __pyx_k_params_dict, sizeof(__pyx_k_params_dict), 0, 0, 1, 1},
     {&__pyx_n_s_payload, __pyx_k_payload, sizeof(__pyx_k_payload), 0, 0, 1, 1},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
+    {&__pyx_n_s_pipeline, __pyx_k_pipeline, sizeof(__pyx_k_pipeline), 0, 0, 1, 1},
+    {&__pyx_n_u_pipeline, __pyx_k_pipeline, sizeof(__pyx_k_pipeline), 0, 1, 0, 1},
     {&__pyx_n_s_post, __pyx_k_post, sizeof(__pyx_k_post), 0, 0, 1, 1},
+    {&__pyx_n_s_print, __pyx_k_print, sizeof(__pyx_k_print), 0, 0, 1, 1},
+    {&__pyx_kp_u_project, __pyx_k_project, sizeof(__pyx_k_project), 0, 1, 0, 0},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_xyellw, __pyx_k_pyx_unpickle_xyellw, sizeof(__pyx_k_pyx_unpickle_xyellw), 0, 0, 1, 1},
+    {&__pyx_n_s_query_payload, __pyx_k_query_payload, sizeof(__pyx_k_query_payload), 0, 0, 1, 1},
+    {&__pyx_n_s_query_vec, __pyx_k_query_vec, sizeof(__pyx_k_query_vec), 0, 0, 1, 1},
+    {&__pyx_n_s_re, __pyx_k_re, sizeof(__pyx_k_re), 0, 0, 1, 1},
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
     {&__pyx_n_s_requests, __pyx_k_requests, sizeof(__pyx_k_requests), 0, 0, 1, 1},
     {&__pyx_n_s_response, __pyx_k_response, sizeof(__pyx_k_response), 0, 0, 1, 1},
+    {&__pyx_n_s_response_data, __pyx_k_response_data, sizeof(__pyx_k_response_data), 0, 0, 1, 1},
+    {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
+    {&__pyx_n_s_reverse, __pyx_k_reverse, sizeof(__pyx_k_reverse), 0, 0, 1, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
     {&__pyx_kp_u_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 1, 0, 0},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_shorten_text, __pyx_k_shorten_text, sizeof(__pyx_k_shorten_text), 0, 0, 1, 1},
+    {&__pyx_n_s_similar_score, __pyx_k_similar_score, sizeof(__pyx_k_similar_score), 0, 0, 1, 1},
+    {&__pyx_n_s_similarities, __pyx_k_similarities, sizeof(__pyx_k_similarities), 0, 0, 1, 1},
+    {&__pyx_n_s_similarities_values, __pyx_k_similarities_values, sizeof(__pyx_k_similarities_values), 0, 0, 1, 1},
+    {&__pyx_n_u_similarity, __pyx_k_similarity, sizeof(__pyx_k_similarity), 0, 1, 0, 1},
+    {&__pyx_n_s_sorted, __pyx_k_sorted, sizeof(__pyx_k_sorted), 0, 0, 1, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
     {&__pyx_n_s_status_code, __pyx_k_status_code, sizeof(__pyx_k_status_code), 0, 0, 1, 1},
     {&__pyx_n_s_strText, __pyx_k_strText, sizeof(__pyx_k_strText), 0, 0, 1, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 0, 1, 1},
     {&__pyx_n_s_text_chunks, __pyx_k_text_chunks, sizeof(__pyx_k_text_chunks), 0, 0, 1, 1},
+    {&__pyx_n_s_text_embed, __pyx_k_text_embed, sizeof(__pyx_k_text_embed), 0, 0, 1, 1},
     {&__pyx_kp_u_text_embedding_ada_002, __pyx_k_text_embedding_ada_002, sizeof(__pyx_k_text_embedding_ada_002), 0, 1, 0, 0},
     {&__pyx_n_u_text_embeddings, __pyx_k_text_embeddings, sizeof(__pyx_k_text_embeddings), 0, 1, 0, 1},
+    {&__pyx_kp_u_text_embeddings_key_not_found_i, __pyx_k_text_embeddings_key_not_found_i, sizeof(__pyx_k_text_embeddings_key_not_found_i), 0, 1, 0, 0},
     {&__pyx_n_s_text_key, __pyx_k_text_key, sizeof(__pyx_k_text_key), 0, 0, 1, 1},
+    {&__pyx_n_s_top_n, __pyx_k_top_n, sizeof(__pyx_k_top_n), 0, 0, 1, 1},
+    {&__pyx_n_s_top_results, __pyx_k_top_results, sizeof(__pyx_k_top_results), 0, 0, 1, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
     {&__pyx_n_u_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 1, 0, 1},
     {&__pyx_n_u_upsert, __pyx_k_upsert, sizeof(__pyx_k_upsert), 0, 1, 0, 1},
+    {&__pyx_n_s_url, __pyx_k_url, sizeof(__pyx_k_url), 0, 0, 1, 1},
     {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
+    {&__pyx_n_s_vector_query, __pyx_k_vector_query, sizeof(__pyx_k_vector_query), 0, 0, 1, 1},
+    {&__pyx_n_s_vector_search, __pyx_k_vector_search, sizeof(__pyx_k_vector_search), 0, 0, 1, 1},
+    {&__pyx_n_s_vector_search_locals_lambda, __pyx_k_vector_search_locals_lambda, sizeof(__pyx_k_vector_search_locals_lambda), 0, 0, 1, 1},
+    {&__pyx_n_s_vectorizeEmbedding, __pyx_k_vectorizeEmbedding, sizeof(__pyx_k_vectorizeEmbedding), 0, 0, 1, 1},
+    {&__pyx_n_s_vectorizeText, __pyx_k_vectorizeText, sizeof(__pyx_k_vectorizeText), 0, 0, 1, 1},
+    {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw, __pyx_k_xyellw, sizeof(__pyx_k_xyellw), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decenigma, __pyx_k_xyellw_Decenigma, sizeof(__pyx_k_xyellw_Decenigma), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decipherx, __pyx_k_xyellw_Decipherx, sizeof(__pyx_k_xyellw_Decipherx), 0, 0, 1, 1},
-    {&__pyx_n_s_xyellw_Embedshroud, __pyx_k_xyellw_Embedshroud, sizeof(__pyx_k_xyellw_Embedshroud), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Encapseal, __pyx_k_xyellw_Encapseal, sizeof(__pyx_k_xyellw_Encapseal), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_SaveToMongoDb, __pyx_k_xyellw_SaveToMongoDb, sizeof(__pyx_k_xyellw_SaveToMongoDb), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___reduce_cython, __pyx_k_xyellw___reduce_cython, sizeof(__pyx_k_xyellw___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___setstate_cython, __pyx_k_xyellw___setstate_cython, sizeof(__pyx_k_xyellw___setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_shorten_text, __pyx_k_xyellw_shorten_text, sizeof(__pyx_k_xyellw_shorten_text), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_vector_search, __pyx_k_xyellw_vector_search, sizeof(__pyx_k_xyellw_vector_search), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_vectorizeEmbedding, __pyx_k_xyellw_vectorizeEmbedding, sizeof(__pyx_k_xyellw_vectorizeEmbedding), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_vectorizeText, __pyx_k_xyellw_vectorizeText, sizeof(__pyx_k_xyellw_vectorizeText), 0, 0, 1, 1},
     {&__pyx_kp_b_y1c8_8BxP9XN_VKM, __pyx_k_y1c8_8BxP9XN_VKM, sizeof(__pyx_k_y1c8_8BxP9XN_VKM), 0, 0, 0, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 168, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_u_filename, __pyx_kp_u_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_u_filename, __pyx_kp_u_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_file_data, __pyx_kp_u_); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_file_data, __pyx_kp_u_); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_extracted_text, __pyx_kp_u_); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_u_extracted_text, __pyx_kp_u_); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_text_embeddings, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_text_embeddings, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  __pyx_tuple__7 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_u_filename, __pyx_kp_u_Unknown_filename); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  __pyx_tuple__9 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 9, __pyx_L1_error)
 
-  __pyx_tuple__11 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 11, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 11, __pyx_L1_error)
 
-  __pyx_tuple__13 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 31, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 18, __pyx_L1_error)
 
-  __pyx_tuple__15 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Embedshroud, 48, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 33, __pyx_L1_error)
 
-  __pyx_tuple__17 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SaveToMongoDb, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeEmbedding, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 50, __pyx_L1_error)
 
-  __pyx_tuple__19 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_text_embed, __pyx_n_s_text_key, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeText, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 67, __pyx_L1_error)
 
-  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SaveToMongoDb, 81, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 81, __pyx_L1_error)
 
-  __pyx_tuple__23 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(27, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_extracted_text_length, __pyx_n_s_vector_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_similarities, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_query_vec, __pyx_n_s_doc, __pyx_n_s_embeddings, __pyx_n_s_emb, __pyx_n_s_emb_vec, __pyx_n_s_similar_score, __pyx_n_s_cleaned_text, __pyx_n_s_top_results, __pyx_n_s_extracted_texts, __pyx_n_s_similarities_values, __pyx_n_s_filenames, __pyx_n_s_result, __pyx_n_s_result, __pyx_n_s_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vector_search, 114, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_int_5); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+
+  __pyx_tuple__26 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_text, __pyx_n_s_max_length); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_shorten_text, 183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_int_1000); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+
+  __pyx_tuple__29 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  __pyx_tuple__31 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(1, 16, __pyx_L1_error)
+
+  __pyx_tuple__33 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_5 = PyInt_FromLong(5); if (unlikely(!__pyx_int_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_200 = PyInt_FromLong(200); if (unlikely(!__pyx_int_200)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_1000 = PyInt_FromLong(1000); if (unlikely(!__pyx_int_1000)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_222419149 = PyInt_FromLong(222419149L); if (unlikely(!__pyx_int_222419149)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_228825662 = PyInt_FromLong(228825662L); if (unlikely(!__pyx_int_228825662)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_238750788 = PyInt_FromLong(238750788L); if (unlikely(!__pyx_int_238750788)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -6152,35 +8320,35 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8aixhello_6xyello_xyellw = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8aixhello_6xyello_xyellw_spec, NULL); if (unlikely(!__pyx_ptype_8aixhello_6xyello_xyellw)) __PYX_ERR(0, 7, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8aixhello_6xyello_xyellw_spec, __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_ptype_8aixhello_6xyello_xyellw = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8aixhello_6xyello_xyellw_spec, NULL); if (unlikely(!__pyx_ptype_8aixhello_6xyello_xyellw)) __PYX_ERR(0, 9, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8aixhello_6xyello_xyellw_spec, __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   #else
   __pyx_ptype_8aixhello_6xyello_xyellw = &__pyx_type_8aixhello_6xyello_xyellw;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8aixhello_6xyello_xyellw->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8aixhello_6xyello_xyellw->tp_dictoffset && __pyx_ptype_8aixhello_6xyello_xyellw->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8aixhello_6xyello_xyellw->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_xyellw, (PyObject *) __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_xyellw, (PyObject *) __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -6489,109 +8657,139 @@
   #endif
 
   __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_base64, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_base64, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_requests, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_re, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_re, __pyx_t_2) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_requests, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_requests, __pyx_t_2) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_requests, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = PyList_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Cipher);
   __Pyx_GIVEREF(__pyx_n_s_Cipher);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Cipher)) __PYX_ERR(0, 3, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Cipher)) __PYX_ERR(0, 4, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_algorithms);
   __Pyx_GIVEREF(__pyx_n_s_algorithms);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_algorithms)) __PYX_ERR(0, 3, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_algorithms)) __PYX_ERR(0, 4, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_modes);
   __Pyx_GIVEREF(__pyx_n_s_modes);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_s_modes)) __PYX_ERR(0, 3, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_cryptography_hazmat_primitives_c, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_s_modes)) __PYX_ERR(0, 4, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_cryptography_hazmat_primitives_c, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Cipher); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Cipher); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Cipher, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Cipher, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_algorithms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_algorithms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_algorithms, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_algorithms, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_modes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_modes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_modes, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_modes, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_default_backend);
   __Pyx_GIVEREF(__pyx_n_s_default_backend);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_default_backend)) __PYX_ERR(0, 4, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_cryptography_hazmat_backends, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_default_backend)) __PYX_ERR(0, 5, __pyx_L1_error);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_cryptography_hazmat_backends, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_default_backend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_default_backend); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_default_backend, __pyx_t_3) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_default_backend, __pyx_t_3) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_openai, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_openai, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_openai, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_openai, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decipherx, __pyx_t_2) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decipherx, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Encapseal, __pyx_t_2) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Encapseal, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decenigma, __pyx_t_2) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbedding, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeEmbedding, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decenigma, __pyx_t_2) < 0) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorizeEmbedding, __pyx_t_2) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7Embedshroud, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Embedshroud, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Embedshroud, __pyx_t_2) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorizeText, __pyx_t_2) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9SaveToMongoDb, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SaveToMongoDb, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11SaveToMongoDb, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SaveToMongoDb, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_SaveToMongoDb, __pyx_t_2) < 0) __PYX_ERR(0, 65, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_SaveToMongoDb, __pyx_t_2) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13vector_search, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vector_search, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__25);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vector_search, __pyx_t_2) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
+
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_15shorten_text, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_shorten_text, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__28);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_shorten_text, __pyx_t_2) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
+
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_17__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_19__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_xyellw, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8234,503 +10432,42 @@
 #endif
         return ((double)a == (double)b);
     }
     return __Pyx_PyObject_IsTrueAndDecref(
         PyObject_RichCompare(op1, op2, Py_EQ));
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
-/* Import */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *module = 0;
-    PyObject *empty_dict = 0;
-    PyObject *empty_list = 0;
-    #if PY_MAJOR_VERSION < 3
-    PyObject *py_import;
-    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (unlikely(!py_import))
-        goto bad;
-    if (!from_list) {
-        empty_list = PyList_New(0);
-        if (unlikely(!empty_list))
-            goto bad;
-        from_list = empty_list;
-    }
-    #endif
-    empty_dict = PyDict_New();
-    if (unlikely(!empty_dict))
-        goto bad;
-    {
-        #if PY_MAJOR_VERSION >= 3
-        if (level == -1) {
-            if (strchr(__Pyx_MODULE_NAME, '.') != NULL) {
-                module = PyImport_ImportModuleLevelObject(
-                    name, __pyx_d, empty_dict, from_list, 1);
-                if (unlikely(!module)) {
-                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
-                        goto bad;
-                    PyErr_Clear();
-                }
-            }
-            level = 0;
-        }
-        #endif
-        if (!module) {
-            #if PY_MAJOR_VERSION < 3
-            PyObject *py_level = PyInt_FromLong(level);
-            if (unlikely(!py_level))
-                goto bad;
-            module = PyObject_CallFunctionObjArgs(py_import,
-                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
-            Py_DECREF(py_level);
-            #else
-            module = PyImport_ImportModuleLevelObject(
-                name, __pyx_d, empty_dict, from_list, level);
-            #endif
-        }
-    }
-bad:
-    Py_XDECREF(empty_dict);
-    Py_XDECREF(empty_list);
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(py_import);
-    #endif
-    return module;
-}
-
-/* ImportFrom */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
-    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
-    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
-        const char* module_name_str = 0;
-        PyObject* module_name = 0;
-        PyObject* module_dot = 0;
-        PyObject* full_name = 0;
-        PyErr_Clear();
-        module_name_str = PyModule_GetName(module);
-        if (unlikely(!module_name_str)) { goto modbad; }
-        module_name = PyUnicode_FromString(module_name_str);
-        if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__8);
-        if (unlikely(!module_dot)) { goto modbad; }
-        full_name = PyUnicode_Concat(module_dot, name);
-        if (unlikely(!full_name)) { goto modbad; }
-        #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
-        {
-            PyObject *modules = PyImport_GetModuleDict();
-            if (unlikely(!modules))
-                goto modbad;
-            value = PyObject_GetItem(modules, full_name);
-        }
-        #else
-        value = PyImport_GetModule(full_name);
-        #endif
-      modbad:
-        Py_XDECREF(full_name);
-        Py_XDECREF(module_dot);
-        Py_XDECREF(module_name);
-    }
+/* DictGetItem */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
+    PyObject *value;
+    value = PyDict_GetItemWithError(d, key);
     if (unlikely(!value)) {
-        PyErr_Format(PyExc_ImportError,
-        #if PY_MAJOR_VERSION < 3
-            "cannot import name %.230s", PyString_AS_STRING(name));
-        #else
-            "cannot import name %S", name);
-        #endif
-    }
-    return value;
-}
-
-/* RaiseException */
-#if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    CYTHON_UNUSED_VAR(cause);
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
+        if (!PyErr_Occurred()) {
+            if (unlikely(PyTuple_Check(key))) {
+                PyObject* args = PyTuple_Pack(1, key);
+                if (likely(args)) {
+                    PyErr_SetObject(PyExc_KeyError, args);
+                    Py_DECREF(args);
                 }
+            } else {
+                PyErr_SetObject(PyExc_KeyError, key);
             }
         }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-      #if PY_VERSION_HEX >= 0x030C00A6
-        PyException_SetTraceback(value, tb);
-      #elif CYTHON_FAST_THREAD_STATE
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#else
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#endif
-    }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
-/* GetAttr */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
-#if CYTHON_USE_TYPE_SLOTS
-#if PY_MAJOR_VERSION >= 3
-    if (likely(PyUnicode_Check(n)))
-#else
-    if (likely(PyString_Check(n)))
-#endif
-        return __Pyx_PyObject_GetAttrStr(o, n);
-#endif
-    return PyObject_GetAttr(o, n);
-}
-
-/* HasAttr */
-#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
-static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
-    PyObject *r;
-    if (unlikely(!__Pyx_PyBaseString_Check(n))) {
-        PyErr_SetString(PyExc_TypeError,
-                        "hasattr(): attribute name must be string");
-        return -1;
-    }
-    r = __Pyx_GetAttr(o, n);
-    if (!r) {
-        PyErr_Clear();
-        return 0;
-    } else {
-        Py_DECREF(r);
-        return 1;
-    }
-}
-#endif
-
-/* FixUpExtensionType */
-#if CYTHON_USE_TYPE_SPECS
-static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
-#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
-    CYTHON_UNUSED_VAR(spec);
-    CYTHON_UNUSED_VAR(type);
-#else
-    const PyType_Slot *slot = spec->slots;
-    while (slot && slot->slot && slot->slot != Py_tp_members)
-        slot++;
-    if (slot && slot->slot == Py_tp_members) {
-        int changed = 0;
-#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
-        const
-#endif
-            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
-        while (memb && memb->name) {
-            if (memb->name[0] == '_' && memb->name[1] == '_') {
-#if PY_VERSION_HEX < 0x030900b1
-                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
-                    assert(memb->type == T_PYSSIZET);
-                    assert(memb->flags == READONLY);
-                    type->tp_weaklistoffset = memb->offset;
-                    changed = 1;
-                }
-                else if (strcmp(memb->name, "__dictoffset__") == 0) {
-                    assert(memb->type == T_PYSSIZET);
-                    assert(memb->flags == READONLY);
-                    type->tp_dictoffset = memb->offset;
-                    changed = 1;
-                }
-#if CYTHON_METH_FASTCALL
-                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
-                    assert(memb->type == T_PYSSIZET);
-                    assert(memb->flags == READONLY);
-#if PY_VERSION_HEX >= 0x030800b4
-                    type->tp_vectorcall_offset = memb->offset;
-#else
-                    type->tp_print = (printfunc) memb->offset;
-#endif
-                    changed = 1;
-                }
-#endif
-#else
-                if ((0));
-#endif
-#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
-                else if (strcmp(memb->name, "__module__") == 0) {
-                    PyObject *descr;
-                    assert(memb->type == T_OBJECT);
-                    assert(memb->flags == 0 || memb->flags == READONLY);
-                    descr = PyDescr_NewMember(type, memb);
-                    if (unlikely(!descr))
-                        return -1;
-                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
-                        Py_DECREF(descr);
-                        return -1;
-                    }
-                    Py_DECREF(descr);
-                    changed = 1;
-                }
-#endif
-            }
-            memb++;
-        }
-        if (changed)
-            PyType_Modified(type);
+        return NULL;
     }
-#endif
-    return 0;
+    Py_INCREF(value);
+    return value;
 }
 #endif
 
-/* PyObjectCallNoArg */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-    PyObject *arg[2] = {NULL, NULL};
-    return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+/* PyObjectCall2Args */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args[3] = {NULL, arg1, arg2};
+    return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectGetMethod */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
     __Pyx_TypeName type_name;
@@ -8826,487 +10563,127 @@
         return 1;
     }
 #endif
     *method = attr;
     return 0;
 }
 
-/* PyObjectCallMethod0 */
-static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
-    PyObject *method = NULL, *result = NULL;
+/* PyObjectCallMethod1 */
+#if !(CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2)
+static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
+    PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
+    Py_DECREF(method);
+    return result;
+}
+#endif
+static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg) {
+#if CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2
+    PyObject *args[2] = {obj, arg};
+    (void) __Pyx_PyObject_GetMethod;
+    (void) __Pyx_PyObject_CallOneArg;
+    (void) __Pyx_PyObject_Call2Args;
+    return PyObject_VectorcallMethod(method_name, args, 2 | PY_VECTORCALL_ARGUMENTS_OFFSET, NULL);
+#else
+    PyObject *method = NULL, *result;
     int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
     if (likely(is_method)) {
-        result = __Pyx_PyObject_CallOneArg(method, obj);
+        result = __Pyx_PyObject_Call2Args(method, obj, arg);
         Py_DECREF(method);
         return result;
     }
-    if (unlikely(!method)) goto bad;
-    result = __Pyx_PyObject_CallNoArg(method);
-    Py_DECREF(method);
-bad:
-    return result;
+    if (unlikely(!method)) return NULL;
+    return __Pyx__PyObject_CallMethod1(method, arg);
+#endif
 }
 
-/* ValidateBasesTuple */
-#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
-static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
-    Py_ssize_t i, n;
-#if CYTHON_ASSUME_SAFE_MACROS
-    n = PyTuple_GET_SIZE(bases);
-#else
-    n = PyTuple_Size(bases);
-    if (n < 0) return -1;
-#endif
-    for (i = 1; i < n; i++)
-    {
-#if CYTHON_AVOID_BORROWED_REFS
-        PyObject *b0 = PySequence_GetItem(bases, i);
-        if (!b0) return -1;
-#elif CYTHON_ASSUME_SAFE_MACROS
-        PyObject *b0 = PyTuple_GET_ITEM(bases, i);
-#else
-        PyObject *b0 = PyTuple_GetItem(bases, i);
-        if (!b0) return -1;
-#endif
-        PyTypeObject *b;
-#if PY_MAJOR_VERSION < 3
-        if (PyClass_Check(b0))
-        {
-            PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
-                         PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
-#if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
-#endif
-            return -1;
-        }
-#endif
-        b = (PyTypeObject*) b0;
-        if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
-        {
-            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-            PyErr_Format(PyExc_TypeError,
-                "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
-            __Pyx_DECREF_TypeName(b_name);
-#if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
-#endif
+/* append */
+static CYTHON_INLINE int __Pyx_PyObject_Append(PyObject* L, PyObject* x) {
+    if (likely(PyList_CheckExact(L))) {
+        if (unlikely(__Pyx_PyList_Append(L, x) < 0)) return -1;
+    } else {
+        PyObject* retval = __Pyx_PyObject_CallMethod1(L, __pyx_n_s_append, x);
+        if (unlikely(!retval))
             return -1;
-        }
-        if (dictoffset == 0)
-        {
-            Py_ssize_t b_dictoffset = 0;
-#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
-            b_dictoffset = b->tp_dictoffset;
-#else
-            PyObject *py_b_dictoffset = PyObject_GetAttrString((PyObject*)b, "__dictoffset__");
-            if (!py_b_dictoffset) goto dictoffset_return;
-            b_dictoffset = PyLong_AsSsize_t(py_b_dictoffset);
-            Py_DECREF(py_b_dictoffset);
-            if (b_dictoffset == -1 && PyErr_Occurred()) goto dictoffset_return;
-#endif
-            if (b_dictoffset) {
-                {
-                    __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-                    PyErr_Format(PyExc_TypeError,
-                        "extension type '%.200s' has no __dict__ slot, "
-                        "but base type '" __Pyx_FMT_TYPENAME "' has: "
-                        "either add 'cdef dict __dict__' to the extension type "
-                        "or add '__slots__ = [...]' to the base type",
-                        type_name, b_name);
-                    __Pyx_DECREF_TypeName(b_name);
-                }
-#if !(CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY)
-              dictoffset_return:
-#endif
-#if CYTHON_AVOID_BORROWED_REFS
-                Py_DECREF(b0);
-#endif
-                return -1;
-            }
-        }
-#if CYTHON_AVOID_BORROWED_REFS
-        Py_DECREF(b0);
-#endif
+        Py_DECREF(retval);
     }
     return 0;
 }
-#endif
 
-/* PyType_Ready */
-static int __Pyx_PyType_Ready(PyTypeObject *t) {
-#if CYTHON_USE_TYPE_SPECS || !(CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API) || defined(PYSTON_MAJOR_VERSION)
-    (void)__Pyx_PyObject_CallMethod0;
+/* FixUpExtensionType */
 #if CYTHON_USE_TYPE_SPECS
-    (void)__Pyx_validate_bases_tuple;
-#endif
-    return PyType_Ready(t);
-#else
-    int r;
-    PyObject *bases = __Pyx_PyType_GetSlot(t, tp_bases, PyObject*);
-    if (bases && unlikely(__Pyx_validate_bases_tuple(t->tp_name, t->tp_dictoffset, bases) == -1))
-        return -1;
-#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
-    {
-        int gc_was_enabled;
-    #if PY_VERSION_HEX >= 0x030A00b1
-        gc_was_enabled = PyGC_Disable();
-        (void)__Pyx_PyObject_CallMethod0;
-    #else
-        PyObject *ret, *py_status;
-        PyObject *gc = NULL;
-        #if PY_VERSION_HEX >= 0x030700a1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM+0 >= 0x07030400)
-        gc = PyImport_GetModule(__pyx_kp_u_gc);
-        #endif
-        if (unlikely(!gc)) gc = PyImport_Import(__pyx_kp_u_gc);
-        if (unlikely(!gc)) return -1;
-        py_status = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_isenabled);
-        if (unlikely(!py_status)) {
-            Py_DECREF(gc);
-            return -1;
-        }
-        gc_was_enabled = __Pyx_PyObject_IsTrue(py_status);
-        Py_DECREF(py_status);
-        if (gc_was_enabled > 0) {
-            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_disable);
-            if (unlikely(!ret)) {
-                Py_DECREF(gc);
-                return -1;
-            }
-            Py_DECREF(ret);
-        } else if (unlikely(gc_was_enabled == -1)) {
-            Py_DECREF(gc);
-            return -1;
-        }
-    #endif
-        t->tp_flags |= Py_TPFLAGS_HEAPTYPE;
-#if PY_VERSION_HEX >= 0x030A0000
-        t->tp_flags |= Py_TPFLAGS_IMMUTABLETYPE;
-#endif
-#else
-        (void)__Pyx_PyObject_CallMethod0;
-#endif
-    r = PyType_Ready(t);
-#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
-        t->tp_flags &= ~Py_TPFLAGS_HEAPTYPE;
-    #if PY_VERSION_HEX >= 0x030A00b1
-        if (gc_was_enabled)
-            PyGC_Enable();
-    #else
-        if (gc_was_enabled) {
-            PyObject *tp, *v, *tb;
-            PyErr_Fetch(&tp, &v, &tb);
-            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_enable);
-            if (likely(ret || r == -1)) {
-                Py_XDECREF(ret);
-                PyErr_Restore(tp, v, tb);
-            } else {
-                Py_XDECREF(tp);
-                Py_XDECREF(v);
-                Py_XDECREF(tb);
-                r = -1;
-            }
-        }
-        Py_DECREF(gc);
-    #endif
-    }
-#endif
-    return r;
-#endif
-}
-
-/* PyObject_GenericGetAttrNoDict */
-#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
-static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
-    __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
-    PyErr_Format(PyExc_AttributeError,
-#if PY_MAJOR_VERSION >= 3
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
-                 type_name, attr_name);
-#else
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
-                 type_name, PyString_AS_STRING(attr_name));
-#endif
-    __Pyx_DECREF_TypeName(type_name);
-    return NULL;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
-    PyObject *descr;
-    PyTypeObject *tp = Py_TYPE(obj);
-    if (unlikely(!PyString_Check(attr_name))) {
-        return PyObject_GenericGetAttr(obj, attr_name);
-    }
-    assert(!tp->tp_dictoffset);
-    descr = _PyType_Lookup(tp, attr_name);
-    if (unlikely(!descr)) {
-        return __Pyx_RaiseGenericGetAttributeError(tp, attr_name);
-    }
-    Py_INCREF(descr);
-    #if PY_MAJOR_VERSION < 3
-    if (likely(PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_HAVE_CLASS)))
-    #endif
-    {
-        descrgetfunc f = Py_TYPE(descr)->tp_descr_get;
-        if (unlikely(f)) {
-            PyObject *res = f(descr, obj, (PyObject *)tp);
-            Py_DECREF(descr);
-            return res;
-        }
-    }
-    return descr;
-}
-#endif
-
-/* PyObject_GenericGetAttr */
-#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
-static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name) {
-    if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
-        return PyObject_GenericGetAttr(obj, attr_name);
-    }
-    return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
-}
-#endif
-
-/* SetupReduce */
-#if !CYTHON_COMPILING_IN_LIMITED_API
-static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
-  int ret;
-  PyObject *name_attr;
-  name_attr = __Pyx_PyObject_GetAttrStrNoError(meth, __pyx_n_s_name);
-  if (likely(name_attr)) {
-      ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
-  } else {
-      ret = -1;
-  }
-  if (unlikely(ret < 0)) {
-      PyErr_Clear();
-      ret = 0;
-  }
-  Py_XDECREF(name_attr);
-  return ret;
-}
-static int __Pyx_setup_reduce(PyObject* type_obj) {
-    int ret = 0;
-    PyObject *object_reduce = NULL;
-    PyObject *object_getstate = NULL;
-    PyObject *object_reduce_ex = NULL;
-    PyObject *reduce = NULL;
-    PyObject *reduce_ex = NULL;
-    PyObject *reduce_cython = NULL;
-    PyObject *setstate = NULL;
-    PyObject *setstate_cython = NULL;
-    PyObject *getstate = NULL;
-#if CYTHON_USE_PYTYPE_LOOKUP
-    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
-#else
-    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
-    if (!getstate && PyErr_Occurred()) {
-        goto __PYX_BAD;
-    }
-#endif
-    if (getstate) {
-#if CYTHON_USE_PYTYPE_LOOKUP
-        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
-#else
-        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
-        if (!object_getstate && PyErr_Occurred()) {
-            goto __PYX_BAD;
-        }
-#endif
-        if (object_getstate != getstate) {
-            goto __PYX_GOOD;
-        }
-    }
-#if CYTHON_USE_PYTYPE_LOOKUP
-    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
-#else
-    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
-#endif
-    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
-    if (reduce_ex == object_reduce_ex) {
-#if CYTHON_USE_PYTYPE_LOOKUP
-        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
 #else
-        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
 #endif
-        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto __PYX_BAD;
-        if (reduce == object_reduce || __Pyx_setup_reduce_is_named(reduce, __pyx_n_s_reduce_cython)) {
-            reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
-            if (likely(reduce_cython)) {
-                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-            } else if (reduce == object_reduce || PyErr_Occurred()) {
-                goto __PYX_BAD;
-            }
-            setstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate);
-            if (!setstate) PyErr_Clear();
-            if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
-                setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
-                if (likely(setstate_cython)) {
-                    ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                    ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                } else if (!setstate || PyErr_Occurred()) {
-                    goto __PYX_BAD;
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
                 }
-            }
-            PyType_Modified((PyTypeObject*)type_obj);
-        }
-    }
-    goto __PYX_GOOD;
-__PYX_BAD:
-    if (!PyErr_Occurred()) {
-        __Pyx_TypeName type_obj_name =
-            __Pyx_PyType_GetName((PyTypeObject*)type_obj);
-        PyErr_Format(PyExc_RuntimeError,
-            "Unable to initialize pickling for " __Pyx_FMT_TYPENAME, type_obj_name);
-        __Pyx_DECREF_TypeName(type_obj_name);
-    }
-    ret = -1;
-__PYX_GOOD:
-#if !CYTHON_USE_PYTYPE_LOOKUP
-    Py_XDECREF(object_reduce);
-    Py_XDECREF(object_reduce_ex);
-    Py_XDECREF(object_getstate);
-    Py_XDECREF(getstate);
-#endif
-    Py_XDECREF(reduce);
-    Py_XDECREF(reduce_ex);
-    Py_XDECREF(reduce_cython);
-    Py_XDECREF(setstate);
-    Py_XDECREF(setstate_cython);
-    return ret;
-}
-#endif
-
-/* ImportDottedModule */
-#if PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
-    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
-    if (unlikely(PyErr_Occurred())) {
-        PyErr_Clear();
-    }
-    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
-        partial_name = name;
-    } else {
-        slice = PySequence_GetSlice(parts_tuple, 0, count);
-        if (unlikely(!slice))
-            goto bad;
-        sep = PyUnicode_FromStringAndSize(".", 1);
-        if (unlikely(!sep))
-            goto bad;
-        partial_name = PyUnicode_Join(sep, slice);
-    }
-    PyErr_Format(
-#if PY_MAJOR_VERSION < 3
-        PyExc_ImportError,
-        "No module named '%s'", PyString_AS_STRING(partial_name));
-#else
-#if PY_VERSION_HEX >= 0x030600B1
-        PyExc_ModuleNotFoundError,
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
 #else
-        PyExc_ImportError,
-#endif
-        "No module named '%U'", partial_name);
+                    type->tp_print = (printfunc) memb->offset;
 #endif
-bad:
-    Py_XDECREF(sep);
-    Py_XDECREF(slice);
-    Py_XDECREF(partial_name);
-    return NULL;
-}
+                    changed = 1;
+                }
 #endif
-#if PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
-    PyObject *imported_module;
-#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
-    PyObject *modules = PyImport_GetModuleDict();
-    if (unlikely(!modules))
-        return NULL;
-    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
-    Py_XINCREF(imported_module);
 #else
-    imported_module = PyImport_GetModule(name);
-#endif
-    return imported_module;
-}
-#endif
-#if PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
-    Py_ssize_t i, nparts;
-    nparts = PyTuple_GET_SIZE(parts_tuple);
-    for (i=1; i < nparts && module; i++) {
-        PyObject *part, *submodule;
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        part = PyTuple_GET_ITEM(parts_tuple, i);
-#else
-        part = PySequence_ITEM(parts_tuple, i);
-#endif
-        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
-#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
-        Py_DECREF(part);
-#endif
-        Py_DECREF(module);
-        module = submodule;
-    }
-    if (unlikely(!module)) {
-        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
-    }
-    return module;
-}
+                if ((0));
 #endif
-static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
-#if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__6;
-    CYTHON_UNUSED_VAR(parts_tuple);
-    from_list = PyList_New(1);
-    if (unlikely(!from_list))
-        return NULL;
-    Py_INCREF(star);
-    PyList_SET_ITEM(from_list, 0, star);
-    module = __Pyx_Import(name, from_list, 0);
-    Py_DECREF(from_list);
-    return module;
-#else
-    PyObject *imported_module;
-    PyObject *module = __Pyx_Import(name, NULL, 0);
-    if (!parts_tuple || unlikely(!module))
-        return module;
-    imported_module = __Pyx__ImportDottedModule_Lookup(name);
-    if (likely(imported_module)) {
-        Py_DECREF(module);
-        return imported_module;
-    }
-    PyErr_Clear();
-    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
 #endif
-}
-static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
-    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
-    if (likely(module)) {
-        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
-        if (likely(spec)) {
-            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
-            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
-                Py_DECREF(spec);
-                spec = NULL;
             }
-            Py_XDECREF(unsafe);
-        }
-        if (likely(!spec)) {
-            PyErr_Clear();
-            return module;
+            memb++;
         }
-        Py_DECREF(spec);
-        Py_DECREF(module);
-    } else if (PyErr_Occurred()) {
-        PyErr_Clear();
+        if (changed)
+            PyType_Modified(type);
     }
 #endif
-    return __Pyx__ImportDottedModule(name, parts_tuple);
+    return 0;
 }
+#endif
 
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
     return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
@@ -10477,14 +11854,906 @@
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
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
+/* Import */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+    PyObject *module = 0;
+    PyObject *empty_dict = 0;
+    PyObject *empty_list = 0;
+    #if PY_MAJOR_VERSION < 3
+    PyObject *py_import;
+    py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
+    if (unlikely(!py_import))
+        goto bad;
+    if (!from_list) {
+        empty_list = PyList_New(0);
+        if (unlikely(!empty_list))
+            goto bad;
+        from_list = empty_list;
+    }
+    #endif
+    empty_dict = PyDict_New();
+    if (unlikely(!empty_dict))
+        goto bad;
+    {
+        #if PY_MAJOR_VERSION >= 3
+        if (level == -1) {
+            if (strchr(__Pyx_MODULE_NAME, '.') != NULL) {
+                module = PyImport_ImportModuleLevelObject(
+                    name, __pyx_d, empty_dict, from_list, 1);
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
+                        goto bad;
+                    PyErr_Clear();
+                }
+            }
+            level = 0;
+        }
+        #endif
+        if (!module) {
+            #if PY_MAJOR_VERSION < 3
+            PyObject *py_level = PyInt_FromLong(level);
+            if (unlikely(!py_level))
+                goto bad;
+            module = PyObject_CallFunctionObjArgs(py_import,
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
+            Py_DECREF(py_level);
+            #else
+            module = PyImport_ImportModuleLevelObject(
+                name, __pyx_d, empty_dict, from_list, level);
+            #endif
+        }
+    }
+bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_import);
+    #endif
+    return module;
+}
+
+/* ImportFrom */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
+    PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
+    if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
+        const char* module_name_str = 0;
+        PyObject* module_name = 0;
+        PyObject* module_dot = 0;
+        PyObject* full_name = 0;
+        PyErr_Clear();
+        module_name_str = PyModule_GetName(module);
+        if (unlikely(!module_name_str)) { goto modbad; }
+        module_name = PyUnicode_FromString(module_name_str);
+        if (unlikely(!module_name)) { goto modbad; }
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__10);
+        if (unlikely(!module_dot)) { goto modbad; }
+        full_name = PyUnicode_Concat(module_dot, name);
+        if (unlikely(!full_name)) { goto modbad; }
+        #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+        {
+            PyObject *modules = PyImport_GetModuleDict();
+            if (unlikely(!modules))
+                goto modbad;
+            value = PyObject_GetItem(modules, full_name);
+        }
+        #else
+        value = PyImport_GetModule(full_name);
+        #endif
+      modbad:
+        Py_XDECREF(full_name);
+        Py_XDECREF(module_dot);
+        Py_XDECREF(module_name);
+    }
+    if (unlikely(!value)) {
+        PyErr_Format(PyExc_ImportError,
+        #if PY_MAJOR_VERSION < 3
+            "cannot import name %.230s", PyString_AS_STRING(name));
+        #else
+            "cannot import name %S", name);
+        #endif
+    }
+    return value;
+}
+
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
+/* GetAttr */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
+#if CYTHON_USE_TYPE_SLOTS
+#if PY_MAJOR_VERSION >= 3
+    if (likely(PyUnicode_Check(n)))
+#else
+    if (likely(PyString_Check(n)))
+#endif
+        return __Pyx_PyObject_GetAttrStr(o, n);
+#endif
+    return PyObject_GetAttr(o, n);
+}
+
+/* HasAttr */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
+    PyObject *r;
+    if (unlikely(!__Pyx_PyBaseString_Check(n))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "hasattr(): attribute name must be string");
+        return -1;
+    }
+    r = __Pyx_GetAttr(o, n);
+    if (!r) {
+        PyErr_Clear();
+        return 0;
+    } else {
+        Py_DECREF(r);
+        return 1;
+    }
+}
+#endif
+
+/* PyObjectCallNoArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+    PyObject *arg[2] = {NULL, NULL};
+    return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectCallMethod0 */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
+    PyObject *method = NULL, *result = NULL;
+    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
+    if (likely(is_method)) {
+        result = __Pyx_PyObject_CallOneArg(method, obj);
+        Py_DECREF(method);
+        return result;
+    }
+    if (unlikely(!method)) goto bad;
+    result = __Pyx_PyObject_CallNoArg(method);
+    Py_DECREF(method);
+bad:
+    return result;
+}
+
+/* ValidateBasesTuple */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
+    Py_ssize_t i, n;
+#if CYTHON_ASSUME_SAFE_MACROS
+    n = PyTuple_GET_SIZE(bases);
+#else
+    n = PyTuple_Size(bases);
+    if (n < 0) return -1;
+#endif
+    for (i = 1; i < n; i++)
+    {
+#if CYTHON_AVOID_BORROWED_REFS
+        PyObject *b0 = PySequence_GetItem(bases, i);
+        if (!b0) return -1;
+#elif CYTHON_ASSUME_SAFE_MACROS
+        PyObject *b0 = PyTuple_GET_ITEM(bases, i);
+#else
+        PyObject *b0 = PyTuple_GetItem(bases, i);
+        if (!b0) return -1;
+#endif
+        PyTypeObject *b;
+#if PY_MAJOR_VERSION < 3
+        if (PyClass_Check(b0))
+        {
+            PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
+                         PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
+            return -1;
+        }
+#endif
+        b = (PyTypeObject*) b0;
+        if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
+            __Pyx_DECREF_TypeName(b_name);
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
+            return -1;
+        }
+        if (dictoffset == 0)
+        {
+            Py_ssize_t b_dictoffset = 0;
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+            b_dictoffset = b->tp_dictoffset;
+#else
+            PyObject *py_b_dictoffset = PyObject_GetAttrString((PyObject*)b, "__dictoffset__");
+            if (!py_b_dictoffset) goto dictoffset_return;
+            b_dictoffset = PyLong_AsSsize_t(py_b_dictoffset);
+            Py_DECREF(py_b_dictoffset);
+            if (b_dictoffset == -1 && PyErr_Occurred()) goto dictoffset_return;
+#endif
+            if (b_dictoffset) {
+                {
+                    __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+                    PyErr_Format(PyExc_TypeError,
+                        "extension type '%.200s' has no __dict__ slot, "
+                        "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                        "either add 'cdef dict __dict__' to the extension type "
+                        "or add '__slots__ = [...]' to the base type",
+                        type_name, b_name);
+                    __Pyx_DECREF_TypeName(b_name);
+                }
+#if !(CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY)
+              dictoffset_return:
+#endif
+#if CYTHON_AVOID_BORROWED_REFS
+                Py_DECREF(b0);
+#endif
+                return -1;
+            }
+        }
+#if CYTHON_AVOID_BORROWED_REFS
+        Py_DECREF(b0);
+#endif
+    }
+    return 0;
+}
+#endif
+
+/* PyType_Ready */
+static int __Pyx_PyType_Ready(PyTypeObject *t) {
+#if CYTHON_USE_TYPE_SPECS || !(CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API) || defined(PYSTON_MAJOR_VERSION)
+    (void)__Pyx_PyObject_CallMethod0;
+#if CYTHON_USE_TYPE_SPECS
+    (void)__Pyx_validate_bases_tuple;
+#endif
+    return PyType_Ready(t);
+#else
+    int r;
+    PyObject *bases = __Pyx_PyType_GetSlot(t, tp_bases, PyObject*);
+    if (bases && unlikely(__Pyx_validate_bases_tuple(t->tp_name, t->tp_dictoffset, bases) == -1))
+        return -1;
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+    {
+        int gc_was_enabled;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        gc_was_enabled = PyGC_Disable();
+        (void)__Pyx_PyObject_CallMethod0;
+    #else
+        PyObject *ret, *py_status;
+        PyObject *gc = NULL;
+        #if PY_VERSION_HEX >= 0x030700a1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM+0 >= 0x07030400)
+        gc = PyImport_GetModule(__pyx_kp_u_gc);
+        #endif
+        if (unlikely(!gc)) gc = PyImport_Import(__pyx_kp_u_gc);
+        if (unlikely(!gc)) return -1;
+        py_status = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_isenabled);
+        if (unlikely(!py_status)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+        gc_was_enabled = __Pyx_PyObject_IsTrue(py_status);
+        Py_DECREF(py_status);
+        if (gc_was_enabled > 0) {
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_disable);
+            if (unlikely(!ret)) {
+                Py_DECREF(gc);
+                return -1;
+            }
+            Py_DECREF(ret);
+        } else if (unlikely(gc_was_enabled == -1)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+    #endif
+        t->tp_flags |= Py_TPFLAGS_HEAPTYPE;
+#if PY_VERSION_HEX >= 0x030A0000
+        t->tp_flags |= Py_TPFLAGS_IMMUTABLETYPE;
+#endif
+#else
+        (void)__Pyx_PyObject_CallMethod0;
+#endif
+    r = PyType_Ready(t);
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+        t->tp_flags &= ~Py_TPFLAGS_HEAPTYPE;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        if (gc_was_enabled)
+            PyGC_Enable();
+    #else
+        if (gc_was_enabled) {
+            PyObject *tp, *v, *tb;
+            PyErr_Fetch(&tp, &v, &tb);
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_enable);
+            if (likely(ret || r == -1)) {
+                Py_XDECREF(ret);
+                PyErr_Restore(tp, v, tb);
+            } else {
+                Py_XDECREF(tp);
+                Py_XDECREF(v);
+                Py_XDECREF(tb);
+                r = -1;
+            }
+        }
+        Py_DECREF(gc);
+    #endif
+    }
+#endif
+    return r;
+#endif
+}
+
+/* PyObject_GenericGetAttrNoDict */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
+    __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, attr_name);
+#else
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(attr_name));
+#endif
+    __Pyx_DECREF_TypeName(type_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
+    PyObject *descr;
+    PyTypeObject *tp = Py_TYPE(obj);
+    if (unlikely(!PyString_Check(attr_name))) {
+        return PyObject_GenericGetAttr(obj, attr_name);
+    }
+    assert(!tp->tp_dictoffset);
+    descr = _PyType_Lookup(tp, attr_name);
+    if (unlikely(!descr)) {
+        return __Pyx_RaiseGenericGetAttributeError(tp, attr_name);
+    }
+    Py_INCREF(descr);
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_HAVE_CLASS)))
+    #endif
+    {
+        descrgetfunc f = Py_TYPE(descr)->tp_descr_get;
+        if (unlikely(f)) {
+            PyObject *res = f(descr, obj, (PyObject *)tp);
+            Py_DECREF(descr);
+            return res;
+        }
+    }
+    return descr;
+}
+#endif
+
+/* PyObject_GenericGetAttr */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name) {
+    if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
+        return PyObject_GenericGetAttr(obj, attr_name);
+    }
+    return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
+}
+#endif
+
+/* SetupReduce */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
+  int ret;
+  PyObject *name_attr;
+  name_attr = __Pyx_PyObject_GetAttrStrNoError(meth, __pyx_n_s_name);
+  if (likely(name_attr)) {
+      ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
+  } else {
+      ret = -1;
+  }
+  if (unlikely(ret < 0)) {
+      PyErr_Clear();
+      ret = 0;
+  }
+  Py_XDECREF(name_attr);
+  return ret;
+}
+static int __Pyx_setup_reduce(PyObject* type_obj) {
+    int ret = 0;
+    PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
+    PyObject *object_reduce_ex = NULL;
+    PyObject *reduce = NULL;
+    PyObject *reduce_ex = NULL;
+    PyObject *reduce_cython = NULL;
+    PyObject *setstate = NULL;
+    PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
+#if CYTHON_USE_PYTYPE_LOOKUP
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
+#else
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
+#endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
+#if CYTHON_USE_PYTYPE_LOOKUP
+    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
+#else
+    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
+#endif
+    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
+    if (reduce_ex == object_reduce_ex) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+#else
+        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+#endif
+        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto __PYX_BAD;
+        if (reduce == object_reduce || __Pyx_setup_reduce_is_named(reduce, __pyx_n_s_reduce_cython)) {
+            reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
+            if (likely(reduce_cython)) {
+                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+            } else if (reduce == object_reduce || PyErr_Occurred()) {
+                goto __PYX_BAD;
+            }
+            setstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate);
+            if (!setstate) PyErr_Clear();
+            if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
+                setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
+                if (likely(setstate_cython)) {
+                    ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                    ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                } else if (!setstate || PyErr_Occurred()) {
+                    goto __PYX_BAD;
+                }
+            }
+            PyType_Modified((PyTypeObject*)type_obj);
+        }
+    }
+    goto __PYX_GOOD;
+__PYX_BAD:
+    if (!PyErr_Occurred()) {
+        __Pyx_TypeName type_obj_name =
+            __Pyx_PyType_GetName((PyTypeObject*)type_obj);
+        PyErr_Format(PyExc_RuntimeError,
+            "Unable to initialize pickling for " __Pyx_FMT_TYPENAME, type_obj_name);
+        __Pyx_DECREF_TypeName(type_obj_name);
+    }
+    ret = -1;
+__PYX_GOOD:
+#if !CYTHON_USE_PYTYPE_LOOKUP
+    Py_XDECREF(object_reduce);
+    Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
+#endif
+    Py_XDECREF(reduce);
+    Py_XDECREF(reduce_ex);
+    Py_XDECREF(reduce_cython);
+    Py_XDECREF(setstate);
+    Py_XDECREF(setstate_cython);
+    return ret;
+}
+#endif
+
+/* ImportDottedModule */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__6;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
@@ -11163,15 +13432,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__25);
+        name = __Pyx_NewRef(__pyx_n_s__35);
     }
     return name;
 }
 #endif
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
```

### Comparing `aixhello-3.1/aixhello.egg-info/PKG-INFO` & `aixhello-3.2/aixhello.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.1
+Version: 3.2
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.1/setup.py` & `aixhello-3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='3.1',  # Increment the version number
+    version='3.2',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

