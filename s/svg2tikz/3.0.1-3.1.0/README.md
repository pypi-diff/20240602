# Comparing `tmp/svg2tikz-3.0.1.tar.gz` & `tmp/svg2tikz-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svg2tikz-3.0.1.tar", max compression
+gzip compressed data, was "svg2tikz-3.1.0.tar", max compression
```

## Comparing `svg2tikz-3.0.1.tar` & `svg2tikz-3.1.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      716 2023-01-12 15:48:31.564669 svg2tikz-3.0.1/LICENSE
--rw-r--r--   0        0        0     1148 2023-12-13 07:10:16.937152 svg2tikz-3.0.1/README.md
--rw-r--r--   0        0        0      965 2024-01-14 21:01:20.410069 svg2tikz-3.0.1/pyproject.toml
--rwxr-xr-x   0        0        0       51 2023-10-06 16:10:53.973707 svg2tikz-3.0.1/svg2tikz/__init__.py
--rw-r--r--   0        0        0    48922 2024-01-14 21:01:20.410069 svg2tikz-3.0.1/svg2tikz/tikz_export.py
--rw-r--r--   0        0        0     4923 2024-01-14 21:01:20.410069 svg2tikz-3.0.1/svg2tikz/tikz_export_effect.inx
--rw-r--r--   0        0        0     4892 2024-01-14 21:01:20.410069 svg2tikz-3.0.1/svg2tikz/tikz_export_output.inx
--rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 svg2tikz-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0      716 2023-01-12 15:48:31.564669 svg2tikz-3.1.0/LICENSE
+-rw-r--r--   0        0        0     1148 2024-05-19 08:16:17.819388 svg2tikz-3.1.0/README.md
+-rw-r--r--   0        0        0      983 2024-06-02 19:52:55.680567 svg2tikz-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-05-19 08:08:05.045057 svg2tikz-3.1.0/svg2tikz/.jukit/.jukit_info.json
+-rwxr-xr-x   0        0        0      136 2024-05-19 08:08:05.045057 svg2tikz-3.1.0/svg2tikz/__init__.py
+-rw-r--r--   0        0        0    50979 2024-05-19 08:13:23.900060 svg2tikz-3.1.0/svg2tikz/tikz_export.py
+-rw-r--r--   0        0        0     5191 2024-05-19 08:13:37.508010 svg2tikz-3.1.0/svg2tikz/tikz_export_effect.inx
+-rw-r--r--   0        0        0     5160 2024-05-19 08:13:49.679965 svg2tikz-3.1.0/svg2tikz/tikz_export_output.inx
+-rw-r--r--   0        0        0     1941 1970-01-01 00:00:00.000000 svg2tikz-3.1.0/PKG-INFO
```

### Comparing `svg2tikz-3.0.1/LICENSE` & `svg2tikz-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svg2tikz-3.0.1/README.md` & `svg2tikz-3.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <picture>
   <img alt="SVG2TikZ Logo" src="logo/svg2tikz.svg">
 </picture>
 
 [![Documentation][documentation-badge]][documentation-url]
 [![PyPI version](https://badge.fury.io/py/svg2tikz.svg)](https://badge.fury.io/py/svg2tikz)
 
-# SVG2TikZ 3.0.X (Inkscape 1.x.x compatible)
+# SVG2TikZ 3.1.X (Inkscape 1.x.x compatible)
 
 
 SVG2TikZ, formally known as Inkscape2TikZ ,are a set of tools for converting SVG graphics to TikZ/PGF code.
 This project is licensed under the GNU GPL  (see  the [LICENSE](/LICENSE) file).
 
 ## Documentation and installation
 `SVG2TikZ` is now available on pypi so you can install it with if you want to use it with a command line. You can install the package with the following command:
```

### Comparing `svg2tikz-3.0.1/pyproject.toml` & `svg2tikz-3.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "svg2tikz"
-version = "3.0.1"
+version = "3.1.0"
 description = "Tools for converting SVG graphics to TikZ/PGF code"
 authors = ["ldevillez <louis.devillez@gmail.com>", " Kjell Magne Fauske <kjellmf@gmail.com>"]
 maintainers = ["ldevillez <louis.devillez@gmail.com>"]
 license = "GPL-2.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -17,23 +17,23 @@
 sphinx-click = "^4.4.0"
 sphinx-copybutton = "^0.5.1"
 sphinxext-opengraph = "^0.7.5"
 furo = "^2023.9.10"
 sphinx-argparse = "^0.4.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
+black = ">=23.1,<25.0"
 pylint = "^2.16.2"
+coverage = "^7.5.1"
 
 
 [[tool.poetry.source]]
 name = "inkex_gitlab"
 url = "https://gitlab.com/api/v4/projects/40060814/packages/pypi/simple"
-default = false
-secondary = true
+priority = "supplemental"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.scripts]
```

### Comparing `svg2tikz-3.0.1/svg2tikz/tikz_export.py` & `svg2tikz-3.1.0/svg2tikz/tikz_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 SVG files from the command line.
 
 Author: Kjell Magne Fauske, Devillez Louis
 """
 
 import platform
 
-__version__ = "3.0.1"
+__version__ = "3.1.0"
 __author__ = "Devillez Louis, Kjell Magne Fauske"
 __maintainer__ = "Deville Louis"
 __email__ = "louis.devillez@gmail.com"
 
-
 import sys
 
 from textwrap import wrap
 import codecs
 import io
 import os
 from subprocess import Popen, PIPE
@@ -38,15 +37,15 @@
 import ctypes
 import inkex
 from inkex.transforms import Vector2d
 from lxml import etree
 
 try:
     SYS_OUTPUT_BUFFER = sys.stdout.buffer
-except AttributeError:
+except AttributeError:  # pragma: no cover
     logging.warning("Sys has no output buffer, redirecting to None")
     SYS_OUTPUT_BUFFER = None
 
 #### Utility functions and classes
 
 TIKZ_BASE_COLOR = [
     "black",
@@ -66,15 +65,14 @@
     "circle",
     "ellipse",
     "line",
     "polyline",
     "polygon",
 ]
 
-
 SPECIAL_TEX_CHARS = ["$", "\\", "%", "_", "#", "{", r"}", "^", "&"]
 SPECIAL_TEX_CHARS_REPLACE = [
     r"\$",
     r"$\backslash$",
     r"\%",
     r"\_",
     r"\#",
@@ -95,15 +93,15 @@
     '10\\%'
     >>> escape_texchars('%{}_^\\$')
     '\\%\\{\\}\\_\\^{}$\\backslash$\\$'
     """
     return "".join([_tex_charmap.get(c, c) for c in input_string])
 
 
-def copy_to_clipboard(text):
+def copy_to_clipboard(text):  # pragma: no cover
     """Copy text to the clipboard
 
     Returns True if successful. False otherwise.
     """
 
     text_type = str
 
@@ -212,28 +210,28 @@
 \usepackage{tikz}
 %(cropcode)s
 \begin{document}
 %(colorcode)s
 %(gradientcode)s
 \def \globalscale {%(scale)f}
 \begin{tikzpicture}[y=1%(unit)s, x=1%(unit)s, yscale=%(ysign)s\globalscale,"""
-    r"""xscale=\globalscale, every node/.append style={scale=\globalscale}, inner sep=0pt, outer sep=0pt%(extraoptions)s]
+    r"""xscale=\globalscale, every node/.append style={scale=\globalscale}, inner sep=0pt, outer sep=0pt]
 %(pathcode)s
 \end{tikzpicture}
 \end{document}
 """
 )
 
 FIG_TEMPLATE = (
     r"""
 %(colorcode)s
 %(gradientcode)s
 \def \globalscale {%(scale)f}
 \begin{tikzpicture}[y=1%(unit)s, x=1%(unit)s, yscale=%(ysign)s\globalscale,"""
-    r"""xscale=\globalscale, every node/.append style={scale=\globalscale}, inner sep=0pt, outer sep=0pt%(extraoptions)s]
+    r"""xscale=\globalscale, every node/.append style={scale=\globalscale}, inner sep=0pt, outer sep=0pt]
 %(pathcode)s
 \end{tikzpicture}
 """
 )
 
 SCALE = "scale"
 DICT = "dict"
@@ -289,14 +287,15 @@
     pos: final control point
 
     The calc_arc function is based on the calc_arc function in the
     paths_svg2obj.py script bundled with Blender 3D
     Copyright (c) jm soler juillet/novembre 2004-april 2007,
     Resource: https://developer.mozilla.org/fr/docs/Web/SVG/Tutorial/Paths#elliptical_arc (in french)
     """
