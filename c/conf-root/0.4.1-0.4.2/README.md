# Comparing `tmp/conf_root-0.4.1.tar.gz` & `tmp/conf_root-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_root-0.4.1.tar", last modified: Fri May 31 03:40:41 2024, max compression
+gzip compressed data, was "conf_root-0.4.2.tar", last modified: Sun Jun  2 10:52:24 2024, max compression
```

## Comparing `conf_root-0.4.1.tar` & `conf_root-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:40:41.268086 conf_root-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 03:40:36.000000 conf_root-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-31 03:40:41.268086 conf_root-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-31 03:40:36.000000 conf_root-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:40:41.264086 conf_root-0.4.1/conf_root/
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/ConfRoot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:40:41.268086 conf_root-0.4.1/conf_root/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/agents/BasicAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/agents/JsonAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/agents/YamlAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/agents/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:40:41.268086 conf_root-0.4.1/conf_root.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-31 03:40:41.000000 conf_root-0.4.1/conf_root.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-31 03:40:41.000000 conf_root-0.4.1/conf_root.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:40:41.000000 conf_root-0.4.1/conf_root.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 03:40:41.000000 conf_root-0.4.1/conf_root.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 03:40:41.000000 conf_root-0.4.1/conf_root.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 03:40:36.000000 conf_root-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 03:40:41.268086 conf_root-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-31 03:40:36.000000 conf_root-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:40:41.268086 conf_root-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_ConfigurationField.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_multi_file_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_nested_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_single_file_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:52:24.469797 conf_root-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-02 10:52:19.000000 conf_root-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-02 10:52:19.000000 conf_root-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-06-02 10:52:24.469797 conf_root-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-06-02 10:52:19.000000 conf_root-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:52:24.465797 conf_root-0.4.2/conf_root/
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-06-02 10:52:19.000000 conf_root-0.4.2/conf_root/ConfRoot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-06-02 10:52:19.000000 conf_root-0.4.2/conf_root/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-06-02 10:52:19.000000 conf_root-0.4.2/conf_root/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:52:24.469797 conf_root-0.4.2/conf_root/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-06-02 10:52:19.000000 conf_root-0.4.2/conf_root/agents/BasicAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-02 10:52:19.000000 conf_root-0.4.2/conf_root/agents/JsonAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-06-02 10:52:19.000000 conf_root-0.4.2/conf_root/agents/YamlAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-06-02 10:52:19.000000 conf_root-0.4.2/conf_root/run_http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:52:24.469797 conf_root-0.4.2/conf_root/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-06-02 10:52:19.000000 conf_root-0.4.2/conf_root/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-02 10:52:19.000000 conf_root-0.4.2/conf_root/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-06-02 10:52:19.000000 conf_root-0.4.2/conf_root/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:52:24.469797 conf_root-0.4.2/conf_root.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-06-02 10:52:24.000000 conf_root-0.4.2/conf_root.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-06-02 10:52:24.000000 conf_root-0.4.2/conf_root.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 10:52:24.000000 conf_root-0.4.2/conf_root.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 10:52:24.000000 conf_root-0.4.2/conf_root.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 10:52:24.000000 conf_root-0.4.2/conf_root.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 10:52:24.000000 conf_root-0.4.2/conf_root.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-06-02 10:52:19.000000 conf_root-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 10:52:24.469797 conf_root-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-06-02 10:52:19.000000 conf_root-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 10:52:24.469797 conf_root-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-06-02 10:52:19.000000 conf_root-0.4.2/tests/test_ConfigurationField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-06-02 10:52:19.000000 conf_root-0.4.2/tests/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-06-02 10:52:19.000000 conf_root-0.4.2/tests/test_extract_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-06-02 10:52:19.000000 conf_root-0.4.2/tests/test_multi_file_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-06-02 10:52:19.000000 conf_root-0.4.2/tests/test_nested_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-06-02 10:52:19.000000 conf_root-0.4.2/tests/test_single_file_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-06-02 10:52:19.000000 conf_root-0.4.2/tests/test_wrap.py
```

### Comparing `conf_root-0.4.1/LICENSE` & `conf_root-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.1/PKG-INFO` & `conf_root-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: conf_root
-Version: 0.4.1
+Version: 0.4.2
 Summary: 基于dataclass的科研配置文件取用工具
 Home-page: https://github.com/ciaranchen/conf_root
 Author: ciaranchen
 Author-email: ciaranchen <ciaranchen@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ruamel-yaml>=0.18.6
