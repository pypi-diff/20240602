# Comparing `tmp/pytest-fail-slow-0.4.0.tar.gz` & `tmp/pytest_fail_slow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-fail-slow-0.4.0.tar", last modified: Sat Oct 21 16:50:37 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pytest-fail-slow-0.4.0.tar` & `pytest_fail_slow-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,13 @@
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-21 16:50:37.457178 pytest-fail-slow-0.4.0/
--rw-r--r--   0 jwodder    (501) staff       (20)      719 2023-10-21 16:50:31.000000 pytest-fail-slow-0.4.0/CHANGELOG.md
--rw-r--r--   0 jwodder    (501) staff       (20)     1095 2023-10-21 16:50:31.000000 pytest-fail-slow-0.4.0/LICENSE
--rw-r--r--   0 jwodder    (501) staff       (20)      126 2021-12-10 14:33:32.000000 pytest-fail-slow-0.4.0/MANIFEST.in
--rw-r--r--   0 jwodder    (501) staff       (20)     6348 2023-10-21 16:50:37.456983 pytest-fail-slow-0.4.0/PKG-INFO
--rw-r--r--   0 jwodder    (501) staff       (20)     5041 2023-10-21 16:43:17.000000 pytest-fail-slow-0.4.0/README.rst
--rw-r--r--   0 jwodder    (501) staff       (20)       91 2022-07-07 12:48:58.000000 pytest-fail-slow-0.4.0/pyproject.toml
--rw-r--r--   0 jwodder    (501) staff       (20)     1424 2023-10-21 16:50:37.458122 pytest-fail-slow-0.4.0/setup.cfg
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-21 16:50:37.450046 pytest-fail-slow-0.4.0/src/
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-21 16:50:37.452423 pytest-fail-slow-0.4.0/src/pytest_fail_slow.egg-info/
--rw-r--r--   0 jwodder    (501) staff       (20)     6348 2023-10-21 16:50:37.000000 pytest-fail-slow-0.4.0/src/pytest_fail_slow.egg-info/PKG-INFO
--rw-r--r--   0 jwodder    (501) staff       (20)      463 2023-10-21 16:50:37.000000 pytest-fail-slow-0.4.0/src/pytest_fail_slow.egg-info/SOURCES.txt
--rw-r--r--   0 jwodder    (501) staff       (20)        1 2023-10-21 16:50:37.000000 pytest-fail-slow-0.4.0/src/pytest_fail_slow.egg-info/dependency_links.txt
--rw-r--r--   0 jwodder    (501) staff       (20)       40 2023-10-21 16:50:37.000000 pytest-fail-slow-0.4.0/src/pytest_fail_slow.egg-info/entry_points.txt
--rw-r--r--   0 jwodder    (501) staff       (20)       12 2023-10-21 16:50:37.000000 pytest-fail-slow-0.4.0/src/pytest_fail_slow.egg-info/requires.txt
--rw-r--r--   0 jwodder    (501) staff       (20)       17 2023-10-21 16:50:37.000000 pytest-fail-slow-0.4.0/src/pytest_fail_slow.egg-info/top_level.txt
--rw-r--r--   0 jwodder    (501) staff       (20)     3880 2023-10-21 16:50:31.000000 pytest-fail-slow-0.4.0/src/pytest_fail_slow.py
-drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-10-21 16:50:37.455272 pytest-fail-slow-0.4.0/test/
--rw-r--r--   0 jwodder    (501) staff       (20)       30 2021-12-10 16:16:56.000000 pytest-fail-slow-0.4.0/test/conftest.py
--rw-r--r--   0 jwodder    (501) staff       (20)     3340 2023-10-21 16:43:17.000000 pytest-fail-slow-0.4.0/test/test_fail_slow.py
--rw-r--r--   0 jwodder    (501) staff       (20)     6023 2023-10-21 16:43:17.000000 pytest-fail-slow-0.4.0/test/test_fail_slow_setup.py
--rw-r--r--   0 jwodder    (501) staff       (20)     1952 2022-02-04 16:39:53.000000 pytest-fail-slow-0.4.0/test/test_parse_duration.py
--rw-r--r--   0 jwodder    (501) staff       (20)     1553 2023-10-03 14:53:26.000000 pytest-fail-slow-0.4.0/tox.ini
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/tox.ini
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/src/pytest_fail_slow/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/src/pytest_fail_slow/py.typed
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/test/conftest.py
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/test/test_fail_slow.py
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/test/test_fail_slow_setup.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/test/test_parse_duration.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/README.rst
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 pytest_fail_slow-0.5.0/PKG-INFO
```

### Comparing `pytest-fail-slow-0.4.0/LICENSE` & `pytest_fail_slow-0.5.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021-2023 John Thorvald Wodder II
+Copyright (c) 2021-2024 John Thorvald Wodder II
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pytest-fail-slow-0.4.0/PKG-INFO` & `pytest_fail_slow-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: pytest-fail-slow
-Version: 0.4.0
+Version: 0.5.0
 Summary: Fail tests that take too long to run
