# Comparing `tmp/nummulith_drawing-0.0.1.tar.gz` & `tmp/nummulith_drawing-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nummulith_drawing-0.0.1.tar", last modified: Sun Jun  2 11:56:37 2024, max compression
+gzip compressed data, was "nummulith_drawing-0.0.19.tar", last modified: Sun Jun  2 20:01:44 2024, max compression
```

## Comparing `nummulith_drawing-0.0.1.tar` & `nummulith_drawing-0.0.19.tar`

### file list

```diff
@@ -1,15 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 11:56:37.579683 nummulith_drawing-0.0.1/
--rw-rw-rw-   0        0        0     1073 2024-06-02 11:50:07.000000 nummulith_drawing-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2579 2024-06-02 11:56:37.572675 nummulith_drawing-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1990 2024-02-26 11:17:31.000000 nummulith_drawing-0.0.1/README.md
--rw-rw-rw-   0        0        0      702 2024-06-02 11:56:16.000000 nummulith_drawing-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-02 11:56:37.580681 nummulith_drawing-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-02 11:56:37.526678 nummulith_drawing-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-06-02 11:56:37.544677 nummulith_drawing-0.0.1/src/Drawing/
--rw-rw-rw-   0        0        0        0 2024-06-02 11:51:43.000000 nummulith_drawing-0.0.1/src/Drawing/__init__.py
--rw-rw-rw-   0        0        0     5873 2024-05-27 22:58:29.000000 nummulith_drawing-0.0.1/src/Drawing/drawing.py
-drwxrwxrwx   0        0        0        0 2024-06-02 11:56:37.570680 nummulith_drawing-0.0.1/src/nummulith_drawing.egg-info/
--rw-rw-rw-   0        0        0     2579 2024-06-02 11:56:37.000000 nummulith_drawing-0.0.1/src/nummulith_drawing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-06-02 11:56:37.000000 nummulith_drawing-0.0.1/src/nummulith_drawing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 11:56:37.000000 nummulith_drawing-0.0.1/src/nummulith_drawing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-06-02 11:56:37.000000 nummulith_drawing-0.0.1/src/nummulith_drawing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:44.215551 nummulith_drawing-0.0.19/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:44.211551 nummulith_drawing-0.0.19/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:44.215551 nummulith_drawing-0.0.19/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-06-02 20:01:33.000000 nummulith_drawing-0.0.19/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-02 20:01:33.000000 nummulith_drawing-0.0.19/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 20:01:33.000000 nummulith_drawing-0.0.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-06-02 20:01:44.215551 nummulith_drawing-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-06-02 20:01:33.000000 nummulith_drawing-0.0.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:44.215551 nummulith_drawing-0.0.19/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)    34662 2024-06-02 20:01:33.000000 nummulith_drawing-0.0.19/doc/GraphDemo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-06-02 20:01:33.000000 nummulith_drawing-0.0.19/doc/GraphDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-06-02 20:01:33.000000 nummulith_drawing-0.0.19/doc/svgForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-06-02 20:01:33.000000 nummulith_drawing-0.0.19/doc/test.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-06-02 20:01:33.000000 nummulith_drawing-0.0.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 20:01:44.215551 nummulith_drawing-0.0.19/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:44.211551 nummulith_drawing-0.0.19/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:44.215551 nummulith_drawing-0.0.19/src/drawing/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 20:01:33.000000 nummulith_drawing-0.0.19/src/drawing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-06-02 20:01:44.000000 nummulith_drawing-0.0.19/src/drawing/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-06-02 20:01:33.000000 nummulith_drawing-0.0.19/src/drawing/drawing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:01:44.215551 nummulith_drawing-0.0.19/src/nummulith_drawing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-06-02 20:01:44.000000 nummulith_drawing-0.0.19/src/nummulith_drawing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-06-02 20:01:44.000000 nummulith_drawing-0.0.19/src/nummulith_drawing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 20:01:44.000000 nummulith_drawing-0.0.19/src/nummulith_drawing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 20:01:44.000000 nummulith_drawing-0.0.19/src/nummulith_drawing.egg-info/top_level.txt
```

### Comparing `nummulith_drawing-0.0.1/LICENSE` & `nummulith_drawing-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `nummulith_drawing-0.0.1/README.md` & `nummulith_drawing-0.0.19/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,38 @@
-[ReadMe.md](../ReadMe.md) \ [Graph Drawing Utility](Graph_Drawing_Utility.md)
-
-<table style="width: 100%">
-  <thead>
-    <tr>
-        <th>
-            <h1>Graph Drawing Utility</h1>
-        </th>
-        <th>
-            <img src="../img/Graph_Drawing_Utility.png" width="100" height="100">
-        </th>
-    </tr>
-  </thead>
-</table>
-
-## Overview
-The **Graph Drawing Utility** project provides a versatile tool for visualizing object relationships. This utility is designed to be seamlessly integrated into projects, allowing users to dynamically represent and explore the connections between objects.
-
-## Adding objects
-Users can add objects to the graph using the add_item method.
-
-## Adding views
-The item_view method provides a means to inspect the details of individual objects, facilitating a deeper understanding of the interconnected elements.
-Relationship Establishment:
-
-## Adding relations
-Users can establish relationships between objects using three types:
-add_parent: Defines an ownership relationship, clustering owned objects together.
-add_link: Creates a connection between objects using arrows.
-
-## Graph Rendering:
-The utility enables users to visualize the constructed object graph, providing a clear representation of the established relationships.
-
-## Example
-
-[Source code](../GraphDemo.py)
-
-<img src="../img/Graph-Demo.png">
-
-## Links
-
-| Read Me | Yet Another AWS Analyser | Object Model Framework | Graph Drawing Utility |
-| ------------- | ------------------------ | ---------------------- | --------------------- |
-| [<img src="../img/Home.png" width="100" height="100">](../ReadMe.md) | [<img src="../img/Yet_Another_AWS_Analyser.png" width="100" height="100">](../docs/Yet_Another_AWS_Analyser.md) | [<img src="../img/Object_Model_Framework.png" width="100" height="100">](../docs/Object_Model_Framework.md) | [<img src="../img/Graph_Drawing_Utility.png" width="100" height="100">](../docs/Graph_Drawing_Utility.md) |
+[ReadMe.md](../ReadMe.md) \ [Graph Drawing Utility](Graph_Drawing_Utility.md)
+
+<table style="width: 100%">
+  <thead>
+    <tr>
+        <th>
+            <h1>Graph Drawing Utility</h1>
+        </th>
+        <th>
+            <img src="https://github.com/nummulith/drawing/raw/main/doc/Graph_Drawing_Utility.png" width="100" height="100">
+        </th>
+    </tr>
+  </thead>
+</table>
+
+## Overview
+The **Graph Drawing Utility** project provides a versatile tool for visualizing object relationships. This utility is designed to be seamlessly integrated into projects, allowing users to dynamically represent and explore the connections between objects.
+
+## Adding objects
+Users can add objects to the graph using the add_item method.
+
+## Adding views
+The item_view method provides a means to inspect the details of individual objects, facilitating a deeper understanding of the interconnected elements.
+Relationship Establishment:
+
+## Adding relations
+Users can establish relationships between objects using three types:
+add_parent: Defines an ownership relationship, clustering owned objects together.
+add_link: Creates a connection between objects using arrows.
+
+## Graph Rendering:
+The utility enables users to visualize the constructed object graph, providing a clear representation of the established relationships.
+
+## Example
+
+[Source code](https://github.com/nummulith/drawing/raw/main/doc/GraphDemo.py)
+
+<img src="https://github.com/nummulith/drawing/raw/main/doc/Graph-Demo.png">
```