+Requires-Dist: wtforms>=3.1.2
+Requires-Dist: jinja2>=3.1.4
 
 # Conf Root
 
 ![PyPI - Version](https://img.shields.io/pypi/v/conf_root)
 
 基于dataclass的科研配置文件取用工具。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
 
 1. 为您定义的类生成一个配置文件；并优先使用配置文件中的值作为类中变量的值。
 2. 将某些科研项目中的argparse转换为dataclass，进而生成配置文件；从而可以在配置文件中修改输入。
+3. 提供脚本 `conf-root-web`。提供一个web界面，允许您可视化修改类定义的配置文件。
 
-> Note: 仅用于配置文件，因此不提倡在配置文件类中使用动态的变量。
+> Note: 仅用于配置文件，不提倡在配置文件类中使用动态的变量。
 
 ## 装饰类的定义生成配置文件
 
 项目使用dataclass对配置类进行封装，并产生配置文件。
 
 > note: 类定义的字段需要类型注解。如果不指定字段类型，将被视为类变量而不会被解析为dataclass中的字段，也无法被这个类进行解析。
 
@@ -110,14 +113,26 @@
 解析Argparse并转换为dataclass，并且用ConfRoot.wrap封装它
 
 - paser。需解析的argparse.ArgumentParser。
 - cls_name。这个参数既是产生的dataclass类的类名，也是使用ConfRoot.wrap封装时的name参数。默认值为argparse。
 
 from_argparse 目前仅支持常见的官方Argparse动作，但是对于自定义的Action来说可能支持有限。这不意味着有不支持的命令行参数会导致报错，这些参数将会被忽略跳过。
 
+## Web界面可视化修改配置文件
+
+```shell
+conf-root-web [-h] [--host HOST] [--port PORT] filename
+```
+
+这个脚本允许您在一个网页中可视化地修改您的配置文件。
+
+- filename 提取配置类的Python文件名
+- HOST 服务器的host
+- PORT 服务器的port
+
 ## More Example
 
 支持嵌套。
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
 from conf_root import ConfRoot, JsonAgent
```

### Comparing `conf_root-0.4.1/README.md` & `conf_root-0.4.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 ![PyPI - Version](https://img.shields.io/pypi/v/conf_root)
 
 基于dataclass的科研配置文件取用工具。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
 
 1. 为您定义的类生成一个配置文件；并优先使用配置文件中的值作为类中变量的值。
 2. 将某些科研项目中的argparse转换为dataclass，进而生成配置文件；从而可以在配置文件中修改输入。
+3. 提供脚本 `conf-root-web`。提供一个web界面，允许您可视化修改类定义的配置文件。
 
-> Note: 仅用于配置文件，因此不提倡在配置文件类中使用动态的变量。
+> Note: 仅用于配置文件，不提倡在配置文件类中使用动态的变量。
 
 ## 装饰类的定义生成配置文件
 
 项目使用dataclass对配置类进行封装，并产生配置文件。
 
 > note: 类定义的字段需要类型注解。如果不指定字段类型，将被视为类变量而不会被解析为dataclass中的字段，也无法被这个类进行解析。
 
@@ -97,14 +98,26 @@
 解析Argparse并转换为dataclass，并且用ConfRoot.wrap封装它
 
 - paser。需解析的argparse.ArgumentParser。
 - cls_name。这个参数既是产生的dataclass类的类名，也是使用ConfRoot.wrap封装时的name参数。默认值为argparse。
 
 from_argparse 目前仅支持常见的官方Argparse动作，但是对于自定义的Action来说可能支持有限。这不意味着有不支持的命令行参数会导致报错，这些参数将会被忽略跳过。
 
+## Web界面可视化修改配置文件
+
+```shell
+conf-root-web [-h] [--host HOST] [--port PORT] filename
+```
+
+这个脚本允许您在一个网页中可视化地修改您的配置文件。
+
+- filename 提取配置类的Python文件名
+- HOST 服务器的host
+- PORT 服务器的port
+
 ## More Example
 
 支持嵌套。
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
 from conf_root import ConfRoot, JsonAgent
```

### Comparing `conf_root-0.4.1/conf_root/ConfRoot.py` & `conf_root-0.4.2/conf_root/ConfRoot.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 from typing import Optional, Type, List
 import logging
 
 from conf_root.Configuration import Configuration
 from conf_root.agents.BasicAgent import BasicAgent
 from conf_root.agents.YamlAgent import YamlAgent
+from conf_root.run_http import run_http, extract_classes_from_file, dataclass_to_wtform
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
                     datefmt='%m-%d %H:%M:%S')
 logger = logging.getLogger(__name__)
 
 
 class ConfRoot:
@@ -25,15 +26,15 @@
         def decorator(cls, name: Optional[str] = None, dynamic=False):
             if not is_dataclass(cls):
                 logger.debug(f'decorate class {cls.__qualname__} to dataclass...')
                 cls = dataclass(cls)
             if name is None:
                 name = cls.__qualname__.replace('<locals>.', '')
 
-            configuration = Configuration(name, cls)
+            configuration = Configuration(name, cls, self)
             setattr(cls, '__CONF_ROOT__', configuration)
 
             # 覆盖其 __init__ 函数
             origin_init = cls.__init__
 
             def decorated_init(_self, *args, **kwargs):
                 origin_init(_self, *args, **kwargs)
@@ -128,7 +129,28 @@
             fields.append(field)
             # print(field)
 
         fields = sorted(fields, key=lambda x: x[2].default == MISSING, reverse=True)
 
         cls = make_dataclass(cls_name.replace(f'.{self.agent.default_extension}', ''), fields)
         return self.config(cls)
+
+
+def main():
+    parser = argparse.ArgumentParser(prog='conf-root-web',
+                                     description="这个脚本允许您在一个网页中可视化地修改您的配置文件。")
+    parser.add_argument('filename', help="提取配置类的Python文件名")
+    parser.add_argument('--host', '-H', default='127.0.0.1', help='服务器的host')
+    parser.add_argument('--port', '-P', default=8080, help='服务器的port')
+    args = parser.parse_args()
+
+    classes = extract_classes_from_file(args.filename)
+    if len(classes) == 0:
+        print(f"No classes found in {args.filename}.")
+        return
+    print(f"Configuration classes defined in {args.filename}: {classes}")
+    forms = {cls: dataclass_to_wtform(cls) for cls in classes}
+    run_http(forms, host=args.host, port=args.port)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `conf_root-0.4.1/conf_root/agents/BasicAgent.py` & `conf_root-0.4.2/conf_root/agents/BasicAgent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.1/conf_root/agents/YamlAgent.py` & `conf_root-0.4.2/conf_root/agents/YamlAgent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dataclasses
 import os.path
 from ruamel.yaml import YAML, CommentedMap
 
 from conf_root.Configuration import Configuration, is_config_class
 from conf_root.agents.BasicAgent import BasicAgent, OneFileAgent
-from conf_root.agents.utils import data2obj
+from conf_root.utils import data2obj
 
 
 def make_serializer(cls):
     name = cls.__CONF_ROOT__.name
 
     def config_class_representer(dumper, data):
         data_dict = CommentedMap()
```

### Comparing `conf_root-0.4.1/conf_root/agents/utils.py` & `conf_root-0.4.2/conf_root/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,65 @@
 from dataclasses import fields
-from typing import Optional, Dict, Any
+from typing import Dict, Any
 
 from conf_root.Configuration import is_config_class
 import logging
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
                     datefmt='%m-%d %H:%M:%S')
 logger = logging.getLogger(__name__)
 
 
 class ValidateException(BaseException):
     pass
 
 
