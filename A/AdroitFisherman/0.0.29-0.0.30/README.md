# Comparing `tmp/AdroitFisherman-0.0.29.tar.gz` & `tmp/AdroitFisherman-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdroitFisherman-0.0.29.tar", last modified: Tue May 28 13:24:41 2024, max compression
+gzip compressed data, was "AdroitFisherman-0.0.30.tar", last modified: Sun Jun  2 12:00:02 2024, max compression
```

## Comparing `AdroitFisherman-0.0.29.tar` & `AdroitFisherman-0.0.30.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.520698 AdroitFisherman-0.0.29/
-drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.410991 AdroitFisherman-0.0.29/AdroitFisherman/
-drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.480804 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/
--rw-rw-rw-   0        0        0      707 2024-05-26 11:34:28.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/Base64Util.py
--rw-rw-rw-   0        0        0     1034 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/CircularSingleLinkedList.py
--rw-rw-rw-   0        0        0     1174 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/DoubleLinkedList.py
--rw-rw-rw-   0        0        0      860 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SequentialList.py
--rw-rw-rw-   0        0        0     1000 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SingleLinkedList.py
--rw-rw-rw-   0        0        0     1039 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
--rw-rw-rw-   0        0        0       32 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.483797 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/__pycache__/
--rw-rw-rw-   0        0        0     1781 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
--rw-rw-rw-   0        0        0      202 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.29/AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0        0 2024-04-29 04:35:09.000000 AdroitFisherman-0.0.29/AdroitFisherman/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.484794 AdroitFisherman-0.0.29/AdroitFisherman/__pycache__/
--rw-rw-rw-   0        0        0      166 2024-04-29 04:35:10.000000 AdroitFisherman-0.0.29/AdroitFisherman/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.519700 AdroitFisherman-0.0.29/AdroitFisherman/includes/
--rw-rw-rw-   0        0        0      588 2024-05-26 02:00:28.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/Base64Util.c
--rw-rw-rw-   0        0        0     6747 2024-05-28 13:24:34.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/Base64Util.h
--rw-rw-rw-   0        0        0      834 2024-05-06 10:24:31.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/CircularSingleLinkedList.c
--rw-rw-rw-   0        0        0     8594 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/CircularSingleLinkedList.h
--rw-rw-rw-   0        0        0     1103 2024-05-11 09:23:06.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/DoubleLinkedList.c
--rw-rw-rw-   0        0        0     9854 2024-05-11 09:37:50.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/DoubleLinkedList.h
--rw-rw-rw-   0        0        0      720 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SeqList.c
--rw-rw-rw-   0        0        0     5179 2024-05-11 09:55:01.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SeqList.h
--rw-rw-rw-   0        0        0     1103 2024-04-29 04:03:41.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedList.c
--rw-rw-rw-   0        0        0     8383 2024-05-11 10:00:29.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedList.h
--rw-rw-rw-   0        0        0      883 2024-05-04 05:23:21.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
--rw-rw-rw-   0        0        0     9370 2024-05-11 10:00:29.000000 AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
-drwxrwxrwx   0        0        0        0 2024-05-28 13:24:41.426947 AdroitFisherman-0.0.29/AdroitFisherman.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-05-28 13:24:41.000000 AdroitFisherman-0.0.29/AdroitFisherman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1556 2024-05-28 13:24:41.000000 AdroitFisherman-0.0.29/AdroitFisherman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 13:24:41.000000 AdroitFisherman-0.0.29/AdroitFisherman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-28 13:24:41.000000 AdroitFisherman-0.0.29/AdroitFisherman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.29/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-05-28 13:24:41.520698 AdroitFisherman-0.0.29/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-05-26 11:35:48.000000 AdroitFisherman-0.0.29/README.md
--rw-rw-rw-   0        0        0       42 2024-05-28 13:24:41.521695 AdroitFisherman-0.0.29/setup.cfg
--rw-rw-rw-   0        0        0     1886 2024-05-28 13:24:34.000000 AdroitFisherman-0.0.29/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:00:02.752816 AdroitFisherman-0.0.30/
+drwxrwxrwx   0        0        0        0 2024-06-02 12:00:02.714344 AdroitFisherman-0.0.30/AdroitFisherman/
+drwxrwxrwx   0        0        0        0 2024-06-02 12:00:02.741322 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/
+-rw-rw-rw-   0        0        0      847 2024-06-02 09:32:55.000000 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/Base64Util.py
+-rw-rw-rw-   0        0        0     1034 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/CircularSingleLinkedList.py
+-rw-rw-rw-   0        0        0     1174 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/DoubleLinkedList.py
+-rw-rw-rw-   0        0        0      803 2024-06-02 11:54:38.000000 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/LinkedStack.py
+-rw-rw-rw-   0        0        0      860 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/SequentialList.py
+-rw-rw-rw-   0        0        0     1000 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/SingleLinkedList.py
+-rw-rw-rw-   0        0        0     1039 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
+-rw-rw-rw-   0        0        0       32 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:00:02.743492 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/__pycache__/
+-rw-rw-rw-   0        0        0     1781 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
+-rw-rw-rw-   0        0        0      202 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.30/AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0        0 2024-04-29 04:35:09.000000 AdroitFisherman-0.0.30/AdroitFisherman/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:00:02.744578 AdroitFisherman-0.0.30/AdroitFisherman/__pycache__/
+-rw-rw-rw-   0        0        0      166 2024-04-29 04:35:10.000000 AdroitFisherman-0.0.30/AdroitFisherman/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2024-06-02 12:00:02.751811 AdroitFisherman-0.0.30/AdroitFisherman/includes/
+-rw-rw-rw-   0        0        0      588 2024-05-26 02:00:28.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/Base64Util.c
+-rw-rw-rw-   0        0        0     6747 2024-05-28 13:24:34.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/Base64Util.h
+-rw-rw-rw-   0        0        0      834 2024-05-06 10:24:31.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/CircularSingleLinkedList.c
+-rw-rw-rw-   0        0        0     8602 2024-06-02 11:27:11.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/CircularSingleLinkedList.h
+-rw-rw-rw-   0        0        0     1103 2024-05-11 09:23:06.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/DoubleLinkedList.c
+-rw-rw-rw-   0        0        0     9862 2024-06-02 11:27:11.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/DoubleLinkedList.h
+-rw-rw-rw-   0        0        0      747 2024-06-02 11:35:33.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/LinkedStack.c
+-rw-rw-rw-   0        0        0     6276 2024-06-02 11:58:50.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/LinkedStack.h
+-rw-rw-rw-   0        0        0      720 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/SeqList.c
+-rw-rw-rw-   0        0        0     5183 2024-06-02 11:27:11.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/SeqList.h
+-rw-rw-rw-   0        0        0     1103 2024-04-29 04:03:41.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/SingleLinkedList.c
+-rw-rw-rw-   0        0        0     8391 2024-06-02 11:27:11.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/SingleLinkedList.h
+-rw-rw-rw-   0        0        0      883 2024-05-04 05:23:21.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
+-rw-rw-rw-   0        0        0     9378 2024-06-02 11:27:11.000000 AdroitFisherman-0.0.30/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
+drwxrwxrwx   0        0        0        0 2024-06-02 12:00:02.727322 AdroitFisherman-0.0.30/AdroitFisherman.egg-info/
+-rw-rw-rw-   0        0        0     1160 2024-06-02 12:00:02.000000 AdroitFisherman-0.0.30/AdroitFisherman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1714 2024-06-02 12:00:02.000000 AdroitFisherman-0.0.30/AdroitFisherman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 12:00:02.000000 AdroitFisherman-0.0.30/AdroitFisherman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-06-02 12:00:02.000000 AdroitFisherman-0.0.30/AdroitFisherman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.30/MANIFEST.in
+-rw-rw-rw-   0        0        0     1160 2024-06-02 12:00:02.752816 AdroitFisherman-0.0.30/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-06-02 11:27:11.000000 AdroitFisherman-0.0.30/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 12:00:02.753931 AdroitFisherman-0.0.30/setup.cfg
+-rw-rw-rw-   0        0        0     2003 2024-06-02 11:28:02.000000 AdroitFisherman-0.0.30/setup.py
```

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/Base64Util.py` & `AdroitFisherman-0.0.30/AdroitFisherman/Utilities/Base64Util.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,17 +7,23 @@
 
     def __del__(self):
         self.__base64utility.destroy_base64()
 
     def base64_encode(self, source, encode='utf-8'):
         return self.__base64utility.Base64Encryptor(bytes(source, encoding=encode)).decode(encode)
 
+    def clear(self):
+        self.__base64utility.destroy_base64()
+
 
 class Base64Decoder:
     def __init__(self):
         self.__base64utility = Base64Block()
 
     def __del__(self):
         self.__base64utility.destroy_base64()
 
     def base64_decode(self, source, encode='utf-8'):
         return self.__base64utility.Base64Decryptor(bytes(source, encoding=encode)).decode(encode)
+
+    def clear(self):
+        self.__base64utility.destroy_base64()
```

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/CircularSingleLinkedList.py` & `AdroitFisherman-0.0.30/AdroitFisherman/Utilities/CircularSingleLinkedList.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/DoubleLinkedList.py` & `AdroitFisherman-0.0.30/AdroitFisherman/Utilities/DoubleLinkedList.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SequentialList.py` & `AdroitFisherman-0.0.30/AdroitFisherman/Utilities/SequentialList.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SingleLinkedList.py` & `AdroitFisherman-0.0.30/AdroitFisherman/Utilities/SingleLinkedList.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py` & `AdroitFisherman-0.0.30/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc` & `AdroitFisherman-0.0.30/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/Base64Util.c` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/Base64Util.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/Base64Util.h` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/Base64Util.h`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/CircularSingleLinkedList.c` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/CircularSingleLinkedList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/CircularSingleLinkedList.h` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/CircularSingleLinkedList.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,39 +32,39 @@
         PyErr_SetString(PyExc_Exception, "list node object created failure!");
         return NULL;
     }
     else
     {
         self->elem = NULL;
         self->next = NULL;
+        Py_INCREF(self);
         return (PyObject*)self;
     }
 }
 static PyObject* List_new(PyTypeObject* type, PyObject* args, PyObject* kwds)
 {
     List* self;
     self = (List*)type->tp_alloc(type, 0);
     if (self == NULL)
     {
         PyErr_SetString(PyExc_Exception, "list object created failure!");
         return NULL;
     }
     else {
         self->instance = NULL;
+        Py_INCREF(self);
         return (PyObject*)self;
     }
 }
 static int LNode_init(LNode* self, PyObject* args, PyObject* kwds)
 {
-    Py_INCREF(self);
     return 0;
 }
 static int List_init(List* self, PyObject* args, PyObject* kwds)
 {
-    Py_INCREF(self);
     return 0;
 }
 static PyMemberDef LNode_members[] = {
     {"elem",T_OBJECT,offsetof(LNode,elem),0,""},
     {"next",T_OBJECT,offsetof(LNode,next),0,""},
     {NULL}
 };
```

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/DoubleLinkedList.c` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/DoubleLinkedList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/DoubleLinkedList.h` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/DoubleLinkedList.h`

 * *Files 0% similar despite different names*

```diff
@@ -35,39 +35,39 @@
         return NULL;
     }
     else
     {
         self->elem = NULL;
         self->next = NULL;
         self->prior = NULL;
+        Py_INCREF(self);
         return (PyObject*)self;
     }
 }
 static PyObject* List_new(PyTypeObject* type, PyObject* args, PyObject* kwds)
 {
     List* self;
     self = (List*)type->tp_alloc(type, 0);
     if (self == NULL)
     {
         PyErr_SetString(PyExc_Exception, "list object created failure!");
         return NULL;
     }
     else {
         self->instance = NULL;
+        Py_INCREF(self);
         return (PyObject*)self;
     }
 }
 static int LNode_init(LNode* self, PyObject* args, PyObject* kwds)
 {
-    Py_INCREF(self);
     return 0;
 }
 static int List_init(List* self, PyObject* args, PyObject* kwds)
 {
-    Py_INCREF(self);
     return 0;
 }
 static PyMemberDef LNode_members[] = {
     {"elem",T_OBJECT,offsetof(LNode,elem),0,""},
     {"next",T_OBJECT,offsetof(LNode,next),0,""},
     {"prior",T_OBJECT,offsetof(LNode,prior),0,""},
     {NULL}
```

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/SeqList.c` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/SeqList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/SeqList.h` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/SeqList.h`

 * *Files 0% similar despite different names*

```diff
@@ -24,20 +24,20 @@
         return NULL;
     }
     else
     {
         list->elem = NULL;
         list->length = 0;
         list->size = 0;
+        Py_INCREF(list);
         return (PyObject*)list;
     }
 }
 static int SeqList_init(SeqList* self, PyObject* args, PyObject* kwds)
 {
-    Py_INCREF(self);
     return 0;
 }
 static PyMemberDef SeqList_members[] = {
     {"elem",T_OBJECT,offsetof(SeqList,elem),0,""},
     {"length",T_INT,offsetof(SeqList,length),0,""},
     {"size",T_INT,offsetof(SeqList,size),0,""},
     {NULL}
```

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedList.c` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/SingleLinkedList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedList.h` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/SingleLinkedList.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         PyErr_SetString(PyExc_Exception, "list node object created failure!");
         return NULL;
     }
     else
     {
         self->elem = NULL;
         self->next = NULL;
+        Py_INCREF(self);
         return (PyObject*)self;
     }
 }
 static PyObject* List_new(PyTypeObject* type, PyObject* args, PyObject* kwds)
 {
     List* self;
     self = (List*)type->tp_alloc(type, 0);
@@ -46,25 +47,24 @@
     {
         PyErr_SetString(PyExc_Exception, "list object created failure!");
         return NULL;
     }
     else
     {
         self->instance = NULL;
+        Py_INCREF(self);
         return (PyObject*)self;
     }
 }
 static int LNode_init(LNode* self,PyObject*args,PyObject*kwds)
 {
-    Py_INCREF(self);
     return 0;
 }
 static int List_init(List*self,PyObject*args,PyObject*kwds)
 {
-    Py_INCREF(self);
     return 0;
 }
 static PyMemberDef LNode_members[] = {
     {"elem",T_OBJECT,offsetof(LNode,elem),0,""},
     {"next",T_OBJECT,offsetof(LNode,next),0,""},
     {NULL}
 };
