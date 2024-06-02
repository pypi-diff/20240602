# Comparing `tmp/dahlia-2.3.2.tar.gz` & `tmp/dahlia-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dahlia-2.3.2.tar", max compression
+gzip compressed data, was "dahlia-3.0.0.tar", max compression
```

## Comparing `dahlia-2.3.2.tar` & `dahlia-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-01-19 17:08:30.010799 dahlia-2.3.2/LICENSE
--rw-r--r--   0        0        0     1184 2023-03-14 06:05:32.029103 dahlia-2.3.2/README.md
--rw-r--r--   0        0        0      611 2023-04-19 05:04:29.369420 dahlia-2.3.2/pyproject.toml
--rw-r--r--   0        0        0      265 2023-02-16 08:21:44.627720 dahlia-2.3.2/src/dahlia/__init__.py
--rw-r--r--   0        0        0     1097 2023-04-19 05:04:35.327748 dahlia-2.3.2/src/dahlia/__main__.py
--rw-r--r--   0        0        0     2993 2023-03-20 21:45:40.260197 dahlia-2.3.2/src/dahlia/constants.py
--rw-r--r--   0        0        0     6044 2023-04-19 05:02:44.556635 dahlia-2.3.2/src/dahlia/dahlia.py
--rw-r--r--   0        0        0     2056 2023-01-19 17:08:30.457820 dahlia-2.3.2/src/dahlia/legacy.py
--rw-r--r--   0        0        0        1 2023-01-19 17:08:30.499731 dahlia-2.3.2/src/dahlia/py.typed
--rw-r--r--   0        0        0     6574 2023-03-07 00:59:51.246219 dahlia-2.3.2/src/dahlia/utils.py
--rw-r--r--   0        0        0     1919 1970-01-01 00:00:00.000000 dahlia-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-29 10:24:32.406427 dahlia-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1611 2024-06-02 18:34:50.908954 dahlia-3.0.0/README.md
+-rw-r--r--   0        0        0      153 2024-05-24 15:36:23.647461 dahlia-3.0.0/dahlia/__init__.py
+-rw-r--r--   0        0        0      491 2024-06-02 18:34:50.909350 dahlia-3.0.0/dahlia/__main__.py
+-rw-r--r--   0        0        0     2276 2024-05-25 16:19:23.950199 dahlia-3.0.0/dahlia/constants.py
+-rw-r--r--   0        0        0     4629 2024-05-25 17:31:25.529957 dahlia-3.0.0/dahlia/lib.py
+-rw-r--r--   0        0        0        1 2024-05-20 20:10:28.359501 dahlia-3.0.0/dahlia/py.typed
+-rw-r--r--   0        0        0     1581 2024-06-01 08:11:25.463953 dahlia-3.0.0/dahlia/utils.py
+-rw-r--r--   0        0        0     1262 2024-06-02 18:44:02.736613 dahlia-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 dahlia-3.0.0/PKG-INFO
```

### Comparing `dahlia-2.3.2/LICENSE` & `dahlia-3.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022–2023 trag1c
+Copyright (c) 2022–2024 trag1c
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dahlia-2.3.2/src/dahlia/dahlia.py` & `dahlia-3.0.0/dahlia/lib.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from __future__ import annotations
 
 from enum import Enum
-from os import system
-from sys import platform
-from typing import Any, Literal
+from os import getenv
+from typing import Any, Literal, cast
 
