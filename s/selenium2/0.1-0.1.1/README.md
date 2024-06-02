# Comparing `tmp/selenium2-0.1.tar.gz` & `tmp/selenium2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium2-0.1.tar", last modified: Tue Apr 30 05:25:01 2024, max compression
+gzip compressed data, was "selenium2-0.1.1.tar", last modified: Sun Jun  2 21:47:04 2024, max compression
```

## Comparing `selenium2-0.1.tar` & `selenium2-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 05:25:01.084592 selenium2-0.1/
--rw-rw-rw-   0        0        0    11556 2024-04-30 03:56:52.000000 selenium2-0.1/LICENSE
--rw-rw-rw-   0        0        0    13622 2024-04-30 05:25:01.083595 selenium2-0.1/PKG-INFO
--rw-rw-rw-   0        0        0    12942 2024-04-30 04:35:17.000000 selenium2-0.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-30 05:25:01.054294 selenium2-0.1/selenium2/
--rw-rw-rw-   0        0        0       39 2021-04-30 16:56:53.000000 selenium2-0.1/selenium2/__init__.py
--rw-rw-rw-   0        0        0    12336 2024-04-30 04:51:34.000000 selenium2-0.1/selenium2/browser.py
--rw-rw-rw-   0        0        0    10829 2024-04-30 03:34:40.000000 selenium2-0.1/selenium2/browser.pyi
-drwxrwxrwx   0        0        0        0 2024-04-30 05:25:01.079592 selenium2-0.1/selenium2/browser_support/
--rw-rw-rw-   0        0        0        0 2021-04-20 15:35:46.000000 selenium2-0.1/selenium2/browser_support/__init__.py
--rw-rw-rw-   0        0        0    10232 2024-04-30 02:43:13.000000 selenium2-0.1/selenium2/browser_support/_base.py
--rw-rw-rw-   0        0        0      859 2024-04-30 02:43:18.000000 selenium2-0.1/selenium2/browser_support/_driver.py
--rw-rw-rw-   0        0        0     7863 2024-04-30 04:50:26.000000 selenium2-0.1/selenium2/browser_support/_webdrivercreator.py
--rw-rw-rw-   0        0        0     3975 2024-04-30 02:44:04.000000 selenium2-0.1/selenium2/browser_support/alert.py
--rw-rw-rw-   0        0        0     1596 2024-04-30 02:45:02.000000 selenium2-0.1/selenium2/browser_support/browsermanagement.py
--rw-rw-rw-   0        0        0     6365 2024-04-30 02:45:18.000000 selenium2-0.1/selenium2/browser_support/cookies.py
--rw-rw-rw-   0        0        0    18255 2024-04-30 02:45:32.000000 selenium2-0.1/selenium2/browser_support/element.py
--rw-rw-rw-   0        0        0     2500 2024-04-30 02:45:41.000000 selenium2-0.1/selenium2/browser_support/frames.py
--rw-rw-rw-   0        0        0     5395 2024-04-30 03:37:40.000000 selenium2-0.1/selenium2/browser_support/javascript.py
--rw-rw-rw-   0        0        0     4801 2024-04-30 02:42:39.000000 selenium2-0.1/selenium2/browser_support/screenshot.py
--rw-rw-rw-   0        0        0    10519 2024-04-30 03:38:51.000000 selenium2-0.1/selenium2/browser_support/selects.py
--rw-rw-rw-   0        0        0     5933 2024-04-30 03:39:02.000000 selenium2-0.1/selenium2/browser_support/tables.py
--rw-rw-rw-   0        0        0    10727 2024-04-30 03:42:11.000000 selenium2-0.1/selenium2/browser_support/waiting.py
--rw-rw-rw-   0        0        0    14498 2024-04-30 03:42:11.000000 selenium2-0.1/selenium2/browser_support/windowmanager.py
--rw-rw-rw-   0        0        0      463 2024-04-30 04:30:04.000000 selenium2-0.1/selenium2/config.py
--rw-rw-rw-   0        0        0     1690 2024-04-30 05:24:29.000000 selenium2-0.1/selenium2/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-30 05:25:01.081595 selenium2-0.1/selenium2/site_specific/
--rw-rw-rw-   0        0        0       51 2024-04-30 04:50:35.000000 selenium2-0.1/selenium2/site_specific/__init__.py
--rw-rw-rw-   0        0        0     2609 2024-04-30 00:40:12.000000 selenium2-0.1/selenium2/site_specific/default.py
-drwxrwxrwx   0        0        0        0 2024-04-30 05:25:01.082593 selenium2-0.1/selenium2.egg-info/
--rw-rw-rw-   0        0        0    13622 2024-04-30 05:25:00.000000 selenium2-0.1/selenium2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1751 2024-04-30 05:25:00.000000 selenium2-0.1/selenium2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 05:25:00.000000 selenium2-0.1/selenium2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-30 05:25:00.000000 selenium2-0.1/selenium2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-30 05:25:00.000000 selenium2-0.1/selenium2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 05:25:01.084592 selenium2-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1063 2024-04-30 05:24:42.000000 selenium2-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:47:04.813065 selenium2-0.1.1/
+-rw-rw-rw-   0        0        0    11556 2024-04-30 03:56:52.000000 selenium2-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    13867 2024-06-02 21:47:04.811766 selenium2-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13146 2024-05-08 17:18:03.000000 selenium2-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-06-02 21:47:04.784048 selenium2-0.1.1/selenium2/
+-rw-rw-rw-   0        0        0       39 2021-04-30 16:56:53.000000 selenium2-0.1.1/selenium2/__init__.py
+-rw-rw-rw-   0        0        0    12641 2024-06-02 21:44:51.000000 selenium2-0.1.1/selenium2/browser.py
+-rw-rw-rw-   0        0        0    10980 2024-06-02 21:38:25.000000 selenium2-0.1.1/selenium2/browser.pyi
+drwxrwxrwx   0        0        0        0 2024-06-02 21:47:04.801759 selenium2-0.1.1/selenium2/browser_support/
+-rw-rw-rw-   0        0        0        0 2021-04-20 15:35:46.000000 selenium2-0.1.1/selenium2/browser_support/__init__.py
+-rw-rw-rw-   0        0        0    10148 2024-05-29 15:55:11.000000 selenium2-0.1.1/selenium2/browser_support/_base.py
+-rw-rw-rw-   0        0        0      859 2024-04-30 02:43:18.000000 selenium2-0.1.1/selenium2/browser_support/_driver.py
+-rw-rw-rw-   0        0        0     8244 2024-06-02 21:46:10.000000 selenium2-0.1.1/selenium2/browser_support/_webdrivercreator.py
+-rw-rw-rw-   0        0        0     3975 2024-04-30 02:44:04.000000 selenium2-0.1.1/selenium2/browser_support/alert.py
+-rw-rw-rw-   0        0        0     1596 2024-04-30 02:45:02.000000 selenium2-0.1.1/selenium2/browser_support/browsermanagement.py
+-rw-rw-rw-   0        0        0     6359 2024-05-08 17:05:52.000000 selenium2-0.1.1/selenium2/browser_support/cookies.py
+-rw-rw-rw-   0        0        0    18255 2024-04-30 02:45:32.000000 selenium2-0.1.1/selenium2/browser_support/element.py
+-rw-rw-rw-   0        0        0     2500 2024-04-30 02:45:41.000000 selenium2-0.1.1/selenium2/browser_support/frames.py
+-rw-rw-rw-   0        0        0     5395 2024-04-30 03:37:40.000000 selenium2-0.1.1/selenium2/browser_support/javascript.py
+-rw-rw-rw-   0        0        0     4801 2024-04-30 02:42:39.000000 selenium2-0.1.1/selenium2/browser_support/screenshot.py
+-rw-rw-rw-   0        0        0    10519 2024-04-30 03:38:51.000000 selenium2-0.1.1/selenium2/browser_support/selects.py
+-rw-rw-rw-   0        0        0     5933 2024-04-30 03:39:02.000000 selenium2-0.1.1/selenium2/browser_support/tables.py
+-rw-rw-rw-   0        0        0     7665 2024-06-02 21:30:56.000000 selenium2-0.1.1/selenium2/browser_support/testing.py
+-rw-rw-rw-   0        0        0    10717 2024-06-02 21:24:25.000000 selenium2-0.1.1/selenium2/browser_support/waiting.py
+-rw-rw-rw-   0        0        0    14498 2024-04-30 03:42:11.000000 selenium2-0.1.1/selenium2/browser_support/windowmanager.py
+-rw-rw-rw-   0        0        0      537 2024-05-08 17:03:58.000000 selenium2-0.1.1/selenium2/config.py
+-rw-rw-rw-   0        0        0     2020 2024-05-08 17:18:03.000000 selenium2-0.1.1/selenium2/logger.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:47:04.803765 selenium2-0.1.1/selenium2/site_specific/
+-rw-rw-rw-   0        0        0       51 2024-04-30 04:50:35.000000 selenium2-0.1.1/selenium2/site_specific/__init__.py
+-rw-rw-rw-   0        0        0     2609 2024-04-30 00:40:12.000000 selenium2-0.1.1/selenium2/site_specific/default.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:47:04.809765 selenium2-0.1.1/selenium2.egg-info/
+-rw-rw-rw-   0        0        0    13867 2024-06-02 21:47:04.000000 selenium2-0.1.1/selenium2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1032 2024-06-02 21:47:04.000000 selenium2-0.1.1/selenium2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 21:47:04.000000 selenium2-0.1.1/selenium2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-06-02 21:47:04.000000 selenium2-0.1.1/selenium2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 21:47:04.000000 selenium2-0.1.1/selenium2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 21:47:04.813065 selenium2-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2024-06-02 21:32:12.000000 selenium2-0.1.1/setup.py
```

### Comparing `selenium2-0.1/LICENSE` & `selenium2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/PKG-INFO` & `selenium2-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: selenium2
-Version: 0.1
+Version: 0.1.1
 Summary: A comprehensive Selenium wrapper designed to simplify browser automation and testing tasks.
 Home-page: https://github.com/loudpumpkins/selenium2
 Author: Alexei Panov
 Author-email: alexei_panov@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: selenium==4.2.0