-Home-page: https://github.com/jwodder/pytest-fail-slow
-Author: John Thorvald Wodder II
-Author-email: pytest-fail-slow@varonathe.org
-License: MIT
 Project-URL: Source Code, https://github.com/jwodder/pytest-fail-slow
 Project-URL: Bug Tracker, https://github.com/jwodder/pytest-fail-slow/issues
+Author-email: John Thorvald Wodder II <pytest-fail-slow@varonathe.org>
+License-Expression: MIT
+License-File: LICENSE
 Keywords: pytest,slow tests,timeout
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Environment :: Plugins
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Plugins
-Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Requires-Dist: pluggy>=1.1
+Requires-Dist: pytest>=7.0
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: pytest>=6.0
 
-.. image:: http://www.repostatus.org/badges/latest/active.svg
-    :target: http://www.repostatus.org/#active
+.. image:: https://www.repostatus.org/badges/latest/active.svg
+    :target: https://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
 
-.. image:: https://github.com/jwodder/pytest-fail-slow/workflows/Test/badge.svg?branch=master
-    :target: https://github.com/jwodder/pytest-fail-slow/actions?workflow=Test
+.. image:: https://github.com/jwodder/pytest-fail-slow/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/jwodder/pytest-fail-slow/actions/workflows/test.yml
     :alt: CI Status
 
 .. image:: https://codecov.io/gh/jwodder/pytest-fail-slow/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/jwodder/pytest-fail-slow
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-fail-slow.svg
     :target: https://pypi.org/project/pytest-fail-slow/
@@ -67,15 +66,15 @@
 
 .. _pytest: https://docs.pytest.org
 .. _pytest-timeout: https://github.com/pytest-dev/pytest-timeout
 
 
 Installation
 ============
-``pytest-fail-slow`` requires Python 3.7 or higher and pytest 6.0 or higher.
+``pytest-fail-slow`` requires Python 3.8 or higher and pytest 7.0 or higher.
 Just use `pip <https://pip.pypa.io>`_ for Python 3 (You have pip, right?) to
 install it::
 
     python3 -m pip install pytest-fail-slow
 
 
 Usage
@@ -131,16 +130,16 @@
         ...
 
 Do not apply the marker to the test's fixtures; markers have no effect on
 fixtures.
 
 In addition, the ``--fail-slow-setup DURATION`` option can be passed to the
 ``pytest`` command to affect all tests in that run.  If ``--fail-slow-setup``