-from .constants import (
+from dahlia.constants import (
     BG_FORMAT_TEMPLATES,
     COLOR_SETS,
-    COLORS_24BIT,
     FORMAT_TEMPLATES,
     FORMATTERS,
-    NO_COLOR,
+    RESET,
 )
-from .utils import _find_codes, _with_marker, clean
+from dahlia.utils import _find_codes, _with_marker, clean
 
-if platform in ("win32", "cygwin"):
-    system("")  # type: ignore
+DepthInt = Literal[3, 4, 8, 24]
 
 
 class Depth(Enum):
     """Specifies usable color depth levels."""
 
     TTY = 3
     """3-bit color (tty)"""
@@ -29,205 +26,129 @@
     MEDIUM = 8
     """8-bit color"""
     HIGH = 24
     """24-bit color (true color)"""
 
 
 class Dahlia:
+    """The main Dahlia class handling string transformations."""
+
     __slots__ = (
-        "__depth",
-        "__marker",
-        "__no_color",
-        "__no_reset",
-        "__patterns",
-        "__reset",
+        "_auto_reset",
+        "_depth",
+        "_hash_fields",
+        "_marker",
+        "_no_color",
+        "_patterns",
+        "_reset",
     )
 
+    _depth: DepthInt | None
+
     def __init__(
         self,
         *,
-        depth: Depth
-        | Literal["tty", "low", "medium", "high"]
-        | Literal[3, 4, 8, 24] = Depth.LOW,
+        depth: Depth | DepthInt | str | None = None,
         marker: str = "&",
-        no_color: bool | None = None,
-        no_reset: bool = False,
+        auto_reset: bool = True,
     ) -> None:
-        if isinstance(depth, int):
-            depth = Depth(depth)
+        self._no_color = bool(getenv("NO_COLOR")) or getenv("TERM") == "dumb"
+        if depth is None:
+            self._depth = None if self._no_color else _resolve_depth().value
+        elif isinstance(depth, int):
+            self._depth = Depth(depth).value
         elif isinstance(depth, str):
-            depth = Depth.__members__[depth.upper()]
-        self.__depth = depth.value
-        self.__marker = marker
-        self.__no_color = NO_COLOR if no_color is None else no_color
-        self.__no_reset = no_reset
-        self.__patterns = _with_marker(marker)
-        self.__reset = marker + "r"
-
-    def __eq__(self, other: Any) -> bool:
-        if isinstance(other, Dahlia):
-            return (self.depth, self.no_reset, self.marker) == (
-                other.depth,
-                other.no_reset,
-                other.marker,
-            )
-        return NotImplemented
+            self._depth = Depth[depth.upper()].value
+        else:
+            self._depth = depth.value
+        self._marker = marker
+        self._auto_reset = auto_reset
+        self._patterns = _with_marker(marker)
+        self._reset = marker + "R"
+        self._hash_fields = (self._depth, self._auto_reset, self._marker)
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Dahlia):
+            return NotImplemented
+        return self._hash_fields == other._hash_fields
 
     def __hash__(self) -> int:
-        return hash((self.depth, self.no_reset, self.marker))
+        return hash(self._hash_fields)
 
     def __repr__(self) -> str:
         return (
-            f"Dahlia(depth={self.depth}, "
-            f"no_reset={self.no_reset}, marker={self.marker!r})"
+            f"Dahlia(depth={self._depth}, "
+            f"auto_reset={self._auto_reset}, marker={self._marker!r})"
         )
 
     @property
-    def depth(self) -> int:
+    def depth(self) -> Depth | None:
         """Specifies what ANSI color set to use (in bits)."""
-        return self.__depth
+        return self._depth and Depth(self._depth)
 
     @property
     def marker(self) -> str:
         """Specifies the prefix used by format codes ("&" by default)."""
-        return self.__marker
+        return self._marker
 
     @property
-    def no_reset(self) -> bool:
-        """When True, doesn't add an "&r" at the end when converting strings."""
-        return self.__no_reset
+    def auto_reset(self) -> bool:
+        """When True, appends a full reset code to the transformed string."""
+        return self._auto_reset
 
     def convert(self, string: str) -> str:
-        r"""
-        Formats a string using the format codes.
-
-        Example
-        -------
-
-        .. code-block :: python
-
-            dahlia = Dahlia()
-            text = dahlia.convert("&aHello\n&cWorld")
-            print(text)
-
-
-        Output would be:
-
-        .. raw:: html
-
-            <pre>
-                <span class="&a">Hello</span>
-                <span class="&c">World</span>
-            </pre>
-
-        For more see :ref:`dahlia usage <usage>`
-
-        Parameters
-        ----------
-        string : str
-            String containing text and format codes.
-
-        Returns
-        -------
-        str
-            A formatted string with the appropriate formatting applied.
-        """
-        if self.__no_color:
+        """Transforms a Dahlia string to an ANSI string."""
+        if self._no_color:
             return clean(string)
