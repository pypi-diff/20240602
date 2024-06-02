# Comparing `tmp/pyimgproxy-0.1.tar.gz` & `tmp/pyimgproxy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimgproxy-0.1.tar", last modified: Mon Mar 25 21:05:56 2024, max compression
+gzip compressed data, was "pyimgproxy-0.2.tar", last modified: Sun Jun  2 20:47:47 2024, max compression
```

## Comparing `pyimgproxy-0.1.tar` & `pyimgproxy-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:05:56.717609 pyimgproxy-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-25 21:05:36.000000 pyimgproxy-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-25 21:05:36.000000 pyimgproxy-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-25 21:05:56.717609 pyimgproxy-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-25 21:05:36.000000 pyimgproxy-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:05:56.717609 pyimgproxy-0.1/pyimgproxy/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-25 21:05:36.000000 pyimgproxy-0.1/pyimgproxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-25 21:05:36.000000 pyimgproxy-0.1/pyimgproxy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25366 2024-03-25 21:05:36.000000 pyimgproxy-0.1/pyimgproxy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-25 21:05:36.000000 pyimgproxy-0.1/pyimgproxy/imgproxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:05:56.717609 pyimgproxy-0.1/pyimgproxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-25 21:05:56.000000 pyimgproxy-0.1/pyimgproxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-25 21:05:56.000000 pyimgproxy-0.1/pyimgproxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 21:05:56.000000 pyimgproxy-0.1/pyimgproxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-25 21:05:56.000000 pyimgproxy-0.1/pyimgproxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-25 21:05:36.000000 pyimgproxy-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 21:05:56.717609 pyimgproxy-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:47:47.654707 pyimgproxy-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-06-02 20:47:32.000000 pyimgproxy-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-02 20:47:32.000000 pyimgproxy-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-02 20:47:47.654707 pyimgproxy-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-06-02 20:47:32.000000 pyimgproxy-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:47:47.650707 pyimgproxy-0.2/pyimgproxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 20:47:32.000000 pyimgproxy-0.2/pyimgproxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-02 20:47:32.000000 pyimgproxy-0.2/pyimgproxy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25576 2024-06-02 20:47:32.000000 pyimgproxy-0.2/pyimgproxy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-06-02 20:47:32.000000 pyimgproxy-0.2/pyimgproxy/imgproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 20:47:47.650707 pyimgproxy-0.2/pyimgproxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-02 20:47:47.000000 pyimgproxy-0.2/pyimgproxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-06-02 20:47:47.000000 pyimgproxy-0.2/pyimgproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 20:47:47.000000 pyimgproxy-0.2/pyimgproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-02 20:47:47.000000 pyimgproxy-0.2/pyimgproxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-06-02 20:47:32.000000 pyimgproxy-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 20:47:47.654707 pyimgproxy-0.2/setup.cfg
```

### Comparing `pyimgproxy-0.1/LICENSE` & `pyimgproxy-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimgproxy-0.1/PKG-INFO` & `pyimgproxy-0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimgproxy
-Version: 0.1
+Version: 0.2
 Summary: Python client for imgproxy
 Maintainer-email: The Developer Society <studio@dev.ngo>
 Project-URL: Homepage, https://github.com/developersociety/pyimgproxy
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `pyimgproxy-0.1/pyimgproxy/image.py` & `pyimgproxy-0.2/pyimgproxy/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,22 @@
         """
         Updates the source URL used for imgproxy to fetch.
         """
         new_image = Image(imgproxy=self.imgproxy, source_url=source_url)
         new_image.options = self.options.copy()
         return new_image
 
-    def _add_option(self, *args: Any) -> "Image":
-        option_list = list(args)
+    def add_option(self, option_name: str, *args: Any) -> "Image":
+        """
+        Add an image processing option, returning a new Image.
+
+        This method is used internally by all other image processing methods, but can also be used
+        to add options directly.
+        """
+        option_list = [option_name, *args]
         # Remove any trailing None values
         while option_list and option_list[-1] is None:
             option_list.pop()
         # Replace remaining None values with empty strings, and convert all other values to strings
         option_string = [str(x) if x is not None else "" for x in option_list]
         new_option = ":".join(option_string)
         new_options_list = [*self.options, new_option]
@@ -52,15 +58,15 @@
         x_offset: Optional[Union[int, float]] = None,
         y_offset: Optional[Union[int, float]] = None,
     ) -> "Image":
         """
         This is a meta-option that defines the resizing type, width, height, enlarge, and extend.
         All arguments are optional and can be omitted to use their default values.
         """
-        return self._add_option(
+        return self.add_option(
             "resize",
             resizing_type,
             width,
             height,
             enlarge,
             extend,
             gravity_type,
@@ -78,15 +84,15 @@
         x_offset: Optional[Union[int, float]] = None,
         y_offset: Optional[Union[int, float]] = None,
     ) -> "Image":
         """
         This is a meta-option that defines the width, height, enlarge, and extend. All arguments
         are optional and can be omitted to use their default values.
         """
-        return self._add_option(
+        return self.add_option(
             "size", width, height, enlarge, extend, gravity_type, x_offset, y_offset
         )
 
     def resizing_type(self, resizing_type: str) -> "Image":
         """
         Defines how imgproxy will resize the source image. Supported resizing types are:
 
@@ -97,101 +103,101 @@
           size, imgproxy will crop the result to keep the requested aspect ratio.
         - `force`: resizes the image without keeping the aspect ratio.
         - `auto`: if both source and resulting dimensions have the same orientation (portrait or
           landscape), imgproxy will use `fill`. Otherwise, it will use `fit`.
 
         Default: `fit`
         """
-        return self._add_option("resizing_type", resizing_type)
+        return self.add_option("resizing_type", resizing_type)
 
     def resizing_algorithm(self, resizing_algorithm: str) -> "Image":
         """
         Defines the algorithm that imgproxy will use for resizing. Supported algorithms are
         `nearest`, `linear`, `cubic`, `lanczos2`, and `lanczos3`.
 
         Default: `lanczos3`
         """
-        return self._add_option("resizing_algorithm", resizing_algorithm)
+        return self.add_option("resizing_algorithm", resizing_algorithm)
 
     def width(self, width: int) -> "Image":
         """
         Defines the width of the resulting image. When set to `0`, imgproxy will calculate width
         using the defined height and source aspect ratio. When set to `0` and resizing type is
         `force`, imgproxy will keep the original width.
 
         Default: `0`
         """
-        return self._add_option("width", width)
+        return self.add_option("width", width)
 
     def height(self, height: int) -> "Image":
         """
         Defines the height of the resulting image. When set to `0`, imgproxy will calculate
         resulting height using the defined width and source aspect ratio. When set to `0` and
         resizing type is `force`, imgproxy will keep the original height.
 
         Default: `0`
         """
-        return self._add_option("height", height)
+        return self.add_option("height", height)
 
     def min_width(self, width: int) -> "Image":
         """
         Defines the minimum width of the resulting image.
 
         When both `width` and `min-width` are set, the final image will be cropped according to
         `width`, so use this combination with care.
 
         Default: `0`
         """
-        return self._add_option("min-width", width)
+        return self.add_option("min-width", width)
 
     def min_height(self, height: int) -> "Image":
         """
         Defines the minimum height of the resulting image.
 
         When both `height` and `min-height` are set, the final image will be cropped according to
         `height`, so use this combination with care.
 
         Default: `0`
         """
-        return self._add_option("min-height", height)
+        return self.add_option("min-height", height)
 
     def zoom(self, x: Union[int, float], y: Optional[Union[int, float]] = None) -> "Image":
         """
         When set, imgproxy will multiply the image dimensions according to these factors. The
         values must be greater than 0.
 
         Can be combined with `width` and `height` options. In this case, imgproxy calculates scale
         factors for the provided size and then multiplies it with the provided zoom factors.
 
         Unlike the `dpr` option, the `zoom` option doesn't affect gravities offsets, watermark
         offsets, and paddings.
 
         Default: `1`
         """
-        return self._add_option("zoom", x, y)
+        return self.add_option("zoom", x, y)
 
     def dpr(self, dpr: Union[int, float]) -> "Image":
         """
         When set, imgproxy will multiply the image dimensions according to this factor for HiDPI
         (Retina) devices. The value must be greater than 0.
 
         The `dpr` option affects gravities offsets, watermark offsets, and paddings to make the
         resulting image structures with and without the `dpr` option applied match.
 
         Default: `1`
         """
-        return self._add_option("dpr", dpr)
+        return self.add_option("dpr", dpr)
 
     def enlarge(self, enlarge: bool = False) -> "Image":
         """
         When set to `True`, imgproxy will enlarge the image if it is smaller than the given size.
 
         Default: `False`
         """
-        return self._add_option("enlarge", enlarge)
+        return self.add_option("enlarge", enlarge)
 
     def extend(
         self,
         extend: Optional[bool] = None,
         gravity_type: Optional[str] = None,
         x_offset: Optional[Union[int, float]] = None,
         y_offset: Optional[Union[int, float]] = None,
@@ -200,15 +206,15 @@
         - When extend is set to `True`, imgproxy will extend the image if it is smaller than the
           given size.
         - `gravity_type` (optional) accepts the same values as the gravity option, except `sm`.
           When `gravity` is not set, imgproxy will use `ce` gravity without offsets.
 
         Default: `false:ce:0:0`
         """
-        return self._add_option("extend", extend, gravity_type, x_offset, y_offset)
+        return self.add_option("extend", extend, gravity_type, x_offset, y_offset)
 
     def extend_aspect_ratio(
         self,
         extend: Optional[bool] = None,
         gravity_type: Optional[str] = None,
         x_offset: Optional[Union[int, float]] = None,
         y_offset: Optional[Union[int, float]] = None,
@@ -217,15 +223,15 @@
         - When extend is set to `True`, imgproxy will extend the image to the requested aspect
           ratio.
         - `gravity_type` (optional) accepts the same values as the gravity option, except `sm`.
           When `gravity_type` is not set, imgproxy will use `ce` gravity without offsets.
 
         Default: `false:ce:0:0`
         """
-        return self._add_option("extend_aspect_ratio", extend, gravity_type, x_offset, y_offset)
+        return self.add_option("extend_aspect_ratio", extend, gravity_type, x_offset, y_offset)
 
     def gravity(
         self,
         gravity_type: Optional[str] = None,
         x_offset: Optional[Union[int, float]] = None,
         y_offset: Optional[Union[int, float]] = None,
     ) -> "Image":
@@ -246,15 +252,15 @@
             - When `x_offset` or `y_offset` is greater than or equal to `1`, imgproxy treats it as
               an absolute value.
             - When `x_offset` or `y_offset` is less than `1`, imgproxy treats it as a relative
               value.
 
         Default: `ce:0:0`
         """
-        return self._add_option("gravity", gravity_type, x_offset, y_offset)
+        return self.add_option("gravity", gravity_type, x_offset, y_offset)
 
     def crop(
         self,
         width: Optional[Union[int, float]] = None,
         height: Optional[Union[int, float]] = None,
         gravity_type: Optional[str] = None,
         x_offset: Optional[Union[int, float]] = None,
@@ -268,15 +274,15 @@
               absolute value.
             - When `width` or `height` is less than `1`, imgproxy treats it as a relative value.
             - When `width` or `height` is set to `0`, imgproxy will use the full width/height of
               the source image.
         - `gravity_type` (optional) accepts the same values as the gravity option. When
           `gravity_type` is not set, imgproxy will use the value of the gravity option.
         """
-        return self._add_option("crop", width, height, gravity_type, x_offset, y_offset)
+        return self.add_option("crop", width, height, gravity_type, x_offset, y_offset)
 
     def trim(
         self,
         threshold: Optional[Union[int, float]] = None,
         color: Optional[str] = None,
         equal_hor: Optional[bool] = None,
         equal_ver: Optional[bool] = None,
@@ -288,15 +294,15 @@
         - `color` - (optional) a hex-coded value of the color that needs to be cut off.
         - `equal_hor` - (optional) set to `True`, imgproxy will cut only equal parts from left and
           right sides. That means that if 10px of background can be cut off from the left and 5px
           from the right, then 5px will be cut off from both sides. For example, this can be useful
           if objects on your images are centered but have non-symmetrical shadow.
         - `equal_ver` - (optional) acts like `equal_hor` but for top/bottom sides.
         """
-        return self._add_option("trim", threshold, color, equal_hor, equal_ver)
+        return self.add_option("trim", threshold, color, equal_hor, equal_ver)
 
     def padding(
         self,
         top: int,
         right: Optional[int] = None,
         bottom: Optional[int] = None,
         left: Optional[int] = None,
@@ -306,36 +312,36 @@
         dimension must be set. Padded space is filled according to the background option.
 
             top - top padding (and for all other sides if they haven't been explicitly set)
             right - right padding (and left if it hasn't been explicitly set)
             bottom - bottom padding
             left - left padding
         """
-        return self._add_option("padding", top, right, bottom, left)
+        return self.add_option("padding", top, right, bottom, left)
 
     def auto_rotate(self, auto_rotate: bool) -> "Image":
         """
         When set to `True`, imgproxy will automatically rotate images based on the EXIF Orientation
         parameter (if available in the image meta data). The orientation tag will be removed from
         the image in all cases. Normally this is controlled by the IMGPROXY_AUTO_ROTATE
         configuration but this procesing option allows the configuration to be set for each
         request.
         """
-        return self._add_option("auto_rotate", auto_rotate)
+        return self.add_option("auto_rotate", auto_rotate)
 
     def rotate(self, angle: int) -> "Image":
         """
         Rotates the image on the specified angle. The orientation from the image metadata is
         applied before the rotation unless autorotation is disabled.
 
         Only `0`, `90`, `180`, `270`, etc., degree angles are supported.
 
         Default: `0`
         """
-        return self._add_option("rotate", angle)
+        return self.add_option("rotate", angle)
 
     @overload
     def background(self, *, hex_color: str) -> "Image": ...
 
     @overload
     def background(self, *, red: int, green: int, blue: int) -> "Image": ...
 
@@ -352,130 +358,130 @@
         `red`, `green`, and `blue` are the channel values of the background color (0-255).
         `hex_color` is a hex-coded value of the color. Useful when you convert an image with
         alpha-channel to JPEG.
 
         Default: disabled
         """
         if hex_color is not None:
-            return self._add_option("background", hex_color)
+            return self.add_option("background", hex_color)
 
-        return self._add_option("background", red, green, blue)
+        return self.add_option("background", red, green, blue)
 
     def background_alpha(self, alpha: Union[int, float]) -> "Image":
         """
         Adds an alpha channel to `background`. The value of `alpha` is a positive floating point
         number between `0` and `1`.
 
         Default: `1`
         """
-        return self._add_option("background_alpha", alpha)
+        return self.add_option("background_alpha", alpha)
 
     def adjust(
         self,
         brightness: Optional[int] = None,
         contrast: Optional[Union[int, float]] = None,
         saturation: Optional[Union[int, float]] = None,
     ) -> "Image":
         """
         This is a meta-option that defines the brightness, contrast, and saturation. All arguments
         are optional and can be omitted to use their default values.
         """
-        return self._add_option("adjust", brightness, contrast, saturation)
+        return self.add_option("adjust", brightness, contrast, saturation)
 
     def brightness(self, brightness: int) -> "Image":
         """
         When set, imgproxy will adjust brightness of the resulting image. `brightness` is an
         integer number ranging from `-255` to `255`.
 
         Default: `0`
         """
-        return self._add_option("brightness", brightness)
+        return self.add_option("brightness", brightness)
 
     def contrast(self, contrast: Union[int, float]) -> "Image":
         """
         When set, imgproxy will adjust the contrast of the resulting image. `contrast` is a
         positive floating point number, where a value of `1` leaves the contrast unchanged.
 
         Default: `1`
         """
-        return self._add_option("contrast", contrast)
+        return self.add_option("contrast", contrast)
 
     def saturation(self, saturation: Union[int, float]) -> "Image":
         """
         When set, imgproxy will adjust saturation of the resulting image. `saturation` is a
         positive floating-point number, where a value of `1` leaves the saturation unchanged.
 
         Default: `1`
         """
-        return self._add_option("saturation", saturation)
+        return self.add_option("saturation", saturation)
 
     def blur(self, sigma: Union[int, float]) -> "Image":
         """
         When set, imgproxy will apply a gaussian blur filter to the resulting image. The value of
         `sigma` defines the size of the mask imgproxy will use.
 
         Default: disabled
         """
-        return self._add_option("blur", sigma)
+        return self.add_option("blur", sigma)
 
     def sharpen(self, sigma: Union[int, float]) -> "Image":
         """
         When set, imgproxy will apply the sharpen filter to the resulting image. The value of
         `sigma` defines the size of the mask imgproxy will use.
 
         As an approximate guideline, use 0.5 sigma for 4 pixels/mm (display resolution), 1.0 for
         12 pixels/mm and 1.5 for 16 pixels/mm (300 dpi == 12 pixels/mm).
 
         Default: disabled
         """
-        return self._add_option("sharpen", sigma)
+        return self.add_option("sharpen", sigma)
 
     def pixelate(self, size: int) -> "Image":
         """
         When set, imgproxy will apply the pixelate filter to the resulting image. The value of
         `size` defines individual pixel size.
 
         Default: disabled
         """
-        return self._add_option("pixelate", size)
+        return self.add_option("pixelate", size)
 
     def unsharp_masking(
         self,
         mode: Optional[str] = None,
         weight: Optional[Union[int, float]] = None,
         divider: Optional[Union[int, float]] = None,
     ) -> "Image":
         """
         Allows redefining unsharp masking options. All arguments have the same meaning as Unsharp
         masking configs. All arguments are optional and can be omitted.
         """
-        return self._add_option("unsharp_masking", mode, weight, divider)
+        return self.add_option("unsharp_masking", mode, weight, divider)
 
     def blur_detections(
         self, sigma: Union[int, float], class_names: Optional[List[str]] = None
     ) -> "Image":
         """
         imgproxy detects objects of the provided classes and blurs them. If class names are
         omitted, imgproxy blurs all the detected objects.
 
         The value of `sigma` defines the size of the mask imgproxy will use.
         """
         if class_names is None:
             class_names = []
-        return self._add_option("blur_detections", sigma, *class_names)
+        return self.add_option("blur_detections", sigma, *class_names)
 
     def draw_detections(self, draw: bool, class_names: Optional[List[str]] = None) -> "Image":
         """
         When draw is set to `True`, imgproxy detects objects of the provided classes and draws
         their bounding boxes. If class names are omitted, imgproxy draws the bounding boxes of all
         the detected objects.
         """
         if class_names is None:
             class_names = []
-        return self._add_option("draw_detections", draw, *class_names)
+        return self.add_option("draw_detections", draw, *class_names)
 
     def gradient(self) -> "Image":
         raise NotImplementedError
 
     def watermark(self) -> "Image":
         raise NotImplementedError
 
@@ -532,52 +538,52 @@
 
     def format(self, extension: str) -> "Image":
         """
         Specifies the resulting image format. Alias for the extension part of the URL.
 
         Default: `jpg`
         """
-        return self._add_option("format", extension)
+        return self.add_option("format", extension)
 
     def page(self, page: int) -> "Image":
         """
         When a source image supports pagination (PDF, TIFF) or animation (GIF, WebP), this option
         allows specifying the page to use. Page numeration starts from zero.
 
         If both the source and the resulting image formats support animation, imgproxy will ignore
         this option and use all the source image pages. Use the `disable_animation` option to make
         imgproxy treat all images as not animated.
 
         Default: `0`
         """
-        return self._add_option("page", page)
+        return self.add_option("page", page)
 
     def pages(self, pages: int) -> "Image":
         """
         When a source image supports pagination (PDF, TIFF) or animation (GIF, WebP), this option
         allows specifying the number of pages to use. The pages will be stacked vertically and
         left-aligned.
 
         If both the source and the resulting image formats support animation, imgproxy will ignore
         this option and use all the source image pages. Use the `disable_animation` option to make
         imgproxy treat all images as not animated.
 
         Default: `1`
         """
-        return self._add_option("pages", pages)
+        return self.add_option("pages", pages)
 
     def disable_animation(self, disable: bool) -> "Image":
         """
         When set to `True`, imgproxy will treat all images as not animated. Use the `page` and the
         `pages` options to specify which frames imgproxy should use.
 
         Default: `False`
         """
 
-        return self._add_option("disable_animation", disable)
+        return self.add_option("disable_animation", disable)
 
     def video_thumbnail_second(self) -> "Image":
         raise NotImplementedError
 
     def video_thumbnail_keyframes(self) -> "Image":
         raise NotImplementedError
 
@@ -601,15 +607,15 @@
           and file size. Basically, the `raw` option allows streaming of any file type
         - With the `raw` option set, imgproxy won't download the whole image to the memory.
           Instead, it will stream the source image directly to the response lowering memory usage
         - The requests with the `raw` option set are not limited by the IMGPROXY_WORKERS config
 
         Default: `False`
         """
-        return self._add_option("raw", raw)
+        return self.add_option("raw", raw)
 
     def cachebuster(self) -> "Image":
         raise NotImplementedError
 
     def expires(self) -> "Image":
         raise NotImplementedError
```

### Comparing `pyimgproxy-0.1/pyimgproxy/imgproxy.py` & `pyimgproxy-0.2/pyimgproxy/imgproxy.py`

 * *Files identical despite different names*

### Comparing `pyimgproxy-0.1/pyimgproxy.egg-info/PKG-INFO` & `pyimgproxy-0.2/pyimgproxy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimgproxy
-Version: 0.1
+Version: 0.2
 Summary: Python client for imgproxy
 Maintainer-email: The Developer Society <studio@dev.ngo>
 Project-URL: Homepage, https://github.com/developersociety/pyimgproxy
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `pyimgproxy-0.1/pyproject.toml` & `pyimgproxy-0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'pyimgproxy'
-version = '0.1'
+version = '0.2'
 description = 'Python client for imgproxy'
 readme = 'README.md'
 maintainers = [{ name = 'The Developer Society', email = 'studio@dev.ngo' }]
 requires-python = '>= 3.8'
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
```

