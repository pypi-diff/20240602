# Comparing `tmp/zprp_ffmpeg-2.0.0.tar.gz` & `tmp/zprp_ffmpeg-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zprp_ffmpeg-2.0.0.tar", max compression
+gzip compressed data, was "zprp_ffmpeg-2.1.0.tar", max compression
```

## Comparing `zprp_ffmpeg-2.0.0.tar` & `zprp_ffmpeg-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       83 2024-03-19 10:18:25.914851 zprp_ffmpeg-2.0.0/AUTHORS.rst
--rw-r--r--   0        0        0     1088 2024-03-19 10:18:25.914851 zprp_ffmpeg-2.0.0/LICENSE
--rw-r--r--   0        0        0     4266 2024-05-31 22:19:01.014961 zprp_ffmpeg-2.0.0/README.rst
--rw-r--r--   0        0        0     1915 2024-05-31 22:19:01.014961 zprp_ffmpeg-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      720 2024-05-20 20:33:29.596366 zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/BaseConnector.py
--rw-r--r--   0        0        0     5711 2024-05-31 22:16:37.465014 zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/FilterGraph.py
--rw-r--r--   0        0        0     1418 2024-05-31 22:16:37.465014 zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/ProcessConnector.py
--rw-r--r--   0        0        0      824 2024-05-31 22:19:01.014961 zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/__init__.py
--rw-r--r--   0        0        0     1028 2024-05-20 20:33:29.596366 zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/_api_compat.py
--rw-r--r--   0        0        0     2731 2024-05-31 22:16:37.465014 zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/filters.py
--rw-r--r--   0        0        0   475344 2024-05-31 22:16:37.465014 zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/generated_filters.py
--rw-r--r--   0        0        0      907 2024-05-25 16:49:31.174794 zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/probe.py
--rw-r--r--   0        0        0        0 2024-05-10 14:12:06.788837 zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/py.typed
--rw-r--r--   0        0        0     1398 2024-05-25 16:49:34.114793 zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/view.py
--rw-r--r--   0        0        0     5050 1970-01-01 00:00:00.000000 zprp_ffmpeg-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       83 2024-03-19 10:18:25.914851 zprp_ffmpeg-2.1.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1088 2024-03-19 10:18:25.914851 zprp_ffmpeg-2.1.0/LICENSE
+-rw-r--r--   0        0        0     4266 2024-06-01 20:08:31.011570 zprp_ffmpeg-2.1.0/README.rst
+-rw-r--r--   0        0        0     1914 2024-06-01 20:08:31.011570 zprp_ffmpeg-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      720 2024-05-20 20:33:29.596366 zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/BaseConnector.py
+-rw-r--r--   0        0        0     5955 2024-06-01 20:08:31.011570 zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/FilterGraph.py
+-rw-r--r--   0        0        0     1418 2024-05-31 22:16:37.465014 zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/ProcessConnector.py
+-rw-r--r--   0        0        0     1072 2024-06-01 20:08:31.011570 zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/__init__.py
+-rw-r--r--   0        0        0     2072 2024-06-01 20:08:31.011570 zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/_api_compat.py
+-rw-r--r--   0        0        0     2738 2024-05-31 23:13:25.841615 zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/filters.py
+-rw-r--r--   0        0        0   475344 2024-05-31 22:16:37.465014 zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/generated_filters.py
+-rw-r--r--   0        0        0      907 2024-05-25 16:49:31.174794 zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/probe.py
+-rw-r--r--   0        0        0        0 2024-05-10 14:12:06.788837 zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/py.typed
+-rw-r--r--   0        0        0     1434 2024-06-01 16:10:23.780649 zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/view.py
+-rw-r--r--   0        0        0     5050 1970-01-01 00:00:00.000000 zprp_ffmpeg-2.1.0/PKG-INFO
```

### Comparing `zprp_ffmpeg-2.0.0/LICENSE` & `zprp_ffmpeg-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zprp_ffmpeg-2.0.0/README.rst` & `zprp_ffmpeg-2.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/zprp-ffmpeg
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/zprp-ffmpeg.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/zprp-ffmpeg
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ffmpeg-zprp/zprp-ffmpeg/v2.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ffmpeg-zprp/zprp-ffmpeg/v2.1.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/compare/v2.0.0...main
+    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/compare/v2.1.0...main
 
 
 
 .. end-badges
 
 Implementation of the successor to the ffmpeg-python library
```

### Comparing `zprp_ffmpeg-2.0.0/pyproject.toml` & `zprp_ffmpeg-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zprp-ffmpeg"
-version = "2.0.0"
+version = "2.1.0"
 description = "ffmpeg filter graph bindings for python"
 authors = ["Your Name <you@example.com>"]
 license = "MIT"
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -14,15 +14,14 @@
 networkx = "^2.6.3"
 matplotlib = "^3.4.3"
 
 [tool.poetry.group.typecheck.dependencies]
 types-tqdm = "^4.66.0.20240417"
 mypy = "^1.10.0"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 extend-exclude = ["static", "ci/templates"]
 line-length = 140
