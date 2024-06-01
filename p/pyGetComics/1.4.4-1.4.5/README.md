# Comparing `tmp/pygetcomics-1.4.4.tar.gz` & `tmp/pygetcomics-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygetcomics-1.4.4.tar", max compression
+gzip compressed data, was "pygetcomics-1.4.5.tar", max compression
```

## Comparing `pygetcomics-1.4.4.tar` & `pygetcomics-1.4.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1323 2017-01-14 11:37:10.942799 pygetcomics-1.4.4/LICENSE
--rw-r--r--   0        0        0       73 2018-09-02 10:16:15.940076 pygetcomics-1.4.4/README.rst
--rw-r--r--   0        0        0      638 2023-06-10 19:44:37.513034 pygetcomics-1.4.4/berhoel/__init__.py
--rw-r--r--   0        0        0     1362 2023-03-18 17:04:23.687285 pygetcomics-1.4.4/berhoel/get_comics/__init__.py
--rw-r--r--   0        0        0     1732 2023-03-19 18:35:26.907425 pygetcomics-1.4.4/berhoel/get_comics/garfield/__init__.py
--rw-r--r--   0        0        0     2430 2023-03-19 18:37:25.695432 pygetcomics-1.4.4/berhoel/get_comics/gen_pdf/__init__.py
--rw-r--r--   0        0        0     1363 2017-01-22 21:50:10.690581 pygetcomics-1.4.4/berhoel/get_comics/gen_pdf/template/book.tex
--rw-r--r--   0        0        0     8953 2023-11-04 21:18:24.260566 pygetcomics-1.4.4/berhoel/get_comics/gocomics/__init__.py
--rw-r--r--   0        0        0     3591 2022-08-09 15:38:07.250228 pygetcomics-1.4.4/berhoel/get_comics/peanuts/__init__.py
--rw-r--r--   0        0        0     1186 2022-08-09 15:01:30.240906 pygetcomics-1.4.4/berhoel/get_comics/peanuts/clean_up.py
--rw-r--r--   0        0        0     5507 2023-03-19 18:38:06.927435 pygetcomics-1.4.4/berhoel/get_comics/peanuts/gen_book.py
--rw-r--r--   0        0        0     1160 2022-08-09 15:51:27.853290 pygetcomics-1.4.4/berhoel/get_comics/tests/test_get_comics.py
--rw-r--r--   0        0        0     2474 2023-11-04 21:19:00.363876 pygetcomics-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pygetcomics-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1323 2017-01-14 11:37:10.942799 pygetcomics-1.4.5/LICENSE
+-rw-r--r--   0        0        0       73 2018-09-02 10:16:15.940076 pygetcomics-1.4.5/README.rst
+-rw-r--r--   0        0        0      638 2023-06-10 19:44:37.513034 pygetcomics-1.4.5/berhoel/__init__.py
+-rw-r--r--   0        0        0     1362 2023-03-18 17:04:23.687285 pygetcomics-1.4.5/berhoel/get_comics/__init__.py
+-rw-r--r--   0        0        0     1732 2023-03-19 18:35:26.907425 pygetcomics-1.4.5/berhoel/get_comics/garfield/__init__.py
+-rw-r--r--   0        0        0     2430 2023-03-19 18:37:25.695432 pygetcomics-1.4.5/berhoel/get_comics/gen_pdf/__init__.py
+-rw-r--r--   0        0        0     1363 2017-01-22 21:50:10.690581 pygetcomics-1.4.5/berhoel/get_comics/gen_pdf/template/book.tex
+-rw-r--r--   0        0        0     8635 2024-05-01 18:53:09.835701 pygetcomics-1.4.5/berhoel/get_comics/gocomics/__init__.py
+-rw-r--r--   0        0        0     3591 2022-08-09 15:38:07.250228 pygetcomics-1.4.5/berhoel/get_comics/peanuts/__init__.py
+-rw-r--r--   0        0        0     1186 2022-08-09 15:01:30.240906 pygetcomics-1.4.5/berhoel/get_comics/peanuts/clean_up.py
+-rw-r--r--   0        0        0     5507 2023-03-19 18:38:06.927435 pygetcomics-1.4.5/berhoel/get_comics/peanuts/gen_book.py
+-rw-r--r--   0        0        0     1160 2022-08-09 15:51:27.853290 pygetcomics-1.4.5/berhoel/get_comics/tests/test_get_comics.py
+-rw-r--r--   0        0        0     2474 2024-05-01 18:40:18.105734 pygetcomics-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 pygetcomics-1.4.5/PKG-INFO
```

### Comparing `pygetcomics-1.4.4/LICENSE` & `pygetcomics-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.4/berhoel/__init__.py` & `pygetcomics-1.4.5/berhoel/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.4/berhoel/get_comics/__init__.py` & `pygetcomics-1.4.5/berhoel/get_comics/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.4/berhoel/get_comics/garfield/__init__.py` & `pygetcomics-1.4.5/berhoel/get_comics/garfield/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.4/berhoel/get_comics/gen_pdf/__init__.py` & `pygetcomics-1.4.5/berhoel/get_comics/gen_pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.4/berhoel/get_comics/gen_pdf/template/book.tex` & `pygetcomics-1.4.5/berhoel/get_comics/gen_pdf/template/book.tex`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.4/berhoel/get_comics/gocomics/__init__.py` & `pygetcomics-1.4.5/berhoel/get_comics/gocomics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 from pathlib import Path
 
 # Third party library imports.
 from selenium import webdriver
 from lxml.html import fromstring
 from selenium.webdriver.common import action_chains
 from selenium.webdriver.common.keys import Keys
-
-# from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.firefox.options import Options
 from selenium.webdriver.firefox.firefox_profile import FirefoxProfile
 
 __date__ = "2023/06/20 21:57:10 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2011-2017 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
@@ -44,29 +42,25 @@
 class SeleniumSingleton:
     __instance = None
 
     def __init__(self):
         """Virtually private constructor."""
         self.driver = None
         if SeleniumSingleton.__instance is None:
-            # https://stackoverflow.com/questions/46920243/how-to-configure-chromedriver-to-initiate-chrome-browser-in-headless-mode-thr<oug
             options = Options()
             options.add_argument("--headless")
-            # options.binary_location = "/usr/bin/google-chrome-stable"
             if os.name == "nt":
                 options.add_argument(
                     "--disable-gpu"
                 )  # Last I checked this was necessary.
                 options.add_argument("--headless")
             firefox_profile = FirefoxProfile()
             firefox_profile.set_preference("javascript.enabled", True)
             options.profile = firefox_profile
             self.driver = webdriver.Firefox(options=options)
-
-            # self.driver = webdriver.Chrome(options)
             self.driver.get("http://www.gocomics.com/")
             if self.driver.current_url.startswith("https://login.microsoftonline.com/"):
                 self.ms_login()
             SeleniumSingleton.__instance = self
         else:
             raise Exception("This class is a singleton!")
 
@@ -234,15 +228,15 @@
 
                     mk_dir_tree(png_path.parent)
 
                     res = request.urlretrieve(data, gif_path)
                     if res[1].get_content_type() == "text/html" and data != data_norm:
                         request.urlretrieve(data_norm, gif_path)
 
-                process = subprocess.Popen(f"convert {gif_path} {png_path}", shell=True)
+                process = subprocess.Popen(f"convert {gif_path} -strip {png_path}", shell=True)
                 os.waitpid(process.pid, 0)
 
                 gif_path.unlink()
                 png_path.chmod(FILE_MODE)
 
                 sys.stdout.write(f"\r                    \r{png_path}\n")
```