+    # print(ang)
     ang = radians(ang)
 
     r = Vector2d(abs(r_i.x), abs(r_i.y))
 
     p_pos = Vector2d(
         abs((cos(ang) * (cp.x - pos.x) + sin(ang) * (cp.y - pos.y)) * 0.5) ** 2.0,
         abs((cos(ang) * (cp.y - pos.y) - sin(ang) * (cp.x - pos.x)) * 0.5) ** 2.0,
@@ -448,17 +447,25 @@
             help="Amount of boilerplate code (standalone, figonly, codeonly).",
         )
         parser.add_argument(
             "-t",
             "--texmode",
             dest="texmode",
             default="escape",
-            choices=("math", "escape", "raw"),
-            help="Set text mode (escape, math, raw). Defaults to 'escape'",
+            choices=("math", "escape", "raw", "attribute"),
+            help="Set text mode (escape, math, raw, attribute). Defaults to 'escape'",
+        )
+        parser.add_argument(
+            "--texmode-attribute",
+            default=None,
+            action="store",
+            dest="texmode_attribute",
+            help="The SVG attribute that specifies how to handle text",
         )
+
         parser.add_argument(
             "--markings",
             dest="markings",
             default="arrows",
             choices=("ignore", "include", "interpret", "arrows"),
             help="Set markings mode. Defaults to 'ignore'",
         )
