# Comparing `tmp/linkedin-jobs-scraper-4.0.0.tar.gz` & `tmp/linkedin-jobs-scraper-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedin-jobs-scraper-4.0.0.tar", last modified: Tue Jan 16 09:46:45 2024, max compression
+gzip compressed data, was "linkedin-jobs-scraper-4.0.1.tar", last modified: Sun Jun  2 14:34:32 2024, max compression
```

## Comparing `linkedin-jobs-scraper-4.0.0.tar` & `linkedin-jobs-scraper-4.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:46:45.121380 linkedin-jobs-scraper-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-01-16 09:46:45.121380 linkedin-jobs-scraper-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:46:45.117380 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:46:45.117380 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/events/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/events/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:46:45.117380 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:46:45.117380 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13102 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/linkedin_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:46:45.117380 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/query/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/query/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:46:45.117380 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13904 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/strategies/anonymous_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    24361 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/strategies/authenticated_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:46:45.121380 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/chrome_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/user_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 09:46:45.117380 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-01-16 09:46:45.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-01-16 09:46:45.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 09:46:45.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-16 09:46:45.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-16 09:46:45.000000 linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 09:46:45.121380 linkedin-jobs-scraper-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-16 09:44:53.000000 linkedin-jobs-scraper-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:34:32.248969 linkedin-jobs-scraper-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-06-02 14:34:32.248969 linkedin-jobs-scraper-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:34:32.244969 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:34:32.244969 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/events/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/events/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:34:32.244969 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:34:32.244969 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/linkedin_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:34:32.244969 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/query/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:34:32.244969 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13904 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/strategies/anonymous_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24361 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/strategies/authenticated_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:34:32.248969 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/chrome_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/user_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:34:32.244969 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-06-02 14:34:32.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-06-02 14:34:32.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 14:34:32.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-02 14:34:32.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 14:34:32.000000 linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 14:34:32.248969 linkedin-jobs-scraper-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-02 14:33:06.000000 linkedin-jobs-scraper-4.0.1/setup.py
```

### Comparing `linkedin-jobs-scraper-4.0.0/LICENSE` & `linkedin-jobs-scraper-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/PKG-INFO` & `linkedin-jobs-scraper-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedin-jobs-scraper
-Version: 4.0.0
+Version: 4.0.1
 Summary: Scrape public available jobs on Linkedin using headless browser
 Home-page: https://github.com/spinlud/py-linkedin-jobs-scraper.git
 Author: Ludovico Fabbri
 Author-email: ludovico.fabbri@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -61,15 +61,15 @@
 * [License](#license)
 
 <!-- toc stop -->
 
 
 ## Requirements
 - [Chrome](https://www.google.com/intl/en_us/chrome/) or [Chromium](https://www.chromium.org/getting-involved/download-chromium)
-- [Chromedriver](https://chromedriver.chromium.org/): latest version tested is `119.0.6045.105` ([Dockerfile](https://github.com/spinlud/python3-selenium-chrome/blob/master/Dockerfile))
+- [Chromedriver](https://chromedriver.chromium.org/): latest version tested is `125.0.6422.141` ([Dockerfile](https://github.com/spinlud/python3-selenium-chrome/blob/master/Dockerfile))
 - Python >= 3.7
 
 
 ## Installation
 Install package:
 ```shell
 pip install linkedin-jobs-scraper
```

### Comparing `linkedin-jobs-scraper-4.0.0/README.md` & `linkedin-jobs-scraper-4.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 * [License](#license)
 
 <!-- toc stop -->
 
 
 ## Requirements
 - [Chrome](https://www.google.com/intl/en_us/chrome/) or [Chromium](https://www.chromium.org/getting-involved/download-chromium)
-- [Chromedriver](https://chromedriver.chromium.org/): latest version tested is `119.0.6045.105` ([Dockerfile](https://github.com/spinlud/python3-selenium-chrome/blob/master/Dockerfile))
+- [Chromedriver](https://chromedriver.chromium.org/): latest version tested is `125.0.6422.141` ([Dockerfile](https://github.com/spinlud/python3-selenium-chrome/blob/master/Dockerfile))
 - Python >= 3.7
 
 
 ## Installation
 Install package:
 ```shell
 pip install linkedin-jobs-scraper
```

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/config.py` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/config.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/events/events.py` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/events/events.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/filters/filters.py` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/filters/filters.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/linkedin_scraper.py` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/linkedin_scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,17 @@
                 )
 
                 websocket_debugger_url = get_websocket_debugger_url(driver)
                 info('Websocket debugger url: ', websocket_debugger_url)
 
                 driver.execute_cdp_cmd('Network.enable', {})
                 driver.execute_cdp_cmd('Page.setBypassCSP', {'enabled': True})
-                driver.execute_cdp_cmd('Network.setUserAgentOverride', {'userAgent': get_random_user_agent()})
+
+                # This can cause the session cookie to be invalidated earlier then expected
+                # driver.execute_cdp_cmd('Network.setUserAgentOverride', {'userAgent': get_random_user_agent()})
 
                 # Run strategy
                 self._strategy.run(
                     driver,
                     search_url,
                     query,
                     location,
```

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/query/query.py` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/query/query.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/strategies/anonymous_strategy.py` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/strategies/anonymous_strategy.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/strategies/authenticated_strategy.py` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/strategies/authenticated_strategy.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/chrome_driver.py` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/chrome_driver.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/logger.py` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/url.py` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/url.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper/utils/user_agent.py` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper.egg-info/PKG-INFO` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedin-jobs-scraper
-Version: 4.0.0
+Version: 4.0.1
 Summary: Scrape public available jobs on Linkedin using headless browser
 Home-page: https://github.com/spinlud/py-linkedin-jobs-scraper.git
 Author: Ludovico Fabbri
 Author-email: ludovico.fabbri@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -61,15 +61,15 @@
 * [License](#license)
 
 <!-- toc stop -->
 
 
 ## Requirements
 - [Chrome](https://www.google.com/intl/en_us/chrome/) or [Chromium](https://www.chromium.org/getting-involved/download-chromium)
-- [Chromedriver](https://chromedriver.chromium.org/): latest version tested is `119.0.6045.105` ([Dockerfile](https://github.com/spinlud/python3-selenium-chrome/blob/master/Dockerfile))
+- [Chromedriver](https://chromedriver.chromium.org/): latest version tested is `125.0.6422.141` ([Dockerfile](https://github.com/spinlud/python3-selenium-chrome/blob/master/Dockerfile))
 - Python >= 3.7
 
 
 ## Installation
 Install package:
 ```shell
 pip install linkedin-jobs-scraper
```

### Comparing `linkedin-jobs-scraper-4.0.0/linkedin_jobs_scraper.egg-info/SOURCES.txt` & `linkedin-jobs-scraper-4.0.1/linkedin_jobs_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linkedin-jobs-scraper-4.0.0/setup.py` & `linkedin-jobs-scraper-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='linkedin-jobs-scraper',
-    version='4.0.0',
+    version='4.0.1',
     author='Ludovico Fabbri',
     author_email='ludovico.fabbri@gmail.com',
     description='Scrape public available jobs on Linkedin using headless browser',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/spinlud/py-linkedin-jobs-scraper.git',
     packages=[
```

