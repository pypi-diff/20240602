# Comparing `tmp/python-table-print-0.2.tar.gz` & `tmp/python_table_print-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-table-print-0.2.tar", last modified: Sun Mar 24 00:36:08 2024, max compression
+gzip compressed data, was "python_table_print-0.3.tar", last modified: Sun Jun  2 11:17:34 2024, max compression
```

## Comparing `python-table-print-0.2.tar` & `python_table_print-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 00:36:08.090696 python-table-print-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-24 00:35:58.000000 python-table-print-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-03-24 00:36:08.086696 python-table-print-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-03-24 00:35:58.000000 python-table-print-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-24 00:35:58.000000 python-table-print-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 00:36:08.090696 python-table-print-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 00:36:08.086696 python-table-print-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 00:36:08.086696 python-table-print-0.2/src/python_table_print/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-24 00:35:58.000000 python-table-print-0.2/src/python_table_print/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-24 00:35:58.000000 python-table-print-0.2/src/python_table_print/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-03-24 00:35:58.000000 python-table-print-0.2/src/python_table_print/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 00:36:08.086696 python-table-print-0.2/src/python_table_print.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-03-24 00:36:08.000000 python-table-print-0.2/src/python_table_print.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-24 00:36:08.000000 python-table-print-0.2/src/python_table_print.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 00:36:08.000000 python-table-print-0.2/src/python_table_print.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-24 00:36:08.000000 python-table-print-0.2/src/python_table_print.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 00:36:08.086696 python-table-print-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-03-24 00:35:58.000000 python-table-print-0.2/tests/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:17:34.574646 python_table_print-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-06-02 11:17:29.000000 python_table_print-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-06-02 11:17:34.574646 python_table_print-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-06-02 11:17:29.000000 python_table_print-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-06-02 11:17:29.000000 python_table_print-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 11:17:34.574646 python_table_print-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:17:34.574646 python_table_print-0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:17:34.574646 python_table_print-0.3/src/python_table_print/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 11:17:29.000000 python_table_print-0.3/src/python_table_print/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-06-02 11:17:29.000000 python_table_print-0.3/src/python_table_print/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-06-02 11:17:29.000000 python_table_print-0.3/src/python_table_print/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:17:34.574646 python_table_print-0.3/src/python_table_print.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-06-02 11:17:34.000000 python_table_print-0.3/src/python_table_print.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-02 11:17:34.000000 python_table_print-0.3/src/python_table_print.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 11:17:34.000000 python_table_print-0.3/src/python_table_print.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-02 11:17:34.000000 python_table_print-0.3/src/python_table_print.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 11:17:34.574646 python_table_print-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-06-02 11:17:29.000000 python_table_print-0.3/tests/test_table.py
```

### Comparing `python-table-print-0.2/LICENSE` & `python_table_print-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-table-print-0.2/PKG-INFO` & `python_table_print-0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-table-print
-Version: 0.2
+Version: 0.3
 Summary: Allows for pretty printing and automatic resizing of tables.
 Author: Centauri_Prime
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -168,7 +168,71 @@
 *       Entry 1 * Entry number 2     *     Entry 3 baby      *
 * Another entry *        yay         * an entry in the table *
 *     Fun times * This is kinda cool *         wooow         *
 **************************************************************
 ```
 
 Notice how in the above examples the justifications of the edited cells were overwritten with the latest justification.
+
+## Title
+
+You can add a title to your table. Defaults to centre justification
+
+```python
+...
+
+my_table.set_title("Title")
+```
+
+Output:
+```
+**************************************************************
+*                           Title                            *
+**************************************************************
+*         Col 1 * Col 2              * Col 3                 *
+**************************************************************
+*       Entry 1 * Entry number 2     *     Entry 3 baby      *
+* Another entry *        yay         * an entry in the table *
+*     Fun times * This is kinda cool *         wooow         *
+**************************************************************
+```
+
+Clearing a title:
+
+```python
+...
+
+my_table.clear_title()
+```
+
+Output:
+```
+**************************************************************
+*       Entry 1 * Entry number 2     *     Entry 3 baby      *
+* Another entry *        yay         * an entry in the table *
+*     Fun times * This is kinda cool *         wooow         *
+**************************************************************\
+```
+
+### Justification for Title
+
+You can change the justification of your title:
+
+```python
+...
+
+my_table.set_title("Title")
+my_table.set_title_justification(Justification.LEFT)
+```
+
+Output:
+```
+**************************************************************
+* Title                                                      *
+**************************************************************
+*         Col 1 * Col 2              * Col 3                 *
+**************************************************************
+*       Entry 1 * Entry number 2     *     Entry 3 baby      *
+* Another entry *        yay         * an entry in the table *
+*     Fun times * This is kinda cool *         wooow         *
+**************************************************************
+```
```

