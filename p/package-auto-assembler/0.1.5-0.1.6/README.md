# Comparing `tmp/package_auto_assembler-0.1.5.tar.gz` & `tmp/package_auto_assembler-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "package_auto_assembler-0.1.5.tar", last modified: Tue May 28 00:48:21 2024, max compression
+gzip compressed data, was "package_auto_assembler-0.1.6.tar", last modified: Sun Jun  2 07:35:01 2024, max compression
```

## Comparing `package_auto_assembler-0.1.5.tar` & `package_auto_assembler-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:48:21.202304 package_auto_assembler-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-28 00:44:05.000000 package_auto_assembler-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28057 2024-05-28 00:48:21.202304 package_auto_assembler-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-28 00:44:05.000000 package_auto_assembler-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:48:21.198304 package_auto_assembler-0.1.5/package_auto_assembler/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:48:07.000000 package_auto_assembler-0.1.5/package_auto_assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76197 2024-05-28 00:48:07.000000 package_auto_assembler-0.1.5/package_auto_assembler/package_auto_assembler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-28 00:48:20.000000 package_auto_assembler-0.1.5/package_auto_assembler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:48:21.202304 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28057 2024-05-28 00:48:21.000000 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 00:48:21.000000 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 00:48:21.000000 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 00:48:21.000000 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 00:48:21.000000 package_auto_assembler-0.1.5/package_auto_assembler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:48:21.202304 package_auto_assembler-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:35:01.280501 package_auto_assembler-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-06-02 07:31:55.000000 package_auto_assembler-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    29056 2024-06-02 07:35:01.280501 package_auto_assembler-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-06-02 07:31:55.000000 package_auto_assembler-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:35:01.276502 package_auto_assembler-0.1.6/package_auto_assembler/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 07:34:48.000000 package_auto_assembler-0.1.6/package_auto_assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79081 2024-06-02 07:34:48.000000 package_auto_assembler-0.1.6/package_auto_assembler/package_auto_assembler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-06-02 07:35:00.000000 package_auto_assembler-0.1.6/package_auto_assembler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 07:35:01.276502 package_auto_assembler-0.1.6/package_auto_assembler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29056 2024-06-02 07:35:01.000000 package_auto_assembler-0.1.6/package_auto_assembler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-02 07:35:01.000000 package_auto_assembler-0.1.6/package_auto_assembler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 07:35:01.000000 package_auto_assembler-0.1.6/package_auto_assembler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 07:35:01.000000 package_auto_assembler-0.1.6/package_auto_assembler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 07:35:01.000000 package_auto_assembler-0.1.6/package_auto_assembler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 07:35:01.280501 package_auto_assembler-0.1.6/setup.cfg
```

### Comparing `package_auto_assembler-0.1.5/LICENSE` & `package_auto_assembler-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `package_auto_assembler-0.1.5/PKG-INFO` & `package_auto_assembler-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package_auto_assembler
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -13,14 +13,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Package auto assembler
+
+Package auto assembler is a tool that meant to streamline creation of single module packages.
+Its purpose is to automate as many aspects of python package creation as possible,
+to shorten a development cycle of reusable components, maintain certain standard of quality
+for reusable code. It provides tool to simplify the process of package creatrion
+to a point that it can be triggered automatically within ci/cd pipelines,
+with minimal preparations and requirements for new modules.
+
 ```python
 import sys
 sys.path.append('../')
 from python_modules.package_auto_assembler import (VersionHandler, \
     ImportMappingHandler, RequirementsHandler, MetadataHandler, \
         LocalDependaciesHandler, LongDocHandler, SetupDirHandler, \
             ReleaseNotesHandler, MkDocsHandler, PackageAutoAssembler)
