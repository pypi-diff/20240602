# Comparing `tmp/qsketchmetric-1.7.1.tar.gz` & `tmp/qsketchmetric-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsketchmetric-1.7.1.tar", last modified: Mon Nov  6 10:15:44 2023, max compression
+gzip compressed data, was "qsketchmetric-1.7.2.tar", last modified: Sun Jun  2 11:36:35 2024, max compression
```

## Comparing `qsketchmetric-1.7.1.tar` & `qsketchmetric-1.7.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 10:15:44.480836 qsketchmetric-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-11-06 10:15:05.000000 qsketchmetric-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2023-11-06 10:15:44.480836 qsketchmetric-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2023-11-06 10:15:05.000000 qsketchmetric-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 10:15:44.476836 qsketchmetric-1.7.1/qsketchmetric/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-06 10:15:05.000000 qsketchmetric-1.7.1/qsketchmetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17730 2023-11-06 10:15:05.000000 qsketchmetric-1.7.1/qsketchmetric/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2023-11-06 10:15:05.000000 qsketchmetric-1.7.1/qsketchmetric/semiautomatic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 10:15:44.480836 qsketchmetric-1.7.1/qsketchmetric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2023-11-06 10:15:44.000000 qsketchmetric-1.7.1/qsketchmetric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-11-06 10:15:44.000000 qsketchmetric-1.7.1/qsketchmetric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 10:15:44.000000 qsketchmetric-1.7.1/qsketchmetric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-06 10:15:44.000000 qsketchmetric-1.7.1/qsketchmetric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-06 10:15:44.000000 qsketchmetric-1.7.1/qsketchmetric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 10:15:44.480836 qsketchmetric-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-11-06 10:15:05.000000 qsketchmetric-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 10:15:44.480836 qsketchmetric-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 10:15:05.000000 qsketchmetric-1.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19786 2023-11-06 10:15:05.000000 qsketchmetric-1.7.1/tests/test_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2023-11-06 10:15:05.000000 qsketchmetric-1.7.1/tests/test_semiautomatic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:36:35.944540 qsketchmetric-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-06-02 11:36:12.000000 qsketchmetric-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-06-02 11:36:35.944540 qsketchmetric-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-06-02 11:36:12.000000 qsketchmetric-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:36:35.944540 qsketchmetric-1.7.2/qsketchmetric/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 11:36:12.000000 qsketchmetric-1.7.2/qsketchmetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18364 2024-06-02 11:36:12.000000 qsketchmetric-1.7.2/qsketchmetric/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-06-02 11:36:12.000000 qsketchmetric-1.7.2/qsketchmetric/semiautomatic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:36:35.944540 qsketchmetric-1.7.2/qsketchmetric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-06-02 11:36:35.000000 qsketchmetric-1.7.2/qsketchmetric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-02 11:36:35.000000 qsketchmetric-1.7.2/qsketchmetric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 11:36:35.000000 qsketchmetric-1.7.2/qsketchmetric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 11:36:35.000000 qsketchmetric-1.7.2/qsketchmetric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-02 11:36:35.000000 qsketchmetric-1.7.2/qsketchmetric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 11:36:35.944540 qsketchmetric-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-06-02 11:36:12.000000 qsketchmetric-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:36:35.944540 qsketchmetric-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 11:36:12.000000 qsketchmetric-1.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20100 2024-06-02 11:36:12.000000 qsketchmetric-1.7.2/tests/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11660 2024-06-02 11:36:12.000000 qsketchmetric-1.7.2/tests/test_semiautomatic.py
```

### Comparing `qsketchmetric-1.7.1/LICENSE` & `qsketchmetric-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qsketchmetric-1.7.1/PKG-INFO` & `qsketchmetric-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsketchmetric
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python 2D parametric DXF rendering engine.
 Home-page: https://github.com/MadScrewdriver/qsketchmetric
 Author: Franciszek Łajszczak
 Author-email: franciszek@lajszczak.dev
 License: MIT
 Project-URL: Documentation, https://qsketchmetric.readthedocs.io/
 Keywords: CAD,QCAD,2D,parametric,drawing,renderer,python renderer,python CAD,python 2d CAD,ppython 2d drawing,python parametric drawing,python parametric CAD,python QCAD,QCAD python,parametric QCAD python,parametric QCAD,QCAD parametric,QCAD python parametric,QCAD python 2d,