```

### Comparing `zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/BaseConnector.py` & `zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/BaseConnector.py`

 * *Files identical despite different names*

### Comparing `zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/FilterGraph.py` & `zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/FilterGraph.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 
 
 class Filter:
     """Filters can have many inputs and many outputs, holds the filter name and potential params"""
 
     def __init__(self, command: str, params: Optional[List[FilterOption]] = None, filter_type: str = FilterType.VIDEO.value):
         self._out: List[AnyNode] = []
-        self._in: List[AnyNode] = []
+        self._in: List[AnyNode | "Stream"] = []
         self.command = command
         self.params = params if params else []
         self.filter_type = filter_type
 
     def add_output(self, parent: "Filter | SinkFilter"):
         self._out.append(parent)
 
     def add_input(self, child: "Filter | SourceFilter | Stream"):
         self._in.append(child)
 
     def get_command(self):
-        joined_params = ":".join(p.name + "=" + str(p.value) for p in self.params if p.value)
+        joined_params = ":".join(p.name + "=" + str(p.value) if p.value else p.name for p in self.params)
         if joined_params:  # if there was no option, leave empty string
             joined_params = "=" + joined_params
         if self.filter_type == "AVMEDIA_TYPE_VIDEO":
             return ":v]" + self.command + joined_params
 
         elif self.filter_type == "AVMEDIA_TYPE_AUDIO":
             return ":a]" + self.command + joined_params
@@ -92,14 +92,15 @@
 
 class Stream:
     """One directional sequence of nodes, in future will be able to visualize them.
     Streams can be concatenated and split with certain filters."""
 
     def __init__(self) -> None:
         self._nodes: List[AnyNode] = []
+        self.global_options: List = []
 
     def append(self, node: AnyNode) -> "Stream":
         if len(self._nodes) > 0:
             # connect head with new node
             if not isinstance(self._nodes[-1], SinkFilter) and not isinstance(node, SourceFilter):
                 self._nodes[-1].add_output(node)
                 node.add_input(self._nodes[-1])
@@ -115,25 +116,25 @@
         self.filter_counter = 0
         self.result_counter = 0
 
         self.inputs = []
         self.outputs = []
         self.filters = []
 
-    def generate_command(self, stream: Stream) -> str:
-        last = None
+    def generate_command(self, stream: Stream) -> str:  # type: ignore
+        last = "None"
         for node in stream._nodes:
             # many inputs one output
             if (command := node.get_command()) and any(filter_ in command for filter_ in self.multi_input):
                 last_results = []
                 _, command = command.split("]")
-                for graph in node._in:
-                    last_results.append(self.generate_command(graph))
-                last_results = "".join([f"[{result}]" for result in last_results])
-                self.filters.append(f"{last_results}{command}[v{self.result_counter}];")
+                for graph in node._in:  # type: ignore
+                    last_results.append(self.generate_command(graph))  # type: ignore
+                results = "".join([f"[{result}]" for result in last_results])
+                self.filters.append(f"{results}{command}[v{self.result_counter}];")
                 last = f"v{self.result_counter}"
                 self.result_counter += 1
             # input
             elif isinstance(node, SourceFilter):
                 self.inputs.append(f"{command}")
                 last = self.inputs_counter
                 self.inputs_counter += 1
@@ -148,12 +149,14 @@
             else:
                 if isinstance(last, int):
                     self.filters.append(f"[{last}{command}[v{self.result_counter}];")
                 else:
                     self.filters.append(f"[{last}{command[2:]}[v{self.result_counter}];")
                 last = f"v{self.result_counter}"
                 self.result_counter += 1
+        if len(self.filters) == 0:
+            raise ValueError("No filters selected")
         return last
 
-    def generate_result(self, stream):
+    def generate_result(self, stream: Stream) -> str:
         self.generate_command(stream)
-        return " ".join(self.inputs) + ' -filter_complex "' + " ".join(self.filters)[:-1] + '" ' + " ".join(self.outputs)
+        return " ".join(self.inputs) + ' -filter_complex "' + " ".join(self.filters)[:-1] + '" ' + " ".join(self.outputs) + ' ' + " ".join(stream.global_options)
```

### Comparing `zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/ProcessConnector.py` & `zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/ProcessConnector.py`

 * *Files identical despite different names*

### Comparing `zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/__init__.py` & `zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,32 @@
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 # from . import longest
 from inspect import getmembers
 from inspect import isfunction
+from typing import Any
 
 from ._api_compat import input
+from ._api_compat import filter
 from ._api_compat import output
+from ._api_compat import global_args
+from ._api_compat import get_args
+from ._api_compat import compile
 from ._api_compat import run
 from ._api_compat import run_async
 from .FilterGraph import Stream
 from .filters import *  # noqa: F403 this is impossible to avoid
 from .generated_filters import *  # noqa: F403 this is impossible to avoid
 from .probe import probe
 from .view import view
 
+generated_filters: Any
+_api_compat: Any
+
 # This is for `from xyz import *`, but also to make linter shut up
 
