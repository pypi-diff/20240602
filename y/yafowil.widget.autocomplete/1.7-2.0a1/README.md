# Comparing `tmp/yafowil.widget.autocomplete-1.7.tar.gz` & `tmp/yafowil_widget_autocomplete-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yafowil.widget.autocomplete-1.7.tar", last modified: Mon Jul 16 13:48:36 2018, max compression
+gzip compressed data, was "yafowil_widget_autocomplete-2.0a1.tar", last modified: Sun Jun  2 10:49:19 2024, max compression
```

## Comparing `yafowil.widget.autocomplete-1.7.tar` & `yafowil_widget_autocomplete-2.0a1.tar`

### file list

```diff
@@ -1,40 +1,31 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/MANIFEST.in
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil.widget.autocomplete.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1523 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil.widget.autocomplete.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      140 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil.widget.autocomplete.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2018-02-02 08:08:30.000000 yafowil.widget.autocomplete-1.7/src/yafowil.widget.autocomplete.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil.widget.autocomplete.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       48 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil.widget.autocomplete.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil.widget.autocomplete.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5730 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil.widget.autocomplete.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil.widget.autocomplete.egg-info/top_level.txt
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2114 2018-07-16 12:38:28.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4397 2018-07-16 12:38:28.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/tests.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4059 2018-07-16 12:38:28.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/example.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2476 2018-07-16 12:38:28.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/widget.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      321 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/jquery.ui.autocomplete.bootstrap.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2418 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/jquery.ui.menu.bootstrap.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)       68 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/widget.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2418 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/jquery.ui.menu.plone5.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3374 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/widget.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      321 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/jquery.ui.autocomplete.plone5.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    16565 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/jquery.ui.menu.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      322 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/jquery.ui.autocomplete.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1454 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/jquery.ui.menu.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7728 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/jquery.ui.autocomplete.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9408 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/jquery.ui.menu.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    15983 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/resources/jquery.ui.autocomplete.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2018-02-02 08:08:21.000000 yafowil.widget.autocomplete-1.7/src/yafowil/widget/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      793 2018-07-16 12:38:28.000000 yafowil.widget.autocomplete-1.7/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1537 2018-07-16 12:38:28.000000 yafowil.widget.autocomplete-1.7/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5730 2018-07-16 13:48:36.000000 yafowil.widget.autocomplete-1.7/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1797 2018-07-16 13:47:57.000000 yafowil.widget.autocomplete-1.7/setup.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1361 2018-07-16 13:47:52.000000 yafowil.widget.autocomplete-1.7/HISTORY.rst
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-06-02 10:49:19.952416 yafowil_widget_autocomplete-2.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1614 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4626 2024-06-02 10:49:19.952416 yafowil_widget_autocomplete-2.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      653 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2024-06-02 10:49:19.952416 yafowil_widget_autocomplete-2.0a1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1804 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-06-02 10:49:19.948415 yafowil_widget_autocomplete-2.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-06-02 10:49:19.948415 yafowil_widget_autocomplete-2.0a1/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-06-02 10:49:19.948415 yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-06-02 10:49:19.948415 yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1644 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4055 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/example.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-06-02 10:49:19.952416 yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/resources/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      625 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/resources/widget.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    13530 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/resources/widget.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5967 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/resources/widget.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5637 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2432 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/widget.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-06-02 10:49:19.952416 yafowil_widget_autocomplete-2.0a1/src/yafowil.widget.autocomplete.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4626 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil.widget.autocomplete.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      891 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil.widget.autocomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil.widget.autocomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      123 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil.widget.autocomplete.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil.widget.autocomplete.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil.widget.autocomplete.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil.widget.autocomplete.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2024-06-02 10:49:19.000000 yafowil_widget_autocomplete-2.0a1/src/yafowil.widget.autocomplete.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yafowil.widget.autocomplete-1.7/src/yafowil.widget.autocomplete.egg-info/SOURCES.txt` & `yafowil_widget_autocomplete-2.0a1/src/yafowil.widget.autocomplete.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-HISTORY.rst
+CHANGES.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
 setup.py
 src/yafowil/__init__.py
 src/yafowil.widget.autocomplete.egg-info/PKG-INFO
 src/yafowil.widget.autocomplete.egg-info/SOURCES.txt