```

### Comparing `qsketchmetric-1.7.1/README.md` & `qsketchmetric-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `qsketchmetric-1.7.1/qsketchmetric/renderer.py` & `qsketchmetric-1.7.2/qsketchmetric/renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import string
 from copy import deepcopy
 from pathlib import Path
 from random import choice
 from typing import Optional, Dict
 
 import ezdxf
-from ezdxf import units, bbox
+from ezdxf import bbox
 from ezdxf.addons import Importer
-from ezdxf.entities import DXFGraphic, Insert
+from ezdxf.document import Drawing
+from ezdxf.entities import DXFGraphic
 from ezdxf.layouts import Modelspace
 from ezdxf.math import Vec3
 from py_expression_eval import Parser  # type: ignore
-from ezdxf.document import Drawing
 
 
 class Renderer:
     """
     :param input_parametric_path: Path to the parametric file intended for rendering.
     :param output_rendered_object: A pre-initialized :class:`ezdxf.document.Drawing` drawing object.
         You can initialize such an object using methods like :meth:`ezdxf.readfile` or :meth:`ezdxf.new`
@@ -163,20 +163,21 @@
                 self.variables["c"] = math.dist(start, end)
 
                 if constant_xdata == "?":
                     pass
                 else:
                     new_length = Parser().parse(constant_xdata).evaluate(self.variables)
 
-                e_data = {"layer": layer, "linetype": line_type}
+                e_data_start = {"layer": layer, "linetype": line_type, "start": True}
+                e_data_end = {"layer": layer, "linetype": line_type, "start": False}
 
-                self.graph[end] = self.graph.get(end, []) + [("LINE", start, new_length, e_data)]
-                self.graph[start] = self.graph.get(start, []) + [("LINE", end, new_length, e_data)]
-                self.visited_graph[end] = self.visited_graph.get(end, []) + [(e_data["layer"], start)]
-                self.visited_graph[start] = self.visited_graph.get(start, []) + [(e_data["layer"], end)]
+                self.graph[end] = self.graph.get(end, []) + [("LINE", start, new_length, e_data_end)]
+                self.graph[start] = self.graph.get(start, []) + [("LINE", end, new_length, e_data_start)]
+                self.visited_graph[end] = self.visited_graph.get(end, []) + [(layer, start)]
+                self.visited_graph[start] = self.visited_graph.get(start, []) + [(layer, end)]
 
             elif entity.dxftype() == "CIRCLE":
                 center = entity.dxf.center
                 center = Vec3(round(center.x, self.accuracy), round(center.y, self.accuracy), 0)
                 self.variables["c"] = entity.dxf.radius
 
                 new_length = Parser().parse(constant_xdata).evaluate(self.variables)
@@ -269,19 +270,25 @@
         This method iterates through the graph data. Identifies lines that were marked with '?' as their length,
         and constructs them based on the already processed entities.
         """
 
         for node, v in self.graph.items():
             for line in [l for l in v if
                          l[0] == "LINE" and l[2] == "?" and (l[3]["layer"], l[1]) in self.visited_graph[node]]:
-                self.new_entities.append(self.output_msp.add_line((
-                    self.new_points[node][0] + self.offset_x, self.new_points[node][1] + self.offset_y),
-                    (self.new_points[line[1]][0] + self.offset_x,
-                     self.new_points[line[1]][1] + self.offset_y),
-                    dxfattribs={"layer": line[3]["layer"], "linetype": line[3]["linetype"]}))
+                start = (self.new_points[node][0] + self.offset_x, self.new_points[node][1] + self.offset_y)
+                end = (self.new_points[line[1]][0] + self.offset_x, self.new_points[line[1]][1] + self.offset_y)
+                start, end = (start, end) if line[3]["start"] else (end, start)
+
+                self.new_entities.append(
+                    self.output_msp.add_line(
+                        start, end,
+                        dxfattribs={"layer": line[3]["layer"], "linetype": line[3]["linetype"]}
+                    )
+                )
+
                 self.visited_graph[line[1]].remove((line[3]["layer"], node))
                 self.visited_graph[node].remove((line[3]["layer"], line[1]))
 
     def _dfs(self, node: Vec3, offset_x: float, offset_y: float):
         """
             .. note:: This method is private and not intended for external use.
 
@@ -314,30 +321,36 @@
 
                     new_offset_x = (vector.x - node.x) * factor - (vector.x - node.x)
                     new_offset_y = (vector.y - node.y) * factor - (vector.y - node.y)
 
                     self.new_points[vector] = (vector.x + offset_x + new_offset_x, vector.y + offset_y + new_offset_y)
 
                     if data["layer"] != "VIRTUAL_LAYER":
+                        start = (node.x + offset_x + self.offset_x, node.y + offset_y + self.offset_y)
+                        end = (vector.x + offset_x + new_offset_x + self.offset_x,
+                               vector.y + offset_y + new_offset_y + self.offset_y)
+
+                        start, end = (start, end) if data["start"] else (end, start)
+
                         self.new_entities.append(self.output_msp.add_line(
-                            (node.x + offset_x + self.offset_x, node.y + offset_y + self.offset_y), (
-                                vector.x + offset_x + new_offset_x + self.offset_x,
-                                vector.y + offset_y + new_offset_y + self.offset_y),
+                            start, end,
                             dxfattribs={"layer": data["layer"], "linetype": data["linetype"]}))
 
                     self.visited_graph[node].remove((data["layer"], vector))
                     self.visited_graph[vector].remove((data["layer"], node))
 
                     self._dfs(vector, offset_x + new_offset_x, offset_y + new_offset_y)
 
             elif name == "INSERT":
                 self.new_entities.append(self.output_msp.add_blockref(data["name"], (
                     node.x + offset_x + self.offset_x, node.y + offset_y + self.offset_y),
-                    dxfattribs={"layer": data["layer"], "xscale": data["xscale"], "yscale": data["yscale"],
-                                "linetype": data["linetype"]}))
+                                                                      dxfattribs={"layer": data["layer"],
+                                                                                  "xscale": data["xscale"],
+                                                                                  "yscale": data["yscale"],
+                                                                                  "linetype": data["linetype"]}))
 
             elif name == "POINT":
                 self.points[data["name"]] = (node.x + offset_x, node.y + offset_y)
 
     def _center_drawing(self):
         """
             .. note:: This method is private and not intended for external use.
```