### Comparing `python-table-print-0.2/README.md` & `python_table_print-0.3/src/python_table_print.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: python-table-print
+Version: 0.3
+Summary: Allows for pretty printing and automatic resizing of tables.
+Author: Centauri_Prime
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Python Table Print
 A project to dynamically scale and print tables using text in Python
 
 # Usage
 
 Python Table Print is object-oriented. This means that a `PrintTable` object gets instantiated and added to/edited. When the table is ready to be printed/created, this can be done by calling the `get_table` method. An example can be found in `example.py`, but is copied here for convenience:
 
@@ -155,8 +167,72 @@
 **************************************************************
 *       Entry 1 * Entry number 2     *     Entry 3 baby      *
 * Another entry *        yay         * an entry in the table *
 *     Fun times * This is kinda cool *         wooow         *
 **************************************************************
 ```
 
-Notice how in the above examples the justifications of the edited cells were overwritten with the latest justification.
+Notice how in the above examples the justifications of the edited cells were overwritten with the latest justification.
+
+## Title
+
+You can add a title to your table. Defaults to centre justification
+
+```python
+...
+
+my_table.set_title("Title")
+```
+
+Output:
+```
+**************************************************************
+*                           Title                            *
+**************************************************************
+*         Col 1 * Col 2              * Col 3                 *
+**************************************************************
+*       Entry 1 * Entry number 2     *     Entry 3 baby      *
+* Another entry *        yay         * an entry in the table *
+*     Fun times * This is kinda cool *         wooow         *
+**************************************************************
+```
+
+Clearing a title:
+
+```python
+...
+
+my_table.clear_title()
+```
+
+Output:
+```
+**************************************************************
+*       Entry 1 * Entry number 2     *     Entry 3 baby      *
+* Another entry *        yay         * an entry in the table *
+*     Fun times * This is kinda cool *         wooow         *
+**************************************************************\
+```
+
+### Justification for Title
+
+You can change the justification of your title:
+
+```python
+...
+
+my_table.set_title("Title")
+my_table.set_title_justification(Justification.LEFT)
+```
+
+Output:
+```
+**************************************************************
+* Title                                                      *
+**************************************************************
+*         Col 1 * Col 2              * Col 3                 *
+**************************************************************
+*       Entry 1 * Entry number 2     *     Entry 3 baby      *
+* Another entry *        yay         * an entry in the table *
+*     Fun times * This is kinda cool *         wooow         *
+**************************************************************
+```
```

### Comparing `python-table-print-0.2/pyproject.toml` & `python_table_print-0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-table-print"
-version = "0.2"
+version = "0.3"
 authors = [
     {"name" = "Centauri_Prime"}
 ]
 description = "Allows for pretty printing and automatic resizing of tables."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `python-table-print-0.2/src/python_table_print/example.py` & `python_table_print-0.3/src/python_table_print/example.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,7 +47,37 @@
 print("\n\n")
 
 my_table.set_cell_justification(1, 1, Justification.LEFT)
 
 print("Table With One Cell Left-Justified\n")
 print(my_table.get_table())
 print("\n\n")
+
+my_table.set_title("Title")
+
+print("Table With Title With Centre Justification\n")
+print(my_table.get_table())
+print("\n\n")
+
+my_table.set_title_justification(Justification.LEFT)
+
+print("Table With Title With Left Justification\n")
+print(my_table.get_table())
+print("\n\n")
+
+my_table.set_title_justification(Justification.RIGHT)
+
+print("Table With Title With Right Justification\n")
+print(my_table.get_table())
+print("\n\n")
+
+my_table.set_title("This title is just way way too long and it wil be truncated")
+
+print("Table With A Truncated Title")
+print(my_table.get_table())
+print("\n\n")
+
+my_table.clear_title()
+
+print("Table With Cleared Title\n")
+print(my_table.get_table())
+print("\n\n")
```

