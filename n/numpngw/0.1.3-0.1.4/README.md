# Comparing `tmp/numpngw-0.1.3.tar.gz` & `tmp/numpngw-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpngw-0.1.3.tar", last modified: Sat Oct  7 17:31:41 2023, max compression
+gzip compressed data, was "numpngw-0.1.4.tar", last modified: Sun Jun  2 19:05:14 2024, max compression
```

## Comparing `numpngw-0.1.3.tar` & `numpngw-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 17:31:41.812492 numpngw-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-10-07 17:31:30.000000 numpngw-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14500 2023-10-07 17:31:41.812492 numpngw-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2023-10-07 17:31:30.000000 numpngw-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 17:31:41.808492 numpngw-0.1.3/numpngw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14500 2023-10-07 17:31:41.000000 numpngw-0.1.3/numpngw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-10-07 17:31:41.000000 numpngw-0.1.3/numpngw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-07 17:31:41.000000 numpngw-0.1.3/numpngw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-07 17:31:41.000000 numpngw-0.1.3/numpngw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-07 17:31:41.000000 numpngw-0.1.3/numpngw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    60414 2023-10-07 17:31:30.000000 numpngw-0.1.3/numpngw.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-07 17:31:41.812492 numpngw-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-10-07 17:31:30.000000 numpngw-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 17:31:41.808492 numpngw-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2023-10-07 17:31:30.000000 numpngw-0.1.3/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    47878 2023-10-07 17:31:30.000000 numpngw-0.1.3/tests/test_write_png.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:05:14.526325 numpngw-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-06-02 19:05:05.000000 numpngw-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-06-02 19:05:14.526325 numpngw-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-06-02 19:05:05.000000 numpngw-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:05:14.526325 numpngw-0.1.4/numpngw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-06-02 19:05:14.000000 numpngw-0.1.4/numpngw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-06-02 19:05:14.000000 numpngw-0.1.4/numpngw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:05:14.000000 numpngw-0.1.4/numpngw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-02 19:05:14.000000 numpngw-0.1.4/numpngw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 19:05:14.000000 numpngw-0.1.4/numpngw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    60307 2024-06-02 19:05:05.000000 numpngw-0.1.4/numpngw.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 19:05:14.526325 numpngw-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-06-02 19:05:05.000000 numpngw-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:05:14.526325 numpngw-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-06-02 19:05:05.000000 numpngw-0.1.4/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48104 2024-06-02 19:05:05.000000 numpngw-0.1.4/tests/test_write_png.py
```

### Comparing `numpngw-0.1.3/LICENSE.txt` & `numpngw-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numpngw-0.1.3/PKG-INFO` & `numpngw-0.1.4/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: numpngw
-Version: 0.1.3
-Summary: Write numpy array(s) to a PNG or animated PNG file.
-Home-page: https://github.com/WarrenWeckesser/numpngw
-Author: Warren Weckesser
-License: BSD
-Keywords: numpy png matplotlib animation
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-License-File: LICENSE.txt
-Requires-Dist: numpy>=1.6.0
-
 numpngw
 =======
 
 This python package (availabe on PyPI at https://pypi.org/project/numpngw/)
 defines the function ``write_png`` that writes a numpy array to a PNG file,
 and the function ``write_apng`` that writes a sequence of arrays to an
 animated PNG (APNG) file.  Also included is the class ``AnimatedPNGWriter``
@@ -65,15 +39,15 @@
 support animated PNG; see https://caniuse.com/apng for support status.
 
 Example 1
 ---------
 
 The following script creates this PNG file, an 8-bit RGB image.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example1.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example1.png
    :alt: Example 1
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -97,15 +71,15 @@
 
 
 Example 2
 ---------
 
 The following script creates this PNG file, a 1-bit grayscale image.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example2.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example2.png
    :alt: Example 2
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -128,15 +102,15 @@
 Example 3
 ---------
 
 The following script creates this PNG file, a 16-bit RGB file in which
 the value (0, 0, 0) is transparent.  It might not be obvious, but the
 two squares are transparent.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example3.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example3.png
    :alt: Example 3
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -147,16 +121,16 @@
 
     # Create some interesting data.
     w = 32
     nrows = 3*w
     ncols = 5*w
     kernel = np.exp(-np.linspace(-2, 2, 35)**2)
     kernel = kernel/kernel.sum()
-    np.random.seed(123)
-    x = np.random.randn(nrows, ncols, 3)
+    rng = np.random.default_rng(seed=121263137472525314065)
+    x = rng.standard_normal((nrows, ncols, 3))
     x = np.apply_along_axis(lambda z: np.convolve(z, kernel, mode='same'), 0, x)
     x = np.apply_along_axis(lambda z: np.convolve(z, kernel, mode='same'), 1, x)
 
     # Convert to 16 bit unsigned integers.
     z = (65535*((x - x.min())/x.ptp())).astype(np.uint16)
 
     # Create two squares containing (0, 0, 0).
@@ -169,15 +143,15 @@
 
 Example 4
 ---------
 
 The following script uses the option ``use_palette=True`` to create this 8-bit
 indexed RGB file.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example4.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example4.png
    :alt: Example 4
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -187,32 +161,32 @@
     #
     # Create an 8-bit indexed RGB image that uses a palette.
 
     img_width = 300
     img_height = 200
     img = np.zeros((img_height, img_width, 3), dtype=np.uint8)
 
-    np.random.seed(222)
+    rng = np.random.default_rng(seed=121263137472525314065)
     for _ in range(40):
-        width = np.random.randint(5, img_width // 5)
-        height = np.random.randint(5, img_height // 5)
-        row = np.random.randint(5, img_height - height - 5)
-        col = np.random.randint(5, img_width - width - 5)
-        color = np.random.randint(80, 256, size=2)
+        width = rng.integers(5, img_width // 5)
+        height = rng.integers(5, img_height // 5)
+        row = rng.integers(5, img_height - height - 5)
+        col = rng.integers(5, img_width - width - 5)
+        color = rng.integers(80, 256, size=2)
         img[row:row+height, col:col+width, 1:] = color
 
     write_png('example4.png', img, use_palette=True)
 
 
 Example 5
 ---------
 
 This animated PNG
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example5.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example5.png
    :alt: Example 5
    :align: center
 
 is created by the following script.  As in the other examples, most of the
 script is code that generates the data to be saved.  The line that creates
 the PNG file is simply::
 
@@ -244,15 +218,15 @@
 Example 6
 ---------
 
 Another animated RGB PNG. In this example, the argument ``seq``
 that is passed to ``write_apng`` is a numpy array with shape
 ``(num_frames, height, width, 3)``.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example6.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example6.png
    :alt: Example 6
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_apng
@@ -270,30 +244,30 @@
         fkernel = np.fft.fftn(kernel, w.shape)
         v = np.fft.ifftn(fw*fkernel).real
         return v
 
     height = 40
     width = 250
     num_frames = 30
-    np.random.seed(12345)
-    w = np.random.randn(num_frames, height, width, 3)
+    rng = np.random.default_rng(seed=121263137472525314065)
+    w = rng.standard_normal((num_frames, height, width, 3))
     for k in range(3):
         w[..., k] = smoother(w[..., k])
 
     seq = (255*(w - w.min())/w.ptp()).astype(np.uint8)
 
     write_apng("example6.png", seq, delay=40)
 
 
 Example 7
 ---------
 
 Create an animated PNG with different display times for each frame.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example7.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example7.png
    :alt: Example 7
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_apng
@@ -417,15 +391,15 @@
 Example 8
 ---------
 
 This example shows how a Matplotlib animation can be saved as
 an animated PNG file with `numpngw.AnimatedPNGWriter`.  (Be careful
 with this class--it can easily create very large PNG files.)
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example8.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example8.png
    :alt: Example 8
    :align: center
 
 The script::
 
     import numpy as np
     from scipy.integrate import odeint
```

### Comparing `numpngw-0.1.3/README.rst` & `numpngw-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: numpngw
+Version: 0.1.4
+Summary: Write numpy array(s) to a PNG or animated PNG file.
+Home-page: https://github.com/WarrenWeckesser/numpngw
+Author: Warren Weckesser
+License: BSD
+Keywords: numpy png matplotlib animation
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+License-File: LICENSE.txt
+Requires-Dist: numpy>=1.6.0
+
 numpngw
 =======
 
 This python package (availabe on PyPI at https://pypi.org/project/numpngw/)
 defines the function ``write_png`` that writes a numpy array to a PNG file,
 and the function ``write_apng`` that writes a sequence of arrays to an
 animated PNG (APNG) file.  Also included is the class ``AnimatedPNGWriter``
@@ -39,15 +60,15 @@
 support animated PNG; see https://caniuse.com/apng for support status.
 
 Example 1
 ---------
 
 The following script creates this PNG file, an 8-bit RGB image.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example1.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example1.png
    :alt: Example 1
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -71,15 +92,15 @@
 
 
 Example 2
 ---------
 
 The following script creates this PNG file, a 1-bit grayscale image.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example2.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example2.png
    :alt: Example 2
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -102,15 +123,15 @@
 Example 3
 ---------
 
 The following script creates this PNG file, a 16-bit RGB file in which
 the value (0, 0, 0) is transparent.  It might not be obvious, but the
 two squares are transparent.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example3.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example3.png
    :alt: Example 3
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -121,16 +142,16 @@
 
     # Create some interesting data.
     w = 32
     nrows = 3*w
     ncols = 5*w
     kernel = np.exp(-np.linspace(-2, 2, 35)**2)
     kernel = kernel/kernel.sum()
-    np.random.seed(123)
-    x = np.random.randn(nrows, ncols, 3)
+    rng = np.random.default_rng(seed=121263137472525314065)
+    x = rng.standard_normal((nrows, ncols, 3))
     x = np.apply_along_axis(lambda z: np.convolve(z, kernel, mode='same'), 0, x)
     x = np.apply_along_axis(lambda z: np.convolve(z, kernel, mode='same'), 1, x)
 
     # Convert to 16 bit unsigned integers.
     z = (65535*((x - x.min())/x.ptp())).astype(np.uint16)
 
     # Create two squares containing (0, 0, 0).
@@ -143,15 +164,15 @@
 
 Example 4
 ---------
 
 The following script uses the option ``use_palette=True`` to create this 8-bit
 indexed RGB file.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example4.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example4.png
    :alt: Example 4
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -161,32 +182,32 @@
     #
     # Create an 8-bit indexed RGB image that uses a palette.
 
     img_width = 300
     img_height = 200
     img = np.zeros((img_height, img_width, 3), dtype=np.uint8)
 
-    np.random.seed(222)
+    rng = np.random.default_rng(seed=121263137472525314065)
     for _ in range(40):
-        width = np.random.randint(5, img_width // 5)
-        height = np.random.randint(5, img_height // 5)
-        row = np.random.randint(5, img_height - height - 5)
-        col = np.random.randint(5, img_width - width - 5)
-        color = np.random.randint(80, 256, size=2)
+        width = rng.integers(5, img_width // 5)
+        height = rng.integers(5, img_height // 5)
+        row = rng.integers(5, img_height - height - 5)
+        col = rng.integers(5, img_width - width - 5)
+        color = rng.integers(80, 256, size=2)
         img[row:row+height, col:col+width, 1:] = color
 
     write_png('example4.png', img, use_palette=True)
 
 
 Example 5
 ---------
 
 This animated PNG
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example5.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example5.png
    :alt: Example 5
    :align: center
 
 is created by the following script.  As in the other examples, most of the
 script is code that generates the data to be saved.  The line that creates
 the PNG file is simply::
 
@@ -218,15 +239,15 @@
 Example 6
 ---------
 
 Another animated RGB PNG. In this example, the argument ``seq``
 that is passed to ``write_apng`` is a numpy array with shape
 ``(num_frames, height, width, 3)``.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example6.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example6.png
    :alt: Example 6
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_apng
@@ -244,30 +265,30 @@
         fkernel = np.fft.fftn(kernel, w.shape)
         v = np.fft.ifftn(fw*fkernel).real
         return v
 
     height = 40
     width = 250
     num_frames = 30
-    np.random.seed(12345)
-    w = np.random.randn(num_frames, height, width, 3)
+    rng = np.random.default_rng(seed=121263137472525314065)
+    w = rng.standard_normal((num_frames, height, width, 3))
     for k in range(3):
         w[..., k] = smoother(w[..., k])
 
     seq = (255*(w - w.min())/w.ptp()).astype(np.uint8)
 
     write_apng("example6.png", seq, delay=40)
 
 
 Example 7
 ---------
 
 Create an animated PNG with different display times for each frame.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example7.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example7.png
    :alt: Example 7
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_apng
@@ -391,15 +412,15 @@
 Example 8
 ---------
 
 This example shows how a Matplotlib animation can be saved as
 an animated PNG file with `numpngw.AnimatedPNGWriter`.  (Be careful
 with this class--it can easily create very large PNG files.)
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example8.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example8.png
    :alt: Example 8
    :align: center
 
 The script::
 
     import numpy as np
     from scipy.integrate import odeint
```

### Comparing `numpngw-0.1.3/numpngw.egg-info/PKG-INFO` & `numpngw-0.1.4/numpngw.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: numpngw
-Version: 0.1.3
+Version: 0.1.4
 Summary: Write numpy array(s) to a PNG or animated PNG file.
 Home-page: https://github.com/WarrenWeckesser/numpngw
 Author: Warren Weckesser
 License: BSD
 Keywords: numpy png matplotlib animation
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
@@ -65,15 +60,15 @@
 support animated PNG; see https://caniuse.com/apng for support status.
 
 Example 1
 ---------
 
 The following script creates this PNG file, an 8-bit RGB image.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example1.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example1.png
    :alt: Example 1
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -97,15 +92,15 @@
 
 
 Example 2
 ---------
 
 The following script creates this PNG file, a 1-bit grayscale image.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example2.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example2.png
    :alt: Example 2
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -128,15 +123,15 @@
 Example 3
 ---------
 
 The following script creates this PNG file, a 16-bit RGB file in which
 the value (0, 0, 0) is transparent.  It might not be obvious, but the
 two squares are transparent.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example3.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example3.png
    :alt: Example 3
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -147,16 +142,16 @@
 
     # Create some interesting data.
     w = 32
     nrows = 3*w
     ncols = 5*w
     kernel = np.exp(-np.linspace(-2, 2, 35)**2)
     kernel = kernel/kernel.sum()
-    np.random.seed(123)
-    x = np.random.randn(nrows, ncols, 3)
+    rng = np.random.default_rng(seed=121263137472525314065)
+    x = rng.standard_normal((nrows, ncols, 3))
     x = np.apply_along_axis(lambda z: np.convolve(z, kernel, mode='same'), 0, x)
     x = np.apply_along_axis(lambda z: np.convolve(z, kernel, mode='same'), 1, x)
 
     # Convert to 16 bit unsigned integers.
     z = (65535*((x - x.min())/x.ptp())).astype(np.uint16)
 
     # Create two squares containing (0, 0, 0).
@@ -169,15 +164,15 @@
 
 Example 4
 ---------
 
 The following script uses the option ``use_palette=True`` to create this 8-bit
 indexed RGB file.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example4.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example4.png
    :alt: Example 4
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_png
@@ -187,32 +182,32 @@
     #
     # Create an 8-bit indexed RGB image that uses a palette.
 
     img_width = 300
     img_height = 200
     img = np.zeros((img_height, img_width, 3), dtype=np.uint8)
 
-    np.random.seed(222)
+    rng = np.random.default_rng(seed=121263137472525314065)
     for _ in range(40):
-        width = np.random.randint(5, img_width // 5)
-        height = np.random.randint(5, img_height // 5)
-        row = np.random.randint(5, img_height - height - 5)
-        col = np.random.randint(5, img_width - width - 5)
-        color = np.random.randint(80, 256, size=2)
+        width = rng.integers(5, img_width // 5)
+        height = rng.integers(5, img_height // 5)
+        row = rng.integers(5, img_height - height - 5)
+        col = rng.integers(5, img_width - width - 5)
+        color = rng.integers(80, 256, size=2)
         img[row:row+height, col:col+width, 1:] = color
 
     write_png('example4.png', img, use_palette=True)
 
 
 Example 5
 ---------
 
 This animated PNG
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example5.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example5.png
    :alt: Example 5
    :align: center
 
 is created by the following script.  As in the other examples, most of the
 script is code that generates the data to be saved.  The line that creates
 the PNG file is simply::
 
@@ -244,15 +239,15 @@
 Example 6
 ---------
 
 Another animated RGB PNG. In this example, the argument ``seq``
 that is passed to ``write_apng`` is a numpy array with shape
 ``(num_frames, height, width, 3)``.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example6.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example6.png
    :alt: Example 6
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_apng
@@ -270,30 +265,30 @@
         fkernel = np.fft.fftn(kernel, w.shape)
         v = np.fft.ifftn(fw*fkernel).real
         return v
 
     height = 40
     width = 250
     num_frames = 30
-    np.random.seed(12345)
-    w = np.random.randn(num_frames, height, width, 3)
+    rng = np.random.default_rng(seed=121263137472525314065)
+    w = rng.standard_normal((num_frames, height, width, 3))
     for k in range(3):
         w[..., k] = smoother(w[..., k])
 
     seq = (255*(w - w.min())/w.ptp()).astype(np.uint8)
 
     write_apng("example6.png", seq, delay=40)
 
 
 Example 7
 ---------
 
 Create an animated PNG with different display times for each frame.
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example7.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example7.png
    :alt: Example 7
    :align: center
 
 The script::
 
     import numpy as np
     from numpngw import write_apng
@@ -417,15 +412,15 @@
 Example 8
 ---------
 
 This example shows how a Matplotlib animation can be saved as
 an animated PNG file with `numpngw.AnimatedPNGWriter`.  (Be careful
 with this class--it can easily create very large PNG files.)
 
-.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/master/examples/example8.png
+.. image:: https://raw.githubusercontent.com/WarrenWeckesser/numpngw/main/examples/example8.png
    :alt: Example 8
    :align: center
 
 The script::
 
     import numpy as np
     from scipy.integrate import odeint
```

### Comparing `numpngw-0.1.3/numpngw.py` & `numpngw-0.1.4/numpngw.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The numpngw module defines two functions and a class:
 
 * write_png(...) writes a numpy array to a PNG file.
 * write_apng(...) writes a sequence of arrays to an animated PNG file.
 * AnimatedPNGWriter is a class that can be used with Matplotlib animations.
 
 -----
-Copyright (c) 2015-2023, Warren Weckesser
+Copyright (c) 2015-2024, Warren Weckesser
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
    this list of conditions and the following disclaimer.
@@ -28,31 +28,28 @@
 SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
 
-from __future__ import (division as _division,
-                        print_function as _print_function)
-
 import sys as _sys
 import contextlib as _contextlib
 from io import BytesIO as _BytesIO
 import time as _time
 import struct as _struct
 import zlib as _zlib
 from fractions import Fraction as _Fraction
 import operator
 import numpy as _np
 
 
 __all__ = ['write_png', 'write_apng', 'AnimatedPNGWriter']
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 _PY3 = _sys.version_info > (3,)
 if _PY3:
     def _bord(c):
         return c
 else:
     _bord = ord
```

### Comparing `numpngw-0.1.3/setup.py` & `numpngw-0.1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,20 +33,15 @@
     long_description=_long_description,
     license="BSD",
     url="https://github.com/WarrenWeckesser/numpngw",
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
```

### Comparing `numpngw-0.1.3/tests/test_utilities.py` & `numpngw-0.1.4/tests/test_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import division, print_function
 
 import unittest
 import numpy as np
 from numpy.testing import assert_equal, assert_array_equal
 import numpngw
```

### Comparing `numpngw-0.1.3/tests/test_write_png.py` & `numpngw-0.1.4/tests/test_write_png.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import division, print_function
-
 import unittest
 import io
 import struct
 import zlib
 import numpy as np
 from numpy.testing import (assert_, assert_equal, assert_array_equal,
                            assert_raises)
@@ -430,23 +428,23 @@
 
 
 class TestWritePng(unittest.TestCase):
 
     def test_write_png_nbit_grayscale(self):
         # Test the creation of grayscale images for bit depths of 1, 2, 4
         # 8 and 16, with or without a `transparent` color selected.
-        np.random.seed(123)
+        rng = np.random.default_rng(seed=121263137472525314065)
         for filter_type in [0, 1, 2, 3, 4, "heuristic", "auto"]:
             for bitdepth in [1, 2, 4, 8, 16]:
                 for transparent in [None, 0]:
                     for interlace in [0, 1]:
                         dt = np.uint16 if bitdepth == 16 else np.uint8
                         maxval = 2**bitdepth
                         sz = (3, 11)
-                        img = np.random.randint(0, maxval, size=sz).astype(dt)
+                        img = rng.integers(0, maxval, size=sz).astype(dt)
                         if transparent is not None:
                             img[2:4, 2:] = transparent
 
                         f = io.BytesIO()
                         numpngw.write_png(f, img, bitdepth=bitdepth,
                                           transparent=transparent,
                                           filter_type=filter_type,
@@ -482,24 +480,23 @@
                         check_iend(file_contents)
 
     def test_write_png_with_alpha(self):
         # Test creation of grayscale+alpha and RGBA images (color types 4
         # and 6, resp.), with bit depths 8 and 16.
         w = 25
         h = 15
-        np.random.seed(12345)
+        rng = np.random.default_rng(seed=121263137472525314065)
         for filter_type in [0, 1, 2, 3, 4, "heuristic", "auto"]:
             for color_type in [4, 6]:
                 num_channels = 2 if color_type == 4 else 4
                 for bit_depth in [8, 16]:
                     for interlace in [0, 1]:
                         dt = np.uint8 if bit_depth == 8 else np.uint16
                         sz = (h, w, num_channels)
-                        img = np.random.randint(0, 2**bit_depth,
-                                                size=sz).astype(dt)
+                        img = rng.integers(0, 2**bit_depth, size=sz).astype(dt)
                         f = io.BytesIO()
                         numpngw.write_png(f, img, filter_type=filter_type,
                                           interlace=interlace)
 
                         file_contents = f.getvalue()
 
                         file_contents = check_signature(file_contents)
@@ -525,23 +522,23 @@
                         check_iend(file_contents)
 
     def test_write_png_RGB(self):
         # Test creation of RGB images (color type 2), with and without
         # a `transparent` color selected, and with bit depth 8 and 16.
         w = 24
         h = 10
-        np.random.seed(12345)
+        rng = np.random.default_rng(seed=121263137472525314065)
         for filter_type in [0, 1, 2, 3, 4, "heuristic", "auto"]:
             for transparent in [None, (0, 0, 0)]:
                 for bit_depth in [8, 16]:
                     for interlace in [0, 1]:
                         dt = np.uint16 if bit_depth == 16 else np.uint8
                         maxval = 2**bit_depth
-                        img = np.random.randint(0, maxval,
-                                                size=(h, w, 3)).astype(dt)
+                        img = rng.integers(0, maxval,
+                                           size=(h, w, 3)).astype(dt)
                         if transparent:
                             img[2:4, 2:4] = transparent
 
                         f = io.BytesIO()
                         numpngw.write_png(f, img, transparent=transparent,
                                           filter_type=filter_type,
                                           interlace=interlace)
@@ -639,15 +636,16 @@
                     check_iend(file_contents)
 
     def test_write_png_max_chunk_len(self):
         # Create an 8-bit grayscale image.
         w = 250
         h = 150
         max_chunk_len = 500
-        img = np.random.randint(0, 256, size=(h, w)).astype(np.uint8)
+        rng = np.random.default_rng(seed=121263137472525314065)
+        img = rng.integers(0, 256, size=(h, w)).astype(np.uint8)
         f = io.BytesIO()
         numpngw.write_png(f, img, max_chunk_len=max_chunk_len)
 
         file_contents = f.getvalue()
 
         file_contents = check_signature(file_contents)
 
@@ -677,16 +675,16 @@
         # in the loop above.
         self.assertEqual(chunk_type, b"IEND")
         self.assertEqual(chunk_data, b"")
 
         self.assertEqual(file_contents, b"")
 
     def test_write_png_timestamp_gamma_chromaticity(self):
-        np.random.seed(123)
-        img = np.random.randint(0, 256, size=(10, 10)).astype(np.uint8)
+        rng = np.random.default_rng(seed=121263137472525314065)
+        img = rng.integers(0, 256, size=(10, 10)).astype(np.uint8)
         f = io.BytesIO()
         timestamp = (1452, 4, 15, 8, 9, 10)
         gamma = 2.2
         chromaticity = [[0.500, 0.750],
                         [0.125, 0.960],
                         [0.875, 0.625],
                         [0.750, 0.375]]
@@ -717,20 +715,20 @@
 
         check_iend(file_contents)
 
     def test_write_png_bkgd(self):
         # Test creation of RGB images (color type 2), with a background color.
         w = 16
         h = 8
-        np.random.seed(123)
+        rng = np.random.default_rng(seed=121263137472525314065)
         for bit_depth in [8, 16]:
             maxval = 2**bit_depth
             bg = (maxval - 1, maxval - 2, maxval - 3)
             dt = np.uint16 if bit_depth == 16 else np.uint8
-            img = np.random.randint(0, maxval, size=(h, w, 3)).astype(dt)
+            img = rng.integers(0, maxval, size=(h, w, 3)).astype(dt)
 
             f = io.BytesIO()
             numpngw.write_png(f, img, background=bg, filter_type=0)
 
             file_contents = f.getvalue()
 
             file_contents = check_signature(file_contents)
@@ -752,20 +750,20 @@
 
             check_iend(file_contents)
 
     def test_write_png_sbit(self):
         # Test creation of sBIT chunks for color_type 0 and 2.
         w = 7
         h = 5
-        np.random.seed(123)
+        rng = np.random.default_rng(seed=121263137472525314065)
         for bit_depth in [8, 16]:
             for size in [(h, w), (h, w, 3)]:
                 maxval = 2**bit_depth
                 dt = np.uint16 if bit_depth == 16 else np.uint8
-                img = np.random.randint(0, maxval, size=size).astype(dt)
+                img = rng.integers(0, maxval, size=size).astype(dt)
 
                 color_type = 0 if len(size) == 2 else 2
 
                 sbit = (bit_depth - 1,)
                 if color_type == 2:
                     sbit = sbit * 3
 
@@ -798,15 +796,14 @@
                 check_iend(file_contents)
 
     def test_write_png_bkgd_palette(self):
         # Test creation of RGB images with a background color
         # when use_palette is True.
         w = 6
         h = 8
-        np.random.seed(123)
         for bg_in_img in [True, False]:
             bit_depth = 8
             maxval = 2**bit_depth
             bg = (maxval - 1, maxval - 3, maxval - 2)
 
             img = np.arange(1, w*h*3 + 1, dtype=np.uint8).reshape(h, w, 3)
             if bg_in_img:
@@ -971,16 +968,16 @@
 
 class TestWritePngFilterType(unittest.TestCase):
 
     def test_basic(self):
         w = 22
         h = 10
         bitdepth = 8
-        np.random.seed(123)
-        img = np.random.randint(0, 256, size=(h, w)).astype(np.uint8)
+        rng = np.random.default_rng(seed=121263137472525314065)
+        img = rng.integers(0, 256, size=(h, w)).astype(np.uint8)
 
         f = io.BytesIO()
         numpngw.write_png(f, img, filter_type=1)
 
         file_contents = f.getvalue()
 
         file_contents = check_signature(file_contents)
@@ -1004,17 +1001,17 @@
 
 class TestWriteApng(unittest.TestCase):
 
     def test_write_apng_8bit_RGBA(self):
         num_frames = 4
         w = 25
         h = 15
-        np.random.seed(12345)
+        rng = np.random.default_rng(seed=121263137472525314065)
         seq_size = (num_frames, h, w, 4)
-        seq = np.random.randint(0, 256, size=seq_size).astype(np.uint8)
+        seq = rng.integers(0, 256, size=seq_size).astype(np.uint8)
         f = io.BytesIO()
         numpngw.write_apng(f, seq)
 
         file_contents = f.getvalue()
 
         file_contents = check_signature(file_contents)
 
@@ -1059,17 +1056,17 @@
 
         check_iend(file_contents)
 
     def test_default_image(self):
         num_frames = 2
         w = 16
         h = 8
-        np.random.seed(12345)
+        rng = np.random.default_rng(seed=121263137472525314065)
         seq_size = (num_frames, h, w, 4)
-        seq = np.random.randint(0, 256, size=seq_size).astype(np.uint8)
+        seq = rng.integers(0, 256, size=seq_size).astype(np.uint8)
         default_image = np.zeros((h, w, 4), dtype=np.uint8)
 
         f = io.BytesIO()
 
         numpngw.write_apng(f, seq, default_image=default_image)
 
         file_contents = f.getvalue()
@@ -1114,26 +1111,26 @@
         check_iend(file_contents)
 
     def test_write_apng_bkgd(self):
         # Test creation of RGB images (color type 2), with a background color.
         # Also test the chromaticity argument.
         w = 16
         h = 8
-        np.random.seed(123)
+        rng = np.random.default_rng(seed=121263137472525314065)
         num_frames = 3
         chromaticity = [[0.500, 0.750],
                         [0.125, 0.960],
                         [0.875, 0.625],
                         [0.750, 0.375]]
         for bit_depth in [8, 16]:
             maxval = 2**bit_depth
             bg = (maxval - 1, maxval - 2, maxval - 3)
             dt = np.uint16 if bit_depth == 16 else np.uint8
-            seq = np.random.randint(0, maxval,
-                                    size=(num_frames, h, w, 3)).astype(dt)
+            seq = rng.integers(0, maxval,
+                               size=(num_frames, h, w, 3)).astype(dt)
 
             f = io.BytesIO()
             numpngw.write_apng(f, seq, background=bg, filter_type=0,
                                chromaticity=chromaticity)
 
             file_contents = f.getvalue()
```