-is given and a test has the ``fail_slow_setupresou`` marker, the duration given
-by the marker takes precedence for that test.
+is given and a test has the ``fail_slow_setup`` marker, the duration given by
+the marker takes precedence for that test.
 
 If the setup for a test takes too long to run, the test will be marked as
 "errored," the test itself will not be run, and pytest's output will include
 the setup stage's duration and the duration threshold, like so::
 
     _______________________ ERROR at setup of test_func _______________________
     Setup passed but took too long to run: Duration 123.0s > 5.0s
```

### Comparing `pytest-fail-slow-0.4.0/README.rst` & `pytest_fail_slow-0.5.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-.. image:: http://www.repostatus.org/badges/latest/active.svg
-    :target: http://www.repostatus.org/#active
+.. image:: https://www.repostatus.org/badges/latest/active.svg
+    :target: https://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
 
-.. image:: https://github.com/jwodder/pytest-fail-slow/workflows/Test/badge.svg?branch=master
-    :target: https://github.com/jwodder/pytest-fail-slow/actions?workflow=Test
+.. image:: https://github.com/jwodder/pytest-fail-slow/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/jwodder/pytest-fail-slow/actions/workflows/test.yml
     :alt: CI Status
 
 .. image:: https://codecov.io/gh/jwodder/pytest-fail-slow/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/jwodder/pytest-fail-slow
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-fail-slow.svg
     :target: https://pypi.org/project/pytest-fail-slow/
@@ -36,15 +36,15 @@
 
 .. _pytest: https://docs.pytest.org
 .. _pytest-timeout: https://github.com/pytest-dev/pytest-timeout
 
 
 Installation
 ============
-``pytest-fail-slow`` requires Python 3.7 or higher and pytest 6.0 or higher.
+``pytest-fail-slow`` requires Python 3.8 or higher and pytest 7.0 or higher.
 Just use `pip <https://pip.pypa.io>`_ for Python 3 (You have pip, right?) to
 install it::
 
     python3 -m pip install pytest-fail-slow
 
 
 Usage
@@ -100,16 +100,16 @@
         ...
 
 Do not apply the marker to the test's fixtures; markers have no effect on
 fixtures.
 
 In addition, the ``--fail-slow-setup DURATION`` option can be passed to the
 ``pytest`` command to affect all tests in that run.  If ``--fail-slow-setup``
-is given and a test has the ``fail_slow_setupresou`` marker, the duration given
-by the marker takes precedence for that test.
+is given and a test has the ``fail_slow_setup`` marker, the duration given by
+the marker takes precedence for that test.
 
 If the setup for a test takes too long to run, the test will be marked as
 "errored," the test itself will not be run, and pytest's output will include
 the setup stage's duration and the duration threshold, like so::
 
     _______________________ ERROR at setup of test_func _______________________
     Setup passed but took too long to run: Duration 123.0s > 5.0s
