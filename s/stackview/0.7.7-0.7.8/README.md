# Comparing `tmp/stackview-0.7.7.tar.gz` & `tmp/stackview-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackview-0.7.7.tar", last modified: Fri May 24 13:48:41 2024, max compression
+gzip compressed data, was "stackview-0.7.8.tar", last modified: Sun Jun  2 10:54:31 2024, max compression
```

## Comparing `stackview-0.7.7.tar` & `stackview-0.7.8.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 13:48:41.577460 stackview-0.7.7/
--rw-rw-rw-   0        0        0     1549 2022-11-28 22:36:36.000000 stackview-0.7.7/LICENSE
--rw-rw-rw-   0        0        0    12050 2024-05-24 13:48:41.577460 stackview-0.7.7/PKG-INFO
--rw-rw-rw-   0        0        0    11252 2024-03-30 17:31:52.000000 stackview-0.7.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 13:48:41.577460 stackview-0.7.7/setup.cfg
--rw-rw-rw-   0        0        0     1114 2024-05-24 13:45:46.000000 stackview-0.7.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:48:41.561833 stackview-0.7.7/stackview/
--rw-rw-rw-   0        0        0      613 2024-05-24 13:45:46.000000 stackview-0.7.7/stackview/__init__.py
--rw-rw-rw-   0        0        0     7993 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_annotate.py
--rw-rw-rw-   0        0        0     5101 2023-03-26 19:33:45.000000 stackview-0.7.7/stackview/_assist.py
--rw-rw-rw-   0        0        0     1429 2024-03-23 12:49:32.000000 stackview-0.7.7/stackview/_bia_bob_plugins.py
--rw-rw-rw-   0        0        0     5467 2023-04-15 09:27:34.000000 stackview-0.7.7/stackview/_colormaps.py
--rw-rw-rw-   0        0        0     2060 2023-01-01 15:16:44.000000 stackview-0.7.7/stackview/_context.py
--rw-rw-rw-   0        0        0     5584 2024-05-24 13:35:04.000000 stackview-0.7.7/stackview/_crop.py
--rw-rw-rw-   0        0        0     5184 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_curtain.py
--rw-rw-rw-   0        0        0     4115 2023-11-17 12:56:59.000000 stackview-0.7.7/stackview/_image_widget.py
--rw-rw-rw-   0        0        0     4457 2024-05-24 13:45:55.000000 stackview-0.7.7/stackview/_imshow.py
--rw-rw-rw-   0        0        0     7964 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_interact.py
--rw-rw-rw-   0        0        0     2367 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_orthogonal.py
--rw-rw-rw-   0        0        0     3516 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_picker.py
--rw-rw-rw-   0        0        0     5252 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_side_by_side.py
--rw-rw-rw-   0        0        0     2280 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_slice.py
--rw-rw-rw-   0        0        0     2823 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_slice_viewer.py
--rw-rw-rw-   0        0        0     8753 2023-10-19 19:42:08.000000 stackview-0.7.7/stackview/_static_view.py
--rw-rw-rw-   0        0        0     6551 2024-03-30 17:27:56.000000 stackview-0.7.7/stackview/_switch.py
--rw-rw-rw-   0        0        0     1066 2022-12-30 17:39:31.000000 stackview-0.7.7/stackview/_uint_field.py
--rw-rw-rw-   0        0        0     2567 2023-01-01 15:16:44.000000 stackview-0.7.7/stackview/_utilities.py
-drwxrwxrwx   0        0        0        0 2024-05-24 13:48:41.577460 stackview-0.7.7/stackview.egg-info/
--rw-rw-rw-   0        0        0    12050 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      696 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 10:54:31.599009 stackview-0.7.8/
+-rw-rw-rw-   0        0        0     1549 2022-11-28 22:36:36.000000 stackview-0.7.8/LICENSE
+-rw-rw-rw-   0        0        0    12658 2024-06-02 10:54:31.598006 stackview-0.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11824 2024-06-02 10:52:28.000000 stackview-0.7.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 10:54:31.599009 stackview-0.7.8/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2024-06-02 10:54:12.000000 stackview-0.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:54:31.566637 stackview-0.7.8/stackview/
+-rw-rw-rw-   0        0        0      661 2024-06-02 10:52:28.000000 stackview-0.7.8/stackview/__init__.py
+-rw-rw-rw-   0        0        0     5616 2024-06-02 10:52:28.000000 stackview-0.7.8/stackview/_animate.py
+-rw-rw-rw-   0        0        0     7993 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_annotate.py
+-rw-rw-rw-   0        0        0     5101 2023-03-26 19:33:45.000000 stackview-0.7.8/stackview/_assist.py
+-rw-rw-rw-   0        0        0     1429 2024-03-23 12:49:32.000000 stackview-0.7.8/stackview/_bia_bob_plugins.py
+-rw-rw-rw-   0        0        0     5467 2023-04-15 09:27:34.000000 stackview-0.7.8/stackview/_colormaps.py
+-rw-rw-rw-   0        0        0     2060 2023-01-01 15:16:44.000000 stackview-0.7.8/stackview/_context.py
+-rw-rw-rw-   0        0        0     5584 2024-05-24 13:35:04.000000 stackview-0.7.8/stackview/_crop.py
+-rw-rw-rw-   0        0        0     5184 2024-06-02 10:49:36.000000 stackview-0.7.8/stackview/_curtain.py
+-rw-rw-rw-   0        0        0     4115 2023-11-17 12:56:59.000000 stackview-0.7.8/stackview/_image_widget.py
+-rw-rw-rw-   0        0        0     4457 2024-05-24 13:45:55.000000 stackview-0.7.8/stackview/_imshow.py
+-rw-rw-rw-   0        0        0     7964 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_interact.py
+-rw-rw-rw-   0        0        0     2367 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_orthogonal.py
+-rw-rw-rw-   0        0        0     3516 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_picker.py
+-rw-rw-rw-   0        0        0     5252 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_side_by_side.py
+-rw-rw-rw-   0        0        0     2280 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_slice.py
+-rw-rw-rw-   0        0        0     2823 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_slice_viewer.py
+-rw-rw-rw-   0        0        0     8753 2023-10-19 19:42:08.000000 stackview-0.7.8/stackview/_static_view.py
+-rw-rw-rw-   0        0        0     6551 2024-03-30 17:27:56.000000 stackview-0.7.8/stackview/_switch.py
+-rw-rw-rw-   0        0        0     1066 2022-12-30 17:39:31.000000 stackview-0.7.8/stackview/_uint_field.py
+-rw-rw-rw-   0        0        0     2567 2023-01-01 15:16:44.000000 stackview-0.7.8/stackview/_utilities.py
+drwxrwxrwx   0        0        0        0 2024-06-02 10:54:31.597005 stackview-0.7.8/stackview.egg-info/
+-rw-rw-rw-   0        0        0    12658 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       93 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/top_level.txt
```

### Comparing `stackview-0.7.7/LICENSE` & `stackview-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/PKG-INFO` & `stackview-0.7.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.7.7
+Version: 0.7.8
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@uni-leipzig.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
 Requires-Dist: ipycanvas
 Requires-Dist: ipywidgets
 Requires-Dist: scikit-image
 Requires-Dist: ipyevents
 Requires-Dist: toolz
 Requires-Dist: matplotlib
 Requires-Dist: ipykernel