-        if not (string.endswith(self.__reset) or self.no_reset):
-            string += self.__reset
-        for code, bg, color in _find_codes(string, self.__patterns):
-            string = string.replace(code, self.__get_ansi(color, bg=bg))
-        return string
+        if self.auto_reset and not string.endswith(self._reset):
+            string += self._reset
+        for code, bg, color in _find_codes(string, self._patterns):
+            string = string.replace(code, self._get_ansi(color, bg=bg))
+        return string.replace(self._marker + "_", self._marker)
 
     def input(self, prompt: str) -> str:
-        """
-        Wrapper over :func:`input`, calling the :func:`dahlia` function on the prompt.
-
-        Example
-        -------
-        .. code-block :: python
-
-            dahlia = Dahlia()
-            text = dahlia.input("&bEnter text: ")
-
-
-        Output would be:
-
-        .. raw:: html
-
-            <pre>
-                <span class="&b">Enter text: </span>
-            </pre>
-
-        Parameters
-        ----------
-        prompt : str
-            String containing text and format codes to prompt the user with.
-
-        Returns
-        -------
-        str
-            User input entered after the formatted prompt.
-        """
+        """Wraps the built-in `input` by transforming the prompt."""
         return input(self.convert(prompt))
 
-    def print(self, *args: Any, **kwargs: Any) -> None:
-        r"""
-        Wrapper over :func:`print`, calling the :func:`dahlia` method for each argument.
-
-        Example
-        -------
-        .. code-block :: python
-
-            dahlia = Dahlia()
-            text = dahlia.print("&bHello", "&5World", sep="\n")
-
-
-        Output would be:
-
-        .. raw:: html
-
-            <pre>
-                <span class="&b">Hello</span>
-                <span class="&5">World</span>
-            </pre>
-
-        Parameters
-        ----------
-        \*args : str
-            Objects to print.
-
-        \*\*kwargs
-            Keyword arguments to pass to :func:`print`.
-        """
+    def print(self, *args: object, **kwargs: Any) -> None:
+        """Wraps the built-in `print` by transforming all of its args."""
         print(*map(self.convert, map(str, args)), **kwargs)
 
-    def reset(self) -> None:
-        """Resets all modifiers."""
-        self.print(self.__reset, end="")
-
-    def test(self) -> None:
-        """Prints all default format codes and their formatting."""
-        self.print(
-            "".join(f"{self.marker}{i * 2}" for i in "0123456789abcdefg")
-            + "&r&ll&r&mm&r&nn&r&oo".replace("&", self.marker)
-        )
-
-    def __get_ansi(self, code: str, *, bg: bool) -> str:
+    def _get_ansi(self, code: str, *, bg: bool | None) -> str:
+        if code == "R":
+            return "\033[0m"
+        if code == "_":
+            return self._marker + code
+        if code[0] == "r":
+            return f"\033[{RESET[code[1]]}m"
         formats = BG_FORMAT_TEMPLATES if bg else FORMAT_TEMPLATES
-        if len(code) == 6:
-            r, g, b = (int(code[i : i + 2], 16) for i in (0, 2, 4))
-            return formats[24].format(r, g, b)
+        code_size, rem3 = divmod(len(code), 3)
+        if not rem3:
+            return formats[24].format(
+                *(
+                    (int(code[i : i + 2], 16) for i in (0, 2, 4))
+                    if code_size == 2
+                    else (int(i, 16) * 0x11 for i in code)
+                )
+            )
         if code in FORMATTERS:
             return formats[3].format(FORMATTERS[code])
 