```

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h` & `AdroitFisherman-0.0.30/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h`

 * *Files 0% similar despite different names*

```diff
@@ -30,39 +30,39 @@
         PyErr_SetString(PyExc_Exception, "list node object created failure!");
         return NULL;
     }
     else
     {
         self->elem = NULL;
         self->next = NULL;
+        Py_INCREF(self);
         return (PyObject*)self;
     }
 }
 static PyObject* List_new(PyTypeObject* type, PyObject* args, PyObject* kwds)
 {
     List* self;
     self = (List*)type->tp_alloc(type, 0);
     if (self == NULL)
     {
         PyErr_SetString(PyExc_Exception, "list object created failure!");
         return NULL;
     }
     else {
         self->instance = NULL;
+        Py_INCREF(self);
         return (PyObject*)self;
     }
 }
 static int LNode_init(LNode* self, PyObject* args, PyObject* kwds)
 {
-    Py_INCREF(self);
     return 0;
 }
 static int List_init(List* self, PyObject* args, PyObject* kwds)
 {
-    Py_INCREF(self);
     return 0;
 }
 static PyMemberDef LNode_members[] = {
     {"elem",T_OBJECT,offsetof(LNode,elem),0,""},
     {"next",T_OBJECT,offsetof(LNode,next),0,""},
     {NULL}
 };
```

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman.egg-info/PKG-INFO` & `AdroitFisherman-0.0.30/AdroitFisherman.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.29
+Version: 0.0.30
 Summary: This is a simple package about Data Structure packed by C/C++ language.
 Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
 License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,21 +15,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 
 # 版本更新总览
