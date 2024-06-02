# Comparing `tmp/selenium_assist-0.3.4.tar.gz` & `tmp/selenium_assist-0.3.5.tar.gz`

## Comparing `selenium_assist-0.3.4.tar` & `selenium_assist-0.3.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/usage.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/.idea/.gitignore
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/.idea/misc.xml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/.idea/modules.xml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/.idea/selenium-assist.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/.idea/vcs.xml
--rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/.idea/workspace.xml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/src/selenium_assist/__init__.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/src/selenium_assist/helpers.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/src/selenium_assist/managers.py
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/src/selenium_assist/wrappers.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/LICENSE
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 selenium_assist-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/usage.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/.idea/.gitignore
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/.idea/misc.xml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/.idea/modules.xml
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/.idea/selenium-assist.iml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/.idea/selenium-helpers.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/.idea/vcs.xml
+-rw-r--r--   0        0        0    24453 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/src/selenium_assist/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/src/selenium_assist/helpers.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/src/selenium_assist/managers.py
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/src/selenium_assist/wrappers.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 selenium_assist-0.3.5/PKG-INFO
```

### Comparing `selenium_assist-0.3.4/usage.md` & `selenium_assist-0.3.5/usage.md`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.3.4/src/selenium_assist/helpers.py` & `selenium_assist-0.3.5/src/selenium_assist/helpers.py`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.3.4/src/selenium_assist/managers.py` & `selenium_assist-0.3.5/src/selenium_assist/managers.py`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.3.4/src/selenium_assist/wrappers.py` & `selenium_assist-0.3.5/src/selenium_assist/wrappers.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,91 +6,112 @@
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import ElementClickInterceptedException
 from selenium.common.exceptions import StaleElementReferenceException
 from selenium.webdriver.common.action_chains import ActionChains
 
 
-def load_page(task, url, driver, continue_on_error=False):
+def load_page(task, url, driver, continue_on_error=False, silence_warning=False):
     logging.debug(task)
     try:
         driver.get(url)
     except Exception as e:
         if not continue_on_error:
             dump_and_exit(
                 "Cannot load webpage, dumping source and exiting!", driver, exc=e
             )
         else:
-            logging.warning("Cannot load webpage, continuing ...")
+            if not silence_warning:
+                logging.warning("Cannot load webpage, continuing ...")
     return
 
 
 def wait_for_presence(
-    task, xpath, driver, timeout=60, extra_timeout=0, continue_on_error=False
+    task,
+    xpath,
+    driver,
+    timeout=60,
+    extra_timeout=0,
+    continue_on_error=False,
+    silence_warning=False,
 ):
     logging.debug(task)
     try:
         element_present = EC.presence_of_element_located((By.XPATH, xpath))
         WebDriverWait(driver, timeout).until(element_present)
         time.sleep(extra_timeout)
     except TimeoutException:
         if not continue_on_error:
             dump_and_exit(
                 f"Timed out waiting for element presence ({xpath}), dumping source and exiting!",
                 driver,
             )
         else:
-            logging.warning(
-                f"Timed out waiting for element presence ({xpath}), continuing ..."
-            )
+            if not silence_warning:
+                logging.warning(
+                    f"Timed out waiting for element presence ({xpath}), continuing ..."
+                )
     return
 
 
 def wait_for_visibility(
-    task, xpath, driver, timeout=60, extra_timeout=3, continue_on_error=False
+    task,
+    xpath,
+    driver,
+    timeout=60,
+    extra_timeout=3,
+    continue_on_error=False,
+    silence_warning=False,
 ):
     logging.debug(task)
     try:
         element_present = EC.visibility_of_element_located((By.XPATH, xpath))
         WebDriverWait(driver, timeout).until(element_present)
         time.sleep(extra_timeout)
     except TimeoutException:
         if not continue_on_error:
             dump_and_exit(
                 "Timed out waiting for element visibility, dumping source and exiting!",
                 driver,
             )
         else:
-            logging.warning("Timed out waiting for element visibility, continuing ...")
+            if not silence_warning:
+                logging.warning(
+                    "Timed out waiting for element visibility, continuing ..."
+                )
     return
 
 
-def click_element(task, xpath, driver, extra_timeout=0, continue_on_error=False):
+def click_element(
+    task, xpath, driver, extra_timeout=0, continue_on_error=False, silence_warning=False
+):
     logging.debug(task)
     try:
         driver.find_element(By.XPATH, xpath).click()
         time.sleep(extra_timeout)
     except (ElementClickInterceptedException, StaleElementReferenceException):
         if not continue_on_error:
             dump_and_exit(
                 "Cannot click on element, dumping source and exiting!", driver
             )
         else:
-            logging.warning("Cannot click on element, continuing ...")
+            if not silence_warning:
+                logging.warning("Cannot click on element, continuing ...")
     return
 
 
 def send_keys(
     task,
     xpath,
     keys,
     driver,
     extra_timeout=5,
     skip_check=False,
     continue_on_error=False,
+    silence_warning=False,
 ):
     logging.debug(task)
     try:
         element_present = EC.element_to_be_clickable((By.XPATH, xpath))
         WebDriverWait(driver, extra_timeout).until(element_present)
         element = driver.find_element(By.XPATH, xpath)
         element.clear()
@@ -103,91 +124,110 @@
         if not continue_on_error:
             dump_and_exit(
                 "Cannot send keys on element, dumping source and exiting!",
                 driver,
                 exc=e,
             )
         else:
-            logging.warning("Cannot send keys on element, continuing ...")
+            if not silence_warning:
+                logging.warning("Cannot send keys on element, continuing ...")
     return
 
 
-def hoover_over_element(task, xpath, driver, continue_on_error=False):
+def hoover_over_element(
+    task, xpath, driver, continue_on_error=False, silence_warning=False
+):
     logging.debug(task)
     try:
         element = driver.find_element(By.XPATH, xpath)
         action = ActionChains(driver)
         action.move_to_element(element).perform()
     except Exception as e:
         if not continue_on_error:
             dump_and_exit(
                 "Cannot hoover over element, dumping source and exiting!", driver, exc=e
             )
         else:
-            logging.warning("Cannot hoover over element, continuing ...")
+            if not silence_warning:
+                logging.warning("Cannot hoover over element, continuing ...")
     return
 
 
 def switch_to_iframe(
-    task, xpath, driver, timeout=60, extra_timeout=0, continue_on_error=False
+    task,
+    xpath,
+    driver,
+    timeout=60,
+    extra_timeout=0,
+    continue_on_error=False,
+    silence_warning=False,
 ):
     logging.debug(task)
     try:
         element_present = EC.frame_to_be_available_and_switch_to_it((By.XPATH, xpath))
         WebDriverWait(driver, timeout).until(element_present)
         time.sleep(extra_timeout)
     except TimeoutException:
         if not continue_on_error:
             dump_and_exit(
                 "Timed out switching to iframe, dumping source and exiting!", driver
             )
         else:
-            logging.warning("Timed out switching to iframe, continuing ...")
+            if not silence_warning:
+                logging.warning("Timed out switching to iframe, continuing ...")
     return
 
 
-def get_table_data(task, xpath, driver, continue_on_error=False):
+def get_table_data(task, xpath, driver, continue_on_error=False, silence_warning=False):
     logging.debug(task)
     data = []
     try:
         for tr in driver.find_elements(By.XPATH, xpath + "//tr"):
             tds = tr.find_elements(By.TAG_NAME, "td")
             if tds:
                 data.append([td.text for td in tds])
     except Exception as e:
         if not continue_on_error:
             dump_and_exit(
                 "Cannot get table data, dumping source and exiting!", driver, exc=e
             )
         else:
-            logging.warning("Cannot get table data, continuing ...")
+            if not silence_warning:
+                logging.warning("Cannot get table data, continuing ...")
     return data
 
 
-def get_element_text(task, xpath, driver, continue_on_error=False):
+def get_element_text(
+    task, xpath, driver, continue_on_error=False, silence_warning=False
+):
     logging.debug(task)
     data = ""
     try:
         data = driver.find_element(By.XPATH, xpath).text
     except Exception as e:
         if not continue_on_error:
             dump_and_exit(
                 "Cannot get element text, dumping source and exiting!", driver, exc=e
             )
         else:
-            logging.warning("Cannot get element text, continuing ...")
+            if not silence_warning:
+                logging.warning("Cannot get element text, continuing ...")
     return data
 
-def execute_script(task, xpath, script, driver, continue_on_error=False):
+
+def execute_script(
+    task, xpath, script, driver, continue_on_error=False, silence_warning=False
+):
     logging.debug(task)
     data = ""
     try:
         data = driver.find_element(By.XPATH, xpath)
         driver.execute_script(script, data)
     except Exception as e:
         if not continue_on_error:
             dump_and_exit(
                 'Cannot execute script "{}", dumping source and exiting!', driver, exc=e
             )
         else:
-            logging.warning('Cannot execute script "{}", continuing ...')
+            if not silence_warning:
+                logging.warning('Cannot execute script "{}", continuing ...')
     return data
```

### Comparing `selenium_assist-0.3.4/.gitignore` & `selenium_assist-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.3.4/LICENSE` & `selenium_assist-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.3.4/README.md` & `selenium_assist-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `selenium_assist-0.3.4/pyproject.toml` & `selenium_assist-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "selenium_assist"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
     { name="Ivan Mičetić", email="ivan.micetic@gmail.com" },
 ]
 description = "Helper functions for Selenium"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `selenium_assist-0.3.4/PKG-INFO` & `selenium_assist-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: selenium_assist
-Version: 0.3.4
+Version: 0.3.5
 Summary: Helper functions for Selenium
 Project-URL: Homepage, https://github.com/ivanmicetic/selenium-assist
 Project-URL: Bug Tracker, https://github.com/ivanmicetic/selenium-assist/issues
 Author-email: Ivan Mičetić <ivan.micetic@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

