# Comparing `tmp/mouse_jiggler_macos-0.4.0.tar.gz` & `tmp/mouse_jiggler_macos-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mouse_jiggler_macos-0.4.0.tar", last modified: Sat Jun  1 03:08:31 2024, max compression
+gzip compressed data, was "mouse_jiggler_macos-0.5.0.tar", last modified: Sun Jun  2 02:01:24 2024, max compression
```

## Comparing `mouse_jiggler_macos-0.4.0.tar` & `mouse_jiggler_macos-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-06-01 03:08:31.494114 mouse_jiggler_macos-0.4.0/
--rw-r--r--   0 umair      (501) staff       (20)     4260 2024-06-01 03:08:31.493724 mouse_jiggler_macos-0.4.0/PKG-INFO
--rw-r--r--   0 umair      (501) staff       (20)     3779 2024-05-31 00:29:28.000000 mouse_jiggler_macos-0.4.0/README.md
-drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-06-01 03:08:31.492564 mouse_jiggler_macos-0.4.0/mouse_jiggler/
--rw-r--r--   0 umair      (501) staff       (20)       44 2024-05-30 04:58:44.000000 mouse_jiggler_macos-0.4.0/mouse_jiggler/__init__.py
--rw-r--r--   0 umair      (501) staff       (20)     3449 2024-06-01 03:08:15.000000 mouse_jiggler_macos-0.4.0/mouse_jiggler/jiggler.py
-drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-06-01 03:08:31.493466 mouse_jiggler_macos-0.4.0/mouse_jiggler_macos.egg-info/
--rw-r--r--   0 umair      (501) staff       (20)     4260 2024-06-01 03:08:31.000000 mouse_jiggler_macos-0.4.0/mouse_jiggler_macos.egg-info/PKG-INFO
--rw-r--r--   0 umair      (501) staff       (20)      329 2024-06-01 03:08:31.000000 mouse_jiggler_macos-0.4.0/mouse_jiggler_macos.egg-info/SOURCES.txt
--rw-r--r--   0 umair      (501) staff       (20)        1 2024-06-01 03:08:31.000000 mouse_jiggler_macos-0.4.0/mouse_jiggler_macos.egg-info/dependency_links.txt
--rw-r--r--   0 umair      (501) staff       (20)       61 2024-06-01 03:08:31.000000 mouse_jiggler_macos-0.4.0/mouse_jiggler_macos.egg-info/entry_points.txt
--rw-r--r--   0 umair      (501) staff       (20)       22 2024-06-01 03:08:31.000000 mouse_jiggler_macos-0.4.0/mouse_jiggler_macos.egg-info/requires.txt
--rw-r--r--   0 umair      (501) staff       (20)       14 2024-06-01 03:08:31.000000 mouse_jiggler_macos-0.4.0/mouse_jiggler_macos.egg-info/top_level.txt
--rw-r--r--   0 umair      (501) staff       (20)       38 2024-06-01 03:08:31.494195 mouse_jiggler_macos-0.4.0/setup.cfg
--rw-r--r--   0 umair      (501) staff       (20)      863 2024-06-01 03:06:49.000000 mouse_jiggler_macos-0.4.0/setup.py
+drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-06-02 02:01:24.293821 mouse_jiggler_macos-0.5.0/
+-rw-r--r--   0 umair      (501) staff       (20)     4260 2024-06-02 02:01:24.293452 mouse_jiggler_macos-0.5.0/PKG-INFO
+-rw-r--r--   0 umair      (501) staff       (20)     3779 2024-05-31 00:29:28.000000 mouse_jiggler_macos-0.5.0/README.md
+drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-06-02 02:01:24.292019 mouse_jiggler_macos-0.5.0/mouse_jiggler/
+-rw-r--r--   0 umair      (501) staff       (20)       44 2024-05-30 04:58:44.000000 mouse_jiggler_macos-0.5.0/mouse_jiggler/__init__.py
+-rw-r--r--   0 umair      (501) staff       (20)     3877 2024-06-02 01:57:39.000000 mouse_jiggler_macos-0.5.0/mouse_jiggler/jiggler.py
+drwxr-xr-x   0 umair      (501) staff       (20)        0 2024-06-02 02:01:24.293194 mouse_jiggler_macos-0.5.0/mouse_jiggler_macos.egg-info/
+-rw-r--r--   0 umair      (501) staff       (20)     4260 2024-06-02 02:01:24.000000 mouse_jiggler_macos-0.5.0/mouse_jiggler_macos.egg-info/PKG-INFO
+-rw-r--r--   0 umair      (501) staff       (20)      329 2024-06-02 02:01:24.000000 mouse_jiggler_macos-0.5.0/mouse_jiggler_macos.egg-info/SOURCES.txt
+-rw-r--r--   0 umair      (501) staff       (20)        1 2024-06-02 02:01:24.000000 mouse_jiggler_macos-0.5.0/mouse_jiggler_macos.egg-info/dependency_links.txt
+-rw-r--r--   0 umair      (501) staff       (20)       61 2024-06-02 02:01:24.000000 mouse_jiggler_macos-0.5.0/mouse_jiggler_macos.egg-info/entry_points.txt
+-rw-r--r--   0 umair      (501) staff       (20)       22 2024-06-02 02:01:24.000000 mouse_jiggler_macos-0.5.0/mouse_jiggler_macos.egg-info/requires.txt
+-rw-r--r--   0 umair      (501) staff       (20)       14 2024-06-02 02:01:24.000000 mouse_jiggler_macos-0.5.0/mouse_jiggler_macos.egg-info/top_level.txt
+-rw-r--r--   0 umair      (501) staff       (20)       38 2024-06-02 02:01:24.293867 mouse_jiggler_macos-0.5.0/setup.cfg
+-rw-r--r--   0 umair      (501) staff       (20)      863 2024-06-02 02:00:14.000000 mouse_jiggler_macos-0.5.0/setup.py
```

### Comparing `mouse_jiggler_macos-0.4.0/PKG-INFO` & `mouse_jiggler_macos-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mouse_jiggler_macos
-Version: 0.4.0
+Version: 0.5.0
 Summary: A simple mouse jiggler for MacOS
 Home-page: https://github.com/UmairK5669/mouse-jiggler
 Author: Umair Khan
 Author-email: u7khan@uwaterloo.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mouse_jiggler_macos-0.4.0/README.md` & `mouse_jiggler_macos-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mouse_jiggler_macos-0.4.0/mouse_jiggler/jiggler.py` & `mouse_jiggler_macos-0.5.0/mouse_jiggler/jiggler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import threading
 import time