@@ -13,19 +13,10 @@
 src/yafowil.widget.autocomplete.egg-info/requires.txt
 src/yafowil.widget.autocomplete.egg-info/top_level.txt
 src/yafowil/widget/__init__.py
 src/yafowil/widget/autocomplete/__init__.py
 src/yafowil/widget/autocomplete/example.py
 src/yafowil/widget/autocomplete/tests.py
 src/yafowil/widget/autocomplete/widget.py
-src/yafowil/widget/autocomplete/resources/jquery.ui.autocomplete.bootstrap.css
-src/yafowil/widget/autocomplete/resources/jquery.ui.autocomplete.css
-src/yafowil/widget/autocomplete/resources/jquery.ui.autocomplete.js
-src/yafowil/widget/autocomplete/resources/jquery.ui.autocomplete.min.js
-src/yafowil/widget/autocomplete/resources/jquery.ui.autocomplete.plone5.css
-src/yafowil/widget/autocomplete/resources/jquery.ui.menu.bootstrap.css
-src/yafowil/widget/autocomplete/resources/jquery.ui.menu.css
-src/yafowil/widget/autocomplete/resources/jquery.ui.menu.js
-src/yafowil/widget/autocomplete/resources/jquery.ui.menu.min.js
-src/yafowil/widget/autocomplete/resources/jquery.ui.menu.plone5.css
 src/yafowil/widget/autocomplete/resources/widget.css
-src/yafowil/widget/autocomplete/resources/widget.js
+src/yafowil/widget/autocomplete/resources/widget.js
+src/yafowil/widget/autocomplete/resources/widget.min.js
```

### Comparing `yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/tests.py` & `yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/tests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from node.utils import UNSET
 from yafowil.base import ExtractionError
 from yafowil.base import factory
 from yafowil.compat import IS_PY2
-from yafowil.tests import YafowilTestCase
 from yafowil.tests import fxml
-import yafowil.loader
+from yafowil.tests import YafowilTestCase
+import os
+import unittest
 
 
 if not IS_PY2:
     from importlib import reload
 
 
+def np(path):
+    return path.replace('/', os.path.sep)
+
+
 class TestAutocompleteWidget(YafowilTestCase):
 
     def setUp(self):
         super(TestAutocompleteWidget, self).setUp()
+        from yafowil.widget import autocomplete
         from yafowil.widget.autocomplete import widget
         reload(widget)
+        autocomplete.register()
 
     def test_source_is_string(self):
         # Render plain, source is string
         widget = factory(
             'autocomplete',
             name='root',
             props={
                 'source': 'http://www.foo.bar/baz'
             })