+Requires-Dist: beautifulsoup4==4.12.3
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
 Requires-Dist: twine>=4.0.2; extra == "dev"
 
 Selenium 2
 ============
 
@@ -258,16 +259,16 @@
 
 Environment Variables
 ---------------------
 
 The following environment variables can be set to configure various aspects of the Selenium2 behavior:
 
 ``DEBUG``
-    Controls the debug output of the Selenium2 wrapper. Set to ``True`` to enable verbose logging.
-    Default is ``False``.
+    Controls the debug output of the Selenium2 wrapper. Set to ``False`` to disable verbose logging.
+    Default is ``True``.
 
     .. code-block:: bash
 
         export SELENIUM2_DEBUG=True
 
 ``SELENIUM2_DEFAULT_TIMEOUT``
     Specifies the default timeout in seconds for explicit waits.
@@ -281,21 +282,29 @@
     Sets the directory where screenshots will be saved.
     Default is 'screenshots'.
 
     .. code-block:: bash
 
         export SELENIUM2_SCREENSHOT_PATH='/path/to/screenshots'
 
-``SELENIUM2_COOKIES_PATH``
+``SELENIUM2_REPORT_PATH``
+    Sets the directory where test results will be saved.
+    Default is 'reports'.
+
+    .. code-block:: bash
+
+        export SELENIUM2_SCREENSHOT_PATH='/path/to/reports'
+
+``SELENIUM2_COOKIE_PATH``
     Defines the directory for storing browser cookies.
     Default is 'cookies'.
 
     .. code-block:: bash
 
