# Comparing `tmp/felicien-0.7.0.tar.gz` & `tmp/felicien-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felicien-0.7.0.tar", max compression
+gzip compressed data, was "felicien-0.8.0.tar", max compression
```

## Comparing `felicien-0.7.0.tar` & `felicien-0.8.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2024-05-29 13:38:35.442392 felicien-0.7.0/LICENSE
--rw-r--r--   0        0        0     2599 2024-05-29 13:38:35.443392 felicien-0.7.0/README.md
--rw-r--r--   0        0        0      142 2024-05-29 13:38:35.449392 felicien-0.7.0/felicien/__init__.py
--rw-r--r--   0        0        0     6695 2024-05-29 13:38:35.449392 felicien-0.7.0/felicien/feliconnector.py
--rw-r--r--   0        0        0    14077 2024-05-29 13:38:35.449392 felicien-0.7.0/felicien/felits.py
--rw-r--r--   0        0        0     1067 2024-05-29 13:38:35.450392 felicien-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 felicien-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-06-02 15:33:43.357796 felicien-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2599 2024-06-02 15:33:43.357796 felicien-0.8.0/README.md
+-rw-r--r--   0        0        0      142 2024-06-02 15:33:43.363796 felicien-0.8.0/felicien/__init__.py
+-rw-r--r--   0        0        0     6695 2024-06-02 15:33:43.363796 felicien-0.8.0/felicien/feliconnector.py
+-rw-r--r--   0        0        0    15567 2024-06-02 15:33:43.363796 felicien-0.8.0/felicien/felits.py
+-rw-r--r--   0        0        0     1067 2024-06-02 15:33:43.364796 felicien-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 felicien-0.8.0/PKG-INFO
```

### Comparing `felicien-0.7.0/LICENSE` & `felicien-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `felicien-0.7.0/README.md` & `felicien-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `felicien-0.7.0/felicien/feliconnector.py` & `felicien-0.8.0/felicien/feliconnector.py`

 * *Files identical despite different names*

### Comparing `felicien-0.7.0/felicien/felits.py` & `felicien-0.8.0/felicien/felits.py`

 * *Files 8% similar despite different names*

```diff
@@ -369,25 +369,62 @@
         return self.data.asfreq(freq=self.frequency)
 
     def longest_continuous_segment(self, position: str = "last") -> pd.Series:
         """Extract the longest continuous segment, which is the longest
             segment of the timeserie respecting the frequency, without any
             missing point
 
+            DEPRECATED: use `continuous_segment` function instead
+
+        Args:
+            position (str, optional): Which longest segment to return, in case
+                multiple segment exist
+                Defaults to last.
+
+        Returns:
+            pd.Series: the extract of the timeserie
+
+        Raises:
+            ValueError if the position argument is not "first" or "last"
+        """
+        # validate arguments
+        if position not in ["first", "last"]:
+            raise ValueError(
+                f"position argument must be 'first' or 'last', not {position}"
+            )
+
+        return self.continuous_segment(position=position, longest=True)
+
+    def continuous_segment(
+        self, position: str = "last", longest: bool = False
+    ) -> pd.Series:
+        """Extract continuous segment from the timeserie respecting the
+            frequency, without any missing point. This segment can be the
+            longest, or any length, but it has to be eother the first segment
+            or the last from the timeserie.
+
         Args:
             position (str, optional): Which longest segment to return, in case
                 multiple segment exist
                 Defaults to last.
+            longest (bool, optional): Should the segment be the longest
+                Defaults to False.
 
         Returns:
             pd.Series: the extract of the timeserie
 
         Raises:
             ValueError if the position argument is not "first" or "last"
         """
+        # validate arguments
+        if position not in ["first", "last"]:
+            raise ValueError(
+                f"position argument must be 'first' or 'last', not {position}"
+            )
+
         # case of series with maximum 2 points
         if self.size <= 2:
             return self.data
 
         # create an array stating if two points are separated by
         # exactly 1 frequency
         segments = self.data.index.diff() == self.frequency  # type: ignore
@@ -396,25 +433,28 @@
         longest_length = max(
             len(list(y)) if is_freq else 0
             for (is_freq, y) in itertools.groupby(segments)
         )
 
         # finding the position of the longest segment (first or last)
         start_position = 0
+        end_position = 0
         cursor = 0
         for is_freq, segment in itertools.groupby(segments):
             local_segment = list(segment)
             # case where the frequency matches and the length of
             # the segment is the longest
-            if is_freq and len(local_segment) == longest_length:
+            if is_freq and (
+                (longest and len(local_segment) == longest_length)
+                or (not longest)
+            ):
                 start_position = cursor
+                end_position = start_position + len(local_segment)
 
                 # in case we found the first longest segment
                 if position == "first":
                     break
 
             # move current cursor along the serie
             cursor += len(local_segment)
 
-        return self.data.iloc[
-            start_position - 1 : start_position + longest_length  # noqa E203
-        ]
+        return self.data.iloc[start_position - 1 : end_position]  # noqa E203
```

### Comparing `felicien-0.7.0/pyproject.toml` & `felicien-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "felicien"
-version = "0.7.0"
+version = "0.8.0"
 description = "Felicien is you companion to retrieve timeseries from a TSDB, to transform it in various format and to push it to a TSDB."
 authors = ["Julien Andrieux <chilladx@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "felicien" },
 ]
```

### Comparing `felicien-0.7.0/PKG-INFO` & `felicien-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felicien
-Version: 0.7.0
+Version: 0.8.0
 Summary: Felicien is you companion to retrieve timeseries from a TSDB, to transform it in various format and to push it to a TSDB.
 License: MIT
 Author: Julien Andrieux
 Author-email: chilladx@pm.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

