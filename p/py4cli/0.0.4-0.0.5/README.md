# Comparing `tmp/py4cli-0.0.4.tar.gz` & `tmp/py4cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\py4cli-0.0.4.tar", last modified: Fri Apr 26 08:24:32 2024, max compression
+gzip compressed data, was "dist\py4cli-0.0.5.tar", last modified: Sun Jun  2 16:54:08 2024, max compression
```

## Comparing `py4cli-0.0.4.tar` & `py4cli-0.0.5.tar`

### file list

```diff
@@ -1,81 +1,104 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/
--rw-rw-rw-   0        0        0    35812 2024-03-31 05:57:29.000000 py4cli-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      101 2024-04-26 07:58:26.000000 py4cli-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5609 2024-04-26 08:24:32.000000 py4cli-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5074 2024-04-26 08:23:33.000000 py4cli-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/SRCS/
-drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/SRCS/py4cli/
--rw-rw-rw-   0        0        0     5854 2024-04-26 05:07:42.000000 py4cli-0.0.4/SRCS/py4cli/minimal.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/
--rw-rw-rw-   0        0        0     5609 2024-04-26 08:24:31.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1975 2024-04-26 08:24:32.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 08:24:31.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-26 08:24:31.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-26 08:24:31.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/TESTS/
--rw-rw-rw-   0        0        0      486 2024-04-23 12:35:47.000000 py4cli-0.0.4/TESTS/conftest.py
-drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/TESTS/ref_files/
--rw-rw-rw-   0        0        0       49 2024-04-26 06:47:42.000000 py4cli-0.0.4/TESTS/ref_files/bool.txt
--rw-rw-rw-   0        0        0       56 2024-04-26 06:47:42.000000 py4cli-0.0.4/TESTS/ref_files/bool_args.txt
--rw-rw-rw-   0        0        0      635 2024-04-26 07:42:00.000000 py4cli-0.0.4/TESTS/ref_files/bool_h.txt
--rw-rw-rw-   0        0        0      639 2024-04-26 07:42:00.000000 py4cli-0.0.4/TESTS/ref_files/bool_help.txt
--rw-rw-rw-   0        0        0       66 2024-04-26 06:47:42.000000 py4cli-0.0.4/TESTS/ref_files/bool_kwargs.txt
--rw-rw-rw-   0        0        0       56 2024-04-26 06:47:41.000000 py4cli-0.0.4/TESTS/ref_files/dict.txt
--rw-rw-rw-   0        0        0       83 2024-04-26 06:47:41.000000 py4cli-0.0.4/TESTS/ref_files/dict_args.txt
--rw-rw-rw-   0        0        0      675 2024-04-26 07:00:39.000000 py4cli-0.0.4/TESTS/ref_files/dict_h.txt
--rw-rw-rw-   0        0        0      679 2024-04-26 07:00:39.000000 py4cli-0.0.4/TESTS/ref_files/dict_help.txt
--rw-rw-rw-   0        0        0       93 2024-04-26 06:47:41.000000 py4cli-0.0.4/TESTS/ref_files/dict_kwargs.txt
--rw-rw-rw-   0        0        0       49 2024-04-26 06:47:35.000000 py4cli-0.0.4/TESTS/ref_files/float.txt
--rw-rw-rw-   0        0        0       58 2024-04-26 06:47:35.000000 py4cli-0.0.4/TESTS/ref_files/float_args.txt
--rw-rw-rw-   0        0        0      652 2024-04-26 06:47:34.000000 py4cli-0.0.4/TESTS/ref_files/float_h.txt
--rw-rw-rw-   0        0        0      656 2024-04-26 06:47:34.000000 py4cli-0.0.4/TESTS/ref_files/float_help.txt
--rw-rw-rw-   0        0        0       69 2024-04-26 06:47:35.000000 py4cli-0.0.4/TESTS/ref_files/float_kwargs.txt
--rw-rw-rw-   0        0        0       43 2024-04-26 06:47:34.000000 py4cli-0.0.4/TESTS/ref_files/int.txt
--rw-rw-rw-   0        0        0       50 2024-04-26 06:47:34.000000 py4cli-0.0.4/TESTS/ref_files/int_args.txt
--rw-rw-rw-   0        0        0      615 2024-04-26 06:47:33.000000 py4cli-0.0.4/TESTS/ref_files/int_h.txt
--rw-rw-rw-   0        0        0      619 2024-04-26 06:47:33.000000 py4cli-0.0.4/TESTS/ref_files/int_help.txt
--rw-rw-rw-   0        0        0       59 2024-04-26 06:47:34.000000 py4cli-0.0.4/TESTS/ref_files/int_kwargs.txt
--rw-rw-rw-   0        0        0       50 2024-04-26 06:47:37.000000 py4cli-0.0.4/TESTS/ref_files/list.txt
--rw-rw-rw-   0        0        0       64 2024-04-26 06:47:37.000000 py4cli-0.0.4/TESTS/ref_files/list_args.txt
--rw-rw-rw-   0        0        0      647 2024-04-26 06:47:37.000000 py4cli-0.0.4/TESTS/ref_files/list_h.txt
--rw-rw-rw-   0        0        0      651 2024-04-26 06:47:37.000000 py4cli-0.0.4/TESTS/ref_files/list_help.txt
--rw-rw-rw-   0        0        0       74 2024-04-26 06:47:37.000000 py4cli-0.0.4/TESTS/ref_files/list_kwargs.txt
--rw-rw-rw-   0        0        0      321 2024-04-26 06:47:43.000000 py4cli-0.0.4/TESTS/ref_files/multi.txt
--rw-rw-rw-   0        0        0      469 2024-04-26 06:52:41.000000 py4cli-0.0.4/TESTS/ref_files/multi_args.txt
--rw-rw-rw-   0        0        0     1254 2024-04-26 06:47:42.000000 py4cli-0.0.4/TESTS/ref_files/multi_h.txt
--rw-rw-rw-   0        0        0     1258 2024-04-26 06:47:43.000000 py4cli-0.0.4/TESTS/ref_files/multi_help.txt
--rw-rw-rw-   0        0        0      548 2024-04-26 06:52:41.000000 py4cli-0.0.4/TESTS/ref_files/multi_kwargs.txt
--rw-rw-rw-   0        0        0      348 2024-04-26 06:47:44.000000 py4cli-0.0.4/TESTS/ref_files/multi_mix1.txt
--rw-rw-rw-   0        0        0      403 2024-04-26 06:47:44.000000 py4cli-0.0.4/TESTS/ref_files/multi_mix2.txt
--rw-rw-rw-   0        0        0      404 2024-04-26 06:47:44.000000 py4cli-0.0.4/TESTS/ref_files/multi_mix3.txt
--rw-rw-rw-   0        0        0       48 2024-04-26 06:47:39.000000 py4cli-0.0.4/TESTS/ref_files/set.txt
--rw-rw-rw-   0        0        0       68 2024-04-26 06:47:40.000000 py4cli-0.0.4/TESTS/ref_files/set_args.txt
--rw-rw-rw-   0        0        0      635 2024-04-26 06:47:39.000000 py4cli-0.0.4/TESTS/ref_files/set_h.txt
--rw-rw-rw-   0        0        0      639 2024-04-26 06:47:39.000000 py4cli-0.0.4/TESTS/ref_files/set_help.txt
--rw-rw-rw-   0        0        0       77 2024-04-26 06:47:40.000000 py4cli-0.0.4/TESTS/ref_files/set_kwargs.txt
--rw-rw-rw-   0        0        0       46 2024-04-26 06:47:36.000000 py4cli-0.0.4/TESTS/ref_files/str.txt
--rw-rw-rw-   0        0        0       56 2024-04-26 06:47:36.000000 py4cli-0.0.4/TESTS/ref_files/str_args.txt
--rw-rw-rw-   0        0        0      630 2024-04-26 06:47:35.000000 py4cli-0.0.4/TESTS/ref_files/str_h.txt
--rw-rw-rw-   0        0        0      634 2024-04-26 06:47:36.000000 py4cli-0.0.4/TESTS/ref_files/str_help.txt
--rw-rw-rw-   0        0        0       65 2024-04-26 06:47:36.000000 py4cli-0.0.4/TESTS/ref_files/str_kwargs.txt
--rw-rw-rw-   0        0        0       53 2024-04-26 06:47:38.000000 py4cli-0.0.4/TESTS/ref_files/tuple.txt
--rw-rw-rw-   0        0        0       66 2024-04-26 06:47:38.000000 py4cli-0.0.4/TESTS/ref_files/tuple_args.txt
--rw-rw-rw-   0        0        0      663 2024-04-26 06:47:38.000000 py4cli-0.0.4/TESTS/ref_files/tuple_h.txt
--rw-rw-rw-   0        0        0      667 2024-04-26 06:47:38.000000 py4cli-0.0.4/TESTS/ref_files/tuple_help.txt
--rw-rw-rw-   0        0        0       77 2024-04-26 06:47:39.000000 py4cli-0.0.4/TESTS/ref_files/tuple_kwargs.txt
-drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/TESTS/scripts/
--rw-rw-rw-   0        0        0     5933 2024-04-26 07:36:42.000000 py4cli-0.0.4/TESTS/scripts/basic_usage.py
--rw-rw-rw-   0        0        0      372 2024-04-26 06:42:28.000000 py4cli-0.0.4/TESTS/scripts/multi_args.py
--rw-rw-rw-   0        0        0      139 2024-04-26 06:42:03.000000 py4cli-0.0.4/TESTS/scripts/use_bool.py
--rw-rw-rw-   0        0        0      141 2024-04-26 06:41:34.000000 py4cli-0.0.4/TESTS/scripts/use_dict.py
--rw-rw-rw-   0        0        0      143 2024-04-26 06:41:27.000000 py4cli-0.0.4/TESTS/scripts/use_float.py
--rw-rw-rw-   0        0        0      139 2024-04-26 06:41:16.000000 py4cli-0.0.4/TESTS/scripts/use_int.py
--rw-rw-rw-   0        0        0      141 2024-04-26 06:41:41.000000 py4cli-0.0.4/TESTS/scripts/use_list.py
--rw-rw-rw-   0        0        0      139 2024-04-26 06:41:46.000000 py4cli-0.0.4/TESTS/scripts/use_set.py
--rw-rw-rw-   0        0        0      139 2024-04-26 06:41:50.000000 py4cli-0.0.4/TESTS/scripts/use_str.py
--rw-rw-rw-   0        0        0      143 2024-04-26 06:41:58.000000 py4cli-0.0.4/TESTS/scripts/use_tuple.py
--rw-rw-rw-   0        0        0    10198 2024-04-26 06:47:28.000000 py4cli-0.0.4/TESTS/test_basic_call.py
--rw-rw-rw-   0        0        0     4211 2024-04-26 06:52:22.000000 py4cli-0.0.4/TESTS/test_basic_os.py
--rw-rw-rw-   0        0        0      144 2024-03-31 05:57:29.000000 py4cli-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 08:24:32.000000 py4cli-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      964 2024-04-26 07:57:37.000000 py4cli-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:54:08.000000 py4cli-0.0.5/
+-rw-rw-rw-   0        0        0    35812 2024-05-27 12:45:50.000000 py4cli-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      101 2024-05-27 12:45:50.000000 py4cli-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    13678 2024-06-02 16:54:08.000000 py4cli-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13143 2024-06-02 16:41:40.000000 py4cli-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 16:54:08.000000 py4cli-0.0.5/SRCS/
+drwxrwxrwx   0        0        0        0 2024-06-02 16:54:08.000000 py4cli-0.0.5/SRCS/py4cli/
+-rw-rw-rw-   0        0        0     7290 2024-06-02 15:26:30.000000 py4cli-0.0.5/SRCS/py4cli/minimal.py
+-rw-rw-rw-   0        0        0     8432 2024-06-02 15:27:44.000000 py4cli-0.0.5/SRCS/py4cli/moderate.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:54:08.000000 py4cli-0.0.5/SRCS/py4cli.egg-info/
+-rw-rw-rw-   0        0        0    13678 2024-06-02 16:54:08.000000 py4cli-0.0.5/SRCS/py4cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2886 2024-06-02 16:54:08.000000 py4cli-0.0.5/SRCS/py4cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 16:54:08.000000 py4cli-0.0.5/SRCS/py4cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-06-02 16:54:08.000000 py4cli-0.0.5/SRCS/py4cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-06-02 16:54:08.000000 py4cli-0.0.5/SRCS/py4cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 16:54:08.000000 py4cli-0.0.5/TESTS/
+-rw-rw-rw-   0        0        0      594 2024-05-28 12:15:13.000000 py4cli-0.0.5/TESTS/conftest.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:54:08.000000 py4cli-0.0.5/TESTS/minimal_scripts/
+-rw-rw-rw-   0        0        0     6635 2024-06-02 07:21:43.000000 py4cli-0.0.5/TESTS/minimal_scripts/basic_usage.py
+-rw-rw-rw-   0        0        0      296 2024-05-28 12:45:47.000000 py4cli-0.0.5/TESTS/minimal_scripts/multi_args.py
+-rw-rw-rw-   0        0        0      139 2024-05-27 12:45:50.000000 py4cli-0.0.5/TESTS/minimal_scripts/use_bool.py
+-rw-rw-rw-   0        0        0      141 2024-05-27 12:45:50.000000 py4cli-0.0.5/TESTS/minimal_scripts/use_dict.py
+-rw-rw-rw-   0        0        0      143 2024-05-27 12:45:50.000000 py4cli-0.0.5/TESTS/minimal_scripts/use_float.py
+-rw-rw-rw-   0        0        0      139 2024-05-27 12:45:50.000000 py4cli-0.0.5/TESTS/minimal_scripts/use_int.py
+-rw-rw-rw-   0        0        0      141 2024-05-27 12:45:50.000000 py4cli-0.0.5/TESTS/minimal_scripts/use_list.py
+-rw-rw-rw-   0        0        0      139 2024-05-27 12:45:50.000000 py4cli-0.0.5/TESTS/minimal_scripts/use_str.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:54:08.000000 py4cli-0.0.5/TESTS/moderate_scripts/
+-rw-rw-rw-   0        0        0     6775 2024-06-02 07:22:58.000000 py4cli-0.0.5/TESTS/moderate_scripts/basic_usage.py
+drwxrwxrwx   0        0        0        0 2024-06-02 16:54:08.000000 py4cli-0.0.5/TESTS/ref_files/
+-rw-rw-rw-   0        0        0       57 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_bool.txt
+-rw-rw-rw-   0        0        0       64 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_bool_args.txt
+-rw-rw-rw-   0        0        0      659 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_bool_h.txt
+-rw-rw-rw-   0        0        0      663 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_bool_help.txt
+-rw-rw-rw-   0        0        0       74 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_bool_kwargs.txt
+-rw-rw-rw-   0        0        0       64 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_dict.txt
+-rw-rw-rw-   0        0        0       91 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_dict_args.txt
+-rw-rw-rw-   0        0        0      699 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_dict_h.txt
+-rw-rw-rw-   0        0        0      703 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_dict_help.txt
+-rw-rw-rw-   0        0        0      101 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_dict_kwargs.txt
+-rw-rw-rw-   0        0        0       57 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_float.txt
+-rw-rw-rw-   0        0        0       66 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_float_args.txt
+-rw-rw-rw-   0        0        0      676 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_float_h.txt
+-rw-rw-rw-   0        0        0      680 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_float_help.txt
+-rw-rw-rw-   0        0        0       77 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_float_kwargs.txt
+-rw-rw-rw-   0        0        0       51 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_int.txt
+-rw-rw-rw-   0        0        0       58 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_int_args.txt
+-rw-rw-rw-   0        0        0      639 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_int_h.txt
+-rw-rw-rw-   0        0        0      643 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_int_help.txt
+-rw-rw-rw-   0        0        0       67 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_int_kwargs.txt
+-rw-rw-rw-   0        0        0       58 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_list.txt
+-rw-rw-rw-   0        0        0       72 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_list_args.txt
+-rw-rw-rw-   0        0        0      671 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_list_h.txt
+-rw-rw-rw-   0        0        0      675 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_list_help.txt
+-rw-rw-rw-   0        0        0       82 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_list_kwargs.txt
+-rw-rw-rw-   0        0        0      265 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_multi.txt
+-rw-rw-rw-   0        0        0      369 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_multi_args.txt
+-rw-rw-rw-   0        0        0     1105 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_multi_h.txt
+-rw-rw-rw-   0        0        0     1109 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_multi_help.txt
+-rw-rw-rw-   0        0        0      428 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_multi_kwargs.txt
+-rw-rw-rw-   0        0        0      292 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_multi_mix1.txt
+-rw-rw-rw-   0        0        0      347 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_multi_mix2.txt
+-rw-rw-rw-   0        0        0      320 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_multi_mix3.txt
+-rw-rw-rw-   0        0        0       54 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_str.txt
+-rw-rw-rw-   0        0        0       64 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_str_args.txt
+-rw-rw-rw-   0        0        0      654 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_str_h.txt
+-rw-rw-rw-   0        0        0      658 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_str_help.txt
+-rw-rw-rw-   0        0        0       73 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/min_str_kwargs.txt
+-rw-rw-rw-   0        0        0      348 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod.txt
+-rw-rw-rw-   0        0        0      100 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_bool.txt
+-rw-rw-rw-   0        0        0      107 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_bool_args.txt
+-rw-rw-rw-   0        0        0      117 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_bool_kwargs.txt
+-rw-rw-rw-   0        0        0      119 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_dict.txt
+-rw-rw-rw-   0        0        0      144 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_dict_args.txt
+-rw-rw-rw-   0        0        0      154 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_dict_kwargs.txt
+-rw-rw-rw-   0        0        0      100 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_float.txt
+-rw-rw-rw-   0        0        0      109 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_float_args.txt
+-rw-rw-rw-   0        0        0      120 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_float_kwargs.txt
+-rw-rw-rw-   0        0        0     7184 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_h.txt
+-rw-rw-rw-   0        0        0     7188 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_help.txt
+-rw-rw-rw-   0        0        0       94 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_int.txt
+-rw-rw-rw-   0        0        0      101 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_int_args.txt
+-rw-rw-rw-   0        0        0      110 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_int_kwargs.txt
+-rw-rw-rw-   0        0        0      111 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_list.txt
+-rw-rw-rw-   0        0        0      135 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_list_args.txt
+-rw-rw-rw-   0        0        0      145 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_list_kwargs.txt
+-rw-rw-rw-   0        0        0      334 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_multi.txt
+-rw-rw-rw-   0        0        0      438 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_multi_args.txt
+-rw-rw-rw-   0        0        0      497 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_multi_kwargs.txt
+-rw-rw-rw-   0        0        0      361 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_multi_mix1.txt
+-rw-rw-rw-   0        0        0      416 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_multi_mix2.txt
+-rw-rw-rw-   0        0        0      389 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_multi_mix3.txt
+-rw-rw-rw-   0        0        0       99 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_str.txt
+-rw-rw-rw-   0        0        0      109 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_str_args.txt
+-rw-rw-rw-   0        0        0      118 2024-06-02 16:45:30.000000 py4cli-0.0.5/TESTS/ref_files/mod_str_kwargs.txt
+-rw-rw-rw-   0        0        0     8010 2024-05-29 12:32:15.000000 py4cli-0.0.5/TESTS/test_min_call.py
+-rw-rw-rw-   0        0        0     4268 2024-06-02 04:57:21.000000 py4cli-0.0.5/TESTS/test_min_os.py
+-rw-rw-rw-   0        0        0     2762 2024-06-02 07:26:51.000000 py4cli-0.0.5/TESTS/test_min_warn.py
+-rw-rw-rw-   0        0        0     2660 2024-06-02 08:03:25.000000 py4cli-0.0.5/TESTS/test_mod_call.py
+-rw-rw-rw-   0        0        0     3964 2024-06-02 08:02:56.000000 py4cli-0.0.5/TESTS/test_mod_os.py
+-rw-rw-rw-   0        0        0     2357 2024-06-02 07:28:40.000000 py4cli-0.0.5/TESTS/test_mod_warn.py
+-rw-rw-rw-   0        0        0       36 2024-05-27 13:59:00.000000 py4cli-0.0.5/rel_reqs.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 16:54:08.000000 py4cli-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-06-02 16:53:54.000000 py4cli-0.0.5/setup.py
+-rw-rw-rw-   0        0        0      114 2024-06-02 04:57:51.000000 py4cli-0.0.5/test_reqs.txt
```

### Comparing `py4cli-0.0.4/LICENSE.txt` & `py4cli-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py4cli-0.0.4/SRCS/py4cli/minimal.py` & `py4cli-0.0.5/SRCS/py4cli/minimal.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,110 +5,132 @@
 import ast
 import __main__
 
 class arg_parser():
 
     def __init__(self, argv=sys.argv):
 