-        export SELENIUM2_COOKIES_PATH='/path/to/cookies'
+        export SELENIUM2_COOKIE_PATH='/path/to/cookies'
 
 These environment variables allow you to customize the behavior of the Selenium2 wrapper without changing the code. They are particularly useful for adapting the wrapper to different testing environments or requirements.
 
 Contributing
 ------------
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `selenium2-0.1/README.rst` & `selenium2-0.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -239,16 +239,16 @@
 
 Environment Variables
 ---------------------
 
 The following environment variables can be set to configure various aspects of the Selenium2 behavior:
 
 ``DEBUG``
-    Controls the debug output of the Selenium2 wrapper. Set to ``True`` to enable verbose logging.
-    Default is ``False``.
+    Controls the debug output of the Selenium2 wrapper. Set to ``False`` to disable verbose logging.
+    Default is ``True``.
 
     .. code-block:: bash
 
         export SELENIUM2_DEBUG=True
 
 ``SELENIUM2_DEFAULT_TIMEOUT``
     Specifies the default timeout in seconds for explicit waits.
@@ -262,21 +262,29 @@
     Sets the directory where screenshots will be saved.
     Default is 'screenshots'.
 
     .. code-block:: bash
 
         export SELENIUM2_SCREENSHOT_PATH='/path/to/screenshots'
 
-``SELENIUM2_COOKIES_PATH``
+``SELENIUM2_REPORT_PATH``
+    Sets the directory where test results will be saved.
+    Default is 'reports'.
+
+    .. code-block:: bash
+
+        export SELENIUM2_SCREENSHOT_PATH='/path/to/reports'
+
+``SELENIUM2_COOKIE_PATH``
     Defines the directory for storing browser cookies.
     Default is 'cookies'.
 
     .. code-block:: bash
 
-        export SELENIUM2_COOKIES_PATH='/path/to/cookies'
+        export SELENIUM2_COOKIE_PATH='/path/to/cookies'
 
 These environment variables allow you to customize the behavior of the Selenium2 wrapper without changing the code. They are particularly useful for adapting the wrapper to different testing environments or requirements.
 
 Contributing
 ------------
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `selenium2-0.1/selenium2/browser.py` & `selenium2-0.1.1/selenium2/browser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+import os
 import re
 from typing import Type
 
 from .config import (DEFAULT_TIMEOUT, DEFAULT_SPEED,
-                     SCREENSHOT_ROOT_DIRECTORY, COOKIES_ROOT_DIRECTORY,)
+                     SCREENSHOT_ROOT_DIRECTORY, COOKIE_ROOT_DIRECTORY, REPORT_ROOT_DIRECTORY, )
 from .logger import Logger
 from .browser_support.alert import Alert
 from .browser_support.browsermanagement import BrowserManagement
 from .browser_support.cookies import Cookies
 from .browser_support.element import Element
 from .browser_support.frames import Frames
 from .browser_support.javascript import Javascript
 from .browser_support.screenshot import Screenshot
 from .browser_support.selects import Selects
 from .browser_support.tables import Tables
+from .browser_support.testing import Testing
 from .browser_support.waiting import Waiting
 from .browser_support.windowmanager import WindowManager
 from .browser_support._webdrivercreator import WebDriverCreator
 from .site_specific import SiteBehaviour
 
 
 class Browser:
@@ -115,28 +117,30 @@
 
     def __init__(self, browser='ff', profile=None, options=None, ip=None):
         self.driver = WebDriverCreator().create_driver(
             browser, profile, options, ip
         )
         self.implicit_wait = 0
         self.log = Logger.get_logger()
