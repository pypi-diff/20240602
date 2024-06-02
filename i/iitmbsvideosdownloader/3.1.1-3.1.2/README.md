# Comparing `tmp/iitmbsvideosdownloader-3.1.1.tar.gz` & `tmp/iitmbsvideosdownloader-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitmbsvideosdownloader-3.1.1.tar", max compression
+gzip compressed data, was "iitmbsvideosdownloader-3.1.2.tar", max compression
```

## Comparing `iitmbsvideosdownloader-3.1.1.tar` & `iitmbsvideosdownloader-3.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     2315 2024-05-31 19:38:06.899649 iitmbsvideosdownloader-3.1.1/README.md
--rwxr-xr-x   0        0        0      348 2024-05-31 19:37:11.188183 iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/SITES.py
--rwxr-xr-x   0        0        0     3893 2024-05-31 19:37:11.192898 iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/SUBJECTS.py
--rw-r--r--   0        0        0        0 2024-05-31 19:32:49.869345 iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/__init__.py
--rwxr-xr-x   0        0        0     8370 2024-05-31 19:37:11.171208 iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/_downloader.py
--rwxr-xr-x   0        0        0     7943 2024-05-31 19:37:11.179558 iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/_functions.py
--rwxr-xr-x   0        0        0     6109 2024-05-31 19:37:11.182448 iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/_iitm.py
--rwxr-xr-x   0        0        0     7281 2024-05-31 19:37:11.185141 iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/iitmbsvideosdownloader.py
--rw-r--r--   0        0        0      364 2024-05-31 20:33:30.656971 iitmbsvideosdownloader-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 iitmbsvideosdownloader-3.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     2840 2024-05-31 20:39:57.140300 iitmbsvideosdownloader-3.1.2/README.md
+-rwxr-xr-x   0        0        0      348 2024-05-31 19:37:11.188183 iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/SITES.py
+-rwxr-xr-x   0        0        0     4029 2024-06-02 13:25:07.899477 iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/SUBJECTS.py
+-rw-r--r--   0        0        0        0 2024-05-31 19:32:49.869345 iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/__init__.py
+-rwxr-xr-x   0        0        0     8370 2024-05-31 19:37:11.171208 iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/_downloader.py
+-rwxr-xr-x   0        0        0     7943 2024-05-31 19:37:11.179558 iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/_functions.py
+-rwxr-xr-x   0        0        0     6109 2024-05-31 19:37:11.182448 iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/_iitm.py
+-rwxr-xr-x   0        0        0     7281 2024-05-31 19:37:11.185141 iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/iitmbsvideosdownloader.py
+-rw-r--r--   0        0        0      364 2024-06-02 13:21:29.185162 iitmbsvideosdownloader-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3369 1970-01-01 00:00:00.000000 iitmbsvideosdownloader-3.1.2/PKG-INFO
```

### Comparing `iitmbsvideosdownloader-3.1.1/README.md` & `iitmbsvideosdownloader-3.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,90 @@
+
+
 IITM BS Videos Downloader
 ===============
 Python Bot Library to download IITM BS videos.
 
+
 Installing
 ============
