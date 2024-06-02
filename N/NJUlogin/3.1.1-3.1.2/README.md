# Comparing `tmp/NJUlogin-3.1.1.tar.gz` & `tmp/NJUlogin-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NJUlogin-3.1.1.tar", last modified: Tue Nov 21 02:25:51 2023, max compression
+gzip compressed data, was "NJUlogin-3.1.2.tar", last modified: Sun Jun  2 15:49:34 2024, max compression
```

## Comparing `NJUlogin-3.1.1.tar` & `NJUlogin-3.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-11-21 02:25:51.478915 NJUlogin-3.1.1/
--rw-rw-rw-   0        0        0     1082 2022-11-04 13:26:44.000000 NJUlogin-3.1.1/LICENSE
--rw-rw-rw-   0        0        0       41 2023-11-15 02:56:13.000000 NJUlogin-3.1.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-11-21 02:25:51.405503 NJUlogin-3.1.1/NJUlogin/
--rw-rw-rw-   0        0        0     5014 2023-08-12 03:03:44.000000 NJUlogin-3.1.1/NJUlogin/QRlogin.py
--rw-rw-rw-   0        0        0      221 2022-11-07 11:22:45.000000 NJUlogin-3.1.1/NJUlogin/__init__.py
--rw-rw-rw-   0        0        0      292 2023-11-21 02:16:43.000000 NJUlogin-3.1.1/NJUlogin/__version__.py
--rw-rw-rw-   0        0        0     1286 2023-02-06 05:06:02.000000 NJUlogin-3.1.1/NJUlogin/_base_.py
-drwxrwxrwx   0        0        0        0 2023-11-21 02:25:51.462401 NJUlogin-3.1.1/NJUlogin/captchaOCR/
--rw-rw-rw-   0        0        0       29 2023-11-15 02:29:03.000000 NJUlogin-3.1.1/NJUlogin/captchaOCR/__init__.py
--rw-rw-rw-   0        0        0    67670 2023-11-15 02:32:08.000000 NJUlogin-3.1.1/NJUlogin/captchaOCR/charsets.py
--rw-rw-rw-   0        0        0 13606198 2023-08-08 13:15:06.000000 NJUlogin-3.1.1/NJUlogin/captchaOCR/common.onnx
--rw-rw-rw-   0        0        0     4757 2023-11-15 02:41:30.000000 NJUlogin-3.1.1/NJUlogin/captchaOCR/ocr.py
--rw-rw-rw-   0        0        0      353 2023-08-11 13:09:46.000000 NJUlogin-3.1.1/NJUlogin/captchaOCR/utils.py
--rw-rw-rw-   0        0        0     4070 2023-11-15 02:28:45.000000 NJUlogin-3.1.1/NJUlogin/pwdLogin.py
-drwxrwxrwx   0        0        0        0 2023-11-21 02:25:51.471473 NJUlogin-3.1.1/NJUlogin/utils/
--rw-rw-rw-   0        0        0       15 2022-11-04 09:03:44.000000 NJUlogin-3.1.1/NJUlogin/utils/__init__.py
--rw-rw-rw-   0        0        0       81 2022-11-04 07:34:30.000000 NJUlogin-3.1.1/NJUlogin/utils/clear.py
--rw-rw-rw-   0        0        0      250 2023-08-12 02:52:33.000000 NJUlogin-3.1.1/NJUlogin/utils/config.py
--rw-rw-rw-   0        0        0      858 2023-03-05 02:48:50.000000 NJUlogin-3.1.1/NJUlogin/utils/get_post.py
--rw-rw-rw-   0        0        0      652 2023-03-03 16:25:08.000000 NJUlogin-3.1.1/NJUlogin/utils/urls.py
-drwxrwxrwx   0        0        0        0 2023-11-21 02:25:51.418032 NJUlogin-3.1.1/NJUlogin.egg-info/
--rw-rw-rw-   0        0        0     2271 2023-11-21 02:25:51.000000 NJUlogin-3.1.1/NJUlogin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-11-21 02:25:51.000000 NJUlogin-3.1.1/NJUlogin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-21 02:25:51.000000 NJUlogin-3.1.1/NJUlogin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-11-21 02:25:51.000000 NJUlogin-3.1.1/NJUlogin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-11-21 02:25:51.000000 NJUlogin-3.1.1/NJUlogin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2271 2023-11-21 02:25:51.477503 NJUlogin-3.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1779 2023-03-03 16:25:49.000000 NJUlogin-3.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-11-21 02:25:51.478915 NJUlogin-3.1.1/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-11-15 02:58:42.000000 NJUlogin-3.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-21 02:25:51.476185 NJUlogin-3.1.1/test/
--rw-rw-rw-   0        0        0     1006 2022-11-05 04:03:41.000000 NJUlogin-3.1.1/test/test.py
--rw-rw-rw-   0        0        0      773 2022-11-25 09:46:41.000000 NJUlogin-3.1.1/test/testlogin.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:49:34.301774 NJUlogin-3.1.2/
+-rw-rw-rw-   0        0        0     1082 2022-11-04 13:26:44.000000 NJUlogin-3.1.2/LICENSE
+-rw-rw-rw-   0        0        0       41 2023-11-15 02:56:13.000000 NJUlogin-3.1.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-06-02 15:49:34.212125 NJUlogin-3.1.2/NJUlogin/
+-rw-rw-rw-   0        0        0     4983 2024-06-02 15:46:27.000000 NJUlogin-3.1.2/NJUlogin/QRlogin.py
+-rw-rw-rw-   0        0        0      221 2022-11-07 11:22:45.000000 NJUlogin-3.1.2/NJUlogin/__init__.py
+-rw-rw-rw-   0        0        0      292 2024-06-02 15:46:39.000000 NJUlogin-3.1.2/NJUlogin/__version__.py
+-rw-rw-rw-   0        0        0     1286 2023-02-06 05:06:02.000000 NJUlogin-3.1.2/NJUlogin/_base_.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:49:34.280084 NJUlogin-3.1.2/NJUlogin/captchaOCR/
+-rw-rw-rw-   0        0        0       29 2023-11-15 02:29:03.000000 NJUlogin-3.1.2/NJUlogin/captchaOCR/__init__.py
+-rw-rw-rw-   0        0        0    67670 2023-11-15 02:32:08.000000 NJUlogin-3.1.2/NJUlogin/captchaOCR/charsets.py
+-rw-rw-rw-   0        0        0 13606198 2023-08-08 13:15:06.000000 NJUlogin-3.1.2/NJUlogin/captchaOCR/common.onnx
+-rw-rw-rw-   0        0        0     4757 2023-11-15 02:41:30.000000 NJUlogin-3.1.2/NJUlogin/captchaOCR/ocr.py
+-rw-rw-rw-   0        0        0      353 2023-08-11 13:09:46.000000 NJUlogin-3.1.2/NJUlogin/captchaOCR/utils.py
+-rw-rw-rw-   0        0        0     4039 2024-06-02 15:46:03.000000 NJUlogin-3.1.2/NJUlogin/pwdLogin.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:49:34.290271 NJUlogin-3.1.2/NJUlogin/utils/
+-rw-rw-rw-   0        0        0       15 2022-11-04 09:03:44.000000 NJUlogin-3.1.2/NJUlogin/utils/__init__.py
+-rw-rw-rw-   0        0        0       81 2022-11-04 07:34:30.000000 NJUlogin-3.1.2/NJUlogin/utils/clear.py
+-rw-rw-rw-   0        0        0      250 2023-08-12 02:52:33.000000 NJUlogin-3.1.2/NJUlogin/utils/config.py
+-rw-rw-rw-   0        0        0      858 2023-03-05 02:48:50.000000 NJUlogin-3.1.2/NJUlogin/utils/get_post.py
+-rw-rw-rw-   0        0        0      652 2023-03-03 16:25:08.000000 NJUlogin-3.1.2/NJUlogin/utils/urls.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:49:34.298739 NJUlogin-3.1.2/NJUlogin.egg-info/
+-rw-rw-rw-   0        0        0     2447 2024-06-02 15:49:34.000000 NJUlogin-3.1.2/NJUlogin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2024-06-02 15:49:34.000000 NJUlogin-3.1.2/NJUlogin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 15:49:34.000000 NJUlogin-3.1.2/NJUlogin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-06-02 15:49:34.000000 NJUlogin-3.1.2/NJUlogin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 15:49:34.000000 NJUlogin-3.1.2/NJUlogin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2447 2024-06-02 15:49:34.299752 NJUlogin-3.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1779 2023-03-03 16:25:49.000000 NJUlogin-3.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-02 15:49:34.301774 NJUlogin-3.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-11-15 02:58:42.000000 NJUlogin-3.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 15:49:34.295659 NJUlogin-3.1.2/test/
+-rw-rw-rw-   0        0        0     1006 2022-11-05 04:03:41.000000 NJUlogin-3.1.2/test/test.py
+-rw-rw-rw-   0        0        0      773 2022-11-25 09:46:41.000000 NJUlogin-3.1.2/test/testlogin.py
```

### Comparing `NJUlogin-3.1.1/LICENSE` & `NJUlogin-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.1.1/NJUlogin/QRlogin.py` & `NJUlogin-3.1.2/NJUlogin/QRlogin.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,10 +122,9 @@
             '_eventId': selector.xpath('//input[@name="_eventId"]/@value')[1],
             'rmShown': selector.xpath('//input[@name="rmShown"]/@value')[1]
         }
         res = self.post(url, data=data, timeout=self.getTimeout)
         if self.judge_not_login(res, url):
             print('登录失败')
             return None
