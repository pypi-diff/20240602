# Comparing `tmp/ezcoding-0.2.2.tar.gz` & `tmp/ezcoding-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcoding-0.2.2.tar", last modified: Wed May 29 15:39:18 2024, max compression
+gzip compressed data, was "ezcoding-0.2.3.tar", last modified: Sun Jun  2 04:25:44 2024, max compression
```

## Comparing `ezcoding-0.2.2.tar` & `ezcoding-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 15:39:18.833727 ezcoding-0.2.2/
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:02:10.000000 ezcoding-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     2004 2024-05-29 15:39:18.833727 ezcoding-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1724 2024-05-28 16:34:00.000000 ezcoding-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 15:39:18.813235 ezcoding-0.2.2/ezcoding/
--rw-rw-rw-   0        0        0      117 2024-05-24 16:11:38.000000 ezcoding-0.2.2/ezcoding/__init__.py
--rw-rw-rw-   0        0        0      162 2024-05-29 15:09:34.000000 ezcoding-0.2.2/ezcoding/const.py
--rw-rw-rw-   0        0        0      441 2024-05-24 15:13:49.000000 ezcoding-0.2.2/ezcoding/generator.py
-drwxrwxrwx   0        0        0        0 2024-05-29 15:39:18.826079 ezcoding-0.2.2/ezcoding/generators/
--rw-rw-rw-   0        0        0      308 2024-05-25 12:15:30.000000 ezcoding-0.2.2/ezcoding/generators/__init__.py
--rw-rw-rw-   0        0        0      946 2024-05-29 14:09:13.000000 ezcoding-0.2.2/ezcoding/generators/author_generator.py
--rw-rw-rw-   0        0        0      272 2024-05-26 05:11:45.000000 ezcoding-0.2.2/ezcoding/generators/date_string_generator.py
--rw-rw-rw-   0        0        0     1032 2024-05-29 14:26:52.000000 ezcoding-0.2.2/ezcoding/generators/header_filename_generator.py
--rw-rw-rw-   0        0        0      888 2024-05-26 05:11:39.000000 ezcoding-0.2.2/ezcoding/generators/header_macro_generator.py
--rw-rw-rw-   0        0        0      256 2024-05-26 05:11:32.000000 ezcoding-0.2.2/ezcoding/generators/uuid_string_generator.py
--rw-rw-rw-   0        0        0     2987 2024-05-29 15:16:48.000000 ezcoding-0.2.2/ezcoding/task.py
--rw-rw-rw-   0        0        0     2537 2024-05-26 06:19:51.000000 ezcoding-0.2.2/ezcoding/template.py
-drwxrwxrwx   0        0        0        0 2024-05-29 15:39:18.829071 ezcoding-0.2.2/ezcoding/ui/
--rw-rw-rw-   0        0        0       93 2024-05-26 03:12:25.000000 ezcoding-0.2.2/ezcoding/ui/__init__.py
--rw-rw-rw-   0        0        0      164 2024-05-26 03:11:52.000000 ezcoding-0.2.2/ezcoding/ui/application.py
--rw-rw-rw-   0        0        0     7614 2024-05-29 15:33:21.000000 ezcoding-0.2.2/ezcoding/ui/editor.py
--rw-rw-rw-   0        0        0      287 2024-05-26 06:18:12.000000 ezcoding-0.2.2/ezcoding/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 15:39:18.831731 ezcoding-0.2.2/ezcoding.egg-info/
--rw-rw-rw-   0        0        0     2004 2024-05-29 15:39:18.000000 ezcoding-0.2.2/ezcoding.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2024-05-29 15:39:18.000000 ezcoding-0.2.2/ezcoding.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 15:39:18.000000 ezcoding-0.2.2/ezcoding.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-29 15:39:18.000000 ezcoding-0.2.2/ezcoding.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-05-29 15:39:18.000000 ezcoding-0.2.2/ezcoding.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-29 15:39:18.000000 ezcoding-0.2.2/ezcoding.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-29 15:39:18.830733 ezcoding-0.2.2/ezcoding_cli/
--rw-rw-rw-   0        0        0       25 2024-05-28 16:51:23.000000 ezcoding-0.2.2/ezcoding_cli/__init__.py
--rw-rw-rw-   0        0        0     1235 2024-05-29 13:56:36.000000 ezcoding-0.2.2/ezcoding_cli/cli.py
--rw-rw-rw-   0        0        0       42 2024-05-29 15:39:18.834725 ezcoding-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1080 2024-05-29 15:38:21.000000 ezcoding-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:25:44.098459 ezcoding-0.2.3/
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:02:10.000000 ezcoding-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2452 2024-06-02 04:25:44.097462 ezcoding-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-06-02 03:28:29.000000 ezcoding-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 04:25:44.074746 ezcoding-0.2.3/ezcoding/
+-rw-rw-rw-   0        0        0      117 2024-06-01 07:04:29.000000 ezcoding-0.2.3/ezcoding/__init__.py
+-rw-rw-rw-   0        0        0      162 2024-05-29 15:09:34.000000 ezcoding-0.2.3/ezcoding/const.py
+-rw-rw-rw-   0        0        0      441 2024-05-24 15:13:49.000000 ezcoding-0.2.3/ezcoding/generator.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:25:44.084698 ezcoding-0.2.3/ezcoding/generators/
+-rw-rw-rw-   0        0        0      308 2024-05-25 12:15:30.000000 ezcoding-0.2.3/ezcoding/generators/__init__.py
+-rw-rw-rw-   0        0        0      946 2024-05-29 14:09:13.000000 ezcoding-0.2.3/ezcoding/generators/author_generator.py
+-rw-rw-rw-   0        0        0      272 2024-05-26 05:11:45.000000 ezcoding-0.2.3/ezcoding/generators/date_string_generator.py
+-rw-rw-rw-   0        0        0     1032 2024-05-29 14:26:52.000000 ezcoding-0.2.3/ezcoding/generators/header_filename_generator.py
+-rw-rw-rw-   0        0        0      888 2024-05-26 05:11:39.000000 ezcoding-0.2.3/ezcoding/generators/header_macro_generator.py
+-rw-rw-rw-   0        0        0      256 2024-05-26 05:11:32.000000 ezcoding-0.2.3/ezcoding/generators/uuid_string_generator.py
+-rw-rw-rw-   0        0        0     3389 2024-06-02 03:52:08.000000 ezcoding-0.2.3/ezcoding/task.py
+-rw-rw-rw-   0        0        0     2537 2024-05-31 15:31:18.000000 ezcoding-0.2.3/ezcoding/template.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:25:44.087689 ezcoding-0.2.3/ezcoding/ui/
+-rw-rw-rw-   0        0        0       93 2024-05-26 03:12:25.000000 ezcoding-0.2.3/ezcoding/ui/__init__.py
+-rw-rw-rw-   0        0        0      164 2024-05-26 03:11:52.000000 ezcoding-0.2.3/ezcoding/ui/application.py
+-rw-rw-rw-   0        0        0     7614 2024-05-29 15:33:21.000000 ezcoding-0.2.3/ezcoding/ui/editor.py
+-rw-rw-rw-   0        0        0      616 2024-06-02 03:51:15.000000 ezcoding-0.2.3/ezcoding/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:25:44.096464 ezcoding-0.2.3/ezcoding.egg-info/
+-rw-rw-rw-   0        0        0     2452 2024-06-02 04:25:43.000000 ezcoding-0.2.3/ezcoding.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2024-06-02 04:25:43.000000 ezcoding-0.2.3/ezcoding.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 04:25:43.000000 ezcoding-0.2.3/ezcoding.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-06-02 04:25:43.000000 ezcoding-0.2.3/ezcoding.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 04:25:43.000000 ezcoding-0.2.3/ezcoding.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-06-02 04:25:43.000000 ezcoding-0.2.3/ezcoding.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 04:25:44.092475 ezcoding-0.2.3/ezcoding_cli/
+-rw-rw-rw-   0        0        0       25 2024-05-28 16:51:23.000000 ezcoding-0.2.3/ezcoding_cli/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-06-01 07:37:55.000000 ezcoding-0.2.3/ezcoding_cli/command.py
+-rw-rw-rw-   0        0        0      901 2024-06-02 04:04:53.000000 ezcoding-0.2.3/ezcoding_cli/command_manager.py
+drwxrwxrwx   0        0        0        0 2024-06-02 04:25:44.095467 ezcoding-0.2.3/ezcoding_cli/commands/
+-rw-rw-rw-   0        0        0      867 2024-06-02 04:07:03.000000 ezcoding-0.2.3/ezcoding_cli/commands/__init__.py
+-rw-rw-rw-   0        0        0     1782 2024-06-02 03:36:15.000000 ezcoding-0.2.3/ezcoding_cli/commands/cmd_create.py
+-rw-rw-rw-   0        0        0     1078 2024-06-02 03:36:31.000000 ezcoding-0.2.3/ezcoding_cli/commands/cmd_help.py
+-rw-rw-rw-   0        0        0      827 2024-06-02 03:36:49.000000 ezcoding-0.2.3/ezcoding_cli/commands/cmd_list_templates.py
+-rw-rw-rw-   0        0        0      690 2024-06-02 04:08:02.000000 ezcoding-0.2.3/ezcoding_cli/main.py
+-rw-rw-rw-   0        0        0      554 2024-06-01 03:16:53.000000 ezcoding-0.2.3/ezcoding_cli/utils.py
+-rw-rw-rw-   0        0        0       42 2024-06-02 04:25:44.098459 ezcoding-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2024-06-02 04:25:28.000000 ezcoding-0.2.3/setup.py
```

### Comparing `ezcoding-0.2.2/LICENSE` & `ezcoding-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2.2/README.md` & `ezcoding-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -64,12 +64,36 @@
 }
 ```
 
 确保将 `ezc.exe` 所在目录添加到环境变量 `Path` 中，使得在任意目录下都可以访问到 `ezc` 命令。
 
 ## 使用
 
-在希望新建文件的目录下，使用命令创建文件。以下命令使用 `Header` 模板，创建文件 `HelloWorld.h`。
+### 创建文件
+
+在希望新建文件的目录下，使用创建子命令（`create`）创建文件。以下命令使用 `Header` 模板，创建文件 `HelloWorld.h`。
+
+子命令后：
+
+- 第一个参数为待创建的文件名。
+- 第二个参数为模板名称。
+- 第三个及以后参数为变量及值对，可以有多个，形式为 `variable=value`。
+
+```shell
+ezc create HelloWorld.h Header Namespace=demo
+```
+
+### 查看模板
+
+使用 `list` 子命令查看模板的目录及模板的名称。
+
+```shell
+ezc list
+```
+
+### 查看帮助
+
+使用 `help` 子命令查看帮助。
 
 ```shell