+        methods = []
+        self.returned = None
+        for name, obj in inspect.getmembers(self, predicate=inspect.ismethod):
+            if not name.startswith('_'):
+                methods.append(name)
+        methods = sorted(methods)
+
         def_func_name = 'parse_args'
-        if len(argv) == 2 and (argv[1] in ['-h', '--help']):
-            self.returned = None
-            self.__doc(def_func_name)
-        else:
-            func_schema = self.__func2schema(def_func_name)
-            args_schema = self.__args2schema(def_func_name, argv[1:])
-            args, kwargs = self.__solve_schema(
-                func_schema[def_func_name], args_schema[def_func_name])
-            if inspect.ismethod(getattr(self, def_func_name)):
+        if def_func_name in methods:
+            if len(argv) == 2 and (argv[1] in ['-h', '--help']):
+                self.returned = None
+                self.__doc(def_func_name)
+            else:
+                func_schema = self.__func2schema(def_func_name)
+                args_schema = self.__args2schema(def_func_name, argv[1:])
+                args, kwargs = self.__solve_schema(func_schema[def_func_name], args_schema[def_func_name])
                 self.returned = self.__func(def_func_name, args, kwargs)
-                if type(self.returned) != func_schema['ret_type']:
+                if func_schema['ret_type'] != inspect._empty and type(self.returned) != func_schema['ret_type']:
                     print(
-                        f"WARNING : '{def_func_name}' returns '{type(self.returned).__name__}', but defined to return '{func_schema['ret_type'].__name__}'")
+                        f"WARNING : '{def_func_name}' returns '{type(self.returned)}', but defined to return '{func_schema['ret_type']}'")
+        else:
+            raise Exception(f"func name : '{def_func_name}' is not defined")
 
     def __func(self, func, args, kwargs):
 
         returned = getattr(self, func)(*args, **kwargs)
         return returned
 
-    def __type(self, dtype, value):
+    def __type(self, var_name, dtype, value):
+
+        if dtype in [str, int, float, list, dict, bool, inspect._empty]:
+            casted, casted_value = self.__validate_and_typecast(dtype, value)
+            if casted:
+                type_casted_value = casted_value
+            else:
+                raise ValueError(f"Expected '{dtype}' value for '{var_name}' in kwargs of method 'parse_args', got '{value}' instead")
+        else:
+            raise Exception(f"Unsupported argument data type : '{dtype}', try using basic types (int, float, str, list, dict, bool) instead")
+        
+        return type_casted_value
+
+    def __validate_and_typecast(self, dtype, value):
 
         if dtype == str:
-            return value
+            return True, value
 
         if dtype in [int, float]:
-            type_casted_value = dtype(value)
-        elif dtype in [list, tuple, dict, bool, set]:
-            type_casted_value = ast.literal_eval(value)
+            try:
+                type_casted_value = dtype(value)
+                return True, type_casted_value
+            except ValueError as err:
+                return False, value
+        elif dtype in [list, dict, bool]:
+            try:
+                type_casted_value = ast.literal_eval(value)
+                return (dtype == type(type_casted_value)), type_casted_value
+            except (SyntaxError, ValueError, Exception) as err:
+                return False, value
         elif dtype in [inspect._empty]:
             type_casted_value = value
-        else:
-            raise Exception(
-                f"Unsupported argument data type : {dtype}, try using basic types (int, float, str, list, tuple, set, dict, bool) instead")
-
-        return type_casted_value
+            return True, type_casted_value
 
     def __solve_schema(self, func, inps):
 
         mod_args = []
         for i in range(len(inps['args'])):
-            type = func['kwargs'][func['args'][i]]['type']
+            var_name = func['args'][i]
+            type = func['kwargs'][var_name]['type']
             val = inps['args'][i]
-            mod_args.append(self.__type(type, val))
+            mod_args.append(self.__type(var_name, type, val))
 
         mod_kwargs = {}
         for key, val in inps['kwargs'].items():
+            var_name = key
             type = func['kwargs'][key]['type']
             val = val['value']
-            mod_kwargs[key] = self.__type(type, val)
+            mod_kwargs[key] = self.__type(var_name, type, val)
 
         return mod_args, mod_kwargs
 
     def __func2schema(self, func_name):
 
         sign = inspect.signature(getattr(self, func_name))
         args = []
         kwargs = {}
         for key, val in sign.parameters.items():
             if val.default == inspect._empty:
-                kwargs[key] = {'value': '_empty',
+                kwargs[key] = {'value': val.default,
                                'type': val.annotation}
             else:
                 kwargs[key] = {'value': val.default,
                                'type': val.annotation}
             args.append(key)
 
-        if sign.return_annotation == inspect._empty:
-            ret_anno = '_empty'
-        else:
-            ret_anno = sign.return_annotation
-
         func_dict = {
             func_name: {
                 'args': args,
                 'kwargs': kwargs
             },
-            'ret_type': ret_anno
+            'ret_type': sign.return_annotation
         }
         return func_dict
 
     def __args2schema(self, func_name, inp_args):
 
         args = []
         kwargs = {}
         kwargs_started = False
         for i in range(len(inp_args)):
-            kwargs_found = re.match("^-(\\S+)=(\\S+)$", inp_args[i])
+            kwargs_found = re.match("^-(\\S+)=(\\S.+)$", inp_args[i])
             if kwargs_found:
                 key, value = kwargs_found.groups()
                 kwargs[key] = {'value': value}
                 kwargs_started = True
             else:
                 if kwargs_started:
                     raise SyntaxError(
-                        f"positional argument follows keyword argument {key}")
+                        f"positional argument follows keyword argument '{key}'")
                 else:
                     args.append(inp_args[i])
 
         func_dict = {func_name: {'args': args, 'kwargs': kwargs}}
         return func_dict
 
     def __doc(self, name):
@@ -142,21 +164,32 @@
 
         func_docs = inspect.getdoc(obj)
         if func_docs:
             print(" |  Usage :")
             print(f" |    ")
             docs = func_docs.splitlines()
             if len(docs) == 1:
-                print(f" |    { docs[0].strip().replace('<__file__>', __main__.__file__) }  ")
+                print(f" |    { self.__mult_repl(docs[0], {'<__file__>': __main__.__file__}) }  ")
             else:
-                print(f" |    { docs[0].strip().replace('<__file__>', __main__.__file__) }  ")
+                print(f" |    { self.__mult_repl(docs[0], {'<__file__>': __main__.__file__}) }  ")
                 for i in range(1, len(docs)-1):
-                    print(f" |    { docs[i].strip().replace('<__file__>', __main__.__file__) } ")
-                print(f" |    { docs[-1].strip().replace('<__file__>', __main__.__file__) }  ")
+                    print(f" |    { self.__mult_repl(docs[i], {'<__file__>': __main__.__file__}) } ")
+                print(f" |    { self.__mult_repl(docs[-1], {'<__file__>': __main__.__file__}) }  ")
             print(f" |    ")
 
         if sign.return_annotation != sign.empty:
             if sign.return_annotation == None:
                 print(f" | -> {None} (Returnable)")
             else:
                 print(
-                    f" | -> {sign.return_annotation.__name__} (Returnable)")
+                    f" | -> {sign.return_annotation.__name__} (Returnable)")
+        else:
+            print(f" | -> Any (Returnable)")
+
+    def __mult_repl(self, str_inp, replacements):
+
+        inp = str_inp.strip()
+        if 'python' in inp:
+            for key, value in replacements.items():
+                inp = inp.replace(key, value)
+
+        return inp
```

### Comparing `py4cli-0.0.4/SRCS/py4cli.egg-info/SOURCES.txt` & `py4cli-0.0.5/SRCS/py4cli.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,94 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-requirements.txt
+rel_reqs.txt
 setup.py
+test_reqs.txt
 SRCS/py4cli/minimal.py
+SRCS/py4cli/moderate.py
 SRCS/py4cli.egg-info/PKG-INFO
 SRCS/py4cli.egg-info/SOURCES.txt
 SRCS/py4cli.egg-info/dependency_links.txt
 SRCS/py4cli.egg-info/requires.txt
 SRCS/py4cli.egg-info/top_level.txt
 TESTS/conftest.py
-TESTS/test_basic_call.py
-TESTS/test_basic_os.py
-TESTS/ref_files/bool.txt
-TESTS/ref_files/bool_args.txt
-TESTS/ref_files/bool_h.txt
-TESTS/ref_files/bool_help.txt
-TESTS/ref_files/bool_kwargs.txt
-TESTS/ref_files/dict.txt
-TESTS/ref_files/dict_args.txt
-TESTS/ref_files/dict_h.txt
-TESTS/ref_files/dict_help.txt
-TESTS/ref_files/dict_kwargs.txt
-TESTS/ref_files/float.txt
-TESTS/ref_files/float_args.txt
-TESTS/ref_files/float_h.txt
-TESTS/ref_files/float_help.txt
-TESTS/ref_files/float_kwargs.txt
-TESTS/ref_files/int.txt
-TESTS/ref_files/int_args.txt
-TESTS/ref_files/int_h.txt
-TESTS/ref_files/int_help.txt
-TESTS/ref_files/int_kwargs.txt
-TESTS/ref_files/list.txt
-TESTS/ref_files/list_args.txt
-TESTS/ref_files/list_h.txt
-TESTS/ref_files/list_help.txt
-TESTS/ref_files/list_kwargs.txt
-TESTS/ref_files/multi.txt
-TESTS/ref_files/multi_args.txt
-TESTS/ref_files/multi_h.txt
-TESTS/ref_files/multi_help.txt
-TESTS/ref_files/multi_kwargs.txt
-TESTS/ref_files/multi_mix1.txt
-TESTS/ref_files/multi_mix2.txt
-TESTS/ref_files/multi_mix3.txt
-TESTS/ref_files/set.txt
-TESTS/ref_files/set_args.txt
-TESTS/ref_files/set_h.txt
-TESTS/ref_files/set_help.txt
-TESTS/ref_files/set_kwargs.txt
-TESTS/ref_files/str.txt
-TESTS/ref_files/str_args.txt
-TESTS/ref_files/str_h.txt
-TESTS/ref_files/str_help.txt
-TESTS/ref_files/str_kwargs.txt
-TESTS/ref_files/tuple.txt
-TESTS/ref_files/tuple_args.txt
-TESTS/ref_files/tuple_h.txt
-TESTS/ref_files/tuple_help.txt
-TESTS/ref_files/tuple_kwargs.txt
-TESTS/scripts/basic_usage.py
-TESTS/scripts/multi_args.py
-TESTS/scripts/use_bool.py
-TESTS/scripts/use_dict.py
-TESTS/scripts/use_float.py
-TESTS/scripts/use_int.py
-TESTS/scripts/use_list.py
-TESTS/scripts/use_set.py
-TESTS/scripts/use_str.py
-TESTS/scripts/use_tuple.py
+TESTS/test_min_call.py
+TESTS/test_min_os.py
+TESTS/test_min_warn.py
+TESTS/test_mod_call.py
+TESTS/test_mod_os.py
+TESTS/test_mod_warn.py
+TESTS/minimal_scripts/basic_usage.py
+TESTS/minimal_scripts/multi_args.py
+TESTS/minimal_scripts/use_bool.py
+TESTS/minimal_scripts/use_dict.py
+TESTS/minimal_scripts/use_float.py
+TESTS/minimal_scripts/use_int.py
+TESTS/minimal_scripts/use_list.py
+TESTS/minimal_scripts/use_str.py
+TESTS/moderate_scripts/basic_usage.py
+TESTS/ref_files/min_bool.txt
+TESTS/ref_files/min_bool_args.txt
+TESTS/ref_files/min_bool_h.txt
+TESTS/ref_files/min_bool_help.txt
+TESTS/ref_files/min_bool_kwargs.txt
+TESTS/ref_files/min_dict.txt
+TESTS/ref_files/min_dict_args.txt
+TESTS/ref_files/min_dict_h.txt
+TESTS/ref_files/min_dict_help.txt
+TESTS/ref_files/min_dict_kwargs.txt
+TESTS/ref_files/min_float.txt
+TESTS/ref_files/min_float_args.txt
+TESTS/ref_files/min_float_h.txt
+TESTS/ref_files/min_float_help.txt
+TESTS/ref_files/min_float_kwargs.txt
+TESTS/ref_files/min_int.txt
+TESTS/ref_files/min_int_args.txt
+TESTS/ref_files/min_int_h.txt
+TESTS/ref_files/min_int_help.txt
+TESTS/ref_files/min_int_kwargs.txt
+TESTS/ref_files/min_list.txt
+TESTS/ref_files/min_list_args.txt
+TESTS/ref_files/min_list_h.txt
+TESTS/ref_files/min_list_help.txt
+TESTS/ref_files/min_list_kwargs.txt
+TESTS/ref_files/min_multi.txt
+TESTS/ref_files/min_multi_args.txt
+TESTS/ref_files/min_multi_h.txt
+TESTS/ref_files/min_multi_help.txt
+TESTS/ref_files/min_multi_kwargs.txt
+TESTS/ref_files/min_multi_mix1.txt
+TESTS/ref_files/min_multi_mix2.txt
+TESTS/ref_files/min_multi_mix3.txt
+TESTS/ref_files/min_str.txt
+TESTS/ref_files/min_str_args.txt
+TESTS/ref_files/min_str_h.txt
+TESTS/ref_files/min_str_help.txt
+TESTS/ref_files/min_str_kwargs.txt
+TESTS/ref_files/mod.txt
+TESTS/ref_files/mod_bool.txt
+TESTS/ref_files/mod_bool_args.txt
+TESTS/ref_files/mod_bool_kwargs.txt
+TESTS/ref_files/mod_dict.txt
+TESTS/ref_files/mod_dict_args.txt
+TESTS/ref_files/mod_dict_kwargs.txt
+TESTS/ref_files/mod_float.txt
+TESTS/ref_files/mod_float_args.txt
+TESTS/ref_files/mod_float_kwargs.txt
+TESTS/ref_files/mod_h.txt
+TESTS/ref_files/mod_help.txt
+TESTS/ref_files/mod_int.txt
+TESTS/ref_files/mod_int_args.txt
+TESTS/ref_files/mod_int_kwargs.txt
+TESTS/ref_files/mod_list.txt
+TESTS/ref_files/mod_list_args.txt
+TESTS/ref_files/mod_list_kwargs.txt
+TESTS/ref_files/mod_multi.txt
+TESTS/ref_files/mod_multi_args.txt
+TESTS/ref_files/mod_multi_kwargs.txt
+TESTS/ref_files/mod_multi_mix1.txt
+TESTS/ref_files/mod_multi_mix2.txt
+TESTS/ref_files/mod_multi_mix3.txt
+TESTS/ref_files/mod_str.txt
+TESTS/ref_files/mod_str_args.txt
+TESTS/ref_files/mod_str_kwargs.txt
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/bool_h.txt` & `py4cli-0.0.5/TESTS/ref_files/min_bool_h.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-['scripts/use_bool.py', '-h']
+['minimal_scripts/use_bool.py', '-h']
 
  | > def parse_args 
  |    
  |  Description :
  |    
  |    example parse_args template function with single argument of type <bool>  
  |    
@@ -10,16 +10,16 @@
  |    
  |   -inp_bool: bool = False
  |    
  |  Usage :
  |    
  |    inp_bool is variable of type <bool>  
  |    any bool value can be passed for the argument, while the default is False 
- |    the function returns the same arg value as type <dict> 
+ |    the function returns the same arg value as type <bool> 
  |     
  |    cmds : 
- |    1. python scripts/use_bool.py True 
- |    2. python scripts/use_bool.py -inp_bool=True  
+ |    1. python minimal_scripts/use_bool.py True 
+ |    2. python minimal_scripts/use_bool.py -inp_bool=True  
  |    
  | -> bool (Returnable)
 
 None <class 'NoneType'>
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/bool_help.txt` & `py4cli-0.0.5/TESTS/ref_files/min_bool_help.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-['scripts/use_bool.py', '--help']
+['minimal_scripts/use_bool.py', '--help']
 
  | > def parse_args 
  |    
  |  Description :
  |    
  |    example parse_args template function with single argument of type <bool>  
  |    
@@ -10,16 +10,16 @@
  |    
  |   -inp_bool: bool = False
  |    
  |  Usage :
  |    
  |    inp_bool is variable of type <bool>  
  |    any bool value can be passed for the argument, while the default is False 
- |    the function returns the same arg value as type <dict> 
+ |    the function returns the same arg value as type <bool> 
  |     
  |    cmds : 