@@ -741,14 +748,15 @@
             start_arrow = marking_interpret(ms)
             end_arrow = marking_interpret(me)
 
             return [start_arrow + "-" + end_arrow]
 
         if self.options.markings == "arrows":
             start_arrow = self.options.arrow[:] if ms is not None else ""
+
             if ms is not None and "end" in ms:
                 start_arrow += " reversed"
 
             if start_arrow == self.options.arrow:
                 start_arrow = "<"
                 if me is not None and "end" in me:
                     start_arrow = ">"
@@ -793,23 +801,28 @@
         style = node.specified_style()
         url = style.get("shape-inside")
         if url is None:
             return None
         shape = inkex.properties.match_url_and_return_element(url, self.svg)
         return shape
 
-    def style_to_tz(self, node=None):
+    def style_to_tz(self, node=None):  # pylint: disable=too-many-branches
         """
         Convert the style from the svg to the option to apply to tikz code
         """
 
         style = node.specified_style()
 
-        # No display
-        if style.get("display") == "none" or not node.is_visible:
+        # No display of the node
+        # Special handling of switch as they are meta elements
+        if node.TAG == "switch":
+            if style.get("display") == "none":
+                return ["none"]
+
+        elif style.get("display") == "none" or not node.is_visible:
             if node.TAG == "g":
                 return ["none"]
             return []
 
         options = []
 
         # Stroke and fill
@@ -843,24 +856,24 @@
                 if val < 1 and valuetype == FACTOR:
                     continue
 
                 if val != 1:
                     options.append(f"{tikzname}={self.round_value(float(value))}")
             elif valuetype == DICT:
                 if tikzname:
-                    options.append(f"{tikzname}={data.get(value,'')}")
+                    options.append(f"{tikzname}={data.get(value, '')}")
                 else:
                     options.append(data.get(value, ""))
-            elif valuetype == DIMENSION:
-                if value and value != data:
-                    options.append(
-                        f"{tikzname}="
-                        f"{self.round_value(self.convert_unit(value))}"
-                        f"{self.options.output_unit}"
-                    )
+
+            elif valuetype == DIMENSION and value and value != data:
+                options.append(
+                    f"{tikzname}="
+                    f"{self.round_value(self.convert_unit(value))}"
+                    f"{self.options.output_unit}"
+                )
 
         # Arrow marker handling
         options += self._handle_markers(style)
 
         # Dash-array
         options += self._handle_dasharray(style)
 
