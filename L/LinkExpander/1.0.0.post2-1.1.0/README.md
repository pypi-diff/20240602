# Comparing `tmp/linkexpander-1.0.0.post2.tar.gz` & `tmp/linkexpander-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkexpander-1.0.0.post2.tar", last modified: Fri May 17 19:47:47 2024, max compression
+gzip compressed data, was "linkexpander-1.1.0.tar", last modified: Sun Jun  2 07:13:04 2024, max compression
```

## Comparing `linkexpander-1.0.0.post2.tar` & `linkexpander-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 19:47:47.218152 linkexpander-1.0.0.post2/
-drwxrwxrwx   0        0        0        0 2024-05-17 19:47:47.209643 linkexpander-1.0.0.post2/LinkExpander/
--rw-rw-rw-   0        0        0       45 2024-05-17 19:45:28.000000 linkexpander-1.0.0.post2/LinkExpander/__init__.py
--rw-rw-rw-   0        0        0     3282 2024-05-13 03:55:41.000000 linkexpander-1.0.0.post2/LinkExpander/linktypes.py
--rw-rw-rw-   0        0        0    32636 2024-05-17 19:45:55.000000 linkexpander-1.0.0.post2/LinkExpander/main.py
-drwxrwxrwx   0        0        0        0 2024-05-17 19:47:47.216148 linkexpander-1.0.0.post2/LinkExpander.egg-info/
--rw-rw-rw-   0        0        0     2205 2024-05-17 19:47:47.000000 linkexpander-1.0.0.post2/LinkExpander.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-17 19:47:47.000000 linkexpander-1.0.0.post2/LinkExpander.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 19:47:47.000000 linkexpander-1.0.0.post2/LinkExpander.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-17 19:47:47.000000 linkexpander-1.0.0.post2/LinkExpander.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2205 2024-05-17 19:47:47.217149 linkexpander-1.0.0.post2/PKG-INFO
--rw-rw-rw-   0        0        0     1630 2024-05-16 18:59:01.000000 linkexpander-1.0.0.post2/README.md
--rw-rw-rw-   0        0        0      641 2024-05-17 19:47:28.000000 linkexpander-1.0.0.post2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 19:47:47.219152 linkexpander-1.0.0.post2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 07:13:04.615685 linkexpander-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-06-02 07:13:04.605168 linkexpander-1.1.0/LinkExpander/
+-rw-rw-rw-   0        0        0       45 2024-05-17 19:45:28.000000 linkexpander-1.1.0/LinkExpander/__init__.py
+-rw-rw-rw-   0        0        0     3282 2024-05-13 03:55:41.000000 linkexpander-1.1.0/LinkExpander/linktypes.py
+-rw-rw-rw-   0        0        0    32636 2024-06-02 07:11:52.000000 linkexpander-1.1.0/LinkExpander/main.py
+drwxrwxrwx   0        0        0        0 2024-06-02 07:13:04.612275 linkexpander-1.1.0/LinkExpander.egg-info/
+-rw-rw-rw-   0        0        0     2199 2024-06-02 07:13:04.000000 linkexpander-1.1.0/LinkExpander.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-06-02 07:13:04.000000 linkexpander-1.1.0/LinkExpander.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 07:13:04.000000 linkexpander-1.1.0/LinkExpander.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 07:13:04.000000 linkexpander-1.1.0/LinkExpander.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2199 2024-06-02 07:13:04.613529 linkexpander-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1630 2024-05-16 18:59:01.000000 linkexpander-1.1.0/README.md
+-rw-rw-rw-   0        0        0      639 2024-06-02 07:12:28.000000 linkexpander-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 07:13:04.615685 linkexpander-1.1.0/setup.cfg
```

### Comparing `linkexpander-1.0.0.post2/LinkExpander/linktypes.py` & `linkexpander-1.1.0/LinkExpander/linktypes.py`

 * *Files identical despite different names*

### Comparing `linkexpander-1.0.0.post2/LinkExpander/main.py` & `linkexpander-1.1.0/LinkExpander/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,37 +31,37 @@
 def resolve_redirects(url:str) -> str:
     resp = requests.get(url, headers=headers)
     if not resp.ok:
         raise RuntimeError(f"{url}::{resp.status_code}")
     return resp.url
 
 @overload
-def webdrv_find(driver : EC.AnyDriver, 
-                condition : Callable[[EC.AnyDriver], WebElement], 
+def webdrv_find(driver : EC.WebDriver, 
+                condition : Callable[[EC.WebDriver], WebElement], 
                 timeout : float = 3.0, 
                 poll_frequency : float = 0.5, 
                 strict = False,
                 invert = False) -> WebElement | None: ...
 @overload
-def webdrv_find(driver : EC.AnyDriver, 
-                condition : Callable[[EC.AnyDriver], WebElement], 
+def webdrv_find(driver : EC.WebDriver, 
+                condition : Callable[[EC.WebDriver], WebElement], 
                 timeout : float = 3.0, 
                 poll_frequency : float = 0.5, 
                 strict = True,
                 invert = False) -> WebElement: ...
 @overload
-def webdrv_find(driver : EC.AnyDriver, 
-                condition : Callable[[EC.AnyDriver], WebElement], 
+def webdrv_find(driver : EC.WebDriver, 
+                condition : Callable[[EC.WebDriver], WebElement], 
                 timeout : float = 3.0, 
                 poll_frequency : float = 0.5, 
                 strict = False,
                 invert = True) -> WebElement | Literal[True] | None: ...
 @overload
-def webdrv_find(driver : EC.AnyDriver, 
-                condition : Callable[[EC.AnyDriver], WebElement], 
+def webdrv_find(driver : EC.WebDriver, 
+                condition : Callable[[EC.WebDriver], WebElement], 
                 timeout : float = 3.0, 
                 poll_frequency : float = 0.5, 
                 strict = True,
                 invert = True) -> WebElement | Literal[True]: ...
 
 def webdrv_find(driver, condition, timeout=3.0, poll_frequency=0.5, strict=False, invert=False):
     try:
```

### Comparing `linkexpander-1.0.0.post2/LinkExpander.egg-info/PKG-INFO` & `linkexpander-1.1.0/LinkExpander.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinkExpander
-Version: 1.0.0.post2
+Version: 1.1.0
 Summary: Link expander in Python which parses and returns the URLs and information in common link domains.
 Author-email: devdagoat <fidevran@hotmail.com>
 Project-URL: Homepage, https://github.com/devdagoat/LinkExpander
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `linkexpander-1.0.0.post2/PKG-INFO` & `linkexpander-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinkExpander
-Version: 1.0.0.post2
+Version: 1.1.0
 Summary: Link expander in Python which parses and returns the URLs and information in common link domains.
 Author-email: devdagoat <fidevran@hotmail.com>
 Project-URL: Homepage, https://github.com/devdagoat/LinkExpander
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `linkexpander-1.0.0.post2/README.md` & `linkexpander-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `linkexpander-1.0.0.post2/pyproject.toml` & `linkexpander-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "LinkExpander"
 authors = [{name="devdagoat", email="fidevran@hotmail.com"},]
-version = "1.0.0r2"
+version = "1.1.0"
 description = "Link expander in Python which parses and returns the URLs and information in common link domains."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
```