### Comparing `python-table-print-0.2/src/python_table_print/table.py` & `python_table_print-0.3/src/python_table_print/table.py`

 * *Files 17% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 return self._print_as_centre_justified(max_length, border_character)
 
             case Justification.RIGHT:
                 return self._print_as_right_justified(max_length, border_character)
 
             # TODO: Raise an "Unknown Justification" exception
             case _:
-                raise Exception
+                raise Exception()
 
 
 class _Column:
     """An abstraction of the column of the table, which holds information about the column"""
 
     def __init__(self) -> None:
         self.max_length = 0
@@ -163,14 +163,16 @@
     def __init__(self) -> None:
         self.has_header_row: bool = True
 
         # TODO: Is a dictionary whose keys are ints essentially a list in Python?
         self._columns: dict[int, _Column] = {}
         self._rows: dict[int, _Row] = {}
         self._border_character = BASE_BORDER
+        self._title: str | None = None
+        self._title_justification: Justification = Justification.CENTRE
 
     def _check_and_increase_max_column_length(self, column_i: int, length: int) -> None:
         """Takes in the column number and the length of the new string at that column and changes the length to the given length if longer, or if that column doesn't yet exist.
 
         Args:
             column (int): The column at which this is ocurring
             length (int): The length of the new string
@@ -182,15 +184,15 @@
             return
 
         # Check if this length is longer than the currently stored one. If so, update
         if length > self._columns[column_i].max_length:
             self._columns[column_i].max_length = length
 
     def _total_border_length(self) -> int:
-        """Figures out the length of the table
+        """Figures out the length of the table, including the two border characters themselves
 
         Returns:
             int: The length of the table
         """
         total_border_length = 0
 
         for col_len in self._columns.values():
@@ -222,14 +224,72 @@
             row.get_row_as_string(
                 border_character,
                 [column.max_length for column in self._columns.values()],
             )
             + self._get_border_row()
         )
 
+    def _get_title_row(self, border_character: str) -> str:
+        """Creates the title row for the table if the title is set. Otherwise returns just the top border row
+
+        NOTE: For now, we will cut off the title if it's too long. This will be fixed in GitHub Issue #61
+        NOTE: For now, we only support centre-justifying the title. This will be addressed in GitHub Issue #62
+
+        Args:
+            border_character (str): The border character
+
+        Returns:
+            str: The title of the table, or an empty string if the title is not set
+        """
+
+        if not self._title:
+            return self._get_border_row()
+
+        # We want to cut off the title (for now) to not go passed the length of the table
+        title = self._title[: self._total_border_length() - 4]
+
+        length_without_borders = self._total_border_length() - 4
+
+        match self._title_justification:
+            case Justification.LEFT:
+                title = (
+                    self._border_character
+                    + " "
+                    + title
+                    + (" " * (length_without_borders - len(title) + 1))
+                    + border_character
+                    + "\n"
+                )
+
+            case Justification.CENTRE:
+                title = (
+                    self._border_character
+                    + " " * (floor((length_without_borders - len(title)) / 2) + 1)
+                    + title
+                    + " " * (ceil((length_without_borders - len(title)) / 2) + 1)
+                    + self._border_character
+                    + "\n"
+                )
+
+            case Justification.RIGHT:
+                title = (
+                    self._border_character
+                    + " " * (length_without_borders - len(title) + 1)
+                    + title
+                    + " "
+                    + self._border_character
+                    + "\n"
+                )
+
+            case _:
+                # TODO: Raise "Unsupported Justification" Exception
+                raise Exception()
+
+        return self._get_border_row() + title + self._get_border_row()
+
     def add_row(self, *row: str) -> None:
         """Adds another row to the bottom of the table
 
         Args:
             row (*str): The next row of text to be added to the table
         """
         for col_i in range(0, len(row)):