@@ -903,25 +916,28 @@
                     options.append(
                         "rotate around={"
                         + f"{ang}:{self.coord_to_tz(Vector2d(0.0, self.update_height(0)))}"
                         + "}"
                     )
                 else:
                     options.append(f"rotate={ang}")
+
             elif trans.is_scale():
                 x = self.round_value(trans.a)
                 y = self.round_value(trans.d)
 
+                if not self.options.noreversey and not is_node:
+                    options.append("shift={(0," + f"{y * self.update_height(0)}" + ")}")
+
                 if x == y:
                     options.append(f"scale={x}")
                 else:
                     options.append(f"xscale={x},yscale={y}")
 
             elif "matrix" in str(trans):
-                # print(trans)
                 tr = self.convert_unit_coord(Vector2d(trans.e, trans.f), False)
                 a = self.round_value(trans.a)
                 b = self.round_value(trans.b)
                 c = self.round_value(trans.c)
                 d = self.round_value(trans.d)
 
                 # globalscale do not impact transform
@@ -998,15 +1014,15 @@
         return s
 
     def _handle_switch(self, groupnode):
         """
         Convert a svg switch to tikzcode
         All the elements are returned for now
         """
-        options = self.trans_to_tz(groupnode)
+        options = self.style_to_tz(groupnode) + self.trans_to_tz(groupnode)
 
         old_indent = self.text_indent
 
         if len(options) > 0:
             self.text_indent += TEXT_INDENT
 
         group_id = groupnode.get_id()
@@ -1022,16 +1038,17 @@
             extra = f"%% {group_id}"
 
         hide = "none" in options
 
         s = ""
         if len(options) > 0 or self.options.verbose:
             # Remove it from the list
-            if hide or self.options.verbose:
+            if hide:
                 options.remove("none")
+                # TODO ID of foreignObject are not consistent
 
             pstyles = [",".join(options)]
 
             if "opacity" in pstyles[0]:
                 pstyles.append("transparency group")
 
             s += self.text_indent + "\\begin{scope}"
@@ -1115,35 +1132,42 @@
                 )
                 # Get acces to this vect2D ?
                 pos = Vector2d(command.x, command.y)
                 pos = self.convert_unit_coord(pos)
                 sweep = command.sweep
 
                 if not self.options.noreversey:
-                    sweep = 1 - sweep
-                    r.y *= -1
+                    current_pos.y = self.update_height(current_pos.y)
+                    pos.y = self.update_height(pos.y)
 
                 start_ang_o, end_ang_o, r = calc_arc(
                     current_pos,
                     r,
                     command.x_axis_rotation,
                     command.large_arc,
                     sweep,
                     pos,
                 )
+
                 r = self.round_coord(r)
+                if not self.options.noreversey:
+                    r.y *= -1
 
                 # pgf 2.0 does not like angles larger than 360
                 # make sure it is in the +- 360 range
                 start_ang = self.round_value(start_ang_o % 360)
                 end_ang = self.round_value(end_ang_o % 360)
-                if start_ang_o < end_ang_o and not start_ang < end_ang:
-                    start_ang -= 360
-                elif start_ang_o > end_ang_o and not start_ang > end_ang:
-                    end_ang -= 360
+                # # Does not to seem a problem anymore
+                # if start_ang_o < end_ang_o and not start_ang < end_ang:
+                # start_ang -= 360
+                # elif start_ang_o > end_ang_o and not start_ang > end_ang:
+                # end_ang -= 360
+
+                if not self.options.noreversey:
+                    command.x_axis_rotation *= -1
 
                 ang = self.round_value(command.x_axis_rotation)
                 if r.x == r.y:
                     # Todo: Transform radi
                     radi = f"{r.x}"
                 else:
                     radi = f"{r.x} and {r.y}"
