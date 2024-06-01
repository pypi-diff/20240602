# Comparing `tmp/apyanki-0.15.7.tar.gz` & `tmp/apyanki-0.15.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apyanki-0.15.7.tar", max compression
+gzip compressed data, was "apyanki-0.15.8.tar", max compression
```

## Comparing `apyanki-0.15.7.tar` & `apyanki-0.15.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2023-06-03 19:56:02.857177 apyanki-0.15.7/LICENSE.md
--rw-r--r--   0        0        0    11250 2024-04-19 20:43:04.288990 apyanki-0.15.7/README.md
--rw-r--r--   0        0        0     1561 2024-05-29 21:45:57.695206 apyanki-0.15.7/pyproject.toml
--rw-r--r--   0        0        0      362 2024-04-11 17:02:39.255040 apyanki-0.15.7/src/apyanki/__init__.py
--rw-r--r--   0        0        0    16926 2024-05-28 21:27:16.653454 apyanki-0.15.7/src/apyanki/anki.py
--rw-r--r--   0        0        0     1964 2024-04-11 17:02:57.515160 apyanki-0.15.7/src/apyanki/cards.py
--rw-r--r--   0        0        0    14650 2024-05-29 19:46:44.352978 apyanki-0.15.7/src/apyanki/cli.py
--rw-r--r--   0        0        0     2064 2024-04-19 20:39:20.334116 apyanki-0.15.7/src/apyanki/config.py
--rw-r--r--   0        0        0     1259 2024-03-22 19:17:12.627164 apyanki-0.15.7/src/apyanki/console.py
--rw-r--r--   0        0        0     9169 2024-04-19 20:40:01.254397 apyanki-0.15.7/src/apyanki/fields.py
--rw-r--r--   0        0        0    23404 2024-05-29 21:40:29.856826 apyanki-0.15.7/src/apyanki/note.py
--rw-r--r--   0        0        0     3051 2024-05-28 21:27:15.306780 apyanki-0.15.7/src/apyanki/utilities.py
--rw-r--r--   0        0        0    12312 1970-01-01 00:00:00.000000 apyanki-0.15.7/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-08 13:41:15.230284 apyanki-0.15.8/LICENSE.md
+-rw-r--r--   0        0        0    11250 2024-05-08 13:41:15.230284 apyanki-0.15.8/README.md
+-rw-r--r--   0        0        0     1561 2024-06-01 23:20:58.603571 apyanki-0.15.8/pyproject.toml
+-rw-r--r--   0        0        0      362 2024-05-08 13:41:15.230284 apyanki-0.15.8/src/apyanki/__init__.py
+-rw-r--r--   0        0        0    16926 2024-06-01 18:26:06.083567 apyanki-0.15.8/src/apyanki/anki.py
+-rw-r--r--   0        0        0     1964 2024-05-08 13:41:15.230284 apyanki-0.15.8/src/apyanki/cards.py
+-rw-r--r--   0        0        0    14900 2024-06-01 23:19:57.178576 apyanki-0.15.8/src/apyanki/cli.py
+-rw-r--r--   0        0        0     2064 2024-05-08 13:41:15.233617 apyanki-0.15.8/src/apyanki/config.py
+-rw-r--r--   0        0        0     1259 2024-05-08 13:41:15.233617 apyanki-0.15.8/src/apyanki/console.py
+-rw-r--r--   0        0        0     9169 2024-05-08 13:41:15.233617 apyanki-0.15.8/src/apyanki/fields.py
+-rw-r--r--   0        0        0    23748 2024-06-01 18:47:26.597756 apyanki-0.15.8/src/apyanki/note.py
+-rw-r--r--   0        0        0     3051 2024-06-01 18:26:06.083567 apyanki-0.15.8/src/apyanki/utilities.py
+-rw-r--r--   0        0        0    12312 1970-01-01 00:00:00.000000 apyanki-0.15.8/PKG-INFO
```

### Comparing `apyanki-0.15.7/LICENSE.md` & `apyanki-0.15.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.7/README.md` & `apyanki-0.15.8/README.md`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.7/pyproject.toml` & `apyanki-0.15.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apyanki"
-version = "0.15.7"
+version = "0.15.8"
 description = "CLI script for interacting with local Anki collection"
 authors = ["Karl Yngve Lervåg <karl.yngve@lervag.net>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `apyanki-0.15.7/src/apyanki/anki.py` & `apyanki-0.15.8/src/apyanki/anki.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.7/src/apyanki/cards.py` & `apyanki-0.15.8/src/apyanki/cards.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.7/src/apyanki/cli.py` & `apyanki-0.15.8/src/apyanki/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,19 +139,20 @@
 def add_from_file(file: Path, tags: str, deck: str) -> None:
     """Add notes from Markdown file.
 
     The example below should adequately specify the syntax. Any initial "key: value"
     pairs specify default values for all the following notes. The following keys are
     accepted:
 
+    \b
     * model:    The note model (required)
     * tags:     The note model (optional)
     * deck:     Which deck the note should be added to (optional)
-    * markdown: Set to "false" or "no" if apy should not use a markdown converter while
-                converting the input note to an Anki note. (optional)
+    * markdown: Set to "false" or "no" if apy should not use a markdown converter
+                while converting the input note to an Anki note. (optional)
 
     Here is the example Markdown input:
 
         // example.md
         model: Basic
         tags: marked
 
@@ -233,16 +234,17 @@
         for key in cfg.keys():
             console.print(f"Config loaded:     {key}")
         console.print(f"Config file:       {cfg_file}")
     else:
         console.print("Config file:       Not found")
 
     with Anki(**cfg) as a:
+        scheduler = 3 if a.col.v3_scheduler() else a.col.sched_ver()
         console.print(f"Collection path:   {a.col.path}")
-        console.print(f"Scheduler version: {a.col.sched_ver()}")
+        console.print(f"Scheduler version: {scheduler}")
 
         if a.col.decks.count() > 1:
             console.print("Decks:")
             for name in sorted(a.deck_names):
                 console.print(f"  - {name}")
 
         sum_notes = a.col.note_count()
@@ -378,19 +380,28 @@
         if check_markdown_consistency:
             notes += [
                 n
                 for n in a.find_notes(f"rated:{cmc_range}")
                 if not n.has_consistent_markdown()
             ]
 
+        i = 0
         number_of_notes = len(notes)
-        for i, note in enumerate(notes):
-            if not note.review(i, number_of_notes):
+        while i < number_of_notes:
+            note = notes[i]
+            status = note.review(i, number_of_notes)
+
+            if status == "stop":
                 break
 
+            if status == "rewind":
+                i = max(i - 1, 0)
+            else:
+                i += 1
+
 
 @main.command()
 def sync() -> None:
     """Synchronize collection with AnkiWeb."""
     with Anki(**cfg) as a:
         a.sync()
```

### Comparing `apyanki-0.15.7/src/apyanki/config.py` & `apyanki-0.15.8/src/apyanki/config.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.7/src/apyanki/console.py` & `apyanki-0.15.8/src/apyanki/console.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.7/src/apyanki/fields.py` & `apyanki-0.15.8/src/apyanki/fields.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.7/src/apyanki/note.py` & `apyanki-0.15.8/src/apyanki/note.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import dataclass
 import os
 from pathlib import Path
 import re
 from subprocess import DEVNULL, Popen
 import tempfile
 from time import localtime, strftime
-from typing import Any, Optional, TYPE_CHECKING
+from typing import Any, Literal, Optional, TYPE_CHECKING
 
 from click import Abort
 import readchar
 from rich.columns import Columns
 from rich.markdown import Markdown
 from rich.table import Table
 from rich.text import Text
@@ -267,17 +267,21 @@
             break
 
         fields: dict[str, str] = {}
         first_field: str = model["flds"][0]["name"]
         for field in model["flds"]:
             fields[field["name"]] = ""
 
+        fields[first_field] = f"Created from Note {self.n.id}\n\n"
         for old_field_name, old_field in self.n.items():
             fields[first_field] += f"### {old_field_name}\n{old_field}\n"
 
+        if model["name"] == "Cloze":
+            fields[first_field] += "\nCloze card needs clozes: {{c1::content}}"
+
         note_data = NoteData(
             model["name"],
             " ".join(self.n.tags),
             fields,
             any(check_if_generated_from_markdown(f) for f in self.n.values()),
         )
 
@@ -382,35 +386,36 @@
         return ", ".join(self.n.tags)
 
     def review(
         self,
         i: Optional[int] = None,
         number_of_notes: Optional[int] = None,
         remove_actions: Optional[list[str]] = None,
-    ) -> bool:
+    ) -> Literal["stop", "continue", "rewind"]:
         """Interactive review of the note
 
         This method is used by the review command.
 
         if the arguments "i" and "number_of_notes" are supplied, then they are
         displayed to show review progress.
 
         The "remove_actions" argument can be used to remove a default action
         from the action menu.
         """
 
         actions = {
             "c": "Continue",
+            "p": "Go back",
             "e": "Edit",
             "a": "Add new",
             "d": "Delete",
             "m": "Toggle markdown",
             "*": "Toggle marked",
             "z": "Toggle suspend",
-            "p": "Toggle pprint",
+            "P": "Toggle pprint",
             "F": "Clear flags",
             "R": "Reset progress",
             "f": "Show images",
             "E": "Edit CSS",
             "D": "Change deck",
             "N": "Change model",
             "s": "Save and stop",
@@ -455,15 +460,18 @@
                 self.pprint(print_raw_fields, list_cards=show_cards)
 
             refresh = True
             choice = readchar.readchar()
             action = actions.get(choice)
 
             if action == "Continue":
-                return True
+                return "continue"
+
+            if action == "Go back":
+                return "rewind"
 
             if action == "Edit":
                 self.edit()
                 continue
 
             if action == "Add new":
                 notes = self.a.add_notes_with_editor(
@@ -476,15 +484,15 @@
                 console.wait_for_keypress()
                 continue
 
             if action == "Delete" and console.confirm(
                 "Are you sure you want to delete the note?"
             ):
                 self.delete()
-                return True
+                return "continue"
 
             if action == "Toggle markdown":
                 self.toggle_markdown()
                 continue
 
             if action == "Toggle marked":
                 self.toggle_marked()
@@ -523,15 +531,15 @@
                 new_note = self.change_model()
                 if new_note is not None:
                     return new_note.review(i, number_of_notes)
                 continue
 
             if action == "Save and stop":
                 console.print("Stopped")
-                return False
+                return "stop"
 
             if action == "Show cards":
                 show_cards = not show_cards
                 continue
 
 
 @dataclass
@@ -572,15 +580,15 @@
             convert_text_to_field(f, use_markdown=self.markdown)
             for f in self.fields.values()
         ]
 
         for tag in self.tags.strip().split():
             new_note.add_tag(tag)
 
-        if not new_note.dupeOrEmpty():
+        if not new_note.duplicate_or_empty():
             anki.col.addNote(new_note)
             anki.modified = True
         else:
             field_name, field_value = list(self.fields.items())[0]
             console.print("[red]Dupe detected, new_note was not added!")
             console.print(f"First field: {field_name}")
             console.print(f"First value: {field_value}")
```

### Comparing `apyanki-0.15.7/src/apyanki/utilities.py` & `apyanki-0.15.8/src/apyanki/utilities.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.7/PKG-INFO` & `apyanki-0.15.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apyanki
-Version: 0.15.7
+Version: 0.15.8
 Summary: CLI script for interacting with local Anki collection
 Home-page: https://github.com/lervag/apy
 Author: Karl Yngve Lervåg
 Author-email: karl.yngve@lervag.net
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