#### html2text {}

```diff
@@ -1,21 +1,17 @@
 [ReadMe.md](../ReadMe.md) \ [Graph Drawing Utility](Graph_Drawing_Utility.md)
-************ GGrraapphh DDrraawwiinngg UUttiilliittyy ************ [[....//iimmgg//GGrraapphh__DDrraawwiinngg__UUttiilliittyy..ppnngg]]
+************ GGrraapphh DDrraawwiinngg UUttiilliittyy ************ [[hhttttppss::////ggiitthhuubb..ccoomm//nnuummmmuulliitthh//ddrraawwiinngg//rraaww//
+                                    mmaaiinn//ddoocc//GGrraapphh__DDrraawwiinngg__UUttiilliittyy..ppnngg]]
 ## Overview The **Graph Drawing Utility** project provides a versatile tool for
 visualizing object relationships. This utility is designed to be seamlessly
 integrated into projects, allowing users to dynamically represent and explore
 the connections between objects. ## Adding objects Users can add objects to the
 graph using the add_item method. ## Adding views The item_view method provides
 a means to inspect the details of individual objects, facilitating a deeper
 understanding of the interconnected elements. Relationship Establishment: ##
 Adding relations Users can establish relationships between objects using three
 types: add_parent: Defines an ownership relationship, clustering owned objects
 together. add_link: Creates a connection between objects using arrows. ## Graph
 Rendering: The utility enables users to visualize the constructed object graph,
 providing a clear representation of the established relationships. ## Example
-[Source code](../GraphDemo.py) [../img/Graph-Demo.png]## Links | Read Me | Yet
-Another AWS Analyser | Object Model Framework | Graph Drawing Utility | | -----
--------- | ------------------------ | ---------------------- | ----------------
------ | | [[../img/Home.png]](../ReadMe.md) | [[../img/
-Yet_Another_AWS_Analyser.png]](../docs/Yet_Another_AWS_Analyser.md) | [[../img/
-Object_Model_Framework.png]](../docs/Object_Model_Framework.md) | [[../img/
-Graph_Drawing_Utility.png]](../docs/Graph_Drawing_Utility.md) |
+[Source code](https://github.com/nummulith/drawing/raw/main/doc/GraphDemo.py)
+[https://github.com/nummulith/drawing/raw/main/doc/Graph-Demo.png]
```

