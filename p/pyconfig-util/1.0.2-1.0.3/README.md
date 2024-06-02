# Comparing `tmp/pyconfig_util-1.0.2.tar.gz` & `tmp/pyconfig_util-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconfig_util-1.0.2.tar", last modified: Wed May  1 13:41:32 2024, max compression
+gzip compressed data, was "pyconfig_util-1.0.3.tar", last modified: Sat Jun  1 16:04:25 2024, max compression
```

## Comparing `pyconfig_util-1.0.2.tar` & `pyconfig_util-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:41:32.341922 pyconfig_util-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-01 13:41:24.000000 pyconfig_util-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-01 13:41:32.337922 pyconfig_util-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-01 13:41:24.000000 pyconfig_util-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:41:32.337922 pyconfig_util-1.0.2/pyconfig_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:41:24.000000 pyconfig_util-1.0.2/pyconfig_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-01 13:41:24.000000 pyconfig_util-1.0.2/pyconfig_util/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:41:32.337922 pyconfig_util-1.0.2/pyconfig_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:41:32.341922 pyconfig_util-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-01 13:41:24.000000 pyconfig_util-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:04:25.055826 pyconfig_util-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-06-01 16:04:17.000000 pyconfig_util-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-06-01 16:04:25.055826 pyconfig_util-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-06-01 16:04:17.000000 pyconfig_util-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:04:25.055826 pyconfig_util-1.0.3/pyconfig_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 16:04:17.000000 pyconfig_util-1.0.3/pyconfig_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-06-01 16:04:17.000000 pyconfig_util-1.0.3/pyconfig_util/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:04:25.055826 pyconfig_util-1.0.3/pyconfig_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-06-01 16:04:25.000000 pyconfig_util-1.0.3/pyconfig_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-06-01 16:04:25.000000 pyconfig_util-1.0.3/pyconfig_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:04:25.000000 pyconfig_util-1.0.3/pyconfig_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 16:04:25.000000 pyconfig_util-1.0.3/pyconfig_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 16:04:25.000000 pyconfig_util-1.0.3/pyconfig_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:04:25.000000 pyconfig_util-1.0.3/pyconfig_util.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:04:25.055826 pyconfig_util-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-06-01 16:04:17.000000 pyconfig_util-1.0.3/setup.py
```

### Comparing `pyconfig_util-1.0.2/LICENSE` & `pyconfig_util-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconfig_util-1.0.2/pyconfig_util/config_util.py` & `pyconfig_util-1.0.3/pyconfig_util/config_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 import yaml
 import logging
 import sys
 
 
 class Setting(object):
     def __init__(self):
-        root_dir = os.getcwd()
-        config_file = root_dir + '/config/' + 'setting.yaml'  # 假设这是你的YAML文件名
-        config_path = os.path.join(root_dir, config_file)
+        self.root_dir = os.getcwd()
+        self.default_config_file = self.root_dir + '/config/' + 'setting.default.yaml'
+        self.default_config_path = os.path.join(self.root_dir, self.default_config_file)
+        self.config_file = self.root_dir + '/config/' + 'setting.yaml'
+        self.config_path = os.path.join(self.root_dir, self.config_file)
+        self._load_config(self.default_config_path)
+        self._load_config(self.config_path)
 
+    def _load_config(self, config_path):
+        """
+        config_path: yaml配置文件的地址
+        加载配置文件
+        """
         # 检查是否存在配置文件
         if not os.path.exists(config_path):
             # 退出整个程序
             logging.error('没有配置文件!!!')
             sys.exit()
 
         with open(config_path, 'r', encoding='utf-8') as file:
```

### Comparing `pyconfig_util-1.0.2/setup.py` & `pyconfig_util-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with io.open("requirements.txt", 'r') as f:
     install_requires = f.read().split(os.sep)
 
 
 setup(
     name='pyconfig_util',
-    version='1.0.2',
+    version='1.0.3',
     description='config助手',
     author='buyfakett',
     author_email='buyfakett@vip.qq.com',
     license='MIT',
     url="https://github.com/buyfakett",
     packages=find_packages(),  # packages=["pytest"],
     long_description=long_description,
```

