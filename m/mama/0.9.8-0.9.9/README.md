# Comparing `tmp/mama-0.9.8.tar.gz` & `tmp/mama-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mama-0.9.8.tar", last modified: Tue May 28 15:29:38 2024, max compression
+gzip compressed data, was "mama-0.9.9.tar", last modified: Sun Jun  2 15:57:49 2024, max compression
```

## Comparing `mama-0.9.8.tar` & `mama-0.9.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.805647 mama-0.9.8/
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2024-01-20 16:30:57.000000 mama-0.9.8/LICENSE
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-28 15:29:38.805647 mama-0.9.8/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11351 2024-03-25 09:35:15.000000 mama-0.9.8/README.md
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.795647 mama-0.9.8/mama/
--rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2024-01-20 16:30:57.000000 mama-0.9.8/mama/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11805 2024-03-25 09:35:15.000000 mama-0.9.8/mama/artifactory.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    40004 2024-05-02 07:54:51.000000 mama-0.9.8/mama/build_config.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    24912 2024-03-25 09:35:15.000000 mama-0.9.8/mama/build_dependency.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    55602 2024-05-02 07:54:51.000000 mama-0.9.8/mama/build_target.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11779 2024-04-07 19:34:43.000000 mama-0.9.8/mama/cmake_configure.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    16670 2024-04-30 10:10:25.000000 mama-0.9.8/mama/dependency_chain.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2024-01-20 16:30:57.000000 mama-0.9.8/mama/init_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12378 2024-03-25 09:35:15.000000 mama-0.9.8/mama/main.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2024-01-20 16:30:57.000000 mama-0.9.8/mama/msbuild.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     9665 2024-04-30 10:23:16.000000 mama-0.9.8/mama/package.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     7757 2024-03-25 09:35:15.000000 mama-0.9.8/mama/papa_deploy.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3778 2024-03-25 09:35:15.000000 mama-0.9.8/mama/papa_upload.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1763 2024-03-25 09:35:15.000000 mama-0.9.8/mama/parse_mamafile.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.805647 mama-0.9.8/mama/platforms/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.8/mama/platforms/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     8558 2024-01-20 16:30:57.000000 mama-0.9.8/mama/platforms/android.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5376 2024-01-20 16:30:57.000000 mama-0.9.8/mama/platforms/mips.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5644 2024-03-25 09:35:15.000000 mama-0.9.8/mama/platforms/oclea.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.805647 mama-0.9.8/mama/types/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.8/mama/types/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2024-01-20 16:30:57.000000 mama-0.9.8/mama/types/artifactory_pkg.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2024-01-20 16:30:57.000000 mama-0.9.8/mama/types/asset.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2024-01-20 16:30:57.000000 mama-0.9.8/mama/types/dep_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    15161 2024-04-07 19:34:43.000000 mama-0.9.8/mama/types/git.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2024-01-20 16:30:57.000000 mama-0.9.8/mama/types/local_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    17510 2024-03-25 09:35:15.000000 mama-0.9.8/mama/util.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.805647 mama-0.9.8/mama/utils/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.8/mama/utils/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1637 2024-01-20 16:30:57.000000 mama-0.9.8/mama/utils/gdb.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    17034 2024-03-25 09:35:15.000000 mama-0.9.8/mama/utils/gnu_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1063 2024-05-28 15:28:16.000000 mama-0.9.8/mama/utils/gtest.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2024-01-20 16:30:57.000000 mama-0.9.8/mama/utils/nonblocking_io.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3789 2024-04-30 09:51:39.000000 mama-0.9.8/mama/utils/run.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    10345 2024-04-07 19:34:43.000000 mama-0.9.8/mama/utils/sub_process.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1310 2024-05-02 08:29:37.000000 mama-0.9.8/mama/utils/system.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-28 15:29:38.805647 mama-0.9.8/mama.egg-info/
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)      921 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/SOURCES.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/dependency_links.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/entry_points.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/requires.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2024-05-28 15:29:38.000000 mama-0.9.8/mama.egg-info/top_level.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2024-05-28 15:26:08.000000 mama-0.9.8/pyproject.toml
--rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2024-05-28 15:29:38.805647 mama-0.9.8/setup.cfg
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-06-02 15:57:49.068556 mama-0.9.9/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2024-01-20 16:30:57.000000 mama-0.9.9/LICENSE
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-06-02 15:57:49.068556 mama-0.9.9/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11351 2024-03-25 09:35:15.000000 mama-0.9.9/README.md
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-06-02 15:57:49.058555 mama-0.9.9/mama/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2024-01-20 16:30:57.000000 mama-0.9.9/mama/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11871 2024-06-02 12:10:17.000000 mama-0.9.9/mama/artifactory.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    41347 2024-06-02 14:52:32.000000 mama-0.9.9/mama/build_config.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    25952 2024-06-02 15:13:25.000000 mama-0.9.9/mama/build_dependency.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    55602 2024-05-02 07:54:51.000000 mama-0.9.9/mama/build_target.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12958 2024-06-02 15:05:39.000000 mama-0.9.9/mama/cmake_configure.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    16670 2024-04-30 10:10:25.000000 mama-0.9.9/mama/dependency_chain.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2024-01-20 16:30:57.000000 mama-0.9.9/mama/init_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    13853 2024-06-02 15:55:50.000000 mama-0.9.9/mama/main.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2024-01-20 16:30:57.000000 mama-0.9.9/mama/msbuild.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     9665 2024-04-30 10:23:16.000000 mama-0.9.9/mama/package.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     7757 2024-03-25 09:35:15.000000 mama-0.9.9/mama/papa_deploy.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3778 2024-03-25 09:35:15.000000 mama-0.9.9/mama/papa_upload.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1763 2024-03-25 09:35:15.000000 mama-0.9.9/mama/parse_mamafile.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-06-02 15:57:49.058555 mama-0.9.9/mama/platforms/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.9/mama/platforms/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     8558 2024-01-20 16:30:57.000000 mama-0.9.9/mama/platforms/android.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5376 2024-01-20 16:30:57.000000 mama-0.9.9/mama/platforms/mips.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5644 2024-03-25 09:35:15.000000 mama-0.9.9/mama/platforms/oclea.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-06-02 15:57:49.058555 mama-0.9.9/mama/types/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.9/mama/types/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2024-01-20 16:30:57.000000 mama-0.9.9/mama/types/artifactory_pkg.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2024-01-20 16:30:57.000000 mama-0.9.9/mama/types/asset.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2024-01-20 16:30:57.000000 mama-0.9.9/mama/types/dep_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    15161 2024-04-07 19:34:43.000000 mama-0.9.9/mama/types/git.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2024-01-20 16:30:57.000000 mama-0.9.9/mama/types/local_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    17510 2024-03-25 09:35:15.000000 mama-0.9.9/mama/util.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-06-02 15:57:49.068556 mama-0.9.9/mama/utils/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.9/mama/utils/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     2098 2024-06-02 14:49:37.000000 mama-0.9.9/mama/utils/gdb.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    17034 2024-03-25 09:35:15.000000 mama-0.9.9/mama/utils/gnu_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1091 2024-06-02 14:21:14.000000 mama-0.9.9/mama/utils/gtest.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2024-01-20 16:30:57.000000 mama-0.9.9/mama/utils/nonblocking_io.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3789 2024-04-30 09:51:39.000000 mama-0.9.9/mama/utils/run.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    10345 2024-04-07 19:34:43.000000 mama-0.9.9/mama/utils/sub_process.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1310 2024-05-02 08:29:37.000000 mama-0.9.9/mama/utils/system.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-06-02 15:57:49.068556 mama-0.9.9/mama.egg-info/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-06-02 15:57:49.000000 mama-0.9.9/mama.egg-info/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      921 2024-06-02 15:57:49.000000 mama-0.9.9/mama.egg-info/SOURCES.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2024-06-02 15:57:49.000000 mama-0.9.9/mama.egg-info/dependency_links.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2024-06-02 15:57:49.000000 mama-0.9.9/mama.egg-info/entry_points.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2024-06-02 15:57:49.000000 mama-0.9.9/mama.egg-info/requires.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2024-06-02 15:57:49.000000 mama-0.9.9/mama.egg-info/top_level.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2024-06-02 12:16:33.000000 mama-0.9.9/pyproject.toml
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2024-06-02 15:57:49.068556 mama-0.9.9/setup.cfg
```

### Comparing `mama-0.9.8/LICENSE` & `mama-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/PKG-INFO` & `mama-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.9.8
+Version: 0.9.9
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.9.8/README.md` & `mama-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/artifactory.py` & `mama-0.9.9/mama/artifactory.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 
     name = target.name
     # triplets information to make this package platform unique
     platform, os_major, _ = target.config.get_distro_info()
     compiler = target.config.compiler_version()
     arch = target.config.arch # eg 'x86', 'arm64'
     build_type = 'release' if target.config.release else 'debug'