### Comparing `nummulith_drawing-0.0.1/src/Drawing/drawing.py` & `nummulith_drawing-0.0.19/src/drawing/drawing.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-"""
-Drawing Module
-
-This module provides a class, Drawing, for generating diagrams with nodes and relationships
-  using the Graphviz engine. It simplifies the process of creating graphical representations
-  of objects, their hierarchy, and relationships.
-
-Class:
-- `Drawing`: Manages the creation and rendering of diagrams.
-
-Methods:
-- `add_item(node_id, node=None, cluster=None, point=None)`:
-      Add an item to the diagram with the specified attributes.
-- `add_parent(node_id, parent)`: Add a parent-child relationship between items.
-- `add_list(node_id, lst)`: Represent a list of items associated with an object in the diagram.
-- `add_link(node_id, link, label="")`: Add a link between two items with an optional label.
-
-Usage:
-- ...
-
-Author: Pavel ERESKO
-"""
-
-
-from graphviz import Digraph
-
-class Drawing:
-    ''' Class that provide drawing structure of nodes with parent, list, and links relations '''
-    def __init__(self):
-        self.items   = {}
-        self.parents = {}
-        self.lists   = {}
-        self.links   = []
-
-        self.linked = None
-
-    def item_view(self,
-        label = "[Item]", shape = "plaintext", style = 'filled', fillcolor = None, width = 0.1
-    ):
-        ''' Parameter passing function '''
-        return {
-            "label": label, "shape": shape, "style": style, "fillcolor": fillcolor, "width": width,
-        }
-
-    def add_item(self, node_id, node = None, cluster = None, point = None):
-        ''' Add node with html representation '''
-        if not node_id in self.items:
-            self.items[node_id] = {}
-
-        for name, par in {"node" : node, "cluster" : cluster, "point" : point}.items():
-            if par is None:
-                continue
-
-            labeldict = par
-            if name == "node" and isinstance(par, str):
-                labeldict = self.item_view(par)
-
-            self.items[node_id][name] = labeldict
-
-    def add_parent(self, node_id, parent):
-        ''' Add parent relation '''
-        self.parents[node_id] = parent
-
-    def add_list(self, node_id, node_list):
-        ''' Add list relation '''
-        self.lists[node_id] = node_list
-
-    def add_link(self, node_id, link, label = ""):
-        ''' Add link relation '''
-        self.links.append((node_id, link, label))
-
-    def print(self):
-        ''' Print nodes and relations added '''
-        print("\nDrawing")
-
-        print("\tItems  :")
-        for i, data in self.items  .items():
-            print(i, end=' ')
-        print()
-
-        print("\tParents:")
-        for i, data in self.parents.items():
-            print(f"{i} -> {data}")
-
-        print("\tLists  :")
-        for i, data in self.lists  .items():
-            print(i)
-
-        print("\tLinks  :")
-        for node_id, link, label in self.links:
-            print(f"{node_id} --[{label}]--> {link}")
-
-    def draw_rec(self, parent, grand_digraph):
-        ''' Recursively draws the nodes '''
-        items = [node_id for node_id in self.items if not node_id in
-                    [chi for chi, par in self.parents.items() if par in self.items]
-                ] if parent is None \
-                  else [node_id for node_id, par in self.parents.items() if par == parent]
-
-        if len(items) == 0:
-            view = self.items[parent]["node"]
-            grand_digraph.node(name=parent, shape=view["shape"], label = view["label"])
-
-        else:
-            par_context = None
-            par_digraph = None if parent is not None else grand_digraph
-
-            for node_id in items:
-                if par_digraph is None:
-                    par_context = grand_digraph.subgraph(name = "cluster_" + parent)
-                    par_digraph = par_context.__enter__()
-
-                    view = self.items[parent]["cluster"]
-
-                    # label = f'''<<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="4">
-                    #             {view["label"]}
-                    #             </TABLE>>'''
-                    label = view["label"]
-                    # print(label.replace("\n", ""))
-
-                    par_digraph.attr(
-                        label = label,
-                        style = view["style"],
-                        fillcolor = view["fillcolor"]
-                    )
-
-                    if parent in self.linked:
-                        view = self.items[parent]["point"]
-                        par_digraph.node(name=parent, shape=view["shape"], width=view["width"])
-
-                self.draw_rec(node_id, par_digraph)
-
-            if par_context is not None:
-                par_context.__exit__(None, None, None)
-
-
-    def draw(self, name):
-        ''' Draws the structure of nodes with all the relations '''
-        dot = Digraph(name)
-
-        self.linked = {}
-        for node_id, link, label in self.links:
-            self.linked[node_id] = True
-            self.linked[link] = True
-            dot.edge(node_id, link, label = label)
-
-        if len(self.items) > 0:
-            self.draw_rec(None, dot)
-
-        self.linked = None
-
-
-        with open('Y3A\\render\\Y3A.txt', 'w') as file:
-            file.write(dot.source)
-
-
-        try:
-            # dot.render(name, format='png', cleanup=True)
-            # dot.render(name, format='svg', cleanup=True)
-
-            #pixmap = QPixmap("Drawing.png")
-            #pixmap_item = QGraphicsPixmapItem(pixmap)
-            #Graph.scene().addItem(pixmap_item)
-            #Graph.fitInView(Graph.scene().sceneRect()) # Autoscaling
-
-            svg_str = dot.pipe(format='svg').decode('utf-8')
-        except Exception as e:
-            print(f"Draw error: {str(e)}")
-            return ""
-
-        svg_str = '\n'.join(svg_str.split('\n')[3:])
-
-        return svg_str
+"""
+Drawing Module
+
+This module provides a class, Drawing, for generating diagrams with nodes and relationships
+  using the Graphviz engine. It simplifies the process of creating graphical representations
+  of objects, their hierarchy, and relationships.
+
+Class:
+- `Drawing`: Manages the creation and rendering of diagrams.
+
+Methods:
+- `add_item(node_id, node=None, cluster=None, point=None)`:
+      Add an item to the diagram with the specified attributes.
+- `add_parent(node_id, parent)`: Add a parent-child relationship between items.
+- `add_list(node_id, lst)`: Represent a list of items associated with an object in the diagram.
+- `add_link(node_id, link, label="")`: Add a link between two items with an optional label.
+
+Usage:
+- ...
+
+Author: Pavel ERESKO
+"""
+
+
+from graphviz import Digraph
+
+class Drawing:
+    ''' Class that provide drawing structure of nodes with parent, list, and links relations '''
+    def __init__(self):
+        self.items   = {}
+        self.parents = {}
+        self.lists   = {}
+        self.links   = []
+
+        self.linked = None
+
+    def item_view(self,
+        label = "[Item]", shape = "plaintext", style = 'filled', fillcolor = None, width = 0.1
+    ):
+        ''' Parameter passing function '''
+        return {
+            "label": label, "shape": shape, "style": style, "fillcolor": fillcolor, "width": width,
+        }
+
+    def add_item(self, node_id, node = None, cluster = None, point = None):
+        ''' Add node with html representation '''
+        if not node_id in self.items:
+            self.items[node_id] = {}
+
+        for name, par in {"node" : node, "cluster" : cluster, "point" : point}.items():
+            if par is None:
+                continue
+
+            labeldict = par
+            if name == "node" and isinstance(par, str):
+                labeldict = self.item_view(par)
+
+            self.items[node_id][name] = labeldict
+
+    def add_parent(self, node_id, parent):
+        ''' Add parent relation '''
+        self.parents[node_id] = parent
+
+    def add_list(self, node_id, node_list):
+        ''' Add list relation '''
+        self.lists[node_id] = node_list
+
+    def add_link(self, node_id, link, label = ""):
+        ''' Add link relation '''
+        self.links.append((node_id, link, label))
+
+    def print(self):
+        ''' Print nodes and relations added '''
+        print("\nDrawing")
+
+        print("\tItems  :")
+        for i, data in self.items  .items():
+            print(i, end=' ')
+        print()
+
+        print("\tParents:")
+        for i, data in self.parents.items():
+            print(f"{i} -> {data}")
+
+        print("\tLists  :")
+        for i, data in self.lists  .items():
+            print(i)
+
+        print("\tLinks  :")
+        for node_id, link, label in self.links:
+            print(f"{node_id} --[{label}]--> {link}")
+
+    def draw_rec(self, parent, grand_digraph):
+        ''' Recursively draws the nodes '''
+        items = [node_id for node_id in self.items if not node_id in
+                    [chi for chi, par in self.parents.items() if par in self.items]
+                ] if parent is None \
+                  else [node_id for node_id, par in self.parents.items() if par == parent]
+
+        if len(items) == 0:
+            view = self.items[parent]["node"]
+            grand_digraph.node(name=parent, shape=view["shape"], label = view["label"])
+
+        else:
+            par_context = None
+            par_digraph = None if parent is not None else grand_digraph
+
+            for node_id in items:
+                if par_digraph is None:
+                    par_context = grand_digraph.subgraph(name = "cluster_" + parent)
+                    par_digraph = par_context.__enter__()
+
+                    view = self.items[parent]["cluster"]
+
+                    # label = f'''<<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="4">
+                    #             {view["label"]}
+                    #             </TABLE>>'''
+                    label = view["label"]
+                    # print(label.replace("\n", ""))
+
+                    par_digraph.attr(
+                        label = label,
+                        style = view["style"],
+                        fillcolor = view["fillcolor"]
+                    )
+
+                    if parent in self.linked:
+                        view = self.items[parent]["point"]
+                        par_digraph.node(name=parent, shape=view["shape"], width=view["width"])
+
+                self.draw_rec(node_id, par_digraph)
+
+            if par_context is not None:
+                par_context.__exit__(None, None, None)
+
+
+    def draw(self, name):
+        ''' Draws the structure of nodes with all the relations '''
+        dot = Digraph(name)
+
+        self.linked = {}
+        for node_id, link, label in self.links:
+            self.linked[node_id] = True
+            self.linked[link] = True
+            dot.edge(node_id, link, label = label)
+
+        if len(self.items) > 0:
+            self.draw_rec(None, dot)
+
+        self.linked = None
+
+
+        with open('Y3A\\render\\Y3A.txt', 'w') as file:
+            file.write(dot.source)
+
+
+        try:
+            # dot.render(name, format='png', cleanup=True)
+            # dot.render(name, format='svg', cleanup=True)
+
+            #pixmap = QPixmap("Drawing.png")
+            #pixmap_item = QGraphicsPixmapItem(pixmap)
+            #Graph.scene().addItem(pixmap_item)
+            #Graph.fitInView(Graph.scene().sceneRect()) # Autoscaling
+
+            svg_str = dot.pipe(format='svg').decode('utf-8')
+        except Exception as e:
+            print(f"Draw error: {str(e)}")
+            return ""
+
+        svg_str = '\n'.join(svg_str.split('\n')[3:])
+
+        return svg_str
```

