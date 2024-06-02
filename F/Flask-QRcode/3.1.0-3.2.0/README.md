# Comparing `tmp/Flask-QRcode-3.1.0.tar.gz` & `tmp/flask_qrcode-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-QRcode-3.1.0.tar", last modified: Tue Jun 28 21:19:00 2022, max compression
+gzip compressed data, was "flask_qrcode-3.2.0.tar", last modified: Sun Jun  2 14:51:55 2024, max compression
```

## Comparing `Flask-QRcode-3.1.0.tar` & `flask_qrcode-3.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-06-28 21:19:00.397455 Flask-QRcode-3.1.0/
--rw-rw-rw-   0        0        0    35821 2022-06-28 21:16:13.000000 Flask-QRcode-3.1.0/COPYING
-drwxrwxrwx   0        0        0        0 2022-06-28 21:19:00.372453 Flask-QRcode-3.1.0/Flask_QRcode.egg-info/
--rw-rw-rw-   0        0        0     3261 2022-06-28 21:18:59.000000 Flask-QRcode-3.1.0/Flask_QRcode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2022-06-28 21:19:00.000000 Flask-QRcode-3.1.0/Flask_QRcode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-28 21:18:59.000000 Flask-QRcode-3.1.0/Flask_QRcode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-28 21:18:57.000000 Flask-QRcode-3.1.0/Flask_QRcode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2022-06-28 21:19:00.000000 Flask-QRcode-3.1.0/Flask_QRcode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-06-28 21:19:00.000000 Flask-QRcode-3.1.0/Flask_QRcode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       19 2022-06-28 21:16:13.000000 Flask-QRcode-3.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3261 2022-06-28 21:19:00.398456 Flask-QRcode-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1908 2022-06-28 21:16:13.000000 Flask-QRcode-3.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-06-28 21:19:00.377455 Flask-QRcode-3.1.0/flask_qrcode/
--rw-rw-rw-   0        0        0     7349 2022-06-28 21:16:13.000000 Flask-QRcode-3.1.0/flask_qrcode/__init__.py
--rw-rw-rw-   0        0        0       86 2022-06-28 21:19:00.401460 Flask-QRcode-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2781 2022-06-28 21:16:13.000000 Flask-QRcode-3.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-28 21:19:00.392455 Flask-QRcode-3.1.0/tests/
--rw-rw-rw-   0        0        0        0 2022-06-28 21:16:13.000000 Flask-QRcode-3.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1121 2022-06-28 21:16:13.000000 Flask-QRcode-3.1.0/tests/server.py
--rw-rw-rw-   0        0        0    79224 2022-06-28 21:16:13.000000 Flask-QRcode-3.1.0/tests/test_functional.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:51:55.856812 flask_qrcode-3.2.0/
+-rw-rw-rw-   0        0        0    35821 2022-06-28 15:46:32.000000 flask_qrcode-3.2.0/COPYING
+drwxrwxrwx   0        0        0        0 2024-06-02 14:51:55.853815 flask_qrcode-3.2.0/Flask_QRcode.egg-info/
+-rw-rw-rw-   0        0        0     3433 2024-06-02 14:51:55.000000 flask_qrcode-3.2.0/Flask_QRcode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-06-02 14:51:55.000000 flask_qrcode-3.2.0/Flask_QRcode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 14:51:55.000000 flask_qrcode-3.2.0/Flask_QRcode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-04-18 18:43:49.000000 flask_qrcode-3.2.0/Flask_QRcode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2024-06-02 14:51:55.000000 flask_qrcode-3.2.0/Flask_QRcode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-06-02 14:51:55.000000 flask_qrcode-3.2.0/Flask_QRcode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       19 2022-06-28 15:46:32.000000 flask_qrcode-3.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3433 2024-06-02 14:51:55.855816 flask_qrcode-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1908 2022-06-28 15:46:32.000000 flask_qrcode-3.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 14:51:55.845552 flask_qrcode-3.2.0/flask_qrcode/
+-rw-rw-rw-   0        0        0     7358 2024-06-02 13:57:30.000000 flask_qrcode-3.2.0/flask_qrcode/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-06-02 14:51:55.858032 flask_qrcode-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2883 2024-06-02 14:26:07.000000 flask_qrcode-3.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 14:51:55.850833 flask_qrcode-3.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-06-28 15:46:32.000000 flask_qrcode-3.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1100 2024-06-02 13:58:40.000000 flask_qrcode-3.2.0/tests/server.py
+-rw-rw-rw-   0        0        0    79224 2024-06-02 14:30:06.000000 flask_qrcode-3.2.0/tests/test_functional.py
```

### Comparing `Flask-QRcode-3.1.0/COPYING` & `flask_qrcode-3.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `Flask-QRcode-3.1.0/Flask_QRcode.egg-info/PKG-INFO` & `flask_qrcode-3.2.0/Flask_QRcode.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-QRcode
-Version: 3.1.0
+Version: 3.2.0
 Summary: A concise Flask extension to render QR codes on Jinja2 templates using python-qrcode
 Home-page: https://github.com/marcoagner/Flask-QRcode
 Author: Marco Agner
 Author-email: marco@agner.io
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -20,18 +20,23 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: COPYING
+Requires-Dist: Flask
+Requires-Dist: qrcode
+Requires-Dist: pillow
 
 Flask-QRcode
 ============
 [![PyPI version](https://badge.fury.io/py/Flask-QRcode.svg)](https://badge.fury.io/py/Flask-QRcode)
 
 > A concise Flask extension to easily render QR codes on Jinja2 templates using
 [python-qrcode](https://github.com/lincolnloop/python-qrcode)
```