-        print('登录成功')
         os.remove('QR.png')
         return self.session
```

### Comparing `NJUlogin-3.1.1/NJUlogin/_base_.py` & `NJUlogin-3.1.2/NJUlogin/_base_.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.1.1/NJUlogin/captchaOCR/charsets.py` & `NJUlogin-3.1.2/NJUlogin/captchaOCR/charsets.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.1.1/NJUlogin/captchaOCR/common.onnx` & `NJUlogin-3.1.2/NJUlogin/captchaOCR/common.onnx`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.1.1/NJUlogin/captchaOCR/ocr.py` & `NJUlogin-3.1.2/NJUlogin/captchaOCR/ocr.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.1.1/NJUlogin/pwdLogin.py` & `NJUlogin-3.1.2/NJUlogin/pwdLogin.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,9 +89,8 @@
                     print('登录失败，验证码识别错误次数过多')
                     return None
                 print('登录失败，验证码识别错误，正在重试')
                 return self.login(dest, trytimes + 1)
             else:
                 print('登录失败，' + errorMsg)
             return None
-        print('登录成功')
         return self.session
```

### Comparing `NJUlogin-3.1.1/NJUlogin/utils/get_post.py` & `NJUlogin-3.1.2/NJUlogin/utils/get_post.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.1.1/NJUlogin/utils/urls.py` & `NJUlogin-3.1.2/NJUlogin/utils/urls.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.1.1/NJUlogin.egg-info/PKG-INFO` & `NJUlogin-3.1.2/NJUlogin.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: NJUlogin
-Version: 3.1.1
+Version: 3.1.2
 Summary: The Nanjing University login module, which can be used to log in to the various campus web sites
 Home-page: https://github.com/Do1e/NJUlogin
 Author: Do1e
 Author-email: dpj.email@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: Pillow