@@ -762,17 +771,14 @@
     version_increment_type = "patch",
     version = "0.0.1",
     versions_filepath = '../tests/package_auto_assembler/lsts_package_versions.yml',
     log_filepath = '../tests/package_auto_assembler/version_logs.csv'
 )
 ```
 
-    There are no known versions of 'example_module', 0.0.1 will be used!
-
-
 #### Prepare setup directory
 
 
 ```python
 paa.prep_setup_dir()
 ```
 
@@ -847,24 +853,25 @@
 paa.prep_setup_file(
     # optional
     metadata = {'author': 'Kyrylo Mordan',
                 'version': '0.0.1',
                 'description': 'Example module',
                 'keywords': ['python']},
     requirements = ['### example_module.py',
-                    'attr>=22.2.0'],
+                    'attrs>=22.2.0'],
     classifiers = ['Development Status :: 3 - Alpha',
                     'Intended Audience :: Developers',
                     'Intended Audience :: Science/Research',
                     'Programming Language :: Python :: 3',
                     'Programming Language :: Python :: 3.9',
                     'Programming Language :: Python :: 3.10',
                     'Programming Language :: Python :: 3.11',
                     'License :: OSI Approved :: MIT License',
-                    'Topic :: Scientific/Engineering']
+                    'Topic :: Scientific/Engineering'],
+    cli_module_filepath = "../tests/package_auto_assembler/cli.py"
 
 )
 ```
 
 #### Make package
 
 
@@ -874,15 +881,15 @@
     setup_directory = "./example_module"
 )
 ```
 
 
 
 
-    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ninstalling to build/bdist.macosx-10.9-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.macosx-10.9-x86_64/wheel\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1-py3.9.egg-info\nrunning install_scripts\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.macosx-10.9-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.macosx-10.9-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/Users/insani_dei/miniconda3/envs/testenv/lib/python3.9/site-packages/setuptools/_distutils/cmd.py:66: SetuptoolsDeprecationWarning: setup.py install is deprecated.\n!!\n\n        ********************************************************************************\n        Please avoid running ``setup.py`` directly.\n        Instead, use pypa/build, pypa/installer or other\n        standards-based tools.\n\n        See https://blog.ganssle.io/articles/2021/10/setup-py-deprecated.html for details.\n        ********************************************************************************\n\n!!\n  self.initialize_options()\n')
+    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting entry points to example_module.egg-info/entry_points.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/cli.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/entry_points.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ncopying example_module/cli.py -> build/lib/example_module\ninstalling to build/bdist.macosx-10.9-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.macosx-10.9-x86_64/wheel\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/cli.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1-py3.9.egg-info\nrunning install_scripts\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.macosx-10.9-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/cli.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/entry_points.txt'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.macosx-10.9-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/Users/insani_dei/miniconda3/envs/testenv/lib/python3.9/site-packages/setuptools/_distutils/cmd.py:66: SetuptoolsDeprecationWarning: setup.py install is deprecated.\n!!\n\n        ********************************************************************************\n        Please avoid running ``setup.py`` directly.\n        Instead, use pypa/build, pypa/installer or other\n        standards-based tools.\n\n        See https://blog.ganssle.io/articles/2021/10/setup-py-deprecated.html for details.\n        ********************************************************************************\n\n!!\n  self.initialize_options()\n')
 
 
 
 ### 9. Creating release notes from commit messages
 
 
 ```python
```

### Comparing `package_auto_assembler-0.1.5/package_auto_assembler/package_auto_assembler.py` & `package_auto_assembler-0.1.6/package_auto_assembler/package_auto_assembler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1168,14 +1168,15 @@
 
     module_filepath = attr.ib(type=str)
     module_name = attr.ib(default='', type=str)
     metadata = attr.ib(default={}, type=dict)
     requirements = attr.ib(default='', type=str)
     classifiers = attr.ib(default=[], type=list)
     setup_directory = attr.ib(default='./setup_dir')
+    add_cli_tool = attr.ib(default=False, type = bool)
 
     logger = attr.ib(default=None)
     logger_name = attr.ib(default='Package Setup Dir Handler')
     loggerLvl = attr.ib(default=logging.INFO)
     logger_format = attr.ib(default=None)
 
     def __attrs_post_init__(self):