-        self.speed = DEFAULT_SPEED  # TODO add a session speed controller
-        self.timeout = DEFAULT_TIMEOUT
-        self.screenshot_directory = SCREENSHOT_ROOT_DIRECTORY
-        self.cookies_directory = COOKIES_ROOT_DIRECTORY
+        self.speed = os.environ.get('DEFAULT_SPEED', 0.0)  # TODO add a session speed controller
+        self.timeout = os.environ.get('SELENIUM2_DEFAULT_TIMEOUT', 15)
+        self.screenshot_directory = os.environ.get('SELENIUM2_SCREENSHOT_PATH', 'screenshots')
+        self.report_directory = os.environ.get('SELENIUM2_REPORT_PATH', 'reports')
+        self.cookie_directory = os.environ.get('SELENIUM2_COOKIE_PATH', 'cookies')
         libraries = [
             Alert(self),
             BrowserManagement(self),
             Cookies(self),
             Element(self),
             Frames(self),
             Javascript(self),
             Screenshot(self),
             Selects(self),
             Tables(self),
+            Testing(self),
             Waiting(self),
             WindowManager(self),
         ]
         self.get_attributes(libraries)
 
     def __enter__(self):
         return self
@@ -279,16 +283,16 @@
     def get_members(self, library):
         """Get the name:value pairs of the methods in the instance provided."""
         for name in dir(library):
             yield name, getattr(library, name)
 
     def set_implicit_wait(self, time_to_wait):
         """
-        Set the time in seconds for the browser to wait for pages/elements.
-        This is implemented by the browser's browser and not selenium. As a
+        Set the time in seconds for the driver to wait for pages/elements.
+        This is implemented by the browser's driver and not selenium. As a
         result, behaviour can be unexpected as it is barely documented and
         each browser might have different implementations.
 
         Recommend using explicit waits or the wait functions in `waiting.py`
 
         :param time_to_wait: int - time to wait in seconds
         :return: NoReturn
```

### Comparing `selenium2-0.1/selenium2/browser.pyi` & `selenium2-0.1.1/selenium2/browser.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Browser:
 
     driver: WebDriver = ...
     implicit_wait: int = ...
     log: Any = ...
     speed: int = ...
     screenshot_directory: str = ...
-    cookies_directory: str = ...
+    cookie_directory: str = ...
     timeout: bool = ...
 
     def assert_proxy_is(self, ip:str)->NoReturn: ...
     def set_implicit_wait(self, time_to_wait: int) -> NoReturn: ...
     def unset_implicit_wait(self) -> NoReturn: ...
 
     """ from browser.py """
@@ -38,16 +38,16 @@
 
     """ from base.py """
     def find_element(self, locator: U[WebElement, str], required: bool=True,
                      parent: U[WebDriver, WebElement]=None) -> WebElement : ...
     def find_elements(self, locator: str, required: bool=False,
                       parent: U[WebDriver, WebElement]=None) -> List[WebElement] : ...
     def is_text_present(self, text: str) -> bool: ...
-    def is_enabled(self, locator: U[WebElement, str], tag: str=None) -> bool: ...
-    def is_visible(self, locator: U[WebElement, str], tag: str=None) -> bool: ...
+    def is_enabled(self, locator: U[WebElement, str]) -> bool: ...
+    def is_visible(self, locator: U[WebElement, str]) -> bool: ...
 
     """ from alert.py """
     def get_alert(self, timeout: int=DEFAULT_TIMEOUT, message: str ='') -> Alert: ...
     def get_alert_text(self, timeout: int=DEFAULT_TIMEOUT) -> str: ...
     def handle_alert(self, action: str='accept', timeout: int=DEFAULT_TIMEOUT) -> str: ...
     def input_text_into_alert(self, text: str, action: str='accept',
                               timeout: int=None) -> str: ...
@@ -91,16 +91,15 @@
     def get_element_size(self, locator: U[WebElement, str]) -> (int, int): ...
     def get_text(self, locator: U[WebElement, str]) -> str: ...
     def page_contains_text(self, text:str) -> bool: ...
     def right_click_element_at_coordinates(self, locator: U[WebElement, str],
                                            xoffset: int, yoffset: int) -> NoReturn: ...
     def send_keys(self, locator: U[WebElement, str]=None,
                   *keys: U[List[str], str]) -> NoReturn: ...
-    def highlight_elements(self, locator: U[List[WebElement], WebElement, str],
-                           tag: str=None) -> NoReturn: ...
+    def highlight_elements(self, locator: U[List[WebElement], WebElement, str]) -> NoReturn: ...
     def set_focus_to_element(self, locator: U[WebElement, str]) -> NoReturn: ...
     def mouse_down(self, locator: U[WebElement, str]) -> NoReturn: ...
     def mouse_out(self, locator: U[WebElement, str]) -> NoReturn: ...
     def mouse_over(self, locator: U[WebElement, str]) -> NoReturn: ...
     def mouse_up(self, locator: U[WebElement, str]) -> NoReturn: ...
     def scroll_element_into_view(self, locator: U[WebElement, str]) -> NoReturn: ...
     def simulate_event(self, locator: U[WebElement, str], event: str) -> NoReturn: ...
@@ -148,14 +147,20 @@
     def get_table_cell_by_text(self, locator: U[WebElement, str],
                                text: str) -> str: ...
     def get_table_row_by_index(self, locator: U[WebElement, str],
                                row: U[str, int]) -> List[WebElement]: ...
     def get_table_row_by_text(self, locator: U[WebElement, str],
                               text: str) -> List[WebElement]: ...
 
+    """ from testing.py """
+
+    def verify_visual_baseline(self, level: int=1, baseline: bool=False, name: str=None) -> NoReturn: ...
+
+    def set_report_directory(self, path: str=None, append: bool=True) -> str: ...
+
     """ from waiting.py """
     def wait_for_element(self, locator: U[WebElement, str], negate:bool =False,
                          timeout: int=DEFAULT_TIMEOUT,
                          parent: U[WebDriver, WebElement]=None) -> WebElement: ...
     def wait_for_element_to_be_enabled(self, locator: U[WebElement, str],
                                        negate: bool=False, timeout: int=DEFAULT_TIMEOUT) -> WebElement : ...
     def wait_for_element_to_be_visible(self, locator, negate=False,
```

### Comparing `selenium2-0.1/selenium2/browser_support/_base.py` & `selenium2-0.1.1/selenium2/browser_support/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         - ``first_only`` will limit the search result to the first matching
           element. In find_elements, we set ``first_only`` to False return a
           list of elements.
 
         :param locator: str
         :param required: bool - [required] will raise 'ElementNotFound' exception
             if element isn't found. [not required] will return 'None'
-        :param parent: WebElement - the browser or parent element
+        :param parent: WebElement - the driver or parent element
         :param first_only: bool - return all elements or only the first
         :return WebElement:
         """
         if parent and not self._is_webelement(parent):
             raise ValueError(f'Parent must be Selenium WebElement but it '
                              f'was {type(parent)}.')
         if self._is_webelement(locator):