+Requires-Dist: numpy
+Requires-Dist: lxml
+Requires-Dist: pycryptodome
+Requires-Dist: user_agents
+Requires-Dist: onnxruntime
 
 # NJUlogin
 
 * 南京大学统一身份认证登录模块，可用于登录校园各种网站，[Github link](https://github.com/Do1e/NJUlogin)，[PyPI link](https://pypi.org/project/NJUlogin/)。
 
 ## 安装
 ```bash
```

### Comparing `NJUlogin-3.1.1/NJUlogin.egg-info/SOURCES.txt` & `NJUlogin-3.1.2/NJUlogin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.1.1/PKG-INFO` & `NJUlogin-3.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: NJUlogin
-Version: 3.1.1
+Version: 3.1.2
 Summary: The Nanjing University login module, which can be used to log in to the various campus web sites
 Home-page: https://github.com/Do1e/NJUlogin
 Author: Do1e
 Author-email: dpj.email@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: Pillow
+Requires-Dist: numpy
+Requires-Dist: lxml
+Requires-Dist: pycryptodome
+Requires-Dist: user_agents
+Requires-Dist: onnxruntime
 
 # NJUlogin
 
 * 南京大学统一身份认证登录模块，可用于登录校园各种网站，[Github link](https://github.com/Do1e/NJUlogin)，[PyPI link](https://pypi.org/project/NJUlogin/)。
 
 ## 安装
 ```bash
```

### Comparing `NJUlogin-3.1.1/README.md` & `NJUlogin-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.1.1/setup.py` & `NJUlogin-3.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.1.1/test/test.py` & `NJUlogin-3.1.2/test/test.py`

 * *Files identical despite different names*

### Comparing `NJUlogin-3.1.1/test/testlogin.py` & `NJUlogin-3.1.2/test/testlogin.py`

 * *Files identical despite different names*

