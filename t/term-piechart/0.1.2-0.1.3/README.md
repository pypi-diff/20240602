# Comparing `tmp/term_piechart-0.1.2.tar.gz` & `tmp/term_piechart-0.1.3.tar.gz`

## Comparing `term_piechart-0.1.2.tar` & `term_piechart-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 term_piechart-0.1.2/Makefile
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 term_piechart-0.1.2/tox.ini
--rw-r--r--   0        0        0    21797 2020-02-02 00:00:00.000000 term_piechart-0.1.2/.github/images/chart_requests.jpg
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 term_piechart-0.1.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 term_piechart-0.1.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 term_piechart-0.1.2/examples/colors.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 term_piechart-0.1.2/examples/format.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 term_piechart-0.1.2/examples/ticking.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 term_piechart-0.1.2/requirements/dev.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 term_piechart-0.1.2/term_piechart/__init__.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 term_piechart-0.1.2/term_piechart/color.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 term_piechart-0.1.2/term_piechart/pie.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 term_piechart-0.1.2/term_piechart/slice.py
--rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 term_piechart-0.1.2/tests/test_color.py
--rw-r--r--   0        0        0    25978 2020-02-02 00:00:00.000000 term_piechart-0.1.2/tests/test_pie.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 term_piechart-0.1.2/tests/test_slice.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 term_piechart-0.1.2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 term_piechart-0.1.2/LICENSE
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 term_piechart-0.1.2/README.md
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 term_piechart-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 term_piechart-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 term_piechart-0.1.3/Makefile
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 term_piechart-0.1.3/tox.ini
+-rw-r--r--   0        0        0    21310 2020-02-02 00:00:00.000000 term_piechart-0.1.3/.github/images/chart_requests.jpg
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 term_piechart-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 term_piechart-0.1.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 term_piechart-0.1.3/examples/colors.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 term_piechart-0.1.3/examples/format.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 term_piechart-0.1.3/examples/ticking.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 term_piechart-0.1.3/requirements/dev.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 term_piechart-0.1.3/term_piechart/__init__.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 term_piechart-0.1.3/term_piechart/color.py
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 term_piechart-0.1.3/term_piechart/pie.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 term_piechart-0.1.3/term_piechart/slice.py
+-rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 term_piechart-0.1.3/tests/test_color.py
+-rw-r--r--   0        0        0    25978 2020-02-02 00:00:00.000000 term_piechart-0.1.3/tests/test_pie.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 term_piechart-0.1.3/tests/test_slice.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 term_piechart-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 term_piechart-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 term_piechart-0.1.3/README.md
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 term_piechart-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 term_piechart-0.1.3/PKG-INFO
```

### Comparing `term_piechart-0.1.2/Makefile` & `term_piechart-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `term_piechart-0.1.2/.github/workflows/tests.yml` & `term_piechart-0.1.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `term_piechart-0.1.2/examples/colors.py` & `term_piechart-0.1.3/examples/colors.py`

 * *Files identical despite different names*

### Comparing `term_piechart-0.1.2/term_piechart/color.py` & `term_piechart-0.1.3/term_piechart/color.py`

 * *Files identical despite different names*

### Comparing `term_piechart-0.1.2/term_piechart/pie.py` & `term_piechart-0.1.3/term_piechart/pie.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# colorama
 from __future__ import annotations
 
 from math import atan2
 from math import degrees
 from math import sqrt
 
 from .color import co
@@ -163,15 +162,15 @@
         label_horiz_space = self.legend_left()
         label_offset = int(len(labels) / 2)
         label_boundry = int(label_vert_space * label_offset)
         labels_range = list(range(-label_boundry, label_boundry + 1, label_vert_space))
 
         for y in range(-self.radius, self.radius + 1):
             width = round(sqrt(self.radius * self.radius - y * y) * self.aspect_ratio)
-            width = width if width != 0 else round(self.radius / self.aspect_ratio)
+            width = width if width != 0 or self.aspect_ratio == 1 else round(self.radius / self.aspect_ratio)
 
             if not self.top:
                 output.append((self.center_x - width) * " ")
 
             for x in range(-width, width + 1):
                 angle = degrees(atan2(x, y))
                 item = items[Pie.select_data_item(angle, angles)]  # type: ignore
```

### Comparing `term_piechart-0.1.2/term_piechart/slice.py` & `term_piechart-0.1.3/term_piechart/slice.py`

 * *Files identical despite different names*

### Comparing `term_piechart-0.1.2/tests/test_color.py` & `term_piechart-0.1.3/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `term_piechart-0.1.2/tests/test_pie.py` & `term_piechart-0.1.3/tests/test_pie.py`

 * *Files identical despite different names*

### Comparing `term_piechart-0.1.2/tests/test_slice.py` & `term_piechart-0.1.3/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `term_piechart-0.1.2/LICENSE` & `term_piechart-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `term_piechart-0.1.2/README.md` & `term_piechart-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `term_piechart-0.1.2/pyproject.toml` & `term_piechart-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `term_piechart-0.1.2/PKG-INFO` & `term_piechart-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: term-piechart
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library to print piecharts in your terminal
 Project-URL: Changelog, https://github.com/va-h/term-piechart/releases
 Project-URL: Homepage, https://github.com/va-h/term-piechart
 Project-URL: Source, https://github.com/va-h/term-piechart
 License: MIT
 License-File: LICENSE
 Classifier: Environment :: Console
```