@@ -1222,30 +1246,50 @@
                 return (
                     f"{self.coord_to_tz(center)} ellipse ({r.x}{self.options.output_unit} and {r.y}{self.options.output_unit})",
                     [],
                 )
 
         return "", []
 
+    def _find_attribute_in_hierarchy(self, current, attr):
+        """Try to find the attribute with the given name in the current node or any of its parents.
+        If the attribute is found, return its value, otherwise None."""
+        while current is not None:
+            value = current.get(attr)
+            if value:
+                return value
+            return self._find_attribute_in_hierarchy(current.getparent(), attr)
+
+        return None
+
     def _handle_text(self, node):
         if self.options.ignore_text:
-            return "", []
+            return ""
 
         raw_textstr = node.get_text(" ").strip()
-        if self.options.texmode == "raw":
+        mode = self.options.texmode
+
+        if mode == "attribute":
+            attribute = self._find_attribute_in_hierarchy(
+                node, self.options.texmode_attribute
+            )
+            if attribute:
+                mode = attribute
+
+        if mode == "raw":
             textstr = raw_textstr
-        elif self.options.texmode == "math":
+        elif mode == "math":
             textstr = f"${raw_textstr}$"
         else:
             textstr = escape_texchars(raw_textstr)
 
         shape = self.get_shape_inside(node)
         if shape is None:
             p = Vector2d(node.x, node.y)
-        else:
+        else:  # pragma: no cover
             # TODO Not working yet
             p = Vector2d(shape.left, shape.bottom)
 
         # We need to apply a rotation to coord
         # In tikz rotate only rotate the node, not its coordinate
         ang = 0.0
         trans = node.transform
@@ -1379,80 +1423,73 @@
 
         if len(nodes) == 0:
             nodes = root
 
         # Recursively process list of nodes or root node
         string = self._output_group(nodes)
 
-        options = []
         # Add necessary boiling plate code to the generated TikZ code.
         codeoutput = self.options.codeoutput
-        if len(options) > 0:
-            extraoptions = f",\n{','.join(options)}"
-        else:
-            extraoptions = ""
         if not self.options.crop:
             cropcode = ""
         else:
             cropcode = CROP_TEMPLATE
         if codeoutput == "standalone":
             output = STANDALONE_TEMPLATE % {
                 "pathcode": string,
                 "colorcode": self.color_code,
                 "unit": self.options.output_unit,
                 "ysign": "-" if self.options.noreversey else "",
                 "cropcode": cropcode,
-                "extraoptions": extraoptions,
                 "gradientcode": self.gradient_code,
                 "scale": self.options.scale,
             }
         elif codeoutput == "figonly":
             output = FIG_TEMPLATE % {
                 "pathcode": string,
                 "colorcode": self.color_code,
                 "unit": self.options.output_unit,
                 "ysign": "-" if self.options.noreversey else "",
-                "extraoptions": extraoptions,
                 "gradientcode": self.gradient_code,
                 "scale": self.options.scale,
             }
         else:
             output = string
 
         self.output_code = output
         if self.options.returnstring:
             return output
         return ""
 
     def save_raw(self, _):
         """Save the file from the save as menu from inkscape"""
-        if self.options.clipboard:
+        if self.options.clipboard:  # pragma: no cover
             success = copy_to_clipboard(self.output_code.encode("utf8"))
             if not success:
                 logging.error("Failed to put output on clipboard")
 
         elif self.options.output is not None:
             if isinstance(self.options.output, str):
                 with codecs.open(self.options.output, "w", "utf8") as stream:
                     stream.write(self.output_code)
             else:
                 out = self.output_code
 
-                if isinstance(self.options.output, io.BufferedWriter):
+                if isinstance(self.options.output, (io.BufferedWriter, io.FileIO)):
                     out = out.encode("utf8")
 
                 self.options.output.write(out)
 
     def run(self, args=None, output=SYS_OUTPUT_BUFFER):
         """
         Custom inkscape entry point to remove agr processing
         """
         try:
             # We parse it ourself in command line but letting it with inkscape