-        template = formats[self.__depth]
-        if self.depth == 24:
-            r, g, b = COLORS_24BIT[code]
-            return template.format(r, g, b)
-
-        color_map = COLOR_SETS[self.depth]
-        value = color_map[code]
-        if self.depth <= 4 and bg:
-            value += 10
-        return template.format(value)
+        depth = cast(int, self._depth)
+        value = COLOR_SETS[depth][code]
+        if bg and depth <= 4:
+            return formats[depth].format(int(value) + 10)
+        return formats[depth].format(value)
+
+
+def _resolve_depth() -> Depth:
+    if getenv("COLORTERM") in {"truecolor", "24bit"}:
+        return Depth.HIGH
+    if (
+        (term := getenv("TERM", "")) in {"terminator", "mosh"}
+        or "24bit" in term
+        or "24-bit" in term
+    ):
+        return Depth.HIGH
+    if "256" in term:
+        return Depth.MEDIUM
+    return Depth.LOW
```

### Comparing `dahlia-2.3.2/PKG-INFO` & `dahlia-3.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,71 @@
 Metadata-Version: 2.1
 Name: dahlia
-Version: 2.3.2
+Version: 3.0.0
 Summary: A library allowing you to use Minecraft format codes in strings.
 Home-page: https://github.com/dahlia-lib/dahlia
 License: MIT
 Author: trag1c
 Author-email: trag1cdev@yahoo.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Project-URL: Documentation, https://dahlia.readthedocs.io/en/latest
+Classifier: Programming Language :: Python :: 3.12
+Project-URL: Documentation, https://dahlia-lib.github.io/dahlia/
 Project-URL: Repository, https://github.com/dahlia-lib/dahlia
 Description-Content-Type: text/markdown
 
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dahlia)](https://pypi.python.org/pypi/dahlia)
-[![PyPI version](https://badge.fury.io/py/dahlia.svg)](https://badge.fury.io/py/dahlia)
-[![Documentation Status](https://readthedocs.org/projects/dahlia/badge/?version=latest)](https://dahlia.readthedocs.io/en/latest/?badge=latest)
-# Dahlia
+[![Dahlia spec](https://img.shields.io/badge/Dahlia%20spec-v1.0-pink?style=flat)](https://github.com/dahlia-lib/spec)
+[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-Dahlia is a simple text formatting package, inspired by text formatting in the game Minecraft.
+# Dahlia
 
-Text is formatted in a similar way to in the game. With Dahlia, it is formatted by typing a special character `&` followed by a format code and finally the text to be formatted.
+Dahlia is a simple text formatting package, inspired by text formatting in the
+game Minecraft.
 
 ## Installation
 
-Dahlia is available on PyPI and can be installed with pip, or any other Python package manager:
-
-```
+Dahlia is available on PyPI and can be installed with pip, or any other Python
+package manager:
+```console
 $ pip install dahlia
 ```
-(Some systems may require you to use `pip3`, `python -m pip`, or `py -m pip` instead)
+(Some systems may require you to use `pip3`, `python -m pip`, or `py -m pip`
+instead)
+
+## [Documentation]
+
+## Contributing
+Contributions are welcome!
 
-## Documentation
+Please open an issue before submitting a pull request (unless it's a minor
+change like fixing a typo).
+
+To get started:
+1. Clone your fork of the project.
+2. Set up the project with `just install` (make sure you have [poetry]
+   installed).
+3. After you're done, run `just check` to check your changes.
+
+> [!Note]
+> If you don't want to install [just], simply look up the recipes
+> in the project's [`justfile`][justfile].
 
-Dahlia documentation is available at https://dahlia.readthedocs.io.
 
 ## License
 
 Dahlia is licensed under the MIT License.
 
-## Examples
+If you have any questions, or would like to get in touch, join my
+[Discord server]!
 
-<img width="805" alt="Screen Shot 2022-10-05 at 22 56 57" src="https://user-images.githubusercontent.com/77130613/194162110-fb77713c-7008-4f5f-a79c-7a3666f2fd11.png">
+[Discord server]: https://discord.gg/C8QE5tVQEq
+[Documentation]: https://dahlia-lib.github.io/dahlia/
+[just]: https://github.com/casey/just
+[justfile]: https://github.com/dahlia-lib/dahlia/blob/master/justfile
+[poetry]: https://python-poetry.org/
```

