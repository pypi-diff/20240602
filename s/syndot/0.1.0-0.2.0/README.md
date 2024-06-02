# Comparing `tmp/syndot-0.1.0.tar.gz` & `tmp/syndot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syndot-0.1.0.tar", last modified: Sun Jun  2 18:08:48 2024, max compression
+gzip compressed data, was "syndot-0.2.0.tar", last modified: Sun Jun  2 19:16:32 2024, max compression
```

## Comparing `syndot-0.1.0.tar` & `syndot-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.289924 syndot-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-02 18:08:26.000000 syndot-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    41886 2024-06-02 18:08:48.289924 syndot-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-06-02 18:08:26.000000 syndot-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-06-02 18:08:26.000000 syndot-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:08:48.289924 syndot-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-02 18:08:26.000000 syndot-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.281924 syndot-0.1.0/syndot/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.281924 syndot-0.1.0/syndot/_colorschemes/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/BlackOnLightYellow.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/BlackOnRandomLight.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/BlackOnWhite.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/BlueOnBlack.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/Breeze.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/DarkPastels.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/GreenOnBlack.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/Linux.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/RedOnBlack.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/Solarized.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/SolarizedLight.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/Sweet.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/Sweetified.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/WhiteOnBlack.colorscheme
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/default.colorscheme
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.281924 syndot-0.1.0/syndot/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_templates/map.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.285924 syndot-0.1.0/syndot/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/diffuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/list_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/unlink.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/init_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.285924 syndot-0.1.0/syndot/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/add_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/diffuse_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/init_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/link_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/list_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/remove_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/unlink_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.289924 syndot-0.1.0/syndot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/file_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/map_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/print_.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.289924 syndot-0.1.0/syndot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41886 2024-06-02 18:08:48.000000 syndot-0.1.0/syndot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-06-02 18:08:48.000000 syndot-0.1.0/syndot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:08:48.000000 syndot-0.1.0/syndot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-02 18:08:48.000000 syndot-0.1.0/syndot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-02 18:08:48.000000 syndot-0.1.0/syndot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.289924 syndot-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-06-02 18:08:26.000000 syndot-0.1.0/tests/test_init_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-06-02 18:08:26.000000 syndot-0.1.0/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:16:32.857737 syndot-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-02 19:16:15.000000 syndot-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46025 2024-06-02 19:16:32.857737 syndot-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-06-02 19:16:15.000000 syndot-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-06-02 19:16:15.000000 syndot-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 19:16:32.857737 syndot-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-02 19:16:15.000000 syndot-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:16:32.849737 syndot-0.2.0/syndot/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:16:32.849737 syndot-0.2.0/syndot/_colorschemes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/BlackOnLightYellow.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/BlackOnRandomLight.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/BlackOnWhite.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/BlueOnBlack.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/Breeze.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/DarkPastels.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/GreenOnBlack.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/Linux.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/RedOnBlack.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/Solarized.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/SolarizedLight.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/Sweet.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/Sweetified.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/WhiteOnBlack.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_colorschemes/default.colorscheme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:16:32.849737 syndot-0.2.0/syndot/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/_templates/map.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:16:32.853737 syndot-0.2.0/syndot/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/commands/diffuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/commands/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/commands/list_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/commands/unlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/init_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:16:32.853737 syndot-0.2.0/syndot/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/parser/add_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/parser/diffuse_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/parser/init_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/parser/link_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/parser/list_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/parser/remove_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/parser/unlink_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:16:32.853737 syndot-0.2.0/syndot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/utils/file_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/utils/map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/utils/print_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 19:16:15.000000 syndot-0.2.0/syndot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:16:32.857737 syndot-0.2.0/syndot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46025 2024-06-02 19:16:32.000000 syndot-0.2.0/syndot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-06-02 19:16:32.000000 syndot-0.2.0/syndot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 19:16:32.000000 syndot-0.2.0/syndot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-02 19:16:32.000000 syndot-0.2.0/syndot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-02 19:16:32.000000 syndot-0.2.0/syndot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 19:16:32.857737 syndot-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-06-02 19:16:15.000000 syndot-0.2.0/tests/test_init_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-06-02 19:16:15.000000 syndot-0.2.0/tests/test_parser.py
```

### Comparing `syndot-0.1.0/LICENSE` & `syndot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/PKG-INFO` & `syndot-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syndot
-Version: 0.1.0
+Version: 0.2.0
 Summary: Dotfiles link management tool
 Author-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 Maintainer-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -679,27 +679,124 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/AndreaBlengino/syndot
 Project-URL: Documentation, https://syndot.readthedocs.io/en/latest/index.html
 Project-URL: Issues, https://github.com/AndreaBlengino/syndot/issues
 Project-URL: Repository, https://github.com/AndreaBlengino/syndot
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Desktop Environment :: File Managers
 Requires-Python: >=3.11
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: doc
 Requires-Dist: furo==2024.5.6; extra == "doc"
 Requires-Dist: sphinx==7.2.6; extra == "doc"
 Provides-Extra: test
 Requires-Dist: coverage==7.3.2; extra == "test"
 Requires-Dist: hypothesis==6.88.1; extra == "test"
 Requires-Dist: pytest==7.4.3; extra == "test"
 Requires-Dist: pytest-cov==4.1.0; extra == "test"