-ezc --filename HelloWorld.h --template Header
+ezc help
 ```
```

### Comparing `ezcoding-0.2.2/ezcoding/generators/author_generator.py` & `ezcoding-0.2.3/ezcoding/generators/author_generator.py`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2.2/ezcoding/generators/header_filename_generator.py` & `ezcoding-0.2.3/ezcoding/generators/header_filename_generator.py`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2.2/ezcoding/generators/header_macro_generator.py` & `ezcoding-0.2.3/ezcoding/generators/header_macro_generator.py`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2.2/ezcoding/task.py` & `ezcoding-0.2.3/ezcoding/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # -*- coding: utf-8 -*-
 
 import importlib.util
+import os.path
 from pathlib import Path
-from typing import Dict, AnyStr, Union, Optional
+from typing import Dict, AnyStr, Union, Optional, Sequence
 
 from ezcoding.template import Template
 from ezcoding.generator import Generator
 from ezcoding.ui import Application, Editor
 from ezcoding.const import FILENAME_KEY, TEMPLATE_KEY
-from ezcoding.utils import create_variable_macro
+from ezcoding.utils import create_variable_macro, load_module
 
 
 class Task(object):
 
-    def __init__(self, template_dir: Path, template_name: AnyStr):
+    def __init__(self, template_dir: Path, template_name: Optional[AnyStr] = None):
         self.__template_directory: Path = template_dir