-        self.check_output("""
+        self.checkOutput("""
         <div class="yafowil-widget-autocomplete">
           <input class="autocomplete" id="input-root" name="root" type="text"/>
           <div class="autocomplete-source hiddenStructure">http://www.foo.bar/baz</div>
           <div class="autocomplete-params hiddenStructure">delay,300|minLength,1|type,remote</div>
         </div>
         """, fxml(widget()))
 
@@ -38,15 +45,15 @@
         # Render plain, source is list
         widget = factory(
             'autocomplete',
             name='root',
             props={
                 'source': ['foo', 'bar']
             })
-        self.check_output("""
+        self.checkOutput("""
         <div class="yafowil-widget-autocomplete">
           <input class="autocomplete" id="input-root" name="root" type="text"/>
           <div class="autocomplete-source hiddenStructure">foo|bar</div>
           <div class="autocomplete-params hiddenStructure">delay,300|minLength,1|type,local</div>
         </div>
         """, fxml(widget()))
 
@@ -57,15 +64,15 @@
 
         widget = factory(
             'autocomplete',
             name='root',
             props={
                 'source': test_source
             })
-        self.check_output("""
+        self.checkOutput("""
         <div class="yafowil-widget-autocomplete">
           <input class="autocomplete" id="input-root" name="root" type="text"/>
           <div class="autocomplete-source hiddenStructure">http://from.callable/</div>
           <div class="autocomplete-params hiddenStructure">delay,300|minLength,1|type,remote</div>
         </div>""", fxml(widget()))
 
     def test_extraction(self):
@@ -94,15 +101,15 @@
         data = widget.extract({'root': ''})
         error = ExtractionError('Autocomplete widget is required')
         self.assertEqual(
             [data.name, data.value, data.extracted, data.errors],
             ['root', UNSET, '', [error]]
         )
 
-        self.check_output("""
+        self.checkOutput("""
         <div class="error">
           <div class="errormessage">Autocomplete widget is required</div>
           <div class="yafowil-widget-autocomplete">
             <input class="autocomplete required" id="input-root" name="root"
                    required="required" type="text" value=""/>
             <div class="autocomplete-source hiddenStructure">http://from.callable/</div>
             <div class="autocomplete-params hiddenStructure">delay,300|minLength,1|type,remote</div>
@@ -113,16 +120,46 @@
     def test_invalid_source_type(self):
         widget = factory(
             'autocomplete',
             name='root',
             props={
                 'source': None
             })
-        err = self.expect_error(
-            ValueError,
-            widget
+        with self.assertRaises(ValueError) as arc:
+            widget()
+        self.assertEqual(
+            str(arc.exception),
+            'resulting source must be tuple/list or string'
+        )
+
+    def test_resources(self):
+        factory.theme = 'default'
+        resources = factory.get_resources('yafowil.widget.autocomplete')
+        self.assertTrue(
+            resources.directory.endswith(np('/autocomplete/resources'))
+        )
+        self.assertEqual(resources.name, 'yafowil.widget.autocomplete')
+        self.assertEqual(resources.path, 'yafowil-autocomplete')
+
+        scripts = resources.scripts
+        self.assertEqual(len(scripts), 1)
+
+        self.assertTrue(
+            scripts[0].directory.endswith(np('/autocomplete/resources'))
+        )
+        self.assertEqual(scripts[0].path, 'yafowil-autocomplete')
+        self.assertEqual(scripts[0].file_name, 'widget.min.js')
+        self.assertTrue(os.path.exists(scripts[0].file_path))
+
+        styles = resources.styles
+        self.assertEqual(len(styles), 1)
+
+        self.assertTrue(
+            styles[0].directory.endswith(np('/autocomplete/resources'))
         )
-        self.assertEqual(str(err), 'resulting source must be tuple/list or string')
+        self.assertEqual(styles[0].path, 'yafowil-autocomplete')
+        self.assertEqual(styles[0].file_name, 'widget.css')
+        self.assertTrue(os.path.exists(styles[0].file_path))
 
 
 if __name__ == '__main__':
-    unittest.main()                                          # pragma: no cover
+    unittest.main()
```

### Comparing `yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/example.py` & `yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from yafowil.base import factory
 from yafowil.compat import IS_PY2
 import json
-import os
+
 
 if IS_PY2:
     from urlparse import urlparse
     from urlparse import parse_qs
 else:
     from urllib.parse import urlparse
     from urllib.parse import parse_qs
@@ -20,16 +20,17 @@
 lipsum = sorted(set(lipsum.lower().replace('.', '').replace(',', '').split()))
 
 
 def json_response(url):
     purl = urlparse(url)
     qs = parse_qs(purl.query)
     data = json_data(qs.get('term', [''])[0])
-    return {'body': json.dumps(data),
-            'header': [('Content-Type', 'application/json')]
+    return {
+        'body': json.dumps(data),
+        'header': [('Content-Type', 'application/json')]
     }
 
 
 def json_data(term):
     data = lipsum
     if term:
         data = [_ for _ in data if _.startswith(term)]
```

### Comparing `yafowil.widget.autocomplete-1.7/src/yafowil/widget/autocomplete/widget.py` & `yafowil_widget_autocomplete-2.0a1/src/yafowil/widget/autocomplete/widget.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from yafowil.base import ExtractionError
 from yafowil.base import factory
 from yafowil.common import generic_extractor
 from yafowil.common import generic_required_extractor
 from yafowil.common import input_generic_renderer
 from yafowil.compat import STR_TYPE
 from yafowil.utils import attr_value
 from yafowil.utils import managedprops
@@ -13,61 +12,71 @@
     result = data.rendered
     tag = data.tag
     source = attr_value('source', widget, data)
     if isinstance(source, (list, tuple)):
         source = '|'.join(source)
         source_type = 'local'
     elif isinstance(source, STR_TYPE):
-        source_type = 'remote'  
+        source_type = 'remote'
     else:
         raise ValueError('resulting source must be tuple/list or string')
-    result += tag('div', source, 
-                  **{'class': 'autocomplete-source hiddenStructure'})
-    params = [('%s,%s' % (_, attr_value(_, widget, data))) \
-                  for _ in ['delay', 'minLength']]
+    result += tag('div', source, **{
+        'class': 'autocomplete-source hiddenStructure'
+    })
+    params = [
+        ('%s,%s' % (_, attr_value(_, widget, data)))
+        for _ in ['delay', 'minLength']
+    ]
     params.append('type,%s' % source_type)
-    result += tag('div', '|'.join(params), 
-                  **{'class': 'autocomplete-params hiddenStructure'})
+    result += tag('div', '|'.join(params), **{
+        'class': 'autocomplete-params hiddenStructure'
+    })
     return tag('div', result, **{'class': 'yafowil-widget-autocomplete'})
 
 
-def autocomplete_extractor(widget, data):    
+def autocomplete_extractor(widget, data):
     return data.extracted
 
 
 factory.register(
-    'autocomplete', 
-    extractors=[generic_extractor,
-                generic_required_extractor,
-                autocomplete_extractor], 
-    edit_renderers=[input_generic_renderer, autocomplete_renderer])
-
-factory.doc['blueprint']['autocomplete'] = \
-"""Add-on blueprint `yafowil.widget.autocomplete 
-<http://github.com/bluedynamics/yafowil.widget.autocomplete/>`_ utilizing 
-``jquery.ui.autocomplete`` to offer the user a selection based on the input 
+    'autocomplete',
+    extractors=[
+        generic_extractor,
+        generic_required_extractor,
+        autocomplete_extractor
+    ],
+    edit_renderers=[
+        input_generic_renderer,
+        autocomplete_renderer
+    ]
+)
+
+factory.doc['blueprint']['autocomplete'] = """\
+Add-on blueprint `yafowil.widget.autocomplete
+<http://github.com/conestack/yafowil.widget.autocomplete/>`_ utilizing
+``jquery.ui.autocomplete`` to offer the user a selection based on the input
 given so far.
 """
 
 factory.defaults['autocomplete.type'] = 'text'
 
 factory.defaults['autocomplete.class'] = 'autocomplete'
 
 factory.defaults['autocomplete.required_class'] = 'required'
 
-factory.defaults['autocomplete.disabled'] = False 
+factory.defaults['autocomplete.disabled'] = False
 
-factory.defaults['autocomplete.size'] = None 
+factory.defaults['autocomplete.size'] = None
 
 factory.defaults['autocomplete.delay'] = '300'
-factory.doc['props']['autocomplete.delay'] = \
-"""Delay in milliseconds.
+factory.doc['props']['autocomplete.delay'] = """\
+Delay in milliseconds.
 """
 
 factory.defaults['autocomplete.minLength'] = '1'
-factory.doc['props']['autocomplete.minLength'] = \
-"""Minimum input length to trigger autocomplete.
+factory.doc['props']['autocomplete.minLength'] = """\
+Minimum input length to trigger autocomplete.
 """
 
-factory.doc['props']['autocomplete.source'] = \
-"""Autocomplete source as python iterable or string defining JSON view callback.
+factory.doc['props']['autocomplete.source'] = """\
+Autocomplete source as python iterable or string defining JSON view callback.
 """
```

### Comparing `yafowil.widget.autocomplete-1.7/README.rst` & `yafowil_widget_autocomplete-2.0a1/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 This is a **autocomplete widget** for for `YAFOWIL
 <http://pypi.python.org/pypi/yafowil>`_ - Yet Another Form WIdget Library.
 
-It utilizes/integrates `jquery.ui.autocomplete
-<http://docs.jquery.com/UI/Autocomplete>`_ for/in YAFOWIL providing an
-autocomplete function on a text input.
-
 - `Documentation <http://docs.yafowil.info/en/latest/blueprints.html#autocomplete>`_
 - `DEMO - see it Live <http://docs.demo.yafowil.info/++widget++yafowil.widget.autocomplete/index.html>`_
 
 
 Source Code
 ===========
 
 The sources are in a GIT DVCS with its main branches at
-`github <http://github.com/bluedynamics/yafowil.widget.autocomplete>`_.
+`github <http://github.com/conestack/yafowil.widget.autocomplete>`_.
 
 We'd be happy to see many forks and pull-requests to make YAFOWIL even better.
 
 
 Contributors
 ============
 
 - Jens Klein
 
 - Robert Niederreiter
 
 - Georg Bernhard
+
+- Lena Daxenbichler
```

### Comparing `yafowil.widget.autocomplete-1.7/setup.py` & `yafowil_widget_autocomplete-2.0a1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from setuptools import find_packages
 from setuptools import setup
 import os
 
 
-version = '1.7'
+def read_file(name):
+    with open(os.path.join(os.path.dirname(__file__), name)) as f:
+        return f.read()
+
+
+version = '2.0a1'
 shortdesc = 'Autocomplete Widget for YAFOWIL'
-longdesc = open(os.path.join(os.path.dirname(__file__), 'README.rst')).read()
-longdesc += open(os.path.join(os.path.dirname(__file__), 'HISTORY.rst')).read()
-longdesc += open(os.path.join(os.path.dirname(__file__), 'LICENSE.rst')).read()
-tests_require = ['yafowil[test]']
+longdesc = '\n\n'.join([read_file(name) for name in [
+    'README.rst',
+    'CHANGES.rst',
+    'LICENSE.rst'
+]])
 
 
 setup(
     name='yafowil.widget.autocomplete',
     version=version,
     description=shortdesc,
     long_description=longdesc,
@@ -24,30 +30,35 @@
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
     keywords='jquery jquery.ui.autocomplete widget yafowil',
-    author='BlueDynamics Alliance',
-    author_email='dev@bluedynamics.com',
-    url=u'http://pypi.python.org/pypi/yafowil.widget.autocomplete',
+    author='Yafowil Contributors',
+    author_email='dev@conestack.org',
+    url=u'http://github.com/conestack/yafowil.widget.autocomplete',
     license='Simplified BSD',
     packages=find_packages('src'),
-    package_dir = {'': 'src'},
+    package_dir={'': 'src'},
     namespace_packages=['yafowil', 'yafowil.widget'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'setuptools',
         'yafowil>2.1.99',
     ],
-    tests_require=tests_require,
+    tests_require=[
+        'lxml',
+        'zope.testrunner'
+    ],
+    extras_require=dict(test=[
+        'lxml',
+        'zope.testrunner'
+    ]),
     test_suite="yafowil.widget.autocomplete.tests",
-    extras_require = dict(
-        test=tests_require,
-    ),
     entry_points="""
     [yafowil.plugin]
     register = yafowil.widget.autocomplete:register
     example = yafowil.widget.autocomplete.example:get_example
-    """)
+    """
+)
```

### Comparing `yafowil.widget.autocomplete-1.7/HISTORY.rst` & `yafowil_widget_autocomplete-2.0a1/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,21 @@
-
-History
+Changes
 =======
 
+2.0a1 (2024-06-02)
+------------------
+
+- Extend JS by ``autocomplete_on_array_add`` and ``register_array_subscribers``
+  to enable usage in ``yafowil.widget.array``.
+  [lenadax]
+
+- Get rid of jQuery UI. Rewrite Jacascript widget using ES6.
+  [lenadax]
+
+
 1.7 (2018-07-16)
 ----------------
 
 - Python 3 compatibility.
   [rnix]
 
 - Convert doctests to unittests.
```