-```
-1、新增Base64编码器和解码器。
-2、修改了部分模块程序潜在的漏洞。
-```
+* 新增对栈的数据类型支持。
+* 修改了部分模块程序潜在的漏洞。
+* 添加了Base64编码器解码器的销毁算法以便对编码器或解码器进行多次使用。
 ## 项目模块清单
-```
-1、Base64Util
-2、CircularSingleLinkedList
-3、DoubleLinkedList
-4、SequentialList
-5、SingleLinkedList
-6、SingleLinkedListWithoutHeadNode
-```
+* Base64Util
+* CircularSingleLinkedList
+* DoubleLinkedList
+* SequentialList
+* SingleLinkedList
+* SingleLinkedListWithoutHeadNode
+* LinkedStack
```

### Comparing `AdroitFisherman-0.0.29/AdroitFisherman.egg-info/SOURCES.txt` & `AdroitFisherman-0.0.30/AdroitFisherman.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -6,32 +6,36 @@
 AdroitFisherman.egg-info/PKG-INFO
 AdroitFisherman.egg-info/SOURCES.txt
 AdroitFisherman.egg-info/dependency_links.txt
 AdroitFisherman.egg-info/top_level.txt
 AdroitFisherman/includes/Base64Util.c
 AdroitFisherman/includes/CircularSingleLinkedList.c
 AdroitFisherman/includes/DoubleLinkedList.c