-        self.__template_name: AnyStr = template_name
+        self.__template_name: Union[None, AnyStr] = template_name
+
+    def list_templates(self) -> Sequence[AnyStr]:
+        result: list[str] = list()
+        it = self.__template_directory.iterdir()
+        for item in it:
+            if not item.is_file():
+                continue
+            stem, ext = os.path.splitext(item.name)
+            if len(stem) == 0 or ext.lower() != '.py':
+                continue
+            result.append(stem)
+        return result
 
     def run(self, filename: Path, values: Optional[Dict[AnyStr, Union[AnyStr, Generator]]] = None):
+        assert isinstance(self.__template_name, str)
         template = self.__load_template()
         assert isinstance(template, Template)
 
         abs_filename = filename
         if not abs_filename.is_absolute():
             abs_filename = Path.cwd().joinpath(filename)
         value_dict = self.__create_values(abs_filename, template, values)
@@ -31,19 +45,17 @@
 
     def __get_template_path(self) -> Path:
         return Path(self.__template_directory).joinpath(f'{self.__template_name}.py')
 
     def __load_template(self) -> Union[None, Template]:
         try:
             filename = self.__get_template_path()
-            if not filename.is_file():
+            module = load_module(self.__template_name, filename)
+            if module is None:
                 return None
-            spec = importlib.util.spec_from_file_location(self.__template_name, filename)
-            module = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(module)
             template = module.get_template()
             return template
         except:
             return None
 
     def __create_values(
             self,
```

### Comparing `ezcoding-0.2.2/ezcoding/template.py` & `ezcoding-0.2.3/ezcoding/template.py`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2.2/ezcoding/ui/editor.py` & `ezcoding-0.2.3/ezcoding/ui/editor.py`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2.2/ezcoding.egg-info/SOURCES.txt` & `ezcoding-0.2.3/ezcoding.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -19,8 +19,15 @@
 ezcoding/generators/header_filename_generator.py
 ezcoding/generators/header_macro_generator.py
 ezcoding/generators/uuid_string_generator.py
 ezcoding/ui/__init__.py
 ezcoding/ui/application.py
 ezcoding/ui/editor.py
 ezcoding_cli/__init__.py
-ezcoding_cli/cli.py
+ezcoding_cli/command.py
+ezcoding_cli/command_manager.py
+ezcoding_cli/main.py
+ezcoding_cli/utils.py
+ezcoding_cli/commands/__init__.py
+ezcoding_cli/commands/cmd_create.py
+ezcoding_cli/commands/cmd_help.py
+ezcoding_cli/commands/cmd_list_templates.py
```

### Comparing `ezcoding-0.2.2/setup.py` & `ezcoding-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     parser = ConfigParser()
     parser.read(filenames=filename, encoding='utf-8')
     return parser.options('packages')
 
 
 setup(
     name='ezcoding',
-    version='0.2.2',
+    version='0.2.3',
     packages=find_packages(),
     url='https://gitee.com/zhuuuoyue/ezcoding',
     license='MIT',
     author='zhuoy',
     author_email='zhuoyue_cn@yeah.net',
     description='Easy coding',
     long_description=load_readme(),
     long_description_content_type='text/markdown',
     install_requires=load_requires(),
     entry_points={
         'console_scripts': [
-            'ezc = ezcoding_cli.cli:main'
+            'ezc = ezcoding_cli.main:main'
         ]
     }
 )
```