-def recursive_data2obj(cls, data: Optional[Dict[str, Any]], custom=False) -> object:
-    if is_config_class(cls):
-        kwargs = {}
-        for field in fields(cls):
-            value = data.get(field.name, None)
-            # 在进行用户自定义 deserialize 之后，不再进入递归流程。
-            if (custom and 'deserialize' in field.metadata and
-                    (deserialize_func := field.metadata['deserialize']) is not None):
-                value = deserialize_func(value)
-                kwargs[field.name] = value
-                continue
-            # 递归反序列化。
-            if value is not None:
-                value = recursive_data2obj(field.type, value, custom)
-                if 'validators' in field.metadata:
-                    for validator in field.metadata['validators']:
-                        if not validator(value):
-                            raise ValidateException(f'{field} with value {value} validate failed.')
-                kwargs[field.name] = value
-        # 默认值将会在dataclass中有默认定义。
-        # TODO: 这个地方会不会有__init__的递归问题？
-        return cls(**kwargs)
-    return data
+def validate(field, value):
+    if 'validators' in field.metadata:
+        for validator in field.metadata['validators']:
+            if not validator(value):
+                raise ValidateException(f'{field} with value {value} validate failed.')
 
 
 def data2obj(instance, data: Dict[str, Any], custom=False) -> None:
     # 这个不需要加载default，因为origin_init中调用过了。
     for field in fields(instance):
         # 从字典中获取值，如果不存在则跳过
         if (value := data.get(field.name, None)) is not None:
             # 在进行用户自定义 deserialize 之后，不再进入递归流程。
             if (custom and 'deserialize' in field.metadata and
                     (deserialize_func := field.metadata['deserialize']) is not None):
                 value = deserialize_func(value)
             else:
-                value = recursive_data2obj(field.type, value, custom)
-            if 'validators' in field.metadata:
-                for validator in field.metadata['validators']:
-                    if not validator(value):
-                        raise ValidateException(f'{field} with value {value} validate failed.')
+                cls = field.type
+                if is_config_class(cls) and isinstance(value, dict):
+                    sub_data = {field.name: value.get(field.name, None) for field in fields(cls)}
+                    # 要求 sub_data 中的内容必须能满足初始化要求
+                    sub_instance = cls(**sub_data)
+                    # 后面继续做这个步骤的原因是避免从文件加载的cls内容，确保是用sub_data建立的。
+                    data2obj(instance=sub_instance, data=sub_data, custom=custom)
+                    value = sub_instance
+                else:
+                    value = value
+            validate(field, value)
             # 设置字段值
             setattr(instance, field.name, value)
+
+
+def obj2data(obj: Any) -> Dict[str, Any]:
+    """
+    递归地将dataclass实例及其嵌套的dataclass字段转换为字典。
+    """
+    if is_config_class(obj):
+        # 对于dataclass实例，递归地处理其字段
+        res = {}
+        for field in fields(obj):
+            value = getattr(obj, field.name)
+            # 尝试获取serialize函数并调用之。
+            if 'serialize' in field.metadata and (serialize_func := field.metadata['serialize']) is not None:
+                value = serialize_func(value)
+                res[field.name] = value
+                # 在进行用户自定义 serialize之后，不再进入递归。
+                continue
+            res[field.name] = obj2data(value)
+        return res
+    return obj
```

### Comparing `conf_root-0.4.1/conf_root.egg-info/PKG-INFO` & `conf_root-0.4.2/conf_root.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: conf_root
-Version: 0.4.1
+Version: 0.4.2
 Summary: 基于dataclass的科研配置文件取用工具
 Home-page: https://github.com/ciaranchen/conf_root
 Author: ciaranchen
 Author-email: ciaranchen <ciaranchen@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ruamel-yaml>=0.18.6