@@ -1254,15 +1255,16 @@
 
     def write_setup_file(self,
                          module_name : str = None,
                          module_docstring : str = None,
                          metadata : dict = None,
                          requirements : str = None,
                          classifiers : list = None,
-                         setup_directory : str = None):
+                         setup_directory : str = None,
+                         add_cli_tool : bool = None):
 
         """
         Create setup.py for the package.
         """
 
         if module_name is None:
             if self.module_name == '':
@@ -1278,24 +1280,35 @@
 
         if classifiers is None:
             classifiers = self.classifiers
 
         if setup_directory is None:
             setup_directory = self.setup_directory
 
+        if add_cli_tool is None:
+            add_cli_tool = self.add_cli_tool
+
         metadata_str = ', '.join([f'{key}="{value}"' for key, value in metadata.items()])
 
         title = module_name.capitalize()
         title = title.replace("_"," ")
 
         long_description_intro = f"""# {title}\n\n"""
 
         if module_docstring:
             long_description_intro += f"""{module_docstring}\n\n"""
 
+        if add_cli_tool:
+            requirements += ['click']
+            entry_points = {
+                'console_scripts': [
+                    f'{module_name} = {module_name}.cli:cli',
+                ]
+            }
+
         setup_content = f"""from setuptools import setup
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 path_to_readme = os.path.join(here, "README.md")
 
@@ -1312,17 +1325,27 @@
 setup(
     name="{module_name}",
     packages=["{module_name}"],
     install_requires={requirements},
     classifiers={classifiers},
     long_description=long_description,
     long_description_content_type='text/markdown',
+"""
+
+        if add_cli_tool:
+            setup_content += f"""
+    entry_points = {entry_points},
+"""
+
+        setup_content += f"""
     {metadata_str}
 )
 """
+
+
         with open(os.path.join(setup_directory, 'setup.py'), 'w') as file:
             file.write(setup_content)
 
 @attr.s
 class ReleaseNotesHandler:
 
     # inputs
@@ -1891,24 +1914,71 @@
             os.chdir(project_name)
             subprocess.run(["mkdocs", "serve"])
         except Exception as e:
             print(e)
         finally:
             os.chdir("..")
 
+@attr.s
+class CliHandler:
+
+    # inputs
+    cli_module_filepath = attr.ib()
+    setup_directory = attr.ib()
+
+    # processed
+    logger = attr.ib(default=None)
+    logger_name = attr.ib(default='MkDocs Handler')
+    loggerLvl = attr.ib(default=logging.INFO)
+    logger_format = attr.ib(default=None)
+
+    def __attrs_post_init__(self):
+        self._initialize_logger()
+
+    def _initialize_logger(self):
+        """
+        Initialize a logger for the class instance based on the specified logging level and logger name.
+        """
+
+        if self.logger is None:
+            logging.basicConfig(level=self.loggerLvl, format=self.logger_format)
+            logger = logging.getLogger(self.logger_name)
+            logger.setLevel(self.loggerLvl)
+
+            self.logger = logger
+
+    def prepare_script(self,
+                       cli_module_filepath: str = None,
+                       setup_directory : str = None):
+
+        """
+        Prepare cli script for packaging.
+        """
+
+        if cli_module_filepath is None:
+            cli_module_filepath = self.cli_module_filepath
+
+        if setup_directory is None:
+            setup_directory = self.setup_directory
+
+        # Copying module to setup directory
+        shutil.copy(cli_module_filepath, os.path.join(setup_directory, "cli.py"))
+
+        return True
 
 @attr.s
 class PackageAutoAssembler:
     # pylint: disable=too-many-instance-attributes
 
     ## inputs
     module_name = attr.ib(type=str)
 
     ## paths
     module_filepath = attr.ib(type=str)
