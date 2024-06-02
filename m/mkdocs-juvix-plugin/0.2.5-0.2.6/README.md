# Comparing `tmp/mkdocs-juvix-plugin-0.2.5.tar.gz` & `tmp/mkdocs-juvix-plugin-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-juvix-plugin-0.2.5.tar", last modified: Sun Jun  2 12:29:35 2024, max compression
+gzip compressed data, was "mkdocs-juvix-plugin-0.2.6.tar", last modified: Sun Jun  2 14:25:19 2024, max compression
```

## Comparing `mkdocs-juvix-plugin-0.2.5.tar` & `mkdocs-juvix-plugin-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-06-02 12:29:35.463801 mkdocs-juvix-plugin-0.2.5/
--rw-r--r--   0 jonaprieto   (501) staff       (20)      492 2024-06-02 12:29:35.463513 mkdocs-juvix-plugin-0.2.5/PKG-INFO
--rw-r--r--   0 jonaprieto   (501) staff       (20)     1882 2024-06-02 12:26:54.000000 mkdocs-juvix-plugin-0.2.5/README.md
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-06-02 12:29:35.461418 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/
--rw-r--r--   0 jonaprieto   (501) staff       (20)        0 2023-10-30 14:15:49.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/__init__.py
--rw-r--r--   0 jonaprieto   (501) staff       (20)    18558 2024-06-02 12:26:54.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/plugin.py
--rw-r--r--   0 jonaprieto   (501) staff       (20)     3364 2024-06-02 12:26:54.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/standalone.py
--rw-r--r--   0 jonaprieto   (501) staff       (20)     2438 2024-06-02 12:26:54.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/utils.py
-drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-06-02 12:29:35.463175 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/
--rw-r--r--   0 jonaprieto   (501) staff       (20)      492 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/PKG-INFO
--rw-r--r--   0 jonaprieto   (501) staff       (20)      375 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)        1 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)      107 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/entry_points.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       40 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/requires.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       13 2024-06-02 12:29:35.000000 mkdocs-juvix-plugin-0.2.5/mkdocs_juvix_plugin.egg-info/top_level.txt
--rw-r--r--   0 jonaprieto   (501) staff       (20)       38 2024-06-02 12:29:35.463856 mkdocs-juvix-plugin-0.2.5/setup.cfg
--rw-r--r--   0 jonaprieto   (501) staff       (20)      826 2024-06-02 12:29:06.000000 mkdocs-juvix-plugin-0.2.5/setup.py
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-06-02 14:25:19.335256 mkdocs-juvix-plugin-0.2.6/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      492 2024-06-02 14:25:19.335070 mkdocs-juvix-plugin-0.2.6/PKG-INFO
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     1882 2024-06-02 14:24:13.000000 mkdocs-juvix-plugin-0.2.6/README.md
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-06-02 14:25:19.334009 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)        0 2023-10-30 14:15:49.000000 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix/__init__.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)    18791 2024-06-02 14:22:46.000000 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix/plugin.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     3364 2024-06-02 12:26:54.000000 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix/standalone.py
+-rw-r--r--   0 jonaprieto   (501) staff       (20)     2438 2024-06-02 12:26:54.000000 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix/utils.py
+drwxr-xr-x   0 jonaprieto   (501) staff       (20)        0 2024-06-02 14:25:19.334890 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix_plugin.egg-info/
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      492 2024-06-02 14:25:19.000000 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      375 2024-06-02 14:25:19.000000 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)        1 2024-06-02 14:25:19.000000 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      107 2024-06-02 14:25:19.000000 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       40 2024-06-02 14:25:19.000000 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix_plugin.egg-info/requires.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       13 2024-06-02 14:25:19.000000 mkdocs-juvix-plugin-0.2.6/mkdocs_juvix_plugin.egg-info/top_level.txt
+-rw-r--r--   0 jonaprieto   (501) staff       (20)       38 2024-06-02 14:25:19.335300 mkdocs-juvix-plugin-0.2.6/setup.cfg
+-rw-r--r--   0 jonaprieto   (501) staff       (20)      826 2024-06-02 14:25:00.000000 mkdocs-juvix-plugin-0.2.6/setup.py
```

### Comparing `mkdocs-juvix-plugin-0.2.5/README.md` & `mkdocs-juvix-plugin-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/plugin.py` & `mkdocs-juvix-plugin-0.2.6/mkdocs_juvix/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import shutil
 import subprocess
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple
 from urllib.parse import urljoin
+from functools import wraps
 
 import pathspec
 from mkdocs.config import config_options as c
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import Files
 from mkdocs.structure.pages import Page
