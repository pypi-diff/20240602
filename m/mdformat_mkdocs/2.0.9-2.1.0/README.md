# Comparing `tmp/mdformat_mkdocs-2.0.9.tar.gz` & `tmp/mdformat_mkdocs-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_mkdocs-2.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mdformat_mkdocs-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_mkdocs-2.0.9.tar` & `mdformat_mkdocs-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      600 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.copier-answers.yml
--rw-r--r--   0        0        0     1819 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.gitignore
--rw-r--r--   0        0        0     1592 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1085 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.pre-commit-test.yaml
--rw-r--r--   0        0        0     2882 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.ruff.toml
--rw-r--r--   0        0        0       21 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.tool-versions
--rw-r--r--   0        0        0      276 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.yamllint.yaml
--rw-r--r--   0        0        0     1366 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/LICENSE
--rw-r--r--   0        0        0     4366 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/README.md
--rw-r--r--   0        0        0      303 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/__init__.py
--rw-r--r--   0        0        0      914 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/_helpers.py
--rw-r--r--   0        0        0    11592 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/_normalize_list.py
--rw-r--r--   0        0        0     2416 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/_postprocess_inline.py
--rw-r--r--   0        0        0      317 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/__init__.py
--rw-r--r--   0        0        0     2368 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_content_tabs.py
--rw-r--r--   0        0        0     2843 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py
--rw-r--r--   0        0        0      785 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py
--rw-r--r--   0        0        0     3966 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/plugin.py
--rw-r--r--   0        0        0     1698 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/pyproject.toml
--rw-r--r--   0        0        0      895 2024-04-15 01:53:06.198283 mdformat_mkdocs-2.0.9/tox.ini
--rw-r--r--   0        0        0     6023 1970-01-01 00:00:00.000000 mdformat_mkdocs-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0      600 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/.copier-answers.yml
+-rw-r--r--   0        0        0     1819 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1592 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1085 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/.pre-commit-test.yaml
+-rw-r--r--   0        0        0     2882 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/.ruff.toml
+-rw-r--r--   0        0        0       21 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/.tool-versions
+-rw-r--r--   0        0        0      276 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/.yamllint.yaml
+-rw-r--r--   0        0        0     1366 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/LICENSE
+-rw-r--r--   0        0        0     5215 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/README.md
+-rw-r--r--   0        0        0      303 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/mdformat_mkdocs/__init__.py
+-rw-r--r--   0        0        0      914 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/mdformat_mkdocs/_helpers.py
+-rw-r--r--   0        0        0    12279 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/mdformat_mkdocs/_normalize_list.py
+-rw-r--r--   0        0        0     2436 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/mdformat_mkdocs/_postprocess_inline.py
+-rw-r--r--   0        0        0      403 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/mdformat_mkdocs/mdit_plugins/__init__.py
+-rw-r--r--   0        0        0     2367 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/mdformat_mkdocs/mdit_plugins/_content_tabs.py
+-rw-r--r--   0        0        0     2843 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py
+-rw-r--r--   0        0        0      785 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py
+-rw-r--r--   0        0        0     2772 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/mdformat_mkdocs/mdit_plugins/_pymd_abbreviations.py
+-rw-r--r--   0        0        0     6210 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/mdformat_mkdocs/plugin.py
+-rw-r--r--   0        0        0     1762 2024-06-02 15:09:31.512153 mdformat_mkdocs-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      895 2024-06-02 15:09:31.516153 mdformat_mkdocs-2.1.0/tox.ini
+-rw-r--r--   0        0        0     6872 1970-01-01 00:00:00.000000 mdformat_mkdocs-2.1.0/PKG-INFO
```

### Comparing `mdformat_mkdocs-2.0.9/.copier-answers.yml` & `mdformat_mkdocs-2.1.0/.copier-answers.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # yamllint disable-file
 # Answer file maintained by Copier for: https://github.com/KyleKing/mdformat-plugin-template
 # DO NOT MODIFY THIS FILE. Edit by re-running copier and changing responses to the questions
 # Check into version control.