+    if target.config.sanitize:
+        build_type += '-sanitized'
 
     return f'{name}-{platform}-{os_major}-{compiler}-{arch}-{build_type}-{version}'
 
 
 keyr = None
 def _get_keyring():
     global keyr
```

### Comparing `mama-0.9.8/mama/build_config.py` & `mama-0.9.9/mama/build_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,18 @@
         self.dirty     = False # marks a target for rebuild on next build even if it's up to date
         self.unshallow = False  # by default, git clones are shallow, this allows unshallowing
         self.mama_init = False
         self.print     = True
         self.verbose   = False
         self.test      = ''
         self.start     = ''
+        self.with_tests = False # forces -DENABLE_TESTS=ON
+        self.sanitize  = None # gcc/clang: -fsanitize=[thread|leak|address|undefined]
+        self.coverage  = None # gcc/clang: gcov | windows: /fsanitize-coverage=edge
+        self.coverage_report = None # runs gcovr to generate coverage report
         # supported platforms
         self.windows = False
         self.linux   = False
         self.macos   = False
         self.ios     = False
         self.android : Android = None
         self.raspi   = False
@@ -132,14 +136,24 @@
             elif arg == 'init':      self.mama_init = True
             elif arg == 'silent':    self.print = False
             elif arg == 'verbose':   self.verbose = True
             elif arg == 'parallel':  self.parallel_load = True
             elif arg == 'all':       self.target = 'all'
             elif arg == 'test':      self.test = ' ' # no test arguments
             elif arg == 'start':     self.start = ' ' # no start arguments
