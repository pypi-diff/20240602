# Comparing `tmp/aws_sso_util-4.32.0.tar.gz` & `tmp/aws_sso_util-4.33.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_sso_util-4.32.0.tar", max compression
+gzip compressed data, was "aws_sso_util-4.33.0.tar", max compression
```

## Comparing `aws_sso_util-4.32.0.tar` & `aws_sso_util-4.33.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1580 2023-01-27 00:02:09.764757 aws_sso_util-4.32.0/README.md
--rw-r--r--   0        0        0     1181 2023-07-19 20:05:43.028601 aws_sso_util-4.32.0/pyproject.toml
--rw-r--r--   0        0        0      624 2023-07-19 20:05:10.898602 aws_sso_util-4.32.0/src/aws_sso_util/__init__.py
--rw-r--r--   0        0        0      650 2022-11-15 22:45:02.830109 aws_sso_util-4.32.0/src/aws_sso_util/__main__.py
--rw-r--r--   0        0        0     7195 2023-01-27 00:02:09.764757 aws_sso_util-4.32.0/src/aws_sso_util/assignments.py
--rw-r--r--   0        0        0    15458 2023-01-27 00:56:16.543998 aws_sso_util-4.32.0/src/aws_sso_util/cfn.py
--rw-r--r--   0        0        0      569 2022-11-15 22:45:02.830109 aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/__init__.py
--rw-r--r--   0        0        0     6774 2022-11-15 22:45:02.830109 aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/cfn_yaml_tags.py
--rw-r--r--   0        0        0    15121 2022-11-15 22:45:02.830109 aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/config.py
--rw-r--r--   0        0        0    12066 2023-01-27 00:56:16.543998 aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/macro.py
--rw-r--r--   0        0        0    16156 2023-01-27 00:02:09.764757 aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/resources.py
--rw-r--r--   0        0        0    13564 2022-11-15 22:45:02.830109 aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/templates.py
--rw-r--r--   0        0        0     4369 2022-11-15 22:45:02.830109 aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/utils.py
--rw-r--r--   0        0        0    14840 2023-07-19 18:57:43.959057 aws_sso_util-4.32.0/src/aws_sso_util/check.py
--rw-r--r--   0        0        0     2123 2023-05-15 22:25:01.328180 aws_sso_util-4.32.0/src/aws_sso_util/cli.py
--rw-r--r--   0        0        0     8737 2023-01-27 00:02:09.764757 aws_sso_util-4.32.0/src/aws_sso_util/configure_profile.py
--rw-r--r--   0        0        0    16034 2023-01-27 00:02:09.764757 aws_sso_util-4.32.0/src/aws_sso_util/console.py
--rw-r--r--   0        0        0     7711 2023-01-27 00:02:09.764757 aws_sso_util-4.32.0/src/aws_sso_util/credential_process.py
--rw-r--r--   0        0        0     4906 2022-11-15 22:45:02.830109 aws_sso_util-4.32.0/src/aws_sso_util/deploy_macro.py
--rw-r--r--   0        0        0     7071 2023-05-15 22:25:01.328180 aws_sso_util-4.32.0/src/aws_sso_util/login.py
--rw-r--r--   0        0        0     3899 2023-01-27 00:02:09.764757 aws_sso_util-4.32.0/src/aws_sso_util/logout.py
--rw-r--r--   0        0        0     7679 2023-01-27 00:02:09.764757 aws_sso_util-4.32.0/src/aws_sso_util/lookup.py
--rw-r--r--   0        0        0    18358 2023-01-27 00:02:09.764757 aws_sso_util-4.32.0/src/aws_sso_util/populate_profiles.py
--rw-r--r--   0        0        0     5054 2023-05-15 22:25:01.328180 aws_sso_util-4.32.0/src/aws_sso_util/roles.py
--rw-r--r--   0        0        0     3788 2023-01-27 00:02:09.764757 aws_sso_util-4.32.0/src/aws_sso_util/run_as.py
--rw-r--r--   0        0        0     6155 2023-05-15 22:25:01.328180 aws_sso_util-4.32.0/src/aws_sso_util/utils.py
--rw-r--r--   0        0        0     2854 1970-01-01 00:00:00.000000 aws_sso_util-4.32.0/PKG-INFO
+-rw-r--r--   0        0        0     1580 2023-01-27 00:02:09.764757 aws_sso_util-4.33.0/README.md
+-rw-r--r--   0        0        0     1181 2024-06-02 14:30:51.457010 aws_sso_util-4.33.0/pyproject.toml
+-rw-r--r--   0        0        0      624 2024-06-02 14:30:55.297010 aws_sso_util-4.33.0/src/aws_sso_util/__init__.py
+-rw-r--r--   0        0        0      650 2022-11-15 22:45:02.830109 aws_sso_util-4.33.0/src/aws_sso_util/__main__.py
+-rw-r--r--   0        0        0     7195 2023-01-27 00:02:09.764757 aws_sso_util-4.33.0/src/aws_sso_util/assignments.py
+-rw-r--r--   0        0        0    15458 2023-01-27 00:56:16.543998 aws_sso_util-4.33.0/src/aws_sso_util/cfn.py
+-rw-r--r--   0        0        0      569 2022-11-15 22:45:02.830109 aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/__init__.py
+-rw-r--r--   0        0        0     6774 2022-11-15 22:45:02.830109 aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/cfn_yaml_tags.py
+-rw-r--r--   0        0        0    15121 2022-11-15 22:45:02.830109 aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/config.py
+-rw-r--r--   0        0        0    12066 2023-01-27 00:56:16.543998 aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/macro.py
+-rw-r--r--   0        0        0    16156 2023-01-27 00:02:09.764757 aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/resources.py
+-rw-r--r--   0        0        0    13564 2022-11-15 22:45:02.830109 aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/templates.py
+-rw-r--r--   0        0        0     4369 2022-11-15 22:45:02.830109 aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/utils.py
+-rw-r--r--   0        0        0    14840 2023-07-19 20:19:31.528524 aws_sso_util-4.33.0/src/aws_sso_util/check.py
+-rw-r--r--   0        0        0     2123 2024-05-26 13:40:28.052200 aws_sso_util-4.33.0/src/aws_sso_util/cli.py
+-rw-r--r--   0        0        0     8737 2023-01-27 00:02:09.764757 aws_sso_util-4.33.0/src/aws_sso_util/configure_profile.py
+-rw-r--r--   0        0        0    16034 2023-01-27 00:02:09.764757 aws_sso_util-4.33.0/src/aws_sso_util/console.py
+-rw-r--r--   0        0        0     7711 2023-01-27 00:02:09.764757 aws_sso_util-4.33.0/src/aws_sso_util/credential_process.py
+-rw-r--r--   0        0        0     4906 2022-11-15 22:45:02.830109 aws_sso_util-4.33.0/src/aws_sso_util/deploy_macro.py
+-rw-r--r--   0        0        0     7071 2024-05-26 13:40:28.052200 aws_sso_util-4.33.0/src/aws_sso_util/login.py
+-rw-r--r--   0        0        0     3899 2023-01-27 00:02:09.764757 aws_sso_util-4.33.0/src/aws_sso_util/logout.py
+-rw-r--r--   0        0        0     7679 2023-01-27 00:02:09.764757 aws_sso_util-4.33.0/src/aws_sso_util/lookup.py
+-rw-r--r--   0        0        0    18358 2023-01-27 00:02:09.764757 aws_sso_util-4.33.0/src/aws_sso_util/populate_profiles.py
+-rw-r--r--   0        0        0     5054 2024-05-26 13:40:28.052200 aws_sso_util-4.33.0/src/aws_sso_util/roles.py
+-rw-r--r--   0        0        0     3788 2023-01-27 00:02:09.764757 aws_sso_util-4.33.0/src/aws_sso_util/run_as.py
+-rw-r--r--   0        0        0     6155 2024-05-26 13:40:28.062200 aws_sso_util-4.33.0/src/aws_sso_util/utils.py
+-rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 aws_sso_util-4.33.0/PKG-INFO
```

### Comparing `aws_sso_util-4.32.0/README.md` & `aws_sso_util-4.33.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/pyproject.toml` & `aws_sso_util-4.33.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-sso-util"
-version = "4.32.0" # change in aws_sso_util/__init__.py too
+version = "4.33.0" # change in aws_sso_util/__init__.py too
 description = "Utilities to make AWS SSO easier"
 authors = ["Ben Kehoe <ben@kehoe.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/benkehoe/aws-sso-util"
 repository = "https://github.com/benkehoe/aws-sso-util"
 classifiers = [
@@ -21,15 +21,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 # botocore = {git = "https://github.com/boto/botocore.git", rev = "v2"}
 click = ">=8.0.0, < 9.0.0"
 boto3 = ">=1.24.60, <2.0.0"
 pyyaml = ">=6.0.1, <7.0.0"
-jsonschema = "^3.2.0"
+jsonschema = "^4.0.1"
 aws-error-utils = "^2.4"
 python-dateutil = "^2.8.1"
 aws-sso-lib = "^1.13.0"
 # aws-sso-lib = { path = "../lib", develop = true }
 requests = "^2.26.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/__init__.py` & `aws_sso_util-4.33.0/src/aws_sso_util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '4.32.0' # change in pyproject.toml too
+__version__ = '4.33.0' # change in pyproject.toml too
```

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/__main__.py` & `aws_sso_util-4.33.0/src/aws_sso_util/__main__.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/assignments.py` & `aws_sso_util-4.33.0/src/aws_sso_util/assignments.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/cfn.py` & `aws_sso_util-4.33.0/src/aws_sso_util/cfn.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/__init__.py` & `aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/cfn_yaml_tags.py` & `aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/cfn_yaml_tags.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/config.py` & `aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/config.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/macro.py` & `aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/macro.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/resources.py` & `aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/resources.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/templates.py` & `aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/templates.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/cfn_lib/utils.py` & `aws_sso_util-4.33.0/src/aws_sso_util/cfn_lib/utils.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/check.py` & `aws_sso_util-4.33.0/src/aws_sso_util/check.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/cli.py` & `aws_sso_util-4.33.0/src/aws_sso_util/cli.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/configure_profile.py` & `aws_sso_util-4.33.0/src/aws_sso_util/configure_profile.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/console.py` & `aws_sso_util-4.33.0/src/aws_sso_util/console.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/credential_process.py` & `aws_sso_util-4.33.0/src/aws_sso_util/credential_process.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/deploy_macro.py` & `aws_sso_util-4.33.0/src/aws_sso_util/deploy_macro.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/login.py` & `aws_sso_util-4.33.0/src/aws_sso_util/login.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/logout.py` & `aws_sso_util-4.33.0/src/aws_sso_util/logout.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/lookup.py` & `aws_sso_util-4.33.0/src/aws_sso_util/lookup.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/populate_profiles.py` & `aws_sso_util-4.33.0/src/aws_sso_util/populate_profiles.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/roles.py` & `aws_sso_util-4.33.0/src/aws_sso_util/roles.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/run_as.py` & `aws_sso_util-4.33.0/src/aws_sso_util/run_as.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/src/aws_sso_util/utils.py` & `aws_sso_util-4.33.0/src/aws_sso_util/utils.py`

 * *Files identical despite different names*

### Comparing `aws_sso_util-4.32.0/PKG-INFO` & `aws_sso_util-4.33.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-sso-util
-Version: 4.32.0
+Version: 4.33.0
 Summary: Utilities to make AWS SSO easier
 Home-page: https://github.com/benkehoe/aws-sso-util
 License: Apache-2.0
 Author: Ben Kehoe
 Author-email: ben@kehoe.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,20 +14,21 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: aws-error-utils (>=2.4,<3.0)
 Requires-Dist: aws-sso-lib (>=1.13.0,<2.0.0)
 Requires-Dist: boto3 (>=1.24.60,<2.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
-Requires-Dist: jsonschema (>=3.2.0,<4.0.0)
+Requires-Dist: jsonschema (>=4.0.1,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Project-URL: Repository, https://github.com/benkehoe/aws-sso-util
 Description-Content-Type: text/markdown
 
 # aws-sso-util
```