### Comparing `pygetcomics-1.4.4/berhoel/get_comics/peanuts/__init__.py` & `pygetcomics-1.4.5/berhoel/get_comics/peanuts/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.4/berhoel/get_comics/peanuts/clean_up.py` & `pygetcomics-1.4.5/berhoel/get_comics/peanuts/clean_up.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.4/berhoel/get_comics/peanuts/gen_book.py` & `pygetcomics-1.4.5/berhoel/get_comics/peanuts/gen_book.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.4/berhoel/get_comics/tests/test_get_comics.py` & `pygetcomics-1.4.5/berhoel/get_comics/tests/test_get_comics.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.4.4/pyproject.toml` & `pygetcomics-1.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyGetComics"
-version = "1.4.4"
+version = "1.4.5"
 
 description = "Download various daily comics."
 
 packages = [{ include = "berhoel" }]
 
 authors = ["Berthold Höllmann <berhoel@gmail.com>"]
 license = "BSD-2-Clause"
```

### Comparing `pygetcomics-1.4.4/PKG-INFO` & `pygetcomics-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGetComics
-Version: 1.4.4
+Version: 1.4.5
 Summary: Download various daily comics.
 Home-page: https://gitlab.com/berhoel/python/pyGetComics.git
 License: BSD-2-Clause
 Author: Berthold Höllmann
 Author-email: berhoel@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

