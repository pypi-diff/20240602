# Comparing `tmp/stackview-0.7.8.tar.gz` & `tmp/stackview-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackview-0.7.8.tar", last modified: Sun Jun  2 10:54:31 2024, max compression
+gzip compressed data, was "stackview-0.7.9.tar", last modified: Sun Jun  2 15:14:54 2024, max compression
```

## Comparing `stackview-0.7.8.tar` & `stackview-0.7.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 10:54:31.599009 stackview-0.7.8/
--rw-rw-rw-   0        0        0     1549 2022-11-28 22:36:36.000000 stackview-0.7.8/LICENSE
--rw-rw-rw-   0        0        0    12658 2024-06-02 10:54:31.598006 stackview-0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0    11824 2024-06-02 10:52:28.000000 stackview-0.7.8/README.md
--rw-rw-rw-   0        0        0       42 2024-06-02 10:54:31.599009 stackview-0.7.8/setup.cfg
--rw-rw-rw-   0        0        0     1125 2024-06-02 10:54:12.000000 stackview-0.7.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:54:31.566637 stackview-0.7.8/stackview/
--rw-rw-rw-   0        0        0      661 2024-06-02 10:52:28.000000 stackview-0.7.8/stackview/__init__.py
--rw-rw-rw-   0        0        0     5616 2024-06-02 10:52:28.000000 stackview-0.7.8/stackview/_animate.py
--rw-rw-rw-   0        0        0     7993 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_annotate.py
--rw-rw-rw-   0        0        0     5101 2023-03-26 19:33:45.000000 stackview-0.7.8/stackview/_assist.py
--rw-rw-rw-   0        0        0     1429 2024-03-23 12:49:32.000000 stackview-0.7.8/stackview/_bia_bob_plugins.py
--rw-rw-rw-   0        0        0     5467 2023-04-15 09:27:34.000000 stackview-0.7.8/stackview/_colormaps.py
--rw-rw-rw-   0        0        0     2060 2023-01-01 15:16:44.000000 stackview-0.7.8/stackview/_context.py
--rw-rw-rw-   0        0        0     5584 2024-05-24 13:35:04.000000 stackview-0.7.8/stackview/_crop.py
--rw-rw-rw-   0        0        0     5184 2024-06-02 10:49:36.000000 stackview-0.7.8/stackview/_curtain.py
--rw-rw-rw-   0        0        0     4115 2023-11-17 12:56:59.000000 stackview-0.7.8/stackview/_image_widget.py
--rw-rw-rw-   0        0        0     4457 2024-05-24 13:45:55.000000 stackview-0.7.8/stackview/_imshow.py
--rw-rw-rw-   0        0        0     7964 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_interact.py
--rw-rw-rw-   0        0        0     2367 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_orthogonal.py
--rw-rw-rw-   0        0        0     3516 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_picker.py
--rw-rw-rw-   0        0        0     5252 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_side_by_side.py
--rw-rw-rw-   0        0        0     2280 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_slice.py
--rw-rw-rw-   0        0        0     2823 2024-03-23 13:51:50.000000 stackview-0.7.8/stackview/_slice_viewer.py
--rw-rw-rw-   0        0        0     8753 2023-10-19 19:42:08.000000 stackview-0.7.8/stackview/_static_view.py
--rw-rw-rw-   0        0        0     6551 2024-03-30 17:27:56.000000 stackview-0.7.8/stackview/_switch.py
--rw-rw-rw-   0        0        0     1066 2022-12-30 17:39:31.000000 stackview-0.7.8/stackview/_uint_field.py
--rw-rw-rw-   0        0        0     2567 2023-01-01 15:16:44.000000 stackview-0.7.8/stackview/_utilities.py
-drwxrwxrwx   0        0        0        0 2024-06-02 10:54:31.597005 stackview-0.7.8/stackview.egg-info/
--rw-rw-rw-   0        0        0    12658 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       93 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-06-02 10:54:31.000000 stackview-0.7.8/stackview.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 15:14:54.016888 stackview-0.7.9/
+-rw-rw-rw-   0        0        0     1549 2022-11-28 22:36:36.000000 stackview-0.7.9/LICENSE
+-rw-rw-rw-   0        0        0    12344 2024-06-02 15:14:54.015885 stackview-0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11522 2024-06-02 15:14:32.000000 stackview-0.7.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 15:14:54.016888 stackview-0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2024-06-02 15:12:13.000000 stackview-0.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:14:53.985807 stackview-0.7.9/stackview/
+-rw-rw-rw-   0        0        0      661 2024-06-02 15:12:13.000000 stackview-0.7.9/stackview/__init__.py
+-rw-rw-rw-   0        0        0     6805 2024-06-02 15:11:46.000000 stackview-0.7.9/stackview/_animate.py
+-rw-rw-rw-   0        0        0     7993 2024-03-23 13:51:50.000000 stackview-0.7.9/stackview/_annotate.py
+-rw-rw-rw-   0        0        0     5101 2023-03-26 19:33:45.000000 stackview-0.7.9/stackview/_assist.py
+-rw-rw-rw-   0        0        0     1429 2024-03-23 12:49:32.000000 stackview-0.7.9/stackview/_bia_bob_plugins.py
+-rw-rw-rw-   0        0        0     5467 2023-04-15 09:27:34.000000 stackview-0.7.9/stackview/_colormaps.py
+-rw-rw-rw-   0        0        0     2060 2023-01-01 15:16:44.000000 stackview-0.7.9/stackview/_context.py
+-rw-rw-rw-   0        0        0     5584 2024-05-24 13:35:04.000000 stackview-0.7.9/stackview/_crop.py
+-rw-rw-rw-   0        0        0     5184 2024-06-02 10:49:36.000000 stackview-0.7.9/stackview/_curtain.py
+-rw-rw-rw-   0        0        0     4115 2023-11-17 12:56:59.000000 stackview-0.7.9/stackview/_image_widget.py
+-rw-rw-rw-   0        0        0     4457 2024-05-24 13:45:55.000000 stackview-0.7.9/stackview/_imshow.py
+-rw-rw-rw-   0        0        0     7964 2024-03-23 13:51:50.000000 stackview-0.7.9/stackview/_interact.py
+-rw-rw-rw-   0        0        0     2367 2024-03-23 13:51:50.000000 stackview-0.7.9/stackview/_orthogonal.py
+-rw-rw-rw-   0        0        0     3516 2024-03-23 13:51:50.000000 stackview-0.7.9/stackview/_picker.py
+-rw-rw-rw-   0        0        0     5252 2024-03-23 13:51:50.000000 stackview-0.7.9/stackview/_side_by_side.py
+-rw-rw-rw-   0        0        0     2280 2024-03-23 13:51:50.000000 stackview-0.7.9/stackview/_slice.py
+-rw-rw-rw-   0        0        0     2823 2024-03-23 13:51:50.000000 stackview-0.7.9/stackview/_slice_viewer.py
+-rw-rw-rw-   0        0        0     8753 2023-10-19 19:42:08.000000 stackview-0.7.9/stackview/_static_view.py
+-rw-rw-rw-   0        0        0     6551 2024-03-30 17:27:56.000000 stackview-0.7.9/stackview/_switch.py
+-rw-rw-rw-   0        0        0     1066 2022-12-30 17:39:31.000000 stackview-0.7.9/stackview/_uint_field.py
+-rw-rw-rw-   0        0        0     3625 2024-06-02 15:11:46.000000 stackview-0.7.9/stackview/_utilities.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:14:54.014882 stackview-0.7.9/stackview.egg-info/
+-rw-rw-rw-   0        0        0    12344 2024-06-02 15:14:53.000000 stackview-0.7.9/stackview.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2024-06-02 15:14:53.000000 stackview-0.7.9/stackview.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 15:14:53.000000 stackview-0.7.9/stackview.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-06-02 15:14:53.000000 stackview-0.7.9/stackview.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       93 2024-06-02 15:14:53.000000 stackview-0.7.9/stackview.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 15:14:53.000000 stackview-0.7.9/stackview.egg-info/top_level.txt
```

### Comparing `stackview-0.7.8/LICENSE` & `stackview-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/PKG-INFO` & `stackview-0.7.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.7.8
+Version: 0.7.9
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@uni-leipzig.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -119,22 +119,22 @@
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/imshow.png)
 
 
 ### Static animations
 
 The `animate` and `animate_curtain` functions can be used to store animations of image stacks / images blended over each other as gif to disk.
 
-Â´Â´Â´
-stackview.animate(blobs_images, filename="images/timelapse2.gif", frame_delay_ms=50)
-Â´Â´Â´
+```python
+stackview.animate(blobs_images, frame_delay_ms=50)
+```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse2.gif)
 
 ```python
-stackview.animate_curtain(blobs, blobs > 128, filename="images/timelapse3.gif")
+stackview.animate_curtain(blobs, blobs > 128)
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse3.gif)
 
 ### Annotate regions
 
 To create label images interactively, e.g. for machine learning training, the `stackview.annotate` function offers basic label drawing tools. 
@@ -152,58 +152,58 @@
 
 Note: In case the interface is slow, consider using smaller images, e.g. by cropping or resampling.
 
 ### Pick intensities
 
 To read the intensity of pixels where the mouse is moving, use the picker.
 ```python
-stackview.picker(image, continuous_update=True)
+stackview.picker(image)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_picker.gif)
 
 ### Orthogonal view
 
 Orthogonal views are also available:
 ```python
-stackview.orthogonal(image, continuous_update=True)
+stackview.orthogonal(image)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_orthogonal.gif)
 
 ### Curtain
 
 Furthermore, to visualize an original image in combination with a processed version, a curtain view may be helpful:
 ```python
-stackview.curtain(image, modified_image * 65537, continuous_update=True)
+stackview.curtain(image, modified_image * 65537)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_curtain.gif)
 
 The curtain also works with 2D data. 
 Btw. to visualize both images properly, you need adjust their grey value range yourself. 
 For example, multiply a binary image with 255 so that it visualizes nicely side-by-side with the original image in 8-bit range:
 ```python
 binary = (slice_image > threshold_otsu(slice_image)) * 255
-stackview.curtain(slice_image, binary, continuous_update=True)
+stackview.curtain(slice_image, binary)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_curtain2.gif)
 
 The same also works with label images
 ```python
 from skimage.measure import label
 labels = label(binary)
-stackview.curtain(slice_image, labels, continuous_update=True)
+stackview.curtain(slice_image, labels)
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_curtain3.gif)
 
 ### Side-by-side view
 
 A side-by-side view for colocalization visualization is also available.
 If you're working with time-lapse data, you can also use this view for visualizing differences between timepoints:
 ```python
-stackview.side_by_side(image_stack[1:], image_stack[:-1], continuous_update=True, display_width=300)
+stackview.side_by_side(image_stack[1:], image_stack[:-1])
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_side_by_side.gif)
 
 ### Switch
 
 The `switch` function allows to switch between a list or dictionary of images.
 
@@ -238,15 +238,15 @@
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_switch_toggleable.gif)
 
 
 ### Crop
 
 You can crop images interactively:
 ```python
-crop_widget = stackview.crop(image_stack, continuous_update=True)
+crop_widget = stackview.crop(image_stack)
 crop_widget
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/crop.gif)
 
 ... and retrieve the crop range as a tuple of `slice` objects:
 ```python
@@ -296,15 +296,15 @@
 
 If you want to use a pulldown for selecting input image(s), you need to pass a dictionary of `(name, image)` pairs as `context`, e.g. `context=globals()`:
 
 ```python
 image1 = imread("data/Haase_MRT_tfl3d1.tif")
 image2 = image1[:,:,::-1]
 
-stackview.interact(gaussian, context=globals(), continuous_update=True)
+stackview.interact(gaussian, context=globals())
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_interact4.gif)
 
 To add an `insight`-view automatically to results of functions, you can add this.
 
 ```python
@@ -317,18 +317,18 @@
 
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/jupyter_displayable_output.png)
 
 ### Assist
 
 The `stackview.assist()` function can guide you through all imported (and supported) image processing functions.
 Note: The interface may be slow or crash if you have many functions imported. Consider using it in an empty notebook 
-with only functions or library imported that might be relevant for the taks.
+with only functions or library imported that might be relevant for the tasks.
 
 ```python
