# Comparing `tmp/pipx-1.4.3.tar.gz` & `tmp/pipx-1.5.0.tar.gz`

## Comparing `pipx-1.4.3.tar` & `pipx-1.5.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
--rw-r--r--   0        0        0    28856 2020-02-02 00:00:00.000000 pipx-1.4.3/CHANGELOG.md
--rw-r--r--   0        0        0     7662 2020-02-02 00:00:00.000000 pipx-1.4.3/CONTRIBUTING.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pipx-1.4.3/installation.md -> docs/installation.md
--rw-r--r--   0        0        0   266063 2020-02-02 00:00:00.000000 pipx-1.4.3/pipx_demo.gif
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/__init__.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/__main__.py
--rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/animate.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/colors.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/constants.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/emojis.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/interpreter.py
--rw-r--r--   0        0        0    34196 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/main.py
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/package_specifier.py
--rw-r--r--   0        0        0     6365 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/pipx_metadata_file.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/shared_libs.py
--rw-r--r--   0        0        0    14906 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/util.py
--rw-r--r--   0        0        0    18270 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/venv.py
--rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/venv_inspect.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/version.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/__init__.py
--rw-r--r--   0        0        0    16868 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/common.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/ensure_path.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/environment.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/inject.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/install.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/list_packages.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/reinstall.py
--rw-r--r--   0        0        0    12341 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/run.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/run_pip.py
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/uninject.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/uninstall.py
--rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 pipx-1.4.3/src/pipx/commands/upgrade.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pipx-1.4.3/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pipx-1.4.3/LICENSE
--rw-r--r--   0        0        0    16126 2020-02-02 00:00:00.000000 pipx-1.4.3/README.md
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 pipx-1.4.3/pyproject.toml
--rw-r--r--   0        0        0    17427 2020-02-02 00:00:00.000000 pipx-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0    32630 2020-02-02 00:00:00.000000 pipx-1.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     7655 2020-02-02 00:00:00.000000 pipx-1.5.0/CONTRIBUTING.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pipx-1.5.0/installation.md -> docs/installation.md
+-rw-r--r--   0        0        0   266063 2020-02-02 00:00:00.000000 pipx-1.5.0/pipx_demo.gif
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/__init__.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/__main__.py
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/animate.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/colors.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/constants.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/emojis.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/interpreter.py
+-rw-r--r--   0        0        0    36088 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/main.py
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/package_specifier.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/paths.py
+-rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/pipx_metadata_file.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/shared_libs.py
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/standalone_python.py
+-rw-r--r--   0        0        0    15258 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/util.py
+-rw-r--r--   0        0        0    19001 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/venv.py
+-rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/venv_inspect.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/version.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/version.pyi
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/__init__.py
+-rw-r--r--   0        0        0    17207 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/common.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/ensure_path.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/environment.py
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/inject.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/install.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/interpreter.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/list_packages.py
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/reinstall.py
+-rw-r--r--   0        0        0    12471 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/run.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/run_pip.py
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/uninject.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/uninstall.py
+-rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 pipx-1.5.0/src/pipx/commands/upgrade.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pipx-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pipx-1.5.0/LICENSE
+-rw-r--r--   0        0        0    16639 2020-02-02 00:00:00.000000 pipx-1.5.0/README.md
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 pipx-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    17940 2020-02-02 00:00:00.000000 pipx-1.5.0/PKG-INFO
```

### Comparing `pipx-1.4.3/CHANGELOG.md` & `pipx-1.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,73 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 This project uses [*towncrier*](https://towncrier.readthedocs.io/) for keeping the changelog. DO NOT commit any changes to this file.
 {% include '_draft_changelog.md' ignore missing %}
 
 <!-- towncrier release notes start -->
 
+## [1.5.0](https://github.com/pypa/pipx/tree/1.5.0) - 2024-03-29
+
+
+### Features
+
+- Add `--global` option to `pipx` commands.
+      - This will run the action in a global scope and affect environment for all system users. ([#754](https://github.com/pypa/pipx/issues/754))
+- Add a `--fetch-missing-python` flag to all commands that accept a `--python` flag.
+      - When combined, this will automatically download a standalone copy of the requested python version if it's not already available on the user's system. ([#1242](https://github.com/pypa/pipx/issues/1242))
+- Add commands to list and prune standalone interpreters ([#1248](https://github.com/pypa/pipx/issues/1248))
+- Revert platform-specific directories on MacOS and Windows
+      - They were leading to a lot of issues with Windows sandboxing and spaces in shebangs on MacOS. ([#1257](https://github.com/pypa/pipx/issues/1257))
+- Add `--install` option to `pipx upgrade` command.
+      - This will install the package given as argument if it is not already installed. ([#1262](https://github.com/pypa/pipx/issues/1262))
+
+### Bugfixes
+
+- Correctly resolve home directory in pipx directory environment variables. ([#94](https://github.com/pypa/pipx/issues/94))
+- Pass through `pip` arguments when upgrading shared libraries. ([#964](https://github.com/pypa/pipx/issues/964))
+- Fix installation issues when files in the working directory interfere with venv creation process. ([#1091](https://github.com/pypa/pipx/issues/1091))
+- Report correct filename in tracebacks with `pipx run <scriptname>` ([#1191](https://github.com/pypa/pipx/issues/1191))
+- Let self-managed pipx uninstall itself on windows again. ([#1203](https://github.com/pypa/pipx/issues/1203))
+- Fix path resolution for python executables looked up in PATH on windows. ([#1205](https://github.com/pypa/pipx/issues/1205))
+- Display help message when `pipx install` is run without arguments. ([#1266](https://github.com/pypa/pipx/issues/1266))
+- Fix crashes due to superfluous `-q ` flags by discarding exceeding values ([#1283](https://github.com/pypa/pipx/issues/1283))
+
+### Improved Documentation
+
+- Update the completion instructions for zipapp users. ([#1072](https://github.com/pypa/pipx/issues/1072))
+- Update the example for running scripts with dependencies. ([#1227](https://github.com/pypa/pipx/issues/1227))
+- Update the docs for package developers on the use of configuration using pyproject.toml ([#1229](https://github.com/pypa/pipx/issues/1229))
+- Add installation instructions for Fedora ([#1239](https://github.com/pypa/pipx/issues/1239))
+- Update the examples for installation from local dir ([#1277](https://github.com/pypa/pipx/issues/1277))
+- Fix inconsistent wording in `pipx install` command description. ([#1307](https://github.com/pypa/pipx/issues/1307))
+
+### Deprecations and Removals
+
+- Deprecate `--skip-maintenance` flag of `pipx list`; maintenance is now never executed there ([#1256](https://github.com/pypa/pipx/issues/1256))
+
+### Misc
+
+- [#1296](https://github.com/pypa/pipx/issues/1296)
+
+
+## [1.4.3](https://github.com/pypa/pipx/tree/1.4.3) - 2024-01-16
+
+
+### Bugfixes
+
+- Autofix python version for pylauncher, when version is provided prefixed with `python` ([#1150](https://github.com/pypa/pipx/issues/1150))
+- Support building pipx wheels with setuptools-scm<7, such as on FreeBSD. ([#1208](https://github.com/pypa/pipx/issues/1208))
+
+### Improved Documentation
+
+- Provide useful error messages when unresolvable python version is passed ([#1150](https://github.com/pypa/pipx/issues/1150))
+- Introduce towncrier for managing the changelog ([#1161](https://github.com/pypa/pipx/issues/1161))
+- Add workaround for using pipx applications in shebang under macOS ([#1198](https://github.com/pypa/pipx/issues/1198))
+
+
 ## [1.4.2](https://github.com/pypa/pipx/tree/1.4.2)
 
 ### Features
 
 - Allow skipping maintenance tasks during list command
 - Raise more user friendly error when provided `--python` version is not found
 - Update `pipx run` on scripts using `/// script` and no `run` table following the updated version of PEP 723 (#1180)
@@ -57,15 +116,15 @@
 
 ### Features
 
 - The project version number is now dynamic and generated from the VCS at build time
 
 ### Improved Documentation
 
-- Add additonal example for --pip-args option, to docs/examples.md
+- Add additional example for --pip-args option, to docs/examples.md
 
 ## [1.3.1](https://github.com/pypa/pipx/tree/1.3.1)
 
 ### Bugfixes
 
 - Fix combining of --editable and --force flag
```

### Comparing `pipx-1.4.3/CONTRIBUTING.md` & `pipx-1.5.0/CONTRIBUTING.md`

 * *Files 8% similar despite different names*

```diff
@@ -122,27 +122,29 @@
 
 To run unit tests in Python3.12, you can run
 
 ```
 nox -s tests-3.12
 ```
 
-!!! tip You can run a specific unit test by passing arguments to pytest, the test runner pipx uses:
-
-    ```
-    nox -s tests-3.8 -- -k EXPRESSION
-    ```
-
-    `EXPRESSION` can be a test name, such as
-
-    ```
-    nox -s tests-3.8 -- -k test_uninstall
-    ```
-
-    Coverage errors can usually be ignored when only running a subset of tests.
+> [!TIP]
+>
+> You can run a specific unit test by passing arguments to pytest, the test runner pipx uses:
+>
+> ```
+> nox -s tests-3.8 -- -k EXPRESSION
+> ```
+>
+> `EXPRESSION` can be a test name, such as
+>
+> ```
+> nox -s tests-3.8 -- -k test_uninstall
+> ```
+>
+> Coverage errors can usually be ignored when only running a subset of tests.
 
 ### Running Unit Tests Offline
 
 Running the unit tests requires a directory `.pipx_tests/package_cache` to be populated from a fixed list of package
 distribution files (wheels or source files). If you have network access, `nox -s tests` automatically makes sure this
 directory is populated (including downloading files if necessary) as a first step. Thus, if you are running the tests
 with network access, you can ignore the rest of this section.
```

### Comparing `pipx-1.4.3/pipx_demo.gif` & `pipx-1.5.0/pipx_demo.gif`

 * *Files identical despite different names*

### Comparing `pipx-1.4.3/src/pipx/animate.py` & `pipx-1.5.0/src/pipx/animate.py`

 * *Files identical despite different names*

### Comparing `pipx-1.4.3/src/pipx/colors.py` & `pipx-1.5.0/src/pipx/colors.py`

 * *Files identical despite different names*

### Comparing `pipx-1.4.3/src/pipx/emojis.py` & `pipx-1.5.0/src/pipx/emojis.py`

 * *Files identical despite different names*

### Comparing `pipx-1.4.3/src/pipx/interpreter.py` & `pipx-1.5.0/src/pipx/interpreter.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import os
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 from typing import Optional
 
-from pipx.constants import WINDOWS
+from pipx.constants import FETCH_MISSING_PYTHON, WINDOWS
+from pipx.standalone_python import download_python_build_standalone
 from pipx.util import PipxError
 
 logger = logging.getLogger(__name__)
 
 
 def has_venv() -> bool:
     try:
@@ -38,30 +39,40 @@
             message += "on your PATH or the file path is valid. "
             if potentially_path:
                 message += "The provided version looks like a path, but no executable was found there."
             if potentially_pylauncher:
                 message += (
                     "The provided version looks like a version for Python Launcher, " "but `py` was not found on PATH."
                 )
+        if source == "the python-build-standalone project":
+            message += "listed in https://github.com/indygreg/python-build-standalone/releases/latest."
         super().__init__(message, wrap_message)
 
 
-def find_python_interpreter(python_version: str) -> str:
+def find_python_interpreter(python_version: str, fetch_missing_python: bool = False) -> str:
     if Path(python_version).is_file():
         return python_version
 
     try:
         py_executable = find_py_launcher_python(python_version)
         if py_executable:
             return py_executable
     except (subprocess.CalledProcessError, FileNotFoundError) as e:
         raise InterpreterResolutionError(source="py launcher", version=python_version) from e
 
     if shutil.which(python_version):
         return python_version
+
+    if fetch_missing_python or FETCH_MISSING_PYTHON:
+        try:
+            standalone_executable = download_python_build_standalone(python_version)
+            return standalone_executable
+        except PipxError as e:
+            raise InterpreterResolutionError(source="the python-build-standalone project", version=python_version) from e
+
     raise InterpreterResolutionError(source="PATH", version=python_version)
 
 
 # The following code was copied from https://github.com/uranusjr/pipx-standalone
 # which uses the same technique to build a completely standalone pipx
 # distribution.
 #
```

### Comparing `pipx-1.4.3/src/pipx/main.py` & `pipx-1.5.0/src/pipx/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,39 @@
 import re
 import shlex
 import sys
 import textwrap
 import time
 import urllib.parse
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import argcomplete
 import platformdirs
 from packaging.utils import canonicalize_name
 
-import pipx.constants
-from pipx import commands, constants
+from pipx import commands, constants, paths
 from pipx.animate import hide_cursor, show_cursor
 from pipx.colors import bold, green
-from pipx.constants import EXIT_CODE_SPECIFIED_PYTHON_EXECUTABLE_NOT_FOUND, MINIMUM_PYTHON_VERSION, WINDOWS, ExitCode
+from pipx.constants import (
+    EXIT_CODE_OK,
+    EXIT_CODE_SPECIFIED_PYTHON_EXECUTABLE_NOT_FOUND,
+    MINIMUM_PYTHON_VERSION,
+    WINDOWS,
+    ExitCode,
+)
 from pipx.emojis import hazard
-from pipx.interpreter import DEFAULT_PYTHON, InterpreterResolutionError, find_python_interpreter
+from pipx.interpreter import (
+    DEFAULT_PYTHON,
+    InterpreterResolutionError,
+    find_python_interpreter,
+)
 from pipx.util import PipxError, mkdir, pipx_wrap, rmdir
 from pipx.venv import VenvContainer
-from pipx.version import __version__
+from pipx.version import version as __version__
 
 logger = logging.getLogger(__name__)
 
 VenvCompleter = Callable[[str], List[str]]
 
 
 def print_version() -> None:
@@ -62,17 +71,17 @@
 PIPX_DESCRIPTION = textwrap.dedent(
     f"""
     Install and execute apps from Python packages.
 
     Binaries can either be installed globally into isolated Virtual Environments
     or run directly in a temporary Virtual Environment.
 
-    Virtual Environment location is {str(constants.PIPX_LOCAL_VENVS)}.
-    Symlinks to apps are placed in {str(constants.LOCAL_BIN_DIR)}.
-    Symlinks to manual pages are placed in {str(constants.LOCAL_MAN_DIR)}.
+    Virtual Environment location is {str(paths.ctx.venvs)}.
+    Symlinks to apps are placed in {str(paths.ctx.bin_dir)}.
+    Symlinks to manual pages are placed in {str(paths.ctx.man_dir)}.
 
     """
 )
 PIPX_DESCRIPTION += pipx_wrap(
     """
     optional environment variables:
       PIPX_HOME             Overrides default pipx location. Virtual Environments will be installed to $PIPX_HOME/venvs.
@@ -91,39 +100,39 @@
     f"""
     The install command is the preferred way to globally install apps
     from python packages on your system. It creates an isolated virtual
     environment for the package, then ensures the package's apps are
     accessible on your $PATH. The package's manual pages installed in
     share/man/man[1-9] can be viewed with man on an operating system where
     it is available and the path in the environment variable `PIPX_MAN_DIR`
-    (default: {constants.DEFAULT_PIPX_MAN_DIR}) is in the man search path
+    (default: {paths.DEFAULT_PIPX_MAN_DIR}) is in the man search path
     ($MANPATH).
 
     The result: apps you can run from anywhere, located in packages
     you can cleanly upgrade or uninstall. Guaranteed to not have
     dependency version conflicts or interfere with your OS's python
     packages. 'sudo' is not required to do this.
 
-    pipx install PACKAGE_NAME ...
-    pipx install --python PYTHON PACKAGE_NAME
+    pipx install PACKAGE_SPEC ...
+    pipx install --python PYTHON PACKAGE_SPEC
     pipx install VCS_URL
     pipx install ./LOCAL_PATH
     pipx install ZIP_FILE
     pipx install TAR_GZ_FILE
 
     The PACKAGE_SPEC argument is passed directly to `pip install`.
 
-    The default virtual environment location is {constants.DEFAULT_PIPX_HOME}
+    The default virtual environment location is {paths.DEFAULT_PIPX_HOME}
     and can be overridden by setting the environment variable `PIPX_HOME`
     (Virtual Environments will be installed to `$PIPX_HOME/venvs`).
 
-    The default app location is {constants.DEFAULT_PIPX_BIN_DIR} and can be
+    The default app location is {paths.DEFAULT_PIPX_BIN_DIR} and can be
     overridden by setting the environment variable `PIPX_BIN_DIR`.
 
-    The default manual pages location is {constants.DEFAULT_PIPX_MAN_DIR} and
+    The default manual pages location is {paths.DEFAULT_PIPX_MAN_DIR} and
     can be overridden by setting the environment variable `PIPX_MAN_DIR`.
 
     The default python executable used to install a package is
     {DOC_DEFAULT_PYTHON} and can be overridden
     by setting the environment variable `PIPX_DEFAULT_PYTHON`.
     """
 )
@@ -161,20 +170,22 @@
 def get_venv_args(parsed_args: Dict[str, str]) -> List[str]:
     venv_args: List[str] = []
     if parsed_args.get("system_site_packages"):
         venv_args += ["--system-site-packages"]
     return venv_args
 
 
-def run_pipx_command(args: argparse.Namespace) -> ExitCode:  # noqa: C901
+def run_pipx_command(args: argparse.Namespace, subparsers: Dict[str, argparse.ArgumentParser]) -> ExitCode:  # noqa: C901
     verbose = args.verbose if "verbose" in args else False
+    if not constants.WINDOWS and args.is_global:
+        paths.ctx.make_global()
     pip_args = get_pip_args(vars(args))
     venv_args = get_venv_args(vars(args))
 
-    venv_container = VenvContainer(constants.PIPX_LOCAL_VENVS)
+    venv_container = VenvContainer(paths.ctx.venvs)
 
     if "package" in args:
         package = args.package
         if urllib.parse.urlparse(package).scheme:
             raise PipxError("Package cannot be a url")
 
         if "spec" in args and args.spec is not None:
@@ -184,18 +195,20 @@
 
         venv_dir = venv_container.get_venv_dir(package)
         logger.info(f"Virtual Environment location is {venv_dir}")
     if "skip" in args:
         skip_list = [canonicalize_name(x) for x in args.skip]
 
     if "python" in args and args.python is not None:
+        fetch_missing_python = args.fetch_missing_python
         try:
-            interpreter = find_python_interpreter(args.python)
+            interpreter = find_python_interpreter(args.python, fetch_missing_python=fetch_missing_python)
             args.python = interpreter
         except InterpreterResolutionError as e:
+            logger.debug("Failed to resolve interpreter:", exc_info=True)
             print(
                 pipx_wrap(
                     f"{hazard} {e}",
                     subsequent_indent=" " * 4,
                 )
             )
             return EXIT_CODE_SPECIFIED_PYTHON_EXECUTABLE_NOT_FOUND
@@ -216,16 +229,16 @@
         # We should never reach here because run() is NoReturn.
         return ExitCode(1)
     elif args.command == "install":
         return commands.install(
             None,
             None,
             args.package_spec,
-            constants.LOCAL_BIN_DIR,
-            constants.LOCAL_MAN_DIR,
+            paths.ctx.bin_dir,
+            paths.ctx.man_dir,
             args.python,
             pip_args,
             venv_args,
             verbose,
             force=args.force,
             reinstall=False,
             include_dependencies=args.include_deps,
@@ -244,56 +257,77 @@
             force=args.force,
             suffix=args.with_suffix,
         )
     elif args.command == "uninject":
         return commands.uninject(
             venv_dir,
             args.dependencies,
-            local_bin_dir=constants.LOCAL_BIN_DIR,
-            local_man_dir=constants.LOCAL_MAN_DIR,
+            local_bin_dir=paths.ctx.bin_dir,
+            local_man_dir=paths.ctx.man_dir,
             leave_deps=args.leave_deps,
             verbose=verbose,
         )
     elif args.command == "upgrade":
         return commands.upgrade(
             venv_dir,
+            args.python,
             pip_args,
             verbose,
             include_injected=args.include_injected,
             force=args.force,
+            install=args.install,
         )
     elif args.command == "upgrade-all":
         return commands.upgrade_all(
             venv_container,
             verbose,
             include_injected=args.include_injected,
             skip=skip_list,
             force=args.force,
+            pip_args=pip_args,
         )
     elif args.command == "list":
         return commands.list_packages(
-            venv_container, args.include_injected, args.json, args.short, args.skip_maintenance
-        )
+            venv_container,
+            args.include_injected,
+            args.json,
+            args.short,
+        )
+    elif args.command == "interpreter":
+        if args.interpreter_command == "list":
+            return commands.list_interpreters(venv_container)
+        elif args.interpreter_command == "prune":
+            return commands.prune_interpreters(venv_container)
+        elif args.interpreter_command is None:
+            subparsers["interpreter"].print_help()
+            return EXIT_CODE_OK
+        else:
+            raise PipxError(f"Unknown interpreter command {args.interpreter_command}")
     elif args.command == "uninstall":
-        return commands.uninstall(venv_dir, constants.LOCAL_BIN_DIR, constants.LOCAL_MAN_DIR, verbose)
+        return commands.uninstall(venv_dir, paths.ctx.bin_dir, paths.ctx.man_dir, verbose)
     elif args.command == "uninstall-all":
-        return commands.uninstall_all(venv_container, constants.LOCAL_BIN_DIR, constants.LOCAL_MAN_DIR, verbose)
+        return commands.uninstall_all(
+            venv_container,
+            paths.ctx.bin_dir,
+            paths.ctx.man_dir,
+            verbose,
+        )
     elif args.command == "reinstall":
         return commands.reinstall(
             venv_dir=venv_dir,
-            local_bin_dir=constants.LOCAL_BIN_DIR,
-            local_man_dir=constants.LOCAL_MAN_DIR,
+            local_bin_dir=paths.ctx.bin_dir,
+            local_man_dir=paths.ctx.man_dir,
             python=args.python,
             verbose=verbose,
         )
     elif args.command == "reinstall-all":
         return commands.reinstall_all(
             venv_container,
-            constants.LOCAL_BIN_DIR,
-            constants.LOCAL_MAN_DIR,
+            paths.ctx.bin_dir,
+            paths.ctx.man_dir,
             args.python,
             verbose,
             skip=skip_list,
         )
     elif args.command == "runpip":
         if not venv_dir:
             raise PipxError("Developer error: venv_dir is not defined.")
@@ -332,23 +366,42 @@
     )
 
 
 def add_include_dependencies(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("--include-deps", help="Include apps of dependent packages", action="store_true")
 
 
+def add_python_options(parser: argparse.ArgumentParser) -> None:
+    parser.add_argument(
+        "--python",
+        default=DEFAULT_PYTHON,
+        help=(
+            "Python to install with. Possible values can be the executable name (python3.11), "
+            "the version to pass to py launcher (3.11), or the full path to the executable."
+            f"Requires Python {MINIMUM_PYTHON_VERSION} or above."
+        ),
+    )
+    parser.add_argument(
+        "--fetch-missing-python",
+        action="store_true",
+        help=(
+            "Whether to fetch a standalone python build from GitHub if the specified python version is not found locally on the system."
+        ),
+    )
+
+
 def _add_install(subparsers: argparse._SubParsersAction, shared_parser: argparse.ArgumentParser) -> None:
     p = subparsers.add_parser(
         "install",
         help="Install a package",
         formatter_class=LineWrapRawTextHelpFormatter,
         description=INSTALL_DESCRIPTION,
         parents=[shared_parser],
     )
-    p.add_argument("package_spec", help="package name(s) or pip installation spec(s)", nargs="*")
+    p.add_argument("package_spec", help="package name(s) or pip installation spec(s)", nargs="+")
     add_include_dependencies(p)
     p.add_argument(
         "--force",
         "-f",
         action="store_true",
         help="Modify existing virtual environment and files in PIPX_BIN_DIR and PIPX_MAN_DIR",
     )
@@ -356,23 +409,15 @@
         "--suffix",
         default="",
         help=(
             "Optional suffix for virtual environment and executable names. "
             "NOTE: The suffix feature is experimental and subject to change."
         ),
     )
-    p.add_argument(
-        "--python",
-        # Don't pass a default Python here so we know whether --python flag was passed
-        help=(
-            "Python to install with. Possible values can be the executable name (python3.11), "
-            "the version to pass to py launcher (3.11), or the full path to the executable."
-            f"Requires Python {MINIMUM_PYTHON_VERSION} or above."
-        ),
-    )
+    add_python_options(p)
     p.add_argument(
         "--preinstall",
         action="append",
         help=("Optional packages to be installed into the Virtual Environment before " "installing the main package."),
     )
     add_pip_venv_args(p)
 
@@ -456,14 +501,20 @@
     p.add_argument(
         "--force",
         "-f",
         action="store_true",
         help="Modify existing virtual environment and files in PIPX_BIN_DIR and PIPX_MAN_DIR",
     )
     add_pip_venv_args(p)
+    p.add_argument(
+        "--install",
+        action="store_true",
+        help="Install package spec if missing",
+    )
+    add_python_options(p)
 
 
 def _add_upgrade_all(subparsers: argparse._SubParsersAction, shared_parser: argparse.ArgumentParser) -> None:
     p = subparsers.add_parser(
         "upgrade-all",
         help="Upgrade all packages. Runs `pip install -U <pkgname>` for each package.",
         description="Upgrades all packages within their virtual environments by running 'pip install --upgrade PACKAGE'",
@@ -515,23 +566,15 @@
             with the same options used in the original install of PACKAGE.
 
             """
         ),
         parents=[shared_parser],
     )
     p.add_argument("package").completer = venv_completer
-    p.add_argument(
-        "--python",
-        default=DEFAULT_PYTHON,
-        help=(
-            "Python to reinstall with. Possible values can be the executable name (python3.11), "
-            "the version to pass to py launcher (3.11), or the full path to the executable."
-            f"Requires Python {MINIMUM_PYTHON_VERSION} or above."
-        ),
-    )
+    add_python_options(p)
 
 
 def _add_reinstall_all(subparsers: argparse._SubParsersAction, shared_parser: argparse.ArgumentParser) -> None:
     p = subparsers.add_parser(
         "reinstall-all",
         formatter_class=LineWrapRawTextHelpFormatter,
         help="Reinstall all packages",
@@ -544,23 +587,15 @@
             This is useful if you upgraded to a new version of Python and want
             all your packages to use the latest as well.
 
             """
         ),
         parents=[shared_parser],
     )
-    p.add_argument(
-        "--python",
-        default=DEFAULT_PYTHON,
-        help=(
-            "Python to reinstall with. Possible values can be the executable name (python3.11), "
-            "the version to pass to py launcher (3.11), or the full path to the executable."
-            f"Requires Python {MINIMUM_PYTHON_VERSION} or above."
-        ),
-    )
+    add_python_options(p)
     p.add_argument("--skip", nargs="+", default=[], help="skip these packages")
 
 
 def _add_list(subparsers: argparse._SubParsersAction, shared_parser: argparse.ArgumentParser) -> None:
     p = subparsers.add_parser(
         "list",
         help="List installed packages",
@@ -571,15 +606,34 @@
         "--include-injected",
         action="store_true",
         help="Show packages injected into the main app's environment",
     )
     g = p.add_mutually_exclusive_group()
     g.add_argument("--json", action="store_true", help="Output rich data in json format.")
     g.add_argument("--short", action="store_true", help="List packages only.")
-    g.add_argument("--skip-maintenance", action="store_true", help="Skip maintenance tasks.")
+    g.add_argument("--skip-maintenance", action="store_true", help="(deprecated) No-op")
+
+
+def _add_interpreter(
+    subparsers: argparse._SubParsersAction, shared_parser: argparse.ArgumentParser
+) -> argparse.ArgumentParser:
+    p: argparse.ArgumentParser = subparsers.add_parser(
+        "interpreter",
+        help="Interact with interpreters managed by pipx",
+        description="Interact with interpreters managed by pipx",
+        parents=[shared_parser],
+    )
+    s = p.add_subparsers(
+        title="subcommands",
+        description="Get help for commands with pipx interpreter COMMAND --help",
+        dest="interpreter_command",
+    )
+    s.add_parser("list", help="List available interpreters", description="List available interpreters")
+    s.add_parser("prune", help="Prune unused interpreters", description="Prune unused interpreters")
+    return p
 
 
 def _add_run(subparsers: argparse._SubParsersAction, shared_parser: argparse.ArgumentParser) -> None:
     p = subparsers.add_parser(
         "run",
         formatter_class=LineWrapRawTextHelpFormatter,
         help=(
@@ -589,28 +643,28 @@
         ),
         description=textwrap.dedent(
             f"""
             Download the latest version of a package to a temporary virtual environment,
             then run an app from it. The environment will be cached
             and re-used for up to {constants.TEMP_VENV_EXPIRATION_THRESHOLD_DAYS} days. This
             means subsequent calls to 'run' for the same package will be faster
-            since they can re-use the cached Virtual Environment.
+            since they can reuse the cached Virtual Environment.
 
             In support of PEP 582 'run' will use apps found in a local __pypackages__
             directory, if present. Please note that this behavior is experimental,
             and acts as a companion tool to pythonloc. It may be modified or
             removed in the future. See https://github.com/cs01/pythonloc.
             """
         ),
         parents=[shared_parser],
     )
     p.add_argument(
         "--no-cache",
         action="store_true",
-        help="Do not re-use cached virtual environment if it exists",
+        help="Do not reuse cached virtual environment if it exists",
     )
     p.add_argument(
         "app_with_args",
         metavar="app ...",
         nargs=argparse.REMAINDER,
         help="app/package name and any arguments to be passed to it",
         default=[],
@@ -618,23 +672,15 @@
     p.add_argument("--path", action="store_true", help="Interpret app name as a local path")
     p.add_argument(
         "--pypackages",
         action="store_true",
         help="Require app to be run from local __pypackages__ directory",
     )
     p.add_argument("--spec", help=SPEC_HELP)
-    p.add_argument(
-        "--python",
-        default=DEFAULT_PYTHON,
-        help=(
-            "Python to run with. Possible values can be the executable name (python3.11), "
-            "the version to pass to py launcher (3.11), or the full path to the executable. "
-            f"Requires Python {MINIMUM_PYTHON_VERSION} or above."
-        ),
-    )
+    add_python_options(p)
     add_pip_venv_args(p)
     p.set_defaults(subparser=p)
 
     # modify usage text to show required app argument
     p.usage = re.sub(r"^usage: ", "", p.format_usage())
     # add a double-dash to usage text to show requirement before app
     p.usage = re.sub(r"\.\.\.", "app ...", p.usage)
@@ -700,82 +746,100 @@
             """
         ),
         parents=[shared_parser],
     )
     p.add_argument("--value", "-V", metavar="VARIABLE", help="Print the value of the variable.")
 
 
-def get_command_parser() -> argparse.ArgumentParser:
-    venv_container = VenvContainer(constants.PIPX_LOCAL_VENVS)
+def get_command_parser() -> Tuple[argparse.ArgumentParser, Dict[str, argparse.ArgumentParser]]:
+    venv_container = VenvContainer(paths.ctx.venvs)
 
     completer_venvs = InstalledVenvsCompleter(venv_container)
 
     shared_parser = argparse.ArgumentParser(add_help=False)
 
     shared_parser.add_argument(
         "--quiet",
         "-q",
         action="count",
         default=0,
         help=(
             "Give less output. May be used multiple times corresponding to the"
-            " WARNING, ERROR, and CRITICAL logging levels."
+            " ERROR and CRITICAL logging levels. The count maxes out at 2."
         ),
     )
 
-    shared_parser.add_argument("--verbose", "-v", action="count", default=0, help=("Give more output."))
+    shared_parser.add_argument(
+        "--verbose",
+        "-v",
+        action="count",
+        default=0,
+        help=(
+            "Give more output. May be used multiple times corresponding to the"
+            " INFO, DEBUG and NOTSET logging levels. The count maxes out at 3."
+        ),
+    )
 
     parser = argparse.ArgumentParser(
         prog=prog_name(),
         formatter_class=LineWrapRawTextHelpFormatter,
         description=PIPX_DESCRIPTION,
         parents=[shared_parser],
     )
     parser.man_short_description = PIPX_DESCRIPTION.splitlines()[1]  # type: ignore
 
     subparsers = parser.add_subparsers(dest="command", description="Get help for commands with pipx COMMAND --help")
 
+    subparsers_with_subcommands = {}
     _add_install(subparsers, shared_parser)
     _add_uninject(subparsers, completer_venvs.use, shared_parser)
     _add_inject(subparsers, completer_venvs.use, shared_parser)
     _add_upgrade(subparsers, completer_venvs.use, shared_parser)
     _add_upgrade_all(subparsers, shared_parser)
     _add_uninstall(subparsers, completer_venvs.use, shared_parser)
     _add_uninstall_all(subparsers, shared_parser)
     _add_reinstall(subparsers, completer_venvs.use, shared_parser)
     _add_reinstall_all(subparsers, shared_parser)
     _add_list(subparsers, shared_parser)
+    subparsers_with_subcommands["interpreter"] = _add_interpreter(subparsers, shared_parser)
     _add_run(subparsers, shared_parser)
     _add_runpip(subparsers, completer_venvs.use, shared_parser)
     _add_ensurepath(subparsers, shared_parser)
     _add_environment(subparsers, shared_parser)
 
+    if not constants.WINDOWS:
+        parser.add_argument(
+            "--global",
+            action="store_true",
+            dest="is_global",
+            help="Perform action globally for all users.",
+        )
     parser.add_argument("--version", action="store_true", help="Print version and exit")
     subparsers.add_parser(
         "completions",
         help="Print instructions on enabling shell completions for pipx",
         description="Print instructions on enabling shell completions for pipx",
         parents=[shared_parser],
     )
-    return parser
+    return parser, subparsers_with_subcommands
 
 
 def delete_oldest_logs(file_list: List[Path], keep_number: int) -> None:
     file_list = sorted(file_list)
     if len(file_list) > keep_number:
         for existing_file in file_list[:-keep_number]:
             try:
                 existing_file.unlink()
             except FileNotFoundError:
                 pass
 
 
 def _setup_log_file(pipx_log_dir: Optional[Path] = None) -> Path:
     max_logs = 10
-    pipx_log_dir = pipx_log_dir or constants.PIPX_LOG_DIR
+    pipx_log_dir = pipx_log_dir or paths.ctx.logs
     # don't use utils.mkdir, to prevent emission of log message
     pipx_log_dir.mkdir(parents=True, exist_ok=True)
 
     delete_oldest_logs(list(pipx_log_dir.glob("cmd_*[0-9].log")), max_logs)
     delete_oldest_logs(list(pipx_log_dir.glob("cmd_*_pip_errors.log")), max_logs)
 
     datetime_str = time.strftime("%Y-%m-%d_%H.%M.%S")
@@ -795,18 +859,18 @@
         return _setup_log_file()
     except PermissionError:
         return _setup_log_file(platformdirs.user_log_path("pipx"))
 
 
 def setup_logging(verbose: int) -> None:
     pipx_str = bold(green("pipx >")) if sys.stdout.isatty() else "pipx >"
-    pipx.constants.pipx_log_file = setup_log_file()
+    paths.ctx.log_file = setup_log_file()
 
-    # Determine logging level
-    level_number = max(0, logging.WARNING - 10 * verbose)
+    # Determine logging level, a value between 0 and 50
+    level_number = min(max(0, logging.WARNING - 10 * verbose), 50)
 
     level = logging.getLevelName(level_number)
 
     # "incremental" is False so previous pytest tests don't accumulate handlers
     logging_config = {
         "version": 1,
         "formatters": {
@@ -831,15 +895,15 @@
                 "class": "logging.StreamHandler",
                 "formatter": "stream_verbose" if verbose else "stream_nonverbose",
                 "level": level,
             },
             "file": {
                 "class": "logging.FileHandler",
                 "formatter": "file",
-                "filename": str(pipx.constants.pipx_log_file),
+                "filename": str(paths.ctx.log_file),
                 "encoding": "utf-8",
                 "level": "DEBUG",
             },
         },
         "loggers": {"pipx": {"handlers": ["stream", "file"], "level": "DEBUG"}},
         "incremental": False,
     }
@@ -856,34 +920,39 @@
     setup_logging(verbose)
 
     logger.debug(f"{time.strftime('%Y-%m-%d %H:%M:%S')}")
     logger.debug(f"{' '.join(sys.argv)}")
     logger.info(f"pipx version is {__version__}")
     logger.info(f"Default python interpreter is '{DEFAULT_PYTHON}'")
 
-    mkdir(constants.PIPX_LOCAL_VENVS)
-    mkdir(constants.LOCAL_BIN_DIR)
-    mkdir(constants.LOCAL_MAN_DIR)
-    mkdir(constants.PIPX_VENV_CACHEDIR)
-
-    cachedir_tag = constants.PIPX_VENV_CACHEDIR / "CACHEDIR.TAG"
-    if not cachedir_tag.exists():
-        logger.debug("Adding CACHEDIR.TAG to cache directory")
-        signature = (
-            "Signature: 8a477f597d28d172789f06886806bc55\n"
-            "# This file is a cache directory tag created by pipx.\n"
-            "# For information about cache directory tags, see:\n"
-            "#       https://bford.info/cachedir/\n"
-        )
-        with open(cachedir_tag, "w") as file:
-            file.write(signature)
+    mkdir(paths.ctx.venvs)
+    mkdir(paths.ctx.bin_dir)
+    mkdir(paths.ctx.man_dir)
+    mkdir(paths.ctx.venv_cache)
+    mkdir(paths.ctx.standalone_python_cachedir)
+
+    for cachedir in [
+        paths.ctx.venv_cache,
+        paths.ctx.standalone_python_cachedir,
+    ]:
+        cachedir_tag = cachedir / "CACHEDIR.TAG"
+        if not cachedir_tag.exists():
+            logger.debug("Adding CACHEDIR.TAG to cache directory")
+            signature = (
+                "Signature: 8a477f597d28d172789f06886806bc55\n"
+                "# This file is a cache directory tag created by pipx.\n"
+                "# For information about cache directory tags, see:\n"
+                "#       https://bford.info/cachedir/\n"
+            )
+            with open(cachedir_tag, "w") as file:
+                file.write(signature)
 
-    rmdir(constants.PIPX_TRASH_DIR, False)
+    rmdir(paths.ctx.trash, False)
 
-    old_pipx_venv_location = constants.PIPX_LOCAL_VENVS / "pipx-app"
+    old_pipx_venv_location = paths.ctx.venvs / "pipx-app"
     if old_pipx_venv_location.exists():
         logger.warning(
             pipx_wrap(
                 f"""
                 {hazard}  A virtual environment for pipx was detected at
                 {str(old_pipx_venv_location)}. The 'pipx-app' package has been
                 renamed back to 'pipx'
@@ -906,23 +975,23 @@
             parsed_pipx_args.subparser.error("the following arguments are required: app")
 
 
 def cli() -> ExitCode:
     """Entry point from command line"""
     try:
         hide_cursor()
-        parser = get_command_parser()
+        parser, subparsers = get_command_parser()
         argcomplete.autocomplete(parser)
         parsed_pipx_args = parser.parse_args()
         setup(parsed_pipx_args)
         check_args(parsed_pipx_args)
         if not parsed_pipx_args.command:
             parser.print_help()
             return ExitCode(1)
-        return run_pipx_command(parsed_pipx_args)
+        return run_pipx_command(parsed_pipx_args, subparsers)
     except PipxError as e:
         print(str(e), file=sys.stderr)
         logger.debug(f"PipxError: {e}", exc_info=True)
         return ExitCode(1)
     except KeyboardInterrupt:
         return ExitCode(1)
     except Exception:
```

### Comparing `pipx-1.4.3/src/pipx/package_specifier.py` & `pipx-1.5.0/src/pipx/package_specifier.py`

 * *Files identical despite different names*

### Comparing `pipx-1.4.3/src/pipx/pipx_metadata_file.py` & `pipx-1.5.0/src/pipx/pipx_metadata_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,19 @@
     man_pages_of_dependencies: List[str] = []
     man_paths_of_dependencies: Dict[str, List[Path]] = {}
     suffix: str = ""
 
 
 class PipxMetadata:
     # Only change this if file format changes
-    __METADATA_VERSION__: str = "0.3"
+    # V0.1 -> original version
+    # V0.2 -> Improve handling of suffixes
+    # V0.3 -> Add man pages fields
+    # V0.4 -> Add source interpreter
+    __METADATA_VERSION__: str = "0.4"
 
     def __init__(self, venv_dir: Path, read: bool = True):
         self.venv_dir = venv_dir
         # We init this instance with reasonable fallback defaults for all
         #   members, EXCEPT for those we cannot know:
         #       self.main_package.package=None
         #       self.main_package.package_or_url=None
@@ -68,51 +72,59 @@
             man_pages=[],
             man_paths=[],
             man_pages_of_dependencies=[],
             man_paths_of_dependencies={},
             package_version="",
         )
         self.python_version: Optional[str] = None
+        self.source_interpreter: Optional[Path] = None
         self.venv_args: List[str] = []
         self.injected_packages: Dict[str, PackageInfo] = {}
 
         if read:
             self.read()
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "main_package": self.main_package._asdict(),
             "python_version": self.python_version,
+            "source_interpreter": self.source_interpreter,
             "venv_args": self.venv_args,
             "injected_packages": {name: data._asdict() for (name, data) in self.injected_packages.items()},
             "pipx_metadata_version": self.__METADATA_VERSION__,
         }
 
     def _convert_legacy_metadata(self, metadata_dict: Dict[str, Any]) -> Dict[str, Any]:
-        if metadata_dict["pipx_metadata_version"] in ("0.2", self.__METADATA_VERSION__):
-            return metadata_dict
+        if metadata_dict["pipx_metadata_version"] in (self.__METADATA_VERSION__):
+            pass
+        elif metadata_dict["pipx_metadata_version"] in ("0.2", "0.3"):
+            metadata_dict["source_interpreter"] = None
         elif metadata_dict["pipx_metadata_version"] == "0.1":
             main_package_data = metadata_dict["main_package"]
             if main_package_data["package"] != self.venv_dir.name:
                 # handle older suffixed packages gracefully
                 main_package_data["suffix"] = self.venv_dir.name.replace(main_package_data["package"], "")
-            return metadata_dict
+            metadata_dict["source_interpreter"] = None
         else:
             raise PipxError(
                 f"""
                 {self.venv_dir.name}: Unknown metadata version
                 {metadata_dict['pipx_metadata_version']}. Perhaps it was
                 installed with a later version of pipx.
                 """
             )
+        return metadata_dict
 
     def from_dict(self, input_dict: Dict[str, Any]) -> None:
         input_dict = self._convert_legacy_metadata(input_dict)
         self.main_package = PackageInfo(**input_dict["main_package"])
         self.python_version = input_dict["python_version"]
+        self.source_interpreter = (
+            Path(input_dict["source_interpreter"]) if input_dict.get("source_interpreter") else None
+        )
         self.venv_args = input_dict["venv_args"]
         self.injected_packages = {
             f"{name}{data.get('suffix', '')}": PackageInfo(**data)
             for (name, data) in input_dict["injected_packages"].items()
         }
 
     def _validate_before_write(self) -> None:
```

### Comparing `pipx-1.4.3/src/pipx/shared_libs.py` & `pipx-1.5.0/src/pipx/shared_libs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import logging
 import time
 from pathlib import Path
 from typing import List, Optional
 
-from pipx import constants
+from pipx import paths
 from pipx.animate import animate
 from pipx.constants import WINDOWS
 from pipx.interpreter import DEFAULT_PYTHON
 from pipx.util import (
     get_site_packages,
     get_venv_paths,
     run_subprocess,
@@ -19,40 +19,45 @@
 
 
 SHARED_LIBS_MAX_AGE_SEC = datetime.timedelta(days=30).total_seconds()
 
 
 class _SharedLibs:
     def __init__(self) -> None:
-        self.root = constants.PIPX_SHARED_LIBS
+        self.root = paths.ctx.shared_libs
         self.bin_path, self.python_path, self.man_path = get_venv_paths(self.root)
         self.pip_path = self.bin_path / ("pip" if not WINDOWS else "pip.exe")
         # i.e. bin_path is ~/.local/share/pipx/shared/bin
         # i.e. python_path is ~/.local/share/pipx/shared/python
         self._site_packages: Optional[Path] = None
         self.has_been_updated_this_run = False
         self.has_been_logged_this_run = False
-        self.skip_upgrade = False
 
     @property
     def site_packages(self) -> Path:
         if self._site_packages is None:
             self._site_packages = get_site_packages(self.python_path)
 
         return self._site_packages
 
-    def create(self, verbose: bool = False) -> None:
+    def create(self, pip_args: List[str], verbose: bool = False) -> None:
         if not self.is_valid:
             with animate("creating shared libraries", not verbose):
-                create_process = run_subprocess([DEFAULT_PYTHON, "-m", "venv", "--clear", self.root])
+                create_process = run_subprocess(
+                    [DEFAULT_PYTHON, "-m", "venv", "--clear", self.root], run_dir=str(self.root)
+                )
             subprocess_post_check(create_process)
+            # Recompute these paths, as they might resolve differently now, see comment in get_venv_paths
+            self.bin_path, self.python_path, self.man_path = get_venv_paths(self.root)
 
             # ignore installed packages to ensure no unexpected patches from the OS vendor
             # are used
-            self.upgrade(pip_args=["--force-reinstall"], verbose=verbose)
+            pip_args = pip_args or []
+            pip_args.append("--force-reinstall")
+            self.upgrade(pip_args=pip_args, verbose=verbose)
 
     @property
     def is_valid(self) -> bool:
         if self.python_path.is_file():
             check_pip = "import importlib.util; print(importlib.util.find_spec('pip'))"
             out = run_subprocess(
                 [self.python_path, "-c", check_pip],
@@ -62,15 +67,15 @@
 
             return self.pip_path.is_file() and out != "None"
         else:
             return False
 
     @property
     def needs_upgrade(self) -> bool:
-        if self.has_been_updated_this_run or self.skip_upgrade:
+        if self.has_been_updated_this_run:
             return False
 
         if not self.pip_path.is_file():
             return True
 
         now = time.time()
         time_since_last_update_sec = now - self.pip_path.stat().st_mtime
@@ -78,17 +83,17 @@
             logger.info(
                 f"Time since last upgrade of shared libs, in seconds: {time_since_last_update_sec:.0f}. "
                 f"Upgrade will be run by pipx if greater than {SHARED_LIBS_MAX_AGE_SEC:.0f}."
             )
             self.has_been_logged_this_run = True
         return time_since_last_update_sec > SHARED_LIBS_MAX_AGE_SEC
 
-    def upgrade(self, *, pip_args: Optional[List[str]] = None, verbose: bool = False) -> None:
+    def upgrade(self, *, pip_args: List[str], verbose: bool = False) -> None:
         if not self.is_valid:
-            self.create(verbose=verbose)
+            self.create(verbose=verbose, pip_args=pip_args)
             return
 
         # Don't try to upgrade multiple times per run
         if self.has_been_updated_this_run:
             logger.info(f"Already upgraded libraries in {self.root}")
             return
```

### Comparing `pipx-1.4.3/src/pipx/util.py` & `pipx-1.5.0/src/pipx/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     Optional,
     Pattern,
     Sequence,
     Tuple,
     Union,
 )
 
-import pipx.constants
+from pipx import paths
 from pipx.animate import show_cursor
-from pipx.constants import MINGW, PIPX_TRASH_DIR, WINDOWS
+from pipx.constants import MINGW, WINDOWS
 
 logger = logging.getLogger(__name__)
 
 
 class PipxError(Exception):
     def __init__(self, message: str, wrap_message: bool = True):
         if wrap_message:
@@ -38,29 +38,30 @@
 
 class RelevantSearch(NamedTuple):
     pattern: Pattern[str]
     category: str
 
 
 def _get_trash_file(path: Path) -> Path:
-    if not PIPX_TRASH_DIR.is_dir():
-        PIPX_TRASH_DIR.mkdir()
+    if not paths.ctx.trash.is_dir():
+        paths.ctx.trash.mkdir()
     prefix = "".join(random.choices(string.ascii_lowercase, k=8))
-    return PIPX_TRASH_DIR / f"{prefix}.{path.name}"
+    return paths.ctx.trash / f"{prefix}.{path.name}"
 
 
 def rmdir(path: Path, safe_rm: bool = True) -> None:
     if not path.is_dir():
         return
 
     logger.info(f"removing directory {path}")
-    try:
-        shutil.rmtree(path)
-    except FileNotFoundError:
-        pass
+    # Windows doesn't let us delete or overwrite files that are being run
+    # But it does let us rename/move it. To get around this issue, we can move
+    # the file to a temporary folder (to be deleted at a later time)
+    # So, if safe_rm is True, we ignore any errors and move the file to the trash with below code
+    shutil.rmtree(path, ignore_errors=safe_rm)
 
     # move it to be deleted later if it still exists
     if path.is_dir():
         if safe_rm:
             logger.warning(f"Failed to delete {path}. Will move it to a temp folder to delete later.")
 
             path.rename(_get_trash_file(path))
@@ -104,14 +105,18 @@
         extra_python_paths=[".", str(bin_path.parent.parent)],
     )
 
 
 if WINDOWS:
 
     def get_venv_paths(root: Path) -> Tuple[Path, Path, Path]:
+        # Make sure to use the real root path. This matters especially on Windows when using the packaged app
+        # (Microsoft Store) version of Python, which uses path redirection for sandboxing.
+        # See https://github.com/pypa/pipx/issues/1164
+        root = root.resolve()
         bin_path = root / "Scripts" if not MINGW else root / "bin"
         python_path = bin_path / "python.exe"
         man_path = root / "share" / "man"
         return bin_path, python_path, man_path
 
 else:
 
@@ -154,40 +159,39 @@
 def run_subprocess(
     cmd: Sequence[Union[str, Path]],
     capture_stdout: bool = True,
     capture_stderr: bool = True,
     log_cmd_str: Optional[str] = None,
     log_stdout: bool = True,
     log_stderr: bool = True,
+    run_dir: Optional[str] = None,
 ) -> "subprocess.CompletedProcess[str]":
     """Run arbitrary command as subprocess, capturing stderr and stout"""
     env = dict(os.environ)
     env = _fix_subprocess_env(env)
 
     if log_cmd_str is None:
         log_cmd_str = " ".join(str(c) for c in cmd)
     logger.info(f"running {log_cmd_str}")
+    if run_dir:
+        os.makedirs(run_dir, exist_ok=True)
     # windows cannot take Path objects, only strings
     cmd_str_list = [str(c) for c in cmd]
-    # Make sure to call the binary using its real path. This matters especially on Windows when using the packaged app
-    # (Microsoft Store) version of Python, which uses path redirection for sandboxing. If the path to the executable is
-    # redirected, the executable can get confused as to which directory it's being run from, leading to problems.
-    # See https://github.com/pypa/pipx/issues/1164
-    # Conversely, if the binary is a symlink, then we should NOT use the real path, as Python expects to receive the
-    # symlink in argv[0] so that it can locate the venv.
-    if not os.path.islink(cmd_str_list[0]) and WINDOWS:
-        cmd_str_list[0] = os.path.realpath(cmd_str_list[0])
+
+    # TODO: Switch to using `-P` / PYTHONSAFEPATH instead of running in
+    # separate directory in Python 3.11
     completed_process = subprocess.run(
         cmd_str_list,
         env=env,
         stdout=subprocess.PIPE if capture_stdout else None,
         stderr=subprocess.PIPE if capture_stderr else None,
         encoding="utf-8",
         universal_newlines=True,
         check=False,
+        cwd=run_dir,
     )
 
     if capture_stdout and log_stdout:
         logger.debug(f"stdout: {completed_process.stdout}".rstrip())
     if capture_stderr and log_stderr:
         logger.debug(f"stderr: {completed_process.stderr}".rstrip())
     logger.debug(f"returncode: {completed_process.returncode}")
@@ -203,15 +207,15 @@
             print(completed_process.stderr, file=sys.stderr, end="")
         if raise_error:
             raise PipxError(f"{' '.join([str(x) for x in completed_process.args])!r} failed")
         else:
             logger.info(f"{' '.join(completed_process.args)!r} failed")
 
 
-def dedup_ordered(input_list: List[Any]) -> List[Any]:
+def dedup_ordered(input_list: List[Tuple[str, Any]]) -> List[Tuple[str, Any]]:
     output_list = []
     seen = set()
     for x in input_list:
         if x[0] not in seen:
             output_list.append(x)
             seen.add(x[0])
 
@@ -322,17 +326,17 @@
 
 def subprocess_post_check_handle_pip_error(
     completed_process: "subprocess.CompletedProcess[str]",
 ) -> None:
     if completed_process.returncode:
         logger.info(f"{' '.join(completed_process.args)!r} failed")
         # Save STDOUT and STDERR to file in pipx/logs/
-        if pipx.constants.pipx_log_file is None:
+        if paths.ctx.log_file is None:
             raise PipxError("Pipx internal error: No log_file present.")
-        pip_error_file = pipx.constants.pipx_log_file.parent / (pipx.constants.pipx_log_file.stem + "_pip_errors.log")
+        pip_error_file = paths.ctx.log_file.parent / (paths.ctx.log_file.stem + "_pip_errors.log")
         with pip_error_file.open("w", encoding="utf-8") as pip_error_fh:
             print("PIP STDOUT", file=pip_error_fh)
             print("----------", file=pip_error_fh)
             if completed_process.stdout is not None:
                 print(completed_process.stdout, file=pip_error_fh, end="")
             print("\nPIP STDERR", file=pip_error_fh)
             print("----------", file=pip_error_fh)
@@ -413,7 +417,16 @@
     else:
         return textwrap.fill(
             text,
             width=width,
             subsequent_indent=subsequent_indent,
             break_on_hyphens=False,
         )
+
+
+def is_paths_relative(path: Path, parent: Path):
+    # Can be replaced with path.is_relative_to() if support for python3.8 is dropped
+    try:
+        path.resolve().relative_to(parent.resolve())
+        return True
+    except ValueError:
+        return False
```

### Comparing `pipx-1.4.3/src/pipx/venv.py` & `pipx-1.5.0/src/pipx/venv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import re
+import shutil
 import time
 from pathlib import Path
 from subprocess import CompletedProcess
 from typing import Dict, Generator, List, NoReturn, Optional, Set
 
 try:
     from importlib.metadata import Distribution, EntryPoint
@@ -72,18 +73,14 @@
                 continue
             yield entry
 
     def get_venv_dir(self, package_name: str) -> Path:
         """Return the expected venv path for given `package_name`."""
         return self._root.joinpath(canonicalize_name(package_name))
 
-    def verify_shared_libs(self) -> None:
-        for p in self.iter_venv_dirs():
-            Venv(p)
-
 
 class Venv:
     """Abstraction for a virtual environment with various useful methods for pipx"""
 
     def __init__(self, path: Path, *, verbose: bool = False, python: str = DEFAULT_PYTHON) -> None:
         self.root = path
         self.python = python
@@ -92,20 +89,29 @@
         self.verbose = verbose
         self.do_animation = not verbose
         try:
             self._existing = self.root.exists() and bool(next(self.root.iterdir()))
         except StopIteration:
             self._existing = False
 
+    def check_upgrade_shared_libs(self, verbose: bool, pip_args: List[str], force_upgrade: bool = False):
+        """
+        If necessary, run maintenance tasks to keep the shared libs up-to-date.
+
+        This can trigger `pip install`/`pip install --upgrade` operations,
+        so we expect the caller to provide sensible `pip_args`
+        ( provided by the user in the current CLI call
+        or retrieved from the metadata of a previous installation)
+        """
         if self._existing and self.uses_shared_libs:
             if shared_libs.is_valid:
-                if shared_libs.needs_upgrade:
-                    shared_libs.upgrade(verbose=verbose)
+                if force_upgrade or shared_libs.needs_upgrade:
+                    shared_libs.upgrade(verbose=verbose, pip_args=pip_args)
             else:
-                shared_libs.create(verbose)
+                shared_libs.create(verbose=verbose, pip_args=pip_args)
 
             if not shared_libs.is_valid:
                 raise PipxError(
                     pipx_wrap(
                         f"""
                         Error: pipx's shared venv {shared_libs.root} is invalid
                         and needs re-installation. To fix this, install or
@@ -153,18 +159,18 @@
         """
         override_shared -- Override installing shared libraries to the pipx shared directory (default False)
         """
         with animate("creating virtual environment", self.do_animation):
             cmd = [self.python, "-m", "venv"]
             if not override_shared:
                 cmd.append("--without-pip")
-            venv_process = run_subprocess(cmd + venv_args + [str(self.root)])
+            venv_process = run_subprocess(cmd + venv_args + [str(self.root)], run_dir=str(self.root))
         subprocess_post_check(venv_process)
 
-        shared_libs.create(self.verbose)
+        shared_libs.create(verbose=self.verbose, pip_args=pip_args)
         if not override_shared:
             pipx_pth = get_site_packages(self.python_path) / PIPX_SHARED_PTH
             # write path pointing to the shared libs site-packages directory
             # example pipx_pth location:
             #   ~/.local/share/pipx/venvs/black/lib/python3.8/site-packages/pipx_shared.pth
             # example shared_libs.site_packages location:
             #   ~/.local/share/pipx/shared/lib/python3.6/site-packages
@@ -172,14 +178,17 @@
             # https://docs.python.org/3/library/site.html
             # A path configuration file is a file whose name has the form 'name.pth'.
             # its contents are additional items (one per line) to be added to sys.path
             pipx_pth.write_text(f"{shared_libs.site_packages}\n", encoding="utf-8")
 
         self.pipx_metadata.venv_args = venv_args
         self.pipx_metadata.python_version = self.get_python_version()
+        source_interpreter = shutil.which(self.python)
+        if source_interpreter:
+            self.pipx_metadata.source_interpreter = Path(source_interpreter)
 
     def safe_to_remove(self) -> bool:
         return not self._existing
 
     def remove_venv(self) -> None:
         if self.safe_to_remove():
             rmdir(self.root)
@@ -244,15 +253,15 @@
                 "--no-input",
                 "install",
                 *pip_args,
                 package_or_url,
             ]
             # no logging because any errors will be specially logged by
             #   subprocess_post_check_handle_pip_error()
-            pip_process = run_subprocess(cmd, log_stdout=False, log_stderr=False)
+            pip_process = run_subprocess(cmd, log_stdout=False, log_stderr=False, run_dir=str(self.root))
         subprocess_post_check_handle_pip_error(pip_process)
         if pip_process.returncode:
             raise PipxError(f"Error installing {full_package_description(package_name, package_or_url)}.")
 
         self._update_package_metadata(
             package_name=package_name,
             package_or_url=package_or_url,
@@ -288,15 +297,15 @@
                 "--no-input",
                 "install",
                 *pip_args,
                 *requirements,
             ]
             # no logging because any errors will be specially logged by
             #   subprocess_post_check_handle_pip_error()
-            pip_process = run_subprocess(cmd, log_stdout=False, log_stderr=False)
+            pip_process = run_subprocess(cmd, log_stdout=False, log_stderr=False, run_dir=str(self.root))
         subprocess_post_check_handle_pip_error(pip_process)
         if pip_process.returncode:
             raise PipxError(f"Error installing {', '.join(requirements)}.")
 
     def install_package_no_deps(self, package_or_url: str, pip_args: List[str]) -> str:
         with animate(f"determining package name from {package_or_url!r}", self.do_animation):
             old_package_set = self.list_installed_packages()
@@ -450,15 +459,15 @@
             suffix=suffix,
         )
 
     def _run_pip(self, cmd: List[str]) -> "CompletedProcess[str]":
         cmd = [str(self.python_path), "-m", "pip"] + cmd
         if not self.verbose:
             cmd.append("-q")
-        return run_subprocess(cmd)
+        return run_subprocess(cmd, run_dir=str(self.root))
 
     def run_pip_get_exit_code(self, cmd: List[str]) -> ExitCode:
         cmd = [str(self.python_path), "-m", "pip"] + cmd
         if not self.verbose:
             cmd.append("-q")
         returncode = run_subprocess(cmd, capture_stdout=False, capture_stderr=False).returncode
         if returncode:
```

### Comparing `pipx-1.4.3/src/pipx/venv_inspect.py` & `pipx-1.5.0/src/pipx/venv_inspect.py`

 * *Files identical despite different names*

### Comparing `pipx-1.4.3/src/pipx/commands/__init__.py` & `pipx-1.5.0/src/pipx/commands/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pipx.commands.ensure_path import ensure_pipx_paths
 from pipx.commands.environment import environment
 from pipx.commands.inject import inject
 from pipx.commands.install import install
+from pipx.commands.interpreter import list_interpreters, prune_interpreters
 from pipx.commands.list_packages import list_packages
 from pipx.commands.reinstall import reinstall, reinstall_all
 from pipx.commands.run import run
 from pipx.commands.run_pip import run_pip
 from pipx.commands.uninject import uninject
 from pipx.commands.uninstall import uninstall, uninstall_all
 from pipx.commands.upgrade import upgrade, upgrade_all
@@ -21,8 +22,10 @@
     "uninstall_all",
     "reinstall",
     "reinstall_all",
     "list_packages",
     "run_pip",
     "ensure_pipx_paths",
     "environment",
+    "list_interpreters",
+    "prune_interpreters",
 ]
```

### Comparing `pipx-1.4.3/src/pipx/commands/common.py` & `pipx-1.5.0/src/pipx/commands/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from shutil import which
 from tempfile import TemporaryDirectory
 from typing import Dict, List, Optional, Set, Tuple
 
 import userpath  # type: ignore
 from packaging.utils import canonicalize_name
 
-from pipx import constants
+from pipx import paths
 from pipx.colors import bold, red
 from pipx.constants import MAN_SECTIONS, WINDOWS
 from pipx.emojis import hazard, stars
 from pipx.package_specifier import parse_specifier_for_install, valid_pypi_name
 from pipx.pipx_metadata_file import PackageInfo
 from pipx.util import PipxError, mkdir, pipx_wrap, rmdir, safe_unlink
 from pipx.venv import Venv
@@ -227,36 +227,43 @@
     man_pages = package_metadata.man_pages
     if package_metadata.include_dependencies:
         apps += package_metadata.apps_of_dependencies
         man_pages += package_metadata.man_pages_of_dependencies
 
     exposed_app_paths = get_exposed_paths_for_package(
         venv.bin_path,
-        constants.LOCAL_BIN_DIR,
+        paths.ctx.bin_dir,
         [add_suffix(app, package_metadata.suffix) for app in apps],
     )
     exposed_binary_names = sorted(p.name for p in exposed_app_paths)
     unavailable_binary_names = sorted(
         {add_suffix(name, package_metadata.suffix) for name in package_metadata.apps} - set(exposed_binary_names)
     )
     exposed_man_paths = set()
     for man_section in MAN_SECTIONS:
         exposed_man_paths |= get_exposed_man_paths_for_package(
             venv.man_path / man_section,
-            constants.LOCAL_MAN_DIR / man_section,
+            paths.ctx.man_dir / man_section,
             man_pages,
         )
     exposed_man_pages = sorted(str(Path(p.parent.name) / p.name) for p in exposed_man_paths)
     unavailable_man_pages = sorted(set(package_metadata.man_pages) - set(exposed_man_pages))
     # The following is to satisfy mypy that python_version is str and not
     #   Optional[str]
     python_version = venv.pipx_metadata.python_version if venv.pipx_metadata.python_version is not None else ""
+    source_interpreter = venv.pipx_metadata.source_interpreter
+    is_standalone = (
+        str(source_interpreter).startswith(str(paths.ctx.standalone_python_cachedir.resolve()))
+        if source_interpreter
+        else False
+    )
     return (
         _get_list_output(
             python_version,
+            is_standalone,
             package_metadata.package_version,
             package_name,
             new_install,
             exposed_binary_names,
             unavailable_binary_names,
             exposed_man_pages,
             unavailable_man_pages,
@@ -318,14 +325,15 @@
             if name.startswith(prefix)
         ],
     )
 
 
 def _get_list_output(
     python_version: str,
+    python_is_standalone: bool,
     package_version: str,
     package_name: str,
     new_install: bool,
     exposed_binary_names: List[str],
     unavailable_binary_names: List[str],
     exposed_man_pages: List[str],
     unavailable_man_pages: List[str],
@@ -333,14 +341,15 @@
     suffix: str = "",
 ) -> str:
     output = []
     suffix = f" ({bold(shlex.quote(package_name + suffix))})" if suffix else ""
     output.append(
         f"  {'installed' if new_install else ''} package {bold(shlex.quote(package_name))}"
         f" {bold(package_version)}{suffix}, installed using {python_version}"
+        + (" (standalone)" if python_is_standalone else "")
     )
 
     if new_install and (exposed_binary_names or unavailable_binary_names):
         output.append("  These apps are now globally available")
     for name in exposed_binary_names:
         output.append(f"    - {name}")
     for name in unavailable_binary_names:
```

### Comparing `pipx-1.4.3/src/pipx/commands/ensure_path.py` & `pipx-1.5.0/src/pipx/commands/ensure_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import site
 import sys
 from pathlib import Path
 from typing import Optional, Tuple
 
 import userpath  # type: ignore
 
-from pipx import constants
+from pipx import paths
 from pipx.constants import EXIT_CODE_OK, ExitCode
 from pipx.emojis import hazard, stars
 from pipx.util import pipx_wrap
 
 logger = logging.getLogger(__name__)
 
 
@@ -93,15 +93,15 @@
         print(pipx_wrap(f"{location_str} is already in PATH.", subsequent_indent=" " * 4))
 
     return (path_added, need_shell_restart)
 
 
 def ensure_pipx_paths(force: bool) -> ExitCode:
     """Returns pipx exit code."""
-    bin_paths = {constants.LOCAL_BIN_DIR}
+    bin_paths = {paths.ctx.bin_dir}
 
     pipx_user_bin_path = get_pipx_user_bin_path()
     if pipx_user_bin_path is not None:
         bin_paths.add(pipx_user_bin_path)
 
     path_added = False
     need_shell_restart = False
```

### Comparing `pipx-1.4.3/src/pipx/commands/environment.py` & `pipx-1.5.0/src/pipx/commands/environment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 import os
 
-from pipx.constants import (
-    EXIT_CODE_OK,
-    LOCAL_BIN_DIR,
-    LOCAL_MAN_DIR,
-    PIPX_HOME,
-    PIPX_LOCAL_VENVS,
-    PIPX_LOG_DIR,
-    PIPX_SHARED_LIBS,
-    PIPX_TRASH_DIR,
-    PIPX_VENV_CACHEDIR,
-    ExitCode,
-)
+from pipx import paths
+from pipx.constants import EXIT_CODE_OK, ExitCode
 from pipx.emojis import EMOJI_SUPPORT
 from pipx.interpreter import DEFAULT_PYTHON
 from pipx.util import PipxError
 
 
 def environment(value: str) -> ExitCode:
     """Print a list of environment variables and paths used by pipx"""
     environment_variables = [
         "PIPX_HOME",
         "PIPX_BIN_DIR",
         "PIPX_MAN_DIR",
         "PIPX_SHARED_LIBS",
         "PIPX_DEFAULT_PYTHON",
+        "PIPX_FETCH_MISSING_PYTHON",
         "USE_EMOJI",
     ]
     derived_values = {
-        "PIPX_HOME": PIPX_HOME,
-        "PIPX_BIN_DIR": LOCAL_BIN_DIR,
-        "PIPX_MAN_DIR": LOCAL_MAN_DIR,
-        "PIPX_SHARED_LIBS": PIPX_SHARED_LIBS,
-        "PIPX_LOCAL_VENVS": PIPX_LOCAL_VENVS,
-        "PIPX_LOG_DIR": PIPX_LOG_DIR,
-        "PIPX_TRASH_DIR": PIPX_TRASH_DIR,
-        "PIPX_VENV_CACHEDIR": PIPX_VENV_CACHEDIR,
+        "PIPX_HOME": paths.ctx.home,
+        "PIPX_BIN_DIR": paths.ctx.bin_dir,
+        "PIPX_MAN_DIR": paths.ctx.man_dir,
+        "PIPX_SHARED_LIBS": paths.ctx.shared_libs,
+        "PIPX_LOCAL_VENVS": paths.ctx.venvs,
+        "PIPX_LOG_DIR": paths.ctx.logs,
+        "PIPX_TRASH_DIR": paths.ctx.trash,
+        "PIPX_VENV_CACHEDIR": paths.ctx.venv_cache,
+        "PIPX_STANDALONE_PYTHON_CACHEDIR": paths.ctx.standalone_python_cachedir,
         "PIPX_DEFAULT_PYTHON": DEFAULT_PYTHON,
         "USE_EMOJI": str(EMOJI_SUPPORT).lower(),
     }
     if value is None:
         print("Environment variables (set by user):")
         print("")
         for env_variable in environment_variables:
```

### Comparing `pipx-1.4.3/src/pipx/commands/inject.py` & `pipx-1.5.0/src/pipx/commands/inject.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from pathlib import Path
 from typing import List, Optional
 
-from pipx import constants
+from pipx import paths
 from pipx.colors import bold
 from pipx.commands.common import package_name_from_spec, run_post_install_actions
 from pipx.constants import EXIT_CODE_INJECT_ERROR, EXIT_CODE_OK, ExitCode
 from pipx.emojis import stars
 from pipx.util import PipxError
 from pipx.venv import Venv
 
@@ -30,14 +30,15 @@
             Can't inject {package_spec!r} into nonexistent Virtual Environment
             {venv_dir.name!r}. Be sure to install the package first with 'pipx
             install {venv_dir.name}' before injecting into it.
             """
         )
 
     venv = Venv(venv_dir, verbose=verbose)
+    venv.check_upgrade_shared_libs(pip_args=pip_args, verbose=verbose)
 
     if not venv.package_metadata:
         raise PipxError(
             f"""
             Can't inject {package_spec!r} into Virtual Environment
             {venv.name!r}. {venv.name!r} has missing internal pipx metadata. It
             was likely installed using a pipx version before 0.15.0.0. Please
@@ -67,16 +68,16 @@
         is_main_package=False,
         suffix=venv_suffix,
     )
     if include_apps:
         run_post_install_actions(
             venv,
             package_name,
-            constants.LOCAL_BIN_DIR,
-            constants.LOCAL_MAN_DIR,
+            paths.ctx.bin_dir,
+            paths.ctx.man_dir,
             venv_dir,
             include_dependencies,
             force=force,
         )
 
     print(f"  injected package {bold(package_name)} into venv {bold(venv.name)}")
     print(f"done! {stars}", file=sys.stderr)
```

### Comparing `pipx-1.4.3/src/pipx/commands/install.py` & `pipx-1.5.0/src/pipx/commands/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import List, Optional
 
-from pipx import constants
+from pipx import paths
 from pipx.commands.common import package_name_from_spec, run_post_install_actions
 from pipx.constants import (
     EXIT_CODE_INSTALL_VENV_EXISTS,
     EXIT_CODE_OK,
     ExitCode,
 )
 from pipx.interpreter import DEFAULT_PYTHON
@@ -42,23 +42,24 @@
         package_names = [
             package_name_from_spec(package_spec, python, pip_args=pip_args, verbose=verbose)
             for package_spec in package_specs
         ]
 
     for package_name, package_spec in zip(package_names, package_specs):
         if venv_dir is None:
-            venv_container = VenvContainer(constants.PIPX_LOCAL_VENVS)
+            venv_container = VenvContainer(paths.ctx.venvs)
             venv_dir = venv_container.get_venv_dir(f"{package_name}{suffix}")
 
         try:
             exists = venv_dir.exists() and bool(next(venv_dir.iterdir()))
         except StopIteration:
             exists = False
 
         venv = Venv(venv_dir, python=python, verbose=verbose)
+        venv.check_upgrade_shared_libs(pip_args=pip_args, verbose=verbose)
         if exists:
             if not reinstall and force and python_flag_was_passed:
                 print(
                     pipx_wrap(
                         f"""
                         --python is ignored when --force is passed.
                         If you want to reinstall {package_name} with {python},
```

### Comparing `pipx-1.4.3/src/pipx/commands/list_packages.py` & `pipx-1.5.0/src/pipx/commands/list_packages.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import sys
 from pathlib import Path
 from typing import Any, Collection, Dict, Tuple
 
-from pipx import constants, shared_libs
+from pipx import paths
 from pipx.colors import bold
 from pipx.commands.common import VenvProblems, get_venv_summary, venv_health_check
 from pipx.constants import EXIT_CODE_LIST_PROBLEM, EXIT_CODE_OK, ExitCode
 from pipx.emojis import sleep
 from pipx.pipx_metadata_file import JsonEncoderHandlesPath, PipxMetadata
 from pipx.venv import Venv, VenvContainer
 
@@ -41,16 +41,16 @@
         all_venv_problems.or_(venv_problems)
 
     return all_venv_problems
 
 
 def list_text(venv_dirs: Collection[Path], include_injected: bool, venv_root_dir: str) -> VenvProblems:
     print(f"venvs are in {bold(venv_root_dir)}")
-    print(f"apps are exposed on your $PATH at {bold(str(constants.LOCAL_BIN_DIR))}")
-    print(f"manual pages are exposed at {bold(str(constants.LOCAL_MAN_DIR))}")
+    print(f"apps are exposed on your $PATH at {bold(str(paths.ctx.bin_dir))}")
+    print(f"manual pages are exposed at {bold(str(paths.ctx.man_dir))}")
 
     all_venv_problems = VenvProblems()
     for venv_dir in venv_dirs:
         package_summary, venv_problems = get_venv_summary(venv_dir, include_injected=include_injected)
         if venv_problems.any_():
             logger.warning(package_summary)
         else:
@@ -85,27 +85,20 @@
 
 
 def list_packages(
     venv_container: VenvContainer,
     include_injected: bool,
     json_format: bool,
     short_format: bool,
-    skip_maintenance: bool,
 ) -> ExitCode:
     """Returns pipx exit code."""
     venv_dirs: Collection[Path] = sorted(venv_container.iter_venv_dirs())
     if not venv_dirs:
         print(f"nothing has been installed with pipx {sleep}", file=sys.stderr)
 
-    if skip_maintenance:
-        shared_libs.shared_libs.skip_upgrade = True
-        logger.info("Skipping shared libs maintenance tasks")
-
-    venv_container.verify_shared_libs()
-
     if json_format:
         all_venv_problems = list_json(venv_dirs)
     elif short_format:
         all_venv_problems = list_short(venv_dirs)
     else:
         if not venv_dirs:
             return EXIT_CODE_OK
```

### Comparing `pipx-1.4.3/src/pipx/commands/reinstall.py` & `pipx-1.5.0/src/pipx/commands/reinstall.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
 from pathlib import Path
 from typing import List, Sequence
 
 from packaging.utils import canonicalize_name
 
-import pipx.shared_libs  # import instead of from so mockable in tests
 from pipx.commands.inject import inject_dep
 from pipx.commands.install import install
 from pipx.commands.uninstall import uninstall
 from pipx.constants import (
     EXIT_CODE_OK,
     EXIT_CODE_REINSTALL_INVALID_PYTHON,
     EXIT_CODE_REINSTALL_VENV_NONEXISTENT,
@@ -22,14 +21,15 @@
 def reinstall(
     *,
     venv_dir: Path,
     local_bin_dir: Path,
     local_man_dir: Path,
     python: str,
     verbose: bool,
+    force_reinstall_shared_libs: bool = False,
 ) -> ExitCode:
     """Returns pipx exit code."""
     if not venv_dir.exists():
         print(f"Nothing to reinstall for {venv_dir.name} {sleep}")
         return EXIT_CODE_REINSTALL_VENV_NONEXISTENT
 
     try:
@@ -40,14 +40,17 @@
         print(
             f"{error} Error, the python executable would be deleted!",
             "Change it using the --python option or PIPX_DEFAULT_PYTHON environment variable.",
         )
         return EXIT_CODE_REINSTALL_INVALID_PYTHON
 
     venv = Venv(venv_dir, verbose=verbose)
+    venv.check_upgrade_shared_libs(
+        pip_args=venv.pipx_metadata.main_package.pip_args, verbose=verbose, force_upgrade=force_reinstall_shared_libs
+    )
 
     if venv.pipx_metadata.main_package.package_or_url is not None:
         package_or_url = venv.pipx_metadata.main_package.package_or_url
     else:
         package_or_url = venv.main_package_name
 
     uninstall(venv_dir, local_bin_dir, local_man_dir, verbose)
@@ -100,31 +103,36 @@
     local_man_dir: Path,
     python: str,
     verbose: bool,
     *,
     skip: Sequence[str],
 ) -> ExitCode:
     """Returns pipx exit code."""
-    pipx.shared_libs.shared_libs.upgrade(verbose=verbose)
-
     failed: List[str] = []
+
+    # iterate on all packages and reinstall them
+    # for the first one, we also trigger
+    # a reinstall of shared libs beforehand
+    first_reinstall = True
     for venv_dir in venv_container.iter_venv_dirs():
         if venv_dir.name in skip:
             continue
         try:
             package_exit = reinstall(
                 venv_dir=venv_dir,
                 local_bin_dir=local_bin_dir,
                 local_man_dir=local_man_dir,
                 python=python,
                 verbose=verbose,
+                force_reinstall_shared_libs=first_reinstall,
             )
         except PipxError as e:
             print(e, file=sys.stderr)
             failed.append(venv_dir.name)
         else:
+            first_reinstall = False
             if package_exit != 0:
                 failed.append(venv_dir.name)
     if len(failed) > 0:
         raise PipxError(f"The following package(s) failed to reinstall: {', '.join(failed)}")
     # Any failure to install will raise PipxError, otherwise success
     return EXIT_CODE_OK
```

### Comparing `pipx-1.4.3/src/pipx/commands/run.py` & `pipx-1.5.0/src/pipx/commands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import urllib.request
 from pathlib import Path
 from shutil import which
 from typing import List, NoReturn, Optional, Union
 
 from packaging.requirements import InvalidRequirement, Requirement
 
-from pipx import constants
+from pipx import paths
 from pipx.commands.common import package_name_from_spec
 from pipx.constants import TEMP_VENV_EXPIRATION_THRESHOLD_DAYS, WINDOWS
 from pipx.emojis import hazard
 from pipx.util import (
     PipxError,
     exec_app,
     get_pypackage_bin_path,
@@ -93,14 +93,15 @@
         venv_dir = _get_temporary_venv_path(requirements, python, pip_args, venv_args)
         venv = Venv(venv_dir)
         _prepare_venv_cache(venv, None, use_cache)
         if venv_dir.exists():
             logger.info(f"Reusing cached venv {venv_dir}")
         else:
             venv = Venv(venv_dir, python=python, verbose=verbose)
+            venv.check_upgrade_shared_libs(pip_args=pip_args, verbose=verbose)
             venv.create_venv(venv_args, pip_args)
             venv.install_unmanaged_packages(requirements, pip_args)
         python_path = venv.python_path
 
     if isinstance(content, Path):
         exec_app([python_path, content, *app_args])
     else:
@@ -224,14 +225,15 @@
     python: str,
     pip_args: List[str],
     venv_args: List[str],
     use_cache: bool,
     verbose: bool,
 ) -> NoReturn:
     venv = Venv(venv_dir, python=python, verbose=verbose)
+    venv.check_upgrade_shared_libs(pip_args=pip_args, verbose=verbose)
 
     if venv.pipx_metadata.main_package.package is not None:
         package_name = venv.pipx_metadata.main_package.package
     else:
         package_name = package_name_from_spec(package_or_url, python, pip_args=pip_args, verbose=verbose)
 
     override_shared = package_name == "pip"
@@ -284,15 +286,15 @@
     """
     m = hashlib.sha256()
     m.update("".join(requirements).encode())
     m.update(python.encode())
     m.update("".join(pip_args).encode())
     m.update("".join(venv_args).encode())
     venv_folder_name = m.hexdigest()[:15]  # 15 chosen arbitrarily
-    return Path(constants.PIPX_VENV_CACHEDIR) / venv_folder_name
+    return Path(paths.ctx.venv_cache) / venv_folder_name
 
 
 def _is_temporary_venv_expired(venv_dir: Path) -> bool:
     created_time_sec = venv_dir.stat().st_ctime
     current_time_sec = time.mktime(datetime.datetime.now().timetuple())
     age = current_time_sec - created_time_sec
     expiration_threshold_sec = 60 * 60 * 24 * TEMP_VENV_EXPIRATION_THRESHOLD_DAYS
@@ -304,15 +306,15 @@
     if not use_cache and (bin_path is None or bin_path.exists()):
         logger.info(f"Removing cached venv {str(venv_dir)}")
         rmdir(venv_dir)
     _remove_all_expired_venvs()
 
 
 def _remove_all_expired_venvs() -> None:
-    for venv_dir in Path(constants.PIPX_VENV_CACHEDIR).iterdir():
+    for venv_dir in Path(paths.ctx.venv_cache).iterdir():
         if _is_temporary_venv_expired(venv_dir):
             logger.info(f"Removing expired venv {str(venv_dir)}")
             rmdir(venv_dir)
 
 
 def _http_get_request(url: str) -> str:
     try:
```

### Comparing `pipx-1.4.3/src/pipx/commands/run_pip.py` & `pipx-1.5.0/src/pipx/commands/run_pip.py`

 * *Files identical despite different names*

### Comparing `pipx-1.4.3/src/pipx/commands/uninject.py` & `pipx-1.5.0/src/pipx/commands/uninject.py`

 * *Files identical despite different names*

### Comparing `pipx-1.4.3/src/pipx/commands/uninstall.py` & `pipx-1.5.0/src/pipx/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pipx-1.4.3/src/pipx/commands/upgrade.py` & `pipx-1.5.0/src/pipx/commands/upgrade.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
+import os
 from pathlib import Path
-from typing import List, Sequence
+from typing import List, Optional, Sequence
 
-from pipx import constants
+from pipx import commands, paths
 from pipx.colors import bold, red
 from pipx.commands.common import expose_resources_globally
 from pipx.constants import EXIT_CODE_OK, ExitCode
 from pipx.emojis import sleep
 from pipx.package_specifier import parse_specifier_for_upgrade
 from pipx.util import PipxError, pipx_wrap
 from pipx.venv import Venv, VenvContainer
@@ -45,32 +46,32 @@
 
     display_name = f"{package_metadata.package}{package_metadata.suffix}"
     new_version = package_metadata.package_version
 
     if package_metadata.include_apps:
         expose_resources_globally(
             "app",
-            constants.LOCAL_BIN_DIR,
+            paths.ctx.bin_dir,
             package_metadata.app_paths,
             force=force,
             suffix=package_metadata.suffix,
         )
-        expose_resources_globally("man", constants.LOCAL_MAN_DIR, package_metadata.man_paths, force=force)
+        expose_resources_globally("man", paths.ctx.man_dir, package_metadata.man_paths, force=force)
 
     if package_metadata.include_dependencies:
         for _, app_paths in package_metadata.app_paths_of_dependencies.items():
             expose_resources_globally(
                 "app",
-                constants.LOCAL_BIN_DIR,
+                paths.ctx.bin_dir,
                 app_paths,
                 force=force,
                 suffix=package_metadata.suffix,
             )
         for _, man_paths in package_metadata.man_paths_of_dependencies.items():
-            expose_resources_globally("man", constants.LOCAL_MAN_DIR, man_paths, force=force)
+            expose_resources_globally("man", paths.ctx.man_dir, man_paths, force=force)
 
     if old_version == new_version:
         if upgrading_all:
             pass
         else:
             print(
                 pipx_wrap(
@@ -97,25 +98,49 @@
     venv_dir: Path,
     pip_args: List[str],
     verbose: bool,
     *,
     include_injected: bool,
     upgrading_all: bool,
     force: bool,
+    install: bool = False,
+    python: Optional[str] = None,
 ) -> int:
-    """Returns number of packages with changed versions."""
+    """Return number of packages with changed versions."""
     if not venv_dir.is_dir():
-        raise PipxError(
-            f"""
-            Package is not installed. Expected to find {str(venv_dir)}, but it
-            does not exist.
-            """
-        )
+        if install:
+            commands.install(
+                venv_dir=None,
+                venv_args=[],
+                package_names=None,
+                package_specs=[str(venv_dir).split(os.path.sep)[-1]],
+                local_bin_dir=paths.ctx.bin_dir,
+                local_man_dir=paths.ctx.man_dir,
+                python=python,
+                pip_args=pip_args,
+                verbose=verbose,
+                force=force,
+                reinstall=False,
+                include_dependencies=False,
+                preinstall_packages=None,
+            )
+            return 0
+        else:
+            raise PipxError(
+                f"""
+                Package is not installed. Expected to find {str(venv_dir)}, but it
+                does not exist.
+                """
+            )
+
+    if python and not install:
+        logger.info("Ignoring --python as not combined with --install")
 
     venv = Venv(venv_dir, verbose=verbose)
+    venv.check_upgrade_shared_libs(pip_args=pip_args, verbose=verbose)
 
     if not venv.package_metadata:
         raise PipxError(
             f"Not upgrading {red(bold(venv_dir.name))}. It has missing internal pipx metadata.\n"
             f"It was likely installed using a pipx version before 0.15.0.0.\n"
             f"Please uninstall and install this package to fix.",
             wrap_message=False,
@@ -150,55 +175,61 @@
             )
 
     return versions_updated
 
 
 def upgrade(
     venv_dir: Path,
+    python: Optional[str],
     pip_args: List[str],
     verbose: bool,
     *,
     include_injected: bool,
     force: bool,
+    install: bool,
 ) -> ExitCode:
-    """Returns pipx exit code."""
+    """Return pipx exit code."""
 
     _ = _upgrade_venv(
         venv_dir,
         pip_args,
         verbose,
         include_injected=include_injected,
         upgrading_all=False,
         force=force,
+        install=install,
+        python=python,
     )
 
     # Any error in upgrade will raise PipxError (e.g. from venv.upgrade_package())
     return EXIT_CODE_OK
 
 
 def upgrade_all(
     venv_container: VenvContainer,
     verbose: bool,
     *,
+    pip_args: List[str],
     include_injected: bool,
     skip: Sequence[str],
     force: bool,
 ) -> ExitCode:
     """Returns pipx exit code."""
     venv_error = False
     venvs_upgraded = 0
     for venv_dir in venv_container.iter_venv_dirs():
         venv = Venv(venv_dir, verbose=verbose)
+        venv.check_upgrade_shared_libs(pip_args=pip_args, verbose=verbose)
         if venv_dir.name in skip or "--editable" in venv.pipx_metadata.main_package.pip_args:
             continue
         try:
             venvs_upgraded += _upgrade_venv(
                 venv_dir,
                 venv.pipx_metadata.main_package.pip_args,
-                verbose,
+                verbose=verbose,
                 include_injected=include_injected,
                 upgrading_all=True,
                 force=force,
             )
 
         except PipxError as e:
             venv_error = True
```

### Comparing `pipx-1.4.3/LICENSE` & `pipx-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipx-1.4.3/README.md` & `pipx-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+Metadata-Version: 2.3
+Name: pipx
+Version: 1.5.0
+Summary: Install and Run Python Applications in Isolated Environments
+Project-URL: Bug Tracker, https://github.com/pypa/pipx/issues
+Project-URL: Documentation, https://pipx.pypa.io
+Project-URL: Homepage, https://pipx.pypa.io
+Project-URL: Release Notes, https://pipx.pypa.io/latest/changelog/
+Project-URL: Source Code, https://github.com/pypa/pipx
+Author-email: Chad Smith <chadsmith.software@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: Virtual Environment,cli,install,pip,workflow
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Requires-Dist: argcomplete>=1.9.4
+Requires-Dist: colorama>=0.4.4; sys_platform == 'win32'
+Requires-Dist: packaging>=20
+Requires-Dist: platformdirs>=2.1
+Requires-Dist: tomli; python_version < '3.11'
+Requires-Dist: userpath!=1.9.0,>=1.6
+Description-Content-Type: text/markdown
+
 <p align="center">
 <a href="https://pipx.pypa.io">
 <img align="center" src="https://github.com/pypa/pipx/raw/main/logo.svg" width="200"/>
 </a>
 </p>
 
 # pipx — Install and Run Python Applications in Isolated Environments
@@ -23,41 +54,54 @@
 **Source Code**: <https://github.com/pypa/pipx>
 
 _For comparison to other tools including pipsi, see
 [Comparison to Other Tools](https://pipx.pypa.io/stable/comparisons/)._
 
 ## Install pipx
 
-> [!NOTE] It is not recommended to install `pipx` via `pipx`. If you'd like to do this anyway, take a look at the
+> [!WARNING]
+>
+> It is not recommended to install `pipx` via `pipx`. If you'd like to do this anyway, take a look at the
 > [`pipx-in-pipx`](https://github.com/mattsb42-meta/pipx-in-pipx) project and read about the limitations there.
 
 ### On macOS
 
 ```
 brew install pipx
 pipx ensurepath
+sudo pipx ensurepath --global # optional to allow pipx actions with --global argument
 ```
 
 Upgrade pipx with `brew update && brew upgrade pipx`.
 
 ### On Linux
 
 - Ubuntu 23.04 or above
 
 ```
 sudo apt update
 sudo apt install pipx
 pipx ensurepath
+sudo pipx ensurepath --global # optional to allow pipx actions with --global argument
+```
+
+- Fedora:
+
+```
+sudo dnf install pipx
+pipx ensurepath
+sudo pipx ensurepath --global # optional to allow pipx actions with --global argument
 ```
 
-- Ubuntu 22.04 or below
+- Using `pip` on other distributions:
 
 ```
 python3 -m pip install --user pipx
 python3 -m pipx ensurepath
+sudo pipx ensurepath --global # optional to allow pipx actions with --global argument
 ```
 
 Upgrade pipx with `python3 -m pip install --user --upgrade pipx`.
 
 ### On Windows
 
 - install via [Scoop](https://scoop.sh/)
@@ -144,16 +188,16 @@
 
 pipx is a tool to install and run any of these thousands of application-containing packages in a safe, convenient, and
 reliable way. **In a way, it turns Python Package Index (PyPI) into a big app store for Python applications.** Not all
 Python packages have entry points, but many do.
 
 If you would like to make your package compatible with pipx, all you need to do is add a
 [console scripts](https://python-packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-scripts-entry-point)
-entry point. If you're a poetry user, use [these instructions](https://python-poetry.org/docs/pyproject/#scripts). Or
-you're using hatch, [try this](https://hatch.pypa.io/latest/config/metadata/#cli).
+entry point. If you're a poetry user, use [these instructions](https://python-poetry.org/docs/pyproject/#scripts). Or,
+if you're using hatch, [try this](https://hatch.pypa.io/latest/config/metadata/#cli).
 
 ## Features
 
 `pipx` enables you to
 
 - Expose CLI entrypoints of packages ("apps") installed to isolated environments with the `install` command. This
   guarantees no dependency conflicts and clean uninstalls!
@@ -459,16 +503,18 @@
 [contributors](https://github.com/pypa/pipx/graphs/contributors). The logo was created by
 [@IrishMorales](https://github.com/IrishMorales).
 
 pipx is maintained by a team of volunteers (in alphabetical order)
 
 - [Bernát Gábor](https://github.com/gaborbernat)
 - [Chad Smith](https://github.com/cs01) - co-lead maintainer
+- [Chrysle](https://github.com/chrysle)
 - [Jason Lam](https://github.com/dukecat0)
 - [Matthew Clapp](https://github.com/itsayellow) - co-lead maintainer
+- [Robert Offner](https://github.com/gitznik)
 - [Tzu-ping Chung](https://github.com/uranusjr)
 
 ## Contributing
 
 Issues and Pull Requests are definitely welcome! Check out [Contributing](https://pipx.pypa.io/stable/contributing/) to
 get started. Everyone who interacts with the pipx project via codebase, issue tracker, chat rooms, or otherwise is
 expected to follow the [PSF Code of Conduct](https://github.com/pypa/.github/blob/main/CODE_OF_CONDUCT.md).
```

#### html2text {}

```diff
@@ -1,40 +1,63 @@
+Metadata-Version: 2.3 Name: pipx Version: 1.5.0 Summary: Install and Run Python
+Applications in Isolated Environments Project-URL: Bug Tracker, https://
+github.com/pypa/pipx/issues Project-URL: Documentation, https://pipx.pypa.io
+Project-URL: Homepage, https://pipx.pypa.io Project-URL: Release Notes, https:/
+/pipx.pypa.io/latest/changelog/ Project-URL: Source Code, https://github.com/
+pypa/pipx Author-email: Chad Smith
+gmail.com> License-Expression: MIT License-File: LICENSE Keywords: Virtual
+Environment,cli,install,pip,workflow Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Python: >=3.8 Requires-Dist:
+argcomplete>=1.9.4 Requires-Dist: colorama>=0.4.4; sys_platform == 'win32'
+Requires-Dist: packaging>=20 Requires-Dist: platformdirs>=2.1 Requires-Dist:
+tomli; python_version < '3.11' Requires-Dist: userpath!=1.9.0,>=1.6
+Description-Content-Type: text/markdown
                _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_p_y_p_a_/_p_i_p_x_/_r_a_w_/_m_a_i_n_/_l_o_g_o_._s_v_g_]
 # pipx â Install and Run Python Applications in Isolated Environments
              _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_p_y_p_a_/_p_i_p_x_/_r_a_w_/_m_a_i_n_/_p_i_p_x___d_e_m_o_._g_i_f_]
           _[_i_m_a_g_e_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_p_i_p_x_]
 **Documentation**:
 pipx.pypa.io> **Source Code**:
 github.com/pypa/pipx> _For comparison to other tools including pipsi, see
 [Comparison to Other Tools](https://pipx.pypa.io/stable/comparisons/)._ ##
-Install pipx > [!NOTE] It is not recommended to install `pipx` via `pipx`. If
-you'd like to do this anyway, take a look at the > [`pipx-in-pipx`](https://
-github.com/mattsb42-meta/pipx-in-pipx) project and read about the limitations
-there. ### On macOS ``` brew install pipx pipx ensurepath ``` Upgrade pipx with
-`brew update && brew upgrade pipx`. ### On Linux - Ubuntu 23.04 or above ```
-sudo apt update sudo apt install pipx pipx ensurepath ``` - Ubuntu 22.04 or
-below ``` python3 -m pip install --user pipx python3 -m pipx ensurepath ```
-Upgrade pipx with `python3 -m pip install --user --upgrade pipx`. ### On
-Windows - install via [Scoop](https://scoop.sh/) ``` scoop install pipx pipx
-ensurepath ``` Upgrade pipx with `scoop update pipx`. - install via pip
-(requires pip 19.0 or later) ``` # If you installed python using Microsoft
-Store, replace `py` with `python3` in the next line. py -m pip install --user
-pipx ``` It is possible (even most likely) the above finishes with a WARNING
-looking similar to this: ``` WARNING: The script pipx.exe is installed in
-`\AppData\Roaming\Python\Python3x\Scripts` which is not on PATH ``` If so, go
-to the mentioned folder, allowing you to run the pipx executable directly.
-Enter the following line (even if you did not get the warning): ``` .\pipx.exe
-ensurepath ``` This will add both the above mentioned path and the
-`%USERPROFILE%\.local\bin` folder to your search path. Restart your terminal
-session and verify `pipx` does run. Upgrade pipx with `py -m pip install --user
---upgrade pipx`. ### Using pipx without installing (via zipapp) You can also
-use pipx without installing it. The zipapp can be downloaded from [Github
-releases](https://github.com/pypa/pipx/releases) and you can invoke it with a
-Python 3.7+ interpreter: ``` python pipx.pyz ensurepath ``` ### Use with pre-
-commit pipx [has pre-commit support](installation.md#pre-commit). ### Shell
+Install pipx > [!WARNING] > > It is not recommended to install `pipx` via
+`pipx`. If you'd like to do this anyway, take a look at the > [`pipx-in-pipx`]
+(https://github.com/mattsb42-meta/pipx-in-pipx) project and read about the
+limitations there. ### On macOS ``` brew install pipx pipx ensurepath sudo pipx
+ensurepath --global # optional to allow pipx actions with --global argument ```
+Upgrade pipx with `brew update && brew upgrade pipx`. ### On Linux - Ubuntu
+23.04 or above ``` sudo apt update sudo apt install pipx pipx ensurepath sudo
+pipx ensurepath --global # optional to allow pipx actions with --global
+argument ``` - Fedora: ``` sudo dnf install pipx pipx ensurepath sudo pipx
+ensurepath --global # optional to allow pipx actions with --global argument ```
+- Using `pip` on other distributions: ``` python3 -m pip install --user pipx
+python3 -m pipx ensurepath sudo pipx ensurepath --global # optional to allow
+pipx actions with --global argument ``` Upgrade pipx with `python3 -m pip
+install --user --upgrade pipx`. ### On Windows - install via [Scoop](https://
+scoop.sh/) ``` scoop install pipx pipx ensurepath ``` Upgrade pipx with `scoop
+update pipx`. - install via pip (requires pip 19.0 or later) ``` # If you
+installed python using Microsoft Store, replace `py` with `python3` in the next
+line. py -m pip install --user pipx ``` It is possible (even most likely) the
+above finishes with a WARNING looking similar to this: ``` WARNING: The script
+pipx.exe is installed in `\AppData\Roaming\Python\Python3x\Scripts` which is
+not on PATH ``` If so, go to the mentioned folder, allowing you to run the pipx
+executable directly. Enter the following line (even if you did not get the
+warning): ``` .\pipx.exe ensurepath ``` This will add both the above mentioned
+path and the `%USERPROFILE%\.local\bin` folder to your search path. Restart
+your terminal session and verify `pipx` does run. Upgrade pipx with `py -m pip
+install --user --upgrade pipx`. ### Using pipx without installing (via zipapp)
+You can also use pipx without installing it. The zipapp can be downloaded from
+[Github releases](https://github.com/pypa/pipx/releases) and you can invoke it
+with a Python 3.7+ interpreter: ``` python pipx.pyz ensurepath ``` ### Use with
+pre-commit pipx [has pre-commit support](installation.md#pre-commit). ### Shell
 completions Shell completions are available by following the instructions
 printed with this command: ``` pipx completions ``` For more details, see the
 [installation instructions](https://pipx.pypa.io/stable/installation/). ##
 Overview: What is `pipx`? pipx is a tool to help you install and run end-user
 applications written in Python. It's roughly similar to macOS's `brew`,
 JavaScript's [npx](https://medium.com/@maybekatz/introducing-npx-an-npm-
 package-runner-55f7d4bd282b), and Linux's `apt`. It's closely related to pip.
@@ -55,15 +78,15 @@
 run any of these thousands of application-containing packages in a safe,
 convenient, and reliable way. **In a way, it turns Python Package Index (PyPI)
 into a big app store for Python applications.** Not all Python packages have
 entry points, but many do. If you would like to make your package compatible
 with pipx, all you need to do is add a [console scripts](https://python-
 packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-
 scripts-entry-point) entry point. If you're a poetry user, use [these
-instructions](https://python-poetry.org/docs/pyproject/#scripts). Or you're
+instructions](https://python-poetry.org/docs/pyproject/#scripts). Or, if you're
 using hatch, [try this](https://hatch.pypa.io/latest/config/metadata/#cli). ##
 Features `pipx` enables you to - Expose CLI entrypoints of packages ("apps")
 installed to isolated environments with the `install` command. This guarantees
 no dependency conflicts and clean uninstalls! - Easily list, upgrade, and
 uninstall packages that were installed with pipx - Run the latest version of a
 Python application in a temporary environment with the `run` command Best of
 all, pipx runs with regular user permissions, never calling `sudo pip install`
@@ -185,14 +208,15 @@
 ## Credits pipx was inspired by [pipsi](https://github.com/mitsuhiko/pipsi) and
 [npx](https://github.com/npm/npx). It was created by [Chad Smith](https://
 github.com/cs01/) and has had lots of help from [contributors](https://
 github.com/pypa/pipx/graphs/contributors). The logo was created by
 [@IrishMorales](https://github.com/IrishMorales). pipx is maintained by a team
 of volunteers (in alphabetical order) - [BernÃ¡t GÃ¡bor](https://github.com/
 gaborbernat) - [Chad Smith](https://github.com/cs01) - co-lead maintainer -
-[Jason Lam](https://github.com/dukecat0) - [Matthew Clapp](https://github.com/
-itsayellow) - co-lead maintainer - [Tzu-ping Chung](https://github.com/
-uranusjr) ## Contributing Issues and Pull Requests are definitely welcome!
-Check out [Contributing](https://pipx.pypa.io/stable/contributing/) to get
-started. Everyone who interacts with the pipx project via codebase, issue
+[Chrysle](https://github.com/chrysle) - [Jason Lam](https://github.com/
+dukecat0) - [Matthew Clapp](https://github.com/itsayellow) - co-lead maintainer
+- [Robert Offner](https://github.com/gitznik) - [Tzu-ping Chung](https://
+github.com/uranusjr) ## Contributing Issues and Pull Requests are definitely
+welcome! Check out [Contributing](https://pipx.pypa.io/stable/contributing/) to
+get started. Everyone who interacts with the pipx project via codebase, issue
 tracker, chat rooms, or otherwise is expected to follow the [PSF Code of
 Conduct](https://github.com/pypa/.github/blob/main/CODE_OF_CONDUCT.md).
```

### Comparing `pipx-1.4.3/pyproject.toml` & `pipx-1.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -67,22 +67,29 @@
   "PLW",
   "RSE",
   "W",
 ]
 lint.isort = {known-first-party = ["helpers", "package_info", "pipx"]}
 lint.mccabe.max-complexity = 15
 
+[tool.codespell]
+# Ref: https://github.com/codespell-project/codespell#using-a-config-file
+skip = '.git,*.pdf,*.svg,.nox,testdata,.mypy_cache'
+check-hidden = true
+# case sensitive etc
+ignore-regex = '\b(UE|path/doesnt/exist)\b'
+
 [tool.pytest.ini_options]
 markers = ["all_packages: test install with maximum number of packages"]
 
 [tool.towncrier]
 directory = "changelog.d"
 filename = "CHANGELOG.md"
 start_string = "<!-- towncrier release notes start -->\n"
 underlines = ["", "", ""]
 title_format = "## [{version}](https://github.com/pypa/pipx/tree/{version}) - {project_date}"
 issue_format = "[#{issue}](https://github.com/pypa/pipx/issues/{issue})"
 package = "pipx"
 
 [[tool.mypy.overrides]]
-module = ["pipx.version", "pycowsay.*"]
+module = ["pycowsay.*"]
 ignore_missing_imports = true
```

### Comparing `pipx-1.4.3/PKG-INFO` & `pipx-1.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: pipx
-Version: 1.4.3
-Summary: Install and Run Python Applications in Isolated Environments
-Project-URL: Bug Tracker, https://github.com/pypa/pipx/issues
-Project-URL: Documentation, https://pipx.pypa.io
-Project-URL: Homepage, https://pipx.pypa.io
-Project-URL: Release Notes, https://pipx.pypa.io/latest/changelog/
-Project-URL: Source Code, https://github.com/pypa/pipx
-Author-email: Chad Smith <chadsmith.software@gmail.com>
-License-Expression: MIT
-License-File: LICENSE
-Keywords: Virtual Environment,cli,install,pip,workflow
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Requires-Dist: argcomplete>=1.9.4
-Requires-Dist: colorama>=0.4.4; sys_platform == 'win32'
-Requires-Dist: packaging>=20
-Requires-Dist: platformdirs>=2.1
-Requires-Dist: tomli; python_version < '3.11'
-Requires-Dist: userpath!=1.9.0,>=1.6
-Description-Content-Type: text/markdown
-
 <p align="center">
 <a href="https://pipx.pypa.io">
 <img align="center" src="https://github.com/pypa/pipx/raw/main/logo.svg" width="200"/>
 </a>
 </p>
 
 # pipx — Install and Run Python Applications in Isolated Environments
@@ -54,41 +23,54 @@
 **Source Code**: <https://github.com/pypa/pipx>
 
 _For comparison to other tools including pipsi, see
 [Comparison to Other Tools](https://pipx.pypa.io/stable/comparisons/)._
 
 ## Install pipx
 
-> [!NOTE] It is not recommended to install `pipx` via `pipx`. If you'd like to do this anyway, take a look at the
+> [!WARNING]
+>
+> It is not recommended to install `pipx` via `pipx`. If you'd like to do this anyway, take a look at the
 > [`pipx-in-pipx`](https://github.com/mattsb42-meta/pipx-in-pipx) project and read about the limitations there.
 
 ### On macOS
 
 ```
 brew install pipx
 pipx ensurepath
+sudo pipx ensurepath --global # optional to allow pipx actions with --global argument
 ```
 
 Upgrade pipx with `brew update && brew upgrade pipx`.
 
 ### On Linux
 
 - Ubuntu 23.04 or above
 
 ```
 sudo apt update
 sudo apt install pipx
 pipx ensurepath
+sudo pipx ensurepath --global # optional to allow pipx actions with --global argument
+```
+
+- Fedora:
+
+```
+sudo dnf install pipx
+pipx ensurepath
+sudo pipx ensurepath --global # optional to allow pipx actions with --global argument
 ```
 
-- Ubuntu 22.04 or below
+- Using `pip` on other distributions:
 
 ```
 python3 -m pip install --user pipx
 python3 -m pipx ensurepath
+sudo pipx ensurepath --global # optional to allow pipx actions with --global argument
 ```
 
 Upgrade pipx with `python3 -m pip install --user --upgrade pipx`.
 
 ### On Windows
 
 - install via [Scoop](https://scoop.sh/)
@@ -175,16 +157,16 @@
 
 pipx is a tool to install and run any of these thousands of application-containing packages in a safe, convenient, and
 reliable way. **In a way, it turns Python Package Index (PyPI) into a big app store for Python applications.** Not all
 Python packages have entry points, but many do.
 
 If you would like to make your package compatible with pipx, all you need to do is add a
 [console scripts](https://python-packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-scripts-entry-point)
-entry point. If you're a poetry user, use [these instructions](https://python-poetry.org/docs/pyproject/#scripts). Or
-you're using hatch, [try this](https://hatch.pypa.io/latest/config/metadata/#cli).
+entry point. If you're a poetry user, use [these instructions](https://python-poetry.org/docs/pyproject/#scripts). Or,
+if you're using hatch, [try this](https://hatch.pypa.io/latest/config/metadata/#cli).
 
 ## Features
 
 `pipx` enables you to
 
 - Expose CLI entrypoints of packages ("apps") installed to isolated environments with the `install` command. This
   guarantees no dependency conflicts and clean uninstalls!
@@ -490,16 +472,18 @@
 [contributors](https://github.com/pypa/pipx/graphs/contributors). The logo was created by
 [@IrishMorales](https://github.com/IrishMorales).
 
 pipx is maintained by a team of volunteers (in alphabetical order)
 
 - [Bernát Gábor](https://github.com/gaborbernat)
 - [Chad Smith](https://github.com/cs01) - co-lead maintainer
+- [Chrysle](https://github.com/chrysle)
 - [Jason Lam](https://github.com/dukecat0)
 - [Matthew Clapp](https://github.com/itsayellow) - co-lead maintainer
+- [Robert Offner](https://github.com/gitznik)
 - [Tzu-ping Chung](https://github.com/uranusjr)
 
 ## Contributing
 
 Issues and Pull Requests are definitely welcome! Check out [Contributing](https://pipx.pypa.io/stable/contributing/) to
 get started. Everyone who interacts with the pipx project via codebase, issue tracker, chat rooms, or otherwise is
 expected to follow the [PSF Code of Conduct](https://github.com/pypa/.github/blob/main/CODE_OF_CONDUCT.md).
```

#### html2text {}

```diff
@@ -1,58 +1,45 @@
-Metadata-Version: 2.1 Name: pipx Version: 1.4.3 Summary: Install and Run Python
-Applications in Isolated Environments Project-URL: Bug Tracker, https://
-github.com/pypa/pipx/issues Project-URL: Documentation, https://pipx.pypa.io
-Project-URL: Homepage, https://pipx.pypa.io Project-URL: Release Notes, https:/
-/pipx.pypa.io/latest/changelog/ Project-URL: Source Code, https://github.com/
-pypa/pipx Author-email: Chad Smith
-gmail.com> License-Expression: MIT License-File: LICENSE Keywords: Virtual
-Environment,cli,install,pip,workflow Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Python: >=3.8 Requires-Dist:
-argcomplete>=1.9.4 Requires-Dist: colorama>=0.4.4; sys_platform == 'win32'
-Requires-Dist: packaging>=20 Requires-Dist: platformdirs>=2.1 Requires-Dist:
-tomli; python_version < '3.11' Requires-Dist: userpath!=1.9.0,>=1.6
-Description-Content-Type: text/markdown
                _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_p_y_p_a_/_p_i_p_x_/_r_a_w_/_m_a_i_n_/_l_o_g_o_._s_v_g_]
 # pipx â Install and Run Python Applications in Isolated Environments
              _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_p_y_p_a_/_p_i_p_x_/_r_a_w_/_m_a_i_n_/_p_i_p_x___d_e_m_o_._g_i_f_]
           _[_i_m_a_g_e_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_p_i_p_x_]
 **Documentation**:
 pipx.pypa.io> **Source Code**:
 github.com/pypa/pipx> _For comparison to other tools including pipsi, see
 [Comparison to Other Tools](https://pipx.pypa.io/stable/comparisons/)._ ##
-Install pipx > [!NOTE] It is not recommended to install `pipx` via `pipx`. If
-you'd like to do this anyway, take a look at the > [`pipx-in-pipx`](https://
-github.com/mattsb42-meta/pipx-in-pipx) project and read about the limitations
-there. ### On macOS ``` brew install pipx pipx ensurepath ``` Upgrade pipx with
-`brew update && brew upgrade pipx`. ### On Linux - Ubuntu 23.04 or above ```
-sudo apt update sudo apt install pipx pipx ensurepath ``` - Ubuntu 22.04 or
-below ``` python3 -m pip install --user pipx python3 -m pipx ensurepath ```
-Upgrade pipx with `python3 -m pip install --user --upgrade pipx`. ### On
-Windows - install via [Scoop](https://scoop.sh/) ``` scoop install pipx pipx
-ensurepath ``` Upgrade pipx with `scoop update pipx`. - install via pip
-(requires pip 19.0 or later) ``` # If you installed python using Microsoft
-Store, replace `py` with `python3` in the next line. py -m pip install --user
-pipx ``` It is possible (even most likely) the above finishes with a WARNING
-looking similar to this: ``` WARNING: The script pipx.exe is installed in
-`\AppData\Roaming\Python\Python3x\Scripts` which is not on PATH ``` If so, go
-to the mentioned folder, allowing you to run the pipx executable directly.
-Enter the following line (even if you did not get the warning): ``` .\pipx.exe
-ensurepath ``` This will add both the above mentioned path and the
-`%USERPROFILE%\.local\bin` folder to your search path. Restart your terminal
-session and verify `pipx` does run. Upgrade pipx with `py -m pip install --user
---upgrade pipx`. ### Using pipx without installing (via zipapp) You can also
-use pipx without installing it. The zipapp can be downloaded from [Github
-releases](https://github.com/pypa/pipx/releases) and you can invoke it with a
-Python 3.7+ interpreter: ``` python pipx.pyz ensurepath ``` ### Use with pre-
-commit pipx [has pre-commit support](installation.md#pre-commit). ### Shell
+Install pipx > [!WARNING] > > It is not recommended to install `pipx` via
+`pipx`. If you'd like to do this anyway, take a look at the > [`pipx-in-pipx`]
+(https://github.com/mattsb42-meta/pipx-in-pipx) project and read about the
+limitations there. ### On macOS ``` brew install pipx pipx ensurepath sudo pipx
+ensurepath --global # optional to allow pipx actions with --global argument ```
+Upgrade pipx with `brew update && brew upgrade pipx`. ### On Linux - Ubuntu
+23.04 or above ``` sudo apt update sudo apt install pipx pipx ensurepath sudo
+pipx ensurepath --global # optional to allow pipx actions with --global
+argument ``` - Fedora: ``` sudo dnf install pipx pipx ensurepath sudo pipx
+ensurepath --global # optional to allow pipx actions with --global argument ```
+- Using `pip` on other distributions: ``` python3 -m pip install --user pipx
+python3 -m pipx ensurepath sudo pipx ensurepath --global # optional to allow
+pipx actions with --global argument ``` Upgrade pipx with `python3 -m pip
+install --user --upgrade pipx`. ### On Windows - install via [Scoop](https://
+scoop.sh/) ``` scoop install pipx pipx ensurepath ``` Upgrade pipx with `scoop
+update pipx`. - install via pip (requires pip 19.0 or later) ``` # If you
+installed python using Microsoft Store, replace `py` with `python3` in the next
+line. py -m pip install --user pipx ``` It is possible (even most likely) the
+above finishes with a WARNING looking similar to this: ``` WARNING: The script
+pipx.exe is installed in `\AppData\Roaming\Python\Python3x\Scripts` which is
+not on PATH ``` If so, go to the mentioned folder, allowing you to run the pipx
+executable directly. Enter the following line (even if you did not get the
+warning): ``` .\pipx.exe ensurepath ``` This will add both the above mentioned
+path and the `%USERPROFILE%\.local\bin` folder to your search path. Restart
+your terminal session and verify `pipx` does run. Upgrade pipx with `py -m pip
+install --user --upgrade pipx`. ### Using pipx without installing (via zipapp)
+You can also use pipx without installing it. The zipapp can be downloaded from
+[Github releases](https://github.com/pypa/pipx/releases) and you can invoke it
+with a Python 3.7+ interpreter: ``` python pipx.pyz ensurepath ``` ### Use with
+pre-commit pipx [has pre-commit support](installation.md#pre-commit). ### Shell
 completions Shell completions are available by following the instructions
 printed with this command: ``` pipx completions ``` For more details, see the
 [installation instructions](https://pipx.pypa.io/stable/installation/). ##
 Overview: What is `pipx`? pipx is a tool to help you install and run end-user
 applications written in Python. It's roughly similar to macOS's `brew`,
 JavaScript's [npx](https://medium.com/@maybekatz/introducing-npx-an-npm-
 package-runner-55f7d4bd282b), and Linux's `apt`. It's closely related to pip.
@@ -73,15 +60,15 @@
 run any of these thousands of application-containing packages in a safe,
 convenient, and reliable way. **In a way, it turns Python Package Index (PyPI)
 into a big app store for Python applications.** Not all Python packages have
 entry points, but many do. If you would like to make your package compatible
 with pipx, all you need to do is add a [console scripts](https://python-
 packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-
 scripts-entry-point) entry point. If you're a poetry user, use [these
-instructions](https://python-poetry.org/docs/pyproject/#scripts). Or you're
+instructions](https://python-poetry.org/docs/pyproject/#scripts). Or, if you're
 using hatch, [try this](https://hatch.pypa.io/latest/config/metadata/#cli). ##
 Features `pipx` enables you to - Expose CLI entrypoints of packages ("apps")
 installed to isolated environments with the `install` command. This guarantees
 no dependency conflicts and clean uninstalls! - Easily list, upgrade, and
 uninstall packages that were installed with pipx - Run the latest version of a
 Python application in a temporary environment with the `run` command Best of
 all, pipx runs with regular user permissions, never calling `sudo pip install`
@@ -203,14 +190,15 @@
 ## Credits pipx was inspired by [pipsi](https://github.com/mitsuhiko/pipsi) and
 [npx](https://github.com/npm/npx). It was created by [Chad Smith](https://
 github.com/cs01/) and has had lots of help from [contributors](https://
 github.com/pypa/pipx/graphs/contributors). The logo was created by
 [@IrishMorales](https://github.com/IrishMorales). pipx is maintained by a team
 of volunteers (in alphabetical order) - [BernÃ¡t GÃ¡bor](https://github.com/
 gaborbernat) - [Chad Smith](https://github.com/cs01) - co-lead maintainer -
-[Jason Lam](https://github.com/dukecat0) - [Matthew Clapp](https://github.com/
-itsayellow) - co-lead maintainer - [Tzu-ping Chung](https://github.com/
-uranusjr) ## Contributing Issues and Pull Requests are definitely welcome!
-Check out [Contributing](https://pipx.pypa.io/stable/contributing/) to get
-started. Everyone who interacts with the pipx project via codebase, issue
+[Chrysle](https://github.com/chrysle) - [Jason Lam](https://github.com/
+dukecat0) - [Matthew Clapp](https://github.com/itsayellow) - co-lead maintainer
+- [Robert Offner](https://github.com/gitznik) - [Tzu-ping Chung](https://
+github.com/uranusjr) ## Contributing Issues and Pull Requests are definitely
+welcome! Check out [Contributing](https://pipx.pypa.io/stable/contributing/) to
+get started. Everyone who interacts with the pipx project via codebase, issue
 tracker, chat rooms, or otherwise is expected to follow the [PSF Code of
 Conduct](https://github.com/pypa/.github/blob/main/CODE_OF_CONDUCT.md).
```