### Comparing `Flask-QRcode-3.1.0/PKG-INFO` & `flask_qrcode-3.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-QRcode
-Version: 3.1.0
+Version: 3.2.0
 Summary: A concise Flask extension to render QR codes on Jinja2 templates using python-qrcode
 Home-page: https://github.com/marcoagner/Flask-QRcode
 Author: Marco Agner
 Author-email: marco@agner.io
 License: GPLv3
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -20,18 +20,23 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: COPYING
+Requires-Dist: Flask
+Requires-Dist: qrcode
+Requires-Dist: pillow
 
 Flask-QRcode
 ============
 [![PyPI version](https://badge.fury.io/py/Flask-QRcode.svg)](https://badge.fury.io/py/Flask-QRcode)
 
 > A concise Flask extension to easily render QR codes on Jinja2 templates using
 [python-qrcode](https://github.com/lincolnloop/python-qrcode)
```

### Comparing `Flask-QRcode-3.1.0/README.md` & `flask_qrcode-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `Flask-QRcode-3.1.0/flask_qrcode/__init__.py` & `flask_qrcode-3.2.0/flask_qrcode/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             icon = Image.open(icon_fp)
         except:
             return qr_img
 
         icon_w, icon_h = icon.size
         icon_w = size_w if icon_w > size_w else icon_w
         icon_h = size_h if icon_h > size_h else icon_h
-        icon = icon.resize((int(icon_w), int(icon_h)), Image.ANTIALIAS)
+        icon = icon.resize((int(icon_w), int(icon_h)), Image.Resampling.LANCZOS)
         icon = icon.convert("RGBA")
 
         left = int((img_w - icon_w) / 2)
         top = int((img_h - icon_h) / 2)
         icon_box = (int(icon_box[0]), int(icon_box[1])) if icon_box else (left, top)
         qr_img.paste(im=icon, box=icon_box, mask=icon)
         return qr_img
```

### Comparing `Flask-QRcode-3.1.0/setup.py` & `flask_qrcode-3.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         err_code = pytest.main(self.test_args)
         sys.exit(err_code)
 
 
 setup(
     name="Flask-QRcode",
-    version="3.1.0",
+    version="3.2.0",
     license="GPLv3",
     description="A concise Flask extension to render QR codes on Jinja2 "
     "templates using python-qrcode",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Marco Agner",
     author_email="marco@agner.io",
@@ -67,12 +67,14 @@
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     packages=find_packages(),
 )
```

### Comparing `Flask-QRcode-3.1.0/tests/server.py` & `flask_qrcode-3.2.0/tests/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,10 +26,9 @@
 class TestServer(socketserver.TCPServer):
     allow_reuse_address = True
 
 
 def start_test_server(port=5000):
     handler = http.server.SimpleHTTPRequestHandler
     httpd = TestServer(("", port), handler)
-    httpd_thread = threading.Thread(target=httpd.serve_forever)
-    httpd_thread.setDaemon(True)
+    httpd_thread = threading.Thread(target=httpd.serve_forever, daemon=True)
     httpd_thread.start()
```

### Comparing `Flask-QRcode-3.1.0/tests/test_functional.py` & `flask_qrcode-3.2.0/tests/test_functional.py`

 * *Files identical despite different names*