-from pynput import keyboard
+from pynput import keyboard, mouse
 import pyautogui
 import random
 import pync
 from pync import Notifier
 
 jiggler_running = False
+manual_movement_detected = False
 
 def executable():
 
-    def mouse_jiggler_function(movement_distance=10, interval=0.5):
-        global jiggler_running
+    def mouse_jiggler_function(movement_distance=12, interval=0.5):
+        global jiggler_running, manual_movement_detected
         screen_width, screen_height = pyautogui.size()
 
-        # Initial delay with periodic checks to allow immediate stopping
         for _ in range(7):
             if not jiggler_running:
                 return
             time.sleep(1)
 
         if not jiggler_running:
             return
@@ -40,15 +40,28 @@
         Notifier.notify('Jiggler Starting Now', title='Jiggler')
 
         time.sleep(1)
         
         pyautogui.moveTo(screen_width / 2, screen_height / 2)
         pyautogui.click()
 
+        last_mouse_pos = pyautogui.position()
+
         while jiggler_running:
+            current_mouse_pos = pyautogui.position()
+            if current_mouse_pos != last_mouse_pos:
+                manual_movement_detected = True
+                last_mouse_pos = current_mouse_pos
+                time.sleep(0.5)  
+                continue
+
+            if manual_movement_detected:
+                manual_movement_detected = False
+                time.sleep(1)  
+
             random_distance_x = random.randint(-movement_distance, movement_distance)
             random_distance_y = random.randint(-movement_distance, movement_distance)
 
             pyautogui.moveRel(random_distance_x, random_distance_y, duration=0.25)
             time.sleep(interval)
 
     def start_jiggler():
@@ -108,8 +121,8 @@
     on_press.shift_pressed = False
 
     # Set up the listener
     with keyboard.Listener(on_press=on_press, on_release=on_release) as listener:
         listener.join()
 
 if __name__ == "__main__":
-    executable()
+    executable()
```

### Comparing `mouse_jiggler_macos-0.4.0/mouse_jiggler_macos.egg-info/PKG-INFO` & `mouse_jiggler_macos-0.5.0/mouse_jiggler_macos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mouse_jiggler_macos
-Version: 0.4.0
+Version: 0.5.0
 Summary: A simple mouse jiggler for MacOS
 Home-page: https://github.com/UmairK5669/mouse-jiggler
 Author: Umair Khan
 Author-email: u7khan@uwaterloo.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mouse_jiggler_macos-0.4.0/setup.py` & `mouse_jiggler_macos-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mouse_jiggler_macos",
-    version="0.4.0",
+    version="0.5.0",
     author="Umair Khan",
     author_email="u7khan@uwaterloo.ca",
     description="A simple mouse jiggler for MacOS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UmairK5669/mouse-jiggler",
     packages=find_packages(),
```