-stackview.assist(context=globals(), continuous_update=True)
+stackview.assist(context=globals())
 ```
 
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_assist.gif)
 
 ## Voila
 
 If you combine stackview with [voila](https://voila.readthedocs.io/en/stable/), you can build powerful, interactive, browser-based image processing apps and demonstrators. Just build a graphical user interface in a Jupyter notebook and then start it using
```

### Comparing `stackview-0.7.8/README.md` & `stackview-0.7.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -94,22 +94,22 @@
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/imshow.png)
 
 
 ### Static animations
 
 The `animate` and `animate_curtain` functions can be used to store animations of image stacks / images blended over each other as gif to disk.
 
-´´´
-stackview.animate(blobs_images, filename="images/timelapse2.gif", frame_delay_ms=50)
-´´´
+```python
+stackview.animate(blobs_images, frame_delay_ms=50)
+```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse2.gif)
 
 ```python
-stackview.animate_curtain(blobs, blobs > 128, filename="images/timelapse3.gif")
+stackview.animate_curtain(blobs, blobs > 128)
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse3.gif)
 
 ### Annotate regions
 
 To create label images interactively, e.g. for machine learning training, the `stackview.annotate` function offers basic label drawing tools. 
@@ -127,58 +127,58 @@
 
 Note: In case the interface is slow, consider using smaller images, e.g. by cropping or resampling.
 
 ### Pick intensities
 
 To read the intensity of pixels where the mouse is moving, use the picker.
 ```python
-stackview.picker(image, continuous_update=True)
+stackview.picker(image)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_picker.gif)
 
 ### Orthogonal view
 
 Orthogonal views are also available:
 ```python
-stackview.orthogonal(image, continuous_update=True)
+stackview.orthogonal(image)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_orthogonal.gif)
 
 ### Curtain
 
 Furthermore, to visualize an original image in combination with a processed version, a curtain view may be helpful:
 ```python
-stackview.curtain(image, modified_image * 65537, continuous_update=True)
+stackview.curtain(image, modified_image * 65537)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_curtain.gif)
 
 The curtain also works with 2D data. 
 Btw. to visualize both images properly, you need adjust their grey value range yourself. 
 For example, multiply a binary image with 255 so that it visualizes nicely side-by-side with the original image in 8-bit range:
 ```python
 binary = (slice_image > threshold_otsu(slice_image)) * 255
-stackview.curtain(slice_image, binary, continuous_update=True)
+stackview.curtain(slice_image, binary)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_curtain2.gif)
 
 The same also works with label images
 ```python
 from skimage.measure import label
 labels = label(binary)
-stackview.curtain(slice_image, labels, continuous_update=True)
+stackview.curtain(slice_image, labels)
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_curtain3.gif)
 
 ### Side-by-side view
 
 A side-by-side view for colocalization visualization is also available.
 If you're working with time-lapse data, you can also use this view for visualizing differences between timepoints:
 ```python
-stackview.side_by_side(image_stack[1:], image_stack[:-1], continuous_update=True, display_width=300)
+stackview.side_by_side(image_stack[1:], image_stack[:-1])
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_side_by_side.gif)
 
 ### Switch
 
 The `switch` function allows to switch between a list or dictionary of images.
 
@@ -213,15 +213,15 @@
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_switch_toggleable.gif)
 
 
 ### Crop
 
 You can crop images interactively:
 ```python
-crop_widget = stackview.crop(image_stack, continuous_update=True)
+crop_widget = stackview.crop(image_stack)
 crop_widget
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/crop.gif)
 
 ... and retrieve the crop range as a tuple of `slice` objects:
 ```python
@@ -271,15 +271,15 @@
 
 If you want to use a pulldown for selecting input image(s), you need to pass a dictionary of `(name, image)` pairs as `context`, e.g. `context=globals()`:
 
 ```python
 image1 = imread("data/Haase_MRT_tfl3d1.tif")
 image2 = image1[:,:,::-1]
 
-stackview.interact(gaussian, context=globals(), continuous_update=True)
+stackview.interact(gaussian, context=globals())
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_interact4.gif)
 
 To add an `insight`-view automatically to results of functions, you can add this.
 
 ```python
@@ -292,18 +292,18 @@
 
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/jupyter_displayable_output.png)
 
 ### Assist
 
 The `stackview.assist()` function can guide you through all imported (and supported) image processing functions.
 Note: The interface may be slow or crash if you have many functions imported. Consider using it in an empty notebook 
-with only functions or library imported that might be relevant for the taks.
+with only functions or library imported that might be relevant for the tasks.
 
 ```python
-stackview.assist(context=globals(), continuous_update=True)
+stackview.assist(context=globals())
 ```
 
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_assist.gif)
 
 ## Voila
 
 If you combine stackview with [voila](https://voila.readthedocs.io/en/stable/), you can build powerful, interactive, browser-based image processing apps and demonstrators. Just build a graphical user interface in a Jupyter notebook and then start it using
```

### Comparing `stackview-0.7.8/setup.py` & `stackview-0.7.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stackview",
-    version="0.7.8",
+    version="0.7.9",
     author="Robert Haase",
     author_email="robert.haase@uni-leipzig.de",
     description="Interactive image stack viewing in jupyter notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/haesleinhuepf/stackview/",
     packages=setuptools.find_packages(),
```

### Comparing `stackview-0.7.8/stackview/__init__.py` & `stackview-0.7.9/stackview/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.8"
+__version__ = "0.7.9"
 
 from ._static_view import jupyter_displayable_output, insight
 from ._utilities import merge_rgb
 from ._context import nop
 from ._crop import crop
 from ._slice_viewer import _SliceViewer
 from ._annotate import annotate
