# Comparing `tmp/upicvision-0.1.0.2.tar.gz` & `tmp/upicvision-0.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upicvision-0.1.0.2.tar", last modified: Sun May 26 03:46:23 2024, max compression
+gzip compressed data, was "upicvision-0.1.0.3.tar", last modified: Sun Jun  2 14:41:59 2024, max compression
```

## Comparing `upicvision-0.1.0.2.tar` & `upicvision-0.1.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2024-05-26 03:46:00.942679 upicvision-0.1.0.2/README.md
--rw-r--r--   0        0        0      494 2024-05-26 03:46:23.910860 upicvision-0.1.0.2/pyproject.toml
--rw-r--r--   0        0        0      180 2024-05-26 03:46:00.942679 upicvision-0.1.0.2/src/upic/__init__.py
--rw-r--r--   0        0        0      574 2024-05-26 03:46:00.942679 upicvision-0.1.0.2/src/upic/modules/logger.py
--rw-r--r--   0        0        0    10629 2024-05-26 03:46:00.942679 upicvision-0.1.0.2/src/upic/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-26 03:46:00.942679 upicvision-0.1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2194 2024-05-26 03:46:00.942679 upicvision-0.1.0.2/tests/test_tag_detector.py
--rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 upicvision-0.1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-06-02 14:41:40.934600 upicvision-0.1.0.3/README.md
+-rw-r--r--   0        0        0      494 2024-06-02 14:41:59.702726 upicvision-0.1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      180 2024-06-02 14:41:40.934600 upicvision-0.1.0.3/src/upic/__init__.py
+-rw-r--r--   0        0        0      574 2024-06-02 14:41:40.934600 upicvision-0.1.0.3/src/upic/modules/logger.py
+-rw-r--r--   0        0        0    10596 2024-06-02 14:41:40.934600 upicvision-0.1.0.3/src/upic/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:41:40.934600 upicvision-0.1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     2194 2024-06-02 14:41:40.934600 upicvision-0.1.0.3/tests/test_tag_detector.py
+-rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 upicvision-0.1.0.3/PKG-INFO
```

### Comparing `upicvision-0.1.0.2/src/upic/modules/logger.py` & `upicvision-0.1.0.3/src/upic/modules/logger.py`

 * *Files identical despite different names*

### Comparing `upicvision-0.1.0.2/src/upic/vision/tagdetector.py` & `upicvision-0.1.0.3/src/upic/vision/tagdetector.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,16 +64,15 @@
 
         Returns:
 
         """
         if self._camera is not None:
             self.release_camera()
         self._camera = cv2.VideoCapture(device_id)
-        read_status, _ = self._camera.read()
-        if read_status:
+        if self._camera.isOpened():
             self._update_cam_center()
             _logger.info(
                 f"CAMERA RESOLUTION：{self._camera.get(cv2.CAP_PROP_FRAME_WIDTH)}x{self._camera.get(cv2.CAP_PROP_FRAME_HEIGHT)}\n"
                 f"CAMERA FPS: [{self._camera.get(cv2.CAP_PROP_FPS)}]\n"
                 f"CAM CENTER: [{self._frame_center}]"
             )
         else:
```

### Comparing `upicvision-0.1.0.2/tests/test_tag_detector.py` & `upicvision-0.1.0.3/tests/test_tag_detector.py`

 * *Files identical despite different names*