+AdroitFisherman/includes/LinkedStack.c
 AdroitFisherman/includes/SeqList.c
 AdroitFisherman/includes/SingleLinkedList.c
 AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
 AdroitFisherman/Utilities/Base64Util.py
 AdroitFisherman/Utilities/CircularSingleLinkedList.py
 AdroitFisherman/Utilities/DoubleLinkedList.py
+AdroitFisherman/Utilities/LinkedStack.py
 AdroitFisherman/Utilities/SequentialList.py
 AdroitFisherman/Utilities/SingleLinkedList.py
 AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
 AdroitFisherman/Utilities/__init__.py
 AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
 AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
 AdroitFisherman/__pycache__/__init__.cpython-310.pyc
 AdroitFisherman/includes/Base64Util.c
 AdroitFisherman/includes/Base64Util.h
 AdroitFisherman/includes/CircularSingleLinkedList.c
 AdroitFisherman/includes/CircularSingleLinkedList.h
 AdroitFisherman/includes/DoubleLinkedList.c
 AdroitFisherman/includes/DoubleLinkedList.h
+AdroitFisherman/includes/LinkedStack.c
+AdroitFisherman/includes/LinkedStack.h
 AdroitFisherman/includes/SeqList.c
 AdroitFisherman/includes/SeqList.h
 AdroitFisherman/includes/SingleLinkedList.c
 AdroitFisherman/includes/SingleLinkedList.h
 AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
 AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