@@ -22,14 +23,25 @@
     fix_site_url,
     hash_file,
 )
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 
+def ifjuvix(func):
+    @wraps(func)
+    def wrapper(self, *args, **kwargs):
+        if getattr(self, "JUVIX_AVAILABLE", False):
+            return func(self, *args, **kwargs)
+        else:
+            return None
+
+    return wrapper
+
+
 class JuvixPlugin(BasePlugin):
 
     mkconfig: MkDocsConfig
     juvix_md_files: List[Dict[str, Any]]
 
     site_dir: Optional[str]
     site_url: str
@@ -75,73 +87,74 @@
 
         self.FIRST_RUN = True
 
         self.HASH_DIR = self.CACHE_DIR / ".HASH"
         self.HASH_DIR.mkdir(parents=True, exist_ok=True)
 
         self.JUVIX_AVAILABLE = shutil.which(self.JUVIX_BIN) is not None
+        if not self.JUVIX_AVAILABLE:
+            self.JUVIX_ENABLED = False
 
         if self.JUVIX_ENABLED:
-
-            if self.JUVIX_AVAILABLE:
-                cmd = [self.JUVIX_BIN, "--numeric-version"]
-                result = subprocess.run(cmd, capture_output=True)
-                if result.returncode == 0:
-                    JUVIX_VERSION = result.stdout.decode("utf-8")
-                    log.info(
-                        f"Using Juvix v{JUVIX_VERSION} to render Juvix Markdown files."
-                    )
-
             try:
                 subprocess.run([self.JUVIX_BIN, "--version"], capture_output=True)
             except FileNotFoundError:
                 log.warning(
                     "The Juvix binary is not available. Please install Juvix and make sure it's available in the PATH."
                 )
+            cmd = [self.JUVIX_BIN, "--numeric-version"]
+            result = subprocess.run(cmd, capture_output=True)
+            if result.returncode == 0:
+                JUVIX_VERSION = result.stdout.decode("utf-8")
+                log.info(
+                    f"Using Juvix v{JUVIX_VERSION} to render Juvix Markdown files."
+                )
 
         config = fix_site_url(config)
         self.mkconfig = config
 
         self.juvix_md_files: List[Dict[str, Any]] = []
 
         self.site_dir = config.get("site_dir", None)
         self.site_url = config.get("site_url", "")
 
-        if not self.JUVIX_ENABLED:
-            log.info("Juvix support is disabled. Set JUVIX_ENABLED to true to enable.")
-
         if not self.JUVIX_AVAILABLE:
             log.info(
                 "Juvix is not available on the system. check the JUVIX_BIN environment variable."
             )
 
         return config
 
+    @ifjuvix
     def on_files(self, files: Files, *, config: MkDocsConfig) -> Optional[Files]:
+        _files = []
         for file in files:
-            if ".juvix-build" in file.abs_src_path:
-                files.remove(file)
-        return files
+            if not (".juvix-build" in file.abs_src_path):
+                _files.append(file)
+        return Files(_files)
 
+    @ifjuvix
     def on_page_read_source(self, page: Page, config: MkDocsConfig) -> Optional[str]:
 
         filepath = Path(page.file.abs_src_path)
 
         if not filepath.as_posix().endswith(".juvix.md"):
             return None
 
         output = self.generate_markdown(filepath)
         if not output:
             log.error(f"Error generating markdown for file: {filepath}")
 
         return output
 
+    @ifjuvix
     def on_post_build(self, config: MkDocsConfig) -> None:
         self.generate_html(generate=False, move_cache=True)
 
+    @ifjuvix
     def on_serve(self, server: Any, config: MkDocsConfig, builder: Any) -> None:
 
         gitignore = None
 
         with open(self.ROOT_DIR / ".gitignore") as file:
             gitignore = pathspec.PathSpec.from_lines(
                 pathspec.patterns.GitWildMatchPattern, file  # type: ignore
@@ -174,34 +187,31 @@
                 if watch.path == config.docs_dir
             )
             .copy()
             .pop()
         )
         handler.on_any_event = callback_wrapper(handler.on_any_event)
 
+    @ifjuvix
     def on_page_markdown(
         self, markdown: str, page: Page, config: MkDocsConfig, files: Files
     ) -> Optional[str]:
         path = page.file.abs_src_path
 
         if not path.endswith(".juvix.md"):
             return markdown
 
         page.file.name = page.file.name.replace(".juvix", "")
         page.file.url = page.file.url.replace(".juvix", "")
         page.file.dest_uri = page.file.dest_uri.replace(".juvix", "")
         page.file.abs_dest_path = page.file.abs_dest_path.replace(".juvix", "")
 
-        # if "vscode" in page.file.src_path:
-        # print(page.file)
-
-        # exit()
-
         return markdown
 