+    cli_module_filepath = attr.ib(default=None)
     mapping_filepath = attr.ib(default=None)
     dependencies_dir = attr.ib(default=None)
     example_notebook_path = attr.ib(default=None)
     versions_filepath = attr.ib(default='./lsts_package_versions.yml')
     log_filepath = attr.ib(default='./version_logs.csv')
     setup_directory = attr.ib(default='./setup_dir')
 
@@ -1934,25 +2004,28 @@
     setup_dir_h_class = attr.ib(default=SetupDirHandler)
     version_h_class = attr.ib(default=VersionHandler)
     import_mapping_h_class = attr.ib(default=ImportMappingHandler)
     local_dependacies_h_class = attr.ib(default=LocalDependaciesHandler)
     requirements_h_class = attr.ib(default=RequirementsHandler)
     metadata_h_class = attr.ib(default=MetadataHandler)
     long_doc_h_class = attr.ib(default=LongDocHandler)
+    cli_h_class = attr.ib(default=CliHandler)
 
     ## handlers
     setup_dir_h = attr.ib(default = None, type = SetupDirHandler)
     version_h = attr.ib(default = None, type = VersionHandler)
     import_mapping_h = attr.ib(default = None, type=ImportMappingHandler)
     local_dependacies_h = attr.ib(default = None, type=LocalDependaciesHandler)
     requirements_h = attr.ib(default = None, type=RequirementsHandler)
     metadata_h = attr.ib(default = None, type=MetadataHandler)
     long_doc_h = attr.ib(default = None, type=LongDocHandler)
+    cli_h = attr.ib(default = None, type=CliHandler)
 
     ## output
+    add_cli_tool = attr.ib(default = None, type = bool)
     package_result = attr.ib(init=False)
     metadata = attr.ib(init=False)
 
     logger = attr.ib(default=None)
     logger_name = attr.ib(default='Package Auto Assembler')
     loggerLvl = attr.ib(default=logging.INFO)
     logger_format = attr.ib(default=None)
@@ -2044,14 +2117,25 @@
 
         self.setup_dir_h = self.setup_dir_h_class(
             module_name = self.module_name,
             module_filepath = self.module_filepath,
             setup_directory = self.setup_directory,
             logger = self.logger)
 
+    def _initialize_cli_handler(self):
+
+        """
+        Initialize cli handler with available parameters.
+        """
+
+        self.cli_h = self.cli_h_class(
+            cli_module_filepath = self.cli_module_filepath,
+            setup_directory = self.setup_directory,
+            logger = self.logger)
+
     def add_metadata_from_module(self, module_filepath : str = None):
 
         """
         Add metadata extracted from the module.
         """
 
         if self.metadata_h is None:
@@ -2216,27 +2300,31 @@
                 notebook_path = example_notebook_path,
                 output_path = output_path
             )
 
 
     def prep_setup_file(self,
                        module_name : str = None,
+                       cli_module_filepath : str = None,
                        metadata : dict = None,
                        requirements : str = None,
                        classifiers : list = None,
                        module_filepath : str = None,
                        module_docstring : str = None):
 
         """
         Assemble setup.py file.
         """
 
         if self.setup_dir_h is None:
             self._initialize_setup_dir_handler()
 
+        if cli_module_filepath is None:
+            cli_module_filepath = self.cli_module_filepath
+
         if metadata is None:
             metadata = self.metadata
 
         if requirements is None:
             requirements = self.requirements_list
 
         if classifiers is None:
@@ -2253,20 +2341,31 @@
             if self.long_doc_h is None:
                 self._initialize_long_doc_handler()
 
             module_content = self.long_doc_h.read_module_content(filepath = module_filepath)
 
             module_docstring = self.long_doc_h.extract_module_docstring(module_content = module_content)
 
