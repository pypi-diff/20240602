# Comparing `tmp/vicodepy-0.4.2.tar.gz` & `tmp/vicodepy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicodepy-0.4.2.tar", last modified: Sat Jun  1 10:38:51 2024, max compression
+gzip compressed data, was "vicodepy-0.4.3.tar", last modified: Sun Jun  2 16:38:25 2024, max compression
```

## Comparing `vicodepy-0.4.2.tar` & `vicodepy-0.4.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1564 2024-06-01 10:38:44.000000 vicodepy-0.4.2/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-06-01 10:38:44.000000 vicodepy-0.4.2/LICENSE
--rw-r--r--   0        0        0     2758 2024-06-01 10:38:44.000000 vicodepy-0.4.2/README.md
--rw-r--r--   0        0        0      896 2024-06-01 10:38:44.000000 vicodepy-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      818 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/__init__.py
--rw-r--r--   0        0        0      957 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/__main__.py
--rw-r--r--   0        0        0    43076 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/app.py
--rw-r--r--   0        0        0     1323 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/command.py
--rw-r--r--   0        0        0      202 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/config/config.yml
--rw-r--r--   0        0        0       43 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/style.qss
--rw-r--r--   0        0        0     3078 2024-06-01 10:38:44.000000 vicodepy-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1685 2024-06-02 16:38:16.000000 vicodepy-0.4.3/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-06-02 16:38:16.000000 vicodepy-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2837 2024-06-02 16:38:16.000000 vicodepy-0.4.3/README.md
+-rw-r--r--   0        0        0      896 2024-06-02 16:38:16.000000 vicodepy-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      818 2024-06-02 16:38:16.000000 vicodepy-0.4.3/vicodepy/__init__.py
+-rw-r--r--   0        0        0      957 2024-06-02 16:38:16.000000 vicodepy-0.4.3/vicodepy/__main__.py
+-rw-r--r--   0        0        0    43110 2024-06-02 16:38:16.000000 vicodepy-0.4.3/vicodepy/app.py
+-rw-r--r--   0        0        0     1323 2024-06-02 16:38:16.000000 vicodepy-0.4.3/vicodepy/command.py
+-rw-r--r--   0        0        0      202 2024-06-02 16:38:16.000000 vicodepy-0.4.3/vicodepy/config/config.yml
+-rw-r--r--   0        0        0       43 2024-06-02 16:38:16.000000 vicodepy-0.4.3/vicodepy/style.qss
+-rw-r--r--   0        0        0     3157 2024-06-02 16:38:16.000000 vicodepy-0.4.3/PKG-INFO
```

### Comparing `vicodepy-0.4.2/CHANGELOG.md` & `vicodepy-0.4.3/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGELOG
 =========
 
+0.4.3 - 2024-06-02
+------------------
+
+* Use better names for columns in the exported CSV file
+* Improved documentation
+
 0.4.2 - 2024-06-01
 ------------------
 
 * The program accepts now command line arguments
 * Annotation labels can be chosen directly using the keyboard, once the annotation dialog is displayed
 
 0.4.1 - 2024-05-31
```

### Comparing `vicodepy-0.4.2/LICENSE` & `vicodepy-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vicodepy-0.4.2/README.md` & `vicodepy-0.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 ### Playing/stopping the video and moving around it
 
 Once the video is loaded, it can be played and stopped using the space key. The left and right arrow keys can be used for going backward and forward, respectively, by one frame in the video. Positioning the cursor (a black triangle) with the mouse is also possible by clicking and dragging the cursor on the timeline.
 
 ### Annotations
 
-Annotations can be defined by pressing the enter key. This will mark one of the borders of the annotation. The other border can be defined by using the arrow keys or by clicking and dragging the cursor. Once the cursor is at the desired position, type enter again. This will open a dialog window for choosing the label and the color of the annotation. New labels can be defined in the dialog window and will be proposed later when new annotations are created.
+Annotations can be defined by pressing the enter key. This will mark one of the borders of the annotation. The other border can be defined by using the arrow keys or by clicking and dragging the cursor. Once the cursor is at the desired position, type enter again. This will open a dialog window for choosing the label and the color of the annotation. New labels can be defined in the dialog window by simply typing them. The new created labels will appear in the list of proposed labels when new annotations will be subsequently created.
 
 Once an annotation is created, it is possible to change its borders by double-clicking on the annotation. Two handles will appear, one at the left border of the annotation and the other at the right border. Click on a border handle and move it with the left and right arrow keys.
 
 The creation of an annotation can be aborted, once it is start by either typing the Escape key or by clicking on the Abort button in the pop-up window.
 
 The timeline can be zoomed in and out by using the scroll wheel of the mouse.