```

### Comparing `pytest-fail-slow-0.4.0/src/pytest_fail_slow.py` & `pytest_fail_slow-0.5.0/src/pytest_fail_slow/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,35 +11,39 @@
 
 .. _pytest: https://docs.pytest.org
 .. _pytest-timeout: https://github.com/pytest-dev/pytest-timeout
 
 Visit <https://github.com/jwodder/pytest-fail-slow> for more information.
 """
 
-__version__ = "0.4.0"
+from __future__ import annotations
+import re
+from typing import Generator, Union
+import pytest
+
+__version__ = "0.5.0"
 __author__ = "John Thorvald Wodder II"
 __author_email__ = "pytest-fail-slow@varonathe.org"
 __license__ = "MIT"
 __url__ = "https://github.com/jwodder/pytest-fail-slow"
 
-from numbers import Number
-import re
-import pytest
-
 TIME_UNITS = {
     "hour": 3600.0,
     "min": 60.0,
     "sec": 1.0,
     "ms": 0.001,
     "us": 0.000001,
 }
 
+setup_timeout_key = pytest.StashKey[Union[int, float, None]]()
+call_timeout_key = pytest.StashKey[Union[int, float, None]]()
+
 
-def parse_duration(s) -> float:
-    if isinstance(s, Number):
+def parse_duration(s: str | int | float) -> int | float:
+    if isinstance(s, (int, float)):
         return s
     m = re.search(
         r"""
         (?<=[\d\s.])
         (?:
             (?P<hour>h(ours?)?)
             |(?P<min>m(in(ute)?s?)?)
@@ -56,73 +60,84 @@
         mul = TIME_UNITS[unit.lower()]
         s = s[: m.start()]
     else:
         mul = 1.0
     return float(s) * mul
 
 
-def pytest_configure(config) -> None:
+def pytest_configure(config: pytest.Config) -> None:
     config.addinivalue_line(
         "markers",
         "fail_slow(duration): Fail test if it takes more than this long to run",
     )
     config.addinivalue_line(
         "markers",
         (
             "fail_slow_setup(duration):"
             " Fail test if it takes more than this long to set up"
         ),
     )
 
 
-def pytest_addoption(parser) -> None:
+def pytest_addoption(parser: pytest.Parser) -> None:
     parser.addoption(
         "--fail-slow",
         type=parse_duration,
         metavar="DURATION",
         help="Fail tests that take more than this long to run",
     )
     parser.addoption(
         "--fail-slow-setup",
         type=parse_duration,
         metavar="DURATION",
         help="Fail tests that take more than this long to set up",
     )
 
 
-@pytest.hookimpl(hookwrapper=True)
-def pytest_runtest_makereport(item, call):
-    report = (yield).get_result()
-    if report is None or report.outcome != "passed":
-        return
+def pytest_runtest_setup(item: pytest.Item) -> None:
+    setup_mark = item.get_closest_marker("fail_slow_setup")
+    if setup_mark is not None:
+        if len(setup_mark.args) != 1:
+            raise pytest.UsageError(
+                "@pytest.mark.fail_slow_setup() takes exactly one argument"
+            )
+        setup_timeout = parse_duration(setup_mark.args[0])
+    else:
+        setup_timeout = item.config.getoption("--fail-slow-setup")
+    item.stash[setup_timeout_key] = setup_timeout
+
+    call_mark = item.get_closest_marker("fail_slow")
+    if call_mark is not None:
+        if len(call_mark.args) != 1:
+            raise pytest.UsageError(
+                "@pytest.mark.fail_slow() takes exactly one argument"
+            )
+        call_timeout = parse_duration(call_mark.args[0])
+    else:
+        call_timeout = item.config.getoption("--fail-slow")
+    item.stash[call_timeout_key] = call_timeout
+
+
+@pytest.hookimpl(wrapper=True)
+def pytest_runtest_makereport(
+    item: pytest.Item, call: pytest.CallInfo
+) -> Generator[None, pytest.TestReport, pytest.TestReport]:
+    report = yield
+    if report.outcome != "passed":
+        return report
     if report.when == "setup":
-        mark = item.get_closest_marker("fail_slow_setup")
-        if mark is not None:
-            if len(mark.args) != 1:
-                raise pytest.UsageError(
-                    "@pytest.mark.fail_slow_setup() takes exactly one argument"
-                )
-            timeout = parse_duration(mark.args[0])
-        else:
-            timeout = item.config.getoption("--fail-slow-setup")
+        timeout = item.stash[setup_timeout_key]
         if timeout is not None and call.duration > timeout:
             report.outcome = "failed"
             report.longrepr = (
                 "Setup passed but took too long to run:"
                 f" Duration {call.duration}s > {timeout}s"
             )
     elif report.when == "call":
-        mark = item.get_closest_marker("fail_slow")
-        if mark is not None:
-            if len(mark.args) != 1:
-                raise pytest.UsageError(
-                    "@pytest.mark.fail_slow() takes exactly one argument"
-                )
-            timeout = parse_duration(mark.args[0])
-        else:
-            timeout = item.config.getoption("--fail-slow")
+        timeout = item.stash[call_timeout_key]
         if timeout is not None and call.duration > timeout:
             report.outcome = "failed"
             report.longrepr = (
                 "Test passed but took too long to run:"
                 f" Duration {call.duration}s > {timeout}s"
             )
+    return report
```

### Comparing `pytest-fail-slow-0.4.0/test/test_fail_slow.py` & `pytest_fail_slow-0.5.0/test/test_fail_slow.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         False,
     ),
 ]
 
 
 @pytest.mark.parametrize("src,success,slow", CASES)
 def test_fail_slow_no_threshold(
-    pytester, src: str, success: bool, slow: bool  # noqa: U100
+    pytester: pytest.Pytester, src: str, success: bool, slow: bool  # noqa: U100
 ) -> None:
     pytester.makepyfile(test_func=src.format(decor=""))
     result = pytester.runpytest()
     if success:
         result.assert_outcomes(passed=1)
     else:
         result.assert_outcomes(failed=1)
