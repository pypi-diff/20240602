# Comparing `tmp/danila-lib-1.8.4.tar.gz` & `tmp/danila-lib-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.8.4.tar", last modified: Thu May 30 06:42:37 2024, max compression
+gzip compressed data, was "danila-lib-1.8.5.tar", last modified: Sun Jun  2 10:18:27 2024, max compression
```

## Comparing `danila-lib-1.8.4.tar` & `danila-lib-1.8.5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.439840 danila-lib-1.8.4/
--rw-rw-rw-   0        0        0     9615 2024-05-30 06:42:37.439840 danila-lib-1.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.320376 danila-lib-1.8.4/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.4/danila/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.8.4/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.4/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.4/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.4/danila/danila_v3.py
--rw-rw-rw-   0        0        0    24356 2024-05-28 10:23:30.000000 danila-lib-1.8.4/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.338295 danila-lib-1.8.4/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-30 06:42:37.000000 danila-lib-1.8.4/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2024-05-30 06:42:37.000000 danila-lib-1.8.4/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 06:42:37.000000 danila-lib-1.8.4/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-30 06:42:37.000000 danila-lib-1.8.4/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-30 06:42:37.000000 danila-lib-1.8.4/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.338295 danila-lib-1.8.4/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.4/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.386081 danila-lib-1.8.4/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.4/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.4/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.4/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.4/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.4/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.4/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.8.4/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      880 2024-05-30 06:42:19.000000 danila-lib-1.8.4/data/neuro/models.py
--rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.4/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.8.4/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:42:37.438845 danila-lib-1.8.4/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.4/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.4/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.4/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.4/data/result/Label_area.py
--rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.4/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.4/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.4/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.4/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.4/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.4/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.4/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-30 06:42:37.444818 danila-lib-1.8.4/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-30 06:42:26.000000 danila-lib-1.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:18:27.626114 danila-lib-1.8.5/
+-rw-rw-rw-   0        0        0     9615 2024-06-02 10:18:27.626114 danila-lib-1.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.8.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 10:18:27.099475 danila-lib-1.8.5/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.8.5/danila/__init__.py
+-rw-rw-rw-   0        0        0     2358 2024-06-02 09:51:55.000000 danila-lib-1.8.5/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.8.5/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.8.5/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.8.5/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    25555 2024-06-02 10:17:58.000000 danila-lib-1.8.5/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:18:27.171152 danila-lib-1.8.5/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-06-02 10:18:26.000000 danila-lib-1.8.5/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2024-06-02 10:18:26.000000 danila-lib-1.8.5/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 10:18:26.000000 danila-lib-1.8.5/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-06-02 10:18:26.000000 danila-lib-1.8.5/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-02 10:18:26.000000 danila-lib-1.8.5/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 10:18:27.172148 danila-lib-1.8.5/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.8.5/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:18:27.266724 danila-lib-1.8.5/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.8.5/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.8.5/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.8.5/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     3000 2024-05-28 08:28:46.000000 danila-lib-1.8.5/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3153 2024-05-23 05:46:54.000000 danila-lib-1.8.5/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0     2657 2024-06-02 10:17:58.000000 danila-lib-1.8.5/data/neuro/Vagon_number_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.5/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6695 2024-05-28 13:59:46.000000 danila-lib-1.8.5/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      959 2024-06-02 10:17:58.000000 danila-lib-1.8.5/data/neuro/models.py
+-rw-rw-rw-   0        0        0     3222 2024-05-27 08:43:50.000000 danila-lib-1.8.5/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4854 2024-05-28 13:59:46.000000 danila-lib-1.8.5/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:18:27.623126 danila-lib-1.8.5/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.8.5/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.8.5/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.8.5/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      332 2024-05-27 09:58:57.000000 danila-lib-1.8.5/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      236 2024-05-27 08:43:50.000000 danila-lib-1.8.5/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.8.5/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.8.5/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.8.5/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.8.5/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.8.5/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.8.5/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 10:18:27.639055 danila-lib-1.8.5/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-06-02 10:18:21.000000 danila-lib-1.8.5/setup.py
```

### Comparing `danila-lib-1.8.4/PKG-INFO` & `danila-lib-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.4
+Version: 1.8.5
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.8.4/README.md` & `danila-lib-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/danila/danila.py` & `danila-lib-1.8.5/danila/danila.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,19 +37,24 @@
     # returns openCV image with cut_rama
     def rama_cut(self, img, size = 256):
         """rama_cut(img : openCV img) -> openCV image of rama rectangle"""
         return self.danila.rama_cut(img, size)
 
     #
     # returns openCV cut rama with drawn text areas