+    @ifjuvix
     def move_html_cache_to_site_dir(self, filepath: Path, site_dir: Path) -> None:
 
         rel_to_docs = filepath.relative_to(self.DOCS_DIR)
         if filepath.is_dir():
             dest_folder = site_dir / rel_to_docs
         else:
             dest_folder = site_dir / rel_to_docs.parent
@@ -229,23 +239,25 @@
         if index_file.exists():
             index_file.unlink()
 
         # move the generated HTML files to the site directory
         shutil.copytree(self.HTML_CACHE_DIR, dest_folder, dirs_exist_ok=True)
         return
 
+    @ifjuvix
     def new_or_changed_or_no_exist(self, filepath: Path) -> bool:
         content_hash = hash_file(filepath)
         path_hash = compute_hash_filepath(filepath, hash_dir=self.HASH_DIR)
         if not path_hash.exists():
             log.debug(f"File: {filepath} does not have a hash file.")
             return True
         fresh_content_hash = path_hash.read_text()
         return content_hash != fresh_content_hash
 
+    @ifjuvix
     def on_pre_build(self, config: MkDocsConfig) -> None:
 
         if self.FIRST_RUN:
             try:
                 log.info("Updating Juvix dependencies...")
                 subprocess.run(
                     [self.JUVIX_BIN, "dependencies", "update"], capture_output=True
@@ -300,15 +312,14 @@
             self.JUVIX_ENABLED
             and self.JUVIX_AVAILABLE
             and (
                 not equal_hashes
                 or (
                     self.HTML_CACHE_DIR.exists()
                     and (len(list(self.HTML_CACHE_DIR.glob("*"))) == 0)
-                    #     )
                 )
             )
         )
 
         if not generate:
             log.info("Skipping Juvix HTML generation for Juvix files.")
         else:
@@ -411,14 +422,15 @@
 
     @lru_cache(maxsize=128)
     def read_cache(self, filepath: Path) -> Optional[str]:
         if cache_path := self.path_juvix_md_cache(filepath):
             return cache_path.read_text()
         return None
 
+    @ifjuvix
     def generate_markdown(self, filepath: Path) -> Optional[str]:
         if (
             not self.JUVIX_ENABLED
             or not self.JUVIX_AVAILABLE
             or not filepath.as_posix().endswith(".juvix.md")
         ):
             return None
@@ -426,20 +438,22 @@
         if self.new_or_changed_or_no_exist(filepath):
             log.info(f"Running Juvix Markdown on file: {filepath}")
             return self.run_juvix(filepath)
 
         log.debug(f"Reading cache for file: {filepath}")
         return self.read_cache(filepath)
 
+    @ifjuvix
     def unqualified_module_name(self, filepath: Path) -> Optional[str]:
         fposix: str = filepath.as_posix()
         if not fposix.endswith(".juvix.md"):
             return None
         return os.path.basename(fposix).replace(".juvix.md", "")
 
+    @ifjuvix
     def qualified_module_name(self, filepath: Path) -> Optional[str]:
         absolute_path = filepath.absolute()
         cmd = [self.JUVIX_BIN, "dev", "root", absolute_path.as_posix()]
         pp = subprocess.run(cmd, cwd=self.DOCS_DIR, capture_output=True)
         root = None
         try:
             root = pp.stdout.decode("utf-8").strip()
@@ -457,18 +471,20 @@
             .replace(".juvix.md", "")
             .replace("./", "")
             .replace("/", ".")
         )
 
         return qualified_name if qualified_name else None
 
+    @ifjuvix
     def md_filename(self, filepath: Path) -> Optional[str]:
         module_name = self.unqualified_module_name(filepath)
         return module_name + ".md" if module_name else None
 
+    @ifjuvix
     def run_juvix(self, _filepath: Path) -> Optional[str]:
 
         filepath = _filepath.absolute()
         fposix: str = filepath.as_posix()
 
         if not fposix.endswith(".juvix.md"):
             log.debug(f"The file: {fposix} is not a Juvix Markdown file.")
```

### Comparing `mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/standalone.py` & `mkdocs-juvix-plugin-0.2.6/mkdocs_juvix/standalone.py`

 * *Files identical despite different names*

### Comparing `mkdocs-juvix-plugin-0.2.5/mkdocs_juvix/utils.py` & `mkdocs-juvix-plugin-0.2.6/mkdocs_juvix/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs-juvix-plugin-0.2.5/setup.py` & `mkdocs-juvix-plugin-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="mkdocs-juvix-plugin",
-    version="0.2.5",
+    version="0.2.6",
     description="A plugin to render Juvix code blocks in MkDocs.",
     long_description="",
     keywords="mkdocs",
     author="Jonathan Prieto-Cubides, and GitHub contributors",
     author_email="jonathan@heliax.dev",
     license="MIT",
     python_requires=">=3.9",
```