@@ -70,15 +70,15 @@
         ([], "import pytest\n@pytest.mark.fail_slow(2.0)\n", r"2\.\d+s"),
         ([], "import pytest\n@pytest.mark.fail_slow('0.0333m')\n", r"1\.9\d+s"),
         (["--fail-slow=30"], "import pytest\n@pytest.mark.fail_slow(2)\n", r"2s"),
         (["--fail-slow=0.01"], "import pytest\n@pytest.mark.fail_slow(2)\n", r"2s"),
     ],
 )
 def test_fail_slow_threshold(
-    pytester,
+    pytester: pytest.Pytester,
     src: str,
     success: bool,
     slow: bool,
     args: list[str],
     decor: str,
     limitrgx: str,
 ) -> None:
@@ -98,23 +98,22 @@
             consecutive=True,
         )
     else:
         result.stdout.no_fnmatch_line("*Test passed but took too long to run*")
 
 
 @pytest.mark.parametrize("args", ["", "42, 'foo'"])
-def test_fail_slow_marker_bad_args(pytester, args: str) -> None:
+def test_fail_slow_marker_bad_args(pytester: pytest.Pytester, args: str) -> None:
     pytester.makepyfile(
         test_func=(
             "import pytest\n"
             "\n"
             f"@pytest.mark.fail_slow({args})\n"
             "def test_func():\n"
             "    assert 2 + 2 == 4\n"
         )
     )
     result = pytester.runpytest()
-    result.assert_outcomes()
-    result.stdout.no_fnmatch_line("?")
-    result.stderr.fnmatch_lines(
-        ["ERROR: @pytest.mark.fail_slow() takes exactly one argument"]
+    result.assert_outcomes(errors=1)
+    result.stdout.fnmatch_lines(
+        ["*UsageError: @pytest.mark.fail_slow() takes exactly one argument"]
     )
```

### Comparing `pytest-fail-slow-0.4.0/test/test_fail_slow_setup.py` & `pytest_fail_slow-0.5.0/test/test_fail_slow_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         ([], "@pytest.mark.fail_slow_setup(10)\n", None),
         (["--fail-slow-setup=30"], "@pytest.mark.fail_slow_setup(2)\n", r"2s"),
         (["--fail-slow-setup=0.01"], "@pytest.mark.fail_slow_setup(2)\n", r"2s"),
         (["--fail-slow-setup=0.01"], "@pytest.mark.fail_slow_setup(10)\n", None),
     ],
 )
 def test_fail_slow_setup_threshold(
-    pytester, args: list[str], decor: str, limitrgx: str | None
+    pytester: pytest.Pytester, args: list[str], decor: str, limitrgx: str | None
 ) -> None:
     pytester.makepyfile(
         test_func=(
             "from time import sleep\n"
             "import pytest\n"
             "\n"
             "@pytest.fixture\n"
@@ -49,15 +49,17 @@
                 rf" Duration \d+\.\d+s > {limitrgx}$",
             ],
             consecutive=True,
         )
 
 
 @pytest.mark.parametrize("threshold,limitrgx", [(4, "4s"), (10, None)])