+        add_cli_tool = None
+        if cli_module_filepath:
+
+            if self.cli_h is None:
+                self._initialize_cli_handler()
+
+            add_cli_tool = self.cli_h.prepare_script(
+                cli_module_filepath = cli_module_filepath
+            )
+
         # create setup.py
         self.setup_dir_h.write_setup_file(module_name = module_name,
                                           module_docstring = module_docstring,
                                           metadata = metadata,
                                           requirements = requirements,
-                                          classifiers = classifiers)
+                                          classifiers = classifiers,
+                                          add_cli_tool = add_cli_tool)
 
     def make_package(self,
                      setup_directory : str = None):
 
         """
         Create a package.
         """
```

### Comparing `package_auto_assembler-0.1.5/package_auto_assembler.egg-info/PKG-INFO` & `package_auto_assembler-0.1.6/package_auto_assembler.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package-auto-assembler
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -13,14 +13,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Package auto assembler
+
+Package auto assembler is a tool that meant to streamline creation of single module packages.
+Its purpose is to automate as many aspects of python package creation as possible,
+to shorten a development cycle of reusable components, maintain certain standard of quality
+for reusable code. It provides tool to simplify the process of package creatrion
+to a point that it can be triggered automatically within ci/cd pipelines,
+with minimal preparations and requirements for new modules.
+
 ```python
 import sys
 sys.path.append('../')
 from python_modules.package_auto_assembler import (VersionHandler, \
     ImportMappingHandler, RequirementsHandler, MetadataHandler, \
         LocalDependaciesHandler, LongDocHandler, SetupDirHandler, \
             ReleaseNotesHandler, MkDocsHandler, PackageAutoAssembler)
@@ -762,17 +771,14 @@
     version_increment_type = "patch",
     version = "0.0.1",
     versions_filepath = '../tests/package_auto_assembler/lsts_package_versions.yml',
     log_filepath = '../tests/package_auto_assembler/version_logs.csv'
 )
 ```
 
-    There are no known versions of 'example_module', 0.0.1 will be used!
-
-
 #### Prepare setup directory
 
 
 ```python
 paa.prep_setup_dir()
 ```
 
@@ -847,24 +853,25 @@
 paa.prep_setup_file(
     # optional
     metadata = {'author': 'Kyrylo Mordan',
                 'version': '0.0.1',
                 'description': 'Example module',
                 'keywords': ['python']},
     requirements = ['### example_module.py',
-                    'attr>=22.2.0'],
+                    'attrs>=22.2.0'],
     classifiers = ['Development Status :: 3 - Alpha',
                     'Intended Audience :: Developers',
                     'Intended Audience :: Science/Research',
                     'Programming Language :: Python :: 3',
                     'Programming Language :: Python :: 3.9',
                     'Programming Language :: Python :: 3.10',
                     'Programming Language :: Python :: 3.11',
                     'License :: OSI Approved :: MIT License',
-                    'Topic :: Scientific/Engineering']
+                    'Topic :: Scientific/Engineering'],
+    cli_module_filepath = "../tests/package_auto_assembler/cli.py"
 
 )
 ```
 
 #### Make package
 
 
@@ -874,15 +881,15 @@
     setup_directory = "./example_module"
 )
 ```
 
 
 
 