@@ -121,15 +121,15 @@
         single WebElement as `find_element` does.
 
         See `find_element` for ``locator`` usage and function details.
 
         :param locator: str
         :param required: bool - [required] will raise 'ElementNotFound' exception
             if element isn't found. [not required] will return 'None'
-        :param parent: WebElement - the browser or parent element
+        :param parent: WebElement - the driver or parent element
         :return: List[WebElement]
         """
         return self.find_element(locator, required, parent, False)
 
     def is_text_present(self, text):
         """
         See if page to contains `text`. This will not look into the page source
@@ -138,47 +138,45 @@
 
         :param text: str
         :return: bool
         """
         locator = "xpath://*[contains(., %s)]" % self._escape_xpath_value(text)
         return self.find_element(locator, required=False) is not None
 
-    def is_enabled(self, locator, tag=None):
+    def is_enabled(self, locator):
         """
         See if an element located by ``locator`` is enabled.
 
         See `find_element()` for ``locator`` syntax.
 
         :param locator: str or WebElement
-        :param tag: str
         :return:
         """
-        element = self.find_element(locator, tag, required=False)
+        element = self.find_element(locator, required=False)
         if element is None:
             return None
         return (element.is_enabled() and
                 element.get_attribute('readonly') is None)
 
-    def is_visible(self, locator, tag=None):
+    def is_visible(self, locator):
         """
         See if an element located by ``locator`` is visible.
         Visibility is determined by selenium and looks for attributes /
         properties such as <input> with type 'hidden', NOSCRIPT elements
         `dom.isElement(elem, goog.dom.TagName.NOSCRIPT)`, styles set as
         'visibility':'hidden' or 'display':'none', opacity set to zero, etc.
         Selenium will also look for the element's parent's visibility to
         determine this element's visibility.
 
         See `find_element()` for ``locator`` syntax.
 
         :param locator: str or WebElement
-        :param tag: str
         :return:
         """
-        element = self.find_element(locator, tag, required=False)
+        element = self.find_element(locator, required=False)
         return element.is_displayed() if element else None
 
     def _get_strategy(self, locator):
         """support method used to parse the locator into two string
         'id:element'            returns     'id' and 'element'
         'class name = myClass'  returns     'class name' and 'myClass'
         """
@@ -222,15 +220,14 @@
 
     def _find_by_class_name(self, query, parent):
         return parent.find_elements(By.CLASS_NAME, query)
 
     def _find_by_tag_name(self, query, parent):
         return parent.find_elements(By.TAG_NAME, query)
 
-
     def _escape_xpath_value(self, value):
         # https://stackoverflow.com/questions/14822153/escape-single-quote-in-xpath-with-nokogiri
         # if you wanted to match the string: "That's mine", he said.,
         # you would need to do something like:
         #   text()=concat('"That', "'", 's mine", he said.')
         if '"' in value and '\'' in value:
             parts_wo_apos = value.split('\'')
```

### Comparing `selenium2-0.1/selenium2/browser_support/_driver.py` & `selenium2-0.1.1/selenium2/browser_support/_driver.py`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/selenium2/browser_support/_webdrivercreator.py` & `selenium2-0.1.1/selenium2/browser_support/_webdrivercreator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from selenium import webdriver
 from selenium.webdriver import ChromeOptions, FirefoxOptions, FirefoxProfile
+from selenium.webdriver.safari.options import Options as SafariOptions
 
 from ..logger import Logger
 
 
 class WebDriverCreator:
     """
     Solely responsible for creating a web driver for the specified browser with