- |    1. python scripts/use_bool.py True 
- |    2. python scripts/use_bool.py -inp_bool=True  
+ |    1. python minimal_scripts/use_bool.py True 
+ |    2. python minimal_scripts/use_bool.py -inp_bool=True  
  |    
  | -> bool (Returnable)
 
 None <class 'NoneType'>
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/dict_h.txt` & `py4cli-0.0.5/TESTS/ref_files/min_dict_h.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-['scripts/use_dict.py', '-h']
+['minimal_scripts/use_dict.py', '-h']
 
  | > def parse_args 
  |    
  |  Description :
  |    
  |    example parse_args template function with single argument of type <dict>  
  |    
@@ -13,13 +13,13 @@
  |  Usage :
  |    
  |    inp_dict is variable of type <dict>  
  |    any dict value can be passed for the argument, while the default is {None: None} 
  |    the function returns the same arg value as type <dict> 
  |     
  |    cmds : 
- |    1. python scripts/use_dict.py {"Empty":"Empty"} 
- |    2. python scripts/use_dict.py -inp_dict={"Empty":"Empty"}  
+ |    1. python minimal_scripts/use_dict.py {"Empty":"Empty"} 
+ |    2. python minimal_scripts/use_dict.py -inp_dict={"Empty":"Empty"}  
  |    
  | -> dict (Returnable)
 
 None <class 'NoneType'>
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/dict_help.txt` & `py4cli-0.0.5/TESTS/ref_files/min_dict_help.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-['scripts/use_dict.py', '--help']
+['minimal_scripts/use_dict.py', '--help']
 
  | > def parse_args 
  |    
  |  Description :
  |    
  |    example parse_args template function with single argument of type <dict>  
  |    
@@ -13,13 +13,13 @@
  |  Usage :
  |    
  |    inp_dict is variable of type <dict>  
  |    any dict value can be passed for the argument, while the default is {None: None} 
  |    the function returns the same arg value as type <dict> 
  |     
  |    cmds : 
- |    1. python scripts/use_dict.py {"Empty":"Empty"} 
- |    2. python scripts/use_dict.py -inp_dict={"Empty":"Empty"}  
+ |    1. python minimal_scripts/use_dict.py {"Empty":"Empty"} 
+ |    2. python minimal_scripts/use_dict.py -inp_dict={"Empty":"Empty"}  
  |    
  | -> dict (Returnable)
 
 None <class 'NoneType'>
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/float_h.txt` & `py4cli-0.0.5/TESTS/ref_files/min_float_help.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-['scripts/use_float.py', '-h']
+['minimal_scripts/use_float.py', '--help']
 
  | > def parse_args 
  |    
  |  Description :
  |    
  |    example parse_args template function with single argument of type <float>  
  |    
@@ -13,13 +13,13 @@
  |  Usage :
  |    
  |    inp_float is variable of type <float>  
  |    any floating point value can be passed for the argument, while the default is 0.0 
  |    the function returns the same arg value as type <float> 
  |     
  |    cmds : 
- |    1. python scripts/use_float.py 10.0 
- |    2. python scripts/use_float.py -inp_float=10.0  
+ |    1. python minimal_scripts/use_float.py 10.0 
+ |    2. python minimal_scripts/use_float.py -inp_float=10.0  
  |    
  | -> float (Returnable)
 
 None <class 'NoneType'>
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/float_help.txt` & `py4cli-0.0.5/TESTS/ref_files/min_float_h.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-['scripts/use_float.py', '--help']
+['minimal_scripts/use_float.py', '-h']
 
  | > def parse_args 
  |    
  |  Description :
  |    
  |    example parse_args template function with single argument of type <float>  
  |    
@@ -13,13 +13,13 @@
  |  Usage :
  |    
  |    inp_float is variable of type <float>  
  |    any floating point value can be passed for the argument, while the default is 0.0 
  |    the function returns the same arg value as type <float> 
  |     
  |    cmds : 