-__all__ = ["input", "output", "run", "run_async", "probe", "view", "generated_filters", "filters"]  # noqa: F405
+__all__ = ["input", "filter", "output", "global_args", "get_args", "compile", "run", "run_async", "probe", "view", "generated_filters", "filters"]  # noqa: F405
 
-stream_modules = [generated_filters, _api_compat]  # noqa: F405
+stream_modules = [generated_filters, _api_compat]  # noqa: F821
 
 for module in stream_modules:
     for name, func in getmembers(module, isfunction):
         setattr(Stream, name, func)
```

### Comparing `zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/filters.py` & `zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .FilterGraph import Filter
 from .FilterGraph import FilterOption
 from .FilterGraph import Stream
 
 
 def concat(graphs: Iterable[Stream], n: Optional[int] = None, v: Optional[int] = None, a: Optional[int] = None) -> Stream:
     """Concatenate audio and video streams, joining them together one after the other.
+
     :param int n: set the number of segments. Default is 2.
     :param int v: set the number of output video streams, that is also the number of video streams in each segment. Default is 1.
     :param int a: set the number of output audio streams, that is also the number of audio streams in each segment. Default is 0.
     """
     filter_ = Filter(
         "concat",
         params=[
@@ -34,26 +35,28 @@
     eval: Optional[str] = None,
     shortest: Optional[bool] = None,
     format: Optional[str] = None,
     repeatlast: Optional[bool] = None,
     alpha: Optional[str] = None,
 ) -> Stream:
     """Overlay a video source on top of the input.
+
     :param str x: set the x expression
     :param str y: set the y expression
     :param str eof_action: Action to take when encountering EOF from secondary input
             possible values: repeat, endall, pass
     :param str eval: specify when to evaluate expressions
             possible values: init, frame
     :param bool shortest: force termination when the shortest input terminates
     :param str format: set output format
             possible values: yuv420, yuv420p10, yuv422, yuv422p10, yuv444, yuv444p10, rgb, gbrp, auto
     :param bool repeatlast: repeat overlay of the last overlay frame
     :param str alpha: alpha format
-            possible values: straight, premultiplied"""
+            possible values: straight, premultiplied
+    """
     filter_ = Filter(
         command="overlay",
         filter_type="AVMEDIA_TYPE_VIDEO",
         params=[
             FilterOption(name="x", value=x),
             FilterOption(name="y", value=y),
             FilterOption(name="eof_action", value=eof_action),
```

### Comparing `zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/generated_filters.py` & `zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/generated_filters.py`

 * *Files identical despite different names*

### Comparing `zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/probe.py` & `zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/probe.py`

 * *Files identical despite different names*

### Comparing `zprp_ffmpeg-2.0.0/src/zprp_ffmpeg/view.py` & `zprp_ffmpeg-2.1.0/src/zprp_ffmpeg/view.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import networkx as nx
+import networkx as nx  # type: ignore
 from matplotlib import pyplot as plt
 
 from .FilterGraph import Filter
 from .FilterGraph import SinkFilter
 from .FilterGraph import SourceFilter
 from .FilterGraph import Stream
 
@@ -21,25 +21,25 @@
             graph_connection.append((node.in_path.split("/")[-1], colors["input"]))
         elif isinstance(node, SinkFilter):
             graph_connection.append((node.out_path.split("/")[-1], colors["output"]))
         elif isinstance(node, Filter):
             graph_connection.append((node.command, colors["filter"]))
 
     # Adding nodes
-    for node, color in graph_connection:
-        G.add_node(node, color=color)
+    for nodeG, color in graph_connection:
+        G.add_node(nodeG, color=color)
 
     # Adding edges
     for i in range(len(graph_connection) - 1):
         G.add_edge(graph_connection[i][0], graph_connection[i + 1][0])
 
     # Set nodes to be horizontal
     pos = {}
-    for i, node in enumerate(graph_connection):
-        pos[node[0]] = (i, 0)
+    for i, nodeG in enumerate(graph_connection):  # type: ignore
+        pos[nodeG[0]] = (i, 0)
 
     nx.draw(
         G, pos, with_labels=True, node_shape="s", node_size=3000, node_color=[color for _, color in graph_connection], font_weight="bold"
     )
 
     if filename:
         plt.savefig(filename)
```

### Comparing `zprp_ffmpeg-2.0.0/PKG-INFO` & `zprp_ffmpeg-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zprp-ffmpeg
-Version: 2.0.0
+Version: 2.1.0
 Summary: ffmpeg filter graph bindings for python
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -104,17 +104,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/zprp-ffmpeg
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/zprp-ffmpeg.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/zprp-ffmpeg
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ffmpeg-zprp/zprp-ffmpeg/v2.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ffmpeg-zprp/zprp-ffmpeg/v2.1.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/compare/v2.0.0...main
+    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/compare/v2.1.0...main
 
 
 
 .. end-badges
 
 Implementation of the successor to the ffmpeg-python library
```