### Comparing `qsketchmetric-1.7.1/qsketchmetric/semiautomatic.py` & `qsketchmetric-1.7.2/qsketchmetric/semiautomatic.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,12 +239,12 @@
             line.set_xdata(self.APPID, [(1000, f"c:{self.value}")])
 
     def _draw_variables(self):
         """
             Draws the MTEXT entity.
         """
 
-        text = "Available variables: \P\P----- buld in -----\P\Pc: const\P?: undefined \P\P ----- custom -----\P\P"
+        text = "Available variables: \P\P----- build in -----\P\Pc: const\P?: undefined \P\P ----- custom -----\P\P"
         variable_text = self.input_msp.add_mtext(text, dxfattribs={"attachment_point": 8})
 
         variable_text.dxf.char_height = 10
         variable_text.set_location(insert=(-100, 100, 0), rotation=0)
```

### Comparing `qsketchmetric-1.7.1/qsketchmetric.egg-info/PKG-INFO` & `qsketchmetric-1.7.2/qsketchmetric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsketchmetric
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python 2D parametric DXF rendering engine.
 Home-page: https://github.com/MadScrewdriver/qsketchmetric
 Author: Franciszek Łajszczak
 Author-email: franciszek@lajszczak.dev
 License: MIT
 Project-URL: Documentation, https://qsketchmetric.readthedocs.io/
 Keywords: CAD,QCAD,2D,parametric,drawing,renderer,python renderer,python CAD,python 2d CAD,ppython 2d drawing,python parametric drawing,python parametric CAD,python QCAD,QCAD python,parametric QCAD python,parametric QCAD,QCAD parametric,QCAD python parametric,QCAD python 2d,
