# Comparing `tmp/extract_emails-5.3.3.tar.gz` & `tmp/extract_emails-5.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extract_emails-5.3.3.tar", max compression
+gzip compressed data, was "extract_emails-5.3.4.tar", max compression
```

## Comparing `extract_emails-5.3.3.tar` & `extract_emails-5.3.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1066 2023-12-29 15:51:32.551211 extract_emails-5.3.3/LICENSE
--rw-r--r--   0        0        0     1536 2024-01-02 08:26:17.841842 extract_emails-5.3.3/README.md
--rw-r--r--   0        0        0      596 2024-02-16 14:09:24.078346 extract_emails-5.3.3/extract_emails/__init__.py
--rw-r--r--   0        0        0       82 2024-01-02 08:26:02.334963 extract_emails-5.3.3/extract_emails/browsers/__init__.py
--rw-r--r--   0        0        0     3730 2024-02-16 14:09:24.078346 extract_emails-5.3.3/extract_emails/browsers/chrome_browser.py
--rw-r--r--   0        0        0      345 2023-12-29 19:17:31.174109 extract_emails-5.3.3/extract_emails/browsers/page_source_getter.py
--rw-r--r--   0        0        0     1389 2024-01-02 16:11:13.533902 extract_emails-5.3.3/extract_emails/browsers/requests_browser.py
--rw-r--r--   0        0        0        0 2023-12-29 15:51:32.551211 extract_emails-5.3.3/extract_emails/console/__init__.py
--rw-r--r--   0        0        0     2383 2024-01-22 17:00:32.961997 extract_emails-5.3.3/extract_emails/console/application.py
--rw-r--r--   0        0        0      204 2023-12-29 19:17:31.174109 extract_emails-5.3.3/extract_emails/data_extractors/__init__.py
--rw-r--r--   0        0        0      510 2023-12-29 19:17:31.174109 extract_emails-5.3.3/extract_emails/data_extractors/data_extractor.py
--rw-r--r--   0        0        0     1092 2023-12-29 19:17:31.174109 extract_emails-5.3.3/extract_emails/data_extractors/email_extractor.py
--rw-r--r--   0        0        0      926 2023-12-29 19:17:31.174109 extract_emails-5.3.3/extract_emails/data_extractors/linkedin_extractor.py
--rw-r--r--   0        0        0       57 2023-12-29 19:17:31.174109 extract_emails-5.3.3/extract_emails/data_savers/__init__.py
--rw-r--r--   0        0        0     1545 2023-12-29 19:17:31.174109 extract_emails-5.3.3/extract_emails/data_savers/csv_saver.py
--rw-r--r--   0        0        0      259 2023-12-29 19:17:31.174109 extract_emails-5.3.3/extract_emails/data_savers/data_saver.py
--rw-r--r--   0        0        0       74 2023-12-29 19:17:31.174109 extract_emails-5.3.3/extract_emails/errors/__init__.py
--rw-r--r--   0        0        0      129 2023-12-29 15:51:32.551211 extract_emails-5.3.3/extract_emails/errors/errors.py
--rw-r--r--   0        0        0      796 2023-12-29 19:17:31.174109 extract_emails-5.3.3/extract_emails/factories/__init__.py
--rw-r--r--   0        0        0     1580 2023-12-29 19:17:31.174109 extract_emails-5.3.3/extract_emails/factories/base_factory.py
--rw-r--r--   0        0        0     2026 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/factories/contact_filter_and_email.py
--rw-r--r--   0        0        0     2351 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/factories/contact_filter_and_email_and_linkedin.py
--rw-r--r--   0        0        0     2071 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/factories/contact_filter_and_linkedin.py
--rw-r--r--   0        0        0     2006 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/factories/default_filter_and_email.py
--rw-r--r--   0        0        0     2335 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/factories/default_filter_and_email_and_linkedin.py
--rw-r--r--   0        0        0     2051 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/factories/default_filter_and_linkedin.py
--rw-r--r--   0        0        0      227 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/link_filters/__init__.py
--rw-r--r--   0        0        0     3397 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/link_filters/contact_link_filter.py
--rw-r--r--   0        0        0     1413 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/link_filters/default_link_filter.py
--rw-r--r--   0        0        0     1957 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/link_filters/link_filter_base.py
--rw-r--r--   0        0        0       57 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/models/__init__.py
--rw-r--r--   0        0        0     2592 2024-01-02 19:05:02.906400 extract_emails-5.3.3/extract_emails/models/page_data.py
--rw-r--r--   0        0        0       68 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/utils/__init__.py
--rw-r--r--   0        0        0    20728 2023-12-29 15:51:32.554544 extract_emails-5.3.3/extract_emails/utils/_top_level_domains.py
--rw-r--r--   0        0        0      678 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/utils/email_filter.py
--rw-r--r--   0        0        0       72 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/workers/__init__.py
--rw-r--r--   0        0        0     2462 2023-12-29 19:17:31.177442 extract_emails-5.3.3/extract_emails/workers/default_worker.py
--rw-r--r--   0        0        0     3003 2024-02-16 14:09:24.081679 extract_emails-5.3.3/pyproject.toml
--rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 extract_emails-5.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-06-02 09:19:17.639070 extract_emails-5.3.4/LICENSE
+-rw-r--r--   0        0        0     1735 2024-06-02 09:47:53.861986 extract_emails-5.3.4/README.md
+-rw-r--r--   0        0        0      596 2024-06-02 09:47:53.861986 extract_emails-5.3.4/extract_emails/__init__.py
+-rw-r--r--   0        0        0       82 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/browsers/__init__.py
+-rw-r--r--   0        0        0     3730 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/browsers/chrome_browser.py
+-rw-r--r--   0        0        0      345 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/browsers/page_source_getter.py
+-rw-r--r--   0        0        0     1389 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/browsers/requests_browser.py
+-rw-r--r--   0        0        0        0 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/console/__init__.py
+-rw-r--r--   0        0        0     2383 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/console/application.py
+-rw-r--r--   0        0        0      204 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/data_extractors/__init__.py
+-rw-r--r--   0        0        0      510 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/data_extractors/data_extractor.py
+-rw-r--r--   0        0        0     1092 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/data_extractors/email_extractor.py
+-rw-r--r--   0        0        0      926 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/data_extractors/linkedin_extractor.py
+-rw-r--r--   0        0        0       57 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/data_savers/__init__.py
+-rw-r--r--   0        0        0     1545 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/data_savers/csv_saver.py
+-rw-r--r--   0        0        0      259 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/data_savers/data_saver.py
+-rw-r--r--   0        0        0       74 2024-06-02 09:19:17.642404 extract_emails-5.3.4/extract_emails/errors/__init__.py
+-rw-r--r--   0        0        0      129 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/errors/errors.py
+-rw-r--r--   0        0        0      796 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/factories/__init__.py
+-rw-r--r--   0        0        0     1580 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/factories/base_factory.py
+-rw-r--r--   0        0        0     2026 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/factories/contact_filter_and_email.py
+-rw-r--r--   0        0        0     2351 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/factories/contact_filter_and_email_and_linkedin.py
+-rw-r--r--   0        0        0     2071 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/factories/contact_filter_and_linkedin.py
+-rw-r--r--   0        0        0     2006 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/factories/default_filter_and_email.py
+-rw-r--r--   0        0        0     2335 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/factories/default_filter_and_email_and_linkedin.py
+-rw-r--r--   0        0        0     2051 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/factories/default_filter_and_linkedin.py
+-rw-r--r--   0        0        0      227 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/link_filters/__init__.py
+-rw-r--r--   0        0        0     3397 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/link_filters/contact_link_filter.py
+-rw-r--r--   0        0        0     1413 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/link_filters/default_link_filter.py
+-rw-r--r--   0        0        0     1957 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/link_filters/link_filter_base.py
+-rw-r--r--   0        0        0       57 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/models/__init__.py
+-rw-r--r--   0        0        0     2592 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/models/page_data.py
+-rw-r--r--   0        0        0       68 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/utils/__init__.py
+-rw-r--r--   0        0        0    20728 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/utils/_top_level_domains.py
+-rw-r--r--   0        0        0      678 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/utils/email_filter.py
+-rw-r--r--   0        0        0       72 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/workers/__init__.py
+-rw-r--r--   0        0        0     2462 2024-06-02 09:19:17.645737 extract_emails-5.3.4/extract_emails/workers/default_worker.py
+-rw-r--r--   0        0        0     2961 2024-06-02 09:47:53.861986 extract_emails-5.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 extract_emails-5.3.4/PKG-INFO
```

### Comparing `extract_emails-5.3.3/LICENSE` & `extract_emails-5.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/__init__.py` & `extract_emails-5.3.4/extract_emails/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "5.3.3"
+__version__ = "5.3.4"
 from .factories import (
     ContactFilterAndEmailAndLinkedinFactory,
     ContactFilterAndEmailFactory,
     ContactFilterAndLinkedinFactory,
     DefaultFilterAndEmailAndLinkedinFactory,
     DefaultFilterAndEmailFactory,
     DefaultFilterAndLinkedinFactory,
```

### Comparing `extract_emails-5.3.3/extract_emails/browsers/chrome_browser.py` & `extract_emails-5.3.4/extract_emails/browsers/chrome_browser.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/browsers/requests_browser.py` & `extract_emails-5.3.4/extract_emails/browsers/requests_browser.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/console/application.py` & `extract_emails-5.3.4/extract_emails/console/application.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/data_extractors/email_extractor.py` & `extract_emails-5.3.4/extract_emails/data_extractors/email_extractor.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/data_extractors/linkedin_extractor.py` & `extract_emails-5.3.4/extract_emails/data_extractors/linkedin_extractor.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/data_savers/csv_saver.py` & `extract_emails-5.3.4/extract_emails/data_savers/csv_saver.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/factories/__init__.py` & `extract_emails-5.3.4/extract_emails/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/factories/base_factory.py` & `extract_emails-5.3.4/extract_emails/factories/base_factory.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/factories/contact_filter_and_email.py` & `extract_emails-5.3.4/extract_emails/factories/contact_filter_and_email.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/factories/contact_filter_and_email_and_linkedin.py` & `extract_emails-5.3.4/extract_emails/factories/contact_filter_and_email_and_linkedin.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/factories/contact_filter_and_linkedin.py` & `extract_emails-5.3.4/extract_emails/factories/contact_filter_and_linkedin.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/factories/default_filter_and_email.py` & `extract_emails-5.3.4/extract_emails/factories/default_filter_and_email.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/factories/default_filter_and_email_and_linkedin.py` & `extract_emails-5.3.4/extract_emails/factories/default_filter_and_email_and_linkedin.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/factories/default_filter_and_linkedin.py` & `extract_emails-5.3.4/extract_emails/factories/default_filter_and_linkedin.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/link_filters/contact_link_filter.py` & `extract_emails-5.3.4/extract_emails/link_filters/contact_link_filter.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/link_filters/default_link_filter.py` & `extract_emails-5.3.4/extract_emails/link_filters/default_link_filter.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/link_filters/link_filter_base.py` & `extract_emails-5.3.4/extract_emails/link_filters/link_filter_base.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/models/page_data.py` & `extract_emails-5.3.4/extract_emails/models/page_data.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/utils/_top_level_domains.py` & `extract_emails-5.3.4/extract_emails/utils/_top_level_domains.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/utils/email_filter.py` & `extract_emails-5.3.4/extract_emails/utils/email_filter.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/extract_emails/workers/default_worker.py` & `extract_emails-5.3.4/extract_emails/workers/default_worker.py`

 * *Files identical despite different names*

### Comparing `extract_emails-5.3.3/pyproject.toml` & `extract_emails-5.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [tool.poetry]
 name = "extract-emails"
-version = "5.3.3"
+version = "5.3.4"
 description = "Extract email addresses and linkedin profiles from given URL."
 authors = ["Dmitrii Kurlov <dmitriik@tutanota.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dmitriiweb/extract-emails"
 documentation = "https://dmitriiweb.github.io/extract-emails"
 keywords = ["parser", "email", "linkedin"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
   "Operating System :: MacOS",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.13"
+python = ">=3.10,<3.13"
 pydantic = "^2.5.3"
 loguru = "^0.5.3"
 click = "^8.1.7"
 requests = { version = "^2.31.0", optional = true }
 selenium = { version = "^4.9", optional = true }
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `extract_emails-5.3.3/PKG-INFO` & `extract_emails-5.3.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: extract-emails
-Version: 5.3.3
+Version: 5.3.4
 Summary: Extract email addresses and linkedin profiles from given URL.
 Home-page: https://github.com/dmitriiweb/extract-emails
 License: MIT
 Keywords: parser,email,linkedin
 Author: Dmitrii Kurlov
 Author-email: dmitriik@tutanota.com
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Provides-Extra: all
 Provides-Extra: requests
@@ -41,27 +40,31 @@
 Extract emails and linkedins profiles from a given website
 
 **Support the project with BTC**: *bc1q0cxl5j3se0ufhr96h8x0zs8nz4t7h6krrxkd6l*
 
 [Documentation](https://dmitriiweb.github.io/extract-emails/)
 
 ## Requirements
-- Python >= 3.9
+
+- Python >= 3.10
 
 ## Installation
+
 ```bash
 pip install extract_emails[all]
 # or
 pip install extract_emails[requests]
 # or
 pip install extract_emails[selenium]
 ```
 
 ## Simple Usage
+
 ### As library
+
 ```python
 from pathlib import Path
 
 from extract_emails import DefaultFilterAndEmailFactory as Factory
 from extract_emails import DefaultWorker
 from extract_emails.browsers.requests_browser import RequestsBrowser as Browser
 from extract_emails.data_savers import CsvSaver
@@ -79,17 +82,25 @@
     factory = Factory(
         website_url=website, browser=browser, depth=5, max_links_from_page=1
     )
     worker = DefaultWorker(factory)
     data = worker.get_data()
     data_saver.save(data)
 ```
+
 ### As CLI tool
+
 ```bash
 $ extract-emails --help
 
 $ extract-emails --url https://en.wikipedia.org/wiki/Email -of output.csv -d 1
 $ cat output.csv
 email,page,website
 bob@b.org,https://en.wikipedia.org/wiki/Email,https://en.wikipedia.org/wiki/Email
 ```
 
+### By me a coffee
+
+- **USDT** (TRC20): TXuYegp5L8Zf7wF2YRFjskZwdBxhRpvxBS
+- **BEP20**: 0x4D51Db2B754eA83ce228F7de8EaEB93a88bdC965
+- **TON**: UQA5quJljQz84RwzteN3uuKsdPTDee7a_GF5lgIgezA2oib5
+
```

