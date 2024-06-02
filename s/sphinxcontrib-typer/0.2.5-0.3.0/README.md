# Comparing `tmp/sphinxcontrib_typer-0.2.5.tar.gz` & `tmp/sphinxcontrib_typer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_typer-0.2.5.tar", max compression
+gzip compressed data, was "sphinxcontrib_typer-0.3.0.tar", max compression
```

## Comparing `sphinxcontrib_typer-0.2.5.tar` & `sphinxcontrib_typer-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2024-04-03 19:52:41.798588 sphinxcontrib_typer-0.2.5/LICENSE
--rw-r--r--   0        0        0     5323 2024-05-29 23:45:18.623298 sphinxcontrib_typer-0.2.5/README.md
--rw-r--r--   0        0        0     2914 2024-05-30 00:00:32.240407 sphinxcontrib_typer-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    34769 2024-05-30 00:00:26.706461 sphinxcontrib_typer-0.2.5/sphinxcontrib/typer/__init__.py
--rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-12-14 00:10:27.893967 sphinxcontrib_typer-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5323 2024-06-02 01:23:17.381811 sphinxcontrib_typer-0.3.0/README.md
+-rw-r--r--   0        0        0     2914 2024-06-02 05:02:44.871357 sphinxcontrib_typer-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    35009 2024-06-02 06:40:40.020361 sphinxcontrib_typer-0.3.0/sphinxcontrib/typer/__init__.py
+-rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.3.0/PKG-INFO
```

### Comparing `sphinxcontrib_typer-0.2.5/LICENSE` & `sphinxcontrib_typer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_typer-0.2.5/README.md` & `sphinxcontrib_typer-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_typer-0.2.5/pyproject.toml` & `sphinxcontrib_typer-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxcontrib-typer"
-version = "0.2.5"
+version = "0.3.0"
 description = "Auto generate docs for typer commands."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sphinx-contrib/typer"
 homepage = "https://sphinxcontrib-typer.readthedocs.io"
 classifiers = [
```

### Comparing `sphinxcontrib_typer-0.2.5/sphinxcontrib/typer/__init__.py` & `sphinxcontrib_typer-0.3.0/sphinxcontrib/typer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,27 +44,35 @@
 from sphinx.util import logging
 
 from typer import rich_utils as typer_rich_utils
 from typer.main import Typer, TyperGroup, TyperInfo
 from typer.main import get_command as get_typer_command
 from typer.models import Context as TyperContext
 
-VERSION = (0, 2, 5)
+VERSION = (0, 3, 0)
 
 __title__ = "SphinxContrib Typer"
 __version__ = ".".join(str(i) for i in VERSION)
 __author__ = "Brian Kohan"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Brian Kohan"
 
 
 SELENIUM_DEFAULT_WINDOW_WIDTH = 1920
 SELENIUM_DEFAULT_WINDOW_HEIGHT = 2048
 
 
+def get_function(function: t.Union[str, t.Callable[..., t.Any]]):
+    if callable(function):
+        return function
+    if isinstance(function, str):
+        parts = function.split(".")
+        return getattr(import_module(".".join(parts[0:-1])), parts[-1])
+
+
 def _filter_commands(ctx: click.Context, cmd_filter: t.Optional[t.List[str]] = None):
     return sorted(
         [
             cmd
             for name, cmd in getattr(
                 ctx.command,
                 "commands",
@@ -477,34 +485,38 @@
             **export_options,
         )
 
         if self.typer_convert_png:
             png_path = Path(self.env.app.builder.outdir) / (
                 f'{normal_cmd.replace(":", "_")}_{self.uuid(normal_cmd)}.png'
             )
-            self.env.app.config.typer_convert_png(self, rendered, png_path)
+            get_function(self.env.app.config.typer_convert_png)(
+                self, rendered, png_path
+            )
             section += nodes.image(
                 uri=os.path.relpath(png_path, Path(self.env.srcdir)),
                 alt=source_name,
             )
         elif self.target == RenderTarget.HTML:
             section += nodes.raw(
                 "",
-                self.env.app.config.typer_render_html(self, normal_cmd, rendered),
+                get_function(self.env.app.config.typer_render_html)(
+                    self, normal_cmd, rendered
+                ),
                 format="html",
             )
         elif self.target == RenderTarget.SVG:
             if "html" in self.builder:
                 section += nodes.raw("", rendered, format="html")
             else:
                 img_name = f'{normal_cmd.replace(":", "_")}_{self.uuid(normal_cmd)}'
                 out_dir = Path(self.env.app.builder.outdir)
                 (out_dir / f"{img_name}.svg").write_text(rendered)
                 pdf_img = out_dir / f"{img_name}.pdf"
-                self.env.app.config.typer_svg2pdf(self, rendered, pdf_img)
+                get_function(self.env.app.config.typer_svg2pdf)(self, rendered, pdf_img)
                 section += nodes.image(
                     uri=os.path.relpath(pdf_img, Path(self.env.srcdir)),
                     alt=source_name,
                 )
 
         elif self.target == RenderTarget.TEXT:
             section += nodes.literal_block("", rendered)
@@ -633,15 +645,17 @@
     if cache_path and cache_path.is_file():
         cache = json.loads(cache_path.read_text())
         cache.setdefault("iframe_heights", {})
 
     if cache["iframe_heights"].get(normal_cmd):
         return cache["iframe_heights"][normal_cmd]
 
-    with directive.env.app.config.typer_get_web_driver(directive) as driver:
+    with get_function(directive.env.app.config.typer_get_web_driver)(
+        directive
+    ) as driver:
         # use base64 to avoid issues with special characters
         driver.get(
             f'data:text/html;base64,'
             f'{base64.b64encode(html_page.encode("utf-8")).decode()}'
         )
         height = (
             int(
@@ -667,15 +681,15 @@
 
     :param directive: The TyperDirective instance
     :param normal_cmd: The normalized name of the command.
         (Subcommands are delimited by :)
     :param html_page: The html page rendered by console.export_html
     """
 
-    height = directive.env.app.config.typer_get_iframe_height(
+    height = get_function(directive.env.app.config.typer_get_iframe_height)(
         directive, normal_cmd, html_page
     )
     return (
         f'<iframe style="border: none;" width="100%" height="'
         f'{height}px"'
         f' srcdoc="{html_escape(html_page)}"></iframe>'
     )
@@ -831,15 +845,17 @@
     import tempfile
     from io import BytesIO
 
     from PIL import Image
     from selenium.webdriver.common.by import By
 
     tag = "code"
-    with directive.env.app.config.typer_get_web_driver(directive) as driver:
+    with get_function(directive.env.app.config.typer_get_web_driver)(
+        directive
+    ) as driver:
         with tempfile.NamedTemporaryFile(suffix=".html") as tmp:
             if directive.target is RenderTarget.TEXT:
                 tag = "pre"
                 rendered = f"<html><body><pre>{rendered}</pre></body></html>"
             elif directive.target is RenderTarget.SVG:
                 tag = "svg"
                 rendered = f"<html><body>{rendered}</body></html>"
@@ -895,40 +911,33 @@
             im.save(str(png_path))  # Saves the screenshot
 
 
 def setup(app: application.Sphinx) -> t.Dict[str, t.Any]:
     # Need autodoc to support mocking modules
     app.add_directive("typer", TyperDirective)
 
-    def get_default_render_html(_):
-        return typer_render_html
-
-    def get_default_get_iframe_height(_):
-        return typer_get_iframe_height
-
-    def get_default_svg2pdf(_):
-        return typer_svg2pdf
-
-    def get_default_convert_png(_):
-        return typer_convert_png
-
-    def get_default_web_driver(_):
-        return typer_get_web_driver
-
-    app.add_config_value("typer_render_html", get_default_render_html, "")
+    app.add_config_value(
+        "typer_render_html", "sphinxcontrib.typer.typer_render_html", "env"
+    )
 
-    app.add_config_value("typer_get_iframe_height", get_default_get_iframe_height, "")
-    app.add_config_value("typer_svg2pdf", get_default_svg2pdf, "")
+    app.add_config_value(
+        "typer_get_iframe_height", "sphinxcontrib.typer.typer_get_iframe_height", "env"
+    )
+    app.add_config_value("typer_svg2pdf", "sphinxcontrib.typer.typer_svg2pdf", "env")
     app.add_config_value("typer_iframe_height_padding", 30, "env")
     app.add_config_value(
         "typer_iframe_height_cache_path",
         Path(app.confdir) / "typer_cache.json",
         "env",
     )
 
-    app.add_config_value("typer_convert_png", get_default_convert_png, "")
-    app.add_config_value("typer_get_web_driver", get_default_web_driver, "")
+    app.add_config_value(
+        "typer_convert_png", "sphinxcontrib.typer.typer_convert_png", "env"
+    )
+    app.add_config_value(
+        "typer_get_web_driver", "sphinxcontrib.typer.typer_get_web_driver", "env"
+    )
 
     return {
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `sphinxcontrib_typer-0.2.5/PKG-INFO` & `sphinxcontrib_typer-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-typer
-Version: 0.2.5
+Version: 0.3.0
 Summary: Auto generate docs for typer commands.
 Home-page: https://sphinxcontrib-typer.readthedocs.io
 License: MIT
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