```

### Comparing `AdroitFisherman-0.0.29/PKG-INFO` & `AdroitFisherman-0.0.30/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.29
+Version: 0.0.30
 Summary: This is a simple package about Data Structure packed by C/C++ language.
 Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
 License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,21 +15,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 
 # 版本更新总览
-```
-1、新增Base64编码器和解码器。
-2、修改了部分模块程序潜在的漏洞。
-```
+* 新增对栈的数据类型支持。
+* 修改了部分模块程序潜在的漏洞。
+* 添加了Base64编码器解码器的销毁算法以便对编码器或解码器进行多次使用。
 ## 项目模块清单
-```
-1、Base64Util
-2、CircularSingleLinkedList
-3、DoubleLinkedList
-4、SequentialList
-5、SingleLinkedList
-6、SingleLinkedListWithoutHeadNode
-```
+* Base64Util
+* CircularSingleLinkedList
+* DoubleLinkedList
+* SequentialList
+* SingleLinkedList
+* SingleLinkedListWithoutHeadNode
+* LinkedStack
```

### Comparing `AdroitFisherman-0.0.29/setup.py` & `AdroitFisherman-0.0.30/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup,Extension
 SeqList=Extension("AdroitFisherman.SequentialList",sources=['AdroitFisherman/includes/SeqList.c'])
 SingleLinkedList=Extension("AdroitFisherman.SingleLinkedList",sources=['AdroitFisherman/includes/SingleLinkedList.c'])
 SingleLinkedListWithoutHeadNode=Extension("AdroitFisherman.SingleLinkedListWithoutHeadNode",sources=['AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c'])
 CircularSingleLinkedList=Extension("AdroitFisherman.CircularSingleLinkedList",sources=['AdroitFisherman/includes/CircularSingleLinkedList.c'])
 DoubleLinkedList=Extension("AdroitFisherman.DoubleLinkedList",sources=['AdroitFisherman/includes/DoubleLinkedList.c'])
 Base64=Extension("AdroitFisherman.Base64Utility",sources=['AdroitFisherman/includes/Base64Util.c'])
+LinkedStack=Extension("AdroitFisherman.LinkedStack",sources=['AdroitFisherman/includes/LinkedStack.c'])
 read_me = open('README.md', 'r',encoding='utf-8')
 setup(
     name="AdroitFisherman",
-    version="0.0.29",
+    version="0.0.30",
     author="adroit_fisherman",
     author_email="1295284735@qq.com",
     platforms="Windows",
     description="This is a simple package about Data Structure packed by C/C++ language.",
     long_description_content_type="text/markdown",
     long_description=read_me.read(),
     classifiers=[
@@ -24,10 +25,10 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.9",
         "Topic :: Utilities"
     ],
     include_package_data=True,
     packages=['AdroitFisherman.Utilities'],
-    ext_modules=[SeqList,SingleLinkedList,SingleLinkedListWithoutHeadNode,CircularSingleLinkedList,DoubleLinkedList,Base64]
+    ext_modules=[SeqList,SingleLinkedList,SingleLinkedListWithoutHeadNode,CircularSingleLinkedList,DoubleLinkedList,Base64,LinkedStack]
 )
 read_me.close()
```