+
+Dotfiles Management
+-------------------
+
+**syndot** is a python library for Linux and macOS dotfiles management.
+
+.. list-table::
+   :stub-columns: 1
+   :widths: auto
+   :width: 100%
+
+   * - Release
+     - |pypi_release| |build|
+   * - Versioning
+     - |supported_python_versions| |semver|
+   * - Tests
+     - |linux_tests| |macos_tests| |test_coverage|
+   * - Documentation
+     - |docs|
+   * - Code Quality
+     - |codefactor_grade| |codacy_grade| |issues|
+   * - License
+     - |license|
+
+.. |pypi_release| image:: https://img.shields.io/pypi/v/syndot?label=release&color=blue
+   :target: https://pypi.org/project/syndot/
+   :alt: PyPI - Library Version
+
+.. |build| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/syndot/release.yml.svg?logo=github
+   :target: https://github.com/AndreaBlengino/syndot/actions/workflows/release.yml
+   :alt: Package Build
+
+.. |supported_python_versions| image:: https://img.shields.io/pypi/pyversions/syndot?logo=python&logoColor=gold
+   :target: https://pypi.org/project/syndot/
+   :alt: PyPI - Supported Python Versions
+
+.. |semver| image:: https://img.shields.io/badge/semver-2.0.0-blue.svg
+   :target: https://semver.org/
+
+.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/syndot/linux_test.yml.svg?logo=linux&logoColor=white&label=Linux
+   :target: https://github.com/AndreaBlengino/syndot/actions/workflows/linux_test.yml
+   :alt: Linux Tests
+
+.. |macos_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/syndot/macos_test.yml.svg?logo=apple&label=macOS
+   :target: https://github.com/AndreaBlengino/syndot/actions/workflows/macos_test.yml
+   :alt: macOS Tests
+
+.. |test_coverage| image:: https://img.shields.io/codecov/c/github/AndreaBlengino/syndot/master?logo=codecov
+   :target: https://codecov.io/gh/AndreaBlengino/syndot
+   :alt: Test Coverage
+
+.. |docs| image:: https://img.shields.io/readthedocs/syndot/latest?logo=read%20the%20docs
+   :target: https://syndot.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Build Status
+
+.. |codefactor_grade| image:: https://img.shields.io/codefactor/grade/github/AndreaBlengino/syndot?logo=codefactor&label=CodeFactor
+   :target: https://www.codefactor.io/repository/github/andreablengino/syndot
+   :alt: CodeFactor Grade
+
+.. |codacy_grade| image:: https://img.shields.io/codacy/grade/132c2f3d93344ae0934ea808bbf17f05?logo=codacy&label=Codacy
+   :target: https://app.codacy.com/gh/AndreaBlengino/syndot/dashboard
+   :alt: Codacy Grade
+
+.. |issues| image:: https://img.shields.io/github/issues/AndreaBlengino/syndot?logo=github
+   :target: https://github.com/AndreaBlengino/syndot/issues
+   :alt: Open Issues
+
+.. |license| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
+   :target: https://github.com/AndreaBlengino/syndot/blob/master/LICENSE
+   :alt: License
+
+
+References
+----------
+
+- `Installation <https://syndot.readthedocs.io/en/latest/get_started.html>`_
+- `PyPI <https://pypi.org/project/syndot/>`_
+- `Documentation <https://syndot.readthedocs.io/en/latest/?badge=latest>`_
+- `Issue tracker <https://github.com/AndreaBlengino/syndot/issues>`_
+- `Source code <https://github.com/AndreaBlengino/syndot/tree/master/syndot>`_
+- `GNU General Public License v3.0 <https://github.com/AndreaBlengino/syndot/blob/master/LICENSE>`_
+
+
+Contributing
+------------
+
+The syndot project welcomes your expertise and enthusiasm!
+All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.
+Writing code isn't the only way to contribute to syndot. You can also:
+
+- develop tutorials, presentations and other educational materials,
+- maintain and improve the `documentation <https://syndot.readthedocs.io/en/latest/?badge=latest>`_,
+- help with outreach and onboard new contributors.
+
+Have a look at the `contributing guide <https://github.com/AndreaBlengino/syndot/blob/master/.github/CONTRIBUTING.md>`_.
+If you are new to contributing to open source, `this guide <https://opensource.guide/how-to-contribute/>`_ helps explain
+why, what, and how to successfully get involved.
```

### Comparing `syndot-0.1.0/README.rst` & `syndot-0.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 .. list-table::
    :stub-columns: 1
    :widths: auto
    :width: 100%
 
    * - Release