-def test_fail_slow_multi_setup(pytester, threshold: str, limitrgx: str | None) -> None:
+def test_fail_slow_multi_setup(
+    pytester: pytest.Pytester, threshold: str, limitrgx: str | None
+) -> None:
     pytester.makepyfile(
         test_func=(
             "from time import sleep\n"
             "import pytest\n"
             "\n"
             "@pytest.fixture\n"
             "def slow_setup():\n"
@@ -85,15 +87,17 @@
                 rf" Duration \d+\.\d+s > {limitrgx}$",
             ],
             consecutive=True,
         )
 
 
 @pytest.mark.parametrize("threshold,success", [(2, False), (5, True)])
-def test_fail_slow_setup_skips_test(pytester, threshold: str, success: bool) -> None:
+def test_fail_slow_setup_skips_test(
+    pytester: pytest.Pytester, threshold: str, success: bool
+) -> None:
     pytester.makepyfile(
         test_func=(
             "from pathlib import Path\n"
             "from time import sleep\n"
             "import pytest\n"
             "\n"
             "@pytest.fixture\n"
@@ -110,15 +114,15 @@
         result.assert_outcomes(passed=1)
         assert (pytester.path / "test.txt").read_text() == "Tested\n"
     else:
         result.assert_outcomes(errors=1)
         assert not (pytester.path / "test.txt").exists()
 
 
-def test_fail_slow_setup_teardown_still_run(pytester) -> None:
+def test_fail_slow_setup_teardown_still_run(pytester: pytest.Pytester) -> None:
     pytester.makepyfile(
         test_func=(
             "from pathlib import Path\n"
             "from time import sleep\n"
             "import pytest\n"
             "\n"
             "@pytest.fixture\n"
@@ -133,15 +137,15 @@
         )
     )
     result = pytester.runpytest()
     result.assert_outcomes(errors=1)
     assert (pytester.path / "teardown.txt").read_text() == "Torn down\n"
 
 
-def test_fail_slow_setup_all_run(pytester) -> None:
+def test_fail_slow_setup_all_run(pytester: pytest.Pytester) -> None:
     pytester.makepyfile(
         test_func=(
             "from pathlib import Path\n"
             "from time import sleep\n"
             "import pytest\n"
             "\n"
             "@pytest.fixture\n"
@@ -159,23 +163,22 @@
     )
     result = pytester.runpytest()
     result.assert_outcomes(errors=1)
     assert (pytester.path / "quick.txt").read_text() == "Set up\n"
 
 
 @pytest.mark.parametrize("args", ["", "42, 'foo'"])
-def test_fail_slow_setup_marker_bad_args(pytester, args: str) -> None:
+def test_fail_slow_setup_marker_bad_args(pytester: pytest.Pytester, args: str) -> None:
     pytester.makepyfile(
         test_func=(
             "import pytest\n"
             "\n"
             f"@pytest.mark.fail_slow_setup({args})\n"
             "def test_func():\n"
             "    assert 2 + 2 == 4\n"
         )
     )
     result = pytester.runpytest()
-    result.assert_outcomes()
-    result.stdout.no_fnmatch_line("?")
-    result.stderr.fnmatch_lines(
-        ["ERROR: @pytest.mark.fail_slow_setup() takes exactly one argument"]
+    result.assert_outcomes(errors=1)
+    result.stdout.fnmatch_lines(
+        ["*UsageError: @pytest.mark.fail_slow_setup() takes exactly one argument"]
     )
```

### Comparing `pytest-fail-slow-0.4.0/test/test_parse_duration.py` & `pytest_fail_slow-0.5.0/test/test_parse_duration.py`

 * *Files identical despite different names*

