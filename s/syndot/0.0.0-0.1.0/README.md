# Comparing `tmp/syndot-0.0.0.tar.gz` & `tmp/syndot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syndot-0.0.0.tar", last modified: Tue Apr 16 22:27:13 2024, max compression
+gzip compressed data, was "syndot-0.1.0.tar", last modified: Sun Jun  2 18:08:48 2024, max compression
```

## Comparing `syndot-0.0.0.tar` & `syndot-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,67 @@
-drwxr-xr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-16 22:27:13.556718 syndot-0.0.0/
--rw-r--r--   0 andrea    (1000) andrea    (1000)      685 2024-04-16 22:27:13.556718 syndot-0.0.0/PKG-INFO
--rw-r--r--   0 andrea    (1000) andrea    (1000)       20 2024-04-16 22:24:23.000000 syndot-0.0.0/README.md
--rw-r--r--   0 andrea    (1000) andrea    (1000)      742 2024-04-16 22:27:02.000000 syndot-0.0.0/pyproject.toml
--rw-r--r--   0 andrea    (1000) andrea    (1000)       38 2024-04-16 22:27:13.556718 syndot-0.0.0/setup.cfg
--rw-r--r--   0 andrea    (1000) andrea    (1000)       57 2024-04-16 22:27:02.000000 syndot-0.0.0/setup.py
-drwxr-xr-x   0 andrea    (1000) andrea    (1000)        0 2024-04-16 22:27:13.555718 syndot-0.0.0/syndot.egg-info/
--rw-r--r--   0 andrea    (1000) andrea    (1000)      685 2024-04-16 22:27:13.000000 syndot-0.0.0/syndot.egg-info/PKG-INFO
--rw-r--r--   0 andrea    (1000) andrea    (1000)      153 2024-04-16 22:27:13.000000 syndot-0.0.0/syndot.egg-info/SOURCES.txt
--rw-r--r--   0 andrea    (1000) andrea    (1000)        1 2024-04-16 22:27:13.000000 syndot-0.0.0/syndot.egg-info/dependency_links.txt
--rw-r--r--   0 andrea    (1000) andrea    (1000)        7 2024-04-16 22:27:13.000000 syndot-0.0.0/syndot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.289924 syndot-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-02 18:08:26.000000 syndot-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41886 2024-06-02 18:08:48.289924 syndot-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-06-02 18:08:26.000000 syndot-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-06-02 18:08:26.000000 syndot-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 18:08:48.289924 syndot-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-02 18:08:26.000000 syndot-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.281924 syndot-0.1.0/syndot/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.281924 syndot-0.1.0/syndot/_colorschemes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/BlackOnLightYellow.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/BlackOnRandomLight.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/BlackOnWhite.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/BlueOnBlack.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/Breeze.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/DarkPastels.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/GreenOnBlack.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/Linux.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/RedOnBlack.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/Solarized.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/SolarizedLight.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/Sweet.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/Sweetified.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/WhiteOnBlack.colorscheme
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_colorschemes/default.colorscheme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.281924 syndot-0.1.0/syndot/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/_templates/map.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.285924 syndot-0.1.0/syndot/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/diffuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/list_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/commands/unlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/init_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.285924 syndot-0.1.0/syndot/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/add_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/diffuse_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/init_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/link_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/list_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/remove_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/parser/unlink_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.289924 syndot-0.1.0/syndot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/file_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/print_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 18:08:26.000000 syndot-0.1.0/syndot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.289924 syndot-0.1.0/syndot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41886 2024-06-02 18:08:48.000000 syndot-0.1.0/syndot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-06-02 18:08:48.000000 syndot-0.1.0/syndot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 18:08:48.000000 syndot-0.1.0/syndot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-02 18:08:48.000000 syndot-0.1.0/syndot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-02 18:08:48.000000 syndot-0.1.0/syndot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 18:08:48.289924 syndot-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-06-02 18:08:26.000000 syndot-0.1.0/tests/test_init_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-06-02 18:08:26.000000 syndot-0.1.0/tests/test_parser.py
```

