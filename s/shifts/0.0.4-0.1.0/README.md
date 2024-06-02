# Comparing `tmp/shifts-0.0.4.tar.gz` & `tmp/shifts-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shifts-0.0.4.tar", max compression
+gzip compressed data, was "shifts-0.1.0.tar", max compression
```

## Comparing `shifts-0.0.4.tar` & `shifts-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-05-31 14:51:23.577219 shifts-0.0.4/LICENSE
--rw-r--r--   0        0        0       42 2024-05-31 21:57:43.156003 shifts-0.0.4/README.md
--rw-r--r--   0        0        0     1245 2024-06-01 06:57:28.991195 shifts-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       42 2024-05-31 19:51:41.125669 shifts-0.0.4/src/shifts/__init__.py
--rw-r--r--   0        0        0     3881 2024-06-01 06:50:43.702912 shifts-0.0.4/src/shifts/shifts.py
--rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 shifts-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-31 14:51:23.577219 shifts-0.1.0/LICENSE
+-rw-r--r--   0        0        0       42 2024-05-31 21:57:43.156003 shifts-0.1.0/README.md
+-rw-r--r--   0        0        0     1245 2024-06-02 10:55:10.787513 shifts-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-05-31 19:51:41.125669 shifts-0.1.0/src/shifts/__init__.py
+-rw-r--r--   0        0        0     4126 2024-06-02 10:52:57.559250 shifts-0.1.0/src/shifts/shifts.py
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 shifts-0.1.0/PKG-INFO
```

### Comparing `shifts-0.0.4/LICENSE` & `shifts-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shifts-0.0.4/pyproject.toml` & `shifts-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.mypy]
 ignore_missing_imports = true
 # https://stackoverflow.com/questions/62265366/does-mypy-only-type-check-a-function-if-it-declares-a-return-type
 check_untyped_defs = true
 
 [tool.poetry]
 name = "shifts"
-version = "0.0.4"
+version = "0.1.0"
 description = "Converts shifts to a ical file"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicense"
 readme = "README.md"
 packages = [{ include = "shifts", from = "src" }]
 exclude = ["**/*_test.py"]
```

### Comparing `shifts-0.0.4/src/shifts/shifts.py` & `shifts-0.1.0/src/shifts/shifts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 import calendar
 import os
-import sys
 from datetime import datetime, timedelta
-from importlib.metadata import version as get_version
 from typing import List, Tuple
 
 import typer
 from dateutil.relativedelta import relativedelta
 from ics import Calendar, Event
+from typing_extensions import Annotated
 
 help_msg: str = "Create an ical file with the shifts for the next month"
 app = typer.Typer(add_completion=False, help=help_msg)
 
 
-@app.command(name="version", help="Shows the current version")
-def version() -> None:
-    typer.echo(get_version("shifts"))
-
-
-@app.command(help=help_msg)
-def cmd(shifts: str):
+@app.command()
+def event(
+    shifts: Annotated[
+        str,
+        typer.Argument(
+            show_default=False,
+            help="A string with each shift code, one per day of the month",
+        ),
+    ]
+):
+    """
+    Example: shifts "M T N D M T N D M T N D M T N D M T N D M T N D M T N D N N N"
+    """
     c = Calendar()
     year, month = next_year_month()
     try:
         clean_shifts = validate_shifts(shifts, year, month)
     except ValueError as e:
         typer.echo(f"Invalid shifts found, {str(e)}", err=True)
-        sys.exit(1)
+        raise typer.Exit(code=1)
 
     for day, shift in enumerate(clean_shifts, start=1):
         if shift == "D":
             continue
         s = Shift(shift, year, month, day)
         c.events.add(
             Event(
@@ -65,14 +70,17 @@
 
     :param shifts: The string with of shifts to validate
     :param year: The year the shifts will be in
     :param month: The month the shifts will be in
     :return: A list of shifts
     """
 
+    if " " not in shifts or not shifts.count(" ") > 10:
+        raise ValueError(f"'{shifts}' is not a valid option")
+
     _, number_of_days = calendar.monthrange(year, month)
     shifts = [item.upper() for item in list(shifts) if item.strip()]  # type: ignore
     if len(shifts) != number_of_days:
         raise ValueError(f"expected {number_of_days} shifts, but got {len(shifts)}")
 
     return shifts
```

### Comparing `shifts-0.0.4/PKG-INFO` & `shifts-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shifts
-Version: 0.0.4
+Version: 0.1.0
 Summary: Converts shifts to a ical file
 License: Unlicense
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