@@ -288,19 +348,44 @@
         Returns:
             str: The currenct table
         """
         if len(self._rows) == 0:
             # TODO: Throw a "table has no length" exception
             raise Exception
 
-        table = self._get_border_row()
+        table = self._get_title_row(self._border_character)
 
         if self.has_header_row:
             table += self._get_header(self._rows[0], self._border_character)
 
         for i in range(1 if self.has_header_row else 0, len(self._rows)):
             table += self._rows[i].get_row_as_string(
                 self._border_character,
                 [column.max_length for column in self._columns.values()],
             )
 
         return table + self._get_border_row()
+
+    def clear_title(self) -> None:
+        """Clears the title, by setting it to None"""
+        self._title = None
+        self._title_justification = Justification.CENTRE
+
+    def set_title(
+        self, title: str, title_justification: Justification = Justification.CENTRE
+    ) -> None:
+        """Sets the title and the title's justification.
+
+        Args:
+            title (str): The new title of the table
+            justification (Justification): The justification for the title of the table. If no justification is passed in, defaults to Justification.CENTRE
+        """
+        self._title = title
+        self._title_justification = title_justification
+
+    def set_title_justification(self, title_justification: Justification) -> None:
+        """Sets the title's justification
+
+        Args:
+            title_justification (Justification): The justification for the title
+        """
+        self._title_justification = title_justification
```

### Comparing `python-table-print-0.2/src/python_table_print.egg-info/PKG-INFO` & `python_table_print-0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: python-table-print
-Version: 0.2
-Summary: Allows for pretty printing and automatic resizing of tables.
-Author: Centauri_Prime
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python Table Print
 A project to dynamically scale and print tables using text in Python
 
 # Usage
 
 Python Table Print is object-oriented. This means that a `PrintTable` object gets instantiated and added to/edited. When the table is ready to be printed/created, this can be done by calling the `get_table` method. An example can be found in `example.py`, but is copied here for convenience:
 
@@ -168,7 +156,71 @@
 *       Entry 1 * Entry number 2     *     Entry 3 baby      *
 * Another entry *        yay         * an entry in the table *
 *     Fun times * This is kinda cool *         wooow         *
 **************************************************************
 ```
 
 Notice how in the above examples the justifications of the edited cells were overwritten with the latest justification.
+
+## Title
+
+You can add a title to your table. Defaults to centre justification
+
+```python
+...
+
+my_table.set_title("Title")
+```
+
+Output:
+```
+**************************************************************
+*                           Title                            *
+**************************************************************
+*         Col 1 * Col 2              * Col 3                 *
+**************************************************************
+*       Entry 1 * Entry number 2     *     Entry 3 baby      *
+* Another entry *        yay         * an entry in the table *
+*     Fun times * This is kinda cool *         wooow         *
+**************************************************************
+```
+
+Clearing a title:
+
+```python
+...
+
+my_table.clear_title()
+```
+
+Output:
+```
+**************************************************************
+*       Entry 1 * Entry number 2     *     Entry 3 baby      *
+* Another entry *        yay         * an entry in the table *
+*     Fun times * This is kinda cool *         wooow         *
+**************************************************************\
+```
+
+### Justification for Title
+
+You can change the justification of your title:
+
+```python
+...
+
+my_table.set_title("Title")
+my_table.set_title_justification(Justification.LEFT)
+```
+
+Output:
+```
+**************************************************************
+* Title                                                      *
+**************************************************************
+*         Col 1 * Col 2              * Col 3                 *
+**************************************************************
+*       Entry 1 * Entry number 2     *     Entry 3 baby      *
+* Another entry *        yay         * an entry in the table *
+*     Fun times * This is kinda cool *         wooow         *
+**************************************************************
+```
```

### Comparing `python-table-print-0.2/tests/test_table.py` & `python_table_print-0.3/tests/test_table.py`

 * *Files 20% similar despite different names*

```diff
@@ -220,7 +220,134 @@
 **************************************************************
 *    Entry 1    *   Entry number 2   *          Entry 3 baby *
 * Another entry * yay                * an entry in the table *
 * Fun times     * This is kinda cool *         wooow         *
 **************************************************************
 """
     )