+[Visit step by step guide to installation](https://drive.google.com/file/d/17R6Jt01sYyVlmPfkB0dUMLwxjYnHKzTs/view?usp=sharing)
 
 ```bash
 pip install iitmbsvideosdownloader
 ```
 
-Usage
-=====
+## How it Works?
+
+The bot is basically a Python Package. It opens the browser then gets videos links from portal and goes to third party sites like Y2mate and downloads videos one by one.
+
+So just one click and all the boring stuff regarding downloading videos bot can handle.
+
+
+
+## Features
 
-Example for Windows
+- Auto Retries if failed to download a video
+- Skips videos if already downloaded
+- Renames videos to the names written on Portal (ex: L1.2 - )
+- Other tasks can be done on PC while it's running
+
+
+
+### Tools required
+
+- Python Setup
+- IDE for Python (PyCharm, Spyder etc)
+- Brave Browser
+
+
+### Example for Windows
 
 ```python
-from iitmbsvideosdownloader import SUBJECTS, iitmbsvideosdownloader
+from iitmbsvideosdownloader import SUBJECTS, SITES, iitmbsvideosdownloader
 
 mySmartBot = iitmbsvideosdownloader.SmartBot(
-    browser_path="C:\\Program Files\\BraveSoftware\\Brave-Browser\\Application\\brave.exe",
-    download_path="D:\\Term 7",
-    user_data_path="C:\\Users\\Shekh\\AppData\\Local\\BraveSoftware\\Brave-Browser\\User Data",
-    profile_name="Default",
+    executable_path=r"C:\Program Files\BraveSoftware\Brave-Browser\Application\brave.exe",
+    profile_path=r"C:\Users\Shekh\AppData\Local\BraveSoftware\Brave-Browser\User Data\Default",
+    download_path=r"D:\Term 8",
     subjects=[
         SUBJECTS.AI_SEARCH_METHODS_FOR_PROBLEM_SOLVING,
         SUBJECTS.DEEP_LEARNING,
         SUBJECTS.SOFTWARE_ENGINEERING,
         SUBJECTS.STRATEGIES_FOR_PROFESSIONAL_GROWTH
     ],
-    year=23,
-    term=1,
-    week=4,
+    year=2023,
+    term=2,
+    week=1,
 )
 
 mySmartBot.start()
 ```
 
 In the Code:
 
-**browser_path**: path of the browser
+**executable_path**: path of the browser
 
-**download_path**: where you want to save all the bot's work, huh?
+**profile_path**: browsers save user's data at a specific location, please provide that here.
 
-**user_data_path**: browsers save user's data at a specific location, please provide that here.
-
-**profile_name**: in the user_data_path you will have folders dedicated to your profiles, if you have only one profile in browser setting it to "Default"  works
+**download_path**: where you want to save all the bot's downloaded videos, set the directory location here.
 
 **subjects**: use SUBJECTS module to provide a list of your subjects
 
-**year**: two digit integer that tells current year
+**year**: current year
 
 **term**: one digit integer that tells current term (1 for Jan Term, 2 for May Term, 3 for Sep Term)
 
 **week**: current week, so bot knows which week to download
 
 
 
-## Essential Steps
+## Install using pip
 
-1) make sure you are logged in to your browser(Brave recommended) on any of the course (on seek portal) and if already logged in then close the browser
+1) make sure you are logged in to your Brave browser on any of the course (on seek portal) and if already logged in then close the browser
 2) install the library using pip
 3) paste the code above in Python Environment (PyCharm recommended)
 4) change the code as per your system and needs
 5) Run it and let the bot do it's work.
 
 
 
@@ -85,7 +107,8 @@
 Did this package helped you save some time? or any suggestions?
 
 Contact - 
 
 Savindra Singh Shekhawat
 
 shekhawatsavindra@gmail.com
+
```

### Comparing `iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/SUBJECTS.py` & `iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/SUBJECTS.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,9 +52,9 @@
 MARKET_RESEARCH = _Subject("Market Research", "ms3002")
 INDUSTRY_4_0 = _Subject("Industry 4_0", "ms4001")
 
 MATHEMATICAL_THINKING = _Subject("Mathematical Thinking", "ma2001")
 INTRODUCTION_TO_BIG_DATA = _Subject("Introduction to Big Data", "cs4004")
 SPECIAL_TOPICS_IN_MACHINE_LEARNING_REINFORCEMENT_LEARNING = _Subject(
     "Special topics in Machine Learning (Reinforcement Learning)", "cs4002")
-
-
+MANAGERIAL_ECONOMICS = _Subject("Managerial Economics", "ms3033")
+GAME_THEORY_AND_STRATEGY = _Subject("Game Theory and Strategy", "ms4023")
```

### Comparing `iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/_downloader.py` & `iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/_downloader.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/_functions.py` & `iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/_functions.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/_iitm.py` & `iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/_iitm.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-3.1.1/iitmbsvideosdownloader/iitmbsvideosdownloader.py` & `iitmbsvideosdownloader-3.1.2/iitmbsvideosdownloader/iitmbsvideosdownloader.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-3.1.1/PKG-INFO` & `iitmbsvideosdownloader-3.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,105 @@
 Metadata-Version: 2.1
 Name: iitmbsvideosdownloader