@@ -40,18 +41,18 @@
             # headless firefox
             'headless_firefox': ['headlessfirefox', 'firefoxheadless',
                                  'headless firefox', 'headless_firefox'],
             # internet explorer
             'ie': ['ie', 'ei', 'internetexplorer', 'explorer'],
             # edge
             'edge': ['edge'],
+            'safari': ['safari'],
 
             # TODO: add other browsers
             # 'opera' : 'opera',
-            # 'safari' : 'safari',
             # 'phantomjs' : 'phantomjs',
             # 'htmlunit' : 'htmlunit',
             # 'htmlunitwithjs' : 'htmlunit_with_js',
             # 'android' : 'android',
             # 'iphone' : 'iphone'
         }
         for key, value in mapper.items():
@@ -180,7 +181,17 @@
         if profile is not None:
             self.log.warning('Edge was instantiated with a profile which is not applicable.')
         if not options:
             options = webdriver.EdgeOptions()
         if ip:
             options.add_argument(f'--proxy-server={ip}')
         return webdriver.Edge(options=options)
+
+    def create_safari(self, profile, options, ip):
+        """
+        Creates a Safari browser instance.
+        """
+        if not options:
+            options = SafariOptions()
+        if ip:
+            options.add_argument(f'--proxy-server={ip}')
+        return webdriver.Safari(options=options)
```

### Comparing `selenium2-0.1/selenium2/browser_support/alert.py` & `selenium2-0.1.1/selenium2/browser_support/alert.py`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/selenium2/browser_support/browsermanagement.py` & `selenium2-0.1.1/selenium2/browser_support/browsermanagement.py`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/selenium2/browser_support/cookies.py` & `selenium2-0.1.1/selenium2/browser_support/cookies.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         `filename` must be a binary data steam.
 
         :param filename: str - filename
         :param path:
         :return:
         """
         if path == 'default':
-            path = os.path.join(self._root.cookies_directory, filename)
+            path = os.path.join(self._root.cookie_directory, filename)
         else:
             path = os.path.join(path, filename)
         try:
             with open(path, 'r') as filehandle:
                 # load binary data steam of a list of cookies
                 cookies = json.load(filehandle)
         except FileNotFoundError:
@@ -118,36 +118,36 @@
         return path
 
     def set_cookies_directory(self, path=None, append=True):
         """
         Sets the directory for saved cookies.
 
         ``path`` can be an absolute path or relative path from the current
-        cookies_directory. If the directory does not exist, it will be
+        cookie_directory. If the directory does not exist, it will be
         created.
 
         ``append`` is set to True by default and will append to current path and
         normalise it, where False will overwrite the path attribute.
 
         Will return the previous path to be stored and re-set if needed.
 
         :param path: str - the path to append or set
         :param append: bool - True will add / False will replace
         :return: str - previous path
         """
         if path is not None:
-            path = os.path.normpath(os.path.join(self._root.cookies_directory, path)) \
+            path = os.path.normpath(os.path.join(self._root.cookie_directory, path)) \
                 if append else path
             self._create_directory(path)
-        previous = self._root.cookies_directory
+        previous = self._root.cookie_directory
         path = os.path.abspath(path)
         self.log.info('Setting cookies directory from {} to {}'.format(
             previous, path
         ))
-        self._root.cookies_directory = path
+        self._root.cookie_directory = path
         return previous
 
     def set_cookies_expiry(self, date: int = 3735325880):
         """
         Sets the expiry date of all cookies to 'date'. Default is 3735325880
         which is equivalent to Thu, 13 May 2088 22:38:37 GMT.
 
@@ -168,10 +168,10 @@
         if not os.path.exists(target_dir):
             self.log.info('Creating new directory to store cookies at {}'.format(
                 target_dir
             ))
             os.makedirs(target_dir)
 
     def _get_cookies_path(self, filename):
-        directory = self._root.cookies_directory
+        directory = self._root.cookie_directory
         filename = filename.replace('/', os.sep)
         return os.path.join(directory, filename)
```

### Comparing `selenium2-0.1/selenium2/browser_support/element.py` & `selenium2-0.1.1/selenium2/browser_support/element.py`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/selenium2/browser_support/frames.py` & `selenium2-0.1.1/selenium2/browser_support/frames.py`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/selenium2/browser_support/javascript.py` & `selenium2-0.1.1/selenium2/browser_support/javascript.py`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/selenium2/browser_support/screenshot.py` & `selenium2-0.1.1/selenium2/browser_support/screenshot.py`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/selenium2/browser_support/selects.py` & `selenium2-0.1.1/selenium2/browser_support/selects.py`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/selenium2/browser_support/tables.py` & `selenium2-0.1.1/selenium2/browser_support/tables.py`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/selenium2/browser_support/waiting.py` & `selenium2-0.1.1/selenium2/browser_support/waiting.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 class Waiting(Base):
 
     def __init__(self, root):
         super().__init__(root)
         self.log = Logger.get_logger()
 