+
+
+def test_table_with_title_centred():
+    table = PrintTable()
+
+    table.add_row("Col 1", "Col 2", "Col 3")
+    table.add_row("Entry 1", "Entry number 2", "Entry 3 baby")
+    table.add_row("Another entry", "yay", "an entry in the table")
+    table.add_row("Fun times", "This is kinda cool", "wooow")
+
+    table.set_title("Title")
+
+    assert (
+        table.get_table()
+        == """**************************************************************
+*                           Title                            *
+**************************************************************
+* Col 1         * Col 2              * Col 3                 *
+**************************************************************
+* Entry 1       * Entry number 2     * Entry 3 baby          *
+* Another entry * yay                * an entry in the table *
+* Fun times     * This is kinda cool * wooow                 *
+**************************************************************
+"""
+    )
+
+
+def test_table_with_title_left_justified():
+    table = PrintTable()
+
+    table.add_row("Col 1", "Col 2", "Col 3")
+    table.add_row("Entry 1", "Entry number 2", "Entry 3 baby")
+    table.add_row("Another entry", "yay", "an entry in the table")
+    table.add_row("Fun times", "This is kinda cool", "wooow")
+
+    table.set_title("Title", Justification.LEFT)
+
+    assert (
+        table.get_table()
+        == """**************************************************************
+* Title                                                      *
+**************************************************************
+* Col 1         * Col 2              * Col 3                 *
+**************************************************************
+* Entry 1       * Entry number 2     * Entry 3 baby          *
+* Another entry * yay                * an entry in the table *
+* Fun times     * This is kinda cool * wooow                 *
+**************************************************************
+"""
+    )
+
+
+def test_table_with_title_right_justified():
+    table = PrintTable()
+
+    table.add_row("Col 1", "Col 2", "Col 3")
+    table.add_row("Entry 1", "Entry number 2", "Entry 3 baby")
+    table.add_row("Another entry", "yay", "an entry in the table")
+    table.add_row("Fun times", "This is kinda cool", "wooow")
+
+    table.set_title("Title")
+    table.set_title_justification(Justification.RIGHT)
+
+    assert (
+        table.get_table()
+        == """**************************************************************
+*                                                      Title *
+**************************************************************
+* Col 1         * Col 2              * Col 3                 *
+**************************************************************
+* Entry 1       * Entry number 2     * Entry 3 baby          *
+* Another entry * yay                * an entry in the table *
+* Fun times     * This is kinda cool * wooow                 *
+**************************************************************
+"""
+    )
+
+
+def test_table_with_a_very_long_title():
+    table = PrintTable()
+
+    table.add_row("Col 1", "Col 2", "Col 3")
+    table.add_row("Entry 1", "Entry number 2", "Entry 3 baby")
+    table.add_row("Another entry", "yay", "an entry in the table")
+    table.add_row("Fun times", "This is kinda cool", "wooow")
+
+    table.set_title(
+        "This is a title that is way, way, way, way, way, way too long and will certainly be truncated"
+    )
+
+    assert (
+        table.get_table()
+        == """**************************************************************
+* This is a title that is way, way, way, way, way, way too l *
+**************************************************************
+* Col 1         * Col 2              * Col 3                 *
+**************************************************************
+* Entry 1       * Entry number 2     * Entry 3 baby          *
+* Another entry * yay                * an entry in the table *
+* Fun times     * This is kinda cool * wooow                 *
+**************************************************************
+"""
+    )
+
+
+def test_table_with_a_cleared_title():
+    table = PrintTable()
+
+    table.add_row("Col 1", "Col 2", "Col 3")
+    table.add_row("Entry 1", "Entry number 2", "Entry 3 baby")
+    table.add_row("Another entry", "yay", "an entry in the table")
+    table.add_row("Fun times", "This is kinda cool", "wooow")
+
+    table.set_title("Title")
+    table.clear_title()
+
+    assert (
+        table.get_table()
+        == """**************************************************************
+* Col 1         * Col 2              * Col 3                 *
+**************************************************************
+* Entry 1       * Entry number 2     * Entry 3 baby          *
+* Another entry * yay                * an entry in the table *
+* Fun times     * This is kinda cool * wooow                 *
+**************************************************************
+"""
+    )
```

