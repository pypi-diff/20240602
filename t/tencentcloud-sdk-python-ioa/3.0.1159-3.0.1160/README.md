# Comparing `tmp/tencentcloud-sdk-python-ioa-3.0.1159.tar.gz` & `tmp/tencentcloud-sdk-python-ioa-3.0.1160.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ioa-3.0.1159.tar", last modified: Thu May 30 20:57:23 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ioa-3.0.1160.tar", last modified: Sun Jun  2 20:40:30 2024, max compression
```

## Comparing `tencentcloud-sdk-python-ioa-3.0.1159.tar` & `tencentcloud-sdk-python-ioa-3.0.1160.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/ioa/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/ioa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/ioa/v20220601/
--rw-r--r--   0 root         (0) root         (0)     1938 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/ioa/v20220601/ioa_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/ioa/v20220601/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1272 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/ioa/v20220601/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    35668 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/ioa/v20220601/models.py
--rw-r--r--   0 root         (0) root         (0)      737 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/README.rst
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud_sdk_python_ioa.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud_sdk_python_ioa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud_sdk_python_ioa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud_sdk_python_ioa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud_sdk_python_ioa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud_sdk_python_ioa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-30 20:57:23.000000 tencentcloud-sdk-python-ioa-3.0.1159/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/ioa/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/ioa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/ioa/v20220601/
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/ioa/v20220601/ioa_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/ioa/v20220601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/ioa/v20220601/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    35668 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/ioa/v20220601/models.py
+-rw-r--r--   0 root         (0) root         (0)      737 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud_sdk_python_ioa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud_sdk_python_ioa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud_sdk_python_ioa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud_sdk_python_ioa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud_sdk_python_ioa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud_sdk_python_ioa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-06-02 20:40:30.000000 tencentcloud-sdk-python-ioa-3.0.1160/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/ioa/v20220601/ioa_client.py` & `tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/ioa/v20220601/ioa_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/ioa/v20220601/errorcodes.py` & `tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/ioa/v20220601/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud/ioa/v20220601/models.py` & `tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud/ioa/v20220601/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ioa-3.0.1159/README.rst` & `tencentcloud-sdk-python-ioa-3.0.1160/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ioa-3.0.1159/setup.py` & `tencentcloud-sdk-python-ioa-3.0.1160/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ioa',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1159"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1160"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ioa SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-ioa-3.0.1159/tencentcloud_sdk_python_ioa.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ioa-3.0.1160/tencentcloud_sdk_python_ioa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ioa
-Version: 3.0.1159
+Version: 3.0.1160
 Summary: Tencent Cloud Ioa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ioa-3.0.1159/PKG-INFO` & `tencentcloud-sdk-python-ioa-3.0.1160/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ioa
-Version: 3.0.1159
+Version: 3.0.1160
 Summary: Tencent Cloud Ioa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

