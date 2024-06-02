# Comparing `tmp/tweeterpy-1.1.4.tar.gz` & `tmp/tweeterpy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeterpy-1.1.4.tar", last modified: Sat May 25 09:13:02 2024, max compression
+gzip compressed data, was "tweeterpy-1.1.5.tar", last modified: Sun Jun  2 12:30:32 2024, max compression
```

## Comparing `tweeterpy-1.1.4.tar` & `tweeterpy-1.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 09:13:02.631258 tweeterpy-1.1.4/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-1.1.4/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3967 2024-05-25 09:13:02.631258 tweeterpy-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2530 2023-10-11 13:44:39.000000 tweeterpy-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-25 09:13:02.631258 tweeterpy-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1499 2024-05-25 08:47:45.000000 tweeterpy-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:13:02.599992 tweeterpy-1.1.4/tweeterpy/
--rw-rw-rw-   0        0        0       34 2023-09-16 06:13:29.000000 tweeterpy-1.1.4/tweeterpy/__init__.py
--rw-rw-rw-   0        0        0     8361 2024-05-24 13:19:12.000000 tweeterpy-1.1.4/tweeterpy/api_util.py
--rw-rw-rw-   0        0        0     2428 2024-05-24 13:19:24.000000 tweeterpy-1.1.4/tweeterpy/config.py
--rw-rw-rw-   0        0        0     3855 2024-05-17 15:23:46.000000 tweeterpy-1.1.4/tweeterpy/constants.py
--rw-rw-rw-   0        0        0     2058 2023-09-09 11:19:04.000000 tweeterpy-1.1.4/tweeterpy/logging_util.py
--rw-rw-rw-   0        0        0     9250 2024-05-24 13:21:29.000000 tweeterpy-1.1.4/tweeterpy/login_util.py
--rw-rw-rw-   0        0        0     2126 2024-05-24 13:38:49.000000 tweeterpy-1.1.4/tweeterpy/request_util.py
--rw-rw-rw-   0        0        0     2462 2024-05-24 13:32:11.000000 tweeterpy-1.1.4/tweeterpy/session_util.py
--rw-rw-rw-   0        0        0    32899 2024-05-25 08:44:57.000000 tweeterpy-1.1.4/tweeterpy/tweeterpy.py
--rw-rw-rw-   0        0        0    16546 2024-05-18 07:23:11.000000 tweeterpy-1.1.4/tweeterpy/util.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:13:02.615638 tweeterpy-1.1.4/tweeterpy.egg-info/
--rw-rw-rw-   0        0        0     3967 2024-05-25 09:13:02.000000 tweeterpy-1.1.4/tweeterpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-05-25 09:13:02.000000 tweeterpy-1.1.4/tweeterpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 09:13:02.000000 tweeterpy-1.1.4/tweeterpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2024-05-25 09:13:02.000000 tweeterpy-1.1.4/tweeterpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-25 09:13:02.000000 tweeterpy-1.1.4/tweeterpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 12:30:32.216671 tweeterpy-1.1.5/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3715 2024-06-02 12:30:32.210443 tweeterpy-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2530 2023-10-11 13:44:39.000000 tweeterpy-1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 12:30:32.217972 tweeterpy-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2024-06-02 12:26:42.000000 tweeterpy-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:30:32.175541 tweeterpy-1.1.5/tweeterpy/
+-rw-rw-rw-   0        0        0       34 2023-09-16 06:13:29.000000 tweeterpy-1.1.5/tweeterpy/__init__.py
+-rw-rw-rw-   0        0        0     8361 2024-05-26 12:46:58.000000 tweeterpy-1.1.5/tweeterpy/api_util.py
+-rw-rw-rw-   0        0        0     2428 2024-05-26 12:47:02.000000 tweeterpy-1.1.5/tweeterpy/config.py
+-rw-rw-rw-   0        0        0     3855 2024-05-17 15:23:46.000000 tweeterpy-1.1.5/tweeterpy/constants.py
+-rw-rw-rw-   0        0        0     2058 2023-09-09 11:19:04.000000 tweeterpy-1.1.5/tweeterpy/logging_util.py
+-rw-rw-rw-   0        0        0     9250 2024-05-26 10:31:08.000000 tweeterpy-1.1.5/tweeterpy/login_util.py
+-rw-rw-rw-   0        0        0     2126 2024-05-26 09:52:55.000000 tweeterpy-1.1.5/tweeterpy/request_util.py
+-rw-rw-rw-   0        0        0     2462 2024-05-24 13:32:11.000000 tweeterpy-1.1.5/tweeterpy/session_util.py
+-rw-rw-rw-   0        0        0    32899 2024-05-26 12:47:09.000000 tweeterpy-1.1.5/tweeterpy/tweeterpy.py
+-rw-rw-rw-   0        0        0    16490 2024-06-02 12:04:12.000000 tweeterpy-1.1.5/tweeterpy/util.py
+drwxrwxrwx   0        0        0        0 2024-06-02 12:30:32.210443 tweeterpy-1.1.5/tweeterpy.egg-info/
+-rw-rw-rw-   0        0        0     3715 2024-06-02 12:30:31.000000 tweeterpy-1.1.5/tweeterpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-06-02 12:30:31.000000 tweeterpy-1.1.5/tweeterpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 12:30:31.000000 tweeterpy-1.1.5/tweeterpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-06-02 12:30:31.000000 tweeterpy-1.1.5/tweeterpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-02 12:30:31.000000 tweeterpy-1.1.5/tweeterpy.egg-info/top_level.txt
```

### Comparing `tweeterpy-1.1.4/LICENSE` & `tweeterpy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.4/PKG-INFO` & `tweeterpy-1.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 1.1.4
+Version: 1.1.5
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
@@ -16,25 +16,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.2
-Requires-Dist: Brotli==1.0.9
-Requires-Dist: bs4==0.0.1
-Requires-Dist: certifi==2023.7.22
-Requires-Dist: charset-normalizer==3.1.0
 Requires-Dist: demjson3==3.0.6