+            elif arg == 'with_tests': self.with_tests = True
+            elif arg.startswith('sanitize='): self.add_sanitizer_option(arg[9:])
+            elif arg == 'asan':    self.add_sanitizer_option('address')
+            elif arg == 'lsan':    self.add_sanitizer_option('leak')
+            elif arg == 'tsan':    self.add_sanitizer_option('thread')
+            elif arg == 'ubsan':   self.add_sanitizer_option('undefined')
+            elif arg.startswith('coverage='): self.add_coverage_option(arg[9:])
+            elif arg == 'coverage': self.add_coverage_option()
+            elif arg == 'coverage-report': self.coverage_report = '.'
+            elif arg.startswith('coverage-report='): self.coverage_report = arg[16:]
             elif arg == 'windows': self.set_platform(windows=True)
             elif arg == 'linux':   self.set_platform(linux=True)
             elif arg == 'macos':   self.set_platform(macos=True)
             elif arg == 'ios':     self.set_platform(ios=True)
             elif arg == 'android': self.set_platform(android=True)
             elif arg == 'raspi':   self.set_platform(raspi=True)
             elif arg == 'oclea':   self.set_platform(oclea=True)
@@ -562,14 +576,24 @@
         for ninja_exe in ninja_executables:        
             if ninja_exe and os.path.isfile(ninja_exe):
                 if self.verbose: console(f'Found Ninja Build System: {ninja_exe}')
                 return ninja_exe
         return ''
 
 
+    def add_sanitizer_option(self, option):
+        if self.sanitize: self.sanitize += ',' + option
+        else:             self.sanitize = option
+
+
+    def add_coverage_option(self, option='default'):
+        if self.coverage: self.coverage += ',' + option
+        else:             self.coverage = option
+
+
     def append_env_path(self, paths, env):
         path = os.getenv(env)
         if path: paths.append(path)
 
 
     def raspi_bin(self):
         if not self.raspi_compilers: self.init_raspi_path()
```

### Comparing `mama-0.9.8/mama/build_dependency.py` & `mama-0.9.9/mama/build_dependency.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os, sys, shutil, time
 
 from .types.dep_source import DepSource
 from .types.git import Git
 from .types.local_source import LocalSource
 from .utils.system import Color, console, error
 from .artifactory import artifactory_fetch_and_reconfigure