-    def text_detect_cut(self, img, size = 256):
+    def rama_text_detect_cut(self, img, size = 256):
         """returns openCV cut rama with drawn text areas"""
         return self.danila.text_detect_cut(img, size)
 
     # returns openCV img with drawn text areas
-    def text_detect(self, img, size = 256):
+    def rama_text_detect(self, img, size = 256):
         """returns openCV img with drawn text areas"""
         return self.danila.text_detect(img, size)
     # returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'
-    def text_recognize(self, img, size = 256):
+    def rama_text_recognize(self, img, size = 256):
         """returns dict {'number', 'prod', 'year'} for openCV rama img or 'no_rama'"""
         return self.danila.text_recognize(img, size)
+
+    # returns openCV img with drawn number areas
+    def vagon_number_detect(self, img, size = 256):
+        """returns openCV img with drawn number areas"""
+        return self.danila.vagon_number_detect(img, size)
```

### Comparing `danila-lib-1.8.4/danila/danila_v1.py` & `danila-lib-1.8.5/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/danila/danila_v2.py` & `danila-lib-1.8.5/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/danila/danila_v3.py` & `danila-lib-1.8.5/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/danila/danila_v4.py` & `danila-lib-1.8.5/danila/danila_v4.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import cv2
 
 from data.neuro.Letters_recognize import Letters_recognize
 from data.neuro.Rama_detect_class import Rama_detect_class
 from data.neuro.Rama_prod_classify_class import Rama_prod_classify_class
 from data.neuro.Text_detect_class import Text_detect_class
+from data.neuro.Vagon_number_detect_class import Vagon_number_detect_class
 from data.neuro.models import *
 from data.result.Class_im import Class_im
 from data.result.Class_text import Class_text
 from data.result.Rama_prod import Rama_Prod
 from data.result.Rect import Rect
 
 """main module for user"""
@@ -56,14 +57,18 @@
                                                                             'rama_text_begickaya_detect', yolo_path)
         text_recognize_yolo_ruzhimmash_model_path = TEXT_RECOGNIZE_RUZHIMMASH_MODEL_ADDRESS
         print('reading and loading - TEXT_RECOGNIZE_RUZHIMMASH_MODEL')
         self.text_recognize_ruzhimmash_model = Text_Recognize_yolo(text_recognize_yolo_ruzhimmash_model_path, yolo_path)
         text_recognize_yolo_begickaya_model_path = TEXT_RECOGNIZE_BEGICKAYA_MODEL_ADDRESS
         print('reading and loading - TEXT_RECOGNIZE_BEGICKAYA_MODEL')
         self.text_recognize_begickaya_model = Text_Recognize_yolo(text_recognize_yolo_begickaya_model_path, yolo_path)
+        vagon_number_detect_model_path = VAGON_NUMBER_DETECT_MODEL_ADDRESS
+        print('reading and loading - VAGON_NUMBER_DETECT_MODEL')
+        self.vagon_number_detect_model = Vagon_number_detect_class(vagon_number_detect_model_path, yolo_path)
+
 
     # returns Rama_Prod_Conf - class of rama and confidence using CNN network
     # img - openCV frame
     def rama_classify(self, img, size = 256):
         """rama_classify(Img : openCv frame): String - returns class of rama using CNN network"""
         """rama_classify uses Rama_classify_class method - classify(Img)"""
         # img = cv2.imread(img_path)
@@ -422,7 +427,23 @@
             res_labels_number_text, res_labels_number_conf = res_labels['number']
             detail.number = Text_cut_recognize_result(res_labels_number_text, res_labels_number_conf)
             res_labels_year_text, res_labels_year_conf = res_labels['year']
             detail.year = Text_cut_recognize_result(res_labels_year_text, res_labels_year_conf)
             res_labels_prod_text, res_labels_prod_conf = res_labels['prod']
             detail.prod = Text_cut_recognize_result(res_labels_prod_text, res_labels_prod_conf)
             return detail