-Requires-Dist: idna==3.7
 Requires-Dist: lxml==5.2.2
 Requires-Dist: requests==2.32.2
-Requires-Dist: six==1.16.0
-Requires-Dist: soupsieve==2.4.1
-Requires-Dist: urllib3==2.0.7
 
 <h1 align="center">TweeterPy</h1>
 
 <p align="center">
 <a href="https://choosealicense.com/licenses/mit/"> <img src="https://img.shields.io/badge/License-MIT-green.svg"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tweeterpy"></a>
 <a href="https://pypi.org/project/tweeterpy/"> <img src="https://img.shields.io/pypi/v/tweeterpy"></a>
```

#### html2text {}

```diff
@@ -1,26 +1,23 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.4 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.5 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix Classifier: License :: OSI Approved :: MIT
 License Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: beautifulsoup4==4.12.2
-Requires-Dist: Brotli==1.0.9 Requires-Dist: bs4==0.0.1 Requires-Dist:
-certifi==2023.7.22 Requires-Dist: charset-normalizer==3.1.0 Requires-Dist:
-demjson3==3.0.6 Requires-Dist: idna==3.7 Requires-Dist: lxml==5.2.2 Requires-
-Dist: requests==2.32.2 Requires-Dist: six==1.16.0 Requires-Dist:
-soupsieve==2.4.1 Requires-Dist: urllib3==2.0.7
+Requires-Dist: demjson3==3.0.6 Requires-Dist: lxml==5.2.2 Requires-Dist:
+requests==2.32.2
                             ************ TTwweeeetteerrPPyy ************
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_g_r_e_e_n_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
  _p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_t_w_e_e_t_e_r_p_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_w_e_e_t_e_r_p_y_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_i_S_a_r_a_b_j_i_t_D_h_i_m_a_n_/_T_w_e_e_t_e_r_P_y_]_[_D_i_s_c_o_r_d_]_[_h_t_t_p_s_:_/_/
     _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/_i_S_a_r_a_b_j_i_t_D_h_i_m_a_n_?_s_t_y_l_e_=_s_o_c_i_a_l_]## Overview
 TweeterPy is a python library to extract data from Twitter. TweeterPy API lets
  you scrape data from a user's profile like username, userid, bio, followers/
```

### Comparing `tweeterpy-1.1.4/README.md` & `tweeterpy-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.4/setup.py` & `tweeterpy-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "1.1.4"
+VERSION = "1.1.5"
 SHORT_DESCRIPTION = "TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