-            if not self.args_parsed:
+            if not self.args_parsed:  # pragma: no cover
                 if args is None:
                     args = sys.argv[1:]
 
                 self.parse_arguments(args)
 
             if (
                 isinstance(self.options.input_file, str)
@@ -1460,42 +1497,57 @@
             ):
                 os.environ["DOCUMENT_PATH"] = self.options.input_file
 
             if self.options.output is None:
                 self.options.output = output
             self.load_raw()
             self.save_raw(self.effect())
-        except inkex.utils.AbortExtension as err:
+        except inkex.utils.AbortExtension as err:  # pragma: no cover
             inkex.utils.errormsg(str(err))
             sys.exit(inkex.utils.ABORT_STATUS)
         finally:
             self.clean_up()
 
     def convert(self, svg_file=None, no_output=False, **kwargs):
         """Convert SVG file to tikz path"""
         self.options = self.arg_parser.parse_args()
         self.args_parsed = True
 
+        # Update args before everything else
+        self.options.__dict__.update(kwargs)
+
+        # Get version
         if self.options.printversion:
             print_version_info()
             return ""
 
+        # if attribute mode, texmode_attribute should not be None
+        if (
+            self.options.texmode == "attribute"
+            and self.options.texmode_attribute is None
+        ):
+            print("Need to specify a texmode attribute with --texmode-attribute")
+            return ""
+
+        # Updating input source
         if svg_file is not None:
             self.options.input_file = svg_file
 
-        self.options.__dict__.update(kwargs)
-
+        # If there is no file, end the code
         if self.options.input_file is None:
             print("No input file -- aborting")
             return ""
+
+        # Run the code
         if no_output:
             self.run(output=None)
         else:
             self.run()
 
+        # Return the output if necessary
         if self.options.returnstring:
             return self.output_code
         return ""
 
 
 def convert_file(svg_file, no_output=True, returnstring=True, **kwargs):
     """
@@ -1533,27 +1585,27 @@
     """
 
     kwargs["returnstring"] = returnstring
     effect = TikZPathExporter(inkscape_mode=False)
     return effect.convert(io.StringIO(svg_source), no_output, **kwargs)
 
 
-def main_inkscape():
+def main_inkscape():  # pragma: no cover
     """Inkscape interface"""
     # Create effect instance and apply it.
     effect = TikZPathExporter(inkscape_mode=True)
     effect.run()
 
 
 def print_version_info():
     """Print the version of svg2tikz"""
     print(f"svg2tikz version {__version__}")
 
 
-def main_cmdline(**kwargs):
+def main_cmdline(**kwargs):  # pragma: no cover
     """Main command line interface"""
     effect = TikZPathExporter(inkscape_mode=False)
     effect.convert(**kwargs)
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
     main_inkscape()
```

### Comparing `svg2tikz-3.0.1/svg2tikz/tikz_export_effect.inx` & `svg2tikz-3.1.0/svg2tikz/tikz_export_effect.inx`

 * *Files 4% similar despite different names*

#### Comparing `svg2tikz-3.0.1/svg2tikz/tikz_export_effect.inx` & `svg2tikz-3.1.0/svg2tikz/tikz_export_effect.inx`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <inkscape-extension>
-  <name>Export to TikZ path v3.0.1</name>
+  <name>Export to TikZ path v3.1.0</name>
   <id>net.texample.tools.svg.export_tikz.effect</id>
   <dependency type="executable" location="extensions">tikz_export.py</dependency>
   <param name="tab" type="notebook">
     <page name="options" gui-text="Document">
       <label appearance="header">Output file</label>
       <param name="output" type="path" mode="file_new" _gui-text="Output filename">none</param>
       <param name="clipboard" type="boolean" _gui-text="Export to clipboard">false</param>
@@ -36,15 +36,17 @@
     </page>
     <page name="Options" gui-text="Options">
       <label appearance="header">Text</label>
       <param name="texmode" type="optiongroup" gui-text="Text interpretation mode" gui-description="How should the text be interpreted">
         <option value="escape">Escape special TeX chars</option>
         <option value="raw">Raw TeX</option>
         <option value="math">Math</option>
+        <option value="attribute">Defined by attribute</option>
       </param>
+      <param name="texmode-attribute" type="string" gui-text="Texmode SVG attribute" gui-description="The text interpretation mode will be defined per SVG object by an attribute with this name."/>
       <param name="notext" type="boolean" gui-text="Ignore the text" gui-description="The text will not be included in the figure">false</param>
       <separator/>
       <label appearance="header" gui-description="How should the markers be interpreted">Markings</label>
       <param name="markings" type="optiongroup" gui-text="Marking interpretation mode">
         <option value="ignore">Not include markings</option>
         <option value="include">Not implemented</option>
         <option value="interpret">Custom interpertation</option>
```