-    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ninstalling to build/bdist.macosx-10.9-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.macosx-10.9-x86_64/wheel\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1-py3.9.egg-info\nrunning install_scripts\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.macosx-10.9-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.macosx-10.9-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/Users/insani_dei/miniconda3/envs/testenv/lib/python3.9/site-packages/setuptools/_distutils/cmd.py:66: SetuptoolsDeprecationWarning: setup.py install is deprecated.\n!!\n\n        ********************************************************************************\n        Please avoid running ``setup.py`` directly.\n        Instead, use pypa/build, pypa/installer or other\n        standards-based tools.\n\n        See https://blog.ganssle.io/articles/2021/10/setup-py-deprecated.html for details.\n        ********************************************************************************\n\n!!\n  self.initialize_options()\n')
+    CompletedProcess(args=['python', './example_module/setup.py', 'sdist', 'bdist_wheel'], returncode=0, stdout="running sdist\nrunning egg_info\nwriting example_module.egg-info/PKG-INFO\nwriting dependency_links to example_module.egg-info/dependency_links.txt\nwriting entry points to example_module.egg-info/entry_points.txt\nwriting requirements to example_module.egg-info/requires.txt\nwriting top-level names to example_module.egg-info/top_level.txt\nreading manifest file 'example_module.egg-info/SOURCES.txt'\nwriting manifest file 'example_module.egg-info/SOURCES.txt'\nrunning check\ncreating example_module-0.0.1\ncreating example_module-0.0.1/example_module\ncreating example_module-0.0.1/example_module.egg-info\ncopying files to example_module-0.0.1...\ncopying example_module/__init__.py -> example_module-0.0.1/example_module\ncopying example_module/cli.py -> example_module-0.0.1/example_module\ncopying example_module/example_module.py -> example_module-0.0.1/example_module\ncopying example_module/setup.py -> example_module-0.0.1/example_module\ncopying example_module.egg-info/PKG-INFO -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/dependency_links.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/entry_points.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/requires.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/top_level.txt -> example_module-0.0.1/example_module.egg-info\ncopying example_module.egg-info/SOURCES.txt -> example_module-0.0.1/example_module.egg-info\nWriting example_module-0.0.1/setup.cfg\ncreating dist\nCreating tar archive\nremoving 'example_module-0.0.1' (and everything under it)\nrunning bdist_wheel\nrunning build\nrunning build_py\ncopying example_module/example_module.py -> build/lib/example_module\ncopying example_module/__init__.py -> build/lib/example_module\ncopying example_module/setup.py -> build/lib/example_module\ncopying example_module/cli.py -> build/lib/example_module\ninstalling to build/bdist.macosx-10.9-x86_64/wheel\nrunning install\nrunning install_lib\ncreating build/bdist.macosx-10.9-x86_64/wheel\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/example_module.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/__init__.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/setup.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\ncopying build/lib/example_module/cli.py -> build/bdist.macosx-10.9-x86_64/wheel/example_module\nrunning install_egg_info\nCopying example_module.egg-info to build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1-py3.9.egg-info\nrunning install_scripts\ncreating build/bdist.macosx-10.9-x86_64/wheel/example_module-0.0.1.dist-info/WHEEL\ncreating 'dist/example_module-0.0.1-py3-none-any.whl' and adding 'build/bdist.macosx-10.9-x86_64/wheel' to it\nadding 'example_module/__init__.py'\nadding 'example_module/cli.py'\nadding 'example_module/example_module.py'\nadding 'example_module/setup.py'\nadding 'example_module-0.0.1.dist-info/METADATA'\nadding 'example_module-0.0.1.dist-info/WHEEL'\nadding 'example_module-0.0.1.dist-info/entry_points.txt'\nadding 'example_module-0.0.1.dist-info/top_level.txt'\nadding 'example_module-0.0.1.dist-info/RECORD'\nremoving build/bdist.macosx-10.9-x86_64/wheel\n", stderr='warning: sdist: standard file not found: should have one of README, README.rst, README.txt, README.md\n\n/Users/insani_dei/miniconda3/envs/testenv/lib/python3.9/site-packages/setuptools/_distutils/cmd.py:66: SetuptoolsDeprecationWarning: setup.py install is deprecated.\n!!\n\n        ********************************************************************************\n        Please avoid running ``setup.py`` directly.\n        Instead, use pypa/build, pypa/installer or other\n        standards-based tools.\n\n        See https://blog.ganssle.io/articles/2021/10/setup-py-deprecated.html for details.\n        ********************************************************************************\n\n!!\n  self.initialize_options()\n')
 
 
 
 ### 9. Creating release notes from commit messages
 
 
 ```python
```