-     - |pypi_release|
+     - |pypi_release| |build|
    * - Versioning
      - |supported_python_versions| |semver|
    * - Tests
      - |linux_tests| |macos_tests| |test_coverage|
    * - Documentation
      - |docs|
    * - Code Quality
@@ -21,14 +21,18 @@
    * - License
      - |license|
 
 .. |pypi_release| image:: https://img.shields.io/pypi/v/syndot?label=release&color=blue
    :target: https://pypi.org/project/syndot/
    :alt: PyPI - Library Version
 
+.. |build| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/syndot/release.yml.svg?logo=github
+   :target: https://github.com/AndreaBlengino/syndot/actions/workflows/release.yml
+   :alt: Package Build
+
 .. |supported_python_versions| image:: https://img.shields.io/pypi/pyversions/syndot?logo=python&logoColor=gold
    :target: https://pypi.org/project/syndot/
    :alt: PyPI - Supported Python Versions
 
 .. |semver| image:: https://img.shields.io/badge/semver-2.0.0-blue.svg
    :target: https://semver.org/
```

### Comparing `syndot-0.1.0/pyproject.toml` & `syndot-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 authors = [
   {name = "Andrea Blengino", email = "ing.andrea.blengino@protonmail.com"},
 ]
 maintainers = [
   {name = "Andrea Blengino", email = "ing.andrea.blengino@protonmail.com"},
 ]
 description = "Dotfiles link management tool"