+Requires-Dist: imageio
 
 # stackview ðŸ§ŠðŸ‘€
 Interactive image stack viewing in jupyter notebooks based on 
 [ipycanvas](https://ipycanvas.readthedocs.io/) and 
 [ipywidgets](https://ipywidgets.readthedocs.io/en/latest/). 
 TL;DR:
 ```python
@@ -113,14 +114,31 @@
 
 stackview.imshow(image, plot=axs[2], continue_drawing=True)
 stackview.imshow(labels, plot=axs[2], alpha=0.4, title='image + labels')
 ```
 
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/imshow.png)
 
+
+### Static animations
+
+The `animate` and `animate_curtain` functions can be used to store animations of image stacks / images blended over each other as gif to disk.
+
+Â´Â´Â´
+stackview.animate(blobs_images, filename="images/timelapse2.gif", frame_delay_ms=50)
+Â´Â´Â´
+
+![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse2.gif)
+
+```python
+stackview.animate_curtain(blobs, blobs > 128, filename="images/timelapse3.gif")
+```
+
+![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse3.gif)
+
 ### Annotate regions
 
 To create label images interactively, e.g. for machine learning training, the `stackview.annotate` function offers basic label drawing tools. 
 Click and drag for drawing. Hold the `ALT` key for erasing.
 Annotations are drawn into a `labels` image you need to create before drawing.
 
 ```python
```

### Comparing `stackview-0.7.7/README.md` & `stackview-0.7.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,31 @@
 
 stackview.imshow(image, plot=axs[2], continue_drawing=True)
 stackview.imshow(labels, plot=axs[2], alpha=0.4, title='image + labels')
 ```
 
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/imshow.png)
 
+
+### Static animations
+
+The `animate` and `animate_curtain` functions can be used to store animations of image stacks / images blended over each other as gif to disk.
+
+´´´
+stackview.animate(blobs_images, filename="images/timelapse2.gif", frame_delay_ms=50)
+´´´
+
+![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse2.gif)
+
+```python
+stackview.animate_curtain(blobs, blobs > 128, filename="images/timelapse3.gif")
+```
+
+![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse3.gif)
+
 ### Annotate regions
 
 To create label images interactively, e.g. for machine learning training, the `stackview.annotate` function offers basic label drawing tools. 
 Click and drag for drawing. Hold the `ALT` key for erasing.
 Annotations are drawn into a `labels` image you need to create before drawing.
 
 ```python
```

### Comparing `stackview-0.7.7/setup.py` & `stackview-0.7.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stackview",
-    version="0.7.7",
+    version="0.7.8",
     author="Robert Haase",
     author_email="robert.haase@uni-leipzig.de",
     description="Interactive image stack viewing in jupyter notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/haesleinhuepf/stackview/",
     packages=setuptools.find_packages(),
     include_package_data=True,
-    install_requires=["numpy!=1.19.4", "ipycanvas", "ipywidgets", "scikit-image", "ipyevents", "toolz", "matplotlib", "ipykernel"],
+    install_requires=["numpy!=1.19.4", "ipycanvas", "ipywidgets", "scikit-image", "ipyevents", "toolz", "matplotlib", "ipykernel", "imageio"],
     python_requires='>=3.6',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Development Status :: 3 - Alpha",
```

### Comparing `stackview-0.7.7/stackview/__init__.py` & `stackview-0.7.8/stackview/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.7"
+__version__ = "0.7.8"
 
 from ._static_view import jupyter_displayable_output, insight
 from ._utilities import merge_rgb
 from ._context import nop
 from ._crop import crop
 from ._slice_viewer import _SliceViewer
 from ._annotate import annotate
@@ -13,8 +13,9 @@
 from ._orthogonal import orthogonal
 from ._side_by_side import side_by_side
 from ._picker import picker
 from ._assist import assist
 from ._switch import switch
 from ._colormaps import create_colormap
 from ._imshow import imshow
+from ._animate import animate, animate_curtain
```

### Comparing `stackview-0.7.7/stackview/_annotate.py` & `stackview-0.7.8/stackview/_annotate.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_assist.py` & `stackview-0.7.8/stackview/_assist.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_bia_bob_plugins.py` & `stackview-0.7.8/stackview/_bia_bob_plugins.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_colormaps.py` & `stackview-0.7.8/stackview/_colormaps.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_context.py` & `stackview-0.7.8/stackview/_context.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_crop.py` & `stackview-0.7.8/stackview/_crop.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_curtain.py` & `stackview-0.7.8/stackview/_curtain.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_image_widget.py` & `stackview-0.7.8/stackview/_image_widget.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_imshow.py` & `stackview-0.7.8/stackview/_imshow.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_interact.py` & `stackview-0.7.8/stackview/_interact.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_orthogonal.py` & `stackview-0.7.8/stackview/_orthogonal.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_picker.py` & `stackview-0.7.8/stackview/_picker.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_side_by_side.py` & `stackview-0.7.8/stackview/_side_by_side.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_slice.py` & `stackview-0.7.8/stackview/_slice.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_slice_viewer.py` & `stackview-0.7.8/stackview/_slice_viewer.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_static_view.py` & `stackview-0.7.8/stackview/_static_view.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_switch.py` & `stackview-0.7.8/stackview/_switch.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_uint_field.py` & `stackview-0.7.8/stackview/_uint_field.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview/_utilities.py` & `stackview-0.7.8/stackview/_utilities.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.7/stackview.egg-info/PKG-INFO` & `stackview-0.7.8/stackview.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.7.7
+Version: 0.7.8
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@uni-leipzig.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -17,14 +17,15 @@
 Requires-Dist: ipycanvas
 Requires-Dist: ipywidgets
 Requires-Dist: scikit-image
 Requires-Dist: ipyevents
 Requires-Dist: toolz
 Requires-Dist: matplotlib
 Requires-Dist: ipykernel
+Requires-Dist: imageio
 
 # stackview ðŸ§ŠðŸ‘€
 Interactive image stack viewing in jupyter notebooks based on 
 [ipycanvas](https://ipycanvas.readthedocs.io/) and 
 [ipywidgets](https://ipywidgets.readthedocs.io/en/latest/). 
 TL;DR:
 ```python
@@ -113,14 +114,31 @@
 
 stackview.imshow(image, plot=axs[2], continue_drawing=True)
 stackview.imshow(labels, plot=axs[2], alpha=0.4, title='image + labels')
 ```
 
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/imshow.png)
 
+
+### Static animations
+
+The `animate` and `animate_curtain` functions can be used to store animations of image stacks / images blended over each other as gif to disk.
+
+Â´Â´Â´
+stackview.animate(blobs_images, filename="images/timelapse2.gif", frame_delay_ms=50)
+Â´Â´Â´
+
+![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse2.gif)
+
+```python
+stackview.animate_curtain(blobs, blobs > 128, filename="images/timelapse3.gif")
+```
+
+![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse3.gif)
+
 ### Annotate regions
 
 To create label images interactively, e.g. for machine learning training, the `stackview.annotate` function offers basic label drawing tools. 
 Click and drag for drawing. Hold the `ALT` key for erasing.
 Annotations are drawn into a `labels` image you need to create before drawing.
 
 ```python
```

### Comparing `stackview-0.7.7/stackview.egg-info/SOURCES.txt` & `stackview-0.7.8/stackview.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 stackview/__init__.py
+stackview/_animate.py
 stackview/_annotate.py
 stackview/_assist.py
 stackview/_bia_bob_plugins.py
 stackview/_colormaps.py
 stackview/_context.py
 stackview/_crop.py
 stackview/_curtain.py
```