-from .util import normalized_join, normalized_path, write_text_to, read_lines_from
+from .util import normalized_join, normalized_path, read_text_from, write_text_to, read_lines_from
 from .parse_mamafile import parse_mamafile, update_mamafile_tag, update_cmakelists_tag
 import mama.package as package
 
 
 if TYPE_CHECKING:
     from .build_config import BuildConfig
     from .build_target import BuildTarget
@@ -511,14 +511,47 @@
 
 
     def build_file_exists(self, filename):
         """ TRUE if a file relative to build_dir exists """
         return os.path.exists(normalized_join(self.build_dir, filename))
 
 
+    def sanitizer_list_path(self):
+        return normalized_join(self.build_dir, 'enabled_sanitizers')
+
+
+    def get_enabled_sanitizers(self):
+        list_path = self.sanitizer_list_path()
+        if os.path.exists(list_path):
+            return read_text_from(list_path)
+        return ''
+
+
+    def save_enabled_sanitizers(self):
+        if self.target.config.sanitize:
+            write_text_to(self.sanitizer_list_path(), self.target.config.sanitize)
+        else: # otherwise delete the file, which means sanitizer was not used
+            os.remove(self.sanitizer_list_path())
+
+
+    def coverage_enabled_path(self):
+        return normalized_join(self.build_dir, 'enabled_coverage')
+
+
+    def get_enabled_coverage(self):
+        return os.path.exists(self.coverage_enabled_path())
+
+
+    def save_enabled_coverage(self):
+        if self.target.config.coverage:
+            write_text_to(self.coverage_enabled_path(), self.target.config.coverage)
+        else:
+            os.remove(self.coverage_enabled_path())
+    
+
     def path_relative_to_us(self, relpath) -> str:
         """
         Converts relative path into an absolute path based on self mamafile location
         """
         if not relpath or os.path.isabs(relpath):
             return relpath # the path is already None, or Absolute
         elif self.mamafile: # if we have mamafile, set path relative to it
```

### Comparing `mama-0.9.8/mama/build_target.py` & `mama-0.9.9/mama/build_target.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/cmake_configure.py` & `mama-0.9.9/mama/cmake_configure.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     exit_status = SubProcess.run(cmd, cwd, io_func=handle_output)
 
     if rerun and allow_rerun:
         if target.config.print: console('Rerunning CMake configure')
         return _rerunnable_cmake_conf(cmd, cwd, False, target, delete_cmakecache=delete_cmakecache)
     if exit_status != 0:
         raise Exception(f'CMake configure error: {error}')
+    target.dep.save_enabled_sanitizers()
+    target.dep.save_enabled_coverage()
 
 
 def run_config(target:BuildTarget):
     if not target.config.update and os.path.exists(target.build_dir('CMakeCache.txt')):
         if target.config.verbose:
             console('Not running CMake configure because CMakeCache.txt exists and `update` was not specified')
         return
@@ -132,15 +134,16 @@
     cxxflags:dict = target.cmake_cxxflags
     ldflags:dict = target.cmake_ldflags
     exceptions = target.enable_exceptions
 
     def add_flag(flag:str, value=''):
         if not flag in cxxflags:  # add flag if not already set
             cxxflags[flag] = value
-    #def add_ldflag(flag:str, value=''): ldflags[flag] = value
+    def add_ldflag(flag:str, value=''):
+        ldflags[flag] = value
     def get_flags_string(flags:dict):
         res = ''
         sep = ':' if config.windows else '='
         for k, v in flags.items():
             if not v:
                 res += f' {k}'
             elif k.startswith('-D') and not '=' in k:
@@ -183,35 +186,64 @@
         config.oclea.get_cxx_flags(add_flag)
     elif config.mips:
         config.mips.get_cxx_flags(add_flag)
 
     if config.flags:
         add_flag(config.flags)
 
+    ld_sanitize = ''
+    ld_coverage = ''
+
+    if config.sanitize:
+        if config.gcc or config.clang:
+            ld_sanitize = f'-fsanitize={config.sanitize}'
+            add_flag('-fsanitize', config.sanitize)
+            add_flag('-fno-omit-frame-pointer')
+            add_flag('-pie')
+            add_flag('-fPIE')
+        elif config.windows: # ASSUMES MSVC
+            ld_sanitize = f'/fsanitize={config.sanitize}'
+
+    if config.coverage:
+        if config.gcc or config.clang:
+            add_flag('--coverage')
+            add_flag('-fprofile-abs-path') # use absolute paths to always find coverage info
+            ld_coverage='--coverage'
+        elif config.windows: # ASSUMES MSVC
+            option = 'edge' if config.coverage == 'default' else config.coverage
+            add_flag('/fsanitize-coverage', option)
+
     opt = [
         "CMAKE_POSITION_INDEPENDENT_CODE=ON",
         "CMAKE_EXPORT_COMPILE_COMMANDS=ON" # for tools like clang-tidy and .vscode intellisense
     ]