```

### Comparing `vicodepy-0.4.2/pyproject.toml` & `vicodepy-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vicodepy"
-version = "0.4.2"
+version = "0.4.3"
 description = "Video coder for psychological experiments"
 authors = [
     { name = "Rafael Laboissière", email = "rafael.laboissiere@cnrs.fr" },
     { name = "Esteban Milleret", email = "esteban.milleret@etu.univ-grenoble-alpes.fr" },
 ]
 dependencies = [
     "PySide6==6.7.1",
```

### Comparing `vicodepy-0.4.2/vicodepy/__init__.py` & `vicodepy-0.4.3/vicodepy/__init__.py`

 * *Files identical despite different names*

### Comparing `vicodepy-0.4.2/vicodepy/__main__.py` & `vicodepy-0.4.3/vicodepy/__main__.py`

 * *Files identical despite different names*

### Comparing `vicodepy-0.4.2/vicodepy/app.py` & `vicodepy-0.4.3/vicodepy/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -596,15 +596,15 @@
             annotation.update_rect()
 
         # Update timelineScale display
         self.parent().timelineScale.update()
 
 
 class TimeLineWidget(QWidget):
-    CSV_HEADERS = ["Start time", "End Time", "Group name", "Timeline name"]
+    CSV_HEADERS = ["begin", "end", "label", "timeline"]
     valueChanged = Signal(int)
     durationChanged = Signal(int)
 
     def __init__(self, player=None):
         """Initializes the timeline widget"""
         super().__init__(player)
         self._duration = 0
@@ -1051,18 +1051,18 @@
             if self.name is None:
                 self.name = group.name
             self.setToolTip(self.name)
 
     def update_rect(self):
         # Calculate position to determine width
         self.startXPosition = (
-                self.startTime * self.timeline.scene.width() / self.timeline.duration
+            self.startTime * self.timeline.scene.width() / self.timeline.duration
         )
         self.endXPosition = (
-                self.endTime * self.timeline.scene.width() / self.timeline.duration
+            self.endTime * self.timeline.scene.width() / self.timeline.duration
         )
         self.setX(self.startXPosition)
 
         # Update the rectangle
         rect = self.rect()
         rect.setWidth(self.endXPosition - self.startXPosition)
         self.setRect(rect)
@@ -1142,15 +1142,19 @@
         super().focusOutEvent(event)
 
     def mouseMoveEvent(self, event):
         if event.buttons() == Qt.MouseButton.LeftButton:
             self.setY(self._height / 2)
 
             # A la souris on déplace le X, il faut changer le temps
-            time = int(event.scenePos().x() * self.annotation.timeline.duration / self.annotation.timeline.scene.width())
+            time = int(
+                event.scenePos().x()
+                * self.annotation.timeline.duration
+                / self.annotation.timeline.scene.width()
+            )
             self.annotation.timeline.player.set_position(time)
 
 
 class AnnotationStartHandle(AnnotationHandle):
 
     def __init__(self, annotation: Annotation):
         super().__init__(annotation, annotation.startTime, 0)
```

### Comparing `vicodepy-0.4.2/vicodepy/command.py` & `vicodepy-0.4.3/vicodepy/command.py`

 * *Files identical despite different names*

### Comparing `vicodepy-0.4.2/PKG-INFO` & `vicodepy-0.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vicodepy
-Version: 0.4.2
+Version: 0.4.3
 Summary: Video coder for psychological experiments
 License: GPL-3.0-or-later
 Author-email: Rafael Laboissière <rafael.laboissiere@cnrs.fr>,Esteban Milleret <esteban.milleret@etu.univ-grenoble-alpes.fr>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # ViCodePy – Video coder in Python for Experimental Psychology
@@ -28,15 +28,15 @@
 
 ### Playing/stopping the video and moving around it
 
 Once the video is loaded, it can be played and stopped using the space key. The left and right arrow keys can be used for going backward and forward, respectively, by one frame in the video. Positioning the cursor (a black triangle) with the mouse is also possible by clicking and dragging the cursor on the timeline.
 
 ### Annotations
 
-Annotations can be defined by pressing the enter key. This will mark one of the borders of the annotation. The other border can be defined by using the arrow keys or by clicking and dragging the cursor. Once the cursor is at the desired position, type enter again. This will open a dialog window for choosing the label and the color of the annotation. New labels can be defined in the dialog window and will be proposed later when new annotations are created.
+Annotations can be defined by pressing the enter key. This will mark one of the borders of the annotation. The other border can be defined by using the arrow keys or by clicking and dragging the cursor. Once the cursor is at the desired position, type enter again. This will open a dialog window for choosing the label and the color of the annotation. New labels can be defined in the dialog window by simply typing them. The new created labels will appear in the list of proposed labels when new annotations will be subsequently created.
 
 Once an annotation is created, it is possible to change its borders by double-clicking on the annotation. Two handles will appear, one at the left border of the annotation and the other at the right border. Click on a border handle and move it with the left and right arrow keys.
 
 The creation of an annotation can be aborted, once it is start by either typing the Escape key or by clicking on the Abort button in the pop-up window.
 
 The timeline can be zoomed in and out by using the scroll wheel of the mouse.
```

