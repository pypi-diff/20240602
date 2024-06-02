# Comparing `tmp/sanghyunjo-1.4.4.tar.gz` & `tmp/sanghyunjo-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sanghyunjo-1.4.4.tar", last modified: Wed May 29 06:42:34 2024, max compression
+gzip compressed data, was "dist\sanghyunjo-1.4.7.tar", last modified: Sun Jun  2 00:12:49 2024, max compression
```

## Comparing `sanghyunjo-1.4.4.tar` & `sanghyunjo-1.4.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 06:42:34.989418 sanghyunjo-1.4.4/
--rw-rw-rw-   0        0        0     1087 2024-05-16 07:32:54.000000 sanghyunjo-1.4.4/LICENSE
--rw-rw-rw-   0        0        0       53 2024-05-16 07:24:52.000000 sanghyunjo-1.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0      365 2024-05-29 06:42:34.989418 sanghyunjo-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-05-28 15:18:59.000000 sanghyunjo-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 06:42:34.965647 sanghyunjo-1.4.4/sanghyunjo/
--rw-rw-rw-   0        0        0      194 2024-05-29 06:42:14.000000 sanghyunjo-1.4.4/sanghyunjo/__init__.py
--rw-rw-rw-   0        0        0     9460 2024-05-29 06:42:09.000000 sanghyunjo-1.4.4/sanghyunjo/cv_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 06:42:34.987422 sanghyunjo-1.4.4/sanghyunjo/fonts/
--rw-rw-rw-   0        0        0    34888 2023-07-19 08:59:35.000000 sanghyunjo-1.4.4/sanghyunjo/fonts/Times New Roman MT Std.otf
--rw-rw-rw-   0        0        0      358 2024-05-20 07:08:56.000000 sanghyunjo-1.4.4/sanghyunjo/json_utils.py
--rw-rw-rw-   0        0        0     3115 2024-05-26 14:14:30.000000 sanghyunjo-1.4.4/sanghyunjo/misc.py
-drwxrwxrwx   0        0        0        0 2024-05-29 06:42:34.988421 sanghyunjo-1.4.4/sanghyunjo.egg-info/
--rw-rw-rw-   0        0        0      365 2024-05-29 06:42:34.000000 sanghyunjo-1.4.4/sanghyunjo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2024-05-29 06:42:34.000000 sanghyunjo-1.4.4/sanghyunjo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 06:42:34.000000 sanghyunjo-1.4.4/sanghyunjo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-16 07:28:15.000000 sanghyunjo-1.4.4/sanghyunjo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-29 06:42:34.000000 sanghyunjo-1.4.4/sanghyunjo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 06:42:34.990415 sanghyunjo-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-05-20 07:09:32.000000 sanghyunjo-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 00:12:49.040593 sanghyunjo-1.4.7/
+-rw-rw-rw-   0        0        0     1087 2024-05-16 07:32:54.000000 sanghyunjo-1.4.7/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-05-16 07:24:52.000000 sanghyunjo-1.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      365 2024-06-02 00:12:49.039591 sanghyunjo-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-05-28 15:18:59.000000 sanghyunjo-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 00:12:49.020708 sanghyunjo-1.4.7/sanghyunjo/
+-rw-rw-rw-   0        0        0      194 2024-06-02 00:12:41.000000 sanghyunjo-1.4.7/sanghyunjo/__init__.py
+-rw-rw-rw-   0        0        0    10168 2024-06-02 00:12:39.000000 sanghyunjo-1.4.7/sanghyunjo/cv_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-02 00:12:49.029683 sanghyunjo-1.4.7/sanghyunjo/fonts/
+-rw-rw-rw-   0        0        0    34888 2023-07-19 08:59:35.000000 sanghyunjo-1.4.7/sanghyunjo/fonts/Times New Roman MT Std.otf
+-rw-rw-rw-   0        0        0      358 2024-05-20 07:08:56.000000 sanghyunjo-1.4.7/sanghyunjo/json_utils.py
+-rw-rw-rw-   0        0        0     3115 2024-05-26 14:14:30.000000 sanghyunjo-1.4.7/sanghyunjo/misc.py
+drwxrwxrwx   0        0        0        0 2024-06-02 00:12:49.031678 sanghyunjo-1.4.7/sanghyunjo.egg-info/
+-rw-rw-rw-   0        0        0      365 2024-06-02 00:12:48.000000 sanghyunjo-1.4.7/sanghyunjo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2024-06-02 00:12:48.000000 sanghyunjo-1.4.7/sanghyunjo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 00:12:48.000000 sanghyunjo-1.4.7/sanghyunjo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-16 07:28:15.000000 sanghyunjo-1.4.7/sanghyunjo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-06-02 00:12:48.000000 sanghyunjo-1.4.7/sanghyunjo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 00:12:49.040593 sanghyunjo-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-05-20 07:09:32.000000 sanghyunjo-1.4.7/setup.py
```

### Comparing `sanghyunjo-1.4.4/LICENSE` & `sanghyunjo-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.4.4/README.md` & `sanghyunjo-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.4.4/sanghyunjo/cv_utils.py` & `sanghyunjo-1.4.7/sanghyunjo/cv_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         }
     }
 
     try: 
         if mode == 'opencv':
             image = cv2.imdecode(np.fromfile(path, np.uint8), color_dict[mode][color])
         else:
-            image = Image.open(path).convert(color_dic[mode][color])
+            image = Image.open(path).convert(color_dict[mode][color])
     except FileNotFoundError: 
         image = None
     
     return image
 
 def write_image(path, image, palette=None):
     if palette is None: cv2.imwrite(path, image)
@@ -219,14 +219,17 @@
         heatmap = colorize(heatmap, option)
         if tag is not None: draw_text(heatmap, tag, (0, 0), font_size=40)
         vis_heatmaps.append(heatmap)
 
     return np.concatenate(vis_heatmaps, axis=1)
 
 def resize(image, size=None, scale=None, mode='bicubic'):
+    if not isinstance(size, tuple):
+        size = get_size(size)
+    
     inp_dict = {
         'bicubic': cv2.INTER_CUBIC,
         'nearest': cv2.INTER_NEAREST,
     }
     if scale is not None:
         h, w = image.shape[:2]
         size = (int(w * scale), int(h * scale))
@@ -297,12 +300,33 @@
 
 def vstack(*images):
     return np.concatenate(images, axis=0)
 
 def hstack(*images):
     return np.concatenate(images, axis=1)
 
-def gray2bgr(image):
-    return cv2.cvtColor(image, cv2.COLOR_GRAY2BGR)
+def convert(image, code='gray2bgr'):
+    if code == 'gray2bgr':
+        code = cv2.COLOR_GRAY2BGR
+    elif code == 'bgr2gray':
+        code = cv2.COLOR_BGR2GRAY
+    elif code == 'bgr2rgb':
+        code = cv2.COLOR_BGR2RGB
+    elif code == 'rgb2bgr':
+        code = cv2.COLOR_RGB2BGR
+    return cv2.cvtColor(image, code)
+
+def cv2pil(image: np.ndarray) -> Image:
+    return Image.fromarray(convert(image, 'bgr2rgb'))
+
+def pil2cv(image: Image) -> np.ndarray:
+    return convert(np.asarray(image), 'rgb2bgr')
 
 def overlay(image1, image2, alpha):
-    return cv2.addWeighted(image1, alpha, image2, 1. - alpha, 0.0)
+    return cv2.addWeighted(image1, alpha, image2, 1. - alpha, 0.0)
+
+def get_size(image) -> tuple:
+    if isinstance(image, np.ndarray): # cv
+        size = tuple(image.shape[:2][::-1])
+    else: # pillow
+        size = image.size
+    return size
```

### Comparing `sanghyunjo-1.4.4/sanghyunjo/fonts/Times New Roman MT Std.otf` & `sanghyunjo-1.4.7/sanghyunjo/fonts/Times New Roman MT Std.otf`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.4.4/sanghyunjo/misc.py` & `sanghyunjo-1.4.7/sanghyunjo/misc.py`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.4.4/setup.py` & `sanghyunjo-1.4.7/setup.py`

 * *Files identical despite different names*