+    if config.with_tests:
+        opt += ["ENABLE_TESTS=ON", "BUILD_TESTS=ON"]
+    
     if config.linux or config.raspi or config.oclea or config.mips:
         opt += _custom_compilers(target)
     
     if target.enable_fortran_build and config.fortran:
         opt += [f'CMAKE_Fortran_COMPILER={config.fortran}']
 
     cxxflags_str = get_flags_string(cxxflags)
     if cxxflags_str and target.enable_cxx_build:
         opt += [f'CMAKE_CXX_FLAGS="{cxxflags_str}"']
 
     ldflags_str = get_flags_string(ldflags)
-    if ldflags_str: opt += [
-        f'CMAKE_EXE_LINKER_FLAGS="{ldflags_str}"',
-        f'CMAKE_MODULE_LINKER_FLAGS="{ldflags_str}"',
-        f'CMAKE_SHARED_LINKER_FLAGS="{ldflags_str}"',
-        f'CMAKE_STATIC_LINKER_FLAGS="{ldflags_str}"'
-    ]
+    if ldflags_str:
+        exe_ldflags = ldflags_str
+        if ld_sanitize: exe_ldflags += ' ' + ld_sanitize
+        if ld_coverage: exe_ldflags += ' ' + ld_coverage
+        opt += [
+            f'CMAKE_EXE_LINKER_FLAGS="{exe_ldflags}"',
+            f'CMAKE_MODULE_LINKER_FLAGS="{exe_ldflags}"',
+            f'CMAKE_SHARED_LINKER_FLAGS="{exe_ldflags}"',
+            f'CMAKE_STATIC_LINKER_FLAGS="{ldflags_str}"'
+        ]
 
     make = _make_program(target)
     if make: opt.append(f'CMAKE_MAKE_PROGRAM="{make}"')
 
     if config.windows:
         if config.is_target_arch_x86(): ## need to override the toolset host
             opt.append('CMAKE_GENERATOR_TOOLSET=host=x86')
```

### Comparing `mama-0.9.8/mama/dependency_chain.py` & `mama-0.9.9/mama/dependency_chain.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/init_project.py` & `mama-0.9.9/mama/init_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/main.py` & `mama-0.9.9/mama/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,19 @@
     console('    release    - (default) CMake configuration RelWithDebInfo')
     console('    debug      - CMake configuration Debug')
     console('    arch=x86   - Override cross-compiling architecture: (x86, x64, arm, arm64)')
     console('    x86        - Shorthand for arch=x86, all shorthands: x86 x64 arm arm64')
     console('    jobs=N     - Max number of parallel compilations. (default=system.core.count)')
     console('    target=P   - Name of the target')
     console('    all        - Short for target=all')
+    console('    with_tests - Forces CMake option -DENABLE_TESTS=ON and -DBUILD_TESTS=ON')
+    console('    sanitize=  - enables -fsanitize= for gcc/clang builds [address|leak|thread|undefined]')
+    console('    asan|lsan|tsan|ubsan - shorthands for sanitize=address|leak|thread|undefined respectively')
+    console('    coverage   - Builds the project with GCC --coverage option')
+    console('    coverage-report[=src_root] - Generates coverage report using gcovr')
     console('    silent     - Greatly reduces verbosity')
     console('    verbose    - Greatly increases verbosity for build dependencies and cmake')
     console('  examples:')
     console('    mama init                      Initialize a new project. Tries to create mamafile.py and CMakeLists.txt')
     console('    mama build                     Update and build main project only. This only clones, but does not update!')
     console('    mama build x86 opencv          Cross compile build target opencv to x86 architecture')
     console('    mama build android             Cross compile to arm64 android NDK')