```

### Comparing `stackview-0.7.8/stackview/_animate.py` & `stackview-0.7.9/stackview/_animate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,351 +1,426 @@
 00000000: 0d0a 6465 6620 616e 696d 6174 6528 7469  ..def animate(ti
 00000010: 6d65 6c61 7073 652c 2066 696c 656e 616d  melapse, filenam
 00000020: 653a 7374 723d 4e6f 6e65 2c20 6f76 6572  e:str=None, over
 00000030: 7772 6974 655f 6669 6c65 3a62 6f6f 6c3d  write_file:bool=
-00000040: 4e6f 6e65 2c20 6672 616d 655f 6465 6c61  None, frame_dela
+00000040: 5472 7565 2c20 6672 616d 655f 6465 6c61  True, frame_dela
 00000050: 795f 6d73 3a69 6e74 3d31 3530 2c20 6e75  y_ms:int=150, nu
 00000060: 6d5f 6c6f 6f70 733a 696e 743d 3130 3030  m_loops:int=1000
-00000070: 293a 0d0a 2020 2020 2222 220d 0a20 2020  ):..    """..   
-00000080: 2043 7265 6174 6520 616e 2061 6e69 6d61   Create an anima
-00000090: 7465 6420 4749 4620 6672 6f6d 2061 206c  ted GIF from a l
-000000a0: 6973 7420 6f66 2032 4420 696d 6167 6573  ist of 2D images
-000000b0: 2061 6e64 2072 6574 7572 6e20 6974 2061   and return it a
-000000c0: 7320 4d61 726b 646f 776e 206f 626a 6563  s Markdown objec
-000000d0: 742c 2074 6861 7420 6361 6e20 6265 2073  t, that can be s
-000000e0: 686f 776e 2069 6e20 4a75 7079 7465 7220  hown in Jupyter 
-000000f0: 6e6f 7465 626f 6f6b 732e 0d0a 2020 2020  notebooks...    
-00000100: 5247 4220 696d 6167 6573 2061 7265 2073  RGB images are s
-00000110: 7570 706f 7274 6564 2061 7320 7765 6c6c  upported as well
-00000120: 2c20 6275 7420 6e6f 2033 4420 696d 6167  , but no 3D imag
-00000130: 6520 7374 6163 6b73 2e0d 0a0d 0a20 2020  e stacks.....   
-00000140: 204e 6f74 653a 2049 7420 6973 2072 6563   Note: It is rec
-00000150: 6f6d 6d65 6e64 6564 2074 6f20 6e6f 726d  ommended to norm
-00000160: 616c 697a 6520 7468 6520 7469 6d65 6c61  alize the timela
-00000170: 7073 6520 746f 2062 6520 696e 7465 6765  pse to be intege
-00000180: 7273 2069 6e20 7468 6520 7261 6e67 6520  rs in the range 
-00000190: 6265 7477 6565 6e20 3020 746f 2032 3535  between 0 to 255
-000001a0: 2e0d 0a0d 0a20 2020 2050 6172 616d 6574  .....    Paramet
-000001b0: 6572 730d 0a20 2020 202d 2d2d 2d2d 2d2d  ers..    -------
-000001c0: 2d2d 2d0d 0a20 2020 2074 696d 656c 6170  ---..    timelap
-000001d0: 7365 3a20 6e70 2e6e 6461 7272 6179 0d0a  se: np.ndarray..
-000001e0: 2020 2020 2020 2020 3244 2069 6d61 6765          2D image
-000001f0: 206f 7220 3344 2069 6d61 6765 2073 7461   or 3D image sta
-00000200: 636b 0d0a 2020 2020 6669 6c65 6e61 6d65  ck..    filename
-00000210: 3a20 7374 722c 206f 7074 696f 6e61 6c0d  : str, optional.
-00000220: 0a20 2020 2020 2020 204e 616d 6520 6f66  .        Name of
-00000230: 2074 6865 2066 696c 6520 7768 6572 6520   the file where 
-00000240: 7468 6520 616e 696d 6174 696f 6e20 7769  the animation wi
-00000250: 6c6c 2062 6520 7361 7665 640d 0a20 2020  ll be saved..   
-00000260: 206f 7665 7277 7269 7465 5f66 696c 653a   overwrite_file:
-00000270: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
-00000280: 0a20 2020 2020 2020 204f 7665 7277 7269  .        Overwri
-00000290: 7465 2074 6865 2066 696c 6520 6966 2069  te the file if i
-000002a0: 7420 616c 7265 6164 7920 6578 6973 7473  t already exists
-000002b0: 2e20 4465 6661 756c 743a 2054 7275 6520  . Default: True 
-000002c0: 6966 2066 696c 656e 616d 6520 6973 2067  if filename is g
-000002d0: 6976 656e 2c20 4661 6c73 6520 6f74 6865  iven, False othe
-000002e0: 7277 6973 650d 0a20 2020 2066 7261 6d65  rwise..    frame
-000002f0: 5f64 656c 6179 5f6d 733a 2069 6e74 2c20  _delay_ms: int, 
-00000300: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00000310: 2020 4465 6c61 7920 6265 7477 6565 6e20    Delay between 
-00000320: 6672 616d 6573 2069 6e20 6d69 6c6c 6973  frames in millis
-00000330: 6563 6f6e 6473 0d0a 2020 2020 6e75 6d5f  econds..    num_
-00000340: 6c6f 6f70 733a 2069 6e74 2c20 6f70 7469  loops: int, opti
-00000350: 6f6e 616c 0d0a 2020 2020 2020 2020 4e75  onal..        Nu
-00000360: 6d62 6572 206f 6620 6c6f 6f70 7320 696e  mber of loops in
-00000370: 2074 6865 2061 6e69 6d61 7469 6f6e 0d0a   the animation..
-00000380: 0d0a 2020 2020 2222 220d 0a20 2020 2069  ..    """..    i
-00000390: 6d70 6f72 7420 6f73 0d0a 2020 2020 696d  mport os..    im
-000003a0: 706f 7274 2069 6d61 6765 696f 0d0a 2020  port imageio..  
-000003b0: 2020 6672 6f6d 2049 5079 7468 6f6e 2e64    from IPython.d
-000003c0: 6973 706c 6179 2069 6d70 6f72 7420 4d61  isplay import Ma
-000003d0: 726b 646f 776e 0d0a 2020 2020 696d 706f  rkdown..    impo
-000003e0: 7274 206e 756d 7079 2061 7320 6e70 0d0a  rt numpy as np..
-000003f0: 2020 2020 696d 706f 7274 2077 6172 6e69      import warni
-00000400: 6e67 730d 0a0d 0a20 2020 2069 6620 6f76  ngs....    if ov
-00000410: 6572 7772 6974 655f 6669 6c65 2069 7320  erwrite_file is 
-00000420: 4e6f 6e65 3a0d 0a20 2020 2020 2020 206f  None:..        o
-00000430: 7665 7277 7269 7465 5f66 696c 6520 3d20  verwrite_file = 
-00000440: 6669 6c65 6e61 6d65 2069 7320 6e6f 7420  filename is not 
-00000450: 4e6f 6e65 0d0a 0d0a 2020 2020 6966 2066  None....    if f
-00000460: 696c 656e 616d 6520 6973 204e 6f6e 653a  ilename is None:
-00000470: 0d0a 2020 2020 2020 2020 6669 6c65 6e61  ..        filena
-00000480: 6d65 203d 2022 616e 696d 6174 696f 6e2e  me = "animation.
-00000490: 6769 6622 0d0a 0d0a 2020 2020 6966 206e  gif"....    if n
-000004a0: 6f74 2066 696c 656e 616d 652e 656e 6473  ot filename.ends
-000004b0: 7769 7468 2822 2e67 6966 2229 3a0d 0a20  with(".gif"):.. 
-000004c0: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
-000004d0: 2b3d 2022 2e67 6966 220d 0a0d 0a20 2020  += ".gif"....   
-000004e0: 2069 6620 3020 3c3d 2074 696d 656c 6170   if 0 <= timelap
-000004f0: 7365 2e6d 696e 2829 203c 3d20 3120 616e  se.min() <= 1 an
-00000500: 6420 3020 3c3d 2074 696d 656c 6170 7365  d 0 <= timelapse
-00000510: 2e6d 6178 2829 203c 3d20 313a 0d0a 2020  .max() <= 1:..  
-00000520: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-00000530: 6172 6e28 2254 6865 2074 696d 656c 6170  arn("The timelap
-00000540: 7365 2068 6173 2061 2073 6d61 6c6c 2069  se has a small i
-00000550: 6e74 656e 7369 7479 2072 616e 6765 2062  ntensity range b
-00000560: 6574 7765 656e 2030 2061 6e64 2031 2e20  etween 0 and 1. 
-00000570: 436f 6e73 6964 6572 206e 6f72 6d61 6c69  Consider normali
-00000580: 7a69 6e67 2069 7420 746f 2074 6865 2072  zing it to the r
-00000590: 616e 6765 2062 6574 7765 656e 2030 2061  ange between 0 a
-000005a0: 6e64 2032 3535 2e22 290d 0a20 2020 2069  nd 255.")..    i
-000005b0: 6620 7469 6d65 6c61 7073 652e 6d69 6e28  f timelapse.min(
-000005c0: 2920 3c20 3020 6f72 2074 696d 656c 6170  ) < 0 or timelap
-000005d0: 7365 2e6d 6178 2829 203e 2032 3535 3a0d  se.max() > 255:.
-000005e0: 0a20 2020 2020 2020 2077 6172 6e69 6e67  .        warning
-000005f0: 732e 7761 726e 2822 5468 6520 7469 6d65  s.warn("The time
-00000600: 6c61 7073 6520 6861 7320 616e 2069 6e74  lapse has an int
-00000610: 656e 7369 7479 2072 616e 6765 2065 7863  ensity range exc
-00000620: 6565 6469 6e67 2030 2e2e 3235 352e 2043  eeding 0..255. C
-00000630: 6f6e 7369 6465 7220 6e6f 726d 616c 697a  onsider normaliz
-00000640: 696e 6720 6974 2074 6f20 7468 6520 7261  ing it to the ra
-00000650: 6e67 6520 6265 7477 6565 6e20 3020 616e  nge between 0 an
-00000660: 6420 3235 352e 2229 0d0a 0d0a 2020 2020  d 255.")....    
-00000670: 6966 206e 6f74 206f 7665 7277 7269 7465  if not overwrite
-00000680: 5f66 696c 653a 0d0a 2020 2020 2020 2020  _file:..        
-00000690: 6920 3d20 300d 0a20 2020 2020 2020 206f  i = 0..        o
-000006a0: 7269 6769 6e61 6c5f 6669 6c65 6e61 6d65  riginal_filename
-000006b0: 203d 2066 696c 656e 616d 650d 0a20 2020   = filename..   
-000006c0: 2020 2020 2077 6869 6c65 206f 732e 7061       while os.pa
-000006d0: 7468 2e65 7869 7374 7328 6669 6c65 6e61  th.exists(filena
-000006e0: 6d65 293a 0d0a 2020 2020 2020 2020 2020  me):..          
-000006f0: 2020 6920 2b3d 2031 0d0a 2020 2020 2020    i += 1..      
-00000700: 2020 2020 2020 6669 6c65 6e61 6d65 203d        filename =
-00000710: 206f 7269 6769 6e61 6c5f 6669 6c65 6e61   original_filena
-00000720: 6d65 2e72 6570 6c61 6365 2822 2e67 6966  me.replace(".gif
-00000730: 222c 2066 225f 7b69 3a30 327d 2e67 6966  ", f"_{i:02}.gif
-00000740: 2229 0d0a 0d0a 2020 2020 7769 7468 2069  ")....    with i
-00000750: 6d61 6765 696f 2e67 6574 5f77 7269 7465  mageio.get_write
-00000760: 7228 6669 6c65 6e61 6d65 2c20 6d6f 6465  r(filename, mode
-00000770: 3d27 4927 2c20 6475 7261 7469 6f6e 3d66  ='I', duration=f
-00000780: 7261 6d65 5f64 656c 6179 5f6d 732c 206c  rame_delay_ms, l
-00000790: 6f6f 703d 6e75 6d5f 6c6f 6f70 7329 2061  oop=num_loops) a
-000007a0: 7320 7772 6974 6572 3a0d 0a20 2020 2020  s writer:..     
-000007b0: 2020 2066 6f72 2066 7261 6d65 2069 6e20     for frame in 
-000007c0: 7469 6d65 6c61 7073 653a 0d0a 2020 2020  timelapse:..    
-000007d0: 2020 2020 2020 2020 7772 6974 6572 2e61          writer.a
-000007e0: 7070 656e 645f 6461 7461 2866 7261 6d65  ppend_data(frame
-000007f0: 2e61 7374 7970 6528 6e70 2e75 696e 7438  .astype(np.uint8
-00000800: 2929 0d0a 0d0a 2020 2020 7265 7475 726e  ))....    return
-00000810: 204d 6172 6b64 6f77 6e28 6622 215b 5d28   Markdown(f"![](
-00000820: 7b66 696c 656e 616d 657d 2922 290d 0a0d  {filename})")...
-00000830: 0a0d 0a64 6566 2061 6e69 6d61 7465 5f63  ...def animate_c
-00000840: 7572 7461 696e 2874 696d 656c 6170 7365  urtain(timelapse
-00000850: 2c20 7469 6d65 6c61 7073 655f 6375 7274  , timelapse_curt
-00000860: 6169 6e2c 2063 6f6c 6f72 6d61 703d 4e6f  ain, colormap=No
-00000870: 6e65 2c20 6469 7370 6c61 795f 6d69 6e3d  ne, display_min=
-00000880: 4e6f 6e65 2c20 6469 7370 6c61 795f 6d61  None, display_ma
-00000890: 783d 4e6f 6e65 2c0d 0a20 2020 2020 2020  x=None,..       
-000008a0: 2020 2020 2020 2020 2020 2020 2061 7869               axi
-000008b0: 733a 2069 6e74 203d 2030 2c0d 0a20 2020  s: int = 0,..   
-000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008d0: 2061 6c70 6861 3a20 666c 6f61 7420 3d20   alpha: float = 
-000008e0: 312c 0d0a 2020 2020 2020 2020 2020 2020  1,..            
-000008f0: 2020 2020 2020 2020 6e75 6d5f 7374 6570          num_step
-00000900: 733a 696e 7420 3d20 3230 2c0d 0a20 2020  s:int = 20,..   
-00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000920: 2063 7572 7461 696e 5f63 6f6c 6f72 6d61   curtain_colorma
-00000930: 703a 7374 7220 3d20 4e6f 6e65 2c0d 0a20  p:str = None,.. 
-00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000950: 2020 2063 7572 7461 696e 5f64 6973 706c     curtain_displ
-00000960: 6179 5f6d 696e 3a66 6c6f 6174 203d 204e  ay_min:float = N
-00000970: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-00000980: 2020 2020 2020 2020 2020 6375 7274 6169            curtai
-00000990: 6e5f 6469 7370 6c61 795f 6d61 783a 666c  n_display_max:fl
-000009a0: 6f61 7420 3d20 4e6f 6e65 2c0d 0a20 2020  oat = None,..   
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2066 696c 656e 616d 653a 7374 723d 4e6f   filename:str=No
-000009d0: 6e65 2c20 6f76 6572 7772 6974 655f 6669  ne, overwrite_fi
-000009e0: 6c65 3a62 6f6f 6c3d 4661 6c73 652c 2066  le:bool=False, f
-000009f0: 7261 6d65 5f64 656c 6179 5f6d 733a 696e  rame_delay_ms:in
-00000a00: 743d 3135 302c 206e 756d 5f6c 6f6f 7073  t=150, num_loops
-00000a10: 3a69 6e74 3d31 3030 3029 3a0d 0a20 2020  :int=1000):..   
-00000a20: 2022 2222 0d0a 2020 2020 5265 6e64 6572   """..    Render
-00000a30: 2061 2063 7572 7461 696e 2073 686f 7769   a curtain showi
-00000a40: 6e67 2074 776f 2032 4420 696d 6167 6573  ng two 2D images
-00000a50: 2e20 5247 4220 696d 6167 6573 2061 7265  . RGB images are
-00000a60: 2073 7570 706f 7274 6564 2061 7320 7765   supported as we
-00000a70: 6c6c 2c20 6275 7420 6e6f 2033 4420 696d  ll, but no 3D im
-00000a80: 6167 6520 7374 6163 6b73 2e0d 0a0d 0a20  age stacks..... 
-00000a90: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-00000aa0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-00000ab0: 2020 2074 696d 656c 6170 7365 3a20 6e70     timelapse: np
-00000ac0: 2e6e 6461 7272 6179 0d0a 2020 2020 2020  .ndarray..      
-00000ad0: 2020 3244 2069 6d61 6765 206f 7220 3344    2D image or 3D
-00000ae0: 2069 6d61 6765 2073 7461 636b 0d0a 2020   image stack..  
-00000af0: 2020 7469 6d65 6c61 7073 655f 6375 7274    timelapse_curt
-00000b00: 6169 6e3a 206e 702e 6e64 6172 7261 790d  ain: np.ndarray.
-00000b10: 0a20 2020 2020 2020 2032 4420 696d 6167  .        2D imag
-00000b20: 6520 6f72 2033 4420 696d 6167 6520 7374  e or 3D image st
-00000b30: 6163 6b0d 0a20 2020 2063 6f6c 6f72 6d61  ack..    colorma
-00000b40: 703a 2073 7472 2c20 6f70 7469 6f6e 616c  p: str, optional
-00000b50: 0d0a 2020 2020 2020 2020 4d61 7470 6c6f  ..        Matplo
-00000b60: 746c 6962 2063 6f6c 6f72 6d61 7020 6e61  tlib colormap na
-00000b70: 6d65 206f 7220 2270 7572 655f 6772 6565  me or "pure_gree
-00000b80: 6e22 2c20 2270 7572 655f 6d61 6765 6e74  n", "pure_magent
-00000b90: 6122 2c20 2e2e 2e0d 0a20 2020 2064 6973  a", .....    dis
-00000ba0: 706c 6179 5f6d 696e 3a20 666c 6f61 742c  play_min: float,
-00000bb0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-00000bc0: 2020 204c 6f77 6572 2062 6f75 6e64 206f     Lower bound o
-00000bd0: 6620 7072 6f70 6572 6c79 2073 686f 776e  f properly shown
-00000be0: 2069 6e74 656e 7369 7469 6573 0d0a 2020   intensities..  
-00000bf0: 2020 6469 7370 6c61 795f 6d61 783a 2066    display_max: f
-00000c00: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0d0a  loat, optional..
-00000c10: 2020 2020 2020 2020 5570 7065 7220 626f          Upper bo
-00000c20: 756e 6420 6f66 2070 726f 7065 726c 7920  und of properly 
-00000c30: 7368 6f77 6e20 696e 7465 6e73 6974 6965  shown intensitie
-00000c40: 730d 0a20 2020 2061 7869 733a 2069 6e74  s..    axis: int
-00000c50: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00000c60: 2020 2020 4178 6973 2069 6e20 6361 7365      Axis in case
-00000c70: 2077 6520 6172 6520 736c 6963 696e 6720   we are slicing 
-00000c80: 6120 7374 6163 6b0d 0a20 2020 2061 6c70  a stack..    alp
-00000c90: 6861 3a20 666c 6f61 742c 206f 7074 696f  ha: float, optio
-00000ca0: 6e61 6c0d 0a20 2020 2020 2020 2073 6574  nal..        set
-00000cb0: 7320 7468 6520 7472 616e 7370 6172 656e  s the transparen
-00000cc0: 6379 206f 6620 7468 6520 6375 7274 6169  cy of the curtai
-00000cd0: 6e0d 0a20 2020 206e 756d 5f73 7465 7073  n..    num_steps
-00000ce0: 3a20 696e 742c 206f 7074 696f 6e61 6c0d  : int, optional.
-00000cf0: 0a20 2020 2020 2020 206e 756d 6265 7220  .        number 
-00000d00: 6f66 2073 7465 7073 2069 6e20 7468 6520  of steps in the 
-00000d10: 616e 696d 6174 696f 6e2c 2068 616c 6620  animation, half 
-00000d20: 6f66 2074 6865 6d20 7468 6520 6375 7274  of them the curt
-00000d30: 6169 6e20 7769 6c6c 2067 6f20 6c65 6674  ain will go left
-00000d40: 2d72 6967 6874 2c20 7468 6520 6f74 6865  -right, the othe
-00000d50: 7220 6861 6c66 2072 6967 6874 2d6c 6566  r half right-lef
-00000d60: 740d 0a20 2020 2063 7572 7461 696e 5f63  t..    curtain_c
-00000d70: 6f6c 6f72 6d61 703a 2073 7472 2c20 6f70  olormap: str, op
-00000d80: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00000d90: 4d61 7470 6c6f 746c 6962 2063 6f6c 6f72  Matplotlib color
-00000da0: 6d61 7020 6e61 6d65 206f 7220 2270 7572  map name or "pur
-00000db0: 655f 6772 6565 6e22 2c20 2270 7572 655f  e_green", "pure_
-00000dc0: 6d61 6765 6e74 6122 2c20 2e2e 2e0d 0a20  magenta", ..... 
-00000dd0: 2020 2063 7572 7461 696e 5f64 6973 706c     curtain_displ
-00000de0: 6179 5f6d 696e 3a20 666c 6f61 742c 206f  ay_min: float, o
-00000df0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-00000e00: 204c 6f77 6572 2062 6f75 6e64 206f 6620   Lower bound of 
-00000e10: 7072 6f70 6572 6c79 2073 686f 776e 2069  properly shown i
-00000e20: 6e74 656e 7369 7469 6573 0d0a 2020 2020  ntensities..    
-00000e30: 6375 7274 6169 6e5f 6469 7370 6c61 795f  curtain_display_
-00000e40: 6d61 783a 2066 6c6f 6174 2c20 6f70 7469  max: float, opti
-00000e50: 6f6e 616c 0d0a 2020 2020 2020 2020 5570  onal..        Up
-00000e60: 7065 7220 626f 756e 6420 6f66 2070 726f  per bound of pro
-00000e70: 7065 726c 7920 7368 6f77 6e20 696e 7465  perly shown inte
-00000e80: 6e73 6974 6965 730d 0a20 2020 2066 696c  nsities..    fil
-00000e90: 656e 616d 653a 2073 7472 2c20 6f70 7469  ename: str, opti
-00000ea0: 6f6e 616c 0d0a 2020 2020 2020 2020 4e61  onal..        Na
-00000eb0: 6d65 206f 6620 7468 6520 6669 6c65 2077  me of the file w
-00000ec0: 6865 7265 2074 6865 2061 6e69 6d61 7469  here the animati
-00000ed0: 6f6e 2077 696c 6c20 6265 2073 6176 6564  on will be saved
-00000ee0: 0d0a 2020 2020 6f76 6572 7772 6974 655f  ..    overwrite_
-00000ef0: 6669 6c65 3a20 626f 6f6c 2c20 6f70 7469  file: bool, opti
-00000f00: 6f6e 616c 0d0a 2020 2020 2020 2020 4f76  onal..        Ov
-00000f10: 6572 7772 6974 6520 7468 6520 6669 6c65  erwrite the file
-00000f20: 2069 6620 6974 2061 6c72 6561 6479 2065   if it already e
-00000f30: 7869 7374 730d 0a20 2020 2066 7261 6d65  xists..    frame
-00000f40: 5f64 656c 6179 5f6d 733a 2069 6e74 2c20  _delay_ms: int, 
-00000f50: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00000f60: 2020 4465 6c61 7920 6265 7477 6565 6e20    Delay between 
-00000f70: 6672 616d 6573 2069 6e20 6d69 6c6c 6973  frames in millis
-00000f80: 6563 6f6e 6473 0d0a 2020 2020 6e75 6d5f  econds..    num_
-00000f90: 6c6f 6f70 733a 2069 6e74 2c20 6f70 7469  loops: int, opti
-00000fa0: 6f6e 616c 0d0a 2020 2020 2020 2020 4e75  onal..        Nu
-00000fb0: 6d62 6572 206f 6620 6c6f 6f70 7320 696e  mber of loops in
-00000fc0: 2074 6865 2061 6e69 6d61 7469 6f6e 0d0a   the animation..
-00000fd0: 0d0a 2020 2020 2222 220d 0a20 2020 2069  ..    """..    i
-00000fe0: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
-00000ff0: 700d 0a20 2020 2066 726f 6d20 2e5f 696d  p..    from ._im
-00001000: 6167 655f 7769 6467 6574 2069 6d70 6f72  age_widget impor
-00001010: 7420 5f69 6d67 5f74 6f5f 7267 620d 0a0d  t _img_to_rgb...
-00001020: 0a20 2020 206d 6178 5f73 697a 6520 3d20  .    max_size = 
-00001030: 7469 6d65 6c61 7073 652e 7368 6170 655b  timelapse.shape[
-00001040: 6178 6973 5d0d 0a0d 0a20 2020 2069 6d61  axis]....    ima
-00001050: 6765 7320 3d20 5b5d 0d0a 2020 2020 7374  ges = []..    st
-00001060: 6570 7320 3d20 6c69 7374 2872 616e 6765  eps = list(range
-00001070: 2830 2c20 6d61 785f 7369 7a65 202b 2031  (0, max_size + 1
-00001080: 2c20 696e 7428 6d61 785f 7369 7a65 202f  , int(max_size /
-00001090: 206e 756d 5f73 7465 7073 202a 2032 2929   num_steps * 2))
-000010a0: 290d 0a20 2020 2073 7465 7073 203d 2073  )..    steps = s
-000010b0: 7465 7073 202b 2073 7465 7073 5b3a 3a2d  teps + steps[::-
-000010c0: 315d 0d0a 0d0a 2020 2020 666f 7220 736c  1]....    for sl
-000010d0: 6964 6572 5f76 616c 7565 2069 6e20 7374  ider_value in st
-000010e0: 6570 733a 0d0a 2020 2020 2020 2020 6966  eps:..        if
-000010f0: 206c 656e 2874 696d 656c 6170 7365 2e73   len(timelapse.s
-00001100: 6861 7065 2920 3c20 3320 6f72 2028 6c65  hape) < 3 or (le
-00001110: 6e28 7469 6d65 6c61 7073 652e 7368 6170  n(timelapse.shap
-00001120: 6529 203d 3d20 3320 616e 6420 7469 6d65  e) == 3 and time
-00001130: 6c61 7073 652e 7368 6170 655b 2d31 5d20  lapse.shape[-1] 
-00001140: 3d3d 2033 293a 0d0a 2020 2020 2020 2020  == 3):..        
-00001150: 2020 2020 696d 6167 655f 736c 6963 6520      image_slice 
-00001160: 3d20 5f69 6d67 5f74 6f5f 7267 6228 7469  = _img_to_rgb(ti
-00001170: 6d65 6c61 7073 652e 636f 7079 2829 2c20  melapse.copy(), 
-00001180: 636f 6c6f 726d 6170 3d63 6f6c 6f72 6d61  colormap=colorma
-00001190: 702c 2064 6973 706c 6179 5f6d 696e 3d64  p, display_min=d
-000011a0: 6973 706c 6179 5f6d 696e 2c20 6469 7370  isplay_min, disp
-000011b0: 6c61 795f 6d61 783d 6469 7370 6c61 795f  lay_max=display_
-000011c0: 6d61 7829 0d0a 2020 2020 2020 2020 2020  max)..          
-000011d0: 2020 696d 6167 655f 736c 6963 655f 6375    image_slice_cu
-000011e0: 7274 6169 6e20 3d20 5f69 6d67 5f74 6f5f  rtain = _img_to_
-000011f0: 7267 6228 7469 6d65 6c61 7073 655f 6375  rgb(timelapse_cu
-00001200: 7274 6169 6e2c 2063 6f6c 6f72 6d61 703d  rtain, colormap=
-00001210: 6375 7274 6169 6e5f 636f 6c6f 726d 6170  curtain_colormap
-00001220: 2c20 6469 7370 6c61 795f 6d69 6e3d 6375  , display_min=cu
-00001230: 7274 6169 6e5f 6469 7370 6c61 795f 6d69  rtain_display_mi
-00001240: 6e2c 0d0a 2020 2020 2020 2020 2020 2020  n,..            
-00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 2020 6469 7370 6c61 795f 6d61 783d 6375    display_max=cu
-00001280: 7274 6169 6e5f 6469 7370 6c61 795f 6d61  rtain_display_ma
-00001290: 7829 0d0a 2020 2020 2020 2020 656c 7365  x)..        else
-000012a0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-000012b0: 6d61 6765 5f73 6c69 6365 203d 205f 696d  mage_slice = _im
-000012c0: 675f 746f 5f72 6762 286e 702e 7461 6b65  g_to_rgb(np.take
-000012d0: 2874 696d 656c 6170 7365 2c20 736c 6964  (timelapse, slid
-000012e0: 6572 5f76 616c 7565 2c20 6178 6973 3d61  er_value, axis=a
-000012f0: 7869 7329 2c20 636f 6c6f 726d 6170 3d63  xis), colormap=c
-00001300: 6f6c 6f72 6d61 702c 0d0a 2020 2020 2020  olormap,..      
-00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001330: 6469 7370 6c61 795f 6d69 6e3d 6469 7370  display_min=disp
-00001340: 6c61 795f 6d69 6e2c 2064 6973 706c 6179  lay_min, display
-00001350: 5f6d 6178 3d64 6973 706c 6179 5f6d 6178  _max=display_max
-00001360: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00001370: 6d61 6765 5f73 6c69 6365 5f63 7572 7461  mage_slice_curta
-00001380: 696e 203d 205f 696d 675f 746f 5f72 6762  in = _img_to_rgb
-00001390: 286e 702e 7461 6b65 2874 696d 656c 6170  (np.take(timelap
-000013a0: 7365 5f63 7572 7461 696e 2c20 736c 6964  se_curtain, slid
-000013b0: 6572 5f76 616c 7565 2c20 6178 6973 3d61  er_value, axis=a
-000013c0: 7869 7329 2c0d 0a20 2020 2020 2020 2020  xis),..         
-000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013f0: 2020 2020 2063 6f6c 6f72 6d61 703d 6375       colormap=cu
-00001400: 7274 6169 6e5f 636f 6c6f 726d 6170 2c20  rtain_colormap, 
-00001410: 6469 7370 6c61 795f 6d69 6e3d 6375 7274  display_min=curt
-00001420: 6169 6e5f 6469 7370 6c61 795f 6d69 6e2c  ain_display_min,
-00001430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001460: 6469 7370 6c61 795f 6d61 783d 6375 7274  display_max=curt
-00001470: 6169 6e5f 6469 7370 6c61 795f 6d61 7829  ain_display_max)
-00001480: 0d0a 2020 2020 2020 2020 696d 6167 655f  ..        image_
-00001490: 736c 6963 655b 3a2c 2073 6c69 6465 725f  slice[:, slider_
-000014a0: 7661 6c75 653a 5d20 3d20 2831 202d 2061  value:] = (1 - a
-000014b0: 6c70 6861 2920 2a20 696d 6167 655f 736c  lpha) * image_sl
-000014c0: 6963 655b 3a2c 2073 6c69 6465 725f 7661  ice[:, slider_va
-000014d0: 6c75 653a 5d20 2b20 5c0d 0a20 2020 2020  lue:] + \..     
-000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001500: 2020 2020 2020 2020 2020 2061 6c70 6861             alpha
-00001510: 202a 2069 6d61 6765 5f73 6c69 6365 5f63   * image_slice_c
-00001520: 7572 7461 696e 5b3a 2c20 736c 6964 6572  urtain[:, slider
-00001530: 5f76 616c 7565 3a5d 0d0a 0d0a 2020 2020  _value:]....    
-00001540: 2020 2020 696d 6167 6573 2e61 7070 656e      images.appen
-00001550: 6428 696d 6167 655f 736c 6963 6529 0d0a  d(image_slice)..
-00001560: 0d0a 2020 2020 7265 7475 726e 2061 6e69  ..    return ani
-00001570: 6d61 7465 286e 702e 6173 6172 7261 7928  mate(np.asarray(
-00001580: 696d 6167 6573 292c 2066 696c 656e 616d  images), filenam
-00001590: 653d 6669 6c65 6e61 6d65 2c20 6f76 6572  e=filename, over
-000015a0: 7772 6974 655f 6669 6c65 3d6f 7665 7277  write_file=overw
-000015b0: 7269 7465 5f66 696c 652c 2066 7261 6d65  rite_file, frame
-000015c0: 5f64 656c 6179 5f6d 733d 6672 616d 655f  _delay_ms=frame_
-000015d0: 6465 6c61 795f 6d73 2c20 6e75 6d5f 6c6f  delay_ms, num_lo
-000015e0: 6f70 733d 6e75 6d5f 6c6f 6f70 7329 0d0a  ops=num_loops)..
+00000070: 2c20 636f 6c6f 726d 6170 3d4e 6f6e 652c  , colormap=None,
+00000080: 2064 6973 706c 6179 5f6d 696e 3d4e 6f6e   display_min=Non
+00000090: 652c 2064 6973 706c 6179 5f6d 6178 3d4e  e, display_max=N
+000000a0: 6f6e 652c 207a 6f6f 6d5f 6661 6374 6f72  one, zoom_factor
+000000b0: 3a66 6c6f 6174 3d31 2e30 293a 0d0a 2020  :float=1.0):..  
+000000c0: 2020 2222 220d 0a20 2020 2043 7265 6174    """..    Creat
+000000d0: 6520 616e 2061 6e69 6d61 7465 6420 4749  e an animated GI
+000000e0: 4620 6672 6f6d 2061 206c 6973 7420 6f66  F from a list of
+000000f0: 2032 4420 696d 6167 6573 2061 6e64 2072   2D images and r
+00000100: 6574 7572 6e20 6974 2061 7320 4d61 726b  eturn it as Mark
+00000110: 646f 776e 206f 626a 6563 742c 2074 6861  down object, tha
+00000120: 7420 6361 6e20 6265 2073 686f 776e 2069  t can be shown i
+00000130: 6e20 4a75 7079 7465 7220 6e6f 7465 626f  n Jupyter notebo
+00000140: 6f6b 732e 0d0a 2020 2020 5247 4220 696d  oks...    RGB im
+00000150: 6167 6573 2061 7265 2073 7570 706f 7274  ages are support
+00000160: 6564 2061 7320 7765 6c6c 2c20 6275 7420  ed as well, but 
+00000170: 6e6f 2033 4420 696d 6167 6520 7374 6163  no 3D image stac
+00000180: 6b73 2e0d 0a0d 0a20 2020 204e 6f74 653a  ks.....    Note:
+00000190: 2049 7420 6973 2072 6563 6f6d 6d65 6e64   It is recommend
+000001a0: 6564 2074 6f20 6e6f 726d 616c 697a 6520  ed to normalize 
+000001b0: 7468 6520 7469 6d65 6c61 7073 6520 746f  the timelapse to
+000001c0: 2062 6520 696e 7465 6765 7273 2069 6e20   be integers in 
+000001d0: 7468 6520 7261 6e67 6520 6265 7477 6565  the range betwee
+000001e0: 6e20 3020 746f 2032 3535 2e0d 0a0d 0a20  n 0 to 255..... 
+000001f0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+00000200: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+00000210: 2020 2074 696d 656c 6170 7365 3a20 6e70     timelapse: np
+00000220: 2e6e 6461 7272 6179 0d0a 2020 2020 2020  .ndarray..      
+00000230: 2020 3244 2069 6d61 6765 206f 7220 3344    2D image or 3D
+00000240: 2069 6d61 6765 2073 7461 636b 0d0a 2020   image stack..  
+00000250: 2020 6669 6c65 6e61 6d65 3a20 7374 722c    filename: str,
+00000260: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00000270: 2020 204e 616d 6520 6f66 2074 6865 2066     Name of the f
+00000280: 696c 6520 7768 6572 6520 7468 6520 616e  ile where the an
+00000290: 696d 6174 696f 6e20 7769 6c6c 2062 6520  imation will be 
+000002a0: 7361 7665 640d 0a20 2020 206f 7665 7277  saved..    overw
+000002b0: 7269 7465 5f66 696c 653a 2062 6f6f 6c2c  rite_file: bool,
+000002c0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+000002d0: 2020 204f 7665 7277 7269 7465 2074 6865     Overwrite the
+000002e0: 2066 696c 6520 6966 2069 7420 616c 7265   file if it alre
+000002f0: 6164 7920 6578 6973 7473 2e20 4465 6661  ady exists. Defa
+00000300: 756c 743a 2054 7275 650d 0a20 2020 2066  ult: True..    f
+00000310: 7261 6d65 5f64 656c 6179 5f6d 733a 2069  rame_delay_ms: i
+00000320: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
+00000330: 2020 2020 2020 4465 6c61 7920 6265 7477        Delay betw
+00000340: 6565 6e20 6672 616d 6573 2069 6e20 6d69  een frames in mi
+00000350: 6c6c 6973 6563 6f6e 6473 0d0a 2020 2020  lliseconds..    
+00000360: 6e75 6d5f 6c6f 6f70 733a 2069 6e74 2c20  num_loops: int, 
+00000370: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00000380: 2020 4e75 6d62 6572 206f 6620 6c6f 6f70    Number of loop
+00000390: 7320 696e 2074 6865 2061 6e69 6d61 7469  s in the animati
+000003a0: 6f6e 0d0a 2020 2020 7a6f 6f6d 5f66 6163  on..    zoom_fac
+000003b0: 746f 723a 2066 6c6f 6174 2c20 6f70 7469  tor: float, opti
+000003c0: 6f6e 616c 0d0a 2020 2020 2020 2020 416c  onal..        Al
+000003d0: 6c6f 7773 2073 686f 7769 6e67 2074 6865  lows showing the
+000003e0: 2069 6d61 6765 206c 6172 6765 7220 283e   image larger (>
+000003f0: 2031 2920 6f72 2073 6d61 6c6c 6572 2028   1) or smaller (
+00000400: 3c31 290d 0a20 2020 2063 6f6c 6f72 6d61  <1)..    colorma
+00000410: 703a 2073 7472 2c20 6f70 7469 6f6e 616c  p: str, optional
+00000420: 0d0a 2020 2020 2020 2020 4d61 7470 6c6f  ..        Matplo
+00000430: 746c 6962 2063 6f6c 6f72 6d61 7020 6e61  tlib colormap na
+00000440: 6d65 206f 7220 2270 7572 655f 6772 6565  me or "pure_gree
+00000450: 6e22 2c20 2270 7572 655f 6d61 6765 6e74  n", "pure_magent
+00000460: 6122 2c20 2e2e 2e0d 0a20 2020 2064 6973  a", .....    dis
+00000470: 706c 6179 5f6d 696e 3a20 666c 6f61 742c  play_min: float,
+00000480: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00000490: 2020 204c 6f77 6572 2062 6f75 6e64 206f     Lower bound o
+000004a0: 6620 7072 6f70 6572 6c79 2073 686f 776e  f properly shown
+000004b0: 2069 6e74 656e 7369 7469 6573 0d0a 2020   intensities..  
+000004c0: 2020 6469 7370 6c61 795f 6d61 783a 2066    display_max: f
+000004d0: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0d0a  loat, optional..
+000004e0: 2020 2020 2020 2020 5570 7065 7220 626f          Upper bo
+000004f0: 756e 6420 6f66 2070 726f 7065 726c 7920  und of properly 
+00000500: 7368 6f77 6e20 696e 7465 6e73 6974 6965  shown intensitie
+00000510: 730d 0a20 2020 2022 2222 0d0a 2020 2020  s..    """..    
+00000520: 696d 706f 7274 206f 730d 0a20 2020 2069  import os..    i
+00000530: 6d70 6f72 7420 696d 6167 6569 6f0d 0a20  mport imageio.. 
+00000540: 2020 2066 726f 6d20 4950 7974 686f 6e2e     from IPython.
+00000550: 6469 7370 6c61 7920 696d 706f 7274 2048  display import H
+00000560: 544d 4c0d 0a20 2020 2069 6d70 6f72 7420  TML..    import 
+00000570: 6e75 6d70 7920 6173 206e 700d 0a20 2020  numpy as np..   
+00000580: 2069 6d70 6f72 7420 7761 726e 696e 6773   import warnings
+00000590: 0d0a 2020 2020 6672 6f6d 2073 7461 636b  ..    from stack
+000005a0: 7669 6577 2e5f 696d 6167 655f 7769 6467  view._image_widg
+000005b0: 6574 2069 6d70 6f72 7420 5f69 6d67 5f74  et import _img_t
+000005c0: 6f5f 7267 620d 0a20 2020 2066 726f 6d20  o_rgb..    from 
+000005d0: 2e5f 7574 696c 6974 6965 7320 696d 706f  ._utilities impo
+000005e0: 7274 206e 756d 7079 5f74 6f5f 6769 665f  rt numpy_to_gif_
+000005f0: 6279 7465 7374 7265 616d 2c20 5f67 6966  bytestream, _gif
+00000600: 5f74 6f5f 6874 6d6c 0d0a 0d0a 2020 2020  _to_html....    
+00000610: 6966 2030 203c 3d20 7469 6d65 6c61 7073  if 0 <= timelaps
+00000620: 652e 6d69 6e28 2920 3c3d 2031 2061 6e64  e.min() <= 1 and
+00000630: 2030 203c 3d20 7469 6d65 6c61 7073 652e   0 <= timelapse.
+00000640: 6d61 7828 2920 3c3d 2031 3a0d 0a20 2020  max() <= 1:..   
+00000650: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+00000660: 726e 2822 5468 6520 7469 6d65 6c61 7073  rn("The timelaps
+00000670: 6520 6861 7320 6120 736d 616c 6c20 696e  e has a small in
+00000680: 7465 6e73 6974 7920 7261 6e67 6520 6265  tensity range be
+00000690: 7477 6565 6e20 3020 616e 6420 312e 2043  tween 0 and 1. C
+000006a0: 6f6e 7369 6465 7220 6e6f 726d 616c 697a  onsider normaliz
+000006b0: 696e 6720 6974 2074 6f20 7468 6520 7261  ing it to the ra
+000006c0: 6e67 6520 6265 7477 6565 6e20 3020 616e  nge between 0 an
+000006d0: 6420 3235 352e 2229 0d0a 2020 2020 6966  d 255.")..    if
+000006e0: 2074 696d 656c 6170 7365 2e6d 696e 2829   timelapse.min()
+000006f0: 203c 2030 206f 7220 7469 6d65 6c61 7073   < 0 or timelaps
+00000700: 652e 6d61 7828 2920 3e20 3235 353a 0d0a  e.max() > 255:..
+00000710: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
+00000720: 2e77 6172 6e28 2254 6865 2074 696d 656c  .warn("The timel
+00000730: 6170 7365 2068 6173 2061 6e20 696e 7465  apse has an inte
+00000740: 6e73 6974 7920 7261 6e67 6520 6578 6365  nsity range exce
+00000750: 6564 696e 6720 302e 2e32 3535 2e20 436f  eding 0..255. Co
+00000760: 6e73 6964 6572 206e 6f72 6d61 6c69 7a69  nsider normalizi
+00000770: 6e67 2069 7420 746f 2074 6865 2072 616e  ng it to the ran
+00000780: 6765 2062 6574 7765 656e 2030 2061 6e64  ge between 0 and
+00000790: 2032 3535 2e22 290d 0a0d 0a20 2020 2069   255.")....    i
+000007a0: 6d61 6765 5f72 6762 203d 206e 702e 6173  mage_rgb = np.as
+000007b0: 6172 7261 7928 5b5f 696d 675f 746f 5f72  array([_img_to_r
+000007c0: 6762 2869 2c20 636f 6c6f 726d 6170 3d63  gb(i, colormap=c
+000007d0: 6f6c 6f72 6d61 702c 2064 6973 706c 6179  olormap, display
+000007e0: 5f6d 696e 3d64 6973 706c 6179 5f6d 696e  _min=display_min
+000007f0: 2c20 6469 7370 6c61 795f 6d61 783d 6469  , display_max=di
+00000800: 7370 6c61 795f 6d61 7829 2066 6f72 2069  splay_max) for i
+00000810: 2069 6e20 7469 6d65 6c61 7073 655d 292e   in timelapse]).
+00000820: 6173 7479 7065 286e 702e 7569 6e74 3829  astype(np.uint8)
+00000830: 0d0a 0d0a 2020 2020 6966 2066 696c 656e  ....    if filen
+00000840: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+00000850: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00000860: 2066 696c 656e 616d 652e 656e 6473 7769   filename.endswi
+00000870: 7468 2822 2e67 6966 2229 3a0d 0a20 2020  th(".gif"):..   
+00000880: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
+00000890: 6520 2b3d 2022 2e67 6966 220d 0a20 2020  e += ".gif"..   
+000008a0: 2020 2020 2069 6620 6e6f 7420 6f76 6572       if not over
+000008b0: 7772 6974 655f 6669 6c65 3a0d 0a20 2020  write_file:..   
+000008c0: 2020 2020 2020 2020 2069 203d 2030 0d0a           i = 0..
+000008d0: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
+000008e0: 696e 616c 5f66 696c 656e 616d 6520 3d20  inal_filename = 
+000008f0: 6669 6c65 6e61 6d65 0d0a 2020 2020 2020  filename..      
+00000900: 2020 2020 2020 7768 696c 6520 6f73 2e70        while os.p
+00000910: 6174 682e 6578 6973 7473 2866 696c 656e  ath.exists(filen
+00000920: 616d 6529 3a0d 0a20 2020 2020 2020 2020  ame):..         
+00000930: 2020 2020 2020 2069 202b 3d20 310d 0a20         i += 1.. 
+00000940: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00000950: 696c 656e 616d 6520 3d20 6f72 6967 696e  ilename = origin
+00000960: 616c 5f66 696c 656e 616d 652e 7265 706c  al_filename.repl
+00000970: 6163 6528 222e 6769 6622 2c20 6622 5f7b  ace(".gif", f"_{
+00000980: 693a 3032 7d2e 6769 6622 290d 0a0d 0a20  i:02}.gif").... 
+00000990: 2020 2020 2020 2077 6974 6820 696d 6167         with imag
+000009a0: 6569 6f2e 6765 745f 7772 6974 6572 2866  eio.get_writer(f
+000009b0: 696c 656e 616d 652c 206d 6f64 653d 2749  ilename, mode='I
+000009c0: 272c 2064 7572 6174 696f 6e3d 6672 616d  ', duration=fram
+000009d0: 655f 6465 6c61 795f 6d73 2c20 6c6f 6f70  e_delay_ms, loop
+000009e0: 3d6e 756d 5f6c 6f6f 7073 2920 6173 2077  =num_loops) as w
+000009f0: 7269 7465 723a 0d0a 2020 2020 2020 2020  riter:..        
+00000a00: 2020 2020 666f 7220 6672 616d 6520 696e      for frame in
+00000a10: 2069 6d61 6765 5f72 6762 3a0d 0a20 2020   image_rgb:..   
+00000a20: 2020 2020 2020 2020 2020 2020 2077 7269               wri
+00000a30: 7465 722e 6170 7065 6e64 5f64 6174 6128  ter.append_data(
+00000a40: 6672 616d 6529 0d0a 0d0a 0d0a 2020 2020  frame)......    
+00000a50: 6966 206e 702e 7072 6f64 2869 6d61 6765  if np.prod(image
+00000a60: 5f72 6762 2e73 6861 7065 2920 3e20 3130  _rgb.shape) > 10
+00000a70: 3234 202a 2031 3032 3420 2a20 3130 3a0d  24 * 1024 * 10:.
+00000a80: 0a20 2020 2020 2020 2077 6172 6e69 6e67  .        warning
+00000a90: 732e 7761 726e 2822 5468 6520 696d 6167  s.warn("The imag
+00000aa0: 6520 6973 2071 7569 7465 206c 6172 6765  e is quite large
+00000ab0: 2028 3e20 3130 204d 4279 7465 2920 616e   (> 10 MByte) an
+00000ac0: 6420 6d69 6768 7420 6e6f 7420 6265 2070  d might not be p
+00000ad0: 726f 7065 726c 7920 7368 6f77 6e20 696e  roperly shown in
+00000ae0: 2074 6865 206e 6f74 6562 6f6f 6b20 7768   the notebook wh
+00000af0: 656e 2072 656e 6465 7265 6420 6f76 6572  en rendered over
+00000b00: 2074 6865 2069 6e74 6572 6e65 742e 2043   the internet. C
+00000b10: 6f6e 7369 6465 7220 7375 6273 616d 706c  onsider subsampl
+00000b20: 696e 6720 6f72 2063 726f 7070 696e 6720  ing or cropping 
+00000b30: 7468 6520 696d 6167 6520 666f 7220 7669  the image for vi
+00000b40: 7375 616c 697a 6174 696f 6e20 7075 7270  sualization purp
+00000b50: 6f73 6573 2e22 290d 0a0d 0a20 2020 2062  oses.")....    b
+00000b60: 7974 6573 7472 6561 6d20 3d20 6e75 6d70  ytestream = nump
+00000b70: 795f 746f 5f67 6966 5f62 7974 6573 7472  y_to_gif_bytestr
+00000b80: 6561 6d28 696d 6167 655f 7267 622c 2066  eam(image_rgb, f
+00000b90: 7261 6d65 5f64 656c 6179 5f6d 733d 6672  rame_delay_ms=fr
+00000ba0: 616d 655f 6465 6c61 795f 6d73 2c20 6e75  ame_delay_ms, nu
+00000bb0: 6d5f 6c6f 6f70 733d 6e75 6d5f 6c6f 6f70  m_loops=num_loop
+00000bc0: 7329 0d0a 2020 2020 7265 7475 726e 2048  s)..    return H
+00000bd0: 544d 4c28 5f67 6966 5f74 6f5f 6874 6d6c  TML(_gif_to_html
+00000be0: 2862 7974 6573 7472 6561 6d2c 2077 6964  (bytestream, wid
+00000bf0: 7468 3d69 6e74 2869 6d61 6765 5f72 6762  th=int(image_rgb
+00000c00: 2e73 6861 7065 5b2d 325d 202a 207a 6f6f  .shape[-2] * zoo
+00000c10: 6d5f 6661 6374 6f72 2929 290d 0a0d 0a64  m_factor)))....d
+00000c20: 6566 2061 6e69 6d61 7465 5f63 7572 7461  ef animate_curta
+00000c30: 696e 2874 696d 656c 6170 7365 2c20 7469  in(timelapse, ti
+00000c40: 6d65 6c61 7073 655f 6375 7274 6169 6e2c  melapse_curtain,
+00000c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000c60: 2020 2020 2020 6178 6973 3a20 696e 7420        axis: int 
+00000c70: 3d20 302c 0d0a 2020 2020 2020 2020 2020  = 0,..          
+00000c80: 2020 2020 2020 2020 2020 616c 7068 613a            alpha:
+00000c90: 2066 6c6f 6174 203d 2031 2c0d 0a20 2020   float = 1,..   
+00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cb0: 206e 756d 5f73 7465 7073 3a69 6e74 203d   num_steps:int =
+00000cc0: 2032 302c 0d0a 2020 2020 2020 2020 2020   20,..          
+00000cd0: 2020 2020 2020 2020 2020 7a6f 6f6d 5f66            zoom_f
+00000ce0: 6163 746f 723a 2066 6c6f 6174 203d 2031  actor: float = 1
+00000cf0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000d00: 2020 2020 2020 2063 6f6c 6f72 6d61 703d         colormap=
+00000d10: 4e6f 6e65 2c20 6469 7370 6c61 795f 6d69  None, display_mi
+00000d20: 6e3d 4e6f 6e65 2c20 6469 7370 6c61 795f  n=None, display_
+00000d30: 6d61 783d 4e6f 6e65 2c0d 0a20 2020 2020  max=None,..     
+00000d40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00000d50: 7572 7461 696e 5f63 6f6c 6f72 6d61 703a  urtain_colormap:
+00000d60: 7374 7220 3d20 4e6f 6e65 2c0d 0a20 2020  str = None,..   
+00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d80: 2063 7572 7461 696e 5f64 6973 706c 6179   curtain_display
+00000d90: 5f6d 696e 3a66 6c6f 6174 203d 204e 6f6e  _min:float = Non
+00000da0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00000db0: 2020 2020 2020 2020 6375 7274 6169 6e5f          curtain_
+00000dc0: 6469 7370 6c61 795f 6d61 783a 666c 6f61  display_max:floa
+00000dd0: 7420 3d20 4e6f 6e65 2c0d 0a20 2020 2020  t = None,..     
+00000de0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00000df0: 696c 656e 616d 653a 7374 723d 4e6f 6e65  ilename:str=None
+00000e00: 2c20 6f76 6572 7772 6974 655f 6669 6c65  , overwrite_file
+00000e10: 3a62 6f6f 6c3d 4661 6c73 652c 2066 7261  :bool=False, fra
+00000e20: 6d65 5f64 656c 6179 5f6d 733a 696e 743d  me_delay_ms:int=
+00000e30: 3135 302c 206e 756d 5f6c 6f6f 7073 3a69  150, num_loops:i
+00000e40: 6e74 3d31 3030 3029 3a0d 0a20 2020 2022  nt=1000):..    "
+00000e50: 2222 0d0a 2020 2020 5265 6e64 6572 2061  ""..    Render a
+00000e60: 2063 7572 7461 696e 2073 686f 7769 6e67   curtain showing
+00000e70: 2074 776f 2032 4420 696d 6167 6573 2e20   two 2D images. 
+00000e80: 5247 4220 696d 6167 6573 2061 7265 2073  RGB images are s
+00000e90: 7570 706f 7274 6564 2061 7320 7765 6c6c  upported as well
+00000ea0: 2c20 6275 7420 6e6f 2033 4420 696d 6167  , but no 3D imag
+00000eb0: 6520 7374 6163 6b73 2e0d 0a0d 0a20 2020  e stacks.....   
+00000ec0: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+00000ed0: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
+00000ee0: 2074 696d 656c 6170 7365 3a20 6e70 2e6e   timelapse: np.n
+00000ef0: 6461 7272 6179 0d0a 2020 2020 2020 2020  darray..        
+00000f00: 3244 2069 6d61 6765 206f 7220 3344 2069  2D image or 3D i
+00000f10: 6d61 6765 2073 7461 636b 0d0a 2020 2020  mage stack..    
+00000f20: 7469 6d65 6c61 7073 655f 6375 7274 6169  timelapse_curtai
+00000f30: 6e3a 206e 702e 6e64 6172 7261 790d 0a20  n: np.ndarray.. 
+00000f40: 2020 2020 2020 2032 4420 696d 6167 6520         2D image 
+00000f50: 6f72 2033 4420 696d 6167 6520 7374 6163  or 3D image stac
+00000f60: 6b0d 0a20 2020 2061 7869 733a 2069 6e74  k..    axis: int
+00000f70: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00000f80: 2020 2020 4178 6973 2069 6e20 6361 7365      Axis in case
+00000f90: 2077 6520 6172 6520 736c 6963 696e 6720   we are slicing 
+00000fa0: 6120 7374 6163 6b0d 0a20 2020 2061 6c70  a stack..    alp
+00000fb0: 6861 3a20 666c 6f61 742c 206f 7074 696f  ha: float, optio
+00000fc0: 6e61 6c0d 0a20 2020 2020 2020 2073 6574  nal..        set
+00000fd0: 7320 7468 6520 7472 616e 7370 6172 656e  s the transparen
+00000fe0: 6379 206f 6620 7468 6520 6375 7274 6169  cy of the curtai
+00000ff0: 6e0d 0a20 2020 206e 756d 5f73 7465 7073  n..    num_steps
+00001000: 3a20 696e 742c 206f 7074 696f 6e61 6c0d  : int, optional.
+00001010: 0a20 2020 2020 2020 206e 756d 6265 7220  .        number 
+00001020: 6f66 2073 7465 7073 2069 6e20 7468 6520  of steps in the 
+00001030: 616e 696d 6174 696f 6e2c 2068 616c 6620  animation, half 
+00001040: 6f66 2074 6865 6d20 7468 6520 6375 7274  of them the curt
+00001050: 6169 6e20 7769 6c6c 2067 6f20 6c65 6674  ain will go left
+00001060: 2d72 6967 6874 2c20 7468 6520 6f74 6865  -right, the othe
+00001070: 7220 6861 6c66 2072 6967 6874 2d6c 6566  r half right-lef
+00001080: 740d 0a20 2020 207a 6f6f 6d5f 6661 6374  t..    zoom_fact
+00001090: 6f72 3a20 666c 6f61 742c 206f 7074 696f  or: float, optio
+000010a0: 6e61 6c0d 0a20 2020 2020 2020 2041 6c6c  nal..        All
+000010b0: 6f77 7320 7368 6f77 696e 6720 7468 6520  ows showing the 
+000010c0: 696d 6167 6520 6c61 7267 6572 2028 3e20  image larger (> 
+000010d0: 3129 206f 7220 736d 616c 6c65 7220 283c  1) or smaller (<
+000010e0: 3129 0d0a 2020 2020 636f 6c6f 726d 6170  1)..    colormap
+000010f0: 3a20 7374 722c 206f 7074 696f 6e61 6c0d  : str, optional.
+00001100: 0a20 2020 2020 2020 204d 6174 706c 6f74  .        Matplot
+00001110: 6c69 6220 636f 6c6f 726d 6170 206e 616d  lib colormap nam
+00001120: 6520 6f72 2022 7075 7265 5f67 7265 656e  e or "pure_green
+00001130: 222c 2022 7075 7265 5f6d 6167 656e 7461  ", "pure_magenta
+00001140: 222c 202e 2e2e 0d0a 2020 2020 6469 7370  ", .....    disp
+00001150: 6c61 795f 6d69 6e3a 2066 6c6f 6174 2c20  lay_min: float, 
+00001160: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00001170: 2020 4c6f 7765 7220 626f 756e 6420 6f66    Lower bound of
+00001180: 2070 726f 7065 726c 7920 7368 6f77 6e20   properly shown 
+00001190: 696e 7465 6e73 6974 6965 730d 0a20 2020  intensities..   
+000011a0: 2064 6973 706c 6179 5f6d 6178 3a20 666c   display_max: fl
+000011b0: 6f61 742c 206f 7074 696f 6e61 6c0d 0a20  oat, optional.. 
+000011c0: 2020 2020 2020 2055 7070 6572 2062 6f75         Upper bou
+000011d0: 6e64 206f 6620 7072 6f70 6572 6c79 2073  nd of properly s
+000011e0: 686f 776e 2069 6e74 656e 7369 7469 6573  hown intensities
+000011f0: 0d0a 2020 2020 6375 7274 6169 6e5f 636f  ..    curtain_co
+00001200: 6c6f 726d 6170 3a20 7374 722c 206f 7074  lormap: str, opt
+00001210: 696f 6e61 6c0d 0a20 2020 2020 2020 204d  ional..        M
+00001220: 6174 706c 6f74 6c69 6220 636f 6c6f 726d  atplotlib colorm
+00001230: 6170 206e 616d 6520 6f72 2022 7075 7265  ap name or "pure
+00001240: 5f67 7265 656e 222c 2022 7075 7265 5f6d  _green", "pure_m
+00001250: 6167 656e 7461 222c 202e 2e2e 0d0a 2020  agenta", .....  
+00001260: 2020 6375 7274 6169 6e5f 6469 7370 6c61    curtain_displa
+00001270: 795f 6d69 6e3a 2066 6c6f 6174 2c20 6f70  y_min: float, op
+00001280: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00001290: 4c6f 7765 7220 626f 756e 6420 6f66 2070  Lower bound of p
+000012a0: 726f 7065 726c 7920 7368 6f77 6e20 696e  roperly shown in
+000012b0: 7465 6e73 6974 6965 730d 0a20 2020 2063  tensities..    c
+000012c0: 7572 7461 696e 5f64 6973 706c 6179 5f6d  urtain_display_m
+000012d0: 6178 3a20 666c 6f61 742c 206f 7074 696f  ax: float, optio
+000012e0: 6e61 6c0d 0a20 2020 2020 2020 2055 7070  nal..        Upp
+000012f0: 6572 2062 6f75 6e64 206f 6620 7072 6f70  er bound of prop
+00001300: 6572 6c79 2073 686f 776e 2069 6e74 656e  erly shown inten
+00001310: 7369 7469 6573 0d0a 2020 2020 6669 6c65  sities..    file
+00001320: 6e61 6d65 3a20 7374 722c 206f 7074 696f  name: str, optio
+00001330: 6e61 6c0d 0a20 2020 2020 2020 204e 616d  nal..        Nam
+00001340: 6520 6f66 2074 6865 2066 696c 6520 7768  e of the file wh
+00001350: 6572 6520 7468 6520 616e 696d 6174 696f  ere the animatio
+00001360: 6e20 7769 6c6c 2062 6520 7361 7665 640d  n will be saved.
+00001370: 0a20 2020 206f 7665 7277 7269 7465 5f66  .    overwrite_f
+00001380: 696c 653a 2062 6f6f 6c2c 206f 7074 696f  ile: bool, optio
+00001390: 6e61 6c0d 0a20 2020 2020 2020 204f 7665  nal..        Ove
+000013a0: 7277 7269 7465 2074 6865 2066 696c 6520  rwrite the file 
+000013b0: 6966 2069 7420 616c 7265 6164 7920 6578  if it already ex
+000013c0: 6973 7473 0d0a 2020 2020 6672 616d 655f  ists..    frame_
+000013d0: 6465 6c61 795f 6d73 3a20 696e 742c 206f  delay_ms: int, o
+000013e0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+000013f0: 2044 656c 6179 2062 6574 7765 656e 2066   Delay between f
+00001400: 7261 6d65 7320 696e 206d 696c 6c69 7365  rames in millise
+00001410: 636f 6e64 730d 0a20 2020 206e 756d 5f6c  conds..    num_l
+00001420: 6f6f 7073 3a20 696e 742c 206f 7074 696f  oops: int, optio
+00001430: 6e61 6c0d 0a20 2020 2020 2020 204e 756d  nal..        Num
+00001440: 6265 7220 6f66 206c 6f6f 7073 2069 6e20  ber of loops in 
+00001450: 7468 6520 616e 696d 6174 696f 6e0d 0a0d  the animation...
+00001460: 0a20 2020 2022 2222 0d0a 2020 2020 696d  .    """..    im
+00001470: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
+00001480: 0d0a 2020 2020 6672 6f6d 202e 5f69 6d61  ..    from ._ima
+00001490: 6765 5f77 6964 6765 7420 696d 706f 7274  ge_widget import
+000014a0: 205f 696d 675f 746f 5f72 6762 0d0a 0d0a   _img_to_rgb....
+000014b0: 2020 2020 6d61 785f 7369 7a65 203d 2074      max_size = t
+000014c0: 696d 656c 6170 7365 2e73 6861 7065 5b31  imelapse.shape[1
+000014d0: 5d0d 0a0d 0a20 2020 2069 6d61 6765 7320  ]....    images 
+000014e0: 3d20 5b5d 0d0a 2020 2020 7374 6570 7320  = []..    steps 
+000014f0: 3d20 6c69 7374 2872 616e 6765 2830 2c20  = list(range(0, 
+00001500: 6d61 785f 7369 7a65 202b 2031 2c20 696e  max_size + 1, in
+00001510: 7428 6d61 785f 7369 7a65 202f 206e 756d  t(max_size / num
+00001520: 5f73 7465 7073 202a 2032 2929 290d 0a20  _steps * 2))).. 
+00001530: 2020 2073 7465 7073 203d 2073 7465 7073     steps = steps
+00001540: 202b 2073 7465 7073 5b3a 3a2d 315d 0d0a   + steps[::-1]..
+00001550: 0d0a 2020 2020 666f 7220 736c 6964 6572  ..    for slider
+00001560: 5f76 616c 7565 2069 6e20 7374 6570 733a  _value in steps:
+00001570: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+00001580: 2874 696d 656c 6170 7365 2e73 6861 7065  (timelapse.shape
+00001590: 2920 3c20 3320 6f72 2028 6c65 6e28 7469  ) < 3 or (len(ti
+000015a0: 6d65 6c61 7073 652e 7368 6170 6529 203d  melapse.shape) =
+000015b0: 3d20 3320 616e 6420 7469 6d65 6c61 7073  = 3 and timelaps
+000015c0: 652e 7368 6170 655b 2d31 5d20 3d3d 2033  e.shape[-1] == 3
+000015d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000015e0: 696d 6167 655f 736c 6963 6520 3d20 5f69  image_slice = _i
+000015f0: 6d67 5f74 6f5f 7267 6228 7469 6d65 6c61  mg_to_rgb(timela
+00001600: 7073 652e 636f 7079 2829 2c20 636f 6c6f  pse.copy(), colo
+00001610: 726d 6170 3d63 6f6c 6f72 6d61 702c 2064  rmap=colormap, d
+00001620: 6973 706c 6179 5f6d 696e 3d64 6973 706c  isplay_min=displ
+00001630: 6179 5f6d 696e 2c20 6469 7370 6c61 795f  ay_min, display_
+00001640: 6d61 783d 6469 7370 6c61 795f 6d61 7829  max=display_max)
+00001650: 0d0a 2020 2020 2020 2020 2020 2020 696d  ..            im
+00001660: 6167 655f 736c 6963 655f 6375 7274 6169  age_slice_curtai
+00001670: 6e20 3d20 5f69 6d67 5f74 6f5f 7267 6228  n = _img_to_rgb(
+00001680: 7469 6d65 6c61 7073 655f 6375 7274 6169  timelapse_curtai
+00001690: 6e2c 2063 6f6c 6f72 6d61 703d 6375 7274  n, colormap=curt
+000016a0: 6169 6e5f 636f 6c6f 726d 6170 2c20 6469  ain_colormap, di
+000016b0: 7370 6c61 795f 6d69 6e3d 6375 7274 6169  splay_min=curtai
+000016c0: 6e5f 6469 7370 6c61 795f 6d69 6e2c 0d0a  n_display_min,..
+000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016f0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00001700: 7370 6c61 795f 6d61 783d 6375 7274 6169  splay_max=curtai
+00001710: 6e5f 6469 7370 6c61 795f 6d61 7829 0d0a  n_display_max)..
+00001720: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00001730: 2020 2020 2020 2020 2020 2069 6d61 6765             image
+00001740: 5f73 6c69 6365 203d 205f 696d 675f 746f  _slice = _img_to
+00001750: 5f72 6762 286e 702e 7461 6b65 2874 696d  _rgb(np.take(tim
+00001760: 656c 6170 7365 2c20 736c 6964 6572 5f76  elapse, slider_v
+00001770: 616c 7565 2c20 6178 6973 3d61 7869 7329  alue, axis=axis)
+00001780: 2c20 636f 6c6f 726d 6170 3d63 6f6c 6f72  , colormap=color
+00001790: 6d61 702c 0d0a 2020 2020 2020 2020 2020  map,..          
+000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017b0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+000017c0: 6c61 795f 6d69 6e3d 6469 7370 6c61 795f  lay_min=display_
+000017d0: 6d69 6e2c 2064 6973 706c 6179 5f6d 6178  min, display_max
+000017e0: 3d64 6973 706c 6179 5f6d 6178 290d 0a20  =display_max).. 
+000017f0: 2020 2020 2020 2020 2020 2069 6d61 6765             image
+00001800: 5f73 6c69 6365 5f63 7572 7461 696e 203d  _slice_curtain =
+00001810: 205f 696d 675f 746f 5f72 6762 286e 702e   _img_to_rgb(np.
+00001820: 7461 6b65 2874 696d 656c 6170 7365 5f63  take(timelapse_c
+00001830: 7572 7461 696e 2c20 736c 6964 6572 5f76  urtain, slider_v
+00001840: 616c 7565 2c20 6178 6973 3d61 7869 7329  alue, axis=axis)
+00001850: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001880: 2063 6f6c 6f72 6d61 703d 6375 7274 6169   colormap=curtai
+00001890: 6e5f 636f 6c6f 726d 6170 2c20 6469 7370  n_colormap, disp
+000018a0: 6c61 795f 6d69 6e3d 6375 7274 6169 6e5f  lay_min=curtain_
+000018b0: 6469 7370 6c61 795f 6d69 6e2c 0d0a 2020  display_min,..  
+000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018e0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+000018f0: 6c61 795f 6d61 783d 6375 7274 6169 6e5f  lay_max=curtain_
+00001900: 6469 7370 6c61 795f 6d61 7829 0d0a 2020  display_max)..  
+00001910: 2020 2020 2020 696d 6167 655f 736c 6963        image_slic
+00001920: 655b 3a2c 2073 6c69 6465 725f 7661 6c75  e[:, slider_valu
+00001930: 653a 5d20 3d20 2831 202d 2061 6c70 6861  e:] = (1 - alpha
+00001940: 2920 2a20 696d 6167 655f 736c 6963 655b  ) * image_slice[
+00001950: 3a2c 2073 6c69 6465 725f 7661 6c75 653a  :, slider_value:
+00001960: 5d20 2b20 5c0d 0a20 2020 2020 2020 2020  ] + \..         
+00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001990: 2020 2020 2020 2061 6c70 6861 202a 2069         alpha * i
+000019a0: 6d61 6765 5f73 6c69 6365 5f63 7572 7461  mage_slice_curta
+000019b0: 696e 5b3a 2c20 736c 6964 6572 5f76 616c  in[:, slider_val
+000019c0: 7565 3a5d 0d0a 0d0a 2020 2020 2020 2020  ue:]....        
+000019d0: 696d 6167 6573 2e61 7070 656e 6428 696d  images.append(im
+000019e0: 6167 655f 736c 6963 6529 0d0a 0d0a 2020  age_slice)....  
+000019f0: 2020 7265 7475 726e 2061 6e69 6d61 7465    return animate
+00001a00: 286e 702e 6173 6172 7261 7928 696d 6167  (np.asarray(imag
+00001a10: 6573 292c 2066 696c 656e 616d 653d 6669  es), filename=fi
+00001a20: 6c65 6e61 6d65 2c20 6f76 6572 7772 6974  lename, overwrit
+00001a30: 655f 6669 6c65 3d6f 7665 7277 7269 7465  e_file=overwrite
+00001a40: 5f66 696c 652c 2066 7261 6d65 5f64 656c  _file, frame_del
+00001a50: 6179 5f6d 733d 6672 616d 655f 6465 6c61  ay_ms=frame_dela
+00001a60: 795f 6d73 2c20 6e75 6d5f 6c6f 6f70 733d  y_ms, num_loops=
+00001a70: 6e75 6d5f 6c6f 6f70 732c 207a 6f6f 6d5f  num_loops, zoom_
+00001a80: 6661 6374 6f72 3d7a 6f6f 6d5f 6661 6374  factor=zoom_fact
+00001a90: 6f72 290d 0a                             or)..
```

### Comparing `stackview-0.7.8/stackview/_annotate.py` & `stackview-0.7.9/stackview/_annotate.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_assist.py` & `stackview-0.7.9/stackview/_assist.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_bia_bob_plugins.py` & `stackview-0.7.9/stackview/_bia_bob_plugins.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_colormaps.py` & `stackview-0.7.9/stackview/_colormaps.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_context.py` & `stackview-0.7.9/stackview/_context.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_crop.py` & `stackview-0.7.9/stackview/_crop.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_curtain.py` & `stackview-0.7.9/stackview/_curtain.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_image_widget.py` & `stackview-0.7.9/stackview/_image_widget.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_imshow.py` & `stackview-0.7.9/stackview/_imshow.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_interact.py` & `stackview-0.7.9/stackview/_interact.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_orthogonal.py` & `stackview-0.7.9/stackview/_orthogonal.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_picker.py` & `stackview-0.7.9/stackview/_picker.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_side_by_side.py` & `stackview-0.7.9/stackview/_side_by_side.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_slice.py` & `stackview-0.7.9/stackview/_slice.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_slice_viewer.py` & `stackview-0.7.9/stackview/_slice_viewer.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_static_view.py` & `stackview-0.7.9/stackview/_static_view.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_switch.py` & `stackview-0.7.9/stackview/_switch.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview/_uint_field.py` & `stackview-0.7.9/stackview/_uint_field.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.8/stackview.egg-info/PKG-INFO` & `stackview-0.7.9/stackview.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.7.8
+Version: 0.7.9
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@uni-leipzig.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -119,22 +119,22 @@
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/imshow.png)
 
 
 ### Static animations
 
 The `animate` and `animate_curtain` functions can be used to store animations of image stacks / images blended over each other as gif to disk.
 
-Â´Â´Â´
-stackview.animate(blobs_images, filename="images/timelapse2.gif", frame_delay_ms=50)
-Â´Â´Â´
+```python
+stackview.animate(blobs_images, frame_delay_ms=50)
+```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse2.gif)
 
 ```python
-stackview.animate_curtain(blobs, blobs > 128, filename="images/timelapse3.gif")
+stackview.animate_curtain(blobs, blobs > 128)
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/timelapse3.gif)
 
 ### Annotate regions
 
 To create label images interactively, e.g. for machine learning training, the `stackview.annotate` function offers basic label drawing tools. 
@@ -152,58 +152,58 @@
 
 Note: In case the interface is slow, consider using smaller images, e.g. by cropping or resampling.
 
 ### Pick intensities
 
 To read the intensity of pixels where the mouse is moving, use the picker.
 ```python
-stackview.picker(image, continuous_update=True)
+stackview.picker(image)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_picker.gif)
 
 ### Orthogonal view
 
 Orthogonal views are also available:
 ```python
-stackview.orthogonal(image, continuous_update=True)
+stackview.orthogonal(image)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_orthogonal.gif)
 
 ### Curtain
 
 Furthermore, to visualize an original image in combination with a processed version, a curtain view may be helpful:
 ```python
-stackview.curtain(image, modified_image * 65537, continuous_update=True)
+stackview.curtain(image, modified_image * 65537)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_curtain.gif)
 
 The curtain also works with 2D data. 
 Btw. to visualize both images properly, you need adjust their grey value range yourself. 
 For example, multiply a binary image with 255 so that it visualizes nicely side-by-side with the original image in 8-bit range:
 ```python
 binary = (slice_image > threshold_otsu(slice_image)) * 255
-stackview.curtain(slice_image, binary, continuous_update=True)
+stackview.curtain(slice_image, binary)
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_curtain2.gif)
 
 The same also works with label images
 ```python
 from skimage.measure import label
 labels = label(binary)
-stackview.curtain(slice_image, labels, continuous_update=True)
+stackview.curtain(slice_image, labels)
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_curtain3.gif)
 
 ### Side-by-side view
 
 A side-by-side view for colocalization visualization is also available.
 If you're working with time-lapse data, you can also use this view for visualizing differences between timepoints:
 ```python
-stackview.side_by_side(image_stack[1:], image_stack[:-1], continuous_update=True, display_width=300)
+stackview.side_by_side(image_stack[1:], image_stack[:-1])
 ```
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_side_by_side.gif)
 
 ### Switch
 
 The `switch` function allows to switch between a list or dictionary of images.
 
@@ -238,15 +238,15 @@
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_switch_toggleable.gif)
 
 
 ### Crop
 
 You can crop images interactively:
 ```python
-crop_widget = stackview.crop(image_stack, continuous_update=True)
+crop_widget = stackview.crop(image_stack)
 crop_widget
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/crop.gif)
 
 ... and retrieve the crop range as a tuple of `slice` objects:
 ```python
@@ -296,15 +296,15 @@
 
 If you want to use a pulldown for selecting input image(s), you need to pass a dictionary of `(name, image)` pairs as `context`, e.g. `context=globals()`:
 
 ```python
 image1 = imread("data/Haase_MRT_tfl3d1.tif")
 image2 = image1[:,:,::-1]
 
-stackview.interact(gaussian, context=globals(), continuous_update=True)
+stackview.interact(gaussian, context=globals())
 ```
 
 ![](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_interact4.gif)
 
 To add an `insight`-view automatically to results of functions, you can add this.
 
 ```python
@@ -317,18 +317,18 @@
 
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/jupyter_displayable_output.png)
 
 ### Assist
 
 The `stackview.assist()` function can guide you through all imported (and supported) image processing functions.
 Note: The interface may be slow or crash if you have many functions imported. Consider using it in an empty notebook 
-with only functions or library imported that might be relevant for the taks.
+with only functions or library imported that might be relevant for the tasks.
 
 ```python
-stackview.assist(context=globals(), continuous_update=True)
+stackview.assist(context=globals())
 ```
 
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/demo_assist.gif)
 
 ## Voila
 
 If you combine stackview with [voila](https://voila.readthedocs.io/en/stable/), you can build powerful, interactive, browser-based image processing apps and demonstrators. Just build a graphical user interface in a Jupyter notebook and then start it using
```

### Comparing `stackview-0.7.8/stackview.egg-info/SOURCES.txt` & `stackview-0.7.9/stackview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