-
     def wait_for_element(self, locator, negate=False, timeout=DEFAULT_TIMEOUT,
                          parent=None):
         """
         Wait for `element` and return it if found or raise timeoutException
 
         Set ``negate`` to True to exit explicit wait when the element is no
         longer present
@@ -56,15 +55,15 @@
 
         :param locator: WebElement or str
         :param negate: bool - True will wait for condition to be truthy, False
             will wait for the condition to be falsy
         :param timeout: int - explicit wait timeout in seconds
         :return: bool or TimeoutException
         """
-        func = lambda _: self.is_element_enabled(locator)
+        func = lambda _: self.is_enabled(locator)
         if negate:
             self.log.info(
                 'Waiting for element `{}` to be disabled.'.format(locator))
             message = ('Failed to wait for element `{}` to be disabled before '
                        'the timeout [{} second(s)].'.format(locator, timeout))
             self._wait_until_not(func, timeout, message)
             return self.find_element(locator, required=False)
```

### Comparing `selenium2-0.1/selenium2/browser_support/windowmanager.py` & `selenium2-0.1.1/selenium2/browser_support/windowmanager.py`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/selenium2/logger.py` & `selenium2-0.1.1/selenium2/logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,62 @@
-from .config import *
-
-# external
 import logging
 import inspect
+import os
 from os.path import basename
 
-# internal
-
 
 class Logger:
-	""" Main classed used throughout the project
+    """ Main classed used throughout the project
 
-	==LEVEL==   Numeric value
-	CRITICAL    50
-	ERROR       40
-	WARNING     30
-	INFO        20
-	DEBUG       10
-	NOTSET      0
-
-	usage:
-	self.log.info("message")
-
-	"""
-	_loggers = {}
-
-	@classmethod
-	def get_logger(cls, name=None):
-		if name is None:
-			name = cls.get_caller_filename()
-		if name in cls._loggers:
-			return cls._loggers[name]
-		else:
-			# Create and configure a new logger
-			logger = logging.getLogger(name)
-			logger.setLevel(logging.DEBUG)  # Base level for all logs
-
-			# Create handlers with formatters
-			c_handler = logging.StreamHandler()
-			f_handler = logging.FileHandler('library.log')
-			c_format = logging.Formatter(
-				'%(name)s::%(funcName)s::line %(lineno)d - %(levelname)s - %(message)s')
-			f_format = logging.Formatter(
-				'%(asctime)s::%(name)s::%(funcName)s::line %(lineno)d - %(levelname)s - %(message)s',
-				datefmt='%Y/%m/%d::%H/%M/%S')
-
-			c_handler.setFormatter(c_format)
-			f_handler.setFormatter(f_format)
-			logger.addHandler(c_handler)
-			logger.addHandler(f_handler)
-			cls._loggers[name] = logger
-			return logger
-
-	@staticmethod
-	def get_caller_filename():
-		# get the caller's stack frame and extract its filename
-		frame_info = inspect.stack()[2]     # go 2 stacks down : get_caller_filename > Logger.__init__ > calling file
-		path = frame_info.filename
-		filename = basename(path)
-		if len(filename) < 3:
-			# return entire path in case of failed filename extraction
-			return path
-		else:
-			return filename
+    ==LEVEL==   Numeric value
+    CRITICAL    50
+    ERROR       40
+    WARNING     30
+    INFO        20
+    DEBUG       10
+    NOTSET      0
+
+    usage:
+    self.log.info("message")
+
+    """
+    _loggers = {}
+
+    @classmethod
+    def get_logger(cls, name=None):
+        if name is None:
+            name = cls.get_caller_filename()
+        if name in cls._loggers:
+            return cls._loggers[name]
+        else:
+            # Create and configure a new logger
+            logger = logging.getLogger(name)
+            logger.setLevel(logging.DEBUG)  # Base level for all logs
+
+            # Create handlers with formatters
+            c_handler = logging.StreamHandler()
+            f_handler = logging.FileHandler('library.log')
+            c_format = logging.Formatter(
+                '%(name)s::%(funcName)s::line %(lineno)d - %(levelname)s - %(message)s')
+            f_format = logging.Formatter(
+                '%(asctime)s::%(name)s::%(funcName)s::line %(lineno)d - %(levelname)s - %(message)s',
+                datefmt='%Y/%m/%d::%H/%M/%S')
+
+            if os.environ.get('SELENIUM2_DEBUG', True):
+                c_handler.setFormatter(c_format)
+            f_handler.setFormatter(f_format)
+            logger.addHandler(c_handler)
+            logger.addHandler(f_handler)
+            cls._loggers[name] = logger
+            return logger
+
+    @staticmethod
+    def get_caller_filename():
+        # get the caller's stack frame and extract its filename
+        frame_info = inspect.stack()[2]     # go 2 stacks down : get_caller_filename > Logger.__init__ > calling file
+        path = frame_info.filename
+        filename = basename(path)
+        if len(filename) < 3:
+            # return entire path in case of failed filename extraction
+            return path
+        else:
+            return filename
```