-readme = "README.md"
+readme = "README.rst"
 license = { file = "LICENSE" }
 classifiers = [
-  "Development Status :: 4 - Beta",
+  "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: End Users/Desktop",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
```

### Comparing `syndot-0.1.0/syndot/_colorschemes/BlackOnLightYellow.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/BlackOnLightYellow.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/BlackOnRandomLight.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/BlackOnRandomLight.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/BlackOnWhite.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/BlackOnWhite.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/BlueOnBlack.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/BlueOnBlack.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/Breeze.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/Breeze.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/DarkPastels.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/DarkPastels.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/GreenOnBlack.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/GreenOnBlack.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/Linux.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/Linux.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/RedOnBlack.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/RedOnBlack.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/Solarized.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/Solarized.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/SolarizedLight.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/SolarizedLight.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/Sweet.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/Sweet.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/Sweetified.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/Sweetified.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/WhiteOnBlack.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/WhiteOnBlack.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/_colorschemes/default.colorscheme` & `syndot-0.2.0/syndot/_colorschemes/default.colorscheme`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/commands/add.py` & `syndot-0.2.0/syndot/commands/add.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/commands/diffuse.py` & `syndot-0.2.0/syndot/commands/diffuse.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/commands/init.py` & `syndot-0.2.0/syndot/commands/init.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/commands/link.py` & `syndot-0.2.0/syndot/commands/link.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/commands/list_.py` & `syndot-0.2.0/syndot/commands/list_.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/commands/remove.py` & `syndot-0.2.0/syndot/commands/remove.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/commands/unlink.py` & `syndot-0.2.0/syndot/commands/unlink.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/init_config.py` & `syndot-0.2.0/syndot/init_config.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/parser/add_parser.py` & `syndot-0.2.0/syndot/parser/add_parser.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/parser/diffuse_parser.py` & `syndot-0.2.0/syndot/parser/diffuse_parser.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/parser/init_parser.py` & `syndot-0.2.0/syndot/parser/init_parser.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/parser/link_parser.py` & `syndot-0.2.0/syndot/parser/link_parser.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/parser/list_parser.py` & `syndot-0.2.0/syndot/parser/list_parser.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/parser/parser.py` & `syndot-0.2.0/syndot/parser/parser.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/parser/remove_parser.py` & `syndot-0.2.0/syndot/parser/remove_parser.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/parser/unlink_parser.py` & `syndot-0.2.0/syndot/parser/unlink_parser.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/utils/colors.py` & `syndot-0.2.0/syndot/utils/colors.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/utils/commands.py` & `syndot-0.2.0/syndot/utils/commands.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/utils/file_actions.py` & `syndot-0.2.0/syndot/utils/file_actions.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/utils/map_file.py` & `syndot-0.2.0/syndot/utils/map_file.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/utils/path.py` & `syndot-0.2.0/syndot/utils/path.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot/utils/print_.py` & `syndot-0.2.0/syndot/utils/print_.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/syndot.egg-info/PKG-INFO` & `syndot-0.2.0/syndot.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syndot
-Version: 0.1.0
+Version: 0.2.0
 Summary: Dotfiles link management tool
 Author-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 Maintainer-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -679,27 +679,124 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/AndreaBlengino/syndot
 Project-URL: Documentation, https://syndot.readthedocs.io/en/latest/index.html
 Project-URL: Issues, https://github.com/AndreaBlengino/syndot/issues
 Project-URL: Repository, https://github.com/AndreaBlengino/syndot
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Desktop Environment :: File Managers
 Requires-Python: >=3.11
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: doc
 Requires-Dist: furo==2024.5.6; extra == "doc"
 Requires-Dist: sphinx==7.2.6; extra == "doc"
 Provides-Extra: test
 Requires-Dist: coverage==7.3.2; extra == "test"
 Requires-Dist: hypothesis==6.88.1; extra == "test"
 Requires-Dist: pytest==7.4.3; extra == "test"
 Requires-Dist: pytest-cov==4.1.0; extra == "test"
+
+Dotfiles Management
+-------------------
+
+**syndot** is a python library for Linux and macOS dotfiles management.
+
+.. list-table::
+   :stub-columns: 1
+   :widths: auto
+   :width: 100%
+
+   * - Release
+     - |pypi_release| |build|
+   * - Versioning
+     - |supported_python_versions| |semver|
+   * - Tests
+     - |linux_tests| |macos_tests| |test_coverage|
+   * - Documentation
+     - |docs|
+   * - Code Quality
+     - |codefactor_grade| |codacy_grade| |issues|
+   * - License
+     - |license|
+
+.. |pypi_release| image:: https://img.shields.io/pypi/v/syndot?label=release&color=blue
+   :target: https://pypi.org/project/syndot/
+   :alt: PyPI - Library Version
+
+.. |build| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/syndot/release.yml.svg?logo=github
+   :target: https://github.com/AndreaBlengino/syndot/actions/workflows/release.yml
+   :alt: Package Build
+
+.. |supported_python_versions| image:: https://img.shields.io/pypi/pyversions/syndot?logo=python&logoColor=gold
+   :target: https://pypi.org/project/syndot/
+   :alt: PyPI - Supported Python Versions
+
+.. |semver| image:: https://img.shields.io/badge/semver-2.0.0-blue.svg
+   :target: https://semver.org/
+
+.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/syndot/linux_test.yml.svg?logo=linux&logoColor=white&label=Linux
+   :target: https://github.com/AndreaBlengino/syndot/actions/workflows/linux_test.yml
+   :alt: Linux Tests
+
+.. |macos_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/syndot/macos_test.yml.svg?logo=apple&label=macOS
+   :target: https://github.com/AndreaBlengino/syndot/actions/workflows/macos_test.yml
+   :alt: macOS Tests
+
+.. |test_coverage| image:: https://img.shields.io/codecov/c/github/AndreaBlengino/syndot/master?logo=codecov
+   :target: https://codecov.io/gh/AndreaBlengino/syndot
+   :alt: Test Coverage
+
+.. |docs| image:: https://img.shields.io/readthedocs/syndot/latest?logo=read%20the%20docs
+   :target: https://syndot.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Build Status
+
+.. |codefactor_grade| image:: https://img.shields.io/codefactor/grade/github/AndreaBlengino/syndot?logo=codefactor&label=CodeFactor
+   :target: https://www.codefactor.io/repository/github/andreablengino/syndot
+   :alt: CodeFactor Grade
+
+.. |codacy_grade| image:: https://img.shields.io/codacy/grade/132c2f3d93344ae0934ea808bbf17f05?logo=codacy&label=Codacy
+   :target: https://app.codacy.com/gh/AndreaBlengino/syndot/dashboard
+   :alt: Codacy Grade
+
+.. |issues| image:: https://img.shields.io/github/issues/AndreaBlengino/syndot?logo=github
+   :target: https://github.com/AndreaBlengino/syndot/issues
+   :alt: Open Issues
+
+.. |license| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
+   :target: https://github.com/AndreaBlengino/syndot/blob/master/LICENSE
+   :alt: License
+
+
+References
+----------
+
+- `Installation <https://syndot.readthedocs.io/en/latest/get_started.html>`_
+- `PyPI <https://pypi.org/project/syndot/>`_
+- `Documentation <https://syndot.readthedocs.io/en/latest/?badge=latest>`_
+- `Issue tracker <https://github.com/AndreaBlengino/syndot/issues>`_
+- `Source code <https://github.com/AndreaBlengino/syndot/tree/master/syndot>`_
+- `GNU General Public License v3.0 <https://github.com/AndreaBlengino/syndot/blob/master/LICENSE>`_
+
+
+Contributing
+------------
+
+The syndot project welcomes your expertise and enthusiasm!
+All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.
+Writing code isn't the only way to contribute to syndot. You can also:
+
+- develop tutorials, presentations and other educational materials,
+- maintain and improve the `documentation <https://syndot.readthedocs.io/en/latest/?badge=latest>`_,
+- help with outreach and onboard new contributors.
+
+Have a look at the `contributing guide <https://github.com/AndreaBlengino/syndot/blob/master/.github/CONTRIBUTING.md>`_.
+If you are new to contributing to open source, `this guide <https://opensource.guide/how-to-contribute/>`_ helps explain
+why, what, and how to successfully get involved.
```

### Comparing `syndot-0.1.0/syndot.egg-info/SOURCES.txt` & `syndot-0.2.0/syndot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/tests/test_init_config.py` & `syndot-0.2.0/tests/test_init_config.py`

 * *Files identical despite different names*

### Comparing `syndot-0.1.0/tests/test_parser.py` & `syndot-0.2.0/tests/test_parser.py`

 * *Files identical despite different names*