+Requires-Dist: wtforms>=3.1.2
+Requires-Dist: jinja2>=3.1.4
 
 # Conf Root
 
 ![PyPI - Version](https://img.shields.io/pypi/v/conf_root)
 
 基于dataclass的科研配置文件取用工具。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
 
 1. 为您定义的类生成一个配置文件；并优先使用配置文件中的值作为类中变量的值。
 2. 将某些科研项目中的argparse转换为dataclass，进而生成配置文件；从而可以在配置文件中修改输入。
+3. 提供脚本 `conf-root-web`。提供一个web界面，允许您可视化修改类定义的配置文件。
 
-> Note: 仅用于配置文件，因此不提倡在配置文件类中使用动态的变量。
+> Note: 仅用于配置文件，不提倡在配置文件类中使用动态的变量。
 
 ## 装饰类的定义生成配置文件
 
 项目使用dataclass对配置类进行封装，并产生配置文件。
 
 > note: 类定义的字段需要类型注解。如果不指定字段类型，将被视为类变量而不会被解析为dataclass中的字段，也无法被这个类进行解析。
 
@@ -110,14 +113,26 @@
 解析Argparse并转换为dataclass，并且用ConfRoot.wrap封装它
 
 - paser。需解析的argparse.ArgumentParser。
 - cls_name。这个参数既是产生的dataclass类的类名，也是使用ConfRoot.wrap封装时的name参数。默认值为argparse。
 
 from_argparse 目前仅支持常见的官方Argparse动作，但是对于自定义的Action来说可能支持有限。这不意味着有不支持的命令行参数会导致报错，这些参数将会被忽略跳过。
 
+## Web界面可视化修改配置文件
+
+```shell
+conf-root-web [-h] [--host HOST] [--port PORT] filename
+```
+
+这个脚本允许您在一个网页中可视化地修改您的配置文件。
+
+- filename 提取配置类的Python文件名
+- HOST 服务器的host
+- PORT 服务器的port
+
 ## More Example
 
 支持嵌套。
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
 from conf_root import ConfRoot, JsonAgent
```

### Comparing `conf_root-0.4.1/conf_root.egg-info/SOURCES.txt` & `conf_root-0.4.2/conf_root.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 conf_root/ConfRoot.py
 conf_root/Configuration.py
 conf_root/__init__.py
+conf_root/run_http.py
+conf_root/utils.py
 conf_root.egg-info/PKG-INFO
 conf_root.egg-info/SOURCES.txt
 conf_root.egg-info/dependency_links.txt
+conf_root.egg-info/entry_points.txt
 conf_root.egg-info/requires.txt
 conf_root.egg-info/top_level.txt
 conf_root/agents/BasicAgent.py
 conf_root/agents/JsonAgent.py
 conf_root/agents/YamlAgent.py
-conf_root/agents/utils.py
+conf_root/templates/form.html
+conf_root/templates/index.html
 tests/test_ConfigurationField.py
 tests/test_argparse.py
+tests/test_extract_class.py
 tests/test_multi_file_agent.py
 tests/test_nested_dataclass.py
 tests/test_single_file_agent.py
 tests/test_wrap.py
```

### Comparing `conf_root-0.4.1/setup.py` & `conf_root-0.4.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="conf_root",  # 包名
-    version="0.4.1",  # 版本号
+    version="0.4.2",  # 版本号
     install_requires=[
-        "ruamel.yaml"
+        "ruamel.yaml>=0.18.6",
+        "wtforms>=3.1.2",
+        "jinja2>=3.1.4"
     ],
     author="ciaranchen",
     author_email="ciaranchen@qq.com",
     description="基于dataclass的配置文件取用工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ciaranchen/conf_root",
     packages=["conf_root", "conf_root.agents"],  # 包含的Python模块或子包
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',  # 兼容的Python版本
+    entry_points={
+        "console_scripts": [
+            'conf-root-web=conf_root.ConfRoot:main'
+        ],
+    },
+    package_data={
+        'conf_root': ['templates/*.html'],  # 这里指定你的html文件
+    },
+    include_package_data=True,  # 必须要有这一行
 )
```

### Comparing `conf_root-0.4.1/tests/test_ConfigurationField.py` & `conf_root-0.4.2/tests/test_ConfigurationField.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.1/tests/test_argparse.py` & `conf_root-0.4.2/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.1/tests/test_multi_file_agent.py` & `conf_root-0.4.2/tests/test_multi_file_agent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.1/tests/test_nested_dataclass.py` & `conf_root-0.4.2/tests/test_nested_dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         # 将处理后的内容写回文件（可以先备份原文件）
         with open(self.location, 'w') as file:
             file.write(content)
 
         DecoratedConfig = ConfRoot().config(self.location, dynamic=True)(AppConfig)
         app_config = DecoratedConfig(NestedConfig(config1='defined1', config2='defined2'))
         self.assertEqual(app_config.nc_default.config1, 'default_load1')
-        self.assertEqual(app_config.nc_default.config2, 'nest_config2')
+        self.assertIsNone(app_config.nc_default.config2)
 
         self.assertEqual(app_config.nc_defined.config1, 'load1')
         self.assertEqual(app_config.nc_defined.config2, 'load2')
 
     def test_save(self):
         DecoratedConfig = ConfRoot().config(self.location, dynamic=True)(AppConfig)
         app_config = DecoratedConfig(NestedConfig(config1='defined1', config2='defined2'))
```

### Comparing `conf_root-0.4.1/tests/test_single_file_agent.py` & `conf_root-0.4.2/tests/test_single_file_agent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.1/tests/test_wrap.py` & `conf_root-0.4.2/tests/test_wrap.py`

 * *Files identical despite different names*