### Comparing `selenium2-0.1/selenium2/site_specific/default.py` & `selenium2-0.1.1/selenium2/site_specific/default.py`

 * *Files identical despite different names*

### Comparing `selenium2-0.1/selenium2.egg-info/PKG-INFO` & `selenium2-0.1.1/selenium2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: selenium2
-Version: 0.1
+Version: 0.1.1
 Summary: A comprehensive Selenium wrapper designed to simplify browser automation and testing tasks.
 Home-page: https://github.com/loudpumpkins/selenium2
 Author: Alexei Panov
 Author-email: alexei_panov@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: selenium==4.2.0
+Requires-Dist: beautifulsoup4==4.12.3
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
 Requires-Dist: twine>=4.0.2; extra == "dev"
 
 Selenium 2
 ============
 
@@ -258,16 +259,16 @@
 
 Environment Variables
 ---------------------
 
 The following environment variables can be set to configure various aspects of the Selenium2 behavior:
 
 ``DEBUG``
-    Controls the debug output of the Selenium2 wrapper. Set to ``True`` to enable verbose logging.
-    Default is ``False``.
+    Controls the debug output of the Selenium2 wrapper. Set to ``False`` to disable verbose logging.
+    Default is ``True``.
 
     .. code-block:: bash
 
         export SELENIUM2_DEBUG=True
 
 ``SELENIUM2_DEFAULT_TIMEOUT``
     Specifies the default timeout in seconds for explicit waits.
@@ -281,21 +282,29 @@
     Sets the directory where screenshots will be saved.
     Default is 'screenshots'.
 
     .. code-block:: bash
 
         export SELENIUM2_SCREENSHOT_PATH='/path/to/screenshots'
 
-``SELENIUM2_COOKIES_PATH``
+``SELENIUM2_REPORT_PATH``
+    Sets the directory where test results will be saved.
+    Default is 'reports'.
+
+    .. code-block:: bash
+
+        export SELENIUM2_SCREENSHOT_PATH='/path/to/reports'
+
+``SELENIUM2_COOKIE_PATH``
     Defines the directory for storing browser cookies.
     Default is 'cookies'.
 
     .. code-block:: bash
 
-        export SELENIUM2_COOKIES_PATH='/path/to/cookies'
+        export SELENIUM2_COOKIE_PATH='/path/to/cookies'
 
 These environment variables allow you to customize the behavior of the Selenium2 wrapper without changing the code. They are particularly useful for adapting the wrapper to different testing environments or requirements.
 
 Contributing
 ------------
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `selenium2-0.1/selenium2.egg-info/SOURCES.txt` & `selenium2-0.1.1/selenium2.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,38 +15,17 @@
 ./selenium2/browser_support/cookies.py
 ./selenium2/browser_support/element.py
 ./selenium2/browser_support/frames.py
 ./selenium2/browser_support/javascript.py
 ./selenium2/browser_support/screenshot.py
 ./selenium2/browser_support/selects.py
 ./selenium2/browser_support/tables.py
+./selenium2/browser_support/testing.py
 ./selenium2/browser_support/waiting.py
 ./selenium2/browser_support/windowmanager.py
 ./selenium2/site_specific/__init__.py
 ./selenium2/site_specific/default.py
-selenium2/__init__.py
-selenium2/browser.py
-selenium2/browser.pyi
-selenium2/config.py
-selenium2/logger.py
 selenium2.egg-info/PKG-INFO
 selenium2.egg-info/SOURCES.txt
 selenium2.egg-info/dependency_links.txt
 selenium2.egg-info/requires.txt
-selenium2.egg-info/top_level.txt
-selenium2/browser_support/__init__.py
-selenium2/browser_support/_base.py
-selenium2/browser_support/_driver.py
-selenium2/browser_support/_webdrivercreator.py
-selenium2/browser_support/alert.py
-selenium2/browser_support/browsermanagement.py
-selenium2/browser_support/cookies.py
-selenium2/browser_support/element.py
-selenium2/browser_support/frames.py
-selenium2/browser_support/javascript.py
-selenium2/browser_support/screenshot.py
-selenium2/browser_support/selects.py
-selenium2/browser_support/tables.py
-selenium2/browser_support/waiting.py
-selenium2/browser_support/windowmanager.py
-selenium2/site_specific/__init__.py
-selenium2/site_specific/default.py
+selenium2.egg-info/top_level.txt
```

### Comparing `selenium2-0.1/setup.py` & `selenium2-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # twine upload dist/*
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setup(
     name="selenium2",
-    version="0.1",
+    version="0.1.1",
     description='A comprehensive Selenium wrapper designed to simplify browser automation and testing tasks.',
     package_dir={"": "."},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/loudpumpkins/selenium2",
     author="Alexei Panov",
@@ -24,14 +24,15 @@
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        "selenium==4.2.0"
+        "selenium==4.2.0",
+        "beautifulsoup4==4.12.3"
     ],
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
     python_requires=">=3.8",
 )
```