```

### Comparing `qsketchmetric-1.7.1/setup.py` & `qsketchmetric-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `qsketchmetric-1.7.1/tests/test_renderer.py` & `qsketchmetric-1.7.2/tests/test_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,29 +53,33 @@
             self.point1: self.new_point1_off,
             self.point2: self.new_point2_off,
             self.point3: self.new_point3_off,
         }
 
         self.graph = {
             self.point1: [
-                ("LINE", self.point2, self.line1_length, {"layer": "VIRTUAL_LAYER", "linetype": "line_linetype"}),
-                ("LINE", self.point3, self.line2_length, {"layer": "line_layer", "linetype": "line_linetype"}),
+                ("LINE", self.point2, self.line1_length, {"layer": "VIRTUAL_LAYER", "linetype": "line_linetype",
+                                                          "start": True}),
+                ("LINE", self.point3, self.line2_length, {"layer": "line_layer", "linetype": "line_linetype",
+                                                          "start": True}),
                 ("ARC", self.point1, self.arc_radius, {"layer": "arc_layer", "linetype": "arc_linetype",
                                                        "radius": self.arc_radius, "start_angle": self.start_angle,
                                                        "end_angle": self.end_angle})],
 
-            self.point2: [("LINE", self.point3, "?", {"layer": "line_layer", "linetype": "line_linetype"}),
+            self.point2: [("LINE", self.point3, "?", {"layer": "line_layer", "linetype": "line_linetype",
+                                                      "start": True}),
                           ("LINE", self.point1, self.line1_length,
-                           {"layer": "VIRTUAL_LAYER", "linetype": "line_linetype"}),
+                           {"layer": "VIRTUAL_LAYER", "linetype": "line_linetype", "start": True}),
                           ("CIRCLE", self.point2, self.circle_radius,
                            {"layer": "circle_layer", "linetype": "circle_linetype", "radius": self.circle_radius})],
 
-            self.point3: [("LINE", self.point2, "?", {"layer": "line_layer", "linetype": "line_linetype"}),
+            self.point3: [("LINE", self.point2, "?", {"layer": "line_layer", "linetype": "line_linetype",
+                                                      "start": True}),
                           ("LINE", self.point1, self.line2_length,
-                           {"layer": "circle_layer", "linetype": "circle_linetype"}),
+                           {"layer": "circle_layer", "linetype": "circle_linetype", "start": True}),
                           ("POINT", self.point3, 0, {"name": "mock"}),
                           ("INSERT", self.point3, 0,
                           {"layer": "insert_layer", "linetype": "insert_linetype", "name": "insert",
                            "xscale": 1.5, "yscale": 1})],
         }
 
         self.entities = ['LINE', 'CIRCLE', 'ARC', 'INSERT']
```

### Comparing `qsketchmetric-1.7.1/tests/test_semiautomatic.py` & `qsketchmetric-1.7.2/tests/test_semiautomatic.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
                                                dxfattribs={"layer": "VIRTUAL_LAYER"})
         obj.input_msp.add_line.assert_any_call(self.point3, (self.point3.x, self.point1.y),
                                                dxfattribs={"layer": "VIRTUAL_LAYER"})
 
     @patch.object(SemiAutomaticParameterization, "_handle_output_path")
     @patch("ezdxf.readfile")
     def test_draw_variables(self, mock_readfile, mock_handle_output_path):
-        text = "Available variables: \P\P----- buld in -----\P\Pc: const\P?: undefined \P\P ----- custom -----\P\P"
+        text = "Available variables: \P\P----- build in -----\P\Pc: const\P?: undefined \P\P ----- custom -----\P\P"
 
         obj = SemiAutomaticParameterization(self.mock_input_dxf_path)
         obj.input_msp = Mock()
 
         variable_text = Mock()
         obj.input_msp.add_mtext.return_value = variable_text
```