-_commit: 0.1.4
+_commit: 0.1.5
 _src_path: gh:KyleKing/mdformat-plugin-template
 author_email: dev.act.kyle@gmail.com
 author_name: Kyle King
 author_username: kyleking
 copyright_date: '2024'
 package_name_kebab: mdformat-mkdocs
 plugin_name: mkdocs
```

### Comparing `mdformat_mkdocs-2.0.9/.gitignore` & `mdformat_mkdocs-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.9/.pre-commit-config.yaml` & `mdformat_mkdocs-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.9/.pre-commit-test.yaml` & `mdformat_mkdocs-2.1.0/.pre-commit-test.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.9/.ruff.toml` & `mdformat_mkdocs-2.1.0/.ruff.toml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.9/CONTRIBUTING.md` & `mdformat_mkdocs-2.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.9/LICENSE` & `mdformat_mkdocs-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.9/README.md` & `mdformat_mkdocs-2.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -7,28 +7,32 @@
 [cov-link]: https://codecov.io/gh/executablebooks/mdformat-mkdocs
  -->
 
 An [mdformat](https://github.com/executablebooks/mdformat) plugin for [mkdocs](https://github.com/mkdocs/mkdocs) and [mkdocs-material](https://squidfunk.github.io/mkdocs-material) in particular.
 
 Supports:
 
-- Indents are converted to 4-spaces instead of 2
-    - *Note*: see caveats when using the optional Semantic Indents on numbered lists which may not be a full multiple of 4
-- List bullets are converted to dashes instead of `*`
-- Admonitions (extends [`mdformat-admon`](https://pypi.org/project/mdformat-admon))
-- MKDocs-Material Content Tabs (<https://squidfunk.github.io/mkdocs-material/reference/content-tabs>)
-    - Note: the markup (HTML) rendered by this plugin is sufficient for formatting but not for viewing in a browser. Please open an issue if you have a need to generate valid HTML.
+- Indents are converted to four-spaces instead of two
+    - *Note*: when specifying `--align-semantic-breaks-in-lists`, the nested indent for ordered lists is three, but is otherwise a multiple of four
+- Unordered list bullets are converted to dashes (`-`) instead of `*`
+- By default, ordered lists are standardized on a single digit (`1.` or `0.`) unless `--number` is specified, then `mdformat-mkdocs` will apply consecutive numbering to ordered lists [for consistency with `mdformat`](https://github.com/executablebooks/mdformat?tab=readme-ov-file#options)
+- [MkDocs-Material Admonitions](https://squidfunk.github.io/mkdocs-material/reference/admonitions)
+- [MkDocs-Material "Content Tabs"\*](https://squidfunk.github.io/mkdocs-material/reference/content-tabs)
+    - \*Note: the markup (HTML) rendered by this plugin is sufficient for formatting but not for viewing in a browser. Please open an issue if you have a need to generate valid HTML.
+- [Python Markdown "Abbreviations"\*](https://squidfunk.github.io/mkdocs-material/reference/tooltips/#adding-abbreviations)
+    - \*Note: the markup (HTML) rendered for abbreviations is not useful for rendering. If important, I'm open to contributions because this is an involved implementation
+- "[Markdown anchors](https://mkdocstrings.github.io/autorefs/#markdown-anchors)" syntax from the `mkdocs` [autorefs](https://mkdocstrings.github.io/autorefs) plugin
 
 See the example test files, [./tests/pre-commit-test.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/pre-commit-test.md) and [./tests/format/fixtures.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/format/fixtures.md)
 
 ## `mdformat` Usage
 
 Add this package wherever you use `mdformat` and the plugin will be auto-recognized. No additional configuration necessary. For additional information on plugins, see [the official `mdformat` documentation here](https://mdformat.readthedocs.io/en/stable/users/plugins.html)
 
-**Tip**: this package specifies an "extra" (`'recommended'`) for plugins that work well with `mkdocs`:
+**Tip**: this package specifies an "extra" (`'recommended'`) for plugins that work well with typical documentation managed by `mkdocs`:
 
 - [mdformat-beautysh](https://pypi.org/project/mdformat-beautysh)
 - [mdformat-black](https://pypi.org/project/mdformat-black)
 - [mdformat-config](https://pypi.org/project/mdformat-config)
 - [mdformat-footnote](https://pypi.org/project/mdformat-footnote)
 - [mdformat-frontmatter](https://pypi.org/project/mdformat-frontmatter)
 - [mdformat-simple-breaks](https://pypi.org/project/mdformat-simple-breaks)
@@ -41,17 +45,17 @@
 ```yaml
 repos:
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
         additional_dependencies:
-          - mdformat-mkdocs>=2.0.0
+          - mdformat-mkdocs>=2.1.0
           # Or
-          # - "mdformat-mkdocs[recommended]>=2.0.6"
+          # - "mdformat-mkdocs[recommended]>=2.1.0"
 ```
 
 ### pipx
 
 ```sh
 pipx install mdformat
 pipx inject mdformat mdformat-mkdocs
```

### Comparing `mdformat_mkdocs-2.0.9/mdformat_mkdocs/_helpers.py` & `mdformat_mkdocs-2.1.0/mdformat_mkdocs/_helpers.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.9/mdformat_mkdocs/_normalize_list.py` & `mdformat_mkdocs-2.1.0/mdformat_mkdocs/_normalize_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     LIST_NUMBERED = "LIST_NUMBERED"
     START_MARKED = "START_MARKED"
     EDGE_CODE = "EDGE_CODE"
     HTML = "HTML"
 
     @classmethod
     def from_content(cls, content: str) -> Syntax | None:
+        """Determine Syntax type from string."""
         if match := RE_LIST_ITEM.fullmatch(content):
             return (
                 cls.LIST_NUMBERED
                 if match["bullet"] not in {"-", "*"}
                 else cls.LIST_BULLETED
             )
         if any(content.startswith(f"{marker} ") for marker in MARKERS):
@@ -91,29 +92,32 @@
 
     parsed: ParsedLine
     parents: list[ParsedLine]
     prev_list_peers: list[ParsedLine]  # Only applicable for lists
 
 
 def is_parent_line(prev_line: LineResult, parsed: ParsedLine) -> bool:
+    """Returns true if previous line has content and a lower indent (e.g. parent)."""
     return bool(prev_line.parsed.content) and len(parsed.indent) > len(
         prev_line.parsed.indent,
     )
 
 
 def is_peer_list_line(prev_line: LineResult, parsed: ParsedLine) -> bool:
+    """Returns True if two list items share the same scope and level."""
     list_types = {Syntax.LIST_BULLETED, Syntax.LIST_NUMBERED}
     return (
         parsed.syntax in list_types
         and prev_line.parsed.syntax in list_types
         and len(parsed.indent) == len(prev_line.parsed.indent)
     )
 
 
 def parse_line(line_num: int, content: str) -> ParsedLine:
+    """Create summary object separating line from content."""
     indent, content = separate_indent(content)
     syntax = Syntax.from_content(content)
     return ParsedLine(
         line_num=line_num,
         indent=indent,
         content=content,
         syntax=syntax,
@@ -172,14 +176,15 @@
 
     raw_indent: str
     indent_depth: int
     kind: Literal["code", "HTML"]
 
 
 def parse_code_block(last: BlockIndent | None, line: LineResult) -> BlockIndent | None:
+    """Identify fenced or indented sections internally referred to as 'code blocks.'"""
     result = last
     if line.parsed.syntax == Syntax.EDGE_CODE:
         # On first edge, start tracking a code block
         #   on the second edge, stop tracking
         result = (
             None
             if last
@@ -189,14 +194,15 @@
                 kind="code",
             )
         )
     return result
 
 
 def parse_html_line(last: BlockIndent | None, line: LineResult) -> BlockIndent | None:
+    """Identify sections of HTML."""
     result = last
     if line.parsed.syntax == Syntax.HTML:
         # Start tracking an HTML block if not already
         result = last or BlockIndent(
             raw_indent=line.parsed.indent,
             indent_depth=len(line.parents),
             kind="HTML",
@@ -211,14 +217,15 @@
 # High-Level Accumulators
 
 DEFAULT_INDENT = " " * MKDOCS_INDENT_COUNT
 """Default indent."""
 
 
 def format_new_indent(line: LineResult, block_indent: BlockIndent | None) -> str:
+    """Normalize the list indent."""
     result = ""
     if line.parsed.content:
         if block_indent:
             depth = block_indent.indent_depth
             extra_indent = get_inner_indent(
                 block_indent=block_indent,
                 line_indent=line.parsed.indent,
@@ -235,24 +242,29 @@
     lines: list[LineResult]
     new_lines: list[tuple[str, str]]
     # Used only for debugging purposes
     debug_block_indents: list[BlockIndent | None]
 
 
 def format_new_content(line: LineResult, inc_numbers: bool, is_code: bool) -> str:
+    """Normalize the list bullet or number."""
     new_content = line.parsed.content
     if not is_code and line.parsed.syntax in {
         Syntax.LIST_BULLETED,
         Syntax.LIST_NUMBERED,
     }:
         list_match = RE_LIST_ITEM.fullmatch(line.parsed.content)
         assert list_match is not None  # for pyright # noqa: S101
         new_bullet = "-"
         if line.parsed.syntax == Syntax.LIST_NUMBERED:
-            counter = len(line.prev_list_peers) + 1 if inc_numbers else 1
+            first_peer = (
+                line.prev_list_peers[-1] if line.prev_list_peers else line.parsed
+            )
+            base_num = 0 if first_peer.content.startswith("0.") else 1
+            counter = len(line.prev_list_peers) + base_num if inc_numbers else base_num
             new_bullet = f"{counter}."
         new_content = f'{new_bullet} {list_match["item"]}'
 
     return new_content
 
 
 def parse_text(text: str, inc_numbers: bool) -> ParsedText:
```

### Comparing `mdformat_mkdocs-2.0.9/mdformat_mkdocs/_postprocess_inline.py` & `mdformat_mkdocs-2.1.0/mdformat_mkdocs/_postprocess_inline.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,27 @@
 from ._helpers import FILLER_CHAR, MKDOCS_INDENT_COUNT, rstrip_result
 
 FILLER = FILLER_CHAR * (MKDOCS_INDENT_COUNT - 2)  # `mdformat` default is two spaces
 """A spacer that is inserted and then removed to ensure proper word wrap."""
 
 
 @rstrip_result
-def postprocess_inline(text: str, node: RenderTreeNode, context: RenderContext) -> str:
+def postprocess_list_wrap(
+    text: str,
+    node: RenderTreeNode,
+    context: RenderContext,
+) -> str:
     """Postprocess inline tokens.
 
     Fix word wrap for lists to account for the change in indentation.
     We fool word wrap by prefixing an unwrappable dummy string of the same length.
-    This prefix needs to be later removed (in `_list_item_renderer`).
+    This prefix needs to be later removed (in `merge_parsed_text`).
 
-    Adapted from: https://github.com/hukkin/mdformat-gfm/blob/cf316a121b6cf35cbff7b0ad6e171f287803f8cb/src/mdformat_gfm/plugin.py#L86-L111
+    Adapted from:
+    https://github.com/hukkin/mdformat-gfm/blob/cf316a121b6cf35cbff7b0ad6e171f287803f8cb/src/mdformat_gfm/plugin.py#L86-L111
 
     """
     if not context.do_wrap:
         return text
     wrap_mode = context.options["mdformat"]["wrap"]
     if (
         not isinstance(wrap_mode, int)  # noqa: PLR0916
```

### Comparing `mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_content_tabs.py` & `mdformat_mkdocs-2.1.0/mdformat_mkdocs/mdit_plugins/_content_tabs.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def format_content_tab_markup(
     state: StateBlock,
     start_line: int,
     admonition: AdmonitionData,
 ) -> None:
-    """WARNING: this is not the proper markup for MKDocs.
+    """WARNING: this is not the proper markup for MkDocs.
 
     Would require recursively calling the parser to identify all sequential
     content tabs
 
     """
     title = admonition.meta_text.strip().strip("'\"")
 
@@ -54,15 +54,15 @@
     state: StateBlock,
     startLine: int,
     endLine: int,
     silent: bool,
 ) -> bool:
     # Because content-tabs look like admonitions syntactically, we can
     #   reuse admonition parsing logic
-    # Supported variations from: https://facelessuser.github.io/pymdown-extensions/extensions/tabbed/
+    # Supported variations from: https://facelessuser.github.io/pymdown-extensions/extensions/tabbed
     parse_possible_whitespace_admon = parse_possible_whitespace_admon_factory(
         markers=CONTENT_TAB_MARKERS,
     )
     result = parse_possible_whitespace_admon(state, startLine, endLine, silent)
     if isinstance(result, AdmonitionData):
         format_content_tab_markup(state, startLine, admonition=result)
         return True
```

### Comparing `mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py` & `mdformat_mkdocs-2.1.0/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""MKDocs Admonition Plugin."""
+"""MkDocs Admonition Plugin."""
 
 from __future__ import annotations
 
 from typing import Any
 
 from markdown_it.rules_block import StateBlock
 from mdformat_admon.factories import (
@@ -14,15 +14,15 @@
 )
 from mdformat_admon.mdit_plugins import format_python_markdown_admon_markup
 
 PREFIX = "admonition_mkdocs"
 """Prefix used to differentiate the parsed output."""
 
 MKDOCS_ADMON_MARKERS = {"!!!", "???", "???+"}
-"""All supported MKDocs Admonition markers."""
+"""All supported MkDocs Admonition markers."""
 
 
 def format_admon_markup(
     state: StateBlock,
     start_line: int,
     admonition: AdmonitionData,
 ) -> None:
@@ -66,15 +66,15 @@
 
 def admonition_logic(
     state: StateBlock,
     startLine: int,
     endLine: int,
     silent: bool,
 ) -> bool:
-    """Parse MKDocs-style Admonitions.
+    """Parse MkDocs-style Admonitions.
 
     `Such as collapsible blocks
     <https://squidfunk.github.io/mkdocs-material/reference/admonitions/#collapsible-blocks>`.
 
     .. code-block:: md
 
         ???+ note
```

### Comparing `mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py` & `mdformat_mkdocs-2.1.0/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.9/pyproject.toml` & `mdformat_mkdocs-2.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 dynamic = ["description", "version"]
 keywords = ["markdown", "markdown-it", "mdformat"]
 name = "mdformat_mkdocs"
 readme = "README.md"
 requires-python = ">=3.8.0"
 
 [project.entry-points."mdformat.parser_extension"]
-mkdocs = "mdformat_mkdocs"
+mkdocs = "mdformat_mkdocs" # Do not change name without modifying '_match_plugin_renderer'
 
 [project.optional-dependencies]
 dev = ["pre-commit"]
 recommended = [
   # Keep in-sync with README
   "mdformat-beautysh >= 0.1.1",
   "mdformat-config >= 0.1.3",
```

### Comparing `mdformat_mkdocs-2.0.9/tox.ini` & `mdformat_mkdocs-2.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.9/PKG-INFO` & `mdformat_mkdocs-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdformat_mkdocs
-Version: 2.0.9
+Version: 2.1.0
 Summary: An mdformat plugin for mkdocs.
 Keywords: markdown,markdown-it,mdformat
 Author-email: kyleking <dev.act.kyle@gmail.com>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -43,28 +43,32 @@
 [cov-link]: https://codecov.io/gh/executablebooks/mdformat-mkdocs
  -->
 
 An [mdformat](https://github.com/executablebooks/mdformat) plugin for [mkdocs](https://github.com/mkdocs/mkdocs) and [mkdocs-material](https://squidfunk.github.io/mkdocs-material) in particular.
 
 Supports:
 
-- Indents are converted to 4-spaces instead of 2
-    - *Note*: see caveats when using the optional Semantic Indents on numbered lists which may not be a full multiple of 4
-- List bullets are converted to dashes instead of `*`
-- Admonitions (extends [`mdformat-admon`](https://pypi.org/project/mdformat-admon))
-- MKDocs-Material Content Tabs (<https://squidfunk.github.io/mkdocs-material/reference/content-tabs>)
-    - Note: the markup (HTML) rendered by this plugin is sufficient for formatting but not for viewing in a browser. Please open an issue if you have a need to generate valid HTML.
+- Indents are converted to four-spaces instead of two
+    - *Note*: when specifying `--align-semantic-breaks-in-lists`, the nested indent for ordered lists is three, but is otherwise a multiple of four
+- Unordered list bullets are converted to dashes (`-`) instead of `*`
+- By default, ordered lists are standardized on a single digit (`1.` or `0.`) unless `--number` is specified, then `mdformat-mkdocs` will apply consecutive numbering to ordered lists [for consistency with `mdformat`](https://github.com/executablebooks/mdformat?tab=readme-ov-file#options)
+- [MkDocs-Material Admonitions](https://squidfunk.github.io/mkdocs-material/reference/admonitions)
+- [MkDocs-Material "Content Tabs"\*](https://squidfunk.github.io/mkdocs-material/reference/content-tabs)
+    - \*Note: the markup (HTML) rendered by this plugin is sufficient for formatting but not for viewing in a browser. Please open an issue if you have a need to generate valid HTML.
+- [Python Markdown "Abbreviations"\*](https://squidfunk.github.io/mkdocs-material/reference/tooltips/#adding-abbreviations)
+    - \*Note: the markup (HTML) rendered for abbreviations is not useful for rendering. If important, I'm open to contributions because this is an involved implementation
+- "[Markdown anchors](https://mkdocstrings.github.io/autorefs/#markdown-anchors)" syntax from the `mkdocs` [autorefs](https://mkdocstrings.github.io/autorefs) plugin
 
 See the example test files, [./tests/pre-commit-test.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/pre-commit-test.md) and [./tests/format/fixtures.md](https://raw.githubusercontent.com/KyleKing/mdformat-mkdocs/main/tests/format/fixtures.md)
 
 ## `mdformat` Usage
 
 Add this package wherever you use `mdformat` and the plugin will be auto-recognized. No additional configuration necessary. For additional information on plugins, see [the official `mdformat` documentation here](https://mdformat.readthedocs.io/en/stable/users/plugins.html)
 
-**Tip**: this package specifies an "extra" (`'recommended'`) for plugins that work well with `mkdocs`:
+**Tip**: this package specifies an "extra" (`'recommended'`) for plugins that work well with typical documentation managed by `mkdocs`:
 
 - [mdformat-beautysh](https://pypi.org/project/mdformat-beautysh)
 - [mdformat-black](https://pypi.org/project/mdformat-black)
 - [mdformat-config](https://pypi.org/project/mdformat-config)
 - [mdformat-footnote](https://pypi.org/project/mdformat-footnote)
 - [mdformat-frontmatter](https://pypi.org/project/mdformat-frontmatter)
 - [mdformat-simple-breaks](https://pypi.org/project/mdformat-simple-breaks)
@@ -77,17 +81,17 @@
 ```yaml
 repos:
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
         additional_dependencies:
-          - mdformat-mkdocs>=2.0.0
+          - mdformat-mkdocs>=2.1.0
           # Or
-          # - "mdformat-mkdocs[recommended]>=2.0.6"
+          # - "mdformat-mkdocs[recommended]>=2.1.0"
 ```
 
 ### pipx
 
 ```sh
 pipx install mdformat
 pipx inject mdformat mdformat-mkdocs
```