### Comparing `tweeterpy-1.1.4/tweeterpy/api_util.py` & `tweeterpy-1.1.5/tweeterpy/api_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.4/tweeterpy/config.py` & `tweeterpy-1.1.5/tweeterpy/config.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.4/tweeterpy/constants.py` & `tweeterpy-1.1.5/tweeterpy/constants.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.4/tweeterpy/logging_util.py` & `tweeterpy-1.1.5/tweeterpy/logging_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.4/tweeterpy/login_util.py` & `tweeterpy-1.1.5/tweeterpy/login_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.4/tweeterpy/request_util.py` & `tweeterpy-1.1.5/tweeterpy/request_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.4/tweeterpy/session_util.py` & `tweeterpy-1.1.5/tweeterpy/session_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.4/tweeterpy/tweeterpy.py` & `tweeterpy-1.1.5/tweeterpy/tweeterpy.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-1.1.4/tweeterpy/util.py` & `tweeterpy-1.1.5/tweeterpy/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         if message is None:
             message = "API rate limit exhausted."
         super().__init__(message)
 
 
 def generate_headers(session=None, custom_headers=None):
     headers = {"Authority": Path.DOMAIN,
-               "Accept-Encoding": "gzip, deflate, br",
                "Accept-Language": "en-US,en;q=0.9",
                "Cache-Control": "no-cache",
                "Referer": Path.BASE_URL,
                "User-Agent": config._USER_AGENT,
                "X-Twitter-Active-User": "yes",
                "X-Twitter-Client-Language": "en"
                }
```

### Comparing `tweeterpy-1.1.4/tweeterpy.egg-info/PKG-INFO` & `tweeterpy-1.1.5/tweeterpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 1.1.4
+Version: 1.1.5
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
@@ -16,25 +16,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.2
-Requires-Dist: Brotli==1.0.9
-Requires-Dist: bs4==0.0.1
-Requires-Dist: certifi==2023.7.22
-Requires-Dist: charset-normalizer==3.1.0
 Requires-Dist: demjson3==3.0.6
-Requires-Dist: idna==3.7
 Requires-Dist: lxml==5.2.2
 Requires-Dist: requests==2.32.2
-Requires-Dist: six==1.16.0
-Requires-Dist: soupsieve==2.4.1
-Requires-Dist: urllib3==2.0.7
 
 <h1 align="center">TweeterPy</h1>
 
 <p align="center">
 <a href="https://choosealicense.com/licenses/mit/"> <img src="https://img.shields.io/badge/License-MIT-green.svg"></a>
 <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tweeterpy"></a>
 <a href="https://pypi.org/project/tweeterpy/"> <img src="https://img.shields.io/pypi/v/tweeterpy"></a>
```

#### html2text {}

```diff
@@ -1,26 +1,23 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.4 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 1.1.5 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix Classifier: License :: OSI Approved :: MIT
 License Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: beautifulsoup4==4.12.2
-Requires-Dist: Brotli==1.0.9 Requires-Dist: bs4==0.0.1 Requires-Dist:
-certifi==2023.7.22 Requires-Dist: charset-normalizer==3.1.0 Requires-Dist:
-demjson3==3.0.6 Requires-Dist: idna==3.7 Requires-Dist: lxml==5.2.2 Requires-
-Dist: requests==2.32.2 Requires-Dist: six==1.16.0 Requires-Dist:
-soupsieve==2.4.1 Requires-Dist: urllib3==2.0.7
+Requires-Dist: demjson3==3.0.6 Requires-Dist: lxml==5.2.2 Requires-Dist:
+requests==2.32.2
                             ************ TTwweeeetteerrPPyy ************
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_g_r_e_e_n_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
  _p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_t_w_e_e_t_e_r_p_y_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_t_w_e_e_t_e_r_p_y_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_i_S_a_r_a_b_j_i_t_D_h_i_m_a_n_/_T_w_e_e_t_e_r_P_y_]_[_D_i_s_c_o_r_d_]_[_h_t_t_p_s_:_/_/
     _i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/_i_S_a_r_a_b_j_i_t_D_h_i_m_a_n_?_s_t_y_l_e_=_s_o_c_i_a_l_]## Overview
 TweeterPy is a python library to extract data from Twitter. TweeterPy API lets
  you scrape data from a user's profile like username, userid, bio, followers/
```