-Version: 3.1.1
+Version: 3.1.2
 Summary: 
 Author: SavindraSinghShekhawat
 Author-email: shekhawatsavindra@gmail.com
 Requires-Python: >=3.9.6,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chromedriver-autoinstaller-fix (>=1.0.6,<2.0.0)
 Requires-Dist: selenium (>=4.21.0,<5.0.0)
 Description-Content-Type: text/markdown
 
+
+
 IITM BS Videos Downloader
 ===============
 Python Bot Library to download IITM BS videos.
 
+
 Installing
 ============
+[Visit step by step guide to installation](https://drive.google.com/file/d/17R6Jt01sYyVlmPfkB0dUMLwxjYnHKzTs/view?usp=sharing)
 
 ```bash
 pip install iitmbsvideosdownloader
 ```
 
-Usage
-=====
+## How it Works?
+
+The bot is basically a Python Package. It opens the browser then gets videos links from portal and goes to third party sites like Y2mate and downloads videos one by one.
+
+So just one click and all the boring stuff regarding downloading videos bot can handle.
+
+
+
+## Features
 
-Example for Windows
+- Auto Retries if failed to download a video
+- Skips videos if already downloaded
+- Renames videos to the names written on Portal (ex: L1.2 - )
+- Other tasks can be done on PC while it's running
+
+
+
+### Tools required
+
+- Python Setup
+- IDE for Python (PyCharm, Spyder etc)
+- Brave Browser
+
+
+### Example for Windows
 
 ```python
-from iitmbsvideosdownloader import SUBJECTS, iitmbsvideosdownloader
+from iitmbsvideosdownloader import SUBJECTS, SITES, iitmbsvideosdownloader
 
 mySmartBot = iitmbsvideosdownloader.SmartBot(
-    browser_path="C:\\Program Files\\BraveSoftware\\Brave-Browser\\Application\\brave.exe",
-    download_path="D:\\Term 7",
-    user_data_path="C:\\Users\\Shekh\\AppData\\Local\\BraveSoftware\\Brave-Browser\\User Data",
-    profile_name="Default",
+    executable_path=r"C:\Program Files\BraveSoftware\Brave-Browser\Application\brave.exe",
+    profile_path=r"C:\Users\Shekh\AppData\Local\BraveSoftware\Brave-Browser\User Data\Default",
+    download_path=r"D:\Term 8",
     subjects=[
         SUBJECTS.AI_SEARCH_METHODS_FOR_PROBLEM_SOLVING,
         SUBJECTS.DEEP_LEARNING,
         SUBJECTS.SOFTWARE_ENGINEERING,
         SUBJECTS.STRATEGIES_FOR_PROFESSIONAL_GROWTH
     ],
-    year=23,
-    term=1,
-    week=4,
+    year=2023,
+    term=2,
+    week=1,
 )
 
 mySmartBot.start()
 ```
 
 In the Code:
 
-**browser_path**: path of the browser
+**executable_path**: path of the browser
 
-**download_path**: where you want to save all the bot's work, huh?
+**profile_path**: browsers save user's data at a specific location, please provide that here.
 
-**user_data_path**: browsers save user's data at a specific location, please provide that here.
-
-**profile_name**: in the user_data_path you will have folders dedicated to your profiles, if you have only one profile in browser setting it to "Default"  works
+**download_path**: where you want to save all the bot's downloaded videos, set the directory location here.
 
 **subjects**: use SUBJECTS module to provide a list of your subjects
 
-**year**: two digit integer that tells current year
+**year**: current year
 
 **term**: one digit integer that tells current term (1 for Jan Term, 2 for May Term, 3 for Sep Term)
 
 **week**: current week, so bot knows which week to download
 
 
 
-## Essential Steps
+## Install using pip
 
-1) make sure you are logged in to your browser(Brave recommended) on any of the course (on seek portal) and if already logged in then close the browser
+1) make sure you are logged in to your Brave browser on any of the course (on seek portal) and if already logged in then close the browser
 2) install the library using pip
 3) paste the code above in Python Environment (PyCharm recommended)
 4) change the code as per your system and needs
 5) Run it and let the bot do it's work.
 
 
 
@@ -101,7 +123,8 @@
 
 Contact - 
 
 Savindra Singh Shekhawat
 
 shekhawatsavindra@gmail.com
 
+
```