@@ -79,14 +84,16 @@
     console('    mama wipe dep1                 Wipe target dependency completely and clone again. Does not build!')
     console('    mama upload dep1               Deploys and uploads dependency to Artifactory server.')
     console('    mama test                      Run tests on main project.')
     console('    mama test=arg                  Run tests on main project with an argument.')
     console('    mama test="arg1 arg2"          Run tests on main project with multiple arguments.')
     console('    mama test dep1                 Run tests on target dependency project.')
     console('    mama start=dbtool              Call main project mamafile start() with args [`dbtool`].')
+    console('    mama rebuild all tsan lsan     Rebuild all targets with thread and leak sanitizers enabled.')
+    console('    mama rebuild all sanitize=leak,undefined Rebuild all targets with leak and undefined sanitizers enabled.')
     console('  environment:')
     console('    setenv("NINJA")                  Path to NINJA build executable')
     console('    setenv("ANDROID_HOME")           Path to Android SDK if auto-detect fails')
     console('    setenv("MAMA_ARTIFACTORY_USER")  Username for Artifactory server')
     console('    setenv("MAMA_ARTIFACTORY_PASS")  Password for Artifactory server')
 
 
@@ -153,14 +160,24 @@
         used_by = ", ".join([d.name for d in dirty_chain]) if dirty_chain else 'none'
         console(f'    Target {dep.name} used by: {used_by}')
     dep.dirty()
     for d in dirty_chain:
         d.dirty()
 
 
+def run_coverage_report(target: BuildTarget):
+    if target.config.windows:
+        console('Coverage report not supported yet on Windows')
+        return
+    root = target.source_dir(target.config.coverage_report)
+    target.config.verbose = True # enable verbose mode before running the command
+    cmd = f'gcovr --sort-percentage --root {root} {target.build_dir()}'
+    target.run(cmd, src_dir=True)
+
+
 def main():
     if sys.version_info < (3, 6):
         console('FATAL ERROR: MamaBuild requires Python 3.6')
         exit(-1)
 
     if len(sys.argv) == 1 or 'help' in sys.argv:
         print_title()
@@ -209,40 +226,42 @@
 
     if config.clean and not config.target:
         root.clean()
 
     load_dependency_chain(root)
     check_config_target(config, root)
 
+    # get the main target dependency
+    if config.target:
+        dep = find_dependency(root, config.target)
+    else:
+        dep = root
+
     # target init
     if config.mama_init and config.target:
-        dep = find_dependency(root, config.target)
         if not dep:
             console(f'init command failed: target {config.target} not found')
             exit(-1)
         mama_init_project(dep)
         return
 
     flat_deps = get_flat_deps(root) # root, dep2, deepest_dep
     flat_deps_reverse = list(reversed(flat_deps)) # deepest_dep, dep2, root
 
     if config.list:
         flat_deps_names = [d.name for d in flat_deps]
         if config.targets_all() or config.target == None:
             console(f'    ALL Dependency List: {flat_deps_names}', Color.BLUE)
-            for dep in flat_deps:
-                print_package_exports(dep)
+            for d in flat_deps: print_package_exports(d)
         else:
-            dep = find_dependency(root, config.target)
             console(f'    {dep.name} Dependency List: {flat_deps_names}', Color.BLUE)
             print_package_exports(dep)
         return
 
     if config.dirty:
-        dep = find_dependency(root, config.target)
         if not dep:
             console(f'dirty command failed: target {config.target} not found')
             exit(-1)
         mama_dirty(root, dep)
         return
 
     # initialize platform compiler config
@@ -254,14 +273,26 @@
     if config.verbose:
         chain = ' -> '.join([d.name for d in flat_deps_reverse])
         console(f'Executing task chain for build:\n    {chain}', Color.BLUE)
         print_package_exports(root)
 
     execute_task_chain(flat_deps_reverse)
 
+    if config.coverage_report:
+        if not dep:
+            console(f'coverage-report failed: target {config.target} not found')
+            exit(-1)
+        run_coverage_report(dep.target)
+        return
+
+    if dep and config.test and dep.get_enabled_coverage():
+        console('Project was built with coverage, generating coverage report')
+        run_coverage_report(dep.target)
+        return
+
     if config.open:
         open_project(config, root)
 
 
 def __main__():
     main()