### Comparing `svg2tikz-3.0.1/svg2tikz/tikz_export_output.inx` & `svg2tikz-3.1.0/svg2tikz/tikz_export_output.inx`

 * *Files 16% similar despite different names*

#### Comparing `svg2tikz-3.0.1/svg2tikz/tikz_export_output.inx` & `svg2tikz-3.1.0/svg2tikz/tikz_export_output.inx`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <inkscape-extension>
-  <name>Export as TikZ code for use with LaTeX v3.0.1</name>
+  <name>Export as TikZ code for use with LaTeX v3.1.0</name>
   <id>net.texample.tools.svg.export_tikz.output</id>
   <dependency type="executable" location="extensions">tikz_export.py</dependency>
   <param name="tab" type="notebook">
     <page name="options" gui-text="Document">
       <label appearance="header">Tikz option</label>
       <param name="codeoutput" type="optiongroup" gui-text="Tex template" gui-description="Template for the tikz code output">
         <option value="standalone">Stand alone</option>
@@ -32,15 +32,17 @@
     </page>
     <page name="Options" gui-text="Options">
       <label appearance="header">Text</label>
       <param name="texmode" type="optiongroup" gui-text="Text interpretation mode" gui-description="How should the text be interpreted">
         <option value="escape">Escape special TeX chars</option>
         <option value="raw">Raw TeX</option>
         <option value="math">Math</option>
+        <option value="attribute">Defined by attribute</option>
       </param>
+      <param name="texmode-attribute" type="string" gui-text="Texmode SVG attribute" gui-description="The text interpretation mode will be defined per SVG object by an attribute with this name."/>
       <param name="notext" type="boolean" gui-text="Ignore the text" gui-description="The text will not be included in the figure">false</param>
       <separator/>
       <label appearance="header" gui-description="How should the markers be interpreted">Markings</label>
       <param name="markings" type="optiongroup" gui-text="Marking interpretation mode">
         <option value="ignore">Not include markings</option>
         <option value="include">Not implemented</option>
         <option value="interpret">Custom interpertation</option>
```

### Comparing `svg2tikz-3.0.1/PKG-INFO` & `svg2tikz-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: svg2tikz
-Version: 3.0.1
+Version: 3.1.0
 Summary: Tools for converting SVG graphics to TikZ/PGF code
 License: GPL-2.0-or-later
 Author: ldevillez
 Author-email: louis.devillez@gmail.com
 Maintainer: ldevillez
 Maintainer-email: louis.devillez@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: inkex (>=1.2.2,<2.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 
 <picture>
   <img alt="SVG2TikZ Logo" src="logo/svg2tikz.svg">
 </picture>
 
 [![Documentation][documentation-badge]][documentation-url]
 [![PyPI version](https://badge.fury.io/py/svg2tikz.svg)](https://badge.fury.io/py/svg2tikz)
 
-# SVG2TikZ 3.0.X (Inkscape 1.x.x compatible)
+# SVG2TikZ 3.1.X (Inkscape 1.x.x compatible)
 
 
 SVG2TikZ, formally known as Inkscape2TikZ ,are a set of tools for converting SVG graphics to TikZ/PGF code.
 This project is licensed under the GNU GPL  (see  the [LICENSE](/LICENSE) file).
 
 ## Documentation and installation
 `SVG2TikZ` is now available on pypi so you can install it with if you want to use it with a command line. You can install the package with the following command:
```