- |    1. python scripts/use_float.py 10.0 
- |    2. python scripts/use_float.py -inp_float=10.0  
+ |    1. python minimal_scripts/use_float.py 10.0 
+ |    2. python minimal_scripts/use_float.py -inp_float=10.0  
  |    
  | -> float (Returnable)
 
 None <class 'NoneType'>
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/list_help.txt` & `py4cli-0.0.5/TESTS/ref_files/min_list_help.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-00000000: 5b27 7363 7269 7074 732f 7573 655f 6c69  ['scripts/use_li
-00000010: 7374 2e70 7927 2c20 272d 2d68 656c 7027  st.py', '--help'
-00000020: 5d0d 0a0d 0a20 7c20 3e20 6465 6620 7061  ].... | > def pa
-00000030: 7273 655f 6172 6773 200d 0a20 7c20 2020  rse_args .. |   
-00000040: 200d 0a20 7c20 2044 6573 6372 6970 7469   .. |  Descripti
-00000050: 6f6e 203a 0d0a 207c 2020 2020 0d0a 207c  on :.. |    .. |
-00000060: 2020 2020 6578 616d 706c 6520 7061 7273      example pars
-00000070: 655f 6172 6773 2074 656d 706c 6174 6520  e_args template 
-00000080: 6675 6e63 7469 6f6e 2077 6974 6820 7369  function with si
-00000090: 6e67 6c65 2061 7267 756d 656e 7420 6f66  ngle argument of
-000000a0: 2074 7970 6520 3c6c 6973 743e 2020 0d0a   type <list>  ..
-000000b0: 207c 2020 2020 0d0a 207c 2020 4172 6775   |    .. |  Argu
-000000c0: 6d65 6e74 7320 3a0d 0a20 7c20 2020 200d  ments :.. |    .
-000000d0: 0a20 7c20 2020 2d69 6e70 5f6c 6973 743a  . |   -inp_list:
-000000e0: 206c 6973 7420 3d20 5b4e 6f6e 655d 0d0a   list = [None]..
-000000f0: 207c 2020 2020 0d0a 207c 2020 5573 6167   |    .. |  Usag
-00000100: 6520 3a0d 0a20 7c20 2020 200d 0a20 7c20  e :.. |    .. | 
-00000110: 2020 2069 6e70 5f6c 6973 7420 6973 2076     inp_list is v
-00000120: 6172 6961 626c 6520 6f66 2074 7970 6520  ariable of type 
-00000130: 3c6c 6973 743e 2020 0d0a 207c 2020 2020  <list>  .. |    
-00000140: 616e 7920 6c69 7374 2076 616c 7565 2063  any list value c
-00000150: 616e 2062 6520 7061 7373 6564 2066 6f72  an be passed for
-00000160: 2074 6865 2061 7267 756d 656e 742c 2077   the argument, w
-00000170: 6869 6c65 2074 6865 2064 6566 6175 6c74  hile the default
-00000180: 2069 7320 5b4e 6f6e 655d 200d 0a20 7c20   is [None] .. | 
-00000190: 2020 2074 6865 2066 756e 6374 696f 6e20     the function 
-000001a0: 7265 7475 726e 7320 7468 6520 7361 6d65  returns the same
-000001b0: 2061 7267 2076 616c 7565 2061 7320 7479   arg value as ty
-000001c0: 7065 203c 6c69 7374 3e20 0d0a 207c 2020  pe <list> .. |  
-000001d0: 2020 200d 0a20 7c20 2020 2063 6d64 7320     .. |    cmds 
-000001e0: 3a20 0d0a 207c 2020 2020 312e 2070 7974  : .. |    1. pyt
-000001f0: 686f 6e20 7363 7269 7074 732f 7573 655f  hon scripts/use_
-00000200: 6c69 7374 2e70 7920 5b22 456d 7074 7922  list.py ["Empty"
-00000210: 5d20 0d0a 207c 2020 2020 322e 2070 7974  ] .. |    2. pyt
-00000220: 686f 6e20 7363 7269 7074 732f 7573 655f  hon scripts/use_
-00000230: 6c69 7374 2e70 7920 2d69 6e70 5f6c 6973  list.py -inp_lis
-00000240: 743d 5b22 456d 7074 7922 5d20 200d 0a20  t=["Empty"]  .. 
-00000250: 7c20 2020 200d 0a20 7c20 2d3e 206c 6973  |    .. | -> lis
-00000260: 7420 2852 6574 7572 6e61 626c 6529 0d0a  t (Returnable)..
-00000270: 0d0a 4e6f 6e65 203c 636c 6173 7320 274e  ..None <class 'N
-00000280: 6f6e 6554 7970 6527 3e0d 0a              oneType'>..
+00000000: 5b27 6d69 6e69 6d61 6c5f 7363 7269 7074  ['minimal_script
+00000010: 732f 7573 655f 6c69 7374 2e70 7927 2c20  s/use_list.py', 
+00000020: 272d 2d68 656c 7027 5d0d 0a0d 0a20 7c20  '--help'].... | 
+00000030: 3e20 6465 6620 7061 7273 655f 6172 6773  > def parse_args
+00000040: 200d 0a20 7c20 2020 200d 0a20 7c20 2044   .. |    .. |  D
+00000050: 6573 6372 6970 7469 6f6e 203a 0d0a 207c  escription :.. |
+00000060: 2020 2020 0d0a 207c 2020 2020 6578 616d      .. |    exam
+00000070: 706c 6520 7061 7273 655f 6172 6773 2074  ple parse_args t
+00000080: 656d 706c 6174 6520 6675 6e63 7469 6f6e  emplate function
+00000090: 2077 6974 6820 7369 6e67 6c65 2061 7267   with single arg
+000000a0: 756d 656e 7420 6f66 2074 7970 6520 3c6c  ument of type <l
+000000b0: 6973 743e 2020 0d0a 207c 2020 2020 0d0a  ist>  .. |    ..
+000000c0: 207c 2020 4172 6775 6d65 6e74 7320 3a0d   |  Arguments :.
+000000d0: 0a20 7c20 2020 200d 0a20 7c20 2020 2d69  . |    .. |   -i
+000000e0: 6e70 5f6c 6973 743a 206c 6973 7420 3d20  np_list: list = 
+000000f0: 5b4e 6f6e 655d 0d0a 207c 2020 2020 0d0a  [None].. |    ..
+00000100: 207c 2020 5573 6167 6520 3a0d 0a20 7c20   |  Usage :.. | 
+00000110: 2020 200d 0a20 7c20 2020 2069 6e70 5f6c     .. |    inp_l
+00000120: 6973 7420 6973 2076 6172 6961 626c 6520  ist is variable 
+00000130: 6f66 2074 7970 6520 3c6c 6973 743e 2020  of type <list>  
+00000140: 0d0a 207c 2020 2020 616e 7920 6c69 7374  .. |    any list
+00000150: 2076 616c 7565 2063 616e 2062 6520 7061   value can be pa
+00000160: 7373 6564 2066 6f72 2074 6865 2061 7267  ssed for the arg
+00000170: 756d 656e 742c 2077 6869 6c65 2074 6865  ument, while the
+00000180: 2064 6566 6175 6c74 2069 7320 5b4e 6f6e   default is [Non
+00000190: 655d 200d 0a20 7c20 2020 2074 6865 2066  e] .. |    the f
+000001a0: 756e 6374 696f 6e20 7265 7475 726e 7320  unction returns 
+000001b0: 7468 6520 7361 6d65 2061 7267 2076 616c  the same arg val
+000001c0: 7565 2061 7320 7479 7065 203c 6c69 7374  ue as type <list
+000001d0: 3e20 0d0a 207c 2020 2020 200d 0a20 7c20  > .. |     .. | 
+000001e0: 2020 2063 6d64 7320 3a20 0d0a 207c 2020     cmds : .. |  
+000001f0: 2020 312e 2070 7974 686f 6e20 6d69 6e69    1. python mini
+00000200: 6d61 6c5f 7363 7269 7074 732f 7573 655f  mal_scripts/use_
+00000210: 6c69 7374 2e70 7920 5b22 456d 7074 7922  list.py ["Empty"
+00000220: 5d20 0d0a 207c 2020 2020 322e 2070 7974  ] .. |    2. pyt
+00000230: 686f 6e20 6d69 6e69 6d61 6c5f 7363 7269  hon minimal_scri
+00000240: 7074 732f 7573 655f 6c69 7374 2e70 7920  pts/use_list.py 
+00000250: 2d69 6e70 5f6c 6973 743d 5b22 456d 7074  -inp_list=["Empt
+00000260: 7922 5d20 200d 0a20 7c20 2020 200d 0a20  y"]  .. |    .. 
+00000270: 7c20 2d3e 206c 6973 7420 2852 6574 7572  | -> list (Retur
+00000280: 6e61 626c 6529 0d0a 0d0a 4e6f 6e65 203c  nable)....None <
+00000290: 636c 6173 7320 274e 6f6e 6554 7970 6527  class 'NoneType'
+000002a0: 3e0d 0a                                  >..
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/multi_h.txt` & `py4cli-0.0.5/TESTS/ref_files/min_multi_help.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-['scripts/multi_args.py', '-h']
+['minimal_scripts/multi_args.py', '--help']
 
  | > def parse_args 
  |    
  |  Description :
  |    
  |    example parse_args template function with multiple arguments of different types  
  |    
  |  Arguments :
  |    
  |   -inp_int: int = 6
  |   -inp_float: float = 6.0
  |   -inp_str: str = 'Six'
  |   -inp_list: list = [6, 6.0, 'Six']
- |   -inp_tuple: tuple = (6, 6.0, 'Six')
- |   -inp_set: set = {'Six'}
  |   -inp_dict: dict = {'int': 6, 'float': 6.0, 'str': 'Six'}
  |   -inp_bool: bool = False
  |    
  |  Usage :
  |    
- |    Seven arguments of different data type can be passed  
+ |    Six arguments of different data type can be passed  
  |    any value of the respective data type can be passed for specific argument. for defaults refer above 
- |    the function returns a json string containing all the arguments and its values. 
+ |    the function returns a dict containing all the arguments and its values. 
  |     
  |    cmds : 
- |    1. python scripts/multi_args.py 10 10.0 Seven [10,10.0,'Seven'] (10,10.0,'Seven') {10,10.0,'Seven'} {'int':10,'float':10.0,'str':'Seven'} True 
- |    2. python scripts/multi_args.py -inp_int=10 -inp_float=10.0 -inp_str=Seven -inp_list=[10,10.0,'Seven'] -inp_tuple=(10,10.0,'Seven') -inp_set={10,10.0,'Seven'} -inp_dict={'int':10,'float':10.0,'str':'Seven'} -inp_bool=True  
+ |    1. python minimal_scripts/multi_args.py 10 10.0 Seven [10,10.0,'Seven'] {'int':10,'float':10.0,'str':'Seven'} True 
+ |    2. python minimal_scripts/multi_args.py -inp_int=10 -inp_float=10.0 -inp_str=Seven -inp_list=[10,10.0,'Seven'] -inp_dict={'int':10,'float':10.0,'str':'Seven'} -inp_bool=True  
  |    
  | -> dict (Returnable)
 
 None <class 'NoneType'>
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/set_h.txt` & `py4cli-0.0.5/TESTS/ref_files/min_str_h.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-['scripts/use_set.py', '-h']
+['minimal_scripts/use_str.py', '-h']
 
  | > def parse_args 
  |    
  |  Description :
  |    
- |    example parse_args template function with single argument of type <set>  
+ |    example parse_args template function with single argument of type <str>  
  |    
  |  Arguments :
  |    
- |   -inp_set: set = {None}
+ |   -inp_str: str = 'None'
  |    
  |  Usage :
  |    
- |    inp_set is variable of type <set>  
- |    any set value can be passed for the argument, while the default is {None} 
- |    the function returns the same arg value as type <set> 
+ |    inp_str is variable of type <str>  
+ |    any string value can be passed for the argument, while the default is "None" 
+ |    the function returns the same arg value as type <str> 
  |     
  |    cmds : 
- |    1. python scripts/use_set.py {'Empty'} 
- |    2. python scripts/use_set.py -inp_set={'Empty'}  
+ |    1. python minimal_scripts/use_str.py Empty 
+ |    2. python minimal_scripts/use_str.py -inp_str=Empty  
  |    
- | -> set (Returnable)
+ | -> str (Returnable)
 
 None <class 'NoneType'>
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/set_help.txt` & `py4cli-0.0.5/TESTS/ref_files/min_str_help.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-['scripts/use_set.py', '--help']
+['minimal_scripts/use_str.py', '--help']
 
  | > def parse_args 
  |    
  |  Description :
  |    
- |    example parse_args template function with single argument of type <set>  
+ |    example parse_args template function with single argument of type <str>  
  |    
  |  Arguments :
  |    
- |   -inp_set: set = {None}
+ |   -inp_str: str = 'None'
  |    
  |  Usage :
  |    
- |    inp_set is variable of type <set>  
- |    any set value can be passed for the argument, while the default is {None} 
- |    the function returns the same arg value as type <set> 
+ |    inp_str is variable of type <str>  
+ |    any string value can be passed for the argument, while the default is "None" 
+ |    the function returns the same arg value as type <str> 
  |     
  |    cmds : 
- |    1. python scripts/use_set.py {'Empty'} 
- |    2. python scripts/use_set.py -inp_set={'Empty'}  
+ |    1. python minimal_scripts/use_str.py Empty 
+ |    2. python minimal_scripts/use_str.py -inp_str=Empty  
  |    
- | -> set (Returnable)
+ | -> str (Returnable)
 
 None <class 'NoneType'>
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/str_h.txt` & `py4cli-0.0.5/TESTS/ref_files/min_int_h.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-['scripts/use_str.py', '-h']
+['minimal_scripts/use_int.py', '-h']
 
  | > def parse_args 
  |    
  |  Description :
  |    
- |    example parse_args template function with single argument of type <str>  
+ |    example parse_args template function with single argument of type <int>  
  |    
  |  Arguments :
  |    
- |   -inp_str: str = 'None'
+ |   -inp_int: int = 0
  |    
  |  Usage :
  |    
- |    inp_str is variable of type <str>  
- |    any string value can be passed for the argument, while the default is "None" 
- |    the function returns the same arg value as type <str> 
+ |    inp_int is variable of type <int>  
+ |    any integer value can be passed for the argument, while the default is 0 
+ |    the function returns the same arg value as type <int> 
  |     
  |    cmds : 
- |    1. python scripts/use_str.py Empty 
- |    2. python scripts/use_str.py -inp_str=Empty  
+ |    1. python minimal_scripts/use_int.py 10 
+ |    2. python minimal_scripts/use_int.py -inp_int=10  
  |    
- | -> str (Returnable)
+ | -> int (Returnable)
 
 None <class 'NoneType'>
```

### Comparing `py4cli-0.0.4/TESTS/ref_files/str_help.txt` & `py4cli-0.0.5/TESTS/ref_files/min_int_help.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-['scripts/use_str.py', '--help']
+['minimal_scripts/use_int.py', '--help']
 
  | > def parse_args 
  |    
  |  Description :
  |    
- |    example parse_args template function with single argument of type <str>  
+ |    example parse_args template function with single argument of type <int>  
  |    
  |  Arguments :
  |    
- |   -inp_str: str = 'None'
+ |   -inp_int: int = 0
  |    
  |  Usage :
  |    
- |    inp_str is variable of type <str>  
- |    any string value can be passed for the argument, while the default is "None" 
- |    the function returns the same arg value as type <str> 
+ |    inp_int is variable of type <int>  
+ |    any integer value can be passed for the argument, while the default is 0 
+ |    the function returns the same arg value as type <int> 
  |     
  |    cmds : 
- |    1. python scripts/use_str.py Empty 
- |    2. python scripts/use_str.py -inp_str=Empty  
+ |    1. python minimal_scripts/use_int.py 10 
+ |    2. python minimal_scripts/use_int.py -inp_int=10  
  |    
- | -> str (Returnable)
+ | -> int (Returnable)
 
 None <class 'NoneType'>
```

### Comparing `py4cli-0.0.4/TESTS/scripts/basic_usage.py` & `py4cli-0.0.5/TESTS/minimal_scripts/basic_usage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,371 +1,415 @@
-00000000: 0d0a 0d0a 6672 6f6d 2070 7934 636c 692e  ....from py4cli.
-00000010: 6d69 6e69 6d61 6c20 696d 706f 7274 2061  minimal import a
-00000020: 7267 5f70 6172 7365 720d 0a0d 0a23 2053  rg_parser....# S
-00000030: 696e 676c 6520 6172 6775 6d65 6e74 2065  ingle argument e
-00000040: 7861 6d70 6c65 730d 0a0d 0a63 6c61 7373  xamples....class
-00000050: 2073 696e 676c 655f 696e 7428 6172 675f   single_int(arg_
-00000060: 7061 7273 6572 293a 0d0a 0d0a 2020 2020  parser):....    
-00000070: 2320 6578 616d 706c 6520 7061 7273 655f  # example parse_
-00000080: 6172 6773 2074 656d 706c 6174 6520 6675  args template fu
-00000090: 6e63 7469 6f6e 2077 6974 6820 7369 6e67  nction with sing
-000000a0: 6c65 2061 7267 756d 656e 7420 6f66 2074  le argument of t
-000000b0: 7970 6520 3c69 6e74 3e0d 0a20 2020 2064  ype <int>..    d
-000000c0: 6566 2070 6172 7365 5f61 7267 7328 7365  ef parse_args(se
-000000d0: 6c66 2c20 696e 705f 696e 743a 2069 6e74  lf, inp_int: int
-000000e0: 203d 2030 2920 2d3e 2069 6e74 3a0d 0a20   = 0) -> int:.. 
-000000f0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00000100: 2020 2020 696e 705f 696e 7420 6973 2076      inp_int is v
-00000110: 6172 6961 626c 6520 6f66 2074 7970 6520  ariable of type 
-00000120: 3c69 6e74 3e0d 0a20 2020 2020 2020 2061  <int>..        a
-00000130: 6e79 2069 6e74 6567 6572 2076 616c 7565  ny integer value
-00000140: 2063 616e 2062 6520 7061 7373 6564 2066   can be passed f
-00000150: 6f72 2074 6865 2061 7267 756d 656e 742c  or the argument,
-00000160: 2077 6869 6c65 2074 6865 2064 6566 6175   while the defau
-00000170: 6c74 2069 7320 300d 0a20 2020 2020 2020  lt is 0..       
-00000180: 2074 6865 2066 756e 6374 696f 6e20 7265   the function re
-00000190: 7475 726e 7320 7468 6520 7361 6d65 2061  turns the same a
-000001a0: 7267 2076 616c 7565 2061 7320 7479 7065  rg value as type
-000001b0: 203c 696e 743e 200d 0a0d 0a20 2020 2020   <int> ....     
-000001c0: 2020 2063 6d64 7320 3a0d 0a20 2020 2020     cmds :..     
-000001d0: 2020 2020 2020 2031 2e20 7079 7468 6f6e         1. python
-000001e0: 203c 5f5f 6669 6c65 5f5f 3e20 3130 0d0a   <__file__> 10..
-000001f0: 2020 2020 2020 2020 2020 2020 322e 2070              2. p
-00000200: 7974 686f 6e20 3c5f 5f66 696c 655f 5f3e  ython <__file__>
-00000210: 202d 696e 705f 696e 743d 3130 0d0a 2020   -inp_int=10..  
-00000220: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00000230: 2020 2072 6574 7572 6e20 696e 705f 696e     return inp_in
-00000240: 740d 0a20 2020 200d 0a63 6c61 7373 2073  t..    ..class s
-00000250: 696e 676c 655f 666c 6f61 7428 6172 675f  ingle_float(arg_
-00000260: 7061 7273 6572 293a 0d0a 0d0a 2020 2020  parser):....    
-00000270: 2320 6578 616d 706c 6520 7061 7273 655f  # example parse_
-00000280: 6172 6773 2074 656d 706c 6174 6520 6675  args template fu
-00000290: 6e63 7469 6f6e 2077 6974 6820 7369 6e67  nction with sing
-000002a0: 6c65 2061 7267 756d 656e 7420 6f66 2074  le argument of t
-000002b0: 7970 6520 3c66 6c6f 6174 3e0d 0a20 2020  ype <float>..   
-000002c0: 2064 6566 2070 6172 7365 5f61 7267 7328   def parse_args(
-000002d0: 7365 6c66 2c20 696e 705f 666c 6f61 743a  self, inp_float:
-000002e0: 2066 6c6f 6174 203d 2030 2e30 2920 2d3e   float = 0.0) ->
-000002f0: 2066 6c6f 6174 3a0d 0a20 2020 2020 2020   float:..       
-00000300: 2022 2222 0d0a 2020 2020 2020 2020 696e   """..        in
-00000310: 705f 666c 6f61 7420 6973 2076 6172 6961  p_float is varia
-00000320: 626c 6520 6f66 2074 7970 6520 3c66 6c6f  ble of type <flo
-00000330: 6174 3e0d 0a20 2020 2020 2020 2061 6e79  at>..        any
-00000340: 2066 6c6f 6174 696e 6720 706f 696e 7420   floating point 
-00000350: 7661 6c75 6520 6361 6e20 6265 2070 6173  value can be pas
-00000360: 7365 6420 666f 7220 7468 6520 6172 6775  sed for the argu
-00000370: 6d65 6e74 2c20 7768 696c 6520 7468 6520  ment, while the 
-00000380: 6465 6661 756c 7420 6973 2030 2e30 0d0a  default is 0.0..
-00000390: 2020 2020 2020 2020 7468 6520 6675 6e63          the func
-000003a0: 7469 6f6e 2072 6574 7572 6e73 2074 6865  tion returns the
-000003b0: 2073 616d 6520 6172 6720 7661 6c75 6520   same arg value 
-000003c0: 6173 2074 7970 6520 3c66 6c6f 6174 3e20  as type <float> 
-000003d0: 0d0a 0d0a 2020 2020 2020 2020 636d 6473  ....        cmds
-000003e0: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
-000003f0: 312e 2070 7974 686f 6e20 3c5f 5f66 696c  1. python <__fil
-00000400: 655f 5f3e 2031 302e 300d 0a20 2020 2020  e__> 10.0..     
-00000410: 2020 2020 2020 2032 2e20 7079 7468 6f6e         2. python
-00000420: 203c 5f5f 6669 6c65 5f5f 3e20 2d69 6e70   <__file__> -inp
-00000430: 5f66 6c6f 6174 3d31 302e 300d 0a20 2020  _float=10.0..   
-00000440: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00000450: 2020 7265 7475 726e 2069 6e70 5f66 6c6f    return inp_flo
-00000460: 6174 0d0a 2020 2020 0d0a 636c 6173 7320  at..    ..class 
-00000470: 7369 6e67 6c65 5f73 7472 2861 7267 5f70  single_str(arg_p
-00000480: 6172 7365 7229 3a0d 0a0d 0a20 2020 2023  arser):....    #
-00000490: 2065 7861 6d70 6c65 2070 6172 7365 5f61   example parse_a
-000004a0: 7267 7320 7465 6d70 6c61 7465 2066 756e  rgs template fun
-000004b0: 6374 696f 6e20 7769 7468 2073 696e 676c  ction with singl
-000004c0: 6520 6172 6775 6d65 6e74 206f 6620 7479  e argument of ty
-000004d0: 7065 203c 7374 723e 0d0a 2020 2020 6465  pe <str>..    de
-000004e0: 6620 7061 7273 655f 6172 6773 2873 656c  f parse_args(sel
-000004f0: 662c 2069 6e70 5f73 7472 3a20 7374 7220  f, inp_str: str 
-00000500: 3d20 224e 6f6e 6522 2920 2d3e 2073 7472  = "None") -> str
-00000510: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00000520: 2020 2020 2020 2020 696e 705f 7374 7220          inp_str 
-00000530: 6973 2076 6172 6961 626c 6520 6f66 2074  is variable of t
-00000540: 7970 6520 3c73 7472 3e0d 0a20 2020 2020  ype <str>..     
-00000550: 2020 2061 6e79 2073 7472 696e 6720 7661     any string va
-00000560: 6c75 6520 6361 6e20 6265 2070 6173 7365  lue can be passe
-00000570: 6420 666f 7220 7468 6520 6172 6775 6d65  d for the argume
-00000580: 6e74 2c20 7768 696c 6520 7468 6520 6465  nt, while the de
-00000590: 6661 756c 7420 6973 2022 4e6f 6e65 220d  fault is "None".
-000005a0: 0a20 2020 2020 2020 2074 6865 2066 756e  .        the fun
-000005b0: 6374 696f 6e20 7265 7475 726e 7320 7468  ction returns th
-000005c0: 6520 7361 6d65 2061 7267 2076 616c 7565  e same arg value
-000005d0: 2061 7320 7479 7065 203c 7374 723e 200d   as type <str> .
-000005e0: 0a0d 0a20 2020 2020 2020 2063 6d64 7320  ...        cmds 
-000005f0: 3a0d 0a20 2020 2020 2020 2020 2020 2031  :..            1
-00000600: 2e20 7079 7468 6f6e 203c 5f5f 6669 6c65  . python <__file
-00000610: 5f5f 3e20 456d 7074 790d 0a20 2020 2020  __> Empty..     
-00000620: 2020 2020 2020 2032 2e20 7079 7468 6f6e         2. python
-00000630: 203c 5f5f 6669 6c65 5f5f 3e20 2d69 6e70   <__file__> -inp
-00000640: 5f73 7472 3d45 6d70 7479 0d0a 2020 2020  _str=Empty..    
-00000650: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00000660: 2072 6574 7572 6e20 696e 705f 7374 720d   return inp_str.
-00000670: 0a20 2020 200d 0a63 6c61 7373 2073 696e  .    ..class sin
-00000680: 676c 655f 6c69 7374 2861 7267 5f70 6172  gle_list(arg_par
-00000690: 7365 7229 3a0d 0a0d 0a20 2020 2023 2065  ser):....    # e
-000006a0: 7861 6d70 6c65 2070 6172 7365 5f61 7267  xample parse_arg
-000006b0: 7320 7465 6d70 6c61 7465 2066 756e 6374  s template funct
-000006c0: 696f 6e20 7769 7468 2073 696e 676c 6520  ion with single 
-000006d0: 6172 6775 6d65 6e74 206f 6620 7479 7065  argument of type
-000006e0: 203c 6c69 7374 3e0d 0a20 2020 2064 6566   <list>..    def
-000006f0: 2070 6172 7365 5f61 7267 7328 7365 6c66   parse_args(self
-00000700: 2c20 696e 705f 6c69 7374 3a20 6c69 7374  , inp_list: list
-00000710: 203d 205b 4e6f 6e65 5d29 202d 3e20 6c69   = [None]) -> li
-00000720: 7374 3a0d 0a20 2020 2020 2020 2022 2222  st:..        """
-00000730: 0d0a 2020 2020 2020 2020 696e 705f 6c69  ..        inp_li
-00000740: 7374 2069 7320 7661 7269 6162 6c65 206f  st is variable o
-00000750: 6620 7479 7065 203c 6c69 7374 3e0d 0a20  f type <list>.. 
-00000760: 2020 2020 2020 2061 6e79 206c 6973 7420         any list 
-00000770: 7661 6c75 6520 6361 6e20 6265 2070 6173  value can be pas
-00000780: 7365 6420 666f 7220 7468 6520 6172 6775  sed for the argu
-00000790: 6d65 6e74 2c20 7768 696c 6520 7468 6520  ment, while the 
-000007a0: 6465 6661 756c 7420 6973 205b 4e6f 6e65  default is [None
-000007b0: 5d0d 0a20 2020 2020 2020 2074 6865 2066  ]..        the f
-000007c0: 756e 6374 696f 6e20 7265 7475 726e 7320  unction returns 
-000007d0: 7468 6520 7361 6d65 2061 7267 2076 616c  the same arg val
-000007e0: 7565 2061 7320 7479 7065 203c 6c69 7374  ue as type <list
-000007f0: 3e20 0d0a 0d0a 2020 2020 2020 2020 636d  > ....        cm
-00000800: 6473 203a 0d0a 2020 2020 2020 2020 2020  ds :..          
-00000810: 2020 312e 2070 7974 686f 6e20 3c5f 5f66    1. python <__f
-00000820: 696c 655f 5f3e 205b 2245 6d70 7479 225d  ile__> ["Empty"]
-00000830: 0d0a 2020 2020 2020 2020 2020 2020 322e  ..            2.
-00000840: 2070 7974 686f 6e20 3c5f 5f66 696c 655f   python <__file_
-00000850: 5f3e 202d 696e 705f 6c69 7374 3d5b 2245  _> -inp_list=["E
-00000860: 6d70 7479 225d 0d0a 2020 2020 2020 2020  mpty"]..        
-00000870: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
-00000880: 7572 6e20 696e 705f 6c69 7374 0d0a 2020  urn inp_list..  
-00000890: 2020 0d0a 636c 6173 7320 7369 6e67 6c65    ..class single
-000008a0: 5f74 7570 6c65 2861 7267 5f70 6172 7365  _tuple(arg_parse
-000008b0: 7229 3a0d 0a0d 0a20 2020 2023 2065 7861  r):....    # exa
-000008c0: 6d70 6c65 2070 6172 7365 5f61 7267 7320  mple parse_args 
-000008d0: 7465 6d70 6c61 7465 2066 756e 6374 696f  template functio
-000008e0: 6e20 7769 7468 2073 696e 676c 6520 6172  n with single ar
-000008f0: 6775 6d65 6e74 206f 6620 7479 7065 203c  gument of type <
-00000900: 7475 706c 653e 0d0a 2020 2020 6465 6620  tuple>..    def 
-00000910: 7061 7273 655f 6172 6773 2873 656c 662c  parse_args(self,
-00000920: 2069 6e70 5f74 7570 6c65 3a20 7475 706c   inp_tuple: tupl
-00000930: 6520 3d20 284e 6f6e 652c 2929 202d 3e20  e = (None,)) -> 
-00000940: 7475 706c 653a 0d0a 2020 2020 2020 2020  tuple:..        
-00000950: 2222 220d 0a20 2020 2020 2020 2069 6e70  """..        inp
-00000960: 5f74 7570 6c65 2069 7320 7661 7269 6162  _tuple is variab
-00000970: 6c65 206f 6620 7479 7065 203c 7475 706c  le of type <tupl
-00000980: 653e 0d0a 2020 2020 2020 2020 616e 7920  e>..        any 
-00000990: 7475 706c 6520 7661 6c75 6520 6361 6e20  tuple value can 
-000009a0: 6265 2070 6173 7365 6420 666f 7220 7468  be passed for th
-000009b0: 6520 6172 6775 6d65 6e74 2c20 7768 696c  e argument, whil
-000009c0: 6520 7468 6520 6465 6661 756c 7420 6973  e the default is
-000009d0: 2028 4e6f 6e65 2c29 0d0a 2020 2020 2020   (None,)..      
-000009e0: 2020 7468 6520 6675 6e63 7469 6f6e 2072    the function r
-000009f0: 6574 7572 6e73 2074 6865 2073 616d 6520  eturns the same 
-00000a00: 6172 6720 7661 6c75 6520 6173 2074 7970  arg value as typ
-00000a10: 6520 3c74 7570 6c65 3e20 0d0a 0d0a 2020  e <tuple> ....  
-00000a20: 2020 2020 2020 636d 6473 203a 0d0a 2020        cmds :..  
-00000a30: 2020 2020 2020 2020 2020 312e 2070 7974            1. pyt
-00000a40: 686f 6e20 3c5f 5f66 696c 655f 5f3e 2028  hon <__file__> (
-00000a50: 2245 6d70 7479 222c 290d 0a20 2020 2020  "Empty",)..     
-00000a60: 2020 2020 2020 2032 2e20 7079 7468 6f6e         2. python
-00000a70: 203c 5f5f 6669 6c65 5f5f 3e20 2d69 6e70   <__file__> -inp
-00000a80: 5f74 7570 6c65 3d28 2245 6d70 7479 222c  _tuple=("Empty",
-00000a90: 290d 0a20 2020 2020 2020 2022 2222 0d0a  )..        """..
-00000aa0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00000ab0: 6e70 5f74 7570 6c65 0d0a 2020 2020 0d0a  np_tuple..    ..
-00000ac0: 636c 6173 7320 7369 6e67 6c65 5f73 6574  class single_set
-00000ad0: 2861 7267 5f70 6172 7365 7229 3a0d 0a0d  (arg_parser):...
-00000ae0: 0a20 2020 2023 2065 7861 6d70 6c65 2070  .    # example p
-00000af0: 6172 7365 5f61 7267 7320 7465 6d70 6c61  arse_args templa
-00000b00: 7465 2066 756e 6374 696f 6e20 7769 7468  te function with
-00000b10: 2073 696e 676c 6520 6172 6775 6d65 6e74   single argument
-00000b20: 206f 6620 7479 7065 203c 7365 743e 0d0a   of type <set>..
-00000b30: 2020 2020 6465 6620 7061 7273 655f 6172      def parse_ar
-00000b40: 6773 2873 656c 662c 2069 6e70 5f73 6574  gs(self, inp_set
-00000b50: 3a20 7365 7420 3d20 7b4e 6f6e 657d 2920  : set = {None}) 
-00000b60: 2d3e 2073 6574 3a0d 0a20 2020 2020 2020  -> set:..       
-00000b70: 2022 2222 0d0a 2020 2020 2020 2020 696e   """..        in
-00000b80: 705f 7365 7420 6973 2076 6172 6961 626c  p_set is variabl
-00000b90: 6520 6f66 2074 7970 6520 3c73 6574 3e0d  e of type <set>.
-00000ba0: 0a20 2020 2020 2020 2061 6e79 2073 6574  .        any set
-00000bb0: 2076 616c 7565 2063 616e 2062 6520 7061   value can be pa
-00000bc0: 7373 6564 2066 6f72 2074 6865 2061 7267  ssed for the arg
-00000bd0: 756d 656e 742c 2077 6869 6c65 2074 6865  ument, while the
-00000be0: 2064 6566 6175 6c74 2069 7320 7b4e 6f6e   default is {Non
-00000bf0: 657d 0d0a 2020 2020 2020 2020 7468 6520  e}..        the 
-00000c00: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
-00000c10: 2074 6865 2073 616d 6520 6172 6720 7661   the same arg va
-00000c20: 6c75 6520 6173 2074 7970 6520 3c73 6574  lue as type <set
-00000c30: 3e20 0d0a 0d0a 2020 2020 2020 2020 636d  > ....        cm
-00000c40: 6473 203a 0d0a 2020 2020 2020 2020 2020  ds :..          
-00000c50: 2020 312e 2070 7974 686f 6e20 3c5f 5f66    1. python <__f
-00000c60: 696c 655f 5f3e 207b 2745 6d70 7479 277d  ile__> {'Empty'}
-00000c70: 0d0a 2020 2020 2020 2020 2020 2020 322e  ..            2.
-00000c80: 2070 7974 686f 6e20 3c5f 5f66 696c 655f   python <__file_
-00000c90: 5f3e 202d 696e 705f 7365 743d 7b27 456d  _> -inp_set={'Em
-00000ca0: 7074 7927 7d0d 0a20 2020 2020 2020 2022  pty'}..        "
-00000cb0: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00000cc0: 726e 2069 6e70 5f73 6574 0d0a 2020 2020  rn inp_set..    
-00000cd0: 0d0a 636c 6173 7320 7369 6e67 6c65 5f64  ..class single_d
-00000ce0: 6963 7428 6172 675f 7061 7273 6572 293a  ict(arg_parser):
-00000cf0: 0d0a 0d0a 2020 2020 2320 6578 616d 706c  ....    # exampl
-00000d00: 6520 7061 7273 655f 6172 6773 2074 656d  e parse_args tem
-00000d10: 706c 6174 6520 6675 6e63 7469 6f6e 2077  plate function w
-00000d20: 6974 6820 7369 6e67 6c65 2061 7267 756d  ith single argum
-00000d30: 656e 7420 6f66 2074 7970 6520 3c64 6963  ent of type <dic
-00000d40: 743e 0d0a 2020 2020 6465 6620 7061 7273  t>..    def pars
-00000d50: 655f 6172 6773 2873 656c 662c 2069 6e70  e_args(self, inp
-00000d60: 5f64 6963 743a 2064 6963 7420 3d20 7b4e  _dict: dict = {N
-00000d70: 6f6e 653a 4e6f 6e65 7d29 202d 3e20 6469  one:None}) -> di
-00000d80: 6374 3a0d 0a20 2020 2020 2020 2022 2222  ct:..        """
-00000d90: 0d0a 2020 2020 2020 2020 696e 705f 6469  ..        inp_di
-00000da0: 6374 2069 7320 7661 7269 6162 6c65 206f  ct is variable o
-00000db0: 6620 7479 7065 203c 6469 6374 3e0d 0a20  f type <dict>.. 
-00000dc0: 2020 2020 2020 2061 6e79 2064 6963 7420         any dict 
-00000dd0: 7661 6c75 6520 6361 6e20 6265 2070 6173  value can be pas
-00000de0: 7365 6420 666f 7220 7468 6520 6172 6775  sed for the argu
-00000df0: 6d65 6e74 2c20 7768 696c 6520 7468 6520  ment, while the 
-00000e00: 6465 6661 756c 7420 6973 207b 4e6f 6e65  default is {None
-00000e10: 3a20 4e6f 6e65 7d0d 0a20 2020 2020 2020  : None}..       
-00000e20: 2074 6865 2066 756e 6374 696f 6e20 7265   the function re
-00000e30: 7475 726e 7320 7468 6520 7361 6d65 2061  turns the same a
-00000e40: 7267 2076 616c 7565 2061 7320 7479 7065  rg value as type
-00000e50: 203c 6469 6374 3e20 0d0a 0d0a 2020 2020   <dict> ....    
-00000e60: 2020 2020 636d 6473 203a 0d0a 2020 2020      cmds :..    
-00000e70: 2020 2020 2020 2020 312e 2070 7974 686f          1. pytho
-00000e80: 6e20 3c5f 5f66 696c 655f 5f3e 207b 2245  n <__file__> {"E
-00000e90: 6d70 7479 223a 2245 6d70 7479 227d 0d0a  mpty":"Empty"}..
-00000ea0: 2020 2020 2020 2020 2020 2020 322e 2070              2. p
-00000eb0: 7974 686f 6e20 3c5f 5f66 696c 655f 5f3e  ython <__file__>
-00000ec0: 202d 696e 705f 6469 6374 3d7b 2245 6d70   -inp_dict={"Emp
-00000ed0: 7479 223a 2245 6d70 7479 227d 0d0a 2020  ty":"Empty"}..  
-00000ee0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00000ef0: 2020 2072 6574 7572 6e20 696e 705f 6469     return inp_di
-00000f00: 6374 0d0a 2020 2020 0d0a 636c 6173 7320  ct..    ..class 
-00000f10: 7369 6e67 6c65 5f62 6f6f 6c28 6172 675f  single_bool(arg_
-00000f20: 7061 7273 6572 293a 0d0a 0d0a 2020 2020  parser):....    
-00000f30: 2320 6578 616d 706c 6520 7061 7273 655f  # example parse_
-00000f40: 6172 6773 2074 656d 706c 6174 6520 6675  args template fu
-00000f50: 6e63 7469 6f6e 2077 6974 6820 7369 6e67  nction with sing
-00000f60: 6c65 2061 7267 756d 656e 7420 6f66 2074  le argument of t
-00000f70: 7970 6520 3c62 6f6f 6c3e 0d0a 2020 2020  ype <bool>..    
-00000f80: 6465 6620 7061 7273 655f 6172 6773 2873  def parse_args(s
-00000f90: 656c 662c 2069 6e70 5f62 6f6f 6c3a 2062  elf, inp_bool: b
-00000fa0: 6f6f 6c20 3d20 4661 6c73 6529 202d 3e20  ool = False) -> 
-00000fb0: 626f 6f6c 3a0d 0a20 2020 2020 2020 2022  bool:..        "
-00000fc0: 2222 0d0a 2020 2020 2020 2020 696e 705f  ""..        inp_
-00000fd0: 626f 6f6c 2069 7320 7661 7269 6162 6c65  bool is variable
-00000fe0: 206f 6620 7479 7065 203c 626f 6f6c 3e0d   of type <bool>.
-00000ff0: 0a20 2020 2020 2020 2061 6e79 2062 6f6f  .        any boo
-00001000: 6c20 7661 6c75 6520 6361 6e20 6265 2070  l value can be p
-00001010: 6173 7365 6420 666f 7220 7468 6520 6172  assed for the ar
-00001020: 6775 6d65 6e74 2c20 7768 696c 6520 7468  gument, while th
-00001030: 6520 6465 6661 756c 7420 6973 2046 616c  e default is Fal
-00001040: 7365 0d0a 2020 2020 2020 2020 7468 6520  se..        the 
-00001050: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
-00001060: 2074 6865 2073 616d 6520 6172 6720 7661   the same arg va
-00001070: 6c75 6520 6173 2074 7970 6520 3c64 6963  lue as type <dic
-00001080: 743e 200d 0a0d 0a20 2020 2020 2020 2063  t> ....        c
-00001090: 6d64 7320 3a0d 0a20 2020 2020 2020 2020  mds :..         
-000010a0: 2020 2031 2e20 7079 7468 6f6e 203c 5f5f     1. python <__
-000010b0: 6669 6c65 5f5f 3e20 5472 7565 0d0a 2020  file__> True..  
-000010c0: 2020 2020 2020 2020 2020 322e 2070 7974            2. pyt
-000010d0: 686f 6e20 3c5f 5f66 696c 655f 5f3e 202d  hon <__file__> -
-000010e0: 696e 705f 626f 6f6c 3d54 7275 650d 0a20  inp_bool=True.. 
-000010f0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00001100: 2020 2020 7265 7475 726e 2069 6e70 5f62      return inp_b
-00001110: 6f6f 6c0d 0a20 2020 200d 0a23 204d 756c  ool..    ..# Mul
-00001120: 7469 706c 6520 6172 6775 6d65 6e74 7320  tiple arguments 
-00001130: 6578 616d 706c 650d 0a0d 0a63 6c61 7373  example....class
-00001140: 206d 756c 7469 5f61 7267 7328 6172 675f   multi_args(arg_
-00001150: 7061 7273 6572 293a 0d0a 0d0a 2020 2020  parser):....    
-00001160: 2320 6578 616d 706c 6520 7061 7273 655f  # example parse_
-00001170: 6172 6773 2074 656d 706c 6174 6520 6675  args template fu
-00001180: 6e63 7469 6f6e 2077 6974 6820 6d75 6c74  nction with mult
-00001190: 6970 6c65 2061 7267 756d 656e 7473 206f  iple arguments o
-000011a0: 6620 6469 6666 6572 656e 7420 7479 7065  f different type
-000011b0: 730d 0a20 2020 2064 6566 2070 6172 7365  s..    def parse
-000011c0: 5f61 7267 7328 7365 6c66 2c20 0d0a 2020  _args(self, ..  
-000011d0: 2020 2020 2020 2020 2020 696e 705f 696e            inp_in
-000011e0: 743a 2069 6e74 203d 2036 2c0d 0a20 2020  t: int = 6,..   
-000011f0: 2020 2020 2020 2020 2069 6e70 5f66 6c6f           inp_flo
-00001200: 6174 3a20 666c 6f61 7420 3d20 362e 302c  at: float = 6.0,
-00001210: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00001220: 705f 7374 723a 2073 7472 203d 2022 5369  p_str: str = "Si
-00001230: 7822 2c0d 0a20 2020 2020 2020 2020 2020  x",..           
-00001240: 2069 6e70 5f6c 6973 743a 206c 6973 7420   inp_list: list 
-00001250: 3d20 5b36 2c20 362e 302c 2022 5369 7822  = [6, 6.0, "Six"
-00001260: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00001270: 696e 705f 7475 706c 653a 2074 7570 6c65  inp_tuple: tuple
-00001280: 203d 2028 362c 2036 2e30 2c20 2253 6978   = (6, 6.0, "Six
-00001290: 2229 2c0d 0a20 2020 2020 2020 2020 2020  "),..           
-000012a0: 2069 6e70 5f73 6574 3a20 7365 7420 3d20   inp_set: set = 
-000012b0: 7b22 5369 7822 7d2c 0d0a 2020 2020 2020  {"Six"},..      
-000012c0: 2020 2020 2020 696e 705f 6469 6374 3a20        inp_dict: 
-000012d0: 6469 6374 203d 207b 2769 6e74 273a 2036  dict = {'int': 6
-000012e0: 2c20 2766 6c6f 6174 273a 2036 2e30 2c20  , 'float': 6.0, 
-000012f0: 2773 7472 273a 2022 5369 7822 7d2c 0d0a  'str': "Six"},..
-00001300: 2020 2020 2020 2020 2020 2020 696e 705f              inp_
-00001310: 626f 6f6c 3a20 626f 6f6c 203d 2046 616c  bool: bool = Fal
-00001320: 7365 2920 2d3e 2064 6963 743a 0d0a 2020  se) -> dict:..  
-00001330: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00001340: 2020 2053 6576 656e 2061 7267 756d 656e     Seven argumen
-00001350: 7473 206f 6620 6469 6666 6572 656e 7420  ts of different 
-00001360: 6461 7461 2074 7970 6520 6361 6e20 6265  data type can be
-00001370: 2070 6173 7365 640d 0a20 2020 2020 2020   passed..       
-00001380: 2061 6e79 2076 616c 7565 206f 6620 7468   any value of th
-00001390: 6520 7265 7370 6563 7469 7665 2064 6174  e respective dat
-000013a0: 6120 7479 7065 2063 616e 2062 6520 7061  a type can be pa
-000013b0: 7373 6564 2066 6f72 2073 7065 6369 6669  ssed for specifi
-000013c0: 6320 6172 6775 6d65 6e74 2e20 666f 7220  c argument. for 
-000013d0: 6465 6661 756c 7473 2072 6566 6572 2061  defaults refer a
-000013e0: 626f 7665 0d0a 2020 2020 2020 2020 7468  bove..        th
-000013f0: 6520 6675 6e63 7469 6f6e 2072 6574 7572  e function retur
-00001400: 6e73 2061 206a 736f 6e20 7374 7269 6e67  ns a json string
-00001410: 2063 6f6e 7461 696e 696e 6720 616c 6c20   containing all 
-00001420: 7468 6520 6172 6775 6d65 6e74 7320 616e  the arguments an
-00001430: 6420 6974 7320 7661 6c75 6573 2e0d 0a0d  d its values....
-00001440: 0a20 2020 2020 2020 2063 6d64 7320 3a0d  .        cmds :.
-00001450: 0a20 2020 2020 2020 2020 2020 2031 2e20  .            1. 
-00001460: 7079 7468 6f6e 203c 5f5f 6669 6c65 5f5f  python <__file__
-00001470: 3e20 3130 2031 302e 3020 5365 7665 6e20  > 10 10.0 Seven 
-00001480: 5b31 302c 3130 2e30 2c27 5365 7665 6e27  [10,10.0,'Seven'
-00001490: 5d20 2831 302c 3130 2e30 2c27 5365 7665  ] (10,10.0,'Seve
-000014a0: 6e27 2920 7b31 302c 3130 2e30 2c27 5365  n') {10,10.0,'Se
-000014b0: 7665 6e27 7d20 7b27 696e 7427 3a31 302c  ven'} {'int':10,
-000014c0: 2766 6c6f 6174 273a 3130 2e30 2c27 7374  'float':10.0,'st
-000014d0: 7227 3a27 5365 7665 6e27 7d20 5472 7565  r':'Seven'} True
-000014e0: 0d0a 2020 2020 2020 2020 2020 2020 322e  ..            2.
-000014f0: 2070 7974 686f 6e20 3c5f 5f66 696c 655f   python <__file_
-00001500: 5f3e 202d 696e 705f 696e 743d 3130 202d  _> -inp_int=10 -
-00001510: 696e 705f 666c 6f61 743d 3130 2e30 202d  inp_float=10.0 -
-00001520: 696e 705f 7374 723d 5365 7665 6e20 2d69  inp_str=Seven -i
-00001530: 6e70 5f6c 6973 743d 5b31 302c 3130 2e30  np_list=[10,10.0
-00001540: 2c27 5365 7665 6e27 5d20 2d69 6e70 5f74  ,'Seven'] -inp_t
-00001550: 7570 6c65 3d28 3130 2c31 302e 302c 2753  uple=(10,10.0,'S
-00001560: 6576 656e 2729 202d 696e 705f 7365 743d  even') -inp_set=
-00001570: 7b31 302c 3130 2e30 2c27 5365 7665 6e27  {10,10.0,'Seven'
-00001580: 7d20 2d69 6e70 5f64 6963 743d 7b27 696e  } -inp_dict={'in
-00001590: 7427 3a31 302c 2766 6c6f 6174 273a 3130  t':10,'float':10
-000015a0: 2e30 2c27 7374 7227 3a27 5365 7665 6e27  .0,'str':'Seven'
-000015b0: 7d20 2d69 6e70 5f62 6f6f 6c3d 5472 7565  } -inp_bool=True
-000015c0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000015d0: 2020 2020 2020 2072 6574 7572 6e20 7b0d         return {.
-000015e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000015f0: 2027 696e 705f 696e 7427 3a20 696e 705f   'inp_int': inp_
-00001600: 696e 742c 0d0a 2020 2020 2020 2020 2020  int,..          
-00001610: 2020 2020 2020 2769 6e70 5f66 6c6f 6174        'inp_float
-00001620: 273a 2069 6e70 5f66 6c6f 6174 2c0d 0a20  ': inp_float,.. 
-00001630: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001640: 696e 705f 7374 7227 3a20 696e 705f 7374  inp_str': inp_st
-00001650: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-00001660: 2020 2020 2769 6e70 5f6c 6973 7427 3a20      'inp_list': 
-00001670: 696e 705f 6c69 7374 2c0d 0a20 2020 2020  inp_list,..     
-00001680: 2020 2020 2020 2020 2020 2027 696e 705f             'inp_
-00001690: 7475 706c 6527 3a20 696e 705f 7475 706c  tuple': inp_tupl
-000016a0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-000016b0: 2020 2020 2769 6e70 5f73 6574 273a 2069      'inp_set': i
-000016c0: 6e70 5f73 6574 2c0d 0a20 2020 2020 2020  np_set,..       
-000016d0: 2020 2020 2020 2020 2027 696e 705f 6469           'inp_di
-000016e0: 6374 273a 2069 6e70 5f64 6963 742c 0d0a  ct': inp_dict,..
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001700: 2769 6e70 5f62 6f6f 6c27 3a20 696e 705f  'inp_bool': inp_
-00001710: 626f 6f6c 0d0a 2020 2020 2020 2020 2020  bool..          
-00001720: 2020 7d0d 0a20 2020 2020 2020 20           }..        
+00000000: 0d0a 696d 706f 7274 2070 616e 6461 7320  ..import pandas 
+00000010: 6173 2070 640d 0a66 726f 6d20 7079 3463  as pd..from py4c
+00000020: 6c69 2e6d 696e 696d 616c 2069 6d70 6f72  li.minimal impor
+00000030: 7420 6172 675f 7061 7273 6572 0d0a 0d0a  t arg_parser....
+00000040: 2320 5369 6e67 6c65 2061 7267 756d 656e  # Single argumen
+00000050: 7420 6578 616d 706c 6573 0d0a 0d0a 636c  t examples....cl
+00000060: 6173 7320 7369 6e67 6c65 5f69 6e74 2861  ass single_int(a
+00000070: 7267 5f70 6172 7365 7229 3a0d 0a0d 0a20  rg_parser):.... 
+00000080: 2020 2023 2065 7861 6d70 6c65 2070 6172     # example par
+00000090: 7365 5f61 7267 7320 7465 6d70 6c61 7465  se_args template
+000000a0: 2066 756e 6374 696f 6e20 7769 7468 2073   function with s
+000000b0: 696e 676c 6520 6172 6775 6d65 6e74 206f  ingle argument o
+000000c0: 6620 7479 7065 203c 696e 743e 0d0a 2020  f type <int>..  
+000000d0: 2020 6465 6620 7061 7273 655f 6172 6773    def parse_args
+000000e0: 2873 656c 662c 2069 6e70 5f69 6e74 3a20  (self, inp_int: 
+000000f0: 696e 7420 3d20 3029 202d 3e20 696e 743a  int = 0) -> int:
+00000100: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00000110: 2020 2020 2020 2069 6e70 5f69 6e74 2069         inp_int i
+00000120: 7320 7661 7269 6162 6c65 206f 6620 7479  s variable of ty
+00000130: 7065 203c 696e 743e 0d0a 2020 2020 2020  pe <int>..      
+00000140: 2020 616e 7920 696e 7465 6765 7220 7661    any integer va
+00000150: 6c75 6520 6361 6e20 6265 2070 6173 7365  lue can be passe
+00000160: 6420 666f 7220 7468 6520 6172 6775 6d65  d for the argume
+00000170: 6e74 2c20 7768 696c 6520 7468 6520 6465  nt, while the de
+00000180: 6661 756c 7420 6973 2030 0d0a 2020 2020  fault is 0..    
+00000190: 2020 2020 7468 6520 6675 6e63 7469 6f6e      the function
+000001a0: 2072 6574 7572 6e73 2074 6865 2073 616d   returns the sam
+000001b0: 6520 6172 6720 7661 6c75 6520 6173 2074  e arg value as t
+000001c0: 7970 6520 3c69 6e74 3e20 0d0a 0d0a 2020  ype <int> ....  
+000001d0: 2020 2020 2020 636d 6473 203a 0d0a 2020        cmds :..  
+000001e0: 2020 2020 2020 2020 2020 312e 2070 7974            1. pyt
+000001f0: 686f 6e20 3c5f 5f66 696c 655f 5f3e 2031  hon <__file__> 1
+00000200: 300d 0a20 2020 2020 2020 2020 2020 2032  0..            2
+00000210: 2e20 7079 7468 6f6e 203c 5f5f 6669 6c65  . python <__file
+00000220: 5f5f 3e20 2d69 6e70 5f69 6e74 3d31 300d  __> -inp_int=10.
+00000230: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00000240: 2020 2020 2020 7265 7475 726e 2069 6e70        return inp
+00000250: 5f69 6e74 0d0a 2020 2020 0d0a 636c 6173  _int..    ..clas
+00000260: 7320 7369 6e67 6c65 5f66 6c6f 6174 2861  s single_float(a
+00000270: 7267 5f70 6172 7365 7229 3a0d 0a0d 0a20  rg_parser):.... 
+00000280: 2020 2023 2065 7861 6d70 6c65 2070 6172     # example par
+00000290: 7365 5f61 7267 7320 7465 6d70 6c61 7465  se_args template
+000002a0: 2066 756e 6374 696f 6e20 7769 7468 2073   function with s
+000002b0: 696e 676c 6520 6172 6775 6d65 6e74 206f  ingle argument o
+000002c0: 6620 7479 7065 203c 666c 6f61 743e 0d0a  f type <float>..
+000002d0: 2020 2020 6465 6620 7061 7273 655f 6172      def parse_ar
+000002e0: 6773 2873 656c 662c 2069 6e70 5f66 6c6f  gs(self, inp_flo
+000002f0: 6174 3a20 666c 6f61 7420 3d20 302e 3029  at: float = 0.0)
+00000300: 202d 3e20 666c 6f61 743a 0d0a 2020 2020   -> float:..    
+00000310: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00000320: 2069 6e70 5f66 6c6f 6174 2069 7320 7661   inp_float is va
+00000330: 7269 6162 6c65 206f 6620 7479 7065 203c  riable of type <
+00000340: 666c 6f61 743e 0d0a 2020 2020 2020 2020  float>..        
+00000350: 616e 7920 666c 6f61 7469 6e67 2070 6f69  any floating poi
+00000360: 6e74 2076 616c 7565 2063 616e 2062 6520  nt value can be 
+00000370: 7061 7373 6564 2066 6f72 2074 6865 2061  passed for the a
+00000380: 7267 756d 656e 742c 2077 6869 6c65 2074  rgument, while t
+00000390: 6865 2064 6566 6175 6c74 2069 7320 302e  he default is 0.
+000003a0: 300d 0a20 2020 2020 2020 2074 6865 2066  0..        the f
+000003b0: 756e 6374 696f 6e20 7265 7475 726e 7320  unction returns 
+000003c0: 7468 6520 7361 6d65 2061 7267 2076 616c  the same arg val
+000003d0: 7565 2061 7320 7479 7065 203c 666c 6f61  ue as type <floa
+000003e0: 743e 200d 0a0d 0a20 2020 2020 2020 2063  t> ....        c
+000003f0: 6d64 7320 3a0d 0a20 2020 2020 2020 2020  mds :..         
+00000400: 2020 2031 2e20 7079 7468 6f6e 203c 5f5f     1. python <__
+00000410: 6669 6c65 5f5f 3e20 3130 2e30 0d0a 2020  file__> 10.0..  
+00000420: 2020 2020 2020 2020 2020 322e 2070 7974            2. pyt
+00000430: 686f 6e20 3c5f 5f66 696c 655f 5f3e 202d  hon <__file__> -
+00000440: 696e 705f 666c 6f61 743d 3130 2e30 0d0a  inp_float=10.0..
+00000450: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00000460: 2020 2020 2072 6574 7572 6e20 696e 705f       return inp_
+00000470: 666c 6f61 740d 0a20 2020 200d 0a63 6c61  float..    ..cla
+00000480: 7373 2073 696e 676c 655f 7374 7228 6172  ss single_str(ar
+00000490: 675f 7061 7273 6572 293a 0d0a 0d0a 2020  g_parser):....  
+000004a0: 2020 2320 6578 616d 706c 6520 7061 7273    # example pars
+000004b0: 655f 6172 6773 2074 656d 706c 6174 6520  e_args template 
+000004c0: 6675 6e63 7469 6f6e 2077 6974 6820 7369  function with si
+000004d0: 6e67 6c65 2061 7267 756d 656e 7420 6f66  ngle argument of
+000004e0: 2074 7970 6520 3c73 7472 3e0d 0a20 2020   type <str>..   
+000004f0: 2064 6566 2070 6172 7365 5f61 7267 7328   def parse_args(
+00000500: 7365 6c66 2c20 696e 705f 7374 723a 2073  self, inp_str: s
+00000510: 7472 203d 2022 4e6f 6e65 2229 202d 3e20  tr = "None") -> 
+00000520: 7374 723a 0d0a 2020 2020 2020 2020 2222  str:..        ""
+00000530: 220d 0a20 2020 2020 2020 2069 6e70 5f73  "..        inp_s
+00000540: 7472 2069 7320 7661 7269 6162 6c65 206f  tr is variable o
+00000550: 6620 7479 7065 203c 7374 723e 0d0a 2020  f type <str>..  
+00000560: 2020 2020 2020 616e 7920 7374 7269 6e67        any string
+00000570: 2076 616c 7565 2063 616e 2062 6520 7061   value can be pa
+00000580: 7373 6564 2066 6f72 2074 6865 2061 7267  ssed for the arg
+00000590: 756d 656e 742c 2077 6869 6c65 2074 6865  ument, while the
+000005a0: 2064 6566 6175 6c74 2069 7320 224e 6f6e   default is "Non
+000005b0: 6522 0d0a 2020 2020 2020 2020 7468 6520  e"..        the 
+000005c0: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
+000005d0: 2074 6865 2073 616d 6520 6172 6720 7661   the same arg va
+000005e0: 6c75 6520 6173 2074 7970 6520 3c73 7472  lue as type <str
+000005f0: 3e20 0d0a 0d0a 2020 2020 2020 2020 636d  > ....        cm
+00000600: 6473 203a 0d0a 2020 2020 2020 2020 2020  ds :..          
+00000610: 2020 312e 2070 7974 686f 6e20 3c5f 5f66    1. python <__f
+00000620: 696c 655f 5f3e 2045 6d70 7479 0d0a 2020  ile__> Empty..  
+00000630: 2020 2020 2020 2020 2020 322e 2070 7974            2. pyt
+00000640: 686f 6e20 3c5f 5f66 696c 655f 5f3e 202d  hon <__file__> -
+00000650: 696e 705f 7374 723d 456d 7074 790d 0a20  inp_str=Empty.. 
+00000660: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00000670: 2020 2020 7265 7475 726e 2069 6e70 5f73      return inp_s
+00000680: 7472 0d0a 2020 2020 0d0a 636c 6173 7320  tr..    ..class 
+00000690: 7369 6e67 6c65 5f6c 6973 7428 6172 675f  single_list(arg_
+000006a0: 7061 7273 6572 293a 0d0a 0d0a 2020 2020  parser):....    
+000006b0: 2320 6578 616d 706c 6520 7061 7273 655f  # example parse_
+000006c0: 6172 6773 2074 656d 706c 6174 6520 6675  args template fu
+000006d0: 6e63 7469 6f6e 2077 6974 6820 7369 6e67  nction with sing
+000006e0: 6c65 2061 7267 756d 656e 7420 6f66 2074  le argument of t
+000006f0: 7970 6520 3c6c 6973 743e 0d0a 2020 2020  ype <list>..    
+00000700: 6465 6620 7061 7273 655f 6172 6773 2873  def parse_args(s
+00000710: 656c 662c 2069 6e70 5f6c 6973 743a 206c  elf, inp_list: l
+00000720: 6973 7420 3d20 5b4e 6f6e 655d 2920 2d3e  ist = [None]) ->
+00000730: 206c 6973 743a 0d0a 2020 2020 2020 2020   list:..        
+00000740: 2222 220d 0a20 2020 2020 2020 2069 6e70  """..        inp
+00000750: 5f6c 6973 7420 6973 2076 6172 6961 626c  _list is variabl
+00000760: 6520 6f66 2074 7970 6520 3c6c 6973 743e  e of type <list>
+00000770: 0d0a 2020 2020 2020 2020 616e 7920 6c69  ..        any li
+00000780: 7374 2076 616c 7565 2063 616e 2062 6520  st value can be 
+00000790: 7061 7373 6564 2066 6f72 2074 6865 2061  passed for the a
+000007a0: 7267 756d 656e 742c 2077 6869 6c65 2074  rgument, while t
+000007b0: 6865 2064 6566 6175 6c74 2069 7320 5b4e  he default is [N
+000007c0: 6f6e 655d 0d0a 2020 2020 2020 2020 7468  one]..        th
+000007d0: 6520 6675 6e63 7469 6f6e 2072 6574 7572  e function retur
+000007e0: 6e73 2074 6865 2073 616d 6520 6172 6720  ns the same arg 
+000007f0: 7661 6c75 6520 6173 2074 7970 6520 3c6c  value as type <l
+00000800: 6973 743e 200d 0a0d 0a20 2020 2020 2020  ist> ....       
+00000810: 2063 6d64 7320 3a0d 0a20 2020 2020 2020   cmds :..       
+00000820: 2020 2020 2031 2e20 7079 7468 6f6e 203c       1. python <
+00000830: 5f5f 6669 6c65 5f5f 3e20 5b22 456d 7074  __file__> ["Empt
+00000840: 7922 5d0d 0a20 2020 2020 2020 2020 2020  y"]..           
+00000850: 2032 2e20 7079 7468 6f6e 203c 5f5f 6669   2. python <__fi
+00000860: 6c65 5f5f 3e20 2d69 6e70 5f6c 6973 743d  le__> -inp_list=
+00000870: 5b22 456d 7074 7922 5d0d 0a20 2020 2020  ["Empty"]..     
+00000880: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00000890: 7265 7475 726e 2069 6e70 5f6c 6973 740d  return inp_list.
+000008a0: 0a20 2020 200d 0a63 6c61 7373 2073 696e  .    ..class sin
+000008b0: 676c 655f 6469 6374 2861 7267 5f70 6172  gle_dict(arg_par
+000008c0: 7365 7229 3a0d 0a0d 0a20 2020 2023 2065  ser):....    # e
+000008d0: 7861 6d70 6c65 2070 6172 7365 5f61 7267  xample parse_arg
+000008e0: 7320 7465 6d70 6c61 7465 2066 756e 6374  s template funct
+000008f0: 696f 6e20 7769 7468 2073 696e 676c 6520  ion with single 
+00000900: 6172 6775 6d65 6e74 206f 6620 7479 7065  argument of type
+00000910: 203c 6469 6374 3e0d 0a20 2020 2064 6566   <dict>..    def
+00000920: 2070 6172 7365 5f61 7267 7328 7365 6c66   parse_args(self
+00000930: 2c20 696e 705f 6469 6374 3a20 6469 6374  , inp_dict: dict
+00000940: 203d 207b 4e6f 6e65 3a4e 6f6e 657d 2920   = {None:None}) 
+00000950: 2d3e 2064 6963 743a 0d0a 2020 2020 2020  -> dict:..      
+00000960: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
+00000970: 6e70 5f64 6963 7420 6973 2076 6172 6961  np_dict is varia
+00000980: 626c 6520 6f66 2074 7970 6520 3c64 6963  ble of type <dic
+00000990: 743e 0d0a 2020 2020 2020 2020 616e 7920  t>..        any 
+000009a0: 6469 6374 2076 616c 7565 2063 616e 2062  dict value can b
+000009b0: 6520 7061 7373 6564 2066 6f72 2074 6865  e passed for the
+000009c0: 2061 7267 756d 656e 742c 2077 6869 6c65   argument, while
+000009d0: 2074 6865 2064 6566 6175 6c74 2069 7320   the default is 
+000009e0: 7b4e 6f6e 653a 204e 6f6e 657d 0d0a 2020  {None: None}..  
+000009f0: 2020 2020 2020 7468 6520 6675 6e63 7469        the functi
+00000a00: 6f6e 2072 6574 7572 6e73 2074 6865 2073  on returns the s
+00000a10: 616d 6520 6172 6720 7661 6c75 6520 6173  ame arg value as
+00000a20: 2074 7970 6520 3c64 6963 743e 200d 0a0d   type <dict> ...
+00000a30: 0a20 2020 2020 2020 2063 6d64 7320 3a0d  .        cmds :.
+00000a40: 0a20 2020 2020 2020 2020 2020 2031 2e20  .            1. 
+00000a50: 7079 7468 6f6e 203c 5f5f 6669 6c65 5f5f  python <__file__
+00000a60: 3e20 7b22 456d 7074 7922 3a22 456d 7074  > {"Empty":"Empt
+00000a70: 7922 7d0d 0a20 2020 2020 2020 2020 2020  y"}..           
+00000a80: 2032 2e20 7079 7468 6f6e 203c 5f5f 6669   2. python <__fi
+00000a90: 6c65 5f5f 3e20 2d69 6e70 5f64 6963 743d  le__> -inp_dict=
+00000aa0: 7b22 456d 7074 7922 3a22 456d 7074 7922  {"Empty":"Empty"
+00000ab0: 7d0d 0a20 2020 2020 2020 2022 2222 0d0a  }..        """..
+00000ac0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00000ad0: 6e70 5f64 6963 740d 0a20 2020 200d 0a63  np_dict..    ..c
+00000ae0: 6c61 7373 2073 696e 676c 655f 626f 6f6c  lass single_bool
+00000af0: 2861 7267 5f70 6172 7365 7229 3a0d 0a0d  (arg_parser):...
+00000b00: 0a20 2020 2023 2065 7861 6d70 6c65 2070  .    # example p
+00000b10: 6172 7365 5f61 7267 7320 7465 6d70 6c61  arse_args templa
+00000b20: 7465 2066 756e 6374 696f 6e20 7769 7468  te function with
+00000b30: 2073 696e 676c 6520 6172 6775 6d65 6e74   single argument
+00000b40: 206f 6620 7479 7065 203c 626f 6f6c 3e0d   of type <bool>.
+00000b50: 0a20 2020 2064 6566 2070 6172 7365 5f61  .    def parse_a
+00000b60: 7267 7328 7365 6c66 2c20 696e 705f 626f  rgs(self, inp_bo
+00000b70: 6f6c 3a20 626f 6f6c 203d 2046 616c 7365  ol: bool = False
+00000b80: 2920 2d3e 2062 6f6f 6c3a 0d0a 2020 2020  ) -> bool:..    
+00000b90: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00000ba0: 2069 6e70 5f62 6f6f 6c20 6973 2076 6172   inp_bool is var
+00000bb0: 6961 626c 6520 6f66 2074 7970 6520 3c62  iable of type <b
+00000bc0: 6f6f 6c3e 0d0a 2020 2020 2020 2020 616e  ool>..        an
+00000bd0: 7920 626f 6f6c 2076 616c 7565 2063 616e  y bool value can
+00000be0: 2062 6520 7061 7373 6564 2066 6f72 2074   be passed for t
+00000bf0: 6865 2061 7267 756d 656e 742c 2077 6869  he argument, whi
+00000c00: 6c65 2074 6865 2064 6566 6175 6c74 2069  le the default i
+00000c10: 7320 4661 6c73 650d 0a20 2020 2020 2020  s False..       
+00000c20: 2074 6865 2066 756e 6374 696f 6e20 7265   the function re
+00000c30: 7475 726e 7320 7468 6520 7361 6d65 2061  turns the same a
+00000c40: 7267 2076 616c 7565 2061 7320 7479 7065  rg value as type
+00000c50: 203c 626f 6f6c 3e20 0d0a 0d0a 2020 2020   <bool> ....    
+00000c60: 2020 2020 636d 6473 203a 0d0a 2020 2020      cmds :..    
+00000c70: 2020 2020 2020 2020 312e 2070 7974 686f          1. pytho
+00000c80: 6e20 3c5f 5f66 696c 655f 5f3e 2054 7275  n <__file__> Tru
+00000c90: 650d 0a20 2020 2020 2020 2020 2020 2032  e..            2
+00000ca0: 2e20 7079 7468 6f6e 203c 5f5f 6669 6c65  . python <__file
+00000cb0: 5f5f 3e20 2d69 6e70 5f62 6f6f 6c3d 5472  __> -inp_bool=Tr
+00000cc0: 7565 0d0a 2020 2020 2020 2020 2222 220d  ue..        """.
+00000cd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000ce0: 696e 705f 626f 6f6c 0d0a 2020 2020 0d0a  inp_bool..    ..
+00000cf0: 2320 4d75 6c74 6970 6c65 2061 7267 756d  # Multiple argum
+00000d00: 656e 7473 2065 7861 6d70 6c65 0d0a 0d0a  ents example....
+00000d10: 636c 6173 7320 6d75 6c74 695f 6172 6773  class multi_args
+00000d20: 2861 7267 5f70 6172 7365 7229 3a0d 0a0d  (arg_parser):...
+00000d30: 0a20 2020 2023 2065 7861 6d70 6c65 2070  .    # example p
+00000d40: 6172 7365 5f61 7267 7320 7465 6d70 6c61  arse_args templa
+00000d50: 7465 2066 756e 6374 696f 6e20 7769 7468  te function with
+00000d60: 206d 756c 7469 706c 6520 6172 6775 6d65   multiple argume
+00000d70: 6e74 7320 6f66 2064 6966 6665 7265 6e74  nts of different
+00000d80: 2074 7970 6573 0d0a 2020 2020 6465 6620   types..    def 
+00000d90: 7061 7273 655f 6172 6773 2873 656c 662c  parse_args(self,
+00000da0: 200d 0a20 2020 2020 2020 2020 2020 2069   ..            i
+00000db0: 6e70 5f69 6e74 3a20 696e 7420 3d20 362c  np_int: int = 6,
+00000dc0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00000dd0: 705f 666c 6f61 743a 2066 6c6f 6174 203d  p_float: float =
+00000de0: 2036 2e30 2c0d 0a20 2020 2020 2020 2020   6.0,..         
+00000df0: 2020 2069 6e70 5f73 7472 3a20 7374 7220     inp_str: str 
+00000e00: 3d20 2253 6978 222c 0d0a 2020 2020 2020  = "Six",..      
+00000e10: 2020 2020 2020 696e 705f 6c69 7374 3a20        inp_list: 
+00000e20: 6c69 7374 203d 205b 362c 2036 2e30 2c20  list = [6, 6.0, 
+00000e30: 2253 6978 225d 2c0d 0a20 2020 2020 2020  "Six"],..       
+00000e40: 2020 2020 2069 6e70 5f64 6963 743a 2064       inp_dict: d
+00000e50: 6963 7420 3d20 7b27 696e 7427 3a20 362c  ict = {'int': 6,
+00000e60: 2027 666c 6f61 7427 3a20 362e 302c 2027   'float': 6.0, '
+00000e70: 7374 7227 3a20 2253 6978 227d 2c0d 0a20  str': "Six"},.. 
+00000e80: 2020 2020 2020 2020 2020 2069 6e70 5f62             inp_b
+00000e90: 6f6f 6c3a 2062 6f6f 6c20 3d20 4661 6c73  ool: bool = Fals
+00000ea0: 6529 202d 3e20 6469 6374 3a0d 0a20 2020  e) -> dict:..   
+00000eb0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00000ec0: 2020 5369 7820 6172 6775 6d65 6e74 7320    Six arguments 
+00000ed0: 6f66 2064 6966 6665 7265 6e74 2064 6174  of different dat
+00000ee0: 6120 7479 7065 2063 616e 2062 6520 7061  a type can be pa
+00000ef0: 7373 6564 0d0a 2020 2020 2020 2020 616e  ssed..        an
+00000f00: 7920 7661 6c75 6520 6f66 2074 6865 2072  y value of the r
+00000f10: 6573 7065 6374 6976 6520 6461 7461 2074  espective data t
+00000f20: 7970 6520 6361 6e20 6265 2070 6173 7365  ype can be passe
+00000f30: 6420 666f 7220 7370 6563 6966 6963 2061  d for specific a
+00000f40: 7267 756d 656e 742e 2066 6f72 2064 6566  rgument. for def
+00000f50: 6175 6c74 7320 7265 6665 7220 6162 6f76  aults refer abov
+00000f60: 650d 0a20 2020 2020 2020 2074 6865 2066  e..        the f
+00000f70: 756e 6374 696f 6e20 7265 7475 726e 7320  unction returns 
+00000f80: 6120 6469 6374 2063 6f6e 7461 696e 696e  a dict containin
+00000f90: 6720 616c 6c20 7468 6520 6172 6775 6d65  g all the argume
+00000fa0: 6e74 7320 616e 6420 6974 7320 7661 6c75  nts and its valu
+00000fb0: 6573 2e0d 0a0d 0a20 2020 2020 2020 2063  es.....        c
+00000fc0: 6d64 7320 3a0d 0a20 2020 2020 2020 2020  mds :..         
+00000fd0: 2020 2031 2e20 7079 7468 6f6e 203c 5f5f     1. python <__
+00000fe0: 6669 6c65 5f5f 3e20 3130 2031 302e 3020  file__> 10 10.0 
+00000ff0: 5365 7665 6e20 5b31 302c 3130 2e30 2c27  Seven [10,10.0,'
+00001000: 5365 7665 6e27 5d20 7b27 696e 7427 3a31  Seven'] {'int':1
+00001010: 302c 2766 6c6f 6174 273a 3130 2e30 2c27  0,'float':10.0,'
+00001020: 7374 7227 3a27 5365 7665 6e27 7d20 5472  str':'Seven'} Tr
+00001030: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+00001040: 322e 2070 7974 686f 6e20 3c5f 5f66 696c  2. python <__fil
+00001050: 655f 5f3e 202d 696e 705f 696e 743d 3130  e__> -inp_int=10
+00001060: 202d 696e 705f 666c 6f61 743d 3130 2e30   -inp_float=10.0
+00001070: 202d 696e 705f 7374 723d 5365 7665 6e20   -inp_str=Seven 
+00001080: 2d69 6e70 5f6c 6973 743d 5b31 302c 3130  -inp_list=[10,10
+00001090: 2e30 2c27 5365 7665 6e27 5d20 2d69 6e70  .0,'Seven'] -inp
+000010a0: 5f64 6963 743d 7b27 696e 7427 3a31 302c  _dict={'int':10,
+000010b0: 2766 6c6f 6174 273a 3130 2e30 2c27 7374  'float':10.0,'st
+000010c0: 7227 3a27 5365 7665 6e27 7d20 2d69 6e70  r':'Seven'} -inp
+000010d0: 5f62 6f6f 6c3d 5472 7565 0d0a 2020 2020  _bool=True..    
+000010e0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000010f0: 2072 6574 7572 6e20 7b0d 0a20 2020 2020   return {..     
+00001100: 2020 2020 2020 2020 2020 2027 696e 705f             'inp_
+00001110: 696e 7427 3a20 696e 705f 696e 742c 0d0a  int': inp_int,..
+00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001130: 2769 6e70 5f66 6c6f 6174 273a 2069 6e70  'inp_float': inp
+00001140: 5f66 6c6f 6174 2c0d 0a20 2020 2020 2020  _float,..       
+00001150: 2020 2020 2020 2020 2027 696e 705f 7374           'inp_st
+00001160: 7227 3a20 696e 705f 7374 722c 0d0a 2020  r': inp_str,..  
+00001170: 2020 2020 2020 2020 2020 2020 2020 2769                'i
+00001180: 6e70 5f6c 6973 7427 3a20 696e 705f 6c69  np_list': inp_li
+00001190: 7374 2c0d 0a20 2020 2020 2020 2020 2020  st,..           
+000011a0: 2020 2020 2027 696e 705f 6469 6374 273a       'inp_dict':
+000011b0: 2069 6e70 5f64 6963 742c 0d0a 2020 2020   inp_dict,..    
+000011c0: 2020 2020 2020 2020 2020 2020 2769 6e70              'inp
+000011d0: 5f62 6f6f 6c27 3a20 696e 705f 626f 6f6c  _bool': inp_bool
+000011e0: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
+000011f0: 0a20 2020 2020 2020 200d 0a23 2057 6172  .        ..# War
+00001200: 6e69 6e67 7320 6368 6563 6b0d 0a0d 0a63  nings check....c
+00001210: 6c61 7373 2077 6172 6e5f 7265 745f 7479  lass warn_ret_ty
+00001220: 7065 2861 7267 5f70 6172 7365 7229 3a0d  pe(arg_parser):.
+00001230: 0a0d 0a20 2020 2023 2065 7861 6d70 6c65  ...    # example
+00001240: 2070 6172 7365 5f61 7267 7320 7465 6d70   parse_args temp
+00001250: 6c61 7465 2066 756e 6374 696f 6e20 666f  late function fo
+00001260: 7220 7465 7374 696e 6720 6966 2077 6172  r testing if war
+00001270: 6e69 6e67 2069 7320 6765 7474 696e 6720  ning is getting 
+00001280: 7072 696e 7465 642e 0d0a 2020 2020 2320  printed...    # 
+00001290: 7265 7475 726e 2074 7970 6520 7761 726e  return type warn
+000012a0: 696e 6720 7769 6c6c 2062 6520 7072 696e  ing will be prin
+000012b0: 7465 6420 6966 2074 6865 7265 2069 7320  ted if there is 
+000012c0: 6120 6d69 736d 6174 6368 2062 6574 7765  a mismatch betwe
+000012d0: 656e 2065 7870 6563 7465 6420 6474 7970  en expected dtyp
+000012e0: 6520 616e 6420 7265 7475 726e 6564 2064  e and returned d
+000012f0: 7479 7065 2e0d 0a20 2020 2023 2077 6172  type...    # war
+00001300: 6e69 6e67 2077 696c 6c20 6f6e 6c79 2062  ning will only b
+00001310: 6520 7072 696e 7465 6420 616e 6420 7769  e printed and wi
+00001320: 6c6c 206e 6f74 2068 616c 7420 7468 6520  ll not halt the 
+00001330: 6578 6563 7574 696f 6e20 666c 6f77 2e0d  execution flow..
+00001340: 0a20 2020 2064 6566 2070 6172 7365 5f61  .    def parse_a
+00001350: 7267 7328 7365 6c66 2c20 0d0a 2020 2020  rgs(self, ..    
+00001360: 2020 2020 2020 2020 696e 705f 696e 743a          inp_int:
+00001370: 2069 6e74 203d 2030 2920 2d3e 2073 7472   int = 0) -> str
+00001380: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00001390: 2020 2020 2020 2020 696e 705f 696e 7420          inp_int 
+000013a0: 6973 2076 6172 6961 626c 6520 6f66 2074  is variable of t
+000013b0: 7970 6520 3c69 6e74 3e0d 0a20 2020 2020  ype <int>..     
+000013c0: 2020 2061 6e79 2069 6e74 2076 616c 7565     any int value
+000013d0: 2063 616e 2062 6520 7061 7373 6564 2066   can be passed f
+000013e0: 6f72 2074 6865 2061 7267 756d 656e 742c  or the argument,
+000013f0: 2077 6869 6c65 2074 6865 2064 6566 6175   while the defau
+00001400: 6c74 2069 7320 300d 0a20 2020 2020 2020  lt is 0..       
+00001410: 2074 6865 2066 756e 6374 696f 6e20 7265   the function re
+00001420: 7475 726e 7320 7468 6520 7361 6d65 2061  turns the same a
+00001430: 7267 2076 616c 7565 2061 7320 7479 7065  rg value as type
+00001440: 203c 696e 743e 200d 0a0d 0a20 2020 2020   <int> ....     
+00001450: 2020 2063 6d64 7320 3a0d 0a20 2020 2020     cmds :..     
+00001460: 2020 2020 2020 2031 2e20 7079 7468 6f6e         1. python
+00001470: 203c 5f5f 6669 6c65 5f5f 3e20 3130 0d0a   <__file__> 10..
+00001480: 2020 2020 2020 2020 2020 2020 322e 2070              2. p
+00001490: 7974 686f 6e20 3c5f 5f66 696c 655f 5f3e  ython <__file__>
+000014a0: 202d 696e 705f 696e 743d 3130 0d0a 2020   -inp_int=10..  
+000014b0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+000014c0: 2020 2072 6574 7572 6e20 696e 705f 696e     return inp_in
+000014d0: 740d 0a20 2020 200d 0a63 6c61 7373 2077  t..    ..class w
+000014e0: 6172 6e5f 776f 5f72 6574 5f74 7970 5f64  arn_wo_ret_typ_d
+000014f0: 6566 2861 7267 5f70 6172 7365 7229 3a0d  ef(arg_parser):.
+00001500: 0a0d 0a20 2020 2023 2065 7861 6d70 6c65  ...    # example
+00001510: 2070 6172 7365 5f61 7267 7320 7465 6d70   parse_args temp
+00001520: 6c61 7465 2066 756e 6374 696f 6e20 666f  late function fo
+00001530: 7220 6368 6563 6b69 6e67 2077 6172 6e69  r checking warni
+00001540: 6e67 730d 0a20 2020 2064 6566 2070 6172  ngs..    def par
+00001550: 7365 5f61 7267 7328 7365 6c66 2c20 0d0a  se_args(self, ..
+00001560: 2020 2020 2020 2020 2020 2020 696e 705f              inp_
+00001570: 626f 6f6c 293a 0d0a 2020 2020 2020 2020  bool):..        
+00001580: 2222 220d 0a20 2020 2020 2020 2069 6e70  """..        inp
+00001590: 5f62 6f6f 6c20 6973 2073 7065 6369 6669  _bool is specifi
+000015a0: 6564 2077 6974 6820 6e6f 2064 7479 7065  ed with no dtype
+000015b0: 206c 696d 6974 6174 696f 6e73 2061 7320   limitations as 
+000015c0: 7065 7220 6465 6669 6e69 7469 6f6e 0d0a  per definition..
+000015d0: 2020 2020 2020 2020 616e 7920 626f 6f6c          any bool
+000015e0: 2076 616c 7565 2063 616e 2062 6520 7061   value can be pa
+000015f0: 7373 6564 2066 6f72 2074 6865 2061 7267  ssed for the arg
+00001600: 756d 656e 740d 0a20 2020 2020 2020 2074  ument..        t
+00001610: 6865 2066 756e 6374 696f 6e20 7265 7475  he function retu
+00001620: 726e 7320 7468 6520 7361 6d65 2061 7267  rns the same arg
+00001630: 2076 616c 7565 0d0a 0d0a 2020 2020 2020   value....      
+00001640: 2020 636d 6473 203a 0d0a 2020 2020 2020    cmds :..      
+00001650: 2020 2020 2020 312e 2070 7974 686f 6e20        1. python 
+00001660: 3c5f 5f66 696c 655f 5f3e 2054 7275 650d  <__file__> True.
+00001670: 0a20 2020 2020 2020 2020 2020 2032 2e20  .            2. 
+00001680: 7079 7468 6f6e 203c 5f5f 6669 6c65 5f5f  python <__file__
+00001690: 3e20 2d69 6e70 5f62 6f6f 6c3d 5472 7565  > -inp_bool=True
+000016a0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000016b0: 2020 2020 2020 2072 6574 7572 6e20 696e         return in
+000016c0: 705f 626f 6f6c 0d0a 2020 2020 0d0a 636c  p_bool..    ..cl
+000016d0: 6173 7320 7761 726e 5f6e 6f5f 7375 7070  ass warn_no_supp
+000016e0: 6f72 745f 7479 705f 6172 6728 6172 675f  ort_typ_arg(arg_
+000016f0: 7061 7273 6572 293a 0d0a 0d0a 2020 2020  parser):....    
+00001700: 2320 6578 616d 706c 6520 7061 7273 655f  # example parse_
+00001710: 6172 6773 2074 656d 706c 6174 6520 6675  args template fu
+00001720: 6e63 7469 6f6e 2066 6f72 2063 6865 636b  nction for check
+00001730: 696e 6720 7761 726e 696e 6773 0d0a 2020  ing warnings..  
+00001740: 2020 6465 6620 7061 7273 655f 6172 6773    def parse_args
+00001750: 2873 656c 662c 200d 0a20 2020 2020 2020  (self, ..       
+00001760: 2020 2020 2069 6e70 5f64 663a 2070 642e       inp_df: pd.
+00001770: 4461 7461 4672 616d 6529 202d 3e20 4e6f  DataFrame) -> No
+00001780: 6e65 3a0d 0a20 2020 2020 2020 2022 2222  ne:..        """
+00001790: 0d0a 2020 2020 2020 2020 6578 616d 706c  ..        exampl
+000017a0: 6520 6465 6669 6e65 6420 666f 7220 6368  e defined for ch
+000017b0: 6563 6b69 6e67 2069 6620 6578 6365 7074  ecking if except
+000017c0: 696f 6e20 6973 2067 6574 7469 6e67 2072  ion is getting r
+000017d0: 6169 7365 642c 2077 696c 6c20 6e6f 7420  aised, will not 
+000017e0: 7265 7475 726e 2061 6e79 206f 7574 7075  return any outpu
+000017f0: 7420 6173 2074 6865 2064 6566 696e 6974  t as the definit
+00001800: 696f 6e20 6973 206e 6f74 2076 616c 6964  ion is not valid
+00001810: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00001820: 2020 2020 2020 2072 6574 7572 6e20 696e         return in
+00001830: 705f 6466 0d0a 2020 2020 0d0a 636c 6173  p_df..    ..clas
+00001840: 7320 7761 726e 5f6f 6e5f 6172 675f 6f72  s warn_on_arg_or
+00001850: 6465 7228 6172 675f 7061 7273 6572 293a  der(arg_parser):
+00001860: 0d0a 0d0a 2020 2020 2320 6578 616d 706c  ....    # exampl
+00001870: 6520 7061 7273 655f 6172 6773 2074 656d  e parse_args tem
+00001880: 706c 6174 6520 6675 6e63 7469 6f6e 2066  plate function f
+00001890: 6f72 2063 6865 636b 696e 6720 7761 726e  or checking warn
+000018a0: 696e 6773 0d0a 2020 2020 6465 6620 7061  ings..    def pa
+000018b0: 7273 655f 6172 6773 2873 656c 662c 200d  rse_args(self, .
+000018c0: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
+000018d0: 5f62 6f6f 6c31 3a20 626f 6f6c 2c20 696e  _bool1: bool, in
+000018e0: 705f 626f 6f6c 323a 2062 6f6f 6c29 202d  p_bool2: bool) -
+000018f0: 3e20 7475 706c 653a 0d0a 2020 2020 2020  > tuple:..      
+00001900: 2020 2222 220d 0a20 2020 2020 2020 2065    """..        e
+00001910: 7861 6d70 6c65 2064 6566 696e 6564 2066  xample defined f
+00001920: 6f72 2063 6865 636b 696e 6720 6966 2065  or checking if e
+00001930: 7863 6570 7469 6f6e 2069 7320 6765 7474  xception is gett
+00001940: 696e 6720 7261 6973 6564 2c20 696e 2073  ing raised, in s
+00001950: 6365 6e61 7269 6f73 2077 6865 7265 2061  cenarios where a
+00001960: 7267 756d 656e 7473 206f 7264 6572 2069  rguments order i
+00001970: 7320 6368 616e 6765 642e 0d0a 2020 2020  s changed...    
+00001980: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00001990: 2072 6574 7572 6e20 696e 705f 626f 6f6c   return inp_bool
+000019a0: 312c 2069 6e70 5f62 6f6f 6c32 0d0a 2020  1, inp_bool2..  
+000019b0: 2020 0d0a 636c 6173 7320 7761 726e 5f6f    ..class warn_o
+000019c0: 6e5f 756e 6465 665f 7061 7273 655f 6172  n_undef_parse_ar
+000019d0: 6773 2861 7267 5f70 6172 7365 7229 3a0d  gs(arg_parser):.
+000019e0: 0a0d 0a20 2020 2070 6173 73              ...    pass
```

### Comparing `py4cli-0.0.4/TESTS/test_basic_call.py` & `py4cli-0.0.5/TESTS/test_min_call.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import pytest
 
 #single args import 
-from scripts.basic_usage import single_int
-from scripts.basic_usage import single_float
-from scripts.basic_usage import single_str
-from scripts.basic_usage import single_list
-from scripts.basic_usage import single_tuple
-from scripts.basic_usage import single_set
-from scripts.basic_usage import single_dict
-from scripts.basic_usage import single_bool
-from scripts.basic_usage import multi_args
+from minimal_scripts.basic_usage import single_int
+from minimal_scripts.basic_usage import single_float
+from minimal_scripts.basic_usage import single_str
+from minimal_scripts.basic_usage import single_list
+from minimal_scripts.basic_usage import single_dict
+from minimal_scripts.basic_usage import single_bool
+from minimal_scripts.basic_usage import multi_args
 
 int_arg_vs_ret = [ 
     ("basic_usage.py -h".split(), None),
     ("basic_usage.py --help".split(), None),
     ("basic_usage.py".split(), 0),
     ("basic_usage.py 10".split(), 10),
     ("basic_usage.py -inp_int=10".split(), 10),
@@ -39,30 +37,14 @@
     ("basic_usage.py -h".split(), None),
     ("basic_usage.py --help".split(), None),
     ("basic_usage.py".split(), [None]),
     ("basic_usage.py ['Empty']".split(), ['Empty']),
     ("basic_usage.py -inp_list=['Empty']".split(), ['Empty']),
     ]
 
-tuple_arg_vs_ret = [ 
-    ("basic_usage.py -h".split(), None),
-    ("basic_usage.py --help".split(), None),
-    ("basic_usage.py".split(), (None,)),
-    ("basic_usage.py ('Empty',)".split(), ('Empty',)),
-    ("basic_usage.py -inp_tuple=('Empty',)".split(), ('Empty',)),
-    ]
-
-set_arg_vs_ret = [ 
-    ("basic_usage.py -h".split(), None),
-    ("basic_usage.py --help".split(), None),
-    ("basic_usage.py".split(), {None}),
-    ("basic_usage.py {'Empty'}".split(), {'Empty'}),
-    ("basic_usage.py -inp_set={'Empty'}".split(), {'Empty'}),
-    ]
-
 dict_arg_vs_ret = [ 
     ("basic_usage.py -h".split(), None),
     ("basic_usage.py --help".split(), None),
     ("basic_usage.py".split(), {None:None}),
     ("basic_usage.py {'Empty':'Empty'}".split(), {'Empty':'Empty'}),
     ("basic_usage.py -inp_dict={'Empty':'Empty'}".split(), {'Empty':'Empty'}),
     ]
@@ -79,66 +61,54 @@
     ("basic_usage.py -h".split(), None),
     ("basic_usage.py --help".split(), None),
     ("basic_usage.py".split(), {
                 'inp_int': 6,
                 'inp_float': 6.0,
                 'inp_str': 'Six',
                 'inp_list': [6, 6.0, "Six"],
-                'inp_tuple': (6, 6.0, "Six"),
-                'inp_set': {"Six"},
                 'inp_dict': {'int': 6, 'float': 6.0, 'str': "Six"},
                 'inp_bool': False
             }),
     ("basic_usage.py 10 10.0 Seven".split(), {
                 'inp_int': 10,
                 'inp_float': 10.0,
                 'inp_str': 'Seven',
                 'inp_list': [6, 6.0, "Six"],
-                'inp_tuple': (6, 6.0, "Six"),
-                'inp_set': {"Six"},
                 'inp_dict': {'int': 6, 'float': 6.0, 'str': "Six"},
                 'inp_bool': False
             }),
     ("basic_usage.py 10 10.0 Seven -inp_dict={'int':10,'float':10.0,'str':'Seven'}".split(), {
                 'inp_int': 10,
                 'inp_float': 10.0,
                 'inp_str': 'Seven',
                 'inp_list': [6, 6.0, "Six"],
-                'inp_tuple': (6, 6.0, "Six"),
-                'inp_set': {"Six"},
                 'inp_dict': {'int': 10, 'float': 10.0, 'str': "Seven"},
                 'inp_bool': False
             }),
-    ("basic_usage.py -inp_set={10,10.0,'Seven',10,10.0,'Seven'} -inp_dict={'int':10,'float':10.0,'str':'Seven'}".split(), {
+    ("basic_usage.py -inp_dict={'int':10,'float':10.0,'str':'Seven'}".split(), {
                 'inp_int': 6,
                 'inp_float': 6.0,
                 'inp_str': 'Six',
                 'inp_list': [6, 6.0, "Six"],
-                'inp_tuple': (6, 6.0, "Six"),
-                'inp_set': {10, 10.0, "Seven"},
                 'inp_dict': {'int': 10, 'float': 10.0, 'str': "Seven"},
                 'inp_bool': False
             }),
-    ("basic_usage.py 10 10.0 Seven [10,10.0,'Seven'] (10,10.0,'Seven') {10,10.0,'Seven'} {'int':10,'float':10.0,'str':'Seven'} True".split(), {
+    ("basic_usage.py 10 10.0 Seven [10,10.0,'Seven'] {'int':10,'float':10.0,'str':'Seven'} True".split(), {
                 'inp_int': 10,
                 'inp_float': 10.0,
                 'inp_str': 'Seven',
                 'inp_list': [10, 10.0, "Seven"],
-                'inp_tuple': (10, 10.0, "Seven"),
-                'inp_set': {10, 10.0, "Seven"},
                 'inp_dict': {'int': 10, 'float': 10.0, 'str': "Seven"},
                 'inp_bool': True
             }),
-    ("basic_usage.py -inp_int=10 -inp_float=10.0 -inp_str=Seven -inp_list=[10,10.0,'Seven'] -inp_tuple=(10,10.0,'Seven') -inp_set={10,10.0,'Seven'} -inp_dict={'int':10,'float':10.0,'str':'Seven'} -inp_bool=True".split(), {
+    ("basic_usage.py -inp_int=10 -inp_float=10.0 -inp_str=Seven -inp_list=[10,10.0,'Seven'] -inp_dict={'int':10,'float':10.0,'str':'Seven'} -inp_bool=True".split(), {
                 'inp_int': 10,
                 'inp_float': 10.0,
                 'inp_str': 'Seven',
                 'inp_list': [10, 10.0, "Seven"],
-                'inp_tuple': (10, 10.0, "Seven"),
-                'inp_set': {10, 10.0, "Seven"},
                 'inp_dict': {'int': 10, 'float': 10.0, 'str': "Seven"},
                 'inp_bool': True
             }),
     ]
 
 args_in = None
 OBJ = None
@@ -225,50 +195,14 @@
     returned = ret
 
     print("")
     if returned != OBJ.returned:
         print(f"{args_in} : Expected({returned}) != Actual({OBJ.returned})")
     else:
         print(f"{args_in} : Expected({returned}) == Actual({OBJ.returned})")
-    print("")
-
-@pytest.mark.parametrize("arg, ret", tuple_arg_vs_ret)
-def test_single_tuple(arg, ret):
-
-    global args_in
-    global OBJ
-    global returned
-
-    args_in = arg
-    OBJ = single_tuple(args_in)
-    returned = ret
-
-    print("")
-    if returned != OBJ.returned:
-        print(f"{args_in} : Expected({returned}) != Actual({OBJ.returned})")
-    else:
-        print(f"{args_in} : Expected({returned}) == Actual({OBJ.returned})")
-    print("")
-
-@pytest.mark.parametrize("arg, ret", set_arg_vs_ret)
-def test_single_set(arg, ret):
-
-    global args_in
-    global OBJ
-    global returned
-
-    args_in = arg
-    OBJ = single_set(args_in)
-    returned = ret
-
-    print("")
-    if returned != OBJ.returned:
-        print(f"{args_in} : Expected({returned}) != Actual({OBJ.returned})")
-    else:
-        print(f"{args_in} : Expected({returned}) == Actual({OBJ.returned})")
     print("")
 
 @pytest.mark.parametrize("arg, ret", dict_arg_vs_ret)
 def test_single_dict(arg, ret):
 
     global args_in
     global OBJ
```

### Comparing `py4cli-0.0.4/TESTS/test_basic_os.py` & `py4cli-0.0.5/TESTS/test_min_os.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,64 @@
+
 import pytest
 import os
 
 cmd_dict = {
     # int
-    'int_h': 'python scripts/use_int.py -h',
-    'int_help': 'python scripts/use_int.py --help',
-    'int': 'python scripts/use_int.py',
-    'int_args': 'python scripts/use_int.py 10',
-    'int_kwargs': 'python scripts/use_int.py -inp_int=10',
+    'min_int_h': 'python minimal_scripts/use_int.py -h',
+    'min_int_help': 'python minimal_scripts/use_int.py --help',
+    'min_int': 'python minimal_scripts/use_int.py',
+    'min_int_args': 'python minimal_scripts/use_int.py 10',
+    'min_int_kwargs': 'python minimal_scripts/use_int.py -inp_int=10',
 
     # float
-    'float_h': 'python scripts/use_float.py -h',
-    'float_help': 'python scripts/use_float.py --help',
-    'float': 'python scripts/use_float.py',
-    'float_args': 'python scripts/use_float.py 10.0',
-    'float_kwargs': 'python scripts/use_float.py -inp_float=10.0',
+    'min_float_h': 'python minimal_scripts/use_float.py -h',
+    'min_float_help': 'python minimal_scripts/use_float.py --help',
+    'min_float': 'python minimal_scripts/use_float.py',
+    'min_float_args': 'python minimal_scripts/use_float.py 10.0',
+    'min_float_kwargs': 'python minimal_scripts/use_float.py -inp_float=10.0',
 
     # str
-    'str_h': 'python scripts/use_str.py -h',
-    'str_help': 'python scripts/use_str.py --help',
-    'str': 'python scripts/use_str.py',
-    'str_args': 'python scripts/use_str.py hello',
-    'str_kwargs': 'python scripts/use_str.py -inp_str=hello',
+    'min_str_h': 'python minimal_scripts/use_str.py -h',
+    'min_str_help': 'python minimal_scripts/use_str.py --help',
+    'min_str': 'python minimal_scripts/use_str.py',
+    'min_str_args': 'python minimal_scripts/use_str.py hello',
+    'min_str_kwargs': 'python minimal_scripts/use_str.py -inp_str=hello',
 
     # list
-    'list_h': 'python scripts/use_list.py -h',
-    'list_help': 'python scripts/use_list.py --help',
-    'list': 'python scripts/use_list.py',
-    'list_args': 'python scripts/use_list.py [1,2,3]',
-    'list_kwargs': 'python scripts/use_list.py -inp_list=[1,2,3]',
-
-    # tuple
-    'tuple_h': 'python scripts/use_tuple.py -h',
-    'tuple_help': 'python scripts/use_tuple.py --help',
-    'tuple': 'python scripts/use_tuple.py',
-    'tuple_args': 'python scripts/use_tuple.py (1,2,3)',
-    'tuple_kwargs': 'python scripts/use_tuple.py -inp_tuple=(1,2,3)',
-
-    # set
-    'set_h': 'python scripts/use_set.py -h',
-    'set_help': 'python scripts/use_set.py --help',
-    'set': 'python scripts/use_set.py',
-    'set_args': 'python scripts/use_set.py {1,2,3,1,2,3}',
-    'set_kwargs': 'python scripts/use_set.py -inp_set={1,2,3,1,2,3}',
+    'min_list_h': 'python minimal_scripts/use_list.py -h',
+    'min_list_help': 'python minimal_scripts/use_list.py --help',
+    'min_list': 'python minimal_scripts/use_list.py',
+    'min_list_args': 'python minimal_scripts/use_list.py [1,2,3]',
+    'min_list_kwargs': 'python minimal_scripts/use_list.py -inp_list=[1,2,3]',
 
     # dict
-    'dict_h': 'python scripts/use_dict.py -h',
-    'dict_help': 'python scripts/use_dict.py --help',
-    'dict': 'python scripts/use_dict.py',
-    'dict_args': 'python scripts/use_dict.py {\'hello\':\'world\'}',
-    'dict_kwargs': 'python scripts/use_dict.py -inp_dict={\'hello\':\'world\'}',
+    'min_dict_h': 'python minimal_scripts/use_dict.py -h',
+    'min_dict_help': 'python minimal_scripts/use_dict.py --help',
+    'min_dict': 'python minimal_scripts/use_dict.py',
+    'min_dict_args': """python minimal_scripts/use_dict.py \"{'hello':'world'}\"""",
+    'min_dict_kwargs': """python minimal_scripts/use_dict.py -inp_dict=\"{'hello':'world'}\"""",
 
     # bool
-    'bool_h': 'python scripts/use_bool.py -h',
-    'bool_help': 'python scripts/use_bool.py --help',
-    'bool': 'python scripts/use_bool.py',
-    'bool_args': 'python scripts/use_bool.py True',
-    'bool_kwargs': 'python scripts/use_bool.py -inp_bool=True',
+    'min_bool_h': 'python minimal_scripts/use_bool.py -h',
+    'min_bool_help': 'python minimal_scripts/use_bool.py --help',
+    'min_bool': 'python minimal_scripts/use_bool.py',
+    'min_bool_args': 'python minimal_scripts/use_bool.py True',
+    'min_bool_kwargs': 'python minimal_scripts/use_bool.py -inp_bool=True',
 
     # multi-args
-    'multi_h': 'python scripts/multi_args.py -h',
-    'multi_help': 'python scripts/multi_args.py --help',
-    'multi': 'python scripts/multi_args.py',
-    'multi_args': 'python scripts/multi_args.py 10 10.0 Seven [10,10.0,\'Seven\'] (10,10.0,\'Seven\') {1,2,3,1,2,3} {\'int\':10,\'float\':10.0,\'str\':\'Seven\'} True',
-    'multi_kwargs': 'python scripts/multi_args.py -inp_int=10 -inp_float=10.0 -inp_str=Seven -inp_list=[10,10.0,\'Seven\'] -inp_tuple=(10,10.0,\'Seven\') -inp_set={1,2,3,1,2,3} -inp_dict={\'int\':10,\'float\':10.0,\'str\':\'Seven\'} -inp_bool=True',
-
-    'multi_mix1': 'python scripts/multi_args.py 10 10.0 Seven',
-    'multi_mix2': 'python scripts/multi_args.py 10 10.0 Seven -inp_dict={\'int\':10,\'float\':10.0,\'str\':\'Seven\'}',
-    'multi_mix3': 'python scripts/multi_args.py -inp_set={1,2,3,1,2,3} -inp_dict={\'int\':10,\'float\':10.0,\'str\':\'Seven\'}',
+    'min_multi_h': 'python minimal_scripts/multi_args.py -h',
+    'min_multi_help': 'python minimal_scripts/multi_args.py --help',
+    'min_multi': 'python minimal_scripts/multi_args.py',
+    'min_multi_args': """python minimal_scripts/multi_args.py 10 10.0 Seven \"[10,10.0,'Seven']\" \"{'int':10,'float':10.0,'str':'Seven'}\" True""",
+    'min_multi_kwargs': """python minimal_scripts/multi_args.py -inp_int=10 -inp_float=10.0 -inp_str=Seven -inp_list=\"[10,10.0,'Seven']\" -inp_dict=\"{'int':10,'float':10.0,'str':'Seven'}\" -inp_bool=True""",
+
+    'min_multi_mix1': 'python minimal_scripts/multi_args.py 10 10.0 Seven',
+    'min_multi_mix2': """python minimal_scripts/multi_args.py 10 10.0 Seven -inp_dict=\"{'int':10,'float':10.0,'str':'Seven'}\"""",
+    'min_multi_mix3': """python minimal_scripts/multi_args.py -inp_dict=\"{'int':10,'float':10.0,'str':'Seven'}\"""",
 }
 
 cmd_vs_out = [ tuple([v, f'{k}.txt']) for k, v in cmd_dict.items() ]
 
 cmd = None
 file = None
 
@@ -80,30 +67,35 @@
 
     global cmd
     global file
     
     yield
 
     if os.path.exists(f'ref_files/{file}'):
-        f1 = open(f'ref_files/{file}', 'r')
+        f1 = open(f'ref_files{os.sep}{file}', 'r')
         Ref_String = f1.read()
         f1.close()
 
-        f2 = open(f'res_files/{file}', 'r')
+        f2 = open(f'res_files{os.sep}{file}', 'r')
         Act_String = f2.read()
         f2.close()
-        assert(Ref_String == Act_String)
+        if file.endswith('_h.txt') or file.endswith('_help.txt'):
+            for inp, out in zip(Ref_String.splitlines(), Act_String.splitlines()):
+                if 'python' not in (inp+out):
+                    assert(inp == out)
+        else:
+            assert(Ref_String == Act_String)
 
 ##########################################################################################################
 ## Single condition based tests for Solver 
 ##########################################################################################################
 
 @pytest.mark.parametrize("args, fname", cmd_vs_out)
 def test_os_calls(args, fname):
 
     global cmd
     global file
     cmd = args
 
-    os.system(f"{cmd} > res_files/{fname}")
+    os.system(f"{cmd} > res_files{os.sep}{fname}")
 
     file = fname
```

### Comparing `py4cli-0.0.4/setup.py` & `py4cli-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="py4cli",
-    version="0.0.4",
+    version="0.0.5",
     description="python for command line interface development",
-    py_modules=["py4cli/minimal"],
+    py_modules=["py4cli/minimal", "py4cli/moderate"],
     package_dir={"": "SRCS"},
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