+
+
+    def vagon_number_detect(self, img, size = 256):
+        hash_object = hashlib.md5(bytes(str(datetime.now()), 'utf-8'))
+        hash_str = hash_object.hexdigest()
+        initial_image_path = 'initial_image' + hash_str + '.jpg'
+        cv2.imwrite(initial_image_path, img)
+        number_rects = self.vagon_number_detect_model.vagon_rama_detect(initial_image_path, size)
+        if len(number_rects) == 0:
+            os.remove(initial_image_path)
+            return img
+        img_with_number = img.copy
+        for number_rect in number_rects:
+            cv2.rectangle(img_with_number, (number_rect.xmin, number_rect.ymin), (number_rect.xmax, number_rect.ymax), (0, 0, 255), 2)
+            cv2.putText(img_with_number, 'number', (number_rect.xmin, number_rect.ymin), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (0, 0, 255), 2)
+        return img_with_number
```

### Comparing `danila-lib-1.8.4/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.8.5/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.8.4
+Version: 1.8.5
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.8.4/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.8.5/danila_lib.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 danila_lib.egg-info/top_level.txt
 data/__init__.py
 data/neuro/Letters_recognize.py
 data/neuro/Rama_classify_class.py
 data/neuro/Rama_detect_class.py
 data/neuro/Rama_prod_classify_class.py
 data/neuro/Text_detect_class.py
+data/neuro/Vagon_number_detect_class.py
 data/neuro/__init__.py
 data/neuro/letters_in_image.py
 data/neuro/models.py
 data/neuro/objs_in_image.py
 data/neuro/text_recognize_yolo.py
 data/result/Class_im.py
 data/result/Class_text.py
```

### Comparing `danila-lib-1.8.4/danila_lib.egg-info/requires.txt` & `danila-lib-1.8.5/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/neuro/Letters_recognize.py` & `danila-lib-1.8.5/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/neuro/Rama_classify_class.py` & `danila-lib-1.8.5/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/neuro/Rama_detect_class.py` & `danila-lib-1.8.5/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.8.5/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/neuro/Text_detect_class.py` & `danila-lib-1.8.5/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/neuro/letters_in_image.py` & `danila-lib-1.8.5/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/neuro/models.py` & `danila-lib-1.8.5/data/neuro/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,8 +4,9 @@
 RAMA_RUZHIMMASH_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/rgthm-mMrbhOmw'
 RAMA_BEJICKAYA_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/QhicLdm2-PT6oA'
 # TEXT_RECOGNIZE_RUZHIMMASH_MODEL_ADDRESS = 'https://disk.yandex.ru/d/C2hDMsbTZMnL8Q' -7500_b7500_r
 # TEXT_RECOGNIZE_BEGICKAYA_MODEL_ADDRESS = 'https://disk.yandex.ru/d/C2hDMsbTZMnL8Q'
 TEXT_RECOGNIZE_RUZHIMMASH_MODEL_ADDRESS = 'https://disk.yandex.ru/d/GcI-mAtwpb2I-g' # 11000_b_11000_r
 TEXT_RECOGNIZE_BEGICKAYA_MODEL_ADDRESS = 'https://disk.yandex.ru/d/GcI-mAtwpb2I-g'  # 11000_b_11000_r
 
-RAMA_PROD_CLASSIFY_MODEL_ADDRESS = 'https://disk.yandex.ru/d/8FI8TaTwaCfbSA'
+RAMA_PROD_CLASSIFY_MODEL_ADDRESS = 'https://disk.yandex.ru/d/8FI8TaTwaCfbSA'
+VAGON_NUMBER_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/ZGS0sdk1syJmcQ'
```

### Comparing `danila-lib-1.8.4/data/neuro/objs_in_image.py` & `danila-lib-1.8.5/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/neuro/text_recognize_yolo.py` & `danila-lib-1.8.5/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/result/Image_text_areas.py` & `danila-lib-1.8.5/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/result/Rect.py` & `danila-lib-1.8.5/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/result/Text_area.py` & `danila-lib-1.8.5/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/data/result/Yolo_label_rect.py` & `danila-lib-1.8.5/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.8.4/setup.py` & `danila-lib-1.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.8.4',
+  version='1.8.5',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

