# Comparing `tmp/tencentcloud-sdk-python-lke-3.0.1159.tar.gz` & `tmp/tencentcloud-sdk-python-lke-3.0.1160.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lke-3.0.1159.tar", last modified: Thu May 30 20:59:46 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lke-3.0.1160.tar", last modified: Sun Jun  2 20:42:56 2024, max compression
```

## Comparing `tencentcloud-sdk-python-lke-3.0.1159.tar` & `tencentcloud-sdk-python-lke-3.0.1160.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/__init__.py
--rw-r--r--   0 root         (0) root         (0)      961 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   384334 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/models.py
--rw-r--r--   0 root         (0) root         (0)    66422 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/lke_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/README.rst
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-30 20:59:46.000000 tencentcloud-sdk-python-lke-3.0.1159/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/lke/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/lke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/lke/v20231130/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/lke/v20231130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      961 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/lke/v20231130/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   384334 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/lke/v20231130/models.py
+-rw-r--r--   0 root         (0) root         (0)    66422 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/lke/v20231130/lke_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud_sdk_python_lke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud_sdk_python_lke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud_sdk_python_lke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud_sdk_python_lke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud_sdk_python_lke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/tencentcloud_sdk_python_lke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-06-02 20:42:56.000000 tencentcloud-sdk-python-lke-3.0.1160/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1159'
+__version__ = '3.0.1160'
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/errorcodes.py` & `tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/lke/v20231130/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/models.py` & `tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/lke/v20231130/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lke-3.0.1159/tencentcloud/lke/v20231130/lke_client.py` & `tencentcloud-sdk-python-lke-3.0.1160/tencentcloud/lke/v20231130/lke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lke-3.0.1159/tencentcloud_sdk_python_lke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lke-3.0.1160/tencentcloud_sdk_python_lke.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lke
-Version: 3.0.1159
+Version: 3.0.1160
 Summary: Tencent Cloud Lke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1159/README.rst` & `tencentcloud-sdk-python-lke-3.0.1160/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lke-3.0.1159/setup.py` & `tencentcloud-sdk-python-lke-3.0.1160/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-lke',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1159"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1160"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Lke SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1159/PKG-INFO` & `tencentcloud-sdk-python-lke-3.0.1160/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lke
-Version: 3.0.1159
+Version: 3.0.1160
 Summary: Tencent Cloud Lke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