```

### Comparing `mama-0.9.8/mama/msbuild.py` & `mama-0.9.9/mama/msbuild.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/package.py` & `mama-0.9.9/mama/package.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/papa_deploy.py` & `mama-0.9.9/mama/papa_deploy.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/papa_upload.py` & `mama-0.9.9/mama/papa_upload.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/parse_mamafile.py` & `mama-0.9.9/mama/parse_mamafile.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/platforms/android.py` & `mama-0.9.9/mama/platforms/android.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/platforms/mips.py` & `mama-0.9.9/mama/platforms/mips.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/platforms/oclea.py` & `mama-0.9.9/mama/platforms/oclea.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/types/artifactory_pkg.py` & `mama-0.9.9/mama/types/artifactory_pkg.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/types/asset.py` & `mama-0.9.9/mama/types/asset.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/types/dep_source.py` & `mama-0.9.9/mama/types/dep_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/types/git.py` & `mama-0.9.9/mama/types/git.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/types/local_source.py` & `mama-0.9.9/mama/types/local_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/util.py` & `mama-0.9.9/mama/util.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/utils/gdb.py` & `mama-0.9.9/mama/utils/gdb.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 from __future__ import annotations
 from typing import Tuple, TYPE_CHECKING
-import os, shlex
-from .system import System, console
+import os
+from .system import console, Color
 from .run import get_cwd_exe_args
 from .sub_process import execute_echo
 
 if TYPE_CHECKING:
     from ..build_target import BuildTarget
 
 
 def filter_gdb_arg(args: str, default_gdb=False) -> Tuple[str, bool]:
     if 'nogdb' == args: return '', False
     if 'nogdb ' in args: return args.replace('nogdb ', ''), False
     if 'gdb' == args: return '', True
     if 'gdb ' in args: return args.replace('gdb ', ''), True
     return args, default_gdb
 
+def _is_running_leak_sanitizer(target: BuildTarget):
+    if target.config.sanitize:
+        sanitizers = target.config.sanitize
+    else:
+        sanitizers = target.dep.get_enabled_sanitizers()
+    return ('leak' in sanitizers) or ('address' in sanitizers)
+
 
 def run_gdb(target: BuildTarget, command: str, src_dir=True):
     if target.android or target.ios or target.raspi or target.oclea or target.mips:
         console('Cannot run tests for Android, iOS, Raspi, Oclea, MIPS builds.')
         return # nothing to run
 
     root_dir = target.source_dir() if src_dir else target.build_dir()
     if target.windows and not src_dir:
         root_dir = f'{root_dir}/{target.cmake_build_type}'
 
     cwd, exe, args = get_cwd_exe_args(target, command, root_dir=root_dir)
 
     if target.windows:
         debugger = f'{exe} {args}'
+    elif _is_running_leak_sanitizer(target):
+        console('LEAK/ADDRESS sanitizer was enabled - GDB would disable LEAK detection, running without GDB', color=Color.YELLOW)
+        debugger = f'{exe} {args}'
     elif target.macos:
         # b: batch, q: quiet, -o r: run
         # -k bt: on crash, backtrace
         # -k q: on crash, quit 
         debugger = f'lldb -b -o r -k bt -k q  -- {exe} {args}'
     else: # linux
         # r: run;  bt: give backtrace;  q: quit when done;
```

### Comparing `mama-0.9.8/mama/utils/gnu_project.py` & `mama-0.9.9/mama/utils/gnu_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/utils/gtest.py` & `mama-0.9.9/mama/utils/gtest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 import os
+from .system import console
 from .gdb import filter_gdb_arg, run_gdb
 from .run import run_in_working_dir
 
 if TYPE_CHECKING:
     from ..build_target import BuildTarget
 
 def run_gtest(target: BuildTarget, executable: str, args='', src_dir=False, gdb=False):
```

### Comparing `mama-0.9.8/mama/utils/nonblocking_io.py` & `mama-0.9.9/mama/utils/nonblocking_io.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/utils/run.py` & `mama-0.9.9/mama/utils/run.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/utils/sub_process.py` & `mama-0.9.9/mama/utils/sub_process.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama/utils/system.py` & `mama-0.9.9/mama/utils/system.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/mama.egg-info/PKG-INFO` & `mama-0.9.9/mama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.9.8
+Version: 0.9.9
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.9.8/mama.egg-info/SOURCES.txt` & `mama-0.9.9/mama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mama-0.9.8/pyproject.toml` & `mama-0.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mama"
-version = "0.9.8"
+version = "0.9.9"
 description = "A modular C++ build tool even your mama can use"
 license = { text = "MIT" }
 authors = [
     { name="Jorma Rebane", email="jorma.rebane@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
```

